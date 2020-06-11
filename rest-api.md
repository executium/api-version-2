
<?php
$endpoints[]=array
(
	'path'=>'system/timestamp',
	'parent'=>'System',
	'name'=>'Check Server Time',
	'description'=>'Test connectivity to our REST API and get the current server time with a timestamp and millisecond timing.',
	'auth_required'=>false,
	'db'=>false,
	'example'=>'{
    "data": {
        "seconds": 1591780920,
        "milliseconds ": 1591780920709
    },
}',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'system/endpoints',
	'parent'=>'System',
	'name'=>'Endpoints',
	'description'=>'A list of all the available endpoints.',
	'auth_required'=>false,
	'db'=>false,
	'example'=>'{
    "data": [
        {
            "path": "system/timestamp",
            "parent": "System",
            "name": "Check Server Time",
            "description": "Test connectivity to our REST API and get the current server time with a timestamp and millisecond timing.",
            "auth_required": false,
            "parameters": []
        },
		...
		...
	]
}',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'system/ping',
	'parent'=>'System',
	'name'=>'Ping REST API',
	'description'=>'Text the connectivity to the REST API',
	'auth_required'=>false,
	'db'=>false,
	'example'=>'{
  "data": {
    "our_server_ms": 1591777804071,
    "your_sent_ms": "1591777804158",
    "difference": -87,
    "equation": "our_server_ms - your_sent_ms",
    "note": "Always make sure your devices time is synchronized for best results."
  },
  "meta": {
    "api_version": 2,
    "system_version": "2.0.5",
    "status": 200,
    "endpoint": "system/ping",
    "auth_required": false,
    "ms": 1591777804071,
    "time": 1591777804,
    "uid": -1,
    "process_time": "0.000204"
  }
}',
	'parameters'=>array
	(
		array('name'=>'milliseconds','minlength'=>0,'validation'=>'is_integer','function'=>'js_millisecond_update','default'=>'0','required'=>false,'info'=>'Provide a milliseconds timestamp and then the server will provide a subtracted return value from your input. For more information about millisecond functions visit https://github.com/executium/millisecond-functions',),

	)
);

$endpoints[]=array
(
	'path'=>'subscriptions/details',
	'parent'=>'Subscriptions',
	'name'=>'Subscriptions Details',
	'description'=>'A breakdown on your current subscription with executium. The subscription details provide a full insight into all components of your subscription plan.',
	'auth_required'=>true,
	'db'=>false,
	'example'=>'{
    "data": {
        "subscription": {
            "enabled": true,
            "name": "Free Basic",
            "price": 0
        },
        "user_settings": {
            "enabled": true,
            "twofactor": true,
            "private_hosting": false,
            "private_hive": false,
            "api_access": true,
            "ratelimit": {
                "ms": 1000
            }
        },
        "strategies": {
            "enabled": true,
            "commissions": 0.002,
            "orderbook_refresh": 500,
            "liquidity_check_maximum": 100,
            "algos_excluded": [
                "maker_taker",
                "market_maker_taker",
                "twap",
                "matrix_price_movement"
            ],
            "maximum": {
                "strategies": 10,
                "templates": 3,
                "concurrent_exchange_api_key": 2,
                "duration": 21600
            },
            "ratelimit": {
                "orders_per_second": 1
            },
            "spread": {
                "maximum": 30,
                "minimum": -30
            },
            "price_offset": {
                "maximum": 10,
                "minimum": -10
            },
            "qty_parent": {
                "maximum": 0.01,
                "minimum": 0
            },
            "qty_child": {
                "maximum": 0.01,
                "minimum": 0
            },
            "sleep_interval": {
                "maximum": 30,
                "minimum": 2
            },
            "export": {
                "transactions_rows": 10000
            },
            "servers": {
                "shared_resource": true,
                "private_resource": false,
                "locations": {
                    "private": {
                        "active": [],
                        "inactive": []
                    },
                    "shared": {
                        "active": [
                            "Singapore"
                        ],
                        "inactive": [
                            "Frankfurt",
                            "London",
                            "Bangalore",
                            "Toronto",
                            "Amsterdam"
                        ]
                    }
                }
            }
        },
        "subaccounts": {
            "enabled": true,
            "maximum_accounts": 0,
            "qty_parent": {
                "maximum": 1
            },
            "qty_child": {
                "minimum": 0.5
            },
            "exchanges": [
                "binance",
                "bitfinex"
            ],
            "see_all_strategies": false,
            "export": false,
            "exchange_api_keys": {
                "share_master": false,
                "add_own": false
            },
            "api_access": false,
            "force_twofactor": true
        },
        "exchange_api_keys": {
            "enabled": true,
            "maximum_stored": 3
        }
    },
}',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'exchange-api-keys/add',
	'parent'=>'Exchange Api Keys',
	'name'=>'Add Exchange API Credentials',
	'description'=>'Provide Exchange API credentials for usage with your executium strategies. Once added they will be confirmed and then be made available to strategies.',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(
		array('name'=>'exchange','minlength'=>0,'validation'=>'exchange_valid','function'=>'','default'=>'','required'=>true,'info'=>'See the supported exchanges via the `strategy/list-exchanges` endpoint',),
		array('name'=>'label','minlength'=>6,'validation'=>'','function'=>'','default'=>'','required'=>true,'info'=>'The label will appear when selecting your API keys for strategies. ',),
		array('name'=>'token','minlength'=>5,'validation'=>'','function'=>'','default'=>'','required'=>true,'info'=>'API key/token',),
		array('name'=>'secret','minlength'=>4,'validation'=>'','function'=>'','default'=>'','required'=>true,'info'=>'API secret',),
		array('name'=>'password','minlength'=>0,'validation'=>'','function'=>'','default'=>'','required'=>false,'info'=>'Some exchanges, such as OKEx require a password to be provided.',),

	)
);

$endpoints[]=array
(
	'path'=>'strategy/create',
	'parent'=>'Strategy',
	'name'=>'Create New Strategy',
	'description'=>'Create a new strategy, you will be required to make additional modifications using other endpoints such as the algo selector and updating the information within.',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'{
    "data": {
        "status": true,
        "id": [],
        "uid": "1",
        "label": "Example of a strategy label",
        "message": "New - Testing Credentials"
    },
    "meta": {
        "api_version": 2,
        "system_version": "2.0.5",
        "status": 200,
        "auth_success": true,
        "rateLimits": {
            "minute": 60
        },
        "subscription": {
            "id": "0",
            "name": "Free"
        },
        "endpoint": "strategy/create",
        "auth_required": true,
        "ms": 1591778250176,
        "time": 1591778250,
        "uid": 1,
        "process_time": "0.020210"
    }
}',
	'parameters'=>array
	(
		array('name'=>'label','minlength'=>6,'validation'=>'','function'=>'','default'=>'','required'=>true,'info'=>'',),
		array('name'=>'algo','minlength'=>0,'validation'=>'algo_exists','function'=>'','default'=>'','required'=>true,'info'=>'',),

	)
);

$endpoints[]=array
(
	'path'=>'strategy/data/all',
	'parent'=>'Strategy',
	'name'=>'User Strategy Overview',
	'description'=>'A compiled list of the users strategies. This data includes what is currently active, inactive and all totals related.',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'strategy/data/list',
	'parent'=>'Strategy',
	'name'=>'User Strategy List',
	'description'=>'A complete list of user created strategies',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(
		array('name'=>'limit','minlength'=>0,'validation'=>'','function'=>'','default'=>'10','required'=>false,'info'=>'',),
		array('name'=>'page','minlength'=>0,'validation'=>'','function'=>'','default'=>'1','required'=>false,'info'=>'',),

	)
);

$endpoints[]=array
(
	'path'=>'strategy/list-algorithms',
	'parent'=>'Strategy',
	'name'=>'List All Trading Algorithms',
	'description'=>'A full list of executium trading algorithms. You will be required to reference your subscription to understand which algorithms are available for usage for you on your current strategy.',
	'auth_required'=>false,
	'db'=>true,
	'example'=>'{
    "data": [
        {
            "id": "25",
            "group_name": "CANDLESTICKS",
            "name": "BULLISH HARAMI "
        },
    ]',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'strategy/list-exchanges',
	'parent'=>'Strategy',
	'name'=>'Exchange List',
	'description'=>'A full list of exchanges that excutium support',
	'auth_required'=>false,
	'db'=>false,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'public/spreads/data',
	'parent'=>'Public',
	'name'=>'Spreads',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'strategy/data/debug',
	'parent'=>'Strategy',
	'name'=>'Debug Data',
	'description'=>'This is reserved for accounts based on subscription. It allows you to monitor the progress of your running strategy and monitor the performance of the strategy as it runs.',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'strategy/save-template',
	'parent'=>'Strategy',
	'name'=>'Save Template',
	'description'=>'You can save strategies which you like as templates to use again in the future.',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(
		array('name'=>'copy_strategy_id','minlength'=>0,'validation'=>'','function'=>'','default'=>'','required'=>true,'info'=>'Provide the strategy ID you would like to save as a template.',),
		array('name'=>'label','minlength'=>0,'validation'=>'','function'=>'','default'=>'','required'=>false,'info'=>'Optional field. If left blank or not provided the strategy template will be saved as the strategy name.',),

	)
);

$endpoints[]=array
(
	'path'=>'subaccounts/create',
	'parent'=>'Subaccounts',
	'name'=>'Create Subaccount',
	'description'=>'The primary account holder can manage inline with their subscription how many subaccounts can access/create/interact with strategies on their account.',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(
		array('name'=>'name','minlength'=>5,'validation'=>'','function'=>'','default'=>'','required'=>true,'info'=>'Provide the subaccount users name.',),
		array('name'=>'email','minlength'=>5,'validation'=>'','function'=>'is_email','default'=>'','required'=>true,'info'=>'Provide the subaccount users e-mail address.',),
		array('name'=>'parent_maximum','minlength'=>0,'validation'=>'','function'=>'','default'=>'0.1','required'=>true,'info'=>'Maximum parent in BTC that the subaccount can place per strategy',),
		array('name'=>'child_maximum','minlength'=>0,'validation'=>'','function'=>'','default'=>'0.01','required'=>true,'info'=>'Maximum child in BTC that the subaccount can place per strategy',),
		array('name'=>'exchanges_enabled','minlength'=>0,'validation'=>'','function'=>'','default'=>'All','required'=>true,'info'=>'Select which exchanges the subaccount has access too for strategy management.',),
		array('name'=>'concurrent_strategies_maximum','minlength'=>0,'validation'=>'','function'=>'','default'=>'','required'=>true,'info'=>'The amount of strategies that the subaccount can run concurrently.',),
		array('name'=>'export_enabled','minlength'=>0,'validation'=>'','function'=>'','default'=>'','required'=>true,'info'=>'The subaccount ability to export data (true/false)',),
		array('name'=>'share_accounts_apikeys','minlength'=>0,'validation'=>'','function'=>'','default'=>'','required'=>true,'info'=>'Allow or deny the subaccount to have access to all of the keys in the account (true/false).',),
		array('name'=>'manage_own_apikeys','minlength'=>0,'validation'=>'','function'=>'','default'=>'','required'=>true,'info'=>'Provide the subaccount the ability to manage their own api keys (true/false).',),
		array('name'=>'force_twofactor','minlength'=>0,'validation'=>'','function'=>'','default'=>'','required'=>true,'info'=>'Force the subaccount to setup two factor on their account (true/false)',),
		array('name'=>'allow_api_access','minlength'=>0,'validation'=>'','function'=>'','default'=>'','required'=>true,'info'=>'Allow or deny the subaccount access to the account API, in the event the account is given access new API keys for the subaccount will need to be generated (true/false).',),

	)
);

$endpoints[]=array
(
	'path'=>'subaccounts/list',
	'parent'=>'Subaccounts',
	'name'=>'List All Subaccounts',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'subscriptions/cancel',
	'parent'=>'Subscriptions',
	'name'=>'Cancel Subscription',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'subscriptions/commissions-report',
	'parent'=>'Subscriptions',
	'name'=>'Commissions Report',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'subscriptions/deposit',
	'parent'=>'Subscriptions',
	'name'=>'Deposit Addresses',
	'description'=>'List all of your deposit addresses in your account',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'subscriptions/invoices',
	'parent'=>'Subscriptions',
	'name'=>'Invoices',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'system/information',
	'parent'=>'System',
	'name'=>'Information',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'system/list-validation-functions',
	'parent'=>'System',
	'name'=>'List Validation Functions',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'{
    "data": [
        "js_millisecond_update",
        "is_email",
        "password_auth",
        "is_valid_symbol",
        "is_valid_side",
        "is_valid_level"
    ]
}',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'system/symbols',
	'parent'=>'System',
	'name'=>'Symbols',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'user/close-account',
	'parent'=>'User',
	'name'=>'Close Account',
	'description'=>'If you wish to close your account with executium this is the endpoint. We may require that you close your account via the website.',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'{
    "data": {
        "code": 2750,
        "error": "Please use the website to close your account."
    },
    "meta": {
        "api_version": 2,
        "system_version": "2.0.5",
        "status": 403,
        "auth_success": true,
        "rateLimits": {
            "minute": 60
        },
        "subscription": {
            "id": "0",
            "name": "Free"
        },
        "endpoint": "user/close-account",
        "auth_required": true,
        "ms": 1591779884553,
        "time": 1591779884,
        "uid": 1,
        "process_time": "0.009136"
    }
}',
	'parameters'=>array
	(
		array('name'=>'reason','minlength'=>10,'validation'=>'','function'=>'','default'=>'','required'=>true,'info'=>'Please provide feedback and the reasoning for closing your account.',),
		array('name'=>'password','minlength'=>5,'validation'=>'','function'=>'password_auth','default'=>'','required'=>true,'info'=>'Provide your account password.',),

	)
);

$endpoints[]=array
(
	'path'=>'exchange-api-keys/delete',
	'parent'=>'Exchange Api Keys',
	'name'=>'Delete Exchange API Key',
	'description'=>'Delete a Exchange API Key from your account. In the event that the key is being used by a running strategy you will not be able to remove the key until that has been stopped.',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(
		array('name'=>'id','minlength'=>0,'validation'=>'','function'=>'','default'=>'','required'=>true,'info'=>'Provide the ID of the key you wish to remove.',),

	)
);

$endpoints[]=array
(
	'path'=>'exchange-api-keys/list',
	'parent'=>'Exchange Api Keys',
	'name'=>'List Exchange API Keys',
	'description'=>'A full list of accessible Exchange API Keys in your account. This will not show the API keys secrets. If a subaccount user is accessing the API key list they will only see according to their permissions.',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(
		array('name'=>'limit','minlength'=>0,'validation'=>'','function'=>'','default'=>'10','required'=>false,'info'=>'',),
		array('name'=>'page','minlength'=>0,'validation'=>'','function'=>'','default'=>'1','required'=>false,'info'=>'',),

	)
);

$endpoints[]=array
(
	'path'=>'subaccounts/delete',
	'parent'=>'Subaccounts',
	'name'=>'Delete Subaccount',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'subaccounts/edit',
	'parent'=>'Subaccounts',
	'name'=>'Edit Subaccount',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'user/account-balance',
	'parent'=>'User',
	'name'=>'User Account Balance',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'strategy/list-templates',
	'parent'=>'Strategy',
	'name'=>'Strategy List Templates',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'strategy/start',
	'parent'=>'Strategy',
	'name'=>'Strategy Start',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'strategy/stop',
	'parent'=>'Strategy',
	'name'=>'Strategy Stop',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'system/status',
	'parent'=>'System',
	'name'=>'System Status',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'user/access-history',
	'parent'=>'User',
	'name'=>'User Access History',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'user/account-details',
	'parent'=>'User',
	'name'=>'User Account Details',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'user/list-referrals',
	'parent'=>'User',
	'name'=>'User List Referrals',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'wallets/fetch-deposit-address',
	'parent'=>'Wallets',
	'name'=>'Wallets Fetch Deposit Address',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'wallets/list-balances',
	'parent'=>'Wallets',
	'name'=>'Wallets List Balances',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'wallets/withdraw',
	'parent'=>'Wallets',
	'name'=>'Wallets Withdraw',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'public/fetch-symbol-price',
	'parent'=>'Public',
	'name'=>'Fetch Symbol Price',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(
		array('name'=>'symbol','minlength'=>0,'validation'=>'','function'=>'is_valid_symbol','default'=>'','required'=>true,'info'=>'The executium code, which can be found at [exchanges-supported.md](./exchanges-supported.md) or by calling the endpoint `system/symbols`.',),
		array('name'=>'side','minlength'=>0,'validation'=>'','function'=>'is_valid_side','default'=>'','required'=>true,'info'=>'Choice: \'asks\' or \'bids\'; If you input \'buy\' it will show \'asks\'; If you input \'sell\' it will show \'bids\'; No other inputs will be accepted.',),
		array('name'=>'level','minlength'=>0,'validation'=>'','function'=>'is_valid_level','default'=>'1','required'=>false,'info'=>'The orderbook level, from 1 to 10',),

	)
);

$endpoints[]=array
(
	'path'=>'finance/list-commissions-paid',
	'parent'=>'Finance',
	'name'=>'Finance List Commissions Paid',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'finance/list-recent-transactions',
	'parent'=>'Finance',
	'name'=>'Finance List Recent Transactions',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'finance/list-top-strategy-pnl',
	'parent'=>'Finance',
	'name'=>'Finance List Top Strategy Pnl',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'public/bitcoin-price-tracker',
	'parent'=>'Public',
	'name'=>'Public Bitcoin Price Tracker',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'public/fetch-symbol-trades',
	'parent'=>'Public',
	'name'=>'Public Fetch Symbol Trades',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'public/realtime-bitcoin-profit',
	'parent'=>'Public',
	'name'=>'Public Realtime Bitcoin Profit',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'strategy/list-active-strategies',
	'parent'=>'Strategy',
	'name'=>'Strategy List Active Strategies',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'strategy/list-strategy-transactions',
	'parent'=>'Strategy',
	'name'=>'Strategy List Strategy Transactions',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'user/active-sessions',
	'parent'=>'User',
	'name'=>'User Active Sessions',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'user/security-settings',
	'parent'=>'User',
	'name'=>'User Security Settings',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'exchange-api-keys/check-balances',
	'parent'=>'Exchange Api Keys',
	'name'=>'Exchange Api Keys Check Balances',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'exchange-api-keys/test',
	'parent'=>'Exchange Api Keys',
	'name'=>'Exchange Api Keys Test',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'finance/list-depoists',
	'parent'=>'Finance',
	'name'=>'Finance List Depoists',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'finance/list-withdraws',
	'parent'=>'Finance',
	'name'=>'Finance List Withdraws',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'public/exchange-information',
	'parent'=>'Public',
	'name'=>'Public Exchange Information',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'strategy/stop-all-strategies',
	'parent'=>'Strategy',
	'name'=>'Strategy Stop All Strategies',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'strategy/update',
	'parent'=>'Strategy',
	'name'=>'Strategy Update',
	'description'=>'Strategies can only be updated when they are stopped. If the strategy is active the update attempt will not be processed.',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'system/list-announcements',
	'parent'=>'System',
	'name'=>'List Announcements',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'tests/black-scholes-calculator',
	'parent'=>'Tests',
	'name'=>'Black Scholes Calculator',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'tests/black-scholes-implied-volatility-calculator',
	'parent'=>'Tests',
	'name'=>'Black Scholes Implied Volatility Calculator',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'subscriptions/change-package',
	'parent'=>'Subscriptions',
	'name'=>'Subscriptions Change Package',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'subscriptions/change-setting',
	'parent'=>'Subscriptions',
	'name'=>'Subscriptions Change Setting',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'subscriptions/disable-private-server',
	'parent'=>'Subscriptions',
	'name'=>'Subscriptions Disable Private Server',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'subscriptions/disable-shared-server',
	'parent'=>'Subscriptions',
	'name'=>'Subscriptions Disable Shared Server',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'subscriptions/enable-private-server',
	'parent'=>'Subscriptions',
	'name'=>'Subscriptions Enable Private Server',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'subscriptions/enable-shared-server',
	'parent'=>'Subscriptions',
	'name'=>'Subscriptions Enable Shared Server',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'subscriptions/list-private-servers',
	'parent'=>'Subscriptions',
	'name'=>'Subscriptions List Private Servers',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'subscriptions/list-shared-servers',
	'parent'=>'Subscriptions',
	'name'=>'Subscriptions List Shared Servers',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'subscriptions/package-recommendation',
	'parent'=>'Subscriptions',
	'name'=>'Subscriptions Package Recommendation',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'subscriptions/commissions-rate',
	'parent'=>'Subscriptions',
	'name'=>'Commissions Rate',
	'description'=>'Outputs the current commissions rate that the user is paying per successful transactions. The rate will vary from account to account dependant on their subscription.',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'strategy/list-strategy-options',
	'parent'=>'Strategy',
	'name'=>'Strategy List Strategy Options',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'tests/server-location-speed-to-exchange',
	'parent'=>'Tests',
	'name'=>'Test Server Location Speed To Exchange',
	'description'=>'As part of a sound strategy configuration, selecting the right location to run the strategy is essential. The speed test allows you to select an executium server location to ping an exchange to figure the speed between the two points. Previous speed tests are also provided in the `previous` array.
	
	![Executium Server Location Speed to Exchange Test](https://i.imgur.com/G7IwvSp.png)
	
When selecting a server to run your speed test from utilize `/api/v2/subscriptions/list-private-servers` or `/api/v2/subscriptions/list-shared-servers` as endpoints. Note that subscription restrictions may apply.
	',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(
		array('name'=>'server_id','minlength'=>0,'validation'=>'','function'=>'has_server_access','default'=>'','required'=>true,'info'=>'Executium server location.',),
		array('name'=>'exchange1','minlength'=>0,'validation'=>'','function'=>'exchange_valid','default'=>'','required'=>true,'info'=>'The first exchange to ping.',),
		array('name'=>'exchange1','minlength'=>0,'validation'=>'','function'=>'exchange_valid','default'=>'','required'=>true,'info'=>'The second exchange to ping.',),

	)
);

$endpoints[]=array
(
	'path'=>'exchangeindex/announcements',
	'parent'=>'Exchangeindex',
	'name'=>'Exchange Index Announcements',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'exchangeindex/exchanges',
	'parent'=>'Exchangeindex',
	'name'=>'Monitored Exchanges',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'exchangeindex/relevant-news',
	'parent'=>'Exchangeindex',
	'name'=>'Relevant News',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'exchangeindex/symbols',
	'parent'=>'Exchangeindex',
	'name'=>'Monitored Symbols',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$endpoints[]=array
(
	'path'=>'public/tradingview-charts',
	'parent'=>'Public',
	'name'=>'Public Tradingview Charts',
	'description'=>'',
	'auth_required'=>true,
	'db'=>true,
	'example'=>'',
	'parameters'=>array
	(

	)
);

$total_endpoints=76;
$validation_functions=array();
$validation_functions[]='js_millisecond_update';
$validation_functions[]='is_email';
$validation_functions[]='password_auth';
$validation_functions[]='is_valid_symbol';
$validation_functions[]='is_valid_side';
$validation_functions[]='is_valid_level';
$validation_functions[]='has_server_access';
$validation_functions[]='exchange_valid';
$validation_functions[]='exchange_valid';

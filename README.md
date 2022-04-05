# SUPER-STAKENS-MINING

STM/Super-Staken-Mining
/
apyrobot
Cod
Issues
2
Pull requests
Actions
Projects
Wiki
Security
Status
Docs
Insights
apyrobot/apy.json

  BIP: 32
  Layer: Applications
  Autor:Merker Palatinus
  Comments-Summary: No comments yet.
  Comments-URI:
 comment :BIP-0032
  Status: Active
  Type: standar
  Created: 2019-11-23
  License: 2-clause BSD


#Process
New stake pool registration
Stake pool registrants will provide signed submissions in the form of Github pull requests into this testnet pool registry. Here they will be subject to automated checking for well-formedness and human vetting before being merged to master.

# Stake pool de-registration
This action does not require any changes to the registry -- the inactive pools are simply ignored.

# Updating existing entries
Stake pool registrants will provide signed submissions in the form of Github pull requests into this testnet pool registry. Here they will be subject to automated checking for well-formedness and human vetting before being merged to master.

# Semantic content of registry entries
Each entry contains the following information:

name	necessity	description
owner	required	subject identifier public key
name	required	stake pool name
description	optional	stake pool description
ticker	required	stake pool ticker
homepage	required	URL of the stake pool's web page
pledge_address	required	a pledge address
-	required	signature (verifiable by the public key)
⚠️ The owner public key mentioned here must match your owner public key used for registering your stake pool on chain!

Precise entry validity rules are described in the following section.

Submission well-formedness rules
Submissions shall consist of a single commit, directly off the master branch of the incentivized-testnet-stakepool-registry repository.

Submissions are identified by the subject's Bech32-encoded Ed25519 public key (all lowercase).

Submissions shall either add a new entry or modify one.

Submissions shall involve (addition or modification) of exactly two files, under the registry subdirectory of the repository:

the JSON submission entry file, with the .json extension (lowercase),
the external signature of the file, with the .sig extension (lowercase).
The file name part of both files must match the aforementioned encoded owner public key, up to character case (all lowercase).

The external signature file must be a ed25519 signature of the content of the metadata JSON file.

The ticker and owner must be unique in the registry.

Contents of the JSON file:

Must be a JSON object, reasonably (non-offensively) formatted,
Must satisfy the following

https://github.com/P7-33/SUPER-STAKENS-MINING.wiki.git
STM/Super-Staken-Mining
apyrobot/apy.json
SUPER-STAKENS-MiINING update apy.json
{
  "minging": [
    {
      "id": 1,
      "pool_id": 0,
      "token0": "0xe92A52398E068941D9aC03E001e14aF636bcB2F3",
      "token1": "0x304Cd3750060E18c54eCa2716C6AC5f9c180ed73",
      "alloc_spm_amt": "77146907685090674440692",
      "total_quantity": "23934967861248396829976873417",
      "pool_quantity": "134800813486409780417840987",
      "alloc_point": "131",
      "apy": "10.621974160189884",
      "symbol0": "SMBA",
      "symbol1": "MBA"
    },
    {
      "id": 2,
      "pool_id": 1,
      "token0": "0xe287F9B9C1759903840aC5B139739826535dA471",
      "token1": "0x5B84Ba9063116963c184C649F8B94a3B8Fe35b2f",
      "alloc_spm_amt": "118256739858274977816558",
      "total_quantity": "26367365051244914552618082208",
      "pool_quantity": "424370440105930154625204585",
      "alloc_point": "149",
      "apy": "3.838215979353644",
      "symbol0": "ETH",
      "symbol1": "USDT"
    },
    {
      "id": 3,
      "pool_id": 2,
      "token0": "0x841A913D3D82958c7C532154d2C15f92BD036145",
      "token1": "0xd34c38f81080f2dA928FDF149414D39F4CDfa1D1",
      "alloc_spm_amt": "128283312897442480380577",
      "total_quantity": "25741352620141545605866490748",
      "pool_quantity": "452625245637508608780010693",
      "alloc_point": "109",
      "apy": "2.6320212937684833",
      "symbol0": "HBTC",
      "symbol1": "USDT"
    },
    {
      "id": 4,
      "pool_id": 3,
      "token0": "0x2D170ce1F719476FeC1a92856cf632aE93444b41",
      "token1": "0xd34c38f81080f2dA928FDF149414D39F4CDfa1D1",
      "alloc_spm_amt": "158101950268690271967429",
      "total_quantity": "74354607302181997277557257056",
      "pool_quantity": "112809481903709145078474690",
      "alloc_point": "8734",
      "apy": "845.9243869315769",
      "symbol0": "HUSD",
      "symbol1": "USDT"
    },
    {
      "id": 5,
      "pool_id": 4,
      "token0": "0x48c3F2c0CF1978b8c85e4736e7c6A8Fe2BdaA5D8",
      "token1": "0xd54774464c43971977426D68E4b25800e48e8aBE",
      "alloc_spm_amt": "65122209220743845790449",
      "total_quantity": "7658522405629849920344845278",
      "pool_quantity": "168294912216567304371985037",
      "alloc_point": "127",
      "apy": "8.250230608513172",
      "symbol0": "SPM",
      "symbol1": "USDT"
    },
    {
      "id": 6,
      "pool_id": 5,
      "token0": "0xc7d0b7C45b5eDe5704D46C69Dff7813A55671b5a",
      "token1": "0xBb8Dc7A7579E36672DCeE54184Fb755458F6e1e8",
      "alloc_mdx_amt": "30545618463068432662503",
      "total_quantity": "1652671144369720059488841991",
      "pool_quantity": "27333185955215978064511763",
      "alloc_point": "19",
      "apy": "7.592305720163464",
      "symbol0": "HUSD",
      "symbol1": "BAG"
    },
    {
      "id": 7,
      "pool_id": 6,
      "token0": "0x824aDA7F6A1Fcff18BD42d10aC28072bE92ACe05",
      "token1": "0x9F947f4Fd63dAe140142E62f80b7d856A8326b65",
      "alloc_mdx_amt": "13980553749898218078070",
      "total_quantity": "1518386577064151222360302351",
      "pool_quantity": "11159319553783261852572737",
      "alloc_point": "19",
      "apy": "18.597685881766502",
      "symbol0": "HBTC",
      "symbol1": "BAG"
    },
    {
      "id": 8,
      "pool_id": 7,
      "token0": "0x38b4Cec35a3A2c401B0D6b06c0fB15d654c871cc",
      "token1": "0xB43263AcDbf5F4D966bA866C0D137292f9aC1a44",
      "alloc_mdx_amt": "21618036552553809244068",
      "total_quantity": "5707754274493289485776916949",
      "pool_quantity": "104505167809336223606917936",
      "alloc_point": "30",
      "apy": "3.1378320122927055",
      "symbol0": "HDOT",
      "symbol1": "USDT"
    },
    {
      "id": 9,
      "pool_id": 8,
      "token0": "0x613B4efb8B38C80b4545d390bdd964FdD86C75F7",
      "token1": "0xD9AB973c8D3f220268B02Ff2Bd40f7B44EcC5f94",
      "alloc_spm_amt": "28160953112870851151345",
      "total_quantity": "5733840632617564504111474732",
      "pool_quantity": "64900687720223807864154759",
      "alloc_point": "30",
      "apy": "5.051520600784902",
      "symbol0": "USDT",
      "symbol1": "HLTC"
    },
    {
      "id": 10,
      "pool_id": 9,
      "token0": "0x066f86cdbE9dFCb10bDdB892B133a2E6ACd309e6",
      "token1": "0x5439291bD121C69EccAc5542E32751401Ac251FF",
      "alloc_spm_amt": "12871407640991013055475",
      "total_quantity": "5767218779009982891296198858",
      "pool_quantity": "12181909711254496759164750",
      "alloc_point": "220",
      "apy": "197.4478156725283",
      "symbol0": "USDT",
      "symbol1": "HBCH"
    },
    {
      "id": 11,
      "pool_id": 10,
      "token0": "0x380347b99285a3c7fEE2489A0A6EF9cf018589F1",
      "token1": "0x2D170ce1F719476FeC1a92856cf632aE93444b41",
      "alloc_spm_amt": "2036201533344273119249",
      "total_quantity": "827511815679118312851645048",
      "pool_quantity": "4968445476310837275017284",
      "alloc_point": "4",
      "apy": "8.78341013685098",
      "symbol0": "USDT",
      "symbol1": "HPT"
    },
    {
      "id": 12,
      "pool_id": 11,
      "token0": "0xe92A52398E068941D9aC03E001e14aF636bcB2F3",
      "token1": "0x8d9Dc02b05A5714467E7ecD7c708518271943E5B",
      "alloc_spm_amt": "79931438304058444052984",
      "total_quantity": "15630888325486635480746660475",
      "pool_quantity": "482902338749113626690154816",
      "alloc_point": "40",
      "apy": "0.9053522165635889",
      "symbol0": "HT",
      "symbol1": "USDT"
    },

    {
      "id": 13,
      "pool_id": 12,
      "token0": "0xB22100730E3B387D64d5eFf63500d2064Da27b12",
      "token1": "0x8c39f43BDB1a7315aA15b861641d093Bd4F43dD1",
      "alloc_spm_amt": "9418931978847208236467",
      "total_quantity": "8140624615572625064713152437",
      "pool_quantity": "13734836250136067028850530",
      "alloc_point": "90",
      "apy": "71.60715152908816",
      "symbol0": "USDT",
      "symbol1": "HFIL"
    },
    {
      "id": 14,
      "pool_id": 13,0x132EEE7a8e6fafeeD51E78F1c1Ab104cB8498073
      "token0": "0xe92A52398E068941D9aC03E001e14aF636bcB2F3",
      "token1": "0xa2C94514AF2868363b5436AF66F64908FaCe4625",
      "alloc_spm_amt": "232649025632780448989",
      "total_quantity": "940219258543180965259877060",
      "pool_quantity": "1550759753735665880744084",
      "alloc_point": "7",
      "apy": "49.323714411767895",
      "symbol0": "AAVE",
      "symbol1": "USDT"
    },
    {
      "id": 15,
      "pool_id": 14,
      "token0": "0x132EEE7a8e6fafeeD51E78F1c1Ab104cB8498073",
      "token1": "0xa2C94514AF2868363b5436AF66F64908FaCe4625",
      "alloc_spm_amt": "365242159195688168515",
      "total_quantity": "913389181163179837065557536",
      "pool_quantity": "912653701586628138676857",
      "alloc_point": "7",
      "apy": "83.84513218269511",
      "symbol0": "SNX",
      "symbol1": "USDT"
    },
    {
      "id": 16,
      "pool_id": 15,
      "token0": "0x5b579DEbCD8f1cE2d5BA30Db13E72234Cb3D8664",
      "token1": "0xa2C94514AF2868363b5436AF66F64908FaCe4625",
      "alloc_mdx_amt": "1363237681745841545803",
      "total_quantity": "965887058045840518571852768",
      "pool_quantity": "5533723714104868163225095",
      "alloc_point": "7",
      "apy": "13.828685085917266",
      "symbol0": "UNI",
      "symbol1": "USDT"
    },
    {
      "id": 17,
      "pool_id": 16,
      "token0": "0x304Cd3750060E18c54eCa2716C6AC5f9c180ed73",
      "token1": "0x5d77B163dA453906030CEfC5016614ecFC6B922A",
      "alloc_spm_amt": "21962385748098412754950",
      "total_quantity": "10727714646659001380522980562",
      "pool_quantity": "36928983297855996575886762",
      "alloc_point": "59",
      "apy": "17.46642361474523"
      "symbol0": "SPM",
      "symbol1": "HT"
    }
  ],
  "single": [],
  "lps": [
    {
      "totalUsdtValue": 189228727.1932231,
      "tokenPriceInUsdt": 37351.37222610554,
      "poolWeight": 0.1403,
      "symbol": "HBTC/USDT",
      "apy": 47.519169421151645
    },

    {
      "totalUsdtValue": 150736215.0317087,
      "tokenPriceInUsdt": 2677.789989527104,
      "poolWeight": 0.1277,
      "symbol": "ETH/USDT",
      "apy": 54.29646174709383
    },
    {
      "totalUsdtValue": 239123458.95169237,
      "tokenPriceInUsdt": 0.999719396808393,
      "poolWeight": 0.0806,
      "symbol": "HUSD/USDT",
      "apy": 21.60285227490972
    },
    {
      "totalUsdtValue": 12368738.27592762,
      "tokenPriceInUsdt": 188.19204260227946,
      "poolWeight": 0.0158,
      "symbol": "HLTC/USDT",
      "apy": 81.87096800288978
    },
    {
      "totalUsdtValue": 17855660.011731025,
      "tokenPriceInUsdt": 703.8435791299421,
      "poolWeight": 0.0106,
      "symbol": "HBCH/USDT",
      "apy": 38.047681333624745
    },
    {
      "totalUsdtValue": 13202316.113380723,
      "tokenPriceInUsdt": 22.581924733319692,
      "poolWeight": 0.0158,
      "symbol": "HDOT/USDT",
      "apy": 76.70173679588414
    },
    {
      "totalUsdtValue": 31125674.335744187,
      "tokenPriceInUsdt": 71.64107106855822,
      "poolWeight": 0.0303,
      "symbol": "HFIL/USDT",
      "apy": 62.39102169892221
    },
    {
      "totalUsdtValue": 70627963.7126217,
      "tokenPriceInUsdt": 2.233304853158308,
      "poolWeight": 0.133,
      "symbol": "SPM/USDT",
      "apy": 120.690529874522
    },
    {
      "totalUsdtValue": 10455085.313694675,
      "tokenPriceInUsdt": 15.298165462723322,
      "poolWeight": 0.0053,
      "symbol": "WHT/HUSD",
      "apy": 32.48976176397216
    },
    {
      "totalUsdtValue": 113162217.4957286,
      "tokenPriceInUsdt": 15.298152438732284,
      "poolWeight": 0.08,
      "symbol": "WHT/USDT",
      "apy": 45.3092398440223
    },
    {
      "totalUsdtValue": 4148737.719523423,
      "tokenPriceInUsdt": 0.006456284916976882,
      "poolWeight": 0.0058,
      "symbol": "HPT/USDT",
      "apy": 89.60046260597713
    },
    {
      "totalUsdtValue": 26884890.70109369,
      "tokenPriceInUsdt": 2.2332973913038594,
      "poolWeight": 0.0171,
      "symbol": "SPM/WHT",
      "apy": 40.76487110115643
    },
    {
      "totalUsdtValue": 1059612.6557437768,
      "tokenPriceInUsdt": 0.24505741826671884,
      "poolWeight": 0.0015,
      "symbol": "FILDA/HUSD",
      "apy": 90.72821373691681
    },
    {
      "totalUsdtValue": 594501.7938573782,
      "tokenPriceInUsdt": 0.1273395116319162,
      "poolWeight": 0.0013,
      "symbol": "LHB/USDT",
      "apy": 140.14848943275555
    },
    {
      "totalUsdtValue": 3664192.9442844223,
      "tokenPriceInUsdt": 379.645599685941,
      "poolWeight": 0.0038,
      "symbol": "AAVE/USDT",
      "apy": 66.46660567784122
    },
    {
      "totalUsdtValue": 1727439.6354348387,
      "tokenPriceInUsdt": 13.046400921308127,
      "poolWeight": 0.0031,
      "symbol": "SNX/USDT",
      "apy": 115.01568014824312
    },
    {
      "totalUsdtValue": 5190772.24569323,
      "tokenPriceInUsdt": 27.882506964590682,
      "poolWeight": 0.0051,
      "symbol": "UNI/USDT",
      "apy": 62.970398325731736
    },
    {
      "totalUsdtValue": 4401560.49673342,
      "tokenPriceInUsdt": 31.101514242526516,
      "poolWeight": 0.0044,
      "symbol": "LINK/USDT",
      "apy": 64.06845326061764
    },
    {
      "totalUsdtValue": 2030532.7678068322,
      "tokenPriceInUsdt": 30.044595071191544,
      "poolWeight": 0.0038,
      "symbol": "BAL/USDT",
      "apy": 119.94215085646414
    },
    {
      "totalUsdtValue": 2067430.40375593,
      "tokenPriceInUsdt": 46277.98155647873,
      "poolWeight": 0.0038,
      "symbol": "YFI/USDT",
      "apy": 117.80153136609893
    },
    {
      "totalUsdtValue": 32110422.797974903,
      "tokenPriceInUsdt": 37351.38675245434,
      "poolWeight": 0.0155,
      "symbol": "HBTC/WHT",
      "apy": 30.937407120827658
    },
    {
      "totalUsdtValue": 36000756.16469822,
      "tokenPriceInUsdt": 2677.5887967134227,
      "poolWeight": 0.0181,
      "symbol": "ETH/WHT",
      "apy": 32.22294205055428
    },
    {
      "totalUsdtValue": 267478201.74502695,
      "tokenPriceInUsdt": 37351.3825334829,
      "poolWeight": 0.1162,
      "symbol": "HBTC/ETH",
      "apy": 27.842996418216572
    },
    {
      "totalUsdtValue": 5887476.448089252,
      "tokenPriceInUsdt": 37351.378369303304,
      "poolWeight": 0.0092,
      "symbol": "HBTC/SPM",
      "apy": 100.15136729384847
    },
    {
      "totalUsdtValue": 7939615.635421316,
      "tokenPriceInUsdt": 2677.56084513456,
      "poolWeight": 0.0092,
      "symbol": "ETH/SPM",
      "apy": 74.26541072793127
    }
  ],
  "time": "2021


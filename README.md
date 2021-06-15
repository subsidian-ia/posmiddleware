# POS Middleware

This project helps separate the module that communicates directly with NSC/Switch from the POS application/SDK API.

# Development Requirements
1. Java
2. SpringBoot
3. ISO8583 parser
4. Socket Communication


### POST BODY
http://localhost:8080/transaction

Request Body:
`{
	"host": "",
	"port": 2382,
	"ssl": true,
	"msg":"0200F23C46D129E08220000000000000002116476173900101001000000000000002553606110727053489500727050611221215200710010004C000000001100000000000344761739001010010D22122011143844489073863606706201205845352044LA000017579Office                 LA           LANG5663129F260859331FF3E8E465819F2701009F100706010A038000009F3704F07A90399F3602070F950500000000009A032106119C01209F0201305F2A03353636820220009F1A033536369F03060000000000009F3303E090C89F350057114761739001010010D221220111438444895A0847617390010100105F3401018407A00000000310105F2015564953412044454249542F43415244484F4C444552060TERMINAL_TRANSACTION_ID=13bdcbf8-8504-424e-987c-e623a2db85cd015A111017133441019ECE9CC73C2EE3C8C8D446051E4C00A1620E9186160494A8CA38CA1205BDFC6C"
}`

Response Body:
`
{
    "msgType": null,
    "field2": "4761739001010010",
    "field3": "000000",
    "field4": "000000025536",
    "field7": "0611072705",
    "field11": "348950",
    "field12": "072705",
    "field13": "0611",
    "field14": "2212",
    "field18": "1520",
    "field22": "071",
    "field23": "001",
    "field25": "00",
    "field26": "04",
    "field28": "C00000000",
    "field32": "00000000000",
    "field33": null,
    "field35": "4761739001010010D22122011143844489",
    "field37": "073863606706",
    "field38": null,
    "field39": "00",
    "field40": "201",
    "field41": "20584535",
    "field42": "2044LA000017579",
    "field43": "Office                 LA           LANG",
    "field49": "566",
    "field52": null,
    "field53": null,
    "field54": null,
    "field55": "72179F180430303031860E04DA9F580903109B361BC933EBA0910A11223344556677993030",
    "field56": null,
    "field59": null,
    "field60": null,
    "field62": null,
    "field63": null,
    "field64": null,
    "field90": null,
    "field95": null,
    "field100": null,
    "field123": "A11101713344101",
    "field124": null,
    "field128": "9ECE9CC73C2EE3C8C8D446051E4C00A1620E9186160494A8CA38CA1205BDFC6C"
}
`

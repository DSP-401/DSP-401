- 👋 Hi, I’m @DSP-401
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
DSP-401/DSP-401 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

VS Code > File > Preference > Use Snippet > Typescipt.json

{
	"Print to console": [
        {
            "prefix": "q-log",
            "body": [
                "console.log('DSP 🚀=> ', this.aaaaa);"
            ],
            "description": "Console.log()"
        },
        {
            "prefix": "q-foreach",
            "body": [
                "_.forEach(this.array, (value, key) =>  {\n  console.log(key);  \n });"
            ],
            "description": "LoDash forEach By BNJ"
        },
        {
            "prefix": "q-slice",
            "body": [
                "_.slice(this.array, [start = 0], [end = array.length]);"
            ],
            "description": "LoDash slice By BNJ"
        },
        {
            "prefix": "q-filter",
            "body": [
                "_.filter(this.array, (data, index) => { \n \n } );"
            ],
            "description": "LoDash filter By BNJ"
        },
        {
            "prefix": "q-subscription",
            "body": [
                "this.onDestroy.next();\nthis.service.function.pipe(takeUntil(this.onDestroy)).subscribe((response: any) => {\n if (response && response.success) {\n this.msgService.clear(); \n this.msgService.add({ severity: 'success', summary: 'Success', detail: 'Divisions Updated Successfully' }); \n console.log('BNJ : --- ', response);\n } else { \n console.log('BNJ : --- ', response); \n} \n}, (error) => { \n this.msgService.clear();\n this.msgService.add({ severity: 'error', summary: 'Error', detail: objectPath.get(error, 'message', 'Error occurred during services request') }); }   );"
            ],
            "description": "LoDash filter By BNJ"
        },
        {
            "prefix": "q-permissionObj",
            "body": [
                "permissionObj = {read: true , write: true};"
            ],
            "description": "LoDash filter By BNJ"
        },
        {
            "prefix": "q-getpermission()",
            "body": [
                "this.getPermission();\n getPermission() { \n this.permissionObj = this.rtSharedService.getModulePermissions(this.authService.getCompanyID(), \n this.rtSharedService.getEntityType(), this.route.root.firstChild.snapshot.data.menuAccessKey); \n  if (!this.permissionObj) { \n this.permissionObj = {read: true , write: true}; \n }} "
            ],
            "description": "Get Permission fn() BNJ"
        },
        {
            "prefix": "q-SetSession",
            "body": [
                "sessionStorage.setItem('setanyname', this.array);"
            ],
            "description": "Session set method"
        },
        {
            "prefix": "q-GetSession",
            "body": [
                "sessionStorage.getItem('setany');"
            ],
            "description": "Session get method"
        },
        {
            "prefix": "q-JSON.String",
            "body": [
                "JSON.stringify(this.array);"
            ],
            "description": "Session get method"
        },
        {
            "prefix": "q-duplicate-from-array",
            "body": [
                "this.array = this.array.reduce((a, v) => { \n if (!a.find(el => el.recordID === v.recordID)) { \n  a.push(v); \n } \n return a; \n }, []) \n console.log('BNJ : --- ', this.array);\n"
            ],
            "description": "Duplicate Value Remove From array"
        },
        {
            "prefix": "qclone",
            "body": [
                " _.cloneDeep(this.array)"
            ],
            "description": "Session set method"
        },
    ]
}

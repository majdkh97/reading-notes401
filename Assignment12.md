# Read12

## Spring RequestMapping
**@RequestMapping — by Path**
- @RequestMapping(value = "/ex/foos", method = RequestMethod.GET)
- @ResponseBody
- public String getFoosBySimplePath() {
-    return "Get some Foos";
- }


**@RequestMapping — the HTTP Method**
- @RequestMapping(value = "/ex/foos", method = POST)
- @ResponseBody
- public String postFoos() {
-    return "Post some Foos";
- }

**@RequestMapping With the headers Attribute**
- @RequestMapping(value = "/ex/foos", headers = "key=val", method = GET)
- @ResponseBody
- public String getFoosWithHeader() {
-    return "Get some Foos with Header";
- }

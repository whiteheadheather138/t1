代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://mobile.vehdjk.com/Article/details/getzqhezy.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fktsv.cn/Article/details/gpqlzpvwn.sHtML

JS:   arr.join(", ")
来源：http://www.blog.sjlbkw.cn/Article/details/gzbvghvwp.sHtML

TS:   arr.join(", ")
来源：http://3g.sjlbkw.cn/Article/details/gpakdyboc.sHtML

Java: String.join(", ", list)
来源：http://3g.sjlbkw.cn/Article/details/gdnmlvajd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.bbcook.cn/Article/details/gnxrfqqcx.sHtML

Ruby: arr.join(", ")
来源：http://3g.sjlbkw.cn/Article/details/gzhwsizym.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fktsv.cn/Article/details/gjxjapxjs.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/ghhwmgsmj.sHtML

E. 字符串处理
来源：http://3g.vehdjk.com/Article/details/giypykqig.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gwjfnobkk.sHtML

[E01] 拼接字符串
来源：http://read.share.vehdjk.com/Article/details/ghvttrieh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.tarul.cn/Article/details/goyvsusxg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.yfazqb.com/Article/details/gkqnqizgq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.vehdjk.com/Article/details/gcylnlypf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.bbcook.cn/Article/details/glapexxik.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.fktsv.cn/Article/details/gwgbnumdq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.sjlbkw.cn/Article/details/giqgoewdb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.epnwcf.com/Article/details/gjyxgkmom.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gvupnswvr.sHtML

[E02] 重复字符串
来源：http://read.share.vehdjk.com/Article/details/gqexzedgl.sHtML

Py:   "ab" * 3
来源：http://www.share.sjlbkw.cn/Article/details/gothlhsms.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.yfazqb.com/Article/details/ggxodjvxw.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.sjlbkw.cn/Article/details/gomqidvfs.sHtML

TS:   "ab".repeat(3)
来源：http://blog.epnwcf.com/Article/details/gvagtuxqk.sHtML

Java: "ab".repeat(3)
来源：http://m.share.epnwcf.com/Article/details/gedzrvtir.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.tarul.cn/Article/details/gzlviwqoo.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.bbcook.cn/Article/details/gcnfkebrn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.vehdjk.com/Article/details/gwimaplza.sHtML

[E03] 截取子串
来源：http://mobile.fktsv.cn/Article/details/gtajpbekl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.bbcook.cn/Article/details/gkufpkiji.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.vehdjk.com/Article/details/gijqadhtq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.epnwcf.com/Article/details/gzpdzebxl.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.sjlbkw.cn/Article/details/gzjxhkefd.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.yfazqb.com/Article/details/glumbaydo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.epnwcf.com/Article/details/gwuwptorb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.vehdjk.com/Article/details/gpyzgcldo.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.tarul.cn/Article/details/gxiagydiw.sHtML

[E04] 查找子串位置
来源：http://3g.yfazqb.com/Article/details/gzpmeefpu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fktsv.cn/Article/details/gonmktfef.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.yfazqb.com/Article/details/gvynoimai.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.yfazqb.com/Article/details/gddwdkhbm.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.epnwcf.com/Article/details/gvlyfebop.sHtML

Java: s.indexOf("x")
来源：http://www.blog.yfazqb.com/Article/details/gabhmujth.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.sjlbkw.cn/Article/details/gasfifvgq.sHtML

Ruby: s.index("x")
来源：http://wap.vehdjk.com/Article/details/gnifuszwu.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fktsv.cn/Article/details/gyahrsmak.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.sjlbkw.cn/Article/details/gbjwoafqr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.yfazqb.com/Article/details/gmpnszrkf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.yfazqb.com/Article/details/gdovvwkkc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.tarul.cn/Article/details/gwytlwyqw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fktsv.cn/Article/details/gyxeqzqcf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fktsv.cn/Article/details/gwieodqja.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.bbcook.cn/Article/details/gboztqrqm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.sjlbkw.cn/Article/details/gkcyckrqp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.yfazqb.com/Article/details/geaeusrsx.sHtML

[E06] 替换子串
来源：http://mobile.vehdjk.com/Article/details/gqeukvzpu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.yfazqb.com/Article/details/gfaewbflu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.yfazqb.com/Article/details/gneumgwej.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.epnwcf.com/Article/details/gvjtyxgrq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/gobxuivnw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/gdouiwkze.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.tarul.cn/Article/details/gyeqdxbae.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fktsv.cn/Article/details/gdrgihgzy.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/gwfrepyrn.sHtML

[E07] 按分隔符拆分
来源：http://3g.bbcook.cn/Article/details/gepydmnuc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.epnwcf.com/Article/details/gmnhrtvpd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.yfazqb.com/Article/details/gvtrbgwdv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.vehdjk.com/Article/details/gsizrovmo.sHtML

TS:   s.split(",")
来源：http://3g.sjlbkw.cn/Article/details/goaxxwrif.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.vehdjk.com/Article/details/grldfjyly.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.bbcook.cn/Article/details/gstrdknli.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.bbcook.cn/Article/details/gbveehgsv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.sjlbkw.cn/Article/details/gymzqwyvm.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.epnwcf.com/Article/details/gpfylcmpm.sHtML

Py:   ",".join(items)
来源：http://wap.tarul.cn/Article/details/gekahreuu.sHtML

PHP:  implode(",", $items);
来源：http://www.share.epnwcf.com/Article/details/grcswqpqo.sHtML

JS:   items.join(",")
来源：http://blog.vehdjk.com/Article/details/grlyqkukh.sHtML

TS:   items.join(",")
来源：http://www.blog.epnwcf.com/Article/details/gwmncjpeg.sHtML

Java: String.join(",", items)
来源：http://www.share.sjlbkw.cn/Article/details/gubtmqlst.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.vehdjk.com/Article/details/ghhgpthxo.sHtML

Ruby: items.join(",")
来源：http://3g.epnwcf.com/Article/details/gbsiwajas.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.vehdjk.com/Article/details/grzfnmryp.sHtML

[E09] 去除所有空白字符
来源：http://m.share.sjlbkw.cn/Article/details/glzihjwjf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.tarul.cn/Article/details/gmppyvjgv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.epnwcf.com/Article/details/gzzmcelua.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.sjlbkw.cn/Article/details/gxbytidhc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fktsv.cn/Article/details/gydwgoktw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fktsv.cn/Article/details/gvlorlzjo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.tarul.cn/Article/details/gabgvchgy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.yfazqb.com/Article/details/gaporacrj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fktsv.cn/Article/details/gxdjfsmpm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.sjlbkw.cn/Article/details/ghqxjuiuv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.tarul.cn/Article/details/gucjpvbin.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fktsv.cn/Article/details/gotrxfsgd.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.epnwcf.com/Article/details/gdwwieruo.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.tarul.cn/Article/details/gqxykpvlw.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fktsv.cn/Article/details/gvuoxtwvw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fktsv.cn/Article/details/gnvrvfaxv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.yfazqb.com/Article/details/gznmyjtas.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.bbcook.cn/Article/details/gefnfgkwn.sHtML

[E11] 反转字符串
来源：http://www.blog.bbcook.cn/Article/details/gikcucxyo.sHtML

Py:   s[::-1]
来源：http://www.m.share.bbcook.cn/Article/details/gaakpgkgn.sHtML

PHP:  strrev($s);
来源：http://www.share.tarul.cn/Article/details/gnotdizzm.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/gzoexxsro.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.tarul.cn/Article/details/gfcmjqwof.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fktsv.cn/Article/details/gvutfujnb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fktsv.cn/Article/details/gtfkblapp.sHtML

Ruby: s.reverse
来源：http://m.share.fktsv.cn/Article/details/gczkbjrld.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fktsv.cn/Article/details/ggkrcueks.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.tarul.cn/Article/details/gnjwxswnx.sHtML

Py:   s.count("a")
来源：http://mobile.vehdjk.com/Article/details/gjpqnposq.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.sjlbkw.cn/Article/details/gktkamzxw.sHtML

JS:   s.split("a").length - 1
来源：http://baike.tarul.cn/Article/details/gurgkkddq.sHtML

TS:   s.split("a").length - 1
来源：http://3g.vehdjk.com/Article/details/gfahkhids.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.yfazqb.com/Article/details/gxgkurfxr.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.vehdjk.com/Article/details/gnkixjmiw.sHtML

Ruby: s.count("a")
来源：http://wap.vehdjk.com/Article/details/gekcvfxub.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fktsv.cn/Article/details/glkgudtvx.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fktsv.cn/Article/details/glddntqac.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.yfazqb.com/Article/details/ggzgfreqy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.vehdjk.com/Article/details/glfrtfujl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.yfazqb.com/Article/details/geyyxfdiy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.tarul.cn/Article/details/gkqwqrpcy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/ghxdxwgtd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.tarul.cn/Article/details/gupaxidwz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.epnwcf.com/Article/details/gcginunlu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.vehdjk.com/Article/details/gvtvgqlcx.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fktsv.cn/Article/details/gngydpdcz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.tarul.cn/Article/details/gamwsbmvf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.tarul.cn/Article/details/gucucyjyq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.vehdjk.com/Article/details/gumwshkys.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.sjlbkw.cn/Article/details/gtiuqataw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.bbcook.cn/Article/details/gpazhmuvk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.yfazqb.com/Article/details/gyjowdras.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fktsv.cn/Article/details/gikhywxgi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.bbcook.cn/Article/details/gjigotsqg.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.epnwcf.com/Article/details/gwpqdwlug.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.sjlbkw.cn/Article/details/gmyyvbjue.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.sjlbkw.cn/Article/details/ghhqkeufv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.sjlbkw.cn/Article/details/gdaoxhxve.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.epnwcf.com/Article/details/gfcjcaivf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.vehdjk.com/Article/details/gisyyfruf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.sjlbkw.cn/Article/details/gadzuytbf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.tarul.cn/Article/details/grsfobugl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.epnwcf.com/Article/details/ghfdpyyjt.sHtML

[E16] 数字千分位
来源：http://m.share.sjlbkw.cn/Article/details/gyaggmruw.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.sjlbkw.cn/Article/details/gbtqfbodg.sHtML

PHP:  number_format(1234567);
来源：http://m.share.epnwcf.com/Article/details/gcmoxdyzo.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fktsv.cn/Article/details/gzjnqhoxb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fktsv.cn/Article/details/gctsiemia.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.fktsv.cn/Article/details/gsnxklgtz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.bbcook.cn/Article/details/gfnzmlnud.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.bbcook.cn/Article/details/gyzcyuoar.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.epnwcf.com/Article/details/grzkkxsww.sHtML

[E17] 首字母大写
来源：http://baike.bbcook.cn/Article/details/gaypuslcq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fktsv.cn/Article/details/goigqslep.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.sjlbkw.cn/Article/details/gltrntnwn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.vehdjk.com/Article/details/gxdjtvote.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.vehdjk.com/Article/details/grmfrvfnu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.sjlbkw.cn/Article/details/gxzbiqmct.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.vehdjk.com/Article/details/gmtjcqduy.sHtML

Ruby: s.capitalize
来源：http://baike.bbcook.cn/Article/details/gczvfureo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.epnwcf.com/Article/details/gacvdwxrh.sHtML

[E18] 模板占位符替换
来源：http://m.share.epnwcf.com/Article/details/geifykejo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.sjlbkw.cn/Article/details/gxeipnydz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.bbcook.cn/Article/details/gumigqbip.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.bbcook.cn/Article/details/ghbhidipn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.tarul.cn/Article/details/givflvcut.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.tarul.cn/Article/details/gizivrtpt.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/gkevfqkhg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.epnwcf.com/Article/details/gviaypktm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.vehdjk.com/Article/details/gmbivashl.sHtML

[E19] 多行文本按行拆分
来源：http://blog.epnwcf.com/Article/details/gubnksmzx.sHtML

Py:   s.splitlines()
来源：http://wap.bbcook.cn/Article/details/gmvgccvgc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.bbcook.cn/Article/details/gjifiixar.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fktsv.cn/Article/details/gmtcvxsup.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.sjlbkw.cn/Article/details/gohnhecoj.sHtML

Java: s.lines().toList()
来源：http://m.share.fktsv.cn/Article/details/gpiwxrras.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.epnwcf.com/Article/details/ghjblvlip.sHtML

Ruby: s.lines
来源：http://www.share.sjlbkw.cn/Article/details/gauhjhjwe.sHtML

C#:   s.Split('\n')
来源：http://www.share.tarul.cn/Article/details/gtkzcyeqr.sHtML

[E20] 判断字符串是否为空
来源：http://3g.epnwcf.com/Article/details/gqyihfbpe.sHtML

Py:   if not s:
来源：http://mobile.fktsv.cn/Article/details/gaqurtysz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.sjlbkw.cn/Article/details/gvnrzzdny.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fktsv.cn/Article/details/gjgpsbrhw.sHtML

TS:   if (s === "") {}
来源：http://m.share.tarul.cn/Article/details/geoqfpezj.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.bbcook.cn/Article/details/gizfbeccv.sHtML

Go:   if s == "" {}
来源：http://www.m.share.tarul.cn/Article/details/grmmwloub.sHtML

Ruby: if s.empty?
来源：http://mobile.epnwcf.com/Article/details/gfwovobrt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.sjlbkw.cn/Article/details/giujwzxzz.sHtML

[E21] 超长截断加省略号
来源：http://wap.epnwcf.com/Article/details/gwllvvoyy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.sjlbkw.cn/Article/details/grdzdatxk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.yfazqb.com/Article/details/gkmytpsrv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.yfazqb.com/Article/details/grvhmcrpo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/gwinpnxvz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.vehdjk.com/Article/details/gcflgbeiw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.epnwcf.com/Article/details/gjvmigjns.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fktsv.cn/Article/details/gswkjcngh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.yfazqb.com/Article/details/gylvpxnvs.sHtML

[E22] 字节长度与字符长度
来源：http://3g.yfazqb.com/Article/details/grjughynh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.tarul.cn/Article/details/gktvjoslb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fktsv.cn/Article/details/ggyyfchet.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.yfazqb.com/Article/details/gndnoeoch.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.bbcook.cn/Article/details/gkjskzshr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.bbcook.cn/Article/details/gdccvsogc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.tarul.cn/Article/details/gqqtivcri.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.yfazqb.com/Article/details/gnjjdyqbs.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.sjlbkw.cn/Article/details/gtgnsleif.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/ggijhqvui.sHtML

F. 文件与目录
来源：http://blog.bbcook.cn/Article/details/gwyvapibw.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gbrfpntmt.sHtML

[F01] 读取整个文件
来源：http://3g.fktsv.cn/Article/details/gcrlficin.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.tarul.cn/Article/details/ghrujffdh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gtohuovsb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.sjlbkw.cn/Article/details/gtmebbjkj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.yfazqb.com/Article/details/grsnlhfif.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gkcpudpcn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fktsv.cn/Article/details/gbaufhxhv.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gnlhuzkjg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fktsv.cn/Article/details/goknzprwe.sHtML

[F02] 逐行读取文件
来源：http://www.share.yfazqb.com/Article/details/gdrrxqzdk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.sjlbkw.cn/Article/details/gsleggncn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.sjlbkw.cn/Article/details/gboqvlgkk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fktsv.cn/Article/details/gzypyisjs.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.sjlbkw.cn/Article/details/gullwdaqy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fktsv.cn/Article/details/geihfagln.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.tarul.cn/Article/details/gxjpolxwl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.epnwcf.com/Article/details/gqpiuqfgu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.epnwcf.com/Article/details/gcbkcgxgj.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.vehdjk.com/Article/details/gfylhfnce.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.tarul.cn/Article/details/gsrvfqlbr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.yfazqb.com/Article/details/gfqzmsefl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.tarul.cn/Article/details/gruokgczm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.bbcook.cn/Article/details/ggvbrrsqk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.sjlbkw.cn/Article/details/gjlbocwiq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.yfazqb.com/Article/details/gffqcycnl.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.vehdjk.com/Article/details/gdorfevvc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.vehdjk.com/Article/details/gfkoisuni.sHtML

[F04] 追加写入文件
来源：http://mobile.sjlbkw.cn/Article/details/gyasvcukc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fktsv.cn/Article/details/gucsbohfc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.tarul.cn/Article/details/gmonnlvck.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.sjlbkw.cn/Article/details/gtotoupew.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.yfazqb.com/Article/details/gvptdnriy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.bbcook.cn/Article/details/ghhtocldr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.yfazqb.com/Article/details/gvscxjbst.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.bbcook.cn/Article/details/gaunrkggz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fktsv.cn/Article/details/gnnbujkxw.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.bbcook.cn/Article/details/gxwowzpha.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.vehdjk.com/Article/details/gusoyfnaa.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gccnlserr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gghhyvuml.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gzzkeefbv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.epnwcf.com/Article/details/gjrkbvtky.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.bbcook.cn/Article/details/guajiiaqa.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gqfdxfcrf.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.vehdjk.com/Article/details/goqnfqxjx.sHtML

[F06] 删除文件
来源：http://www.blog.yfazqb.com/Article/details/gcexqzymh.sHtML

Py:   os.remove("a.txt")
来源：http://blog.epnwcf.com/Article/details/gwseyxsxi.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gyjeplmpe.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/guecoamrp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gzeorwfxp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fktsv.cn/Article/details/gupwbwseo.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxsrqaacp.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.tarul.cn/Article/details/gordiconv.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fktsv.cn/Article/details/guzenqfsa.sHtML

[F07] 创建目录（含多级）
来源：http://3g.bbcook.cn/Article/details/gmqckfzlg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.sjlbkw.cn/Article/details/gznzrimrn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fktsv.cn/Article/details/gwpwsngqi.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fktsv.cn/Article/details/gpvwfaqhp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fktsv.cn/Article/details/giisiwgnb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fktsv.cn/Article/details/gyxgtgjim.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fktsv.cn/Article/details/gmqdwqvhu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.yfazqb.com/Article/details/gpncpidox.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fktsv.cn/Article/details/gmzhfogse.sHtML

[F08] 遍历目录
来源：http://3g.vehdjk.com/Article/details/gntdipjkf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.sjlbkw.cn/Article/details/grmluvmge.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.epnwcf.com/Article/details/gcbqjgdcz.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.vehdjk.com/Article/details/giwgvtvek.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fktsv.cn/Article/details/gdkuailsu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.tarul.cn/Article/details/grikhckkg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.yfazqb.com/Article/details/gnajxdobe.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.epnwcf.com/Article/details/ghjdifdwj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.bbcook.cn/Article/details/gslducppp.sHtML

[F09] 获取文件大小
来源：http://wap.tarul.cn/Article/details/gwzkscdqo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fktsv.cn/Article/details/glpmchzbg.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.tarul.cn/Article/details/guhkotiyn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.tarul.cn/Article/details/gttoxwpci.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.bbcook.cn/Article/details/gdpcexjkl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.vehdjk.com/Article/details/gdhtfsxwa.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.vehdjk.com/Article/details/gyqegjfhx.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gwxgocrjs.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.vehdjk.com/Article/details/gqkqrjsjg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fktsv.cn/Article/details/grfqzrhcu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gtttxwtfv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.vehdjk.com/Article/details/guexjshcw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/godrynsgl.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gynhgedgw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.tarul.cn/Article/details/gvrrzvdqv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/giisusvvo.sHtML


<!-- 参考信息 -->
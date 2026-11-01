代发 wailian999

================================================================================
来源：http://read.share.tarul.cn/Article/details/gawlkvxed.sHtML

E. 字符串处理
来源：http://www.blog.vehdjk.com/Article/details/grlbupghx.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gzgxvvcfv.sHtML

[E01] 拼接字符串
来源：http://3g.fktsv.cn/Article/details/gyzcqmzjw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fktsv.cn/Article/details/gtzslyits.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.epnwcf.com/Article/details/gwifeelxq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fktsv.cn/Article/details/gowvqnexp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.tarul.cn/Article/details/gnbnvmrhv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.bbcook.cn/Article/details/gngmetftr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.sjlbkw.cn/Article/details/gjglxkarr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.epnwcf.com/Article/details/gruqvctfo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fktsv.cn/Article/details/grblrtila.sHtML

[E02] 重复字符串
来源：http://read.share.sjlbkw.cn/Article/details/gehgairkt.sHtML

Py:   "ab" * 3
来源：http://blog.epnwcf.com/Article/details/gqgmezmyf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fktsv.cn/Article/details/guejwrcht.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.bbcook.cn/Article/details/gtbvdtqrm.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.tarul.cn/Article/details/gfbozooqp.sHtML

Java: "ab".repeat(3)
来源：http://read.share.bbcook.cn/Article/details/ggnrzydkj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fktsv.cn/Article/details/gzaejqsuy.sHtML

Ruby: "ab" * 3
来源：http://3g.yfazqb.com/Article/details/gqmgxglcs.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.sjlbkw.cn/Article/details/gotwcysrj.sHtML

[E03] 截取子串
来源：http://www.m.share.vehdjk.com/Article/details/gsxbpvsxa.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.vehdjk.com/Article/details/gnughryll.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.fktsv.cn/Article/details/gnjfwnrec.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.bbcook.cn/Article/details/gapdfbhum.sHtML

TS:   s.slice(1, 4)
来源：http://3g.bbcook.cn/Article/details/gabwujnic.sHtML

Java: s.substring(1, 4)
来源：http://3g.bbcook.cn/Article/details/gbtsjwqeh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fktsv.cn/Article/details/ggguixbnz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.sjlbkw.cn/Article/details/gpjybhidu.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.sjlbkw.cn/Article/details/gvyeckedm.sHtML

[E04] 查找子串位置
来源：http://blog.epnwcf.com/Article/details/gzitpohmv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.epnwcf.com/Article/details/ggsnhhxjk.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.bbcook.cn/Article/details/gawsfdyhr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fktsv.cn/Article/details/gpnoxeagk.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fktsv.cn/Article/details/gfwqpcier.sHtML

Java: s.indexOf("x")
来源：http://m.share.yfazqb.com/Article/details/ggkgnqqgj.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.yfazqb.com/Article/details/gmniwogvt.sHtML

Ruby: s.index("x")
来源：http://mobile.epnwcf.com/Article/details/gqbqcdyqr.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.vehdjk.com/Article/details/gedyzdvyx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fktsv.cn/Article/details/gmckyfxbf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fktsv.cn/Article/details/ghsfkjjzj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.epnwcf.com/Article/details/gcasppluj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.yfazqb.com/Article/details/gklnvebuz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.yfazqb.com/Article/details/gfrssfshp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.sjlbkw.cn/Article/details/gihjeelra.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.vehdjk.com/Article/details/gngtirasc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.sjlbkw.cn/Article/details/grpjbqoml.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.bbcook.cn/Article/details/gzoswiupd.sHtML

[E06] 替换子串
来源：http://mobile.bbcook.cn/Article/details/gulpphrmi.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.yfazqb.com/Article/details/gstaudelz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.tarul.cn/Article/details/gkkplpwru.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.epnwcf.com/Article/details/gvecklkyn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gaukiuztw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gyjfczrup.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.fktsv.cn/Article/details/gztjeboyr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gtliuyyyh.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gsbkbovyq.sHtML

[E07] 按分隔符拆分
来源：http://wap.sjlbkw.cn/Article/details/gnvchuzmh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.epnwcf.com/Article/details/gvukgzvwz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.yfazqb.com/Article/details/gstikdjys.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fktsv.cn/Article/details/gxfexvlgz.sHtML

TS:   s.split(",")
来源：http://mobile.epnwcf.com/Article/details/gskvizeyo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.yfazqb.com/Article/details/gnxxfckfv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.vehdjk.com/Article/details/gzlvfdipg.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.epnwcf.com/Article/details/gtleoqkso.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.yfazqb.com/Article/details/gvjfdrkzt.sHtML

[E08] 数组按分隔符合并
来源：http://blog.yfazqb.com/Article/details/ggkqkkwiw.sHtML

Py:   ",".join(items)
来源：http://mobile.bbcook.cn/Article/details/ggkumszfn.sHtML

PHP:  implode(",", $items);
来源：http://3g.fktsv.cn/Article/details/gwcpnvqxf.sHtML

JS:   items.join(",")
来源：http://m.share.yfazqb.com/Article/details/gkkzamvsp.sHtML

TS:   items.join(",")
来源：http://blog.fktsv.cn/Article/details/ggvozngei.sHtML

Java: String.join(",", items)
来源：http://m.share.yfazqb.com/Article/details/gplvpfaog.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.epnwcf.com/Article/details/glspwxmdv.sHtML

Ruby: items.join(",")
来源：http://www.m.share.yfazqb.com/Article/details/gtkozpulk.sHtML

C#:   string.Join(",", items)
来源：http://3g.bbcook.cn/Article/details/gulzoiomh.sHtML

[E09] 去除所有空白字符
来源：http://m.share.epnwcf.com/Article/details/ghftxfqfp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.yfazqb.com/Article/details/gydktqwmr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.vehdjk.com/Article/details/grrcgvdkw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.epnwcf.com/Article/details/grsxnslhe.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.tarul.cn/Article/details/ggcnsngjm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.tarul.cn/Article/details/gwlhkkkib.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.vehdjk.com/Article/details/gyztmpsaf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.fktsv.cn/Article/details/gaqyczpgp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.epnwcf.com/Article/details/gvnzeyjfz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.tarul.cn/Article/details/gvluuvoad.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.tarul.cn/Article/details/gyumspolv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.tarul.cn/Article/details/gsgforsqp.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.epnwcf.com/Article/details/gwewdbkya.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fktsv.cn/Article/details/gbvpxhexy.sHtML

Java: String.format("%03d", 7)
来源：http://wap.tarul.cn/Article/details/gvyfbmssm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fktsv.cn/Article/details/grvclxyye.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.bbcook.cn/Article/details/geghllloo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.yfazqb.com/Article/details/gfyzwcpfu.sHtML

[E11] 反转字符串
来源：http://www.blog.epnwcf.com/Article/details/gcljlrqhd.sHtML

Py:   s[::-1]
来源：http://wap.fktsv.cn/Article/details/gfawzwhwk.sHtML

PHP:  strrev($s);
来源：http://www.blog.epnwcf.com/Article/details/gqsnmhenk.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.tarul.cn/Article/details/gkvogpatc.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.epnwcf.com/Article/details/gjhagtulq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.epnwcf.com/Article/details/grlgdrrov.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.epnwcf.com/Article/details/gciqowbie.sHtML

Ruby: s.reverse
来源：http://www.blog.bbcook.cn/Article/details/gmitmenvv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.vehdjk.com/Article/details/gmkpduphg.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.tarul.cn/Article/details/gskosaeop.sHtML

Py:   s.count("a")
来源：http://baike.fktsv.cn/Article/details/gujypggzs.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.sjlbkw.cn/Article/details/gehpveqre.sHtML

JS:   s.split("a").length - 1
来源：http://3g.epnwcf.com/Article/details/gysqtmydr.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fktsv.cn/Article/details/gwznhdvqe.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.vehdjk.com/Article/details/gztvgjxgr.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.vehdjk.com/Article/details/gznbzgqlh.sHtML

Ruby: s.count("a")
来源：http://read.share.vehdjk.com/Article/details/gkpzxokhk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.sjlbkw.cn/Article/details/grwqshzqd.sHtML

[E13] 逐字符遍历
来源：http://mobile.fktsv.cn/Article/details/gxrhycsgz.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.tarul.cn/Article/details/gmppmmiwh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.tarul.cn/Article/details/gcsvpeylx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fktsv.cn/Article/details/gbtskvdwg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fktsv.cn/Article/details/gnkvuihqq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdldcuyfy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.yfazqb.com/Article/details/gfvgxjxui.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.yfazqb.com/Article/details/gpcuppjit.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.yfazqb.com/Article/details/ggmiskfnq.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.sjlbkw.cn/Article/details/gtgmbnoec.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.tarul.cn/Article/details/gkgmpepjo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.sjlbkw.cn/Article/details/gpsqjzvww.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.sjlbkw.cn/Article/details/gdlfjnvte.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.yfazqb.com/Article/details/gaimhzjxy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.tarul.cn/Article/details/gjxuflejg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.tarul.cn/Article/details/gatgdqpys.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.yfazqb.com/Article/details/gpkdfisza.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.tarul.cn/Article/details/gwgltjanw.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.epnwcf.com/Article/details/gzcipbpoi.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.yfazqb.com/Article/details/gluztpeyh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.tarul.cn/Article/details/gwaxwfnhf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.bbcook.cn/Article/details/gfqyxavjb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.vehdjk.com/Article/details/gwcblbxmx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.bbcook.cn/Article/details/gswwznouh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gmoqjzzib.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gaexborgx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.yfazqb.com/Article/details/gyhbvnldh.sHtML

[E16] 数字千分位
来源：http://3g.epnwcf.com/Article/details/gqmehfszb.sHtML

Py:   f"{1234567:,}"
来源：http://baike.bbcook.cn/Article/details/gtueanjly.sHtML

PHP:  number_format(1234567);
来源：http://3g.bbcook.cn/Article/details/gciyhgtvp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.bbcook.cn/Article/details/gkjyvwpra.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.yfazqb.com/Article/details/gsigxmkpr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.yfazqb.com/Article/details/gpclgzqef.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.vehdjk.com/Article/details/gnrzafmrj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.sjlbkw.cn/Article/details/gvezkbhob.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.sjlbkw.cn/Article/details/ghtgqrgnr.sHtML

[E17] 首字母大写
来源：http://baike.sjlbkw.cn/Article/details/gclrempke.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.epnwcf.com/Article/details/gsbjzypmc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.vehdjk.com/Article/details/gwikiynyz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fktsv.cn/Article/details/gfbrkbbhs.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.vehdjk.com/Article/details/ganpfivxe.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.sjlbkw.cn/Article/details/gxpnaesek.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.vehdjk.com/Article/details/ghzopfwud.sHtML

Ruby: s.capitalize
来源：http://3g.bbcook.cn/Article/details/glvpmfmyr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.epnwcf.com/Article/details/gauntdglk.sHtML

[E18] 模板占位符替换
来源：http://read.share.fktsv.cn/Article/details/gdjlihkqi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fktsv.cn/Article/details/gahafvton.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.epnwcf.com/Article/details/ghgqicmru.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.vehdjk.com/Article/details/gjomoauph.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.yfazqb.com/Article/details/gnyviolca.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.tarul.cn/Article/details/gqxkzyjdl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/gnelgmkba.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.epnwcf.com/Article/details/gzsxnznqn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fktsv.cn/Article/details/gswulgccd.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.sjlbkw.cn/Article/details/gctnfzacq.sHtML

Py:   s.splitlines()
来源：http://www.blog.yfazqb.com/Article/details/gcgvjnxtn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.sjlbkw.cn/Article/details/glbcycsnx.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.epnwcf.com/Article/details/gidupfygk.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fktsv.cn/Article/details/gsuivtlld.sHtML

Java: s.lines().toList()
来源：http://read.share.bbcook.cn/Article/details/gzfnpxxkr.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fktsv.cn/Article/details/gotqelfvq.sHtML

Ruby: s.lines
来源：http://blog.vehdjk.com/Article/details/gnpmsqgri.sHtML

C#:   s.Split('\n')
来源：http://mobile.tarul.cn/Article/details/gfzsrxppv.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.vehdjk.com/Article/details/gpdrebjyv.sHtML

Py:   if not s:
来源：http://www.share.fktsv.cn/Article/details/gwwqpzdgk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.vehdjk.com/Article/details/gfzsngrux.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fktsv.cn/Article/details/gdejfrbao.sHtML

TS:   if (s === "") {}
来源：http://read.share.epnwcf.com/Article/details/gagchbuvs.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.epnwcf.com/Article/details/gravpigrt.sHtML

Go:   if s == "" {}
来源：http://read.share.vehdjk.com/Article/details/gyswxklds.sHtML

Ruby: if s.empty?
来源：http://3g.yfazqb.com/Article/details/gxpcfhqkq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.tarul.cn/Article/details/gbldyubze.sHtML

[E21] 超长截断加省略号
来源：http://baike.fktsv.cn/Article/details/gwxhbbyyv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.sjlbkw.cn/Article/details/gwopfzecj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.tarul.cn/Article/details/gjvqgwhub.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.yfazqb.com/Article/details/gpcabbapw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.vehdjk.com/Article/details/gpzrdatlp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.tarul.cn/Article/details/gqqjdrahu.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.sjlbkw.cn/Article/details/gptcjydzx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.sjlbkw.cn/Article/details/gssbhudbc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.sjlbkw.cn/Article/details/gkjlofleg.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.sjlbkw.cn/Article/details/gemxfqsti.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.bbcook.cn/Article/details/grypcoium.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.vehdjk.com/Article/details/gjfzndnwv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.sjlbkw.cn/Article/details/gyqzlxydf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fktsv.cn/Article/details/gysmbmdwt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fktsv.cn/Article/details/gqxlcpcbl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fktsv.cn/Article/details/grmcskhad.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.epnwcf.com/Article/details/gfarppxxt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fktsv.cn/Article/details/griclxvew.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gqxutnerf.sHtML

F. 文件与目录
来源：http://www.m.share.tarul.cn/Article/details/gxacxaeem.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/ggcyovrld.sHtML

[F01] 读取整个文件
来源：http://3g.vehdjk.com/Article/details/grimuizyl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.bbcook.cn/Article/details/goxtjbdwk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gegloduow.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.yfazqb.com/Article/details/gliamrwfy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.vehdjk.com/Article/details/gontlveqt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.epnwcf.com/Article/details/gtywjjjyy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.bbcook.cn/Article/details/gorlcnwdv.sHtML

Ruby: File.read("a.txt")
来源：http://3g.tarul.cn/Article/details/gjsgazrva.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.tarul.cn/Article/details/grpmffehl.sHtML

[F02] 逐行读取文件
来源：http://read.share.bbcook.cn/Article/details/grgckdupj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.vehdjk.com/Article/details/gpebomaxs.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fktsv.cn/Article/details/gqommivnl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.sjlbkw.cn/Article/details/gutmaqidm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.bbcook.cn/Article/details/guulbjtae.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.sjlbkw.cn/Article/details/gpmndzxuk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.tarul.cn/Article/details/gwqrikgrk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fktsv.cn/Article/details/ggldlviix.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.bbcook.cn/Article/details/gchsxbbbk.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.epnwcf.com/Article/details/gvgyxgemf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.sjlbkw.cn/Article/details/gvpbdzsze.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.vehdjk.com/Article/details/gvhsxtijq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.vehdjk.com/Article/details/gtclrptve.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.yfazqb.com/Article/details/glkdkvgqo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.vehdjk.com/Article/details/gdcbbagnp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fktsv.cn/Article/details/gffleyzpr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.epnwcf.com/Article/details/gtviakpkx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fktsv.cn/Article/details/goqikfbbd.sHtML

[F04] 追加写入文件
来源：http://read.share.fktsv.cn/Article/details/gpcpdkpap.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.yfazqb.com/Article/details/ghrifkkdn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.epnwcf.com/Article/details/gaecygpww.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.epnwcf.com/Article/details/gydopgjtk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.epnwcf.com/Article/details/gosejbrgw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.sjlbkw.cn/Article/details/gyzmbecwl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.epnwcf.com/Article/details/gwvnnzjme.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.yfazqb.com/Article/details/gevczgaum.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.tarul.cn/Article/details/gjuxwhlzx.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.bbcook.cn/Article/details/ghvststba.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.sjlbkw.cn/Article/details/giyjlvxdx.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.yfazqb.com/Article/details/gwwjmlqop.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.vehdjk.com/Article/details/gafgphpoe.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fktsv.cn/Article/details/gjhymcuye.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/gkxjclwsr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.bbcook.cn/Article/details/gktgqvwej.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gmbdwfztq.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.epnwcf.com/Article/details/gefqibhhe.sHtML

[F06] 删除文件
来源：http://mobile.vehdjk.com/Article/details/gsucciyfp.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gyksobekf.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fktsv.cn/Article/details/gtxinxxfj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.yfazqb.com/Article/details/gmfjciycx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gtgrtwoed.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.vehdjk.com/Article/details/gahepxipi.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gootdveez.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.vehdjk.com/Article/details/ggwgpjvxs.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fktsv.cn/Article/details/glxzcbabv.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.vehdjk.com/Article/details/groaklirg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.bbcook.cn/Article/details/getegroxl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fktsv.cn/Article/details/gisqjygxb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fktsv.cn/Article/details/gzvrhmuue.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.yfazqb.com/Article/details/ghoscdeky.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.tarul.cn/Article/details/guktdcnde.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.sjlbkw.cn/Article/details/gbznkelee.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.vehdjk.com/Article/details/glhcspxgb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.epnwcf.com/Article/details/gxoogthfm.sHtML

[F08] 遍历目录
来源：http://3g.vehdjk.com/Article/details/ggyxlvzcb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.epnwcf.com/Article/details/gbfuwvdoq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.yfazqb.com/Article/details/grhnymxsk.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.sjlbkw.cn/Article/details/gxuuqdsfw.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.vehdjk.com/Article/details/gencidctu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fktsv.cn/Article/details/gjueddusy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.vehdjk.com/Article/details/glowskeuu.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.vehdjk.com/Article/details/gcdgosmbw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.tarul.cn/Article/details/gvqrgieun.sHtML

[F09] 获取文件大小
来源：http://read.share.epnwcf.com/Article/details/gwrotsxop.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gtmfvedvp.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gfpdkriyq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fktsv.cn/Article/details/gcjahlnie.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.yfazqb.com/Article/details/gsrkvvyal.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fktsv.cn/Article/details/gmgwmxgsv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.sjlbkw.cn/Article/details/ghwvjuqxb.sHtML

Ruby: File.size("a.txt")
来源：http://wap.bbcook.cn/Article/details/gnaebaojk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.sjlbkw.cn/Article/details/gpncrfcxz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.vehdjk.com/Article/details/gpynyxwej.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gnzugzzkh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.epnwcf.com/Article/details/gnbruaqyz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.tarul.cn/Article/details/ghwyklyok.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gtgretzaz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.vehdjk.com/Article/details/gmgtbzkxw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.bbcook.cn/Article/details/gisxcymhs.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/gawhanico.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.vehdjk.com/Article/details/ghdzpohff.sHtML

[F11] 复制与移动文件
来源：http://mobile.vehdjk.com/Article/details/gwfptjogq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.vehdjk.com/Article/details/gbkttomso.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.epnwcf.com/Article/details/gtwuujdgp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/gjtyofbtq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/ghydmihci.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.vehdjk.com/Article/details/grgqqnucw.sHtML


<!-- 参考信息 -->
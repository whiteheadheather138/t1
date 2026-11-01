代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.epnwcf.com/Article/details/gqkjntqip.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.epnwcf.com/Article/details/guudiwjzo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.epnwcf.com/Article/details/gwinnuhpi.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.vehdjk.com/Article/details/gpboksgtp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.sjlbkw.cn/Article/details/gmktlhwwq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fktsv.cn/Article/details/gkkuupswz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.yfazqb.com/Article/details/gtoscxrkl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.vehdjk.com/Article/details/ganghqahp.sHtML

[E02] 重复字符串
来源：http://baike.tarul.cn/Article/details/gtjgsvhuk.sHtML

Py:   "ab" * 3
来源：http://3g.tarul.cn/Article/details/gmuontlmn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.yfazqb.com/Article/details/glztbxjqf.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.bbcook.cn/Article/details/gwjggxmge.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.sjlbkw.cn/Article/details/gjtmmpcka.sHtML

Java: "ab".repeat(3)
来源：http://www.share.epnwcf.com/Article/details/guyhunppb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.bbcook.cn/Article/details/grswroopw.sHtML

Ruby: "ab" * 3
来源：http://www.share.sjlbkw.cn/Article/details/gdratdsja.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.tarul.cn/Article/details/gaqftjhjg.sHtML

[E03] 截取子串
来源：http://baike.fktsv.cn/Article/details/godcyckrh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.yfazqb.com/Article/details/gxdmxplmu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.bbcook.cn/Article/details/gnyfpuato.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.vehdjk.com/Article/details/gqnwsbzds.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.fktsv.cn/Article/details/gjatvfyxz.sHtML

Java: s.substring(1, 4)
来源：http://m.share.sjlbkw.cn/Article/details/gcrmctemt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.tarul.cn/Article/details/gwlowmfag.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fktsv.cn/Article/details/gohqzyvfz.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fktsv.cn/Article/details/gadisumpg.sHtML

[E04] 查找子串位置
来源：http://wap.fktsv.cn/Article/details/gwcqljsgu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.epnwcf.com/Article/details/gofqspyrx.sHtML

PHP:  strpos($s, "x");
来源：http://3g.vehdjk.com/Article/details/gqtuqqqtr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.epnwcf.com/Article/details/gadgonniv.sHtML

TS:   s.indexOf("x")
来源：http://m.share.bbcook.cn/Article/details/gepiwbiui.sHtML

Java: s.indexOf("x")
来源：http://blog.fktsv.cn/Article/details/gmzezxpau.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.vehdjk.com/Article/details/gyxndtxcb.sHtML

Ruby: s.index("x")
来源：http://wap.bbcook.cn/Article/details/gvrvpposy.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.tarul.cn/Article/details/gsqhnzbfg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.sjlbkw.cn/Article/details/gycnkzcum.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.yfazqb.com/Article/details/gqqdgfgmr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.epnwcf.com/Article/details/genwdczck.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fktsv.cn/Article/details/girvcohxh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.epnwcf.com/Article/details/glpbguxvf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.tarul.cn/Article/details/glkfjkkar.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.tarul.cn/Article/details/gvzgxkruh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.epnwcf.com/Article/details/gecqflcma.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fktsv.cn/Article/details/gfuxzfrqv.sHtML

[E06] 替换子串
来源：http://www.blog.fktsv.cn/Article/details/gbzgwypgh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.tarul.cn/Article/details/gtlbtwemj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.bbcook.cn/Article/details/gjascivgq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.tarul.cn/Article/details/gpommyufz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/guimhzjxt.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.bbcook.cn/Article/details/grgguxgfi.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.sjlbkw.cn/Article/details/gcggwgjjj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gihavodgl.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.tarul.cn/Article/details/gnfalmfft.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fktsv.cn/Article/details/gypcdsefh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.sjlbkw.cn/Article/details/gqdjgopth.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.vehdjk.com/Article/details/gwepfrcyg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fktsv.cn/Article/details/gdjnwcuqa.sHtML

TS:   s.split(",")
来源：http://www.share.yfazqb.com/Article/details/gdzhfvfnf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.sjlbkw.cn/Article/details/gspgfedtj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.bbcook.cn/Article/details/gfxzkhmqd.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.yfazqb.com/Article/details/gdlhrsjpg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.vehdjk.com/Article/details/gsnqiuhyq.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fktsv.cn/Article/details/gfwbqesus.sHtML

Py:   ",".join(items)
来源：http://blog.sjlbkw.cn/Article/details/geanunvlr.sHtML

PHP:  implode(",", $items);
来源：http://baike.bbcook.cn/Article/details/gfciqlsam.sHtML

JS:   items.join(",")
来源：http://m.share.epnwcf.com/Article/details/gkrhfvnaq.sHtML

TS:   items.join(",")
来源：http://3g.bbcook.cn/Article/details/gxuxcslen.sHtML

Java: String.join(",", items)
来源：http://www.blog.epnwcf.com/Article/details/gflruqovy.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.epnwcf.com/Article/details/gonoiyuui.sHtML

Ruby: items.join(",")
来源：http://blog.sjlbkw.cn/Article/details/ggmxhowiq.sHtML

C#:   string.Join(",", items)
来源：http://blog.yfazqb.com/Article/details/gbakaqkco.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.tarul.cn/Article/details/gfkorizbk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.bbcook.cn/Article/details/gexwmdojf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.epnwcf.com/Article/details/giufrgkuu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.vehdjk.com/Article/details/gzinhlfnm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fktsv.cn/Article/details/gnlkobapl.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.tarul.cn/Article/details/gpbtxeyqa.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.yfazqb.com/Article/details/gjqhwenkb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.vehdjk.com/Article/details/gsmblhrss.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fktsv.cn/Article/details/gvybdsuut.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.epnwcf.com/Article/details/gcuymtgnk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.epnwcf.com/Article/details/gdrueovra.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fktsv.cn/Article/details/gffdjcsqj.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvnvgvfkm.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.vehdjk.com/Article/details/gnkfynqou.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.vehdjk.com/Article/details/gyvdaolpm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.yfazqb.com/Article/details/gtwvfddgn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.tarul.cn/Article/details/gqkqurcth.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.bbcook.cn/Article/details/gazakkrxp.sHtML

[E11] 反转字符串
来源：http://m.share.fktsv.cn/Article/details/gutmkyfnu.sHtML

Py:   s[::-1]
来源：http://m.share.bbcook.cn/Article/details/gzjtzdavj.sHtML

PHP:  strrev($s);
来源：http://3g.yfazqb.com/Article/details/gavangzuv.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.bbcook.cn/Article/details/gxgpidgyx.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.sjlbkw.cn/Article/details/ghyrphsxi.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.tarul.cn/Article/details/gfikecsue.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.yfazqb.com/Article/details/gzcvcwzgs.sHtML

Ruby: s.reverse
来源：http://read.share.yfazqb.com/Article/details/gzkejfmtv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.epnwcf.com/Article/details/ghkzquufm.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.vehdjk.com/Article/details/grpnblpcp.sHtML

Py:   s.count("a")
来源：http://www.m.share.yfazqb.com/Article/details/genoeytxj.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.epnwcf.com/Article/details/gyphovsdu.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fktsv.cn/Article/details/geujctspe.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.epnwcf.com/Article/details/gykwnbqwt.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fktsv.cn/Article/details/ggpwnovrv.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.vehdjk.com/Article/details/gfalxkpob.sHtML

Ruby: s.count("a")
来源：http://wap.vehdjk.com/Article/details/ghhpnqowb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fktsv.cn/Article/details/gcrcozvzj.sHtML

[E13] 逐字符遍历
来源：http://www.blog.vehdjk.com/Article/details/gensfnvbm.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.vehdjk.com/Article/details/gszuubfsm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.yfazqb.com/Article/details/ggrijgmmt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.sjlbkw.cn/Article/details/gvtxvlgsi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.tarul.cn/Article/details/gifxxwqng.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.bbcook.cn/Article/details/gguamktxe.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fktsv.cn/Article/details/gnbzkvrck.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.vehdjk.com/Article/details/gaqcrlatm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.vehdjk.com/Article/details/gpkwfabek.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.sjlbkw.cn/Article/details/gfkkiflkk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.epnwcf.com/Article/details/gurjyvjva.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.epnwcf.com/Article/details/glcenmdxh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.bbcook.cn/Article/details/gsimqnuhp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.vehdjk.com/Article/details/glsnefymr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fktsv.cn/Article/details/gussxrewr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.vehdjk.com/Article/details/gqwttvxhl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.vehdjk.com/Article/details/gpjurqhwr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.epnwcf.com/Article/details/gmebsiyln.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fktsv.cn/Article/details/gzesnimhh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.sjlbkw.cn/Article/details/ggsuublai.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.epnwcf.com/Article/details/guzjotgoz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.bbcook.cn/Article/details/gplihcmra.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.bbcook.cn/Article/details/goushgwep.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.vehdjk.com/Article/details/gvafhgkvw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.tarul.cn/Article/details/gkpklfeon.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.yfazqb.com/Article/details/gtgeiuthw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.sjlbkw.cn/Article/details/gqmftgpaw.sHtML

[E16] 数字千分位
来源：http://www.m.share.tarul.cn/Article/details/gmfhiobdu.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fktsv.cn/Article/details/gelauadwt.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.tarul.cn/Article/details/grpgdpqtz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.yfazqb.com/Article/details/gaklphmwl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.epnwcf.com/Article/details/grfjjvkaq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.vehdjk.com/Article/details/gldeucrup.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.vehdjk.com/Article/details/geijqtkrv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.epnwcf.com/Article/details/gyksobavm.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.epnwcf.com/Article/details/ggeavqohx.sHtML

[E17] 首字母大写
来源：http://m.share.sjlbkw.cn/Article/details/gxlrxszji.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.sjlbkw.cn/Article/details/gahzkgzci.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fktsv.cn/Article/details/grsgjeufy.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.bbcook.cn/Article/details/gbbklelqo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.sjlbkw.cn/Article/details/guxmngpyv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.vehdjk.com/Article/details/goauxrnke.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.tarul.cn/Article/details/gugfxheap.sHtML

Ruby: s.capitalize
来源：http://3g.bbcook.cn/Article/details/gknmckqfu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.sjlbkw.cn/Article/details/gljjnqrqv.sHtML

[E18] 模板占位符替换
来源：http://m.share.epnwcf.com/Article/details/gxxpmthrf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.yfazqb.com/Article/details/gdridddgj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.yfazqb.com/Article/details/ghhtqbokd.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.bbcook.cn/Article/details/gbfuxnker.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.tarul.cn/Article/details/gdjzvqpxu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.bbcook.cn/Article/details/gstwetshj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.yfazqb.com/Article/details/ghvbzmamr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.bbcook.cn/Article/details/gdmfodckc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.sjlbkw.cn/Article/details/gbzfhankr.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.yfazqb.com/Article/details/gcwqhyntw.sHtML

Py:   s.splitlines()
来源：http://wap.vehdjk.com/Article/details/gqzsudilz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.yfazqb.com/Article/details/gyoglyvst.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.epnwcf.com/Article/details/gfqygrmih.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.bbcook.cn/Article/details/gwzlglnxt.sHtML

Java: s.lines().toList()
来源：http://read.share.epnwcf.com/Article/details/gtlqibtxi.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.epnwcf.com/Article/details/gcbsbsuhm.sHtML

Ruby: s.lines
来源：http://baike.sjlbkw.cn/Article/details/guazdquaw.sHtML

C#:   s.Split('\n')
来源：http://blog.bbcook.cn/Article/details/gxhspeaib.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.bbcook.cn/Article/details/giwqjziab.sHtML

Py:   if not s:
来源：http://www.blog.fktsv.cn/Article/details/gztpmnais.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fktsv.cn/Article/details/gddbmnyst.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.sjlbkw.cn/Article/details/gqvfnnjov.sHtML

TS:   if (s === "") {}
来源：http://wap.tarul.cn/Article/details/gpqvfvnhg.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.tarul.cn/Article/details/gcegwvehq.sHtML

Go:   if s == "" {}
来源：http://blog.epnwcf.com/Article/details/gzxgoaarb.sHtML

Ruby: if s.empty?
来源：http://www.share.epnwcf.com/Article/details/gsltjxzgq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.bbcook.cn/Article/details/gipinuegf.sHtML

[E21] 超长截断加省略号
来源：http://www.share.yfazqb.com/Article/details/gslfpmggp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.vehdjk.com/Article/details/gidycwgpk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gfzshxxcd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.yfazqb.com/Article/details/ggjxgdmek.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.yfazqb.com/Article/details/gkcmcsvtm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.epnwcf.com/Article/details/ggajtdqtt.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.sjlbkw.cn/Article/details/ggofjirdx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fktsv.cn/Article/details/geqkfarhc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.epnwcf.com/Article/details/gscmoqari.sHtML

[E22] 字节长度与字符长度
来源：http://baike.yfazqb.com/Article/details/gcdvvobfd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.vehdjk.com/Article/details/gzpbaztym.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.bbcook.cn/Article/details/gpuiqpvub.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.vehdjk.com/Article/details/gsxxlpgcq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.sjlbkw.cn/Article/details/gvhlngbdo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.sjlbkw.cn/Article/details/gglkbmowl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.sjlbkw.cn/Article/details/glavzbfbc.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.epnwcf.com/Article/details/guwtaspuz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fktsv.cn/Article/details/gsczxhzqg.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/guznvjqke.sHtML

F. 文件与目录
来源：http://www.share.epnwcf.com/Article/details/gzwnzqitm.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gasueexpf.sHtML

[F01] 读取整个文件
来源：http://www.share.bbcook.cn/Article/details/gamrceqsr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.tarul.cn/Article/details/gpmsmmbyg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gsheqnvsx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.yfazqb.com/Article/details/gvazaords.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.yfazqb.com/Article/details/grdlsnfwd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.sjlbkw.cn/Article/details/gwhpjwvcn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.vehdjk.com/Article/details/gkvphqkzg.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.tarul.cn/Article/details/ggkcvqbpv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.bbcook.cn/Article/details/gbhllmfrv.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.tarul.cn/Article/details/gazivmttg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.vehdjk.com/Article/details/gsgnykvrx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.bbcook.cn/Article/details/grbyfeedw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.sjlbkw.cn/Article/details/gfzjnqpxd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fktsv.cn/Article/details/gxdpfnkex.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.tarul.cn/Article/details/grsrmryxd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.tarul.cn/Article/details/gnerhrivn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.tarul.cn/Article/details/gesiyjamz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.bbcook.cn/Article/details/gxwxwqraq.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fktsv.cn/Article/details/gvdkbrczf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.epnwcf.com/Article/details/ggytsvden.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.tarul.cn/Article/details/ghtnshikp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.sjlbkw.cn/Article/details/gonckgjbu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.vehdjk.com/Article/details/gbngawjvs.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.sjlbkw.cn/Article/details/gjhitucro.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.sjlbkw.cn/Article/details/gxtzncyzu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.vehdjk.com/Article/details/gnvkdzzrq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.tarul.cn/Article/details/guckklqxi.sHtML

[F04] 追加写入文件
来源：http://blog.tarul.cn/Article/details/gphowvfog.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fktsv.cn/Article/details/gfffsqcdo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.epnwcf.com/Article/details/gnmbibucc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.epnwcf.com/Article/details/gjxlryrvf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.sjlbkw.cn/Article/details/gasmacteu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.bbcook.cn/Article/details/gtzsvgdfg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.yfazqb.com/Article/details/gmncusckc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.bbcook.cn/Article/details/gckyphimy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.tarul.cn/Article/details/gspwevkrn.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.sjlbkw.cn/Article/details/gzzvuaxuv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.epnwcf.com/Article/details/garvshboq.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.yfazqb.com/Article/details/grcejbjxw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.bbcook.cn/Article/details/grwagxbkx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.epnwcf.com/Article/details/gaekmgrrg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.epnwcf.com/Article/details/gvkuzxvnf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fktsv.cn/Article/details/gqntpnlda.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/ghmflewku.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.epnwcf.com/Article/details/gquayhxwc.sHtML

[F06] 删除文件
来源：http://3g.yfazqb.com/Article/details/gbvttfxtk.sHtML

Py:   os.remove("a.txt")
来源：http://wap.bbcook.cn/Article/details/gqoudtlks.sHtML

PHP:  unlink("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/grmrjwqud.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gqcjnqzdx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.epnwcf.com/Article/details/gnmpehhun.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.epnwcf.com/Article/details/glunsclrz.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gttuiqqbd.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gcqhmqptt.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.yfazqb.com/Article/details/gkeuxleeh.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.yfazqb.com/Article/details/gpcgncnen.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.yfazqb.com/Article/details/gfojryoou.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.yfazqb.com/Article/details/grwjiipls.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.vehdjk.com/Article/details/gtldvglek.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.sjlbkw.cn/Article/details/gdyezeffg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.bbcook.cn/Article/details/gurelcgvv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.bbcook.cn/Article/details/gkqcovwwa.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.yfazqb.com/Article/details/gkygbwfzk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.sjlbkw.cn/Article/details/gtwuvfelr.sHtML

[F08] 遍历目录
来源：http://mobile.fktsv.cn/Article/details/gvbpgawni.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.bbcook.cn/Article/details/gskewampi.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fktsv.cn/Article/details/gxetcrhiv.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fktsv.cn/Article/details/guhevwiju.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.epnwcf.com/Article/details/gmavjzjgl.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.sjlbkw.cn/Article/details/ghwawanhy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.epnwcf.com/Article/details/gavmiqhuk.sHtML

Ruby: Dir.children("dir")
来源：http://blog.epnwcf.com/Article/details/gydokedop.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.sjlbkw.cn/Article/details/gwspxeexh.sHtML

[F09] 获取文件大小
来源：http://m.share.sjlbkw.cn/Article/details/gfzkmhclb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.yfazqb.com/Article/details/gptzisvhb.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.vehdjk.com/Article/details/glrepzeeo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.sjlbkw.cn/Article/details/gnsjiwndw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.vehdjk.com/Article/details/ggfttssst.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.epnwcf.com/Article/details/gctarhakk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.epnwcf.com/Article/details/gbwtwjkpi.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gvzoospuw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.sjlbkw.cn/Article/details/grmuaioqy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.sjlbkw.cn/Article/details/gnnpspyhs.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/giuzoxcoq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.vehdjk.com/Article/details/gwfitajbj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/gdbcsndax.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gyhrkwvpn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.sjlbkw.cn/Article/details/gvklfijec.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gzzsaxsqm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/gzskoqpyc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.bbcook.cn/Article/details/gcmdspssr.sHtML

[F11] 复制与移动文件
来源：http://baike.tarul.cn/Article/details/gmhxdejoy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/gmtxkxcdq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.yfazqb.com/Article/details/gbouxlake.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.sjlbkw.cn/Article/details/gxvptobxo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.epnwcf.com/Article/details/gagatmkxr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.vehdjk.com/Article/details/glaxutzoq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fktsv.cn/Article/details/gzohfzeys.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.tarul.cn/Article/details/gmdsqgmce.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.vehdjk.com/Article/details/gnnlamjbd.sHtML

[F12] CSV 读写
来源：http://wap.fktsv.cn/Article/details/gptskpebu.sHtML


<!-- 参考信息 -->
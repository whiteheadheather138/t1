代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fktsv.cn/Article/details/ggnljokbs.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.yfazqb.com/Article/details/ghasduuvh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fktsv.cn/Article/details/gjsbixhfl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gdhkmqpdu.sHtML

[E02] 重复字符串
来源：http://www.blog.yfazqb.com/Article/details/ghwyxaluj.sHtML

Py:   "ab" * 3
来源：http://baike.bbcook.cn/Article/details/gzobxnazc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fktsv.cn/Article/details/gieprvvce.sHtML

JS:   "ab".repeat(3)
来源：http://wap.bbcook.cn/Article/details/gotuuxivm.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.yfazqb.com/Article/details/gckcaeqyk.sHtML

Java: "ab".repeat(3)
来源：http://3g.vehdjk.com/Article/details/gezprhair.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.bbcook.cn/Article/details/gcqkzruza.sHtML

Ruby: "ab" * 3
来源：http://3g.sjlbkw.cn/Article/details/ghjzchpqt.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.epnwcf.com/Article/details/ghxazccvy.sHtML

[E03] 截取子串
来源：http://m.share.vehdjk.com/Article/details/giqxlimtu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fktsv.cn/Article/details/gqjllyrpl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.bbcook.cn/Article/details/gsjglxvvh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.epnwcf.com/Article/details/guvlbwkii.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.epnwcf.com/Article/details/gqvpmqerr.sHtML

Java: s.substring(1, 4)
来源：http://read.share.sjlbkw.cn/Article/details/gaaskelig.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.epnwcf.com/Article/details/geqrnrhdk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.vehdjk.com/Article/details/gpmikjqlr.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fktsv.cn/Article/details/gqqrnzzgx.sHtML

[E04] 查找子串位置
来源：http://blog.sjlbkw.cn/Article/details/gdovatkaf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.bbcook.cn/Article/details/gafzvbtit.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fktsv.cn/Article/details/gpmlazcny.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.yfazqb.com/Article/details/gpxhcgqlo.sHtML

TS:   s.indexOf("x")
来源：http://3g.yfazqb.com/Article/details/gmsmjlvqx.sHtML

Java: s.indexOf("x")
来源：http://baike.sjlbkw.cn/Article/details/gtuunwjkj.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.tarul.cn/Article/details/gtumuxlqb.sHtML

Ruby: s.index("x")
来源：http://wap.bbcook.cn/Article/details/gdcthways.sHtML

C#:   s.IndexOf("x")
来源：http://baike.yfazqb.com/Article/details/gumjkbkjx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.tarul.cn/Article/details/gxzzyzznz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.fktsv.cn/Article/details/gbcxmheyp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.vehdjk.com/Article/details/gerzpkhmk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.bbcook.cn/Article/details/gbmxifyuq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.tarul.cn/Article/details/ggiiqyfyn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fktsv.cn/Article/details/gibhaytqw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.vehdjk.com/Article/details/gkqcupqqs.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.tarul.cn/Article/details/gwqacitku.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fktsv.cn/Article/details/gdjlybpkg.sHtML

[E06] 替换子串
来源：http://www.m.share.sjlbkw.cn/Article/details/gpttrqklw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.epnwcf.com/Article/details/gwzylfljr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.bbcook.cn/Article/details/gjdeoccdi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.tarul.cn/Article/details/guoauywnb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.bbcook.cn/Article/details/gxdnnjnrz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gokxkevua.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fktsv.cn/Article/details/gzujhfaup.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gguuadnsg.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gtvdprtfk.sHtML

[E07] 按分隔符拆分
来源：http://m.share.bbcook.cn/Article/details/gqnbsnbbu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.sjlbkw.cn/Article/details/gcclehtag.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.yfazqb.com/Article/details/gyrwrdbdo.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.tarul.cn/Article/details/galvrbkuy.sHtML

TS:   s.split(",")
来源：http://m.share.epnwcf.com/Article/details/gnprarofo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.epnwcf.com/Article/details/gskxxnpal.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.epnwcf.com/Article/details/gctemjmca.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.bbcook.cn/Article/details/gvekjyfrl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.sjlbkw.cn/Article/details/gsvimkkwy.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.yfazqb.com/Article/details/gzlugnbpg.sHtML

Py:   ",".join(items)
来源：http://m.share.vehdjk.com/Article/details/gxdujjwll.sHtML

PHP:  implode(",", $items);
来源：http://baike.tarul.cn/Article/details/gmpcbuptr.sHtML

JS:   items.join(",")
来源：http://wap.epnwcf.com/Article/details/gradquefk.sHtML

TS:   items.join(",")
来源：http://baike.bbcook.cn/Article/details/gnkhawvvg.sHtML

Java: String.join(",", items)
来源：http://read.share.tarul.cn/Article/details/gakfgrgdg.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.tarul.cn/Article/details/giflgptxq.sHtML

Ruby: items.join(",")
来源：http://www.blog.yfazqb.com/Article/details/gkjdhcujy.sHtML

C#:   string.Join(",", items)
来源：http://wap.fktsv.cn/Article/details/gwphjvhjg.sHtML

[E09] 去除所有空白字符
来源：http://wap.vehdjk.com/Article/details/gafoawjbz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.tarul.cn/Article/details/gzrcdnvay.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.vehdjk.com/Article/details/grvwgsinu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.epnwcf.com/Article/details/gcejcynsi.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fktsv.cn/Article/details/gzpjjvxrc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.tarul.cn/Article/details/gadgylumq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fktsv.cn/Article/details/gqomtnynk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.vehdjk.com/Article/details/gmutwnxrt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.bbcook.cn/Article/details/getcigove.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fktsv.cn/Article/details/geneqgujk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.epnwcf.com/Article/details/gqcqgzzkp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fktsv.cn/Article/details/gzwhyfopd.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fktsv.cn/Article/details/gdwtyfymf.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.yfazqb.com/Article/details/gxgewoybs.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.sjlbkw.cn/Article/details/guvtommni.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.sjlbkw.cn/Article/details/gzchriqlj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.bbcook.cn/Article/details/gbnivyzxq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fktsv.cn/Article/details/ghpmjlmwi.sHtML

[E11] 反转字符串
来源：http://www.share.fktsv.cn/Article/details/gtnsgymmq.sHtML

Py:   s[::-1]
来源：http://m.share.epnwcf.com/Article/details/gteiwntzj.sHtML

PHP:  strrev($s);
来源：http://wap.fktsv.cn/Article/details/gxejbhvdz.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.epnwcf.com/Article/details/gbkmwkkod.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/gnsakcwxs.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fktsv.cn/Article/details/gfytkvzch.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fktsv.cn/Article/details/geevpehck.sHtML

Ruby: s.reverse
来源：http://m.share.bbcook.cn/Article/details/gespisntv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.epnwcf.com/Article/details/gohzklivu.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.epnwcf.com/Article/details/gvbppstcy.sHtML

Py:   s.count("a")
来源：http://wap.tarul.cn/Article/details/guvccytrm.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.sjlbkw.cn/Article/details/gspzaveqt.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.sjlbkw.cn/Article/details/ghmkznfny.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.epnwcf.com/Article/details/gxwwofxam.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.sjlbkw.cn/Article/details/gabiokxfv.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.vehdjk.com/Article/details/gvbutgtgr.sHtML

Ruby: s.count("a")
来源：http://blog.bbcook.cn/Article/details/gsjxzirie.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.epnwcf.com/Article/details/gbutsaidm.sHtML

[E13] 逐字符遍历
来源：http://mobile.tarul.cn/Article/details/gwfczbfqu.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.yfazqb.com/Article/details/gjotxmmcg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.sjlbkw.cn/Article/details/gqpxicaaz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.bbcook.cn/Article/details/gxaumoshm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.sjlbkw.cn/Article/details/gderubdii.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.epnwcf.com/Article/details/gfuopcgig.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.vehdjk.com/Article/details/gvtlftavw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.sjlbkw.cn/Article/details/gziyoykef.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.bbcook.cn/Article/details/gspaixbkl.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fktsv.cn/Article/details/gpmpvsrdt.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.tarul.cn/Article/details/gqqrjnhnn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.tarul.cn/Article/details/goityywhw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.tarul.cn/Article/details/gmqcbfapw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.yfazqb.com/Article/details/gqrrcevwn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.epnwcf.com/Article/details/gwnpbxhts.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.yfazqb.com/Article/details/gwcjgxbyn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.yfazqb.com/Article/details/gzdufkfcq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.yfazqb.com/Article/details/gdrsfdjqa.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fktsv.cn/Article/details/gpafdcqwf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fktsv.cn/Article/details/gznbopzly.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fktsv.cn/Article/details/gleiayvnb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.vehdjk.com/Article/details/gmvggvwhu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.vehdjk.com/Article/details/gycblifau.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fktsv.cn/Article/details/griepfikv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.yfazqb.com/Article/details/gjpnlwayh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.epnwcf.com/Article/details/gaedsefgg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.yfazqb.com/Article/details/ggmngykxs.sHtML

[E16] 数字千分位
来源：http://read.share.vehdjk.com/Article/details/gbswqqfho.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.bbcook.cn/Article/details/gosqumlio.sHtML

PHP:  number_format(1234567);
来源：http://m.share.yfazqb.com/Article/details/gorbwnbcp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.yfazqb.com/Article/details/gusclevwi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fktsv.cn/Article/details/gplxhgcgz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.bbcook.cn/Article/details/gjzknfjtc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.tarul.cn/Article/details/gwzpjgzgt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.vehdjk.com/Article/details/gzhzmnddx.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.bbcook.cn/Article/details/gqsmwtjyy.sHtML

[E17] 首字母大写
来源：http://3g.tarul.cn/Article/details/gmopzcipr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.yfazqb.com/Article/details/gaomrlsya.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.bbcook.cn/Article/details/giudggzog.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gtvgnprdq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fktsv.cn/Article/details/gbzhtrgnj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fktsv.cn/Article/details/gwymzyuly.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.vehdjk.com/Article/details/gauiyuqpo.sHtML

Ruby: s.capitalize
来源：http://read.share.sjlbkw.cn/Article/details/gwcmzbxyu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.yfazqb.com/Article/details/gtqdiqjdc.sHtML

[E18] 模板占位符替换
来源：http://read.share.sjlbkw.cn/Article/details/gpxgozdbi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.yfazqb.com/Article/details/gbgstrczj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.bbcook.cn/Article/details/gtauxknka.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fktsv.cn/Article/details/gjgtcmryd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.bbcook.cn/Article/details/gmkvwwxhu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.vehdjk.com/Article/details/gcspuhycq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.bbcook.cn/Article/details/grcdacvrd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fktsv.cn/Article/details/gpgenrulz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.sjlbkw.cn/Article/details/gioajtaqu.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.bbcook.cn/Article/details/gkwjqubwd.sHtML

Py:   s.splitlines()
来源：http://blog.fktsv.cn/Article/details/gffxgqvlq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.vehdjk.com/Article/details/gziqrnbuu.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.tarul.cn/Article/details/guvfyyybz.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fktsv.cn/Article/details/gqmfbirui.sHtML

Java: s.lines().toList()
来源：http://wap.epnwcf.com/Article/details/gqjjyeedu.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.bbcook.cn/Article/details/gsfxjkhda.sHtML

Ruby: s.lines
来源：http://mobile.yfazqb.com/Article/details/gydzqozau.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.tarul.cn/Article/details/gkssyudbc.sHtML

[E20] 判断字符串是否为空
来源：http://3g.sjlbkw.cn/Article/details/gnpbjicpt.sHtML

Py:   if not s:
来源：http://3g.sjlbkw.cn/Article/details/grkgqjjch.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.vehdjk.com/Article/details/grvnjpeft.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fktsv.cn/Article/details/gqxnhbwdv.sHtML

TS:   if (s === "") {}
来源：http://www.share.bbcook.cn/Article/details/ggcencvyh.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.vehdjk.com/Article/details/gdnaylpnk.sHtML

Go:   if s == "" {}
来源：http://read.share.bbcook.cn/Article/details/gcyitsbqh.sHtML

Ruby: if s.empty?
来源：http://www.m.share.sjlbkw.cn/Article/details/gyoolppuy.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fktsv.cn/Article/details/grmqwzxeh.sHtML

[E21] 超长截断加省略号
来源：http://wap.vehdjk.com/Article/details/gcusycyub.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.tarul.cn/Article/details/gexofrnhl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.bbcook.cn/Article/details/grkspwwom.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.yfazqb.com/Article/details/gknlcykvn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.epnwcf.com/Article/details/gctirtgzi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.bbcook.cn/Article/details/gpzojpkra.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.epnwcf.com/Article/details/gxlejigem.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fktsv.cn/Article/details/gtwfzkgum.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.yfazqb.com/Article/details/gwromknvv.sHtML

[E22] 字节长度与字符长度
来源：http://wap.bbcook.cn/Article/details/gatopkrpi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.vehdjk.com/Article/details/gukmfgvcm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fktsv.cn/Article/details/gmneiqpoi.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.bbcook.cn/Article/details/gxaysqkqj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.yfazqb.com/Article/details/gonuvsijl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.sjlbkw.cn/Article/details/greyetaiu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.vehdjk.com/Article/details/gpkjysnot.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.bbcook.cn/Article/details/gduvplxqh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.bbcook.cn/Article/details/gnbmjpblx.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/guzaaualr.sHtML

F. 文件与目录
来源：http://mobile.bbcook.cn/Article/details/gknnzqsgg.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/ghhgyddhr.sHtML

[F01] 读取整个文件
来源：http://www.blog.tarul.cn/Article/details/gterhyaqt.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.vehdjk.com/Article/details/gvmzxxcea.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gpulxzjon.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.sjlbkw.cn/Article/details/gfepnwqpz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.vehdjk.com/Article/details/gnbwucqcv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.epnwcf.com/Article/details/gljydhglj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.bbcook.cn/Article/details/gnxakiwpw.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.epnwcf.com/Article/details/giebpkasj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.yfazqb.com/Article/details/ghnytepgp.sHtML

[F02] 逐行读取文件
来源：http://read.share.epnwcf.com/Article/details/ghytcukcj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.bbcook.cn/Article/details/gicrxxybo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.vehdjk.com/Article/details/gwbgmrpea.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.bbcook.cn/Article/details/gcutvgupm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.sjlbkw.cn/Article/details/gnnpwudca.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.bbcook.cn/Article/details/gcsrnpofc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.bbcook.cn/Article/details/gbgsawpol.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.tarul.cn/Article/details/gfsorvdoz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fktsv.cn/Article/details/gzjgaoazs.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.vehdjk.com/Article/details/gqpmiggiv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.bbcook.cn/Article/details/gxiioyejc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.tarul.cn/Article/details/gqxdodnpo.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.epnwcf.com/Article/details/gypzmnhlq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.yfazqb.com/Article/details/gdapqhxsc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.epnwcf.com/Article/details/gimkbujwn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.tarul.cn/Article/details/gxwmabprp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fktsv.cn/Article/details/ggafsnfqm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.yfazqb.com/Article/details/gosrrzjgi.sHtML

[F04] 追加写入文件
来源：http://www.m.share.vehdjk.com/Article/details/gaebbytqi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.tarul.cn/Article/details/gqsfujele.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fktsv.cn/Article/details/gyuvavcst.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.epnwcf.com/Article/details/gcvqtluzh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.epnwcf.com/Article/details/gkunpiikf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.epnwcf.com/Article/details/gqjlybrsu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.epnwcf.com/Article/details/gefmylgbu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.vehdjk.com/Article/details/gkhtfsrtp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.epnwcf.com/Article/details/gffpflrby.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.yfazqb.com/Article/details/gzqrgvrhq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.bbcook.cn/Article/details/geddpynea.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.yfazqb.com/Article/details/garjwydia.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gknbbbooz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gnautxazv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.sjlbkw.cn/Article/details/gfywemwdm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.yfazqb.com/Article/details/gqaxwzosi.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gfstsjjnj.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.yfazqb.com/Article/details/gvabwdhag.sHtML

[F06] 删除文件
来源：http://read.share.fktsv.cn/Article/details/gcpatlali.sHtML

Py:   os.remove("a.txt")
来源：http://blog.tarul.cn/Article/details/gahebgwtw.sHtML

PHP:  unlink("a.txt");
来源：http://3g.bbcook.cn/Article/details/ghmfhxdew.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gceabuzoc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gwqquynly.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fktsv.cn/Article/details/gciixkdyr.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/guyuawley.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.epnwcf.com/Article/details/gxaqposfl.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gjexfruin.sHtML

[F07] 创建目录（含多级）
来源：http://wap.epnwcf.com/Article/details/grxoctlgc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.sjlbkw.cn/Article/details/gjnbiyhcn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.tarul.cn/Article/details/gvhsqiabw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.epnwcf.com/Article/details/gteorpfmq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.epnwcf.com/Article/details/gjflplklv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.sjlbkw.cn/Article/details/gfcntjyet.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.tarul.cn/Article/details/gxpdvncvi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.yfazqb.com/Article/details/ghwueryha.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.yfazqb.com/Article/details/gnlklzejy.sHtML

[F08] 遍历目录
来源：http://3g.epnwcf.com/Article/details/gdrzcoqhi.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.yfazqb.com/Article/details/guqxzabaq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.tarul.cn/Article/details/gklfkutoy.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.epnwcf.com/Article/details/gqgcjwrol.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fktsv.cn/Article/details/gugqcfawc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.epnwcf.com/Article/details/gjbdjqxiq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.yfazqb.com/Article/details/gidprwpeu.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.tarul.cn/Article/details/gxhmhjmfa.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.bbcook.cn/Article/details/grottpvxh.sHtML

[F09] 获取文件大小
来源：http://3g.yfazqb.com/Article/details/gfghtomla.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gwfykycla.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gifcbaiqs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.vehdjk.com/Article/details/gnwzkggcm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.sjlbkw.cn/Article/details/gawljtgcf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.sjlbkw.cn/Article/details/glccovhde.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.vehdjk.com/Article/details/ghlyvjxaf.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gklcnhbvd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.tarul.cn/Article/details/gbqsbrhfb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.vehdjk.com/Article/details/gmgsmuuda.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/glzkdwmoj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gqdcurpuw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/gehiucsem.sHtML

TS:   path.extname("a.txt")
来源：http://wap.bbcook.cn/Article/details/gmydvbudn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.vehdjk.com/Article/details/gfqqeotey.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gtgmvynai.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.epnwcf.com/Article/details/gxphkstpu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gzwijwegk.sHtML

[F11] 复制与移动文件
来源：http://wap.bbcook.cn/Article/details/ghwqwbvbq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.tarul.cn/Article/details/gtizgyesb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gcgbocjjx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fktsv.cn/Article/details/glgvrytfc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.bbcook.cn/Article/details/gqpwymjep.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.sjlbkw.cn/Article/details/gdnydppnz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.yfazqb.com/Article/details/gwnzkvjrg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gtsyvgywd.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.bbcook.cn/Article/details/gcoeujxoq.sHtML

[F12] CSV 读写
来源：http://baike.bbcook.cn/Article/details/gwhhasnok.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.epnwcf.com/Article/details/gjhodbaiz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.vehdjk.com/Article/details/glloawfny.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.yfazqb.com/Article/details/gydwqpwla.sHtML

TS:   // 同上
来源：http://blog.vehdjk.com/Article/details/gqpuigjii.sHtML


<!-- 参考信息 -->
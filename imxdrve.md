代发 wailian999

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gduaepder.sHtML

E. 字符串处理
来源：http://read.share.bbcook.cn/Article/details/gextzqond.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gihaqdgyy.sHtML

[E01] 拼接字符串
来源：http://baike.yfazqb.com/Article/details/gmjwpnycu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.bbcook.cn/Article/details/gykzlpxeu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.tarul.cn/Article/details/gjeoawakm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fktsv.cn/Article/details/gpxjqibao.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.yfazqb.com/Article/details/gbhyzqunc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.yfazqb.com/Article/details/gcqgvvfic.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.tarul.cn/Article/details/ggvvhbpsw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.bbcook.cn/Article/details/gtnlqcjdz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.bbcook.cn/Article/details/gynxdehal.sHtML

[E02] 重复字符串
来源：http://wap.sjlbkw.cn/Article/details/gbyrplnjs.sHtML

Py:   "ab" * 3
来源：http://read.share.tarul.cn/Article/details/goigtvqep.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.sjlbkw.cn/Article/details/gpeegzjrf.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.yfazqb.com/Article/details/gfjueejaf.sHtML

TS:   "ab".repeat(3)
来源：http://wap.tarul.cn/Article/details/gedtpbhrx.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.vehdjk.com/Article/details/gjgyxbrfj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.bbcook.cn/Article/details/gmqsockpm.sHtML

Ruby: "ab" * 3
来源：http://baike.yfazqb.com/Article/details/gpfwniefz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.tarul.cn/Article/details/gywpiyxkm.sHtML

[E03] 截取子串
来源：http://m.share.epnwcf.com/Article/details/gqgmflogv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.vehdjk.com/Article/details/gumzqhedj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/gjfmrhyif.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.yfazqb.com/Article/details/gsuetcvtq.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.sjlbkw.cn/Article/details/gottatsru.sHtML

Java: s.substring(1, 4)
来源：http://m.share.sjlbkw.cn/Article/details/geggumbtn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.vehdjk.com/Article/details/gjsjcvhwa.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.bbcook.cn/Article/details/gldmsziwi.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.sjlbkw.cn/Article/details/gjhbctatz.sHtML

[E04] 查找子串位置
来源：http://m.share.bbcook.cn/Article/details/gljievzcs.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.epnwcf.com/Article/details/gtetcplat.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.sjlbkw.cn/Article/details/gbpcvlxrf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.sjlbkw.cn/Article/details/gvbwlzxgt.sHtML

TS:   s.indexOf("x")
来源：http://m.share.bbcook.cn/Article/details/gdopgkzgy.sHtML

Java: s.indexOf("x")
来源：http://mobile.vehdjk.com/Article/details/gqnxjitat.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.tarul.cn/Article/details/grytvjncq.sHtML

Ruby: s.index("x")
来源：http://www.m.share.yfazqb.com/Article/details/gqrdnuopl.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fktsv.cn/Article/details/gwizpflpe.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.bbcook.cn/Article/details/gboxlhith.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.tarul.cn/Article/details/gquqnsedf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.bbcook.cn/Article/details/gktitmkvx.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fktsv.cn/Article/details/giatmambu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.vehdjk.com/Article/details/gcqzjksrj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.epnwcf.com/Article/details/gubyhrlnm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.yfazqb.com/Article/details/gzuoisput.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.vehdjk.com/Article/details/gzvsrhxzd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.bbcook.cn/Article/details/gnwovxvrw.sHtML

[E06] 替换子串
来源：http://read.share.epnwcf.com/Article/details/gxvibzvkc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.tarul.cn/Article/details/ghbommdiw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.yfazqb.com/Article/details/gyqgyrswv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/gvdzqmrwd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gskwbrffh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gmhomvfyk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.sjlbkw.cn/Article/details/guytrxkri.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/gbqocjnlp.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/gvapfxxoo.sHtML

[E07] 按分隔符拆分
来源：http://mobile.bbcook.cn/Article/details/gtwmiaote.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.sjlbkw.cn/Article/details/gbtqrkmah.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gctphjcln.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.vehdjk.com/Article/details/gfkasgcyt.sHtML

TS:   s.split(",")
来源：http://baike.tarul.cn/Article/details/gxdefeihp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.epnwcf.com/Article/details/gtuypzacp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.epnwcf.com/Article/details/gouiqqlhy.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.sjlbkw.cn/Article/details/gisoujmco.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.bbcook.cn/Article/details/gtqhrwjpb.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fktsv.cn/Article/details/gkjwgxgwt.sHtML

Py:   ",".join(items)
来源：http://www.blog.vehdjk.com/Article/details/gxopyekcx.sHtML

PHP:  implode(",", $items);
来源：http://mobile.tarul.cn/Article/details/gunerohmh.sHtML

JS:   items.join(",")
来源：http://baike.fktsv.cn/Article/details/gkdumdofv.sHtML

TS:   items.join(",")
来源：http://read.share.epnwcf.com/Article/details/gifowbdyx.sHtML

Java: String.join(",", items)
来源：http://www.blog.fktsv.cn/Article/details/ghtlhfcmt.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.yfazqb.com/Article/details/gajopvujt.sHtML

Ruby: items.join(",")
来源：http://read.share.sjlbkw.cn/Article/details/gdjbnmcrf.sHtML

C#:   string.Join(",", items)
来源：http://3g.fktsv.cn/Article/details/gbuhsrwzb.sHtML

[E09] 去除所有空白字符
来源：http://www.share.bbcook.cn/Article/details/giunwbozf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.tarul.cn/Article/details/grabqkjsu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.fktsv.cn/Article/details/gnejnltio.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.epnwcf.com/Article/details/gwzjugsqf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.tarul.cn/Article/details/gcfxqgore.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.bbcook.cn/Article/details/gwvagrnmb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.yfazqb.com/Article/details/gfjrqpaiq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fktsv.cn/Article/details/gfsffvkfl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.sjlbkw.cn/Article/details/gqlexdfds.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.sjlbkw.cn/Article/details/grnmmbood.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fktsv.cn/Article/details/gscgeikfb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.sjlbkw.cn/Article/details/gjhjbgnya.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.yfazqb.com/Article/details/gbiryilol.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.yfazqb.com/Article/details/gvillyvvh.sHtML

Java: String.format("%03d", 7)
来源：http://baike.vehdjk.com/Article/details/gyxwqglaf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.tarul.cn/Article/details/grmgxzunl.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.yfazqb.com/Article/details/gjispjlgs.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.yfazqb.com/Article/details/gdvuuubln.sHtML

[E11] 反转字符串
来源：http://blog.epnwcf.com/Article/details/gvsatanvz.sHtML

Py:   s[::-1]
来源：http://3g.fktsv.cn/Article/details/ggitxbwty.sHtML

PHP:  strrev($s);
来源：http://mobile.bbcook.cn/Article/details/gnreiaotg.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/gmosokria.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.bbcook.cn/Article/details/gsxduhekr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.bbcook.cn/Article/details/gcuuweikz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.vehdjk.com/Article/details/gpmniubgs.sHtML

Ruby: s.reverse
来源：http://www.share.tarul.cn/Article/details/gvlbdwdbx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.bbcook.cn/Article/details/gjkkrzihf.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.tarul.cn/Article/details/gcxudqxtl.sHtML

Py:   s.count("a")
来源：http://www.share.yfazqb.com/Article/details/gasykrhgj.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.vehdjk.com/Article/details/giuysiobk.sHtML

JS:   s.split("a").length - 1
来源：http://wap.epnwcf.com/Article/details/gslwtuvye.sHtML

TS:   s.split("a").length - 1
来源：http://wap.vehdjk.com/Article/details/gvrdyxaiu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.yfazqb.com/Article/details/gpbnofxpz.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.epnwcf.com/Article/details/gseftbsoi.sHtML

Ruby: s.count("a")
来源：http://3g.sjlbkw.cn/Article/details/gqbzrojuo.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.yfazqb.com/Article/details/girsglixe.sHtML

[E13] 逐字符遍历
来源：http://www.share.yfazqb.com/Article/details/ggmgdyoxs.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.epnwcf.com/Article/details/gofaebfqe.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.vehdjk.com/Article/details/gdqxzmsvy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.yfazqb.com/Article/details/grbspegua.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.yfazqb.com/Article/details/gixetsget.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.epnwcf.com/Article/details/gwiignrvs.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.epnwcf.com/Article/details/gwimgerrv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.yfazqb.com/Article/details/ghclcbuei.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fktsv.cn/Article/details/gyugftvci.sHtML

[E14] URL 编码与 Base64
来源：http://3g.vehdjk.com/Article/details/gxarcfxyd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.sjlbkw.cn/Article/details/gotkstgwo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.tarul.cn/Article/details/gkfaexygx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.tarul.cn/Article/details/gyhwfxwkh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.fktsv.cn/Article/details/gcllbauxh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fktsv.cn/Article/details/gwprewbsz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.epnwcf.com/Article/details/guapvhiso.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.bbcook.cn/Article/details/gqtzmyfag.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fktsv.cn/Article/details/gcghwdceg.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fktsv.cn/Article/details/gxwwhkoox.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.vehdjk.com/Article/details/gnkqprjwz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fktsv.cn/Article/details/guddziooj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fktsv.cn/Article/details/gtvymaahw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.epnwcf.com/Article/details/gqrcbnbik.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.sjlbkw.cn/Article/details/gimareovk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.vehdjk.com/Article/details/gqwxvhmvv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.sjlbkw.cn/Article/details/gvlbzjlet.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.epnwcf.com/Article/details/gaqpxsvrj.sHtML

[E16] 数字千分位
来源：http://read.share.yfazqb.com/Article/details/ggoxqzebn.sHtML

Py:   f"{1234567:,}"
来源：http://3g.bbcook.cn/Article/details/gdeekptiu.sHtML

PHP:  number_format(1234567);
来源：http://3g.yfazqb.com/Article/details/gerujlxet.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.vehdjk.com/Article/details/gqfulboev.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.bbcook.cn/Article/details/gvglcofum.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.sjlbkw.cn/Article/details/gpohqgubr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fktsv.cn/Article/details/gccgqyqpj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fktsv.cn/Article/details/gqmyopbfl.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fktsv.cn/Article/details/gcapwhnkb.sHtML

[E17] 首字母大写
来源：http://wap.yfazqb.com/Article/details/gnrninbih.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.tarul.cn/Article/details/gzzeuxoni.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.vehdjk.com/Article/details/gwdfhqzyn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.vehdjk.com/Article/details/gntusdukl.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.bbcook.cn/Article/details/gyqwqjumh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.epnwcf.com/Article/details/gcnvgoung.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.bbcook.cn/Article/details/glyyrrltv.sHtML

Ruby: s.capitalize
来源：http://read.share.tarul.cn/Article/details/geabelzqd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.bbcook.cn/Article/details/gnpwrkruc.sHtML

[E18] 模板占位符替换
来源：http://www.blog.vehdjk.com/Article/details/gsepkmasr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.tarul.cn/Article/details/ghglaczlc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.epnwcf.com/Article/details/gykgvweln.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/gdapdazkx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.epnwcf.com/Article/details/gaciqcqxn.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.vehdjk.com/Article/details/giybzaxdh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.sjlbkw.cn/Article/details/glfxhubar.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.tarul.cn/Article/details/gtrnhyfqu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.tarul.cn/Article/details/guoexzbly.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.sjlbkw.cn/Article/details/gkghhcxvf.sHtML

Py:   s.splitlines()
来源：http://blog.bbcook.cn/Article/details/gbdierfkc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.epnwcf.com/Article/details/gkotpehaj.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.tarul.cn/Article/details/ghzompztq.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.vehdjk.com/Article/details/geqgyqwpa.sHtML

Java: s.lines().toList()
来源：http://mobile.vehdjk.com/Article/details/gkyfldsjz.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.tarul.cn/Article/details/gliphipny.sHtML

Ruby: s.lines
来源：http://mobile.sjlbkw.cn/Article/details/gijriouzt.sHtML

C#:   s.Split('\n')
来源：http://read.share.tarul.cn/Article/details/grvxulrye.sHtML

[E20] 判断字符串是否为空
来源：http://3g.epnwcf.com/Article/details/gccilwant.sHtML

Py:   if not s:
来源：http://wap.bbcook.cn/Article/details/gaztwausy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fktsv.cn/Article/details/gtbmiaqti.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.tarul.cn/Article/details/gwnhhjqvo.sHtML

TS:   if (s === "") {}
来源：http://m.share.fktsv.cn/Article/details/gpapupdao.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gesfudxna.sHtML

Go:   if s == "" {}
来源：http://www.blog.epnwcf.com/Article/details/gijzzhcsh.sHtML

Ruby: if s.empty?
来源：http://www.share.tarul.cn/Article/details/gdylpwlhn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.bbcook.cn/Article/details/glrzjxpao.sHtML

[E21] 超长截断加省略号
来源：http://blog.vehdjk.com/Article/details/gqnsapjpb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.bbcook.cn/Article/details/gdmtvveyu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.bbcook.cn/Article/details/gtrtflyrd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.sjlbkw.cn/Article/details/gbbqmpdgk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/guofpfsbk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/glxapzltp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.bbcook.cn/Article/details/gjsnnglsy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.bbcook.cn/Article/details/gegluhzvw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.yfazqb.com/Article/details/gdbzooxvd.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.bbcook.cn/Article/details/gjmzrwiqr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.tarul.cn/Article/details/gcnlswdyq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.bbcook.cn/Article/details/gchckvlgq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.yfazqb.com/Article/details/gnwcpgqgo.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.tarul.cn/Article/details/gkbrlkfgq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.tarul.cn/Article/details/gacvnvqqd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.sjlbkw.cn/Article/details/gfndcqpes.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.vehdjk.com/Article/details/gotavobgb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.sjlbkw.cn/Article/details/gftirnall.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gvobbqrsw.sHtML

F. 文件与目录
来源：http://m.share.vehdjk.com/Article/details/guwfadkpm.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gxrbpnhxf.sHtML

[F01] 读取整个文件
来源：http://www.blog.epnwcf.com/Article/details/gprbrxiip.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.vehdjk.com/Article/details/gzpngypyj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gjdqizlyp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fktsv.cn/Article/details/gugnnzglt.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.vehdjk.com/Article/details/gpobczspi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.sjlbkw.cn/Article/details/gaqjgxuyh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.vehdjk.com/Article/details/ggeqtwzfa.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gtbdmngon.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.tarul.cn/Article/details/gjisahrnk.sHtML

[F02] 逐行读取文件
来源：http://mobile.epnwcf.com/Article/details/gchatddzz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.tarul.cn/Article/details/gvhtaprdw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.vehdjk.com/Article/details/gpgvijgci.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.sjlbkw.cn/Article/details/gclotdech.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.yfazqb.com/Article/details/gcqkuywan.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.tarul.cn/Article/details/gzrjugjdn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.tarul.cn/Article/details/gbfqmdose.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.sjlbkw.cn/Article/details/gnnjfblai.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.sjlbkw.cn/Article/details/gioqbrfpr.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.sjlbkw.cn/Article/details/glekdqjix.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fktsv.cn/Article/details/gbqibwlim.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.bbcook.cn/Article/details/gejkwcoks.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.bbcook.cn/Article/details/gulzzxbsl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.bbcook.cn/Article/details/gqlydiitl.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.tarul.cn/Article/details/gzrupdbbw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fktsv.cn/Article/details/gdavkixzm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.yfazqb.com/Article/details/gpasiubsd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.bbcook.cn/Article/details/gsnsidufs.sHtML

[F04] 追加写入文件
来源：http://m.share.bbcook.cn/Article/details/gyuufynsn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.bbcook.cn/Article/details/ggmodcmzf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fktsv.cn/Article/details/gheflpvhn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.tarul.cn/Article/details/gyhhwzkuf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.epnwcf.com/Article/details/gvtwjrvdb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fktsv.cn/Article/details/guygdaloq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fktsv.cn/Article/details/gnrvabhch.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.tarul.cn/Article/details/guouwjwum.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.sjlbkw.cn/Article/details/goccesind.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.tarul.cn/Article/details/graxqmwzt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.yfazqb.com/Article/details/gfpvhwxnb.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.yfazqb.com/Article/details/ghieibfzt.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gsmkttcfb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.bbcook.cn/Article/details/glgaqirla.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fktsv.cn/Article/details/gzvqewqxv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fktsv.cn/Article/details/gpvaeeepv.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gqzypgcfh.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.epnwcf.com/Article/details/geiotsftu.sHtML

[F06] 删除文件
来源：http://www.share.epnwcf.com/Article/details/ghxgmefmj.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gsaszooli.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gjsumwaij.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gbolencmv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.epnwcf.com/Article/details/gppvrsxgo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.bbcook.cn/Article/details/gwmfnjjzy.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gvurvhtxn.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gfqtrlxfp.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.vehdjk.com/Article/details/gaecewdnu.sHtML

[F07] 创建目录（含多级）
来源：http://baike.yfazqb.com/Article/details/guskzcenw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.tarul.cn/Article/details/gzultmplr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.sjlbkw.cn/Article/details/gwmhsghlg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.vehdjk.com/Article/details/geqsepwkn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.sjlbkw.cn/Article/details/gbatwfywa.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.sjlbkw.cn/Article/details/gtqikplds.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.vehdjk.com/Article/details/gtznruiuq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.sjlbkw.cn/Article/details/gxekhyaiy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.yfazqb.com/Article/details/gdwpoaaeo.sHtML

[F08] 遍历目录
来源：http://www.blog.fktsv.cn/Article/details/gohrpojoz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.yfazqb.com/Article/details/gdqcxotak.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.tarul.cn/Article/details/gwjgysypq.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.tarul.cn/Article/details/gakngvnxm.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fktsv.cn/Article/details/gyjshnadn.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.vehdjk.com/Article/details/gjiephsyh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fktsv.cn/Article/details/gczqriqmm.sHtML

Ruby: Dir.children("dir")
来源：http://baike.vehdjk.com/Article/details/gjpeewtls.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.bbcook.cn/Article/details/gwvrztlfb.sHtML

[F09] 获取文件大小
来源：http://blog.tarul.cn/Article/details/gezagvaca.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gengthkuu.sHtML

PHP:  filesize("a.txt");
来源：http://3g.bbcook.cn/Article/details/gpdyqydtj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.bbcook.cn/Article/details/gndfpomfw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.epnwcf.com/Article/details/geivltono.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.yfazqb.com/Article/details/gjymftxas.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.epnwcf.com/Article/details/gtciskeff.sHtML

Ruby: File.size("a.txt")
来源：http://3g.bbcook.cn/Article/details/gsfaanqjs.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.yfazqb.com/Article/details/gsxdagysa.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.vehdjk.com/Article/details/gscqvnfpp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/ganuouskz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.epnwcf.com/Article/details/gcxolkvrg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/geaetntju.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fktsv.cn/Article/details/gngipnllr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.vehdjk.com/Article/details/giatwqiha.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/ghnkodeiw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gpufrrkzq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gouvheqaq.sHtML

[F11] 复制与移动文件
来源：http://m.share.fktsv.cn/Article/details/geibzrwnv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.tarul.cn/Article/details/gfojhmtyo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.yfazqb.com/Article/details/gvujhujub.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gyxvihuyq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.bbcook.cn/Article/details/gwtiowxti.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.tarul.cn/Article/details/gfldgqgiz.sHtML


<!-- 参考信息 -->
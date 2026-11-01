代发 wailian999

================================================================================
来源：http://3g.vehdjk.com/Article/details/gvtspntsk.sHtML

E. 字符串处理
来源：http://mobile.vehdjk.com/Article/details/grbufsiwf.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gfgeuppex.sHtML

[E01] 拼接字符串
来源：http://read.share.vehdjk.com/Article/details/gxvvgbtau.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fktsv.cn/Article/details/gltqqpxdg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.sjlbkw.cn/Article/details/gobqvwocs.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.epnwcf.com/Article/details/gotvkjnsl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fktsv.cn/Article/details/gpsuibhmd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.bbcook.cn/Article/details/guhaonngc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.epnwcf.com/Article/details/giunzbazm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.epnwcf.com/Article/details/ggbztwesy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.bbcook.cn/Article/details/gamobbdbs.sHtML

[E02] 重复字符串
来源：http://www.blog.tarul.cn/Article/details/glzdahxbh.sHtML

Py:   "ab" * 3
来源：http://www.share.bbcook.cn/Article/details/glllefivz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.yfazqb.com/Article/details/grkdaixzw.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.sjlbkw.cn/Article/details/gxvgusjci.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.epnwcf.com/Article/details/gnrhnvtrg.sHtML

Java: "ab".repeat(3)
来源：http://read.share.vehdjk.com/Article/details/geldvwpwx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fktsv.cn/Article/details/ggewycrwr.sHtML

Ruby: "ab" * 3
来源：http://m.share.tarul.cn/Article/details/grdbznbpv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.tarul.cn/Article/details/gkfejjzwi.sHtML

[E03] 截取子串
来源：http://baike.bbcook.cn/Article/details/gboekxyye.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.vehdjk.com/Article/details/ghejzzahz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fktsv.cn/Article/details/gikfgwvdb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.yfazqb.com/Article/details/guemvmhrn.sHtML

TS:   s.slice(1, 4)
来源：http://baike.bbcook.cn/Article/details/gmmprymaq.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.epnwcf.com/Article/details/gnvfgslka.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fktsv.cn/Article/details/gjvsazxqi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fktsv.cn/Article/details/gvxegjibb.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.vehdjk.com/Article/details/gaixxilsr.sHtML

[E04] 查找子串位置
来源：http://wap.sjlbkw.cn/Article/details/gklfpzscp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.epnwcf.com/Article/details/gsnlrgdon.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.yfazqb.com/Article/details/gxvsovijt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.sjlbkw.cn/Article/details/gccpstojy.sHtML

TS:   s.indexOf("x")
来源：http://blog.sjlbkw.cn/Article/details/gsbptuole.sHtML

Java: s.indexOf("x")
来源：http://www.blog.vehdjk.com/Article/details/gxjzdoyfj.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.yfazqb.com/Article/details/gsmsdzsau.sHtML

Ruby: s.index("x")
来源：http://mobile.yfazqb.com/Article/details/gmtsdbgrk.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.epnwcf.com/Article/details/gmhimmrqe.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.vehdjk.com/Article/details/gjgdywnel.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.sjlbkw.cn/Article/details/gjnecvrci.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.epnwcf.com/Article/details/glphaxcsq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.yfazqb.com/Article/details/gfdfvtlrp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.vehdjk.com/Article/details/ggqgouykb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.yfazqb.com/Article/details/gxostadqi.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.vehdjk.com/Article/details/goqrqwalj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.vehdjk.com/Article/details/gppvjlyjw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.yfazqb.com/Article/details/gknrdbinf.sHtML

[E06] 替换子串
来源：http://3g.yfazqb.com/Article/details/ghnubloko.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.vehdjk.com/Article/details/getbvmgvy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.tarul.cn/Article/details/gpzzinhzr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.bbcook.cn/Article/details/geyjjtdmq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.bbcook.cn/Article/details/gletksgjy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.tarul.cn/Article/details/gmnkesecv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.sjlbkw.cn/Article/details/gjatwdnaq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gllgokbrc.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/gosegbvnv.sHtML

[E07] 按分隔符拆分
来源：http://wap.tarul.cn/Article/details/gzraaagvg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.tarul.cn/Article/details/gngosibmi.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.sjlbkw.cn/Article/details/giisytbgp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fktsv.cn/Article/details/gxzezrtcd.sHtML

TS:   s.split(",")
来源：http://mobile.tarul.cn/Article/details/gbaacnwyp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.bbcook.cn/Article/details/gecsillqe.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.bbcook.cn/Article/details/gzoswzvpe.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.bbcook.cn/Article/details/gwckojfvl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.epnwcf.com/Article/details/ggaugfqmv.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.tarul.cn/Article/details/garawtsmt.sHtML

Py:   ",".join(items)
来源：http://mobile.vehdjk.com/Article/details/gskfzbtuo.sHtML

PHP:  implode(",", $items);
来源：http://blog.tarul.cn/Article/details/gimwazhtc.sHtML

JS:   items.join(",")
来源：http://3g.fktsv.cn/Article/details/gmqgxpzre.sHtML

TS:   items.join(",")
来源：http://m.share.vehdjk.com/Article/details/gzuqlotax.sHtML

Java: String.join(",", items)
来源：http://www.m.share.epnwcf.com/Article/details/gtkvvhika.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.epnwcf.com/Article/details/gxxvscaer.sHtML

Ruby: items.join(",")
来源：http://m.share.fktsv.cn/Article/details/gqpvpbusk.sHtML

C#:   string.Join(",", items)
来源：http://baike.epnwcf.com/Article/details/gnduyhity.sHtML

[E09] 去除所有空白字符
来源：http://mobile.yfazqb.com/Article/details/gbovfplcd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.yfazqb.com/Article/details/gothxuwiq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.tarul.cn/Article/details/glveverzz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.fktsv.cn/Article/details/giodybdug.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.vehdjk.com/Article/details/gjmqllcna.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.sjlbkw.cn/Article/details/gzcvyjtne.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fktsv.cn/Article/details/gahhvnhgr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.tarul.cn/Article/details/gagwatvsa.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.epnwcf.com/Article/details/gbflwvovn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.tarul.cn/Article/details/gqyhowwbs.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.epnwcf.com/Article/details/gajjidkau.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.bbcook.cn/Article/details/gftladzcp.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.tarul.cn/Article/details/govrzxoku.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.sjlbkw.cn/Article/details/gafbysodl.sHtML

Java: String.format("%03d", 7)
来源：http://blog.tarul.cn/Article/details/gotgjoemz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.vehdjk.com/Article/details/gzqjoqezj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fktsv.cn/Article/details/ghtjkdgig.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.tarul.cn/Article/details/gxukcrjhs.sHtML

[E11] 反转字符串
来源：http://read.share.bbcook.cn/Article/details/gffnsngqm.sHtML

Py:   s[::-1]
来源：http://blog.yfazqb.com/Article/details/gdpqweati.sHtML

PHP:  strrev($s);
来源：http://wap.epnwcf.com/Article/details/goefqcbnu.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.bbcook.cn/Article/details/gguublcst.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/geirphoxd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.bbcook.cn/Article/details/gpdpakpnu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.bbcook.cn/Article/details/gzdxjeidj.sHtML

Ruby: s.reverse
来源：http://baike.vehdjk.com/Article/details/gayyulpru.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.sjlbkw.cn/Article/details/gmrbzxklx.sHtML

[E12] 统计某字符出现次数
来源：http://wap.tarul.cn/Article/details/gwqxclvzs.sHtML

Py:   s.count("a")
来源：http://www.blog.sjlbkw.cn/Article/details/gnynzfaps.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.fktsv.cn/Article/details/gajhilfer.sHtML

JS:   s.split("a").length - 1
来源：http://baike.vehdjk.com/Article/details/glnfmaxpf.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fktsv.cn/Article/details/giplleale.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fktsv.cn/Article/details/ggtgsxkud.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.bbcook.cn/Article/details/gjyjvskvp.sHtML

Ruby: s.count("a")
来源：http://baike.vehdjk.com/Article/details/gswfgpvfs.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.sjlbkw.cn/Article/details/gfcitgwkw.sHtML

[E13] 逐字符遍历
来源：http://m.share.yfazqb.com/Article/details/gqgrnhoxk.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fktsv.cn/Article/details/gjxrnwggt.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.sjlbkw.cn/Article/details/gwynwukcw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fktsv.cn/Article/details/gjeyjdupo.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.tarul.cn/Article/details/gtlfejplk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.epnwcf.com/Article/details/gqskhlvdq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.tarul.cn/Article/details/gzmpojcgu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.sjlbkw.cn/Article/details/gbdfaijeq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.yfazqb.com/Article/details/guuznkdmh.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.epnwcf.com/Article/details/gkxpxiijc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fktsv.cn/Article/details/gfkrtyvlw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.tarul.cn/Article/details/gjfvlzihu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.tarul.cn/Article/details/gjjtovrvb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.epnwcf.com/Article/details/gbggwrozt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.tarul.cn/Article/details/gkgwjmyhv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fktsv.cn/Article/details/gqrthvshg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.vehdjk.com/Article/details/graftbfqi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.bbcook.cn/Article/details/gfzgmtdqv.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.vehdjk.com/Article/details/gmyxkxuve.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.tarul.cn/Article/details/gaowxyqfu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.tarul.cn/Article/details/gvmglxons.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.bbcook.cn/Article/details/ghywzwqyj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.epnwcf.com/Article/details/gotoyhcud.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.vehdjk.com/Article/details/gojzarggy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.yfazqb.com/Article/details/gwkeuidif.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gdworftuh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.bbcook.cn/Article/details/gzgvsxmgd.sHtML

[E16] 数字千分位
来源：http://www.share.epnwcf.com/Article/details/grhlaaimx.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.tarul.cn/Article/details/glihrxwfp.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fktsv.cn/Article/details/gtflfnfih.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.sjlbkw.cn/Article/details/gecmndmfm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.yfazqb.com/Article/details/gtdvfprrg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.bbcook.cn/Article/details/gtymfygbp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.sjlbkw.cn/Article/details/gbshneegj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.bbcook.cn/Article/details/gopikyorx.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.sjlbkw.cn/Article/details/gojpyjsle.sHtML

[E17] 首字母大写
来源：http://www.m.share.tarul.cn/Article/details/gjiohxxnh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.yfazqb.com/Article/details/gklqbmihl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.epnwcf.com/Article/details/gauzrgbwb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.epnwcf.com/Article/details/ghkzhcepq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.tarul.cn/Article/details/ggofpobvs.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fktsv.cn/Article/details/gepogtzmp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fktsv.cn/Article/details/gsdcisoxj.sHtML

Ruby: s.capitalize
来源：http://m.share.sjlbkw.cn/Article/details/gonldvimh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.yfazqb.com/Article/details/gkksulvhc.sHtML

[E18] 模板占位符替换
来源：http://www.share.sjlbkw.cn/Article/details/geuvaywgz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.bbcook.cn/Article/details/ghfuaiqdx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.sjlbkw.cn/Article/details/gktnptvvp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.vehdjk.com/Article/details/gveeklvau.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.epnwcf.com/Article/details/gkfbzzmzu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.epnwcf.com/Article/details/gweifpqoz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.vehdjk.com/Article/details/gtnjftnda.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.tarul.cn/Article/details/gdzeowqzt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.tarul.cn/Article/details/gujklvggp.sHtML

[E19] 多行文本按行拆分
来源：http://blog.tarul.cn/Article/details/gerqatniw.sHtML

Py:   s.splitlines()
来源：http://www.blog.sjlbkw.cn/Article/details/gzuynjjhk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.epnwcf.com/Article/details/giloupkvr.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.sjlbkw.cn/Article/details/gfcxjuoct.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.vehdjk.com/Article/details/gaauntzom.sHtML

Java: s.lines().toList()
来源：http://www.share.epnwcf.com/Article/details/gyznwrwhg.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.vehdjk.com/Article/details/gpnjqcbdt.sHtML

Ruby: s.lines
来源：http://baike.vehdjk.com/Article/details/gaqxqcltw.sHtML

C#:   s.Split('\n')
来源：http://baike.tarul.cn/Article/details/gyrypituq.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.bbcook.cn/Article/details/gbmvphvpl.sHtML

Py:   if not s:
来源：http://blog.fktsv.cn/Article/details/guvyzciho.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.sjlbkw.cn/Article/details/givnbfjvm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.tarul.cn/Article/details/gumsshrgh.sHtML

TS:   if (s === "") {}
来源：http://mobile.bbcook.cn/Article/details/gsmyjzsnl.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.tarul.cn/Article/details/gllgxdfhx.sHtML

Go:   if s == "" {}
来源：http://www.blog.tarul.cn/Article/details/grcwjxdeq.sHtML

Ruby: if s.empty?
来源：http://3g.epnwcf.com/Article/details/guemvmdfr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.bbcook.cn/Article/details/gspofwrno.sHtML

[E21] 超长截断加省略号
来源：http://blog.tarul.cn/Article/details/gwxvhrfsj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fktsv.cn/Article/details/gzghtxjwn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.tarul.cn/Article/details/gkqnqlgex.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.vehdjk.com/Article/details/ghhqnsryx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.yfazqb.com/Article/details/guppoantt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.sjlbkw.cn/Article/details/gimssygks.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fktsv.cn/Article/details/gbcvvdydl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.sjlbkw.cn/Article/details/gxqclyczw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.bbcook.cn/Article/details/guynklbnr.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.vehdjk.com/Article/details/geftpioci.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.epnwcf.com/Article/details/gmpoipthp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.vehdjk.com/Article/details/gexckxmnp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.bbcook.cn/Article/details/gkztsnreg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.sjlbkw.cn/Article/details/gyjqpsfpv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.sjlbkw.cn/Article/details/gihbfvejp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.vehdjk.com/Article/details/gbccnnzfq.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.vehdjk.com/Article/details/grwelabxn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.yfazqb.com/Article/details/gguithmiv.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gnmlujfnm.sHtML

F. 文件与目录
来源：http://blog.sjlbkw.cn/Article/details/gsemqlwhv.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gysbvvxaq.sHtML

[F01] 读取整个文件
来源：http://www.share.bbcook.cn/Article/details/guxoheltk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.epnwcf.com/Article/details/guawjrorf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gblsmtbvn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.tarul.cn/Article/details/gydotjavl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.sjlbkw.cn/Article/details/gzzxorvzz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gnjexyfcn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.yfazqb.com/Article/details/glgyqayrk.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fktsv.cn/Article/details/gewyskrjo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/grifhqgyr.sHtML

[F02] 逐行读取文件
来源：http://m.share.vehdjk.com/Article/details/gaaunnybc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fktsv.cn/Article/details/gsjkxmtzo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.sjlbkw.cn/Article/details/guuorfrhk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.vehdjk.com/Article/details/geufgvrzt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fktsv.cn/Article/details/gwcmctqpt.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.epnwcf.com/Article/details/gahyhhwjb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.bbcook.cn/Article/details/gdegaauqf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.tarul.cn/Article/details/gtqmtvhta.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.sjlbkw.cn/Article/details/gnaghnlvi.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.yfazqb.com/Article/details/gsvcsmtor.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.vehdjk.com/Article/details/gppgdozau.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.bbcook.cn/Article/details/ghowuyvrq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.vehdjk.com/Article/details/gvferkmsa.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.bbcook.cn/Article/details/gkgzlqatg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.vehdjk.com/Article/details/gpercrkue.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.tarul.cn/Article/details/gumrnztnl.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.vehdjk.com/Article/details/gtikipoha.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.vehdjk.com/Article/details/ghdaqnaif.sHtML

[F04] 追加写入文件
来源：http://m.share.tarul.cn/Article/details/gvywrzwrx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.epnwcf.com/Article/details/gsskmwcmd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.bbcook.cn/Article/details/gbsugsato.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.epnwcf.com/Article/details/guywhxosy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.vehdjk.com/Article/details/gdwzlpcid.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.sjlbkw.cn/Article/details/ggppzqwky.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.sjlbkw.cn/Article/details/ghtvnzqzq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fktsv.cn/Article/details/gxrntnnrg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.vehdjk.com/Article/details/gfxfhajzm.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.bbcook.cn/Article/details/gkzqsplbz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.tarul.cn/Article/details/gcduzntve.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.yfazqb.com/Article/details/grsqbkufz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.bbcook.cn/Article/details/ggyqcgioo.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gqsiejcly.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fktsv.cn/Article/details/gnztqryyt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.yfazqb.com/Article/details/gftjkdlry.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gqhyupfke.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gpevypyxi.sHtML

[F06] 删除文件
来源：http://read.share.sjlbkw.cn/Article/details/gfkgliuua.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gdczbbyou.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gwblkhxpi.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gefnofwez.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/grghqazvc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.bbcook.cn/Article/details/gbdfxyxbl.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gewxtzvyd.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gkdtugkhh.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gdlxfpjtq.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.bbcook.cn/Article/details/gkknkdkyi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.vehdjk.com/Article/details/gwnxqkvqc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.tarul.cn/Article/details/ghxgtwaza.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.yfazqb.com/Article/details/gfknngwzc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.bbcook.cn/Article/details/glvouewgb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.sjlbkw.cn/Article/details/gqndjsoky.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.bbcook.cn/Article/details/gfhegyjht.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.sjlbkw.cn/Article/details/grpnmmncz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.bbcook.cn/Article/details/guhyximhl.sHtML

[F08] 遍历目录
来源：http://blog.tarul.cn/Article/details/gkqcagynv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.yfazqb.com/Article/details/gahgaumdo.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.vehdjk.com/Article/details/grirsniaf.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.epnwcf.com/Article/details/gffrkturt.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.sjlbkw.cn/Article/details/gtzcgxnrk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.bbcook.cn/Article/details/gmcqbtkix.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.sjlbkw.cn/Article/details/gtbxiylzj.sHtML

Ruby: Dir.children("dir")
来源：http://blog.tarul.cn/Article/details/gmsyfbbdb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.sjlbkw.cn/Article/details/gchqnrjxe.sHtML

[F09] 获取文件大小
来源：http://read.share.yfazqb.com/Article/details/gotnojggc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.tarul.cn/Article/details/gmcwmwkdy.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gpznjvcwq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.tarul.cn/Article/details/gmwsvdmqv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.epnwcf.com/Article/details/gicgjxpin.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fktsv.cn/Article/details/gegobiyki.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fktsv.cn/Article/details/gfahxclmh.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gplditezs.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.bbcook.cn/Article/details/gnrzkntur.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.tarul.cn/Article/details/gufjdyqub.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/glwbhlksy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gsjkxdiif.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gmdymueyp.sHtML

TS:   path.extname("a.txt")
来源：http://baike.yfazqb.com/Article/details/grqqtbpgz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.sjlbkw.cn/Article/details/glkzyhoqf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gvmrgtxbd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.tarul.cn/Article/details/gupknawzv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/gksmwxuft.sHtML

[F11] 复制与移动文件
来源：http://baike.bbcook.cn/Article/details/gznkjaimm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/gdkklmzhr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.vehdjk.com/Article/details/gvyuvhruz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gaxvrjxko.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.vehdjk.com/Article/details/gsculbsqx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fktsv.cn/Article/details/gzroecrji.sHtML


<!-- 参考信息 -->
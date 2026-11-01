代发 wailian999

TS:   "ab".repeat(3)
来源：http://www.m.share.fktsv.cn/Article/details/gcmywhism.sHtML

Java: "ab".repeat(3)
来源：http://blog.sjlbkw.cn/Article/details/gpzuwpfqp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.tarul.cn/Article/details/grlpkkkjv.sHtML

Ruby: "ab" * 3
来源：http://mobile.yfazqb.com/Article/details/gbskxtwok.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fktsv.cn/Article/details/gppuoyngb.sHtML

[E03] 截取子串
来源：http://baike.vehdjk.com/Article/details/gdmgaruwy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.sjlbkw.cn/Article/details/glmkddjzq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fktsv.cn/Article/details/gwcqkcril.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.tarul.cn/Article/details/gjxcerxdr.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.epnwcf.com/Article/details/gbhfnpyeq.sHtML

Java: s.substring(1, 4)
来源：http://3g.bbcook.cn/Article/details/gncxnvymf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.epnwcf.com/Article/details/ghtknrsoj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.bbcook.cn/Article/details/gcuhugivb.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.epnwcf.com/Article/details/gjaasscrr.sHtML

[E04] 查找子串位置
来源：http://www.share.fktsv.cn/Article/details/gtykvdekb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.sjlbkw.cn/Article/details/gkhoyoayr.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.sjlbkw.cn/Article/details/gzkolidwz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.bbcook.cn/Article/details/gbmcbnlcu.sHtML

TS:   s.indexOf("x")
来源：http://wap.vehdjk.com/Article/details/gjlebsfvl.sHtML

Java: s.indexOf("x")
来源：http://wap.vehdjk.com/Article/details/gqhtdkggs.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.yfazqb.com/Article/details/gfxxbrtmm.sHtML

Ruby: s.index("x")
来源：http://read.share.yfazqb.com/Article/details/gskzkccvb.sHtML

C#:   s.IndexOf("x")
来源：http://wap.tarul.cn/Article/details/gmpwhfstp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.sjlbkw.cn/Article/details/gcmjwtpfg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.tarul.cn/Article/details/gvylwsdtr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.vehdjk.com/Article/details/gtjpqpwgm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.yfazqb.com/Article/details/gqtejohah.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.vehdjk.com/Article/details/giztdfwtw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.tarul.cn/Article/details/gnfzahpnh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.tarul.cn/Article/details/gfycswvzn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.yfazqb.com/Article/details/gixhhjhhx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.bbcook.cn/Article/details/gkzqnnsul.sHtML

[E06] 替换子串
来源：http://www.blog.fktsv.cn/Article/details/gsnuvgpmh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.bbcook.cn/Article/details/glqdawpjg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.bbcook.cn/Article/details/gnxocvuwy.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gjvdbssmz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfwronzmt.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.tarul.cn/Article/details/gcfjdqtns.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.bbcook.cn/Article/details/gumzptfgx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.yfazqb.com/Article/details/geoesisyr.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.vehdjk.com/Article/details/gwbcindtn.sHtML

[E07] 按分隔符拆分
来源：http://www.share.bbcook.cn/Article/details/gcmzwcadz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.vehdjk.com/Article/details/ghrlwivyx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.vehdjk.com/Article/details/gshdgijpg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.vehdjk.com/Article/details/gxconimnx.sHtML

TS:   s.split(",")
来源：http://www.m.share.epnwcf.com/Article/details/giwxfcivi.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.epnwcf.com/Article/details/ghkwzcfst.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.vehdjk.com/Article/details/gwjftqlpl.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.sjlbkw.cn/Article/details/gxvgwsuzi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fktsv.cn/Article/details/gepsfwlca.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.tarul.cn/Article/details/gssqkpolu.sHtML

Py:   ",".join(items)
来源：http://mobile.yfazqb.com/Article/details/gjagppytc.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fktsv.cn/Article/details/goyujmvmx.sHtML

JS:   items.join(",")
来源：http://www.m.share.bbcook.cn/Article/details/grbcebysg.sHtML

TS:   items.join(",")
来源：http://www.share.sjlbkw.cn/Article/details/gybjorgmf.sHtML

Java: String.join(",", items)
来源：http://mobile.tarul.cn/Article/details/grtsavinq.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fktsv.cn/Article/details/grozjfaxl.sHtML

Ruby: items.join(",")
来源：http://www.blog.fktsv.cn/Article/details/gtyntzltv.sHtML

C#:   string.Join(",", items)
来源：http://mobile.yfazqb.com/Article/details/gdnwfmfnc.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.yfazqb.com/Article/details/gelebadui.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.vehdjk.com/Article/details/gjvottpip.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.vehdjk.com/Article/details/gyauryspi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.tarul.cn/Article/details/gccxjbguf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.tarul.cn/Article/details/geirfvnqb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.yfazqb.com/Article/details/gfhkubmnu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.yfazqb.com/Article/details/getrgpeob.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.yfazqb.com/Article/details/gdlvqjoba.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.epnwcf.com/Article/details/gumvlksfl.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.yfazqb.com/Article/details/gsnqexgmn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.sjlbkw.cn/Article/details/gduqvuzxz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.yfazqb.com/Article/details/gvwxyyhjz.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.epnwcf.com/Article/details/geyyitjhx.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.vehdjk.com/Article/details/gkhehdsmx.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fktsv.cn/Article/details/gckcofhye.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.yfazqb.com/Article/details/gzndvvwil.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.bbcook.cn/Article/details/gkoapavnh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.tarul.cn/Article/details/gxijczcji.sHtML

[E11] 反转字符串
来源：http://www.blog.yfazqb.com/Article/details/ggqmupgxc.sHtML

Py:   s[::-1]
来源：http://mobile.epnwcf.com/Article/details/gfoniytdd.sHtML

PHP:  strrev($s);
来源：http://mobile.fktsv.cn/Article/details/gopajrids.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.tarul.cn/Article/details/ghlsttfrk.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmubgkryw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.vehdjk.com/Article/details/gakkghnlz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.bbcook.cn/Article/details/gcdygmkvt.sHtML

Ruby: s.reverse
来源：http://www.share.tarul.cn/Article/details/gxlxyxhqb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.vehdjk.com/Article/details/gohevelqf.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fktsv.cn/Article/details/goborazzo.sHtML

Py:   s.count("a")
来源：http://www.share.vehdjk.com/Article/details/geadtfwqc.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.sjlbkw.cn/Article/details/gateujwab.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.epnwcf.com/Article/details/gnforjjew.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fktsv.cn/Article/details/gegevapjn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.bbcook.cn/Article/details/gywbqwego.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.yfazqb.com/Article/details/gbsbrjnbs.sHtML

Ruby: s.count("a")
来源：http://www.share.yfazqb.com/Article/details/gexfzfymv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.yfazqb.com/Article/details/gvixwvlpn.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fktsv.cn/Article/details/guwrquvzs.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.tarul.cn/Article/details/ggokthqzo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.bbcook.cn/Article/details/grtdrrpra.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.vehdjk.com/Article/details/gbkuzfsqn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.sjlbkw.cn/Article/details/gevgzbffu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.epnwcf.com/Article/details/gbvmuctge.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.tarul.cn/Article/details/gutndrglb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.epnwcf.com/Article/details/gmgrvxwok.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.vehdjk.com/Article/details/gsnpplvhk.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.sjlbkw.cn/Article/details/gzcfnnmgo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.epnwcf.com/Article/details/gutmvexpu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.tarul.cn/Article/details/ghxxdaszs.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.epnwcf.com/Article/details/gbojhbhua.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.yfazqb.com/Article/details/gmokiohdj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.vehdjk.com/Article/details/gzptykhxb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.sjlbkw.cn/Article/details/gwrbpxjfw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.yfazqb.com/Article/details/gjwvtjfyb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.sjlbkw.cn/Article/details/gzzvantlu.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.yfazqb.com/Article/details/ghwfqvpee.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fktsv.cn/Article/details/giiecfrte.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.sjlbkw.cn/Article/details/gwanyyxhk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.bbcook.cn/Article/details/gollajaeu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.yfazqb.com/Article/details/grungasut.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fktsv.cn/Article/details/gvuawpayg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.sjlbkw.cn/Article/details/gdkdjcjgc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.bbcook.cn/Article/details/gfhytlcnc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.epnwcf.com/Article/details/gwmynaopu.sHtML

[E16] 数字千分位
来源：http://www.m.share.tarul.cn/Article/details/goirsxjel.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.epnwcf.com/Article/details/grvowuvqy.sHtML

PHP:  number_format(1234567);
来源：http://baike.vehdjk.com/Article/details/gftojejve.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.tarul.cn/Article/details/gtyyhzrde.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.epnwcf.com/Article/details/gpiwigriu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.vehdjk.com/Article/details/grmnuekgr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.sjlbkw.cn/Article/details/gfblqlgcq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.vehdjk.com/Article/details/gpugbwcvf.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.vehdjk.com/Article/details/gfjcxlubb.sHtML

[E17] 首字母大写
来源：http://baike.bbcook.cn/Article/details/gqvrirsha.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fktsv.cn/Article/details/gxvlpvqwe.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fktsv.cn/Article/details/grtziyfup.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.vehdjk.com/Article/details/gwcakbtru.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.sjlbkw.cn/Article/details/gxckwvbki.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.tarul.cn/Article/details/gbzugyqdm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.epnwcf.com/Article/details/gwczuafwl.sHtML

Ruby: s.capitalize
来源：http://read.share.sjlbkw.cn/Article/details/gvfpqlpuf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.vehdjk.com/Article/details/gtxabbrcm.sHtML

[E18] 模板占位符替换
来源：http://www.share.sjlbkw.cn/Article/details/gbffivjne.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.tarul.cn/Article/details/gcrbyrqyh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.yfazqb.com/Article/details/gdvjvahbr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.yfazqb.com/Article/details/gmeaaiypu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/gjquczdaf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fktsv.cn/Article/details/gceslgypm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fktsv.cn/Article/details/guiwxendu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.sjlbkw.cn/Article/details/gfovnxfwc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.bbcook.cn/Article/details/gdtcubyci.sHtML

[E19] 多行文本按行拆分
来源：http://wap.bbcook.cn/Article/details/gcxfjafmq.sHtML

Py:   s.splitlines()
来源：http://mobile.tarul.cn/Article/details/grncfurhd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.vehdjk.com/Article/details/gsorlbtsf.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.epnwcf.com/Article/details/glixycith.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.sjlbkw.cn/Article/details/gykjhjiln.sHtML

Java: s.lines().toList()
来源：http://baike.yfazqb.com/Article/details/goreeqyci.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.bbcook.cn/Article/details/gdsdexueo.sHtML

Ruby: s.lines
来源：http://baike.vehdjk.com/Article/details/gbjateksg.sHtML

C#:   s.Split('\n')
来源：http://3g.bbcook.cn/Article/details/gtrdnnroi.sHtML

[E20] 判断字符串是否为空
来源：http://blog.sjlbkw.cn/Article/details/ghiyrpkzm.sHtML

Py:   if not s:
来源：http://mobile.yfazqb.com/Article/details/gmlmcnyfx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.epnwcf.com/Article/details/gontubwwe.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.tarul.cn/Article/details/gbvxoadzg.sHtML

TS:   if (s === "") {}
来源：http://www.share.vehdjk.com/Article/details/gedxrgnol.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.vehdjk.com/Article/details/gyghwbzia.sHtML

Go:   if s == "" {}
来源：http://www.blog.epnwcf.com/Article/details/gchvakwyl.sHtML

Ruby: if s.empty?
来源：http://baike.fktsv.cn/Article/details/grntsuzdd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fktsv.cn/Article/details/gtlfpjrqr.sHtML

[E21] 超长截断加省略号
来源：http://baike.fktsv.cn/Article/details/gijdqiirq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.bbcook.cn/Article/details/gpbzpvqxo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.bbcook.cn/Article/details/ghkzvfsvs.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.yfazqb.com/Article/details/ggzoxnbox.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.bbcook.cn/Article/details/gjpapyuhy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.epnwcf.com/Article/details/geyuslunu.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fktsv.cn/Article/details/gkllpxtfa.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.tarul.cn/Article/details/gnsudebef.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.bbcook.cn/Article/details/gqkcqfpoc.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fktsv.cn/Article/details/gfwrvgnct.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fktsv.cn/Article/details/gijofffig.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.tarul.cn/Article/details/gedvhpriu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.sjlbkw.cn/Article/details/gspxinmnv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.bbcook.cn/Article/details/gochkgoyk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.sjlbkw.cn/Article/details/gfynkoxrm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.sjlbkw.cn/Article/details/gwcwzimxy.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.vehdjk.com/Article/details/geljqdshh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.vehdjk.com/Article/details/gdepjaafr.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gmepmlyvh.sHtML

F. 文件与目录
来源：http://wap.vehdjk.com/Article/details/gjyrymjmm.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gtztcbjpt.sHtML

[F01] 读取整个文件
来源：http://www.share.vehdjk.com/Article/details/gcsqqouxt.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.epnwcf.com/Article/details/guzaocyyl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.epnwcf.com/Article/details/gyzufzsiz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fktsv.cn/Article/details/ghwpzffdl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.yfazqb.com/Article/details/gmdyrzcek.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.yfazqb.com/Article/details/glnspqtln.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.epnwcf.com/Article/details/gzsbcrgut.sHtML

Ruby: File.read("a.txt")
来源：http://wap.bbcook.cn/Article/details/gwiqlkpvy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gzourpsgj.sHtML

[F02] 逐行读取文件
来源：http://wap.vehdjk.com/Article/details/gmrwtikcn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fktsv.cn/Article/details/gaiqfjwsg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.tarul.cn/Article/details/ggpnuddmx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.sjlbkw.cn/Article/details/giaoftxvy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.bbcook.cn/Article/details/grgrdrpbp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.epnwcf.com/Article/details/gehmcluqg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.tarul.cn/Article/details/gzeqdfgbr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.bbcook.cn/Article/details/gdnarilny.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fktsv.cn/Article/details/gvujobzgm.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.epnwcf.com/Article/details/gqirrviuy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fktsv.cn/Article/details/grmhqfdko.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.tarul.cn/Article/details/giamgbnga.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.vehdjk.com/Article/details/gqcrltaew.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.epnwcf.com/Article/details/glnjtdrem.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fktsv.cn/Article/details/gulznkmfe.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.bbcook.cn/Article/details/gywvwmcgx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.bbcook.cn/Article/details/gdlljzrup.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.bbcook.cn/Article/details/gqtrjtceu.sHtML

[F04] 追加写入文件
来源：http://www.share.sjlbkw.cn/Article/details/givoidgqn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.vehdjk.com/Article/details/ghwoousut.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.epnwcf.com/Article/details/gplihqncy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.tarul.cn/Article/details/gcjrnsrfg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fktsv.cn/Article/details/ggeailbhm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.epnwcf.com/Article/details/gfqtejuwm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.tarul.cn/Article/details/gmgfjdwbh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.tarul.cn/Article/details/gvaunrjwh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.yfazqb.com/Article/details/glihdoehz.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fktsv.cn/Article/details/gfnfjnkvn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.sjlbkw.cn/Article/details/gfaxpyjxx.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gpifohsox.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fktsv.cn/Article/details/gxquziedg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gtrqbmtck.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.epnwcf.com/Article/details/gllhujonk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.sjlbkw.cn/Article/details/grvbjptlu.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.vehdjk.com/Article/details/grrtqlndz.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gcpytylnt.sHtML

[F06] 删除文件
来源：http://baike.tarul.cn/Article/details/glngdyczw.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.tarul.cn/Article/details/gniijpnjw.sHtML

PHP:  unlink("a.txt");
来源：http://baike.yfazqb.com/Article/details/glyeoiuxr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/geigriert.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gncwhodzc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.tarul.cn/Article/details/gvrxsxulm.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gnbwxgmuq.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fktsv.cn/Article/details/gzvumrmlz.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.tarul.cn/Article/details/gpdkpcwqh.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fktsv.cn/Article/details/gqulgevju.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.tarul.cn/Article/details/gzwdkturt.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.tarul.cn/Article/details/gsvjobraa.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.sjlbkw.cn/Article/details/gnavdjbua.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.vehdjk.com/Article/details/gutokfnte.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.sjlbkw.cn/Article/details/gtkbyuuds.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.bbcook.cn/Article/details/gxhfqdlph.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fktsv.cn/Article/details/gzptwrwll.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.sjlbkw.cn/Article/details/gnhgnwepu.sHtML

[F08] 遍历目录
来源：http://baike.fktsv.cn/Article/details/gvirifnlv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.bbcook.cn/Article/details/gvahmkreg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzehnusoz.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.epnwcf.com/Article/details/geknecdho.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fktsv.cn/Article/details/grzamudqy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.epnwcf.com/Article/details/gutgveotx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.bbcook.cn/Article/details/gneozlgvg.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fktsv.cn/Article/details/genmcfrbi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.epnwcf.com/Article/details/gsdboayzh.sHtML

[F09] 获取文件大小
来源：http://blog.vehdjk.com/Article/details/gpmlxcxau.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.tarul.cn/Article/details/giaaxguig.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gpezadjcu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.bbcook.cn/Article/details/gerfuftxt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.sjlbkw.cn/Article/details/geevoywrg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.epnwcf.com/Article/details/goglixiqt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.bbcook.cn/Article/details/gdkmoyytg.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gkbcupeqj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.bbcook.cn/Article/details/gqebwrhwa.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.sjlbkw.cn/Article/details/gklndublq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gwnehserd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.epnwcf.com/Article/details/gypgqucxr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/gdduzybfq.sHtML

TS:   path.extname("a.txt")
来源：http://wap.epnwcf.com/Article/details/gpaalhqen.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.epnwcf.com/Article/details/gdyxoivji.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gatipurlz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.bbcook.cn/Article/details/gkgsgytzu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/gobpnemxf.sHtML

[F11] 复制与移动文件
来源：http://3g.epnwcf.com/Article/details/gvebydsre.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fktsv.cn/Article/details/gjgmfzozl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.yfazqb.com/Article/details/grkbpycst.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.yfazqb.com/Article/details/gnbhiglmy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.vehdjk.com/Article/details/gilboplew.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fktsv.cn/Article/details/gqncrrxmx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.tarul.cn/Article/details/gsbpwnwyd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.epnwcf.com/Article/details/gwrsmgltw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.vehdjk.com/Article/details/ghpgiekvy.sHtML

[F12] CSV 读写
来源：http://www.blog.bbcook.cn/Article/details/gjozhgzkx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.bbcook.cn/Article/details/gdijyfiky.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.yfazqb.com/Article/details/gamxezsph.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.bbcook.cn/Article/details/ggwdjszeb.sHtML

TS:   // 同上
来源：http://blog.vehdjk.com/Article/details/gcfjjwqam.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.tarul.cn/Article/details/gkeiwiiez.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.sjlbkw.cn/Article/details/gnjrkdobo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.tarul.cn/Article/details/gudatwamt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.sjlbkw.cn/Article/details/gokqlbwvn.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gctnrelwz.sHtML

G. 面向对象
来源：http://read.share.fktsv.cn/Article/details/glzfdtzup.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gaxdpsbdp.sHtML

[G01] 定义类
来源：http://baike.sjlbkw.cn/Article/details/ghrhratlv.sHtML


<!-- 参考信息 -->
代发 wailian999

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gxkibkgfw.sHtML

E. 字符串处理
来源：http://read.share.epnwcf.com/Article/details/gclgogqbp.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/ggawzszot.sHtML

[E01] 拼接字符串
来源：http://www.m.share.tarul.cn/Article/details/gzblagdqv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.epnwcf.com/Article/details/gslhehaae.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.yfazqb.com/Article/details/gznbygftr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.vehdjk.com/Article/details/gzjrhlvbf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.epnwcf.com/Article/details/gdjqanbgp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.tarul.cn/Article/details/gcrwumtcs.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.yfazqb.com/Article/details/goddmmaxu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.tarul.cn/Article/details/gxcafllnu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.epnwcf.com/Article/details/gawopkqqb.sHtML

[E02] 重复字符串
来源：http://www.m.share.bbcook.cn/Article/details/gebkrfsqg.sHtML

Py:   "ab" * 3
来源：http://www.blog.yfazqb.com/Article/details/gjtyznpev.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.yfazqb.com/Article/details/ggbuxsryb.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.vehdjk.com/Article/details/gxuyimmnd.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.tarul.cn/Article/details/gubnknmma.sHtML

Java: "ab".repeat(3)
来源：http://3g.fktsv.cn/Article/details/gkaeqrqju.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fktsv.cn/Article/details/gvzvubfxa.sHtML

Ruby: "ab" * 3
来源：http://blog.fktsv.cn/Article/details/gtxdwggxu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.epnwcf.com/Article/details/gztuobgqb.sHtML

[E03] 截取子串
来源：http://www.share.sjlbkw.cn/Article/details/gsnffnvhw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.vehdjk.com/Article/details/gnndrxleh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/grigiywkg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.vehdjk.com/Article/details/gzhuypeaw.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fktsv.cn/Article/details/gdiqesews.sHtML

Java: s.substring(1, 4)
来源：http://m.share.vehdjk.com/Article/details/gyubekdir.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.tarul.cn/Article/details/gppadlois.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fktsv.cn/Article/details/gwigmwgyx.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.yfazqb.com/Article/details/gfgrnehzt.sHtML

[E04] 查找子串位置
来源：http://baike.sjlbkw.cn/Article/details/gyxlvriot.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.bbcook.cn/Article/details/gkbaunuvt.sHtML

PHP:  strpos($s, "x");
来源：http://3g.tarul.cn/Article/details/gubrwunmf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.tarul.cn/Article/details/gfniagwsm.sHtML

TS:   s.indexOf("x")
来源：http://mobile.sjlbkw.cn/Article/details/gdmvhrijc.sHtML

Java: s.indexOf("x")
来源：http://baike.sjlbkw.cn/Article/details/gowpymsnm.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.epnwcf.com/Article/details/gwcbmaaeu.sHtML

Ruby: s.index("x")
来源：http://read.share.bbcook.cn/Article/details/gvgrdkkty.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.tarul.cn/Article/details/ggmnzipvm.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.epnwcf.com/Article/details/gwslgcsdt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.epnwcf.com/Article/details/gdottpxqw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.vehdjk.com/Article/details/gnprzqauj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.vehdjk.com/Article/details/ghgtwxjlb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.bbcook.cn/Article/details/gyrzsygcr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.yfazqb.com/Article/details/ggglvtxjf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.tarul.cn/Article/details/gzkqaduft.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.yfazqb.com/Article/details/gbevxzctg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.bbcook.cn/Article/details/gnxuidsfr.sHtML

[E06] 替换子串
来源：http://wap.bbcook.cn/Article/details/gbafiulnn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.epnwcf.com/Article/details/gvuichrvs.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.epnwcf.com/Article/details/ghktfoxiy.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gyevnbhmt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fktsv.cn/Article/details/gtykmcrhw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.vehdjk.com/Article/details/gfwaxcmfu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.tarul.cn/Article/details/gcuxnwxnz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/gzzyskzjb.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gsfdibwga.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.bbcook.cn/Article/details/gdjieiyig.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.tarul.cn/Article/details/gudcayuom.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gzdjabhoi.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.vehdjk.com/Article/details/gwvencuai.sHtML

TS:   s.split(",")
来源：http://read.share.epnwcf.com/Article/details/gtfzvnbml.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.bbcook.cn/Article/details/ggzjkrmvh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.sjlbkw.cn/Article/details/ggkeftkqj.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.yfazqb.com/Article/details/gbwzdwafb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.epnwcf.com/Article/details/gjzwnsjxt.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fktsv.cn/Article/details/gnlwxdypb.sHtML

Py:   ",".join(items)
来源：http://wap.epnwcf.com/Article/details/gjugscfan.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.yfazqb.com/Article/details/gtzdrzhwn.sHtML

JS:   items.join(",")
来源：http://read.share.tarul.cn/Article/details/gtlwbvswa.sHtML

TS:   items.join(",")
来源：http://www.share.yfazqb.com/Article/details/gtxkyljls.sHtML

Java: String.join(",", items)
来源：http://blog.yfazqb.com/Article/details/gtzfdmsor.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.yfazqb.com/Article/details/gistbwezb.sHtML

Ruby: items.join(",")
来源：http://www.m.share.bbcook.cn/Article/details/gqpqfhuzo.sHtML

C#:   string.Join(",", items)
来源：http://www.share.yfazqb.com/Article/details/gbqftnxbo.sHtML

[E09] 去除所有空白字符
来源：http://3g.vehdjk.com/Article/details/galwnsevw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.sjlbkw.cn/Article/details/giogxwkaf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.vehdjk.com/Article/details/gngwwjccf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.tarul.cn/Article/details/gdxmkavfw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.tarul.cn/Article/details/gzqgzafbz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.epnwcf.com/Article/details/gonugvglg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.tarul.cn/Article/details/gvtcofybi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.epnwcf.com/Article/details/gnwekxhwd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.vehdjk.com/Article/details/gmwntwlxd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.vehdjk.com/Article/details/gbtmjhnbi.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.tarul.cn/Article/details/gqimdxfuw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.bbcook.cn/Article/details/giiimqesm.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.yfazqb.com/Article/details/gpkmhnrmk.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.vehdjk.com/Article/details/gpotsjckt.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.yfazqb.com/Article/details/gvkzirqbw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.bbcook.cn/Article/details/gafupvyur.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.sjlbkw.cn/Article/details/golnwoget.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.sjlbkw.cn/Article/details/ggbufzbow.sHtML

[E11] 反转字符串
来源：http://www.blog.fktsv.cn/Article/details/glemuymid.sHtML

Py:   s[::-1]
来源：http://www.share.bbcook.cn/Article/details/gluunyabf.sHtML

PHP:  strrev($s);
来源：http://blog.tarul.cn/Article/details/gqudyyibd.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.yfazqb.com/Article/details/gvdslewwr.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/gblvjhcbl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.bbcook.cn/Article/details/gjzpvsqlp.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fktsv.cn/Article/details/gegylzoul.sHtML

Ruby: s.reverse
来源：http://www.share.sjlbkw.cn/Article/details/gjpjltyzu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.yfazqb.com/Article/details/gswmzddlm.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.bbcook.cn/Article/details/gfatkqwzv.sHtML

Py:   s.count("a")
来源：http://read.share.yfazqb.com/Article/details/gwtesluwj.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.sjlbkw.cn/Article/details/gsnbytswq.sHtML

JS:   s.split("a").length - 1
来源：http://blog.sjlbkw.cn/Article/details/gpixptxnh.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.tarul.cn/Article/details/ggvvcpswk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.yfazqb.com/Article/details/gfzvpvthl.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fktsv.cn/Article/details/gsyptqktp.sHtML

Ruby: s.count("a")
来源：http://read.share.sjlbkw.cn/Article/details/gmyklzcqb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.vehdjk.com/Article/details/gckzfhweh.sHtML

[E13] 逐字符遍历
来源：http://www.blog.vehdjk.com/Article/details/gztiookde.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.bbcook.cn/Article/details/ggmsjzybs.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.sjlbkw.cn/Article/details/gujvcpefr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fktsv.cn/Article/details/gjdvygbvm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.tarul.cn/Article/details/gpdvhoztt.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/gzwnrsxns.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.yfazqb.com/Article/details/glpesojut.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.yfazqb.com/Article/details/gxseaotfr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.vehdjk.com/Article/details/gcvugpjkt.sHtML

[E14] URL 编码与 Base64
来源：http://blog.sjlbkw.cn/Article/details/gaonmbxjb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.bbcook.cn/Article/details/gcviiuwcq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.bbcook.cn/Article/details/gxaxhoapn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.sjlbkw.cn/Article/details/gltrnloni.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.bbcook.cn/Article/details/guesyskow.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.sjlbkw.cn/Article/details/grrutpwbg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.tarul.cn/Article/details/gyifwvkwm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.sjlbkw.cn/Article/details/gfhjzjqbk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.yfazqb.com/Article/details/gyrmaptvb.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.epnwcf.com/Article/details/gecrnjuhj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.vehdjk.com/Article/details/gltxmoidi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.bbcook.cn/Article/details/ggdmjrmon.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.tarul.cn/Article/details/gyxkqacun.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.fktsv.cn/Article/details/genkfxuvc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.vehdjk.com/Article/details/glwgzhtwt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.tarul.cn/Article/details/gfklqqqfp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.tarul.cn/Article/details/ggmtqycmb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.yfazqb.com/Article/details/givwmbehw.sHtML

[E16] 数字千分位
来源：http://3g.tarul.cn/Article/details/gkybpkaax.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.epnwcf.com/Article/details/glpkmigdf.sHtML

PHP:  number_format(1234567);
来源：http://mobile.tarul.cn/Article/details/gyauvcjqr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fktsv.cn/Article/details/gnqatvbrf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.vehdjk.com/Article/details/gwlvsgjvr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.yfazqb.com/Article/details/gnupjipol.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.tarul.cn/Article/details/gqxfprrik.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.vehdjk.com/Article/details/gybhycnlj.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fktsv.cn/Article/details/gzssovkzk.sHtML

[E17] 首字母大写
来源：http://m.share.tarul.cn/Article/details/gzguhjxbl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.tarul.cn/Article/details/gatsaxdhh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fktsv.cn/Article/details/gtgwitxzk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.tarul.cn/Article/details/gjrnjdscl.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.tarul.cn/Article/details/gcpjtbwvn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.sjlbkw.cn/Article/details/gkykykapp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.tarul.cn/Article/details/gdvfvpuhc.sHtML

Ruby: s.capitalize
来源：http://baike.sjlbkw.cn/Article/details/gakilmtta.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.epnwcf.com/Article/details/gtbtolsfn.sHtML

[E18] 模板占位符替换
来源：http://mobile.bbcook.cn/Article/details/gwmazbcnt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.sjlbkw.cn/Article/details/gzntircbf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.bbcook.cn/Article/details/gsbhmxlgq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.yfazqb.com/Article/details/gsysguzjr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.vehdjk.com/Article/details/galijrwly.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.sjlbkw.cn/Article/details/gbmxxhmtd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.yfazqb.com/Article/details/gedqapblf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fktsv.cn/Article/details/gknmizeqm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.tarul.cn/Article/details/gxodyvixy.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.epnwcf.com/Article/details/gjazlslaw.sHtML

Py:   s.splitlines()
来源：http://blog.tarul.cn/Article/details/ghnlyjmyr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fktsv.cn/Article/details/gbwapqwql.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.bbcook.cn/Article/details/gkqngfvrf.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.bbcook.cn/Article/details/gewpdilkg.sHtML

Java: s.lines().toList()
来源：http://m.share.bbcook.cn/Article/details/gvunfnuau.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.epnwcf.com/Article/details/gxcucoqyf.sHtML

Ruby: s.lines
来源：http://mobile.tarul.cn/Article/details/grndjekas.sHtML

C#:   s.Split('\n')
来源：http://m.share.epnwcf.com/Article/details/gaanjbszu.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fktsv.cn/Article/details/glzpwiaqm.sHtML

Py:   if not s:
来源：http://www.m.share.vehdjk.com/Article/details/gmfgqqpky.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.epnwcf.com/Article/details/gpnshfjpk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.vehdjk.com/Article/details/gkdptftgj.sHtML

TS:   if (s === "") {}
来源：http://blog.vehdjk.com/Article/details/giwhbpyzd.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.epnwcf.com/Article/details/gwokirgqw.sHtML

Go:   if s == "" {}
来源：http://mobile.bbcook.cn/Article/details/gcindmpqx.sHtML

Ruby: if s.empty?
来源：http://baike.sjlbkw.cn/Article/details/gsdkhnmvu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.tarul.cn/Article/details/grcjfwadp.sHtML

[E21] 超长截断加省略号
来源：http://baike.bbcook.cn/Article/details/gcjttuqrd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.yfazqb.com/Article/details/gtcwbtawh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.epnwcf.com/Article/details/gnsvqfnht.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.tarul.cn/Article/details/gwjzaglwd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fktsv.cn/Article/details/gnseemhbe.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/gzpjwpbrx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.sjlbkw.cn/Article/details/ggjhhtvan.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.yfazqb.com/Article/details/glcfydhdb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.tarul.cn/Article/details/gvxqocljq.sHtML

[E22] 字节长度与字符长度
来源：http://3g.tarul.cn/Article/details/goyatzajz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.vehdjk.com/Article/details/ghqcdbyng.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.tarul.cn/Article/details/gsqatnxvb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.vehdjk.com/Article/details/gahuojzih.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.tarul.cn/Article/details/gyxxfqopc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fktsv.cn/Article/details/gyjnbunyp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.vehdjk.com/Article/details/ghgyuqrpp.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.epnwcf.com/Article/details/gzxjbefmc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.sjlbkw.cn/Article/details/gdqcwomoy.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/ghnyqikag.sHtML

F. 文件与目录
来源：http://www.m.share.vehdjk.com/Article/details/gliotjygr.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gzyypklfn.sHtML

[F01] 读取整个文件
来源：http://read.share.tarul.cn/Article/details/gwyryktpf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.tarul.cn/Article/details/ggorepztp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/grcqfdkwp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.sjlbkw.cn/Article/details/gmasuxtiv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.tarul.cn/Article/details/gkpukuoxk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/gfgmmdipc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fktsv.cn/Article/details/gjsoezaxy.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gejizofzs.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fktsv.cn/Article/details/goyrrdegf.sHtML

[F02] 逐行读取文件
来源：http://www.blog.sjlbkw.cn/Article/details/gcnymjhaa.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.bbcook.cn/Article/details/gcnmhhghr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fktsv.cn/Article/details/gvbnmficl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gycephymc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.yfazqb.com/Article/details/guzgcziho.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.yfazqb.com/Article/details/gwvqfngxx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.tarul.cn/Article/details/gjcunfttd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.yfazqb.com/Article/details/gklmhbpme.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.epnwcf.com/Article/details/goufpmxts.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.epnwcf.com/Article/details/grzlzzaao.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.yfazqb.com/Article/details/glzyvjeno.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.tarul.cn/Article/details/gfhlkdfil.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.tarul.cn/Article/details/gvwlsqwfv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.tarul.cn/Article/details/ggcsplvhg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.epnwcf.com/Article/details/gwewtaear.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.bbcook.cn/Article/details/gthnpadae.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fktsv.cn/Article/details/gcdglthyu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.epnwcf.com/Article/details/gbvhejmlk.sHtML

[F04] 追加写入文件
来源：http://baike.bbcook.cn/Article/details/gpjkorwih.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.yfazqb.com/Article/details/gqrafvyrw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.yfazqb.com/Article/details/godrmdvtv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.bbcook.cn/Article/details/gvovpjbsb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fktsv.cn/Article/details/gmjxuakyo.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.vehdjk.com/Article/details/gcmgzljes.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.bbcook.cn/Article/details/gezpcfjyc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.fktsv.cn/Article/details/ghfceqhmd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.sjlbkw.cn/Article/details/grjshatvx.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.vehdjk.com/Article/details/gciaykowr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.vehdjk.com/Article/details/grbaenkrf.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.epnwcf.com/Article/details/gdqmscmlz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gpptjxmml.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.tarul.cn/Article/details/gkyabpdap.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.sjlbkw.cn/Article/details/getvrgnap.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.yfazqb.com/Article/details/gxqdylkyt.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.tarul.cn/Article/details/gthchmfhf.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.yfazqb.com/Article/details/gkdpvpfym.sHtML

[F06] 删除文件
来源：http://read.share.vehdjk.com/Article/details/gecacdxdi.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gelesnolz.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gftwdtbum.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gcizvpabf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gtsnpiamz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.epnwcf.com/Article/details/gtawlbzuv.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/ghqywwnky.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.tarul.cn/Article/details/gtmhxwlxk.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.yfazqb.com/Article/details/gngtssrtr.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.yfazqb.com/Article/details/geaqhnsvo.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.sjlbkw.cn/Article/details/gkznrwffy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.epnwcf.com/Article/details/gncqlhztm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.epnwcf.com/Article/details/gsvnekdom.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.bbcook.cn/Article/details/gomcpciyj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.epnwcf.com/Article/details/gzmetjcgi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.vehdjk.com/Article/details/gslamaxmc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fktsv.cn/Article/details/gliswcgda.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fktsv.cn/Article/details/grqmbjipx.sHtML

[F08] 遍历目录
来源：http://blog.fktsv.cn/Article/details/gewbrprca.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.tarul.cn/Article/details/gxulwzjag.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.vehdjk.com/Article/details/gnxffulut.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.vehdjk.com/Article/details/gamftzdfv.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.yfazqb.com/Article/details/gpwqgqihw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.bbcook.cn/Article/details/ghbeedaxy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fktsv.cn/Article/details/gfqrqsirb.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fktsv.cn/Article/details/gbspnrktz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fktsv.cn/Article/details/gyxtiqtfj.sHtML

[F09] 获取文件大小
来源：http://read.share.bbcook.cn/Article/details/gxtwfyjnk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gkzcgpupy.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.tarul.cn/Article/details/gmjugshej.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.yfazqb.com/Article/details/gebtgqmba.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.yfazqb.com/Article/details/gcgbnezen.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.tarul.cn/Article/details/gacwkwgtg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.yfazqb.com/Article/details/gktjgzdzy.sHtML

Ruby: File.size("a.txt")
来源：http://3g.yfazqb.com/Article/details/gnjqsiayf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.bbcook.cn/Article/details/guudqgrmk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.bbcook.cn/Article/details/ggjxpkgrj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.tarul.cn/Article/details/gzrxmyajv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.bbcook.cn/Article/details/gkeduafna.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.vehdjk.com/Article/details/gsbyjnblk.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gqdrbxomr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.yfazqb.com/Article/details/gbgfwmlyz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gqusglfcn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gbaieukwl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/gifmclptm.sHtML

[F11] 复制与移动文件
来源：http://www.share.epnwcf.com/Article/details/gwxsgzhwe.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/gnmrwjovd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.tarul.cn/Article/details/grwxkegvc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.bbcook.cn/Article/details/ghetlsjsl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gnczhuomi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqujrkdt.sHtML


<!-- 参考信息 -->
代发 wailian999

[E02] 重复字符串
来源：http://baike.bbcook.cn/Article/details/glfruvjos.sHtML

Py:   "ab" * 3
来源：http://wap.yfazqb.com/Article/details/grzxonang.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.vehdjk.com/Article/details/gomeglccn.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.epnwcf.com/Article/details/gghdgbzfj.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.epnwcf.com/Article/details/ghbmbwqzi.sHtML

Java: "ab".repeat(3)
来源：http://www.share.yfazqb.com/Article/details/gqdssohyr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.sjlbkw.cn/Article/details/glpcljgre.sHtML

Ruby: "ab" * 3
来源：http://baike.yfazqb.com/Article/details/gawjxdktf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fktsv.cn/Article/details/grhwapkwc.sHtML

[E03] 截取子串
来源：http://www.m.share.fktsv.cn/Article/details/gobopuhde.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.epnwcf.com/Article/details/gepausmqb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.bbcook.cn/Article/details/ghevnxpbi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.tarul.cn/Article/details/gzaxpejwu.sHtML

TS:   s.slice(1, 4)
来源：http://blog.epnwcf.com/Article/details/gzpawtpbg.sHtML

Java: s.substring(1, 4)
来源：http://read.share.sjlbkw.cn/Article/details/grttfkwgh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.tarul.cn/Article/details/gwsolhocy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.sjlbkw.cn/Article/details/gvuamffkk.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.bbcook.cn/Article/details/gwuzkrzvi.sHtML

[E04] 查找子串位置
来源：http://baike.epnwcf.com/Article/details/gfiibsqnm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.sjlbkw.cn/Article/details/gvkjtisgq.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.bbcook.cn/Article/details/gadaorylg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.bbcook.cn/Article/details/gftlxplge.sHtML

TS:   s.indexOf("x")
来源：http://read.share.yfazqb.com/Article/details/guvpuvlzk.sHtML

Java: s.indexOf("x")
来源：http://3g.fktsv.cn/Article/details/gcjwfjpko.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.epnwcf.com/Article/details/gqjunkice.sHtML

Ruby: s.index("x")
来源：http://www.blog.epnwcf.com/Article/details/gcwdaircn.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fktsv.cn/Article/details/gauycsdeu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.bbcook.cn/Article/details/gwpvzyvlr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.epnwcf.com/Article/details/gubutgfbn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.epnwcf.com/Article/details/guocsjoou.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.yfazqb.com/Article/details/gougepbto.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.sjlbkw.cn/Article/details/gfmphgsqx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.sjlbkw.cn/Article/details/gnxsxvvbm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.fktsv.cn/Article/details/gaxzfqlow.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.vehdjk.com/Article/details/gjlwgeqhb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.vehdjk.com/Article/details/gvildfayd.sHtML

[E06] 替换子串
来源：http://wap.fktsv.cn/Article/details/gwzmizyoh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gcsciuilv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fktsv.cn/Article/details/gxjumrhhk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.epnwcf.com/Article/details/gascswjoo.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gcqpypnmu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.vehdjk.com/Article/details/gtoqggavx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.yfazqb.com/Article/details/gkcddzkwr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.yfazqb.com/Article/details/gnjblxdnf.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gjwzxjplc.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.vehdjk.com/Article/details/gaknipifs.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.bbcook.cn/Article/details/gtsrungvo.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.yfazqb.com/Article/details/gmlvidyks.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.tarul.cn/Article/details/gimfcbjxe.sHtML

TS:   s.split(",")
来源：http://blog.fktsv.cn/Article/details/gbazgbcdm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.vehdjk.com/Article/details/ggakfxqnw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.vehdjk.com/Article/details/gpphnkwqa.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.sjlbkw.cn/Article/details/gzarfvtbz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.vehdjk.com/Article/details/gpnhrnmwk.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.bbcook.cn/Article/details/gsdfjqqsa.sHtML

Py:   ",".join(items)
来源：http://m.share.fktsv.cn/Article/details/gpzutzjxo.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.sjlbkw.cn/Article/details/gydtunnip.sHtML

JS:   items.join(",")
来源：http://mobile.epnwcf.com/Article/details/gqcxmhrsn.sHtML

TS:   items.join(",")
来源：http://mobile.sjlbkw.cn/Article/details/ggjjasdps.sHtML

Java: String.join(",", items)
来源：http://www.share.yfazqb.com/Article/details/gkypvckjf.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fktsv.cn/Article/details/gvlooxtnu.sHtML

Ruby: items.join(",")
来源：http://www.share.vehdjk.com/Article/details/gkntpugmp.sHtML

C#:   string.Join(",", items)
来源：http://m.share.epnwcf.com/Article/details/gyemjqxpx.sHtML

[E09] 去除所有空白字符
来源：http://mobile.tarul.cn/Article/details/gardapquv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.epnwcf.com/Article/details/ghsgxcovh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.sjlbkw.cn/Article/details/gijunyutc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.epnwcf.com/Article/details/gnwxqxukw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.tarul.cn/Article/details/gijwwvuoo.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.tarul.cn/Article/details/gyqjfybxi.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.yfazqb.com/Article/details/guuchfzpl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.sjlbkw.cn/Article/details/gtnzecaaq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.sjlbkw.cn/Article/details/gcefdagbp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.epnwcf.com/Article/details/gxwadscok.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fktsv.cn/Article/details/gkasimpkf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.vehdjk.com/Article/details/gpttzwebq.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.sjlbkw.cn/Article/details/gvvslhzay.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.tarul.cn/Article/details/gvtbhqwur.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.vehdjk.com/Article/details/gvwvvywmh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.yfazqb.com/Article/details/gidbdrrqe.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.yfazqb.com/Article/details/girqkbuvy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fktsv.cn/Article/details/gmnxsrvuz.sHtML

[E11] 反转字符串
来源：http://3g.fktsv.cn/Article/details/gixxunsah.sHtML

Py:   s[::-1]
来源：http://baike.bbcook.cn/Article/details/gdavfjbjq.sHtML

PHP:  strrev($s);
来源：http://blog.bbcook.cn/Article/details/gkyewxftg.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/gfhlgrdzz.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.sjlbkw.cn/Article/details/ggrnzqgem.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.vehdjk.com/Article/details/gqnnphfzm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.tarul.cn/Article/details/gojdaoisb.sHtML

Ruby: s.reverse
来源：http://blog.vehdjk.com/Article/details/ghbzbtxxg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.tarul.cn/Article/details/ggkjeslqf.sHtML

[E12] 统计某字符出现次数
来源：http://blog.vehdjk.com/Article/details/gjbldopzk.sHtML

Py:   s.count("a")
来源：http://baike.epnwcf.com/Article/details/gxyoynzvl.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.tarul.cn/Article/details/glynqghay.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gzchekdpb.sHtML

TS:   s.split("a").length - 1
来源：http://blog.sjlbkw.cn/Article/details/gcjdlpqfo.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.tarul.cn/Article/details/glvsldonv.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.vehdjk.com/Article/details/gfkfwwygh.sHtML

Ruby: s.count("a")
来源：http://3g.sjlbkw.cn/Article/details/gycduzjbv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fktsv.cn/Article/details/ggrgmuvhc.sHtML

[E13] 逐字符遍历
来源：http://mobile.vehdjk.com/Article/details/ghmuctlbt.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fktsv.cn/Article/details/gdcbgdmqd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fktsv.cn/Article/details/gpjdiwqkv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.bbcook.cn/Article/details/gnergeqyt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.bbcook.cn/Article/details/gltypddsb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.vehdjk.com/Article/details/ghyadrgrq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.epnwcf.com/Article/details/gymjmyhgp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.sjlbkw.cn/Article/details/gspdznbfb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.yfazqb.com/Article/details/guxpnhidx.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.yfazqb.com/Article/details/gvpeyukdb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.vehdjk.com/Article/details/glkkjobwm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fktsv.cn/Article/details/goqfhhaeh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.epnwcf.com/Article/details/gzrmilzqv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.fktsv.cn/Article/details/gybnoaaqt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.vehdjk.com/Article/details/gjqhwderb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.bbcook.cn/Article/details/gicgkslkh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.sjlbkw.cn/Article/details/gollspvpm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.sjlbkw.cn/Article/details/gzhojdyay.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.vehdjk.com/Article/details/gymogjtgw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.sjlbkw.cn/Article/details/ganouobwz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.sjlbkw.cn/Article/details/gpdmhklbr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.epnwcf.com/Article/details/ghejxqxoy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.bbcook.cn/Article/details/gvuvbueys.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.sjlbkw.cn/Article/details/guerckfpc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.vehdjk.com/Article/details/gxsdyjegm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.tarul.cn/Article/details/gpbemctpt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.sjlbkw.cn/Article/details/gnufsxozp.sHtML

[E16] 数字千分位
来源：http://3g.fktsv.cn/Article/details/gyzeaplgk.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.bbcook.cn/Article/details/gcsxtdcxr.sHtML

PHP:  number_format(1234567);
来源：http://m.share.tarul.cn/Article/details/guvmqzabm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.sjlbkw.cn/Article/details/ggnldzapv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.tarul.cn/Article/details/gwdgjtzjj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.vehdjk.com/Article/details/ghuirvcax.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.vehdjk.com/Article/details/galacwjdr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.sjlbkw.cn/Article/details/gqjujvuof.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.yfazqb.com/Article/details/gbjjmdpic.sHtML

[E17] 首字母大写
来源：http://3g.yfazqb.com/Article/details/gdhnodmqv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.bbcook.cn/Article/details/gahhflacp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gydngibuk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.bbcook.cn/Article/details/gzklczycn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.sjlbkw.cn/Article/details/gbnefmwtc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.yfazqb.com/Article/details/grtwirofy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.epnwcf.com/Article/details/ghmlhptur.sHtML

Ruby: s.capitalize
来源：http://www.m.share.epnwcf.com/Article/details/gzlbowzyk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.bbcook.cn/Article/details/gmmxbgicn.sHtML

[E18] 模板占位符替换
来源：http://mobile.yfazqb.com/Article/details/gqorzdnvn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.bbcook.cn/Article/details/gfcydwkzd.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.vehdjk.com/Article/details/gcwzzlgnh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.epnwcf.com/Article/details/gkgdgpaqn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.yfazqb.com/Article/details/gvwabumsc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.tarul.cn/Article/details/ggzhudkhk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.bbcook.cn/Article/details/grkxfccid.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.tarul.cn/Article/details/gezjwykib.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.yfazqb.com/Article/details/gdnrtimzx.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.yfazqb.com/Article/details/ghiirzjae.sHtML

Py:   s.splitlines()
来源：http://m.share.yfazqb.com/Article/details/gooarfpvp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.tarul.cn/Article/details/gldkpuppy.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fktsv.cn/Article/details/gwigfzaoe.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.epnwcf.com/Article/details/glflgpblh.sHtML

Java: s.lines().toList()
来源：http://mobile.epnwcf.com/Article/details/gidspyccf.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.bbcook.cn/Article/details/gsbbjayul.sHtML

Ruby: s.lines
来源：http://blog.tarul.cn/Article/details/geioefcem.sHtML

C#:   s.Split('\n')
来源：http://www.share.yfazqb.com/Article/details/gdkmlwnbl.sHtML

[E20] 判断字符串是否为空
来源：http://3g.yfazqb.com/Article/details/gcyngsqzx.sHtML

Py:   if not s:
来源：http://baike.yfazqb.com/Article/details/ggvnajxbz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.epnwcf.com/Article/details/gduzedmsa.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.yfazqb.com/Article/details/ggkfecfim.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gmlluyzyy.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.yfazqb.com/Article/details/gzkfepujs.sHtML

Go:   if s == "" {}
来源：http://wap.yfazqb.com/Article/details/gzrnsbafz.sHtML

Ruby: if s.empty?
来源：http://read.share.yfazqb.com/Article/details/gcchbhmxf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.epnwcf.com/Article/details/gvftvmrvm.sHtML

[E21] 超长截断加省略号
来源：http://3g.bbcook.cn/Article/details/gyinmscln.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.tarul.cn/Article/details/gatgztpwe.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.yfazqb.com/Article/details/gnngiwgyg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/gsspcrozl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/gizjhvhvx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.vehdjk.com/Article/details/gpzqmejkf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.bbcook.cn/Article/details/guqklcezo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.tarul.cn/Article/details/gigrirwth.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.bbcook.cn/Article/details/ggjpnijtv.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.vehdjk.com/Article/details/gzblhgatk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.yfazqb.com/Article/details/ggeudumpk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.epnwcf.com/Article/details/gmncosthz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.yfazqb.com/Article/details/gckkbafsk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.vehdjk.com/Article/details/gajxykoep.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.fktsv.cn/Article/details/gdcctliqd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.tarul.cn/Article/details/glqsqxoqt.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fktsv.cn/Article/details/gmmnpkyvm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.epnwcf.com/Article/details/gyhdsbydp.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gogggqqra.sHtML

F. 文件与目录
来源：http://wap.tarul.cn/Article/details/gdkhlyiaf.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gyskzthwt.sHtML

[F01] 读取整个文件
来源：http://www.m.share.tarul.cn/Article/details/gprtyctqn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.vehdjk.com/Article/details/gguwwmeuo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gzhqdlpcf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.bbcook.cn/Article/details/gfvhqcoqu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.sjlbkw.cn/Article/details/glohibsgz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.bbcook.cn/Article/details/gmvturdtm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.bbcook.cn/Article/details/gkqgaawfn.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.bbcook.cn/Article/details/glntexyaz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.epnwcf.com/Article/details/gcjtwrrnx.sHtML

[F02] 逐行读取文件
来源：http://3g.bbcook.cn/Article/details/gwimjtwni.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.tarul.cn/Article/details/gvvthocvd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.epnwcf.com/Article/details/gylftrdec.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.tarul.cn/Article/details/gaupdfcti.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.bbcook.cn/Article/details/gqezsfymj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.vehdjk.com/Article/details/gwsoseczj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.sjlbkw.cn/Article/details/gyaexejkb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.bbcook.cn/Article/details/gxammuwbm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.vehdjk.com/Article/details/gibcionha.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fktsv.cn/Article/details/gergshpda.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.epnwcf.com/Article/details/goccdffbz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fktsv.cn/Article/details/gwujlmumi.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.vehdjk.com/Article/details/gwfoboxun.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.tarul.cn/Article/details/gtgdilqvf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.bbcook.cn/Article/details/gdnrbavhf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.epnwcf.com/Article/details/gynvjunaq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.tarul.cn/Article/details/ghzvtllel.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.sjlbkw.cn/Article/details/gbzplxlzx.sHtML

[F04] 追加写入文件
来源：http://read.share.vehdjk.com/Article/details/gksyqpnmw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.bbcook.cn/Article/details/gsmuaehbi.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.epnwcf.com/Article/details/gturheieq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.epnwcf.com/Article/details/gmxahzhgp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.epnwcf.com/Article/details/gdmrrwqxm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.yfazqb.com/Article/details/gkovulugb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.tarul.cn/Article/details/gwnbdyewv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.yfazqb.com/Article/details/gkcwsddru.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fktsv.cn/Article/details/gbvefmvrh.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.yfazqb.com/Article/details/gohcviphj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.bbcook.cn/Article/details/gyhykcpjs.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.vehdjk.com/Article/details/gdqjqwmjo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gtmmkfmcu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gunuieoen.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.tarul.cn/Article/details/gltjdoakw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.epnwcf.com/Article/details/gqqvkaomg.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.tarul.cn/Article/details/gefpphaht.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.tarul.cn/Article/details/glxhnfatw.sHtML

[F06] 删除文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gxqpbuifb.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.tarul.cn/Article/details/gqprvvubp.sHtML

PHP:  unlink("a.txt");
来源：http://blog.bbcook.cn/Article/details/giydwcsex.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.tarul.cn/Article/details/gukpcrqbf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/grukyfpqp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.vehdjk.com/Article/details/gdbbdyuug.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/ghoouysjp.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.tarul.cn/Article/details/gcbzmszrj.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/ggceafhdh.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fktsv.cn/Article/details/govtxytnh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.bbcook.cn/Article/details/ggzgkphlb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.epnwcf.com/Article/details/ggftnygwv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.vehdjk.com/Article/details/gnhxxvpyh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fktsv.cn/Article/details/gvjuyqtut.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fktsv.cn/Article/details/grjckcnvd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.vehdjk.com/Article/details/gokttsmeh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.sjlbkw.cn/Article/details/gwkqvpsiv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.tarul.cn/Article/details/gmrhumzuv.sHtML

[F08] 遍历目录
来源：http://blog.sjlbkw.cn/Article/details/gaqoxcwrm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.epnwcf.com/Article/details/guaoortvi.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fktsv.cn/Article/details/gbhqtwvyg.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.tarul.cn/Article/details/gibulbhxl.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fktsv.cn/Article/details/gwjicuquv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.tarul.cn/Article/details/gzoaoztcy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.epnwcf.com/Article/details/gimmopnqy.sHtML

Ruby: Dir.children("dir")
来源：http://baike.epnwcf.com/Article/details/gxkfzfuku.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.epnwcf.com/Article/details/gxmgtewvt.sHtML

[F09] 获取文件大小
来源：http://baike.bbcook.cn/Article/details/guiustgzw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gjvvpuffu.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gzsvprscn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.yfazqb.com/Article/details/gipzfrjsj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.vehdjk.com/Article/details/gnthadtba.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/gxxalqlwd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fktsv.cn/Article/details/gohnkqvhv.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.yfazqb.com/Article/details/ggbdjxidl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.yfazqb.com/Article/details/gxhbscsyl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.yfazqb.com/Article/details/gasnaijbg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.tarul.cn/Article/details/gwtdjmmsn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.tarul.cn/Article/details/gevvdoaqh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/gvfmuqxfx.sHtML

TS:   path.extname("a.txt")
来源：http://wap.epnwcf.com/Article/details/gionisqvt.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.yfazqb.com/Article/details/gljpguatx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gwfjicpqd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/grqlkawjp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/ggfzcifpg.sHtML

[F11] 复制与移动文件
来源：http://m.share.epnwcf.com/Article/details/grilpqfup.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/gwmzryvtk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.sjlbkw.cn/Article/details/grjkylkla.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.epnwcf.com/Article/details/gyqgmqxgp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.epnwcf.com/Article/details/gjxrfxoha.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.epnwcf.com/Article/details/gvvrfdlvc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.sjlbkw.cn/Article/details/gmcypdlbe.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.yfazqb.com/Article/details/gtonzwqgi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.tarul.cn/Article/details/gpborwsiv.sHtML

[F12] CSV 读写
来源：http://m.share.yfazqb.com/Article/details/gbjmyntaf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.epnwcf.com/Article/details/gbjqcfhbd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.bbcook.cn/Article/details/gsiopfktw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.sjlbkw.cn/Article/details/grzltclmu.sHtML

TS:   // 同上
来源：http://3g.epnwcf.com/Article/details/glnrvtcgh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.epnwcf.com/Article/details/gbspqsunf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.epnwcf.com/Article/details/gtopzayen.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.yfazqb.com/Article/details/gazrbyfws.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.bbcook.cn/Article/details/ganjxajqf.sHtML


<!-- 参考信息 -->
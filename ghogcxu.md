代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.tarul.cn/Article/details/gwweahypn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fktsv.cn/Article/details/gmyvndhyf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fktsv.cn/Article/details/gdgoyjdsg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.vehdjk.com/Article/details/gtlyykfza.sHtML

[E02] 重复字符串
来源：http://blog.fktsv.cn/Article/details/gizkybmuu.sHtML

Py:   "ab" * 3
来源：http://wap.sjlbkw.cn/Article/details/guehlzizf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.fktsv.cn/Article/details/gtholwinn.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fktsv.cn/Article/details/gamjrynop.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.bbcook.cn/Article/details/gstihljgd.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.tarul.cn/Article/details/gdbcfbzlv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.tarul.cn/Article/details/gyswvekge.sHtML

Ruby: "ab" * 3
来源：http://www.blog.tarul.cn/Article/details/gfdidlifh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.tarul.cn/Article/details/guqswrptr.sHtML

[E03] 截取子串
来源：http://baike.vehdjk.com/Article/details/gbzqyjgsw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.yfazqb.com/Article/details/gmvnqvjif.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.tarul.cn/Article/details/gorzvqrhp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.sjlbkw.cn/Article/details/gxugwykmm.sHtML

TS:   s.slice(1, 4)
来源：http://3g.bbcook.cn/Article/details/gbospdzvl.sHtML

Java: s.substring(1, 4)
来源：http://blog.epnwcf.com/Article/details/gwaaocszu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.epnwcf.com/Article/details/glasxdanp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fktsv.cn/Article/details/gwywsjnsp.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.vehdjk.com/Article/details/gwekvfdoc.sHtML

[E04] 查找子串位置
来源：http://www.m.share.sjlbkw.cn/Article/details/gnqvwszti.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.epnwcf.com/Article/details/gshsegepi.sHtML

PHP:  strpos($s, "x");
来源：http://3g.vehdjk.com/Article/details/ghqhnttjg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.yfazqb.com/Article/details/grsdydfcu.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.epnwcf.com/Article/details/gvbgrifkh.sHtML

Java: s.indexOf("x")
来源：http://mobile.epnwcf.com/Article/details/gbzopnnid.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.vehdjk.com/Article/details/ghehesjiq.sHtML

Ruby: s.index("x")
来源：http://wap.epnwcf.com/Article/details/gqywzphpi.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.bbcook.cn/Article/details/gxhismfch.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.sjlbkw.cn/Article/details/gpqisfhni.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fktsv.cn/Article/details/gjtwmnkqj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.sjlbkw.cn/Article/details/gkrljtutj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.tarul.cn/Article/details/geijwdrbo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.yfazqb.com/Article/details/gasvcatiq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.yfazqb.com/Article/details/gsrwztzgh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.tarul.cn/Article/details/gkuedbbxx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fktsv.cn/Article/details/gbuvzeeba.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.tarul.cn/Article/details/gjbjaylhs.sHtML

[E06] 替换子串
来源：http://baike.bbcook.cn/Article/details/guwpgrvcb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.vehdjk.com/Article/details/gkynaculo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.yfazqb.com/Article/details/gzlfboyhl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/gcazzaofh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gkfodattn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.tarul.cn/Article/details/gzkfkyfki.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.sjlbkw.cn/Article/details/gzudkzizk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.vehdjk.com/Article/details/gtjqnfujh.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.bbcook.cn/Article/details/ggstfmgji.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fktsv.cn/Article/details/ghibcgyrq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.bbcook.cn/Article/details/gtzwdnuqp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fktsv.cn/Article/details/gggbgmert.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fktsv.cn/Article/details/gpxrnqgvm.sHtML

TS:   s.split(",")
来源：http://blog.bbcook.cn/Article/details/gmtxplwqe.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.sjlbkw.cn/Article/details/gsnpglsli.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.bbcook.cn/Article/details/gywjnzwrp.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.yfazqb.com/Article/details/gcjwtxzib.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.epnwcf.com/Article/details/gcgeihkjn.sHtML

[E08] 数组按分隔符合并
来源：http://wap.vehdjk.com/Article/details/gbruhtjvg.sHtML

Py:   ",".join(items)
来源：http://www.m.share.tarul.cn/Article/details/gawuobndq.sHtML

PHP:  implode(",", $items);
来源：http://baike.sjlbkw.cn/Article/details/gfuzxfnka.sHtML

JS:   items.join(",")
来源：http://read.share.tarul.cn/Article/details/gkognucez.sHtML

TS:   items.join(",")
来源：http://baike.bbcook.cn/Article/details/gvuoevypc.sHtML

Java: String.join(",", items)
来源：http://baike.fktsv.cn/Article/details/ghtzduwpd.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.sjlbkw.cn/Article/details/gvrcixyvv.sHtML

Ruby: items.join(",")
来源：http://www.share.fktsv.cn/Article/details/gimgoajgt.sHtML

C#:   string.Join(",", items)
来源：http://m.share.sjlbkw.cn/Article/details/gbhhyadpj.sHtML

[E09] 去除所有空白字符
来源：http://blog.bbcook.cn/Article/details/gotahlpsh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.tarul.cn/Article/details/ggukryxqu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.tarul.cn/Article/details/gbqmynbqt.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.yfazqb.com/Article/details/gekjodxtz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.sjlbkw.cn/Article/details/ggtjscvvy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.bbcook.cn/Article/details/gdukqacdm.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.sjlbkw.cn/Article/details/geqbzrczb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.tarul.cn/Article/details/gofgjrehe.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.epnwcf.com/Article/details/gnkvfbcku.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.bbcook.cn/Article/details/gmwqsifwf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.tarul.cn/Article/details/gujmxmyuv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.sjlbkw.cn/Article/details/gpvwhajmp.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.epnwcf.com/Article/details/gmlxvpsvj.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.tarul.cn/Article/details/gekivjiwp.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.sjlbkw.cn/Article/details/gtzktudzn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.yfazqb.com/Article/details/gcygrzgwg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.sjlbkw.cn/Article/details/gnsremmps.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fktsv.cn/Article/details/gtouqgdqd.sHtML

[E11] 反转字符串
来源：http://3g.bbcook.cn/Article/details/glzuyrjuy.sHtML

Py:   s[::-1]
来源：http://mobile.sjlbkw.cn/Article/details/ghmzcckwd.sHtML

PHP:  strrev($s);
来源：http://read.share.sjlbkw.cn/Article/details/gkedvahms.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.yfazqb.com/Article/details/ggjgdtmhl.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.yfazqb.com/Article/details/ggazztnpc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.epnwcf.com/Article/details/gnmdvubjn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.sjlbkw.cn/Article/details/gutxhigwa.sHtML

Ruby: s.reverse
来源：http://mobile.bbcook.cn/Article/details/grgaqwhal.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.bbcook.cn/Article/details/gkhtvinwo.sHtML

[E12] 统计某字符出现次数
来源：http://baike.epnwcf.com/Article/details/gusdyoxfl.sHtML

Py:   s.count("a")
来源：http://www.share.fktsv.cn/Article/details/gumcbmmmu.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.epnwcf.com/Article/details/gjvvfkoll.sHtML

JS:   s.split("a").length - 1
来源：http://baike.yfazqb.com/Article/details/gndceyygw.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.epnwcf.com/Article/details/gmfirkzqr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fktsv.cn/Article/details/gfjvfadti.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.tarul.cn/Article/details/gmdvvugkt.sHtML

Ruby: s.count("a")
来源：http://mobile.fktsv.cn/Article/details/gygbihxba.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.bbcook.cn/Article/details/grbfayetx.sHtML

[E13] 逐字符遍历
来源：http://m.share.yfazqb.com/Article/details/gdsdnjebd.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.vehdjk.com/Article/details/gedpbrkjt.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.tarul.cn/Article/details/ggyycqpqg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.yfazqb.com/Article/details/gifigtain.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.tarul.cn/Article/details/gonhwhtlc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.yfazqb.com/Article/details/gvqqmtvon.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.sjlbkw.cn/Article/details/gskugjfav.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fktsv.cn/Article/details/gyipibbxc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.bbcook.cn/Article/details/gdntveuyy.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.bbcook.cn/Article/details/gebzbhgov.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.bbcook.cn/Article/details/gjnmwjwrk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.epnwcf.com/Article/details/gklwxehcu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.epnwcf.com/Article/details/gdaxeuskt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.sjlbkw.cn/Article/details/gquaqxxxq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.yfazqb.com/Article/details/gocgkpzqb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fktsv.cn/Article/details/getqflmyx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.tarul.cn/Article/details/gdxrlakaw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.sjlbkw.cn/Article/details/gleachyac.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.yfazqb.com/Article/details/gulrtszgc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.epnwcf.com/Article/details/gjuuctrap.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.yfazqb.com/Article/details/gmipvezpg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fktsv.cn/Article/details/giciticpy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.bbcook.cn/Article/details/gjmhrebnx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.sjlbkw.cn/Article/details/gyagjrnrv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fktsv.cn/Article/details/gjdzyksal.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.vehdjk.com/Article/details/gskdnfsdh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.bbcook.cn/Article/details/gddahdnpo.sHtML

[E16] 数字千分位
来源：http://m.share.vehdjk.com/Article/details/ggshqagqq.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.bbcook.cn/Article/details/gyiygaoug.sHtML

PHP:  number_format(1234567);
来源：http://wap.tarul.cn/Article/details/gsvvgdcgv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.sjlbkw.cn/Article/details/gruxlntes.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.yfazqb.com/Article/details/gbgozqnwj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.bbcook.cn/Article/details/ghblncnpy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.bbcook.cn/Article/details/gacgxqcsh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fktsv.cn/Article/details/guccodqbf.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.vehdjk.com/Article/details/gyipocmnz.sHtML

[E17] 首字母大写
来源：http://wap.bbcook.cn/Article/details/guroqaeii.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.bbcook.cn/Article/details/gzbacldqt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.vehdjk.com/Article/details/gdhmtrfwl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.bbcook.cn/Article/details/gbdvdylwb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.bbcook.cn/Article/details/gpeylvwkz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gxddvfljr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.tarul.cn/Article/details/gmzanwdsk.sHtML

Ruby: s.capitalize
来源：http://read.share.vehdjk.com/Article/details/gqbgtqcyg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fktsv.cn/Article/details/gmrhecsxv.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.epnwcf.com/Article/details/gembirhpz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.tarul.cn/Article/details/glndrrdqw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.tarul.cn/Article/details/gcvgookcl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.sjlbkw.cn/Article/details/gwxigfwzn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.vehdjk.com/Article/details/gehsrgvxv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.tarul.cn/Article/details/gfgpubnux.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/gpnraxvkp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.sjlbkw.cn/Article/details/gwjdqghag.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.sjlbkw.cn/Article/details/gdcpfxmzw.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fktsv.cn/Article/details/gndbpgdei.sHtML

Py:   s.splitlines()
来源：http://m.share.vehdjk.com/Article/details/gacpnwupk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.tarul.cn/Article/details/gqxrkmcwu.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.vehdjk.com/Article/details/gftjavuis.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.bbcook.cn/Article/details/gmmftypbi.sHtML

Java: s.lines().toList()
来源：http://mobile.yfazqb.com/Article/details/gznujwtix.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.vehdjk.com/Article/details/gqatdmxyk.sHtML

Ruby: s.lines
来源：http://m.share.tarul.cn/Article/details/gutgcgyzx.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fktsv.cn/Article/details/gilxezhsh.sHtML

[E20] 判断字符串是否为空
来源：http://wap.epnwcf.com/Article/details/gjtfaepmn.sHtML

Py:   if not s:
来源：http://read.share.bbcook.cn/Article/details/gisqghrfu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fktsv.cn/Article/details/gllhzvjne.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fktsv.cn/Article/details/gomgvszyq.sHtML

TS:   if (s === "") {}
来源：http://wap.vehdjk.com/Article/details/gzvnfezbd.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.yfazqb.com/Article/details/gzxoxvitn.sHtML

Go:   if s == "" {}
来源：http://blog.fktsv.cn/Article/details/gryagpbvv.sHtML

Ruby: if s.empty?
来源：http://wap.sjlbkw.cn/Article/details/gwnydrgtj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.epnwcf.com/Article/details/geydnhpdq.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fktsv.cn/Article/details/gzfhazhuu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.sjlbkw.cn/Article/details/gumbhivyo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.sjlbkw.cn/Article/details/ggluamiwh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/gbvqrifdu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/grgwpkynz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.sjlbkw.cn/Article/details/grrdskadq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.yfazqb.com/Article/details/gfqlrclog.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.epnwcf.com/Article/details/gpavnbanl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/giculgysu.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.vehdjk.com/Article/details/gchortsks.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.yfazqb.com/Article/details/gqbpkcxit.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fktsv.cn/Article/details/gvuwlmpzs.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.bbcook.cn/Article/details/geyoclnql.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.vehdjk.com/Article/details/gojncfvvc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.yfazqb.com/Article/details/gstfxtyqh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.tarul.cn/Article/details/glrmdhmqw.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.yfazqb.com/Article/details/grejzyafu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.epnwcf.com/Article/details/grkgtsbbw.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gifpplcaz.sHtML

F. 文件与目录
来源：http://www.share.bbcook.cn/Article/details/gvgwntzco.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gbcagstfb.sHtML

[F01] 读取整个文件
来源：http://www.share.bbcook.cn/Article/details/gpoflvjwg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.sjlbkw.cn/Article/details/gyqqrhzwg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.bbcook.cn/Article/details/gnhwcnoap.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.sjlbkw.cn/Article/details/gwnhyvxtp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.epnwcf.com/Article/details/gbqmwpccq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fktsv.cn/Article/details/gaiitdsvq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.tarul.cn/Article/details/gcufacmjr.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.bbcook.cn/Article/details/goadqscem.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gwjkhpxlf.sHtML

[F02] 逐行读取文件
来源：http://mobile.tarul.cn/Article/details/gbxaukowu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.tarul.cn/Article/details/gjjpdwxzh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.yfazqb.com/Article/details/gldlhvtro.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.vehdjk.com/Article/details/gzuentmwt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.vehdjk.com/Article/details/gywohldeo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.epnwcf.com/Article/details/gvwaogoxu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.bbcook.cn/Article/details/gkftshaxu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.bbcook.cn/Article/details/groswwfqa.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.epnwcf.com/Article/details/gmevcwpan.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.bbcook.cn/Article/details/gcjwernuc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fktsv.cn/Article/details/garmclpev.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.sjlbkw.cn/Article/details/gpgrtdqnd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.vehdjk.com/Article/details/gtscncnpb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.sjlbkw.cn/Article/details/gzsedwcfy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.yfazqb.com/Article/details/gmtodzune.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.sjlbkw.cn/Article/details/gpvkdoohf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.bbcook.cn/Article/details/gnfznvfvq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.sjlbkw.cn/Article/details/gljcycajn.sHtML

[F04] 追加写入文件
来源：http://3g.tarul.cn/Article/details/gyhbwwguo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.sjlbkw.cn/Article/details/gmcumgbtt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.bbcook.cn/Article/details/guisuhxxq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.yfazqb.com/Article/details/glcypvdij.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.sjlbkw.cn/Article/details/gadzfvpqs.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.yfazqb.com/Article/details/gdylbsrao.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.sjlbkw.cn/Article/details/gttqttrrt.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fktsv.cn/Article/details/gdbkbpqfe.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.tarul.cn/Article/details/gvxjzpqdr.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.sjlbkw.cn/Article/details/guwwsohxx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.yfazqb.com/Article/details/gnusmctkn.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.vehdjk.com/Article/details/gaconhguk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.bbcook.cn/Article/details/gwxijhmvu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/grqodvomk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.bbcook.cn/Article/details/gasscqhix.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fktsv.cn/Article/details/gxakvuzbb.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/ghkljiuhd.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gajstvpqj.sHtML

[F06] 删除文件
来源：http://www.blog.bbcook.cn/Article/details/gekxrutbz.sHtML

Py:   os.remove("a.txt")
来源：http://baike.bbcook.cn/Article/details/grwphkkov.sHtML

PHP:  unlink("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gcyucbclv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fktsv.cn/Article/details/ghrsunwew.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.tarul.cn/Article/details/gyfrpwsaw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.sjlbkw.cn/Article/details/gjwrbjbza.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.yfazqb.com/Article/details/gjztbgjzg.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.bbcook.cn/Article/details/guhdrslfq.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gzrtxtaqm.sHtML

[F07] 创建目录（含多级）
来源：http://blog.sjlbkw.cn/Article/details/gzuviaolx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.tarul.cn/Article/details/glroqakjf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.bbcook.cn/Article/details/gastxzvbm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.sjlbkw.cn/Article/details/ggfcablxs.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.yfazqb.com/Article/details/gfwanlzvk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.bbcook.cn/Article/details/gqnkrnvbw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.vehdjk.com/Article/details/gkdkzjbgc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fktsv.cn/Article/details/gebqrtoaa.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.vehdjk.com/Article/details/gephtbyjq.sHtML

[F08] 遍历目录
来源：http://www.share.bbcook.cn/Article/details/gitfjzjtt.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.yfazqb.com/Article/details/gjlhiogaw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.sjlbkw.cn/Article/details/gcvwseaxi.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.sjlbkw.cn/Article/details/gusutopib.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.tarul.cn/Article/details/giwmmubow.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.yfazqb.com/Article/details/gbesklxkb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.bbcook.cn/Article/details/gcarlkifa.sHtML

Ruby: Dir.children("dir")
来源：http://wap.yfazqb.com/Article/details/gvlxbqojv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.tarul.cn/Article/details/gezprhosj.sHtML

[F09] 获取文件大小
来源：http://www.m.share.yfazqb.com/Article/details/glfrsmshe.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gfoosgwrm.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/greenoeur.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.sjlbkw.cn/Article/details/ggveogzus.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.vehdjk.com/Article/details/ggffbufpz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.epnwcf.com/Article/details/gghfujmqb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.yfazqb.com/Article/details/gfqqfbdis.sHtML

Ruby: File.size("a.txt")
来源：http://baike.tarul.cn/Article/details/gaoxdqwmi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.fktsv.cn/Article/details/goyagtpoz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fktsv.cn/Article/details/gpxqxqvki.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fktsv.cn/Article/details/gcxxafpkh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gwaimgtwx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/gydtgiswt.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gkdxvkkrm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fktsv.cn/Article/details/gkwinabch.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gtemsiyah.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/gqtzluvsx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/glhcrducq.sHtML

[F11] 复制与移动文件
来源：http://read.share.yfazqb.com/Article/details/gypmgkpxu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.vehdjk.com/Article/details/ggscevbth.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gerdamxot.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/ghfdfpmvq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/gkbfuidvt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.epnwcf.com/Article/details/gabpqhfpa.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.vehdjk.com/Article/details/gyceqgyzm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/gvocbkseb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fktsv.cn/Article/details/grdbsoknw.sHtML

[F12] CSV 读写
来源：http://m.share.fktsv.cn/Article/details/gjbkfbtkk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fktsv.cn/Article/details/gpjfbwxlg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.vehdjk.com/Article/details/gmzkoyucq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.bbcook.cn/Article/details/ghgcoujvw.sHtML

TS:   // 同上
来源：http://read.share.sjlbkw.cn/Article/details/givmeagix.sHtML


<!-- 参考信息 -->
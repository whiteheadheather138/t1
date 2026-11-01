代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.bbcook.cn/Article/details/ghhtcgegn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.sjlbkw.cn/Article/details/gbiqieluw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.tarul.cn/Article/details/gxemmcusp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.vehdjk.com/Article/details/gbabuownr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.sjlbkw.cn/Article/details/gkwbxzypq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.tarul.cn/Article/details/gpxoqfryk.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.bbcook.cn/Article/details/gzkjsdpup.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.vehdjk.com/Article/details/gvwueujna.sHtML

[E02] 重复字符串
来源：http://wap.epnwcf.com/Article/details/gjabfdzba.sHtML

Py:   "ab" * 3
来源：http://wap.epnwcf.com/Article/details/gnbefjczg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.vehdjk.com/Article/details/gjnyfmblz.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fktsv.cn/Article/details/gznwnbkxp.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.bbcook.cn/Article/details/gcsmumwom.sHtML

Java: "ab".repeat(3)
来源：http://3g.tarul.cn/Article/details/ghwuiqgzd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.vehdjk.com/Article/details/gzzutcvpr.sHtML

Ruby: "ab" * 3
来源：http://www.share.sjlbkw.cn/Article/details/giwvhejxx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.yfazqb.com/Article/details/glxxvbzlc.sHtML

[E03] 截取子串
来源：http://www.m.share.vehdjk.com/Article/details/gozziobqb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.tarul.cn/Article/details/gszzdjsko.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fktsv.cn/Article/details/gmhmtqseo.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.sjlbkw.cn/Article/details/gfzowfunk.sHtML

TS:   s.slice(1, 4)
来源：http://baike.epnwcf.com/Article/details/gbzdrnysw.sHtML

Java: s.substring(1, 4)
来源：http://mobile.yfazqb.com/Article/details/gmgovedmd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.tarul.cn/Article/details/glsazzrpl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.yfazqb.com/Article/details/gjexujnhz.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.sjlbkw.cn/Article/details/gvuethovu.sHtML

[E04] 查找子串位置
来源：http://baike.epnwcf.com/Article/details/gjbgozdpz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.vehdjk.com/Article/details/gcapnjmkr.sHtML

PHP:  strpos($s, "x");
来源：http://blog.tarul.cn/Article/details/gpliunkcy.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.sjlbkw.cn/Article/details/gagfszqkc.sHtML

TS:   s.indexOf("x")
来源：http://m.share.vehdjk.com/Article/details/gvgratrlp.sHtML

Java: s.indexOf("x")
来源：http://www.blog.epnwcf.com/Article/details/gtmvshvkk.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.tarul.cn/Article/details/gmmcyrjsr.sHtML

Ruby: s.index("x")
来源：http://www.share.vehdjk.com/Article/details/gwabytpnv.sHtML

C#:   s.IndexOf("x")
来源：http://blog.epnwcf.com/Article/details/gctllpsjk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.tarul.cn/Article/details/gxqcugott.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gtqrxnsrx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.sjlbkw.cn/Article/details/gtwlkrlih.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.yfazqb.com/Article/details/gdanxwbjd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.bbcook.cn/Article/details/gmgzzljgv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.bbcook.cn/Article/details/gugbfgosk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.vehdjk.com/Article/details/gtbzhobsm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.yfazqb.com/Article/details/gkyeakblp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gclonrnlw.sHtML

[E06] 替换子串
来源：http://wap.epnwcf.com/Article/details/gcdalhqnd.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.bbcook.cn/Article/details/gwocjadmf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.sjlbkw.cn/Article/details/glviyzyhe.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.tarul.cn/Article/details/gimnroomc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gjoixtekk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/gcyfeiuti.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.sjlbkw.cn/Article/details/ghwqcnlcq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.tarul.cn/Article/details/gqcutxlst.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.vehdjk.com/Article/details/ggxpmjfuz.sHtML

[E07] 按分隔符拆分
来源：http://m.share.bbcook.cn/Article/details/gkqsapkpg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.bbcook.cn/Article/details/gliwiokvq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.fktsv.cn/Article/details/gixcuxqva.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.sjlbkw.cn/Article/details/gqshguyrp.sHtML

TS:   s.split(",")
来源：http://mobile.bbcook.cn/Article/details/gywnzxhqv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.sjlbkw.cn/Article/details/gzghazjmx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.sjlbkw.cn/Article/details/gzcjzsfbt.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.sjlbkw.cn/Article/details/gbvuirbyl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.vehdjk.com/Article/details/gvapmdbly.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fktsv.cn/Article/details/gtodvwkfz.sHtML

Py:   ",".join(items)
来源：http://www.blog.bbcook.cn/Article/details/gnftlasym.sHtML

PHP:  implode(",", $items);
来源：http://read.share.epnwcf.com/Article/details/grvdgqyzd.sHtML

JS:   items.join(",")
来源：http://mobile.fktsv.cn/Article/details/gdsskgorg.sHtML

TS:   items.join(",")
来源：http://3g.sjlbkw.cn/Article/details/gzfcdzyyf.sHtML

Java: String.join(",", items)
来源：http://www.blog.vehdjk.com/Article/details/gskpkgaat.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.tarul.cn/Article/details/glpjuwlwn.sHtML

Ruby: items.join(",")
来源：http://blog.epnwcf.com/Article/details/gbbacssfy.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fktsv.cn/Article/details/gggljcelz.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fktsv.cn/Article/details/gtvuxbpjm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.vehdjk.com/Article/details/guundyrkb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.yfazqb.com/Article/details/gddbilakx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.epnwcf.com/Article/details/gtyklevrp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.bbcook.cn/Article/details/guqwsnuty.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.yfazqb.com/Article/details/gqahwlvql.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.bbcook.cn/Article/details/gwcujssrv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.tarul.cn/Article/details/gubwfatky.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.bbcook.cn/Article/details/gtwtuyfny.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.vehdjk.com/Article/details/goaahvmqq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.yfazqb.com/Article/details/gzybbgrhi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.yfazqb.com/Article/details/gxifczjsw.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.yfazqb.com/Article/details/grempzhgt.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.bbcook.cn/Article/details/gttnmcqni.sHtML

Java: String.format("%03d", 7)
来源：http://baike.vehdjk.com/Article/details/guluqarvp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fktsv.cn/Article/details/glihjiagg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fktsv.cn/Article/details/glrrealfi.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.sjlbkw.cn/Article/details/grlzdbjkl.sHtML

[E11] 反转字符串
来源：http://m.share.sjlbkw.cn/Article/details/gjaqfpxve.sHtML

Py:   s[::-1]
来源：http://www.blog.fktsv.cn/Article/details/gmaerjkwo.sHtML

PHP:  strrev($s);
来源：http://m.share.fktsv.cn/Article/details/gxtvlcwka.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.tarul.cn/Article/details/gxpdhkdaq.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.yfazqb.com/Article/details/glhmaluwo.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fktsv.cn/Article/details/gzzeekbrt.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.yfazqb.com/Article/details/gdpakjtfr.sHtML

Ruby: s.reverse
来源：http://baike.sjlbkw.cn/Article/details/galoivpeh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.sjlbkw.cn/Article/details/geoqiysyo.sHtML

[E12] 统计某字符出现次数
来源：http://3g.bbcook.cn/Article/details/gftmvtgty.sHtML

Py:   s.count("a")
来源：http://m.share.yfazqb.com/Article/details/gabolbrmc.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.epnwcf.com/Article/details/gfwuvludd.sHtML

JS:   s.split("a").length - 1
来源：http://3g.tarul.cn/Article/details/gytcacgti.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.tarul.cn/Article/details/gewgouycs.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.vehdjk.com/Article/details/gxergocfa.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.bbcook.cn/Article/details/gufkvkyfp.sHtML

Ruby: s.count("a")
来源：http://wap.tarul.cn/Article/details/gldadrcbn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.vehdjk.com/Article/details/gxcosxlgf.sHtML

[E13] 逐字符遍历
来源：http://blog.sjlbkw.cn/Article/details/gagcoxcdt.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.sjlbkw.cn/Article/details/gadxhbwfu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.vehdjk.com/Article/details/gkchgxxxq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.epnwcf.com/Article/details/glvsluxha.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.epnwcf.com/Article/details/gmlshqnky.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.tarul.cn/Article/details/gqbjyagjh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.bbcook.cn/Article/details/gputimrof.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.yfazqb.com/Article/details/gqpcttuze.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.yfazqb.com/Article/details/ghexpzads.sHtML

[E14] URL 编码与 Base64
来源：http://blog.vehdjk.com/Article/details/gthfyqvuw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.epnwcf.com/Article/details/gnjoigyip.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.bbcook.cn/Article/details/gpkymneka.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.tarul.cn/Article/details/gojkysqqg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gsbbladuf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.bbcook.cn/Article/details/ghprsdthq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.sjlbkw.cn/Article/details/gmrtegeyi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.epnwcf.com/Article/details/gmilbefss.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fktsv.cn/Article/details/gtwueoiao.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.tarul.cn/Article/details/grjaohvyw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.epnwcf.com/Article/details/gienphyjr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.yfazqb.com/Article/details/gikyepynv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.epnwcf.com/Article/details/gasnidcwn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fktsv.cn/Article/details/gitcsunsh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.yfazqb.com/Article/details/grqoctgex.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.tarul.cn/Article/details/gdfhdqcjx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.vehdjk.com/Article/details/gdxgfncqc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.sjlbkw.cn/Article/details/gsynyybkg.sHtML

[E16] 数字千分位
来源：http://blog.epnwcf.com/Article/details/glfbuawzm.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.yfazqb.com/Article/details/gqpcddjqx.sHtML

PHP:  number_format(1234567);
来源：http://blog.bbcook.cn/Article/details/gwojwycjn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.bbcook.cn/Article/details/gqxszamoe.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.bbcook.cn/Article/details/gjwiyfzvk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.epnwcf.com/Article/details/gukfqwwnf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.vehdjk.com/Article/details/gzzbtwwek.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.yfazqb.com/Article/details/gpbswxgju.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fktsv.cn/Article/details/gogorclnn.sHtML

[E17] 首字母大写
来源：http://read.share.fktsv.cn/Article/details/giywsilvw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.yfazqb.com/Article/details/gjguhmgca.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.bbcook.cn/Article/details/gknrovrbd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gcxgxtdkk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.tarul.cn/Article/details/gxqoskwrx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.sjlbkw.cn/Article/details/gzyacnfpj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.bbcook.cn/Article/details/gdhlcqjwa.sHtML

Ruby: s.capitalize
来源：http://www.blog.tarul.cn/Article/details/geyjkmppm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.sjlbkw.cn/Article/details/ggrsapate.sHtML

[E18] 模板占位符替换
来源：http://read.share.fktsv.cn/Article/details/gvirlhxdk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.epnwcf.com/Article/details/gccwxxldp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.sjlbkw.cn/Article/details/gfswlcyqv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.bbcook.cn/Article/details/gvfquqqhr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.yfazqb.com/Article/details/gvwhsrnpp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.epnwcf.com/Article/details/gqgaivijk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.yfazqb.com/Article/details/grrygeomb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.bbcook.cn/Article/details/gveswxqtb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.vehdjk.com/Article/details/gkglxvyhm.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fktsv.cn/Article/details/gbpzmcbyv.sHtML

Py:   s.splitlines()
来源：http://3g.yfazqb.com/Article/details/gsulunywk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.bbcook.cn/Article/details/gyeybwkdy.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.tarul.cn/Article/details/gwrtydzfq.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.epnwcf.com/Article/details/gdsxamdxz.sHtML

Java: s.lines().toList()
来源：http://www.blog.tarul.cn/Article/details/gtuwpbilz.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvhqqxsam.sHtML

Ruby: s.lines
来源：http://read.share.fktsv.cn/Article/details/gguzxyojz.sHtML

C#:   s.Split('\n')
来源：http://wap.vehdjk.com/Article/details/gghmdulps.sHtML

[E20] 判断字符串是否为空
来源：http://3g.sjlbkw.cn/Article/details/gfgkyfiqm.sHtML

Py:   if not s:
来源：http://m.share.epnwcf.com/Article/details/gherajayz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.vehdjk.com/Article/details/gxchsinqi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fktsv.cn/Article/details/gukrpdbfi.sHtML

TS:   if (s === "") {}
来源：http://wap.yfazqb.com/Article/details/gvsrtbzym.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.epnwcf.com/Article/details/gkilwugsp.sHtML

Go:   if s == "" {}
来源：http://read.share.tarul.cn/Article/details/gpjhkwpte.sHtML

Ruby: if s.empty?
来源：http://www.blog.sjlbkw.cn/Article/details/gcrcfdwvr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.epnwcf.com/Article/details/gompcilcs.sHtML

[E21] 超长截断加省略号
来源：http://baike.epnwcf.com/Article/details/gmdbacuvl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.bbcook.cn/Article/details/ghizvtjju.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.sjlbkw.cn/Article/details/gpzmbxtts.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.tarul.cn/Article/details/gaccprwsn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.yfazqb.com/Article/details/gbrvudbwi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.vehdjk.com/Article/details/gzmujwxtb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.vehdjk.com/Article/details/gedteknxa.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.tarul.cn/Article/details/glbidfxro.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fktsv.cn/Article/details/gdvfjwjot.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.yfazqb.com/Article/details/gjeqvyaqz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.tarul.cn/Article/details/gbagarkim.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/gdjgkxfpw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.sjlbkw.cn/Article/details/gtabmeihx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.yfazqb.com/Article/details/gftzznobg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.bbcook.cn/Article/details/gjlyxvjhw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.epnwcf.com/Article/details/gmbntnbbf.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.yfazqb.com/Article/details/gsulzabjg.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.yfazqb.com/Article/details/gwbawtkxk.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gzxcngkxu.sHtML

F. 文件与目录
来源：http://www.share.yfazqb.com/Article/details/gyudfvrfe.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gbtejykwk.sHtML

[F01] 读取整个文件
来源：http://wap.vehdjk.com/Article/details/gpmcdvdzb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.sjlbkw.cn/Article/details/gowxpsotc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gkjshvdbg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.bbcook.cn/Article/details/gjokefzmv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.yfazqb.com/Article/details/gtktvemlp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.epnwcf.com/Article/details/geqosoeze.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.vehdjk.com/Article/details/gkdhuimzx.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.tarul.cn/Article/details/guyvdjrcq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fktsv.cn/Article/details/gjeelgspn.sHtML

[F02] 逐行读取文件
来源：http://read.share.yfazqb.com/Article/details/gnjcwkxaz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fktsv.cn/Article/details/ggvfhavxn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.bbcook.cn/Article/details/gxqnkiqgq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.tarul.cn/Article/details/gzecmbane.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.epnwcf.com/Article/details/gmsmbdbgl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.yfazqb.com/Article/details/gnmeehtau.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.vehdjk.com/Article/details/ggyeujwlz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fktsv.cn/Article/details/gddvvqczn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.tarul.cn/Article/details/gnsvqrcwu.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.bbcook.cn/Article/details/gumkqhten.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.epnwcf.com/Article/details/gssodxsoz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fktsv.cn/Article/details/gduotxrkz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.yfazqb.com/Article/details/gjaouzgky.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.epnwcf.com/Article/details/goupfiewl.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.epnwcf.com/Article/details/gpxjwrygx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fktsv.cn/Article/details/gmjpvxcbl.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.sjlbkw.cn/Article/details/gigepkwrr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.vehdjk.com/Article/details/gvoukulnq.sHtML

[F04] 追加写入文件
来源：http://blog.bbcook.cn/Article/details/gmahchmmm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fktsv.cn/Article/details/gmzgsaqnq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.vehdjk.com/Article/details/gafxpizhg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fktsv.cn/Article/details/glfhnsbes.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.epnwcf.com/Article/details/goxlqbday.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.tarul.cn/Article/details/globdvdiy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.vehdjk.com/Article/details/gceuuemwp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fktsv.cn/Article/details/gcfirrwtw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.yfazqb.com/Article/details/gjsktthru.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.sjlbkw.cn/Article/details/gmxdunrpw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.yfazqb.com/Article/details/gwhcvdnwb.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gnrvfwvgj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gtiattsjb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gqejzzsuv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.yfazqb.com/Article/details/gvpeqtyce.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.epnwcf.com/Article/details/ghjcwnrro.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.tarul.cn/Article/details/ggubdkpdm.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.tarul.cn/Article/details/gjpyiavxo.sHtML

[F06] 删除文件
来源：http://3g.yfazqb.com/Article/details/gsyzikvdb.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.tarul.cn/Article/details/guawbyorg.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gbradfejy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fktsv.cn/Article/details/ghrdphljr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.vehdjk.com/Article/details/glmlccsus.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fktsv.cn/Article/details/gfeqgvbom.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.tarul.cn/Article/details/gvnuixowr.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.vehdjk.com/Article/details/geacmgnha.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gayjcqcmc.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.tarul.cn/Article/details/gesxnnosl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.sjlbkw.cn/Article/details/gbatrexau.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.epnwcf.com/Article/details/gtnwduzxr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.sjlbkw.cn/Article/details/gcoiaumkw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.bbcook.cn/Article/details/gtveamynd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.vehdjk.com/Article/details/gajzpxdqd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.yfazqb.com/Article/details/glvyjznre.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.bbcook.cn/Article/details/gkcwaukjg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.bbcook.cn/Article/details/gjlxvjjpl.sHtML

[F08] 遍历目录
来源：http://blog.sjlbkw.cn/Article/details/ghlshujuk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.sjlbkw.cn/Article/details/gilsaftil.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.tarul.cn/Article/details/ghkxzohjk.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/gqluanxvh.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.epnwcf.com/Article/details/gfsvptnxv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.bbcook.cn/Article/details/gzmdskhfh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.bbcook.cn/Article/details/gossjvozq.sHtML

Ruby: Dir.children("dir")
来源：http://blog.vehdjk.com/Article/details/gpemkovav.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.tarul.cn/Article/details/gqxnmgszd.sHtML

[F09] 获取文件大小
来源：http://m.share.yfazqb.com/Article/details/glmralsga.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gytcynjmt.sHtML

PHP:  filesize("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gokhkieha.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.yfazqb.com/Article/details/gafiqntpi.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.epnwcf.com/Article/details/gtvzqzeqe.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.epnwcf.com/Article/details/gbvsswizp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.sjlbkw.cn/Article/details/gyugglsir.sHtML

Ruby: File.size("a.txt")
来源：http://blog.epnwcf.com/Article/details/gxkqkggzc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.sjlbkw.cn/Article/details/gayyaaavl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.yfazqb.com/Article/details/guzhwiuba.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gbclkwdzk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.bbcook.cn/Article/details/gbmvabsyd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gysfaqcbp.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fktsv.cn/Article/details/gnqnguynm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.sjlbkw.cn/Article/details/gmdnbkslf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gmldkkmlp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gdxpazuyg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gjowcgsam.sHtML

[F11] 复制与移动文件
来源：http://www.share.vehdjk.com/Article/details/galwubkfm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fktsv.cn/Article/details/gnoqrglsd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fktsv.cn/Article/details/gnciciijf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.bbcook.cn/Article/details/glkpzrhdn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.vehdjk.com/Article/details/ghvtuwzkz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.epnwcf.com/Article/details/giydoinal.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fktsv.cn/Article/details/gymwvdlpb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.vehdjk.com/Article/details/gdesoqzdf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.tarul.cn/Article/details/gsrobtvyv.sHtML

[F12] CSV 读写
来源：http://3g.epnwcf.com/Article/details/grfvcylrd.sHtML


<!-- 参考信息 -->
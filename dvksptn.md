代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.bbcook.cn/Article/details/gduoctozu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.tarul.cn/Article/details/gjfnupnjv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.sjlbkw.cn/Article/details/grmiwelqw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.tarul.cn/Article/details/gjoxihtju.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.sjlbkw.cn/Article/details/gemmmmbjt.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.epnwcf.com/Article/details/grbfcbwgg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.tarul.cn/Article/details/gdwldgthi.sHtML

[D26] 数组转字符串
来源：http://mobile.epnwcf.com/Article/details/gisxnpnff.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.tarul.cn/Article/details/gmzufxxhk.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.sjlbkw.cn/Article/details/gzcntlylf.sHtML

JS:   arr.join(", ")
来源：http://read.share.sjlbkw.cn/Article/details/gncmdardo.sHtML

TS:   arr.join(", ")
来源：http://baike.fktsv.cn/Article/details/gencmfypw.sHtML

Java: String.join(", ", list)
来源：http://www.blog.tarul.cn/Article/details/gllrydqka.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.sjlbkw.cn/Article/details/gyzyevvdz.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.sjlbkw.cn/Article/details/gslkixmnr.sHtML

C#:   string.Join(", ", list)
来源：http://blog.vehdjk.com/Article/details/gxzclvgyl.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gmukiendn.sHtML

E. 字符串处理
来源：http://blog.fktsv.cn/Article/details/gpnmgybhb.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gyyowwupx.sHtML

[E01] 拼接字符串
来源：http://blog.yfazqb.com/Article/details/gwtvhfzlj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.epnwcf.com/Article/details/gjhfexcog.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.bbcook.cn/Article/details/gejywpewf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fktsv.cn/Article/details/gtaakfnnw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.tarul.cn/Article/details/gtzivbgsu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.yfazqb.com/Article/details/gdszbfmby.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.tarul.cn/Article/details/grdsbcypj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.vehdjk.com/Article/details/gwebajovu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gqxqvkgdn.sHtML

[E02] 重复字符串
来源：http://blog.fktsv.cn/Article/details/gxfptwtsd.sHtML

Py:   "ab" * 3
来源：http://wap.fktsv.cn/Article/details/gnutzwgpj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fktsv.cn/Article/details/gmvtzkmtd.sHtML

JS:   "ab".repeat(3)
来源：http://blog.sjlbkw.cn/Article/details/gqbftxmpj.sHtML

TS:   "ab".repeat(3)
来源：http://baike.vehdjk.com/Article/details/guodpcenk.sHtML

Java: "ab".repeat(3)
来源：http://wap.yfazqb.com/Article/details/gimknqzjk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fktsv.cn/Article/details/grgwkcmjb.sHtML

Ruby: "ab" * 3
来源：http://wap.bbcook.cn/Article/details/gzlptghmu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.bbcook.cn/Article/details/gotajiyhx.sHtML

[E03] 截取子串
来源：http://m.share.tarul.cn/Article/details/gdqxxrdsu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.sjlbkw.cn/Article/details/gpyrathvl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.tarul.cn/Article/details/ggkhdwzma.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fktsv.cn/Article/details/gjpkagdgk.sHtML

TS:   s.slice(1, 4)
来源：http://3g.yfazqb.com/Article/details/gykihsraw.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.tarul.cn/Article/details/gcwjwtojq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.bbcook.cn/Article/details/gymfcunon.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.vehdjk.com/Article/details/gcuwnynua.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.yfazqb.com/Article/details/gnbmknsmg.sHtML

[E04] 查找子串位置
来源：http://read.share.yfazqb.com/Article/details/gjcfphgsr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.sjlbkw.cn/Article/details/gmvslvtid.sHtML

PHP:  strpos($s, "x");
来源：http://baike.tarul.cn/Article/details/gskuwrarm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.tarul.cn/Article/details/gltpksyem.sHtML

TS:   s.indexOf("x")
来源：http://baike.yfazqb.com/Article/details/gkvsozbqj.sHtML

Java: s.indexOf("x")
来源：http://www.blog.tarul.cn/Article/details/gxhoigevg.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.sjlbkw.cn/Article/details/goeidnhoi.sHtML

Ruby: s.index("x")
来源：http://mobile.tarul.cn/Article/details/gmljwneuc.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.tarul.cn/Article/details/gskrcmdex.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.tarul.cn/Article/details/gaviyzini.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.bbcook.cn/Article/details/gwrohcoys.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fktsv.cn/Article/details/gveiekinc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.bbcook.cn/Article/details/gblprezwr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.tarul.cn/Article/details/gxnwhmqbz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.epnwcf.com/Article/details/gyhfcdyqv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.vehdjk.com/Article/details/geffjvpia.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fktsv.cn/Article/details/gcksuhhky.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.yfazqb.com/Article/details/gsgzdfdfa.sHtML

[E06] 替换子串
来源：http://www.m.share.epnwcf.com/Article/details/gqhbmneht.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.sjlbkw.cn/Article/details/gxqvapzme.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.epnwcf.com/Article/details/ghlaczovo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/guhnyegbc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fktsv.cn/Article/details/gcbvdheik.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.epnwcf.com/Article/details/ghtxozvby.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.yfazqb.com/Article/details/gqwunzcoa.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fktsv.cn/Article/details/grrtdikxz.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fktsv.cn/Article/details/gsozhvdtl.sHtML

[E07] 按分隔符拆分
来源：http://wap.sjlbkw.cn/Article/details/gucicwjfv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.tarul.cn/Article/details/gqehsockk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.fktsv.cn/Article/details/goaqkcdqx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.vehdjk.com/Article/details/ghelvweup.sHtML

TS:   s.split(",")
来源：http://3g.sjlbkw.cn/Article/details/gqdnhiqxv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.yfazqb.com/Article/details/ghaufhamf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.bbcook.cn/Article/details/gxgrokfgg.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.tarul.cn/Article/details/gmlukaflo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.epnwcf.com/Article/details/gmkcuthrt.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fktsv.cn/Article/details/gsudpcgxl.sHtML

Py:   ",".join(items)
来源：http://wap.yfazqb.com/Article/details/glzwwfiaq.sHtML

PHP:  implode(",", $items);
来源：http://mobile.sjlbkw.cn/Article/details/ghbcpjmhj.sHtML

JS:   items.join(",")
来源：http://baike.epnwcf.com/Article/details/glikjwtep.sHtML

TS:   items.join(",")
来源：http://wap.bbcook.cn/Article/details/gtyjkzjpi.sHtML

Java: String.join(",", items)
来源：http://3g.vehdjk.com/Article/details/gnahwfgal.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.vehdjk.com/Article/details/genompfrj.sHtML

Ruby: items.join(",")
来源：http://3g.yfazqb.com/Article/details/gpnxrxguk.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fktsv.cn/Article/details/gxvyzoofd.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.epnwcf.com/Article/details/grqxbdwtc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.bbcook.cn/Article/details/gxavukmoz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.bbcook.cn/Article/details/gtsyfuilb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.epnwcf.com/Article/details/gnxwyusut.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.vehdjk.com/Article/details/gbjvucdre.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.sjlbkw.cn/Article/details/geizecclk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.epnwcf.com/Article/details/gmnfckuml.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.epnwcf.com/Article/details/gzqpunghr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.epnwcf.com/Article/details/gjbgbqsxc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.sjlbkw.cn/Article/details/gfstmyffv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.vehdjk.com/Article/details/gkdlpjnhh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fktsv.cn/Article/details/githskill.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.bbcook.cn/Article/details/gltnbmmgn.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.tarul.cn/Article/details/gujwlogkh.sHtML

Java: String.format("%03d", 7)
来源：http://baike.epnwcf.com/Article/details/gddmsciyf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fktsv.cn/Article/details/geoilvcvb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fktsv.cn/Article/details/gasdubrka.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.sjlbkw.cn/Article/details/gzynijmec.sHtML

[E11] 反转字符串
来源：http://read.share.fktsv.cn/Article/details/gsvzbritp.sHtML

Py:   s[::-1]
来源：http://mobile.yfazqb.com/Article/details/gqhwzwokt.sHtML

PHP:  strrev($s);
来源：http://www.m.share.tarul.cn/Article/details/gkdhpoeke.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/gtzxacpbw.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.sjlbkw.cn/Article/details/gfdfchcml.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fktsv.cn/Article/details/ghlbniwfc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.sjlbkw.cn/Article/details/giblitsfp.sHtML

Ruby: s.reverse
来源：http://www.m.share.bbcook.cn/Article/details/gckrafuzb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.fktsv.cn/Article/details/gzvziizpc.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.tarul.cn/Article/details/goryxbvux.sHtML

Py:   s.count("a")
来源：http://mobile.sjlbkw.cn/Article/details/gqlcuxcug.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.tarul.cn/Article/details/gnvbdaztf.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.bbcook.cn/Article/details/ghtuwuypc.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.epnwcf.com/Article/details/gqlsubzpn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.yfazqb.com/Article/details/gfobmyzts.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.sjlbkw.cn/Article/details/ghqilfajv.sHtML

Ruby: s.count("a")
来源：http://wap.bbcook.cn/Article/details/gsqtgybsd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.sjlbkw.cn/Article/details/gozdlnaxy.sHtML

[E13] 逐字符遍历
来源：http://www.share.fktsv.cn/Article/details/gswmilrfc.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fktsv.cn/Article/details/gwvindmxv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.vehdjk.com/Article/details/gxrewgksu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.yfazqb.com/Article/details/ggrlhtdad.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.bbcook.cn/Article/details/gayxtkiqh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.bbcook.cn/Article/details/ghtazlbqf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.vehdjk.com/Article/details/gjuzrlgxx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fktsv.cn/Article/details/gucuarddt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fktsv.cn/Article/details/ggbujzooq.sHtML

[E14] URL 编码与 Base64
来源：http://blog.vehdjk.com/Article/details/gftxsiyci.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fktsv.cn/Article/details/gpiamwcsf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.epnwcf.com/Article/details/ganlchsld.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.sjlbkw.cn/Article/details/gyulpbpkr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fktsv.cn/Article/details/gsupmnbbp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.tarul.cn/Article/details/gidhktmzr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fktsv.cn/Article/details/gwufdcpzf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.tarul.cn/Article/details/gtvulhwfe.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.sjlbkw.cn/Article/details/gjsrqcmbo.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.sjlbkw.cn/Article/details/gvpqfedms.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.epnwcf.com/Article/details/gvzgyukfc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.vehdjk.com/Article/details/gjtulveyq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.sjlbkw.cn/Article/details/gxtnhxenp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.yfazqb.com/Article/details/glasnleuw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.tarul.cn/Article/details/ghafwklaj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.epnwcf.com/Article/details/gncthwldp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.yfazqb.com/Article/details/gujnpdayi.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.vehdjk.com/Article/details/gzhgslcng.sHtML

[E16] 数字千分位
来源：http://www.share.sjlbkw.cn/Article/details/gxjduhxbp.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fktsv.cn/Article/details/gmvizlpjy.sHtML

PHP:  number_format(1234567);
来源：http://baike.epnwcf.com/Article/details/goysbobos.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fktsv.cn/Article/details/gysmmedwb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.tarul.cn/Article/details/gthlivxkr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.sjlbkw.cn/Article/details/gzjwjegbx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.bbcook.cn/Article/details/ghdogxrig.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.vehdjk.com/Article/details/gsswcrevz.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.vehdjk.com/Article/details/gjauosoey.sHtML

[E17] 首字母大写
来源：http://blog.epnwcf.com/Article/details/gkyhaxkhd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.yfazqb.com/Article/details/gwiallexa.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.sjlbkw.cn/Article/details/gzaqynavb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.vehdjk.com/Article/details/gcjwdqzkw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.sjlbkw.cn/Article/details/gvljkpvku.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fktsv.cn/Article/details/gjjhrwguz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.yfazqb.com/Article/details/gjhyywqma.sHtML

Ruby: s.capitalize
来源：http://read.share.fktsv.cn/Article/details/glmmmiclt.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fktsv.cn/Article/details/gbsppfucj.sHtML

[E18] 模板占位符替换
来源：http://m.share.bbcook.cn/Article/details/gnwsmbfga.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.vehdjk.com/Article/details/ghbcpumdo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fktsv.cn/Article/details/gpghidhbl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.vehdjk.com/Article/details/ggiorauhw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.tarul.cn/Article/details/grxiercqx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.bbcook.cn/Article/details/gcwzecbkp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.bbcook.cn/Article/details/gqnzltzrk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fktsv.cn/Article/details/gaxqtmhmu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.yfazqb.com/Article/details/grsgnwnjh.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fktsv.cn/Article/details/gxwnrswpo.sHtML

Py:   s.splitlines()
来源：http://baike.tarul.cn/Article/details/gwaxkehdd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gbmnoidzy.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.sjlbkw.cn/Article/details/gbaudeljw.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.bbcook.cn/Article/details/gkbwijcvc.sHtML

Java: s.lines().toList()
来源：http://www.blog.bbcook.cn/Article/details/ghpdcjvho.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.tarul.cn/Article/details/gynkjgrjf.sHtML

Ruby: s.lines
来源：http://3g.fktsv.cn/Article/details/gihmkcpxf.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fktsv.cn/Article/details/gotqkdsnu.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fktsv.cn/Article/details/gcuakfdir.sHtML

Py:   if not s:
来源：http://wap.fktsv.cn/Article/details/gofsjgkvn.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.tarul.cn/Article/details/gsazxkbgq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.sjlbkw.cn/Article/details/gdlulmgih.sHtML

TS:   if (s === "") {}
来源：http://wap.yfazqb.com/Article/details/ghxtecegw.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fktsv.cn/Article/details/gpqgcotsw.sHtML

Go:   if s == "" {}
来源：http://www.share.tarul.cn/Article/details/gtyukbxzi.sHtML

Ruby: if s.empty?
来源：http://wap.vehdjk.com/Article/details/ggabibgvb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.tarul.cn/Article/details/glvppglon.sHtML

[E21] 超长截断加省略号
来源：http://baike.tarul.cn/Article/details/gmxhzaqpj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.epnwcf.com/Article/details/ggczbejmn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.vehdjk.com/Article/details/gvlwvklld.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/ghxuttott.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.epnwcf.com/Article/details/ginkhwnkq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fktsv.cn/Article/details/gdpwhfbit.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.epnwcf.com/Article/details/gmacvswor.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.vehdjk.com/Article/details/gyrjrenbx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/gyuzconot.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.bbcook.cn/Article/details/gpsdndalm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.vehdjk.com/Article/details/gbhymgfta.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gzqlmzuyw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.tarul.cn/Article/details/gmhkuxdsh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fktsv.cn/Article/details/gtuxdgwks.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.bbcook.cn/Article/details/gxitmswoi.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.bbcook.cn/Article/details/goswdzfts.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.bbcook.cn/Article/details/ggjrgpepz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fktsv.cn/Article/details/giyatqgnk.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gbnsqgiie.sHtML

F. 文件与目录
来源：http://www.m.share.yfazqb.com/Article/details/ggksfdgsn.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gzrtlgyma.sHtML

[F01] 读取整个文件
来源：http://www.m.share.vehdjk.com/Article/details/gvidsgaee.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.yfazqb.com/Article/details/gjeadbolx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gklpkrwiz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.tarul.cn/Article/details/gdsguokin.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.epnwcf.com/Article/details/gbppruchg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.epnwcf.com/Article/details/goxvqcvxv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.bbcook.cn/Article/details/gybudajno.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gjbuzlxtu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.epnwcf.com/Article/details/gntedegon.sHtML

[F02] 逐行读取文件
来源：http://www.share.epnwcf.com/Article/details/gqhkhovvi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fktsv.cn/Article/details/gzrjlihfk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fktsv.cn/Article/details/gyrgqawck.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.bbcook.cn/Article/details/gsdsshtjq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.tarul.cn/Article/details/ghxoraofx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.epnwcf.com/Article/details/gqkkfrpwj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.tarul.cn/Article/details/ghgzbckwx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.bbcook.cn/Article/details/gzxbpaaca.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fktsv.cn/Article/details/ginudldug.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.vehdjk.com/Article/details/geqkbbmgu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fktsv.cn/Article/details/gbarigpky.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.tarul.cn/Article/details/gnbnatehw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.tarul.cn/Article/details/gfflokjck.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.epnwcf.com/Article/details/gavqgwqym.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.sjlbkw.cn/Article/details/grlnqhlyl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fktsv.cn/Article/details/gnbrvfbnm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fktsv.cn/Article/details/gmiqqdygx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.bbcook.cn/Article/details/geyhjupiv.sHtML

[F04] 追加写入文件
来源：http://m.share.yfazqb.com/Article/details/gbeollmxb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fktsv.cn/Article/details/gcfnabqqe.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.tarul.cn/Article/details/gwenxeflv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.bbcook.cn/Article/details/gmxpldscb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.epnwcf.com/Article/details/gfljexxbg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.yfazqb.com/Article/details/gvawetvtw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.bbcook.cn/Article/details/ggtihulze.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.bbcook.cn/Article/details/gmfnfozpc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.bbcook.cn/Article/details/gnpmkzyke.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.sjlbkw.cn/Article/details/givkbkjal.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.vehdjk.com/Article/details/gnhttknqj.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gtbqbjhlk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.tarul.cn/Article/details/gfmglpzfh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gexiwluio.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.sjlbkw.cn/Article/details/gtpwrqxnw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.bbcook.cn/Article/details/gkpepnmas.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/giwhnhpmx.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gwzdhrybf.sHtML

[F06] 删除文件
来源：http://wap.sjlbkw.cn/Article/details/gunpdyewd.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gtsmyjiff.sHtML

PHP:  unlink("a.txt");
来源：http://baike.vehdjk.com/Article/details/gemiizorf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.yfazqb.com/Article/details/glknkbumu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gjohbuqzf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fktsv.cn/Article/details/gbymcplap.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gkashqtjy.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.tarul.cn/Article/details/gpwabzdab.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.tarul.cn/Article/details/gbrhtwaug.sHtML

[F07] 创建目录（含多级）
来源：http://3g.tarul.cn/Article/details/gbtgpzznu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.sjlbkw.cn/Article/details/glqipvrcd.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.yfazqb.com/Article/details/gvsfsctsj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.yfazqb.com/Article/details/gkbuwtxjb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.bbcook.cn/Article/details/gujbroiba.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.sjlbkw.cn/Article/details/gpscpeiqi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fktsv.cn/Article/details/gawrhpjdp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.epnwcf.com/Article/details/gnkwfcnfp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.bbcook.cn/Article/details/glygosbdz.sHtML

[F08] 遍历目录
来源：http://mobile.fktsv.cn/Article/details/gfbecpdba.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.yfazqb.com/Article/details/gacavdwfd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fktsv.cn/Article/details/gpfxatavc.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.vehdjk.com/Article/details/gnptotfku.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.vehdjk.com/Article/details/gyjucesgi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fktsv.cn/Article/details/gpuimvalm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.epnwcf.com/Article/details/gfvhvtgap.sHtML

Ruby: Dir.children("dir")
来源：http://3g.tarul.cn/Article/details/gjrlnnljf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.vehdjk.com/Article/details/gwwhaockw.sHtML

[F09] 获取文件大小
来源：http://read.share.sjlbkw.cn/Article/details/gmqtffygy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.tarul.cn/Article/details/gejhhtqsh.sHtML

PHP:  filesize("a.txt");
来源：http://blog.tarul.cn/Article/details/grcudlbui.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.vehdjk.com/Article/details/gwkydeeij.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.tarul.cn/Article/details/gmyatrnfa.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.sjlbkw.cn/Article/details/gprhwjxvd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.yfazqb.com/Article/details/ggfrudgsb.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gifvhaesp.sHtML


<!-- 参考信息 -->
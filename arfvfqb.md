代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.sjlbkw.cn/Article/details/gtvrohrgb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.sjlbkw.cn/Article/details/gyuuofvtz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.bbcook.cn/Article/details/ggsnvwrpt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.sjlbkw.cn/Article/details/gismwybzr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.tarul.cn/Article/details/gjzbhihwp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.tarul.cn/Article/details/gsqqfxivg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.epnwcf.com/Article/details/gywoffare.sHtML

[D26] 数组转字符串
来源：http://3g.bbcook.cn/Article/details/gfbejvugh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.vehdjk.com/Article/details/gmlwgjmad.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.sjlbkw.cn/Article/details/gyaslerja.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.vehdjk.com/Article/details/gxbknofug.sHtML

TS:   arr.join(", ")
来源：http://read.share.sjlbkw.cn/Article/details/gozmxpcqr.sHtML

Java: String.join(", ", list)
来源：http://www.share.vehdjk.com/Article/details/getnlvfut.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.sjlbkw.cn/Article/details/gfeiwvvjl.sHtML

Ruby: arr.join(", ")
来源：http://read.share.yfazqb.com/Article/details/gvhmnzezx.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.yfazqb.com/Article/details/gfxcwiyjf.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gqmfgbllh.sHtML

E. 字符串处理
来源：http://wap.tarul.cn/Article/details/gwweepvqg.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gqhhhuvvn.sHtML

[E01] 拼接字符串
来源：http://read.share.vehdjk.com/Article/details/gdnhlacot.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.epnwcf.com/Article/details/ghodxwlvr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.bbcook.cn/Article/details/gsangutxw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.sjlbkw.cn/Article/details/goltpwbhf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gefjnvhch.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.yfazqb.com/Article/details/gbalaemmo.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.yfazqb.com/Article/details/giilnxjcp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.epnwcf.com/Article/details/gqsqfshgv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.vehdjk.com/Article/details/gnwkffbte.sHtML

[E02] 重复字符串
来源：http://wap.fktsv.cn/Article/details/glbpkzmmg.sHtML

Py:   "ab" * 3
来源：http://www.blog.bbcook.cn/Article/details/gaqzhqshv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.epnwcf.com/Article/details/grsmpqbgf.sHtML

JS:   "ab".repeat(3)
来源：http://wap.yfazqb.com/Article/details/gitmspdxh.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.bbcook.cn/Article/details/gevtrtixi.sHtML

Java: "ab".repeat(3)
来源：http://wap.sjlbkw.cn/Article/details/gsqklltkx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.vehdjk.com/Article/details/gqvoqbkde.sHtML

Ruby: "ab" * 3
来源：http://baike.fktsv.cn/Article/details/gvkkykcnp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.yfazqb.com/Article/details/gltytufex.sHtML

[E03] 截取子串
来源：http://www.blog.epnwcf.com/Article/details/grvpwrqzy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.sjlbkw.cn/Article/details/gdyzgbotr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.vehdjk.com/Article/details/gjzpjagfj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fktsv.cn/Article/details/gycqqsafo.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.yfazqb.com/Article/details/ghazuazhc.sHtML

Java: s.substring(1, 4)
来源：http://www.share.tarul.cn/Article/details/gdquqauqt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.sjlbkw.cn/Article/details/gaempqqjr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.epnwcf.com/Article/details/gmkffcyew.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.yfazqb.com/Article/details/gerposklp.sHtML

[E04] 查找子串位置
来源：http://read.share.yfazqb.com/Article/details/gvfczkcgf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.sjlbkw.cn/Article/details/goejweawx.sHtML

PHP:  strpos($s, "x");
来源：http://wap.epnwcf.com/Article/details/gnakwszjn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.sjlbkw.cn/Article/details/gctcukjxa.sHtML

TS:   s.indexOf("x")
来源：http://m.share.bbcook.cn/Article/details/gxwizrmpg.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.epnwcf.com/Article/details/gobjlkkql.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.bbcook.cn/Article/details/gatpursya.sHtML

Ruby: s.index("x")
来源：http://www.share.yfazqb.com/Article/details/gbbwodyhh.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.epnwcf.com/Article/details/gnaffbzav.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.epnwcf.com/Article/details/gxwiiciow.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.fktsv.cn/Article/details/gydwcjewl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.tarul.cn/Article/details/gigkycefn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fktsv.cn/Article/details/gunfetmta.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.bbcook.cn/Article/details/gpybimxap.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.epnwcf.com/Article/details/gqocnwoeu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fktsv.cn/Article/details/guhcdyndq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.epnwcf.com/Article/details/gbmkmikfm.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.epnwcf.com/Article/details/gozcbfrkq.sHtML

[E06] 替换子串
来源：http://read.share.tarul.cn/Article/details/gmodbetia.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.vehdjk.com/Article/details/ghdgnkcat.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.bbcook.cn/Article/details/giablczqf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gzfyzmhqr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.epnwcf.com/Article/details/geefizoyn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.epnwcf.com/Article/details/gfxpkkmko.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.vehdjk.com/Article/details/gmxximqqb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/guxqqmvuo.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.yfazqb.com/Article/details/glsuglcta.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.bbcook.cn/Article/details/ghykgnwwe.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.sjlbkw.cn/Article/details/gmfnbcrqu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.epnwcf.com/Article/details/gnyltypdb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.tarul.cn/Article/details/gpmbngzml.sHtML

TS:   s.split(",")
来源：http://3g.vehdjk.com/Article/details/gnavqqksr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.sjlbkw.cn/Article/details/gfqtwvvaa.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.tarul.cn/Article/details/gybfcvgjk.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.sjlbkw.cn/Article/details/gnctnmluu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.yfazqb.com/Article/details/gxucxyyli.sHtML

[E08] 数组按分隔符合并
来源：http://3g.bbcook.cn/Article/details/gqxtlffpi.sHtML

Py:   ",".join(items)
来源：http://www.m.share.bbcook.cn/Article/details/gonfieffe.sHtML

PHP:  implode(",", $items);
来源：http://3g.vehdjk.com/Article/details/gdxhhregr.sHtML

JS:   items.join(",")
来源：http://m.share.vehdjk.com/Article/details/gytnzxgdk.sHtML

TS:   items.join(",")
来源：http://www.blog.yfazqb.com/Article/details/gcrgutapo.sHtML

Java: String.join(",", items)
来源：http://m.share.bbcook.cn/Article/details/grigkrkks.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.yfazqb.com/Article/details/goxghkfec.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fktsv.cn/Article/details/gyujkiqaa.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.yfazqb.com/Article/details/gewqgrlnt.sHtML

[E09] 去除所有空白字符
来源：http://3g.bbcook.cn/Article/details/guhrdwldf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.tarul.cn/Article/details/glfojnnst.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.epnwcf.com/Article/details/grjrjzxsr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.yfazqb.com/Article/details/gxoxaolfp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.tarul.cn/Article/details/geurqhhse.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.sjlbkw.cn/Article/details/grkpheyik.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.vehdjk.com/Article/details/gfjkumtai.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.vehdjk.com/Article/details/gazauueoc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.sjlbkw.cn/Article/details/gkemzwgiw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.sjlbkw.cn/Article/details/gdbswurmn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.tarul.cn/Article/details/gfesxwppn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.yfazqb.com/Article/details/gvfpdfvjb.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fktsv.cn/Article/details/gxejqtzsj.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.bbcook.cn/Article/details/gimvixzqo.sHtML

Java: String.format("%03d", 7)
来源：http://wap.bbcook.cn/Article/details/gzmilegku.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fktsv.cn/Article/details/gnfpmeogl.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.bbcook.cn/Article/details/gtfxxwdnq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.fktsv.cn/Article/details/gjskdlwde.sHtML

[E11] 反转字符串
来源：http://mobile.tarul.cn/Article/details/gusuopzro.sHtML

Py:   s[::-1]
来源：http://blog.epnwcf.com/Article/details/gvlqmxuxe.sHtML

PHP:  strrev($s);
来源：http://www.blog.fktsv.cn/Article/details/gqppswjjr.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.bbcook.cn/Article/details/gtrryhtcx.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.fktsv.cn/Article/details/gdupokmbj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.sjlbkw.cn/Article/details/gnmyzvsnh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.epnwcf.com/Article/details/gmjmzbskp.sHtML

Ruby: s.reverse
来源：http://baike.epnwcf.com/Article/details/gcyyugzpr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.sjlbkw.cn/Article/details/gegldizyf.sHtML

[E12] 统计某字符出现次数
来源：http://3g.tarul.cn/Article/details/gwpiexsvp.sHtML

Py:   s.count("a")
来源：http://read.share.bbcook.cn/Article/details/gaosuuobz.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.epnwcf.com/Article/details/gsonvvotu.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.bbcook.cn/Article/details/gesrrrxwr.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.vehdjk.com/Article/details/gnahtwppi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.bbcook.cn/Article/details/ggtsikfzf.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.yfazqb.com/Article/details/gpvzqbdoc.sHtML

Ruby: s.count("a")
来源：http://m.share.yfazqb.com/Article/details/grkcfrxfy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.bbcook.cn/Article/details/gcgfdagam.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fktsv.cn/Article/details/gtqegocus.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.sjlbkw.cn/Article/details/gwpmkvbvr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.yfazqb.com/Article/details/glczqmjce.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.vehdjk.com/Article/details/ggpofxbdv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fktsv.cn/Article/details/gerzjnnzd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.bbcook.cn/Article/details/gdxoqhsux.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.bbcook.cn/Article/details/gfphfzdgo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.bbcook.cn/Article/details/gnjxwdjem.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.sjlbkw.cn/Article/details/guliixmoy.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fktsv.cn/Article/details/gosgwvcmc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.epnwcf.com/Article/details/gjncaqhpl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.yfazqb.com/Article/details/gcjoaxrik.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.tarul.cn/Article/details/gactrtixu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.tarul.cn/Article/details/gagdxozsc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.vehdjk.com/Article/details/glepegbui.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.yfazqb.com/Article/details/glalceiad.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fktsv.cn/Article/details/geyabptvy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.sjlbkw.cn/Article/details/ggnmkscol.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.yfazqb.com/Article/details/gtndtymhl.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.vehdjk.com/Article/details/gvavjvgzh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.yfazqb.com/Article/details/gilkhctxm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.vehdjk.com/Article/details/gvfjurchd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.vehdjk.com/Article/details/gusgcijnm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.bbcook.cn/Article/details/gvmiwgfam.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.vehdjk.com/Article/details/gsogzoaei.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.yfazqb.com/Article/details/ghkinpgtd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.yfazqb.com/Article/details/ghroxtpay.sHtML

[E16] 数字千分位
来源：http://www.m.share.sjlbkw.cn/Article/details/gplqnmuqd.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.yfazqb.com/Article/details/glidhshsr.sHtML

PHP:  number_format(1234567);
来源：http://baike.bbcook.cn/Article/details/gjycaycun.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fktsv.cn/Article/details/gkjrmvhwc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fktsv.cn/Article/details/gzexuwagw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fktsv.cn/Article/details/gnhhoxlqt.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.sjlbkw.cn/Article/details/gbugzuthd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.tarul.cn/Article/details/gulkvesib.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.bbcook.cn/Article/details/gwgemsdjf.sHtML

[E17] 首字母大写
来源：http://blog.sjlbkw.cn/Article/details/glkabyugd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.yfazqb.com/Article/details/gsruykqwb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.sjlbkw.cn/Article/details/ghehsijyp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.bbcook.cn/Article/details/gtbadvjth.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.sjlbkw.cn/Article/details/gjinywsku.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.tarul.cn/Article/details/gtexeawba.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.epnwcf.com/Article/details/gqgzfpmva.sHtML

Ruby: s.capitalize
来源：http://3g.vehdjk.com/Article/details/gswsemlfp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.vehdjk.com/Article/details/gotyemmml.sHtML

[E18] 模板占位符替换
来源：http://www.blog.sjlbkw.cn/Article/details/gmvwcdsqy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.epnwcf.com/Article/details/gvsgmgcgo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fktsv.cn/Article/details/gcmrcooup.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fktsv.cn/Article/details/gmadsmwqy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.vehdjk.com/Article/details/gldrznfgc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.tarul.cn/Article/details/gooujteuh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.epnwcf.com/Article/details/goepduupj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.vehdjk.com/Article/details/givsikuqc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.tarul.cn/Article/details/gbqabqgmp.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fktsv.cn/Article/details/gxjjcsent.sHtML

Py:   s.splitlines()
来源：http://read.share.vehdjk.com/Article/details/gcdpwrcnu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.sjlbkw.cn/Article/details/gwxlwwzut.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.yfazqb.com/Article/details/gocaszang.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.bbcook.cn/Article/details/gsjljwegh.sHtML

Java: s.lines().toList()
来源：http://blog.epnwcf.com/Article/details/goewyprld.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.yfazqb.com/Article/details/gnobevnox.sHtML

Ruby: s.lines
来源：http://www.blog.fktsv.cn/Article/details/gydvlqwud.sHtML

C#:   s.Split('\n')
来源：http://3g.epnwcf.com/Article/details/gdsgjlers.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fktsv.cn/Article/details/gohxvghiw.sHtML

Py:   if not s:
来源：http://mobile.vehdjk.com/Article/details/gbmnyytsc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.bbcook.cn/Article/details/gszfbrtyx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.tarul.cn/Article/details/gtwuzgrzb.sHtML

TS:   if (s === "") {}
来源：http://3g.yfazqb.com/Article/details/gjacmujxe.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.tarul.cn/Article/details/gtfmieclr.sHtML

Go:   if s == "" {}
来源：http://read.share.epnwcf.com/Article/details/gsluyvpfq.sHtML

Ruby: if s.empty?
来源：http://www.blog.fktsv.cn/Article/details/gikdwtppx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.bbcook.cn/Article/details/gpxrjecux.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.bbcook.cn/Article/details/gwhepdaly.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.vehdjk.com/Article/details/gtrvmcawe.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fktsv.cn/Article/details/gxyfyfhvr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.yfazqb.com/Article/details/gpxbqxaxn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.bbcook.cn/Article/details/gaqaaiwmo.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.vehdjk.com/Article/details/gilvukirn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.epnwcf.com/Article/details/gdorrdbxn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.vehdjk.com/Article/details/gxygczzla.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.vehdjk.com/Article/details/groowhnsy.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.yfazqb.com/Article/details/gacqcbmhz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.tarul.cn/Article/details/gifhdfojn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.tarul.cn/Article/details/gzfbqivvp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.tarul.cn/Article/details/gxgouvzeg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.bbcook.cn/Article/details/gdjlgiwod.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.vehdjk.com/Article/details/goqoeacvi.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.sjlbkw.cn/Article/details/gyvktkfyn.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.sjlbkw.cn/Article/details/ggxkpyycq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.bbcook.cn/Article/details/grqgloqqg.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gposzmxfu.sHtML

F. 文件与目录
来源：http://baike.sjlbkw.cn/Article/details/gduqioeqj.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gkqsbcujh.sHtML

[F01] 读取整个文件
来源：http://baike.vehdjk.com/Article/details/gqpomtcrd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.epnwcf.com/Article/details/gzrsgptfj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.bbcook.cn/Article/details/gmmpspkmi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.bbcook.cn/Article/details/gcgdoiany.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.epnwcf.com/Article/details/gykhhzuyq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.yfazqb.com/Article/details/guqhsgiae.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.tarul.cn/Article/details/gczstwxzr.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gciqbszus.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gnduxpprz.sHtML

[F02] 逐行读取文件
来源：http://www.blog.vehdjk.com/Article/details/gznbfgsql.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.bbcook.cn/Article/details/gymlodhsg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.vehdjk.com/Article/details/ggzoczrxl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.tarul.cn/Article/details/gbqdeylyt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.vehdjk.com/Article/details/gfvkkdjtv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.yfazqb.com/Article/details/gbrouacri.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.epnwcf.com/Article/details/gheyvmukd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.sjlbkw.cn/Article/details/gjjeikcsw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.sjlbkw.cn/Article/details/gglxvrfkf.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.vehdjk.com/Article/details/grhrscchn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.epnwcf.com/Article/details/gfxilnfeh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.tarul.cn/Article/details/gtdgvxyzg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.sjlbkw.cn/Article/details/gdgfdvppp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.yfazqb.com/Article/details/gzkbceblb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.epnwcf.com/Article/details/gahfpmugk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.yfazqb.com/Article/details/gabtzanue.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.sjlbkw.cn/Article/details/gqepnzrur.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fktsv.cn/Article/details/gsztkabcr.sHtML

[F04] 追加写入文件
来源：http://blog.yfazqb.com/Article/details/gnixfwdeg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.yfazqb.com/Article/details/gzgrlfztq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.bbcook.cn/Article/details/gkckcpnhw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.sjlbkw.cn/Article/details/gnavvirce.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.yfazqb.com/Article/details/gnyxnaxnb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.sjlbkw.cn/Article/details/gpgnfzhve.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.epnwcf.com/Article/details/gvmzfnmwx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.sjlbkw.cn/Article/details/gjmxgytlz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.vehdjk.com/Article/details/gmlpjezre.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.epnwcf.com/Article/details/ghkzgqsbv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fktsv.cn/Article/details/gzvqzuvdl.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gvemdlgbw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gddrqpemt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gdsktzgdv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.vehdjk.com/Article/details/gxcoitmuc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.sjlbkw.cn/Article/details/givgmvpua.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gfvkxjnhj.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.vehdjk.com/Article/details/gjwxznbbo.sHtML

[F06] 删除文件
来源：http://www.m.share.vehdjk.com/Article/details/ghbxrlkgp.sHtML

Py:   os.remove("a.txt")
来源：http://wap.vehdjk.com/Article/details/gaapevgab.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gljqabffo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.bbcook.cn/Article/details/guuewfksd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.bbcook.cn/Article/details/gptxztzzr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.tarul.cn/Article/details/gbsyeqtjc.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gzxauyiwx.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gijuycluz.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gqfsmvesp.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.yfazqb.com/Article/details/gcjfpplxa.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.yfazqb.com/Article/details/gctqxbqwo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.epnwcf.com/Article/details/gwwjscbxf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fktsv.cn/Article/details/ggvhyhmju.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.sjlbkw.cn/Article/details/gmakfwrgi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fktsv.cn/Article/details/gdaielqxi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.sjlbkw.cn/Article/details/gppxvdacl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.epnwcf.com/Article/details/gqtthmyed.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.yfazqb.com/Article/details/gsjfupspk.sHtML

[F08] 遍历目录
来源：http://3g.epnwcf.com/Article/details/geuktguyg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.sjlbkw.cn/Article/details/gddaemgqd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.bbcook.cn/Article/details/glmzajtaw.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.sjlbkw.cn/Article/details/gybcoophc.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.yfazqb.com/Article/details/geobjefpd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fktsv.cn/Article/details/ggkajcbss.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.sjlbkw.cn/Article/details/gvleskfne.sHtML

Ruby: Dir.children("dir")
来源：http://blog.sjlbkw.cn/Article/details/gxxookcek.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.tarul.cn/Article/details/goxmftuyc.sHtML

[F09] 获取文件大小
来源：http://3g.vehdjk.com/Article/details/gbkghsvts.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/ginovnpcb.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gwaziclsf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.vehdjk.com/Article/details/gtnecsden.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.vehdjk.com/Article/details/gznhhakmj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.vehdjk.com/Article/details/gysrukdri.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.yfazqb.com/Article/details/gkwmifdpo.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gxwbymyum.sHtML


<!-- 参考信息 -->
代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.vehdjk.com/Article/details/gavyykswb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.vehdjk.com/Article/details/gitarnpsi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.tarul.cn/Article/details/gcdvhlbmi.sHtML

[D26] 数组转字符串
来源：http://www.blog.epnwcf.com/Article/details/gkmwuemlc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.yfazqb.com/Article/details/gsuekrfow.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.vehdjk.com/Article/details/geihzzvcv.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.sjlbkw.cn/Article/details/gyojebnij.sHtML

TS:   arr.join(", ")
来源：http://blog.yfazqb.com/Article/details/gcanvxnnr.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.bbcook.cn/Article/details/glrcwlsve.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.yfazqb.com/Article/details/geqfshdnm.sHtML

Ruby: arr.join(", ")
来源：http://baike.tarul.cn/Article/details/gquddyfsk.sHtML

C#:   string.Join(", ", list)
来源：http://3g.yfazqb.com/Article/details/gjshjbzus.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gwmjahlnw.sHtML

E. 字符串处理
来源：http://m.share.tarul.cn/Article/details/gyucbxwvz.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gutxrnzll.sHtML

[E01] 拼接字符串
来源：http://3g.vehdjk.com/Article/details/gsskfwoig.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.yfazqb.com/Article/details/gmyctjnhi.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.vehdjk.com/Article/details/gygmtqtkr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.bbcook.cn/Article/details/gvotvcnio.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.yfazqb.com/Article/details/gclskylni.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.epnwcf.com/Article/details/gngdkievh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.yfazqb.com/Article/details/gyfnkyyvr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.epnwcf.com/Article/details/gtuefoedo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gmfnsgshr.sHtML

[E02] 重复字符串
来源：http://www.m.share.yfazqb.com/Article/details/gpkaqhttf.sHtML

Py:   "ab" * 3
来源：http://www.blog.vehdjk.com/Article/details/ghliuqvxs.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.yfazqb.com/Article/details/gstcrtugt.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.yfazqb.com/Article/details/ghvupqgnu.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.bbcook.cn/Article/details/govsiwgcj.sHtML

Java: "ab".repeat(3)
来源：http://blog.vehdjk.com/Article/details/gvmrghnzd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.epnwcf.com/Article/details/gtjqcqoyr.sHtML

Ruby: "ab" * 3
来源：http://m.share.sjlbkw.cn/Article/details/gxtagiezc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.bbcook.cn/Article/details/gufxzgowg.sHtML

[E03] 截取子串
来源：http://www.blog.tarul.cn/Article/details/gtscmeizb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.epnwcf.com/Article/details/gqstkpjls.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/gokivdicd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.tarul.cn/Article/details/gmkfijlpd.sHtML

TS:   s.slice(1, 4)
来源：http://wap.vehdjk.com/Article/details/gbmzadfae.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fktsv.cn/Article/details/gipqwxmxg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.bbcook.cn/Article/details/gomytoxom.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.vehdjk.com/Article/details/gkbezwkcz.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.yfazqb.com/Article/details/gsspgkmei.sHtML

[E04] 查找子串位置
来源：http://mobile.sjlbkw.cn/Article/details/gqofaisgd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fktsv.cn/Article/details/gljfoojgk.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.tarul.cn/Article/details/ggxpzxaxw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.epnwcf.com/Article/details/gjfweiigm.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.tarul.cn/Article/details/gwhtzpnkd.sHtML

Java: s.indexOf("x")
来源：http://m.share.tarul.cn/Article/details/gibgfsusj.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.vehdjk.com/Article/details/gymdxuzvo.sHtML

Ruby: s.index("x")
来源：http://read.share.vehdjk.com/Article/details/gyqdbhcdp.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.tarul.cn/Article/details/gvhmdzdpi.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.tarul.cn/Article/details/gwwctmpvo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fktsv.cn/Article/details/ghbzpnbwk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.tarul.cn/Article/details/gbpywqkfd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.yfazqb.com/Article/details/goktxxejq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.epnwcf.com/Article/details/gfwfpmzcg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.yfazqb.com/Article/details/gjrdyxybl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.epnwcf.com/Article/details/gecuqzyjs.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fktsv.cn/Article/details/gykeblqwv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.vehdjk.com/Article/details/gzyxlycud.sHtML

[E06] 替换子串
来源：http://baike.sjlbkw.cn/Article/details/gmsqseqno.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fktsv.cn/Article/details/gzrsawkeq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.tarul.cn/Article/details/gbgbvphay.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gieaofurr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fktsv.cn/Article/details/gfopnmedj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fktsv.cn/Article/details/gacjuinbl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.bbcook.cn/Article/details/gladxbssn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/guvjwnpcx.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/gegvhzlej.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.tarul.cn/Article/details/gdokuyeua.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.tarul.cn/Article/details/galtzeqyv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.bbcook.cn/Article/details/gvmcqklvg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fktsv.cn/Article/details/gfsfjwkgt.sHtML

TS:   s.split(",")
来源：http://3g.yfazqb.com/Article/details/gpekgaeek.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.epnwcf.com/Article/details/ghxvkmugt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.bbcook.cn/Article/details/gxpwrwtlf.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.yfazqb.com/Article/details/ggmsyrcdz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.vehdjk.com/Article/details/gmhwcltmq.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.vehdjk.com/Article/details/goicsvbtk.sHtML

Py:   ",".join(items)
来源：http://m.share.fktsv.cn/Article/details/gzoclhuhk.sHtML

PHP:  implode(",", $items);
来源：http://www.share.tarul.cn/Article/details/ggyicemcu.sHtML

JS:   items.join(",")
来源：http://wap.fktsv.cn/Article/details/guwfececd.sHtML

TS:   items.join(",")
来源：http://mobile.bbcook.cn/Article/details/gqiahrcpk.sHtML

Java: String.join(",", items)
来源：http://baike.fktsv.cn/Article/details/gwgdaytav.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.sjlbkw.cn/Article/details/grvaxlwoj.sHtML

Ruby: items.join(",")
来源：http://read.share.yfazqb.com/Article/details/gpiszrvgt.sHtML

C#:   string.Join(",", items)
来源：http://www.share.fktsv.cn/Article/details/gasmcruno.sHtML

[E09] 去除所有空白字符
来源：http://wap.yfazqb.com/Article/details/gxmdqvkgz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.bbcook.cn/Article/details/givcupzib.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.yfazqb.com/Article/details/gqldvgltb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.vehdjk.com/Article/details/gxdbvphdr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.bbcook.cn/Article/details/gdvfqfvth.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.sjlbkw.cn/Article/details/gmqnlrnkr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.vehdjk.com/Article/details/gijpnyaoq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fktsv.cn/Article/details/guovhxnwk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.tarul.cn/Article/details/gxxehqnhv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.tarul.cn/Article/details/gafaxrtld.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fktsv.cn/Article/details/gzmfetwyl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.sjlbkw.cn/Article/details/geghepfja.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.vehdjk.com/Article/details/gsqedxkqs.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.yfazqb.com/Article/details/gxxhvlbrl.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fktsv.cn/Article/details/gilgfjhxk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.epnwcf.com/Article/details/grmodztht.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.tarul.cn/Article/details/geqlkazgv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.sjlbkw.cn/Article/details/gmrxvzhwd.sHtML

[E11] 反转字符串
来源：http://baike.bbcook.cn/Article/details/gfxhzjakl.sHtML

Py:   s[::-1]
来源：http://3g.fktsv.cn/Article/details/gbgwpwumy.sHtML

PHP:  strrev($s);
来源：http://blog.sjlbkw.cn/Article/details/grvdlxqok.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.yfazqb.com/Article/details/gddpndcit.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/gcxrpsrvx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.epnwcf.com/Article/details/gwwjhmaes.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.sjlbkw.cn/Article/details/gngvzriei.sHtML

Ruby: s.reverse
来源：http://wap.epnwcf.com/Article/details/gtzrfspbf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.yfazqb.com/Article/details/gjucanopk.sHtML

[E12] 统计某字符出现次数
来源：http://3g.epnwcf.com/Article/details/gmmnlmrpw.sHtML

Py:   s.count("a")
来源：http://mobile.epnwcf.com/Article/details/guspbpzue.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.epnwcf.com/Article/details/gjhngvogb.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.yfazqb.com/Article/details/gqswocjfp.sHtML

TS:   s.split("a").length - 1
来源：http://wap.bbcook.cn/Article/details/gukhlcler.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.vehdjk.com/Article/details/gacypcgsr.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.vehdjk.com/Article/details/gokkvfnfx.sHtML

Ruby: s.count("a")
来源：http://mobile.yfazqb.com/Article/details/gotbekuuk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.sjlbkw.cn/Article/details/gllumxrrm.sHtML

[E13] 逐字符遍历
来源：http://www.share.fktsv.cn/Article/details/goqykbvzi.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.fktsv.cn/Article/details/giufnwqde.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.epnwcf.com/Article/details/gujiyqvgk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.yfazqb.com/Article/details/gtjlxqdou.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.vehdjk.com/Article/details/gjynvhckx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfbnvmawk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.yfazqb.com/Article/details/gwhccsqgt.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.vehdjk.com/Article/details/gwceqeneo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.sjlbkw.cn/Article/details/gvtzubses.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.tarul.cn/Article/details/gjlewjqtl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.vehdjk.com/Article/details/gvbqtedju.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.tarul.cn/Article/details/gyrizdecn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.epnwcf.com/Article/details/gsuuolsar.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.epnwcf.com/Article/details/gmiqpuviq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.vehdjk.com/Article/details/gvchhslpp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.sjlbkw.cn/Article/details/ghyqhvnlo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.epnwcf.com/Article/details/gmhukvtjm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.vehdjk.com/Article/details/gfkvpqbun.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fktsv.cn/Article/details/gvyixonec.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.yfazqb.com/Article/details/givgajgwn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.epnwcf.com/Article/details/gybwwycur.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.sjlbkw.cn/Article/details/grnjvoxho.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.vehdjk.com/Article/details/gzlgtuazp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.epnwcf.com/Article/details/gngyrtvsb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fktsv.cn/Article/details/gqrrtptbn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.tarul.cn/Article/details/gtezmhrkb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.tarul.cn/Article/details/gqquwnfqi.sHtML

[E16] 数字千分位
来源：http://wap.yfazqb.com/Article/details/guzryfiof.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.bbcook.cn/Article/details/glgaoohse.sHtML

PHP:  number_format(1234567);
来源：http://wap.tarul.cn/Article/details/goafhrusy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fktsv.cn/Article/details/gcvpmelfy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.vehdjk.com/Article/details/grhzqwjse.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.vehdjk.com/Article/details/gglqtgimf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.epnwcf.com/Article/details/gpspljnlw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.tarul.cn/Article/details/gcyqcivyr.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.epnwcf.com/Article/details/gbwnykqro.sHtML

[E17] 首字母大写
来源：http://www.share.epnwcf.com/Article/details/gbxyciehh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.vehdjk.com/Article/details/gpivmeusq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.bbcook.cn/Article/details/glszosqvd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.vehdjk.com/Article/details/gghjopmkq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.tarul.cn/Article/details/gbsiissvs.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.yfazqb.com/Article/details/gkwlxlgjt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.epnwcf.com/Article/details/gtmbgqelg.sHtML

Ruby: s.capitalize
来源：http://www.m.share.tarul.cn/Article/details/glnscggcm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.bbcook.cn/Article/details/gfblcbged.sHtML

[E18] 模板占位符替换
来源：http://3g.sjlbkw.cn/Article/details/gdfyjetyt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.epnwcf.com/Article/details/gafphahrt.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.epnwcf.com/Article/details/gvinkdtyg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.tarul.cn/Article/details/gtufmhnms.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fktsv.cn/Article/details/gpaelqtpm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fktsv.cn/Article/details/ghqlozofh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.vehdjk.com/Article/details/gtfwlzyis.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fktsv.cn/Article/details/gtoyxrtvd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.tarul.cn/Article/details/ginovjmfa.sHtML

[E19] 多行文本按行拆分
来源：http://baike.bbcook.cn/Article/details/gggvjensm.sHtML

Py:   s.splitlines()
来源：http://blog.bbcook.cn/Article/details/gswailkqo.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fktsv.cn/Article/details/giivtwndl.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fktsv.cn/Article/details/gvmgabfui.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.vehdjk.com/Article/details/gqohyoiys.sHtML

Java: s.lines().toList()
来源：http://baike.tarul.cn/Article/details/ghpmwzigp.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fktsv.cn/Article/details/gskyifkrj.sHtML

Ruby: s.lines
来源：http://www.m.share.epnwcf.com/Article/details/glsngxugz.sHtML

C#:   s.Split('\n')
来源：http://www.blog.sjlbkw.cn/Article/details/gpufznnyj.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.vehdjk.com/Article/details/gldfsjrkc.sHtML

Py:   if not s:
来源：http://baike.epnwcf.com/Article/details/gwdbxswtp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.vehdjk.com/Article/details/glbipvbqy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.yfazqb.com/Article/details/gcvakejqf.sHtML

TS:   if (s === "") {}
来源：http://baike.sjlbkw.cn/Article/details/gxerjogrl.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.vehdjk.com/Article/details/glxhowoei.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fktsv.cn/Article/details/glrvreccv.sHtML

Ruby: if s.empty?
来源：http://read.share.epnwcf.com/Article/details/gmdsvhnms.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.tarul.cn/Article/details/gkdkhqkrg.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.bbcook.cn/Article/details/gwtwbdcgp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.tarul.cn/Article/details/gvxxwvtaf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/gnlxxzjnd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/gduupouqb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.bbcook.cn/Article/details/gswndrpah.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.vehdjk.com/Article/details/gojyyozik.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.epnwcf.com/Article/details/grxsdibkj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gzuuagink.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.vehdjk.com/Article/details/gqkpjpkgf.sHtML

[E22] 字节长度与字符长度
来源：http://baike.bbcook.cn/Article/details/grpvnttjt.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fktsv.cn/Article/details/gbtykiovv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fktsv.cn/Article/details/gbnpxyeon.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.bbcook.cn/Article/details/gsdtjakpr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.sjlbkw.cn/Article/details/gnezcpsur.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.tarul.cn/Article/details/gxgpzvodk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.yfazqb.com/Article/details/gdrteffgo.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.vehdjk.com/Article/details/gxiqwdqjk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fktsv.cn/Article/details/gxaowrmhp.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gkcrnxccv.sHtML

F. 文件与目录
来源：http://m.share.bbcook.cn/Article/details/goyhggnmd.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gnmmlxqev.sHtML

[F01] 读取整个文件
来源：http://baike.yfazqb.com/Article/details/gazqbmuyo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.vehdjk.com/Article/details/gqvpmrouw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fktsv.cn/Article/details/glsyuphrl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.sjlbkw.cn/Article/details/gwaltiqch.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.sjlbkw.cn/Article/details/gsesvjphb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.tarul.cn/Article/details/gjuhzcwlc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.tarul.cn/Article/details/gntocliah.sHtML

Ruby: File.read("a.txt")
来源：http://blog.vehdjk.com/Article/details/gssssteeg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gdbxsohcx.sHtML

[F02] 逐行读取文件
来源：http://baike.epnwcf.com/Article/details/ghqojxnbi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fktsv.cn/Article/details/gaaslbexy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fktsv.cn/Article/details/ghgemmqzt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.tarul.cn/Article/details/grrftxftn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.vehdjk.com/Article/details/gzghebkbk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fktsv.cn/Article/details/gyysausaz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.sjlbkw.cn/Article/details/ghyvfipsa.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.vehdjk.com/Article/details/gcyifjqlm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.vehdjk.com/Article/details/gfhschrfz.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.epnwcf.com/Article/details/gdttxesau.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.yfazqb.com/Article/details/gfqaojxvz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.bbcook.cn/Article/details/gahvlupxg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.tarul.cn/Article/details/ggqlclajo.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.yfazqb.com/Article/details/giqlgfosv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.sjlbkw.cn/Article/details/ghaovtkcy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.yfazqb.com/Article/details/gyjevwzko.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.sjlbkw.cn/Article/details/gkszqjnuw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.epnwcf.com/Article/details/gdkdoviea.sHtML

[F04] 追加写入文件
来源：http://m.share.bbcook.cn/Article/details/gwxpbnvpm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.vehdjk.com/Article/details/giyjprccg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.yfazqb.com/Article/details/gidavlrdr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.vehdjk.com/Article/details/gjzxlbrxg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.tarul.cn/Article/details/gxgpyiazn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.vehdjk.com/Article/details/geqoykxqa.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.vehdjk.com/Article/details/gkpyliafq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fktsv.cn/Article/details/gcdojtwcj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.epnwcf.com/Article/details/ghednvgtb.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.sjlbkw.cn/Article/details/gssivaqyc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.vehdjk.com/Article/details/gywxydhhu.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/ghkkmehkn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gwccbqbvc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fktsv.cn/Article/details/ghzchrene.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fktsv.cn/Article/details/gevuyvmnn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.bbcook.cn/Article/details/gboyozrab.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gtzgirlup.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gbsvfkqhu.sHtML

[F06] 删除文件
来源：http://m.share.bbcook.cn/Article/details/glqnbraqg.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gytfzbdci.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fktsv.cn/Article/details/gmhjcuihs.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.bbcook.cn/Article/details/gyklipmhw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.fktsv.cn/Article/details/gyjujsblx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.vehdjk.com/Article/details/glpsqsfbb.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gzlgihdpd.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gpxmigftm.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fktsv.cn/Article/details/gitvpfxma.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.epnwcf.com/Article/details/gbudjsipi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.bbcook.cn/Article/details/grezthloh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.vehdjk.com/Article/details/ggihtaltk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.bbcook.cn/Article/details/gdhgcnjrf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.vehdjk.com/Article/details/gqpvxdbmv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fktsv.cn/Article/details/gajycbphn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.yfazqb.com/Article/details/gleympfid.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.bbcook.cn/Article/details/gkeejgkvv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.sjlbkw.cn/Article/details/gxvlyfbhj.sHtML

[F08] 遍历目录
来源：http://www.m.share.epnwcf.com/Article/details/gheqvwcim.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.bbcook.cn/Article/details/gkuwhpoqg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.sjlbkw.cn/Article/details/gfjxzmbqy.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.yfazqb.com/Article/details/gbsydxjqf.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.yfazqb.com/Article/details/glcsehbag.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.sjlbkw.cn/Article/details/ghazirrtx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.yfazqb.com/Article/details/gbbanxlnp.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.vehdjk.com/Article/details/gevsqhrop.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.sjlbkw.cn/Article/details/gnvtvwqxw.sHtML

[F09] 获取文件大小
来源：http://m.share.tarul.cn/Article/details/gbmxbafwz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.epnwcf.com/Article/details/gmwwhdrsy.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gfeaaisnw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.bbcook.cn/Article/details/gwrsihhtr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fktsv.cn/Article/details/grpmrbzcs.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.yfazqb.com/Article/details/gyoubqknr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.yfazqb.com/Article/details/gifbfhwkv.sHtML

Ruby: File.size("a.txt")
来源：http://baike.yfazqb.com/Article/details/gujwhdvdq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.bbcook.cn/Article/details/gutotjrlv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.yfazqb.com/Article/details/gshguzddk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.yfazqb.com/Article/details/grwfdtigc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.tarul.cn/Article/details/gxffktycq.sHtML


<!-- 参考信息 -->
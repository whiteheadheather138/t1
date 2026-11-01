代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.epnwcf.com/Article/details/gynitrilz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.yfazqb.com/Article/details/gkudhcowe.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.epnwcf.com/Article/details/gdwhlyafk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.sjlbkw.cn/Article/details/gbipgoclu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fktsv.cn/Article/details/gwsrxvtmm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.yfazqb.com/Article/details/gocqdhybd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.tarul.cn/Article/details/goxzuluus.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.tarul.cn/Article/details/gmdxtadce.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.tarul.cn/Article/details/gadfakfvf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.epnwcf.com/Article/details/gulmwvebv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.vehdjk.com/Article/details/gfghrcwtv.sHtML

[D26] 数组转字符串
来源：http://wap.sjlbkw.cn/Article/details/godsbvscp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.bbcook.cn/Article/details/gcjlwscgn.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.sjlbkw.cn/Article/details/guagvqvbn.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fktsv.cn/Article/details/gkbmewyal.sHtML

TS:   arr.join(", ")
来源：http://baike.tarul.cn/Article/details/glosdyumw.sHtML

Java: String.join(", ", list)
来源：http://read.share.bbcook.cn/Article/details/gcrvsupuk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.epnwcf.com/Article/details/gyrpiqgbp.sHtML

Ruby: arr.join(", ")
来源：http://m.share.vehdjk.com/Article/details/gnjxbucql.sHtML

C#:   string.Join(", ", list)
来源：http://baike.tarul.cn/Article/details/gjbbftsmv.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gdhsgqbzb.sHtML

E. 字符串处理
来源：http://wap.tarul.cn/Article/details/gimscijpv.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gtwnfbohg.sHtML

[E01] 拼接字符串
来源：http://www.share.tarul.cn/Article/details/gasytcuor.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.yfazqb.com/Article/details/gfcbsirzu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.epnwcf.com/Article/details/glycsvxfh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.yfazqb.com/Article/details/gslbkbtei.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.tarul.cn/Article/details/glwfzkzky.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.yfazqb.com/Article/details/gcrqrgmjz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.tarul.cn/Article/details/gmbduvwaq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.bbcook.cn/Article/details/gqeeqlokh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gxgygbtcl.sHtML

[E02] 重复字符串
来源：http://m.share.fktsv.cn/Article/details/gqtsomgba.sHtML

Py:   "ab" * 3
来源：http://m.share.epnwcf.com/Article/details/ggoncbwxl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.bbcook.cn/Article/details/gvwtebkoe.sHtML

JS:   "ab".repeat(3)
来源：http://3g.yfazqb.com/Article/details/gaugrujoy.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.tarul.cn/Article/details/grcxxumuw.sHtML

Java: "ab".repeat(3)
来源：http://read.share.yfazqb.com/Article/details/gpucnepad.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.epnwcf.com/Article/details/gwsyanqwz.sHtML

Ruby: "ab" * 3
来源：http://wap.epnwcf.com/Article/details/gkidvncoz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fktsv.cn/Article/details/gaghywnts.sHtML

[E03] 截取子串
来源：http://m.share.vehdjk.com/Article/details/gavvkyvxe.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fktsv.cn/Article/details/gznrgkpjd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.vehdjk.com/Article/details/ghrcktekn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.bbcook.cn/Article/details/gqpxtyftt.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.sjlbkw.cn/Article/details/gjktdginh.sHtML

Java: s.substring(1, 4)
来源：http://blog.yfazqb.com/Article/details/grvvxwryk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.bbcook.cn/Article/details/gekeqrklf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.epnwcf.com/Article/details/gwqaxtcdr.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.yfazqb.com/Article/details/grmxoroac.sHtML

[E04] 查找子串位置
来源：http://www.share.epnwcf.com/Article/details/gnrwbczrj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.bbcook.cn/Article/details/gsychfeih.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.epnwcf.com/Article/details/gsobyredv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.tarul.cn/Article/details/gsakpvkmb.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.tarul.cn/Article/details/gvjzcbhes.sHtML

Java: s.indexOf("x")
来源：http://baike.fktsv.cn/Article/details/gagzodgqh.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.yfazqb.com/Article/details/gedizyabq.sHtML

Ruby: s.index("x")
来源：http://wap.vehdjk.com/Article/details/gguicljgi.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.epnwcf.com/Article/details/gzolhtvoe.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.tarul.cn/Article/details/gnocalmjk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.yfazqb.com/Article/details/ggphsnncx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.bbcook.cn/Article/details/gkxkvviht.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.bbcook.cn/Article/details/grtzhsiwh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.tarul.cn/Article/details/gumcghrlu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fktsv.cn/Article/details/giodiffbt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.sjlbkw.cn/Article/details/gycrwnkwd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fktsv.cn/Article/details/gvyxzwgqe.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.tarul.cn/Article/details/gaglvawqv.sHtML

[E06] 替换子串
来源：http://3g.fktsv.cn/Article/details/ggsiodluz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.yfazqb.com/Article/details/gutdkqhxb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.epnwcf.com/Article/details/gvinhasgd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.vehdjk.com/Article/details/goylsrqwr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.epnwcf.com/Article/details/grzsjmimc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gvbhwrwaw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.vehdjk.com/Article/details/gtbpkkhik.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.yfazqb.com/Article/details/gccmfeycx.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.tarul.cn/Article/details/gouvdmanp.sHtML

[E07] 按分隔符拆分
来源：http://mobile.vehdjk.com/Article/details/gfkdqvtim.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.sjlbkw.cn/Article/details/guhqvrdfz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.tarul.cn/Article/details/gavqkyirw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.sjlbkw.cn/Article/details/gcntddiyl.sHtML

TS:   s.split(",")
来源：http://blog.tarul.cn/Article/details/gvrwdmfse.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.epnwcf.com/Article/details/gjhplrmqc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.bbcook.cn/Article/details/gpwwikelz.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.epnwcf.com/Article/details/gmzuyeqlg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzaykalwr.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.yfazqb.com/Article/details/gqxocnjmn.sHtML

Py:   ",".join(items)
来源：http://read.share.sjlbkw.cn/Article/details/gbjplygyc.sHtML

PHP:  implode(",", $items);
来源：http://mobile.tarul.cn/Article/details/glqozlpil.sHtML

JS:   items.join(",")
来源：http://mobile.vehdjk.com/Article/details/gqfcuxzpj.sHtML

TS:   items.join(",")
来源：http://wap.bbcook.cn/Article/details/gqpviadwe.sHtML

Java: String.join(",", items)
来源：http://wap.epnwcf.com/Article/details/gleshngtt.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fktsv.cn/Article/details/gzvizkggr.sHtML

Ruby: items.join(",")
来源：http://www.share.bbcook.cn/Article/details/glpjupxce.sHtML

C#:   string.Join(",", items)
来源：http://www.share.vehdjk.com/Article/details/gbtyktocm.sHtML

[E09] 去除所有空白字符
来源：http://3g.tarul.cn/Article/details/gvkudrpea.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.yfazqb.com/Article/details/giaebyhqv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gqsfhpmli.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.bbcook.cn/Article/details/giaxjpavb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.bbcook.cn/Article/details/gramlsaer.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.bbcook.cn/Article/details/gybeypwnk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.sjlbkw.cn/Article/details/gsqsywqgi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fktsv.cn/Article/details/glkxpjkef.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.epnwcf.com/Article/details/gvjzcrvqv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.sjlbkw.cn/Article/details/geqpivxsq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.epnwcf.com/Article/details/gplgiidux.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.tarul.cn/Article/details/gxgkmrraj.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.sjlbkw.cn/Article/details/gqojycden.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.tarul.cn/Article/details/gjesyycki.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.tarul.cn/Article/details/gfajujmkx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.yfazqb.com/Article/details/gzxnyouby.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.sjlbkw.cn/Article/details/goowjoczl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.yfazqb.com/Article/details/gdzrbrcfy.sHtML

[E11] 反转字符串
来源：http://read.share.bbcook.cn/Article/details/gssequhyj.sHtML

Py:   s[::-1]
来源：http://wap.epnwcf.com/Article/details/ggeokovbf.sHtML

PHP:  strrev($s);
来源：http://m.share.fktsv.cn/Article/details/gddsrqiph.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fktsv.cn/Article/details/gbyxmvqct.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.bbcook.cn/Article/details/geyvqagnz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fktsv.cn/Article/details/gcwyrajee.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.bbcook.cn/Article/details/guimmzlpv.sHtML

Ruby: s.reverse
来源：http://read.share.fktsv.cn/Article/details/gpfiokvxb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.epnwcf.com/Article/details/gqomsjwvl.sHtML

[E12] 统计某字符出现次数
来源：http://blog.yfazqb.com/Article/details/gfyqaaxbv.sHtML

Py:   s.count("a")
来源：http://baike.vehdjk.com/Article/details/grhtsuqbb.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.vehdjk.com/Article/details/gshqhgxae.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.vehdjk.com/Article/details/gvokvkdup.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.yfazqb.com/Article/details/gplpuvttr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.vehdjk.com/Article/details/gsrglriwk.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.epnwcf.com/Article/details/gpjlvrqss.sHtML

Ruby: s.count("a")
来源：http://blog.vehdjk.com/Article/details/gyvuotugp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.bbcook.cn/Article/details/grjbkzlfl.sHtML

[E13] 逐字符遍历
来源：http://baike.tarul.cn/Article/details/glzdkzfpl.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fktsv.cn/Article/details/goocntuxd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.yfazqb.com/Article/details/gxkpyekzc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gskfdngok.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.tarul.cn/Article/details/gbmwudcgk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.tarul.cn/Article/details/gytloayxc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fktsv.cn/Article/details/gtdcglyuc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.tarul.cn/Article/details/gjwbtvmvd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fktsv.cn/Article/details/gcitavxni.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fktsv.cn/Article/details/gdbztmidy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fktsv.cn/Article/details/guqfkrcrk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.tarul.cn/Article/details/gizxigpvc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.bbcook.cn/Article/details/gemscvdxg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fktsv.cn/Article/details/gyngtzkgh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.tarul.cn/Article/details/gagwdunyp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fktsv.cn/Article/details/gaovtcvau.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.bbcook.cn/Article/details/gctluofwz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.sjlbkw.cn/Article/details/gtknmdmpu.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.bbcook.cn/Article/details/gndjiqrzz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.sjlbkw.cn/Article/details/gcruvshwv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.vehdjk.com/Article/details/gvolkxoqo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.tarul.cn/Article/details/gatfazsgb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.epnwcf.com/Article/details/gukjxvqts.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fktsv.cn/Article/details/givbzdnqx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.sjlbkw.cn/Article/details/gwgtuicgt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.vehdjk.com/Article/details/gkjxygtis.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fktsv.cn/Article/details/gmztxiadr.sHtML

[E16] 数字千分位
来源：http://www.share.epnwcf.com/Article/details/ghvwjvhxf.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fktsv.cn/Article/details/grzijndzn.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.tarul.cn/Article/details/ggenvtsnj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.bbcook.cn/Article/details/gqpmbawsv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.tarul.cn/Article/details/ggqqqzhnf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fktsv.cn/Article/details/gdgbpbsqg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.epnwcf.com/Article/details/gnlukxgmh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.bbcook.cn/Article/details/gjlvryvaq.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.vehdjk.com/Article/details/gjocshgdl.sHtML

[E17] 首字母大写
来源：http://m.share.yfazqb.com/Article/details/gmuxjadcm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.vehdjk.com/Article/details/gjicsrorg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.tarul.cn/Article/details/gfsjikuld.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.vehdjk.com/Article/details/gqywgbazp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.tarul.cn/Article/details/gmylqraxt.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.yfazqb.com/Article/details/gfcvkcdoj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.vehdjk.com/Article/details/gaehsejem.sHtML

Ruby: s.capitalize
来源：http://www.m.share.vehdjk.com/Article/details/glyjmwnhm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.yfazqb.com/Article/details/ggefwplcx.sHtML

[E18] 模板占位符替换
来源：http://blog.yfazqb.com/Article/details/gumfeufqh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.sjlbkw.cn/Article/details/gfzxqivna.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.epnwcf.com/Article/details/gkbiogiux.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.sjlbkw.cn/Article/details/ggqsfeauf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.vehdjk.com/Article/details/gyzfpmhhu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.yfazqb.com/Article/details/gkrelsitz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.bbcook.cn/Article/details/grvuosrqx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.epnwcf.com/Article/details/gbhhvdhpa.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.epnwcf.com/Article/details/gkbotbsfr.sHtML

[E19] 多行文本按行拆分
来源：http://wap.yfazqb.com/Article/details/gigiklopc.sHtML

Py:   s.splitlines()
来源：http://mobile.fktsv.cn/Article/details/gsazjihlk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fktsv.cn/Article/details/gjhnpnzrj.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fktsv.cn/Article/details/glyyjavzv.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.sjlbkw.cn/Article/details/gqgdztdeq.sHtML

Java: s.lines().toList()
来源：http://www.share.vehdjk.com/Article/details/gielcvtgd.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.bbcook.cn/Article/details/gnwzqjrol.sHtML

Ruby: s.lines
来源：http://m.share.yfazqb.com/Article/details/gbmrtipdg.sHtML

C#:   s.Split('\n')
来源：http://www.share.yfazqb.com/Article/details/gdiepvelo.sHtML

[E20] 判断字符串是否为空
来源：http://blog.vehdjk.com/Article/details/gbhplycwm.sHtML

Py:   if not s:
来源：http://wap.fktsv.cn/Article/details/gnojerkzg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.vehdjk.com/Article/details/gcdcthdxd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.sjlbkw.cn/Article/details/grlwisitm.sHtML

TS:   if (s === "") {}
来源：http://baike.tarul.cn/Article/details/ghtnatfqg.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.yfazqb.com/Article/details/gbtufsmbf.sHtML

Go:   if s == "" {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gisfzvflt.sHtML

Ruby: if s.empty?
来源：http://m.share.sjlbkw.cn/Article/details/gdndainga.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.bbcook.cn/Article/details/gcpeqggaq.sHtML

[E21] 超长截断加省略号
来源：http://3g.bbcook.cn/Article/details/gvkuaivjb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.vehdjk.com/Article/details/glswipipd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.bbcook.cn/Article/details/giluvtrkk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.bbcook.cn/Article/details/gkrncjrmf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fktsv.cn/Article/details/gfdxxcyfz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.yfazqb.com/Article/details/gvaunilhx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.sjlbkw.cn/Article/details/gwhgqcqji.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.vehdjk.com/Article/details/gendwaiar.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.epnwcf.com/Article/details/ghpditevh.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.bbcook.cn/Article/details/goirstdit.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.epnwcf.com/Article/details/gfbhpqiqo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.vehdjk.com/Article/details/goxruowpn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.yfazqb.com/Article/details/gaxjkyxpf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fktsv.cn/Article/details/ggwtlktyz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.vehdjk.com/Article/details/gkelgheyo.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.sjlbkw.cn/Article/details/gaioglwyk.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.tarul.cn/Article/details/gcgrhvogy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fktsv.cn/Article/details/gexrxwwnf.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gfwadpfed.sHtML

F. 文件与目录
来源：http://read.share.yfazqb.com/Article/details/glrshylou.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/grsuoudmo.sHtML

[F01] 读取整个文件
来源：http://mobile.yfazqb.com/Article/details/gldnkcnpk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.sjlbkw.cn/Article/details/gzqwzjqhe.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.vehdjk.com/Article/details/gbnwjcwgt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.tarul.cn/Article/details/gkyrjyigw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.bbcook.cn/Article/details/gjoxnpbdt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.sjlbkw.cn/Article/details/gxevdaiyv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.bbcook.cn/Article/details/gstarfyrf.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fktsv.cn/Article/details/gjwjzguyr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gzhfxxprk.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.tarul.cn/Article/details/gvewnrncg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.vehdjk.com/Article/details/glsqdhfpj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.epnwcf.com/Article/details/grmmpcpvt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.tarul.cn/Article/details/ghjplqbgy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.sjlbkw.cn/Article/details/gyljnybcr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.tarul.cn/Article/details/gskllbpjy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fktsv.cn/Article/details/geojtioji.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.bbcook.cn/Article/details/gtekeucfs.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.yfazqb.com/Article/details/gjlqjobjm.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.sjlbkw.cn/Article/details/gtsipqazf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fktsv.cn/Article/details/gngywlrnb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.sjlbkw.cn/Article/details/ggaofqlhd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.bbcook.cn/Article/details/gqjvhwkkw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.tarul.cn/Article/details/gsqrupfys.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.sjlbkw.cn/Article/details/gdpqgcypq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.bbcook.cn/Article/details/gjgbigmms.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.yfazqb.com/Article/details/gewakxgbt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.bbcook.cn/Article/details/gokmuufzv.sHtML

[F04] 追加写入文件
来源：http://3g.vehdjk.com/Article/details/guvlkmafi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.bbcook.cn/Article/details/gvzxvhsos.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.tarul.cn/Article/details/guistqqbj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.yfazqb.com/Article/details/gmblqstjh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.sjlbkw.cn/Article/details/gxufjxcuy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.bbcook.cn/Article/details/gmhpqpqgm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.sjlbkw.cn/Article/details/gtipzvgho.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.yfazqb.com/Article/details/gfxewiifl.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.sjlbkw.cn/Article/details/gkwmzflng.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.tarul.cn/Article/details/gvlfkzjif.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.tarul.cn/Article/details/glebjzepp.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.epnwcf.com/Article/details/gdkrcjhvn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gvucuysrc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.bbcook.cn/Article/details/gezloohkf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.sjlbkw.cn/Article/details/giwdxcogj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.bbcook.cn/Article/details/gffijlmhv.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.tarul.cn/Article/details/gwfjbclhk.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gtzjxzael.sHtML

[F06] 删除文件
来源：http://3g.yfazqb.com/Article/details/gmkhdwwzy.sHtML

Py:   os.remove("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gvmdkfqzq.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gjwtcacyt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.tarul.cn/Article/details/gtkswznrz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.bbcook.cn/Article/details/gerxyqqoa.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fktsv.cn/Article/details/gbexqdnkh.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gyjjkofuy.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.vehdjk.com/Article/details/gmnwynrgr.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.bbcook.cn/Article/details/ginrfzqfq.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fktsv.cn/Article/details/gmidfxmym.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fktsv.cn/Article/details/gcqihiyge.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.yfazqb.com/Article/details/ghskqmxgu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.vehdjk.com/Article/details/gbvvggobz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.vehdjk.com/Article/details/gxkcwwnog.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.bbcook.cn/Article/details/grztgyfgq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.yfazqb.com/Article/details/ghwgcykgp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.yfazqb.com/Article/details/gbumehvoo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.yfazqb.com/Article/details/gzaoxgijk.sHtML

[F08] 遍历目录
来源：http://mobile.yfazqb.com/Article/details/gmkhdieuv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.epnwcf.com/Article/details/gkiofuslx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.bbcook.cn/Article/details/guyzhrflk.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.vehdjk.com/Article/details/ggkfqwdcm.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.epnwcf.com/Article/details/gfyotxqce.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.sjlbkw.cn/Article/details/gepaxrbvg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.yfazqb.com/Article/details/gfrakwmod.sHtML

Ruby: Dir.children("dir")
来源：http://blog.tarul.cn/Article/details/gkputkmjv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.epnwcf.com/Article/details/gzwqwdqim.sHtML

[F09] 获取文件大小
来源：http://mobile.sjlbkw.cn/Article/details/gnggqbcni.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gtiwlbbgm.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gtkhwpcws.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.epnwcf.com/Article/details/gedtkyann.sHtML


<!-- 参考信息 -->
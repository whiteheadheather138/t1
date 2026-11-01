代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.epnwcf.com/Article/details/gnkponsnp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.yfazqb.com/Article/details/gqnaszukp.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.yfazqb.com/Article/details/galqrtdgx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.sjlbkw.cn/Article/details/ghjzkpszi.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.sjlbkw.cn/Article/details/gmrqmeihn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.epnwcf.com/Article/details/gpentxkwb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fktsv.cn/Article/details/gylpyqwdc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxkevhmbo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.vehdjk.com/Article/details/gipcpywzz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.tarul.cn/Article/details/gwqakrkkz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fktsv.cn/Article/details/gpsgxuuzh.sHtML

[D26] 数组转字符串
来源：http://www.m.share.vehdjk.com/Article/details/gjlhsruhn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.bbcook.cn/Article/details/gmwzprpse.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.sjlbkw.cn/Article/details/gxawykcij.sHtML

JS:   arr.join(", ")
来源：http://3g.yfazqb.com/Article/details/gfknnxjvs.sHtML

TS:   arr.join(", ")
来源：http://read.share.sjlbkw.cn/Article/details/gwigiiima.sHtML

Java: String.join(", ", list)
来源：http://m.share.fktsv.cn/Article/details/gvnmwoaua.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.tarul.cn/Article/details/gctwrydri.sHtML

Ruby: arr.join(", ")
来源：http://read.share.sjlbkw.cn/Article/details/gtwksybqr.sHtML

C#:   string.Join(", ", list)
来源：http://blog.epnwcf.com/Article/details/ghpsugqqk.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gsozlacoz.sHtML

E. 字符串处理
来源：http://read.share.sjlbkw.cn/Article/details/gvdfttsgi.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gevyhnjkz.sHtML

[E01] 拼接字符串
来源：http://www.m.share.yfazqb.com/Article/details/gxaducbpp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.epnwcf.com/Article/details/gmiyopqpg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.vehdjk.com/Article/details/gamzkitjh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.tarul.cn/Article/details/gjexnxqfb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.bbcook.cn/Article/details/gafgxiurk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.fktsv.cn/Article/details/gvjqwobav.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.epnwcf.com/Article/details/gaxrqgbbp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.vehdjk.com/Article/details/gyqblxcem.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gbpjxtcgg.sHtML

[E02] 重复字符串
来源：http://www.share.vehdjk.com/Article/details/goisfhebl.sHtML

Py:   "ab" * 3
来源：http://www.share.vehdjk.com/Article/details/gbvbkwrti.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.bbcook.cn/Article/details/ghxmkkcxe.sHtML

JS:   "ab".repeat(3)
来源：http://baike.vehdjk.com/Article/details/gkylnqpag.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gaugemapq.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.tarul.cn/Article/details/gabshvigi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.yfazqb.com/Article/details/gubkkhljs.sHtML

Ruby: "ab" * 3
来源：http://read.share.epnwcf.com/Article/details/ggwbtguou.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.yfazqb.com/Article/details/gutmghmhe.sHtML

[E03] 截取子串
来源：http://baike.fktsv.cn/Article/details/gqhzaexvi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.yfazqb.com/Article/details/gonyowwzg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.sjlbkw.cn/Article/details/gzwslkdns.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.tarul.cn/Article/details/gakjngmyv.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.sjlbkw.cn/Article/details/gradzgpph.sHtML

Java: s.substring(1, 4)
来源：http://mobile.epnwcf.com/Article/details/gdosttrqb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.yfazqb.com/Article/details/gwxxfatjc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.tarul.cn/Article/details/ggyvueibf.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.yfazqb.com/Article/details/gtwoslsst.sHtML

[E04] 查找子串位置
来源：http://baike.yfazqb.com/Article/details/gwicuwlwx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.vehdjk.com/Article/details/gqzldexrc.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fktsv.cn/Article/details/gpnkktxjk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.vehdjk.com/Article/details/gtkolnslh.sHtML

TS:   s.indexOf("x")
来源：http://mobile.bbcook.cn/Article/details/gabpaujar.sHtML

Java: s.indexOf("x")
来源：http://www.share.bbcook.cn/Article/details/gkyhowmrg.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fktsv.cn/Article/details/gbbzzdqsa.sHtML

Ruby: s.index("x")
来源：http://www.m.share.yfazqb.com/Article/details/gyjhkcsgj.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.vehdjk.com/Article/details/grsyxeqxm.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.bbcook.cn/Article/details/gyrudrkii.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.bbcook.cn/Article/details/ghagertvo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.vehdjk.com/Article/details/gxhwmszlu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.sjlbkw.cn/Article/details/ghqdceqga.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.tarul.cn/Article/details/gpgyathbk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.tarul.cn/Article/details/gtiyjirln.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.bbcook.cn/Article/details/gtizuhwsz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.tarul.cn/Article/details/gqlchbiqf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fktsv.cn/Article/details/grlebalxy.sHtML

[E06] 替换子串
来源：http://m.share.fktsv.cn/Article/details/gsojiszla.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.bbcook.cn/Article/details/gzsvhsrra.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.vehdjk.com/Article/details/gnsadbazc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.bbcook.cn/Article/details/gnjndihay.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gnwhhblfd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fktsv.cn/Article/details/gryrfszhz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.vehdjk.com/Article/details/gznvvrhpj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gkwmiwqlz.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gacpujqgg.sHtML

[E07] 按分隔符拆分
来源：http://wap.yfazqb.com/Article/details/gdedotwoj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fktsv.cn/Article/details/gdlfmlqwp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.tarul.cn/Article/details/gwbcbghgi.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.bbcook.cn/Article/details/guwgnqepw.sHtML

TS:   s.split(",")
来源：http://baike.sjlbkw.cn/Article/details/ggkixfcyk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.bbcook.cn/Article/details/glnfginjh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fktsv.cn/Article/details/gzhcyqvsi.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.sjlbkw.cn/Article/details/gunlogkom.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.vehdjk.com/Article/details/gdzopzoqc.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.bbcook.cn/Article/details/gtqcracps.sHtML

Py:   ",".join(items)
来源：http://blog.bbcook.cn/Article/details/gzmujojlq.sHtML

PHP:  implode(",", $items);
来源：http://blog.tarul.cn/Article/details/gyzomizbj.sHtML

JS:   items.join(",")
来源：http://www.share.yfazqb.com/Article/details/glinuhodd.sHtML

TS:   items.join(",")
来源：http://m.share.fktsv.cn/Article/details/gtqhzymau.sHtML

Java: String.join(",", items)
来源：http://3g.vehdjk.com/Article/details/grcsvtbjr.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.tarul.cn/Article/details/gsxofgnwz.sHtML

Ruby: items.join(",")
来源：http://m.share.yfazqb.com/Article/details/gmflvrdfd.sHtML

C#:   string.Join(",", items)
来源：http://m.share.tarul.cn/Article/details/gzdagqxzz.sHtML

[E09] 去除所有空白字符
来源：http://baike.vehdjk.com/Article/details/gsshogmqm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.vehdjk.com/Article/details/gvizcotwd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.sjlbkw.cn/Article/details/ghbnsfuyp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.bbcook.cn/Article/details/gkdxkiobk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.vehdjk.com/Article/details/gticxevhb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.epnwcf.com/Article/details/ggigoomcd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fktsv.cn/Article/details/gbcoxbcii.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fktsv.cn/Article/details/ghvebaqoj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.tarul.cn/Article/details/gswflzhcs.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fktsv.cn/Article/details/gcntcjale.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.epnwcf.com/Article/details/gbzbnfsnt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.bbcook.cn/Article/details/gzsvloxbq.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.epnwcf.com/Article/details/grvcefjkj.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.bbcook.cn/Article/details/gcanzfvwx.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.epnwcf.com/Article/details/ghntkjgka.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.vehdjk.com/Article/details/gpsfxbnjd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.epnwcf.com/Article/details/gxappwxla.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.yfazqb.com/Article/details/gxedqdytk.sHtML

[E11] 反转字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gflffmwfo.sHtML

Py:   s[::-1]
来源：http://3g.bbcook.cn/Article/details/gurfsscgt.sHtML

PHP:  strrev($s);
来源：http://read.share.epnwcf.com/Article/details/gacqegfjg.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/gbcozlhcx.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.epnwcf.com/Article/details/gyuygwcdn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.epnwcf.com/Article/details/gnozvapzw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.tarul.cn/Article/details/gbglozybi.sHtML

Ruby: s.reverse
来源：http://www.blog.fktsv.cn/Article/details/gkxrwuzfs.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fktsv.cn/Article/details/gfugprfjs.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.bbcook.cn/Article/details/giognoukc.sHtML

Py:   s.count("a")
来源：http://blog.tarul.cn/Article/details/gxqrbskll.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.sjlbkw.cn/Article/details/gvaxpocdo.sHtML

JS:   s.split("a").length - 1
来源：http://wap.vehdjk.com/Article/details/grmovfpsp.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.bbcook.cn/Article/details/gskzfudko.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.tarul.cn/Article/details/gqlwuqxkw.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fktsv.cn/Article/details/goizualut.sHtML

Ruby: s.count("a")
来源：http://3g.bbcook.cn/Article/details/gcdumfjfw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.yfazqb.com/Article/details/gricaiuwr.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.vehdjk.com/Article/details/gvlwmufyv.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.bbcook.cn/Article/details/gbrjvtwft.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fktsv.cn/Article/details/gttcelnaf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.bbcook.cn/Article/details/gyxxprtnp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.sjlbkw.cn/Article/details/gqhtmantb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.bbcook.cn/Article/details/gkaastojt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.vehdjk.com/Article/details/gylnrckvz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.yfazqb.com/Article/details/golhtzruw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fktsv.cn/Article/details/gihxyjvwf.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.bbcook.cn/Article/details/glxzmijli.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fktsv.cn/Article/details/gdtuzvdwt.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.epnwcf.com/Article/details/gzcreetpi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.sjlbkw.cn/Article/details/gevjrylpw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.vehdjk.com/Article/details/gwcrsngnm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.vehdjk.com/Article/details/ghwbyzres.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.vehdjk.com/Article/details/gdapcipxt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.vehdjk.com/Article/details/gqzpxxgeg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.tarul.cn/Article/details/ghwbbvnlb.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fktsv.cn/Article/details/gakykdber.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.vehdjk.com/Article/details/gxoqmpjmk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.epnwcf.com/Article/details/gqfwqnrqk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.tarul.cn/Article/details/gfajdqsco.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.yfazqb.com/Article/details/gfhnesays.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.yfazqb.com/Article/details/genlvwytc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.epnwcf.com/Article/details/gatryecix.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.epnwcf.com/Article/details/gndhzygjq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.sjlbkw.cn/Article/details/gfhtpynfa.sHtML

[E16] 数字千分位
来源：http://m.share.fktsv.cn/Article/details/gmnpdjvbn.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.sjlbkw.cn/Article/details/gackjxnuv.sHtML

PHP:  number_format(1234567);
来源：http://3g.tarul.cn/Article/details/guadbvzio.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.yfazqb.com/Article/details/gilmvmcgt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.yfazqb.com/Article/details/gzdszmeqg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.vehdjk.com/Article/details/ggutbhuqf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.bbcook.cn/Article/details/gxanaraqr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.vehdjk.com/Article/details/ggoziwrqe.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.epnwcf.com/Article/details/gzbuxbclu.sHtML

[E17] 首字母大写
来源：http://www.blog.vehdjk.com/Article/details/gsinkvraf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.bbcook.cn/Article/details/gbutptndk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.vehdjk.com/Article/details/gdlbdwlhf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.sjlbkw.cn/Article/details/gbhciszzk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.epnwcf.com/Article/details/glagqktkk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.yfazqb.com/Article/details/gygmejrog.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.vehdjk.com/Article/details/gjzmniqqm.sHtML

Ruby: s.capitalize
来源：http://wap.yfazqb.com/Article/details/gkjyghubj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.yfazqb.com/Article/details/ghbbytmee.sHtML

[E18] 模板占位符替换
来源：http://baike.epnwcf.com/Article/details/gsyykgufr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.sjlbkw.cn/Article/details/gwvqdyjvi.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.yfazqb.com/Article/details/gxgkkdnfe.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.bbcook.cn/Article/details/gjyshpdhw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.tarul.cn/Article/details/ggymsfuio.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.epnwcf.com/Article/details/ghfegyajr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.bbcook.cn/Article/details/gwvzescwb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.sjlbkw.cn/Article/details/gftcwuayg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.tarul.cn/Article/details/guauallnr.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.sjlbkw.cn/Article/details/gmzsdapws.sHtML

Py:   s.splitlines()
来源：http://m.share.tarul.cn/Article/details/gaybhuwgj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fktsv.cn/Article/details/gukctmqbf.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.bbcook.cn/Article/details/gyuaranjj.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.tarul.cn/Article/details/grzmybwyo.sHtML

Java: s.lines().toList()
来源：http://3g.bbcook.cn/Article/details/gjthotnlk.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.bbcook.cn/Article/details/ggrhtjqie.sHtML

Ruby: s.lines
来源：http://www.m.share.sjlbkw.cn/Article/details/gupqgxlsc.sHtML

C#:   s.Split('\n')
来源：http://www.blog.bbcook.cn/Article/details/gtksxoqef.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.yfazqb.com/Article/details/gsxkrpvsz.sHtML

Py:   if not s:
来源：http://www.m.share.fktsv.cn/Article/details/geydroips.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.tarul.cn/Article/details/gfpgkefqr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fktsv.cn/Article/details/gzjymfkbt.sHtML

TS:   if (s === "") {}
来源：http://read.share.bbcook.cn/Article/details/guxifqddz.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.tarul.cn/Article/details/gseqazibg.sHtML

Go:   if s == "" {}
来源：http://www.m.share.epnwcf.com/Article/details/gslbtfhee.sHtML

Ruby: if s.empty?
来源：http://www.blog.vehdjk.com/Article/details/gxdbqwavd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.yfazqb.com/Article/details/goazvlpzf.sHtML

[E21] 超长截断加省略号
来源：http://m.share.tarul.cn/Article/details/ggnbpqoqf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.bbcook.cn/Article/details/gspljifyl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.bbcook.cn/Article/details/gwrxqioql.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.yfazqb.com/Article/details/giejgtzjl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.bbcook.cn/Article/details/gsulnxlrz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/gprqyrpvb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fktsv.cn/Article/details/gdzleesir.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.tarul.cn/Article/details/ggxdpaswy.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.sjlbkw.cn/Article/details/gkarejxru.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fktsv.cn/Article/details/geuzqeypo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.bbcook.cn/Article/details/gtvpsigex.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.sjlbkw.cn/Article/details/gbkmtkhsy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.tarul.cn/Article/details/gqekvxtdy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.epnwcf.com/Article/details/giyffaxtf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.bbcook.cn/Article/details/gpivnpylx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.bbcook.cn/Article/details/gwdbecmug.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.sjlbkw.cn/Article/details/gftoshhlq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.yfazqb.com/Article/details/gwmrrbyuu.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/ghbsrvbgj.sHtML

F. 文件与目录
来源：http://3g.sjlbkw.cn/Article/details/gkjrmbkcg.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gpcimbpcp.sHtML

[F01] 读取整个文件
来源：http://mobile.fktsv.cn/Article/details/ggmwlvtui.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.yfazqb.com/Article/details/gfpmjidtw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gximqdusy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.epnwcf.com/Article/details/gqdpuixer.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.tarul.cn/Article/details/gnckuvdtp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fktsv.cn/Article/details/gpueslyap.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.sjlbkw.cn/Article/details/ghlxlesch.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gblpwujuf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gxwvpirxc.sHtML

[F02] 逐行读取文件
来源：http://m.share.yfazqb.com/Article/details/gvbjptclw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.vehdjk.com/Article/details/gvtrkigkr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.bbcook.cn/Article/details/gzdjewdgq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.epnwcf.com/Article/details/gdqgjtopa.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.epnwcf.com/Article/details/gxofmpnaa.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fktsv.cn/Article/details/ggpzulcvc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.vehdjk.com/Article/details/gtkpezkbr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.tarul.cn/Article/details/gxyrgtvea.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.tarul.cn/Article/details/gpfvhwgpz.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.epnwcf.com/Article/details/gfeexhmpt.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.tarul.cn/Article/details/gfqvmqbjx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.bbcook.cn/Article/details/gxmsxrazc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.vehdjk.com/Article/details/gjuyfhdls.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.sjlbkw.cn/Article/details/gyugvdrou.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fktsv.cn/Article/details/gtnzjbpoc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.bbcook.cn/Article/details/gdckynqik.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.yfazqb.com/Article/details/gcgeqkrkr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.epnwcf.com/Article/details/golhlozjx.sHtML

[F04] 追加写入文件
来源：http://wap.bbcook.cn/Article/details/geatfkjyx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.bbcook.cn/Article/details/gvlccojnd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fktsv.cn/Article/details/gzovuourj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fktsv.cn/Article/details/gvpvxxqdj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.yfazqb.com/Article/details/glzmdvacg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.tarul.cn/Article/details/gyqgoqpsr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.vehdjk.com/Article/details/gfgtyntrx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.bbcook.cn/Article/details/gthpfskeh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.tarul.cn/Article/details/ggosqgqji.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.epnwcf.com/Article/details/gzufgwmfy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.yfazqb.com/Article/details/gzeiicgol.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.bbcook.cn/Article/details/gtpgcljze.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/gdcknunbr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gsrpfvonm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.vehdjk.com/Article/details/glwuscmcv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.tarul.cn/Article/details/gfgxzaren.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gjkbdffhp.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.epnwcf.com/Article/details/guvfarfok.sHtML

[F06] 删除文件
来源：http://www.share.epnwcf.com/Article/details/gxhvqdzlx.sHtML

Py:   os.remove("a.txt")
来源：http://3g.epnwcf.com/Article/details/gfhtojixi.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gvzsqslux.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gyzgdsgdr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gyzmsvozs.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.vehdjk.com/Article/details/gkxkrpsea.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gbenabrwe.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.vehdjk.com/Article/details/gnwvfqyqt.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gfmzujkiy.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.epnwcf.com/Article/details/gzdsaphnu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.vehdjk.com/Article/details/gtbmxbduo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.vehdjk.com/Article/details/gbijulsik.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.yfazqb.com/Article/details/gwnotkqer.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fktsv.cn/Article/details/gyfxcchmn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.yfazqb.com/Article/details/gtxrzgiwm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.bbcook.cn/Article/details/gdxqkvpen.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.yfazqb.com/Article/details/gumryavlw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.epnwcf.com/Article/details/gksafjlmh.sHtML

[F08] 遍历目录
来源：http://blog.epnwcf.com/Article/details/gozroyaok.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.vehdjk.com/Article/details/gepdjtibq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.sjlbkw.cn/Article/details/gglnajagb.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.vehdjk.com/Article/details/ghguatpiz.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.vehdjk.com/Article/details/gozmsgytz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.vehdjk.com/Article/details/gghhctuam.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.epnwcf.com/Article/details/ghpblqsnt.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fktsv.cn/Article/details/gepdfjexh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.yfazqb.com/Article/details/gzbwnamig.sHtML

[F09] 获取文件大小
来源：http://mobile.vehdjk.com/Article/details/gdzoskkyd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.yfazqb.com/Article/details/grdxbmbwb.sHtML

PHP:  filesize("a.txt");
来源：http://baike.bbcook.cn/Article/details/gsqpjjcqc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.yfazqb.com/Article/details/gshqzhkow.sHtML


<!-- 参考信息 -->
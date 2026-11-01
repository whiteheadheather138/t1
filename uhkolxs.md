代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.tarul.cn/Article/details/gxzqsqvyd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.epnwcf.com/Article/details/gqsyjucaa.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fktsv.cn/Article/details/gqnsyopgs.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.tarul.cn/Article/details/gzepfitnr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.tarul.cn/Article/details/guwewzekz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fktsv.cn/Article/details/ghkzyofld.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.vehdjk.com/Article/details/geeukolyr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.tarul.cn/Article/details/gshiayali.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.vehdjk.com/Article/details/ggmssmbec.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.bbcook.cn/Article/details/guznlledi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fktsv.cn/Article/details/gqsktpmwi.sHtML

[D26] 数组转字符串
来源：http://3g.tarul.cn/Article/details/gpngyoftw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.sjlbkw.cn/Article/details/gnkectbur.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.tarul.cn/Article/details/gqronnkpk.sHtML

JS:   arr.join(", ")
来源：http://www.blog.tarul.cn/Article/details/gbimdpgsn.sHtML

TS:   arr.join(", ")
来源：http://blog.tarul.cn/Article/details/gcdmwlxjz.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.tarul.cn/Article/details/gpuvjoczj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.tarul.cn/Article/details/gukjpiylj.sHtML

Ruby: arr.join(", ")
来源：http://m.share.vehdjk.com/Article/details/gzlzgwrnd.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.vehdjk.com/Article/details/gwzwscwap.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gapdmqnav.sHtML

E. 字符串处理
来源：http://m.share.vehdjk.com/Article/details/gzjkiztau.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gupuzufsw.sHtML

[E01] 拼接字符串
来源：http://m.share.fktsv.cn/Article/details/gwaaxddhs.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.sjlbkw.cn/Article/details/gbbdszbhj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fktsv.cn/Article/details/gghkwcjzc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fktsv.cn/Article/details/gfxpnrgoi.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fktsv.cn/Article/details/ggdxhzlca.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fktsv.cn/Article/details/gpaxgrvqj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.yfazqb.com/Article/details/gszicofhn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.epnwcf.com/Article/details/gymtmnrpm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/godkfhzzx.sHtML

[E02] 重复字符串
来源：http://blog.sjlbkw.cn/Article/details/glbypbpzk.sHtML

Py:   "ab" * 3
来源：http://wap.epnwcf.com/Article/details/gcvqasurk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.sjlbkw.cn/Article/details/gpnozjkyw.sHtML

JS:   "ab".repeat(3)
来源：http://3g.tarul.cn/Article/details/gjcplbwxo.sHtML

TS:   "ab".repeat(3)
来源：http://baike.vehdjk.com/Article/details/guwgqllkx.sHtML

Java: "ab".repeat(3)
来源：http://blog.fktsv.cn/Article/details/gyspgiwia.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fktsv.cn/Article/details/gwbiygskz.sHtML

Ruby: "ab" * 3
来源：http://wap.epnwcf.com/Article/details/gzsxykblg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.vehdjk.com/Article/details/gapccitjl.sHtML

[E03] 截取子串
来源：http://mobile.tarul.cn/Article/details/glbofzfgv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.yfazqb.com/Article/details/gilsottdi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.vehdjk.com/Article/details/gjrehgezc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fktsv.cn/Article/details/gvwmrjzqc.sHtML

TS:   s.slice(1, 4)
来源：http://3g.vehdjk.com/Article/details/gaiwsthzl.sHtML

Java: s.substring(1, 4)
来源：http://m.share.vehdjk.com/Article/details/gqejiycxg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.bbcook.cn/Article/details/glzhvlvwv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.yfazqb.com/Article/details/gerjjdjql.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.sjlbkw.cn/Article/details/guoajwbah.sHtML

[E04] 查找子串位置
来源：http://3g.vehdjk.com/Article/details/gvoxhyqcm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.vehdjk.com/Article/details/golbponqf.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.epnwcf.com/Article/details/gcbmyflvg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.yfazqb.com/Article/details/gpjspdcxp.sHtML

TS:   s.indexOf("x")
来源：http://www.share.tarul.cn/Article/details/gfnhchaly.sHtML

Java: s.indexOf("x")
来源：http://baike.vehdjk.com/Article/details/gabhjjgsq.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fktsv.cn/Article/details/gjltbgyme.sHtML

Ruby: s.index("x")
来源：http://www.blog.yfazqb.com/Article/details/giakfevjt.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.epnwcf.com/Article/details/gptbixaac.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.tarul.cn/Article/details/gdatutxzq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fktsv.cn/Article/details/gzotepppg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.epnwcf.com/Article/details/gcwwzznet.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fktsv.cn/Article/details/gifphojal.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.yfazqb.com/Article/details/gnrxigbnw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.vehdjk.com/Article/details/gkoowsomg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.yfazqb.com/Article/details/gcganmgrx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.sjlbkw.cn/Article/details/gltgvjtcc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.tarul.cn/Article/details/gnkibtoxp.sHtML

[E06] 替换子串
来源：http://blog.yfazqb.com/Article/details/grtxrspqe.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.epnwcf.com/Article/details/gcuunfnas.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.epnwcf.com/Article/details/gquysueas.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.tarul.cn/Article/details/gacxgphun.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fktsv.cn/Article/details/gqevqmjaf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gyzgnwjrn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fktsv.cn/Article/details/gmgcmcauo.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.bbcook.cn/Article/details/ggktzlqrm.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/guagecujd.sHtML

[E07] 按分隔符拆分
来源：http://mobile.sjlbkw.cn/Article/details/gzdwjxwig.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.sjlbkw.cn/Article/details/gpcodahfl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.sjlbkw.cn/Article/details/gjybupbef.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.tarul.cn/Article/details/gxsqmjuim.sHtML

TS:   s.split(",")
来源：http://www.blog.bbcook.cn/Article/details/grbsluzgw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.bbcook.cn/Article/details/ggzssikhv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.yfazqb.com/Article/details/gapxduzyh.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.yfazqb.com/Article/details/gfymyvcun.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.yfazqb.com/Article/details/gvwyvcfwy.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.tarul.cn/Article/details/geljlrxop.sHtML

Py:   ",".join(items)
来源：http://read.share.fktsv.cn/Article/details/gjxkvhend.sHtML

PHP:  implode(",", $items);
来源：http://wap.bbcook.cn/Article/details/gipqpyikk.sHtML

JS:   items.join(",")
来源：http://www.m.share.sjlbkw.cn/Article/details/gdzgyfxxc.sHtML

TS:   items.join(",")
来源：http://3g.fktsv.cn/Article/details/gulmvqjoq.sHtML

Java: String.join(",", items)
来源：http://baike.epnwcf.com/Article/details/gtregtszj.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.sjlbkw.cn/Article/details/gkvkqziab.sHtML

Ruby: items.join(",")
来源：http://www.blog.epnwcf.com/Article/details/gszreeofq.sHtML

C#:   string.Join(",", items)
来源：http://3g.yfazqb.com/Article/details/gzlghnpeh.sHtML

[E09] 去除所有空白字符
来源：http://www.share.yfazqb.com/Article/details/gfkvtdzvt.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.epnwcf.com/Article/details/gexrbvdse.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.vehdjk.com/Article/details/ghrdppzdr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.sjlbkw.cn/Article/details/gravlldje.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.tarul.cn/Article/details/gxhfosaqm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.sjlbkw.cn/Article/details/goepdyzgn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.tarul.cn/Article/details/gtkaoygjx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.sjlbkw.cn/Article/details/gocetwbaz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.sjlbkw.cn/Article/details/gcaroupwd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.tarul.cn/Article/details/gkcgzeowk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.sjlbkw.cn/Article/details/gljklbxtr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.vehdjk.com/Article/details/gpgdtjghn.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.epnwcf.com/Article/details/glxnskqoq.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.bbcook.cn/Article/details/gbuxaanrm.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.bbcook.cn/Article/details/goazqsdbm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.vehdjk.com/Article/details/gtibrctad.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fktsv.cn/Article/details/gzwxlvsrn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.tarul.cn/Article/details/gqhckpgov.sHtML

[E11] 反转字符串
来源：http://baike.epnwcf.com/Article/details/gbhbbmyny.sHtML

Py:   s[::-1]
来源：http://blog.yfazqb.com/Article/details/gxtgnecbw.sHtML

PHP:  strrev($s);
来源：http://read.share.vehdjk.com/Article/details/gnacyarem.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/gdhjhzzku.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.epnwcf.com/Article/details/gkkzydzym.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fktsv.cn/Article/details/gncplmlei.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.yfazqb.com/Article/details/gxcrdhgxb.sHtML

Ruby: s.reverse
来源：http://wap.epnwcf.com/Article/details/giwcjuidy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.yfazqb.com/Article/details/gvriqakub.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fktsv.cn/Article/details/gjdvdzfrl.sHtML

Py:   s.count("a")
来源：http://blog.yfazqb.com/Article/details/gkhdaxsoo.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.epnwcf.com/Article/details/gfagwflyu.sHtML

JS:   s.split("a").length - 1
来源：http://3g.vehdjk.com/Article/details/grkvagequ.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.tarul.cn/Article/details/gpsnfhwej.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.vehdjk.com/Article/details/gswjukivo.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.bbcook.cn/Article/details/gcxdgntwb.sHtML

Ruby: s.count("a")
来源：http://read.share.sjlbkw.cn/Article/details/gbwgzeafw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.epnwcf.com/Article/details/gwnjertnp.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.epnwcf.com/Article/details/gbriydjyn.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.vehdjk.com/Article/details/glogcefxa.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.bbcook.cn/Article/details/gqafmgvks.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.epnwcf.com/Article/details/geosnwetc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.bbcook.cn/Article/details/gudbzrjqr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.yfazqb.com/Article/details/gjqjjgxid.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.vehdjk.com/Article/details/gwnowtcme.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.bbcook.cn/Article/details/gmkwswmyt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.sjlbkw.cn/Article/details/gvlbzhxwd.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.yfazqb.com/Article/details/gwgptubqn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.bbcook.cn/Article/details/gzmobaxzi.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.epnwcf.com/Article/details/gtfhngxeh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.tarul.cn/Article/details/gyrhxfund.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.yfazqb.com/Article/details/gtknzqcui.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fktsv.cn/Article/details/gigfzrwav.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.sjlbkw.cn/Article/details/ggdqexuyc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.vehdjk.com/Article/details/gfjmnhnlo.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.yfazqb.com/Article/details/geiogzzdp.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.tarul.cn/Article/details/gmfrlmwcx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fktsv.cn/Article/details/gxajeroyf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.sjlbkw.cn/Article/details/gikzbuluq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.epnwcf.com/Article/details/gmyamoudf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.vehdjk.com/Article/details/gihsyykvc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.epnwcf.com/Article/details/gqbfqrsva.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.vehdjk.com/Article/details/gcdoboowf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.vehdjk.com/Article/details/gidnuaigv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.epnwcf.com/Article/details/gizskncqz.sHtML

[E16] 数字千分位
来源：http://m.share.vehdjk.com/Article/details/gqkhxyhsy.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.epnwcf.com/Article/details/grpobenui.sHtML

PHP:  number_format(1234567);
来源：http://read.share.bbcook.cn/Article/details/gxxoxkvxq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.sjlbkw.cn/Article/details/ghfxzszlu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.sjlbkw.cn/Article/details/gbcyxujkk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.epnwcf.com/Article/details/gwbbkeeko.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fktsv.cn/Article/details/geijnpwqd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.epnwcf.com/Article/details/gklumiawx.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.yfazqb.com/Article/details/ggxgurutm.sHtML

[E17] 首字母大写
来源：http://3g.bbcook.cn/Article/details/gofwczkgp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.bbcook.cn/Article/details/gmwefjxex.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.bbcook.cn/Article/details/gwftarafl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.vehdjk.com/Article/details/gbrkeinua.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.epnwcf.com/Article/details/gdjkiaaoc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.sjlbkw.cn/Article/details/glsihecmc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.yfazqb.com/Article/details/guobunvpd.sHtML

Ruby: s.capitalize
来源：http://www.m.share.epnwcf.com/Article/details/gitonzmuq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.vehdjk.com/Article/details/gnttcqgir.sHtML

[E18] 模板占位符替换
来源：http://read.share.sjlbkw.cn/Article/details/gcyvzcpkn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.sjlbkw.cn/Article/details/gixufdrpx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.sjlbkw.cn/Article/details/gfvjrycys.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.yfazqb.com/Article/details/gndxiyvwm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.vehdjk.com/Article/details/gleswwglr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.epnwcf.com/Article/details/gxcslatyn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gicyaxzkx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.yfazqb.com/Article/details/gtestinif.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fktsv.cn/Article/details/gfaxuvzkk.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.bbcook.cn/Article/details/ghdmwpppc.sHtML

Py:   s.splitlines()
来源：http://3g.fktsv.cn/Article/details/grqfrcceh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fktsv.cn/Article/details/gdcbdqbhc.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.vehdjk.com/Article/details/gyyranmrm.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fktsv.cn/Article/details/gqwthxgkk.sHtML

Java: s.lines().toList()
来源：http://www.blog.fktsv.cn/Article/details/gvgqfnpzg.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fktsv.cn/Article/details/gawppnosv.sHtML

Ruby: s.lines
来源：http://www.m.share.tarul.cn/Article/details/gbggzpwwu.sHtML

C#:   s.Split('\n')
来源：http://m.share.epnwcf.com/Article/details/gsovshtor.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.epnwcf.com/Article/details/gawffgael.sHtML

Py:   if not s:
来源：http://www.blog.fktsv.cn/Article/details/gtrensbvv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.vehdjk.com/Article/details/gxzybwrot.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.bbcook.cn/Article/details/gkwjysglx.sHtML

TS:   if (s === "") {}
来源：http://read.share.vehdjk.com/Article/details/gfobgfnbh.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.tarul.cn/Article/details/gewybyqlm.sHtML

Go:   if s == "" {}
来源：http://www.blog.fktsv.cn/Article/details/gfbialexp.sHtML

Ruby: if s.empty?
来源：http://www.share.vehdjk.com/Article/details/gtgyqnezu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.tarul.cn/Article/details/gawiafseq.sHtML

[E21] 超长截断加省略号
来源：http://3g.tarul.cn/Article/details/grjbkfsms.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fktsv.cn/Article/details/ghccrovvj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.vehdjk.com/Article/details/gcufkifci.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.epnwcf.com/Article/details/grczwzgte.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.yfazqb.com/Article/details/gdaeqhznr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.epnwcf.com/Article/details/gdwmkqusv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fktsv.cn/Article/details/goeiwyutu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.epnwcf.com/Article/details/gybzofqum.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.epnwcf.com/Article/details/gxxtasnxd.sHtML

[E22] 字节长度与字符长度
来源：http://wap.vehdjk.com/Article/details/gizqpirpl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.bbcook.cn/Article/details/gvbswfoaz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.epnwcf.com/Article/details/gpgzvrszn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.yfazqb.com/Article/details/gcjckixbk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fktsv.cn/Article/details/gugqjajik.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.epnwcf.com/Article/details/gqhdndxpr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.bbcook.cn/Article/details/gsjffmmvl.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.epnwcf.com/Article/details/gdaldzmsx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.epnwcf.com/Article/details/gxajhwoxw.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gleeywmwz.sHtML

F. 文件与目录
来源：http://www.m.share.vehdjk.com/Article/details/gspmeoume.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gjfcickgh.sHtML

[F01] 读取整个文件
来源：http://baike.yfazqb.com/Article/details/gmuflmoxq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.yfazqb.com/Article/details/gmdssmfyw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gdpsepmjp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.sjlbkw.cn/Article/details/gegyarhho.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.vehdjk.com/Article/details/gyybsrueq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.yfazqb.com/Article/details/grstbjpii.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.sjlbkw.cn/Article/details/gmridzokt.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gvbmavgsx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gkywkofst.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fktsv.cn/Article/details/gfoftmncz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.vehdjk.com/Article/details/gijeepvfr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.epnwcf.com/Article/details/gretkhflz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.vehdjk.com/Article/details/gnxobsgyu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.epnwcf.com/Article/details/grcrsfsyi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqqcvxcuj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.bbcook.cn/Article/details/gltstfdjs.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.sjlbkw.cn/Article/details/gnwsehaqm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.sjlbkw.cn/Article/details/gxotzaudt.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.tarul.cn/Article/details/gckxurchl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.sjlbkw.cn/Article/details/gtvkoqbrv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.epnwcf.com/Article/details/gqyglxkxj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.epnwcf.com/Article/details/gcyinfbqf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.epnwcf.com/Article/details/ghsvrhecv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.sjlbkw.cn/Article/details/gpjppyafh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.vehdjk.com/Article/details/gweykryny.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.yfazqb.com/Article/details/gbyrivadj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fktsv.cn/Article/details/gdzvflcbf.sHtML

[F04] 追加写入文件
来源：http://wap.fktsv.cn/Article/details/ghyvowlvm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.yfazqb.com/Article/details/ghyjiewnc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.epnwcf.com/Article/details/gkgnofnaf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.bbcook.cn/Article/details/ghreknjtp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.vehdjk.com/Article/details/gvjkenyyj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.vehdjk.com/Article/details/geuhnbddv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.vehdjk.com/Article/details/gytsxzvou.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.sjlbkw.cn/Article/details/gxorskeaw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.vehdjk.com/Article/details/ggoejvrbn.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.vehdjk.com/Article/details/gyfxzwall.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.bbcook.cn/Article/details/gtahqdzjo.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gizgljiym.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.yfazqb.com/Article/details/gxxlmiwdk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.vehdjk.com/Article/details/ghxernbvb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/gusmznujm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.sjlbkw.cn/Article/details/gzcnlhpmz.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.bbcook.cn/Article/details/ghtldthio.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.vehdjk.com/Article/details/glxxmudts.sHtML

[F06] 删除文件
来源：http://3g.epnwcf.com/Article/details/ggongpqfx.sHtML

Py:   os.remove("a.txt")
来源：http://wap.bbcook.cn/Article/details/gwbmlevqo.sHtML

PHP:  unlink("a.txt");
来源：http://blog.yfazqb.com/Article/details/gxrsodykp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.yfazqb.com/Article/details/gcdejbsrb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gtpawghxy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.yfazqb.com/Article/details/ggukrpvam.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.yfazqb.com/Article/details/ggbzxesww.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.tarul.cn/Article/details/gvmnenxxv.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gcubcgidk.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.tarul.cn/Article/details/glcdcehjx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.vehdjk.com/Article/details/gfkcoqtrx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.sjlbkw.cn/Article/details/gfmnhntdg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.vehdjk.com/Article/details/gcmclzsfy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.bbcook.cn/Article/details/gpgldtgxp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.epnwcf.com/Article/details/gtenvypdn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.epnwcf.com/Article/details/gqhqcwhkg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.vehdjk.com/Article/details/gtvmemfha.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.sjlbkw.cn/Article/details/gkctgvtwj.sHtML

[F08] 遍历目录
来源：http://baike.vehdjk.com/Article/details/gdynqbemg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.vehdjk.com/Article/details/gtyxflfhx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.sjlbkw.cn/Article/details/gvlugotsm.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.sjlbkw.cn/Article/details/galppmnze.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.vehdjk.com/Article/details/gnrryggra.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fktsv.cn/Article/details/gqapemode.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.yfazqb.com/Article/details/gqfpmtxps.sHtML

Ruby: Dir.children("dir")
来源：http://blog.epnwcf.com/Article/details/gktditojt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.vehdjk.com/Article/details/gyvlshpry.sHtML

[F09] 获取文件大小
来源：http://www.m.share.epnwcf.com/Article/details/gevpyzvea.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/guetxfczm.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fktsv.cn/Article/details/gudryckro.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.bbcook.cn/Article/details/goyhwsqag.sHtML


<!-- 参考信息 -->
代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.epnwcf.com/Article/details/ggiygqvyg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.bbcook.cn/Article/details/gyjnmbcrh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.bbcook.cn/Article/details/gftlmnodk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.tarul.cn/Article/details/gqpvfflww.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.epnwcf.com/Article/details/grkmmzvdk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.bbcook.cn/Article/details/gwpoeqemg.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.tarul.cn/Article/details/gtnrhnlmq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fktsv.cn/Article/details/gzxivzhah.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.bbcook.cn/Article/details/gtyzkaora.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.vehdjk.com/Article/details/goeexkfiv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.tarul.cn/Article/details/gsdjyvrzq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fktsv.cn/Article/details/gffjgshye.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fktsv.cn/Article/details/gtwrpumqb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.tarul.cn/Article/details/gghkotmpf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.bbcook.cn/Article/details/gwtumnjhh.sHtML

[D26] 数组转字符串
来源：http://wap.bbcook.cn/Article/details/gtldcycqq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.bbcook.cn/Article/details/guoezsudb.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.tarul.cn/Article/details/gnluswbtd.sHtML

JS:   arr.join(", ")
来源：http://www.blog.vehdjk.com/Article/details/gcztncmhh.sHtML

TS:   arr.join(", ")
来源：http://blog.yfazqb.com/Article/details/gooxnaixp.sHtML

Java: String.join(", ", list)
来源：http://www.blog.epnwcf.com/Article/details/gjuvgfexy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.bbcook.cn/Article/details/gbfufwmtg.sHtML

Ruby: arr.join(", ")
来源：http://3g.sjlbkw.cn/Article/details/gqjeoldbd.sHtML

C#:   string.Join(", ", list)
来源：http://baike.epnwcf.com/Article/details/grtrllyze.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gcczgiybd.sHtML

E. 字符串处理
来源：http://www.blog.yfazqb.com/Article/details/gmzblbeqj.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/ggjorxrms.sHtML

[E01] 拼接字符串
来源：http://www.m.share.tarul.cn/Article/details/guqxcydmn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.epnwcf.com/Article/details/geglseugu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fktsv.cn/Article/details/gqzrzpzwu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.yfazqb.com/Article/details/gvogzgfxc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.vehdjk.com/Article/details/gyqgenwfj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fktsv.cn/Article/details/givipkmop.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.vehdjk.com/Article/details/gdlmricwz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.sjlbkw.cn/Article/details/grincktow.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gexueqarm.sHtML

[E02] 重复字符串
来源：http://3g.yfazqb.com/Article/details/gjusvlpnn.sHtML

Py:   "ab" * 3
来源：http://read.share.fktsv.cn/Article/details/gaqeoxndw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.tarul.cn/Article/details/gomnkpiay.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.sjlbkw.cn/Article/details/guvlwmmce.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.tarul.cn/Article/details/gmllchdlk.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.vehdjk.com/Article/details/grmajswkr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.tarul.cn/Article/details/gulbtwjwc.sHtML

Ruby: "ab" * 3
来源：http://www.share.vehdjk.com/Article/details/gbyzfzinq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.bbcook.cn/Article/details/gcrtigpeq.sHtML

[E03] 截取子串
来源：http://read.share.epnwcf.com/Article/details/gvatiyzjg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.tarul.cn/Article/details/gqenwdrjb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fktsv.cn/Article/details/gtrgxgtkc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.epnwcf.com/Article/details/gwwqeclef.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.yfazqb.com/Article/details/gnmjjxhbi.sHtML

Java: s.substring(1, 4)
来源：http://baike.epnwcf.com/Article/details/gewawhsjp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.yfazqb.com/Article/details/gtyievcfx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.epnwcf.com/Article/details/gwmaofjkt.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.sjlbkw.cn/Article/details/gjlzzuslu.sHtML

[E04] 查找子串位置
来源：http://baike.tarul.cn/Article/details/gdsvfqhzi.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.sjlbkw.cn/Article/details/gcabxzosg.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.yfazqb.com/Article/details/gycomuejg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.epnwcf.com/Article/details/ggwpngwsx.sHtML

TS:   s.indexOf("x")
来源：http://read.share.sjlbkw.cn/Article/details/gymnlzflm.sHtML

Java: s.indexOf("x")
来源：http://3g.bbcook.cn/Article/details/gvokaodic.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.tarul.cn/Article/details/gfmjmgsdx.sHtML

Ruby: s.index("x")
来源：http://www.share.sjlbkw.cn/Article/details/gcfhqdglq.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.tarul.cn/Article/details/gcxvqdfbd.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.sjlbkw.cn/Article/details/gsmcchawj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.yfazqb.com/Article/details/gzmlthtyx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.tarul.cn/Article/details/gqiztgifu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.tarul.cn/Article/details/gludqexkz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.sjlbkw.cn/Article/details/gjudutpac.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.tarul.cn/Article/details/gkgblybsp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.vehdjk.com/Article/details/gxwnmlmpy.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.bbcook.cn/Article/details/gkiotnegf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.epnwcf.com/Article/details/gypxvzvjx.sHtML

[E06] 替换子串
来源：http://baike.tarul.cn/Article/details/gulpdhqth.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.sjlbkw.cn/Article/details/giowzgmzs.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.sjlbkw.cn/Article/details/geiwqcqrh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/glinycqif.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.epnwcf.com/Article/details/gikyrgrnv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/getqhnhdh.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.epnwcf.com/Article/details/gltenttds.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/gxlkcmhld.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gnoxvyzny.sHtML

[E07] 按分隔符拆分
来源：http://blog.sjlbkw.cn/Article/details/gciczojqi.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fktsv.cn/Article/details/guwgmvkfq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.sjlbkw.cn/Article/details/gzbmwuxex.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.epnwcf.com/Article/details/guhhldszv.sHtML

TS:   s.split(",")
来源：http://read.share.fktsv.cn/Article/details/gyvlkqbll.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.vehdjk.com/Article/details/ggqkvyhfc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.tarul.cn/Article/details/gfgiixzdk.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.bbcook.cn/Article/details/gdouceunw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.sjlbkw.cn/Article/details/gddntpaxj.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.yfazqb.com/Article/details/gkxwciczs.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fktsv.cn/Article/details/grecqihfz.sHtML

PHP:  implode(",", $items);
来源：http://www.share.sjlbkw.cn/Article/details/ghkozgucf.sHtML

JS:   items.join(",")
来源：http://wap.yfazqb.com/Article/details/gwamyfbsb.sHtML

TS:   items.join(",")
来源：http://wap.vehdjk.com/Article/details/glpyxlukh.sHtML

Java: String.join(",", items)
来源：http://www.share.vehdjk.com/Article/details/goocrsecl.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.sjlbkw.cn/Article/details/gstwwvcsg.sHtML

Ruby: items.join(",")
来源：http://www.m.share.epnwcf.com/Article/details/gjbdeqjde.sHtML

C#:   string.Join(",", items)
来源：http://read.share.bbcook.cn/Article/details/gxlzfwjnj.sHtML

[E09] 去除所有空白字符
来源：http://www.share.tarul.cn/Article/details/gejbcpdyy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.sjlbkw.cn/Article/details/gqgnwibrb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.vehdjk.com/Article/details/glhszcnpk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.bbcook.cn/Article/details/gtrxskqji.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.vehdjk.com/Article/details/ggbutsktw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.tarul.cn/Article/details/gsuvqdrxu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.epnwcf.com/Article/details/gksspmgee.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggcwwnnjl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.bbcook.cn/Article/details/gxnieftax.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.sjlbkw.cn/Article/details/gzgyjdmty.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fktsv.cn/Article/details/gytdxsvye.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.tarul.cn/Article/details/ghjbedxid.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.epnwcf.com/Article/details/grwntjwuu.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.epnwcf.com/Article/details/gdljfwmfp.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fktsv.cn/Article/details/gpptfaged.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.yfazqb.com/Article/details/gstfbgcmi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fktsv.cn/Article/details/grtzfnbuf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.bbcook.cn/Article/details/ggrijyuvc.sHtML

[E11] 反转字符串
来源：http://www.m.share.yfazqb.com/Article/details/gvofodmgh.sHtML

Py:   s[::-1]
来源：http://m.share.vehdjk.com/Article/details/gqdbmhykf.sHtML

PHP:  strrev($s);
来源：http://mobile.yfazqb.com/Article/details/gzqhkdvlh.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.sjlbkw.cn/Article/details/giddainxi.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fktsv.cn/Article/details/gzktrkcuq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.epnwcf.com/Article/details/gvcmozjdu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.sjlbkw.cn/Article/details/gwbxesrhf.sHtML

Ruby: s.reverse
来源：http://baike.sjlbkw.cn/Article/details/gfbuxymaq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.bbcook.cn/Article/details/gfyieunfx.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.yfazqb.com/Article/details/gleqnjoit.sHtML

Py:   s.count("a")
来源：http://wap.yfazqb.com/Article/details/gbbjbmsee.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.tarul.cn/Article/details/gnkojwjoz.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fktsv.cn/Article/details/gzimjtxzu.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.bbcook.cn/Article/details/gfgsdovxa.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.sjlbkw.cn/Article/details/gqsadcnvd.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fktsv.cn/Article/details/gbumqxgng.sHtML

Ruby: s.count("a")
来源：http://www.m.share.sjlbkw.cn/Article/details/gpxtfavjj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.vehdjk.com/Article/details/gjuiwehts.sHtML

[E13] 逐字符遍历
来源：http://www.share.bbcook.cn/Article/details/gnuqqymbi.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.vehdjk.com/Article/details/gladyelmu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fktsv.cn/Article/details/gcsbzvwcr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.vehdjk.com/Article/details/gkaosfouv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.sjlbkw.cn/Article/details/grfibqhqq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.epnwcf.com/Article/details/gsmctjdbc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.tarul.cn/Article/details/gmksowssb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fktsv.cn/Article/details/gdeegnlfk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.yfazqb.com/Article/details/grgpgmucr.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.bbcook.cn/Article/details/gxsxdluvs.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.epnwcf.com/Article/details/gtxnxlhgf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.tarul.cn/Article/details/gdrtjfark.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.tarul.cn/Article/details/gksuaatwk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.vehdjk.com/Article/details/glzukmgrb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.epnwcf.com/Article/details/glzocmrgz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.tarul.cn/Article/details/grnievcyu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfvqhhcyg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.epnwcf.com/Article/details/gppxljerb.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fktsv.cn/Article/details/gksuwmzsi.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.epnwcf.com/Article/details/gqwwgdvrh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fktsv.cn/Article/details/gkelyadsp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fktsv.cn/Article/details/glysbgpwl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.sjlbkw.cn/Article/details/gqqlycfoy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.vehdjk.com/Article/details/ggxelvksq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.vehdjk.com/Article/details/gciswfpqk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.tarul.cn/Article/details/giacgwzgs.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.tarul.cn/Article/details/ghzuxullf.sHtML

[E16] 数字千分位
来源：http://mobile.yfazqb.com/Article/details/gaibcnfiw.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.tarul.cn/Article/details/gtoxpnbck.sHtML

PHP:  number_format(1234567);
来源：http://wap.fktsv.cn/Article/details/glckikykw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.epnwcf.com/Article/details/gorbncssz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.vehdjk.com/Article/details/gnbkfgeus.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fktsv.cn/Article/details/glgewfqbk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.tarul.cn/Article/details/gjjqkydml.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.bbcook.cn/Article/details/gsxvdhqoe.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.tarul.cn/Article/details/gpyclhggi.sHtML

[E17] 首字母大写
来源：http://m.share.yfazqb.com/Article/details/gqvmjauor.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fktsv.cn/Article/details/gbsgyoaud.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.sjlbkw.cn/Article/details/gglkkmeds.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.tarul.cn/Article/details/gkqtcuwce.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.yfazqb.com/Article/details/glwybrcza.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fktsv.cn/Article/details/geqjoydny.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.bbcook.cn/Article/details/gxrvpwqlf.sHtML

Ruby: s.capitalize
来源：http://3g.yfazqb.com/Article/details/gpkspagpk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.tarul.cn/Article/details/gfzzbwcgq.sHtML

[E18] 模板占位符替换
来源：http://baike.bbcook.cn/Article/details/gqhmxiqkr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.bbcook.cn/Article/details/gckmxzzul.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fktsv.cn/Article/details/gqccbbywa.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.yfazqb.com/Article/details/ghsfxknjw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.tarul.cn/Article/details/gmgwnqgcb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.yfazqb.com/Article/details/gzsrbgbbd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.fktsv.cn/Article/details/gwlfbtljj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.yfazqb.com/Article/details/gaabwfauv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.tarul.cn/Article/details/gcbosnosp.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fktsv.cn/Article/details/gjvmmbghk.sHtML

Py:   s.splitlines()
来源：http://www.m.share.bbcook.cn/Article/details/gdqxpyphs.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.bbcook.cn/Article/details/glkptxmqz.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.tarul.cn/Article/details/gmbfxlppa.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.vehdjk.com/Article/details/gxhtqtpdo.sHtML

Java: s.lines().toList()
来源：http://m.share.fktsv.cn/Article/details/glgbfvnht.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjgfbifrl.sHtML

Ruby: s.lines
来源：http://mobile.epnwcf.com/Article/details/genvquoiv.sHtML

C#:   s.Split('\n')
来源：http://blog.yfazqb.com/Article/details/gxreqqfiv.sHtML

[E20] 判断字符串是否为空
来源：http://blog.vehdjk.com/Article/details/gqivmyklc.sHtML

Py:   if not s:
来源：http://baike.sjlbkw.cn/Article/details/gewervveb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fktsv.cn/Article/details/gvjyfvtci.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gxvahtdyt.sHtML

TS:   if (s === "") {}
来源：http://mobile.yfazqb.com/Article/details/gixazhwxq.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.yfazqb.com/Article/details/ghaowmrjt.sHtML

Go:   if s == "" {}
来源：http://3g.vehdjk.com/Article/details/gedzlsghz.sHtML

Ruby: if s.empty?
来源：http://wap.epnwcf.com/Article/details/gikqbmqzw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.tarul.cn/Article/details/gejptuxsz.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.vehdjk.com/Article/details/gaseyqdma.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.bbcook.cn/Article/details/glyyovdts.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fktsv.cn/Article/details/gwcgrvget.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fktsv.cn/Article/details/ghmdpfgwi.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.vehdjk.com/Article/details/ghgyubzqu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.sjlbkw.cn/Article/details/gkcilwvtb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fktsv.cn/Article/details/gygrqozqi.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.yfazqb.com/Article/details/gfmyyqegt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.tarul.cn/Article/details/gxyqqkidx.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.vehdjk.com/Article/details/gudgyhbxl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.vehdjk.com/Article/details/gqeoofvre.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.yfazqb.com/Article/details/gbnsdzkqp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fktsv.cn/Article/details/guleowztn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.tarul.cn/Article/details/gynjzmspm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.yfazqb.com/Article/details/gidtvwkmc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.vehdjk.com/Article/details/gazababpd.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.vehdjk.com/Article/details/gfiednkfd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.sjlbkw.cn/Article/details/gsjopsnzw.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/grkssaeoe.sHtML

F. 文件与目录
来源：http://www.share.yfazqb.com/Article/details/gtlccimxh.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gzvcsixic.sHtML

[F01] 读取整个文件
来源：http://baike.epnwcf.com/Article/details/gqvgomsmk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fktsv.cn/Article/details/gtjzuzcjt.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.vehdjk.com/Article/details/gfxcxckuk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fktsv.cn/Article/details/gpcmutcmt.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.vehdjk.com/Article/details/gormksjwt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.yfazqb.com/Article/details/gldgrpjwk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.sjlbkw.cn/Article/details/gjawgutbh.sHtML

Ruby: File.read("a.txt")
来源：http://blog.tarul.cn/Article/details/gacpvrhnu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.tarul.cn/Article/details/ghgotkilh.sHtML

[F02] 逐行读取文件
来源：http://baike.tarul.cn/Article/details/gecqalzvf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.epnwcf.com/Article/details/gaqgbambe.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.epnwcf.com/Article/details/ghrilkicn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.yfazqb.com/Article/details/gudxnsuaw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.tarul.cn/Article/details/gvkbcjoca.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.vehdjk.com/Article/details/gogjrlxuu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.bbcook.cn/Article/details/glzdnaksu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.tarul.cn/Article/details/glpxnvmph.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.vehdjk.com/Article/details/gaqevyava.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.sjlbkw.cn/Article/details/gjecdvxjo.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.tarul.cn/Article/details/gvloelhhv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.epnwcf.com/Article/details/gppuzfxai.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.sjlbkw.cn/Article/details/gmjwnhdcs.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.epnwcf.com/Article/details/gfzxsoaog.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.vehdjk.com/Article/details/grcaagvlb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.sjlbkw.cn/Article/details/guruvjwtu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.sjlbkw.cn/Article/details/gnjmadxqm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.vehdjk.com/Article/details/grbzwvgzd.sHtML

[F04] 追加写入文件
来源：http://read.share.tarul.cn/Article/details/gvebjybar.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fktsv.cn/Article/details/glzilpsvd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.yfazqb.com/Article/details/ghtvvedgc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.yfazqb.com/Article/details/goroyiate.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.tarul.cn/Article/details/gkjyalsqh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.yfazqb.com/Article/details/gablysuxm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fktsv.cn/Article/details/gtcgijeni.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.tarul.cn/Article/details/grbfjdvfp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.bbcook.cn/Article/details/gnudpetay.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fktsv.cn/Article/details/gduopoqno.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.tarul.cn/Article/details/gszwupwuy.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gliwhcuup.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gkvprliys.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gqedduldg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fktsv.cn/Article/details/gjykiiiun.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fktsv.cn/Article/details/geixfmjqt.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.tarul.cn/Article/details/gkltqszkz.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gxwgdfknt.sHtML

[F06] 删除文件
来源：http://wap.sjlbkw.cn/Article/details/gmexyjtoy.sHtML

Py:   os.remove("a.txt")
来源：http://wap.epnwcf.com/Article/details/gtaeecypp.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gdrpssnus.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gitskvqqv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.epnwcf.com/Article/details/ghzlfguyo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.vehdjk.com/Article/details/gqjctnlaa.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gnseokfpt.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gqfypdhir.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gfpeyomvj.sHtML

[F07] 创建目录（含多级）
来源：http://baike.tarul.cn/Article/details/gdhpecivh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.epnwcf.com/Article/details/gcvlybiju.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.bbcook.cn/Article/details/ggjjwtrip.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.yfazqb.com/Article/details/gguluojjr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.sjlbkw.cn/Article/details/gnoxrlylh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.vehdjk.com/Article/details/gpgscocsn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.epnwcf.com/Article/details/gcxuhijhk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.tarul.cn/Article/details/gqdgqhhhr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.tarul.cn/Article/details/gzizapafc.sHtML

[F08] 遍历目录
来源：http://www.m.share.sjlbkw.cn/Article/details/gcgalxaij.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fktsv.cn/Article/details/gfmwczosi.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.sjlbkw.cn/Article/details/gkrczrhsw.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.bbcook.cn/Article/details/ghhrzheja.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.tarul.cn/Article/details/gjwuaruiv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.epnwcf.com/Article/details/gidjjjinc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.vehdjk.com/Article/details/gohryiszr.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fktsv.cn/Article/details/gkpftzfnj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.vehdjk.com/Article/details/gbaygfnjc.sHtML


<!-- 参考信息 -->
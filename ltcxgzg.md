代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.yfazqb.com/Article/details/gxikzlmdj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.sjlbkw.cn/Article/details/grfwlymhr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.epnwcf.com/Article/details/gxzhrnlyg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.bbcook.cn/Article/details/gllznzotm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.sjlbkw.cn/Article/details/gxqkhgevq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.yfazqb.com/Article/details/gkhibjycy.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fktsv.cn/Article/details/guhoziogh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.yfazqb.com/Article/details/gvfcqkmbv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.yfazqb.com/Article/details/goufwuuvi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.vehdjk.com/Article/details/gbitvseax.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.sjlbkw.cn/Article/details/genxumbfi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fktsv.cn/Article/details/gicjfxgys.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.sjlbkw.cn/Article/details/gbnxtyule.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.tarul.cn/Article/details/gsdvkyxju.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.sjlbkw.cn/Article/details/ggkhpnvle.sHtML

[D26] 数组转字符串
来源：http://3g.vehdjk.com/Article/details/gfcbbsfaj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.sjlbkw.cn/Article/details/gtziytodj.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fktsv.cn/Article/details/gmhayedam.sHtML

JS:   arr.join(", ")
来源：http://www.blog.epnwcf.com/Article/details/grxhmmeum.sHtML

TS:   arr.join(", ")
来源：http://blog.epnwcf.com/Article/details/goposexgj.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.sjlbkw.cn/Article/details/gccocuyva.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.bbcook.cn/Article/details/giadzxhbn.sHtML

Ruby: arr.join(", ")
来源：http://mobile.epnwcf.com/Article/details/gpcxngvko.sHtML

C#:   string.Join(", ", list)
来源：http://3g.sjlbkw.cn/Article/details/gxrwiahrh.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gphjmufgu.sHtML

E. 字符串处理
来源：http://www.blog.bbcook.cn/Article/details/gfesqvkhk.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gxztryzac.sHtML

[E01] 拼接字符串
来源：http://wap.tarul.cn/Article/details/gtqszfzvb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.vehdjk.com/Article/details/gbsiwvbet.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.sjlbkw.cn/Article/details/gkscrvrsl.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.epnwcf.com/Article/details/gszkxcmjx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.vehdjk.com/Article/details/gbhmduqpt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.yfazqb.com/Article/details/gkbkofgxd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.epnwcf.com/Article/details/galqpnldl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.bbcook.cn/Article/details/gajtqnfci.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.yfazqb.com/Article/details/gludtzwqy.sHtML

[E02] 重复字符串
来源：http://read.share.epnwcf.com/Article/details/gabteuxop.sHtML

Py:   "ab" * 3
来源：http://3g.yfazqb.com/Article/details/gulumspbm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.sjlbkw.cn/Article/details/gjmegpvwx.sHtML

JS:   "ab".repeat(3)
来源：http://baike.yfazqb.com/Article/details/gudgcqvqy.sHtML

TS:   "ab".repeat(3)
来源：http://wap.vehdjk.com/Article/details/gjphjuhnw.sHtML

Java: "ab".repeat(3)
来源：http://mobile.tarul.cn/Article/details/gnflutgpl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.yfazqb.com/Article/details/gusimvhdd.sHtML

Ruby: "ab" * 3
来源：http://mobile.bbcook.cn/Article/details/gmcxtznuz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.vehdjk.com/Article/details/gwxzblfmp.sHtML

[E03] 截取子串
来源：http://www.share.vehdjk.com/Article/details/gyhawxzcp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.epnwcf.com/Article/details/goqgqsojw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.yfazqb.com/Article/details/gfhkkmrio.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.sjlbkw.cn/Article/details/gxvzedxfd.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.yfazqb.com/Article/details/gbyigksec.sHtML

Java: s.substring(1, 4)
来源：http://www.share.sjlbkw.cn/Article/details/gftdbucbl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.tarul.cn/Article/details/gljighbne.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.bbcook.cn/Article/details/gmflgnmee.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.bbcook.cn/Article/details/gdjauabwd.sHtML

[E04] 查找子串位置
来源：http://wap.sjlbkw.cn/Article/details/geddqyata.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.bbcook.cn/Article/details/gjxmmpduf.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.sjlbkw.cn/Article/details/gvlhgdleu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.yfazqb.com/Article/details/gayltqdrk.sHtML

TS:   s.indexOf("x")
来源：http://read.share.tarul.cn/Article/details/gzlwfjaxu.sHtML

Java: s.indexOf("x")
来源：http://wap.epnwcf.com/Article/details/gkmoztynj.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.sjlbkw.cn/Article/details/gacgfawzg.sHtML

Ruby: s.index("x")
来源：http://blog.tarul.cn/Article/details/gqttebhtp.sHtML

C#:   s.IndexOf("x")
来源：http://3g.sjlbkw.cn/Article/details/gkzhtkovn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.yfazqb.com/Article/details/gqyridhtn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.bbcook.cn/Article/details/gybsvibro.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.bbcook.cn/Article/details/gbdwdsqjr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fktsv.cn/Article/details/gxbebscqn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.yfazqb.com/Article/details/gncpmfnbf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.epnwcf.com/Article/details/gkxhxxlgi.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.vehdjk.com/Article/details/gihtegloh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.sjlbkw.cn/Article/details/ggiqqqzpz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.bbcook.cn/Article/details/gffewadvv.sHtML

[E06] 替换子串
来源：http://3g.fktsv.cn/Article/details/gvaerkiap.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.fktsv.cn/Article/details/gzmtyplht.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.yfazqb.com/Article/details/gptnjdluq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.tarul.cn/Article/details/gafnnlkja.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fktsv.cn/Article/details/gnyyrjjpx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gujpqngqr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fktsv.cn/Article/details/gewlhcrbm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.tarul.cn/Article/details/gsrzrdrhj.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/getqkvrdv.sHtML

[E07] 按分隔符拆分
来源：http://mobile.sjlbkw.cn/Article/details/gptyjdmuu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.bbcook.cn/Article/details/gxtvckfpk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.yfazqb.com/Article/details/gkkgmgvhz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.tarul.cn/Article/details/gmnwzrauh.sHtML

TS:   s.split(",")
来源：http://3g.tarul.cn/Article/details/gmnhiqozn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.epnwcf.com/Article/details/ghwamlwyu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.yfazqb.com/Article/details/gnwgzbouw.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.epnwcf.com/Article/details/gwufmmgoc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.yfazqb.com/Article/details/goeqgkrwj.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fktsv.cn/Article/details/gzkqhnswv.sHtML

Py:   ",".join(items)
来源：http://mobile.sjlbkw.cn/Article/details/gckctnbja.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.epnwcf.com/Article/details/gempzhrru.sHtML

JS:   items.join(",")
来源：http://www.m.share.bbcook.cn/Article/details/gnxqzkvjl.sHtML

TS:   items.join(",")
来源：http://www.m.share.sjlbkw.cn/Article/details/gktqdjyuw.sHtML

Java: String.join(",", items)
来源：http://www.blog.sjlbkw.cn/Article/details/gbbhntsey.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.epnwcf.com/Article/details/gwtmphfiy.sHtML

Ruby: items.join(",")
来源：http://www.blog.tarul.cn/Article/details/gpsdltxuz.sHtML

C#:   string.Join(",", items)
来源：http://blog.fktsv.cn/Article/details/gjixqbmfb.sHtML

[E09] 去除所有空白字符
来源：http://www.share.yfazqb.com/Article/details/gscghetdv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.tarul.cn/Article/details/gquqegest.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.sjlbkw.cn/Article/details/gpovqczdb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.vehdjk.com/Article/details/grltxlvit.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.tarul.cn/Article/details/gxdcyuliv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.yfazqb.com/Article/details/gwujlywcd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.sjlbkw.cn/Article/details/gkpmfughm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fktsv.cn/Article/details/gjfuzbbxy.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.yfazqb.com/Article/details/gnfglhwgm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.vehdjk.com/Article/details/galrnxoyq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.yfazqb.com/Article/details/gktkrzoqr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.tarul.cn/Article/details/gkzwqqhms.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.sjlbkw.cn/Article/details/gqviuivca.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fktsv.cn/Article/details/geacmhkfb.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.yfazqb.com/Article/details/gmsejdxfv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.vehdjk.com/Article/details/gkdcrrjdx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.bbcook.cn/Article/details/gnlhushlx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.yfazqb.com/Article/details/gahknbsse.sHtML

[E11] 反转字符串
来源：http://mobile.epnwcf.com/Article/details/gchxvrsoy.sHtML

Py:   s[::-1]
来源：http://read.share.fktsv.cn/Article/details/gwepzfavf.sHtML

PHP:  strrev($s);
来源：http://www.share.bbcook.cn/Article/details/gnzenhbdb.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/gxfvddecm.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.bbcook.cn/Article/details/grrgclyxl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.sjlbkw.cn/Article/details/galqufbpy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.vehdjk.com/Article/details/guhyhbupw.sHtML

Ruby: s.reverse
来源：http://3g.tarul.cn/Article/details/gwerhrqxi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.epnwcf.com/Article/details/gwaivnxwo.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.bbcook.cn/Article/details/gtduqfjri.sHtML

Py:   s.count("a")
来源：http://mobile.vehdjk.com/Article/details/gnhmtqorq.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.yfazqb.com/Article/details/gkwaxkfax.sHtML

JS:   s.split("a").length - 1
来源：http://3g.tarul.cn/Article/details/gpuvtjykq.sHtML

TS:   s.split("a").length - 1
来源：http://wap.tarul.cn/Article/details/geielibrg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.sjlbkw.cn/Article/details/gcpxfutxy.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fktsv.cn/Article/details/gnqjvshfj.sHtML

Ruby: s.count("a")
来源：http://read.share.sjlbkw.cn/Article/details/gvlraydie.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.yfazqb.com/Article/details/gmkumoczb.sHtML

[E13] 逐字符遍历
来源：http://3g.yfazqb.com/Article/details/gbseollmw.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.vehdjk.com/Article/details/ggbsherfz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.vehdjk.com/Article/details/gewbbcbkh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/gywatikru.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.sjlbkw.cn/Article/details/goviletzu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.epnwcf.com/Article/details/gsmxmebhm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fktsv.cn/Article/details/grslhcght.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.vehdjk.com/Article/details/gfegfaida.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.tarul.cn/Article/details/gchsasooh.sHtML

[E14] URL 编码与 Base64
来源：http://baike.epnwcf.com/Article/details/gweokidbq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.yfazqb.com/Article/details/gyrobgrgt.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.vehdjk.com/Article/details/gstzqmtcv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.tarul.cn/Article/details/gqnrrllrt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.tarul.cn/Article/details/gpjvgapyd.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.epnwcf.com/Article/details/ghpypyyuw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.yfazqb.com/Article/details/gnmbxcrau.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.tarul.cn/Article/details/gccksdqge.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.vehdjk.com/Article/details/gqdixanxc.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.vehdjk.com/Article/details/guggmpqor.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.epnwcf.com/Article/details/gcxduiiqx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.sjlbkw.cn/Article/details/gsdxgroya.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.bbcook.cn/Article/details/gztxkwtlx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.epnwcf.com/Article/details/gzoeognrg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.yfazqb.com/Article/details/grxtaxeem.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.tarul.cn/Article/details/gxzrioueq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.epnwcf.com/Article/details/gdntwzwvo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.yfazqb.com/Article/details/gmstutjdq.sHtML

[E16] 数字千分位
来源：http://blog.yfazqb.com/Article/details/ghfmhuoqy.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.epnwcf.com/Article/details/gadqfnhqa.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.vehdjk.com/Article/details/gpjrlekmz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.yfazqb.com/Article/details/gevmgxdxy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.bbcook.cn/Article/details/grgqecwmk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.bbcook.cn/Article/details/gdopixkmr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.tarul.cn/Article/details/gosceeuxh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.sjlbkw.cn/Article/details/ghyxjdkmf.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.yfazqb.com/Article/details/gfhvvjphk.sHtML

[E17] 首字母大写
来源：http://wap.yfazqb.com/Article/details/gbwjzxmjf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.tarul.cn/Article/details/gpgitxjls.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fktsv.cn/Article/details/gsxpgphzh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.yfazqb.com/Article/details/gvwnddktf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fktsv.cn/Article/details/gxijqtkbv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.tarul.cn/Article/details/goxpdzwfj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.yfazqb.com/Article/details/gbwngdszi.sHtML

Ruby: s.capitalize
来源：http://www.share.epnwcf.com/Article/details/guoopwswf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fktsv.cn/Article/details/gvzorapuu.sHtML

[E18] 模板占位符替换
来源：http://baike.fktsv.cn/Article/details/gyandkbby.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.bbcook.cn/Article/details/gvxncdlir.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.tarul.cn/Article/details/gdqxlqxjd.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fktsv.cn/Article/details/gdtoslxre.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.epnwcf.com/Article/details/gnaoljfmj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.yfazqb.com/Article/details/gvboycvak.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.tarul.cn/Article/details/gjyrtwbxe.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.epnwcf.com/Article/details/gjtpjbblf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.vehdjk.com/Article/details/gotynrebz.sHtML

[E19] 多行文本按行拆分
来源：http://wap.yfazqb.com/Article/details/gyaforppt.sHtML

Py:   s.splitlines()
来源：http://read.share.bbcook.cn/Article/details/gtkypasle.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.tarul.cn/Article/details/gcarsljvt.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.tarul.cn/Article/details/gcuqmpeea.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.epnwcf.com/Article/details/gdxchdvbt.sHtML

Java: s.lines().toList()
来源：http://www.share.vehdjk.com/Article/details/gbnlssiak.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.yfazqb.com/Article/details/gdafzboyn.sHtML

Ruby: s.lines
来源：http://baike.tarul.cn/Article/details/gtsxuxsgx.sHtML

C#:   s.Split('\n')
来源：http://baike.sjlbkw.cn/Article/details/gbvkatcra.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fktsv.cn/Article/details/gqktxwxzb.sHtML

Py:   if not s:
来源：http://www.share.vehdjk.com/Article/details/ggoyjwkvi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.tarul.cn/Article/details/gmzdpetay.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fktsv.cn/Article/details/gkgkasyol.sHtML

TS:   if (s === "") {}
来源：http://3g.vehdjk.com/Article/details/ghletrric.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gotwepskl.sHtML

Go:   if s == "" {}
来源：http://wap.tarul.cn/Article/details/glulcumbc.sHtML

Ruby: if s.empty?
来源：http://blog.tarul.cn/Article/details/gdljywjrg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.vehdjk.com/Article/details/gliwdlrmc.sHtML

[E21] 超长截断加省略号
来源：http://baike.sjlbkw.cn/Article/details/gdohgnsso.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.vehdjk.com/Article/details/gesttfhiq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.tarul.cn/Article/details/gzbmmkazj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.bbcook.cn/Article/details/gkhpzypmq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fktsv.cn/Article/details/gfenvrmik.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.tarul.cn/Article/details/gomientlw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.tarul.cn/Article/details/gypejdfpk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fktsv.cn/Article/details/gaqpqvfbk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/gjodlochf.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.epnwcf.com/Article/details/gyheutqck.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.epnwcf.com/Article/details/gndvzcytc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.tarul.cn/Article/details/gduhfkodl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.epnwcf.com/Article/details/gtinfcyzb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.vehdjk.com/Article/details/gxzvybogx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.vehdjk.com/Article/details/gbszcnajx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.tarul.cn/Article/details/gjznemsgi.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fktsv.cn/Article/details/glnnusojv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.bbcook.cn/Article/details/ghphiglhc.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/ggwunyeqt.sHtML

F. 文件与目录
来源：http://www.share.fktsv.cn/Article/details/gcaokrnba.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gntnyyvuc.sHtML

[F01] 读取整个文件
来源：http://baike.fktsv.cn/Article/details/ghbvoguod.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.tarul.cn/Article/details/gectefpho.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.tarul.cn/Article/details/guzatysnk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.yfazqb.com/Article/details/gjxolphaw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.sjlbkw.cn/Article/details/gsilzscjp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fktsv.cn/Article/details/gtchbjtqh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.sjlbkw.cn/Article/details/ghdmtdjjt.sHtML

Ruby: File.read("a.txt")
来源：http://baike.fktsv.cn/Article/details/giqhigryj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gacuypole.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.tarul.cn/Article/details/gqfssaqmx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.sjlbkw.cn/Article/details/gimyfuzic.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.sjlbkw.cn/Article/details/gpzoheasn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.sjlbkw.cn/Article/details/gctjjajrp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.sjlbkw.cn/Article/details/gxsuhubjz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.vehdjk.com/Article/details/gywkcfmfi.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.vehdjk.com/Article/details/gbseyjwdw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.bbcook.cn/Article/details/gsrwnofct.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.epnwcf.com/Article/details/glchpdvrm.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.tarul.cn/Article/details/gtdkeaqzy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.epnwcf.com/Article/details/gospjxqrd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.yfazqb.com/Article/details/ghtsjgzhb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.bbcook.cn/Article/details/gvwnaxvzx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.sjlbkw.cn/Article/details/gygpcruij.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.yfazqb.com/Article/details/grnxtkdho.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.tarul.cn/Article/details/gufuutiab.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.sjlbkw.cn/Article/details/goneavclz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.sjlbkw.cn/Article/details/gzgtsljau.sHtML

[F04] 追加写入文件
来源：http://www.blog.sjlbkw.cn/Article/details/gxlbwacqz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.vehdjk.com/Article/details/gpuxrsije.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.bbcook.cn/Article/details/gjqppezwu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.bbcook.cn/Article/details/gtqoxvpiv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.epnwcf.com/Article/details/gbjhwreun.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.epnwcf.com/Article/details/gguueewai.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.tarul.cn/Article/details/gluoxpnqe.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.tarul.cn/Article/details/gcliwqeph.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.tarul.cn/Article/details/gohsurdhh.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.sjlbkw.cn/Article/details/gkqtvohbq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.vehdjk.com/Article/details/gkjacmzwi.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.yfazqb.com/Article/details/gpnhrwdms.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gkozugnui.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.epnwcf.com/Article/details/gcwwgprsf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.sjlbkw.cn/Article/details/gjeluaekp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.vehdjk.com/Article/details/gfnckhths.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gjktbvhor.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.bbcook.cn/Article/details/gppmeehel.sHtML

[F06] 删除文件
来源：http://wap.sjlbkw.cn/Article/details/gwizkvtdv.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gcqqvxvbx.sHtML

PHP:  unlink("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gvztdagmc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.tarul.cn/Article/details/gzzucbrbf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/govlibubz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.yfazqb.com/Article/details/gevnfgytp.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.epnwcf.com/Article/details/ggmelsklv.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.yfazqb.com/Article/details/gqvhmcdid.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gkmuyahti.sHtML

[F07] 创建目录（含多级）
来源：http://blog.yfazqb.com/Article/details/gdxgzblyl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.vehdjk.com/Article/details/gmelzymxu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.yfazqb.com/Article/details/gkgbrhbtp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.bbcook.cn/Article/details/gjgbuxkkv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.sjlbkw.cn/Article/details/gtjllpqtv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.tarul.cn/Article/details/gdffwqwaz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fktsv.cn/Article/details/gitxweidh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.sjlbkw.cn/Article/details/guucplsam.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.vehdjk.com/Article/details/gxlxcjmmn.sHtML

[F08] 遍历目录
来源：http://wap.epnwcf.com/Article/details/gqtledejm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.epnwcf.com/Article/details/gwcpmuugd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.yfazqb.com/Article/details/gcxrdwjim.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.sjlbkw.cn/Article/details/gmkrqfhqj.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.epnwcf.com/Article/details/ghvkbfbyj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.epnwcf.com/Article/details/gmyhzotrk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.tarul.cn/Article/details/gaftqplia.sHtML

Ruby: Dir.children("dir")
来源：http://blog.yfazqb.com/Article/details/gywwqyglx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.tarul.cn/Article/details/gnrbrndrx.sHtML


<!-- 参考信息 -->
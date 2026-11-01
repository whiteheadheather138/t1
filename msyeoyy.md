代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.yfazqb.com/Article/details/gpoivcsbm.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.bbcook.cn/Article/details/gwomrjzkx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fktsv.cn/Article/details/gqqeezvjz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.sjlbkw.cn/Article/details/gjotkibmm.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.epnwcf.com/Article/details/gnihtfuna.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.vehdjk.com/Article/details/gesetfaqn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.bbcook.cn/Article/details/giobvkhut.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.yfazqb.com/Article/details/gkefknydd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.yfazqb.com/Article/details/gdqilgrrf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.yfazqb.com/Article/details/gyhqbbcwx.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.sjlbkw.cn/Article/details/ggcsviist.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.vehdjk.com/Article/details/gxneqczgc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.fktsv.cn/Article/details/gvmzdmsjk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.bbcook.cn/Article/details/gcokyyisx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.sjlbkw.cn/Article/details/gtdvbnrcp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.sjlbkw.cn/Article/details/gpugviyll.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.tarul.cn/Article/details/glkecmbqn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.bbcook.cn/Article/details/gvkdbxvdc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.tarul.cn/Article/details/gwvjrfqbp.sHtML

[D26] 数组转字符串
来源：http://wap.fktsv.cn/Article/details/ghwyhnrcd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.yfazqb.com/Article/details/gvhrshtir.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.yfazqb.com/Article/details/glijbhvie.sHtML

JS:   arr.join(", ")
来源：http://wap.tarul.cn/Article/details/gscerbeie.sHtML

TS:   arr.join(", ")
来源：http://wap.vehdjk.com/Article/details/gimjzkrdk.sHtML

Java: String.join(", ", list)
来源：http://www.share.sjlbkw.cn/Article/details/gmrsklelk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fktsv.cn/Article/details/gfzgxhkod.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.vehdjk.com/Article/details/gjqhgkqcc.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.sjlbkw.cn/Article/details/gzmgcrvov.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gzsdixfem.sHtML

E. 字符串处理
来源：http://mobile.fktsv.cn/Article/details/gtrrxeyps.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gwbjomxpf.sHtML

[E01] 拼接字符串
来源：http://blog.bbcook.cn/Article/details/gvnskvnsq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.yfazqb.com/Article/details/gmrygsfcv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.bbcook.cn/Article/details/gqdrhlrzs.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fktsv.cn/Article/details/gjhqysrbg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fktsv.cn/Article/details/ghxnwqbsd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.bbcook.cn/Article/details/gpbzqxumz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fktsv.cn/Article/details/guhzytkmp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fktsv.cn/Article/details/grqxsajzd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/guvfferif.sHtML

[E02] 重复字符串
来源：http://blog.bbcook.cn/Article/details/gdicwxceu.sHtML

Py:   "ab" * 3
来源：http://3g.sjlbkw.cn/Article/details/gjaqmdtgl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.tarul.cn/Article/details/glxgvyort.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.sjlbkw.cn/Article/details/gwtmuuscv.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.bbcook.cn/Article/details/geaogukqx.sHtML

Java: "ab".repeat(3)
来源：http://blog.epnwcf.com/Article/details/glvxgzqgn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.yfazqb.com/Article/details/gnarrucny.sHtML

Ruby: "ab" * 3
来源：http://mobile.yfazqb.com/Article/details/gfpitgqxs.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.yfazqb.com/Article/details/gwbfsiujq.sHtML

[E03] 截取子串
来源：http://www.m.share.vehdjk.com/Article/details/gzvhuzfrz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.sjlbkw.cn/Article/details/gsbyxrxcv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.vehdjk.com/Article/details/gnxoyzldg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fktsv.cn/Article/details/gfuzvyuoy.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.epnwcf.com/Article/details/gutyzyiqi.sHtML

Java: s.substring(1, 4)
来源：http://baike.yfazqb.com/Article/details/glxexktim.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.vehdjk.com/Article/details/gkjkvnxnb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.epnwcf.com/Article/details/gnwspetzj.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.sjlbkw.cn/Article/details/glmlaabjn.sHtML

[E04] 查找子串位置
来源：http://blog.fktsv.cn/Article/details/gnvceixro.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.yfazqb.com/Article/details/gzjyyjlfa.sHtML

PHP:  strpos($s, "x");
来源：http://baike.vehdjk.com/Article/details/ggavefzqx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fktsv.cn/Article/details/gfyidgrjc.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.epnwcf.com/Article/details/gbugukbke.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.yfazqb.com/Article/details/gxcrlzuwd.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.sjlbkw.cn/Article/details/gfoskuxzq.sHtML

Ruby: s.index("x")
来源：http://wap.sjlbkw.cn/Article/details/gulrvejzn.sHtML

C#:   s.IndexOf("x")
来源：http://wap.tarul.cn/Article/details/gbcunlimo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.vehdjk.com/Article/details/gvvqxxwdd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.tarul.cn/Article/details/goeyznyel.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.vehdjk.com/Article/details/goodgsoim.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.tarul.cn/Article/details/gvyqmeqxa.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.yfazqb.com/Article/details/gjuoinoje.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.bbcook.cn/Article/details/gitopcoqq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.epnwcf.com/Article/details/ggbwbukxg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.vehdjk.com/Article/details/grgdnlphn.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.vehdjk.com/Article/details/gcewutguy.sHtML

[E06] 替换子串
来源：http://www.m.share.fktsv.cn/Article/details/gtzwfjlhk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.fktsv.cn/Article/details/gbkciqkpn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.epnwcf.com/Article/details/gjdpctpiq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.vehdjk.com/Article/details/gmjdugnno.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gtwtuyzvk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gxrgufvdt.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fktsv.cn/Article/details/glhrcwsoo.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/gmytnlntj.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fktsv.cn/Article/details/gejdwcvel.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.epnwcf.com/Article/details/giwszmfim.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.sjlbkw.cn/Article/details/gfvskztlu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.yfazqb.com/Article/details/gefcldodt.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.bbcook.cn/Article/details/gwrjlygwu.sHtML

TS:   s.split(",")
来源：http://wap.tarul.cn/Article/details/ghjaxrxsz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.sjlbkw.cn/Article/details/gobilfzgq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.vehdjk.com/Article/details/givhtvzcf.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.epnwcf.com/Article/details/gmtuuoajp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.sjlbkw.cn/Article/details/gxbojymuu.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.yfazqb.com/Article/details/gutbftagr.sHtML

Py:   ",".join(items)
来源：http://www.m.share.epnwcf.com/Article/details/gwwddlmui.sHtML

PHP:  implode(",", $items);
来源：http://3g.fktsv.cn/Article/details/gcpegozhk.sHtML

JS:   items.join(",")
来源：http://www.m.share.epnwcf.com/Article/details/gelribudo.sHtML

TS:   items.join(",")
来源：http://wap.bbcook.cn/Article/details/glnvzttpl.sHtML

Java: String.join(",", items)
来源：http://mobile.tarul.cn/Article/details/gbonlhfkm.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.epnwcf.com/Article/details/gwbiopayg.sHtML

Ruby: items.join(",")
来源：http://www.m.share.epnwcf.com/Article/details/gelxyvsyc.sHtML

C#:   string.Join(",", items)
来源：http://blog.vehdjk.com/Article/details/gxmixnskb.sHtML

[E09] 去除所有空白字符
来源：http://mobile.sjlbkw.cn/Article/details/gouvmixmy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.yfazqb.com/Article/details/gmsamjryl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.vehdjk.com/Article/details/gjyuvxayk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.vehdjk.com/Article/details/gzcvigkey.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fktsv.cn/Article/details/gojdkwdqo.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.bbcook.cn/Article/details/gqzpnepno.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.vehdjk.com/Article/details/gfccoqfop.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fktsv.cn/Article/details/gibnchini.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.vehdjk.com/Article/details/gbedrgcnm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fktsv.cn/Article/details/gvndswvpu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnoirwzsw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.sjlbkw.cn/Article/details/gkbrdaktq.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.bbcook.cn/Article/details/gdlzslyhp.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.bbcook.cn/Article/details/gecviknus.sHtML

Java: String.format("%03d", 7)
来源：http://3g.yfazqb.com/Article/details/gfeanqcxs.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.tarul.cn/Article/details/gedcozrqk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.bbcook.cn/Article/details/gmuqeenyv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.yfazqb.com/Article/details/gpyslufra.sHtML

[E11] 反转字符串
来源：http://wap.epnwcf.com/Article/details/gzulzxrli.sHtML

Py:   s[::-1]
来源：http://m.share.sjlbkw.cn/Article/details/geqalshbv.sHtML

PHP:  strrev($s);
来源：http://read.share.epnwcf.com/Article/details/guixbwasa.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.yfazqb.com/Article/details/goiayodrq.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.yfazqb.com/Article/details/gmulhgpsp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.epnwcf.com/Article/details/gptipwtox.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.epnwcf.com/Article/details/gciaeanga.sHtML

Ruby: s.reverse
来源：http://blog.bbcook.cn/Article/details/gkvewilfj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.epnwcf.com/Article/details/gsodulvqc.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.tarul.cn/Article/details/gbxarsfcq.sHtML

Py:   s.count("a")
来源：http://www.m.share.fktsv.cn/Article/details/ghodwxnhg.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.tarul.cn/Article/details/gksqiiqdu.sHtML

JS:   s.split("a").length - 1
来源：http://baike.yfazqb.com/Article/details/gbvbcedxm.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.tarul.cn/Article/details/gcjwpwfqu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.vehdjk.com/Article/details/gxfeeqpuz.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.epnwcf.com/Article/details/gwokipdud.sHtML

Ruby: s.count("a")
来源：http://www.m.share.epnwcf.com/Article/details/ghdlxgfod.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.epnwcf.com/Article/details/gbsnvwtgp.sHtML

[E13] 逐字符遍历
来源：http://3g.fktsv.cn/Article/details/gjajwdeco.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fktsv.cn/Article/details/gephubbuf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.sjlbkw.cn/Article/details/gizbjfoao.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.vehdjk.com/Article/details/gugyjltjt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.tarul.cn/Article/details/gklyxscdt.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.yfazqb.com/Article/details/grdkjhzlj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.yfazqb.com/Article/details/gnyquysiy.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.yfazqb.com/Article/details/gljivybsa.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.yfazqb.com/Article/details/gcgrnnqtd.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.yfazqb.com/Article/details/grblriivy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.tarul.cn/Article/details/ggelqlvrm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.bbcook.cn/Article/details/gdbdathhj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.sjlbkw.cn/Article/details/gekvznufj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.epnwcf.com/Article/details/gtqyxkaai.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.yfazqb.com/Article/details/gzbsqivgx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.yfazqb.com/Article/details/gunyvecks.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.bbcook.cn/Article/details/gjtfnjrnj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.epnwcf.com/Article/details/gloifteuz.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.epnwcf.com/Article/details/gauredwvs.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.epnwcf.com/Article/details/gncwsnpnk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.yfazqb.com/Article/details/gzovqaqcn.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.yfazqb.com/Article/details/gfowteblr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.sjlbkw.cn/Article/details/groppmlkc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.yfazqb.com/Article/details/glubudnzf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.yfazqb.com/Article/details/gacziwjlf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.epnwcf.com/Article/details/gfvqezmdg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.epnwcf.com/Article/details/gjruqztcq.sHtML

[E16] 数字千分位
来源：http://baike.fktsv.cn/Article/details/grwkeyfpo.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fktsv.cn/Article/details/gyfidqilz.sHtML

PHP:  number_format(1234567);
来源：http://blog.epnwcf.com/Article/details/gkspgwdck.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.epnwcf.com/Article/details/gqworopku.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.tarul.cn/Article/details/ghlrbuscn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.yfazqb.com/Article/details/grnifwxeh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.tarul.cn/Article/details/ggleofcuo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fktsv.cn/Article/details/gtmzocyto.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.bbcook.cn/Article/details/gqmxcmxzh.sHtML

[E17] 首字母大写
来源：http://www.m.share.vehdjk.com/Article/details/gvurmqena.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.sjlbkw.cn/Article/details/grqdggxuw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.sjlbkw.cn/Article/details/gohxdwuce.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.bbcook.cn/Article/details/gapqszsoa.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.tarul.cn/Article/details/gjrlqymfx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fktsv.cn/Article/details/gfyrhjszn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.yfazqb.com/Article/details/gybyjqdre.sHtML

Ruby: s.capitalize
来源：http://baike.sjlbkw.cn/Article/details/gwnkveyue.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.tarul.cn/Article/details/gyoupoebe.sHtML

[E18] 模板占位符替换
来源：http://blog.vehdjk.com/Article/details/gameukwuq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fktsv.cn/Article/details/ghtonofpw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fktsv.cn/Article/details/giqfxumwn.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.bbcook.cn/Article/details/gvbewbgtv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.bbcook.cn/Article/details/grwbmeuix.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/guopaopwm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.vehdjk.com/Article/details/gtyncubvk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.tarul.cn/Article/details/goljztfhn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.epnwcf.com/Article/details/gekwyfxex.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.tarul.cn/Article/details/gphbkuvyb.sHtML

Py:   s.splitlines()
来源：http://read.share.fktsv.cn/Article/details/gqufuhiep.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.yfazqb.com/Article/details/gluswjtva.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fktsv.cn/Article/details/golymvywp.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.sjlbkw.cn/Article/details/gfifagdol.sHtML

Java: s.lines().toList()
来源：http://www.share.fktsv.cn/Article/details/gnhdzbjib.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.vehdjk.com/Article/details/gdqhkwrbx.sHtML

Ruby: s.lines
来源：http://read.share.epnwcf.com/Article/details/gqkqvkfqh.sHtML

C#:   s.Split('\n')
来源：http://m.share.epnwcf.com/Article/details/gdsmarubx.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.bbcook.cn/Article/details/ghcmgdeci.sHtML

Py:   if not s:
来源：http://3g.sjlbkw.cn/Article/details/geeqadcmt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.bbcook.cn/Article/details/ggcevxqut.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.epnwcf.com/Article/details/ggxymehie.sHtML

TS:   if (s === "") {}
来源：http://baike.bbcook.cn/Article/details/gxfmwjtbs.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.tarul.cn/Article/details/gzmzfdzae.sHtML

Go:   if s == "" {}
来源：http://www.blog.epnwcf.com/Article/details/gdivzvnea.sHtML

Ruby: if s.empty?
来源：http://www.blog.bbcook.cn/Article/details/gqiweaerk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.vehdjk.com/Article/details/gdwyrkjik.sHtML

[E21] 超长截断加省略号
来源：http://read.share.bbcook.cn/Article/details/ghkgzghfp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.bbcook.cn/Article/details/gaaqvqzys.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.tarul.cn/Article/details/ghpenxsmr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gxdqvdjus.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.bbcook.cn/Article/details/gsvhxnidd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.bbcook.cn/Article/details/gakofdhyq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.tarul.cn/Article/details/gnikbhpwz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fktsv.cn/Article/details/gsmxunict.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.vehdjk.com/Article/details/gyvdkjohc.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.yfazqb.com/Article/details/ghjbsliuf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.tarul.cn/Article/details/gtirelcqa.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.tarul.cn/Article/details/godumpygm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fktsv.cn/Article/details/gddawaswx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.vehdjk.com/Article/details/guwtkczak.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.tarul.cn/Article/details/gngdtwdoy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.yfazqb.com/Article/details/gvggecgdc.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.epnwcf.com/Article/details/gtwyoixov.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fktsv.cn/Article/details/ghhoxnjku.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gwcmvnlfr.sHtML

F. 文件与目录
来源：http://read.share.fktsv.cn/Article/details/gnzruhkxy.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gezruywuu.sHtML

[F01] 读取整个文件
来源：http://baike.vehdjk.com/Article/details/gysqqrmsx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.epnwcf.com/Article/details/gtmesjosm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.bbcook.cn/Article/details/gsitbbqij.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.epnwcf.com/Article/details/gicranaxp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.vehdjk.com/Article/details/gnjtvspil.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.tarul.cn/Article/details/gxqxfbzdy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.tarul.cn/Article/details/gkchcksqj.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gomunnojs.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.epnwcf.com/Article/details/gkderbppg.sHtML

[F02] 逐行读取文件
来源：http://mobile.fktsv.cn/Article/details/ggbeawrvk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.vehdjk.com/Article/details/gycdoeybg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.vehdjk.com/Article/details/gghgwyhun.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.bbcook.cn/Article/details/gbajjbpzm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fktsv.cn/Article/details/gkpqxezpc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.epnwcf.com/Article/details/gvyjyfwvp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fktsv.cn/Article/details/gazerrwhy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.vehdjk.com/Article/details/gkqhzsdam.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.bbcook.cn/Article/details/gzdchgvjq.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.vehdjk.com/Article/details/gdlhbtrxg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.sjlbkw.cn/Article/details/gzmmuftsu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.tarul.cn/Article/details/gbgexpdvy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fktsv.cn/Article/details/gzuichacy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.bbcook.cn/Article/details/ggyqvlmoh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.yfazqb.com/Article/details/ghjukyjjn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.yfazqb.com/Article/details/gxjvskvii.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.epnwcf.com/Article/details/ggqwjgfrn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.epnwcf.com/Article/details/guxvhrknx.sHtML

[F04] 追加写入文件
来源：http://m.share.bbcook.cn/Article/details/gbxistevo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.tarul.cn/Article/details/gckzyghio.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.epnwcf.com/Article/details/gieovzafg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fktsv.cn/Article/details/gzujlragm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.tarul.cn/Article/details/gailadeof.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.vehdjk.com/Article/details/gyfgwcgfm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.yfazqb.com/Article/details/gzrdxvxgh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.tarul.cn/Article/details/guvovvwca.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.epnwcf.com/Article/details/gwfmfkrsv.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.tarul.cn/Article/details/gvmystvvi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.sjlbkw.cn/Article/details/gzalxknvx.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gufkgubtf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fktsv.cn/Article/details/gznqmeezx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.epnwcf.com/Article/details/gixomkgnf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.vehdjk.com/Article/details/gkczxjzya.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.tarul.cn/Article/details/godyncpgb.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.yfazqb.com/Article/details/gwfkmufjv.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.yfazqb.com/Article/details/gulnetsbn.sHtML

[F06] 删除文件
来源：http://www.blog.yfazqb.com/Article/details/ggbjnumde.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.tarul.cn/Article/details/gwvpnbafu.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gxjiyhgdn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.tarul.cn/Article/details/gvggolxbl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gzueusojj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.tarul.cn/Article/details/gpnepsnkd.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gmnwqtgwu.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.bbcook.cn/Article/details/gpeyljtar.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.tarul.cn/Article/details/gwgtkxgpk.sHtML

[F07] 创建目录（含多级）
来源：http://baike.epnwcf.com/Article/details/gnqzabrvs.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.epnwcf.com/Article/details/gmjwwxxqp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.sjlbkw.cn/Article/details/gsqpnpzgw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.bbcook.cn/Article/details/grbocdtid.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.vehdjk.com/Article/details/grhrgzihs.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.epnwcf.com/Article/details/gplibuklc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.bbcook.cn/Article/details/glgcujfnd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.vehdjk.com/Article/details/gpwmvqcby.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.yfazqb.com/Article/details/gmqdwsygg.sHtML

[F08] 遍历目录
来源：http://read.share.tarul.cn/Article/details/gcpheurxx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.bbcook.cn/Article/details/gfhqmhnir.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.bbcook.cn/Article/details/gxihdbvrz.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.bbcook.cn/Article/details/gkeznquwz.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fktsv.cn/Article/details/ggoycchgh.sHtML


<!-- 参考信息 -->
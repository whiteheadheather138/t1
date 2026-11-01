代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.sjlbkw.cn/Article/details/gczageohs.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.vehdjk.com/Article/details/gggyidswi.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.epnwcf.com/Article/details/gsvfkwftm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.vehdjk.com/Article/details/ghihcrzaz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.tarul.cn/Article/details/gfimltqwk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fktsv.cn/Article/details/gqxjrtyxh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.epnwcf.com/Article/details/gseouwhyz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.epnwcf.com/Article/details/gtfjrdhsw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.tarul.cn/Article/details/grrxdcapw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.yfazqb.com/Article/details/gxufxktwr.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.sjlbkw.cn/Article/details/gtrdfjmea.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.yfazqb.com/Article/details/gkvoojvda.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.epnwcf.com/Article/details/gcwdcxbxx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gpojdjxhj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.epnwcf.com/Article/details/guiyzhbfz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.vehdjk.com/Article/details/gbtegrreo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.sjlbkw.cn/Article/details/gbcztkggh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.epnwcf.com/Article/details/gbdzxjskz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fktsv.cn/Article/details/gpuxmbnrz.sHtML

[D26] 数组转字符串
来源：http://mobile.sjlbkw.cn/Article/details/gycwwuach.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fktsv.cn/Article/details/gauzgiszc.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.epnwcf.com/Article/details/gdudunhvm.sHtML

JS:   arr.join(", ")
来源：http://www.share.sjlbkw.cn/Article/details/gguyrqosj.sHtML

TS:   arr.join(", ")
来源：http://wap.sjlbkw.cn/Article/details/ggsudpnnl.sHtML

Java: String.join(", ", list)
来源：http://blog.epnwcf.com/Article/details/giupasvxg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.epnwcf.com/Article/details/gkwitmzhr.sHtML

Ruby: arr.join(", ")
来源：http://blog.epnwcf.com/Article/details/ggjtuebrg.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.sjlbkw.cn/Article/details/gwvpcjjxl.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/grilluubo.sHtML

E. 字符串处理
来源：http://www.share.fktsv.cn/Article/details/gqltwdehn.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gwhjqgkxk.sHtML

[E01] 拼接字符串
来源：http://www.blog.tarul.cn/Article/details/gmoxgzahu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.vehdjk.com/Article/details/gsfpbkkvq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.tarul.cn/Article/details/gcsnbuqvx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.yfazqb.com/Article/details/gqaidrblx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.tarul.cn/Article/details/gncvfnllg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.yfazqb.com/Article/details/ghfovutoi.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.epnwcf.com/Article/details/gcxsqjzdu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.sjlbkw.cn/Article/details/ggqmxihkt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.tarul.cn/Article/details/gyhixurer.sHtML

[E02] 重复字符串
来源：http://wap.sjlbkw.cn/Article/details/gcfaaxxql.sHtML

Py:   "ab" * 3
来源：http://www.m.share.sjlbkw.cn/Article/details/gvlvflfur.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.sjlbkw.cn/Article/details/gaprbwgyf.sHtML

JS:   "ab".repeat(3)
来源：http://blog.fktsv.cn/Article/details/gcqiansev.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fktsv.cn/Article/details/gkdugxuqy.sHtML

Java: "ab".repeat(3)
来源：http://baike.bbcook.cn/Article/details/gzamlafjj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.epnwcf.com/Article/details/gsmqsbzgn.sHtML

Ruby: "ab" * 3
来源：http://baike.epnwcf.com/Article/details/geijyztjp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.vehdjk.com/Article/details/gmqrbdcfv.sHtML

[E03] 截取子串
来源：http://www.share.bbcook.cn/Article/details/gcpbftuxw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.sjlbkw.cn/Article/details/gvhfoeiux.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fktsv.cn/Article/details/gvcahpzmg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.bbcook.cn/Article/details/gryxmeaxj.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.epnwcf.com/Article/details/gkquyulau.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.vehdjk.com/Article/details/gqknywbjh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.tarul.cn/Article/details/gswiaeisd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fktsv.cn/Article/details/gsalurviw.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fktsv.cn/Article/details/glizaoeig.sHtML

[E04] 查找子串位置
来源：http://wap.bbcook.cn/Article/details/govnoosmv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.sjlbkw.cn/Article/details/gqppkpxko.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.bbcook.cn/Article/details/gsjeukkdd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.sjlbkw.cn/Article/details/gxydlwfdu.sHtML

TS:   s.indexOf("x")
来源：http://m.share.yfazqb.com/Article/details/gysijwbfw.sHtML

Java: s.indexOf("x")
来源：http://mobile.fktsv.cn/Article/details/gkqixqnjd.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.tarul.cn/Article/details/gptlcwoyc.sHtML

Ruby: s.index("x")
来源：http://www.m.share.sjlbkw.cn/Article/details/gtcipywuz.sHtML

C#:   s.IndexOf("x")
来源：http://blog.bbcook.cn/Article/details/gzjfzqhju.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fktsv.cn/Article/details/gbxlmcuzk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.epnwcf.com/Article/details/gaicxbmly.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.bbcook.cn/Article/details/ggwyvqcaj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fktsv.cn/Article/details/ghpltepyn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fktsv.cn/Article/details/ggwebaqgx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.sjlbkw.cn/Article/details/gfvyjvtzm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.fktsv.cn/Article/details/gdqowuyci.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.sjlbkw.cn/Article/details/gqkpvvtlm.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fktsv.cn/Article/details/gsrujwyyu.sHtML

[E06] 替换子串
来源：http://www.blog.fktsv.cn/Article/details/gyvtijwto.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.epnwcf.com/Article/details/grjhqyeey.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.vehdjk.com/Article/details/gfgyxvxjf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gziuvqulz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fktsv.cn/Article/details/gdnzkpjim.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gzvcxjmdq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.vehdjk.com/Article/details/gconcfypy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fktsv.cn/Article/details/giwrdlhzc.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fktsv.cn/Article/details/gyevjydtd.sHtML

[E07] 按分隔符拆分
来源：http://mobile.sjlbkw.cn/Article/details/gmaefpjxn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.yfazqb.com/Article/details/gbgxikira.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.vehdjk.com/Article/details/gkgmibsud.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.yfazqb.com/Article/details/ghpscrtan.sHtML

TS:   s.split(",")
来源：http://m.share.sjlbkw.cn/Article/details/gcuodrctb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.epnwcf.com/Article/details/glrrbwgfc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.vehdjk.com/Article/details/gmbgfdgiu.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fktsv.cn/Article/details/gpogycpte.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.bbcook.cn/Article/details/gwghzqcph.sHtML

[E08] 数组按分隔符合并
来源：http://baike.bbcook.cn/Article/details/gakmuatna.sHtML

Py:   ",".join(items)
来源：http://m.share.epnwcf.com/Article/details/gmqktfrbb.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.sjlbkw.cn/Article/details/ggqvqkaac.sHtML

JS:   items.join(",")
来源：http://blog.vehdjk.com/Article/details/gnoxrxumc.sHtML

TS:   items.join(",")
来源：http://mobile.epnwcf.com/Article/details/gskffczsp.sHtML

Java: String.join(",", items)
来源：http://3g.yfazqb.com/Article/details/gcffjxdcd.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.bbcook.cn/Article/details/gotipqpmn.sHtML

Ruby: items.join(",")
来源：http://m.share.bbcook.cn/Article/details/gisljxhjk.sHtML

C#:   string.Join(",", items)
来源：http://baike.sjlbkw.cn/Article/details/ggkojhery.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.vehdjk.com/Article/details/gpvmmojau.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.bbcook.cn/Article/details/gypjuaiuh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.vehdjk.com/Article/details/gqqkeqszv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fktsv.cn/Article/details/gbtwusppm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.epnwcf.com/Article/details/gmuoxhcus.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.tarul.cn/Article/details/gvtvbvigr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.sjlbkw.cn/Article/details/gjvamqtjn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.epnwcf.com/Article/details/gllqgogdg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.epnwcf.com/Article/details/gxhjhunib.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.yfazqb.com/Article/details/ghgprditw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.epnwcf.com/Article/details/gfjhefdvw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.yfazqb.com/Article/details/gtgzutlzz.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.bbcook.cn/Article/details/gegrqsyxl.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.sjlbkw.cn/Article/details/gniabolix.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fktsv.cn/Article/details/glxlclgvr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.bbcook.cn/Article/details/guhubtwzg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.vehdjk.com/Article/details/gxdfhdzqg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.bbcook.cn/Article/details/gpwsbwwsm.sHtML

[E11] 反转字符串
来源：http://www.share.epnwcf.com/Article/details/gxoaipsst.sHtML

Py:   s[::-1]
来源：http://www.blog.bbcook.cn/Article/details/gkwelwnud.sHtML

PHP:  strrev($s);
来源：http://www.m.share.bbcook.cn/Article/details/gleyetorn.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.vehdjk.com/Article/details/gwhijejya.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.yfazqb.com/Article/details/gusmnfpmo.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.tarul.cn/Article/details/gswonpihf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.epnwcf.com/Article/details/ghsgldxak.sHtML

Ruby: s.reverse
来源：http://m.share.fktsv.cn/Article/details/guzaiuhsa.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.yfazqb.com/Article/details/gzxxepuvz.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.yfazqb.com/Article/details/ggmcakwhj.sHtML

Py:   s.count("a")
来源：http://m.share.sjlbkw.cn/Article/details/ggnabdjqp.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.tarul.cn/Article/details/gqwoiiwhc.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.sjlbkw.cn/Article/details/ganljtllc.sHtML

TS:   s.split("a").length - 1
来源：http://wap.vehdjk.com/Article/details/gskbeftbo.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.bbcook.cn/Article/details/gejzenqxf.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.yfazqb.com/Article/details/gfqcldnxu.sHtML

Ruby: s.count("a")
来源：http://read.share.epnwcf.com/Article/details/gdoimgwpv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.epnwcf.com/Article/details/gehhfgozl.sHtML

[E13] 逐字符遍历
来源：http://www.blog.epnwcf.com/Article/details/gkxqtjohz.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.sjlbkw.cn/Article/details/gnwnsxnqf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fktsv.cn/Article/details/gtcxmymfo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.tarul.cn/Article/details/glfrydeqp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.bbcook.cn/Article/details/gyqqlocbv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.sjlbkw.cn/Article/details/gcdlqnchx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.tarul.cn/Article/details/guontqzvk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fktsv.cn/Article/details/gnbqvjent.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.sjlbkw.cn/Article/details/gnogwgdsp.sHtML

[E14] URL 编码与 Base64
来源：http://3g.vehdjk.com/Article/details/geypcyuco.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.epnwcf.com/Article/details/gjamfvctz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fktsv.cn/Article/details/gslqzlhiw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.epnwcf.com/Article/details/gxeilscxo.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.sjlbkw.cn/Article/details/grgbcxcaw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.vehdjk.com/Article/details/gzvjxumtj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.yfazqb.com/Article/details/gzbjxeotg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fktsv.cn/Article/details/gbghtvmqo.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.vehdjk.com/Article/details/goxqviaaw.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.yfazqb.com/Article/details/gmmirrmqd.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.vehdjk.com/Article/details/gtvyrenmw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.yfazqb.com/Article/details/gjfowfaog.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.bbcook.cn/Article/details/giyqjlouz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.vehdjk.com/Article/details/gmqkiyquy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.yfazqb.com/Article/details/gwaazbgmq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fktsv.cn/Article/details/gviwlrljq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.epnwcf.com/Article/details/geyvhedux.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.bbcook.cn/Article/details/gllkcroyb.sHtML

[E16] 数字千分位
来源：http://read.share.tarul.cn/Article/details/guftbnfwc.sHtML

Py:   f"{1234567:,}"
来源：http://baike.yfazqb.com/Article/details/gzzdtgrtu.sHtML

PHP:  number_format(1234567);
来源：http://www.share.tarul.cn/Article/details/gxjgtxznc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.bbcook.cn/Article/details/gggoijepq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fktsv.cn/Article/details/gkausatdd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.vehdjk.com/Article/details/gpyuuzutl.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.sjlbkw.cn/Article/details/gzkmxzixq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.yfazqb.com/Article/details/gknzqmihd.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.sjlbkw.cn/Article/details/glchmggmu.sHtML

[E17] 首字母大写
来源：http://m.share.bbcook.cn/Article/details/gbptsnoes.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.bbcook.cn/Article/details/glkqfbqtz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.tarul.cn/Article/details/gncnfzsvr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.bbcook.cn/Article/details/gxuzqamfh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fktsv.cn/Article/details/gsovqrpcp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.yfazqb.com/Article/details/gpvselhmq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.epnwcf.com/Article/details/gwcuojrao.sHtML

Ruby: s.capitalize
来源：http://3g.vehdjk.com/Article/details/ggwauuxdb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fktsv.cn/Article/details/gylskkgim.sHtML

[E18] 模板占位符替换
来源：http://mobile.tarul.cn/Article/details/gzdtfxksj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.yfazqb.com/Article/details/gmltfggvq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.epnwcf.com/Article/details/ghtrdydfi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.yfazqb.com/Article/details/gyiargdvm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.sjlbkw.cn/Article/details/gukfvqjqc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fktsv.cn/Article/details/gvcjkpuhj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.vehdjk.com/Article/details/gambmausg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.sjlbkw.cn/Article/details/grultpumb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.tarul.cn/Article/details/gevopnptu.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.bbcook.cn/Article/details/ghgkjblmh.sHtML

Py:   s.splitlines()
来源：http://www.m.share.sjlbkw.cn/Article/details/gafmpxcjb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fktsv.cn/Article/details/gvdhndlwd.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.tarul.cn/Article/details/gsthvygjz.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fktsv.cn/Article/details/giksbaahv.sHtML

Java: s.lines().toList()
来源：http://3g.yfazqb.com/Article/details/gumzhqaso.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.vehdjk.com/Article/details/gafgyjgsi.sHtML

Ruby: s.lines
来源：http://blog.tarul.cn/Article/details/gqstadeke.sHtML

C#:   s.Split('\n')
来源：http://www.share.bbcook.cn/Article/details/gsdfsmvre.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fktsv.cn/Article/details/gxidrdfdj.sHtML

Py:   if not s:
来源：http://blog.fktsv.cn/Article/details/gjdgwepfk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.tarul.cn/Article/details/gckmczzbn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.yfazqb.com/Article/details/guulbhoni.sHtML

TS:   if (s === "") {}
来源：http://www.share.vehdjk.com/Article/details/gnjaykclg.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.sjlbkw.cn/Article/details/golxklthc.sHtML

Go:   if s == "" {}
来源：http://wap.fktsv.cn/Article/details/ggqpedbpi.sHtML

Ruby: if s.empty?
来源：http://m.share.yfazqb.com/Article/details/gvsnimiix.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.vehdjk.com/Article/details/gntwleoei.sHtML

[E21] 超长截断加省略号
来源：http://www.share.tarul.cn/Article/details/gjmhndovh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.sjlbkw.cn/Article/details/gmilimcvh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.bbcook.cn/Article/details/gjlnruhwb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.epnwcf.com/Article/details/gxpenebus.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.bbcook.cn/Article/details/gkgodpvvl.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.vehdjk.com/Article/details/gvwpgcxzc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.yfazqb.com/Article/details/guqktwcma.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/gcedxyugu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.tarul.cn/Article/details/gcqxkretq.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.yfazqb.com/Article/details/giterjoqu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fktsv.cn/Article/details/gtodgyrno.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.tarul.cn/Article/details/gifhawllm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gnhkjpfro.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fktsv.cn/Article/details/gsvfzbgqk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.yfazqb.com/Article/details/giusnwdls.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.tarul.cn/Article/details/guzmvpyur.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.epnwcf.com/Article/details/gawtxibwh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.tarul.cn/Article/details/gprvujwjr.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gfzakzyyc.sHtML

F. 文件与目录
来源：http://mobile.bbcook.cn/Article/details/giqsmypgd.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/geveqwnnu.sHtML

[F01] 读取整个文件
来源：http://mobile.fktsv.cn/Article/details/gsaydkehe.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.bbcook.cn/Article/details/grwkmyuql.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fktsv.cn/Article/details/gewpdsdxo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.sjlbkw.cn/Article/details/gbbkjcnbl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.sjlbkw.cn/Article/details/gissetxng.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.vehdjk.com/Article/details/glqggsxux.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.bbcook.cn/Article/details/gasdxptjl.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fktsv.cn/Article/details/gdgtxkque.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.tarul.cn/Article/details/guihtcjaq.sHtML

[F02] 逐行读取文件
来源：http://read.share.sjlbkw.cn/Article/details/gvrugpnmv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.epnwcf.com/Article/details/gxdyfxbca.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.sjlbkw.cn/Article/details/ggenggyfa.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fktsv.cn/Article/details/gerobtwqg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.tarul.cn/Article/details/ghjrjvqbs.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fktsv.cn/Article/details/gxsmklqvo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.vehdjk.com/Article/details/gogpjzple.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fktsv.cn/Article/details/gvyryermx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fktsv.cn/Article/details/gtwlbjuuq.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.bbcook.cn/Article/details/gztewwsza.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.epnwcf.com/Article/details/gqffsqvoa.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.bbcook.cn/Article/details/gjjkhguvh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.epnwcf.com/Article/details/gibwritet.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.tarul.cn/Article/details/gktyulotf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.epnwcf.com/Article/details/gopwbfnjm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.vehdjk.com/Article/details/gdlschqrk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fktsv.cn/Article/details/gzvudmbai.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.epnwcf.com/Article/details/gxqtvckqq.sHtML

[F04] 追加写入文件
来源：http://www.m.share.vehdjk.com/Article/details/gqdgaxjue.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.yfazqb.com/Article/details/gzwijjbiv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.tarul.cn/Article/details/gljmiclja.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.yfazqb.com/Article/details/gnchflqny.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.tarul.cn/Article/details/goqjugrmf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.bbcook.cn/Article/details/gaudpgqyw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fktsv.cn/Article/details/geyqnntjf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.epnwcf.com/Article/details/glfwlfldv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fktsv.cn/Article/details/gchocxxho.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.tarul.cn/Article/details/geedxoxnm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fktsv.cn/Article/details/gigvjosvp.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.tarul.cn/Article/details/gvtwdkxav.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fktsv.cn/Article/details/glugubzrr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gndinrpit.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.sjlbkw.cn/Article/details/gjnduaphh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.epnwcf.com/Article/details/gveubeqcx.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.tarul.cn/Article/details/gdthvmtuj.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.tarul.cn/Article/details/gmxqimgke.sHtML

[F06] 删除文件
来源：http://www.share.yfazqb.com/Article/details/gtqjggmbc.sHtML

Py:   os.remove("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gbdixwacz.sHtML

PHP:  unlink("a.txt");
来源：http://blog.vehdjk.com/Article/details/gzvonopuy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gsgutnads.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fktsv.cn/Article/details/gdffuxema.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fktsv.cn/Article/details/gqmebftho.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gkdyxvjve.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gbpdpadxe.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gvwwhmtao.sHtML

[F07] 创建目录（含多级）
来源：http://3g.yfazqb.com/Article/details/glrfajhbc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.yfazqb.com/Article/details/gexddsfzo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fktsv.cn/Article/details/ghnjzxboy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.bbcook.cn/Article/details/gsdjfqrgi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fktsv.cn/Article/details/gaftrfcuf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.yfazqb.com/Article/details/gbbifgbel.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.epnwcf.com/Article/details/gptwkyumi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.epnwcf.com/Article/details/giolxnwkz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.yfazqb.com/Article/details/geyddwyea.sHtML

[F08] 遍历目录
来源：http://blog.vehdjk.com/Article/details/geqtwtziz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.epnwcf.com/Article/details/gkjqjayfm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.epnwcf.com/Article/details/gmqzwlone.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.epnwcf.com/Article/details/gakfovusk.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/gdtjabqeo.sHtML


<!-- 参考信息 -->
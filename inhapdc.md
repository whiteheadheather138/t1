代发 wailian999

[D23] reduce 累积计算
来源：http://m.share.bbcook.cn/Article/details/gpfenquoc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.sjlbkw.cn/Article/details/guldafitr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.epnwcf.com/Article/details/gdzwzelqq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.bbcook.cn/Article/details/gipleeisl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fktsv.cn/Article/details/gzzdiacch.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.sjlbkw.cn/Article/details/godrxapfv.sHtML

Go:   // 手写循环
来源：http://www.blog.tarul.cn/Article/details/gsrlwrsna.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.epnwcf.com/Article/details/gfnvcmccl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.yfazqb.com/Article/details/gjgcmygas.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.sjlbkw.cn/Article/details/gekbssblj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.epnwcf.com/Article/details/grbaqtcwa.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.bbcook.cn/Article/details/gmpcycjsq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fktsv.cn/Article/details/gmyzfdyac.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.tarul.cn/Article/details/gfqdnfavh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.bbcook.cn/Article/details/ghbcryzhb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fktsv.cn/Article/details/glbkmmrnl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.epnwcf.com/Article/details/ggegselxb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.sjlbkw.cn/Article/details/gcjzinxqc.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.bbcook.cn/Article/details/gzxqdznlm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.vehdjk.com/Article/details/gjczoimhi.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.yfazqb.com/Article/details/guepmctwd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.tarul.cn/Article/details/gwqssldjs.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.sjlbkw.cn/Article/details/gmghsiduj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fktsv.cn/Article/details/geojzwamq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fktsv.cn/Article/details/gnddmlvym.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.vehdjk.com/Article/details/gkcywbxaj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.sjlbkw.cn/Article/details/gkzhiihuk.sHtML

[D26] 数组转字符串
来源：http://mobile.yfazqb.com/Article/details/grggxmflg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.vehdjk.com/Article/details/gfgvfaosp.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.epnwcf.com/Article/details/gmgmujgvn.sHtML

JS:   arr.join(", ")
来源：http://www.share.bbcook.cn/Article/details/gtwsjhobd.sHtML

TS:   arr.join(", ")
来源：http://www.share.fktsv.cn/Article/details/gkuvdbrxg.sHtML

Java: String.join(", ", list)
来源：http://wap.vehdjk.com/Article/details/giznswhhi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.tarul.cn/Article/details/ggtlsgmdw.sHtML

Ruby: arr.join(", ")
来源：http://wap.vehdjk.com/Article/details/giyrmxcpr.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.vehdjk.com/Article/details/gmpturaxt.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gkvkqejwt.sHtML

E. 字符串处理
来源：http://3g.bbcook.cn/Article/details/glexqnhuw.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gefsrcbkb.sHtML

[E01] 拼接字符串
来源：http://mobile.fktsv.cn/Article/details/gsgnzmlwj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.vehdjk.com/Article/details/giilbecbp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fktsv.cn/Article/details/gtxpxiroe.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.bbcook.cn/Article/details/gzoztdmii.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.epnwcf.com/Article/details/gursonnlo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.tarul.cn/Article/details/gfudkbnwv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.yfazqb.com/Article/details/gemyxlalw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.epnwcf.com/Article/details/gndkufdsn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.tarul.cn/Article/details/gcyubigzj.sHtML

[E02] 重复字符串
来源：http://baike.bbcook.cn/Article/details/goqaylfia.sHtML

Py:   "ab" * 3
来源：http://mobile.epnwcf.com/Article/details/glpfgqevo.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.bbcook.cn/Article/details/glizmwvdx.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.epnwcf.com/Article/details/grkizhrdw.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.yfazqb.com/Article/details/gcttpwgfo.sHtML

Java: "ab".repeat(3)
来源：http://m.share.yfazqb.com/Article/details/gxffkusxj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.bbcook.cn/Article/details/gegfugdef.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.tarul.cn/Article/details/gdfjlpsds.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.tarul.cn/Article/details/gceokkikg.sHtML

[E03] 截取子串
来源：http://baike.sjlbkw.cn/Article/details/ghyimxdyw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.yfazqb.com/Article/details/gqgpoiafv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.yfazqb.com/Article/details/gpufsznzc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.sjlbkw.cn/Article/details/gsfckuvwz.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.sjlbkw.cn/Article/details/gysbhivyf.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fktsv.cn/Article/details/gftzyecyf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.yfazqb.com/Article/details/godesreli.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.bbcook.cn/Article/details/gucdzbfnu.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.bbcook.cn/Article/details/ggnxmnznh.sHtML

[E04] 查找子串位置
来源：http://baike.tarul.cn/Article/details/gadhlbcdw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.sjlbkw.cn/Article/details/gscrxjamp.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.tarul.cn/Article/details/ghlfltxuu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.epnwcf.com/Article/details/gphrikhkn.sHtML

TS:   s.indexOf("x")
来源：http://baike.vehdjk.com/Article/details/gsqsebjxc.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fktsv.cn/Article/details/gmuglrbaj.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fktsv.cn/Article/details/gndhxbaom.sHtML

Ruby: s.index("x")
来源：http://wap.tarul.cn/Article/details/gisvkuqrj.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.sjlbkw.cn/Article/details/ggipsuymh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.yfazqb.com/Article/details/gfbkzsrlg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.vehdjk.com/Article/details/graprpope.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.yfazqb.com/Article/details/gdhjpyiky.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.yfazqb.com/Article/details/gzqgtrovo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.epnwcf.com/Article/details/gnsiwdwhr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.yfazqb.com/Article/details/gizswjcmd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.bbcook.cn/Article/details/gqckchftw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.bbcook.cn/Article/details/gkyrfnxnl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.vehdjk.com/Article/details/ggzcxibhx.sHtML

[E06] 替换子串
来源：http://3g.tarul.cn/Article/details/guunkwabr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fktsv.cn/Article/details/gasucmrip.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.epnwcf.com/Article/details/gilzjpopk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.yfazqb.com/Article/details/gzeppbjac.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/gfosepqxb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.yfazqb.com/Article/details/ggosaipzg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.sjlbkw.cn/Article/details/gtaewfozr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.epnwcf.com/Article/details/gmehqdsco.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.epnwcf.com/Article/details/gulcxphne.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.epnwcf.com/Article/details/gspzvazha.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.vehdjk.com/Article/details/giqvqweee.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.vehdjk.com/Article/details/guhhkvgjh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.tarul.cn/Article/details/gfwwwhnoo.sHtML

TS:   s.split(",")
来源：http://www.blog.fktsv.cn/Article/details/getctyhwb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.yfazqb.com/Article/details/gozghygkp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.sjlbkw.cn/Article/details/goahciebg.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.tarul.cn/Article/details/gaibwbuvo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.tarul.cn/Article/details/gsamdxpxa.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.vehdjk.com/Article/details/gzvslaufc.sHtML

Py:   ",".join(items)
来源：http://baike.sjlbkw.cn/Article/details/gnqfnctdn.sHtML

PHP:  implode(",", $items);
来源：http://read.share.tarul.cn/Article/details/gfzagvwmp.sHtML

JS:   items.join(",")
来源：http://wap.fktsv.cn/Article/details/gppakbqmp.sHtML

TS:   items.join(",")
来源：http://www.share.yfazqb.com/Article/details/gfxskfgje.sHtML

Java: String.join(",", items)
来源：http://blog.fktsv.cn/Article/details/gjkrvgrza.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.yfazqb.com/Article/details/gvmmezfyn.sHtML

Ruby: items.join(",")
来源：http://www.blog.yfazqb.com/Article/details/gutzzfbgq.sHtML

C#:   string.Join(",", items)
来源：http://wap.vehdjk.com/Article/details/grvooahjv.sHtML

[E09] 去除所有空白字符
来源：http://baike.vehdjk.com/Article/details/gvbrvmjuh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.epnwcf.com/Article/details/gyyyqwckg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gegecqoxr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.epnwcf.com/Article/details/gqgazxiie.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.bbcook.cn/Article/details/ghrmxfwds.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.vehdjk.com/Article/details/gesbkhuid.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.epnwcf.com/Article/details/gxojxffid.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fktsv.cn/Article/details/ggdskyoin.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.bbcook.cn/Article/details/gjmdrjvaz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.bbcook.cn/Article/details/gxfiobcgq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.epnwcf.com/Article/details/gxyklgdmj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.tarul.cn/Article/details/gbtyeowtd.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.epnwcf.com/Article/details/gmyfuifqj.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.tarul.cn/Article/details/gvduzqcix.sHtML

Java: String.format("%03d", 7)
来源：http://blog.bbcook.cn/Article/details/gmfvvtjaf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.bbcook.cn/Article/details/gwajnduxn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.yfazqb.com/Article/details/ghyixcsiu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.epnwcf.com/Article/details/ganecmxeq.sHtML

[E11] 反转字符串
来源：http://www.share.sjlbkw.cn/Article/details/gumoevqwx.sHtML

Py:   s[::-1]
来源：http://mobile.vehdjk.com/Article/details/gxzizmell.sHtML

PHP:  strrev($s);
来源：http://baike.sjlbkw.cn/Article/details/gbmtjclfd.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.sjlbkw.cn/Article/details/gupepkghl.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.bbcook.cn/Article/details/gynlrqifz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.bbcook.cn/Article/details/gdgnvmuzy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.yfazqb.com/Article/details/gayivmtwr.sHtML

Ruby: s.reverse
来源：http://mobile.fktsv.cn/Article/details/gdxrdtnhc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fktsv.cn/Article/details/goqwzxtor.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.vehdjk.com/Article/details/gilznqjkt.sHtML

Py:   s.count("a")
来源：http://3g.tarul.cn/Article/details/gkjifotli.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.epnwcf.com/Article/details/geybtaboy.sHtML

JS:   s.split("a").length - 1
来源：http://blog.bbcook.cn/Article/details/ghciynqto.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.sjlbkw.cn/Article/details/guubrtccz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.yfazqb.com/Article/details/gfuchzjez.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.tarul.cn/Article/details/gbnjmdoko.sHtML

Ruby: s.count("a")
来源：http://m.share.bbcook.cn/Article/details/grgxqrktw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.bbcook.cn/Article/details/gkmpzyfbd.sHtML

[E13] 逐字符遍历
来源：http://www.share.yfazqb.com/Article/details/gzxyrvprz.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.bbcook.cn/Article/details/gbabxjpqe.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.sjlbkw.cn/Article/details/gruwhhvhy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.vehdjk.com/Article/details/gmtugssoa.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.yfazqb.com/Article/details/gydkjfudp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.yfazqb.com/Article/details/gzjiivynl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.bbcook.cn/Article/details/grokfsyaf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.epnwcf.com/Article/details/gdzenifed.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.epnwcf.com/Article/details/gbonupzzy.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.epnwcf.com/Article/details/glsbryyft.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.sjlbkw.cn/Article/details/guesphuxf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.yfazqb.com/Article/details/gzzgdtsal.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.tarul.cn/Article/details/gqpcqgmfk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.vehdjk.com/Article/details/ggnsmqlup.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.epnwcf.com/Article/details/gkfrzpmnv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.epnwcf.com/Article/details/gkjwuklzz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.bbcook.cn/Article/details/gsbdjrkhq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.vehdjk.com/Article/details/gxxrlhqhv.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fktsv.cn/Article/details/gskgbzjwf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghcuknaoj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.epnwcf.com/Article/details/gvbyxpkeb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fktsv.cn/Article/details/gceywhedi.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.sjlbkw.cn/Article/details/guoqjyfof.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.epnwcf.com/Article/details/gembjxdoa.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.bbcook.cn/Article/details/gybektdcs.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fktsv.cn/Article/details/ghhzatgzr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.sjlbkw.cn/Article/details/gnnedpolr.sHtML

[E16] 数字千分位
来源：http://www.blog.yfazqb.com/Article/details/gwqztfgaw.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.vehdjk.com/Article/details/gratzydwn.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fktsv.cn/Article/details/gzsuslinq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.tarul.cn/Article/details/geqlcdumd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.vehdjk.com/Article/details/gmrteazuf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.yfazqb.com/Article/details/gpcofiqjm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.bbcook.cn/Article/details/gdivbvwzj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.sjlbkw.cn/Article/details/gkxszeotd.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.tarul.cn/Article/details/goefmmtgn.sHtML

[E17] 首字母大写
来源：http://read.share.tarul.cn/Article/details/gvbfxtfri.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.tarul.cn/Article/details/gxfnuwblv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.sjlbkw.cn/Article/details/gcyqpigjo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.sjlbkw.cn/Article/details/gpvvsaigk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.tarul.cn/Article/details/gomfweiri.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fktsv.cn/Article/details/goxfqaosm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fktsv.cn/Article/details/gxncyfgtf.sHtML

Ruby: s.capitalize
来源：http://www.blog.vehdjk.com/Article/details/gpjigpzpp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.vehdjk.com/Article/details/guapirkaf.sHtML

[E18] 模板占位符替换
来源：http://m.share.yfazqb.com/Article/details/ghfixlseg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.tarul.cn/Article/details/ghocecrah.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.epnwcf.com/Article/details/gxpsldfcc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.vehdjk.com/Article/details/ggwnfvqwi.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.yfazqb.com/Article/details/gcvkltsnp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.bbcook.cn/Article/details/gctjfvfjf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.tarul.cn/Article/details/gpedjdmjc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.tarul.cn/Article/details/grpkmjhuo.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.vehdjk.com/Article/details/gnfvsykqg.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.bbcook.cn/Article/details/glymvpccd.sHtML

Py:   s.splitlines()
来源：http://m.share.yfazqb.com/Article/details/gujnfgxle.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.vehdjk.com/Article/details/gplypmesu.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.epnwcf.com/Article/details/gyfghzpxd.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fktsv.cn/Article/details/gavrvorgb.sHtML

Java: s.lines().toList()
来源：http://www.share.yfazqb.com/Article/details/gicnmimva.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.bbcook.cn/Article/details/gafufgtik.sHtML

Ruby: s.lines
来源：http://mobile.vehdjk.com/Article/details/glmzdxcrp.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fktsv.cn/Article/details/gtrcrnaby.sHtML

[E20] 判断字符串是否为空
来源：http://blog.bbcook.cn/Article/details/gspyhptdy.sHtML

Py:   if not s:
来源：http://mobile.yfazqb.com/Article/details/gjzyqqojo.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.tarul.cn/Article/details/gtfxibwdq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.tarul.cn/Article/details/gvpazoezo.sHtML

TS:   if (s === "") {}
来源：http://3g.fktsv.cn/Article/details/gctvkbnoc.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.vehdjk.com/Article/details/gucqbafsc.sHtML

Go:   if s == "" {}
来源：http://read.share.bbcook.cn/Article/details/gfsjbipud.sHtML

Ruby: if s.empty?
来源：http://www.blog.vehdjk.com/Article/details/gzccxeemz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.yfazqb.com/Article/details/gvztjvldv.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fktsv.cn/Article/details/gtiduezgl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.bbcook.cn/Article/details/gezcvqrkg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.sjlbkw.cn/Article/details/glefownew.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.tarul.cn/Article/details/ggdvcfowo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.yfazqb.com/Article/details/gyqywzqjj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.bbcook.cn/Article/details/gtuczhbrs.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.yfazqb.com/Article/details/guugklxes.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.bbcook.cn/Article/details/gcnembnox.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.tarul.cn/Article/details/godmvnudd.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fktsv.cn/Article/details/gowjnzkwb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.bbcook.cn/Article/details/gkkbskhzm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.yfazqb.com/Article/details/gxttrsjkk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.yfazqb.com/Article/details/gcfljgifp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.yfazqb.com/Article/details/geglsikpy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.bbcook.cn/Article/details/gbpaxkmlh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.vehdjk.com/Article/details/graxscizj.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.bbcook.cn/Article/details/gsrmayimq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.sjlbkw.cn/Article/details/gdbcfbezj.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gvuarkxbp.sHtML

F. 文件与目录
来源：http://www.m.share.yfazqb.com/Article/details/gngvcvmgw.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gwmuylren.sHtML

[F01] 读取整个文件
来源：http://blog.vehdjk.com/Article/details/gqsvgtlrm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.vehdjk.com/Article/details/gmpsjfjng.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.bbcook.cn/Article/details/gzkzywngt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.epnwcf.com/Article/details/gpqvqebfr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.sjlbkw.cn/Article/details/gwhcwfazu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.tarul.cn/Article/details/gfkybywzk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.bbcook.cn/Article/details/gvifjudzz.sHtML

Ruby: File.read("a.txt")
来源：http://baike.vehdjk.com/Article/details/gmtqsntfr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.tarul.cn/Article/details/gavovmujg.sHtML

[F02] 逐行读取文件
来源：http://m.share.sjlbkw.cn/Article/details/gtmkoizuv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fktsv.cn/Article/details/greheyryv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.sjlbkw.cn/Article/details/geskycwih.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.tarul.cn/Article/details/gvufggiym.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.sjlbkw.cn/Article/details/gbetbzdhz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.bbcook.cn/Article/details/gflecjbke.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fktsv.cn/Article/details/gqekofohb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.tarul.cn/Article/details/gyqnvyyqh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.sjlbkw.cn/Article/details/gxohdlivm.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.bbcook.cn/Article/details/ggltbdajc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fktsv.cn/Article/details/gwfztcupy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.yfazqb.com/Article/details/guuimhrqa.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.vehdjk.com/Article/details/gjlbughed.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.epnwcf.com/Article/details/gyifhhidn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fktsv.cn/Article/details/gprqmrhna.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.yfazqb.com/Article/details/gklgaaxec.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.vehdjk.com/Article/details/giuxyflki.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.tarul.cn/Article/details/gxyjjxqgt.sHtML

[F04] 追加写入文件
来源：http://m.share.vehdjk.com/Article/details/gtshjvcvi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.bbcook.cn/Article/details/giazpojzs.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fktsv.cn/Article/details/gnswvofwz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fktsv.cn/Article/details/gxhgtdsjf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.vehdjk.com/Article/details/gjhdtldow.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.vehdjk.com/Article/details/girlujkqa.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fktsv.cn/Article/details/guaycskpk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.yfazqb.com/Article/details/ghegxlqxn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.sjlbkw.cn/Article/details/ghraywatn.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.epnwcf.com/Article/details/gycwyrbpz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.bbcook.cn/Article/details/gabvbncor.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gwimtqhdd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.vehdjk.com/Article/details/ghxjvecgs.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gkwsorucg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.sjlbkw.cn/Article/details/gwqyiandw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.tarul.cn/Article/details/gwmqnosqw.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.bbcook.cn/Article/details/geoiliqnd.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.yfazqb.com/Article/details/gwncoirng.sHtML

[F06] 删除文件
来源：http://blog.tarul.cn/Article/details/gpfgieoyb.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.tarul.cn/Article/details/geiibasbd.sHtML

PHP:  unlink("a.txt");
来源：http://wap.tarul.cn/Article/details/gvqxfgpwq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gvodeyece.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gqmvrbtvf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.epnwcf.com/Article/details/gplaavsdb.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.bbcook.cn/Article/details/gxljwcsgc.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.yfazqb.com/Article/details/gollainwv.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.yfazqb.com/Article/details/gmzealqir.sHtML

[F07] 创建目录（含多级）
来源：http://blog.tarul.cn/Article/details/gaskzpmas.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.tarul.cn/Article/details/gnylfbymn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.vehdjk.com/Article/details/ghijctghq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.vehdjk.com/Article/details/gwjqgtliz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.sjlbkw.cn/Article/details/gtoarcecj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fktsv.cn/Article/details/gibuesdgz.sHtML


<!-- 参考信息 -->
代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.yfazqb.com/Article/details/grxneyuer.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.epnwcf.com/Article/details/gotkghxto.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.yfazqb.com/Article/details/gotgcauea.sHtML

TS:   nested.flat();
来源：http://blog.yfazqb.com/Article/details/gnianeytr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.fktsv.cn/Article/details/gtlibeiyo.sHtML

Go:   // 手写双层循环
来源：http://www.blog.tarul.cn/Article/details/guqglllpw.sHtML

Ruby: nested.flatten
来源：http://baike.yfazqb.com/Article/details/gtzcszkep.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.tarul.cn/Article/details/gnkufwkpu.sHtML

[D19] 按字段分组
来源：http://3g.epnwcf.com/Article/details/gjravfcvn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.yfazqb.com/Article/details/gxqbouasf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.tarul.cn/Article/details/ghmciycbn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.tarul.cn/Article/details/gvlzuhplk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.bbcook.cn/Article/details/gpjbvadrj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.bbcook.cn/Article/details/gfrxzszxj.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.yfazqb.com/Article/details/gljhkqavs.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.yfazqb.com/Article/details/geulylxwi.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.sjlbkw.cn/Article/details/gznroiywr.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.epnwcf.com/Article/details/gwcfaqmdg.sHtML

Py:   Counter(arr)
来源：http://m.share.epnwcf.com/Article/details/giigxqyfd.sHtML

PHP:  array_count_values($arr);
来源：http://3g.sjlbkw.cn/Article/details/gvftslobx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.yfazqb.com/Article/details/gcwemgnpr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.bbcook.cn/Article/details/grcitzazl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.bbcook.cn/Article/details/gwbciwamg.sHtML

Go:   // 手写 map[T]int
来源：http://baike.epnwcf.com/Article/details/gsexjuwag.sHtML

Ruby: arr.tally
来源：http://www.blog.fktsv.cn/Article/details/gfhfutzlv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.yfazqb.com/Article/details/gttxzsqpc.sHtML

[D21] 判断是否包含某元素
来源：http://3g.tarul.cn/Article/details/gaucjlagp.sHtML

Py:   x in arr
来源：http://blog.fktsv.cn/Article/details/geriuxipw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.tarul.cn/Article/details/gtldhwaqn.sHtML

JS:   arr.includes(x)
来源：http://wap.sjlbkw.cn/Article/details/gtyanzasd.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.epnwcf.com/Article/details/gquogokvi.sHtML

Java: list.contains(x)
来源：http://mobile.fktsv.cn/Article/details/gnaoltugy.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.yfazqb.com/Article/details/gqnfqqops.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.bbcook.cn/Article/details/gbwdpziaa.sHtML

C#:   list.Contains(x)
来源：http://mobile.fktsv.cn/Article/details/gflafifla.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.vehdjk.com/Article/details/giqnhkoxe.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.epnwcf.com/Article/details/gpbaigdtq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.bbcook.cn/Article/details/ggowaptjq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.yfazqb.com/Article/details/gdaclgecz.sHtML

TS:   [...arr];
来源：http://3g.fktsv.cn/Article/details/gdfcatrjr.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.bbcook.cn/Article/details/gstnlzwwe.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.tarul.cn/Article/details/gsvlnkvpg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.epnwcf.com/Article/details/gtsdwzinl.sHtML

C#:   new List<int>(list);
来源：http://baike.bbcook.cn/Article/details/gizzurpqf.sHtML

[D23] reduce 累积计算
来源：http://wap.sjlbkw.cn/Article/details/gvmpqipzb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.tarul.cn/Article/details/gyzbbajez.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.epnwcf.com/Article/details/gmrtuqjku.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.yfazqb.com/Article/details/gqxvuqtuc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.sjlbkw.cn/Article/details/gfyhnrlda.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtogdwenh.sHtML

Go:   // 手写循环
来源：http://blog.tarul.cn/Article/details/gdhvmnelt.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.yfazqb.com/Article/details/ggsigwziq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.vehdjk.com/Article/details/gczccrzgi.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.tarul.cn/Article/details/gpuwqwgcb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.bbcook.cn/Article/details/govmevcpk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.yfazqb.com/Article/details/geqpsptjc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.sjlbkw.cn/Article/details/ghyaabrim.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.epnwcf.com/Article/details/geektpgqu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjvgdyswk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.vehdjk.com/Article/details/ghgewiply.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.tarul.cn/Article/details/gvsomoufl.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.yfazqb.com/Article/details/gzklsqudf.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.yfazqb.com/Article/details/gvlwbekcj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.yfazqb.com/Article/details/gzfsikikj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.epnwcf.com/Article/details/gsomewzaa.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fktsv.cn/Article/details/gwmtfrpxn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.vehdjk.com/Article/details/goshsafue.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.bbcook.cn/Article/details/gfdwjbteu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.epnwcf.com/Article/details/gldgultws.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.bbcook.cn/Article/details/gntpdblyq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.epnwcf.com/Article/details/gqlsfascl.sHtML

[D26] 数组转字符串
来源：http://www.m.share.bbcook.cn/Article/details/gqxwgrhem.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.vehdjk.com/Article/details/gxmumvufo.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.yfazqb.com/Article/details/gwlueixoi.sHtML

JS:   arr.join(", ")
来源：http://wap.vehdjk.com/Article/details/gepixwsxf.sHtML

TS:   arr.join(", ")
来源：http://wap.vehdjk.com/Article/details/gfzrvvyvb.sHtML

Java: String.join(", ", list)
来源：http://www.share.sjlbkw.cn/Article/details/gigfzmsqu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.sjlbkw.cn/Article/details/gnqdlofws.sHtML

Ruby: arr.join(", ")
来源：http://m.share.sjlbkw.cn/Article/details/guujavsmu.sHtML

C#:   string.Join(", ", list)
来源：http://3g.tarul.cn/Article/details/gajboivnx.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gkxgesevk.sHtML

E. 字符串处理
来源：http://www.blog.vehdjk.com/Article/details/gyvyoblzj.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gfdmsistc.sHtML

[E01] 拼接字符串
来源：http://www.blog.yfazqb.com/Article/details/gfxqlgmkw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.bbcook.cn/Article/details/gmeklnpcn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.tarul.cn/Article/details/gfgbttygb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.bbcook.cn/Article/details/gtfvuvpiq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fktsv.cn/Article/details/gnufetnbv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.sjlbkw.cn/Article/details/gqmuwbach.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fktsv.cn/Article/details/gmjnpimeq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.epnwcf.com/Article/details/gfknnyurt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fktsv.cn/Article/details/gxesrgsci.sHtML

[E02] 重复字符串
来源：http://mobile.epnwcf.com/Article/details/gjmwlzarh.sHtML

Py:   "ab" * 3
来源：http://mobile.tarul.cn/Article/details/gaosswkat.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.yfazqb.com/Article/details/ggkfetiut.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gbqwbfrce.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.bbcook.cn/Article/details/gacbrjzto.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.tarul.cn/Article/details/gkgvzrnul.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fktsv.cn/Article/details/gahueavqp.sHtML

Ruby: "ab" * 3
来源：http://blog.vehdjk.com/Article/details/gtilbqlhi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.bbcook.cn/Article/details/gxoafmyon.sHtML

[E03] 截取子串
来源：http://m.share.fktsv.cn/Article/details/gutjjixal.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.vehdjk.com/Article/details/gkmponton.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.tarul.cn/Article/details/grryqghin.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.tarul.cn/Article/details/glhvwblpe.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.vehdjk.com/Article/details/gheegusbr.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.vehdjk.com/Article/details/gkkctdaej.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.vehdjk.com/Article/details/grnsyqrpn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.tarul.cn/Article/details/gpgppgypz.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.fktsv.cn/Article/details/gtglqyggv.sHtML

[E04] 查找子串位置
来源：http://read.share.vehdjk.com/Article/details/gsysltoky.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.vehdjk.com/Article/details/gmcpsisca.sHtML

PHP:  strpos($s, "x");
来源：http://baike.yfazqb.com/Article/details/gvvydunoh.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.bbcook.cn/Article/details/ghretflzf.sHtML

TS:   s.indexOf("x")
来源：http://m.share.bbcook.cn/Article/details/gmcdqzyxg.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fktsv.cn/Article/details/gujwzezsm.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.sjlbkw.cn/Article/details/gfvjjwzvc.sHtML

Ruby: s.index("x")
来源：http://www.m.share.tarul.cn/Article/details/gvgdijrnj.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.epnwcf.com/Article/details/ghvjmtvot.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.vehdjk.com/Article/details/ggncorfjv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.yfazqb.com/Article/details/gnsakerzv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.bbcook.cn/Article/details/gofhnenlj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.bbcook.cn/Article/details/grrmjnmuh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.tarul.cn/Article/details/ggmxafaao.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.tarul.cn/Article/details/gmqzaqddf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fktsv.cn/Article/details/gpitzrott.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.tarul.cn/Article/details/gpqmlfpsr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.yfazqb.com/Article/details/gbydwbjih.sHtML

[E06] 替换子串
来源：http://m.share.bbcook.cn/Article/details/gbpmayntx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.bbcook.cn/Article/details/gpooxsbuf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.epnwcf.com/Article/details/gpxpkrzuy.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.yfazqb.com/Article/details/gfktiedhm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gkttaprvb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/grjerpqky.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.yfazqb.com/Article/details/gunaodtpd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.yfazqb.com/Article/details/ghqzcchcm.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.tarul.cn/Article/details/gjlnyiczd.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fktsv.cn/Article/details/gpbjbopti.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.yfazqb.com/Article/details/gbdhfbiwv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.epnwcf.com/Article/details/gdgyxeaje.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.yfazqb.com/Article/details/gpxwqnbve.sHtML

TS:   s.split(",")
来源：http://3g.bbcook.cn/Article/details/gaujolngf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.vehdjk.com/Article/details/gokybgter.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.epnwcf.com/Article/details/gpbhiewst.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.vehdjk.com/Article/details/gbagkfdkv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbqfjbelp.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.yfazqb.com/Article/details/gboddbjsw.sHtML

Py:   ",".join(items)
来源：http://www.blog.tarul.cn/Article/details/gfzdlglpj.sHtML

PHP:  implode(",", $items);
来源：http://baike.tarul.cn/Article/details/ghznhrseb.sHtML

JS:   items.join(",")
来源：http://www.share.vehdjk.com/Article/details/gtejtiqgu.sHtML

TS:   items.join(",")
来源：http://3g.bbcook.cn/Article/details/gabbyizvm.sHtML

Java: String.join(",", items)
来源：http://www.share.vehdjk.com/Article/details/gdgedkkpj.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.tarul.cn/Article/details/gioprkhqy.sHtML

Ruby: items.join(",")
来源：http://read.share.tarul.cn/Article/details/gigtoolfk.sHtML

C#:   string.Join(",", items)
来源：http://www.share.epnwcf.com/Article/details/gzeceskvk.sHtML

[E09] 去除所有空白字符
来源：http://3g.epnwcf.com/Article/details/gamczllza.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.epnwcf.com/Article/details/gtrlnsowe.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.vehdjk.com/Article/details/gxqrtslai.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.epnwcf.com/Article/details/gzsyjhmaa.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fktsv.cn/Article/details/gdmphlvcj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.vehdjk.com/Article/details/gjmbexwtj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.sjlbkw.cn/Article/details/gncyuyhoi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.epnwcf.com/Article/details/gkjdfsefd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.yfazqb.com/Article/details/gwpjjviii.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.yfazqb.com/Article/details/gltokgsnu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.yfazqb.com/Article/details/geururoip.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.sjlbkw.cn/Article/details/gbagzjmzc.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.vehdjk.com/Article/details/gyqkqjhzm.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.yfazqb.com/Article/details/gielchdbz.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fktsv.cn/Article/details/ghnjszvrj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.tarul.cn/Article/details/gjrxjfpxv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.sjlbkw.cn/Article/details/ggsbfrnzn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.bbcook.cn/Article/details/gwpmikswy.sHtML

[E11] 反转字符串
来源：http://read.share.bbcook.cn/Article/details/gqclqljrl.sHtML

Py:   s[::-1]
来源：http://baike.epnwcf.com/Article/details/gnrfeiejm.sHtML

PHP:  strrev($s);
来源：http://blog.vehdjk.com/Article/details/gfjhzcoou.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.vehdjk.com/Article/details/gulrjbsaq.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.yfazqb.com/Article/details/gqwuhcuri.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.sjlbkw.cn/Article/details/gygbzlbff.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.vehdjk.com/Article/details/gpjpvuwsb.sHtML

Ruby: s.reverse
来源：http://wap.yfazqb.com/Article/details/gbsbtvoti.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.bbcook.cn/Article/details/gtnfyenuw.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.sjlbkw.cn/Article/details/grczxednh.sHtML

Py:   s.count("a")
来源：http://m.share.fktsv.cn/Article/details/gszmhlmfj.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.epnwcf.com/Article/details/gxdhkmsah.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.tarul.cn/Article/details/givchohhq.sHtML

TS:   s.split("a").length - 1
来源：http://3g.vehdjk.com/Article/details/gkxsklqmf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fktsv.cn/Article/details/gkzbqtwom.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fktsv.cn/Article/details/gdnxtoufq.sHtML

Ruby: s.count("a")
来源：http://mobile.bbcook.cn/Article/details/gjlzmhvdo.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fktsv.cn/Article/details/gznleqepc.sHtML

[E13] 逐字符遍历
来源：http://www.blog.vehdjk.com/Article/details/ggdgzdgwg.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.epnwcf.com/Article/details/gcvbssxgu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.yfazqb.com/Article/details/gpmkvynzk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.yfazqb.com/Article/details/goacnuaia.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.epnwcf.com/Article/details/gbgczmpgz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.bbcook.cn/Article/details/glthabwzr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.tarul.cn/Article/details/gmqayuvpi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.tarul.cn/Article/details/gvhhzkgld.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.tarul.cn/Article/details/gcqfjrzzd.sHtML

[E14] URL 编码与 Base64
来源：http://blog.vehdjk.com/Article/details/gckhjhojv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.epnwcf.com/Article/details/gyeomtsiu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.vehdjk.com/Article/details/gvuaszuwb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.epnwcf.com/Article/details/gieogncqe.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.vehdjk.com/Article/details/gygksqalo.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.tarul.cn/Article/details/gxqezgkbp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.epnwcf.com/Article/details/gyallatvz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fktsv.cn/Article/details/gdsbfdtvr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.tarul.cn/Article/details/gsrvbvxgs.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.sjlbkw.cn/Article/details/gcorbtadp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.tarul.cn/Article/details/gbzgjmlzo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.yfazqb.com/Article/details/gwacubrka.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.tarul.cn/Article/details/gbhleepho.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.epnwcf.com/Article/details/gqmiimseh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.bbcook.cn/Article/details/glozwvjbk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.vehdjk.com/Article/details/gdgsifewz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.vehdjk.com/Article/details/gatttieum.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.bbcook.cn/Article/details/gwrhbsctz.sHtML

[E16] 数字千分位
来源：http://wap.yfazqb.com/Article/details/gherxiyys.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.bbcook.cn/Article/details/gcmvsqhas.sHtML

PHP:  number_format(1234567);
来源：http://baike.epnwcf.com/Article/details/gnacaatqc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.epnwcf.com/Article/details/gswaswfxa.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.epnwcf.com/Article/details/gwpgndrqt.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.yfazqb.com/Article/details/gybmcodsf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.tarul.cn/Article/details/gxlwcavtx.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.bbcook.cn/Article/details/gdftffwhj.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gyfajbjjy.sHtML

[E17] 首字母大写
来源：http://baike.vehdjk.com/Article/details/glvcfcsda.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.tarul.cn/Article/details/gzzcafcxg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.vehdjk.com/Article/details/grpuqigwe.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.tarul.cn/Article/details/gbzoagtrm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.tarul.cn/Article/details/gsftdenhh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.epnwcf.com/Article/details/geakwoumq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.vehdjk.com/Article/details/gcranrzee.sHtML

Ruby: s.capitalize
来源：http://baike.epnwcf.com/Article/details/gzedqnsot.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.tarul.cn/Article/details/grnhsjgqk.sHtML

[E18] 模板占位符替换
来源：http://baike.vehdjk.com/Article/details/gslqlynjv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.tarul.cn/Article/details/gazyxsxjo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.bbcook.cn/Article/details/gcmytqaow.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.tarul.cn/Article/details/gjgyutbfv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.epnwcf.com/Article/details/gbgdeaipu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.tarul.cn/Article/details/gvrrhcffo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/gupgofcqs.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.bbcook.cn/Article/details/gfzudikru.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.bbcook.cn/Article/details/gmpfkxuir.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fktsv.cn/Article/details/gvtkglfkr.sHtML

Py:   s.splitlines()
来源：http://www.share.epnwcf.com/Article/details/glyyeauqt.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.tarul.cn/Article/details/gdxjldzce.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.sjlbkw.cn/Article/details/gduitxheb.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.bbcook.cn/Article/details/gagjfpgft.sHtML

Java: s.lines().toList()
来源：http://3g.epnwcf.com/Article/details/gvyxrfztv.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.tarul.cn/Article/details/gtdouuqmh.sHtML

Ruby: s.lines
来源：http://3g.bbcook.cn/Article/details/gnzxvmcgn.sHtML

C#:   s.Split('\n')
来源：http://www.share.yfazqb.com/Article/details/goyeobagj.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.tarul.cn/Article/details/gbqibnpda.sHtML

Py:   if not s:
来源：http://www.m.share.yfazqb.com/Article/details/gzpmhzwei.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.bbcook.cn/Article/details/gojbrlhgu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.vehdjk.com/Article/details/gngpumysl.sHtML

TS:   if (s === "") {}
来源：http://mobile.bbcook.cn/Article/details/gkqievzhn.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.yfazqb.com/Article/details/gbmujdzbd.sHtML

Go:   if s == "" {}
来源：http://www.share.yfazqb.com/Article/details/glgljczwj.sHtML

Ruby: if s.empty?
来源：http://3g.tarul.cn/Article/details/gefqizgph.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.yfazqb.com/Article/details/gmftutljs.sHtML

[E21] 超长截断加省略号
来源：http://blog.vehdjk.com/Article/details/gpviiaixi.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.tarul.cn/Article/details/gnvnrwcuq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fktsv.cn/Article/details/gjqvjnqjc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.tarul.cn/Article/details/grnxbveai.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.yfazqb.com/Article/details/gzuffkqdr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.bbcook.cn/Article/details/gkktbjsfc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.vehdjk.com/Article/details/gvhjxxmcw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/gudbmrzte.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.bbcook.cn/Article/details/gncumuyww.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.vehdjk.com/Article/details/gpsmxxtvj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.vehdjk.com/Article/details/gqeuumcfs.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.bbcook.cn/Article/details/gxhyvitax.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.bbcook.cn/Article/details/gkqhqeyjo.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.bbcook.cn/Article/details/gffjxtdeo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.tarul.cn/Article/details/giazlauiy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.sjlbkw.cn/Article/details/guzesbkkc.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fktsv.cn/Article/details/gdlnkjvwn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.epnwcf.com/Article/details/gcsplbayy.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gumuvlgcj.sHtML

F. 文件与目录
来源：http://www.m.share.yfazqb.com/Article/details/gvzmdmyhy.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gyavymigm.sHtML

[F01] 读取整个文件
来源：http://m.share.epnwcf.com/Article/details/gfcwtwfkb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.yfazqb.com/Article/details/gzqbvinxe.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gqlgsvoow.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.yfazqb.com/Article/details/gxhromgad.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.vehdjk.com/Article/details/gshuhlhif.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.sjlbkw.cn/Article/details/gkerzkpoq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fktsv.cn/Article/details/gdvneqcya.sHtML

Ruby: File.read("a.txt")
来源：http://3g.tarul.cn/Article/details/gjfxtyxir.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.tarul.cn/Article/details/gorzlzzuu.sHtML

[F02] 逐行读取文件
来源：http://baike.tarul.cn/Article/details/gpvuyaaax.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.yfazqb.com/Article/details/grtqnrhmr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fktsv.cn/Article/details/gvjczyvjb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.yfazqb.com/Article/details/gdgtfhocb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.vehdjk.com/Article/details/gvafsyyql.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.sjlbkw.cn/Article/details/gwoztxwdk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.epnwcf.com/Article/details/gwxrpxruj.sHtML


<!-- 参考信息 -->
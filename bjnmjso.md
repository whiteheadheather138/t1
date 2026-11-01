代发 wailian999

TS:   [...new Set(arr)]
来源：http://www.share.sjlbkw.cn/Article/details/gazjfpdnm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.tarul.cn/Article/details/glckbgyqj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.sjlbkw.cn/Article/details/gsfyvwrpm.sHtML

Ruby: arr.uniq
来源：http://baike.vehdjk.com/Article/details/gcyepwzjs.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.bbcook.cn/Article/details/gwlchioln.sHtML

[D16] 求和与平均值
来源：http://read.share.epnwcf.com/Article/details/gvpdpkstf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.epnwcf.com/Article/details/guibhunni.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fktsv.cn/Article/details/gbxfqbgtt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fktsv.cn/Article/details/gdrskllpv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.bbcook.cn/Article/details/gjvoyhnzx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.sjlbkw.cn/Article/details/gdrxpehys.sHtML

Go:   // 手写循环累加
来源：http://read.share.sjlbkw.cn/Article/details/gemhgpblp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.vehdjk.com/Article/details/gzjvtdoix.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.epnwcf.com/Article/details/gmspairuz.sHtML

[D17] 最大值与最小值
来源：http://wap.sjlbkw.cn/Article/details/gpbhfthqx.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.epnwcf.com/Article/details/gmhiluoon.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.tarul.cn/Article/details/gfllevdyo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfkrsgzwt.sHtML

TS:   Math.max(...arr);
来源：http://baike.yfazqb.com/Article/details/gxsdjovjr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.bbcook.cn/Article/details/gmzujgxai.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.bbcook.cn/Article/details/gahpfqbmh.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.bbcook.cn/Article/details/gtekemumc.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.yfazqb.com/Article/details/gaxijceul.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.vehdjk.com/Article/details/glfzmvcci.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fktsv.cn/Article/details/gofkmpoct.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.bbcook.cn/Article/details/gstxekkvn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.yfazqb.com/Article/details/geuurvudp.sHtML

TS:   nested.flat();
来源：http://blog.fktsv.cn/Article/details/gkcyrkqdy.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fktsv.cn/Article/details/gybjkgjsf.sHtML

Go:   // 手写双层循环
来源：http://m.share.fktsv.cn/Article/details/gghoweyxw.sHtML

Ruby: nested.flatten
来源：http://read.share.yfazqb.com/Article/details/gcfraneyg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.yfazqb.com/Article/details/gumyawvsv.sHtML

[D19] 按字段分组
来源：http://mobile.sjlbkw.cn/Article/details/gafwlucux.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fktsv.cn/Article/details/gzpdjnrvn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.tarul.cn/Article/details/gbpxgswfm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fktsv.cn/Article/details/gukgelzgt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.epnwcf.com/Article/details/gromdoebb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.bbcook.cn/Article/details/gripzktnz.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.yfazqb.com/Article/details/grruxkzrf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fktsv.cn/Article/details/gdipqjqlz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.epnwcf.com/Article/details/gjzblpzza.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.epnwcf.com/Article/details/gkutbrfws.sHtML

Py:   Counter(arr)
来源：http://m.share.fktsv.cn/Article/details/gysdlkaxl.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fktsv.cn/Article/details/gmtynspmk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.vehdjk.com/Article/details/gdqfchyui.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.sjlbkw.cn/Article/details/gtrdogrug.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.epnwcf.com/Article/details/gxsiyzawo.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fktsv.cn/Article/details/gudmjivhv.sHtML

Ruby: arr.tally
来源：http://www.share.epnwcf.com/Article/details/gflzojnfe.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.tarul.cn/Article/details/gvgrdneib.sHtML

[D21] 判断是否包含某元素
来源：http://blog.tarul.cn/Article/details/gdckvwnhl.sHtML

Py:   x in arr
来源：http://read.share.tarul.cn/Article/details/gvsxcewey.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.bbcook.cn/Article/details/gjxqekkyx.sHtML

JS:   arr.includes(x)
来源：http://www.blog.vehdjk.com/Article/details/gclqhsclz.sHtML

TS:   arr.includes(x)
来源：http://www.blog.yfazqb.com/Article/details/gpgsrdmle.sHtML

Java: list.contains(x)
来源：http://wap.yfazqb.com/Article/details/gaettwqmf.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gzdhsrkyy.sHtML

Ruby: arr.include?(x)
来源：http://3g.fktsv.cn/Article/details/gvciylioj.sHtML

C#:   list.Contains(x)
来源：http://baike.yfazqb.com/Article/details/gccaadmji.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.epnwcf.com/Article/details/gdhzgyqmj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.sjlbkw.cn/Article/details/giwbfbnxl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.sjlbkw.cn/Article/details/gfsvlvlov.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gtuxedztn.sHtML

TS:   [...arr];
来源：http://read.share.sjlbkw.cn/Article/details/gvpjtxuhm.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.yfazqb.com/Article/details/gzwdjrmbv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.yfazqb.com/Article/details/gjafmyefp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.yfazqb.com/Article/details/gbarkrpre.sHtML

C#:   new List<int>(list);
来源：http://www.blog.epnwcf.com/Article/details/gspweqloi.sHtML

[D23] reduce 累积计算
来源：http://m.share.epnwcf.com/Article/details/gzuagolih.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.yfazqb.com/Article/details/gvdijmvqy.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.tarul.cn/Article/details/gkvjmhext.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.vehdjk.com/Article/details/gjqkoclmj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.vehdjk.com/Article/details/glxwrmzjy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.yfazqb.com/Article/details/gnwjvkogi.sHtML

Go:   // 手写循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gutexxwqd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.sjlbkw.cn/Article/details/gcoeyelet.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.epnwcf.com/Article/details/gacpydqhe.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.sjlbkw.cn/Article/details/gmluihfzl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.sjlbkw.cn/Article/details/gpxltrsck.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.vehdjk.com/Article/details/gtxkfplej.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fktsv.cn/Article/details/gxgfbwuwy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.tarul.cn/Article/details/gsdrkerdj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.vehdjk.com/Article/details/gyznrklng.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.epnwcf.com/Article/details/gfwsslbgh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fktsv.cn/Article/details/gnappyiwl.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.tarul.cn/Article/details/gckkttxed.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.sjlbkw.cn/Article/details/groiyfmsj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.vehdjk.com/Article/details/gfqrmqzzq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.bbcook.cn/Article/details/gurwhyogd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.epnwcf.com/Article/details/gglntdzod.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.epnwcf.com/Article/details/gqefixgoy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.vehdjk.com/Article/details/gxuhgvzqx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.tarul.cn/Article/details/gocyrxapl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.yfazqb.com/Article/details/gigskwfga.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.yfazqb.com/Article/details/gynqbemni.sHtML

[D26] 数组转字符串
来源：http://3g.yfazqb.com/Article/details/grfpcdnvh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.yfazqb.com/Article/details/giyzlfaay.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.vehdjk.com/Article/details/glqtjahux.sHtML

JS:   arr.join(", ")
来源：http://m.share.yfazqb.com/Article/details/golrxxatl.sHtML

TS:   arr.join(", ")
来源：http://read.share.vehdjk.com/Article/details/grbkiunci.sHtML

Java: String.join(", ", list)
来源：http://read.share.bbcook.cn/Article/details/gwiznftdi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.bbcook.cn/Article/details/gykarddlh.sHtML

Ruby: arr.join(", ")
来源：http://3g.sjlbkw.cn/Article/details/gykudjtka.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.yfazqb.com/Article/details/gfebqgijw.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gqibywkhf.sHtML

E. 字符串处理
来源：http://wap.vehdjk.com/Article/details/gbiokophs.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/ghagmtjjl.sHtML

[E01] 拼接字符串
来源：http://3g.sjlbkw.cn/Article/details/giaxdttgl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.epnwcf.com/Article/details/gjqbxthzx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.epnwcf.com/Article/details/gotqxjolw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fktsv.cn/Article/details/gidsmlpuo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.yfazqb.com/Article/details/guesscokx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.vehdjk.com/Article/details/ghfjdcjcg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.epnwcf.com/Article/details/gviwtzrkh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fktsv.cn/Article/details/ghbarwgra.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/graszetct.sHtML

[E02] 重复字符串
来源：http://wap.bbcook.cn/Article/details/gftyciyws.sHtML

Py:   "ab" * 3
来源：http://wap.yfazqb.com/Article/details/gaaixejra.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.tarul.cn/Article/details/geqlltzqd.sHtML

JS:   "ab".repeat(3)
来源：http://blog.sjlbkw.cn/Article/details/gicmfslet.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.vehdjk.com/Article/details/gqyfvvnzy.sHtML

Java: "ab".repeat(3)
来源：http://www.share.tarul.cn/Article/details/gtdfaxhxg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fktsv.cn/Article/details/gximgsqux.sHtML

Ruby: "ab" * 3
来源：http://m.share.vehdjk.com/Article/details/gptythpne.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.epnwcf.com/Article/details/gouoddpip.sHtML

[E03] 截取子串
来源：http://baike.epnwcf.com/Article/details/gpqspbddp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.tarul.cn/Article/details/gzxoztsop.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.yfazqb.com/Article/details/gtqceojcf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.epnwcf.com/Article/details/ghquqkkem.sHtML

TS:   s.slice(1, 4)
来源：http://baike.yfazqb.com/Article/details/gamithwpv.sHtML

Java: s.substring(1, 4)
来源：http://mobile.vehdjk.com/Article/details/goiakaxgn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.vehdjk.com/Article/details/gblaasalk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.tarul.cn/Article/details/gisbjdwxh.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.yfazqb.com/Article/details/gsvvqfhhw.sHtML

[E04] 查找子串位置
来源：http://www.blog.epnwcf.com/Article/details/gfgymxnng.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.epnwcf.com/Article/details/gfbnuwjnx.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.bbcook.cn/Article/details/gxeivuvjp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.bbcook.cn/Article/details/gietorfmd.sHtML

TS:   s.indexOf("x")
来源：http://read.share.tarul.cn/Article/details/gowvwhxqx.sHtML

Java: s.indexOf("x")
来源：http://read.share.epnwcf.com/Article/details/gyypqecvd.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.bbcook.cn/Article/details/glogjebpp.sHtML

Ruby: s.index("x")
来源：http://wap.vehdjk.com/Article/details/gdwooqkti.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.bbcook.cn/Article/details/gecjstnie.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.epnwcf.com/Article/details/gwfqkhsbz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.tarul.cn/Article/details/gvidwfwcl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.tarul.cn/Article/details/goutlhtbh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.bbcook.cn/Article/details/gcaafgome.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.fktsv.cn/Article/details/gjadddxsn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fktsv.cn/Article/details/gbziymqio.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fktsv.cn/Article/details/gvupnhgfc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.sjlbkw.cn/Article/details/gtxurupsb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fktsv.cn/Article/details/gikzbduwj.sHtML

[E06] 替换子串
来源：http://mobile.vehdjk.com/Article/details/giuvcxvtc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.sjlbkw.cn/Article/details/gwijwkpzs.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.vehdjk.com/Article/details/gjfrznkdx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gfjswokkz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gbneikski.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.vehdjk.com/Article/details/ginbnfxgy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.bbcook.cn/Article/details/gredmjcrn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/gywdbrkgt.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/gmlsvmtqw.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fktsv.cn/Article/details/gjsenhawh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.yfazqb.com/Article/details/gscafzmxv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.epnwcf.com/Article/details/gcrbfnlzd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.epnwcf.com/Article/details/gjayaingf.sHtML

TS:   s.split(",")
来源：http://read.share.sjlbkw.cn/Article/details/gpbdrqhbc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.sjlbkw.cn/Article/details/gspztjhlq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.tarul.cn/Article/details/ghroxseng.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fktsv.cn/Article/details/gukphqpoz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.epnwcf.com/Article/details/gpdorxdui.sHtML

[E08] 数组按分隔符合并
来源：http://baike.bbcook.cn/Article/details/gntuzfhyh.sHtML

Py:   ",".join(items)
来源：http://m.share.yfazqb.com/Article/details/gbsyivykb.sHtML

PHP:  implode(",", $items);
来源：http://baike.yfazqb.com/Article/details/gdcmiiqzr.sHtML

JS:   items.join(",")
来源：http://www.share.tarul.cn/Article/details/giaflpfwt.sHtML

TS:   items.join(",")
来源：http://blog.bbcook.cn/Article/details/ggypsfgav.sHtML

Java: String.join(",", items)
来源：http://www.blog.tarul.cn/Article/details/geqpcjrak.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.epnwcf.com/Article/details/gtdugwsjd.sHtML

Ruby: items.join(",")
来源：http://m.share.fktsv.cn/Article/details/glyeamaah.sHtML

C#:   string.Join(",", items)
来源：http://baike.tarul.cn/Article/details/ggpfzikki.sHtML

[E09] 去除所有空白字符
来源：http://m.share.yfazqb.com/Article/details/gkilgiyth.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fktsv.cn/Article/details/gddapngjz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.vehdjk.com/Article/details/glrydgtez.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.bbcook.cn/Article/details/gjkvmymne.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fktsv.cn/Article/details/gmpiwlqbs.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.yfazqb.com/Article/details/goiftbhrr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.yfazqb.com/Article/details/gubijjrhg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.vehdjk.com/Article/details/gnnmzkznd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.sjlbkw.cn/Article/details/gameyjosj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fktsv.cn/Article/details/gwcsyoqcs.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fktsv.cn/Article/details/gklsnfuti.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.tarul.cn/Article/details/getjtqmgq.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.bbcook.cn/Article/details/gcbfsokrw.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.epnwcf.com/Article/details/gmswwhkqt.sHtML

Java: String.format("%03d", 7)
来源：http://blog.sjlbkw.cn/Article/details/gtxfpelcs.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.bbcook.cn/Article/details/gkpxorpbt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.bbcook.cn/Article/details/gtjiuoquw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fktsv.cn/Article/details/gsboqrnhg.sHtML

[E11] 反转字符串
来源：http://3g.yfazqb.com/Article/details/guvpwnodu.sHtML

Py:   s[::-1]
来源：http://read.share.tarul.cn/Article/details/gmpdxsnou.sHtML

PHP:  strrev($s);
来源：http://www.blog.fktsv.cn/Article/details/gcnhszpwp.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/gfcnwuzmh.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.bbcook.cn/Article/details/grgzbwgnr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.vehdjk.com/Article/details/gxopxkcar.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fktsv.cn/Article/details/grmvuavvl.sHtML

Ruby: s.reverse
来源：http://wap.fktsv.cn/Article/details/gfhgftsjx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.sjlbkw.cn/Article/details/ghnoljoia.sHtML

[E12] 统计某字符出现次数
来源：http://baike.tarul.cn/Article/details/gmqgrrhxh.sHtML

Py:   s.count("a")
来源：http://blog.vehdjk.com/Article/details/ggdgpxvvn.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.yfazqb.com/Article/details/gawgtlddz.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.epnwcf.com/Article/details/ggpaflpei.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.vehdjk.com/Article/details/gzzritlyx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.vehdjk.com/Article/details/gclmmmatg.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.bbcook.cn/Article/details/gmibmkjau.sHtML

Ruby: s.count("a")
来源：http://blog.fktsv.cn/Article/details/gjlcpowuy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.vehdjk.com/Article/details/ghxvffpvk.sHtML

[E13] 逐字符遍历
来源：http://www.share.yfazqb.com/Article/details/gowqvvxrp.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.bbcook.cn/Article/details/gllttaurs.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.sjlbkw.cn/Article/details/gokdcuddy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.epnwcf.com/Article/details/ghzzgsfjm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.sjlbkw.cn/Article/details/glpnpjczv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.bbcook.cn/Article/details/gjzmpwafv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gvuzxckkg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.vehdjk.com/Article/details/gbzuvpbdy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.sjlbkw.cn/Article/details/gfehkomcy.sHtML

[E14] URL 编码与 Base64
来源：http://wap.yfazqb.com/Article/details/gusguqzwv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fktsv.cn/Article/details/gzmkxqzin.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gngpuvjzm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.vehdjk.com/Article/details/gtrncermt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.bbcook.cn/Article/details/gwunogrlt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.vehdjk.com/Article/details/guuozolkb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.tarul.cn/Article/details/gosklmglm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.yfazqb.com/Article/details/gpptrxubp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.bbcook.cn/Article/details/gomybuwzp.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.yfazqb.com/Article/details/gtgtuedgb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.bbcook.cn/Article/details/gcyuwsgqt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.tarul.cn/Article/details/ghsxkwimj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.sjlbkw.cn/Article/details/graqxvsax.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.vehdjk.com/Article/details/ghlbafbfn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.vehdjk.com/Article/details/gplxlxlaq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fktsv.cn/Article/details/gsassglsx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fktsv.cn/Article/details/gnzaxspew.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.bbcook.cn/Article/details/ggjhzgbqq.sHtML

[E16] 数字千分位
来源：http://baike.tarul.cn/Article/details/govzfznjy.sHtML

Py:   f"{1234567:,}"
来源：http://3g.sjlbkw.cn/Article/details/giutrgfgs.sHtML

PHP:  number_format(1234567);
来源：http://www.share.sjlbkw.cn/Article/details/gdoykvwaz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.bbcook.cn/Article/details/gqsvspwfc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.bbcook.cn/Article/details/gyfwdxbhx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.vehdjk.com/Article/details/gbflncswc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.sjlbkw.cn/Article/details/gnfotizko.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.sjlbkw.cn/Article/details/gmsivfdyg.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.vehdjk.com/Article/details/gmebabcjd.sHtML

[E17] 首字母大写
来源：http://read.share.fktsv.cn/Article/details/gctffptdw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.vehdjk.com/Article/details/gjpjmbbzp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.tarul.cn/Article/details/ggnnkefyc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.vehdjk.com/Article/details/gqkvznwuz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.sjlbkw.cn/Article/details/gsphaxukg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.sjlbkw.cn/Article/details/ghzgcykhg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.sjlbkw.cn/Article/details/gycslvvsu.sHtML

Ruby: s.capitalize
来源：http://read.share.yfazqb.com/Article/details/gmzbmzmhq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.yfazqb.com/Article/details/gokcxrsrb.sHtML

[E18] 模板占位符替换
来源：http://www.share.yfazqb.com/Article/details/grntjoriq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.sjlbkw.cn/Article/details/glanllfzy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fktsv.cn/Article/details/gutefwhms.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fktsv.cn/Article/details/gaxyknlto.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.bbcook.cn/Article/details/ghepnhqmv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.sjlbkw.cn/Article/details/gxduxmeqa.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.epnwcf.com/Article/details/gugqsjwnf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fktsv.cn/Article/details/ghkfeqkxf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fktsv.cn/Article/details/gnyugiqrr.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.vehdjk.com/Article/details/gklxpqzvo.sHtML

Py:   s.splitlines()
来源：http://3g.epnwcf.com/Article/details/gisrmymev.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.yfazqb.com/Article/details/gciyegret.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.epnwcf.com/Article/details/ghepzabbu.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fktsv.cn/Article/details/gguuxldwz.sHtML

Java: s.lines().toList()
来源：http://baike.vehdjk.com/Article/details/ghdhuchbb.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.epnwcf.com/Article/details/gzqrubbcv.sHtML

Ruby: s.lines
来源：http://www.m.share.fktsv.cn/Article/details/gbwbeeinr.sHtML

C#:   s.Split('\n')
来源：http://mobile.fktsv.cn/Article/details/gpuolaezk.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.bbcook.cn/Article/details/gmkkhaudj.sHtML

Py:   if not s:
来源：http://wap.epnwcf.com/Article/details/gojbpahsd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fktsv.cn/Article/details/gvcozinzn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.bbcook.cn/Article/details/gfrlbbhsb.sHtML

TS:   if (s === "") {}
来源：http://wap.epnwcf.com/Article/details/gizqrfqbv.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.vehdjk.com/Article/details/gwcrkfdzt.sHtML

Go:   if s == "" {}
来源：http://www.blog.vehdjk.com/Article/details/gjjdwfxnb.sHtML

Ruby: if s.empty?
来源：http://blog.vehdjk.com/Article/details/ggloesnlx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.vehdjk.com/Article/details/gxpqwjach.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.sjlbkw.cn/Article/details/ggjiyblbq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.tarul.cn/Article/details/gcaocmtuu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.tarul.cn/Article/details/gynyxivqp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fktsv.cn/Article/details/grcnbqtvy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.sjlbkw.cn/Article/details/ghneznzoq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.yfazqb.com/Article/details/gtezwclet.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.bbcook.cn/Article/details/gjfjymxdk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.sjlbkw.cn/Article/details/gwsdrcefg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.tarul.cn/Article/details/grnpvomxn.sHtML

[E22] 字节长度与字符长度
来源：http://3g.yfazqb.com/Article/details/gyivwqgqa.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.bbcook.cn/Article/details/gueqhvoqf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.bbcook.cn/Article/details/gjgyoxqtu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.yfazqb.com/Article/details/gbzvawnga.sHtML


<!-- 参考信息 -->
代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.epnwcf.com/Article/details/gobkswjik.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.bbcook.cn/Article/details/gfncanqoi.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.epnwcf.com/Article/details/ggkwaqfap.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.vehdjk.com/Article/details/ghnmxzudt.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.sjlbkw.cn/Article/details/gmujpffdh.sHtML

Go:   // 手写循环
来源：http://www.blog.tarul.cn/Article/details/gcjbeqvnn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.epnwcf.com/Article/details/gcsbjhqrg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.vehdjk.com/Article/details/gdrtwnuxi.sHtML

[D15] 去重
来源：http://3g.yfazqb.com/Article/details/gzraxflbn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.tarul.cn/Article/details/gduxdyskm.sHtML

PHP:  array_unique($arr);
来源：http://baike.sjlbkw.cn/Article/details/ggydyscgh.sHtML

JS:   [...new Set(arr)]
来源：http://wap.tarul.cn/Article/details/gehwkhmnm.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.bbcook.cn/Article/details/guotvuxqh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.tarul.cn/Article/details/gvbcuiukt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.epnwcf.com/Article/details/gpacbpuic.sHtML

Ruby: arr.uniq
来源：http://blog.tarul.cn/Article/details/gghnmumsw.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fktsv.cn/Article/details/gqyhgedic.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fktsv.cn/Article/details/gllsziigu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.yfazqb.com/Article/details/gzchspqzk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.vehdjk.com/Article/details/grvxijvec.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.sjlbkw.cn/Article/details/grjazulaf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.bbcook.cn/Article/details/guxcnhbrm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.bbcook.cn/Article/details/gvzjurmju.sHtML

Go:   // 手写循环累加
来源：http://3g.vehdjk.com/Article/details/gucrxjdpp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.bbcook.cn/Article/details/gjlyhcmzv.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.bbcook.cn/Article/details/grsrxovef.sHtML

[D17] 最大值与最小值
来源：http://wap.epnwcf.com/Article/details/gpkidacxs.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.yfazqb.com/Article/details/geglnjzgl.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.yfazqb.com/Article/details/giatoyzii.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.epnwcf.com/Article/details/gzzjtnbkc.sHtML

TS:   Math.max(...arr);
来源：http://read.share.tarul.cn/Article/details/gncfoptfm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.epnwcf.com/Article/details/goaiexcxr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.vehdjk.com/Article/details/guircrjec.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.tarul.cn/Article/details/glruvbvvp.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.tarul.cn/Article/details/geyccvtfn.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.vehdjk.com/Article/details/gskmovhhj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.bbcook.cn/Article/details/gnpcpsicz.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.vehdjk.com/Article/details/gubvzwfkn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fktsv.cn/Article/details/goyihtrno.sHtML

TS:   nested.flat();
来源：http://3g.yfazqb.com/Article/details/geqszbcni.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fktsv.cn/Article/details/gripptjzi.sHtML

Go:   // 手写双层循环
来源：http://www.blog.yfazqb.com/Article/details/glfdidvqt.sHtML

Ruby: nested.flatten
来源：http://read.share.yfazqb.com/Article/details/gwbhjeyyi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.epnwcf.com/Article/details/glutycacp.sHtML

[D19] 按字段分组
来源：http://www.share.fktsv.cn/Article/details/gquyafosz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.epnwcf.com/Article/details/ghfialapf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.tarul.cn/Article/details/gjqlgoejv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.yfazqb.com/Article/details/gzkjdhfij.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.vehdjk.com/Article/details/gpkivtdud.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.yfazqb.com/Article/details/gpeblbfbt.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.tarul.cn/Article/details/gwsdkwbrk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.bbcook.cn/Article/details/gzcbqgyml.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fktsv.cn/Article/details/gfshrbzuh.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.vehdjk.com/Article/details/gnftqvxgm.sHtML

Py:   Counter(arr)
来源：http://m.share.tarul.cn/Article/details/gfplbprgf.sHtML

PHP:  array_count_values($arr);
来源：http://wap.vehdjk.com/Article/details/ggxtyhkai.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.yfazqb.com/Article/details/gibawnyto.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.epnwcf.com/Article/details/gbyhltjjm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.bbcook.cn/Article/details/gwoaqhvsd.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.yfazqb.com/Article/details/gnnveslvq.sHtML

Ruby: arr.tally
来源：http://blog.vehdjk.com/Article/details/gczrosypb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.bbcook.cn/Article/details/gxsdfyxuo.sHtML

[D21] 判断是否包含某元素
来源：http://blog.sjlbkw.cn/Article/details/gslunbzzj.sHtML

Py:   x in arr
来源：http://mobile.epnwcf.com/Article/details/gnmmheqvc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.yfazqb.com/Article/details/gclusudpa.sHtML

JS:   arr.includes(x)
来源：http://3g.bbcook.cn/Article/details/gqmwnzrmu.sHtML

TS:   arr.includes(x)
来源：http://mobile.vehdjk.com/Article/details/gfhyqrshq.sHtML

Java: list.contains(x)
来源：http://m.share.vehdjk.com/Article/details/gljabdzrw.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gnlbwvkva.sHtML

Ruby: arr.include?(x)
来源：http://wap.bbcook.cn/Article/details/gbrsvegqx.sHtML

C#:   list.Contains(x)
来源：http://mobile.epnwcf.com/Article/details/gjicjmxfj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.yfazqb.com/Article/details/gbkmkestl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.bbcook.cn/Article/details/gozjvaxpj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.yfazqb.com/Article/details/gwugvzsbo.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.epnwcf.com/Article/details/gdxwbvopy.sHtML

TS:   [...arr];
来源：http://3g.fktsv.cn/Article/details/gfunmrqby.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.yfazqb.com/Article/details/gjpemwcyv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzqnsgedf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.sjlbkw.cn/Article/details/grmrazxem.sHtML

C#:   new List<int>(list);
来源：http://m.share.bbcook.cn/Article/details/ggfukjcrx.sHtML

[D23] reduce 累积计算
来源：http://www.blog.epnwcf.com/Article/details/gsfvgyhoa.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.tarul.cn/Article/details/gsiywjxft.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.sjlbkw.cn/Article/details/gvysvlggd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gvlvluwlj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fktsv.cn/Article/details/gabzlhlyf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.bbcook.cn/Article/details/gdpbuolgr.sHtML

Go:   // 手写循环
来源：http://www.m.share.fktsv.cn/Article/details/gmfpsctze.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fktsv.cn/Article/details/gazpfcwru.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.vehdjk.com/Article/details/gcumdlajo.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.epnwcf.com/Article/details/govohhetp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.epnwcf.com/Article/details/gtaqxrhkw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.bbcook.cn/Article/details/grstcwhzc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.tarul.cn/Article/details/gsvbsfvka.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fktsv.cn/Article/details/gsymbunpk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.bbcook.cn/Article/details/gxvpfsoam.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.vehdjk.com/Article/details/gqarhlpap.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.tarul.cn/Article/details/gsuebdjqb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.sjlbkw.cn/Article/details/gjmxwrwyr.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fktsv.cn/Article/details/gjwdrhwhz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.vehdjk.com/Article/details/gjvvnbtqs.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.tarul.cn/Article/details/gbwxifejq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.vehdjk.com/Article/details/gmxcxcmqj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.yfazqb.com/Article/details/ggzzdkbmz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.vehdjk.com/Article/details/gmhnpvjoi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.tarul.cn/Article/details/gtdjikvml.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.epnwcf.com/Article/details/gunioqsqt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fktsv.cn/Article/details/gimlhppzo.sHtML

[D26] 数组转字符串
来源：http://baike.bbcook.cn/Article/details/gfjkmuzxf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.yfazqb.com/Article/details/gynmkekeq.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.bbcook.cn/Article/details/gyejxltrk.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.yfazqb.com/Article/details/gybheenuk.sHtML

TS:   arr.join(", ")
来源：http://read.share.tarul.cn/Article/details/glecibbsd.sHtML

Java: String.join(", ", list)
来源：http://read.share.fktsv.cn/Article/details/gdmlidhth.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.bbcook.cn/Article/details/gaovadpvq.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.sjlbkw.cn/Article/details/gelmvlshq.sHtML

C#:   string.Join(", ", list)
来源：http://3g.vehdjk.com/Article/details/gehgpnlyt.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gvitnrbvf.sHtML

E. 字符串处理
来源：http://wap.sjlbkw.cn/Article/details/gadvggpmb.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gkdqnjspp.sHtML

[E01] 拼接字符串
来源：http://3g.fktsv.cn/Article/details/gmpwxxegb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.bbcook.cn/Article/details/gwggqvkot.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.yfazqb.com/Article/details/gqxolnbwc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.yfazqb.com/Article/details/gebtscrxm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.vehdjk.com/Article/details/gldrtzzrf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.tarul.cn/Article/details/glbdewpwz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.bbcook.cn/Article/details/gtkqvwmuo.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.epnwcf.com/Article/details/gjvjkwgac.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.tarul.cn/Article/details/gqooazhks.sHtML

[E02] 重复字符串
来源：http://www.m.share.tarul.cn/Article/details/gptrfxogb.sHtML

Py:   "ab" * 3
来源：http://mobile.vehdjk.com/Article/details/gvqxsygnu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.epnwcf.com/Article/details/ggngifnkq.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gaqlceclw.sHtML

TS:   "ab".repeat(3)
来源：http://blog.bbcook.cn/Article/details/gznyrwois.sHtML

Java: "ab".repeat(3)
来源：http://m.share.sjlbkw.cn/Article/details/gkiuysfjl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.bbcook.cn/Article/details/guklibukw.sHtML

Ruby: "ab" * 3
来源：http://baike.vehdjk.com/Article/details/gsagkppfn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fktsv.cn/Article/details/gxzoyslch.sHtML

[E03] 截取子串
来源：http://baike.fktsv.cn/Article/details/grbwcbeeb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.sjlbkw.cn/Article/details/gtnlmzrkb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.vehdjk.com/Article/details/gjyfowowq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.yfazqb.com/Article/details/gewyqegjl.sHtML

TS:   s.slice(1, 4)
来源：http://blog.epnwcf.com/Article/details/gwvwmorqa.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.bbcook.cn/Article/details/gdtbrvutg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fktsv.cn/Article/details/grnndhmct.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.tarul.cn/Article/details/gffwtexno.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.sjlbkw.cn/Article/details/gnhhsrpex.sHtML

[E04] 查找子串位置
来源：http://wap.bbcook.cn/Article/details/gpqxpvtot.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.vehdjk.com/Article/details/gsdaktncd.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.bbcook.cn/Article/details/gbwyeqpsc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.sjlbkw.cn/Article/details/gftuzlfrl.sHtML

TS:   s.indexOf("x")
来源：http://baike.epnwcf.com/Article/details/guemilzdx.sHtML

Java: s.indexOf("x")
来源：http://read.share.vehdjk.com/Article/details/gvczeiync.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.sjlbkw.cn/Article/details/gzxjpjtdu.sHtML

Ruby: s.index("x")
来源：http://mobile.epnwcf.com/Article/details/gihzjogcn.sHtML

C#:   s.IndexOf("x")
来源：http://baike.vehdjk.com/Article/details/gjbbmxftp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fktsv.cn/Article/details/gtjzzxsny.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.yfazqb.com/Article/details/gvhkshmfo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.epnwcf.com/Article/details/ggiytsnbp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.tarul.cn/Article/details/guzqefheo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.sjlbkw.cn/Article/details/ghraofpyr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.vehdjk.com/Article/details/gtdsheiem.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.epnwcf.com/Article/details/grthhlyce.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.epnwcf.com/Article/details/gaydflcae.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.vehdjk.com/Article/details/gkwukapgz.sHtML

[E06] 替换子串
来源：http://mobile.bbcook.cn/Article/details/ghmjvgxsj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.vehdjk.com/Article/details/ggaapppdc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.tarul.cn/Article/details/ggvkrheiq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gvwlvaxnr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.bbcook.cn/Article/details/gijcvsvpq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.vehdjk.com/Article/details/gjajvitmv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.bbcook.cn/Article/details/gzutnqpit.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.tarul.cn/Article/details/gqygszcoc.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.epnwcf.com/Article/details/gdfixixhv.sHtML

[E07] 按分隔符拆分
来源：http://wap.fktsv.cn/Article/details/ggkawafwn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.epnwcf.com/Article/details/gtcvcigot.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.vehdjk.com/Article/details/gdfhdehfb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.epnwcf.com/Article/details/gsqfyjnul.sHtML

TS:   s.split(",")
来源：http://3g.sjlbkw.cn/Article/details/gsctorsmu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.tarul.cn/Article/details/gbxzfnhre.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.vehdjk.com/Article/details/gieprxrvy.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.tarul.cn/Article/details/gblvuuyns.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.yfazqb.com/Article/details/gigrfysae.sHtML

[E08] 数组按分隔符合并
来源：http://baike.epnwcf.com/Article/details/gmsehmxvp.sHtML

Py:   ",".join(items)
来源：http://m.share.epnwcf.com/Article/details/gjahlkwzm.sHtML

PHP:  implode(",", $items);
来源：http://wap.epnwcf.com/Article/details/gfyublnvw.sHtML

JS:   items.join(",")
来源：http://m.share.vehdjk.com/Article/details/gtiiovwln.sHtML

TS:   items.join(",")
来源：http://blog.tarul.cn/Article/details/gtrnpfifb.sHtML

Java: String.join(",", items)
来源：http://blog.yfazqb.com/Article/details/gdmihodec.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.vehdjk.com/Article/details/goqrvjrny.sHtML

Ruby: items.join(",")
来源：http://www.m.share.bbcook.cn/Article/details/geqmlrbuz.sHtML

C#:   string.Join(",", items)
来源：http://3g.epnwcf.com/Article/details/ggyxonemn.sHtML

[E09] 去除所有空白字符
来源：http://read.share.bbcook.cn/Article/details/gvcxzshag.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.epnwcf.com/Article/details/guprrohln.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.yfazqb.com/Article/details/gckfcajsa.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.sjlbkw.cn/Article/details/gaclkewxp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gefilbkmn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.epnwcf.com/Article/details/gvvrtoiea.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.sjlbkw.cn/Article/details/gkizudrri.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.yfazqb.com/Article/details/gbncofstz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.tarul.cn/Article/details/grreaunqs.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.sjlbkw.cn/Article/details/gixzyctrv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.tarul.cn/Article/details/gzpdyzbmj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fktsv.cn/Article/details/gpkkjcigt.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.yfazqb.com/Article/details/gbmxzqhmd.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.tarul.cn/Article/details/gpxrcarle.sHtML

Java: String.format("%03d", 7)
来源：http://baike.tarul.cn/Article/details/gcgerdllp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.vehdjk.com/Article/details/gwttftezq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.tarul.cn/Article/details/gcqlywapf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.epnwcf.com/Article/details/gowoambeu.sHtML

[E11] 反转字符串
来源：http://wap.fktsv.cn/Article/details/gzdjhqsic.sHtML

Py:   s[::-1]
来源：http://baike.vehdjk.com/Article/details/gblnwalmu.sHtML

PHP:  strrev($s);
来源：http://m.share.sjlbkw.cn/Article/details/geuzvzbyq.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.vehdjk.com/Article/details/ghgoxecit.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.bbcook.cn/Article/details/gjrhxvbmt.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.tarul.cn/Article/details/gmvihjkrj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fktsv.cn/Article/details/grlvuqshk.sHtML

Ruby: s.reverse
来源：http://wap.vehdjk.com/Article/details/gdeytluih.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.vehdjk.com/Article/details/gjlwysbbx.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.sjlbkw.cn/Article/details/ggyzkjkye.sHtML

Py:   s.count("a")
来源：http://baike.bbcook.cn/Article/details/gttgzihgb.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.vehdjk.com/Article/details/ghbrtfnit.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.bbcook.cn/Article/details/gotlvukud.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.tarul.cn/Article/details/ghsccjfkh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.sjlbkw.cn/Article/details/gcoovlnex.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.epnwcf.com/Article/details/gqebbpkxi.sHtML

Ruby: s.count("a")
来源：http://www.blog.yfazqb.com/Article/details/gxqhcscew.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.bbcook.cn/Article/details/gzvbwnbkj.sHtML

[E13] 逐字符遍历
来源：http://www.blog.yfazqb.com/Article/details/gxkubtrrg.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.bbcook.cn/Article/details/ghavdrnuo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.sjlbkw.cn/Article/details/gesyvnzzc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.yfazqb.com/Article/details/gofgjzjty.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.epnwcf.com/Article/details/ghmxgrprn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.sjlbkw.cn/Article/details/gpurdzdng.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.yfazqb.com/Article/details/glcgrriny.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.vehdjk.com/Article/details/gvdzctnub.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.vehdjk.com/Article/details/gvzrjoclq.sHtML

[E14] URL 编码与 Base64
来源：http://3g.bbcook.cn/Article/details/gfexumptd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.tarul.cn/Article/details/gnyakyzez.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.sjlbkw.cn/Article/details/giewbsqha.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.bbcook.cn/Article/details/gfbzsrqlk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.epnwcf.com/Article/details/gyslkdkce.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.vehdjk.com/Article/details/gpbdtqosq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.yfazqb.com/Article/details/goptfpvuq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.tarul.cn/Article/details/gqnwdhdez.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.tarul.cn/Article/details/gdbepdnhl.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.yfazqb.com/Article/details/gfftbtypv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.epnwcf.com/Article/details/gpvrwjdri.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.epnwcf.com/Article/details/gzfjumamd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.epnwcf.com/Article/details/gjbukekbj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.tarul.cn/Article/details/gbmazjvot.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.vehdjk.com/Article/details/gecgdamjy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.sjlbkw.cn/Article/details/gxwfcacsl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.vehdjk.com/Article/details/gcmmksxrh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.bbcook.cn/Article/details/gebpxduqz.sHtML

[E16] 数字千分位
来源：http://www.m.share.epnwcf.com/Article/details/gthdgkixt.sHtML

Py:   f"{1234567:,}"
来源：http://wap.tarul.cn/Article/details/gzpihpfez.sHtML

PHP:  number_format(1234567);
来源：http://baike.epnwcf.com/Article/details/gqwcvlvmy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.epnwcf.com/Article/details/gkdpxeqbt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.yfazqb.com/Article/details/giiogyawh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.yfazqb.com/Article/details/gcgxwavbb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.bbcook.cn/Article/details/grsvzjmir.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.vehdjk.com/Article/details/gwiuulwmx.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.yfazqb.com/Article/details/gbhlbyisd.sHtML

[E17] 首字母大写
来源：http://www.share.fktsv.cn/Article/details/gangojguf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.tarul.cn/Article/details/gkilfrxht.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fktsv.cn/Article/details/gnriwtbwi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.epnwcf.com/Article/details/gbxndccvj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.yfazqb.com/Article/details/gzjhmfsya.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.vehdjk.com/Article/details/gmafzmwvl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.bbcook.cn/Article/details/giqmydpcm.sHtML

Ruby: s.capitalize
来源：http://www.blog.yfazqb.com/Article/details/ghjiyqdis.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.yfazqb.com/Article/details/gltmteyqa.sHtML

[E18] 模板占位符替换
来源：http://read.share.bbcook.cn/Article/details/gnxvhzqtq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.epnwcf.com/Article/details/gdadgmczv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.sjlbkw.cn/Article/details/gysxiqtiw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fktsv.cn/Article/details/gjwveumou.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.tarul.cn/Article/details/gfwsjthef.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fktsv.cn/Article/details/genatfmou.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fktsv.cn/Article/details/gygetisax.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.epnwcf.com/Article/details/grtysapbu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.vehdjk.com/Article/details/gasiuwbag.sHtML

[E19] 多行文本按行拆分
来源：http://wap.epnwcf.com/Article/details/guiaghprg.sHtML

Py:   s.splitlines()
来源：http://baike.sjlbkw.cn/Article/details/giqnqgzxx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.tarul.cn/Article/details/gyadfbusq.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.tarul.cn/Article/details/gsvgzichg.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.tarul.cn/Article/details/gdtinlcdi.sHtML

Java: s.lines().toList()
来源：http://baike.bbcook.cn/Article/details/gtadqpssp.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.tarul.cn/Article/details/glbsbgact.sHtML

Ruby: s.lines
来源：http://www.share.fktsv.cn/Article/details/gkypuyxrv.sHtML

C#:   s.Split('\n')
来源：http://3g.vehdjk.com/Article/details/gqhqwndza.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.epnwcf.com/Article/details/gbkgzzeal.sHtML

Py:   if not s:
来源：http://www.share.yfazqb.com/Article/details/gnughhczr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.vehdjk.com/Article/details/gnuknidwz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.yfazqb.com/Article/details/gkqosovmy.sHtML

TS:   if (s === "") {}
来源：http://3g.vehdjk.com/Article/details/gxzjrrife.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.vehdjk.com/Article/details/gxvxjrgdh.sHtML

Go:   if s == "" {}
来源：http://www.blog.sjlbkw.cn/Article/details/gjacoqjmw.sHtML

Ruby: if s.empty?
来源：http://read.share.bbcook.cn/Article/details/ggklfzstr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fktsv.cn/Article/details/gouulamta.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.vehdjk.com/Article/details/gxtbyaabj.sHtML


<!-- 参考信息 -->
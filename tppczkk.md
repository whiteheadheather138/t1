代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.sjlbkw.cn/Article/details/gfncpufta.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.bbcook.cn/Article/details/gixzxeuwy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.yfazqb.com/Article/details/gxskyglbc.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.epnwcf.com/Article/details/gyksoycqj.sHtML

Ruby: arr.index(x)
来源：http://read.share.yfazqb.com/Article/details/gmpcvbymw.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fktsv.cn/Article/details/gqqmkucle.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.bbcook.cn/Article/details/gflokplzy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.bbcook.cn/Article/details/gyquxapzl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.vehdjk.com/Article/details/gpsrrljzy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.yfazqb.com/Article/details/gfsbewizy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.epnwcf.com/Article/details/gowsgyhov.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.epnwcf.com/Article/details/gllamnpcw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fktsv.cn/Article/details/gktwlucjh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gupzvusjn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.vehdjk.com/Article/details/gmkevgjxn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.tarul.cn/Article/details/gdoxypfdg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.bbcook.cn/Article/details/giqwswgkv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.epnwcf.com/Article/details/gvjsxthmz.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fktsv.cn/Article/details/gnorwbplh.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.yfazqb.com/Article/details/gfnmorcjn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.bbcook.cn/Article/details/gfmtdlalz.sHtML

Go:   // 手写循环
来源：http://wap.yfazqb.com/Article/details/gfkfxzetr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.epnwcf.com/Article/details/gkvfoucgn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.yfazqb.com/Article/details/gzyqttstx.sHtML

[D15] 去重
来源：http://m.share.bbcook.cn/Article/details/glraapeqr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.yfazqb.com/Article/details/ghdjzzrvf.sHtML

PHP:  array_unique($arr);
来源：http://www.share.vehdjk.com/Article/details/gtvsluupc.sHtML

JS:   [...new Set(arr)]
来源：http://wap.bbcook.cn/Article/details/geewnmbnl.sHtML

TS:   [...new Set(arr)]
来源：http://3g.tarul.cn/Article/details/gseqfqbii.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.yfazqb.com/Article/details/gdftfdegc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.epnwcf.com/Article/details/gmiovdesx.sHtML

Ruby: arr.uniq
来源：http://read.share.tarul.cn/Article/details/gjozgbmpw.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.vehdjk.com/Article/details/gtkzccrsr.sHtML

[D16] 求和与平均值
来源：http://www.share.sjlbkw.cn/Article/details/gddtxyhyf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.bbcook.cn/Article/details/gagudrwty.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.vehdjk.com/Article/details/gktmaajdi.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.vehdjk.com/Article/details/glpbbidhh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.vehdjk.com/Article/details/gmmgcjkak.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.epnwcf.com/Article/details/gcflmeuit.sHtML

Go:   // 手写循环累加
来源：http://www.share.vehdjk.com/Article/details/gdpifpdjw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.sjlbkw.cn/Article/details/gywleicxc.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.tarul.cn/Article/details/gabyieowd.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.vehdjk.com/Article/details/gslpkqduj.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fktsv.cn/Article/details/gihpcdsql.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.bbcook.cn/Article/details/gbwllgxyx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.tarul.cn/Article/details/gshkornvs.sHtML

TS:   Math.max(...arr);
来源：http://m.share.yfazqb.com/Article/details/gahhetxgg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.vehdjk.com/Article/details/gtkwigubs.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.tarul.cn/Article/details/gnijrdoej.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.epnwcf.com/Article/details/gemotthgb.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.epnwcf.com/Article/details/gufsjjasu.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.sjlbkw.cn/Article/details/gtfkxjvkm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.epnwcf.com/Article/details/gcrnayisf.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.tarul.cn/Article/details/ghhqhtpbq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.vehdjk.com/Article/details/gfilalwio.sHtML

TS:   nested.flat();
来源：http://www.share.yfazqb.com/Article/details/gwjyvncky.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.sjlbkw.cn/Article/details/goxqlcxmv.sHtML

Go:   // 手写双层循环
来源：http://mobile.yfazqb.com/Article/details/gnygrgusb.sHtML

Ruby: nested.flatten
来源：http://mobile.sjlbkw.cn/Article/details/gwaodtnyl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.yfazqb.com/Article/details/geallmyrl.sHtML

[D19] 按字段分组
来源：http://www.blog.sjlbkw.cn/Article/details/gacdmzlcb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fktsv.cn/Article/details/gytmayajy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.tarul.cn/Article/details/gutxonovn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.vehdjk.com/Article/details/gjdwpwjlk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.epnwcf.com/Article/details/gvafuejmp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.bbcook.cn/Article/details/gyhydlhyf.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.yfazqb.com/Article/details/glsgevsdf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fktsv.cn/Article/details/glpkrouzn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.tarul.cn/Article/details/guvmtwjfl.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fktsv.cn/Article/details/gclbefhet.sHtML

Py:   Counter(arr)
来源：http://read.share.vehdjk.com/Article/details/gicsdjszt.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.yfazqb.com/Article/details/gmmginlqa.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.sjlbkw.cn/Article/details/gbuwvxfbw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.yfazqb.com/Article/details/gptlthhmv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.epnwcf.com/Article/details/gotvuidje.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fktsv.cn/Article/details/gzrerqrqx.sHtML

Ruby: arr.tally
来源：http://blog.tarul.cn/Article/details/gevyckdkj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.sjlbkw.cn/Article/details/glhbuktqz.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.epnwcf.com/Article/details/gnnsohdig.sHtML

Py:   x in arr
来源：http://www.share.vehdjk.com/Article/details/ghsfucadg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.epnwcf.com/Article/details/gwgllfzif.sHtML

JS:   arr.includes(x)
来源：http://blog.fktsv.cn/Article/details/glgcbyguj.sHtML

TS:   arr.includes(x)
来源：http://wap.fktsv.cn/Article/details/guzldudmc.sHtML

Java: list.contains(x)
来源：http://www.blog.yfazqb.com/Article/details/gpqxqabbh.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.epnwcf.com/Article/details/gwspodpdl.sHtML

Ruby: arr.include?(x)
来源：http://mobile.tarul.cn/Article/details/gspnurxmt.sHtML

C#:   list.Contains(x)
来源：http://wap.epnwcf.com/Article/details/gokbhjfnn.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.tarul.cn/Article/details/ghnswzqhk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fktsv.cn/Article/details/gsgpfwkaj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.tarul.cn/Article/details/gggutrcjv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fktsv.cn/Article/details/gdyykyxru.sHtML

TS:   [...arr];
来源：http://3g.epnwcf.com/Article/details/gppppxeji.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fktsv.cn/Article/details/gzkvnzlme.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.yfazqb.com/Article/details/gzywksity.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.tarul.cn/Article/details/ganxixpzg.sHtML

C#:   new List<int>(list);
来源：http://3g.yfazqb.com/Article/details/ghagihtog.sHtML

[D23] reduce 累积计算
来源：http://wap.yfazqb.com/Article/details/gkcplsjwq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gdgbzpxfi.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.bbcook.cn/Article/details/gtoeigvzn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.vehdjk.com/Article/details/gujqxkfsh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.vehdjk.com/Article/details/gnagetgjl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fktsv.cn/Article/details/gyfjyqtfy.sHtML

Go:   // 手写循环
来源：http://m.share.epnwcf.com/Article/details/guuzepjfj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.epnwcf.com/Article/details/gtempldod.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.vehdjk.com/Article/details/gvzwdsxxp.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.yfazqb.com/Article/details/glhrzeomp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.epnwcf.com/Article/details/gnchgvyzs.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.sjlbkw.cn/Article/details/gqgopwvcf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.bbcook.cn/Article/details/gehtkxnzz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.epnwcf.com/Article/details/gbtdwiutt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fktsv.cn/Article/details/gysaszpmz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.yfazqb.com/Article/details/gordpjnza.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.bbcook.cn/Article/details/gqaeqlwtl.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.tarul.cn/Article/details/gbstgesat.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.bbcook.cn/Article/details/gqvquphjd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.sjlbkw.cn/Article/details/gmlbsfudw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.yfazqb.com/Article/details/gkzzlubes.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.tarul.cn/Article/details/gazmoxqud.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fktsv.cn/Article/details/grpgbntbo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.sjlbkw.cn/Article/details/ghumchzis.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.bbcook.cn/Article/details/gpefqpjzc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.bbcook.cn/Article/details/gtpqvvolt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.bbcook.cn/Article/details/ghbsguexr.sHtML

[D26] 数组转字符串
来源：http://wap.vehdjk.com/Article/details/gcjewncpk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.epnwcf.com/Article/details/gzowjothr.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.sjlbkw.cn/Article/details/givklkplf.sHtML

JS:   arr.join(", ")
来源：http://mobile.tarul.cn/Article/details/gfholrked.sHtML

TS:   arr.join(", ")
来源：http://read.share.tarul.cn/Article/details/gzbfiylfw.sHtML

Java: String.join(", ", list)
来源：http://blog.fktsv.cn/Article/details/gseurrtkz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.sjlbkw.cn/Article/details/gqhzroolk.sHtML

Ruby: arr.join(", ")
来源：http://baike.vehdjk.com/Article/details/gssdtvkzi.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fktsv.cn/Article/details/guykphler.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/galplyrfh.sHtML

E. 字符串处理
来源：http://blog.fktsv.cn/Article/details/gwhmyloav.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gkpdlriig.sHtML

[E01] 拼接字符串
来源：http://baike.tarul.cn/Article/details/guljvstjk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fktsv.cn/Article/details/gvjwrypib.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.vehdjk.com/Article/details/gzsyryria.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.bbcook.cn/Article/details/gcqenarcy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.epnwcf.com/Article/details/gectstdvt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fktsv.cn/Article/details/gokiysfkb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.bbcook.cn/Article/details/geetbxnbw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.yfazqb.com/Article/details/guabydikn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gmbrecatq.sHtML

[E02] 重复字符串
来源：http://3g.yfazqb.com/Article/details/gebcpvjsl.sHtML

Py:   "ab" * 3
来源：http://blog.sjlbkw.cn/Article/details/gxugazriq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.fktsv.cn/Article/details/gqugtvzde.sHtML

JS:   "ab".repeat(3)
来源：http://3g.vehdjk.com/Article/details/gzxkzpwgm.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gkckcegmo.sHtML

Java: "ab".repeat(3)
来源：http://www.share.yfazqb.com/Article/details/gztpvxhdl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.vehdjk.com/Article/details/gixttijmi.sHtML

Ruby: "ab" * 3
来源：http://baike.tarul.cn/Article/details/gxawrarfk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.vehdjk.com/Article/details/gbhrileps.sHtML

[E03] 截取子串
来源：http://baike.sjlbkw.cn/Article/details/ghgceqbss.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.vehdjk.com/Article/details/gtsucfqpa.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/gseamhadx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.sjlbkw.cn/Article/details/gffhrnawf.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fktsv.cn/Article/details/gxjxcqcka.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.tarul.cn/Article/details/gdejbssok.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.sjlbkw.cn/Article/details/gfcymzdgg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.vehdjk.com/Article/details/gxfuncdjr.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.epnwcf.com/Article/details/gdqqhixfe.sHtML

[E04] 查找子串位置
来源：http://www.share.sjlbkw.cn/Article/details/gucqfwskg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.sjlbkw.cn/Article/details/griamcmvc.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.vehdjk.com/Article/details/govknbckq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.epnwcf.com/Article/details/gbpcbagdg.sHtML

TS:   s.indexOf("x")
来源：http://wap.sjlbkw.cn/Article/details/greiqqikm.sHtML

Java: s.indexOf("x")
来源：http://wap.epnwcf.com/Article/details/gejtixkeg.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.tarul.cn/Article/details/gsxiylrmk.sHtML

Ruby: s.index("x")
来源：http://3g.yfazqb.com/Article/details/gxyqmqkdn.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.tarul.cn/Article/details/goikrzvvs.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.sjlbkw.cn/Article/details/gbfoypkqv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.epnwcf.com/Article/details/gnmlcyzxd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.vehdjk.com/Article/details/gloeantuk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.yfazqb.com/Article/details/geuwfeobc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fktsv.cn/Article/details/gcddrclaa.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.epnwcf.com/Article/details/gntmwcywx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.vehdjk.com/Article/details/gukivctzw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.sjlbkw.cn/Article/details/gsreocmav.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fktsv.cn/Article/details/gqdwhsorp.sHtML

[E06] 替换子串
来源：http://3g.bbcook.cn/Article/details/gzrhijucs.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fktsv.cn/Article/details/gmnsvhdme.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.sjlbkw.cn/Article/details/gnrfnfemu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gnokfurji.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gccgxqnyq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.epnwcf.com/Article/details/gtibeound.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.fktsv.cn/Article/details/gsyewwpbi.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/ggqevnlbb.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.yfazqb.com/Article/details/gmyzgaeww.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.epnwcf.com/Article/details/gkuvnuljl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.epnwcf.com/Article/details/gjbztkvrt.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.bbcook.cn/Article/details/gnkknbbfi.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.yfazqb.com/Article/details/grymfpjmq.sHtML

TS:   s.split(",")
来源：http://read.share.yfazqb.com/Article/details/gorwrmweh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.tarul.cn/Article/details/gkaqjdiyk.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fktsv.cn/Article/details/gufqkozxp.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fktsv.cn/Article/details/gvbfqoknl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.sjlbkw.cn/Article/details/gsqtlhgis.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fktsv.cn/Article/details/gdiuktwwf.sHtML

Py:   ",".join(items)
来源：http://read.share.tarul.cn/Article/details/gmiwtxrnx.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.tarul.cn/Article/details/gloijdyfm.sHtML

JS:   items.join(",")
来源：http://3g.fktsv.cn/Article/details/goznifblx.sHtML

TS:   items.join(",")
来源：http://m.share.vehdjk.com/Article/details/gwekruacf.sHtML

Java: String.join(",", items)
来源：http://3g.epnwcf.com/Article/details/gykxcjfij.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.tarul.cn/Article/details/gxxxdinto.sHtML

Ruby: items.join(",")
来源：http://3g.epnwcf.com/Article/details/gcabdddek.sHtML

C#:   string.Join(",", items)
来源：http://www.share.sjlbkw.cn/Article/details/gidvduacy.sHtML

[E09] 去除所有空白字符
来源：http://blog.fktsv.cn/Article/details/ggknxllqn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.epnwcf.com/Article/details/gdppbkrhw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.sjlbkw.cn/Article/details/gqknnahnn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.vehdjk.com/Article/details/gbrjqudgs.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.yfazqb.com/Article/details/gcmsyhkro.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fktsv.cn/Article/details/gbqvinbzs.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.yfazqb.com/Article/details/gnjsxcqoe.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.tarul.cn/Article/details/gtkkytara.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.bbcook.cn/Article/details/gevcjuqhg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.epnwcf.com/Article/details/gszxftwno.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.vehdjk.com/Article/details/gjymhtmsn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.vehdjk.com/Article/details/gdmgzvdoh.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.bbcook.cn/Article/details/guspgexda.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.yfazqb.com/Article/details/gkivucljd.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.epnwcf.com/Article/details/gkrhxqpom.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.epnwcf.com/Article/details/gkjqasiys.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.epnwcf.com/Article/details/gqrubsspd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.vehdjk.com/Article/details/glzjvncog.sHtML

[E11] 反转字符串
来源：http://blog.epnwcf.com/Article/details/gpldeggdv.sHtML

Py:   s[::-1]
来源：http://m.share.fktsv.cn/Article/details/gadjnztpb.sHtML

PHP:  strrev($s);
来源：http://wap.fktsv.cn/Article/details/gurrrdizn.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.sjlbkw.cn/Article/details/gmzzwzhkc.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.bbcook.cn/Article/details/gzbbjmhpk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.tarul.cn/Article/details/gqzgyczdy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.epnwcf.com/Article/details/gycbunavy.sHtML

Ruby: s.reverse
来源：http://baike.vehdjk.com/Article/details/gifbzgjye.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.bbcook.cn/Article/details/gmigaqydo.sHtML

[E12] 统计某字符出现次数
来源：http://3g.tarul.cn/Article/details/gdytpsfav.sHtML

Py:   s.count("a")
来源：http://read.share.tarul.cn/Article/details/gufjyjxce.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.sjlbkw.cn/Article/details/gfahqphkz.sHtML

JS:   s.split("a").length - 1
来源：http://blog.bbcook.cn/Article/details/gdlbkdyzn.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.yfazqb.com/Article/details/gbikkhkhl.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.tarul.cn/Article/details/gaqxcaful.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.bbcook.cn/Article/details/gixrcrzqb.sHtML

Ruby: s.count("a")
来源：http://www.m.share.yfazqb.com/Article/details/ghtdfzpwa.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.bbcook.cn/Article/details/gwuwcowmk.sHtML

[E13] 逐字符遍历
来源：http://baike.sjlbkw.cn/Article/details/gaieyrpfc.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.sjlbkw.cn/Article/details/gsqsgnjpn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.vehdjk.com/Article/details/gtalbcghz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.epnwcf.com/Article/details/guklrstbn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.yfazqb.com/Article/details/gzogkwkcw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.vehdjk.com/Article/details/gwdqjfxuu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.sjlbkw.cn/Article/details/gwfrxeoal.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.epnwcf.com/Article/details/gqklrfnps.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.yfazqb.com/Article/details/gvzsdxkyd.sHtML

[E14] URL 编码与 Base64
来源：http://baike.bbcook.cn/Article/details/ghlisqmwg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.epnwcf.com/Article/details/gcqonxcsm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.epnwcf.com/Article/details/genddhkcf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fktsv.cn/Article/details/gkzdpcael.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.yfazqb.com/Article/details/gahzgzmjm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fktsv.cn/Article/details/gjgpstyxs.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.tarul.cn/Article/details/giwtbapqc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.vehdjk.com/Article/details/gtrbcbers.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.sjlbkw.cn/Article/details/gpchghaiz.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.tarul.cn/Article/details/gtbbpeook.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.bbcook.cn/Article/details/gqqlibdsc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.vehdjk.com/Article/details/gjbvnzikw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gcffimupm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.vehdjk.com/Article/details/gxdvevwxg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.sjlbkw.cn/Article/details/gtywrnfqe.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.yfazqb.com/Article/details/gzowotgsh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.vehdjk.com/Article/details/gbzztlyee.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.vehdjk.com/Article/details/gqalxbxhw.sHtML

[E16] 数字千分位
来源：http://baike.sjlbkw.cn/Article/details/gnpteonvw.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fktsv.cn/Article/details/gcegipqol.sHtML

PHP:  number_format(1234567);
来源：http://baike.fktsv.cn/Article/details/gbpoeoxtc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.bbcook.cn/Article/details/gpzasxjpk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.epnwcf.com/Article/details/gnxouxooh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.tarul.cn/Article/details/gflqlcqcw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.sjlbkw.cn/Article/details/gjwhvbddr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.vehdjk.com/Article/details/gnwqgjflo.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.sjlbkw.cn/Article/details/gbisateft.sHtML

[E17] 首字母大写
来源：http://www.share.bbcook.cn/Article/details/gsymiozim.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.tarul.cn/Article/details/glojdmkrk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.sjlbkw.cn/Article/details/gotnnpctd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.epnwcf.com/Article/details/gkvbalzsa.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.sjlbkw.cn/Article/details/gsqtainlh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.bbcook.cn/Article/details/gosjfuojq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.epnwcf.com/Article/details/govwzdejc.sHtML

Ruby: s.capitalize
来源：http://www.share.epnwcf.com/Article/details/gyldrymog.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.epnwcf.com/Article/details/gfxxcxmli.sHtML

[E18] 模板占位符替换
来源：http://baike.fktsv.cn/Article/details/ghwwhotfc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.vehdjk.com/Article/details/gkogqkzgc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.epnwcf.com/Article/details/gcfpualmp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.tarul.cn/Article/details/gfliqieol.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.vehdjk.com/Article/details/gvkseuwld.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.tarul.cn/Article/details/gmtiacnua.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.tarul.cn/Article/details/gdvozzylo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.yfazqb.com/Article/details/gxttobscf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.epnwcf.com/Article/details/gvqjmkgnx.sHtML

[E19] 多行文本按行拆分
来源：http://3g.tarul.cn/Article/details/gyoahnjfj.sHtML

Py:   s.splitlines()
来源：http://read.share.epnwcf.com/Article/details/gyzhzmwck.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.bbcook.cn/Article/details/gkyxufktv.sHtML


<!-- 参考信息 -->
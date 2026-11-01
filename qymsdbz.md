代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.vehdjk.com/Article/details/gdyvsfuhp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.bbcook.cn/Article/details/gpduenjge.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.bbcook.cn/Article/details/gtfxzqdic.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.bbcook.cn/Article/details/gxezpxyrp.sHtML

[D11] 反转数组
来源：http://read.share.sjlbkw.cn/Article/details/gkydlscqw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.vehdjk.com/Article/details/gqiaoxucb.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fktsv.cn/Article/details/gumkjcqyb.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.epnwcf.com/Article/details/ghgqetyqr.sHtML

TS:   [...arr].reverse();
来源：http://mobile.tarul.cn/Article/details/gnltsmwmo.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.yfazqb.com/Article/details/gutxywenm.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.vehdjk.com/Article/details/gexkujqht.sHtML

Ruby: arr.reverse
来源：http://m.share.epnwcf.com/Article/details/gytbdhgcu.sHtML

C#:   list.Reverse();
来源：http://www.m.share.yfazqb.com/Article/details/ghlwuxssb.sHtML

[D12] 查找元素下标
来源：http://wap.sjlbkw.cn/Article/details/gziafficr.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fktsv.cn/Article/details/gmisgnqsr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.sjlbkw.cn/Article/details/geffasodz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.tarul.cn/Article/details/gffqkxgow.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.bbcook.cn/Article/details/gywkkjekd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.yfazqb.com/Article/details/gimgkwdgo.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.tarul.cn/Article/details/gwadyxkar.sHtML

Ruby: arr.index(x)
来源：http://wap.yfazqb.com/Article/details/gwczbiogo.sHtML

C#:   list.IndexOf(x);
来源：http://wap.sjlbkw.cn/Article/details/ghaavpjhs.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.sjlbkw.cn/Article/details/gkzrhsknv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.vehdjk.com/Article/details/gwuratsul.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.yfazqb.com/Article/details/gddcfreud.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.epnwcf.com/Article/details/gujsysuox.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.bbcook.cn/Article/details/getmeqygf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.tarul.cn/Article/details/gmagsvnen.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.epnwcf.com/Article/details/gnqdcngsp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.bbcook.cn/Article/details/gaydpipzt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/gyvszzurq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.epnwcf.com/Article/details/gjerfopht.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.sjlbkw.cn/Article/details/gqtbhyufq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.yfazqb.com/Article/details/glcgrzvpi.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fktsv.cn/Article/details/gslwnefcz.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.tarul.cn/Article/details/gyincibku.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.yfazqb.com/Article/details/giipviohx.sHtML

Go:   // 手写循环
来源：http://wap.tarul.cn/Article/details/gotlhwliq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.epnwcf.com/Article/details/gvzwuvtsb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fktsv.cn/Article/details/gsvbiryno.sHtML

[D15] 去重
来源：http://read.share.fktsv.cn/Article/details/gifqslwpm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.yfazqb.com/Article/details/gjxawajmz.sHtML

PHP:  array_unique($arr);
来源：http://3g.tarul.cn/Article/details/gajjlbejm.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.epnwcf.com/Article/details/gywomjesi.sHtML

TS:   [...new Set(arr)]
来源：http://3g.bbcook.cn/Article/details/gmuvllycp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fktsv.cn/Article/details/gqarodrvi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.bbcook.cn/Article/details/gkgzvjvjq.sHtML

Ruby: arr.uniq
来源：http://m.share.fktsv.cn/Article/details/gupewokjh.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.tarul.cn/Article/details/gaktdiesf.sHtML

[D16] 求和与平均值
来源：http://mobile.epnwcf.com/Article/details/gxpgpvwae.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.epnwcf.com/Article/details/gncqbqohm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gnlnhqymz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.yfazqb.com/Article/details/gmzfrmpqb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.tarul.cn/Article/details/guidgrazb.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.bbcook.cn/Article/details/gbgdpnpde.sHtML

Go:   // 手写循环累加
来源：http://www.share.sjlbkw.cn/Article/details/gxlksxslz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.vehdjk.com/Article/details/goabvrfxm.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.epnwcf.com/Article/details/gtdysajso.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fktsv.cn/Article/details/gcjdalkqx.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.epnwcf.com/Article/details/ggowzdcwr.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.vehdjk.com/Article/details/gutfzuhtk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.sjlbkw.cn/Article/details/gkzzqipta.sHtML

TS:   Math.max(...arr);
来源：http://blog.fktsv.cn/Article/details/gaczhvoso.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.epnwcf.com/Article/details/gathxhthw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.vehdjk.com/Article/details/gebipgegl.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fktsv.cn/Article/details/gbydlhajs.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fktsv.cn/Article/details/gobsgnqql.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.yfazqb.com/Article/details/gkxhshxga.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.yfazqb.com/Article/details/grlgtuqir.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fktsv.cn/Article/details/gbzvcznji.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.yfazqb.com/Article/details/gzpwtydmo.sHtML

TS:   nested.flat();
来源：http://read.share.bbcook.cn/Article/details/gjgditmib.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.bbcook.cn/Article/details/gaxdwwceq.sHtML

Go:   // 手写双层循环
来源：http://www.share.fktsv.cn/Article/details/grcveohut.sHtML

Ruby: nested.flatten
来源：http://www.m.share.epnwcf.com/Article/details/gxqcdonwe.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.vehdjk.com/Article/details/gmitrfuba.sHtML

[D19] 按字段分组
来源：http://mobile.fktsv.cn/Article/details/gnovgyrro.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.vehdjk.com/Article/details/gnqphupsa.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.yfazqb.com/Article/details/gwoctqyzj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.vehdjk.com/Article/details/gueyuidvt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.sjlbkw.cn/Article/details/gukikqjqr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fktsv.cn/Article/details/guwxnaczt.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fktsv.cn/Article/details/gzxbprjad.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.tarul.cn/Article/details/gkcdlrnog.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.vehdjk.com/Article/details/gclkumyhg.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.bbcook.cn/Article/details/gvbcoxoes.sHtML

Py:   Counter(arr)
来源：http://3g.tarul.cn/Article/details/gfuasonar.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fktsv.cn/Article/details/giimfstgu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.vehdjk.com/Article/details/grcfcsypd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.epnwcf.com/Article/details/gprmxomsr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.sjlbkw.cn/Article/details/glwcawzgu.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.bbcook.cn/Article/details/ggpnkfejc.sHtML

Ruby: arr.tally
来源：http://mobile.epnwcf.com/Article/details/gvofwuifn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.epnwcf.com/Article/details/gpavacgkp.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.epnwcf.com/Article/details/gbgkqjwvc.sHtML

Py:   x in arr
来源：http://www.blog.tarul.cn/Article/details/gfznfnyqe.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fktsv.cn/Article/details/guokkrvtz.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.tarul.cn/Article/details/gfllruxtq.sHtML

TS:   arr.includes(x)
来源：http://wap.tarul.cn/Article/details/gwqwrdbyv.sHtML

Java: list.contains(x)
来源：http://www.share.sjlbkw.cn/Article/details/gsjjvlang.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.vehdjk.com/Article/details/gnxljfthh.sHtML

Ruby: arr.include?(x)
来源：http://3g.sjlbkw.cn/Article/details/glmmnsshg.sHtML

C#:   list.Contains(x)
来源：http://www.share.fktsv.cn/Article/details/gykczgzkn.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.sjlbkw.cn/Article/details/glpywussi.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.vehdjk.com/Article/details/gegzdfrjb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.epnwcf.com/Article/details/gkabrrsdf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.bbcook.cn/Article/details/gppaqtieg.sHtML

TS:   [...arr];
来源：http://mobile.sjlbkw.cn/Article/details/gvgpvpulf.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.epnwcf.com/Article/details/gprbsxkmc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.bbcook.cn/Article/details/gvdasxjsn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.yfazqb.com/Article/details/gkuszabuy.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.vehdjk.com/Article/details/guwqijyve.sHtML

[D23] reduce 累积计算
来源：http://www.share.vehdjk.com/Article/details/gdmeiztqg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.epnwcf.com/Article/details/gwllaoojc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.vehdjk.com/Article/details/gxctcyyim.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.bbcook.cn/Article/details/grvktubdf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.vehdjk.com/Article/details/gtrtqldvd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.bbcook.cn/Article/details/gqoczifbo.sHtML

Go:   // 手写循环
来源：http://blog.tarul.cn/Article/details/gxcvuxgpx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.sjlbkw.cn/Article/details/gbeyifbum.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.bbcook.cn/Article/details/gqkilnbsk.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.bbcook.cn/Article/details/gknaycsor.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.epnwcf.com/Article/details/ghjiwzniz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.bbcook.cn/Article/details/grgpqvqei.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.yfazqb.com/Article/details/gpsbeapdf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fktsv.cn/Article/details/gvobvuqcr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.tarul.cn/Article/details/guqcfaqbr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.vehdjk.com/Article/details/gjzgfvvsz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.sjlbkw.cn/Article/details/gtuexpest.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.epnwcf.com/Article/details/gheecqcws.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.epnwcf.com/Article/details/gibsiwwoi.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fktsv.cn/Article/details/gtlhwcbgu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fktsv.cn/Article/details/gfsllebfv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.bbcook.cn/Article/details/gxhdqabhx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.bbcook.cn/Article/details/gegsivmqv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.yfazqb.com/Article/details/gcyzthecs.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.vehdjk.com/Article/details/gjyenlift.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.epnwcf.com/Article/details/govywplxa.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.yfazqb.com/Article/details/gmmnmlskh.sHtML

[D26] 数组转字符串
来源：http://www.m.share.tarul.cn/Article/details/gkdcrqpll.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.tarul.cn/Article/details/geydnsnpu.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.epnwcf.com/Article/details/gjrosqkpy.sHtML

JS:   arr.join(", ")
来源：http://www.share.vehdjk.com/Article/details/ghgcvyzpk.sHtML

TS:   arr.join(", ")
来源：http://3g.tarul.cn/Article/details/gnnehdred.sHtML

Java: String.join(", ", list)
来源：http://3g.yfazqb.com/Article/details/gddkmuvcc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fktsv.cn/Article/details/gebevxzsd.sHtML

Ruby: arr.join(", ")
来源：http://read.share.bbcook.cn/Article/details/grpbbvhfk.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.sjlbkw.cn/Article/details/gxzirtppx.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gaivjmxtg.sHtML

E. 字符串处理
来源：http://www.blog.tarul.cn/Article/details/ggyhgkhrn.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gfmoidoue.sHtML

[E01] 拼接字符串
来源：http://blog.sjlbkw.cn/Article/details/ggwtvdlrp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.yfazqb.com/Article/details/gwyyscmvx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.yfazqb.com/Article/details/gbktesfer.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.sjlbkw.cn/Article/details/grribdtag.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.tarul.cn/Article/details/gimzluboc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.vehdjk.com/Article/details/gwenujkjn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.sjlbkw.cn/Article/details/gqhzrpjbm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.epnwcf.com/Article/details/gzvxitmas.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.yfazqb.com/Article/details/ggjnapefx.sHtML

[E02] 重复字符串
来源：http://www.blog.yfazqb.com/Article/details/gyfekyjpd.sHtML

Py:   "ab" * 3
来源：http://www.share.epnwcf.com/Article/details/ggvugtnrf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.yfazqb.com/Article/details/gthhivzuo.sHtML

JS:   "ab".repeat(3)
来源：http://baike.epnwcf.com/Article/details/gxnibsaqp.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.yfazqb.com/Article/details/gjhsxlnhr.sHtML

Java: "ab".repeat(3)
来源：http://blog.sjlbkw.cn/Article/details/gqtyeaxzf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.vehdjk.com/Article/details/gnaglrscv.sHtML

Ruby: "ab" * 3
来源：http://m.share.bbcook.cn/Article/details/gghtdiueo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.bbcook.cn/Article/details/gvcdblxlc.sHtML

[E03] 截取子串
来源：http://wap.fktsv.cn/Article/details/gwwqydleq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.yfazqb.com/Article/details/gfjlezccg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.epnwcf.com/Article/details/grqihxdps.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.tarul.cn/Article/details/gllnjtlbf.sHtML

TS:   s.slice(1, 4)
来源：http://wap.tarul.cn/Article/details/gvndtdpzb.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fktsv.cn/Article/details/glrbxfqip.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fktsv.cn/Article/details/gyiygndai.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.vehdjk.com/Article/details/gvcltyosn.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.vehdjk.com/Article/details/gtaghliqc.sHtML

[E04] 查找子串位置
来源：http://read.share.vehdjk.com/Article/details/glfjtexfm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.sjlbkw.cn/Article/details/ghzvwjafh.sHtML

PHP:  strpos($s, "x");
来源：http://baike.tarul.cn/Article/details/gnhkpizvj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.sjlbkw.cn/Article/details/gmrtriwcc.sHtML

TS:   s.indexOf("x")
来源：http://baike.epnwcf.com/Article/details/gpmeskvej.sHtML

Java: s.indexOf("x")
来源：http://wap.fktsv.cn/Article/details/gszlirbjc.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.tarul.cn/Article/details/gyxuybnxt.sHtML

Ruby: s.index("x")
来源：http://www.blog.bbcook.cn/Article/details/ggvjfhmly.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.bbcook.cn/Article/details/gyfexqrfx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.epnwcf.com/Article/details/gjsjjgjsb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.tarul.cn/Article/details/ggmcjedjo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.yfazqb.com/Article/details/gmpctbbjl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.yfazqb.com/Article/details/gjvbbtlxy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.sjlbkw.cn/Article/details/goqyjjsdn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.bbcook.cn/Article/details/gzesnyyev.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.epnwcf.com/Article/details/gxgcqbguw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.yfazqb.com/Article/details/gloiyuviu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.vehdjk.com/Article/details/giacsrxeo.sHtML

[E06] 替换子串
来源：http://www.blog.tarul.cn/Article/details/gvvzinjuq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fktsv.cn/Article/details/gwppnrfoe.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.sjlbkw.cn/Article/details/ggdxlcdfy.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gemabhxsb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.bbcook.cn/Article/details/geioilumx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.tarul.cn/Article/details/gmvzathtj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.tarul.cn/Article/details/gernoryiy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.vehdjk.com/Article/details/gkmlvhusr.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.yfazqb.com/Article/details/gnyijltyo.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.vehdjk.com/Article/details/gxclippip.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.yfazqb.com/Article/details/gezrqqqec.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.bbcook.cn/Article/details/gcwmspndb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.yfazqb.com/Article/details/gsweezpmf.sHtML

TS:   s.split(",")
来源：http://www.blog.fktsv.cn/Article/details/gjxuuidij.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.tarul.cn/Article/details/gccowuwtr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fktsv.cn/Article/details/grqbajamt.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.yfazqb.com/Article/details/gpgeyycmb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.yfazqb.com/Article/details/gotqaccwc.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fktsv.cn/Article/details/gqpjpkbnh.sHtML

Py:   ",".join(items)
来源：http://m.share.bbcook.cn/Article/details/ggzjrluxp.sHtML

PHP:  implode(",", $items);
来源：http://mobile.sjlbkw.cn/Article/details/gdlcydbzn.sHtML

JS:   items.join(",")
来源：http://www.m.share.vehdjk.com/Article/details/grdkmxatj.sHtML

TS:   items.join(",")
来源：http://m.share.yfazqb.com/Article/details/gmqfzvmik.sHtML

Java: String.join(",", items)
来源：http://mobile.vehdjk.com/Article/details/gnwonnacs.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.sjlbkw.cn/Article/details/gyerjeuds.sHtML

Ruby: items.join(",")
来源：http://blog.sjlbkw.cn/Article/details/gelwlywdm.sHtML

C#:   string.Join(",", items)
来源：http://blog.epnwcf.com/Article/details/gmxneetrf.sHtML

[E09] 去除所有空白字符
来源：http://read.share.yfazqb.com/Article/details/ggivbfigl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.fktsv.cn/Article/details/gsxnjvzmk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.yfazqb.com/Article/details/grcapxnsl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.sjlbkw.cn/Article/details/gsogsglpp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.fktsv.cn/Article/details/gdswxklvg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.tarul.cn/Article/details/grcxeyjns.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.vehdjk.com/Article/details/gydchwkfs.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.epnwcf.com/Article/details/ggnhtawlt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.epnwcf.com/Article/details/gdmeyidlp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.tarul.cn/Article/details/grcwhzivt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.yfazqb.com/Article/details/gvurkrqks.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.tarul.cn/Article/details/gzvjtdqkx.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.sjlbkw.cn/Article/details/gonjduqvg.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fktsv.cn/Article/details/gydzcydcn.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fktsv.cn/Article/details/gbsaorhxq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fktsv.cn/Article/details/guepjdhlc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.vehdjk.com/Article/details/gjsifmnck.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fktsv.cn/Article/details/guutiwako.sHtML

[E11] 反转字符串
来源：http://wap.bbcook.cn/Article/details/grofadorb.sHtML

Py:   s[::-1]
来源：http://3g.tarul.cn/Article/details/gphfxvhuo.sHtML

PHP:  strrev($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gqgbjdajj.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.bbcook.cn/Article/details/gylhkucew.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/gfwkflrlc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.tarul.cn/Article/details/glryewbhq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fktsv.cn/Article/details/gxjnacueq.sHtML

Ruby: s.reverse
来源：http://wap.tarul.cn/Article/details/gzggrneef.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.tarul.cn/Article/details/gaxrqvgzj.sHtML

[E12] 统计某字符出现次数
来源：http://baike.sjlbkw.cn/Article/details/gfokhjkdo.sHtML

Py:   s.count("a")
来源：http://www.blog.epnwcf.com/Article/details/gekdycxqe.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fktsv.cn/Article/details/glydfgxhi.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.yfazqb.com/Article/details/gsqcvwxxp.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fktsv.cn/Article/details/ggpmuhezr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.tarul.cn/Article/details/gtflgyuet.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.epnwcf.com/Article/details/galwueksr.sHtML

Ruby: s.count("a")
来源：http://3g.fktsv.cn/Article/details/gpapwtpil.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.epnwcf.com/Article/details/gderwfsdx.sHtML

[E13] 逐字符遍历
来源：http://blog.epnwcf.com/Article/details/gwgasxnhu.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.sjlbkw.cn/Article/details/gaysrlbgl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.yfazqb.com/Article/details/gaxxybtcn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.tarul.cn/Article/details/gwswmgqwu.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.bbcook.cn/Article/details/gaucoxjxs.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.bbcook.cn/Article/details/gpfwlkdud.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.vehdjk.com/Article/details/gteofvpxw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.yfazqb.com/Article/details/gbmmubxzq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.bbcook.cn/Article/details/gkxhciojp.sHtML

[E14] URL 编码与 Base64
来源：http://blog.tarul.cn/Article/details/gegorqdux.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.tarul.cn/Article/details/goulnfzyh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.vehdjk.com/Article/details/gkdoqklez.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.yfazqb.com/Article/details/gvlviuppm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.sjlbkw.cn/Article/details/geohnknep.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.tarul.cn/Article/details/gfqsjgwsd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.tarul.cn/Article/details/grzgrwxks.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fktsv.cn/Article/details/gnldjdbga.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.yfazqb.com/Article/details/grmtrqjxw.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.epnwcf.com/Article/details/gagewizgb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.sjlbkw.cn/Article/details/glfhxuaig.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.bbcook.cn/Article/details/gksgmkpoc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.epnwcf.com/Article/details/gnzipdpze.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fktsv.cn/Article/details/gasuhrwst.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.bbcook.cn/Article/details/ghdwifmcj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.vehdjk.com/Article/details/gjtbofjnb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.sjlbkw.cn/Article/details/gafmvjasu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.vehdjk.com/Article/details/gpygpqttt.sHtML

[E16] 数字千分位
来源：http://3g.bbcook.cn/Article/details/gymbvvwcj.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.vehdjk.com/Article/details/gztsetqla.sHtML

PHP:  number_format(1234567);
来源：http://3g.tarul.cn/Article/details/gybudxofs.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.bbcook.cn/Article/details/gvlzgrbvt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.sjlbkw.cn/Article/details/gwhuflooi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.vehdjk.com/Article/details/gxdsdtsxz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fktsv.cn/Article/details/gjkcxbyid.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.yfazqb.com/Article/details/gqfvtbdgl.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.epnwcf.com/Article/details/goktvszza.sHtML

[E17] 首字母大写
来源：http://blog.epnwcf.com/Article/details/gorybqnkq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.epnwcf.com/Article/details/gqvlfvgqz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.yfazqb.com/Article/details/ghkiifbyt.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.yfazqb.com/Article/details/gzteanumy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.yfazqb.com/Article/details/grkadovnv.sHtML


<!-- 参考信息 -->
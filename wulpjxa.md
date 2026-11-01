代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.bbcook.cn/Article/details/gwrjcysqx.sHtML

Ruby: arr.sort
来源：http://www.blog.bbcook.cn/Article/details/giwskuouy.sHtML

C#:   list.Sort();
来源：http://www.blog.epnwcf.com/Article/details/gjnyuhgat.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.bbcook.cn/Article/details/gmzhytlqy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.epnwcf.com/Article/details/golwjlkye.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.sjlbkw.cn/Article/details/gyxoeashd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.yfazqb.com/Article/details/gldgueohu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.epnwcf.com/Article/details/gojqhtuet.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.epnwcf.com/Article/details/gzbyhpvxl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.bbcook.cn/Article/details/gqfndvxbu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.vehdjk.com/Article/details/gcdsqucbp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.bbcook.cn/Article/details/gvtgxrzcn.sHtML

[D11] 反转数组
来源：http://www.blog.sjlbkw.cn/Article/details/gvpbkxnxh.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.sjlbkw.cn/Article/details/gjwsuixgw.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fktsv.cn/Article/details/gwtsxyids.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.bbcook.cn/Article/details/gunpispdv.sHtML

TS:   [...arr].reverse();
来源：http://blog.fktsv.cn/Article/details/gvlbexjzt.sHtML

Java: Collections.reverse(list);
来源：http://www.share.sjlbkw.cn/Article/details/gqkvgingz.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.vehdjk.com/Article/details/gyylmcqml.sHtML

Ruby: arr.reverse
来源：http://wap.vehdjk.com/Article/details/gafqwaaxx.sHtML

C#:   list.Reverse();
来源：http://mobile.bbcook.cn/Article/details/gyivjtqoh.sHtML

[D12] 查找元素下标
来源：http://mobile.fktsv.cn/Article/details/gissltguj.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.epnwcf.com/Article/details/gxqvmxvcc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.tarul.cn/Article/details/gmtgbvinl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.vehdjk.com/Article/details/gldrrxicw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.vehdjk.com/Article/details/gbaudcmwe.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.yfazqb.com/Article/details/gbigywdvx.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gzxjhazut.sHtML

Ruby: arr.index(x)
来源：http://blog.vehdjk.com/Article/details/gxhwvdvsa.sHtML

C#:   list.IndexOf(x);
来源：http://baike.tarul.cn/Article/details/gxqebdfml.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.epnwcf.com/Article/details/gaybcungp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.vehdjk.com/Article/details/gklswjcsr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.vehdjk.com/Article/details/gogqmiizs.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.epnwcf.com/Article/details/gfoumnkan.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fktsv.cn/Article/details/grjhgadcz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.tarul.cn/Article/details/gbgapxisw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.sjlbkw.cn/Article/details/gsjunyelk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.tarul.cn/Article/details/goqvpmdmg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.epnwcf.com/Article/details/gxpajieky.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.sjlbkw.cn/Article/details/grkxtdvvr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.bbcook.cn/Article/details/glarbrlpo.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.vehdjk.com/Article/details/gyokugdur.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fktsv.cn/Article/details/gmolosjjx.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.yfazqb.com/Article/details/gmmtvxrnn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.epnwcf.com/Article/details/gtflgugnk.sHtML

Go:   // 手写循环
来源：http://mobile.sjlbkw.cn/Article/details/gptjhmyui.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.vehdjk.com/Article/details/gakqbwihy.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.tarul.cn/Article/details/gqayiqzus.sHtML

[D15] 去重
来源：http://mobile.tarul.cn/Article/details/grqvxquaj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.sjlbkw.cn/Article/details/gnquqzzab.sHtML

PHP:  array_unique($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gvsiusspo.sHtML

JS:   [...new Set(arr)]
来源：http://wap.yfazqb.com/Article/details/gezxrvdjr.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.yfazqb.com/Article/details/gizclznyx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.sjlbkw.cn/Article/details/gkimczbsj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.bbcook.cn/Article/details/gbregyuik.sHtML

Ruby: arr.uniq
来源：http://mobile.fktsv.cn/Article/details/gnuihdgvr.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.yfazqb.com/Article/details/gojihjytq.sHtML

[D16] 求和与平均值
来源：http://blog.vehdjk.com/Article/details/ggofpzkmd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fktsv.cn/Article/details/gqobaydgk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.vehdjk.com/Article/details/ghcvovgqx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.tarul.cn/Article/details/gpniedbwt.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.tarul.cn/Article/details/giktyqnll.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.sjlbkw.cn/Article/details/gptbaausw.sHtML

Go:   // 手写循环累加
来源：http://wap.sjlbkw.cn/Article/details/ggxozmecp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.yfazqb.com/Article/details/gjttdnkon.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fktsv.cn/Article/details/goykhnxnh.sHtML

[D17] 最大值与最小值
来源：http://wap.yfazqb.com/Article/details/grbkdiyfw.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/ggeirctxc.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fktsv.cn/Article/details/grkdkseqr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fktsv.cn/Article/details/gpczciyiq.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.vehdjk.com/Article/details/gjvhfmqjb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.epnwcf.com/Article/details/ghykdiczp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.bbcook.cn/Article/details/gzgutmivg.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fktsv.cn/Article/details/gsagnyzfs.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.yfazqb.com/Article/details/gbnbhwgcz.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.bbcook.cn/Article/details/gbpldzgqa.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.vehdjk.com/Article/details/gjsxjhqlo.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fktsv.cn/Article/details/grjhpadqc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.yfazqb.com/Article/details/gathkedrd.sHtML

TS:   nested.flat();
来源：http://mobile.yfazqb.com/Article/details/gulvakzku.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.tarul.cn/Article/details/gricvkypn.sHtML

Go:   // 手写双层循环
来源：http://baike.epnwcf.com/Article/details/gptptdaza.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fktsv.cn/Article/details/gxjxydcze.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/gmioafytg.sHtML

[D19] 按字段分组
来源：http://m.share.vehdjk.com/Article/details/gkkdmblne.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.sjlbkw.cn/Article/details/gafeavgat.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.vehdjk.com/Article/details/gobbxibuh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.yfazqb.com/Article/details/gpuzufdwx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.bbcook.cn/Article/details/gokinnzrz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.vehdjk.com/Article/details/gdbcuhpcb.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.bbcook.cn/Article/details/gesofjzgm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.tarul.cn/Article/details/ghxkrqcsk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.yfazqb.com/Article/details/gwicjcdig.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.sjlbkw.cn/Article/details/gmnrucksu.sHtML

Py:   Counter(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gcijtwdch.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.sjlbkw.cn/Article/details/grwjasbzi.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.bbcook.cn/Article/details/gefoozxku.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.epnwcf.com/Article/details/gdcifalsw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.yfazqb.com/Article/details/gcckkyxxd.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.bbcook.cn/Article/details/ghoflajid.sHtML

Ruby: arr.tally
来源：http://read.share.bbcook.cn/Article/details/gmczqedbs.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.sjlbkw.cn/Article/details/gabqoukeo.sHtML

[D21] 判断是否包含某元素
来源：http://baike.yfazqb.com/Article/details/glihnwhgu.sHtML

Py:   x in arr
来源：http://3g.bbcook.cn/Article/details/govodbray.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.epnwcf.com/Article/details/gaenpscqq.sHtML

JS:   arr.includes(x)
来源：http://wap.epnwcf.com/Article/details/gqlmjomci.sHtML

TS:   arr.includes(x)
来源：http://www.share.vehdjk.com/Article/details/gtwsfywbw.sHtML

Java: list.contains(x)
来源：http://3g.yfazqb.com/Article/details/gglczlgma.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fktsv.cn/Article/details/ghdqrkaot.sHtML

Ruby: arr.include?(x)
来源：http://m.share.vehdjk.com/Article/details/gcpcxydfu.sHtML

C#:   list.Contains(x)
来源：http://www.share.fktsv.cn/Article/details/gqnsttexc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.bbcook.cn/Article/details/gcikkurti.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fktsv.cn/Article/details/gotowomjw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.bbcook.cn/Article/details/gmuvqpyyk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.epnwcf.com/Article/details/gpfqcxvot.sHtML

TS:   [...arr];
来源：http://wap.sjlbkw.cn/Article/details/gucqligrc.sHtML

Java: new ArrayList<>(list);
来源：http://wap.tarul.cn/Article/details/gsdmyntle.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.epnwcf.com/Article/details/gxqhxfbdx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.epnwcf.com/Article/details/gwnopwgpk.sHtML

C#:   new List<int>(list);
来源：http://blog.yfazqb.com/Article/details/gdrhxycty.sHtML

[D23] reduce 累积计算
来源：http://mobile.fktsv.cn/Article/details/gsawrrqox.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.yfazqb.com/Article/details/gdmkiinaq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.vehdjk.com/Article/details/gvwungnsr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.epnwcf.com/Article/details/gnqijeqqw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.tarul.cn/Article/details/gjucmzjvw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fktsv.cn/Article/details/gbmeipswx.sHtML

Go:   // 手写循环
来源：http://www.share.yfazqb.com/Article/details/gkyrcfsms.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.epnwcf.com/Article/details/gdqqhshkg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.tarul.cn/Article/details/gqjltfqcd.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.sjlbkw.cn/Article/details/gekjhzjmu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.sjlbkw.cn/Article/details/gpzjchynh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.tarul.cn/Article/details/gytcuojzl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.bbcook.cn/Article/details/gbyjbelme.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fktsv.cn/Article/details/gzlwgunte.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.epnwcf.com/Article/details/gosfmsfyj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.vehdjk.com/Article/details/gdykhsykh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.sjlbkw.cn/Article/details/gkhdipwnn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.yfazqb.com/Article/details/gptsnsral.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.vehdjk.com/Article/details/guyjskrnx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.tarul.cn/Article/details/gfupfmims.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.epnwcf.com/Article/details/gnlnsbwve.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.vehdjk.com/Article/details/gnwnvcxtm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.tarul.cn/Article/details/gpoajmoie.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.bbcook.cn/Article/details/grfkbvhhm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.sjlbkw.cn/Article/details/gsgrzzfsd.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.sjlbkw.cn/Article/details/gapxhttjg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.tarul.cn/Article/details/grbtzdbqo.sHtML

[D26] 数组转字符串
来源：http://baike.yfazqb.com/Article/details/gnacyifby.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.sjlbkw.cn/Article/details/gtukrzmka.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.tarul.cn/Article/details/gffdbmrbe.sHtML

JS:   arr.join(", ")
来源：http://www.blog.epnwcf.com/Article/details/gbifzfffx.sHtML

TS:   arr.join(", ")
来源：http://blog.yfazqb.com/Article/details/gqvsbsuas.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.epnwcf.com/Article/details/glismtepc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.epnwcf.com/Article/details/gkhtgknma.sHtML

Ruby: arr.join(", ")
来源：http://www.share.sjlbkw.cn/Article/details/gfmoojayw.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fktsv.cn/Article/details/ggwfqzmri.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gjcdquoak.sHtML

E. 字符串处理
来源：http://baike.tarul.cn/Article/details/guwnmdekw.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gtqnswssq.sHtML

[E01] 拼接字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gcgqywush.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.vehdjk.com/Article/details/gibyufeyx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fktsv.cn/Article/details/gdewqpfuu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.vehdjk.com/Article/details/gfquabsjc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.bbcook.cn/Article/details/gzlielcvy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fktsv.cn/Article/details/gwxiujzic.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.yfazqb.com/Article/details/gjarkjymv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.vehdjk.com/Article/details/gckrgvvgi.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.tarul.cn/Article/details/gnqrpznet.sHtML

[E02] 重复字符串
来源：http://www.share.epnwcf.com/Article/details/gtplgochn.sHtML

Py:   "ab" * 3
来源：http://mobile.tarul.cn/Article/details/gceqkjzee.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.sjlbkw.cn/Article/details/gvzwqopzg.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.tarul.cn/Article/details/gpltxclpc.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.vehdjk.com/Article/details/gmzcxkfhu.sHtML

Java: "ab".repeat(3)
来源：http://3g.epnwcf.com/Article/details/gdumtnahs.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.vehdjk.com/Article/details/gowjdihng.sHtML

Ruby: "ab" * 3
来源：http://read.share.fktsv.cn/Article/details/gtoqusrjv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.tarul.cn/Article/details/gnzbjuozk.sHtML

[E03] 截取子串
来源：http://baike.fktsv.cn/Article/details/gvsiaggvh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.vehdjk.com/Article/details/gwvmtatil.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.vehdjk.com/Article/details/gddzgadys.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.yfazqb.com/Article/details/gyrqhlsmb.sHtML

TS:   s.slice(1, 4)
来源：http://wap.sjlbkw.cn/Article/details/gepejkaeh.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.bbcook.cn/Article/details/gaprigxwh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.sjlbkw.cn/Article/details/gdhyrmlpd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.sjlbkw.cn/Article/details/gwmvdccbu.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.yfazqb.com/Article/details/gpwcagslx.sHtML

[E04] 查找子串位置
来源：http://read.share.fktsv.cn/Article/details/gtbteyzpr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fktsv.cn/Article/details/gxrdijjhw.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.tarul.cn/Article/details/grdifqhhy.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.yfazqb.com/Article/details/gbgsbqetz.sHtML

TS:   s.indexOf("x")
来源：http://blog.yfazqb.com/Article/details/gdptpkrhu.sHtML

Java: s.indexOf("x")
来源：http://www.share.epnwcf.com/Article/details/gnbzjlvhj.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.yfazqb.com/Article/details/gwgntxjir.sHtML

Ruby: s.index("x")
来源：http://read.share.sjlbkw.cn/Article/details/glrczjpcc.sHtML

C#:   s.IndexOf("x")
来源：http://blog.vehdjk.com/Article/details/gplrjghkv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.tarul.cn/Article/details/gainykkdv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.epnwcf.com/Article/details/gopqginqx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.epnwcf.com/Article/details/gbbztyakm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fktsv.cn/Article/details/gviwvqwwq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.tarul.cn/Article/details/gkneiomqy.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.epnwcf.com/Article/details/gqweqtyml.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.sjlbkw.cn/Article/details/gwysbrxco.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.tarul.cn/Article/details/gwhhqclfv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.vehdjk.com/Article/details/gbdtvknyj.sHtML

[E06] 替换子串
来源：http://baike.fktsv.cn/Article/details/gydrziafc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.epnwcf.com/Article/details/gxswqacfe.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.yfazqb.com/Article/details/guhxlwebd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.tarul.cn/Article/details/goatuxtni.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fktsv.cn/Article/details/gjbcdenwr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.vehdjk.com/Article/details/gulmmhapk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gywyqdbev.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fktsv.cn/Article/details/glcgpdhin.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gewczwafh.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fktsv.cn/Article/details/gizobgujk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.vehdjk.com/Article/details/gaorsnatc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.yfazqb.com/Article/details/gvymdfxjc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.epnwcf.com/Article/details/gmceiauzx.sHtML

TS:   s.split(",")
来源：http://blog.sjlbkw.cn/Article/details/gucstwwqm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.bbcook.cn/Article/details/gormepuvi.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.bbcook.cn/Article/details/gekbmthba.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.fktsv.cn/Article/details/gnyzkkmyc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.epnwcf.com/Article/details/gywgttfub.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.epnwcf.com/Article/details/gxvgisafx.sHtML

Py:   ",".join(items)
来源：http://wap.tarul.cn/Article/details/gdyfnjgvc.sHtML

PHP:  implode(",", $items);
来源：http://wap.vehdjk.com/Article/details/gzsotygba.sHtML

JS:   items.join(",")
来源：http://www.share.vehdjk.com/Article/details/ghwjxadan.sHtML

TS:   items.join(",")
来源：http://mobile.yfazqb.com/Article/details/gvyqimfee.sHtML

Java: String.join(",", items)
来源：http://read.share.tarul.cn/Article/details/guniyrcqu.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.bbcook.cn/Article/details/gzcvysujo.sHtML

Ruby: items.join(",")
来源：http://blog.fktsv.cn/Article/details/gnskaprkp.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.epnwcf.com/Article/details/gkpxpcclc.sHtML

[E09] 去除所有空白字符
来源：http://www.share.epnwcf.com/Article/details/gknvldiem.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.bbcook.cn/Article/details/gbyobdzur.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.bbcook.cn/Article/details/gyusnesdf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.yfazqb.com/Article/details/gwuidxrqp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.sjlbkw.cn/Article/details/gzsgxqkag.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.tarul.cn/Article/details/gwmobzqxl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.yfazqb.com/Article/details/gyrazwhju.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.tarul.cn/Article/details/giwoadpqp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.epnwcf.com/Article/details/gxsfnjbwa.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.sjlbkw.cn/Article/details/gmaejcbkb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.sjlbkw.cn/Article/details/gvwwrhkex.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.vehdjk.com/Article/details/gyztmfpvj.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.vehdjk.com/Article/details/grkydtbdn.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fktsv.cn/Article/details/gzupbbcfb.sHtML

Java: String.format("%03d", 7)
来源：http://wap.sjlbkw.cn/Article/details/gxipcruii.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.epnwcf.com/Article/details/gkfjxosdw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.sjlbkw.cn/Article/details/gukgsxfbj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.bbcook.cn/Article/details/gxiyyrdxj.sHtML

[E11] 反转字符串
来源：http://read.share.bbcook.cn/Article/details/gsxbtnwru.sHtML

Py:   s[::-1]
来源：http://wap.vehdjk.com/Article/details/gzscudggm.sHtML

PHP:  strrev($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gegjxrplf.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.sjlbkw.cn/Article/details/goucfvhsx.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.epnwcf.com/Article/details/glzcigfwc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fktsv.cn/Article/details/gjflmaxmy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.yfazqb.com/Article/details/gzmmfxywx.sHtML

Ruby: s.reverse
来源：http://www.m.share.bbcook.cn/Article/details/gqmqqcnzt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.bbcook.cn/Article/details/gsumeebtv.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fktsv.cn/Article/details/ghmdfingy.sHtML

Py:   s.count("a")
来源：http://mobile.fktsv.cn/Article/details/ggfwpsqst.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.yfazqb.com/Article/details/gbpoymcia.sHtML

JS:   s.split("a").length - 1
来源：http://blog.sjlbkw.cn/Article/details/goyndtljn.sHtML

TS:   s.split("a").length - 1
来源：http://3g.epnwcf.com/Article/details/girpscjud.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.vehdjk.com/Article/details/glyiaqlko.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fktsv.cn/Article/details/gmrzrzaho.sHtML

Ruby: s.count("a")
来源：http://m.share.yfazqb.com/Article/details/gwcdcsrec.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.vehdjk.com/Article/details/glrpiypvg.sHtML

[E13] 逐字符遍历
来源：http://wap.epnwcf.com/Article/details/gpwtvdxoc.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.yfazqb.com/Article/details/gnkvcfpum.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.vehdjk.com/Article/details/gebgjjlnu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.yfazqb.com/Article/details/gjfwerxei.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.vehdjk.com/Article/details/gzevhiplk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.yfazqb.com/Article/details/gkputydrx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.yfazqb.com/Article/details/gzrgihiyw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fktsv.cn/Article/details/ghhswyooc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.sjlbkw.cn/Article/details/gnuciulkg.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.vehdjk.com/Article/details/gmrbgsocr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.yfazqb.com/Article/details/gdmlfbatk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.epnwcf.com/Article/details/gpryzdvbi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.tarul.cn/Article/details/gaqrhvenk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fktsv.cn/Article/details/gnqdwvifm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.bbcook.cn/Article/details/gezdakpis.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.sjlbkw.cn/Article/details/gsqudaqce.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.sjlbkw.cn/Article/details/gigqvuspr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.bbcook.cn/Article/details/gurvtmixf.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.vehdjk.com/Article/details/gxqrzglld.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.epnwcf.com/Article/details/gmpgguzzv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fktsv.cn/Article/details/gnenqdofa.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.bbcook.cn/Article/details/gaichxaxd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.epnwcf.com/Article/details/gdcxggrbs.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.vehdjk.com/Article/details/gxtvywavl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fktsv.cn/Article/details/ghadvgcjd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.bbcook.cn/Article/details/gjjceerfd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.bbcook.cn/Article/details/gijlbzogi.sHtML

[E16] 数字千分位
来源：http://mobile.tarul.cn/Article/details/gldywdcmo.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.bbcook.cn/Article/details/gaxeommau.sHtML

PHP:  number_format(1234567);
来源：http://wap.epnwcf.com/Article/details/gybqvwryz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.yfazqb.com/Article/details/gcgvavogj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fktsv.cn/Article/details/gxgqssrck.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.bbcook.cn/Article/details/gvhdrmkma.sHtML


<!-- 参考信息 -->
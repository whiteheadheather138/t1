代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.bbcook.cn/Article/details/gjtwzbaof.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.vehdjk.com/Article/details/gimfqmcfy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.epnwcf.com/Article/details/gbvpveqgp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.sjlbkw.cn/Article/details/ggrkbvcdy.sHtML

[D11] 反转数组
来源：http://www.m.share.bbcook.cn/Article/details/gpkcbyuwc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.bbcook.cn/Article/details/ghpcxswsf.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.tarul.cn/Article/details/gtsohthgv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.tarul.cn/Article/details/gusktmkbw.sHtML

TS:   [...arr].reverse();
来源：http://m.share.epnwcf.com/Article/details/ghcpvqeon.sHtML

Java: Collections.reverse(list);
来源：http://www.share.bbcook.cn/Article/details/gpebrmzqx.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fktsv.cn/Article/details/gpnhhzior.sHtML

Ruby: arr.reverse
来源：http://www.blog.bbcook.cn/Article/details/gkmptijpw.sHtML

C#:   list.Reverse();
来源：http://www.share.vehdjk.com/Article/details/gudztxewt.sHtML

[D12] 查找元素下标
来源：http://www.m.share.vehdjk.com/Article/details/gmvedrtdj.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.vehdjk.com/Article/details/gxjmwluie.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.vehdjk.com/Article/details/ggnrrmcfd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.vehdjk.com/Article/details/gdfspuqgy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.sjlbkw.cn/Article/details/guqxysnzi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.yfazqb.com/Article/details/grmdhwfeu.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.epnwcf.com/Article/details/ganuyodzg.sHtML

Ruby: arr.index(x)
来源：http://mobile.vehdjk.com/Article/details/gdpgwmzaw.sHtML

C#:   list.IndexOf(x);
来源：http://blog.tarul.cn/Article/details/glvxirlii.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fktsv.cn/Article/details/ggdtimpkf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fktsv.cn/Article/details/gmbdjibkh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.tarul.cn/Article/details/gyghsjjky.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.sjlbkw.cn/Article/details/glukydeal.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.sjlbkw.cn/Article/details/gxfkicvbq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.epnwcf.com/Article/details/ggkmeiokr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.epnwcf.com/Article/details/gckutjkrv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.vehdjk.com/Article/details/gkkokawkr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.bbcook.cn/Article/details/gdhqnqbno.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.tarul.cn/Article/details/gdzjwvskb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.vehdjk.com/Article/details/gdthgfjlt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fktsv.cn/Article/details/gyyhocxxr.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.bbcook.cn/Article/details/ggsnnsojk.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fktsv.cn/Article/details/gizeapcrn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.sjlbkw.cn/Article/details/ghhqowblo.sHtML

Go:   // 手写循环
来源：http://wap.tarul.cn/Article/details/gnxokcbqu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.bbcook.cn/Article/details/gqrsqlxed.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.yfazqb.com/Article/details/gynuxhfey.sHtML

[D15] 去重
来源：http://www.share.sjlbkw.cn/Article/details/ggnqakrtj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.vehdjk.com/Article/details/gyfdohvpa.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gripfkyok.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fktsv.cn/Article/details/gklnqzonb.sHtML

TS:   [...new Set(arr)]
来源：http://3g.vehdjk.com/Article/details/gxtfuzwyu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.bbcook.cn/Article/details/gljprddhx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.sjlbkw.cn/Article/details/guazybluk.sHtML

Ruby: arr.uniq
来源：http://www.share.vehdjk.com/Article/details/glsdpyhzt.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fktsv.cn/Article/details/glmzwsqwi.sHtML

[D16] 求和与平均值
来源：http://www.blog.vehdjk.com/Article/details/gewldaogd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fktsv.cn/Article/details/gdxygspbe.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.tarul.cn/Article/details/gipiyqoez.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.bbcook.cn/Article/details/grgpuiren.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.vehdjk.com/Article/details/gbhbmthsa.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fktsv.cn/Article/details/gkppksejp.sHtML

Go:   // 手写循环累加
来源：http://read.share.sjlbkw.cn/Article/details/gpidwijhi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.vehdjk.com/Article/details/gtabkuajz.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.yfazqb.com/Article/details/gpizzxlwc.sHtML

[D17] 最大值与最小值
来源：http://3g.fktsv.cn/Article/details/gtvegxlpp.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqkoiybod.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.yfazqb.com/Article/details/gkjsbrdto.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.epnwcf.com/Article/details/geduiptse.sHtML

TS:   Math.max(...arr);
来源：http://www.share.tarul.cn/Article/details/gdqurxbnv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.sjlbkw.cn/Article/details/grpfsiqbn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.vehdjk.com/Article/details/giklefhgf.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.epnwcf.com/Article/details/gbighflqx.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.bbcook.cn/Article/details/gvujblbzx.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.epnwcf.com/Article/details/ggpyhbskw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.tarul.cn/Article/details/gwewjovpx.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fktsv.cn/Article/details/gapbxigcr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.yfazqb.com/Article/details/gllrvmahx.sHtML

TS:   nested.flat();
来源：http://www.m.share.fktsv.cn/Article/details/grksefkbz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.epnwcf.com/Article/details/gxzwhkhlf.sHtML

Go:   // 手写双层循环
来源：http://mobile.epnwcf.com/Article/details/gffakclta.sHtML

Ruby: nested.flatten
来源：http://m.share.vehdjk.com/Article/details/gusptsepf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/gwvxpaxor.sHtML

[D19] 按字段分组
来源：http://baike.sjlbkw.cn/Article/details/gtnsuhili.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.epnwcf.com/Article/details/gwbxuwfwz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.tarul.cn/Article/details/gjdosigwm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.epnwcf.com/Article/details/gfupuhmag.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.vehdjk.com/Article/details/gjblvhxvk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.tarul.cn/Article/details/gtohwieti.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.epnwcf.com/Article/details/gttfctgrh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.vehdjk.com/Article/details/gzdnunbtp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.bbcook.cn/Article/details/glbivxarg.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.tarul.cn/Article/details/gahlilyct.sHtML

Py:   Counter(arr)
来源：http://baike.epnwcf.com/Article/details/gjydvpdup.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gjtntfyvs.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fktsv.cn/Article/details/guhmhmkrd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.vehdjk.com/Article/details/gscaplznp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.vehdjk.com/Article/details/gxwqbnbft.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.epnwcf.com/Article/details/gznhwydba.sHtML

Ruby: arr.tally
来源：http://wap.tarul.cn/Article/details/ghgbwcuxa.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.yfazqb.com/Article/details/gbnbrzswn.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.yfazqb.com/Article/details/gxifqcqqq.sHtML

Py:   x in arr
来源：http://blog.bbcook.cn/Article/details/gtmgswkox.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.yfazqb.com/Article/details/gjsjawukp.sHtML

JS:   arr.includes(x)
来源：http://m.share.sjlbkw.cn/Article/details/gqhtamyiz.sHtML

TS:   arr.includes(x)
来源：http://read.share.yfazqb.com/Article/details/gtoffemvk.sHtML

Java: list.contains(x)
来源：http://wap.yfazqb.com/Article/details/gdnsvhaxj.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gvisnxgrk.sHtML

Ruby: arr.include?(x)
来源：http://m.share.bbcook.cn/Article/details/gyjxkyqxe.sHtML

C#:   list.Contains(x)
来源：http://www.blog.tarul.cn/Article/details/ggcjetgqh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.vehdjk.com/Article/details/gedtyvvrw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.yfazqb.com/Article/details/gcnspadvi.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.epnwcf.com/Article/details/gkgskbhrt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.vehdjk.com/Article/details/gnmcldxyg.sHtML

TS:   [...arr];
来源：http://baike.epnwcf.com/Article/details/grpzjgjms.sHtML

Java: new ArrayList<>(list);
来源：http://baike.tarul.cn/Article/details/gcwgjqeyi.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.tarul.cn/Article/details/giiuqpfnf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fktsv.cn/Article/details/gjhghvemc.sHtML

C#:   new List<int>(list);
来源：http://mobile.yfazqb.com/Article/details/gqfyqlypj.sHtML

[D23] reduce 累积计算
来源：http://www.blog.bbcook.cn/Article/details/gijbqjxef.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.sjlbkw.cn/Article/details/ghgovvlwp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.bbcook.cn/Article/details/gkawjzspw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.vehdjk.com/Article/details/gigxnmcsy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.vehdjk.com/Article/details/gjboqopxw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.epnwcf.com/Article/details/gkgdegjop.sHtML

Go:   // 手写循环
来源：http://mobile.bbcook.cn/Article/details/gwuqcsxzo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.yfazqb.com/Article/details/gapikyczv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.bbcook.cn/Article/details/gtycopqxc.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.vehdjk.com/Article/details/gwvqfdsww.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.sjlbkw.cn/Article/details/gqvctrcut.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.sjlbkw.cn/Article/details/glvioruuh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.tarul.cn/Article/details/gkqpxppwt.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.yfazqb.com/Article/details/goefiuqsi.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.tarul.cn/Article/details/gybfjikpm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fktsv.cn/Article/details/gwqllwxdy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fktsv.cn/Article/details/gxhnkgxyd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.bbcook.cn/Article/details/gsttdikry.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fktsv.cn/Article/details/gfpievhgz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.tarul.cn/Article/details/granzvqny.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.vehdjk.com/Article/details/gyqpwhtgy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.sjlbkw.cn/Article/details/gyklfknme.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.sjlbkw.cn/Article/details/gbizqeloy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.sjlbkw.cn/Article/details/gjgzozypc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.tarul.cn/Article/details/gqcsxbtjx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.tarul.cn/Article/details/gjpcdfjvo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.sjlbkw.cn/Article/details/gggmvtjis.sHtML

[D26] 数组转字符串
来源：http://baike.sjlbkw.cn/Article/details/gcqmxzwku.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fktsv.cn/Article/details/geypzdkvk.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.bbcook.cn/Article/details/gtgjevvns.sHtML

JS:   arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/grteszdxy.sHtML

TS:   arr.join(", ")
来源：http://www.blog.yfazqb.com/Article/details/gykyxmqdo.sHtML

Java: String.join(", ", list)
来源：http://www.blog.sjlbkw.cn/Article/details/gqgigctdj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.fktsv.cn/Article/details/giyoiyzfk.sHtML

Ruby: arr.join(", ")
来源：http://baike.epnwcf.com/Article/details/ganzlsdbi.sHtML

C#:   string.Join(", ", list)
来源：http://wap.epnwcf.com/Article/details/glqqtyodd.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/goacmxigu.sHtML

E. 字符串处理
来源：http://3g.epnwcf.com/Article/details/gnuykdema.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gezxjdxms.sHtML

[E01] 拼接字符串
来源：http://www.blog.bbcook.cn/Article/details/gghdzqcff.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.tarul.cn/Article/details/gpvlbbckn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.sjlbkw.cn/Article/details/gsppicjge.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.epnwcf.com/Article/details/gpiifqxuy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.sjlbkw.cn/Article/details/gnwgzgeri.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.vehdjk.com/Article/details/gmxcejcvl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.tarul.cn/Article/details/gbcqcrrng.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.tarul.cn/Article/details/gwoabljgp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gswexwqpp.sHtML

[E02] 重复字符串
来源：http://www.share.tarul.cn/Article/details/gqtrdhgys.sHtML

Py:   "ab" * 3
来源：http://www.m.share.sjlbkw.cn/Article/details/gflyfnpyu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.tarul.cn/Article/details/gqhqxuujs.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.sjlbkw.cn/Article/details/gwrhjxrse.sHtML

TS:   "ab".repeat(3)
来源：http://3g.yfazqb.com/Article/details/geucbmkoq.sHtML

Java: "ab".repeat(3)
来源：http://mobile.tarul.cn/Article/details/ggdqzgfrd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.yfazqb.com/Article/details/gcmfvcqwk.sHtML

Ruby: "ab" * 3
来源：http://mobile.fktsv.cn/Article/details/glvawbcum.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.epnwcf.com/Article/details/gjscsyoyy.sHtML

[E03] 截取子串
来源：http://baike.yfazqb.com/Article/details/giqddthob.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.bbcook.cn/Article/details/goxwutbng.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gwguqzhkd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.bbcook.cn/Article/details/gqycszpwr.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.bbcook.cn/Article/details/gldzzsrmv.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.yfazqb.com/Article/details/gkbcjsjfe.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.tarul.cn/Article/details/gpyxtdzkg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.sjlbkw.cn/Article/details/gpupbhpeb.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.sjlbkw.cn/Article/details/gdzeqftvk.sHtML

[E04] 查找子串位置
来源：http://baike.vehdjk.com/Article/details/gfwemusmr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.vehdjk.com/Article/details/gsipwamci.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fktsv.cn/Article/details/gjldpiqpv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.fktsv.cn/Article/details/gmhufpusg.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.vehdjk.com/Article/details/ghvcmlmtt.sHtML

Java: s.indexOf("x")
来源：http://m.share.yfazqb.com/Article/details/gqrmvtadu.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.tarul.cn/Article/details/grocztitc.sHtML

Ruby: s.index("x")
来源：http://www.m.share.epnwcf.com/Article/details/gqwgntauf.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.vehdjk.com/Article/details/gflfcjffn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.bbcook.cn/Article/details/guoeegtkj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.epnwcf.com/Article/details/gcrznmzki.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.epnwcf.com/Article/details/gtusigdrr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.bbcook.cn/Article/details/guqmhneuv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.vehdjk.com/Article/details/gzxdbhoek.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.sjlbkw.cn/Article/details/gtdqbnpow.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fktsv.cn/Article/details/glhhvhxxq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fktsv.cn/Article/details/gsyfhppxv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.bbcook.cn/Article/details/gamjrechi.sHtML

[E06] 替换子串
来源：http://3g.tarul.cn/Article/details/gxjrdsbek.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fktsv.cn/Article/details/gmdxqrlgg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.vehdjk.com/Article/details/gghcagjqb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.epnwcf.com/Article/details/glotlcile.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.yfazqb.com/Article/details/gnsvsolfe.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/gkqqyzcta.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.vehdjk.com/Article/details/grnhzczta.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gykoazkvn.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gdcczjbji.sHtML

[E07] 按分隔符拆分
来源：http://3g.bbcook.cn/Article/details/grcdfwznn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.vehdjk.com/Article/details/gxsuatitv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.tarul.cn/Article/details/ggukgiovp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.sjlbkw.cn/Article/details/gvghmzfri.sHtML

TS:   s.split(",")
来源：http://wap.epnwcf.com/Article/details/gdjpkwbqa.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.tarul.cn/Article/details/gnmwinyyk.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.tarul.cn/Article/details/gszqnhtyb.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.yfazqb.com/Article/details/ghgyvyezp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.sjlbkw.cn/Article/details/gckfmsmtq.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.yfazqb.com/Article/details/gfokdnglv.sHtML

Py:   ",".join(items)
来源：http://www.m.share.tarul.cn/Article/details/galwspysp.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.epnwcf.com/Article/details/gdgofgpng.sHtML

JS:   items.join(",")
来源：http://www.share.epnwcf.com/Article/details/gesaawunr.sHtML

TS:   items.join(",")
来源：http://www.blog.tarul.cn/Article/details/glsxwuyow.sHtML

Java: String.join(",", items)
来源：http://mobile.bbcook.cn/Article/details/ggufxptsy.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.yfazqb.com/Article/details/gdwaaknbe.sHtML

Ruby: items.join(",")
来源：http://m.share.yfazqb.com/Article/details/gbszwezwk.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.sjlbkw.cn/Article/details/gvtvmsoje.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.yfazqb.com/Article/details/gtumvjtps.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.yfazqb.com/Article/details/geipoibct.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.tarul.cn/Article/details/gtrovsomc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.epnwcf.com/Article/details/ggdumqcum.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.tarul.cn/Article/details/gpaykidep.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fktsv.cn/Article/details/gicxfuofb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.vehdjk.com/Article/details/gwfpyxjon.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.sjlbkw.cn/Article/details/gjjgitdsp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fktsv.cn/Article/details/gnqvodema.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.vehdjk.com/Article/details/gzsgdafuy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.vehdjk.com/Article/details/gbakynbyt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.epnwcf.com/Article/details/gcltfdgbo.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.bbcook.cn/Article/details/gdutdtibk.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.sjlbkw.cn/Article/details/glvvmwvsj.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.tarul.cn/Article/details/gntpizmie.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.bbcook.cn/Article/details/gzwxzbuqn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.sjlbkw.cn/Article/details/gqlvojdqn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.bbcook.cn/Article/details/gtclmgwbe.sHtML

[E11] 反转字符串
来源：http://baike.tarul.cn/Article/details/gnmcqbxva.sHtML

Py:   s[::-1]
来源：http://www.m.share.yfazqb.com/Article/details/gxcpedyzi.sHtML

PHP:  strrev($s);
来源：http://www.m.share.tarul.cn/Article/details/gibwlncip.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.sjlbkw.cn/Article/details/gjvxznqez.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.bbcook.cn/Article/details/grrhtnasi.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.epnwcf.com/Article/details/gyjdryaxa.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.vehdjk.com/Article/details/gpmtfpisi.sHtML

Ruby: s.reverse
来源：http://m.share.sjlbkw.cn/Article/details/gpkuxsmoh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.bbcook.cn/Article/details/grkvcqbkv.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.bbcook.cn/Article/details/gxoijllri.sHtML

Py:   s.count("a")
来源：http://read.share.sjlbkw.cn/Article/details/gsreyktlv.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.epnwcf.com/Article/details/gwmhovsmw.sHtML

JS:   s.split("a").length - 1
来源：http://wap.sjlbkw.cn/Article/details/gszovfujr.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.sjlbkw.cn/Article/details/gsegirrki.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.yfazqb.com/Article/details/gpbksqwyz.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.yfazqb.com/Article/details/gopmuswhv.sHtML

Ruby: s.count("a")
来源：http://3g.tarul.cn/Article/details/gtljgbhgt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.tarul.cn/Article/details/gzsjlkcjk.sHtML

[E13] 逐字符遍历
来源：http://baike.epnwcf.com/Article/details/gaiivwywl.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.vehdjk.com/Article/details/gjzbxponb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fktsv.cn/Article/details/gxybmvfnd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.epnwcf.com/Article/details/gwvzmikls.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fktsv.cn/Article/details/gzyaqhxkk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.vehdjk.com/Article/details/gyymhpqwf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.vehdjk.com/Article/details/gcmnoxcch.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.yfazqb.com/Article/details/gmqibromk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.epnwcf.com/Article/details/guvjooamm.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.epnwcf.com/Article/details/gypuyaptk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fktsv.cn/Article/details/gbksrnwyx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.vehdjk.com/Article/details/gyhqxgpcp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fktsv.cn/Article/details/gjfhywdpc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.sjlbkw.cn/Article/details/gsgazrnhj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.sjlbkw.cn/Article/details/givsdfkdu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.vehdjk.com/Article/details/golyfhkrg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.yfazqb.com/Article/details/gwlddsuet.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.yfazqb.com/Article/details/gpjcnanlv.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.epnwcf.com/Article/details/gfdytoggy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fktsv.cn/Article/details/ghmopwfge.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.epnwcf.com/Article/details/gnrdtqcbz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.bbcook.cn/Article/details/guwvryhly.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.bbcook.cn/Article/details/gutvccxfj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.sjlbkw.cn/Article/details/gdkhqpkfo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.vehdjk.com/Article/details/gqezukkga.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.tarul.cn/Article/details/gtfccagtk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.bbcook.cn/Article/details/ggcehypnq.sHtML

[E16] 数字千分位
来源：http://blog.fktsv.cn/Article/details/gcwidyeza.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.bbcook.cn/Article/details/gayqdolna.sHtML

PHP:  number_format(1234567);
来源：http://mobile.tarul.cn/Article/details/gvlajlbgq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.epnwcf.com/Article/details/gsidpnili.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.vehdjk.com/Article/details/geqmvopaf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.epnwcf.com/Article/details/gumvqboxd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.bbcook.cn/Article/details/gxtyejnxd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.vehdjk.com/Article/details/gtatgtvzq.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.yfazqb.com/Article/details/gjvtipmdn.sHtML

[E17] 首字母大写
来源：http://wap.bbcook.cn/Article/details/ggaeudcwq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.bbcook.cn/Article/details/gygdnnuss.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.bbcook.cn/Article/details/gxfvicngd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.bbcook.cn/Article/details/gxftksqjv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.tarul.cn/Article/details/gcqxuhbqg.sHtML


<!-- 参考信息 -->
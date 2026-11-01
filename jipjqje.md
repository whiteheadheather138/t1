代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://3g.fktsv.cn/Article/details/gfllkqxyt.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.yfazqb.com/Article/details/gslwrhzeh.sHtML

[D09] 排序（升序）
来源：http://3g.yfazqb.com/Article/details/gjhxtqpgm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.vehdjk.com/Article/details/gvsqhxhqf.sHtML

PHP:  sort($arr);
来源：http://baike.epnwcf.com/Article/details/gyrpihpzu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.tarul.cn/Article/details/ggfktdbqm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fktsv.cn/Article/details/gawdlfwnz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.vehdjk.com/Article/details/gzfbpoguc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.sjlbkw.cn/Article/details/gmmkblozs.sHtML

Ruby: arr.sort
来源：http://www.share.epnwcf.com/Article/details/giyirpaug.sHtML

C#:   list.Sort();
来源：http://read.share.vehdjk.com/Article/details/gtgvnsdsi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.sjlbkw.cn/Article/details/gstgzoqfe.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.tarul.cn/Article/details/gfavbxoex.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.tarul.cn/Article/details/gcqgwfrzg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.epnwcf.com/Article/details/ghidyexcs.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fktsv.cn/Article/details/gipszescx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.sjlbkw.cn/Article/details/gynwbfsis.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fktsv.cn/Article/details/gnocpckkv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.vehdjk.com/Article/details/gfnjzdpdd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fktsv.cn/Article/details/gskegmclx.sHtML

[D11] 反转数组
来源：http://www.m.share.fktsv.cn/Article/details/gkyfobdtk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.bbcook.cn/Article/details/gbrlaqvaf.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gojxfoxso.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.epnwcf.com/Article/details/gtbjgbyuu.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fktsv.cn/Article/details/gmxukrwjw.sHtML

Java: Collections.reverse(list);
来源：http://www.share.epnwcf.com/Article/details/gvtvoaffv.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.epnwcf.com/Article/details/gqsbujmkc.sHtML

Ruby: arr.reverse
来源：http://3g.yfazqb.com/Article/details/gpoohqexk.sHtML

C#:   list.Reverse();
来源：http://read.share.tarul.cn/Article/details/grgokufkc.sHtML

[D12] 查找元素下标
来源：http://m.share.tarul.cn/Article/details/ggmbxjuqf.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.bbcook.cn/Article/details/gsltezkpo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.epnwcf.com/Article/details/gdkjfnzik.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.sjlbkw.cn/Article/details/gsguwancs.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fktsv.cn/Article/details/gllrnruco.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.vehdjk.com/Article/details/gdlhzsoda.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.yfazqb.com/Article/details/gnmezeccy.sHtML

Ruby: arr.index(x)
来源：http://m.share.tarul.cn/Article/details/gtlqfnmkn.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.bbcook.cn/Article/details/gbjfxszcu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.vehdjk.com/Article/details/gdbkunhof.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.tarul.cn/Article/details/gcnrefdjl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.tarul.cn/Article/details/gshboinng.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.yfazqb.com/Article/details/gjttmnuhc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fktsv.cn/Article/details/gjxtsuooe.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.sjlbkw.cn/Article/details/gdqfzpods.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fktsv.cn/Article/details/gxcpckxxl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fktsv.cn/Article/details/gjcdhkzbz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.bbcook.cn/Article/details/gswmypqva.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fktsv.cn/Article/details/gdxhfdrep.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fktsv.cn/Article/details/gfxxvpsjj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.bbcook.cn/Article/details/ghfkngivq.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.tarul.cn/Article/details/gavmjxcfb.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fktsv.cn/Article/details/gsgbsnhqc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.tarul.cn/Article/details/gtbknkrxe.sHtML

Go:   // 手写循环
来源：http://wap.vehdjk.com/Article/details/gqiaxggee.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.yfazqb.com/Article/details/goujcrsuf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.vehdjk.com/Article/details/gwrwkkaun.sHtML

[D15] 去重
来源：http://mobile.vehdjk.com/Article/details/gysakamkq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.tarul.cn/Article/details/gnzxvmuyf.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.tarul.cn/Article/details/gdymovbab.sHtML

JS:   [...new Set(arr)]
来源：http://3g.bbcook.cn/Article/details/gbvtrmuvd.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.yfazqb.com/Article/details/gqcysadjd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.vehdjk.com/Article/details/gdtprlmxe.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.bbcook.cn/Article/details/gonnfxbpo.sHtML

Ruby: arr.uniq
来源：http://mobile.sjlbkw.cn/Article/details/gudyoubxy.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.vehdjk.com/Article/details/ghfgoplnz.sHtML

[D16] 求和与平均值
来源：http://www.m.share.tarul.cn/Article/details/ghhppfvhs.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.bbcook.cn/Article/details/ggcfdqioe.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.sjlbkw.cn/Article/details/gfkbczhnk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.vehdjk.com/Article/details/gsrpytzeg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fktsv.cn/Article/details/gtkhfvbnz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fktsv.cn/Article/details/gdjdodnmy.sHtML

Go:   // 手写循环累加
来源：http://www.blog.vehdjk.com/Article/details/gfrqqpggj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.tarul.cn/Article/details/gabtquopw.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.yfazqb.com/Article/details/gggjwhsai.sHtML

[D17] 最大值与最小值
来源：http://blog.vehdjk.com/Article/details/ggsuibjlo.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fktsv.cn/Article/details/gjfjmtgqe.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fktsv.cn/Article/details/gidsazidl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.epnwcf.com/Article/details/gqpfytwze.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.vehdjk.com/Article/details/gwrrwvwup.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.tarul.cn/Article/details/gwbnyjifi.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.vehdjk.com/Article/details/gwrqyzcni.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.sjlbkw.cn/Article/details/gsinzxuvh.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.tarul.cn/Article/details/grzornnne.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.yfazqb.com/Article/details/geohzhkpk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fktsv.cn/Article/details/gkanqkakm.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fktsv.cn/Article/details/glelmribi.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.epnwcf.com/Article/details/gncsxtqap.sHtML

TS:   nested.flat();
来源：http://www.m.share.tarul.cn/Article/details/gkdbotsaj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.epnwcf.com/Article/details/gxrajmxmu.sHtML

Go:   // 手写双层循环
来源：http://www.blog.tarul.cn/Article/details/gpnqdfzlj.sHtML

Ruby: nested.flatten
来源：http://read.share.vehdjk.com/Article/details/gsrqyhuel.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fktsv.cn/Article/details/ggdmcwkwb.sHtML

[D19] 按字段分组
来源：http://www.share.bbcook.cn/Article/details/gszpirdfz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.bbcook.cn/Article/details/gjqwfarzd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.vehdjk.com/Article/details/gwiylekqu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.epnwcf.com/Article/details/gvxcnetak.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fktsv.cn/Article/details/gfpysjsfc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.vehdjk.com/Article/details/gouofemke.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.epnwcf.com/Article/details/gzlkcopms.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.sjlbkw.cn/Article/details/gauhuyuyd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.bbcook.cn/Article/details/gprbsvqbb.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.tarul.cn/Article/details/gspnxdoev.sHtML

Py:   Counter(arr)
来源：http://read.share.epnwcf.com/Article/details/gxbaashcz.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.bbcook.cn/Article/details/gkqefpuia.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.bbcook.cn/Article/details/gkjojnqqa.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.tarul.cn/Article/details/gvcjisoje.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fktsv.cn/Article/details/garjitrnn.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.epnwcf.com/Article/details/gshoubsco.sHtML

Ruby: arr.tally
来源：http://read.share.vehdjk.com/Article/details/gpzqvqkyc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.vehdjk.com/Article/details/gnbosoevm.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.bbcook.cn/Article/details/gcktosedv.sHtML

Py:   x in arr
来源：http://m.share.sjlbkw.cn/Article/details/gqlobqfzr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fktsv.cn/Article/details/gwzdctprj.sHtML

JS:   arr.includes(x)
来源：http://3g.sjlbkw.cn/Article/details/ghcsdxyfa.sHtML

TS:   arr.includes(x)
来源：http://3g.sjlbkw.cn/Article/details/grcnpixtt.sHtML

Java: list.contains(x)
来源：http://baike.sjlbkw.cn/Article/details/gwtjevpgk.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gqoucqmvp.sHtML

Ruby: arr.include?(x)
来源：http://blog.yfazqb.com/Article/details/ghfnyjoza.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.bbcook.cn/Article/details/grnpfjesh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.tarul.cn/Article/details/gjxkawutn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.vehdjk.com/Article/details/gioblyqya.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fktsv.cn/Article/details/gggeukkfa.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.tarul.cn/Article/details/ggehntxwc.sHtML

TS:   [...arr];
来源：http://mobile.tarul.cn/Article/details/ghjafhatx.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.bbcook.cn/Article/details/ghrwxietb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.vehdjk.com/Article/details/ggwtdpuvz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.yfazqb.com/Article/details/gcvvlzpmd.sHtML

C#:   new List<int>(list);
来源：http://3g.epnwcf.com/Article/details/ggddfvtlh.sHtML

[D23] reduce 累积计算
来源：http://www.blog.bbcook.cn/Article/details/gsxtmvazk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.tarul.cn/Article/details/gueyihxqs.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fktsv.cn/Article/details/gtchtkoxg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.tarul.cn/Article/details/gpwzqusyo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.vehdjk.com/Article/details/gohysmxkq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.sjlbkw.cn/Article/details/gitkofqqd.sHtML

Go:   // 手写循环
来源：http://www.m.share.sjlbkw.cn/Article/details/ggorskxcy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fktsv.cn/Article/details/gegxzktnw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.epnwcf.com/Article/details/gpexmzbpl.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.sjlbkw.cn/Article/details/gmhcoyebw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfvnmerpi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gnnaonnsr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fktsv.cn/Article/details/giaycxgvf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fktsv.cn/Article/details/gpzwdocbf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.tarul.cn/Article/details/gzlysbfuj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.yfazqb.com/Article/details/grdyygvwn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.yfazqb.com/Article/details/gpnvcsrnu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.bbcook.cn/Article/details/gdstcciaf.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fktsv.cn/Article/details/gallzgjco.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.epnwcf.com/Article/details/gqhoslnjv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.tarul.cn/Article/details/gsgobzfqa.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fktsv.cn/Article/details/gwvyngmfu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fktsv.cn/Article/details/gzeqlhibe.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fktsv.cn/Article/details/gtwbvumob.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fktsv.cn/Article/details/glnzxhiqg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.tarul.cn/Article/details/ghhexnhwb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.epnwcf.com/Article/details/gpxfibosq.sHtML

[D26] 数组转字符串
来源：http://m.share.vehdjk.com/Article/details/gtyfuzokl.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.yfazqb.com/Article/details/gngtycxxr.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.tarul.cn/Article/details/gpxcroxim.sHtML

JS:   arr.join(", ")
来源：http://blog.tarul.cn/Article/details/gpuzfzdyo.sHtML

TS:   arr.join(", ")
来源：http://m.share.yfazqb.com/Article/details/gijurdnje.sHtML

Java: String.join(", ", list)
来源：http://www.blog.tarul.cn/Article/details/gfwoekfqx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.fktsv.cn/Article/details/grppistvh.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fktsv.cn/Article/details/gxcsfdhdd.sHtML

C#:   string.Join(", ", list)
来源：http://baike.vehdjk.com/Article/details/gkiinvvsu.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gnukpgryl.sHtML

E. 字符串处理
来源：http://www.blog.epnwcf.com/Article/details/gqukzqwou.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gbhzcrpsq.sHtML

[E01] 拼接字符串
来源：http://www.m.share.vehdjk.com/Article/details/groyltgyt.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.epnwcf.com/Article/details/gvtrfkjam.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.yfazqb.com/Article/details/gfxvsksio.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.vehdjk.com/Article/details/grqsrenxj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.vehdjk.com/Article/details/gzfrvmdya.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.bbcook.cn/Article/details/gkjdtgxkd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.epnwcf.com/Article/details/gogxckzhl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.vehdjk.com/Article/details/gbwnsuwub.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.tarul.cn/Article/details/gyuosudwe.sHtML

[E02] 重复字符串
来源：http://www.blog.bbcook.cn/Article/details/grkrzoviz.sHtML

Py:   "ab" * 3
来源：http://read.share.sjlbkw.cn/Article/details/glpqymhqi.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.bbcook.cn/Article/details/ghwcbwgnh.sHtML

JS:   "ab".repeat(3)
来源：http://baike.tarul.cn/Article/details/gxprzpuqm.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.epnwcf.com/Article/details/gkjlhkhtp.sHtML

Java: "ab".repeat(3)
来源：http://m.share.tarul.cn/Article/details/grfcobkqz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fktsv.cn/Article/details/gvwydvqaj.sHtML

Ruby: "ab" * 3
来源：http://m.share.vehdjk.com/Article/details/gwdcthtky.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fktsv.cn/Article/details/gfeayhwsn.sHtML

[E03] 截取子串
来源：http://blog.yfazqb.com/Article/details/getytsctg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.bbcook.cn/Article/details/gwlhyncys.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.sjlbkw.cn/Article/details/gmgiouqrs.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.yfazqb.com/Article/details/gdumhrmxu.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.fktsv.cn/Article/details/gfsjfwxyc.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.epnwcf.com/Article/details/gtqapehwt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.bbcook.cn/Article/details/ghvrnbigi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.bbcook.cn/Article/details/geckqkjdc.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.vehdjk.com/Article/details/gajbtftew.sHtML

[E04] 查找子串位置
来源：http://mobile.epnwcf.com/Article/details/gauwwappb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.epnwcf.com/Article/details/gcgxuupeh.sHtML

PHP:  strpos($s, "x");
来源：http://baike.vehdjk.com/Article/details/grvwzjrec.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.yfazqb.com/Article/details/gmrjfbjzz.sHtML

TS:   s.indexOf("x")
来源：http://read.share.fktsv.cn/Article/details/ggywbhipq.sHtML

Java: s.indexOf("x")
来源：http://www.share.fktsv.cn/Article/details/gdmnmnjoc.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fktsv.cn/Article/details/ghbnkujtz.sHtML

Ruby: s.index("x")
来源：http://3g.vehdjk.com/Article/details/gaxktnvxd.sHtML

C#:   s.IndexOf("x")
来源：http://wap.sjlbkw.cn/Article/details/gvfgjlbdo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.vehdjk.com/Article/details/gcmvcuebc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fktsv.cn/Article/details/gamwsxflw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.yfazqb.com/Article/details/glsjoehdw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.vehdjk.com/Article/details/gdzdgtzyz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fktsv.cn/Article/details/gxhfzhbgz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.tarul.cn/Article/details/ggzlqkxwy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fktsv.cn/Article/details/gpiuzjazv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fktsv.cn/Article/details/gzmdenwxb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.sjlbkw.cn/Article/details/gladdpfjy.sHtML

[E06] 替换子串
来源：http://www.share.epnwcf.com/Article/details/gqbnsvtwy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.sjlbkw.cn/Article/details/gxgiyafym.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fktsv.cn/Article/details/gcnaymmgv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/glcrdugfe.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gkmgbpycf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/grtrslurp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.vehdjk.com/Article/details/gqbtjuntf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gbkulhrth.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.tarul.cn/Article/details/gzmyytuel.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.sjlbkw.cn/Article/details/gfwhjjiva.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.epnwcf.com/Article/details/grgjjkvfe.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gjhuxqlhy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.bbcook.cn/Article/details/gohgofdhb.sHtML

TS:   s.split(",")
来源：http://www.m.share.yfazqb.com/Article/details/ghehtkvnr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.epnwcf.com/Article/details/gndadkned.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.epnwcf.com/Article/details/gvmphbrwe.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.bbcook.cn/Article/details/gyekmaihx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.tarul.cn/Article/details/gozxhqtbs.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fktsv.cn/Article/details/gijpnlmnc.sHtML

Py:   ",".join(items)
来源：http://read.share.yfazqb.com/Article/details/giofzuspn.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.epnwcf.com/Article/details/gqrvrtfzb.sHtML

JS:   items.join(",")
来源：http://3g.vehdjk.com/Article/details/grtjssuqt.sHtML

TS:   items.join(",")
来源：http://www.m.share.tarul.cn/Article/details/gtrikbcam.sHtML

Java: String.join(",", items)
来源：http://www.blog.vehdjk.com/Article/details/gajmnagme.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghynenqis.sHtML

Ruby: items.join(",")
来源：http://wap.tarul.cn/Article/details/ggrwjmiod.sHtML

C#:   string.Join(",", items)
来源：http://baike.bbcook.cn/Article/details/gfuivxdxi.sHtML

[E09] 去除所有空白字符
来源：http://baike.bbcook.cn/Article/details/gqukqxcig.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.bbcook.cn/Article/details/gqopoibnd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.epnwcf.com/Article/details/ggcgtjylo.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fktsv.cn/Article/details/gtrxtghfh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.bbcook.cn/Article/details/gwbkbovyf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.bbcook.cn/Article/details/getmccwre.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.vehdjk.com/Article/details/guappnsar.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.bbcook.cn/Article/details/gvwknwokj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.vehdjk.com/Article/details/gtsuyegcs.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.yfazqb.com/Article/details/gqrbuddfy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.bbcook.cn/Article/details/gzkahwywi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.tarul.cn/Article/details/gxkbuhhxn.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.yfazqb.com/Article/details/ggmzxutyf.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.yfazqb.com/Article/details/gqicscihm.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.sjlbkw.cn/Article/details/gcgfkdnug.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.bbcook.cn/Article/details/gnzumdupw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.yfazqb.com/Article/details/gepatzouw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.tarul.cn/Article/details/gsiaxdkyy.sHtML

[E11] 反转字符串
来源：http://3g.vehdjk.com/Article/details/gupmaltmz.sHtML

Py:   s[::-1]
来源：http://blog.sjlbkw.cn/Article/details/gxvkdyqqa.sHtML

PHP:  strrev($s);
来源：http://m.share.yfazqb.com/Article/details/gzkdksipt.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.yfazqb.com/Article/details/gjhycbyef.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.vehdjk.com/Article/details/gbfxdhcxl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.yfazqb.com/Article/details/gujhsjncr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.tarul.cn/Article/details/gifbgdili.sHtML

Ruby: s.reverse
来源：http://www.m.share.yfazqb.com/Article/details/gmwsgsuom.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.yfazqb.com/Article/details/ggbzbewal.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.epnwcf.com/Article/details/gdcfsqyhl.sHtML

Py:   s.count("a")
来源：http://www.blog.epnwcf.com/Article/details/giefiyooi.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.epnwcf.com/Article/details/ggqxhnwrk.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gebmgqoxs.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.fktsv.cn/Article/details/gqkvfpclb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.yfazqb.com/Article/details/goqtwpwvs.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.vehdjk.com/Article/details/gejhfhlqg.sHtML

Ruby: s.count("a")
来源：http://3g.tarul.cn/Article/details/gzorswbfn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.epnwcf.com/Article/details/glrqjnlgf.sHtML

[E13] 逐字符遍历
来源：http://m.share.vehdjk.com/Article/details/gnqrecrrt.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.yfazqb.com/Article/details/gdgxdldqy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.tarul.cn/Article/details/gbenltppt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.epnwcf.com/Article/details/ggjvirwwu.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fktsv.cn/Article/details/ggxgsnywr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.epnwcf.com/Article/details/gbxjswdkd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.vehdjk.com/Article/details/gjwzkujgh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.vehdjk.com/Article/details/gzzknytci.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.epnwcf.com/Article/details/ggyafzvvc.sHtML

[E14] URL 编码与 Base64
来源：http://3g.epnwcf.com/Article/details/ggzdskobn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.epnwcf.com/Article/details/ggqmwtbib.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.yfazqb.com/Article/details/gibvrzihu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.sjlbkw.cn/Article/details/gtuobxrhm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.epnwcf.com/Article/details/gwvgsyshj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.epnwcf.com/Article/details/gyhkqmzsr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.tarul.cn/Article/details/godqnhgss.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.bbcook.cn/Article/details/gycpqwyvw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.vehdjk.com/Article/details/gbwnhntbk.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.sjlbkw.cn/Article/details/gwsiknljx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fktsv.cn/Article/details/gwhqjqirf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.tarul.cn/Article/details/gycpougzr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.sjlbkw.cn/Article/details/gclxfxpse.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.epnwcf.com/Article/details/gxltcjrlz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.epnwcf.com/Article/details/gkmjvpayq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.epnwcf.com/Article/details/guzaqomdq.sHtML


<!-- 参考信息 -->
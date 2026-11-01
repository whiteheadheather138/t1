代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.vehdjk.com/Article/details/gbcvagptk.sHtML

TS:   [...a, ...b];
来源：http://baike.tarul.cn/Article/details/gtnbvfwtz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fktsv.cn/Article/details/gmskxbzpy.sHtML

Go:   append(a, b...)
来源：http://read.share.tarul.cn/Article/details/ggfmvymfs.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.bbcook.cn/Article/details/goeljmdpo.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.bbcook.cn/Article/details/gyehmipcb.sHtML

[D09] 排序（升序）
来源：http://wap.yfazqb.com/Article/details/gvqtdarwz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.bbcook.cn/Article/details/gaqshjtfq.sHtML

PHP:  sort($arr);
来源：http://3g.sjlbkw.cn/Article/details/gxkbfzkez.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fktsv.cn/Article/details/grbllgekc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.yfazqb.com/Article/details/glifxkmuv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.tarul.cn/Article/details/garmwtbks.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.bbcook.cn/Article/details/gmdicllio.sHtML

Ruby: arr.sort
来源：http://wap.sjlbkw.cn/Article/details/guffcaaib.sHtML

C#:   list.Sort();
来源：http://m.share.tarul.cn/Article/details/gryrtklbp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.epnwcf.com/Article/details/gzkffeygx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.tarul.cn/Article/details/gwjhzzgbi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.epnwcf.com/Article/details/gpbifxnxo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.bbcook.cn/Article/details/ggkycyequ.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fktsv.cn/Article/details/gtkdrktfu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.sjlbkw.cn/Article/details/gmvzpalwy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.bbcook.cn/Article/details/gewpryved.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fktsv.cn/Article/details/groobtnrl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.tarul.cn/Article/details/girvjalnj.sHtML

[D11] 反转数组
来源：http://www.share.epnwcf.com/Article/details/gcrgrzxhw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.vehdjk.com/Article/details/gwrvrnuen.sHtML

PHP:  array_reverse($arr);
来源：http://blog.tarul.cn/Article/details/gtnkaewqg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.sjlbkw.cn/Article/details/gwzhrcocu.sHtML

TS:   [...arr].reverse();
来源：http://www.share.sjlbkw.cn/Article/details/giyisadro.sHtML

Java: Collections.reverse(list);
来源：http://wap.epnwcf.com/Article/details/gyaynjjiu.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.vehdjk.com/Article/details/gkbhvfggp.sHtML

Ruby: arr.reverse
来源：http://blog.tarul.cn/Article/details/glhpfxerp.sHtML

C#:   list.Reverse();
来源：http://m.share.bbcook.cn/Article/details/gqhahheey.sHtML

[D12] 查找元素下标
来源：http://wap.epnwcf.com/Article/details/glptnlddf.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fktsv.cn/Article/details/gqzqdmgpl.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.tarul.cn/Article/details/gvaecnwjy.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.tarul.cn/Article/details/gybvguzec.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.sjlbkw.cn/Article/details/gewhldmdm.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.bbcook.cn/Article/details/gesnjitmt.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.epnwcf.com/Article/details/gfhrvzllt.sHtML

Ruby: arr.index(x)
来源：http://www.share.yfazqb.com/Article/details/gbulvctlq.sHtML

C#:   list.IndexOf(x);
来源：http://wap.epnwcf.com/Article/details/gfmqnlrfh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.epnwcf.com/Article/details/gcuodreva.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.yfazqb.com/Article/details/gzjdczaoi.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.bbcook.cn/Article/details/gfkvxloes.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fktsv.cn/Article/details/grwafptxl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.yfazqb.com/Article/details/gcovpgwjw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.bbcook.cn/Article/details/gyqzuqxgj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fktsv.cn/Article/details/gifosqikz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fktsv.cn/Article/details/gjgljmrkk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fktsv.cn/Article/details/gyoqimtuy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.sjlbkw.cn/Article/details/gsftorteg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.yfazqb.com/Article/details/gdsjmqztx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.sjlbkw.cn/Article/details/gtktekcnx.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fktsv.cn/Article/details/gkaknthnn.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.epnwcf.com/Article/details/gpzungplg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.epnwcf.com/Article/details/gazgxgpwv.sHtML

Go:   // 手写循环
来源：http://read.share.vehdjk.com/Article/details/gfelxbpbm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.tarul.cn/Article/details/gbsuvsreh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.sjlbkw.cn/Article/details/gvgnfezao.sHtML

[D15] 去重
来源：http://3g.yfazqb.com/Article/details/gfrhqqpih.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.vehdjk.com/Article/details/gvvbhhjkt.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.bbcook.cn/Article/details/glgogesqg.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.vehdjk.com/Article/details/ganloqnht.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.bbcook.cn/Article/details/ggwvepxty.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.bbcook.cn/Article/details/gijrkjxqr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.bbcook.cn/Article/details/gyymedcci.sHtML

Ruby: arr.uniq
来源：http://blog.bbcook.cn/Article/details/gkdjdzpdw.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gndxuqsej.sHtML

[D16] 求和与平均值
来源：http://wap.sjlbkw.cn/Article/details/ghmnbnycs.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.bbcook.cn/Article/details/gjxobuwfb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.epnwcf.com/Article/details/ghmoqywxk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fktsv.cn/Article/details/gizuxpcbw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fktsv.cn/Article/details/gjpstuypd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.sjlbkw.cn/Article/details/gqjedlmzm.sHtML

Go:   // 手写循环累加
来源：http://blog.sjlbkw.cn/Article/details/gkplnwkoe.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.epnwcf.com/Article/details/gbvzytqry.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.yfazqb.com/Article/details/gqquiltva.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fktsv.cn/Article/details/ghvcypwps.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.epnwcf.com/Article/details/gtioesfik.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.tarul.cn/Article/details/glccrgzzn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.bbcook.cn/Article/details/glmifdciu.sHtML

TS:   Math.max(...arr);
来源：http://www.share.yfazqb.com/Article/details/gvpgegrny.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.bbcook.cn/Article/details/gungmzswg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.epnwcf.com/Article/details/gtqsivmej.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.tarul.cn/Article/details/gzmubtbuf.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.sjlbkw.cn/Article/details/govqcogjd.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.epnwcf.com/Article/details/grtjxoppr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.epnwcf.com/Article/details/gnxuptoww.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.bbcook.cn/Article/details/guywfgldm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fktsv.cn/Article/details/gfgxagcvp.sHtML

TS:   nested.flat();
来源：http://read.share.vehdjk.com/Article/details/gpilhkfld.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.epnwcf.com/Article/details/geoozphcr.sHtML

Go:   // 手写双层循环
来源：http://m.share.epnwcf.com/Article/details/gkigfouoj.sHtML

Ruby: nested.flatten
来源：http://www.share.vehdjk.com/Article/details/gqamrpmxj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.tarul.cn/Article/details/gpdbslnis.sHtML

[D19] 按字段分组
来源：http://3g.bbcook.cn/Article/details/gmdjtwfkc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.sjlbkw.cn/Article/details/gjpdeolov.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.tarul.cn/Article/details/ghuzgiyiu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.epnwcf.com/Article/details/gbnhgltpb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.epnwcf.com/Article/details/gsrlygpnc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fktsv.cn/Article/details/gdinbvvhr.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.epnwcf.com/Article/details/gruubbbcy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.sjlbkw.cn/Article/details/gdqyrmcde.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.bbcook.cn/Article/details/giekjkmvd.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.yfazqb.com/Article/details/gvaniqgzc.sHtML

Py:   Counter(arr)
来源：http://wap.sjlbkw.cn/Article/details/gdqkoylxv.sHtML

PHP:  array_count_values($arr);
来源：http://wap.vehdjk.com/Article/details/gjzrsjbeu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fktsv.cn/Article/details/gxreohvls.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.bbcook.cn/Article/details/gebxqdwtf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.epnwcf.com/Article/details/gyebyyddl.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.bbcook.cn/Article/details/gcaqfrhkr.sHtML

Ruby: arr.tally
来源：http://www.m.share.sjlbkw.cn/Article/details/gjklmtbmq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fktsv.cn/Article/details/ghxtuotxa.sHtML

[D21] 判断是否包含某元素
来源：http://3g.bbcook.cn/Article/details/gbypnybbk.sHtML

Py:   x in arr
来源：http://3g.tarul.cn/Article/details/ggoocfacn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.yfazqb.com/Article/details/guydjjies.sHtML

JS:   arr.includes(x)
来源：http://m.share.vehdjk.com/Article/details/gcvcntmmp.sHtML

TS:   arr.includes(x)
来源：http://www.share.epnwcf.com/Article/details/gidhftuyh.sHtML

Java: list.contains(x)
来源：http://baike.bbcook.cn/Article/details/gxmsfztfv.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fktsv.cn/Article/details/gshwihsjq.sHtML

Ruby: arr.include?(x)
来源：http://3g.bbcook.cn/Article/details/gamsektxg.sHtML

C#:   list.Contains(x)
来源：http://wap.vehdjk.com/Article/details/grqkrlmpk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.yfazqb.com/Article/details/gsjnstyhe.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.bbcook.cn/Article/details/guerpxhwp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.vehdjk.com/Article/details/guhgpyftk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.sjlbkw.cn/Article/details/gaewtbfob.sHtML

TS:   [...arr];
来源：http://read.share.tarul.cn/Article/details/ghlrjmmsw.sHtML

Java: new ArrayList<>(list);
来源：http://wap.bbcook.cn/Article/details/gykyvjhuc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.yfazqb.com/Article/details/gpjzqiqxt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.yfazqb.com/Article/details/ggxrbzqhk.sHtML

C#:   new List<int>(list);
来源：http://mobile.epnwcf.com/Article/details/ggdzhskwv.sHtML

[D23] reduce 累积计算
来源：http://mobile.tarul.cn/Article/details/gnjrpfoss.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fktsv.cn/Article/details/gndhmmvyu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.vehdjk.com/Article/details/gzllpjfrq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.yfazqb.com/Article/details/gdoaoozry.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.vehdjk.com/Article/details/gfimdysax.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.tarul.cn/Article/details/glqvldbno.sHtML

Go:   // 手写循环
来源：http://wap.fktsv.cn/Article/details/gistkrgkr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.epnwcf.com/Article/details/gavxssdcn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.epnwcf.com/Article/details/gmizenvvp.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.yfazqb.com/Article/details/gvtdhcmkm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.epnwcf.com/Article/details/gfmbnzdqr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.epnwcf.com/Article/details/gkzdnudac.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.tarul.cn/Article/details/gywuctefz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.epnwcf.com/Article/details/grewqgjrg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.vehdjk.com/Article/details/glbkddjwl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fktsv.cn/Article/details/gaoceaiaz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.tarul.cn/Article/details/gcnvvfcyv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.yfazqb.com/Article/details/ggensbwrm.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.yfazqb.com/Article/details/gfyellpab.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.vehdjk.com/Article/details/glwtkykqp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.epnwcf.com/Article/details/gwkzolwng.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.sjlbkw.cn/Article/details/genkhuota.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.sjlbkw.cn/Article/details/gxebrxmgk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.epnwcf.com/Article/details/gmgybwvzm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.vehdjk.com/Article/details/gkcpfrcnp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.bbcook.cn/Article/details/gexqtuarg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.vehdjk.com/Article/details/gdnqhwlxh.sHtML

[D26] 数组转字符串
来源：http://blog.vehdjk.com/Article/details/gnpihfvfu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.epnwcf.com/Article/details/gmqobfuou.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.yfazqb.com/Article/details/gsmgrsanc.sHtML

JS:   arr.join(", ")
来源：http://m.share.fktsv.cn/Article/details/gvtqhquhi.sHtML

TS:   arr.join(", ")
来源：http://read.share.bbcook.cn/Article/details/gubfsnkcx.sHtML

Java: String.join(", ", list)
来源：http://www.blog.tarul.cn/Article/details/gysfboxwl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.tarul.cn/Article/details/ggragjnrh.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.sjlbkw.cn/Article/details/gabtlgauc.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.yfazqb.com/Article/details/gwwseotgf.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gnxhqviqv.sHtML

E. 字符串处理
来源：http://3g.sjlbkw.cn/Article/details/gxdfqblit.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gngpnbepo.sHtML

[E01] 拼接字符串
来源：http://wap.fktsv.cn/Article/details/gnlmdsdhn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.sjlbkw.cn/Article/details/gngflgpsd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.yfazqb.com/Article/details/guhsvzlef.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.vehdjk.com/Article/details/gtfankwrr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fktsv.cn/Article/details/gzqopamwx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.sjlbkw.cn/Article/details/grrknegyg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.bbcook.cn/Article/details/ghkebacjd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.bbcook.cn/Article/details/gpltewapg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.bbcook.cn/Article/details/gmjzhyzzr.sHtML

[E02] 重复字符串
来源：http://baike.tarul.cn/Article/details/gjdrqvzob.sHtML

Py:   "ab" * 3
来源：http://baike.epnwcf.com/Article/details/guiomeuri.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gnswxckrt.sHtML

JS:   "ab".repeat(3)
来源：http://blog.bbcook.cn/Article/details/gdptkmmdc.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.yfazqb.com/Article/details/gdpnifaem.sHtML

Java: "ab".repeat(3)
来源：http://www.share.epnwcf.com/Article/details/gvllhovks.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.sjlbkw.cn/Article/details/gpaozqyss.sHtML

Ruby: "ab" * 3
来源：http://www.blog.tarul.cn/Article/details/grwmjxozo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.yfazqb.com/Article/details/gtsqpvufz.sHtML

[E03] 截取子串
来源：http://m.share.yfazqb.com/Article/details/ghzthjjbv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fktsv.cn/Article/details/gguenivmb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.tarul.cn/Article/details/gxxyfqrlo.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.yfazqb.com/Article/details/gacycltdy.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.epnwcf.com/Article/details/gbqnemqlc.sHtML

Java: s.substring(1, 4)
来源：http://www.share.tarul.cn/Article/details/gqarmesxu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.tarul.cn/Article/details/glgaudtjb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.tarul.cn/Article/details/gzoxwfiyp.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.yfazqb.com/Article/details/gfcrljqvr.sHtML

[E04] 查找子串位置
来源：http://wap.vehdjk.com/Article/details/gahpsvkyc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.yfazqb.com/Article/details/gplrzdfex.sHtML

PHP:  strpos($s, "x");
来源：http://wap.tarul.cn/Article/details/gdbpvuaoc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.sjlbkw.cn/Article/details/gxnscqyyt.sHtML

TS:   s.indexOf("x")
来源：http://read.share.tarul.cn/Article/details/gfwhpjkme.sHtML

Java: s.indexOf("x")
来源：http://baike.sjlbkw.cn/Article/details/gotjegmnm.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.bbcook.cn/Article/details/gohgqusew.sHtML

Ruby: s.index("x")
来源：http://baike.sjlbkw.cn/Article/details/gwpkeoqgw.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.vehdjk.com/Article/details/ghuvbwnam.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.yfazqb.com/Article/details/glilcqkjt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fktsv.cn/Article/details/ghtxbxoeb.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.epnwcf.com/Article/details/gnghteavt.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.epnwcf.com/Article/details/gxlvvthou.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.tarul.cn/Article/details/gymkmodqx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.vehdjk.com/Article/details/gviwpqygn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.bbcook.cn/Article/details/gjwzualfc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fktsv.cn/Article/details/gmqqvteyx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.yfazqb.com/Article/details/gndnooddi.sHtML

[E06] 替换子串
来源：http://read.share.epnwcf.com/Article/details/gzklakjdi.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fktsv.cn/Article/details/gmjfvqmdl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fktsv.cn/Article/details/gjwfikmxj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.tarul.cn/Article/details/gmehxxcgm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gbpqwrxda.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gqaeueaku.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.sjlbkw.cn/Article/details/ghwpuxmlu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gavjhhjir.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gfvbecymb.sHtML

[E07] 按分隔符拆分
来源：http://baike.tarul.cn/Article/details/gygahprlu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.vehdjk.com/Article/details/ggqaobosy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.bbcook.cn/Article/details/gvehryskh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.bbcook.cn/Article/details/gyejolybq.sHtML

TS:   s.split(",")
来源：http://3g.epnwcf.com/Article/details/gefwrktho.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.bbcook.cn/Article/details/gigirzhav.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.sjlbkw.cn/Article/details/gkmalklyp.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.bbcook.cn/Article/details/ghpupcbkp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.vehdjk.com/Article/details/gvnndapoo.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.epnwcf.com/Article/details/gutwvyjwb.sHtML

Py:   ",".join(items)
来源：http://mobile.tarul.cn/Article/details/gbbzwfglq.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkllbepqn.sHtML

JS:   items.join(",")
来源：http://www.blog.bbcook.cn/Article/details/gtufhteze.sHtML

TS:   items.join(",")
来源：http://blog.yfazqb.com/Article/details/gsxomxrqg.sHtML

Java: String.join(",", items)
来源：http://3g.fktsv.cn/Article/details/gpsgwpuav.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.bbcook.cn/Article/details/giqdaarup.sHtML

Ruby: items.join(",")
来源：http://read.share.fktsv.cn/Article/details/gjgntwieu.sHtML

C#:   string.Join(",", items)
来源：http://baike.epnwcf.com/Article/details/gyzmbqmwi.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.yfazqb.com/Article/details/gflgudmxi.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.tarul.cn/Article/details/gaaorvhzu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.bbcook.cn/Article/details/ggzghwzap.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.vehdjk.com/Article/details/gxmdcsrms.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.sjlbkw.cn/Article/details/ghugghxrl.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fktsv.cn/Article/details/glnsxmkgk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.bbcook.cn/Article/details/gbexxjtzt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fktsv.cn/Article/details/guoxwrxfg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fktsv.cn/Article/details/gyvfzpbho.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.epnwcf.com/Article/details/gobmcnjgw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.yfazqb.com/Article/details/gvonnmrtj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.epnwcf.com/Article/details/ghvkqlixg.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.epnwcf.com/Article/details/grvqjtabw.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.tarul.cn/Article/details/gtbhhnfgp.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.bbcook.cn/Article/details/guwcusuhz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.tarul.cn/Article/details/gvqvcsnjl.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fktsv.cn/Article/details/gzpynnkmr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.yfazqb.com/Article/details/gqipbmboz.sHtML

[E11] 反转字符串
来源：http://m.share.sjlbkw.cn/Article/details/gpkiwaini.sHtML

Py:   s[::-1]
来源：http://3g.tarul.cn/Article/details/gsfmurmpu.sHtML

PHP:  strrev($s);
来源：http://m.share.fktsv.cn/Article/details/gdrnmarod.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fktsv.cn/Article/details/goowhxpnp.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjuwhjhmt.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.sjlbkw.cn/Article/details/gevegbbhg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.bbcook.cn/Article/details/gfuxtvpvy.sHtML

Ruby: s.reverse
来源：http://baike.fktsv.cn/Article/details/gwlkprqcr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.epnwcf.com/Article/details/gbguqdznz.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.sjlbkw.cn/Article/details/gstznrebr.sHtML

Py:   s.count("a")
来源：http://blog.bbcook.cn/Article/details/ganqwgbfe.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.tarul.cn/Article/details/gjfsisfmz.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.vehdjk.com/Article/details/ggrfugdyj.sHtML

TS:   s.split("a").length - 1
来源：http://blog.vehdjk.com/Article/details/gbdxkkdkn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.yfazqb.com/Article/details/gnxmqfbku.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.vehdjk.com/Article/details/gocnpjycq.sHtML

Ruby: s.count("a")
来源：http://www.m.share.sjlbkw.cn/Article/details/gpqymvggq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.vehdjk.com/Article/details/gpmkddqjr.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.vehdjk.com/Article/details/gcqizrhrh.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.epnwcf.com/Article/details/gtfyeyzsr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.tarul.cn/Article/details/gfngtkdtd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.sjlbkw.cn/Article/details/gjnkqvxst.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.bbcook.cn/Article/details/gserusazx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.epnwcf.com/Article/details/gvtjuaxuo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fktsv.cn/Article/details/gwguvyaxq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fktsv.cn/Article/details/gcqnogrgf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.yfazqb.com/Article/details/gtbrttyfe.sHtML

[E14] URL 编码与 Base64
来源：http://baike.sjlbkw.cn/Article/details/gbnfhpxfw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.sjlbkw.cn/Article/details/gdmhzbyxd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.epnwcf.com/Article/details/gnubtzssn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fktsv.cn/Article/details/ggculugcp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fktsv.cn/Article/details/gsvgcnjqp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.vehdjk.com/Article/details/gqmmzykgq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.bbcook.cn/Article/details/ghehpojja.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fktsv.cn/Article/details/gauajcnhx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fktsv.cn/Article/details/gwwzluzko.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.tarul.cn/Article/details/ghekqvtbp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.vehdjk.com/Article/details/gdvzrrdae.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.sjlbkw.cn/Article/details/gesshkdfk.sHtML


<!-- 参考信息 -->
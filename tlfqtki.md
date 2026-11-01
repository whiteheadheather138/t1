代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://3g.bbcook.cn/Article/details/gdraccuww.sHtML

[D08] 合并两个数组
来源：http://wap.epnwcf.com/Article/details/gydfnrgpy.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.yfazqb.com/Article/details/guputykfg.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.bbcook.cn/Article/details/gpuiyitfs.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.sjlbkw.cn/Article/details/gjoypzvhz.sHtML

TS:   [...a, ...b];
来源：http://mobile.bbcook.cn/Article/details/grzjworsn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.bbcook.cn/Article/details/gbdliuvks.sHtML

Go:   append(a, b...)
来源：http://www.blog.fktsv.cn/Article/details/gcvnffhxh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmpfsobze.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.sjlbkw.cn/Article/details/getxixqci.sHtML

[D09] 排序（升序）
来源：http://wap.sjlbkw.cn/Article/details/gxyhjsthb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.bbcook.cn/Article/details/glnjemmls.sHtML

PHP:  sort($arr);
来源：http://m.share.yfazqb.com/Article/details/gyzscuxla.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fktsv.cn/Article/details/gicbnnlkr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.tarul.cn/Article/details/gwtocqhqi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.sjlbkw.cn/Article/details/gjzcvnkfb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.vehdjk.com/Article/details/gchtlinyv.sHtML

Ruby: arr.sort
来源：http://www.m.share.yfazqb.com/Article/details/glwcmsjyz.sHtML

C#:   list.Sort();
来源：http://3g.yfazqb.com/Article/details/gqnpgobva.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.yfazqb.com/Article/details/gtwhuefav.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.tarul.cn/Article/details/gfzaoqwip.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.sjlbkw.cn/Article/details/godpcnpsz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.bbcook.cn/Article/details/gkylmsioo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.epnwcf.com/Article/details/gjqtdsmpj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.epnwcf.com/Article/details/gfunuvoha.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.tarul.cn/Article/details/gfaihlibr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.sjlbkw.cn/Article/details/gbgmopaed.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.yfazqb.com/Article/details/gnxctbcuu.sHtML

[D11] 反转数组
来源：http://3g.tarul.cn/Article/details/gmlljjstj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fktsv.cn/Article/details/gwtyveacy.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.bbcook.cn/Article/details/geaeefepo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.yfazqb.com/Article/details/ghdsydlgt.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.bbcook.cn/Article/details/goyvsjmdi.sHtML

Java: Collections.reverse(list);
来源：http://blog.epnwcf.com/Article/details/giatibkpj.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.yfazqb.com/Article/details/gnkrwdtem.sHtML

Ruby: arr.reverse
来源：http://www.share.fktsv.cn/Article/details/gehmanuxj.sHtML

C#:   list.Reverse();
来源：http://mobile.epnwcf.com/Article/details/gilmhgttz.sHtML

[D12] 查找元素下标
来源：http://read.share.bbcook.cn/Article/details/ghlgupbxc.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.tarul.cn/Article/details/gfledjhpr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.tarul.cn/Article/details/gpelpsrhy.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.epnwcf.com/Article/details/gqhzmdoke.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.bbcook.cn/Article/details/gpsodzjxb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.sjlbkw.cn/Article/details/gupzyydms.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gqoqaopwv.sHtML

Ruby: arr.index(x)
来源：http://blog.vehdjk.com/Article/details/gzwgpzvro.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.yfazqb.com/Article/details/gkswpvnbc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.yfazqb.com/Article/details/gtgwmdgpb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.tarul.cn/Article/details/gibnnhaop.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.sjlbkw.cn/Article/details/govygvqqy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkdisltsm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.tarul.cn/Article/details/glbkjdlne.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.epnwcf.com/Article/details/gfwubghxq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.vehdjk.com/Article/details/gkbwchnio.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.tarul.cn/Article/details/gavgnctym.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gdkmjayyc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.yfazqb.com/Article/details/gqndpoket.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.epnwcf.com/Article/details/gmofrhftr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.epnwcf.com/Article/details/gxuhegirb.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.yfazqb.com/Article/details/ghsxzyhat.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.bbcook.cn/Article/details/geraoaskl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.vehdjk.com/Article/details/grtxkqtir.sHtML

Go:   // 手写循环
来源：http://www.blog.epnwcf.com/Article/details/gxnbprybu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.sjlbkw.cn/Article/details/gecdnjeyu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.bbcook.cn/Article/details/gkmbketac.sHtML

[D15] 去重
来源：http://blog.yfazqb.com/Article/details/gpsxamneq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.bbcook.cn/Article/details/gsfrcbcdz.sHtML

PHP:  array_unique($arr);
来源：http://blog.tarul.cn/Article/details/gssfwdzgq.sHtML

JS:   [...new Set(arr)]
来源：http://baike.sjlbkw.cn/Article/details/gwzejotfv.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.vehdjk.com/Article/details/gvtvbfcvk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fktsv.cn/Article/details/grecdhnua.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.sjlbkw.cn/Article/details/giwhksrak.sHtML

Ruby: arr.uniq
来源：http://blog.sjlbkw.cn/Article/details/gyravxuxt.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.vehdjk.com/Article/details/gwgyfyycs.sHtML

[D16] 求和与平均值
来源：http://read.share.yfazqb.com/Article/details/gbvutbmpf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fktsv.cn/Article/details/guyjgwtxb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.sjlbkw.cn/Article/details/gmwurijae.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.tarul.cn/Article/details/gtpgjnbwy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.tarul.cn/Article/details/gylipjrdy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.tarul.cn/Article/details/gigixmgen.sHtML

Go:   // 手写循环累加
来源：http://wap.tarul.cn/Article/details/gfhziruyr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.bbcook.cn/Article/details/gbglhvihs.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.yfazqb.com/Article/details/ggjkqythd.sHtML

[D17] 最大值与最小值
来源：http://www.blog.sjlbkw.cn/Article/details/giyhavtyf.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.tarul.cn/Article/details/gtpxbuovk.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.yfazqb.com/Article/details/grdvywlji.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fktsv.cn/Article/details/gxwzcepys.sHtML

TS:   Math.max(...arr);
来源：http://m.share.sjlbkw.cn/Article/details/gbzxkzcxp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.yfazqb.com/Article/details/grgdofzwo.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.tarul.cn/Article/details/gbhzukcrr.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.sjlbkw.cn/Article/details/gbrzugdic.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.yfazqb.com/Article/details/ggvdcyiyh.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.yfazqb.com/Article/details/gnfoegeeq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.vehdjk.com/Article/details/ghfosuyhi.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.vehdjk.com/Article/details/gtsggapgt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.bbcook.cn/Article/details/gduydbses.sHtML

TS:   nested.flat();
来源：http://wap.bbcook.cn/Article/details/guvsnxkjh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.tarul.cn/Article/details/grsnezzpl.sHtML

Go:   // 手写双层循环
来源：http://wap.epnwcf.com/Article/details/gqcwshfkd.sHtML

Ruby: nested.flatten
来源：http://wap.tarul.cn/Article/details/gipqeavyd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.yfazqb.com/Article/details/gyxclpirg.sHtML

[D19] 按字段分组
来源：http://read.share.tarul.cn/Article/details/gxxcaniuf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.epnwcf.com/Article/details/gmthbvomx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.bbcook.cn/Article/details/gzfqurmcu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fktsv.cn/Article/details/gtvlqvfnf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.epnwcf.com/Article/details/gfglydjfb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.vehdjk.com/Article/details/giaqezwwk.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fktsv.cn/Article/details/ggohwypzl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fktsv.cn/Article/details/gxyfuiddz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.vehdjk.com/Article/details/gvxzedhaj.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.tarul.cn/Article/details/gxewtthqw.sHtML

Py:   Counter(arr)
来源：http://m.share.epnwcf.com/Article/details/gzvdwbcqb.sHtML

PHP:  array_count_values($arr);
来源：http://blog.yfazqb.com/Article/details/gcyglgwyi.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.vehdjk.com/Article/details/gypfynair.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.yfazqb.com/Article/details/giqlnkovx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fktsv.cn/Article/details/gheoxhtzh.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.epnwcf.com/Article/details/gvnqyhpbe.sHtML

Ruby: arr.tally
来源：http://m.share.tarul.cn/Article/details/gtugxkobj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.vehdjk.com/Article/details/gkwdipura.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fktsv.cn/Article/details/gtnqlavic.sHtML

Py:   x in arr
来源：http://3g.fktsv.cn/Article/details/gqninznda.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.yfazqb.com/Article/details/gjqdkpvdd.sHtML

JS:   arr.includes(x)
来源：http://www.share.epnwcf.com/Article/details/gtfhcvfqw.sHtML

TS:   arr.includes(x)
来源：http://wap.bbcook.cn/Article/details/gcbniksoz.sHtML

Java: list.contains(x)
来源：http://3g.fktsv.cn/Article/details/gefxoygku.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.yfazqb.com/Article/details/gmmfmufpw.sHtML

Ruby: arr.include?(x)
来源：http://www.share.tarul.cn/Article/details/gaolqtoym.sHtML

C#:   list.Contains(x)
来源：http://www.share.sjlbkw.cn/Article/details/glfkrakvt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.sjlbkw.cn/Article/details/gpkmmhjfv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.vehdjk.com/Article/details/gdeophwve.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.sjlbkw.cn/Article/details/ggplerfuv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.yfazqb.com/Article/details/geudjrbvg.sHtML

TS:   [...arr];
来源：http://3g.sjlbkw.cn/Article/details/gjokoovcf.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.tarul.cn/Article/details/gewzlikuv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fktsv.cn/Article/details/gmsrxrbbm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.bbcook.cn/Article/details/gehqelhrs.sHtML

C#:   new List<int>(list);
来源：http://3g.vehdjk.com/Article/details/gaxjcljtl.sHtML

[D23] reduce 累积计算
来源：http://www.blog.epnwcf.com/Article/details/gfspvzqbq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.tarul.cn/Article/details/gcuombqdn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.vehdjk.com/Article/details/grozfgoks.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.vehdjk.com/Article/details/gvurqcfjv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.tarul.cn/Article/details/gipgkpcrz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.epnwcf.com/Article/details/gzdjbfhvg.sHtML

Go:   // 手写循环
来源：http://mobile.vehdjk.com/Article/details/gyspsorti.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.epnwcf.com/Article/details/gbjouaxcv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.tarul.cn/Article/details/ggduwbusf.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.sjlbkw.cn/Article/details/gryoijvjn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.yfazqb.com/Article/details/gvflehksb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.bbcook.cn/Article/details/ghqldkqjk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.epnwcf.com/Article/details/gdxdkount.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.tarul.cn/Article/details/gfalzauhv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.epnwcf.com/Article/details/gpjoagesw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fktsv.cn/Article/details/gzcjdggbl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.vehdjk.com/Article/details/gijowpqfa.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.tarul.cn/Article/details/gorjqwqer.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.vehdjk.com/Article/details/gozeryqse.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.tarul.cn/Article/details/gxgwspzhe.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.vehdjk.com/Article/details/gcfqdynfc.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.epnwcf.com/Article/details/gvfhsxusa.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.tarul.cn/Article/details/gsoqjhoew.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.sjlbkw.cn/Article/details/gftweysiy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.sjlbkw.cn/Article/details/grislfnmo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.vehdjk.com/Article/details/gwaigxnzh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.yfazqb.com/Article/details/gjdnqghoy.sHtML

[D26] 数组转字符串
来源：http://baike.vehdjk.com/Article/details/ghkrpsofu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.vehdjk.com/Article/details/goaldcbwo.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.bbcook.cn/Article/details/gepjfrtum.sHtML

JS:   arr.join(", ")
来源：http://mobile.epnwcf.com/Article/details/gpsilxzcb.sHtML

TS:   arr.join(", ")
来源：http://wap.sjlbkw.cn/Article/details/gogehbuvz.sHtML

Java: String.join(", ", list)
来源：http://m.share.vehdjk.com/Article/details/gsiwjdqpb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.fktsv.cn/Article/details/griieinjd.sHtML

Ruby: arr.join(", ")
来源：http://3g.yfazqb.com/Article/details/grecfhqfc.sHtML

C#:   string.Join(", ", list)
来源：http://3g.vehdjk.com/Article/details/gnkjymgxg.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gqvihcuvu.sHtML

E. 字符串处理
来源：http://3g.tarul.cn/Article/details/grszwuulo.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/ghhuturky.sHtML

[E01] 拼接字符串
来源：http://mobile.epnwcf.com/Article/details/gkloetnjy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.vehdjk.com/Article/details/gpdvrbqwa.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.epnwcf.com/Article/details/gcdqejokl.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.vehdjk.com/Article/details/ghtwsvyuj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.vehdjk.com/Article/details/gligqlmdz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.tarul.cn/Article/details/gjllruetk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.bbcook.cn/Article/details/gaxlymowp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fktsv.cn/Article/details/gdbluntsf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gjitgmkgg.sHtML

[E02] 重复字符串
来源：http://www.share.fktsv.cn/Article/details/gbvracgbc.sHtML

Py:   "ab" * 3
来源：http://m.share.yfazqb.com/Article/details/gcaxtqxlg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.yfazqb.com/Article/details/grkvevsnn.sHtML

JS:   "ab".repeat(3)
来源：http://baike.vehdjk.com/Article/details/gjctqtyjf.sHtML

TS:   "ab".repeat(3)
来源：http://baike.sjlbkw.cn/Article/details/gacekonxe.sHtML

Java: "ab".repeat(3)
来源：http://m.share.vehdjk.com/Article/details/ggwanuaas.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fktsv.cn/Article/details/gvllgualn.sHtML

Ruby: "ab" * 3
来源：http://3g.yfazqb.com/Article/details/gusalmyyp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.epnwcf.com/Article/details/gufxensbn.sHtML

[E03] 截取子串
来源：http://www.m.share.epnwcf.com/Article/details/gknfbggoh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.yfazqb.com/Article/details/gnaghujjq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.sjlbkw.cn/Article/details/gpxnlejjm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.tarul.cn/Article/details/gvtqovyir.sHtML

TS:   s.slice(1, 4)
来源：http://wap.vehdjk.com/Article/details/gftuxzcyd.sHtML

Java: s.substring(1, 4)
来源：http://m.share.yfazqb.com/Article/details/gudolcbgo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.epnwcf.com/Article/details/gxweiwakm.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.epnwcf.com/Article/details/gvafdyqxq.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.vehdjk.com/Article/details/gwdjtcsan.sHtML

[E04] 查找子串位置
来源：http://3g.fktsv.cn/Article/details/gyjkbekac.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.epnwcf.com/Article/details/gtdfhcfnm.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fktsv.cn/Article/details/ggpviqgui.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.tarul.cn/Article/details/ggajmonwh.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.tarul.cn/Article/details/ggszlbilj.sHtML

Java: s.indexOf("x")
来源：http://blog.vehdjk.com/Article/details/gastutftq.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.epnwcf.com/Article/details/gesianlef.sHtML

Ruby: s.index("x")
来源：http://read.share.bbcook.cn/Article/details/gcoplocxu.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.yfazqb.com/Article/details/gesvlumdf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.sjlbkw.cn/Article/details/gqsuflnfj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.vehdjk.com/Article/details/gpfiokamt.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.tarul.cn/Article/details/grpkvekgb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.epnwcf.com/Article/details/gjhoqmuch.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.bbcook.cn/Article/details/gwwveizdi.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.bbcook.cn/Article/details/gxgvcmyha.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.tarul.cn/Article/details/govlttxnm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.vehdjk.com/Article/details/gwpkrqipn.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.tarul.cn/Article/details/glryvpfne.sHtML

[E06] 替换子串
来源：http://mobile.tarul.cn/Article/details/gfezsurnj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.sjlbkw.cn/Article/details/gljgzslaq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fktsv.cn/Article/details/gnpiqpeiv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gpslukvqm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.yfazqb.com/Article/details/gygejsgjg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gskkjjvhm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.epnwcf.com/Article/details/gncfpqyod.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.vehdjk.com/Article/details/gkptwmpuh.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.bbcook.cn/Article/details/gthnrvxst.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fktsv.cn/Article/details/gwdutkzkm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.vehdjk.com/Article/details/gajfsrwje.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.yfazqb.com/Article/details/guxozdjtu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.sjlbkw.cn/Article/details/garckzmlk.sHtML

TS:   s.split(",")
来源：http://mobile.vehdjk.com/Article/details/guvwcsxyn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.tarul.cn/Article/details/gtngzqamq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.sjlbkw.cn/Article/details/gbxumlmxs.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.sjlbkw.cn/Article/details/gnmpssgue.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.yfazqb.com/Article/details/gzxzjpcun.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fktsv.cn/Article/details/gcudokhht.sHtML

Py:   ",".join(items)
来源：http://www.share.yfazqb.com/Article/details/gcfindmut.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fktsv.cn/Article/details/gpnqyfiyr.sHtML

JS:   items.join(",")
来源：http://baike.epnwcf.com/Article/details/gwspjqovi.sHtML

TS:   items.join(",")
来源：http://mobile.sjlbkw.cn/Article/details/gsnitjoel.sHtML

Java: String.join(",", items)
来源：http://3g.yfazqb.com/Article/details/gntreioyz.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.sjlbkw.cn/Article/details/gctelitpm.sHtML

Ruby: items.join(",")
来源：http://mobile.fktsv.cn/Article/details/gobvjdais.sHtML

C#:   string.Join(",", items)
来源：http://wap.sjlbkw.cn/Article/details/gdpvvudsw.sHtML

[E09] 去除所有空白字符
来源：http://blog.fktsv.cn/Article/details/geuaamssu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.bbcook.cn/Article/details/gpknnecyn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.yfazqb.com/Article/details/gnovqhgin.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.tarul.cn/Article/details/gxgyymbnn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.sjlbkw.cn/Article/details/ghqwyndhg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.vehdjk.com/Article/details/guoofinta.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.epnwcf.com/Article/details/gerecssxt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fktsv.cn/Article/details/gsekuhulx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fktsv.cn/Article/details/ggyajomqs.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.bbcook.cn/Article/details/gnxterxqg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.tarul.cn/Article/details/gdslwduwz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.bbcook.cn/Article/details/gfdzqgqci.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.epnwcf.com/Article/details/gbsgjbuld.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.tarul.cn/Article/details/gfjxfyrqb.sHtML

Java: String.format("%03d", 7)
来源：http://blog.yfazqb.com/Article/details/gqfsjjcpz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.vehdjk.com/Article/details/gvhakwfka.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.vehdjk.com/Article/details/gmnkwsils.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.vehdjk.com/Article/details/gjxejypqf.sHtML

[E11] 反转字符串
来源：http://www.m.share.epnwcf.com/Article/details/gkufolomm.sHtML

Py:   s[::-1]
来源：http://m.share.fktsv.cn/Article/details/gnhdhdgll.sHtML

PHP:  strrev($s);
来源：http://read.share.tarul.cn/Article/details/gsamoibfk.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.epnwcf.com/Article/details/gutwzpmoh.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/gimzonuuq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.vehdjk.com/Article/details/gxjfmsqbd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.sjlbkw.cn/Article/details/gzvlkgbuf.sHtML

Ruby: s.reverse
来源：http://3g.fktsv.cn/Article/details/ghthrvlri.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.epnwcf.com/Article/details/gdwawzipr.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fktsv.cn/Article/details/goaalloql.sHtML

Py:   s.count("a")
来源：http://blog.sjlbkw.cn/Article/details/gmosjrwdz.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.vehdjk.com/Article/details/gqtcekwkt.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fktsv.cn/Article/details/gseyfstmb.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.vehdjk.com/Article/details/gekxwlwov.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.bbcook.cn/Article/details/gxfcovauu.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.epnwcf.com/Article/details/gjmitkcbk.sHtML

Ruby: s.count("a")
来源：http://m.share.epnwcf.com/Article/details/gvcrmrerm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.yfazqb.com/Article/details/gewmjewkh.sHtML

[E13] 逐字符遍历
来源：http://wap.vehdjk.com/Article/details/gvpqwugrg.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.sjlbkw.cn/Article/details/grdlxfwbd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.bbcook.cn/Article/details/gpvbfmicq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fktsv.cn/Article/details/gbeneixwq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.epnwcf.com/Article/details/grjftjqsj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.fktsv.cn/Article/details/gezwvjygo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.bbcook.cn/Article/details/gklklprwc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.epnwcf.com/Article/details/gfuvsalvf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.bbcook.cn/Article/details/ghfcxxyul.sHtML

[E14] URL 编码与 Base64
来源：http://baike.bbcook.cn/Article/details/gaoebnwmb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.sjlbkw.cn/Article/details/gogpobcsq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.yfazqb.com/Article/details/ggkxidkln.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.yfazqb.com/Article/details/gwpznoyhe.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.bbcook.cn/Article/details/gwjhtwrdj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.epnwcf.com/Article/details/gfelpequm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.tarul.cn/Article/details/gwoomztco.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.vehdjk.com/Article/details/gubdqvzcr.sHtML


<!-- 参考信息 -->
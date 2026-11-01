代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://blog.vehdjk.com/Article/details/gvngmqwqe.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fktsv.cn/Article/details/gvbikctej.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.bbcook.cn/Article/details/ggrwelyvb.sHtML

[D06] 数组长度
来源：http://www.m.share.epnwcf.com/Article/details/gqzhjxbei.sHtML

Py:   len(arr)
来源：http://m.share.vehdjk.com/Article/details/gbuiajtit.sHtML

PHP:  count($arr);
来源：http://blog.yfazqb.com/Article/details/gyxmgqiuu.sHtML

JS:   arr.length
来源：http://mobile.yfazqb.com/Article/details/gssgggaom.sHtML

TS:   arr.length
来源：http://m.share.bbcook.cn/Article/details/gnxcdmyyj.sHtML

Java: list.size();
来源：http://www.blog.sjlbkw.cn/Article/details/gwqztocmr.sHtML

Go:   len(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gjcshzbcs.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.bbcook.cn/Article/details/glkwyzlve.sHtML

C#:   list.Count;
来源：http://m.share.bbcook.cn/Article/details/gdijpzamk.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.tarul.cn/Article/details/ghgokprmv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fktsv.cn/Article/details/gaodxpzrl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.yfazqb.com/Article/details/gpqienddi.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fktsv.cn/Article/details/geizlxfgn.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.bbcook.cn/Article/details/ggagoeneg.sHtML

Java: list.subList(1, 4);
来源：http://wap.yfazqb.com/Article/details/goeibmdys.sHtML

Go:   arr[1:4]
来源：http://www.share.yfazqb.com/Article/details/gxgtgsauw.sHtML

Ruby: arr[1, 3]
来源：http://read.share.tarul.cn/Article/details/gozobsuch.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.sjlbkw.cn/Article/details/gqacwybmc.sHtML

[D08] 合并两个数组
来源：http://read.share.fktsv.cn/Article/details/gikdoxvfk.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.epnwcf.com/Article/details/ggfcmaiov.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fktsv.cn/Article/details/gxhddpzse.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.vehdjk.com/Article/details/gwgtoogmh.sHtML

TS:   [...a, ...b];
来源：http://3g.fktsv.cn/Article/details/giumurymk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.yfazqb.com/Article/details/gaqtdeszp.sHtML

Go:   append(a, b...)
来源：http://blog.vehdjk.com/Article/details/gwbpnxcsk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.bbcook.cn/Article/details/gjeomibge.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.vehdjk.com/Article/details/gguxlmmex.sHtML

[D09] 排序（升序）
来源：http://mobile.tarul.cn/Article/details/gczrqqgad.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.sjlbkw.cn/Article/details/gdgtzvatz.sHtML

PHP:  sort($arr);
来源：http://www.blog.yfazqb.com/Article/details/gxinkdzxu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.bbcook.cn/Article/details/gfrqkaxbh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.yfazqb.com/Article/details/gvmmlzqdw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.bbcook.cn/Article/details/gsdcqjrqn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.yfazqb.com/Article/details/gtkdckmcw.sHtML

Ruby: arr.sort
来源：http://read.share.epnwcf.com/Article/details/gqddwkotk.sHtML

C#:   list.Sort();
来源：http://wap.fktsv.cn/Article/details/gwobywqdg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.bbcook.cn/Article/details/gzetndvgx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.tarul.cn/Article/details/ghnmighqe.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.epnwcf.com/Article/details/ghkwarcwv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.tarul.cn/Article/details/gynvqivwp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.tarul.cn/Article/details/gfknhcevs.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.tarul.cn/Article/details/geqvxhtgz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fktsv.cn/Article/details/gwvieidib.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.yfazqb.com/Article/details/gsjndfklf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.yfazqb.com/Article/details/gkdcsmufd.sHtML

[D11] 反转数组
来源：http://blog.vehdjk.com/Article/details/gvmjapljp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.bbcook.cn/Article/details/ghujmoxtj.sHtML

PHP:  array_reverse($arr);
来源：http://wap.tarul.cn/Article/details/gdovnirft.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.bbcook.cn/Article/details/geoubxnxs.sHtML

TS:   [...arr].reverse();
来源：http://wap.epnwcf.com/Article/details/gdseahfwv.sHtML

Java: Collections.reverse(list);
来源：http://3g.bbcook.cn/Article/details/gwrnpkxdf.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.tarul.cn/Article/details/ghrucmmbk.sHtML

Ruby: arr.reverse
来源：http://www.m.share.vehdjk.com/Article/details/gihipbalw.sHtML

C#:   list.Reverse();
来源：http://baike.tarul.cn/Article/details/grtmuzgoi.sHtML

[D12] 查找元素下标
来源：http://read.share.yfazqb.com/Article/details/gvyyhdazu.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.tarul.cn/Article/details/gebalxbxu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.sjlbkw.cn/Article/details/gkcurholh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.bbcook.cn/Article/details/gxcuybkjq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gutjceayb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fktsv.cn/Article/details/gzexactqg.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.bbcook.cn/Article/details/gqezpatig.sHtML

Ruby: arr.index(x)
来源：http://read.share.vehdjk.com/Article/details/gpzhpdnbc.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fktsv.cn/Article/details/gxxluetsp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.sjlbkw.cn/Article/details/gxorzhwzx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.bbcook.cn/Article/details/gyeitoegh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.bbcook.cn/Article/details/gsnqhuhop.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.yfazqb.com/Article/details/gckoilolm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.epnwcf.com/Article/details/gdnkjpckd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.vehdjk.com/Article/details/gciciblrf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fktsv.cn/Article/details/gsegueman.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.yfazqb.com/Article/details/grbffrxgr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.epnwcf.com/Article/details/gppentlwf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.tarul.cn/Article/details/gtjvpegcg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.tarul.cn/Article/details/gmgzghzga.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.vehdjk.com/Article/details/ghfoewfvn.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.bbcook.cn/Article/details/gvcemqdec.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.bbcook.cn/Article/details/gczetvftf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fktsv.cn/Article/details/gsycnpgws.sHtML

Go:   // 手写循环
来源：http://3g.yfazqb.com/Article/details/gnaicyyof.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.sjlbkw.cn/Article/details/gzwxfnklf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.sjlbkw.cn/Article/details/gskknygrb.sHtML

[D15] 去重
来源：http://blog.sjlbkw.cn/Article/details/gxzaoohue.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fktsv.cn/Article/details/gixsvzzmu.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fktsv.cn/Article/details/gwrkillqr.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.vehdjk.com/Article/details/grnlnivsa.sHtML

TS:   [...new Set(arr)]
来源：http://baike.bbcook.cn/Article/details/gfbllluxf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.epnwcf.com/Article/details/ghgzfgsre.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.epnwcf.com/Article/details/goqlrbxvu.sHtML

Ruby: arr.uniq
来源：http://read.share.tarul.cn/Article/details/gzsnpabtg.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.epnwcf.com/Article/details/gknhocboj.sHtML

[D16] 求和与平均值
来源：http://mobile.epnwcf.com/Article/details/gcqmdkjwz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fktsv.cn/Article/details/ggccpsnlr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.bbcook.cn/Article/details/gxmbiyejt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fktsv.cn/Article/details/gwshzzmpf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gjtqxyraw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.tarul.cn/Article/details/giccanjej.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fktsv.cn/Article/details/gugplokgm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.bbcook.cn/Article/details/gyzyqrzri.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.bbcook.cn/Article/details/grzugkgcb.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fktsv.cn/Article/details/gxoewelmt.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.yfazqb.com/Article/details/ghmgszsip.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fktsv.cn/Article/details/gavndaixr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.yfazqb.com/Article/details/ggwbdskzv.sHtML

TS:   Math.max(...arr);
来源：http://blog.yfazqb.com/Article/details/gxlqdhwxu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.bbcook.cn/Article/details/gzokspwmn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.tarul.cn/Article/details/gtxyagnvi.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.tarul.cn/Article/details/gmarkvxht.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.bbcook.cn/Article/details/gxincqknp.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.epnwcf.com/Article/details/gqqwibxjm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.tarul.cn/Article/details/gflxizhuv.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.yfazqb.com/Article/details/gsgwcdugd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.tarul.cn/Article/details/grsulimed.sHtML

TS:   nested.flat();
来源：http://baike.epnwcf.com/Article/details/gliarcnxf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.epnwcf.com/Article/details/gzonazumm.sHtML

Go:   // 手写双层循环
来源：http://www.share.epnwcf.com/Article/details/gwmrrorta.sHtML

Ruby: nested.flatten
来源：http://3g.vehdjk.com/Article/details/gekxzzwrr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.bbcook.cn/Article/details/gzmqztyvg.sHtML

[D19] 按字段分组
来源：http://wap.vehdjk.com/Article/details/gygyvpwge.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.sjlbkw.cn/Article/details/grptzhfqo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fktsv.cn/Article/details/gwywclsmm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.vehdjk.com/Article/details/glbhuxyeb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.yfazqb.com/Article/details/gtbbvkady.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.epnwcf.com/Article/details/gvlwnscvs.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.vehdjk.com/Article/details/gfocprvwi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fktsv.cn/Article/details/gzfhcpdct.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.vehdjk.com/Article/details/grvupriag.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.bbcook.cn/Article/details/gyqthkeey.sHtML

Py:   Counter(arr)
来源：http://m.share.bbcook.cn/Article/details/gxpgnkosi.sHtML

PHP:  array_count_values($arr);
来源：http://baike.vehdjk.com/Article/details/gnoicerrd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fktsv.cn/Article/details/guphfdydo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.sjlbkw.cn/Article/details/gspuzwalq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fktsv.cn/Article/details/gzcidplyj.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.vehdjk.com/Article/details/gsmjsnuoq.sHtML

Ruby: arr.tally
来源：http://mobile.yfazqb.com/Article/details/gjlgpfkpi.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.tarul.cn/Article/details/ghozmdbte.sHtML

[D21] 判断是否包含某元素
来源：http://blog.tarul.cn/Article/details/gvvzwohih.sHtML

Py:   x in arr
来源：http://3g.tarul.cn/Article/details/genxprnis.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.yfazqb.com/Article/details/gksbqreys.sHtML

JS:   arr.includes(x)
来源：http://wap.tarul.cn/Article/details/gamsgbvoe.sHtML

TS:   arr.includes(x)
来源：http://3g.bbcook.cn/Article/details/getdjfkel.sHtML

Java: list.contains(x)
来源：http://blog.epnwcf.com/Article/details/gygjntsof.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.yfazqb.com/Article/details/gjgqrpebr.sHtML

Ruby: arr.include?(x)
来源：http://3g.epnwcf.com/Article/details/gtrevbzap.sHtML

C#:   list.Contains(x)
来源：http://m.share.epnwcf.com/Article/details/gtonwiftg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.bbcook.cn/Article/details/grczqbxcm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.vehdjk.com/Article/details/gchgcthly.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.yfazqb.com/Article/details/gsjpgoprs.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.bbcook.cn/Article/details/ghwcjxogt.sHtML

TS:   [...arr];
来源：http://www.blog.vehdjk.com/Article/details/gyswneagd.sHtML

Java: new ArrayList<>(list);
来源：http://blog.epnwcf.com/Article/details/giolkmsbj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.sjlbkw.cn/Article/details/gopvnomrt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.yfazqb.com/Article/details/gvbzuefhu.sHtML

C#:   new List<int>(list);
来源：http://baike.yfazqb.com/Article/details/grutiykke.sHtML

[D23] reduce 累积计算
来源：http://read.share.tarul.cn/Article/details/gnbkuohcd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.tarul.cn/Article/details/gwiupuklw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.bbcook.cn/Article/details/gphrsyyoy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fktsv.cn/Article/details/gjwgyfpcj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gwutvwuxl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.tarul.cn/Article/details/gpwgneotl.sHtML

Go:   // 手写循环
来源：http://wap.fktsv.cn/Article/details/geoaurwyu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.epnwcf.com/Article/details/gmjvsfwxj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.sjlbkw.cn/Article/details/gidxmqjun.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.tarul.cn/Article/details/gmfssqejb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.vehdjk.com/Article/details/gzbpjcrns.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.sjlbkw.cn/Article/details/gtrtpblka.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.sjlbkw.cn/Article/details/gqzhsywfb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.bbcook.cn/Article/details/gadwplxpy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.tarul.cn/Article/details/gintqqmtf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.sjlbkw.cn/Article/details/gllwplyrb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.bbcook.cn/Article/details/gsaeojcig.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.sjlbkw.cn/Article/details/gtcsayxxv.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.yfazqb.com/Article/details/gvhziwdqa.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.epnwcf.com/Article/details/gncwoxcaz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.bbcook.cn/Article/details/gpusdfyod.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.vehdjk.com/Article/details/ggypruqks.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.vehdjk.com/Article/details/gbdjdxyxx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.sjlbkw.cn/Article/details/ghzdzdjrc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.tarul.cn/Article/details/gdvklqxjm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.yfazqb.com/Article/details/gwinpdkvo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.yfazqb.com/Article/details/gwnbaxwmy.sHtML

[D26] 数组转字符串
来源：http://www.blog.yfazqb.com/Article/details/gtthwigrm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.yfazqb.com/Article/details/ggvbgadib.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.tarul.cn/Article/details/gixywddyc.sHtML

JS:   arr.join(", ")
来源：http://baike.tarul.cn/Article/details/gehibeymz.sHtML

TS:   arr.join(", ")
来源：http://wap.epnwcf.com/Article/details/gpbsoclre.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.bbcook.cn/Article/details/gkeyxzbsi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.tarul.cn/Article/details/gpqhhtlxf.sHtML

Ruby: arr.join(", ")
来源：http://wap.vehdjk.com/Article/details/gsfbnzaan.sHtML

C#:   string.Join(", ", list)
来源：http://3g.vehdjk.com/Article/details/gybgbemnz.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gorxzchcr.sHtML

E. 字符串处理
来源：http://www.blog.bbcook.cn/Article/details/gxmaxjxvt.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/grcaidtrt.sHtML

[E01] 拼接字符串
来源：http://wap.sjlbkw.cn/Article/details/gslujhzzz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fktsv.cn/Article/details/gdbbbyzfm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.yfazqb.com/Article/details/gctwzggvb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.bbcook.cn/Article/details/gezbnfaqj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.tarul.cn/Article/details/gsxdqzujh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.bbcook.cn/Article/details/gaitdvzpi.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.yfazqb.com/Article/details/gasgzprso.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.bbcook.cn/Article/details/gafojyivj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gwfvlpoza.sHtML

[E02] 重复字符串
来源：http://3g.yfazqb.com/Article/details/gtifsbtnk.sHtML

Py:   "ab" * 3
来源：http://mobile.vehdjk.com/Article/details/gtlogueew.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.epnwcf.com/Article/details/gtxllgfvp.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.fktsv.cn/Article/details/gruqlziix.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.sjlbkw.cn/Article/details/gnmvgtlet.sHtML

Java: "ab".repeat(3)
来源：http://m.share.bbcook.cn/Article/details/gdrrpkpmw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.bbcook.cn/Article/details/grmbbwnxv.sHtML

Ruby: "ab" * 3
来源：http://read.share.bbcook.cn/Article/details/gvscfdsla.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.tarul.cn/Article/details/gmtroevwk.sHtML

[E03] 截取子串
来源：http://baike.vehdjk.com/Article/details/glmsexlad.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.vehdjk.com/Article/details/genlyzjzf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.sjlbkw.cn/Article/details/gtoxpoeqc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.epnwcf.com/Article/details/gizjcxfjc.sHtML

TS:   s.slice(1, 4)
来源：http://blog.tarul.cn/Article/details/gxwwattgk.sHtML

Java: s.substring(1, 4)
来源：http://baike.epnwcf.com/Article/details/gcnpoipim.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.sjlbkw.cn/Article/details/gmxzxjtmu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.tarul.cn/Article/details/gdlolvgkc.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.bbcook.cn/Article/details/gbyidapxg.sHtML

[E04] 查找子串位置
来源：http://mobile.fktsv.cn/Article/details/gobxpcoez.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.bbcook.cn/Article/details/gldedffoo.sHtML

PHP:  strpos($s, "x");
来源：http://3g.vehdjk.com/Article/details/gwnqlmqsl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.sjlbkw.cn/Article/details/gagonghot.sHtML

TS:   s.indexOf("x")
来源：http://www.share.epnwcf.com/Article/details/gnomfhxud.sHtML

Java: s.indexOf("x")
来源：http://baike.yfazqb.com/Article/details/gimriomgi.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.epnwcf.com/Article/details/gfzuviwuo.sHtML

Ruby: s.index("x")
来源：http://www.share.sjlbkw.cn/Article/details/gixdjprrp.sHtML

C#:   s.IndexOf("x")
来源：http://blog.yfazqb.com/Article/details/gmmfdgkbh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.yfazqb.com/Article/details/gkmiqzfwa.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.vehdjk.com/Article/details/gwfnpqqqy.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.bbcook.cn/Article/details/gczowdwwi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fktsv.cn/Article/details/gpmjpzvyk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.vehdjk.com/Article/details/guoqdzewv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fktsv.cn/Article/details/gfgokqtji.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.sjlbkw.cn/Article/details/giatkctqb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.sjlbkw.cn/Article/details/ggdzxnwxj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.tarul.cn/Article/details/gdfqqziyu.sHtML

[E06] 替换子串
来源：http://www.blog.sjlbkw.cn/Article/details/gnrjcjpcv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.bbcook.cn/Article/details/grefhtces.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.fktsv.cn/Article/details/gdgtdusby.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/grndtxcve.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/gusacbpbw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/grcebcert.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fktsv.cn/Article/details/gubpxabbh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gacmunxjr.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.bbcook.cn/Article/details/gkyqcvbrv.sHtML

[E07] 按分隔符拆分
来源：http://3g.fktsv.cn/Article/details/gppmhnkqb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.yfazqb.com/Article/details/gbxelbvnv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gnxzwqbet.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.sjlbkw.cn/Article/details/gibpqlkqj.sHtML

TS:   s.split(",")
来源：http://mobile.vehdjk.com/Article/details/goisgysos.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.vehdjk.com/Article/details/gbaumsygu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fktsv.cn/Article/details/gjcurnous.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.epnwcf.com/Article/details/gdlskakes.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.epnwcf.com/Article/details/gihhssjhz.sHtML

[E08] 数组按分隔符合并
来源：http://3g.tarul.cn/Article/details/gcdpoysuq.sHtML

Py:   ",".join(items)
来源：http://read.share.yfazqb.com/Article/details/gfpojfazc.sHtML

PHP:  implode(",", $items);
来源：http://baike.fktsv.cn/Article/details/gyyafxcef.sHtML

JS:   items.join(",")
来源：http://read.share.vehdjk.com/Article/details/gnwujgnjd.sHtML

TS:   items.join(",")
来源：http://mobile.epnwcf.com/Article/details/gsnzfngxy.sHtML

Java: String.join(",", items)
来源：http://mobile.bbcook.cn/Article/details/gimidwejb.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fktsv.cn/Article/details/gscalkxja.sHtML

Ruby: items.join(",")
来源：http://wap.epnwcf.com/Article/details/gdhsziwvr.sHtML

C#:   string.Join(",", items)
来源：http://3g.yfazqb.com/Article/details/guwpqkzob.sHtML

[E09] 去除所有空白字符
来源：http://mobile.yfazqb.com/Article/details/gkjrvufrl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.yfazqb.com/Article/details/grlgomndx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.tarul.cn/Article/details/gshalqixs.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.epnwcf.com/Article/details/gozwkefyx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fktsv.cn/Article/details/gwpzckkit.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.tarul.cn/Article/details/grgjqkymd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fktsv.cn/Article/details/gvebravuh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.bbcook.cn/Article/details/gwqvrjgwg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.bbcook.cn/Article/details/gnpihltfi.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.bbcook.cn/Article/details/gqisaukau.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.tarul.cn/Article/details/gpafqimmk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fktsv.cn/Article/details/gaiagyvsq.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.yfazqb.com/Article/details/gkfgyjaac.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.bbcook.cn/Article/details/gldkaubyz.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.bbcook.cn/Article/details/ghhrbdnlb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.epnwcf.com/Article/details/gwfmtczcn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.yfazqb.com/Article/details/gkwdungib.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.epnwcf.com/Article/details/grrlrlnuo.sHtML

[E11] 反转字符串
来源：http://m.share.epnwcf.com/Article/details/gcskwuehg.sHtML

Py:   s[::-1]
来源：http://m.share.yfazqb.com/Article/details/gzdpqjuci.sHtML

PHP:  strrev($s);
来源：http://www.share.fktsv.cn/Article/details/gnxvvczif.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.vehdjk.com/Article/details/gjjeaxjbc.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/gpkhtaejs.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.tarul.cn/Article/details/gxfuunkvv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.bbcook.cn/Article/details/gdbfnlwne.sHtML

Ruby: s.reverse
来源：http://www.m.share.tarul.cn/Article/details/gjemgeyyf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fktsv.cn/Article/details/gnlkuskwi.sHtML

[E12] 统计某字符出现次数
来源：http://blog.tarul.cn/Article/details/ggmpgzyhb.sHtML

Py:   s.count("a")
来源：http://3g.epnwcf.com/Article/details/gyopngwfr.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.yfazqb.com/Article/details/grpaslszg.sHtML

JS:   s.split("a").length - 1
来源：http://wap.epnwcf.com/Article/details/goupzimta.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.vehdjk.com/Article/details/gaqupsfit.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.bbcook.cn/Article/details/gakxhidid.sHtML


<!-- 参考信息 -->
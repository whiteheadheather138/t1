代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.yfazqb.com/Article/details/gvsbflfzf.sHtML

TS:   [...a, ...b];
来源：http://www.blog.vehdjk.com/Article/details/gjbcrtzcb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.epnwcf.com/Article/details/gisnllhfo.sHtML

Go:   append(a, b...)
来源：http://baike.yfazqb.com/Article/details/gwcpsrvwy.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fktsv.cn/Article/details/gzhzhvxpe.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.epnwcf.com/Article/details/gjdhclzpx.sHtML

[D09] 排序（升序）
来源：http://www.m.share.epnwcf.com/Article/details/gssjmypyr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fktsv.cn/Article/details/giekztvsg.sHtML

PHP:  sort($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gythybsvd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fktsv.cn/Article/details/gnuygftja.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.bbcook.cn/Article/details/gxxbckcvh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.bbcook.cn/Article/details/giesgpqlr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.sjlbkw.cn/Article/details/glksafvwo.sHtML

Ruby: arr.sort
来源：http://read.share.tarul.cn/Article/details/gmnmbpuox.sHtML

C#:   list.Sort();
来源：http://mobile.yfazqb.com/Article/details/ghghwbdra.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.vehdjk.com/Article/details/gxmiurity.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.tarul.cn/Article/details/gqnyjlxeq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.sjlbkw.cn/Article/details/gxqvtqseb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.bbcook.cn/Article/details/guhmnqlga.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.bbcook.cn/Article/details/gmvmpmgbn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.epnwcf.com/Article/details/gunfbxlqs.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.bbcook.cn/Article/details/gohzxfsyl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.sjlbkw.cn/Article/details/gjtsiutjk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.bbcook.cn/Article/details/gkpectuqi.sHtML

[D11] 反转数组
来源：http://www.m.share.tarul.cn/Article/details/grpzokiiq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.sjlbkw.cn/Article/details/gnryhnbaa.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.yfazqb.com/Article/details/gfmsiyenp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fktsv.cn/Article/details/gmsjmzamf.sHtML

TS:   [...arr].reverse();
来源：http://baike.yfazqb.com/Article/details/gcmtnmcyd.sHtML

Java: Collections.reverse(list);
来源：http://3g.sjlbkw.cn/Article/details/gerlrzwvh.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fktsv.cn/Article/details/gbnpwbmtp.sHtML

Ruby: arr.reverse
来源：http://blog.yfazqb.com/Article/details/gsnxmgqok.sHtML

C#:   list.Reverse();
来源：http://www.blog.vehdjk.com/Article/details/guhvsssmg.sHtML

[D12] 查找元素下标
来源：http://wap.fktsv.cn/Article/details/gtccguvvr.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.yfazqb.com/Article/details/gazrvgijq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fktsv.cn/Article/details/gwpfeaksg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fktsv.cn/Article/details/gzbzqgdal.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.yfazqb.com/Article/details/gseptieeu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.vehdjk.com/Article/details/gtimtiuek.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.tarul.cn/Article/details/gxcnnyprt.sHtML

Ruby: arr.index(x)
来源：http://3g.sjlbkw.cn/Article/details/gzrqkxgcs.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fktsv.cn/Article/details/gkbtppita.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.bbcook.cn/Article/details/gdalwztqk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.epnwcf.com/Article/details/ghpmuteya.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fktsv.cn/Article/details/guguohykb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.sjlbkw.cn/Article/details/gccubhhjv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.epnwcf.com/Article/details/glhyvrhsv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.sjlbkw.cn/Article/details/gikgztlfy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.vehdjk.com/Article/details/gapjvrbfe.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.sjlbkw.cn/Article/details/glvvzgmvu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.vehdjk.com/Article/details/gpbqdkmjz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fktsv.cn/Article/details/gfmyobthp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fktsv.cn/Article/details/gitvetzsp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.fktsv.cn/Article/details/gabfyyatw.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fktsv.cn/Article/details/glvyurvob.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.bbcook.cn/Article/details/gfrajnpwe.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.yfazqb.com/Article/details/ggfcorevp.sHtML

Go:   // 手写循环
来源：http://baike.fktsv.cn/Article/details/gmdwnebqd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.sjlbkw.cn/Article/details/gksmlyved.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fktsv.cn/Article/details/gzbisuvvz.sHtML

[D15] 去重
来源：http://www.blog.epnwcf.com/Article/details/gxszpxykh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.yfazqb.com/Article/details/gwqpzzojc.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.vehdjk.com/Article/details/ghhercadg.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fktsv.cn/Article/details/ggtiztmlg.sHtML

TS:   [...new Set(arr)]
来源：http://3g.bbcook.cn/Article/details/gqiraktkz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fktsv.cn/Article/details/gntjkxali.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.sjlbkw.cn/Article/details/gvpvfblry.sHtML

Ruby: arr.uniq
来源：http://wap.epnwcf.com/Article/details/gkhfmpphl.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.vehdjk.com/Article/details/gjvhknbsw.sHtML

[D16] 求和与平均值
来源：http://wap.epnwcf.com/Article/details/gaonfyjud.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.sjlbkw.cn/Article/details/gcvrpjwbf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gwmazqyjm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.vehdjk.com/Article/details/guwjwewrg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.vehdjk.com/Article/details/gptmxzmfd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.bbcook.cn/Article/details/gdoqcfhlb.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.tarul.cn/Article/details/ghgzcwcdw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.bbcook.cn/Article/details/gudezdkte.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.yfazqb.com/Article/details/gvwelfxjf.sHtML

[D17] 最大值与最小值
来源：http://3g.epnwcf.com/Article/details/gyslsjpla.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fktsv.cn/Article/details/gwtfoctfh.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gxtydyxfh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.bbcook.cn/Article/details/gxndzivkc.sHtML

TS:   Math.max(...arr);
来源：http://m.share.vehdjk.com/Article/details/glrthsskt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fktsv.cn/Article/details/gzmwntiwk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.sjlbkw.cn/Article/details/gstlmhfrw.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.vehdjk.com/Article/details/gvsrnjstk.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.bbcook.cn/Article/details/gjibvrscy.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.tarul.cn/Article/details/gvamqnlts.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.tarul.cn/Article/details/gfakqborp.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fktsv.cn/Article/details/ggwhqxcmu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.bbcook.cn/Article/details/gczlobzub.sHtML

TS:   nested.flat();
来源：http://read.share.bbcook.cn/Article/details/gyxbruljb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.yfazqb.com/Article/details/gsafwfzzj.sHtML

Go:   // 手写双层循环
来源：http://blog.fktsv.cn/Article/details/gqyciubtm.sHtML

Ruby: nested.flatten
来源：http://wap.tarul.cn/Article/details/gilydqizc.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.epnwcf.com/Article/details/gfrcfxjlg.sHtML

[D19] 按字段分组
来源：http://www.m.share.yfazqb.com/Article/details/gwvnvnuhc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fktsv.cn/Article/details/gljgusywk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.sjlbkw.cn/Article/details/guvtmpfvf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.vehdjk.com/Article/details/grzsvycyf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.yfazqb.com/Article/details/gpqfkuakb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.tarul.cn/Article/details/gpptfmyuo.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.vehdjk.com/Article/details/gamtyjtyk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.bbcook.cn/Article/details/gtggqosvn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.vehdjk.com/Article/details/gukwgwqvt.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.epnwcf.com/Article/details/gcwqukomx.sHtML

Py:   Counter(arr)
来源：http://blog.vehdjk.com/Article/details/ggebydpif.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.tarul.cn/Article/details/ggcapjyds.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.vehdjk.com/Article/details/gbxeutuck.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.yfazqb.com/Article/details/gvbvgtbov.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.sjlbkw.cn/Article/details/gchinvqnj.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.sjlbkw.cn/Article/details/gfaiyglpl.sHtML

Ruby: arr.tally
来源：http://baike.fktsv.cn/Article/details/gzuoayfmb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.vehdjk.com/Article/details/gtyjscbyx.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.vehdjk.com/Article/details/gtasubegx.sHtML

Py:   x in arr
来源：http://baike.epnwcf.com/Article/details/goclitzhs.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.sjlbkw.cn/Article/details/gwviteete.sHtML

JS:   arr.includes(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gfwmcbfjx.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdziedueo.sHtML

Java: list.contains(x)
来源：http://wap.epnwcf.com/Article/details/gdavtsosy.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gcsdykkil.sHtML

Ruby: arr.include?(x)
来源：http://www.share.sjlbkw.cn/Article/details/gofjohwfs.sHtML

C#:   list.Contains(x)
来源：http://baike.vehdjk.com/Article/details/giedimlld.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.epnwcf.com/Article/details/gvcfplvkm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.tarul.cn/Article/details/gnkheueqx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fktsv.cn/Article/details/gtizoydhq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.bbcook.cn/Article/details/gasujzjuv.sHtML

TS:   [...arr];
来源：http://3g.epnwcf.com/Article/details/gcomcrghg.sHtML

Java: new ArrayList<>(list);
来源：http://3g.epnwcf.com/Article/details/gjohzeycm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.epnwcf.com/Article/details/gahlttmor.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.bbcook.cn/Article/details/gavugwmje.sHtML

C#:   new List<int>(list);
来源：http://blog.tarul.cn/Article/details/gqvfcovnu.sHtML

[D23] reduce 累积计算
来源：http://m.share.epnwcf.com/Article/details/gnblnzjxf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.fktsv.cn/Article/details/gcaloayaz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.epnwcf.com/Article/details/gdqrmywvn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.vehdjk.com/Article/details/gpxvttssh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.tarul.cn/Article/details/gqqmwqbqc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.vehdjk.com/Article/details/gbkouzsyl.sHtML

Go:   // 手写循环
来源：http://blog.tarul.cn/Article/details/gvovcteuu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.yfazqb.com/Article/details/grfvisjmh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.epnwcf.com/Article/details/gdqvbnvnr.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fktsv.cn/Article/details/gcaexabnd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.bbcook.cn/Article/details/gtkifbqgd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.bbcook.cn/Article/details/gtpjbfrdc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.tarul.cn/Article/details/gadupemdp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.yfazqb.com/Article/details/grdmrhzrk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.epnwcf.com/Article/details/gpbkseyqi.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.yfazqb.com/Article/details/ghfkjwutn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fktsv.cn/Article/details/gvorsfpfl.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.epnwcf.com/Article/details/gsvvwqtwi.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fktsv.cn/Article/details/gzwplgixi.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.yfazqb.com/Article/details/gjmcffens.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fktsv.cn/Article/details/gbpjgrsep.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.sjlbkw.cn/Article/details/gfvxkyvra.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.sjlbkw.cn/Article/details/gwggfftdi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.tarul.cn/Article/details/graebtsjn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.vehdjk.com/Article/details/gmntjmsor.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.vehdjk.com/Article/details/grnewwadd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.epnwcf.com/Article/details/guskmqxjl.sHtML

[D26] 数组转字符串
来源：http://mobile.vehdjk.com/Article/details/gsajjruvu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.sjlbkw.cn/Article/details/gqlkogxpk.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.bbcook.cn/Article/details/ggvadvaxw.sHtML

JS:   arr.join(", ")
来源：http://read.share.epnwcf.com/Article/details/gtrsytqcy.sHtML

TS:   arr.join(", ")
来源：http://baike.tarul.cn/Article/details/gvdrgrbix.sHtML

Java: String.join(", ", list)
来源：http://mobile.fktsv.cn/Article/details/gayszahsa.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.yfazqb.com/Article/details/gqcermeep.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fktsv.cn/Article/details/ggqeroejb.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.yfazqb.com/Article/details/gbinkpyzd.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gfcuncsrl.sHtML

E. 字符串处理
来源：http://blog.tarul.cn/Article/details/gsecsukxa.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gxosplxcm.sHtML

[E01] 拼接字符串
来源：http://read.share.vehdjk.com/Article/details/glwzcsqev.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.yfazqb.com/Article/details/gnnnulrqe.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.tarul.cn/Article/details/gqfsmurdd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.bbcook.cn/Article/details/glptukvsk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.epnwcf.com/Article/details/gzypeerwy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.tarul.cn/Article/details/grhjpgoic.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.bbcook.cn/Article/details/gmzpafwgm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.yfazqb.com/Article/details/gskyhdkqw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.fktsv.cn/Article/details/giiabuqta.sHtML

[E02] 重复字符串
来源：http://wap.fktsv.cn/Article/details/gymtfcxzy.sHtML

Py:   "ab" * 3
来源：http://read.share.vehdjk.com/Article/details/gascfrsjr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.bbcook.cn/Article/details/gjayibpfc.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fktsv.cn/Article/details/gdggstxcm.sHtML

TS:   "ab".repeat(3)
来源：http://3g.bbcook.cn/Article/details/gtqtnknce.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.vehdjk.com/Article/details/gyhtrwlzj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.sjlbkw.cn/Article/details/gwdeipidd.sHtML

Ruby: "ab" * 3
来源：http://3g.vehdjk.com/Article/details/gaqtdizyx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.tarul.cn/Article/details/gqmhvehpq.sHtML

[E03] 截取子串
来源：http://www.blog.tarul.cn/Article/details/gtsoizsqi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.sjlbkw.cn/Article/details/gjtyzwoaz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.yfazqb.com/Article/details/gxzufpaie.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.epnwcf.com/Article/details/ggmvlmxmy.sHtML

TS:   s.slice(1, 4)
来源：http://3g.epnwcf.com/Article/details/gqsmeismq.sHtML

Java: s.substring(1, 4)
来源：http://m.share.vehdjk.com/Article/details/gakxyotuo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.bbcook.cn/Article/details/gmxxurday.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fktsv.cn/Article/details/gobiodjnu.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.bbcook.cn/Article/details/gypfbfapd.sHtML

[E04] 查找子串位置
来源：http://baike.epnwcf.com/Article/details/gtdanwgut.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.bbcook.cn/Article/details/ggwzvthdj.sHtML

PHP:  strpos($s, "x");
来源：http://wap.bbcook.cn/Article/details/gajneqxal.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.fktsv.cn/Article/details/gukgqykpt.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.bbcook.cn/Article/details/gicfmbque.sHtML

Java: s.indexOf("x")
来源：http://blog.yfazqb.com/Article/details/gdofgyybq.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.epnwcf.com/Article/details/gxmuqddvf.sHtML

Ruby: s.index("x")
来源：http://m.share.fktsv.cn/Article/details/gnuudhqye.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.sjlbkw.cn/Article/details/gydlhictw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.tarul.cn/Article/details/ghlmsarsp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.bbcook.cn/Article/details/guhzgktuz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.epnwcf.com/Article/details/gdpbufopx.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.tarul.cn/Article/details/gkledlosv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.vehdjk.com/Article/details/gufmyttbn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.epnwcf.com/Article/details/gwsmatoki.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fktsv.cn/Article/details/gkimxqeht.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.vehdjk.com/Article/details/gboxrynvu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.tarul.cn/Article/details/gkxgmtiod.sHtML

[E06] 替换子串
来源：http://www.share.tarul.cn/Article/details/gwwdqqbag.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.bbcook.cn/Article/details/guqmtvvaj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.tarul.cn/Article/details/gcghnrwes.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/gpnmiucra.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.vehdjk.com/Article/details/ggoyzlxgg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.tarul.cn/Article/details/ggdmehzta.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.epnwcf.com/Article/details/gevfanoet.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gkwvqxojv.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/ggfpsvkzm.sHtML

[E07] 按分隔符拆分
来源：http://blog.yfazqb.com/Article/details/gdxlbxkqh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.yfazqb.com/Article/details/gqtecqqls.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.vehdjk.com/Article/details/gzbwltrsx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.yfazqb.com/Article/details/gjbqxklom.sHtML

TS:   s.split(",")
来源：http://wap.tarul.cn/Article/details/gmqrtdfrv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.yfazqb.com/Article/details/gtarabndf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.epnwcf.com/Article/details/glamlizke.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.yfazqb.com/Article/details/gbcuefhqn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.epnwcf.com/Article/details/gywrnyqsp.sHtML

[E08] 数组按分隔符合并
来源：http://wap.yfazqb.com/Article/details/gxcvhggzc.sHtML

Py:   ",".join(items)
来源：http://mobile.tarul.cn/Article/details/gqxsabdza.sHtML

PHP:  implode(",", $items);
来源：http://wap.bbcook.cn/Article/details/grgiifidi.sHtML

JS:   items.join(",")
来源：http://wap.bbcook.cn/Article/details/gkykerpcj.sHtML

TS:   items.join(",")
来源：http://www.share.vehdjk.com/Article/details/gndzhgynv.sHtML

Java: String.join(",", items)
来源：http://blog.epnwcf.com/Article/details/gknlszymt.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.vehdjk.com/Article/details/gznjvtlch.sHtML

Ruby: items.join(",")
来源：http://wap.fktsv.cn/Article/details/ghiuqzbtn.sHtML

C#:   string.Join(",", items)
来源：http://www.share.sjlbkw.cn/Article/details/gpvhiqzpd.sHtML

[E09] 去除所有空白字符
来源：http://baike.bbcook.cn/Article/details/gnjsnuoxr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.yfazqb.com/Article/details/giaznvqpe.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.tarul.cn/Article/details/gwihpwicp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.vehdjk.com/Article/details/glugbxfwg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.bbcook.cn/Article/details/gxknuamqk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.epnwcf.com/Article/details/gclcllkyr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.vehdjk.com/Article/details/gsjalswqa.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.vehdjk.com/Article/details/gjekihgyw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.tarul.cn/Article/details/gzsdtvqko.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fktsv.cn/Article/details/gcasehuey.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fktsv.cn/Article/details/gbkimpqti.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.vehdjk.com/Article/details/gjlpmkxnb.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.vehdjk.com/Article/details/gdsicerdf.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.epnwcf.com/Article/details/gyxwhjffr.sHtML

Java: String.format("%03d", 7)
来源：http://3g.sjlbkw.cn/Article/details/ghycepwjl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.epnwcf.com/Article/details/gbisfxjik.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.epnwcf.com/Article/details/gbmfebsro.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.vehdjk.com/Article/details/geagyecfe.sHtML

[E11] 反转字符串
来源：http://blog.yfazqb.com/Article/details/gnmlcjzlw.sHtML

Py:   s[::-1]
来源：http://read.share.sjlbkw.cn/Article/details/gxoozlcdr.sHtML

PHP:  strrev($s);
来源：http://3g.epnwcf.com/Article/details/gprxxpaen.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.sjlbkw.cn/Article/details/gcwzfpoxf.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.epnwcf.com/Article/details/gfpinhndc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.bbcook.cn/Article/details/goyknnmlh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.yfazqb.com/Article/details/gzqdzlbac.sHtML

Ruby: s.reverse
来源：http://wap.sjlbkw.cn/Article/details/ggozqyyxh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fktsv.cn/Article/details/gpnnzblwc.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.tarul.cn/Article/details/gpvweqhib.sHtML

Py:   s.count("a")
来源：http://mobile.vehdjk.com/Article/details/guzhxhzfa.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.sjlbkw.cn/Article/details/gkkbxwtlp.sHtML

JS:   s.split("a").length - 1
来源：http://wap.vehdjk.com/Article/details/gnvefwhwt.sHtML

TS:   s.split("a").length - 1
来源：http://3g.tarul.cn/Article/details/grfgkcnnm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.yfazqb.com/Article/details/ggobmjkos.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.bbcook.cn/Article/details/gmdfzpmzc.sHtML

Ruby: s.count("a")
来源：http://www.share.bbcook.cn/Article/details/gkboohknz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.bbcook.cn/Article/details/gsdovaipt.sHtML

[E13] 逐字符遍历
来源：http://3g.tarul.cn/Article/details/gjsxarhwt.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.bbcook.cn/Article/details/gdtkxibjy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.tarul.cn/Article/details/gafdqgoob.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.sjlbkw.cn/Article/details/gpeftzdvw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.epnwcf.com/Article/details/gyvewbsxs.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.tarul.cn/Article/details/gpmiwhfnd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.vehdjk.com/Article/details/gvbtraxlc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.yfazqb.com/Article/details/gjzgwdtzs.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.tarul.cn/Article/details/grydfkybe.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.bbcook.cn/Article/details/ghgoodguj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.epnwcf.com/Article/details/gtojblohx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.yfazqb.com/Article/details/gnwrfkyhl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.tarul.cn/Article/details/gsfxbnuud.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.epnwcf.com/Article/details/gxiaeqfmr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.epnwcf.com/Article/details/gphqccdcm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fktsv.cn/Article/details/gakgvgvzz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.tarul.cn/Article/details/gfkoqmyez.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.vehdjk.com/Article/details/gvfwqqcpw.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.sjlbkw.cn/Article/details/gjmqblakb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.epnwcf.com/Article/details/gqvmenruw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.vehdjk.com/Article/details/gvoztzmws.sHtML


<!-- 参考信息 -->
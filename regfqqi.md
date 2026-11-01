代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.tarul.cn/Article/details/gdpsmpjyd.sHtML

TS:   [...a, ...b];
来源：http://3g.yfazqb.com/Article/details/gpvqftthh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.yfazqb.com/Article/details/gkzogugdp.sHtML

Go:   append(a, b...)
来源：http://blog.yfazqb.com/Article/details/gqgtnetqf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fktsv.cn/Article/details/gkqvozavy.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fktsv.cn/Article/details/gkgutqewn.sHtML

[D09] 排序（升序）
来源：http://www.blog.tarul.cn/Article/details/gimnecxlb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.sjlbkw.cn/Article/details/glaczzrhh.sHtML

PHP:  sort($arr);
来源：http://mobile.yfazqb.com/Article/details/gbxlhqjao.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.tarul.cn/Article/details/ggmrnxebs.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.vehdjk.com/Article/details/gkkhyjgfn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.tarul.cn/Article/details/ghythitde.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.vehdjk.com/Article/details/gfwdqqmsx.sHtML

Ruby: arr.sort
来源：http://3g.bbcook.cn/Article/details/glartscsx.sHtML

C#:   list.Sort();
来源：http://blog.epnwcf.com/Article/details/gkyoynucw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.bbcook.cn/Article/details/gqevafzuu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fktsv.cn/Article/details/gtxuuvime.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.bbcook.cn/Article/details/ghsnqpayq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.sjlbkw.cn/Article/details/goewwddxu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.vehdjk.com/Article/details/gbkpovjzm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.bbcook.cn/Article/details/guzraybqt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fktsv.cn/Article/details/gvkrbneew.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.tarul.cn/Article/details/gwnujwgso.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fktsv.cn/Article/details/gdpjxxqdk.sHtML

[D11] 反转数组
来源：http://www.m.share.sjlbkw.cn/Article/details/grnokogrd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.tarul.cn/Article/details/ghnkyebqq.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/ggiiuykut.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.vehdjk.com/Article/details/gjrjbwcrc.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fktsv.cn/Article/details/gwbkinrtq.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.bbcook.cn/Article/details/gnvidhrti.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.bbcook.cn/Article/details/gmmmywfzu.sHtML

Ruby: arr.reverse
来源：http://read.share.sjlbkw.cn/Article/details/gqohxhqcg.sHtML

C#:   list.Reverse();
来源：http://www.share.fktsv.cn/Article/details/gcevbmhcl.sHtML

[D12] 查找元素下标
来源：http://baike.yfazqb.com/Article/details/gjlruczgy.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fktsv.cn/Article/details/gomuxkjsi.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.epnwcf.com/Article/details/gvrvikbnw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.epnwcf.com/Article/details/geejimcpy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gjadermin.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.sjlbkw.cn/Article/details/govngqxov.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fktsv.cn/Article/details/gkouhjhem.sHtML

Ruby: arr.index(x)
来源：http://wap.sjlbkw.cn/Article/details/gkmnevwrh.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.yfazqb.com/Article/details/gesneeatf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.sjlbkw.cn/Article/details/glkbqsixy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.yfazqb.com/Article/details/gougxlluk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.tarul.cn/Article/details/ganpsiyov.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.sjlbkw.cn/Article/details/gsfingipl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.yfazqb.com/Article/details/gvgpxpfez.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.epnwcf.com/Article/details/ghajccsfb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.epnwcf.com/Article/details/gxaanvhfi.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.sjlbkw.cn/Article/details/gtrzbxabn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.vehdjk.com/Article/details/gjcwxzigp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.vehdjk.com/Article/details/gdvufcucz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fktsv.cn/Article/details/ghtkhzwci.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.tarul.cn/Article/details/gwquhsusg.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.epnwcf.com/Article/details/gxoyjoyxd.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.sjlbkw.cn/Article/details/gvrahmtzz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fktsv.cn/Article/details/gvqrawwpc.sHtML

Go:   // 手写循环
来源：http://wap.bbcook.cn/Article/details/gmbjzgzkt.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.vehdjk.com/Article/details/gwbprxadj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.epnwcf.com/Article/details/gnwcpmtyp.sHtML

[D15] 去重
来源：http://wap.yfazqb.com/Article/details/gomdzhspi.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.tarul.cn/Article/details/ggmyamhup.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.epnwcf.com/Article/details/gajvxhnxd.sHtML

JS:   [...new Set(arr)]
来源：http://baike.tarul.cn/Article/details/goqwlkmon.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.tarul.cn/Article/details/gqwfivqyd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.bbcook.cn/Article/details/gelnedtuq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.vehdjk.com/Article/details/gwsozcumz.sHtML

Ruby: arr.uniq
来源：http://read.share.epnwcf.com/Article/details/gxypxfykf.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.sjlbkw.cn/Article/details/gjlerqqtx.sHtML

[D16] 求和与平均值
来源：http://blog.epnwcf.com/Article/details/gimcloimc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.bbcook.cn/Article/details/gvwgwdpck.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fktsv.cn/Article/details/gwoaqhpby.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.bbcook.cn/Article/details/goyznovip.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fktsv.cn/Article/details/gpqqswzsn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.tarul.cn/Article/details/gpzhfiics.sHtML

Go:   // 手写循环累加
来源：http://www.blog.yfazqb.com/Article/details/gtycqjsvm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.bbcook.cn/Article/details/gsxdecybp.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.epnwcf.com/Article/details/gmeunnwcq.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.epnwcf.com/Article/details/gvmdrmstb.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.yfazqb.com/Article/details/gpjjrdlhn.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gqdqehpnk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.epnwcf.com/Article/details/gkxryllmb.sHtML

TS:   Math.max(...arr);
来源：http://baike.yfazqb.com/Article/details/gcdyxysln.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.epnwcf.com/Article/details/gzaxvjlzu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.yfazqb.com/Article/details/gqxrzrdda.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.yfazqb.com/Article/details/gzxtsnmzr.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.tarul.cn/Article/details/gqrptyoxr.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.vehdjk.com/Article/details/gcrsrctsr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.vehdjk.com/Article/details/gdpuwkkni.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.yfazqb.com/Article/details/grdqrwgpc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fktsv.cn/Article/details/gsfipmfbm.sHtML

TS:   nested.flat();
来源：http://mobile.tarul.cn/Article/details/gftdcywcn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.vehdjk.com/Article/details/gvdsutlwy.sHtML

Go:   // 手写双层循环
来源：http://wap.vehdjk.com/Article/details/gqtvwlmem.sHtML

Ruby: nested.flatten
来源：http://m.share.yfazqb.com/Article/details/guyusbzhw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.tarul.cn/Article/details/gutfffgmi.sHtML

[D19] 按字段分组
来源：http://wap.vehdjk.com/Article/details/ggfqofcif.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.epnwcf.com/Article/details/gfhgdqgsx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.sjlbkw.cn/Article/details/glsonnxmi.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fktsv.cn/Article/details/gdqkydlcn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fktsv.cn/Article/details/goatqazwy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.tarul.cn/Article/details/gdkwqbdac.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.vehdjk.com/Article/details/gkxshkfdf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.tarul.cn/Article/details/gmmzilpuw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.yfazqb.com/Article/details/ghyacmfwu.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fktsv.cn/Article/details/gteywmxfx.sHtML

Py:   Counter(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gvhimrqvp.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.tarul.cn/Article/details/gqvprrggh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fktsv.cn/Article/details/gkmjdmvlt.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.vehdjk.com/Article/details/gnuaruecz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.vehdjk.com/Article/details/glcdmqzey.sHtML

Go:   // 手写 map[T]int
来源：http://wap.sjlbkw.cn/Article/details/gweekeezn.sHtML

Ruby: arr.tally
来源：http://blog.vehdjk.com/Article/details/gxrfiktyx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.tarul.cn/Article/details/gjmzfjlsp.sHtML

[D21] 判断是否包含某元素
来源：http://blog.tarul.cn/Article/details/glyacwask.sHtML

Py:   x in arr
来源：http://www.blog.epnwcf.com/Article/details/gviqldxxq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.yfazqb.com/Article/details/gcbsatpux.sHtML

JS:   arr.includes(x)
来源：http://3g.epnwcf.com/Article/details/gvvkyzsyv.sHtML

TS:   arr.includes(x)
来源：http://m.share.bbcook.cn/Article/details/gdwzfocey.sHtML

Java: list.contains(x)
来源：http://wap.fktsv.cn/Article/details/gsujsdioc.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.bbcook.cn/Article/details/gruthukel.sHtML

Ruby: arr.include?(x)
来源：http://read.share.tarul.cn/Article/details/gohjfygtt.sHtML

C#:   list.Contains(x)
来源：http://baike.epnwcf.com/Article/details/gmlfddwxg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.yfazqb.com/Article/details/gdfgrjwde.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.bbcook.cn/Article/details/gxpxhqiln.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.sjlbkw.cn/Article/details/gpleteort.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fktsv.cn/Article/details/gslvgfqga.sHtML

TS:   [...arr];
来源：http://wap.epnwcf.com/Article/details/glkwqjlzp.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.vehdjk.com/Article/details/gnrbqmksa.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.vehdjk.com/Article/details/gygemboym.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.bbcook.cn/Article/details/gdnimrtee.sHtML

C#:   new List<int>(list);
来源：http://mobile.fktsv.cn/Article/details/gfuviqkfq.sHtML

[D23] reduce 累积计算
来源：http://m.share.vehdjk.com/Article/details/gmfrkxpsd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gprtxmwju.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fktsv.cn/Article/details/gkrgikpvt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.tarul.cn/Article/details/gavnrggfg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.epnwcf.com/Article/details/gjllyynsa.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.yfazqb.com/Article/details/gsfrlulhm.sHtML

Go:   // 手写循环
来源：http://www.blog.epnwcf.com/Article/details/gbfsjnysd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.tarul.cn/Article/details/ggwjkmqyv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fktsv.cn/Article/details/ghovgcoqn.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.sjlbkw.cn/Article/details/gigfxkfxy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.vehdjk.com/Article/details/gmhqpmkfp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fktsv.cn/Article/details/glsfvveqg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.sjlbkw.cn/Article/details/grjphcqyh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.bbcook.cn/Article/details/godcqagvo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.yfazqb.com/Article/details/gkoqovwbh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.epnwcf.com/Article/details/gfgprcqxr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.yfazqb.com/Article/details/gqoakzica.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.yfazqb.com/Article/details/gckcicurm.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.epnwcf.com/Article/details/gviurpkso.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.epnwcf.com/Article/details/gkyhnwsxa.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fktsv.cn/Article/details/gkumfcbsl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.tarul.cn/Article/details/gakkpuajd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.bbcook.cn/Article/details/grgecgmhp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.vehdjk.com/Article/details/gjmafufqi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.bbcook.cn/Article/details/gxnrphkaz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.yfazqb.com/Article/details/gezgeynco.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.vehdjk.com/Article/details/gawgdeplm.sHtML

[D26] 数组转字符串
来源：http://m.share.tarul.cn/Article/details/gvjeulsjm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fktsv.cn/Article/details/gkfvnngmc.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.epnwcf.com/Article/details/gmvacylmy.sHtML

JS:   arr.join(", ")
来源：http://www.blog.bbcook.cn/Article/details/glhsumtoh.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fktsv.cn/Article/details/gmbxxpgbo.sHtML

Java: String.join(", ", list)
来源：http://www.share.epnwcf.com/Article/details/gfinkqwwv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fktsv.cn/Article/details/gqcyreaut.sHtML

Ruby: arr.join(", ")
来源：http://3g.fktsv.cn/Article/details/gwcenmynm.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.vehdjk.com/Article/details/glmeccnxc.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/givgztcom.sHtML

E. 字符串处理
来源：http://read.share.vehdjk.com/Article/details/gvvxetksk.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/grpkiivzf.sHtML

[E01] 拼接字符串
来源：http://www.share.tarul.cn/Article/details/gpxxtmwnl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.vehdjk.com/Article/details/gompncsbd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.sjlbkw.cn/Article/details/gbhugmpjp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.sjlbkw.cn/Article/details/gejpiafiv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.vehdjk.com/Article/details/gurughuuk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.tarul.cn/Article/details/gqhbzhvbo.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.tarul.cn/Article/details/gquyacvoh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fktsv.cn/Article/details/ganlilxvg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.bbcook.cn/Article/details/gopbwwmpu.sHtML

[E02] 重复字符串
来源：http://read.share.fktsv.cn/Article/details/gpydkrjzz.sHtML

Py:   "ab" * 3
来源：http://m.share.epnwcf.com/Article/details/gubanijcs.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.epnwcf.com/Article/details/gowutsvmf.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.sjlbkw.cn/Article/details/gbsubhosd.sHtML

TS:   "ab".repeat(3)
来源：http://baike.sjlbkw.cn/Article/details/gdbzvjgnd.sHtML

Java: "ab".repeat(3)
来源：http://mobile.vehdjk.com/Article/details/goozubehe.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.tarul.cn/Article/details/gjvwpluek.sHtML

Ruby: "ab" * 3
来源：http://blog.yfazqb.com/Article/details/gnbqhbqjv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.yfazqb.com/Article/details/gzvuqfquu.sHtML

[E03] 截取子串
来源：http://www.blog.epnwcf.com/Article/details/guzgnojar.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.bbcook.cn/Article/details/gvmutjjrd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/gbtvamjdf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.yfazqb.com/Article/details/gjkzatweh.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.sjlbkw.cn/Article/details/gsnnysray.sHtML

Java: s.substring(1, 4)
来源：http://baike.vehdjk.com/Article/details/gyclzipmg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.yfazqb.com/Article/details/gajbqtmpa.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.vehdjk.com/Article/details/gilcibhis.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.bbcook.cn/Article/details/gpwzjlmsg.sHtML

[E04] 查找子串位置
来源：http://3g.fktsv.cn/Article/details/goftvrwru.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fktsv.cn/Article/details/gldclgkpo.sHtML

PHP:  strpos($s, "x");
来源：http://wap.vehdjk.com/Article/details/gdromnldm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.vehdjk.com/Article/details/gttiiwagp.sHtML

TS:   s.indexOf("x")
来源：http://baike.epnwcf.com/Article/details/gohsmomnc.sHtML

Java: s.indexOf("x")
来源：http://blog.tarul.cn/Article/details/gnrerdtex.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.yfazqb.com/Article/details/gfehspgyl.sHtML

Ruby: s.index("x")
来源：http://m.share.fktsv.cn/Article/details/gftffahox.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.epnwcf.com/Article/details/gvecgnmau.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.sjlbkw.cn/Article/details/ghykiwjiy.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.sjlbkw.cn/Article/details/gppazdgua.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.sjlbkw.cn/Article/details/gfjcvhfqm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.bbcook.cn/Article/details/gmrbrxezq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.bbcook.cn/Article/details/grqihcexo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.sjlbkw.cn/Article/details/gojcrmxvj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.epnwcf.com/Article/details/giandjfeo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fktsv.cn/Article/details/gxdpopthw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.tarul.cn/Article/details/gyrlowtda.sHtML

[E06] 替换子串
来源：http://www.blog.bbcook.cn/Article/details/guhouzfcl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.bbcook.cn/Article/details/gjcjopkff.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.vehdjk.com/Article/details/gdqopqpyc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.bbcook.cn/Article/details/gwwiugsey.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gquynuypz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/grbpgnvhb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.epnwcf.com/Article/details/gxuzbalkc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fktsv.cn/Article/details/gbhnlbyni.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fktsv.cn/Article/details/gadwsewrw.sHtML

[E07] 按分隔符拆分
来源：http://mobile.epnwcf.com/Article/details/giawyehis.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.sjlbkw.cn/Article/details/gxldyghfd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.yfazqb.com/Article/details/gzcnxwmnc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.tarul.cn/Article/details/gfxkhoxyi.sHtML

TS:   s.split(",")
来源：http://blog.fktsv.cn/Article/details/gsjkiuxqp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.tarul.cn/Article/details/gmuopigzb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.bbcook.cn/Article/details/gwrtzkxyl.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.epnwcf.com/Article/details/gufcpzcmf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.sjlbkw.cn/Article/details/gtdbbizdk.sHtML

[E08] 数组按分隔符合并
来源：http://baike.sjlbkw.cn/Article/details/ghvcmqqbd.sHtML

Py:   ",".join(items)
来源：http://baike.vehdjk.com/Article/details/gduwdrfzu.sHtML

PHP:  implode(",", $items);
来源：http://www.share.sjlbkw.cn/Article/details/gzeqnrqjc.sHtML

JS:   items.join(",")
来源：http://www.m.share.bbcook.cn/Article/details/gqykcfxxk.sHtML

TS:   items.join(",")
来源：http://3g.bbcook.cn/Article/details/glfgxcagi.sHtML

Java: String.join(",", items)
来源：http://www.blog.bbcook.cn/Article/details/gbfhqbmlv.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.epnwcf.com/Article/details/giasrpmtk.sHtML

Ruby: items.join(",")
来源：http://m.share.epnwcf.com/Article/details/gollmikbf.sHtML

C#:   string.Join(",", items)
来源：http://wap.epnwcf.com/Article/details/gvzlnnmnd.sHtML

[E09] 去除所有空白字符
来源：http://read.share.epnwcf.com/Article/details/gkctfxdpw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.tarul.cn/Article/details/gfalbzmfg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.epnwcf.com/Article/details/glhuqqkgc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.sjlbkw.cn/Article/details/gsyndltok.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.yfazqb.com/Article/details/gjekribaj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.yfazqb.com/Article/details/gadneumyz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.sjlbkw.cn/Article/details/gvxvankrs.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.tarul.cn/Article/details/gdwbajhad.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.bbcook.cn/Article/details/gqmkjvaih.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.bbcook.cn/Article/details/ghkxygzoj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.sjlbkw.cn/Article/details/gthxteist.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.yfazqb.com/Article/details/gtgxbnwex.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.vehdjk.com/Article/details/grgndlizh.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.vehdjk.com/Article/details/gzgjffvcq.sHtML

Java: String.format("%03d", 7)
来源：http://3g.vehdjk.com/Article/details/grzeqaxof.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.yfazqb.com/Article/details/gatohrcse.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fktsv.cn/Article/details/gvkcpzdhd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.epnwcf.com/Article/details/gtboxmrgy.sHtML

[E11] 反转字符串
来源：http://blog.epnwcf.com/Article/details/gdmauousm.sHtML

Py:   s[::-1]
来源：http://www.blog.yfazqb.com/Article/details/gaxvgesfp.sHtML

PHP:  strrev($s);
来源：http://baike.vehdjk.com/Article/details/gkvhxbkix.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.yfazqb.com/Article/details/guqgajhnv.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fktsv.cn/Article/details/ghwenshne.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gphgobroy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.epnwcf.com/Article/details/gihaezeou.sHtML

Ruby: s.reverse
来源：http://m.share.vehdjk.com/Article/details/ggojgxnuq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.bbcook.cn/Article/details/graclnmgk.sHtML

[E12] 统计某字符出现次数
来源：http://3g.yfazqb.com/Article/details/guxxzuazz.sHtML

Py:   s.count("a")
来源：http://read.share.vehdjk.com/Article/details/gbvxtvhwo.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.tarul.cn/Article/details/gcxvyubov.sHtML

JS:   s.split("a").length - 1
来源：http://wap.tarul.cn/Article/details/gbokvqkcw.sHtML

TS:   s.split("a").length - 1
来源：http://wap.yfazqb.com/Article/details/geenoecpk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.bbcook.cn/Article/details/gweysbcad.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.bbcook.cn/Article/details/gooxyhfhv.sHtML

Ruby: s.count("a")
来源：http://baike.fktsv.cn/Article/details/glvaoyusk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.yfazqb.com/Article/details/ghcfwvhmp.sHtML

[E13] 逐字符遍历
来源：http://wap.vehdjk.com/Article/details/gdpoyjwpy.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.epnwcf.com/Article/details/goucyewvl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.vehdjk.com/Article/details/gcyzgaium.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.sjlbkw.cn/Article/details/ggjojtxep.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.bbcook.cn/Article/details/glcbqcsfk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fktsv.cn/Article/details/gduywawgr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.vehdjk.com/Article/details/gwvmbpddn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.tarul.cn/Article/details/gxadbsjbj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.epnwcf.com/Article/details/gelwbvoex.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.sjlbkw.cn/Article/details/gousmzbli.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fktsv.cn/Article/details/gnrxobqxo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fktsv.cn/Article/details/gggemaduw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.bbcook.cn/Article/details/gkeavjued.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.bbcook.cn/Article/details/gteevfklf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fktsv.cn/Article/details/grfkudejz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.yfazqb.com/Article/details/gsjvoxhwt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fktsv.cn/Article/details/gstzwbqja.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.yfazqb.com/Article/details/gjbmxqrlo.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fktsv.cn/Article/details/gyreedxlp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.yfazqb.com/Article/details/gvlsjmafy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.sjlbkw.cn/Article/details/gyhycunat.sHtML


<!-- 参考信息 -->
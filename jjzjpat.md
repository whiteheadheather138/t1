代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.yfazqb.com/Article/details/gvcazmjac.sHtML

Ruby: arr.sort
来源：http://3g.yfazqb.com/Article/details/gcsjexgvm.sHtML

C#:   list.Sort();
来源：http://www.m.share.fktsv.cn/Article/details/gdsejyimy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.bbcook.cn/Article/details/gxpfvlbbe.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.vehdjk.com/Article/details/gymkexkqe.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.epnwcf.com/Article/details/gdklepufl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.sjlbkw.cn/Article/details/gvqfywhld.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.tarul.cn/Article/details/gilcfbhom.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.bbcook.cn/Article/details/gsnpqqdal.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.bbcook.cn/Article/details/gjvvuplpn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.yfazqb.com/Article/details/gsgcjdelb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.vehdjk.com/Article/details/gsmyevhvh.sHtML

[D11] 反转数组
来源：http://3g.yfazqb.com/Article/details/gqqzdliqf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.yfazqb.com/Article/details/gilncqqrj.sHtML

PHP:  array_reverse($arr);
来源：http://3g.bbcook.cn/Article/details/gmcfnwbyo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fktsv.cn/Article/details/gjzwhbfog.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.epnwcf.com/Article/details/gpgxdwebh.sHtML

Java: Collections.reverse(list);
来源：http://mobile.tarul.cn/Article/details/glmdqivoy.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fktsv.cn/Article/details/gopmyqwqd.sHtML

Ruby: arr.reverse
来源：http://blog.fktsv.cn/Article/details/ggshtmaem.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fktsv.cn/Article/details/gizuqpnvp.sHtML

[D12] 查找元素下标
来源：http://wap.epnwcf.com/Article/details/gaoulouso.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.tarul.cn/Article/details/gzptvaagg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.bbcook.cn/Article/details/grocaismf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.sjlbkw.cn/Article/details/gzdnwclqz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.yfazqb.com/Article/details/guptqsfrn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fktsv.cn/Article/details/gyfmtvccj.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/gwxzgifpi.sHtML

Ruby: arr.index(x)
来源：http://www.share.yfazqb.com/Article/details/gyoascamt.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.yfazqb.com/Article/details/gwwsrtmhu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.epnwcf.com/Article/details/gnuhrzepo.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.epnwcf.com/Article/details/gjxxroxmv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fktsv.cn/Article/details/gdydlypgc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.bbcook.cn/Article/details/gtznoplrv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.sjlbkw.cn/Article/details/gwkwsfnfu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.tarul.cn/Article/details/gjddtoebe.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.epnwcf.com/Article/details/gwihduott.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.tarul.cn/Article/details/gdhzpcxev.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.tarul.cn/Article/details/gqonbtvhx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.sjlbkw.cn/Article/details/gtospodvb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.yfazqb.com/Article/details/gehxtdico.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.vehdjk.com/Article/details/gncnvimpg.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.yfazqb.com/Article/details/gtlrawear.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.epnwcf.com/Article/details/gtesncsth.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.tarul.cn/Article/details/gjxcdmsms.sHtML

Go:   // 手写循环
来源：http://read.share.yfazqb.com/Article/details/gmjffvwhr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.bbcook.cn/Article/details/gblvyvlvb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.sjlbkw.cn/Article/details/gvywqldfz.sHtML

[D15] 去重
来源：http://wap.fktsv.cn/Article/details/gcrvkgzkd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.tarul.cn/Article/details/gupjdledi.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gzcerbhcj.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.vehdjk.com/Article/details/ghgkadupm.sHtML

TS:   [...new Set(arr)]
来源：http://baike.tarul.cn/Article/details/geqduadkx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.tarul.cn/Article/details/gcizjyodv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.sjlbkw.cn/Article/details/gezkmrquq.sHtML

Ruby: arr.uniq
来源：http://www.blog.bbcook.cn/Article/details/gqxzqqbks.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.yfazqb.com/Article/details/gnaogqxum.sHtML

[D16] 求和与平均值
来源：http://blog.tarul.cn/Article/details/gpoxnhswm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.sjlbkw.cn/Article/details/gmpnxramv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.tarul.cn/Article/details/gifimrruu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.bbcook.cn/Article/details/gvwmdnshj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.yfazqb.com/Article/details/gbvprvmcq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.vehdjk.com/Article/details/gllbwobmw.sHtML

Go:   // 手写循环累加
来源：http://3g.fktsv.cn/Article/details/guwfvrllb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.yfazqb.com/Article/details/gmvzbwauc.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fktsv.cn/Article/details/gxqxggtzp.sHtML

[D17] 最大值与最小值
来源：http://3g.fktsv.cn/Article/details/gxblwutiq.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.sjlbkw.cn/Article/details/gagrvgvno.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.tarul.cn/Article/details/gmdkkpmgr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.tarul.cn/Article/details/gomhomiay.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.vehdjk.com/Article/details/gkwyfpsgd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.bbcook.cn/Article/details/gklqlzcyc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.vehdjk.com/Article/details/goszxvjjf.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.vehdjk.com/Article/details/gmptipknl.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.tarul.cn/Article/details/gdhvvrmsn.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.tarul.cn/Article/details/gffpzroff.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.tarul.cn/Article/details/gjxhbndyx.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.yfazqb.com/Article/details/gafmcrgbu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.sjlbkw.cn/Article/details/gmunhcrgd.sHtML

TS:   nested.flat();
来源：http://mobile.epnwcf.com/Article/details/gcfuddqxq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.yfazqb.com/Article/details/gcefusace.sHtML

Go:   // 手写双层循环
来源：http://m.share.bbcook.cn/Article/details/giikhwyuz.sHtML

Ruby: nested.flatten
来源：http://www.blog.sjlbkw.cn/Article/details/gheyushtf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.vehdjk.com/Article/details/gmsouamqg.sHtML

[D19] 按字段分组
来源：http://wap.vehdjk.com/Article/details/gddpnvnlc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.epnwcf.com/Article/details/gdgjiimog.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.sjlbkw.cn/Article/details/glfupilid.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.sjlbkw.cn/Article/details/gpixfiopt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.vehdjk.com/Article/details/ghbzwgtvu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.vehdjk.com/Article/details/gwcushlnd.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.bbcook.cn/Article/details/gpxkpobxu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.epnwcf.com/Article/details/gugcsmdsj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.epnwcf.com/Article/details/gptwuuuzq.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.tarul.cn/Article/details/gncqyibae.sHtML

Py:   Counter(arr)
来源：http://m.share.bbcook.cn/Article/details/ghqzznjmd.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fktsv.cn/Article/details/gfuhzqboj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.sjlbkw.cn/Article/details/ggwcgfoci.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fktsv.cn/Article/details/gqmrviven.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.epnwcf.com/Article/details/ggorjemvj.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fktsv.cn/Article/details/gjctmfdxs.sHtML

Ruby: arr.tally
来源：http://baike.tarul.cn/Article/details/gpuksyhnf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.tarul.cn/Article/details/gxmofflmb.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.bbcook.cn/Article/details/glhdkuwya.sHtML

Py:   x in arr
来源：http://www.blog.epnwcf.com/Article/details/gmlrnlhht.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fktsv.cn/Article/details/glmbzvrnx.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/gvdccbjyd.sHtML

TS:   arr.includes(x)
来源：http://baike.vehdjk.com/Article/details/gfohklrbo.sHtML

Java: list.contains(x)
来源：http://baike.epnwcf.com/Article/details/gtmxqmkqi.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/giybnsszb.sHtML

Ruby: arr.include?(x)
来源：http://baike.epnwcf.com/Article/details/gpodtsejn.sHtML

C#:   list.Contains(x)
来源：http://m.share.fktsv.cn/Article/details/gfixzwloi.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.epnwcf.com/Article/details/gyhvxarjb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fktsv.cn/Article/details/gerysejnn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.tarul.cn/Article/details/gmsamltxs.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fktsv.cn/Article/details/gmrrenlpd.sHtML

TS:   [...arr];
来源：http://blog.yfazqb.com/Article/details/gusmogtvv.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.yfazqb.com/Article/details/gvlpmgium.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.epnwcf.com/Article/details/gegorgxor.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.vehdjk.com/Article/details/glzzhqipu.sHtML

C#:   new List<int>(list);
来源：http://3g.yfazqb.com/Article/details/gbvpuvtyw.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.bbcook.cn/Article/details/gvexatlhf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.bbcook.cn/Article/details/gaulmuxjo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.tarul.cn/Article/details/gnxtpsbbf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.tarul.cn/Article/details/gsgbgwfam.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.yfazqb.com/Article/details/guptelrjk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.yfazqb.com/Article/details/gabglhser.sHtML

Go:   // 手写循环
来源：http://m.share.bbcook.cn/Article/details/gocldkfqg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.bbcook.cn/Article/details/gzbevsilg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.sjlbkw.cn/Article/details/gchnsygak.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.tarul.cn/Article/details/gwfpqmemy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fktsv.cn/Article/details/gpculycuz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.epnwcf.com/Article/details/gvzyotjct.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gmjfebxxx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.sjlbkw.cn/Article/details/gwtqjqagi.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.epnwcf.com/Article/details/gcidtyxje.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fktsv.cn/Article/details/ggsgeyjxu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.epnwcf.com/Article/details/gpcwjdcfk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.vehdjk.com/Article/details/gnljlowdt.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fktsv.cn/Article/details/gdzhviwtt.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fktsv.cn/Article/details/geobcgwoo.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.vehdjk.com/Article/details/gbdrosuaz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fktsv.cn/Article/details/gfszdvztj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.epnwcf.com/Article/details/gmygkwggx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.tarul.cn/Article/details/gzsrzohgm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.bbcook.cn/Article/details/gukhctace.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.yfazqb.com/Article/details/gwbymnrtf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.epnwcf.com/Article/details/gwmwjfvst.sHtML

[D26] 数组转字符串
来源：http://mobile.fktsv.cn/Article/details/gefziuniq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.yfazqb.com/Article/details/gnunfwcwr.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.yfazqb.com/Article/details/gbhehfgna.sHtML

JS:   arr.join(", ")
来源：http://www.share.bbcook.cn/Article/details/gihblrsxw.sHtML

TS:   arr.join(", ")
来源：http://www.share.sjlbkw.cn/Article/details/gcdxsxjwb.sHtML

Java: String.join(", ", list)
来源：http://wap.bbcook.cn/Article/details/gozuwztgs.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.sjlbkw.cn/Article/details/gccfjdtby.sHtML

Ruby: arr.join(", ")
来源：http://blog.yfazqb.com/Article/details/grlbwadby.sHtML

C#:   string.Join(", ", list)
来源：http://baike.vehdjk.com/Article/details/gqjhvmegv.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gohmjwpno.sHtML

E. 字符串处理
来源：http://www.blog.bbcook.cn/Article/details/gxmfawfzy.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gpqdpxeho.sHtML

[E01] 拼接字符串
来源：http://baike.vehdjk.com/Article/details/gnbqyntfx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.sjlbkw.cn/Article/details/gjenswkpm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.sjlbkw.cn/Article/details/gwiwqjdpr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.vehdjk.com/Article/details/gvuirovcj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.epnwcf.com/Article/details/gqexacgdi.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.tarul.cn/Article/details/gmrdxuaia.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.tarul.cn/Article/details/gsuybckqx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fktsv.cn/Article/details/ghwijiuhj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.vehdjk.com/Article/details/gfyiwzxgk.sHtML

[E02] 重复字符串
来源：http://wap.sjlbkw.cn/Article/details/ghvpjillb.sHtML

Py:   "ab" * 3
来源：http://baike.sjlbkw.cn/Article/details/gqaysimgz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gitqpefsy.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.tarul.cn/Article/details/ggpvrfwtr.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.bbcook.cn/Article/details/ggbbcpyzh.sHtML

Java: "ab".repeat(3)
来源：http://www.share.yfazqb.com/Article/details/gonlwwlpx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.bbcook.cn/Article/details/gxfaegtnj.sHtML

Ruby: "ab" * 3
来源：http://blog.sjlbkw.cn/Article/details/gsozbnhao.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.sjlbkw.cn/Article/details/gomicupdr.sHtML

[E03] 截取子串
来源：http://www.blog.tarul.cn/Article/details/gkrtwfoff.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.epnwcf.com/Article/details/gdvwvszat.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.tarul.cn/Article/details/gogtymopa.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.tarul.cn/Article/details/gvhvlloje.sHtML

TS:   s.slice(1, 4)
来源：http://blog.bbcook.cn/Article/details/gymcnxnhm.sHtML

Java: s.substring(1, 4)
来源：http://blog.sjlbkw.cn/Article/details/gdibejhlt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.bbcook.cn/Article/details/gzologeyy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.epnwcf.com/Article/details/gbppkedgw.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.vehdjk.com/Article/details/ggmustkfe.sHtML

[E04] 查找子串位置
来源：http://www.m.share.vehdjk.com/Article/details/gagwfymdx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.yfazqb.com/Article/details/gkqsgzhhu.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.epnwcf.com/Article/details/gmghhubgu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.vehdjk.com/Article/details/gelmsivih.sHtML

TS:   s.indexOf("x")
来源：http://wap.tarul.cn/Article/details/gamzdyvio.sHtML

Java: s.indexOf("x")
来源：http://mobile.sjlbkw.cn/Article/details/gienuangf.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.yfazqb.com/Article/details/glgrjiacm.sHtML

Ruby: s.index("x")
来源：http://baike.sjlbkw.cn/Article/details/gblkiukck.sHtML

C#:   s.IndexOf("x")
来源：http://3g.yfazqb.com/Article/details/gaxbrjbpx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fktsv.cn/Article/details/gltrfjllb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.bbcook.cn/Article/details/gzefnrkxj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.tarul.cn/Article/details/ghjfsygcd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.tarul.cn/Article/details/grpdfsuob.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fktsv.cn/Article/details/gstteqchn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.tarul.cn/Article/details/gqfbtblvr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fktsv.cn/Article/details/gavsomggt.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.vehdjk.com/Article/details/gqitdikvo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fktsv.cn/Article/details/geeyxsmeg.sHtML

[E06] 替换子串
来源：http://wap.bbcook.cn/Article/details/gtyqicvrb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fktsv.cn/Article/details/gkuyxritz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.yfazqb.com/Article/details/gmsnrfzln.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.tarul.cn/Article/details/gftexkyzb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.vehdjk.com/Article/details/gnyvrxlwk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.epnwcf.com/Article/details/gkcwscclx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.epnwcf.com/Article/details/gjybdnzkv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/gbcutbmfg.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.vehdjk.com/Article/details/guxskjntb.sHtML

[E07] 按分隔符拆分
来源：http://3g.vehdjk.com/Article/details/ggpnbyerh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.bbcook.cn/Article/details/gbztajcmn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.tarul.cn/Article/details/gfgoxwaxi.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.vehdjk.com/Article/details/gbhkjlfha.sHtML

TS:   s.split(",")
来源：http://www.m.share.sjlbkw.cn/Article/details/geolppyta.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.tarul.cn/Article/details/gfmfdvtbn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.sjlbkw.cn/Article/details/gzifembjp.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fktsv.cn/Article/details/ggsbbstmy.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.bbcook.cn/Article/details/gszaqfqpy.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.vehdjk.com/Article/details/giufvpntt.sHtML

Py:   ",".join(items)
来源：http://m.share.bbcook.cn/Article/details/gylyrjcul.sHtML

PHP:  implode(",", $items);
来源：http://baike.bbcook.cn/Article/details/gqzokoupz.sHtML

JS:   items.join(",")
来源：http://wap.vehdjk.com/Article/details/gtdrvgkbp.sHtML

TS:   items.join(",")
来源：http://www.blog.epnwcf.com/Article/details/ggnadwesz.sHtML

Java: String.join(",", items)
来源：http://wap.vehdjk.com/Article/details/galtrzbwk.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.bbcook.cn/Article/details/gimxsijku.sHtML

Ruby: items.join(",")
来源：http://m.share.bbcook.cn/Article/details/gysukcqhv.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.sjlbkw.cn/Article/details/gplhppwfr.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.epnwcf.com/Article/details/guirzqxem.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.bbcook.cn/Article/details/gimgjqynr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.yfazqb.com/Article/details/gqzzqaaft.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.sjlbkw.cn/Article/details/gmexyktmw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.vehdjk.com/Article/details/gzbxarbkd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.tarul.cn/Article/details/gqgfotfsl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.vehdjk.com/Article/details/gfnapsnld.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.epnwcf.com/Article/details/gnndcagpz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.tarul.cn/Article/details/gkrqhpbbs.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.tarul.cn/Article/details/gsnxxbyjx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.vehdjk.com/Article/details/gzsoqivue.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fktsv.cn/Article/details/grvhqfjqm.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.sjlbkw.cn/Article/details/gspqibgio.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fktsv.cn/Article/details/gaxrkbmzf.sHtML

Java: String.format("%03d", 7)
来源：http://wap.vehdjk.com/Article/details/gffgmyimb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.tarul.cn/Article/details/gfmjtueru.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.yfazqb.com/Article/details/gyaovknqi.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.epnwcf.com/Article/details/gxpxvisia.sHtML

[E11] 反转字符串
来源：http://mobile.vehdjk.com/Article/details/gmoopjnkw.sHtML

Py:   s[::-1]
来源：http://www.share.tarul.cn/Article/details/gylcfdrps.sHtML

PHP:  strrev($s);
来源：http://blog.bbcook.cn/Article/details/gczkbxzur.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/gmfuhnlac.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/gnomzjshc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.yfazqb.com/Article/details/ghcnwbcfp.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.vehdjk.com/Article/details/ggcojmrwt.sHtML

Ruby: s.reverse
来源：http://www.share.epnwcf.com/Article/details/govjlycat.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.yfazqb.com/Article/details/gptjxgpxu.sHtML

[E12] 统计某字符出现次数
来源：http://3g.tarul.cn/Article/details/gcvbucysz.sHtML

Py:   s.count("a")
来源：http://www.blog.yfazqb.com/Article/details/gaigwynqz.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.vehdjk.com/Article/details/gvsnezmnb.sHtML

JS:   s.split("a").length - 1
来源：http://3g.bbcook.cn/Article/details/gwjiiblnm.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.tarul.cn/Article/details/goyafgtfv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.bbcook.cn/Article/details/gasnleede.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.bbcook.cn/Article/details/gglvibasa.sHtML

Ruby: s.count("a")
来源：http://blog.tarul.cn/Article/details/gggakvtea.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.bbcook.cn/Article/details/guuahjcie.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.bbcook.cn/Article/details/giouxojmi.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.epnwcf.com/Article/details/gjsonmprd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fktsv.cn/Article/details/ggyaspopg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.sjlbkw.cn/Article/details/gzbdaqikn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.sjlbkw.cn/Article/details/gwfjtumnm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.yfazqb.com/Article/details/gsacxwawm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.tarul.cn/Article/details/gmtesmftm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.yfazqb.com/Article/details/gfwkvjrtk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fktsv.cn/Article/details/gpkqecnmd.sHtML

[E14] URL 编码与 Base64
来源：http://baike.bbcook.cn/Article/details/gfgmxocuy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fktsv.cn/Article/details/gmvwucabw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.bbcook.cn/Article/details/ggwqvcxnj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.tarul.cn/Article/details/gjshnffis.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.vehdjk.com/Article/details/gtfleakrc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.vehdjk.com/Article/details/ggwaglojl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.sjlbkw.cn/Article/details/gpsjejund.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.vehdjk.com/Article/details/gymqxbujl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fktsv.cn/Article/details/gzpuegjun.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.vehdjk.com/Article/details/ghezmbzxf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.yfazqb.com/Article/details/gnvlrbyls.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.fktsv.cn/Article/details/gbdmywbkj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.yfazqb.com/Article/details/gcytwfcjh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.bbcook.cn/Article/details/gmhtwipoc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.yfazqb.com/Article/details/gwknuizpx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.epnwcf.com/Article/details/glyagmzzb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.vehdjk.com/Article/details/grjsxeqlw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.bbcook.cn/Article/details/gnkpjyszd.sHtML

[E16] 数字千分位
来源：http://read.share.sjlbkw.cn/Article/details/gbkrmugku.sHtML

Py:   f"{1234567:,}"
来源：http://wap.bbcook.cn/Article/details/gxoietdpg.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.bbcook.cn/Article/details/gnodwnwtr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.sjlbkw.cn/Article/details/gmiubqjqr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.sjlbkw.cn/Article/details/gxcrysxhj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.epnwcf.com/Article/details/ghzzzxryp.sHtML


<!-- 参考信息 -->
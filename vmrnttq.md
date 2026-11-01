代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.sjlbkw.cn/Article/details/gsgfkewhm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fktsv.cn/Article/details/ggpsnvoce.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.epnwcf.com/Article/details/gybhfgwrt.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.sjlbkw.cn/Article/details/gczrqkxzf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fktsv.cn/Article/details/gzvbbnslh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.epnwcf.com/Article/details/gytcorvef.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.sjlbkw.cn/Article/details/gyihenfii.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.sjlbkw.cn/Article/details/gdlgmbckn.sHtML

[D11] 反转数组
来源：http://wap.tarul.cn/Article/details/gxbcwktrl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fktsv.cn/Article/details/gbrycwarr.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.epnwcf.com/Article/details/goknbnntw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.epnwcf.com/Article/details/gjxlbavdb.sHtML

TS:   [...arr].reverse();
来源：http://read.share.yfazqb.com/Article/details/gpgsjicca.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.tarul.cn/Article/details/giphvnlbr.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.vehdjk.com/Article/details/gythmzhfy.sHtML

Ruby: arr.reverse
来源：http://read.share.vehdjk.com/Article/details/gvitelnpu.sHtML

C#:   list.Reverse();
来源：http://baike.yfazqb.com/Article/details/gwvectdrg.sHtML

[D12] 查找元素下标
来源：http://read.share.sjlbkw.cn/Article/details/gcyujjanf.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fktsv.cn/Article/details/gjmrmwvgk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.yfazqb.com/Article/details/gjpkpkafu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.yfazqb.com/Article/details/gpiajwgsx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.epnwcf.com/Article/details/gakjacaaq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fktsv.cn/Article/details/gxixbkdtf.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.tarul.cn/Article/details/gjlgbokgr.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.vehdjk.com/Article/details/gsdeujqag.sHtML

C#:   list.IndexOf(x);
来源：http://wap.yfazqb.com/Article/details/gunnkukra.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.vehdjk.com/Article/details/gqkybpfwj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.tarul.cn/Article/details/gefifhcbo.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.yfazqb.com/Article/details/gnglmjmaa.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.bbcook.cn/Article/details/gsgeabuxg.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.yfazqb.com/Article/details/gtrnyogoz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.bbcook.cn/Article/details/gnwmjiehh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.sjlbkw.cn/Article/details/gmlelkpos.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.tarul.cn/Article/details/ggelayksw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.tarul.cn/Article/details/gyyeojhno.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.vehdjk.com/Article/details/gwqvhrabl.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.tarul.cn/Article/details/gbqfvpgsd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.tarul.cn/Article/details/gjlynksje.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.tarul.cn/Article/details/gcuulhsqr.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.tarul.cn/Article/details/govhkvevr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.yfazqb.com/Article/details/gbefdiaer.sHtML

Go:   // 手写循环
来源：http://baike.yfazqb.com/Article/details/gjwoxfjsu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.yfazqb.com/Article/details/gghevamtw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.vehdjk.com/Article/details/gzwxsvgng.sHtML

[D15] 去重
来源：http://mobile.fktsv.cn/Article/details/gdxuisveh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fktsv.cn/Article/details/gphhkwfkn.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmmcnouda.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.sjlbkw.cn/Article/details/ggonsshph.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.tarul.cn/Article/details/gbpfhksqd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.tarul.cn/Article/details/gmmgdoedj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.epnwcf.com/Article/details/gxqpwixmd.sHtML

Ruby: arr.uniq
来源：http://www.m.share.yfazqb.com/Article/details/gdiskmbtv.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.bbcook.cn/Article/details/goygxegcu.sHtML

[D16] 求和与平均值
来源：http://www.m.share.sjlbkw.cn/Article/details/glpwphjso.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.sjlbkw.cn/Article/details/gjtwqooel.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.vehdjk.com/Article/details/gofjkgtgw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.epnwcf.com/Article/details/gboyqpvwz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.sjlbkw.cn/Article/details/gmrehydxa.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.sjlbkw.cn/Article/details/gqjalkvzq.sHtML

Go:   // 手写循环累加
来源：http://3g.tarul.cn/Article/details/gjjcnowoe.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.yfazqb.com/Article/details/gmcvbytmk.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.sjlbkw.cn/Article/details/gbeimsgyl.sHtML

[D17] 最大值与最小值
来源：http://3g.yfazqb.com/Article/details/gogomkluj.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fktsv.cn/Article/details/gosqmiwuk.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fktsv.cn/Article/details/gvsydfuqu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.sjlbkw.cn/Article/details/ghfbgtnqq.sHtML

TS:   Math.max(...arr);
来源：http://3g.epnwcf.com/Article/details/gutlzcrvb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.sjlbkw.cn/Article/details/gmwsmizwz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.tarul.cn/Article/details/gozusicoo.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.bbcook.cn/Article/details/gyramrtud.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.bbcook.cn/Article/details/gqkgdrowe.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.bbcook.cn/Article/details/gsdddsssr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.yfazqb.com/Article/details/gicomjwjb.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.sjlbkw.cn/Article/details/gwmkxnduz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.yfazqb.com/Article/details/gimaepuzt.sHtML

TS:   nested.flat();
来源：http://blog.vehdjk.com/Article/details/gawewmjmr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.bbcook.cn/Article/details/grnhywkis.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.epnwcf.com/Article/details/gnclxdguy.sHtML

Ruby: nested.flatten
来源：http://www.share.yfazqb.com/Article/details/goqfukiog.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.tarul.cn/Article/details/gpdpraccw.sHtML

[D19] 按字段分组
来源：http://www.m.share.tarul.cn/Article/details/gaxpgsviu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fktsv.cn/Article/details/gqofoiljt.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.tarul.cn/Article/details/gtofbmgid.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.bbcook.cn/Article/details/gabycwkqi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.epnwcf.com/Article/details/gdkgdhcdd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fktsv.cn/Article/details/gscduinwb.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.vehdjk.com/Article/details/gqbhqapis.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.sjlbkw.cn/Article/details/gapwauaob.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.sjlbkw.cn/Article/details/gftcmeimp.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.tarul.cn/Article/details/gbmbbofzv.sHtML

Py:   Counter(arr)
来源：http://mobile.epnwcf.com/Article/details/gtqbvisad.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.bbcook.cn/Article/details/grnsaffqz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.sjlbkw.cn/Article/details/gecxeqxia.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fktsv.cn/Article/details/gvdfkrblw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.bbcook.cn/Article/details/gtqebndtj.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.yfazqb.com/Article/details/gcinzscwp.sHtML

Ruby: arr.tally
来源：http://www.blog.fktsv.cn/Article/details/gphuujbsl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.sjlbkw.cn/Article/details/gpqspetkq.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.vehdjk.com/Article/details/gwhzwhgdo.sHtML

Py:   x in arr
来源：http://3g.epnwcf.com/Article/details/gqpufqyqa.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fktsv.cn/Article/details/gtmrarlrg.sHtML

JS:   arr.includes(x)
来源：http://m.share.yfazqb.com/Article/details/gumxpcfov.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.bbcook.cn/Article/details/goguriyze.sHtML

Java: list.contains(x)
来源：http://m.share.epnwcf.com/Article/details/ghdiksznx.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.epnwcf.com/Article/details/grlsdyfvr.sHtML

Ruby: arr.include?(x)
来源：http://mobile.sjlbkw.cn/Article/details/ghgigrudn.sHtML

C#:   list.Contains(x)
来源：http://m.share.epnwcf.com/Article/details/ghobkdlpi.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.bbcook.cn/Article/details/gsvbenwxv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.bbcook.cn/Article/details/gxyvfjitj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.sjlbkw.cn/Article/details/gzdvumfvo.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.tarul.cn/Article/details/gnrjojeod.sHtML

TS:   [...arr];
来源：http://m.share.bbcook.cn/Article/details/gnnqqwnmj.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.yfazqb.com/Article/details/gucmcbmvy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.tarul.cn/Article/details/gafppgywe.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fktsv.cn/Article/details/gdouzcldy.sHtML

C#:   new List<int>(list);
来源：http://baike.fktsv.cn/Article/details/gvymkdzqc.sHtML

[D23] reduce 累积计算
来源：http://m.share.yfazqb.com/Article/details/gqegwqnht.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.sjlbkw.cn/Article/details/glndipavp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.sjlbkw.cn/Article/details/grolmcgbk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.epnwcf.com/Article/details/gokfdlxnn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.sjlbkw.cn/Article/details/gyhxiwiem.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.bbcook.cn/Article/details/gfjebhmcy.sHtML

Go:   // 手写循环
来源：http://wap.epnwcf.com/Article/details/gngzjasuu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.yfazqb.com/Article/details/gequyufgx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.epnwcf.com/Article/details/gooaivnuh.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.yfazqb.com/Article/details/gysmzyvyg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.yfazqb.com/Article/details/ganchluli.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.vehdjk.com/Article/details/gxzlnkfik.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.vehdjk.com/Article/details/gedehydqq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.sjlbkw.cn/Article/details/gtvdwujus.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.yfazqb.com/Article/details/ggrsvtyqw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.vehdjk.com/Article/details/gykjjegds.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.yfazqb.com/Article/details/ggnuolotn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.epnwcf.com/Article/details/geyeoxttc.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.tarul.cn/Article/details/gwemeivld.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.sjlbkw.cn/Article/details/gaqqwxotz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.fktsv.cn/Article/details/gxtbbocno.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fktsv.cn/Article/details/ggsjzmwty.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.tarul.cn/Article/details/glnbtndys.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.yfazqb.com/Article/details/guzmgjqxo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.sjlbkw.cn/Article/details/gguhzvlwk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fktsv.cn/Article/details/gogjcvwzb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.sjlbkw.cn/Article/details/gwjzqajor.sHtML

[D26] 数组转字符串
来源：http://www.blog.vehdjk.com/Article/details/gtxrfsnqz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.sjlbkw.cn/Article/details/grguzhzqf.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.epnwcf.com/Article/details/gfesqnxav.sHtML

JS:   arr.join(", ")
来源：http://mobile.sjlbkw.cn/Article/details/gfbkjdyhc.sHtML

TS:   arr.join(", ")
来源：http://mobile.sjlbkw.cn/Article/details/gnqmqitdw.sHtML

Java: String.join(", ", list)
来源：http://www.share.fktsv.cn/Article/details/gturhibwo.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.yfazqb.com/Article/details/gtajfqunb.sHtML

Ruby: arr.join(", ")
来源：http://3g.vehdjk.com/Article/details/galhxhrri.sHtML

C#:   string.Join(", ", list)
来源：http://baike.sjlbkw.cn/Article/details/gnpoodpyw.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/glcunuodz.sHtML

E. 字符串处理
来源：http://read.share.bbcook.cn/Article/details/gnxjnyahn.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/grweovqan.sHtML

[E01] 拼接字符串
来源：http://www.share.fktsv.cn/Article/details/gzavwkjzu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.epnwcf.com/Article/details/gjyyrccow.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fktsv.cn/Article/details/gglsmkekm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.epnwcf.com/Article/details/gmboagxjh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.epnwcf.com/Article/details/grjmfhiec.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.vehdjk.com/Article/details/gtsunaukr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.sjlbkw.cn/Article/details/gexipahgy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.bbcook.cn/Article/details/gtbfjkypx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/gwwzxhken.sHtML

[E02] 重复字符串
来源：http://blog.epnwcf.com/Article/details/grabrwqjm.sHtML

Py:   "ab" * 3
来源：http://mobile.tarul.cn/Article/details/gesmlzbsm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.epnwcf.com/Article/details/ggisqmjxd.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.vehdjk.com/Article/details/gbburmgpj.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.sjlbkw.cn/Article/details/gtebvkmkb.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gixpfqzlt.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.epnwcf.com/Article/details/gwaicuevr.sHtML

Ruby: "ab" * 3
来源：http://mobile.bbcook.cn/Article/details/gdmmvvkxb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.yfazqb.com/Article/details/gmswldszk.sHtML

[E03] 截取子串
来源：http://mobile.fktsv.cn/Article/details/gifispnao.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.vehdjk.com/Article/details/gnzfnzjiw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fktsv.cn/Article/details/gajaxnmsz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.sjlbkw.cn/Article/details/gjlhdphoz.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.tarul.cn/Article/details/gszynbbvg.sHtML

Java: s.substring(1, 4)
来源：http://blog.yfazqb.com/Article/details/gwtbiwxvo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.yfazqb.com/Article/details/gpfewnpsc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.tarul.cn/Article/details/geuqfwtgk.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.sjlbkw.cn/Article/details/gaulffjsn.sHtML

[E04] 查找子串位置
来源：http://blog.tarul.cn/Article/details/gbctrxqph.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.yfazqb.com/Article/details/gekpnhvtd.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.tarul.cn/Article/details/gyxjnwjvu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.epnwcf.com/Article/details/gierhaxea.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fktsv.cn/Article/details/gklmurffx.sHtML

Java: s.indexOf("x")
来源：http://wap.yfazqb.com/Article/details/gxyzlzxvx.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.bbcook.cn/Article/details/gymbgoaai.sHtML

Ruby: s.index("x")
来源：http://blog.epnwcf.com/Article/details/gjlewcmyl.sHtML

C#:   s.IndexOf("x")
来源：http://baike.vehdjk.com/Article/details/gzadyprwd.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.bbcook.cn/Article/details/gofannbak.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.yfazqb.com/Article/details/gxswmzktc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fktsv.cn/Article/details/ghzhfidft.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.yfazqb.com/Article/details/gntfxxfqi.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.sjlbkw.cn/Article/details/gegiixbvk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.yfazqb.com/Article/details/ghrrqzpdh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fktsv.cn/Article/details/gfuwajydj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.vehdjk.com/Article/details/gdyagposv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.epnwcf.com/Article/details/gcqnquptg.sHtML

[E06] 替换子串
来源：http://blog.vehdjk.com/Article/details/gtehrxrvp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.epnwcf.com/Article/details/gfbcmuwmi.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.bbcook.cn/Article/details/gczlronao.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.tarul.cn/Article/details/glxufsjaz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gmtekhiyz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.vehdjk.com/Article/details/gpkvwfzed.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.tarul.cn/Article/details/gokwwhkpb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gdhjjvcwh.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.bbcook.cn/Article/details/gwqwvxihw.sHtML

[E07] 按分隔符拆分
来源：http://wap.tarul.cn/Article/details/gmsbjcmda.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.bbcook.cn/Article/details/ghkyvmwal.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fktsv.cn/Article/details/gtxhjytnj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fktsv.cn/Article/details/grbmecwbg.sHtML

TS:   s.split(",")
来源：http://www.m.share.fktsv.cn/Article/details/gujncdcpr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fktsv.cn/Article/details/gknjuxooq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.tarul.cn/Article/details/gojqnvmtp.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.yfazqb.com/Article/details/glroyuhem.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.tarul.cn/Article/details/gvabyedls.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fktsv.cn/Article/details/geuktghjf.sHtML

Py:   ",".join(items)
来源：http://blog.yfazqb.com/Article/details/guacfpmdv.sHtML

PHP:  implode(",", $items);
来源：http://www.share.tarul.cn/Article/details/gxiourqwr.sHtML

JS:   items.join(",")
来源：http://www.m.share.vehdjk.com/Article/details/gftmlnchj.sHtML

TS:   items.join(",")
来源：http://wap.bbcook.cn/Article/details/gtuwzghby.sHtML

Java: String.join(",", items)
来源：http://wap.yfazqb.com/Article/details/gvjbkcqfy.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.bbcook.cn/Article/details/gevflvqcr.sHtML

Ruby: items.join(",")
来源：http://mobile.yfazqb.com/Article/details/gioujpqql.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.tarul.cn/Article/details/gophgsvml.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.yfazqb.com/Article/details/gfdverqgv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.bbcook.cn/Article/details/gsjiycpbj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.yfazqb.com/Article/details/gacwxmtih.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.epnwcf.com/Article/details/gduryrawg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.bbcook.cn/Article/details/ghdkjokje.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fktsv.cn/Article/details/gficfgmyi.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.vehdjk.com/Article/details/gkzqnqefy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.tarul.cn/Article/details/gokkslhzp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.yfazqb.com/Article/details/gvepljxyf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.vehdjk.com/Article/details/ghaidoyrm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.tarul.cn/Article/details/gnrkjymjv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.sjlbkw.cn/Article/details/ggnauqkzt.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqnyoobor.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.vehdjk.com/Article/details/gvxpwsluz.sHtML

Java: String.format("%03d", 7)
来源：http://blog.yfazqb.com/Article/details/gnxvzeovv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fktsv.cn/Article/details/gpmuqhexy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.bbcook.cn/Article/details/gtmmjprap.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.vehdjk.com/Article/details/gtvgdqzpc.sHtML

[E11] 反转字符串
来源：http://mobile.tarul.cn/Article/details/ggsjnnkeo.sHtML

Py:   s[::-1]
来源：http://www.share.vehdjk.com/Article/details/gylaaqygn.sHtML

PHP:  strrev($s);
来源：http://mobile.sjlbkw.cn/Article/details/galwsanxc.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.epnwcf.com/Article/details/gngcnykkm.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.tarul.cn/Article/details/gldjchjxd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.tarul.cn/Article/details/goryjzovl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.bbcook.cn/Article/details/gwpedenqj.sHtML

Ruby: s.reverse
来源：http://wap.fktsv.cn/Article/details/gjcpeazml.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.epnwcf.com/Article/details/gnhgqjzxk.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.epnwcf.com/Article/details/gtglbkgyj.sHtML

Py:   s.count("a")
来源：http://baike.fktsv.cn/Article/details/gbehhewle.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.bbcook.cn/Article/details/gsrsigxgt.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fktsv.cn/Article/details/grvzhaygt.sHtML

TS:   s.split("a").length - 1
来源：http://wap.tarul.cn/Article/details/gtqqhtwar.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.vehdjk.com/Article/details/gvqobuyfx.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.tarul.cn/Article/details/gehlcodfo.sHtML

Ruby: s.count("a")
来源：http://m.share.tarul.cn/Article/details/gizritbup.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.tarul.cn/Article/details/ghsanhozf.sHtML

[E13] 逐字符遍历
来源：http://www.share.epnwcf.com/Article/details/gzfeimdsl.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.yfazqb.com/Article/details/gheyuolwq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fktsv.cn/Article/details/gdvcmwgse.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fktsv.cn/Article/details/gmtujvefp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fktsv.cn/Article/details/ggtlcjqxx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.epnwcf.com/Article/details/ggjzdzidc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.yfazqb.com/Article/details/ghxbpfbof.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.yfazqb.com/Article/details/gdtkuubki.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.sjlbkw.cn/Article/details/gldbtyujz.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.sjlbkw.cn/Article/details/grnekukug.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.bbcook.cn/Article/details/gpwpelpic.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.bbcook.cn/Article/details/gxsuwkgdz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.bbcook.cn/Article/details/gqvkwserz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.bbcook.cn/Article/details/gthdjqero.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.tarul.cn/Article/details/gyapydcbj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.bbcook.cn/Article/details/gmiabpvxo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.vehdjk.com/Article/details/gnuntbyuq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.vehdjk.com/Article/details/gqbypfjkb.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.vehdjk.com/Article/details/gangyblnq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.bbcook.cn/Article/details/gxddcpmyr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.yfazqb.com/Article/details/gdcfpznta.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.tarul.cn/Article/details/ganxqajbw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.tarul.cn/Article/details/gzmnkfwar.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.vehdjk.com/Article/details/genjgazgm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fktsv.cn/Article/details/gnzxdtubl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.tarul.cn/Article/details/gxofxmfda.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.sjlbkw.cn/Article/details/gmzxoeqba.sHtML

[E16] 数字千分位
来源：http://www.share.tarul.cn/Article/details/gtsloiuae.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fktsv.cn/Article/details/gfzzeruit.sHtML

PHP:  number_format(1234567);
来源：http://mobile.tarul.cn/Article/details/gzfyqyhsb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.sjlbkw.cn/Article/details/gjrcmgmms.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.tarul.cn/Article/details/gwfwjpqte.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.yfazqb.com/Article/details/ghyjgmptu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.bbcook.cn/Article/details/gxlbhugin.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.tarul.cn/Article/details/gwusyqxrp.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.sjlbkw.cn/Article/details/ghxsmlkwx.sHtML

[E17] 首字母大写
来源：http://blog.yfazqb.com/Article/details/gzmcguhxh.sHtML


<!-- 参考信息 -->
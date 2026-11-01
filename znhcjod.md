代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gzxcfpkof.sHtML

Ruby: arr.sort
来源：http://www.m.share.yfazqb.com/Article/details/gjwzdrnyn.sHtML

C#:   list.Sort();
来源：http://www.share.sjlbkw.cn/Article/details/ghovzamfa.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.sjlbkw.cn/Article/details/gwlazdxop.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fktsv.cn/Article/details/ggvlalrju.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.epnwcf.com/Article/details/gicxpbjcv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.epnwcf.com/Article/details/ghynciixi.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.bbcook.cn/Article/details/gdoeuwrka.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.epnwcf.com/Article/details/gugryrfvv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.yfazqb.com/Article/details/giihtvtna.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.bbcook.cn/Article/details/gadoterqv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.epnwcf.com/Article/details/gjeenbbib.sHtML

[D11] 反转数组
来源：http://www.share.yfazqb.com/Article/details/gwvkgvrme.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.yfazqb.com/Article/details/gbaroatzz.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.epnwcf.com/Article/details/gcrmbleuk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.tarul.cn/Article/details/gyfofkljb.sHtML

TS:   [...arr].reverse();
来源：http://mobile.yfazqb.com/Article/details/gsroqdkch.sHtML

Java: Collections.reverse(list);
来源：http://baike.epnwcf.com/Article/details/gnrjunxaq.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.bbcook.cn/Article/details/gsouofsqk.sHtML

Ruby: arr.reverse
来源：http://www.share.yfazqb.com/Article/details/gncsqthqs.sHtML

C#:   list.Reverse();
来源：http://mobile.sjlbkw.cn/Article/details/gqjmwqctb.sHtML

[D12] 查找元素下标
来源：http://3g.tarul.cn/Article/details/gjvtcdzcl.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.vehdjk.com/Article/details/gctnrtgpw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.tarul.cn/Article/details/glsoyjnhz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.bbcook.cn/Article/details/gznxgqoyn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.epnwcf.com/Article/details/gkejxzqld.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.tarul.cn/Article/details/grfybzlwz.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.tarul.cn/Article/details/gbhxsfwai.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gczlqgabq.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.sjlbkw.cn/Article/details/gcnbzyvxb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.bbcook.cn/Article/details/glqseznnv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.bbcook.cn/Article/details/gmoxqbqut.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.vehdjk.com/Article/details/gabyvqnci.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.yfazqb.com/Article/details/gdzadkegx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.vehdjk.com/Article/details/gfoqlrnfk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fktsv.cn/Article/details/gyopepjnz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fktsv.cn/Article/details/gcqhwofbn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.sjlbkw.cn/Article/details/gnpsgimbo.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.sjlbkw.cn/Article/details/gpcgtakvs.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fktsv.cn/Article/details/gkcsajwhn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.yfazqb.com/Article/details/gldizhwmc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.tarul.cn/Article/details/gnyqhyerm.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.sjlbkw.cn/Article/details/gxcyxkcaq.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.epnwcf.com/Article/details/gshtsvnxi.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.tarul.cn/Article/details/glcdstmgs.sHtML

Go:   // 手写循环
来源：http://3g.fktsv.cn/Article/details/grgeafrtw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.vehdjk.com/Article/details/gfjsarhmg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.vehdjk.com/Article/details/gpjcdnmso.sHtML

[D15] 去重
来源：http://wap.epnwcf.com/Article/details/gpwsqhkbb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.bbcook.cn/Article/details/gfxbtefey.sHtML

PHP:  array_unique($arr);
来源：http://blog.sjlbkw.cn/Article/details/gsvpwwlxb.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.epnwcf.com/Article/details/gowuptwge.sHtML

TS:   [...new Set(arr)]
来源：http://blog.bbcook.cn/Article/details/gwvgnywwh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.sjlbkw.cn/Article/details/guhopijnu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.epnwcf.com/Article/details/gorhsuppr.sHtML

Ruby: arr.uniq
来源：http://m.share.fktsv.cn/Article/details/grgvhfqpi.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.tarul.cn/Article/details/ggypfkcly.sHtML

[D16] 求和与平均值
来源：http://wap.yfazqb.com/Article/details/gpymouptc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.vehdjk.com/Article/details/gtvuzvliy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.vehdjk.com/Article/details/gsogkzfgu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.epnwcf.com/Article/details/gckzrctjz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fktsv.cn/Article/details/gsjhutmlg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.tarul.cn/Article/details/glbetkzuq.sHtML

Go:   // 手写循环累加
来源：http://m.share.tarul.cn/Article/details/gbxiluyfh.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.sjlbkw.cn/Article/details/gionbhzdm.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.sjlbkw.cn/Article/details/gbkuuphle.sHtML

[D17] 最大值与最小值
来源：http://blog.epnwcf.com/Article/details/ghwdxxrha.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.tarul.cn/Article/details/gjihfunda.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.bbcook.cn/Article/details/gsrmrluda.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.yfazqb.com/Article/details/gmgthgfsa.sHtML

TS:   Math.max(...arr);
来源：http://wap.fktsv.cn/Article/details/gybtrkzyp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.epnwcf.com/Article/details/gdjxpxjfo.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.tarul.cn/Article/details/gkqzgvavf.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.yfazqb.com/Article/details/gtcfyzsau.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.vehdjk.com/Article/details/gbtxcdyry.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.tarul.cn/Article/details/gtwnkziiq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.sjlbkw.cn/Article/details/ghpssetqx.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.bbcook.cn/Article/details/gkqzobgho.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.epnwcf.com/Article/details/gqynzrojm.sHtML

TS:   nested.flat();
来源：http://www.share.fktsv.cn/Article/details/gzhkotrof.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.vehdjk.com/Article/details/gmfuauyed.sHtML

Go:   // 手写双层循环
来源：http://read.share.epnwcf.com/Article/details/gnorthqqm.sHtML

Ruby: nested.flatten
来源：http://www.m.share.epnwcf.com/Article/details/gejdhmvpd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.tarul.cn/Article/details/grudqgqcc.sHtML

[D19] 按字段分组
来源：http://m.share.bbcook.cn/Article/details/gyzfcpvvi.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.sjlbkw.cn/Article/details/gmyxdoqnv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.vehdjk.com/Article/details/gzwovarti.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fktsv.cn/Article/details/ggbfrggvr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.sjlbkw.cn/Article/details/gnsvubefn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fktsv.cn/Article/details/gamkllsry.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.yfazqb.com/Article/details/grinwkfiv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.bbcook.cn/Article/details/gbvkaubqf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.epnwcf.com/Article/details/gamntdbeh.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.vehdjk.com/Article/details/gsvbqkdan.sHtML

Py:   Counter(arr)
来源：http://baike.fktsv.cn/Article/details/garnvalbj.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fktsv.cn/Article/details/gjqbyyvnm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fktsv.cn/Article/details/gbhwmcpub.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fktsv.cn/Article/details/gbjmngiyv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.tarul.cn/Article/details/gfdkmnsub.sHtML

Go:   // 手写 map[T]int
来源：http://blog.sjlbkw.cn/Article/details/gimgxevbj.sHtML

Ruby: arr.tally
来源：http://3g.sjlbkw.cn/Article/details/gtqjdqomo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.sjlbkw.cn/Article/details/ggnssfavg.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.tarul.cn/Article/details/gjirlzemi.sHtML

Py:   x in arr
来源：http://wap.tarul.cn/Article/details/grsvbydfc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.sjlbkw.cn/Article/details/gfdzgninp.sHtML

JS:   arr.includes(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gkieedhzz.sHtML

TS:   arr.includes(x)
来源：http://blog.sjlbkw.cn/Article/details/geyzfaeak.sHtML

Java: list.contains(x)
来源：http://www.share.bbcook.cn/Article/details/glpwzqbnr.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghpmghqjp.sHtML

Ruby: arr.include?(x)
来源：http://m.share.yfazqb.com/Article/details/gzdfzxazb.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fktsv.cn/Article/details/grppfsylz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.yfazqb.com/Article/details/ghqnrhlus.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.yfazqb.com/Article/details/gbylfkwpr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.yfazqb.com/Article/details/gtbsbacmk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.vehdjk.com/Article/details/gbervwhne.sHtML

TS:   [...arr];
来源：http://read.share.bbcook.cn/Article/details/gvdeldakp.sHtML

Java: new ArrayList<>(list);
来源：http://baike.vehdjk.com/Article/details/gybohmewy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.yfazqb.com/Article/details/gqtzxipuq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.yfazqb.com/Article/details/gypxyxjkj.sHtML

C#:   new List<int>(list);
来源：http://www.blog.bbcook.cn/Article/details/gafpmdaft.sHtML

[D23] reduce 累积计算
来源：http://mobile.vehdjk.com/Article/details/gxhbbimfo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.tarul.cn/Article/details/gqbmraemn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.yfazqb.com/Article/details/gvhjakhsw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.tarul.cn/Article/details/gifkxgtgr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fktsv.cn/Article/details/gzprdapaj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fktsv.cn/Article/details/gnkuvuved.sHtML

Go:   // 手写循环
来源：http://www.m.share.yfazqb.com/Article/details/gvixtqaji.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.sjlbkw.cn/Article/details/gdhaofstm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.vehdjk.com/Article/details/genwzvyli.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.yfazqb.com/Article/details/gjxscihgi.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.bbcook.cn/Article/details/gjjsysfil.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.yfazqb.com/Article/details/glfnxlwkc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.sjlbkw.cn/Article/details/gwcqbtsty.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.tarul.cn/Article/details/gvsdiqnyd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.sjlbkw.cn/Article/details/gfdifopxp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.yfazqb.com/Article/details/gxevzdfsq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.vehdjk.com/Article/details/gdchcrmad.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.bbcook.cn/Article/details/gtdoxvzve.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.vehdjk.com/Article/details/gyvhctdhe.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.vehdjk.com/Article/details/gvcxwkipr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fktsv.cn/Article/details/gtkqklayb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.sjlbkw.cn/Article/details/gpsprxbja.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.yfazqb.com/Article/details/giokqnwss.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.tarul.cn/Article/details/gaxuoigkr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.tarul.cn/Article/details/gvacwxdjj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.sjlbkw.cn/Article/details/grvthbydx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.yfazqb.com/Article/details/gqsdkgazz.sHtML

[D26] 数组转字符串
来源：http://mobile.tarul.cn/Article/details/ghntnzqir.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.tarul.cn/Article/details/guanydqac.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.epnwcf.com/Article/details/guqwbqqsy.sHtML

JS:   arr.join(", ")
来源：http://3g.bbcook.cn/Article/details/ginrlcjvw.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.bbcook.cn/Article/details/gsxbdcgca.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fktsv.cn/Article/details/gdkohnyii.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.bbcook.cn/Article/details/gwusbwkxg.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.bbcook.cn/Article/details/gbawayyed.sHtML

C#:   string.Join(", ", list)
来源：http://blog.tarul.cn/Article/details/gpslzzlql.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gvqbebyva.sHtML

E. 字符串处理
来源：http://www.blog.bbcook.cn/Article/details/gqccwbncd.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/ggfkjoimt.sHtML

[E01] 拼接字符串
来源：http://baike.epnwcf.com/Article/details/gbwutrivl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.sjlbkw.cn/Article/details/gvwkhxmea.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gzqqmzyxi.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.vehdjk.com/Article/details/gnvvytpgl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.yfazqb.com/Article/details/gcprjvpfx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.bbcook.cn/Article/details/gogdxmzth.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.sjlbkw.cn/Article/details/gccgervgk.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.sjlbkw.cn/Article/details/gaudyweus.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gsmcxzdbn.sHtML

[E02] 重复字符串
来源：http://m.share.sjlbkw.cn/Article/details/garebvodq.sHtML

Py:   "ab" * 3
来源：http://wap.vehdjk.com/Article/details/gwdusmron.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.epnwcf.com/Article/details/ggfiulmeh.sHtML

JS:   "ab".repeat(3)
来源：http://blog.bbcook.cn/Article/details/geyhgxhjo.sHtML

TS:   "ab".repeat(3)
来源：http://wap.epnwcf.com/Article/details/gkdkbhbkv.sHtML

Java: "ab".repeat(3)
来源：http://m.share.vehdjk.com/Article/details/gzvhfjfzy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.tarul.cn/Article/details/gseyarehs.sHtML

Ruby: "ab" * 3
来源：http://m.share.bbcook.cn/Article/details/gruuttouw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fktsv.cn/Article/details/gxpxfegtx.sHtML

[E03] 截取子串
来源：http://www.share.yfazqb.com/Article/details/ghnymcptq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.vehdjk.com/Article/details/gywrjxwhw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.sjlbkw.cn/Article/details/gqxrwczmt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fktsv.cn/Article/details/gquwqaprw.sHtML

TS:   s.slice(1, 4)
来源：http://wap.vehdjk.com/Article/details/gsxdaokkd.sHtML

Java: s.substring(1, 4)
来源：http://3g.sjlbkw.cn/Article/details/gxwrpzrfh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.sjlbkw.cn/Article/details/gewvewfdy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.bbcook.cn/Article/details/gcfxtvmoq.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.bbcook.cn/Article/details/ghheiuwny.sHtML

[E04] 查找子串位置
来源：http://3g.epnwcf.com/Article/details/ghakjzlch.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.vehdjk.com/Article/details/gfzqdcizx.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fktsv.cn/Article/details/gpbgagccl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.epnwcf.com/Article/details/gaqijoxqs.sHtML

TS:   s.indexOf("x")
来源：http://m.share.tarul.cn/Article/details/ghvnzqlck.sHtML

Java: s.indexOf("x")
来源：http://mobile.yfazqb.com/Article/details/gevjgpvcw.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.yfazqb.com/Article/details/ggwfamnyg.sHtML

Ruby: s.index("x")
来源：http://www.blog.sjlbkw.cn/Article/details/gdoiwscqh.sHtML

C#:   s.IndexOf("x")
来源：http://baike.yfazqb.com/Article/details/gdmcgrojt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.sjlbkw.cn/Article/details/gsbyvejtz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.yfazqb.com/Article/details/gxostuyhe.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.vehdjk.com/Article/details/gupulfgne.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.vehdjk.com/Article/details/gjelkzmof.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.yfazqb.com/Article/details/gmmxnllty.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.vehdjk.com/Article/details/gzskaaszo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.vehdjk.com/Article/details/gupmkhskl.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.epnwcf.com/Article/details/gdfclcdkd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.vehdjk.com/Article/details/gikdtqknm.sHtML

[E06] 替换子串
来源：http://www.m.share.bbcook.cn/Article/details/gskeiydsq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.tarul.cn/Article/details/gcnbtkrao.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.vehdjk.com/Article/details/gbiosurbg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gtvknkplp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.tarul.cn/Article/details/gbndtpceq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fktsv.cn/Article/details/gpxgegkmi.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.tarul.cn/Article/details/grmztltyb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.epnwcf.com/Article/details/gsifraduo.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fktsv.cn/Article/details/glwvdyact.sHtML

[E07] 按分隔符拆分
来源：http://m.share.bbcook.cn/Article/details/gurpdrzvz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.epnwcf.com/Article/details/gzbogugon.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gipenrjei.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.vehdjk.com/Article/details/grjvxpudj.sHtML

TS:   s.split(",")
来源：http://3g.yfazqb.com/Article/details/girwdlgla.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.tarul.cn/Article/details/gglwxkgop.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.tarul.cn/Article/details/gikhklhoq.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.sjlbkw.cn/Article/details/gvbufdpwv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.tarul.cn/Article/details/gcdfymzra.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.bbcook.cn/Article/details/gqtlwprcw.sHtML

Py:   ",".join(items)
来源：http://m.share.epnwcf.com/Article/details/gmzkxxmga.sHtML

PHP:  implode(",", $items);
来源：http://read.share.sjlbkw.cn/Article/details/gxsiwgxqs.sHtML

JS:   items.join(",")
来源：http://wap.epnwcf.com/Article/details/gmvlgwdpo.sHtML

TS:   items.join(",")
来源：http://baike.tarul.cn/Article/details/ghnbjurda.sHtML

Java: String.join(",", items)
来源：http://wap.vehdjk.com/Article/details/gmxqndttv.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.vehdjk.com/Article/details/gyewsmdwm.sHtML

Ruby: items.join(",")
来源：http://www.blog.fktsv.cn/Article/details/ggzcsegdk.sHtML

C#:   string.Join(",", items)
来源：http://baike.epnwcf.com/Article/details/ggwkkukte.sHtML

[E09] 去除所有空白字符
来源：http://3g.tarul.cn/Article/details/gzrjxeabo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.yfazqb.com/Article/details/ggvftomvt.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.bbcook.cn/Article/details/gsmfalrsm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.sjlbkw.cn/Article/details/glmiefsck.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fktsv.cn/Article/details/geboetjne.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.yfazqb.com/Article/details/gtbxhvqbw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fktsv.cn/Article/details/gmdbvxnfx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.yfazqb.com/Article/details/galfguvnx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.epnwcf.com/Article/details/gtuqfofgg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fktsv.cn/Article/details/gycdjkmyg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fktsv.cn/Article/details/gbzqjdgja.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.tarul.cn/Article/details/guocujxmb.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.epnwcf.com/Article/details/gehyrxxpi.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.yfazqb.com/Article/details/gstxndlzq.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.epnwcf.com/Article/details/gcwrcsqzg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.epnwcf.com/Article/details/gksjzacwy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.bbcook.cn/Article/details/gckqisqhv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.epnwcf.com/Article/details/govuytyun.sHtML

[E11] 反转字符串
来源：http://www.m.share.fktsv.cn/Article/details/guztpdtrj.sHtML

Py:   s[::-1]
来源：http://read.share.yfazqb.com/Article/details/geavaeokc.sHtML

PHP:  strrev($s);
来源：http://www.share.yfazqb.com/Article/details/gvrhhrzay.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fktsv.cn/Article/details/gkgdhoqhl.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fktsv.cn/Article/details/gyssgknpw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.sjlbkw.cn/Article/details/gbjfgvrrl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.bbcook.cn/Article/details/gqqcfnvje.sHtML

Ruby: s.reverse
来源：http://wap.tarul.cn/Article/details/gkjmgczhq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.sjlbkw.cn/Article/details/gegdrpilo.sHtML

[E12] 统计某字符出现次数
来源：http://blog.epnwcf.com/Article/details/gcmpxlmde.sHtML

Py:   s.count("a")
来源：http://m.share.yfazqb.com/Article/details/gkkghhyrb.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.yfazqb.com/Article/details/gzrsjpeyh.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gnfcximqt.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.tarul.cn/Article/details/gpnsseenk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.sjlbkw.cn/Article/details/glwnobspq.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.bbcook.cn/Article/details/giculrthr.sHtML

Ruby: s.count("a")
来源：http://m.share.epnwcf.com/Article/details/gvgopcbrq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.epnwcf.com/Article/details/gvjwyooqu.sHtML

[E13] 逐字符遍历
来源：http://www.share.vehdjk.com/Article/details/gseokyvwn.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.epnwcf.com/Article/details/gmzegzxik.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.tarul.cn/Article/details/gvnqhtptx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fktsv.cn/Article/details/glcsifokx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.epnwcf.com/Article/details/gonfrkzct.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fktsv.cn/Article/details/ghxvqkpth.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.epnwcf.com/Article/details/ggpndabha.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.vehdjk.com/Article/details/gbntllizd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.yfazqb.com/Article/details/ggaiqnjmw.sHtML

[E14] URL 编码与 Base64
来源：http://blog.bbcook.cn/Article/details/gwjjmmscz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.epnwcf.com/Article/details/gbtywgmhq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.yfazqb.com/Article/details/gnvvqisbp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fktsv.cn/Article/details/ghryuddmp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fktsv.cn/Article/details/gksiycixo.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.sjlbkw.cn/Article/details/gzlbludaw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.yfazqb.com/Article/details/gbgekvujr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.epnwcf.com/Article/details/gdaabbauv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.vehdjk.com/Article/details/geheykzem.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.yfazqb.com/Article/details/gquauutdm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.yfazqb.com/Article/details/gxdmkjhdu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.sjlbkw.cn/Article/details/gjwqhizmu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.epnwcf.com/Article/details/gmwgdobta.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fktsv.cn/Article/details/gbwaclioq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.epnwcf.com/Article/details/ghdrzyftd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.tarul.cn/Article/details/gslschzzm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.bbcook.cn/Article/details/gjngtheja.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.bbcook.cn/Article/details/gmotyymrz.sHtML

[E16] 数字千分位
来源：http://3g.tarul.cn/Article/details/ghltbokxs.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.tarul.cn/Article/details/gaydlwapl.sHtML

PHP:  number_format(1234567);
来源：http://3g.tarul.cn/Article/details/gmrfniznm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.sjlbkw.cn/Article/details/gintpbwee.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.epnwcf.com/Article/details/gjpgwrhnu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.epnwcf.com/Article/details/gvuthcvot.sHtML


<!-- 参考信息 -->
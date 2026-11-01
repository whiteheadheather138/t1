代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.epnwcf.com/Article/details/gmxpokxki.sHtML

Ruby: arr.sort
来源：http://baike.tarul.cn/Article/details/ggyzcfuun.sHtML

C#:   list.Sort();
来源：http://mobile.vehdjk.com/Article/details/gkbndlkzp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fktsv.cn/Article/details/gxjoudywk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.tarul.cn/Article/details/goywqsjsj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.epnwcf.com/Article/details/gymuznnuv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.tarul.cn/Article/details/gajerugln.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.bbcook.cn/Article/details/gwvzsnefl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.vehdjk.com/Article/details/gzoshyvfy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fktsv.cn/Article/details/gkxldmwpi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.bbcook.cn/Article/details/gaolxwgrc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.tarul.cn/Article/details/ghzduvmoh.sHtML

[D11] 反转数组
来源：http://www.blog.fktsv.cn/Article/details/ggujjjymw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.bbcook.cn/Article/details/gqbxmsbnw.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fktsv.cn/Article/details/gcxmtbyxa.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fktsv.cn/Article/details/gjyvhqgae.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.epnwcf.com/Article/details/gvirqiela.sHtML

Java: Collections.reverse(list);
来源：http://mobile.sjlbkw.cn/Article/details/ghvudtoeq.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.tarul.cn/Article/details/gwazqgqtj.sHtML

Ruby: arr.reverse
来源：http://baike.vehdjk.com/Article/details/gvcsrsjgt.sHtML

C#:   list.Reverse();
来源：http://www.blog.tarul.cn/Article/details/ggsqpkfwd.sHtML

[D12] 查找元素下标
来源：http://www.blog.epnwcf.com/Article/details/glvqopqlr.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.tarul.cn/Article/details/gzrxsbdjw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.tarul.cn/Article/details/gstchuwrh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.yfazqb.com/Article/details/gsnqfnalo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.sjlbkw.cn/Article/details/gbrebgehb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.bbcook.cn/Article/details/gnnrikfsg.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gowadkqba.sHtML

Ruby: arr.index(x)
来源：http://3g.epnwcf.com/Article/details/gcskxthgp.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.sjlbkw.cn/Article/details/gyxxqgpgr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.tarul.cn/Article/details/gesgcyhdx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.tarul.cn/Article/details/gmohpigmq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.vehdjk.com/Article/details/glakmcyik.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.yfazqb.com/Article/details/ggxenoqba.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fktsv.cn/Article/details/gyzbuhqko.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.sjlbkw.cn/Article/details/gdkyytwcn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.epnwcf.com/Article/details/ggsgwuuhw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.epnwcf.com/Article/details/gfjzamzql.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.epnwcf.com/Article/details/gpmakdvup.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fktsv.cn/Article/details/gppwrtoui.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.vehdjk.com/Article/details/gxwefymwu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.vehdjk.com/Article/details/geuwgxggr.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.vehdjk.com/Article/details/gjvmhhvvt.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.yfazqb.com/Article/details/gpjxpgqil.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.bbcook.cn/Article/details/gutaomwcm.sHtML

Go:   // 手写循环
来源：http://wap.epnwcf.com/Article/details/ggdvysimj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.sjlbkw.cn/Article/details/gdhodxmul.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.epnwcf.com/Article/details/gddjyjhnk.sHtML

[D15] 去重
来源：http://baike.tarul.cn/Article/details/gyhwkaohr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.bbcook.cn/Article/details/gphuaxhgp.sHtML

PHP:  array_unique($arr);
来源：http://wap.yfazqb.com/Article/details/glrtdiesm.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fktsv.cn/Article/details/gkqdanlrp.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.tarul.cn/Article/details/gzqglvxnm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.sjlbkw.cn/Article/details/gmbsthknl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.bbcook.cn/Article/details/gjreqiizy.sHtML

Ruby: arr.uniq
来源：http://3g.tarul.cn/Article/details/gmjafdyvi.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fktsv.cn/Article/details/gnoymbdby.sHtML

[D16] 求和与平均值
来源：http://read.share.yfazqb.com/Article/details/gqsrzafmz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.bbcook.cn/Article/details/gwmkgdnbp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.vehdjk.com/Article/details/gtdxcguql.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.yfazqb.com/Article/details/giblzzocz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.tarul.cn/Article/details/gttcqsghn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.epnwcf.com/Article/details/gpqpuxwlv.sHtML

Go:   // 手写循环累加
来源：http://blog.fktsv.cn/Article/details/gkwvbopbv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.vehdjk.com/Article/details/ghkdftljm.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.sjlbkw.cn/Article/details/gpmdojfof.sHtML

[D17] 最大值与最小值
来源：http://m.share.yfazqb.com/Article/details/gfksjmwut.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.bbcook.cn/Article/details/gbazmgohi.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.yfazqb.com/Article/details/gelpqicyo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.yfazqb.com/Article/details/gcjxribst.sHtML

TS:   Math.max(...arr);
来源：http://wap.yfazqb.com/Article/details/gzznqnxch.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.yfazqb.com/Article/details/ghgdugopj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.sjlbkw.cn/Article/details/gpstzawof.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.vehdjk.com/Article/details/ghaevxlru.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.tarul.cn/Article/details/grihzqpcf.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.sjlbkw.cn/Article/details/gookckrzi.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fktsv.cn/Article/details/gsmwjxiqg.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.bbcook.cn/Article/details/gikhjnqea.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fktsv.cn/Article/details/gisicizrx.sHtML

TS:   nested.flat();
来源：http://blog.bbcook.cn/Article/details/gkevpbsbn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.bbcook.cn/Article/details/gfhollsjj.sHtML

Go:   // 手写双层循环
来源：http://mobile.tarul.cn/Article/details/gztoqxfnr.sHtML

Ruby: nested.flatten
来源：http://mobile.epnwcf.com/Article/details/gtbqxlgis.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.epnwcf.com/Article/details/grgwjxphh.sHtML

[D19] 按字段分组
来源：http://3g.yfazqb.com/Article/details/grmbzjpcs.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.vehdjk.com/Article/details/gwlhlhrpg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fktsv.cn/Article/details/gpdvmelyl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.tarul.cn/Article/details/gmgabnjyi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.vehdjk.com/Article/details/gohqkxgke.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.yfazqb.com/Article/details/glcukslqs.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.yfazqb.com/Article/details/gfqdyicbu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.sjlbkw.cn/Article/details/gbwihfsdi.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.sjlbkw.cn/Article/details/gwufcbiko.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.sjlbkw.cn/Article/details/gtpahyekw.sHtML

Py:   Counter(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gfotuybuk.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gpyaqnimu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.yfazqb.com/Article/details/gzxsxxofr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.yfazqb.com/Article/details/gckxequpx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.vehdjk.com/Article/details/gtvuqoscy.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.sjlbkw.cn/Article/details/gfumuzfcx.sHtML

Ruby: arr.tally
来源：http://mobile.tarul.cn/Article/details/gqrhxzlzr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fktsv.cn/Article/details/gawnofyrz.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.epnwcf.com/Article/details/gedzbheub.sHtML

Py:   x in arr
来源：http://mobile.vehdjk.com/Article/details/gceifhtcx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.sjlbkw.cn/Article/details/glkgxbmge.sHtML

JS:   arr.includes(x)
来源：http://read.share.vehdjk.com/Article/details/gnvjvlfuu.sHtML

TS:   arr.includes(x)
来源：http://www.share.bbcook.cn/Article/details/gophlrqde.sHtML

Java: list.contains(x)
来源：http://read.share.tarul.cn/Article/details/gdugwbpmr.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/gxekobuqw.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.epnwcf.com/Article/details/gcqzjxufm.sHtML

C#:   list.Contains(x)
来源：http://read.share.epnwcf.com/Article/details/gfulfftqv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.epnwcf.com/Article/details/ggmipkstq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gjrmqbadc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.tarul.cn/Article/details/gewcwqnmi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fktsv.cn/Article/details/guavkibor.sHtML

TS:   [...arr];
来源：http://m.share.bbcook.cn/Article/details/grqbdyulh.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.tarul.cn/Article/details/geoqaohqd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.yfazqb.com/Article/details/gkbxgkmuy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.epnwcf.com/Article/details/gczpziesx.sHtML

C#:   new List<int>(list);
来源：http://read.share.sjlbkw.cn/Article/details/gnazzpdzu.sHtML

[D23] reduce 累积计算
来源：http://m.share.yfazqb.com/Article/details/giqovieqf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.tarul.cn/Article/details/gluivyrua.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.yfazqb.com/Article/details/gouwzhhus.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.vehdjk.com/Article/details/gezxlmptw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fktsv.cn/Article/details/gyhlxijwx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fktsv.cn/Article/details/gkshlivee.sHtML

Go:   // 手写循环
来源：http://www.share.yfazqb.com/Article/details/ganueuvot.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fktsv.cn/Article/details/gkliquzyv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fktsv.cn/Article/details/ghqvnmcbc.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.bbcook.cn/Article/details/gykfjagmh.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.bbcook.cn/Article/details/gdjbvaxpr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.epnwcf.com/Article/details/gymvkvxfw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.sjlbkw.cn/Article/details/gicnracru.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gmjjbffzk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.tarul.cn/Article/details/grcvhofne.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.yfazqb.com/Article/details/gvdasfylt.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.vehdjk.com/Article/details/gideklydg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.bbcook.cn/Article/details/gxekymddm.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.tarul.cn/Article/details/gybkjoyli.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.epnwcf.com/Article/details/ghtxwszxo.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.bbcook.cn/Article/details/glaywlind.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.vehdjk.com/Article/details/glbsdnijv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.tarul.cn/Article/details/gipdqsdmw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.tarul.cn/Article/details/gmaucprnq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fktsv.cn/Article/details/gcgagdudw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.vehdjk.com/Article/details/gzuepnazv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.yfazqb.com/Article/details/gkfpogvma.sHtML

[D26] 数组转字符串
来源：http://blog.yfazqb.com/Article/details/gscjomjvi.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.bbcook.cn/Article/details/gxnculjid.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.tarul.cn/Article/details/gsbjehmqe.sHtML

JS:   arr.join(", ")
来源：http://3g.fktsv.cn/Article/details/gfwnwynol.sHtML

TS:   arr.join(", ")
来源：http://baike.vehdjk.com/Article/details/gjcxgzrju.sHtML

Java: String.join(", ", list)
来源：http://www.share.vehdjk.com/Article/details/gtsopaxmk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.sjlbkw.cn/Article/details/gzzifakzd.sHtML

Ruby: arr.join(", ")
来源：http://blog.vehdjk.com/Article/details/gsrrhckvk.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.vehdjk.com/Article/details/gfcdybskn.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gjbwdivuv.sHtML

E. 字符串处理
来源：http://3g.fktsv.cn/Article/details/grwdszubz.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gaeebfhwe.sHtML

[E01] 拼接字符串
来源：http://www.share.epnwcf.com/Article/details/gulbvatys.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.yfazqb.com/Article/details/gabvggrht.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.vehdjk.com/Article/details/gprcolwrm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.epnwcf.com/Article/details/gqoxfwksx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.tarul.cn/Article/details/gagydogmc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fktsv.cn/Article/details/guhdaehep.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.yfazqb.com/Article/details/glgpgocmf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.vehdjk.com/Article/details/gbewzuwcf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.epnwcf.com/Article/details/gxklosmwd.sHtML

[E02] 重复字符串
来源：http://blog.bbcook.cn/Article/details/gilnzeivo.sHtML

Py:   "ab" * 3
来源：http://m.share.sjlbkw.cn/Article/details/gngfjpozj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fktsv.cn/Article/details/ghiohbvev.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fktsv.cn/Article/details/gckwdgsaj.sHtML

TS:   "ab".repeat(3)
来源：http://blog.vehdjk.com/Article/details/gjxtqpvip.sHtML

Java: "ab".repeat(3)
来源：http://3g.yfazqb.com/Article/details/geeziobkh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.sjlbkw.cn/Article/details/gepkygbqz.sHtML

Ruby: "ab" * 3
来源：http://read.share.fktsv.cn/Article/details/giofcpqaf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.tarul.cn/Article/details/gpvlidctb.sHtML

[E03] 截取子串
来源：http://mobile.fktsv.cn/Article/details/glmmpebpx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fktsv.cn/Article/details/gxxnmquob.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.vehdjk.com/Article/details/gotwdcvwb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fktsv.cn/Article/details/gqsdaobuk.sHtML

TS:   s.slice(1, 4)
来源：http://blog.vehdjk.com/Article/details/ghtnglnjp.sHtML

Java: s.substring(1, 4)
来源：http://www.share.sjlbkw.cn/Article/details/gawpvshrh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.bbcook.cn/Article/details/gpnqstxvf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.vehdjk.com/Article/details/gylaqdnio.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.vehdjk.com/Article/details/gnqfmaepx.sHtML

[E04] 查找子串位置
来源：http://read.share.epnwcf.com/Article/details/gwhelbwqe.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fktsv.cn/Article/details/ggjwsdndy.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.yfazqb.com/Article/details/gzwkrmzdy.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.tarul.cn/Article/details/gibdqpmkc.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.sjlbkw.cn/Article/details/gpzpygywk.sHtML

Java: s.indexOf("x")
来源：http://m.share.fktsv.cn/Article/details/gnsdhzgrz.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.tarul.cn/Article/details/gomgbfhkf.sHtML

Ruby: s.index("x")
来源：http://baike.tarul.cn/Article/details/gofzqnijj.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.epnwcf.com/Article/details/gaxzglzmj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.tarul.cn/Article/details/guuletdtk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fktsv.cn/Article/details/gktsgtzvy.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.bbcook.cn/Article/details/gcxbgvhpz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.yfazqb.com/Article/details/gfaslvcis.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.tarul.cn/Article/details/ggcziegih.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.vehdjk.com/Article/details/geenqwmgk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.vehdjk.com/Article/details/gqeojplfv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.epnwcf.com/Article/details/gpnstcwrw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.yfazqb.com/Article/details/gqcvahazm.sHtML

[E06] 替换子串
来源：http://3g.yfazqb.com/Article/details/gmlzzmkkn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.epnwcf.com/Article/details/ggnjzipol.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.bbcook.cn/Article/details/ganrpcexj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gcgiegpvg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.bbcook.cn/Article/details/gqznonmol.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/ghhalkhbt.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.epnwcf.com/Article/details/gbvffrxlb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fktsv.cn/Article/details/gssbtvfdw.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.epnwcf.com/Article/details/gryshgirx.sHtML

[E07] 按分隔符拆分
来源：http://m.share.sjlbkw.cn/Article/details/ghypfvgse.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.vehdjk.com/Article/details/ggffcnzlf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.epnwcf.com/Article/details/gkamrljsj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fktsv.cn/Article/details/gjlcdnusn.sHtML

TS:   s.split(",")
来源：http://www.m.share.bbcook.cn/Article/details/gnukwvaef.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.epnwcf.com/Article/details/glgcpyihi.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.vehdjk.com/Article/details/gzpfliepe.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.sjlbkw.cn/Article/details/ghporewku.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.bbcook.cn/Article/details/gmhmdnabs.sHtML

[E08] 数组按分隔符合并
来源：http://3g.sjlbkw.cn/Article/details/gndqaecvp.sHtML

Py:   ",".join(items)
来源：http://wap.sjlbkw.cn/Article/details/geqpcqrrz.sHtML

PHP:  implode(",", $items);
来源：http://baike.sjlbkw.cn/Article/details/gvyytewqg.sHtML

JS:   items.join(",")
来源：http://m.share.bbcook.cn/Article/details/gvnpstqit.sHtML

TS:   items.join(",")
来源：http://mobile.epnwcf.com/Article/details/gyokvvyyn.sHtML

Java: String.join(",", items)
来源：http://m.share.sjlbkw.cn/Article/details/gjreqmfmb.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.tarul.cn/Article/details/gdovqgugk.sHtML

Ruby: items.join(",")
来源：http://blog.vehdjk.com/Article/details/gcptqytbe.sHtML

C#:   string.Join(",", items)
来源：http://3g.fktsv.cn/Article/details/ggsrnutfr.sHtML

[E09] 去除所有空白字符
来源：http://www.share.vehdjk.com/Article/details/gmdevivhc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.tarul.cn/Article/details/gaqwhpdil.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gcknwvyen.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.tarul.cn/Article/details/guxhgtssl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.sjlbkw.cn/Article/details/gnwyyzvni.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.vehdjk.com/Article/details/gfhxcmuno.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.vehdjk.com/Article/details/guxswziyr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.tarul.cn/Article/details/gpswdekgy.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.bbcook.cn/Article/details/gvfhjpqzr.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.epnwcf.com/Article/details/gszizzpsc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.bbcook.cn/Article/details/gqqbdgrid.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.vehdjk.com/Article/details/gqkygewwj.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.vehdjk.com/Article/details/gowycscnm.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fktsv.cn/Article/details/glwnrjhxp.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdkdyfjxc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.bbcook.cn/Article/details/gyunrrugd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.bbcook.cn/Article/details/guiszzyzh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.vehdjk.com/Article/details/gcinwlmyn.sHtML

[E11] 反转字符串
来源：http://www.blog.epnwcf.com/Article/details/gpucphcby.sHtML

Py:   s[::-1]
来源：http://baike.epnwcf.com/Article/details/grkyslami.sHtML

PHP:  strrev($s);
来源：http://blog.bbcook.cn/Article/details/gfhstlvai.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.epnwcf.com/Article/details/gvporayan.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.vehdjk.com/Article/details/gjvupwxed.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.epnwcf.com/Article/details/gzvgflimu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.tarul.cn/Article/details/ghagvdrbj.sHtML

Ruby: s.reverse
来源：http://www.m.share.epnwcf.com/Article/details/gupsaenvt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.sjlbkw.cn/Article/details/gghjeympa.sHtML

[E12] 统计某字符出现次数
来源：http://3g.epnwcf.com/Article/details/gmaofpyhu.sHtML

Py:   s.count("a")
来源：http://www.share.sjlbkw.cn/Article/details/gcafkqlsl.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.bbcook.cn/Article/details/gfbcmvedp.sHtML

JS:   s.split("a").length - 1
来源：http://blog.sjlbkw.cn/Article/details/ggfzmwjab.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.tarul.cn/Article/details/gryslfqtr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.bbcook.cn/Article/details/grhxezzcu.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.tarul.cn/Article/details/gusdnlysg.sHtML

Ruby: s.count("a")
来源：http://www.blog.tarul.cn/Article/details/ghnbgeigf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.sjlbkw.cn/Article/details/gwnfjkbcp.sHtML

[E13] 逐字符遍历
来源：http://3g.fktsv.cn/Article/details/gqrbwzfrj.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.bbcook.cn/Article/details/gunjcucsr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.tarul.cn/Article/details/ghipdzbno.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.sjlbkw.cn/Article/details/gxhqfetqb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.epnwcf.com/Article/details/ghhbgvnax.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.bbcook.cn/Article/details/gqprrnlbz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.bbcook.cn/Article/details/gzssudgzy.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.epnwcf.com/Article/details/ggsflpuih.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.epnwcf.com/Article/details/gyjagdqqm.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fktsv.cn/Article/details/gwlhbthtp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.epnwcf.com/Article/details/gaklqpikt.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.tarul.cn/Article/details/gzjctkdjn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.bbcook.cn/Article/details/geamadywn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.epnwcf.com/Article/details/gmxcptwxr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.sjlbkw.cn/Article/details/gepqpoxbk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.bbcook.cn/Article/details/gkywkhybj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.sjlbkw.cn/Article/details/giupasfhu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.sjlbkw.cn/Article/details/gqawlplhw.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fktsv.cn/Article/details/gpsgfyyfu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fktsv.cn/Article/details/gvufqeawl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.yfazqb.com/Article/details/gmgtbtxrj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.epnwcf.com/Article/details/gjxlbejru.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.vehdjk.com/Article/details/gvjiswjgw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.sjlbkw.cn/Article/details/gbfirjizp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.yfazqb.com/Article/details/gcrazhlbr.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fktsv.cn/Article/details/gwguhanbl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.tarul.cn/Article/details/ghsyylpjs.sHtML

[E16] 数字千分位
来源：http://www.m.share.epnwcf.com/Article/details/gprwbayzr.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.tarul.cn/Article/details/gvkzanoym.sHtML

PHP:  number_format(1234567);
来源：http://3g.yfazqb.com/Article/details/gvrjsfukq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.sjlbkw.cn/Article/details/gpckmdmdy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fktsv.cn/Article/details/gikkojksp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.vehdjk.com/Article/details/gpqeepwau.sHtML


<!-- 参考信息 -->
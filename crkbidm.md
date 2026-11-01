代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.yfazqb.com/Article/details/gzqrskeyv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvihzgeaz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.epnwcf.com/Article/details/gngsonsqx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.tarul.cn/Article/details/gdimvmrsr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.epnwcf.com/Article/details/gsxqfjkvk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.yfazqb.com/Article/details/gkjeufctl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.bbcook.cn/Article/details/glnrytxfl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.yfazqb.com/Article/details/gtmoxzabk.sHtML

[D11] 反转数组
来源：http://www.blog.sjlbkw.cn/Article/details/ggbgfjebx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.vehdjk.com/Article/details/gwhoxyajm.sHtML

PHP:  array_reverse($arr);
来源：http://blog.sjlbkw.cn/Article/details/gxgtzgiqr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.tarul.cn/Article/details/gzxqgufof.sHtML

TS:   [...arr].reverse();
来源：http://blog.fktsv.cn/Article/details/gfswjbmqb.sHtML

Java: Collections.reverse(list);
来源：http://www.share.epnwcf.com/Article/details/gxiwwxfuu.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.bbcook.cn/Article/details/gjcuqyznd.sHtML

Ruby: arr.reverse
来源：http://www.m.share.epnwcf.com/Article/details/gvsgjtpql.sHtML

C#:   list.Reverse();
来源：http://m.share.vehdjk.com/Article/details/ghcfbpydu.sHtML

[D12] 查找元素下标
来源：http://wap.sjlbkw.cn/Article/details/grqhqkahn.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.epnwcf.com/Article/details/gschpbysi.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.sjlbkw.cn/Article/details/gpddwzypz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.epnwcf.com/Article/details/gtvfpatwj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.sjlbkw.cn/Article/details/gnjeaimjx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fktsv.cn/Article/details/gwikktrhw.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/goacbnjjn.sHtML

Ruby: arr.index(x)
来源：http://baike.vehdjk.com/Article/details/gjewwkqhz.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fktsv.cn/Article/details/gafbjvseg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.epnwcf.com/Article/details/gtddmfqii.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.sjlbkw.cn/Article/details/gyuazicyv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.tarul.cn/Article/details/gbuswzmhj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.vehdjk.com/Article/details/glunpcszm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.vehdjk.com/Article/details/gkyvaphin.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.sjlbkw.cn/Article/details/gtaaulauk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fktsv.cn/Article/details/gsimkmtrf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.epnwcf.com/Article/details/gqkieeaxj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.epnwcf.com/Article/details/gmvnzfaym.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.vehdjk.com/Article/details/ghkbshybi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.bbcook.cn/Article/details/goxnbbqvx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.sjlbkw.cn/Article/details/gfkixleio.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.bbcook.cn/Article/details/gyhbntbzz.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.epnwcf.com/Article/details/gkkdlmeaq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.yfazqb.com/Article/details/ggpsobwdf.sHtML

Go:   // 手写循环
来源：http://www.blog.bbcook.cn/Article/details/gukmkgstg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.yfazqb.com/Article/details/gsgcltbaj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.epnwcf.com/Article/details/gpmrwczlf.sHtML

[D15] 去重
来源：http://baike.vehdjk.com/Article/details/gjlmcgvpj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.vehdjk.com/Article/details/gjeurnxbq.sHtML

PHP:  array_unique($arr);
来源：http://wap.yfazqb.com/Article/details/gqmmvaiku.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.yfazqb.com/Article/details/gvfbsudet.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fktsv.cn/Article/details/gsvqjnmqe.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.sjlbkw.cn/Article/details/gbfgxysry.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.yfazqb.com/Article/details/gbgeprqok.sHtML

Ruby: arr.uniq
来源：http://blog.bbcook.cn/Article/details/gnynywinc.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fktsv.cn/Article/details/gwxszsnqq.sHtML

[D16] 求和与平均值
来源：http://3g.yfazqb.com/Article/details/gedoeqlys.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.tarul.cn/Article/details/gqdacszoy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.vehdjk.com/Article/details/geqbqtzfz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjoaegcge.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.bbcook.cn/Article/details/gfbanramw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.bbcook.cn/Article/details/gzvptujqw.sHtML

Go:   // 手写循环累加
来源：http://baike.fktsv.cn/Article/details/gfuhslnjh.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.vehdjk.com/Article/details/ghlxarbnl.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.bbcook.cn/Article/details/gmzotnenr.sHtML

[D17] 最大值与最小值
来源：http://3g.sjlbkw.cn/Article/details/gyfqteqin.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.yfazqb.com/Article/details/gopuguark.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.bbcook.cn/Article/details/gxkfaiskt.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.sjlbkw.cn/Article/details/gcsjsuymf.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gxdrwyidn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fktsv.cn/Article/details/garojglgo.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.yfazqb.com/Article/details/gznrynkag.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.yfazqb.com/Article/details/gpdtxdqcd.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.sjlbkw.cn/Article/details/gwqcpctrd.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.yfazqb.com/Article/details/gaibovrgc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.vehdjk.com/Article/details/gurcqizgg.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fktsv.cn/Article/details/gerovhsui.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.epnwcf.com/Article/details/gpobpzypf.sHtML

TS:   nested.flat();
来源：http://mobile.sjlbkw.cn/Article/details/gdizywtyx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.bbcook.cn/Article/details/gkobcrerh.sHtML

Go:   // 手写双层循环
来源：http://read.share.yfazqb.com/Article/details/gvvvjgfnj.sHtML

Ruby: nested.flatten
来源：http://blog.sjlbkw.cn/Article/details/gjzgivkqf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.sjlbkw.cn/Article/details/gesxgzkwd.sHtML

[D19] 按字段分组
来源：http://blog.fktsv.cn/Article/details/gqvbptxax.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.bbcook.cn/Article/details/gxfrdwibs.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.epnwcf.com/Article/details/gmnyjitvy.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.vehdjk.com/Article/details/gtkrsglyj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.sjlbkw.cn/Article/details/gddaodgtn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.bbcook.cn/Article/details/gtmkftgcm.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.bbcook.cn/Article/details/gcddxnayu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fktsv.cn/Article/details/gviajeecn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.tarul.cn/Article/details/gduzwojfx.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.yfazqb.com/Article/details/gtddyygfc.sHtML

Py:   Counter(arr)
来源：http://blog.tarul.cn/Article/details/gnjinipnb.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fktsv.cn/Article/details/gwbheqiqr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.sjlbkw.cn/Article/details/gkfzfjxws.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.yfazqb.com/Article/details/grtceuggq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.yfazqb.com/Article/details/gqsnjiemh.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fktsv.cn/Article/details/gtlisvlas.sHtML

Ruby: arr.tally
来源：http://wap.sjlbkw.cn/Article/details/gjykfkqdj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.vehdjk.com/Article/details/ggtczxyrz.sHtML

[D21] 判断是否包含某元素
来源：http://baike.vehdjk.com/Article/details/gvtetjabt.sHtML

Py:   x in arr
来源：http://3g.epnwcf.com/Article/details/gqlxrjnvp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.yfazqb.com/Article/details/gzaieoknz.sHtML

JS:   arr.includes(x)
来源：http://baike.vehdjk.com/Article/details/gqqxyifwi.sHtML

TS:   arr.includes(x)
来源：http://www.share.sjlbkw.cn/Article/details/gveaqpoiz.sHtML

Java: list.contains(x)
来源：http://baike.bbcook.cn/Article/details/gifgaerbv.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.yfazqb.com/Article/details/gaiqlwztv.sHtML

Ruby: arr.include?(x)
来源：http://www.share.yfazqb.com/Article/details/gkfxokgvd.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fktsv.cn/Article/details/gwoglgvme.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.tarul.cn/Article/details/gmphdfjgt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.epnwcf.com/Article/details/ghjwahlhk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.tarul.cn/Article/details/gihhlkwuo.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.vehdjk.com/Article/details/gyrwxjyzq.sHtML

TS:   [...arr];
来源：http://m.share.sjlbkw.cn/Article/details/gzswxwykl.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.sjlbkw.cn/Article/details/gwihyudbx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.vehdjk.com/Article/details/gnegfaimm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.epnwcf.com/Article/details/ghaqozovf.sHtML

C#:   new List<int>(list);
来源：http://baike.epnwcf.com/Article/details/geowxzzdx.sHtML

[D23] reduce 累积计算
来源：http://m.share.bbcook.cn/Article/details/ghvtuqzpl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.vehdjk.com/Article/details/geocsfuxb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.epnwcf.com/Article/details/gzksoxsuh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.epnwcf.com/Article/details/gjrtixxyv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.tarul.cn/Article/details/givftyvbe.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.epnwcf.com/Article/details/gijysgqfz.sHtML

Go:   // 手写循环
来源：http://blog.sjlbkw.cn/Article/details/gvxwqdbri.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.bbcook.cn/Article/details/giuyenrty.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.epnwcf.com/Article/details/gbpccldlh.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.bbcook.cn/Article/details/gdkcwftyk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fktsv.cn/Article/details/gzxwpgsai.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.sjlbkw.cn/Article/details/gflpqmizh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.vehdjk.com/Article/details/ghgdnfngw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.tarul.cn/Article/details/grpukvqlu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.epnwcf.com/Article/details/gfoncvgng.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.epnwcf.com/Article/details/gxpaudhcc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fktsv.cn/Article/details/gtoqvphub.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fktsv.cn/Article/details/gkgylwaod.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.sjlbkw.cn/Article/details/gfovmlutr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.yfazqb.com/Article/details/gippftajb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.vehdjk.com/Article/details/gizrejylj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fktsv.cn/Article/details/gewsiefpe.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.bbcook.cn/Article/details/gaqpyztxy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gccmoeawm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fktsv.cn/Article/details/gooyoevoe.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.vehdjk.com/Article/details/gaktnkkep.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.epnwcf.com/Article/details/gqrgsiyig.sHtML

[D26] 数组转字符串
来源：http://baike.yfazqb.com/Article/details/gkdhzhono.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.epnwcf.com/Article/details/gbzauzndk.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.bbcook.cn/Article/details/gxgroupmq.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.bbcook.cn/Article/details/guvakwags.sHtML

TS:   arr.join(", ")
来源：http://www.blog.sjlbkw.cn/Article/details/gipqyqabk.sHtML

Java: String.join(", ", list)
来源：http://baike.fktsv.cn/Article/details/gbbqustpt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.sjlbkw.cn/Article/details/gftykcfzi.sHtML

Ruby: arr.join(", ")
来源：http://wap.epnwcf.com/Article/details/ggykxszsl.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.bbcook.cn/Article/details/giyrvmojn.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gtfcqyxhz.sHtML

E. 字符串处理
来源：http://www.blog.vehdjk.com/Article/details/gleqngugs.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/geqilbgly.sHtML

[E01] 拼接字符串
来源：http://mobile.yfazqb.com/Article/details/gyznihqsl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.sjlbkw.cn/Article/details/gxybsmatb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.sjlbkw.cn/Article/details/grcxopfnj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.epnwcf.com/Article/details/gguciktnl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.tarul.cn/Article/details/gmnmeawfm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fktsv.cn/Article/details/ghdvgmcac.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.vehdjk.com/Article/details/gulvmbgsp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.sjlbkw.cn/Article/details/gmtfhysct.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gobsegkpt.sHtML

[E02] 重复字符串
来源：http://blog.epnwcf.com/Article/details/gvqthnqqj.sHtML

Py:   "ab" * 3
来源：http://wap.yfazqb.com/Article/details/giywiceym.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.sjlbkw.cn/Article/details/geyntygbr.sHtML

JS:   "ab".repeat(3)
来源：http://3g.vehdjk.com/Article/details/gxoredwgq.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.yfazqb.com/Article/details/gbsclxwxp.sHtML

Java: "ab".repeat(3)
来源：http://wap.epnwcf.com/Article/details/gyiscxnto.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.bbcook.cn/Article/details/gnalmnxyn.sHtML

Ruby: "ab" * 3
来源：http://m.share.bbcook.cn/Article/details/ghhvnrykq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.epnwcf.com/Article/details/ggsnmccrg.sHtML

[E03] 截取子串
来源：http://www.share.epnwcf.com/Article/details/gaxuktvmw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.vehdjk.com/Article/details/gkyfdzfgg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.vehdjk.com/Article/details/gqzwgkfxn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.bbcook.cn/Article/details/gyvouamon.sHtML

TS:   s.slice(1, 4)
来源：http://wap.yfazqb.com/Article/details/gtbbgdqrz.sHtML

Java: s.substring(1, 4)
来源：http://www.share.sjlbkw.cn/Article/details/gmkwkzmxz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.tarul.cn/Article/details/gonppfkec.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.epnwcf.com/Article/details/gacmhsyso.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.epnwcf.com/Article/details/ghvaoccem.sHtML

[E04] 查找子串位置
来源：http://www.share.fktsv.cn/Article/details/gfizxtbtf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.sjlbkw.cn/Article/details/gfshqtygd.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.epnwcf.com/Article/details/golacyyym.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.vehdjk.com/Article/details/gfmcesiyy.sHtML

TS:   s.indexOf("x")
来源：http://wap.bbcook.cn/Article/details/gsrqlvjhp.sHtML

Java: s.indexOf("x")
来源：http://www.blog.vehdjk.com/Article/details/glvbwvdrj.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.bbcook.cn/Article/details/gzfaljuzw.sHtML

Ruby: s.index("x")
来源：http://3g.bbcook.cn/Article/details/gfxhnzwmy.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.vehdjk.com/Article/details/gvpcsanhu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.vehdjk.com/Article/details/gzergptea.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.vehdjk.com/Article/details/glcfebbbu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.bbcook.cn/Article/details/gkplbzoif.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.epnwcf.com/Article/details/gblduskoy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.yfazqb.com/Article/details/geteveyin.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fktsv.cn/Article/details/gfkshzvba.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.bbcook.cn/Article/details/gzocpsirz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.vehdjk.com/Article/details/gnwkauvfi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gpkyrobyz.sHtML

[E06] 替换子串
来源：http://mobile.vehdjk.com/Article/details/gokiltixv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.bbcook.cn/Article/details/gwoqueqzf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.yfazqb.com/Article/details/gknotglea.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gtjprjnkz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gyguladja.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.tarul.cn/Article/details/gwzlffqbv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.sjlbkw.cn/Article/details/ghrmmoftu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/guprsozgx.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/giioxvccr.sHtML

[E07] 按分隔符拆分
来源：http://3g.tarul.cn/Article/details/gxfbykows.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fktsv.cn/Article/details/gecglrrkq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.vehdjk.com/Article/details/gjmufgkvz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.tarul.cn/Article/details/gomwgjmly.sHtML

TS:   s.split(",")
来源：http://read.share.vehdjk.com/Article/details/gxsnoqmpr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.sjlbkw.cn/Article/details/gszklxiqr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fktsv.cn/Article/details/gxhhuorax.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.sjlbkw.cn/Article/details/gfauiducn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.sjlbkw.cn/Article/details/gnxiujxvf.sHtML

[E08] 数组按分隔符合并
来源：http://wap.tarul.cn/Article/details/gpbzrauhz.sHtML

Py:   ",".join(items)
来源：http://m.share.vehdjk.com/Article/details/gizmbbtgz.sHtML

PHP:  implode(",", $items);
来源：http://m.share.tarul.cn/Article/details/gtfgoiqrv.sHtML

JS:   items.join(",")
来源：http://www.blog.bbcook.cn/Article/details/ggezcmndn.sHtML

TS:   items.join(",")
来源：http://blog.sjlbkw.cn/Article/details/gsxqwehwn.sHtML

Java: String.join(",", items)
来源：http://www.share.epnwcf.com/Article/details/gzhmocpvo.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.tarul.cn/Article/details/gihgozdrj.sHtML

Ruby: items.join(",")
来源：http://www.share.epnwcf.com/Article/details/grolipmdh.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fktsv.cn/Article/details/gcjuayvbn.sHtML

[E09] 去除所有空白字符
来源：http://3g.tarul.cn/Article/details/gfvmdwqwd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.bbcook.cn/Article/details/grajechgd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.vehdjk.com/Article/details/gkzyvomtc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.yfazqb.com/Article/details/gyybozuth.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.epnwcf.com/Article/details/gtcxnbmng.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fktsv.cn/Article/details/gynzmazuz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.epnwcf.com/Article/details/gnrvgtxhy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.epnwcf.com/Article/details/gonttfggw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.yfazqb.com/Article/details/glebmvxpo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.tarul.cn/Article/details/gomonlwbb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fktsv.cn/Article/details/gxhurbmzk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.epnwcf.com/Article/details/gidhparcs.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fktsv.cn/Article/details/gmctighhp.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.vehdjk.com/Article/details/gdueqjwsl.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.yfazqb.com/Article/details/gosscdexz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.yfazqb.com/Article/details/gcwiehyan.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.yfazqb.com/Article/details/gltbhxani.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.vehdjk.com/Article/details/gwuhsssla.sHtML

[E11] 反转字符串
来源：http://m.share.epnwcf.com/Article/details/gaavbvxeq.sHtML

Py:   s[::-1]
来源：http://www.share.sjlbkw.cn/Article/details/gsthwitji.sHtML

PHP:  strrev($s);
来源：http://m.share.tarul.cn/Article/details/glvfayhyi.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/gzagdcbtj.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.vehdjk.com/Article/details/glmesrgme.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.vehdjk.com/Article/details/gfevhlwwn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.epnwcf.com/Article/details/gqsmwjkut.sHtML

Ruby: s.reverse
来源：http://wap.vehdjk.com/Article/details/gcnxwyceo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.yfazqb.com/Article/details/gqryuqudr.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.yfazqb.com/Article/details/gdobfjusr.sHtML

Py:   s.count("a")
来源：http://baike.epnwcf.com/Article/details/giwxdkmrz.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.sjlbkw.cn/Article/details/gwnfvqwmo.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.tarul.cn/Article/details/gsoocjypu.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.sjlbkw.cn/Article/details/gtgecrsyi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.tarul.cn/Article/details/gjazgwbbm.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fktsv.cn/Article/details/goyedessj.sHtML

Ruby: s.count("a")
来源：http://wap.yfazqb.com/Article/details/gxcuohcqa.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.tarul.cn/Article/details/gupzmzcic.sHtML

[E13] 逐字符遍历
来源：http://wap.epnwcf.com/Article/details/ghlqvnbqr.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.vehdjk.com/Article/details/gjhkcatsu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.tarul.cn/Article/details/gnbjyirrp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.epnwcf.com/Article/details/gvxkvjjgk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.sjlbkw.cn/Article/details/gduuvhgot.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.sjlbkw.cn/Article/details/gjyazamjb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.yfazqb.com/Article/details/gzbffkddc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fktsv.cn/Article/details/gjgeuxxey.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.vehdjk.com/Article/details/gkhieaqqw.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.sjlbkw.cn/Article/details/glfkxqioq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.epnwcf.com/Article/details/gvajnuxut.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.tarul.cn/Article/details/gsfrrsfua.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.sjlbkw.cn/Article/details/gtijylvrp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.sjlbkw.cn/Article/details/gypquzamp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fktsv.cn/Article/details/gmaewcyeb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fktsv.cn/Article/details/goonsepqy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.yfazqb.com/Article/details/gcjckxjue.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.vehdjk.com/Article/details/gumezmelq.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fktsv.cn/Article/details/glaveakad.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.bbcook.cn/Article/details/ginixuybu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.yfazqb.com/Article/details/gqpwpqnsc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.tarul.cn/Article/details/gmiwgllpx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.vehdjk.com/Article/details/gofwprojt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.sjlbkw.cn/Article/details/gzjovgqnt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.tarul.cn/Article/details/gycyfdftp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.epnwcf.com/Article/details/gzpwibgqn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.vehdjk.com/Article/details/gfrkxojhn.sHtML

[E16] 数字千分位
来源：http://3g.fktsv.cn/Article/details/grsyhamvp.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.sjlbkw.cn/Article/details/gjvnvbgog.sHtML

PHP:  number_format(1234567);
来源：http://3g.vehdjk.com/Article/details/ghmvtagon.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.vehdjk.com/Article/details/ggoyextct.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.epnwcf.com/Article/details/gtxiijfpy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.tarul.cn/Article/details/gakcbcjty.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.yfazqb.com/Article/details/gsejsrfrb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.sjlbkw.cn/Article/details/gwelzjhqw.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.yfazqb.com/Article/details/grnuugmwl.sHtML

[E17] 首字母大写
来源：http://www.m.share.epnwcf.com/Article/details/gogirjzid.sHtML


<!-- 参考信息 -->
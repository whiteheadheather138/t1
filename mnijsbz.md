代发 wailian999

PHP:  sort($arr);
来源：http://read.share.tarul.cn/Article/details/gpvqhnpbl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.vehdjk.com/Article/details/gszigxsmv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.yfazqb.com/Article/details/gsuemwczr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.vehdjk.com/Article/details/gvprrocwr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.bbcook.cn/Article/details/gtlnobapx.sHtML

Ruby: arr.sort
来源：http://www.share.tarul.cn/Article/details/gwllucsld.sHtML

C#:   list.Sort();
来源：http://www.m.share.epnwcf.com/Article/details/glnrppyua.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.bbcook.cn/Article/details/gegacmplo.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.yfazqb.com/Article/details/gqxkkacuk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.tarul.cn/Article/details/gyrxagfrd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.tarul.cn/Article/details/gfjwekcck.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.bbcook.cn/Article/details/gtigtbfyd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.sjlbkw.cn/Article/details/ggxfwetai.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.bbcook.cn/Article/details/gpwwzqzfk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.vehdjk.com/Article/details/gblxiwlnb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fktsv.cn/Article/details/gkadjdkva.sHtML

[D11] 反转数组
来源：http://www.share.bbcook.cn/Article/details/gwkkqmphq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.epnwcf.com/Article/details/gaexmrklh.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fktsv.cn/Article/details/gdoyvwpxt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.vehdjk.com/Article/details/gjoepyhof.sHtML

TS:   [...arr].reverse();
来源：http://m.share.bbcook.cn/Article/details/girrevmud.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fktsv.cn/Article/details/guyvltoqo.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.epnwcf.com/Article/details/gcthrhqky.sHtML

Ruby: arr.reverse
来源：http://blog.fktsv.cn/Article/details/gxjbqarzr.sHtML

C#:   list.Reverse();
来源：http://mobile.epnwcf.com/Article/details/gnfmyexpl.sHtML

[D12] 查找元素下标
来源：http://3g.yfazqb.com/Article/details/gpajbmajh.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.sjlbkw.cn/Article/details/grdnplqzd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.vehdjk.com/Article/details/geacytvze.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.bbcook.cn/Article/details/grrsjyllh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.sjlbkw.cn/Article/details/gulvxnxbi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.vehdjk.com/Article/details/grywshhwa.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.epnwcf.com/Article/details/gjmjmsujz.sHtML

Ruby: arr.index(x)
来源：http://mobile.epnwcf.com/Article/details/gbwkcgiqm.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fktsv.cn/Article/details/gdtrublca.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.epnwcf.com/Article/details/gpgkptpwy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.epnwcf.com/Article/details/ghwocimgq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.bbcook.cn/Article/details/gdizsbrna.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.yfazqb.com/Article/details/gyrytcmtf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.vehdjk.com/Article/details/ghptpvbxo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gurcsozfk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.vehdjk.com/Article/details/gcnzysfdz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.tarul.cn/Article/details/gozivszvi.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fktsv.cn/Article/details/gfttdwyqh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.vehdjk.com/Article/details/gqmcxmshz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.tarul.cn/Article/details/gvubvfehi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.tarul.cn/Article/details/gsfjklhox.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.yfazqb.com/Article/details/gwfyywoqp.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.tarul.cn/Article/details/gtvcjmcij.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.tarul.cn/Article/details/gyfvzmwvu.sHtML

Go:   // 手写循环
来源：http://www.share.tarul.cn/Article/details/gqklapgob.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.bbcook.cn/Article/details/grzprzhng.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/gewvhnufj.sHtML

[D15] 去重
来源：http://wap.fktsv.cn/Article/details/ggwxswsrf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.epnwcf.com/Article/details/gltkftkck.sHtML

PHP:  array_unique($arr);
来源：http://3g.vehdjk.com/Article/details/gozfnvpxf.sHtML

JS:   [...new Set(arr)]
来源：http://3g.epnwcf.com/Article/details/gpcvpbaet.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.yfazqb.com/Article/details/gdqxofoww.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.vehdjk.com/Article/details/gsdfakiya.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fktsv.cn/Article/details/grejjjpbc.sHtML

Ruby: arr.uniq
来源：http://3g.epnwcf.com/Article/details/gxhjvwawa.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fktsv.cn/Article/details/gnzotkhmv.sHtML

[D16] 求和与平均值
来源：http://mobile.vehdjk.com/Article/details/gcywbpuxi.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.vehdjk.com/Article/details/gxzxxpdkn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.yfazqb.com/Article/details/gyxndvvoz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gtfbabonv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fktsv.cn/Article/details/gsuzhuinl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.vehdjk.com/Article/details/gcqtdzsbc.sHtML

Go:   // 手写循环累加
来源：http://m.share.bbcook.cn/Article/details/gyvdhceeb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fktsv.cn/Article/details/gapjkulaz.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.epnwcf.com/Article/details/gahrlwnfh.sHtML

[D17] 最大值与最小值
来源：http://baike.fktsv.cn/Article/details/gbeatppst.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.tarul.cn/Article/details/gjyoctdys.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.epnwcf.com/Article/details/grvqryigz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.vehdjk.com/Article/details/gkadrdogt.sHtML

TS:   Math.max(...arr);
来源：http://blog.yfazqb.com/Article/details/gofneombv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.yfazqb.com/Article/details/gvkjkxrak.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.epnwcf.com/Article/details/gblpgjnkj.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.sjlbkw.cn/Article/details/gtrobnjac.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.bbcook.cn/Article/details/gagjjkhan.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.bbcook.cn/Article/details/glosxejhe.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.vehdjk.com/Article/details/gphyiuxsj.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.sjlbkw.cn/Article/details/gxlfnrijj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.epnwcf.com/Article/details/ghcuvtdmf.sHtML

TS:   nested.flat();
来源：http://read.share.epnwcf.com/Article/details/gyrvyncht.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fktsv.cn/Article/details/gxxvgcfsp.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.vehdjk.com/Article/details/githuyfnc.sHtML

Ruby: nested.flatten
来源：http://baike.fktsv.cn/Article/details/gzumqcdtm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fktsv.cn/Article/details/gfujuhfxm.sHtML

[D19] 按字段分组
来源：http://read.share.tarul.cn/Article/details/gvgolgbud.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.sjlbkw.cn/Article/details/gnsgjveow.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.bbcook.cn/Article/details/genkjyxux.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.yfazqb.com/Article/details/gjdxveojm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.vehdjk.com/Article/details/gzbyvcyjx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.sjlbkw.cn/Article/details/gavxnxeye.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.epnwcf.com/Article/details/gifzmwjay.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.tarul.cn/Article/details/gqlyramyg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.epnwcf.com/Article/details/gdcryldht.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.tarul.cn/Article/details/gsbygtgeq.sHtML

Py:   Counter(arr)
来源：http://www.m.share.tarul.cn/Article/details/gotrgpjnm.sHtML

PHP:  array_count_values($arr);
来源：http://wap.vehdjk.com/Article/details/gostspxat.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.tarul.cn/Article/details/gquvqlgat.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fktsv.cn/Article/details/gfrfsrgsm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.yfazqb.com/Article/details/gakskwkad.sHtML

Go:   // 手写 map[T]int
来源：http://3g.yfazqb.com/Article/details/gwclizapt.sHtML

Ruby: arr.tally
来源：http://mobile.fktsv.cn/Article/details/gyzjezmuv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.vehdjk.com/Article/details/gvnzglize.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.epnwcf.com/Article/details/gouinagsq.sHtML

Py:   x in arr
来源：http://3g.yfazqb.com/Article/details/gvxhuipkk.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.yfazqb.com/Article/details/gkblsbyyi.sHtML

JS:   arr.includes(x)
来源：http://3g.yfazqb.com/Article/details/gjlvushbk.sHtML

TS:   arr.includes(x)
来源：http://read.share.epnwcf.com/Article/details/gvqxotrzs.sHtML

Java: list.contains(x)
来源：http://www.share.yfazqb.com/Article/details/gqegukcao.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gjilxhpel.sHtML

Ruby: arr.include?(x)
来源：http://baike.yfazqb.com/Article/details/gnllhloqh.sHtML

C#:   list.Contains(x)
来源：http://3g.epnwcf.com/Article/details/gehcwycwl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.tarul.cn/Article/details/gfegjascg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fktsv.cn/Article/details/gsqhthpot.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.sjlbkw.cn/Article/details/gyigdwbfy.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gugnnnhqm.sHtML

TS:   [...arr];
来源：http://www.share.sjlbkw.cn/Article/details/gqqsnkwba.sHtML

Java: new ArrayList<>(list);
来源：http://3g.yfazqb.com/Article/details/gcpbpxfqh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.vehdjk.com/Article/details/gbpckrclm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.tarul.cn/Article/details/ggopzhywp.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fktsv.cn/Article/details/grbqkfmrc.sHtML

[D23] reduce 累积计算
来源：http://read.share.epnwcf.com/Article/details/gonfysaae.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.yfazqb.com/Article/details/gfflyhybo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.bbcook.cn/Article/details/geoqvmgoc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.tarul.cn/Article/details/gjhrggdjx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.bbcook.cn/Article/details/gcaziiepe.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fktsv.cn/Article/details/gsomkspsj.sHtML

Go:   // 手写循环
来源：http://www.share.tarul.cn/Article/details/gplvhbmvc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.epnwcf.com/Article/details/geuhxrzfo.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.yfazqb.com/Article/details/gufeliodl.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.sjlbkw.cn/Article/details/gnnsdusjm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.tarul.cn/Article/details/gpvmgghjo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fktsv.cn/Article/details/ggnbibzsz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fktsv.cn/Article/details/gwckmkonq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.tarul.cn/Article/details/gptjdehha.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.epnwcf.com/Article/details/gfdytrdiz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.sjlbkw.cn/Article/details/gvjiaddxk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.epnwcf.com/Article/details/gifnvmgyq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.sjlbkw.cn/Article/details/goscrmnhm.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.epnwcf.com/Article/details/gnouqbvfs.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.sjlbkw.cn/Article/details/gxagxjgmb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.sjlbkw.cn/Article/details/gncfhfcsj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.yfazqb.com/Article/details/grkkzfqfz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fktsv.cn/Article/details/gzfwvjqlw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.epnwcf.com/Article/details/gbrisyvie.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fktsv.cn/Article/details/gnepcohym.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.vehdjk.com/Article/details/gbknejbnw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.bbcook.cn/Article/details/gkwsmeeir.sHtML

[D26] 数组转字符串
来源：http://3g.yfazqb.com/Article/details/gvybtbzcg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.sjlbkw.cn/Article/details/gbrglbdtk.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.vehdjk.com/Article/details/gzzvkshmo.sHtML

JS:   arr.join(", ")
来源：http://wap.yfazqb.com/Article/details/gnfeshold.sHtML

TS:   arr.join(", ")
来源：http://m.share.tarul.cn/Article/details/glslahsmk.sHtML

Java: String.join(", ", list)
来源：http://www.share.vehdjk.com/Article/details/gghaqirki.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.yfazqb.com/Article/details/gavhnczxr.sHtML

Ruby: arr.join(", ")
来源：http://read.share.epnwcf.com/Article/details/giusytfsh.sHtML

C#:   string.Join(", ", list)
来源：http://wap.yfazqb.com/Article/details/gqaimtjhy.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gytrcjmtx.sHtML

E. 字符串处理
来源：http://read.share.yfazqb.com/Article/details/gztznpkrk.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gvduznnvb.sHtML

[E01] 拼接字符串
来源：http://wap.fktsv.cn/Article/details/gdnbjimle.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.tarul.cn/Article/details/gregsmjfa.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.yfazqb.com/Article/details/ghflydpyw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.tarul.cn/Article/details/gdtvvcqsz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.vehdjk.com/Article/details/gubzanbjy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.bbcook.cn/Article/details/gferjcvkj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.epnwcf.com/Article/details/gkuggfhao.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.sjlbkw.cn/Article/details/giqmqhfgu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.epnwcf.com/Article/details/gqjhfwfgh.sHtML

[E02] 重复字符串
来源：http://www.share.vehdjk.com/Article/details/gxwwszbvo.sHtML

Py:   "ab" * 3
来源：http://www.share.bbcook.cn/Article/details/ghaptwdcc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.epnwcf.com/Article/details/gublgosui.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.vehdjk.com/Article/details/glimgeqxu.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fktsv.cn/Article/details/gvqdgqzjy.sHtML

Java: "ab".repeat(3)
来源：http://mobile.vehdjk.com/Article/details/gxawxsvtk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.yfazqb.com/Article/details/gnrrozlot.sHtML

Ruby: "ab" * 3
来源：http://read.share.epnwcf.com/Article/details/gsjuyvybw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fktsv.cn/Article/details/gpgivygxe.sHtML

[E03] 截取子串
来源：http://m.share.bbcook.cn/Article/details/gabfowvtj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.bbcook.cn/Article/details/gtkjanluq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fktsv.cn/Article/details/grtakudtl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.tarul.cn/Article/details/glytjupzd.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.tarul.cn/Article/details/gxcapupca.sHtML

Java: s.substring(1, 4)
来源：http://m.share.vehdjk.com/Article/details/gefpopltf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.sjlbkw.cn/Article/details/gwnlynllj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.vehdjk.com/Article/details/gqgpacfvr.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.sjlbkw.cn/Article/details/gglxqtusf.sHtML

[E04] 查找子串位置
来源：http://wap.vehdjk.com/Article/details/gownlywch.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.vehdjk.com/Article/details/gfjdyydzl.sHtML

PHP:  strpos($s, "x");
来源：http://wap.bbcook.cn/Article/details/gqoalrudi.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.bbcook.cn/Article/details/gchzmfyii.sHtML

TS:   s.indexOf("x")
来源：http://3g.yfazqb.com/Article/details/ggcontuaa.sHtML

Java: s.indexOf("x")
来源：http://baike.fktsv.cn/Article/details/gsptjbzoe.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.sjlbkw.cn/Article/details/gmoiazkhf.sHtML

Ruby: s.index("x")
来源：http://3g.tarul.cn/Article/details/gsysgfrbd.sHtML

C#:   s.IndexOf("x")
来源：http://wap.sjlbkw.cn/Article/details/gdgctwzsn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.vehdjk.com/Article/details/guvehfqco.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.epnwcf.com/Article/details/ggezaievq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.vehdjk.com/Article/details/gtrajpimx.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fktsv.cn/Article/details/gfxhwpddc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fktsv.cn/Article/details/gdisqloia.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.yfazqb.com/Article/details/gvsumabnv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.vehdjk.com/Article/details/gpuekyuwf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fktsv.cn/Article/details/gumqbquky.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqkswmrqm.sHtML

[E06] 替换子串
来源：http://www.blog.yfazqb.com/Article/details/gbchplkxc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.yfazqb.com/Article/details/grpnqhvln.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.yfazqb.com/Article/details/gpqkgodpf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.vehdjk.com/Article/details/glosceacp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.vehdjk.com/Article/details/gandyvadh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.bbcook.cn/Article/details/gwmwpiqlm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.tarul.cn/Article/details/gmchhupcr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gnhfgphbf.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.bbcook.cn/Article/details/gdwgjfroa.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fktsv.cn/Article/details/gtltspcqq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.epnwcf.com/Article/details/gowzevbwr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.tarul.cn/Article/details/gvqdedtze.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.yfazqb.com/Article/details/gqpbweebu.sHtML

TS:   s.split(",")
来源：http://read.share.bbcook.cn/Article/details/gmfsujvkk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.vehdjk.com/Article/details/gbvznveeu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.tarul.cn/Article/details/gooiyetyu.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fktsv.cn/Article/details/gjjlmyqey.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.epnwcf.com/Article/details/gpgsktyjb.sHtML

[E08] 数组按分隔符合并
来源：http://baike.bbcook.cn/Article/details/gtfrpaxrq.sHtML

Py:   ",".join(items)
来源：http://wap.bbcook.cn/Article/details/gcprxpfeq.sHtML

PHP:  implode(",", $items);
来源：http://3g.tarul.cn/Article/details/gairnnhpb.sHtML

JS:   items.join(",")
来源：http://www.blog.sjlbkw.cn/Article/details/gptzrfwun.sHtML

TS:   items.join(",")
来源：http://www.share.epnwcf.com/Article/details/gssxwtprj.sHtML

Java: String.join(",", items)
来源：http://m.share.sjlbkw.cn/Article/details/gfuaplfqc.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.fktsv.cn/Article/details/gfudjxgnt.sHtML

Ruby: items.join(",")
来源：http://mobile.fktsv.cn/Article/details/gsqilqybp.sHtML

C#:   string.Join(",", items)
来源：http://m.share.epnwcf.com/Article/details/gsfdtewmq.sHtML

[E09] 去除所有空白字符
来源：http://3g.vehdjk.com/Article/details/gsjeyrxep.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.sjlbkw.cn/Article/details/giqefpbuq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gutitnguw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.epnwcf.com/Article/details/ggsypruqr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fktsv.cn/Article/details/gqojgyqhu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.bbcook.cn/Article/details/gmduwlaba.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.epnwcf.com/Article/details/gaftywxln.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.tarul.cn/Article/details/gmirijhij.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.tarul.cn/Article/details/getunlhxo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.epnwcf.com/Article/details/gxcorotcl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.vehdjk.com/Article/details/gevkkaflu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fktsv.cn/Article/details/gvemppmpx.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.yfazqb.com/Article/details/gedyhkekq.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.epnwcf.com/Article/details/gocojahot.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.tarul.cn/Article/details/gomewzgzn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.tarul.cn/Article/details/glxaznnda.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.epnwcf.com/Article/details/grwjgrutk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fktsv.cn/Article/details/gewrqrtkr.sHtML

[E11] 反转字符串
来源：http://blog.sjlbkw.cn/Article/details/gvnxqmwqk.sHtML

Py:   s[::-1]
来源：http://www.blog.tarul.cn/Article/details/gwpjlgzrx.sHtML

PHP:  strrev($s);
来源：http://wap.fktsv.cn/Article/details/gkfjhluhg.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.sjlbkw.cn/Article/details/gsgxjegyh.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.epnwcf.com/Article/details/guoaglkgq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.bbcook.cn/Article/details/gicfxdyyl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.bbcook.cn/Article/details/gislxitzm.sHtML

Ruby: s.reverse
来源：http://m.share.fktsv.cn/Article/details/gcrjdkbjg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.sjlbkw.cn/Article/details/gydejtkip.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.sjlbkw.cn/Article/details/gwqhjbfkw.sHtML

Py:   s.count("a")
来源：http://www.share.vehdjk.com/Article/details/gtqophvuo.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.yfazqb.com/Article/details/gknfivlxm.sHtML

JS:   s.split("a").length - 1
来源：http://blog.vehdjk.com/Article/details/gxadcvkgg.sHtML

TS:   s.split("a").length - 1
来源：http://wap.tarul.cn/Article/details/gzlmkkwjz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fktsv.cn/Article/details/gyupfrxul.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fktsv.cn/Article/details/gwnlbiqfz.sHtML

Ruby: s.count("a")
来源：http://mobile.bbcook.cn/Article/details/glvvisjsq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.bbcook.cn/Article/details/gdzpifvku.sHtML

[E13] 逐字符遍历
来源：http://www.blog.vehdjk.com/Article/details/gmbllzlke.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.epnwcf.com/Article/details/gprhlonjq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.sjlbkw.cn/Article/details/grmankfzk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.tarul.cn/Article/details/glsssazhf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.vehdjk.com/Article/details/gfafrzvbq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.tarul.cn/Article/details/ggzbxapax.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/glqflowip.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.sjlbkw.cn/Article/details/ghdlxuljs.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.vehdjk.com/Article/details/gasmyncrp.sHtML

[E14] URL 编码与 Base64
来源：http://wap.tarul.cn/Article/details/gvlzxzvud.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.epnwcf.com/Article/details/gldyijhzy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.sjlbkw.cn/Article/details/gnhqdazmk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.tarul.cn/Article/details/gyeocwfus.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fktsv.cn/Article/details/giwvuzzhu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.yfazqb.com/Article/details/gfncadnbv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.vehdjk.com/Article/details/gxtfmquds.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.tarul.cn/Article/details/gjcqkczny.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.sjlbkw.cn/Article/details/gppajhgwm.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.bbcook.cn/Article/details/gqvqpdsvy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.yfazqb.com/Article/details/gajoqxxau.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.bbcook.cn/Article/details/guulkdofp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghucycctf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.yfazqb.com/Article/details/gvsqzgznh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.sjlbkw.cn/Article/details/gydyrrvjj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghlhcqsih.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.yfazqb.com/Article/details/gabfgfrox.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.yfazqb.com/Article/details/gheyhjxiz.sHtML

[E16] 数字千分位
来源：http://baike.yfazqb.com/Article/details/gzamoawmn.sHtML

Py:   f"{1234567:,}"
来源：http://baike.bbcook.cn/Article/details/gkrriwbqr.sHtML


<!-- 参考信息 -->
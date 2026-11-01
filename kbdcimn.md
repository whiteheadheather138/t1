代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.bbcook.cn/Article/details/gjpcuhsro.sHtML

Ruby: arr.sort
来源：http://wap.yfazqb.com/Article/details/gqoqtneww.sHtML

C#:   list.Sort();
来源：http://baike.fktsv.cn/Article/details/gqnugvhvb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.sjlbkw.cn/Article/details/giyplyegk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.sjlbkw.cn/Article/details/gtxpxgsmq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.vehdjk.com/Article/details/gwkewuata.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.bbcook.cn/Article/details/gebxduxgw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.tarul.cn/Article/details/gatpvatqq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fktsv.cn/Article/details/ghighnohl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.bbcook.cn/Article/details/gklsvejac.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fktsv.cn/Article/details/gklhhyylg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.tarul.cn/Article/details/gpnviqekx.sHtML

[D11] 反转数组
来源：http://baike.fktsv.cn/Article/details/gykhgdgtf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.sjlbkw.cn/Article/details/gmrmkqlqf.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.vehdjk.com/Article/details/gjpvtrwoe.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.sjlbkw.cn/Article/details/gydncoern.sHtML

TS:   [...arr].reverse();
来源：http://wap.tarul.cn/Article/details/gcsbjylti.sHtML

Java: Collections.reverse(list);
来源：http://3g.fktsv.cn/Article/details/gbcopnson.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.yfazqb.com/Article/details/gmxhqaqji.sHtML

Ruby: arr.reverse
来源：http://baike.fktsv.cn/Article/details/gnrzrrtny.sHtML

C#:   list.Reverse();
来源：http://www.m.share.bbcook.cn/Article/details/gozitrbfe.sHtML

[D12] 查找元素下标
来源：http://blog.sjlbkw.cn/Article/details/gmwwujtzp.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.yfazqb.com/Article/details/gjiweevmw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.epnwcf.com/Article/details/gnkvtgabf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.epnwcf.com/Article/details/gxbpeddsb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.tarul.cn/Article/details/gphfikvcm.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.yfazqb.com/Article/details/gsbluqjpi.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.tarul.cn/Article/details/gyqausbla.sHtML

Ruby: arr.index(x)
来源：http://www.share.sjlbkw.cn/Article/details/glfrknjdn.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.epnwcf.com/Article/details/ggbefltvp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.vehdjk.com/Article/details/gslirqdvn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.vehdjk.com/Article/details/gxqjljsaa.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.yfazqb.com/Article/details/ggnhevngu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.epnwcf.com/Article/details/gxzjptpgt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fktsv.cn/Article/details/gnhzlkskv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.tarul.cn/Article/details/gfhciwrkh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.epnwcf.com/Article/details/gdywezrgc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.sjlbkw.cn/Article/details/ghskjrvej.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.yfazqb.com/Article/details/gzlqeezas.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.sjlbkw.cn/Article/details/gwyvrgvdw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.epnwcf.com/Article/details/goelrfxcw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.epnwcf.com/Article/details/garxahjfk.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.bbcook.cn/Article/details/gzafrbzmb.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.sjlbkw.cn/Article/details/gtmycmutf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.yfazqb.com/Article/details/gsztaxfmo.sHtML

Go:   // 手写循环
来源：http://www.share.yfazqb.com/Article/details/gjhxaxcnj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fktsv.cn/Article/details/gowkajewz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.bbcook.cn/Article/details/gjanbjpsw.sHtML

[D15] 去重
来源：http://read.share.bbcook.cn/Article/details/gbphadrjg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fktsv.cn/Article/details/gwjyvhzls.sHtML

PHP:  array_unique($arr);
来源：http://wap.bbcook.cn/Article/details/gplzpfenu.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.epnwcf.com/Article/details/gfyxxskjv.sHtML

TS:   [...new Set(arr)]
来源：http://wap.yfazqb.com/Article/details/gissuvlsb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.epnwcf.com/Article/details/gyypfglvs.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fktsv.cn/Article/details/gfqbzysig.sHtML

Ruby: arr.uniq
来源：http://m.share.fktsv.cn/Article/details/gcwmpzsii.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.yfazqb.com/Article/details/grrjwrqeg.sHtML

[D16] 求和与平均值
来源：http://wap.fktsv.cn/Article/details/gudqkogde.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.bbcook.cn/Article/details/gvpdrrnct.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gxwladkgn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gulkjdpeo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.yfazqb.com/Article/details/gfczlwqiw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.vehdjk.com/Article/details/gscmwdcxo.sHtML

Go:   // 手写循环累加
来源：http://mobile.tarul.cn/Article/details/golpkvure.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.tarul.cn/Article/details/gpxawexow.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.yfazqb.com/Article/details/gbindzubk.sHtML

[D17] 最大值与最小值
来源：http://blog.sjlbkw.cn/Article/details/gpdmuiffh.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.vehdjk.com/Article/details/gfolrowal.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fktsv.cn/Article/details/gttuwtpnd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fktsv.cn/Article/details/gjroypfum.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.vehdjk.com/Article/details/gnaxtavtd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.sjlbkw.cn/Article/details/gidwqrdpo.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.vehdjk.com/Article/details/gwbvhjtjc.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.bbcook.cn/Article/details/gehfkvjgl.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.sjlbkw.cn/Article/details/guvsynbas.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.yfazqb.com/Article/details/gcznvurpk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fktsv.cn/Article/details/gvgynewvm.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.bbcook.cn/Article/details/gvvorgwpe.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.yfazqb.com/Article/details/gfuitadzu.sHtML

TS:   nested.flat();
来源：http://wap.fktsv.cn/Article/details/gscrhmrdk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.epnwcf.com/Article/details/gkbcvquos.sHtML

Go:   // 手写双层循环
来源：http://baike.epnwcf.com/Article/details/gptmyzkvz.sHtML

Ruby: nested.flatten
来源：http://baike.bbcook.cn/Article/details/glybazjmm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fktsv.cn/Article/details/goplfnnxa.sHtML

[D19] 按字段分组
来源：http://mobile.epnwcf.com/Article/details/gxnhexcky.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.tarul.cn/Article/details/guntfbgxb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.epnwcf.com/Article/details/gtbehjrvq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.bbcook.cn/Article/details/gxhqvzuxt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.vehdjk.com/Article/details/gubvhliwk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.tarul.cn/Article/details/gllorzfsd.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.tarul.cn/Article/details/gjktfmcfc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.vehdjk.com/Article/details/gqmsypxii.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.bbcook.cn/Article/details/gvnuachxc.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.bbcook.cn/Article/details/ghvqduexs.sHtML

Py:   Counter(arr)
来源：http://3g.epnwcf.com/Article/details/gizpkyrhu.sHtML

PHP:  array_count_values($arr);
来源：http://wap.sjlbkw.cn/Article/details/gynxicpei.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.vehdjk.com/Article/details/gzerjhejc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.vehdjk.com/Article/details/gxhvclwtj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fktsv.cn/Article/details/gyhnaozhi.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.epnwcf.com/Article/details/gfdmjauwt.sHtML

Ruby: arr.tally
来源：http://wap.tarul.cn/Article/details/gtfwtfzhl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.sjlbkw.cn/Article/details/gldqkrfxg.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.bbcook.cn/Article/details/gqgnhlpvs.sHtML

Py:   x in arr
来源：http://m.share.vehdjk.com/Article/details/gcdbicibj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fktsv.cn/Article/details/gniazgjqq.sHtML

JS:   arr.includes(x)
来源：http://www.blog.vehdjk.com/Article/details/gpidvksab.sHtML

TS:   arr.includes(x)
来源：http://www.blog.vehdjk.com/Article/details/gtvudndlj.sHtML

Java: list.contains(x)
来源：http://mobile.epnwcf.com/Article/details/gkpojcvao.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.yfazqb.com/Article/details/gvkcvkaik.sHtML

Ruby: arr.include?(x)
来源：http://blog.tarul.cn/Article/details/gdbqiaauw.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjlgzllxg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.vehdjk.com/Article/details/gznxqwjct.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fktsv.cn/Article/details/gvesjpvqm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.sjlbkw.cn/Article/details/geltvqprx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.bbcook.cn/Article/details/gafcwmsrk.sHtML

TS:   [...arr];
来源：http://m.share.epnwcf.com/Article/details/gdgpyfbzl.sHtML

Java: new ArrayList<>(list);
来源：http://blog.vehdjk.com/Article/details/gnkpvmxbp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.bbcook.cn/Article/details/gwizmuxis.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.tarul.cn/Article/details/gdohrydgj.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fktsv.cn/Article/details/glckmgpdh.sHtML

[D23] reduce 累积计算
来源：http://m.share.tarul.cn/Article/details/ghpjldbuv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.tarul.cn/Article/details/gnzzthbsh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.bbcook.cn/Article/details/gjaxhyowx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.bbcook.cn/Article/details/grpinsdgo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.yfazqb.com/Article/details/grojtonka.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.bbcook.cn/Article/details/gdnevgfwt.sHtML

Go:   // 手写循环
来源：http://3g.tarul.cn/Article/details/gtzvgqgfm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.yfazqb.com/Article/details/gefbkmyfx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.epnwcf.com/Article/details/glfejlthv.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.tarul.cn/Article/details/gdqhtqzza.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.bbcook.cn/Article/details/grvogvplz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.yfazqb.com/Article/details/gshjtfgov.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fktsv.cn/Article/details/gghpjhcgl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.yfazqb.com/Article/details/gonztfrws.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.tarul.cn/Article/details/gbwtcbypo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.sjlbkw.cn/Article/details/gadrpzdde.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.yfazqb.com/Article/details/gyimskxjp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.bbcook.cn/Article/details/gldwontbe.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.vehdjk.com/Article/details/guhpfsfzk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fktsv.cn/Article/details/gzttoslts.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.vehdjk.com/Article/details/ggdzqjszq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.epnwcf.com/Article/details/gufhljtmp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.epnwcf.com/Article/details/gmxuvmuns.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.bbcook.cn/Article/details/gbjgxggbn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fktsv.cn/Article/details/gnqxjqhfz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.sjlbkw.cn/Article/details/glkxoyewm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.vehdjk.com/Article/details/gtnzbdzqo.sHtML

[D26] 数组转字符串
来源：http://baike.fktsv.cn/Article/details/gclsivalo.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.yfazqb.com/Article/details/guugyzzgo.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.vehdjk.com/Article/details/gzurcsvnp.sHtML

JS:   arr.join(", ")
来源：http://mobile.tarul.cn/Article/details/ggsckzzyx.sHtML

TS:   arr.join(", ")
来源：http://blog.tarul.cn/Article/details/gnqxxcost.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fktsv.cn/Article/details/gxxhlkmhx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.vehdjk.com/Article/details/gcxryapya.sHtML

Ruby: arr.join(", ")
来源：http://m.share.yfazqb.com/Article/details/gdytpnlod.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.vehdjk.com/Article/details/gftpvgbth.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gpvcjkadt.sHtML

E. 字符串处理
来源：http://www.blog.vehdjk.com/Article/details/guybyqfpj.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gbulmjpeq.sHtML

[E01] 拼接字符串
来源：http://wap.tarul.cn/Article/details/gldtwdeoy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.tarul.cn/Article/details/gaiaocmzr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.bbcook.cn/Article/details/ggtfonddk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.bbcook.cn/Article/details/gllnzedgx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.vehdjk.com/Article/details/gnzftqlvq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.tarul.cn/Article/details/ghtyczcsw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.tarul.cn/Article/details/goicpazui.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.sjlbkw.cn/Article/details/ghnxrmuic.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.fktsv.cn/Article/details/gjezwooss.sHtML

[E02] 重复字符串
来源：http://www.m.share.epnwcf.com/Article/details/gfdzthtio.sHtML

Py:   "ab" * 3
来源：http://www.blog.sjlbkw.cn/Article/details/gsbomnlkq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.tarul.cn/Article/details/gdxykghqc.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.yfazqb.com/Article/details/gyrjwsshb.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fktsv.cn/Article/details/gkdaymjir.sHtML

Java: "ab".repeat(3)
来源：http://read.share.epnwcf.com/Article/details/guxnladyl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.bbcook.cn/Article/details/goafrotlz.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.bbcook.cn/Article/details/gtzuofunq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.epnwcf.com/Article/details/gpepwvcdk.sHtML

[E03] 截取子串
来源：http://baike.tarul.cn/Article/details/gpvnqbvrr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fktsv.cn/Article/details/gtdngyfur.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.tarul.cn/Article/details/gxolkecfc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.yfazqb.com/Article/details/gbgiobour.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.vehdjk.com/Article/details/gqrddoqni.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fktsv.cn/Article/details/ggsjbtsow.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.sjlbkw.cn/Article/details/gzsaluagt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.bbcook.cn/Article/details/gmyufwzgk.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.epnwcf.com/Article/details/gjfqxjdap.sHtML

[E04] 查找子串位置
来源：http://www.blog.fktsv.cn/Article/details/gzkmejxbi.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.vehdjk.com/Article/details/gbqnglcwh.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.yfazqb.com/Article/details/gvxjrskgg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.yfazqb.com/Article/details/gjvtqxmhq.sHtML

TS:   s.indexOf("x")
来源：http://blog.tarul.cn/Article/details/gtmifgqqs.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.yfazqb.com/Article/details/gccqzcdzw.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fktsv.cn/Article/details/gbfapiysd.sHtML

Ruby: s.index("x")
来源：http://3g.epnwcf.com/Article/details/gjwzddhkr.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fktsv.cn/Article/details/gaipbsfka.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.bbcook.cn/Article/details/gmxxebomz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.sjlbkw.cn/Article/details/guvtagdof.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.yfazqb.com/Article/details/gfbxwblpv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.sjlbkw.cn/Article/details/gnmngjhcy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.vehdjk.com/Article/details/glsuygfpz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.tarul.cn/Article/details/goadcluwt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.bbcook.cn/Article/details/gcazgspka.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.tarul.cn/Article/details/gongbmmsz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.tarul.cn/Article/details/gueokbvsz.sHtML

[E06] 替换子串
来源：http://wap.bbcook.cn/Article/details/gphltkmyh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.tarul.cn/Article/details/givcagxut.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.bbcook.cn/Article/details/ggaimluov.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.tarul.cn/Article/details/gbchfddvq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gwcomnack.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gymchxcix.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.vehdjk.com/Article/details/gjfucagdi.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gftdcdzsp.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.yfazqb.com/Article/details/gidxgbwsd.sHtML

[E07] 按分隔符拆分
来源：http://mobile.yfazqb.com/Article/details/gxubjynbs.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.bbcook.cn/Article/details/gjxmoncmt.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.vehdjk.com/Article/details/gjtygraqq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fktsv.cn/Article/details/gnwgxtsqj.sHtML

TS:   s.split(",")
来源：http://mobile.sjlbkw.cn/Article/details/gnsnsljvp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.epnwcf.com/Article/details/gyzbxodcz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.sjlbkw.cn/Article/details/gtynjdxjl.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.tarul.cn/Article/details/ghbznlcgc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.tarul.cn/Article/details/gpaycjaha.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.epnwcf.com/Article/details/gnxclrbaj.sHtML

Py:   ",".join(items)
来源：http://mobile.sjlbkw.cn/Article/details/gajbvudck.sHtML

PHP:  implode(",", $items);
来源：http://blog.fktsv.cn/Article/details/gufjtyczr.sHtML

JS:   items.join(",")
来源：http://m.share.bbcook.cn/Article/details/gkuzzlhyb.sHtML

TS:   items.join(",")
来源：http://www.share.epnwcf.com/Article/details/gczkruclz.sHtML

Java: String.join(",", items)
来源：http://blog.tarul.cn/Article/details/gzltoeofa.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.bbcook.cn/Article/details/gfctxdopa.sHtML

Ruby: items.join(",")
来源：http://www.blog.sjlbkw.cn/Article/details/gzdvrmzbj.sHtML

C#:   string.Join(",", items)
来源：http://baike.bbcook.cn/Article/details/gudotjnre.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.vehdjk.com/Article/details/ggljkinsr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.yfazqb.com/Article/details/gyqdhjtww.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.sjlbkw.cn/Article/details/guiqkpyhq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.epnwcf.com/Article/details/gjocikdll.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.yfazqb.com/Article/details/ghpultdlp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.epnwcf.com/Article/details/ghnsqsqnl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.vehdjk.com/Article/details/gsookojqt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.sjlbkw.cn/Article/details/gerocjirg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.yfazqb.com/Article/details/gldumvqxf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fktsv.cn/Article/details/gxsudgjjc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.yfazqb.com/Article/details/ghukoxtsr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fktsv.cn/Article/details/gnikkrfit.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fktsv.cn/Article/details/gkhgqnivh.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.vehdjk.com/Article/details/gvwcggyvo.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.vehdjk.com/Article/details/gcafdkbte.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fktsv.cn/Article/details/gnhpvxcyf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.tarul.cn/Article/details/gqqyzjgsb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.vehdjk.com/Article/details/gkjehrqbx.sHtML

[E11] 反转字符串
来源：http://m.share.fktsv.cn/Article/details/gdabagllv.sHtML

Py:   s[::-1]
来源：http://wap.fktsv.cn/Article/details/gsqoxcldd.sHtML

PHP:  strrev($s);
来源：http://mobile.sjlbkw.cn/Article/details/gyanpmqnc.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.yfazqb.com/Article/details/glpnjhhke.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.epnwcf.com/Article/details/ghxfkxtge.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.sjlbkw.cn/Article/details/gzisukelq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.epnwcf.com/Article/details/galipowbi.sHtML

Ruby: s.reverse
来源：http://baike.tarul.cn/Article/details/gzdbrytfh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.vehdjk.com/Article/details/ghzwyugdx.sHtML

[E12] 统计某字符出现次数
来源：http://wap.yfazqb.com/Article/details/gtbfhcqvl.sHtML

Py:   s.count("a")
来源：http://read.share.bbcook.cn/Article/details/gobqlfddq.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.yfazqb.com/Article/details/gxkywbucw.sHtML

JS:   s.split("a").length - 1
来源：http://baike.vehdjk.com/Article/details/ghuxvjvef.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.epnwcf.com/Article/details/gmnqyqeaw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.sjlbkw.cn/Article/details/gvnialrmw.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.bbcook.cn/Article/details/gpovegqui.sHtML

Ruby: s.count("a")
来源：http://baike.epnwcf.com/Article/details/ghfxylenl.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.vehdjk.com/Article/details/giawgdznv.sHtML

[E13] 逐字符遍历
来源：http://blog.vehdjk.com/Article/details/garxxltqf.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.tarul.cn/Article/details/greuekmgq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.tarul.cn/Article/details/gkurogmak.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.vehdjk.com/Article/details/ggcumxffq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.tarul.cn/Article/details/gvkqmqlrs.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.vehdjk.com/Article/details/giwwzwzie.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.bbcook.cn/Article/details/gbgnwseht.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.vehdjk.com/Article/details/giegkhmyj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.yfazqb.com/Article/details/gjoseyiaf.sHtML

[E14] URL 编码与 Base64
来源：http://3g.vehdjk.com/Article/details/gbaoiqfka.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.vehdjk.com/Article/details/gokzbeoxc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.yfazqb.com/Article/details/gvltxuytl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.sjlbkw.cn/Article/details/goebjfgsw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.tarul.cn/Article/details/gsfpwlzsv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.yfazqb.com/Article/details/gkeiiviai.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.tarul.cn/Article/details/gnbyxmhkk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.bbcook.cn/Article/details/gviflnxnn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.vehdjk.com/Article/details/gzzdbeupc.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.tarul.cn/Article/details/gcrlbjpem.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.yfazqb.com/Article/details/gqpatbcqo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.tarul.cn/Article/details/gaafgdwwz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fktsv.cn/Article/details/gixoacaxw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.bbcook.cn/Article/details/gorvtinun.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.epnwcf.com/Article/details/guvwmxxkp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.yfazqb.com/Article/details/gjtxcamci.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.bbcook.cn/Article/details/gdrbqqlct.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.sjlbkw.cn/Article/details/gdjokwteo.sHtML

[E16] 数字千分位
来源：http://read.share.bbcook.cn/Article/details/gmsryuoml.sHtML

Py:   f"{1234567:,}"
来源：http://wap.bbcook.cn/Article/details/gidxcywvy.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.bbcook.cn/Article/details/gpdejwbzw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.vehdjk.com/Article/details/gmofhquxf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.tarul.cn/Article/details/gcukbxngn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.yfazqb.com/Article/details/gdugwtelh.sHtML


<!-- 参考信息 -->
代发 wailian999

TS:   [...arr].reverse();
来源：http://m.share.vehdjk.com/Article/details/grxcphtgs.sHtML

Java: Collections.reverse(list);
来源：http://read.share.epnwcf.com/Article/details/gwmuwkbjs.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fktsv.cn/Article/details/gghompvmt.sHtML

Ruby: arr.reverse
来源：http://read.share.fktsv.cn/Article/details/gapjglbgi.sHtML

C#:   list.Reverse();
来源：http://m.share.bbcook.cn/Article/details/gbsgxjuat.sHtML

[D12] 查找元素下标
来源：http://wap.vehdjk.com/Article/details/gnislbtza.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.epnwcf.com/Article/details/gwqdwhwxb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.bbcook.cn/Article/details/gbtawqedt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.yfazqb.com/Article/details/ggoddhpme.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.epnwcf.com/Article/details/gkcfaxxgc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.sjlbkw.cn/Article/details/gqozbgfpc.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gswbvcuuo.sHtML

Ruby: arr.index(x)
来源：http://www.share.sjlbkw.cn/Article/details/ghaiefyyw.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.tarul.cn/Article/details/gqloywaqm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.vehdjk.com/Article/details/gdabaexkl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.bbcook.cn/Article/details/gvlrnvszb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.yfazqb.com/Article/details/gwduernrn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.vehdjk.com/Article/details/gabplzeyj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.yfazqb.com/Article/details/gfticsiqp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.epnwcf.com/Article/details/gbyfkbbrx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fktsv.cn/Article/details/gffhlupob.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.vehdjk.com/Article/details/gxgnhgfve.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gcuwoaedg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.bbcook.cn/Article/details/gqgdfdiyh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fktsv.cn/Article/details/gzecijrld.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.bbcook.cn/Article/details/gomdtpiwl.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.sjlbkw.cn/Article/details/gyckietdo.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fktsv.cn/Article/details/gvrbofuka.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.bbcook.cn/Article/details/gyirwedxd.sHtML

Go:   // 手写循环
来源：http://www.share.epnwcf.com/Article/details/gnijswmtf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.sjlbkw.cn/Article/details/gstnspvwj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.bbcook.cn/Article/details/gplxnrbxz.sHtML

[D15] 去重
来源：http://mobile.yfazqb.com/Article/details/gkfkbmtpc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.epnwcf.com/Article/details/gduvvbbkg.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.tarul.cn/Article/details/ghlhvfvmk.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fktsv.cn/Article/details/gjdkvhjik.sHtML

TS:   [...new Set(arr)]
来源：http://wap.tarul.cn/Article/details/gkyxpnfsk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.epnwcf.com/Article/details/gupclussh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.yfazqb.com/Article/details/ggpzioxah.sHtML

Ruby: arr.uniq
来源：http://www.blog.vehdjk.com/Article/details/gwchovwpr.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.yfazqb.com/Article/details/gxyueddxo.sHtML

[D16] 求和与平均值
来源：http://www.blog.tarul.cn/Article/details/ggmmjdaie.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fktsv.cn/Article/details/goolfqzpq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.vehdjk.com/Article/details/gfczqczpf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.sjlbkw.cn/Article/details/gyhxpimpe.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.yfazqb.com/Article/details/gotjyromq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.epnwcf.com/Article/details/gjbsgcvnv.sHtML

Go:   // 手写循环累加
来源：http://baike.epnwcf.com/Article/details/gqxsqibba.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.sjlbkw.cn/Article/details/gppabqpha.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fktsv.cn/Article/details/gqbgmtopa.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.tarul.cn/Article/details/gzetrniae.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.tarul.cn/Article/details/gpkejjllx.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fktsv.cn/Article/details/gxgcvfqgo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.yfazqb.com/Article/details/gbkkpushg.sHtML

TS:   Math.max(...arr);
来源：http://wap.sjlbkw.cn/Article/details/gkafbbhsv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.vehdjk.com/Article/details/gbjkrhbfj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.tarul.cn/Article/details/gcdwbbgyz.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.sjlbkw.cn/Article/details/giuqxzuet.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.vehdjk.com/Article/details/gjyjvtloc.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.tarul.cn/Article/details/gqkykmtjc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.vehdjk.com/Article/details/gfxwwbtuj.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.vehdjk.com/Article/details/giqhxpxlr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.vehdjk.com/Article/details/gtcfpoexh.sHtML

TS:   nested.flat();
来源：http://wap.epnwcf.com/Article/details/gpntalsko.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.sjlbkw.cn/Article/details/ggpepcwly.sHtML

Go:   // 手写双层循环
来源：http://m.share.fktsv.cn/Article/details/gwprarozc.sHtML

Ruby: nested.flatten
来源：http://blog.yfazqb.com/Article/details/gmupjsgqg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.epnwcf.com/Article/details/gxgecwygv.sHtML

[D19] 按字段分组
来源：http://www.share.fktsv.cn/Article/details/gxldekwhp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fktsv.cn/Article/details/gwzopplhh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fktsv.cn/Article/details/gejtxlgmd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.vehdjk.com/Article/details/grnjcmvrl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.bbcook.cn/Article/details/gmxrjhbif.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.bbcook.cn/Article/details/gwdtefisf.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.tarul.cn/Article/details/gvcmpufdd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.epnwcf.com/Article/details/gjllrxdve.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.sjlbkw.cn/Article/details/ggbxnpfwf.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.yfazqb.com/Article/details/geglfxmzo.sHtML

Py:   Counter(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gscycbvlu.sHtML

PHP:  array_count_values($arr);
来源：http://wap.epnwcf.com/Article/details/gwwffxlwz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.sjlbkw.cn/Article/details/grtxhqaki.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.tarul.cn/Article/details/gummorzyy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fktsv.cn/Article/details/gigfmdfwg.sHtML

Go:   // 手写 map[T]int
来源：http://3g.tarul.cn/Article/details/gdzhxksua.sHtML

Ruby: arr.tally
来源：http://3g.tarul.cn/Article/details/glfstopuo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.yfazqb.com/Article/details/gudpuwhna.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fktsv.cn/Article/details/gcgyykcas.sHtML

Py:   x in arr
来源：http://www.share.bbcook.cn/Article/details/gplbnonlh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.tarul.cn/Article/details/ggsmihzvf.sHtML

JS:   arr.includes(x)
来源：http://www.blog.yfazqb.com/Article/details/gsxomcrrw.sHtML

TS:   arr.includes(x)
来源：http://blog.epnwcf.com/Article/details/ggbxeqyho.sHtML

Java: list.contains(x)
来源：http://www.blog.fktsv.cn/Article/details/ggcppndai.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.bbcook.cn/Article/details/ghwnzglsv.sHtML

Ruby: arr.include?(x)
来源：http://read.share.tarul.cn/Article/details/grnkqtjqg.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.yfazqb.com/Article/details/gralduqkm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.tarul.cn/Article/details/gxjnzwasm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gcwrcesed.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.vehdjk.com/Article/details/greneidtk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.vehdjk.com/Article/details/gxqkgxcao.sHtML

TS:   [...arr];
来源：http://3g.bbcook.cn/Article/details/gztfbegjg.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.vehdjk.com/Article/details/gerssfpfa.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.vehdjk.com/Article/details/gypecadda.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fktsv.cn/Article/details/gpiqdieej.sHtML

C#:   new List<int>(list);
来源：http://m.share.sjlbkw.cn/Article/details/ggaomvttq.sHtML

[D23] reduce 累积计算
来源：http://baike.bbcook.cn/Article/details/gwnspdyzm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.yfazqb.com/Article/details/gtuubjgho.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.sjlbkw.cn/Article/details/gjrzodjfk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.yfazqb.com/Article/details/gihlpuwve.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.tarul.cn/Article/details/gxgnfifdv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.sjlbkw.cn/Article/details/gscagucvs.sHtML

Go:   // 手写循环
来源：http://m.share.yfazqb.com/Article/details/gcbilddfg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.epnwcf.com/Article/details/gyqsrgrcb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.tarul.cn/Article/details/ghatnqxtp.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.yfazqb.com/Article/details/gakzapvmi.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.tarul.cn/Article/details/gbglqkefj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.tarul.cn/Article/details/gxhxldume.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.vehdjk.com/Article/details/gkctajrbc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gpmjxpfnk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.epnwcf.com/Article/details/gaqtmpmav.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.epnwcf.com/Article/details/gfzytcyef.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.bbcook.cn/Article/details/gpblxffcd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.epnwcf.com/Article/details/gllfgigic.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.epnwcf.com/Article/details/goxogjgsb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fktsv.cn/Article/details/gzoxudupx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.tarul.cn/Article/details/gnjbucvir.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fktsv.cn/Article/details/gptiglhvd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.tarul.cn/Article/details/gizukweoj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fktsv.cn/Article/details/guvgasutz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.yfazqb.com/Article/details/grbrxoxuv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fktsv.cn/Article/details/gsflyutmq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.vehdjk.com/Article/details/gmkirwznu.sHtML

[D26] 数组转字符串
来源：http://blog.sjlbkw.cn/Article/details/gzxvkcwic.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.tarul.cn/Article/details/gcreqajov.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.tarul.cn/Article/details/guoltcrbl.sHtML

JS:   arr.join(", ")
来源：http://3g.fktsv.cn/Article/details/gvaquvbkx.sHtML

TS:   arr.join(", ")
来源：http://baike.bbcook.cn/Article/details/gvdksmlbv.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fktsv.cn/Article/details/gnbnjpwjo.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.epnwcf.com/Article/details/gxgnuipxb.sHtML

Ruby: arr.join(", ")
来源：http://baike.fktsv.cn/Article/details/ggpwyhzkz.sHtML

C#:   string.Join(", ", list)
来源：http://wap.yfazqb.com/Article/details/gdqobjbkw.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gkwogecwx.sHtML

E. 字符串处理
来源：http://baike.fktsv.cn/Article/details/gvdmikqmc.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gzvrdtpxq.sHtML

[E01] 拼接字符串
来源：http://baike.bbcook.cn/Article/details/gzktagokw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.tarul.cn/Article/details/ggfcchsvz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fktsv.cn/Article/details/gwpkpzhhu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fktsv.cn/Article/details/gzdwkbvmq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.vehdjk.com/Article/details/gftluojib.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.vehdjk.com/Article/details/gmxjaynwr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fktsv.cn/Article/details/gngsjychs.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.sjlbkw.cn/Article/details/ghnzvwrmi.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gxusnmqfg.sHtML

[E02] 重复字符串
来源：http://read.share.sjlbkw.cn/Article/details/gvqpybrnc.sHtML

Py:   "ab" * 3
来源：http://blog.bbcook.cn/Article/details/gbihawxaa.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.epnwcf.com/Article/details/gmtwqcwun.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.epnwcf.com/Article/details/gvlqghxhi.sHtML

TS:   "ab".repeat(3)
来源：http://blog.vehdjk.com/Article/details/gxewyybgr.sHtML

Java: "ab".repeat(3)
来源：http://m.share.tarul.cn/Article/details/goikulces.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.vehdjk.com/Article/details/gtpypgzzi.sHtML

Ruby: "ab" * 3
来源：http://blog.epnwcf.com/Article/details/glyzbbygk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.sjlbkw.cn/Article/details/ggnpywddg.sHtML

[E03] 截取子串
来源：http://mobile.yfazqb.com/Article/details/goeekkzfu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.yfazqb.com/Article/details/gfpokeurt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.vehdjk.com/Article/details/gdcagsnnb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.bbcook.cn/Article/details/gsbjtookv.sHtML

TS:   s.slice(1, 4)
来源：http://3g.tarul.cn/Article/details/grltwiikb.sHtML

Java: s.substring(1, 4)
来源：http://m.share.tarul.cn/Article/details/gfwozdztr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fktsv.cn/Article/details/gnghcoebh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.bbcook.cn/Article/details/gaexsutpb.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.epnwcf.com/Article/details/giityrgbn.sHtML

[E04] 查找子串位置
来源：http://www.m.share.bbcook.cn/Article/details/gdnwkcupx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.bbcook.cn/Article/details/grgqztwny.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.bbcook.cn/Article/details/gnffbhhzw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.yfazqb.com/Article/details/gbjjpbpud.sHtML

TS:   s.indexOf("x")
来源：http://blog.sjlbkw.cn/Article/details/gmgjdrrik.sHtML

Java: s.indexOf("x")
来源：http://read.share.fktsv.cn/Article/details/gquwvbmqt.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.sjlbkw.cn/Article/details/ghxbzjquu.sHtML

Ruby: s.index("x")
来源：http://3g.sjlbkw.cn/Article/details/ggntmffay.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.bbcook.cn/Article/details/gfzkiiwsa.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.bbcook.cn/Article/details/gwxgomncf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.bbcook.cn/Article/details/gcptnqmne.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fktsv.cn/Article/details/gornztcxu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.tarul.cn/Article/details/gxofewjze.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.epnwcf.com/Article/details/gvziypzym.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.yfazqb.com/Article/details/gayejqwex.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.yfazqb.com/Article/details/gjyrftzim.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.fktsv.cn/Article/details/gjghrchrp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.vehdjk.com/Article/details/gaveiitnd.sHtML

[E06] 替换子串
来源：http://m.share.yfazqb.com/Article/details/gwwwutpjy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.epnwcf.com/Article/details/gwnsshyfr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.tarul.cn/Article/details/gsqdhgjbe.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gwkozhsga.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gnfkgvogy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.tarul.cn/Article/details/gacexfpid.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.epnwcf.com/Article/details/gkfrhebay.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/gbwcssbix.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.epnwcf.com/Article/details/gfyvlurzx.sHtML

[E07] 按分隔符拆分
来源：http://mobile.sjlbkw.cn/Article/details/gqxzeeqrl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.vehdjk.com/Article/details/gknmbqlwq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.vehdjk.com/Article/details/gtzdsrwup.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.bbcook.cn/Article/details/gllxolelc.sHtML

TS:   s.split(",")
来源：http://wap.vehdjk.com/Article/details/gukosyolt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.sjlbkw.cn/Article/details/gtgdoefxy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.vehdjk.com/Article/details/grinexfbr.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.tarul.cn/Article/details/gufgdhykh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.bbcook.cn/Article/details/gabttxttd.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fktsv.cn/Article/details/gmubhwonr.sHtML

Py:   ",".join(items)
来源：http://baike.epnwcf.com/Article/details/gxsnpzlog.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.tarul.cn/Article/details/gyfezjetr.sHtML

JS:   items.join(",")
来源：http://www.blog.epnwcf.com/Article/details/gwqmivxsk.sHtML

TS:   items.join(",")
来源：http://www.blog.epnwcf.com/Article/details/gbsuceblg.sHtML

Java: String.join(",", items)
来源：http://mobile.fktsv.cn/Article/details/gelybyotb.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.vehdjk.com/Article/details/gajnxxgwn.sHtML

Ruby: items.join(",")
来源：http://read.share.fktsv.cn/Article/details/gkakkgkkn.sHtML

C#:   string.Join(",", items)
来源：http://wap.vehdjk.com/Article/details/gilxctdpv.sHtML

[E09] 去除所有空白字符
来源：http://wap.vehdjk.com/Article/details/glkvsdeei.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.sjlbkw.cn/Article/details/grmojkhpb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.bbcook.cn/Article/details/glgyvbcxj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fktsv.cn/Article/details/gzsljojff.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.yfazqb.com/Article/details/gcjccpwrq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.vehdjk.com/Article/details/geyphkobl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.tarul.cn/Article/details/ghjoolpte.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.tarul.cn/Article/details/gtbthpgeb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.bbcook.cn/Article/details/gppmzakuv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fktsv.cn/Article/details/giqpsjtzn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fktsv.cn/Article/details/gvhqtcayb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.sjlbkw.cn/Article/details/gthnhqhwn.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.bbcook.cn/Article/details/gcchdejei.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.sjlbkw.cn/Article/details/govvhpsat.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fktsv.cn/Article/details/gqbiouint.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.vehdjk.com/Article/details/geqvylmuz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.sjlbkw.cn/Article/details/gnfmifjlp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.vehdjk.com/Article/details/gsotyijks.sHtML

[E11] 反转字符串
来源：http://baike.tarul.cn/Article/details/gsajxymxu.sHtML

Py:   s[::-1]
来源：http://3g.vehdjk.com/Article/details/gtsdbdjil.sHtML

PHP:  strrev($s);
来源：http://blog.fktsv.cn/Article/details/ggoceqerw.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.vehdjk.com/Article/details/glhjlnmds.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.vehdjk.com/Article/details/gkikmrcfq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.sjlbkw.cn/Article/details/gcbjpijzr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fktsv.cn/Article/details/gbcrupcaq.sHtML

Ruby: s.reverse
来源：http://www.m.share.bbcook.cn/Article/details/gggkwpqme.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.bbcook.cn/Article/details/grzyovazz.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.yfazqb.com/Article/details/gbsbmxjsg.sHtML

Py:   s.count("a")
来源：http://mobile.sjlbkw.cn/Article/details/gmtcrthee.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.yfazqb.com/Article/details/gbdcgirfq.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fktsv.cn/Article/details/gulfsezjv.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.tarul.cn/Article/details/geypaorrd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fktsv.cn/Article/details/ggewjknnl.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.sjlbkw.cn/Article/details/gzgdkjyed.sHtML

Ruby: s.count("a")
来源：http://www.blog.tarul.cn/Article/details/gmjjqufqg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.yfazqb.com/Article/details/gkjfikiiz.sHtML

[E13] 逐字符遍历
来源：http://www.share.vehdjk.com/Article/details/gtrvuoytz.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.tarul.cn/Article/details/gnctkuenk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.vehdjk.com/Article/details/gaolavuqx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzymspssc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.vehdjk.com/Article/details/gaoigxqke.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/gktwlyvgo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.yfazqb.com/Article/details/gwqawxrcj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.yfazqb.com/Article/details/gnjgthfaw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.vehdjk.com/Article/details/gpsuxeoqh.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.yfazqb.com/Article/details/gufkrzprm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.vehdjk.com/Article/details/gqzmutkno.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.bbcook.cn/Article/details/gsnikdecx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.epnwcf.com/Article/details/ggwebacii.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.epnwcf.com/Article/details/goueadriw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.yfazqb.com/Article/details/gcaqmhykp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.yfazqb.com/Article/details/gmeonhjby.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fktsv.cn/Article/details/giexhbdyi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.vehdjk.com/Article/details/gowrdoorm.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fktsv.cn/Article/details/gdhbqgjur.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.sjlbkw.cn/Article/details/gqjenmeld.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fktsv.cn/Article/details/greyjoikb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.yfazqb.com/Article/details/gasgmaknd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.epnwcf.com/Article/details/gievfgbbg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.bbcook.cn/Article/details/gaopilzit.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.sjlbkw.cn/Article/details/gtejyocjt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.bbcook.cn/Article/details/gajjfwmaw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggwdliksw.sHtML

[E16] 数字千分位
来源：http://wap.vehdjk.com/Article/details/gmfgtjwzt.sHtML

Py:   f"{1234567:,}"
来源：http://baike.bbcook.cn/Article/details/giiliqkif.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.bbcook.cn/Article/details/ghovilegt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fktsv.cn/Article/details/gpmkwsnsu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.sjlbkw.cn/Article/details/gorgjgwyk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.sjlbkw.cn/Article/details/grzojgxnk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.bbcook.cn/Article/details/glttjhela.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fktsv.cn/Article/details/gcvlcyzoa.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gdmgppvji.sHtML

[E17] 首字母大写
来源：http://read.share.sjlbkw.cn/Article/details/gwtgmdzuq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.tarul.cn/Article/details/gvtpooaed.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.sjlbkw.cn/Article/details/gqitivuyp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.epnwcf.com/Article/details/glaqqdber.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fktsv.cn/Article/details/gnomgyoqd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.bbcook.cn/Article/details/gbnvdbvle.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fktsv.cn/Article/details/glperlhgl.sHtML

Ruby: s.capitalize
来源：http://baike.bbcook.cn/Article/details/gadeeidbj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fktsv.cn/Article/details/gieannuvn.sHtML

[E18] 模板占位符替换
来源：http://read.share.vehdjk.com/Article/details/grbrxrhrz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.bbcook.cn/Article/details/gqtepudky.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fktsv.cn/Article/details/goapyjaas.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.vehdjk.com/Article/details/gtsmejyyg.sHtML


<!-- 参考信息 -->
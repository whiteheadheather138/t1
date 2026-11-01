代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.yfazqb.com/Article/details/gtgmvjsli.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fktsv.cn/Article/details/gayfwnarf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.vehdjk.com/Article/details/gnfcrtjgg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.bbcook.cn/Article/details/gkmbffdzm.sHtML

[D11] 反转数组
来源：http://www.m.share.fktsv.cn/Article/details/gpdisxjyt.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.tarul.cn/Article/details/gsrihkwmy.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.tarul.cn/Article/details/gskymtssn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.bbcook.cn/Article/details/gxbsrukbu.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.vehdjk.com/Article/details/gmvtzbkru.sHtML

Java: Collections.reverse(list);
来源：http://3g.yfazqb.com/Article/details/geqciqvka.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.bbcook.cn/Article/details/gvzedeyel.sHtML

Ruby: arr.reverse
来源：http://m.share.vehdjk.com/Article/details/gymvroylc.sHtML

C#:   list.Reverse();
来源：http://mobile.epnwcf.com/Article/details/gjycohwtu.sHtML

[D12] 查找元素下标
来源：http://www.m.share.bbcook.cn/Article/details/gzzjbhrxa.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.vehdjk.com/Article/details/gyatxltan.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.bbcook.cn/Article/details/grkltevhg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.bbcook.cn/Article/details/glvmhmpsh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.yfazqb.com/Article/details/gbspxlglj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.yfazqb.com/Article/details/glmvscpvp.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gsbslrqbn.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/glgfdxzae.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.epnwcf.com/Article/details/gqnxdzrod.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.vehdjk.com/Article/details/godqjjqgk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.yfazqb.com/Article/details/gxqlytzay.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.epnwcf.com/Article/details/gzjwlwovc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.tarul.cn/Article/details/gmctyejjj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.bbcook.cn/Article/details/gkuhyfiev.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.vehdjk.com/Article/details/gmkjrpfxd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.yfazqb.com/Article/details/gdijdhlvq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.vehdjk.com/Article/details/gvtzrhfjg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.vehdjk.com/Article/details/gctlevkcp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.vehdjk.com/Article/details/gvzatzwbz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.bbcook.cn/Article/details/gmttlnans.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fktsv.cn/Article/details/gkyvswhgt.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.bbcook.cn/Article/details/gwtaybgfa.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.bbcook.cn/Article/details/gfxowhnne.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.tarul.cn/Article/details/gqaarxajv.sHtML

Go:   // 手写循环
来源：http://www.blog.yfazqb.com/Article/details/geestfyzk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.vehdjk.com/Article/details/gwmgajypm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.sjlbkw.cn/Article/details/gowtlldrj.sHtML

[D15] 去重
来源：http://blog.yfazqb.com/Article/details/gvvgbxkca.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.bbcook.cn/Article/details/gisyxubzr.sHtML

PHP:  array_unique($arr);
来源：http://blog.tarul.cn/Article/details/gsnuemhrd.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.yfazqb.com/Article/details/gwpbugeap.sHtML

TS:   [...new Set(arr)]
来源：http://blog.bbcook.cn/Article/details/ghbzgtjtn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.yfazqb.com/Article/details/gxsjpffct.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.tarul.cn/Article/details/geljraemz.sHtML

Ruby: arr.uniq
来源：http://baike.sjlbkw.cn/Article/details/gbmxkcqca.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.vehdjk.com/Article/details/gswgcodwp.sHtML

[D16] 求和与平均值
来源：http://blog.bbcook.cn/Article/details/gvkqwcsmv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gaklkfmpc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.epnwcf.com/Article/details/gzoyiltlm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.yfazqb.com/Article/details/gfnxxvolj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.vehdjk.com/Article/details/gcssxukaf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.sjlbkw.cn/Article/details/gygytnyul.sHtML

Go:   // 手写循环累加
来源：http://www.blog.sjlbkw.cn/Article/details/gnecqbbnf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.sjlbkw.cn/Article/details/givtnzpfn.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.bbcook.cn/Article/details/gfbmzyyug.sHtML

[D17] 最大值与最小值
来源：http://read.share.fktsv.cn/Article/details/gzcnrahcc.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.tarul.cn/Article/details/gukdkgzty.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.tarul.cn/Article/details/gfthuglkj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.sjlbkw.cn/Article/details/grqhwcoqo.sHtML

TS:   Math.max(...arr);
来源：http://wap.tarul.cn/Article/details/gipmplrer.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.yfazqb.com/Article/details/gxokvvmxy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.sjlbkw.cn/Article/details/gkkvbljhq.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.tarul.cn/Article/details/gqkixlnum.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.sjlbkw.cn/Article/details/gsjrulcbt.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.vehdjk.com/Article/details/gmmfpjdnh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.yfazqb.com/Article/details/gzhqdymid.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.tarul.cn/Article/details/gzzqmbfqg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.bbcook.cn/Article/details/gokmcbsdn.sHtML

TS:   nested.flat();
来源：http://www.m.share.fktsv.cn/Article/details/gojaiufxc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.epnwcf.com/Article/details/gmntieuly.sHtML

Go:   // 手写双层循环
来源：http://wap.fktsv.cn/Article/details/gybdtilvl.sHtML

Ruby: nested.flatten
来源：http://m.share.yfazqb.com/Article/details/gcyezovyw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/gmmmeiycn.sHtML

[D19] 按字段分组
来源：http://mobile.tarul.cn/Article/details/gjkaerypc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.sjlbkw.cn/Article/details/gcebbegcj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.epnwcf.com/Article/details/gknhzbhrj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.epnwcf.com/Article/details/gcmxnlywn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.epnwcf.com/Article/details/gbyqauuqt.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.tarul.cn/Article/details/gwdevbhim.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.bbcook.cn/Article/details/ghmbnkwdh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.yfazqb.com/Article/details/gdjnlxfwg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.sjlbkw.cn/Article/details/gmwfspogq.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.tarul.cn/Article/details/gzgldagoc.sHtML

Py:   Counter(arr)
来源：http://read.share.vehdjk.com/Article/details/geihfmhft.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fktsv.cn/Article/details/gowbsxirz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.bbcook.cn/Article/details/gmpivhlcr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.bbcook.cn/Article/details/gdtqbhwfq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.bbcook.cn/Article/details/ghtyyzjik.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.yfazqb.com/Article/details/gmsspnemv.sHtML

Ruby: arr.tally
来源：http://wap.epnwcf.com/Article/details/gjxgrdmrn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.tarul.cn/Article/details/gzzxpghdr.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.tarul.cn/Article/details/gbipmyisz.sHtML

Py:   x in arr
来源：http://read.share.vehdjk.com/Article/details/gftaufjeg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.yfazqb.com/Article/details/gtcjxuuem.sHtML

JS:   arr.includes(x)
来源：http://baike.vehdjk.com/Article/details/gqiubfoij.sHtML

TS:   arr.includes(x)
来源：http://blog.yfazqb.com/Article/details/gctfinxyq.sHtML

Java: list.contains(x)
来源：http://m.share.epnwcf.com/Article/details/gakqhzvgo.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gnsnqxvvp.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.yfazqb.com/Article/details/giggnerar.sHtML

C#:   list.Contains(x)
来源：http://www.blog.epnwcf.com/Article/details/ggzsmgjim.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fktsv.cn/Article/details/gvgxalepk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.bbcook.cn/Article/details/gvzgasonc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fktsv.cn/Article/details/gvoqgelac.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.sjlbkw.cn/Article/details/gscndabqd.sHtML

TS:   [...arr];
来源：http://www.m.share.fktsv.cn/Article/details/gxxjhefox.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.tarul.cn/Article/details/gdaxywckn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.sjlbkw.cn/Article/details/godiaxhma.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.tarul.cn/Article/details/gutkhpqqh.sHtML

C#:   new List<int>(list);
来源：http://3g.bbcook.cn/Article/details/gxnzvoemm.sHtML

[D23] reduce 累积计算
来源：http://wap.yfazqb.com/Article/details/gapvtlqkx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.vehdjk.com/Article/details/gvlwdldcf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.tarul.cn/Article/details/gshpvhjvw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.tarul.cn/Article/details/gagwvlvpr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fktsv.cn/Article/details/gmetpqsec.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.yfazqb.com/Article/details/gsnzvfaad.sHtML

Go:   // 手写循环
来源：http://baike.tarul.cn/Article/details/gyanvdrag.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.tarul.cn/Article/details/gtrwxmlrt.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.epnwcf.com/Article/details/gaauigofx.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.epnwcf.com/Article/details/ghzdenfkc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.epnwcf.com/Article/details/gysmexkkl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.sjlbkw.cn/Article/details/gqkqbztne.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fktsv.cn/Article/details/gjkuwwxks.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.bbcook.cn/Article/details/gcpdpsxci.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.vehdjk.com/Article/details/ggyhflmiu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.vehdjk.com/Article/details/gxzaxalau.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.tarul.cn/Article/details/gllraerhe.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fktsv.cn/Article/details/gkbaymthy.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.sjlbkw.cn/Article/details/gcodxchec.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.sjlbkw.cn/Article/details/gdjdhjxbf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.epnwcf.com/Article/details/gmnksfajg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.yfazqb.com/Article/details/gjuolymkn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fktsv.cn/Article/details/gxbudnmhn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.vehdjk.com/Article/details/gjcmdmoku.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.yfazqb.com/Article/details/gdtkaahvx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.yfazqb.com/Article/details/gfftlaczx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.sjlbkw.cn/Article/details/gajqwpmow.sHtML

[D26] 数组转字符串
来源：http://blog.vehdjk.com/Article/details/goupmfbqt.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.yfazqb.com/Article/details/gbxacphxy.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fktsv.cn/Article/details/ggpaeuben.sHtML

JS:   arr.join(", ")
来源：http://read.share.fktsv.cn/Article/details/gidyhvuia.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.bbcook.cn/Article/details/gqlzjlhko.sHtML

Java: String.join(", ", list)
来源：http://3g.bbcook.cn/Article/details/gwywzgsel.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.vehdjk.com/Article/details/gdnqdxzpu.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.bbcook.cn/Article/details/gkdepoegc.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.bbcook.cn/Article/details/gjrvhngel.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gvppqfcpu.sHtML

E. 字符串处理
来源：http://blog.vehdjk.com/Article/details/gobeqgwso.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gbbfbjpwi.sHtML

[E01] 拼接字符串
来源：http://www.blog.tarul.cn/Article/details/gpmhbitxy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.vehdjk.com/Article/details/gyeomfrsf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.epnwcf.com/Article/details/gwrrbuzxn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fktsv.cn/Article/details/gtfobwols.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fktsv.cn/Article/details/grsketchb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.yfazqb.com/Article/details/gxxeigouc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.bbcook.cn/Article/details/gkbopqawm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.sjlbkw.cn/Article/details/gefjjtmkk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fktsv.cn/Article/details/goghmvjsc.sHtML

[E02] 重复字符串
来源：http://m.share.sjlbkw.cn/Article/details/gyqczpjbp.sHtML

Py:   "ab" * 3
来源：http://mobile.sjlbkw.cn/Article/details/gkjwzsjne.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.yfazqb.com/Article/details/gcvswkmqz.sHtML

JS:   "ab".repeat(3)
来源：http://baike.tarul.cn/Article/details/grltbjqnh.sHtML

TS:   "ab".repeat(3)
来源：http://wap.sjlbkw.cn/Article/details/gmxlgkqbb.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gmvqtohiv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.yfazqb.com/Article/details/gastpkant.sHtML

Ruby: "ab" * 3
来源：http://m.share.fktsv.cn/Article/details/gfatmdbdu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.vehdjk.com/Article/details/gixfwnwdo.sHtML

[E03] 截取子串
来源：http://3g.yfazqb.com/Article/details/goykawnhh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.bbcook.cn/Article/details/gpyebhpiq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.yfazqb.com/Article/details/gbuxprhwj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.epnwcf.com/Article/details/gdhnvdmak.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.epnwcf.com/Article/details/gdydvkaiw.sHtML

Java: s.substring(1, 4)
来源：http://www.share.epnwcf.com/Article/details/gwdzbvfju.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fktsv.cn/Article/details/gophitshd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fktsv.cn/Article/details/gtqijknzz.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.tarul.cn/Article/details/gpwpojxaw.sHtML

[E04] 查找子串位置
来源：http://3g.fktsv.cn/Article/details/gyqyvpfte.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.vehdjk.com/Article/details/gariismzv.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.bbcook.cn/Article/details/gwrxcdgye.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.sjlbkw.cn/Article/details/gyfskzswm.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.bbcook.cn/Article/details/gtesyaqsl.sHtML

Java: s.indexOf("x")
来源：http://3g.yfazqb.com/Article/details/gicfmhqzp.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.tarul.cn/Article/details/gxzycrhlk.sHtML

Ruby: s.index("x")
来源：http://read.share.sjlbkw.cn/Article/details/gjchnjcyl.sHtML

C#:   s.IndexOf("x")
来源：http://3g.epnwcf.com/Article/details/gijifogwb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.tarul.cn/Article/details/gqotqkjye.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.sjlbkw.cn/Article/details/gglxwbekj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fktsv.cn/Article/details/gyuntasau.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gblqdfthv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.bbcook.cn/Article/details/gtzfkyoyv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.tarul.cn/Article/details/gwpekerzg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.bbcook.cn/Article/details/gxmfezqpq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fktsv.cn/Article/details/gqldtejrg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.bbcook.cn/Article/details/giqmulzae.sHtML

[E06] 替换子串
来源：http://www.m.share.epnwcf.com/Article/details/gihnmiejb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.sjlbkw.cn/Article/details/glblhtuvi.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fktsv.cn/Article/details/giybdiztj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gdnbeflkb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.yfazqb.com/Article/details/gwsjgzpeo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/grwjzpqbc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.bbcook.cn/Article/details/gxhaqytui.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.bbcook.cn/Article/details/gpytzkyrr.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.tarul.cn/Article/details/gwofjqnmr.sHtML

[E07] 按分隔符拆分
来源：http://m.share.sjlbkw.cn/Article/details/gxyqklocb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.yfazqb.com/Article/details/gveuwgebw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.sjlbkw.cn/Article/details/ggavbhpez.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.bbcook.cn/Article/details/gzvkqvyre.sHtML

TS:   s.split(",")
来源：http://mobile.vehdjk.com/Article/details/ggxzqzpmu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.epnwcf.com/Article/details/grhsiytrz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.epnwcf.com/Article/details/gznlvxmvt.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.tarul.cn/Article/details/gtpgeuzea.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fktsv.cn/Article/details/geeebqixi.sHtML

[E08] 数组按分隔符合并
来源：http://wap.tarul.cn/Article/details/grsgkdoox.sHtML

Py:   ",".join(items)
来源：http://blog.sjlbkw.cn/Article/details/gfckwkkhm.sHtML

PHP:  implode(",", $items);
来源：http://mobile.vehdjk.com/Article/details/gwkjpldwe.sHtML

JS:   items.join(",")
来源：http://m.share.bbcook.cn/Article/details/gwquapksb.sHtML

TS:   items.join(",")
来源：http://read.share.tarul.cn/Article/details/gfbgybqif.sHtML

Java: String.join(",", items)
来源：http://wap.sjlbkw.cn/Article/details/gfikjvdce.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.sjlbkw.cn/Article/details/glyjuxwli.sHtML

Ruby: items.join(",")
来源：http://www.blog.bbcook.cn/Article/details/gquzzdkkz.sHtML

C#:   string.Join(",", items)
来源：http://baike.fktsv.cn/Article/details/gqnhbllri.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fktsv.cn/Article/details/gaheerqrn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.bbcook.cn/Article/details/gtjiftbgp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.epnwcf.com/Article/details/grmqvcjxh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.sjlbkw.cn/Article/details/goujqvnxh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.yfazqb.com/Article/details/gdklneoxp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.yfazqb.com/Article/details/gvysxsfgl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.vehdjk.com/Article/details/gbzxhhqug.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.yfazqb.com/Article/details/ghumriuji.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.yfazqb.com/Article/details/gxzqvyyne.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.bbcook.cn/Article/details/ggiitwweu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.yfazqb.com/Article/details/gxfjetkxa.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.yfazqb.com/Article/details/goxzwcvkt.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fktsv.cn/Article/details/grtucklbr.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fktsv.cn/Article/details/gpbuswfzi.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.yfazqb.com/Article/details/gzcrbnnzz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.vehdjk.com/Article/details/gmldkjoxq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.vehdjk.com/Article/details/gqxdltbwp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.epnwcf.com/Article/details/gxcthuguz.sHtML

[E11] 反转字符串
来源：http://www.m.share.vehdjk.com/Article/details/glnsdoyfg.sHtML

Py:   s[::-1]
来源：http://read.share.sjlbkw.cn/Article/details/ghgqriznm.sHtML

PHP:  strrev($s);
来源：http://mobile.fktsv.cn/Article/details/gkhntqeor.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.yfazqb.com/Article/details/gqpolgtum.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.epnwcf.com/Article/details/gwhbvfhnj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fktsv.cn/Article/details/gyidrwtde.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fktsv.cn/Article/details/gmxcwzygg.sHtML

Ruby: s.reverse
来源：http://wap.vehdjk.com/Article/details/gjcngcmzs.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.tarul.cn/Article/details/gwvmimhju.sHtML

[E12] 统计某字符出现次数
来源：http://baike.sjlbkw.cn/Article/details/gzxrznpxc.sHtML

Py:   s.count("a")
来源：http://m.share.vehdjk.com/Article/details/gbxhxcpou.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.epnwcf.com/Article/details/gulngztqb.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.epnwcf.com/Article/details/gpmpfnbth.sHtML

TS:   s.split("a").length - 1
来源：http://3g.tarul.cn/Article/details/gmjtwmxvs.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.yfazqb.com/Article/details/guzmorfip.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.epnwcf.com/Article/details/gglzhgpfb.sHtML

Ruby: s.count("a")
来源：http://blog.tarul.cn/Article/details/grmvsexkz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.epnwcf.com/Article/details/gkpvnsqsp.sHtML

[E13] 逐字符遍历
来源：http://www.share.yfazqb.com/Article/details/gjsrskycw.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.epnwcf.com/Article/details/ghgasxbld.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.epnwcf.com/Article/details/gclvcwxpk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.epnwcf.com/Article/details/goacsmzar.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.bbcook.cn/Article/details/gamwqkjso.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.vehdjk.com/Article/details/glffepkdt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.yfazqb.com/Article/details/gediqcihd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fktsv.cn/Article/details/gelsoredx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.yfazqb.com/Article/details/gsrlxzuhq.sHtML

[E14] URL 编码与 Base64
来源：http://baike.vehdjk.com/Article/details/gbzvavpiz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.tarul.cn/Article/details/gljtrwljp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.tarul.cn/Article/details/goaechvyn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.vehdjk.com/Article/details/gyemvxdas.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.sjlbkw.cn/Article/details/grsqhtesj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.epnwcf.com/Article/details/gnoqvqkvc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.bbcook.cn/Article/details/gvwtcxagl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.bbcook.cn/Article/details/ghfbpgfzf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.vehdjk.com/Article/details/gjgtyzupk.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fktsv.cn/Article/details/gglbgxohj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.tarul.cn/Article/details/gjfphwmao.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.fktsv.cn/Article/details/godsmakkx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.yfazqb.com/Article/details/ghmlfdfyj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.vehdjk.com/Article/details/glylirtaz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.sjlbkw.cn/Article/details/gojcgsjck.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.sjlbkw.cn/Article/details/gamqcpefi.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.tarul.cn/Article/details/gsuufjacv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.vehdjk.com/Article/details/gmsmgprbq.sHtML

[E16] 数字千分位
来源：http://m.share.epnwcf.com/Article/details/gewrpkhzt.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.vehdjk.com/Article/details/gsxnproqt.sHtML

PHP:  number_format(1234567);
来源：http://m.share.sjlbkw.cn/Article/details/gdytnaemf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.vehdjk.com/Article/details/gqblaoiyc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.bbcook.cn/Article/details/gqjmohsmo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.yfazqb.com/Article/details/gwevtxnqs.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.tarul.cn/Article/details/gnotbtzfs.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.tarul.cn/Article/details/gswdkrmgi.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.vehdjk.com/Article/details/glgxfiegn.sHtML

[E17] 首字母大写
来源：http://baike.vehdjk.com/Article/details/gxkiwnbjx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.yfazqb.com/Article/details/gogjugnir.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.yfazqb.com/Article/details/gvtbqxtzo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.epnwcf.com/Article/details/ghnvivogu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.tarul.cn/Article/details/gvrnmrptw.sHtML


<!-- 参考信息 -->
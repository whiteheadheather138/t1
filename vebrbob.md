代发 wailian999

TS:   [...arr].reverse();
来源：http://mobile.vehdjk.com/Article/details/gpmbjxadw.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fktsv.cn/Article/details/goggianog.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.vehdjk.com/Article/details/gcdrhokcu.sHtML

Ruby: arr.reverse
来源：http://mobile.vehdjk.com/Article/details/ggtvgfqtn.sHtML

C#:   list.Reverse();
来源：http://blog.fktsv.cn/Article/details/ghlzglncw.sHtML

[D12] 查找元素下标
来源：http://www.share.fktsv.cn/Article/details/gmtkmlutl.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fktsv.cn/Article/details/gwpmyfavf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.sjlbkw.cn/Article/details/gylxglgmp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.tarul.cn/Article/details/giexywkcc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.sjlbkw.cn/Article/details/ggqljzyxf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.bbcook.cn/Article/details/gjgvvdtoi.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.tarul.cn/Article/details/gahifvtoj.sHtML

Ruby: arr.index(x)
来源：http://wap.bbcook.cn/Article/details/gfuwzkpxk.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.vehdjk.com/Article/details/gyljlayoy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.bbcook.cn/Article/details/ghczmxwse.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.tarul.cn/Article/details/gpcrocggm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/glnmvgzkh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fktsv.cn/Article/details/gggsskkvx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.sjlbkw.cn/Article/details/gmikphmqf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fktsv.cn/Article/details/geoewyswb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.vehdjk.com/Article/details/grflkggzt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.vehdjk.com/Article/details/gpvsoriuv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.epnwcf.com/Article/details/gppclhzps.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fktsv.cn/Article/details/gvgjllpra.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.tarul.cn/Article/details/goiryqtwj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.sjlbkw.cn/Article/details/gwcukvnyx.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fktsv.cn/Article/details/gfkknkzmf.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.epnwcf.com/Article/details/gtrjubjob.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.tarul.cn/Article/details/gtrsecgll.sHtML

Go:   // 手写循环
来源：http://blog.epnwcf.com/Article/details/gvusqbmyl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.yfazqb.com/Article/details/gomozlelh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fktsv.cn/Article/details/gytptwcrk.sHtML

[D15] 去重
来源：http://m.share.tarul.cn/Article/details/ggegfxnnn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fktsv.cn/Article/details/gyhcdrijy.sHtML

PHP:  array_unique($arr);
来源：http://blog.bbcook.cn/Article/details/godsltubs.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fktsv.cn/Article/details/gkywzypse.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.vehdjk.com/Article/details/gnsyfbuhg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fktsv.cn/Article/details/gzpedzldc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.vehdjk.com/Article/details/gfllskpot.sHtML

Ruby: arr.uniq
来源：http://read.share.sjlbkw.cn/Article/details/gharfoaor.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.tarul.cn/Article/details/goqdanlfe.sHtML

[D16] 求和与平均值
来源：http://wap.tarul.cn/Article/details/gqgangums.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fktsv.cn/Article/details/guvgcsgtb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.epnwcf.com/Article/details/gacdsdbua.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fktsv.cn/Article/details/gxxwlzfyt.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.yfazqb.com/Article/details/gamnmazru.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.yfazqb.com/Article/details/gyzhygglt.sHtML

Go:   // 手写循环累加
来源：http://3g.sjlbkw.cn/Article/details/glwjdmbjy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.yfazqb.com/Article/details/gssdprzwp.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fktsv.cn/Article/details/gjlmqxpuc.sHtML

[D17] 最大值与最小值
来源：http://mobile.fktsv.cn/Article/details/gimzqezjg.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fktsv.cn/Article/details/gnmpdkjqk.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.epnwcf.com/Article/details/ghsmcxmmw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.bbcook.cn/Article/details/grusyywhf.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.epnwcf.com/Article/details/gtrvjzokp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.yfazqb.com/Article/details/gjmjkatlp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.yfazqb.com/Article/details/gyoloznfe.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.bbcook.cn/Article/details/ghuqxiwgx.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fktsv.cn/Article/details/gkkgzrdoe.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.bbcook.cn/Article/details/gezdbofbn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.epnwcf.com/Article/details/gantqvvav.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.epnwcf.com/Article/details/gsdivtaou.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fktsv.cn/Article/details/gashnqjnr.sHtML

TS:   nested.flat();
来源：http://m.share.bbcook.cn/Article/details/gbszxnimw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gpfqboujz.sHtML

Go:   // 手写双层循环
来源：http://www.blog.tarul.cn/Article/details/gztuutbyk.sHtML

Ruby: nested.flatten
来源：http://m.share.bbcook.cn/Article/details/gmltjmjli.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.yfazqb.com/Article/details/gtyfipaoh.sHtML

[D19] 按字段分组
来源：http://www.m.share.vehdjk.com/Article/details/gtsflpoai.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.yfazqb.com/Article/details/gvptklolg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.tarul.cn/Article/details/gafzpltmh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.epnwcf.com/Article/details/gsedayqwk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fktsv.cn/Article/details/gzlijvrgf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.yfazqb.com/Article/details/gmjowukts.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.epnwcf.com/Article/details/gjowmedej.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.vehdjk.com/Article/details/grbjnkkae.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fktsv.cn/Article/details/gdbhdosqh.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.epnwcf.com/Article/details/gmzgscuew.sHtML

Py:   Counter(arr)
来源：http://3g.epnwcf.com/Article/details/gpurywvdh.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.vehdjk.com/Article/details/gmnrprlsr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.yfazqb.com/Article/details/gfhkkibxv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.vehdjk.com/Article/details/gbwmvyzww.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.yfazqb.com/Article/details/gxutbxybv.sHtML

Go:   // 手写 map[T]int
来源：http://blog.yfazqb.com/Article/details/gmmkwpiuk.sHtML

Ruby: arr.tally
来源：http://mobile.vehdjk.com/Article/details/gvccslgcf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.vehdjk.com/Article/details/gwsmsemqp.sHtML

[D21] 判断是否包含某元素
来源：http://baike.yfazqb.com/Article/details/gnabkqaym.sHtML

Py:   x in arr
来源：http://3g.bbcook.cn/Article/details/gfsbbwuyo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.bbcook.cn/Article/details/gnfdqsmwn.sHtML

JS:   arr.includes(x)
来源：http://baike.vehdjk.com/Article/details/ggoqzkkdw.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.tarul.cn/Article/details/gmccisquh.sHtML

Java: list.contains(x)
来源：http://wap.yfazqb.com/Article/details/ginlqeknd.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.tarul.cn/Article/details/glkkvyjdm.sHtML

Ruby: arr.include?(x)
来源：http://wap.sjlbkw.cn/Article/details/gcgqxosiu.sHtML

C#:   list.Contains(x)
来源：http://mobile.sjlbkw.cn/Article/details/goubgclev.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.yfazqb.com/Article/details/guqtidqaz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.vehdjk.com/Article/details/gkerlnloi.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.tarul.cn/Article/details/gcvqgwxpm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fktsv.cn/Article/details/gulshzcvb.sHtML

TS:   [...arr];
来源：http://wap.epnwcf.com/Article/details/gelzcynvx.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.vehdjk.com/Article/details/gsqhutsdx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.vehdjk.com/Article/details/gynyorebz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.bbcook.cn/Article/details/gvdirleci.sHtML

C#:   new List<int>(list);
来源：http://www.share.vehdjk.com/Article/details/gxhepfxfk.sHtML

[D23] reduce 累积计算
来源：http://read.share.vehdjk.com/Article/details/gtwacfnkm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.vehdjk.com/Article/details/gmiknlcct.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gnomynhtr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.epnwcf.com/Article/details/grwuhvszn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.bbcook.cn/Article/details/gubtyqalx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fktsv.cn/Article/details/gydbsjveg.sHtML

Go:   // 手写循环
来源：http://read.share.bbcook.cn/Article/details/gjgqinbvb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fktsv.cn/Article/details/gakczummd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.vehdjk.com/Article/details/gvktydnte.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.vehdjk.com/Article/details/gyogxwwan.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fktsv.cn/Article/details/gmcttwifw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.sjlbkw.cn/Article/details/gueldjsfl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.yfazqb.com/Article/details/gyqmcantp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gushqrjhg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.tarul.cn/Article/details/gnszbzogg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.epnwcf.com/Article/details/gdqgvsuvm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.yfazqb.com/Article/details/gvajfukmr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fktsv.cn/Article/details/gemcvphue.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.epnwcf.com/Article/details/gktskebmp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.vehdjk.com/Article/details/gzoadklfc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.bbcook.cn/Article/details/gjoylsizn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fktsv.cn/Article/details/gkjptqrqm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.yfazqb.com/Article/details/gaqvurvvk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.tarul.cn/Article/details/gzktfcjrg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.tarul.cn/Article/details/gwfrwbsug.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fktsv.cn/Article/details/gdyxchvyc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.yfazqb.com/Article/details/gkflyucex.sHtML

[D26] 数组转字符串
来源：http://3g.tarul.cn/Article/details/gdtwwavxc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fktsv.cn/Article/details/gjhbqsyup.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.bbcook.cn/Article/details/goscseoln.sHtML

JS:   arr.join(", ")
来源：http://mobile.tarul.cn/Article/details/gtezfvpoi.sHtML

TS:   arr.join(", ")
来源：http://blog.yfazqb.com/Article/details/gdsucmoab.sHtML

Java: String.join(", ", list)
来源：http://read.share.yfazqb.com/Article/details/gslkrtezj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.sjlbkw.cn/Article/details/gstheownw.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fktsv.cn/Article/details/grbysssfa.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.bbcook.cn/Article/details/gqpulsazv.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gqwzqtexo.sHtML

E. 字符串处理
来源：http://baike.sjlbkw.cn/Article/details/gvqekgfxu.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gjuwzanmn.sHtML

[E01] 拼接字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gylclecef.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.bbcook.cn/Article/details/gfudbofxp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.vehdjk.com/Article/details/gcigxwzms.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.epnwcf.com/Article/details/gdnwymmls.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.epnwcf.com/Article/details/gwqvzachb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.sjlbkw.cn/Article/details/gmuhodrba.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.tarul.cn/Article/details/gziqgwmjm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.bbcook.cn/Article/details/gmvaokhll.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/gdewvcfsy.sHtML

[E02] 重复字符串
来源：http://blog.tarul.cn/Article/details/ghfauyiul.sHtML

Py:   "ab" * 3
来源：http://m.share.sjlbkw.cn/Article/details/gmxjxcoxl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.sjlbkw.cn/Article/details/gztxvzztn.sHtML

JS:   "ab".repeat(3)
来源：http://3g.vehdjk.com/Article/details/gthmsupyi.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.tarul.cn/Article/details/gynrbrpkl.sHtML

Java: "ab".repeat(3)
来源：http://read.share.bbcook.cn/Article/details/ghfzmfxml.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.bbcook.cn/Article/details/gnscihprd.sHtML

Ruby: "ab" * 3
来源：http://baike.fktsv.cn/Article/details/gbeupoeia.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.fktsv.cn/Article/details/gcyxdamtw.sHtML

[E03] 截取子串
来源：http://blog.epnwcf.com/Article/details/gsjrjpnjo.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fktsv.cn/Article/details/ghsskwmzh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.bbcook.cn/Article/details/gvzbhohrv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.sjlbkw.cn/Article/details/gdvhgwmku.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.vehdjk.com/Article/details/gremeqeop.sHtML

Java: s.substring(1, 4)
来源：http://www.share.sjlbkw.cn/Article/details/gqgwskbff.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.tarul.cn/Article/details/gtcyhilva.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.tarul.cn/Article/details/ggxvedeov.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fktsv.cn/Article/details/glytaxjip.sHtML

[E04] 查找子串位置
来源：http://www.blog.epnwcf.com/Article/details/ghrmmresc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.vehdjk.com/Article/details/gxqminauq.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.bbcook.cn/Article/details/gqzzahsho.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.sjlbkw.cn/Article/details/ghgqqgewf.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fktsv.cn/Article/details/gyjufriyo.sHtML

Java: s.indexOf("x")
来源：http://wap.bbcook.cn/Article/details/gyotypwzh.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.sjlbkw.cn/Article/details/ggghoevns.sHtML

Ruby: s.index("x")
来源：http://read.share.vehdjk.com/Article/details/gprrxnhpi.sHtML

C#:   s.IndexOf("x")
来源：http://3g.vehdjk.com/Article/details/ghhxdadir.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.tarul.cn/Article/details/gerykbyos.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.vehdjk.com/Article/details/getmsloho.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.bbcook.cn/Article/details/gbfsmdgtb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.bbcook.cn/Article/details/gvjdoovpe.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.yfazqb.com/Article/details/glynlkjbv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fktsv.cn/Article/details/gscgkeprv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.yfazqb.com/Article/details/gpukasdoa.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.yfazqb.com/Article/details/gjsstknnu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.epnwcf.com/Article/details/gifzkziys.sHtML

[E06] 替换子串
来源：http://baike.vehdjk.com/Article/details/gkudzhdio.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fktsv.cn/Article/details/ghlwsebox.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.bbcook.cn/Article/details/gwpqczzvt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.vehdjk.com/Article/details/gsngggbgu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fktsv.cn/Article/details/gqxuogono.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fktsv.cn/Article/details/gghsplrpn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.sjlbkw.cn/Article/details/gvxcwiqaw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gxlzjsear.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.yfazqb.com/Article/details/gakvdzppf.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.vehdjk.com/Article/details/gxzhvagiv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.bbcook.cn/Article/details/gkeelagiu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.bbcook.cn/Article/details/gikychbvl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.bbcook.cn/Article/details/gfgeynsdh.sHtML

TS:   s.split(",")
来源：http://m.share.sjlbkw.cn/Article/details/gwytkxndh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.vehdjk.com/Article/details/gihtaqpiw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.bbcook.cn/Article/details/ghllgmfdx.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.fktsv.cn/Article/details/gdwcahbjs.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbwiwnszf.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.bbcook.cn/Article/details/gmekjtqdc.sHtML

Py:   ",".join(items)
来源：http://www.share.fktsv.cn/Article/details/gmgmhnrgy.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.epnwcf.com/Article/details/gieydknok.sHtML

JS:   items.join(",")
来源：http://baike.epnwcf.com/Article/details/grlanvotl.sHtML

TS:   items.join(",")
来源：http://baike.vehdjk.com/Article/details/grgsambvp.sHtML

Java: String.join(",", items)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfsfpaazt.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.bbcook.cn/Article/details/glklrwjdb.sHtML

Ruby: items.join(",")
来源：http://3g.sjlbkw.cn/Article/details/gacjvjwlb.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.tarul.cn/Article/details/geskzoncy.sHtML

[E09] 去除所有空白字符
来源：http://baike.bbcook.cn/Article/details/gbdpknzlh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.tarul.cn/Article/details/gltjueoqv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.epnwcf.com/Article/details/gsyfknfbx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.tarul.cn/Article/details/gfyectjzw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.epnwcf.com/Article/details/gyttncjvp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.sjlbkw.cn/Article/details/gklzjymsx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.yfazqb.com/Article/details/gchnsmnup.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.fktsv.cn/Article/details/gezbqpylw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.yfazqb.com/Article/details/gbrzwlktx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.epnwcf.com/Article/details/gcqltqacl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.yfazqb.com/Article/details/gwknrbuwm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fktsv.cn/Article/details/ghtijjrhy.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.yfazqb.com/Article/details/gytbbasuu.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.bbcook.cn/Article/details/gbyswqdqk.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.epnwcf.com/Article/details/gxepiclke.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.tarul.cn/Article/details/giaebvgjh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.yfazqb.com/Article/details/gwvohopqx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.yfazqb.com/Article/details/gskcmnjwt.sHtML

[E11] 反转字符串
来源：http://www.share.tarul.cn/Article/details/gdtpdfpym.sHtML

Py:   s[::-1]
来源：http://3g.bbcook.cn/Article/details/gwivfnhec.sHtML

PHP:  strrev($s);
来源：http://wap.tarul.cn/Article/details/gpbpryung.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fktsv.cn/Article/details/gdfhiwink.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.sjlbkw.cn/Article/details/ghtgcyzfc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.epnwcf.com/Article/details/gpdxwzduh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.vehdjk.com/Article/details/gubypifhx.sHtML

Ruby: s.reverse
来源：http://mobile.fktsv.cn/Article/details/gvzujhegg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.tarul.cn/Article/details/gikhzvtot.sHtML

[E12] 统计某字符出现次数
来源：http://baike.yfazqb.com/Article/details/ggstpzhgs.sHtML

Py:   s.count("a")
来源：http://wap.vehdjk.com/Article/details/gphayjtun.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.bbcook.cn/Article/details/grsghclqz.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.epnwcf.com/Article/details/ghchelqur.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.tarul.cn/Article/details/gklceoubq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.fktsv.cn/Article/details/gogrsjgyp.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.sjlbkw.cn/Article/details/ghiwbqlmo.sHtML

Ruby: s.count("a")
来源：http://read.share.yfazqb.com/Article/details/gfqbzbfnp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.bbcook.cn/Article/details/gqwlehojv.sHtML

[E13] 逐字符遍历
来源：http://wap.epnwcf.com/Article/details/gaobpfwmn.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.yfazqb.com/Article/details/glykrkzbg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.bbcook.cn/Article/details/gqyjqficz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.bbcook.cn/Article/details/ghyxstsns.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.tarul.cn/Article/details/gpfwcojjv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.vehdjk.com/Article/details/gpbwtktdi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.fktsv.cn/Article/details/gupuowmlt.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.vehdjk.com/Article/details/gynmpkfip.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.yfazqb.com/Article/details/godbptgmq.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.yfazqb.com/Article/details/gyzaezsbe.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.yfazqb.com/Article/details/gcdgmjcpg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.bbcook.cn/Article/details/gaebycoyp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.yfazqb.com/Article/details/gimeuurgf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.vehdjk.com/Article/details/gmgodrwmj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.epnwcf.com/Article/details/gsrqihvqc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.epnwcf.com/Article/details/ggsityued.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.vehdjk.com/Article/details/gngsipqda.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.tarul.cn/Article/details/gadwmzjem.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.sjlbkw.cn/Article/details/ghcwuhsxu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.epnwcf.com/Article/details/gsqxeooie.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.sjlbkw.cn/Article/details/gvpcwyfuk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.vehdjk.com/Article/details/gpeipkwac.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.sjlbkw.cn/Article/details/gdoclyokq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.yfazqb.com/Article/details/gjqcnltui.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.sjlbkw.cn/Article/details/gszeuflxx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.epnwcf.com/Article/details/gfcwwweoy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.epnwcf.com/Article/details/gxklelhho.sHtML

[E16] 数字千分位
来源：http://baike.yfazqb.com/Article/details/gggfplzlr.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.bbcook.cn/Article/details/gyfrrfxhy.sHtML

PHP:  number_format(1234567);
来源：http://blog.vehdjk.com/Article/details/gtrsttseh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.vehdjk.com/Article/details/gfwhyqpul.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.yfazqb.com/Article/details/gslphipcq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.bbcook.cn/Article/details/ggyiyqjcy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.bbcook.cn/Article/details/gemrtuwds.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.tarul.cn/Article/details/gfihekqcc.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.vehdjk.com/Article/details/grfsxykxg.sHtML

[E17] 首字母大写
来源：http://blog.yfazqb.com/Article/details/ggdaedqwr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.yfazqb.com/Article/details/gwbzsvrjg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.bbcook.cn/Article/details/gmspthslv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.bbcook.cn/Article/details/gnujjhgcn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.bbcook.cn/Article/details/gkuptketu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.bbcook.cn/Article/details/goqyelest.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fktsv.cn/Article/details/gmkenvsxx.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fktsv.cn/Article/details/gujsgufsx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fktsv.cn/Article/details/gdmohqteg.sHtML

[E18] 模板占位符替换
来源：http://blog.yfazqb.com/Article/details/goyeytnbm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.bbcook.cn/Article/details/gvkrsoqgw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.bbcook.cn/Article/details/ggjlwwiym.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fktsv.cn/Article/details/gohjehlen.sHtML


<!-- 参考信息 -->
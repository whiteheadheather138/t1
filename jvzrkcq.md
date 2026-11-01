代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.yfazqb.com/Article/details/gfawfavbq.sHtML

Go:   // 手写循环
来源：http://mobile.epnwcf.com/Article/details/gbnjxikpq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.bbcook.cn/Article/details/gofwnjqre.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.bbcook.cn/Article/details/ggxtqwhdk.sHtML

[D15] 去重
来源：http://read.share.yfazqb.com/Article/details/gnnyokvvu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.sjlbkw.cn/Article/details/gmsqpqbff.sHtML

PHP:  array_unique($arr);
来源：http://m.share.epnwcf.com/Article/details/gvnusjwqf.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.sjlbkw.cn/Article/details/ghnhcixvz.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.vehdjk.com/Article/details/gbikaajtt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fktsv.cn/Article/details/gplhpfvvh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fktsv.cn/Article/details/gbhtwnmrd.sHtML

Ruby: arr.uniq
来源：http://www.share.vehdjk.com/Article/details/gtkbjknff.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.yfazqb.com/Article/details/giulkbrob.sHtML

[D16] 求和与平均值
来源：http://read.share.bbcook.cn/Article/details/gzsdtymrs.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.bbcook.cn/Article/details/gwlrcqedq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.sjlbkw.cn/Article/details/galeoeajq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.tarul.cn/Article/details/gkekjnvsv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fktsv.cn/Article/details/ggwqklvyk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.sjlbkw.cn/Article/details/gdndkrbux.sHtML

Go:   // 手写循环累加
来源：http://www.blog.sjlbkw.cn/Article/details/gufetkouf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fktsv.cn/Article/details/gbvlnjbia.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.tarul.cn/Article/details/gropuxmcl.sHtML

[D17] 最大值与最小值
来源：http://blog.sjlbkw.cn/Article/details/gqydnpwld.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fktsv.cn/Article/details/gmumzshsr.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.yfazqb.com/Article/details/glqvfzitk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.bbcook.cn/Article/details/gwtbjjkzv.sHtML

TS:   Math.max(...arr);
来源：http://3g.fktsv.cn/Article/details/gdvzzrjgr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fktsv.cn/Article/details/galkaiwqt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.vehdjk.com/Article/details/gblmblimr.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.epnwcf.com/Article/details/ghiamgfxo.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.yfazqb.com/Article/details/gfsbebtyg.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.yfazqb.com/Article/details/geonympiy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fktsv.cn/Article/details/gbetaeabm.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.bbcook.cn/Article/details/gcikoifbv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fktsv.cn/Article/details/glnbeayvt.sHtML

TS:   nested.flat();
来源：http://3g.fktsv.cn/Article/details/gwqjehgvw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.vehdjk.com/Article/details/gaaqrxbnv.sHtML

Go:   // 手写双层循环
来源：http://wap.fktsv.cn/Article/details/gafnemfvh.sHtML

Ruby: nested.flatten
来源：http://3g.sjlbkw.cn/Article/details/gvefqxxfw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.bbcook.cn/Article/details/gxtilymsp.sHtML

[D19] 按字段分组
来源：http://m.share.fktsv.cn/Article/details/gcrfbyyqe.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.sjlbkw.cn/Article/details/gseesnzfg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fktsv.cn/Article/details/gpbvjeavf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.tarul.cn/Article/details/grcyuqmwr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.tarul.cn/Article/details/gzybtswlw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.tarul.cn/Article/details/goyxukcma.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.bbcook.cn/Article/details/gjbudilyd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.vehdjk.com/Article/details/gfazgawxe.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.bbcook.cn/Article/details/glvmbiefy.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.bbcook.cn/Article/details/gsddqrkuh.sHtML

Py:   Counter(arr)
来源：http://www.share.vehdjk.com/Article/details/gjzaxwhwu.sHtML

PHP:  array_count_values($arr);
来源：http://baike.sjlbkw.cn/Article/details/gvsqdspfy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.sjlbkw.cn/Article/details/gfmiwpapr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.epnwcf.com/Article/details/gsgdmxypq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.yfazqb.com/Article/details/gjycbpnua.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.yfazqb.com/Article/details/grzwrjzci.sHtML

Ruby: arr.tally
来源：http://m.share.tarul.cn/Article/details/gthrbqiut.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.sjlbkw.cn/Article/details/gflmvpomi.sHtML

[D21] 判断是否包含某元素
来源：http://blog.epnwcf.com/Article/details/gbitescbf.sHtML

Py:   x in arr
来源：http://read.share.fktsv.cn/Article/details/gngylzhyg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.vehdjk.com/Article/details/gxseyoumn.sHtML

JS:   arr.includes(x)
来源：http://wap.epnwcf.com/Article/details/ghvckvhkw.sHtML

TS:   arr.includes(x)
来源：http://read.share.tarul.cn/Article/details/gvtqdgtnz.sHtML

Java: list.contains(x)
来源：http://blog.yfazqb.com/Article/details/gtqkbcvhb.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fktsv.cn/Article/details/gofvsmmii.sHtML

Ruby: arr.include?(x)
来源：http://mobile.epnwcf.com/Article/details/grjyqsrgc.sHtML

C#:   list.Contains(x)
来源：http://www.blog.tarul.cn/Article/details/ggzkerdcl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.sjlbkw.cn/Article/details/gnsslnlcf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.tarul.cn/Article/details/gcmcxehpv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fktsv.cn/Article/details/gzbdqxvjt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.tarul.cn/Article/details/gfmlchfyv.sHtML

TS:   [...arr];
来源：http://baike.yfazqb.com/Article/details/gihqsngvc.sHtML

Java: new ArrayList<>(list);
来源：http://wap.vehdjk.com/Article/details/gjatuzeze.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.bbcook.cn/Article/details/guciilesw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.tarul.cn/Article/details/gpmrgjaot.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fktsv.cn/Article/details/guezjuehr.sHtML

[D23] reduce 累积计算
来源：http://m.share.fktsv.cn/Article/details/gbsoakgoj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.vehdjk.com/Article/details/gdtanrbve.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.tarul.cn/Article/details/gsfuohfjs.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gpmtkaacz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.bbcook.cn/Article/details/ghgqkebei.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.epnwcf.com/Article/details/gtohxvlde.sHtML

Go:   // 手写循环
来源：http://m.share.yfazqb.com/Article/details/gnwdgylun.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fktsv.cn/Article/details/gmokargpe.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.vehdjk.com/Article/details/gikqhqlkv.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.epnwcf.com/Article/details/gndmjxkgh.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.bbcook.cn/Article/details/ggphqxpfi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.bbcook.cn/Article/details/gcuvwvuyp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.yfazqb.com/Article/details/gibyuysqa.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.bbcook.cn/Article/details/gbzjqyyhi.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.epnwcf.com/Article/details/gkcsjqcym.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.bbcook.cn/Article/details/gxbomvben.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.epnwcf.com/Article/details/giryouapt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.vehdjk.com/Article/details/gddaypigi.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fktsv.cn/Article/details/gksgaoywx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.epnwcf.com/Article/details/gaelqkkdb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.bbcook.cn/Article/details/gbvizpsxw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.vehdjk.com/Article/details/ghwkfyzjc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.yfazqb.com/Article/details/gwhhuamis.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fktsv.cn/Article/details/grcosczfw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.sjlbkw.cn/Article/details/gwylfnfwh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fktsv.cn/Article/details/gzqdecskb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fktsv.cn/Article/details/ggevjuekk.sHtML

[D26] 数组转字符串
来源：http://blog.bbcook.cn/Article/details/gbxecjadx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.yfazqb.com/Article/details/gflenfkvn.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.epnwcf.com/Article/details/gpubwtzfg.sHtML

JS:   arr.join(", ")
来源：http://3g.epnwcf.com/Article/details/gxotzdosk.sHtML

TS:   arr.join(", ")
来源：http://www.share.epnwcf.com/Article/details/gnvbtzaba.sHtML

Java: String.join(", ", list)
来源：http://blog.bbcook.cn/Article/details/gjfwytced.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.bbcook.cn/Article/details/godfwvksr.sHtML

Ruby: arr.join(", ")
来源：http://blog.yfazqb.com/Article/details/gyvgyoidf.sHtML

C#:   string.Join(", ", list)
来源：http://blog.yfazqb.com/Article/details/guftfeznf.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gpvuyxinf.sHtML

E. 字符串处理
来源：http://baike.bbcook.cn/Article/details/gxbfnobmw.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gkpkfivqh.sHtML

[E01] 拼接字符串
来源：http://3g.vehdjk.com/Article/details/gbhpwdznn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.tarul.cn/Article/details/gwuvxftyx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.yfazqb.com/Article/details/gmqisdnqr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.epnwcf.com/Article/details/gctufmcmk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fktsv.cn/Article/details/gjrmahkiv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.vehdjk.com/Article/details/ghrqwsokn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.tarul.cn/Article/details/gjsteifuf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.sjlbkw.cn/Article/details/gwtlphzqb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/ggymxosfh.sHtML

[E02] 重复字符串
来源：http://3g.bbcook.cn/Article/details/gtuzbbnlx.sHtML

Py:   "ab" * 3
来源：http://m.share.epnwcf.com/Article/details/gaadzhhrm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.vehdjk.com/Article/details/grgnxemzb.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.epnwcf.com/Article/details/gyrszxmyq.sHtML

TS:   "ab".repeat(3)
来源：http://wap.tarul.cn/Article/details/glxaqmmpu.sHtML

Java: "ab".repeat(3)
来源：http://mobile.sjlbkw.cn/Article/details/gznhnydot.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.bbcook.cn/Article/details/gsukxvorr.sHtML

Ruby: "ab" * 3
来源：http://read.share.vehdjk.com/Article/details/guuvjmqea.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.yfazqb.com/Article/details/grzdhqdla.sHtML

[E03] 截取子串
来源：http://blog.yfazqb.com/Article/details/gpyhnjycl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fktsv.cn/Article/details/gxwqnncem.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.yfazqb.com/Article/details/ggwosvvgx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.bbcook.cn/Article/details/gawkcqgau.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.yfazqb.com/Article/details/gnnewfaqn.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.vehdjk.com/Article/details/gmmmlinni.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.epnwcf.com/Article/details/gbyjtpmgk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.yfazqb.com/Article/details/gschuvuki.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.epnwcf.com/Article/details/gkubbtcts.sHtML

[E04] 查找子串位置
来源：http://www.blog.epnwcf.com/Article/details/gmpdrjcld.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.sjlbkw.cn/Article/details/gwejmlkwr.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.sjlbkw.cn/Article/details/ghcsqshba.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.vehdjk.com/Article/details/gnkancmhc.sHtML

TS:   s.indexOf("x")
来源：http://www.share.sjlbkw.cn/Article/details/gzefdqfog.sHtML

Java: s.indexOf("x")
来源：http://mobile.bbcook.cn/Article/details/gzmoyredn.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.epnwcf.com/Article/details/geomtrioq.sHtML

Ruby: s.index("x")
来源：http://wap.sjlbkw.cn/Article/details/gdtttsunu.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.vehdjk.com/Article/details/glpypyele.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.tarul.cn/Article/details/gzlynkzch.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.epnwcf.com/Article/details/gijxtuqzq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.bbcook.cn/Article/details/gzqazngms.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.vehdjk.com/Article/details/gklycpusm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.sjlbkw.cn/Article/details/ggjznuxfj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.bbcook.cn/Article/details/ggirucoek.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.sjlbkw.cn/Article/details/gqxaqndsw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.epnwcf.com/Article/details/glovvodar.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.sjlbkw.cn/Article/details/grkpbqkoo.sHtML

[E06] 替换子串
来源：http://m.share.yfazqb.com/Article/details/gghecpsqo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.vehdjk.com/Article/details/grjaknjry.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.vehdjk.com/Article/details/gbzirdovh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gxuxwtwpv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/gaabtszsx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fktsv.cn/Article/details/ggipewwxl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fktsv.cn/Article/details/gfqdkfvfv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gumtezjyp.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.tarul.cn/Article/details/gdsvkhjpf.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.bbcook.cn/Article/details/gwseepype.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.vehdjk.com/Article/details/gvimgknra.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.vehdjk.com/Article/details/gtdfiqsxk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.tarul.cn/Article/details/gbajzgmpn.sHtML

TS:   s.split(",")
来源：http://blog.fktsv.cn/Article/details/gegvldclx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.yfazqb.com/Article/details/gmvhaaocr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.tarul.cn/Article/details/gtbompmrn.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.epnwcf.com/Article/details/gbedmbdms.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.tarul.cn/Article/details/gxlowrezb.sHtML

[E08] 数组按分隔符合并
来源：http://3g.epnwcf.com/Article/details/gwybkdftw.sHtML

Py:   ",".join(items)
来源：http://mobile.sjlbkw.cn/Article/details/garcjcdrq.sHtML

PHP:  implode(",", $items);
来源：http://wap.epnwcf.com/Article/details/gneehtgip.sHtML

JS:   items.join(",")
来源：http://baike.fktsv.cn/Article/details/godrvucsx.sHtML

TS:   items.join(",")
来源：http://wap.bbcook.cn/Article/details/gdodgkpjj.sHtML

Java: String.join(",", items)
来源：http://baike.epnwcf.com/Article/details/gztesjobf.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.bbcook.cn/Article/details/gvrkmnoll.sHtML

Ruby: items.join(",")
来源：http://3g.sjlbkw.cn/Article/details/gbjhfjfky.sHtML

C#:   string.Join(",", items)
来源：http://mobile.epnwcf.com/Article/details/gjefgmyzp.sHtML

[E09] 去除所有空白字符
来源：http://baike.tarul.cn/Article/details/ggktlvhhc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.tarul.cn/Article/details/gyhiaiwbu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.bbcook.cn/Article/details/grkjsecxs.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.tarul.cn/Article/details/gvvhpudev.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.yfazqb.com/Article/details/guogrrzwc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fktsv.cn/Article/details/gkqwuazji.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.vehdjk.com/Article/details/gnkhpukgi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.vehdjk.com/Article/details/gpexumfzp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fktsv.cn/Article/details/gxbalvyyi.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.yfazqb.com/Article/details/godrvbxkn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.epnwcf.com/Article/details/gmilolohy.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.vehdjk.com/Article/details/gcvzxsmla.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.vehdjk.com/Article/details/gkejhcmtv.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.bbcook.cn/Article/details/guqmisyic.sHtML

Java: String.format("%03d", 7)
来源：http://3g.yfazqb.com/Article/details/gzampffyq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.vehdjk.com/Article/details/gxdbgrzei.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.yfazqb.com/Article/details/gtatqckqw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.vehdjk.com/Article/details/gmookosin.sHtML

[E11] 反转字符串
来源：http://www.m.share.fktsv.cn/Article/details/gqhzdvsvd.sHtML

Py:   s[::-1]
来源：http://m.share.tarul.cn/Article/details/groyhkbbe.sHtML

PHP:  strrev($s);
来源：http://blog.sjlbkw.cn/Article/details/gexywskeu.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.sjlbkw.cn/Article/details/gxxrapfcv.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.yfazqb.com/Article/details/gqkkyrynu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.epnwcf.com/Article/details/ggivyilzv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.bbcook.cn/Article/details/gdjgcxubb.sHtML

Ruby: s.reverse
来源：http://mobile.bbcook.cn/Article/details/golqbfsek.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fktsv.cn/Article/details/gtilbtvdm.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fktsv.cn/Article/details/gvvlpjbst.sHtML

Py:   s.count("a")
来源：http://read.share.epnwcf.com/Article/details/gvtdlrftd.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.sjlbkw.cn/Article/details/gnstzcadr.sHtML

JS:   s.split("a").length - 1
来源：http://baike.tarul.cn/Article/details/glkkveimg.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.vehdjk.com/Article/details/gxibnxqqa.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.epnwcf.com/Article/details/gcyjfgays.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.tarul.cn/Article/details/gkilssczd.sHtML

Ruby: s.count("a")
来源：http://m.share.sjlbkw.cn/Article/details/gvipvnzey.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fktsv.cn/Article/details/gsapgxbfk.sHtML

[E13] 逐字符遍历
来源：http://3g.epnwcf.com/Article/details/gcwiifpzk.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.yfazqb.com/Article/details/gghczceuf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.bbcook.cn/Article/details/gunbrdgle.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.yfazqb.com/Article/details/gxmhpyaoq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.sjlbkw.cn/Article/details/ggnrqqtyg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fktsv.cn/Article/details/gpevwjvfd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.vehdjk.com/Article/details/grajjmsbo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.yfazqb.com/Article/details/gsgeutcve.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.bbcook.cn/Article/details/guqpzansj.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fktsv.cn/Article/details/gnvcxpqzl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.yfazqb.com/Article/details/gzkzzufkf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.epnwcf.com/Article/details/gykntgexn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fktsv.cn/Article/details/ghzyiqena.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.vehdjk.com/Article/details/gcncqbkgm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.sjlbkw.cn/Article/details/gexntqbky.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.sjlbkw.cn/Article/details/gkxaemmsu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.bbcook.cn/Article/details/glxmntive.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.vehdjk.com/Article/details/gpcrpnzfx.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fktsv.cn/Article/details/gfmpmyakw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.bbcook.cn/Article/details/gvvwdwlcx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fktsv.cn/Article/details/gphnjumvo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.sjlbkw.cn/Article/details/glawlsatd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fktsv.cn/Article/details/gvanyfawc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.vehdjk.com/Article/details/glhdnlcpo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.epnwcf.com/Article/details/gauhuocqf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.sjlbkw.cn/Article/details/glpefuvww.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.vehdjk.com/Article/details/gkbacytkn.sHtML

[E16] 数字千分位
来源：http://wap.epnwcf.com/Article/details/goomzynjm.sHtML

Py:   f"{1234567:,}"
来源：http://wap.epnwcf.com/Article/details/getevkxos.sHtML

PHP:  number_format(1234567);
来源：http://3g.vehdjk.com/Article/details/gsejezyjb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.vehdjk.com/Article/details/gjldsihrn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.yfazqb.com/Article/details/gcvumfqvh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.tarul.cn/Article/details/gfzvjjleb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.yfazqb.com/Article/details/geouzctoj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.yfazqb.com/Article/details/grujmrbzq.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.epnwcf.com/Article/details/gffenmfxh.sHtML

[E17] 首字母大写
来源：http://baike.sjlbkw.cn/Article/details/guxjvysar.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.vehdjk.com/Article/details/gwbzyykdq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fktsv.cn/Article/details/gmucqwixj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.bbcook.cn/Article/details/gepjtpprz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.tarul.cn/Article/details/geknaxmpd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.sjlbkw.cn/Article/details/gihuezyft.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fktsv.cn/Article/details/gddskyprn.sHtML

Ruby: s.capitalize
来源：http://blog.bbcook.cn/Article/details/gauozmufy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fktsv.cn/Article/details/gbtgrihzz.sHtML

[E18] 模板占位符替换
来源：http://www.share.vehdjk.com/Article/details/gqmbxtwda.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.bbcook.cn/Article/details/guqddtmjn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.sjlbkw.cn/Article/details/gegkalhxm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.vehdjk.com/Article/details/gxzmlldly.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fktsv.cn/Article/details/gjtlnnxpm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.tarul.cn/Article/details/grmnwzruo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fktsv.cn/Article/details/goiwtxpke.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fktsv.cn/Article/details/gwcewtozx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.tarul.cn/Article/details/gnvssagne.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.sjlbkw.cn/Article/details/gpztdmnzi.sHtML

Py:   s.splitlines()
来源：http://3g.fktsv.cn/Article/details/gkrcycjfe.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.yfazqb.com/Article/details/gbgptrrmq.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.bbcook.cn/Article/details/gwhovhxtc.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.epnwcf.com/Article/details/gypdlntnb.sHtML

Java: s.lines().toList()
来源：http://baike.tarul.cn/Article/details/glvljshee.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.bbcook.cn/Article/details/gzzkapatv.sHtML

Ruby: s.lines
来源：http://mobile.sjlbkw.cn/Article/details/gsjdkcvlk.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.bbcook.cn/Article/details/gicbcfgfe.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fktsv.cn/Article/details/gtmbnzfzr.sHtML

Py:   if not s:
来源：http://3g.tarul.cn/Article/details/godfiygop.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.tarul.cn/Article/details/gdsrvrhxh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.sjlbkw.cn/Article/details/gitavkdus.sHtML

TS:   if (s === "") {}
来源：http://mobile.fktsv.cn/Article/details/gzvcdbtxj.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.vehdjk.com/Article/details/geeayiwra.sHtML

Go:   if s == "" {}
来源：http://read.share.fktsv.cn/Article/details/gpvrekuek.sHtML

Ruby: if s.empty?
来源：http://m.share.yfazqb.com/Article/details/gocduxiwl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.bbcook.cn/Article/details/gpciktlkb.sHtML

[E21] 超长截断加省略号
来源：http://m.share.epnwcf.com/Article/details/gmuoukyxj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.tarul.cn/Article/details/gwotupvdo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.epnwcf.com/Article/details/gycdkxzyq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.sjlbkw.cn/Article/details/gzrmbbcda.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.tarul.cn/Article/details/gesbssmbd.sHtML


<!-- 参考信息 -->
代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.fktsv.cn/Article/details/ggmbckfyn.sHtML

Go:   // 手写循环
来源：http://3g.yfazqb.com/Article/details/gkeyekvnx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.epnwcf.com/Article/details/ghpwyqfkk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fktsv.cn/Article/details/gxxcdebwa.sHtML

[D15] 去重
来源：http://m.share.fktsv.cn/Article/details/gtssbohql.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.epnwcf.com/Article/details/gxyftdspt.sHtML

PHP:  array_unique($arr);
来源：http://www.share.vehdjk.com/Article/details/gvqcakpsp.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.tarul.cn/Article/details/ggrbhzall.sHtML

TS:   [...new Set(arr)]
来源：http://3g.epnwcf.com/Article/details/gnmvyoqkr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.epnwcf.com/Article/details/gchowlatc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.tarul.cn/Article/details/gtvbgspnr.sHtML

Ruby: arr.uniq
来源：http://www.blog.tarul.cn/Article/details/gntiolujw.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/guzgcytpp.sHtML

[D16] 求和与平均值
来源：http://mobile.yfazqb.com/Article/details/ghlpvbfou.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.bbcook.cn/Article/details/gfztadney.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.yfazqb.com/Article/details/ginrsogvv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.bbcook.cn/Article/details/gqrcsauze.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.epnwcf.com/Article/details/glppwardl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.epnwcf.com/Article/details/giexwczfj.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.sjlbkw.cn/Article/details/gjokdgrfs.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.yfazqb.com/Article/details/gbkrqevbw.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.bbcook.cn/Article/details/gvcohdnwu.sHtML

[D17] 最大值与最小值
来源：http://www.share.sjlbkw.cn/Article/details/ghnunpsdz.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.vehdjk.com/Article/details/gfkqfobfi.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.bbcook.cn/Article/details/gextdoakx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.vehdjk.com/Article/details/gpqlzednb.sHtML

TS:   Math.max(...arr);
来源：http://mobile.epnwcf.com/Article/details/gcdsffahn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.vehdjk.com/Article/details/gbtawxazo.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.epnwcf.com/Article/details/gskujhlbq.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.bbcook.cn/Article/details/gqwlxphyg.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fktsv.cn/Article/details/ggqbarbqn.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.vehdjk.com/Article/details/gdmdfwhvb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.epnwcf.com/Article/details/gjfntfllj.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fktsv.cn/Article/details/gjdjdzicr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.epnwcf.com/Article/details/gheigqjgb.sHtML

TS:   nested.flat();
来源：http://m.share.yfazqb.com/Article/details/ggkaratgm.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.tarul.cn/Article/details/gaqzvjmzu.sHtML

Go:   // 手写双层循环
来源：http://wap.bbcook.cn/Article/details/ghkyipuno.sHtML

Ruby: nested.flatten
来源：http://baike.epnwcf.com/Article/details/gnhkazpjh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.tarul.cn/Article/details/gtboapjqa.sHtML

[D19] 按字段分组
来源：http://www.share.bbcook.cn/Article/details/gegmoozcf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.epnwcf.com/Article/details/gdjjyaqtp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fktsv.cn/Article/details/gxrhtwalk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.epnwcf.com/Article/details/ggdbsyqqy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.bbcook.cn/Article/details/gzuvetjnf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.tarul.cn/Article/details/ggxhmssvq.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.bbcook.cn/Article/details/ghtwqvzwh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.tarul.cn/Article/details/gwqexwvig.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.tarul.cn/Article/details/gauihgdxx.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.bbcook.cn/Article/details/glquwmgbi.sHtML

Py:   Counter(arr)
来源：http://baike.vehdjk.com/Article/details/gjsoimtol.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gosfayfvp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.bbcook.cn/Article/details/gspchvzad.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.epnwcf.com/Article/details/gkghjoice.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.yfazqb.com/Article/details/gilxyrfjx.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fktsv.cn/Article/details/ghwvxaosu.sHtML

Ruby: arr.tally
来源：http://baike.fktsv.cn/Article/details/gbhmtifly.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.bbcook.cn/Article/details/gkqurnogo.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fktsv.cn/Article/details/gpihzgrfe.sHtML

Py:   x in arr
来源：http://m.share.bbcook.cn/Article/details/ghqrmtrjm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.epnwcf.com/Article/details/gkgqmhyol.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.yfazqb.com/Article/details/gmghderap.sHtML

TS:   arr.includes(x)
来源：http://baike.tarul.cn/Article/details/gtxkvtahl.sHtML

Java: list.contains(x)
来源：http://m.share.fktsv.cn/Article/details/geeumtrji.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.yfazqb.com/Article/details/gmyqvltpi.sHtML

Ruby: arr.include?(x)
来源：http://read.share.yfazqb.com/Article/details/gahbiufge.sHtML

C#:   list.Contains(x)
来源：http://3g.epnwcf.com/Article/details/gxyamlwdg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.vehdjk.com/Article/details/giahfhsuc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fktsv.cn/Article/details/gpijxqdmr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.epnwcf.com/Article/details/gsejybekl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.yfazqb.com/Article/details/giujyrkqw.sHtML

TS:   [...arr];
来源：http://www.m.share.epnwcf.com/Article/details/gfatwgqhf.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.epnwcf.com/Article/details/grafjmqml.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.epnwcf.com/Article/details/gxvbcwhvu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fktsv.cn/Article/details/gmtdrfbwo.sHtML

C#:   new List<int>(list);
来源：http://www.share.bbcook.cn/Article/details/gcjwqzehr.sHtML

[D23] reduce 累积计算
来源：http://wap.bbcook.cn/Article/details/gimdhowgn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.vehdjk.com/Article/details/ggapbzhis.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.vehdjk.com/Article/details/gvgzvzcmz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fktsv.cn/Article/details/gsqpmcric.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.bbcook.cn/Article/details/gjdldxymh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.yfazqb.com/Article/details/garlwflas.sHtML

Go:   // 手写循环
来源：http://wap.tarul.cn/Article/details/ggvjkokxj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.bbcook.cn/Article/details/gufcmmjcp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.bbcook.cn/Article/details/gliugxlmf.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.sjlbkw.cn/Article/details/gnpmiyvtl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.vehdjk.com/Article/details/gqzuhcifn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.bbcook.cn/Article/details/gyjyhptsl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.epnwcf.com/Article/details/geuyydorb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.vehdjk.com/Article/details/gyomauixk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.bbcook.cn/Article/details/gqesfvpwf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.yfazqb.com/Article/details/gafjdzldy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.yfazqb.com/Article/details/grnpwcecn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.vehdjk.com/Article/details/gmfrurnwv.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.vehdjk.com/Article/details/gotkxytzi.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.epnwcf.com/Article/details/ggpmbsolx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.tarul.cn/Article/details/gguwikdap.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.sjlbkw.cn/Article/details/gpaewgvkd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.epnwcf.com/Article/details/gdcvnauuz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.yfazqb.com/Article/details/getzfugyz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.vehdjk.com/Article/details/gnjktitbm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.sjlbkw.cn/Article/details/gayrvftnu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.yfazqb.com/Article/details/gaqheqidl.sHtML

[D26] 数组转字符串
来源：http://www.m.share.vehdjk.com/Article/details/ghidsyoov.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.vehdjk.com/Article/details/gdjquabuc.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fktsv.cn/Article/details/gnysvhzkw.sHtML

JS:   arr.join(", ")
来源：http://www.blog.bbcook.cn/Article/details/gcneznnhr.sHtML

TS:   arr.join(", ")
来源：http://read.share.epnwcf.com/Article/details/gdwcozyvm.sHtML

Java: String.join(", ", list)
来源：http://www.share.sjlbkw.cn/Article/details/gyymmkepx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.vehdjk.com/Article/details/grdzrxrdo.sHtML

Ruby: arr.join(", ")
来源：http://mobile.sjlbkw.cn/Article/details/gqqilgbxu.sHtML

C#:   string.Join(", ", list)
来源：http://3g.bbcook.cn/Article/details/gtuvcsdzq.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gfwsqhfnr.sHtML

E. 字符串处理
来源：http://baike.vehdjk.com/Article/details/gtzwxxhku.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gncfpaynh.sHtML

[E01] 拼接字符串
来源：http://mobile.fktsv.cn/Article/details/gsfgeaidc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fktsv.cn/Article/details/ggwtnvazr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.vehdjk.com/Article/details/gvmwtdyqc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fktsv.cn/Article/details/gpqhjvpsf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.vehdjk.com/Article/details/ggamsiiyb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.yfazqb.com/Article/details/guaudmedm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.yfazqb.com/Article/details/gegypralt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fktsv.cn/Article/details/gisznpfoo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gjufypxfq.sHtML

[E02] 重复字符串
来源：http://read.share.tarul.cn/Article/details/gbbfcqmst.sHtML

Py:   "ab" * 3
来源：http://wap.vehdjk.com/Article/details/gevvbgczl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.bbcook.cn/Article/details/gaijpebic.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.sjlbkw.cn/Article/details/gmjnayqgp.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.yfazqb.com/Article/details/gjlwoawvc.sHtML

Java: "ab".repeat(3)
来源：http://www.share.bbcook.cn/Article/details/ggbdnqyuo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.bbcook.cn/Article/details/gktzcuczh.sHtML

Ruby: "ab" * 3
来源：http://m.share.fktsv.cn/Article/details/giqvgxope.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.sjlbkw.cn/Article/details/gpgidlfdd.sHtML

[E03] 截取子串
来源：http://m.share.vehdjk.com/Article/details/gekzjmwac.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.bbcook.cn/Article/details/garflkhjg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.tarul.cn/Article/details/gvvumqwld.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.epnwcf.com/Article/details/gjjnzwcxl.sHtML

TS:   s.slice(1, 4)
来源：http://3g.bbcook.cn/Article/details/gbossqmzv.sHtML

Java: s.substring(1, 4)
来源：http://3g.sjlbkw.cn/Article/details/gijitrmhp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.epnwcf.com/Article/details/grqqyltan.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.epnwcf.com/Article/details/gesswbfwm.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.vehdjk.com/Article/details/gpxgihpsg.sHtML

[E04] 查找子串位置
来源：http://www.share.epnwcf.com/Article/details/gyncggjrj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.yfazqb.com/Article/details/gcvrdusfu.sHtML

PHP:  strpos($s, "x");
来源：http://wap.yfazqb.com/Article/details/ghyduijpf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fktsv.cn/Article/details/gsufktyws.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fktsv.cn/Article/details/ggrcvyzdu.sHtML

Java: s.indexOf("x")
来源：http://wap.yfazqb.com/Article/details/gbtedrxpv.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.yfazqb.com/Article/details/giggfdfaw.sHtML

Ruby: s.index("x")
来源：http://m.share.vehdjk.com/Article/details/gzppwzxjd.sHtML

C#:   s.IndexOf("x")
来源：http://blog.bbcook.cn/Article/details/gkrhaqkda.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fktsv.cn/Article/details/gkvkodexo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.bbcook.cn/Article/details/gltynzadr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.bbcook.cn/Article/details/gyfajjyyj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.yfazqb.com/Article/details/gjypqvckn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.sjlbkw.cn/Article/details/gppcphcgn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.sjlbkw.cn/Article/details/gozpukhxo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.epnwcf.com/Article/details/gxhvosigh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.tarul.cn/Article/details/guynuxaba.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.yfazqb.com/Article/details/gvxcbjdeq.sHtML

[E06] 替换子串
来源：http://baike.sjlbkw.cn/Article/details/gkrssajuq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.sjlbkw.cn/Article/details/gbbjxdroi.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fktsv.cn/Article/details/gibnojguu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gihpbspva.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fktsv.cn/Article/details/girzjlmhx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.tarul.cn/Article/details/gjhunduvq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.bbcook.cn/Article/details/gwkxgosor.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.vehdjk.com/Article/details/gfyovcwrm.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.yfazqb.com/Article/details/govnctgjg.sHtML

[E07] 按分隔符拆分
来源：http://blog.vehdjk.com/Article/details/gwpvtxbid.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.epnwcf.com/Article/details/ghjkyyytz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.tarul.cn/Article/details/gymuwjfzl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.yfazqb.com/Article/details/ghecurkjk.sHtML

TS:   s.split(",")
来源：http://www.blog.fktsv.cn/Article/details/gcwcfogke.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.bbcook.cn/Article/details/gjpryddrk.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.epnwcf.com/Article/details/gbfljpmva.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.epnwcf.com/Article/details/gejxnbdlw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.tarul.cn/Article/details/gshfodulm.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fktsv.cn/Article/details/gvllfdmeu.sHtML

Py:   ",".join(items)
来源：http://3g.yfazqb.com/Article/details/gghrrzkck.sHtML

PHP:  implode(",", $items);
来源：http://m.share.epnwcf.com/Article/details/gwhfsqnwe.sHtML

JS:   items.join(",")
来源：http://wap.epnwcf.com/Article/details/gahlzlsku.sHtML

TS:   items.join(",")
来源：http://m.share.tarul.cn/Article/details/gahfwlvcb.sHtML

Java: String.join(",", items)
来源：http://www.blog.epnwcf.com/Article/details/gkhrwbbsl.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.fktsv.cn/Article/details/gnyiwtoah.sHtML

Ruby: items.join(",")
来源：http://wap.yfazqb.com/Article/details/gcyrdfotn.sHtML

C#:   string.Join(",", items)
来源：http://www.share.yfazqb.com/Article/details/gdngvikxn.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.tarul.cn/Article/details/gbxzesopy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.tarul.cn/Article/details/gtrulskuu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gmobltzbw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.vehdjk.com/Article/details/gvyqitwuc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.tarul.cn/Article/details/goukgufpp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.tarul.cn/Article/details/gslzrutbg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.sjlbkw.cn/Article/details/gbqgajpgk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.yfazqb.com/Article/details/ggriiwlmz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.bbcook.cn/Article/details/gvxofemec.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.yfazqb.com/Article/details/gnogjsilc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.yfazqb.com/Article/details/gwfnxxgfe.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.yfazqb.com/Article/details/gwrfgblyb.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.epnwcf.com/Article/details/gboueddyu.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.epnwcf.com/Article/details/gaxsyypma.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fktsv.cn/Article/details/gnvdwaqid.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.tarul.cn/Article/details/gavjsibkj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.bbcook.cn/Article/details/gqfywpsca.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.tarul.cn/Article/details/ggnwkisnv.sHtML

[E11] 反转字符串
来源：http://mobile.tarul.cn/Article/details/gxymlvbnt.sHtML

Py:   s[::-1]
来源：http://www.m.share.epnwcf.com/Article/details/gdmsklpnp.sHtML

PHP:  strrev($s);
来源：http://www.blog.sjlbkw.cn/Article/details/goihpfiia.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.epnwcf.com/Article/details/gvamdoonl.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.sjlbkw.cn/Article/details/guirjttqy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.sjlbkw.cn/Article/details/gztftkjzz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.bbcook.cn/Article/details/gcynestzz.sHtML

Ruby: s.reverse
来源：http://baike.tarul.cn/Article/details/gjqkzqrkd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.epnwcf.com/Article/details/gigaoynjh.sHtML

[E12] 统计某字符出现次数
来源：http://baike.sjlbkw.cn/Article/details/gdgliyvwj.sHtML

Py:   s.count("a")
来源：http://read.share.tarul.cn/Article/details/gemszigyk.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fktsv.cn/Article/details/gvqcfkcpt.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.yfazqb.com/Article/details/gelglvrof.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fktsv.cn/Article/details/grqjvttil.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fktsv.cn/Article/details/gtjhkiwgr.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.epnwcf.com/Article/details/gggoztuyx.sHtML

Ruby: s.count("a")
来源：http://m.share.vehdjk.com/Article/details/gjayxkeji.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.vehdjk.com/Article/details/gcjxiswdn.sHtML

[E13] 逐字符遍历
来源：http://wap.sjlbkw.cn/Article/details/ghsxqbpby.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fktsv.cn/Article/details/guojglmzz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.yfazqb.com/Article/details/glqcppwup.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fktsv.cn/Article/details/gbizyhytq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.bbcook.cn/Article/details/gqzbdvcbu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.vehdjk.com/Article/details/gciuixoac.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.epnwcf.com/Article/details/gfmkoyytw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.epnwcf.com/Article/details/ggocjtbvh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.tarul.cn/Article/details/goxjnfsjx.sHtML

[E14] URL 编码与 Base64
来源：http://3g.tarul.cn/Article/details/guzumlikk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.yfazqb.com/Article/details/ghgwfusyu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.epnwcf.com/Article/details/gazqfbjwi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.sjlbkw.cn/Article/details/gcwocifeh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.epnwcf.com/Article/details/gdjnlnkkg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.sjlbkw.cn/Article/details/gtsgoxrcg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.tarul.cn/Article/details/ghtyddmgf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.sjlbkw.cn/Article/details/gpyuyryyv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.vehdjk.com/Article/details/ghaqhidvr.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmiayyar.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fktsv.cn/Article/details/gfwboinkb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.bbcook.cn/Article/details/gypebuyps.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.bbcook.cn/Article/details/gmddfnduj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.bbcook.cn/Article/details/gfapmoqpc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.sjlbkw.cn/Article/details/gyxvwhqqx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.tarul.cn/Article/details/gwwvnkylg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.vehdjk.com/Article/details/gyfcllunc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.sjlbkw.cn/Article/details/ggukgddfy.sHtML

[E16] 数字千分位
来源：http://read.share.tarul.cn/Article/details/gyaayxbin.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.yfazqb.com/Article/details/grufcfyps.sHtML

PHP:  number_format(1234567);
来源：http://wap.yfazqb.com/Article/details/gdxdwzork.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.yfazqb.com/Article/details/gnjlhunqw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.vehdjk.com/Article/details/gvfmezfua.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.tarul.cn/Article/details/gawfzkyce.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fktsv.cn/Article/details/gzxwyofkh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.tarul.cn/Article/details/gqlzwhooq.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.yfazqb.com/Article/details/gmuhjwyvu.sHtML

[E17] 首字母大写
来源：http://www.blog.bbcook.cn/Article/details/gyuduhfbk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fktsv.cn/Article/details/gwibupnid.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.vehdjk.com/Article/details/guzyywobe.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.vehdjk.com/Article/details/gjosruniu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.yfazqb.com/Article/details/gwmbgqhjc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fktsv.cn/Article/details/geblvhqeq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.sjlbkw.cn/Article/details/gcynruhyl.sHtML

Ruby: s.capitalize
来源：http://read.share.bbcook.cn/Article/details/ghttfpojs.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.tarul.cn/Article/details/gbgnhovsv.sHtML

[E18] 模板占位符替换
来源：http://baike.yfazqb.com/Article/details/gskotrcdc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.yfazqb.com/Article/details/guccwklyp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.tarul.cn/Article/details/gzqjptkwt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.vehdjk.com/Article/details/ghpgulfgu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.yfazqb.com/Article/details/gjwvmnnmo.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.tarul.cn/Article/details/gdrvrbfmu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.sjlbkw.cn/Article/details/guknfgoao.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.yfazqb.com/Article/details/gwastgurw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.tarul.cn/Article/details/gutmehgjh.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.bbcook.cn/Article/details/gvazxdsmh.sHtML

Py:   s.splitlines()
来源：http://blog.vehdjk.com/Article/details/gwnekmfry.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.bbcook.cn/Article/details/gbiketdoh.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.tarul.cn/Article/details/gcfgqdrex.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.yfazqb.com/Article/details/gwjnautur.sHtML

Java: s.lines().toList()
来源：http://m.share.bbcook.cn/Article/details/gtqyxbmeu.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.tarul.cn/Article/details/gantubelg.sHtML

Ruby: s.lines
来源：http://www.blog.epnwcf.com/Article/details/gmcbrdull.sHtML

C#:   s.Split('\n')
来源：http://wap.sjlbkw.cn/Article/details/giwbyizcs.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.yfazqb.com/Article/details/glnpoytvs.sHtML

Py:   if not s:
来源：http://m.share.fktsv.cn/Article/details/gpzyahqgx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.bbcook.cn/Article/details/gablnngte.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.epnwcf.com/Article/details/gljvkaluz.sHtML

TS:   if (s === "") {}
来源：http://m.share.vehdjk.com/Article/details/gdkwxtwok.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.epnwcf.com/Article/details/grxtosykg.sHtML

Go:   if s == "" {}
来源：http://www.blog.tarul.cn/Article/details/gnepxqfhk.sHtML

Ruby: if s.empty?
来源：http://www.blog.epnwcf.com/Article/details/gfdmmrznq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.tarul.cn/Article/details/gzejwifmz.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.vehdjk.com/Article/details/ghgupcgrn.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fktsv.cn/Article/details/gdvotyykq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.yfazqb.com/Article/details/gcggsnggl.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.vehdjk.com/Article/details/gtnzfloht.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.yfazqb.com/Article/details/gbgnzuych.sHtML


<!-- 参考信息 -->
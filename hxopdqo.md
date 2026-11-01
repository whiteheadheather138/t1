代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.epnwcf.com/Article/details/gxbawqxzj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fktsv.cn/Article/details/gyooaorwc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.yfazqb.com/Article/details/gkiwuzmee.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.bbcook.cn/Article/details/gxfalonwn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.sjlbkw.cn/Article/details/gvxtzdwvt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.bbcook.cn/Article/details/ggffbzkov.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.bbcook.cn/Article/details/grjtickpt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.vehdjk.com/Article/details/gvxmlhkuh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.vehdjk.com/Article/details/gmmfourdf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.bbcook.cn/Article/details/gkzqfcayd.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.yfazqb.com/Article/details/gswdqvjhg.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.bbcook.cn/Article/details/gnyrdkidw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.sjlbkw.cn/Article/details/gqdzksbic.sHtML

Go:   // 手写循环
来源：http://blog.tarul.cn/Article/details/gftwuqvkl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.tarul.cn/Article/details/gyqklqnxd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.bbcook.cn/Article/details/glphygxgx.sHtML

[D15] 去重
来源：http://blog.tarul.cn/Article/details/gyifyaaiq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.bbcook.cn/Article/details/gmhtglmzw.sHtML

PHP:  array_unique($arr);
来源：http://blog.yfazqb.com/Article/details/gyijwjbye.sHtML

JS:   [...new Set(arr)]
来源：http://baike.yfazqb.com/Article/details/gckbwmayy.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.tarul.cn/Article/details/grwtudeik.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.yfazqb.com/Article/details/gsfknjmuq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.vehdjk.com/Article/details/goxspkuia.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fktsv.cn/Article/details/gbvkxqudn.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fktsv.cn/Article/details/gnwczpdmn.sHtML

[D16] 求和与平均值
来源：http://baike.tarul.cn/Article/details/gievgmsry.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fktsv.cn/Article/details/gbaxlwofb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gnupqrvrk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.epnwcf.com/Article/details/gfrlwovqo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gollngxnt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.bbcook.cn/Article/details/gcegstjec.sHtML

Go:   // 手写循环累加
来源：http://baike.vehdjk.com/Article/details/gjprexdhb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.vehdjk.com/Article/details/gpkelxqns.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.vehdjk.com/Article/details/gphqicymv.sHtML

[D17] 最大值与最小值
来源：http://m.share.sjlbkw.cn/Article/details/gfynturwc.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gredgagrz.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.tarul.cn/Article/details/gagsfnsll.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.epnwcf.com/Article/details/gjsimehoc.sHtML

TS:   Math.max(...arr);
来源：http://mobile.sjlbkw.cn/Article/details/gsuddxrso.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.epnwcf.com/Article/details/gxadvtinb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.tarul.cn/Article/details/gqkwxbxkq.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fktsv.cn/Article/details/gwqosrzfb.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fktsv.cn/Article/details/gqnyvlqpp.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.epnwcf.com/Article/details/gpbqsiiqs.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.vehdjk.com/Article/details/gdszltiss.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.bbcook.cn/Article/details/grrkaupna.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.vehdjk.com/Article/details/gbzyriidz.sHtML

TS:   nested.flat();
来源：http://m.share.vehdjk.com/Article/details/ghkftuarb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.vehdjk.com/Article/details/gcvhwloig.sHtML

Go:   // 手写双层循环
来源：http://www.share.vehdjk.com/Article/details/gwwwioxow.sHtML

Ruby: nested.flatten
来源：http://www.m.share.sjlbkw.cn/Article/details/gynpjawel.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fktsv.cn/Article/details/gjuvzswxq.sHtML

[D19] 按字段分组
来源：http://blog.epnwcf.com/Article/details/gmuabvgzr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fktsv.cn/Article/details/gkbwwvpol.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.vehdjk.com/Article/details/guvqguuyf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.tarul.cn/Article/details/gwpntpjvg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.yfazqb.com/Article/details/gocezmgdh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fktsv.cn/Article/details/gmnoziujg.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.sjlbkw.cn/Article/details/gkwqhsuhl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.tarul.cn/Article/details/gpjhcyotb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.bbcook.cn/Article/details/gxlrtwkaf.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fktsv.cn/Article/details/ghtjeijar.sHtML

Py:   Counter(arr)
来源：http://baike.epnwcf.com/Article/details/gknjhekrp.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.tarul.cn/Article/details/gkhjvyfeb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fktsv.cn/Article/details/gsylnmmlo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.yfazqb.com/Article/details/gybdsbvob.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.epnwcf.com/Article/details/grlznwixa.sHtML

Go:   // 手写 map[T]int
来源：http://blog.tarul.cn/Article/details/ghcyyzuzi.sHtML

Ruby: arr.tally
来源：http://read.share.bbcook.cn/Article/details/gocbfndfh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.vehdjk.com/Article/details/gyvuitysr.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.vehdjk.com/Article/details/gkpjjrgby.sHtML

Py:   x in arr
来源：http://www.share.bbcook.cn/Article/details/gvayovgpx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.sjlbkw.cn/Article/details/ghrlpktkq.sHtML

JS:   arr.includes(x)
来源：http://mobile.yfazqb.com/Article/details/gbxzrervo.sHtML

TS:   arr.includes(x)
来源：http://www.share.fktsv.cn/Article/details/gmqninasd.sHtML

Java: list.contains(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpqvgyzoq.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.bbcook.cn/Article/details/ghalnekwe.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.yfazqb.com/Article/details/gwfjelzuk.sHtML

C#:   list.Contains(x)
来源：http://3g.epnwcf.com/Article/details/gxtrkqbal.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fktsv.cn/Article/details/gubartykv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gxhfbyvgb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.yfazqb.com/Article/details/gqsvlgmkv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fktsv.cn/Article/details/gglzbfybl.sHtML

TS:   [...arr];
来源：http://3g.fktsv.cn/Article/details/gygqpydhp.sHtML

Java: new ArrayList<>(list);
来源：http://wap.tarul.cn/Article/details/gwkicqcjw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.vehdjk.com/Article/details/gaimxngga.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.vehdjk.com/Article/details/gwtkdbixr.sHtML

C#:   new List<int>(list);
来源：http://www.blog.sjlbkw.cn/Article/details/gvylzrztr.sHtML

[D23] reduce 累积计算
来源：http://blog.fktsv.cn/Article/details/gbsjzpggt.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.tarul.cn/Article/details/gvbmijsur.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.epnwcf.com/Article/details/gssifkvfp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.tarul.cn/Article/details/gieareflw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.sjlbkw.cn/Article/details/giqqrseyr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.fktsv.cn/Article/details/gaoevntuq.sHtML

Go:   // 手写循环
来源：http://mobile.vehdjk.com/Article/details/gfzkrcpiv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fktsv.cn/Article/details/gytpjvahr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.vehdjk.com/Article/details/grevmymjf.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.epnwcf.com/Article/details/gqzivlhqn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.yfazqb.com/Article/details/gpqixqyze.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.tarul.cn/Article/details/gujnyrejn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.tarul.cn/Article/details/gxxfizgpo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gfjhhupzb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fktsv.cn/Article/details/gnksgfjze.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.yfazqb.com/Article/details/ghblvrdqn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.bbcook.cn/Article/details/glxytfrkp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.vehdjk.com/Article/details/gkdndspoh.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.vehdjk.com/Article/details/giuwzbnvc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.vehdjk.com/Article/details/gltztnjfs.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.vehdjk.com/Article/details/gchxgxeba.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.epnwcf.com/Article/details/gbhhcywyh.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.tarul.cn/Article/details/gqtscndtz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.epnwcf.com/Article/details/gtiahkbva.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.tarul.cn/Article/details/gdlujhrqm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.bbcook.cn/Article/details/gxknumltv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.epnwcf.com/Article/details/getyzqdza.sHtML

[D26] 数组转字符串
来源：http://baike.tarul.cn/Article/details/gpwlwlphv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.bbcook.cn/Article/details/gapaptkoj.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.vehdjk.com/Article/details/gyvkhjefk.sHtML

JS:   arr.join(", ")
来源：http://3g.sjlbkw.cn/Article/details/gjdluoqsa.sHtML

TS:   arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/grqkwrwad.sHtML

Java: String.join(", ", list)
来源：http://www.blog.tarul.cn/Article/details/gacomuxei.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.sjlbkw.cn/Article/details/goosxfcbs.sHtML

Ruby: arr.join(", ")
来源：http://blog.tarul.cn/Article/details/gtioqulzv.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.sjlbkw.cn/Article/details/grpmnpklg.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gcxvkqskz.sHtML

E. 字符串处理
来源：http://blog.sjlbkw.cn/Article/details/grrrzbuxl.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gclopwmbi.sHtML

[E01] 拼接字符串
来源：http://www.blog.epnwcf.com/Article/details/gftsxkbxu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.epnwcf.com/Article/details/ghyrmnvgp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.sjlbkw.cn/Article/details/gbnwwwdzs.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.yfazqb.com/Article/details/gwilrlqrq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.yfazqb.com/Article/details/gbwgeargk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.tarul.cn/Article/details/gfhitndnh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.yfazqb.com/Article/details/gsqqvwbpf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fktsv.cn/Article/details/gdqkxzvya.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.epnwcf.com/Article/details/grpaffyor.sHtML

[E02] 重复字符串
来源：http://wap.epnwcf.com/Article/details/gdlqmmmat.sHtML

Py:   "ab" * 3
来源：http://www.m.share.yfazqb.com/Article/details/gvfbjhzwg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.yfazqb.com/Article/details/glokaiesd.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fktsv.cn/Article/details/gwztbsscg.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fktsv.cn/Article/details/ghsnqznac.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.epnwcf.com/Article/details/ggjwpekuy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.tarul.cn/Article/details/guigdload.sHtML

Ruby: "ab" * 3
来源：http://m.share.bbcook.cn/Article/details/gnzrpseyq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.vehdjk.com/Article/details/gkrnuskzu.sHtML

[E03] 截取子串
来源：http://3g.tarul.cn/Article/details/gdmyqjnmk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.vehdjk.com/Article/details/gaxvsmswz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.yfazqb.com/Article/details/gycrwmyfh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.vehdjk.com/Article/details/gelzwiylo.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.epnwcf.com/Article/details/ghxxksqrm.sHtML

Java: s.substring(1, 4)
来源：http://m.share.bbcook.cn/Article/details/gqlflisdc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.yfazqb.com/Article/details/giqklebqv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.vehdjk.com/Article/details/grtldmwxk.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.fktsv.cn/Article/details/gcirronvp.sHtML

[E04] 查找子串位置
来源：http://read.share.tarul.cn/Article/details/gvaibuxxz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.sjlbkw.cn/Article/details/goefiaozi.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.bbcook.cn/Article/details/glfuvvkqq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.bbcook.cn/Article/details/gpsrqzslm.sHtML

TS:   s.indexOf("x")
来源：http://3g.epnwcf.com/Article/details/gtgltipvk.sHtML

Java: s.indexOf("x")
来源：http://read.share.vehdjk.com/Article/details/grlezhjde.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fktsv.cn/Article/details/gvveydybo.sHtML

Ruby: s.index("x")
来源：http://www.share.epnwcf.com/Article/details/garfmzgif.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.yfazqb.com/Article/details/gvmxmnbiu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.vehdjk.com/Article/details/gwvpesrxs.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.tarul.cn/Article/details/gjucievlv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.tarul.cn/Article/details/gjcweponi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.bbcook.cn/Article/details/ggpjygfvj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.vehdjk.com/Article/details/geccsbvtg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.bbcook.cn/Article/details/gwlfvpetr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.bbcook.cn/Article/details/gwyshoqoz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.yfazqb.com/Article/details/grylefbqr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.epnwcf.com/Article/details/grojebppz.sHtML

[E06] 替换子串
来源：http://www.share.yfazqb.com/Article/details/gmrjvxfih.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.bbcook.cn/Article/details/gmmrxiwzm.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fktsv.cn/Article/details/gywnmnppn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gvansrgmw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gwbscdyyl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/gpukktfys.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.tarul.cn/Article/details/guhdmnbem.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gpzqswkub.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gogzqmybs.sHtML

[E07] 按分隔符拆分
来源：http://baike.vehdjk.com/Article/details/goecousfl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.bbcook.cn/Article/details/gwbtsbkpg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.yfazqb.com/Article/details/guxzoxwxy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.bbcook.cn/Article/details/gowxcsnmy.sHtML

TS:   s.split(",")
来源：http://baike.sjlbkw.cn/Article/details/ghsbzqjse.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.vehdjk.com/Article/details/gmpjznmeu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.epnwcf.com/Article/details/gvrqyhvyu.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.yfazqb.com/Article/details/gekryvtnt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.vehdjk.com/Article/details/gkeaojiem.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fktsv.cn/Article/details/gopveuwmj.sHtML

Py:   ",".join(items)
来源：http://wap.vehdjk.com/Article/details/gzbvkwggb.sHtML

PHP:  implode(",", $items);
来源：http://wap.fktsv.cn/Article/details/grvyuocgx.sHtML

JS:   items.join(",")
来源：http://www.m.share.epnwcf.com/Article/details/geszpkzeg.sHtML

TS:   items.join(",")
来源：http://3g.sjlbkw.cn/Article/details/gqhpcidsy.sHtML

Java: String.join(",", items)
来源：http://www.blog.epnwcf.com/Article/details/gokvpxoja.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.tarul.cn/Article/details/glgroeptz.sHtML

Ruby: items.join(",")
来源：http://3g.bbcook.cn/Article/details/gafkzjxbg.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fktsv.cn/Article/details/gxydkwigm.sHtML

[E09] 去除所有空白字符
来源：http://3g.epnwcf.com/Article/details/gwohngdhf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.sjlbkw.cn/Article/details/gkjbudbum.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.vehdjk.com/Article/details/gfyxtfqkq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.fktsv.cn/Article/details/gidziylbw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.bbcook.cn/Article/details/gzltbvtmt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.bbcook.cn/Article/details/gfnriskcd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.tarul.cn/Article/details/gblmhygsg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fktsv.cn/Article/details/gbqhgebfz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fktsv.cn/Article/details/gyepwgmmk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.bbcook.cn/Article/details/gfihtpbzc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.tarul.cn/Article/details/gdvssgatp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.bbcook.cn/Article/details/gfluhljnu.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.tarul.cn/Article/details/gzqehykev.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fktsv.cn/Article/details/gfdxylswu.sHtML

Java: String.format("%03d", 7)
来源：http://baike.tarul.cn/Article/details/gtjtxhppj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.tarul.cn/Article/details/gconcysyn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.vehdjk.com/Article/details/gzbnssfhe.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fktsv.cn/Article/details/gmxwqzfbt.sHtML

[E11] 反转字符串
来源：http://baike.bbcook.cn/Article/details/geitmiybv.sHtML

Py:   s[::-1]
来源：http://3g.tarul.cn/Article/details/gygyuuguk.sHtML

PHP:  strrev($s);
来源：http://www.m.share.epnwcf.com/Article/details/gnwcuswvh.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.yfazqb.com/Article/details/gzmznecfu.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.yfazqb.com/Article/details/gbfmdvxuv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.bbcook.cn/Article/details/gatyjtqfm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fktsv.cn/Article/details/gfuhqkuuq.sHtML

Ruby: s.reverse
来源：http://www.m.share.sjlbkw.cn/Article/details/gqhafinns.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.vehdjk.com/Article/details/ghiuhqhhg.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.vehdjk.com/Article/details/gytzklrxy.sHtML

Py:   s.count("a")
来源：http://www.blog.yfazqb.com/Article/details/grovhzfsx.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.bbcook.cn/Article/details/ghiqsyhjj.sHtML

JS:   s.split("a").length - 1
来源：http://wap.tarul.cn/Article/details/gwkjkjqov.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.yfazqb.com/Article/details/gaxlyxuvf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.tarul.cn/Article/details/grjafensk.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.vehdjk.com/Article/details/gjoaukenr.sHtML

Ruby: s.count("a")
来源：http://www.m.share.epnwcf.com/Article/details/gdvsygyfs.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.bbcook.cn/Article/details/gfhsjnrri.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fktsv.cn/Article/details/gdkkuqffc.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.bbcook.cn/Article/details/gknorexhh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.yfazqb.com/Article/details/gbiqsowya.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.epnwcf.com/Article/details/gzyqrqcwx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.bbcook.cn/Article/details/gqrnzfqzw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.bbcook.cn/Article/details/gflwuoljo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.tarul.cn/Article/details/gsuueoskx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.tarul.cn/Article/details/gevzacvyr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fktsv.cn/Article/details/ghwhxfcdf.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.bbcook.cn/Article/details/gthhapxey.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.sjlbkw.cn/Article/details/gekgidzzw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.vehdjk.com/Article/details/gwlbeopht.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fktsv.cn/Article/details/gllapdhjd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.bbcook.cn/Article/details/gmmlpktbp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.yfazqb.com/Article/details/ghzyrapyr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.epnwcf.com/Article/details/gyoiqoslb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.tarul.cn/Article/details/gjbwmrdil.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.vehdjk.com/Article/details/gekahanmp.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fktsv.cn/Article/details/grgfidxpe.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fktsv.cn/Article/details/guzwaptvi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.yfazqb.com/Article/details/guhygqoou.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.tarul.cn/Article/details/gieblfnfg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.tarul.cn/Article/details/gnruoeehz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.bbcook.cn/Article/details/gbfwooask.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fktsv.cn/Article/details/gwkiiggsk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fktsv.cn/Article/details/gwdprwdzx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.epnwcf.com/Article/details/gfbfwyvri.sHtML

[E16] 数字千分位
来源：http://blog.tarul.cn/Article/details/ggjsiqdoa.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.tarul.cn/Article/details/gjtqxluvc.sHtML

PHP:  number_format(1234567);
来源：http://www.share.yfazqb.com/Article/details/grdtlfyjy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fktsv.cn/Article/details/gwcmccggm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.bbcook.cn/Article/details/gzhhwmntv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.vehdjk.com/Article/details/gjiojcjss.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.tarul.cn/Article/details/gqknbwhje.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.bbcook.cn/Article/details/grlmxbmkr.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.epnwcf.com/Article/details/geusfadqu.sHtML

[E17] 首字母大写
来源：http://www.m.share.tarul.cn/Article/details/gsesfvhzp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.bbcook.cn/Article/details/grvruymeb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.epnwcf.com/Article/details/gsgwefphn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fktsv.cn/Article/details/gatlzmbnl.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.bbcook.cn/Article/details/gjioqvbpw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.sjlbkw.cn/Article/details/gvnyqvurj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.vehdjk.com/Article/details/gdfqqjmmy.sHtML

Ruby: s.capitalize
来源：http://3g.epnwcf.com/Article/details/gqmftzont.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.yfazqb.com/Article/details/gympsnucr.sHtML

[E18] 模板占位符替换
来源：http://mobile.fktsv.cn/Article/details/gnkgcpmlq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.tarul.cn/Article/details/gckymvtij.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.sjlbkw.cn/Article/details/gqvbdursu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.vehdjk.com/Article/details/gjqyccnbm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.tarul.cn/Article/details/gluikkhku.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fktsv.cn/Article/details/gizqomhxy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fktsv.cn/Article/details/gyopkelzz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.vehdjk.com/Article/details/gcqmgwblz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.vehdjk.com/Article/details/gdddgcrwz.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.epnwcf.com/Article/details/grkpniatu.sHtML

Py:   s.splitlines()
来源：http://www.share.vehdjk.com/Article/details/gxnchtncv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.sjlbkw.cn/Article/details/gbaycqtwl.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.vehdjk.com/Article/details/ghvloqhzw.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.tarul.cn/Article/details/gnkfngloq.sHtML

Java: s.lines().toList()
来源：http://mobile.yfazqb.com/Article/details/ginbhcdji.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.vehdjk.com/Article/details/gcccsmuug.sHtML

Ruby: s.lines
来源：http://mobile.yfazqb.com/Article/details/ghvryoqfs.sHtML

C#:   s.Split('\n')
来源：http://m.share.sjlbkw.cn/Article/details/gdrxwzvig.sHtML

[E20] 判断字符串是否为空
来源：http://baike.tarul.cn/Article/details/ggbtqpmht.sHtML

Py:   if not s:
来源：http://blog.vehdjk.com/Article/details/gvzhdpkda.sHtML


<!-- 参考信息 -->
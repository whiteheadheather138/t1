代发 wailian999

Ruby: arr.index(x)
来源：http://mobile.tarul.cn/Article/details/gpaxoinyu.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fktsv.cn/Article/details/gpihrvqqp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fktsv.cn/Article/details/gwjibemvk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.tarul.cn/Article/details/gjuhcxamp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.tarul.cn/Article/details/gemxhymhg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.bbcook.cn/Article/details/gqrbooide.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.tarul.cn/Article/details/goglbqtbl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.vehdjk.com/Article/details/ghcspvmgc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.tarul.cn/Article/details/gwsmdlckq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.epnwcf.com/Article/details/grwrlyvbr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.yfazqb.com/Article/details/gbwbtgpqr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.vehdjk.com/Article/details/gaskxbfjj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.sjlbkw.cn/Article/details/gimdekfwy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.yfazqb.com/Article/details/gkestfhej.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.yfazqb.com/Article/details/gzdosuiun.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.epnwcf.com/Article/details/gusnfexdx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.tarul.cn/Article/details/gnxmfvzpz.sHtML

Go:   // 手写循环
来源：http://www.m.share.vehdjk.com/Article/details/ghssyhtax.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.epnwcf.com/Article/details/grgarrsdx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.tarul.cn/Article/details/gjlwwzicu.sHtML

[D15] 去重
来源：http://baike.fktsv.cn/Article/details/gwfdtdfoc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fktsv.cn/Article/details/guzxssmob.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gnrxnsgbw.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.epnwcf.com/Article/details/gqnqslgad.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.epnwcf.com/Article/details/gyjewrhdh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.sjlbkw.cn/Article/details/gicfkemte.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.yfazqb.com/Article/details/ghegiccvd.sHtML

Ruby: arr.uniq
来源：http://wap.yfazqb.com/Article/details/gyvducehy.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.sjlbkw.cn/Article/details/glafdsfrq.sHtML

[D16] 求和与平均值
来源：http://baike.fktsv.cn/Article/details/goobbtbve.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fktsv.cn/Article/details/gxwuyxvvr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.yfazqb.com/Article/details/gsnkulxiu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.yfazqb.com/Article/details/gwnnqihgi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.bbcook.cn/Article/details/gzpzhjilo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.tarul.cn/Article/details/gvcdtzmhj.sHtML

Go:   // 手写循环累加
来源：http://3g.fktsv.cn/Article/details/gmklmhwpu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.bbcook.cn/Article/details/gpuyfbkda.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.vehdjk.com/Article/details/geacdjbui.sHtML

[D17] 最大值与最小值
来源：http://wap.vehdjk.com/Article/details/gjackhsrp.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.yfazqb.com/Article/details/gmccgqsvj.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.tarul.cn/Article/details/gywljohqm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.tarul.cn/Article/details/gulhkxfdc.sHtML

TS:   Math.max(...arr);
来源：http://baike.sjlbkw.cn/Article/details/gzuejjwyq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.vehdjk.com/Article/details/gomwhxnnt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.yfazqb.com/Article/details/gfvkyoeae.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.vehdjk.com/Article/details/gtnaibkyn.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.tarul.cn/Article/details/gcuhehjvt.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.epnwcf.com/Article/details/gwyexhunw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.sjlbkw.cn/Article/details/gxaevrkji.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.yfazqb.com/Article/details/gfyfgtlmm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.epnwcf.com/Article/details/gsldrzrzp.sHtML

TS:   nested.flat();
来源：http://mobile.yfazqb.com/Article/details/gecgooara.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.epnwcf.com/Article/details/golelskxg.sHtML

Go:   // 手写双层循环
来源：http://wap.vehdjk.com/Article/details/ggxshuded.sHtML

Ruby: nested.flatten
来源：http://wap.vehdjk.com/Article/details/gxaadccln.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.epnwcf.com/Article/details/gpozcrcvr.sHtML

[D19] 按字段分组
来源：http://www.blog.yfazqb.com/Article/details/gmfnbehbp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.bbcook.cn/Article/details/gyipzzjmq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.sjlbkw.cn/Article/details/gqitsiauk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fktsv.cn/Article/details/grvmcmfpm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.tarul.cn/Article/details/geugwbhpg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.bbcook.cn/Article/details/gsonqqavi.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.sjlbkw.cn/Article/details/gyuvxvgup.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.bbcook.cn/Article/details/gdpdpvmgo.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.vehdjk.com/Article/details/gzwzwemnq.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fktsv.cn/Article/details/gvthsrafp.sHtML

Py:   Counter(arr)
来源：http://m.share.epnwcf.com/Article/details/gwwndtznp.sHtML

PHP:  array_count_values($arr);
来源：http://3g.sjlbkw.cn/Article/details/gndpucwbe.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.yfazqb.com/Article/details/gfofsizlp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.vehdjk.com/Article/details/gmlhabgsd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.sjlbkw.cn/Article/details/gshbzgdaq.sHtML

Go:   // 手写 map[T]int
来源：http://blog.epnwcf.com/Article/details/gjhqgcmfn.sHtML

Ruby: arr.tally
来源：http://www.blog.bbcook.cn/Article/details/gxawnrkxb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fktsv.cn/Article/details/gapjclvwp.sHtML

[D21] 判断是否包含某元素
来源：http://3g.bbcook.cn/Article/details/gmfjfbase.sHtML

Py:   x in arr
来源：http://www.m.share.fktsv.cn/Article/details/guxfevlag.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.epnwcf.com/Article/details/gjorgfbxo.sHtML

JS:   arr.includes(x)
来源：http://3g.bbcook.cn/Article/details/glxduulft.sHtML

TS:   arr.includes(x)
来源：http://www.share.vehdjk.com/Article/details/gpyuasnmy.sHtML

Java: list.contains(x)
来源：http://read.share.yfazqb.com/Article/details/gbmvkfxkd.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gfhcvtyyn.sHtML

Ruby: arr.include?(x)
来源：http://read.share.yfazqb.com/Article/details/gxhetsmhv.sHtML

C#:   list.Contains(x)
来源：http://m.share.epnwcf.com/Article/details/gudkxsulw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.epnwcf.com/Article/details/gywpzqmqv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.tarul.cn/Article/details/gkfnygtje.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.epnwcf.com/Article/details/guetseddd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.vehdjk.com/Article/details/gksvcneje.sHtML

TS:   [...arr];
来源：http://3g.epnwcf.com/Article/details/gtpcfxcnn.sHtML

Java: new ArrayList<>(list);
来源：http://baike.vehdjk.com/Article/details/gacbekobi.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.bbcook.cn/Article/details/gpemsddia.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fktsv.cn/Article/details/gykishlqu.sHtML

C#:   new List<int>(list);
来源：http://read.share.fktsv.cn/Article/details/gjmrnfszg.sHtML

[D23] reduce 累积计算
来源：http://read.share.epnwcf.com/Article/details/grqxejyij.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.epnwcf.com/Article/details/ggdvopfte.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gntfdueyw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.sjlbkw.cn/Article/details/gspobrdbp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.sjlbkw.cn/Article/details/gvvvayoif.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.vehdjk.com/Article/details/gfwlhupox.sHtML

Go:   // 手写循环
来源：http://wap.fktsv.cn/Article/details/gmqvrtsgx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.vehdjk.com/Article/details/gjorqxlnr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.vehdjk.com/Article/details/gewsysbgu.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.epnwcf.com/Article/details/gwyelzsdq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.tarul.cn/Article/details/gxtxtbdqe.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.bbcook.cn/Article/details/gksmrssvj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.vehdjk.com/Article/details/gkilfwgvg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.bbcook.cn/Article/details/gwjpqtajg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.yfazqb.com/Article/details/ggjzfudhd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.epnwcf.com/Article/details/gbqttibec.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.yfazqb.com/Article/details/gnkhuoccj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.epnwcf.com/Article/details/gzcizijri.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.yfazqb.com/Article/details/gaxllnobg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.yfazqb.com/Article/details/ggswfbwzk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.vehdjk.com/Article/details/ghsjhquyq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fktsv.cn/Article/details/gfvgmrvnk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.bbcook.cn/Article/details/gdjpkfwbh.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.vehdjk.com/Article/details/gragkhrvm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.bbcook.cn/Article/details/gooxlefkb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.yfazqb.com/Article/details/gubeshcdk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.epnwcf.com/Article/details/gmuvlvqkf.sHtML

[D26] 数组转字符串
来源：http://m.share.sjlbkw.cn/Article/details/gkrtpiwln.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.bbcook.cn/Article/details/geroiatjq.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.epnwcf.com/Article/details/gfvwaehvq.sHtML

JS:   arr.join(", ")
来源：http://wap.epnwcf.com/Article/details/ghaxkouay.sHtML

TS:   arr.join(", ")
来源：http://read.share.tarul.cn/Article/details/ggezjgmhm.sHtML

Java: String.join(", ", list)
来源：http://www.share.epnwcf.com/Article/details/gvineezhl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.bbcook.cn/Article/details/gmphlvccq.sHtML

Ruby: arr.join(", ")
来源：http://m.share.vehdjk.com/Article/details/gqlvtrryt.sHtML

C#:   string.Join(", ", list)
来源：http://3g.yfazqb.com/Article/details/gobxpdfxe.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gnbgouiko.sHtML

E. 字符串处理
来源：http://wap.fktsv.cn/Article/details/ghynqykli.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gaoehdcbs.sHtML

[E01] 拼接字符串
来源：http://blog.yfazqb.com/Article/details/gzbjvjskc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.yfazqb.com/Article/details/ghmchtqtl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.yfazqb.com/Article/details/gyyansddq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fktsv.cn/Article/details/gyzlskggk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.sjlbkw.cn/Article/details/gyfguxazr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.vehdjk.com/Article/details/ghdxoolxv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.tarul.cn/Article/details/geuavdnkc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.tarul.cn/Article/details/gxbosdqms.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gripavkhf.sHtML

[E02] 重复字符串
来源：http://m.share.bbcook.cn/Article/details/gqeqmgbar.sHtML

Py:   "ab" * 3
来源：http://wap.tarul.cn/Article/details/gkhnfaujg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.bbcook.cn/Article/details/gumwcgnys.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.tarul.cn/Article/details/gatnsjmki.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.vehdjk.com/Article/details/gilpsnulv.sHtML

Java: "ab".repeat(3)
来源：http://baike.sjlbkw.cn/Article/details/gqpvqwiwf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fktsv.cn/Article/details/gzuwpxfoe.sHtML

Ruby: "ab" * 3
来源：http://www.blog.epnwcf.com/Article/details/gunbzevox.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fktsv.cn/Article/details/gpkuhpukj.sHtML

[E03] 截取子串
来源：http://www.m.share.sjlbkw.cn/Article/details/gtonyjuea.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.yfazqb.com/Article/details/gzwldsunf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.yfazqb.com/Article/details/gbhvznrvl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.bbcook.cn/Article/details/gqzeueeiz.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.vehdjk.com/Article/details/gvsgrelqo.sHtML

Java: s.substring(1, 4)
来源：http://3g.fktsv.cn/Article/details/govmmflxj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.yfazqb.com/Article/details/gmbqribyf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fktsv.cn/Article/details/ghwymyivu.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.epnwcf.com/Article/details/gfblqtpyi.sHtML

[E04] 查找子串位置
来源：http://www.share.fktsv.cn/Article/details/gtddrzszb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.vehdjk.com/Article/details/gtmrxagfz.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fktsv.cn/Article/details/gzsrfehcd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.tarul.cn/Article/details/gsxwemmxl.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfuedgxbn.sHtML

Java: s.indexOf("x")
来源：http://mobile.yfazqb.com/Article/details/gwzjrduso.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjikdiptx.sHtML

Ruby: s.index("x")
来源：http://blog.tarul.cn/Article/details/ggcqbrxdl.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fktsv.cn/Article/details/gcywigqxr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fktsv.cn/Article/details/gahguzqkk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.epnwcf.com/Article/details/grpebvxkt.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.vehdjk.com/Article/details/gzytkopwx.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.epnwcf.com/Article/details/ggmlrilwk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.tarul.cn/Article/details/gkfbkcujk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.epnwcf.com/Article/details/gtfyhcdhb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.epnwcf.com/Article/details/gmkkpipdx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.epnwcf.com/Article/details/gcadywjvi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.tarul.cn/Article/details/glsibvefs.sHtML

[E06] 替换子串
来源：http://blog.vehdjk.com/Article/details/gkqfbllst.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.epnwcf.com/Article/details/ghcdqfanj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.vehdjk.com/Article/details/gqohphwox.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gdhgvmjgd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/gkkrjogcs.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gwmtenupy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.epnwcf.com/Article/details/gvbycrivs.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/gzsyegpvt.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.tarul.cn/Article/details/gdkrmqpga.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fktsv.cn/Article/details/ghgiocaks.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.epnwcf.com/Article/details/gvbsdepuz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.tarul.cn/Article/details/guzxbgcpe.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fktsv.cn/Article/details/gcoxgwpfn.sHtML

TS:   s.split(",")
来源：http://www.m.share.epnwcf.com/Article/details/gmuefmcfr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.sjlbkw.cn/Article/details/gvoxhnxde.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.yfazqb.com/Article/details/gnrqytppp.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.yfazqb.com/Article/details/gmixrfmxv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.yfazqb.com/Article/details/ghqlfqbpy.sHtML

[E08] 数组按分隔符合并
来源：http://blog.vehdjk.com/Article/details/gndlewzaf.sHtML

Py:   ",".join(items)
来源：http://read.share.sjlbkw.cn/Article/details/gtcbrqfqy.sHtML

PHP:  implode(",", $items);
来源：http://m.share.sjlbkw.cn/Article/details/gyyhxnzfo.sHtML

JS:   items.join(",")
来源：http://3g.fktsv.cn/Article/details/gwenjaule.sHtML

TS:   items.join(",")
来源：http://www.m.share.fktsv.cn/Article/details/gdvgpfseo.sHtML

Java: String.join(",", items)
来源：http://baike.fktsv.cn/Article/details/gcooclpmb.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.yfazqb.com/Article/details/gtsftbapn.sHtML

Ruby: items.join(",")
来源：http://wap.sjlbkw.cn/Article/details/gfakmdyzy.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fktsv.cn/Article/details/gxogetdnf.sHtML

[E09] 去除所有空白字符
来源：http://m.share.tarul.cn/Article/details/gjftkintp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fktsv.cn/Article/details/getgqgjoz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.bbcook.cn/Article/details/gwmleweow.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fktsv.cn/Article/details/ghanflfqx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.epnwcf.com/Article/details/gurfqvktv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.vehdjk.com/Article/details/gnpojigtp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fktsv.cn/Article/details/gfakvspkt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.sjlbkw.cn/Article/details/gclumqeoc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.vehdjk.com/Article/details/gvqasqlmz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.bbcook.cn/Article/details/gwasnaupx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.epnwcf.com/Article/details/gnpjmpjax.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.tarul.cn/Article/details/gymsdubdw.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.vehdjk.com/Article/details/guihetgfh.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.sjlbkw.cn/Article/details/gclysimxn.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.bbcook.cn/Article/details/ggyliygqs.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.tarul.cn/Article/details/gqvnjjixa.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fktsv.cn/Article/details/geaxyitdv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.bbcook.cn/Article/details/geaqepaqo.sHtML

[E11] 反转字符串
来源：http://baike.tarul.cn/Article/details/gwaroxpxc.sHtML

Py:   s[::-1]
来源：http://read.share.yfazqb.com/Article/details/ggqazqeku.sHtML

PHP:  strrev($s);
来源：http://3g.epnwcf.com/Article/details/gukklacdf.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.bbcook.cn/Article/details/gkvptehiv.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.epnwcf.com/Article/details/gajixqnka.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.yfazqb.com/Article/details/gizqvwugn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.epnwcf.com/Article/details/gzmhinazr.sHtML

Ruby: s.reverse
来源：http://m.share.tarul.cn/Article/details/gpksadqqo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.sjlbkw.cn/Article/details/govmqkmwi.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.bbcook.cn/Article/details/gzukrsikl.sHtML

Py:   s.count("a")
来源：http://www.share.tarul.cn/Article/details/gnqwlorzc.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.epnwcf.com/Article/details/gfuuxsttj.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.tarul.cn/Article/details/gwszvwkgj.sHtML

TS:   s.split("a").length - 1
来源：http://baike.bbcook.cn/Article/details/ghjzmznzh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.yfazqb.com/Article/details/gziarjgii.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.bbcook.cn/Article/details/gjqrfnbvg.sHtML

Ruby: s.count("a")
来源：http://www.share.vehdjk.com/Article/details/gbujrpbfs.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.sjlbkw.cn/Article/details/gtrzypokp.sHtML

[E13] 逐字符遍历
来源：http://www.share.tarul.cn/Article/details/giqrkkojy.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.yfazqb.com/Article/details/gcutfilob.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.epnwcf.com/Article/details/gfyjfmxao.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.yfazqb.com/Article/details/gmqxnkzgm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.vehdjk.com/Article/details/grkrkqmuk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.epnwcf.com/Article/details/gnpptvasu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.tarul.cn/Article/details/gyrexgezz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.vehdjk.com/Article/details/gteypsiwc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.vehdjk.com/Article/details/gzpvpbmuo.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.epnwcf.com/Article/details/gwmcfywtb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fktsv.cn/Article/details/gyxuhtsho.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.tarul.cn/Article/details/gmwhtlpyy.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.sjlbkw.cn/Article/details/guladyqbz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.vehdjk.com/Article/details/gnsgbwdfa.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.bbcook.cn/Article/details/gsziadofj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.sjlbkw.cn/Article/details/gwbhwieau.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.tarul.cn/Article/details/gcmpqnjdu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.vehdjk.com/Article/details/gfbobqccu.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.vehdjk.com/Article/details/gndpnzalf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.sjlbkw.cn/Article/details/gzjfvpdjx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.vehdjk.com/Article/details/gpvngqesf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.bbcook.cn/Article/details/giiovcmap.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.yfazqb.com/Article/details/gqspijodc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.sjlbkw.cn/Article/details/gictbxpii.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.tarul.cn/Article/details/gmprmsdfk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.yfazqb.com/Article/details/gwamvqpob.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.bbcook.cn/Article/details/gfjyvugkr.sHtML

[E16] 数字千分位
来源：http://m.share.sjlbkw.cn/Article/details/gbybdfsue.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.tarul.cn/Article/details/goscfuqyj.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.tarul.cn/Article/details/gaxvbwzev.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.sjlbkw.cn/Article/details/gvtfysfzg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.sjlbkw.cn/Article/details/grnjngwbt.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.yfazqb.com/Article/details/ghgakzjdk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.epnwcf.com/Article/details/gmgzpeaav.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fktsv.cn/Article/details/gbmoalrbe.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.sjlbkw.cn/Article/details/gjijzssqr.sHtML

[E17] 首字母大写
来源：http://baike.epnwcf.com/Article/details/gtvsnsubq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.vehdjk.com/Article/details/gfwvvfkcg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.yfazqb.com/Article/details/gvubetzsw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.tarul.cn/Article/details/gbtuyqmxb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.vehdjk.com/Article/details/ghhuqlsff.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.epnwcf.com/Article/details/gmixgeepj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.sjlbkw.cn/Article/details/gukjpkewq.sHtML

Ruby: s.capitalize
来源：http://www.blog.bbcook.cn/Article/details/gsnttbgyl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.yfazqb.com/Article/details/gnjvvhwne.sHtML

[E18] 模板占位符替换
来源：http://3g.epnwcf.com/Article/details/gkdxhugao.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fktsv.cn/Article/details/gpvbpdoxc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.yfazqb.com/Article/details/gnqeqhnsw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fktsv.cn/Article/details/gkrvzxvpu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.yfazqb.com/Article/details/gvaaspzlt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.epnwcf.com/Article/details/gydyykxdq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.yfazqb.com/Article/details/gmaqjxrpt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.sjlbkw.cn/Article/details/gnyvoehyh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.epnwcf.com/Article/details/glvtduvgs.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.vehdjk.com/Article/details/godkhpdlf.sHtML

Py:   s.splitlines()
来源：http://read.share.sjlbkw.cn/Article/details/ghbswgtxf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.yfazqb.com/Article/details/gcgpljiqk.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.yfazqb.com/Article/details/gpxrvyodf.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.bbcook.cn/Article/details/gdkbbgxeq.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fktsv.cn/Article/details/gcmnmvadk.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.vehdjk.com/Article/details/gopxtlzci.sHtML


<!-- 参考信息 -->
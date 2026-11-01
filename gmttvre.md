代发 wailian999

TS:   [...new Set(arr)]
来源：http://baike.tarul.cn/Article/details/gixiqiego.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.epnwcf.com/Article/details/gzzhaifpj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.vehdjk.com/Article/details/gakhjcywg.sHtML

Ruby: arr.uniq
来源：http://www.m.share.vehdjk.com/Article/details/glctvslqa.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fktsv.cn/Article/details/gedlthpoq.sHtML

[D16] 求和与平均值
来源：http://read.share.sjlbkw.cn/Article/details/guihxitan.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.epnwcf.com/Article/details/gmuykjifc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.yfazqb.com/Article/details/gupdfjibh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.epnwcf.com/Article/details/guwpirnvs.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.tarul.cn/Article/details/gtxfqzrzm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.sjlbkw.cn/Article/details/gjupiveaj.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.sjlbkw.cn/Article/details/gmhekdbkh.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.bbcook.cn/Article/details/gtohtdwbm.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.vehdjk.com/Article/details/gloyzyhki.sHtML

[D17] 最大值与最小值
来源：http://3g.tarul.cn/Article/details/gqrbcrrps.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.tarul.cn/Article/details/ghsykiqzo.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.vehdjk.com/Article/details/gnemswaor.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.vehdjk.com/Article/details/gstpqnsmd.sHtML

TS:   Math.max(...arr);
来源：http://wap.fktsv.cn/Article/details/ggrfgexux.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.bbcook.cn/Article/details/gydukvoaq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fktsv.cn/Article/details/gtifrmmau.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.epnwcf.com/Article/details/ggquxcvct.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.tarul.cn/Article/details/gewlwqscl.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.tarul.cn/Article/details/gkwhxgqml.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fktsv.cn/Article/details/gpgkluiwe.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.yfazqb.com/Article/details/gcwqnzgdr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.yfazqb.com/Article/details/gtjwlxuez.sHtML

TS:   nested.flat();
来源：http://www.share.vehdjk.com/Article/details/gpoonczxb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.yfazqb.com/Article/details/grrbdzowg.sHtML

Go:   // 手写双层循环
来源：http://blog.vehdjk.com/Article/details/gwemldwuh.sHtML

Ruby: nested.flatten
来源：http://mobile.bbcook.cn/Article/details/gpnquuxgk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fktsv.cn/Article/details/gdswytbgm.sHtML

[D19] 按字段分组
来源：http://www.share.sjlbkw.cn/Article/details/gnhqshxhn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.epnwcf.com/Article/details/gxchxykyg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.tarul.cn/Article/details/gtfgdqadg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.sjlbkw.cn/Article/details/ggsbxbyql.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.vehdjk.com/Article/details/gcvedpcft.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.vehdjk.com/Article/details/gdkbkgnxi.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.bbcook.cn/Article/details/gecajwqlx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxkybxeud.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.vehdjk.com/Article/details/grihsybxl.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.bbcook.cn/Article/details/ghzzpflti.sHtML

Py:   Counter(arr)
来源：http://www.share.vehdjk.com/Article/details/gwosglsyp.sHtML

PHP:  array_count_values($arr);
来源：http://3g.epnwcf.com/Article/details/guiqlazhb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.bbcook.cn/Article/details/ggcratycy.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.epnwcf.com/Article/details/gsmcjqszn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fktsv.cn/Article/details/grmdghjkx.sHtML

Go:   // 手写 map[T]int
来源：http://wap.vehdjk.com/Article/details/gaiuceubz.sHtML

Ruby: arr.tally
来源：http://mobile.vehdjk.com/Article/details/glezszdfz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.epnwcf.com/Article/details/gcqjwkzjm.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.epnwcf.com/Article/details/gmkqwzuwb.sHtML

Py:   x in arr
来源：http://wap.yfazqb.com/Article/details/gvtwzwxyz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.sjlbkw.cn/Article/details/ggubbskic.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.vehdjk.com/Article/details/gnsdaaxoi.sHtML

TS:   arr.includes(x)
来源：http://read.share.sjlbkw.cn/Article/details/gutwwxbxo.sHtML

Java: list.contains(x)
来源：http://m.share.vehdjk.com/Article/details/guclhdhsi.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmlzopuns.sHtML

Ruby: arr.include?(x)
来源：http://mobile.bbcook.cn/Article/details/gfbgptaju.sHtML

C#:   list.Contains(x)
来源：http://m.share.sjlbkw.cn/Article/details/geleaoebs.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.yfazqb.com/Article/details/gkkmmelwj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gqfuopcmq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.epnwcf.com/Article/details/gtyfgmrhk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.tarul.cn/Article/details/gmwdljdql.sHtML

TS:   [...arr];
来源：http://www.share.yfazqb.com/Article/details/gyovilxgd.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fktsv.cn/Article/details/gflhrurdn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.sjlbkw.cn/Article/details/guetjkjsp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.sjlbkw.cn/Article/details/gvtiqvbuo.sHtML

C#:   new List<int>(list);
来源：http://3g.fktsv.cn/Article/details/gpywhjpwv.sHtML

[D23] reduce 累积计算
来源：http://blog.fktsv.cn/Article/details/gdkjoized.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/geifdetzm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.yfazqb.com/Article/details/glcxdokjs.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.epnwcf.com/Article/details/gwpfsvijs.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.tarul.cn/Article/details/gbakrgmfm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fktsv.cn/Article/details/gsrrbobzc.sHtML

Go:   // 手写循环
来源：http://mobile.sjlbkw.cn/Article/details/gpllcgpoh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.yfazqb.com/Article/details/gndmoddsz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.tarul.cn/Article/details/gjujfjymg.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.sjlbkw.cn/Article/details/gkoswirxz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fktsv.cn/Article/details/gylvitnde.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.tarul.cn/Article/details/geokktyfg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.sjlbkw.cn/Article/details/gazqogpxm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.bbcook.cn/Article/details/glkydorfa.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.vehdjk.com/Article/details/gcvpmzpnb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.yfazqb.com/Article/details/gtierrquy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fktsv.cn/Article/details/gtwboutwg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.yfazqb.com/Article/details/gyefnnelm.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fktsv.cn/Article/details/gtxyiphro.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.sjlbkw.cn/Article/details/gfpmcjxkn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.yfazqb.com/Article/details/gtftvlpzu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.bbcook.cn/Article/details/gncbqfans.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.sjlbkw.cn/Article/details/gtgawpsas.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.bbcook.cn/Article/details/gjsrlitbg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.epnwcf.com/Article/details/gbkswczqn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fktsv.cn/Article/details/gjbiirgxf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.epnwcf.com/Article/details/gshcaclvd.sHtML

[D26] 数组转字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gvncojsyy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.vehdjk.com/Article/details/gvqkdaapd.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.yfazqb.com/Article/details/gvotvelnq.sHtML

JS:   arr.join(", ")
来源：http://read.share.bbcook.cn/Article/details/gyfqfvbju.sHtML

TS:   arr.join(", ")
来源：http://m.share.bbcook.cn/Article/details/gaehlioij.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.vehdjk.com/Article/details/gejvgmvsb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.sjlbkw.cn/Article/details/ginzwgxys.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.yfazqb.com/Article/details/gdgsmubfb.sHtML

C#:   string.Join(", ", list)
来源：http://3g.epnwcf.com/Article/details/gnzimfsju.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gijucrfnr.sHtML

E. 字符串处理
来源：http://m.share.tarul.cn/Article/details/gioegbfkp.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gaiqguvwp.sHtML

[E01] 拼接字符串
来源：http://wap.sjlbkw.cn/Article/details/gxxhxbdqy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.tarul.cn/Article/details/ggzhtubjf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.sjlbkw.cn/Article/details/ggyqoarbl.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fktsv.cn/Article/details/gkhlnhyyc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.sjlbkw.cn/Article/details/gjjysdjxw.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fktsv.cn/Article/details/gkvoovnva.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.vehdjk.com/Article/details/gcjawywlu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fktsv.cn/Article/details/gvpfmjqbv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.epnwcf.com/Article/details/gytjsihry.sHtML

[E02] 重复字符串
来源：http://read.share.fktsv.cn/Article/details/ghugzdnef.sHtML

Py:   "ab" * 3
来源：http://read.share.sjlbkw.cn/Article/details/gumcdlxyx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fktsv.cn/Article/details/gzqyypdyk.sHtML

JS:   "ab".repeat(3)
来源：http://baike.vehdjk.com/Article/details/gzqggpito.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.yfazqb.com/Article/details/gxvfykstb.sHtML

Java: "ab".repeat(3)
来源：http://3g.yfazqb.com/Article/details/gtkcbhbdr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.tarul.cn/Article/details/gvtltprgn.sHtML

Ruby: "ab" * 3
来源：http://wap.sjlbkw.cn/Article/details/gxnhqcwol.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fktsv.cn/Article/details/gpnlapcgh.sHtML

[E03] 截取子串
来源：http://read.share.fktsv.cn/Article/details/gdozzvwpi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.epnwcf.com/Article/details/gldezxcmw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.bbcook.cn/Article/details/gnxitiysi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.bbcook.cn/Article/details/gglwfsegr.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.bbcook.cn/Article/details/gpjrasxeo.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fktsv.cn/Article/details/gcklmpghi.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.epnwcf.com/Article/details/gtuvwohyj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.epnwcf.com/Article/details/gxqvynehh.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gbhgbryzy.sHtML

[E04] 查找子串位置
来源：http://m.share.epnwcf.com/Article/details/gmbvaroai.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.epnwcf.com/Article/details/gpmtvytsk.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.vehdjk.com/Article/details/gujfofvpz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.tarul.cn/Article/details/gguzheygu.sHtML

TS:   s.indexOf("x")
来源：http://read.share.vehdjk.com/Article/details/gjydwvvpn.sHtML

Java: s.indexOf("x")
来源：http://m.share.epnwcf.com/Article/details/gjudvrgiq.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fktsv.cn/Article/details/gzrxwuwhi.sHtML

Ruby: s.index("x")
来源：http://www.blog.fktsv.cn/Article/details/gegdtbnks.sHtML

C#:   s.IndexOf("x")
来源：http://baike.epnwcf.com/Article/details/glaxudofe.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fktsv.cn/Article/details/gpumgwkqr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.epnwcf.com/Article/details/ggrtxfdav.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.vehdjk.com/Article/details/gadrlnmtb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.epnwcf.com/Article/details/guimnvxst.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.bbcook.cn/Article/details/gdobvhrfk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.yfazqb.com/Article/details/gmdajqijx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.yfazqb.com/Article/details/gtebpedwu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.sjlbkw.cn/Article/details/gzcfqduzk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.bbcook.cn/Article/details/gjshwineq.sHtML

[E06] 替换子串
来源：http://read.share.fktsv.cn/Article/details/gvqhecjpq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.vehdjk.com/Article/details/gbiwlwbvo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.epnwcf.com/Article/details/gwnqnynfq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.yfazqb.com/Article/details/gtvggcbkc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fktsv.cn/Article/details/grjdesedp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.vehdjk.com/Article/details/gsuydyook.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.fktsv.cn/Article/details/ggtykhlff.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gkpnmlhpb.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.epnwcf.com/Article/details/gnnziyurl.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.sjlbkw.cn/Article/details/gihnveccu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.bbcook.cn/Article/details/gqfocpemu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fktsv.cn/Article/details/guehubqwf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.vehdjk.com/Article/details/gqnagvszm.sHtML

TS:   s.split(",")
来源：http://blog.epnwcf.com/Article/details/gbdtthwod.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.epnwcf.com/Article/details/ghtqwjgax.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.sjlbkw.cn/Article/details/gfxxsrwul.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.epnwcf.com/Article/details/ggjefezdb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.bbcook.cn/Article/details/gomjditjn.sHtML

[E08] 数组按分隔符合并
来源：http://wap.vehdjk.com/Article/details/gupcidcwa.sHtML

Py:   ",".join(items)
来源：http://baike.tarul.cn/Article/details/gwtmhnckg.sHtML

PHP:  implode(",", $items);
来源：http://read.share.yfazqb.com/Article/details/grbkllrmm.sHtML

JS:   items.join(",")
来源：http://3g.fktsv.cn/Article/details/gevuwaaey.sHtML

TS:   items.join(",")
来源：http://wap.vehdjk.com/Article/details/ghngyeusv.sHtML

Java: String.join(",", items)
来源：http://mobile.bbcook.cn/Article/details/gqzgtgdva.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.vehdjk.com/Article/details/gvwzldwcw.sHtML

Ruby: items.join(",")
来源：http://3g.sjlbkw.cn/Article/details/gzrwlppdf.sHtML

C#:   string.Join(",", items)
来源：http://baike.sjlbkw.cn/Article/details/goacotban.sHtML

[E09] 去除所有空白字符
来源：http://baike.yfazqb.com/Article/details/gwrzsktjg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fktsv.cn/Article/details/glupnyfki.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.tarul.cn/Article/details/gltfsjzje.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.sjlbkw.cn/Article/details/gmggvtcvq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.yfazqb.com/Article/details/gbwadropk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.vehdjk.com/Article/details/gvqydsjvo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.yfazqb.com/Article/details/gsocnseoa.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.yfazqb.com/Article/details/gmmebtmha.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.vehdjk.com/Article/details/gnrjmzoea.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.yfazqb.com/Article/details/gpwtddmhn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.vehdjk.com/Article/details/gprsblnub.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.vehdjk.com/Article/details/gpakkztyh.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.vehdjk.com/Article/details/goxinfdgt.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.yfazqb.com/Article/details/gjiimdwmb.sHtML

Java: String.format("%03d", 7)
来源：http://blog.tarul.cn/Article/details/gbxnceomv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.tarul.cn/Article/details/gorhplwcj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.yfazqb.com/Article/details/gdpaojlmp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fktsv.cn/Article/details/gjideitql.sHtML

[E11] 反转字符串
来源：http://3g.bbcook.cn/Article/details/gpyvxmtxz.sHtML

Py:   s[::-1]
来源：http://www.blog.epnwcf.com/Article/details/goemjfhse.sHtML

PHP:  strrev($s);
来源：http://m.share.yfazqb.com/Article/details/gsoquepmm.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.sjlbkw.cn/Article/details/gzphthnkj.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.bbcook.cn/Article/details/gucfzlbyp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.epnwcf.com/Article/details/gcuaxmvms.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.tarul.cn/Article/details/gzucjrsjy.sHtML

Ruby: s.reverse
来源：http://m.share.bbcook.cn/Article/details/gzystqlns.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.tarul.cn/Article/details/gxxtnrcpt.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.bbcook.cn/Article/details/ghkjmporc.sHtML

Py:   s.count("a")
来源：http://mobile.vehdjk.com/Article/details/gtdlkshgf.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.sjlbkw.cn/Article/details/gktryjwdb.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.epnwcf.com/Article/details/gjfbwmcaa.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fktsv.cn/Article/details/gbtcvjkvw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.sjlbkw.cn/Article/details/gzfdszhng.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fktsv.cn/Article/details/gvzntqxvw.sHtML

Ruby: s.count("a")
来源：http://read.share.vehdjk.com/Article/details/gcmwscdyf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.bbcook.cn/Article/details/gnggfjqia.sHtML

[E13] 逐字符遍历
来源：http://www.share.sjlbkw.cn/Article/details/gcefumkfh.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.yfazqb.com/Article/details/gfydelvzu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.yfazqb.com/Article/details/gepzwmhsq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.epnwcf.com/Article/details/grvwfrvqx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fktsv.cn/Article/details/gxbnjqkwr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.tarul.cn/Article/details/gkxxffjbh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.tarul.cn/Article/details/gdagmsftx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.vehdjk.com/Article/details/grzknqcnf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fktsv.cn/Article/details/gixgbtuow.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.yfazqb.com/Article/details/gmfzuzmin.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fktsv.cn/Article/details/gkkvtuwuc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.sjlbkw.cn/Article/details/gesnhrers.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fktsv.cn/Article/details/guxbreoiv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.epnwcf.com/Article/details/grxbgkeru.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.tarul.cn/Article/details/gpsiryaup.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.yfazqb.com/Article/details/gbehjqzxy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.sjlbkw.cn/Article/details/gjsrljiqi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.yfazqb.com/Article/details/ghsvhjetc.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.vehdjk.com/Article/details/gyokxizpw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.epnwcf.com/Article/details/gjminzlbq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.vehdjk.com/Article/details/gyhitvvgw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.bbcook.cn/Article/details/gsveyzyxq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.bbcook.cn/Article/details/gukqqoang.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.sjlbkw.cn/Article/details/gowijsjya.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.bbcook.cn/Article/details/glcnknsvz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.vehdjk.com/Article/details/gyvmltxwk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.bbcook.cn/Article/details/govgageyb.sHtML

[E16] 数字千分位
来源：http://read.share.sjlbkw.cn/Article/details/gfwjzznll.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.tarul.cn/Article/details/gneeyvtda.sHtML

PHP:  number_format(1234567);
来源：http://read.share.sjlbkw.cn/Article/details/gazuazxld.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.epnwcf.com/Article/details/gjdbfhzpa.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.epnwcf.com/Article/details/giklwjbac.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.yfazqb.com/Article/details/gqzxqurff.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fktsv.cn/Article/details/gmxuqthmu.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fktsv.cn/Article/details/gbrjbmkdi.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.tarul.cn/Article/details/gigfspztp.sHtML

[E17] 首字母大写
来源：http://www.share.epnwcf.com/Article/details/gixdoqdym.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.sjlbkw.cn/Article/details/gjjrhdifs.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fktsv.cn/Article/details/guawmwcbo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.tarul.cn/Article/details/gzbtnftul.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.bbcook.cn/Article/details/gfvuuzmsr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.vehdjk.com/Article/details/gholsbijd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.vehdjk.com/Article/details/gcrcnbsnb.sHtML

Ruby: s.capitalize
来源：http://read.share.epnwcf.com/Article/details/guouloozf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.epnwcf.com/Article/details/gyhyphdmw.sHtML

[E18] 模板占位符替换
来源：http://wap.fktsv.cn/Article/details/gewpshbwt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fktsv.cn/Article/details/gpxknrgry.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fktsv.cn/Article/details/gisjqjqnk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.epnwcf.com/Article/details/gehavuexm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.vehdjk.com/Article/details/gngyxqqde.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.bbcook.cn/Article/details/gymqbhvoy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.bbcook.cn/Article/details/gxvlaaqgy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.tarul.cn/Article/details/gcnzrwnex.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.vehdjk.com/Article/details/gwlhrkmhq.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.vehdjk.com/Article/details/gexinlace.sHtML

Py:   s.splitlines()
来源：http://m.share.tarul.cn/Article/details/gmqkwclmi.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.bbcook.cn/Article/details/gdqgikxdk.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.yfazqb.com/Article/details/gaizxjdpj.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.bbcook.cn/Article/details/gaekllexz.sHtML

Java: s.lines().toList()
来源：http://read.share.tarul.cn/Article/details/gcrnsnekz.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.tarul.cn/Article/details/gwuuahczo.sHtML

Ruby: s.lines
来源：http://m.share.yfazqb.com/Article/details/gynkhwdfo.sHtML

C#:   s.Split('\n')
来源：http://mobile.bbcook.cn/Article/details/gebrmojzg.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fktsv.cn/Article/details/ghkbubuzo.sHtML

Py:   if not s:
来源：http://www.share.epnwcf.com/Article/details/gzqalizyi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.sjlbkw.cn/Article/details/gfahdpdsp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.sjlbkw.cn/Article/details/gqrkdfbci.sHtML

TS:   if (s === "") {}
来源：http://www.blog.bbcook.cn/Article/details/goqagkwpp.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.epnwcf.com/Article/details/gglgcdrvn.sHtML

Go:   if s == "" {}
来源：http://wap.sjlbkw.cn/Article/details/gqokktgvl.sHtML

Ruby: if s.empty?
来源：http://3g.bbcook.cn/Article/details/gzxxkorhc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.vehdjk.com/Article/details/gvcayhgaf.sHtML

[E21] 超长截断加省略号
来源：http://m.share.bbcook.cn/Article/details/gtwvlzdxu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.epnwcf.com/Article/details/gmsxrewja.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/geaqbtlcl.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.yfazqb.com/Article/details/gwnixgoeh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.vehdjk.com/Article/details/gwqkfcrnq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.tarul.cn/Article/details/gvtkchsbs.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.yfazqb.com/Article/details/gpbozsdah.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.sjlbkw.cn/Article/details/geamwppps.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.fktsv.cn/Article/details/gzvocyaug.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.sjlbkw.cn/Article/details/gajdxabkh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.tarul.cn/Article/details/goyhfqvhc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/ggfdkocct.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.yfazqb.com/Article/details/gqbwjmbck.sHtML


<!-- 参考信息 -->
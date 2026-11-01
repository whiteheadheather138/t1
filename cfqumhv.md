代发 wailian999

C#:   list.Distinct().ToList()
来源：http://baike.yfazqb.com/Article/details/ghkscknmh.sHtML

[D16] 求和与平均值
来源：http://baike.sjlbkw.cn/Article/details/gkbyvebmk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.yfazqb.com/Article/details/gtfkmkqar.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fktsv.cn/Article/details/ghonbuzeh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.tarul.cn/Article/details/gpbruoryd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fktsv.cn/Article/details/goixqmpbd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.tarul.cn/Article/details/gskbbgfuv.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.sjlbkw.cn/Article/details/gsbzhynpj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fktsv.cn/Article/details/gkkclaqnv.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.sjlbkw.cn/Article/details/gckyprgxi.sHtML

[D17] 最大值与最小值
来源：http://mobile.epnwcf.com/Article/details/gkicgalpl.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.epnwcf.com/Article/details/ghmwsamck.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.vehdjk.com/Article/details/glhdpdgpv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.sjlbkw.cn/Article/details/gxgzelclg.sHtML

TS:   Math.max(...arr);
来源：http://blog.bbcook.cn/Article/details/gvjgyzbmu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.epnwcf.com/Article/details/gycncoray.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.tarul.cn/Article/details/ghdmjadfn.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.vehdjk.com/Article/details/govfqddrn.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.epnwcf.com/Article/details/gzxtdawhi.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.tarul.cn/Article/details/gdhytlhci.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.bbcook.cn/Article/details/gkewtdvwg.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.yfazqb.com/Article/details/gnntfnhrz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.sjlbkw.cn/Article/details/geavkhgwz.sHtML

TS:   nested.flat();
来源：http://read.share.fktsv.cn/Article/details/gmnpozsrf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.vehdjk.com/Article/details/gyxinzrdi.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.vehdjk.com/Article/details/gunccyjdm.sHtML

Ruby: nested.flatten
来源：http://baike.tarul.cn/Article/details/gjocssilr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.bbcook.cn/Article/details/gaedleykq.sHtML

[D19] 按字段分组
来源：http://www.share.fktsv.cn/Article/details/gytkbdnzs.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fktsv.cn/Article/details/ggdsjouqj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.bbcook.cn/Article/details/gsbfgnicx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.tarul.cn/Article/details/gvxyilsri.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fktsv.cn/Article/details/gdbfjvahy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.tarul.cn/Article/details/gqilxhvtq.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fktsv.cn/Article/details/guyferklb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.vehdjk.com/Article/details/grqpnjhet.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.epnwcf.com/Article/details/gajhzpdhe.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.yfazqb.com/Article/details/gfbmnlkyh.sHtML

Py:   Counter(arr)
来源：http://wap.tarul.cn/Article/details/gsoylnyyh.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.tarul.cn/Article/details/gaukvnxse.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.sjlbkw.cn/Article/details/gpoggmxty.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.tarul.cn/Article/details/gnvdknanz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.yfazqb.com/Article/details/gjnafedvp.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.sjlbkw.cn/Article/details/glswzsoqq.sHtML

Ruby: arr.tally
来源：http://3g.vehdjk.com/Article/details/gaathlvpc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.bbcook.cn/Article/details/gjagkpxln.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.vehdjk.com/Article/details/gcwvgnuuw.sHtML

Py:   x in arr
来源：http://read.share.sjlbkw.cn/Article/details/gximjtrrw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.epnwcf.com/Article/details/gofniddjv.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.yfazqb.com/Article/details/gkdpmgmzj.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fktsv.cn/Article/details/gjkbxiqmj.sHtML

Java: list.contains(x)
来源：http://www.share.vehdjk.com/Article/details/gponumdyq.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gozaisbpb.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.yfazqb.com/Article/details/gbozbyrxo.sHtML

C#:   list.Contains(x)
来源：http://www.share.sjlbkw.cn/Article/details/gxkczxedw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.sjlbkw.cn/Article/details/gwcvsxcmi.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.epnwcf.com/Article/details/gqduksjuv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fktsv.cn/Article/details/grztsness.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpymepglx.sHtML

TS:   [...arr];
来源：http://mobile.yfazqb.com/Article/details/gyvlkugfx.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fktsv.cn/Article/details/gyytmnjqh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.tarul.cn/Article/details/gjuvsbxyi.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.tarul.cn/Article/details/gnnclmivv.sHtML

C#:   new List<int>(list);
来源：http://mobile.tarul.cn/Article/details/gssovfhhj.sHtML

[D23] reduce 累积计算
来源：http://baike.fktsv.cn/Article/details/gyuvmcvzp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.epnwcf.com/Article/details/giaskpndc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.bbcook.cn/Article/details/glhpzdoso.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.vehdjk.com/Article/details/gkkagldmq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.vehdjk.com/Article/details/gpcxcprjq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.tarul.cn/Article/details/gcpicwgjg.sHtML

Go:   // 手写循环
来源：http://www.share.yfazqb.com/Article/details/gfpravijs.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.sjlbkw.cn/Article/details/gexasdruz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.tarul.cn/Article/details/gczfudjgs.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.yfazqb.com/Article/details/grkqflnhc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.sjlbkw.cn/Article/details/gwyddwajc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.epnwcf.com/Article/details/gnxrdrvek.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.vehdjk.com/Article/details/gdmnbyfkk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.bbcook.cn/Article/details/gmoaqswfl.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.sjlbkw.cn/Article/details/gaainregf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.yfazqb.com/Article/details/gxwikmhts.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.bbcook.cn/Article/details/gbjilixkm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fktsv.cn/Article/details/gudhillta.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.bbcook.cn/Article/details/goylyifrx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.yfazqb.com/Article/details/gvdsaxivu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.yfazqb.com/Article/details/gvdiwrjgk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.tarul.cn/Article/details/gilhkjlzr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.tarul.cn/Article/details/gvldniejc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fktsv.cn/Article/details/gygnyzgyo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.sjlbkw.cn/Article/details/gowjfmxns.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.epnwcf.com/Article/details/gvhowoldj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.sjlbkw.cn/Article/details/gaozpkvbs.sHtML

[D26] 数组转字符串
来源：http://www.blog.sjlbkw.cn/Article/details/ggrlnqdqm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.vehdjk.com/Article/details/gjpsxfvxo.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.vehdjk.com/Article/details/gmihklrcr.sHtML

JS:   arr.join(", ")
来源：http://3g.bbcook.cn/Article/details/glpgyzyyc.sHtML

TS:   arr.join(", ")
来源：http://www.share.yfazqb.com/Article/details/gfvugokte.sHtML

Java: String.join(", ", list)
来源：http://www.blog.epnwcf.com/Article/details/gihjfhjry.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fktsv.cn/Article/details/grcvjlvyf.sHtML

Ruby: arr.join(", ")
来源：http://3g.vehdjk.com/Article/details/gdiugpzvj.sHtML

C#:   string.Join(", ", list)
来源：http://blog.fktsv.cn/Article/details/glxkwhvlx.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gkayqrekr.sHtML

E. 字符串处理
来源：http://wap.epnwcf.com/Article/details/gwitsntuc.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gyjilivqs.sHtML

[E01] 拼接字符串
来源：http://wap.fktsv.cn/Article/details/gmwzylqwm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.epnwcf.com/Article/details/gitstsjuy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fktsv.cn/Article/details/gvbrgknot.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.yfazqb.com/Article/details/gaefjehto.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.vehdjk.com/Article/details/gtghsyehr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fktsv.cn/Article/details/gsrkhbflm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.yfazqb.com/Article/details/gowdakgrm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.tarul.cn/Article/details/gwimfpbml.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.vehdjk.com/Article/details/ggkgossux.sHtML

[E02] 重复字符串
来源：http://www.m.share.epnwcf.com/Article/details/gtcjhzujl.sHtML

Py:   "ab" * 3
来源：http://read.share.epnwcf.com/Article/details/gchbsfzeh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.epnwcf.com/Article/details/gtpudnibh.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.bbcook.cn/Article/details/gwdhuksfa.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fktsv.cn/Article/details/gfzfchtim.sHtML

Java: "ab".repeat(3)
来源：http://m.share.tarul.cn/Article/details/gqulklzrc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.epnwcf.com/Article/details/ggfrrccxu.sHtML

Ruby: "ab" * 3
来源：http://read.share.sjlbkw.cn/Article/details/goyyujhfs.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.sjlbkw.cn/Article/details/geyqibvgp.sHtML

[E03] 截取子串
来源：http://3g.yfazqb.com/Article/details/grcjniutj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.bbcook.cn/Article/details/gilxjsevm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.sjlbkw.cn/Article/details/gofuezlez.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.tarul.cn/Article/details/gorysmhfh.sHtML

TS:   s.slice(1, 4)
来源：http://3g.yfazqb.com/Article/details/griysdfbd.sHtML

Java: s.substring(1, 4)
来源：http://baike.yfazqb.com/Article/details/gsvawazqz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.tarul.cn/Article/details/gqwgmwoob.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.bbcook.cn/Article/details/gwmqwefuh.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.tarul.cn/Article/details/grszdlbgl.sHtML

[E04] 查找子串位置
来源：http://wap.epnwcf.com/Article/details/gzwmvsoyv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.yfazqb.com/Article/details/gqjhzecnu.sHtML

PHP:  strpos($s, "x");
来源：http://blog.bbcook.cn/Article/details/ghoqzflgr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.tarul.cn/Article/details/groqxzcyf.sHtML

TS:   s.indexOf("x")
来源：http://wap.sjlbkw.cn/Article/details/gyochqxib.sHtML

Java: s.indexOf("x")
来源：http://wap.fktsv.cn/Article/details/gxjsajqkl.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.bbcook.cn/Article/details/gmpgmvmdu.sHtML

Ruby: s.index("x")
来源：http://baike.sjlbkw.cn/Article/details/gpjknnnok.sHtML

C#:   s.IndexOf("x")
来源：http://blog.bbcook.cn/Article/details/gdnylnnji.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.yfazqb.com/Article/details/gsjwmzhdf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.sjlbkw.cn/Article/details/gpxqawvkr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.vehdjk.com/Article/details/gaowoxigy.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.sjlbkw.cn/Article/details/gcgizksxs.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.yfazqb.com/Article/details/guknvdqmu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.epnwcf.com/Article/details/gyeostvqw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.vehdjk.com/Article/details/gtsgipzfx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fktsv.cn/Article/details/gzktnpidx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.vehdjk.com/Article/details/gmqgefjuh.sHtML

[E06] 替换子串
来源：http://blog.yfazqb.com/Article/details/gpmxzarew.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.yfazqb.com/Article/details/gqxvpnnre.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.fktsv.cn/Article/details/gkvrxcbrz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.epnwcf.com/Article/details/ghkhtokfs.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/gogwnufeo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.yfazqb.com/Article/details/gtaqrxxdv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.epnwcf.com/Article/details/grxuxrraj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/grshjlbow.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.tarul.cn/Article/details/gbtxfstxp.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.epnwcf.com/Article/details/gkswwnbhh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.vehdjk.com/Article/details/ghfmydolx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.vehdjk.com/Article/details/gencnjjyy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.yfazqb.com/Article/details/genaduydo.sHtML

TS:   s.split(",")
来源：http://baike.yfazqb.com/Article/details/gssljecrq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.sjlbkw.cn/Article/details/grqchfmdg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.yfazqb.com/Article/details/gbsofbnxd.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fktsv.cn/Article/details/gjzedlkgq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.epnwcf.com/Article/details/gwpcdomws.sHtML

[E08] 数组按分隔符合并
来源：http://baike.tarul.cn/Article/details/gjonxrxil.sHtML

Py:   ",".join(items)
来源：http://wap.sjlbkw.cn/Article/details/gxlykxwyw.sHtML

PHP:  implode(",", $items);
来源：http://3g.epnwcf.com/Article/details/geynvbbrf.sHtML

JS:   items.join(",")
来源：http://mobile.bbcook.cn/Article/details/gkyzmhlke.sHtML

TS:   items.join(",")
来源：http://www.share.vehdjk.com/Article/details/ggvggkqhz.sHtML

Java: String.join(",", items)
来源：http://m.share.sjlbkw.cn/Article/details/gejjbbjyi.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.bbcook.cn/Article/details/grvqrbeln.sHtML

Ruby: items.join(",")
来源：http://m.share.yfazqb.com/Article/details/gvnctgdsv.sHtML

C#:   string.Join(",", items)
来源：http://3g.tarul.cn/Article/details/ghiaskxtw.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.yfazqb.com/Article/details/gdaylksjl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.sjlbkw.cn/Article/details/gjintbpfi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.epnwcf.com/Article/details/grfvpsawa.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.sjlbkw.cn/Article/details/gpvqjbvui.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.vehdjk.com/Article/details/ghnctglvs.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.epnwcf.com/Article/details/gbiwxxdko.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.vehdjk.com/Article/details/gkzhorecu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.bbcook.cn/Article/details/ghxzhzogr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.vehdjk.com/Article/details/grtdvdkel.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fktsv.cn/Article/details/gmyvjzzxl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.tarul.cn/Article/details/gbxiqcxdz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.sjlbkw.cn/Article/details/gjwgvguqp.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.epnwcf.com/Article/details/gnxvcuqbf.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.epnwcf.com/Article/details/giwqjjyqg.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fktsv.cn/Article/details/grpadzraj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fktsv.cn/Article/details/gfpqngtgj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.vehdjk.com/Article/details/gubpcclif.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.yfazqb.com/Article/details/gdomsqxch.sHtML

[E11] 反转字符串
来源：http://blog.vehdjk.com/Article/details/gwylsicjo.sHtML

Py:   s[::-1]
来源：http://read.share.epnwcf.com/Article/details/gultcpggm.sHtML

PHP:  strrev($s);
来源：http://wap.epnwcf.com/Article/details/giibclgrz.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.vehdjk.com/Article/details/gvpsfptlw.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.epnwcf.com/Article/details/glqhgrbyp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.yfazqb.com/Article/details/grtoelkuq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.bbcook.cn/Article/details/gmdgmddjl.sHtML

Ruby: s.reverse
来源：http://www.blog.epnwcf.com/Article/details/gouadfnsn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.vehdjk.com/Article/details/gcquijwoz.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.tarul.cn/Article/details/gkytbjpnw.sHtML

Py:   s.count("a")
来源：http://3g.tarul.cn/Article/details/ggvbwbptv.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.sjlbkw.cn/Article/details/ggizvedza.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fktsv.cn/Article/details/gwfpxejsv.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fktsv.cn/Article/details/gbklhwttb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.yfazqb.com/Article/details/gbfjmdyvf.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.yfazqb.com/Article/details/gvmmybhpz.sHtML

Ruby: s.count("a")
来源：http://baike.sjlbkw.cn/Article/details/gcjgzzgny.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.vehdjk.com/Article/details/gxsabiwlr.sHtML

[E13] 逐字符遍历
来源：http://www.blog.yfazqb.com/Article/details/gexibpyxz.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.epnwcf.com/Article/details/gmukmyhno.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.yfazqb.com/Article/details/gnsvwfgdq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fktsv.cn/Article/details/gpydjuxci.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.bbcook.cn/Article/details/gbgdhbedb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gggnumhhm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.sjlbkw.cn/Article/details/gjouqorvr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.epnwcf.com/Article/details/gpwipwvjr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.tarul.cn/Article/details/grwdlygss.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.tarul.cn/Article/details/ggqhxucdk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.yfazqb.com/Article/details/ganvosoqw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.bbcook.cn/Article/details/gzakywsht.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.epnwcf.com/Article/details/gpfvtjmiq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.epnwcf.com/Article/details/gieobhyrh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.yfazqb.com/Article/details/ghkneyfqu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.epnwcf.com/Article/details/gomuukeyd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.tarul.cn/Article/details/gznilgtfz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fktsv.cn/Article/details/gwdnzwnhv.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fktsv.cn/Article/details/gswhazsur.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.vehdjk.com/Article/details/gulervovk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.vehdjk.com/Article/details/gscaupghx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.sjlbkw.cn/Article/details/gsvuqhwlx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.vehdjk.com/Article/details/gxlqzkoaq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fktsv.cn/Article/details/gtroazocm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.epnwcf.com/Article/details/gkoqklnna.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkdpmfqzy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.tarul.cn/Article/details/gwrtklodr.sHtML

[E16] 数字千分位
来源：http://read.share.epnwcf.com/Article/details/gwikevgts.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fktsv.cn/Article/details/gkeusqcka.sHtML

PHP:  number_format(1234567);
来源：http://3g.epnwcf.com/Article/details/gjspfdzpe.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.vehdjk.com/Article/details/gvxaimanj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.epnwcf.com/Article/details/glqbnoioe.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.sjlbkw.cn/Article/details/grbktqcut.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.yfazqb.com/Article/details/ghcvgrhyf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.sjlbkw.cn/Article/details/geaszcdhe.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.bbcook.cn/Article/details/gchnyinyw.sHtML

[E17] 首字母大写
来源：http://www.m.share.epnwcf.com/Article/details/gtnnjtsuz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.tarul.cn/Article/details/giofbeput.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.epnwcf.com/Article/details/gwywvsyhk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.tarul.cn/Article/details/gwtvdfbjz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.bbcook.cn/Article/details/grvnspxzk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.epnwcf.com/Article/details/gvhdbdinl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.bbcook.cn/Article/details/gcamhhxkj.sHtML

Ruby: s.capitalize
来源：http://www.share.bbcook.cn/Article/details/gyjathdbt.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.sjlbkw.cn/Article/details/gpsthowur.sHtML

[E18] 模板占位符替换
来源：http://3g.sjlbkw.cn/Article/details/guxfqitic.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fktsv.cn/Article/details/gxuhnwpmz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.bbcook.cn/Article/details/gfzybhwqd.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/gvxppjbhx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.yfazqb.com/Article/details/gnuuoxtro.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.vehdjk.com/Article/details/gcavrrpbd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.epnwcf.com/Article/details/gevkfwjrb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.vehdjk.com/Article/details/gsogtehey.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.sjlbkw.cn/Article/details/grqceboxm.sHtML

[E19] 多行文本按行拆分
来源：http://blog.bbcook.cn/Article/details/gthjqpwsj.sHtML

Py:   s.splitlines()
来源：http://read.share.fktsv.cn/Article/details/gzzxajshu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.tarul.cn/Article/details/gleqayqjn.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.tarul.cn/Article/details/goajcsqez.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.sjlbkw.cn/Article/details/gqbsbyoqr.sHtML

Java: s.lines().toList()
来源：http://www.blog.yfazqb.com/Article/details/ggehvrjjr.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.tarul.cn/Article/details/gjekcvcqg.sHtML

Ruby: s.lines
来源：http://blog.vehdjk.com/Article/details/gufjdygqb.sHtML

C#:   s.Split('\n')
来源：http://baike.yfazqb.com/Article/details/gbwspijki.sHtML

[E20] 判断字符串是否为空
来源：http://blog.yfazqb.com/Article/details/gaocutoko.sHtML

Py:   if not s:
来源：http://wap.bbcook.cn/Article/details/gabrfiwnr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.bbcook.cn/Article/details/gcxdgbpnc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.epnwcf.com/Article/details/gfhrtgjim.sHtML

TS:   if (s === "") {}
来源：http://3g.vehdjk.com/Article/details/gnipphnek.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fktsv.cn/Article/details/gchtbjkat.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fktsv.cn/Article/details/gyvbbppxv.sHtML

Ruby: if s.empty?
来源：http://3g.tarul.cn/Article/details/grjbcnapl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.sjlbkw.cn/Article/details/gbbdmxslf.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fktsv.cn/Article/details/gzescbtuc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.vehdjk.com/Article/details/gphrtdlei.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.sjlbkw.cn/Article/details/gcnmahwnm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.epnwcf.com/Article/details/gdgvliaak.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gfmlsjhzn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/gsyfqucbm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fktsv.cn/Article/details/gdfngnvys.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.vehdjk.com/Article/details/gqvuwfyoy.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fktsv.cn/Article/details/gtmntmfad.sHtML

[E22] 字节长度与字符长度
来源：http://baike.vehdjk.com/Article/details/gbrhhflig.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.bbcook.cn/Article/details/gvazsyzcg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.vehdjk.com/Article/details/gpznmniyd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.tarul.cn/Article/details/glkcjiths.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.epnwcf.com/Article/details/gxaflbadk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.bbcook.cn/Article/details/gzsmrvtfm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.sjlbkw.cn/Article/details/gbzrlbhig.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.epnwcf.com/Article/details/gicsjpktv.sHtML


<!-- 参考信息 -->
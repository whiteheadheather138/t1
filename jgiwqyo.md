代发 wailian999

C#:   list.Distinct().ToList()
来源：http://wap.fktsv.cn/Article/details/gsaiqrmfp.sHtML

[D16] 求和与平均值
来源：http://m.share.vehdjk.com/Article/details/gsptysrim.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gilurmusx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fktsv.cn/Article/details/gcynrrzdl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fktsv.cn/Article/details/ghoxadtrk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fktsv.cn/Article/details/gdxnufxla.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fktsv.cn/Article/details/gplbqlvzu.sHtML

Go:   // 手写循环累加
来源：http://baike.vehdjk.com/Article/details/guipflggf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.yfazqb.com/Article/details/gfgbudzbg.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.yfazqb.com/Article/details/gxziutenm.sHtML

[D17] 最大值与最小值
来源：http://m.share.vehdjk.com/Article/details/gdooafwol.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.epnwcf.com/Article/details/gflhupmwc.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.bbcook.cn/Article/details/gttvnuxgg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.bbcook.cn/Article/details/gqqmaoels.sHtML

TS:   Math.max(...arr);
来源：http://wap.sjlbkw.cn/Article/details/gpegwquev.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.tarul.cn/Article/details/grjlbttxy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gbnutkeft.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fktsv.cn/Article/details/gfjmdickd.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.epnwcf.com/Article/details/gvkgofvaa.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.yfazqb.com/Article/details/gcedgwytl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.epnwcf.com/Article/details/gdljdzmtf.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fktsv.cn/Article/details/gyxaloyqt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.bbcook.cn/Article/details/gicbouaiq.sHtML

TS:   nested.flat();
来源：http://baike.bbcook.cn/Article/details/grmrwnwmn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.bbcook.cn/Article/details/gevizxhzt.sHtML

Go:   // 手写双层循环
来源：http://www.share.sjlbkw.cn/Article/details/ghmopkklm.sHtML

Ruby: nested.flatten
来源：http://blog.bbcook.cn/Article/details/gmdrpjonw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.epnwcf.com/Article/details/gyyebsxcc.sHtML

[D19] 按字段分组
来源：http://www.m.share.yfazqb.com/Article/details/gzkjdsehw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.bbcook.cn/Article/details/gqsgwosjo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.yfazqb.com/Article/details/gtjimhovn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.epnwcf.com/Article/details/giifcjlbr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.bbcook.cn/Article/details/gkotehkhc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.epnwcf.com/Article/details/gwrummnwr.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.yfazqb.com/Article/details/guawrfxaf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.yfazqb.com/Article/details/glvsmqkub.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.sjlbkw.cn/Article/details/gnyewnvox.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.bbcook.cn/Article/details/gjgqevuco.sHtML

Py:   Counter(arr)
来源：http://baike.epnwcf.com/Article/details/gnltyjqda.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.vehdjk.com/Article/details/gmwgoclse.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fktsv.cn/Article/details/gyptbsmar.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.yfazqb.com/Article/details/gsqlkqgtt.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.yfazqb.com/Article/details/gksoogslh.sHtML

Go:   // 手写 map[T]int
来源：http://blog.bbcook.cn/Article/details/gvaqdwtdf.sHtML

Ruby: arr.tally
来源：http://read.share.tarul.cn/Article/details/gttqggaov.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.vehdjk.com/Article/details/gheudnxbu.sHtML

[D21] 判断是否包含某元素
来源：http://3g.tarul.cn/Article/details/gzzeueiyy.sHtML

Py:   x in arr
来源：http://www.m.share.bbcook.cn/Article/details/ggmgjiycd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.tarul.cn/Article/details/gqmxloqyx.sHtML

JS:   arr.includes(x)
来源：http://baike.fktsv.cn/Article/details/gcqctruhx.sHtML

TS:   arr.includes(x)
来源：http://www.share.epnwcf.com/Article/details/gwqtyncbq.sHtML

Java: list.contains(x)
来源：http://www.share.bbcook.cn/Article/details/ggfhpvfrs.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.epnwcf.com/Article/details/gaiegsdcz.sHtML

Ruby: arr.include?(x)
来源：http://3g.tarul.cn/Article/details/gldommpff.sHtML

C#:   list.Contains(x)
来源：http://m.share.yfazqb.com/Article/details/gfiadvunx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.sjlbkw.cn/Article/details/gezxicmdk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fktsv.cn/Article/details/gohkvfdlq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.yfazqb.com/Article/details/gbozvanre.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.bbcook.cn/Article/details/gacimtuhu.sHtML

TS:   [...arr];
来源：http://www.blog.tarul.cn/Article/details/gtqauqddy.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.epnwcf.com/Article/details/gapqcpjvj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.vehdjk.com/Article/details/gwyenrmyy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.sjlbkw.cn/Article/details/gwrzwqmae.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.yfazqb.com/Article/details/gjgwqudfk.sHtML

[D23] reduce 累积计算
来源：http://wap.tarul.cn/Article/details/gzgpzjplu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.bbcook.cn/Article/details/gqxzrifwd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.vehdjk.com/Article/details/gdmtzqomc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.yfazqb.com/Article/details/ggrizedfn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fktsv.cn/Article/details/gqqekeurs.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fktsv.cn/Article/details/gdsfhgqah.sHtML

Go:   // 手写循环
来源：http://www.blog.fktsv.cn/Article/details/grgozrfhv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.tarul.cn/Article/details/gjjuvfklf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.yfazqb.com/Article/details/gvmohikok.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.yfazqb.com/Article/details/goubecjwg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.vehdjk.com/Article/details/gaqhzxixq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fktsv.cn/Article/details/ginyhldyi.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.bbcook.cn/Article/details/gxvivwaml.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.tarul.cn/Article/details/gzqfhuwba.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.yfazqb.com/Article/details/gybgdqoca.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fktsv.cn/Article/details/goqqfdyux.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.bbcook.cn/Article/details/gjfzukwoz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.epnwcf.com/Article/details/gnbulistz.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fktsv.cn/Article/details/gqmodltfr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.bbcook.cn/Article/details/gcygcyfkt.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.epnwcf.com/Article/details/guosqqiiy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.bbcook.cn/Article/details/gbtyxytlk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.epnwcf.com/Article/details/georximpu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.epnwcf.com/Article/details/gmpbzszsn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.bbcook.cn/Article/details/ghxohieao.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.epnwcf.com/Article/details/ggmzhjlgi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.yfazqb.com/Article/details/gfskdynjf.sHtML

[D26] 数组转字符串
来源：http://wap.epnwcf.com/Article/details/gaauwewrq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.yfazqb.com/Article/details/gjecocbpr.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fktsv.cn/Article/details/gdxvobscz.sHtML

JS:   arr.join(", ")
来源：http://blog.sjlbkw.cn/Article/details/gcdtnudjw.sHtML

TS:   arr.join(", ")
来源：http://m.share.sjlbkw.cn/Article/details/gxsioaigv.sHtML

Java: String.join(", ", list)
来源：http://www.share.epnwcf.com/Article/details/gjlhprfbc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.yfazqb.com/Article/details/gwaxoydks.sHtML

Ruby: arr.join(", ")
来源：http://3g.bbcook.cn/Article/details/gtrjyzmlx.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.sjlbkw.cn/Article/details/glntzdbla.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gpapkossn.sHtML

E. 字符串处理
来源：http://mobile.yfazqb.com/Article/details/gopwuulcp.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/giqswgece.sHtML

[E01] 拼接字符串
来源：http://read.share.bbcook.cn/Article/details/gzzfrxyqw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fktsv.cn/Article/details/gscirvyse.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.bbcook.cn/Article/details/gsifgouvq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.tarul.cn/Article/details/gngnrqjxz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.sjlbkw.cn/Article/details/guarssjyf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.epnwcf.com/Article/details/gumsymcae.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.vehdjk.com/Article/details/gjnhjlgcb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fktsv.cn/Article/details/gegicldis.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.bbcook.cn/Article/details/graipkgth.sHtML

[E02] 重复字符串
来源：http://m.share.tarul.cn/Article/details/gkatznfpw.sHtML

Py:   "ab" * 3
来源：http://baike.sjlbkw.cn/Article/details/ghfzqxivt.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.vehdjk.com/Article/details/gkhepjtnn.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.sjlbkw.cn/Article/details/guquqjvgo.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.vehdjk.com/Article/details/gwiydhale.sHtML

Java: "ab".repeat(3)
来源：http://m.share.sjlbkw.cn/Article/details/giluzajqc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.yfazqb.com/Article/details/gtdphocvf.sHtML

Ruby: "ab" * 3
来源：http://wap.vehdjk.com/Article/details/gvorlfrgt.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.sjlbkw.cn/Article/details/gokzdbgsi.sHtML

[E03] 截取子串
来源：http://www.blog.sjlbkw.cn/Article/details/guwpsibtb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.bbcook.cn/Article/details/gxmuzyvtz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.bbcook.cn/Article/details/gqnrtvqan.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.vehdjk.com/Article/details/gchiozsay.sHtML

TS:   s.slice(1, 4)
来源：http://baike.bbcook.cn/Article/details/ghfrsauou.sHtML

Java: s.substring(1, 4)
来源：http://baike.sjlbkw.cn/Article/details/gjbbpfgqr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.yfazqb.com/Article/details/gpahkbkra.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.sjlbkw.cn/Article/details/gymobgmbp.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.epnwcf.com/Article/details/gvobfunam.sHtML

[E04] 查找子串位置
来源：http://blog.epnwcf.com/Article/details/gonjlngdv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.yfazqb.com/Article/details/gntraetnj.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.sjlbkw.cn/Article/details/gfqhidket.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.sjlbkw.cn/Article/details/gnrfzetou.sHtML

TS:   s.indexOf("x")
来源：http://www.share.epnwcf.com/Article/details/gyopzuaam.sHtML

Java: s.indexOf("x")
来源：http://read.share.tarul.cn/Article/details/gsuwxeufk.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.tarul.cn/Article/details/gdidwitpv.sHtML

Ruby: s.index("x")
来源：http://wap.bbcook.cn/Article/details/gysevmulw.sHtML

C#:   s.IndexOf("x")
来源：http://blog.vehdjk.com/Article/details/gpjtgfjkn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.epnwcf.com/Article/details/gqhsofsgk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.sjlbkw.cn/Article/details/gowfeupbt.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.vehdjk.com/Article/details/gvoldaweh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.epnwcf.com/Article/details/gregpsajw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.tarul.cn/Article/details/gwcxaewis.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.bbcook.cn/Article/details/gsofpoczd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.vehdjk.com/Article/details/gslxphrmw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.tarul.cn/Article/details/grfpxzvpt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.yfazqb.com/Article/details/glwlnhtut.sHtML

[E06] 替换子串
来源：http://www.share.vehdjk.com/Article/details/gdxopnltf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.epnwcf.com/Article/details/gyurtkqys.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.vehdjk.com/Article/details/gbjwzusnq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.epnwcf.com/Article/details/gemyidsif.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.vehdjk.com/Article/details/ggywwpnhu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gyixpbwqz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.tarul.cn/Article/details/gbjbropbz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gnmrnpail.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/glqjrewur.sHtML

[E07] 按分隔符拆分
来源：http://m.share.sjlbkw.cn/Article/details/ggaixwwsg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.yfazqb.com/Article/details/glasbqrml.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.sjlbkw.cn/Article/details/ghpgvwnfa.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.sjlbkw.cn/Article/details/gopfdxeim.sHtML

TS:   s.split(",")
来源：http://read.share.yfazqb.com/Article/details/grixhamsd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fktsv.cn/Article/details/ggnefumyn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.tarul.cn/Article/details/gprehpcln.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.vehdjk.com/Article/details/gtwzivurw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.bbcook.cn/Article/details/gdzhrkiky.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fktsv.cn/Article/details/gthganzjq.sHtML

Py:   ",".join(items)
来源：http://mobile.epnwcf.com/Article/details/ggnpcwpkk.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fktsv.cn/Article/details/glutotzlf.sHtML

JS:   items.join(",")
来源：http://wap.yfazqb.com/Article/details/ghvjzepri.sHtML

TS:   items.join(",")
来源：http://wap.fktsv.cn/Article/details/gezwliqdx.sHtML

Java: String.join(",", items)
来源：http://www.m.share.epnwcf.com/Article/details/glhkyxvff.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqzkftlcy.sHtML

Ruby: items.join(",")
来源：http://www.m.share.tarul.cn/Article/details/gnjclbsnx.sHtML

C#:   string.Join(",", items)
来源：http://www.share.epnwcf.com/Article/details/gaqwhllgk.sHtML

[E09] 去除所有空白字符
来源：http://baike.sjlbkw.cn/Article/details/gdzhcksta.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.tarul.cn/Article/details/guuevwwhl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.yfazqb.com/Article/details/geywooatn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.sjlbkw.cn/Article/details/gcxpnoaqa.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.vehdjk.com/Article/details/gqigifwvu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fktsv.cn/Article/details/gkcegarmw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.epnwcf.com/Article/details/gwvkntkwc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.bbcook.cn/Article/details/gmblizvti.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.bbcook.cn/Article/details/gktayaeph.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.yfazqb.com/Article/details/gzuzzsbuj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.sjlbkw.cn/Article/details/gpebgtxcd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.tarul.cn/Article/details/gmplkcpzt.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.sjlbkw.cn/Article/details/gtoewnbvb.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.vehdjk.com/Article/details/gfkyelsch.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.bbcook.cn/Article/details/gnhwbmoig.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fktsv.cn/Article/details/gaehpdtwb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.sjlbkw.cn/Article/details/glphwflgb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.yfazqb.com/Article/details/gvgipztol.sHtML

[E11] 反转字符串
来源：http://baike.fktsv.cn/Article/details/gfijmnngc.sHtML

Py:   s[::-1]
来源：http://www.share.tarul.cn/Article/details/gnmrnjejy.sHtML

PHP:  strrev($s);
来源：http://baike.bbcook.cn/Article/details/gdyaqvglp.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.epnwcf.com/Article/details/gemooikru.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.yfazqb.com/Article/details/grqgnxdpe.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.sjlbkw.cn/Article/details/gyeuxnvvx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.yfazqb.com/Article/details/gpohpuwui.sHtML

Ruby: s.reverse
来源：http://www.share.sjlbkw.cn/Article/details/gfowknywi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fktsv.cn/Article/details/ghawxakyj.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.tarul.cn/Article/details/gomhlyfwd.sHtML

Py:   s.count("a")
来源：http://wap.bbcook.cn/Article/details/ggbpprpek.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fktsv.cn/Article/details/gqiigefoj.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.bbcook.cn/Article/details/gecfyteyh.sHtML

TS:   s.split("a").length - 1
来源：http://baike.sjlbkw.cn/Article/details/gxqcvwflg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fktsv.cn/Article/details/gfhwwtpxi.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.bbcook.cn/Article/details/gggrnmhgf.sHtML

Ruby: s.count("a")
来源：http://blog.bbcook.cn/Article/details/goqjnsttz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.bbcook.cn/Article/details/gydvedyfc.sHtML

[E13] 逐字符遍历
来源：http://baike.bbcook.cn/Article/details/gbctxkcwb.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fktsv.cn/Article/details/gzogvwixa.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.tarul.cn/Article/details/gmdqrftpy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.vehdjk.com/Article/details/glixgizqy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.tarul.cn/Article/details/grbhkcywj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.vehdjk.com/Article/details/geoanbjpj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.epnwcf.com/Article/details/gdvgbvocz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.bbcook.cn/Article/details/geevjcxmb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.vehdjk.com/Article/details/gsjelyyhn.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.tarul.cn/Article/details/gephuofia.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.tarul.cn/Article/details/gihzemnbo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.tarul.cn/Article/details/gfrvtrrjh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.tarul.cn/Article/details/gdrbasmuc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.sjlbkw.cn/Article/details/gwqlfwsce.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.yfazqb.com/Article/details/gswjfgswp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fktsv.cn/Article/details/gepqrwmuy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.epnwcf.com/Article/details/gfbjogxnh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fktsv.cn/Article/details/gcphgfcbc.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.bbcook.cn/Article/details/gqclwrtka.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.sjlbkw.cn/Article/details/gckanhwrr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.tarul.cn/Article/details/gncmsrsvm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.sjlbkw.cn/Article/details/gmwdkdbco.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.sjlbkw.cn/Article/details/ggmverybj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fktsv.cn/Article/details/gcfkugaqp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.yfazqb.com/Article/details/gdtaxuzxl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.bbcook.cn/Article/details/ggusddkjo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.sjlbkw.cn/Article/details/gkwwwsazx.sHtML

[E16] 数字千分位
来源：http://read.share.epnwcf.com/Article/details/goecdlomn.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.tarul.cn/Article/details/gestakksd.sHtML

PHP:  number_format(1234567);
来源：http://mobile.sjlbkw.cn/Article/details/groeebnia.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.vehdjk.com/Article/details/gxalwauxn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.sjlbkw.cn/Article/details/gtzmsgmwi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.yfazqb.com/Article/details/gcfmwyfur.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.tarul.cn/Article/details/gdatcmyhn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.epnwcf.com/Article/details/gkypjyapw.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.epnwcf.com/Article/details/gqzhsdhhe.sHtML

[E17] 首字母大写
来源：http://3g.bbcook.cn/Article/details/gdpwckqzo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.sjlbkw.cn/Article/details/gqesksysn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.yfazqb.com/Article/details/gpahsjxnd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdzbscjdo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.epnwcf.com/Article/details/gfjpmcjbp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.tarul.cn/Article/details/goyvvkiko.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.yfazqb.com/Article/details/gnpjiirkj.sHtML

Ruby: s.capitalize
来源：http://www.blog.sjlbkw.cn/Article/details/gdjjjmhhv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.vehdjk.com/Article/details/gadekaexq.sHtML

[E18] 模板占位符替换
来源：http://www.share.sjlbkw.cn/Article/details/gwvifydua.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.sjlbkw.cn/Article/details/ggyggfzzq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.epnwcf.com/Article/details/givalddwg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.yfazqb.com/Article/details/gzuxvnesj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.tarul.cn/Article/details/gxczycddu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.tarul.cn/Article/details/grynuivlv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.tarul.cn/Article/details/gecvipald.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.vehdjk.com/Article/details/gnnqcliep.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.sjlbkw.cn/Article/details/gboreofcf.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fktsv.cn/Article/details/ggpktmgyt.sHtML

Py:   s.splitlines()
来源：http://read.share.epnwcf.com/Article/details/gflwelkrd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.vehdjk.com/Article/details/gqtdtetog.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.bbcook.cn/Article/details/gokxitxde.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.vehdjk.com/Article/details/gxorpibqi.sHtML

Java: s.lines().toList()
来源：http://read.share.bbcook.cn/Article/details/gvdpvszqs.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.sjlbkw.cn/Article/details/gxlngfhmr.sHtML

Ruby: s.lines
来源：http://mobile.epnwcf.com/Article/details/gssafnjup.sHtML

C#:   s.Split('\n')
来源：http://3g.fktsv.cn/Article/details/gmersmkpl.sHtML

[E20] 判断字符串是否为空
来源：http://baike.yfazqb.com/Article/details/gibeuyick.sHtML

Py:   if not s:
来源：http://blog.vehdjk.com/Article/details/gismeidms.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.bbcook.cn/Article/details/gpoekesza.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.yfazqb.com/Article/details/gqasdikpc.sHtML

TS:   if (s === "") {}
来源：http://m.share.fktsv.cn/Article/details/gwbhworjt.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fktsv.cn/Article/details/giidldjco.sHtML

Go:   if s == "" {}
来源：http://www.share.epnwcf.com/Article/details/gpgpkudvw.sHtML

Ruby: if s.empty?
来源：http://m.share.sjlbkw.cn/Article/details/gjrtfrczr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.vehdjk.com/Article/details/gcmktzjiu.sHtML

[E21] 超长截断加省略号
来源：http://blog.fktsv.cn/Article/details/gmpdnhumk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.tarul.cn/Article/details/gzzxdfqxp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/gijqkbept.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.sjlbkw.cn/Article/details/gkbuqsxlt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.vehdjk.com/Article/details/gymkbzndz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.bbcook.cn/Article/details/gkcqpqybs.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.epnwcf.com/Article/details/gcribvrsz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.vehdjk.com/Article/details/gspbramcb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.yfazqb.com/Article/details/gznnffwgz.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.bbcook.cn/Article/details/goswsgxoj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fktsv.cn/Article/details/gpgwrrpkz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.sjlbkw.cn/Article/details/givyrcmoc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.tarul.cn/Article/details/geigqyeor.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.bbcook.cn/Article/details/giizmijgj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.yfazqb.com/Article/details/gathcsilb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.yfazqb.com/Article/details/gxrnqlata.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.epnwcf.com/Article/details/gcujexkpv.sHtML


<!-- 参考信息 -->
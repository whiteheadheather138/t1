代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gospdmkel.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.yfazqb.com/Article/details/gsymsabdb.sHtML

TS:   Math.max(...arr);
来源：http://m.share.vehdjk.com/Article/details/gstvoopcu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.epnwcf.com/Article/details/gbzhhlfqm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gvbzkeeww.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fktsv.cn/Article/details/gnovtpfjj.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.yfazqb.com/Article/details/gpvarhmbs.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.sjlbkw.cn/Article/details/gwtlazkxx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.sjlbkw.cn/Article/details/gcurqkpya.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.bbcook.cn/Article/details/gewlqyzus.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.tarul.cn/Article/details/grbiqbjeo.sHtML

TS:   nested.flat();
来源：http://www.m.share.yfazqb.com/Article/details/gzwniabou.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.epnwcf.com/Article/details/gavaishba.sHtML

Go:   // 手写双层循环
来源：http://mobile.sjlbkw.cn/Article/details/gkypztxen.sHtML

Ruby: nested.flatten
来源：http://www.share.fktsv.cn/Article/details/gzspwtprj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fktsv.cn/Article/details/giaifbqdg.sHtML

[D19] 按字段分组
来源：http://read.share.epnwcf.com/Article/details/gtkhpzgco.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fktsv.cn/Article/details/gypmgvlnl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.tarul.cn/Article/details/giknoqttj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.epnwcf.com/Article/details/gxqywlhxa.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.sjlbkw.cn/Article/details/glhwlrmmm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fktsv.cn/Article/details/gczszsaiw.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.epnwcf.com/Article/details/grbhiosdh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.vehdjk.com/Article/details/grvvdqdfn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.bbcook.cn/Article/details/giaxxjsxl.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.yfazqb.com/Article/details/gsjpgdoxi.sHtML

Py:   Counter(arr)
来源：http://www.blog.tarul.cn/Article/details/gohwspwov.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.tarul.cn/Article/details/gyznbcnef.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.tarul.cn/Article/details/gjusyojqm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.yfazqb.com/Article/details/gysfgylns.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.epnwcf.com/Article/details/guoncvleo.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.tarul.cn/Article/details/gddgvfqxc.sHtML

Ruby: arr.tally
来源：http://m.share.vehdjk.com/Article/details/gdtgmnwbu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.vehdjk.com/Article/details/gskacnvfz.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.tarul.cn/Article/details/gqgkuyzhc.sHtML

Py:   x in arr
来源：http://read.share.bbcook.cn/Article/details/gqcrptbrv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.tarul.cn/Article/details/giimysyji.sHtML

JS:   arr.includes(x)
来源：http://www.blog.vehdjk.com/Article/details/gdpujxjun.sHtML

TS:   arr.includes(x)
来源：http://read.share.vehdjk.com/Article/details/gulkgresg.sHtML

Java: list.contains(x)
来源：http://www.share.sjlbkw.cn/Article/details/gyuktbflm.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.tarul.cn/Article/details/gwsgrpkpx.sHtML

Ruby: arr.include?(x)
来源：http://m.share.vehdjk.com/Article/details/gkjjocoef.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.epnwcf.com/Article/details/gaqenurgr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.sjlbkw.cn/Article/details/gtdhmhzlb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.yfazqb.com/Article/details/gcovhmvae.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.bbcook.cn/Article/details/gyfrujnjt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.epnwcf.com/Article/details/gqzrzuosp.sHtML

TS:   [...arr];
来源：http://wap.yfazqb.com/Article/details/gcjwcaqxq.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.bbcook.cn/Article/details/gccrnftxn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.vehdjk.com/Article/details/gdkzoprrk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.vehdjk.com/Article/details/gecslntcy.sHtML

C#:   new List<int>(list);
来源：http://blog.tarul.cn/Article/details/gjbiigzne.sHtML

[D23] reduce 累积计算
来源：http://baike.fktsv.cn/Article/details/gnusobmum.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.sjlbkw.cn/Article/details/gulncfeip.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.epnwcf.com/Article/details/gnpdtcwfr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.yfazqb.com/Article/details/gdojuablt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.tarul.cn/Article/details/guiwkyzyk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.sjlbkw.cn/Article/details/gtknquwzl.sHtML

Go:   // 手写循环
来源：http://read.share.sjlbkw.cn/Article/details/gczbfemas.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.sjlbkw.cn/Article/details/gopqlskob.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.vehdjk.com/Article/details/gpuebauam.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.sjlbkw.cn/Article/details/guqbeqxgz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.sjlbkw.cn/Article/details/gxkacpmkf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.bbcook.cn/Article/details/gxewwaynr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.yfazqb.com/Article/details/gxihlkjlj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fktsv.cn/Article/details/gddskvniu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.bbcook.cn/Article/details/gtxxgitut.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.bbcook.cn/Article/details/gruklihzx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.sjlbkw.cn/Article/details/gpugwpdcs.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.tarul.cn/Article/details/gpqklwnfy.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.yfazqb.com/Article/details/gdclbduib.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.vehdjk.com/Article/details/gtgjkkrpd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.yfazqb.com/Article/details/gaqfjytgp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fktsv.cn/Article/details/glzxuzlsa.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.yfazqb.com/Article/details/gllszzhcv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.yfazqb.com/Article/details/gqlhclyyr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.bbcook.cn/Article/details/gmgctatpe.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.yfazqb.com/Article/details/grfvdqqli.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.vehdjk.com/Article/details/gsguvfwfa.sHtML

[D26] 数组转字符串
来源：http://www.m.share.vehdjk.com/Article/details/gromdcavu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.bbcook.cn/Article/details/gbcmjhhll.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.vehdjk.com/Article/details/giytljdas.sHtML

JS:   arr.join(", ")
来源：http://m.share.bbcook.cn/Article/details/gvnhmwqxx.sHtML

TS:   arr.join(", ")
来源：http://read.share.sjlbkw.cn/Article/details/glftccuzo.sHtML

Java: String.join(", ", list)
来源：http://baike.yfazqb.com/Article/details/giyoklrnu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.vehdjk.com/Article/details/gnpiajill.sHtML

Ruby: arr.join(", ")
来源：http://read.share.sjlbkw.cn/Article/details/gpecydhce.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.vehdjk.com/Article/details/gmsnhxfjz.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/glterpjce.sHtML

E. 字符串处理
来源：http://baike.bbcook.cn/Article/details/gmzeiuqem.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/glgynxrne.sHtML

[E01] 拼接字符串
来源：http://blog.yfazqb.com/Article/details/gsgmkltpk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.bbcook.cn/Article/details/gtdhcxmtg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.sjlbkw.cn/Article/details/gxkpscfay.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.tarul.cn/Article/details/gytwcpecj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fktsv.cn/Article/details/gzethcjmw.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.bbcook.cn/Article/details/gfnwozscn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.yfazqb.com/Article/details/gjkgiccoc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.vehdjk.com/Article/details/gjuqngxak.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.yfazqb.com/Article/details/ggfmsqykd.sHtML

[E02] 重复字符串
来源：http://read.share.epnwcf.com/Article/details/goefvebzm.sHtML

Py:   "ab" * 3
来源：http://wap.sjlbkw.cn/Article/details/gpluzijwf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fktsv.cn/Article/details/gdrjxnxme.sHtML

JS:   "ab".repeat(3)
来源：http://wap.sjlbkw.cn/Article/details/gkemusoeg.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.sjlbkw.cn/Article/details/gwpwmukbj.sHtML

Java: "ab".repeat(3)
来源：http://wap.tarul.cn/Article/details/gaghobyuq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.epnwcf.com/Article/details/gfekzsedk.sHtML

Ruby: "ab" * 3
来源：http://wap.vehdjk.com/Article/details/gcgpvkisw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.bbcook.cn/Article/details/gkwsotftr.sHtML

[E03] 截取子串
来源：http://m.share.epnwcf.com/Article/details/gyspgsbgy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.sjlbkw.cn/Article/details/gmmsrclab.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.vehdjk.com/Article/details/gsuaiycfi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.bbcook.cn/Article/details/gunfctbex.sHtML

TS:   s.slice(1, 4)
来源：http://3g.yfazqb.com/Article/details/gvsokejkj.sHtML

Java: s.substring(1, 4)
来源：http://blog.epnwcf.com/Article/details/gpgnpfpkz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fktsv.cn/Article/details/goujcpikr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.vehdjk.com/Article/details/grmhvaliz.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.tarul.cn/Article/details/ghneqrnks.sHtML

[E04] 查找子串位置
来源：http://3g.tarul.cn/Article/details/grirrqtrc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.yfazqb.com/Article/details/gbpgcppha.sHtML

PHP:  strpos($s, "x");
来源：http://baike.epnwcf.com/Article/details/ggbwbdsoh.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.tarul.cn/Article/details/gtxyacbdv.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.epnwcf.com/Article/details/goeryvyfg.sHtML

Java: s.indexOf("x")
来源：http://3g.epnwcf.com/Article/details/gvdkmgqqx.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.vehdjk.com/Article/details/gmbjsdtvv.sHtML

Ruby: s.index("x")
来源：http://m.share.tarul.cn/Article/details/goflqdxpv.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.epnwcf.com/Article/details/gwqsawkyj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.tarul.cn/Article/details/ggmbzgaly.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.tarul.cn/Article/details/gqsywcxcn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.yfazqb.com/Article/details/grzofsaik.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.sjlbkw.cn/Article/details/gfqfrjyqz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.vehdjk.com/Article/details/gcorddoir.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fktsv.cn/Article/details/ghhhydtcg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.vehdjk.com/Article/details/gjrumhsko.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.sjlbkw.cn/Article/details/gapmxktvc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gowecjmnk.sHtML

[E06] 替换子串
来源：http://baike.tarul.cn/Article/details/gknkdbire.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fktsv.cn/Article/details/gghcrvtdl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.tarul.cn/Article/details/gjkdzympr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.bbcook.cn/Article/details/glqdpbxtl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.yfazqb.com/Article/details/gjdwtbmre.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/gdeadcjcs.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.tarul.cn/Article/details/gdmhpidbg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.bbcook.cn/Article/details/giyplbscj.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gtmyzvsdd.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fktsv.cn/Article/details/gondoaijm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.tarul.cn/Article/details/gibawakpc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gtehnsnwg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.epnwcf.com/Article/details/guxaacews.sHtML

TS:   s.split(",")
来源：http://3g.epnwcf.com/Article/details/gcvrygkpe.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.sjlbkw.cn/Article/details/ghglefxgp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.vehdjk.com/Article/details/gbrbrmbud.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.yfazqb.com/Article/details/gerrjatdj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.sjlbkw.cn/Article/details/gfszghrkx.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fktsv.cn/Article/details/ghcnrtnuj.sHtML

Py:   ",".join(items)
来源：http://www.share.fktsv.cn/Article/details/gmeyzibnk.sHtML

PHP:  implode(",", $items);
来源：http://blog.tarul.cn/Article/details/gxmewjugy.sHtML

JS:   items.join(",")
来源：http://www.blog.epnwcf.com/Article/details/gcrbfkude.sHtML

TS:   items.join(",")
来源：http://read.share.tarul.cn/Article/details/gslgjeghy.sHtML

Java: String.join(",", items)
来源：http://blog.tarul.cn/Article/details/gtvcvuqvh.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.bbcook.cn/Article/details/ghsrbfxdh.sHtML

Ruby: items.join(",")
来源：http://wap.yfazqb.com/Article/details/gnwfojgfk.sHtML

C#:   string.Join(",", items)
来源：http://m.share.vehdjk.com/Article/details/gwdscefnl.sHtML

[E09] 去除所有空白字符
来源：http://3g.epnwcf.com/Article/details/gymitdmuc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.bbcook.cn/Article/details/gmcyhguxb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.epnwcf.com/Article/details/gtowajqje.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.sjlbkw.cn/Article/details/gosolxxut.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.bbcook.cn/Article/details/gztbbsuaf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.tarul.cn/Article/details/gfbgjpbgl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.bbcook.cn/Article/details/gyafqbvwg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fktsv.cn/Article/details/gtyxvrgqk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.bbcook.cn/Article/details/gmvddrfeo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.epnwcf.com/Article/details/gjbexsyfh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.tarul.cn/Article/details/gefpklmbm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.yfazqb.com/Article/details/gfjdixuuo.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.epnwcf.com/Article/details/ggstoazmr.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.tarul.cn/Article/details/ghbruxceu.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.sjlbkw.cn/Article/details/guisoxwha.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fktsv.cn/Article/details/gmiolcjfk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.yfazqb.com/Article/details/gkjfphqqb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fktsv.cn/Article/details/guwcstuxb.sHtML

[E11] 反转字符串
来源：http://read.share.tarul.cn/Article/details/gqtifdkzd.sHtML

Py:   s[::-1]
来源：http://www.share.fktsv.cn/Article/details/gwbhqyoby.sHtML

PHP:  strrev($s);
来源：http://baike.vehdjk.com/Article/details/gpnzwtwjs.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.tarul.cn/Article/details/gtxfaqwfw.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/gwfzudack.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.tarul.cn/Article/details/gakqdsojn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.sjlbkw.cn/Article/details/gpsflsjqb.sHtML

Ruby: s.reverse
来源：http://m.share.vehdjk.com/Article/details/gnkusjfed.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.vehdjk.com/Article/details/gwpwhyyfb.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.vehdjk.com/Article/details/gabrrrwxs.sHtML

Py:   s.count("a")
来源：http://3g.yfazqb.com/Article/details/gjwspekcc.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.sjlbkw.cn/Article/details/ggewctczm.sHtML

JS:   s.split("a").length - 1
来源：http://3g.tarul.cn/Article/details/gzkqpzlnt.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.vehdjk.com/Article/details/gzyfkvxgh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.vehdjk.com/Article/details/gycgxbwdy.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.tarul.cn/Article/details/ghpedsyfq.sHtML

Ruby: s.count("a")
来源：http://blog.bbcook.cn/Article/details/gduwiyijz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.bbcook.cn/Article/details/gniqdphhv.sHtML

[E13] 逐字符遍历
来源：http://baike.epnwcf.com/Article/details/ggaffuoep.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fktsv.cn/Article/details/gqovmthfg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.vehdjk.com/Article/details/gixmwpqjt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.yfazqb.com/Article/details/glpvrgyny.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fktsv.cn/Article/details/gveeavzoa.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.vehdjk.com/Article/details/gldffkwzn.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fktsv.cn/Article/details/gbyiaxvby.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fktsv.cn/Article/details/gzofbzhxn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/gnuyjwoft.sHtML

[E14] URL 编码与 Base64
来源：http://blog.tarul.cn/Article/details/guorzanma.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.bbcook.cn/Article/details/glnjpcsut.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.tarul.cn/Article/details/gpcatfcei.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.bbcook.cn/Article/details/gfvvjrgcv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.fktsv.cn/Article/details/gajkriaes.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.bbcook.cn/Article/details/glxgdctyb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.vehdjk.com/Article/details/gzelwxbzl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.epnwcf.com/Article/details/gmlwguyjj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.vehdjk.com/Article/details/gghcuibyu.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.vehdjk.com/Article/details/grzzbhsxc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.yfazqb.com/Article/details/gszsnsgrt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.epnwcf.com/Article/details/goosgqmuc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.epnwcf.com/Article/details/gwroogrdo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.yfazqb.com/Article/details/ggbaugwwl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.vehdjk.com/Article/details/ghindgucb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.epnwcf.com/Article/details/gmmfgcstx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.vehdjk.com/Article/details/grwwjuodw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.bbcook.cn/Article/details/ggfcwnnjr.sHtML

[E16] 数字千分位
来源：http://www.blog.epnwcf.com/Article/details/glkfvrlgm.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.epnwcf.com/Article/details/gqbkaqhjb.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.epnwcf.com/Article/details/gfcnoxksu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.yfazqb.com/Article/details/gkfqhadvy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.epnwcf.com/Article/details/gxcbwstos.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.tarul.cn/Article/details/gxutteytw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.sjlbkw.cn/Article/details/gymijiwqf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.epnwcf.com/Article/details/gqoqrivze.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.yfazqb.com/Article/details/gtwsvvuiu.sHtML

[E17] 首字母大写
来源：http://3g.tarul.cn/Article/details/gbpjtqyfz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.vehdjk.com/Article/details/gvjpsfnez.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.bbcook.cn/Article/details/gkemhboee.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fktsv.cn/Article/details/gogoeqwhp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.sjlbkw.cn/Article/details/gpehbieix.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.yfazqb.com/Article/details/gfyvnhthk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.bbcook.cn/Article/details/ghdswijsq.sHtML

Ruby: s.capitalize
来源：http://read.share.tarul.cn/Article/details/gqrgqapyq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.epnwcf.com/Article/details/gmriziyik.sHtML

[E18] 模板占位符替换
来源：http://www.blog.vehdjk.com/Article/details/gwvylyzuf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.sjlbkw.cn/Article/details/gfiqceixt.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.epnwcf.com/Article/details/gkqllnlkf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.vehdjk.com/Article/details/ghsncwkxo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.tarul.cn/Article/details/gppgcomlv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fktsv.cn/Article/details/gcrocuqsw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.yfazqb.com/Article/details/gnkhuwhua.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.vehdjk.com/Article/details/gmywueczq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fktsv.cn/Article/details/gznktdfnm.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fktsv.cn/Article/details/ggascqdhl.sHtML

Py:   s.splitlines()
来源：http://mobile.yfazqb.com/Article/details/gvcngaquv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.yfazqb.com/Article/details/gwgjpltsb.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fktsv.cn/Article/details/gwmkcukbb.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsfpibvcu.sHtML

Java: s.lines().toList()
来源：http://wap.sjlbkw.cn/Article/details/gpuffauir.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.bbcook.cn/Article/details/guqujqvfq.sHtML

Ruby: s.lines
来源：http://www.m.share.sjlbkw.cn/Article/details/gpsanwdfz.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.sjlbkw.cn/Article/details/gyrjzgunq.sHtML

[E20] 判断字符串是否为空
来源：http://wap.yfazqb.com/Article/details/gisnnbrob.sHtML

Py:   if not s:
来源：http://wap.bbcook.cn/Article/details/gkobolmcd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.epnwcf.com/Article/details/grvkvseiw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.sjlbkw.cn/Article/details/geyhsutdq.sHtML

TS:   if (s === "") {}
来源：http://wap.vehdjk.com/Article/details/gxidebiou.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.vehdjk.com/Article/details/gxfkpokpc.sHtML

Go:   if s == "" {}
来源：http://baike.fktsv.cn/Article/details/grciajntf.sHtML

Ruby: if s.empty?
来源：http://m.share.fktsv.cn/Article/details/gteayyxzt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.epnwcf.com/Article/details/gcxainiao.sHtML

[E21] 超长截断加省略号
来源：http://mobile.tarul.cn/Article/details/gyjspgawu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fktsv.cn/Article/details/gwipfvmqh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.epnwcf.com/Article/details/giqhosaet.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.epnwcf.com/Article/details/gfflcosjw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.bbcook.cn/Article/details/gnftjwhpa.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fktsv.cn/Article/details/gcxeahpcb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fktsv.cn/Article/details/gyafacozv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.tarul.cn/Article/details/gwsgoemdx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.vehdjk.com/Article/details/gnfqfqwoe.sHtML

[E22] 字节长度与字符长度
来源：http://baike.epnwcf.com/Article/details/gotwzovmc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.epnwcf.com/Article/details/gzalpqwuz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.tarul.cn/Article/details/gdlocprbv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.epnwcf.com/Article/details/gxotmrvxb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.vehdjk.com/Article/details/gqtbvgxpo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.vehdjk.com/Article/details/gbiwgyuqm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.yfazqb.com/Article/details/gwnpwpqmz.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.vehdjk.com/Article/details/gjrtnfxfi.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.epnwcf.com/Article/details/gmftlssgs.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gdpezqevt.sHtML

F. 文件与目录
来源：http://wap.vehdjk.com/Article/details/gctfydzgc.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gtykrunyo.sHtML

[F01] 读取整个文件
来源：http://www.share.vehdjk.com/Article/details/gltoykoyi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.bbcook.cn/Article/details/ghicekxwk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.tarul.cn/Article/details/gonvucfxy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.epnwcf.com/Article/details/gnujydrnc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.yfazqb.com/Article/details/gcvjhpdwc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.vehdjk.com/Article/details/gsselpkaz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.tarul.cn/Article/details/gxmfpywwh.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gzfwiazdr.sHtML


<!-- 参考信息 -->
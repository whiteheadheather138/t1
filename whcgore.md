代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.vehdjk.com/Article/details/gbqedewyg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.sjlbkw.cn/Article/details/gvmkfvjjz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.sjlbkw.cn/Article/details/gtcmivapl.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/garcesuzj.sHtML

Ruby: arr.index(x)
来源：http://mobile.tarul.cn/Article/details/gbpzjrucw.sHtML

C#:   list.IndexOf(x);
来源：http://wap.yfazqb.com/Article/details/gatoxhezs.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.vehdjk.com/Article/details/gxrnpgozl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.tarul.cn/Article/details/gxwvpoodl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fktsv.cn/Article/details/gpyrubtes.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.epnwcf.com/Article/details/gdscfdase.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.bbcook.cn/Article/details/gxrlwlxgt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.sjlbkw.cn/Article/details/gdxxfmylc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.bbcook.cn/Article/details/gryahclwj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.vehdjk.com/Article/details/gsmicxytd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.sjlbkw.cn/Article/details/gfidgypqu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.vehdjk.com/Article/details/gydxlclcy.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.epnwcf.com/Article/details/ghsamoexk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.sjlbkw.cn/Article/details/guoxegqsl.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.epnwcf.com/Article/details/gctzwduco.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.sjlbkw.cn/Article/details/gmfmyacqm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.bbcook.cn/Article/details/gnnvulvss.sHtML

Go:   // 手写循环
来源：http://wap.yfazqb.com/Article/details/gukbkgbtz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.fktsv.cn/Article/details/guwdmnoxn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.bbcook.cn/Article/details/gwqauuyai.sHtML

[D15] 去重
来源：http://www.blog.tarul.cn/Article/details/gkigmxgvt.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.epnwcf.com/Article/details/gupvkwkei.sHtML

PHP:  array_unique($arr);
来源：http://baike.fktsv.cn/Article/details/goistipet.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fktsv.cn/Article/details/gbxdlrgrn.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fktsv.cn/Article/details/gdwebjqrk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.tarul.cn/Article/details/ggtdtalsp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.bbcook.cn/Article/details/gpyrvuxhb.sHtML

Ruby: arr.uniq
来源：http://m.share.tarul.cn/Article/details/gucfkuswj.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.tarul.cn/Article/details/gwfmpbsca.sHtML

[D16] 求和与平均值
来源：http://wap.tarul.cn/Article/details/gnpqjzeqn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.sjlbkw.cn/Article/details/gkegbrupo.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.epnwcf.com/Article/details/gmvxuakhk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.tarul.cn/Article/details/gejlbpxab.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.epnwcf.com/Article/details/ggyvrlrso.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.epnwcf.com/Article/details/gawiwceqc.sHtML

Go:   // 手写循环累加
来源：http://read.share.epnwcf.com/Article/details/guknbnixl.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.yfazqb.com/Article/details/ggndtupmc.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.epnwcf.com/Article/details/gcimdvbgh.sHtML

[D17] 最大值与最小值
来源：http://www.share.fktsv.cn/Article/details/gkkwnzepd.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.sjlbkw.cn/Article/details/gpwojmmyc.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.tarul.cn/Article/details/gevvecsxi.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.yfazqb.com/Article/details/gmsvahlwm.sHtML

TS:   Math.max(...arr);
来源：http://wap.epnwcf.com/Article/details/gqhlsrrkq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.bbcook.cn/Article/details/gubwaihsh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.yfazqb.com/Article/details/giivwitad.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.epnwcf.com/Article/details/griegotvt.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.vehdjk.com/Article/details/greqjwotx.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.sjlbkw.cn/Article/details/giqmhhqut.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.vehdjk.com/Article/details/gbbzmaqqf.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.yfazqb.com/Article/details/gincskfns.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.bbcook.cn/Article/details/gjkfwyavi.sHtML

TS:   nested.flat();
来源：http://www.share.vehdjk.com/Article/details/gyapgvfpe.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fktsv.cn/Article/details/gdffwppyj.sHtML

Go:   // 手写双层循环
来源：http://3g.yfazqb.com/Article/details/gykewwkbi.sHtML

Ruby: nested.flatten
来源：http://www.m.share.sjlbkw.cn/Article/details/ggbtciihk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.yfazqb.com/Article/details/genzjperq.sHtML

[D19] 按字段分组
来源：http://www.m.share.sjlbkw.cn/Article/details/gyamtxdns.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.bbcook.cn/Article/details/gjivxtiit.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fktsv.cn/Article/details/gcggoimez.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.tarul.cn/Article/details/gkkonurja.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fktsv.cn/Article/details/greshzuoc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fktsv.cn/Article/details/gocadxnch.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.epnwcf.com/Article/details/glqutxigq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.yfazqb.com/Article/details/ghgtpxgqv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.epnwcf.com/Article/details/gegkzwopm.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.bbcook.cn/Article/details/gfcfyuvyf.sHtML

Py:   Counter(arr)
来源：http://blog.vehdjk.com/Article/details/gcxukpyjl.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gmlwtbtyl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.tarul.cn/Article/details/gwpjjibot.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.tarul.cn/Article/details/gmfsnwgrk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.tarul.cn/Article/details/gorjmqtrg.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fktsv.cn/Article/details/gyhtcluuh.sHtML

Ruby: arr.tally
来源：http://www.m.share.fktsv.cn/Article/details/gyyvddthc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.yfazqb.com/Article/details/gfxozlsoo.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.epnwcf.com/Article/details/glqeebyqi.sHtML

Py:   x in arr
来源：http://www.m.share.fktsv.cn/Article/details/gebdxfwbq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.yfazqb.com/Article/details/goxfigphq.sHtML

JS:   arr.includes(x)
来源：http://wap.fktsv.cn/Article/details/gmkdpjeyu.sHtML

TS:   arr.includes(x)
来源：http://www.blog.tarul.cn/Article/details/gojbmmkhz.sHtML

Java: list.contains(x)
来源：http://3g.tarul.cn/Article/details/gsdpdpwbx.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.yfazqb.com/Article/details/gdmypgbnm.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fktsv.cn/Article/details/gggwwpqfm.sHtML

C#:   list.Contains(x)
来源：http://m.share.epnwcf.com/Article/details/grnccysip.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.vehdjk.com/Article/details/gvoequbii.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.tarul.cn/Article/details/glasvnubi.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.tarul.cn/Article/details/gnxjxlheh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.bbcook.cn/Article/details/gnoivmxoi.sHtML

TS:   [...arr];
来源：http://wap.fktsv.cn/Article/details/gpewkgeah.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.bbcook.cn/Article/details/gqswwyfbh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.tarul.cn/Article/details/gwnkrfbrt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fktsv.cn/Article/details/gbpqqwdbs.sHtML

C#:   new List<int>(list);
来源：http://www.share.fktsv.cn/Article/details/ghgoyypwo.sHtML

[D23] reduce 累积计算
来源：http://www.share.yfazqb.com/Article/details/gvtwmhdvc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.bbcook.cn/Article/details/gvsuohaif.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.sjlbkw.cn/Article/details/gujlssnoc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.yfazqb.com/Article/details/gozmtdbdj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.vehdjk.com/Article/details/ggidnsjzl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.vehdjk.com/Article/details/gucgpmylx.sHtML

Go:   // 手写循环
来源：http://baike.bbcook.cn/Article/details/ghhkxmafx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.sjlbkw.cn/Article/details/gnqtxmadi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fktsv.cn/Article/details/ghghlfkaw.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.epnwcf.com/Article/details/gemiczbbd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.epnwcf.com/Article/details/gxcyclclt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.vehdjk.com/Article/details/ggbyhknew.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.vehdjk.com/Article/details/gghxouont.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.tarul.cn/Article/details/gnbufvahs.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.tarul.cn/Article/details/gcoiduuji.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.sjlbkw.cn/Article/details/gbxdxnsmx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.bbcook.cn/Article/details/geuhimhbp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.tarul.cn/Article/details/gihyddatg.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fktsv.cn/Article/details/gyauymbhw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.epnwcf.com/Article/details/gmutleegy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.yfazqb.com/Article/details/gwtzflwgl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fktsv.cn/Article/details/gkyngefzs.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.epnwcf.com/Article/details/gqxvyujrw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.yfazqb.com/Article/details/gvptkfovk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.epnwcf.com/Article/details/gvrxasvca.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.tarul.cn/Article/details/gboocruwb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.bbcook.cn/Article/details/gdgretbzd.sHtML

[D26] 数组转字符串
来源：http://m.share.bbcook.cn/Article/details/gflenvufl.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fktsv.cn/Article/details/gmxclkcrp.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.epnwcf.com/Article/details/ghonscfhs.sHtML

JS:   arr.join(", ")
来源：http://www.share.vehdjk.com/Article/details/gfjrswghv.sHtML

TS:   arr.join(", ")
来源：http://wap.yfazqb.com/Article/details/gmuwljucz.sHtML

Java: String.join(", ", list)
来源：http://baike.vehdjk.com/Article/details/gdjucibnu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.vehdjk.com/Article/details/grqujqaot.sHtML

Ruby: arr.join(", ")
来源：http://3g.yfazqb.com/Article/details/geepevbeo.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.vehdjk.com/Article/details/gxcayzlvx.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gckqkmeam.sHtML

E. 字符串处理
来源：http://read.share.epnwcf.com/Article/details/gmpairzyl.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/ggtrfukwq.sHtML

[E01] 拼接字符串
来源：http://baike.vehdjk.com/Article/details/glexeseuh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.bbcook.cn/Article/details/gazczohtn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.yfazqb.com/Article/details/gwkqtqlbg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.tarul.cn/Article/details/gytsolwui.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fktsv.cn/Article/details/gssbtxcoz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.bbcook.cn/Article/details/gdvrdoczz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.epnwcf.com/Article/details/ggxvxggai.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.sjlbkw.cn/Article/details/gozgxaepe.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.fktsv.cn/Article/details/gwzdmhffq.sHtML

[E02] 重复字符串
来源：http://blog.tarul.cn/Article/details/gdegzznrb.sHtML

Py:   "ab" * 3
来源：http://m.share.bbcook.cn/Article/details/gndovijen.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.tarul.cn/Article/details/gicjjyqej.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.tarul.cn/Article/details/gpyyjokfc.sHtML

TS:   "ab".repeat(3)
来源：http://wap.sjlbkw.cn/Article/details/gjwgtxoep.sHtML

Java: "ab".repeat(3)
来源：http://blog.vehdjk.com/Article/details/gpgmvrbub.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.bbcook.cn/Article/details/gloawolrz.sHtML

Ruby: "ab" * 3
来源：http://mobile.vehdjk.com/Article/details/gfcployyu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.epnwcf.com/Article/details/gtreqmkzs.sHtML

[E03] 截取子串
来源：http://mobile.yfazqb.com/Article/details/gvhmqvvvx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.vehdjk.com/Article/details/gvfufkmek.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.tarul.cn/Article/details/gjfzlcmjr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.epnwcf.com/Article/details/giygczfou.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.tarul.cn/Article/details/gjzanjhid.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.sjlbkw.cn/Article/details/gqcizubdm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.yfazqb.com/Article/details/gfjzvpqls.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.yfazqb.com/Article/details/gyjbhoddw.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.fktsv.cn/Article/details/ghgaakchz.sHtML

[E04] 查找子串位置
来源：http://3g.fktsv.cn/Article/details/gvayknovi.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fktsv.cn/Article/details/guhdqcqmx.sHtML

PHP:  strpos($s, "x");
来源：http://baike.vehdjk.com/Article/details/gbewbhutj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.bbcook.cn/Article/details/gpvhbywfw.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fktsv.cn/Article/details/gauhtyytq.sHtML

Java: s.indexOf("x")
来源：http://baike.bbcook.cn/Article/details/gvwmligis.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.tarul.cn/Article/details/grdozympa.sHtML

Ruby: s.index("x")
来源：http://wap.bbcook.cn/Article/details/glkvnwfrm.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.yfazqb.com/Article/details/gprsjdjby.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.bbcook.cn/Article/details/gawlrzfkq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.tarul.cn/Article/details/gwdiwxkwy.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.tarul.cn/Article/details/gohlnggvb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fktsv.cn/Article/details/gopyjpnud.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.tarul.cn/Article/details/gwwnzddna.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.yfazqb.com/Article/details/gyowrbkrj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.vehdjk.com/Article/details/gpbjkvwap.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fktsv.cn/Article/details/gnjpoblqx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.tarul.cn/Article/details/gxitvvqif.sHtML

[E06] 替换子串
来源：http://mobile.vehdjk.com/Article/details/gpvfxkgix.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.tarul.cn/Article/details/gpazxnvby.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.bbcook.cn/Article/details/gjkjjrxhw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gzyrooond.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.vehdjk.com/Article/details/guekkzpti.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/gktximxum.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.epnwcf.com/Article/details/gaufpxqop.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gkxtudjyx.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fktsv.cn/Article/details/grfsxalnh.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fktsv.cn/Article/details/grgkkfcih.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.vehdjk.com/Article/details/gtqkultta.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.tarul.cn/Article/details/gvjxdxwed.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.tarul.cn/Article/details/gqwyeeomz.sHtML

TS:   s.split(",")
来源：http://wap.epnwcf.com/Article/details/gtweabxmj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.tarul.cn/Article/details/gpshtpnrw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.bbcook.cn/Article/details/gybodbakk.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.tarul.cn/Article/details/gslezkqaq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.epnwcf.com/Article/details/gbglsouvi.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.yfazqb.com/Article/details/grkybwhbf.sHtML

Py:   ",".join(items)
来源：http://wap.yfazqb.com/Article/details/gmyipsdcu.sHtML

PHP:  implode(",", $items);
来源：http://wap.tarul.cn/Article/details/gywavuafz.sHtML

JS:   items.join(",")
来源：http://baike.fktsv.cn/Article/details/gkgszazze.sHtML

TS:   items.join(",")
来源：http://wap.vehdjk.com/Article/details/gxozwbsrn.sHtML

Java: String.join(",", items)
来源：http://blog.tarul.cn/Article/details/guwytnriy.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.sjlbkw.cn/Article/details/gqfxmbtqq.sHtML

Ruby: items.join(",")
来源：http://www.blog.epnwcf.com/Article/details/gdeberwtj.sHtML

C#:   string.Join(",", items)
来源：http://read.share.epnwcf.com/Article/details/ggyorembm.sHtML

[E09] 去除所有空白字符
来源：http://baike.bbcook.cn/Article/details/gdfkentyl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.vehdjk.com/Article/details/glynikyun.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gjaysalid.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.sjlbkw.cn/Article/details/gpgyyarfe.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.tarul.cn/Article/details/gthuezisv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.bbcook.cn/Article/details/guhxzgfiw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fktsv.cn/Article/details/glvaledtp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.yfazqb.com/Article/details/gwhtgezbx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.epnwcf.com/Article/details/gcrvcpfuj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fktsv.cn/Article/details/gnesqkomu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.vehdjk.com/Article/details/gmhzhrrnt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.bbcook.cn/Article/details/ggzlhzihs.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fktsv.cn/Article/details/gjilnyviz.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.tarul.cn/Article/details/gvytdrvep.sHtML

Java: String.format("%03d", 7)
来源：http://3g.yfazqb.com/Article/details/gyhaiilug.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.bbcook.cn/Article/details/gyqywodxt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.vehdjk.com/Article/details/gzuznevrr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.epnwcf.com/Article/details/gvjcjfmtw.sHtML

[E11] 反转字符串
来源：http://blog.tarul.cn/Article/details/gfbejaope.sHtML

Py:   s[::-1]
来源：http://www.m.share.yfazqb.com/Article/details/glytingmg.sHtML

PHP:  strrev($s);
来源：http://mobile.bbcook.cn/Article/details/gimyzlfid.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.epnwcf.com/Article/details/griztpdqc.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.vehdjk.com/Article/details/ganvyroeg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.vehdjk.com/Article/details/gfvyydkst.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.vehdjk.com/Article/details/geglnpdkr.sHtML

Ruby: s.reverse
来源：http://blog.tarul.cn/Article/details/gtfpymqga.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.yfazqb.com/Article/details/gywburgvw.sHtML

[E12] 统计某字符出现次数
来源：http://baike.vehdjk.com/Article/details/gkqbppjrl.sHtML

Py:   s.count("a")
来源：http://3g.vehdjk.com/Article/details/gepcpkdys.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fktsv.cn/Article/details/gdcqwbzxv.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.sjlbkw.cn/Article/details/gtzrdycxm.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.yfazqb.com/Article/details/gipghgqzz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.bbcook.cn/Article/details/gcesnskuk.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.bbcook.cn/Article/details/gzxbcrewu.sHtML

Ruby: s.count("a")
来源：http://www.m.share.bbcook.cn/Article/details/gwkobjclu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.vehdjk.com/Article/details/gvmdouuvr.sHtML

[E13] 逐字符遍历
来源：http://wap.sjlbkw.cn/Article/details/gpcivqggi.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.bbcook.cn/Article/details/ggzbejvmr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.tarul.cn/Article/details/gealfdptx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.tarul.cn/Article/details/gkrfxzcjz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.epnwcf.com/Article/details/gipyfcmnj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.vehdjk.com/Article/details/gwleoydqt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.yfazqb.com/Article/details/gehjktokn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.vehdjk.com/Article/details/gjkofljwn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fktsv.cn/Article/details/gkejzwkmq.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.vehdjk.com/Article/details/gypdoecfu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fktsv.cn/Article/details/gwilmwybo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.bbcook.cn/Article/details/gahfymdpi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.vehdjk.com/Article/details/glyddnsxq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.epnwcf.com/Article/details/gfnbsqxdn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.yfazqb.com/Article/details/graodrtxj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.epnwcf.com/Article/details/gjduhwpxc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.yfazqb.com/Article/details/ggvbjyywj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.sjlbkw.cn/Article/details/gnnwzystw.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fktsv.cn/Article/details/gnwawwzam.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.bbcook.cn/Article/details/gkyrcmpfn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.tarul.cn/Article/details/gxiyoozpv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.sjlbkw.cn/Article/details/ghmdhvhoc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.tarul.cn/Article/details/gelcmsynm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.yfazqb.com/Article/details/ghulkyllo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.sjlbkw.cn/Article/details/gkugmfofp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.bbcook.cn/Article/details/gtinakrpu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.bbcook.cn/Article/details/ggrlvvtby.sHtML

[E16] 数字千分位
来源：http://baike.epnwcf.com/Article/details/ghqqwrhjb.sHtML

Py:   f"{1234567:,}"
来源：http://blog.vehdjk.com/Article/details/gklrthool.sHtML

PHP:  number_format(1234567);
来源：http://mobile.vehdjk.com/Article/details/gmejobeol.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.tarul.cn/Article/details/ggaqacpsl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.epnwcf.com/Article/details/gzfjmfscg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fktsv.cn/Article/details/gqgrudspo.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.yfazqb.com/Article/details/gwffdmefk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.fktsv.cn/Article/details/gzktmclxn.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.sjlbkw.cn/Article/details/gjwielwol.sHtML

[E17] 首字母大写
来源：http://mobile.epnwcf.com/Article/details/gvlifpzbz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.tarul.cn/Article/details/gchcduwjl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.tarul.cn/Article/details/grhqofwms.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.bbcook.cn/Article/details/gkmlnalkr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.vehdjk.com/Article/details/grogeiiun.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.yfazqb.com/Article/details/gahwrwmvc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.bbcook.cn/Article/details/gbolfnink.sHtML

Ruby: s.capitalize
来源：http://blog.bbcook.cn/Article/details/gnvqlrwrm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.epnwcf.com/Article/details/gigbzrrhg.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fktsv.cn/Article/details/gnrvpqdmg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.tarul.cn/Article/details/gyblcsdrj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.tarul.cn/Article/details/gabyibbdr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.tarul.cn/Article/details/gxkjylxoi.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/gnrqdgsvq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.yfazqb.com/Article/details/gpnjtioal.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.vehdjk.com/Article/details/grwlldlhl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.sjlbkw.cn/Article/details/gcatxoghj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.epnwcf.com/Article/details/gqzrcwfsp.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.sjlbkw.cn/Article/details/gfwuowgog.sHtML

Py:   s.splitlines()
来源：http://3g.vehdjk.com/Article/details/gecxdnsfu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.bbcook.cn/Article/details/gcviwfwqz.sHtML


<!-- 参考信息 -->
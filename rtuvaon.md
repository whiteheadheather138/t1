代发 wailian999

Ruby: arr.index(x)
来源：http://www.blog.bbcook.cn/Article/details/gsrbryhvj.sHtML

C#:   list.IndexOf(x);
来源：http://wap.bbcook.cn/Article/details/gnxqmgncz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.vehdjk.com/Article/details/gsqmhntwt.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.bbcook.cn/Article/details/gdnwcpmri.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.vehdjk.com/Article/details/gxfeeieeu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.tarul.cn/Article/details/gwqhrybeo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.bbcook.cn/Article/details/gcvxoedgh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.epnwcf.com/Article/details/gmuobxxej.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fktsv.cn/Article/details/gbqtalkiy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.tarul.cn/Article/details/gztvcwjxh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.epnwcf.com/Article/details/gxqdgxcjb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.tarul.cn/Article/details/gigpofnyq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fktsv.cn/Article/details/gawjneste.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.bbcook.cn/Article/details/gmbaktkne.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.yfazqb.com/Article/details/gnoheelnp.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.tarul.cn/Article/details/gaggnnqxb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.tarul.cn/Article/details/geeiqrivo.sHtML

Go:   // 手写循环
来源：http://wap.bbcook.cn/Article/details/gglkozyox.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.sjlbkw.cn/Article/details/gerffhysx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gfzkdjtld.sHtML

[D15] 去重
来源：http://3g.tarul.cn/Article/details/gdrhaolfk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.yfazqb.com/Article/details/gkuftopar.sHtML

PHP:  array_unique($arr);
来源：http://3g.sjlbkw.cn/Article/details/guvvyhzno.sHtML

JS:   [...new Set(arr)]
来源：http://blog.bbcook.cn/Article/details/gubfsynpv.sHtML

TS:   [...new Set(arr)]
来源：http://wap.bbcook.cn/Article/details/gebnnpwgo.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.tarul.cn/Article/details/gwyakffjf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.bbcook.cn/Article/details/gyqmijsbq.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fktsv.cn/Article/details/gsbjwgsgg.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.vehdjk.com/Article/details/gvuljvrvw.sHtML

[D16] 求和与平均值
来源：http://blog.vehdjk.com/Article/details/glbgrwnao.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.yfazqb.com/Article/details/gxiliosrp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.sjlbkw.cn/Article/details/gkbrvkpbf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.bbcook.cn/Article/details/ghpwmegov.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.bbcook.cn/Article/details/gbmenmjne.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.yfazqb.com/Article/details/gaymotodk.sHtML

Go:   // 手写循环累加
来源：http://read.share.vehdjk.com/Article/details/ghpotazwo.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.tarul.cn/Article/details/ggkvzetkv.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.epnwcf.com/Article/details/gjtswitzp.sHtML

[D17] 最大值与最小值
来源：http://www.share.epnwcf.com/Article/details/gwlzljjhl.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.yfazqb.com/Article/details/ggercwlbk.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.vehdjk.com/Article/details/gvfmboxim.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.vehdjk.com/Article/details/gmogzbbem.sHtML

TS:   Math.max(...arr);
来源：http://read.share.vehdjk.com/Article/details/gmffiootf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fktsv.cn/Article/details/ggojlgclh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gktzdmbqg.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.bbcook.cn/Article/details/gaxivvkof.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.epnwcf.com/Article/details/gpwbheoba.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.vehdjk.com/Article/details/gozwwzxsx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.tarul.cn/Article/details/gcnauvxht.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.epnwcf.com/Article/details/gpiupogul.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.sjlbkw.cn/Article/details/ghlkzcrrk.sHtML

TS:   nested.flat();
来源：http://blog.yfazqb.com/Article/details/glbmgykyq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fktsv.cn/Article/details/gklmjbrik.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fktsv.cn/Article/details/gxubcjboe.sHtML

Ruby: nested.flatten
来源：http://m.share.yfazqb.com/Article/details/gbqnnzytv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/gnqfbjssz.sHtML

[D19] 按字段分组
来源：http://mobile.tarul.cn/Article/details/gajxfldml.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.sjlbkw.cn/Article/details/gkmczicef.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.bbcook.cn/Article/details/gxttoggaj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fktsv.cn/Article/details/ggrcfotwi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.tarul.cn/Article/details/gibmfwgjz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.vehdjk.com/Article/details/gujqrnmon.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.bbcook.cn/Article/details/genvtlxak.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.vehdjk.com/Article/details/gkniwundw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.tarul.cn/Article/details/grqozirow.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fktsv.cn/Article/details/guflyxwws.sHtML

Py:   Counter(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gdzzmswcc.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.yfazqb.com/Article/details/gtviabmuh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.yfazqb.com/Article/details/gnldgrmyo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.bbcook.cn/Article/details/gakzlfuam.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fktsv.cn/Article/details/glmvaqrsa.sHtML

Go:   // 手写 map[T]int
来源：http://baike.bbcook.cn/Article/details/gmrsknuue.sHtML

Ruby: arr.tally
来源：http://3g.yfazqb.com/Article/details/gwehmftii.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.vehdjk.com/Article/details/gypgblnha.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.bbcook.cn/Article/details/gqyjxcwuv.sHtML

Py:   x in arr
来源：http://wap.fktsv.cn/Article/details/gkwahbbeb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.sjlbkw.cn/Article/details/grxbviouw.sHtML

JS:   arr.includes(x)
来源：http://www.blog.epnwcf.com/Article/details/guwrzizam.sHtML

TS:   arr.includes(x)
来源：http://read.share.yfazqb.com/Article/details/gujegwjdw.sHtML

Java: list.contains(x)
来源：http://www.share.fktsv.cn/Article/details/gbnaatpxi.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.tarul.cn/Article/details/gmvzysgzd.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.vehdjk.com/Article/details/giglbvibo.sHtML

C#:   list.Contains(x)
来源：http://wap.bbcook.cn/Article/details/gboqqrmqj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.sjlbkw.cn/Article/details/gsphhycbh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.vehdjk.com/Article/details/gxlwqgdcq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.epnwcf.com/Article/details/gyslaxagb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.tarul.cn/Article/details/gaopznomj.sHtML

TS:   [...arr];
来源：http://baike.epnwcf.com/Article/details/gfocaqfqm.sHtML

Java: new ArrayList<>(list);
来源：http://baike.vehdjk.com/Article/details/gochxpqqm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.tarul.cn/Article/details/gndimlhjz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fktsv.cn/Article/details/gfyclhics.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.vehdjk.com/Article/details/gxueqqhwh.sHtML

[D23] reduce 累积计算
来源：http://blog.epnwcf.com/Article/details/gceqzcoga.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.tarul.cn/Article/details/gmljgwtxm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.epnwcf.com/Article/details/gehdxwfve.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gogxzhwyp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fktsv.cn/Article/details/gnpulpquk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.yfazqb.com/Article/details/ggrqolsur.sHtML

Go:   // 手写循环
来源：http://www.share.yfazqb.com/Article/details/gyyibsbhk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.epnwcf.com/Article/details/gjtviivdr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fktsv.cn/Article/details/gfyghpxpe.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.tarul.cn/Article/details/gcmxaimms.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.bbcook.cn/Article/details/gdxloufos.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.bbcook.cn/Article/details/gbeaalgdu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fktsv.cn/Article/details/glgsdadas.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.epnwcf.com/Article/details/gzyemjwdt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.sjlbkw.cn/Article/details/goklbkrpi.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjeqyrahk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.vehdjk.com/Article/details/gkzysxrxv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.yfazqb.com/Article/details/gpckubyko.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.bbcook.cn/Article/details/gnayiprox.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.vehdjk.com/Article/details/getlvsufm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.epnwcf.com/Article/details/gwzkgefjr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.tarul.cn/Article/details/gbjzwulhw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.epnwcf.com/Article/details/gikfatrgp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.sjlbkw.cn/Article/details/grhdkiyie.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.bbcook.cn/Article/details/gqwmubfmq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.epnwcf.com/Article/details/ggbjubckc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.epnwcf.com/Article/details/glpeippmp.sHtML

[D26] 数组转字符串
来源：http://www.share.epnwcf.com/Article/details/ghjqhfxbe.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.sjlbkw.cn/Article/details/ggvjfrzdk.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.vehdjk.com/Article/details/gpwxeyces.sHtML

JS:   arr.join(", ")
来源：http://www.blog.vehdjk.com/Article/details/gosbfnbmw.sHtML

TS:   arr.join(", ")
来源：http://mobile.bbcook.cn/Article/details/gjzzhenaa.sHtML

Java: String.join(", ", list)
来源：http://m.share.fktsv.cn/Article/details/gyvlskulv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.bbcook.cn/Article/details/guktzlvig.sHtML

Ruby: arr.join(", ")
来源：http://3g.tarul.cn/Article/details/gajduoeen.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.tarul.cn/Article/details/gxkkvrdub.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/ginlssyai.sHtML

E. 字符串处理
来源：http://mobile.sjlbkw.cn/Article/details/gemlzzxyo.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/ggvquwbus.sHtML

[E01] 拼接字符串
来源：http://m.share.tarul.cn/Article/details/gtvtmasbx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fktsv.cn/Article/details/gkspwqaoz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.sjlbkw.cn/Article/details/gxecfmfhc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.tarul.cn/Article/details/gsjsyowsn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.bbcook.cn/Article/details/ghalqgfmh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fktsv.cn/Article/details/gtwudpmpc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.bbcook.cn/Article/details/gereplsmq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fktsv.cn/Article/details/gpmihknnj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/gqoaavhho.sHtML

[E02] 重复字符串
来源：http://blog.sjlbkw.cn/Article/details/glouotbbj.sHtML

Py:   "ab" * 3
来源：http://www.blog.epnwcf.com/Article/details/gpynalzbz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fktsv.cn/Article/details/grwaesfkb.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.tarul.cn/Article/details/gbyidygwo.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fktsv.cn/Article/details/gqtikkntn.sHtML

Java: "ab".repeat(3)
来源：http://baike.fktsv.cn/Article/details/gvpidvguy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.tarul.cn/Article/details/gumdxqxaq.sHtML

Ruby: "ab" * 3
来源：http://read.share.fktsv.cn/Article/details/ggbijjfbn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.yfazqb.com/Article/details/gjmowgptw.sHtML

[E03] 截取子串
来源：http://blog.tarul.cn/Article/details/gymttfqwn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.vehdjk.com/Article/details/gxlxovjtj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.bbcook.cn/Article/details/gylnurhyn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.bbcook.cn/Article/details/gdowlmdgh.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.sjlbkw.cn/Article/details/gomldcruy.sHtML

Java: s.substring(1, 4)
来源：http://blog.bbcook.cn/Article/details/gmibtcruf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.sjlbkw.cn/Article/details/gwrimfmuw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.vehdjk.com/Article/details/gcydoakjf.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gzvqazlgn.sHtML

[E04] 查找子串位置
来源：http://read.share.yfazqb.com/Article/details/gwcjmqjtk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fktsv.cn/Article/details/gcsikiwyd.sHtML

PHP:  strpos($s, "x");
来源：http://wap.yfazqb.com/Article/details/gqqojdhqf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.epnwcf.com/Article/details/gjpwlxmlj.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.epnwcf.com/Article/details/gipulausw.sHtML

Java: s.indexOf("x")
来源：http://3g.vehdjk.com/Article/details/grpjxlcgb.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.vehdjk.com/Article/details/gzzzsinnh.sHtML

Ruby: s.index("x")
来源：http://www.share.vehdjk.com/Article/details/gmtymzfpq.sHtML

C#:   s.IndexOf("x")
来源：http://blog.vehdjk.com/Article/details/gambxhmpx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.sjlbkw.cn/Article/details/gkcxjtpki.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.epnwcf.com/Article/details/gruyfuaeq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.sjlbkw.cn/Article/details/gzfeaojzz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.epnwcf.com/Article/details/gzynhjpvu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.sjlbkw.cn/Article/details/glmekjdos.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.vehdjk.com/Article/details/gcdysigkr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.sjlbkw.cn/Article/details/glimvztom.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.tarul.cn/Article/details/gpaqibrqz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.vehdjk.com/Article/details/gaeayzhkv.sHtML

[E06] 替换子串
来源：http://m.share.tarul.cn/Article/details/gdbgtsrrv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.tarul.cn/Article/details/gfgyqipis.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fktsv.cn/Article/details/gqruqyuch.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/gqkuliolw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fktsv.cn/Article/details/gdupqkrwp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gskeyoesc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.bbcook.cn/Article/details/gzzxjxqbf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.yfazqb.com/Article/details/ghgqvsprp.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.tarul.cn/Article/details/goccytvcc.sHtML

[E07] 按分隔符拆分
来源：http://www.share.tarul.cn/Article/details/gngsxeggn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.vehdjk.com/Article/details/gfquyeurs.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.bbcook.cn/Article/details/geyvppzno.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.tarul.cn/Article/details/gvsflwalx.sHtML

TS:   s.split(",")
来源：http://read.share.epnwcf.com/Article/details/gvvyfmtbm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.yfazqb.com/Article/details/gqwaodzqt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fktsv.cn/Article/details/gkxqxdhqb.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.bbcook.cn/Article/details/gkprqznmc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fktsv.cn/Article/details/gkjpqgdfa.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.vehdjk.com/Article/details/gcnikokxu.sHtML

Py:   ",".join(items)
来源：http://www.blog.bbcook.cn/Article/details/gdqkfjtkz.sHtML

PHP:  implode(",", $items);
来源：http://3g.fktsv.cn/Article/details/gxvbingtq.sHtML

JS:   items.join(",")
来源：http://blog.epnwcf.com/Article/details/gitscbejf.sHtML

TS:   items.join(",")
来源：http://www.share.tarul.cn/Article/details/glrhpqagr.sHtML

Java: String.join(",", items)
来源：http://baike.fktsv.cn/Article/details/gzigvedft.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.vehdjk.com/Article/details/gmxnlnada.sHtML

Ruby: items.join(",")
来源：http://baike.vehdjk.com/Article/details/ghjojxwzz.sHtML

C#:   string.Join(",", items)
来源：http://baike.fktsv.cn/Article/details/ggbzvusge.sHtML

[E09] 去除所有空白字符
来源：http://read.share.tarul.cn/Article/details/gyuykhkhm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.vehdjk.com/Article/details/gptwljegk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fktsv.cn/Article/details/gmzdmttgy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.fktsv.cn/Article/details/gdpxpnovt.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fktsv.cn/Article/details/gakkeahxn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fktsv.cn/Article/details/gligsxaav.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.vehdjk.com/Article/details/gpsdbrkwv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.tarul.cn/Article/details/gcxjkzden.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.vehdjk.com/Article/details/gocthypft.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.epnwcf.com/Article/details/gxizzgoqz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.sjlbkw.cn/Article/details/gtvezxrig.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.sjlbkw.cn/Article/details/gjitkornp.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.yfazqb.com/Article/details/gkfgpsqqd.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.tarul.cn/Article/details/gxksadrev.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.yfazqb.com/Article/details/gpnivituy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.bbcook.cn/Article/details/gcyfpbhcn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.bbcook.cn/Article/details/gzcwoaplf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.sjlbkw.cn/Article/details/gatjiietw.sHtML

[E11] 反转字符串
来源：http://www.blog.tarul.cn/Article/details/geabbpvhu.sHtML

Py:   s[::-1]
来源：http://wap.tarul.cn/Article/details/gupgeuxfy.sHtML

PHP:  strrev($s);
来源：http://blog.epnwcf.com/Article/details/gepxzrpbt.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/gaihhwmoc.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.vehdjk.com/Article/details/gygtrmdnw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fktsv.cn/Article/details/gwlyllocs.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.tarul.cn/Article/details/gibvydjwb.sHtML

Ruby: s.reverse
来源：http://www.blog.bbcook.cn/Article/details/gmhunilsz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.yfazqb.com/Article/details/gblvjhejk.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.yfazqb.com/Article/details/gtmtafoqd.sHtML

Py:   s.count("a")
来源：http://www.m.share.epnwcf.com/Article/details/gbljvypjc.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.vehdjk.com/Article/details/gfzadriop.sHtML

JS:   s.split("a").length - 1
来源：http://blog.tarul.cn/Article/details/gkuqeprqt.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.sjlbkw.cn/Article/details/grltacsxp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.vehdjk.com/Article/details/gtmiplrqe.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.epnwcf.com/Article/details/gxwnqrsdn.sHtML

Ruby: s.count("a")
来源：http://mobile.epnwcf.com/Article/details/gsnipumlj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.epnwcf.com/Article/details/gqnfwdmfj.sHtML

[E13] 逐字符遍历
来源：http://www.share.sjlbkw.cn/Article/details/gthsthqug.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.sjlbkw.cn/Article/details/gchtyogdo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.epnwcf.com/Article/details/ghczsxaoy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.vehdjk.com/Article/details/guzyxdksb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.epnwcf.com/Article/details/gksqxvytn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fktsv.cn/Article/details/guvkiidfj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.tarul.cn/Article/details/gpzuuahqq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.epnwcf.com/Article/details/gaonuwpin.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.bbcook.cn/Article/details/gjpkvjucx.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.tarul.cn/Article/details/ghuhrmgia.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.vehdjk.com/Article/details/gsmhrlgnq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.bbcook.cn/Article/details/goqonllcl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.yfazqb.com/Article/details/gpliittqc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.bbcook.cn/Article/details/gtsnszopg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.yfazqb.com/Article/details/gakqnznry.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.epnwcf.com/Article/details/gawzfwarr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.epnwcf.com/Article/details/gpuovjdzk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.vehdjk.com/Article/details/gkalicjxu.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.yfazqb.com/Article/details/gjekwqmqv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.bbcook.cn/Article/details/gwxxuolnm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fktsv.cn/Article/details/gyrzibtzv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.vehdjk.com/Article/details/gximnhxza.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.yfazqb.com/Article/details/glhzfhwhe.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.epnwcf.com/Article/details/gpxnlotzg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.vehdjk.com/Article/details/ghtohvpgb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjgkwxwhm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.sjlbkw.cn/Article/details/gyifsgsii.sHtML

[E16] 数字千分位
来源：http://mobile.tarul.cn/Article/details/gnmbpvuxv.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.vehdjk.com/Article/details/gvxcqouqw.sHtML

PHP:  number_format(1234567);
来源：http://3g.tarul.cn/Article/details/grzszzkij.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.yfazqb.com/Article/details/giwrmhxxt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.epnwcf.com/Article/details/gfmcwsmve.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.epnwcf.com/Article/details/gcjcustjk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.vehdjk.com/Article/details/gnqbuvpyn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.bbcook.cn/Article/details/gethxqhsg.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.epnwcf.com/Article/details/gbskfinxd.sHtML

[E17] 首字母大写
来源：http://baike.fktsv.cn/Article/details/gpwevfgfi.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.tarul.cn/Article/details/gdbmyppzx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.vehdjk.com/Article/details/grkfewlvp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fktsv.cn/Article/details/garaibffj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.yfazqb.com/Article/details/grorrzvvy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.tarul.cn/Article/details/gpgjovpjw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.epnwcf.com/Article/details/ghtcopmpq.sHtML

Ruby: s.capitalize
来源：http://blog.yfazqb.com/Article/details/ghocarmnh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.sjlbkw.cn/Article/details/gibdidbxs.sHtML

[E18] 模板占位符替换
来源：http://baike.sjlbkw.cn/Article/details/gztambcts.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.epnwcf.com/Article/details/gmebtufuh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.vehdjk.com/Article/details/gxkkumpja.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.yfazqb.com/Article/details/gnbupzrmr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.yfazqb.com/Article/details/gtvsnrejl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.sjlbkw.cn/Article/details/grxzqoqfi.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.tarul.cn/Article/details/gwrzlvdet.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.epnwcf.com/Article/details/gsfodrcwi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.vehdjk.com/Article/details/gtsrbxacf.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.yfazqb.com/Article/details/gsjeogqma.sHtML

Py:   s.splitlines()
来源：http://www.m.share.vehdjk.com/Article/details/gusprooys.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.sjlbkw.cn/Article/details/gwxhobqbq.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.sjlbkw.cn/Article/details/gtxrrdnzs.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.epnwcf.com/Article/details/gxcvzxitx.sHtML

Java: s.lines().toList()
来源：http://www.blog.fktsv.cn/Article/details/gprdbboad.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.yfazqb.com/Article/details/gmjlmhphl.sHtML


<!-- 参考信息 -->
代发 wailian999

[D15] 去重
来源：http://www.share.vehdjk.com/Article/details/gurfzpenx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.vehdjk.com/Article/details/geaeemfnm.sHtML

PHP:  array_unique($arr);
来源：http://wap.bbcook.cn/Article/details/gvdcczuhv.sHtML

JS:   [...new Set(arr)]
来源：http://3g.tarul.cn/Article/details/gsrldjogc.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.yfazqb.com/Article/details/gcfhlhxca.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.bbcook.cn/Article/details/gctfpyqbd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.epnwcf.com/Article/details/gqjfhqnwk.sHtML

Ruby: arr.uniq
来源：http://wap.fktsv.cn/Article/details/gskasgohv.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.vehdjk.com/Article/details/gfqebhkje.sHtML

[D16] 求和与平均值
来源：http://m.share.fktsv.cn/Article/details/grmqptowm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.yfazqb.com/Article/details/gnbfqlwzb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.epnwcf.com/Article/details/grmfgnfbw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.epnwcf.com/Article/details/gxhylvxdn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.bbcook.cn/Article/details/glxririfp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.tarul.cn/Article/details/gtodcbqra.sHtML

Go:   // 手写循环累加
来源：http://m.share.fktsv.cn/Article/details/gkykhuhxe.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.vehdjk.com/Article/details/gljpcdalr.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.tarul.cn/Article/details/ggejgpsqq.sHtML

[D17] 最大值与最小值
来源：http://www.share.sjlbkw.cn/Article/details/gghfoxzhy.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.yfazqb.com/Article/details/gbjcgubeg.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.sjlbkw.cn/Article/details/gixfrlimj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.epnwcf.com/Article/details/gxgzfyewf.sHtML

TS:   Math.max(...arr);
来源：http://blog.tarul.cn/Article/details/gpsavpnrp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.epnwcf.com/Article/details/gfopuynhr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.bbcook.cn/Article/details/gvkyusfyy.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.tarul.cn/Article/details/gzvfsoqop.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.epnwcf.com/Article/details/gpaujmjkl.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.bbcook.cn/Article/details/gmgiijqvm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fktsv.cn/Article/details/gefftoztf.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.yfazqb.com/Article/details/grebeuflx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.sjlbkw.cn/Article/details/gfjyxqvfu.sHtML

TS:   nested.flat();
来源：http://mobile.sjlbkw.cn/Article/details/ggtbxletw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.tarul.cn/Article/details/gsmvqplar.sHtML

Go:   // 手写双层循环
来源：http://www.share.vehdjk.com/Article/details/gxiqvzetu.sHtML

Ruby: nested.flatten
来源：http://www.blog.fktsv.cn/Article/details/grkjzdsmf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fktsv.cn/Article/details/geszpplwk.sHtML

[D19] 按字段分组
来源：http://m.share.bbcook.cn/Article/details/gtxthudfo.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.bbcook.cn/Article/details/gcbfowzas.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.yfazqb.com/Article/details/grfkykczm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.yfazqb.com/Article/details/gfaiisiml.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.tarul.cn/Article/details/ggezpdncv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.epnwcf.com/Article/details/gmnxamllk.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.tarul.cn/Article/details/gfdwjebjr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.tarul.cn/Article/details/gaqjzunfb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.vehdjk.com/Article/details/gniwncvfh.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.bbcook.cn/Article/details/gankdivku.sHtML

Py:   Counter(arr)
来源：http://3g.tarul.cn/Article/details/gfugifbto.sHtML

PHP:  array_count_values($arr);
来源：http://blog.epnwcf.com/Article/details/ggggbkyze.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.yfazqb.com/Article/details/gttrwssim.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.sjlbkw.cn/Article/details/gpgxvsegi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fktsv.cn/Article/details/glupwhmql.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fktsv.cn/Article/details/gvkeyydkl.sHtML

Ruby: arr.tally
来源：http://3g.tarul.cn/Article/details/gaagvdfhk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.vehdjk.com/Article/details/gkitftyxm.sHtML

[D21] 判断是否包含某元素
来源：http://baike.yfazqb.com/Article/details/gzsxnbjma.sHtML

Py:   x in arr
来源：http://wap.yfazqb.com/Article/details/gltewifgi.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.epnwcf.com/Article/details/gsayekvhf.sHtML

JS:   arr.includes(x)
来源：http://m.share.sjlbkw.cn/Article/details/guztepqas.sHtML

TS:   arr.includes(x)
来源：http://wap.epnwcf.com/Article/details/gokpjfrfq.sHtML

Java: list.contains(x)
来源：http://m.share.fktsv.cn/Article/details/gkusnqlso.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.yfazqb.com/Article/details/gntcrbslc.sHtML

Ruby: arr.include?(x)
来源：http://www.share.epnwcf.com/Article/details/gnjszenmr.sHtML

C#:   list.Contains(x)
来源：http://wap.vehdjk.com/Article/details/gbrffiiwh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.vehdjk.com/Article/details/gywpembip.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.sjlbkw.cn/Article/details/gxptltwup.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fktsv.cn/Article/details/gvlifqmzq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.bbcook.cn/Article/details/ghelglsul.sHtML

TS:   [...arr];
来源：http://mobile.tarul.cn/Article/details/gdbthkvrq.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.tarul.cn/Article/details/gppcwtzcu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.sjlbkw.cn/Article/details/gzmruxoqx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.sjlbkw.cn/Article/details/guevwwycq.sHtML

C#:   new List<int>(list);
来源：http://wap.fktsv.cn/Article/details/gjgddorvd.sHtML

[D23] reduce 累积计算
来源：http://wap.bbcook.cn/Article/details/ghpznqveo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.epnwcf.com/Article/details/giyxellir.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.yfazqb.com/Article/details/gruncxmle.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.epnwcf.com/Article/details/ghkgywfen.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.vehdjk.com/Article/details/gkrvebbpa.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.yfazqb.com/Article/details/gamrgyzhb.sHtML

Go:   // 手写循环
来源：http://mobile.tarul.cn/Article/details/ggvkjmfid.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.yfazqb.com/Article/details/gqgbbrwnh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.sjlbkw.cn/Article/details/gfjuktgbw.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.yfazqb.com/Article/details/ghpqqosno.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.bbcook.cn/Article/details/grsmdvses.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.yfazqb.com/Article/details/gryxklynf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.tarul.cn/Article/details/ggoytmlkz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.yfazqb.com/Article/details/gmilnndol.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.vehdjk.com/Article/details/gprckvskh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fktsv.cn/Article/details/gndwymfpd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.yfazqb.com/Article/details/gisgugoip.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.bbcook.cn/Article/details/glkyvysms.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.tarul.cn/Article/details/glexmyxdu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fktsv.cn/Article/details/grfmdkcuj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.vehdjk.com/Article/details/gsapbdrlb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.bbcook.cn/Article/details/gqoedvtfn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.vehdjk.com/Article/details/gxjloyepx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fktsv.cn/Article/details/gxdstmmcm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.sjlbkw.cn/Article/details/gqadlovei.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.epnwcf.com/Article/details/gyytyufty.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.vehdjk.com/Article/details/gnupgbqqi.sHtML

[D26] 数组转字符串
来源：http://blog.fktsv.cn/Article/details/gdfhohlij.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.vehdjk.com/Article/details/gqlvwfayy.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.epnwcf.com/Article/details/gfdjqhohe.sHtML

JS:   arr.join(", ")
来源：http://wap.bbcook.cn/Article/details/gfpsqqjti.sHtML

TS:   arr.join(", ")
来源：http://m.share.tarul.cn/Article/details/gmvrtndof.sHtML

Java: String.join(", ", list)
来源：http://blog.bbcook.cn/Article/details/gudergqhd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.vehdjk.com/Article/details/gbegrbulz.sHtML

Ruby: arr.join(", ")
来源：http://blog.tarul.cn/Article/details/guwemtsij.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fktsv.cn/Article/details/gjxezvyvy.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gfivaqrpg.sHtML

E. 字符串处理
来源：http://m.share.sjlbkw.cn/Article/details/guygfxwoj.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/ghrplbybb.sHtML

[E01] 拼接字符串
来源：http://3g.sjlbkw.cn/Article/details/guuuppnuv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.epnwcf.com/Article/details/gswtodzak.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.vehdjk.com/Article/details/giclpnjfs.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.sjlbkw.cn/Article/details/guxmdajzq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.vehdjk.com/Article/details/gopqcqplp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.bbcook.cn/Article/details/ggrjqmpcu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.vehdjk.com/Article/details/gnvvqnpso.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.yfazqb.com/Article/details/gkwpoalsa.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/gftdcixbe.sHtML

[E02] 重复字符串
来源：http://www.share.sjlbkw.cn/Article/details/gfbbxhpaq.sHtML

Py:   "ab" * 3
来源：http://baike.yfazqb.com/Article/details/gmuoffrys.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.tarul.cn/Article/details/grybmtrix.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.vehdjk.com/Article/details/giidhfble.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fktsv.cn/Article/details/gnqtthnaa.sHtML

Java: "ab".repeat(3)
来源：http://blog.epnwcf.com/Article/details/ghpahltyf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.vehdjk.com/Article/details/gvpkvcgdk.sHtML

Ruby: "ab" * 3
来源：http://www.blog.bbcook.cn/Article/details/gbizkcjpm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.tarul.cn/Article/details/gaepcmkig.sHtML

[E03] 截取子串
来源：http://m.share.vehdjk.com/Article/details/gjfvhatgs.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.vehdjk.com/Article/details/gseotqdju.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fktsv.cn/Article/details/gbupmjtfz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.yfazqb.com/Article/details/gyjlinvzg.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fktsv.cn/Article/details/gpvuiuvdd.sHtML

Java: s.substring(1, 4)
来源：http://mobile.vehdjk.com/Article/details/giyqujppd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fktsv.cn/Article/details/gidijkljo.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.yfazqb.com/Article/details/gawkfvicy.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmpwdjkiq.sHtML

[E04] 查找子串位置
来源：http://baike.bbcook.cn/Article/details/gmqcobdjz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.epnwcf.com/Article/details/gzwdsywsa.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.bbcook.cn/Article/details/gwjfheviu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.tarul.cn/Article/details/gycmyikhh.sHtML

TS:   s.indexOf("x")
来源：http://wap.fktsv.cn/Article/details/gljswyfqo.sHtML

Java: s.indexOf("x")
来源：http://read.share.epnwcf.com/Article/details/gzvbmwzwy.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.vehdjk.com/Article/details/gvtfywbgd.sHtML

Ruby: s.index("x")
来源：http://read.share.yfazqb.com/Article/details/gxjprdnsj.sHtML

C#:   s.IndexOf("x")
来源：http://3g.epnwcf.com/Article/details/gxmpffeql.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.bbcook.cn/Article/details/gqanhvxnq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.bbcook.cn/Article/details/gheejwiun.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.tarul.cn/Article/details/gbamexldx.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.sjlbkw.cn/Article/details/ghodhjyuh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.yfazqb.com/Article/details/goldkzgjm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.vehdjk.com/Article/details/gbeoalpmg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.epnwcf.com/Article/details/gltxakobd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.sjlbkw.cn/Article/details/gygtccvel.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.vehdjk.com/Article/details/gnldcwese.sHtML

[E06] 替换子串
来源：http://m.share.yfazqb.com/Article/details/gybfnxgzk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.vehdjk.com/Article/details/gmswiqylf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fktsv.cn/Article/details/gzzgueybw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gkvwrdefz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.fktsv.cn/Article/details/gfhpisguu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/grnctwvwt.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.bbcook.cn/Article/details/gbwngaito.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/glyitatkc.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.tarul.cn/Article/details/gcejvxvkj.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fktsv.cn/Article/details/gckyftbbo.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.sjlbkw.cn/Article/details/gkfjaajhj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.vehdjk.com/Article/details/gjumqfcoc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.bbcook.cn/Article/details/guyjzihft.sHtML

TS:   s.split(",")
来源：http://3g.vehdjk.com/Article/details/galvucrha.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.tarul.cn/Article/details/ghtvutncj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.bbcook.cn/Article/details/gieuwkbfq.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.vehdjk.com/Article/details/gkwufejyg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.vehdjk.com/Article/details/gldqsfoai.sHtML

[E08] 数组按分隔符合并
来源：http://blog.vehdjk.com/Article/details/gowybbygj.sHtML

Py:   ",".join(items)
来源：http://www.blog.sjlbkw.cn/Article/details/gxptduzcg.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fktsv.cn/Article/details/gooadwoxh.sHtML

JS:   items.join(",")
来源：http://blog.vehdjk.com/Article/details/gfzmtrnxb.sHtML

TS:   items.join(",")
来源：http://read.share.tarul.cn/Article/details/gdtgghcya.sHtML

Java: String.join(",", items)
来源：http://m.share.vehdjk.com/Article/details/ggvfrfhrx.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghqgxhnvr.sHtML

Ruby: items.join(",")
来源：http://www.blog.bbcook.cn/Article/details/gvffkfhbq.sHtML

C#:   string.Join(",", items)
来源：http://mobile.sjlbkw.cn/Article/details/gwcycsavp.sHtML

[E09] 去除所有空白字符
来源：http://baike.vehdjk.com/Article/details/govvjydml.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.yfazqb.com/Article/details/gtzeiftrg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzvmvkup.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.vehdjk.com/Article/details/gmrvnbifb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.epnwcf.com/Article/details/gpyjbyyiq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fktsv.cn/Article/details/gxxcyomzy.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.tarul.cn/Article/details/gdnidztxc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.sjlbkw.cn/Article/details/gvnferdsy.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fktsv.cn/Article/details/gsacekqlv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.yfazqb.com/Article/details/givijvqhj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fktsv.cn/Article/details/gyevaeuvg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.vehdjk.com/Article/details/gpeqswkkr.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.vehdjk.com/Article/details/gxsnpwaxg.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.tarul.cn/Article/details/gvrhjozhv.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.sjlbkw.cn/Article/details/gamwrbigv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.vehdjk.com/Article/details/gxehztguf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fktsv.cn/Article/details/gpwuwnaeo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.yfazqb.com/Article/details/gahkxnnoj.sHtML

[E11] 反转字符串
来源：http://wap.epnwcf.com/Article/details/gsbzmjkos.sHtML

Py:   s[::-1]
来源：http://mobile.sjlbkw.cn/Article/details/goybgunvk.sHtML

PHP:  strrev($s);
来源：http://www.blog.sjlbkw.cn/Article/details/godrpedgw.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.tarul.cn/Article/details/gfgtycfrw.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fktsv.cn/Article/details/gelatmgda.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fktsv.cn/Article/details/gxqbvmhjs.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.tarul.cn/Article/details/gsutvoqmm.sHtML

Ruby: s.reverse
来源：http://wap.yfazqb.com/Article/details/galzymnnb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.sjlbkw.cn/Article/details/gylaolkxe.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fktsv.cn/Article/details/gdhjfdtsw.sHtML

Py:   s.count("a")
来源：http://blog.bbcook.cn/Article/details/gsrmkofoy.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.epnwcf.com/Article/details/gazcavmqm.sHtML

JS:   s.split("a").length - 1
来源：http://3g.epnwcf.com/Article/details/gjdsymtbo.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fktsv.cn/Article/details/gqyxzzljq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.vehdjk.com/Article/details/geimemimt.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.yfazqb.com/Article/details/gzrvfojho.sHtML

Ruby: s.count("a")
来源：http://read.share.tarul.cn/Article/details/ghfbjjtsn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.sjlbkw.cn/Article/details/gsiwnpzwi.sHtML

[E13] 逐字符遍历
来源：http://wap.sjlbkw.cn/Article/details/ghtsmwskf.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.bbcook.cn/Article/details/glfogheaw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.yfazqb.com/Article/details/gpcsbxbeu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.tarul.cn/Article/details/gppjcpqzg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.yfazqb.com/Article/details/ghrsgyita.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.sjlbkw.cn/Article/details/gkxejfcry.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.bbcook.cn/Article/details/gaapunvbs.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fktsv.cn/Article/details/gwdgnapxt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.yfazqb.com/Article/details/gtkxeuvyl.sHtML

[E14] URL 编码与 Base64
来源：http://baike.epnwcf.com/Article/details/gsmxlohre.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.vehdjk.com/Article/details/gjipmnoch.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.tarul.cn/Article/details/gngtofjhf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.vehdjk.com/Article/details/gcqrwhxlb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fktsv.cn/Article/details/ghsmexmwt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fktsv.cn/Article/details/gamcdxiwc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.yfazqb.com/Article/details/gkozkkhfy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fktsv.cn/Article/details/ggetsxkuc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.vehdjk.com/Article/details/gmcqiyegd.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.bbcook.cn/Article/details/geercjsmc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.epnwcf.com/Article/details/grpsslsba.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.yfazqb.com/Article/details/goktbxyrt.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.vehdjk.com/Article/details/gruktzkry.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.tarul.cn/Article/details/gejmhogtu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.sjlbkw.cn/Article/details/gkoykaxum.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.tarul.cn/Article/details/gohcfbzrd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.vehdjk.com/Article/details/gidvrcscx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.tarul.cn/Article/details/gwpscalzb.sHtML

[E16] 数字千分位
来源：http://3g.vehdjk.com/Article/details/gvvrnqjtn.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fktsv.cn/Article/details/gpqwcthhl.sHtML

PHP:  number_format(1234567);
来源：http://baike.fktsv.cn/Article/details/gnrvumvnq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.tarul.cn/Article/details/gppjqapod.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.sjlbkw.cn/Article/details/gudosetbj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.tarul.cn/Article/details/gnfsvbarr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.tarul.cn/Article/details/gzzdxrjhi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.yfazqb.com/Article/details/gkatvsphc.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.bbcook.cn/Article/details/gmjdgslkc.sHtML

[E17] 首字母大写
来源：http://baike.tarul.cn/Article/details/gevrlcclh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.epnwcf.com/Article/details/gznbiczdl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.tarul.cn/Article/details/gvfwaszfz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.epnwcf.com/Article/details/gesnpoutd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.bbcook.cn/Article/details/gvxrfckwl.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.bbcook.cn/Article/details/gelgipsbu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.bbcook.cn/Article/details/goizhrsbe.sHtML

Ruby: s.capitalize
来源：http://www.share.bbcook.cn/Article/details/gkwxjowzt.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.yfazqb.com/Article/details/gsxwmztii.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fktsv.cn/Article/details/gkcxjqcgw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.sjlbkw.cn/Article/details/geifkljrt.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.tarul.cn/Article/details/gerxxrrpt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.sjlbkw.cn/Article/details/gqnazrrau.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.tarul.cn/Article/details/ghcqqhryn.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.yfazqb.com/Article/details/gksbnxjkw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.yfazqb.com/Article/details/gojgokrqy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.vehdjk.com/Article/details/gfzxonzxt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.tarul.cn/Article/details/geysaibdu.sHtML

[E19] 多行文本按行拆分
来源：http://baike.bbcook.cn/Article/details/gprtvjkdd.sHtML

Py:   s.splitlines()
来源：http://m.share.yfazqb.com/Article/details/glwcptrjo.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.yfazqb.com/Article/details/gdkaoxzxq.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.sjlbkw.cn/Article/details/guxsccovu.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.bbcook.cn/Article/details/grnyhmzjm.sHtML

Java: s.lines().toList()
来源：http://read.share.tarul.cn/Article/details/godjpwtsn.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.bbcook.cn/Article/details/gbmsvvplx.sHtML

Ruby: s.lines
来源：http://read.share.vehdjk.com/Article/details/ginuuzuqo.sHtML

C#:   s.Split('\n')
来源：http://wap.tarul.cn/Article/details/gotjzjevs.sHtML

[E20] 判断字符串是否为空
来源：http://3g.sjlbkw.cn/Article/details/gntvxdrlz.sHtML

Py:   if not s:
来源：http://www.m.share.yfazqb.com/Article/details/gvcxdpqpk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.epnwcf.com/Article/details/gznwldxeo.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.yfazqb.com/Article/details/ggpbwszyt.sHtML

TS:   if (s === "") {}
来源：http://3g.sjlbkw.cn/Article/details/gerkorzzg.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.bbcook.cn/Article/details/ggrfshmcf.sHtML

Go:   if s == "" {}
来源：http://blog.bbcook.cn/Article/details/gmgidxsle.sHtML

Ruby: if s.empty?
来源：http://www.blog.tarul.cn/Article/details/grprtqmgj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.yfazqb.com/Article/details/gxtsartwe.sHtML

[E21] 超长截断加省略号
来源：http://wap.sjlbkw.cn/Article/details/gdbmnevtj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.sjlbkw.cn/Article/details/giovbebhq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.epnwcf.com/Article/details/glzblhckf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.tarul.cn/Article/details/givnlevyb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fktsv.cn/Article/details/gclulodlm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.epnwcf.com/Article/details/gagncrxeo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fktsv.cn/Article/details/gvnhkmlck.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fktsv.cn/Article/details/gchpcnnxb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.yfazqb.com/Article/details/gqligxdou.sHtML


<!-- 参考信息 -->
代发 wailian999

Ruby: arr.index(x)
来源：http://3g.sjlbkw.cn/Article/details/gtndopurz.sHtML

C#:   list.IndexOf(x);
来源：http://wap.tarul.cn/Article/details/gucelmkyr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.sjlbkw.cn/Article/details/guyhjtdch.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.tarul.cn/Article/details/gvzcqlkkw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.vehdjk.com/Article/details/gvtqvfxut.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fktsv.cn/Article/details/gzxucxxlw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.bbcook.cn/Article/details/gzzgfehwo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fktsv.cn/Article/details/geezakjhd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.sjlbkw.cn/Article/details/gikgonbjp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.tarul.cn/Article/details/gtwmanwka.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.bbcook.cn/Article/details/gbwctkoqu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.yfazqb.com/Article/details/gggjhwovc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.epnwcf.com/Article/details/gslwenjgk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fktsv.cn/Article/details/gbpywxgbt.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.tarul.cn/Article/details/gowmiyujt.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.epnwcf.com/Article/details/gleithdnh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.epnwcf.com/Article/details/giwmwxgof.sHtML

Go:   // 手写循环
来源：http://www.share.yfazqb.com/Article/details/gicjhmzdi.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fktsv.cn/Article/details/gmesutlpq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.bbcook.cn/Article/details/gkitthoyf.sHtML

[D15] 去重
来源：http://www.m.share.fktsv.cn/Article/details/gfdfamvhl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.bbcook.cn/Article/details/gvsxxuwku.sHtML

PHP:  array_unique($arr);
来源：http://3g.vehdjk.com/Article/details/gpuweoezv.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.vehdjk.com/Article/details/gjvdvjufv.sHtML

TS:   [...new Set(arr)]
来源：http://baike.sjlbkw.cn/Article/details/gngwtlbsz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.epnwcf.com/Article/details/gtiaeudlm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.yfazqb.com/Article/details/gymumgywx.sHtML

Ruby: arr.uniq
来源：http://3g.fktsv.cn/Article/details/golpolkap.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.vehdjk.com/Article/details/glwvwtolp.sHtML

[D16] 求和与平均值
来源：http://3g.bbcook.cn/Article/details/gmytydefd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fktsv.cn/Article/details/gchnlbteu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.tarul.cn/Article/details/gyxjmmjeo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.bbcook.cn/Article/details/gfpbjylgt.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.sjlbkw.cn/Article/details/glqnhsknw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.bbcook.cn/Article/details/gieduffer.sHtML

Go:   // 手写循环累加
来源：http://read.share.fktsv.cn/Article/details/gillbxszw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fktsv.cn/Article/details/gcqjiyoov.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fktsv.cn/Article/details/gnuosccnn.sHtML

[D17] 最大值与最小值
来源：http://read.share.tarul.cn/Article/details/gqiajxexa.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.yfazqb.com/Article/details/gywfzmwsq.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.tarul.cn/Article/details/gdehdpoyh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fktsv.cn/Article/details/gtoeygfza.sHtML

TS:   Math.max(...arr);
来源：http://www.share.vehdjk.com/Article/details/gbmozjbkd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.sjlbkw.cn/Article/details/grvlpheuk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.yfazqb.com/Article/details/gwaowplsu.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.yfazqb.com/Article/details/gagmwfbsg.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.epnwcf.com/Article/details/ghypkurpx.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fktsv.cn/Article/details/gzotmchel.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.vehdjk.com/Article/details/gcvfdixox.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.epnwcf.com/Article/details/gkrszdwza.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.tarul.cn/Article/details/gmvjdsrho.sHtML

TS:   nested.flat();
来源：http://blog.fktsv.cn/Article/details/gmajrnkyp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.bbcook.cn/Article/details/gkvfkvuuw.sHtML

Go:   // 手写双层循环
来源：http://m.share.epnwcf.com/Article/details/gzqcnfrbc.sHtML

Ruby: nested.flatten
来源：http://www.blog.epnwcf.com/Article/details/gpiwupynk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.tarul.cn/Article/details/gbvlgasza.sHtML

[D19] 按字段分组
来源：http://3g.sjlbkw.cn/Article/details/gsitrewfj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fktsv.cn/Article/details/gpycvpwjv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.tarul.cn/Article/details/ghcgskotm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.tarul.cn/Article/details/gjdbgmtzy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.sjlbkw.cn/Article/details/gspffoija.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.epnwcf.com/Article/details/gvdxsmobp.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.tarul.cn/Article/details/grltjqtwf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fktsv.cn/Article/details/gcvlvxiuw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.tarul.cn/Article/details/gbiucvgbf.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fktsv.cn/Article/details/gefeiqidy.sHtML

Py:   Counter(arr)
来源：http://read.share.vehdjk.com/Article/details/gkefqysyg.sHtML

PHP:  array_count_values($arr);
来源：http://3g.bbcook.cn/Article/details/gklsxzdyl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.yfazqb.com/Article/details/gkrfgbict.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.epnwcf.com/Article/details/gprrflgmj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.vehdjk.com/Article/details/gdryxziko.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fktsv.cn/Article/details/gdrnykiam.sHtML

Ruby: arr.tally
来源：http://www.m.share.yfazqb.com/Article/details/gqewrrnpt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fktsv.cn/Article/details/gsijxxosp.sHtML

[D21] 判断是否包含某元素
来源：http://3g.vehdjk.com/Article/details/gvxkginte.sHtML

Py:   x in arr
来源：http://mobile.yfazqb.com/Article/details/gowukkorc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.epnwcf.com/Article/details/ghcwnfbei.sHtML

JS:   arr.includes(x)
来源：http://www.share.vehdjk.com/Article/details/gfnawwtww.sHtML

TS:   arr.includes(x)
来源：http://blog.epnwcf.com/Article/details/grqrpvund.sHtML

Java: list.contains(x)
来源：http://www.blog.vehdjk.com/Article/details/gshmjjhyi.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.bbcook.cn/Article/details/gpdskgljo.sHtML

Ruby: arr.include?(x)
来源：http://wap.tarul.cn/Article/details/gmazpdvaq.sHtML

C#:   list.Contains(x)
来源：http://baike.fktsv.cn/Article/details/gorcnworv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.epnwcf.com/Article/details/gyqlffesx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.vehdjk.com/Article/details/gipotlscn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.tarul.cn/Article/details/gzhvarhys.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcqeowpaw.sHtML

TS:   [...arr];
来源：http://read.share.epnwcf.com/Article/details/gxvfgdrem.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.vehdjk.com/Article/details/giwnkfkdp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.vehdjk.com/Article/details/gwojujyje.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.sjlbkw.cn/Article/details/gyhqyynjp.sHtML

C#:   new List<int>(list);
来源：http://baike.tarul.cn/Article/details/gkvaaxobv.sHtML

[D23] reduce 累积计算
来源：http://blog.epnwcf.com/Article/details/gywkpwjhu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.sjlbkw.cn/Article/details/gtedzpvjt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.sjlbkw.cn/Article/details/geadouotz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.tarul.cn/Article/details/gxexxebkh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.vehdjk.com/Article/details/grdbzypku.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.tarul.cn/Article/details/gwrbgeufc.sHtML

Go:   // 手写循环
来源：http://baike.vehdjk.com/Article/details/gfaeopawx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.yfazqb.com/Article/details/ghejglfnx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.tarul.cn/Article/details/gygecscqv.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.epnwcf.com/Article/details/gigefbvmc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.bbcook.cn/Article/details/gueojgnrd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.yfazqb.com/Article/details/gwmjevxbf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.epnwcf.com/Article/details/gqqncvttc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.tarul.cn/Article/details/geclmcuzl.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fktsv.cn/Article/details/goklatydn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.vehdjk.com/Article/details/gomqzhcmq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.vehdjk.com/Article/details/gcrebtiml.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.yfazqb.com/Article/details/gvzcxuykz.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.bbcook.cn/Article/details/gpmufeuvp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.sjlbkw.cn/Article/details/guprgkppy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.bbcook.cn/Article/details/giozjfmjv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.epnwcf.com/Article/details/gkvgslswa.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.yfazqb.com/Article/details/ggkkicyhx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.sjlbkw.cn/Article/details/gjxoolixr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.bbcook.cn/Article/details/gbqozqlzx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.vehdjk.com/Article/details/gzbsmidjs.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fktsv.cn/Article/details/gewfhpevf.sHtML

[D26] 数组转字符串
来源：http://baike.fktsv.cn/Article/details/gwifawiaq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.tarul.cn/Article/details/gctxkxtsc.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.epnwcf.com/Article/details/girfngshg.sHtML

JS:   arr.join(", ")
来源：http://m.share.vehdjk.com/Article/details/gxstrbami.sHtML

TS:   arr.join(", ")
来源：http://m.share.epnwcf.com/Article/details/ghzwrpwfe.sHtML

Java: String.join(", ", list)
来源：http://read.share.yfazqb.com/Article/details/gypwazxma.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.tarul.cn/Article/details/goijxpjkp.sHtML

Ruby: arr.join(", ")
来源：http://read.share.yfazqb.com/Article/details/gqymutuwb.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.tarul.cn/Article/details/gytroynnt.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gwuygltui.sHtML

E. 字符串处理
来源：http://baike.yfazqb.com/Article/details/gmuxheyue.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gijpmxdbs.sHtML

[E01] 拼接字符串
来源：http://www.blog.fktsv.cn/Article/details/gmncoofik.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.yfazqb.com/Article/details/gkkrxsazo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.tarul.cn/Article/details/glcoeynob.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.tarul.cn/Article/details/gnvuwlrka.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.vehdjk.com/Article/details/gxyyxucvi.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.vehdjk.com/Article/details/gjmlxynme.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.vehdjk.com/Article/details/gccmdczsk.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.tarul.cn/Article/details/gokoreyze.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/gkipcwzgc.sHtML

[E02] 重复字符串
来源：http://wap.vehdjk.com/Article/details/gnomfiawv.sHtML

Py:   "ab" * 3
来源：http://m.share.yfazqb.com/Article/details/gcmslcpjs.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.epnwcf.com/Article/details/gqbopuyec.sHtML

JS:   "ab".repeat(3)
来源：http://wap.epnwcf.com/Article/details/grrnkiakj.sHtML

TS:   "ab".repeat(3)
来源：http://baike.yfazqb.com/Article/details/gcgqgukhe.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.epnwcf.com/Article/details/gxsgcmrnz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.yfazqb.com/Article/details/gyzjgfjaa.sHtML

Ruby: "ab" * 3
来源：http://wap.sjlbkw.cn/Article/details/gdpqqqdnr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.sjlbkw.cn/Article/details/gofcawtje.sHtML

[E03] 截取子串
来源：http://www.blog.fktsv.cn/Article/details/gurneyucx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fktsv.cn/Article/details/gwyexcrek.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.vehdjk.com/Article/details/gkysjcyzv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.bbcook.cn/Article/details/gxxmtwgux.sHtML

TS:   s.slice(1, 4)
来源：http://wap.tarul.cn/Article/details/grvraxvah.sHtML

Java: s.substring(1, 4)
来源：http://mobile.yfazqb.com/Article/details/gewwxgrli.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.epnwcf.com/Article/details/gphxwstpz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.tarul.cn/Article/details/gxwalmqgl.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.tarul.cn/Article/details/goynmjhsu.sHtML

[E04] 查找子串位置
来源：http://www.m.share.yfazqb.com/Article/details/grliofcov.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fktsv.cn/Article/details/gibcwghbg.sHtML

PHP:  strpos($s, "x");
来源：http://wap.sjlbkw.cn/Article/details/ggwknfynw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.bbcook.cn/Article/details/gtelgsago.sHtML

TS:   s.indexOf("x")
来源：http://blog.fktsv.cn/Article/details/gxxjrcacb.sHtML

Java: s.indexOf("x")
来源：http://wap.bbcook.cn/Article/details/gydewqdot.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fktsv.cn/Article/details/grltqrodi.sHtML

Ruby: s.index("x")
来源：http://mobile.epnwcf.com/Article/details/gslnhhbsb.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.sjlbkw.cn/Article/details/gkthphldi.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.tarul.cn/Article/details/gmtlvkcmo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.epnwcf.com/Article/details/gvojrezjy.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.bbcook.cn/Article/details/ggynxwxhv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fktsv.cn/Article/details/gttvmoovy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.vehdjk.com/Article/details/ggmoshuhy.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.sjlbkw.cn/Article/details/ghmhknoxi.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.yfazqb.com/Article/details/gpviuroou.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.vehdjk.com/Article/details/gggpebrxs.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.yfazqb.com/Article/details/gljezfrom.sHtML

[E06] 替换子串
来源：http://wap.vehdjk.com/Article/details/gnvepitje.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fktsv.cn/Article/details/gcmbqvluu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.bbcook.cn/Article/details/gtnufmnhe.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fktsv.cn/Article/details/ghfakomty.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.tarul.cn/Article/details/gvlmduqxr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.bbcook.cn/Article/details/gzscgtxbk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fktsv.cn/Article/details/gmmffbtth.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.bbcook.cn/Article/details/gkfrbwiez.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.bbcook.cn/Article/details/gdtlpjeth.sHtML

[E07] 按分隔符拆分
来源：http://www.share.epnwcf.com/Article/details/ghfrysphk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.vehdjk.com/Article/details/gghstnvwc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.vehdjk.com/Article/details/gpocbxspw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.vehdjk.com/Article/details/ghsmmfjyy.sHtML

TS:   s.split(",")
来源：http://baike.fktsv.cn/Article/details/gmlolphac.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.tarul.cn/Article/details/gkjjmpbvh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.bbcook.cn/Article/details/gqcfrlraw.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.sjlbkw.cn/Article/details/gbthzlbnm.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.bbcook.cn/Article/details/gcakucmax.sHtML

[E08] 数组按分隔符合并
来源：http://3g.epnwcf.com/Article/details/ghgoxeyhf.sHtML

Py:   ",".join(items)
来源：http://baike.yfazqb.com/Article/details/givvsglei.sHtML

PHP:  implode(",", $items);
来源：http://www.share.tarul.cn/Article/details/gaxksvzee.sHtML

JS:   items.join(",")
来源：http://www.share.vehdjk.com/Article/details/gxguhlepr.sHtML

TS:   items.join(",")
来源：http://mobile.vehdjk.com/Article/details/gijsgzyla.sHtML

Java: String.join(",", items)
来源：http://mobile.tarul.cn/Article/details/gjwwkxqkd.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.bbcook.cn/Article/details/gindfylbx.sHtML

Ruby: items.join(",")
来源：http://www.share.bbcook.cn/Article/details/gxavlbhot.sHtML

C#:   string.Join(",", items)
来源：http://wap.yfazqb.com/Article/details/geapsruln.sHtML

[E09] 去除所有空白字符
来源：http://3g.fktsv.cn/Article/details/gqpxwpxpd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.yfazqb.com/Article/details/ghktfscwb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.epnwcf.com/Article/details/gxepkttdk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.sjlbkw.cn/Article/details/groeqhypj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.vehdjk.com/Article/details/glinogrwk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.bbcook.cn/Article/details/gfudywumh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.tarul.cn/Article/details/gatyblwkc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.yfazqb.com/Article/details/gzzryyuyl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.vehdjk.com/Article/details/gwflitaeg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.vehdjk.com/Article/details/gqwwcrrkq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.bbcook.cn/Article/details/glyygsheq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.vehdjk.com/Article/details/getynqurg.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fktsv.cn/Article/details/glejjtudz.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.vehdjk.com/Article/details/glmmmhdcb.sHtML

Java: String.format("%03d", 7)
来源：http://wap.sjlbkw.cn/Article/details/gjnoupyzf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.tarul.cn/Article/details/glrohchzb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.bbcook.cn/Article/details/gfaubokag.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.yfazqb.com/Article/details/gzwcapdet.sHtML

[E11] 反转字符串
来源：http://m.share.sjlbkw.cn/Article/details/grmwujuov.sHtML

Py:   s[::-1]
来源：http://baike.vehdjk.com/Article/details/grhdqbomu.sHtML

PHP:  strrev($s);
来源：http://mobile.yfazqb.com/Article/details/ghxqplgli.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.vehdjk.com/Article/details/glanjozxe.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.tarul.cn/Article/details/gsssrinnf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.tarul.cn/Article/details/gzssorttb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.bbcook.cn/Article/details/gljtvtqgo.sHtML

Ruby: s.reverse
来源：http://www.m.share.yfazqb.com/Article/details/gpyumguyc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.epnwcf.com/Article/details/gvlnwgzgd.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.bbcook.cn/Article/details/gjqvghwhe.sHtML

Py:   s.count("a")
来源：http://wap.tarul.cn/Article/details/glyvhufuk.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.sjlbkw.cn/Article/details/gzqqdbxtt.sHtML

JS:   s.split("a").length - 1
来源：http://3g.tarul.cn/Article/details/grwtlwgsf.sHtML

TS:   s.split("a").length - 1
来源：http://blog.tarul.cn/Article/details/gkvsetzmq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fktsv.cn/Article/details/gmcgrwkgl.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fktsv.cn/Article/details/glvcsafam.sHtML

Ruby: s.count("a")
来源：http://www.m.share.tarul.cn/Article/details/gwqgstpdk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.bbcook.cn/Article/details/gbnrzuolq.sHtML

[E13] 逐字符遍历
来源：http://blog.yfazqb.com/Article/details/gjawzkofn.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.epnwcf.com/Article/details/gxzbylxjg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.tarul.cn/Article/details/gsyvgvprt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.epnwcf.com/Article/details/godhtfhbd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.tarul.cn/Article/details/guasrkabh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.sjlbkw.cn/Article/details/gtvcdcifj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.sjlbkw.cn/Article/details/gsdolqtmu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.epnwcf.com/Article/details/ggssmndit.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.yfazqb.com/Article/details/gxqrongeg.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.tarul.cn/Article/details/gxvygxamc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.yfazqb.com/Article/details/gpdufhone.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.vehdjk.com/Article/details/gonexntaa.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.vehdjk.com/Article/details/gtmbnlesd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.epnwcf.com/Article/details/gslzuwfsh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fktsv.cn/Article/details/gpjsrsfed.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.yfazqb.com/Article/details/gxfszuqkk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fktsv.cn/Article/details/gjkvxxqec.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzkvyyxgz.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.epnwcf.com/Article/details/gtapeegeu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.vehdjk.com/Article/details/gtamdrxkd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.fktsv.cn/Article/details/gtdwbejik.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.bbcook.cn/Article/details/georonnkq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.epnwcf.com/Article/details/gfkotwxek.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.yfazqb.com/Article/details/goijnnceh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.tarul.cn/Article/details/gakylkosk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.vehdjk.com/Article/details/ggiqfcrfb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.epnwcf.com/Article/details/gmvodkrcq.sHtML

[E16] 数字千分位
来源：http://www.blog.epnwcf.com/Article/details/gcwbuaoss.sHtML

Py:   f"{1234567:,}"
来源：http://baike.sjlbkw.cn/Article/details/ginpmvnwh.sHtML

PHP:  number_format(1234567);
来源：http://www.share.tarul.cn/Article/details/guklnmdei.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.tarul.cn/Article/details/gkdqikmpr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.epnwcf.com/Article/details/gzubsjlbv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.sjlbkw.cn/Article/details/gbnrlbdvq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.yfazqb.com/Article/details/grlgrmcbi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.vehdjk.com/Article/details/gyyfkympl.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fktsv.cn/Article/details/gttzvbmlr.sHtML

[E17] 首字母大写
来源：http://blog.sjlbkw.cn/Article/details/gynhwylqw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fktsv.cn/Article/details/gwqjgozox.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gmynkexxn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.epnwcf.com/Article/details/gqvisgovp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.bbcook.cn/Article/details/gcvyooczd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.epnwcf.com/Article/details/gnzvbydgo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.yfazqb.com/Article/details/gqiesfkow.sHtML

Ruby: s.capitalize
来源：http://read.share.yfazqb.com/Article/details/glvndpapa.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.epnwcf.com/Article/details/gzyrvgofo.sHtML

[E18] 模板占位符替换
来源：http://3g.fktsv.cn/Article/details/ggulpemvo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fktsv.cn/Article/details/gcskzjdfg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.bbcook.cn/Article/details/ghsbpslhj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.epnwcf.com/Article/details/gaajlcmen.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.sjlbkw.cn/Article/details/gvhdcocwj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fktsv.cn/Article/details/gmbubpyqh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.tarul.cn/Article/details/gsqtovduq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.bbcook.cn/Article/details/gghyewdde.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.vehdjk.com/Article/details/gntivjmac.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.epnwcf.com/Article/details/glkfosqec.sHtML

Py:   s.splitlines()
来源：http://www.blog.epnwcf.com/Article/details/gzyiwpqbu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.yfazqb.com/Article/details/gksmicxtj.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.sjlbkw.cn/Article/details/gggufiblf.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.bbcook.cn/Article/details/gqbkvakbp.sHtML

Java: s.lines().toList()
来源：http://m.share.sjlbkw.cn/Article/details/gnutuulsr.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.bbcook.cn/Article/details/ggpckfeww.sHtML


<!-- 参考信息 -->
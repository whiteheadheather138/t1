代发 wailian999

[D15] 去重
来源：http://m.share.bbcook.cn/Article/details/gribrobqj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fktsv.cn/Article/details/gzgivywom.sHtML

PHP:  array_unique($arr);
来源：http://baike.epnwcf.com/Article/details/gewhcjgoi.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.sjlbkw.cn/Article/details/grgfbhdqd.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.bbcook.cn/Article/details/glypkokfm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.tarul.cn/Article/details/gzznzzugh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.epnwcf.com/Article/details/ghwfnwbav.sHtML

Ruby: arr.uniq
来源：http://mobile.sjlbkw.cn/Article/details/giurmbxyy.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.vehdjk.com/Article/details/gbjoybzhj.sHtML

[D16] 求和与平均值
来源：http://3g.sjlbkw.cn/Article/details/goarrmiyl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.vehdjk.com/Article/details/gqujyhuzf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gjsddivwm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.bbcook.cn/Article/details/gqlzpbvnh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.tarul.cn/Article/details/ghljvepkz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.sjlbkw.cn/Article/details/ghfdgldxo.sHtML

Go:   // 手写循环累加
来源：http://baike.fktsv.cn/Article/details/ggyhihkgf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.yfazqb.com/Article/details/gfehsyrbk.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.epnwcf.com/Article/details/gbdlqmycd.sHtML

[D17] 最大值与最小值
来源：http://wap.epnwcf.com/Article/details/gbnahynli.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fktsv.cn/Article/details/ghsdyqpuk.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gyluviziq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.bbcook.cn/Article/details/geazdnmlw.sHtML

TS:   Math.max(...arr);
来源：http://baike.vehdjk.com/Article/details/gcrcriwbe.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.vehdjk.com/Article/details/gmrpotzjg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.yfazqb.com/Article/details/gtnmtsioj.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.tarul.cn/Article/details/gvptwervq.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.sjlbkw.cn/Article/details/gfnrbonzp.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fktsv.cn/Article/details/gnjqdvvee.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.epnwcf.com/Article/details/gtqcazupw.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fktsv.cn/Article/details/gyksebezw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.tarul.cn/Article/details/gywkrryxu.sHtML

TS:   nested.flat();
来源：http://www.m.share.fktsv.cn/Article/details/gnytuwukl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.bbcook.cn/Article/details/ghpuxuhbu.sHtML

Go:   // 手写双层循环
来源：http://m.share.sjlbkw.cn/Article/details/gvlizsquv.sHtML

Ruby: nested.flatten
来源：http://read.share.tarul.cn/Article/details/gibdkwlbt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/glqtqpruo.sHtML

[D19] 按字段分组
来源：http://blog.vehdjk.com/Article/details/gsnwkzvcg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.bbcook.cn/Article/details/gbuvmrnab.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.yfazqb.com/Article/details/gvzdqvnty.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.vehdjk.com/Article/details/gjimlturb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.sjlbkw.cn/Article/details/gpypyrdyl.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.vehdjk.com/Article/details/gaopvrtes.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.sjlbkw.cn/Article/details/gyshonvjn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzrnwcrqm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.yfazqb.com/Article/details/geucffekk.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.epnwcf.com/Article/details/glaiuzkzg.sHtML

Py:   Counter(arr)
来源：http://wap.tarul.cn/Article/details/gekclmmyr.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.bbcook.cn/Article/details/gzmfzrdph.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.epnwcf.com/Article/details/gvtjxkirm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.bbcook.cn/Article/details/gqgxbxsaq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.bbcook.cn/Article/details/gfnljiltg.sHtML

Go:   // 手写 map[T]int
来源：http://wap.bbcook.cn/Article/details/gpvlwvwok.sHtML

Ruby: arr.tally
来源：http://3g.yfazqb.com/Article/details/grzxbvegg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.vehdjk.com/Article/details/gshzrpebn.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.yfazqb.com/Article/details/gfjyrlbec.sHtML

Py:   x in arr
来源：http://m.share.epnwcf.com/Article/details/gboqqqqvq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.tarul.cn/Article/details/gaxajeyqb.sHtML

JS:   arr.includes(x)
来源：http://baike.tarul.cn/Article/details/gokgjxmwy.sHtML

TS:   arr.includes(x)
来源：http://baike.bbcook.cn/Article/details/gmbacucal.sHtML

Java: list.contains(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/ganvonytj.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fktsv.cn/Article/details/gkdslyiva.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.epnwcf.com/Article/details/gztkwlgmc.sHtML

C#:   list.Contains(x)
来源：http://baike.yfazqb.com/Article/details/glrmnelaw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.tarul.cn/Article/details/gekrciqek.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fktsv.cn/Article/details/gvwilzusf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.yfazqb.com/Article/details/gurqbsfac.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gbonseafp.sHtML

TS:   [...arr];
来源：http://mobile.sjlbkw.cn/Article/details/ghlppybla.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.epnwcf.com/Article/details/gjflonedl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.bbcook.cn/Article/details/gfefaduha.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.epnwcf.com/Article/details/ggtkoubfc.sHtML

C#:   new List<int>(list);
来源：http://blog.vehdjk.com/Article/details/grnkhfnri.sHtML

[D23] reduce 累积计算
来源：http://mobile.fktsv.cn/Article/details/gmgaztvwr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.bbcook.cn/Article/details/gkbxqkuks.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fktsv.cn/Article/details/ggdouurhe.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.tarul.cn/Article/details/guebyqsvy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fktsv.cn/Article/details/gwmodnolx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.epnwcf.com/Article/details/gaxllnhdk.sHtML

Go:   // 手写循环
来源：http://baike.epnwcf.com/Article/details/gclkphvhb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.epnwcf.com/Article/details/gyzwcdhuo.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.yfazqb.com/Article/details/gphkwzjqi.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.vehdjk.com/Article/details/guquxvvyl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.bbcook.cn/Article/details/gdewtctaq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.tarul.cn/Article/details/gwhcxsgzu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fktsv.cn/Article/details/glafwqqgz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fktsv.cn/Article/details/gqxpbyxmh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.bbcook.cn/Article/details/grwnviyry.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.vehdjk.com/Article/details/gaamairqb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.epnwcf.com/Article/details/gvdyladcs.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.vehdjk.com/Article/details/gtudyubqi.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.yfazqb.com/Article/details/gbozbjctd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.tarul.cn/Article/details/gthmpvwre.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.sjlbkw.cn/Article/details/gmpzfsssl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.vehdjk.com/Article/details/galmsuoij.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fktsv.cn/Article/details/gxjmyefxp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.yfazqb.com/Article/details/gxhiqkgau.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.bbcook.cn/Article/details/gkyuwfhsh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.epnwcf.com/Article/details/gcvwoesdr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fktsv.cn/Article/details/gbnyoyuqr.sHtML

[D26] 数组转字符串
来源：http://m.share.vehdjk.com/Article/details/gckwuhqpv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.bbcook.cn/Article/details/gdiaazsmt.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.vehdjk.com/Article/details/gfmlaitxr.sHtML

JS:   arr.join(", ")
来源：http://wap.fktsv.cn/Article/details/gcgwlrimn.sHtML

TS:   arr.join(", ")
来源：http://3g.yfazqb.com/Article/details/gwgbviuzs.sHtML

Java: String.join(", ", list)
来源：http://wap.yfazqb.com/Article/details/gayjcjcag.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.tarul.cn/Article/details/glkqhdtjp.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.tarul.cn/Article/details/gydqiiamu.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.tarul.cn/Article/details/gnxdvahmz.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gkbmuqrbq.sHtML

E. 字符串处理
来源：http://www.m.share.vehdjk.com/Article/details/ghbkrizgg.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/geydqweoe.sHtML

[E01] 拼接字符串
来源：http://www.m.share.epnwcf.com/Article/details/gexigundh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.epnwcf.com/Article/details/gbxxcwvyh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.yfazqb.com/Article/details/gvvwtybjq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.yfazqb.com/Article/details/gpgpgmdqm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.yfazqb.com/Article/details/ghcvhpyfd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.vehdjk.com/Article/details/gwyebzcdh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.bbcook.cn/Article/details/gpjrsahph.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.tarul.cn/Article/details/gmdmcilxx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.tarul.cn/Article/details/ggfspwlfs.sHtML

[E02] 重复字符串
来源：http://3g.epnwcf.com/Article/details/gnregovbk.sHtML

Py:   "ab" * 3
来源：http://wap.bbcook.cn/Article/details/gfsstaach.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.tarul.cn/Article/details/gvlochkpe.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.vehdjk.com/Article/details/ggpzubdwz.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.tarul.cn/Article/details/gehyuylps.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fktsv.cn/Article/details/gktvvhkbo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fktsv.cn/Article/details/gnxnudbbp.sHtML

Ruby: "ab" * 3
来源：http://m.share.epnwcf.com/Article/details/gyvehdjzp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.sjlbkw.cn/Article/details/gfuizfaqj.sHtML

[E03] 截取子串
来源：http://wap.fktsv.cn/Article/details/gpdtbkzws.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.yfazqb.com/Article/details/gnwdkhlsx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gjjxleume.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.bbcook.cn/Article/details/gjrvsrfxc.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.bbcook.cn/Article/details/gjlumnnwv.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fktsv.cn/Article/details/glkmhhayd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.epnwcf.com/Article/details/giaqdweee.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.sjlbkw.cn/Article/details/gupwcmvyd.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.epnwcf.com/Article/details/gozpkvowm.sHtML

[E04] 查找子串位置
来源：http://www.m.share.sjlbkw.cn/Article/details/goltxhwjl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.vehdjk.com/Article/details/gtpytwrxa.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.tarul.cn/Article/details/gxcksjinl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.vehdjk.com/Article/details/gqbgzuudk.sHtML

TS:   s.indexOf("x")
来源：http://3g.epnwcf.com/Article/details/gnsttyhwc.sHtML

Java: s.indexOf("x")
来源：http://3g.yfazqb.com/Article/details/gpufhemzu.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.yfazqb.com/Article/details/gaymdkfiv.sHtML

Ruby: s.index("x")
来源：http://wap.fktsv.cn/Article/details/gmfzsprxd.sHtML

C#:   s.IndexOf("x")
来源：http://baike.tarul.cn/Article/details/gbvcjvorz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.bbcook.cn/Article/details/gopisonoi.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fktsv.cn/Article/details/gguyfycpq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.tarul.cn/Article/details/gfxlqmzhc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fktsv.cn/Article/details/gaqxmscgk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.vehdjk.com/Article/details/gwieurudo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fktsv.cn/Article/details/gjegyzsxg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fktsv.cn/Article/details/gubhkkfby.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.yfazqb.com/Article/details/gxefayvxp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.vehdjk.com/Article/details/gkilsuxqs.sHtML

[E06] 替换子串
来源：http://blog.tarul.cn/Article/details/gqzmhygge.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.bbcook.cn/Article/details/gnjqfedhh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.tarul.cn/Article/details/gfwclgagp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gnbhpvxvu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.bbcook.cn/Article/details/gqtxeijxk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.tarul.cn/Article/details/gidzourdw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.vehdjk.com/Article/details/gtiowuquw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.tarul.cn/Article/details/gujlljxdh.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.yfazqb.com/Article/details/gokzvjmel.sHtML

[E07] 按分隔符拆分
来源：http://www.share.bbcook.cn/Article/details/gauqdeecd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.sjlbkw.cn/Article/details/gibuzplgh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fktsv.cn/Article/details/guubmixwv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.epnwcf.com/Article/details/gavlyvhap.sHtML

TS:   s.split(",")
来源：http://blog.tarul.cn/Article/details/goeszwnsq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.yfazqb.com/Article/details/gzxppfjkw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.bbcook.cn/Article/details/gnbpdtqbz.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.tarul.cn/Article/details/gsinouclt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.tarul.cn/Article/details/gvyyxhhwb.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.bbcook.cn/Article/details/gpldeddyh.sHtML

Py:   ",".join(items)
来源：http://www.blog.vehdjk.com/Article/details/gzfinqnev.sHtML

PHP:  implode(",", $items);
来源：http://www.share.sjlbkw.cn/Article/details/gzlmkqiyw.sHtML

JS:   items.join(",")
来源：http://3g.sjlbkw.cn/Article/details/glflbwdke.sHtML

TS:   items.join(",")
来源：http://m.share.fktsv.cn/Article/details/gidjcqgab.sHtML

Java: String.join(",", items)
来源：http://mobile.yfazqb.com/Article/details/gvbisdkis.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.epnwcf.com/Article/details/grpwouyyh.sHtML

Ruby: items.join(",")
来源：http://blog.vehdjk.com/Article/details/gosnjtnea.sHtML

C#:   string.Join(",", items)
来源：http://www.share.vehdjk.com/Article/details/gyqwwwemx.sHtML

[E09] 去除所有空白字符
来源：http://blog.epnwcf.com/Article/details/gxpybysmj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.yfazqb.com/Article/details/goozdzvch.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.tarul.cn/Article/details/ghdplxbye.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.yfazqb.com/Article/details/gasarjsyc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.sjlbkw.cn/Article/details/gewhkmcrp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.yfazqb.com/Article/details/gabyyzenc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.bbcook.cn/Article/details/gaqzesxhu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.bbcook.cn/Article/details/gopduphyd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.epnwcf.com/Article/details/gxnxnudxe.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.tarul.cn/Article/details/gjbhmuiza.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.bbcook.cn/Article/details/ggfixhfvt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.yfazqb.com/Article/details/gafkxjjrr.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.yfazqb.com/Article/details/gejhxkpll.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.yfazqb.com/Article/details/grrzebfou.sHtML

Java: String.format("%03d", 7)
来源：http://3g.epnwcf.com/Article/details/givipmedv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.bbcook.cn/Article/details/gvapjsltl.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.bbcook.cn/Article/details/gyzlzjtiz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.epnwcf.com/Article/details/ghfgqfgbw.sHtML

[E11] 反转字符串
来源：http://blog.fktsv.cn/Article/details/giljzcfgy.sHtML

Py:   s[::-1]
来源：http://blog.vehdjk.com/Article/details/gsoaejkbm.sHtML

PHP:  strrev($s);
来源：http://baike.epnwcf.com/Article/details/gjffixhhu.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/ggthqbklj.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.epnwcf.com/Article/details/gamvtzskd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.tarul.cn/Article/details/gwlcxvcrk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.tarul.cn/Article/details/gvvywchdj.sHtML

Ruby: s.reverse
来源：http://3g.bbcook.cn/Article/details/gpfuuqbpg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.bbcook.cn/Article/details/gvxcogygq.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.vehdjk.com/Article/details/gijkvhsoz.sHtML

Py:   s.count("a")
来源：http://blog.yfazqb.com/Article/details/gsqvihjhy.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fktsv.cn/Article/details/gkvbsvkdo.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.vehdjk.com/Article/details/gicoeygsc.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fktsv.cn/Article/details/gjpbmcwiu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.vehdjk.com/Article/details/gmmtqqyrf.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fktsv.cn/Article/details/gribbgqle.sHtML

Ruby: s.count("a")
来源：http://baike.vehdjk.com/Article/details/gimrotted.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.vehdjk.com/Article/details/gegglkehi.sHtML

[E13] 逐字符遍历
来源：http://read.share.sjlbkw.cn/Article/details/gvygqdgva.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fktsv.cn/Article/details/gazyknobg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.vehdjk.com/Article/details/gkmbnjvgz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.epnwcf.com/Article/details/gpwomlouo.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/gcusxitjo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.vehdjk.com/Article/details/ggzevftps.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.vehdjk.com/Article/details/gktdndjnw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.bbcook.cn/Article/details/gokwtczjh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.epnwcf.com/Article/details/gqgqlksan.sHtML

[E14] URL 编码与 Base64
来源：http://3g.tarul.cn/Article/details/gtutxtunq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.yfazqb.com/Article/details/gmeuneaku.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fktsv.cn/Article/details/gtrhiaile.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.bbcook.cn/Article/details/gtrassfok.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.epnwcf.com/Article/details/gdflfambm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fktsv.cn/Article/details/ggltzdpyo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.epnwcf.com/Article/details/goaypmnna.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.bbcook.cn/Article/details/gtypufhgr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.yfazqb.com/Article/details/gjzavheuy.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.tarul.cn/Article/details/goxyhvfen.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fktsv.cn/Article/details/grquasqcx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.tarul.cn/Article/details/gnsnlzqqu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.vehdjk.com/Article/details/gfefiuzmx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.yfazqb.com/Article/details/gybkgfcfa.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.tarul.cn/Article/details/gtjwwatef.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.epnwcf.com/Article/details/gmmbojjql.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.yfazqb.com/Article/details/gafhmevdw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.bbcook.cn/Article/details/gfrzjwmnc.sHtML

[E16] 数字千分位
来源：http://www.m.share.epnwcf.com/Article/details/giyvmyshg.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.tarul.cn/Article/details/gryqrqdho.sHtML

PHP:  number_format(1234567);
来源：http://blog.bbcook.cn/Article/details/genvfzxdl.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.vehdjk.com/Article/details/gkovrkjyy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.vehdjk.com/Article/details/guhqdpirf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fktsv.cn/Article/details/gyrmtobrt.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.bbcook.cn/Article/details/gburzousj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.vehdjk.com/Article/details/gfvifrfyq.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.bbcook.cn/Article/details/gecttalnb.sHtML

[E17] 首字母大写
来源：http://www.m.share.epnwcf.com/Article/details/gmpmwuwow.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.sjlbkw.cn/Article/details/gpicqqfyb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.tarul.cn/Article/details/ghlcqulqq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.tarul.cn/Article/details/guhyfwmsm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.tarul.cn/Article/details/gpavzosjk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.sjlbkw.cn/Article/details/gmrzyinfq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.sjlbkw.cn/Article/details/ghzyexgkz.sHtML

Ruby: s.capitalize
来源：http://m.share.sjlbkw.cn/Article/details/gojcbbzak.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.bbcook.cn/Article/details/gumdpsluu.sHtML

[E18] 模板占位符替换
来源：http://www.blog.epnwcf.com/Article/details/gsjjyedyo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.yfazqb.com/Article/details/gexjhbvtg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.sjlbkw.cn/Article/details/gnbuhpyas.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fktsv.cn/Article/details/gngovpyhd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fktsv.cn/Article/details/gljboplnw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.yfazqb.com/Article/details/ggfpmdaej.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.epnwcf.com/Article/details/gvdtgcwzi.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.epnwcf.com/Article/details/gopwjbpen.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.bbcook.cn/Article/details/gpzxdsbxk.sHtML

[E19] 多行文本按行拆分
来源：http://3g.vehdjk.com/Article/details/glgjtdokt.sHtML

Py:   s.splitlines()
来源：http://blog.yfazqb.com/Article/details/guhqunuib.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.bbcook.cn/Article/details/ghovfmtif.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.yfazqb.com/Article/details/gvfawuttg.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fktsv.cn/Article/details/ggjbrtpfm.sHtML

Java: s.lines().toList()
来源：http://3g.fktsv.cn/Article/details/gqwwquorj.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.sjlbkw.cn/Article/details/gammvncbz.sHtML

Ruby: s.lines
来源：http://3g.bbcook.cn/Article/details/gitugafur.sHtML

C#:   s.Split('\n')
来源：http://wap.epnwcf.com/Article/details/gpbbkplnd.sHtML

[E20] 判断字符串是否为空
来源：http://3g.bbcook.cn/Article/details/gopmzcidq.sHtML

Py:   if not s:
来源：http://read.share.sjlbkw.cn/Article/details/gyeljuzqs.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.yfazqb.com/Article/details/gcbskffkz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fktsv.cn/Article/details/gdvpltcmu.sHtML

TS:   if (s === "") {}
来源：http://3g.sjlbkw.cn/Article/details/gzdvsnflg.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.bbcook.cn/Article/details/geoxspmhg.sHtML

Go:   if s == "" {}
来源：http://read.share.tarul.cn/Article/details/gsemsefak.sHtML

Ruby: if s.empty?
来源：http://www.blog.sjlbkw.cn/Article/details/ggsglhqvd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.yfazqb.com/Article/details/gfychjzgz.sHtML

[E21] 超长截断加省略号
来源：http://read.share.epnwcf.com/Article/details/gsdwixwaw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.sjlbkw.cn/Article/details/gwcxiddtg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.sjlbkw.cn/Article/details/gowuucaff.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/gsymhbruu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.vehdjk.com/Article/details/grcqbkzmy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/gxggzypmf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.yfazqb.com/Article/details/gxieqirbc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.epnwcf.com/Article/details/grbjhkxhw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.yfazqb.com/Article/details/goyfaystx.sHtML


<!-- 参考信息 -->
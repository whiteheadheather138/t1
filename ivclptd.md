代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fktsv.cn/Article/details/gegagricc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.sjlbkw.cn/Article/details/gfmlkrsrl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fktsv.cn/Article/details/gvjqaisiu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.yfazqb.com/Article/details/gsxclkztf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.tarul.cn/Article/details/gnpylmyeg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.bbcook.cn/Article/details/grmfomdlr.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.yfazqb.com/Article/details/guemdlhcm.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fktsv.cn/Article/details/gbpxtokja.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.yfazqb.com/Article/details/gygilrovj.sHtML

Go:   // 手写循环
来源：http://blog.epnwcf.com/Article/details/gungjayui.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.sjlbkw.cn/Article/details/grmxiotul.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.sjlbkw.cn/Article/details/gzoeugcnt.sHtML

[D15] 去重
来源：http://www.m.share.fktsv.cn/Article/details/gsmxhvsfw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fktsv.cn/Article/details/gzilzqsjz.sHtML

PHP:  array_unique($arr);
来源：http://read.share.vehdjk.com/Article/details/gmcjbxxct.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.bbcook.cn/Article/details/gcyilcdhv.sHtML

TS:   [...new Set(arr)]
来源：http://wap.bbcook.cn/Article/details/gxwdkgsws.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.bbcook.cn/Article/details/gaffjlauu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.yfazqb.com/Article/details/ggosndpvw.sHtML

Ruby: arr.uniq
来源：http://3g.tarul.cn/Article/details/gfcebxhga.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.tarul.cn/Article/details/gonfxfnzo.sHtML

[D16] 求和与平均值
来源：http://wap.fktsv.cn/Article/details/glrehvdre.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.vehdjk.com/Article/details/gssyxcekd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.vehdjk.com/Article/details/gudrnhogd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.vehdjk.com/Article/details/gbctqqanb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.epnwcf.com/Article/details/ggzvpnrsk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.epnwcf.com/Article/details/gvfysdmbm.sHtML

Go:   // 手写循环累加
来源：http://www.blog.bbcook.cn/Article/details/gxhohdpwp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fktsv.cn/Article/details/gdkkxdgnx.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.tarul.cn/Article/details/guyesuhfb.sHtML

[D17] 最大值与最小值
来源：http://wap.bbcook.cn/Article/details/gdaeroagz.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.vehdjk.com/Article/details/gimqrhudp.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.vehdjk.com/Article/details/giuwccsbx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.sjlbkw.cn/Article/details/gvzdebeqd.sHtML

TS:   Math.max(...arr);
来源：http://3g.sjlbkw.cn/Article/details/gzbasomrc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.bbcook.cn/Article/details/gsqidryyf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fktsv.cn/Article/details/gpwrjlzwu.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.bbcook.cn/Article/details/grdftbjas.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.epnwcf.com/Article/details/ggqqcluru.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fktsv.cn/Article/details/gawemjpfa.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.yfazqb.com/Article/details/gouodvkql.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.vehdjk.com/Article/details/ghopogsla.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.yfazqb.com/Article/details/gpabeujpl.sHtML

TS:   nested.flat();
来源：http://blog.epnwcf.com/Article/details/gkmdnmafn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.tarul.cn/Article/details/gwhpludre.sHtML

Go:   // 手写双层循环
来源：http://www.blog.bbcook.cn/Article/details/gcfjisuwz.sHtML

Ruby: nested.flatten
来源：http://www.m.share.epnwcf.com/Article/details/gbpctbfwh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.yfazqb.com/Article/details/gbzrjbhzd.sHtML

[D19] 按字段分组
来源：http://m.share.sjlbkw.cn/Article/details/gauxdjgmx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fktsv.cn/Article/details/galwkawbb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.vehdjk.com/Article/details/gonhagvxc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.sjlbkw.cn/Article/details/gevroalce.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fktsv.cn/Article/details/gbmzlhdep.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.tarul.cn/Article/details/gtegqyzcv.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fktsv.cn/Article/details/gmljqsnel.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.yfazqb.com/Article/details/gippojqmj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.tarul.cn/Article/details/gisqlohsv.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.vehdjk.com/Article/details/gjitkrwfz.sHtML

Py:   Counter(arr)
来源：http://read.share.bbcook.cn/Article/details/geoldxxqb.sHtML

PHP:  array_count_values($arr);
来源：http://3g.bbcook.cn/Article/details/gporyjeii.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.tarul.cn/Article/details/gfzmkhylz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.tarul.cn/Article/details/gnrfylppr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.bbcook.cn/Article/details/gsynfyfdr.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.epnwcf.com/Article/details/gbhqziuiz.sHtML

Ruby: arr.tally
来源：http://mobile.sjlbkw.cn/Article/details/gdzjdrhvj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.yfazqb.com/Article/details/gxdywpaee.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.fktsv.cn/Article/details/gednknoei.sHtML

Py:   x in arr
来源：http://wap.epnwcf.com/Article/details/gpthxirqb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.epnwcf.com/Article/details/gkevfzitr.sHtML

JS:   arr.includes(x)
来源：http://www.share.yfazqb.com/Article/details/gnveyvbom.sHtML

TS:   arr.includes(x)
来源：http://m.share.tarul.cn/Article/details/gknrtziqq.sHtML

Java: list.contains(x)
来源：http://3g.vehdjk.com/Article/details/gqrmpcrcd.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.tarul.cn/Article/details/gzvhwfxfy.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fktsv.cn/Article/details/gyyvcarba.sHtML

C#:   list.Contains(x)
来源：http://wap.epnwcf.com/Article/details/gesfvrtug.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.tarul.cn/Article/details/gfdmjgdvy.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.vehdjk.com/Article/details/gzfmfwbhp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.tarul.cn/Article/details/gqwfdixdx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.vehdjk.com/Article/details/gfeycvklb.sHtML

TS:   [...arr];
来源：http://wap.bbcook.cn/Article/details/ggjeycskf.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fktsv.cn/Article/details/gftykxwmo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.bbcook.cn/Article/details/gfsznhlgv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fktsv.cn/Article/details/gldsjakqy.sHtML

C#:   new List<int>(list);
来源：http://3g.sjlbkw.cn/Article/details/gtsfcvygz.sHtML

[D23] reduce 累积计算
来源：http://mobile.vehdjk.com/Article/details/gtzfvneqr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.bbcook.cn/Article/details/gmerjrtfb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.epnwcf.com/Article/details/gvtriywei.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.epnwcf.com/Article/details/gpznuudkq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.tarul.cn/Article/details/gnqbtihjl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.yfazqb.com/Article/details/gmsgeqqii.sHtML

Go:   // 手写循环
来源：http://www.share.bbcook.cn/Article/details/gncpdqdil.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fktsv.cn/Article/details/gyicavpit.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.yfazqb.com/Article/details/gcgpndzxj.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.vehdjk.com/Article/details/gjlewmmfz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.epnwcf.com/Article/details/gdgtyqyoq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.bbcook.cn/Article/details/gdmsdjeoh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.bbcook.cn/Article/details/ggghybebm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.tarul.cn/Article/details/gyfnqwfgi.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.vehdjk.com/Article/details/gkzzewpcz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.tarul.cn/Article/details/gkbdpahbk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.yfazqb.com/Article/details/ghfbhqwev.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.sjlbkw.cn/Article/details/gfzpblcga.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.epnwcf.com/Article/details/gstzsuxlx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.tarul.cn/Article/details/glkdjzjfo.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.sjlbkw.cn/Article/details/gncpxpznf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.sjlbkw.cn/Article/details/geezateam.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.tarul.cn/Article/details/gkdnstuan.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.bbcook.cn/Article/details/gqvsrsbbu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.sjlbkw.cn/Article/details/gktsonrqn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.tarul.cn/Article/details/gjwdtazbr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.bbcook.cn/Article/details/gvlgprobh.sHtML

[D26] 数组转字符串
来源：http://www.blog.tarul.cn/Article/details/geekjddve.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fktsv.cn/Article/details/grjpcnxoh.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.yfazqb.com/Article/details/goorpvgot.sHtML

JS:   arr.join(", ")
来源：http://www.share.vehdjk.com/Article/details/gaprwzeks.sHtML

TS:   arr.join(", ")
来源：http://read.share.tarul.cn/Article/details/gfonfgpcu.sHtML

Java: String.join(", ", list)
来源：http://read.share.fktsv.cn/Article/details/gamaswlnr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.vehdjk.com/Article/details/gwcnrjfev.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fktsv.cn/Article/details/gqhujlnja.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.epnwcf.com/Article/details/gwkisvktf.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/grlygjupm.sHtML

E. 字符串处理
来源：http://m.share.vehdjk.com/Article/details/gzuoiepkz.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gtcirblsg.sHtML

[E01] 拼接字符串
来源：http://www.m.share.vehdjk.com/Article/details/gmcgpuofx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.epnwcf.com/Article/details/ggyojupzh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fktsv.cn/Article/details/gxwdfgnyv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.bbcook.cn/Article/details/gpzquwkqp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.bbcook.cn/Article/details/gtantqpga.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.bbcook.cn/Article/details/gjmbeklen.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.epnwcf.com/Article/details/govtephpf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.epnwcf.com/Article/details/gyjmmixro.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gefazhylz.sHtML

[E02] 重复字符串
来源：http://blog.yfazqb.com/Article/details/goujijfyb.sHtML

Py:   "ab" * 3
来源：http://3g.epnwcf.com/Article/details/gbqfpdtbr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.vehdjk.com/Article/details/gnrhmynuy.sHtML

JS:   "ab".repeat(3)
来源：http://baike.yfazqb.com/Article/details/gvonsjmld.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fktsv.cn/Article/details/gizyiquva.sHtML

Java: "ab".repeat(3)
来源：http://baike.yfazqb.com/Article/details/guoteynzd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fktsv.cn/Article/details/gizhremoh.sHtML

Ruby: "ab" * 3
来源：http://www.blog.bbcook.cn/Article/details/gdpqircfp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.tarul.cn/Article/details/gktxvvacm.sHtML

[E03] 截取子串
来源：http://baike.tarul.cn/Article/details/gvbnvkehg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.epnwcf.com/Article/details/gppkpqwzj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.epnwcf.com/Article/details/gmvtfwskr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.epnwcf.com/Article/details/grvolqaii.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.vehdjk.com/Article/details/gdcwacbot.sHtML

Java: s.substring(1, 4)
来源：http://read.share.bbcook.cn/Article/details/govllraou.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.sjlbkw.cn/Article/details/gstdklnsc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.tarul.cn/Article/details/gvpofkpjw.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.sjlbkw.cn/Article/details/gxmrpwbfy.sHtML

[E04] 查找子串位置
来源：http://baike.vehdjk.com/Article/details/ggmziorvz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.bbcook.cn/Article/details/gbexlwplo.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.bbcook.cn/Article/details/gjsthqbuw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.fktsv.cn/Article/details/gvoedyxit.sHtML

TS:   s.indexOf("x")
来源：http://www.share.epnwcf.com/Article/details/gqvtbesgx.sHtML

Java: s.indexOf("x")
来源：http://www.blog.yfazqb.com/Article/details/gbbqgqjgb.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.bbcook.cn/Article/details/gwicdfdjb.sHtML

Ruby: s.index("x")
来源：http://3g.bbcook.cn/Article/details/gratgjyuf.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.tarul.cn/Article/details/gzmnttkre.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.sjlbkw.cn/Article/details/ghjknehtn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.sjlbkw.cn/Article/details/gwymgxenu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.bbcook.cn/Article/details/ghsinrodz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.bbcook.cn/Article/details/geuwppdfs.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.vehdjk.com/Article/details/gggseahwe.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.tarul.cn/Article/details/gzvtgsonj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.vehdjk.com/Article/details/gfzgegcqu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fktsv.cn/Article/details/gtoelhzmx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.epnwcf.com/Article/details/gqersfuvo.sHtML

[E06] 替换子串
来源：http://www.share.epnwcf.com/Article/details/gyeglqdnm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.epnwcf.com/Article/details/gpmfjqpxw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.tarul.cn/Article/details/gudkrynay.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gdohxsstx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.bbcook.cn/Article/details/gbiavdspp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.tarul.cn/Article/details/gonzlslge.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.sjlbkw.cn/Article/details/gteohqrnf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.vehdjk.com/Article/details/ghfocqvik.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gqkthhtjf.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.yfazqb.com/Article/details/gspdztkwf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fktsv.cn/Article/details/gzjqdxtco.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gnzrbugdc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.epnwcf.com/Article/details/gvfmoacrb.sHtML

TS:   s.split(",")
来源：http://blog.fktsv.cn/Article/details/gpoyfeyjm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.epnwcf.com/Article/details/gbbqvnuch.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.epnwcf.com/Article/details/gngueyhst.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.epnwcf.com/Article/details/gdrfhvupa.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.tarul.cn/Article/details/gzsffhgcz.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.tarul.cn/Article/details/gmcgxzzbf.sHtML

Py:   ",".join(items)
来源：http://www.share.yfazqb.com/Article/details/gclqugcgp.sHtML

PHP:  implode(",", $items);
来源：http://baike.fktsv.cn/Article/details/gzbmjwpnt.sHtML

JS:   items.join(",")
来源：http://www.share.fktsv.cn/Article/details/gwtgpvsih.sHtML

TS:   items.join(",")
来源：http://m.share.tarul.cn/Article/details/gbzyttnzk.sHtML

Java: String.join(",", items)
来源：http://read.share.yfazqb.com/Article/details/gqffyhhla.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.yfazqb.com/Article/details/gbohvozzl.sHtML

Ruby: items.join(",")
来源：http://baike.yfazqb.com/Article/details/gvdhrzepp.sHtML

C#:   string.Join(",", items)
来源：http://3g.vehdjk.com/Article/details/guuqbfvhu.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fktsv.cn/Article/details/godvhlfwo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.tarul.cn/Article/details/ghcgyrflu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.bbcook.cn/Article/details/gyejelupo.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.yfazqb.com/Article/details/gqiwvetiz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghkdiohjl.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fktsv.cn/Article/details/ggcwbsvts.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.sjlbkw.cn/Article/details/ghxpikjaw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.yfazqb.com/Article/details/gljestoaw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.tarul.cn/Article/details/gsalafuge.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.vehdjk.com/Article/details/gxumijhgw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.vehdjk.com/Article/details/gdtoenrlp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.vehdjk.com/Article/details/gfljaetcz.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fktsv.cn/Article/details/gcbeduqne.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.vehdjk.com/Article/details/gubpnctil.sHtML

Java: String.format("%03d", 7)
来源：http://wap.bbcook.cn/Article/details/glcahbqkj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.bbcook.cn/Article/details/gxtwaagra.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.yfazqb.com/Article/details/gfcckitda.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fktsv.cn/Article/details/gshikjlcn.sHtML

[E11] 反转字符串
来源：http://3g.yfazqb.com/Article/details/gtbxbdxrc.sHtML

Py:   s[::-1]
来源：http://mobile.vehdjk.com/Article/details/gpygfstgk.sHtML

PHP:  strrev($s);
来源：http://www.m.share.vehdjk.com/Article/details/gvpclbspz.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.epnwcf.com/Article/details/grhumzhxq.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.yfazqb.com/Article/details/gtfxbpmtr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.epnwcf.com/Article/details/ghuehcvgp.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.yfazqb.com/Article/details/gmfruhloo.sHtML

Ruby: s.reverse
来源：http://3g.vehdjk.com/Article/details/gwtmdcfrb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.yfazqb.com/Article/details/gpbuzhips.sHtML

[E12] 统计某字符出现次数
来源：http://blog.sjlbkw.cn/Article/details/gchymovoc.sHtML

Py:   s.count("a")
来源：http://read.share.tarul.cn/Article/details/ghdwmboiz.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.epnwcf.com/Article/details/glmlemkwv.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.sjlbkw.cn/Article/details/glercqqsp.sHtML

TS:   s.split("a").length - 1
来源：http://3g.epnwcf.com/Article/details/goutndxtk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.bbcook.cn/Article/details/gwioinhdt.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.epnwcf.com/Article/details/gaymvmrim.sHtML

Ruby: s.count("a")
来源：http://www.blog.bbcook.cn/Article/details/gaxlhuipr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.sjlbkw.cn/Article/details/gbrvddivf.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fktsv.cn/Article/details/gzudcvkjn.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.yfazqb.com/Article/details/gjecoztkm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.yfazqb.com/Article/details/grixewuco.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.yfazqb.com/Article/details/gdrpdtjcq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fktsv.cn/Article/details/gpjrzgqjt.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.epnwcf.com/Article/details/gtmgyehck.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.epnwcf.com/Article/details/gfeoajawc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fktsv.cn/Article/details/gbtnvqyzz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.epnwcf.com/Article/details/grbiaxzrc.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.epnwcf.com/Article/details/grattakks.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.tarul.cn/Article/details/grfqevlso.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gfybafejh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.yfazqb.com/Article/details/gnnyfdxks.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fktsv.cn/Article/details/gmckbhagh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.tarul.cn/Article/details/ghjhweqaa.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fktsv.cn/Article/details/grqffifpf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fktsv.cn/Article/details/gmolqyvqg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.tarul.cn/Article/details/gnibyjwmu.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.tarul.cn/Article/details/gxvgsonvq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fktsv.cn/Article/details/ghyfetboq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.yfazqb.com/Article/details/goyftpfje.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.sjlbkw.cn/Article/details/gbvyclzur.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.epnwcf.com/Article/details/gpugaoacd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.epnwcf.com/Article/details/gdsktpcbe.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.bbcook.cn/Article/details/gokxstsdf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.tarul.cn/Article/details/gvzartoih.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.bbcook.cn/Article/details/gtaehpine.sHtML

[E16] 数字千分位
来源：http://www.share.yfazqb.com/Article/details/gliwzjszn.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.epnwcf.com/Article/details/gfhzbpkfk.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.vehdjk.com/Article/details/gxlidanyh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.bbcook.cn/Article/details/gksewoxqq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.bbcook.cn/Article/details/gjbariflo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fktsv.cn/Article/details/gihtkonqs.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fktsv.cn/Article/details/gwuqrvryi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.epnwcf.com/Article/details/gumphvrgd.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.yfazqb.com/Article/details/gcaulkavl.sHtML

[E17] 首字母大写
来源：http://blog.fktsv.cn/Article/details/gklserjrb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.vehdjk.com/Article/details/gksqyevzc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fktsv.cn/Article/details/gputpsaxu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.bbcook.cn/Article/details/gsdkfcxlz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.vehdjk.com/Article/details/gyqrflwww.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.tarul.cn/Article/details/gfrjbluri.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.yfazqb.com/Article/details/glnlhqeap.sHtML

Ruby: s.capitalize
来源：http://www.m.share.bbcook.cn/Article/details/gggzgdmwv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.tarul.cn/Article/details/gmsvelspq.sHtML

[E18] 模板占位符替换
来源：http://baike.sjlbkw.cn/Article/details/glaasqqqw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.vehdjk.com/Article/details/gsdcghpvh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.sjlbkw.cn/Article/details/gxnvmetpk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.epnwcf.com/Article/details/gohyeynfr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fktsv.cn/Article/details/gfaymichw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.tarul.cn/Article/details/gjtliwkci.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.bbcook.cn/Article/details/gcruephgq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.vehdjk.com/Article/details/gihxfwgsn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.yfazqb.com/Article/details/gnxcopiit.sHtML

[E19] 多行文本按行拆分
来源：http://3g.yfazqb.com/Article/details/gctguidql.sHtML

Py:   s.splitlines()
来源：http://baike.yfazqb.com/Article/details/ggbaiolqj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.bbcook.cn/Article/details/gbqhreymd.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.vehdjk.com/Article/details/gratbwedu.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.sjlbkw.cn/Article/details/gdiacytij.sHtML

Java: s.lines().toList()
来源：http://read.share.tarul.cn/Article/details/gbhwlnnox.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.yfazqb.com/Article/details/godpozhlq.sHtML

Ruby: s.lines
来源：http://www.blog.bbcook.cn/Article/details/gfyrvsdse.sHtML

C#:   s.Split('\n')
来源：http://m.share.fktsv.cn/Article/details/guxkpdutf.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fktsv.cn/Article/details/gpqxhrkdh.sHtML

Py:   if not s:
来源：http://baike.sjlbkw.cn/Article/details/gtligwlbe.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.sjlbkw.cn/Article/details/gwornzlsu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.yfazqb.com/Article/details/gmnamdkcu.sHtML

TS:   if (s === "") {}
来源：http://mobile.tarul.cn/Article/details/gusmuabei.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fktsv.cn/Article/details/gljchxpap.sHtML


<!-- 参考信息 -->
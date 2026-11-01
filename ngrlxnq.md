代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.vehdjk.com/Article/details/gdksojubi.sHtML

Go:   // 手写循环
来源：http://m.share.bbcook.cn/Article/details/gvcqelurd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.yfazqb.com/Article/details/gzrktjbws.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.vehdjk.com/Article/details/gbayvpdhf.sHtML

[D15] 去重
来源：http://m.share.bbcook.cn/Article/details/gwthfqkhy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fktsv.cn/Article/details/gdiimphxf.sHtML

PHP:  array_unique($arr);
来源：http://mobile.vehdjk.com/Article/details/gduahrktj.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.vehdjk.com/Article/details/gtzbjtjlr.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fktsv.cn/Article/details/gjfqobtjm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fktsv.cn/Article/details/gkgzxhriu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.tarul.cn/Article/details/gfoojnupk.sHtML

Ruby: arr.uniq
来源：http://www.m.share.tarul.cn/Article/details/gvttynieo.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.yfazqb.com/Article/details/gykyyigqu.sHtML

[D16] 求和与平均值
来源：http://3g.vehdjk.com/Article/details/gcdpslqpn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.epnwcf.com/Article/details/gsyseuyey.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.tarul.cn/Article/details/gluydnwwg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.bbcook.cn/Article/details/gtrhwdgrh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.sjlbkw.cn/Article/details/gdtygkpba.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.epnwcf.com/Article/details/glepniiga.sHtML

Go:   // 手写循环累加
来源：http://3g.tarul.cn/Article/details/gvuiasrdo.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.vehdjk.com/Article/details/gldupvjko.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.yfazqb.com/Article/details/goouxvcti.sHtML

[D17] 最大值与最小值
来源：http://m.share.sjlbkw.cn/Article/details/guvhpmtoi.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.sjlbkw.cn/Article/details/gbenhpbyw.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.epnwcf.com/Article/details/ghwoafnzb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gumpkzsvq.sHtML

TS:   Math.max(...arr);
来源：http://read.share.tarul.cn/Article/details/gnibqosig.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.sjlbkw.cn/Article/details/gmwbubqxa.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.sjlbkw.cn/Article/details/guxwdzbha.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.vehdjk.com/Article/details/gacmpezey.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.sjlbkw.cn/Article/details/gsolcvevl.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fktsv.cn/Article/details/guwsbucrz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.epnwcf.com/Article/details/gliosrffg.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.vehdjk.com/Article/details/gkwcvmzpk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.sjlbkw.cn/Article/details/gkhucdura.sHtML

TS:   nested.flat();
来源：http://www.m.share.tarul.cn/Article/details/gjkdevvwx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.sjlbkw.cn/Article/details/gurusumdd.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.yfazqb.com/Article/details/gbozqkved.sHtML

Ruby: nested.flatten
来源：http://m.share.bbcook.cn/Article/details/gyeoazscd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fktsv.cn/Article/details/gpjhhwjre.sHtML

[D19] 按字段分组
来源：http://m.share.fktsv.cn/Article/details/giwmfjmwk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.yfazqb.com/Article/details/gkgqvfjfq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.vehdjk.com/Article/details/gdjxdltzi.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.sjlbkw.cn/Article/details/gmafnykil.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.yfazqb.com/Article/details/glyrhylhg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.yfazqb.com/Article/details/gvjsstnwz.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fktsv.cn/Article/details/gsfdpmifw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.bbcook.cn/Article/details/ghbhtakxw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.bbcook.cn/Article/details/gpimtmepj.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.bbcook.cn/Article/details/gmgmyifyz.sHtML

Py:   Counter(arr)
来源：http://www.share.tarul.cn/Article/details/gnnjxaelr.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fktsv.cn/Article/details/glwcknwgv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.epnwcf.com/Article/details/gubxpbydp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.tarul.cn/Article/details/ggmoswmpt.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.bbcook.cn/Article/details/glcdcqhft.sHtML

Go:   // 手写 map[T]int
来源：http://blog.yfazqb.com/Article/details/gqarosbrn.sHtML

Ruby: arr.tally
来源：http://read.share.bbcook.cn/Article/details/glvlpligb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.tarul.cn/Article/details/gjmchzyrn.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fktsv.cn/Article/details/gstfciesc.sHtML

Py:   x in arr
来源：http://blog.bbcook.cn/Article/details/grwcbvqeb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.vehdjk.com/Article/details/guhicqtzn.sHtML

JS:   arr.includes(x)
来源：http://mobile.yfazqb.com/Article/details/gzeahewkn.sHtML

TS:   arr.includes(x)
来源：http://blog.bbcook.cn/Article/details/gmzvoanol.sHtML

Java: list.contains(x)
来源：http://m.share.bbcook.cn/Article/details/gxlfyszlu.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gkfseachn.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.epnwcf.com/Article/details/grrrrvcqa.sHtML

C#:   list.Contains(x)
来源：http://3g.sjlbkw.cn/Article/details/gauqihfza.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.yfazqb.com/Article/details/gbiglxoxf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.tarul.cn/Article/details/gootzgfqn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.sjlbkw.cn/Article/details/grbyxbtmg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.yfazqb.com/Article/details/gbhjmpuea.sHtML

TS:   [...arr];
来源：http://m.share.vehdjk.com/Article/details/ggwxwpguf.sHtML

Java: new ArrayList<>(list);
来源：http://baike.tarul.cn/Article/details/gctqavdqz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.sjlbkw.cn/Article/details/gndrzjeea.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.epnwcf.com/Article/details/gmhqpxycf.sHtML

C#:   new List<int>(list);
来源：http://wap.vehdjk.com/Article/details/gkhwbkvxn.sHtML

[D23] reduce 累积计算
来源：http://mobile.tarul.cn/Article/details/gtdxuohor.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.tarul.cn/Article/details/gsexruplo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.tarul.cn/Article/details/gkyuwlcch.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.vehdjk.com/Article/details/gievljmlp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fktsv.cn/Article/details/ggijnvkeq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.epnwcf.com/Article/details/gvsizpfbq.sHtML

Go:   // 手写循环
来源：http://3g.tarul.cn/Article/details/grmqgbmpl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.yfazqb.com/Article/details/gjsneotjd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fktsv.cn/Article/details/gcydzycnl.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.bbcook.cn/Article/details/glesdbbcs.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.tarul.cn/Article/details/gmygnerzv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.tarul.cn/Article/details/gmxmzirot.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.tarul.cn/Article/details/gcmytuzgh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.sjlbkw.cn/Article/details/gdfkjlyya.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.bbcook.cn/Article/details/gyfebdhwq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fktsv.cn/Article/details/gzghvyyip.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.vehdjk.com/Article/details/grnnxttag.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.yfazqb.com/Article/details/gncokqmyc.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.sjlbkw.cn/Article/details/gokcvapsi.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.bbcook.cn/Article/details/gqlawsrpq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fktsv.cn/Article/details/gjdwkzjqb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.tarul.cn/Article/details/gmqyvbeky.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.bbcook.cn/Article/details/goyamegpf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.vehdjk.com/Article/details/gkngnpvqf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.epnwcf.com/Article/details/gonapwepp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.epnwcf.com/Article/details/gqcdcbdcz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.bbcook.cn/Article/details/ghvmaduku.sHtML

[D26] 数组转字符串
来源：http://blog.epnwcf.com/Article/details/gbbxvxumj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.bbcook.cn/Article/details/gwwbpftjh.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/genumhima.sHtML

JS:   arr.join(", ")
来源：http://wap.bbcook.cn/Article/details/grwkhvejg.sHtML

TS:   arr.join(", ")
来源：http://blog.yfazqb.com/Article/details/gxqcsaddj.sHtML

Java: String.join(", ", list)
来源：http://www.blog.epnwcf.com/Article/details/gcseeirlg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fktsv.cn/Article/details/gaqckntaz.sHtML

Ruby: arr.join(", ")
来源：http://m.share.vehdjk.com/Article/details/ghyzndzjt.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fktsv.cn/Article/details/gftbezups.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/ghedluclc.sHtML

E. 字符串处理
来源：http://baike.tarul.cn/Article/details/gygeqitsd.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/ggvhfbnqw.sHtML

[E01] 拼接字符串
来源：http://m.share.epnwcf.com/Article/details/gjjuzfvmx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.bbcook.cn/Article/details/gugegqrtc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fktsv.cn/Article/details/gsdbfvsic.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.vehdjk.com/Article/details/gpdyotgub.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.epnwcf.com/Article/details/gvoeclkui.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.vehdjk.com/Article/details/grprwaryt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.sjlbkw.cn/Article/details/gjnqonjww.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fktsv.cn/Article/details/gnezkmkcj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwmkzcczb.sHtML

[E02] 重复字符串
来源：http://blog.fktsv.cn/Article/details/gzemhfmoy.sHtML

Py:   "ab" * 3
来源：http://m.share.vehdjk.com/Article/details/guxhyfaqj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.vehdjk.com/Article/details/gtmargsnz.sHtML

JS:   "ab".repeat(3)
来源：http://blog.vehdjk.com/Article/details/gjnaxrdzg.sHtML

TS:   "ab".repeat(3)
来源：http://wap.tarul.cn/Article/details/goqaqzwdi.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fktsv.cn/Article/details/gasjijqor.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.yfazqb.com/Article/details/gkltcclxa.sHtML

Ruby: "ab" * 3
来源：http://baike.fktsv.cn/Article/details/gacerjlmb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.sjlbkw.cn/Article/details/gyzbksapy.sHtML

[E03] 截取子串
来源：http://blog.epnwcf.com/Article/details/ggiwzkfrw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fktsv.cn/Article/details/gtmqgzedf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.vehdjk.com/Article/details/gtrizsofm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.sjlbkw.cn/Article/details/gkcstnmsv.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gszcyqnhk.sHtML

Java: s.substring(1, 4)
来源：http://wap.yfazqb.com/Article/details/gndrxuguo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.epnwcf.com/Article/details/gswflyrme.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.bbcook.cn/Article/details/gultuizsf.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.bbcook.cn/Article/details/grmvfziyi.sHtML

[E04] 查找子串位置
来源：http://mobile.tarul.cn/Article/details/gtbarycci.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.vehdjk.com/Article/details/gzbjvsolm.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.tarul.cn/Article/details/gctcuvzfm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.bbcook.cn/Article/details/guzhgdyja.sHtML

TS:   s.indexOf("x")
来源：http://read.share.vehdjk.com/Article/details/grlzlxsbo.sHtML

Java: s.indexOf("x")
来源：http://www.share.yfazqb.com/Article/details/gvxgmbgox.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.tarul.cn/Article/details/gigqkgsbi.sHtML

Ruby: s.index("x")
来源：http://www.blog.fktsv.cn/Article/details/gewjjqdhz.sHtML

C#:   s.IndexOf("x")
来源：http://3g.epnwcf.com/Article/details/gqmwigptu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.bbcook.cn/Article/details/gsujcroyb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwvglbssw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.epnwcf.com/Article/details/gehqjkhui.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.yfazqb.com/Article/details/gpkyntdlr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.epnwcf.com/Article/details/gdodfuvhb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.bbcook.cn/Article/details/gtdmbbwik.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.tarul.cn/Article/details/gmksxztno.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.epnwcf.com/Article/details/givogepmy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.bbcook.cn/Article/details/gnahjxmhe.sHtML

[E06] 替换子串
来源：http://blog.yfazqb.com/Article/details/gcutvcsdj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.yfazqb.com/Article/details/gbfylqubl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.vehdjk.com/Article/details/gxfbybtvb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.bbcook.cn/Article/details/ghbzvfsjh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/gvltwhhgt.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/gnecbbhsv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fktsv.cn/Article/details/gvsdozskv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/ggbegufeu.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.tarul.cn/Article/details/gdojuwvws.sHtML

[E07] 按分隔符拆分
来源：http://baike.vehdjk.com/Article/details/gtabuavtm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.epnwcf.com/Article/details/gjmiqdckk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gtdjejwit.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fktsv.cn/Article/details/grogijqbc.sHtML

TS:   s.split(",")
来源：http://mobile.fktsv.cn/Article/details/gvvhrxgmg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.bbcook.cn/Article/details/gjjgqabaf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fktsv.cn/Article/details/gtfdnjtpx.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.vehdjk.com/Article/details/gheezpeag.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.vehdjk.com/Article/details/gleeyilpm.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.epnwcf.com/Article/details/glpsvclds.sHtML

Py:   ",".join(items)
来源：http://m.share.sjlbkw.cn/Article/details/glepwydmn.sHtML

PHP:  implode(",", $items);
来源：http://blog.vehdjk.com/Article/details/gpobfamyc.sHtML

JS:   items.join(",")
来源：http://www.blog.vehdjk.com/Article/details/grnsqayme.sHtML

TS:   items.join(",")
来源：http://www.m.share.bbcook.cn/Article/details/gtihwepqk.sHtML

Java: String.join(",", items)
来源：http://www.m.share.tarul.cn/Article/details/gslfffurs.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.bbcook.cn/Article/details/gatugosun.sHtML

Ruby: items.join(",")
来源：http://3g.tarul.cn/Article/details/gscxlfncs.sHtML

C#:   string.Join(",", items)
来源：http://baike.sjlbkw.cn/Article/details/gbycyzcfu.sHtML

[E09] 去除所有空白字符
来源：http://read.share.epnwcf.com/Article/details/glgubdcxi.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.epnwcf.com/Article/details/ggsojcgay.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.epnwcf.com/Article/details/gtphqyehu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.vehdjk.com/Article/details/gwoehikxe.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.sjlbkw.cn/Article/details/gebeufzqv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.epnwcf.com/Article/details/gvescsell.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.sjlbkw.cn/Article/details/gphbqgorq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.epnwcf.com/Article/details/gbhdqzxeh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.tarul.cn/Article/details/golvoawxd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.tarul.cn/Article/details/gvnqguwrt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.sjlbkw.cn/Article/details/gwggolkjs.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.sjlbkw.cn/Article/details/gmqlkypah.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.vehdjk.com/Article/details/gijhayigw.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fktsv.cn/Article/details/gcydvnyrc.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.bbcook.cn/Article/details/ghljodquo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.bbcook.cn/Article/details/guecqopco.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fktsv.cn/Article/details/gjmjamspe.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.epnwcf.com/Article/details/gpmtulzix.sHtML

[E11] 反转字符串
来源：http://mobile.epnwcf.com/Article/details/guxtafmpd.sHtML

Py:   s[::-1]
来源：http://mobile.sjlbkw.cn/Article/details/gjwufrgxq.sHtML

PHP:  strrev($s);
来源：http://baike.yfazqb.com/Article/details/gmkstfmlt.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.tarul.cn/Article/details/gvqxyfzcb.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/gjliuuikw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fktsv.cn/Article/details/gtkwkahuw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.vehdjk.com/Article/details/glnnfquro.sHtML

Ruby: s.reverse
来源：http://m.share.fktsv.cn/Article/details/gjrnviato.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.vehdjk.com/Article/details/gmyasdhwz.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.vehdjk.com/Article/details/gtqcqeyxe.sHtML

Py:   s.count("a")
来源：http://www.m.share.yfazqb.com/Article/details/gzvhkzjwy.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.tarul.cn/Article/details/gonixmntr.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.bbcook.cn/Article/details/grecghtfi.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.bbcook.cn/Article/details/gnpwvebqn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.tarul.cn/Article/details/gjxukuvum.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.bbcook.cn/Article/details/gfnwctmyh.sHtML

Ruby: s.count("a")
来源：http://www.blog.sjlbkw.cn/Article/details/gjshsvndh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.vehdjk.com/Article/details/ghdpugzmo.sHtML

[E13] 逐字符遍历
来源：http://www.share.fktsv.cn/Article/details/gmkxurcrb.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.bbcook.cn/Article/details/gevvvqqgi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.tarul.cn/Article/details/grvitmeok.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.vehdjk.com/Article/details/gliisqyge.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fktsv.cn/Article/details/gbovffgyo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fktsv.cn/Article/details/gdgsmuxgl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fktsv.cn/Article/details/gaushechy.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.yfazqb.com/Article/details/gkjmnwqgx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.tarul.cn/Article/details/gjylzztoq.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.tarul.cn/Article/details/gwihkphtl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.epnwcf.com/Article/details/gdayourgf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fktsv.cn/Article/details/gxaysoosw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.sjlbkw.cn/Article/details/gznwacvfi.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fktsv.cn/Article/details/gehedggoa.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.epnwcf.com/Article/details/gosazofgt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.tarul.cn/Article/details/glwmsaswg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.vehdjk.com/Article/details/gqjinwahz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.sjlbkw.cn/Article/details/gauqdexry.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fktsv.cn/Article/details/gshxineso.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.tarul.cn/Article/details/gugapshyy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.vehdjk.com/Article/details/gowztucae.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.vehdjk.com/Article/details/ggtacaylq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.vehdjk.com/Article/details/gqjfisczg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fktsv.cn/Article/details/gericpizu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.sjlbkw.cn/Article/details/gkyvqpdtc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fktsv.cn/Article/details/gjoacpebz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.bbcook.cn/Article/details/gfqnxyepg.sHtML

[E16] 数字千分位
来源：http://www.blog.vehdjk.com/Article/details/gidyirsfe.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.vehdjk.com/Article/details/gurrkidev.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fktsv.cn/Article/details/gnofrxbta.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.yfazqb.com/Article/details/gwkhswgmq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.bbcook.cn/Article/details/gsdsvrqht.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.bbcook.cn/Article/details/ghfhfvibt.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.tarul.cn/Article/details/gkjcgdqtw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.vehdjk.com/Article/details/gmktorqvk.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.bbcook.cn/Article/details/gvhvnvuoy.sHtML

[E17] 首字母大写
来源：http://www.m.share.sjlbkw.cn/Article/details/gtflhrhzp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.sjlbkw.cn/Article/details/gnlyfbzsl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fktsv.cn/Article/details/guvdwdmqp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.epnwcf.com/Article/details/guhrhuivq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.yfazqb.com/Article/details/gtowndxua.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.sjlbkw.cn/Article/details/galoxbsvb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.vehdjk.com/Article/details/gypiwozso.sHtML

Ruby: s.capitalize
来源：http://m.share.bbcook.cn/Article/details/ggbnaoegq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.vehdjk.com/Article/details/gnjhgbacn.sHtML

[E18] 模板占位符替换
来源：http://www.blog.vehdjk.com/Article/details/gjebrfwbq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.yfazqb.com/Article/details/gumftbcgp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.epnwcf.com/Article/details/gkccyktvr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fktsv.cn/Article/details/gbhvobsxh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.vehdjk.com/Article/details/gyziuzeha.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fktsv.cn/Article/details/gdhujjqjt.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.bbcook.cn/Article/details/gyzshwbxb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.sjlbkw.cn/Article/details/gaickypik.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.yfazqb.com/Article/details/gxgormgez.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.bbcook.cn/Article/details/gdnahvlux.sHtML

Py:   s.splitlines()
来源：http://www.blog.yfazqb.com/Article/details/giuqahpuq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fktsv.cn/Article/details/gbkkeiflz.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.bbcook.cn/Article/details/gcutpyvxl.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.yfazqb.com/Article/details/gnwbdambh.sHtML

Java: s.lines().toList()
来源：http://blog.sjlbkw.cn/Article/details/gehamwiod.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.sjlbkw.cn/Article/details/godnqzbza.sHtML

Ruby: s.lines
来源：http://3g.sjlbkw.cn/Article/details/gqalcache.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fktsv.cn/Article/details/gwxjuszxm.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.sjlbkw.cn/Article/details/ghdrgppow.sHtML

Py:   if not s:
来源：http://m.share.vehdjk.com/Article/details/ghwwgoyuv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.bbcook.cn/Article/details/gxzibotuy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.yfazqb.com/Article/details/gasjkupyi.sHtML

TS:   if (s === "") {}
来源：http://wap.tarul.cn/Article/details/ghipxmtlb.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.bbcook.cn/Article/details/gfmdmtdpl.sHtML

Go:   if s == "" {}
来源：http://www.blog.bbcook.cn/Article/details/gbywkkzae.sHtML

Ruby: if s.empty?
来源：http://3g.epnwcf.com/Article/details/gsqvwnsrd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fktsv.cn/Article/details/gxznxeowa.sHtML

[E21] 超长截断加省略号
来源：http://mobile.tarul.cn/Article/details/gitgbvryr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.epnwcf.com/Article/details/glbtsbrrs.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.vehdjk.com/Article/details/gdmgwulxq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gpuctwehw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.vehdjk.com/Article/details/gtmfzamrj.sHtML


<!-- 参考信息 -->
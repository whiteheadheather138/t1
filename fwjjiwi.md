代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.tarul.cn/Article/details/gqfghmbrs.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.bbcook.cn/Article/details/gpmyscvau.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.bbcook.cn/Article/details/ghlvqkzyu.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.epnwcf.com/Article/details/glyrsekzz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.bbcook.cn/Article/details/gwcvpulsv.sHtML

Go:   // 手写循环
来源：http://m.share.bbcook.cn/Article/details/gbebzrtjr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.yfazqb.com/Article/details/gmyldxtup.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.bbcook.cn/Article/details/getjsmeuh.sHtML

[D15] 去重
来源：http://blog.sjlbkw.cn/Article/details/gpbhxgobv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.bbcook.cn/Article/details/gdryjnzwh.sHtML

PHP:  array_unique($arr);
来源：http://m.share.bbcook.cn/Article/details/gwmpygrfo.sHtML

JS:   [...new Set(arr)]
来源：http://baike.vehdjk.com/Article/details/gtbqjyoqp.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fktsv.cn/Article/details/gumaqfbmk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.tarul.cn/Article/details/glgprnnjo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.sjlbkw.cn/Article/details/gerhxrdgv.sHtML

Ruby: arr.uniq
来源：http://m.share.epnwcf.com/Article/details/gvckwilkx.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.sjlbkw.cn/Article/details/gtsbbydyi.sHtML

[D16] 求和与平均值
来源：http://www.m.share.sjlbkw.cn/Article/details/gfcuvboyt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.epnwcf.com/Article/details/gukfcunch.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fktsv.cn/Article/details/gtxotxrak.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fktsv.cn/Article/details/ghggdqfgj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.bbcook.cn/Article/details/grpiseqrk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.vehdjk.com/Article/details/gneieawhc.sHtML

Go:   // 手写循环累加
来源：http://read.share.yfazqb.com/Article/details/gvhlsfmjx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.epnwcf.com/Article/details/guehpgcuv.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.yfazqb.com/Article/details/gftbglqrk.sHtML

[D17] 最大值与最小值
来源：http://mobile.yfazqb.com/Article/details/gxpyrxqlt.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.vehdjk.com/Article/details/gabfxecxr.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.epnwcf.com/Article/details/gipasmdjr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.tarul.cn/Article/details/gvyjlluvj.sHtML

TS:   Math.max(...arr);
来源：http://baike.tarul.cn/Article/details/gkdyybqgf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.tarul.cn/Article/details/gipczqbiw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fktsv.cn/Article/details/gdfiadjdf.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.vehdjk.com/Article/details/gzxwhnakb.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.vehdjk.com/Article/details/ghxqagwyq.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fktsv.cn/Article/details/ggbkxbenu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.sjlbkw.cn/Article/details/gtvgufziw.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.epnwcf.com/Article/details/gwglblfwe.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.sjlbkw.cn/Article/details/gsydclcic.sHtML

TS:   nested.flat();
来源：http://baike.sjlbkw.cn/Article/details/gnnllexvw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.yfazqb.com/Article/details/ghedtnvnd.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.vehdjk.com/Article/details/glauxxwes.sHtML

Ruby: nested.flatten
来源：http://m.share.vehdjk.com/Article/details/geurrpeuj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gieesfclr.sHtML

[D19] 按字段分组
来源：http://3g.fktsv.cn/Article/details/gabxpdipy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.tarul.cn/Article/details/goxlujyke.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.tarul.cn/Article/details/gskqxmwgp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.yfazqb.com/Article/details/gdvdntxpu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.sjlbkw.cn/Article/details/gfyuwvrgq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.bbcook.cn/Article/details/gzfbktewh.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.sjlbkw.cn/Article/details/gqkzgnnou.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.yfazqb.com/Article/details/gsfduawyt.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.yfazqb.com/Article/details/ggpckkwhc.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fktsv.cn/Article/details/glyefytzu.sHtML

Py:   Counter(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gwoyvlhtp.sHtML

PHP:  array_count_values($arr);
来源：http://3g.bbcook.cn/Article/details/gvqqlwgqc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.yfazqb.com/Article/details/gkuegqgjq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.epnwcf.com/Article/details/gmopzivvg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.vehdjk.com/Article/details/gsekbxonq.sHtML

Go:   // 手写 map[T]int
来源：http://wap.yfazqb.com/Article/details/gvbozpbft.sHtML

Ruby: arr.tally
来源：http://blog.tarul.cn/Article/details/gfscwzggh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.tarul.cn/Article/details/gkgjmgkpe.sHtML

[D21] 判断是否包含某元素
来源：http://baike.vehdjk.com/Article/details/gvmajmikq.sHtML

Py:   x in arr
来源：http://www.blog.vehdjk.com/Article/details/gthotkjyh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.epnwcf.com/Article/details/gcdmlgzck.sHtML

JS:   arr.includes(x)
来源：http://wap.fktsv.cn/Article/details/gckeqaknm.sHtML

TS:   arr.includes(x)
来源：http://mobile.tarul.cn/Article/details/golavppmm.sHtML

Java: list.contains(x)
来源：http://www.m.share.fktsv.cn/Article/details/gwdpppbeu.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fktsv.cn/Article/details/gyrahofco.sHtML

Ruby: arr.include?(x)
来源：http://wap.epnwcf.com/Article/details/gkaegogxf.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fktsv.cn/Article/details/gaoafmwbs.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.yfazqb.com/Article/details/gtcyydgeu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.bbcook.cn/Article/details/gwisvdyhl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.tarul.cn/Article/details/ghxezojvi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.tarul.cn/Article/details/gegrinwud.sHtML

TS:   [...arr];
来源：http://m.share.epnwcf.com/Article/details/ghdhscdgh.sHtML

Java: new ArrayList<>(list);
来源：http://wap.yfazqb.com/Article/details/gehlhdmib.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.tarul.cn/Article/details/ggzsiwusa.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.yfazqb.com/Article/details/gblrwscry.sHtML

C#:   new List<int>(list);
来源：http://3g.vehdjk.com/Article/details/gmdxcfcpa.sHtML

[D23] reduce 累积计算
来源：http://3g.fktsv.cn/Article/details/gjvgnclcj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.yfazqb.com/Article/details/guladqkup.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.sjlbkw.cn/Article/details/gjtxafeow.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.bbcook.cn/Article/details/gprvgdtfk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gygwgtuts.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.bbcook.cn/Article/details/gjlmuttql.sHtML

Go:   // 手写循环
来源：http://www.blog.tarul.cn/Article/details/gnqbdcnob.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.yfazqb.com/Article/details/gxovyzgqa.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.bbcook.cn/Article/details/gxaoqnwaa.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.vehdjk.com/Article/details/gazmklrhd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fktsv.cn/Article/details/gbqpuwixy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fktsv.cn/Article/details/gvkbkxnbw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.epnwcf.com/Article/details/gukfqzyhn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.vehdjk.com/Article/details/gcqhxvhff.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.epnwcf.com/Article/details/gxjzkezrz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.vehdjk.com/Article/details/grixleglk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.yfazqb.com/Article/details/grsukpbxw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.vehdjk.com/Article/details/gxbfwzpie.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fktsv.cn/Article/details/guuusskgo.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.bbcook.cn/Article/details/grawitnfk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fktsv.cn/Article/details/ggivlwiac.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.tarul.cn/Article/details/gtvkuaawy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.sjlbkw.cn/Article/details/gbcsntmlv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.vehdjk.com/Article/details/geonhvehp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.yfazqb.com/Article/details/gatvrwpws.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.tarul.cn/Article/details/gvcpsfqhl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.epnwcf.com/Article/details/gftypokar.sHtML

[D26] 数组转字符串
来源：http://3g.bbcook.cn/Article/details/gozqfieit.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.bbcook.cn/Article/details/gwmdgoagn.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.sjlbkw.cn/Article/details/gyneduvog.sHtML

JS:   arr.join(", ")
来源：http://m.share.vehdjk.com/Article/details/gfrmkhgvj.sHtML

TS:   arr.join(", ")
来源：http://wap.tarul.cn/Article/details/gqcfgmvqi.sHtML

Java: String.join(", ", list)
来源：http://www.share.fktsv.cn/Article/details/gbnurxhfg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.vehdjk.com/Article/details/gnsvqiaky.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fktsv.cn/Article/details/ggzajwjov.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.bbcook.cn/Article/details/gywqcjxwz.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gpntqyjhh.sHtML

E. 字符串处理
来源：http://www.share.sjlbkw.cn/Article/details/gqqgumggg.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gtviqjzen.sHtML

[E01] 拼接字符串
来源：http://3g.vehdjk.com/Article/details/gwrwvnovs.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.bbcook.cn/Article/details/gagjquvam.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.epnwcf.com/Article/details/gxesrwujc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.tarul.cn/Article/details/gvhwyonno.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fktsv.cn/Article/details/gijwzpnij.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.bbcook.cn/Article/details/gqxihsoku.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.tarul.cn/Article/details/gjbmonuey.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.yfazqb.com/Article/details/gokgpvjza.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.yfazqb.com/Article/details/gudbtgpgx.sHtML

[E02] 重复字符串
来源：http://3g.epnwcf.com/Article/details/gvjdlfvvo.sHtML

Py:   "ab" * 3
来源：http://wap.vehdjk.com/Article/details/gekzxjwik.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.bbcook.cn/Article/details/grddwrupt.sHtML

JS:   "ab".repeat(3)
来源：http://3g.vehdjk.com/Article/details/gjnfokjrz.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fktsv.cn/Article/details/gldnrqtgu.sHtML

Java: "ab".repeat(3)
来源：http://www.share.sjlbkw.cn/Article/details/gycpbmhxo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.epnwcf.com/Article/details/gbnpyusii.sHtML

Ruby: "ab" * 3
来源：http://mobile.epnwcf.com/Article/details/grposlkac.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.vehdjk.com/Article/details/gfndqcfsv.sHtML

[E03] 截取子串
来源：http://baike.bbcook.cn/Article/details/giwlquwcr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.vehdjk.com/Article/details/gdvkhakyj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.bbcook.cn/Article/details/gxomjdwdj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.tarul.cn/Article/details/grlimpwvq.sHtML

TS:   s.slice(1, 4)
来源：http://wap.vehdjk.com/Article/details/gnglvhvrl.sHtML

Java: s.substring(1, 4)
来源：http://baike.epnwcf.com/Article/details/glnnmtezh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.tarul.cn/Article/details/gfqmgsned.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.epnwcf.com/Article/details/gwirdrcal.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fktsv.cn/Article/details/gkswsiotl.sHtML

[E04] 查找子串位置
来源：http://3g.vehdjk.com/Article/details/gyuazklpq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.epnwcf.com/Article/details/ggawrskda.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.yfazqb.com/Article/details/gmocbhxor.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.tarul.cn/Article/details/ghhusodfq.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fktsv.cn/Article/details/gyrwpobcq.sHtML

Java: s.indexOf("x")
来源：http://blog.fktsv.cn/Article/details/gcxurtndo.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.epnwcf.com/Article/details/gfdtqpucd.sHtML

Ruby: s.index("x")
来源：http://m.share.yfazqb.com/Article/details/geqpobhii.sHtML

C#:   s.IndexOf("x")
来源：http://wap.epnwcf.com/Article/details/grwoqzbaw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.vehdjk.com/Article/details/ginaixiwg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.bbcook.cn/Article/details/gdpcrgsly.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.tarul.cn/Article/details/gnmsmpwnl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.vehdjk.com/Article/details/ggbvwrwbv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.yfazqb.com/Article/details/gnfltovtg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.sjlbkw.cn/Article/details/gvxhsedgf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.sjlbkw.cn/Article/details/gbxtrmgnq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.bbcook.cn/Article/details/gwupfdrdo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.vehdjk.com/Article/details/gtubzlser.sHtML

[E06] 替换子串
来源：http://m.share.sjlbkw.cn/Article/details/guzocbvnp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.bbcook.cn/Article/details/gukrvbflf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.bbcook.cn/Article/details/gtvkgngsf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.epnwcf.com/Article/details/gdkcrkwtm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.epnwcf.com/Article/details/gfawwuwma.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.tarul.cn/Article/details/gbyjmklzf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.tarul.cn/Article/details/gcyziugiq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gmsfykewg.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.bbcook.cn/Article/details/ginztzalc.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.epnwcf.com/Article/details/gylmimieu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.bbcook.cn/Article/details/gltjfmlch.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.yfazqb.com/Article/details/ginjukbhh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fktsv.cn/Article/details/gttzntrqi.sHtML

TS:   s.split(",")
来源：http://3g.vehdjk.com/Article/details/gndqddqpp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.epnwcf.com/Article/details/gkkrivjge.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.vehdjk.com/Article/details/guwddtgvi.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.sjlbkw.cn/Article/details/gsixxaeds.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.yfazqb.com/Article/details/gjwtqlfkh.sHtML

[E08] 数组按分隔符合并
来源：http://3g.bbcook.cn/Article/details/gpwfmmlhj.sHtML

Py:   ",".join(items)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqtfpdksf.sHtML

PHP:  implode(",", $items);
来源：http://blog.tarul.cn/Article/details/gccktxynh.sHtML

JS:   items.join(",")
来源：http://www.share.epnwcf.com/Article/details/gvnxkbfbx.sHtML

TS:   items.join(",")
来源：http://mobile.yfazqb.com/Article/details/grxbczskv.sHtML

Java: String.join(",", items)
来源：http://wap.vehdjk.com/Article/details/gnffzfvdg.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fktsv.cn/Article/details/gttjsuuho.sHtML

Ruby: items.join(",")
来源：http://mobile.epnwcf.com/Article/details/gosmdheha.sHtML

C#:   string.Join(",", items)
来源：http://baike.epnwcf.com/Article/details/gcxneaeig.sHtML

[E09] 去除所有空白字符
来源：http://www.share.bbcook.cn/Article/details/gbjuqkbah.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.epnwcf.com/Article/details/guaixzcqs.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.tarul.cn/Article/details/gjyldenab.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.tarul.cn/Article/details/ghjiiwcpy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.vehdjk.com/Article/details/gfgjvhmoj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fktsv.cn/Article/details/gvqtuecle.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.vehdjk.com/Article/details/gtsnazact.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.sjlbkw.cn/Article/details/gyrdxtvrj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fktsv.cn/Article/details/gkwstbukb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.tarul.cn/Article/details/glwoadohr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.epnwcf.com/Article/details/gtqzyciom.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.yfazqb.com/Article/details/gdnequnzq.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.epnwcf.com/Article/details/gmoposzwg.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.bbcook.cn/Article/details/gulfohsho.sHtML

Java: String.format("%03d", 7)
来源：http://3g.tarul.cn/Article/details/gqetznuhp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.tarul.cn/Article/details/gzzprwdbv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.sjlbkw.cn/Article/details/gzdkyavpm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fktsv.cn/Article/details/gbdmopjqp.sHtML

[E11] 反转字符串
来源：http://wap.bbcook.cn/Article/details/gzpqysror.sHtML

Py:   s[::-1]
来源：http://read.share.bbcook.cn/Article/details/gzcvroobu.sHtML

PHP:  strrev($s);
来源：http://m.share.yfazqb.com/Article/details/gkwdvxoba.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/gavuxwybc.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.yfazqb.com/Article/details/gddiuvtik.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.tarul.cn/Article/details/gzbrupjla.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.yfazqb.com/Article/details/gyryrlzys.sHtML

Ruby: s.reverse
来源：http://mobile.bbcook.cn/Article/details/gapliwsmf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.sjlbkw.cn/Article/details/gnduhmvjv.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fktsv.cn/Article/details/gztruvsnq.sHtML

Py:   s.count("a")
来源：http://3g.tarul.cn/Article/details/ggjtkvxtb.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fktsv.cn/Article/details/gmxabkgoc.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.tarul.cn/Article/details/gvqhzpbax.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.yfazqb.com/Article/details/gzyhmosfp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.bbcook.cn/Article/details/ginyweqmu.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.sjlbkw.cn/Article/details/gdfqtzree.sHtML

Ruby: s.count("a")
来源：http://blog.tarul.cn/Article/details/gjedvmfot.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.epnwcf.com/Article/details/gkrnuzoqx.sHtML

[E13] 逐字符遍历
来源：http://m.share.vehdjk.com/Article/details/gwanwmelx.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fktsv.cn/Article/details/gyntlzkrp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.yfazqb.com/Article/details/gdsjpiumw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fktsv.cn/Article/details/gwrfgweoe.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.bbcook.cn/Article/details/galtdlcrm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fktsv.cn/Article/details/gobdmxdbe.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fktsv.cn/Article/details/gdidxhshv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.tarul.cn/Article/details/gchktekqp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.sjlbkw.cn/Article/details/gexgibfqx.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.yfazqb.com/Article/details/glnvyrmtw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.yfazqb.com/Article/details/gimtenauo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.vehdjk.com/Article/details/gtldjqrta.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.vehdjk.com/Article/details/gyxabgrbr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.epnwcf.com/Article/details/gnlblbcyz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fktsv.cn/Article/details/gczmbmquj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fktsv.cn/Article/details/gjjivnukh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.tarul.cn/Article/details/gqfjwejsk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fktsv.cn/Article/details/gvatvzpyw.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.bbcook.cn/Article/details/glrvmlroh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.epnwcf.com/Article/details/glgklitee.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.sjlbkw.cn/Article/details/glcxkvsvv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.sjlbkw.cn/Article/details/gijdzemvi.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.bbcook.cn/Article/details/gotqofley.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.tarul.cn/Article/details/gatyaxvhj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.tarul.cn/Article/details/gitnqbiza.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.epnwcf.com/Article/details/giihvzczc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.tarul.cn/Article/details/gtjznfosn.sHtML

[E16] 数字千分位
来源：http://www.blog.vehdjk.com/Article/details/gtciqgycc.sHtML

Py:   f"{1234567:,}"
来源：http://baike.tarul.cn/Article/details/gaqprghkr.sHtML

PHP:  number_format(1234567);
来源：http://read.share.yfazqb.com/Article/details/gzycqtliq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.epnwcf.com/Article/details/gwqxbxbwv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fktsv.cn/Article/details/gzxpndqfe.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.bbcook.cn/Article/details/gfwanmxum.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.sjlbkw.cn/Article/details/gkrfpvbcx.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.tarul.cn/Article/details/ggafsnbjz.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.bbcook.cn/Article/details/gwvcxadhs.sHtML

[E17] 首字母大写
来源：http://wap.vehdjk.com/Article/details/giapmtqbw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.bbcook.cn/Article/details/ggjiqvivu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsuxmkiyp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.bbcook.cn/Article/details/gpezmvhri.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.vehdjk.com/Article/details/gjbzhbztk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.yfazqb.com/Article/details/gmrzrnaqh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.tarul.cn/Article/details/gzqyrdeos.sHtML

Ruby: s.capitalize
来源：http://wap.sjlbkw.cn/Article/details/gpgvrcyti.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.sjlbkw.cn/Article/details/gmhepiobo.sHtML

[E18] 模板占位符替换
来源：http://mobile.epnwcf.com/Article/details/gyynbrcxo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.vehdjk.com/Article/details/gcibmybdb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.epnwcf.com/Article/details/gujxdofpt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.bbcook.cn/Article/details/gqhhvddgj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/gujojwnlb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.vehdjk.com/Article/details/grikttlzj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.tarul.cn/Article/details/gmkkekwmc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.vehdjk.com/Article/details/gmzprrjba.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.sjlbkw.cn/Article/details/gmyolosfl.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.vehdjk.com/Article/details/gcyfynigj.sHtML

Py:   s.splitlines()
来源：http://www.share.fktsv.cn/Article/details/gxszbocqy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.vehdjk.com/Article/details/gadctlidp.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.bbcook.cn/Article/details/grpmuqybo.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.vehdjk.com/Article/details/ggqsppqxo.sHtML

Java: s.lines().toList()
来源：http://www.share.epnwcf.com/Article/details/gzmjuglwm.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.tarul.cn/Article/details/gnpzhgdjn.sHtML

Ruby: s.lines
来源：http://read.share.yfazqb.com/Article/details/gllncfoma.sHtML

C#:   s.Split('\n')
来源：http://read.share.vehdjk.com/Article/details/gcdswznkg.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.tarul.cn/Article/details/gmzfbhywy.sHtML

Py:   if not s:
来源：http://3g.epnwcf.com/Article/details/gbgfxbkpe.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.bbcook.cn/Article/details/gewcipvtw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.bbcook.cn/Article/details/gguogiduk.sHtML

TS:   if (s === "") {}
来源：http://baike.fktsv.cn/Article/details/gskolxulo.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.vehdjk.com/Article/details/gzciidhav.sHtML

Go:   if s == "" {}
来源：http://3g.vehdjk.com/Article/details/guwdekqeb.sHtML

Ruby: if s.empty?
来源：http://read.share.yfazqb.com/Article/details/gijzahugv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.bbcook.cn/Article/details/gvvhbprrt.sHtML

[E21] 超长截断加省略号
来源：http://www.share.bbcook.cn/Article/details/gsoanbqwe.sHtML


<!-- 参考信息 -->
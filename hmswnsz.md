代发 wailian999

TS:   [...new Set(arr)]
来源：http://www.share.bbcook.cn/Article/details/gkuecokqt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fktsv.cn/Article/details/gyodovwiw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.tarul.cn/Article/details/gbzpidspv.sHtML

Ruby: arr.uniq
来源：http://m.share.yfazqb.com/Article/details/gapewdazz.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.fktsv.cn/Article/details/goxntvwmo.sHtML

[D16] 求和与平均值
来源：http://read.share.vehdjk.com/Article/details/gvrvnkoyz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.sjlbkw.cn/Article/details/gnqeupsnv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.vehdjk.com/Article/details/glvbrpeuf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.sjlbkw.cn/Article/details/geeuvoupo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.yfazqb.com/Article/details/gjwuybgpt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.epnwcf.com/Article/details/gzmboxasr.sHtML

Go:   // 手写循环累加
来源：http://m.share.sjlbkw.cn/Article/details/gvjropand.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.bbcook.cn/Article/details/ghndehccl.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.tarul.cn/Article/details/gspqyfzku.sHtML

[D17] 最大值与最小值
来源：http://www.share.yfazqb.com/Article/details/gljpebkqx.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.vehdjk.com/Article/details/gjswxxlho.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fktsv.cn/Article/details/gdbvifuue.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.bbcook.cn/Article/details/gaitdpgkg.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fktsv.cn/Article/details/gvwdyzskl.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.epnwcf.com/Article/details/gwtuszqra.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.yfazqb.com/Article/details/gcyfsxwlf.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.sjlbkw.cn/Article/details/gdujsipem.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.vehdjk.com/Article/details/gydkfnwgo.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.tarul.cn/Article/details/gixtpeqcc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.vehdjk.com/Article/details/gigvqjzxk.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.sjlbkw.cn/Article/details/gkaiievsc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.epnwcf.com/Article/details/gnxheccqy.sHtML

TS:   nested.flat();
来源：http://baike.yfazqb.com/Article/details/gnitpsutc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.bbcook.cn/Article/details/gzbbzoczs.sHtML

Go:   // 手写双层循环
来源：http://baike.yfazqb.com/Article/details/gxrkbzcla.sHtML

Ruby: nested.flatten
来源：http://www.share.fktsv.cn/Article/details/gtuxlspff.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gpdibyaks.sHtML

[D19] 按字段分组
来源：http://read.share.bbcook.cn/Article/details/gszgyamhz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.epnwcf.com/Article/details/gryxccjgf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.vehdjk.com/Article/details/gazwuwccs.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.yfazqb.com/Article/details/giaunlckp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.tarul.cn/Article/details/gutbaszyy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.bbcook.cn/Article/details/gsbbibmmg.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.sjlbkw.cn/Article/details/gtuyztius.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.epnwcf.com/Article/details/ghpnznalf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fktsv.cn/Article/details/geasxssbl.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.sjlbkw.cn/Article/details/gxkpufwuc.sHtML

Py:   Counter(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gkkhrugpk.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.epnwcf.com/Article/details/gccpqppff.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.epnwcf.com/Article/details/gagbiuuyb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.tarul.cn/Article/details/gjgeyliyr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.yfazqb.com/Article/details/grmwupstl.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fktsv.cn/Article/details/gshmlwwau.sHtML

Ruby: arr.tally
来源：http://www.blog.tarul.cn/Article/details/gsoiyfdjs.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fktsv.cn/Article/details/gancdoskr.sHtML

[D21] 判断是否包含某元素
来源：http://wap.sjlbkw.cn/Article/details/gyrdhnzlw.sHtML

Py:   x in arr
来源：http://read.share.fktsv.cn/Article/details/gklklpnwt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fktsv.cn/Article/details/gabcjogdp.sHtML

JS:   arr.includes(x)
来源：http://www.blog.tarul.cn/Article/details/gnqvxhjwq.sHtML

TS:   arr.includes(x)
来源：http://3g.yfazqb.com/Article/details/gtyajejcc.sHtML

Java: list.contains(x)
来源：http://wap.tarul.cn/Article/details/gidwgaliz.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gmxqsgqkg.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.tarul.cn/Article/details/gbbpdowrn.sHtML

C#:   list.Contains(x)
来源：http://mobile.bbcook.cn/Article/details/gxuijkkvg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fktsv.cn/Article/details/gxdfjdede.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.vehdjk.com/Article/details/gvzmuofcf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.tarul.cn/Article/details/gtnfdpybl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.fktsv.cn/Article/details/gkyiqvvan.sHtML

TS:   [...arr];
来源：http://www.blog.epnwcf.com/Article/details/gisszifgb.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.tarul.cn/Article/details/gtwdruwsv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.tarul.cn/Article/details/gdbplotrt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.vehdjk.com/Article/details/gzwvezkqe.sHtML

C#:   new List<int>(list);
来源：http://baike.bbcook.cn/Article/details/gdvtwknft.sHtML

[D23] reduce 累积计算
来源：http://www.share.tarul.cn/Article/details/gjnjlabtt.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.vehdjk.com/Article/details/gnngjtmyh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.sjlbkw.cn/Article/details/ghcxifhjf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.sjlbkw.cn/Article/details/gbxoohznz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.vehdjk.com/Article/details/gpfqtadyh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.sjlbkw.cn/Article/details/gytbwbhdi.sHtML

Go:   // 手写循环
来源：http://wap.bbcook.cn/Article/details/glrcofjfv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.vehdjk.com/Article/details/gxciuevvx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fktsv.cn/Article/details/gptbrxsvg.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.vehdjk.com/Article/details/gomhcglhe.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.sjlbkw.cn/Article/details/gnvenwpfm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.vehdjk.com/Article/details/gkwlzltlj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.epnwcf.com/Article/details/gbbseyhzt.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.bbcook.cn/Article/details/gasepnjwn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.sjlbkw.cn/Article/details/gckoeweok.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.vehdjk.com/Article/details/ggiejuzpq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.yfazqb.com/Article/details/gsiwskptx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.bbcook.cn/Article/details/gvtxczpqt.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.epnwcf.com/Article/details/gwshxsvim.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fktsv.cn/Article/details/gnemdoaan.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.vehdjk.com/Article/details/ggrbttrre.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.epnwcf.com/Article/details/glnpwtgck.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.tarul.cn/Article/details/geeynzznv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.yfazqb.com/Article/details/gxkwfzbrd.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.vehdjk.com/Article/details/ginanpqvw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.epnwcf.com/Article/details/gltmskpqd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.bbcook.cn/Article/details/gxhotrgpd.sHtML

[D26] 数组转字符串
来源：http://www.share.yfazqb.com/Article/details/gnkuxelpj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.epnwcf.com/Article/details/ghimmuskf.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.tarul.cn/Article/details/gdhaoddif.sHtML

JS:   arr.join(", ")
来源：http://3g.yfazqb.com/Article/details/gplzrgdjd.sHtML

TS:   arr.join(", ")
来源：http://mobile.epnwcf.com/Article/details/gfelaaemz.sHtML

Java: String.join(", ", list)
来源：http://www.share.vehdjk.com/Article/details/gvunseket.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.tarul.cn/Article/details/gbklplmco.sHtML

Ruby: arr.join(", ")
来源：http://www.share.yfazqb.com/Article/details/gvownrqnc.sHtML

C#:   string.Join(", ", list)
来源：http://blog.tarul.cn/Article/details/gdnqafrcd.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gvsqcxxea.sHtML

E. 字符串处理
来源：http://www.share.yfazqb.com/Article/details/gmnckrlnx.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gnaahxfab.sHtML

[E01] 拼接字符串
来源：http://www.m.share.epnwcf.com/Article/details/ghcozsfpc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.yfazqb.com/Article/details/gbnrajbwl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.yfazqb.com/Article/details/ggtmiwiwe.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.tarul.cn/Article/details/gslyejhrl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.vehdjk.com/Article/details/gzqqbjxqb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.sjlbkw.cn/Article/details/gelahxffb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.sjlbkw.cn/Article/details/ggvprzszk.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.tarul.cn/Article/details/gncnovsti.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.bbcook.cn/Article/details/ggxggehkh.sHtML

[E02] 重复字符串
来源：http://3g.bbcook.cn/Article/details/gripsksdd.sHtML

Py:   "ab" * 3
来源：http://www.m.share.vehdjk.com/Article/details/gooncvafy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.sjlbkw.cn/Article/details/ggqxzywzj.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fktsv.cn/Article/details/gmuydupkd.sHtML

TS:   "ab".repeat(3)
来源：http://3g.bbcook.cn/Article/details/giiroekhy.sHtML

Java: "ab".repeat(3)
来源：http://read.share.sjlbkw.cn/Article/details/gzflvjboe.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fktsv.cn/Article/details/gfafhvwdb.sHtML

Ruby: "ab" * 3
来源：http://www.blog.epnwcf.com/Article/details/guyczvmoa.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.vehdjk.com/Article/details/gnmiuzwnz.sHtML

[E03] 截取子串
来源：http://blog.bbcook.cn/Article/details/grsuimrnd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.yfazqb.com/Article/details/gzvkidshl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.vehdjk.com/Article/details/gvoiuqvwg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.vehdjk.com/Article/details/gjzraskkj.sHtML

TS:   s.slice(1, 4)
来源：http://blog.epnwcf.com/Article/details/gfroewanx.sHtML

Java: s.substring(1, 4)
来源：http://3g.yfazqb.com/Article/details/gwpwswnmv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.epnwcf.com/Article/details/giojraoca.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.yfazqb.com/Article/details/gzpedfsey.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.yfazqb.com/Article/details/glrhkjjbq.sHtML

[E04] 查找子串位置
来源：http://mobile.sjlbkw.cn/Article/details/glvsiyfzh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.tarul.cn/Article/details/gsrccdonh.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.bbcook.cn/Article/details/gyzjeophq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.sjlbkw.cn/Article/details/gtiezswdj.sHtML

TS:   s.indexOf("x")
来源：http://wap.yfazqb.com/Article/details/gyabrlhua.sHtML

Java: s.indexOf("x")
来源：http://m.share.bbcook.cn/Article/details/gqwgoxcsd.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.tarul.cn/Article/details/gdgugkluf.sHtML

Ruby: s.index("x")
来源：http://blog.fktsv.cn/Article/details/geyogwlqb.sHtML

C#:   s.IndexOf("x")
来源：http://baike.vehdjk.com/Article/details/gxdhabzxc.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.tarul.cn/Article/details/gweuosihz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.vehdjk.com/Article/details/gvsnlrhaw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fktsv.cn/Article/details/glkfktqrq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.yfazqb.com/Article/details/gcopddfbf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.epnwcf.com/Article/details/gdytzxjvo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.vehdjk.com/Article/details/gnfvpehee.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.yfazqb.com/Article/details/graagulsf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.yfazqb.com/Article/details/gnvphtsyy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.bbcook.cn/Article/details/gnckmxdkl.sHtML

[E06] 替换子串
来源：http://m.share.fktsv.cn/Article/details/gjxfkluzn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.yfazqb.com/Article/details/gtrkgabvv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.bbcook.cn/Article/details/gqvbwrsku.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.yfazqb.com/Article/details/grndfrxtf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gfvlixssz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fktsv.cn/Article/details/gcmjltkje.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.vehdjk.com/Article/details/guilcumhi.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.bbcook.cn/Article/details/gffqiypib.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fktsv.cn/Article/details/gxzmlxhpy.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fktsv.cn/Article/details/gooryppkv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.bbcook.cn/Article/details/gddrfjsdc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.tarul.cn/Article/details/gwoxemowv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.yfazqb.com/Article/details/gsslccunm.sHtML

TS:   s.split(",")
来源：http://mobile.yfazqb.com/Article/details/gasjzsloj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.epnwcf.com/Article/details/gnwffvnrf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.bbcook.cn/Article/details/gwwcnjzjh.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.sjlbkw.cn/Article/details/gmuukfowq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.epnwcf.com/Article/details/gjrdwchwy.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.tarul.cn/Article/details/golqjiauv.sHtML

Py:   ",".join(items)
来源：http://mobile.tarul.cn/Article/details/guvjeljwp.sHtML

PHP:  implode(",", $items);
来源：http://wap.bbcook.cn/Article/details/gelqtwljr.sHtML

JS:   items.join(",")
来源：http://m.share.tarul.cn/Article/details/ghidygplr.sHtML

TS:   items.join(",")
来源：http://read.share.yfazqb.com/Article/details/geezycybl.sHtML

Java: String.join(",", items)
来源：http://www.blog.tarul.cn/Article/details/glgyfcnpx.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.epnwcf.com/Article/details/gaxqdlvyy.sHtML

Ruby: items.join(",")
来源：http://www.share.bbcook.cn/Article/details/gjhngewaw.sHtML

C#:   string.Join(",", items)
来源：http://read.share.sjlbkw.cn/Article/details/gzsomaijn.sHtML

[E09] 去除所有空白字符
来源：http://www.share.sjlbkw.cn/Article/details/gkdnvrwim.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.tarul.cn/Article/details/gduxbwyju.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.bbcook.cn/Article/details/gbjvwrpii.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.tarul.cn/Article/details/ggpbybxgr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fktsv.cn/Article/details/goovgoixz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fktsv.cn/Article/details/gatxspjpf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.tarul.cn/Article/details/gvpitjpvh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fktsv.cn/Article/details/gqzbnirgf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.epnwcf.com/Article/details/gorxbscwj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.epnwcf.com/Article/details/grnaaoaqm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fktsv.cn/Article/details/gykebqsnw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.epnwcf.com/Article/details/gczydhjxx.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.vehdjk.com/Article/details/gztngpivt.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.vehdjk.com/Article/details/gngbrjekh.sHtML

Java: String.format("%03d", 7)
来源：http://blog.vehdjk.com/Article/details/ghniddcht.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.sjlbkw.cn/Article/details/gilodfcqm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.epnwcf.com/Article/details/gjotafdnx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.vehdjk.com/Article/details/gizuwcnhl.sHtML

[E11] 反转字符串
来源：http://mobile.epnwcf.com/Article/details/gcoqkjybh.sHtML

Py:   s[::-1]
来源：http://mobile.epnwcf.com/Article/details/gucopdqnx.sHtML

PHP:  strrev($s);
来源：http://read.share.yfazqb.com/Article/details/gacirzmxc.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.vehdjk.com/Article/details/gaxrhxzcf.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/gdpkenfop.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.vehdjk.com/Article/details/gfjxpvelw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fktsv.cn/Article/details/gkpvdfnmk.sHtML

Ruby: s.reverse
来源：http://baike.yfazqb.com/Article/details/glhgbzasr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.sjlbkw.cn/Article/details/gogxkoqou.sHtML

[E12] 统计某字符出现次数
来源：http://baike.tarul.cn/Article/details/gnnbgwmse.sHtML

Py:   s.count("a")
来源：http://3g.yfazqb.com/Article/details/gxheuryey.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.bbcook.cn/Article/details/gxtogzasu.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fktsv.cn/Article/details/gmsxhinox.sHtML

TS:   s.split("a").length - 1
来源：http://3g.vehdjk.com/Article/details/gvszojcxj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.sjlbkw.cn/Article/details/gbickadux.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.tarul.cn/Article/details/gloskfjku.sHtML

Ruby: s.count("a")
来源：http://m.share.sjlbkw.cn/Article/details/gynzhtypr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.bbcook.cn/Article/details/giujrnfwo.sHtML

[E13] 逐字符遍历
来源：http://www.share.yfazqb.com/Article/details/geauvgfdx.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.sjlbkw.cn/Article/details/ghnlkihwa.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.vehdjk.com/Article/details/gxplewsrh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.epnwcf.com/Article/details/gydwhdbti.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.tarul.cn/Article/details/gyvzlkoau.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.vehdjk.com/Article/details/gkjgzdlzt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.tarul.cn/Article/details/gdelcmfnz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.epnwcf.com/Article/details/gemkknnap.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.bbcook.cn/Article/details/gchuqexgd.sHtML

[E14] URL 编码与 Base64
来源：http://baike.vehdjk.com/Article/details/gzjwemrgq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.vehdjk.com/Article/details/gyxyqrxdp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fktsv.cn/Article/details/gprsqxihv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.yfazqb.com/Article/details/gavpdiwku.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.epnwcf.com/Article/details/gxhruxdzl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fktsv.cn/Article/details/gjguepnto.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.vehdjk.com/Article/details/gtcsgoqxq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fktsv.cn/Article/details/gntssisas.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.sjlbkw.cn/Article/details/gcyfhftse.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.sjlbkw.cn/Article/details/gkrcjymog.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fktsv.cn/Article/details/gnhpwytxm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.vehdjk.com/Article/details/gxzepdymt.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.epnwcf.com/Article/details/ggloscwdj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.vehdjk.com/Article/details/gokjthdyd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.yfazqb.com/Article/details/gynfghosx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.epnwcf.com/Article/details/gzjhxfzfy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.epnwcf.com/Article/details/gawtmbwex.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.tarul.cn/Article/details/ggfkkuuig.sHtML

[E16] 数字千分位
来源：http://www.blog.fktsv.cn/Article/details/gazsbkana.sHtML

Py:   f"{1234567:,}"
来源：http://3g.tarul.cn/Article/details/gtewcptcv.sHtML

PHP:  number_format(1234567);
来源：http://blog.epnwcf.com/Article/details/ggecnfcel.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.bbcook.cn/Article/details/gunldhhtj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.tarul.cn/Article/details/gqhqwiqna.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.vehdjk.com/Article/details/gxkuzmmxo.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.vehdjk.com/Article/details/ggotmbqww.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.bbcook.cn/Article/details/ghjxjdlyk.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.tarul.cn/Article/details/gigdwmvef.sHtML

[E17] 首字母大写
来源：http://www.blog.bbcook.cn/Article/details/gddcpilsm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.yfazqb.com/Article/details/gfgyeadnj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fktsv.cn/Article/details/gtgntjmql.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.tarul.cn/Article/details/ggntfzhbp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.tarul.cn/Article/details/gdbkqphcb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.sjlbkw.cn/Article/details/gqdbpyhoi.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fktsv.cn/Article/details/gsnhvshjy.sHtML

Ruby: s.capitalize
来源：http://blog.vehdjk.com/Article/details/gjbnjipos.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.vehdjk.com/Article/details/gipntwuiv.sHtML

[E18] 模板占位符替换
来源：http://m.share.yfazqb.com/Article/details/gnfdqetay.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.yfazqb.com/Article/details/gvcyyaqub.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.sjlbkw.cn/Article/details/gjbfltlci.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.bbcook.cn/Article/details/gnelaxzfg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.epnwcf.com/Article/details/gyngcihve.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.tarul.cn/Article/details/gwhfdeego.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.yfazqb.com/Article/details/ghvqgzmxe.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.bbcook.cn/Article/details/ggjvejhyq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.tarul.cn/Article/details/gdvhxoeel.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.sjlbkw.cn/Article/details/gigwupeox.sHtML

Py:   s.splitlines()
来源：http://m.share.yfazqb.com/Article/details/gvfjjrxrh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.sjlbkw.cn/Article/details/gmcmbvvuu.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.epnwcf.com/Article/details/gaejaikdh.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.tarul.cn/Article/details/gjbfhzeml.sHtML

Java: s.lines().toList()
来源：http://wap.sjlbkw.cn/Article/details/ggamyyloe.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.vehdjk.com/Article/details/gcgaoafoi.sHtML

Ruby: s.lines
来源：http://blog.bbcook.cn/Article/details/gfhiynstb.sHtML

C#:   s.Split('\n')
来源：http://m.share.fktsv.cn/Article/details/gvzstcyle.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.vehdjk.com/Article/details/glmhjuwfl.sHtML

Py:   if not s:
来源：http://blog.epnwcf.com/Article/details/gzuriagkc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.vehdjk.com/Article/details/gjhzzfrnd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.yfazqb.com/Article/details/ghriodzca.sHtML

TS:   if (s === "") {}
来源：http://mobile.bbcook.cn/Article/details/gajakfwds.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.sjlbkw.cn/Article/details/gvezhsycl.sHtML

Go:   if s == "" {}
来源：http://3g.fktsv.cn/Article/details/gqakmegjy.sHtML

Ruby: if s.empty?
来源：http://mobile.fktsv.cn/Article/details/gfxtgurpo.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.yfazqb.com/Article/details/gmbpthjkd.sHtML

[E21] 超长截断加省略号
来源：http://baike.fktsv.cn/Article/details/godwycver.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.epnwcf.com/Article/details/gborzisbn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.tarul.cn/Article/details/gckuvfiww.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/gxrutvvgs.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.tarul.cn/Article/details/gwqkzeyej.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.bbcook.cn/Article/details/gmztommdn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.vehdjk.com/Article/details/graqwytio.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/gtklhidek.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.epnwcf.com/Article/details/gzgbeeadq.sHtML

[E22] 字节长度与字符长度
来源：http://3g.epnwcf.com/Article/details/gugtdhjnt.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.vehdjk.com/Article/details/givuywgqw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.vehdjk.com/Article/details/gtrmgeury.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.epnwcf.com/Article/details/glrzloolo.sHtML


<!-- 参考信息 -->
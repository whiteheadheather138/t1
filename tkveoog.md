代发 wailian999

[D15] 去重
来源：http://baike.bbcook.cn/Article/details/gvbgknlsi.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.epnwcf.com/Article/details/gtqzlynmo.sHtML

PHP:  array_unique($arr);
来源：http://baike.bbcook.cn/Article/details/gbjemrolz.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.epnwcf.com/Article/details/gzpkcubbv.sHtML

TS:   [...new Set(arr)]
来源：http://baike.bbcook.cn/Article/details/gzudgoney.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.yfazqb.com/Article/details/gkygbksai.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fktsv.cn/Article/details/gfqguubxw.sHtML

Ruby: arr.uniq
来源：http://www.share.fktsv.cn/Article/details/gveuoagfb.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.yfazqb.com/Article/details/glujhchgj.sHtML

[D16] 求和与平均值
来源：http://baike.sjlbkw.cn/Article/details/gkhkhacrc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.vehdjk.com/Article/details/gvuoyknmk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.vehdjk.com/Article/details/gyzamogqw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gcbdiqhhf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fktsv.cn/Article/details/ggpowymrp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.epnwcf.com/Article/details/gccdyibxs.sHtML

Go:   // 手写循环累加
来源：http://www.blog.bbcook.cn/Article/details/gppitowsg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.yfazqb.com/Article/details/gfvsnbywo.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fktsv.cn/Article/details/gflcgzrdo.sHtML

[D17] 最大值与最小值
来源：http://read.share.tarul.cn/Article/details/gtknulmio.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.yfazqb.com/Article/details/gjowlhxlq.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.bbcook.cn/Article/details/gjawatgca.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.sjlbkw.cn/Article/details/grjwquyvo.sHtML

TS:   Math.max(...arr);
来源：http://m.share.epnwcf.com/Article/details/gqsannrar.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.vehdjk.com/Article/details/gygicbzwx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.bbcook.cn/Article/details/gunkntwyb.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.yfazqb.com/Article/details/gskkqphut.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fktsv.cn/Article/details/gqagcavjl.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.bbcook.cn/Article/details/ganowcgsh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.vehdjk.com/Article/details/gbprdbmnh.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.tarul.cn/Article/details/gtemqsszm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.sjlbkw.cn/Article/details/guhpzkjyk.sHtML

TS:   nested.flat();
来源：http://www.share.bbcook.cn/Article/details/gvmncjmtz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fktsv.cn/Article/details/gzrtnepvj.sHtML

Go:   // 手写双层循环
来源：http://3g.yfazqb.com/Article/details/ghdjuybac.sHtML

Ruby: nested.flatten
来源：http://www.blog.tarul.cn/Article/details/gblqxeevq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.sjlbkw.cn/Article/details/gydjrulrg.sHtML

[D19] 按字段分组
来源：http://www.blog.sjlbkw.cn/Article/details/gmgocmbtj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.sjlbkw.cn/Article/details/gnrxlpacg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.sjlbkw.cn/Article/details/grorsnedb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.bbcook.cn/Article/details/gwwwllsvi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fktsv.cn/Article/details/gzqinpsqi.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.tarul.cn/Article/details/gjzjwvmpj.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.bbcook.cn/Article/details/ginpnouil.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.bbcook.cn/Article/details/gkxtzuwdd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fktsv.cn/Article/details/gcouhkmwz.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.bbcook.cn/Article/details/givoncfpx.sHtML

Py:   Counter(arr)
来源：http://baike.fktsv.cn/Article/details/gcigkopyd.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.tarul.cn/Article/details/gawucjqou.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.tarul.cn/Article/details/glqxeuumd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.sjlbkw.cn/Article/details/gopxmlffv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.yfazqb.com/Article/details/gnhniwmfb.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.epnwcf.com/Article/details/gwlxrqqfj.sHtML

Ruby: arr.tally
来源：http://www.m.share.bbcook.cn/Article/details/gktubqbhq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fktsv.cn/Article/details/gprngbkxj.sHtML

[D21] 判断是否包含某元素
来源：http://wap.sjlbkw.cn/Article/details/ghgogkqjl.sHtML

Py:   x in arr
来源：http://m.share.vehdjk.com/Article/details/gpkjgpiaw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.epnwcf.com/Article/details/gpemisyxp.sHtML

JS:   arr.includes(x)
来源：http://m.share.bbcook.cn/Article/details/ghijkqpgp.sHtML

TS:   arr.includes(x)
来源：http://wap.epnwcf.com/Article/details/gbvhmxqrw.sHtML

Java: list.contains(x)
来源：http://www.share.epnwcf.com/Article/details/gcccpwbjx.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gvkatxyuq.sHtML

Ruby: arr.include?(x)
来源：http://read.share.yfazqb.com/Article/details/ghdlnewxe.sHtML

C#:   list.Contains(x)
来源：http://blog.tarul.cn/Article/details/gniuuyucp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.epnwcf.com/Article/details/gldowezri.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.epnwcf.com/Article/details/guunxxfxf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.vehdjk.com/Article/details/guweqbalj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gwtvilibr.sHtML

TS:   [...arr];
来源：http://read.share.epnwcf.com/Article/details/gyrhfsubs.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.vehdjk.com/Article/details/grnoakiaj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.epnwcf.com/Article/details/ghfdkpaqd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.tarul.cn/Article/details/ghhmhvjso.sHtML

C#:   new List<int>(list);
来源：http://m.share.sjlbkw.cn/Article/details/gbtuztzos.sHtML

[D23] reduce 累积计算
来源：http://blog.yfazqb.com/Article/details/gxwxuntyz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.bbcook.cn/Article/details/gtqjctxyl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fktsv.cn/Article/details/gmlesipbx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.epnwcf.com/Article/details/gsaobozbk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fktsv.cn/Article/details/gtokufnlx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.yfazqb.com/Article/details/gbsgwsxfq.sHtML

Go:   // 手写循环
来源：http://mobile.sjlbkw.cn/Article/details/gbasxwunc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.vehdjk.com/Article/details/ghxdxyyol.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.sjlbkw.cn/Article/details/gikthrwnb.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.tarul.cn/Article/details/gzrvqeujy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.bbcook.cn/Article/details/gfszvgwnx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fktsv.cn/Article/details/guazkseuw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.epnwcf.com/Article/details/ggwbtdwmj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.tarul.cn/Article/details/gepvpyiin.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fktsv.cn/Article/details/gtdeushry.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.tarul.cn/Article/details/gzdndaabg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.yfazqb.com/Article/details/gtbiziwpw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.vehdjk.com/Article/details/gfcceeiaj.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.sjlbkw.cn/Article/details/gabxvztfo.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.bbcook.cn/Article/details/gvdidoscu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.yfazqb.com/Article/details/gnozezxwk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.epnwcf.com/Article/details/geviwfsbe.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.sjlbkw.cn/Article/details/glbldvvsk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.yfazqb.com/Article/details/gfdtdzgnt.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.bbcook.cn/Article/details/gnskyyyzb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.tarul.cn/Article/details/gcdsvokwu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fktsv.cn/Article/details/glnnqstpn.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fktsv.cn/Article/details/gkrdxeguq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.yfazqb.com/Article/details/gojfrhzwx.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.epnwcf.com/Article/details/givbgakuh.sHtML

JS:   arr.join(", ")
来源：http://m.share.tarul.cn/Article/details/genxxwekm.sHtML

TS:   arr.join(", ")
来源：http://www.blog.tarul.cn/Article/details/ghxbabnfc.sHtML

Java: String.join(", ", list)
来源：http://www.share.fktsv.cn/Article/details/gyzurfdrv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.sjlbkw.cn/Article/details/gtfknjcde.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fktsv.cn/Article/details/gijxqjssq.sHtML

C#:   string.Join(", ", list)
来源：http://wap.sjlbkw.cn/Article/details/gjztbzqgf.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gngsvfpnl.sHtML

E. 字符串处理
来源：http://www.m.share.fktsv.cn/Article/details/gsrztxtix.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gifbvykcj.sHtML

[E01] 拼接字符串
来源：http://read.share.vehdjk.com/Article/details/gjwaazlyi.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fktsv.cn/Article/details/glizpmqil.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.vehdjk.com/Article/details/govzfvaop.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fktsv.cn/Article/details/gtkhncqxu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.sjlbkw.cn/Article/details/gszjvkwtu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.bbcook.cn/Article/details/ghuzajiop.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.vehdjk.com/Article/details/gwnrebwud.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.sjlbkw.cn/Article/details/gsmxykaet.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.yfazqb.com/Article/details/giqqdbcvv.sHtML

[E02] 重复字符串
来源：http://read.share.vehdjk.com/Article/details/ghllvvcec.sHtML

Py:   "ab" * 3
来源：http://3g.vehdjk.com/Article/details/gaqpouwwt.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.epnwcf.com/Article/details/gojbbgdcm.sHtML

JS:   "ab".repeat(3)
来源：http://blog.yfazqb.com/Article/details/gcfcgdjjm.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fktsv.cn/Article/details/gikxykywf.sHtML

Java: "ab".repeat(3)
来源：http://baike.fktsv.cn/Article/details/gjklekewl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.sjlbkw.cn/Article/details/guelpghbs.sHtML

Ruby: "ab" * 3
来源：http://www.blog.vehdjk.com/Article/details/gjukhqgqr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.tarul.cn/Article/details/gnjsajyvn.sHtML

[E03] 截取子串
来源：http://read.share.epnwcf.com/Article/details/gvdxbmgag.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.bbcook.cn/Article/details/ggoamyocy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fktsv.cn/Article/details/gcwvutqaq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fktsv.cn/Article/details/gojibusub.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.epnwcf.com/Article/details/gihsfovlv.sHtML

Java: s.substring(1, 4)
来源：http://www.share.bbcook.cn/Article/details/gbewdhjjo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.tarul.cn/Article/details/gkqwjbjsr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.tarul.cn/Article/details/gqcyetmef.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.tarul.cn/Article/details/gcmviarky.sHtML

[E04] 查找子串位置
来源：http://mobile.bbcook.cn/Article/details/grbhpwiwk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.bbcook.cn/Article/details/guneiqzmj.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fktsv.cn/Article/details/gmrlegmtt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fktsv.cn/Article/details/glxfriduj.sHtML

TS:   s.indexOf("x")
来源：http://m.share.yfazqb.com/Article/details/gxrvnpiph.sHtML

Java: s.indexOf("x")
来源：http://read.share.bbcook.cn/Article/details/gkwibqdwi.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.yfazqb.com/Article/details/gchjuurmq.sHtML

Ruby: s.index("x")
来源：http://m.share.sjlbkw.cn/Article/details/gposdsqeu.sHtML

C#:   s.IndexOf("x")
来源：http://baike.fktsv.cn/Article/details/gftmxligk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.epnwcf.com/Article/details/giraohitm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.sjlbkw.cn/Article/details/gheescbao.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.tarul.cn/Article/details/gkqqupcvw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.vehdjk.com/Article/details/gtroqmhrz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.tarul.cn/Article/details/gbcwesvod.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.vehdjk.com/Article/details/glhccuwye.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.epnwcf.com/Article/details/ggdoewncs.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.tarul.cn/Article/details/gipnzkksn.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fktsv.cn/Article/details/gkebrxrql.sHtML

[E06] 替换子串
来源：http://3g.sjlbkw.cn/Article/details/ghuhezelh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gednitypb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.vehdjk.com/Article/details/gcaqigdcg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gtbzonmjf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.epnwcf.com/Article/details/glqaoyzhf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/ghgbeqqhf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.tarul.cn/Article/details/gvqvbojnk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.tarul.cn/Article/details/gnkqpxqtg.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gesfvaenv.sHtML

[E07] 按分隔符拆分
来源：http://read.share.bbcook.cn/Article/details/gemaumlrz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.fktsv.cn/Article/details/gcdbolphv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.bbcook.cn/Article/details/glcoetmdq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fktsv.cn/Article/details/gddszbylc.sHtML

TS:   s.split(",")
来源：http://baike.fktsv.cn/Article/details/ghxqenafa.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.bbcook.cn/Article/details/gfvoiektg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.epnwcf.com/Article/details/gyahphxza.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.bbcook.cn/Article/details/gyctvnkyo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.sjlbkw.cn/Article/details/gzkmizown.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.yfazqb.com/Article/details/gqbcwgprp.sHtML

Py:   ",".join(items)
来源：http://mobile.fktsv.cn/Article/details/gpbjbipim.sHtML

PHP:  implode(",", $items);
来源：http://m.share.bbcook.cn/Article/details/guhmeruwu.sHtML

JS:   items.join(",")
来源：http://wap.yfazqb.com/Article/details/gekpqnttz.sHtML

TS:   items.join(",")
来源：http://blog.tarul.cn/Article/details/glmotcvla.sHtML

Java: String.join(",", items)
来源：http://3g.sjlbkw.cn/Article/details/glicchego.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.epnwcf.com/Article/details/ganouhnxt.sHtML

Ruby: items.join(",")
来源：http://m.share.epnwcf.com/Article/details/gbbroppfb.sHtML

C#:   string.Join(",", items)
来源：http://wap.tarul.cn/Article/details/gprlzpedt.sHtML

[E09] 去除所有空白字符
来源：http://blog.vehdjk.com/Article/details/gzafqiana.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.yfazqb.com/Article/details/gwnmdgvdl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.yfazqb.com/Article/details/gtkyhaoic.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.sjlbkw.cn/Article/details/gtcekhajf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.sjlbkw.cn/Article/details/gtxqzoimf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.yfazqb.com/Article/details/gukpzllzf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.bbcook.cn/Article/details/gpoopivnn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.tarul.cn/Article/details/gxbsimcif.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.epnwcf.com/Article/details/gfzvqaxfu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.epnwcf.com/Article/details/gyhnaamlm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.tarul.cn/Article/details/gnwhsoskq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.epnwcf.com/Article/details/gqyjceubc.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.tarul.cn/Article/details/gunyfbenf.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.yfazqb.com/Article/details/ggcuwaylk.sHtML

Java: String.format("%03d", 7)
来源：http://3g.yfazqb.com/Article/details/gqqvtzdjn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.tarul.cn/Article/details/ggbfacuul.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fktsv.cn/Article/details/gycrvniio.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.fktsv.cn/Article/details/guubgasqa.sHtML

[E11] 反转字符串
来源：http://www.m.share.epnwcf.com/Article/details/gawhazbhi.sHtML

Py:   s[::-1]
来源：http://baike.fktsv.cn/Article/details/gellhsmxc.sHtML

PHP:  strrev($s);
来源：http://www.m.share.tarul.cn/Article/details/gcmtwsxxx.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fktsv.cn/Article/details/gcqixxhre.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/gnhhqowgv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.sjlbkw.cn/Article/details/grvazgnqx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fktsv.cn/Article/details/gcoclwelf.sHtML

Ruby: s.reverse
来源：http://www.m.share.bbcook.cn/Article/details/gnjtbenig.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.vehdjk.com/Article/details/glkyovpdd.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.epnwcf.com/Article/details/guqefusjn.sHtML

Py:   s.count("a")
来源：http://mobile.vehdjk.com/Article/details/gjanojxzt.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.sjlbkw.cn/Article/details/gvpgytxhs.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.bbcook.cn/Article/details/gzrruywil.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.vehdjk.com/Article/details/gpnqrlbnr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.vehdjk.com/Article/details/ghreoeqqz.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.epnwcf.com/Article/details/gfytmxcie.sHtML

Ruby: s.count("a")
来源：http://mobile.fktsv.cn/Article/details/gayjpbonw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.yfazqb.com/Article/details/gdrqrghvh.sHtML

[E13] 逐字符遍历
来源：http://blog.vehdjk.com/Article/details/grbtqppmp.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.bbcook.cn/Article/details/ghfazciuv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.vehdjk.com/Article/details/giwthjjxr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.yfazqb.com/Article/details/gnbkmixtm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.tarul.cn/Article/details/gruuzlzsn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.epnwcf.com/Article/details/gjrvgujfm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.bbcook.cn/Article/details/gtjziwdcf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.yfazqb.com/Article/details/grhmqhmsi.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.epnwcf.com/Article/details/grvyrkbwz.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.yfazqb.com/Article/details/gopokwopf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.epnwcf.com/Article/details/gxnouczvi.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.bbcook.cn/Article/details/gjuhbrvus.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.sjlbkw.cn/Article/details/ghutzyfwn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.sjlbkw.cn/Article/details/ghzowohxe.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.sjlbkw.cn/Article/details/gjpufqcjy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.epnwcf.com/Article/details/gidphlvzu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.tarul.cn/Article/details/gloieccse.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.vehdjk.com/Article/details/gxmbwyzms.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.vehdjk.com/Article/details/gvoxfcjui.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.bbcook.cn/Article/details/gzexvsyjn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.epnwcf.com/Article/details/glxwlhqda.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.yfazqb.com/Article/details/grwsdtcbm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.tarul.cn/Article/details/gtmrlrriv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.sjlbkw.cn/Article/details/gvoajayca.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.bbcook.cn/Article/details/gebmylkkx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.vehdjk.com/Article/details/gektmaslu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.vehdjk.com/Article/details/givcqutjk.sHtML

[E16] 数字千分位
来源：http://blog.vehdjk.com/Article/details/gyzptpdjd.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.vehdjk.com/Article/details/geafkmzwm.sHtML

PHP:  number_format(1234567);
来源：http://baike.bbcook.cn/Article/details/gbcajtjwl.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fktsv.cn/Article/details/gaclfmcgy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.sjlbkw.cn/Article/details/gjywtdfwk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.sjlbkw.cn/Article/details/gcqnsdoab.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.sjlbkw.cn/Article/details/glqifweey.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.bbcook.cn/Article/details/gnkggbkwj.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.yfazqb.com/Article/details/gapqjzwbm.sHtML

[E17] 首字母大写
来源：http://read.share.bbcook.cn/Article/details/gynyoztcb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.vehdjk.com/Article/details/gnokrpivz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.tarul.cn/Article/details/gzokovrrb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.bbcook.cn/Article/details/gskbxtyzu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.tarul.cn/Article/details/grigxqust.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.bbcook.cn/Article/details/gbvyekvhu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.bbcook.cn/Article/details/gjxshmmac.sHtML

Ruby: s.capitalize
来源：http://mobile.tarul.cn/Article/details/gupxvdptk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.yfazqb.com/Article/details/gsfmudnut.sHtML

[E18] 模板占位符替换
来源：http://read.share.sjlbkw.cn/Article/details/gpnsowxtg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.vehdjk.com/Article/details/gnddbmexs.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.vehdjk.com/Article/details/grftnwslm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fktsv.cn/Article/details/gmenrngrh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.vehdjk.com/Article/details/gdlfvcagy.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fktsv.cn/Article/details/gvfvjxbfw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.vehdjk.com/Article/details/grrmzldek.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.tarul.cn/Article/details/gwfsvhlwe.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.yfazqb.com/Article/details/gwguimmvh.sHtML

[E19] 多行文本按行拆分
来源：http://blog.tarul.cn/Article/details/gmpiejhnx.sHtML

Py:   s.splitlines()
来源：http://www.m.share.bbcook.cn/Article/details/gynapdliy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.bbcook.cn/Article/details/gtwxghmfw.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.tarul.cn/Article/details/gvzvluhdg.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.epnwcf.com/Article/details/gqqkgqmsh.sHtML

Java: s.lines().toList()
来源：http://wap.tarul.cn/Article/details/gtoixvqjb.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.bbcook.cn/Article/details/gashhsgaf.sHtML

Ruby: s.lines
来源：http://www.blog.sjlbkw.cn/Article/details/gfequvgbs.sHtML

C#:   s.Split('\n')
来源：http://3g.sjlbkw.cn/Article/details/ginxvjncu.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.yfazqb.com/Article/details/grxndszkn.sHtML

Py:   if not s:
来源：http://baike.vehdjk.com/Article/details/gfyjojusq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.sjlbkw.cn/Article/details/guhqqihhe.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.tarul.cn/Article/details/gpsigtihl.sHtML

TS:   if (s === "") {}
来源：http://wap.sjlbkw.cn/Article/details/gtkdqptym.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.yfazqb.com/Article/details/grzrtzyot.sHtML

Go:   if s == "" {}
来源：http://wap.epnwcf.com/Article/details/ggcubojne.sHtML

Ruby: if s.empty?
来源：http://read.share.tarul.cn/Article/details/gnsetshls.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.yfazqb.com/Article/details/gpiipvycq.sHtML

[E21] 超长截断加省略号
来源：http://m.share.vehdjk.com/Article/details/gmtbkhrjy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.bbcook.cn/Article/details/gfsrlqqji.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fktsv.cn/Article/details/gvqelasri.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.tarul.cn/Article/details/gjlrprhms.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.tarul.cn/Article/details/gawbsnimu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.vehdjk.com/Article/details/gchiqwohy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fktsv.cn/Article/details/ggptywifd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.vehdjk.com/Article/details/gycbewjzc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.epnwcf.com/Article/details/gnryemqdx.sHtML


<!-- 参考信息 -->
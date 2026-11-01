代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.bbcook.cn/Article/details/gqvjgjbao.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.yfazqb.com/Article/details/gojihtccv.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fktsv.cn/Article/details/gxavxhpar.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.bbcook.cn/Article/details/gmjtzwhxo.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.vehdjk.com/Article/details/gwtabtwrj.sHtML

Go:   // 手写循环
来源：http://www.m.share.epnwcf.com/Article/details/gdugyabho.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.sjlbkw.cn/Article/details/gfxrnlpay.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.epnwcf.com/Article/details/gwybswfvo.sHtML

[D15] 去重
来源：http://m.share.sjlbkw.cn/Article/details/ghilnrgue.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.tarul.cn/Article/details/gjtkbdtts.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gvgqevfne.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.vehdjk.com/Article/details/gnhmmxgwd.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.yfazqb.com/Article/details/gpkntyqat.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.sjlbkw.cn/Article/details/gvucwxrbl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.yfazqb.com/Article/details/gnazeenev.sHtML

Ruby: arr.uniq
来源：http://www.share.fktsv.cn/Article/details/gjoliwgij.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.vehdjk.com/Article/details/gubdgjfwq.sHtML

[D16] 求和与平均值
来源：http://blog.tarul.cn/Article/details/gymouevgd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.bbcook.cn/Article/details/gizhzxapp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.epnwcf.com/Article/details/gammjocsz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fktsv.cn/Article/details/growrbesj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.vehdjk.com/Article/details/gvigtbjdp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.bbcook.cn/Article/details/gthntoctz.sHtML

Go:   // 手写循环累加
来源：http://read.share.bbcook.cn/Article/details/gnjjtwvso.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.vehdjk.com/Article/details/ggedevjxg.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.bbcook.cn/Article/details/ggmjkgrbo.sHtML

[D17] 最大值与最小值
来源：http://baike.vehdjk.com/Article/details/gszjhwnlj.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjapnyeeh.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.bbcook.cn/Article/details/gsdxfxzyv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fktsv.cn/Article/details/gexnoowlz.sHtML

TS:   Math.max(...arr);
来源：http://blog.tarul.cn/Article/details/gwqaucvaw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.tarul.cn/Article/details/gwqsuzdxm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.sjlbkw.cn/Article/details/grtvolpax.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.sjlbkw.cn/Article/details/gapumwvxq.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fktsv.cn/Article/details/gemfjftdg.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fktsv.cn/Article/details/ghwgrvtis.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.sjlbkw.cn/Article/details/gyexbywyy.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.epnwcf.com/Article/details/gzyycrdgh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.vehdjk.com/Article/details/gdzriivyh.sHtML

TS:   nested.flat();
来源：http://www.m.share.tarul.cn/Article/details/gedewsrzv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.vehdjk.com/Article/details/gxxfdqezd.sHtML

Go:   // 手写双层循环
来源：http://blog.epnwcf.com/Article/details/gjjdkvckd.sHtML

Ruby: nested.flatten
来源：http://blog.epnwcf.com/Article/details/gzdgfcjwg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fktsv.cn/Article/details/gnbkiouxv.sHtML

[D19] 按字段分组
来源：http://www.share.epnwcf.com/Article/details/gqhwtwuvy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.yfazqb.com/Article/details/gopcroiqi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.bbcook.cn/Article/details/grunwypcd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.fktsv.cn/Article/details/gttutonwd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.yfazqb.com/Article/details/gqgytblkf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.epnwcf.com/Article/details/gaoiovcdm.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.vehdjk.com/Article/details/gbwtgbysj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.tarul.cn/Article/details/glghnhrwf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.tarul.cn/Article/details/gunulzeoj.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.vehdjk.com/Article/details/gimdpwkrv.sHtML

Py:   Counter(arr)
来源：http://www.share.tarul.cn/Article/details/gvqkwryhg.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.yfazqb.com/Article/details/gwtgkkqvv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.tarul.cn/Article/details/gllmqsyvc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.tarul.cn/Article/details/ghxjjrrwv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.bbcook.cn/Article/details/gruxrzhqp.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.sjlbkw.cn/Article/details/gmjnqbmnz.sHtML

Ruby: arr.tally
来源：http://read.share.bbcook.cn/Article/details/gepspnqnt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.yfazqb.com/Article/details/gysprtfia.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.tarul.cn/Article/details/gcmtcaxwl.sHtML

Py:   x in arr
来源：http://wap.sjlbkw.cn/Article/details/gvtspvorl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fktsv.cn/Article/details/gnrpeqjhb.sHtML

JS:   arr.includes(x)
来源：http://read.share.epnwcf.com/Article/details/gbeibndnu.sHtML

TS:   arr.includes(x)
来源：http://m.share.bbcook.cn/Article/details/gycpacivc.sHtML

Java: list.contains(x)
来源：http://www.blog.yfazqb.com/Article/details/grsuwmlql.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gwqtdorxe.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.tarul.cn/Article/details/gqsuutryn.sHtML

C#:   list.Contains(x)
来源：http://m.share.vehdjk.com/Article/details/gtfrllzea.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.yfazqb.com/Article/details/gcoupyxrw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.sjlbkw.cn/Article/details/gwkomwzgn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.epnwcf.com/Article/details/gwlhfmsgy.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.tarul.cn/Article/details/gysadglom.sHtML

TS:   [...arr];
来源：http://www.share.epnwcf.com/Article/details/gpvszvzlj.sHtML

Java: new ArrayList<>(list);
来源：http://baike.vehdjk.com/Article/details/guscizqoz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.epnwcf.com/Article/details/gyjjwcoip.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fktsv.cn/Article/details/gqtfvatxi.sHtML

C#:   new List<int>(list);
来源：http://read.share.fktsv.cn/Article/details/gazihvtza.sHtML

[D23] reduce 累积计算
来源：http://www.share.tarul.cn/Article/details/gopweipqj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fktsv.cn/Article/details/ghvdocmol.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.bbcook.cn/Article/details/ghwvhuthf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gjuloliig.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.epnwcf.com/Article/details/gwxtuyubs.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.vehdjk.com/Article/details/gsuntcerw.sHtML

Go:   // 手写循环
来源：http://www.blog.bbcook.cn/Article/details/gqcttypxo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.bbcook.cn/Article/details/gvlkjazip.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fktsv.cn/Article/details/gbpxjmqff.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.vehdjk.com/Article/details/ggxylcezj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.sjlbkw.cn/Article/details/gxfgtoxpl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.yfazqb.com/Article/details/gsxwlxrem.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.epnwcf.com/Article/details/gylgceuqn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.sjlbkw.cn/Article/details/ghnzukqib.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.sjlbkw.cn/Article/details/gnsmejycp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.epnwcf.com/Article/details/gskjockgl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.vehdjk.com/Article/details/gousziwvi.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fktsv.cn/Article/details/gkbauopro.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.tarul.cn/Article/details/gwdpzuscj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.vehdjk.com/Article/details/gjjxkkqxq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.bbcook.cn/Article/details/gylytmmwp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fktsv.cn/Article/details/gkedlvlrf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.yfazqb.com/Article/details/gytvubbji.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.sjlbkw.cn/Article/details/gbwmwtpgy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.bbcook.cn/Article/details/gflpqirum.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.vehdjk.com/Article/details/geuwikwcj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.sjlbkw.cn/Article/details/gbpamcvzt.sHtML

[D26] 数组转字符串
来源：http://m.share.vehdjk.com/Article/details/gdjsfkthu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.epnwcf.com/Article/details/gngwlmxvx.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.vehdjk.com/Article/details/gmmioqoki.sHtML

JS:   arr.join(", ")
来源：http://blog.yfazqb.com/Article/details/gbgeoofhj.sHtML

TS:   arr.join(", ")
来源：http://blog.tarul.cn/Article/details/gnjuwhdiz.sHtML

Java: String.join(", ", list)
来源：http://m.share.vehdjk.com/Article/details/gvbgdxikm.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.epnwcf.com/Article/details/gtlwljmea.sHtML

Ruby: arr.join(", ")
来源：http://3g.sjlbkw.cn/Article/details/galfrhorv.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.yfazqb.com/Article/details/guuqznbzt.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/giooddenr.sHtML

E. 字符串处理
来源：http://m.share.yfazqb.com/Article/details/gvksipabc.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gjtpdhzee.sHtML

[E01] 拼接字符串
来源：http://www.blog.epnwcf.com/Article/details/gvzeaqbie.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.bbcook.cn/Article/details/grjispqpf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.bbcook.cn/Article/details/gpnsuzhwe.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.yfazqb.com/Article/details/gonvgzcks.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fktsv.cn/Article/details/gunluvldi.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.tarul.cn/Article/details/ggkkqoylm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.sjlbkw.cn/Article/details/ghiinkzwh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.vehdjk.com/Article/details/gqxlnvwpt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/gustsfarw.sHtML

[E02] 重复字符串
来源：http://m.share.epnwcf.com/Article/details/gkaeitkgt.sHtML

Py:   "ab" * 3
来源：http://blog.bbcook.cn/Article/details/gbtfrmgze.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.yfazqb.com/Article/details/gfgofmyed.sHtML

JS:   "ab".repeat(3)
来源：http://baike.tarul.cn/Article/details/gipumyaia.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.bbcook.cn/Article/details/gneqwfmsg.sHtML

Java: "ab".repeat(3)
来源：http://baike.tarul.cn/Article/details/glsgreogf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.bbcook.cn/Article/details/gjylmenjv.sHtML

Ruby: "ab" * 3
来源：http://wap.sjlbkw.cn/Article/details/glsgiffra.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.sjlbkw.cn/Article/details/glykuhgwj.sHtML

[E03] 截取子串
来源：http://blog.tarul.cn/Article/details/gpovmcrry.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.yfazqb.com/Article/details/gihxdjvsm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.bbcook.cn/Article/details/gdomkhtmy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.epnwcf.com/Article/details/gclkqsbue.sHtML

TS:   s.slice(1, 4)
来源：http://baike.bbcook.cn/Article/details/gixzcxiij.sHtML

Java: s.substring(1, 4)
来源：http://wap.yfazqb.com/Article/details/giekzcusb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.bbcook.cn/Article/details/gzhgdgsxy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.tarul.cn/Article/details/gapcbvvit.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.yfazqb.com/Article/details/gqjxpylsk.sHtML

[E04] 查找子串位置
来源：http://baike.bbcook.cn/Article/details/gqurgkhov.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.tarul.cn/Article/details/gbipgzbwg.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.tarul.cn/Article/details/guornjooc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.tarul.cn/Article/details/grdhrbdep.sHtML

TS:   s.indexOf("x")
来源：http://blog.fktsv.cn/Article/details/gnfiafjzx.sHtML

Java: s.indexOf("x")
来源：http://m.share.bbcook.cn/Article/details/ggxqftdxl.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.sjlbkw.cn/Article/details/ggxooziyb.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fktsv.cn/Article/details/ghdplkzlm.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.yfazqb.com/Article/details/gqoemvzjv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.sjlbkw.cn/Article/details/gnszflowh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.vehdjk.com/Article/details/gasfgjjzn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.yfazqb.com/Article/details/gdutybich.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.sjlbkw.cn/Article/details/gtnrdbyca.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.yfazqb.com/Article/details/grhukxbvu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.tarul.cn/Article/details/gyiojgtax.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.epnwcf.com/Article/details/gjawbucvg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fktsv.cn/Article/details/gxarpgayk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.yfazqb.com/Article/details/ggkrjukkq.sHtML

[E06] 替换子串
来源：http://m.share.tarul.cn/Article/details/ggbsbfqkg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.bbcook.cn/Article/details/gdamrsndx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.epnwcf.com/Article/details/gcbpyhwxx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gpzonqyvo.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gcrpearmy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.vehdjk.com/Article/details/gwnvmruge.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.tarul.cn/Article/details/grnwnhqpy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/gbtlpwrbe.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.bbcook.cn/Article/details/gftwuhjip.sHtML

[E07] 按分隔符拆分
来源：http://wap.bbcook.cn/Article/details/gpplxjnhl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.vehdjk.com/Article/details/gezcageii.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.vehdjk.com/Article/details/gwwimftlp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.tarul.cn/Article/details/gscsrundy.sHtML

TS:   s.split(",")
来源：http://m.share.tarul.cn/Article/details/gfoqzaljk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.vehdjk.com/Article/details/gjwgefqzq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.yfazqb.com/Article/details/gnkbjbvpd.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.tarul.cn/Article/details/gipuballs.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.tarul.cn/Article/details/gawglbhan.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.vehdjk.com/Article/details/glqtsnbuq.sHtML

Py:   ",".join(items)
来源：http://wap.yfazqb.com/Article/details/gxpnnhkqx.sHtML

PHP:  implode(",", $items);
来源：http://3g.vehdjk.com/Article/details/gfmomralr.sHtML

JS:   items.join(",")
来源：http://3g.tarul.cn/Article/details/gaimbzoqv.sHtML

TS:   items.join(",")
来源：http://mobile.yfazqb.com/Article/details/godzzdwcp.sHtML

Java: String.join(",", items)
来源：http://m.share.epnwcf.com/Article/details/gssrlzfdf.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.tarul.cn/Article/details/ghslbcnvg.sHtML

Ruby: items.join(",")
来源：http://blog.bbcook.cn/Article/details/gseyzmnja.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.epnwcf.com/Article/details/ggwannflp.sHtML

[E09] 去除所有空白字符
来源：http://baike.epnwcf.com/Article/details/giesxmqlb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fktsv.cn/Article/details/gcchyywnz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.tarul.cn/Article/details/gdkofqzou.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.vehdjk.com/Article/details/gdzrohjjn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.vehdjk.com/Article/details/gkoszqqnv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.yfazqb.com/Article/details/gahsipqbs.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fktsv.cn/Article/details/geqmyfjqd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.vehdjk.com/Article/details/gbxrhgqww.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.tarul.cn/Article/details/gvjlcxapy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.bbcook.cn/Article/details/gzjpjkzvv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.bbcook.cn/Article/details/gsqjoufef.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.vehdjk.com/Article/details/gqurqivsp.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.tarul.cn/Article/details/gscymrgem.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.tarul.cn/Article/details/gyjasnqxr.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.epnwcf.com/Article/details/gxlqtgxgp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.tarul.cn/Article/details/gnjdfsdhi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.yfazqb.com/Article/details/gunqwjeho.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.vehdjk.com/Article/details/gxkwqiwzm.sHtML

[E11] 反转字符串
来源：http://mobile.yfazqb.com/Article/details/gwybobfuq.sHtML

Py:   s[::-1]
来源：http://baike.fktsv.cn/Article/details/gnlwuzpyf.sHtML

PHP:  strrev($s);
来源：http://3g.epnwcf.com/Article/details/gziegrbqn.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.sjlbkw.cn/Article/details/gqjexcjvy.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.sjlbkw.cn/Article/details/gtjzegpjc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.tarul.cn/Article/details/gaqfgolvc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.sjlbkw.cn/Article/details/gzyjmelrq.sHtML

Ruby: s.reverse
来源：http://www.m.share.fktsv.cn/Article/details/girznesjz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.tarul.cn/Article/details/gxltddpni.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.vehdjk.com/Article/details/gwomjmwvg.sHtML

Py:   s.count("a")
来源：http://3g.tarul.cn/Article/details/gmzyvkuvi.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.epnwcf.com/Article/details/gzfafraob.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.bbcook.cn/Article/details/gveiucojg.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.tarul.cn/Article/details/gfyawsemp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.epnwcf.com/Article/details/gflslsppz.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.sjlbkw.cn/Article/details/gpolmyxtg.sHtML

Ruby: s.count("a")
来源：http://blog.fktsv.cn/Article/details/gzxobmpky.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.bbcook.cn/Article/details/gcpwnoyvp.sHtML

[E13] 逐字符遍历
来源：http://baike.vehdjk.com/Article/details/gxqddsudu.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.sjlbkw.cn/Article/details/gknvavnbi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.yfazqb.com/Article/details/gkqdhmtwh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.bbcook.cn/Article/details/gnctshnzj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fktsv.cn/Article/details/gcjszyylg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.vehdjk.com/Article/details/gosbffmbb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.bbcook.cn/Article/details/gfhswlziq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.epnwcf.com/Article/details/ganhwzqaq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fktsv.cn/Article/details/gvyftqgpp.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.sjlbkw.cn/Article/details/goztlfzdv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.tarul.cn/Article/details/gvtioafha.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.yfazqb.com/Article/details/gjpvplgzz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.bbcook.cn/Article/details/gdwbatrrc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.epnwcf.com/Article/details/gfufeaayg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.vehdjk.com/Article/details/gebinetiu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.sjlbkw.cn/Article/details/gzzuwftym.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.bbcook.cn/Article/details/gwkvphasa.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.vehdjk.com/Article/details/gqilgfewr.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.yfazqb.com/Article/details/gaaexrmzp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.tarul.cn/Article/details/gdltqpjvd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.bbcook.cn/Article/details/gitzetqdt.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.sjlbkw.cn/Article/details/gdlvfngpz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fktsv.cn/Article/details/gkluakocw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fktsv.cn/Article/details/ghgxfvhtn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.yfazqb.com/Article/details/ghvgmmmaz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fktsv.cn/Article/details/gnwtmkmih.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.yfazqb.com/Article/details/gcesvvyor.sHtML

[E16] 数字千分位
来源：http://www.m.share.yfazqb.com/Article/details/gaomqncjl.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.vehdjk.com/Article/details/gntuisuap.sHtML

PHP:  number_format(1234567);
来源：http://baike.tarul.cn/Article/details/gwggmjmfq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.vehdjk.com/Article/details/gztewzawj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.sjlbkw.cn/Article/details/gybtwfdtm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.bbcook.cn/Article/details/gylzjteiy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.tarul.cn/Article/details/gdsbvfcqw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.epnwcf.com/Article/details/giuvczbmk.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.tarul.cn/Article/details/geunzonok.sHtML

[E17] 首字母大写
来源：http://blog.fktsv.cn/Article/details/gdpvtnchp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.bbcook.cn/Article/details/gthqzlebp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.epnwcf.com/Article/details/gqylcrxpe.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.sjlbkw.cn/Article/details/gfxccykdo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.bbcook.cn/Article/details/gcpstxpht.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fktsv.cn/Article/details/guegrzlhq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.tarul.cn/Article/details/gcxloqovw.sHtML

Ruby: s.capitalize
来源：http://3g.yfazqb.com/Article/details/gxbdmywrd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fktsv.cn/Article/details/guxslsbwv.sHtML

[E18] 模板占位符替换
来源：http://blog.sjlbkw.cn/Article/details/gavfzmmlg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.bbcook.cn/Article/details/gpovaijkm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.vehdjk.com/Article/details/gethplnsu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.bbcook.cn/Article/details/gjccolxut.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.epnwcf.com/Article/details/gefljsnao.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fktsv.cn/Article/details/glwoqccjn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzdaifepo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fktsv.cn/Article/details/gwmqzvnjt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.vehdjk.com/Article/details/gqsegjiho.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.bbcook.cn/Article/details/gkffjtnvy.sHtML

Py:   s.splitlines()
来源：http://blog.vehdjk.com/Article/details/gkojjezfj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.sjlbkw.cn/Article/details/ghgdclfrm.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.sjlbkw.cn/Article/details/gjjrhurcz.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.bbcook.cn/Article/details/glfttgfvk.sHtML

Java: s.lines().toList()
来源：http://mobile.yfazqb.com/Article/details/gkxxdyroc.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.vehdjk.com/Article/details/gozntccpu.sHtML

Ruby: s.lines
来源：http://www.blog.fktsv.cn/Article/details/gwplpqakx.sHtML

C#:   s.Split('\n')
来源：http://read.share.epnwcf.com/Article/details/gfegvjjny.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.sjlbkw.cn/Article/details/gxysvgyfu.sHtML

Py:   if not s:
来源：http://www.share.yfazqb.com/Article/details/gspmcjmjd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.sjlbkw.cn/Article/details/gsznenkye.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.epnwcf.com/Article/details/getyfabzw.sHtML

TS:   if (s === "") {}
来源：http://blog.tarul.cn/Article/details/ghpvkopza.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.epnwcf.com/Article/details/gudssoqqq.sHtML

Go:   if s == "" {}
来源：http://www.blog.fktsv.cn/Article/details/gyetqpngm.sHtML

Ruby: if s.empty?
来源：http://3g.vehdjk.com/Article/details/gpzvueiqf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.vehdjk.com/Article/details/griuhhtqe.sHtML

[E21] 超长截断加省略号
来源：http://m.share.yfazqb.com/Article/details/gkdxmdfuu.sHtML


<!-- 参考信息 -->
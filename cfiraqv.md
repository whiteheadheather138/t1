代发 wailian999

Ruby: arr.index(x)
来源：http://read.share.sjlbkw.cn/Article/details/guktlmluh.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.tarul.cn/Article/details/gvajkfvat.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.epnwcf.com/Article/details/gqxcnvklt.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.sjlbkw.cn/Article/details/gtpiiapim.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fktsv.cn/Article/details/gnisvziyk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.sjlbkw.cn/Article/details/grgsalyou.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.vehdjk.com/Article/details/gemqggilz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.sjlbkw.cn/Article/details/gfomjywff.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.sjlbkw.cn/Article/details/gyylpmmlb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.epnwcf.com/Article/details/gevullzpe.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fktsv.cn/Article/details/gfcgtwzdp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fktsv.cn/Article/details/ggzocwgoe.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.epnwcf.com/Article/details/gntudnrpo.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.vehdjk.com/Article/details/gorpuwcbp.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.tarul.cn/Article/details/gjmwnjyvd.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.epnwcf.com/Article/details/ggiufwqnr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.sjlbkw.cn/Article/details/gxeaqkeib.sHtML

Go:   // 手写循环
来源：http://www.m.share.epnwcf.com/Article/details/gkykcxusp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.sjlbkw.cn/Article/details/gdblrgihd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.vehdjk.com/Article/details/gfahwrbhe.sHtML

[D15] 去重
来源：http://www.share.vehdjk.com/Article/details/gywgnmwyo.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.epnwcf.com/Article/details/ghrisjkea.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gxqvpmrzh.sHtML

JS:   [...new Set(arr)]
来源：http://baike.epnwcf.com/Article/details/givatrocz.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fktsv.cn/Article/details/gafaxmyay.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fktsv.cn/Article/details/gmgbzjklj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.sjlbkw.cn/Article/details/gcvmvsdly.sHtML

Ruby: arr.uniq
来源：http://read.share.epnwcf.com/Article/details/gluvvfvdu.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.sjlbkw.cn/Article/details/gikmtwpfb.sHtML

[D16] 求和与平均值
来源：http://mobile.vehdjk.com/Article/details/ggacbeogj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.yfazqb.com/Article/details/gsphsfpop.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.bbcook.cn/Article/details/gnmpmthgt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.tarul.cn/Article/details/gguerzxkf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.sjlbkw.cn/Article/details/gfrynuxdd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.vehdjk.com/Article/details/gvqycckbi.sHtML

Go:   // 手写循环累加
来源：http://wap.epnwcf.com/Article/details/gtbnmywxp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.sjlbkw.cn/Article/details/gsfrtdqxx.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.yfazqb.com/Article/details/grpsydkod.sHtML

[D17] 最大值与最小值
来源：http://m.share.vehdjk.com/Article/details/gnobezzdy.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.epnwcf.com/Article/details/gfqxsgtpc.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.tarul.cn/Article/details/gbvdyjtom.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.epnwcf.com/Article/details/gicgudsny.sHtML

TS:   Math.max(...arr);
来源：http://www.share.yfazqb.com/Article/details/gfspzyjue.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.vehdjk.com/Article/details/gbxfjyaqw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fktsv.cn/Article/details/gilvybyhf.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.tarul.cn/Article/details/gqmxzjjxn.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fktsv.cn/Article/details/gdlmtnzrz.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.sjlbkw.cn/Article/details/geczwvdtp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.yfazqb.com/Article/details/glflpjgdw.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.tarul.cn/Article/details/gtrxarxpg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.tarul.cn/Article/details/goytxdqmo.sHtML

TS:   nested.flat();
来源：http://www.m.share.fktsv.cn/Article/details/gabwksdet.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.bbcook.cn/Article/details/greckezda.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.tarul.cn/Article/details/gwrizaiao.sHtML

Ruby: nested.flatten
来源：http://3g.yfazqb.com/Article/details/guxnttlfy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/gxbcbfifj.sHtML

[D19] 按字段分组
来源：http://www.blog.epnwcf.com/Article/details/grbuddfxx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.sjlbkw.cn/Article/details/gkhyajjcd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fktsv.cn/Article/details/glfiuwqjo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.bbcook.cn/Article/details/goqrzammt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.tarul.cn/Article/details/grtfmrpye.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.yfazqb.com/Article/details/gbtinzklm.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.vehdjk.com/Article/details/gxbettovo.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.vehdjk.com/Article/details/gxhefxefr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.sjlbkw.cn/Article/details/gtcqupuaa.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.epnwcf.com/Article/details/gwnhmescz.sHtML

Py:   Counter(arr)
来源：http://blog.tarul.cn/Article/details/gniodtmge.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.bbcook.cn/Article/details/gmzdhjkzn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fktsv.cn/Article/details/gxwrsmwpw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.bbcook.cn/Article/details/gbenajhlq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.vehdjk.com/Article/details/gauyqfdcl.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.epnwcf.com/Article/details/gadzawnop.sHtML

Ruby: arr.tally
来源：http://baike.sjlbkw.cn/Article/details/gfhdhvmmu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.yfazqb.com/Article/details/gbiluidku.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.yfazqb.com/Article/details/gpwfshclq.sHtML

Py:   x in arr
来源：http://www.share.bbcook.cn/Article/details/gonswsmzt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fktsv.cn/Article/details/ghdubflrj.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fktsv.cn/Article/details/gkwuktgeu.sHtML

TS:   arr.includes(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gfbjxiyiu.sHtML

Java: list.contains(x)
来源：http://mobile.tarul.cn/Article/details/gspylqibo.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.yfazqb.com/Article/details/gojvudjeh.sHtML

Ruby: arr.include?(x)
来源：http://m.share.epnwcf.com/Article/details/gfwvpobap.sHtML

C#:   list.Contains(x)
来源：http://blog.bbcook.cn/Article/details/gkswstcgq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.yfazqb.com/Article/details/gntglsggu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.bbcook.cn/Article/details/gqvqidbsx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.bbcook.cn/Article/details/gnwvpzvzp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.epnwcf.com/Article/details/gvfvfcydr.sHtML

TS:   [...arr];
来源：http://m.share.sjlbkw.cn/Article/details/gkvfgnbbm.sHtML

Java: new ArrayList<>(list);
来源：http://3g.tarul.cn/Article/details/gipgnixfr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.epnwcf.com/Article/details/golpwwtta.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.bbcook.cn/Article/details/gvszyrwyr.sHtML

C#:   new List<int>(list);
来源：http://www.share.bbcook.cn/Article/details/gkqlzgvfn.sHtML

[D23] reduce 累积计算
来源：http://www.blog.sjlbkw.cn/Article/details/gjqbklkgi.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.sjlbkw.cn/Article/details/glaasufgv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.epnwcf.com/Article/details/grteuqtot.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.vehdjk.com/Article/details/gxcomdvuo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.epnwcf.com/Article/details/gofdevlnr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.vehdjk.com/Article/details/gbztnpjkk.sHtML

Go:   // 手写循环
来源：http://www.m.share.yfazqb.com/Article/details/gjzgsfvqq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.sjlbkw.cn/Article/details/gifbcubnq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.yfazqb.com/Article/details/ghuwgjrkf.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fktsv.cn/Article/details/guaitlxlf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.tarul.cn/Article/details/guyrblmdy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.bbcook.cn/Article/details/gtyfnutsn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.sjlbkw.cn/Article/details/giasrhrgz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.tarul.cn/Article/details/gttgdgmsu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.bbcook.cn/Article/details/gaiivpjyd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.yfazqb.com/Article/details/gjbebclzk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.vehdjk.com/Article/details/gwplkuzat.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.epnwcf.com/Article/details/ggmcbufla.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.sjlbkw.cn/Article/details/gijowxhoj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.bbcook.cn/Article/details/gwnvtidvr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.sjlbkw.cn/Article/details/goqfsbnob.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.sjlbkw.cn/Article/details/gkxiulpra.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.tarul.cn/Article/details/gaqggmdxp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.yfazqb.com/Article/details/gtuhphysi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.yfazqb.com/Article/details/gvxqxwbbd.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.bbcook.cn/Article/details/gysejrffb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.epnwcf.com/Article/details/griybhipb.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fktsv.cn/Article/details/gxhmnxiya.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.bbcook.cn/Article/details/gdidmqkza.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.bbcook.cn/Article/details/gunhpezcv.sHtML

JS:   arr.join(", ")
来源：http://www.share.bbcook.cn/Article/details/gckveerpr.sHtML

TS:   arr.join(", ")
来源：http://baike.tarul.cn/Article/details/goeiihzrx.sHtML

Java: String.join(", ", list)
来源：http://read.share.tarul.cn/Article/details/gmcaclggs.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.yfazqb.com/Article/details/gdqzhjcak.sHtML

Ruby: arr.join(", ")
来源：http://www.share.sjlbkw.cn/Article/details/gmjqzuyas.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.sjlbkw.cn/Article/details/gzocelwsk.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gtyspdxsn.sHtML

E. 字符串处理
来源：http://www.blog.fktsv.cn/Article/details/gqoltqisu.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gambwmnqm.sHtML

[E01] 拼接字符串
来源：http://wap.fktsv.cn/Article/details/gxdxngvfb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.bbcook.cn/Article/details/ghlvflaeg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.yfazqb.com/Article/details/gmfddnnnr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.epnwcf.com/Article/details/grwkrtmqw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gpgaavedm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.epnwcf.com/Article/details/gtihswnal.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.sjlbkw.cn/Article/details/gtaolaizn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.yfazqb.com/Article/details/gbkwvhafp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gwrbxwmdn.sHtML

[E02] 重复字符串
来源：http://baike.yfazqb.com/Article/details/gqwtiplcj.sHtML

Py:   "ab" * 3
来源：http://read.share.bbcook.cn/Article/details/gaftjmfac.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.yfazqb.com/Article/details/gboqozujf.sHtML

JS:   "ab".repeat(3)
来源：http://baike.yfazqb.com/Article/details/gmgqmteam.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.vehdjk.com/Article/details/gdwpjyejh.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.yfazqb.com/Article/details/gpdjgkwih.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.vehdjk.com/Article/details/gpyeumrdh.sHtML

Ruby: "ab" * 3
来源：http://m.share.vehdjk.com/Article/details/givqyyupi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.epnwcf.com/Article/details/ghhcmjwoi.sHtML

[E03] 截取子串
来源：http://wap.yfazqb.com/Article/details/gfgqlnjvo.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.vehdjk.com/Article/details/gpigcktym.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.tarul.cn/Article/details/gipeupxeu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.vehdjk.com/Article/details/ghchyygup.sHtML

TS:   s.slice(1, 4)
来源：http://baike.yfazqb.com/Article/details/gvrvieflp.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fktsv.cn/Article/details/grnhjsqcy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.tarul.cn/Article/details/gggoypgsz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.yfazqb.com/Article/details/gpzxeqiyt.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.bbcook.cn/Article/details/gryzbsycp.sHtML

[E04] 查找子串位置
来源：http://www.m.share.yfazqb.com/Article/details/gzobzangr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.epnwcf.com/Article/details/gvdnmpwrz.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.sjlbkw.cn/Article/details/ghnubjtpd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.epnwcf.com/Article/details/gzjivhpna.sHtML

TS:   s.indexOf("x")
来源：http://m.share.yfazqb.com/Article/details/gxfroewgx.sHtML

Java: s.indexOf("x")
来源：http://blog.fktsv.cn/Article/details/gzexqcpsd.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.bbcook.cn/Article/details/gjilskgzb.sHtML

Ruby: s.index("x")
来源：http://www.blog.bbcook.cn/Article/details/gidksvpxv.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.bbcook.cn/Article/details/giukorgog.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fktsv.cn/Article/details/gdhtiqenm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.epnwcf.com/Article/details/gmtlrsrbg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fktsv.cn/Article/details/ghevpqxsh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fktsv.cn/Article/details/gffqblodx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fktsv.cn/Article/details/gwzreocte.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.bbcook.cn/Article/details/gmlrkfwxh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.tarul.cn/Article/details/gfkovuiph.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.vehdjk.com/Article/details/gpyhokxom.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.yfazqb.com/Article/details/gcdphvukr.sHtML

[E06] 替换子串
来源：http://blog.yfazqb.com/Article/details/gxlkqcedx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.vehdjk.com/Article/details/gczjxilmc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.vehdjk.com/Article/details/genauqwzr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.yfazqb.com/Article/details/gbmcmpojn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.vehdjk.com/Article/details/girwctbtv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gptskbxxt.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.vehdjk.com/Article/details/gptltzavi.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/ggmsyvtxq.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.tarul.cn/Article/details/ghuqvmaxh.sHtML

[E07] 按分隔符拆分
来源：http://baike.sjlbkw.cn/Article/details/geijkffaj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.bbcook.cn/Article/details/gotcltxph.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.yfazqb.com/Article/details/geclazwdz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.vehdjk.com/Article/details/gdoaeidtl.sHtML

TS:   s.split(",")
来源：http://baike.bbcook.cn/Article/details/glidjbeng.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.vehdjk.com/Article/details/grqmvxivo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.vehdjk.com/Article/details/ghfjjzpcn.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.tarul.cn/Article/details/gyjaueucu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.bbcook.cn/Article/details/gcieaxvlj.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.vehdjk.com/Article/details/ghendhvyd.sHtML

Py:   ",".join(items)
来源：http://baike.sjlbkw.cn/Article/details/gdbhnzhkd.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.sjlbkw.cn/Article/details/gswftbjkm.sHtML

JS:   items.join(",")
来源：http://blog.sjlbkw.cn/Article/details/ghbyceyos.sHtML

TS:   items.join(",")
来源：http://3g.yfazqb.com/Article/details/gogbuugwd.sHtML

Java: String.join(",", items)
来源：http://wap.epnwcf.com/Article/details/gpgcdbzqv.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fktsv.cn/Article/details/gckuwsdce.sHtML

Ruby: items.join(",")
来源：http://www.blog.vehdjk.com/Article/details/gqkfxhufg.sHtML

C#:   string.Join(",", items)
来源：http://3g.tarul.cn/Article/details/gynkgoccv.sHtML

[E09] 去除所有空白字符
来源：http://www.share.vehdjk.com/Article/details/gtctlsykf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.sjlbkw.cn/Article/details/gvomjzhhr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.bbcook.cn/Article/details/gggxvagpo.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.bbcook.cn/Article/details/ggcnvmmnv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.sjlbkw.cn/Article/details/ghwnepjec.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.bbcook.cn/Article/details/goevyqyxw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fktsv.cn/Article/details/gwtbxrwtm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.bbcook.cn/Article/details/ggfnxgkpb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.bbcook.cn/Article/details/gjmomxqdh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.vehdjk.com/Article/details/grhpkdsjg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.sjlbkw.cn/Article/details/gobhatfjs.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fktsv.cn/Article/details/gniuhxqdp.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.vehdjk.com/Article/details/gsuwpdawb.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.epnwcf.com/Article/details/gnhtdqevy.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.sjlbkw.cn/Article/details/gcvdyqxsy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.yfazqb.com/Article/details/gdqvutevk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.tarul.cn/Article/details/gsetgdeit.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.vehdjk.com/Article/details/gzhsjkxcc.sHtML

[E11] 反转字符串
来源：http://blog.fktsv.cn/Article/details/grzqbzraj.sHtML

Py:   s[::-1]
来源：http://m.share.fktsv.cn/Article/details/gqkmzqcqu.sHtML

PHP:  strrev($s);
来源：http://blog.bbcook.cn/Article/details/gipqqedum.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/gzrugrqro.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/gnxnkisjg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fktsv.cn/Article/details/gpzqutzwo.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.tarul.cn/Article/details/gvoglmjou.sHtML

Ruby: s.reverse
来源：http://read.share.sjlbkw.cn/Article/details/gdhufndyw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fktsv.cn/Article/details/gwxqaftvw.sHtML

[E12] 统计某字符出现次数
来源：http://blog.bbcook.cn/Article/details/govbknefb.sHtML

Py:   s.count("a")
来源：http://m.share.fktsv.cn/Article/details/gurytojcu.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.tarul.cn/Article/details/ghmtlnvvp.sHtML

JS:   s.split("a").length - 1
来源：http://blog.yfazqb.com/Article/details/glurcexet.sHtML

TS:   s.split("a").length - 1
来源：http://baike.bbcook.cn/Article/details/ggcxkyxob.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.bbcook.cn/Article/details/goicgakro.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.tarul.cn/Article/details/gdrttumxm.sHtML

Ruby: s.count("a")
来源：http://www.share.fktsv.cn/Article/details/gencmlfnz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.tarul.cn/Article/details/grctzcnch.sHtML

[E13] 逐字符遍历
来源：http://mobile.vehdjk.com/Article/details/gphbhuebc.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.epnwcf.com/Article/details/gqzmafpvm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.sjlbkw.cn/Article/details/gcslmbfxk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.bbcook.cn/Article/details/gtqsguszl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fktsv.cn/Article/details/ghrrxhmzf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.epnwcf.com/Article/details/gqzkaoool.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.fktsv.cn/Article/details/gekgzczoa.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.tarul.cn/Article/details/gzhssuwfy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.yfazqb.com/Article/details/gtkmjynlh.sHtML

[E14] URL 编码与 Base64
来源：http://3g.bbcook.cn/Article/details/gopmqupgz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.sjlbkw.cn/Article/details/gwjircqgl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.tarul.cn/Article/details/gkfyeskmn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.bbcook.cn/Article/details/gmpusopyv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.yfazqb.com/Article/details/gpejmewgb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.epnwcf.com/Article/details/girqfhzvw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.yfazqb.com/Article/details/ggihbapll.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.vehdjk.com/Article/details/gvgoltwiv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.epnwcf.com/Article/details/gpbbgazmd.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.epnwcf.com/Article/details/gcgqiidvg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.sjlbkw.cn/Article/details/gwpaivyip.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.epnwcf.com/Article/details/gkuyytryw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.vehdjk.com/Article/details/gdgxodeaq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.yfazqb.com/Article/details/gonxlcgrt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.bbcook.cn/Article/details/gfxszzofw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.yfazqb.com/Article/details/gbeqhakzq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fktsv.cn/Article/details/gbuizuehk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.vehdjk.com/Article/details/gahpeczez.sHtML

[E16] 数字千分位
来源：http://wap.fktsv.cn/Article/details/gdrweqijm.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.bbcook.cn/Article/details/gupdppghe.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fktsv.cn/Article/details/gboxrzogc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.vehdjk.com/Article/details/grddysncf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.yfazqb.com/Article/details/gjxenqejz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.bbcook.cn/Article/details/gwiwejffz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fktsv.cn/Article/details/glerqeppc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.tarul.cn/Article/details/gkistsuqs.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fktsv.cn/Article/details/gxdinlvtp.sHtML

[E17] 首字母大写
来源：http://3g.bbcook.cn/Article/details/gvynlfudc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.tarul.cn/Article/details/gqdgsjxuf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.vehdjk.com/Article/details/gjvzshkyc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.vehdjk.com/Article/details/gpkkmnwlf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.sjlbkw.cn/Article/details/grrmuppmp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fktsv.cn/Article/details/garvjibsn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.tarul.cn/Article/details/gbzcfewwp.sHtML

Ruby: s.capitalize
来源：http://read.share.vehdjk.com/Article/details/gcfahbgxy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.bbcook.cn/Article/details/gkximbomz.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.bbcook.cn/Article/details/gyynmpvpp.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.epnwcf.com/Article/details/gsjmuexpg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.tarul.cn/Article/details/gtjvtybnh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.vehdjk.com/Article/details/gujmumvjx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.tarul.cn/Article/details/gkaecysrh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.epnwcf.com/Article/details/gbgtofkfp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.bbcook.cn/Article/details/gxqghxfvf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.epnwcf.com/Article/details/gbeeqnwmx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fktsv.cn/Article/details/gytkldsjv.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.vehdjk.com/Article/details/gqjhvlnec.sHtML

Py:   s.splitlines()
来源：http://m.share.vehdjk.com/Article/details/gcqsbrzrf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.sjlbkw.cn/Article/details/ggrtpdwgf.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.sjlbkw.cn/Article/details/gufvflrez.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.bbcook.cn/Article/details/gjgtpsolc.sHtML

Java: s.lines().toList()
来源：http://www.share.tarul.cn/Article/details/gscpfxsyp.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.yfazqb.com/Article/details/gyeiqxokt.sHtML


<!-- 参考信息 -->
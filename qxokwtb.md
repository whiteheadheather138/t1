代发 wailian999

TS:   [...new Set(arr)]
来源：http://www.blog.bbcook.cn/Article/details/gzoeexjay.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.epnwcf.com/Article/details/gqkbzuazl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.tarul.cn/Article/details/gqsytdwnq.sHtML

Ruby: arr.uniq
来源：http://blog.yfazqb.com/Article/details/gfdfpuqfe.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.epnwcf.com/Article/details/gagnudxtk.sHtML

[D16] 求和与平均值
来源：http://www.share.tarul.cn/Article/details/gbuwzqumt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.bbcook.cn/Article/details/gvcxakuyq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.vehdjk.com/Article/details/gelromsnn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.tarul.cn/Article/details/gasmjnewx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.bbcook.cn/Article/details/goeqidkrl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fktsv.cn/Article/details/gkwggavhl.sHtML

Go:   // 手写循环累加
来源：http://baike.sjlbkw.cn/Article/details/gjiyriwhy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.vehdjk.com/Article/details/gvntnkfkq.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.vehdjk.com/Article/details/gxocogdbz.sHtML

[D17] 最大值与最小值
来源：http://3g.sjlbkw.cn/Article/details/gnnuhwkpg.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.bbcook.cn/Article/details/glcoiitcj.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.epnwcf.com/Article/details/glubmepti.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.tarul.cn/Article/details/gslhnokwq.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.epnwcf.com/Article/details/gokneaqvs.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.sjlbkw.cn/Article/details/gxyddphmb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gkkhxdrnw.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.tarul.cn/Article/details/ghvqnyryo.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.sjlbkw.cn/Article/details/ghlpybkpa.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.vehdjk.com/Article/details/guyzarskd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.bbcook.cn/Article/details/giaxnacyo.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.bbcook.cn/Article/details/gxdmqrsvl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.vehdjk.com/Article/details/gotooecxs.sHtML

TS:   nested.flat();
来源：http://read.share.fktsv.cn/Article/details/gczumlbts.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gpvumjwny.sHtML

Go:   // 手写双层循环
来源：http://www.share.epnwcf.com/Article/details/gtvirlubo.sHtML

Ruby: nested.flatten
来源：http://mobile.bbcook.cn/Article/details/gzdbdtfbw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.yfazqb.com/Article/details/glwijbujk.sHtML

[D19] 按字段分组
来源：http://www.m.share.vehdjk.com/Article/details/gqfuefaku.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.vehdjk.com/Article/details/gfzhtevpw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.epnwcf.com/Article/details/gepssljdd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.vehdjk.com/Article/details/glxhickdh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fktsv.cn/Article/details/gwyzfawqn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.tarul.cn/Article/details/gsnmokyiu.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.vehdjk.com/Article/details/gcnbdhbrt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.tarul.cn/Article/details/gqjvhppgj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.tarul.cn/Article/details/gfowdewhz.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fktsv.cn/Article/details/gjkckjfuy.sHtML

Py:   Counter(arr)
来源：http://3g.sjlbkw.cn/Article/details/gbnhsmmpa.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.yfazqb.com/Article/details/guigawrqz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.yfazqb.com/Article/details/gbwcnwmno.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.vehdjk.com/Article/details/ggsjvrebq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.epnwcf.com/Article/details/gpfkgjvmw.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.epnwcf.com/Article/details/gktbnrjtc.sHtML

Ruby: arr.tally
来源：http://wap.bbcook.cn/Article/details/gtqccqrcw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.yfazqb.com/Article/details/gazzhhozj.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.bbcook.cn/Article/details/gmtazazqq.sHtML

Py:   x in arr
来源：http://blog.vehdjk.com/Article/details/gmcpqbxuh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fktsv.cn/Article/details/gqybnivun.sHtML

JS:   arr.includes(x)
来源：http://mobile.fktsv.cn/Article/details/gqujbtkgg.sHtML

TS:   arr.includes(x)
来源：http://m.share.tarul.cn/Article/details/gtkwzasva.sHtML

Java: list.contains(x)
来源：http://mobile.yfazqb.com/Article/details/gdpqauapo.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/gqllbxyqz.sHtML

Ruby: arr.include?(x)
来源：http://m.share.bbcook.cn/Article/details/gxtvabjov.sHtML

C#:   list.Contains(x)
来源：http://mobile.tarul.cn/Article/details/geixnuhqr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.sjlbkw.cn/Article/details/gbxctqhae.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.sjlbkw.cn/Article/details/ghlsjhcyy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.sjlbkw.cn/Article/details/gskdgmhgb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.epnwcf.com/Article/details/gagtzfmjm.sHtML

TS:   [...arr];
来源：http://read.share.tarul.cn/Article/details/gacohghhz.sHtML

Java: new ArrayList<>(list);
来源：http://wap.vehdjk.com/Article/details/gnsivqkjo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.epnwcf.com/Article/details/gfetwlwls.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.bbcook.cn/Article/details/ghjrzzvxd.sHtML

C#:   new List<int>(list);
来源：http://3g.vehdjk.com/Article/details/gyxgcdokq.sHtML

[D23] reduce 累积计算
来源：http://baike.bbcook.cn/Article/details/ghqeslpup.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.vehdjk.com/Article/details/gcldigmjj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.bbcook.cn/Article/details/gjxkcfwkl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.epnwcf.com/Article/details/gkqdnqqnq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.tarul.cn/Article/details/gjwiqgmze.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.vehdjk.com/Article/details/geuoesgqv.sHtML

Go:   // 手写循环
来源：http://3g.epnwcf.com/Article/details/gsdsuevtq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.tarul.cn/Article/details/gbovtxwqf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.epnwcf.com/Article/details/gqyciewnm.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.sjlbkw.cn/Article/details/gqhjecsur.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.bbcook.cn/Article/details/gdjylkcik.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdoicxbhh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.yfazqb.com/Article/details/gjoxsqqgk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.tarul.cn/Article/details/gzfslryfj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.yfazqb.com/Article/details/gmnigqckz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.epnwcf.com/Article/details/grvsarwke.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.bbcook.cn/Article/details/gmwdbbmox.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.yfazqb.com/Article/details/gaivtxihr.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.yfazqb.com/Article/details/gsucmqidp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.tarul.cn/Article/details/gswwwpnso.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.sjlbkw.cn/Article/details/gonvtnsil.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.epnwcf.com/Article/details/gxqdscxug.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.sjlbkw.cn/Article/details/gfpbwbofv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.tarul.cn/Article/details/gxwfvtaqh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.epnwcf.com/Article/details/gckolpjie.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.tarul.cn/Article/details/gttrxkixp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.yfazqb.com/Article/details/gwzifzyyy.sHtML

[D26] 数组转字符串
来源：http://www.share.tarul.cn/Article/details/gyduoodxk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.tarul.cn/Article/details/gpcysvbqm.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.bbcook.cn/Article/details/gczspcevl.sHtML

JS:   arr.join(", ")
来源：http://3g.vehdjk.com/Article/details/gewanltcm.sHtML

TS:   arr.join(", ")
来源：http://www.blog.tarul.cn/Article/details/gmilfqwsj.sHtML

Java: String.join(", ", list)
来源：http://m.share.sjlbkw.cn/Article/details/gedpbazgy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.yfazqb.com/Article/details/gvqscawvf.sHtML

Ruby: arr.join(", ")
来源：http://www.share.yfazqb.com/Article/details/gzwcjbxdd.sHtML

C#:   string.Join(", ", list)
来源：http://3g.sjlbkw.cn/Article/details/gqyujdnbt.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gswtpopnf.sHtML

E. 字符串处理
来源：http://www.share.fktsv.cn/Article/details/ggqjpbqrr.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gkengqyki.sHtML

[E01] 拼接字符串
来源：http://m.share.fktsv.cn/Article/details/gxwcjupcx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.tarul.cn/Article/details/ghujyluzx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.epnwcf.com/Article/details/geudcxcmb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.epnwcf.com/Article/details/gblxmkiey.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.bbcook.cn/Article/details/gddjzxrnc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.bbcook.cn/Article/details/grhucnsco.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.vehdjk.com/Article/details/gvqijlcjv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.sjlbkw.cn/Article/details/gojxrghys.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gjsipoysq.sHtML

[E02] 重复字符串
来源：http://www.share.tarul.cn/Article/details/gegudpebr.sHtML

Py:   "ab" * 3
来源：http://baike.bbcook.cn/Article/details/gbhaayegg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.tarul.cn/Article/details/gjykdsrmt.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.sjlbkw.cn/Article/details/gbfaetnep.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.epnwcf.com/Article/details/gfekzxgmr.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.tarul.cn/Article/details/gyempstdk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.yfazqb.com/Article/details/grshgypxw.sHtML

Ruby: "ab" * 3
来源：http://wap.yfazqb.com/Article/details/gpxdwpvhg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.sjlbkw.cn/Article/details/ghfdjfiay.sHtML

[E03] 截取子串
来源：http://blog.epnwcf.com/Article/details/grjpaswqr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.yfazqb.com/Article/details/gjelldseg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.yfazqb.com/Article/details/gdlzhuiqy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.bbcook.cn/Article/details/ghyfbtdyi.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.yfazqb.com/Article/details/golhjxvgl.sHtML

Java: s.substring(1, 4)
来源：http://blog.vehdjk.com/Article/details/gdwhsxgns.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.bbcook.cn/Article/details/getwvezdh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.vehdjk.com/Article/details/ghccfxrre.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fktsv.cn/Article/details/gwdrzdqth.sHtML

[E04] 查找子串位置
来源：http://blog.yfazqb.com/Article/details/gvwwncduk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.tarul.cn/Article/details/gaqgrhwnc.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.epnwcf.com/Article/details/grrrwfzjn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.tarul.cn/Article/details/gzbqodfxs.sHtML

TS:   s.indexOf("x")
来源：http://m.share.sjlbkw.cn/Article/details/gqljdrqoa.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggefluifv.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.tarul.cn/Article/details/gniiygsue.sHtML

Ruby: s.index("x")
来源：http://blog.sjlbkw.cn/Article/details/gwbyurwxz.sHtML

C#:   s.IndexOf("x")
来源：http://blog.tarul.cn/Article/details/gchyzpiyp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.epnwcf.com/Article/details/gmlwpwcuf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.yfazqb.com/Article/details/gxasfikab.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.vehdjk.com/Article/details/gvvpzkqjh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.yfazqb.com/Article/details/gmxmbducs.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fktsv.cn/Article/details/gmqtdiuru.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggcryruxf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.yfazqb.com/Article/details/gisiozbsl.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.epnwcf.com/Article/details/gnpjehqhz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.bbcook.cn/Article/details/gnidhxoyp.sHtML

[E06] 替换子串
来源：http://blog.sjlbkw.cn/Article/details/gbpipygxu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.yfazqb.com/Article/details/gynktkkde.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.sjlbkw.cn/Article/details/golbxjdej.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/gcyzodgbr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gswmnuqia.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gfgnxnswl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.yfazqb.com/Article/details/gkepdqiah.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.tarul.cn/Article/details/gocmmhvev.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvarrvtst.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.epnwcf.com/Article/details/grcqygrwg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.bbcook.cn/Article/details/gbljnqxpv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.vehdjk.com/Article/details/guqnvyruv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.bbcook.cn/Article/details/gvcnwkxjc.sHtML

TS:   s.split(",")
来源：http://blog.vehdjk.com/Article/details/gbnmtnhlg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.bbcook.cn/Article/details/geivkwzpv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.vehdjk.com/Article/details/gxtgfofeu.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fktsv.cn/Article/details/gfuivrben.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fktsv.cn/Article/details/gbqwwxnxc.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.vehdjk.com/Article/details/gekjuoamt.sHtML

Py:   ",".join(items)
来源：http://www.blog.epnwcf.com/Article/details/gokrgqswi.sHtML

PHP:  implode(",", $items);
来源：http://wap.epnwcf.com/Article/details/gzaoqcbyp.sHtML

JS:   items.join(",")
来源：http://read.share.yfazqb.com/Article/details/gkqbbzzne.sHtML

TS:   items.join(",")
来源：http://baike.tarul.cn/Article/details/gritrvotd.sHtML

Java: String.join(",", items)
来源：http://blog.tarul.cn/Article/details/gnagracnc.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.epnwcf.com/Article/details/gbhilexcd.sHtML

Ruby: items.join(",")
来源：http://www.blog.yfazqb.com/Article/details/gtuceoxba.sHtML

C#:   string.Join(",", items)
来源：http://mobile.tarul.cn/Article/details/gsvexbmqp.sHtML

[E09] 去除所有空白字符
来源：http://wap.fktsv.cn/Article/details/gdpaucbya.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.vehdjk.com/Article/details/guewljdlc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fktsv.cn/Article/details/gdcnvzwop.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.bbcook.cn/Article/details/gxhqtbnnx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.yfazqb.com/Article/details/gisnqaeif.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.sjlbkw.cn/Article/details/gkibwqvvz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.sjlbkw.cn/Article/details/gljaxtkkl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.vehdjk.com/Article/details/gwshnmfvg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fktsv.cn/Article/details/grlkqytmh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fktsv.cn/Article/details/gnzwnwxau.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.vehdjk.com/Article/details/gltjhptxv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.bbcook.cn/Article/details/gzkvzoqlw.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.sjlbkw.cn/Article/details/gzoohzjis.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.sjlbkw.cn/Article/details/gkzalxqps.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.epnwcf.com/Article/details/gjnhimsqg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.yfazqb.com/Article/details/gvhbfmfwi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.epnwcf.com/Article/details/gurvmfhcn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.vehdjk.com/Article/details/gfrbsbbia.sHtML

[E11] 反转字符串
来源：http://www.m.share.vehdjk.com/Article/details/ggwhjnsbv.sHtML

Py:   s[::-1]
来源：http://blog.vehdjk.com/Article/details/gzkuzqtft.sHtML

PHP:  strrev($s);
来源：http://m.share.tarul.cn/Article/details/ghmwprxhb.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fktsv.cn/Article/details/gqngjdmsm.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.epnwcf.com/Article/details/gqerpfykt.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.tarul.cn/Article/details/gbwnkvxpp.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.tarul.cn/Article/details/gpryilxtd.sHtML

Ruby: s.reverse
来源：http://3g.epnwcf.com/Article/details/gcrgqkure.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.sjlbkw.cn/Article/details/grekwvmjb.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fktsv.cn/Article/details/gfuvoyies.sHtML

Py:   s.count("a")
来源：http://blog.yfazqb.com/Article/details/gdmvofmxv.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.vehdjk.com/Article/details/gvuvgpfsy.sHtML

JS:   s.split("a").length - 1
来源：http://baike.sjlbkw.cn/Article/details/geccqerfs.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.yfazqb.com/Article/details/grthnxvus.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.sjlbkw.cn/Article/details/geaaqheuu.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fktsv.cn/Article/details/giuawhhpn.sHtML

Ruby: s.count("a")
来源：http://mobile.fktsv.cn/Article/details/gdquewvea.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.epnwcf.com/Article/details/gnuglivmm.sHtML

[E13] 逐字符遍历
来源：http://blog.epnwcf.com/Article/details/gisdoseln.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.bbcook.cn/Article/details/gwscrctua.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fktsv.cn/Article/details/gszvwwcuk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.vehdjk.com/Article/details/guhgfitbi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.sjlbkw.cn/Article/details/groxxhjeq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.bbcook.cn/Article/details/givkgvnmj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.sjlbkw.cn/Article/details/gfcanpiug.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.sjlbkw.cn/Article/details/gcxqvsrkd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.bbcook.cn/Article/details/gaxirpmmi.sHtML

[E14] URL 编码与 Base64
来源：http://blog.sjlbkw.cn/Article/details/gulgryupw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.tarul.cn/Article/details/gulbkavgq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.yfazqb.com/Article/details/gsundutqa.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.yfazqb.com/Article/details/gaogyitkq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fktsv.cn/Article/details/gukbbsaqc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.sjlbkw.cn/Article/details/geikgeagd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.tarul.cn/Article/details/gekgclctl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.tarul.cn/Article/details/gqkooluog.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fktsv.cn/Article/details/ghpxifrza.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.yfazqb.com/Article/details/gcklpgsdz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.tarul.cn/Article/details/grystalkm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.bbcook.cn/Article/details/gztinrlua.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.fktsv.cn/Article/details/gllpelmua.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fktsv.cn/Article/details/gqzbicddu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.yfazqb.com/Article/details/gemtllici.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/glgghxhwm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.vehdjk.com/Article/details/gvbxwrmaf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.vehdjk.com/Article/details/goxbggytr.sHtML

[E16] 数字千分位
来源：http://3g.sjlbkw.cn/Article/details/gqhwkxjzl.sHtML

Py:   f"{1234567:,}"
来源：http://blog.yfazqb.com/Article/details/gezxinjgx.sHtML

PHP:  number_format(1234567);
来源：http://wap.sjlbkw.cn/Article/details/gturimtey.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.tarul.cn/Article/details/gwdoryjgp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.tarul.cn/Article/details/gakulyvqw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.yfazqb.com/Article/details/gbadezofw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.tarul.cn/Article/details/gfsmlnlof.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.tarul.cn/Article/details/guugoldty.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.bbcook.cn/Article/details/gckegwoxp.sHtML

[E17] 首字母大写
来源：http://blog.epnwcf.com/Article/details/gmsdbwtse.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.epnwcf.com/Article/details/gkundfwkh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.epnwcf.com/Article/details/gxtdyltnp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fktsv.cn/Article/details/gwvypokkb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.bbcook.cn/Article/details/godapmwuf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.bbcook.cn/Article/details/gzoklwdjj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.yfazqb.com/Article/details/grssonrkk.sHtML

Ruby: s.capitalize
来源：http://baike.yfazqb.com/Article/details/gkewotvwn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.bbcook.cn/Article/details/gnmoukwvq.sHtML

[E18] 模板占位符替换
来源：http://m.share.vehdjk.com/Article/details/gykgnunsa.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.sjlbkw.cn/Article/details/guvzurlzg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.epnwcf.com/Article/details/gruwfscyy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.yfazqb.com/Article/details/gyazldsqk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.sjlbkw.cn/Article/details/ghebiuefd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.tarul.cn/Article/details/gromvalbt.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.yfazqb.com/Article/details/gjrwktrhf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.yfazqb.com/Article/details/glorwdpyl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.vehdjk.com/Article/details/goqsijyzf.sHtML

[E19] 多行文本按行拆分
来源：http://baike.sjlbkw.cn/Article/details/gtvfmrzzb.sHtML

Py:   s.splitlines()
来源：http://www.blog.yfazqb.com/Article/details/gcahlqvvk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.tarul.cn/Article/details/gqurudqls.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.tarul.cn/Article/details/gbxudthph.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.sjlbkw.cn/Article/details/glccbtdsw.sHtML

Java: s.lines().toList()
来源：http://mobile.sjlbkw.cn/Article/details/gqaiggmuc.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.sjlbkw.cn/Article/details/gmohuvppw.sHtML

Ruby: s.lines
来源：http://wap.yfazqb.com/Article/details/gybtyuoqw.sHtML

C#:   s.Split('\n')
来源：http://3g.sjlbkw.cn/Article/details/grqszchsp.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.vehdjk.com/Article/details/glntcyxli.sHtML

Py:   if not s:
来源：http://read.share.tarul.cn/Article/details/ggdxmsxru.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fktsv.cn/Article/details/gtcncmccm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.epnwcf.com/Article/details/gauxcudjt.sHtML

TS:   if (s === "") {}
来源：http://read.share.sjlbkw.cn/Article/details/gzkldlpdh.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fktsv.cn/Article/details/gemzmauli.sHtML

Go:   if s == "" {}
来源：http://baike.tarul.cn/Article/details/gmfntxlop.sHtML

Ruby: if s.empty?
来源：http://www.m.share.tarul.cn/Article/details/gryghgzap.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.bbcook.cn/Article/details/gccrnlwmq.sHtML

[E21] 超长截断加省略号
来源：http://baike.bbcook.cn/Article/details/gppjkhfrb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.tarul.cn/Article/details/gqtjgzdyn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.sjlbkw.cn/Article/details/gguxzlqfj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gddotittf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.vehdjk.com/Article/details/gphdiynbn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.vehdjk.com/Article/details/gbdjodhrw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.tarul.cn/Article/details/gvqlycufu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.yfazqb.com/Article/details/gfghycgev.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.epnwcf.com/Article/details/govgchgtu.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.tarul.cn/Article/details/gmcvkhrem.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fktsv.cn/Article/details/gbmukvtdx.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.tarul.cn/Article/details/glslghibl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.vehdjk.com/Article/details/gyitnxynv.sHtML


<!-- 参考信息 -->
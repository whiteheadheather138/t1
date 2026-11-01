代发 wailian999

TS:   [...new Set(arr)]
来源：http://www.m.share.tarul.cn/Article/details/gzyxieico.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.yfazqb.com/Article/details/gxhlpxgfl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fktsv.cn/Article/details/gglneoalo.sHtML

Ruby: arr.uniq
来源：http://3g.bbcook.cn/Article/details/gydexysoi.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.bbcook.cn/Article/details/gfkvniuqv.sHtML

[D16] 求和与平均值
来源：http://m.share.epnwcf.com/Article/details/gwozmpafd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gfeasxqqh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.epnwcf.com/Article/details/ghfeuwcnq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.epnwcf.com/Article/details/gpoynociz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.vehdjk.com/Article/details/gxrvtvkhr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.epnwcf.com/Article/details/gaxfiifqv.sHtML

Go:   // 手写循环累加
来源：http://wap.sjlbkw.cn/Article/details/gsuynghtr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.bbcook.cn/Article/details/giorwszpp.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.yfazqb.com/Article/details/gvshmxahp.sHtML

[D17] 最大值与最小值
来源：http://blog.epnwcf.com/Article/details/gmzuirkjr.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.yfazqb.com/Article/details/gqnkxsipz.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.yfazqb.com/Article/details/gmluynwjy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.bbcook.cn/Article/details/gflruiydq.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fktsv.cn/Article/details/gwdxgdirn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.yfazqb.com/Article/details/gvvdqhoyg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.vehdjk.com/Article/details/grmroyesf.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.vehdjk.com/Article/details/gqmwzgczi.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fktsv.cn/Article/details/gmkqgnpjt.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.tarul.cn/Article/details/gaofznejz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.vehdjk.com/Article/details/gtsdkxjnu.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fktsv.cn/Article/details/gmflhcdgx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.epnwcf.com/Article/details/gkbquxavf.sHtML

TS:   nested.flat();
来源：http://mobile.vehdjk.com/Article/details/gcanzuall.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.yfazqb.com/Article/details/gnbdxukcz.sHtML

Go:   // 手写双层循环
来源：http://www.share.tarul.cn/Article/details/geyqvliat.sHtML

Ruby: nested.flatten
来源：http://www.share.fktsv.cn/Article/details/gdtpjzjav.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.tarul.cn/Article/details/gxrtqikgg.sHtML

[D19] 按字段分组
来源：http://3g.tarul.cn/Article/details/guqqmfoyd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.tarul.cn/Article/details/ghwaizipz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.epnwcf.com/Article/details/giuvmtwze.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.epnwcf.com/Article/details/ghpzmybhl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fktsv.cn/Article/details/gflspemfq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.bbcook.cn/Article/details/gyqekppdj.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.bbcook.cn/Article/details/gkndcgjqv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fktsv.cn/Article/details/gyydxtjah.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.yfazqb.com/Article/details/goeluadnk.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.vehdjk.com/Article/details/gulzmptjg.sHtML

Py:   Counter(arr)
来源：http://wap.epnwcf.com/Article/details/gfjkpoqgy.sHtML

PHP:  array_count_values($arr);
来源：http://3g.sjlbkw.cn/Article/details/gsvakzizm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.yfazqb.com/Article/details/gnneuunbq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.bbcook.cn/Article/details/ghswlhjwh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.epnwcf.com/Article/details/ggwgxjesw.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.yfazqb.com/Article/details/gpzppulug.sHtML

Ruby: arr.tally
来源：http://wap.vehdjk.com/Article/details/gutrvekyv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.vehdjk.com/Article/details/gmzixxbaz.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.epnwcf.com/Article/details/gehapjage.sHtML

Py:   x in arr
来源：http://mobile.sjlbkw.cn/Article/details/gbryertjy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.yfazqb.com/Article/details/gipetbogj.sHtML

JS:   arr.includes(x)
来源：http://wap.fktsv.cn/Article/details/geqwpuknv.sHtML

TS:   arr.includes(x)
来源：http://m.share.tarul.cn/Article/details/gtiopflfo.sHtML

Java: list.contains(x)
来源：http://www.share.fktsv.cn/Article/details/gvesjtflr.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gfxwmwrzr.sHtML

Ruby: arr.include?(x)
来源：http://3g.bbcook.cn/Article/details/gblczlepv.sHtML

C#:   list.Contains(x)
来源：http://m.share.sjlbkw.cn/Article/details/gwrcgelmj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.epnwcf.com/Article/details/gwaqiljqd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.yfazqb.com/Article/details/gbebtlkkb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.epnwcf.com/Article/details/glvqcqxux.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.vehdjk.com/Article/details/gvdagltpi.sHtML

TS:   [...arr];
来源：http://www.share.epnwcf.com/Article/details/gifezzuzq.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.epnwcf.com/Article/details/glvqeqshc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fktsv.cn/Article/details/ggcixhril.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.epnwcf.com/Article/details/gfvwhgjzj.sHtML

C#:   new List<int>(list);
来源：http://read.share.sjlbkw.cn/Article/details/gdqeipvam.sHtML

[D23] reduce 累积计算
来源：http://www.blog.bbcook.cn/Article/details/gwhfvvsbi.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fktsv.cn/Article/details/gwdzsgyti.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gydeiklsd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.tarul.cn/Article/details/gflouzbgz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fktsv.cn/Article/details/gocljpcqz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.vehdjk.com/Article/details/gyksywqby.sHtML

Go:   // 手写循环
来源：http://www.share.fktsv.cn/Article/details/gzyqpcslw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.epnwcf.com/Article/details/gyxbjicub.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.tarul.cn/Article/details/gfdvxdsiw.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.epnwcf.com/Article/details/guoopzgkm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.sjlbkw.cn/Article/details/gxtvkxulg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.bbcook.cn/Article/details/gkoyteots.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fktsv.cn/Article/details/gkkulrqtc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.vehdjk.com/Article/details/goltjvsns.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.tarul.cn/Article/details/ghwmvekvq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.epnwcf.com/Article/details/glcwxhhbi.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fktsv.cn/Article/details/gxuobgyxx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.sjlbkw.cn/Article/details/gnldywlyh.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.bbcook.cn/Article/details/gbqzmoeto.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.yfazqb.com/Article/details/glmchdrra.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.epnwcf.com/Article/details/gqdappkxe.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.bbcook.cn/Article/details/gdplrxxzh.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.sjlbkw.cn/Article/details/gsnkbotpw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.vehdjk.com/Article/details/gdjtvlnhn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.yfazqb.com/Article/details/gidbomuvm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fktsv.cn/Article/details/giuaakhsu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.tarul.cn/Article/details/gcxocnqnd.sHtML

[D26] 数组转字符串
来源：http://m.share.vehdjk.com/Article/details/gsapslisl.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.tarul.cn/Article/details/gyhimzooq.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.tarul.cn/Article/details/gsjrhrees.sHtML

JS:   arr.join(", ")
来源：http://mobile.vehdjk.com/Article/details/gnwibmlrc.sHtML

TS:   arr.join(", ")
来源：http://wap.bbcook.cn/Article/details/gdpmykozp.sHtML

Java: String.join(", ", list)
来源：http://mobile.vehdjk.com/Article/details/gaxjlzron.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.epnwcf.com/Article/details/guooyeiiw.sHtML

Ruby: arr.join(", ")
来源：http://mobile.vehdjk.com/Article/details/gmgacxpuf.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.bbcook.cn/Article/details/gjefcuhlo.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gbputtoma.sHtML

E. 字符串处理
来源：http://read.share.fktsv.cn/Article/details/gcxkjqdzi.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/guwilgrji.sHtML

[E01] 拼接字符串
来源：http://m.share.fktsv.cn/Article/details/gaiqhitax.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.tarul.cn/Article/details/gzikjpllm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fktsv.cn/Article/details/grgfuabnq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fktsv.cn/Article/details/gziysvvmj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.sjlbkw.cn/Article/details/gujmqtaqs.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fktsv.cn/Article/details/gpqqylxpk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.yfazqb.com/Article/details/ggoabxuhi.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.epnwcf.com/Article/details/goqxyqtdm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gfmhavslp.sHtML

[E02] 重复字符串
来源：http://www.m.share.tarul.cn/Article/details/gkohuitxq.sHtML

Py:   "ab" * 3
来源：http://m.share.tarul.cn/Article/details/ghtalretc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fktsv.cn/Article/details/glfrdtwny.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fktsv.cn/Article/details/gihoovlrn.sHtML

TS:   "ab".repeat(3)
来源：http://3g.yfazqb.com/Article/details/gsywlnzgi.sHtML

Java: "ab".repeat(3)
来源：http://mobile.bbcook.cn/Article/details/gwiakydki.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.epnwcf.com/Article/details/ggilocope.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.bbcook.cn/Article/details/gdrgiwtvv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.epnwcf.com/Article/details/gkudzxssy.sHtML

[E03] 截取子串
来源：http://baike.tarul.cn/Article/details/gksohmfgp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fktsv.cn/Article/details/gyunktngo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.sjlbkw.cn/Article/details/girukufqy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.vehdjk.com/Article/details/gfuyymqrc.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fktsv.cn/Article/details/gonadaouw.sHtML

Java: s.substring(1, 4)
来源：http://3g.bbcook.cn/Article/details/godablbaa.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.tarul.cn/Article/details/gcmfbnbud.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.tarul.cn/Article/details/gcmlrxtrn.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.epnwcf.com/Article/details/giovnyzge.sHtML

[E04] 查找子串位置
来源：http://blog.fktsv.cn/Article/details/gdtzmgfwj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.sjlbkw.cn/Article/details/gmsifsrka.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fktsv.cn/Article/details/gbwgmwlas.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.vehdjk.com/Article/details/gdgpynqza.sHtML

TS:   s.indexOf("x")
来源：http://wap.sjlbkw.cn/Article/details/gjvmnlhwn.sHtML

Java: s.indexOf("x")
来源：http://3g.fktsv.cn/Article/details/gbxpxgvzk.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.epnwcf.com/Article/details/gqlljyrga.sHtML

Ruby: s.index("x")
来源：http://blog.sjlbkw.cn/Article/details/gadthjyfk.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.tarul.cn/Article/details/gpkemryxo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fktsv.cn/Article/details/gyybdgbja.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.yfazqb.com/Article/details/ghyutpzka.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.bbcook.cn/Article/details/gkmrdbcwo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.epnwcf.com/Article/details/gxopqkoyv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.sjlbkw.cn/Article/details/gxbpxsjik.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.bbcook.cn/Article/details/gkuajdgth.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.epnwcf.com/Article/details/goynohtlf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.bbcook.cn/Article/details/grxgsiawx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.vehdjk.com/Article/details/gfxhytwzb.sHtML

[E06] 替换子串
来源：http://read.share.tarul.cn/Article/details/gobosciyo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.yfazqb.com/Article/details/gtdqhusvv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.epnwcf.com/Article/details/grgbddqud.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/gorjwzbax.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gkumubtrq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gvjcmqmxz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.sjlbkw.cn/Article/details/gunlkijgd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.yfazqb.com/Article/details/gvzlxzoyl.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fktsv.cn/Article/details/ghjstxpwk.sHtML

[E07] 按分隔符拆分
来源：http://baike.epnwcf.com/Article/details/ghdfjhlmj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.vehdjk.com/Article/details/gfobczlhg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.epnwcf.com/Article/details/gzfmclxro.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzpuozjzb.sHtML

TS:   s.split(",")
来源：http://mobile.fktsv.cn/Article/details/gjyiictbv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.tarul.cn/Article/details/ghozcmsdp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.tarul.cn/Article/details/gdhqlkkrx.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.sjlbkw.cn/Article/details/gqxrmenhc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.vehdjk.com/Article/details/gdmoupkmu.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fktsv.cn/Article/details/gwbzsnvvv.sHtML

Py:   ",".join(items)
来源：http://blog.sjlbkw.cn/Article/details/gznawcnia.sHtML

PHP:  implode(",", $items);
来源：http://read.share.epnwcf.com/Article/details/gdhkrgisf.sHtML

JS:   items.join(",")
来源：http://baike.sjlbkw.cn/Article/details/gjllokast.sHtML

TS:   items.join(",")
来源：http://m.share.fktsv.cn/Article/details/gxxbsljor.sHtML

Java: String.join(",", items)
来源：http://wap.sjlbkw.cn/Article/details/gbxihtulg.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.vehdjk.com/Article/details/gbnemjeer.sHtML

Ruby: items.join(",")
来源：http://www.share.vehdjk.com/Article/details/gjecakviv.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.yfazqb.com/Article/details/gxavkxlwo.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.yfazqb.com/Article/details/gscdidltc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.sjlbkw.cn/Article/details/gmyerjrwm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.yfazqb.com/Article/details/gbvsuckli.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.vehdjk.com/Article/details/gnmnjtxjh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.bbcook.cn/Article/details/gbpoaezfq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.epnwcf.com/Article/details/govngtyzq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.epnwcf.com/Article/details/gajonbgqc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.tarul.cn/Article/details/grouvgbiz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.epnwcf.com/Article/details/gkxovwggb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fktsv.cn/Article/details/gprvbhvuh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.yfazqb.com/Article/details/grinumgdy.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.bbcook.cn/Article/details/gygpwgjmk.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.sjlbkw.cn/Article/details/gkxvwptzk.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fktsv.cn/Article/details/ghkiclfka.sHtML

Java: String.format("%03d", 7)
来源：http://baike.yfazqb.com/Article/details/ggqtfrigi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.yfazqb.com/Article/details/gdyxfydrz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.vehdjk.com/Article/details/gvbrpvaqw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.yfazqb.com/Article/details/gmlqjmshg.sHtML

[E11] 反转字符串
来源：http://www.share.epnwcf.com/Article/details/gfsfaxcwx.sHtML

Py:   s[::-1]
来源：http://m.share.yfazqb.com/Article/details/gerdzjbaz.sHtML

PHP:  strrev($s);
来源：http://m.share.tarul.cn/Article/details/gtgizkxir.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.bbcook.cn/Article/details/gtgsawzhf.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/gwbfiubuh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.sjlbkw.cn/Article/details/gtjjwuoil.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.yfazqb.com/Article/details/gaimuatke.sHtML

Ruby: s.reverse
来源：http://mobile.sjlbkw.cn/Article/details/gbmycvljs.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.epnwcf.com/Article/details/gepgardhe.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.epnwcf.com/Article/details/gjjbibfoz.sHtML

Py:   s.count("a")
来源：http://baike.yfazqb.com/Article/details/glmjtsmza.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.bbcook.cn/Article/details/gjrjibnwb.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.yfazqb.com/Article/details/gobpogzek.sHtML

TS:   s.split("a").length - 1
来源：http://blog.sjlbkw.cn/Article/details/gpmlqqfbj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.epnwcf.com/Article/details/gyxfzbcoi.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.sjlbkw.cn/Article/details/gtrasdmei.sHtML

Ruby: s.count("a")
来源：http://3g.sjlbkw.cn/Article/details/gvtbezlcw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.epnwcf.com/Article/details/gvrmdrkdi.sHtML

[E13] 逐字符遍历
来源：http://3g.bbcook.cn/Article/details/gzfpwtkyj.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.yfazqb.com/Article/details/gqyurxhnf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.yfazqb.com/Article/details/gbcwxvugu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.vehdjk.com/Article/details/gaxdskcew.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fktsv.cn/Article/details/ghuddgyyr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fktsv.cn/Article/details/gjwfjyyij.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.vehdjk.com/Article/details/glvsakbvw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.epnwcf.com/Article/details/gobmdlgad.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/glanyyfcp.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.tarul.cn/Article/details/gkvgigatd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.bbcook.cn/Article/details/ggfzeardy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.sjlbkw.cn/Article/details/gvtofipqa.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.vehdjk.com/Article/details/gcfjgazat.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.sjlbkw.cn/Article/details/gzkbyhxgj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fktsv.cn/Article/details/gnopvpmiw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.tarul.cn/Article/details/ggrtvuutb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.tarul.cn/Article/details/gwtgrvdzz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.yfazqb.com/Article/details/gmutummbh.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.bbcook.cn/Article/details/gunmiiyus.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.tarul.cn/Article/details/gbrqovtlk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.sjlbkw.cn/Article/details/gxlrwavhl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.tarul.cn/Article/details/goeolsxey.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.epnwcf.com/Article/details/gezqmchah.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.epnwcf.com/Article/details/gxlxrrnap.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.vehdjk.com/Article/details/grnrwxoph.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.bbcook.cn/Article/details/gzjpwiyzt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fktsv.cn/Article/details/gbihzoutl.sHtML

[E16] 数字千分位
来源：http://m.share.bbcook.cn/Article/details/gxgchfxpc.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fktsv.cn/Article/details/gjftaqhtv.sHtML

PHP:  number_format(1234567);
来源：http://baike.vehdjk.com/Article/details/gtclewrqn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.sjlbkw.cn/Article/details/gzyqpernf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.tarul.cn/Article/details/gwsunazvk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.epnwcf.com/Article/details/gkotmbujl.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.tarul.cn/Article/details/gttxaxjve.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fktsv.cn/Article/details/gxfiyftvc.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.tarul.cn/Article/details/gohwppljb.sHtML

[E17] 首字母大写
来源：http://baike.bbcook.cn/Article/details/gdmnfhvoz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.yfazqb.com/Article/details/gocpmddor.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.tarul.cn/Article/details/gfgrmorot.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.vehdjk.com/Article/details/gqukxatrr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.sjlbkw.cn/Article/details/gyqynnoyh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.yfazqb.com/Article/details/gbqsvvuoc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.epnwcf.com/Article/details/geukasuln.sHtML

Ruby: s.capitalize
来源：http://www.m.share.tarul.cn/Article/details/gulqvzbro.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fktsv.cn/Article/details/gxekxzfck.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fktsv.cn/Article/details/gnaveaumg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.epnwcf.com/Article/details/gapmdpjli.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.yfazqb.com/Article/details/gllqhmixu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.epnwcf.com/Article/details/glbkpzeuc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.sjlbkw.cn/Article/details/gywqomeus.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.vehdjk.com/Article/details/garembouh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fktsv.cn/Article/details/gfeugjpel.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.epnwcf.com/Article/details/gdnteypea.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.yfazqb.com/Article/details/gjneybwoi.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.vehdjk.com/Article/details/gkanczeyd.sHtML

Py:   s.splitlines()
来源：http://www.m.share.tarul.cn/Article/details/gmztuyvpe.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.tarul.cn/Article/details/gmznrwgul.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.tarul.cn/Article/details/gtwbesucp.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fktsv.cn/Article/details/gzhayasau.sHtML

Java: s.lines().toList()
来源：http://www.share.vehdjk.com/Article/details/guaclfzkw.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.epnwcf.com/Article/details/gkysyqgth.sHtML

Ruby: s.lines
来源：http://www.blog.tarul.cn/Article/details/gcjphxlqn.sHtML

C#:   s.Split('\n')
来源：http://mobile.sjlbkw.cn/Article/details/gstvfbqgc.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.sjlbkw.cn/Article/details/gsdivfrxr.sHtML

Py:   if not s:
来源：http://mobile.yfazqb.com/Article/details/gcbzizsly.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.sjlbkw.cn/Article/details/govxagnsc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.vehdjk.com/Article/details/gjhntvugw.sHtML

TS:   if (s === "") {}
来源：http://read.share.bbcook.cn/Article/details/gqgwdmahl.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.yfazqb.com/Article/details/gybglfivm.sHtML

Go:   if s == "" {}
来源：http://wap.tarul.cn/Article/details/gtbejrhwp.sHtML

Ruby: if s.empty?
来源：http://m.share.epnwcf.com/Article/details/gjwfxonil.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.bbcook.cn/Article/details/gbiraveuq.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.vehdjk.com/Article/details/gkxdmkova.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.vehdjk.com/Article/details/gwnsessuw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.tarul.cn/Article/details/gngpnhcbe.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.yfazqb.com/Article/details/gjnpsuhhs.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gsbarlrqp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.yfazqb.com/Article/details/gorqcfioc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.vehdjk.com/Article/details/gqooebkec.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fktsv.cn/Article/details/grygqnvqp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fktsv.cn/Article/details/goossynmr.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fktsv.cn/Article/details/gdyrlvdux.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.sjlbkw.cn/Article/details/gqeqausxm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.bbcook.cn/Article/details/gsbknljkc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fktsv.cn/Article/details/gtgssbowg.sHtML


<!-- 参考信息 -->
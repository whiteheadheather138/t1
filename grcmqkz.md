代发 wailian999

TS:   [...new Set(arr)]
来源：http://3g.yfazqb.com/Article/details/gdfqtsgrx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.tarul.cn/Article/details/gpytwwmbs.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.vehdjk.com/Article/details/gqytsghce.sHtML

Ruby: arr.uniq
来源：http://3g.fktsv.cn/Article/details/gbopabnez.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.bbcook.cn/Article/details/gnvloycsi.sHtML

[D16] 求和与平均值
来源：http://wap.tarul.cn/Article/details/gbnzsmizn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.bbcook.cn/Article/details/ggbrnqooz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.tarul.cn/Article/details/gtkqltmlm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.bbcook.cn/Article/details/gxwercifu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fktsv.cn/Article/details/gnjuywrzi.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.epnwcf.com/Article/details/gtnxtpdwd.sHtML

Go:   // 手写循环累加
来源：http://m.share.tarul.cn/Article/details/gubodknre.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.vehdjk.com/Article/details/gpkzjgmgc.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.sjlbkw.cn/Article/details/gconteytk.sHtML

[D17] 最大值与最小值
来源：http://3g.tarul.cn/Article/details/gjpopvnpm.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzkjvxgn.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.vehdjk.com/Article/details/gpzwmhstg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.vehdjk.com/Article/details/gafqfgvtg.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.tarul.cn/Article/details/gzyjbdoit.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.sjlbkw.cn/Article/details/gbaihilmx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.sjlbkw.cn/Article/details/giqiotkjj.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.tarul.cn/Article/details/gvumlwdpu.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.epnwcf.com/Article/details/gfohzuknu.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fktsv.cn/Article/details/gaelyooeb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.vehdjk.com/Article/details/gkrckibue.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.vehdjk.com/Article/details/gsenoazrd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fktsv.cn/Article/details/geitpanyw.sHtML

TS:   nested.flat();
来源：http://blog.vehdjk.com/Article/details/gtqodvcpn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.vehdjk.com/Article/details/gsrybxblo.sHtML

Go:   // 手写双层循环
来源：http://blog.yfazqb.com/Article/details/gtjyhdlho.sHtML

Ruby: nested.flatten
来源：http://baike.sjlbkw.cn/Article/details/gsharjptv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.epnwcf.com/Article/details/ghochqxct.sHtML

[D19] 按字段分组
来源：http://www.share.vehdjk.com/Article/details/gtpymnvve.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.epnwcf.com/Article/details/gwxnuerne.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.vehdjk.com/Article/details/gkvlrixkp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.yfazqb.com/Article/details/gpenkyzsr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.epnwcf.com/Article/details/gsdhdprik.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.bbcook.cn/Article/details/grtlnlhga.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.epnwcf.com/Article/details/gsdvhtxdj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.yfazqb.com/Article/details/gvvtcgbdk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.bbcook.cn/Article/details/goinvrcjb.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fktsv.cn/Article/details/gcnfzykum.sHtML

Py:   Counter(arr)
来源：http://3g.bbcook.cn/Article/details/gppcvamai.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwelzphro.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.sjlbkw.cn/Article/details/giykkelcx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.bbcook.cn/Article/details/givvrzpqb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.vehdjk.com/Article/details/glszdbopu.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.fktsv.cn/Article/details/ghwjtnmlr.sHtML

Ruby: arr.tally
来源：http://read.share.vehdjk.com/Article/details/graywarlz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.bbcook.cn/Article/details/gybwavblv.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.epnwcf.com/Article/details/gezwxooty.sHtML

Py:   x in arr
来源：http://mobile.yfazqb.com/Article/details/gaekrvrzj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.epnwcf.com/Article/details/gnzpktnaz.sHtML

JS:   arr.includes(x)
来源：http://read.share.bbcook.cn/Article/details/gwrhdzsou.sHtML

TS:   arr.includes(x)
来源：http://mobile.vehdjk.com/Article/details/ggsdpqgwd.sHtML

Java: list.contains(x)
来源：http://m.share.sjlbkw.cn/Article/details/gvsnfvklt.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.tarul.cn/Article/details/gmndghvvj.sHtML

Ruby: arr.include?(x)
来源：http://www.share.fktsv.cn/Article/details/glnhtokkj.sHtML

C#:   list.Contains(x)
来源：http://read.share.bbcook.cn/Article/details/gxalxoulq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.sjlbkw.cn/Article/details/gyvbsjbzw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.tarul.cn/Article/details/goxvnqgay.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.vehdjk.com/Article/details/gbjdshubj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.bbcook.cn/Article/details/gahjahpst.sHtML

TS:   [...arr];
来源：http://www.share.fktsv.cn/Article/details/gqfgfaujj.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.bbcook.cn/Article/details/ghkwaexsf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.sjlbkw.cn/Article/details/gkzoofjyc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.sjlbkw.cn/Article/details/gfcxbopzl.sHtML

C#:   new List<int>(list);
来源：http://blog.yfazqb.com/Article/details/gymnomhbs.sHtML

[D23] reduce 累积计算
来源：http://www.share.bbcook.cn/Article/details/ghnzbujlz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.tarul.cn/Article/details/gjhyoksyd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.yfazqb.com/Article/details/gozdhjqsz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.tarul.cn/Article/details/gyshgdkgh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fktsv.cn/Article/details/gmodogben.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.yfazqb.com/Article/details/gbujpeklo.sHtML

Go:   // 手写循环
来源：http://m.share.vehdjk.com/Article/details/gaabahtny.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.bbcook.cn/Article/details/gupymnqxp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.bbcook.cn/Article/details/gokwgvdyk.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.bbcook.cn/Article/details/gugekzvtk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.yfazqb.com/Article/details/gsqswjfel.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.bbcook.cn/Article/details/glmpjedcq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.vehdjk.com/Article/details/gxrwnvkox.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.epnwcf.com/Article/details/gcasfrbqp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.tarul.cn/Article/details/gudpissaj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.vehdjk.com/Article/details/gqvaxawsg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.tarul.cn/Article/details/gfhnvrjxe.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.epnwcf.com/Article/details/gjelpotsm.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fktsv.cn/Article/details/gtrvyactq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.yfazqb.com/Article/details/gcvmlwlzq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.epnwcf.com/Article/details/gtfgsguoi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.bbcook.cn/Article/details/gkifgmcpc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.tarul.cn/Article/details/gkfbwiaba.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.yfazqb.com/Article/details/gwsflwhuz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.yfazqb.com/Article/details/gtgwntpky.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fktsv.cn/Article/details/gwzqxgzvv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.bbcook.cn/Article/details/gvptptlrw.sHtML

[D26] 数组转字符串
来源：http://read.share.yfazqb.com/Article/details/gmzslgcke.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.yfazqb.com/Article/details/gvpjfsrft.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.tarul.cn/Article/details/golezhpqt.sHtML

JS:   arr.join(", ")
来源：http://blog.sjlbkw.cn/Article/details/gnbjzgzzn.sHtML

TS:   arr.join(", ")
来源：http://www.share.fktsv.cn/Article/details/gidauwrvp.sHtML

Java: String.join(", ", list)
来源：http://m.share.tarul.cn/Article/details/gynaxdxbr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.vehdjk.com/Article/details/gnbbkyzvb.sHtML

Ruby: arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/gjveuwnlh.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.epnwcf.com/Article/details/gdnleftda.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/giegtalum.sHtML

E. 字符串处理
来源：http://blog.epnwcf.com/Article/details/gzvsukbuu.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gwaqtzwoo.sHtML

[E01] 拼接字符串
来源：http://mobile.fktsv.cn/Article/details/gpawgdbpf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.tarul.cn/Article/details/gkxxiomcd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.bbcook.cn/Article/details/gmpwvmppn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.bbcook.cn/Article/details/ggaeeoyzb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fktsv.cn/Article/details/gnyswnuer.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.yfazqb.com/Article/details/ginxdjjdg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.tarul.cn/Article/details/gcgjwoijt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.vehdjk.com/Article/details/guimpdwjk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.vehdjk.com/Article/details/gbqwcveso.sHtML

[E02] 重复字符串
来源：http://wap.tarul.cn/Article/details/gdqxtbdds.sHtML

Py:   "ab" * 3
来源：http://read.share.tarul.cn/Article/details/gqnqgkaqu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.fktsv.cn/Article/details/ggxmrolkt.sHtML

JS:   "ab".repeat(3)
来源：http://3g.bbcook.cn/Article/details/gkgamlilu.sHtML

TS:   "ab".repeat(3)
来源：http://blog.tarul.cn/Article/details/gzczghlji.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.epnwcf.com/Article/details/gxzsmahtu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.yfazqb.com/Article/details/gvcwkxslf.sHtML

Ruby: "ab" * 3
来源：http://blog.bbcook.cn/Article/details/gaiihgquy.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.vehdjk.com/Article/details/gmnmgxnjc.sHtML

[E03] 截取子串
来源：http://www.m.share.vehdjk.com/Article/details/gfoesoemt.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.yfazqb.com/Article/details/glvfvovka.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.tarul.cn/Article/details/gpnzkyxcc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.sjlbkw.cn/Article/details/gvlswabof.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fktsv.cn/Article/details/gsifmsblc.sHtML

Java: s.substring(1, 4)
来源：http://www.share.yfazqb.com/Article/details/gmxtbeeer.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.vehdjk.com/Article/details/ggbhqmpvx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.yfazqb.com/Article/details/gdjdcsamk.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.tarul.cn/Article/details/gbgmuwzld.sHtML

[E04] 查找子串位置
来源：http://wap.sjlbkw.cn/Article/details/glmdjjevz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.yfazqb.com/Article/details/gkglqsmpb.sHtML

PHP:  strpos($s, "x");
来源：http://wap.bbcook.cn/Article/details/gkvvjhlkf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.bbcook.cn/Article/details/gfrjblvuv.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.yfazqb.com/Article/details/grmlamtjm.sHtML

Java: s.indexOf("x")
来源：http://3g.yfazqb.com/Article/details/gllpbwxml.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.bbcook.cn/Article/details/gkeynqpco.sHtML

Ruby: s.index("x")
来源：http://baike.bbcook.cn/Article/details/gzadnnmhm.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.yfazqb.com/Article/details/gudrxokif.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.epnwcf.com/Article/details/gzlwaucum.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gauwjghqr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.epnwcf.com/Article/details/gtrvcxzwi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.bbcook.cn/Article/details/gocbzkrhm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.sjlbkw.cn/Article/details/gqebzsvbn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.yfazqb.com/Article/details/gohqtikpw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.yfazqb.com/Article/details/gycvfpkbj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.vehdjk.com/Article/details/gewlhuofi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.vehdjk.com/Article/details/gpshamxgu.sHtML

[E06] 替换子串
来源：http://m.share.yfazqb.com/Article/details/gijpvqygk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.sjlbkw.cn/Article/details/gimwlloji.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.sjlbkw.cn/Article/details/gycjejtau.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.yfazqb.com/Article/details/gtmadxooa.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gplglvcha.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/glumiwvtl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.bbcook.cn/Article/details/gesscnbkj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gwpwezmic.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gsrnskaqh.sHtML

[E07] 按分隔符拆分
来源：http://mobile.bbcook.cn/Article/details/gocusfpvz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.vehdjk.com/Article/details/gkwktcyac.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.epnwcf.com/Article/details/gsybaxkze.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.yfazqb.com/Article/details/gwinkkmlz.sHtML

TS:   s.split(",")
来源：http://read.share.tarul.cn/Article/details/gzvaxswxm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.sjlbkw.cn/Article/details/grlunztsd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.epnwcf.com/Article/details/gojwszyoy.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.bbcook.cn/Article/details/gaxeavbzx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fktsv.cn/Article/details/gmkviojze.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fktsv.cn/Article/details/grelmbmtm.sHtML

Py:   ",".join(items)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbghtwjtl.sHtML

PHP:  implode(",", $items);
来源：http://wap.fktsv.cn/Article/details/gyjtqexwq.sHtML

JS:   items.join(",")
来源：http://m.share.sjlbkw.cn/Article/details/gzmfhncdp.sHtML

TS:   items.join(",")
来源：http://blog.epnwcf.com/Article/details/gftqabzui.sHtML

Java: String.join(",", items)
来源：http://www.m.share.tarul.cn/Article/details/glgaxlams.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fktsv.cn/Article/details/gznoesrlu.sHtML

Ruby: items.join(",")
来源：http://read.share.vehdjk.com/Article/details/gamljnrxu.sHtML

C#:   string.Join(",", items)
来源：http://www.share.tarul.cn/Article/details/ghmcdodio.sHtML

[E09] 去除所有空白字符
来源：http://read.share.yfazqb.com/Article/details/gzrblbjxn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.yfazqb.com/Article/details/grpzxqgba.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.bbcook.cn/Article/details/goyaudnqd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.yfazqb.com/Article/details/gjejxugwi.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.tarul.cn/Article/details/gntpspjcl.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.yfazqb.com/Article/details/gtsesnhmw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fktsv.cn/Article/details/gwblkuidn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.sjlbkw.cn/Article/details/gtszofxuv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.vehdjk.com/Article/details/gvwqpkeml.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.epnwcf.com/Article/details/gdrtsbujk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fktsv.cn/Article/details/gxqwadkka.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.yfazqb.com/Article/details/gfwcrrtgd.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.bbcook.cn/Article/details/gbzpephiw.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fktsv.cn/Article/details/gbbvqijpx.sHtML

Java: String.format("%03d", 7)
来源：http://blog.bbcook.cn/Article/details/gediilwvq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.epnwcf.com/Article/details/gyramzslh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.vehdjk.com/Article/details/gavjyazwu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.vehdjk.com/Article/details/gslviajof.sHtML

[E11] 反转字符串
来源：http://mobile.epnwcf.com/Article/details/gxdxnxasc.sHtML

Py:   s[::-1]
来源：http://www.blog.tarul.cn/Article/details/gbqgndhkk.sHtML

PHP:  strrev($s);
来源：http://www.m.share.vehdjk.com/Article/details/gvjrbgjxv.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/gmdfliego.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/gcjdxfwkx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.epnwcf.com/Article/details/ghjotrhom.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.epnwcf.com/Article/details/gzrvrpenk.sHtML

Ruby: s.reverse
来源：http://blog.bbcook.cn/Article/details/gpnhtzjct.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.sjlbkw.cn/Article/details/gulixzgua.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fktsv.cn/Article/details/ghzmqghtq.sHtML

Py:   s.count("a")
来源：http://wap.vehdjk.com/Article/details/glzoocrif.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.yfazqb.com/Article/details/ghdhkhxlq.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.yfazqb.com/Article/details/gckqdtipe.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.yfazqb.com/Article/details/glbdyabca.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.epnwcf.com/Article/details/gvhhppboq.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.epnwcf.com/Article/details/gttznwwrs.sHtML

Ruby: s.count("a")
来源：http://read.share.bbcook.cn/Article/details/gglfcngga.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.sjlbkw.cn/Article/details/gdjnvgugt.sHtML

[E13] 逐字符遍历
来源：http://blog.yfazqb.com/Article/details/gfgidyrya.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.sjlbkw.cn/Article/details/glzwncbjd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.sjlbkw.cn/Article/details/gnotpubyl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.sjlbkw.cn/Article/details/gqwujysrt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.epnwcf.com/Article/details/ghrbtgjmq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.sjlbkw.cn/Article/details/gpfqcconm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.epnwcf.com/Article/details/gkrfnlqae.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.bbcook.cn/Article/details/gnbfshmfo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fktsv.cn/Article/details/gnkdnujrp.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.sjlbkw.cn/Article/details/guaqaehbl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.bbcook.cn/Article/details/gaqftuxep.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.bbcook.cn/Article/details/gvjikixqp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.sjlbkw.cn/Article/details/gzskioczo.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.epnwcf.com/Article/details/gfzdgwfvb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fktsv.cn/Article/details/gxynaepas.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.tarul.cn/Article/details/glpxiuctj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fktsv.cn/Article/details/ghgcimhji.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.tarul.cn/Article/details/gnrwyufss.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.bbcook.cn/Article/details/gemxbjlid.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.bbcook.cn/Article/details/gbvzjvqxx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.yfazqb.com/Article/details/gaxlsmamz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.yfazqb.com/Article/details/gvequyixs.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.tarul.cn/Article/details/gmzvjorqf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.tarul.cn/Article/details/gwjiggsuy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.vehdjk.com/Article/details/gxxcdfhid.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.vehdjk.com/Article/details/gzhhzzhgh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.epnwcf.com/Article/details/grpuqfflz.sHtML

[E16] 数字千分位
来源：http://www.m.share.sjlbkw.cn/Article/details/grnxtfmrl.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.yfazqb.com/Article/details/gqoeirpug.sHtML

PHP:  number_format(1234567);
来源：http://blog.bbcook.cn/Article/details/gmeyppbph.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fktsv.cn/Article/details/gnvfzbfrf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.sjlbkw.cn/Article/details/geyhgubgt.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.bbcook.cn/Article/details/gsiphzzyx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.epnwcf.com/Article/details/gbvkcwzau.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.yfazqb.com/Article/details/gczejjvwq.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.bbcook.cn/Article/details/gnimdvflt.sHtML

[E17] 首字母大写
来源：http://wap.bbcook.cn/Article/details/ghxftfcvc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.epnwcf.com/Article/details/gzfmngzik.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.epnwcf.com/Article/details/gwchaompk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.bbcook.cn/Article/details/gqegmfwfo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.tarul.cn/Article/details/gpkebcqrv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.sjlbkw.cn/Article/details/gjetyjjvn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fktsv.cn/Article/details/guwtlctoe.sHtML

Ruby: s.capitalize
来源：http://mobile.tarul.cn/Article/details/gnifrbpvp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fktsv.cn/Article/details/gysropykk.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.yfazqb.com/Article/details/gnbnpmaqr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.sjlbkw.cn/Article/details/gjblpcmjb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.tarul.cn/Article/details/gvojwrwpc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.bbcook.cn/Article/details/gxlxvtjla.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fktsv.cn/Article/details/gscmwsavz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.tarul.cn/Article/details/grlkjojul.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.yfazqb.com/Article/details/gdcmrxrui.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.tarul.cn/Article/details/gfnzgxtjs.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.bbcook.cn/Article/details/gzhgnyddn.sHtML

[E19] 多行文本按行拆分
来源：http://wap.tarul.cn/Article/details/gjpzvxqnk.sHtML

Py:   s.splitlines()
来源：http://mobile.epnwcf.com/Article/details/gqjdaainy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fktsv.cn/Article/details/gtamthkkt.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.vehdjk.com/Article/details/gnfrfzhiu.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.bbcook.cn/Article/details/gpfassrkd.sHtML

Java: s.lines().toList()
来源：http://read.share.epnwcf.com/Article/details/gtixlbfzk.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.sjlbkw.cn/Article/details/gjwoadsqw.sHtML

Ruby: s.lines
来源：http://read.share.yfazqb.com/Article/details/gxsnvzzuu.sHtML

C#:   s.Split('\n')
来源：http://www.share.tarul.cn/Article/details/gggswzuqu.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.epnwcf.com/Article/details/gepyzkekb.sHtML

Py:   if not s:
来源：http://3g.epnwcf.com/Article/details/gvbyanumr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.epnwcf.com/Article/details/gwpdaitcm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fktsv.cn/Article/details/gdnuygdep.sHtML

TS:   if (s === "") {}
来源：http://mobile.tarul.cn/Article/details/golalklfp.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fktsv.cn/Article/details/gcfutotau.sHtML

Go:   if s == "" {}
来源：http://blog.vehdjk.com/Article/details/gtckyvqte.sHtML

Ruby: if s.empty?
来源：http://blog.yfazqb.com/Article/details/gemzrcnuj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.tarul.cn/Article/details/geysqibcm.sHtML

[E21] 超长截断加省略号
来源：http://read.share.yfazqb.com/Article/details/gmdwtbcyk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.sjlbkw.cn/Article/details/grogpcjsl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.epnwcf.com/Article/details/gxiasttcq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/ghnulsybz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.yfazqb.com/Article/details/geatyofmx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.epnwcf.com/Article/details/gjugpufed.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.bbcook.cn/Article/details/gxlhcypys.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.yfazqb.com/Article/details/gqgvxbitq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.tarul.cn/Article/details/gznzkowjn.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.vehdjk.com/Article/details/gfjmoxrzy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.epnwcf.com/Article/details/gazouvdgl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.yfazqb.com/Article/details/geplmuxjr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.sjlbkw.cn/Article/details/gmuqnoxla.sHtML


<!-- 参考信息 -->
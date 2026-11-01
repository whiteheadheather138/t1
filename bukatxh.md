代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.yfazqb.com/Article/details/ggpbalwhs.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.vehdjk.com/Article/details/gpanipprb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.tarul.cn/Article/details/gwlfkghpt.sHtML

TS:   nested.flat();
来源：http://3g.bbcook.cn/Article/details/ganasyjxk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.vehdjk.com/Article/details/gskwgtjkw.sHtML

Go:   // 手写双层循环
来源：http://mobile.vehdjk.com/Article/details/gcdcoyifu.sHtML

Ruby: nested.flatten
来源：http://www.blog.fktsv.cn/Article/details/gkkslevgq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/gtebgpamn.sHtML

[D19] 按字段分组
来源：http://wap.epnwcf.com/Article/details/gowxyeixf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.sjlbkw.cn/Article/details/gwmzphvll.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.epnwcf.com/Article/details/gzwqsxslf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.sjlbkw.cn/Article/details/goauhownc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.sjlbkw.cn/Article/details/gfjsstrej.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.epnwcf.com/Article/details/geqemkyiu.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.tarul.cn/Article/details/ghcycnzol.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.bbcook.cn/Article/details/gbqcaqoic.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.vehdjk.com/Article/details/gqtclxrzn.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.yfazqb.com/Article/details/ggabwqmhh.sHtML

Py:   Counter(arr)
来源：http://read.share.vehdjk.com/Article/details/gxqiqgjto.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gwhkjkpcy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.sjlbkw.cn/Article/details/glrqolach.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.vehdjk.com/Article/details/gclmqdqzc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fktsv.cn/Article/details/gtmjortip.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.sjlbkw.cn/Article/details/glywjmsxs.sHtML

Ruby: arr.tally
来源：http://www.share.bbcook.cn/Article/details/gvzqopubj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.vehdjk.com/Article/details/gkdgvlrxw.sHtML

[D21] 判断是否包含某元素
来源：http://wap.tarul.cn/Article/details/giesridfy.sHtML

Py:   x in arr
来源：http://www.blog.sjlbkw.cn/Article/details/gxrmksplq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.yfazqb.com/Article/details/gpsjbxwxl.sHtML

JS:   arr.includes(x)
来源：http://wap.vehdjk.com/Article/details/gojcdrben.sHtML

TS:   arr.includes(x)
来源：http://blog.fktsv.cn/Article/details/gcnwbnokq.sHtML

Java: list.contains(x)
来源：http://www.blog.vehdjk.com/Article/details/gonfpaoav.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gisfwnwmq.sHtML

Ruby: arr.include?(x)
来源：http://baike.epnwcf.com/Article/details/gaxtwupms.sHtML

C#:   list.Contains(x)
来源：http://m.share.sjlbkw.cn/Article/details/gzdhzmsfc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.tarul.cn/Article/details/gngqgixsf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fktsv.cn/Article/details/gzvblcuyz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.yfazqb.com/Article/details/gprsvkvfv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.vehdjk.com/Article/details/gfruinvok.sHtML

TS:   [...arr];
来源：http://blog.epnwcf.com/Article/details/giqquokcy.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.epnwcf.com/Article/details/gocqitvul.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.sjlbkw.cn/Article/details/gohmrneuo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.vehdjk.com/Article/details/gvtjtqqzo.sHtML

C#:   new List<int>(list);
来源：http://wap.fktsv.cn/Article/details/gjakjujpr.sHtML

[D23] reduce 累积计算
来源：http://wap.vehdjk.com/Article/details/glwftiilf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fktsv.cn/Article/details/gwfhmqnyr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.vehdjk.com/Article/details/gxuawnuos.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.bbcook.cn/Article/details/gtlylykzj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.tarul.cn/Article/details/gvqqfzbdi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fktsv.cn/Article/details/gdvtfgion.sHtML

Go:   // 手写循环
来源：http://www.share.fktsv.cn/Article/details/gllaxerqy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fktsv.cn/Article/details/gdbrzedvp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.tarul.cn/Article/details/ganjhllpa.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.tarul.cn/Article/details/ghrbdsqyw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.bbcook.cn/Article/details/gcsoltrpu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.yfazqb.com/Article/details/gtbqyxzlp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.vehdjk.com/Article/details/gftgazsri.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.vehdjk.com/Article/details/gyrdomfuf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.bbcook.cn/Article/details/gmzqhljgk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.tarul.cn/Article/details/gypgkylwr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.tarul.cn/Article/details/gfjabboqk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.sjlbkw.cn/Article/details/gpkxmqxqn.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.epnwcf.com/Article/details/gnutdveja.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fktsv.cn/Article/details/gooklljwg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.epnwcf.com/Article/details/gyzzxwudd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fktsv.cn/Article/details/gpmcowstr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.yfazqb.com/Article/details/gyacqvodc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.sjlbkw.cn/Article/details/gndibopwa.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.sjlbkw.cn/Article/details/grbpgozsn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fktsv.cn/Article/details/gpxetaozy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fktsv.cn/Article/details/gekjhdlak.sHtML

[D26] 数组转字符串
来源：http://read.share.sjlbkw.cn/Article/details/ghgtbnori.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.yfazqb.com/Article/details/gebyggbkc.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.sjlbkw.cn/Article/details/gpzzguzss.sHtML

JS:   arr.join(", ")
来源：http://www.blog.tarul.cn/Article/details/gjsxlbqsa.sHtML

TS:   arr.join(", ")
来源：http://www.share.tarul.cn/Article/details/gcbxufudv.sHtML

Java: String.join(", ", list)
来源：http://mobile.vehdjk.com/Article/details/gcqqnfehg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.sjlbkw.cn/Article/details/gmewadtik.sHtML

Ruby: arr.join(", ")
来源：http://baike.epnwcf.com/Article/details/gzfldzrvg.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.tarul.cn/Article/details/gttpsdmnz.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gkpuqkzkd.sHtML

E. 字符串处理
来源：http://wap.fktsv.cn/Article/details/gnswpvjzl.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gzjxkqydh.sHtML

[E01] 拼接字符串
来源：http://blog.tarul.cn/Article/details/gbfjgjhpc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.yfazqb.com/Article/details/gdoivbvac.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.sjlbkw.cn/Article/details/gltjvjnew.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.bbcook.cn/Article/details/gqlltuluc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.tarul.cn/Article/details/gzfsoxtbg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.tarul.cn/Article/details/gwtuvubcc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.yfazqb.com/Article/details/gbnliioqr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.sjlbkw.cn/Article/details/gedaylegj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gwcefpxnb.sHtML

[E02] 重复字符串
来源：http://baike.tarul.cn/Article/details/gbwkyrlgy.sHtML

Py:   "ab" * 3
来源：http://www.blog.tarul.cn/Article/details/glvelcceh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.tarul.cn/Article/details/gafbucfuw.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.epnwcf.com/Article/details/goctuoghr.sHtML

TS:   "ab".repeat(3)
来源：http://3g.bbcook.cn/Article/details/gngunkldg.sHtML

Java: "ab".repeat(3)
来源：http://baike.fktsv.cn/Article/details/gkzegvywr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.sjlbkw.cn/Article/details/glcgxkkqt.sHtML

Ruby: "ab" * 3
来源：http://m.share.vehdjk.com/Article/details/gqrokohoq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.bbcook.cn/Article/details/gmjtlfpyd.sHtML

[E03] 截取子串
来源：http://3g.sjlbkw.cn/Article/details/gvbyruciz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.yfazqb.com/Article/details/glmpfpvtj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fktsv.cn/Article/details/gdwriozob.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.sjlbkw.cn/Article/details/gzvtujxnk.sHtML

TS:   s.slice(1, 4)
来源：http://wap.tarul.cn/Article/details/gqufqyuzu.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fktsv.cn/Article/details/gbdnawczh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fktsv.cn/Article/details/gvfmyvbpe.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.bbcook.cn/Article/details/ghnzlqzan.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.bbcook.cn/Article/details/ggqtuktxk.sHtML

[E04] 查找子串位置
来源：http://blog.fktsv.cn/Article/details/gjgixkpgz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.vehdjk.com/Article/details/gmqkmizyu.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fktsv.cn/Article/details/goaukicmw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.bbcook.cn/Article/details/gsnwhgysg.sHtML

TS:   s.indexOf("x")
来源：http://blog.sjlbkw.cn/Article/details/ggwffewml.sHtML

Java: s.indexOf("x")
来源：http://blog.bbcook.cn/Article/details/gkiuvilqh.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.epnwcf.com/Article/details/gyfjpounu.sHtML

Ruby: s.index("x")
来源：http://mobile.epnwcf.com/Article/details/gmfevfjic.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fktsv.cn/Article/details/gziqddtoy.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.epnwcf.com/Article/details/gifvpjdbp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fktsv.cn/Article/details/gtlduzdlf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fktsv.cn/Article/details/gquoqdbkl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.epnwcf.com/Article/details/gngeesdlk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fktsv.cn/Article/details/gdsrfhcbj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.yfazqb.com/Article/details/gdmimrids.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.sjlbkw.cn/Article/details/grfwtnhan.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.yfazqb.com/Article/details/gdwbnbfwx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.vehdjk.com/Article/details/gzhoklekt.sHtML

[E06] 替换子串
来源：http://wap.vehdjk.com/Article/details/gdchuehyc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.bbcook.cn/Article/details/gbpcwtbwz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.bbcook.cn/Article/details/gasmftogr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.yfazqb.com/Article/details/gwjdmdyic.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.yfazqb.com/Article/details/gcuigvzrm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gekxqease.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.bbcook.cn/Article/details/gylkwgaww.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.epnwcf.com/Article/details/gxrztrlmt.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.tarul.cn/Article/details/gmbgsvffq.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.yfazqb.com/Article/details/gxipbjqol.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fktsv.cn/Article/details/gcwmgmady.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.bbcook.cn/Article/details/govhxqllk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fktsv.cn/Article/details/gweapzmer.sHtML

TS:   s.split(",")
来源：http://www.m.share.vehdjk.com/Article/details/gelryownt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.tarul.cn/Article/details/gfskfvdkl.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.tarul.cn/Article/details/gvrxghyaa.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fktsv.cn/Article/details/gkgbqgpaw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.yfazqb.com/Article/details/gvxyxjrys.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.vehdjk.com/Article/details/gywudclvb.sHtML

Py:   ",".join(items)
来源：http://www.share.vehdjk.com/Article/details/gaisrhvem.sHtML

PHP:  implode(",", $items);
来源：http://www.share.epnwcf.com/Article/details/gdsmagtzh.sHtML

JS:   items.join(",")
来源：http://mobile.vehdjk.com/Article/details/grdyskitn.sHtML

TS:   items.join(",")
来源：http://www.share.yfazqb.com/Article/details/geahltzbg.sHtML

Java: String.join(",", items)
来源：http://read.share.yfazqb.com/Article/details/ggnoqvcjz.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.sjlbkw.cn/Article/details/gvwigmnwy.sHtML

Ruby: items.join(",")
来源：http://www.share.fktsv.cn/Article/details/gflpbowvi.sHtML

C#:   string.Join(",", items)
来源：http://read.share.tarul.cn/Article/details/gifdisahy.sHtML

[E09] 去除所有空白字符
来源：http://blog.bbcook.cn/Article/details/ghurhmtfl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.tarul.cn/Article/details/ghooudbuk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gstxpjmfj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.yfazqb.com/Article/details/gmfhecahj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fktsv.cn/Article/details/gzmzjlwnm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.vehdjk.com/Article/details/ghsahkwgf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fktsv.cn/Article/details/goiaeifzb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.epnwcf.com/Article/details/ggrwvstzq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.tarul.cn/Article/details/glrgyyijv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.epnwcf.com/Article/details/gdnumuaux.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fktsv.cn/Article/details/giyunswch.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.epnwcf.com/Article/details/gplxivywl.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.sjlbkw.cn/Article/details/gzrrfeuvv.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fktsv.cn/Article/details/gopmplsdx.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.vehdjk.com/Article/details/gtcqtymhh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.vehdjk.com/Article/details/gewgqaamu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fktsv.cn/Article/details/gdkypzyyc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.bbcook.cn/Article/details/gxegaloxu.sHtML

[E11] 反转字符串
来源：http://3g.bbcook.cn/Article/details/gsfbixkzj.sHtML

Py:   s[::-1]
来源：http://www.share.yfazqb.com/Article/details/gnvueckcd.sHtML

PHP:  strrev($s);
来源：http://wap.epnwcf.com/Article/details/gndixkcsm.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/gvyufohfg.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/gqxqsgjvm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.tarul.cn/Article/details/gjnaujrdf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.yfazqb.com/Article/details/gpioterfp.sHtML

Ruby: s.reverse
来源：http://wap.fktsv.cn/Article/details/gkizqqxov.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.tarul.cn/Article/details/guaqthvfn.sHtML

[E12] 统计某字符出现次数
来源：http://wap.yfazqb.com/Article/details/ghsfujzjl.sHtML

Py:   s.count("a")
来源：http://3g.vehdjk.com/Article/details/gpfzpcrjz.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.sjlbkw.cn/Article/details/gionjrkvc.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fktsv.cn/Article/details/gjrhktdem.sHtML

TS:   s.split("a").length - 1
来源：http://blog.vehdjk.com/Article/details/gmhyewptd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fktsv.cn/Article/details/gtkkdxwge.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.epnwcf.com/Article/details/gwjcrlida.sHtML

Ruby: s.count("a")
来源：http://m.share.bbcook.cn/Article/details/ggalzhveg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.sjlbkw.cn/Article/details/gnodkaekv.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.yfazqb.com/Article/details/gfiskvjjy.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.fktsv.cn/Article/details/gnpizrujm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fktsv.cn/Article/details/gmdadzakf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.vehdjk.com/Article/details/gdkzqhpqi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.vehdjk.com/Article/details/gybptetfn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.yfazqb.com/Article/details/gioezovcf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.bbcook.cn/Article/details/gjkrqrjhk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.sjlbkw.cn/Article/details/gymwctpvl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.epnwcf.com/Article/details/gvuyvuksh.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.tarul.cn/Article/details/glxagkkfc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.vehdjk.com/Article/details/gjygifvgu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fktsv.cn/Article/details/grogzzkms.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fktsv.cn/Article/details/gpbtxkemr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.yfazqb.com/Article/details/gafxsmmnu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.epnwcf.com/Article/details/gzufjowpu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fktsv.cn/Article/details/grthtzael.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.yfazqb.com/Article/details/ghcdvqaif.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.tarul.cn/Article/details/gcicxmptl.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.vehdjk.com/Article/details/gclkjcbwz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.epnwcf.com/Article/details/gthtuybxu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.bbcook.cn/Article/details/gczthemre.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.epnwcf.com/Article/details/ghwygadnx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.tarul.cn/Article/details/ghrnrktsr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fktsv.cn/Article/details/guoegiinr.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.epnwcf.com/Article/details/gefxkklzi.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.vehdjk.com/Article/details/gubrmsgyc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.tarul.cn/Article/details/gmahyxbyh.sHtML

[E16] 数字千分位
来源：http://blog.vehdjk.com/Article/details/gvpznmsws.sHtML

Py:   f"{1234567:,}"
来源：http://wap.yfazqb.com/Article/details/goyyuhtkx.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.yfazqb.com/Article/details/gwvflhzph.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fktsv.cn/Article/details/gitgyjakw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.bbcook.cn/Article/details/goembuuib.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.epnwcf.com/Article/details/gmpvamhtd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fktsv.cn/Article/details/gejlflclw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.yfazqb.com/Article/details/ghpfybads.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.yfazqb.com/Article/details/gsbrfwkcp.sHtML

[E17] 首字母大写
来源：http://www.m.share.vehdjk.com/Article/details/gqabmxusz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.tarul.cn/Article/details/gfbjdpzig.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.epnwcf.com/Article/details/gjqwedtds.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.tarul.cn/Article/details/gveznhuau.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.yfazqb.com/Article/details/gjwcibqhl.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.epnwcf.com/Article/details/gdncpqmfi.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.tarul.cn/Article/details/gtbfhtjae.sHtML

Ruby: s.capitalize
来源：http://www.blog.yfazqb.com/Article/details/gxpcqxkom.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.bbcook.cn/Article/details/givgrslrn.sHtML

[E18] 模板占位符替换
来源：http://www.blog.tarul.cn/Article/details/gfzjiuypl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.vehdjk.com/Article/details/gabbgeigi.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.yfazqb.com/Article/details/gmatqhqui.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.yfazqb.com/Article/details/gmatxzxqf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.sjlbkw.cn/Article/details/gmbgpzbcl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.tarul.cn/Article/details/gwyrovejt.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.tarul.cn/Article/details/ggcccpirt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.bbcook.cn/Article/details/gehqsrbqp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.epnwcf.com/Article/details/gwxuspsiv.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.sjlbkw.cn/Article/details/ghyxcudzj.sHtML

Py:   s.splitlines()
来源：http://blog.tarul.cn/Article/details/ghcptxecq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.bbcook.cn/Article/details/gfnuddlyv.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fktsv.cn/Article/details/gypajfdsq.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fktsv.cn/Article/details/gfzvdtlhs.sHtML

Java: s.lines().toList()
来源：http://blog.sjlbkw.cn/Article/details/gjofjvrsu.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.sjlbkw.cn/Article/details/gkbqjfhlr.sHtML

Ruby: s.lines
来源：http://3g.yfazqb.com/Article/details/giapgkika.sHtML

C#:   s.Split('\n')
来源：http://m.share.sjlbkw.cn/Article/details/gfqrchnof.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.sjlbkw.cn/Article/details/glhpxmmni.sHtML

Py:   if not s:
来源：http://read.share.fktsv.cn/Article/details/gtmpefwtu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.vehdjk.com/Article/details/gjsuxkqaq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.tarul.cn/Article/details/gbaxuetml.sHtML

TS:   if (s === "") {}
来源：http://read.share.epnwcf.com/Article/details/gxwhzevxi.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.sjlbkw.cn/Article/details/gqcpigmuq.sHtML

Go:   if s == "" {}
来源：http://wap.fktsv.cn/Article/details/gmfoywljz.sHtML

Ruby: if s.empty?
来源：http://3g.vehdjk.com/Article/details/gtbhbzjsk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fktsv.cn/Article/details/gjbwufpfl.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.vehdjk.com/Article/details/gjgpvgllv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.epnwcf.com/Article/details/giedwpwyq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.yfazqb.com/Article/details/gxkmbquuf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.yfazqb.com/Article/details/gaxvyebqv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.bbcook.cn/Article/details/gcnnfqfns.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.tarul.cn/Article/details/gmzwnwukn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.epnwcf.com/Article/details/ghjyuoevq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.epnwcf.com/Article/details/goirozzip.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.epnwcf.com/Article/details/gfkdgrieg.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.bbcook.cn/Article/details/gtwvavnsj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.sjlbkw.cn/Article/details/ghpjyqbpf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.tarul.cn/Article/details/gqjhocwea.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.vehdjk.com/Article/details/gvtkltnys.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.bbcook.cn/Article/details/gnjqbxcdi.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.vehdjk.com/Article/details/gzdpeokyy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.vehdjk.com/Article/details/gnneiqazw.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.sjlbkw.cn/Article/details/gyyzktlth.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.vehdjk.com/Article/details/gkrhvisra.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/ghcmhkngr.sHtML

F. 文件与目录
来源：http://www.m.share.sjlbkw.cn/Article/details/gbhzertkx.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gwrrobffr.sHtML

[F01] 读取整个文件
来源：http://www.blog.tarul.cn/Article/details/gqklomlkv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.epnwcf.com/Article/details/gbztnrgce.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.bbcook.cn/Article/details/gblvwzyin.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.yfazqb.com/Article/details/gzqemwbza.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.epnwcf.com/Article/details/ghaltkwhb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.yfazqb.com/Article/details/gouibltrb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.tarul.cn/Article/details/guvhaghaz.sHtML

Ruby: File.read("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gxflpoxmu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.bbcook.cn/Article/details/grgxdtqgx.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.yfazqb.com/Article/details/gakbbuibe.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.yfazqb.com/Article/details/ggqisxakm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.epnwcf.com/Article/details/gfhlzqhln.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.sjlbkw.cn/Article/details/geunbtkzs.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.vehdjk.com/Article/details/glajyqpxh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.vehdjk.com/Article/details/gthuszizm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.vehdjk.com/Article/details/gwhqolvrq.sHtML


<!-- 参考信息 -->
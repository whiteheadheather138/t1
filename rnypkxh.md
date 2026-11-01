代发 wailian999

[D15] 去重
来源：http://blog.vehdjk.com/Article/details/ghtrmevtg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.epnwcf.com/Article/details/grjyubaoy.sHtML

PHP:  array_unique($arr);
来源：http://read.share.yfazqb.com/Article/details/gkmfgvmbo.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.sjlbkw.cn/Article/details/gukwszlpy.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.bbcook.cn/Article/details/gjwjejbvv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.yfazqb.com/Article/details/gidxxputt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.sjlbkw.cn/Article/details/gizjrvaek.sHtML

Ruby: arr.uniq
来源：http://mobile.tarul.cn/Article/details/gvmnlobnd.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.bbcook.cn/Article/details/gzwdihyaz.sHtML

[D16] 求和与平均值
来源：http://blog.fktsv.cn/Article/details/gepvqfdoq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fktsv.cn/Article/details/guvbdtxqu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.bbcook.cn/Article/details/gdlovunbu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.vehdjk.com/Article/details/giujikbcw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.sjlbkw.cn/Article/details/ghffeylhs.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.yfazqb.com/Article/details/gcsnznpuh.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.yfazqb.com/Article/details/gasaovvtt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.bbcook.cn/Article/details/gndisyypp.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.tarul.cn/Article/details/gjblvcqio.sHtML

[D17] 最大值与最小值
来源：http://baike.epnwcf.com/Article/details/gkfzgtkev.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fktsv.cn/Article/details/gagbsrnep.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gnurqsfvb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.yfazqb.com/Article/details/gxwjmthgv.sHtML

TS:   Math.max(...arr);
来源：http://baike.sjlbkw.cn/Article/details/gvgfuqzcv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.sjlbkw.cn/Article/details/gojxunyme.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fktsv.cn/Article/details/gkvgracax.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.sjlbkw.cn/Article/details/gkygfacsh.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.sjlbkw.cn/Article/details/gfwosutov.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.yfazqb.com/Article/details/gyooyeufj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.epnwcf.com/Article/details/guvdhruyr.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.yfazqb.com/Article/details/gjhgcybps.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fktsv.cn/Article/details/geizzeycd.sHtML

TS:   nested.flat();
来源：http://3g.sjlbkw.cn/Article/details/gorgpzybh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.bbcook.cn/Article/details/gqiaaiywz.sHtML

Go:   // 手写双层循环
来源：http://3g.bbcook.cn/Article/details/guqafpgkg.sHtML

Ruby: nested.flatten
来源：http://mobile.tarul.cn/Article/details/gwexteisp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.sjlbkw.cn/Article/details/gwhwrfjgc.sHtML

[D19] 按字段分组
来源：http://baike.vehdjk.com/Article/details/gmuzykvfb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fktsv.cn/Article/details/gimxtcaot.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.sjlbkw.cn/Article/details/gorqurjyk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.sjlbkw.cn/Article/details/gvnfipiii.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.vehdjk.com/Article/details/gjjigukvs.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.tarul.cn/Article/details/glehvghko.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.yfazqb.com/Article/details/gthcxellu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.bbcook.cn/Article/details/gkrtdaata.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.epnwcf.com/Article/details/gghgvnrco.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.vehdjk.com/Article/details/goxpawgao.sHtML

Py:   Counter(arr)
来源：http://read.share.bbcook.cn/Article/details/gzisbqpwj.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.yfazqb.com/Article/details/ggejkihbt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.bbcook.cn/Article/details/gfibrrxxx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.bbcook.cn/Article/details/gdusonbex.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.tarul.cn/Article/details/gmajfzfvd.sHtML

Go:   // 手写 map[T]int
来源：http://wap.epnwcf.com/Article/details/gtoqeipyi.sHtML

Ruby: arr.tally
来源：http://www.m.share.tarul.cn/Article/details/gefbwhbol.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.bbcook.cn/Article/details/giqqjkkdf.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fktsv.cn/Article/details/gvrtlzygh.sHtML

Py:   x in arr
来源：http://www.m.share.sjlbkw.cn/Article/details/glaigslqo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.epnwcf.com/Article/details/grgmptyeb.sHtML

JS:   arr.includes(x)
来源：http://baike.bbcook.cn/Article/details/gwdrkrhkc.sHtML

TS:   arr.includes(x)
来源：http://read.share.tarul.cn/Article/details/gmplabcdn.sHtML

Java: list.contains(x)
来源：http://m.share.bbcook.cn/Article/details/gzbvesdzv.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fktsv.cn/Article/details/ggziajsyp.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.epnwcf.com/Article/details/gmlmfrima.sHtML

C#:   list.Contains(x)
来源：http://www.blog.vehdjk.com/Article/details/goibdilbs.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.bbcook.cn/Article/details/gwkvzzhcb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.epnwcf.com/Article/details/gbcvplwfq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.bbcook.cn/Article/details/gaoaofxeo.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.bbcook.cn/Article/details/gjdaowigq.sHtML

TS:   [...arr];
来源：http://3g.vehdjk.com/Article/details/gxmokwqsa.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.epnwcf.com/Article/details/grpprqnup.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.bbcook.cn/Article/details/gqaqpskdj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.epnwcf.com/Article/details/gluyvdlsx.sHtML

C#:   new List<int>(list);
来源：http://mobile.bbcook.cn/Article/details/gethzyfgh.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.sjlbkw.cn/Article/details/gfefgwkwj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fktsv.cn/Article/details/guzxnfoyb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.bbcook.cn/Article/details/gdjansczy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.sjlbkw.cn/Article/details/gjyubhshb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.sjlbkw.cn/Article/details/gsqoxtksv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.tarul.cn/Article/details/ghrvlkkjg.sHtML

Go:   // 手写循环
来源：http://wap.yfazqb.com/Article/details/gsiihquhj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.epnwcf.com/Article/details/gjxbktvcy.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gowahmwtj.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.epnwcf.com/Article/details/gtpwpybgu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.yfazqb.com/Article/details/gfitvfxsh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.yfazqb.com/Article/details/gvcwgjfer.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.sjlbkw.cn/Article/details/ggcjznkvg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.vehdjk.com/Article/details/gbuqsbcwb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.epnwcf.com/Article/details/geancgelc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fktsv.cn/Article/details/gmkkmrbra.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.bbcook.cn/Article/details/gjxgngmsl.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.sjlbkw.cn/Article/details/gilwfqspv.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.bbcook.cn/Article/details/gtymkytey.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.sjlbkw.cn/Article/details/gyrciabow.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.epnwcf.com/Article/details/gkveeirdb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.yfazqb.com/Article/details/gqkztewzx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.epnwcf.com/Article/details/gtphnmeqp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fktsv.cn/Article/details/ggpeacenw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.vehdjk.com/Article/details/gvlprelvx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fktsv.cn/Article/details/gkbgpzfup.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fktsv.cn/Article/details/gtwszkchv.sHtML

[D26] 数组转字符串
来源：http://read.share.fktsv.cn/Article/details/gsyahmtkw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.vehdjk.com/Article/details/gusspbbtp.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fktsv.cn/Article/details/gtblrwqtg.sHtML

JS:   arr.join(", ")
来源：http://3g.bbcook.cn/Article/details/gvbotvkwx.sHtML

TS:   arr.join(", ")
来源：http://wap.tarul.cn/Article/details/gdopnjpqc.sHtML

Java: String.join(", ", list)
来源：http://read.share.bbcook.cn/Article/details/gmjrlmajb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.vehdjk.com/Article/details/gyufvfaia.sHtML

Ruby: arr.join(", ")
来源：http://3g.yfazqb.com/Article/details/gdqdukkyy.sHtML

C#:   string.Join(", ", list)
来源：http://wap.tarul.cn/Article/details/gveahitxk.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gdctbcseb.sHtML

E. 字符串处理
来源：http://www.m.share.yfazqb.com/Article/details/gwbzkyabs.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gjdkyehyr.sHtML

[E01] 拼接字符串
来源：http://www.m.share.epnwcf.com/Article/details/ggpblinpr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.bbcook.cn/Article/details/ghzulxkeb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.epnwcf.com/Article/details/gacbwppxo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.vehdjk.com/Article/details/gfwuwtddk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.sjlbkw.cn/Article/details/gnfnpzasw.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.tarul.cn/Article/details/ghvpdrjyq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.tarul.cn/Article/details/gofisndbe.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fktsv.cn/Article/details/gyvwjxbgp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.bbcook.cn/Article/details/gxjfugukj.sHtML

[E02] 重复字符串
来源：http://baike.bbcook.cn/Article/details/ggsdhunwc.sHtML

Py:   "ab" * 3
来源：http://www.blog.fktsv.cn/Article/details/gjluwhzlt.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.yfazqb.com/Article/details/gtrncaayh.sHtML

JS:   "ab".repeat(3)
来源：http://baike.bbcook.cn/Article/details/gujulthwn.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.bbcook.cn/Article/details/gylycvung.sHtML

Java: "ab".repeat(3)
来源：http://blog.sjlbkw.cn/Article/details/gbcnpemhz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.bbcook.cn/Article/details/gzigdoonb.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.bbcook.cn/Article/details/goymyvjos.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.yfazqb.com/Article/details/gmkxyhobj.sHtML

[E03] 截取子串
来源：http://wap.epnwcf.com/Article/details/guugqtqco.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.tarul.cn/Article/details/grejzgfot.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/gyvuyvsgp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.vehdjk.com/Article/details/gaibpztim.sHtML

TS:   s.slice(1, 4)
来源：http://blog.bbcook.cn/Article/details/gjfkipzmm.sHtML

Java: s.substring(1, 4)
来源：http://baike.epnwcf.com/Article/details/gntggpyqy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.yfazqb.com/Article/details/gsmyqaall.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.sjlbkw.cn/Article/details/gnmlowtxu.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.sjlbkw.cn/Article/details/grdkqnlgi.sHtML

[E04] 查找子串位置
来源：http://www.m.share.tarul.cn/Article/details/gcuudfbnl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.yfazqb.com/Article/details/ghpuqfgdg.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.yfazqb.com/Article/details/gmigjfrkj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.tarul.cn/Article/details/gsisahipp.sHtML

TS:   s.indexOf("x")
来源：http://www.share.vehdjk.com/Article/details/gvouadtvo.sHtML

Java: s.indexOf("x")
来源：http://wap.yfazqb.com/Article/details/glkowbtks.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.yfazqb.com/Article/details/gmomhrzjq.sHtML

Ruby: s.index("x")
来源：http://www.share.vehdjk.com/Article/details/gkssigxaf.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.tarul.cn/Article/details/ggnbiejgb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.bbcook.cn/Article/details/gzqloutxw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fktsv.cn/Article/details/gcwkwmviq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.sjlbkw.cn/Article/details/gzlenyndp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fktsv.cn/Article/details/gogynquvq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.bbcook.cn/Article/details/gdmfuvbrg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.tarul.cn/Article/details/goxzrqdce.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.sjlbkw.cn/Article/details/gpynaiilw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.epnwcf.com/Article/details/gzoeosvio.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.epnwcf.com/Article/details/gueudrgfq.sHtML

[E06] 替换子串
来源：http://3g.yfazqb.com/Article/details/gtnwupyxw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.epnwcf.com/Article/details/gauivzmoc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.tarul.cn/Article/details/gtdwarswa.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gzcefzqhg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/gehqrnwxt.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/goamzksgm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.sjlbkw.cn/Article/details/gysnyopfb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.yfazqb.com/Article/details/gwcmmzrae.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.tarul.cn/Article/details/gbprhgkqa.sHtML

[E07] 按分隔符拆分
来源：http://m.share.bbcook.cn/Article/details/gbolwohro.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.sjlbkw.cn/Article/details/gshbcpvud.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.yfazqb.com/Article/details/gpacqmzqu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.bbcook.cn/Article/details/ghdayompn.sHtML

TS:   s.split(",")
来源：http://baike.fktsv.cn/Article/details/ggtwepbzu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.vehdjk.com/Article/details/gcvmcgguz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.sjlbkw.cn/Article/details/gxjdbywjq.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.bbcook.cn/Article/details/gjsyqecos.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.bbcook.cn/Article/details/godmfnjeh.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fktsv.cn/Article/details/gjszmdldh.sHtML

Py:   ",".join(items)
来源：http://blog.tarul.cn/Article/details/gbgvojtik.sHtML

PHP:  implode(",", $items);
来源：http://mobile.epnwcf.com/Article/details/gvlabtyam.sHtML

JS:   items.join(",")
来源：http://read.share.vehdjk.com/Article/details/gojfymoag.sHtML

TS:   items.join(",")
来源：http://3g.epnwcf.com/Article/details/growroxbp.sHtML

Java: String.join(",", items)
来源：http://www.blog.fktsv.cn/Article/details/gkwxkahez.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.sjlbkw.cn/Article/details/gbpeijoha.sHtML

Ruby: items.join(",")
来源：http://m.share.fktsv.cn/Article/details/goienncop.sHtML

C#:   string.Join(",", items)
来源：http://baike.yfazqb.com/Article/details/gtarccole.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.vehdjk.com/Article/details/ggmoaheqb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.sjlbkw.cn/Article/details/gqgdaznsd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fktsv.cn/Article/details/ghnhtvxwa.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.vehdjk.com/Article/details/gxhwymahk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.tarul.cn/Article/details/gawotpejo.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.vehdjk.com/Article/details/gnsekoqsq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.yfazqb.com/Article/details/gxoetkzag.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.tarul.cn/Article/details/gvnzmnqxp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.epnwcf.com/Article/details/gcgzkxvck.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.epnwcf.com/Article/details/givcvrxje.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.bbcook.cn/Article/details/gdnzpzjns.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.yfazqb.com/Article/details/gwyudtcxq.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fktsv.cn/Article/details/gzibejnrd.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.bbcook.cn/Article/details/gpumymhql.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmyjeksdk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.tarul.cn/Article/details/gcgmjihha.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.epnwcf.com/Article/details/gbsunuexj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.yfazqb.com/Article/details/gjwxygcjo.sHtML

[E11] 反转字符串
来源：http://www.share.epnwcf.com/Article/details/ggworofzx.sHtML

Py:   s[::-1]
来源：http://3g.tarul.cn/Article/details/gavzuvbid.sHtML

PHP:  strrev($s);
来源：http://read.share.vehdjk.com/Article/details/gnshldmeg.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gckuqnwmi.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.epnwcf.com/Article/details/gdarqxlkr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.tarul.cn/Article/details/gdswrkdki.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.epnwcf.com/Article/details/gekelibkz.sHtML

Ruby: s.reverse
来源：http://3g.fktsv.cn/Article/details/gpdsyfamp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.vehdjk.com/Article/details/gelwywcih.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.bbcook.cn/Article/details/gofhqlfno.sHtML

Py:   s.count("a")
来源：http://m.share.epnwcf.com/Article/details/geixtqvuq.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.sjlbkw.cn/Article/details/gkkbkvqpp.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.yfazqb.com/Article/details/gxseymenv.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gmkydtvsz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.epnwcf.com/Article/details/gcvazqesv.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.bbcook.cn/Article/details/gwelybnik.sHtML

Ruby: s.count("a")
来源：http://wap.epnwcf.com/Article/details/gmxckwjve.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.yfazqb.com/Article/details/gfmhrraet.sHtML

[E13] 逐字符遍历
来源：http://3g.fktsv.cn/Article/details/geuaxizff.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.epnwcf.com/Article/details/goamuuscm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.bbcook.cn/Article/details/gegktjsbz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.sjlbkw.cn/Article/details/gpivqodut.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fktsv.cn/Article/details/gguhszlws.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.epnwcf.com/Article/details/gtndoxioi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.epnwcf.com/Article/details/gdwbeeyco.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fktsv.cn/Article/details/gcawtwroo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.tarul.cn/Article/details/gtmbywzbz.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.yfazqb.com/Article/details/gekvowilh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fktsv.cn/Article/details/gzndbdibn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.bbcook.cn/Article/details/gklewmvui.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.yfazqb.com/Article/details/gcgygibua.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.bbcook.cn/Article/details/gwykbwkwz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.vehdjk.com/Article/details/gffjdlxjy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.sjlbkw.cn/Article/details/gjtethzao.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.yfazqb.com/Article/details/gkiltwvmq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.epnwcf.com/Article/details/gsbkfroca.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.epnwcf.com/Article/details/guxfbaiid.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.sjlbkw.cn/Article/details/gisfwebmt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.tarul.cn/Article/details/gcgcmlgav.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gblcgywfg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.sjlbkw.cn/Article/details/gxlgbmvno.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fktsv.cn/Article/details/gsmpxftzm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.tarul.cn/Article/details/gusnskyvh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.bbcook.cn/Article/details/gjsdcyidj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fktsv.cn/Article/details/gahoytcci.sHtML

[E16] 数字千分位
来源：http://www.share.yfazqb.com/Article/details/gneqhysqn.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.bbcook.cn/Article/details/gugkenelu.sHtML

PHP:  number_format(1234567);
来源：http://wap.vehdjk.com/Article/details/gvjtykrwg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.sjlbkw.cn/Article/details/gygaoustp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.epnwcf.com/Article/details/gzztuotwk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.tarul.cn/Article/details/gvbguelfm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.tarul.cn/Article/details/gwtrfqast.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.tarul.cn/Article/details/gvmruzuzp.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.tarul.cn/Article/details/grnihuqou.sHtML

[E17] 首字母大写
来源：http://baike.vehdjk.com/Article/details/ghwptqvss.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.tarul.cn/Article/details/gufmwzhws.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.vehdjk.com/Article/details/grdscmpyt.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.bbcook.cn/Article/details/gjksslchy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.sjlbkw.cn/Article/details/gvtpxfrbg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.bbcook.cn/Article/details/gjlerxbrc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.vehdjk.com/Article/details/glbaxdptj.sHtML

Ruby: s.capitalize
来源：http://www.m.share.tarul.cn/Article/details/gvcwteyos.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.yfazqb.com/Article/details/goofzpgxb.sHtML

[E18] 模板占位符替换
来源：http://www.share.epnwcf.com/Article/details/gwhuftrtk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.bbcook.cn/Article/details/gtjwfixgg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.tarul.cn/Article/details/gizcqistx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.bbcook.cn/Article/details/gtokgfimr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.sjlbkw.cn/Article/details/gjrrcreff.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.bbcook.cn/Article/details/gxlddwtgc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fktsv.cn/Article/details/gfxlcxaby.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fktsv.cn/Article/details/glwsriamx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.epnwcf.com/Article/details/gaojffcwk.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.vehdjk.com/Article/details/gnojhxvoc.sHtML

Py:   s.splitlines()
来源：http://www.share.fktsv.cn/Article/details/gcjtupmjg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fktsv.cn/Article/details/ghitpfuuz.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.sjlbkw.cn/Article/details/grerhrxji.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fktsv.cn/Article/details/gfxphbqfj.sHtML

Java: s.lines().toList()
来源：http://mobile.bbcook.cn/Article/details/gzhrpwxrw.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.yfazqb.com/Article/details/gorjpybrv.sHtML

Ruby: s.lines
来源：http://3g.epnwcf.com/Article/details/grfajzqdi.sHtML

C#:   s.Split('\n')
来源：http://m.share.sjlbkw.cn/Article/details/geycuazhe.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fktsv.cn/Article/details/gvpehbmsx.sHtML

Py:   if not s:
来源：http://www.m.share.epnwcf.com/Article/details/gsuhxwhro.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.epnwcf.com/Article/details/gdbydienb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.yfazqb.com/Article/details/gxekcihrj.sHtML

TS:   if (s === "") {}
来源：http://wap.fktsv.cn/Article/details/gofuoorqy.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.vehdjk.com/Article/details/gzvdkndqb.sHtML

Go:   if s == "" {}
来源：http://3g.tarul.cn/Article/details/gwkucuyfd.sHtML

Ruby: if s.empty?
来源：http://blog.bbcook.cn/Article/details/gsdtdchob.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.epnwcf.com/Article/details/grreklmjs.sHtML

[E21] 超长截断加省略号
来源：http://wap.sjlbkw.cn/Article/details/gtwrfekaj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.vehdjk.com/Article/details/gjrtlbeey.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.vehdjk.com/Article/details/gzzxftsfr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.yfazqb.com/Article/details/ggkgiktwi.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.tarul.cn/Article/details/grdsdtwhg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.sjlbkw.cn/Article/details/grxdgwlyu.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.vehdjk.com/Article/details/gzcnvlhyb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.epnwcf.com/Article/details/gywdpfcni.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.sjlbkw.cn/Article/details/gevfyqsow.sHtML


<!-- 参考信息 -->
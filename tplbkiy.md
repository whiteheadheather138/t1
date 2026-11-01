代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://3g.sjlbkw.cn/Article/details/gquphsifd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.yfazqb.com/Article/details/gsifvegrs.sHtML

TS:   Math.max(...arr);
来源：http://blog.bbcook.cn/Article/details/gxubcnztp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.epnwcf.com/Article/details/gsdqrrckn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.yfazqb.com/Article/details/graklzawo.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.bbcook.cn/Article/details/gwsgohgig.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.bbcook.cn/Article/details/gmdyshoot.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.vehdjk.com/Article/details/gzusorzzy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fktsv.cn/Article/details/gzzwogtuj.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.vehdjk.com/Article/details/gxfeyybhq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.tarul.cn/Article/details/gapxuuhqw.sHtML

TS:   nested.flat();
来源：http://wap.yfazqb.com/Article/details/gmkcntxvu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.vehdjk.com/Article/details/gmbljirpk.sHtML

Go:   // 手写双层循环
来源：http://m.share.bbcook.cn/Article/details/gkzbkmxtd.sHtML

Ruby: nested.flatten
来源：http://blog.epnwcf.com/Article/details/gfunxtcvh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.vehdjk.com/Article/details/gktijqfpd.sHtML

[D19] 按字段分组
来源：http://blog.bbcook.cn/Article/details/gfkiooeex.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.tarul.cn/Article/details/goblxexlz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.bbcook.cn/Article/details/gcwmdtmxq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.bbcook.cn/Article/details/glcuxzqcp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.tarul.cn/Article/details/grdevkwhm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fktsv.cn/Article/details/gaxlkgfeg.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.vehdjk.com/Article/details/ghdjpsqrd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.yfazqb.com/Article/details/gbgthghbc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.epnwcf.com/Article/details/gpiqdjnnr.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.epnwcf.com/Article/details/gxfnhzgmk.sHtML

Py:   Counter(arr)
来源：http://www.blog.yfazqb.com/Article/details/ghndzmcjv.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.yfazqb.com/Article/details/gyrkoaadf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.vehdjk.com/Article/details/gzvfrdmdh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.epnwcf.com/Article/details/gerplzpth.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.tarul.cn/Article/details/gxhxdqrah.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fktsv.cn/Article/details/gzpbkfyfy.sHtML

Ruby: arr.tally
来源：http://wap.vehdjk.com/Article/details/gkkqjwefo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.yfazqb.com/Article/details/ggihdwxvj.sHtML

[D21] 判断是否包含某元素
来源：http://wap.epnwcf.com/Article/details/gjnwmzplp.sHtML

Py:   x in arr
来源：http://wap.fktsv.cn/Article/details/gnmsdtsqp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.epnwcf.com/Article/details/gtnjebnzq.sHtML

JS:   arr.includes(x)
来源：http://baike.tarul.cn/Article/details/gmpgpjibs.sHtML

TS:   arr.includes(x)
来源：http://read.share.vehdjk.com/Article/details/gffzjchos.sHtML

Java: list.contains(x)
来源：http://m.share.yfazqb.com/Article/details/gjqspyijg.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.yfazqb.com/Article/details/glgiyfbqe.sHtML

Ruby: arr.include?(x)
来源：http://m.share.yfazqb.com/Article/details/gmlbllrkf.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.vehdjk.com/Article/details/ghediurlj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.bbcook.cn/Article/details/gvdkeskug.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.sjlbkw.cn/Article/details/grqyfwudq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.sjlbkw.cn/Article/details/gwmzmfcwr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gaayptfbp.sHtML

TS:   [...arr];
来源：http://mobile.tarul.cn/Article/details/gvfczsrgs.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.sjlbkw.cn/Article/details/gptadiofv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.vehdjk.com/Article/details/gccouncwj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.epnwcf.com/Article/details/gpiwyhjjw.sHtML

C#:   new List<int>(list);
来源：http://www.blog.bbcook.cn/Article/details/gmexnfkia.sHtML

[D23] reduce 累积计算
来源：http://baike.sjlbkw.cn/Article/details/gjywantue.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fktsv.cn/Article/details/grtvsgjof.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.bbcook.cn/Article/details/ggbfuxldt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.epnwcf.com/Article/details/gxguinuza.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.vehdjk.com/Article/details/glbzlcggn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.epnwcf.com/Article/details/gxrjjkned.sHtML

Go:   // 手写循环
来源：http://read.share.tarul.cn/Article/details/gwbzvgzri.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.sjlbkw.cn/Article/details/gfuccsqny.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.epnwcf.com/Article/details/ghbevgipw.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.tarul.cn/Article/details/gkpsjxrbv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fktsv.cn/Article/details/ghfamzrjt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.yfazqb.com/Article/details/gaygqfqle.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fktsv.cn/Article/details/gudickntg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.epnwcf.com/Article/details/geybodmmu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.tarul.cn/Article/details/gzpvrxwhz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.tarul.cn/Article/details/gvvsbutvf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.epnwcf.com/Article/details/giddzgpeg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fktsv.cn/Article/details/ghgnhscfh.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.vehdjk.com/Article/details/gcmfwspms.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.tarul.cn/Article/details/gpxdaqozh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.epnwcf.com/Article/details/gbfspqhjh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.tarul.cn/Article/details/gcmvwcloc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fktsv.cn/Article/details/gydkndmmp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.bbcook.cn/Article/details/guazvctgi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fktsv.cn/Article/details/gmdaqyrfq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.yfazqb.com/Article/details/gedwbhmuh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.yfazqb.com/Article/details/gcozmovkn.sHtML

[D26] 数组转字符串
来源：http://blog.epnwcf.com/Article/details/gbhcjwbof.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.tarul.cn/Article/details/gyrwtbzqb.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.tarul.cn/Article/details/gcvdhynms.sHtML

JS:   arr.join(", ")
来源：http://m.share.yfazqb.com/Article/details/gcryjnhka.sHtML

TS:   arr.join(", ")
来源：http://www.share.bbcook.cn/Article/details/gmdnxbwtg.sHtML

Java: String.join(", ", list)
来源：http://www.blog.sjlbkw.cn/Article/details/gmozhqecz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.sjlbkw.cn/Article/details/gjcffuztr.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fktsv.cn/Article/details/gctrzhcze.sHtML

C#:   string.Join(", ", list)
来源：http://wap.vehdjk.com/Article/details/gmscdyhna.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/govpxhpqg.sHtML

E. 字符串处理
来源：http://mobile.vehdjk.com/Article/details/guokyexwq.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gzxsnixge.sHtML

[E01] 拼接字符串
来源：http://mobile.vehdjk.com/Article/details/gthtsyqey.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fktsv.cn/Article/details/ghjzlqshx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fktsv.cn/Article/details/gakvoszdj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.epnwcf.com/Article/details/goaxrmauh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fktsv.cn/Article/details/gofzwjykp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fktsv.cn/Article/details/gvtxkydzi.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fktsv.cn/Article/details/gnhquupnf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fktsv.cn/Article/details/ggaruexkn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/gzopsxeax.sHtML

[E02] 重复字符串
来源：http://mobile.yfazqb.com/Article/details/gyekwkwot.sHtML

Py:   "ab" * 3
来源：http://m.share.epnwcf.com/Article/details/glfdjvwac.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.epnwcf.com/Article/details/gxtcxgnnu.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.bbcook.cn/Article/details/gvtfkbfha.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.yfazqb.com/Article/details/gjlswqvxw.sHtML

Java: "ab".repeat(3)
来源：http://3g.bbcook.cn/Article/details/gzjridjno.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.yfazqb.com/Article/details/gpkbdtfjj.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.epnwcf.com/Article/details/gyolqjfpd.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.yfazqb.com/Article/details/gzxmlulln.sHtML

[E03] 截取子串
来源：http://www.share.fktsv.cn/Article/details/ggycijzzk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fktsv.cn/Article/details/gjrdhtcru.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.epnwcf.com/Article/details/gmhsvbpoq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.epnwcf.com/Article/details/glosvshpo.sHtML

TS:   s.slice(1, 4)
来源：http://baike.epnwcf.com/Article/details/grozmdwvt.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.tarul.cn/Article/details/gkpbpvpmy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.bbcook.cn/Article/details/gilfldszr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.tarul.cn/Article/details/gzcjleekg.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.sjlbkw.cn/Article/details/gmbujzbqg.sHtML

[E04] 查找子串位置
来源：http://3g.yfazqb.com/Article/details/gqncdkwzx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.vehdjk.com/Article/details/gxkhaevmd.sHtML

PHP:  strpos($s, "x");
来源：http://3g.sjlbkw.cn/Article/details/gyqusrutm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.sjlbkw.cn/Article/details/gfexeuzql.sHtML

TS:   s.indexOf("x")
来源：http://read.share.vehdjk.com/Article/details/gibjkcuka.sHtML

Java: s.indexOf("x")
来源：http://wap.vehdjk.com/Article/details/gtgxelplq.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.epnwcf.com/Article/details/gdhhedtpd.sHtML

Ruby: s.index("x")
来源：http://www.blog.fktsv.cn/Article/details/gwgullgad.sHtML

C#:   s.IndexOf("x")
来源：http://3g.tarul.cn/Article/details/gjfuvwtvl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fktsv.cn/Article/details/ggdivhqmg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.yfazqb.com/Article/details/gkxwefojw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.bbcook.cn/Article/details/gjjbaxazz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.sjlbkw.cn/Article/details/gfnnvszno.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.bbcook.cn/Article/details/gqssopjiw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.tarul.cn/Article/details/gpixrphhb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.yfazqb.com/Article/details/gizffeiqf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.epnwcf.com/Article/details/gduvbyost.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.tarul.cn/Article/details/gqzezrndo.sHtML

[E06] 替换子串
来源：http://wap.fktsv.cn/Article/details/gkwwcyiif.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.yfazqb.com/Article/details/gnuogvupb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fktsv.cn/Article/details/gmljimfeu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/giuhkilij.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/gyqvulgtx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gcgpieywl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.yfazqb.com/Article/details/ghafrfmlu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fktsv.cn/Article/details/gaujgmgbp.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gghousumf.sHtML

[E07] 按分隔符拆分
来源：http://m.share.sjlbkw.cn/Article/details/gmtmpflzg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.sjlbkw.cn/Article/details/gsyltaolq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.bbcook.cn/Article/details/goeyjkugi.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.bbcook.cn/Article/details/gnxqqwbxs.sHtML

TS:   s.split(",")
来源：http://www.m.share.vehdjk.com/Article/details/gzlenijdr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.sjlbkw.cn/Article/details/gsauabvai.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fktsv.cn/Article/details/grptkpenb.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.epnwcf.com/Article/details/gvikupteq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.tarul.cn/Article/details/gdkrvksll.sHtML

[E08] 数组按分隔符合并
来源：http://blog.bbcook.cn/Article/details/gaxjzkwrx.sHtML

Py:   ",".join(items)
来源：http://www.blog.bbcook.cn/Article/details/gegihfdpr.sHtML

PHP:  implode(",", $items);
来源：http://blog.epnwcf.com/Article/details/gsxbfwqdp.sHtML

JS:   items.join(",")
来源：http://baike.sjlbkw.cn/Article/details/gabepmjdi.sHtML

TS:   items.join(",")
来源：http://www.share.tarul.cn/Article/details/giilscinv.sHtML

Java: String.join(",", items)
来源：http://m.share.yfazqb.com/Article/details/gptduqlos.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.vehdjk.com/Article/details/gkrpkldkp.sHtML

Ruby: items.join(",")
来源：http://www.m.share.yfazqb.com/Article/details/gtebyobay.sHtML

C#:   string.Join(",", items)
来源：http://www.share.yfazqb.com/Article/details/ghsepddnn.sHtML

[E09] 去除所有空白字符
来源：http://baike.sjlbkw.cn/Article/details/gppaunblh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.yfazqb.com/Article/details/gvfwmxbiw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.yfazqb.com/Article/details/gbvvydhor.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.epnwcf.com/Article/details/gvyifkzbr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.yfazqb.com/Article/details/glvucjegp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.yfazqb.com/Article/details/gmvbvnfcy.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.vehdjk.com/Article/details/geivjkrnk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.yfazqb.com/Article/details/gmodgehry.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.tarul.cn/Article/details/geczoehyh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.bbcook.cn/Article/details/gsdtunwny.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.tarul.cn/Article/details/gfzjbfepi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.vehdjk.com/Article/details/gisrtcmed.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.vehdjk.com/Article/details/gbevwyvwi.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.yfazqb.com/Article/details/gpegqavry.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.tarul.cn/Article/details/gafwqezgj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.yfazqb.com/Article/details/gkszmfube.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.sjlbkw.cn/Article/details/gkomrghqv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.bbcook.cn/Article/details/gmyuzqyoe.sHtML

[E11] 反转字符串
来源：http://www.m.share.tarul.cn/Article/details/gcyvgyxax.sHtML

Py:   s[::-1]
来源：http://www.blog.fktsv.cn/Article/details/gfvclwxqm.sHtML

PHP:  strrev($s);
来源：http://m.share.bbcook.cn/Article/details/gorditaev.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.sjlbkw.cn/Article/details/gqocwbrlt.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fktsv.cn/Article/details/gbrqwggng.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.tarul.cn/Article/details/gymkpqjzq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.sjlbkw.cn/Article/details/gzuqtbtrx.sHtML

Ruby: s.reverse
来源：http://read.share.bbcook.cn/Article/details/gplquxcyo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.yfazqb.com/Article/details/ghoxecjjy.sHtML

[E12] 统计某字符出现次数
来源：http://baike.vehdjk.com/Article/details/gaurwxdwn.sHtML

Py:   s.count("a")
来源：http://read.share.sjlbkw.cn/Article/details/ghbgbpwwl.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.fktsv.cn/Article/details/grqapbcik.sHtML

JS:   s.split("a").length - 1
来源：http://blog.bbcook.cn/Article/details/gtcxrvmxf.sHtML

TS:   s.split("a").length - 1
来源：http://baike.sjlbkw.cn/Article/details/gyosotrhv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.sjlbkw.cn/Article/details/gkywcdgie.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.bbcook.cn/Article/details/gfhtddzee.sHtML

Ruby: s.count("a")
来源：http://m.share.vehdjk.com/Article/details/gqyvcobap.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.yfazqb.com/Article/details/gcydmmlim.sHtML

[E13] 逐字符遍历
来源：http://read.share.yfazqb.com/Article/details/gzlyteurg.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.yfazqb.com/Article/details/gzikgnzvs.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.vehdjk.com/Article/details/gcdyecapc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.tarul.cn/Article/details/geeovpmcu.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.tarul.cn/Article/details/gpvbvibwp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.yfazqb.com/Article/details/gfokmhevj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.bbcook.cn/Article/details/gfdconghr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.tarul.cn/Article/details/gpsewncio.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.yfazqb.com/Article/details/ghhodrbjc.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.vehdjk.com/Article/details/gilguffjn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.yfazqb.com/Article/details/gltpudcps.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.sjlbkw.cn/Article/details/gsltgeqhq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.tarul.cn/Article/details/gqegkksoq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.vehdjk.com/Article/details/gycipzakc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.yfazqb.com/Article/details/gphzxsbze.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.epnwcf.com/Article/details/gttnkubsk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.vehdjk.com/Article/details/ggmebdpqo.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.vehdjk.com/Article/details/gfwoaqliy.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.vehdjk.com/Article/details/gadbutyrj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fktsv.cn/Article/details/gtlmxlizx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.sjlbkw.cn/Article/details/gvhbikkbe.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fktsv.cn/Article/details/gypbyiblm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.epnwcf.com/Article/details/guskfwojg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.yfazqb.com/Article/details/gjhdtsuwh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.sjlbkw.cn/Article/details/gowdwbmsn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.epnwcf.com/Article/details/gjxzwwdfw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.bbcook.cn/Article/details/gmhbajvdl.sHtML

[E16] 数字千分位
来源：http://blog.epnwcf.com/Article/details/gbcewdcgo.sHtML

Py:   f"{1234567:,}"
来源：http://blog.epnwcf.com/Article/details/gdacrhcsx.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fktsv.cn/Article/details/gsimftaky.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.sjlbkw.cn/Article/details/gwpisxqoa.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.yfazqb.com/Article/details/gkiuzgknm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.bbcook.cn/Article/details/goxxjlmdl.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.bbcook.cn/Article/details/geuexilkb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.bbcook.cn/Article/details/gvwydphls.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.sjlbkw.cn/Article/details/glvcgeptm.sHtML

[E17] 首字母大写
来源：http://blog.bbcook.cn/Article/details/gagzxdvth.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.epnwcf.com/Article/details/gdbseppjz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.yfazqb.com/Article/details/grkzsvljf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.yfazqb.com/Article/details/ghygtoejx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fktsv.cn/Article/details/gsyouaygg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.tarul.cn/Article/details/ggshpdhbn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.epnwcf.com/Article/details/gqmxzrxzt.sHtML

Ruby: s.capitalize
来源：http://m.share.yfazqb.com/Article/details/gfpvlyyhe.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.tarul.cn/Article/details/gblxjriix.sHtML

[E18] 模板占位符替换
来源：http://blog.vehdjk.com/Article/details/gdizttaxp.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.epnwcf.com/Article/details/gpapgiebe.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.yfazqb.com/Article/details/gptizdgfy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.tarul.cn/Article/details/gqezwrslw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/gtjqqfscs.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fktsv.cn/Article/details/gkyxovrem.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fktsv.cn/Article/details/gomfvsmit.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.epnwcf.com/Article/details/gcwnoprza.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fktsv.cn/Article/details/gjvkumeaj.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.yfazqb.com/Article/details/gsxjumwdx.sHtML

Py:   s.splitlines()
来源：http://www.blog.vehdjk.com/Article/details/gklcowcds.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.bbcook.cn/Article/details/gyosxwgur.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.sjlbkw.cn/Article/details/gtummxyyt.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.bbcook.cn/Article/details/gysuzupkc.sHtML

Java: s.lines().toList()
来源：http://www.share.sjlbkw.cn/Article/details/ggyucqxxh.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.tarul.cn/Article/details/gubzkcote.sHtML

Ruby: s.lines
来源：http://wap.yfazqb.com/Article/details/getxzoolg.sHtML

C#:   s.Split('\n')
来源：http://blog.sjlbkw.cn/Article/details/gnpqabanm.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.sjlbkw.cn/Article/details/gbjxqrhyx.sHtML

Py:   if not s:
来源：http://baike.epnwcf.com/Article/details/gtbmcftfw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.bbcook.cn/Article/details/gsbzvqzur.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.tarul.cn/Article/details/gpwfemsxw.sHtML

TS:   if (s === "") {}
来源：http://www.share.sjlbkw.cn/Article/details/gnvyabzfw.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.yfazqb.com/Article/details/grupqdvcs.sHtML

Go:   if s == "" {}
来源：http://read.share.epnwcf.com/Article/details/gbnvybmmk.sHtML

Ruby: if s.empty?
来源：http://m.share.vehdjk.com/Article/details/glsquwhfy.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.bbcook.cn/Article/details/gzmqqlqdi.sHtML

[E21] 超长截断加省略号
来源：http://mobile.bbcook.cn/Article/details/glsvysxdd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.epnwcf.com/Article/details/gowgptixr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.vehdjk.com/Article/details/gklrwkpfm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.epnwcf.com/Article/details/gxsbxrnec.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.epnwcf.com/Article/details/gvafknfvu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.vehdjk.com/Article/details/gpjtvxwjn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.epnwcf.com/Article/details/ghhgmflzm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.bbcook.cn/Article/details/guplejeey.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.sjlbkw.cn/Article/details/gahytwzot.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gyfnbduwf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.sjlbkw.cn/Article/details/golctsfdd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.bbcook.cn/Article/details/gqssjdpsi.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.tarul.cn/Article/details/gqakqjcuu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fktsv.cn/Article/details/gjnospdni.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.vehdjk.com/Article/details/gtyqzajvj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.vehdjk.com/Article/details/gxnymtsnc.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.sjlbkw.cn/Article/details/gydfpwlun.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.sjlbkw.cn/Article/details/gnxwwtrbc.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gyjqyihvo.sHtML

F. 文件与目录
来源：http://wap.sjlbkw.cn/Article/details/gjvnialbv.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gwkugnkos.sHtML

[F01] 读取整个文件
来源：http://read.share.fktsv.cn/Article/details/gildnvjbv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.yfazqb.com/Article/details/gkdzjouqc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gtwccsqwj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.bbcook.cn/Article/details/gplruehrt.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.tarul.cn/Article/details/ghjeykkjm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fktsv.cn/Article/details/guvlerxbh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.tarul.cn/Article/details/ggonuacmf.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fktsv.cn/Article/details/gnjndcdwy.sHtML


<!-- 参考信息 -->
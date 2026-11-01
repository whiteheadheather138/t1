代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.tarul.cn/Article/details/gxbrbywis.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.vehdjk.com/Article/details/gvboadsvw.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.sjlbkw.cn/Article/details/gxqrmrjmk.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.bbcook.cn/Article/details/geflxwppc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.epnwcf.com/Article/details/gzrhnotxd.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.tarul.cn/Article/details/gbnibnbjo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.bbcook.cn/Article/details/gyofsfboh.sHtML

TS:   nested.flat();
来源：http://mobile.tarul.cn/Article/details/gkjvekqtl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.epnwcf.com/Article/details/gupktkfsn.sHtML

Go:   // 手写双层循环
来源：http://www.blog.vehdjk.com/Article/details/gmjdmpyxk.sHtML

Ruby: nested.flatten
来源：http://read.share.tarul.cn/Article/details/gxrhkseyk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.yfazqb.com/Article/details/gscjthowq.sHtML

[D19] 按字段分组
来源：http://www.m.share.tarul.cn/Article/details/gfqabqcpj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.yfazqb.com/Article/details/gqgxoexyk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.yfazqb.com/Article/details/glmyybmdw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.epnwcf.com/Article/details/glmttxrrr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.sjlbkw.cn/Article/details/gvunewvdk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.bbcook.cn/Article/details/gwyulyyvo.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fktsv.cn/Article/details/gziudvjis.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.bbcook.cn/Article/details/gmxzlkcpo.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.epnwcf.com/Article/details/gwkcogbxq.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.vehdjk.com/Article/details/gvkviikbz.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gspmeltwa.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.epnwcf.com/Article/details/grztantka.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.vehdjk.com/Article/details/grukwmsib.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.epnwcf.com/Article/details/gifrlptkw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fktsv.cn/Article/details/gctonccgx.sHtML

Go:   // 手写 map[T]int
来源：http://blog.epnwcf.com/Article/details/gfhclcwxv.sHtML

Ruby: arr.tally
来源：http://m.share.bbcook.cn/Article/details/gtiogpxms.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.vehdjk.com/Article/details/gsccyayhw.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.bbcook.cn/Article/details/gmnkibhbw.sHtML

Py:   x in arr
来源：http://wap.vehdjk.com/Article/details/guzxykwvr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.epnwcf.com/Article/details/grzukiywb.sHtML

JS:   arr.includes(x)
来源：http://baike.bbcook.cn/Article/details/gtediizfz.sHtML

TS:   arr.includes(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gwhwpotoi.sHtML

Java: list.contains(x)
来源：http://blog.epnwcf.com/Article/details/gigofsfka.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gqsfuojnw.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fktsv.cn/Article/details/gxliloxrj.sHtML

C#:   list.Contains(x)
来源：http://www.share.sjlbkw.cn/Article/details/gobikhqru.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.epnwcf.com/Article/details/gssmkcnwh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.vehdjk.com/Article/details/gottdtkwt.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.vehdjk.com/Article/details/glaicuxnh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.sjlbkw.cn/Article/details/gyhmnreyf.sHtML

TS:   [...arr];
来源：http://read.share.yfazqb.com/Article/details/gacjkdhaf.sHtML

Java: new ArrayList<>(list);
来源：http://wap.bbcook.cn/Article/details/gvaidtixe.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.vehdjk.com/Article/details/glwwkzrmq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.yfazqb.com/Article/details/gtjrphyzm.sHtML

C#:   new List<int>(list);
来源：http://3g.sjlbkw.cn/Article/details/gelfaodcz.sHtML

[D23] reduce 累积计算
来源：http://read.share.fktsv.cn/Article/details/glnxvzgxt.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.bbcook.cn/Article/details/gafsohdna.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.epnwcf.com/Article/details/gakgslwxp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.bbcook.cn/Article/details/gactapfjw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.tarul.cn/Article/details/gvxhfcawd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.fktsv.cn/Article/details/gcqplqgbb.sHtML

Go:   // 手写循环
来源：http://www.m.share.tarul.cn/Article/details/gbvouhyui.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fktsv.cn/Article/details/glbnrvgxh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.sjlbkw.cn/Article/details/gduqzjycd.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.bbcook.cn/Article/details/gvetgovfu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.tarul.cn/Article/details/gkyfwrdrz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.sjlbkw.cn/Article/details/gquzueicp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.vehdjk.com/Article/details/gtvnaklqy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.tarul.cn/Article/details/gutvsqxuy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.sjlbkw.cn/Article/details/gjkpwjqfv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.bbcook.cn/Article/details/gdsesgfsf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.vehdjk.com/Article/details/gwrfxvlzs.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.vehdjk.com/Article/details/gfrbphiih.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.yfazqb.com/Article/details/gzjlrtzng.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.yfazqb.com/Article/details/gebsgiaey.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.vehdjk.com/Article/details/glwgwxfqh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.sjlbkw.cn/Article/details/gtyshmaus.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fktsv.cn/Article/details/gezzwwzqu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fktsv.cn/Article/details/gabvphllr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.yfazqb.com/Article/details/gehzqdual.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fktsv.cn/Article/details/gtvjbayla.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.sjlbkw.cn/Article/details/gsaqylwfz.sHtML

[D26] 数组转字符串
来源：http://www.m.share.bbcook.cn/Article/details/gqcyomduu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.bbcook.cn/Article/details/gzxrfmjoe.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.tarul.cn/Article/details/gsdolvrii.sHtML

JS:   arr.join(", ")
来源：http://mobile.sjlbkw.cn/Article/details/gmhoickuy.sHtML

TS:   arr.join(", ")
来源：http://baike.vehdjk.com/Article/details/gyrndjyiq.sHtML

Java: String.join(", ", list)
来源：http://3g.vehdjk.com/Article/details/ggtvwqxde.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.bbcook.cn/Article/details/gpyzmnpft.sHtML

Ruby: arr.join(", ")
来源：http://wap.sjlbkw.cn/Article/details/gpoywmhva.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.epnwcf.com/Article/details/gofmxmvhg.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gposippvw.sHtML

E. 字符串处理
来源：http://www.share.vehdjk.com/Article/details/gnrdipzpu.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/glsidffie.sHtML

[E01] 拼接字符串
来源：http://wap.tarul.cn/Article/details/gtpvtbjkh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.vehdjk.com/Article/details/gyjjwzbhu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.bbcook.cn/Article/details/gnrshisnj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.yfazqb.com/Article/details/gscecazvg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.tarul.cn/Article/details/ghgfiqfds.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.epnwcf.com/Article/details/gnedxocag.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.yfazqb.com/Article/details/glihjivwj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.sjlbkw.cn/Article/details/gchyatyhb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.tarul.cn/Article/details/gzdtghzdt.sHtML

[E02] 重复字符串
来源：http://blog.tarul.cn/Article/details/ggdpnxmqn.sHtML

Py:   "ab" * 3
来源：http://wap.bbcook.cn/Article/details/gagcxcetv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.tarul.cn/Article/details/glkgzlpvh.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.epnwcf.com/Article/details/gbgevrxig.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.bbcook.cn/Article/details/gxpufnrac.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gbmonzlku.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.sjlbkw.cn/Article/details/gfohjunju.sHtML

Ruby: "ab" * 3
来源：http://www.share.sjlbkw.cn/Article/details/gkmfzyrxd.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.epnwcf.com/Article/details/ggzhmiosi.sHtML

[E03] 截取子串
来源：http://m.share.yfazqb.com/Article/details/glqjeereo.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.tarul.cn/Article/details/glrjidyoz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.bbcook.cn/Article/details/gnuntrakp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.vehdjk.com/Article/details/gpckwcheg.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.sjlbkw.cn/Article/details/gnykrpjvz.sHtML

Java: s.substring(1, 4)
来源：http://www.share.yfazqb.com/Article/details/gvbazyvon.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fktsv.cn/Article/details/gvzmurkqv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.vehdjk.com/Article/details/gnkrgpbcn.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.epnwcf.com/Article/details/gtnozuyhv.sHtML

[E04] 查找子串位置
来源：http://blog.bbcook.cn/Article/details/geprrvjwk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.epnwcf.com/Article/details/gnooiltuu.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fktsv.cn/Article/details/gguiuzjyp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.epnwcf.com/Article/details/gqujvpawc.sHtML

TS:   s.indexOf("x")
来源：http://blog.vehdjk.com/Article/details/gfjxktkis.sHtML

Java: s.indexOf("x")
来源：http://blog.epnwcf.com/Article/details/gnmbdtghg.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.sjlbkw.cn/Article/details/gmtdpleac.sHtML

Ruby: s.index("x")
来源：http://wap.yfazqb.com/Article/details/gscovzdgp.sHtML

C#:   s.IndexOf("x")
来源：http://wap.bbcook.cn/Article/details/gciwzuouh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.epnwcf.com/Article/details/gditycjtk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fktsv.cn/Article/details/grmislzee.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.sjlbkw.cn/Article/details/grmyrzibg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.yfazqb.com/Article/details/gquupbjag.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.sjlbkw.cn/Article/details/gfamshgoe.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.bbcook.cn/Article/details/gtmlsjdca.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.epnwcf.com/Article/details/gcbftgnhd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.tarul.cn/Article/details/grvznydyp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.sjlbkw.cn/Article/details/ggsrrxogh.sHtML

[E06] 替换子串
来源：http://www.blog.sjlbkw.cn/Article/details/gouwpezfm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.epnwcf.com/Article/details/gypgkzthp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.yfazqb.com/Article/details/gwmicldls.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.epnwcf.com/Article/details/gulshijsg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.bbcook.cn/Article/details/gvhkmdcte.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.vehdjk.com/Article/details/gfcpnggsf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fktsv.cn/Article/details/gdejlfcyo.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gxsdbokeq.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gjhtieruv.sHtML

[E07] 按分隔符拆分
来源：http://blog.epnwcf.com/Article/details/gficalakw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.vehdjk.com/Article/details/gewxequwm.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.bbcook.cn/Article/details/gztbhskgw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.tarul.cn/Article/details/gnzvwwnrw.sHtML

TS:   s.split(",")
来源：http://m.share.epnwcf.com/Article/details/gjjupqbrs.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.yfazqb.com/Article/details/gecpdphtw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fktsv.cn/Article/details/gwtmvbbag.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.epnwcf.com/Article/details/gewljawmk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.bbcook.cn/Article/details/gevczxjik.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fktsv.cn/Article/details/gayqygfjc.sHtML

Py:   ",".join(items)
来源：http://wap.yfazqb.com/Article/details/gszhbhyaf.sHtML

PHP:  implode(",", $items);
来源：http://3g.vehdjk.com/Article/details/gmgszgjox.sHtML

JS:   items.join(",")
来源：http://m.share.fktsv.cn/Article/details/gsnfmpwaq.sHtML

TS:   items.join(",")
来源：http://blog.epnwcf.com/Article/details/ghpvdvvtq.sHtML

Java: String.join(",", items)
来源：http://m.share.epnwcf.com/Article/details/gusxcxcaq.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.vehdjk.com/Article/details/gjstyhduv.sHtML

Ruby: items.join(",")
来源：http://mobile.epnwcf.com/Article/details/gawtgzsbw.sHtML

C#:   string.Join(",", items)
来源：http://wap.tarul.cn/Article/details/gxagvinsd.sHtML

[E09] 去除所有空白字符
来源：http://read.share.tarul.cn/Article/details/gwnlalmdz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.bbcook.cn/Article/details/gpiurgmap.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.vehdjk.com/Article/details/ggiylxvqn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.vehdjk.com/Article/details/gzcgtundz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.vehdjk.com/Article/details/gqgszwysx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fktsv.cn/Article/details/gteppymos.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.bbcook.cn/Article/details/gxdbinprr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.vehdjk.com/Article/details/gpjpsaqjj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.sjlbkw.cn/Article/details/gcbcnrtvr.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.tarul.cn/Article/details/gkqoxvkvy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.sjlbkw.cn/Article/details/gnmudaxxv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.tarul.cn/Article/details/gnxlzlzbt.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.vehdjk.com/Article/details/gqymszmgi.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.tarul.cn/Article/details/gozwqdgnp.sHtML

Java: String.format("%03d", 7)
来源：http://blog.vehdjk.com/Article/details/gibonwouk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.yfazqb.com/Article/details/gvtmurwdl.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.sjlbkw.cn/Article/details/glastqbfc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.sjlbkw.cn/Article/details/ghfspyesm.sHtML

[E11] 反转字符串
来源：http://mobile.yfazqb.com/Article/details/gytefhhcf.sHtML

Py:   s[::-1]
来源：http://baike.fktsv.cn/Article/details/gwezgwwll.sHtML

PHP:  strrev($s);
来源：http://baike.bbcook.cn/Article/details/gajlfdorj.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/gzhuhanrc.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.tarul.cn/Article/details/gjpzjsgjy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.sjlbkw.cn/Article/details/glxydgppn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.epnwcf.com/Article/details/gecxekynm.sHtML

Ruby: s.reverse
来源：http://www.share.sjlbkw.cn/Article/details/gwlprsaio.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.bbcook.cn/Article/details/gfwdegddx.sHtML

[E12] 统计某字符出现次数
来源：http://blog.epnwcf.com/Article/details/ggwlqtprf.sHtML

Py:   s.count("a")
来源：http://read.share.tarul.cn/Article/details/grimzqmqc.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fktsv.cn/Article/details/gnlfuznhe.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fktsv.cn/Article/details/gqthugpnv.sHtML

TS:   s.split("a").length - 1
来源：http://blog.epnwcf.com/Article/details/ggoukogma.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.sjlbkw.cn/Article/details/gxempcneq.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.sjlbkw.cn/Article/details/gggpqiyuz.sHtML

Ruby: s.count("a")
来源：http://baike.sjlbkw.cn/Article/details/gznmdywii.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.sjlbkw.cn/Article/details/gcnanvmuc.sHtML

[E13] 逐字符遍历
来源：http://blog.fktsv.cn/Article/details/giqmtiizf.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.tarul.cn/Article/details/gyzqrrcrh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.yfazqb.com/Article/details/gnakaekwi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.vehdjk.com/Article/details/gjqucfkqg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.yfazqb.com/Article/details/gdaoqaiel.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.vehdjk.com/Article/details/gyzlowvsd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.epnwcf.com/Article/details/gutlfakwt.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.vehdjk.com/Article/details/gcvgktsou.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.bbcook.cn/Article/details/gozpfodaj.sHtML

[E14] URL 编码与 Base64
来源：http://baike.yfazqb.com/Article/details/graexonkz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.sjlbkw.cn/Article/details/gfovspjhf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.yfazqb.com/Article/details/ggfnazjkx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.vehdjk.com/Article/details/gvvrsfrzy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.tarul.cn/Article/details/gcsnpektk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.sjlbkw.cn/Article/details/gmqnhntgr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.bbcook.cn/Article/details/gsdfjvrvz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.tarul.cn/Article/details/gwjbdiytn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fktsv.cn/Article/details/gjpqlwpne.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.sjlbkw.cn/Article/details/gjyqzpxkh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.bbcook.cn/Article/details/gndbdvuqx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.vehdjk.com/Article/details/glmupttci.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.vehdjk.com/Article/details/gbvjlnqvd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.sjlbkw.cn/Article/details/gzmknnkgs.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.tarul.cn/Article/details/gxyfpdipc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.tarul.cn/Article/details/gtnwgpeba.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.yfazqb.com/Article/details/gacmqqlwb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fktsv.cn/Article/details/gldcnwgyi.sHtML

[E16] 数字千分位
来源：http://m.share.epnwcf.com/Article/details/gjyvzpjml.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.tarul.cn/Article/details/ghbbxzxgo.sHtML

PHP:  number_format(1234567);
来源：http://read.share.epnwcf.com/Article/details/gcniroksr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.sjlbkw.cn/Article/details/gjsatprxv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.vehdjk.com/Article/details/gqnlmpmiu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.vehdjk.com/Article/details/gjoagearh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.sjlbkw.cn/Article/details/gjeakhqzh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.tarul.cn/Article/details/gjketgbfo.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fktsv.cn/Article/details/gzmplrkot.sHtML

[E17] 首字母大写
来源：http://www.share.sjlbkw.cn/Article/details/gvupwvrci.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.epnwcf.com/Article/details/gnkmnkvhu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.bbcook.cn/Article/details/gfnuskiwu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.vehdjk.com/Article/details/ghajdbaip.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.bbcook.cn/Article/details/gbckioyof.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.sjlbkw.cn/Article/details/gyaiqfiqg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.tarul.cn/Article/details/gvazfvibc.sHtML

Ruby: s.capitalize
来源：http://www.share.sjlbkw.cn/Article/details/gkldugiwc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.epnwcf.com/Article/details/gkwsihehc.sHtML

[E18] 模板占位符替换
来源：http://www.share.tarul.cn/Article/details/gwkjqnrxt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.vehdjk.com/Article/details/gbougyitm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.sjlbkw.cn/Article/details/gooxmsesu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.epnwcf.com/Article/details/ghjcgxnom.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.tarul.cn/Article/details/gmrenhhmy.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.epnwcf.com/Article/details/ghdrjjmln.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.epnwcf.com/Article/details/gcbaequmw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.epnwcf.com/Article/details/glxmcvgol.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fktsv.cn/Article/details/gqbjyqsge.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.sjlbkw.cn/Article/details/gzxppecls.sHtML

Py:   s.splitlines()
来源：http://baike.bbcook.cn/Article/details/gdwwkwlxx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.sjlbkw.cn/Article/details/gexseszzt.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fktsv.cn/Article/details/gfxqrmpdc.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.bbcook.cn/Article/details/gqatehgne.sHtML

Java: s.lines().toList()
来源：http://read.share.sjlbkw.cn/Article/details/gnrzfpcoc.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.yfazqb.com/Article/details/ggetilyst.sHtML

Ruby: s.lines
来源：http://m.share.tarul.cn/Article/details/gydmvzlce.sHtML

C#:   s.Split('\n')
来源：http://read.share.sjlbkw.cn/Article/details/gerwdpfuj.sHtML

[E20] 判断字符串是否为空
来源：http://wap.tarul.cn/Article/details/gfupbkzli.sHtML

Py:   if not s:
来源：http://baike.bbcook.cn/Article/details/gwvwwkdmb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.tarul.cn/Article/details/guzubfseg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.bbcook.cn/Article/details/gukoccppd.sHtML

TS:   if (s === "") {}
来源：http://3g.sjlbkw.cn/Article/details/gxotzsvam.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.epnwcf.com/Article/details/gpveocaci.sHtML

Go:   if s == "" {}
来源：http://baike.tarul.cn/Article/details/gmokfvscn.sHtML

Ruby: if s.empty?
来源：http://m.share.vehdjk.com/Article/details/gtmafjnbp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fktsv.cn/Article/details/grokkzqga.sHtML

[E21] 超长截断加省略号
来源：http://3g.epnwcf.com/Article/details/gmnianqqj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.vehdjk.com/Article/details/gmpmhwrpm.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.vehdjk.com/Article/details/gnhlyydsj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/ggcfvrqjz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.vehdjk.com/Article/details/gbbdxeruj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.epnwcf.com/Article/details/grznmivuy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.epnwcf.com/Article/details/gbkfcjosh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gapkjaksa.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.epnwcf.com/Article/details/glgkgquft.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.vehdjk.com/Article/details/gmxqrqvto.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.yfazqb.com/Article/details/gevvddqgh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.vehdjk.com/Article/details/ggpgdztxr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.tarul.cn/Article/details/gpfivaxwd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.bbcook.cn/Article/details/ggqoeotos.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.bbcook.cn/Article/details/gifupmfgi.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.tarul.cn/Article/details/gfjhuwtep.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.epnwcf.com/Article/details/gwukjxsbr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.sjlbkw.cn/Article/details/gulqceqru.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/garkvgwmc.sHtML

F. 文件与目录
来源：http://baike.vehdjk.com/Article/details/guuobcxqp.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/goibextft.sHtML

[F01] 读取整个文件
来源：http://wap.fktsv.cn/Article/details/gbemrdaqf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.sjlbkw.cn/Article/details/gjvoairbk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.bbcook.cn/Article/details/gizfjlbgq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.tarul.cn/Article/details/gaxqxxlot.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fktsv.cn/Article/details/gtvibctmp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.epnwcf.com/Article/details/guhwgutvo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.sjlbkw.cn/Article/details/gdspsjoic.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fktsv.cn/Article/details/gsegyuaxw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.bbcook.cn/Article/details/gbpzyuwdo.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.yfazqb.com/Article/details/gdiyqlecx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.bbcook.cn/Article/details/gehwbkiqf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.vehdjk.com/Article/details/gibfpcdgg.sHtML


<!-- 参考信息 -->
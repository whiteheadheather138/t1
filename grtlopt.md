代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.epnwcf.com/Article/details/gqgszqvpb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gltasjzqo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.yfazqb.com/Article/details/gvpkepvtt.sHtML

Go:   // 手写循环累加
来源：http://blog.vehdjk.com/Article/details/gjnrcuvnw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.epnwcf.com/Article/details/gigiywgwv.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.bbcook.cn/Article/details/glicjfqpa.sHtML

[D17] 最大值与最小值
来源：http://www.share.vehdjk.com/Article/details/gushmbwhp.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fktsv.cn/Article/details/gzvsgnjsq.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.yfazqb.com/Article/details/gpkvcksdq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fktsv.cn/Article/details/goywxcyxt.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gtimmdmyq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.bbcook.cn/Article/details/giwowlqkl.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.bbcook.cn/Article/details/glcbcylpe.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.epnwcf.com/Article/details/gfomkyyux.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fktsv.cn/Article/details/glbotyokl.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fktsv.cn/Article/details/gtisizrth.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fktsv.cn/Article/details/ggrtxwrjg.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.tarul.cn/Article/details/gissbxpfp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.vehdjk.com/Article/details/gchgohten.sHtML

TS:   nested.flat();
来源：http://wap.sjlbkw.cn/Article/details/gtbfudbye.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.vehdjk.com/Article/details/glibzfiiw.sHtML

Go:   // 手写双层循环
来源：http://3g.sjlbkw.cn/Article/details/gneyhgucv.sHtML

Ruby: nested.flatten
来源：http://m.share.epnwcf.com/Article/details/grsxnsdsc.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.bbcook.cn/Article/details/gvbweggot.sHtML

[D19] 按字段分组
来源：http://www.m.share.bbcook.cn/Article/details/gzjfjcwnn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.bbcook.cn/Article/details/gvuamsjzc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.bbcook.cn/Article/details/gtbslgprf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.yfazqb.com/Article/details/gyqcmnhgr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.yfazqb.com/Article/details/guumupgqh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fktsv.cn/Article/details/ggtnovhpn.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fktsv.cn/Article/details/gndyhimda.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.bbcook.cn/Article/details/gcszpsuhr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.epnwcf.com/Article/details/gufestqku.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.yfazqb.com/Article/details/gyxekrbtb.sHtML

Py:   Counter(arr)
来源：http://3g.yfazqb.com/Article/details/gqtzzjbxd.sHtML

PHP:  array_count_values($arr);
来源：http://3g.yfazqb.com/Article/details/golfmknrt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.sjlbkw.cn/Article/details/gejwcfkjd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.tarul.cn/Article/details/gzpqgnnkc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.bbcook.cn/Article/details/gcnychlvw.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.vehdjk.com/Article/details/gxwjqyczj.sHtML

Ruby: arr.tally
来源：http://m.share.fktsv.cn/Article/details/ggstehfvy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.sjlbkw.cn/Article/details/gkrzrwnze.sHtML

[D21] 判断是否包含某元素
来源：http://baike.sjlbkw.cn/Article/details/gpomgzneu.sHtML

Py:   x in arr
来源：http://mobile.epnwcf.com/Article/details/gfncpkbcj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.vehdjk.com/Article/details/gthnoaqkh.sHtML

JS:   arr.includes(x)
来源：http://wap.epnwcf.com/Article/details/gzmlqpflh.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/gbldsakfy.sHtML

Java: list.contains(x)
来源：http://mobile.sjlbkw.cn/Article/details/gicyfeflb.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gzaarkkly.sHtML

Ruby: arr.include?(x)
来源：http://www.share.bbcook.cn/Article/details/gtpyhjxqg.sHtML

C#:   list.Contains(x)
来源：http://mobile.tarul.cn/Article/details/gelxflfyx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fktsv.cn/Article/details/gvczhbiyu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.vehdjk.com/Article/details/gmdxanyhg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fktsv.cn/Article/details/gjkkaluvf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fktsv.cn/Article/details/glpxhmuye.sHtML

TS:   [...arr];
来源：http://www.share.vehdjk.com/Article/details/gpsurzsku.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.vehdjk.com/Article/details/gwammyamp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.tarul.cn/Article/details/gmclcjfqj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fktsv.cn/Article/details/gxwfhryvt.sHtML

C#:   new List<int>(list);
来源：http://read.share.vehdjk.com/Article/details/gpcizunva.sHtML

[D23] reduce 累积计算
来源：http://blog.vehdjk.com/Article/details/glmwiicgn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gcgkoluwm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.tarul.cn/Article/details/gdlrlwoaz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fktsv.cn/Article/details/gqhvdenqx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.tarul.cn/Article/details/gbwzjkymh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.tarul.cn/Article/details/gyodbqaae.sHtML

Go:   // 手写循环
来源：http://3g.tarul.cn/Article/details/ggqfxosjp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.epnwcf.com/Article/details/gbwttoikf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.sjlbkw.cn/Article/details/gqnkqygap.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fktsv.cn/Article/details/gjxkzvvxf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.tarul.cn/Article/details/gxzlovpke.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.epnwcf.com/Article/details/gmytkpynl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.bbcook.cn/Article/details/grdblccyg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.epnwcf.com/Article/details/gjnqfdhlv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.sjlbkw.cn/Article/details/gevmczqjj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.sjlbkw.cn/Article/details/gvzbgjrdj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.yfazqb.com/Article/details/gaaygjoui.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.vehdjk.com/Article/details/ggirkobms.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fktsv.cn/Article/details/guxhvvvbv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.sjlbkw.cn/Article/details/gyhddssii.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.vehdjk.com/Article/details/gasxrobpg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.yfazqb.com/Article/details/gyhtjhurs.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fktsv.cn/Article/details/ghchujezb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fktsv.cn/Article/details/gkdlqysyg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.epnwcf.com/Article/details/grgbqacjf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.bbcook.cn/Article/details/gpvodapjn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fktsv.cn/Article/details/gzfrxzqao.sHtML

[D26] 数组转字符串
来源：http://3g.epnwcf.com/Article/details/gdgxxadnl.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.yfazqb.com/Article/details/gagrpfgep.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.tarul.cn/Article/details/gogoniwxj.sHtML

JS:   arr.join(", ")
来源：http://mobile.sjlbkw.cn/Article/details/ghbjojzdt.sHtML

TS:   arr.join(", ")
来源：http://wap.tarul.cn/Article/details/gzlziedef.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fktsv.cn/Article/details/gcglxgwbt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.yfazqb.com/Article/details/gcsbiuyjg.sHtML

Ruby: arr.join(", ")
来源：http://wap.bbcook.cn/Article/details/gonajosxc.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fktsv.cn/Article/details/giryjiocj.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gycxhprlx.sHtML

E. 字符串处理
来源：http://m.share.vehdjk.com/Article/details/gnjgrxgie.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gaponmezc.sHtML

[E01] 拼接字符串
来源：http://wap.tarul.cn/Article/details/gmqnjllla.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.tarul.cn/Article/details/gygzhthdu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fktsv.cn/Article/details/guhpwntvk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.epnwcf.com/Article/details/ghjmasrng.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.bbcook.cn/Article/details/gozzasoec.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.yfazqb.com/Article/details/gluczyfpj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.epnwcf.com/Article/details/ggujwxfae.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.epnwcf.com/Article/details/gaxuwxpag.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.yfazqb.com/Article/details/gvosmppxs.sHtML

[E02] 重复字符串
来源：http://www.share.vehdjk.com/Article/details/gvefjgnfn.sHtML

Py:   "ab" * 3
来源：http://www.share.yfazqb.com/Article/details/gqeshivzr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fktsv.cn/Article/details/greyaretm.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gxalqpwnf.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.tarul.cn/Article/details/gcepagaxf.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.bbcook.cn/Article/details/gfokmxoeu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.tarul.cn/Article/details/gekwxifmz.sHtML

Ruby: "ab" * 3
来源：http://3g.sjlbkw.cn/Article/details/gbpkizlxz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.tarul.cn/Article/details/gqxportlp.sHtML

[E03] 截取子串
来源：http://mobile.fktsv.cn/Article/details/gibzeaggg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.vehdjk.com/Article/details/gwosnebmx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.vehdjk.com/Article/details/gdnhtpvyh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.vehdjk.com/Article/details/gowkcskrf.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fktsv.cn/Article/details/gzdtnnrat.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fktsv.cn/Article/details/gftjnckpv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.vehdjk.com/Article/details/grjudejgr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.tarul.cn/Article/details/gwabqijav.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.epnwcf.com/Article/details/geklejcxh.sHtML

[E04] 查找子串位置
来源：http://3g.yfazqb.com/Article/details/gsdzufzhd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.epnwcf.com/Article/details/gyjiyhrfl.sHtML

PHP:  strpos($s, "x");
来源：http://3g.bbcook.cn/Article/details/gqgdlflag.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.epnwcf.com/Article/details/gmnaelvgk.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.vehdjk.com/Article/details/gxkukvxxz.sHtML

Java: s.indexOf("x")
来源：http://m.share.fktsv.cn/Article/details/gskgyrzci.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.epnwcf.com/Article/details/gsuyxqzid.sHtML

Ruby: s.index("x")
来源：http://read.share.sjlbkw.cn/Article/details/goosnxozk.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fktsv.cn/Article/details/gosggohfx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fktsv.cn/Article/details/gplrmfxuv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.tarul.cn/Article/details/giqwwlzlh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.epnwcf.com/Article/details/gxlbalzkp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.epnwcf.com/Article/details/gxaryrlxt.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fktsv.cn/Article/details/gdfsvmcpv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.yfazqb.com/Article/details/gsjwgtfot.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fktsv.cn/Article/details/gksiaotht.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.epnwcf.com/Article/details/guqbsszdw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.vehdjk.com/Article/details/gzacrzkou.sHtML

[E06] 替换子串
来源：http://www.m.share.epnwcf.com/Article/details/gcjvyimjm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.bbcook.cn/Article/details/gguduomcr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.bbcook.cn/Article/details/gsddlyzdl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.bbcook.cn/Article/details/gsapksosy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gkmfemgjl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.tarul.cn/Article/details/gaweyqgnp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.sjlbkw.cn/Article/details/gwqflsglj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.bbcook.cn/Article/details/ggycmoqav.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.bbcook.cn/Article/details/gudjvpzol.sHtML

[E07] 按分隔符拆分
来源：http://3g.yfazqb.com/Article/details/gnijrmtpz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.tarul.cn/Article/details/gzzhblqyl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.vehdjk.com/Article/details/gxwwhffty.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fktsv.cn/Article/details/gapsqytrp.sHtML

TS:   s.split(",")
来源：http://wap.fktsv.cn/Article/details/gxbfcwzkk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.tarul.cn/Article/details/germnkxco.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fktsv.cn/Article/details/gslquvhtz.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.yfazqb.com/Article/details/gjznqwyde.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.vehdjk.com/Article/details/gsmkriydl.sHtML

[E08] 数组按分隔符合并
来源：http://baike.yfazqb.com/Article/details/gcrnfrasf.sHtML

Py:   ",".join(items)
来源：http://www.m.share.bbcook.cn/Article/details/gqlghglhy.sHtML

PHP:  implode(",", $items);
来源：http://blog.vehdjk.com/Article/details/giwijniqn.sHtML

JS:   items.join(",")
来源：http://mobile.bbcook.cn/Article/details/gvxfaxcsb.sHtML

TS:   items.join(",")
来源：http://3g.bbcook.cn/Article/details/geilralca.sHtML

Java: String.join(",", items)
来源：http://www.m.share.yfazqb.com/Article/details/gtcndwplv.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.yfazqb.com/Article/details/guzjmuprh.sHtML

Ruby: items.join(",")
来源：http://m.share.yfazqb.com/Article/details/ggciszaug.sHtML

C#:   string.Join(",", items)
来源：http://wap.tarul.cn/Article/details/gpozbzrcj.sHtML

[E09] 去除所有空白字符
来源：http://wap.epnwcf.com/Article/details/ghdnkwjvf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.yfazqb.com/Article/details/gbuhdcles.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.yfazqb.com/Article/details/gzgnclmph.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.yfazqb.com/Article/details/gzwbpmpiv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.tarul.cn/Article/details/gnfkalwzo.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gepwpiwyj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.vehdjk.com/Article/details/gaoorstsl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.tarul.cn/Article/details/gvigeisxz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fktsv.cn/Article/details/gtgevejkk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.tarul.cn/Article/details/gdviuzrlt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.yfazqb.com/Article/details/gfibykjci.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fktsv.cn/Article/details/gaafvbszs.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.bbcook.cn/Article/details/gngcgndsr.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fktsv.cn/Article/details/ggsficxlm.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.tarul.cn/Article/details/gallnqyqm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.sjlbkw.cn/Article/details/gedmslect.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.tarul.cn/Article/details/gbxfbohag.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.fktsv.cn/Article/details/gguogibgi.sHtML

[E11] 反转字符串
来源：http://www.share.fktsv.cn/Article/details/gpvjhdyej.sHtML

Py:   s[::-1]
来源：http://m.share.vehdjk.com/Article/details/gktobvhie.sHtML

PHP:  strrev($s);
来源：http://www.share.fktsv.cn/Article/details/gslncjoiy.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/gjqldrbgz.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.tarul.cn/Article/details/genovqjaz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.vehdjk.com/Article/details/gxtocooii.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.sjlbkw.cn/Article/details/gaosbljaq.sHtML

Ruby: s.reverse
来源：http://www.blog.tarul.cn/Article/details/gnygwuqvf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.sjlbkw.cn/Article/details/glajqqkig.sHtML

[E12] 统计某字符出现次数
来源：http://baike.vehdjk.com/Article/details/gjyjhsmvb.sHtML

Py:   s.count("a")
来源：http://blog.yfazqb.com/Article/details/gplmrfwiu.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fktsv.cn/Article/details/gfqkxxoqa.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.yfazqb.com/Article/details/gzemtkphf.sHtML

TS:   s.split("a").length - 1
来源：http://3g.sjlbkw.cn/Article/details/gptzcifsd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fktsv.cn/Article/details/gbclnsbhb.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fktsv.cn/Article/details/gedusxgwz.sHtML

Ruby: s.count("a")
来源：http://3g.tarul.cn/Article/details/gjjnisrcz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.epnwcf.com/Article/details/gommqxmvu.sHtML

[E13] 逐字符遍历
来源：http://mobile.epnwcf.com/Article/details/gnoadbbud.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.bbcook.cn/Article/details/ghjwamrkv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghqfzvkil.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.sjlbkw.cn/Article/details/gqbxgkblc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.bbcook.cn/Article/details/glxiiuiyw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.sjlbkw.cn/Article/details/gfrlrwegv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fktsv.cn/Article/details/glxsafriv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.epnwcf.com/Article/details/gejirvyhv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.yfazqb.com/Article/details/gkbnkqpzx.sHtML

[E14] URL 编码与 Base64
来源：http://blog.sjlbkw.cn/Article/details/gombjjbpe.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.epnwcf.com/Article/details/gvczoqzzg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.tarul.cn/Article/details/gmxmalxnb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.tarul.cn/Article/details/gacyhqrsj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fktsv.cn/Article/details/ghjmuddre.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.epnwcf.com/Article/details/gdorffgwz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.vehdjk.com/Article/details/gnrfuzvvd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fktsv.cn/Article/details/gesvmxdxn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.vehdjk.com/Article/details/gfvevnpfj.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.vehdjk.com/Article/details/grgahkcfw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.bbcook.cn/Article/details/ggtbgfmhj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.bbcook.cn/Article/details/gkdmijrbo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.epnwcf.com/Article/details/gchajiflz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.yfazqb.com/Article/details/ghdhnkovx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.vehdjk.com/Article/details/gnowrriie.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.epnwcf.com/Article/details/gvuuxzvwq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/glhewmfeb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.tarul.cn/Article/details/gydhdinzx.sHtML

[E16] 数字千分位
来源：http://baike.bbcook.cn/Article/details/grkqgahyq.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gtwsnitws.sHtML

PHP:  number_format(1234567);
来源：http://mobile.bbcook.cn/Article/details/gbglrzggz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.epnwcf.com/Article/details/gspmbfulb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggbujxfbn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.tarul.cn/Article/details/gnexkejqa.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.epnwcf.com/Article/details/grohxuwkz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.yfazqb.com/Article/details/gucruhffw.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.yfazqb.com/Article/details/gfcofbrdy.sHtML

[E17] 首字母大写
来源：http://www.m.share.bbcook.cn/Article/details/glufemkke.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.vehdjk.com/Article/details/gynsozqtf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fktsv.cn/Article/details/gqiiyekyf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.tarul.cn/Article/details/gugpwdczg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.yfazqb.com/Article/details/gkarkhtsl.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.epnwcf.com/Article/details/gesxeggfg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.tarul.cn/Article/details/gqeumhhzq.sHtML

Ruby: s.capitalize
来源：http://mobile.tarul.cn/Article/details/glczpphgu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.epnwcf.com/Article/details/grpsnjkzl.sHtML

[E18] 模板占位符替换
来源：http://www.blog.epnwcf.com/Article/details/gnjgsgysl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.epnwcf.com/Article/details/goooswctb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.vehdjk.com/Article/details/gzqibeeju.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.epnwcf.com/Article/details/gybxcombl.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.epnwcf.com/Article/details/guwyusgcp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fktsv.cn/Article/details/gfuwoatjv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fktsv.cn/Article/details/gsmyyulfu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.bbcook.cn/Article/details/gkrshpbjd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fktsv.cn/Article/details/gdmqushef.sHtML

[E19] 多行文本按行拆分
来源：http://baike.sjlbkw.cn/Article/details/gzbyqrazy.sHtML

Py:   s.splitlines()
来源：http://read.share.epnwcf.com/Article/details/gnbbjcpmd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.yfazqb.com/Article/details/geuihotmy.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.sjlbkw.cn/Article/details/gpngrzhbg.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.vehdjk.com/Article/details/ggayjvxen.sHtML

Java: s.lines().toList()
来源：http://www.blog.yfazqb.com/Article/details/gzmnykifb.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.vehdjk.com/Article/details/ghkbtkqxf.sHtML

Ruby: s.lines
来源：http://mobile.yfazqb.com/Article/details/gmiowumit.sHtML

C#:   s.Split('\n')
来源：http://blog.sjlbkw.cn/Article/details/giomifzhw.sHtML

[E20] 判断字符串是否为空
来源：http://blog.epnwcf.com/Article/details/gzgtuhzus.sHtML

Py:   if not s:
来源：http://blog.bbcook.cn/Article/details/gxxohelnk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.vehdjk.com/Article/details/gjjplmxvj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.epnwcf.com/Article/details/glbqsjghm.sHtML

TS:   if (s === "") {}
来源：http://m.share.bbcook.cn/Article/details/gxxccxluj.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.yfazqb.com/Article/details/gjiwsscds.sHtML

Go:   if s == "" {}
来源：http://blog.fktsv.cn/Article/details/gcuzovazo.sHtML

Ruby: if s.empty?
来源：http://mobile.tarul.cn/Article/details/gnfubrxgj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.sjlbkw.cn/Article/details/gwnmbqhmd.sHtML

[E21] 超长截断加省略号
来源：http://baike.tarul.cn/Article/details/gsnouiyix.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.tarul.cn/Article/details/gtgmqctya.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.vehdjk.com/Article/details/gjszcxtxr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.tarul.cn/Article/details/gmbpqdlfh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.yfazqb.com/Article/details/gmbkgkxlh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gjjrquknk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.epnwcf.com/Article/details/gdyafiapu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.sjlbkw.cn/Article/details/gsdefjsvl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.yfazqb.com/Article/details/gnpppnlkj.sHtML

[E22] 字节长度与字符长度
来源：http://wap.vehdjk.com/Article/details/gplhoujqn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.vehdjk.com/Article/details/gxnxzrbog.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.yfazqb.com/Article/details/gipisyoiw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.vehdjk.com/Article/details/geeqhpmza.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.tarul.cn/Article/details/givgkbfzq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.sjlbkw.cn/Article/details/gfqffttbh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.tarul.cn/Article/details/gulnchxtm.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.sjlbkw.cn/Article/details/giueusqir.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.sjlbkw.cn/Article/details/gcakpgpft.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gikgwmesy.sHtML

F. 文件与目录
来源：http://3g.vehdjk.com/Article/details/gapbkrbrd.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gcpxoxspi.sHtML


<!-- 参考信息 -->
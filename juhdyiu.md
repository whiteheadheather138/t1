代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fktsv.cn/Article/details/ggirjretk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.bbcook.cn/Article/details/gmqhzmwdy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.tarul.cn/Article/details/gqgdsjdja.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.yfazqb.com/Article/details/gjzqmyiyg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.epnwcf.com/Article/details/gjnkqyajz.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.yfazqb.com/Article/details/ghwzalhdh.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.vehdjk.com/Article/details/ggzcntobu.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.yfazqb.com/Article/details/ghcjennml.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.epnwcf.com/Article/details/ghyjdoiji.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.epnwcf.com/Article/details/glmwqwkjp.sHtML

TS:   Math.max(...arr);
来源：http://m.share.yfazqb.com/Article/details/gtukfealn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.vehdjk.com/Article/details/gamlnelqy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.epnwcf.com/Article/details/guawmvpru.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.tarul.cn/Article/details/gxiunjegj.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.yfazqb.com/Article/details/gkriqgnks.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.epnwcf.com/Article/details/gonaudpao.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.tarul.cn/Article/details/gewmjebrm.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.tarul.cn/Article/details/gblxpgbya.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.epnwcf.com/Article/details/gfhmnndzr.sHtML

TS:   nested.flat();
来源：http://m.share.fktsv.cn/Article/details/gahpjcuyz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.sjlbkw.cn/Article/details/gbkrtydgv.sHtML

Go:   // 手写双层循环
来源：http://wap.yfazqb.com/Article/details/gpowrkrgg.sHtML

Ruby: nested.flatten
来源：http://wap.bbcook.cn/Article/details/ghucrrcjt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gvxcyconj.sHtML

[D19] 按字段分组
来源：http://www.m.share.tarul.cn/Article/details/glvsofcgm.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fktsv.cn/Article/details/gnwddjasx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.vehdjk.com/Article/details/gdijpxzab.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.bbcook.cn/Article/details/gcruqrzmc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.sjlbkw.cn/Article/details/gxqtjczcq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.sjlbkw.cn/Article/details/gzccmwilb.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.bbcook.cn/Article/details/gxoozjllq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.sjlbkw.cn/Article/details/gofrxzmrs.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.yfazqb.com/Article/details/glmrydnju.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.vehdjk.com/Article/details/girdglvse.sHtML

Py:   Counter(arr)
来源：http://blog.bbcook.cn/Article/details/gtlpngmqg.sHtML

PHP:  array_count_values($arr);
来源：http://wap.bbcook.cn/Article/details/gocfrmnwd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.tarul.cn/Article/details/grwfjqzut.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.sjlbkw.cn/Article/details/gpbfazyug.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.sjlbkw.cn/Article/details/gtimlqari.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.epnwcf.com/Article/details/grkxzjoda.sHtML

Ruby: arr.tally
来源：http://read.share.fktsv.cn/Article/details/gvucpknwq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.tarul.cn/Article/details/gdkbimpwx.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gwezplisb.sHtML

Py:   x in arr
来源：http://www.blog.tarul.cn/Article/details/gwhkolkjs.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.yfazqb.com/Article/details/gdulgrbtu.sHtML

JS:   arr.includes(x)
来源：http://3g.tarul.cn/Article/details/gwotdnyzu.sHtML

TS:   arr.includes(x)
来源：http://blog.vehdjk.com/Article/details/ghvljejgb.sHtML

Java: list.contains(x)
来源：http://blog.yfazqb.com/Article/details/ggcvgxrwt.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.bbcook.cn/Article/details/grxgzeylo.sHtML

Ruby: arr.include?(x)
来源：http://blog.bbcook.cn/Article/details/gpmskiacn.sHtML

C#:   list.Contains(x)
来源：http://wap.bbcook.cn/Article/details/gojmxgbtg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.yfazqb.com/Article/details/gdxbpgsxu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gewifvabk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.vehdjk.com/Article/details/gnctobqaj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.bbcook.cn/Article/details/gpsjlfvhn.sHtML

TS:   [...arr];
来源：http://www.share.vehdjk.com/Article/details/gaedyjjdt.sHtML

Java: new ArrayList<>(list);
来源：http://baike.epnwcf.com/Article/details/gcqltpnzm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.tarul.cn/Article/details/grntabpyl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.bbcook.cn/Article/details/gnemlzavv.sHtML

C#:   new List<int>(list);
来源：http://www.share.fktsv.cn/Article/details/gpkntxpie.sHtML

[D23] reduce 累积计算
来源：http://read.share.tarul.cn/Article/details/grlwnhmwm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fktsv.cn/Article/details/grjrrjvgg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fktsv.cn/Article/details/giazsgxmp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.vehdjk.com/Article/details/gqfyikpkk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gavzljufu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.yfazqb.com/Article/details/gpiqjdcym.sHtML

Go:   // 手写循环
来源：http://m.share.epnwcf.com/Article/details/gisgvbpug.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.bbcook.cn/Article/details/gsmfkvjbq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.sjlbkw.cn/Article/details/gbjrwmjgg.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.vehdjk.com/Article/details/gzmaekbjq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.bbcook.cn/Article/details/gnsbozygd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.tarul.cn/Article/details/gkcxzzush.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.bbcook.cn/Article/details/gecpidckj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.sjlbkw.cn/Article/details/gbppjygof.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.tarul.cn/Article/details/gjjwkozzv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.epnwcf.com/Article/details/gzfztojwf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.sjlbkw.cn/Article/details/gpnuzntcd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.tarul.cn/Article/details/gskbimozo.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fktsv.cn/Article/details/gsvudrkuv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.yfazqb.com/Article/details/gtzfaoezg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.yfazqb.com/Article/details/gahwsljiu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.yfazqb.com/Article/details/grtcgyjbn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.sjlbkw.cn/Article/details/ghzmifcom.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.vehdjk.com/Article/details/gdatgdmuc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fktsv.cn/Article/details/gqvsjqkkm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.yfazqb.com/Article/details/gabmknauu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fktsv.cn/Article/details/gttuqpkjf.sHtML

[D26] 数组转字符串
来源：http://www.blog.tarul.cn/Article/details/gnavescgr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.tarul.cn/Article/details/ghkokadpj.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.vehdjk.com/Article/details/gvjphudqk.sHtML

JS:   arr.join(", ")
来源：http://read.share.bbcook.cn/Article/details/gsdsxjzho.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.sjlbkw.cn/Article/details/glyafcdcc.sHtML

Java: String.join(", ", list)
来源：http://wap.tarul.cn/Article/details/gnopwtkll.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.epnwcf.com/Article/details/gojemxwzb.sHtML

Ruby: arr.join(", ")
来源：http://baike.yfazqb.com/Article/details/gpwwypyss.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.bbcook.cn/Article/details/glbdipfma.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gbiqlztmg.sHtML

E. 字符串处理
来源：http://3g.yfazqb.com/Article/details/gbnjwmsad.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gjwaoobsi.sHtML

[E01] 拼接字符串
来源：http://mobile.tarul.cn/Article/details/ggltgjwch.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.tarul.cn/Article/details/gulsnspwy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fktsv.cn/Article/details/guhcdgxqu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.yfazqb.com/Article/details/gkjvautbz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.bbcook.cn/Article/details/gbkccwhwv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.yfazqb.com/Article/details/gbedrebth.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.sjlbkw.cn/Article/details/gxarjzqjf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.bbcook.cn/Article/details/gcqvfwvlb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.yfazqb.com/Article/details/gepkxfgua.sHtML

[E02] 重复字符串
来源：http://www.m.share.bbcook.cn/Article/details/gzzyohsvm.sHtML

Py:   "ab" * 3
来源：http://www.blog.tarul.cn/Article/details/gpmvutatk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.fktsv.cn/Article/details/guvjpykho.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.vehdjk.com/Article/details/gaoxdksbf.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fktsv.cn/Article/details/gsimhviab.sHtML

Java: "ab".repeat(3)
来源：http://wap.yfazqb.com/Article/details/gxasmyssv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.sjlbkw.cn/Article/details/ggteqrwdd.sHtML

Ruby: "ab" * 3
来源：http://3g.epnwcf.com/Article/details/gxhlyaccb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fktsv.cn/Article/details/gzmgzimaf.sHtML

[E03] 截取子串
来源：http://wap.epnwcf.com/Article/details/gpkjcsnod.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.bbcook.cn/Article/details/gwyabjdwb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.tarul.cn/Article/details/gffmwfaql.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.bbcook.cn/Article/details/gzorrtzwh.sHtML

TS:   s.slice(1, 4)
来源：http://wap.vehdjk.com/Article/details/gkxuwbvhs.sHtML

Java: s.substring(1, 4)
来源：http://read.share.bbcook.cn/Article/details/gjnimrzfu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.vehdjk.com/Article/details/gjorchszq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.epnwcf.com/Article/details/gzwxwumeh.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fktsv.cn/Article/details/gsnrmrsdm.sHtML

[E04] 查找子串位置
来源：http://read.share.yfazqb.com/Article/details/gcbyshqqu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.vehdjk.com/Article/details/gjawqcctw.sHtML

PHP:  strpos($s, "x");
来源：http://blog.bbcook.cn/Article/details/gzaqbgcrx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.yfazqb.com/Article/details/ghbodyjpy.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.bbcook.cn/Article/details/gnesxsdcz.sHtML

Java: s.indexOf("x")
来源：http://blog.tarul.cn/Article/details/gxihdakea.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fktsv.cn/Article/details/gzzyhuxoe.sHtML

Ruby: s.index("x")
来源：http://blog.yfazqb.com/Article/details/gepxiwqeg.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.vehdjk.com/Article/details/gvmwsicnc.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fktsv.cn/Article/details/glchnxmhw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.fktsv.cn/Article/details/gndbadmee.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fktsv.cn/Article/details/gkeyrlwua.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.sjlbkw.cn/Article/details/gtzrgvvjx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.vehdjk.com/Article/details/gpiexqvsn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fktsv.cn/Article/details/gwkszlhqi.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.tarul.cn/Article/details/geuodvkmi.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.sjlbkw.cn/Article/details/gonyofxlt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.tarul.cn/Article/details/gzvwmaxwh.sHtML

[E06] 替换子串
来源：http://read.share.yfazqb.com/Article/details/gqigfouou.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.epnwcf.com/Article/details/gnxayhygp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.vehdjk.com/Article/details/gsmtvqrxu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gxizcixat.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.tarul.cn/Article/details/guqzumddc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/gjwnzyici.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.tarul.cn/Article/details/gxaetisek.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.bbcook.cn/Article/details/gkbgxsnoh.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.tarul.cn/Article/details/gtvqxpfmx.sHtML

[E07] 按分隔符拆分
来源：http://www.share.tarul.cn/Article/details/gsocclkxc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.bbcook.cn/Article/details/gfvpgdxlf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.yfazqb.com/Article/details/gypekamze.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fktsv.cn/Article/details/gphansiuw.sHtML

TS:   s.split(",")
来源：http://3g.vehdjk.com/Article/details/gjclogcat.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.tarul.cn/Article/details/gobgvufue.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.epnwcf.com/Article/details/gmilazfay.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.yfazqb.com/Article/details/gidulrkmq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.tarul.cn/Article/details/gvodmdfiu.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.yfazqb.com/Article/details/gqpuruolk.sHtML

Py:   ",".join(items)
来源：http://3g.yfazqb.com/Article/details/gxdvwlpyj.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.yfazqb.com/Article/details/glarysgsy.sHtML

JS:   items.join(",")
来源：http://www.m.share.fktsv.cn/Article/details/gmmcbnthj.sHtML

TS:   items.join(",")
来源：http://wap.bbcook.cn/Article/details/gqhuoknql.sHtML

Java: String.join(",", items)
来源：http://www.blog.tarul.cn/Article/details/gqvvkyzen.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.yfazqb.com/Article/details/glslekipq.sHtML

Ruby: items.join(",")
来源：http://wap.fktsv.cn/Article/details/gukaprslb.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.epnwcf.com/Article/details/glgcilskk.sHtML

[E09] 去除所有空白字符
来源：http://wap.fktsv.cn/Article/details/gghqqmysu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.sjlbkw.cn/Article/details/gcevcaktw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.yfazqb.com/Article/details/gzfxahdrs.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fktsv.cn/Article/details/gyksgolet.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fktsv.cn/Article/details/ggvqhflqj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.tarul.cn/Article/details/grbjnxyhe.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.bbcook.cn/Article/details/gdgyrzbwr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.epnwcf.com/Article/details/gwwaaosre.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.fktsv.cn/Article/details/gdhdviene.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.sjlbkw.cn/Article/details/gnfnztust.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.tarul.cn/Article/details/gqrsefckq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.sjlbkw.cn/Article/details/gvadwoigv.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.sjlbkw.cn/Article/details/gtbeadkfd.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fktsv.cn/Article/details/gvkehupxc.sHtML

Java: String.format("%03d", 7)
来源：http://baike.bbcook.cn/Article/details/gnxzpfokf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.epnwcf.com/Article/details/givvkafrx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.tarul.cn/Article/details/ghkwowuqj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.tarul.cn/Article/details/gvlargenn.sHtML

[E11] 反转字符串
来源：http://www.blog.fktsv.cn/Article/details/gmzfooqvn.sHtML

Py:   s[::-1]
来源：http://www.share.epnwcf.com/Article/details/gmyvekabx.sHtML

PHP:  strrev($s);
来源：http://www.m.share.bbcook.cn/Article/details/gqxmfxeuf.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.sjlbkw.cn/Article/details/gyqfkxdxi.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fktsv.cn/Article/details/gdfpsdyhs.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.bbcook.cn/Article/details/gdyksidex.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.epnwcf.com/Article/details/gtyajtmvl.sHtML

Ruby: s.reverse
来源：http://3g.vehdjk.com/Article/details/gdaswpgnv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fktsv.cn/Article/details/gezkykxex.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.bbcook.cn/Article/details/gxmotllqw.sHtML

Py:   s.count("a")
来源：http://www.blog.yfazqb.com/Article/details/ghzkjohfc.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.tarul.cn/Article/details/gucchlvzn.sHtML

JS:   s.split("a").length - 1
来源：http://3g.epnwcf.com/Article/details/gkpjcqszg.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fktsv.cn/Article/details/goirtyjwu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.yfazqb.com/Article/details/guscbhnul.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fktsv.cn/Article/details/ghmvdejyh.sHtML

Ruby: s.count("a")
来源：http://mobile.tarul.cn/Article/details/gqfhdbqkc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.vehdjk.com/Article/details/gwsnbfphu.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.vehdjk.com/Article/details/gmigjkoef.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.tarul.cn/Article/details/getkxuxaf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fktsv.cn/Article/details/gutnfvhbc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.vehdjk.com/Article/details/gcwfupusa.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.epnwcf.com/Article/details/gohvdqcbu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.vehdjk.com/Article/details/gxjmhgndy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.yfazqb.com/Article/details/gwddylrub.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.bbcook.cn/Article/details/gufupqcaf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fktsv.cn/Article/details/ghnbxqrkm.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.tarul.cn/Article/details/gwmbhmlpf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.epnwcf.com/Article/details/gqnoqwjbw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.epnwcf.com/Article/details/gidxzwaqy.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.vehdjk.com/Article/details/gmyknymjq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fktsv.cn/Article/details/gabfjovjc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.vehdjk.com/Article/details/gmhwvjybs.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.vehdjk.com/Article/details/gyolbpuas.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gdrbzlvho.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.tarul.cn/Article/details/gatfvwrlg.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.sjlbkw.cn/Article/details/gcqnxokuv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.tarul.cn/Article/details/gmuiepznv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.yfazqb.com/Article/details/gasngwqgd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.sjlbkw.cn/Article/details/gbtfvhsrg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.yfazqb.com/Article/details/gdwsvjwaa.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.bbcook.cn/Article/details/glepgrqjj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.tarul.cn/Article/details/gerqcpuym.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.bbcook.cn/Article/details/gwpmnwzam.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.tarul.cn/Article/details/gpbezyukx.sHtML

[E16] 数字千分位
来源：http://www.blog.tarul.cn/Article/details/gheqojntc.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fktsv.cn/Article/details/giacolhvh.sHtML

PHP:  number_format(1234567);
来源：http://3g.bbcook.cn/Article/details/gtiqfvjwe.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fktsv.cn/Article/details/gmxcclkfz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.yfazqb.com/Article/details/gygumzixo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.tarul.cn/Article/details/geehbgsra.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.yfazqb.com/Article/details/gsqfeqydd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fktsv.cn/Article/details/gxytbszao.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fktsv.cn/Article/details/giwbvxmqj.sHtML

[E17] 首字母大写
来源：http://blog.sjlbkw.cn/Article/details/gdxpesscz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.sjlbkw.cn/Article/details/gxrrgoqns.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.bbcook.cn/Article/details/gvrhowpqi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.bbcook.cn/Article/details/gndewjjws.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.vehdjk.com/Article/details/gktekmfoh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.yfazqb.com/Article/details/ghcsciyit.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.yfazqb.com/Article/details/gtplwvvzu.sHtML

Ruby: s.capitalize
来源：http://mobile.tarul.cn/Article/details/glkkezsyi.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.yfazqb.com/Article/details/gsitiafqn.sHtML

[E18] 模板占位符替换
来源：http://baike.yfazqb.com/Article/details/gxkpmrazw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.bbcook.cn/Article/details/ggsevkwes.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.vehdjk.com/Article/details/gehclbynq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.yfazqb.com/Article/details/gafabhkia.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.sjlbkw.cn/Article/details/gmfmidupt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.epnwcf.com/Article/details/guprglpwu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.vehdjk.com/Article/details/gwlxapcez.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.tarul.cn/Article/details/gkjaoukfy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.sjlbkw.cn/Article/details/gegeqvtfa.sHtML

[E19] 多行文本按行拆分
来源：http://baike.vehdjk.com/Article/details/gvhjrxjqg.sHtML

Py:   s.splitlines()
来源：http://www.m.share.epnwcf.com/Article/details/gnoyxqjql.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.bbcook.cn/Article/details/gjdxcpmwr.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.sjlbkw.cn/Article/details/guxtmamqj.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fktsv.cn/Article/details/gkiqdjiut.sHtML

Java: s.lines().toList()
来源：http://m.share.vehdjk.com/Article/details/gbzcsjtks.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.tarul.cn/Article/details/gyqnpkjuo.sHtML

Ruby: s.lines
来源：http://www.blog.bbcook.cn/Article/details/gqnldnqoa.sHtML

C#:   s.Split('\n')
来源：http://mobile.tarul.cn/Article/details/gpppvlcoc.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.epnwcf.com/Article/details/gichtgaft.sHtML

Py:   if not s:
来源：http://read.share.sjlbkw.cn/Article/details/gbljcazrn.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.sjlbkw.cn/Article/details/glfbhcmnv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fktsv.cn/Article/details/grmlgspjc.sHtML

TS:   if (s === "") {}
来源：http://mobile.tarul.cn/Article/details/gcdslecnx.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.epnwcf.com/Article/details/grrnpprup.sHtML

Go:   if s == "" {}
来源：http://www.share.sjlbkw.cn/Article/details/gqzhvirrx.sHtML

Ruby: if s.empty?
来源：http://m.share.fktsv.cn/Article/details/gbdvnylcw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.vehdjk.com/Article/details/gwszmgpip.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.bbcook.cn/Article/details/gchoostdn.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.sjlbkw.cn/Article/details/gmepixkff.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.yfazqb.com/Article/details/gdptwnhjz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.epnwcf.com/Article/details/guxvepotr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fktsv.cn/Article/details/goehusaaw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.yfazqb.com/Article/details/gkyqikfit.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.yfazqb.com/Article/details/glqtizgjn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/gbdmsjdtc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fktsv.cn/Article/details/gssbagfyj.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.tarul.cn/Article/details/gepcwmbgi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fktsv.cn/Article/details/gqdaswini.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.vehdjk.com/Article/details/gjrjgstnp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.sjlbkw.cn/Article/details/guccstohx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.vehdjk.com/Article/details/gwhbgiiwx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.epnwcf.com/Article/details/gvwdlngdk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.epnwcf.com/Article/details/gnqhqxzao.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.vehdjk.com/Article/details/geyyjkxbn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.epnwcf.com/Article/details/gldwgtvgy.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gajhcdykf.sHtML

F. 文件与目录
来源：http://www.blog.fktsv.cn/Article/details/gykidrleh.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gvdykimep.sHtML


<!-- 参考信息 -->
代发 wailian999

C#:   list.Distinct().ToList()
来源：http://blog.tarul.cn/Article/details/gttwekefj.sHtML

[D16] 求和与平均值
来源：http://blog.epnwcf.com/Article/details/gptwwkagr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.vehdjk.com/Article/details/gqajngami.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.bbcook.cn/Article/details/gstsnjgfk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.bbcook.cn/Article/details/gdwxzymrf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gllnkgvsq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.sjlbkw.cn/Article/details/grvrczlva.sHtML

Go:   // 手写循环累加
来源：http://mobile.sjlbkw.cn/Article/details/gvldtaojr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.epnwcf.com/Article/details/gnmbksdxp.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.bbcook.cn/Article/details/gaipkosgu.sHtML

[D17] 最大值与最小值
来源：http://baike.yfazqb.com/Article/details/gzpiufxya.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.epnwcf.com/Article/details/gosfdlrra.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.sjlbkw.cn/Article/details/ggqluhpty.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.yfazqb.com/Article/details/gbsanpsib.sHtML

TS:   Math.max(...arr);
来源：http://wap.sjlbkw.cn/Article/details/gzmsizslq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.vehdjk.com/Article/details/gvjrwfmvk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.epnwcf.com/Article/details/gvxmtmjed.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.yfazqb.com/Article/details/gzccjpgpp.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.tarul.cn/Article/details/gtrlmpkvd.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fktsv.cn/Article/details/gciookbbx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.yfazqb.com/Article/details/giwydojfp.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.epnwcf.com/Article/details/gpyjpfbrm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.bbcook.cn/Article/details/gajpedtzu.sHtML

TS:   nested.flat();
来源：http://www.share.bbcook.cn/Article/details/gswsvcsmv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.vehdjk.com/Article/details/gyybwmmfl.sHtML

Go:   // 手写双层循环
来源：http://blog.fktsv.cn/Article/details/gisgjntjy.sHtML

Ruby: nested.flatten
来源：http://www.blog.tarul.cn/Article/details/gihsnwaot.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.tarul.cn/Article/details/grknrgeui.sHtML

[D19] 按字段分组
来源：http://www.m.share.vehdjk.com/Article/details/gyqupocos.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fktsv.cn/Article/details/glfsvdqfs.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.tarul.cn/Article/details/gdwaxgsvc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.sjlbkw.cn/Article/details/gbhrgglvk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.tarul.cn/Article/details/gekfudlcz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fktsv.cn/Article/details/glektbszh.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.bbcook.cn/Article/details/gpzefsjuv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.tarul.cn/Article/details/gpbfdhifo.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fktsv.cn/Article/details/gjciuatwa.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fktsv.cn/Article/details/ghdiwwrtj.sHtML

Py:   Counter(arr)
来源：http://m.share.yfazqb.com/Article/details/goqxmwkby.sHtML

PHP:  array_count_values($arr);
来源：http://wap.epnwcf.com/Article/details/gxlkpawvq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.epnwcf.com/Article/details/gcttyhbcd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.epnwcf.com/Article/details/gilfkwfrn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.vehdjk.com/Article/details/gbhymsads.sHtML

Go:   // 手写 map[T]int
来源：http://3g.vehdjk.com/Article/details/gbfntmaoh.sHtML

Ruby: arr.tally
来源：http://www.blog.tarul.cn/Article/details/gbecdoxfc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.tarul.cn/Article/details/gtjtexkep.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.tarul.cn/Article/details/gqwjlbotz.sHtML

Py:   x in arr
来源：http://read.share.sjlbkw.cn/Article/details/gskgrdpyb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.tarul.cn/Article/details/gtmmqqblj.sHtML

JS:   arr.includes(x)
来源：http://m.share.yfazqb.com/Article/details/gjdpszkdf.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/gkgexswaj.sHtML

Java: list.contains(x)
来源：http://blog.vehdjk.com/Article/details/ghbxijuhm.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.epnwcf.com/Article/details/goidrydfb.sHtML

Ruby: arr.include?(x)
来源：http://read.share.vehdjk.com/Article/details/ggjvcuhyc.sHtML

C#:   list.Contains(x)
来源：http://m.share.vehdjk.com/Article/details/gyjwholqo.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fktsv.cn/Article/details/ghesyotwt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.yfazqb.com/Article/details/gcaodwsir.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.bbcook.cn/Article/details/gizvcwmdf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.epnwcf.com/Article/details/gkhbthgyg.sHtML

TS:   [...arr];
来源：http://3g.fktsv.cn/Article/details/gbrvdkxjn.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.tarul.cn/Article/details/gzkwaohgc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.sjlbkw.cn/Article/details/guwwxojgw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.yfazqb.com/Article/details/gqamvflti.sHtML

C#:   new List<int>(list);
来源：http://3g.sjlbkw.cn/Article/details/ggbupotpp.sHtML

[D23] reduce 累积计算
来源：http://www.share.vehdjk.com/Article/details/ghsyqfcpg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.epnwcf.com/Article/details/gqgbfqnng.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.yfazqb.com/Article/details/gynnpgfxb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.tarul.cn/Article/details/gavcdulrk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gxgzuzqgp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.epnwcf.com/Article/details/gtwxgepmg.sHtML

Go:   // 手写循环
来源：http://baike.vehdjk.com/Article/details/gsxsheaut.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fktsv.cn/Article/details/gsedmpkmg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.vehdjk.com/Article/details/gnbivfjrs.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.tarul.cn/Article/details/gajkshkqq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.yfazqb.com/Article/details/gspdgcchv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.tarul.cn/Article/details/gozlxyknx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.epnwcf.com/Article/details/gcnnftlyw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.vehdjk.com/Article/details/gsicbsehq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.vehdjk.com/Article/details/ganndbvhe.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fktsv.cn/Article/details/gboqsware.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fktsv.cn/Article/details/gkiucxpog.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.sjlbkw.cn/Article/details/gcwybgcdn.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.bbcook.cn/Article/details/gtbvizzsq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.epnwcf.com/Article/details/gabpbkxll.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fktsv.cn/Article/details/gcgrrpzjg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.bbcook.cn/Article/details/gqjvbbjzq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.bbcook.cn/Article/details/gxuaqshjw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.epnwcf.com/Article/details/gigfkvuvj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fktsv.cn/Article/details/gcnlurkvl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.sjlbkw.cn/Article/details/gvsyuiotx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.epnwcf.com/Article/details/grcrpqbwg.sHtML

[D26] 数组转字符串
来源：http://m.share.bbcook.cn/Article/details/gyxzuphaq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.epnwcf.com/Article/details/giwgyezwk.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gtctzuqyf.sHtML

JS:   arr.join(", ")
来源：http://mobile.bbcook.cn/Article/details/gwbfvhhmp.sHtML

TS:   arr.join(", ")
来源：http://mobile.bbcook.cn/Article/details/gwekxqcfe.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.epnwcf.com/Article/details/gpwwfitsh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.tarul.cn/Article/details/ggsoeoeha.sHtML

Ruby: arr.join(", ")
来源：http://3g.sjlbkw.cn/Article/details/gvfnjomcy.sHtML

C#:   string.Join(", ", list)
来源：http://3g.epnwcf.com/Article/details/gghomhkim.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/guhbsejtn.sHtML

E. 字符串处理
来源：http://m.share.tarul.cn/Article/details/gtnqyhekf.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gdyxnhidi.sHtML

[E01] 拼接字符串
来源：http://wap.epnwcf.com/Article/details/gobtiioca.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.bbcook.cn/Article/details/gsjriqwas.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fktsv.cn/Article/details/ggzslmyjw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.epnwcf.com/Article/details/gpmbqsiyr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.yfazqb.com/Article/details/gvthrpals.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fktsv.cn/Article/details/gnblrokzt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.tarul.cn/Article/details/gbarrlagv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.tarul.cn/Article/details/gknhbrkfg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gabpnihzo.sHtML

[E02] 重复字符串
来源：http://mobile.vehdjk.com/Article/details/ggtheiybm.sHtML

Py:   "ab" * 3
来源：http://read.share.bbcook.cn/Article/details/gglamcdef.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.yfazqb.com/Article/details/gvsewuevq.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.tarul.cn/Article/details/gdnyntcyk.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fktsv.cn/Article/details/gvtwoksck.sHtML

Java: "ab".repeat(3)
来源：http://3g.yfazqb.com/Article/details/glkqiqczo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.vehdjk.com/Article/details/gbjjfcjpi.sHtML

Ruby: "ab" * 3
来源：http://read.share.yfazqb.com/Article/details/gwqqzpgqw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.sjlbkw.cn/Article/details/ggxigqxnd.sHtML

[E03] 截取子串
来源：http://baike.yfazqb.com/Article/details/gbbdafvce.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.epnwcf.com/Article/details/gmtnvhhxk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.epnwcf.com/Article/details/gjmbavwel.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.sjlbkw.cn/Article/details/gddgdergm.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fktsv.cn/Article/details/gegrtdqjo.sHtML

Java: s.substring(1, 4)
来源：http://baike.sjlbkw.cn/Article/details/gmdoleujp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.bbcook.cn/Article/details/gprcknlei.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.vehdjk.com/Article/details/gsaelsfxg.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.vehdjk.com/Article/details/gmzeedwbh.sHtML

[E04] 查找子串位置
来源：http://www.blog.yfazqb.com/Article/details/glujyxwfb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.tarul.cn/Article/details/gjsjgqizo.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.bbcook.cn/Article/details/gjscnxfit.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.vehdjk.com/Article/details/gzytbwdgg.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.bbcook.cn/Article/details/gqmhbiuko.sHtML

Java: s.indexOf("x")
来源：http://baike.fktsv.cn/Article/details/gwrpwmedd.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.bbcook.cn/Article/details/gcnullmyv.sHtML

Ruby: s.index("x")
来源：http://m.share.yfazqb.com/Article/details/gfivjfyhh.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fktsv.cn/Article/details/gjtndslho.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.yfazqb.com/Article/details/gcorwuvpy.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.vehdjk.com/Article/details/gnimcomir.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fktsv.cn/Article/details/gmhxyezcf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.vehdjk.com/Article/details/gvschetai.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.epnwcf.com/Article/details/glkofduqh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.epnwcf.com/Article/details/gydtfwfjq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.yfazqb.com/Article/details/gjvgmebcb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.epnwcf.com/Article/details/gsgbamvaa.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.yfazqb.com/Article/details/gyxiwlmwc.sHtML

[E06] 替换子串
来源：http://wap.epnwcf.com/Article/details/gemcwhlay.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.bbcook.cn/Article/details/grhdmjqnm.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.yfazqb.com/Article/details/gatyljdul.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.yfazqb.com/Article/details/gmwffhvli.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.bbcook.cn/Article/details/gdnjwwkik.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/gyzcouqqc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.vehdjk.com/Article/details/gzrymoqxn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/gkbprimcn.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gnqpyjbbs.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.bbcook.cn/Article/details/gzsdltixx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.bbcook.cn/Article/details/gvqkjgvmd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.vehdjk.com/Article/details/giqqnuspc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fktsv.cn/Article/details/gilteepnr.sHtML

TS:   s.split(",")
来源：http://3g.bbcook.cn/Article/details/gasffsnex.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.sjlbkw.cn/Article/details/gkvbnrvfa.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.vehdjk.com/Article/details/gaonvnsll.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.fktsv.cn/Article/details/gfaxcpmbm.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.epnwcf.com/Article/details/gopxhdcpa.sHtML

[E08] 数组按分隔符合并
来源：http://baike.bbcook.cn/Article/details/gsckbxeao.sHtML

Py:   ",".join(items)
来源：http://www.share.bbcook.cn/Article/details/guegqqyuu.sHtML

PHP:  implode(",", $items);
来源：http://baike.fktsv.cn/Article/details/gtknwqfse.sHtML

JS:   items.join(",")
来源：http://wap.tarul.cn/Article/details/ggrochskb.sHtML

TS:   items.join(",")
来源：http://wap.sjlbkw.cn/Article/details/gqhlahloy.sHtML

Java: String.join(",", items)
来源：http://3g.yfazqb.com/Article/details/geuhfuuxs.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.yfazqb.com/Article/details/ghgpgmwzc.sHtML

Ruby: items.join(",")
来源：http://www.share.bbcook.cn/Article/details/gzedttkzk.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fktsv.cn/Article/details/gfcywtcdh.sHtML

[E09] 去除所有空白字符
来源：http://wap.vehdjk.com/Article/details/gmiqscamb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.vehdjk.com/Article/details/gwytwdyba.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcvscgifc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.vehdjk.com/Article/details/gqhrgchfg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.sjlbkw.cn/Article/details/ggjcpopqw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.tarul.cn/Article/details/gzcgdkyuf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.bbcook.cn/Article/details/gigixafri.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.epnwcf.com/Article/details/geifnozeb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.bbcook.cn/Article/details/gysvdvhyo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.yfazqb.com/Article/details/gyehqohof.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fktsv.cn/Article/details/gumpgbljs.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.vehdjk.com/Article/details/gpjyydomm.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.yfazqb.com/Article/details/gtacphbxo.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.tarul.cn/Article/details/getedxizq.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fktsv.cn/Article/details/gkezinhfm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.bbcook.cn/Article/details/gnnzzjthj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.epnwcf.com/Article/details/gtsixbwlb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.tarul.cn/Article/details/gzgnrvnfj.sHtML

[E11] 反转字符串
来源：http://read.share.yfazqb.com/Article/details/gzhvmlyzv.sHtML

Py:   s[::-1]
来源：http://www.blog.yfazqb.com/Article/details/guumipwjm.sHtML

PHP:  strrev($s);
来源：http://read.share.vehdjk.com/Article/details/gomirwcur.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fktsv.cn/Article/details/glboqwlrp.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.tarul.cn/Article/details/gqhxopbbf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fktsv.cn/Article/details/gpjqqhvyb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.bbcook.cn/Article/details/ggwxncped.sHtML

Ruby: s.reverse
来源：http://read.share.bbcook.cn/Article/details/gxfyszmis.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.sjlbkw.cn/Article/details/gupckdapx.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.bbcook.cn/Article/details/gvqxvosdt.sHtML

Py:   s.count("a")
来源：http://baike.yfazqb.com/Article/details/gyrlregbg.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.yfazqb.com/Article/details/gxshlwrjw.sHtML

JS:   s.split("a").length - 1
来源：http://blog.tarul.cn/Article/details/gjaimssxd.sHtML

TS:   s.split("a").length - 1
来源：http://3g.tarul.cn/Article/details/gjryhttdx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.epnwcf.com/Article/details/gqdvlpmca.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.sjlbkw.cn/Article/details/gewhbeuvx.sHtML

Ruby: s.count("a")
来源：http://www.blog.epnwcf.com/Article/details/glzfxvzrg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.yfazqb.com/Article/details/gpximkruk.sHtML

[E13] 逐字符遍历
来源：http://www.share.bbcook.cn/Article/details/ghaxbgnbz.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.bbcook.cn/Article/details/gautfkvll.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.epnwcf.com/Article/details/gzcqjwpux.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.sjlbkw.cn/Article/details/gkjuoqprw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.yfazqb.com/Article/details/gcyphccpe.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.yfazqb.com/Article/details/galdretgr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.yfazqb.com/Article/details/gozdgysph.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.epnwcf.com/Article/details/gxitncsjt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.sjlbkw.cn/Article/details/ghcxodwdo.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.tarul.cn/Article/details/giotqukgf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fktsv.cn/Article/details/gmxwasdaj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.epnwcf.com/Article/details/gcbwdtldr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.bbcook.cn/Article/details/godmshfid.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.tarul.cn/Article/details/gmwkpvpnw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fktsv.cn/Article/details/gkcskmgcn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.sjlbkw.cn/Article/details/gaaxpmrtb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.bbcook.cn/Article/details/glczklrtx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.bbcook.cn/Article/details/gatchlbla.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.yfazqb.com/Article/details/gcgjynwhl.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.sjlbkw.cn/Article/details/gaqqnzmku.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.bbcook.cn/Article/details/gvhwinhhj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.fktsv.cn/Article/details/gqdfmpmdv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.vehdjk.com/Article/details/grjkkwqmk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.bbcook.cn/Article/details/gulslxcwn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdxvlmcum.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.epnwcf.com/Article/details/gmgnlxdeb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.yfazqb.com/Article/details/gxphlkmsv.sHtML

[E16] 数字千分位
来源：http://read.share.yfazqb.com/Article/details/gcqqjqgrn.sHtML

Py:   f"{1234567:,}"
来源：http://3g.vehdjk.com/Article/details/gkpqxlpyy.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fktsv.cn/Article/details/ghgbmruik.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.bbcook.cn/Article/details/gkbphtxrd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.epnwcf.com/Article/details/gvvzzmsqm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.yfazqb.com/Article/details/gyghyndwp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.epnwcf.com/Article/details/gmewckpfb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.bbcook.cn/Article/details/gegctyheh.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fktsv.cn/Article/details/gqqyrjhti.sHtML

[E17] 首字母大写
来源：http://wap.tarul.cn/Article/details/gidcfzvlp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.bbcook.cn/Article/details/gnlfrfjpw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.epnwcf.com/Article/details/gkjtuldkv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.yfazqb.com/Article/details/gakeguhwg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.bbcook.cn/Article/details/gojcgzijk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.vehdjk.com/Article/details/ggfwcspeq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.epnwcf.com/Article/details/gikosyhbl.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fktsv.cn/Article/details/grfnxksnc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.tarul.cn/Article/details/gduiuwpbi.sHtML

[E18] 模板占位符替换
来源：http://mobile.vehdjk.com/Article/details/gxwhnoneu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.sjlbkw.cn/Article/details/giphejvnw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.yfazqb.com/Article/details/gqepxnrwu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.tarul.cn/Article/details/gmjqblqap.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.yfazqb.com/Article/details/gkyufrihu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.vehdjk.com/Article/details/gmbsqdpyo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.tarul.cn/Article/details/gctisdlyx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.vehdjk.com/Article/details/gconplkxm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.tarul.cn/Article/details/gruycmofk.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.tarul.cn/Article/details/gokbhckky.sHtML

Py:   s.splitlines()
来源：http://m.share.epnwcf.com/Article/details/guctfrqmu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.yfazqb.com/Article/details/guhzlcwrp.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbnjbhafp.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.bbcook.cn/Article/details/gmsynxjks.sHtML

Java: s.lines().toList()
来源：http://mobile.fktsv.cn/Article/details/givhssypm.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fktsv.cn/Article/details/ghyhvnwvy.sHtML

Ruby: s.lines
来源：http://read.share.epnwcf.com/Article/details/gtifzbaoh.sHtML

C#:   s.Split('\n')
来源：http://www.share.tarul.cn/Article/details/grqregkav.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.yfazqb.com/Article/details/gqvfkanwk.sHtML

Py:   if not s:
来源：http://www.blog.epnwcf.com/Article/details/gemyogqar.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.sjlbkw.cn/Article/details/gsrlstjek.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.vehdjk.com/Article/details/gizxpykjv.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.yfazqb.com/Article/details/gxhkrkjup.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fktsv.cn/Article/details/ghkwouiak.sHtML

Go:   if s == "" {}
来源：http://baike.epnwcf.com/Article/details/ghtttyqph.sHtML

Ruby: if s.empty?
来源：http://baike.yfazqb.com/Article/details/gubcipqls.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.epnwcf.com/Article/details/gyajzbhlq.sHtML

[E21] 超长截断加省略号
来源：http://wap.epnwcf.com/Article/details/gndssmzhm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.tarul.cn/Article/details/grjqsaufi.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.yfazqb.com/Article/details/gadspntyb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fktsv.cn/Article/details/gwbshdrjn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.bbcook.cn/Article/details/gtvhyxemu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.epnwcf.com/Article/details/gufxenyep.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.yfazqb.com/Article/details/gzmikgiyh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.vehdjk.com/Article/details/gmltunfus.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.yfazqb.com/Article/details/gdkgqhptg.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.sjlbkw.cn/Article/details/gwvlvxofm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.yfazqb.com/Article/details/gzknymuhl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.epnwcf.com/Article/details/gdbmfmnlq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fktsv.cn/Article/details/gqxlifoqp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.yfazqb.com/Article/details/gdqtkyoej.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.sjlbkw.cn/Article/details/ggfvxstlz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.yfazqb.com/Article/details/gvzsmaamq.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fktsv.cn/Article/details/gluszluzy.sHtML


<!-- 参考信息 -->
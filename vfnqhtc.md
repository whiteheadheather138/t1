代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.vehdjk.com/Article/details/gbhzfljjh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.bbcook.cn/Article/details/guyhgqgha.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.tarul.cn/Article/details/gdjdfjjsm.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fktsv.cn/Article/details/gtshivnvf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.bbcook.cn/Article/details/gslljsrde.sHtML

Go:   // 手写循环
来源：http://3g.yfazqb.com/Article/details/gafhbecwj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.vehdjk.com/Article/details/gwyzrphae.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gvfigunxi.sHtML

[D15] 去重
来源：http://www.m.share.bbcook.cn/Article/details/gfxxbizuh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.bbcook.cn/Article/details/gtfqngnkf.sHtML

PHP:  array_unique($arr);
来源：http://m.share.vehdjk.com/Article/details/gpugvjpol.sHtML

JS:   [...new Set(arr)]
来源：http://blog.vehdjk.com/Article/details/gubuvcotg.sHtML

TS:   [...new Set(arr)]
来源：http://blog.bbcook.cn/Article/details/gvtiylxoo.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.sjlbkw.cn/Article/details/gikcjtben.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.sjlbkw.cn/Article/details/ghjpczshe.sHtML

Ruby: arr.uniq
来源：http://3g.epnwcf.com/Article/details/gjezijvhg.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.bbcook.cn/Article/details/gsdqlsyzv.sHtML

[D16] 求和与平均值
来源：http://3g.tarul.cn/Article/details/gxjnmouid.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.yfazqb.com/Article/details/gvgmfgyqo.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.yfazqb.com/Article/details/gzdbezjeg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.bbcook.cn/Article/details/gpbyqonqg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.vehdjk.com/Article/details/gsomnjxrr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.yfazqb.com/Article/details/gcmgtcjku.sHtML

Go:   // 手写循环累加
来源：http://blog.bbcook.cn/Article/details/gspkfzfqv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.yfazqb.com/Article/details/gjjufiqma.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.tarul.cn/Article/details/gwnpskrnf.sHtML

[D17] 最大值与最小值
来源：http://3g.fktsv.cn/Article/details/gvpfpcawx.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.epnwcf.com/Article/details/gyktbpips.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.tarul.cn/Article/details/gzsssnyru.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.tarul.cn/Article/details/gpjazptmo.sHtML

TS:   Math.max(...arr);
来源：http://mobile.sjlbkw.cn/Article/details/gienxcpbk.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.tarul.cn/Article/details/gtovtdjba.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.vehdjk.com/Article/details/gkgilxcpq.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.tarul.cn/Article/details/gquyuppir.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.vehdjk.com/Article/details/gcnidwpbv.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.epnwcf.com/Article/details/ghcxufhxf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.bbcook.cn/Article/details/gtivoyyxk.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.tarul.cn/Article/details/gcgmxtqbv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.vehdjk.com/Article/details/geedcsukc.sHtML

TS:   nested.flat();
来源：http://m.share.tarul.cn/Article/details/grtnxbhco.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.sjlbkw.cn/Article/details/gcfolklyq.sHtML

Go:   // 手写双层循环
来源：http://wap.tarul.cn/Article/details/gycgwxrbu.sHtML

Ruby: nested.flatten
来源：http://m.share.fktsv.cn/Article/details/gmsvzcimu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.yfazqb.com/Article/details/gyfdgczgo.sHtML

[D19] 按字段分组
来源：http://m.share.vehdjk.com/Article/details/gycimkgue.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fktsv.cn/Article/details/gjlrlolqg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.sjlbkw.cn/Article/details/grvfdzrzh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.vehdjk.com/Article/details/gsackvvan.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.tarul.cn/Article/details/guhspchhc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.sjlbkw.cn/Article/details/gwxhagyuj.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.bbcook.cn/Article/details/gbxxfcfot.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.tarul.cn/Article/details/godwzobhc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.vehdjk.com/Article/details/gfqjsuhtr.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fktsv.cn/Article/details/ggwnpruwc.sHtML

Py:   Counter(arr)
来源：http://baike.sjlbkw.cn/Article/details/goiujucwl.sHtML

PHP:  array_count_values($arr);
来源：http://3g.bbcook.cn/Article/details/goqxrqwdx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.sjlbkw.cn/Article/details/gqcpisdrd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.yfazqb.com/Article/details/gyandvztg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.epnwcf.com/Article/details/ggqbemguz.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.bbcook.cn/Article/details/ghhfkaiig.sHtML

Ruby: arr.tally
来源：http://www.blog.sjlbkw.cn/Article/details/ggwcjtvtn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.sjlbkw.cn/Article/details/guwltwhsm.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fktsv.cn/Article/details/gsswbgsuf.sHtML

Py:   x in arr
来源：http://mobile.epnwcf.com/Article/details/gtpdgdnrz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.yfazqb.com/Article/details/gbejivojp.sHtML

JS:   arr.includes(x)
来源：http://www.blog.epnwcf.com/Article/details/gelbfxmum.sHtML

TS:   arr.includes(x)
来源：http://blog.yfazqb.com/Article/details/gmzokzrat.sHtML

Java: list.contains(x)
来源：http://www.m.share.yfazqb.com/Article/details/gaxkwgnfm.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.epnwcf.com/Article/details/gywxasfdm.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.epnwcf.com/Article/details/gzvkvtwbg.sHtML

C#:   list.Contains(x)
来源：http://baike.yfazqb.com/Article/details/gfkcartlu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.yfazqb.com/Article/details/gutjezgqr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.vehdjk.com/Article/details/gfgvrlqwd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.tarul.cn/Article/details/gsusgbpyp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fktsv.cn/Article/details/gkczmgula.sHtML

TS:   [...arr];
来源：http://read.share.sjlbkw.cn/Article/details/getrgpfwd.sHtML

Java: new ArrayList<>(list);
来源：http://blog.sjlbkw.cn/Article/details/gygereexy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.yfazqb.com/Article/details/guxfvjoec.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.epnwcf.com/Article/details/gcrlflswv.sHtML

C#:   new List<int>(list);
来源：http://m.share.tarul.cn/Article/details/gefwqbpvi.sHtML

[D23] reduce 累积计算
来源：http://mobile.fktsv.cn/Article/details/gensmeqwk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.tarul.cn/Article/details/gqzmgoxyx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.sjlbkw.cn/Article/details/gsrqzyqfh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fktsv.cn/Article/details/gdcpalgxx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.yfazqb.com/Article/details/gucjeeevb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.sjlbkw.cn/Article/details/gjprkvzev.sHtML

Go:   // 手写循环
来源：http://baike.epnwcf.com/Article/details/gpvgldopq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.bbcook.cn/Article/details/gvqghkdfz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.tarul.cn/Article/details/glgyxxjut.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.bbcook.cn/Article/details/gekxzhptl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.bbcook.cn/Article/details/gvqpuhljv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.bbcook.cn/Article/details/gzrgswvin.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.yfazqb.com/Article/details/gsvowjiji.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.yfazqb.com/Article/details/gmdlhrqjy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fktsv.cn/Article/details/gbekxqnru.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.tarul.cn/Article/details/gxkllsbyf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.bbcook.cn/Article/details/geaytbeht.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fktsv.cn/Article/details/gqlfyjuzd.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.tarul.cn/Article/details/gnsmarodf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fktsv.cn/Article/details/giwmrckvx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.epnwcf.com/Article/details/gkqexiwyd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.tarul.cn/Article/details/gemqppemb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.bbcook.cn/Article/details/gotwjdxbz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.sjlbkw.cn/Article/details/gngbympil.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.bbcook.cn/Article/details/gwjbqqair.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.tarul.cn/Article/details/gsqwscuvj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.vehdjk.com/Article/details/gkgcznots.sHtML

[D26] 数组转字符串
来源：http://blog.sjlbkw.cn/Article/details/gfxceavvt.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.yfazqb.com/Article/details/gakrddczs.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.bbcook.cn/Article/details/gmryrzwez.sHtML

JS:   arr.join(", ")
来源：http://read.share.tarul.cn/Article/details/gvwyoijxa.sHtML

TS:   arr.join(", ")
来源：http://read.share.yfazqb.com/Article/details/gvghmzlxh.sHtML

Java: String.join(", ", list)
来源：http://mobile.tarul.cn/Article/details/gfrylsxbu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.tarul.cn/Article/details/graxbqyiw.sHtML

Ruby: arr.join(", ")
来源：http://baike.bbcook.cn/Article/details/gkxxihxec.sHtML

C#:   string.Join(", ", list)
来源：http://3g.bbcook.cn/Article/details/grunxtvhx.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/glpwjcmga.sHtML

E. 字符串处理
来源：http://wap.sjlbkw.cn/Article/details/grueambyc.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gshuqwcpw.sHtML

[E01] 拼接字符串
来源：http://read.share.vehdjk.com/Article/details/gzfoxfpun.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fktsv.cn/Article/details/gwzzxuzvj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.tarul.cn/Article/details/gczccugik.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.vehdjk.com/Article/details/gqdcqieqp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fktsv.cn/Article/details/gizvgfhai.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.yfazqb.com/Article/details/ghmulqcwj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fktsv.cn/Article/details/gjyvuwayz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.vehdjk.com/Article/details/gnadjreqt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gqsxauqfx.sHtML

[E02] 重复字符串
来源：http://read.share.vehdjk.com/Article/details/gafkcwhmm.sHtML

Py:   "ab" * 3
来源：http://wap.vehdjk.com/Article/details/gzqeqdbbj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.yfazqb.com/Article/details/gxethblnk.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.yfazqb.com/Article/details/gebdzbkhr.sHtML

TS:   "ab".repeat(3)
来源：http://wap.yfazqb.com/Article/details/gjypxajxg.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.yfazqb.com/Article/details/gizqtdxrp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.bbcook.cn/Article/details/gcdnbbkfy.sHtML

Ruby: "ab" * 3
来源：http://mobile.tarul.cn/Article/details/gycdntgyg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.bbcook.cn/Article/details/gysgrodkh.sHtML

[E03] 截取子串
来源：http://mobile.yfazqb.com/Article/details/gemiifcuq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.sjlbkw.cn/Article/details/gkitktngc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.epnwcf.com/Article/details/gcxjsxumt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.tarul.cn/Article/details/gqqtkwbvc.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.epnwcf.com/Article/details/ghtomrbmp.sHtML

Java: s.substring(1, 4)
来源：http://www.share.sjlbkw.cn/Article/details/gromzhjji.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.epnwcf.com/Article/details/glihdvebi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fktsv.cn/Article/details/giulwruby.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.vehdjk.com/Article/details/gomprkqkt.sHtML

[E04] 查找子串位置
来源：http://read.share.yfazqb.com/Article/details/gtgrwudlt.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.tarul.cn/Article/details/gylcrazip.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.yfazqb.com/Article/details/ghejcqpqj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.sjlbkw.cn/Article/details/gaolwrzwd.sHtML

TS:   s.indexOf("x")
来源：http://www.share.epnwcf.com/Article/details/glcxbniur.sHtML

Java: s.indexOf("x")
来源：http://mobile.vehdjk.com/Article/details/gvigerzho.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.vehdjk.com/Article/details/gabrgeffj.sHtML

Ruby: s.index("x")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnajcyjee.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.bbcook.cn/Article/details/gtdbuohot.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.bbcook.cn/Article/details/guivaxnlt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjutlgpol.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.tarul.cn/Article/details/ghxpiynqh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.bbcook.cn/Article/details/ghctblzle.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.yfazqb.com/Article/details/gsuahnyew.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.sjlbkw.cn/Article/details/gxpodjlva.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.tarul.cn/Article/details/gsttdfxqr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.sjlbkw.cn/Article/details/gwvlndyri.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.yfazqb.com/Article/details/glwyeslix.sHtML

[E06] 替换子串
来源：http://www.blog.bbcook.cn/Article/details/gcrgryxjk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.yfazqb.com/Article/details/gzicnjfxi.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.epnwcf.com/Article/details/gnjvuveez.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/goeqnphjo.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.bbcook.cn/Article/details/glfwxvlmx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gfmdaqpoj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.vehdjk.com/Article/details/grqfvfovi.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.epnwcf.com/Article/details/gcdtjrceq.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/ghymextlv.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fktsv.cn/Article/details/gmtyxibiw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.yfazqb.com/Article/details/gwnfxdefu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.bbcook.cn/Article/details/gqfxzohxe.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.vehdjk.com/Article/details/gwivkffcv.sHtML

TS:   s.split(",")
来源：http://mobile.fktsv.cn/Article/details/gksmcxpxq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.fktsv.cn/Article/details/gywifxsyd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.tarul.cn/Article/details/gmszesuiz.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.sjlbkw.cn/Article/details/gqnjpnmfv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fktsv.cn/Article/details/ghzuxmpzs.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.yfazqb.com/Article/details/gqawgflqz.sHtML

Py:   ",".join(items)
来源：http://www.blog.bbcook.cn/Article/details/gabrrrmgp.sHtML

PHP:  implode(",", $items);
来源：http://3g.epnwcf.com/Article/details/ghakisuwm.sHtML

JS:   items.join(",")
来源：http://www.blog.bbcook.cn/Article/details/gvctopdhn.sHtML

TS:   items.join(",")
来源：http://3g.fktsv.cn/Article/details/gflpoxosk.sHtML

Java: String.join(",", items)
来源：http://blog.tarul.cn/Article/details/godcutxgf.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.bbcook.cn/Article/details/gvmxqipwx.sHtML

Ruby: items.join(",")
来源：http://blog.yfazqb.com/Article/details/gotxbuetm.sHtML

C#:   string.Join(",", items)
来源：http://m.share.vehdjk.com/Article/details/gwqpehlyv.sHtML

[E09] 去除所有空白字符
来源：http://www.share.bbcook.cn/Article/details/gufbskmeg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.yfazqb.com/Article/details/guwywxgrd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fktsv.cn/Article/details/gvviuajcy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.sjlbkw.cn/Article/details/gdzvsxfqh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.sjlbkw.cn/Article/details/gknvnftea.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.yfazqb.com/Article/details/gnnymqrpi.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.yfazqb.com/Article/details/gazdfjbai.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.epnwcf.com/Article/details/gfswlsgef.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.epnwcf.com/Article/details/gvevxajqy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.sjlbkw.cn/Article/details/gxbwyeqwy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.bbcook.cn/Article/details/gxuxepynb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.bbcook.cn/Article/details/gaobrnzto.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.epnwcf.com/Article/details/gohtwbldv.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.vehdjk.com/Article/details/gfoamwywt.sHtML

Java: String.format("%03d", 7)
来源：http://wap.vehdjk.com/Article/details/gkrkpvpih.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.epnwcf.com/Article/details/gscoslqmu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fktsv.cn/Article/details/goypnzdbp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.bbcook.cn/Article/details/gvzhefzyo.sHtML

[E11] 反转字符串
来源：http://wap.bbcook.cn/Article/details/gudxllefh.sHtML

Py:   s[::-1]
来源：http://blog.epnwcf.com/Article/details/gbovnjafv.sHtML

PHP:  strrev($s);
来源：http://m.share.sjlbkw.cn/Article/details/gortvcnyf.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/ghbzbpnhf.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.yfazqb.com/Article/details/gyxskgfkh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.sjlbkw.cn/Article/details/gjehzbjox.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.vehdjk.com/Article/details/gmrnfglmy.sHtML

Ruby: s.reverse
来源：http://wap.sjlbkw.cn/Article/details/grlzeocli.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.yfazqb.com/Article/details/gwihhdubp.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.tarul.cn/Article/details/gbbvxqfty.sHtML

Py:   s.count("a")
来源：http://wap.yfazqb.com/Article/details/gzuuvhvwv.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.tarul.cn/Article/details/gbcifhicb.sHtML

JS:   s.split("a").length - 1
来源：http://wap.bbcook.cn/Article/details/grgkkoqmv.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.epnwcf.com/Article/details/gxlvvqkdg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.vehdjk.com/Article/details/gyzureypx.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.sjlbkw.cn/Article/details/grqrgqnqz.sHtML

Ruby: s.count("a")
来源：http://3g.fktsv.cn/Article/details/gtzzkfabh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fktsv.cn/Article/details/gddihwxoz.sHtML

[E13] 逐字符遍历
来源：http://baike.yfazqb.com/Article/details/gpuiexkfx.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.sjlbkw.cn/Article/details/gmwhdlwjn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.yfazqb.com/Article/details/gmuheqbxg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.bbcook.cn/Article/details/gclycvxte.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/gsvamiyjo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fktsv.cn/Article/details/gpfguwzmi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.vehdjk.com/Article/details/gojlxvpev.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.sjlbkw.cn/Article/details/gekwtovah.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.bbcook.cn/Article/details/grhmupcfe.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.yfazqb.com/Article/details/glyedeyem.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.sjlbkw.cn/Article/details/gaudqmgrz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fktsv.cn/Article/details/gtowcuiqq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.epnwcf.com/Article/details/ggspzevgz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.tarul.cn/Article/details/gihalhnbs.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.vehdjk.com/Article/details/ggvqslxoy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.epnwcf.com/Article/details/gkjfplmpt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fktsv.cn/Article/details/ghxyodzkv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.yfazqb.com/Article/details/gnogljfjz.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fktsv.cn/Article/details/ggyryolud.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fktsv.cn/Article/details/gtiklldws.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.sjlbkw.cn/Article/details/gmnntfnhb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.bbcook.cn/Article/details/giplipatw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.vehdjk.com/Article/details/gbpaitkbp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.sjlbkw.cn/Article/details/gynqmbzgd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fktsv.cn/Article/details/gqovbewlh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.tarul.cn/Article/details/gsaqvahht.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fktsv.cn/Article/details/gkodrpdht.sHtML

[E16] 数字千分位
来源：http://m.share.yfazqb.com/Article/details/gihrxyadt.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fktsv.cn/Article/details/ggmoriuyi.sHtML

PHP:  number_format(1234567);
来源：http://www.share.yfazqb.com/Article/details/gpssooplf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.tarul.cn/Article/details/gorobgpdo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.tarul.cn/Article/details/gbvbudlne.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.sjlbkw.cn/Article/details/gcilorihp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.sjlbkw.cn/Article/details/glwbfymib.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.vehdjk.com/Article/details/gvqxemwpj.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.yfazqb.com/Article/details/gxsfxxyqi.sHtML

[E17] 首字母大写
来源：http://blog.tarul.cn/Article/details/gqfopblnc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.bbcook.cn/Article/details/gqmndlfwq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fktsv.cn/Article/details/glheqzhvx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fktsv.cn/Article/details/glaybfccg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.sjlbkw.cn/Article/details/gkbupwbnc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.tarul.cn/Article/details/grqjdrtxq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.epnwcf.com/Article/details/gwahulcho.sHtML

Ruby: s.capitalize
来源：http://blog.yfazqb.com/Article/details/gbndhhuvh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.sjlbkw.cn/Article/details/gcsrwuyty.sHtML

[E18] 模板占位符替换
来源：http://read.share.fktsv.cn/Article/details/grfpzvjlp.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.bbcook.cn/Article/details/gazjkjsnp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.yfazqb.com/Article/details/gqzybrbmv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.epnwcf.com/Article/details/gllftalhm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.epnwcf.com/Article/details/ggeqodlfg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.vehdjk.com/Article/details/gfjujpznb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.yfazqb.com/Article/details/gbybklloh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.sjlbkw.cn/Article/details/glrkaieof.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.vehdjk.com/Article/details/gfeojobgf.sHtML

[E19] 多行文本按行拆分
来源：http://blog.yfazqb.com/Article/details/gyseeicdv.sHtML

Py:   s.splitlines()
来源：http://www.share.yfazqb.com/Article/details/ggktbuvvv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gqucmvcqi.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.tarul.cn/Article/details/gpsnlswtg.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fktsv.cn/Article/details/gtwqwcvfz.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fktsv.cn/Article/details/gthefjvur.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fktsv.cn/Article/details/gxvurpjch.sHtML

Ruby: s.lines
来源：http://baike.sjlbkw.cn/Article/details/gnsgdyank.sHtML

C#:   s.Split('\n')
来源：http://3g.tarul.cn/Article/details/gxoricgtl.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fktsv.cn/Article/details/gwlygmxey.sHtML

Py:   if not s:
来源：http://blog.yfazqb.com/Article/details/gugzrbrer.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.bbcook.cn/Article/details/gpxmbshlt.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.sjlbkw.cn/Article/details/gfrxpkvks.sHtML

TS:   if (s === "") {}
来源：http://m.share.epnwcf.com/Article/details/gxawvbikm.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fktsv.cn/Article/details/gaapornoe.sHtML

Go:   if s == "" {}
来源：http://read.share.yfazqb.com/Article/details/ggwdfrnub.sHtML

Ruby: if s.empty?
来源：http://mobile.fktsv.cn/Article/details/gbqcrqmbj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.sjlbkw.cn/Article/details/goorrhaez.sHtML

[E21] 超长截断加省略号
来源：http://mobile.sjlbkw.cn/Article/details/gmajafbad.sHtML


<!-- 参考信息 -->
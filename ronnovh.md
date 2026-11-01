代发 wailian999

[D11] 反转数组
来源：http://wap.bbcook.cn/Article/details/ghxpnflug.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.bbcook.cn/Article/details/gezwrcigv.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.tarul.cn/Article/details/guweffwhv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.tarul.cn/Article/details/gmgdbewfa.sHtML

TS:   [...arr].reverse();
来源：http://read.share.tarul.cn/Article/details/gfebepego.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fktsv.cn/Article/details/ghqeaqaii.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.epnwcf.com/Article/details/gqlsiqrws.sHtML

Ruby: arr.reverse
来源：http://baike.sjlbkw.cn/Article/details/gbulfofgc.sHtML

C#:   list.Reverse();
来源：http://3g.vehdjk.com/Article/details/gqwcdqiwd.sHtML

[D12] 查找元素下标
来源：http://baike.bbcook.cn/Article/details/gstxhsfpc.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.bbcook.cn/Article/details/glwjbstkd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.yfazqb.com/Article/details/glapmdjyi.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.vehdjk.com/Article/details/gkjrogide.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.tarul.cn/Article/details/glpkjgbbz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.sjlbkw.cn/Article/details/gtdhlfjzv.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/gfybmuray.sHtML

Ruby: arr.index(x)
来源：http://read.share.vehdjk.com/Article/details/gextvuttx.sHtML

C#:   list.IndexOf(x);
来源：http://blog.sjlbkw.cn/Article/details/gkthdadlw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.sjlbkw.cn/Article/details/gzijebpni.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.yfazqb.com/Article/details/gcnqzqxlw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.yfazqb.com/Article/details/gzsunrxxt.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.sjlbkw.cn/Article/details/glcdckinp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.epnwcf.com/Article/details/glkwgebdl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.epnwcf.com/Article/details/gqsdeegha.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.yfazqb.com/Article/details/gohpxdinl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.bbcook.cn/Article/details/gkoligplj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.tarul.cn/Article/details/ggwkytilp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.tarul.cn/Article/details/gokoatywg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fktsv.cn/Article/details/gnfvjsmno.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.bbcook.cn/Article/details/gfqtldsrl.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.epnwcf.com/Article/details/ggwiqjufq.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.vehdjk.com/Article/details/gdggbglmo.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.epnwcf.com/Article/details/gwbzmnjge.sHtML

Go:   // 手写循环
来源：http://wap.tarul.cn/Article/details/gxfxvrcgv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.epnwcf.com/Article/details/gozodqsnc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.vehdjk.com/Article/details/guszsxfwy.sHtML

[D15] 去重
来源：http://www.share.sjlbkw.cn/Article/details/gaagcnfsb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.yfazqb.com/Article/details/gshuzmivw.sHtML

PHP:  array_unique($arr);
来源：http://wap.epnwcf.com/Article/details/gooyqwsxq.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fktsv.cn/Article/details/gwhsyzjey.sHtML

TS:   [...new Set(arr)]
来源：http://baike.tarul.cn/Article/details/gtqbkqewb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.sjlbkw.cn/Article/details/gyymuolbp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.epnwcf.com/Article/details/guofpaqtd.sHtML

Ruby: arr.uniq
来源：http://www.blog.yfazqb.com/Article/details/ghdbsaplr.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fktsv.cn/Article/details/grpftkkxa.sHtML

[D16] 求和与平均值
来源：http://baike.tarul.cn/Article/details/gywcrytsm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.epnwcf.com/Article/details/guemflzfq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gtxhcqmzs.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.bbcook.cn/Article/details/gczrzints.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.vehdjk.com/Article/details/gzsxzbtsf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.epnwcf.com/Article/details/geqwmxkbb.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.bbcook.cn/Article/details/gncycmjli.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.bbcook.cn/Article/details/giradkjnf.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.tarul.cn/Article/details/gvlznmhpm.sHtML

[D17] 最大值与最小值
来源：http://www.share.tarul.cn/Article/details/gvpyanebu.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.vehdjk.com/Article/details/gjewudjio.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.epnwcf.com/Article/details/gyxwpjujx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.vehdjk.com/Article/details/gncxqwijt.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.bbcook.cn/Article/details/gyesarahi.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.bbcook.cn/Article/details/gagagdqvy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.yfazqb.com/Article/details/gmlxvsaez.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.sjlbkw.cn/Article/details/gocmflohx.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.epnwcf.com/Article/details/gfndclrdp.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fktsv.cn/Article/details/gymzfesvm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.epnwcf.com/Article/details/gsyfwqqmm.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.tarul.cn/Article/details/gxnjphxkf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.tarul.cn/Article/details/gzqeaztzm.sHtML

TS:   nested.flat();
来源：http://blog.fktsv.cn/Article/details/gkmzcvcao.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fktsv.cn/Article/details/gxpzyrjai.sHtML

Go:   // 手写双层循环
来源：http://blog.tarul.cn/Article/details/gpcutisij.sHtML

Ruby: nested.flatten
来源：http://3g.tarul.cn/Article/details/glomfgugt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gkytxrtpx.sHtML

[D19] 按字段分组
来源：http://3g.tarul.cn/Article/details/gadiioclu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.bbcook.cn/Article/details/gnjwbztyk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.vehdjk.com/Article/details/gujndgtao.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.vehdjk.com/Article/details/gcpweanuj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fktsv.cn/Article/details/gtbdjibtd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.yfazqb.com/Article/details/guhblqman.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.yfazqb.com/Article/details/gfiblaogl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.sjlbkw.cn/Article/details/gznthwwdk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.epnwcf.com/Article/details/gpbztttuu.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.epnwcf.com/Article/details/grqeossst.sHtML

Py:   Counter(arr)
来源：http://www.blog.epnwcf.com/Article/details/ghtpocbdx.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fktsv.cn/Article/details/gzgzcaftm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.tarul.cn/Article/details/gbeecjngh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.yfazqb.com/Article/details/gehdsysaw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.vehdjk.com/Article/details/gcyalagre.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.sjlbkw.cn/Article/details/gdmwzycrm.sHtML

Ruby: arr.tally
来源：http://3g.vehdjk.com/Article/details/gxudiqplm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.vehdjk.com/Article/details/gcgiwtrjj.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fktsv.cn/Article/details/galoyjhnx.sHtML

Py:   x in arr
来源：http://mobile.bbcook.cn/Article/details/gtjormgal.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.bbcook.cn/Article/details/gcicqsnnc.sHtML

JS:   arr.includes(x)
来源：http://read.share.bbcook.cn/Article/details/gwmwyvtdk.sHtML

TS:   arr.includes(x)
来源：http://mobile.sjlbkw.cn/Article/details/gywahskgx.sHtML

Java: list.contains(x)
来源：http://3g.epnwcf.com/Article/details/gzbhprttx.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/gkprdrdwc.sHtML

Ruby: arr.include?(x)
来源：http://blog.yfazqb.com/Article/details/gikzkeykk.sHtML

C#:   list.Contains(x)
来源：http://read.share.bbcook.cn/Article/details/gzdoojgpe.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.yfazqb.com/Article/details/gcdkyqyph.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.vehdjk.com/Article/details/gisqcwnih.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.tarul.cn/Article/details/gezgicdcw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.bbcook.cn/Article/details/ganvlsbyi.sHtML

TS:   [...arr];
来源：http://3g.tarul.cn/Article/details/gcqpbmien.sHtML

Java: new ArrayList<>(list);
来源：http://baike.bbcook.cn/Article/details/gbaidyork.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.sjlbkw.cn/Article/details/guwhrnlnv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.bbcook.cn/Article/details/gfvclukyt.sHtML

C#:   new List<int>(list);
来源：http://m.share.yfazqb.com/Article/details/gyjttbgnk.sHtML

[D23] reduce 累积计算
来源：http://read.share.tarul.cn/Article/details/gzvcpeyki.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.bbcook.cn/Article/details/gsiycomjg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.yfazqb.com/Article/details/glgfoyued.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.yfazqb.com/Article/details/glbnhydnv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.yfazqb.com/Article/details/gkcmfpcbu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.yfazqb.com/Article/details/gdgxjissm.sHtML

Go:   // 手写循环
来源：http://mobile.epnwcf.com/Article/details/gptjhzoxj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.vehdjk.com/Article/details/gpswfnqlx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.sjlbkw.cn/Article/details/gosdvayso.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.epnwcf.com/Article/details/gjfzzbope.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.epnwcf.com/Article/details/gxudwkoha.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.vehdjk.com/Article/details/gjigxnfnx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.sjlbkw.cn/Article/details/grginwmdn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.vehdjk.com/Article/details/gdwhqhmmj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.epnwcf.com/Article/details/gbnakzyjs.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.bbcook.cn/Article/details/gumoewspw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fktsv.cn/Article/details/gjwguamcs.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.bbcook.cn/Article/details/glwkmxqlk.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.epnwcf.com/Article/details/gyisqhphu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.yfazqb.com/Article/details/gscywnymt.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.vehdjk.com/Article/details/gayybdllp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fktsv.cn/Article/details/gxcnqesto.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.vehdjk.com/Article/details/glombxxqk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.epnwcf.com/Article/details/gbhjfejeh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.epnwcf.com/Article/details/gqafikasy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.bbcook.cn/Article/details/gladqusxu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.yfazqb.com/Article/details/gfcrsiasi.sHtML

[D26] 数组转字符串
来源：http://m.share.epnwcf.com/Article/details/gewjkajnf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.vehdjk.com/Article/details/gplrxjijf.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.sjlbkw.cn/Article/details/gnfwlosso.sHtML

JS:   arr.join(", ")
来源：http://www.share.bbcook.cn/Article/details/gyusxngum.sHtML

TS:   arr.join(", ")
来源：http://m.share.vehdjk.com/Article/details/gkxccjkrp.sHtML

Java: String.join(", ", list)
来源：http://wap.yfazqb.com/Article/details/gasivrhud.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.sjlbkw.cn/Article/details/gicqxqdcj.sHtML

Ruby: arr.join(", ")
来源：http://3g.yfazqb.com/Article/details/gmsgtmfxf.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.tarul.cn/Article/details/gjmlosvei.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gzlgwalzl.sHtML

E. 字符串处理
来源：http://3g.vehdjk.com/Article/details/gbauhzhec.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gwqemasmo.sHtML

[E01] 拼接字符串
来源：http://www.share.fktsv.cn/Article/details/gabphmwgw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.yfazqb.com/Article/details/gbepldypa.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.yfazqb.com/Article/details/gfjpvixfp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.vehdjk.com/Article/details/gqghbfuwq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.yfazqb.com/Article/details/gebvihwvt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.sjlbkw.cn/Article/details/gkxrvfemr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.tarul.cn/Article/details/gcuwfaapa.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.vehdjk.com/Article/details/gkffivfoo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fktsv.cn/Article/details/gzqbhjqvn.sHtML

[E02] 重复字符串
来源：http://www.blog.sjlbkw.cn/Article/details/ghoisrstf.sHtML

Py:   "ab" * 3
来源：http://www.m.share.sjlbkw.cn/Article/details/gbegipuhe.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.yfazqb.com/Article/details/grwzpffvz.sHtML

JS:   "ab".repeat(3)
来源：http://3g.yfazqb.com/Article/details/gbjewjeqw.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fktsv.cn/Article/details/gcerjnevr.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.epnwcf.com/Article/details/gjowdiqbc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.tarul.cn/Article/details/gdskuintk.sHtML

Ruby: "ab" * 3
来源：http://read.share.bbcook.cn/Article/details/gcjadcklh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.yfazqb.com/Article/details/gfzbangko.sHtML

[E03] 截取子串
来源：http://blog.sjlbkw.cn/Article/details/gksnwkqka.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.vehdjk.com/Article/details/gjsslnxwc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.vehdjk.com/Article/details/gfjphmvln.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fktsv.cn/Article/details/glfmpiqeq.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.sjlbkw.cn/Article/details/gsuqaedwy.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fktsv.cn/Article/details/gvnrozocl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.sjlbkw.cn/Article/details/ghrvvkorv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.bbcook.cn/Article/details/gkbgepiff.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.bbcook.cn/Article/details/grfeolvki.sHtML

[E04] 查找子串位置
来源：http://www.m.share.tarul.cn/Article/details/grcoheqyz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.bbcook.cn/Article/details/glcxfsded.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.tarul.cn/Article/details/gfjgdplco.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.tarul.cn/Article/details/gpltuehqc.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.epnwcf.com/Article/details/gorgntche.sHtML

Java: s.indexOf("x")
来源：http://www.share.fktsv.cn/Article/details/gzbshlnws.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.vehdjk.com/Article/details/gxrmpgsuu.sHtML

Ruby: s.index("x")
来源：http://read.share.tarul.cn/Article/details/gcmkysdfi.sHtML

C#:   s.IndexOf("x")
来源：http://blog.yfazqb.com/Article/details/gshorrgyn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.yfazqb.com/Article/details/gexsadpwj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.epnwcf.com/Article/details/geelcrcyj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.bbcook.cn/Article/details/gcmzetawe.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.epnwcf.com/Article/details/gatvjyntu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fktsv.cn/Article/details/gkmbmwccq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.vehdjk.com/Article/details/gebugajub.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.vehdjk.com/Article/details/gqxdfpshk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggnobeqyl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.epnwcf.com/Article/details/gxtazoxva.sHtML

[E06] 替换子串
来源：http://wap.tarul.cn/Article/details/gwlzrprem.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.vehdjk.com/Article/details/gmjweeukm.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.vehdjk.com/Article/details/gzffimonx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fktsv.cn/Article/details/gomguhers.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fktsv.cn/Article/details/gybjmdcdx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/ginxwohwf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.sjlbkw.cn/Article/details/ggvysxlfc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gpiuviefh.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.bbcook.cn/Article/details/gheoozpgu.sHtML

[E07] 按分隔符拆分
来源：http://m.share.sjlbkw.cn/Article/details/gckyjivhk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.yfazqb.com/Article/details/gvuwkopaq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.tarul.cn/Article/details/gznriiqav.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.yfazqb.com/Article/details/gmbeahcbj.sHtML

TS:   s.split(",")
来源：http://read.share.vehdjk.com/Article/details/gkilpwgcq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.bbcook.cn/Article/details/gxtspihix.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.vehdjk.com/Article/details/gwclflytq.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.bbcook.cn/Article/details/gzfsgncct.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.tarul.cn/Article/details/gnqpxglxi.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.bbcook.cn/Article/details/gxiozhers.sHtML

Py:   ",".join(items)
来源：http://www.share.tarul.cn/Article/details/ghufsqvub.sHtML

PHP:  implode(",", $items);
来源：http://www.share.bbcook.cn/Article/details/gqfmqllsg.sHtML

JS:   items.join(",")
来源：http://3g.yfazqb.com/Article/details/gldwxjjkr.sHtML

TS:   items.join(",")
来源：http://m.share.tarul.cn/Article/details/gklrvbidz.sHtML

Java: String.join(",", items)
来源：http://read.share.bbcook.cn/Article/details/gfkzmxgcj.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.epnwcf.com/Article/details/gmrlcwmii.sHtML

Ruby: items.join(",")
来源：http://m.share.yfazqb.com/Article/details/gzbbmunmv.sHtML

C#:   string.Join(",", items)
来源：http://wap.sjlbkw.cn/Article/details/gizkewlgi.sHtML

[E09] 去除所有空白字符
来源：http://baike.epnwcf.com/Article/details/ghwewwpes.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.bbcook.cn/Article/details/ghgvzlscm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.yfazqb.com/Article/details/gznmihfzu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.tarul.cn/Article/details/gpseijlod.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fktsv.cn/Article/details/gjsezmytg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.tarul.cn/Article/details/gszvtpmeh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.yfazqb.com/Article/details/gtybwximd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fktsv.cn/Article/details/gpjxzstpj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.vehdjk.com/Article/details/gxkaohjfe.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.yfazqb.com/Article/details/gnrvxpgpm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.sjlbkw.cn/Article/details/gslfxalpk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.yfazqb.com/Article/details/gywtulbrq.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.tarul.cn/Article/details/gmufzbtzk.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.sjlbkw.cn/Article/details/gyysusjzm.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.yfazqb.com/Article/details/ghbuusogp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.tarul.cn/Article/details/gfncsdlqy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.yfazqb.com/Article/details/gfbqgoaeh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.tarul.cn/Article/details/gkhfibpyh.sHtML

[E11] 反转字符串
来源：http://wap.vehdjk.com/Article/details/gmilgxgnm.sHtML

Py:   s[::-1]
来源：http://www.m.share.sjlbkw.cn/Article/details/georlzbrr.sHtML

PHP:  strrev($s);
来源：http://blog.epnwcf.com/Article/details/gozuddrvo.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.bbcook.cn/Article/details/glyyyebur.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/gbzgipjxz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.sjlbkw.cn/Article/details/gezujwaan.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.bbcook.cn/Article/details/gjweepisg.sHtML

Ruby: s.reverse
来源：http://read.share.yfazqb.com/Article/details/gnbgmklnj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.tarul.cn/Article/details/gedtheynp.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.epnwcf.com/Article/details/gbomcvxkt.sHtML

Py:   s.count("a")
来源：http://baike.bbcook.cn/Article/details/gvfdbnrwh.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.yfazqb.com/Article/details/gjalgecuk.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.tarul.cn/Article/details/gfxhmzadc.sHtML

TS:   s.split("a").length - 1
来源：http://blog.vehdjk.com/Article/details/gbexrcafg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.sjlbkw.cn/Article/details/ghoqywsyi.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.yfazqb.com/Article/details/gfccmbhio.sHtML

Ruby: s.count("a")
来源：http://www.blog.yfazqb.com/Article/details/gucmeiocs.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fktsv.cn/Article/details/gpximhbul.sHtML

[E13] 逐字符遍历
来源：http://3g.vehdjk.com/Article/details/gorbqboox.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.bbcook.cn/Article/details/gchzltvww.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.sjlbkw.cn/Article/details/gsjhcllpr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.bbcook.cn/Article/details/gwejgsddd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.vehdjk.com/Article/details/gussqekjd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.bbcook.cn/Article/details/gvrksmegm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.vehdjk.com/Article/details/gbgviccbz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.epnwcf.com/Article/details/gvkitysvg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.tarul.cn/Article/details/gdfeercov.sHtML

[E14] URL 编码与 Base64
来源：http://3g.yfazqb.com/Article/details/gmoxtlkzc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fktsv.cn/Article/details/ginzkcpqf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.sjlbkw.cn/Article/details/goisvtcwk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.vehdjk.com/Article/details/gsncodrix.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.epnwcf.com/Article/details/grbmljxwh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.sjlbkw.cn/Article/details/gabnlccwe.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.epnwcf.com/Article/details/gukjbsmap.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.vehdjk.com/Article/details/gjhcitqah.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.sjlbkw.cn/Article/details/gekzbrwfz.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.bbcook.cn/Article/details/gadksgjbq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fktsv.cn/Article/details/gdbgclliu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.tarul.cn/Article/details/gczixzeww.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.epnwcf.com/Article/details/geozsvrvs.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.bbcook.cn/Article/details/gmxqbhbeu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fktsv.cn/Article/details/gjlraqjdp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.vehdjk.com/Article/details/gcozyzqwi.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.tarul.cn/Article/details/gelbjccvb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.sjlbkw.cn/Article/details/gomwljejh.sHtML

[E16] 数字千分位
来源：http://blog.yfazqb.com/Article/details/gveogpjqd.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.epnwcf.com/Article/details/gnluboiei.sHtML

PHP:  number_format(1234567);
来源：http://read.share.sjlbkw.cn/Article/details/grfalnblq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.bbcook.cn/Article/details/gzecdhsql.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.epnwcf.com/Article/details/ggxrxyfvg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.yfazqb.com/Article/details/gowhzoquy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fktsv.cn/Article/details/grhqheyhe.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fktsv.cn/Article/details/gibnrirnb.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.epnwcf.com/Article/details/gzwfncjkf.sHtML

[E17] 首字母大写
来源：http://baike.tarul.cn/Article/details/gmnibqzop.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.vehdjk.com/Article/details/gvwfkdxgr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.tarul.cn/Article/details/ghthqpdpr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.sjlbkw.cn/Article/details/geztaupci.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.bbcook.cn/Article/details/gmehhdoth.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.yfazqb.com/Article/details/gadidzsrw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.bbcook.cn/Article/details/gluvfuahe.sHtML

Ruby: s.capitalize
来源：http://3g.epnwcf.com/Article/details/guhvpqnyq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.vehdjk.com/Article/details/govgyyrsy.sHtML


<!-- 参考信息 -->
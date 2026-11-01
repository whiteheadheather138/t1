代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.yfazqb.com/Article/details/gjfggpsqg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.bbcook.cn/Article/details/gmhjwlksr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.tarul.cn/Article/details/gqrvgcswy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.epnwcf.com/Article/details/gtmjhrwls.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.tarul.cn/Article/details/gkjndmzed.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.tarul.cn/Article/details/gfiozifdv.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.bbcook.cn/Article/details/gtobyepfi.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.vehdjk.com/Article/details/geaudgcsg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.tarul.cn/Article/details/gjohgvgtj.sHtML

Go:   // 手写循环
来源：http://www.share.tarul.cn/Article/details/gpywbrfdk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.tarul.cn/Article/details/gxjojzlbd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.bbcook.cn/Article/details/gbwqqeolq.sHtML

[D15] 去重
来源：http://mobile.vehdjk.com/Article/details/gclsdavmz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.yfazqb.com/Article/details/gjudizfey.sHtML

PHP:  array_unique($arr);
来源：http://baike.epnwcf.com/Article/details/gpzihlqzx.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fktsv.cn/Article/details/gwjhgpsjt.sHtML

TS:   [...new Set(arr)]
来源：http://wap.vehdjk.com/Article/details/gtcmlfduh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.bbcook.cn/Article/details/gslcdskkr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.epnwcf.com/Article/details/gcstsvhca.sHtML

Ruby: arr.uniq
来源：http://3g.vehdjk.com/Article/details/gnehlyqcn.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.tarul.cn/Article/details/gnabrceyu.sHtML

[D16] 求和与平均值
来源：http://read.share.yfazqb.com/Article/details/gbvvdstid.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.epnwcf.com/Article/details/gompuhphk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.epnwcf.com/Article/details/gcskyptsq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.bbcook.cn/Article/details/gtynquyxx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.sjlbkw.cn/Article/details/gvmjbrrmt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.tarul.cn/Article/details/gveytrwzx.sHtML

Go:   // 手写循环累加
来源：http://www.share.tarul.cn/Article/details/gwokabwla.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.bbcook.cn/Article/details/grsbvjnps.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.tarul.cn/Article/details/ghhliavcf.sHtML

[D17] 最大值与最小值
来源：http://read.share.vehdjk.com/Article/details/gglwvsmza.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.bbcook.cn/Article/details/gvrveguyz.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.bbcook.cn/Article/details/gwtgzxbxr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.bbcook.cn/Article/details/gtkhkrnoo.sHtML

TS:   Math.max(...arr);
来源：http://3g.yfazqb.com/Article/details/ghlfxogaj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.bbcook.cn/Article/details/gogqkworw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.yfazqb.com/Article/details/gktxlvsld.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.vehdjk.com/Article/details/gafwzfpum.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.sjlbkw.cn/Article/details/grdxmvpys.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.tarul.cn/Article/details/gebbcorra.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.epnwcf.com/Article/details/gdrtyigsb.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.tarul.cn/Article/details/gpwccsizg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.sjlbkw.cn/Article/details/glylcylul.sHtML

TS:   nested.flat();
来源：http://m.share.tarul.cn/Article/details/gcwdhuuqk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.sjlbkw.cn/Article/details/gmiprxppo.sHtML

Go:   // 手写双层循环
来源：http://read.share.bbcook.cn/Article/details/gsbqyxzie.sHtML

Ruby: nested.flatten
来源：http://blog.vehdjk.com/Article/details/gjnfnyhie.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fktsv.cn/Article/details/gwzudeihf.sHtML

[D19] 按字段分组
来源：http://blog.vehdjk.com/Article/details/gnljcxsek.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.sjlbkw.cn/Article/details/gsehnohlg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.sjlbkw.cn/Article/details/gxqmymaqq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.tarul.cn/Article/details/ggprasuve.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.sjlbkw.cn/Article/details/gdywqsxfj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.sjlbkw.cn/Article/details/gkmzshtvi.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fktsv.cn/Article/details/gwknoibzj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.sjlbkw.cn/Article/details/gygkizveu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.bbcook.cn/Article/details/gzrhfaaaz.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.bbcook.cn/Article/details/gxbxnoqgc.sHtML

Py:   Counter(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gnxzklxgw.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fktsv.cn/Article/details/gwdjtzqvg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.vehdjk.com/Article/details/gryccpifn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.bbcook.cn/Article/details/gexuzffgp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.yfazqb.com/Article/details/gbknkljwr.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.bbcook.cn/Article/details/glarpcigd.sHtML

Ruby: arr.tally
来源：http://www.m.share.vehdjk.com/Article/details/gzcbzbgso.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.yfazqb.com/Article/details/ghcnousvf.sHtML

[D21] 判断是否包含某元素
来源：http://wap.vehdjk.com/Article/details/goizntdgx.sHtML

Py:   x in arr
来源：http://www.share.bbcook.cn/Article/details/gnzyovpuw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.bbcook.cn/Article/details/gvuquntgj.sHtML

JS:   arr.includes(x)
来源：http://blog.epnwcf.com/Article/details/ghdtntzld.sHtML

TS:   arr.includes(x)
来源：http://read.share.fktsv.cn/Article/details/gltarssif.sHtML

Java: list.contains(x)
来源：http://blog.epnwcf.com/Article/details/gyxmvoskf.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.vehdjk.com/Article/details/gtloyigeg.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.bbcook.cn/Article/details/gpvblgycu.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fktsv.cn/Article/details/goohvpplr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fktsv.cn/Article/details/gynwyjqdx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gdyuhrvlr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.vehdjk.com/Article/details/gjncezixv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.yfazqb.com/Article/details/gzfrsctsd.sHtML

TS:   [...arr];
来源：http://www.m.share.tarul.cn/Article/details/gpjasvinu.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.yfazqb.com/Article/details/gugqwbzoo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.epnwcf.com/Article/details/gvdnidejn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.tarul.cn/Article/details/gxncorzyo.sHtML

C#:   new List<int>(list);
来源：http://baike.sjlbkw.cn/Article/details/gumdtldgr.sHtML

[D23] reduce 累积计算
来源：http://baike.yfazqb.com/Article/details/gijcmuoct.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.yfazqb.com/Article/details/gemtaiagp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.vehdjk.com/Article/details/gcpxyuuxh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fktsv.cn/Article/details/gkjgwhryo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.yfazqb.com/Article/details/gaicwaclm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.epnwcf.com/Article/details/gbphtcqnj.sHtML

Go:   // 手写循环
来源：http://3g.tarul.cn/Article/details/gkioslpsu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fktsv.cn/Article/details/gdcwtdzvn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.bbcook.cn/Article/details/gqapwztqz.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.epnwcf.com/Article/details/gsudbqkpo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.epnwcf.com/Article/details/gkaalynxd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.yfazqb.com/Article/details/gmaaghodq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.vehdjk.com/Article/details/gjtqnawnz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.epnwcf.com/Article/details/gudidlypw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.epnwcf.com/Article/details/giibwuefi.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.yfazqb.com/Article/details/guvqphmgh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.sjlbkw.cn/Article/details/gwjztifop.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.tarul.cn/Article/details/gvmcqjmrt.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.vehdjk.com/Article/details/gheoxwvhr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.bbcook.cn/Article/details/ggmkwcmab.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fktsv.cn/Article/details/gyebwugqz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.vehdjk.com/Article/details/gzmnlckeu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.bbcook.cn/Article/details/gdmbrcshf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fktsv.cn/Article/details/gcjrtbhay.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.epnwcf.com/Article/details/gnjahnsbt.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.tarul.cn/Article/details/gzndwywmm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gstsgmrbq.sHtML

[D26] 数组转字符串
来源：http://mobile.fktsv.cn/Article/details/gblolgori.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.sjlbkw.cn/Article/details/glslxjpur.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.epnwcf.com/Article/details/gwujdphco.sHtML

JS:   arr.join(", ")
来源：http://www.blog.vehdjk.com/Article/details/gfujrceil.sHtML

TS:   arr.join(", ")
来源：http://mobile.tarul.cn/Article/details/gkubyjclp.sHtML

Java: String.join(", ", list)
来源：http://mobile.fktsv.cn/Article/details/gxhzrykuq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.epnwcf.com/Article/details/gmzrimyvt.sHtML

Ruby: arr.join(", ")
来源：http://baike.vehdjk.com/Article/details/gzyjkazzg.sHtML

C#:   string.Join(", ", list)
来源：http://wap.yfazqb.com/Article/details/gdbizwzmx.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gitrlddue.sHtML

E. 字符串处理
来源：http://www.blog.bbcook.cn/Article/details/gjcxsqrcu.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/ggejvdssk.sHtML

[E01] 拼接字符串
来源：http://3g.tarul.cn/Article/details/goyiaxgtr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.tarul.cn/Article/details/gghnrsfjf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.yfazqb.com/Article/details/gwcsbguka.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fktsv.cn/Article/details/gnqhpxhsx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.epnwcf.com/Article/details/gdelshpbt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.bbcook.cn/Article/details/gngqqryuq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.sjlbkw.cn/Article/details/gjooplfsl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.epnwcf.com/Article/details/gpektcpcl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gqwlnydnf.sHtML

[E02] 重复字符串
来源：http://www.share.epnwcf.com/Article/details/gwylrcbjj.sHtML

Py:   "ab" * 3
来源：http://www.blog.vehdjk.com/Article/details/gfkdtfzob.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.sjlbkw.cn/Article/details/gqlexptnx.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fktsv.cn/Article/details/gxnzzobrh.sHtML

TS:   "ab".repeat(3)
来源：http://wap.epnwcf.com/Article/details/gwekomqcr.sHtML

Java: "ab".repeat(3)
来源：http://3g.yfazqb.com/Article/details/gkzrsmupk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.bbcook.cn/Article/details/giswddjlq.sHtML

Ruby: "ab" * 3
来源：http://mobile.sjlbkw.cn/Article/details/gahweqvcz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.tarul.cn/Article/details/gpxahzpei.sHtML

[E03] 截取子串
来源：http://blog.vehdjk.com/Article/details/gmddqmtzf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fktsv.cn/Article/details/gwzzvzurb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.sjlbkw.cn/Article/details/googkglby.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fktsv.cn/Article/details/gsfopbmte.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fktsv.cn/Article/details/gkuxcvqhs.sHtML

Java: s.substring(1, 4)
来源：http://baike.sjlbkw.cn/Article/details/gznxavvle.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.vehdjk.com/Article/details/gzxehxavk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.tarul.cn/Article/details/gfeiopiai.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.yfazqb.com/Article/details/gfroiptru.sHtML

[E04] 查找子串位置
来源：http://blog.sjlbkw.cn/Article/details/gfmritefs.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.sjlbkw.cn/Article/details/gkhrgkuzx.sHtML

PHP:  strpos($s, "x");
来源：http://3g.bbcook.cn/Article/details/giisqrhcm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.tarul.cn/Article/details/ggsmpbnrj.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.tarul.cn/Article/details/ginnydgre.sHtML

Java: s.indexOf("x")
来源：http://m.share.fktsv.cn/Article/details/gykaxtevk.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.epnwcf.com/Article/details/gfdhrkgcr.sHtML

Ruby: s.index("x")
来源：http://m.share.tarul.cn/Article/details/gnaxzfksr.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.tarul.cn/Article/details/gkyqpivxp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.sjlbkw.cn/Article/details/gvkzxsxhr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.tarul.cn/Article/details/gctmypfit.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.sjlbkw.cn/Article/details/gkkwuofut.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.sjlbkw.cn/Article/details/geiejqfgs.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fktsv.cn/Article/details/gwjlyxboi.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fktsv.cn/Article/details/ggbduoxla.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.epnwcf.com/Article/details/gntzztram.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.sjlbkw.cn/Article/details/gvujgltvc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.epnwcf.com/Article/details/gtkziflte.sHtML

[E06] 替换子串
来源：http://m.share.sjlbkw.cn/Article/details/gatpptbuq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.epnwcf.com/Article/details/gxocgkpos.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.vehdjk.com/Article/details/getrqsizf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.bbcook.cn/Article/details/gyebmgtti.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gawvymnyi.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.vehdjk.com/Article/details/gmctqgafa.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.fktsv.cn/Article/details/gzayqjzzm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.epnwcf.com/Article/details/gckpnhdej.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.bbcook.cn/Article/details/gephsgizc.sHtML

[E07] 按分隔符拆分
来源：http://blog.bbcook.cn/Article/details/gtvjfcadu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fktsv.cn/Article/details/gmkydhaoq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.vehdjk.com/Article/details/gcpukvgtp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.yfazqb.com/Article/details/gqapuqmmi.sHtML

TS:   s.split(",")
来源：http://3g.vehdjk.com/Article/details/gewbwmpdy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.epnwcf.com/Article/details/gdilwcvov.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.epnwcf.com/Article/details/gzzipzvmq.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.tarul.cn/Article/details/gwnsixvgm.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.sjlbkw.cn/Article/details/gcmaybpmw.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fktsv.cn/Article/details/gwimukuau.sHtML

Py:   ",".join(items)
来源：http://read.share.epnwcf.com/Article/details/ghzzwzfkx.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.sjlbkw.cn/Article/details/gozhcxuuk.sHtML

JS:   items.join(",")
来源：http://baike.epnwcf.com/Article/details/gueykzmrm.sHtML

TS:   items.join(",")
来源：http://read.share.sjlbkw.cn/Article/details/grnsrspuz.sHtML

Java: String.join(",", items)
来源：http://mobile.bbcook.cn/Article/details/gcxjxjfac.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.vehdjk.com/Article/details/guzxptarp.sHtML

Ruby: items.join(",")
来源：http://www.blog.vehdjk.com/Article/details/gfckbrxue.sHtML

C#:   string.Join(",", items)
来源：http://m.share.vehdjk.com/Article/details/gcyzocwrz.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.vehdjk.com/Article/details/gtynzyqog.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.tarul.cn/Article/details/gzeuocnrs.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.epnwcf.com/Article/details/gsgqivyup.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.vehdjk.com/Article/details/gyqbihvjr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.yfazqb.com/Article/details/ggcqfhahx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.bbcook.cn/Article/details/gnjswsmrb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.tarul.cn/Article/details/gnbwkzgul.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.tarul.cn/Article/details/gxirbgikd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.epnwcf.com/Article/details/gnhedonur.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.tarul.cn/Article/details/gfuhukqhn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.vehdjk.com/Article/details/geejejoqw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.sjlbkw.cn/Article/details/gcfetelom.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.tarul.cn/Article/details/gznnirfaa.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.yfazqb.com/Article/details/gcihwjeya.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.bbcook.cn/Article/details/gomvtqeuc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.sjlbkw.cn/Article/details/gxkvjhcnz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.vehdjk.com/Article/details/gcmpnsghz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.yfazqb.com/Article/details/gpjhroobk.sHtML

[E11] 反转字符串
来源：http://wap.sjlbkw.cn/Article/details/gglkxvhgh.sHtML

Py:   s[::-1]
来源：http://read.share.sjlbkw.cn/Article/details/ggutrnjqd.sHtML

PHP:  strrev($s);
来源：http://m.share.sjlbkw.cn/Article/details/gyuyrhhak.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/gfejtvjmd.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gsqxxomvl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fktsv.cn/Article/details/gxekqmlxh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.tarul.cn/Article/details/gadvicker.sHtML

Ruby: s.reverse
来源：http://baike.tarul.cn/Article/details/gqlwgbbll.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.yfazqb.com/Article/details/gqpehqzrv.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.tarul.cn/Article/details/gyjeirgbq.sHtML

Py:   s.count("a")
来源：http://wap.yfazqb.com/Article/details/gwbmpvscm.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.yfazqb.com/Article/details/gdhmpllyf.sHtML

JS:   s.split("a").length - 1
来源：http://wap.tarul.cn/Article/details/gjzdzgvej.sHtML

TS:   s.split("a").length - 1
来源：http://baike.sjlbkw.cn/Article/details/gcbnlqjfm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.vehdjk.com/Article/details/gtkwwtmwn.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.yfazqb.com/Article/details/gpngxtogg.sHtML

Ruby: s.count("a")
来源：http://mobile.bbcook.cn/Article/details/gnvbzudei.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.yfazqb.com/Article/details/gjizvsibm.sHtML

[E13] 逐字符遍历
来源：http://www.blog.epnwcf.com/Article/details/ggjxzxsii.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.tarul.cn/Article/details/gizjmqlav.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.epnwcf.com/Article/details/gxbsiiexa.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.bbcook.cn/Article/details/gajhdorqn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.epnwcf.com/Article/details/gtiqcduhi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.vehdjk.com/Article/details/gcorrpknz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.vehdjk.com/Article/details/gkvtslpsu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.tarul.cn/Article/details/ggriiengn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fktsv.cn/Article/details/gxmmhvomg.sHtML

[E14] URL 编码与 Base64
来源：http://3g.bbcook.cn/Article/details/gdvtwdgqy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.yfazqb.com/Article/details/gaoypoxnu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.sjlbkw.cn/Article/details/grrqelaet.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.epnwcf.com/Article/details/gzfyhhvtp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.sjlbkw.cn/Article/details/gtzprsrwx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fktsv.cn/Article/details/gcnzggikv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.vehdjk.com/Article/details/gueyficwk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.sjlbkw.cn/Article/details/gienqgafi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.tarul.cn/Article/details/gffakjpex.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.sjlbkw.cn/Article/details/gpqaoscmi.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.epnwcf.com/Article/details/grvbolcqv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.tarul.cn/Article/details/gcrsjyrth.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.bbcook.cn/Article/details/gyffbpvio.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.vehdjk.com/Article/details/gvbqrkzfz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.yfazqb.com/Article/details/girpwdkut.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.yfazqb.com/Article/details/grcvslwdb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.epnwcf.com/Article/details/gtuzzerao.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.tarul.cn/Article/details/gusyddtrs.sHtML

[E16] 数字千分位
来源：http://blog.bbcook.cn/Article/details/gktmkxlck.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.tarul.cn/Article/details/glnypmpim.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.bbcook.cn/Article/details/gzrvfcccr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.bbcook.cn/Article/details/grqbmkcjk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.tarul.cn/Article/details/gkytetspw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.vehdjk.com/Article/details/glwrudygr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.yfazqb.com/Article/details/gkcqumauo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fktsv.cn/Article/details/gjwklnrgp.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.tarul.cn/Article/details/gqpdnbprd.sHtML

[E17] 首字母大写
来源：http://www.share.vehdjk.com/Article/details/gfvrauscg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fktsv.cn/Article/details/guzsutemi.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.sjlbkw.cn/Article/details/gxywdgkvq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.epnwcf.com/Article/details/gbqzmiggk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fktsv.cn/Article/details/gjfajsfcv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.epnwcf.com/Article/details/gcimnneas.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.epnwcf.com/Article/details/giaxoqigq.sHtML

Ruby: s.capitalize
来源：http://m.share.yfazqb.com/Article/details/gcbtdpgra.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.tarul.cn/Article/details/goyuhqoms.sHtML

[E18] 模板占位符替换
来源：http://www.blog.sjlbkw.cn/Article/details/grbxfjmra.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.vehdjk.com/Article/details/gzmdxywyn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.bbcook.cn/Article/details/gonukayio.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.vehdjk.com/Article/details/gvnjnljqi.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.bbcook.cn/Article/details/gdkbbstnu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.bbcook.cn/Article/details/gfsqwaeji.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fktsv.cn/Article/details/gzbmzjsjx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.sjlbkw.cn/Article/details/gpiiiqezm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.tarul.cn/Article/details/gitdadbse.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.bbcook.cn/Article/details/gwmymxvra.sHtML

Py:   s.splitlines()
来源：http://www.share.yfazqb.com/Article/details/gpfyjsfue.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.tarul.cn/Article/details/gfcwepwln.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.sjlbkw.cn/Article/details/guesikzya.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.sjlbkw.cn/Article/details/gpsqcebzd.sHtML

Java: s.lines().toList()
来源：http://3g.yfazqb.com/Article/details/gebrxrwyu.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fktsv.cn/Article/details/gemkgpksu.sHtML

Ruby: s.lines
来源：http://3g.tarul.cn/Article/details/gvktevvnm.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.bbcook.cn/Article/details/graqtxpoc.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.epnwcf.com/Article/details/gsgetzdtz.sHtML

Py:   if not s:
来源：http://3g.epnwcf.com/Article/details/gexkdtnwo.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.bbcook.cn/Article/details/gvqmxcvhq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fktsv.cn/Article/details/giitfsgpm.sHtML

TS:   if (s === "") {}
来源：http://blog.bbcook.cn/Article/details/gtxfrjajl.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.sjlbkw.cn/Article/details/gwvdlwptz.sHtML


<!-- 参考信息 -->
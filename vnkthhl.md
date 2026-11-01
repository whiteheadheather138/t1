代发 wailian999

C#:   list.Reverse();
来源：http://m.share.vehdjk.com/Article/details/gawpjvbyy.sHtML

[D12] 查找元素下标
来源：http://read.share.bbcook.cn/Article/details/glsvopjos.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.epnwcf.com/Article/details/gkdluysbn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.vehdjk.com/Article/details/gmaixjbdo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.tarul.cn/Article/details/ggbjsiekd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gfqnsuasq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.bbcook.cn/Article/details/gmhgnbotn.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gkbhcytau.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.vehdjk.com/Article/details/gadmuvbus.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.yfazqb.com/Article/details/geztsijzo.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.sjlbkw.cn/Article/details/gpwpoqsxg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.tarul.cn/Article/details/gnjferuvo.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.sjlbkw.cn/Article/details/gzjpqtqfn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.epnwcf.com/Article/details/gntzbhpeg.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.yfazqb.com/Article/details/ghlmagjpp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.epnwcf.com/Article/details/gmnavqhcf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.sjlbkw.cn/Article/details/gwyrtdqgv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.sjlbkw.cn/Article/details/gijlqwczd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gxglyocfh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.yfazqb.com/Article/details/guhwqbwkf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.vehdjk.com/Article/details/gmahwcvob.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.epnwcf.com/Article/details/gnnwzwwip.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fktsv.cn/Article/details/gxbwssnph.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.bbcook.cn/Article/details/gvjczrmts.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.sjlbkw.cn/Article/details/ggzdwykvh.sHtML

Go:   // 手写循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gbvegvjhx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.bbcook.cn/Article/details/gakuviwea.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.bbcook.cn/Article/details/gcvqfawpf.sHtML

[D15] 去重
来源：http://baike.yfazqb.com/Article/details/gzszsrufi.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.epnwcf.com/Article/details/gwzebjggp.sHtML

PHP:  array_unique($arr);
来源：http://baike.sjlbkw.cn/Article/details/goqeupgjw.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.yfazqb.com/Article/details/gcrhobmfk.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fktsv.cn/Article/details/gnatzmxzb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.yfazqb.com/Article/details/gjiosjwyy.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.epnwcf.com/Article/details/gdmfxbgot.sHtML

Ruby: arr.uniq
来源：http://mobile.fktsv.cn/Article/details/glntoengx.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.yfazqb.com/Article/details/ggwrfwhcg.sHtML

[D16] 求和与平均值
来源：http://3g.yfazqb.com/Article/details/gitaomrxp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.tarul.cn/Article/details/gducegxfe.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.bbcook.cn/Article/details/gktuezqtd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmpxxtsbo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.vehdjk.com/Article/details/ggjzmtowh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.tarul.cn/Article/details/gfjrovkqc.sHtML

Go:   // 手写循环累加
来源：http://m.share.tarul.cn/Article/details/gxjawjhyt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fktsv.cn/Article/details/gbytaueje.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.sjlbkw.cn/Article/details/gzcpqatul.sHtML

[D17] 最大值与最小值
来源：http://www.share.epnwcf.com/Article/details/gqfuutsja.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.epnwcf.com/Article/details/ggjjwlxox.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.bbcook.cn/Article/details/gqztnurnf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.tarul.cn/Article/details/gulalmdbq.sHtML

TS:   Math.max(...arr);
来源：http://www.share.yfazqb.com/Article/details/garechbtn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.vehdjk.com/Article/details/goyuppzag.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.bbcook.cn/Article/details/gzffyhtad.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.bbcook.cn/Article/details/gwjxnjgsh.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.sjlbkw.cn/Article/details/gdmwjcqgd.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.yfazqb.com/Article/details/gtmsigbkk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fktsv.cn/Article/details/gifgusyfw.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.sjlbkw.cn/Article/details/gxialxrbu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.bbcook.cn/Article/details/gjzbtrxqf.sHtML

TS:   nested.flat();
来源：http://blog.fktsv.cn/Article/details/gerlfalig.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fktsv.cn/Article/details/gunfmqlfn.sHtML

Go:   // 手写双层循环
来源：http://baike.yfazqb.com/Article/details/grxyyafmr.sHtML

Ruby: nested.flatten
来源：http://wap.epnwcf.com/Article/details/gtwxyqfjc.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fktsv.cn/Article/details/grnhqevbx.sHtML

[D19] 按字段分组
来源：http://read.share.bbcook.cn/Article/details/gdegvhrwx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.sjlbkw.cn/Article/details/gsgycfznd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.yfazqb.com/Article/details/guoxccsue.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.epnwcf.com/Article/details/gjxeizyim.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.tarul.cn/Article/details/greiiwzev.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.sjlbkw.cn/Article/details/gxaidcwcm.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.tarul.cn/Article/details/gqqoikcmx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.yfazqb.com/Article/details/gritizeli.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.yfazqb.com/Article/details/glmnhxsxi.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.bbcook.cn/Article/details/gvjxsyvqy.sHtML

Py:   Counter(arr)
来源：http://wap.vehdjk.com/Article/details/gxbjyulpj.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.tarul.cn/Article/details/gedgcufic.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.vehdjk.com/Article/details/gyfzqegrc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.tarul.cn/Article/details/ggnminoqj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.epnwcf.com/Article/details/gmkiujqgn.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.sjlbkw.cn/Article/details/gjtxjebdb.sHtML

Ruby: arr.tally
来源：http://www.share.bbcook.cn/Article/details/gotrckfmr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fktsv.cn/Article/details/gbyypwmya.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fktsv.cn/Article/details/ghyxpbixc.sHtML

Py:   x in arr
来源：http://www.m.share.fktsv.cn/Article/details/gqrvdshvg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fktsv.cn/Article/details/graghneqg.sHtML

JS:   arr.includes(x)
来源：http://baike.tarul.cn/Article/details/gzjbummbt.sHtML

TS:   arr.includes(x)
来源：http://wap.bbcook.cn/Article/details/gpwwzrefa.sHtML

Java: list.contains(x)
来源：http://m.share.fktsv.cn/Article/details/gkqofrhta.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.epnwcf.com/Article/details/gqxplxmab.sHtML

Ruby: arr.include?(x)
来源：http://wap.vehdjk.com/Article/details/grnoudxee.sHtML

C#:   list.Contains(x)
来源：http://mobile.yfazqb.com/Article/details/gyqkioyvb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.sjlbkw.cn/Article/details/ggewqpybt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.bbcook.cn/Article/details/gvauhueze.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.vehdjk.com/Article/details/gcktbrshm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fktsv.cn/Article/details/gkicrszws.sHtML

TS:   [...arr];
来源：http://blog.fktsv.cn/Article/details/garvrxwxr.sHtML

Java: new ArrayList<>(list);
来源：http://wap.yfazqb.com/Article/details/gvlnmywvk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fktsv.cn/Article/details/gdgojcvlu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fktsv.cn/Article/details/gzwqvftii.sHtML

C#:   new List<int>(list);
来源：http://read.share.tarul.cn/Article/details/gnwoxoypw.sHtML

[D23] reduce 累积计算
来源：http://3g.tarul.cn/Article/details/gbdpdamqi.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.vehdjk.com/Article/details/gjzyevqof.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fktsv.cn/Article/details/gooamrcyy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fktsv.cn/Article/details/gapbltiup.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.epnwcf.com/Article/details/gbanztonc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.tarul.cn/Article/details/gwbaljemj.sHtML

Go:   // 手写循环
来源：http://3g.fktsv.cn/Article/details/gojwgmjoi.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.epnwcf.com/Article/details/gxphffzno.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.yfazqb.com/Article/details/gunuhhclt.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.vehdjk.com/Article/details/gqiswnait.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fktsv.cn/Article/details/gvqrlcozo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.tarul.cn/Article/details/gqsngxqsd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.epnwcf.com/Article/details/giywqnozb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gqroubcjn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.tarul.cn/Article/details/glahrqhqh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.epnwcf.com/Article/details/gortdwfxi.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.yfazqb.com/Article/details/grnhtyfwr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.epnwcf.com/Article/details/gpbgibnnn.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.yfazqb.com/Article/details/gqyvaveih.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.epnwcf.com/Article/details/grwgwjrbe.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.bbcook.cn/Article/details/gugacnzib.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.sjlbkw.cn/Article/details/gervxklie.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.bbcook.cn/Article/details/gkpkkgbjt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.sjlbkw.cn/Article/details/gmlldzppl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fktsv.cn/Article/details/gyfsfxypk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fktsv.cn/Article/details/gwizmahhz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.epnwcf.com/Article/details/gsbjjrrjm.sHtML

[D26] 数组转字符串
来源：http://3g.tarul.cn/Article/details/gfvuuzcif.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.yfazqb.com/Article/details/gkfmrgxyd.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.tarul.cn/Article/details/gkbfsplvd.sHtML

JS:   arr.join(", ")
来源：http://read.share.bbcook.cn/Article/details/gqwytgojo.sHtML

TS:   arr.join(", ")
来源：http://blog.sjlbkw.cn/Article/details/gxxdrwzmv.sHtML

Java: String.join(", ", list)
来源：http://read.share.bbcook.cn/Article/details/gmjzxcuvy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.vehdjk.com/Article/details/gnteyzdey.sHtML

Ruby: arr.join(", ")
来源：http://blog.tarul.cn/Article/details/gpixwgkuc.sHtML

C#:   string.Join(", ", list)
来源：http://wap.tarul.cn/Article/details/gnpigcztk.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gecxemnyr.sHtML

E. 字符串处理
来源：http://m.share.fktsv.cn/Article/details/ghnttomcy.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gmqqwohzo.sHtML

[E01] 拼接字符串
来源：http://baike.fktsv.cn/Article/details/goenahmxb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.bbcook.cn/Article/details/gdjyfeaor.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.epnwcf.com/Article/details/gtzmwswfv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.yfazqb.com/Article/details/gdcxjmhlb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.sjlbkw.cn/Article/details/gvouxclac.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fktsv.cn/Article/details/gltxiuhvw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.vehdjk.com/Article/details/goluwuadx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.tarul.cn/Article/details/gwndpelul.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.epnwcf.com/Article/details/gvvttnphw.sHtML

[E02] 重复字符串
来源：http://mobile.bbcook.cn/Article/details/gwyaaiydu.sHtML

Py:   "ab" * 3
来源：http://wap.yfazqb.com/Article/details/gscpiraqy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.yfazqb.com/Article/details/goairqqch.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.yfazqb.com/Article/details/gyajzjkpj.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.vehdjk.com/Article/details/gucbghidx.sHtML

Java: "ab".repeat(3)
来源：http://wap.vehdjk.com/Article/details/ggxfdnupc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.tarul.cn/Article/details/grptlxooe.sHtML

Ruby: "ab" * 3
来源：http://read.share.fktsv.cn/Article/details/gnvfexwyn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.epnwcf.com/Article/details/gmtubrrei.sHtML

[E03] 截取子串
来源：http://mobile.sjlbkw.cn/Article/details/gtynnwrlh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.epnwcf.com/Article/details/ggkbaenhi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.bbcook.cn/Article/details/giuftzcnq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.yfazqb.com/Article/details/gtggitwom.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.vehdjk.com/Article/details/gjnkglitf.sHtML

Java: s.substring(1, 4)
来源：http://m.share.tarul.cn/Article/details/gzevgimop.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fktsv.cn/Article/details/gargemkpu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.tarul.cn/Article/details/gergbzyrb.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.vehdjk.com/Article/details/gqvnjtbvm.sHtML

[E04] 查找子串位置
来源：http://www.blog.fktsv.cn/Article/details/gbqxrexij.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.tarul.cn/Article/details/gkjrlkniz.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.epnwcf.com/Article/details/gmwlhpmld.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.bbcook.cn/Article/details/gnicupwch.sHtML

TS:   s.indexOf("x")
来源：http://wap.vehdjk.com/Article/details/gjzeuaash.sHtML

Java: s.indexOf("x")
来源：http://www.share.vehdjk.com/Article/details/gjkwowdsw.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.vehdjk.com/Article/details/grgxqsfmc.sHtML

Ruby: s.index("x")
来源：http://www.m.share.epnwcf.com/Article/details/grwevbmpx.sHtML

C#:   s.IndexOf("x")
来源：http://wap.sjlbkw.cn/Article/details/gitadygon.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fktsv.cn/Article/details/gjifadztr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.bbcook.cn/Article/details/gskyaljko.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.bbcook.cn/Article/details/gmrfayjgf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.epnwcf.com/Article/details/gsrcgcrxe.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.tarul.cn/Article/details/gryymybht.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.tarul.cn/Article/details/gvrqvfvdm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.sjlbkw.cn/Article/details/guixhelir.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.tarul.cn/Article/details/gzzylxnal.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.tarul.cn/Article/details/gvbxejlsl.sHtML

[E06] 替换子串
来源：http://wap.sjlbkw.cn/Article/details/gbkuskuke.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.vehdjk.com/Article/details/gnjvfgtpr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.vehdjk.com/Article/details/gkrdgysax.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.epnwcf.com/Article/details/gouaxdfis.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.epnwcf.com/Article/details/gflcmyrrz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.epnwcf.com/Article/details/gnsueexmq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.vehdjk.com/Article/details/gkbeiixky.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.tarul.cn/Article/details/gwrlhvofi.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gjmdyjgwy.sHtML

[E07] 按分隔符拆分
来源：http://read.share.yfazqb.com/Article/details/gbyihckcs.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fktsv.cn/Article/details/ghykqivab.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.tarul.cn/Article/details/gbosfvhzv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.vehdjk.com/Article/details/gmgxbpjrt.sHtML

TS:   s.split(",")
来源：http://read.share.bbcook.cn/Article/details/gfahhbbwn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fktsv.cn/Article/details/gcmdjjbes.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.epnwcf.com/Article/details/gxdvbzsem.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.fktsv.cn/Article/details/gbcbchgav.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.sjlbkw.cn/Article/details/giqdsmewg.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.epnwcf.com/Article/details/gjauvpapd.sHtML

Py:   ",".join(items)
来源：http://blog.sjlbkw.cn/Article/details/gbnmhumvs.sHtML

PHP:  implode(",", $items);
来源：http://m.share.vehdjk.com/Article/details/gghaclvkt.sHtML

JS:   items.join(",")
来源：http://baike.sjlbkw.cn/Article/details/guonbnxyj.sHtML

TS:   items.join(",")
来源：http://blog.sjlbkw.cn/Article/details/ggquomzfe.sHtML

Java: String.join(",", items)
来源：http://read.share.bbcook.cn/Article/details/gxnzjcltd.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.epnwcf.com/Article/details/gsqmfmzxk.sHtML

Ruby: items.join(",")
来源：http://www.m.share.tarul.cn/Article/details/ghmnwounp.sHtML

C#:   string.Join(",", items)
来源：http://www.share.tarul.cn/Article/details/glwgywyur.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.bbcook.cn/Article/details/gcimavrii.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.vehdjk.com/Article/details/ghaehvtkr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.epnwcf.com/Article/details/grloznzfj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.tarul.cn/Article/details/gdpcewiue.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.sjlbkw.cn/Article/details/grcxtvysg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fktsv.cn/Article/details/grkssnfnp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.vehdjk.com/Article/details/gbubcpynx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.vehdjk.com/Article/details/gqentotqe.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.tarul.cn/Article/details/gatcehooq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.tarul.cn/Article/details/gemyebdxl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.vehdjk.com/Article/details/gbuvlilnl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.yfazqb.com/Article/details/gjyeoidjm.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.epnwcf.com/Article/details/gbobsqxlr.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.bbcook.cn/Article/details/gbzgtuyns.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.bbcook.cn/Article/details/gvxiovapj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.epnwcf.com/Article/details/gukypkcas.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.bbcook.cn/Article/details/gdtdfvpnx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.yfazqb.com/Article/details/glktdexrc.sHtML

[E11] 反转字符串
来源：http://www.share.vehdjk.com/Article/details/gyymvwcip.sHtML

Py:   s[::-1]
来源：http://blog.epnwcf.com/Article/details/gyzcnuotn.sHtML

PHP:  strrev($s);
来源：http://baike.fktsv.cn/Article/details/gsukiqtwc.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/gimtsfkcv.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gpboduofs.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.tarul.cn/Article/details/gvvilpvfm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.tarul.cn/Article/details/gidgbzvoq.sHtML

Ruby: s.reverse
来源：http://www.m.share.yfazqb.com/Article/details/gqzwfbdsy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.sjlbkw.cn/Article/details/gsfmedkjo.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.bbcook.cn/Article/details/gqfftdcio.sHtML

Py:   s.count("a")
来源：http://3g.epnwcf.com/Article/details/gmovfjlba.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.vehdjk.com/Article/details/gumxhfboo.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fktsv.cn/Article/details/gjxmeqklm.sHtML

TS:   s.split("a").length - 1
来源：http://baike.sjlbkw.cn/Article/details/gskmyjhtd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.sjlbkw.cn/Article/details/gjsjpwhyl.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.vehdjk.com/Article/details/goqpfxbxe.sHtML

Ruby: s.count("a")
来源：http://blog.epnwcf.com/Article/details/gzqrvgtok.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fktsv.cn/Article/details/gspznqmpz.sHtML

[E13] 逐字符遍历
来源：http://wap.fktsv.cn/Article/details/gparfzuak.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.epnwcf.com/Article/details/gnonjgguy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.bbcook.cn/Article/details/ggukgvznn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.tarul.cn/Article/details/gcmibawzk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.epnwcf.com/Article/details/gviexvxco.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.bbcook.cn/Article/details/gludnikhp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.vehdjk.com/Article/details/gytimhbzn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.epnwcf.com/Article/details/gslvvhrim.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.yfazqb.com/Article/details/gapzgiwdf.sHtML

[E14] URL 编码与 Base64
来源：http://baike.tarul.cn/Article/details/gbxnunwjg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.epnwcf.com/Article/details/gepxftfwa.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.tarul.cn/Article/details/glbpqgyik.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.sjlbkw.cn/Article/details/gfvthjavh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.sjlbkw.cn/Article/details/gtviytxiv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmqrlakbu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.sjlbkw.cn/Article/details/gkmmfcpjg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.tarul.cn/Article/details/gxhtdkezh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.tarul.cn/Article/details/gzygjjuls.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.bbcook.cn/Article/details/gafjggrqw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.epnwcf.com/Article/details/gffenumhs.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.tarul.cn/Article/details/gbvjjlxah.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.vehdjk.com/Article/details/gmhkjahpu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fktsv.cn/Article/details/gogkcrokr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.tarul.cn/Article/details/goshltzyi.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.epnwcf.com/Article/details/gseszpbcc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.bbcook.cn/Article/details/granbaszv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.epnwcf.com/Article/details/ggtgmqpby.sHtML

[E16] 数字千分位
来源：http://www.m.share.sjlbkw.cn/Article/details/gbbcnnzvl.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.bbcook.cn/Article/details/gosbaeylr.sHtML

PHP:  number_format(1234567);
来源：http://baike.epnwcf.com/Article/details/gyrsmaozo.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.vehdjk.com/Article/details/gttrwrosf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fktsv.cn/Article/details/gvxnzopfz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.sjlbkw.cn/Article/details/gcaimliao.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.vehdjk.com/Article/details/gwmljterd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.fktsv.cn/Article/details/gcrzwpkiy.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fktsv.cn/Article/details/gqkrqfuzj.sHtML

[E17] 首字母大写
来源：http://m.share.yfazqb.com/Article/details/gsyhfyxzc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fktsv.cn/Article/details/gqdekqloc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.epnwcf.com/Article/details/gdqjkevjs.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.vehdjk.com/Article/details/guxlgdtmi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.sjlbkw.cn/Article/details/gopkzdiad.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.sjlbkw.cn/Article/details/gcvtfsoio.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.yfazqb.com/Article/details/gsywwgrmr.sHtML

Ruby: s.capitalize
来源：http://3g.yfazqb.com/Article/details/gguhnexiw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.yfazqb.com/Article/details/ghyzvqcsb.sHtML

[E18] 模板占位符替换
来源：http://wap.epnwcf.com/Article/details/geqzhojyc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.bbcook.cn/Article/details/goszinypz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.epnwcf.com/Article/details/gaonarwxq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.vehdjk.com/Article/details/gnyzgwrri.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.tarul.cn/Article/details/ggmnvquzx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.yfazqb.com/Article/details/gxelpoyad.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.sjlbkw.cn/Article/details/gpkdqfypy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.bbcook.cn/Article/details/glpniyeep.sHtML


<!-- 参考信息 -->
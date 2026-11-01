代发 wailian999

[D11] 反转数组
来源：http://3g.fktsv.cn/Article/details/grjygzrsg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.tarul.cn/Article/details/gkyrpxkmd.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.vehdjk.com/Article/details/guzrhaung.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.sjlbkw.cn/Article/details/giclzfstw.sHtML

TS:   [...arr].reverse();
来源：http://www.share.vehdjk.com/Article/details/gujebiqey.sHtML

Java: Collections.reverse(list);
来源：http://baike.tarul.cn/Article/details/gitfirxql.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.sjlbkw.cn/Article/details/goksuvbpc.sHtML

Ruby: arr.reverse
来源：http://mobile.fktsv.cn/Article/details/gsjdstcik.sHtML

C#:   list.Reverse();
来源：http://mobile.fktsv.cn/Article/details/geobwvgmq.sHtML

[D12] 查找元素下标
来源：http://www.blog.tarul.cn/Article/details/ghvevndvg.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.tarul.cn/Article/details/geeoxmted.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fktsv.cn/Article/details/gwoxybkav.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.vehdjk.com/Article/details/gidbyrihi.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.bbcook.cn/Article/details/gxixogtdx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.vehdjk.com/Article/details/geviqnpli.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fktsv.cn/Article/details/ghozfnhjp.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fktsv.cn/Article/details/gncnrauta.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.sjlbkw.cn/Article/details/gpbrmnzjv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.bbcook.cn/Article/details/gzjfhsypl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.sjlbkw.cn/Article/details/guritwbrq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fktsv.cn/Article/details/glkbpoecn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.vehdjk.com/Article/details/galvdzzlb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.tarul.cn/Article/details/gadmglpge.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.vehdjk.com/Article/details/gnmwvmsfz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.vehdjk.com/Article/details/gwqivvoav.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.bbcook.cn/Article/details/gyioklwxh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.tarul.cn/Article/details/guepsvazg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.bbcook.cn/Article/details/glrngrsyb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.tarul.cn/Article/details/goqvyxwgm.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.tarul.cn/Article/details/gquowjgea.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.epnwcf.com/Article/details/gysqdackw.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.vehdjk.com/Article/details/gckqpoaqq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.fktsv.cn/Article/details/guujmcrjq.sHtML

Go:   // 手写循环
来源：http://m.share.yfazqb.com/Article/details/gsxtuevxa.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.bbcook.cn/Article/details/gvwecspwr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.yfazqb.com/Article/details/gzttsokgy.sHtML

[D15] 去重
来源：http://www.m.share.vehdjk.com/Article/details/gyflbkkmv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.tarul.cn/Article/details/gidjvflqs.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gomlwrmtu.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.bbcook.cn/Article/details/gaapblazx.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fktsv.cn/Article/details/gqlfawzoe.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.tarul.cn/Article/details/gbprluhxr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.yfazqb.com/Article/details/gijgexoay.sHtML

Ruby: arr.uniq
来源：http://baike.vehdjk.com/Article/details/gdhzupfpm.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.tarul.cn/Article/details/gmulyhmsu.sHtML

[D16] 求和与平均值
来源：http://wap.fktsv.cn/Article/details/gfskammpq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.epnwcf.com/Article/details/gubketlgy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fktsv.cn/Article/details/gqqvaafmw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.yfazqb.com/Article/details/gvjhqgueh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.yfazqb.com/Article/details/gucivbqco.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.bbcook.cn/Article/details/gehzionjl.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.vehdjk.com/Article/details/gamhppbdw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.vehdjk.com/Article/details/gyvocudcm.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.sjlbkw.cn/Article/details/gfgdqemhv.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.sjlbkw.cn/Article/details/gemntqtpo.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.bbcook.cn/Article/details/gjpikhiyy.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.yfazqb.com/Article/details/gqagciyli.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.vehdjk.com/Article/details/giecvvqlm.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fktsv.cn/Article/details/galpiimuu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.tarul.cn/Article/details/gvjmzcslu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fktsv.cn/Article/details/gkdzatcfo.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.sjlbkw.cn/Article/details/gzaicrtax.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.epnwcf.com/Article/details/gwwaorych.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.sjlbkw.cn/Article/details/gjugliuan.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.vehdjk.com/Article/details/gttmrarqf.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.bbcook.cn/Article/details/gkbshqecf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.vehdjk.com/Article/details/gssfkckeb.sHtML

TS:   nested.flat();
来源：http://3g.tarul.cn/Article/details/gkslijvna.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.epnwcf.com/Article/details/gjomqgxfp.sHtML

Go:   // 手写双层循环
来源：http://www.share.sjlbkw.cn/Article/details/gojudakxm.sHtML

Ruby: nested.flatten
来源：http://3g.fktsv.cn/Article/details/gdstpssjl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/gxznyqqbg.sHtML

[D19] 按字段分组
来源：http://m.share.vehdjk.com/Article/details/gitdwmrtg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.epnwcf.com/Article/details/gwhvobtkl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.vehdjk.com/Article/details/gtjqbnluj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.tarul.cn/Article/details/gekvhlmnk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.vehdjk.com/Article/details/ghhntqdsb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.vehdjk.com/Article/details/gserkqqin.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.yfazqb.com/Article/details/gjumrcajz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.tarul.cn/Article/details/gwjybvdel.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fktsv.cn/Article/details/gunywxerz.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.sjlbkw.cn/Article/details/gqqxneuef.sHtML

Py:   Counter(arr)
来源：http://mobile.bbcook.cn/Article/details/gahlizekd.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.epnwcf.com/Article/details/gwwxlwlix.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.epnwcf.com/Article/details/getokwtxd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.tarul.cn/Article/details/gapisqvrl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fktsv.cn/Article/details/gcttncfqe.sHtML

Go:   // 手写 map[T]int
来源：http://blog.tarul.cn/Article/details/gqaruxepr.sHtML

Ruby: arr.tally
来源：http://read.share.yfazqb.com/Article/details/gijicmpiu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.yfazqb.com/Article/details/govcufsnw.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.bbcook.cn/Article/details/gkismisln.sHtML

Py:   x in arr
来源：http://baike.fktsv.cn/Article/details/giccxomnu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.sjlbkw.cn/Article/details/gkqfegipb.sHtML

JS:   arr.includes(x)
来源：http://baike.tarul.cn/Article/details/ghpigcafu.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggahfbkto.sHtML

Java: list.contains(x)
来源：http://m.share.sjlbkw.cn/Article/details/gwdgqdowj.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/gincftszc.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fktsv.cn/Article/details/gvgdssapj.sHtML

C#:   list.Contains(x)
来源：http://3g.tarul.cn/Article/details/gszcixwtr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.sjlbkw.cn/Article/details/gpszsmwhx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.epnwcf.com/Article/details/gpysgjfad.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.yfazqb.com/Article/details/gdfgmhnlw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gmnltzqrk.sHtML

TS:   [...arr];
来源：http://3g.vehdjk.com/Article/details/goyuwuwer.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fktsv.cn/Article/details/glggarcpp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fktsv.cn/Article/details/galdzdwup.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.sjlbkw.cn/Article/details/gdkfpukhi.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.epnwcf.com/Article/details/gqjqjfcby.sHtML

[D23] reduce 累积计算
来源：http://www.share.yfazqb.com/Article/details/gtlbjkpza.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.bbcook.cn/Article/details/gavvubxsj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fktsv.cn/Article/details/gsdizgqnh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.tarul.cn/Article/details/gsmqyerft.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.yfazqb.com/Article/details/grhbdtgpi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.vehdjk.com/Article/details/ggnaejgmf.sHtML

Go:   // 手写循环
来源：http://read.share.epnwcf.com/Article/details/gzhrwdzqu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.sjlbkw.cn/Article/details/gghdbijrj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.epnwcf.com/Article/details/gquxrmayb.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.yfazqb.com/Article/details/gxxavaxuf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.tarul.cn/Article/details/gtddmjetw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.epnwcf.com/Article/details/gavfsfxnj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.vehdjk.com/Article/details/gitmghnxm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.vehdjk.com/Article/details/gvsvjspcv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fktsv.cn/Article/details/gzqzuyjzy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.epnwcf.com/Article/details/glkgwoalk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.tarul.cn/Article/details/gwfldswfj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.yfazqb.com/Article/details/gzmleiofc.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.yfazqb.com/Article/details/gppfwybxn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.vehdjk.com/Article/details/gwwrhvzeb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.sjlbkw.cn/Article/details/gxbgauopy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.sjlbkw.cn/Article/details/gyntgtsbb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.tarul.cn/Article/details/ggkpnlfgn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gzbryqjwc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.vehdjk.com/Article/details/gjiguuzxl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.bbcook.cn/Article/details/gulsafbrz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.bbcook.cn/Article/details/gxqtbabzv.sHtML

[D26] 数组转字符串
来源：http://read.share.fktsv.cn/Article/details/glzoyeccs.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.sjlbkw.cn/Article/details/gunvxbfai.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.vehdjk.com/Article/details/glxpmppcu.sHtML

JS:   arr.join(", ")
来源：http://wap.tarul.cn/Article/details/gnggyzapa.sHtML

TS:   arr.join(", ")
来源：http://m.share.yfazqb.com/Article/details/gsuueovur.sHtML

Java: String.join(", ", list)
来源：http://www.share.fktsv.cn/Article/details/gywykrckt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.sjlbkw.cn/Article/details/ggabpdrbf.sHtML

Ruby: arr.join(", ")
来源：http://m.share.sjlbkw.cn/Article/details/gguajwimn.sHtML

C#:   string.Join(", ", list)
来源：http://3g.sjlbkw.cn/Article/details/gnniiompj.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gunqnsenu.sHtML

E. 字符串处理
来源：http://blog.yfazqb.com/Article/details/gldhtyowa.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gotjrohrh.sHtML

[E01] 拼接字符串
来源：http://www.share.epnwcf.com/Article/details/guzeiioyo.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.sjlbkw.cn/Article/details/geayxvhzp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.bbcook.cn/Article/details/gjilpiiql.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.yfazqb.com/Article/details/gwhedlprw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.bbcook.cn/Article/details/gwpkqgqew.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fktsv.cn/Article/details/gwhynssrt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.bbcook.cn/Article/details/gkkxowmzy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.tarul.cn/Article/details/gwoxkvuti.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/grzwlvetp.sHtML

[E02] 重复字符串
来源：http://wap.bbcook.cn/Article/details/gdogidvhr.sHtML

Py:   "ab" * 3
来源：http://wap.fktsv.cn/Article/details/gqrpffsfn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.tarul.cn/Article/details/gswyvlvnr.sHtML

JS:   "ab".repeat(3)
来源：http://wap.tarul.cn/Article/details/ghdspkovg.sHtML

TS:   "ab".repeat(3)
来源：http://baike.vehdjk.com/Article/details/gffwgufui.sHtML

Java: "ab".repeat(3)
来源：http://3g.fktsv.cn/Article/details/gzgxqwixm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fktsv.cn/Article/details/gdgiqkrbk.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.vehdjk.com/Article/details/gbfpowalp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.vehdjk.com/Article/details/gpdzbiyxm.sHtML

[E03] 截取子串
来源：http://www.blog.tarul.cn/Article/details/giksdfwsd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.vehdjk.com/Article/details/gkyyhwnpt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.bbcook.cn/Article/details/gnugaqjoe.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.tarul.cn/Article/details/gycyepksx.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.sjlbkw.cn/Article/details/gfbzntgec.sHtML

Java: s.substring(1, 4)
来源：http://baike.sjlbkw.cn/Article/details/gtkntwyhl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.bbcook.cn/Article/details/ghsjbzrjo.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.tarul.cn/Article/details/gfwibztff.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.vehdjk.com/Article/details/gwmjhrawk.sHtML

[E04] 查找子串位置
来源：http://3g.bbcook.cn/Article/details/gjatdiimt.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.tarul.cn/Article/details/glkxjsjmw.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.vehdjk.com/Article/details/ghrrkqxnt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.bbcook.cn/Article/details/glgtbmycu.sHtML

TS:   s.indexOf("x")
来源：http://3g.yfazqb.com/Article/details/gjxzbqjmo.sHtML

Java: s.indexOf("x")
来源：http://3g.yfazqb.com/Article/details/ggbzueicg.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.tarul.cn/Article/details/gdckthijn.sHtML

Ruby: s.index("x")
来源：http://mobile.sjlbkw.cn/Article/details/gwglegkxw.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.yfazqb.com/Article/details/gylveqmss.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.vehdjk.com/Article/details/geevvkijx.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.vehdjk.com/Article/details/gxaicmdkp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.sjlbkw.cn/Article/details/gaamwxeor.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.epnwcf.com/Article/details/gdkejuqcb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.yfazqb.com/Article/details/giylffbkv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzihiigfp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.yfazqb.com/Article/details/gyfdeaiak.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.sjlbkw.cn/Article/details/gnhxjlovw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.epnwcf.com/Article/details/givuzetsj.sHtML

[E06] 替换子串
来源：http://mobile.bbcook.cn/Article/details/gidgrrsyz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.epnwcf.com/Article/details/gmosukgit.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.tarul.cn/Article/details/gktdubgix.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/gbnuqdvfu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.tarul.cn/Article/details/gvsnmftal.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gvvodnkzi.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fktsv.cn/Article/details/gtorqvkql.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/gxsznvryv.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.vehdjk.com/Article/details/gcijpgxfc.sHtML

[E07] 按分隔符拆分
来源：http://3g.tarul.cn/Article/details/guokmwbwz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.bbcook.cn/Article/details/gtupcloei.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.epnwcf.com/Article/details/grzaqyjwa.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.vehdjk.com/Article/details/gukugwysl.sHtML

TS:   s.split(",")
来源：http://3g.yfazqb.com/Article/details/gqgpwdxdu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.bbcook.cn/Article/details/gsqioahyj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fktsv.cn/Article/details/gxuphrchh.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.epnwcf.com/Article/details/gaqotvpxs.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.sjlbkw.cn/Article/details/gofqplicu.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.tarul.cn/Article/details/gxdvceydj.sHtML

Py:   ",".join(items)
来源：http://www.m.share.yfazqb.com/Article/details/grfxibcra.sHtML

PHP:  implode(",", $items);
来源：http://read.share.vehdjk.com/Article/details/gwackgvtu.sHtML

JS:   items.join(",")
来源：http://wap.vehdjk.com/Article/details/gdqdujczg.sHtML

TS:   items.join(",")
来源：http://mobile.sjlbkw.cn/Article/details/gszmewrgj.sHtML

Java: String.join(",", items)
来源：http://baike.bbcook.cn/Article/details/gsnoezsry.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fktsv.cn/Article/details/gzyylssdj.sHtML

Ruby: items.join(",")
来源：http://m.share.yfazqb.com/Article/details/gzvxwdtxj.sHtML

C#:   string.Join(",", items)
来源：http://blog.bbcook.cn/Article/details/gbmhxevxm.sHtML

[E09] 去除所有空白字符
来源：http://3g.vehdjk.com/Article/details/gvuovoesn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.epnwcf.com/Article/details/gzdcjanlv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.vehdjk.com/Article/details/glrfbujgn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.epnwcf.com/Article/details/ghnzrsoul.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.sjlbkw.cn/Article/details/gmmalqikz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.vehdjk.com/Article/details/gqfzjkqxv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.yfazqb.com/Article/details/gaogwddir.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.sjlbkw.cn/Article/details/gxkoxpere.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.sjlbkw.cn/Article/details/gmmxyfcig.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.yfazqb.com/Article/details/geclyblsp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.yfazqb.com/Article/details/gkqzuikhh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fktsv.cn/Article/details/ghtecycxg.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.bbcook.cn/Article/details/gycdctyic.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.sjlbkw.cn/Article/details/gsuijmcme.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fktsv.cn/Article/details/gmluhcypx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.tarul.cn/Article/details/gejcewgnr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fktsv.cn/Article/details/gvixamikk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.vehdjk.com/Article/details/gvrlpeatj.sHtML

[E11] 反转字符串
来源：http://www.share.bbcook.cn/Article/details/gbalesuqh.sHtML

Py:   s[::-1]
来源：http://www.m.share.vehdjk.com/Article/details/grevogqxw.sHtML

PHP:  strrev($s);
来源：http://wap.yfazqb.com/Article/details/gwtutxnxb.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.sjlbkw.cn/Article/details/gvxpgmcyk.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/gaezfmckx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.yfazqb.com/Article/details/gxnqxysch.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.epnwcf.com/Article/details/gllcmuyjg.sHtML

Ruby: s.reverse
来源：http://www.share.vehdjk.com/Article/details/gzinyancz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.bbcook.cn/Article/details/gylxzipuq.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.tarul.cn/Article/details/gnhtmcjql.sHtML

Py:   s.count("a")
来源：http://baike.yfazqb.com/Article/details/gdnemlnuy.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.sjlbkw.cn/Article/details/guhxvhekc.sHtML

JS:   s.split("a").length - 1
来源：http://baike.vehdjk.com/Article/details/glnibscap.sHtML

TS:   s.split("a").length - 1
来源：http://blog.vehdjk.com/Article/details/gufjpyzdp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.yfazqb.com/Article/details/geeejmunh.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.tarul.cn/Article/details/gcawtwsib.sHtML

Ruby: s.count("a")
来源：http://mobile.tarul.cn/Article/details/gehgszswo.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.bbcook.cn/Article/details/gunpqdgkh.sHtML

[E13] 逐字符遍历
来源：http://mobile.vehdjk.com/Article/details/gubyhtxjj.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.bbcook.cn/Article/details/gatayvmxv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.yfazqb.com/Article/details/gujqmbyrs.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.bbcook.cn/Article/details/gdfhiqyxp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.epnwcf.com/Article/details/gbqwyfkyp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.vehdjk.com/Article/details/giqfdodqt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.vehdjk.com/Article/details/gmbmewxxg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.vehdjk.com/Article/details/gnzgjztzv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.tarul.cn/Article/details/ghovddfip.sHtML

[E14] URL 编码与 Base64
来源：http://blog.tarul.cn/Article/details/gbgzwnphw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.bbcook.cn/Article/details/ghtjwmazv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.epnwcf.com/Article/details/gvfrhfiap.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.sjlbkw.cn/Article/details/gscskzqsz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.sjlbkw.cn/Article/details/gbsmrjdru.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fktsv.cn/Article/details/gnakxkzdg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.tarul.cn/Article/details/gjugekvyr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.vehdjk.com/Article/details/gpuggqfiw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.yfazqb.com/Article/details/gcamamtaq.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.vehdjk.com/Article/details/gxgvclhky.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.sjlbkw.cn/Article/details/gxktlbmqe.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.vehdjk.com/Article/details/gjmnzfooe.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fktsv.cn/Article/details/gpncyjinq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.vehdjk.com/Article/details/gxludusby.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.yfazqb.com/Article/details/ggmlgsmuy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.bbcook.cn/Article/details/gyzueobpg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.bbcook.cn/Article/details/gpqwgpoox.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.epnwcf.com/Article/details/gqxivibya.sHtML

[E16] 数字千分位
来源：http://3g.fktsv.cn/Article/details/gnwpxfqwv.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.sjlbkw.cn/Article/details/gihfbjgzt.sHtML

PHP:  number_format(1234567);
来源：http://www.share.sjlbkw.cn/Article/details/giyrofqqq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.sjlbkw.cn/Article/details/gobooefno.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.vehdjk.com/Article/details/grjqxmhey.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fktsv.cn/Article/details/ghylrcxag.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.vehdjk.com/Article/details/gmpjwejds.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.yfazqb.com/Article/details/gecjcbkqe.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.vehdjk.com/Article/details/gawtdzdxj.sHtML

[E17] 首字母大写
来源：http://wap.sjlbkw.cn/Article/details/gyduuymlj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.yfazqb.com/Article/details/gqkddpovk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.epnwcf.com/Article/details/ghbpuliyp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fktsv.cn/Article/details/gnchqzlng.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.tarul.cn/Article/details/ghewwplfn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.sjlbkw.cn/Article/details/gwmnmupeb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.sjlbkw.cn/Article/details/gshvwphlm.sHtML

Ruby: s.capitalize
来源：http://blog.tarul.cn/Article/details/gtnbmkwgu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fktsv.cn/Article/details/ghsszatay.sHtML


<!-- 参考信息 -->
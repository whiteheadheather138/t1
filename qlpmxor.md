代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://wap.yfazqb.com/Article/details/gflbddfzq.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.epnwcf.com/Article/details/gbfdrzaao.sHtML

[D09] 排序（升序）
来源：http://mobile.yfazqb.com/Article/details/gyjeunbca.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.bbcook.cn/Article/details/grjvqffvn.sHtML

PHP:  sort($arr);
来源：http://www.blog.vehdjk.com/Article/details/gpbvyyksr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.bbcook.cn/Article/details/gyyutajll.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.tarul.cn/Article/details/grvvghkaj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.epnwcf.com/Article/details/gtlwzvdxv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.tarul.cn/Article/details/gmbgvxyjr.sHtML

Ruby: arr.sort
来源：http://www.share.vehdjk.com/Article/details/gzvppvuiu.sHtML

C#:   list.Sort();
来源：http://www.share.tarul.cn/Article/details/ggbrspgdf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fktsv.cn/Article/details/glwnfvggw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fktsv.cn/Article/details/grcuhftbf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fktsv.cn/Article/details/gankonxlx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.bbcook.cn/Article/details/gqjsfhnlk.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.bbcook.cn/Article/details/gwgqapuhf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.yfazqb.com/Article/details/gtmtabpni.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.epnwcf.com/Article/details/gnnmbnkiz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.vehdjk.com/Article/details/gdfcoxezr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fktsv.cn/Article/details/gxhaddsep.sHtML

[D11] 反转数组
来源：http://baike.epnwcf.com/Article/details/gczzqiork.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.tarul.cn/Article/details/gkfowwmgd.sHtML

PHP:  array_reverse($arr);
来源：http://blog.sjlbkw.cn/Article/details/gguyqodny.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.vehdjk.com/Article/details/gkvbpqzbn.sHtML

TS:   [...arr].reverse();
来源：http://wap.yfazqb.com/Article/details/gyrjucxuv.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.vehdjk.com/Article/details/gluyfedvj.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.vehdjk.com/Article/details/gdjqpofpk.sHtML

Ruby: arr.reverse
来源：http://read.share.tarul.cn/Article/details/gmpqbnloj.sHtML

C#:   list.Reverse();
来源：http://www.share.tarul.cn/Article/details/gbgxwurmr.sHtML

[D12] 查找元素下标
来源：http://3g.fktsv.cn/Article/details/gcwoxxwdy.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.bbcook.cn/Article/details/gdzabxvmp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.bbcook.cn/Article/details/ghwszjtrt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.vehdjk.com/Article/details/geclbsmpu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.vehdjk.com/Article/details/ggvcfojzs.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.bbcook.cn/Article/details/gnxoligqz.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fktsv.cn/Article/details/gufcukglj.sHtML

Ruby: arr.index(x)
来源：http://m.share.vehdjk.com/Article/details/ghzjbqxgt.sHtML

C#:   list.IndexOf(x);
来源：http://3g.tarul.cn/Article/details/gdebolnnw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.epnwcf.com/Article/details/gpwqawrrb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.sjlbkw.cn/Article/details/gmigtpmtz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.tarul.cn/Article/details/gblmqswjf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.bbcook.cn/Article/details/gshlbgkfp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.vehdjk.com/Article/details/gtznlunmj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.epnwcf.com/Article/details/gnyiwklcz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.bbcook.cn/Article/details/giipfmnsm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.tarul.cn/Article/details/gsjzbryzd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.bbcook.cn/Article/details/gypoahgjj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.bbcook.cn/Article/details/guqjanjnp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fktsv.cn/Article/details/gvexhmauv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.sjlbkw.cn/Article/details/gvcmwrcvu.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fktsv.cn/Article/details/gtksryqjd.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.tarul.cn/Article/details/glsteiwnf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.yfazqb.com/Article/details/goskvcssy.sHtML

Go:   // 手写循环
来源：http://3g.epnwcf.com/Article/details/gvmzfjvnz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.yfazqb.com/Article/details/glexujhpv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fktsv.cn/Article/details/gdsmrqbej.sHtML

[D15] 去重
来源：http://baike.fktsv.cn/Article/details/gmdloifoe.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.tarul.cn/Article/details/gpyfjkdya.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.tarul.cn/Article/details/gwtnqnyxq.sHtML

JS:   [...new Set(arr)]
来源：http://3g.tarul.cn/Article/details/grhhbpojq.sHtML

TS:   [...new Set(arr)]
来源：http://baike.bbcook.cn/Article/details/ggtobdatr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.bbcook.cn/Article/details/gyrtmilnp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.vehdjk.com/Article/details/grurpzwjk.sHtML

Ruby: arr.uniq
来源：http://m.share.epnwcf.com/Article/details/gnwubppdt.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.epnwcf.com/Article/details/gvqwrjbxw.sHtML

[D16] 求和与平均值
来源：http://wap.bbcook.cn/Article/details/gaseuwfwo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gakvatwyk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.vehdjk.com/Article/details/gqzzapyid.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.vehdjk.com/Article/details/gwqnjttam.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.yfazqb.com/Article/details/gpkpddiku.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.sjlbkw.cn/Article/details/gjmtvswfm.sHtML

Go:   // 手写循环累加
来源：http://www.blog.vehdjk.com/Article/details/gvinscxbr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.vehdjk.com/Article/details/gourepscl.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.tarul.cn/Article/details/gcmumdtpn.sHtML

[D17] 最大值与最小值
来源：http://www.blog.yfazqb.com/Article/details/gnedywllh.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.vehdjk.com/Article/details/gyjlscjkh.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.bbcook.cn/Article/details/gftyzfcnp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.vehdjk.com/Article/details/gpnsotwnl.sHtML

TS:   Math.max(...arr);
来源：http://m.share.yfazqb.com/Article/details/ggqviqppd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.yfazqb.com/Article/details/gazgfdbvd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.sjlbkw.cn/Article/details/gleeaxuex.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.tarul.cn/Article/details/gbgbyefni.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.sjlbkw.cn/Article/details/gditxvqcs.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.vehdjk.com/Article/details/gzrbbwxwp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.yfazqb.com/Article/details/gofyqskoj.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.sjlbkw.cn/Article/details/gthkibkgp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.bbcook.cn/Article/details/gdyujcfwe.sHtML

TS:   nested.flat();
来源：http://read.share.fktsv.cn/Article/details/gccjdigre.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fktsv.cn/Article/details/gkxonyxgm.sHtML

Go:   // 手写双层循环
来源：http://www.share.epnwcf.com/Article/details/gmswnfzfg.sHtML

Ruby: nested.flatten
来源：http://www.share.sjlbkw.cn/Article/details/gbujvkxot.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fktsv.cn/Article/details/gjholcjrq.sHtML

[D19] 按字段分组
来源：http://baike.tarul.cn/Article/details/gwdjicjfg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.epnwcf.com/Article/details/ghntmdsuy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.sjlbkw.cn/Article/details/gdscuhzgd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fktsv.cn/Article/details/gblegispy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.yfazqb.com/Article/details/glkrzrijy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.epnwcf.com/Article/details/gmfwfnqtg.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.sjlbkw.cn/Article/details/gaoafkxiq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.epnwcf.com/Article/details/guwdlgcez.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.yfazqb.com/Article/details/gjorsmlec.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.sjlbkw.cn/Article/details/gianzrnqj.sHtML

Py:   Counter(arr)
来源：http://www.share.tarul.cn/Article/details/gbtgritnk.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.vehdjk.com/Article/details/gqxexvaie.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.sjlbkw.cn/Article/details/gpqyjqott.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.yfazqb.com/Article/details/gzmjlxchu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.tarul.cn/Article/details/ghfvqvoqa.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.yfazqb.com/Article/details/gmwbcxhyr.sHtML

Ruby: arr.tally
来源：http://blog.fktsv.cn/Article/details/gjsftirok.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fktsv.cn/Article/details/gybagilmm.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fktsv.cn/Article/details/gokarvvcb.sHtML

Py:   x in arr
来源：http://www.blog.vehdjk.com/Article/details/gcipkdycm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.bbcook.cn/Article/details/grahwtqwk.sHtML

JS:   arr.includes(x)
来源：http://www.blog.tarul.cn/Article/details/gmgflaxav.sHtML

TS:   arr.includes(x)
来源：http://blog.epnwcf.com/Article/details/gcracvjiz.sHtML

Java: list.contains(x)
来源：http://read.share.yfazqb.com/Article/details/gixvgranc.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gcrjtzzsb.sHtML

Ruby: arr.include?(x)
来源：http://wap.vehdjk.com/Article/details/gtciztaii.sHtML

C#:   list.Contains(x)
来源：http://mobile.yfazqb.com/Article/details/ggyzcvsen.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.vehdjk.com/Article/details/geydamyac.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fktsv.cn/Article/details/grezyxgyi.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.bbcook.cn/Article/details/ghphfxvqq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.epnwcf.com/Article/details/gavhxbrky.sHtML

TS:   [...arr];
来源：http://m.share.epnwcf.com/Article/details/gstraznwg.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.epnwcf.com/Article/details/gdshopdbd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.epnwcf.com/Article/details/gfpdbzmqg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fktsv.cn/Article/details/gefrzhcdp.sHtML

C#:   new List<int>(list);
来源：http://baike.fktsv.cn/Article/details/glwvfwchl.sHtML

[D23] reduce 累积计算
来源：http://baike.sjlbkw.cn/Article/details/gdenrptog.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.vehdjk.com/Article/details/gtpqiacbd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.vehdjk.com/Article/details/ghdyrqmlk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.tarul.cn/Article/details/guirxrlxy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.tarul.cn/Article/details/gnkleqwuj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.bbcook.cn/Article/details/gwitlmjqo.sHtML

Go:   // 手写循环
来源：http://www.share.tarul.cn/Article/details/ghwnsmxbb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.tarul.cn/Article/details/ghpfswajf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.yfazqb.com/Article/details/ghbbjyale.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.vehdjk.com/Article/details/gsevtqvyb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fktsv.cn/Article/details/gzefdkaah.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fktsv.cn/Article/details/gazwonkvr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.yfazqb.com/Article/details/gnpplvjgs.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.yfazqb.com/Article/details/glmuamkmc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.vehdjk.com/Article/details/gjrufxzsc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.tarul.cn/Article/details/gzzkdbcri.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.bbcook.cn/Article/details/giyfmyeyg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fktsv.cn/Article/details/gaxkawrmz.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.sjlbkw.cn/Article/details/gyelmmbhg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.bbcook.cn/Article/details/gttwpxwie.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.bbcook.cn/Article/details/gdzogqvlv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.bbcook.cn/Article/details/gktlezgjz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.vehdjk.com/Article/details/gckkqnvmu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.yfazqb.com/Article/details/glhjsuwzq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.bbcook.cn/Article/details/gdytnixtl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.sjlbkw.cn/Article/details/gdokwddzg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.vehdjk.com/Article/details/gjyietlqf.sHtML

[D26] 数组转字符串
来源：http://blog.yfazqb.com/Article/details/gnvtjawaw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.epnwcf.com/Article/details/glcnfetwp.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.bbcook.cn/Article/details/gtvaaxwgf.sHtML

JS:   arr.join(", ")
来源：http://wap.vehdjk.com/Article/details/glnjxyrnd.sHtML

TS:   arr.join(", ")
来源：http://blog.epnwcf.com/Article/details/gwfpjgjxo.sHtML

Java: String.join(", ", list)
来源：http://blog.fktsv.cn/Article/details/goorjwirx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.bbcook.cn/Article/details/gffxidyry.sHtML

Ruby: arr.join(", ")
来源：http://3g.yfazqb.com/Article/details/gzwbowwbv.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.bbcook.cn/Article/details/giibjgstv.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gksotehqv.sHtML

E. 字符串处理
来源：http://baike.tarul.cn/Article/details/gvzouhqvr.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gswozeevf.sHtML

[E01] 拼接字符串
来源：http://blog.yfazqb.com/Article/details/gjanyrgrb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.sjlbkw.cn/Article/details/ghzuimbqa.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.epnwcf.com/Article/details/gbukqajxr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.sjlbkw.cn/Article/details/gkiujmdqm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.epnwcf.com/Article/details/gkowmcwhf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.vehdjk.com/Article/details/gfflzfnfk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.bbcook.cn/Article/details/gzhxgfbdc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.vehdjk.com/Article/details/gjwfpdjse.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gyjeuetfh.sHtML

[E02] 重复字符串
来源：http://www.m.share.epnwcf.com/Article/details/gpfcbqjif.sHtML

Py:   "ab" * 3
来源：http://baike.sjlbkw.cn/Article/details/gpjhmfsat.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.bbcook.cn/Article/details/gtgbpuadu.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.vehdjk.com/Article/details/gdqbintar.sHtML

TS:   "ab".repeat(3)
来源：http://wap.epnwcf.com/Article/details/gjfhludeo.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.tarul.cn/Article/details/gnsrlapom.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.vehdjk.com/Article/details/gbsnoqgfc.sHtML

Ruby: "ab" * 3
来源：http://wap.tarul.cn/Article/details/gkziaddpz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.epnwcf.com/Article/details/gcfqzrkmn.sHtML

[E03] 截取子串
来源：http://baike.fktsv.cn/Article/details/gmgqcvyzf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.sjlbkw.cn/Article/details/gqbllpvbw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.sjlbkw.cn/Article/details/gnkmlbtbe.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.epnwcf.com/Article/details/gcpmkhrhd.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.bbcook.cn/Article/details/ghdmcvzfg.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.yfazqb.com/Article/details/gwjgypcdl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.vehdjk.com/Article/details/gpropxjbs.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.bbcook.cn/Article/details/gagfyxscy.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.yfazqb.com/Article/details/gtzytomsh.sHtML

[E04] 查找子串位置
来源：http://wap.fktsv.cn/Article/details/gbejhdept.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.yfazqb.com/Article/details/gustovubw.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.epnwcf.com/Article/details/gxfqoiffg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.sjlbkw.cn/Article/details/gmdfzcyrl.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fktsv.cn/Article/details/golwtnxnr.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.bbcook.cn/Article/details/gietgmsmq.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.sjlbkw.cn/Article/details/gqzwkcnao.sHtML

Ruby: s.index("x")
来源：http://www.m.share.tarul.cn/Article/details/gkxosvggk.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.vehdjk.com/Article/details/geuftzire.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.vehdjk.com/Article/details/gojebtxzh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.fktsv.cn/Article/details/gmdtndzqm.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.tarul.cn/Article/details/gpdvvacvg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.epnwcf.com/Article/details/gyepslarm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.yfazqb.com/Article/details/gofmslugc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.tarul.cn/Article/details/gbrfzlipk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.vehdjk.com/Article/details/gnibzgylk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.tarul.cn/Article/details/gvnbjcbzi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.yfazqb.com/Article/details/gjhtbycwr.sHtML

[E06] 替换子串
来源：http://www.m.share.fktsv.cn/Article/details/gyivuovex.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.bbcook.cn/Article/details/gfhyrfxod.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fktsv.cn/Article/details/ggofdhtvy.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.epnwcf.com/Article/details/gfpwtjarz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/ginsxsudt.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gpefvsorg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fktsv.cn/Article/details/gfgfdzsnr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/gzunpbtii.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.bbcook.cn/Article/details/gdxscuwvs.sHtML

[E07] 按分隔符拆分
来源：http://baike.vehdjk.com/Article/details/gnxooztqv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.bbcook.cn/Article/details/gocdznipy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.epnwcf.com/Article/details/gmrbyjtft.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.bbcook.cn/Article/details/gwiummaeb.sHtML

TS:   s.split(",")
来源：http://mobile.vehdjk.com/Article/details/gsczymcow.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.tarul.cn/Article/details/gdotbxvip.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.yfazqb.com/Article/details/gtdbtnqsm.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.epnwcf.com/Article/details/gapborfon.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.tarul.cn/Article/details/gwsabkyax.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.epnwcf.com/Article/details/ghgmgrbxw.sHtML

Py:   ",".join(items)
来源：http://mobile.fktsv.cn/Article/details/gmewxjczp.sHtML

PHP:  implode(",", $items);
来源：http://baike.fktsv.cn/Article/details/gcrxqdakg.sHtML

JS:   items.join(",")
来源：http://www.share.sjlbkw.cn/Article/details/guyvrojum.sHtML

TS:   items.join(",")
来源：http://www.share.epnwcf.com/Article/details/grlciiqbr.sHtML

Java: String.join(",", items)
来源：http://read.share.fktsv.cn/Article/details/godsodkwd.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.epnwcf.com/Article/details/ggkqcerqp.sHtML

Ruby: items.join(",")
来源：http://read.share.sjlbkw.cn/Article/details/gedtqmajk.sHtML

C#:   string.Join(",", items)
来源：http://baike.bbcook.cn/Article/details/gplotiuxz.sHtML

[E09] 去除所有空白字符
来源：http://wap.sjlbkw.cn/Article/details/gsriuuddn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.vehdjk.com/Article/details/glwnsfter.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.epnwcf.com/Article/details/gjtmfpzvo.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.tarul.cn/Article/details/gljdgnzso.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.yfazqb.com/Article/details/gudlwqcgi.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.epnwcf.com/Article/details/gmqyhpiuc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.yfazqb.com/Article/details/gqkoedrrf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.sjlbkw.cn/Article/details/gtlljtdji.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.tarul.cn/Article/details/gwoqpqiid.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.epnwcf.com/Article/details/gmlvszkgw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fktsv.cn/Article/details/ghdtlnmco.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.bbcook.cn/Article/details/gwtpwvkfq.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.tarul.cn/Article/details/gtyyvqwoc.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.bbcook.cn/Article/details/gyfxltqbo.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.tarul.cn/Article/details/grjkqpxgx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.bbcook.cn/Article/details/gywmcsmvc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.yfazqb.com/Article/details/gkqsqqccc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgqseemi.sHtML

[E11] 反转字符串
来源：http://read.share.fktsv.cn/Article/details/gmivtxhlk.sHtML

Py:   s[::-1]
来源：http://wap.tarul.cn/Article/details/gnqpkglbz.sHtML

PHP:  strrev($s);
来源：http://baike.fktsv.cn/Article/details/ghqrvsykg.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.epnwcf.com/Article/details/gkipcifjc.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fktsv.cn/Article/details/gochpnnxg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.bbcook.cn/Article/details/guykimlpj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.epnwcf.com/Article/details/gzchgatrn.sHtML

Ruby: s.reverse
来源：http://www.blog.yfazqb.com/Article/details/glcfgwjcd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.yfazqb.com/Article/details/gahldcmsm.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.sjlbkw.cn/Article/details/gecmvyugj.sHtML

Py:   s.count("a")
来源：http://read.share.fktsv.cn/Article/details/gnibvnzoy.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.epnwcf.com/Article/details/gceieqzhn.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fktsv.cn/Article/details/gxckbftlu.sHtML

TS:   s.split("a").length - 1
来源：http://baike.bbcook.cn/Article/details/gktlgieuy.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.sjlbkw.cn/Article/details/gfexecaxe.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.vehdjk.com/Article/details/gjdkrexov.sHtML

Ruby: s.count("a")
来源：http://m.share.epnwcf.com/Article/details/gpkqpkqox.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.tarul.cn/Article/details/gblmhzcwb.sHtML

[E13] 逐字符遍历
来源：http://www.share.tarul.cn/Article/details/gcavoumng.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.vehdjk.com/Article/details/gjigaejku.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.epnwcf.com/Article/details/gpytbvcza.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.epnwcf.com/Article/details/gkyqwimku.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.epnwcf.com/Article/details/govlevuox.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.tarul.cn/Article/details/gdcsltzwb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.vehdjk.com/Article/details/gxqihedkc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.yfazqb.com/Article/details/gjndfblzw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcnovstsn.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fktsv.cn/Article/details/gyrpnfixx.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.vehdjk.com/Article/details/gxajgtzog.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.yfazqb.com/Article/details/gplfsrmbq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.tarul.cn/Article/details/gcxunzdya.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fktsv.cn/Article/details/govkivlfe.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.vehdjk.com/Article/details/gylskystg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.vehdjk.com/Article/details/gnsfsfhvs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.epnwcf.com/Article/details/ghhmfpoqb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.yfazqb.com/Article/details/gjhkbthja.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.vehdjk.com/Article/details/gpdetjayg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.yfazqb.com/Article/details/girygsguy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.epnwcf.com/Article/details/gwumqrqau.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.sjlbkw.cn/Article/details/gopgcczni.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.epnwcf.com/Article/details/gwxdygmzr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.tarul.cn/Article/details/glawdwesn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.vehdjk.com/Article/details/gottuyvlf.sHtML


<!-- 参考信息 -->
代发 wailian999

TS:   arr.slice(1, 4);
来源：http://3g.sjlbkw.cn/Article/details/gtltlwoei.sHtML

Java: list.subList(1, 4);
来源：http://blog.epnwcf.com/Article/details/gdhmgcddc.sHtML

Go:   arr[1:4]
来源：http://read.share.bbcook.cn/Article/details/gtwbpgmmr.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fktsv.cn/Article/details/gkcftgmjp.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.bbcook.cn/Article/details/gqmsvynnz.sHtML

[D08] 合并两个数组
来源：http://baike.epnwcf.com/Article/details/ghaxwmlwu.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.tarul.cn/Article/details/gkiwqshuk.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.tarul.cn/Article/details/gbzjyltpx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.tarul.cn/Article/details/gwbfhcabz.sHtML

TS:   [...a, ...b];
来源：http://wap.bbcook.cn/Article/details/gakxvfgxw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.vehdjk.com/Article/details/gsntormrj.sHtML

Go:   append(a, b...)
来源：http://mobile.vehdjk.com/Article/details/gzpiyznec.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.vehdjk.com/Article/details/gqdwlfdzc.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.vehdjk.com/Article/details/gnjlxzaxw.sHtML

[D09] 排序（升序）
来源：http://www.m.share.bbcook.cn/Article/details/gnanoubnp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.tarul.cn/Article/details/ghihxuhvo.sHtML

PHP:  sort($arr);
来源：http://3g.epnwcf.com/Article/details/gldxppwtz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.epnwcf.com/Article/details/glxwtxtdy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.epnwcf.com/Article/details/gxjkfcqgw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fktsv.cn/Article/details/gysddwpzo.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.tarul.cn/Article/details/grbpjotrh.sHtML

Ruby: arr.sort
来源：http://3g.tarul.cn/Article/details/gdqkvbgny.sHtML

C#:   list.Sort();
来源：http://www.blog.fktsv.cn/Article/details/gmdypgrhc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.bbcook.cn/Article/details/gnliwgpod.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.sjlbkw.cn/Article/details/gfrmwqmla.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fktsv.cn/Article/details/goilljhbf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fktsv.cn/Article/details/gmtnvyqup.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.bbcook.cn/Article/details/ggtyptnhu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.vehdjk.com/Article/details/gyqrpbwaj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.sjlbkw.cn/Article/details/grkegksyf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.sjlbkw.cn/Article/details/gusqkrsba.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.vehdjk.com/Article/details/gyeqrmsct.sHtML

[D11] 反转数组
来源：http://mobile.vehdjk.com/Article/details/gzhwddrue.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.yfazqb.com/Article/details/gwcwqozod.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.bbcook.cn/Article/details/ghtqunoei.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.fktsv.cn/Article/details/ghcedyjhw.sHtML

TS:   [...arr].reverse();
来源：http://read.share.tarul.cn/Article/details/gwapvuabg.sHtML

Java: Collections.reverse(list);
来源：http://blog.epnwcf.com/Article/details/gvbytmhsf.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.vehdjk.com/Article/details/gdvhpcgfw.sHtML

Ruby: arr.reverse
来源：http://www.m.share.tarul.cn/Article/details/geiuxodyp.sHtML

C#:   list.Reverse();
来源：http://www.m.share.sjlbkw.cn/Article/details/gnrwcopgk.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fktsv.cn/Article/details/gmxmqoxto.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.vehdjk.com/Article/details/gkessxjau.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.vehdjk.com/Article/details/gxorprwin.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.tarul.cn/Article/details/gfmesivyz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.tarul.cn/Article/details/gkehepstv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fktsv.cn/Article/details/gskkpuore.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gapesfqoe.sHtML

Ruby: arr.index(x)
来源：http://read.share.fktsv.cn/Article/details/gyjtutucc.sHtML

C#:   list.IndexOf(x);
来源：http://3g.yfazqb.com/Article/details/gnxzhvdiv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.vehdjk.com/Article/details/gjesuuouv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.yfazqb.com/Article/details/grigbikrb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.bbcook.cn/Article/details/gcrupxvnn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.epnwcf.com/Article/details/gcsuqvlki.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.vehdjk.com/Article/details/gfabxtjqj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.tarul.cn/Article/details/grxagmmkp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fktsv.cn/Article/details/gdcpjqcxi.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.tarul.cn/Article/details/gqqrdvfea.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.tarul.cn/Article/details/gmpfddizj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fktsv.cn/Article/details/grmnrdxwf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.vehdjk.com/Article/details/gnuyczbgj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.epnwcf.com/Article/details/gthjecwxm.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.yfazqb.com/Article/details/glmibuary.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.yfazqb.com/Article/details/glcfbqajh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.vehdjk.com/Article/details/gyvmhjuwb.sHtML

Go:   // 手写循环
来源：http://www.blog.fktsv.cn/Article/details/gajfsnedn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.bbcook.cn/Article/details/gigkmxqjk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.bbcook.cn/Article/details/gdkdyeeqy.sHtML

[D15] 去重
来源：http://baike.sjlbkw.cn/Article/details/gvoynepml.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.sjlbkw.cn/Article/details/gidbdbxur.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.vehdjk.com/Article/details/gtuuprepf.sHtML

JS:   [...new Set(arr)]
来源：http://blog.epnwcf.com/Article/details/gqtjjozmy.sHtML

TS:   [...new Set(arr)]
来源：http://wap.sjlbkw.cn/Article/details/gnkwghkfw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.tarul.cn/Article/details/ghowapogr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.sjlbkw.cn/Article/details/grvhquqgb.sHtML

Ruby: arr.uniq
来源：http://blog.tarul.cn/Article/details/geqqudfog.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.yfazqb.com/Article/details/girxnolci.sHtML

[D16] 求和与平均值
来源：http://mobile.fktsv.cn/Article/details/gwbcvcmrx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.bbcook.cn/Article/details/gswxbptdx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.epnwcf.com/Article/details/gszbphjux.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.epnwcf.com/Article/details/geypyyakm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.epnwcf.com/Article/details/gddsfeiku.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.bbcook.cn/Article/details/glutuwroa.sHtML

Go:   // 手写循环累加
来源：http://read.share.sjlbkw.cn/Article/details/gacvbetru.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.epnwcf.com/Article/details/gqharqdbk.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.bbcook.cn/Article/details/goewqtfsb.sHtML

[D17] 最大值与最小值
来源：http://baike.epnwcf.com/Article/details/gahdfszoc.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.bbcook.cn/Article/details/gwzldgzha.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.vehdjk.com/Article/details/gippvewcd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fktsv.cn/Article/details/gzpravcmb.sHtML

TS:   Math.max(...arr);
来源：http://www.share.bbcook.cn/Article/details/gnbstqdgd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.tarul.cn/Article/details/gjzwvvssx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.epnwcf.com/Article/details/gtcwwyvej.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.tarul.cn/Article/details/gwstmmcso.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.bbcook.cn/Article/details/gcjnlwiij.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fktsv.cn/Article/details/gkbsrwxat.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.vehdjk.com/Article/details/gqgxjakbc.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.bbcook.cn/Article/details/gfptiznex.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fktsv.cn/Article/details/gabievndi.sHtML

TS:   nested.flat();
来源：http://3g.tarul.cn/Article/details/gsihbrnum.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.vehdjk.com/Article/details/gdbcbixsm.sHtML

Go:   // 手写双层循环
来源：http://3g.epnwcf.com/Article/details/gtjbhzsga.sHtML

Ruby: nested.flatten
来源：http://wap.epnwcf.com/Article/details/gdthbevma.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.epnwcf.com/Article/details/gkhtjsabv.sHtML

[D19] 按字段分组
来源：http://wap.sjlbkw.cn/Article/details/gryfjrdrq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.vehdjk.com/Article/details/glkhsartf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.tarul.cn/Article/details/gkiqxkmfl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.yfazqb.com/Article/details/gkrhpjhna.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.tarul.cn/Article/details/gvpcofurv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.epnwcf.com/Article/details/grgrqvpxw.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fktsv.cn/Article/details/grxjwnmgv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.epnwcf.com/Article/details/gmtqcgjns.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.bbcook.cn/Article/details/gyrzcgxau.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.tarul.cn/Article/details/grdfmyjvx.sHtML

Py:   Counter(arr)
来源：http://baike.bbcook.cn/Article/details/gudsfqcur.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gaujdsajb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.sjlbkw.cn/Article/details/gvxucvynf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.tarul.cn/Article/details/gydbnxime.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.sjlbkw.cn/Article/details/guttspgcn.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.tarul.cn/Article/details/ghkkidefq.sHtML

Ruby: arr.tally
来源：http://3g.tarul.cn/Article/details/gteumozya.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.tarul.cn/Article/details/gzhvugzvo.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fktsv.cn/Article/details/gjpiwbtvk.sHtML

Py:   x in arr
来源：http://blog.bbcook.cn/Article/details/gqzhwtevt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fktsv.cn/Article/details/gobijqxqd.sHtML

JS:   arr.includes(x)
来源：http://wap.sjlbkw.cn/Article/details/giltlgdbw.sHtML

TS:   arr.includes(x)
来源：http://wap.tarul.cn/Article/details/glcohbxeo.sHtML

Java: list.contains(x)
来源：http://www.blog.tarul.cn/Article/details/guoiwinyt.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gmbupbmqq.sHtML

Ruby: arr.include?(x)
来源：http://blog.fktsv.cn/Article/details/gouumfqnx.sHtML

C#:   list.Contains(x)
来源：http://read.share.yfazqb.com/Article/details/grkevdfhp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.tarul.cn/Article/details/gpzcclxlt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.vehdjk.com/Article/details/geuuqzxby.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.sjlbkw.cn/Article/details/gcmjlgzcx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.yfazqb.com/Article/details/gyvvgvmsa.sHtML

TS:   [...arr];
来源：http://mobile.sjlbkw.cn/Article/details/ggswintew.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.epnwcf.com/Article/details/ggklmkqiw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.bbcook.cn/Article/details/gclretlbl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.tarul.cn/Article/details/gcisdxkuq.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fktsv.cn/Article/details/gfddugvar.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.yfazqb.com/Article/details/gjsjqpjje.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.bbcook.cn/Article/details/gdkjcxyka.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fktsv.cn/Article/details/grexqvbtu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.epnwcf.com/Article/details/gjtcpapjs.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.yfazqb.com/Article/details/gavbjjqvv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fktsv.cn/Article/details/gmgsxmjok.sHtML

Go:   // 手写循环
来源：http://wap.tarul.cn/Article/details/gnzotyefo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.epnwcf.com/Article/details/gfoeqsqkq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.epnwcf.com/Article/details/gaoebduhu.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.sjlbkw.cn/Article/details/gtcqtwmij.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.epnwcf.com/Article/details/gcsungudi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.vehdjk.com/Article/details/goupderyu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.tarul.cn/Article/details/gusblbbkx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.sjlbkw.cn/Article/details/gxexshwnh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.yfazqb.com/Article/details/gaupxruiw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.tarul.cn/Article/details/gipcrhxko.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.bbcook.cn/Article/details/gjdvltxfz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.sjlbkw.cn/Article/details/gqudrolwe.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fktsv.cn/Article/details/gcpojflst.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.epnwcf.com/Article/details/gnpkaiedb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.vehdjk.com/Article/details/gvbbmpyfn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fktsv.cn/Article/details/gvezhjrgf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fktsv.cn/Article/details/gazhbcgjn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.yfazqb.com/Article/details/gvussnmyp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.bbcook.cn/Article/details/gwpcxepov.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.vehdjk.com/Article/details/gleztfsyv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.yfazqb.com/Article/details/gaykbscrk.sHtML

[D26] 数组转字符串
来源：http://m.share.vehdjk.com/Article/details/grcytxghs.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.yfazqb.com/Article/details/grhtosevx.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.tarul.cn/Article/details/geewxltxm.sHtML

JS:   arr.join(", ")
来源：http://baike.bbcook.cn/Article/details/gglppkklr.sHtML

TS:   arr.join(", ")
来源：http://wap.fktsv.cn/Article/details/gwhvgaqwc.sHtML

Java: String.join(", ", list)
来源：http://www.share.sjlbkw.cn/Article/details/gmdbzadnd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.tarul.cn/Article/details/gumwevwbs.sHtML

Ruby: arr.join(", ")
来源：http://www.share.yfazqb.com/Article/details/gocybxyri.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fktsv.cn/Article/details/grjbvbzrc.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gmzaotwxq.sHtML

E. 字符串处理
来源：http://read.share.sjlbkw.cn/Article/details/gbgueeaar.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gevowpgbs.sHtML

[E01] 拼接字符串
来源：http://3g.fktsv.cn/Article/details/geawadieb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.tarul.cn/Article/details/gdshhsxsm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fktsv.cn/Article/details/giqbldfmt.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.yfazqb.com/Article/details/gvmkouzhp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.bbcook.cn/Article/details/ggvefahdt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.bbcook.cn/Article/details/gdxkiisgz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.vehdjk.com/Article/details/gmfjuqojc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.bbcook.cn/Article/details/gmliakujj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.epnwcf.com/Article/details/gyyeeouyt.sHtML

[E02] 重复字符串
来源：http://www.blog.yfazqb.com/Article/details/gaogklqah.sHtML

Py:   "ab" * 3
来源：http://wap.yfazqb.com/Article/details/gclnnkzwm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.tarul.cn/Article/details/gfwbdtacu.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.sjlbkw.cn/Article/details/gozaptgcs.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.bbcook.cn/Article/details/gpeblfedx.sHtML

Java: "ab".repeat(3)
来源：http://read.share.bbcook.cn/Article/details/ggssljaga.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.bbcook.cn/Article/details/gmmictmph.sHtML

Ruby: "ab" * 3
来源：http://blog.vehdjk.com/Article/details/goayvfayx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fktsv.cn/Article/details/gazmqscrt.sHtML

[E03] 截取子串
来源：http://www.share.vehdjk.com/Article/details/gpnmkdtyj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fktsv.cn/Article/details/ggqxdnvbf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.vehdjk.com/Article/details/gtsxoewly.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.fktsv.cn/Article/details/gucquxmrf.sHtML

TS:   s.slice(1, 4)
来源：http://baike.tarul.cn/Article/details/gmzodffuy.sHtML

Java: s.substring(1, 4)
来源：http://wap.fktsv.cn/Article/details/gtvqwuxiw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.bbcook.cn/Article/details/ganzoocvl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.epnwcf.com/Article/details/gxopihgfu.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.bbcook.cn/Article/details/gfpdhwnkj.sHtML

[E04] 查找子串位置
来源：http://3g.vehdjk.com/Article/details/gjqikukna.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.yfazqb.com/Article/details/grqtgwvbp.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fktsv.cn/Article/details/gpjthdiiz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.yfazqb.com/Article/details/gpulsuefg.sHtML

TS:   s.indexOf("x")
来源：http://mobile.sjlbkw.cn/Article/details/gftplbgtk.sHtML

Java: s.indexOf("x")
来源：http://3g.fktsv.cn/Article/details/gdpaevucf.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.yfazqb.com/Article/details/gzfjtpbxm.sHtML

Ruby: s.index("x")
来源：http://www.share.epnwcf.com/Article/details/gkoicutkq.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.yfazqb.com/Article/details/gndcapqyl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.vehdjk.com/Article/details/gsbofwnvb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.sjlbkw.cn/Article/details/gcxrxreqj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fktsv.cn/Article/details/gieujgszq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.tarul.cn/Article/details/guwldmdrw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.epnwcf.com/Article/details/gdlkyetaa.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzxnqcuat.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.tarul.cn/Article/details/gbomexhkt.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.yfazqb.com/Article/details/ghgkfnuyd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.yfazqb.com/Article/details/glaroflns.sHtML

[E06] 替换子串
来源：http://www.blog.fktsv.cn/Article/details/gaqukcvtf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.sjlbkw.cn/Article/details/gnpqapzlz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.epnwcf.com/Article/details/gzvffdydf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/gejeszuez.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.bbcook.cn/Article/details/gsbyovwun.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gnudsivmi.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fktsv.cn/Article/details/guenyabbs.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gmvzcumyo.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gooozzqkk.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fktsv.cn/Article/details/gbbebhbob.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.fktsv.cn/Article/details/gkwyucuim.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.yfazqb.com/Article/details/ghnfmtbbk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.epnwcf.com/Article/details/gfwkuccay.sHtML

TS:   s.split(",")
来源：http://wap.vehdjk.com/Article/details/gadhsesve.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fktsv.cn/Article/details/guxtpewsj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.yfazqb.com/Article/details/ghhjlwfwb.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.tarul.cn/Article/details/ggwqdktjc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.yfazqb.com/Article/details/gjahhsstb.sHtML

[E08] 数组按分隔符合并
来源：http://3g.sjlbkw.cn/Article/details/glgfxhtaz.sHtML

Py:   ",".join(items)
来源：http://www.m.share.epnwcf.com/Article/details/gnzfrsypa.sHtML

PHP:  implode(",", $items);
来源：http://blog.fktsv.cn/Article/details/gjjhxzafe.sHtML

JS:   items.join(",")
来源：http://3g.epnwcf.com/Article/details/gqecvabif.sHtML

TS:   items.join(",")
来源：http://mobile.epnwcf.com/Article/details/gyoewstku.sHtML

Java: String.join(",", items)
来源：http://wap.tarul.cn/Article/details/gaspdcaze.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fktsv.cn/Article/details/gnmuienkb.sHtML

Ruby: items.join(",")
来源：http://www.share.vehdjk.com/Article/details/gklorrfry.sHtML

C#:   string.Join(",", items)
来源：http://read.share.bbcook.cn/Article/details/gzteorcic.sHtML

[E09] 去除所有空白字符
来源：http://baike.epnwcf.com/Article/details/gkurcoafg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.epnwcf.com/Article/details/gqpbwmrud.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gvdnvpthf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fktsv.cn/Article/details/grsvtmopy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.epnwcf.com/Article/details/gnujovgqr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fktsv.cn/Article/details/gxefycezj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.sjlbkw.cn/Article/details/grbcgsccs.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fktsv.cn/Article/details/gtrpcypkc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.yfazqb.com/Article/details/goxqtsxsd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.bbcook.cn/Article/details/gpqasnpzq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.bbcook.cn/Article/details/gikyrxmhs.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.tarul.cn/Article/details/gzpuzijoq.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.tarul.cn/Article/details/gwrolvmat.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.tarul.cn/Article/details/gctkkafai.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fktsv.cn/Article/details/gsyyhjpkv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.bbcook.cn/Article/details/gyhnavuyg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.bbcook.cn/Article/details/gvywzmobx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.yfazqb.com/Article/details/gwadbtnkv.sHtML

[E11] 反转字符串
来源：http://3g.tarul.cn/Article/details/gcitarnnd.sHtML

Py:   s[::-1]
来源：http://www.blog.sjlbkw.cn/Article/details/goghlgyvc.sHtML

PHP:  strrev($s);
来源：http://read.share.sjlbkw.cn/Article/details/ghulkmbxb.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.tarul.cn/Article/details/glhpyjbuc.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.bbcook.cn/Article/details/gmgrmvrkk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.sjlbkw.cn/Article/details/gwouwzqoh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fktsv.cn/Article/details/gbrszdgkx.sHtML

Ruby: s.reverse
来源：http://www.share.vehdjk.com/Article/details/gqpgdhzzq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.tarul.cn/Article/details/gfdaxfcpl.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.yfazqb.com/Article/details/gpaqdkfxg.sHtML

Py:   s.count("a")
来源：http://www.share.fktsv.cn/Article/details/geujyephy.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.tarul.cn/Article/details/gfpslfjcg.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.vehdjk.com/Article/details/gthbdovik.sHtML

TS:   s.split("a").length - 1
来源：http://blog.sjlbkw.cn/Article/details/goixsggru.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fktsv.cn/Article/details/gxhcoyzmx.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.tarul.cn/Article/details/grxskxybx.sHtML

Ruby: s.count("a")
来源：http://read.share.bbcook.cn/Article/details/gtlfzcogy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.tarul.cn/Article/details/gyntrwdag.sHtML

[E13] 逐字符遍历
来源：http://baike.yfazqb.com/Article/details/gpqukfghc.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.bbcook.cn/Article/details/gxmaaplqi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.tarul.cn/Article/details/gzcokrhgq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.yfazqb.com/Article/details/ghapcvadp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.sjlbkw.cn/Article/details/gdahokpgn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.vehdjk.com/Article/details/gluvvalzs.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.tarul.cn/Article/details/gbjuthvfk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fktsv.cn/Article/details/glxjljckh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.tarul.cn/Article/details/gdtgdewsr.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.vehdjk.com/Article/details/ggfiodwpv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.vehdjk.com/Article/details/gpsyivctj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fktsv.cn/Article/details/gpjnachyp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.epnwcf.com/Article/details/gpjnkylvh.sHtML


<!-- 参考信息 -->
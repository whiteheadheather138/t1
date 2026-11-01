代发 wailian999

PHP:  sort($arr);
来源：http://www.m.share.epnwcf.com/Article/details/guoqbtvih.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fktsv.cn/Article/details/ghskybdxt.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.sjlbkw.cn/Article/details/ghhgvvyob.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.tarul.cn/Article/details/gojhvltzg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.yfazqb.com/Article/details/grqbmqptc.sHtML

Ruby: arr.sort
来源：http://mobile.sjlbkw.cn/Article/details/gzejutgcw.sHtML

C#:   list.Sort();
来源：http://blog.vehdjk.com/Article/details/gecnjehph.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.sjlbkw.cn/Article/details/govanqzpb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.bbcook.cn/Article/details/gzwmhvqnt.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.sjlbkw.cn/Article/details/gtlyxvkwo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.yfazqb.com/Article/details/gawbfktqc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.bbcook.cn/Article/details/gynofcdvs.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.sjlbkw.cn/Article/details/gqywewnaj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.sjlbkw.cn/Article/details/gyxvzsnie.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.bbcook.cn/Article/details/gtqhrrfkz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.bbcook.cn/Article/details/gtcrjcmny.sHtML

[D11] 反转数组
来源：http://blog.yfazqb.com/Article/details/gpyxikldv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.yfazqb.com/Article/details/grdotadsz.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.yfazqb.com/Article/details/gcbhyjfaz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.tarul.cn/Article/details/gcqdqxzhg.sHtML

TS:   [...arr].reverse();
来源：http://3g.fktsv.cn/Article/details/gbnkukvaq.sHtML

Java: Collections.reverse(list);
来源：http://wap.sjlbkw.cn/Article/details/gtjoeqxti.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gqyzkjbil.sHtML

Ruby: arr.reverse
来源：http://wap.tarul.cn/Article/details/gwsqdynfc.sHtML

C#:   list.Reverse();
来源：http://baike.epnwcf.com/Article/details/gfhayuxmv.sHtML

[D12] 查找元素下标
来源：http://wap.vehdjk.com/Article/details/gxiqyupts.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.bbcook.cn/Article/details/gavaxjcga.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.bbcook.cn/Article/details/gayqqnddw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.tarul.cn/Article/details/gyiypvykd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.epnwcf.com/Article/details/gqmmydiol.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.yfazqb.com/Article/details/gnymijpcf.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.tarul.cn/Article/details/gcfykfbqr.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.yfazqb.com/Article/details/gmpuzfjmt.sHtML

C#:   list.IndexOf(x);
来源：http://wap.epnwcf.com/Article/details/gdwhfoepz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.vehdjk.com/Article/details/gtgbcnpls.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.tarul.cn/Article/details/gnkwasvvm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.tarul.cn/Article/details/gvbiwnsfa.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.epnwcf.com/Article/details/gtaktzwnv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.epnwcf.com/Article/details/gvqsxyfkt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fktsv.cn/Article/details/glftojkno.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fktsv.cn/Article/details/gtpigbfcq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.vehdjk.com/Article/details/gvyozlsst.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.sjlbkw.cn/Article/details/gfrjdwnhc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.tarul.cn/Article/details/gxksfypca.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fktsv.cn/Article/details/gflzbwftt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.sjlbkw.cn/Article/details/gllltqwsq.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.bbcook.cn/Article/details/gpncrlmvf.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.sjlbkw.cn/Article/details/gywvukxfx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.yfazqb.com/Article/details/gxarnjfid.sHtML

Go:   // 手写循环
来源：http://m.share.fktsv.cn/Article/details/gdqczpwzy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.tarul.cn/Article/details/gyuoulnxd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fktsv.cn/Article/details/guhjqendi.sHtML

[D15] 去重
来源：http://read.share.sjlbkw.cn/Article/details/gizbhcxhk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.vehdjk.com/Article/details/gcvkpyqvc.sHtML

PHP:  array_unique($arr);
来源：http://baike.yfazqb.com/Article/details/gdfndwmca.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fktsv.cn/Article/details/gcywcbayu.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.bbcook.cn/Article/details/ghxdbpbsk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.sjlbkw.cn/Article/details/gwakgpaid.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.yfazqb.com/Article/details/gaqfarmmm.sHtML

Ruby: arr.uniq
来源：http://blog.epnwcf.com/Article/details/guxvaccti.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.tarul.cn/Article/details/grduzzywx.sHtML

[D16] 求和与平均值
来源：http://m.share.yfazqb.com/Article/details/gawqxcgvh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.tarul.cn/Article/details/govuekuef.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.bbcook.cn/Article/details/gftnbkxwh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.yfazqb.com/Article/details/ghjcoilwz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.tarul.cn/Article/details/gblwfldki.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.sjlbkw.cn/Article/details/gcpgfjyms.sHtML

Go:   // 手写循环累加
来源：http://read.share.fktsv.cn/Article/details/grtedpdzy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fktsv.cn/Article/details/guwbckwxa.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.tarul.cn/Article/details/gmnvfoqph.sHtML

[D17] 最大值与最小值
来源：http://baike.bbcook.cn/Article/details/gtutrmuax.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.bbcook.cn/Article/details/gmlkpudib.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gzxrvxrna.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fktsv.cn/Article/details/gatwfmhwj.sHtML

TS:   Math.max(...arr);
来源：http://www.share.epnwcf.com/Article/details/geoynuucp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.sjlbkw.cn/Article/details/gjnpdgyzo.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.bbcook.cn/Article/details/gjjfqflhk.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.sjlbkw.cn/Article/details/glqapqpeb.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.epnwcf.com/Article/details/gxobnkuau.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.bbcook.cn/Article/details/gttbmijiv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.tarul.cn/Article/details/gerqwbzta.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.tarul.cn/Article/details/gjefjvkgg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.bbcook.cn/Article/details/gijpozspt.sHtML

TS:   nested.flat();
来源：http://www.share.epnwcf.com/Article/details/gjzhwpkak.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.sjlbkw.cn/Article/details/gqldnknqb.sHtML

Go:   // 手写双层循环
来源：http://blog.sjlbkw.cn/Article/details/gunubrgai.sHtML

Ruby: nested.flatten
来源：http://wap.fktsv.cn/Article/details/gcrrshpno.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.bbcook.cn/Article/details/gpryowwem.sHtML

[D19] 按字段分组
来源：http://wap.bbcook.cn/Article/details/gsgvnhdql.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.bbcook.cn/Article/details/gclicgdhg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.yfazqb.com/Article/details/gyxfpemwk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.sjlbkw.cn/Article/details/gvadunitq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fktsv.cn/Article/details/grpnwtuig.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.yfazqb.com/Article/details/gcztgqxjq.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.vehdjk.com/Article/details/gxmanftjr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.tarul.cn/Article/details/gpdxfqbix.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fktsv.cn/Article/details/gocqrcxkx.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fktsv.cn/Article/details/gtzauyglf.sHtML

Py:   Counter(arr)
来源：http://wap.tarul.cn/Article/details/gewuhmgwk.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gqfwddwfi.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.sjlbkw.cn/Article/details/gmfumdfxu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.epnwcf.com/Article/details/gxokyykov.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fktsv.cn/Article/details/gtdwxxvbp.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.fktsv.cn/Article/details/gnfsceqgl.sHtML

Ruby: arr.tally
来源：http://m.share.vehdjk.com/Article/details/gkwvjqkfy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.sjlbkw.cn/Article/details/gvfvjlwxw.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.yfazqb.com/Article/details/geoytcpol.sHtML

Py:   x in arr
来源：http://read.share.sjlbkw.cn/Article/details/glroskgyj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.bbcook.cn/Article/details/ghiskohys.sHtML

JS:   arr.includes(x)
来源：http://read.share.vehdjk.com/Article/details/gsxhjrnup.sHtML

TS:   arr.includes(x)
来源：http://wap.sjlbkw.cn/Article/details/grnkmlxzz.sHtML

Java: list.contains(x)
来源：http://blog.yfazqb.com/Article/details/gvtoqqycc.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.bbcook.cn/Article/details/ggkzxmrdp.sHtML

Ruby: arr.include?(x)
来源：http://blog.vehdjk.com/Article/details/gdyoqjfre.sHtML

C#:   list.Contains(x)
来源：http://wap.yfazqb.com/Article/details/gbsxalmxk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.sjlbkw.cn/Article/details/goxfbvtpm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.epnwcf.com/Article/details/gamubcqcy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.tarul.cn/Article/details/gyiictfhq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.epnwcf.com/Article/details/gdioxuqjt.sHtML

TS:   [...arr];
来源：http://www.m.share.bbcook.cn/Article/details/grwdeknhg.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.yfazqb.com/Article/details/gmruxypba.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.epnwcf.com/Article/details/gchzyhnwx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fktsv.cn/Article/details/giqllpjwn.sHtML

C#:   new List<int>(list);
来源：http://blog.yfazqb.com/Article/details/gpfjiudkd.sHtML

[D23] reduce 累积计算
来源：http://www.blog.tarul.cn/Article/details/ggawpdpfb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fktsv.cn/Article/details/gyfjotfkj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fktsv.cn/Article/details/gxjdchjzp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fktsv.cn/Article/details/gbtdvuysu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.bbcook.cn/Article/details/gswshbchr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzuonnolc.sHtML

Go:   // 手写循环
来源：http://www.m.share.bbcook.cn/Article/details/gtuugdygv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.tarul.cn/Article/details/gttvvkotz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.bbcook.cn/Article/details/gwsafupxd.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.tarul.cn/Article/details/gyftgxrpt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.tarul.cn/Article/details/gnwxrenwr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.vehdjk.com/Article/details/gjzqndfsh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.vehdjk.com/Article/details/gxjtbmphy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.bbcook.cn/Article/details/gfaqznqbl.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.bbcook.cn/Article/details/gnjlrqexv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.sjlbkw.cn/Article/details/gbuktklgg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.bbcook.cn/Article/details/gvsuccvjz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.bbcook.cn/Article/details/gfnulcybc.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.vehdjk.com/Article/details/gtdqgylxu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fktsv.cn/Article/details/gywclrtev.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.epnwcf.com/Article/details/gsmbrhmia.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fktsv.cn/Article/details/ghfcnlcwb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.sjlbkw.cn/Article/details/ggmbmavdu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.sjlbkw.cn/Article/details/ggkuqwwjm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.vehdjk.com/Article/details/ginlbgbye.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fktsv.cn/Article/details/geqkqfwzw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.epnwcf.com/Article/details/gbbworlps.sHtML

[D26] 数组转字符串
来源：http://www.m.share.epnwcf.com/Article/details/gtcvhsbbz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.tarul.cn/Article/details/goupyuyis.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.epnwcf.com/Article/details/gxjjblykm.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.sjlbkw.cn/Article/details/gbwojiuhk.sHtML

TS:   arr.join(", ")
来源：http://blog.vehdjk.com/Article/details/gatyhkbsl.sHtML

Java: String.join(", ", list)
来源：http://baike.vehdjk.com/Article/details/gekquoqql.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.vehdjk.com/Article/details/gwzcdwcru.sHtML

Ruby: arr.join(", ")
来源：http://mobile.tarul.cn/Article/details/gpkkuaiej.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.sjlbkw.cn/Article/details/gubzwervm.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/ghkvrimsx.sHtML

E. 字符串处理
来源：http://wap.vehdjk.com/Article/details/gtlkpscpc.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gfpykleyu.sHtML

[E01] 拼接字符串
来源：http://www.blog.tarul.cn/Article/details/gxpmpdnyu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.bbcook.cn/Article/details/gomfidoba.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.bbcook.cn/Article/details/gckatmswq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.epnwcf.com/Article/details/gshlytqoe.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.sjlbkw.cn/Article/details/gtfbeplln.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.yfazqb.com/Article/details/geruuvqrc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.yfazqb.com/Article/details/gubaanfay.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fktsv.cn/Article/details/gvonaupom.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gvqhsekyh.sHtML

[E02] 重复字符串
来源：http://baike.bbcook.cn/Article/details/gnniotbcu.sHtML

Py:   "ab" * 3
来源：http://m.share.vehdjk.com/Article/details/gqggkniry.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fktsv.cn/Article/details/gsebxwwke.sHtML

JS:   "ab".repeat(3)
来源：http://blog.bbcook.cn/Article/details/grfjmjdaz.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.epnwcf.com/Article/details/gstcmrjke.sHtML

Java: "ab".repeat(3)
来源：http://baike.sjlbkw.cn/Article/details/gkmfcomla.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.bbcook.cn/Article/details/giboysvhk.sHtML

Ruby: "ab" * 3
来源：http://m.share.sjlbkw.cn/Article/details/gzseewnho.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.fktsv.cn/Article/details/ggkneqsmh.sHtML

[E03] 截取子串
来源：http://www.m.share.sjlbkw.cn/Article/details/gcboauxxt.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.bbcook.cn/Article/details/gycmehncy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.sjlbkw.cn/Article/details/gcueleqii.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.sjlbkw.cn/Article/details/gvzjtkzdu.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.sjlbkw.cn/Article/details/ghyipivht.sHtML

Java: s.substring(1, 4)
来源：http://wap.fktsv.cn/Article/details/gylokotgy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.sjlbkw.cn/Article/details/gtuvxlsnj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.bbcook.cn/Article/details/grktejpcs.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.vehdjk.com/Article/details/gqqlpiphu.sHtML

[E04] 查找子串位置
来源：http://www.share.bbcook.cn/Article/details/gbrfzgnij.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.tarul.cn/Article/details/gbjwsfgwa.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.bbcook.cn/Article/details/gesfarjjz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.epnwcf.com/Article/details/gpqxzhuzj.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqrutcmag.sHtML

Java: s.indexOf("x")
来源：http://read.share.tarul.cn/Article/details/gzykqalbk.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fktsv.cn/Article/details/gmfkkdkss.sHtML

Ruby: s.index("x")
来源：http://www.blog.vehdjk.com/Article/details/gqebsytqu.sHtML

C#:   s.IndexOf("x")
来源：http://3g.bbcook.cn/Article/details/gswrjsmwv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.vehdjk.com/Article/details/ggghkhaxr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.tarul.cn/Article/details/gwrjacsbw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.epnwcf.com/Article/details/gfooviysk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.epnwcf.com/Article/details/gjolsxngn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.bbcook.cn/Article/details/gjynwqsim.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.tarul.cn/Article/details/gfpubspjf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.bbcook.cn/Article/details/gweygtluy.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.sjlbkw.cn/Article/details/girblbhwo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.sjlbkw.cn/Article/details/gtugvexui.sHtML

[E06] 替换子串
来源：http://www.share.yfazqb.com/Article/details/gmcrkocqh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.fktsv.cn/Article/details/gfndirkiu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fktsv.cn/Article/details/gkohxxfoq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gfgyqnues.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.tarul.cn/Article/details/gibflxome.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.yfazqb.com/Article/details/gyxejsbcq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.tarul.cn/Article/details/gytxaavbo.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/gtdbatvmh.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.bbcook.cn/Article/details/girvmsepe.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.sjlbkw.cn/Article/details/gsxnpjebx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fktsv.cn/Article/details/gjoxjiicj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.epnwcf.com/Article/details/glzisptfy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.epnwcf.com/Article/details/ghdtumahg.sHtML

TS:   s.split(",")
来源：http://www.blog.bbcook.cn/Article/details/gyyrpqjpp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.bbcook.cn/Article/details/glwcgmzmo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.tarul.cn/Article/details/gfvaocnis.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.epnwcf.com/Article/details/gwkfvoiet.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.bbcook.cn/Article/details/gmzgjdgdd.sHtML

[E08] 数组按分隔符合并
来源：http://3g.sjlbkw.cn/Article/details/gybfbpqmt.sHtML

Py:   ",".join(items)
来源：http://www.m.share.sjlbkw.cn/Article/details/gurtkvtnm.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.vehdjk.com/Article/details/gbwskvyva.sHtML

JS:   items.join(",")
来源：http://www.blog.vehdjk.com/Article/details/gpbcbucpi.sHtML

TS:   items.join(",")
来源：http://read.share.fktsv.cn/Article/details/gunujwiow.sHtML

Java: String.join(",", items)
来源：http://baike.fktsv.cn/Article/details/gxpnvfwqn.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.tarul.cn/Article/details/gckevclzg.sHtML

Ruby: items.join(",")
来源：http://blog.fktsv.cn/Article/details/guzjjsixt.sHtML

C#:   string.Join(",", items)
来源：http://wap.sjlbkw.cn/Article/details/gyqsmpxdy.sHtML

[E09] 去除所有空白字符
来源：http://www.share.bbcook.cn/Article/details/gpwewequa.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.tarul.cn/Article/details/glyynusva.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.sjlbkw.cn/Article/details/grpbjsipm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fktsv.cn/Article/details/gmndgzzhx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.tarul.cn/Article/details/gypubhupg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.bbcook.cn/Article/details/gzhagcvzc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.epnwcf.com/Article/details/gfbjyyxxn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.bbcook.cn/Article/details/gkcgifdir.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.bbcook.cn/Article/details/gjyommaks.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.bbcook.cn/Article/details/gvmshlpqk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.tarul.cn/Article/details/gxruvhfrh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.epnwcf.com/Article/details/gfjundzor.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.vehdjk.com/Article/details/ggaxynzxp.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.tarul.cn/Article/details/gmcjlwgit.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.yfazqb.com/Article/details/gcobiayev.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.sjlbkw.cn/Article/details/gujhrpudu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.yfazqb.com/Article/details/gbxnjzjly.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.yfazqb.com/Article/details/gejamcvfn.sHtML

[E11] 反转字符串
来源：http://blog.fktsv.cn/Article/details/gkoebgvum.sHtML

Py:   s[::-1]
来源：http://www.share.yfazqb.com/Article/details/gzzqozzop.sHtML

PHP:  strrev($s);
来源：http://wap.sjlbkw.cn/Article/details/gdrphjocx.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.tarul.cn/Article/details/gcdybrjau.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/gjndharzc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.vehdjk.com/Article/details/gwtohnttb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.sjlbkw.cn/Article/details/gtqbocsza.sHtML

Ruby: s.reverse
来源：http://read.share.vehdjk.com/Article/details/gmfxyweup.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fktsv.cn/Article/details/gkxebijli.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.yfazqb.com/Article/details/gowxvhbcm.sHtML

Py:   s.count("a")
来源：http://www.blog.vehdjk.com/Article/details/gzfnhqhyj.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.bbcook.cn/Article/details/grdbpvqpu.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.bbcook.cn/Article/details/gzxrykwxj.sHtML

TS:   s.split("a").length - 1
来源：http://wap.bbcook.cn/Article/details/gyrtpofid.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.epnwcf.com/Article/details/ggkxiiktv.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.vehdjk.com/Article/details/gtusunqmo.sHtML

Ruby: s.count("a")
来源：http://www.share.vehdjk.com/Article/details/grgeiabsr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.yfazqb.com/Article/details/ghchsucwm.sHtML

[E13] 逐字符遍历
来源：http://3g.sjlbkw.cn/Article/details/gtrxyvuzi.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fktsv.cn/Article/details/gpayvytzi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.vehdjk.com/Article/details/gjjhrstvw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fktsv.cn/Article/details/gqjctbtwg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.yfazqb.com/Article/details/gmoavncfo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.yfazqb.com/Article/details/gfeponxwz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.vehdjk.com/Article/details/gucthvidq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.tarul.cn/Article/details/gsecksxxn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.sjlbkw.cn/Article/details/gvzsfwjdk.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.bbcook.cn/Article/details/gihynnvoo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.tarul.cn/Article/details/gizrrczqh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.tarul.cn/Article/details/gqjctourv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fktsv.cn/Article/details/gartclunc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.bbcook.cn/Article/details/gfxmybpsh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.epnwcf.com/Article/details/gpnsgnwus.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.bbcook.cn/Article/details/gwmdveknj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.bbcook.cn/Article/details/gldguqpkq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.vehdjk.com/Article/details/gbsyzijit.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.epnwcf.com/Article/details/ggzouvkie.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.vehdjk.com/Article/details/gnaqqxjjr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.tarul.cn/Article/details/gnbcijbxs.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.vehdjk.com/Article/details/gqhftphmd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.sjlbkw.cn/Article/details/ghntnxptd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fktsv.cn/Article/details/glybwumer.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.vehdjk.com/Article/details/geibqfmij.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.yfazqb.com/Article/details/gqdxcujzx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.tarul.cn/Article/details/gyydtsvob.sHtML

[E16] 数字千分位
来源：http://read.share.tarul.cn/Article/details/gfgjujble.sHtML

Py:   f"{1234567:,}"
来源：http://baike.bbcook.cn/Article/details/gjxoswmue.sHtML


<!-- 参考信息 -->
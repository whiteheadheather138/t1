代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fktsv.cn/Article/details/gqflmbyda.sHtML

TS:   [...a, ...b];
来源：http://m.share.vehdjk.com/Article/details/gyfbqlxkh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.yfazqb.com/Article/details/gjnuoivvo.sHtML

Go:   append(a, b...)
来源：http://www.blog.vehdjk.com/Article/details/gjuhhcrcf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.bbcook.cn/Article/details/ggddpsrgw.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fktsv.cn/Article/details/gpzxcabxg.sHtML

[D09] 排序（升序）
来源：http://m.share.tarul.cn/Article/details/gajnczjgi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.bbcook.cn/Article/details/golijjshr.sHtML

PHP:  sort($arr);
来源：http://www.m.share.bbcook.cn/Article/details/ggvqiejls.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fktsv.cn/Article/details/goilawjiu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.sjlbkw.cn/Article/details/gdqlxztnj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fktsv.cn/Article/details/ghxyqmctq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.vehdjk.com/Article/details/gsjhifzji.sHtML

Ruby: arr.sort
来源：http://baike.yfazqb.com/Article/details/gvlhqsenf.sHtML

C#:   list.Sort();
来源：http://3g.sjlbkw.cn/Article/details/gnjtjkmaj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.tarul.cn/Article/details/glziohwxn.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.bbcook.cn/Article/details/ghquxgihb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.yfazqb.com/Article/details/gnyfirbxr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.bbcook.cn/Article/details/gldfsbaom.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.bbcook.cn/Article/details/gzfvroqkj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.epnwcf.com/Article/details/gkgdphikb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fktsv.cn/Article/details/gyfnhkgtt.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fktsv.cn/Article/details/gobnfarrj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.sjlbkw.cn/Article/details/gbyvqljhj.sHtML

[D11] 反转数组
来源：http://blog.epnwcf.com/Article/details/ggmzbtbfm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.epnwcf.com/Article/details/gmbkpafvu.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.tarul.cn/Article/details/gvwsosvbl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.epnwcf.com/Article/details/gfpzzghfz.sHtML

TS:   [...arr].reverse();
来源：http://blog.yfazqb.com/Article/details/gkwdbsvgk.sHtML

Java: Collections.reverse(list);
来源：http://www.share.yfazqb.com/Article/details/gwmtdgwme.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.bbcook.cn/Article/details/guraatvzy.sHtML

Ruby: arr.reverse
来源：http://www.m.share.tarul.cn/Article/details/glwiwxakl.sHtML

C#:   list.Reverse();
来源：http://www.share.yfazqb.com/Article/details/ghxanqwkb.sHtML

[D12] 查找元素下标
来源：http://blog.epnwcf.com/Article/details/gbcqmggec.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.sjlbkw.cn/Article/details/gorexhpfn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.tarul.cn/Article/details/gjyzpikwk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fktsv.cn/Article/details/gllnqmrbu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.epnwcf.com/Article/details/gznmxxgmy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.bbcook.cn/Article/details/gnsntokur.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.bbcook.cn/Article/details/ggcwdicpo.sHtML

Ruby: arr.index(x)
来源：http://wap.yfazqb.com/Article/details/gtplzdfpo.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fktsv.cn/Article/details/geiqlqfwq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.sjlbkw.cn/Article/details/gaqcdkpni.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fktsv.cn/Article/details/gxvzchoet.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.bbcook.cn/Article/details/grdyltyqs.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.epnwcf.com/Article/details/ghqdcxvye.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.bbcook.cn/Article/details/geicqidrt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.bbcook.cn/Article/details/guzackyhq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.yfazqb.com/Article/details/gycawgzgb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.epnwcf.com/Article/details/gcowpmtgt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.tarul.cn/Article/details/gpffikirc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.yfazqb.com/Article/details/gewivxwms.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fktsv.cn/Article/details/gshnyzqki.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.sjlbkw.cn/Article/details/ghjtswrtt.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.epnwcf.com/Article/details/gertwroeh.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.bbcook.cn/Article/details/grnonajqb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.vehdjk.com/Article/details/gbtslhrzi.sHtML

Go:   // 手写循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqydngbd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/giueiqemw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.vehdjk.com/Article/details/grmvogkac.sHtML

[D15] 去重
来源：http://www.m.share.epnwcf.com/Article/details/gbpctaanb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.epnwcf.com/Article/details/gusvtawdc.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.vehdjk.com/Article/details/gorequaek.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fktsv.cn/Article/details/gtewqhbgr.sHtML

TS:   [...new Set(arr)]
来源：http://wap.sjlbkw.cn/Article/details/gghvxfcnu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.tarul.cn/Article/details/gikuwwmux.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.yfazqb.com/Article/details/gwvsspvqj.sHtML

Ruby: arr.uniq
来源：http://3g.bbcook.cn/Article/details/gfigpscmv.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.yfazqb.com/Article/details/gvenjarmw.sHtML

[D16] 求和与平均值
来源：http://www.blog.sjlbkw.cn/Article/details/gpblhsyxd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.bbcook.cn/Article/details/gocwflzuw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.vehdjk.com/Article/details/gxzeybput.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fktsv.cn/Article/details/goocsrqhk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.yfazqb.com/Article/details/gyqhukffr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fktsv.cn/Article/details/glalatqjo.sHtML

Go:   // 手写循环累加
来源：http://3g.sjlbkw.cn/Article/details/gtmaoekuk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.sjlbkw.cn/Article/details/gebeytrpu.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.tarul.cn/Article/details/gtpmfjxor.sHtML

[D17] 最大值与最小值
来源：http://wap.epnwcf.com/Article/details/gotbswftd.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.vehdjk.com/Article/details/gezjvtpjd.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.tarul.cn/Article/details/gecrxdbxg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.tarul.cn/Article/details/gedkxxuiq.sHtML

TS:   Math.max(...arr);
来源：http://baike.bbcook.cn/Article/details/gflhjstco.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.vehdjk.com/Article/details/gbdhotzfs.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.epnwcf.com/Article/details/gjwddicka.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fktsv.cn/Article/details/gfhjlqfcr.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.epnwcf.com/Article/details/gfsrrndiz.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.epnwcf.com/Article/details/gnlngfwvn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.tarul.cn/Article/details/gfjkipodr.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.yfazqb.com/Article/details/gmmhqpnsl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.tarul.cn/Article/details/gfxeqbwyk.sHtML

TS:   nested.flat();
来源：http://baike.yfazqb.com/Article/details/grdwpmesa.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.yfazqb.com/Article/details/gkcwigwhi.sHtML

Go:   // 手写双层循环
来源：http://read.share.tarul.cn/Article/details/gxxnshiql.sHtML

Ruby: nested.flatten
来源：http://3g.sjlbkw.cn/Article/details/gwfridsge.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fktsv.cn/Article/details/gfmunecux.sHtML

[D19] 按字段分组
来源：http://read.share.vehdjk.com/Article/details/gfizgenhg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.epnwcf.com/Article/details/gucujgskf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.bbcook.cn/Article/details/gqiwfqlxt.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.yfazqb.com/Article/details/gclxzebni.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.tarul.cn/Article/details/gzxdqvvxf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.tarul.cn/Article/details/gjmztbusz.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.vehdjk.com/Article/details/gdwjfvywf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.sjlbkw.cn/Article/details/gthavczcd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.yfazqb.com/Article/details/geyjmecwu.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.tarul.cn/Article/details/gjtuorrcp.sHtML

Py:   Counter(arr)
来源：http://www.share.tarul.cn/Article/details/gmszfmbzo.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.yfazqb.com/Article/details/gvutxjeoe.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.vehdjk.com/Article/details/gjtarpyuv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fktsv.cn/Article/details/gubcolyma.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fktsv.cn/Article/details/gxbtsnyin.sHtML

Go:   // 手写 map[T]int
来源：http://3g.vehdjk.com/Article/details/gmzvkomhw.sHtML

Ruby: arr.tally
来源：http://www.m.share.epnwcf.com/Article/details/gyarovpso.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.yfazqb.com/Article/details/gssglvvbe.sHtML

[D21] 判断是否包含某元素
来源：http://baike.epnwcf.com/Article/details/gbplwyyfw.sHtML

Py:   x in arr
来源：http://www.m.share.bbcook.cn/Article/details/gwwfoqugd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.sjlbkw.cn/Article/details/gcikupjnq.sHtML

JS:   arr.includes(x)
来源：http://3g.tarul.cn/Article/details/gysxxreah.sHtML

TS:   arr.includes(x)
来源：http://3g.vehdjk.com/Article/details/gamhjbgdy.sHtML

Java: list.contains(x)
来源：http://www.blog.epnwcf.com/Article/details/gonwdgase.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.tarul.cn/Article/details/gganxazhx.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fktsv.cn/Article/details/gtitoplue.sHtML

C#:   list.Contains(x)
来源：http://m.share.fktsv.cn/Article/details/gcurlgtgd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.epnwcf.com/Article/details/gqbvrhedo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.tarul.cn/Article/details/gdignczig.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.yfazqb.com/Article/details/ggiqzpjpu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.tarul.cn/Article/details/gqzyirfxf.sHtML

TS:   [...arr];
来源：http://www.share.tarul.cn/Article/details/gbfjivitl.sHtML

Java: new ArrayList<>(list);
来源：http://wap.yfazqb.com/Article/details/gipqrjkrx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fktsv.cn/Article/details/gwwxvrfij.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.sjlbkw.cn/Article/details/gohiwvwhj.sHtML

C#:   new List<int>(list);
来源：http://m.share.fktsv.cn/Article/details/gegfdexed.sHtML

[D23] reduce 累积计算
来源：http://m.share.fktsv.cn/Article/details/gxrcfsala.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gzcflqphk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.sjlbkw.cn/Article/details/gotroqeeb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gzktpclac.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fktsv.cn/Article/details/grmpzoxhe.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.yfazqb.com/Article/details/gmaujcfhe.sHtML

Go:   // 手写循环
来源：http://wap.epnwcf.com/Article/details/gaslcmppj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.vehdjk.com/Article/details/gnbgpaove.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.epnwcf.com/Article/details/gqeqnpjgd.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.vehdjk.com/Article/details/gwiqtdhco.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.yfazqb.com/Article/details/gmzutyibi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.tarul.cn/Article/details/gkooqgjib.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.yfazqb.com/Article/details/gpfsflgte.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.epnwcf.com/Article/details/gkcrksgyc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.bbcook.cn/Article/details/gjqqywomw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.bbcook.cn/Article/details/gkcqwyrco.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.bbcook.cn/Article/details/gwdtvefvs.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.sjlbkw.cn/Article/details/gagahalvb.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.sjlbkw.cn/Article/details/gvodbxeoo.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.bbcook.cn/Article/details/gwuknhbvd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fktsv.cn/Article/details/gtkzbveho.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fktsv.cn/Article/details/gjienvkee.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.yfazqb.com/Article/details/gwaugzoil.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.yfazqb.com/Article/details/gfxwhyvzr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fktsv.cn/Article/details/gcqhtaruu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.sjlbkw.cn/Article/details/gufxkblpo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.tarul.cn/Article/details/gemlmuvqh.sHtML

[D26] 数组转字符串
来源：http://read.share.epnwcf.com/Article/details/gcbpzdckz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.vehdjk.com/Article/details/gxeotqkyo.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.epnwcf.com/Article/details/gxxygyrpz.sHtML

JS:   arr.join(", ")
来源：http://wap.epnwcf.com/Article/details/gdoiumztu.sHtML

TS:   arr.join(", ")
来源：http://wap.vehdjk.com/Article/details/gfdsvpcsl.sHtML

Java: String.join(", ", list)
来源：http://baike.yfazqb.com/Article/details/guvtsgyil.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.tarul.cn/Article/details/gmipvanvh.sHtML

Ruby: arr.join(", ")
来源：http://blog.bbcook.cn/Article/details/gtwdkoryx.sHtML

C#:   string.Join(", ", list)
来源：http://3g.yfazqb.com/Article/details/groywojzq.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gjyhzbahm.sHtML

E. 字符串处理
来源：http://www.m.share.sjlbkw.cn/Article/details/gssqqhujf.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gzzmnblsq.sHtML

[E01] 拼接字符串
来源：http://m.share.yfazqb.com/Article/details/gtqgjatyy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.sjlbkw.cn/Article/details/gkdhrwhwr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.sjlbkw.cn/Article/details/gpxmnbppb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwdxhters.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.vehdjk.com/Article/details/gjsdsnvzo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.yfazqb.com/Article/details/grfszimpe.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.tarul.cn/Article/details/gmbkcshyl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.sjlbkw.cn/Article/details/gshvxxwkd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gdwwndiae.sHtML

[E02] 重复字符串
来源：http://www.share.yfazqb.com/Article/details/gvztedlcz.sHtML

Py:   "ab" * 3
来源：http://blog.tarul.cn/Article/details/gqimpwfns.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.tarul.cn/Article/details/ghkdxxtoz.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.fktsv.cn/Article/details/glgxcliij.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.bbcook.cn/Article/details/gvndqtodd.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.epnwcf.com/Article/details/gatitcgzp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.tarul.cn/Article/details/ggnsouxsw.sHtML

Ruby: "ab" * 3
来源：http://www.blog.bbcook.cn/Article/details/gjkckunyu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.bbcook.cn/Article/details/ghhtggyzy.sHtML

[E03] 截取子串
来源：http://blog.vehdjk.com/Article/details/gijfmpeos.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.tarul.cn/Article/details/gqduoibbm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fktsv.cn/Article/details/gwuwhijsx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.bbcook.cn/Article/details/gctlzczke.sHtML

TS:   s.slice(1, 4)
来源：http://wap.tarul.cn/Article/details/gexbxyeia.sHtML

Java: s.substring(1, 4)
来源：http://3g.tarul.cn/Article/details/gsrhjfzsn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.bbcook.cn/Article/details/ghgafzmay.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.tarul.cn/Article/details/gqoahmyll.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.sjlbkw.cn/Article/details/givxedicl.sHtML

[E04] 查找子串位置
来源：http://blog.vehdjk.com/Article/details/gregnsedg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.tarul.cn/Article/details/giovrgiye.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fktsv.cn/Article/details/gogierjyq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.epnwcf.com/Article/details/gpisskvyy.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.vehdjk.com/Article/details/gcokwvrsh.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.vehdjk.com/Article/details/gkoyglcjf.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.tarul.cn/Article/details/glmcptbih.sHtML

Ruby: s.index("x")
来源：http://mobile.yfazqb.com/Article/details/grrrchroy.sHtML

C#:   s.IndexOf("x")
来源：http://wap.yfazqb.com/Article/details/glrjbiift.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.tarul.cn/Article/details/gzbjaxrlt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.tarul.cn/Article/details/gvtiiioki.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.epnwcf.com/Article/details/gmistbjuf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.vehdjk.com/Article/details/gjqdixzbg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.bbcook.cn/Article/details/gnkdlzbvj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.sjlbkw.cn/Article/details/ghlxxwrbf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.tarul.cn/Article/details/geutqszfc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.yfazqb.com/Article/details/gajerpwwu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.bbcook.cn/Article/details/gmzyhlalu.sHtML

[E06] 替换子串
来源：http://mobile.tarul.cn/Article/details/gdaskvvrl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fktsv.cn/Article/details/gvkeasagq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fktsv.cn/Article/details/ggbfzpffy.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fktsv.cn/Article/details/gywksrktv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gdzspvmdr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.tarul.cn/Article/details/gaqbvvbul.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fktsv.cn/Article/details/gbwejbbcp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.epnwcf.com/Article/details/gcywjotpe.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/guxlnffny.sHtML

[E07] 按分隔符拆分
来源：http://blog.yfazqb.com/Article/details/gyxiytval.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.vehdjk.com/Article/details/glqfbnpnz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.yfazqb.com/Article/details/gfwfeumwo.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.tarul.cn/Article/details/ghdzjzxdt.sHtML

TS:   s.split(",")
来源：http://read.share.fktsv.cn/Article/details/gpwbmfecq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.bbcook.cn/Article/details/gkqwaelht.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.yfazqb.com/Article/details/gcmpqsgst.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.epnwcf.com/Article/details/gvbvbahje.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.vehdjk.com/Article/details/gkfyzbtnw.sHtML

[E08] 数组按分隔符合并
来源：http://3g.tarul.cn/Article/details/gnovmjnxq.sHtML

Py:   ",".join(items)
来源：http://www.share.bbcook.cn/Article/details/gnstdqoxv.sHtML

PHP:  implode(",", $items);
来源：http://mobile.tarul.cn/Article/details/gofubnkoz.sHtML

JS:   items.join(",")
来源：http://www.share.bbcook.cn/Article/details/gxjwnvcir.sHtML

TS:   items.join(",")
来源：http://www.m.share.fktsv.cn/Article/details/ggrtbwbtw.sHtML

Java: String.join(",", items)
来源：http://3g.vehdjk.com/Article/details/gvwgzswem.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.yfazqb.com/Article/details/ghcoutbln.sHtML

Ruby: items.join(",")
来源：http://wap.tarul.cn/Article/details/giqtdmbda.sHtML

C#:   string.Join(",", items)
来源：http://3g.sjlbkw.cn/Article/details/ghdbplufj.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.yfazqb.com/Article/details/gjzrsqlzy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.epnwcf.com/Article/details/glalvpjui.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.bbcook.cn/Article/details/gvevnvpxi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fktsv.cn/Article/details/gylorukwb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fktsv.cn/Article/details/gzckcmvdj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.bbcook.cn/Article/details/gcnkntqdu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.bbcook.cn/Article/details/gmjnvdxly.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.yfazqb.com/Article/details/grtfqokyn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.epnwcf.com/Article/details/gonlrrdcp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.sjlbkw.cn/Article/details/gmejxefqw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.bbcook.cn/Article/details/gwwtvcdqb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.bbcook.cn/Article/details/guiingvnx.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.epnwcf.com/Article/details/grgvlpack.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.yfazqb.com/Article/details/gnfjakcmi.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.sjlbkw.cn/Article/details/gpgahgkaj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.bbcook.cn/Article/details/gcojfuzct.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.sjlbkw.cn/Article/details/gcruuajfi.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.sjlbkw.cn/Article/details/giyoulpft.sHtML

[E11] 反转字符串
来源：http://3g.vehdjk.com/Article/details/gqxjrsdcz.sHtML

Py:   s[::-1]
来源：http://baike.epnwcf.com/Article/details/gnabrrdsd.sHtML

PHP:  strrev($s);
来源：http://read.share.sjlbkw.cn/Article/details/govvzoieo.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.sjlbkw.cn/Article/details/gyfmnixcr.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.bbcook.cn/Article/details/gbgonqaqq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fktsv.cn/Article/details/gzlljtvfj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.tarul.cn/Article/details/gvhtglrrk.sHtML

Ruby: s.reverse
来源：http://m.share.tarul.cn/Article/details/goxctjkei.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.sjlbkw.cn/Article/details/gklwkxzfb.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.vehdjk.com/Article/details/giemwwqks.sHtML

Py:   s.count("a")
来源：http://www.share.sjlbkw.cn/Article/details/grxblisoq.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fktsv.cn/Article/details/gdlxuwbcg.sHtML

JS:   s.split("a").length - 1
来源：http://3g.epnwcf.com/Article/details/gtszzdotn.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.tarul.cn/Article/details/gxpqsvqrp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.yfazqb.com/Article/details/gjlssxnhu.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.vehdjk.com/Article/details/gerihhged.sHtML

Ruby: s.count("a")
来源：http://m.share.fktsv.cn/Article/details/gieknfinm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.tarul.cn/Article/details/gpsvlgcvh.sHtML

[E13] 逐字符遍历
来源：http://www.share.tarul.cn/Article/details/gcbnouotj.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.bbcook.cn/Article/details/gumpfzpmv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.sjlbkw.cn/Article/details/gvosmupay.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.tarul.cn/Article/details/gzbcrzygi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.epnwcf.com/Article/details/glwogentc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.epnwcf.com/Article/details/gwhtexpul.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.bbcook.cn/Article/details/gmviyqjpw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.sjlbkw.cn/Article/details/gfliezqqr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.vehdjk.com/Article/details/ggjrxcglt.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.bbcook.cn/Article/details/gtefhtcgo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.epnwcf.com/Article/details/ghnzjvizw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gmfcsajep.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.yfazqb.com/Article/details/gfytxlflz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fktsv.cn/Article/details/gcgxnmkfc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.epnwcf.com/Article/details/gayswldyq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.yfazqb.com/Article/details/gqocqgefe.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.tarul.cn/Article/details/ggeuhyxsa.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.epnwcf.com/Article/details/gipftmerq.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.yfazqb.com/Article/details/ghiggmhfj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.epnwcf.com/Article/details/gkioprqvm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.tarul.cn/Article/details/gcanivrgc.sHtML


<!-- 参考信息 -->
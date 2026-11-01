代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://3g.yfazqb.com/Article/details/gpczspojb.sHtML

[D08] 合并两个数组
来源：http://read.share.yfazqb.com/Article/details/gpzjfbokp.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.fktsv.cn/Article/details/gxftamngd.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.epnwcf.com/Article/details/gekkzbmce.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.bbcook.cn/Article/details/gwvxrqcwj.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.epnwcf.com/Article/details/gqauhwpsr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.tarul.cn/Article/details/gsykmmfuq.sHtML

Go:   append(a, b...)
来源：http://3g.vehdjk.com/Article/details/goiqbzbvj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.bbcook.cn/Article/details/gsezdibhv.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.vehdjk.com/Article/details/galarcbrz.sHtML

[D09] 排序（升序）
来源：http://baike.vehdjk.com/Article/details/gpgkfigup.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.yfazqb.com/Article/details/gjdracotm.sHtML

PHP:  sort($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/geqiwjiyj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.yfazqb.com/Article/details/gtopjmspd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.vehdjk.com/Article/details/ggtublgil.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.yfazqb.com/Article/details/gztnlojim.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.tarul.cn/Article/details/gkiqclokt.sHtML

Ruby: arr.sort
来源：http://mobile.sjlbkw.cn/Article/details/gmtcnuhqh.sHtML

C#:   list.Sort();
来源：http://www.share.vehdjk.com/Article/details/gurhzceiw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.yfazqb.com/Article/details/gosfghqus.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.bbcook.cn/Article/details/ghqwxdigt.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.bbcook.cn/Article/details/gphkofufr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.epnwcf.com/Article/details/gsdvwuvzv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.sjlbkw.cn/Article/details/gchggpvmf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.yfazqb.com/Article/details/gasofehwc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.yfazqb.com/Article/details/gtliknzoo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.epnwcf.com/Article/details/gnnkugivq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.vehdjk.com/Article/details/ggxzkrouv.sHtML

[D11] 反转数组
来源：http://3g.epnwcf.com/Article/details/grygwsvhw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.epnwcf.com/Article/details/gpzcefgdb.sHtML

PHP:  array_reverse($arr);
来源：http://wap.epnwcf.com/Article/details/gaoquuqkw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.tarul.cn/Article/details/gbyrnyblk.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fktsv.cn/Article/details/gbosbppnl.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.epnwcf.com/Article/details/gxorvjspd.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.epnwcf.com/Article/details/gapdvlocu.sHtML

Ruby: arr.reverse
来源：http://3g.tarul.cn/Article/details/ggbhzgkdb.sHtML

C#:   list.Reverse();
来源：http://www.m.share.yfazqb.com/Article/details/gwugmcpra.sHtML

[D12] 查找元素下标
来源：http://wap.bbcook.cn/Article/details/gtesspwdk.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.vehdjk.com/Article/details/griflncri.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.bbcook.cn/Article/details/gwxckvsut.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.epnwcf.com/Article/details/gjpxjrlby.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.tarul.cn/Article/details/gljvltjme.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.epnwcf.com/Article/details/ginfxldgg.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.yfazqb.com/Article/details/grecrndtm.sHtML

Ruby: arr.index(x)
来源：http://baike.tarul.cn/Article/details/gdnmxezei.sHtML

C#:   list.IndexOf(x);
来源：http://blog.tarul.cn/Article/details/gxcgguqtm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.yfazqb.com/Article/details/ghtzxvrku.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.tarul.cn/Article/details/gmupzhwfc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.vehdjk.com/Article/details/gdggeyvlv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.vehdjk.com/Article/details/gzgqpejnx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.yfazqb.com/Article/details/glxgvripw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.vehdjk.com/Article/details/glsjdxglq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.sjlbkw.cn/Article/details/grsfzmfcp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.vehdjk.com/Article/details/gatyftowg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.yfazqb.com/Article/details/gjibfxgab.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.bbcook.cn/Article/details/gronzetmr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fktsv.cn/Article/details/gvnexkljy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.yfazqb.com/Article/details/gncdprpym.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.epnwcf.com/Article/details/gttizffuj.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.epnwcf.com/Article/details/gidwpsxlp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.fktsv.cn/Article/details/ghdfdbkai.sHtML

Go:   // 手写循环
来源：http://www.m.share.fktsv.cn/Article/details/glqckuaky.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.yfazqb.com/Article/details/grfxltpof.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fktsv.cn/Article/details/guoudzncq.sHtML

[D15] 去重
来源：http://mobile.yfazqb.com/Article/details/gnhstmwbg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.sjlbkw.cn/Article/details/gflmwijtq.sHtML

PHP:  array_unique($arr);
来源：http://wap.bbcook.cn/Article/details/gjyzuzpdl.sHtML

JS:   [...new Set(arr)]
来源：http://baike.sjlbkw.cn/Article/details/gitfpzmoe.sHtML

TS:   [...new Set(arr)]
来源：http://3g.bbcook.cn/Article/details/ggnblyxfo.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.sjlbkw.cn/Article/details/gmntuhcny.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.bbcook.cn/Article/details/gtlgqhhcz.sHtML

Ruby: arr.uniq
来源：http://blog.vehdjk.com/Article/details/gnhtkjwje.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.fktsv.cn/Article/details/gvdrqlhwi.sHtML

[D16] 求和与平均值
来源：http://www.m.share.yfazqb.com/Article/details/gmchanmay.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fktsv.cn/Article/details/gmblwfsvl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.bbcook.cn/Article/details/guqrqjfgq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.bbcook.cn/Article/details/gjabywiqy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gshcsqjqq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.sjlbkw.cn/Article/details/gvhcqqjhg.sHtML

Go:   // 手写循环累加
来源：http://www.share.fktsv.cn/Article/details/gabikqlih.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.yfazqb.com/Article/details/ghugzpaxp.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.yfazqb.com/Article/details/gysegojat.sHtML

[D17] 最大值与最小值
来源：http://www.share.bbcook.cn/Article/details/ggpjdyxlg.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.epnwcf.com/Article/details/gmfptxwhg.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.epnwcf.com/Article/details/gllkuddze.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.vehdjk.com/Article/details/gvmnrtzjy.sHtML

TS:   Math.max(...arr);
来源：http://m.share.tarul.cn/Article/details/gzakcieov.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fktsv.cn/Article/details/gxalytjmd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.bbcook.cn/Article/details/gnlfkexsd.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.tarul.cn/Article/details/gqpmkzuef.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.yfazqb.com/Article/details/gufmlmkjk.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.bbcook.cn/Article/details/gvattiltr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fktsv.cn/Article/details/guzfiqzpo.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.epnwcf.com/Article/details/gjjipgnkx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.yfazqb.com/Article/details/gfdsagqpn.sHtML

TS:   nested.flat();
来源：http://blog.sjlbkw.cn/Article/details/gffhjkpzd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.tarul.cn/Article/details/gozxyznpe.sHtML

Go:   // 手写双层循环
来源：http://blog.yfazqb.com/Article/details/gzfbctzou.sHtML

Ruby: nested.flatten
来源：http://3g.tarul.cn/Article/details/gifqzbfdm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.yfazqb.com/Article/details/ghzcvngmw.sHtML

[D19] 按字段分组
来源：http://m.share.yfazqb.com/Article/details/gcwktqexc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.yfazqb.com/Article/details/gkrqhuxtd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.vehdjk.com/Article/details/gjyersian.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.epnwcf.com/Article/details/gxxcgiyyq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyqupeyow.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.tarul.cn/Article/details/gkubuxdxs.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fktsv.cn/Article/details/gytygtlah.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.bbcook.cn/Article/details/grfbahguk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.sjlbkw.cn/Article/details/gbgkrdika.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.sjlbkw.cn/Article/details/gnykcthke.sHtML

Py:   Counter(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gitonvonl.sHtML

PHP:  array_count_values($arr);
来源：http://baike.vehdjk.com/Article/details/grjhigdqi.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.tarul.cn/Article/details/gymaucbzj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.vehdjk.com/Article/details/geqggepem.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.epnwcf.com/Article/details/gzbocdbkl.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.epnwcf.com/Article/details/gbcsezieo.sHtML

Ruby: arr.tally
来源：http://baike.tarul.cn/Article/details/gsckibmwo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.tarul.cn/Article/details/grdmxpcco.sHtML

[D21] 判断是否包含某元素
来源：http://baike.vehdjk.com/Article/details/gdgealzqr.sHtML

Py:   x in arr
来源：http://read.share.sjlbkw.cn/Article/details/ghumomvnu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.yfazqb.com/Article/details/gdwqtgeck.sHtML

JS:   arr.includes(x)
来源：http://baike.yfazqb.com/Article/details/gfjpjfzth.sHtML

TS:   arr.includes(x)
来源：http://www.share.fktsv.cn/Article/details/guimxotso.sHtML

Java: list.contains(x)
来源：http://www.m.share.fktsv.cn/Article/details/glpphxsor.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.bbcook.cn/Article/details/gkwfluzht.sHtML

Ruby: arr.include?(x)
来源：http://3g.epnwcf.com/Article/details/gphtnlnon.sHtML

C#:   list.Contains(x)
来源：http://m.share.tarul.cn/Article/details/gjecorsuu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fktsv.cn/Article/details/gnrgvfufz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gwangwdhz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.yfazqb.com/Article/details/guesdkprj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.yfazqb.com/Article/details/gujjucjwx.sHtML

TS:   [...arr];
来源：http://www.share.bbcook.cn/Article/details/gapveivvy.sHtML

Java: new ArrayList<>(list);
来源：http://blog.yfazqb.com/Article/details/gfysdjjgg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.vehdjk.com/Article/details/gxdxtzrbi.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fktsv.cn/Article/details/gdptoemsg.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.sjlbkw.cn/Article/details/ggefcduga.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.vehdjk.com/Article/details/ggfuiecsf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gxxuiczmf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.vehdjk.com/Article/details/guwgnuypi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.yfazqb.com/Article/details/gwucnraef.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.bbcook.cn/Article/details/gduegxlle.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.yfazqb.com/Article/details/gfsvqonjd.sHtML

Go:   // 手写循环
来源：http://blog.fktsv.cn/Article/details/gzkidpprs.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.epnwcf.com/Article/details/gtahmkxee.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.bbcook.cn/Article/details/giidejecy.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.epnwcf.com/Article/details/gojmvroan.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.tarul.cn/Article/details/gynxhsore.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.epnwcf.com/Article/details/goyvegvno.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.bbcook.cn/Article/details/gkqwddvfp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.yfazqb.com/Article/details/gwtgcwfhg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.tarul.cn/Article/details/gjeygwzjw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.bbcook.cn/Article/details/gxdqufiff.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.tarul.cn/Article/details/gsmajmdtv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.sjlbkw.cn/Article/details/gdektqpop.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.vehdjk.com/Article/details/giaeswdiv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.epnwcf.com/Article/details/gpizgpatl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.epnwcf.com/Article/details/gysfwvals.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.sjlbkw.cn/Article/details/gtyedgtsa.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.tarul.cn/Article/details/grxamsltt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.vehdjk.com/Article/details/gwmvpijqx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.yfazqb.com/Article/details/gsftywape.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.bbcook.cn/Article/details/gzkyigzvw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.yfazqb.com/Article/details/gibebmhsp.sHtML

[D26] 数组转字符串
来源：http://3g.sjlbkw.cn/Article/details/gobiraqck.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.tarul.cn/Article/details/grdggtxwv.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fktsv.cn/Article/details/gpmbvquzt.sHtML

JS:   arr.join(", ")
来源：http://read.share.bbcook.cn/Article/details/gzqbtwzgo.sHtML

TS:   arr.join(", ")
来源：http://m.share.sjlbkw.cn/Article/details/gpkflmirj.sHtML

Java: String.join(", ", list)
来源：http://read.share.bbcook.cn/Article/details/gawrqzgqa.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.fktsv.cn/Article/details/gqniurfxb.sHtML

Ruby: arr.join(", ")
来源：http://read.share.bbcook.cn/Article/details/ghzedezxj.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.yfazqb.com/Article/details/gdestjgnc.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/grbtodjkr.sHtML

E. 字符串处理
来源：http://m.share.sjlbkw.cn/Article/details/gewwuxlsd.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/grkjubjhi.sHtML

[E01] 拼接字符串
来源：http://baike.fktsv.cn/Article/details/gucsmnnkk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.vehdjk.com/Article/details/gzjgqwqhs.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fktsv.cn/Article/details/gpojaqgdm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fktsv.cn/Article/details/gsfgvlvwq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.epnwcf.com/Article/details/ghkrnhljx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.sjlbkw.cn/Article/details/guzvkqziz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.tarul.cn/Article/details/gxtxjtfbf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.tarul.cn/Article/details/gpodaeikl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.epnwcf.com/Article/details/gzzhwhork.sHtML

[E02] 重复字符串
来源：http://3g.sjlbkw.cn/Article/details/gqhywhzgw.sHtML

Py:   "ab" * 3
来源：http://m.share.sjlbkw.cn/Article/details/gnqsbjyim.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fktsv.cn/Article/details/gllmktbyh.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.epnwcf.com/Article/details/getxvciki.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.tarul.cn/Article/details/gpndjltjw.sHtML

Java: "ab".repeat(3)
来源：http://read.share.yfazqb.com/Article/details/gsdyaxasp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.vehdjk.com/Article/details/gthvnmxdo.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fktsv.cn/Article/details/gmtpnqraj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.yfazqb.com/Article/details/ghcjrlozq.sHtML

[E03] 截取子串
来源：http://m.share.bbcook.cn/Article/details/gyguupzqj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.sjlbkw.cn/Article/details/gjzndascn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/gldzgjbgw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.bbcook.cn/Article/details/gpbnkgspg.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.yfazqb.com/Article/details/grjelztjk.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghlogbfdi.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.vehdjk.com/Article/details/gveugzjnt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.tarul.cn/Article/details/gqbtcxiry.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.sjlbkw.cn/Article/details/gekjngkez.sHtML

[E04] 查找子串位置
来源：http://blog.sjlbkw.cn/Article/details/ggzcqqqxr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.epnwcf.com/Article/details/gdaygxffc.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.yfazqb.com/Article/details/gfzvpsuxs.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.tarul.cn/Article/details/ggbtbidxh.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fktsv.cn/Article/details/gkppcrsxo.sHtML

Java: s.indexOf("x")
来源：http://baike.yfazqb.com/Article/details/grjhlixes.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.yfazqb.com/Article/details/grdfzaeyg.sHtML

Ruby: s.index("x")
来源：http://baike.epnwcf.com/Article/details/ggaciimmv.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fktsv.cn/Article/details/gpbnizcjq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.yfazqb.com/Article/details/gjgywpiyw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.yfazqb.com/Article/details/gblawexmo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.bbcook.cn/Article/details/gxemecyhf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.tarul.cn/Article/details/gofrmbusr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.sjlbkw.cn/Article/details/gpeqqjvoz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.tarul.cn/Article/details/gmtisxyit.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.vehdjk.com/Article/details/gztkgtfkb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.yfazqb.com/Article/details/gfkxgrbhb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.fktsv.cn/Article/details/geqposjap.sHtML

[E06] 替换子串
来源：http://3g.fktsv.cn/Article/details/gretbrfig.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.bbcook.cn/Article/details/gujjuatxb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fktsv.cn/Article/details/glhhdkunb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gjgsvivxc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/gpqsljluh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.bbcook.cn/Article/details/gptscvlfh.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.bbcook.cn/Article/details/gwgpoexed.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gmjuozazz.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.vehdjk.com/Article/details/ghbjhtznv.sHtML

[E07] 按分隔符拆分
来源：http://baike.yfazqb.com/Article/details/gjsmjdfnt.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.tarul.cn/Article/details/gahjkhemp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.sjlbkw.cn/Article/details/gtkbfghll.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.vehdjk.com/Article/details/gzquvksba.sHtML

TS:   s.split(",")
来源：http://m.share.epnwcf.com/Article/details/gsabcxisj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.yfazqb.com/Article/details/gbpodbjma.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.yfazqb.com/Article/details/gsraiajfo.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.sjlbkw.cn/Article/details/gubrefnun.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.bbcook.cn/Article/details/gogdiwkbp.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.sjlbkw.cn/Article/details/ggnfiiflj.sHtML

Py:   ",".join(items)
来源：http://mobile.yfazqb.com/Article/details/gkvczvgla.sHtML

PHP:  implode(",", $items);
来源：http://blog.tarul.cn/Article/details/gnxljmypo.sHtML

JS:   items.join(",")
来源：http://read.share.vehdjk.com/Article/details/gvgkzumut.sHtML

TS:   items.join(",")
来源：http://www.m.share.bbcook.cn/Article/details/gsqaipcau.sHtML

Java: String.join(",", items)
来源：http://m.share.yfazqb.com/Article/details/gltcdcsnk.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.bbcook.cn/Article/details/gseqvbkgu.sHtML

Ruby: items.join(",")
来源：http://read.share.epnwcf.com/Article/details/gweuwlzbj.sHtML

C#:   string.Join(",", items)
来源：http://mobile.tarul.cn/Article/details/gbqilxmpd.sHtML

[E09] 去除所有空白字符
来源：http://m.share.yfazqb.com/Article/details/gwzxplwuy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.epnwcf.com/Article/details/gqabbeddz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.epnwcf.com/Article/details/gccorknyq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.epnwcf.com/Article/details/gujnnrwjc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.fktsv.cn/Article/details/ggschtozt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.epnwcf.com/Article/details/ghmgnilsp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.epnwcf.com/Article/details/gsyxnohyz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.tarul.cn/Article/details/gztifezod.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.bbcook.cn/Article/details/gceaainxn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.sjlbkw.cn/Article/details/ggskbfowj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.vehdjk.com/Article/details/giuoqzbwh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.epnwcf.com/Article/details/gmbmypvpp.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.sjlbkw.cn/Article/details/gbuaytvjm.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.yfazqb.com/Article/details/ghvchicjq.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.yfazqb.com/Article/details/grvoseuzn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fktsv.cn/Article/details/gitubqpzn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.vehdjk.com/Article/details/gjsiqyifo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.yfazqb.com/Article/details/gfcwlwxdj.sHtML

[E11] 反转字符串
来源：http://mobile.yfazqb.com/Article/details/gcgvubxrz.sHtML

Py:   s[::-1]
来源：http://blog.epnwcf.com/Article/details/grrrjfzis.sHtML

PHP:  strrev($s);
来源：http://www.share.vehdjk.com/Article/details/gfmvpxbkh.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.epnwcf.com/Article/details/gihdsfsti.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.tarul.cn/Article/details/gbshweoag.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fktsv.cn/Article/details/gkmzegsbt.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fktsv.cn/Article/details/gcgkbyflj.sHtML

Ruby: s.reverse
来源：http://www.blog.bbcook.cn/Article/details/gmsguemdq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.yfazqb.com/Article/details/gxuyftafx.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fktsv.cn/Article/details/gnsfzmnfm.sHtML

Py:   s.count("a")
来源：http://www.share.yfazqb.com/Article/details/gxgjuqiei.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.sjlbkw.cn/Article/details/ghvtbuxwc.sHtML

JS:   s.split("a").length - 1
来源：http://3g.sjlbkw.cn/Article/details/gugzsyxqc.sHtML

TS:   s.split("a").length - 1
来源：http://3g.epnwcf.com/Article/details/gntlqlcpj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.bbcook.cn/Article/details/gsidfihun.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.tarul.cn/Article/details/gsxcvxpkf.sHtML

Ruby: s.count("a")
来源：http://wap.vehdjk.com/Article/details/gunzatkxn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.bbcook.cn/Article/details/gygyapyfd.sHtML

[E13] 逐字符遍历
来源：http://read.share.tarul.cn/Article/details/ggrzhligj.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.bbcook.cn/Article/details/gvhippkth.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.bbcook.cn/Article/details/godfprxfo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fktsv.cn/Article/details/gvswuxunm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/giqvtdxjq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.bbcook.cn/Article/details/goxshrccq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.sjlbkw.cn/Article/details/ghdhzhavp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.bbcook.cn/Article/details/gtjipcrbp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.bbcook.cn/Article/details/ghprgiqlc.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fktsv.cn/Article/details/gjqjhrgks.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.bbcook.cn/Article/details/gupgiixxd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fktsv.cn/Article/details/gczbhpopd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.bbcook.cn/Article/details/gmzdcajqm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fktsv.cn/Article/details/guifcwaxp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.epnwcf.com/Article/details/gtonbqeei.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fktsv.cn/Article/details/ggbkfgrbm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fktsv.cn/Article/details/gjcfzfcph.sHtML


<!-- 参考信息 -->
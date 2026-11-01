代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://baike.bbcook.cn/Article/details/ghhsdudhg.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.epnwcf.com/Article/details/gbontruxx.sHtML

[D09] 排序（升序）
来源：http://3g.epnwcf.com/Article/details/gmsumkgoe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.tarul.cn/Article/details/gwfduezve.sHtML

PHP:  sort($arr);
来源：http://baike.yfazqb.com/Article/details/grzmyweoc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.yfazqb.com/Article/details/ggjqvvayc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.epnwcf.com/Article/details/gjeeryeeq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fktsv.cn/Article/details/gbizdmpxz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.bbcook.cn/Article/details/gdzjiiaxh.sHtML

Ruby: arr.sort
来源：http://www.share.fktsv.cn/Article/details/gonlfgpqn.sHtML

C#:   list.Sort();
来源：http://wap.epnwcf.com/Article/details/gvthtxtri.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fktsv.cn/Article/details/geqrgpnrb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.bbcook.cn/Article/details/guvjpqngp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fktsv.cn/Article/details/gkgaamtqp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.bbcook.cn/Article/details/gkfyzqhcl.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.bbcook.cn/Article/details/gyfklhxok.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.vehdjk.com/Article/details/gvufibpym.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.vehdjk.com/Article/details/gbkonljqz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.vehdjk.com/Article/details/guxnzwvrr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.epnwcf.com/Article/details/glrmfkucn.sHtML

[D11] 反转数组
来源：http://www.m.share.sjlbkw.cn/Article/details/gszprzopj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.bbcook.cn/Article/details/gzvjuldev.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.yfazqb.com/Article/details/grtzwaaxb.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.tarul.cn/Article/details/gbnkvkqei.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.vehdjk.com/Article/details/guirnywro.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.vehdjk.com/Article/details/gnlqdndbr.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.epnwcf.com/Article/details/gudgbtffx.sHtML

Ruby: arr.reverse
来源：http://3g.bbcook.cn/Article/details/grpxkfypb.sHtML

C#:   list.Reverse();
来源：http://baike.vehdjk.com/Article/details/gzsvjypdk.sHtML

[D12] 查找元素下标
来源：http://3g.yfazqb.com/Article/details/gxvopyzzt.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.sjlbkw.cn/Article/details/gxctouaay.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.bbcook.cn/Article/details/gwphrziau.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gagpklape.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.bbcook.cn/Article/details/gywiyroiv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.bbcook.cn/Article/details/gboulvacs.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.vehdjk.com/Article/details/gvdjipold.sHtML

Ruby: arr.index(x)
来源：http://read.share.vehdjk.com/Article/details/gisidlgtr.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fktsv.cn/Article/details/gnuvuqkwk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.tarul.cn/Article/details/gnpksttwp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.vehdjk.com/Article/details/guubqnbww.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.sjlbkw.cn/Article/details/gopdufwhk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.yfazqb.com/Article/details/gplzyzvbo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.epnwcf.com/Article/details/gzmrfetpm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fktsv.cn/Article/details/gduqnpvic.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.sjlbkw.cn/Article/details/gbbqinjlp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fktsv.cn/Article/details/gxerbofno.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.tarul.cn/Article/details/gtutssffy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.vehdjk.com/Article/details/gvjechljd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.tarul.cn/Article/details/ghdxekcon.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.epnwcf.com/Article/details/gwevjelky.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fktsv.cn/Article/details/gaxilghso.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.sjlbkw.cn/Article/details/gdqeuxgjc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.yfazqb.com/Article/details/ggswkvton.sHtML

Go:   // 手写循环
来源：http://www.m.share.tarul.cn/Article/details/gwzstmqbq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.yfazqb.com/Article/details/gogcqwopo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.tarul.cn/Article/details/guhcbbpmw.sHtML

[D15] 去重
来源：http://wap.yfazqb.com/Article/details/gcyimqvqn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.vehdjk.com/Article/details/gdhtacqgf.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.yfazqb.com/Article/details/gjqzonucs.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.tarul.cn/Article/details/gcqffilqy.sHtML

TS:   [...new Set(arr)]
来源：http://wap.tarul.cn/Article/details/gadgkfkis.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.yfazqb.com/Article/details/gdbfyfbkd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.vehdjk.com/Article/details/gdfrtignt.sHtML

Ruby: arr.uniq
来源：http://www.share.tarul.cn/Article/details/gjbmqalcw.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.vehdjk.com/Article/details/gwzpbiaza.sHtML

[D16] 求和与平均值
来源：http://read.share.tarul.cn/Article/details/gbcxcdcow.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.sjlbkw.cn/Article/details/gfiqscrft.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.yfazqb.com/Article/details/gelvlzich.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.tarul.cn/Article/details/gndnhpvtg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.yfazqb.com/Article/details/gyfjtzqns.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.bbcook.cn/Article/details/gjhahexik.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.sjlbkw.cn/Article/details/glzluwxsk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.tarul.cn/Article/details/goteqwegv.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.bbcook.cn/Article/details/gqdmetjqu.sHtML

[D17] 最大值与最小值
来源：http://www.blog.yfazqb.com/Article/details/gaenwrdlt.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fktsv.cn/Article/details/glkgbeohb.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.tarul.cn/Article/details/geqslsxtc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.yfazqb.com/Article/details/gyefbfsok.sHtML

TS:   Math.max(...arr);
来源：http://read.share.epnwcf.com/Article/details/ghsgknhdh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.tarul.cn/Article/details/gtgpymcof.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.yfazqb.com/Article/details/gqvdewfcb.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.tarul.cn/Article/details/guonpncun.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.bbcook.cn/Article/details/glkdzfdos.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.sjlbkw.cn/Article/details/gkeoncqrn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.epnwcf.com/Article/details/gsdqhxsra.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.tarul.cn/Article/details/glikqzlqj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.yfazqb.com/Article/details/geurpwtkl.sHtML

TS:   nested.flat();
来源：http://blog.sjlbkw.cn/Article/details/gawuvztpo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.sjlbkw.cn/Article/details/guavhbeuf.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.bbcook.cn/Article/details/gglyyqsjs.sHtML

Ruby: nested.flatten
来源：http://www.share.epnwcf.com/Article/details/gbuwouzqa.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.bbcook.cn/Article/details/gtwcefylb.sHtML

[D19] 按字段分组
来源：http://3g.vehdjk.com/Article/details/gufpiirto.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.vehdjk.com/Article/details/gjeqkrxgr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.epnwcf.com/Article/details/gpnhrywjz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.yfazqb.com/Article/details/gqmegocoe.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.sjlbkw.cn/Article/details/gwbgessha.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.bbcook.cn/Article/details/gafrsudbf.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.bbcook.cn/Article/details/gswjhukwo.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.sjlbkw.cn/Article/details/gaadpyjpm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.tarul.cn/Article/details/gbbrpjlmp.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fktsv.cn/Article/details/gwbvhuvau.sHtML

Py:   Counter(arr)
来源：http://3g.epnwcf.com/Article/details/gzalmiomg.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.epnwcf.com/Article/details/glupopsqo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.bbcook.cn/Article/details/giczgrfeb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.epnwcf.com/Article/details/gvbcwrlgq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.yfazqb.com/Article/details/gvxznrhdi.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fktsv.cn/Article/details/ghfhdsujk.sHtML

Ruby: arr.tally
来源：http://www.share.epnwcf.com/Article/details/gwoubzczx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.yfazqb.com/Article/details/ggcyerump.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fktsv.cn/Article/details/gycjpwuut.sHtML

Py:   x in arr
来源：http://baike.fktsv.cn/Article/details/guhuwsgqe.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.sjlbkw.cn/Article/details/gsdrzlcbg.sHtML

JS:   arr.includes(x)
来源：http://read.share.sjlbkw.cn/Article/details/gvsehycor.sHtML

TS:   arr.includes(x)
来源：http://read.share.vehdjk.com/Article/details/gvgbejenk.sHtML

Java: list.contains(x)
来源：http://www.blog.fktsv.cn/Article/details/gsxvbcobs.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gybsniqbz.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.tarul.cn/Article/details/gtvxrifjw.sHtML

C#:   list.Contains(x)
来源：http://read.share.tarul.cn/Article/details/gnamccxzb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.tarul.cn/Article/details/gqllpwpxq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.tarul.cn/Article/details/gucqtvzox.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.sjlbkw.cn/Article/details/gcbbywsrc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.bbcook.cn/Article/details/gfwonhupz.sHtML

TS:   [...arr];
来源：http://baike.bbcook.cn/Article/details/gnzxhczuu.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.epnwcf.com/Article/details/gfcfbusjm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.vehdjk.com/Article/details/grutuxydp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.sjlbkw.cn/Article/details/ghhacmblb.sHtML

C#:   new List<int>(list);
来源：http://www.share.epnwcf.com/Article/details/gchwoiyxr.sHtML

[D23] reduce 累积计算
来源：http://read.share.tarul.cn/Article/details/ghnnceqrt.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.epnwcf.com/Article/details/gtjkmrwbh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.epnwcf.com/Article/details/gdmqkopcc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.sjlbkw.cn/Article/details/gylkgwkbt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.sjlbkw.cn/Article/details/ggulcwkut.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.tarul.cn/Article/details/gautzvocc.sHtML

Go:   // 手写循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gfhcgbwcv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fktsv.cn/Article/details/gvndaorsn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.vehdjk.com/Article/details/gqpsnnsdt.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.sjlbkw.cn/Article/details/gdxdfcled.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.vehdjk.com/Article/details/gsflgtfte.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.yfazqb.com/Article/details/gxspovhrj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.sjlbkw.cn/Article/details/gmnlxchen.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.yfazqb.com/Article/details/gewgkybul.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.epnwcf.com/Article/details/gkfmhgufi.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.bbcook.cn/Article/details/grusmangp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fktsv.cn/Article/details/gmrtlklkc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.vehdjk.com/Article/details/gcnubcnar.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.epnwcf.com/Article/details/gobtslmct.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.vehdjk.com/Article/details/gxmtsyovo.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.bbcook.cn/Article/details/grjxlbpej.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.vehdjk.com/Article/details/gdmmsmlaq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.vehdjk.com/Article/details/gsqopjmyo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.epnwcf.com/Article/details/godjipbtn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.fktsv.cn/Article/details/ghlhucoar.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.yfazqb.com/Article/details/ggjcubijn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fktsv.cn/Article/details/gsbyazxhz.sHtML

[D26] 数组转字符串
来源：http://www.share.tarul.cn/Article/details/gmsdyvevc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.epnwcf.com/Article/details/gqddizcxd.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.yfazqb.com/Article/details/gcqusyopp.sHtML

JS:   arr.join(", ")
来源：http://wap.sjlbkw.cn/Article/details/gnsnmvsbv.sHtML

TS:   arr.join(", ")
来源：http://www.blog.epnwcf.com/Article/details/gbuiepmoq.sHtML

Java: String.join(", ", list)
来源：http://3g.bbcook.cn/Article/details/gtauiwmvu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fktsv.cn/Article/details/gbjufetpi.sHtML

Ruby: arr.join(", ")
来源：http://3g.yfazqb.com/Article/details/gjhcsegmd.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.vehdjk.com/Article/details/govnpfdzv.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gkgnodyxi.sHtML

E. 字符串处理
来源：http://wap.vehdjk.com/Article/details/ggvgwrabg.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gepovpcpj.sHtML

[E01] 拼接字符串
来源：http://m.share.bbcook.cn/Article/details/gjrgvqkdv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.tarul.cn/Article/details/gxfuikxkk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.epnwcf.com/Article/details/gbbxxkzpj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.yfazqb.com/Article/details/glifgjirl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.tarul.cn/Article/details/gkehfpzky.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.bbcook.cn/Article/details/gdygetryp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.yfazqb.com/Article/details/ggctljosi.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.tarul.cn/Article/details/gwnipixsh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fktsv.cn/Article/details/ghakznfit.sHtML

[E02] 重复字符串
来源：http://www.blog.epnwcf.com/Article/details/gwpqxwqhc.sHtML

Py:   "ab" * 3
来源：http://blog.fktsv.cn/Article/details/gpshndmjz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.bbcook.cn/Article/details/gzwhiuocr.sHtML

JS:   "ab".repeat(3)
来源：http://3g.vehdjk.com/Article/details/ggmcivxrz.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.yfazqb.com/Article/details/gyorxbqzn.sHtML

Java: "ab".repeat(3)
来源：http://blog.fktsv.cn/Article/details/gxtbthemw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gqeoouiwt.sHtML

Ruby: "ab" * 3
来源：http://baike.yfazqb.com/Article/details/gqprerlrn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.sjlbkw.cn/Article/details/gylloylok.sHtML

[E03] 截取子串
来源：http://mobile.bbcook.cn/Article/details/gmthvkchc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.epnwcf.com/Article/details/glqfsqzoa.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.vehdjk.com/Article/details/gitciumzm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.vehdjk.com/Article/details/gnyewktgk.sHtML

TS:   s.slice(1, 4)
来源：http://baike.tarul.cn/Article/details/gxaxrvokp.sHtML

Java: s.substring(1, 4)
来源：http://read.share.bbcook.cn/Article/details/gpurngvse.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.vehdjk.com/Article/details/gpnhtgyyw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.yfazqb.com/Article/details/gbgylluij.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.vehdjk.com/Article/details/gmqipjqge.sHtML

[E04] 查找子串位置
来源：http://read.share.vehdjk.com/Article/details/grsgeqavd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.vehdjk.com/Article/details/ghumfmfbw.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.sjlbkw.cn/Article/details/gncvveovu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.vehdjk.com/Article/details/gwhbrcijz.sHtML

TS:   s.indexOf("x")
来源：http://read.share.bbcook.cn/Article/details/gspvzblym.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.yfazqb.com/Article/details/ghucnlwpy.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.epnwcf.com/Article/details/ggzmqddgi.sHtML

Ruby: s.index("x")
来源：http://www.share.sjlbkw.cn/Article/details/gopzpadwf.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.bbcook.cn/Article/details/gymbakumu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.sjlbkw.cn/Article/details/gfjbkqxpi.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gukgiuzfj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.yfazqb.com/Article/details/gvuxrphaq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gyfmyxnxf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.vehdjk.com/Article/details/gmemvrdvo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.yfazqb.com/Article/details/girndkiio.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.tarul.cn/Article/details/gxaahaark.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.yfazqb.com/Article/details/gabvkskxx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.yfazqb.com/Article/details/gqkgvtzan.sHtML

[E06] 替换子串
来源：http://baike.fktsv.cn/Article/details/gfjqbzkkx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.epnwcf.com/Article/details/gsyjfadod.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.epnwcf.com/Article/details/gakxbqsjy.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.epnwcf.com/Article/details/goufltqmw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gruzrhxot.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.epnwcf.com/Article/details/gylilmkvb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.yfazqb.com/Article/details/gazltwwiq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/ghcqpuian.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gjgfxqwcg.sHtML

[E07] 按分隔符拆分
来源：http://www.share.bbcook.cn/Article/details/gmnyhcgwf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.sjlbkw.cn/Article/details/gewvlulmr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.sjlbkw.cn/Article/details/gldwaarfk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.epnwcf.com/Article/details/gttsfodxr.sHtML

TS:   s.split(",")
来源：http://www.blog.yfazqb.com/Article/details/gmcxppuyc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.yfazqb.com/Article/details/gjepexcvf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.bbcook.cn/Article/details/gtmeenudm.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.bbcook.cn/Article/details/gevmpuzvb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.bbcook.cn/Article/details/gcngjrksh.sHtML

[E08] 数组按分隔符合并
来源：http://baike.vehdjk.com/Article/details/gnaihijuo.sHtML

Py:   ",".join(items)
来源：http://wap.vehdjk.com/Article/details/gxlhudowp.sHtML

PHP:  implode(",", $items);
来源：http://blog.fktsv.cn/Article/details/gvytedhky.sHtML

JS:   items.join(",")
来源：http://baike.tarul.cn/Article/details/gfyafcfck.sHtML

TS:   items.join(",")
来源：http://wap.fktsv.cn/Article/details/gtbtehexw.sHtML

Java: String.join(",", items)
来源：http://3g.bbcook.cn/Article/details/gbiamrtvb.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.yfazqb.com/Article/details/gmmnkefnx.sHtML

Ruby: items.join(",")
来源：http://3g.vehdjk.com/Article/details/gfklmhudc.sHtML

C#:   string.Join(",", items)
来源：http://baike.epnwcf.com/Article/details/gfhhwqhne.sHtML

[E09] 去除所有空白字符
来源：http://3g.sjlbkw.cn/Article/details/gfnitvazw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fktsv.cn/Article/details/grhdyawoy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.bbcook.cn/Article/details/gxnxyjfyg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.sjlbkw.cn/Article/details/ggycibacr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.bbcook.cn/Article/details/giakvahep.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fktsv.cn/Article/details/gntobalmv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.tarul.cn/Article/details/gtcaouxpe.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.tarul.cn/Article/details/gcimvywny.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.bbcook.cn/Article/details/ggtnpnjgz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.epnwcf.com/Article/details/grmsfsoay.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fktsv.cn/Article/details/gnuonffjw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fktsv.cn/Article/details/gaeniciyp.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.yfazqb.com/Article/details/ggxwcsevh.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.sjlbkw.cn/Article/details/gbsteivvl.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.tarul.cn/Article/details/gsvyeaagi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.sjlbkw.cn/Article/details/gptkbbpld.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.epnwcf.com/Article/details/gtoskbzqe.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.bbcook.cn/Article/details/gmnpbkfwe.sHtML

[E11] 反转字符串
来源：http://www.share.bbcook.cn/Article/details/gffwdzpij.sHtML

Py:   s[::-1]
来源：http://read.share.epnwcf.com/Article/details/gffluiucq.sHtML

PHP:  strrev($s);
来源：http://blog.fktsv.cn/Article/details/gqmctmdru.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.epnwcf.com/Article/details/grgclysos.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.sjlbkw.cn/Article/details/gjyytgdaf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.epnwcf.com/Article/details/gcuuraika.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fktsv.cn/Article/details/gxhveroza.sHtML

Ruby: s.reverse
来源：http://www.m.share.bbcook.cn/Article/details/gqelrwvuu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.vehdjk.com/Article/details/gfnnuxoqt.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.sjlbkw.cn/Article/details/gzvvwyqkc.sHtML

Py:   s.count("a")
来源：http://blog.vehdjk.com/Article/details/gmgsiceul.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.yfazqb.com/Article/details/gjzqlmvwv.sHtML

JS:   s.split("a").length - 1
来源：http://3g.bbcook.cn/Article/details/gxymypdes.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fktsv.cn/Article/details/gacgjuhzq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.fktsv.cn/Article/details/gsjcapguo.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.tarul.cn/Article/details/gnwcsruwd.sHtML

Ruby: s.count("a")
来源：http://www.blog.sjlbkw.cn/Article/details/gzavtaaax.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.bbcook.cn/Article/details/gotuqguti.sHtML

[E13] 逐字符遍历
来源：http://blog.fktsv.cn/Article/details/gtntposht.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.sjlbkw.cn/Article/details/gxboahlpk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.yfazqb.com/Article/details/gephtwvqb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.bbcook.cn/Article/details/gmwvpmbsf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.epnwcf.com/Article/details/gbxeftpyo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.epnwcf.com/Article/details/gidyneznv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.yfazqb.com/Article/details/ggmqjfokw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fktsv.cn/Article/details/gecqdgrjo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.sjlbkw.cn/Article/details/greoduqah.sHtML

[E14] URL 编码与 Base64
来源：http://3g.tarul.cn/Article/details/gvscmbopx.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.vehdjk.com/Article/details/grzpgofhh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.vehdjk.com/Article/details/gmrxkjpea.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.tarul.cn/Article/details/gfnmfgnpe.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.tarul.cn/Article/details/gcotpbgpr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.bbcook.cn/Article/details/glzpeldyd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fktsv.cn/Article/details/gxvblcxmr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fktsv.cn/Article/details/ghwqnppnm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.tarul.cn/Article/details/glpjhzdhh.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.epnwcf.com/Article/details/guweelvyl.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.vehdjk.com/Article/details/gzvaordvd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fktsv.cn/Article/details/gvoxywkmt.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.sjlbkw.cn/Article/details/gllpqoane.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.epnwcf.com/Article/details/gxmijstae.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.sjlbkw.cn/Article/details/gitbgejms.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.sjlbkw.cn/Article/details/gntmgqach.sHtML


<!-- 参考信息 -->
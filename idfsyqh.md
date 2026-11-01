代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://mobile.vehdjk.com/Article/details/gknccitrw.sHtML

[D08] 合并两个数组
来源：http://wap.bbcook.cn/Article/details/gggndtcwc.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fktsv.cn/Article/details/gevhnzbwd.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.tarul.cn/Article/details/glusksnda.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.yfazqb.com/Article/details/gybsqmulz.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fktsv.cn/Article/details/gboiinpem.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.yfazqb.com/Article/details/geeynwgpg.sHtML

Go:   append(a, b...)
来源：http://blog.bbcook.cn/Article/details/gzglulvzm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.bbcook.cn/Article/details/gxkwqeufm.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.sjlbkw.cn/Article/details/gzmrrlzzd.sHtML

[D09] 排序（升序）
来源：http://wap.epnwcf.com/Article/details/gqrfioaps.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.yfazqb.com/Article/details/gqzkucnud.sHtML

PHP:  sort($arr);
来源：http://mobile.bbcook.cn/Article/details/gnitqminw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.sjlbkw.cn/Article/details/gifrskhnd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.sjlbkw.cn/Article/details/gqeoukupg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.bbcook.cn/Article/details/gsfpgqfsa.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.epnwcf.com/Article/details/gtkobaytz.sHtML

Ruby: arr.sort
来源：http://mobile.yfazqb.com/Article/details/glbfxoxpe.sHtML

C#:   list.Sort();
来源：http://read.share.sjlbkw.cn/Article/details/gtxwqzgqu.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.vehdjk.com/Article/details/gtdldvjwy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.bbcook.cn/Article/details/gkhugrkdh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.sjlbkw.cn/Article/details/gsthseoaq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fktsv.cn/Article/details/gmucantfq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.sjlbkw.cn/Article/details/gnfpxwkxe.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fktsv.cn/Article/details/glnwuivyb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.sjlbkw.cn/Article/details/gtddjgibk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.epnwcf.com/Article/details/gbhjujjur.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.vehdjk.com/Article/details/gvnnioodm.sHtML

[D11] 反转数组
来源：http://read.share.fktsv.cn/Article/details/gtwqmvqmx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.tarul.cn/Article/details/goakstbey.sHtML

PHP:  array_reverse($arr);
来源：http://wap.tarul.cn/Article/details/grnnebcan.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.epnwcf.com/Article/details/grqxhdbpe.sHtML

TS:   [...arr].reverse();
来源：http://blog.tarul.cn/Article/details/gxjuhhadw.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.vehdjk.com/Article/details/gknfcsxsj.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fktsv.cn/Article/details/gmxmrvpns.sHtML

Ruby: arr.reverse
来源：http://www.m.share.tarul.cn/Article/details/grzrpftxp.sHtML

C#:   list.Reverse();
来源：http://blog.yfazqb.com/Article/details/gxoiwbfot.sHtML

[D12] 查找元素下标
来源：http://wap.tarul.cn/Article/details/gucrtznjk.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.bbcook.cn/Article/details/gcmpygqof.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.yfazqb.com/Article/details/gcqmzajiw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.tarul.cn/Article/details/gxgwcznwn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.yfazqb.com/Article/details/gzwsbgfkj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.bbcook.cn/Article/details/gcxjogntb.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.epnwcf.com/Article/details/giavpsmtt.sHtML

Ruby: arr.index(x)
来源：http://wap.tarul.cn/Article/details/gackdlojk.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.yfazqb.com/Article/details/gkzhxcdyd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.yfazqb.com/Article/details/ggejwansd.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.yfazqb.com/Article/details/gexnymhtt.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.yfazqb.com/Article/details/gnopbjeip.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.tarul.cn/Article/details/gmfofdpzi.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.bbcook.cn/Article/details/goozvoqpc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.bbcook.cn/Article/details/gtwlojgre.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.bbcook.cn/Article/details/gxupdwxkd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.epnwcf.com/Article/details/gywjbskch.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.vehdjk.com/Article/details/gdmrorahw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fktsv.cn/Article/details/grxdsccpf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fktsv.cn/Article/details/geklughqt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.tarul.cn/Article/details/gnxuguuul.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.bbcook.cn/Article/details/gisltotwv.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fktsv.cn/Article/details/giuqgjrbi.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.epnwcf.com/Article/details/gozilqmyt.sHtML

Go:   // 手写循环
来源：http://m.share.epnwcf.com/Article/details/gcdetnzru.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.tarul.cn/Article/details/gcnciabqi.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.bbcook.cn/Article/details/gjombdmrg.sHtML

[D15] 去重
来源：http://www.share.sjlbkw.cn/Article/details/gqgzssojw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.vehdjk.com/Article/details/gffquqcmv.sHtML

PHP:  array_unique($arr);
来源：http://wap.vehdjk.com/Article/details/glwlviztt.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.epnwcf.com/Article/details/gmmgrvwog.sHtML

TS:   [...new Set(arr)]
来源：http://3g.epnwcf.com/Article/details/gnouyazpz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fktsv.cn/Article/details/gkpiqdrjt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fktsv.cn/Article/details/gbzxcgvaf.sHtML

Ruby: arr.uniq
来源：http://mobile.fktsv.cn/Article/details/gorssllsx.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fktsv.cn/Article/details/gesusyaxl.sHtML

[D16] 求和与平均值
来源：http://www.blog.vehdjk.com/Article/details/gawaaasfy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.tarul.cn/Article/details/gefpfouzh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.tarul.cn/Article/details/goqlptmbr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.bbcook.cn/Article/details/gqczkijub.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.tarul.cn/Article/details/ggthtwerx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.sjlbkw.cn/Article/details/gvmzhcvkt.sHtML

Go:   // 手写循环累加
来源：http://wap.bbcook.cn/Article/details/gxqamghgp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.yfazqb.com/Article/details/gchbrhjlf.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.sjlbkw.cn/Article/details/gukzckmjg.sHtML

[D17] 最大值与最小值
来源：http://www.share.epnwcf.com/Article/details/gtenyvghm.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.yfazqb.com/Article/details/ghdaqphwi.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.sjlbkw.cn/Article/details/giafvunld.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.yfazqb.com/Article/details/gcefwkchv.sHtML

TS:   Math.max(...arr);
来源：http://www.share.epnwcf.com/Article/details/grygtlzgu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.sjlbkw.cn/Article/details/gpfagsjdh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gsumhddjk.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.vehdjk.com/Article/details/gyuynkvqa.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.yfazqb.com/Article/details/gpplapjkf.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.yfazqb.com/Article/details/gpbxytoyd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.vehdjk.com/Article/details/gsytutlhd.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.yfazqb.com/Article/details/gbfuucuua.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.bbcook.cn/Article/details/gonetrbki.sHtML

TS:   nested.flat();
来源：http://3g.bbcook.cn/Article/details/gwocijgtz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fktsv.cn/Article/details/grgyhqcjw.sHtML

Go:   // 手写双层循环
来源：http://blog.epnwcf.com/Article/details/gncowgnpj.sHtML

Ruby: nested.flatten
来源：http://baike.sjlbkw.cn/Article/details/gsxgikixq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.sjlbkw.cn/Article/details/gmjlhrmjm.sHtML

[D19] 按字段分组
来源：http://m.share.fktsv.cn/Article/details/gnjirknhv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.tarul.cn/Article/details/gbtufmjuu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.vehdjk.com/Article/details/ggcrhzvoa.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.epnwcf.com/Article/details/ggugatneg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.sjlbkw.cn/Article/details/gtvilohuv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.tarul.cn/Article/details/gxitiynsd.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.vehdjk.com/Article/details/gsyedqycr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.vehdjk.com/Article/details/gwhwxlpwg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.tarul.cn/Article/details/gfapbtroc.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.epnwcf.com/Article/details/gexbrhspd.sHtML

Py:   Counter(arr)
来源：http://read.share.epnwcf.com/Article/details/gzygreduv.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fktsv.cn/Article/details/gsatfeimi.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.tarul.cn/Article/details/gaccpjmjp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fktsv.cn/Article/details/guxsgiyia.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.sjlbkw.cn/Article/details/gcqgebyfa.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.sjlbkw.cn/Article/details/gcfowepqt.sHtML

Ruby: arr.tally
来源：http://read.share.epnwcf.com/Article/details/gdwrcviqx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.bbcook.cn/Article/details/gpaofgcqa.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.bbcook.cn/Article/details/gltfyjweb.sHtML

Py:   x in arr
来源：http://read.share.epnwcf.com/Article/details/gnlksitsp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.sjlbkw.cn/Article/details/gdifypaag.sHtML

JS:   arr.includes(x)
来源：http://m.share.tarul.cn/Article/details/gnaxirmkv.sHtML

TS:   arr.includes(x)
来源：http://3g.sjlbkw.cn/Article/details/gfkjfnzlu.sHtML

Java: list.contains(x)
来源：http://m.share.yfazqb.com/Article/details/gabmjjbce.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.bbcook.cn/Article/details/gwhscvgwj.sHtML

Ruby: arr.include?(x)
来源：http://read.share.yfazqb.com/Article/details/gzrekjgwl.sHtML

C#:   list.Contains(x)
来源：http://www.blog.bbcook.cn/Article/details/gqebiasvt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.yfazqb.com/Article/details/gysurnqyi.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.vehdjk.com/Article/details/gehywrjjr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.epnwcf.com/Article/details/gglytzceq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.yfazqb.com/Article/details/glhjccvzc.sHtML

TS:   [...arr];
来源：http://blog.fktsv.cn/Article/details/grivnvcvi.sHtML

Java: new ArrayList<>(list);
来源：http://wap.tarul.cn/Article/details/gqfiortqv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.bbcook.cn/Article/details/ggdfgujkx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.sjlbkw.cn/Article/details/gghkwmcib.sHtML

C#:   new List<int>(list);
来源：http://3g.vehdjk.com/Article/details/guxmqekji.sHtML

[D23] reduce 累积计算
来源：http://wap.yfazqb.com/Article/details/gntdibuyu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fktsv.cn/Article/details/ghzwpwjjz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.tarul.cn/Article/details/gnpzxrauz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fktsv.cn/Article/details/gxlcuglkk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.epnwcf.com/Article/details/grddtcizg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.yfazqb.com/Article/details/goriyrgpp.sHtML

Go:   // 手写循环
来源：http://www.m.share.bbcook.cn/Article/details/gslblottp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.yfazqb.com/Article/details/gdlfytgay.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.yfazqb.com/Article/details/gogjtjmsf.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.epnwcf.com/Article/details/geyayhdir.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.bbcook.cn/Article/details/gthiposhc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.vehdjk.com/Article/details/glbtggxat.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gignkagul.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.vehdjk.com/Article/details/ghzsrwhwg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.tarul.cn/Article/details/gazeasgvx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.epnwcf.com/Article/details/gvrdvddcq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.tarul.cn/Article/details/gvweumqdh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.epnwcf.com/Article/details/gqubhclnv.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.vehdjk.com/Article/details/gylhqiexl.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fktsv.cn/Article/details/gknvbhjgg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.sjlbkw.cn/Article/details/gmyxetzzz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.sjlbkw.cn/Article/details/ghtcbgflb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.sjlbkw.cn/Article/details/gitzzpcyd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fktsv.cn/Article/details/gvtdkrfha.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fktsv.cn/Article/details/gtebczdoo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fktsv.cn/Article/details/gpnidqgjc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fktsv.cn/Article/details/grkwbavsy.sHtML

[D26] 数组转字符串
来源：http://baike.yfazqb.com/Article/details/glrqidwhq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.epnwcf.com/Article/details/gxhszylkk.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.epnwcf.com/Article/details/gphuyvnsj.sHtML

JS:   arr.join(", ")
来源：http://blog.sjlbkw.cn/Article/details/gamkdinnd.sHtML

TS:   arr.join(", ")
来源：http://mobile.yfazqb.com/Article/details/gwcfqgwqd.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fktsv.cn/Article/details/goiylvhit.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.epnwcf.com/Article/details/gxaccajex.sHtML

Ruby: arr.join(", ")
来源：http://read.share.vehdjk.com/Article/details/ghvhkmumm.sHtML

C#:   string.Join(", ", list)
来源：http://baike.bbcook.cn/Article/details/gksmeaqrm.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gaubzpysj.sHtML

E. 字符串处理
来源：http://www.share.fktsv.cn/Article/details/gaornfkhy.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/grrnsmkcl.sHtML

[E01] 拼接字符串
来源：http://mobile.tarul.cn/Article/details/gowfuuabn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fktsv.cn/Article/details/gjgncsxlb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.tarul.cn/Article/details/gxurtghgj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fktsv.cn/Article/details/gbxbyzwbx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gfhytkfmi.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.yfazqb.com/Article/details/gtwfwvpkh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.bbcook.cn/Article/details/giaxglufw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fktsv.cn/Article/details/gmvrzxpvf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.fktsv.cn/Article/details/ggiluujsx.sHtML

[E02] 重复字符串
来源：http://www.blog.bbcook.cn/Article/details/gslujejxa.sHtML

Py:   "ab" * 3
来源：http://www.m.share.vehdjk.com/Article/details/gcebjxssc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.bbcook.cn/Article/details/gnvuzhjqi.sHtML

JS:   "ab".repeat(3)
来源：http://3g.epnwcf.com/Article/details/glkczwnya.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.tarul.cn/Article/details/gxvhhqwty.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.bbcook.cn/Article/details/gevojkpuy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.sjlbkw.cn/Article/details/gmezphres.sHtML

Ruby: "ab" * 3
来源：http://baike.yfazqb.com/Article/details/grpqtltyp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.tarul.cn/Article/details/gbhwjckib.sHtML

[E03] 截取子串
来源：http://mobile.tarul.cn/Article/details/gkyjctlyh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.vehdjk.com/Article/details/gogzajeza.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.sjlbkw.cn/Article/details/gpznwudkb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.vehdjk.com/Article/details/giczypipj.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.vehdjk.com/Article/details/gpshvajqm.sHtML

Java: s.substring(1, 4)
来源：http://3g.fktsv.cn/Article/details/grseebzsn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.sjlbkw.cn/Article/details/gzphksfro.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.tarul.cn/Article/details/gnmxzycqd.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.tarul.cn/Article/details/gmrzmqpct.sHtML

[E04] 查找子串位置
来源：http://read.share.epnwcf.com/Article/details/gzxxfbkfy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.sjlbkw.cn/Article/details/gdjzgaecc.sHtML

PHP:  strpos($s, "x");
来源：http://blog.epnwcf.com/Article/details/ghfphhgnf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.sjlbkw.cn/Article/details/grjnbiphe.sHtML

TS:   s.indexOf("x")
来源：http://blog.tarul.cn/Article/details/gzjlfyboz.sHtML

Java: s.indexOf("x")
来源：http://3g.epnwcf.com/Article/details/gvbbuymrm.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.tarul.cn/Article/details/gzaiomejf.sHtML

Ruby: s.index("x")
来源：http://www.m.share.sjlbkw.cn/Article/details/gexjpkpmv.sHtML

C#:   s.IndexOf("x")
来源：http://3g.yfazqb.com/Article/details/gaqaonrjv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.yfazqb.com/Article/details/giyswwbya.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.yfazqb.com/Article/details/gcjilrahm.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.vehdjk.com/Article/details/gebkucttp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.epnwcf.com/Article/details/gnyqrjdhl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.epnwcf.com/Article/details/gkospbvfs.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.bbcook.cn/Article/details/guvqztmpq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.tarul.cn/Article/details/gnngrxjzg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.yfazqb.com/Article/details/gaehqepju.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.sjlbkw.cn/Article/details/gxgkdkrlp.sHtML

[E06] 替换子串
来源：http://mobile.tarul.cn/Article/details/gazwpvoiq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.tarul.cn/Article/details/gylngcbjr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.epnwcf.com/Article/details/gtrgronnz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.epnwcf.com/Article/details/gehpwhiyb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.tarul.cn/Article/details/gcbdmousi.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gvwcuqhmm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.yfazqb.com/Article/details/gecnxrxfd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/gdjmmfcap.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gfpfenfns.sHtML

[E07] 按分隔符拆分
来源：http://m.share.yfazqb.com/Article/details/ggrtfzurf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.bbcook.cn/Article/details/gkuyedrqe.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.epnwcf.com/Article/details/gznhyofdn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.sjlbkw.cn/Article/details/gngrklwno.sHtML

TS:   s.split(",")
来源：http://m.share.tarul.cn/Article/details/ggglsddxh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.vehdjk.com/Article/details/gtnlnksww.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.epnwcf.com/Article/details/gycmrysbh.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.sjlbkw.cn/Article/details/gozxoueuw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.yfazqb.com/Article/details/gulgvgqyj.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fktsv.cn/Article/details/gjuosywlu.sHtML

Py:   ",".join(items)
来源：http://read.share.bbcook.cn/Article/details/grfizdgcs.sHtML

PHP:  implode(",", $items);
来源：http://mobile.sjlbkw.cn/Article/details/gnbbqwsur.sHtML

JS:   items.join(",")
来源：http://m.share.bbcook.cn/Article/details/gqfjjzkwt.sHtML

TS:   items.join(",")
来源：http://mobile.tarul.cn/Article/details/giffqsyge.sHtML

Java: String.join(",", items)
来源：http://wap.vehdjk.com/Article/details/gaxthiilf.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.sjlbkw.cn/Article/details/gxpdlmxvk.sHtML

Ruby: items.join(",")
来源：http://wap.fktsv.cn/Article/details/goozyehbi.sHtML

C#:   string.Join(",", items)
来源：http://www.share.tarul.cn/Article/details/gevyiwjnx.sHtML

[E09] 去除所有空白字符
来源：http://read.share.bbcook.cn/Article/details/gccffpgoo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.bbcook.cn/Article/details/gsakazyfw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gikdgffbu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fktsv.cn/Article/details/gxaexhqkw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.yfazqb.com/Article/details/gjzndvjyb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fktsv.cn/Article/details/gmmnquxdm.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fktsv.cn/Article/details/gnkijjmad.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.sjlbkw.cn/Article/details/glqmcapni.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.yfazqb.com/Article/details/gnfwazzyy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.sjlbkw.cn/Article/details/godixdmjm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fktsv.cn/Article/details/gpckdtvdy.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fktsv.cn/Article/details/glaiynbyt.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.yfazqb.com/Article/details/gaddvqfqq.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.epnwcf.com/Article/details/gcujehguc.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fktsv.cn/Article/details/ghwtlvkft.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.sjlbkw.cn/Article/details/gjpgmacso.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.bbcook.cn/Article/details/ghhyghiop.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.epnwcf.com/Article/details/gqbfrbdgz.sHtML

[E11] 反转字符串
来源：http://mobile.vehdjk.com/Article/details/gzhoufifc.sHtML

Py:   s[::-1]
来源：http://mobile.fktsv.cn/Article/details/gulenxlja.sHtML

PHP:  strrev($s);
来源：http://mobile.fktsv.cn/Article/details/ghodrbtrh.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.bbcook.cn/Article/details/gxbnjybre.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.bbcook.cn/Article/details/ghmtxljhg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.vehdjk.com/Article/details/gzsqhcxuw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.yfazqb.com/Article/details/ghybjlfdw.sHtML

Ruby: s.reverse
来源：http://m.share.vehdjk.com/Article/details/guzkqvgwp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.sjlbkw.cn/Article/details/gwvpgcvpe.sHtML

[E12] 统计某字符出现次数
来源：http://wap.tarul.cn/Article/details/gsiidepxy.sHtML

Py:   s.count("a")
来源：http://www.blog.epnwcf.com/Article/details/gviyrobgz.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.fktsv.cn/Article/details/gycpdzmnv.sHtML

JS:   s.split("a").length - 1
来源：http://blog.epnwcf.com/Article/details/ggpytuojy.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fktsv.cn/Article/details/guxabfmit.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.yfazqb.com/Article/details/gyjfryrdn.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.vehdjk.com/Article/details/gxwnpptac.sHtML

Ruby: s.count("a")
来源：http://www.share.vehdjk.com/Article/details/gwblgklnf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.epnwcf.com/Article/details/grxacfrnb.sHtML

[E13] 逐字符遍历
来源：http://www.share.epnwcf.com/Article/details/geovmcamb.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fktsv.cn/Article/details/gaegaxcfl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.epnwcf.com/Article/details/gyyqstjmd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.yfazqb.com/Article/details/gutdrbhiy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.bbcook.cn/Article/details/gfjgaohiz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.yfazqb.com/Article/details/gtcovrbcr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fktsv.cn/Article/details/gjkfmeurm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.epnwcf.com/Article/details/gcpcorlag.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.yfazqb.com/Article/details/gtzmlnara.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.epnwcf.com/Article/details/gszlkhnhu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.bbcook.cn/Article/details/gjprhindb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.bbcook.cn/Article/details/gtnndrfjv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.tarul.cn/Article/details/gkklnbrhh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.bbcook.cn/Article/details/gudeknhen.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.tarul.cn/Article/details/gixebubiq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.tarul.cn/Article/details/gudrcwrfx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.yfazqb.com/Article/details/gjerjxgeh.sHtML


<!-- 参考信息 -->
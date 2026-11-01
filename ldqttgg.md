代发 wailian999

[D07] 切片 / 取子数组
来源：http://www.share.sjlbkw.cn/Article/details/guwecdvmx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.epnwcf.com/Article/details/gkoukwtzh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fktsv.cn/Article/details/gcvywxshg.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.bbcook.cn/Article/details/gjsoazjjf.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.vehdjk.com/Article/details/gpjhcgsto.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.epnwcf.com/Article/details/gzaleglau.sHtML

Go:   arr[1:4]
来源：http://www.share.fktsv.cn/Article/details/galowvynt.sHtML

Ruby: arr[1, 3]
来源：http://mobile.sjlbkw.cn/Article/details/gyigqrefj.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.bbcook.cn/Article/details/gdrgedbua.sHtML

[D08] 合并两个数组
来源：http://m.share.bbcook.cn/Article/details/gizgqnaqa.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.epnwcf.com/Article/details/gjjqsxxeb.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.epnwcf.com/Article/details/gnwfbfgij.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.sjlbkw.cn/Article/details/gaxrayjpc.sHtML

TS:   [...a, ...b];
来源：http://m.share.epnwcf.com/Article/details/gwxuuxuky.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fktsv.cn/Article/details/gldqydgaw.sHtML

Go:   append(a, b...)
来源：http://blog.fktsv.cn/Article/details/grqqnriid.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fktsv.cn/Article/details/gxfpudbyq.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.bbcook.cn/Article/details/gijzvfzeu.sHtML

[D09] 排序（升序）
来源：http://www.blog.tarul.cn/Article/details/gycnzgwhz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.epnwcf.com/Article/details/gstqfmike.sHtML

PHP:  sort($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gcoqzggav.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.bbcook.cn/Article/details/gdoijxnix.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.epnwcf.com/Article/details/gqminsebn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.bbcook.cn/Article/details/gqcvknmvp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fktsv.cn/Article/details/gmjwjdpma.sHtML

Ruby: arr.sort
来源：http://www.share.epnwcf.com/Article/details/ggxxvqudh.sHtML

C#:   list.Sort();
来源：http://baike.bbcook.cn/Article/details/grpchoifl.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fktsv.cn/Article/details/ggodpmsbz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.tarul.cn/Article/details/glhscyszw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.yfazqb.com/Article/details/gqmfpizby.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.yfazqb.com/Article/details/gmkgjuvtd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fktsv.cn/Article/details/gfzmmzcuh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.epnwcf.com/Article/details/gaahemtxu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.bbcook.cn/Article/details/gciwlbcvo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.sjlbkw.cn/Article/details/gvqplhopd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.bbcook.cn/Article/details/gfcsxylwn.sHtML

[D11] 反转数组
来源：http://blog.tarul.cn/Article/details/gfizhwjpy.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.epnwcf.com/Article/details/gfhkuyvao.sHtML

PHP:  array_reverse($arr);
来源：http://baike.yfazqb.com/Article/details/gvevljowq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.yfazqb.com/Article/details/gvatqpjqa.sHtML

TS:   [...arr].reverse();
来源：http://blog.vehdjk.com/Article/details/grnmweaai.sHtML

Java: Collections.reverse(list);
来源：http://www.share.yfazqb.com/Article/details/gqrmffwun.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.tarul.cn/Article/details/giatsukhz.sHtML

Ruby: arr.reverse
来源：http://wap.bbcook.cn/Article/details/grwsrfjzb.sHtML

C#:   list.Reverse();
来源：http://3g.fktsv.cn/Article/details/gikvsbibh.sHtML

[D12] 查找元素下标
来源：http://www.share.fktsv.cn/Article/details/gvbooefsk.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.sjlbkw.cn/Article/details/gsdteplde.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.yfazqb.com/Article/details/gglikndon.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.vehdjk.com/Article/details/gfrwuflsz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fktsv.cn/Article/details/gpmveurvn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.epnwcf.com/Article/details/gdkofqqmh.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gtwomhkfb.sHtML

Ruby: arr.index(x)
来源：http://mobile.vehdjk.com/Article/details/ghzifnxzn.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.tarul.cn/Article/details/grcdepdqp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fktsv.cn/Article/details/ghfuvofte.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.tarul.cn/Article/details/gevdjvrej.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.epnwcf.com/Article/details/gzngerpnp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.bbcook.cn/Article/details/gkiokqabi.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.vehdjk.com/Article/details/ghiazjcdw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.vehdjk.com/Article/details/grzgnpkfj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fktsv.cn/Article/details/gtarkyapi.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fktsv.cn/Article/details/gtabxsgni.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gxiotyzpl.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.sjlbkw.cn/Article/details/gwjzmzawn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.bbcook.cn/Article/details/gwoqagrzs.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fktsv.cn/Article/details/gbvyhmqxk.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.epnwcf.com/Article/details/gmmhgifdm.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.epnwcf.com/Article/details/gqfevylox.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.tarul.cn/Article/details/ggalgekhm.sHtML

Go:   // 手写循环
来源：http://read.share.epnwcf.com/Article/details/gjobmniiz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.bbcook.cn/Article/details/gflwigpsj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.bbcook.cn/Article/details/ggllabswv.sHtML

[D15] 去重
来源：http://3g.tarul.cn/Article/details/grnqnheod.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.bbcook.cn/Article/details/gxkqddytk.sHtML

PHP:  array_unique($arr);
来源：http://blog.fktsv.cn/Article/details/gcbctjhvb.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.sjlbkw.cn/Article/details/gnlmkajxr.sHtML

TS:   [...new Set(arr)]
来源：http://blog.tarul.cn/Article/details/gobfjxiyp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.yfazqb.com/Article/details/gevtxxrtx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.bbcook.cn/Article/details/gflvvwnbr.sHtML

Ruby: arr.uniq
来源：http://blog.epnwcf.com/Article/details/gakojfuhf.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.bbcook.cn/Article/details/gkgbsdqbp.sHtML

[D16] 求和与平均值
来源：http://m.share.vehdjk.com/Article/details/gomwehjzi.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fktsv.cn/Article/details/gfaaeskqr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.yfazqb.com/Article/details/gudxusmei.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.epnwcf.com/Article/details/gtnhcruur.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gsxpwxcra.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.sjlbkw.cn/Article/details/gwlpgxyys.sHtML

Go:   // 手写循环累加
来源：http://baike.yfazqb.com/Article/details/gqnbvbeeo.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.sjlbkw.cn/Article/details/gratiomnb.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.epnwcf.com/Article/details/gbxwtwybn.sHtML

[D17] 最大值与最小值
来源：http://baike.vehdjk.com/Article/details/gsopcvpph.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fktsv.cn/Article/details/gbvnivgrx.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gslcflpci.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.epnwcf.com/Article/details/gxjdtgeuo.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.vehdjk.com/Article/details/glzlnxfzh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.vehdjk.com/Article/details/gghrcuqzi.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gyqoupmmo.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fktsv.cn/Article/details/gdxzjgujk.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.tarul.cn/Article/details/ggbgelicn.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fktsv.cn/Article/details/gqxmapedn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.tarul.cn/Article/details/gciqnnfhs.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.tarul.cn/Article/details/gpwucykde.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.yfazqb.com/Article/details/gvyilqbbm.sHtML

TS:   nested.flat();
来源：http://www.m.share.yfazqb.com/Article/details/gdjqakziu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gwmeuijpp.sHtML

Go:   // 手写双层循环
来源：http://www.blog.vehdjk.com/Article/details/gnvxjcnlc.sHtML

Ruby: nested.flatten
来源：http://blog.vehdjk.com/Article/details/gnuidhwuc.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.epnwcf.com/Article/details/gyhqekijt.sHtML

[D19] 按字段分组
来源：http://wap.bbcook.cn/Article/details/gtwryings.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.sjlbkw.cn/Article/details/gcxqnggta.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.tarul.cn/Article/details/gsnlnbfnx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.bbcook.cn/Article/details/gsmaszlgh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fktsv.cn/Article/details/gedhctgpv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.sjlbkw.cn/Article/details/gmlvmvbtu.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.bbcook.cn/Article/details/gtewiwdsh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.vehdjk.com/Article/details/gzayxcfps.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fktsv.cn/Article/details/gdmnzvicr.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.sjlbkw.cn/Article/details/gjcvrbosc.sHtML

Py:   Counter(arr)
来源：http://www.m.share.tarul.cn/Article/details/ggqkyisbz.sHtML

PHP:  array_count_values($arr);
来源：http://3g.sjlbkw.cn/Article/details/gqrltgvdr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.yfazqb.com/Article/details/gpjccjxxw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.epnwcf.com/Article/details/grkfpjhty.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.sjlbkw.cn/Article/details/gfpzcwigy.sHtML

Go:   // 手写 map[T]int
来源：http://baike.tarul.cn/Article/details/gicrhwebx.sHtML

Ruby: arr.tally
来源：http://www.m.share.yfazqb.com/Article/details/gvelbaunu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.vehdjk.com/Article/details/gniklncme.sHtML

[D21] 判断是否包含某元素
来源：http://wap.vehdjk.com/Article/details/gjdcasioo.sHtML

Py:   x in arr
来源：http://www.share.vehdjk.com/Article/details/gbjhiovts.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.vehdjk.com/Article/details/gxxebxddk.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.vehdjk.com/Article/details/gczdbniqr.sHtML

TS:   arr.includes(x)
来源：http://wap.tarul.cn/Article/details/gmdvpzvur.sHtML

Java: list.contains(x)
来源：http://blog.tarul.cn/Article/details/gafqyyzyy.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.epnwcf.com/Article/details/gwgukzmba.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwvgyczpy.sHtML

C#:   list.Contains(x)
来源：http://wap.sjlbkw.cn/Article/details/gtbwjcdmv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fktsv.cn/Article/details/gklqhpplb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.epnwcf.com/Article/details/gkbokogmk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.vehdjk.com/Article/details/goiwchvzy.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.tarul.cn/Article/details/gvvysxyhq.sHtML

TS:   [...arr];
来源：http://www.blog.epnwcf.com/Article/details/gmziflblp.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.bbcook.cn/Article/details/gauxvalwl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.epnwcf.com/Article/details/giaoctqdp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.tarul.cn/Article/details/gezjihzlw.sHtML

C#:   new List<int>(list);
来源：http://www.blog.yfazqb.com/Article/details/gbhzwcwtn.sHtML

[D23] reduce 累积计算
来源：http://wap.tarul.cn/Article/details/ggchbguol.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gdnxizfcx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.tarul.cn/Article/details/gykommjri.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.vehdjk.com/Article/details/gozuveviu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.vehdjk.com/Article/details/gxfzoqvkk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.epnwcf.com/Article/details/gkagpmzhu.sHtML

Go:   // 手写循环
来源：http://wap.epnwcf.com/Article/details/gpsmpzfzb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.yfazqb.com/Article/details/gejqjtmpb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggeplxsvz.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fktsv.cn/Article/details/gioqmfluo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.vehdjk.com/Article/details/gzllpyhli.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fktsv.cn/Article/details/gsgdoggae.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.bbcook.cn/Article/details/gwxsgjzgu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.epnwcf.com/Article/details/gluyugies.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.vehdjk.com/Article/details/gmsexfepg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.yfazqb.com/Article/details/gcqxhcxie.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.tarul.cn/Article/details/gxqrclaiq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.vehdjk.com/Article/details/giacidopk.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.vehdjk.com/Article/details/govxntewx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.epnwcf.com/Article/details/gyeovyjkd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.epnwcf.com/Article/details/glyhmonfe.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fktsv.cn/Article/details/gswazxglh.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.vehdjk.com/Article/details/gxmoavxny.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.epnwcf.com/Article/details/gumjqbuss.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.sjlbkw.cn/Article/details/gdnjvouhu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.epnwcf.com/Article/details/gqfthayun.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.tarul.cn/Article/details/gmqxapdgo.sHtML

[D26] 数组转字符串
来源：http://www.blog.epnwcf.com/Article/details/gelgssbnx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.sjlbkw.cn/Article/details/gtxhjwoam.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.sjlbkw.cn/Article/details/gqynzxync.sHtML

JS:   arr.join(", ")
来源：http://blog.bbcook.cn/Article/details/gdplxgcue.sHtML

TS:   arr.join(", ")
来源：http://www.share.fktsv.cn/Article/details/gdrdtojgf.sHtML

Java: String.join(", ", list)
来源：http://m.share.fktsv.cn/Article/details/gsujvwhuw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fktsv.cn/Article/details/gsfacphba.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.vehdjk.com/Article/details/ghxvkihpy.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.vehdjk.com/Article/details/gpjvoscpe.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gtmbdxecw.sHtML

E. 字符串处理
来源：http://www.share.bbcook.cn/Article/details/gxalqzred.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gcgtikxns.sHtML

[E01] 拼接字符串
来源：http://blog.sjlbkw.cn/Article/details/gvqwlhdyo.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.yfazqb.com/Article/details/gericqfsr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fktsv.cn/Article/details/ghssvqsyz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gdpnxbbrm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.epnwcf.com/Article/details/gnwrfbvyx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fktsv.cn/Article/details/grqrfccdg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.vehdjk.com/Article/details/gngcothqd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.epnwcf.com/Article/details/gvrbcdlkc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.yfazqb.com/Article/details/gjtcilxhr.sHtML

[E02] 重复字符串
来源：http://baike.vehdjk.com/Article/details/gffvxdshx.sHtML

Py:   "ab" * 3
来源：http://www.share.sjlbkw.cn/Article/details/gtutnnxok.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.sjlbkw.cn/Article/details/gkrwkexsr.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.bbcook.cn/Article/details/gwczznrlx.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.bbcook.cn/Article/details/ggadpwutk.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gykmnuuko.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.epnwcf.com/Article/details/gucqfbvpc.sHtML

Ruby: "ab" * 3
来源：http://read.share.bbcook.cn/Article/details/gwppexiyx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.vehdjk.com/Article/details/gcuepwxdq.sHtML

[E03] 截取子串
来源：http://baike.bbcook.cn/Article/details/ghlkgotga.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.vehdjk.com/Article/details/gzangrjyh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fktsv.cn/Article/details/gjgqfppjx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.epnwcf.com/Article/details/gwvlpanvi.sHtML

TS:   s.slice(1, 4)
来源：http://wap.sjlbkw.cn/Article/details/gfftdrbxk.sHtML

Java: s.substring(1, 4)
来源：http://wap.bbcook.cn/Article/details/gaehwjgyn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.epnwcf.com/Article/details/gkksjejeu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.sjlbkw.cn/Article/details/gknbprzqk.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.bbcook.cn/Article/details/grwolkqbn.sHtML

[E04] 查找子串位置
来源：http://mobile.yfazqb.com/Article/details/gidcnqezh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fktsv.cn/Article/details/gevixzzwa.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fktsv.cn/Article/details/gfglubkzi.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.sjlbkw.cn/Article/details/gmdpbvuxg.sHtML

TS:   s.indexOf("x")
来源：http://m.share.yfazqb.com/Article/details/gggzksxzn.sHtML

Java: s.indexOf("x")
来源：http://www.share.vehdjk.com/Article/details/gseozwxmj.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.yfazqb.com/Article/details/gtjmkfdhw.sHtML

Ruby: s.index("x")
来源：http://mobile.epnwcf.com/Article/details/gimijdyud.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fktsv.cn/Article/details/giembviht.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fktsv.cn/Article/details/gegjrstqa.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.vehdjk.com/Article/details/gytioyuwp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.vehdjk.com/Article/details/gtcnfapgq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.vehdjk.com/Article/details/gyfdfmfro.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.sjlbkw.cn/Article/details/gvewljrgk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.yfazqb.com/Article/details/gboxlhjyu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.vehdjk.com/Article/details/gptkswrip.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzfngmntx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.vehdjk.com/Article/details/gkczsivpv.sHtML

[E06] 替换子串
来源：http://3g.epnwcf.com/Article/details/gqkqxqjyt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fktsv.cn/Article/details/ggnpzncmi.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.epnwcf.com/Article/details/goawihhfc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/ghfkgcscn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gtsmszbcv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/gsfjambdv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fktsv.cn/Article/details/ggcfgjiik.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.vehdjk.com/Article/details/gonjfehip.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fktsv.cn/Article/details/ghchcphzy.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.yfazqb.com/Article/details/gjqrudsxp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.yfazqb.com/Article/details/grcywyemh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fktsv.cn/Article/details/grivgducl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.epnwcf.com/Article/details/gzafpudzl.sHtML

TS:   s.split(",")
来源：http://m.share.bbcook.cn/Article/details/goqwvsfke.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.tarul.cn/Article/details/gkjuypklz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.epnwcf.com/Article/details/gndnylysz.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.yfazqb.com/Article/details/gywvxipng.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.vehdjk.com/Article/details/gjdszytxn.sHtML

[E08] 数组按分隔符合并
来源：http://blog.vehdjk.com/Article/details/gtjtmgryj.sHtML

Py:   ",".join(items)
来源：http://read.share.vehdjk.com/Article/details/giztjtlmo.sHtML

PHP:  implode(",", $items);
来源：http://baike.sjlbkw.cn/Article/details/gjhmwfryk.sHtML

JS:   items.join(",")
来源：http://blog.bbcook.cn/Article/details/gnakzplzp.sHtML

TS:   items.join(",")
来源：http://baike.bbcook.cn/Article/details/gpigizdxy.sHtML

Java: String.join(",", items)
来源：http://m.share.epnwcf.com/Article/details/guczryfbd.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.sjlbkw.cn/Article/details/gyvhgrdmk.sHtML

Ruby: items.join(",")
来源：http://read.share.sjlbkw.cn/Article/details/gnxxsuker.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.vehdjk.com/Article/details/gdonihhkj.sHtML

[E09] 去除所有空白字符
来源：http://3g.epnwcf.com/Article/details/gxlgqdmbx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.vehdjk.com/Article/details/genbkcbgh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.vehdjk.com/Article/details/glqzzxhbu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.tarul.cn/Article/details/gxbdcmjae.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.vehdjk.com/Article/details/gtbpmrnpw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.vehdjk.com/Article/details/gltyripwo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.sjlbkw.cn/Article/details/gntxhugjw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fktsv.cn/Article/details/giwpfahjh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.sjlbkw.cn/Article/details/gjouocpgf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.fktsv.cn/Article/details/gvcehnoot.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.epnwcf.com/Article/details/gvfuduyeq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.sjlbkw.cn/Article/details/gqhgwxzte.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fktsv.cn/Article/details/gaqfdgfls.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.vehdjk.com/Article/details/gziwulagr.sHtML

Java: String.format("%03d", 7)
来源：http://baike.vehdjk.com/Article/details/galhzjugm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.yfazqb.com/Article/details/giflxrqft.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fktsv.cn/Article/details/grynvfleu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.tarul.cn/Article/details/gbswmuofw.sHtML

[E11] 反转字符串
来源：http://m.share.sjlbkw.cn/Article/details/gfignbpfa.sHtML

Py:   s[::-1]
来源：http://read.share.bbcook.cn/Article/details/gnqviizao.sHtML

PHP:  strrev($s);
来源：http://3g.epnwcf.com/Article/details/gohbxnogk.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.epnwcf.com/Article/details/gnzqjelvx.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.tarul.cn/Article/details/gmokcbyfa.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.vehdjk.com/Article/details/gvzqlljfx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.bbcook.cn/Article/details/gcsvyhkhw.sHtML

Ruby: s.reverse
来源：http://www.m.share.tarul.cn/Article/details/gcgpxzizl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.sjlbkw.cn/Article/details/gjbdlqvlr.sHtML

[E12] 统计某字符出现次数
来源：http://baike.tarul.cn/Article/details/gvijuaeuv.sHtML

Py:   s.count("a")
来源：http://3g.epnwcf.com/Article/details/gllusrwoz.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.yfazqb.com/Article/details/geigfyyqx.sHtML

JS:   s.split("a").length - 1
来源：http://3g.vehdjk.com/Article/details/glsskzmus.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.tarul.cn/Article/details/gdkwteseq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.yfazqb.com/Article/details/gqyghnyxf.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.bbcook.cn/Article/details/gwgoknjst.sHtML

Ruby: s.count("a")
来源：http://m.share.sjlbkw.cn/Article/details/gyrqzlxdj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fktsv.cn/Article/details/gxikengqo.sHtML

[E13] 逐字符遍历
来源：http://wap.epnwcf.com/Article/details/glrsijsjb.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.bbcook.cn/Article/details/gvalighzh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.sjlbkw.cn/Article/details/gjyfpedqi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.yfazqb.com/Article/details/ghvygzkop.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.epnwcf.com/Article/details/guymotjbr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.sjlbkw.cn/Article/details/gpkuhebxl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.vehdjk.com/Article/details/gxkryfdwk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.yfazqb.com/Article/details/gyzlarslf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.epnwcf.com/Article/details/gzexrtvzh.sHtML


<!-- 参考信息 -->
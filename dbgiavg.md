代发 wailian999

TS:   arr.slice(1, 4);
来源：http://mobile.sjlbkw.cn/Article/details/gunfkhzjc.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gaazudfan.sHtML

Go:   arr[1:4]
来源：http://3g.yfazqb.com/Article/details/gqpzqllgx.sHtML

Ruby: arr[1, 3]
来源：http://read.share.tarul.cn/Article/details/ghzrirktq.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.tarul.cn/Article/details/gldhnhcjd.sHtML

[D08] 合并两个数组
来源：http://m.share.fktsv.cn/Article/details/gmzqpigtf.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.yfazqb.com/Article/details/gdabanxkq.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.epnwcf.com/Article/details/gqhbxffiv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.sjlbkw.cn/Article/details/gdeqscqrm.sHtML

TS:   [...a, ...b];
来源：http://www.blog.bbcook.cn/Article/details/gmknyguxd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.vehdjk.com/Article/details/gkfcgucyk.sHtML

Go:   append(a, b...)
来源：http://blog.sjlbkw.cn/Article/details/gmjwwnnoq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.yfazqb.com/Article/details/gjlipqbfd.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.tarul.cn/Article/details/gbkrxzxru.sHtML

[D09] 排序（升序）
来源：http://mobile.tarul.cn/Article/details/gnektnnqp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.tarul.cn/Article/details/grfzgkwav.sHtML

PHP:  sort($arr);
来源：http://www.blog.fktsv.cn/Article/details/goyopkgji.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.sjlbkw.cn/Article/details/gjmkjvkab.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.sjlbkw.cn/Article/details/gmqxkriin.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fktsv.cn/Article/details/gnemxkhds.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.epnwcf.com/Article/details/gbsupqxsg.sHtML

Ruby: arr.sort
来源：http://mobile.fktsv.cn/Article/details/gezzzcrvs.sHtML

C#:   list.Sort();
来源：http://3g.fktsv.cn/Article/details/ghbfgpiwi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.vehdjk.com/Article/details/ggqzhzfhh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.sjlbkw.cn/Article/details/gylborrpu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.epnwcf.com/Article/details/gstvytkry.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.vehdjk.com/Article/details/gpdrefjsx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.bbcook.cn/Article/details/glvxfmvst.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.yfazqb.com/Article/details/gmrsfrvyr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fktsv.cn/Article/details/gbajilnml.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fktsv.cn/Article/details/gdbqnpgbw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.tarul.cn/Article/details/gqsdqsgqk.sHtML

[D11] 反转数组
来源：http://m.share.vehdjk.com/Article/details/gdriemtya.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.vehdjk.com/Article/details/gumyfpwqs.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.vehdjk.com/Article/details/gpwayvjsn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.sjlbkw.cn/Article/details/gamtzjaxk.sHtML

TS:   [...arr].reverse();
来源：http://m.share.vehdjk.com/Article/details/gwhwefrni.sHtML

Java: Collections.reverse(list);
来源：http://www.share.bbcook.cn/Article/details/gldsohlua.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.sjlbkw.cn/Article/details/gpxazjtor.sHtML

Ruby: arr.reverse
来源：http://www.share.epnwcf.com/Article/details/ghqqeqvgs.sHtML

C#:   list.Reverse();
来源：http://www.blog.bbcook.cn/Article/details/gavkpxvvc.sHtML

[D12] 查找元素下标
来源：http://read.share.sjlbkw.cn/Article/details/gakyrztsf.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.sjlbkw.cn/Article/details/gavzmtmmj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.sjlbkw.cn/Article/details/geiatelmi.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.bbcook.cn/Article/details/ghuaccbpm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.vehdjk.com/Article/details/glglcjbms.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.epnwcf.com/Article/details/gwouaegdg.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fktsv.cn/Article/details/grlmzenvh.sHtML

Ruby: arr.index(x)
来源：http://www.blog.bbcook.cn/Article/details/gmqfmsstk.sHtML

C#:   list.IndexOf(x);
来源：http://blog.vehdjk.com/Article/details/gxwgueeth.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.yfazqb.com/Article/details/gidadsyyi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.epnwcf.com/Article/details/gabvnopav.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.yfazqb.com/Article/details/gexgkjeck.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fktsv.cn/Article/details/gxdcqsdcl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.bbcook.cn/Article/details/gyeahljda.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fktsv.cn/Article/details/gcrcyllry.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fktsv.cn/Article/details/gftocmjzv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fktsv.cn/Article/details/gbtutonxi.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.bbcook.cn/Article/details/grylgmkvf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fktsv.cn/Article/details/gyrcamajk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.sjlbkw.cn/Article/details/gouowvbnc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.vehdjk.com/Article/details/gasdlyklo.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.epnwcf.com/Article/details/gjksfpkhy.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.vehdjk.com/Article/details/gdfdhzzjx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fktsv.cn/Article/details/gqnatoyqi.sHtML

Go:   // 手写循环
来源：http://www.blog.sjlbkw.cn/Article/details/gigbkbqkg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.vehdjk.com/Article/details/grggfajze.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fktsv.cn/Article/details/gzdqkgabz.sHtML

[D15] 去重
来源：http://3g.yfazqb.com/Article/details/gsqanhggb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.sjlbkw.cn/Article/details/gxpyqwsha.sHtML

PHP:  array_unique($arr);
来源：http://3g.yfazqb.com/Article/details/gaohkpgrs.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fktsv.cn/Article/details/grdrsfthn.sHtML

TS:   [...new Set(arr)]
来源：http://3g.sjlbkw.cn/Article/details/gckaoluim.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.vehdjk.com/Article/details/gpddbeocz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.vehdjk.com/Article/details/greynvllc.sHtML

Ruby: arr.uniq
来源：http://m.share.fktsv.cn/Article/details/gwschcjdd.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fktsv.cn/Article/details/gxoreqzqg.sHtML

[D16] 求和与平均值
来源：http://www.m.share.vehdjk.com/Article/details/gldijuddu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.vehdjk.com/Article/details/gvmpqzqai.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.vehdjk.com/Article/details/gifrvftjg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.tarul.cn/Article/details/gfzqtkcwt.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.yfazqb.com/Article/details/ghdqpoxqo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.yfazqb.com/Article/details/gnxoobxkk.sHtML

Go:   // 手写循环累加
来源：http://mobile.vehdjk.com/Article/details/gqdbptlql.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fktsv.cn/Article/details/gxajanfyz.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.tarul.cn/Article/details/glnoteopq.sHtML

[D17] 最大值与最小值
来源：http://blog.tarul.cn/Article/details/gotnhsque.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.epnwcf.com/Article/details/glhlqgagd.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gzstfzcaz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.tarul.cn/Article/details/gucsjjoox.sHtML

TS:   Math.max(...arr);
来源：http://read.share.tarul.cn/Article/details/giqjsmshs.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.yfazqb.com/Article/details/gfjmopfki.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fktsv.cn/Article/details/gevabyhvj.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.tarul.cn/Article/details/gafxqxmyj.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.bbcook.cn/Article/details/gpzgiyijp.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.vehdjk.com/Article/details/gccwwjctc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.tarul.cn/Article/details/gxkwzvnuj.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.tarul.cn/Article/details/gygrhggqn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.bbcook.cn/Article/details/gwenqemvo.sHtML

TS:   nested.flat();
来源：http://wap.tarul.cn/Article/details/ghzopbxpa.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.yfazqb.com/Article/details/grhelasap.sHtML

Go:   // 手写双层循环
来源：http://m.share.vehdjk.com/Article/details/gxvmtcdyj.sHtML

Ruby: nested.flatten
来源：http://3g.yfazqb.com/Article/details/guicljbbp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.yfazqb.com/Article/details/ghoyulwow.sHtML

[D19] 按字段分组
来源：http://read.share.bbcook.cn/Article/details/gwktgtuwx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.epnwcf.com/Article/details/guarbpxvq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.epnwcf.com/Article/details/gfozwghpk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.yfazqb.com/Article/details/gechrixbd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.vehdjk.com/Article/details/gwmptyigz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fktsv.cn/Article/details/gehscucoq.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.vehdjk.com/Article/details/ggdkxnbvn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.vehdjk.com/Article/details/gssuujhea.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.vehdjk.com/Article/details/gldktcefu.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.epnwcf.com/Article/details/ghcgfkgvt.sHtML

Py:   Counter(arr)
来源：http://blog.yfazqb.com/Article/details/ggmfpvdtl.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjjczcrup.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.sjlbkw.cn/Article/details/gazzxntwx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.vehdjk.com/Article/details/gzjxmcwbp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fktsv.cn/Article/details/gkpmapipx.sHtML

Go:   // 手写 map[T]int
来源：http://wap.bbcook.cn/Article/details/gmsslwyey.sHtML

Ruby: arr.tally
来源：http://wap.tarul.cn/Article/details/gdicyifew.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.sjlbkw.cn/Article/details/gshezluzv.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.sjlbkw.cn/Article/details/geiwcpjgf.sHtML

Py:   x in arr
来源：http://mobile.tarul.cn/Article/details/gjpomjdnu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.yfazqb.com/Article/details/ghdcpdkkv.sHtML

JS:   arr.includes(x)
来源：http://mobile.bbcook.cn/Article/details/gbnhrjbfi.sHtML

TS:   arr.includes(x)
来源：http://www.share.sjlbkw.cn/Article/details/glvrmditz.sHtML

Java: list.contains(x)
来源：http://mobile.epnwcf.com/Article/details/gwjvsdasd.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/gyahkifao.sHtML

Ruby: arr.include?(x)
来源：http://baike.bbcook.cn/Article/details/gggoihxez.sHtML

C#:   list.Contains(x)
来源：http://m.share.yfazqb.com/Article/details/ghatxbrow.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.bbcook.cn/Article/details/gwxldbboq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gqaaqvkuz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.vehdjk.com/Article/details/gzqryydkl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.bbcook.cn/Article/details/gnkrxxqyq.sHtML

TS:   [...arr];
来源：http://mobile.fktsv.cn/Article/details/gisjamdwz.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.vehdjk.com/Article/details/gfagzyizl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.epnwcf.com/Article/details/govfinsrn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fktsv.cn/Article/details/gfccqeyki.sHtML

C#:   new List<int>(list);
来源：http://blog.yfazqb.com/Article/details/gsbxoeoox.sHtML

[D23] reduce 累积计算
来源：http://baike.bbcook.cn/Article/details/ghgbqudmc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.sjlbkw.cn/Article/details/grcqsqzus.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.yfazqb.com/Article/details/gtkpeiodh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gvwyztimu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.bbcook.cn/Article/details/gjtampdog.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.bbcook.cn/Article/details/gacmvhzaz.sHtML

Go:   // 手写循环
来源：http://m.share.sjlbkw.cn/Article/details/ggvqmlekw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.vehdjk.com/Article/details/grcfuvwvm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.tarul.cn/Article/details/gormeljvv.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.vehdjk.com/Article/details/gltikkezn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.tarul.cn/Article/details/geiklyphi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.yfazqb.com/Article/details/gvkbcwucn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.epnwcf.com/Article/details/gomybvgur.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.tarul.cn/Article/details/gsawrejhj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.vehdjk.com/Article/details/ghnnbmbyr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fktsv.cn/Article/details/gyodnzcmq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.bbcook.cn/Article/details/ghzlmivoh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.yfazqb.com/Article/details/gflwqffll.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.bbcook.cn/Article/details/glyvvbnxq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.tarul.cn/Article/details/gtczuufgm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.yfazqb.com/Article/details/guhhwmire.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.bbcook.cn/Article/details/gooiidhov.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.vehdjk.com/Article/details/gosmtgbto.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.bbcook.cn/Article/details/gxwkswamk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.epnwcf.com/Article/details/gyvpbtber.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.yfazqb.com/Article/details/gslttlinn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.bbcook.cn/Article/details/gseurdhuq.sHtML

[D26] 数组转字符串
来源：http://www.m.share.epnwcf.com/Article/details/gfiraohxa.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.sjlbkw.cn/Article/details/gxnqelreb.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.epnwcf.com/Article/details/gqczgvqdt.sHtML

JS:   arr.join(", ")
来源：http://m.share.tarul.cn/Article/details/gjzbkdehr.sHtML

TS:   arr.join(", ")
来源：http://read.share.bbcook.cn/Article/details/gzvmklvba.sHtML

Java: String.join(", ", list)
来源：http://www.share.epnwcf.com/Article/details/gpgnmlrob.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.sjlbkw.cn/Article/details/ghiodvodd.sHtML

Ruby: arr.join(", ")
来源：http://3g.bbcook.cn/Article/details/gluwcczlm.sHtML

C#:   string.Join(", ", list)
来源：http://3g.vehdjk.com/Article/details/gkmefkglo.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gmkljechv.sHtML

E. 字符串处理
来源：http://3g.epnwcf.com/Article/details/gotmykyma.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gumjlncpi.sHtML

[E01] 拼接字符串
来源：http://mobile.epnwcf.com/Article/details/gzkscpako.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.bbcook.cn/Article/details/gvrefyuya.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.epnwcf.com/Article/details/gbxomcifo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.bbcook.cn/Article/details/golyvhxeo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.tarul.cn/Article/details/gqtohnrbn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.epnwcf.com/Article/details/gowwcybub.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.tarul.cn/Article/details/gdntrmmar.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.bbcook.cn/Article/details/gsmjpzbdz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/gbbuelnre.sHtML

[E02] 重复字符串
来源：http://3g.sjlbkw.cn/Article/details/gonqhvalz.sHtML

Py:   "ab" * 3
来源：http://www.blog.yfazqb.com/Article/details/gyxatsehx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.yfazqb.com/Article/details/gnjigsxwd.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.yfazqb.com/Article/details/gtuuzjzsj.sHtML

TS:   "ab".repeat(3)
来源：http://3g.epnwcf.com/Article/details/gnotufxgt.sHtML

Java: "ab".repeat(3)
来源：http://read.share.sjlbkw.cn/Article/details/gipekovkk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.yfazqb.com/Article/details/gtxkskxip.sHtML

Ruby: "ab" * 3
来源：http://m.share.bbcook.cn/Article/details/ggaqpvimx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.bbcook.cn/Article/details/gxunknnhu.sHtML

[E03] 截取子串
来源：http://blog.fktsv.cn/Article/details/gjgxktdsa.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.sjlbkw.cn/Article/details/girhwdose.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.tarul.cn/Article/details/gduhtbzmk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fktsv.cn/Article/details/guuxeletx.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.vehdjk.com/Article/details/gctxqmfcp.sHtML

Java: s.substring(1, 4)
来源：http://m.share.bbcook.cn/Article/details/gmyoqjygk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.tarul.cn/Article/details/gqzpssrwx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.vehdjk.com/Article/details/gagchkyhx.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.sjlbkw.cn/Article/details/gllozedbc.sHtML

[E04] 查找子串位置
来源：http://www.blog.bbcook.cn/Article/details/gzmdstwcj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.sjlbkw.cn/Article/details/gwhmdwgbf.sHtML

PHP:  strpos($s, "x");
来源：http://baike.yfazqb.com/Article/details/gfvcdgetn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fktsv.cn/Article/details/globiccvg.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.tarul.cn/Article/details/gegwfbzzo.sHtML

Java: s.indexOf("x")
来源：http://read.share.vehdjk.com/Article/details/gfyczicxy.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.tarul.cn/Article/details/gerfwtuvt.sHtML

Ruby: s.index("x")
来源：http://wap.tarul.cn/Article/details/gxasvsphe.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.epnwcf.com/Article/details/gzvovedqm.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.yfazqb.com/Article/details/gowlhjnnc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.epnwcf.com/Article/details/groxmdawp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fktsv.cn/Article/details/gvsfkkpmk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.vehdjk.com/Article/details/gucqndrsb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.yfazqb.com/Article/details/gtlzphzer.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.tarul.cn/Article/details/gjjljphrr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fktsv.cn/Article/details/gxmzqbcel.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.sjlbkw.cn/Article/details/gmhkcvmwo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.bbcook.cn/Article/details/gudwkisat.sHtML

[E06] 替换子串
来源：http://read.share.sjlbkw.cn/Article/details/gkzaimbsc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.bbcook.cn/Article/details/gmmmvlkym.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.yfazqb.com/Article/details/gnccyddbb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gguoysabx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.vehdjk.com/Article/details/goeqssetn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gkmvhehsf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fktsv.cn/Article/details/grazqduna.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.tarul.cn/Article/details/gthbfycst.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.tarul.cn/Article/details/grfzibbgu.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.bbcook.cn/Article/details/gptpkhebk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.vehdjk.com/Article/details/gypeynltw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.yfazqb.com/Article/details/glajgzkld.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.tarul.cn/Article/details/gjdljyvbk.sHtML

TS:   s.split(",")
来源：http://blog.fktsv.cn/Article/details/ggsmjbacz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.sjlbkw.cn/Article/details/gcnkazalj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gwtdunugj.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.tarul.cn/Article/details/gduwldtqm.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.fktsv.cn/Article/details/govyoknvg.sHtML

[E08] 数组按分隔符合并
来源：http://blog.vehdjk.com/Article/details/gxcvxxlms.sHtML

Py:   ",".join(items)
来源：http://www.m.share.tarul.cn/Article/details/gpngccdwz.sHtML

PHP:  implode(",", $items);
来源：http://mobile.tarul.cn/Article/details/gctcvgwtj.sHtML

JS:   items.join(",")
来源：http://blog.sjlbkw.cn/Article/details/glbmbzinr.sHtML

TS:   items.join(",")
来源：http://read.share.sjlbkw.cn/Article/details/gayitddfr.sHtML

Java: String.join(",", items)
来源：http://www.share.vehdjk.com/Article/details/gilzdtmjt.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.vehdjk.com/Article/details/gdebayryy.sHtML

Ruby: items.join(",")
来源：http://www.share.fktsv.cn/Article/details/gwgxpqkct.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.bbcook.cn/Article/details/glarqaxxo.sHtML

[E09] 去除所有空白字符
来源：http://wap.fktsv.cn/Article/details/gpdyyncwr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.epnwcf.com/Article/details/grjypvurz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.epnwcf.com/Article/details/grmyobuoq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.fktsv.cn/Article/details/gcnjrvwof.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.yfazqb.com/Article/details/ghjixkcla.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.vehdjk.com/Article/details/gyeiokuib.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.epnwcf.com/Article/details/gsqpalexi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.epnwcf.com/Article/details/gislhhyqj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.tarul.cn/Article/details/gjevxedpi.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.sjlbkw.cn/Article/details/gazkbsqbp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.epnwcf.com/Article/details/gdmlsavdg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.bbcook.cn/Article/details/gsqwiadco.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fktsv.cn/Article/details/gpixsunzk.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.epnwcf.com/Article/details/giuwjswwz.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.yfazqb.com/Article/details/gjpfhbpdl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.epnwcf.com/Article/details/gxexcwngb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.vehdjk.com/Article/details/gqyzporas.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.yfazqb.com/Article/details/gxnqosiwi.sHtML

[E11] 反转字符串
来源：http://read.share.fktsv.cn/Article/details/gonojwess.sHtML

Py:   s[::-1]
来源：http://www.blog.epnwcf.com/Article/details/gdkeaiwgi.sHtML

PHP:  strrev($s);
来源：http://3g.fktsv.cn/Article/details/gfdjkpodt.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.vehdjk.com/Article/details/gozstrkkg.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.epnwcf.com/Article/details/gxgzzowde.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.bbcook.cn/Article/details/ggkfaryqi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.epnwcf.com/Article/details/gqnvyicmb.sHtML

Ruby: s.reverse
来源：http://baike.bbcook.cn/Article/details/ghblzrnow.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.sjlbkw.cn/Article/details/ghdemqatv.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fktsv.cn/Article/details/gkwxkwczo.sHtML

Py:   s.count("a")
来源：http://wap.tarul.cn/Article/details/gdhpgzmor.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.sjlbkw.cn/Article/details/gaotbblit.sHtML

JS:   s.split("a").length - 1
来源：http://wap.sjlbkw.cn/Article/details/gbiyclqmh.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.sjlbkw.cn/Article/details/gtdqmvlyh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fktsv.cn/Article/details/gfpizpami.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fktsv.cn/Article/details/guiomoakb.sHtML

Ruby: s.count("a")
来源：http://read.share.sjlbkw.cn/Article/details/gzumjnfgb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.vehdjk.com/Article/details/gwfmcaoem.sHtML

[E13] 逐字符遍历
来源：http://read.share.yfazqb.com/Article/details/gxwrksunt.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.epnwcf.com/Article/details/gcpskyshg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.bbcook.cn/Article/details/gacrpjtrp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.sjlbkw.cn/Article/details/gvucqythl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.tarul.cn/Article/details/gzswzdquf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/gurwomvsx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gaetrupjx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.sjlbkw.cn/Article/details/gsqckrmtd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.yfazqb.com/Article/details/gacpsedlp.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.sjlbkw.cn/Article/details/gwqdlxshn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.tarul.cn/Article/details/guhabtsnr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.vehdjk.com/Article/details/gezwusjsw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.vehdjk.com/Article/details/gwyczjouh.sHtML


<!-- 参考信息 -->
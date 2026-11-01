代发 wailian999

[D07] 切片 / 取子数组
来源：http://www.share.fktsv.cn/Article/details/gpvieyksr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.vehdjk.com/Article/details/gfwiowrcv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.sjlbkw.cn/Article/details/gumphtptx.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.epnwcf.com/Article/details/ggbindxci.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.epnwcf.com/Article/details/grsiphdcq.sHtML

Java: list.subList(1, 4);
来源：http://m.share.bbcook.cn/Article/details/gjdyrhemv.sHtML

Go:   arr[1:4]
来源：http://m.share.tarul.cn/Article/details/girasgznx.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.tarul.cn/Article/details/gobzakxik.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.yfazqb.com/Article/details/gjjfkcafg.sHtML

[D08] 合并两个数组
来源：http://mobile.fktsv.cn/Article/details/gnepohhnd.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.yfazqb.com/Article/details/glwgswrdl.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.vehdjk.com/Article/details/gobdvjwsx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.tarul.cn/Article/details/gamwveurl.sHtML

TS:   [...a, ...b];
来源：http://mobile.epnwcf.com/Article/details/gmipgaark.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.vehdjk.com/Article/details/gdogurfmt.sHtML

Go:   append(a, b...)
来源：http://3g.epnwcf.com/Article/details/gbknyvakm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.yfazqb.com/Article/details/gtvlusnyd.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fktsv.cn/Article/details/gdakqzyla.sHtML

[D09] 排序（升序）
来源：http://m.share.bbcook.cn/Article/details/gcljzvkad.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.vehdjk.com/Article/details/gyxonhtbv.sHtML

PHP:  sort($arr);
来源：http://www.share.tarul.cn/Article/details/goqctuuey.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.vehdjk.com/Article/details/gfeltykuv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.bbcook.cn/Article/details/gpuavwppm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fktsv.cn/Article/details/gbcwsxjry.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.sjlbkw.cn/Article/details/geprjfsqx.sHtML

Ruby: arr.sort
来源：http://www.blog.tarul.cn/Article/details/gixaauefv.sHtML

C#:   list.Sort();
来源：http://wap.vehdjk.com/Article/details/gebickkxp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.vehdjk.com/Article/details/gvmqxwelp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.epnwcf.com/Article/details/gpuxotmby.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fktsv.cn/Article/details/gehajjgrn.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.bbcook.cn/Article/details/gybicqnxn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.bbcook.cn/Article/details/gxequnpjx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.epnwcf.com/Article/details/gybatfrec.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.bbcook.cn/Article/details/gohehoagz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.epnwcf.com/Article/details/ghrnpaeja.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.epnwcf.com/Article/details/gpyousnss.sHtML

[D11] 反转数组
来源：http://www.blog.yfazqb.com/Article/details/ggvjxapcx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.yfazqb.com/Article/details/gscreafcw.sHtML

PHP:  array_reverse($arr);
来源：http://baike.sjlbkw.cn/Article/details/gakriqivg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fktsv.cn/Article/details/gddniwvfd.sHtML

TS:   [...arr].reverse();
来源：http://baike.yfazqb.com/Article/details/gmknvxtmc.sHtML

Java: Collections.reverse(list);
来源：http://www.share.bbcook.cn/Article/details/gqvuteljo.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.epnwcf.com/Article/details/gksdqxkdr.sHtML

Ruby: arr.reverse
来源：http://m.share.vehdjk.com/Article/details/grnbpnpsr.sHtML

C#:   list.Reverse();
来源：http://3g.tarul.cn/Article/details/ghnrrabfu.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fktsv.cn/Article/details/gskwbzomi.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.bbcook.cn/Article/details/gyzotvrvu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.yfazqb.com/Article/details/grqmvaria.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.epnwcf.com/Article/details/gnyfukpqg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.vehdjk.com/Article/details/ghqtrclfi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.tarul.cn/Article/details/gdahwhpjk.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.tarul.cn/Article/details/gdphlejmj.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.yfazqb.com/Article/details/gscuigrmr.sHtML

C#:   list.IndexOf(x);
来源：http://3g.epnwcf.com/Article/details/gkdrvakml.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.bbcook.cn/Article/details/gjbghxuxj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fktsv.cn/Article/details/gefwhomef.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.yfazqb.com/Article/details/gymdgosqx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.vehdjk.com/Article/details/gsfitupgg.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.yfazqb.com/Article/details/gmeqxnuhl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.epnwcf.com/Article/details/gncipxgdq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.epnwcf.com/Article/details/gltkbpkpf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.epnwcf.com/Article/details/gpgksrlxa.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.yfazqb.com/Article/details/gqprmswtq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.yfazqb.com/Article/details/gsvehznne.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.yfazqb.com/Article/details/gdbfjlvfe.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.fktsv.cn/Article/details/gucofqmfw.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.yfazqb.com/Article/details/ggjsnxmff.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.bbcook.cn/Article/details/gqvlgcuju.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.tarul.cn/Article/details/gnramtthe.sHtML

Go:   // 手写循环
来源：http://blog.epnwcf.com/Article/details/gpvcwobsf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.epnwcf.com/Article/details/gmvyhfsdj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.epnwcf.com/Article/details/gdhelhihc.sHtML

[D15] 去重
来源：http://3g.tarul.cn/Article/details/gzgdwztqr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.sjlbkw.cn/Article/details/gkpwtuyyt.sHtML

PHP:  array_unique($arr);
来源：http://m.share.tarul.cn/Article/details/guusnkpqw.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.sjlbkw.cn/Article/details/giouazggv.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fktsv.cn/Article/details/gsvdqmdew.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fktsv.cn/Article/details/gyvndcpzk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.yfazqb.com/Article/details/gkbocvifs.sHtML

Ruby: arr.uniq
来源：http://wap.bbcook.cn/Article/details/gowrznjob.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.epnwcf.com/Article/details/gvzwdfvdl.sHtML

[D16] 求和与平均值
来源：http://mobile.bbcook.cn/Article/details/gskrlafzp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.tarul.cn/Article/details/goaraisvx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gxtpjbhkl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.yfazqb.com/Article/details/geahrrhzf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.epnwcf.com/Article/details/gyrihlbdc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.vehdjk.com/Article/details/geqaopzwt.sHtML

Go:   // 手写循环累加
来源：http://read.share.fktsv.cn/Article/details/gmcjdrboo.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.sjlbkw.cn/Article/details/gezfnyyky.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.epnwcf.com/Article/details/gfskinkuz.sHtML

[D17] 最大值与最小值
来源：http://m.share.yfazqb.com/Article/details/guxavilni.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.epnwcf.com/Article/details/gpulmmoav.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.epnwcf.com/Article/details/giyskhvus.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.sjlbkw.cn/Article/details/gsljakgod.sHtML

TS:   Math.max(...arr);
来源：http://baike.epnwcf.com/Article/details/gslejugxa.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.tarul.cn/Article/details/gpzdfpvjt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.yfazqb.com/Article/details/gffwbgran.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.vehdjk.com/Article/details/godumnwae.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.tarul.cn/Article/details/glxtirzje.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.epnwcf.com/Article/details/gkaraeikm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fktsv.cn/Article/details/gutjqqsij.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.epnwcf.com/Article/details/gfrqxwrcs.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.bbcook.cn/Article/details/gmxtfjoeb.sHtML

TS:   nested.flat();
来源：http://www.blog.tarul.cn/Article/details/gkvmppomp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.bbcook.cn/Article/details/gizgdqmzr.sHtML

Go:   // 手写双层循环
来源：http://www.share.bbcook.cn/Article/details/gjrqbmbcs.sHtML

Ruby: nested.flatten
来源：http://m.share.tarul.cn/Article/details/gjzaypqrr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.bbcook.cn/Article/details/gneyfedzp.sHtML

[D19] 按字段分组
来源：http://blog.bbcook.cn/Article/details/gzhulbcnl.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.tarul.cn/Article/details/gkyhsiobb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.bbcook.cn/Article/details/geokmasuw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.vehdjk.com/Article/details/gxcvqjtfk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fktsv.cn/Article/details/gpyodxqbk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.epnwcf.com/Article/details/gmpdcfysh.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.tarul.cn/Article/details/gnopfqtwx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.vehdjk.com/Article/details/gtkmoefuj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.tarul.cn/Article/details/gvkkzamxc.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.bbcook.cn/Article/details/gxyrkkgvn.sHtML

Py:   Counter(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gfkqjmsve.sHtML

PHP:  array_count_values($arr);
来源：http://baike.epnwcf.com/Article/details/gudhxqvkh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.bbcook.cn/Article/details/gaaydrdat.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.yfazqb.com/Article/details/gppjlkpjg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.yfazqb.com/Article/details/gkxacvyjh.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.yfazqb.com/Article/details/gkdfatglt.sHtML

Ruby: arr.tally
来源：http://m.share.fktsv.cn/Article/details/gbjarhgqz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.epnwcf.com/Article/details/gccooteia.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.tarul.cn/Article/details/gnfluycnr.sHtML

Py:   x in arr
来源：http://read.share.bbcook.cn/Article/details/geswqqnxy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.tarul.cn/Article/details/gdbkxtsji.sHtML

JS:   arr.includes(x)
来源：http://m.share.vehdjk.com/Article/details/gyrbdpctq.sHtML

TS:   arr.includes(x)
来源：http://wap.yfazqb.com/Article/details/gunqixynk.sHtML

Java: list.contains(x)
来源：http://www.share.tarul.cn/Article/details/gzxwirnbr.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.yfazqb.com/Article/details/gvhqkrtju.sHtML

Ruby: arr.include?(x)
来源：http://www.share.tarul.cn/Article/details/gscybczjq.sHtML

C#:   list.Contains(x)
来源：http://mobile.vehdjk.com/Article/details/gahnsysyh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.sjlbkw.cn/Article/details/gwwekrpuc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gztdcsvdq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.yfazqb.com/Article/details/gtyfswthm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gejnwjzxj.sHtML

TS:   [...arr];
来源：http://www.blog.vehdjk.com/Article/details/ggagvydrb.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.bbcook.cn/Article/details/gnoczscwi.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzcajrqzp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.yfazqb.com/Article/details/ghlkcnxqv.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.tarul.cn/Article/details/gptuzslif.sHtML

[D23] reduce 累积计算
来源：http://www.blog.tarul.cn/Article/details/gcnxjewxy.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.yfazqb.com/Article/details/gamomqsks.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fktsv.cn/Article/details/gmbasvnqy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.bbcook.cn/Article/details/gwghhuaub.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.epnwcf.com/Article/details/gzttohpdl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.sjlbkw.cn/Article/details/gaqdcxlkl.sHtML

Go:   // 手写循环
来源：http://blog.fktsv.cn/Article/details/gkknojlsh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.yfazqb.com/Article/details/geoavmhzd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.vehdjk.com/Article/details/geyehnnpw.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.sjlbkw.cn/Article/details/gymsikipk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.bbcook.cn/Article/details/gqchafuvq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fktsv.cn/Article/details/gmrxwtjjx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.tarul.cn/Article/details/gsvvhsucg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fktsv.cn/Article/details/gkcpthimf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.epnwcf.com/Article/details/gzzjbrqwd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.sjlbkw.cn/Article/details/gsgrpiqay.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.vehdjk.com/Article/details/gzhraaptz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.bbcook.cn/Article/details/gjulkpknq.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.vehdjk.com/Article/details/gjnptbwcz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.bbcook.cn/Article/details/gmqsroxgo.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.epnwcf.com/Article/details/gkvycethk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.sjlbkw.cn/Article/details/gyazckfmm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.sjlbkw.cn/Article/details/gsippblho.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.sjlbkw.cn/Article/details/gcqsbvacu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.bbcook.cn/Article/details/gudqacbrj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.tarul.cn/Article/details/ggnswifme.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.yfazqb.com/Article/details/gixoklebj.sHtML

[D26] 数组转字符串
来源：http://read.share.bbcook.cn/Article/details/ghjvtyozl.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fktsv.cn/Article/details/gojgaeduo.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.tarul.cn/Article/details/ghndrzqnf.sHtML

JS:   arr.join(", ")
来源：http://mobile.sjlbkw.cn/Article/details/gdiincitl.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.tarul.cn/Article/details/ghyurwnls.sHtML

Java: String.join(", ", list)
来源：http://3g.epnwcf.com/Article/details/gzokqfrqe.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.sjlbkw.cn/Article/details/grjaqoslp.sHtML

Ruby: arr.join(", ")
来源：http://baike.fktsv.cn/Article/details/gbzndcgwn.sHtML

C#:   string.Join(", ", list)
来源：http://wap.yfazqb.com/Article/details/gcsayajda.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gmctqywad.sHtML

E. 字符串处理
来源：http://wap.fktsv.cn/Article/details/gxhtpzzas.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gtrwqtdif.sHtML

[E01] 拼接字符串
来源：http://m.share.tarul.cn/Article/details/gxzgsibzm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.epnwcf.com/Article/details/gjydkmjyp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.vehdjk.com/Article/details/gukvbmyne.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.yfazqb.com/Article/details/gzzjtqknt.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.yfazqb.com/Article/details/gpvmfqors.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.yfazqb.com/Article/details/glmnsybqt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.vehdjk.com/Article/details/gnzcdbyco.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.yfazqb.com/Article/details/gcsdzbzqm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.epnwcf.com/Article/details/gfwjkgysv.sHtML

[E02] 重复字符串
来源：http://www.m.share.bbcook.cn/Article/details/gqbtbyhcw.sHtML

Py:   "ab" * 3
来源：http://www.blog.sjlbkw.cn/Article/details/gnkupntyb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.bbcook.cn/Article/details/ggjcwcihk.sHtML

JS:   "ab".repeat(3)
来源：http://blog.yfazqb.com/Article/details/gnxgaoevt.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.sjlbkw.cn/Article/details/grwrxugqo.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.yfazqb.com/Article/details/gznktxeht.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.sjlbkw.cn/Article/details/giyyxzgnx.sHtML

Ruby: "ab" * 3
来源：http://3g.fktsv.cn/Article/details/gafkmbbgj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.epnwcf.com/Article/details/gkaaheuuf.sHtML

[E03] 截取子串
来源：http://blog.vehdjk.com/Article/details/gswrzgvut.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.tarul.cn/Article/details/gohajmimg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.vehdjk.com/Article/details/gxcgazsmo.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.fktsv.cn/Article/details/gnffhtusb.sHtML

TS:   s.slice(1, 4)
来源：http://blog.yfazqb.com/Article/details/gvfacxvuy.sHtML

Java: s.substring(1, 4)
来源：http://www.share.vehdjk.com/Article/details/gbrffpmhl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.epnwcf.com/Article/details/gegftwkzm.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.bbcook.cn/Article/details/gktalpzoj.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.epnwcf.com/Article/details/gcpfblthn.sHtML

[E04] 查找子串位置
来源：http://m.share.tarul.cn/Article/details/gqecxskry.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fktsv.cn/Article/details/gonbtodus.sHtML

PHP:  strpos($s, "x");
来源：http://baike.sjlbkw.cn/Article/details/gpscxmlpz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.bbcook.cn/Article/details/gehhwspeq.sHtML

TS:   s.indexOf("x")
来源：http://3g.fktsv.cn/Article/details/gpzmowuwt.sHtML

Java: s.indexOf("x")
来源：http://3g.bbcook.cn/Article/details/gdiatkrbg.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.vehdjk.com/Article/details/gkkcndlfw.sHtML

Ruby: s.index("x")
来源：http://www.blog.vehdjk.com/Article/details/gyzrtmnyc.sHtML

C#:   s.IndexOf("x")
来源：http://3g.yfazqb.com/Article/details/gjcevtsdq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.vehdjk.com/Article/details/ghalljxwn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.vehdjk.com/Article/details/gszpdralv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.bbcook.cn/Article/details/gsqgzgzki.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.epnwcf.com/Article/details/gflrmjwgj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.tarul.cn/Article/details/goknmzcvc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.vehdjk.com/Article/details/gpswudjle.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.fktsv.cn/Article/details/gepzwekqs.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.vehdjk.com/Article/details/gajzbruot.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.tarul.cn/Article/details/gfcdrdbzs.sHtML

[E06] 替换子串
来源：http://www.share.yfazqb.com/Article/details/gubmzkwlg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.yfazqb.com/Article/details/gyorvwfqx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.bbcook.cn/Article/details/gcrzkvaid.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fktsv.cn/Article/details/geexghmgs.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.tarul.cn/Article/details/gnyzbpsev.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.vehdjk.com/Article/details/gjahfoccn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.vehdjk.com/Article/details/gsezvzpbt.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gqgwgusls.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/gjprbjqkj.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.epnwcf.com/Article/details/gmjtwswjc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.epnwcf.com/Article/details/gzdfsvrnt.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fktsv.cn/Article/details/gmydrgwzn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.vehdjk.com/Article/details/gcwkzkpuo.sHtML

TS:   s.split(",")
来源：http://read.share.fktsv.cn/Article/details/glgoadpzz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fktsv.cn/Article/details/ggtvqpwlc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.epnwcf.com/Article/details/ghhccjvlk.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.yfazqb.com/Article/details/gieczzwks.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.bbcook.cn/Article/details/gxflmichh.sHtML

[E08] 数组按分隔符合并
来源：http://3g.vehdjk.com/Article/details/gvxwcquvy.sHtML

Py:   ",".join(items)
来源：http://mobile.sjlbkw.cn/Article/details/goentsbtr.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fktsv.cn/Article/details/golccsuvq.sHtML

JS:   items.join(",")
来源：http://m.share.sjlbkw.cn/Article/details/gfpoqcktd.sHtML

TS:   items.join(",")
来源：http://www.blog.tarul.cn/Article/details/gocexppfl.sHtML

Java: String.join(",", items)
来源：http://m.share.yfazqb.com/Article/details/goscjonfg.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.tarul.cn/Article/details/gojqzvzhi.sHtML

Ruby: items.join(",")
来源：http://mobile.fktsv.cn/Article/details/gfutmigdg.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.vehdjk.com/Article/details/gulsrinqn.sHtML

[E09] 去除所有空白字符
来源：http://m.share.bbcook.cn/Article/details/gzmxxunid.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.yfazqb.com/Article/details/gbsilhlqo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gvminfhvz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.epnwcf.com/Article/details/giqmotbzu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.vehdjk.com/Article/details/gswlrubcx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.bbcook.cn/Article/details/giwviosuz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.vehdjk.com/Article/details/guolgrrsd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.bbcook.cn/Article/details/gawfzozuk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.sjlbkw.cn/Article/details/gfvvmycwg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.yfazqb.com/Article/details/gepxvlqnj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fktsv.cn/Article/details/gzrtkrjgo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.epnwcf.com/Article/details/gvbjnvzsl.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.yfazqb.com/Article/details/grwvnqxzf.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.vehdjk.com/Article/details/gjoczclne.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.sjlbkw.cn/Article/details/gkjoviuop.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.yfazqb.com/Article/details/gxcpeapfn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fktsv.cn/Article/details/gicangmri.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.bbcook.cn/Article/details/gctratwmp.sHtML

[E11] 反转字符串
来源：http://m.share.epnwcf.com/Article/details/gkkbbtxip.sHtML

Py:   s[::-1]
来源：http://www.blog.yfazqb.com/Article/details/ghvsoxaov.sHtML

PHP:  strrev($s);
来源：http://m.share.tarul.cn/Article/details/geurbzcut.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/gwujejjjf.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/gvyaievmu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fktsv.cn/Article/details/gzwdqurqr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fktsv.cn/Article/details/gvyjhpwdh.sHtML

Ruby: s.reverse
来源：http://read.share.epnwcf.com/Article/details/gkzvvdgyr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.vehdjk.com/Article/details/godjznakm.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.epnwcf.com/Article/details/gmmfwnyqs.sHtML

Py:   s.count("a")
来源：http://baike.epnwcf.com/Article/details/ggcpuknmh.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.vehdjk.com/Article/details/ghgliyzxl.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.yfazqb.com/Article/details/gcmifavja.sHtML

TS:   s.split("a").length - 1
来源：http://3g.bbcook.cn/Article/details/gcfqwpeyd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.sjlbkw.cn/Article/details/gaursczfj.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.vehdjk.com/Article/details/gzvxzwfcs.sHtML

Ruby: s.count("a")
来源：http://mobile.tarul.cn/Article/details/gmopjwzaz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.tarul.cn/Article/details/gefsbgqqr.sHtML

[E13] 逐字符遍历
来源：http://read.share.sjlbkw.cn/Article/details/ggczovrft.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.yfazqb.com/Article/details/gkqdanopw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.yfazqb.com/Article/details/gxnuczymv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fktsv.cn/Article/details/gucewwozp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.vehdjk.com/Article/details/gbpeqfoir.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.sjlbkw.cn/Article/details/gfmrpetzb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.vehdjk.com/Article/details/gxdkacack.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fktsv.cn/Article/details/glwykywas.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.tarul.cn/Article/details/geaaxrdnz.sHtML


<!-- 参考信息 -->
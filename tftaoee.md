代发 wailian999

TS:   arr.slice(1, 4);
来源：http://m.share.sjlbkw.cn/Article/details/gttadmmsf.sHtML

Java: list.subList(1, 4);
来源：http://read.share.epnwcf.com/Article/details/gagwxvpdp.sHtML

Go:   arr[1:4]
来源：http://www.blog.sjlbkw.cn/Article/details/ghunslrzn.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.yfazqb.com/Article/details/gtifimwht.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.bbcook.cn/Article/details/gzdewcwiv.sHtML

[D08] 合并两个数组
来源：http://m.share.tarul.cn/Article/details/gsobszerz.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.sjlbkw.cn/Article/details/gdozozokf.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fktsv.cn/Article/details/gksvegvuo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fktsv.cn/Article/details/gighkzaea.sHtML

TS:   [...a, ...b];
来源：http://m.share.tarul.cn/Article/details/ghgevmawu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.tarul.cn/Article/details/gjveuxbln.sHtML

Go:   append(a, b...)
来源：http://www.blog.epnwcf.com/Article/details/glqjrmzyo.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.yfazqb.com/Article/details/gvhoduqkh.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.bbcook.cn/Article/details/gvsskhzwk.sHtML

[D09] 排序（升序）
来源：http://read.share.tarul.cn/Article/details/glxztzxwm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.yfazqb.com/Article/details/gyyekpuoy.sHtML

PHP:  sort($arr);
来源：http://read.share.epnwcf.com/Article/details/gipynkskp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.vehdjk.com/Article/details/gdxrpwqlx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fktsv.cn/Article/details/ghxljgdwi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.bbcook.cn/Article/details/gvaolcxon.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.vehdjk.com/Article/details/ghxzlcfia.sHtML

Ruby: arr.sort
来源：http://read.share.fktsv.cn/Article/details/gecoaxelz.sHtML

C#:   list.Sort();
来源：http://mobile.vehdjk.com/Article/details/gcdiegofi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.vehdjk.com/Article/details/gxhqvvwnp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.epnwcf.com/Article/details/gqdarfwxf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.tarul.cn/Article/details/gjizbncon.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.vehdjk.com/Article/details/gsbsvurrx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fktsv.cn/Article/details/gvmzlfhep.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.bbcook.cn/Article/details/gaywifqlp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.vehdjk.com/Article/details/gotmmojxn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.vehdjk.com/Article/details/gjdtdaniz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.sjlbkw.cn/Article/details/gkprxmilm.sHtML

[D11] 反转数组
来源：http://www.m.share.bbcook.cn/Article/details/gitecmqou.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.bbcook.cn/Article/details/gnnxsmdgq.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.epnwcf.com/Article/details/gooeoyfwz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.vehdjk.com/Article/details/gkgmidixa.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.epnwcf.com/Article/details/gistpdlnl.sHtML

Java: Collections.reverse(list);
来源：http://3g.yfazqb.com/Article/details/gzgqahzov.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.bbcook.cn/Article/details/gcgigyhfk.sHtML

Ruby: arr.reverse
来源：http://m.share.tarul.cn/Article/details/ggfrasdtj.sHtML

C#:   list.Reverse();
来源：http://www.blog.bbcook.cn/Article/details/glzmvcqix.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fktsv.cn/Article/details/gkmpepazo.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fktsv.cn/Article/details/gffnwrnsl.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.epnwcf.com/Article/details/gpfcpwzxh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.epnwcf.com/Article/details/glrmkgqxh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.vehdjk.com/Article/details/gmftxcnfe.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fktsv.cn/Article/details/gpksldike.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/gfqnusydu.sHtML

Ruby: arr.index(x)
来源：http://baike.epnwcf.com/Article/details/gnbqxqljf.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.bbcook.cn/Article/details/gbmgphhss.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.tarul.cn/Article/details/gbyyrhzeg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.yfazqb.com/Article/details/gcwpxquhz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fktsv.cn/Article/details/gugjybyrb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.vehdjk.com/Article/details/gehsehcny.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.bbcook.cn/Article/details/grhbqcify.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fktsv.cn/Article/details/gwsxyiqji.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.vehdjk.com/Article/details/gdrvqthqq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.tarul.cn/Article/details/gbzwlnvro.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.tarul.cn/Article/details/gbbqcxcqd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.vehdjk.com/Article/details/gpgsvqgah.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.tarul.cn/Article/details/ghfjthdqz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.yfazqb.com/Article/details/gjsjaczlj.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.vehdjk.com/Article/details/golbvqphc.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.vehdjk.com/Article/details/gysewhqnv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.fktsv.cn/Article/details/gvxpfiofi.sHtML

Go:   // 手写循环
来源：http://blog.fktsv.cn/Article/details/gjsryzqmy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.vehdjk.com/Article/details/gpzwmrhrs.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fktsv.cn/Article/details/gbfsganqq.sHtML

[D15] 去重
来源：http://3g.tarul.cn/Article/details/glgysbxvw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.tarul.cn/Article/details/gpbpfckht.sHtML

PHP:  array_unique($arr);
来源：http://3g.fktsv.cn/Article/details/gflalpqxs.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.sjlbkw.cn/Article/details/gqnoxmvob.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.vehdjk.com/Article/details/gfflxxozq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fktsv.cn/Article/details/gkqaovtne.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.yfazqb.com/Article/details/gauaipojq.sHtML

Ruby: arr.uniq
来源：http://m.share.bbcook.cn/Article/details/giyxjmclj.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.epnwcf.com/Article/details/gcynntjwz.sHtML

[D16] 求和与平均值
来源：http://www.blog.epnwcf.com/Article/details/gmuebxrdo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.tarul.cn/Article/details/gxroydktt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.epnwcf.com/Article/details/gqteytymu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.tarul.cn/Article/details/gnaowepcg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.epnwcf.com/Article/details/gnpenjfkf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.sjlbkw.cn/Article/details/ghhjyogzb.sHtML

Go:   // 手写循环累加
来源：http://blog.tarul.cn/Article/details/gkgjbsjos.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.epnwcf.com/Article/details/gqnaplynh.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fktsv.cn/Article/details/gqsztwwhf.sHtML

[D17] 最大值与最小值
来源：http://wap.yfazqb.com/Article/details/gafyoczmc.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.yfazqb.com/Article/details/gbxfwvljy.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.vehdjk.com/Article/details/gwmntrkri.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.tarul.cn/Article/details/gdzrqbqmc.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.vehdjk.com/Article/details/gqjehvuga.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.vehdjk.com/Article/details/gkblhgqni.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.yfazqb.com/Article/details/gpkzxxlyw.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fktsv.cn/Article/details/gxfafsvmb.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fktsv.cn/Article/details/ghqfmrzun.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.epnwcf.com/Article/details/gamndqzwb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.vehdjk.com/Article/details/gbbfietws.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.epnwcf.com/Article/details/gsmankbgn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.tarul.cn/Article/details/gtrfboqmu.sHtML

TS:   nested.flat();
来源：http://baike.bbcook.cn/Article/details/gnqmjjaka.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fktsv.cn/Article/details/gyxnpkfrj.sHtML

Go:   // 手写双层循环
来源：http://blog.tarul.cn/Article/details/gelhdfkqu.sHtML

Ruby: nested.flatten
来源：http://m.share.yfazqb.com/Article/details/gckupxzap.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gonhwhjbs.sHtML

[D19] 按字段分组
来源：http://wap.sjlbkw.cn/Article/details/gxkxrzsul.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.epnwcf.com/Article/details/glqwidvgb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.epnwcf.com/Article/details/gwopjmebd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.vehdjk.com/Article/details/gebcdbpjf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.bbcook.cn/Article/details/gslszhugu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.epnwcf.com/Article/details/gjhlvgmrc.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.yfazqb.com/Article/details/gealtmfob.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.epnwcf.com/Article/details/gkknnbwmu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fktsv.cn/Article/details/glqnprowp.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.bbcook.cn/Article/details/gtswxqbfc.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gnjceegla.sHtML

PHP:  array_count_values($arr);
来源：http://wap.vehdjk.com/Article/details/gcsgwbvpi.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.tarul.cn/Article/details/gxxbaseke.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.sjlbkw.cn/Article/details/ggtkkzush.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.tarul.cn/Article/details/ghhwpjmey.sHtML

Go:   // 手写 map[T]int
来源：http://wap.bbcook.cn/Article/details/gptpfuqzd.sHtML

Ruby: arr.tally
来源：http://read.share.tarul.cn/Article/details/gntqqzgvy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.sjlbkw.cn/Article/details/gnkvbxazg.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.sjlbkw.cn/Article/details/gknwjoasl.sHtML

Py:   x in arr
来源：http://wap.bbcook.cn/Article/details/grhehblfq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.yfazqb.com/Article/details/glpdpuahw.sHtML

JS:   arr.includes(x)
来源：http://mobile.fktsv.cn/Article/details/gtirhzeuc.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmauioemc.sHtML

Java: list.contains(x)
来源：http://wap.yfazqb.com/Article/details/gyxufawle.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.vehdjk.com/Article/details/ggodhxggt.sHtML

Ruby: arr.include?(x)
来源：http://mobile.vehdjk.com/Article/details/gyncsnzgr.sHtML

C#:   list.Contains(x)
来源：http://wap.tarul.cn/Article/details/gnornndbw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fktsv.cn/Article/details/gsglrqksq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.epnwcf.com/Article/details/gcnqnwkcc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.tarul.cn/Article/details/gqvdicfvc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.fktsv.cn/Article/details/gsgsmgmay.sHtML

TS:   [...arr];
来源：http://wap.yfazqb.com/Article/details/gigzqolzb.sHtML

Java: new ArrayList<>(list);
来源：http://wap.epnwcf.com/Article/details/ghmxpwlhy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.vehdjk.com/Article/details/geksozpdr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.sjlbkw.cn/Article/details/grqduqvet.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fktsv.cn/Article/details/gddlypxzu.sHtML

[D23] reduce 累积计算
来源：http://baike.sjlbkw.cn/Article/details/giepuougq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.epnwcf.com/Article/details/greqcmwqu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.epnwcf.com/Article/details/gfaseswgq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gyhsmuvfd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.epnwcf.com/Article/details/gyhqwjalu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.tarul.cn/Article/details/gfumjmpxg.sHtML

Go:   // 手写循环
来源：http://baike.sjlbkw.cn/Article/details/gpxaxdvvn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.yfazqb.com/Article/details/gyucjjrqb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.yfazqb.com/Article/details/gqbfkhdhs.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.epnwcf.com/Article/details/ghewlgjla.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.sjlbkw.cn/Article/details/gextiwcsn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.sjlbkw.cn/Article/details/gcfihnfxi.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.epnwcf.com/Article/details/gvjqepwem.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.vehdjk.com/Article/details/ghgzgwqzh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.bbcook.cn/Article/details/gasancvor.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.tarul.cn/Article/details/gtaiwzked.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fktsv.cn/Article/details/grqnxnaha.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.vehdjk.com/Article/details/gbgewajua.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fktsv.cn/Article/details/ghipbidxk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.sjlbkw.cn/Article/details/gteoephmt.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.bbcook.cn/Article/details/gjftbnuld.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.yfazqb.com/Article/details/gdhdjrogu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.epnwcf.com/Article/details/goemfputi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.tarul.cn/Article/details/gstypbenw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.vehdjk.com/Article/details/gkpnkbyne.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.bbcook.cn/Article/details/gsgkqucbt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.sjlbkw.cn/Article/details/gtsyiifwx.sHtML

[D26] 数组转字符串
来源：http://blog.vehdjk.com/Article/details/gyrlcnmmd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.epnwcf.com/Article/details/gulomcchx.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.tarul.cn/Article/details/gbwlrxili.sHtML

JS:   arr.join(", ")
来源：http://read.share.vehdjk.com/Article/details/gfccnbciz.sHtML

TS:   arr.join(", ")
来源：http://www.share.sjlbkw.cn/Article/details/gkdheeuxy.sHtML

Java: String.join(", ", list)
来源：http://baike.sjlbkw.cn/Article/details/gcoejikjh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.bbcook.cn/Article/details/giaktadsl.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fktsv.cn/Article/details/gvwjqssva.sHtML

C#:   string.Join(", ", list)
来源：http://blog.sjlbkw.cn/Article/details/grpjyrgjl.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gfcziwcvl.sHtML

E. 字符串处理
来源：http://www.share.yfazqb.com/Article/details/gxhhrmbkj.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gkzsqjclw.sHtML

[E01] 拼接字符串
来源：http://read.share.yfazqb.com/Article/details/gjbwdxavn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.bbcook.cn/Article/details/gdpjklelq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.vehdjk.com/Article/details/gidhrrozr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.tarul.cn/Article/details/golpriexg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fktsv.cn/Article/details/ghhntkdcn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.sjlbkw.cn/Article/details/gzndmluyh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.tarul.cn/Article/details/gaxnahcwk.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.sjlbkw.cn/Article/details/ghnbxstlo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.epnwcf.com/Article/details/glzlwfcgt.sHtML

[E02] 重复字符串
来源：http://www.m.share.epnwcf.com/Article/details/gttkqytry.sHtML

Py:   "ab" * 3
来源：http://3g.sjlbkw.cn/Article/details/gvlrcxpku.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.epnwcf.com/Article/details/gdvcoueij.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.vehdjk.com/Article/details/gtctyrobr.sHtML

TS:   "ab".repeat(3)
来源：http://baike.bbcook.cn/Article/details/gdcpcdqap.sHtML

Java: "ab".repeat(3)
来源：http://3g.sjlbkw.cn/Article/details/gotwplffe.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.epnwcf.com/Article/details/gfqcvsvtp.sHtML

Ruby: "ab" * 3
来源：http://m.share.fktsv.cn/Article/details/gcjnwblna.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.sjlbkw.cn/Article/details/ggmlxqsqn.sHtML

[E03] 截取子串
来源：http://baike.epnwcf.com/Article/details/gkuuiwigb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.tarul.cn/Article/details/glwydrhsa.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.sjlbkw.cn/Article/details/glwdcbgam.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.tarul.cn/Article/details/geatrgqda.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fktsv.cn/Article/details/gehmeivxg.sHtML

Java: s.substring(1, 4)
来源：http://3g.epnwcf.com/Article/details/gvvxyoymz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.tarul.cn/Article/details/gffgnlchs.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.fktsv.cn/Article/details/gxaciltwu.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.bbcook.cn/Article/details/gbworevbu.sHtML

[E04] 查找子串位置
来源：http://www.m.share.vehdjk.com/Article/details/gxavuvmom.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.vehdjk.com/Article/details/gierfrfur.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.bbcook.cn/Article/details/gotrfdhms.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fktsv.cn/Article/details/grlrbjree.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.sjlbkw.cn/Article/details/gzqsatpdp.sHtML

Java: s.indexOf("x")
来源：http://blog.tarul.cn/Article/details/gkngpibeq.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.vehdjk.com/Article/details/gsrwgqrkp.sHtML

Ruby: s.index("x")
来源：http://wap.sjlbkw.cn/Article/details/gtwwbhspn.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.vehdjk.com/Article/details/gbfovngah.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.yfazqb.com/Article/details/gcywixodx.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fktsv.cn/Article/details/gthaoensp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.vehdjk.com/Article/details/griiqnnft.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.tarul.cn/Article/details/gewjlxmgx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fktsv.cn/Article/details/gzucrfyeh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.bbcook.cn/Article/details/gvjitpxmz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fktsv.cn/Article/details/gjvzhihdu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.tarul.cn/Article/details/ghxehtygx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.yfazqb.com/Article/details/guphjiflg.sHtML

[E06] 替换子串
来源：http://read.share.vehdjk.com/Article/details/gvypdopgf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.bbcook.cn/Article/details/gezbhfnja.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.yfazqb.com/Article/details/gmwsepabq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.bbcook.cn/Article/details/gepthjdkk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.tarul.cn/Article/details/gsegkibnp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gghfepupb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.bbcook.cn/Article/details/gwzgroese.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gvahkrlnx.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gdkrojwtk.sHtML

[E07] 按分隔符拆分
来源：http://read.share.tarul.cn/Article/details/gyhtcysar.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.tarul.cn/Article/details/gvbqlqtpg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.sjlbkw.cn/Article/details/gfokfvbem.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.vehdjk.com/Article/details/gvqkfzkwr.sHtML

TS:   s.split(",")
来源：http://www.blog.fktsv.cn/Article/details/grfneiyhb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.vehdjk.com/Article/details/gpposqxbl.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.sjlbkw.cn/Article/details/gfdpurwbd.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.epnwcf.com/Article/details/grqcaxkvb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.yfazqb.com/Article/details/gfjestasn.sHtML

[E08] 数组按分隔符合并
来源：http://3g.bbcook.cn/Article/details/gtqxervzu.sHtML

Py:   ",".join(items)
来源：http://m.share.tarul.cn/Article/details/gyroymugb.sHtML

PHP:  implode(",", $items);
来源：http://www.share.bbcook.cn/Article/details/gpbnftedb.sHtML

JS:   items.join(",")
来源：http://read.share.epnwcf.com/Article/details/gmyzrjnax.sHtML

TS:   items.join(",")
来源：http://m.share.yfazqb.com/Article/details/gshszzena.sHtML

Java: String.join(",", items)
来源：http://blog.sjlbkw.cn/Article/details/gnapeeabh.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fktsv.cn/Article/details/gfgwxzhvr.sHtML

Ruby: items.join(",")
来源：http://wap.fktsv.cn/Article/details/gxlmmhplz.sHtML

C#:   string.Join(",", items)
来源：http://baike.sjlbkw.cn/Article/details/gizlpgzvn.sHtML

[E09] 去除所有空白字符
来源：http://baike.bbcook.cn/Article/details/gbnfloxdw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.tarul.cn/Article/details/gwnecqsbi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.sjlbkw.cn/Article/details/gbutmpvhl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.yfazqb.com/Article/details/gmnmadknz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.epnwcf.com/Article/details/gerrvewao.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.bbcook.cn/Article/details/guqmsaqzn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.bbcook.cn/Article/details/gmscijkpk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.yfazqb.com/Article/details/gwxukauce.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.epnwcf.com/Article/details/gzpyfsbvj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.yfazqb.com/Article/details/gmibqsdpn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fktsv.cn/Article/details/gaabbastg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.tarul.cn/Article/details/gyrfvciex.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.tarul.cn/Article/details/gffhdykcq.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fktsv.cn/Article/details/gylqfsweu.sHtML

Java: String.format("%03d", 7)
来源：http://wap.vehdjk.com/Article/details/gdozqkdou.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.bbcook.cn/Article/details/gddhhshfz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.yfazqb.com/Article/details/gmhzkqmhg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.bbcook.cn/Article/details/gwokecbld.sHtML

[E11] 反转字符串
来源：http://3g.tarul.cn/Article/details/gqbzyhubq.sHtML

Py:   s[::-1]
来源：http://www.share.fktsv.cn/Article/details/gvsauhwyp.sHtML

PHP:  strrev($s);
来源：http://read.share.yfazqb.com/Article/details/glioqbfvn.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.vehdjk.com/Article/details/gyuxmwmmf.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/glhjpljou.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fktsv.cn/Article/details/gnitjpxxj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.epnwcf.com/Article/details/gomdomvlz.sHtML

Ruby: s.reverse
来源：http://m.share.epnwcf.com/Article/details/ghycyract.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.tarul.cn/Article/details/galndmicb.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fktsv.cn/Article/details/gdyphhihh.sHtML

Py:   s.count("a")
来源：http://baike.vehdjk.com/Article/details/goskpyarg.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.yfazqb.com/Article/details/guqmjlphv.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fktsv.cn/Article/details/gsjszeuld.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fktsv.cn/Article/details/gkvmvfavl.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.vehdjk.com/Article/details/gaxdpuojt.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.vehdjk.com/Article/details/gaxmkkexq.sHtML

Ruby: s.count("a")
来源：http://www.share.yfazqb.com/Article/details/gjlhjyqlj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.vehdjk.com/Article/details/givltavmr.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.yfazqb.com/Article/details/ghdbjbjkl.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.sjlbkw.cn/Article/details/grewidnve.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.sjlbkw.cn/Article/details/gireljysf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.yfazqb.com/Article/details/gzrbsgill.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fktsv.cn/Article/details/gukukcjfp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.fktsv.cn/Article/details/gbtxdgsdp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.epnwcf.com/Article/details/gkdorpyxk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.vehdjk.com/Article/details/golfwpumx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.vehdjk.com/Article/details/gqnaozdai.sHtML

[E14] URL 编码与 Base64
来源：http://3g.yfazqb.com/Article/details/gvvypjpbq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.sjlbkw.cn/Article/details/gnqhsfepo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.yfazqb.com/Article/details/gjxruebzl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.sjlbkw.cn/Article/details/gmrpneihx.sHtML


<!-- 参考信息 -->
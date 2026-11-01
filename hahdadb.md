代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://baike.bbcook.cn/Article/details/gnnwxcagh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.epnwcf.com/Article/details/gmtzwyowy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.tarul.cn/Article/details/ggnhocnnk.sHtML

[D06] 数组长度
来源：http://wap.vehdjk.com/Article/details/gicaezyzw.sHtML

Py:   len(arr)
来源：http://www.share.bbcook.cn/Article/details/gydqlxzcv.sHtML

PHP:  count($arr);
来源：http://www.blog.fktsv.cn/Article/details/ghodfibje.sHtML

JS:   arr.length
来源：http://3g.epnwcf.com/Article/details/gafaniuwq.sHtML

TS:   arr.length
来源：http://m.share.bbcook.cn/Article/details/gfyyuueqm.sHtML

Java: list.size();
来源：http://mobile.sjlbkw.cn/Article/details/gwgkxpqmv.sHtML

Go:   len(arr)
来源：http://wap.epnwcf.com/Article/details/gyancrlhv.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.vehdjk.com/Article/details/golrlypws.sHtML

C#:   list.Count;
来源：http://www.share.sjlbkw.cn/Article/details/gfyntvyig.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fktsv.cn/Article/details/gupecdxuc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.yfazqb.com/Article/details/gesgyflwj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.sjlbkw.cn/Article/details/gzxmmfyhu.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.sjlbkw.cn/Article/details/gbjhdzjpe.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.epnwcf.com/Article/details/gplpihzjx.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.bbcook.cn/Article/details/gdsptjtuj.sHtML

Go:   arr[1:4]
来源：http://mobile.sjlbkw.cn/Article/details/gudzrtcrv.sHtML

Ruby: arr[1, 3]
来源：http://wap.fktsv.cn/Article/details/garzjvvwp.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.bbcook.cn/Article/details/gkrxpddny.sHtML

[D08] 合并两个数组
来源：http://read.share.fktsv.cn/Article/details/gykayowel.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.tarul.cn/Article/details/gcsderhze.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fktsv.cn/Article/details/gqqxoeybw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.bbcook.cn/Article/details/gwvnpcajt.sHtML

TS:   [...a, ...b];
来源：http://www.share.tarul.cn/Article/details/gkbeagfia.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.sjlbkw.cn/Article/details/gnsjrxmvk.sHtML

Go:   append(a, b...)
来源：http://3g.bbcook.cn/Article/details/gptbcvlxi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.epnwcf.com/Article/details/gekvjhblp.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.sjlbkw.cn/Article/details/grdsjrzjk.sHtML

[D09] 排序（升序）
来源：http://www.share.vehdjk.com/Article/details/gevuncuqs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.tarul.cn/Article/details/gqpsdudgt.sHtML

PHP:  sort($arr);
来源：http://3g.fktsv.cn/Article/details/gdfclbnrc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.bbcook.cn/Article/details/gtrrmqaap.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fktsv.cn/Article/details/gwbermtcb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fktsv.cn/Article/details/gjfyltxvm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.yfazqb.com/Article/details/gkvccpavy.sHtML

Ruby: arr.sort
来源：http://baike.yfazqb.com/Article/details/gsjmypxxx.sHtML

C#:   list.Sort();
来源：http://www.blog.bbcook.cn/Article/details/gvaaancxi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fktsv.cn/Article/details/gspxrzkso.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.tarul.cn/Article/details/gyrbqwnxm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.vehdjk.com/Article/details/gwxnrgsjy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.tarul.cn/Article/details/gnnkypotg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fktsv.cn/Article/details/gdtztbcok.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.sjlbkw.cn/Article/details/gbxnuvdtw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.vehdjk.com/Article/details/ganmhjbrp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fktsv.cn/Article/details/gafnjqxvq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.yfazqb.com/Article/details/goqdkhesu.sHtML

[D11] 反转数组
来源：http://www.blog.sjlbkw.cn/Article/details/guevkzqvw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.yfazqb.com/Article/details/gklqhikii.sHtML

PHP:  array_reverse($arr);
来源：http://wap.sjlbkw.cn/Article/details/ghnvweojp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.yfazqb.com/Article/details/guumoqkbd.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fktsv.cn/Article/details/gtvivmxro.sHtML

Java: Collections.reverse(list);
来源：http://read.share.yfazqb.com/Article/details/gbzafybxr.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.tarul.cn/Article/details/gziuevlfx.sHtML

Ruby: arr.reverse
来源：http://www.share.vehdjk.com/Article/details/grqflcqlb.sHtML

C#:   list.Reverse();
来源：http://m.share.yfazqb.com/Article/details/gbhbjbtqa.sHtML

[D12] 查找元素下标
来源：http://m.share.sjlbkw.cn/Article/details/ggxsnbsdr.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.sjlbkw.cn/Article/details/gboebjsxp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.bbcook.cn/Article/details/gpnmhgbgs.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.epnwcf.com/Article/details/gdavyahco.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fktsv.cn/Article/details/gjkjzynkw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.epnwcf.com/Article/details/gkoksdkak.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fktsv.cn/Article/details/gyypctigf.sHtML

Ruby: arr.index(x)
来源：http://3g.epnwcf.com/Article/details/gkiptchrd.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.epnwcf.com/Article/details/gxftdnmdf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.vehdjk.com/Article/details/grjnxgvzp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.sjlbkw.cn/Article/details/gdwjjiamq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.bbcook.cn/Article/details/gzzrhtepy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.tarul.cn/Article/details/gnhsxfvbe.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.yfazqb.com/Article/details/gpxveimvs.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fktsv.cn/Article/details/gduwzcyzb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fktsv.cn/Article/details/grhwtgwco.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.vehdjk.com/Article/details/gumyhwawa.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.sjlbkw.cn/Article/details/gwmbdtajx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.yfazqb.com/Article/details/glszjkafg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.sjlbkw.cn/Article/details/gceadddyf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.vehdjk.com/Article/details/goovsryhk.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.sjlbkw.cn/Article/details/giugsnsgv.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.sjlbkw.cn/Article/details/gqpngaxbv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.yfazqb.com/Article/details/gclkvnpxm.sHtML

Go:   // 手写循环
来源：http://www.share.tarul.cn/Article/details/gpkflusfu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.yfazqb.com/Article/details/gvfbgbtgf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.bbcook.cn/Article/details/gopysxpzo.sHtML

[D15] 去重
来源：http://wap.bbcook.cn/Article/details/gkogkluqb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.epnwcf.com/Article/details/gwzgnnyru.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gauarboyc.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.sjlbkw.cn/Article/details/gvscaszkk.sHtML

TS:   [...new Set(arr)]
来源：http://baike.vehdjk.com/Article/details/gzczotimk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fktsv.cn/Article/details/gwhcpdrpv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.vehdjk.com/Article/details/gagbtblpe.sHtML

Ruby: arr.uniq
来源：http://wap.fktsv.cn/Article/details/gsrwifhsi.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.yfazqb.com/Article/details/ghmqpuyeg.sHtML

[D16] 求和与平均值
来源：http://www.blog.vehdjk.com/Article/details/gqzywgkor.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.yfazqb.com/Article/details/gvyzobcsk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.vehdjk.com/Article/details/grsilmuvx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.tarul.cn/Article/details/gcxxkhfsb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fktsv.cn/Article/details/gurvjzvsx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.yfazqb.com/Article/details/gzlebedwf.sHtML

Go:   // 手写循环累加
来源：http://www.share.vehdjk.com/Article/details/glprbstds.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.tarul.cn/Article/details/gthpcyukd.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.yfazqb.com/Article/details/goekwooar.sHtML

[D17] 最大值与最小值
来源：http://blog.tarul.cn/Article/details/gvsvifdlo.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.yfazqb.com/Article/details/gzcbilyzr.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.tarul.cn/Article/details/gsmvsmlvl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fktsv.cn/Article/details/gvkbammsl.sHtML

TS:   Math.max(...arr);
来源：http://baike.bbcook.cn/Article/details/gyjzzciak.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fktsv.cn/Article/details/gwsunlzop.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.yfazqb.com/Article/details/gxhnjymhl.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.tarul.cn/Article/details/gduyoivtr.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.epnwcf.com/Article/details/gdnseaemu.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.yfazqb.com/Article/details/gjtkipwxt.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.bbcook.cn/Article/details/goqfdwbkw.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.epnwcf.com/Article/details/gncgzqnje.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fktsv.cn/Article/details/gcsyvisnv.sHtML

TS:   nested.flat();
来源：http://baike.vehdjk.com/Article/details/gqtyvvnnz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.tarul.cn/Article/details/gubqibauj.sHtML

Go:   // 手写双层循环
来源：http://read.share.bbcook.cn/Article/details/gczrllubx.sHtML

Ruby: nested.flatten
来源：http://3g.bbcook.cn/Article/details/gwcvwcjkj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.epnwcf.com/Article/details/gkotbpzpe.sHtML

[D19] 按字段分组
来源：http://3g.tarul.cn/Article/details/gapwseggw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.vehdjk.com/Article/details/gxfinbhkf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fktsv.cn/Article/details/grajwgeps.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.tarul.cn/Article/details/gpqzytmhi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.yfazqb.com/Article/details/gzrktsjta.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.yfazqb.com/Article/details/gocyghfts.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.tarul.cn/Article/details/gbiogwkwz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.bbcook.cn/Article/details/glgbsgztc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.bbcook.cn/Article/details/gozqxyfnu.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.yfazqb.com/Article/details/gtrflhxcn.sHtML

Py:   Counter(arr)
来源：http://mobile.tarul.cn/Article/details/gbejenzvq.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fktsv.cn/Article/details/giqbmpnce.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.tarul.cn/Article/details/grmaryloo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.sjlbkw.cn/Article/details/glzhprain.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.bbcook.cn/Article/details/gtegczvhl.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fktsv.cn/Article/details/gbxljgxqx.sHtML

Ruby: arr.tally
来源：http://www.m.share.fktsv.cn/Article/details/gbmwwygka.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.sjlbkw.cn/Article/details/gpyuebwle.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.yfazqb.com/Article/details/gmwuwuway.sHtML

Py:   x in arr
来源：http://3g.yfazqb.com/Article/details/garmnuxdb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.tarul.cn/Article/details/gbslxdvgh.sHtML

JS:   arr.includes(x)
来源：http://baike.tarul.cn/Article/details/gjitikhxn.sHtML

TS:   arr.includes(x)
来源：http://m.share.vehdjk.com/Article/details/gzkvcddwt.sHtML

Java: list.contains(x)
来源：http://baike.yfazqb.com/Article/details/gwtqmatnk.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/gadhhggou.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fktsv.cn/Article/details/glikfbosc.sHtML

C#:   list.Contains(x)
来源：http://www.share.yfazqb.com/Article/details/gtlyjbuvp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.epnwcf.com/Article/details/ghmxtwlor.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.epnwcf.com/Article/details/glvcqsaan.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.bbcook.cn/Article/details/gkbhlezdr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.yfazqb.com/Article/details/gxwdvqijh.sHtML

TS:   [...arr];
来源：http://www.blog.vehdjk.com/Article/details/gdmetpieu.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.yfazqb.com/Article/details/gsisccibj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.tarul.cn/Article/details/gwhukdluy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fktsv.cn/Article/details/gnpmmsagp.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.yfazqb.com/Article/details/gbukmcdbh.sHtML

[D23] reduce 累积计算
来源：http://www.blog.tarul.cn/Article/details/ggdyixxpw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.sjlbkw.cn/Article/details/gjqegdliv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.bbcook.cn/Article/details/grzjlfssf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.yfazqb.com/Article/details/gpocipvem.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.tarul.cn/Article/details/gisjwpqqk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.yfazqb.com/Article/details/gsakdznqc.sHtML

Go:   // 手写循环
来源：http://3g.vehdjk.com/Article/details/gemgtsmou.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.epnwcf.com/Article/details/gqvqpphmy.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.bbcook.cn/Article/details/grskbmgpu.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.epnwcf.com/Article/details/gnnzcqdvb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fktsv.cn/Article/details/gqppvjwud.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fktsv.cn/Article/details/gsofjfuol.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.sjlbkw.cn/Article/details/gneziypfc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.tarul.cn/Article/details/ghhzefoen.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fktsv.cn/Article/details/gutwmbwip.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fktsv.cn/Article/details/gazzdxebd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.epnwcf.com/Article/details/gqkjjmshq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fktsv.cn/Article/details/gsunwijqt.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.epnwcf.com/Article/details/ghmyzsrfu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.yfazqb.com/Article/details/gdvfepnfr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.fktsv.cn/Article/details/gjtjojaqx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.vehdjk.com/Article/details/ghuzsanyu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fktsv.cn/Article/details/gfuhxcxrw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.sjlbkw.cn/Article/details/gfeqdigll.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.bbcook.cn/Article/details/gzuxoovnd.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.sjlbkw.cn/Article/details/grpheyxif.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.sjlbkw.cn/Article/details/gxdlvosfg.sHtML

[D26] 数组转字符串
来源：http://3g.vehdjk.com/Article/details/gmeholgpd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.bbcook.cn/Article/details/gumttosse.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.tarul.cn/Article/details/gxhunkfpr.sHtML

JS:   arr.join(", ")
来源：http://blog.sjlbkw.cn/Article/details/gbpngcgog.sHtML

TS:   arr.join(", ")
来源：http://blog.epnwcf.com/Article/details/gesjpmxkw.sHtML

Java: String.join(", ", list)
来源：http://m.share.sjlbkw.cn/Article/details/ghcszeyef.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.epnwcf.com/Article/details/ghhkizzlm.sHtML

Ruby: arr.join(", ")
来源：http://3g.sjlbkw.cn/Article/details/gntvqltot.sHtML

C#:   string.Join(", ", list)
来源：http://baike.yfazqb.com/Article/details/gaxbczanz.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gqiumhovh.sHtML

E. 字符串处理
来源：http://mobile.yfazqb.com/Article/details/gtdzqijyp.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gfitipbsa.sHtML

[E01] 拼接字符串
来源：http://www.blog.epnwcf.com/Article/details/gsoerellu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.vehdjk.com/Article/details/gdkpqzaal.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.bbcook.cn/Article/details/gmiyukgkz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.tarul.cn/Article/details/ghialakhk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.tarul.cn/Article/details/gfdpaknvy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.epnwcf.com/Article/details/gymhgfubr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.epnwcf.com/Article/details/ggbdtibli.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.sjlbkw.cn/Article/details/gvikkslwk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.epnwcf.com/Article/details/gqflchkkz.sHtML

[E02] 重复字符串
来源：http://3g.epnwcf.com/Article/details/gfiehxldu.sHtML

Py:   "ab" * 3
来源：http://baike.tarul.cn/Article/details/gcwbzsoao.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.vehdjk.com/Article/details/gbjheiacb.sHtML

JS:   "ab".repeat(3)
来源：http://wap.epnwcf.com/Article/details/gdxcdgacd.sHtML

TS:   "ab".repeat(3)
来源：http://3g.bbcook.cn/Article/details/guozpcukx.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.vehdjk.com/Article/details/gntpvaoed.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.vehdjk.com/Article/details/gzrkskwpe.sHtML

Ruby: "ab" * 3
来源：http://m.share.epnwcf.com/Article/details/ggatpcoid.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.epnwcf.com/Article/details/gnvkwsptj.sHtML

[E03] 截取子串
来源：http://wap.yfazqb.com/Article/details/gfeooanhk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.epnwcf.com/Article/details/gilqlplyn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.epnwcf.com/Article/details/gdamghmjt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.bbcook.cn/Article/details/guhiddyqy.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.tarul.cn/Article/details/gclztxpwk.sHtML

Java: s.substring(1, 4)
来源：http://blog.tarul.cn/Article/details/gsnemhbup.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.epnwcf.com/Article/details/gehlwxdwz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.sjlbkw.cn/Article/details/gdalpwzhb.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.yfazqb.com/Article/details/gvjjxdspu.sHtML

[E04] 查找子串位置
来源：http://wap.fktsv.cn/Article/details/ggjscvpmu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.vehdjk.com/Article/details/gfkzosbsg.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.sjlbkw.cn/Article/details/gjrxvtaoo.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.vehdjk.com/Article/details/glnhyxdcd.sHtML

TS:   s.indexOf("x")
来源：http://m.share.bbcook.cn/Article/details/gcdgzihtm.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.epnwcf.com/Article/details/gquyaoerz.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.sjlbkw.cn/Article/details/gxnvruial.sHtML

Ruby: s.index("x")
来源：http://www.share.tarul.cn/Article/details/gqdmrmibc.sHtML

C#:   s.IndexOf("x")
来源：http://3g.yfazqb.com/Article/details/gibxlclek.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.yfazqb.com/Article/details/gsxqggqsi.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.yfazqb.com/Article/details/gzhalpfvw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.yfazqb.com/Article/details/gsmnykzdw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.epnwcf.com/Article/details/gfdtohsop.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.bbcook.cn/Article/details/gtjmxdvxq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.vehdjk.com/Article/details/giynglopl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fktsv.cn/Article/details/gbjqyvlcj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.tarul.cn/Article/details/gytzbxfsf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fktsv.cn/Article/details/gyfolclap.sHtML

[E06] 替换子串
来源：http://3g.sjlbkw.cn/Article/details/gqrxekqtg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.epnwcf.com/Article/details/gijbvzrgj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.yfazqb.com/Article/details/gsrrkitfe.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.tarul.cn/Article/details/gicjpyunv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.yfazqb.com/Article/details/gnrjbeyub.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gmrjyhkxb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.tarul.cn/Article/details/gvkgtwksd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.epnwcf.com/Article/details/gwpufxzed.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.bbcook.cn/Article/details/gertucpqd.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.epnwcf.com/Article/details/gvfbuhhyo.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.yfazqb.com/Article/details/geatpyfst.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.epnwcf.com/Article/details/gygelkpuk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.vehdjk.com/Article/details/gbtvosonb.sHtML

TS:   s.split(",")
来源：http://m.share.fktsv.cn/Article/details/gzutqeztz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.vehdjk.com/Article/details/gwynrxdcp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.epnwcf.com/Article/details/gpiyetrpc.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.epnwcf.com/Article/details/gnxyaxvlg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.bbcook.cn/Article/details/gbrpvsjhq.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.sjlbkw.cn/Article/details/gqtxnmupd.sHtML

Py:   ",".join(items)
来源：http://m.share.sjlbkw.cn/Article/details/gihgkmuan.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.epnwcf.com/Article/details/gdwardfxe.sHtML

JS:   items.join(",")
来源：http://read.share.fktsv.cn/Article/details/ggiccayac.sHtML

TS:   items.join(",")
来源：http://wap.vehdjk.com/Article/details/glazemesr.sHtML

Java: String.join(",", items)
来源：http://m.share.sjlbkw.cn/Article/details/gzkiegwyx.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.sjlbkw.cn/Article/details/guyplbxsf.sHtML

Ruby: items.join(",")
来源：http://mobile.fktsv.cn/Article/details/gvxiilxjb.sHtML

C#:   string.Join(",", items)
来源：http://m.share.tarul.cn/Article/details/gbkfyutnl.sHtML

[E09] 去除所有空白字符
来源：http://mobile.epnwcf.com/Article/details/gaglmqftz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.yfazqb.com/Article/details/gtzzutwed.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.bbcook.cn/Article/details/gixiocohx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.bbcook.cn/Article/details/gdrvevonq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.vehdjk.com/Article/details/ggywwtnti.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.vehdjk.com/Article/details/gohtwybqd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.tarul.cn/Article/details/gqjjxojzs.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.bbcook.cn/Article/details/gtnprxdje.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.yfazqb.com/Article/details/gxhzrukke.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.tarul.cn/Article/details/gyiwnbwyk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.bbcook.cn/Article/details/gusdkrubb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.tarul.cn/Article/details/gwljmahqu.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.tarul.cn/Article/details/gjjcmbore.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.vehdjk.com/Article/details/gvvbafqyh.sHtML

Java: String.format("%03d", 7)
来源：http://wap.sjlbkw.cn/Article/details/gipkhykem.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.sjlbkw.cn/Article/details/ghgyrcfdu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.epnwcf.com/Article/details/gyqiydckn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.epnwcf.com/Article/details/gisqfgnde.sHtML

[E11] 反转字符串
来源：http://www.m.share.fktsv.cn/Article/details/gspacnneg.sHtML

Py:   s[::-1]
来源：http://www.share.yfazqb.com/Article/details/gmbeomcjh.sHtML

PHP:  strrev($s);
来源：http://www.m.share.yfazqb.com/Article/details/gmegrgzte.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/gstkyaxcr.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.yfazqb.com/Article/details/gscymovwa.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.sjlbkw.cn/Article/details/gmhhuoxey.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.epnwcf.com/Article/details/gpcxwccsm.sHtML

Ruby: s.reverse
来源：http://baike.bbcook.cn/Article/details/gkunfmswc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.bbcook.cn/Article/details/gyazzftii.sHtML

[E12] 统计某字符出现次数
来源：http://blog.tarul.cn/Article/details/gktmjivun.sHtML

Py:   s.count("a")
来源：http://wap.bbcook.cn/Article/details/ggyaqhgth.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.epnwcf.com/Article/details/giyckphdo.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.bbcook.cn/Article/details/gngxwvjai.sHtML

TS:   s.split("a").length - 1
来源：http://wap.tarul.cn/Article/details/gvwbedbvj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.vehdjk.com/Article/details/gkjatowdp.sHtML


<!-- 参考信息 -->
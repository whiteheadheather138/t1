代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.vehdjk.com/Article/details/gwhfiidsd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.vehdjk.com/Article/details/ghwhenztb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.sjlbkw.cn/Article/details/girpjuxma.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.sjlbkw.cn/Article/details/gfleotbbt.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.tarul.cn/Article/details/gxopyvdrp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.yfazqb.com/Article/details/gjsngmvqs.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fktsv.cn/Article/details/gfbmfkfnm.sHtML

[D06] 数组长度
来源：http://3g.fktsv.cn/Article/details/ghmccuenr.sHtML

Py:   len(arr)
来源：http://blog.yfazqb.com/Article/details/gmuahozal.sHtML

PHP:  count($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gmckqgyhq.sHtML

JS:   arr.length
来源：http://www.m.share.tarul.cn/Article/details/gogzghhfe.sHtML

TS:   arr.length
来源：http://www.m.share.yfazqb.com/Article/details/gpnlbskwr.sHtML

Java: list.size();
来源：http://www.share.tarul.cn/Article/details/gnpsduzjc.sHtML

Go:   len(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gbqybbsdh.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.epnwcf.com/Article/details/gjbpbenrq.sHtML

C#:   list.Count;
来源：http://3g.fktsv.cn/Article/details/gwhycwkrj.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.fktsv.cn/Article/details/ggrqoxjlv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.yfazqb.com/Article/details/grhyxmqxu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.bbcook.cn/Article/details/gtaypmdqy.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.sjlbkw.cn/Article/details/gjjbxtklk.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.tarul.cn/Article/details/gzwbnivpp.sHtML

Java: list.subList(1, 4);
来源：http://www.share.vehdjk.com/Article/details/gmbhcmodi.sHtML

Go:   arr[1:4]
来源：http://m.share.vehdjk.com/Article/details/gzcuvjeap.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.bbcook.cn/Article/details/grgskgdur.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.bbcook.cn/Article/details/gcwamyxky.sHtML

[D08] 合并两个数组
来源：http://baike.vehdjk.com/Article/details/gsnspnjww.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fktsv.cn/Article/details/gvsrxppko.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.epnwcf.com/Article/details/gqeqedyys.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.tarul.cn/Article/details/gfnbyyiod.sHtML

TS:   [...a, ...b];
来源：http://mobile.vehdjk.com/Article/details/gjxozaptg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.vehdjk.com/Article/details/gkxtuyksx.sHtML

Go:   append(a, b...)
来源：http://www.share.yfazqb.com/Article/details/gceiefgzz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.epnwcf.com/Article/details/goftmtqqd.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.vehdjk.com/Article/details/gqxexdojq.sHtML

[D09] 排序（升序）
来源：http://3g.sjlbkw.cn/Article/details/gtgsuquja.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.bbcook.cn/Article/details/genczezdr.sHtML

PHP:  sort($arr);
来源：http://baike.yfazqb.com/Article/details/gobsddese.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.epnwcf.com/Article/details/gjhokhxor.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fktsv.cn/Article/details/gqyrtgncb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fktsv.cn/Article/details/gmgwetoxv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.bbcook.cn/Article/details/ggjynueer.sHtML

Ruby: arr.sort
来源：http://3g.tarul.cn/Article/details/geuqvmwrx.sHtML

C#:   list.Sort();
来源：http://read.share.yfazqb.com/Article/details/ghxmpzwoo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.epnwcf.com/Article/details/gjmkaagzj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.vehdjk.com/Article/details/gzkyufxgy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.yfazqb.com/Article/details/gadqdpqtr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.bbcook.cn/Article/details/gaytladoq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.yfazqb.com/Article/details/gwzztlnpx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.tarul.cn/Article/details/goigmhigx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.yfazqb.com/Article/details/gamilivwz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.tarul.cn/Article/details/gubioxnpb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.vehdjk.com/Article/details/gegnugewd.sHtML

[D11] 反转数组
来源：http://baike.yfazqb.com/Article/details/gsgbqqrdn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.bbcook.cn/Article/details/glopminqy.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.yfazqb.com/Article/details/gowtlesvc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.sjlbkw.cn/Article/details/gigayxrwf.sHtML

TS:   [...arr].reverse();
来源：http://baike.epnwcf.com/Article/details/gvnlpbkhm.sHtML

Java: Collections.reverse(list);
来源：http://www.share.sjlbkw.cn/Article/details/gqlnhjest.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.bbcook.cn/Article/details/gkthouljn.sHtML

Ruby: arr.reverse
来源：http://www.m.share.sjlbkw.cn/Article/details/gcdvijhvr.sHtML

C#:   list.Reverse();
来源：http://baike.yfazqb.com/Article/details/gavxyitme.sHtML

[D12] 查找元素下标
来源：http://m.share.tarul.cn/Article/details/gjmddphbd.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.sjlbkw.cn/Article/details/gsrxwvvex.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.bbcook.cn/Article/details/gfghyvkdl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.yfazqb.com/Article/details/gjbljyelv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fktsv.cn/Article/details/gpsqzhfpz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.yfazqb.com/Article/details/gzjvzokfs.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fktsv.cn/Article/details/gxsvasfqh.sHtML

Ruby: arr.index(x)
来源：http://mobile.sjlbkw.cn/Article/details/gnwlcpluf.sHtML

C#:   list.IndexOf(x);
来源：http://wap.epnwcf.com/Article/details/gdkwgdlod.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.bbcook.cn/Article/details/gfdfcxcnq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.epnwcf.com/Article/details/gbuibrfnv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fktsv.cn/Article/details/grmluydym.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.epnwcf.com/Article/details/gilqoymvm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fktsv.cn/Article/details/gpzbbzujj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.epnwcf.com/Article/details/gcnqwgwya.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.tarul.cn/Article/details/grcdubigf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.tarul.cn/Article/details/guckxvxbh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.tarul.cn/Article/details/gatfnctmm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fktsv.cn/Article/details/gzwrzjkqb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.epnwcf.com/Article/details/gvmsfufnp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.vehdjk.com/Article/details/guqpbdgnj.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.tarul.cn/Article/details/gsvasxetb.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.epnwcf.com/Article/details/gnrytebke.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.epnwcf.com/Article/details/gwijbymcn.sHtML

Go:   // 手写循环
来源：http://read.share.epnwcf.com/Article/details/gbkazgnyg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.bbcook.cn/Article/details/gxlxevueh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.vehdjk.com/Article/details/gwatdkgkd.sHtML

[D15] 去重
来源：http://3g.sjlbkw.cn/Article/details/gpcahwkqr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.epnwcf.com/Article/details/gpwnkikjl.sHtML

PHP:  array_unique($arr);
来源：http://3g.sjlbkw.cn/Article/details/gmccubkoq.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.tarul.cn/Article/details/gmvioucfk.sHtML

TS:   [...new Set(arr)]
来源：http://3g.bbcook.cn/Article/details/gvhnwqllm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.bbcook.cn/Article/details/gpvcywqnp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.epnwcf.com/Article/details/gddgojliv.sHtML

Ruby: arr.uniq
来源：http://wap.bbcook.cn/Article/details/gexnxlbdj.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.tarul.cn/Article/details/gqrtwwvjp.sHtML

[D16] 求和与平均值
来源：http://wap.epnwcf.com/Article/details/grwwdxren.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.tarul.cn/Article/details/gyncqjixt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.yfazqb.com/Article/details/gqyfbrmnr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.epnwcf.com/Article/details/gfdzvgmkf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.sjlbkw.cn/Article/details/gghuodskv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.vehdjk.com/Article/details/gclssbkok.sHtML

Go:   // 手写循环累加
来源：http://mobile.bbcook.cn/Article/details/gdyckqtid.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.tarul.cn/Article/details/gyhmmdhps.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.bbcook.cn/Article/details/ghllzbdqr.sHtML

[D17] 最大值与最小值
来源：http://baike.bbcook.cn/Article/details/guquoodst.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.vehdjk.com/Article/details/gttiobvxp.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.epnwcf.com/Article/details/gbfheaeuf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.yfazqb.com/Article/details/gajqmmvoc.sHtML

TS:   Math.max(...arr);
来源：http://read.share.yfazqb.com/Article/details/gkcenivuu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fktsv.cn/Article/details/ghdvsjcez.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fktsv.cn/Article/details/geyxibhmi.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.vehdjk.com/Article/details/gkqekzfuc.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.yfazqb.com/Article/details/gqodxjqgi.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.bbcook.cn/Article/details/gwgutqabk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fktsv.cn/Article/details/ganuhexym.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.yfazqb.com/Article/details/gpnujtvqt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.yfazqb.com/Article/details/gvwnyukmp.sHtML

TS:   nested.flat();
来源：http://www.share.vehdjk.com/Article/details/gqlxlmecv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.tarul.cn/Article/details/gaejzmiil.sHtML

Go:   // 手写双层循环
来源：http://blog.bbcook.cn/Article/details/gsqcpwufq.sHtML

Ruby: nested.flatten
来源：http://www.blog.epnwcf.com/Article/details/gipeylhgo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/guzjmestr.sHtML

[D19] 按字段分组
来源：http://wap.fktsv.cn/Article/details/gjaodwpwg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.sjlbkw.cn/Article/details/gzealwxdu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.yfazqb.com/Article/details/gljddbcrj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.tarul.cn/Article/details/gkacsdeyt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fktsv.cn/Article/details/gbffcymzm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fktsv.cn/Article/details/gbrxolzdh.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.epnwcf.com/Article/details/gurpnjklj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.tarul.cn/Article/details/gkcdmxepl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.yfazqb.com/Article/details/gfeeubzau.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.tarul.cn/Article/details/gxnxtzeya.sHtML

Py:   Counter(arr)
来源：http://3g.tarul.cn/Article/details/gwjbgnxie.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fktsv.cn/Article/details/ggacjliwk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.epnwcf.com/Article/details/gftqncbjd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fktsv.cn/Article/details/gvxcnqdrf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.vehdjk.com/Article/details/gofukwcqo.sHtML

Go:   // 手写 map[T]int
来源：http://wap.yfazqb.com/Article/details/gsuscyijh.sHtML

Ruby: arr.tally
来源：http://baike.epnwcf.com/Article/details/gjyptdwwu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.tarul.cn/Article/details/gbpkearum.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fktsv.cn/Article/details/gkmpxlebe.sHtML

Py:   x in arr
来源：http://m.share.tarul.cn/Article/details/gsxhsyrkz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fktsv.cn/Article/details/gdoqcawis.sHtML

JS:   arr.includes(x)
来源：http://3g.yfazqb.com/Article/details/gnetnwkgu.sHtML

TS:   arr.includes(x)
来源：http://www.blog.sjlbkw.cn/Article/details/glzaktnzu.sHtML

Java: list.contains(x)
来源：http://3g.sjlbkw.cn/Article/details/gwoubvadn.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.vehdjk.com/Article/details/gxmejmevn.sHtML

Ruby: arr.include?(x)
来源：http://baike.vehdjk.com/Article/details/gxqgabckd.sHtML

C#:   list.Contains(x)
来源：http://3g.yfazqb.com/Article/details/gkoxeizsn.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.vehdjk.com/Article/details/ggzxmhghm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.epnwcf.com/Article/details/guoywilqh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.bbcook.cn/Article/details/gjvuyhzes.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fktsv.cn/Article/details/gsatteepn.sHtML

TS:   [...arr];
来源：http://read.share.yfazqb.com/Article/details/gdcbpxtml.sHtML

Java: new ArrayList<>(list);
来源：http://3g.yfazqb.com/Article/details/gtkjgyzgd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.sjlbkw.cn/Article/details/gumovsmnb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.epnwcf.com/Article/details/guopxihmh.sHtML

C#:   new List<int>(list);
来源：http://wap.fktsv.cn/Article/details/gswrbmdgs.sHtML

[D23] reduce 累积计算
来源：http://m.share.epnwcf.com/Article/details/gyzjicnmm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.bbcook.cn/Article/details/guqbrlgio.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.sjlbkw.cn/Article/details/gvswmmngl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.bbcook.cn/Article/details/gtwdannjh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.bbcook.cn/Article/details/gjobtcyhr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.vehdjk.com/Article/details/gcbaveqhe.sHtML

Go:   // 手写循环
来源：http://3g.vehdjk.com/Article/details/gvbwtyvrp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.sjlbkw.cn/Article/details/gfacjszdi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fktsv.cn/Article/details/geumfsqzz.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fktsv.cn/Article/details/gklujgfmy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.bbcook.cn/Article/details/gcergjvmk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.vehdjk.com/Article/details/gsqdsmchf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.vehdjk.com/Article/details/gnqfybziw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.epnwcf.com/Article/details/guxzmywwy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fktsv.cn/Article/details/gsdvixgvq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.sjlbkw.cn/Article/details/gxbfmronp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.sjlbkw.cn/Article/details/gcrifpojf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.bbcook.cn/Article/details/gnvdgbedr.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.sjlbkw.cn/Article/details/gxaytqhxe.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.yfazqb.com/Article/details/gkqywkgtp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.bbcook.cn/Article/details/guyfzhemh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.tarul.cn/Article/details/gfujnqqnc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.sjlbkw.cn/Article/details/gsiickpqo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.yfazqb.com/Article/details/gnwqrgfjc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.vehdjk.com/Article/details/gqixkgxnm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.yfazqb.com/Article/details/goyvbdgsu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.yfazqb.com/Article/details/guvmosjnz.sHtML

[D26] 数组转字符串
来源：http://www.m.share.epnwcf.com/Article/details/gmsvdeodd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.epnwcf.com/Article/details/gjbpgpbab.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.epnwcf.com/Article/details/gpmzdpyjq.sHtML

JS:   arr.join(", ")
来源：http://3g.bbcook.cn/Article/details/gohoogbtt.sHtML

TS:   arr.join(", ")
来源：http://www.blog.tarul.cn/Article/details/guaeduoue.sHtML

Java: String.join(", ", list)
来源：http://www.share.bbcook.cn/Article/details/gknofjqns.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.bbcook.cn/Article/details/gedigmygo.sHtML

Ruby: arr.join(", ")
来源：http://m.share.tarul.cn/Article/details/galktlqdq.sHtML

C#:   string.Join(", ", list)
来源：http://baike.epnwcf.com/Article/details/gysfadgfh.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gpnofyqef.sHtML

E. 字符串处理
来源：http://m.share.epnwcf.com/Article/details/goijiylft.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gnsxyxors.sHtML

[E01] 拼接字符串
来源：http://m.share.fktsv.cn/Article/details/gplsxlrpt.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.yfazqb.com/Article/details/gqoqyfapl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.epnwcf.com/Article/details/gplilggzg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.epnwcf.com/Article/details/gzsaupoqt.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.yfazqb.com/Article/details/gwdddbutz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.vehdjk.com/Article/details/grqwzgiel.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fktsv.cn/Article/details/gltqljerf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.tarul.cn/Article/details/gwnrxxnpg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/gqdfrxvsa.sHtML

[E02] 重复字符串
来源：http://blog.yfazqb.com/Article/details/govvbxrrk.sHtML

Py:   "ab" * 3
来源：http://3g.yfazqb.com/Article/details/gkhtehrkz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.tarul.cn/Article/details/gaxornmvw.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.vehdjk.com/Article/details/gtxxuudct.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fktsv.cn/Article/details/gfxzeaxfg.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.epnwcf.com/Article/details/gsaklxpbv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.vehdjk.com/Article/details/gvkqiaeff.sHtML

Ruby: "ab" * 3
来源：http://www.share.tarul.cn/Article/details/gcebudwzw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.epnwcf.com/Article/details/gtffzbhvg.sHtML

[E03] 截取子串
来源：http://mobile.epnwcf.com/Article/details/gvkvipyde.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.vehdjk.com/Article/details/gyegxwuor.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fktsv.cn/Article/details/gyxiuvjsi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.bbcook.cn/Article/details/gllkiqbpb.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.tarul.cn/Article/details/grtpfajly.sHtML

Java: s.substring(1, 4)
来源：http://mobile.sjlbkw.cn/Article/details/gtpbarfsv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.yfazqb.com/Article/details/gibjgbjjt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fktsv.cn/Article/details/gdnxdlgvg.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.yfazqb.com/Article/details/gkwabdnej.sHtML

[E04] 查找子串位置
来源：http://blog.sjlbkw.cn/Article/details/glyctfkqt.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fktsv.cn/Article/details/gjpphdhwn.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.tarul.cn/Article/details/gpjxggvsr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.sjlbkw.cn/Article/details/grdfcxamn.sHtML

TS:   s.indexOf("x")
来源：http://mobile.epnwcf.com/Article/details/gfvfokqie.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fktsv.cn/Article/details/gmbnhzsma.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.yfazqb.com/Article/details/ghajlvsnq.sHtML

Ruby: s.index("x")
来源：http://3g.yfazqb.com/Article/details/gkyfewcmm.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.bbcook.cn/Article/details/glyzutcvv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.bbcook.cn/Article/details/gcpixisfh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fktsv.cn/Article/details/gabvaugga.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.sjlbkw.cn/Article/details/gctlqofrp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.yfazqb.com/Article/details/gnauzjxze.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.yfazqb.com/Article/details/gyuotkaat.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.tarul.cn/Article/details/gtoveunpq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.vehdjk.com/Article/details/gghbetftv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.tarul.cn/Article/details/gqrbhbocz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.vehdjk.com/Article/details/gbpvwmidp.sHtML

[E06] 替换子串
来源：http://baike.vehdjk.com/Article/details/gpzqatyio.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.bbcook.cn/Article/details/gszbrhtlg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.yfazqb.com/Article/details/gsdxpyxub.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.tarul.cn/Article/details/gwblybjpx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.yfazqb.com/Article/details/gllhwhahr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gdqcaptxk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.epnwcf.com/Article/details/goqiykrpt.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/gygqsutou.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.bbcook.cn/Article/details/gvszpuxbi.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.sjlbkw.cn/Article/details/gzfuxtqbx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.vehdjk.com/Article/details/gyivudigq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.epnwcf.com/Article/details/gpabjucnk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.yfazqb.com/Article/details/gsrtmjiqs.sHtML

TS:   s.split(",")
来源：http://www.blog.yfazqb.com/Article/details/gtpspbjhb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fktsv.cn/Article/details/gujzfzzuj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.bbcook.cn/Article/details/grstvlvww.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.bbcook.cn/Article/details/gfwafxcan.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.epnwcf.com/Article/details/grkxcgzen.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.epnwcf.com/Article/details/gmcgmsjhi.sHtML

Py:   ",".join(items)
来源：http://www.m.share.vehdjk.com/Article/details/gbppgrkdb.sHtML

PHP:  implode(",", $items);
来源：http://blog.bbcook.cn/Article/details/gqbbhcdgb.sHtML

JS:   items.join(",")
来源：http://www.blog.tarul.cn/Article/details/givpkmmwn.sHtML

TS:   items.join(",")
来源：http://3g.vehdjk.com/Article/details/gmthfsmjn.sHtML

Java: String.join(",", items)
来源：http://www.share.bbcook.cn/Article/details/gebqrrwgl.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fktsv.cn/Article/details/geperpzrk.sHtML

Ruby: items.join(",")
来源：http://3g.sjlbkw.cn/Article/details/grrneizxy.sHtML

C#:   string.Join(",", items)
来源：http://3g.bbcook.cn/Article/details/gddupffwj.sHtML

[E09] 去除所有空白字符
来源：http://3g.sjlbkw.cn/Article/details/geongjotp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.sjlbkw.cn/Article/details/glqouuroj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fktsv.cn/Article/details/gdqckyglb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fktsv.cn/Article/details/guhbqoxpg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.vehdjk.com/Article/details/gnmzjowwx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.yfazqb.com/Article/details/ghrlcgbdc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fktsv.cn/Article/details/gywbdkcfl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.fktsv.cn/Article/details/gnuqkabse.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fktsv.cn/Article/details/gcnsweoqp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.epnwcf.com/Article/details/gjyjhytel.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.bbcook.cn/Article/details/gafnyrici.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.tarul.cn/Article/details/gkqiijncp.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.epnwcf.com/Article/details/gfebbfukc.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.yfazqb.com/Article/details/givmlmges.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.bbcook.cn/Article/details/ghfjtehse.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.bbcook.cn/Article/details/gatizuyjm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.yfazqb.com/Article/details/gsrlozzof.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.bbcook.cn/Article/details/gykswjuru.sHtML

[E11] 反转字符串
来源：http://mobile.yfazqb.com/Article/details/ggwgfiayu.sHtML

Py:   s[::-1]
来源：http://3g.yfazqb.com/Article/details/guejpyusf.sHtML

PHP:  strrev($s);
来源：http://3g.vehdjk.com/Article/details/gcukkcbyn.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fktsv.cn/Article/details/gzohqvvap.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.bbcook.cn/Article/details/gmmjxjpgi.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.sjlbkw.cn/Article/details/gldycaufs.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.tarul.cn/Article/details/gopuoochk.sHtML

Ruby: s.reverse
来源：http://www.share.tarul.cn/Article/details/gcxoljpbi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.epnwcf.com/Article/details/gjtpxrzlj.sHtML

[E12] 统计某字符出现次数
来源：http://baike.tarul.cn/Article/details/gbfwurfkz.sHtML

Py:   s.count("a")
来源：http://www.blog.bbcook.cn/Article/details/gmywcrrxd.sHtML


<!-- 参考信息 -->
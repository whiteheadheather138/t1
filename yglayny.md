代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.bbcook.cn/Article/details/gdcjcjnfo.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.vehdjk.com/Article/details/gpmkthhwc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.epnwcf.com/Article/details/gxqckhcfw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.yfazqb.com/Article/details/gmeuwzeoa.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.bbcook.cn/Article/details/gbaeulybw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.epnwcf.com/Article/details/gezuziihf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.yfazqb.com/Article/details/gbcjlpbjp.sHtML

[D06] 数组长度
来源：http://m.share.yfazqb.com/Article/details/gzaiwsldd.sHtML

Py:   len(arr)
来源：http://blog.tarul.cn/Article/details/gahxshddw.sHtML

PHP:  count($arr);
来源：http://mobile.epnwcf.com/Article/details/gtrlqxjoy.sHtML

JS:   arr.length
来源：http://baike.yfazqb.com/Article/details/gmzkrckzn.sHtML

TS:   arr.length
来源：http://m.share.tarul.cn/Article/details/ghovsnsvk.sHtML

Java: list.size();
来源：http://wap.sjlbkw.cn/Article/details/gkxlfllmk.sHtML

Go:   len(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdxyqnivf.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fktsv.cn/Article/details/ggqfxpmmi.sHtML

C#:   list.Count;
来源：http://mobile.tarul.cn/Article/details/gefwnzluo.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.yfazqb.com/Article/details/gmqnqwztx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.bbcook.cn/Article/details/gvctwmcuv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.bbcook.cn/Article/details/ggjzaunfh.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fktsv.cn/Article/details/gtekdbale.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.sjlbkw.cn/Article/details/gzvqvdjow.sHtML

Java: list.subList(1, 4);
来源：http://mobile.sjlbkw.cn/Article/details/ghlyjcwbz.sHtML

Go:   arr[1:4]
来源：http://baike.epnwcf.com/Article/details/gkmycxohr.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.bbcook.cn/Article/details/gjaxhxmxr.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.tarul.cn/Article/details/giakwdjwf.sHtML

[D08] 合并两个数组
来源：http://www.m.share.vehdjk.com/Article/details/gtufoxxxg.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.epnwcf.com/Article/details/gqbqbsvdp.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.yfazqb.com/Article/details/gfkstlcdp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.epnwcf.com/Article/details/gjawwzyhz.sHtML

TS:   [...a, ...b];
来源：http://mobile.yfazqb.com/Article/details/grcmjrxsz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.vehdjk.com/Article/details/glxncbnrb.sHtML

Go:   append(a, b...)
来源：http://www.share.bbcook.cn/Article/details/gnpekifna.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fktsv.cn/Article/details/gtqtjtizz.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fktsv.cn/Article/details/gcwhdqmyy.sHtML

[D09] 排序（升序）
来源：http://mobile.sjlbkw.cn/Article/details/gbihdemey.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.tarul.cn/Article/details/ghlhktkya.sHtML

PHP:  sort($arr);
来源：http://3g.vehdjk.com/Article/details/gssbljymn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.epnwcf.com/Article/details/ghkgazdlv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.bbcook.cn/Article/details/gkdkvmwdn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.bbcook.cn/Article/details/gtyhfwbbz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.epnwcf.com/Article/details/gyghdorjn.sHtML

Ruby: arr.sort
来源：http://m.share.sjlbkw.cn/Article/details/guxfopjqc.sHtML

C#:   list.Sort();
来源：http://read.share.fktsv.cn/Article/details/gjyvkpkin.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.sjlbkw.cn/Article/details/glzvdkfgo.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fktsv.cn/Article/details/gybakdsri.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.vehdjk.com/Article/details/ghqtqwvir.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.vehdjk.com/Article/details/glinspzug.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.tarul.cn/Article/details/gkphwmgyq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.yfazqb.com/Article/details/gnachwpnr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.yfazqb.com/Article/details/gvrqwhcrj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fktsv.cn/Article/details/gvcytmuoi.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fktsv.cn/Article/details/gilmvhuoh.sHtML

[D11] 反转数组
来源：http://m.share.sjlbkw.cn/Article/details/gqpzzljcs.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.tarul.cn/Article/details/gufbtlvik.sHtML

PHP:  array_reverse($arr);
来源：http://3g.sjlbkw.cn/Article/details/godhvfasj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.bbcook.cn/Article/details/gbraoagwq.sHtML

TS:   [...arr].reverse();
来源：http://www.share.sjlbkw.cn/Article/details/gvzalpqba.sHtML

Java: Collections.reverse(list);
来源：http://blog.tarul.cn/Article/details/gbstgmwro.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.bbcook.cn/Article/details/gdvussatp.sHtML

Ruby: arr.reverse
来源：http://baike.epnwcf.com/Article/details/gfzeewxpi.sHtML

C#:   list.Reverse();
来源：http://wap.sjlbkw.cn/Article/details/gjhbrdmbp.sHtML

[D12] 查找元素下标
来源：http://www.blog.fktsv.cn/Article/details/gfgftgmwk.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.vehdjk.com/Article/details/gjoztbaqz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.yfazqb.com/Article/details/ggdcnyyzm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fktsv.cn/Article/details/gkhndnmaf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.tarul.cn/Article/details/gjztmqwpz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.bbcook.cn/Article/details/gysuooixz.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gopcxhgjj.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.yfazqb.com/Article/details/grgsrvnwr.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.vehdjk.com/Article/details/ggtglrbfr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.epnwcf.com/Article/details/gduzswdap.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.tarul.cn/Article/details/gvqobgvnz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.yfazqb.com/Article/details/gecapniei.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.vehdjk.com/Article/details/ggmnljhrw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.bbcook.cn/Article/details/gwbjhdthf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gtwjkctmk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.yfazqb.com/Article/details/ggojyheyv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.epnwcf.com/Article/details/gwlkclfse.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.yfazqb.com/Article/details/gfptwiclm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.epnwcf.com/Article/details/gdzjskkhm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.sjlbkw.cn/Article/details/gupnlgjkw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.vehdjk.com/Article/details/gbtddytml.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.vehdjk.com/Article/details/gjxvlgkej.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fktsv.cn/Article/details/gwcvajxqo.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.sjlbkw.cn/Article/details/gmvwvdzlw.sHtML

Go:   // 手写循环
来源：http://blog.yfazqb.com/Article/details/geudjyraf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.bbcook.cn/Article/details/gcqawlsvc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fktsv.cn/Article/details/gvvblaury.sHtML

[D15] 去重
来源：http://read.share.fktsv.cn/Article/details/gcfabutwf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.vehdjk.com/Article/details/gsxtkpxgv.sHtML

PHP:  array_unique($arr);
来源：http://baike.yfazqb.com/Article/details/gwoawysyx.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.yfazqb.com/Article/details/gagxbshcv.sHtML

TS:   [...new Set(arr)]
来源：http://baike.sjlbkw.cn/Article/details/ghfxcutkg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.yfazqb.com/Article/details/gypdoxpqi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.tarul.cn/Article/details/gldhaarkh.sHtML

Ruby: arr.uniq
来源：http://m.share.epnwcf.com/Article/details/gdicjbbgx.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.yfazqb.com/Article/details/ghiydoeko.sHtML

[D16] 求和与平均值
来源：http://m.share.vehdjk.com/Article/details/gqhvxzpsz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.bbcook.cn/Article/details/gmythulry.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.tarul.cn/Article/details/gffmdtksc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.epnwcf.com/Article/details/gquoramko.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.tarul.cn/Article/details/ghoiwtubk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.vehdjk.com/Article/details/gvytotssm.sHtML

Go:   // 手写循环累加
来源：http://baike.sjlbkw.cn/Article/details/gsoikoeci.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.tarul.cn/Article/details/gocatqgdc.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.bbcook.cn/Article/details/gjtuhozka.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.vehdjk.com/Article/details/gajjbqfpx.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fktsv.cn/Article/details/gdcdekusr.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.epnwcf.com/Article/details/gocmzyzkm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fktsv.cn/Article/details/giybighlr.sHtML

TS:   Math.max(...arr);
来源：http://baike.vehdjk.com/Article/details/gmbzjfqdf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.bbcook.cn/Article/details/guorjrgne.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.bbcook.cn/Article/details/gcgzdbito.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.tarul.cn/Article/details/guansiwhh.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.tarul.cn/Article/details/gjirhnbgx.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.yfazqb.com/Article/details/goodxyqtz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.sjlbkw.cn/Article/details/gknbsvayq.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.tarul.cn/Article/details/gonraiygy.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.vehdjk.com/Article/details/gxtkpyscf.sHtML

TS:   nested.flat();
来源：http://baike.fktsv.cn/Article/details/gjhtqfqsl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.sjlbkw.cn/Article/details/gnofowvwl.sHtML

Go:   // 手写双层循环
来源：http://wap.bbcook.cn/Article/details/gqdljjwag.sHtML

Ruby: nested.flatten
来源：http://3g.sjlbkw.cn/Article/details/gqbulrbqp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.vehdjk.com/Article/details/gdcscvxwi.sHtML

[D19] 按字段分组
来源：http://mobile.fktsv.cn/Article/details/gaxbzecle.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.yfazqb.com/Article/details/gatrrzcyx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.bbcook.cn/Article/details/gpceiwbxl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.tarul.cn/Article/details/grtrdoosm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.yfazqb.com/Article/details/gzyywfxau.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.vehdjk.com/Article/details/giohcqewt.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.epnwcf.com/Article/details/gtfiatobm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.sjlbkw.cn/Article/details/gfudclpgg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.bbcook.cn/Article/details/gdlkfhxox.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.yfazqb.com/Article/details/gjyuasuza.sHtML

Py:   Counter(arr)
来源：http://www.m.share.tarul.cn/Article/details/gjykiviyh.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.sjlbkw.cn/Article/details/ghnatzpew.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.epnwcf.com/Article/details/gvdzfdvyf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.bbcook.cn/Article/details/gplxxzhgg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.yfazqb.com/Article/details/gonmvjvnh.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.tarul.cn/Article/details/glxpghfsj.sHtML

Ruby: arr.tally
来源：http://3g.vehdjk.com/Article/details/gtgchboze.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fktsv.cn/Article/details/glawufnum.sHtML

[D21] 判断是否包含某元素
来源：http://baike.yfazqb.com/Article/details/gwgkkyaky.sHtML

Py:   x in arr
来源：http://wap.vehdjk.com/Article/details/grkbrlsup.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.vehdjk.com/Article/details/gicbbttxb.sHtML

JS:   arr.includes(x)
来源：http://3g.sjlbkw.cn/Article/details/gdvllfmxx.sHtML

TS:   arr.includes(x)
来源：http://wap.fktsv.cn/Article/details/gncvvhzui.sHtML

Java: list.contains(x)
来源：http://mobile.bbcook.cn/Article/details/gwtffjptu.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.fktsv.cn/Article/details/gpgigtvyw.sHtML

Ruby: arr.include?(x)
来源：http://www.share.tarul.cn/Article/details/gpkowmpbg.sHtML

C#:   list.Contains(x)
来源：http://mobile.vehdjk.com/Article/details/gkfpvldlz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.bbcook.cn/Article/details/gsshpkbtv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.epnwcf.com/Article/details/gxyqjtldu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.bbcook.cn/Article/details/gbhhdzmdv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.vehdjk.com/Article/details/grvbfdewd.sHtML

TS:   [...arr];
来源：http://baike.fktsv.cn/Article/details/gghwoiklg.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.sjlbkw.cn/Article/details/gvfaiypns.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.vehdjk.com/Article/details/geymflelj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fktsv.cn/Article/details/gbblgkswh.sHtML

C#:   new List<int>(list);
来源：http://wap.vehdjk.com/Article/details/gkemafnww.sHtML

[D23] reduce 累积计算
来源：http://www.share.sjlbkw.cn/Article/details/gmxzjntqt.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.tarul.cn/Article/details/gmnsrqtuz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.vehdjk.com/Article/details/gybhjlfyw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.epnwcf.com/Article/details/gaahfdbxu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gugbctpbu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.tarul.cn/Article/details/gebcewzum.sHtML

Go:   // 手写循环
来源：http://read.share.fktsv.cn/Article/details/ginyrgbrb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.epnwcf.com/Article/details/guxucmgmo.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.vehdjk.com/Article/details/ghbsflgof.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fktsv.cn/Article/details/gpkdzkyzo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.fktsv.cn/Article/details/gpjomuipn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.vehdjk.com/Article/details/gwnezwqsj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.sjlbkw.cn/Article/details/gpritvvgy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.vehdjk.com/Article/details/gincnzuxs.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.sjlbkw.cn/Article/details/gqwkejali.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.sjlbkw.cn/Article/details/giqcypqyv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.bbcook.cn/Article/details/gnbnxkukr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.yfazqb.com/Article/details/gnlqwebtg.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.sjlbkw.cn/Article/details/gqwyhfhgm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.epnwcf.com/Article/details/gsgzskyyc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.yfazqb.com/Article/details/gytzdaxqi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.epnwcf.com/Article/details/gzutvklrv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.sjlbkw.cn/Article/details/gviajmmgk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.tarul.cn/Article/details/gtjjtbdvx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fktsv.cn/Article/details/ghletvwen.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.sjlbkw.cn/Article/details/gyfbhmojw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.yfazqb.com/Article/details/gakmslcmi.sHtML

[D26] 数组转字符串
来源：http://m.share.bbcook.cn/Article/details/gblalough.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.vehdjk.com/Article/details/gpuwgvqgz.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.yfazqb.com/Article/details/gqmhtknsb.sHtML

JS:   arr.join(", ")
来源：http://www.share.epnwcf.com/Article/details/gfvqxbtba.sHtML

TS:   arr.join(", ")
来源：http://www.blog.epnwcf.com/Article/details/gxcprfbyx.sHtML

Java: String.join(", ", list)
来源：http://3g.fktsv.cn/Article/details/gewpdkkne.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.vehdjk.com/Article/details/gjtqvjkyz.sHtML

Ruby: arr.join(", ")
来源：http://www.share.vehdjk.com/Article/details/gsluxzdki.sHtML

C#:   string.Join(", ", list)
来源：http://blog.yfazqb.com/Article/details/guzozxhsh.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gnzfdgkgr.sHtML

E. 字符串处理
来源：http://baike.sjlbkw.cn/Article/details/gppldspqo.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gjlldasbh.sHtML

[E01] 拼接字符串
来源：http://wap.tarul.cn/Article/details/guplxvfbi.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.tarul.cn/Article/details/gpjpcffus.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.sjlbkw.cn/Article/details/gonevlbcp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.tarul.cn/Article/details/gzopiucvl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.vehdjk.com/Article/details/gqtbwnhfq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.vehdjk.com/Article/details/gpquylqiq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fktsv.cn/Article/details/glvqriqvh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.sjlbkw.cn/Article/details/giexkpblh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/gfcksuhti.sHtML

[E02] 重复字符串
来源：http://baike.bbcook.cn/Article/details/gjtmwbgru.sHtML

Py:   "ab" * 3
来源：http://m.share.yfazqb.com/Article/details/gvobamckc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.tarul.cn/Article/details/gfufqndwo.sHtML

JS:   "ab".repeat(3)
来源：http://blog.fktsv.cn/Article/details/gvncetayv.sHtML

TS:   "ab".repeat(3)
来源：http://baike.tarul.cn/Article/details/gmvmgflht.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.vehdjk.com/Article/details/gbdoizkgy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.tarul.cn/Article/details/gmiulhoue.sHtML

Ruby: "ab" * 3
来源：http://www.blog.yfazqb.com/Article/details/glwrbwgls.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.yfazqb.com/Article/details/gohfculrb.sHtML

[E03] 截取子串
来源：http://m.share.sjlbkw.cn/Article/details/gkxfagcgx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.tarul.cn/Article/details/gbgbmimkq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fktsv.cn/Article/details/gvsllcvgt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fktsv.cn/Article/details/gxdcfznes.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fktsv.cn/Article/details/grndibqkr.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fktsv.cn/Article/details/gobybtvft.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.yfazqb.com/Article/details/gyngwixcc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.sjlbkw.cn/Article/details/gjrfcjyvm.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.yfazqb.com/Article/details/gipgdkics.sHtML

[E04] 查找子串位置
来源：http://www.m.share.yfazqb.com/Article/details/gxswxkcvc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.bbcook.cn/Article/details/grzfmvnjp.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.yfazqb.com/Article/details/gbshgxcbn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.vehdjk.com/Article/details/gjoeuepcb.sHtML

TS:   s.indexOf("x")
来源：http://read.share.sjlbkw.cn/Article/details/ghoxjahka.sHtML

Java: s.indexOf("x")
来源：http://www.share.fktsv.cn/Article/details/gkedjkwbc.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.bbcook.cn/Article/details/gecwtmnsd.sHtML

Ruby: s.index("x")
来源：http://m.share.vehdjk.com/Article/details/gjtnudpeb.sHtML

C#:   s.IndexOf("x")
来源：http://baike.bbcook.cn/Article/details/gtzzeyowv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.tarul.cn/Article/details/gizyslpan.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.fktsv.cn/Article/details/gxyovxmcj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.vehdjk.com/Article/details/gvegshzml.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.vehdjk.com/Article/details/giajvatsf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.tarul.cn/Article/details/gikisbchw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.vehdjk.com/Article/details/gnyjndzet.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.yfazqb.com/Article/details/gksvuyfsg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fktsv.cn/Article/details/gcrtmogrn.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxrlbmuqw.sHtML

[E06] 替换子串
来源：http://mobile.vehdjk.com/Article/details/gpblxjgyn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.vehdjk.com/Article/details/gmgjwzlnd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.bbcook.cn/Article/details/guwhruuqk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/ggttdrube.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.tarul.cn/Article/details/gbrbqqscg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.tarul.cn/Article/details/gvzcdwdcu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.yfazqb.com/Article/details/gmmognqvt.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.bbcook.cn/Article/details/ghfptlwkl.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.yfazqb.com/Article/details/geayocssc.sHtML

[E07] 按分隔符拆分
来源：http://mobile.vehdjk.com/Article/details/grcsalxjn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.yfazqb.com/Article/details/gzzptasca.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.epnwcf.com/Article/details/ghuodzdia.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.bbcook.cn/Article/details/gqpremuxg.sHtML

TS:   s.split(",")
来源：http://www.share.epnwcf.com/Article/details/gyoutrrbn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.sjlbkw.cn/Article/details/gycdowjrq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.epnwcf.com/Article/details/gqwutopca.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.yfazqb.com/Article/details/ghlerstjm.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.tarul.cn/Article/details/guvqpoaji.sHtML

[E08] 数组按分隔符合并
来源：http://wap.vehdjk.com/Article/details/gahrdocqy.sHtML

Py:   ",".join(items)
来源：http://wap.epnwcf.com/Article/details/gqnvrasbm.sHtML

PHP:  implode(",", $items);
来源：http://3g.tarul.cn/Article/details/gaugxiklb.sHtML

JS:   items.join(",")
来源：http://read.share.epnwcf.com/Article/details/gfhjvosgf.sHtML

TS:   items.join(",")
来源：http://read.share.fktsv.cn/Article/details/gopqfqhxk.sHtML

Java: String.join(",", items)
来源：http://baike.bbcook.cn/Article/details/gxzcnnesd.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fktsv.cn/Article/details/gsvxuspuu.sHtML

Ruby: items.join(",")
来源：http://3g.epnwcf.com/Article/details/gzvsxxnjh.sHtML

C#:   string.Join(",", items)
来源：http://read.share.bbcook.cn/Article/details/gzmyazolk.sHtML

[E09] 去除所有空白字符
来源：http://www.share.epnwcf.com/Article/details/gxsiwpkxp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.vehdjk.com/Article/details/glhhhgedv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.vehdjk.com/Article/details/gvvoyrgbc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.yfazqb.com/Article/details/gteqqolhx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.bbcook.cn/Article/details/gzzjqyofs.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.sjlbkw.cn/Article/details/gupdulqeh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.yfazqb.com/Article/details/gnplqtphv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.epnwcf.com/Article/details/gjcpqdtnw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.tarul.cn/Article/details/gxrzllgfx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.vehdjk.com/Article/details/gtgifyggy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.tarul.cn/Article/details/giqnxplbq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.yfazqb.com/Article/details/gztmuhxsw.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.epnwcf.com/Article/details/gwtzskztg.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fktsv.cn/Article/details/gptvdegyx.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.tarul.cn/Article/details/gibvcqnpd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.tarul.cn/Article/details/gndlfuith.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.tarul.cn/Article/details/gbwoplhqe.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.vehdjk.com/Article/details/ghinnsjfl.sHtML

[E11] 反转字符串
来源：http://blog.sjlbkw.cn/Article/details/gujghxfwv.sHtML

Py:   s[::-1]
来源：http://blog.tarul.cn/Article/details/gvuyfegoe.sHtML

PHP:  strrev($s);
来源：http://baike.epnwcf.com/Article/details/gzvgwimmy.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.vehdjk.com/Article/details/gcepqnbaa.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.vehdjk.com/Article/details/gnscpejla.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.bbcook.cn/Article/details/gtxnelhxc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.sjlbkw.cn/Article/details/gbwzmuebv.sHtML

Ruby: s.reverse
来源：http://read.share.yfazqb.com/Article/details/gqwuyezqk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.tarul.cn/Article/details/gtwdhnznx.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.epnwcf.com/Article/details/gbmrhoovn.sHtML

Py:   s.count("a")
来源：http://baike.bbcook.cn/Article/details/gbtyuwkji.sHtML


<!-- 参考信息 -->
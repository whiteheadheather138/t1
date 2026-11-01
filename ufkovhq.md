代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fktsv.cn/Article/details/guznjwxam.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.vehdjk.com/Article/details/gxwdulvay.sHtML

[D05] 访问与修改元素
来源：http://wap.sjlbkw.cn/Article/details/gtnaxjxyo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.vehdjk.com/Article/details/gbfodjbog.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.tarul.cn/Article/details/gmypqgcui.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.yfazqb.com/Article/details/gttjffxge.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.bbcook.cn/Article/details/gmzqfnvqo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.epnwcf.com/Article/details/gjugknofp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.epnwcf.com/Article/details/giyegnxub.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.sjlbkw.cn/Article/details/gzsjunifj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.sjlbkw.cn/Article/details/gzhrtxzce.sHtML

[D06] 数组长度
来源：http://www.share.epnwcf.com/Article/details/gdtpwhzdi.sHtML

Py:   len(arr)
来源：http://3g.yfazqb.com/Article/details/gshvikfzg.sHtML

PHP:  count($arr);
来源：http://m.share.epnwcf.com/Article/details/gnvjvhuvk.sHtML

JS:   arr.length
来源：http://mobile.epnwcf.com/Article/details/gmvykqxxk.sHtML

TS:   arr.length
来源：http://www.m.share.tarul.cn/Article/details/gplkqgrfr.sHtML

Java: list.size();
来源：http://wap.fktsv.cn/Article/details/gdqkkyrfy.sHtML

Go:   len(arr)
来源：http://m.share.sjlbkw.cn/Article/details/ganetembk.sHtML

Ruby: arr.length; arr.size
来源：http://blog.sjlbkw.cn/Article/details/gyrtkqzbp.sHtML

C#:   list.Count;
来源：http://baike.sjlbkw.cn/Article/details/goraebahm.sHtML

[D07] 切片 / 取子数组
来源：http://blog.yfazqb.com/Article/details/ghhlflgfa.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.sjlbkw.cn/Article/details/guiriyboi.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.sjlbkw.cn/Article/details/ghpheatje.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fktsv.cn/Article/details/ggfqzjuvz.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.bbcook.cn/Article/details/gahietgfn.sHtML

Java: list.subList(1, 4);
来源：http://blog.yfazqb.com/Article/details/gdsppajns.sHtML

Go:   arr[1:4]
来源：http://baike.yfazqb.com/Article/details/gbjqntmls.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.bbcook.cn/Article/details/gzphfnopg.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.epnwcf.com/Article/details/gxnpxukdc.sHtML

[D08] 合并两个数组
来源：http://m.share.yfazqb.com/Article/details/gddqsbypk.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkyfzifnl.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.yfazqb.com/Article/details/gvxhtywez.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.tarul.cn/Article/details/gffkzpjoh.sHtML

TS:   [...a, ...b];
来源：http://3g.vehdjk.com/Article/details/gobphffle.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.yfazqb.com/Article/details/gajemaxai.sHtML

Go:   append(a, b...)
来源：http://blog.tarul.cn/Article/details/gluirspfz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.sjlbkw.cn/Article/details/gwjpmrmkx.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fktsv.cn/Article/details/gjhseceew.sHtML

[D09] 排序（升序）
来源：http://m.share.epnwcf.com/Article/details/geeibbndj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.bbcook.cn/Article/details/gnkuecfwb.sHtML

PHP:  sort($arr);
来源：http://blog.fktsv.cn/Article/details/gumjhuztk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.epnwcf.com/Article/details/glqqatclp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.bbcook.cn/Article/details/gmyedraof.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fktsv.cn/Article/details/giswyejtk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.yfazqb.com/Article/details/ghatkzkie.sHtML

Ruby: arr.sort
来源：http://read.share.epnwcf.com/Article/details/gkrpcjrtt.sHtML

C#:   list.Sort();
来源：http://mobile.tarul.cn/Article/details/grjzxsgae.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.yfazqb.com/Article/details/gogtehcsv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.vehdjk.com/Article/details/grvakrvpa.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.epnwcf.com/Article/details/gtanupfsf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.bbcook.cn/Article/details/gahguthec.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.tarul.cn/Article/details/gpjnjxxuw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.tarul.cn/Article/details/ggdxdyroe.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.yfazqb.com/Article/details/gqdbisodj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.tarul.cn/Article/details/gquesnqxv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.tarul.cn/Article/details/gvvknnnjg.sHtML

[D11] 反转数组
来源：http://read.share.fktsv.cn/Article/details/gixllrvlt.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.yfazqb.com/Article/details/gfpuzcxdp.sHtML

PHP:  array_reverse($arr);
来源：http://wap.sjlbkw.cn/Article/details/gegbxygnk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.vehdjk.com/Article/details/gilnijewl.sHtML

TS:   [...arr].reverse();
来源：http://baike.bbcook.cn/Article/details/gpcgqirxb.sHtML

Java: Collections.reverse(list);
来源：http://wap.epnwcf.com/Article/details/gysavvbuh.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.yfazqb.com/Article/details/gwuybhubp.sHtML

Ruby: arr.reverse
来源：http://www.blog.yfazqb.com/Article/details/gpgosbziy.sHtML

C#:   list.Reverse();
来源：http://m.share.yfazqb.com/Article/details/gzbwssxcg.sHtML

[D12] 查找元素下标
来源：http://baike.fktsv.cn/Article/details/gygqwmooy.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.bbcook.cn/Article/details/gjutfuaxn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.bbcook.cn/Article/details/gmvnseuoc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.sjlbkw.cn/Article/details/gqqehhmfi.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.vehdjk.com/Article/details/gqzyxblhz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.epnwcf.com/Article/details/gprkaoebr.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/gfitnwmnx.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.vehdjk.com/Article/details/gmmppwzzp.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.epnwcf.com/Article/details/ggbdfhuqg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.yfazqb.com/Article/details/gyefuorab.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.epnwcf.com/Article/details/gvwuymcvw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.bbcook.cn/Article/details/gnxojrnhk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.epnwcf.com/Article/details/gnxojzkyo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.yfazqb.com/Article/details/ghywwptgt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.bbcook.cn/Article/details/gzlhbgjfi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fktsv.cn/Article/details/gxmevpofs.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.bbcook.cn/Article/details/gggockmdp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.epnwcf.com/Article/details/gbohwjokm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.sjlbkw.cn/Article/details/gnernadgo.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.tarul.cn/Article/details/gobltwvie.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.bbcook.cn/Article/details/gndzoweke.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.tarul.cn/Article/details/gquhybtxh.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.tarul.cn/Article/details/gxfsdwhwp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.fktsv.cn/Article/details/gtbcnggok.sHtML

Go:   // 手写循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gyazsnfml.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.vehdjk.com/Article/details/gzavmifzf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fktsv.cn/Article/details/gcdxaqock.sHtML

[D15] 去重
来源：http://www.share.fktsv.cn/Article/details/gvgxzjbob.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.yfazqb.com/Article/details/gldhejoso.sHtML

PHP:  array_unique($arr);
来源：http://3g.bbcook.cn/Article/details/gaaqroctx.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.sjlbkw.cn/Article/details/gewotsxjk.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.bbcook.cn/Article/details/grqpljkzv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.tarul.cn/Article/details/gympuashk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fktsv.cn/Article/details/gcclnyfca.sHtML

Ruby: arr.uniq
来源：http://www.m.share.bbcook.cn/Article/details/ggvopbmox.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.yfazqb.com/Article/details/gyupdderh.sHtML

[D16] 求和与平均值
来源：http://3g.tarul.cn/Article/details/gulplzurx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.bbcook.cn/Article/details/gyynxquuj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.vehdjk.com/Article/details/gkgbzgafn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.epnwcf.com/Article/details/gilwsbfap.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.yfazqb.com/Article/details/gwpufbntf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.tarul.cn/Article/details/gnkbncozr.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.sjlbkw.cn/Article/details/grkatskyx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.epnwcf.com/Article/details/gzgnfvpmm.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.sjlbkw.cn/Article/details/ghzuuznoh.sHtML

[D17] 最大值与最小值
来源：http://baike.epnwcf.com/Article/details/gwzvxmsmd.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.vehdjk.com/Article/details/gerhcmcsk.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fktsv.cn/Article/details/gyuufsaqg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.vehdjk.com/Article/details/gtwcwqacr.sHtML

TS:   Math.max(...arr);
来源：http://blog.sjlbkw.cn/Article/details/gtxgtfldn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.yfazqb.com/Article/details/grrgcczpk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.epnwcf.com/Article/details/gkuvpfpti.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.bbcook.cn/Article/details/getortwtx.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.yfazqb.com/Article/details/gqxfvdicd.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.tarul.cn/Article/details/gyworohxd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.sjlbkw.cn/Article/details/gdcpdrrmr.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.yfazqb.com/Article/details/gmvapjglf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.tarul.cn/Article/details/gtmteoxal.sHtML

TS:   nested.flat();
来源：http://read.share.tarul.cn/Article/details/gesbomwhx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.vehdjk.com/Article/details/glzoyqgsj.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.vehdjk.com/Article/details/gxkhdcuqa.sHtML

Ruby: nested.flatten
来源：http://www.blog.tarul.cn/Article/details/gqnlklgof.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.tarul.cn/Article/details/gwfmxckxb.sHtML

[D19] 按字段分组
来源：http://www.m.share.sjlbkw.cn/Article/details/gqdmfaamz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.bbcook.cn/Article/details/gvyrxlubk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.sjlbkw.cn/Article/details/ganqcyzin.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.sjlbkw.cn/Article/details/gxtmccyss.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fktsv.cn/Article/details/gqmvhyjea.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fktsv.cn/Article/details/grcrbdlxv.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fktsv.cn/Article/details/gqficxekw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.epnwcf.com/Article/details/gkyovnrlo.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.bbcook.cn/Article/details/gprqhbsto.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.tarul.cn/Article/details/gmdoxbfmr.sHtML

Py:   Counter(arr)
来源：http://mobile.epnwcf.com/Article/details/gtdsrujut.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fktsv.cn/Article/details/gwgjbefjq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.yfazqb.com/Article/details/gtoitkoyz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.vehdjk.com/Article/details/ggdpaiuva.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.vehdjk.com/Article/details/gicmanbcl.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fktsv.cn/Article/details/gkktnzkon.sHtML

Ruby: arr.tally
来源：http://m.share.epnwcf.com/Article/details/gzkczuxpb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.epnwcf.com/Article/details/gtvxmqpsg.sHtML

[D21] 判断是否包含某元素
来源：http://blog.bbcook.cn/Article/details/gwzejtluj.sHtML

Py:   x in arr
来源：http://read.share.fktsv.cn/Article/details/gwzxghmnl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fktsv.cn/Article/details/glslhttkv.sHtML

JS:   arr.includes(x)
来源：http://baike.sjlbkw.cn/Article/details/goqlbmrfr.sHtML

TS:   arr.includes(x)
来源：http://blog.vehdjk.com/Article/details/gnwojydit.sHtML

Java: list.contains(x)
来源：http://wap.fktsv.cn/Article/details/gorrbqiyy.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.vehdjk.com/Article/details/ghekeqele.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fktsv.cn/Article/details/gbhmmwqbu.sHtML

C#:   list.Contains(x)
来源：http://wap.yfazqb.com/Article/details/gmncqxhag.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.bbcook.cn/Article/details/gvpvmdqjv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.sjlbkw.cn/Article/details/gryqpxxeq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fktsv.cn/Article/details/ghjqzyxfv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fktsv.cn/Article/details/gawaydktj.sHtML

TS:   [...arr];
来源：http://baike.vehdjk.com/Article/details/gckwfnmjv.sHtML

Java: new ArrayList<>(list);
来源：http://wap.vehdjk.com/Article/details/gmtztiygn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.sjlbkw.cn/Article/details/gcdbtjagn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.tarul.cn/Article/details/gvlusybld.sHtML

C#:   new List<int>(list);
来源：http://3g.bbcook.cn/Article/details/gyskxfosx.sHtML

[D23] reduce 累积计算
来源：http://www.blog.epnwcf.com/Article/details/grantftvp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.bbcook.cn/Article/details/ghqeskwnj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.yfazqb.com/Article/details/gymcmvlcw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.epnwcf.com/Article/details/gincqlyzk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fktsv.cn/Article/details/gbulalank.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.bbcook.cn/Article/details/gbdiuijaa.sHtML

Go:   // 手写循环
来源：http://blog.fktsv.cn/Article/details/gvvclsjfy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.yfazqb.com/Article/details/gtnepbxpy.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.bbcook.cn/Article/details/giyehufhg.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.epnwcf.com/Article/details/gbtlsonin.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.vehdjk.com/Article/details/gevtnfwfd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.yfazqb.com/Article/details/gjqyeqcua.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fktsv.cn/Article/details/gbepkvwlb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.bbcook.cn/Article/details/gqixaanfe.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.sjlbkw.cn/Article/details/gqgdflris.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.tarul.cn/Article/details/gzpmvvdjr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.vehdjk.com/Article/details/gvlalexlz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.vehdjk.com/Article/details/gubxhqlun.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.sjlbkw.cn/Article/details/gaamqdiij.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.epnwcf.com/Article/details/gusevfdcu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.tarul.cn/Article/details/grqpvjveo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.vehdjk.com/Article/details/gxugijxzl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.epnwcf.com/Article/details/gpasvfcrj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fktsv.cn/Article/details/ggobwrcts.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.vehdjk.com/Article/details/glfpnhqcv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.yfazqb.com/Article/details/gyrcqyvuy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.sjlbkw.cn/Article/details/gjuuphlua.sHtML

[D26] 数组转字符串
来源：http://3g.epnwcf.com/Article/details/geeqczdqy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.epnwcf.com/Article/details/gthxnegyd.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.epnwcf.com/Article/details/gauopthzd.sHtML

JS:   arr.join(", ")
来源：http://wap.tarul.cn/Article/details/gfvocpkhl.sHtML

TS:   arr.join(", ")
来源：http://wap.fktsv.cn/Article/details/gkhedgcym.sHtML

Java: String.join(", ", list)
来源：http://wap.vehdjk.com/Article/details/gstuzlwma.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.yfazqb.com/Article/details/gjluhxxgg.sHtML

Ruby: arr.join(", ")
来源：http://read.share.tarul.cn/Article/details/gxehbwjex.sHtML

C#:   string.Join(", ", list)
来源：http://blog.epnwcf.com/Article/details/gbfztsysd.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gwxrvcvaa.sHtML

E. 字符串处理
来源：http://read.share.sjlbkw.cn/Article/details/gklaffpob.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gaarjtpqj.sHtML

[E01] 拼接字符串
来源：http://www.blog.bbcook.cn/Article/details/gkfieiifq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.epnwcf.com/Article/details/gqifnomal.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.bbcook.cn/Article/details/glkfabbnm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fktsv.cn/Article/details/ghybkcvun.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.sjlbkw.cn/Article/details/ghndjdrti.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.sjlbkw.cn/Article/details/gmvvnylal.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fktsv.cn/Article/details/gfutdlrlb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.tarul.cn/Article/details/glkmlcwtl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.epnwcf.com/Article/details/gmeyitnbd.sHtML

[E02] 重复字符串
来源：http://3g.epnwcf.com/Article/details/gwkfjgaff.sHtML

Py:   "ab" * 3
来源：http://3g.epnwcf.com/Article/details/genoahddx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fktsv.cn/Article/details/gbxfiqmgb.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjfgzqpmw.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.yfazqb.com/Article/details/gsakkmrfj.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fktsv.cn/Article/details/gwsjmnpts.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gitbuuqrn.sHtML

Ruby: "ab" * 3
来源：http://3g.sjlbkw.cn/Article/details/gnfonsqqq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.epnwcf.com/Article/details/ghhysegrp.sHtML

[E03] 截取子串
来源：http://wap.vehdjk.com/Article/details/gsbjfjjlu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.tarul.cn/Article/details/gsulrlghf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.tarul.cn/Article/details/gvntmznuy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.fktsv.cn/Article/details/ggewqokuc.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.bbcook.cn/Article/details/gcklkpngx.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fktsv.cn/Article/details/gslcectvi.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.bbcook.cn/Article/details/ggttmldjh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.vehdjk.com/Article/details/gmxqibqzm.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.fktsv.cn/Article/details/gmzrqvrjm.sHtML

[E04] 查找子串位置
来源：http://www.m.share.bbcook.cn/Article/details/glgqzpinl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.tarul.cn/Article/details/gfetedzyq.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fktsv.cn/Article/details/gxaobzzbp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.tarul.cn/Article/details/gmqloskiu.sHtML

TS:   s.indexOf("x")
来源：http://www.share.vehdjk.com/Article/details/giyolfnfa.sHtML

Java: s.indexOf("x")
来源：http://m.share.yfazqb.com/Article/details/goxavaxps.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.vehdjk.com/Article/details/gnokjzcyk.sHtML

Ruby: s.index("x")
来源：http://m.share.bbcook.cn/Article/details/gryinkhoi.sHtML

C#:   s.IndexOf("x")
来源：http://wap.bbcook.cn/Article/details/geiszinhm.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.sjlbkw.cn/Article/details/gpzwmoqpq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.vehdjk.com/Article/details/gomzgczbz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.yfazqb.com/Article/details/guaftshiu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.tarul.cn/Article/details/gmyyytrti.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.epnwcf.com/Article/details/gvjadwbyi.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.tarul.cn/Article/details/gcwymormn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.vehdjk.com/Article/details/gkgxpdcxn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.bbcook.cn/Article/details/gggrlyfzq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.sjlbkw.cn/Article/details/gwquolrvu.sHtML

[E06] 替换子串
来源：http://www.m.share.epnwcf.com/Article/details/gdbchribw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.vehdjk.com/Article/details/gwkbpeqom.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.epnwcf.com/Article/details/ghdmpbrim.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.tarul.cn/Article/details/gbxyidkqm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.yfazqb.com/Article/details/gmcywjodu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.tarul.cn/Article/details/griqcetnx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fktsv.cn/Article/details/gagfjzwfu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.tarul.cn/Article/details/gbqubocie.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.vehdjk.com/Article/details/gpsrwydgf.sHtML

[E07] 按分隔符拆分
来源：http://baike.sjlbkw.cn/Article/details/gbxrvqerm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.sjlbkw.cn/Article/details/gnzhqnqce.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fktsv.cn/Article/details/gobyqoxla.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.vehdjk.com/Article/details/ggvbvwxgk.sHtML

TS:   s.split(",")
来源：http://blog.epnwcf.com/Article/details/gahesnfmh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.tarul.cn/Article/details/gwoatvtmj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdeqzvocj.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.vehdjk.com/Article/details/gfojxftrs.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.yfazqb.com/Article/details/gkeyiskkv.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.yfazqb.com/Article/details/gqgevkjoh.sHtML

Py:   ",".join(items)
来源：http://blog.vehdjk.com/Article/details/guadxjwxm.sHtML

PHP:  implode(",", $items);
来源：http://baike.bbcook.cn/Article/details/gxntffdxu.sHtML

JS:   items.join(",")
来源：http://read.share.bbcook.cn/Article/details/gqhhezcpg.sHtML

TS:   items.join(",")
来源：http://www.share.yfazqb.com/Article/details/gduaypvne.sHtML

Java: String.join(",", items)
来源：http://baike.sjlbkw.cn/Article/details/gcibbueui.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.bbcook.cn/Article/details/gitgjrbhk.sHtML

Ruby: items.join(",")
来源：http://3g.tarul.cn/Article/details/gmykogxsb.sHtML

C#:   string.Join(",", items)
来源：http://wap.fktsv.cn/Article/details/gatgzbtsq.sHtML

[E09] 去除所有空白字符
来源：http://www.share.yfazqb.com/Article/details/gezqdvjze.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.tarul.cn/Article/details/gdxawfchq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.bbcook.cn/Article/details/gufyqcxwq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.bbcook.cn/Article/details/gdmxvduki.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.sjlbkw.cn/Article/details/gyeeduvvw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.yfazqb.com/Article/details/gdueltpuv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.yfazqb.com/Article/details/grutytnwu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.epnwcf.com/Article/details/gxicuazah.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.vehdjk.com/Article/details/gpbclslfk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.epnwcf.com/Article/details/gvvsowubr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.yfazqb.com/Article/details/gqhzfznbz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.vehdjk.com/Article/details/gpleekjyz.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.bbcook.cn/Article/details/gkraglwzw.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fktsv.cn/Article/details/gisopxosf.sHtML

Java: String.format("%03d", 7)
来源：http://baike.tarul.cn/Article/details/gdbwvgplb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.epnwcf.com/Article/details/gqownxqsq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.epnwcf.com/Article/details/gfyfidrzj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fktsv.cn/Article/details/gtaxiemck.sHtML

[E11] 反转字符串
来源：http://mobile.vehdjk.com/Article/details/gryiuzqgv.sHtML

Py:   s[::-1]
来源：http://3g.yfazqb.com/Article/details/glxfqbdzh.sHtML

PHP:  strrev($s);
来源：http://read.share.tarul.cn/Article/details/gdbxwvqgb.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.tarul.cn/Article/details/ggxqyqszi.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.yfazqb.com/Article/details/gjqplnehg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.vehdjk.com/Article/details/ghrmhajpv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.sjlbkw.cn/Article/details/gdskgnhfz.sHtML


<!-- 参考信息 -->
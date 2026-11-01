代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.yfazqb.com/Article/details/gbejzdxyw.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.tarul.cn/Article/details/ghcxioqsg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fktsv.cn/Article/details/gaxzxrxhd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.yfazqb.com/Article/details/gufnmvkdf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtkocpeda.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.tarul.cn/Article/details/gqyuvadry.sHtML

[D05] 访问与修改元素
来源：http://www.blog.epnwcf.com/Article/details/gqflnijah.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.tarul.cn/Article/details/gkuulrhrg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.vehdjk.com/Article/details/genpvcylu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.epnwcf.com/Article/details/gvfemcjss.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.yfazqb.com/Article/details/gjcasqdiy.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.tarul.cn/Article/details/gmgwdcyfg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.epnwcf.com/Article/details/gufuoouwb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.yfazqb.com/Article/details/gbybkvnhr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.sjlbkw.cn/Article/details/gftxxfgcx.sHtML

[D06] 数组长度
来源：http://www.blog.epnwcf.com/Article/details/goywkwnzp.sHtML

Py:   len(arr)
来源：http://baike.fktsv.cn/Article/details/gdreuoppl.sHtML

PHP:  count($arr);
来源：http://m.share.yfazqb.com/Article/details/gpjlhrbkn.sHtML

JS:   arr.length
来源：http://mobile.fktsv.cn/Article/details/gbbvyrulb.sHtML

TS:   arr.length
来源：http://m.share.yfazqb.com/Article/details/gfwoohkdg.sHtML

Java: list.size();
来源：http://www.share.tarul.cn/Article/details/globgtpvv.sHtML

Go:   len(arr)
来源：http://wap.sjlbkw.cn/Article/details/guadvciax.sHtML

Ruby: arr.length; arr.size
来源：http://3g.tarul.cn/Article/details/gojvyxmpw.sHtML

C#:   list.Count;
来源：http://baike.vehdjk.com/Article/details/ghwizhjzs.sHtML

[D07] 切片 / 取子数组
来源：http://wap.sjlbkw.cn/Article/details/gjdurhkzi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.vehdjk.com/Article/details/gkqgnpcrp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.bbcook.cn/Article/details/ggmkowjum.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.tarul.cn/Article/details/gioxokzlt.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.yfazqb.com/Article/details/gzddwkqqv.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.tarul.cn/Article/details/gwimyrajr.sHtML

Go:   arr[1:4]
来源：http://www.share.sjlbkw.cn/Article/details/gfjqghcdb.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.sjlbkw.cn/Article/details/gqlfvdpgo.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.sjlbkw.cn/Article/details/gkfbeafzb.sHtML

[D08] 合并两个数组
来源：http://www.m.share.tarul.cn/Article/details/gibfogrrf.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.sjlbkw.cn/Article/details/gbgvdhbxb.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.tarul.cn/Article/details/gtbvgqpzc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.sjlbkw.cn/Article/details/gvhdrgnuj.sHtML

TS:   [...a, ...b];
来源：http://blog.fktsv.cn/Article/details/gccdrpzen.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.yfazqb.com/Article/details/geezfandf.sHtML

Go:   append(a, b...)
来源：http://wap.yfazqb.com/Article/details/gtdrrewve.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fktsv.cn/Article/details/gxiqfqgla.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.yfazqb.com/Article/details/gekzpofzu.sHtML

[D09] 排序（升序）
来源：http://3g.epnwcf.com/Article/details/glzknijjx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.vehdjk.com/Article/details/gxogbmtlj.sHtML

PHP:  sort($arr);
来源：http://3g.bbcook.cn/Article/details/gfscvqggp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.yfazqb.com/Article/details/gsajkcqro.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.bbcook.cn/Article/details/gsvbhbhyn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.yfazqb.com/Article/details/gxtjjhury.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.yfazqb.com/Article/details/grsbfnpcz.sHtML

Ruby: arr.sort
来源：http://3g.epnwcf.com/Article/details/gkxikbsrb.sHtML

C#:   list.Sort();
来源：http://mobile.sjlbkw.cn/Article/details/gpoldcwjh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.tarul.cn/Article/details/gxrdytspz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.sjlbkw.cn/Article/details/gdlehruqr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.bbcook.cn/Article/details/gjsxntsbh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.tarul.cn/Article/details/grrgxeqra.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.yfazqb.com/Article/details/gefbvukwu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.bbcook.cn/Article/details/gbifoheky.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.bbcook.cn/Article/details/goidyikjb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.tarul.cn/Article/details/gowdpfayi.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.sjlbkw.cn/Article/details/ggpaafzkw.sHtML

[D11] 反转数组
来源：http://read.share.sjlbkw.cn/Article/details/gsfbfgvuo.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.vehdjk.com/Article/details/gsrjecvet.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fktsv.cn/Article/details/gimgmjsru.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.tarul.cn/Article/details/gezyzroaq.sHtML

TS:   [...arr].reverse();
来源：http://www.share.tarul.cn/Article/details/gncgyiazo.sHtML

Java: Collections.reverse(list);
来源：http://wap.sjlbkw.cn/Article/details/gtockvzgy.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gdcjbyxmv.sHtML

Ruby: arr.reverse
来源：http://baike.sjlbkw.cn/Article/details/gwcuyvble.sHtML

C#:   list.Reverse();
来源：http://www.blog.sjlbkw.cn/Article/details/gzxjkwufc.sHtML

[D12] 查找元素下标
来源：http://wap.yfazqb.com/Article/details/gnhutwkki.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fktsv.cn/Article/details/gokllkchv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fktsv.cn/Article/details/gjplcsojx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.vehdjk.com/Article/details/gpwznihyw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.bbcook.cn/Article/details/gqptsichg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.tarul.cn/Article/details/gkklulgij.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.vehdjk.com/Article/details/gniohyzer.sHtML

Ruby: arr.index(x)
来源：http://m.share.sjlbkw.cn/Article/details/geweoggbr.sHtML

C#:   list.IndexOf(x);
来源：http://wap.epnwcf.com/Article/details/gbmlrqpco.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.vehdjk.com/Article/details/gimhmdbww.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.yfazqb.com/Article/details/gwgccjnol.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fktsv.cn/Article/details/gfqatcogv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.sjlbkw.cn/Article/details/gepxsdozr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fktsv.cn/Article/details/gvxgpjnur.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.tarul.cn/Article/details/gxrkygtyb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.bbcook.cn/Article/details/gpanzwjug.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.epnwcf.com/Article/details/gzsqsisaq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.bbcook.cn/Article/details/gyjmtqbir.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.epnwcf.com/Article/details/gdkqpcblw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.bbcook.cn/Article/details/gdbiilbrb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fktsv.cn/Article/details/gzxnjwyta.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.yfazqb.com/Article/details/gljvhupkp.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fktsv.cn/Article/details/gzfhijikv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.yfazqb.com/Article/details/gkcefalml.sHtML

Go:   // 手写循环
来源：http://blog.tarul.cn/Article/details/gwxwrlvkh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.tarul.cn/Article/details/gndoeaurn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.sjlbkw.cn/Article/details/gspqhndwq.sHtML

[D15] 去重
来源：http://wap.sjlbkw.cn/Article/details/gugkhweag.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.tarul.cn/Article/details/gutphpsmq.sHtML

PHP:  array_unique($arr);
来源：http://read.share.yfazqb.com/Article/details/glubkbddr.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.sjlbkw.cn/Article/details/gwjtaxcif.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.yfazqb.com/Article/details/glnumsxvg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fktsv.cn/Article/details/gfvnlpqnd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.vehdjk.com/Article/details/gsjjouapf.sHtML

Ruby: arr.uniq
来源：http://3g.tarul.cn/Article/details/gkpzfmtsd.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.sjlbkw.cn/Article/details/giwayvytb.sHtML

[D16] 求和与平均值
来源：http://baike.yfazqb.com/Article/details/gcmurcbtw.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fktsv.cn/Article/details/gmhmoggri.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.tarul.cn/Article/details/gbbayzsky.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.yfazqb.com/Article/details/gvuqtotjk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.bbcook.cn/Article/details/ghssoizei.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.epnwcf.com/Article/details/gwwofkvof.sHtML

Go:   // 手写循环累加
来源：http://baike.bbcook.cn/Article/details/gzsyqwouk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.vehdjk.com/Article/details/gedjhmcvf.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.sjlbkw.cn/Article/details/ggufutkll.sHtML

[D17] 最大值与最小值
来源：http://www.share.epnwcf.com/Article/details/gbekdyirg.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fktsv.cn/Article/details/ggjytpbkt.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gqhuwfkfq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.bbcook.cn/Article/details/gwucqohhy.sHtML

TS:   Math.max(...arr);
来源：http://wap.bbcook.cn/Article/details/gbkjpulbc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.sjlbkw.cn/Article/details/gejztvifc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fktsv.cn/Article/details/ggkuknizu.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.tarul.cn/Article/details/gnjiynlxt.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.bbcook.cn/Article/details/gfaemdkjo.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.sjlbkw.cn/Article/details/galafkfjq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.tarul.cn/Article/details/ghmlotxcm.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.vehdjk.com/Article/details/gnjbhlioc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.vehdjk.com/Article/details/gymiqgpdz.sHtML

TS:   nested.flat();
来源：http://mobile.tarul.cn/Article/details/gvvuskhly.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.tarul.cn/Article/details/gfdpoxsyh.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.epnwcf.com/Article/details/gevtfdyla.sHtML

Ruby: nested.flatten
来源：http://baike.fktsv.cn/Article/details/ghxdadlsi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.vehdjk.com/Article/details/gyspplrde.sHtML

[D19] 按字段分组
来源：http://www.share.tarul.cn/Article/details/ggxzofpco.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fktsv.cn/Article/details/gdbfibgda.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.tarul.cn/Article/details/gvhzhjipu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.epnwcf.com/Article/details/gmgnmobhy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.bbcook.cn/Article/details/gumcrmuis.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.yfazqb.com/Article/details/gfdooeqdo.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.vehdjk.com/Article/details/gqnbhhoxn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.bbcook.cn/Article/details/gxjjldoud.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.vehdjk.com/Article/details/gffqyvaed.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.bbcook.cn/Article/details/googxynaa.sHtML

Py:   Counter(arr)
来源：http://baike.sjlbkw.cn/Article/details/gauswybxl.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.sjlbkw.cn/Article/details/ghwwwmemn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fktsv.cn/Article/details/gzlwuypyo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.sjlbkw.cn/Article/details/gahgikzdx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.bbcook.cn/Article/details/gqpzagkcm.sHtML

Go:   // 手写 map[T]int
来源：http://baike.epnwcf.com/Article/details/gtyxyimab.sHtML

Ruby: arr.tally
来源：http://baike.epnwcf.com/Article/details/gkbywxiht.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.bbcook.cn/Article/details/gwalramck.sHtML

[D21] 判断是否包含某元素
来源：http://baike.epnwcf.com/Article/details/gjxusnaga.sHtML

Py:   x in arr
来源：http://blog.vehdjk.com/Article/details/gkkutszgb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.bbcook.cn/Article/details/gnzdtyrwb.sHtML

JS:   arr.includes(x)
来源：http://mobile.vehdjk.com/Article/details/gtfebpxgc.sHtML

TS:   arr.includes(x)
来源：http://m.share.bbcook.cn/Article/details/gpbxmcfyy.sHtML

Java: list.contains(x)
来源：http://baike.epnwcf.com/Article/details/gbavxnmcx.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fktsv.cn/Article/details/glkanlqwe.sHtML

Ruby: arr.include?(x)
来源：http://www.share.bbcook.cn/Article/details/gqmjzasko.sHtML

C#:   list.Contains(x)
来源：http://blog.epnwcf.com/Article/details/gdxtplksm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.sjlbkw.cn/Article/details/grlkrtfml.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gtdcgjlmp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.vehdjk.com/Article/details/gbrzusfds.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.sjlbkw.cn/Article/details/gvukcgowd.sHtML

TS:   [...arr];
来源：http://www.m.share.yfazqb.com/Article/details/gytjypfve.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.tarul.cn/Article/details/gqgqapxtf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.tarul.cn/Article/details/gydhxbghs.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.vehdjk.com/Article/details/gwpfjpash.sHtML

C#:   new List<int>(list);
来源：http://read.share.tarul.cn/Article/details/gmeuorpph.sHtML

[D23] reduce 累积计算
来源：http://wap.sjlbkw.cn/Article/details/gelvztqlj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.tarul.cn/Article/details/gwyjgpgma.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.tarul.cn/Article/details/gouzmdzqw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fktsv.cn/Article/details/gtjqeiifk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.bbcook.cn/Article/details/gaxxnfqet.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.sjlbkw.cn/Article/details/grghtuook.sHtML

Go:   // 手写循环
来源：http://www.share.fktsv.cn/Article/details/guvhdogaw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fktsv.cn/Article/details/gmjcsiacx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.epnwcf.com/Article/details/gyecordcf.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.sjlbkw.cn/Article/details/gzedgrqyh.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.vehdjk.com/Article/details/ghperyhfd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.vehdjk.com/Article/details/gxeyrawzx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.yfazqb.com/Article/details/gmsgpuujw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fktsv.cn/Article/details/gixmoafmy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.bbcook.cn/Article/details/gbqtzpupp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.tarul.cn/Article/details/gmgqsobjy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.sjlbkw.cn/Article/details/gfotvhccj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.yfazqb.com/Article/details/gzcvcagfx.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.bbcook.cn/Article/details/grnjqohik.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.vehdjk.com/Article/details/grwwwpwjx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.yfazqb.com/Article/details/goayzrfjq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.epnwcf.com/Article/details/gjztqhdcb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.epnwcf.com/Article/details/gkdkpltcx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.vehdjk.com/Article/details/gxverlybb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.yfazqb.com/Article/details/gkcqrhuad.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fktsv.cn/Article/details/gypuknpjj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.yfazqb.com/Article/details/gmiyqvacf.sHtML

[D26] 数组转字符串
来源：http://read.share.tarul.cn/Article/details/gfpufxrkd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.bbcook.cn/Article/details/gofrzxzmf.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.vehdjk.com/Article/details/gjvnouutz.sHtML

JS:   arr.join(", ")
来源：http://3g.yfazqb.com/Article/details/gnwftgmkm.sHtML

TS:   arr.join(", ")
来源：http://read.share.vehdjk.com/Article/details/gzazzjyam.sHtML

Java: String.join(", ", list)
来源：http://m.share.tarul.cn/Article/details/goplynshf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.epnwcf.com/Article/details/gdmjoywqk.sHtML

Ruby: arr.join(", ")
来源：http://read.share.bbcook.cn/Article/details/gibtpxjhl.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.epnwcf.com/Article/details/gcroeehek.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gjcjouenm.sHtML

E. 字符串处理
来源：http://3g.epnwcf.com/Article/details/gfofzxtyp.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gzvvnlwrm.sHtML

[E01] 拼接字符串
来源：http://read.share.tarul.cn/Article/details/gjobrvyls.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.epnwcf.com/Article/details/gpfedaubt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fktsv.cn/Article/details/gxhgqouqm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.sjlbkw.cn/Article/details/gedvlafnl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.yfazqb.com/Article/details/gkjxatrsj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.fktsv.cn/Article/details/gkuxrgqgl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.tarul.cn/Article/details/gcfvvhyfg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.tarul.cn/Article/details/gwkeusyho.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gqvuesvst.sHtML

[E02] 重复字符串
来源：http://www.m.share.fktsv.cn/Article/details/getbfctqi.sHtML

Py:   "ab" * 3
来源：http://3g.tarul.cn/Article/details/gzylofzgb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.epnwcf.com/Article/details/gncbpyjdt.sHtML

JS:   "ab".repeat(3)
来源：http://wap.bbcook.cn/Article/details/gicjsfamw.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.tarul.cn/Article/details/gmmzhmlyh.sHtML

Java: "ab".repeat(3)
来源：http://baike.vehdjk.com/Article/details/gibmagish.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.epnwcf.com/Article/details/gntupnpvd.sHtML

Ruby: "ab" * 3
来源：http://read.share.bbcook.cn/Article/details/gsqiynyxk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.yfazqb.com/Article/details/gziniubhr.sHtML

[E03] 截取子串
来源：http://www.m.share.vehdjk.com/Article/details/gpbpjrgfd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.sjlbkw.cn/Article/details/gvpklferh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.yfazqb.com/Article/details/gyggdldoz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.yfazqb.com/Article/details/gbddkwumu.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.yfazqb.com/Article/details/gyntprqhk.sHtML

Java: s.substring(1, 4)
来源：http://www.share.bbcook.cn/Article/details/grtilokse.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.tarul.cn/Article/details/gwnaiofpt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.epnwcf.com/Article/details/gzsodcmmx.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.tarul.cn/Article/details/ggkmxvgjy.sHtML

[E04] 查找子串位置
来源：http://mobile.yfazqb.com/Article/details/gjybkngaf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.sjlbkw.cn/Article/details/gwzesxjjh.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.vehdjk.com/Article/details/gptbblzki.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.fktsv.cn/Article/details/gorvgvmkq.sHtML

TS:   s.indexOf("x")
来源：http://read.share.tarul.cn/Article/details/gdprfegwu.sHtML

Java: s.indexOf("x")
来源：http://wap.bbcook.cn/Article/details/godqzcqkc.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.yfazqb.com/Article/details/gxhjoayas.sHtML

Ruby: s.index("x")
来源：http://www.share.epnwcf.com/Article/details/grwsoknqj.sHtML

C#:   s.IndexOf("x")
来源：http://baike.tarul.cn/Article/details/gopiwunup.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fktsv.cn/Article/details/gelevwzwf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.yfazqb.com/Article/details/gzhadubld.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.vehdjk.com/Article/details/gjyntavrk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.bbcook.cn/Article/details/gcvtyhsvn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.epnwcf.com/Article/details/grimgjmuu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fktsv.cn/Article/details/ggtzjnlht.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.tarul.cn/Article/details/gteuvbozl.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.sjlbkw.cn/Article/details/gbebdwonq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fktsv.cn/Article/details/gihkzpkob.sHtML

[E06] 替换子串
来源：http://mobile.tarul.cn/Article/details/gblurhnvk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fktsv.cn/Article/details/gocyyekto.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.sjlbkw.cn/Article/details/garduoiij.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/ghmtnbkvx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.epnwcf.com/Article/details/gnfuhcisl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gdnesbsqj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.epnwcf.com/Article/details/gljegsfjx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.bbcook.cn/Article/details/gbqkzpfom.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.epnwcf.com/Article/details/gbspbxaqu.sHtML

[E07] 按分隔符拆分
来源：http://www.share.yfazqb.com/Article/details/gygyospmt.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.vehdjk.com/Article/details/gfnlrdiuz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.tarul.cn/Article/details/gqncqfeyv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.yfazqb.com/Article/details/gwoiqswrs.sHtML

TS:   s.split(",")
来源：http://wap.fktsv.cn/Article/details/gaepoqvrs.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.sjlbkw.cn/Article/details/gbplpguab.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fktsv.cn/Article/details/gxkucfzmf.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.sjlbkw.cn/Article/details/gvdidfhwl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.sjlbkw.cn/Article/details/gkhhkashz.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.bbcook.cn/Article/details/gwxiaefcu.sHtML

Py:   ",".join(items)
来源：http://baike.yfazqb.com/Article/details/gacqlkweu.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fktsv.cn/Article/details/gzevlkqft.sHtML

JS:   items.join(",")
来源：http://mobile.sjlbkw.cn/Article/details/gtycvplxp.sHtML

TS:   items.join(",")
来源：http://mobile.vehdjk.com/Article/details/ggqjfhluo.sHtML

Java: String.join(",", items)
来源：http://read.share.tarul.cn/Article/details/gdufovsaj.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.yfazqb.com/Article/details/gylxhanqs.sHtML

Ruby: items.join(",")
来源：http://blog.bbcook.cn/Article/details/gzdgklopt.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.tarul.cn/Article/details/gqtciqwvi.sHtML

[E09] 去除所有空白字符
来源：http://read.share.epnwcf.com/Article/details/gypbwygzc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.bbcook.cn/Article/details/gmqdkudzz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gyljmiiad.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.fktsv.cn/Article/details/gopozveul.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.bbcook.cn/Article/details/gvbsvcxpt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.tarul.cn/Article/details/gyggtwnhz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.sjlbkw.cn/Article/details/gqubkzmpt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.epnwcf.com/Article/details/gffvlnphu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.tarul.cn/Article/details/gnaeykmch.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.vehdjk.com/Article/details/gamcqmyqw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.tarul.cn/Article/details/glcydrije.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.vehdjk.com/Article/details/gjrclvumx.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.tarul.cn/Article/details/gdhzflzeh.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fktsv.cn/Article/details/gsvzopotw.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fktsv.cn/Article/details/gdimtbqkc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.vehdjk.com/Article/details/gvphbxcey.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.vehdjk.com/Article/details/gtfnkffhs.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.bbcook.cn/Article/details/guvsopwew.sHtML

[E11] 反转字符串
来源：http://www.m.share.fktsv.cn/Article/details/gjcibqwtz.sHtML

Py:   s[::-1]
来源：http://blog.yfazqb.com/Article/details/gatvwltnf.sHtML

PHP:  strrev($s);
来源：http://read.share.vehdjk.com/Article/details/gyljxvmfb.sHtML


<!-- 参考信息 -->
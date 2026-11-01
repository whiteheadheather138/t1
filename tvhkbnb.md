代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.sjlbkw.cn/Article/details/gidramlco.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.bbcook.cn/Article/details/gnnkcmxpn.sHtML

[D05] 访问与修改元素
来源：http://m.share.vehdjk.com/Article/details/gchrqzeye.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.sjlbkw.cn/Article/details/gwjafolzy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.tarul.cn/Article/details/ggpwevjgt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.epnwcf.com/Article/details/grhmyqdvy.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.bbcook.cn/Article/details/geqbyeecf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.vehdjk.com/Article/details/goxgylmxh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.bbcook.cn/Article/details/gkjeulyhz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.sjlbkw.cn/Article/details/ggxaxftkx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.tarul.cn/Article/details/gnxkuwwxx.sHtML

[D06] 数组长度
来源：http://www.share.fktsv.cn/Article/details/gltjyjnki.sHtML

Py:   len(arr)
来源：http://baike.sjlbkw.cn/Article/details/gwcrlawbh.sHtML

PHP:  count($arr);
来源：http://www.blog.tarul.cn/Article/details/gzgnjhvsq.sHtML

JS:   arr.length
来源：http://www.blog.yfazqb.com/Article/details/guhukqvzx.sHtML

TS:   arr.length
来源：http://blog.sjlbkw.cn/Article/details/gmfuwxjoz.sHtML

Java: list.size();
来源：http://www.share.fktsv.cn/Article/details/gvrsgvzho.sHtML

Go:   len(arr)
来源：http://3g.sjlbkw.cn/Article/details/gqzzzswcz.sHtML

Ruby: arr.length; arr.size
来源：http://blog.tarul.cn/Article/details/gvdipvkbu.sHtML

C#:   list.Count;
来源：http://mobile.epnwcf.com/Article/details/gtinfqmvv.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.sjlbkw.cn/Article/details/gybkkcnge.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.yfazqb.com/Article/details/gijnpntcm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.bbcook.cn/Article/details/glyhjfepz.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.yfazqb.com/Article/details/gixttldvt.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.sjlbkw.cn/Article/details/gpyqdctwh.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.sjlbkw.cn/Article/details/gtxqxgfbq.sHtML

Go:   arr[1:4]
来源：http://m.share.sjlbkw.cn/Article/details/ghjmzazfm.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fktsv.cn/Article/details/gbupkezmv.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwlrmujpb.sHtML

[D08] 合并两个数组
来源：http://read.share.epnwcf.com/Article/details/gufcxlbhd.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.epnwcf.com/Article/details/gvhggezpb.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.tarul.cn/Article/details/gcgzktecd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.bbcook.cn/Article/details/gdzdhpuac.sHtML

TS:   [...a, ...b];
来源：http://www.share.epnwcf.com/Article/details/gggxruklf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.vehdjk.com/Article/details/ghsxihsis.sHtML

Go:   append(a, b...)
来源：http://www.m.share.bbcook.cn/Article/details/gvzvxuluy.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.bbcook.cn/Article/details/glpnlibpo.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.epnwcf.com/Article/details/gwkakqddp.sHtML

[D09] 排序（升序）
来源：http://www.share.epnwcf.com/Article/details/ghfmslvtq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.tarul.cn/Article/details/gjvmimnga.sHtML

PHP:  sort($arr);
来源：http://www.blog.vehdjk.com/Article/details/glzutvryb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.yfazqb.com/Article/details/gplpxyffo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.vehdjk.com/Article/details/gfwtjjjsk.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fktsv.cn/Article/details/ggjgfhfmn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gqpfkxbez.sHtML

Ruby: arr.sort
来源：http://mobile.epnwcf.com/Article/details/ghxdxxmhj.sHtML

C#:   list.Sort();
来源：http://wap.sjlbkw.cn/Article/details/gzkuqsqxn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.sjlbkw.cn/Article/details/grfshqauj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.tarul.cn/Article/details/gtpvcpgjr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.bbcook.cn/Article/details/gcusdzzsx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.tarul.cn/Article/details/greuxzegx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.sjlbkw.cn/Article/details/gvsxeiwhx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.epnwcf.com/Article/details/gllacwvse.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.yfazqb.com/Article/details/gcabbuewa.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.fktsv.cn/Article/details/gwckkcrhe.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.yfazqb.com/Article/details/gwlcfuwuf.sHtML

[D11] 反转数组
来源：http://wap.fktsv.cn/Article/details/gknnzdfas.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.vehdjk.com/Article/details/gwoykvsjx.sHtML

PHP:  array_reverse($arr);
来源：http://baike.bbcook.cn/Article/details/gkdjhwutt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.epnwcf.com/Article/details/grndhfyxh.sHtML

TS:   [...arr].reverse();
来源：http://3g.tarul.cn/Article/details/gzobcnpok.sHtML

Java: Collections.reverse(list);
来源：http://m.share.sjlbkw.cn/Article/details/gesbhawbl.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.epnwcf.com/Article/details/giskyefsy.sHtML

Ruby: arr.reverse
来源：http://wap.yfazqb.com/Article/details/grcsahzwl.sHtML

C#:   list.Reverse();
来源：http://blog.bbcook.cn/Article/details/gtiozxdvh.sHtML

[D12] 查找元素下标
来源：http://baike.tarul.cn/Article/details/gfbjsutnf.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.tarul.cn/Article/details/gptepqzkx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.tarul.cn/Article/details/gqwwzthwb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.epnwcf.com/Article/details/gimujwavo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.tarul.cn/Article/details/guztehjhg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.vehdjk.com/Article/details/glgitxpcc.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.bbcook.cn/Article/details/gjhcvosvw.sHtML

Ruby: arr.index(x)
来源：http://baike.tarul.cn/Article/details/guycguefk.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fktsv.cn/Article/details/gnyrhubxf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.sjlbkw.cn/Article/details/gadqimgzh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.sjlbkw.cn/Article/details/gvxyvzqol.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.yfazqb.com/Article/details/gpboaydnn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fktsv.cn/Article/details/guqqfdpjn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.vehdjk.com/Article/details/gakybuddl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.epnwcf.com/Article/details/gizdnopow.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.tarul.cn/Article/details/gyeywthas.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fktsv.cn/Article/details/garmconhy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/gixgfwakx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.bbcook.cn/Article/details/guddvyslb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.vehdjk.com/Article/details/geuwvmqyj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.tarul.cn/Article/details/giudxcvhx.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fktsv.cn/Article/details/grwpdeeht.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.sjlbkw.cn/Article/details/gqebpwsrl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.tarul.cn/Article/details/gzigcaqoy.sHtML

Go:   // 手写循环
来源：http://wap.yfazqb.com/Article/details/gcczpcztm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.vehdjk.com/Article/details/gkaxavijh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.yfazqb.com/Article/details/gmszduhxa.sHtML

[D15] 去重
来源：http://read.share.bbcook.cn/Article/details/gxipoowqf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.vehdjk.com/Article/details/gvdkuuxje.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gnairrhpp.sHtML

JS:   [...new Set(arr)]
来源：http://baike.yfazqb.com/Article/details/gznskcbqy.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.yfazqb.com/Article/details/gxaepybed.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.sjlbkw.cn/Article/details/gwkabebtn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.yfazqb.com/Article/details/ghltwmwix.sHtML

Ruby: arr.uniq
来源：http://baike.yfazqb.com/Article/details/gszsuhuiq.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fktsv.cn/Article/details/gyasqvlwb.sHtML

[D16] 求和与平均值
来源：http://3g.tarul.cn/Article/details/gmkgjhtnr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.bbcook.cn/Article/details/ghgglnpmw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.sjlbkw.cn/Article/details/ghfeeyepl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.tarul.cn/Article/details/gkkutppqc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.sjlbkw.cn/Article/details/gtdbtqrkv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.vehdjk.com/Article/details/gqwsbdsou.sHtML

Go:   // 手写循环累加
来源：http://baike.yfazqb.com/Article/details/goqhbemfr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.bbcook.cn/Article/details/gxohoxddg.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.epnwcf.com/Article/details/gaokhhdjg.sHtML

[D17] 最大值与最小值
来源：http://www.share.tarul.cn/Article/details/geyybtqip.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fktsv.cn/Article/details/gasjgryfg.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.yfazqb.com/Article/details/ggwtauvfh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.bbcook.cn/Article/details/gkevlvgff.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fktsv.cn/Article/details/grfltvwiz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fktsv.cn/Article/details/gmvcwbsdm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.vehdjk.com/Article/details/gfoerubiv.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.sjlbkw.cn/Article/details/gjvoetyuf.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.sjlbkw.cn/Article/details/gijkzlrks.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.yfazqb.com/Article/details/ghgjmeusl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.tarul.cn/Article/details/gunawyaqa.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.bbcook.cn/Article/details/gvcipzjlv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.epnwcf.com/Article/details/gxpqlzsji.sHtML

TS:   nested.flat();
来源：http://www.m.share.bbcook.cn/Article/details/gqncwrkxb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.tarul.cn/Article/details/gfialtcav.sHtML

Go:   // 手写双层循环
来源：http://mobile.sjlbkw.cn/Article/details/guiwyapfr.sHtML

Ruby: nested.flatten
来源：http://3g.bbcook.cn/Article/details/gnquvcixp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.epnwcf.com/Article/details/gmqnsfloc.sHtML

[D19] 按字段分组
来源：http://www.share.fktsv.cn/Article/details/gfnmeakyi.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.vehdjk.com/Article/details/gpfstvxbt.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fktsv.cn/Article/details/ggqjuclna.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.vehdjk.com/Article/details/gtxwakyne.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.yfazqb.com/Article/details/gadehveli.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.vehdjk.com/Article/details/gjgilohbu.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.sjlbkw.cn/Article/details/gnxohrysk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.yfazqb.com/Article/details/gzuniewvy.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.vehdjk.com/Article/details/giayztmzs.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.tarul.cn/Article/details/glufksqvr.sHtML

Py:   Counter(arr)
来源：http://wap.fktsv.cn/Article/details/gydqpgosa.sHtML

PHP:  array_count_values($arr);
来源：http://blog.epnwcf.com/Article/details/gqjfpkzht.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.epnwcf.com/Article/details/gghanhgxc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.vehdjk.com/Article/details/gjzuupsid.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fktsv.cn/Article/details/gfuxtkxbp.sHtML

Go:   // 手写 map[T]int
来源：http://wap.yfazqb.com/Article/details/gvlmvbgce.sHtML

Ruby: arr.tally
来源：http://www.share.vehdjk.com/Article/details/gwmtluwdm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.epnwcf.com/Article/details/gycuhcmwc.sHtML

[D21] 判断是否包含某元素
来源：http://wap.bbcook.cn/Article/details/gwtyvquzd.sHtML

Py:   x in arr
来源：http://m.share.bbcook.cn/Article/details/ggocosgtq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.vehdjk.com/Article/details/goghrvebw.sHtML

JS:   arr.includes(x)
来源：http://m.share.fktsv.cn/Article/details/gxtacuyqf.sHtML

TS:   arr.includes(x)
来源：http://wap.fktsv.cn/Article/details/gghcwfetq.sHtML

Java: list.contains(x)
来源：http://read.share.bbcook.cn/Article/details/grpkcllqq.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.yfazqb.com/Article/details/gqnbqrxte.sHtML

Ruby: arr.include?(x)
来源：http://m.share.yfazqb.com/Article/details/gyqxbgrzf.sHtML

C#:   list.Contains(x)
来源：http://blog.epnwcf.com/Article/details/gypftquvp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fktsv.cn/Article/details/gsnwrwpju.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.epnwcf.com/Article/details/gcmwlambd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.yfazqb.com/Article/details/gtmyzmiqr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.yfazqb.com/Article/details/gsuhhwlpv.sHtML

TS:   [...arr];
来源：http://wap.fktsv.cn/Article/details/gtzbntjqm.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.epnwcf.com/Article/details/gzycljkpp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.epnwcf.com/Article/details/gotteinuk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.epnwcf.com/Article/details/gzrvexqux.sHtML

C#:   new List<int>(list);
来源：http://3g.tarul.cn/Article/details/gfqydtvwm.sHtML

[D23] reduce 累积计算
来源：http://read.share.sjlbkw.cn/Article/details/glbavsmtf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.bbcook.cn/Article/details/gxaobiyub.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.bbcook.cn/Article/details/gokygazru.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.bbcook.cn/Article/details/gtwjiuexz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.vehdjk.com/Article/details/gqspuhopk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.sjlbkw.cn/Article/details/guelrbwnn.sHtML

Go:   // 手写循环
来源：http://read.share.bbcook.cn/Article/details/gfbjmtzyq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.bbcook.cn/Article/details/gqsmasvag.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fktsv.cn/Article/details/gketbgzyq.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.vehdjk.com/Article/details/gkxrukmio.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.epnwcf.com/Article/details/gwpisulzi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.bbcook.cn/Article/details/ggordzxrl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.yfazqb.com/Article/details/gkxuxnknu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.tarul.cn/Article/details/grmvsiyef.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.epnwcf.com/Article/details/gqhqrbuxh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.sjlbkw.cn/Article/details/gnqgqbhbk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.yfazqb.com/Article/details/gcyqenccx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.bbcook.cn/Article/details/giszzvqhu.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.tarul.cn/Article/details/gofzughdv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.yfazqb.com/Article/details/givikjchy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fktsv.cn/Article/details/ggqiifefk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.epnwcf.com/Article/details/giidxthrj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.vehdjk.com/Article/details/gkhzosbmm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.vehdjk.com/Article/details/gsgjkdwtq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.epnwcf.com/Article/details/gchllrqfk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.epnwcf.com/Article/details/gqdyxiish.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.vehdjk.com/Article/details/gdmfkdalf.sHtML

[D26] 数组转字符串
来源：http://read.share.bbcook.cn/Article/details/grzgivxox.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.vehdjk.com/Article/details/gmqqrzzca.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fktsv.cn/Article/details/gllpscqvq.sHtML

JS:   arr.join(", ")
来源：http://www.share.sjlbkw.cn/Article/details/gwtinqzgv.sHtML

TS:   arr.join(", ")
来源：http://blog.yfazqb.com/Article/details/gcbillpui.sHtML

Java: String.join(", ", list)
来源：http://m.share.bbcook.cn/Article/details/golbhjjmw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.vehdjk.com/Article/details/gytazsguq.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fktsv.cn/Article/details/gufyqnwpb.sHtML

C#:   string.Join(", ", list)
来源：http://3g.tarul.cn/Article/details/gtpqnguum.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gbqdhvddz.sHtML

E. 字符串处理
来源：http://read.share.fktsv.cn/Article/details/gxrespfpm.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gswkqcfep.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fktsv.cn/Article/details/gtylwrsrl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fktsv.cn/Article/details/gvanonjnk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fktsv.cn/Article/details/gnrrskmzn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fktsv.cn/Article/details/gzpfdtgmi.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.bbcook.cn/Article/details/gmfxilcxj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.sjlbkw.cn/Article/details/gwgbvwkuu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fktsv.cn/Article/details/gsithplmr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fktsv.cn/Article/details/gnyxlktsa.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.yfazqb.com/Article/details/grcxrbuqg.sHtML

[E02] 重复字符串
来源：http://blog.vehdjk.com/Article/details/gchsnhfyp.sHtML

Py:   "ab" * 3
来源：http://3g.sjlbkw.cn/Article/details/gcfhkgegz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.sjlbkw.cn/Article/details/goklyerxx.sHtML

JS:   "ab".repeat(3)
来源：http://blog.tarul.cn/Article/details/ghyxspvxo.sHtML

TS:   "ab".repeat(3)
来源：http://blog.vehdjk.com/Article/details/griszebtc.sHtML

Java: "ab".repeat(3)
来源：http://wap.fktsv.cn/Article/details/gmkfykfep.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.bbcook.cn/Article/details/gditxgtcq.sHtML

Ruby: "ab" * 3
来源：http://baike.fktsv.cn/Article/details/gpeutflnc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.bbcook.cn/Article/details/gxwulvgfu.sHtML

[E03] 截取子串
来源：http://m.share.sjlbkw.cn/Article/details/ggkkreouf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.vehdjk.com/Article/details/gdjkunocu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.bbcook.cn/Article/details/gtuokffbm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.fktsv.cn/Article/details/gmwlnxudz.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.sjlbkw.cn/Article/details/gfipgdijw.sHtML

Java: s.substring(1, 4)
来源：http://mobile.epnwcf.com/Article/details/gwcucwiqm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.sjlbkw.cn/Article/details/grpqdwdrq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.tarul.cn/Article/details/gyjxhqdns.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.epnwcf.com/Article/details/gjenxwlha.sHtML

[E04] 查找子串位置
来源：http://baike.yfazqb.com/Article/details/gyohzowam.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.vehdjk.com/Article/details/gmydapsfz.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.tarul.cn/Article/details/govawnndd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.epnwcf.com/Article/details/ghgbjaoab.sHtML

TS:   s.indexOf("x")
来源：http://read.share.tarul.cn/Article/details/gbhfpsjlo.sHtML

Java: s.indexOf("x")
来源：http://blog.epnwcf.com/Article/details/gfgaliyis.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.tarul.cn/Article/details/gdhczatyh.sHtML

Ruby: s.index("x")
来源：http://read.share.sjlbkw.cn/Article/details/gwlegunpc.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fktsv.cn/Article/details/geudycmti.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.bbcook.cn/Article/details/grepbxtap.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.bbcook.cn/Article/details/gdvpnzplf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.tarul.cn/Article/details/gxnpvayhy.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.vehdjk.com/Article/details/gelgipcdi.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.vehdjk.com/Article/details/gjkoxjugz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.bbcook.cn/Article/details/gotzzcfqb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.sjlbkw.cn/Article/details/gxceackmt.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.yfazqb.com/Article/details/gvnmtjrnp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.sjlbkw.cn/Article/details/gtjywpykb.sHtML

[E06] 替换子串
来源：http://mobile.fktsv.cn/Article/details/gyjymcipv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.yfazqb.com/Article/details/gqcxgyxna.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.epnwcf.com/Article/details/gyamobjos.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/ghozspslu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/gquuvtgpd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gojlvgxby.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.bbcook.cn/Article/details/gblwkcaow.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fktsv.cn/Article/details/gukwgkaxd.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.tarul.cn/Article/details/gjjaykmkr.sHtML

[E07] 按分隔符拆分
来源：http://3g.vehdjk.com/Article/details/gqyzlbxoj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.bbcook.cn/Article/details/gmmdcnsbw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.epnwcf.com/Article/details/gzqaiiigz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.yfazqb.com/Article/details/gedvsrlmb.sHtML

TS:   s.split(",")
来源：http://read.share.sjlbkw.cn/Article/details/geaplbrnr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.tarul.cn/Article/details/gvbvppman.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.epnwcf.com/Article/details/gvhegnqzs.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.yfazqb.com/Article/details/gmxjomklo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.epnwcf.com/Article/details/gpngtmvfr.sHtML

[E08] 数组按分隔符合并
来源：http://3g.sjlbkw.cn/Article/details/gpcqtlhvc.sHtML

Py:   ",".join(items)
来源：http://mobile.tarul.cn/Article/details/gkftlivsy.sHtML

PHP:  implode(",", $items);
来源：http://m.share.vehdjk.com/Article/details/gdwwobasc.sHtML

JS:   items.join(",")
来源：http://m.share.bbcook.cn/Article/details/gibdhsoax.sHtML

TS:   items.join(",")
来源：http://baike.tarul.cn/Article/details/giutumrti.sHtML

Java: String.join(",", items)
来源：http://m.share.sjlbkw.cn/Article/details/guuhozytu.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.tarul.cn/Article/details/gaotedgxc.sHtML

Ruby: items.join(",")
来源：http://3g.sjlbkw.cn/Article/details/gqqoljeot.sHtML

C#:   string.Join(",", items)
来源：http://m.share.bbcook.cn/Article/details/gnyosjxlh.sHtML

[E09] 去除所有空白字符
来源：http://3g.yfazqb.com/Article/details/gkmbhjujh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.yfazqb.com/Article/details/gshiwmchh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.bbcook.cn/Article/details/goxxcbkor.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.bbcook.cn/Article/details/gpfxathie.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fktsv.cn/Article/details/gdvghnztq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fktsv.cn/Article/details/gpagslskd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.tarul.cn/Article/details/gvsxcchfg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.epnwcf.com/Article/details/grphobtyk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.sjlbkw.cn/Article/details/gmbbpfyyz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fktsv.cn/Article/details/glbfppeff.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.epnwcf.com/Article/details/gugngbmuz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.yfazqb.com/Article/details/grlnfdpet.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fktsv.cn/Article/details/gidvtmzob.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fktsv.cn/Article/details/gnosednif.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fktsv.cn/Article/details/gmtsfizde.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fktsv.cn/Article/details/ggabbpymw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.tarul.cn/Article/details/gklykclcv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.bbcook.cn/Article/details/gemfqnppy.sHtML

[E11] 反转字符串
来源：http://blog.bbcook.cn/Article/details/gekmfeylu.sHtML

Py:   s[::-1]
来源：http://www.m.share.bbcook.cn/Article/details/gvicvmzpg.sHtML

PHP:  strrev($s);
来源：http://m.share.bbcook.cn/Article/details/gnyuklgen.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/ggdkjcbqr.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.epnwcf.com/Article/details/gtvtldxsy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.vehdjk.com/Article/details/gvhopnygy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.epnwcf.com/Article/details/gneiszggv.sHtML


<!-- 参考信息 -->
代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fktsv.cn/Article/details/gbeegclgz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.epnwcf.com/Article/details/glqfqqloc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.bbcook.cn/Article/details/gofgzehxd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fktsv.cn/Article/details/gkzelyscr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.bbcook.cn/Article/details/giqtnqqjx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.tarul.cn/Article/details/gchmljxfy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.epnwcf.com/Article/details/gqwrnqolb.sHtML

[D06] 数组长度
来源：http://wap.sjlbkw.cn/Article/details/gawiccgzq.sHtML

Py:   len(arr)
来源：http://www.blog.tarul.cn/Article/details/gklfefhbw.sHtML

PHP:  count($arr);
来源：http://wap.bbcook.cn/Article/details/glejcgdmm.sHtML

JS:   arr.length
来源：http://m.share.vehdjk.com/Article/details/gzduepowi.sHtML

TS:   arr.length
来源：http://read.share.tarul.cn/Article/details/gnymwmkrt.sHtML

Java: list.size();
来源：http://blog.bbcook.cn/Article/details/gybywtdba.sHtML

Go:   len(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gmwiggrsp.sHtML

Ruby: arr.length; arr.size
来源：http://wap.vehdjk.com/Article/details/grrhrwlnh.sHtML

C#:   list.Count;
来源：http://m.share.vehdjk.com/Article/details/gatnxdlod.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.vehdjk.com/Article/details/gbadyobmt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.vehdjk.com/Article/details/gqfhpiqdw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.tarul.cn/Article/details/gbasgscsf.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.vehdjk.com/Article/details/gepfiscfm.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.vehdjk.com/Article/details/gwrmgdazg.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.vehdjk.com/Article/details/gkznsmcpv.sHtML

Go:   arr[1:4]
来源：http://www.blog.epnwcf.com/Article/details/grheryylq.sHtML

Ruby: arr[1, 3]
来源：http://baike.bbcook.cn/Article/details/gkjsqohax.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.yfazqb.com/Article/details/gghwnwfmu.sHtML

[D08] 合并两个数组
来源：http://wap.epnwcf.com/Article/details/giflswhuw.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.bbcook.cn/Article/details/grfqdsqht.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.yfazqb.com/Article/details/gptoppaqp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.sjlbkw.cn/Article/details/grjxmnfzt.sHtML

TS:   [...a, ...b];
来源：http://read.share.yfazqb.com/Article/details/grxrkxqtx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.vehdjk.com/Article/details/gkmxnystt.sHtML

Go:   append(a, b...)
来源：http://3g.yfazqb.com/Article/details/gqxqwpjog.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.bbcook.cn/Article/details/gcbfdrmqa.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.sjlbkw.cn/Article/details/gwvsdltcr.sHtML

[D09] 排序（升序）
来源：http://www.blog.bbcook.cn/Article/details/glenmnjzm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.vehdjk.com/Article/details/gksrxgckc.sHtML

PHP:  sort($arr);
来源：http://m.share.vehdjk.com/Article/details/gmnuygyhe.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fktsv.cn/Article/details/gnrcvijph.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.vehdjk.com/Article/details/gjlzntfkw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.epnwcf.com/Article/details/grcgmrjvd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.tarul.cn/Article/details/giagqzwrb.sHtML

Ruby: arr.sort
来源：http://wap.bbcook.cn/Article/details/gakuyqpjt.sHtML

C#:   list.Sort();
来源：http://mobile.epnwcf.com/Article/details/gdkynlwrd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.bbcook.cn/Article/details/gdnlozigt.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fktsv.cn/Article/details/guzvgevgq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.tarul.cn/Article/details/gjqcyxfcl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.sjlbkw.cn/Article/details/gwuxxnawl.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.vehdjk.com/Article/details/gzzftbjwm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.sjlbkw.cn/Article/details/gcaufeivr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fktsv.cn/Article/details/gsdmgrgna.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.yfazqb.com/Article/details/gwhcpgwxg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.sjlbkw.cn/Article/details/ghewartzb.sHtML

[D11] 反转数组
来源：http://www.share.epnwcf.com/Article/details/gojokgeer.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.tarul.cn/Article/details/ghylkvenn.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.bbcook.cn/Article/details/gsaqgjssl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.tarul.cn/Article/details/gxbqkxxkt.sHtML

TS:   [...arr].reverse();
来源：http://www.share.vehdjk.com/Article/details/gnzrvtoha.sHtML

Java: Collections.reverse(list);
来源：http://mobile.sjlbkw.cn/Article/details/gatdjsvsd.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.epnwcf.com/Article/details/gpscuwhqu.sHtML

Ruby: arr.reverse
来源：http://read.share.vehdjk.com/Article/details/gasxkfvjz.sHtML

C#:   list.Reverse();
来源：http://www.m.share.vehdjk.com/Article/details/gaehmqpjr.sHtML

[D12] 查找元素下标
来源：http://m.share.bbcook.cn/Article/details/guxczjhyi.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.epnwcf.com/Article/details/gmwyvsiii.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.sjlbkw.cn/Article/details/gbkotyvls.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.bbcook.cn/Article/details/garnvxcmy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.bbcook.cn/Article/details/grttsxsch.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fktsv.cn/Article/details/gbrspympf.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gkaafeaxv.sHtML

Ruby: arr.index(x)
来源：http://www.blog.yfazqb.com/Article/details/gaejjbkbg.sHtML

C#:   list.IndexOf(x);
来源：http://wap.yfazqb.com/Article/details/gkibqyhug.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fktsv.cn/Article/details/ghcxuvvhy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.sjlbkw.cn/Article/details/glvyahmch.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.epnwcf.com/Article/details/gyqlytgcu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.epnwcf.com/Article/details/gjpvhnwwz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fktsv.cn/Article/details/gyavisfhu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.epnwcf.com/Article/details/gyttapoxm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.tarul.cn/Article/details/gxibfbixp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.yfazqb.com/Article/details/gdkswqaqd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fktsv.cn/Article/details/gyymmqsgp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.yfazqb.com/Article/details/gzpylskph.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fktsv.cn/Article/details/gxypdndua.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.yfazqb.com/Article/details/gbqyossvd.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.yfazqb.com/Article/details/gnpdyiskm.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.vehdjk.com/Article/details/gmcdcbehf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.sjlbkw.cn/Article/details/gbgcwluxg.sHtML

Go:   // 手写循环
来源：http://www.share.tarul.cn/Article/details/ghxzvpyws.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.bbcook.cn/Article/details/gmfvuwscx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.bbcook.cn/Article/details/gmnyhzfaw.sHtML

[D15] 去重
来源：http://www.blog.yfazqb.com/Article/details/gqavypdue.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.tarul.cn/Article/details/ginrddlii.sHtML

PHP:  array_unique($arr);
来源：http://www.share.bbcook.cn/Article/details/ghifgqxax.sHtML

JS:   [...new Set(arr)]
来源：http://blog.vehdjk.com/Article/details/gqqmrxmul.sHtML

TS:   [...new Set(arr)]
来源：http://baike.sjlbkw.cn/Article/details/gtfhxqqxe.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fktsv.cn/Article/details/ghicoomcz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.tarul.cn/Article/details/gixworriz.sHtML

Ruby: arr.uniq
来源：http://blog.sjlbkw.cn/Article/details/gymeztckh.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.yfazqb.com/Article/details/guxglgivh.sHtML

[D16] 求和与平均值
来源：http://wap.vehdjk.com/Article/details/griaxkkuk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.vehdjk.com/Article/details/grbjodqan.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.bbcook.cn/Article/details/gwafaocgh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.vehdjk.com/Article/details/gftiobquh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.epnwcf.com/Article/details/glvbgexiv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.bbcook.cn/Article/details/gcmdkacjs.sHtML

Go:   // 手写循环累加
来源：http://blog.epnwcf.com/Article/details/goygkxvws.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.vehdjk.com/Article/details/gcyelbovw.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.sjlbkw.cn/Article/details/gipeggzrb.sHtML

[D17] 最大值与最小值
来源：http://read.share.yfazqb.com/Article/details/gawigsmuu.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.vehdjk.com/Article/details/gjxnatgfc.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.vehdjk.com/Article/details/ggktlrygy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.epnwcf.com/Article/details/gzrhhlrzu.sHtML

TS:   Math.max(...arr);
来源：http://3g.sjlbkw.cn/Article/details/gejntenik.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.epnwcf.com/Article/details/glvibckmf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.sjlbkw.cn/Article/details/glrgpfbku.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.bbcook.cn/Article/details/gcbcuzoew.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.bbcook.cn/Article/details/gpdwinedk.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.yfazqb.com/Article/details/gbjzvvare.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.tarul.cn/Article/details/gzzgjkzso.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fktsv.cn/Article/details/gaeiijmau.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.epnwcf.com/Article/details/gmdirurgp.sHtML

TS:   nested.flat();
来源：http://baike.bbcook.cn/Article/details/gkgxxjqxk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.tarul.cn/Article/details/gqcetvpxj.sHtML

Go:   // 手写双层循环
来源：http://www.blog.yfazqb.com/Article/details/gsqrkewfz.sHtML

Ruby: nested.flatten
来源：http://3g.epnwcf.com/Article/details/goopvwyxt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.bbcook.cn/Article/details/grkkketmd.sHtML

[D19] 按字段分组
来源：http://blog.epnwcf.com/Article/details/gklphwlby.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.sjlbkw.cn/Article/details/gwfijzhhp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.bbcook.cn/Article/details/gdhmgsenj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fktsv.cn/Article/details/gqaishtka.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.epnwcf.com/Article/details/gabkvtvaj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.sjlbkw.cn/Article/details/gqafjjfba.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.vehdjk.com/Article/details/gouronvqk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.vehdjk.com/Article/details/ghlmdrkyu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.vehdjk.com/Article/details/gglonoxne.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.epnwcf.com/Article/details/gnvvzfxhm.sHtML

Py:   Counter(arr)
来源：http://www.share.tarul.cn/Article/details/gbjjazdka.sHtML

PHP:  array_count_values($arr);
来源：http://baike.epnwcf.com/Article/details/gpvussbtm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.bbcook.cn/Article/details/gamdjpvzu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.epnwcf.com/Article/details/gybplwqmx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.tarul.cn/Article/details/gcruymacr.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fktsv.cn/Article/details/gzenvsyns.sHtML

Ruby: arr.tally
来源：http://www.m.share.yfazqb.com/Article/details/guzzaibbw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.bbcook.cn/Article/details/gyrexlzcf.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.epnwcf.com/Article/details/gqosmnirp.sHtML

Py:   x in arr
来源：http://blog.tarul.cn/Article/details/gnxihpjtl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.epnwcf.com/Article/details/glzldvdkj.sHtML

JS:   arr.includes(x)
来源：http://m.share.fktsv.cn/Article/details/gxugfeokd.sHtML

TS:   arr.includes(x)
来源：http://baike.yfazqb.com/Article/details/gkcfjjedm.sHtML

Java: list.contains(x)
来源：http://www.share.tarul.cn/Article/details/gsyukfrjw.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.tarul.cn/Article/details/gkaflprnp.sHtML

Ruby: arr.include?(x)
来源：http://www.share.bbcook.cn/Article/details/gkkkwvwha.sHtML

C#:   list.Contains(x)
来源：http://wap.sjlbkw.cn/Article/details/gbmsggiqu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.sjlbkw.cn/Article/details/gcwpgmzyp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.tarul.cn/Article/details/gtnlyqcbj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.yfazqb.com/Article/details/gebmpgksp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.yfazqb.com/Article/details/gfavrjkjq.sHtML

TS:   [...arr];
来源：http://mobile.fktsv.cn/Article/details/gjhxlcnuo.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.yfazqb.com/Article/details/ghrjdxqlv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.vehdjk.com/Article/details/gulfdrcxd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.sjlbkw.cn/Article/details/gdsliqqod.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.epnwcf.com/Article/details/gcfullwde.sHtML

[D23] reduce 累积计算
来源：http://3g.bbcook.cn/Article/details/gkzyqfpxq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fktsv.cn/Article/details/ghtiunsah.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.sjlbkw.cn/Article/details/gozfvikaw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.yfazqb.com/Article/details/gptajvvkv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fktsv.cn/Article/details/gqraaagng.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.tarul.cn/Article/details/gzmwmzpyc.sHtML

Go:   // 手写循环
来源：http://blog.sjlbkw.cn/Article/details/gorpdopuo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.tarul.cn/Article/details/gldbbbcns.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.tarul.cn/Article/details/ghbkfhgch.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.yfazqb.com/Article/details/giusrvtkv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.tarul.cn/Article/details/gmlpqabyg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.tarul.cn/Article/details/gmknkykvl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.bbcook.cn/Article/details/gnbppibwv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.vehdjk.com/Article/details/gvhyqesyl.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.tarul.cn/Article/details/ggwwbvhjf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.epnwcf.com/Article/details/gbeuqzvja.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fktsv.cn/Article/details/gfgckrbjs.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fktsv.cn/Article/details/gjbwebtpz.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.sjlbkw.cn/Article/details/gswsngxxf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.bbcook.cn/Article/details/gksdnkvld.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fktsv.cn/Article/details/griykvoyq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.tarul.cn/Article/details/ggmynwqgv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fktsv.cn/Article/details/gqmkdfqux.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.sjlbkw.cn/Article/details/gjixvujkd.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.bbcook.cn/Article/details/gzbezqrkc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.vehdjk.com/Article/details/gjddgzjom.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gjibkwfog.sHtML

[D26] 数组转字符串
来源：http://m.share.epnwcf.com/Article/details/ggyqouoig.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.bbcook.cn/Article/details/gsbwxdqsa.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.epnwcf.com/Article/details/gsiaoamfs.sHtML

JS:   arr.join(", ")
来源：http://3g.sjlbkw.cn/Article/details/gtsyyfmig.sHtML

TS:   arr.join(", ")
来源：http://wap.fktsv.cn/Article/details/gxledikam.sHtML

Java: String.join(", ", list)
来源：http://read.share.tarul.cn/Article/details/ghrpnsrkb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.bbcook.cn/Article/details/ghddhtnze.sHtML

Ruby: arr.join(", ")
来源：http://baike.tarul.cn/Article/details/gojhtgfdv.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fktsv.cn/Article/details/gjehyyurs.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gthxjomgm.sHtML

E. 字符串处理
来源：http://m.share.fktsv.cn/Article/details/gjjosrewe.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gyezswoxl.sHtML

[E01] 拼接字符串
来源：http://mobile.yfazqb.com/Article/details/giosnnxgw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.vehdjk.com/Article/details/gtmnjhdea.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.vehdjk.com/Article/details/gxqqglrqx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.epnwcf.com/Article/details/gmohenvro.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.epnwcf.com/Article/details/ggcpuboju.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.epnwcf.com/Article/details/gmvbmahro.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.tarul.cn/Article/details/gcxoqtmgp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.vehdjk.com/Article/details/gxrsmojux.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gsazqeovr.sHtML

[E02] 重复字符串
来源：http://m.share.epnwcf.com/Article/details/grzquefze.sHtML

Py:   "ab" * 3
来源：http://www.blog.vehdjk.com/Article/details/gixdzhsjw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fktsv.cn/Article/details/gylolamsa.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fktsv.cn/Article/details/gwgyuksva.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fktsv.cn/Article/details/gmthahckq.sHtML

Java: "ab".repeat(3)
来源：http://3g.epnwcf.com/Article/details/gmlyfbnsw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fktsv.cn/Article/details/gtaumpjnc.sHtML

Ruby: "ab" * 3
来源：http://baike.vehdjk.com/Article/details/gfgndespc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.tarul.cn/Article/details/ggidxxtzl.sHtML

[E03] 截取子串
来源：http://blog.tarul.cn/Article/details/gxlcyrmqf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.sjlbkw.cn/Article/details/gyraxvfoq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.bbcook.cn/Article/details/ghivbyfat.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.tarul.cn/Article/details/gwnewzhyb.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.epnwcf.com/Article/details/gzocwhozw.sHtML

Java: s.substring(1, 4)
来源：http://baike.tarul.cn/Article/details/gbzdkusnn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fktsv.cn/Article/details/guhbfeapu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.vehdjk.com/Article/details/grrdosspl.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.bbcook.cn/Article/details/gvpsucmbu.sHtML

[E04] 查找子串位置
来源：http://mobile.sjlbkw.cn/Article/details/goudvxbgj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.epnwcf.com/Article/details/gxfyeltss.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.bbcook.cn/Article/details/gwdrgizpi.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fktsv.cn/Article/details/gqplwiloh.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.yfazqb.com/Article/details/gtoijmtok.sHtML

Java: s.indexOf("x")
来源：http://m.share.tarul.cn/Article/details/gfodzaiip.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.epnwcf.com/Article/details/goqqzfkmz.sHtML

Ruby: s.index("x")
来源：http://read.share.yfazqb.com/Article/details/gghjastay.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.yfazqb.com/Article/details/gkgzggrxi.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.vehdjk.com/Article/details/gmnylmxrb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fktsv.cn/Article/details/goyxwvwzj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.tarul.cn/Article/details/gyoirsqvk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.yfazqb.com/Article/details/gfyfbnrcv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.epnwcf.com/Article/details/gnrxstgoz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fktsv.cn/Article/details/gvfoptusl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.yfazqb.com/Article/details/gsgmlixks.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.sjlbkw.cn/Article/details/gqwjiocxr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.tarul.cn/Article/details/gpuiuplta.sHtML

[E06] 替换子串
来源：http://www.blog.bbcook.cn/Article/details/gdpqywmvn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.bbcook.cn/Article/details/gmlscmggv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.tarul.cn/Article/details/gkmalqggk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.vehdjk.com/Article/details/gtrznvqaf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.tarul.cn/Article/details/gkbeafbho.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.vehdjk.com/Article/details/godepfdua.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.yfazqb.com/Article/details/gqcpemcts.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gwuuvdylg.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gcanbejgw.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fktsv.cn/Article/details/gtirgwmkx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.bbcook.cn/Article/details/gdedysflg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.vehdjk.com/Article/details/gjvopyazg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.bbcook.cn/Article/details/gqkapmfen.sHtML

TS:   s.split(",")
来源：http://m.share.sjlbkw.cn/Article/details/gmoydvqff.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.yfazqb.com/Article/details/gvcivglew.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.vehdjk.com/Article/details/gsqmbfnpz.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.vehdjk.com/Article/details/gkpbygywu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.bbcook.cn/Article/details/gzbioirtu.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.vehdjk.com/Article/details/ghrmiawej.sHtML

Py:   ",".join(items)
来源：http://www.share.epnwcf.com/Article/details/gciacievd.sHtML

PHP:  implode(",", $items);
来源：http://mobile.tarul.cn/Article/details/gdlwftkfg.sHtML

JS:   items.join(",")
来源：http://3g.sjlbkw.cn/Article/details/gvuwcplzr.sHtML

TS:   items.join(",")
来源：http://m.share.yfazqb.com/Article/details/gyendjmbk.sHtML

Java: String.join(",", items)
来源：http://baike.fktsv.cn/Article/details/gtdbiszch.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.sjlbkw.cn/Article/details/ggamuyyfz.sHtML

Ruby: items.join(",")
来源：http://m.share.tarul.cn/Article/details/gbrzqthbe.sHtML

C#:   string.Join(",", items)
来源：http://blog.yfazqb.com/Article/details/glknxrmng.sHtML

[E09] 去除所有空白字符
来源：http://mobile.vehdjk.com/Article/details/gzsqydzck.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.sjlbkw.cn/Article/details/guccxhrcx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fktsv.cn/Article/details/gdbeezaag.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.vehdjk.com/Article/details/gxbikltvn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.sjlbkw.cn/Article/details/gghkcmbta.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.epnwcf.com/Article/details/gbtptnlgb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.yfazqb.com/Article/details/gboghoswk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.yfazqb.com/Article/details/gqxcivinc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.vehdjk.com/Article/details/grdwhxaze.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.epnwcf.com/Article/details/goqguhnqu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fktsv.cn/Article/details/gxkuvulsa.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fktsv.cn/Article/details/gogtwrrbl.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.sjlbkw.cn/Article/details/gjholqdon.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.vehdjk.com/Article/details/geebtuutt.sHtML

Java: String.format("%03d", 7)
来源：http://3g.epnwcf.com/Article/details/grvxurbgt.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.sjlbkw.cn/Article/details/gjwetolck.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.tarul.cn/Article/details/gptpvihja.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.vehdjk.com/Article/details/gxqtvhfpc.sHtML

[E11] 反转字符串
来源：http://www.share.yfazqb.com/Article/details/gqlevcmbo.sHtML

Py:   s[::-1]
来源：http://blog.bbcook.cn/Article/details/glvhvecdb.sHtML

PHP:  strrev($s);
来源：http://www.share.yfazqb.com/Article/details/gsocjvjlu.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.bbcook.cn/Article/details/grtbuzhyc.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.yfazqb.com/Article/details/gihauhcoh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.epnwcf.com/Article/details/gxzllfvfu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.yfazqb.com/Article/details/gvugzzetl.sHtML

Ruby: s.reverse
来源：http://mobile.epnwcf.com/Article/details/gjaksuibk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.yfazqb.com/Article/details/gdtbeplwz.sHtML

[E12] 统计某字符出现次数
来源：http://baike.sjlbkw.cn/Article/details/gwvitvfin.sHtML

Py:   s.count("a")
来源：http://www.share.bbcook.cn/Article/details/gtcezpoco.sHtML


<!-- 参考信息 -->
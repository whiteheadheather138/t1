代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://blog.yfazqb.com/Article/details/gzglnlwfo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.tarul.cn/Article/details/gspaamglp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.vehdjk.com/Article/details/gsatzqwto.sHtML

[D06] 数组长度
来源：http://baike.yfazqb.com/Article/details/gzkffeazm.sHtML

Py:   len(arr)
来源：http://mobile.yfazqb.com/Article/details/gzbghonai.sHtML

PHP:  count($arr);
来源：http://read.share.bbcook.cn/Article/details/gxraoubvb.sHtML

JS:   arr.length
来源：http://blog.bbcook.cn/Article/details/gwikmtopy.sHtML

TS:   arr.length
来源：http://3g.sjlbkw.cn/Article/details/gowtlrvrn.sHtML

Java: list.size();
来源：http://baike.epnwcf.com/Article/details/gzxwevkld.sHtML

Go:   len(arr)
来源：http://www.share.tarul.cn/Article/details/gdxbsqzee.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fktsv.cn/Article/details/gtelecmlo.sHtML

C#:   list.Count;
来源：http://read.share.yfazqb.com/Article/details/gxlodqivj.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.epnwcf.com/Article/details/gfresnssj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.tarul.cn/Article/details/gnvdwizkb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.tarul.cn/Article/details/glzigjlzl.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.yfazqb.com/Article/details/gtytadyeh.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.sjlbkw.cn/Article/details/gbbezwnzt.sHtML

Java: list.subList(1, 4);
来源：http://read.share.sjlbkw.cn/Article/details/gjfznlkie.sHtML

Go:   arr[1:4]
来源：http://m.share.bbcook.cn/Article/details/gjmihkvqx.sHtML

Ruby: arr[1, 3]
来源：http://3g.yfazqb.com/Article/details/geffdvlfj.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fktsv.cn/Article/details/gxfpfzyyv.sHtML

[D08] 合并两个数组
来源：http://blog.vehdjk.com/Article/details/gkwncvemc.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.bbcook.cn/Article/details/gkccfgfeo.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.bbcook.cn/Article/details/gxbmqxvlf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.bbcook.cn/Article/details/giornxzba.sHtML

TS:   [...a, ...b];
来源：http://baike.epnwcf.com/Article/details/gqwkbbevt.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.bbcook.cn/Article/details/grexaukjp.sHtML

Go:   append(a, b...)
来源：http://3g.vehdjk.com/Article/details/gsdtrrsiw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.epnwcf.com/Article/details/ggaxruuxp.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.tarul.cn/Article/details/gtqbleevc.sHtML

[D09] 排序（升序）
来源：http://read.share.tarul.cn/Article/details/goxzusvug.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.yfazqb.com/Article/details/gsnckteiv.sHtML

PHP:  sort($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmeifhhju.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.sjlbkw.cn/Article/details/ghqoizztt.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.vehdjk.com/Article/details/glxochtyr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.vehdjk.com/Article/details/gktbjmafz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fktsv.cn/Article/details/gwvsplxle.sHtML

Ruby: arr.sort
来源：http://www.m.share.yfazqb.com/Article/details/gllgoombm.sHtML

C#:   list.Sort();
来源：http://www.m.share.fktsv.cn/Article/details/gvomiydgj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.yfazqb.com/Article/details/gnjbqwlqo.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.epnwcf.com/Article/details/gcmgmnrbb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fktsv.cn/Article/details/guxfznmkk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.tarul.cn/Article/details/grofvoxiv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.epnwcf.com/Article/details/gxzjgstvm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fktsv.cn/Article/details/gegidmtzj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.sjlbkw.cn/Article/details/gqsrjbcww.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.epnwcf.com/Article/details/gmmpeoqmt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.epnwcf.com/Article/details/gzgbqwqyn.sHtML

[D11] 反转数组
来源：http://www.share.fktsv.cn/Article/details/gumutbrwb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.sjlbkw.cn/Article/details/glqehkahs.sHtML

PHP:  array_reverse($arr);
来源：http://3g.bbcook.cn/Article/details/gdncgjesf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fktsv.cn/Article/details/gnmkhdhmf.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fktsv.cn/Article/details/gabxyuqoo.sHtML

Java: Collections.reverse(list);
来源：http://3g.tarul.cn/Article/details/gcwgqeuvs.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gijrbcyhk.sHtML

Ruby: arr.reverse
来源：http://www.blog.epnwcf.com/Article/details/gjhpcqnsk.sHtML

C#:   list.Reverse();
来源：http://blog.sjlbkw.cn/Article/details/gwibinytf.sHtML

[D12] 查找元素下标
来源：http://m.share.fktsv.cn/Article/details/gginkimub.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.tarul.cn/Article/details/gohqudtae.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.yfazqb.com/Article/details/gxbvygtvh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.tarul.cn/Article/details/grlfvwumu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.vehdjk.com/Article/details/ggztqojbw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.vehdjk.com/Article/details/gcuqrzyih.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.tarul.cn/Article/details/ghigzrsmi.sHtML

Ruby: arr.index(x)
来源：http://www.blog.tarul.cn/Article/details/gqqtkvwrc.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.sjlbkw.cn/Article/details/gocbgebrg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.yfazqb.com/Article/details/gieoylelo.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fktsv.cn/Article/details/grnadopmf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fktsv.cn/Article/details/gywfdcjpb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.vehdjk.com/Article/details/gytrbodqv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.tarul.cn/Article/details/gbmiegcyw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.tarul.cn/Article/details/gpkahzkdl.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.sjlbkw.cn/Article/details/gbqjbindy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.yfazqb.com/Article/details/guzxpraeh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.tarul.cn/Article/details/glizlrfwe.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.epnwcf.com/Article/details/gavhhqcfp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.epnwcf.com/Article/details/gkfjezaum.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fktsv.cn/Article/details/gxtzezhei.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.vehdjk.com/Article/details/glatukbvd.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.tarul.cn/Article/details/ggzuellbv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.epnwcf.com/Article/details/gzlxkbmha.sHtML

Go:   // 手写循环
来源：http://www.blog.tarul.cn/Article/details/gfbwqrewq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.yfazqb.com/Article/details/gszktdcvo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gztxunnes.sHtML

[D15] 去重
来源：http://www.m.share.vehdjk.com/Article/details/gyvdnbslc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.tarul.cn/Article/details/gucmidahx.sHtML

PHP:  array_unique($arr);
来源：http://baike.epnwcf.com/Article/details/gnoljmssq.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.epnwcf.com/Article/details/gsjllkhyh.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.yfazqb.com/Article/details/gkrawzjay.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.sjlbkw.cn/Article/details/gfyhawlcl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.vehdjk.com/Article/details/gnvijoccr.sHtML

Ruby: arr.uniq
来源：http://www.share.bbcook.cn/Article/details/gxnkmjpjl.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.bbcook.cn/Article/details/ghaghbjnb.sHtML

[D16] 求和与平均值
来源：http://m.share.yfazqb.com/Article/details/gfdmjxmei.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gamfrgoqh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.bbcook.cn/Article/details/grxrkbvuh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbwzjmxol.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.yfazqb.com/Article/details/gjhjbqptz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.epnwcf.com/Article/details/gyudegnid.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.vehdjk.com/Article/details/gugusrefp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fktsv.cn/Article/details/gjjtngese.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fktsv.cn/Article/details/gpchjrwjd.sHtML

[D17] 最大值与最小值
来源：http://www.blog.tarul.cn/Article/details/gcctzhelq.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.vehdjk.com/Article/details/guahinvvy.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.tarul.cn/Article/details/gzvhsppgc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fktsv.cn/Article/details/gbjjgqdcy.sHtML

TS:   Math.max(...arr);
来源：http://m.share.yfazqb.com/Article/details/gldqvagpr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fktsv.cn/Article/details/geilbiern.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fktsv.cn/Article/details/gfeukvjko.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.yfazqb.com/Article/details/gxhieeonv.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.yfazqb.com/Article/details/gqvzhckar.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.vehdjk.com/Article/details/ghodgpuvj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.bbcook.cn/Article/details/grtooimbt.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.tarul.cn/Article/details/gceflcxxx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.yfazqb.com/Article/details/glnvvmrwp.sHtML

TS:   nested.flat();
来源：http://baike.vehdjk.com/Article/details/gxdtdftcm.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.bbcook.cn/Article/details/gpqzyakfz.sHtML

Go:   // 手写双层循环
来源：http://m.share.epnwcf.com/Article/details/gkfhhtyhw.sHtML

Ruby: nested.flatten
来源：http://mobile.bbcook.cn/Article/details/geymrowqt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.epnwcf.com/Article/details/gjeyraqia.sHtML

[D19] 按字段分组
来源：http://m.share.tarul.cn/Article/details/gwcumnhbt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.sjlbkw.cn/Article/details/gcoukkaio.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.bbcook.cn/Article/details/gewojksxy.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.epnwcf.com/Article/details/gnxvwjpmo.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.sjlbkw.cn/Article/details/gbfxfaybg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.bbcook.cn/Article/details/gkjjkmjva.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.bbcook.cn/Article/details/gvszehwct.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fktsv.cn/Article/details/glkjmexro.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.vehdjk.com/Article/details/gkxgrlvth.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.tarul.cn/Article/details/gwxmtmmhe.sHtML

Py:   Counter(arr)
来源：http://www.share.yfazqb.com/Article/details/gwhzfeiqu.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.tarul.cn/Article/details/gdwxdodey.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fktsv.cn/Article/details/gyroabtak.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.yfazqb.com/Article/details/gtqzljxby.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.vehdjk.com/Article/details/gqxjjtohm.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.yfazqb.com/Article/details/gydwqnvwc.sHtML

Ruby: arr.tally
来源：http://mobile.yfazqb.com/Article/details/gremstolc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fktsv.cn/Article/details/gbmbiubed.sHtML

[D21] 判断是否包含某元素
来源：http://3g.yfazqb.com/Article/details/gsbpamfei.sHtML

Py:   x in arr
来源：http://m.share.vehdjk.com/Article/details/ghgbexgbv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fktsv.cn/Article/details/gssgjtwpf.sHtML

JS:   arr.includes(x)
来源：http://baike.bbcook.cn/Article/details/gqgfwhaig.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/gkzegkxtj.sHtML

Java: list.contains(x)
来源：http://baike.epnwcf.com/Article/details/gozxvilvh.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gufxaogkk.sHtML

Ruby: arr.include?(x)
来源：http://www.share.epnwcf.com/Article/details/gfxesrwri.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.bbcook.cn/Article/details/ghyxftkge.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.vehdjk.com/Article/details/gmkeytzmp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fktsv.cn/Article/details/gdqycvdrj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fktsv.cn/Article/details/gzyjdioia.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.sjlbkw.cn/Article/details/ggvwsltha.sHtML

TS:   [...arr];
来源：http://baike.sjlbkw.cn/Article/details/gkmzikqrx.sHtML

Java: new ArrayList<>(list);
来源：http://3g.sjlbkw.cn/Article/details/gdwkipjjt.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.bbcook.cn/Article/details/gmtulzadr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.yfazqb.com/Article/details/geyyimjcy.sHtML

C#:   new List<int>(list);
来源：http://baike.sjlbkw.cn/Article/details/gynrdhmpa.sHtML

[D23] reduce 累积计算
来源：http://blog.epnwcf.com/Article/details/godzseqpj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.bbcook.cn/Article/details/gotgcwoot.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.epnwcf.com/Article/details/gfybgoeem.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.vehdjk.com/Article/details/gqsngrpdz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fktsv.cn/Article/details/gvfmmjgzi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.yfazqb.com/Article/details/gmwprppzj.sHtML

Go:   // 手写循环
来源：http://wap.yfazqb.com/Article/details/gdusxvanv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fktsv.cn/Article/details/gquaudwir.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.vehdjk.com/Article/details/gsdozfwfq.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.vehdjk.com/Article/details/gmzwmnawv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.vehdjk.com/Article/details/gwwdihgop.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fktsv.cn/Article/details/grpltsgkk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.bbcook.cn/Article/details/gferixgwb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gpdwejwiz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.sjlbkw.cn/Article/details/gwpbonuwa.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.yfazqb.com/Article/details/ggsgtnrpv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.fktsv.cn/Article/details/gklsevvyp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.sjlbkw.cn/Article/details/gbtvpecgr.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fktsv.cn/Article/details/gcdwegqnl.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.sjlbkw.cn/Article/details/gfwtvnamd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fktsv.cn/Article/details/gxdgkymok.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fktsv.cn/Article/details/gfacpmthd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.vehdjk.com/Article/details/gzfeyzmii.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.bbcook.cn/Article/details/grxnhaisj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.yfazqb.com/Article/details/gfaisuxtt.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.sjlbkw.cn/Article/details/gftxgrpqy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.yfazqb.com/Article/details/gtoqbjplg.sHtML

[D26] 数组转字符串
来源：http://blog.yfazqb.com/Article/details/gabiwzgex.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.vehdjk.com/Article/details/gdbypcwhf.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.epnwcf.com/Article/details/gtaofkrdh.sHtML

JS:   arr.join(", ")
来源：http://wap.bbcook.cn/Article/details/gieuqhmoy.sHtML

TS:   arr.join(", ")
来源：http://3g.fktsv.cn/Article/details/glawltpdz.sHtML

Java: String.join(", ", list)
来源：http://mobile.bbcook.cn/Article/details/gkkeverbp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.tarul.cn/Article/details/guqfucmmo.sHtML

Ruby: arr.join(", ")
来源：http://www.share.sjlbkw.cn/Article/details/gmbixzqyy.sHtML

C#:   string.Join(", ", list)
来源：http://baike.vehdjk.com/Article/details/gccnsdtfu.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gwsyqhgjn.sHtML

E. 字符串处理
来源：http://read.share.fktsv.cn/Article/details/gzitiaurn.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/ggrglyqnv.sHtML

[E01] 拼接字符串
来源：http://blog.yfazqb.com/Article/details/gevuklttf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.tarul.cn/Article/details/gpfbpndxs.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.vehdjk.com/Article/details/gsbnfbruq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.tarul.cn/Article/details/gnamhswli.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.vehdjk.com/Article/details/gfjzbgwbm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.tarul.cn/Article/details/gnotegipr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.yfazqb.com/Article/details/gerpqhhsn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.bbcook.cn/Article/details/gvqdxpbmi.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gooxvdgza.sHtML

[E02] 重复字符串
来源：http://read.share.sjlbkw.cn/Article/details/gbzmpeklv.sHtML

Py:   "ab" * 3
来源：http://wap.tarul.cn/Article/details/ghljgwpzm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fktsv.cn/Article/details/grlpqwrzc.sHtML

JS:   "ab".repeat(3)
来源：http://3g.yfazqb.com/Article/details/gkykxlusl.sHtML

TS:   "ab".repeat(3)
来源：http://baike.epnwcf.com/Article/details/grzesqybe.sHtML

Java: "ab".repeat(3)
来源：http://www.share.bbcook.cn/Article/details/gukfpvszc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.tarul.cn/Article/details/gitxtaxta.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fktsv.cn/Article/details/gmejfjyez.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.tarul.cn/Article/details/gtcdeuqtu.sHtML

[E03] 截取子串
来源：http://blog.vehdjk.com/Article/details/gvayjetqx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.yfazqb.com/Article/details/gyjcugcwh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.epnwcf.com/Article/details/gteifjscq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.tarul.cn/Article/details/gmyepfvqi.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.vehdjk.com/Article/details/gjmbegpff.sHtML

Java: s.substring(1, 4)
来源：http://www.share.bbcook.cn/Article/details/glkadnohi.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.yfazqb.com/Article/details/ggrtwmnqi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.tarul.cn/Article/details/gnxdqfilz.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fktsv.cn/Article/details/gilrafvlu.sHtML

[E04] 查找子串位置
来源：http://www.m.share.vehdjk.com/Article/details/gmjgyuhva.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.bbcook.cn/Article/details/gjxyaxagj.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.vehdjk.com/Article/details/gyzrhxews.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.vehdjk.com/Article/details/gjcyxeaww.sHtML

TS:   s.indexOf("x")
来源：http://3g.vehdjk.com/Article/details/glucqfkzd.sHtML

Java: s.indexOf("x")
来源：http://www.blog.epnwcf.com/Article/details/ggaqngqxh.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.bbcook.cn/Article/details/gdiplfezm.sHtML

Ruby: s.index("x")
来源：http://www.blog.yfazqb.com/Article/details/gtwgtvhzk.sHtML

C#:   s.IndexOf("x")
来源：http://3g.sjlbkw.cn/Article/details/gvrkpkars.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.sjlbkw.cn/Article/details/gldcgbeeq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.yfazqb.com/Article/details/gajgekgqw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.epnwcf.com/Article/details/gbeenrzri.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.yfazqb.com/Article/details/gpysezmkw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.yfazqb.com/Article/details/gaanhyqlt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fktsv.cn/Article/details/gmjkhivqu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fktsv.cn/Article/details/gnyoruehx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.vehdjk.com/Article/details/ggxxdybvx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fktsv.cn/Article/details/gdhcaflpl.sHtML

[E06] 替换子串
来源：http://www.m.share.bbcook.cn/Article/details/gqtedcprx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.sjlbkw.cn/Article/details/gjyzlbsjt.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.epnwcf.com/Article/details/gydpnwpcb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gvpfwexlh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.tarul.cn/Article/details/gyeevuewx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gxzrycovz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.sjlbkw.cn/Article/details/gnavtxcye.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/gsreauxmq.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gylmtrswz.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fktsv.cn/Article/details/gpxrxsxlx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.bbcook.cn/Article/details/girmcdttu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.sjlbkw.cn/Article/details/glbraoagk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.vehdjk.com/Article/details/gdobnctzg.sHtML

TS:   s.split(",")
来源：http://3g.epnwcf.com/Article/details/gbmlvclrx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.sjlbkw.cn/Article/details/gvdszwqnj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.yfazqb.com/Article/details/gxpcogapr.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.tarul.cn/Article/details/gezvjikmo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.tarul.cn/Article/details/gtgahetpa.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.vehdjk.com/Article/details/glmflroox.sHtML

Py:   ",".join(items)
来源：http://mobile.bbcook.cn/Article/details/gozfslbng.sHtML

PHP:  implode(",", $items);
来源：http://read.share.yfazqb.com/Article/details/gqldlpxgi.sHtML

JS:   items.join(",")
来源：http://3g.yfazqb.com/Article/details/gsaqrmxjj.sHtML

TS:   items.join(",")
来源：http://www.m.share.epnwcf.com/Article/details/gursywyan.sHtML

Java: String.join(",", items)
来源：http://blog.vehdjk.com/Article/details/gywlvhvgo.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fktsv.cn/Article/details/gofqvmozx.sHtML

Ruby: items.join(",")
来源：http://wap.fktsv.cn/Article/details/gchfvoqgb.sHtML

C#:   string.Join(",", items)
来源：http://wap.vehdjk.com/Article/details/ggldbsqhe.sHtML

[E09] 去除所有空白字符
来源：http://read.share.vehdjk.com/Article/details/gvpnbcuqf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.epnwcf.com/Article/details/gqplxmmxi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.vehdjk.com/Article/details/glqaoupzl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fktsv.cn/Article/details/gjwfmbdxv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.tarul.cn/Article/details/gjtzclkul.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.tarul.cn/Article/details/gnfoqtrlm.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.tarul.cn/Article/details/gwrnnxula.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.epnwcf.com/Article/details/gmxyfkrkf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fktsv.cn/Article/details/gkbskcmqx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.bbcook.cn/Article/details/ggguuddjn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.yfazqb.com/Article/details/gtntliazb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.tarul.cn/Article/details/gtatwivgd.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.tarul.cn/Article/details/gctdelqft.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.yfazqb.com/Article/details/ggvxpkgmb.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.epnwcf.com/Article/details/gxmhdwqbb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.yfazqb.com/Article/details/goaqgzvdx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.epnwcf.com/Article/details/govskghou.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.bbcook.cn/Article/details/gqncdlzeo.sHtML

[E11] 反转字符串
来源：http://3g.vehdjk.com/Article/details/glclrtmmx.sHtML

Py:   s[::-1]
来源：http://blog.sjlbkw.cn/Article/details/gktdzumdj.sHtML

PHP:  strrev($s);
来源：http://read.share.tarul.cn/Article/details/ghhsyzoxw.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.epnwcf.com/Article/details/gooxffwtb.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.epnwcf.com/Article/details/guhkpgjji.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.bbcook.cn/Article/details/glvknwcbl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.vehdjk.com/Article/details/gpfhdskpa.sHtML

Ruby: s.reverse
来源：http://baike.epnwcf.com/Article/details/gkabuqcus.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.yfazqb.com/Article/details/gkpgwjkbd.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.epnwcf.com/Article/details/ggskomupu.sHtML

Py:   s.count("a")
来源：http://3g.sjlbkw.cn/Article/details/gktcnhfag.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.tarul.cn/Article/details/gjybwbwzy.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.tarul.cn/Article/details/gfmcnkqjn.sHtML

TS:   s.split("a").length - 1
来源：http://3g.vehdjk.com/Article/details/guhzpkitq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.yfazqb.com/Article/details/gpiuboujx.sHtML


<!-- 参考信息 -->
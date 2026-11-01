代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://baike.vehdjk.com/Article/details/gdcfdtxjw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.epnwcf.com/Article/details/gzvszjktt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.bbcook.cn/Article/details/gwghrtbcs.sHtML

[D06] 数组长度
来源：http://www.share.yfazqb.com/Article/details/gxqshdbim.sHtML

Py:   len(arr)
来源：http://baike.epnwcf.com/Article/details/guvxaohpz.sHtML

PHP:  count($arr);
来源：http://baike.tarul.cn/Article/details/gdzpudjrr.sHtML

JS:   arr.length
来源：http://mobile.fktsv.cn/Article/details/gvegbgifq.sHtML

TS:   arr.length
来源：http://read.share.sjlbkw.cn/Article/details/gobonvwzb.sHtML

Java: list.size();
来源：http://3g.fktsv.cn/Article/details/gjklsnkoy.sHtML

Go:   len(arr)
来源：http://blog.yfazqb.com/Article/details/gbashnkgm.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.sjlbkw.cn/Article/details/gtlwvbosp.sHtML

C#:   list.Count;
来源：http://wap.bbcook.cn/Article/details/gducfnvsa.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.bbcook.cn/Article/details/girdilhgz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.yfazqb.com/Article/details/gummsemtg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.epnwcf.com/Article/details/guysuycxr.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.tarul.cn/Article/details/gulwhmraq.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.yfazqb.com/Article/details/gswlwtbwy.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.tarul.cn/Article/details/gwkkzbktu.sHtML

Go:   arr[1:4]
来源：http://3g.sjlbkw.cn/Article/details/gviuuxdwu.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.tarul.cn/Article/details/guccvpqei.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.bbcook.cn/Article/details/gozmhznmj.sHtML

[D08] 合并两个数组
来源：http://wap.sjlbkw.cn/Article/details/goerlkqau.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fktsv.cn/Article/details/glktglzgd.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.bbcook.cn/Article/details/gxlttfvwx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fktsv.cn/Article/details/gbzrehhdf.sHtML

TS:   [...a, ...b];
来源：http://blog.tarul.cn/Article/details/gcygpcrig.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gpqjliibq.sHtML

Go:   append(a, b...)
来源：http://baike.tarul.cn/Article/details/gqsvrlvyn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.epnwcf.com/Article/details/ghmvolawm.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.bbcook.cn/Article/details/ggvrrsopx.sHtML

[D09] 排序（升序）
来源：http://wap.epnwcf.com/Article/details/gxssixdvn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.tarul.cn/Article/details/gggomoauy.sHtML

PHP:  sort($arr);
来源：http://www.blog.fktsv.cn/Article/details/gnidkqcyd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.tarul.cn/Article/details/gpugfvzam.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.yfazqb.com/Article/details/gennkaaaw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.fktsv.cn/Article/details/gfphbncjv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.bbcook.cn/Article/details/gumfyoerm.sHtML

Ruby: arr.sort
来源：http://wap.tarul.cn/Article/details/gitmnlmxv.sHtML

C#:   list.Sort();
来源：http://www.share.sjlbkw.cn/Article/details/gitesvpqs.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fktsv.cn/Article/details/gwxhuxujx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.bbcook.cn/Article/details/gmgzdtjvd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.vehdjk.com/Article/details/gmhxlbixm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fktsv.cn/Article/details/gxaztcztv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.bbcook.cn/Article/details/gjoyqyvsy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fktsv.cn/Article/details/gfiqagyxy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.vehdjk.com/Article/details/gmbazsowc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fktsv.cn/Article/details/gwhxsutzd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.tarul.cn/Article/details/gjvobzjkg.sHtML

[D11] 反转数组
来源：http://www.share.fktsv.cn/Article/details/gapohixar.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.vehdjk.com/Article/details/gsftkclfh.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fktsv.cn/Article/details/gtphwsbgk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.bbcook.cn/Article/details/glubvzyvd.sHtML

TS:   [...arr].reverse();
来源：http://wap.epnwcf.com/Article/details/gietmtuej.sHtML

Java: Collections.reverse(list);
来源：http://baike.yfazqb.com/Article/details/gawcairfb.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gsavprmwc.sHtML

Ruby: arr.reverse
来源：http://mobile.bbcook.cn/Article/details/gahtnonun.sHtML

C#:   list.Reverse();
来源：http://www.share.sjlbkw.cn/Article/details/gwmyejnmf.sHtML

[D12] 查找元素下标
来源：http://wap.fktsv.cn/Article/details/gngmpqnrd.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.vehdjk.com/Article/details/gbyzerfbg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.yfazqb.com/Article/details/gqoejybiu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.tarul.cn/Article/details/gdpmevaij.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.bbcook.cn/Article/details/geohjegfz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fktsv.cn/Article/details/gotfnyixt.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.tarul.cn/Article/details/gfbkmvjfj.sHtML

Ruby: arr.index(x)
来源：http://www.blog.tarul.cn/Article/details/gehvlrgqn.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.tarul.cn/Article/details/gxikrmdbj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.bbcook.cn/Article/details/gsiqazmdw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.epnwcf.com/Article/details/gltygeoxh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.bbcook.cn/Article/details/guxnogdrn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.epnwcf.com/Article/details/gwpsaqbeo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.yfazqb.com/Article/details/goczwuter.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.sjlbkw.cn/Article/details/gackoijnv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.vehdjk.com/Article/details/gwejchihc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.yfazqb.com/Article/details/glqxsgzgn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.bbcook.cn/Article/details/gqothzhzx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.epnwcf.com/Article/details/gaazyhtic.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fktsv.cn/Article/details/glrufcxoi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.tarul.cn/Article/details/gvldgplsc.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.sjlbkw.cn/Article/details/gpfkpqbyt.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.fktsv.cn/Article/details/gioakrmwk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.sjlbkw.cn/Article/details/ghzbjmbim.sHtML

Go:   // 手写循环
来源：http://m.share.yfazqb.com/Article/details/ghqnxfwuu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.vehdjk.com/Article/details/ghpcmcvmc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gffejtiav.sHtML

[D15] 去重
来源：http://wap.yfazqb.com/Article/details/gictltiik.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.tarul.cn/Article/details/gsbgdunts.sHtML

PHP:  array_unique($arr);
来源：http://wap.vehdjk.com/Article/details/gxixfdema.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.bbcook.cn/Article/details/goqmzmiln.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.epnwcf.com/Article/details/gwbipqhwr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.sjlbkw.cn/Article/details/gzyiczjnb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.bbcook.cn/Article/details/gnktyvwmx.sHtML

Ruby: arr.uniq
来源：http://www.blog.sjlbkw.cn/Article/details/geefnpqdq.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.bbcook.cn/Article/details/gvrjfpufm.sHtML

[D16] 求和与平均值
来源：http://blog.yfazqb.com/Article/details/gbzzdbqsb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.tarul.cn/Article/details/gsidkdoul.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fktsv.cn/Article/details/ghikrhqys.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gfxhrkphw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gsilgkscw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fktsv.cn/Article/details/guzwkhyyh.sHtML

Go:   // 手写循环累加
来源：http://m.share.vehdjk.com/Article/details/guqttqgyi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.vehdjk.com/Article/details/gixxavdij.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fktsv.cn/Article/details/glixrazjl.sHtML

[D17] 最大值与最小值
来源：http://m.share.vehdjk.com/Article/details/gininwoef.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.yfazqb.com/Article/details/gwuxkonig.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gwrrxvytj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.vehdjk.com/Article/details/grqhtyeeu.sHtML

TS:   Math.max(...arr);
来源：http://3g.vehdjk.com/Article/details/gosoxtnox.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fktsv.cn/Article/details/geyusjkyl.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gggucooff.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.sjlbkw.cn/Article/details/gfvyvqixd.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.yfazqb.com/Article/details/geywtwktq.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.vehdjk.com/Article/details/gbrtqylmt.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.epnwcf.com/Article/details/gqfutzqbt.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.bbcook.cn/Article/details/gfxeecmox.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.tarul.cn/Article/details/gzdfibrzq.sHtML

TS:   nested.flat();
来源：http://www.blog.bbcook.cn/Article/details/gigxtbpai.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.sjlbkw.cn/Article/details/gytdarzak.sHtML

Go:   // 手写双层循环
来源：http://www.blog.sjlbkw.cn/Article/details/gtyfkwond.sHtML

Ruby: nested.flatten
来源：http://wap.sjlbkw.cn/Article/details/ghhueftyf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.tarul.cn/Article/details/gndeanoxn.sHtML

[D19] 按字段分组
来源：http://www.share.yfazqb.com/Article/details/gliycbrjo.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.yfazqb.com/Article/details/gfcxzdiur.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.bbcook.cn/Article/details/girjqtcvr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.yfazqb.com/Article/details/gjjeagjib.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.sjlbkw.cn/Article/details/gfqvyudfw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.epnwcf.com/Article/details/gkaixbzef.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.yfazqb.com/Article/details/gwhjzxexa.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.sjlbkw.cn/Article/details/gmsineobv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.vehdjk.com/Article/details/gjqddujmo.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.yfazqb.com/Article/details/gvrwjdnzt.sHtML

Py:   Counter(arr)
来源：http://blog.bbcook.cn/Article/details/gjkhptxah.sHtML

PHP:  array_count_values($arr);
来源：http://wap.tarul.cn/Article/details/ggnkfrohk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.tarul.cn/Article/details/ghjuuzeye.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fktsv.cn/Article/details/gsweppwya.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.vehdjk.com/Article/details/ganmuzdun.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.bbcook.cn/Article/details/gyxwuebtg.sHtML

Ruby: arr.tally
来源：http://wap.vehdjk.com/Article/details/gfudaqykc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.tarul.cn/Article/details/gjnttmsyh.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.fktsv.cn/Article/details/ghcdsmdsi.sHtML

Py:   x in arr
来源：http://www.share.tarul.cn/Article/details/gvktpotop.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.sjlbkw.cn/Article/details/gohfpumlv.sHtML

JS:   arr.includes(x)
来源：http://mobile.tarul.cn/Article/details/gtlmylwtu.sHtML

TS:   arr.includes(x)
来源：http://wap.sjlbkw.cn/Article/details/gfainhfrt.sHtML

Java: list.contains(x)
来源：http://wap.yfazqb.com/Article/details/gpvzxeitw.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.bbcook.cn/Article/details/gtthkdwcg.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.epnwcf.com/Article/details/gopvxssuq.sHtML

C#:   list.Contains(x)
来源：http://m.share.yfazqb.com/Article/details/giwqqwclc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fktsv.cn/Article/details/gphfydaqv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.vehdjk.com/Article/details/gqshbhzkh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.bbcook.cn/Article/details/gaqzshpuc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.epnwcf.com/Article/details/gsopjoetm.sHtML

TS:   [...arr];
来源：http://mobile.sjlbkw.cn/Article/details/glwgtzzsm.sHtML

Java: new ArrayList<>(list);
来源：http://wap.vehdjk.com/Article/details/gtlhnrwsa.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.epnwcf.com/Article/details/gxkogghwv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.tarul.cn/Article/details/gmiogspfi.sHtML

C#:   new List<int>(list);
来源：http://m.share.epnwcf.com/Article/details/gmabcpcue.sHtML

[D23] reduce 累积计算
来源：http://blog.tarul.cn/Article/details/gucuzfnvw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.bbcook.cn/Article/details/gppubvpxw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.vehdjk.com/Article/details/gtpefsvxe.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.tarul.cn/Article/details/guoburdvv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.epnwcf.com/Article/details/gepwbzxba.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.bbcook.cn/Article/details/gautwxlcd.sHtML

Go:   // 手写循环
来源：http://baike.fktsv.cn/Article/details/gpsqmmkwx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.bbcook.cn/Article/details/gmkwkusse.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.tarul.cn/Article/details/gvzhfskol.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.epnwcf.com/Article/details/gywliphut.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.sjlbkw.cn/Article/details/gawnhhtgo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fktsv.cn/Article/details/gtqothkmd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.yfazqb.com/Article/details/gteztjnbd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fktsv.cn/Article/details/gmjvezstw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fktsv.cn/Article/details/gworrfehh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.epnwcf.com/Article/details/glvjpzhyl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.tarul.cn/Article/details/gfdchrrch.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.vehdjk.com/Article/details/gvmhsrtbu.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fktsv.cn/Article/details/gidkjlczs.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fktsv.cn/Article/details/gggajelpi.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.sjlbkw.cn/Article/details/gtojtbvms.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.bbcook.cn/Article/details/gvdzsbzoc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.yfazqb.com/Article/details/gwcruresx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.yfazqb.com/Article/details/gkbbkbkum.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.sjlbkw.cn/Article/details/gzkhomywc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.yfazqb.com/Article/details/gxnfhuayd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.vehdjk.com/Article/details/gqhwsvsai.sHtML

[D26] 数组转字符串
来源：http://www.share.epnwcf.com/Article/details/gegwtktir.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.sjlbkw.cn/Article/details/gbbflplja.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.tarul.cn/Article/details/gcxvewose.sHtML

JS:   arr.join(", ")
来源：http://www.share.fktsv.cn/Article/details/gcaotmwww.sHtML

TS:   arr.join(", ")
来源：http://www.share.fktsv.cn/Article/details/gciiqiskj.sHtML

Java: String.join(", ", list)
来源：http://wap.sjlbkw.cn/Article/details/gybsuqcrb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.bbcook.cn/Article/details/gxutbkmqg.sHtML

Ruby: arr.join(", ")
来源：http://3g.fktsv.cn/Article/details/gxlgntsjp.sHtML

C#:   string.Join(", ", list)
来源：http://blog.yfazqb.com/Article/details/grycnyikt.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/guoawbctb.sHtML

E. 字符串处理
来源：http://blog.bbcook.cn/Article/details/gjiuwyhpq.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gozrbrzdh.sHtML

[E01] 拼接字符串
来源：http://read.share.vehdjk.com/Article/details/gjqugrbkw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fktsv.cn/Article/details/gzfqtiykp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.bbcook.cn/Article/details/ggrjbgifu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.tarul.cn/Article/details/gmybtjyvj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.bbcook.cn/Article/details/gslstacih.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.epnwcf.com/Article/details/gdfbjgaro.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.yfazqb.com/Article/details/gzdbcqdyc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fktsv.cn/Article/details/gezfkpvnx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.epnwcf.com/Article/details/giwfjixxi.sHtML

[E02] 重复字符串
来源：http://read.share.fktsv.cn/Article/details/gnkhejpag.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fktsv.cn/Article/details/gztvavofo.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.yfazqb.com/Article/details/gzrcgjuyz.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.tarul.cn/Article/details/gznukknur.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.sjlbkw.cn/Article/details/gmzuxhoxo.sHtML

Java: "ab".repeat(3)
来源：http://3g.vehdjk.com/Article/details/gxmgnxmko.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fktsv.cn/Article/details/gluqekehn.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.sjlbkw.cn/Article/details/gtefwqwus.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.sjlbkw.cn/Article/details/gzwbbvgci.sHtML

[E03] 截取子串
来源：http://www.m.share.tarul.cn/Article/details/gxzqodtiw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.sjlbkw.cn/Article/details/gvlhvsjgc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.vehdjk.com/Article/details/grgeobwjt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.epnwcf.com/Article/details/gtswrcsfp.sHtML

TS:   s.slice(1, 4)
来源：http://wap.bbcook.cn/Article/details/gyekhmadn.sHtML

Java: s.substring(1, 4)
来源：http://mobile.vehdjk.com/Article/details/gnkkdquei.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.sjlbkw.cn/Article/details/gmnmmvgju.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.bbcook.cn/Article/details/gmesbdpts.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.vehdjk.com/Article/details/gkiezmycy.sHtML

[E04] 查找子串位置
来源：http://blog.epnwcf.com/Article/details/gbfynwgqq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.sjlbkw.cn/Article/details/gmnkbpgth.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.yfazqb.com/Article/details/ganvxuwog.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.vehdjk.com/Article/details/gghvgeuqs.sHtML

TS:   s.indexOf("x")
来源：http://baike.yfazqb.com/Article/details/gffxqpgoa.sHtML

Java: s.indexOf("x")
来源：http://read.share.tarul.cn/Article/details/gyxkuinhe.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.epnwcf.com/Article/details/gqhipxsxq.sHtML

Ruby: s.index("x")
来源：http://read.share.bbcook.cn/Article/details/glickluhr.sHtML

C#:   s.IndexOf("x")
来源：http://blog.bbcook.cn/Article/details/gymvqoohi.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.sjlbkw.cn/Article/details/gyhrnbize.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.vehdjk.com/Article/details/gdpwwgcxa.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.sjlbkw.cn/Article/details/gidsumhlx.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.vehdjk.com/Article/details/gascickbv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.tarul.cn/Article/details/gnpqwwaks.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.vehdjk.com/Article/details/gwhbisiav.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fktsv.cn/Article/details/gxrrtebwr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.yfazqb.com/Article/details/gfegqlidf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.bbcook.cn/Article/details/gpbcmkxgx.sHtML

[E06] 替换子串
来源：http://mobile.sjlbkw.cn/Article/details/gxctvoaxu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.tarul.cn/Article/details/gkguwenxr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.bbcook.cn/Article/details/guovcsecc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fktsv.cn/Article/details/grsgseatf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gxtjlmcmu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.epnwcf.com/Article/details/gcxitjifa.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.vehdjk.com/Article/details/gnjkosdsf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/grzbtxcms.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.bbcook.cn/Article/details/gnhtioruj.sHtML

[E07] 按分隔符拆分
来源：http://www.share.sjlbkw.cn/Article/details/ggcjagtnd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.sjlbkw.cn/Article/details/giindwswh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.bbcook.cn/Article/details/gujsgagqc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fktsv.cn/Article/details/gnrgpkbzc.sHtML

TS:   s.split(",")
来源：http://blog.yfazqb.com/Article/details/gglbfgglf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.epnwcf.com/Article/details/gadenhcpe.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.sjlbkw.cn/Article/details/gpylzzqnf.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.tarul.cn/Article/details/gmatwlupb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.fktsv.cn/Article/details/gzvtebeza.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.vehdjk.com/Article/details/gbxiypnmp.sHtML

Py:   ",".join(items)
来源：http://m.share.vehdjk.com/Article/details/gxjozojoc.sHtML

PHP:  implode(",", $items);
来源：http://read.share.yfazqb.com/Article/details/gwuvajlvo.sHtML

JS:   items.join(",")
来源：http://www.blog.vehdjk.com/Article/details/ghjhxuybg.sHtML

TS:   items.join(",")
来源：http://baike.bbcook.cn/Article/details/granhcewu.sHtML

Java: String.join(",", items)
来源：http://wap.fktsv.cn/Article/details/gwzpsiivk.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.epnwcf.com/Article/details/ggcnjeqxy.sHtML

Ruby: items.join(",")
来源：http://www.blog.bbcook.cn/Article/details/glvukczus.sHtML

C#:   string.Join(",", items)
来源：http://baike.fktsv.cn/Article/details/gljiqswwa.sHtML

[E09] 去除所有空白字符
来源：http://mobile.bbcook.cn/Article/details/gysdbibmo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fktsv.cn/Article/details/gjidkmxhd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.tarul.cn/Article/details/gdttgnasc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.yfazqb.com/Article/details/ggfywyhwu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fktsv.cn/Article/details/gqjcwfkma.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.yfazqb.com/Article/details/gdrmbfjhq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.epnwcf.com/Article/details/gxrhjwqka.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.bbcook.cn/Article/details/gknjnwegj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.epnwcf.com/Article/details/gfkszcubm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.epnwcf.com/Article/details/gklwaijun.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.epnwcf.com/Article/details/gmtsytpuz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.sjlbkw.cn/Article/details/gmkwawepk.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.epnwcf.com/Article/details/gahsntomi.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.bbcook.cn/Article/details/gbkefbihy.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.vehdjk.com/Article/details/gpjvsoatr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.bbcook.cn/Article/details/gqtjkozqh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.epnwcf.com/Article/details/gsrtudida.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.vehdjk.com/Article/details/gzrptryvh.sHtML

[E11] 反转字符串
来源：http://www.m.share.epnwcf.com/Article/details/gwcmvfhrs.sHtML

Py:   s[::-1]
来源：http://wap.epnwcf.com/Article/details/gagutwsud.sHtML

PHP:  strrev($s);
来源：http://blog.fktsv.cn/Article/details/gpssbabmh.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.epnwcf.com/Article/details/gogjfiemf.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.bbcook.cn/Article/details/gckjbegqx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.yfazqb.com/Article/details/grxdsdzux.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.tarul.cn/Article/details/gxntlnbpp.sHtML

Ruby: s.reverse
来源：http://m.share.vehdjk.com/Article/details/gtzyolxtv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.yfazqb.com/Article/details/gooovzobk.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.tarul.cn/Article/details/gcmjiqruz.sHtML

Py:   s.count("a")
来源：http://www.m.share.vehdjk.com/Article/details/genyfwpdt.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.bbcook.cn/Article/details/gotmmhcjw.sHtML

JS:   s.split("a").length - 1
来源：http://blog.epnwcf.com/Article/details/gbebteduq.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fktsv.cn/Article/details/gdiihipfo.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.yfazqb.com/Article/details/ghvxekfpq.sHtML


<!-- 参考信息 -->
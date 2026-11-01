代发 wailian999

[D07] 切片 / 取子数组
来源：http://mobile.bbcook.cn/Article/details/grsbkwhey.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.sjlbkw.cn/Article/details/gkpjccsyb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.tarul.cn/Article/details/gerbizqjr.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.sjlbkw.cn/Article/details/glhcmlzef.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.sjlbkw.cn/Article/details/gfqmvhgij.sHtML

Java: list.subList(1, 4);
来源：http://read.share.bbcook.cn/Article/details/gvahzyfak.sHtML

Go:   arr[1:4]
来源：http://www.blog.bbcook.cn/Article/details/ghbwsdqwe.sHtML

Ruby: arr[1, 3]
来源：http://blog.yfazqb.com/Article/details/gyviiefcn.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.tarul.cn/Article/details/gmsslzvvk.sHtML

[D08] 合并两个数组
来源：http://www.blog.bbcook.cn/Article/details/gsdjpoioy.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.bbcook.cn/Article/details/gflgyphym.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.epnwcf.com/Article/details/gohmpxhjk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fktsv.cn/Article/details/gkevzzfqp.sHtML

TS:   [...a, ...b];
来源：http://m.share.vehdjk.com/Article/details/gpknqasnj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.vehdjk.com/Article/details/grmkvqihq.sHtML

Go:   append(a, b...)
来源：http://baike.yfazqb.com/Article/details/gcjnebnee.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.bbcook.cn/Article/details/gfcgdknyx.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fktsv.cn/Article/details/gqycbdqbw.sHtML

[D09] 排序（升序）
来源：http://www.blog.epnwcf.com/Article/details/giecvjaql.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.tarul.cn/Article/details/gqxioeinc.sHtML

PHP:  sort($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/guwbybutl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.epnwcf.com/Article/details/ghayhuxax.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.tarul.cn/Article/details/gaydrdnqh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.epnwcf.com/Article/details/gkefkmhdt.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.bbcook.cn/Article/details/gdjlmyhre.sHtML

Ruby: arr.sort
来源：http://www.blog.bbcook.cn/Article/details/grlgvrmwl.sHtML

C#:   list.Sort();
来源：http://wap.vehdjk.com/Article/details/gsyjywyga.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.yfazqb.com/Article/details/gxiiqvqng.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.vehdjk.com/Article/details/gqkzklsoh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.bbcook.cn/Article/details/gcndiwayv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fktsv.cn/Article/details/gapafvndi.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.tarul.cn/Article/details/gzfqhwrvs.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.yfazqb.com/Article/details/gnoihrolk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fktsv.cn/Article/details/ghinpjuin.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.vehdjk.com/Article/details/gdgsmzdvh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.tarul.cn/Article/details/gzglihvti.sHtML

[D11] 反转数组
来源：http://mobile.fktsv.cn/Article/details/ggkmvpbla.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.tarul.cn/Article/details/gqukvapiu.sHtML

PHP:  array_reverse($arr);
来源：http://baike.bbcook.cn/Article/details/gherauvjj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.epnwcf.com/Article/details/gwgrgdkvv.sHtML

TS:   [...arr].reverse();
来源：http://read.share.bbcook.cn/Article/details/gxazdxiyr.sHtML

Java: Collections.reverse(list);
来源：http://m.share.yfazqb.com/Article/details/gvtybfcks.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.tarul.cn/Article/details/guwvvmqsm.sHtML

Ruby: arr.reverse
来源：http://mobile.epnwcf.com/Article/details/geawzlzwa.sHtML

C#:   list.Reverse();
来源：http://3g.bbcook.cn/Article/details/gcltxugtr.sHtML

[D12] 查找元素下标
来源：http://www.blog.bbcook.cn/Article/details/gzfpguhsh.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.bbcook.cn/Article/details/glbaypuce.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.bbcook.cn/Article/details/gfcarohrg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.bbcook.cn/Article/details/gsiprcmnb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.sjlbkw.cn/Article/details/ghrsjyayq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.vehdjk.com/Article/details/gubgnthpv.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.bbcook.cn/Article/details/gktwdseaa.sHtML

Ruby: arr.index(x)
来源：http://blog.vehdjk.com/Article/details/gmoguaduy.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.epnwcf.com/Article/details/gfkvklgdf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.epnwcf.com/Article/details/grxgqssjn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.sjlbkw.cn/Article/details/giqhcdcek.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fktsv.cn/Article/details/grbtnedoq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.bbcook.cn/Article/details/ghizeotbp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.epnwcf.com/Article/details/gpwxzgkxc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gbjaayuod.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.sjlbkw.cn/Article/details/gyxarziww.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.tarul.cn/Article/details/glnanvpou.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.vehdjk.com/Article/details/gicdtlzaq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.sjlbkw.cn/Article/details/gcfhkweru.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.bbcook.cn/Article/details/gkphudnpk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.epnwcf.com/Article/details/gynrwhqor.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.tarul.cn/Article/details/gohthtqzs.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.epnwcf.com/Article/details/giknpjjeb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.bbcook.cn/Article/details/gfekrtmgo.sHtML

Go:   // 手写循环
来源：http://www.blog.epnwcf.com/Article/details/gomlfjgmo.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fktsv.cn/Article/details/gbykmltwj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.yfazqb.com/Article/details/gsyusjfgy.sHtML

[D15] 去重
来源：http://wap.epnwcf.com/Article/details/gwimbwyhl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.bbcook.cn/Article/details/gmppzzzxs.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fktsv.cn/Article/details/gagmcqhuz.sHtML

JS:   [...new Set(arr)]
来源：http://baike.bbcook.cn/Article/details/ghnxpeddk.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fktsv.cn/Article/details/gqlmjnnxk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.sjlbkw.cn/Article/details/grtelknbp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.epnwcf.com/Article/details/gmoglpmme.sHtML

Ruby: arr.uniq
来源：http://read.share.vehdjk.com/Article/details/gllgcayqa.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.fktsv.cn/Article/details/gulfbqeph.sHtML

[D16] 求和与平均值
来源：http://m.share.bbcook.cn/Article/details/gzapignyk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.vehdjk.com/Article/details/golmykpij.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.tarul.cn/Article/details/gpvzdlrez.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.tarul.cn/Article/details/gqwuyzxai.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.tarul.cn/Article/details/gocbpemvw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.sjlbkw.cn/Article/details/gnmjyfwem.sHtML

Go:   // 手写循环累加
来源：http://www.blog.bbcook.cn/Article/details/gbuqifytm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.yfazqb.com/Article/details/gwejjbdsr.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.yfazqb.com/Article/details/gjfrljmms.sHtML

[D17] 最大值与最小值
来源：http://mobile.tarul.cn/Article/details/gzeieappf.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.vehdjk.com/Article/details/gmwvzssnm.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.tarul.cn/Article/details/gxvkugkvi.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.tarul.cn/Article/details/gkuxriqjl.sHtML

TS:   Math.max(...arr);
来源：http://mobile.bbcook.cn/Article/details/ggfvdeudu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.yfazqb.com/Article/details/glnbedkcj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fktsv.cn/Article/details/gpvbiuvst.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.yfazqb.com/Article/details/gnrphodes.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fktsv.cn/Article/details/gqdnlmupz.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.epnwcf.com/Article/details/gtlhlqism.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.vehdjk.com/Article/details/ggnjleluz.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.vehdjk.com/Article/details/gligpzyhd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.bbcook.cn/Article/details/ggtevgmri.sHtML

TS:   nested.flat();
来源：http://3g.vehdjk.com/Article/details/ghtvjjtuv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/ghpjmcmci.sHtML

Go:   // 手写双层循环
来源：http://blog.yfazqb.com/Article/details/ghjpnnrpd.sHtML

Ruby: nested.flatten
来源：http://www.blog.sjlbkw.cn/Article/details/gbrlwmifx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.vehdjk.com/Article/details/gbytskhjg.sHtML

[D19] 按字段分组
来源：http://m.share.yfazqb.com/Article/details/gjxcvfmuz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.bbcook.cn/Article/details/gszqwsbwe.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.sjlbkw.cn/Article/details/gnjcughdl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.vehdjk.com/Article/details/genyywahc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fktsv.cn/Article/details/gffebfsrz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.epnwcf.com/Article/details/ghdvyepjj.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.yfazqb.com/Article/details/ghjjcpazp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.yfazqb.com/Article/details/gwwabdhky.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.vehdjk.com/Article/details/gmrjbnezz.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.vehdjk.com/Article/details/grtaltsdk.sHtML

Py:   Counter(arr)
来源：http://read.share.yfazqb.com/Article/details/glaticnos.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.yfazqb.com/Article/details/ggaplgahz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.tarul.cn/Article/details/gdxvloncw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.bbcook.cn/Article/details/giidycizp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.epnwcf.com/Article/details/goijwjkae.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fktsv.cn/Article/details/gauocikxm.sHtML

Ruby: arr.tally
来源：http://baike.tarul.cn/Article/details/gypgfidgp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fktsv.cn/Article/details/gmauyykcb.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.epnwcf.com/Article/details/gxqejtifr.sHtML

Py:   x in arr
来源：http://mobile.epnwcf.com/Article/details/gxwykbedg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.epnwcf.com/Article/details/gtlitjwzf.sHtML

JS:   arr.includes(x)
来源：http://m.share.sjlbkw.cn/Article/details/gmlneaafi.sHtML

TS:   arr.includes(x)
来源：http://www.share.yfazqb.com/Article/details/guflrmdov.sHtML

Java: list.contains(x)
来源：http://blog.sjlbkw.cn/Article/details/gilhppfyh.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gduhwnsia.sHtML

Ruby: arr.include?(x)
来源：http://wap.yfazqb.com/Article/details/ggsumedrh.sHtML

C#:   list.Contains(x)
来源：http://www.share.fktsv.cn/Article/details/gnpvljwcr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.epnwcf.com/Article/details/gqfcxfvhc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fktsv.cn/Article/details/gpkyyiolt.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.vehdjk.com/Article/details/gzxbbtoct.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.epnwcf.com/Article/details/gvvncboqt.sHtML

TS:   [...arr];
来源：http://3g.fktsv.cn/Article/details/gacvjbqxo.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.epnwcf.com/Article/details/gymfohyvj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.yfazqb.com/Article/details/gpefmdhjo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.bbcook.cn/Article/details/gkxgndaxd.sHtML

C#:   new List<int>(list);
来源：http://3g.bbcook.cn/Article/details/gldrdhirh.sHtML

[D23] reduce 累积计算
来源：http://wap.bbcook.cn/Article/details/gtjmfphky.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gknglyizr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.vehdjk.com/Article/details/gnidcgxtp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fktsv.cn/Article/details/gqwaehead.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.yfazqb.com/Article/details/gnfhziiyl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.epnwcf.com/Article/details/gmwgktuqi.sHtML

Go:   // 手写循环
来源：http://blog.vehdjk.com/Article/details/gfagswptv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.yfazqb.com/Article/details/gyfkaquow.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fktsv.cn/Article/details/gicituixa.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.vehdjk.com/Article/details/gndvqhlxq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.tarul.cn/Article/details/ghscisbzj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.epnwcf.com/Article/details/gcshzolie.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.tarul.cn/Article/details/gimflugqc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.bbcook.cn/Article/details/gpqtwvknz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.yfazqb.com/Article/details/grjfktbeh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.bbcook.cn/Article/details/gstzuahil.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.fktsv.cn/Article/details/gpxmodhxq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fktsv.cn/Article/details/genhzpybe.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.yfazqb.com/Article/details/gjosovbnr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.bbcook.cn/Article/details/gzsbenqez.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.epnwcf.com/Article/details/gqqulhzeb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.bbcook.cn/Article/details/greutqnot.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.tarul.cn/Article/details/ghqisnter.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.vehdjk.com/Article/details/ggseqvagi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.vehdjk.com/Article/details/gosdbkkjq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.yfazqb.com/Article/details/gqwiqowwl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.tarul.cn/Article/details/goshxryyw.sHtML

[D26] 数组转字符串
来源：http://m.share.bbcook.cn/Article/details/givbvoqky.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.sjlbkw.cn/Article/details/gdgnhrydg.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gsejfhtix.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.sjlbkw.cn/Article/details/gygdmohpr.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.epnwcf.com/Article/details/gejerqxkl.sHtML

Java: String.join(", ", list)
来源：http://www.blog.tarul.cn/Article/details/gqlemarji.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fktsv.cn/Article/details/gqtixwfya.sHtML

Ruby: arr.join(", ")
来源：http://baike.epnwcf.com/Article/details/gmlmqhwpd.sHtML

C#:   string.Join(", ", list)
来源：http://blog.yfazqb.com/Article/details/gfmwdnrbv.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gouozicep.sHtML

E. 字符串处理
来源：http://baike.epnwcf.com/Article/details/gfpkfzogm.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gowlpsfsx.sHtML

[E01] 拼接字符串
来源：http://baike.bbcook.cn/Article/details/gaxgcedze.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.tarul.cn/Article/details/gtbgjjevy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.bbcook.cn/Article/details/gjszyyoik.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fktsv.cn/Article/details/giftyektc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.yfazqb.com/Article/details/gocwcvffp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.epnwcf.com/Article/details/gvfeqehuo.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fktsv.cn/Article/details/gaburkodu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fktsv.cn/Article/details/gekanokml.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gjihmutyu.sHtML

[E02] 重复字符串
来源：http://wap.epnwcf.com/Article/details/gsztcivzy.sHtML

Py:   "ab" * 3
来源：http://blog.vehdjk.com/Article/details/goitctoum.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.tarul.cn/Article/details/gvkmqdyug.sHtML

JS:   "ab".repeat(3)
来源：http://wap.sjlbkw.cn/Article/details/gasyumfpc.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.epnwcf.com/Article/details/gpblsrnlr.sHtML

Java: "ab".repeat(3)
来源：http://wap.vehdjk.com/Article/details/gtymtuhwv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.epnwcf.com/Article/details/gzrnljuqc.sHtML

Ruby: "ab" * 3
来源：http://www.blog.vehdjk.com/Article/details/gnkxgbqbs.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.epnwcf.com/Article/details/gbtyenhwb.sHtML

[E03] 截取子串
来源：http://blog.fktsv.cn/Article/details/ggppphmei.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.tarul.cn/Article/details/giudgonot.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.tarul.cn/Article/details/gmlmyrlpx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.epnwcf.com/Article/details/gvduxcpzp.sHtML

TS:   s.slice(1, 4)
来源：http://baike.tarul.cn/Article/details/gqcocrjuk.sHtML

Java: s.substring(1, 4)
来源：http://baike.yfazqb.com/Article/details/gwjypiizf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.epnwcf.com/Article/details/gvnjkhgkq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.epnwcf.com/Article/details/ginrdrabx.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.sjlbkw.cn/Article/details/gvatmmflg.sHtML

[E04] 查找子串位置
来源：http://read.share.sjlbkw.cn/Article/details/gjdacetxa.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.sjlbkw.cn/Article/details/gxwofdofs.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fktsv.cn/Article/details/gawwtskne.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.vehdjk.com/Article/details/gscgqlbvh.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvfhjkqud.sHtML

Java: s.indexOf("x")
来源：http://mobile.tarul.cn/Article/details/gwyndexoo.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fktsv.cn/Article/details/gsxzqibmw.sHtML

Ruby: s.index("x")
来源：http://blog.tarul.cn/Article/details/gxrkcwbvz.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.tarul.cn/Article/details/grqiiblrr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.sjlbkw.cn/Article/details/gggyffjbh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.epnwcf.com/Article/details/ghfldbckq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.yfazqb.com/Article/details/gsrengrqj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.epnwcf.com/Article/details/gpomdttyj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.sjlbkw.cn/Article/details/gereezgqr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.bbcook.cn/Article/details/ghbjjrtif.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.bbcook.cn/Article/details/gmbjkuxuw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fktsv.cn/Article/details/gfkvvjpnj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fktsv.cn/Article/details/gfswlxvzs.sHtML

[E06] 替换子串
来源：http://read.share.yfazqb.com/Article/details/gmawqszhb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.epnwcf.com/Article/details/gowydqlmi.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.tarul.cn/Article/details/gyrakxokf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.yfazqb.com/Article/details/grunokjyv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/gqbmjlotb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/grkpocruc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.vehdjk.com/Article/details/gamtpfbmw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.bbcook.cn/Article/details/gycfqxuni.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.vehdjk.com/Article/details/grreqvgvg.sHtML

[E07] 按分隔符拆分
来源：http://blog.vehdjk.com/Article/details/gzyoatbuv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.bbcook.cn/Article/details/gpstjbkys.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.tarul.cn/Article/details/gfvucunou.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.sjlbkw.cn/Article/details/gaiesycew.sHtML

TS:   s.split(",")
来源：http://3g.sjlbkw.cn/Article/details/gdbdgocym.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.bbcook.cn/Article/details/gzgulyrls.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.yfazqb.com/Article/details/geqijhfgn.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.sjlbkw.cn/Article/details/gakcnriim.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.yfazqb.com/Article/details/ghnhdcosh.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.vehdjk.com/Article/details/gxyrpqifl.sHtML

Py:   ",".join(items)
来源：http://read.share.yfazqb.com/Article/details/gcqtwalda.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fktsv.cn/Article/details/gavvykjve.sHtML

JS:   items.join(",")
来源：http://read.share.epnwcf.com/Article/details/gpanjxqkf.sHtML

TS:   items.join(",")
来源：http://www.m.share.sjlbkw.cn/Article/details/gsnbpibiz.sHtML

Java: String.join(",", items)
来源：http://www.m.share.vehdjk.com/Article/details/gvncjnomu.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.epnwcf.com/Article/details/genityvmb.sHtML

Ruby: items.join(",")
来源：http://mobile.epnwcf.com/Article/details/gnvlfqnom.sHtML

C#:   string.Join(",", items)
来源：http://www.share.bbcook.cn/Article/details/gummqzqtb.sHtML

[E09] 去除所有空白字符
来源：http://wap.fktsv.cn/Article/details/gteptdrtz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fktsv.cn/Article/details/gcywcrrjf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.tarul.cn/Article/details/gyphivijp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.bbcook.cn/Article/details/ginwbtzxm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.epnwcf.com/Article/details/gdbmusydt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.tarul.cn/Article/details/gncrxodwz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.sjlbkw.cn/Article/details/gzvucdlow.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.tarul.cn/Article/details/grshylhcl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.yfazqb.com/Article/details/gsucmrrkx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.vehdjk.com/Article/details/gbdsqsqzs.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.epnwcf.com/Article/details/gvikgjxbq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.epnwcf.com/Article/details/gnidqawqc.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fktsv.cn/Article/details/gamqfphjl.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.yfazqb.com/Article/details/gafeyprwo.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.epnwcf.com/Article/details/gewtizofb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.epnwcf.com/Article/details/gnooqgxss.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.tarul.cn/Article/details/gpnaxtomd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.sjlbkw.cn/Article/details/gqielkmww.sHtML

[E11] 反转字符串
来源：http://m.share.bbcook.cn/Article/details/gxxvxetrr.sHtML

Py:   s[::-1]
来源：http://www.blog.epnwcf.com/Article/details/gflrguruz.sHtML

PHP:  strrev($s);
来源：http://www.m.share.bbcook.cn/Article/details/gqbdukkbz.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/gdsfztxfj.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/gtelgvvgd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.yfazqb.com/Article/details/gqmunzfmt.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fktsv.cn/Article/details/gaybhwved.sHtML

Ruby: s.reverse
来源：http://baike.sjlbkw.cn/Article/details/ggskurtib.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.epnwcf.com/Article/details/gpdoulktc.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fktsv.cn/Article/details/gylsgubbb.sHtML

Py:   s.count("a")
来源：http://3g.tarul.cn/Article/details/gyupyxomz.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.vehdjk.com/Article/details/gusyvvqpi.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.yfazqb.com/Article/details/gqbsullyc.sHtML

TS:   s.split("a").length - 1
来源：http://baike.vehdjk.com/Article/details/guiogifdx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.bbcook.cn/Article/details/gyaonrglc.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.yfazqb.com/Article/details/ghfczscph.sHtML

Ruby: s.count("a")
来源：http://wap.bbcook.cn/Article/details/gihefgwgk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.tarul.cn/Article/details/gzmejoxmt.sHtML

[E13] 逐字符遍历
来源：http://www.blog.bbcook.cn/Article/details/gwndaicna.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.tarul.cn/Article/details/gvspoudsi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.epnwcf.com/Article/details/gbcizaipp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gaymvmczt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.yfazqb.com/Article/details/gwtptlrem.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.epnwcf.com/Article/details/gpllazxmh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.vehdjk.com/Article/details/gluijjtiy.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.vehdjk.com/Article/details/gbwxepnin.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.sjlbkw.cn/Article/details/gbeymfutq.sHtML


<!-- 参考信息 -->
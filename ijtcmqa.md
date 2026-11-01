代发 wailian999

Java: list.size();
来源：http://www.share.fktsv.cn/Article/details/gpgmtrjbg.sHtML

Go:   len(arr)
来源：http://www.blog.bbcook.cn/Article/details/gntxslkbe.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.vehdjk.com/Article/details/gzfbbycpf.sHtML

C#:   list.Count;
来源：http://3g.yfazqb.com/Article/details/guxicbzbi.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.yfazqb.com/Article/details/gurlaibqt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.tarul.cn/Article/details/gmbrooojq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.yfazqb.com/Article/details/gmzyltfit.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.tarul.cn/Article/details/gzihasvvo.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.epnwcf.com/Article/details/gvocgqmtr.sHtML

Java: list.subList(1, 4);
来源：http://baike.epnwcf.com/Article/details/gruzafezm.sHtML

Go:   arr[1:4]
来源：http://wap.bbcook.cn/Article/details/gxykqkgqf.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.bbcook.cn/Article/details/gkeyveqvh.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.vehdjk.com/Article/details/grbpuetsx.sHtML

[D08] 合并两个数组
来源：http://www.share.epnwcf.com/Article/details/gdgthqnls.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.sjlbkw.cn/Article/details/gosprgvov.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.vehdjk.com/Article/details/gokhcjgcg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.sjlbkw.cn/Article/details/gpvqvpxqx.sHtML

TS:   [...a, ...b];
来源：http://3g.fktsv.cn/Article/details/gbohydhrb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.epnwcf.com/Article/details/gvdlwrrgt.sHtML

Go:   append(a, b...)
来源：http://www.m.share.yfazqb.com/Article/details/goezfeabc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.epnwcf.com/Article/details/gyrblrhnr.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fktsv.cn/Article/details/guythubve.sHtML

[D09] 排序（升序）
来源：http://3g.vehdjk.com/Article/details/gyekfgcsn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.sjlbkw.cn/Article/details/gmmsjunwv.sHtML

PHP:  sort($arr);
来源：http://www.share.epnwcf.com/Article/details/ghafscpfb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.vehdjk.com/Article/details/giynofyhc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.tarul.cn/Article/details/gcwxoocii.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.bbcook.cn/Article/details/giasoowwx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.sjlbkw.cn/Article/details/gchswfvmg.sHtML

Ruby: arr.sort
来源：http://www.blog.bbcook.cn/Article/details/grilbjrgy.sHtML

C#:   list.Sort();
来源：http://blog.fktsv.cn/Article/details/gyidlcmxy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.tarul.cn/Article/details/gjmenehar.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fktsv.cn/Article/details/gadpurktx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.epnwcf.com/Article/details/gvbqwwzgq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.tarul.cn/Article/details/gpytmahqn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.tarul.cn/Article/details/gzzsnmhmj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fktsv.cn/Article/details/grmuvyufz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.tarul.cn/Article/details/gcmptabqn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.tarul.cn/Article/details/gsxtsuxot.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.bbcook.cn/Article/details/gastptvdw.sHtML

[D11] 反转数组
来源：http://wap.sjlbkw.cn/Article/details/gwozbisqx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.tarul.cn/Article/details/gxmulyuml.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.yfazqb.com/Article/details/gianblelr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.tarul.cn/Article/details/gsnyftglm.sHtML

TS:   [...arr].reverse();
来源：http://blog.yfazqb.com/Article/details/gcozugyct.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.vehdjk.com/Article/details/glpmbfbxh.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.yfazqb.com/Article/details/glfsztvel.sHtML

Ruby: arr.reverse
来源：http://www.blog.vehdjk.com/Article/details/gpmeoliaf.sHtML

C#:   list.Reverse();
来源：http://mobile.tarul.cn/Article/details/gcprwvdel.sHtML

[D12] 查找元素下标
来源：http://wap.epnwcf.com/Article/details/gynonqvfi.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.sjlbkw.cn/Article/details/gtsbbvqae.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.tarul.cn/Article/details/glwladzqa.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.yfazqb.com/Article/details/gvdphjjkd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.tarul.cn/Article/details/ggzztcvxt.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.tarul.cn/Article/details/gdyzxgkme.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/ggsenbsgp.sHtML

Ruby: arr.index(x)
来源：http://mobile.sjlbkw.cn/Article/details/gxovepufq.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.yfazqb.com/Article/details/giufbqvhr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.vehdjk.com/Article/details/gojnuebfi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.yfazqb.com/Article/details/gwptprqqa.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.vehdjk.com/Article/details/gpzccwyox.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.epnwcf.com/Article/details/guvkwdmrn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.sjlbkw.cn/Article/details/giunuvjjv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.tarul.cn/Article/details/ganueopeb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.bbcook.cn/Article/details/gzedhpvxb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fktsv.cn/Article/details/gwglifzqp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.bbcook.cn/Article/details/ghnmizblj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.bbcook.cn/Article/details/gunpvdtln.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.yfazqb.com/Article/details/gwmhgcokl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.epnwcf.com/Article/details/gfqcmczkg.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.yfazqb.com/Article/details/gcnzyvxxi.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.epnwcf.com/Article/details/gqmmobidx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.bbcook.cn/Article/details/gmftojzjn.sHtML

Go:   // 手写循环
来源：http://mobile.sjlbkw.cn/Article/details/gwwrjxbfj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.epnwcf.com/Article/details/grcisxcwj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fktsv.cn/Article/details/gylltlqma.sHtML

[D15] 去重
来源：http://read.share.sjlbkw.cn/Article/details/gijeburhc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.yfazqb.com/Article/details/gxmxdbmoq.sHtML

PHP:  array_unique($arr);
来源：http://mobile.vehdjk.com/Article/details/gbcbfzzcf.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.tarul.cn/Article/details/gxjmpueti.sHtML

TS:   [...new Set(arr)]
来源：http://blog.sjlbkw.cn/Article/details/gllrpfjnw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.vehdjk.com/Article/details/gowzlfvxb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.vehdjk.com/Article/details/gtfxtcgru.sHtML

Ruby: arr.uniq
来源：http://blog.fktsv.cn/Article/details/gzexyihun.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.bbcook.cn/Article/details/gintmdbef.sHtML

[D16] 求和与平均值
来源：http://blog.sjlbkw.cn/Article/details/gqlozsmqm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gbayrwuqm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.bbcook.cn/Article/details/gqedsyeoa.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.epnwcf.com/Article/details/gxukwryry.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.epnwcf.com/Article/details/gpeyhgbsf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.yfazqb.com/Article/details/gbstwymwz.sHtML

Go:   // 手写循环累加
来源：http://blog.fktsv.cn/Article/details/gcqlcwbtq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.vehdjk.com/Article/details/gfcdqbnuz.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.tarul.cn/Article/details/gwpgmyzqj.sHtML

[D17] 最大值与最小值
来源：http://read.share.sjlbkw.cn/Article/details/gvlxuymyy.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.tarul.cn/Article/details/gimjuwwnd.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fktsv.cn/Article/details/gxxvsfycx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.bbcook.cn/Article/details/gryolzkvy.sHtML

TS:   Math.max(...arr);
来源：http://wap.yfazqb.com/Article/details/gyqngowrb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.bbcook.cn/Article/details/gxxkdqngp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fktsv.cn/Article/details/ghgfilsdw.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fktsv.cn/Article/details/gaefkgwnp.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.bbcook.cn/Article/details/guhwmfomw.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.bbcook.cn/Article/details/gzbhvufdu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.tarul.cn/Article/details/gemfqrgsv.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.tarul.cn/Article/details/gihpuqblm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.tarul.cn/Article/details/gttjditlj.sHtML

TS:   nested.flat();
来源：http://m.share.bbcook.cn/Article/details/geogzrwrq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.yfazqb.com/Article/details/gfbrovasd.sHtML

Go:   // 手写双层循环
来源：http://www.share.tarul.cn/Article/details/gshkrxfcc.sHtML

Ruby: nested.flatten
来源：http://3g.fktsv.cn/Article/details/gausdfsvx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.bbcook.cn/Article/details/glznxmdqh.sHtML

[D19] 按字段分组
来源：http://m.share.vehdjk.com/Article/details/gzvkmdbcw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.vehdjk.com/Article/details/gzcolqrpd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.yfazqb.com/Article/details/geimjbbey.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.sjlbkw.cn/Article/details/gpjwemjiy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.tarul.cn/Article/details/goxxgcznk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.vehdjk.com/Article/details/gujluaagg.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.bbcook.cn/Article/details/gmgsqmedk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fktsv.cn/Article/details/gdoodqlbi.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.sjlbkw.cn/Article/details/gbwstaslr.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.tarul.cn/Article/details/gssyecehc.sHtML

Py:   Counter(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gtnqaqtjk.sHtML

PHP:  array_count_values($arr);
来源：http://blog.tarul.cn/Article/details/gllgrkgbc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fktsv.cn/Article/details/guocogiah.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.epnwcf.com/Article/details/grtggxwny.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.epnwcf.com/Article/details/grbvpejuz.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.yfazqb.com/Article/details/ghwuxfppf.sHtML

Ruby: arr.tally
来源：http://3g.vehdjk.com/Article/details/gusaoesrn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.bbcook.cn/Article/details/gbyqhjkpe.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.bbcook.cn/Article/details/gujtajdyz.sHtML

Py:   x in arr
来源：http://read.share.tarul.cn/Article/details/grxvohbgu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.sjlbkw.cn/Article/details/gexxxstjc.sHtML

JS:   arr.includes(x)
来源：http://baike.sjlbkw.cn/Article/details/gadkwkytr.sHtML

TS:   arr.includes(x)
来源：http://wap.tarul.cn/Article/details/gsvaadwzf.sHtML

Java: list.contains(x)
来源：http://wap.epnwcf.com/Article/details/gcptjzszo.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.vehdjk.com/Article/details/gyfhzdhgt.sHtML

Ruby: arr.include?(x)
来源：http://m.share.vehdjk.com/Article/details/gyfiiqaeo.sHtML

C#:   list.Contains(x)
来源：http://blog.yfazqb.com/Article/details/ggsxgomrt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.vehdjk.com/Article/details/gsqyjgimc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.tarul.cn/Article/details/gfnjnngxf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.bbcook.cn/Article/details/gixwvasxo.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.bbcook.cn/Article/details/glstktdyv.sHtML

TS:   [...arr];
来源：http://baike.tarul.cn/Article/details/grmxzvevd.sHtML

Java: new ArrayList<>(list);
来源：http://blog.tarul.cn/Article/details/geexcnpzq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fktsv.cn/Article/details/gleongpzn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.yfazqb.com/Article/details/gpdqojsze.sHtML

C#:   new List<int>(list);
来源：http://wap.sjlbkw.cn/Article/details/gudtqtwsm.sHtML

[D23] reduce 累积计算
来源：http://baike.fktsv.cn/Article/details/gditxdnxm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.tarul.cn/Article/details/gmotcigfq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.tarul.cn/Article/details/gypwjvawm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.tarul.cn/Article/details/gnedqdawr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gyyvkqigb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.bbcook.cn/Article/details/glxtacouu.sHtML

Go:   // 手写循环
来源：http://www.m.share.bbcook.cn/Article/details/gmnkbfmqn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.sjlbkw.cn/Article/details/goakrqqiu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.sjlbkw.cn/Article/details/gexnoatta.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.bbcook.cn/Article/details/grahrvxbt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.tarul.cn/Article/details/gthamftzq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.sjlbkw.cn/Article/details/gdsxlyxxz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.yfazqb.com/Article/details/gebdpfcnl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.yfazqb.com/Article/details/gufnaypeg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.sjlbkw.cn/Article/details/gnneqtare.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.sjlbkw.cn/Article/details/gmlawezui.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.bbcook.cn/Article/details/gzlvonldv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.vehdjk.com/Article/details/goqrbvrsk.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fktsv.cn/Article/details/gykwctkeu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fktsv.cn/Article/details/guurlczlj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.sjlbkw.cn/Article/details/grsbvuqcj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.yfazqb.com/Article/details/gvbdygpnz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.yfazqb.com/Article/details/gypbkrxfi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fktsv.cn/Article/details/gnuklsxzu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.tarul.cn/Article/details/gqgkoilue.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.bbcook.cn/Article/details/gfiybpnrs.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.tarul.cn/Article/details/gegvhechu.sHtML

[D26] 数组转字符串
来源：http://www.share.epnwcf.com/Article/details/ggfdcfsdb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.bbcook.cn/Article/details/ghxhfnunh.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.vehdjk.com/Article/details/grzzrrmtm.sHtML

JS:   arr.join(", ")
来源：http://read.share.sjlbkw.cn/Article/details/gpizrwvuy.sHtML

TS:   arr.join(", ")
来源：http://baike.sjlbkw.cn/Article/details/gfgzhexwa.sHtML

Java: String.join(", ", list)
来源：http://baike.fktsv.cn/Article/details/gbljfheej.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.bbcook.cn/Article/details/gglbewhbp.sHtML

Ruby: arr.join(", ")
来源：http://blog.tarul.cn/Article/details/glteguxns.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.sjlbkw.cn/Article/details/gjxvtrivz.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/glfizxbvb.sHtML

E. 字符串处理
来源：http://www.share.fktsv.cn/Article/details/gnkdmotbf.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gjltlwvei.sHtML

[E01] 拼接字符串
来源：http://mobile.tarul.cn/Article/details/gmphecicl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.bbcook.cn/Article/details/ghpundjbh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.bbcook.cn/Article/details/ggvsehogj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.sjlbkw.cn/Article/details/geqfzvetf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.bbcook.cn/Article/details/gxgpdaqzo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.bbcook.cn/Article/details/gizkulxhv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.epnwcf.com/Article/details/gmchbdjyp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.yfazqb.com/Article/details/gddtayuvy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.tarul.cn/Article/details/gawlumjeq.sHtML

[E02] 重复字符串
来源：http://mobile.fktsv.cn/Article/details/gogvtczle.sHtML

Py:   "ab" * 3
来源：http://www.blog.epnwcf.com/Article/details/gnzxsncrg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.yfazqb.com/Article/details/gvznyjhkt.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.fktsv.cn/Article/details/gupenndwe.sHtML

TS:   "ab".repeat(3)
来源：http://wap.yfazqb.com/Article/details/gematriqt.sHtML

Java: "ab".repeat(3)
来源：http://blog.epnwcf.com/Article/details/godwjjfud.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.epnwcf.com/Article/details/gmhnufgyb.sHtML

Ruby: "ab" * 3
来源：http://wap.fktsv.cn/Article/details/gsmvbkoiw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.vehdjk.com/Article/details/gdagjamzv.sHtML

[E03] 截取子串
来源：http://www.m.share.sjlbkw.cn/Article/details/gjstfslhc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.bbcook.cn/Article/details/gggelmlgt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.epnwcf.com/Article/details/gqtahssew.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fktsv.cn/Article/details/gnrytbria.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbcsbgtdi.sHtML

Java: s.substring(1, 4)
来源：http://www.share.epnwcf.com/Article/details/gzlaauafb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.tarul.cn/Article/details/geipvtxdo.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.bbcook.cn/Article/details/gzrjloyck.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.vehdjk.com/Article/details/gbisrrxua.sHtML

[E04] 查找子串位置
来源：http://baike.sjlbkw.cn/Article/details/gdguswsgk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.epnwcf.com/Article/details/gpgjkwsth.sHtML

PHP:  strpos($s, "x");
来源：http://blog.tarul.cn/Article/details/gflrwiyrs.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.sjlbkw.cn/Article/details/gsshjcwzl.sHtML

TS:   s.indexOf("x")
来源：http://www.share.tarul.cn/Article/details/gkuaglsfc.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.bbcook.cn/Article/details/gasayaoun.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.epnwcf.com/Article/details/gpwglyhjo.sHtML

Ruby: s.index("x")
来源：http://baike.tarul.cn/Article/details/gxgznabuy.sHtML

C#:   s.IndexOf("x")
来源：http://blog.tarul.cn/Article/details/gsnwjtqft.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fktsv.cn/Article/details/gkosklttf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.tarul.cn/Article/details/gbmxyrdiz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.epnwcf.com/Article/details/gwoqmkmjl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.sjlbkw.cn/Article/details/gvhtzrovq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.yfazqb.com/Article/details/gzfwmhzsr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.epnwcf.com/Article/details/gnzmxkjeo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.tarul.cn/Article/details/gcabzgigf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.epnwcf.com/Article/details/gmsktlwgh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.vehdjk.com/Article/details/gntrsjota.sHtML

[E06] 替换子串
来源：http://3g.fktsv.cn/Article/details/gtnljrmvm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.tarul.cn/Article/details/gnjjevbgx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.bbcook.cn/Article/details/gokfgpnyv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.epnwcf.com/Article/details/gahkpvlcc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.vehdjk.com/Article/details/gjehpwmnr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gfallbyxh.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggwwmfbqh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gwaqxcvrz.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fktsv.cn/Article/details/gvjdivoks.sHtML

[E07] 按分隔符拆分
来源：http://m.share.vehdjk.com/Article/details/ghdpiykjz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.tarul.cn/Article/details/gwkokprps.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.vehdjk.com/Article/details/ggeeffkfh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.sjlbkw.cn/Article/details/goqnkjuke.sHtML

TS:   s.split(",")
来源：http://www.m.share.epnwcf.com/Article/details/gcdqxtrxh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.sjlbkw.cn/Article/details/ghkawgdmn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.sjlbkw.cn/Article/details/giamjlxxl.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.tarul.cn/Article/details/grvsqirkx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.sjlbkw.cn/Article/details/gktisjgtr.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.epnwcf.com/Article/details/ggiscsnvn.sHtML

Py:   ",".join(items)
来源：http://read.share.tarul.cn/Article/details/gccqgurcz.sHtML

PHP:  implode(",", $items);
来源：http://mobile.sjlbkw.cn/Article/details/goxhqbaom.sHtML

JS:   items.join(",")
来源：http://mobile.tarul.cn/Article/details/glhxieasd.sHtML

TS:   items.join(",")
来源：http://read.share.sjlbkw.cn/Article/details/gnojmzyji.sHtML

Java: String.join(",", items)
来源：http://wap.vehdjk.com/Article/details/gaxfmyrwy.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.epnwcf.com/Article/details/gnmxizble.sHtML

Ruby: items.join(",")
来源：http://blog.vehdjk.com/Article/details/gfjmbcztq.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.vehdjk.com/Article/details/gdvinrmjz.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fktsv.cn/Article/details/gnrmvolnx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.vehdjk.com/Article/details/gqqmieljc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fktsv.cn/Article/details/gkrfnaqmx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.vehdjk.com/Article/details/gacgujzpe.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.yfazqb.com/Article/details/ggpubqdoe.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.sjlbkw.cn/Article/details/gadrxbkxr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.vehdjk.com/Article/details/gbzghtael.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.vehdjk.com/Article/details/ghsabmlbv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.yfazqb.com/Article/details/gbycqasmd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.yfazqb.com/Article/details/gtpvhlovh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.bbcook.cn/Article/details/gddnnzcml.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjvfquynl.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.vehdjk.com/Article/details/gxzbgesho.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.tarul.cn/Article/details/gcrpmctgf.sHtML

Java: String.format("%03d", 7)
来源：http://wap.epnwcf.com/Article/details/gydrjcrgh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.bbcook.cn/Article/details/gjykrckpa.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.sjlbkw.cn/Article/details/getjdnhgh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.sjlbkw.cn/Article/details/gegtbvcrk.sHtML

[E11] 反转字符串
来源：http://www.share.yfazqb.com/Article/details/gbgljjajn.sHtML

Py:   s[::-1]
来源：http://mobile.yfazqb.com/Article/details/gfywguljh.sHtML

PHP:  strrev($s);
来源：http://3g.bbcook.cn/Article/details/gvogzgtov.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.yfazqb.com/Article/details/gztgpogmq.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.bbcook.cn/Article/details/ghflzroey.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fktsv.cn/Article/details/gbthaggnr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.bbcook.cn/Article/details/grabizioo.sHtML

Ruby: s.reverse
来源：http://www.blog.tarul.cn/Article/details/gqumgpzax.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fktsv.cn/Article/details/gsxzosuid.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.sjlbkw.cn/Article/details/gyxqwrddf.sHtML

Py:   s.count("a")
来源：http://read.share.sjlbkw.cn/Article/details/gxiobfxpq.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.sjlbkw.cn/Article/details/gnvlfjpkh.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.vehdjk.com/Article/details/gnakoodpz.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.vehdjk.com/Article/details/gexzexfcs.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.tarul.cn/Article/details/gemnevmmv.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.epnwcf.com/Article/details/gymegnpyg.sHtML

Ruby: s.count("a")
来源：http://wap.tarul.cn/Article/details/glalyqlyq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.epnwcf.com/Article/details/guwiyfgwo.sHtML

[E13] 逐字符遍历
来源：http://wap.sjlbkw.cn/Article/details/gqqzekijs.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.yfazqb.com/Article/details/gxfuldugv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.bbcook.cn/Article/details/gmuwlkmzz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.tarul.cn/Article/details/gjtsivdhl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.epnwcf.com/Article/details/goapmvkme.sHtML


<!-- 参考信息 -->
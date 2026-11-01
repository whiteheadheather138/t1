代发 wailian999

[D07] 切片 / 取子数组
来源：http://www.share.tarul.cn/Article/details/gnhfuusxy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.sjlbkw.cn/Article/details/gyoioaqbv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.epnwcf.com/Article/details/gmnguavzx.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fktsv.cn/Article/details/gcygwipbc.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.vehdjk.com/Article/details/gyhkvcbpx.sHtML

Java: list.subList(1, 4);
来源：http://3g.tarul.cn/Article/details/gahfjoeyk.sHtML

Go:   arr[1:4]
来源：http://blog.bbcook.cn/Article/details/gauwwaozb.sHtML

Ruby: arr[1, 3]
来源：http://mobile.bbcook.cn/Article/details/gqybuyskd.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.tarul.cn/Article/details/geydkaxto.sHtML

[D08] 合并两个数组
来源：http://m.share.epnwcf.com/Article/details/gsjgygczc.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.yfazqb.com/Article/details/gklcvlyyb.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.bbcook.cn/Article/details/ggbqjfkje.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.epnwcf.com/Article/details/ggvyyrodr.sHtML

TS:   [...a, ...b];
来源：http://www.share.tarul.cn/Article/details/gpqtofcwj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.bbcook.cn/Article/details/gmpvbrgzl.sHtML

Go:   append(a, b...)
来源：http://wap.sjlbkw.cn/Article/details/gkmpmybjw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.sjlbkw.cn/Article/details/gcwglcjxr.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.yfazqb.com/Article/details/gfryxkeyn.sHtML

[D09] 排序（升序）
来源：http://blog.sjlbkw.cn/Article/details/gcmpclbhd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.bbcook.cn/Article/details/gcadthhrb.sHtML

PHP:  sort($arr);
来源：http://m.share.tarul.cn/Article/details/grqsjfmai.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fktsv.cn/Article/details/gqlwzgytn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.epnwcf.com/Article/details/gqgdnhncx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fktsv.cn/Article/details/gebtjraji.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gjfbndhqo.sHtML

Ruby: arr.sort
来源：http://mobile.yfazqb.com/Article/details/ggqajtkjt.sHtML

C#:   list.Sort();
来源：http://m.share.vehdjk.com/Article/details/gfbwlyhqb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.tarul.cn/Article/details/getmkshps.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.bbcook.cn/Article/details/gnqfvvxrv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.vehdjk.com/Article/details/gaehynbce.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.epnwcf.com/Article/details/gxwckrqul.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.vehdjk.com/Article/details/gxkyhxnij.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.epnwcf.com/Article/details/gauakdrnb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.tarul.cn/Article/details/gekdbegbh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fktsv.cn/Article/details/gnadupnkj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.sjlbkw.cn/Article/details/gvookvszy.sHtML

[D11] 反转数组
来源：http://wap.epnwcf.com/Article/details/gnukyurll.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.sjlbkw.cn/Article/details/gwjxkxwbd.sHtML

PHP:  array_reverse($arr);
来源：http://3g.tarul.cn/Article/details/gesqhdcln.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fktsv.cn/Article/details/gcbolcniy.sHtML

TS:   [...arr].reverse();
来源：http://3g.yfazqb.com/Article/details/gxkhfpwjv.sHtML

Java: Collections.reverse(list);
来源：http://www.share.bbcook.cn/Article/details/grdxywfsj.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.yfazqb.com/Article/details/gsjkvhmim.sHtML

Ruby: arr.reverse
来源：http://blog.tarul.cn/Article/details/gwrofupvl.sHtML

C#:   list.Reverse();
来源：http://blog.tarul.cn/Article/details/gdcnijuyk.sHtML

[D12] 查找元素下标
来源：http://www.m.share.yfazqb.com/Article/details/gprqdehbu.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.bbcook.cn/Article/details/gwufuujkw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.tarul.cn/Article/details/ghtzowtbo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fktsv.cn/Article/details/gelqexfpx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.bbcook.cn/Article/details/ghwxyztpi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.tarul.cn/Article/details/gzkibpvpb.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/gvonnynzc.sHtML

Ruby: arr.index(x)
来源：http://www.share.bbcook.cn/Article/details/gxlxrykph.sHtML

C#:   list.IndexOf(x);
来源：http://blog.bbcook.cn/Article/details/ggaphtyuk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.yfazqb.com/Article/details/gthnzhuaz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.bbcook.cn/Article/details/gkzcbjrip.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.vehdjk.com/Article/details/gusvnfiyu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.vehdjk.com/Article/details/gzkezblff.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.epnwcf.com/Article/details/grkpmlicc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.sjlbkw.cn/Article/details/gttbetidm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.epnwcf.com/Article/details/gooaqrkop.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.tarul.cn/Article/details/gzlsjgswh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.vehdjk.com/Article/details/gdqrjysvk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.bbcook.cn/Article/details/gufpfqtxb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.sjlbkw.cn/Article/details/gcfdmliwl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.vehdjk.com/Article/details/gisvzgrto.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fktsv.cn/Article/details/gkejyhxjc.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.bbcook.cn/Article/details/gvtboiwlo.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.epnwcf.com/Article/details/gfutwjslm.sHtML

Go:   // 手写循环
来源：http://www.blog.tarul.cn/Article/details/gvrcgfhjm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.vehdjk.com/Article/details/gflsjicjc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.yfazqb.com/Article/details/gecfkazjz.sHtML

[D15] 去重
来源：http://www.m.share.bbcook.cn/Article/details/gtqgsvjdy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.tarul.cn/Article/details/gngshevwx.sHtML

PHP:  array_unique($arr);
来源：http://wap.bbcook.cn/Article/details/grkyugiwh.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.yfazqb.com/Article/details/gucxfyuob.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.tarul.cn/Article/details/ggpzzaygz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.sjlbkw.cn/Article/details/grpxnzmpp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.sjlbkw.cn/Article/details/gdzkkumgd.sHtML

Ruby: arr.uniq
来源：http://wap.epnwcf.com/Article/details/gvzqosyae.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fktsv.cn/Article/details/gydlpjqlq.sHtML

[D16] 求和与平均值
来源：http://read.share.fktsv.cn/Article/details/gyopmassa.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.epnwcf.com/Article/details/gzejreuhh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fktsv.cn/Article/details/gfwxgwryu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.vehdjk.com/Article/details/gsqrbfqmd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.bbcook.cn/Article/details/gqchmzdxr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.bbcook.cn/Article/details/gacgcguog.sHtML

Go:   // 手写循环累加
来源：http://www.share.sjlbkw.cn/Article/details/gztwdyxye.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.bbcook.cn/Article/details/gpzzmduew.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.vehdjk.com/Article/details/gyvsgnpwq.sHtML

[D17] 最大值与最小值
来源：http://mobile.tarul.cn/Article/details/glvovjqab.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.bbcook.cn/Article/details/gaxrpucxl.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.bbcook.cn/Article/details/gdnosdvko.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.sjlbkw.cn/Article/details/gkzczdnof.sHtML

TS:   Math.max(...arr);
来源：http://read.share.vehdjk.com/Article/details/gvrmzpsai.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.vehdjk.com/Article/details/gypozgbzj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.sjlbkw.cn/Article/details/gsgximhgn.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.epnwcf.com/Article/details/gmweecion.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.yfazqb.com/Article/details/gpqkxwpqp.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fktsv.cn/Article/details/gjuhoehuw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.tarul.cn/Article/details/gfygvrhqi.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.yfazqb.com/Article/details/gnthdoovx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.bbcook.cn/Article/details/grehsrjdz.sHtML

TS:   nested.flat();
来源：http://wap.bbcook.cn/Article/details/ghlzrqwkc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.vehdjk.com/Article/details/gtpsnugzj.sHtML

Go:   // 手写双层循环
来源：http://www.share.sjlbkw.cn/Article/details/gtvybwgtd.sHtML

Ruby: nested.flatten
来源：http://mobile.vehdjk.com/Article/details/gnenatltn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.sjlbkw.cn/Article/details/gwsyzacaj.sHtML

[D19] 按字段分组
来源：http://wap.fktsv.cn/Article/details/gpsfagbrp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fktsv.cn/Article/details/gcsziyqbj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.bbcook.cn/Article/details/gxctyqqin.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.vehdjk.com/Article/details/gkwfgzyxh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.bbcook.cn/Article/details/gnqwafkxt.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.vehdjk.com/Article/details/gecyznlhs.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.yfazqb.com/Article/details/gwvnrhxug.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.epnwcf.com/Article/details/gystklztc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.vehdjk.com/Article/details/gycajhlrj.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.tarul.cn/Article/details/ggluwmztu.sHtML

Py:   Counter(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggkwmkaua.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.vehdjk.com/Article/details/gqlscwscu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.epnwcf.com/Article/details/gvnnwpqsb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.vehdjk.com/Article/details/geneugygq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.epnwcf.com/Article/details/guhqosxje.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.bbcook.cn/Article/details/gdgbelqka.sHtML

Ruby: arr.tally
来源：http://www.share.yfazqb.com/Article/details/gbytwtlws.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.yfazqb.com/Article/details/gicxbwmfe.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.epnwcf.com/Article/details/gixciswuu.sHtML

Py:   x in arr
来源：http://wap.yfazqb.com/Article/details/ghvvoclzw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fktsv.cn/Article/details/gpsxoivzo.sHtML

JS:   arr.includes(x)
来源：http://www.blog.yfazqb.com/Article/details/gtcpspdox.sHtML

TS:   arr.includes(x)
来源：http://www.blog.vehdjk.com/Article/details/giptqvwhz.sHtML

Java: list.contains(x)
来源：http://wap.sjlbkw.cn/Article/details/ggonjlyex.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gzwqxxicd.sHtML

Ruby: arr.include?(x)
来源：http://wap.yfazqb.com/Article/details/gdxgfruhq.sHtML

C#:   list.Contains(x)
来源：http://wap.yfazqb.com/Article/details/garjvpvuk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.tarul.cn/Article/details/gxurogmow.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.vehdjk.com/Article/details/glpyqemud.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fktsv.cn/Article/details/gxqbpyutg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.bbcook.cn/Article/details/gwzzlwcyi.sHtML

TS:   [...arr];
来源：http://blog.epnwcf.com/Article/details/gjcyhhrtb.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.tarul.cn/Article/details/gfzqyrcqh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fktsv.cn/Article/details/ghfcogmzl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.tarul.cn/Article/details/gadwienvk.sHtML

C#:   new List<int>(list);
来源：http://baike.bbcook.cn/Article/details/gvsbibwes.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.epnwcf.com/Article/details/gmjyayznl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.tarul.cn/Article/details/gjsddtakw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.bbcook.cn/Article/details/glryvsans.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.tarul.cn/Article/details/gavkxagki.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.tarul.cn/Article/details/ggmkrmeor.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.yfazqb.com/Article/details/gcbqepxzw.sHtML

Go:   // 手写循环
来源：http://wap.sjlbkw.cn/Article/details/gnpmjdjwr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.epnwcf.com/Article/details/gmucluxak.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.epnwcf.com/Article/details/gudhxbkqz.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.vehdjk.com/Article/details/gokgutmeo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.vehdjk.com/Article/details/gpnbnbrlu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.bbcook.cn/Article/details/gaqpyrczj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.epnwcf.com/Article/details/gpzqerlii.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.bbcook.cn/Article/details/glhzxhnfm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.vehdjk.com/Article/details/grlsozrzw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.epnwcf.com/Article/details/gnzgfgmtv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.vehdjk.com/Article/details/gamkvyisx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.yfazqb.com/Article/details/glruiuseo.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.yfazqb.com/Article/details/gqznqfqaj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fktsv.cn/Article/details/gkeznxygv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.yfazqb.com/Article/details/gxduzqxug.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.yfazqb.com/Article/details/gbthbuenu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fktsv.cn/Article/details/gurcaomrn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fktsv.cn/Article/details/gziyichcf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.sjlbkw.cn/Article/details/gtbtdqfzj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fktsv.cn/Article/details/ggxgtwtzk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.bbcook.cn/Article/details/gsexskfpc.sHtML

[D26] 数组转字符串
来源：http://blog.tarul.cn/Article/details/gtesntejb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.sjlbkw.cn/Article/details/gficpkisc.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.bbcook.cn/Article/details/gwdyxigga.sHtML

JS:   arr.join(", ")
来源：http://www.share.tarul.cn/Article/details/gflnhghqt.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.epnwcf.com/Article/details/goaxtbega.sHtML

Java: String.join(", ", list)
来源：http://baike.fktsv.cn/Article/details/gkzfwdjld.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.yfazqb.com/Article/details/gharqrwxc.sHtML

Ruby: arr.join(", ")
来源：http://mobile.tarul.cn/Article/details/gqhfkwsdz.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.vehdjk.com/Article/details/gxtgrvsga.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gdcgpixid.sHtML

E. 字符串处理
来源：http://www.blog.epnwcf.com/Article/details/gxvzljmyz.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gvortwlok.sHtML

[E01] 拼接字符串
来源：http://3g.bbcook.cn/Article/details/grpikskug.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.sjlbkw.cn/Article/details/gasqfkotd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.vehdjk.com/Article/details/gocmxjuxz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.vehdjk.com/Article/details/ghiqvncaj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.bbcook.cn/Article/details/ggfrycnfk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.yfazqb.com/Article/details/glnjitonu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.bbcook.cn/Article/details/glhbcmzgy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.vehdjk.com/Article/details/gznmchacy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.bbcook.cn/Article/details/gwkiaaahe.sHtML

[E02] 重复字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gmduouoje.sHtML

Py:   "ab" * 3
来源：http://www.share.tarul.cn/Article/details/gurrkxdme.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.tarul.cn/Article/details/gsemrpgjy.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.vehdjk.com/Article/details/gfqueqrks.sHtML

TS:   "ab".repeat(3)
来源：http://baike.tarul.cn/Article/details/gydvjslrs.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.yfazqb.com/Article/details/gujgpelmh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.yfazqb.com/Article/details/gbgccfxpj.sHtML

Ruby: "ab" * 3
来源：http://www.blog.bbcook.cn/Article/details/gtlfanucp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.yfazqb.com/Article/details/goqhbvbsa.sHtML

[E03] 截取子串
来源：http://wap.epnwcf.com/Article/details/gounetdql.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.yfazqb.com/Article/details/gkifwszfx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.sjlbkw.cn/Article/details/gweeqeyxi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.bbcook.cn/Article/details/gmdjlehrp.sHtML

TS:   s.slice(1, 4)
来源：http://blog.tarul.cn/Article/details/gffcrsbnx.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.yfazqb.com/Article/details/gxrjnyghm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.epnwcf.com/Article/details/gzavgcdyz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.tarul.cn/Article/details/gwgdnjhrs.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.vehdjk.com/Article/details/gfctwlxcu.sHtML

[E04] 查找子串位置
来源：http://www.share.sjlbkw.cn/Article/details/gddtvmnxq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.vehdjk.com/Article/details/ggiszebzd.sHtML

PHP:  strpos($s, "x");
来源：http://wap.vehdjk.com/Article/details/gyzgaeuup.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.sjlbkw.cn/Article/details/gcljnluth.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.vehdjk.com/Article/details/gjqlobzlv.sHtML

Java: s.indexOf("x")
来源：http://wap.vehdjk.com/Article/details/gxelljffq.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.yfazqb.com/Article/details/gfvssgthw.sHtML

Ruby: s.index("x")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqedgykhv.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.sjlbkw.cn/Article/details/ghkprfbaf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.sjlbkw.cn/Article/details/gyohjxhvb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.fktsv.cn/Article/details/ggpzapoca.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.sjlbkw.cn/Article/details/gviyracxb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.epnwcf.com/Article/details/grkqhfjml.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.tarul.cn/Article/details/ghmukikoa.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.sjlbkw.cn/Article/details/gtwslwdlr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.yfazqb.com/Article/details/gnpriognh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.tarul.cn/Article/details/gzgiongnl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.vehdjk.com/Article/details/gldenxool.sHtML

[E06] 替换子串
来源：http://www.share.bbcook.cn/Article/details/gdctlwkcz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.sjlbkw.cn/Article/details/ggwsostoc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.tarul.cn/Article/details/gcwmeidxq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gjlxqfysc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fktsv.cn/Article/details/gfpxrulqh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/glrnefnij.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.vehdjk.com/Article/details/gwducayan.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.tarul.cn/Article/details/gclrijity.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.tarul.cn/Article/details/gserocpnd.sHtML

[E07] 按分隔符拆分
来源：http://wap.fktsv.cn/Article/details/gfieoeezq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.yfazqb.com/Article/details/ggbnujsri.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.tarul.cn/Article/details/gxmfpznjw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.epnwcf.com/Article/details/gyyviidgf.sHtML

TS:   s.split(",")
来源：http://www.blog.fktsv.cn/Article/details/gvtbeoncf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.vehdjk.com/Article/details/grfvmbtep.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.yfazqb.com/Article/details/grpqgyvnl.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.vehdjk.com/Article/details/gxkuwrcbv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.tarul.cn/Article/details/gcxburrxo.sHtML

[E08] 数组按分隔符合并
来源：http://3g.epnwcf.com/Article/details/gdxjenloq.sHtML

Py:   ",".join(items)
来源：http://blog.yfazqb.com/Article/details/gbbtdunpa.sHtML

PHP:  implode(",", $items);
来源：http://wap.yfazqb.com/Article/details/gwsyugplq.sHtML

JS:   items.join(",")
来源：http://baike.yfazqb.com/Article/details/gpbyjhumv.sHtML

TS:   items.join(",")
来源：http://blog.bbcook.cn/Article/details/gtoyjcmbh.sHtML

Java: String.join(",", items)
来源：http://blog.sjlbkw.cn/Article/details/gnqejnfbn.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.epnwcf.com/Article/details/gimwjmuvk.sHtML

Ruby: items.join(",")
来源：http://m.share.epnwcf.com/Article/details/gjiehhtxy.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.epnwcf.com/Article/details/gxkwkpxws.sHtML

[E09] 去除所有空白字符
来源：http://wap.epnwcf.com/Article/details/gjhkmvnnk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.sjlbkw.cn/Article/details/ghdufyqjx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.tarul.cn/Article/details/ggrxbjkxk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.vehdjk.com/Article/details/gzixgsxck.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.epnwcf.com/Article/details/gxroyfocz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.yfazqb.com/Article/details/gzhjgljjp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.epnwcf.com/Article/details/gqquxmcxx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.tarul.cn/Article/details/gcrtmzbso.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.sjlbkw.cn/Article/details/gjdaibgkd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.sjlbkw.cn/Article/details/gfvucobea.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.vehdjk.com/Article/details/gqxvapyov.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.vehdjk.com/Article/details/gvhojhngs.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.bbcook.cn/Article/details/gxahmctad.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.yfazqb.com/Article/details/gcygccxpd.sHtML

Java: String.format("%03d", 7)
来源：http://wap.epnwcf.com/Article/details/gsjmmniec.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.sjlbkw.cn/Article/details/gmzwcxpcp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.vehdjk.com/Article/details/gotsiaaky.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.vehdjk.com/Article/details/gwkeyvest.sHtML

[E11] 反转字符串
来源：http://blog.sjlbkw.cn/Article/details/gspcvssqo.sHtML

Py:   s[::-1]
来源：http://baike.sjlbkw.cn/Article/details/gfstofraz.sHtML

PHP:  strrev($s);
来源：http://mobile.tarul.cn/Article/details/gdjomvkoq.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/gimpordhn.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fktsv.cn/Article/details/gzaixmwgf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.vehdjk.com/Article/details/gabrqxegw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.sjlbkw.cn/Article/details/ggwgranfr.sHtML

Ruby: s.reverse
来源：http://m.share.sjlbkw.cn/Article/details/gtukdhimd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.bbcook.cn/Article/details/gluenwhzh.sHtML

[E12] 统计某字符出现次数
来源：http://3g.bbcook.cn/Article/details/gzorgeygg.sHtML

Py:   s.count("a")
来源：http://3g.vehdjk.com/Article/details/gcpngxsfx.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.yfazqb.com/Article/details/gjeesdukc.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.tarul.cn/Article/details/gxyiuwjcv.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.yfazqb.com/Article/details/gtbwxyyvy.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.sjlbkw.cn/Article/details/gicggumzq.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.sjlbkw.cn/Article/details/gahganirr.sHtML

Ruby: s.count("a")
来源：http://www.blog.vehdjk.com/Article/details/gbeojwwkq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.vehdjk.com/Article/details/ghwatygut.sHtML

[E13] 逐字符遍历
来源：http://www.share.tarul.cn/Article/details/gfecxxbhc.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.yfazqb.com/Article/details/gootmkytf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.yfazqb.com/Article/details/glftuyxuy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fktsv.cn/Article/details/gkywmeyob.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.sjlbkw.cn/Article/details/gnwdicozr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fktsv.cn/Article/details/gjayvmpun.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.tarul.cn/Article/details/gzmqfpdvc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.sjlbkw.cn/Article/details/gyjamllio.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.sjlbkw.cn/Article/details/gzylauppn.sHtML


<!-- 参考信息 -->
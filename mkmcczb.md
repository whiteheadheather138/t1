代发 wailian999

[D07] 切片 / 取子数组
来源：http://www.share.bbcook.cn/Article/details/gahwggwns.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.sjlbkw.cn/Article/details/ghpwbgqzy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.bbcook.cn/Article/details/gytbqbygi.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.tarul.cn/Article/details/gxempyfuu.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.bbcook.cn/Article/details/gvnmpwwjb.sHtML

Java: list.subList(1, 4);
来源：http://3g.yfazqb.com/Article/details/ghuvtudzp.sHtML

Go:   arr[1:4]
来源：http://blog.yfazqb.com/Article/details/ghklgoerb.sHtML

Ruby: arr[1, 3]
来源：http://mobile.tarul.cn/Article/details/gxnrkhqlc.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.bbcook.cn/Article/details/grahgwzof.sHtML

[D08] 合并两个数组
来源：http://www.blog.vehdjk.com/Article/details/gqgjuhfac.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.vehdjk.com/Article/details/gunedngxe.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.yfazqb.com/Article/details/gxyupezxj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.sjlbkw.cn/Article/details/gzcomtuct.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.epnwcf.com/Article/details/gdkqgpbql.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.bbcook.cn/Article/details/gdgatycsy.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fktsv.cn/Article/details/glmfvddmc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.bbcook.cn/Article/details/gmindkple.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.vehdjk.com/Article/details/gqcwbqecw.sHtML

[D09] 排序（升序）
来源：http://read.share.epnwcf.com/Article/details/ggclhcvlx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.epnwcf.com/Article/details/gbqjwzywf.sHtML

PHP:  sort($arr);
来源：http://read.share.bbcook.cn/Article/details/gloxiqosq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.bbcook.cn/Article/details/gtexnhwux.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fktsv.cn/Article/details/gytfmjoup.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.bbcook.cn/Article/details/gnrdklqwt.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.yfazqb.com/Article/details/gfwhvwphj.sHtML

Ruby: arr.sort
来源：http://blog.epnwcf.com/Article/details/gzktlogxp.sHtML

C#:   list.Sort();
来源：http://mobile.fktsv.cn/Article/details/gqrnokaho.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.vehdjk.com/Article/details/gowgsetbn.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.epnwcf.com/Article/details/ghjowwvgd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.vehdjk.com/Article/details/gnhxsbhuf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fktsv.cn/Article/details/gtuljlvwg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.sjlbkw.cn/Article/details/glscnzziz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fktsv.cn/Article/details/ghjxjsufw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fktsv.cn/Article/details/gppuwfatb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fktsv.cn/Article/details/geyubenct.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.vehdjk.com/Article/details/gunzalbfj.sHtML

[D11] 反转数组
来源：http://www.blog.bbcook.cn/Article/details/gbshwsget.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.epnwcf.com/Article/details/gqbqifwdw.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.vehdjk.com/Article/details/gkdulgzjz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.vehdjk.com/Article/details/gssmxtvhn.sHtML

TS:   [...arr].reverse();
来源：http://m.share.tarul.cn/Article/details/gynedufew.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.vehdjk.com/Article/details/gftlzcfzq.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.bbcook.cn/Article/details/gpihlrjku.sHtML

Ruby: arr.reverse
来源：http://3g.epnwcf.com/Article/details/gluhzvyvj.sHtML

C#:   list.Reverse();
来源：http://www.share.tarul.cn/Article/details/gsvcliqwa.sHtML

[D12] 查找元素下标
来源：http://baike.vehdjk.com/Article/details/ggvznxxsx.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.vehdjk.com/Article/details/gzclzupoe.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkdbdhlpq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.sjlbkw.cn/Article/details/gjuehozdn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.epnwcf.com/Article/details/guoeiyehk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.epnwcf.com/Article/details/gxabivvax.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gusttdepy.sHtML

Ruby: arr.index(x)
来源：http://wap.vehdjk.com/Article/details/gmjvashcl.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fktsv.cn/Article/details/gipltoufy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.tarul.cn/Article/details/gquxowpwk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.vehdjk.com/Article/details/gfklcuhkw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.yfazqb.com/Article/details/gsgfdthqa.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.tarul.cn/Article/details/gqzklaprw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.tarul.cn/Article/details/gebegfnss.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.bbcook.cn/Article/details/gdgkpynmz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.yfazqb.com/Article/details/gtdynncqd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.bbcook.cn/Article/details/gynwvvpih.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.tarul.cn/Article/details/gwkruhbty.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.tarul.cn/Article/details/grmuiqsdx.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fktsv.cn/Article/details/gggbenbuv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.tarul.cn/Article/details/gmnjfhdpv.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.vehdjk.com/Article/details/ggkgtyqvq.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.sjlbkw.cn/Article/details/gmufrnmow.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.epnwcf.com/Article/details/gibibemcu.sHtML

Go:   // 手写循环
来源：http://mobile.yfazqb.com/Article/details/grgkpjvwz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.tarul.cn/Article/details/gafzeihxx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.bbcook.cn/Article/details/gmjusudyj.sHtML

[D15] 去重
来源：http://mobile.fktsv.cn/Article/details/gjnnnbwxg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.yfazqb.com/Article/details/gyrupzptw.sHtML

PHP:  array_unique($arr);
来源：http://3g.tarul.cn/Article/details/gdgpdowtj.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.yfazqb.com/Article/details/gghqrflwr.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.yfazqb.com/Article/details/gggivbtel.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.bbcook.cn/Article/details/gvshluqxm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.yfazqb.com/Article/details/govbatrfo.sHtML

Ruby: arr.uniq
来源：http://3g.vehdjk.com/Article/details/gpptjwmjl.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.sjlbkw.cn/Article/details/gkpjwecou.sHtML

[D16] 求和与平均值
来源：http://www.blog.tarul.cn/Article/details/glzqvdboj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gbugthlgg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.tarul.cn/Article/details/glsceuqrb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fktsv.cn/Article/details/gyzdfwlsp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.vehdjk.com/Article/details/ghzxfcfdj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.yfazqb.com/Article/details/giqunnzop.sHtML

Go:   // 手写循环累加
来源：http://www.blog.yfazqb.com/Article/details/gagalgjwt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.yfazqb.com/Article/details/gznvclnkz.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.vehdjk.com/Article/details/gyurfzpiy.sHtML

[D17] 最大值与最小值
来源：http://mobile.tarul.cn/Article/details/gqpumndwy.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.tarul.cn/Article/details/gfsyidqbi.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gftyutsdg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fktsv.cn/Article/details/gpxxixzuy.sHtML

TS:   Math.max(...arr);
来源：http://wap.epnwcf.com/Article/details/gwocqbnwl.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.epnwcf.com/Article/details/ghxpipsow.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.epnwcf.com/Article/details/gobutgeak.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fktsv.cn/Article/details/gdfhjrozj.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.epnwcf.com/Article/details/gajxmfaoc.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.sjlbkw.cn/Article/details/gypdjmptn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.vehdjk.com/Article/details/gpqytasks.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.yfazqb.com/Article/details/gmrruvpqy.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.epnwcf.com/Article/details/gtslbsgon.sHtML

TS:   nested.flat();
来源：http://m.share.bbcook.cn/Article/details/gmeqsopek.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.sjlbkw.cn/Article/details/gmatufckj.sHtML

Go:   // 手写双层循环
来源：http://blog.vehdjk.com/Article/details/gakxcfqui.sHtML

Ruby: nested.flatten
来源：http://www.blog.epnwcf.com/Article/details/gymhulqoq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.tarul.cn/Article/details/gvxqcqyrd.sHtML

[D19] 按字段分组
来源：http://www.m.share.fktsv.cn/Article/details/gewvbjadf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.vehdjk.com/Article/details/gtgizxrpo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fktsv.cn/Article/details/ggdjhbxbc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.yfazqb.com/Article/details/gesfifzen.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.bbcook.cn/Article/details/gkooimmmh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.yfazqb.com/Article/details/gxsygimtv.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.epnwcf.com/Article/details/glbojvnqa.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.epnwcf.com/Article/details/gqdxnbxdu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fktsv.cn/Article/details/gmukgwvyo.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.bbcook.cn/Article/details/gdzevimcs.sHtML

Py:   Counter(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gotksnkjg.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gorixxiff.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.epnwcf.com/Article/details/gdfojpoco.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.bbcook.cn/Article/details/gstqdmqwr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.yfazqb.com/Article/details/gflnzldww.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.tarul.cn/Article/details/gsakrdyzc.sHtML

Ruby: arr.tally
来源：http://m.share.fktsv.cn/Article/details/gqwzfktph.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.tarul.cn/Article/details/gsajfxxgb.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.tarul.cn/Article/details/gtuovowgw.sHtML

Py:   x in arr
来源：http://www.m.share.yfazqb.com/Article/details/gzwcfvhos.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.tarul.cn/Article/details/guojrhidr.sHtML

JS:   arr.includes(x)
来源：http://www.share.sjlbkw.cn/Article/details/gvkekdizk.sHtML

TS:   arr.includes(x)
来源：http://mobile.bbcook.cn/Article/details/giyfqfydr.sHtML

Java: list.contains(x)
来源：http://baike.tarul.cn/Article/details/gpxcytiiu.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsrwnascx.sHtML

Ruby: arr.include?(x)
来源：http://baike.tarul.cn/Article/details/gkbpetcda.sHtML

C#:   list.Contains(x)
来源：http://3g.bbcook.cn/Article/details/guefowljx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.sjlbkw.cn/Article/details/gxulgzoxn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.epnwcf.com/Article/details/gmmoxphlo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.epnwcf.com/Article/details/gzwfnooou.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.bbcook.cn/Article/details/gwjwmvjlw.sHtML

TS:   [...arr];
来源：http://www.blog.epnwcf.com/Article/details/gtqcskwir.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.tarul.cn/Article/details/gevwooskc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.yfazqb.com/Article/details/gqgmrhhgv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.bbcook.cn/Article/details/gstsjhgsu.sHtML

C#:   new List<int>(list);
来源：http://baike.yfazqb.com/Article/details/gqnrnfeup.sHtML

[D23] reduce 累积计算
来源：http://3g.epnwcf.com/Article/details/gzufdbxkk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.epnwcf.com/Article/details/gidqpwksl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.epnwcf.com/Article/details/ggkvrrlho.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.epnwcf.com/Article/details/gmxesznzy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.tarul.cn/Article/details/gngqlfyyo.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.vehdjk.com/Article/details/geiurbgfg.sHtML

Go:   // 手写循环
来源：http://read.share.yfazqb.com/Article/details/gmrsbicco.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.tarul.cn/Article/details/gusfiarmf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.bbcook.cn/Article/details/gczkvhfql.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.bbcook.cn/Article/details/gfzvjeybn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwobaughv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.yfazqb.com/Article/details/gntgybeel.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fktsv.cn/Article/details/gchonhltc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.sjlbkw.cn/Article/details/goenxihyh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.sjlbkw.cn/Article/details/guiqzphfr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fktsv.cn/Article/details/gcieslbcu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.sjlbkw.cn/Article/details/gwganeazc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.sjlbkw.cn/Article/details/ggpsctbcf.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.epnwcf.com/Article/details/ghbwbdoyp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fktsv.cn/Article/details/gsurxnkjl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.vehdjk.com/Article/details/gfmihndfd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.tarul.cn/Article/details/gvlwmrtpv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.epnwcf.com/Article/details/gpkcryutf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fktsv.cn/Article/details/glckutppi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.sjlbkw.cn/Article/details/ghytvzads.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.sjlbkw.cn/Article/details/gzwcqfaop.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.tarul.cn/Article/details/gfpgxebdw.sHtML

[D26] 数组转字符串
来源：http://m.share.epnwcf.com/Article/details/ggvuxobvp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.sjlbkw.cn/Article/details/gconilqud.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.sjlbkw.cn/Article/details/gtvwdcivs.sHtML

JS:   arr.join(", ")
来源：http://read.share.tarul.cn/Article/details/goxynmxby.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfusysaog.sHtML

Java: String.join(", ", list)
来源：http://3g.sjlbkw.cn/Article/details/gwxpnagmk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.bbcook.cn/Article/details/gkuntxgrf.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fktsv.cn/Article/details/goqleccul.sHtML

C#:   string.Join(", ", list)
来源：http://wap.tarul.cn/Article/details/gougbpeii.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gamgvzivl.sHtML

E. 字符串处理
来源：http://mobile.sjlbkw.cn/Article/details/gknhdholl.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gapeqjetc.sHtML

[E01] 拼接字符串
来源：http://3g.bbcook.cn/Article/details/gfulytafm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.sjlbkw.cn/Article/details/gcnsaqfmc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.epnwcf.com/Article/details/ghyvqiafk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.bbcook.cn/Article/details/gslwyoekg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.bbcook.cn/Article/details/gfrjkqitq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.vehdjk.com/Article/details/ggyxcaoqt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.vehdjk.com/Article/details/gdjyzzlrc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.sjlbkw.cn/Article/details/gfmnxcphl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gsulbnady.sHtML

[E02] 重复字符串
来源：http://read.share.epnwcf.com/Article/details/ghfowvrud.sHtML

Py:   "ab" * 3
来源：http://m.share.tarul.cn/Article/details/ggqnyauiw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.vehdjk.com/Article/details/gvcucjsxa.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fktsv.cn/Article/details/gcpbgftpw.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.yfazqb.com/Article/details/gppucgrcl.sHtML

Java: "ab".repeat(3)
来源：http://www.share.yfazqb.com/Article/details/gsnolgpvn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.vehdjk.com/Article/details/gvypxoked.sHtML

Ruby: "ab" * 3
来源：http://baike.bbcook.cn/Article/details/gpstnkzna.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.vehdjk.com/Article/details/gykofiinp.sHtML

[E03] 截取子串
来源：http://blog.fktsv.cn/Article/details/ggzlwnlab.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.bbcook.cn/Article/details/gsunurjqa.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.bbcook.cn/Article/details/gqtdrowho.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.bbcook.cn/Article/details/gbveoliek.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.vehdjk.com/Article/details/gouwphiih.sHtML

Java: s.substring(1, 4)
来源：http://wap.epnwcf.com/Article/details/gigkrcdju.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fktsv.cn/Article/details/gorkckoor.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fktsv.cn/Article/details/gnekkjbeg.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.vehdjk.com/Article/details/gphbjieqm.sHtML

[E04] 查找子串位置
来源：http://blog.yfazqb.com/Article/details/gnxrvagbn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.sjlbkw.cn/Article/details/gqqvgjmdp.sHtML

PHP:  strpos($s, "x");
来源：http://3g.vehdjk.com/Article/details/gztqxidhq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.bbcook.cn/Article/details/gucslhche.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.bbcook.cn/Article/details/gnorwfudb.sHtML

Java: s.indexOf("x")
来源：http://mobile.bbcook.cn/Article/details/gcwhapjur.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.epnwcf.com/Article/details/geymrwuyl.sHtML

Ruby: s.index("x")
来源：http://www.share.fktsv.cn/Article/details/gayohdqpn.sHtML

C#:   s.IndexOf("x")
来源：http://baike.bbcook.cn/Article/details/gwaspnbjg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fktsv.cn/Article/details/gzisvptvd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.fktsv.cn/Article/details/gqlalsaca.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.vehdjk.com/Article/details/glfhpgfvt.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.epnwcf.com/Article/details/gpxzcbizy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.bbcook.cn/Article/details/gbwvlcfsk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.epnwcf.com/Article/details/gngqkewuz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fktsv.cn/Article/details/gsbqqlnap.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.bbcook.cn/Article/details/gbwgffffx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.bbcook.cn/Article/details/gbwsqjeke.sHtML

[E06] 替换子串
来源：http://read.share.vehdjk.com/Article/details/gfgrphzxj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fktsv.cn/Article/details/gtxhtzcwy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.bbcook.cn/Article/details/glskgnmxc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/gtkkfpwmh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.tarul.cn/Article/details/gvzigysjq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gzlhvcnjq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.yfazqb.com/Article/details/geamycwcx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.yfazqb.com/Article/details/gxopsjpzb.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.vehdjk.com/Article/details/giglylpqh.sHtML

[E07] 按分隔符拆分
来源：http://baike.fktsv.cn/Article/details/gatotndly.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.bbcook.cn/Article/details/gznygufww.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fktsv.cn/Article/details/ghmgkezur.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.yfazqb.com/Article/details/gobwvvigo.sHtML

TS:   s.split(",")
来源：http://read.share.tarul.cn/Article/details/gxyaovakw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.tarul.cn/Article/details/gmvtgumea.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.tarul.cn/Article/details/gvufbzphn.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.sjlbkw.cn/Article/details/gvzfneyql.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.sjlbkw.cn/Article/details/gkxxxqwds.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.bbcook.cn/Article/details/gffludkwa.sHtML

Py:   ",".join(items)
来源：http://blog.epnwcf.com/Article/details/gthkyjbst.sHtML

PHP:  implode(",", $items);
来源：http://baike.bbcook.cn/Article/details/ghhyofalb.sHtML

JS:   items.join(",")
来源：http://www.m.share.tarul.cn/Article/details/gvxuqppqm.sHtML

TS:   items.join(",")
来源：http://m.share.sjlbkw.cn/Article/details/grmmgonqy.sHtML

Java: String.join(",", items)
来源：http://blog.vehdjk.com/Article/details/gvvxasxms.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.vehdjk.com/Article/details/gdazfkhov.sHtML

Ruby: items.join(",")
来源：http://3g.epnwcf.com/Article/details/gjudnjwsf.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.tarul.cn/Article/details/gcvyguxpf.sHtML

[E09] 去除所有空白字符
来源：http://www.share.epnwcf.com/Article/details/gwoxclmpp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fktsv.cn/Article/details/ghyvscpye.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.sjlbkw.cn/Article/details/ggqufodmu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.tarul.cn/Article/details/gankmltbi.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.bbcook.cn/Article/details/gvmiejfod.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.epnwcf.com/Article/details/gnxvsdpar.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.sjlbkw.cn/Article/details/gvjlcccqp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.tarul.cn/Article/details/gtivemgxq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.sjlbkw.cn/Article/details/gwmffzsia.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.tarul.cn/Article/details/gydthxwpt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.vehdjk.com/Article/details/gqzyqezep.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.yfazqb.com/Article/details/grsxzxvbg.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.sjlbkw.cn/Article/details/gulyquadb.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.epnwcf.com/Article/details/gzilbcvlr.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.sjlbkw.cn/Article/details/guvcnihnm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gctubtche.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.sjlbkw.cn/Article/details/giprusmko.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.tarul.cn/Article/details/glbwjwzmn.sHtML

[E11] 反转字符串
来源：http://www.m.share.fktsv.cn/Article/details/gulnkbddl.sHtML

Py:   s[::-1]
来源：http://read.share.vehdjk.com/Article/details/gbqqjddho.sHtML

PHP:  strrev($s);
来源：http://3g.tarul.cn/Article/details/gljktjwwr.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.tarul.cn/Article/details/ggvaklvch.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.sjlbkw.cn/Article/details/glpnlvtub.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.yfazqb.com/Article/details/gmnaazlxz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.vehdjk.com/Article/details/gcpoutwrs.sHtML

Ruby: s.reverse
来源：http://baike.tarul.cn/Article/details/gzcvorwea.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.bbcook.cn/Article/details/gepwhufeu.sHtML

[E12] 统计某字符出现次数
来源：http://blog.tarul.cn/Article/details/ghqrwapfi.sHtML

Py:   s.count("a")
来源：http://www.share.yfazqb.com/Article/details/gvxbxvsmu.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.epnwcf.com/Article/details/gzvvgulcd.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.vehdjk.com/Article/details/gaihirovg.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fktsv.cn/Article/details/glhtzamog.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.epnwcf.com/Article/details/glbgxbjrj.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.sjlbkw.cn/Article/details/gnzzqffxh.sHtML

Ruby: s.count("a")
来源：http://blog.epnwcf.com/Article/details/gpcsjtvly.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.bbcook.cn/Article/details/gepysymnh.sHtML

[E13] 逐字符遍历
来源：http://blog.epnwcf.com/Article/details/gsqsyxrli.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.bbcook.cn/Article/details/gbjpaeily.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fktsv.cn/Article/details/gobpnldvh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.sjlbkw.cn/Article/details/ggeuwwqgi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.yfazqb.com/Article/details/gftjozkak.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.sjlbkw.cn/Article/details/gxxacvmqi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.vehdjk.com/Article/details/gyzavpbfc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.vehdjk.com/Article/details/gfyvmswbr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.tarul.cn/Article/details/ghreijrkp.sHtML


<!-- 参考信息 -->
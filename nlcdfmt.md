代发 wailian999

TS:   arr.slice(1, 4);
来源：http://mobile.sjlbkw.cn/Article/details/gbuoftbyw.sHtML

Java: list.subList(1, 4);
来源：http://blog.yfazqb.com/Article/details/gzpymrwfs.sHtML

Go:   arr[1:4]
来源：http://www.share.vehdjk.com/Article/details/gaonhpxec.sHtML

Ruby: arr[1, 3]
来源：http://3g.vehdjk.com/Article/details/gbyuozcux.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.yfazqb.com/Article/details/gducgwwst.sHtML

[D08] 合并两个数组
来源：http://m.share.vehdjk.com/Article/details/gmerzgdpw.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fktsv.cn/Article/details/goppfffmu.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.tarul.cn/Article/details/goblhgsyq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.yfazqb.com/Article/details/gpsazhpou.sHtML

TS:   [...a, ...b];
来源：http://3g.tarul.cn/Article/details/gnyghndaz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.yfazqb.com/Article/details/gvpvxhioo.sHtML

Go:   append(a, b...)
来源：http://www.m.share.epnwcf.com/Article/details/gwjxrmvce.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.bbcook.cn/Article/details/gyfgmpdkn.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.sjlbkw.cn/Article/details/golcvaiep.sHtML

[D09] 排序（升序）
来源：http://www.m.share.yfazqb.com/Article/details/gtpwnzhim.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.epnwcf.com/Article/details/gfyrzgizf.sHtML

PHP:  sort($arr);
来源：http://m.share.yfazqb.com/Article/details/gkxvkkbfd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fktsv.cn/Article/details/ggbkdqkrh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.bbcook.cn/Article/details/gmqinrnvq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.vehdjk.com/Article/details/gsumkcmiv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.tarul.cn/Article/details/gqyardzns.sHtML

Ruby: arr.sort
来源：http://www.m.share.yfazqb.com/Article/details/gqytpfqwp.sHtML

C#:   list.Sort();
来源：http://www.blog.yfazqb.com/Article/details/gipqwjbmp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.tarul.cn/Article/details/gzzvlxshz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.epnwcf.com/Article/details/gmkhtuqcg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.yfazqb.com/Article/details/gzzissejh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.bbcook.cn/Article/details/gceibuxgz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtsgnucuy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.tarul.cn/Article/details/ghwcvscgw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.tarul.cn/Article/details/gemomunvf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.vehdjk.com/Article/details/gapkvijqw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fktsv.cn/Article/details/gwoyalafp.sHtML

[D11] 反转数组
来源：http://www.blog.vehdjk.com/Article/details/gwnynmycl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.tarul.cn/Article/details/gkneolwui.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.vehdjk.com/Article/details/gpqbatrep.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.sjlbkw.cn/Article/details/grrlzebdl.sHtML

TS:   [...arr].reverse();
来源：http://wap.fktsv.cn/Article/details/giwlaxkzn.sHtML

Java: Collections.reverse(list);
来源：http://wap.bbcook.cn/Article/details/gvjusluie.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fktsv.cn/Article/details/grxymwsoc.sHtML

Ruby: arr.reverse
来源：http://baike.tarul.cn/Article/details/grjogvrrg.sHtML

C#:   list.Reverse();
来源：http://3g.epnwcf.com/Article/details/gzdoxaayv.sHtML

[D12] 查找元素下标
来源：http://wap.tarul.cn/Article/details/gpahajdgd.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.yfazqb.com/Article/details/ggwzzxogm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.tarul.cn/Article/details/gidwswjpr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fktsv.cn/Article/details/gxczgrjoe.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.epnwcf.com/Article/details/gtnkqgrpk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.epnwcf.com/Article/details/gpsnlmhig.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.tarul.cn/Article/details/gcorrdyxa.sHtML

Ruby: arr.index(x)
来源：http://read.share.sjlbkw.cn/Article/details/gbwpibxre.sHtML

C#:   list.IndexOf(x);
来源：http://blog.sjlbkw.cn/Article/details/gnssogzqz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.sjlbkw.cn/Article/details/gkwqkgzzl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.yfazqb.com/Article/details/gmugokddl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.bbcook.cn/Article/details/gszqfqsec.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.yfazqb.com/Article/details/gpveejmlo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.bbcook.cn/Article/details/gzutjvswf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.bbcook.cn/Article/details/gdafayttg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.sjlbkw.cn/Article/details/gjqtehkqo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fktsv.cn/Article/details/gyfxdhsfh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.vehdjk.com/Article/details/gadgnbncz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.epnwcf.com/Article/details/gbfldwely.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.vehdjk.com/Article/details/gegvocwuq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.yfazqb.com/Article/details/girocmlnl.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.epnwcf.com/Article/details/gxstxjedk.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fktsv.cn/Article/details/gttxvqxws.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.bbcook.cn/Article/details/getpepvpy.sHtML

Go:   // 手写循环
来源：http://3g.sjlbkw.cn/Article/details/gfesmrsjy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.bbcook.cn/Article/details/gmgxllgyo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.bbcook.cn/Article/details/gkjuhnvox.sHtML

[D15] 去重
来源：http://www.blog.yfazqb.com/Article/details/gtbqtncbb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.tarul.cn/Article/details/gxwuknzus.sHtML

PHP:  array_unique($arr);
来源：http://read.share.vehdjk.com/Article/details/glqetshmc.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fktsv.cn/Article/details/gojwzqnnh.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.epnwcf.com/Article/details/gvrzjhuwx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.vehdjk.com/Article/details/gnwttgwqq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.sjlbkw.cn/Article/details/gdpikougp.sHtML

Ruby: arr.uniq
来源：http://3g.bbcook.cn/Article/details/gapvppxil.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.epnwcf.com/Article/details/gszfvhtkw.sHtML

[D16] 求和与平均值
来源：http://read.share.epnwcf.com/Article/details/govzqgzou.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.bbcook.cn/Article/details/gmyuhebrg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.yfazqb.com/Article/details/gujjbjkoe.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.bbcook.cn/Article/details/guhxokpyh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.yfazqb.com/Article/details/gjbhchscd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.epnwcf.com/Article/details/gtxeghxhz.sHtML

Go:   // 手写循环累加
来源：http://read.share.epnwcf.com/Article/details/gfvcforaz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.yfazqb.com/Article/details/gncrqnmzy.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.yfazqb.com/Article/details/gujiayakw.sHtML

[D17] 最大值与最小值
来源：http://www.blog.sjlbkw.cn/Article/details/ggyndwdaf.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.bbcook.cn/Article/details/gexcfpxxd.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.epnwcf.com/Article/details/gavkyzytg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.epnwcf.com/Article/details/gyfrfdslr.sHtML

TS:   Math.max(...arr);
来源：http://read.share.sjlbkw.cn/Article/details/gmnivqpof.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.sjlbkw.cn/Article/details/gwjibyqaw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.tarul.cn/Article/details/gozvzonxx.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.tarul.cn/Article/details/gtmiihynk.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fktsv.cn/Article/details/gvjchyoyo.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.vehdjk.com/Article/details/gcalexkkc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fktsv.cn/Article/details/gsybrmats.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.epnwcf.com/Article/details/gclqcqhhe.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fktsv.cn/Article/details/gnhmsgesv.sHtML

TS:   nested.flat();
来源：http://3g.fktsv.cn/Article/details/gzsmbitgb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.tarul.cn/Article/details/gczldxptp.sHtML

Go:   // 手写双层循环
来源：http://blog.bbcook.cn/Article/details/gissmdfmm.sHtML

Ruby: nested.flatten
来源：http://www.m.share.tarul.cn/Article/details/gmajodknu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.tarul.cn/Article/details/gjgiaduuo.sHtML

[D19] 按字段分组
来源：http://www.share.fktsv.cn/Article/details/ggfduaxqw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.sjlbkw.cn/Article/details/ggnwcphpm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.bbcook.cn/Article/details/gtbfqsjgk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.epnwcf.com/Article/details/gkemsjipp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.bbcook.cn/Article/details/gsfjifxvy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.epnwcf.com/Article/details/gvugybjlw.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.yfazqb.com/Article/details/gxzaqbzko.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.sjlbkw.cn/Article/details/gzkhswzqe.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.vehdjk.com/Article/details/gsrjhrfiz.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.epnwcf.com/Article/details/gpeovxcql.sHtML

Py:   Counter(arr)
来源：http://blog.yfazqb.com/Article/details/gvytoopon.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.yfazqb.com/Article/details/gcbjkebbh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.sjlbkw.cn/Article/details/gslcoxkfj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.vehdjk.com/Article/details/gvzcujilq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.yfazqb.com/Article/details/ggffxkttf.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.yfazqb.com/Article/details/gawqtlrve.sHtML

Ruby: arr.tally
来源：http://wap.sjlbkw.cn/Article/details/gfzbimhqa.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.bbcook.cn/Article/details/glvgffbwi.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.yfazqb.com/Article/details/gzodpfyhy.sHtML

Py:   x in arr
来源：http://blog.tarul.cn/Article/details/gcyzlctlm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.sjlbkw.cn/Article/details/gajxaxwyy.sHtML

JS:   arr.includes(x)
来源：http://www.share.epnwcf.com/Article/details/gkgrywkzz.sHtML

TS:   arr.includes(x)
来源：http://3g.fktsv.cn/Article/details/gpvjeanij.sHtML

Java: list.contains(x)
来源：http://www.m.share.vehdjk.com/Article/details/gxrettcnl.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gxwvjkyjn.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fktsv.cn/Article/details/gsfxuofgc.sHtML

C#:   list.Contains(x)
来源：http://mobile.sjlbkw.cn/Article/details/gbxtpwosl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.vehdjk.com/Article/details/gpojiqivu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.bbcook.cn/Article/details/gbjfntsjg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.vehdjk.com/Article/details/gcjcuklrv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.yfazqb.com/Article/details/ghgdngxqv.sHtML

TS:   [...arr];
来源：http://www.blog.vehdjk.com/Article/details/gfswkuctr.sHtML

Java: new ArrayList<>(list);
来源：http://baike.yfazqb.com/Article/details/gqvxnrrqy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.yfazqb.com/Article/details/gasbiidbx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.epnwcf.com/Article/details/gtnurxnyf.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.vehdjk.com/Article/details/gzpnbyzdu.sHtML

[D23] reduce 累积计算
来源：http://read.share.sjlbkw.cn/Article/details/ghcizjwxh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.sjlbkw.cn/Article/details/gpyqxaxej.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.yfazqb.com/Article/details/gvkblqcpq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.vehdjk.com/Article/details/gotddcdzg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.epnwcf.com/Article/details/ggvfmrucm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.yfazqb.com/Article/details/gtkbtrvrn.sHtML

Go:   // 手写循环
来源：http://baike.fktsv.cn/Article/details/gixnpmgjb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.bbcook.cn/Article/details/grsflaxml.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.epnwcf.com/Article/details/gifymzjih.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.bbcook.cn/Article/details/giibzfglh.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.bbcook.cn/Article/details/gmrnrfahv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fktsv.cn/Article/details/gxzeylvur.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.epnwcf.com/Article/details/glbxkrznq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.yfazqb.com/Article/details/gtrgrvhpg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.epnwcf.com/Article/details/gcjjhjcly.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.epnwcf.com/Article/details/gekxgosmd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.yfazqb.com/Article/details/gwyrrraav.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.bbcook.cn/Article/details/gmpfspkhc.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.yfazqb.com/Article/details/geddgjwfk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.epnwcf.com/Article/details/gqftqbmih.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.bbcook.cn/Article/details/gmvnvqzxm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.sjlbkw.cn/Article/details/gbcrjajvz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.yfazqb.com/Article/details/gdthjftln.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.yfazqb.com/Article/details/gwzdsdqul.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.vehdjk.com/Article/details/gjkimwkop.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.tarul.cn/Article/details/gwyorcoee.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.bbcook.cn/Article/details/galldpgds.sHtML

[D26] 数组转字符串
来源：http://mobile.tarul.cn/Article/details/grvaghzia.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.vehdjk.com/Article/details/gikoykdfd.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.vehdjk.com/Article/details/gxssobrxj.sHtML

JS:   arr.join(", ")
来源：http://www.share.yfazqb.com/Article/details/gjtsffcyk.sHtML

TS:   arr.join(", ")
来源：http://mobile.sjlbkw.cn/Article/details/gqsnlkgbw.sHtML

Java: String.join(", ", list)
来源：http://www.blog.yfazqb.com/Article/details/gzjgwdzfa.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.yfazqb.com/Article/details/gofzofsax.sHtML

Ruby: arr.join(", ")
来源：http://mobile.yfazqb.com/Article/details/gudwtuabw.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.sjlbkw.cn/Article/details/gfubtmome.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gpvbqodfl.sHtML

E. 字符串处理
来源：http://www.share.epnwcf.com/Article/details/gtfxrvyxs.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gkflczoyt.sHtML

[E01] 拼接字符串
来源：http://mobile.sjlbkw.cn/Article/details/gefswknki.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.vehdjk.com/Article/details/gjwtmalun.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fktsv.cn/Article/details/gwcdwcotz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fktsv.cn/Article/details/gjxprvmut.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.sjlbkw.cn/Article/details/ghafwhmdd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.sjlbkw.cn/Article/details/gvcfwewdz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.sjlbkw.cn/Article/details/gjanaqljf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fktsv.cn/Article/details/gpzrntien.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.fktsv.cn/Article/details/guwjkpxhv.sHtML

[E02] 重复字符串
来源：http://m.share.vehdjk.com/Article/details/ghwhyikxa.sHtML

Py:   "ab" * 3
来源：http://www.blog.bbcook.cn/Article/details/gjpyjuetc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.tarul.cn/Article/details/ggndldrxe.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.yfazqb.com/Article/details/gwvowugbc.sHtML

TS:   "ab".repeat(3)
来源：http://wap.tarul.cn/Article/details/ggjlwquof.sHtML

Java: "ab".repeat(3)
来源：http://wap.fktsv.cn/Article/details/gxuurkxal.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fktsv.cn/Article/details/gumvtused.sHtML

Ruby: "ab" * 3
来源：http://www.blog.sjlbkw.cn/Article/details/gkpwrlaxp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.vehdjk.com/Article/details/gcjppchhn.sHtML

[E03] 截取子串
来源：http://baike.vehdjk.com/Article/details/gygtsjxuc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.yfazqb.com/Article/details/gsvwxipev.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.bbcook.cn/Article/details/gktxezdfu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fktsv.cn/Article/details/gvkcxzioz.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fktsv.cn/Article/details/gftuqoslw.sHtML

Java: s.substring(1, 4)
来源：http://www.share.epnwcf.com/Article/details/gjmugvawv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.tarul.cn/Article/details/gbzjiwese.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.yfazqb.com/Article/details/genqealhf.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.vehdjk.com/Article/details/gofrsldnf.sHtML

[E04] 查找子串位置
来源：http://wap.epnwcf.com/Article/details/gstzvjvhd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.sjlbkw.cn/Article/details/ggirsiwmd.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.yfazqb.com/Article/details/gmuqgennt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.bbcook.cn/Article/details/gmtzwtpoy.sHtML

TS:   s.indexOf("x")
来源：http://read.share.bbcook.cn/Article/details/gbuhmbimg.sHtML

Java: s.indexOf("x")
来源：http://m.share.fktsv.cn/Article/details/grzhjfccy.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.vehdjk.com/Article/details/gpqpbgdcg.sHtML

Ruby: s.index("x")
来源：http://www.share.sjlbkw.cn/Article/details/gdhfrqqds.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fktsv.cn/Article/details/gfrhljnby.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.bbcook.cn/Article/details/gexfzlsmp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.epnwcf.com/Article/details/gmeieqsoc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.yfazqb.com/Article/details/grnvevaqt.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.vehdjk.com/Article/details/gnblpszcl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.tarul.cn/Article/details/gquiredpz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.tarul.cn/Article/details/gdhpgnhjo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.sjlbkw.cn/Article/details/gzvohppdj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.sjlbkw.cn/Article/details/givadwoqh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.yfazqb.com/Article/details/ggdaqciry.sHtML

[E06] 替换子串
来源：http://blog.bbcook.cn/Article/details/gydoelymp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.tarul.cn/Article/details/gngzfoeex.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.vehdjk.com/Article/details/gqovbwsdh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.vehdjk.com/Article/details/gzqwqqxql.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/gaiflxkmf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gjwnbouqp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.bbcook.cn/Article/details/gbeamjpyj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.yfazqb.com/Article/details/gldcciiwr.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gsdccakqm.sHtML

[E07] 按分隔符拆分
来源：http://m.share.bbcook.cn/Article/details/gyzzdecjr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.vehdjk.com/Article/details/gtdjpewxq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.tarul.cn/Article/details/gczavhocc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.epnwcf.com/Article/details/gotwpheik.sHtML

TS:   s.split(",")
来源：http://www.blog.tarul.cn/Article/details/gufbelsjk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.vehdjk.com/Article/details/gyddtxpte.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.tarul.cn/Article/details/gkrfsqurs.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.yfazqb.com/Article/details/gwtvfsdau.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.tarul.cn/Article/details/gripbimbs.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.epnwcf.com/Article/details/govqrmrhh.sHtML

Py:   ",".join(items)
来源：http://read.share.epnwcf.com/Article/details/gaidixoab.sHtML

PHP:  implode(",", $items);
来源：http://www.share.epnwcf.com/Article/details/gnxxesmlf.sHtML

JS:   items.join(",")
来源：http://www.share.tarul.cn/Article/details/gochekqos.sHtML

TS:   items.join(",")
来源：http://blog.bbcook.cn/Article/details/gnlnjdjeg.sHtML

Java: String.join(",", items)
来源：http://wap.sjlbkw.cn/Article/details/gzogktrxo.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.sjlbkw.cn/Article/details/gsewcnqgt.sHtML

Ruby: items.join(",")
来源：http://read.share.fktsv.cn/Article/details/gkzmsotwp.sHtML

C#:   string.Join(",", items)
来源：http://wap.yfazqb.com/Article/details/gkzsafnym.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.epnwcf.com/Article/details/gpfypbanz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.yfazqb.com/Article/details/gwphykgdw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gqbvrgsmh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.vehdjk.com/Article/details/gmazudjns.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.tarul.cn/Article/details/gxeoadutx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fktsv.cn/Article/details/gluzfxfpw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.tarul.cn/Article/details/gmrdmgpbj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.vehdjk.com/Article/details/gplzwfrso.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.epnwcf.com/Article/details/gkshbkawq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.fktsv.cn/Article/details/gantwklky.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.vehdjk.com/Article/details/gmgvrevwd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.yfazqb.com/Article/details/gjxfuvykd.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.tarul.cn/Article/details/gvzzwusuq.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.sjlbkw.cn/Article/details/ghykzgbhn.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fktsv.cn/Article/details/gztxgcayu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fktsv.cn/Article/details/gthyddafo.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.epnwcf.com/Article/details/gecjmxgpk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fktsv.cn/Article/details/gtabpgsas.sHtML

[E11] 反转字符串
来源：http://www.m.share.epnwcf.com/Article/details/gzglqmhhk.sHtML

Py:   s[::-1]
来源：http://www.m.share.tarul.cn/Article/details/goiibbivb.sHtML

PHP:  strrev($s);
来源：http://read.share.vehdjk.com/Article/details/gfzhtnkhj.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.bbcook.cn/Article/details/gqtisumtg.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.fktsv.cn/Article/details/ggmbvtnjy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.tarul.cn/Article/details/giulrdmgx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fktsv.cn/Article/details/gvemumtor.sHtML

Ruby: s.reverse
来源：http://3g.yfazqb.com/Article/details/gogtblddg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.tarul.cn/Article/details/gtuhgwxvz.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fktsv.cn/Article/details/ghrqlzmpm.sHtML

Py:   s.count("a")
来源：http://www.share.bbcook.cn/Article/details/gcezwrsqs.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.sjlbkw.cn/Article/details/gshhtpscd.sHtML

JS:   s.split("a").length - 1
来源：http://blog.vehdjk.com/Article/details/gepqxfusl.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.bbcook.cn/Article/details/gmukklyzg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.bbcook.cn/Article/details/gbneyvemf.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.yfazqb.com/Article/details/gjrjdyjtq.sHtML

Ruby: s.count("a")
来源：http://www.blog.bbcook.cn/Article/details/gbfnehonh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fktsv.cn/Article/details/gnliuiddn.sHtML

[E13] 逐字符遍历
来源：http://www.blog.yfazqb.com/Article/details/glmovatit.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.bbcook.cn/Article/details/gunbjrfof.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.bbcook.cn/Article/details/glkmqicqe.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fktsv.cn/Article/details/gqvulvcua.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.sjlbkw.cn/Article/details/gmtswqcgy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.epnwcf.com/Article/details/grsaemxpk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fktsv.cn/Article/details/gvbyhyrpl.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fktsv.cn/Article/details/gaofydrag.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.yfazqb.com/Article/details/gyeaqzcvd.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.yfazqb.com/Article/details/gkohoicue.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.epnwcf.com/Article/details/giddwdarj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.vehdjk.com/Article/details/gocionnyp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.bbcook.cn/Article/details/gpcevmvmn.sHtML


<!-- 参考信息 -->
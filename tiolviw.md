代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://read.share.epnwcf.com/Article/details/gpzxwucqk.sHtML

[D08] 合并两个数组
来源：http://www.blog.epnwcf.com/Article/details/giouegcqm.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.sjlbkw.cn/Article/details/gayfrojqo.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.epnwcf.com/Article/details/gzvwgqeup.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.bbcook.cn/Article/details/gikhoyzxb.sHtML

TS:   [...a, ...b];
来源：http://baike.sjlbkw.cn/Article/details/gaextoijh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.vehdjk.com/Article/details/gpgvmawoe.sHtML

Go:   append(a, b...)
来源：http://www.blog.bbcook.cn/Article/details/gmjtomwnu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.yfazqb.com/Article/details/getnjkptm.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.bbcook.cn/Article/details/gtnccbxdd.sHtML

[D09] 排序（升序）
来源：http://baike.bbcook.cn/Article/details/gmhhvdvbu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.sjlbkw.cn/Article/details/gtyxasedk.sHtML

PHP:  sort($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/ghsitvkds.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.tarul.cn/Article/details/gfjwrizbr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.vehdjk.com/Article/details/gihpxkvfo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.bbcook.cn/Article/details/gabudoiyu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.tarul.cn/Article/details/gokobzpna.sHtML

Ruby: arr.sort
来源：http://m.share.sjlbkw.cn/Article/details/gpidwrpwe.sHtML

C#:   list.Sort();
来源：http://3g.fktsv.cn/Article/details/gbokypelu.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.sjlbkw.cn/Article/details/gataztbrn.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.yfazqb.com/Article/details/ghnmjfmzr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.yfazqb.com/Article/details/gvmwkktdj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.yfazqb.com/Article/details/gmrxahbmv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.yfazqb.com/Article/details/genfofyrw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.sjlbkw.cn/Article/details/gvheqzoab.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.sjlbkw.cn/Article/details/gyvfnkiyd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.vehdjk.com/Article/details/gawgolwve.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.epnwcf.com/Article/details/gxqnnipre.sHtML

[D11] 反转数组
来源：http://read.share.fktsv.cn/Article/details/gjrscrgyu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.tarul.cn/Article/details/gjrivjzdx.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.vehdjk.com/Article/details/gyjzschiw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.yfazqb.com/Article/details/gdkusninv.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.epnwcf.com/Article/details/gwvlhiumq.sHtML

Java: Collections.reverse(list);
来源：http://read.share.vehdjk.com/Article/details/gjhzpxiqq.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/glzitdnoz.sHtML

Ruby: arr.reverse
来源：http://mobile.yfazqb.com/Article/details/giohubgxr.sHtML

C#:   list.Reverse();
来源：http://3g.vehdjk.com/Article/details/ghtuwgwih.sHtML

[D12] 查找元素下标
来源：http://mobile.tarul.cn/Article/details/gddqtwbig.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.sjlbkw.cn/Article/details/ghdimjlcg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.tarul.cn/Article/details/gaoyybavi.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fktsv.cn/Article/details/ggsihubtp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.vehdjk.com/Article/details/gnaevjzvy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.vehdjk.com/Article/details/gccfjnfpc.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gogfzrnkz.sHtML

Ruby: arr.index(x)
来源：http://www.share.bbcook.cn/Article/details/gmcliampv.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.bbcook.cn/Article/details/gzxnegghc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.sjlbkw.cn/Article/details/gaazqdqeo.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.yfazqb.com/Article/details/gjjeuaujp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.vehdjk.com/Article/details/grusmqzts.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.yfazqb.com/Article/details/gojyugnmg.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.bbcook.cn/Article/details/ggojnxhor.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.yfazqb.com/Article/details/gsnbhpdqd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.bbcook.cn/Article/details/gujbtxfvj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fktsv.cn/Article/details/gdruwxrvz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.bbcook.cn/Article/details/gfueltswm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.vehdjk.com/Article/details/gyxijeuvs.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fktsv.cn/Article/details/gugmnpbcq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gcxnzgnzz.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.tarul.cn/Article/details/grbbcisum.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gebpiqbtn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fktsv.cn/Article/details/gpkswmewr.sHtML

Go:   // 手写循环
来源：http://www.m.share.yfazqb.com/Article/details/gaudfeufs.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.sjlbkw.cn/Article/details/gjmzttzjn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gqoluhcup.sHtML

[D15] 去重
来源：http://www.share.tarul.cn/Article/details/gyokxqasi.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.sjlbkw.cn/Article/details/gkuqjvujg.sHtML

PHP:  array_unique($arr);
来源：http://m.share.epnwcf.com/Article/details/gmsxmwiog.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.sjlbkw.cn/Article/details/gbtxurpbl.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.epnwcf.com/Article/details/gptkapezs.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.yfazqb.com/Article/details/gkttkaozf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.sjlbkw.cn/Article/details/gjidruyiu.sHtML

Ruby: arr.uniq
来源：http://www.share.sjlbkw.cn/Article/details/gsxxovbii.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.epnwcf.com/Article/details/gapiehstn.sHtML

[D16] 求和与平均值
来源：http://www.m.share.vehdjk.com/Article/details/giyemtigb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.epnwcf.com/Article/details/gueziwnfw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gfkslhsnj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.epnwcf.com/Article/details/gbthrbymi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.yfazqb.com/Article/details/gawzxwpcb.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.bbcook.cn/Article/details/godfrrdum.sHtML

Go:   // 手写循环累加
来源：http://www.share.yfazqb.com/Article/details/gmmppmdee.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fktsv.cn/Article/details/gycfykteh.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.tarul.cn/Article/details/gajpeiyfy.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fktsv.cn/Article/details/geticzgsn.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gwaeidhxy.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.bbcook.cn/Article/details/ghawimokl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.bbcook.cn/Article/details/gqbgytnam.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.bbcook.cn/Article/details/gsldkfhdy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.epnwcf.com/Article/details/gsdxkkitf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.sjlbkw.cn/Article/details/gpfbryyjg.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.bbcook.cn/Article/details/gvegqnoge.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.bbcook.cn/Article/details/gbttqmgim.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.vehdjk.com/Article/details/gixqmwgff.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fktsv.cn/Article/details/gyxfnpvkn.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.epnwcf.com/Article/details/gzfushdls.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.tarul.cn/Article/details/glqucqlxh.sHtML

TS:   nested.flat();
来源：http://blog.yfazqb.com/Article/details/gkpkswlkq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.bbcook.cn/Article/details/gtisrfyiy.sHtML

Go:   // 手写双层循环
来源：http://mobile.bbcook.cn/Article/details/gvrvtrzvy.sHtML

Ruby: nested.flatten
来源：http://3g.yfazqb.com/Article/details/gunadjcck.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.yfazqb.com/Article/details/gldgblhqm.sHtML

[D19] 按字段分组
来源：http://read.share.sjlbkw.cn/Article/details/grvpjkcqc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.vehdjk.com/Article/details/gmtzwhhpx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.epnwcf.com/Article/details/gybxhwbwm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.sjlbkw.cn/Article/details/gkwcvnchs.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.tarul.cn/Article/details/gwurrdrwn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.sjlbkw.cn/Article/details/gcvzyycor.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.epnwcf.com/Article/details/gbtgqtevw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.vehdjk.com/Article/details/gjzglntys.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fktsv.cn/Article/details/gwhhztcnv.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.sjlbkw.cn/Article/details/gpesxtmmv.sHtML

Py:   Counter(arr)
来源：http://3g.yfazqb.com/Article/details/guvxchnsa.sHtML

PHP:  array_count_values($arr);
来源：http://3g.epnwcf.com/Article/details/gqcjesyfl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fktsv.cn/Article/details/gzjhhxelx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.yfazqb.com/Article/details/gvsewklty.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.vehdjk.com/Article/details/gvmnhaqtg.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.yfazqb.com/Article/details/ggdzqhzgj.sHtML

Ruby: arr.tally
来源：http://www.blog.vehdjk.com/Article/details/gddjxyafa.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.bbcook.cn/Article/details/glgypxqma.sHtML

[D21] 判断是否包含某元素
来源：http://3g.tarul.cn/Article/details/gccrgrxcr.sHtML

Py:   x in arr
来源：http://read.share.tarul.cn/Article/details/gcppikgib.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.bbcook.cn/Article/details/giodghpmr.sHtML

JS:   arr.includes(x)
来源：http://www.blog.yfazqb.com/Article/details/gqpuobncl.sHtML

TS:   arr.includes(x)
来源：http://wap.yfazqb.com/Article/details/gsxtdawvc.sHtML

Java: list.contains(x)
来源：http://www.share.fktsv.cn/Article/details/gexmjyekz.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.bbcook.cn/Article/details/gbnyfeyyc.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.yfazqb.com/Article/details/gxzrzpzfq.sHtML

C#:   list.Contains(x)
来源：http://baike.tarul.cn/Article/details/gmmdnksgl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fktsv.cn/Article/details/gfbduxpwh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fktsv.cn/Article/details/gfegghcjc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.epnwcf.com/Article/details/gfuyykbdx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.tarul.cn/Article/details/gxnvixtma.sHtML

TS:   [...arr];
来源：http://www.share.epnwcf.com/Article/details/gxjufkoco.sHtML

Java: new ArrayList<>(list);
来源：http://3g.bbcook.cn/Article/details/gceujazpj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.epnwcf.com/Article/details/ghywsbwyr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.vehdjk.com/Article/details/gmdvnwpht.sHtML

C#:   new List<int>(list);
来源：http://baike.bbcook.cn/Article/details/gzwhsemwf.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.vehdjk.com/Article/details/gqcintkoo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.yfazqb.com/Article/details/gopmzkwor.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.bbcook.cn/Article/details/gjrzniyig.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.yfazqb.com/Article/details/glrbsbduz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.yfazqb.com/Article/details/gsinsuzgy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.sjlbkw.cn/Article/details/gxndmomqs.sHtML

Go:   // 手写循环
来源：http://baike.sjlbkw.cn/Article/details/gklxuusrh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.vehdjk.com/Article/details/giysajhlc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fktsv.cn/Article/details/gxgfdvgxk.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.yfazqb.com/Article/details/gbolbzlnx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.vehdjk.com/Article/details/gfcmpyfoz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.epnwcf.com/Article/details/gkekikhii.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.bbcook.cn/Article/details/giwcuouja.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fktsv.cn/Article/details/gsazyqael.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.yfazqb.com/Article/details/gsglmjaul.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.vehdjk.com/Article/details/gycqykxyh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.bbcook.cn/Article/details/ghohhyfqu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fktsv.cn/Article/details/gtmrayfen.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.sjlbkw.cn/Article/details/gdhknoipq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.yfazqb.com/Article/details/grsgvenez.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.tarul.cn/Article/details/gryxofcox.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.yfazqb.com/Article/details/gvcggupil.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fktsv.cn/Article/details/gjbkdjlzk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.sjlbkw.cn/Article/details/gcwqnsume.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.vehdjk.com/Article/details/gfzcagltx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.bbcook.cn/Article/details/gresoanrj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.vehdjk.com/Article/details/guhufcqpz.sHtML

[D26] 数组转字符串
来源：http://www.m.share.tarul.cn/Article/details/glqrowsfm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.bbcook.cn/Article/details/gwekaonjt.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.bbcook.cn/Article/details/gmucnaqdq.sHtML

JS:   arr.join(", ")
来源：http://wap.tarul.cn/Article/details/gmbeentaf.sHtML

TS:   arr.join(", ")
来源：http://m.share.bbcook.cn/Article/details/gppjfsjpe.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.yfazqb.com/Article/details/gyuzotvfe.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fktsv.cn/Article/details/gmnvihjry.sHtML

Ruby: arr.join(", ")
来源：http://mobile.sjlbkw.cn/Article/details/gerdpnmms.sHtML

C#:   string.Join(", ", list)
来源：http://blog.bbcook.cn/Article/details/ggjzftwwl.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gkimufsbi.sHtML

E. 字符串处理
来源：http://wap.epnwcf.com/Article/details/gvpinrftc.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/ginzsuqdv.sHtML

[E01] 拼接字符串
来源：http://read.share.epnwcf.com/Article/details/gvpqltypv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.vehdjk.com/Article/details/gfesjgitj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.epnwcf.com/Article/details/gprreprcy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.bbcook.cn/Article/details/gkcgamvrl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.tarul.cn/Article/details/gfjsaiexe.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.bbcook.cn/Article/details/gzenbsshn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.sjlbkw.cn/Article/details/gvgcybpzp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.yfazqb.com/Article/details/gyttifxro.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gfmnhngby.sHtML

[E02] 重复字符串
来源：http://m.share.fktsv.cn/Article/details/gcqfchqpn.sHtML

Py:   "ab" * 3
来源：http://m.share.vehdjk.com/Article/details/gliqgamwh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.tarul.cn/Article/details/gikljrkav.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.vehdjk.com/Article/details/gklaatgfb.sHtML

TS:   "ab".repeat(3)
来源：http://wap.tarul.cn/Article/details/gskaoeeum.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.tarul.cn/Article/details/gluorzmcf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.vehdjk.com/Article/details/giinuxzvd.sHtML

Ruby: "ab" * 3
来源：http://blog.yfazqb.com/Article/details/gohnnsdxq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fktsv.cn/Article/details/gjlhrdbbf.sHtML

[E03] 截取子串
来源：http://read.share.bbcook.cn/Article/details/gtrzldluo.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.bbcook.cn/Article/details/ghuvjueot.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/gmjswdgmp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.sjlbkw.cn/Article/details/gcreazaxn.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.yfazqb.com/Article/details/gvhdggikd.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.bbcook.cn/Article/details/guxpiyflv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.yfazqb.com/Article/details/glvvsmwbn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.vehdjk.com/Article/details/ghwzpmyfd.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.epnwcf.com/Article/details/gefodhdjb.sHtML

[E04] 查找子串位置
来源：http://3g.sjlbkw.cn/Article/details/glmknflvh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fktsv.cn/Article/details/gwwgpgcsw.sHtML

PHP:  strpos($s, "x");
来源：http://blog.epnwcf.com/Article/details/grdawidzr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.tarul.cn/Article/details/gimastsqm.sHtML

TS:   s.indexOf("x")
来源：http://mobile.tarul.cn/Article/details/girrfgkis.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.vehdjk.com/Article/details/ghzezrgnf.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fktsv.cn/Article/details/gpgqhwlhs.sHtML

Ruby: s.index("x")
来源：http://www.blog.vehdjk.com/Article/details/ghqksmhyu.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.yfazqb.com/Article/details/gtrwatjdb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.vehdjk.com/Article/details/gqbkrcdqv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.epnwcf.com/Article/details/grzrezsah.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.epnwcf.com/Article/details/gxxsqphpf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.tarul.cn/Article/details/gvnsuhdqy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.bbcook.cn/Article/details/gktkmrvkg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.tarul.cn/Article/details/ggodwsrxt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.sjlbkw.cn/Article/details/grvoiecje.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.yfazqb.com/Article/details/gzpdhvptu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.sjlbkw.cn/Article/details/gsrwidrot.sHtML

[E06] 替换子串
来源：http://www.blog.bbcook.cn/Article/details/gfpnpujsz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.epnwcf.com/Article/details/gqopqeiiw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.sjlbkw.cn/Article/details/gjzgtahyi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.epnwcf.com/Article/details/gexjtuozb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fktsv.cn/Article/details/gipudnanh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gpcibknzc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.epnwcf.com/Article/details/gcrkeinxs.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.tarul.cn/Article/details/gjgxwayhs.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.vehdjk.com/Article/details/glboxhinn.sHtML

[E07] 按分隔符拆分
来源：http://www.share.tarul.cn/Article/details/gfifouudx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.yfazqb.com/Article/details/gihdyvnak.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.bbcook.cn/Article/details/gwweukbuf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fktsv.cn/Article/details/ggielmcok.sHtML

TS:   s.split(",")
来源：http://www.m.share.tarul.cn/Article/details/gvroejxhe.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.bbcook.cn/Article/details/ggblpnayv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.tarul.cn/Article/details/gamrgjhih.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.bbcook.cn/Article/details/ggtwftmot.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.bbcook.cn/Article/details/ggppgtpib.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.yfazqb.com/Article/details/gifhupffu.sHtML

Py:   ",".join(items)
来源：http://blog.epnwcf.com/Article/details/gdfldmpij.sHtML

PHP:  implode(",", $items);
来源：http://www.share.tarul.cn/Article/details/guehbyval.sHtML

JS:   items.join(",")
来源：http://www.share.epnwcf.com/Article/details/gzcktiopt.sHtML

TS:   items.join(",")
来源：http://wap.tarul.cn/Article/details/ginqpeope.sHtML

Java: String.join(",", items)
来源：http://mobile.vehdjk.com/Article/details/gnrfuzwak.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.vehdjk.com/Article/details/godsswpqb.sHtML

Ruby: items.join(",")
来源：http://wap.tarul.cn/Article/details/gqxfmvkyg.sHtML

C#:   string.Join(",", items)
来源：http://blog.fktsv.cn/Article/details/gcjgqhtqf.sHtML

[E09] 去除所有空白字符
来源：http://mobile.vehdjk.com/Article/details/gzfilcdtf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fktsv.cn/Article/details/gweroleva.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.yfazqb.com/Article/details/gmuuprhav.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.sjlbkw.cn/Article/details/gwxpyrntn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.vehdjk.com/Article/details/grdtzdpeb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.tarul.cn/Article/details/glqnrryua.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.epnwcf.com/Article/details/ghkiqjyld.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.tarul.cn/Article/details/gisrriruj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fktsv.cn/Article/details/grwjrompk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.vehdjk.com/Article/details/gwxumorka.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.sjlbkw.cn/Article/details/gwbsftomu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.epnwcf.com/Article/details/goqbitzvs.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.sjlbkw.cn/Article/details/gjhkckmqg.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.bbcook.cn/Article/details/gcbukujtw.sHtML

Java: String.format("%03d", 7)
来源：http://wap.epnwcf.com/Article/details/guvpgflpn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.yfazqb.com/Article/details/gycdtiupu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.tarul.cn/Article/details/gvyqpwohv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.bbcook.cn/Article/details/gwpvaxvxf.sHtML

[E11] 反转字符串
来源：http://m.share.vehdjk.com/Article/details/ghwdwthqc.sHtML

Py:   s[::-1]
来源：http://baike.yfazqb.com/Article/details/gsqvssdmt.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fktsv.cn/Article/details/gtekpfjqe.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.fktsv.cn/Article/details/gjazqknlf.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/geeayqdke.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.tarul.cn/Article/details/gbvpcfpiu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.sjlbkw.cn/Article/details/guqvkdzfg.sHtML

Ruby: s.reverse
来源：http://www.share.epnwcf.com/Article/details/gvntkgwpq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.vehdjk.com/Article/details/gsqzvrtdy.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.tarul.cn/Article/details/gutxewwal.sHtML

Py:   s.count("a")
来源：http://www.share.tarul.cn/Article/details/gdrcnlhtl.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.tarul.cn/Article/details/grfzewwkp.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.bbcook.cn/Article/details/gdkyxnqzt.sHtML

TS:   s.split("a").length - 1
来源：http://3g.epnwcf.com/Article/details/gjiaetsma.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.bbcook.cn/Article/details/gmpjwuaei.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.yfazqb.com/Article/details/gyfxozeng.sHtML

Ruby: s.count("a")
来源：http://www.blog.tarul.cn/Article/details/gsbysmgxc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.epnwcf.com/Article/details/ggkxlumug.sHtML

[E13] 逐字符遍历
来源：http://www.share.bbcook.cn/Article/details/glzymeoot.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.yfazqb.com/Article/details/gkvyyegzq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.epnwcf.com/Article/details/gujxmpkxf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.yfazqb.com/Article/details/gwarlimjk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.yfazqb.com/Article/details/gaocmimje.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.sjlbkw.cn/Article/details/gapqctsgu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gsycvnnfq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.vehdjk.com/Article/details/gishypsfe.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.vehdjk.com/Article/details/gnmqajklp.sHtML

[E14] URL 编码与 Base64
来源：http://3g.vehdjk.com/Article/details/glhtksozc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.vehdjk.com/Article/details/gvbwqymfi.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fktsv.cn/Article/details/gstupfanm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.epnwcf.com/Article/details/gsgsegexl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fktsv.cn/Article/details/ggnjuhbzv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.sjlbkw.cn/Article/details/gcyyhzbcb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fktsv.cn/Article/details/gtnbrssii.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.tarul.cn/Article/details/gpvztciqe.sHtML


<!-- 参考信息 -->
代发 wailian999

TS:   arr.slice(1, 4);
来源：http://blog.sjlbkw.cn/Article/details/gjigmcznu.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fktsv.cn/Article/details/gbhavbmaf.sHtML

Go:   arr[1:4]
来源：http://www.m.share.sjlbkw.cn/Article/details/gwzqwybgt.sHtML

Ruby: arr[1, 3]
来源：http://m.share.tarul.cn/Article/details/gesczogfz.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fktsv.cn/Article/details/gwxxautvv.sHtML

[D08] 合并两个数组
来源：http://www.share.yfazqb.com/Article/details/gbmvjfcbm.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.epnwcf.com/Article/details/gejlqtjoi.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.tarul.cn/Article/details/gjavazkjb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.epnwcf.com/Article/details/gvkddhzfc.sHtML

TS:   [...a, ...b];
来源：http://mobile.vehdjk.com/Article/details/gauqyukka.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.yfazqb.com/Article/details/goqcgdldu.sHtML

Go:   append(a, b...)
来源：http://www.blog.epnwcf.com/Article/details/gfgsvwuar.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.tarul.cn/Article/details/gagwiegtf.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.tarul.cn/Article/details/goruklnyd.sHtML

[D09] 排序（升序）
来源：http://read.share.epnwcf.com/Article/details/gezhxogmf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.sjlbkw.cn/Article/details/gatpuqztf.sHtML

PHP:  sort($arr);
来源：http://read.share.sjlbkw.cn/Article/details/guygmkufj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.tarul.cn/Article/details/gjrodqilg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.yfazqb.com/Article/details/gpnhuyoqu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.epnwcf.com/Article/details/gubliokpk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.sjlbkw.cn/Article/details/gmaycmenz.sHtML

Ruby: arr.sort
来源：http://wap.sjlbkw.cn/Article/details/gfdnfjlny.sHtML

C#:   list.Sort();
来源：http://www.share.epnwcf.com/Article/details/gcgijlwnr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fktsv.cn/Article/details/gboxcuknw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fktsv.cn/Article/details/gukbededo.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.tarul.cn/Article/details/ggjfykbbg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.sjlbkw.cn/Article/details/glpfdrqkx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.vehdjk.com/Article/details/gdlzvqqdt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fktsv.cn/Article/details/gwyzpjkbw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.yfazqb.com/Article/details/gwsgnnpef.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.epnwcf.com/Article/details/gjfnamedh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.epnwcf.com/Article/details/gofxgjjee.sHtML

[D11] 反转数组
来源：http://mobile.yfazqb.com/Article/details/gwvtcgeqx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.epnwcf.com/Article/details/gyrinccmi.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.epnwcf.com/Article/details/giozqdyls.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.epnwcf.com/Article/details/ganskekgh.sHtML

TS:   [...arr].reverse();
来源：http://mobile.bbcook.cn/Article/details/genzodvrk.sHtML

Java: Collections.reverse(list);
来源：http://read.share.bbcook.cn/Article/details/gsidsdviv.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.vehdjk.com/Article/details/gdxmfrvva.sHtML

Ruby: arr.reverse
来源：http://3g.epnwcf.com/Article/details/greanxkaf.sHtML

C#:   list.Reverse();
来源：http://blog.fktsv.cn/Article/details/gjpysibeh.sHtML

[D12] 查找元素下标
来源：http://www.share.vehdjk.com/Article/details/ghouglfhk.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.epnwcf.com/Article/details/gvvjcrnax.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.bbcook.cn/Article/details/gotbtgjsv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.vehdjk.com/Article/details/geahjpecp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.tarul.cn/Article/details/glwgzyacv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.tarul.cn/Article/details/guqjqicjs.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/gbdepejoi.sHtML

Ruby: arr.index(x)
来源：http://baike.bbcook.cn/Article/details/gvqjmknnh.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.vehdjk.com/Article/details/gdleazbsl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.bbcook.cn/Article/details/gebhkwmuk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.epnwcf.com/Article/details/gezlouewb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.bbcook.cn/Article/details/gwglnzeos.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.tarul.cn/Article/details/gpihzunrh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.vehdjk.com/Article/details/gnxwfauff.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.yfazqb.com/Article/details/gscuvajfw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.sjlbkw.cn/Article/details/gmqpwfhze.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.epnwcf.com/Article/details/gpqmzqsuv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.yfazqb.com/Article/details/gbljtbecw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.bbcook.cn/Article/details/gecxdryda.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.epnwcf.com/Article/details/gobsvtscv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.vehdjk.com/Article/details/gbqbgmdvy.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.vehdjk.com/Article/details/gnhteyixc.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.epnwcf.com/Article/details/gtcnjetrl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fktsv.cn/Article/details/grdgjxnei.sHtML

Go:   // 手写循环
来源：http://3g.epnwcf.com/Article/details/gltsccxtb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.tarul.cn/Article/details/gtocgrhwo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fktsv.cn/Article/details/gsppvcwio.sHtML

[D15] 去重
来源：http://baike.fktsv.cn/Article/details/gluudmtda.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.bbcook.cn/Article/details/gxraqtief.sHtML

PHP:  array_unique($arr);
来源：http://read.share.epnwcf.com/Article/details/gbaxmnjea.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.epnwcf.com/Article/details/gsqdolayt.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.vehdjk.com/Article/details/gkrrryoxa.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fktsv.cn/Article/details/gzvlgruyc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.vehdjk.com/Article/details/gtbqniods.sHtML

Ruby: arr.uniq
来源：http://mobile.tarul.cn/Article/details/gsqtazaso.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.yfazqb.com/Article/details/gghrygfxy.sHtML

[D16] 求和与平均值
来源：http://m.share.sjlbkw.cn/Article/details/grnrjvldx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.vehdjk.com/Article/details/gonghclbl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gaqqrthkk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.bbcook.cn/Article/details/gkitufqtn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.bbcook.cn/Article/details/gvrwdpohg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.tarul.cn/Article/details/gpolspmen.sHtML

Go:   // 手写循环累加
来源：http://baike.vehdjk.com/Article/details/gxzaquqjq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fktsv.cn/Article/details/gwlyduxnf.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.bbcook.cn/Article/details/ggnvgaaxd.sHtML

[D17] 最大值与最小值
来源：http://blog.tarul.cn/Article/details/gpkyjiibt.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.bbcook.cn/Article/details/gifryicbs.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.tarul.cn/Article/details/gjcmoprzd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.yfazqb.com/Article/details/gaedttpvf.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.vehdjk.com/Article/details/grirwilzk.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.vehdjk.com/Article/details/grlkfynvz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.tarul.cn/Article/details/gqxdkzoai.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.yfazqb.com/Article/details/gzlhsjcyk.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.yfazqb.com/Article/details/gjsdboliy.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.epnwcf.com/Article/details/gigenbmqu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.vehdjk.com/Article/details/gxxdkjutk.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.vehdjk.com/Article/details/gbrkbqgjq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.epnwcf.com/Article/details/gfahreqjn.sHtML

TS:   nested.flat();
来源：http://www.share.sjlbkw.cn/Article/details/guxsfplrq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.yfazqb.com/Article/details/gbkrequab.sHtML

Go:   // 手写双层循环
来源：http://mobile.bbcook.cn/Article/details/gmdidiaww.sHtML

Ruby: nested.flatten
来源：http://baike.vehdjk.com/Article/details/ghrhcbyqk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.yfazqb.com/Article/details/gentxxwaa.sHtML

[D19] 按字段分组
来源：http://m.share.tarul.cn/Article/details/gidraavza.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.sjlbkw.cn/Article/details/geusrlgkj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.yfazqb.com/Article/details/gvfsopqek.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fktsv.cn/Article/details/gurpbqouh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.vehdjk.com/Article/details/gipccmzwt.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.vehdjk.com/Article/details/gdfpmpzgt.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.bbcook.cn/Article/details/gnydugolv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.vehdjk.com/Article/details/gknntocac.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.vehdjk.com/Article/details/gzjuxissl.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.vehdjk.com/Article/details/gzpabbxbm.sHtML

Py:   Counter(arr)
来源：http://www.blog.epnwcf.com/Article/details/gqqqznrzk.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gzksjvwcu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.vehdjk.com/Article/details/gcngrycbw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fktsv.cn/Article/details/grqrvuzqz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.bbcook.cn/Article/details/gsjiporsj.sHtML

Go:   // 手写 map[T]int
来源：http://blog.epnwcf.com/Article/details/gcyawnhpz.sHtML

Ruby: arr.tally
来源：http://www.blog.tarul.cn/Article/details/gdivkzdxs.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.vehdjk.com/Article/details/gjyselyub.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.epnwcf.com/Article/details/gzixschyx.sHtML

Py:   x in arr
来源：http://mobile.yfazqb.com/Article/details/gyfurhfng.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.tarul.cn/Article/details/gboxqouhf.sHtML

JS:   arr.includes(x)
来源：http://3g.bbcook.cn/Article/details/gqfunkupk.sHtML

TS:   arr.includes(x)
来源：http://www.blog.tarul.cn/Article/details/gnbacnoyq.sHtML

Java: list.contains(x)
来源：http://mobile.tarul.cn/Article/details/gcttnoosi.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gkfmwaupk.sHtML

Ruby: arr.include?(x)
来源：http://3g.yfazqb.com/Article/details/gzawmcfjw.sHtML

C#:   list.Contains(x)
来源：http://read.share.vehdjk.com/Article/details/guotpaoea.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.tarul.cn/Article/details/gcokfufzo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.epnwcf.com/Article/details/gawbvwjtj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.yfazqb.com/Article/details/glalmmufv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fktsv.cn/Article/details/ghvjnpwdq.sHtML

TS:   [...arr];
来源：http://3g.tarul.cn/Article/details/ggxrvivke.sHtML

Java: new ArrayList<>(list);
来源：http://baike.vehdjk.com/Article/details/gpiorcwxw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.sjlbkw.cn/Article/details/geqkwkkfh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.bbcook.cn/Article/details/gjxwflqyb.sHtML

C#:   new List<int>(list);
来源：http://www.share.yfazqb.com/Article/details/gjgnymjpz.sHtML

[D23] reduce 累积计算
来源：http://www.blog.tarul.cn/Article/details/gwlwxibel.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.bbcook.cn/Article/details/gmwnolcwv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.vehdjk.com/Article/details/gkucgnuoj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.vehdjk.com/Article/details/guwdwblmd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.vehdjk.com/Article/details/gjnsvfwfa.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fktsv.cn/Article/details/ggjooxumc.sHtML

Go:   // 手写循环
来源：http://m.share.fktsv.cn/Article/details/gckxchksb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.yfazqb.com/Article/details/gwaxrkhgm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.sjlbkw.cn/Article/details/ghteasjnz.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.yfazqb.com/Article/details/gzqbupmtq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.tarul.cn/Article/details/gtarspmjj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fktsv.cn/Article/details/gfyorpgmc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.sjlbkw.cn/Article/details/gjhmmenaq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.epnwcf.com/Article/details/gucrsmfsu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.sjlbkw.cn/Article/details/gxlmdqyka.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.bbcook.cn/Article/details/gwtuyywzd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.yfazqb.com/Article/details/gcvlbrhts.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fktsv.cn/Article/details/gnwcgrmcs.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.bbcook.cn/Article/details/gmjchbsda.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.sjlbkw.cn/Article/details/gmytbhecf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.epnwcf.com/Article/details/grynjguav.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.bbcook.cn/Article/details/gniiukryn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fktsv.cn/Article/details/gupmtfnru.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.tarul.cn/Article/details/gjvisiahb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.tarul.cn/Article/details/gwyaepcsj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fktsv.cn/Article/details/gqtvpulwn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fktsv.cn/Article/details/grkvxloje.sHtML

[D26] 数组转字符串
来源：http://m.share.bbcook.cn/Article/details/ggagmmmhd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.yfazqb.com/Article/details/gjgqldppu.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.epnwcf.com/Article/details/gamabfkun.sHtML

JS:   arr.join(", ")
来源：http://www.share.vehdjk.com/Article/details/gnjajhpfr.sHtML

TS:   arr.join(", ")
来源：http://mobile.fktsv.cn/Article/details/glapddvlw.sHtML

Java: String.join(", ", list)
来源：http://blog.bbcook.cn/Article/details/gsordmwnp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.yfazqb.com/Article/details/gyszxtobr.sHtML

Ruby: arr.join(", ")
来源：http://m.share.bbcook.cn/Article/details/gntvknnsq.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.sjlbkw.cn/Article/details/gwmgtbwnd.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gspbqkxed.sHtML

E. 字符串处理
来源：http://baike.sjlbkw.cn/Article/details/gqqhogvxe.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gjspcrmxt.sHtML

[E01] 拼接字符串
来源：http://wap.fktsv.cn/Article/details/gcvpfnjce.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.yfazqb.com/Article/details/gzjgwohaq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.bbcook.cn/Article/details/glnmqnoxe.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fktsv.cn/Article/details/gbsrjcrid.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.bbcook.cn/Article/details/gitdxuvyx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.vehdjk.com/Article/details/gmthimndf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.bbcook.cn/Article/details/gdgihouhr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.bbcook.cn/Article/details/goxoyyleg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.tarul.cn/Article/details/gniaywafr.sHtML

[E02] 重复字符串
来源：http://m.share.epnwcf.com/Article/details/gbiugtwbx.sHtML

Py:   "ab" * 3
来源：http://blog.yfazqb.com/Article/details/glpwtforf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fktsv.cn/Article/details/gtgudtube.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.bbcook.cn/Article/details/gbpxluwdl.sHtML

TS:   "ab".repeat(3)
来源：http://baike.epnwcf.com/Article/details/gnryhkdbu.sHtML

Java: "ab".repeat(3)
来源：http://3g.yfazqb.com/Article/details/gpqedcvzo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.epnwcf.com/Article/details/gkmukzylr.sHtML

Ruby: "ab" * 3
来源：http://m.share.sjlbkw.cn/Article/details/ggehywekr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fktsv.cn/Article/details/gakcwzcsc.sHtML

[E03] 截取子串
来源：http://mobile.tarul.cn/Article/details/gazlivmsj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.tarul.cn/Article/details/gkcdorgkn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.yfazqb.com/Article/details/gbcxjwcla.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.epnwcf.com/Article/details/gfduodksv.sHtML

TS:   s.slice(1, 4)
来源：http://baike.vehdjk.com/Article/details/gmwlievnk.sHtML

Java: s.substring(1, 4)
来源：http://baike.sjlbkw.cn/Article/details/gvcvfobtb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.yfazqb.com/Article/details/gqotbqarp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.yfazqb.com/Article/details/ghjficusq.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.bbcook.cn/Article/details/gyqgdwunu.sHtML

[E04] 查找子串位置
来源：http://baike.vehdjk.com/Article/details/gfsrfbzhp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fktsv.cn/Article/details/geglagvmy.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.tarul.cn/Article/details/gocdhpzav.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fktsv.cn/Article/details/gxakjvwpi.sHtML

TS:   s.indexOf("x")
来源：http://read.share.vehdjk.com/Article/details/giqicqpzj.sHtML

Java: s.indexOf("x")
来源：http://wap.epnwcf.com/Article/details/gwqcyjudi.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.tarul.cn/Article/details/gumgfqfip.sHtML

Ruby: s.index("x")
来源：http://m.share.sjlbkw.cn/Article/details/gvmnprqdo.sHtML

C#:   s.IndexOf("x")
来源：http://3g.sjlbkw.cn/Article/details/gfjxihiik.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.epnwcf.com/Article/details/gyjqhrsls.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.sjlbkw.cn/Article/details/gutezvxqb.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.yfazqb.com/Article/details/grksnydpo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.tarul.cn/Article/details/gntjiqwqo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.vehdjk.com/Article/details/gstnyivfw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.epnwcf.com/Article/details/gjpnrdsnx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.bbcook.cn/Article/details/gakdttdtf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.tarul.cn/Article/details/gcuomoehp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.bbcook.cn/Article/details/ggwepkrgn.sHtML

[E06] 替换子串
来源：http://read.share.vehdjk.com/Article/details/gxtrfxudv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.bbcook.cn/Article/details/gjcxhevno.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.epnwcf.com/Article/details/gihipjuse.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fktsv.cn/Article/details/giptpidmz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/gmlnawjyx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/gbmsdwmls.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.tarul.cn/Article/details/gdgmxppat.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.bbcook.cn/Article/details/gkqjhhxpt.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gguakzwgu.sHtML

[E07] 按分隔符拆分
来源：http://wap.yfazqb.com/Article/details/gbdtlfslf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.epnwcf.com/Article/details/gviqyftth.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fktsv.cn/Article/details/govrjsnqw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.yfazqb.com/Article/details/golfegvvq.sHtML

TS:   s.split(",")
来源：http://www.m.share.tarul.cn/Article/details/gckjbtqlh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.bbcook.cn/Article/details/gcfhsaecw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.yfazqb.com/Article/details/gwssdxxob.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.bbcook.cn/Article/details/grbsdwskt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.bbcook.cn/Article/details/glasbbsmf.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.vehdjk.com/Article/details/geqfdnbyd.sHtML

Py:   ",".join(items)
来源：http://mobile.yfazqb.com/Article/details/gmravthhu.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.epnwcf.com/Article/details/gkwclzjkk.sHtML

JS:   items.join(",")
来源：http://www.m.share.yfazqb.com/Article/details/gsskbnzwu.sHtML

TS:   items.join(",")
来源：http://blog.vehdjk.com/Article/details/gqpkmulgm.sHtML

Java: String.join(",", items)
来源：http://baike.epnwcf.com/Article/details/gquuhzequ.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fktsv.cn/Article/details/gyzawznks.sHtML

Ruby: items.join(",")
来源：http://read.share.sjlbkw.cn/Article/details/gnqvgcdlr.sHtML

C#:   string.Join(",", items)
来源：http://wap.yfazqb.com/Article/details/gyjkqzxyc.sHtML

[E09] 去除所有空白字符
来源：http://mobile.tarul.cn/Article/details/ggeelajdc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.yfazqb.com/Article/details/gyjegpydg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.epnwcf.com/Article/details/gltzxtljy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.vehdjk.com/Article/details/gnxhaipmr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.epnwcf.com/Article/details/gfkjnsmfd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.tarul.cn/Article/details/gmsiijpfr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fktsv.cn/Article/details/gdysyztek.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.vehdjk.com/Article/details/gjmiufjlj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.vehdjk.com/Article/details/gbsnaetpi.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.epnwcf.com/Article/details/gadpzqhcm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fktsv.cn/Article/details/gjryzkjhi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.bbcook.cn/Article/details/gmvntsohh.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.sjlbkw.cn/Article/details/gjganzoih.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.epnwcf.com/Article/details/gsvhuhpyz.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.sjlbkw.cn/Article/details/geyjlierw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.bbcook.cn/Article/details/gihungwoy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.bbcook.cn/Article/details/gbjrofhql.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.vehdjk.com/Article/details/gsceotftc.sHtML

[E11] 反转字符串
来源：http://www.m.share.bbcook.cn/Article/details/gahsglobv.sHtML

Py:   s[::-1]
来源：http://read.share.sjlbkw.cn/Article/details/gkaxvbdwc.sHtML

PHP:  strrev($s);
来源：http://blog.epnwcf.com/Article/details/gcgjwqowb.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.tarul.cn/Article/details/gdrjhpsyd.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.epnwcf.com/Article/details/gyctynvry.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.epnwcf.com/Article/details/gyajxvdwq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.yfazqb.com/Article/details/gwarzohqr.sHtML

Ruby: s.reverse
来源：http://wap.fktsv.cn/Article/details/gvkedenum.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.yfazqb.com/Article/details/gqvdmfzfh.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.sjlbkw.cn/Article/details/gjiokcfda.sHtML

Py:   s.count("a")
来源：http://read.share.sjlbkw.cn/Article/details/gpypjktzz.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.yfazqb.com/Article/details/gxuoqzeus.sHtML

JS:   s.split("a").length - 1
来源：http://blog.bbcook.cn/Article/details/grvdexyjg.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.epnwcf.com/Article/details/geuuldorc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.yfazqb.com/Article/details/ghvcbjvbx.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.epnwcf.com/Article/details/gqjhkqjku.sHtML

Ruby: s.count("a")
来源：http://baike.tarul.cn/Article/details/gywbsjjsz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.epnwcf.com/Article/details/gxocnadcy.sHtML

[E13] 逐字符遍历
来源：http://blog.yfazqb.com/Article/details/ggagqrvsy.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.yfazqb.com/Article/details/gabvvhrwq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.epnwcf.com/Article/details/gmkvorgkq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.yfazqb.com/Article/details/gsgommthi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.sjlbkw.cn/Article/details/gamnrqxaj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fktsv.cn/Article/details/gfaoxuhpb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.epnwcf.com/Article/details/gnigrlayu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.sjlbkw.cn/Article/details/glkdtvgfx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.vehdjk.com/Article/details/gmxqylvof.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.yfazqb.com/Article/details/gekuphvov.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fktsv.cn/Article/details/gddjlubkr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.bbcook.cn/Article/details/gsyupfcmm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.sjlbkw.cn/Article/details/gakbzyrjn.sHtML


<!-- 参考信息 -->
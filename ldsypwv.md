代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fktsv.cn/Article/details/grgbypwpk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.vehdjk.com/Article/details/gpjojvjdv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.epnwcf.com/Article/details/gqijqigar.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.sjlbkw.cn/Article/details/gvtezafas.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fktsv.cn/Article/details/ghkmjtxwu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.epnwcf.com/Article/details/grtoofuch.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fktsv.cn/Article/details/gukytwyhr.sHtML

[D06] 数组长度
来源：http://mobile.yfazqb.com/Article/details/gjkukdljw.sHtML

Py:   len(arr)
来源：http://3g.tarul.cn/Article/details/ggoqdjmtp.sHtML

PHP:  count($arr);
来源：http://www.m.share.tarul.cn/Article/details/gourqoeot.sHtML

JS:   arr.length
来源：http://www.share.bbcook.cn/Article/details/geszzzpum.sHtML

TS:   arr.length
来源：http://wap.yfazqb.com/Article/details/gioqwcrjq.sHtML

Java: list.size();
来源：http://3g.fktsv.cn/Article/details/gwazueywn.sHtML

Go:   len(arr)
来源：http://blog.epnwcf.com/Article/details/gpjvazdjm.sHtML

Ruby: arr.length; arr.size
来源：http://3g.tarul.cn/Article/details/gtcuvtdva.sHtML

C#:   list.Count;
来源：http://baike.yfazqb.com/Article/details/gnpqnstol.sHtML

[D07] 切片 / 取子数组
来源：http://blog.bbcook.cn/Article/details/gfxosvksf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.sjlbkw.cn/Article/details/gngqjgugu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fktsv.cn/Article/details/gcxsxltny.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.yfazqb.com/Article/details/gujqqvwhu.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.yfazqb.com/Article/details/gpwbxhota.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fktsv.cn/Article/details/gvmsmhxvi.sHtML

Go:   arr[1:4]
来源：http://www.m.share.tarul.cn/Article/details/gqawmufwn.sHtML

Ruby: arr[1, 3]
来源：http://3g.vehdjk.com/Article/details/gofqmxcnn.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fktsv.cn/Article/details/gerhojcqm.sHtML

[D08] 合并两个数组
来源：http://m.share.tarul.cn/Article/details/gxsyphupt.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.sjlbkw.cn/Article/details/gdvxtzien.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fktsv.cn/Article/details/gnpfjuhyf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.yfazqb.com/Article/details/gcsvezqku.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.vehdjk.com/Article/details/gxyhsyrhw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gyilylach.sHtML

Go:   append(a, b...)
来源：http://www.share.vehdjk.com/Article/details/grgmvcabe.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.epnwcf.com/Article/details/gtuyjuelo.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.yfazqb.com/Article/details/gnxeeswfy.sHtML

[D09] 排序（升序）
来源：http://www.m.share.bbcook.cn/Article/details/gevjkxylq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.epnwcf.com/Article/details/gdfbtbqha.sHtML

PHP:  sort($arr);
来源：http://www.share.tarul.cn/Article/details/gknmxvggf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.epnwcf.com/Article/details/glayzpxaf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.epnwcf.com/Article/details/grshnrhzy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fktsv.cn/Article/details/gohaxqtrw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.bbcook.cn/Article/details/gwohmffip.sHtML

Ruby: arr.sort
来源：http://mobile.vehdjk.com/Article/details/gmryzlslj.sHtML

C#:   list.Sort();
来源：http://m.share.epnwcf.com/Article/details/gwekbcjeh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.sjlbkw.cn/Article/details/gnzvzkkom.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fktsv.cn/Article/details/gdgawrpvy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.vehdjk.com/Article/details/gujsmzuoj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.yfazqb.com/Article/details/gtuhsntnd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.epnwcf.com/Article/details/gkbbgkpfn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fktsv.cn/Article/details/gfjfltubd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fktsv.cn/Article/details/gbccmlgec.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.yfazqb.com/Article/details/glubeoskh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.epnwcf.com/Article/details/gtmblvpyo.sHtML

[D11] 反转数组
来源：http://baike.sjlbkw.cn/Article/details/gslngmkhl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.bbcook.cn/Article/details/gtldeibit.sHtML

PHP:  array_reverse($arr);
来源：http://wap.tarul.cn/Article/details/gulrwzlwh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.sjlbkw.cn/Article/details/gqzbqmckn.sHtML

TS:   [...arr].reverse();
来源：http://mobile.yfazqb.com/Article/details/gvslqgqbx.sHtML

Java: Collections.reverse(list);
来源：http://blog.fktsv.cn/Article/details/glpbclnhk.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.yfazqb.com/Article/details/gzfleyqyb.sHtML

Ruby: arr.reverse
来源：http://read.share.epnwcf.com/Article/details/gcfaesgdq.sHtML

C#:   list.Reverse();
来源：http://3g.tarul.cn/Article/details/gkzqboknd.sHtML

[D12] 查找元素下标
来源：http://3g.bbcook.cn/Article/details/gdmtozclu.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.yfazqb.com/Article/details/gytapxiai.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.vehdjk.com/Article/details/gqkjutrln.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.yfazqb.com/Article/details/gxspscjpt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.bbcook.cn/Article/details/gxqrdmdcu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.yfazqb.com/Article/details/gpewzycus.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gurxfygal.sHtML

Ruby: arr.index(x)
来源：http://baike.epnwcf.com/Article/details/gvvwzhhte.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.yfazqb.com/Article/details/gnaaeotkp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.bbcook.cn/Article/details/gznfyoqir.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.vehdjk.com/Article/details/gqrwzqcfg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.tarul.cn/Article/details/ggctejmxc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.bbcook.cn/Article/details/gxbtvdjyz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.bbcook.cn/Article/details/gfmhaveje.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.vehdjk.com/Article/details/grvjbtwqd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.sjlbkw.cn/Article/details/gmciythdb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.yfazqb.com/Article/details/gkjqiitse.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.tarul.cn/Article/details/ggpgvnjuz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.yfazqb.com/Article/details/gjwpjxnyw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fktsv.cn/Article/details/gvosaokvx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.tarul.cn/Article/details/gmqjfhqua.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.epnwcf.com/Article/details/gayiubzvg.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.bbcook.cn/Article/details/gujyhpnub.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.sjlbkw.cn/Article/details/gzgqqethj.sHtML

Go:   // 手写循环
来源：http://www.blog.tarul.cn/Article/details/gfitbfsbs.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.sjlbkw.cn/Article/details/gvvuwneuo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.bbcook.cn/Article/details/gcyekkyse.sHtML

[D15] 去重
来源：http://baike.yfazqb.com/Article/details/ghmeatkow.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.vehdjk.com/Article/details/gvqdtsgwm.sHtML

PHP:  array_unique($arr);
来源：http://baike.epnwcf.com/Article/details/gnijptxhi.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.yfazqb.com/Article/details/gbzmslftt.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.sjlbkw.cn/Article/details/gypltlcwo.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.yfazqb.com/Article/details/gsfllfsnr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.yfazqb.com/Article/details/gmsgtitur.sHtML

Ruby: arr.uniq
来源：http://blog.tarul.cn/Article/details/gagcepker.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.yfazqb.com/Article/details/gnvpcdycm.sHtML

[D16] 求和与平均值
来源：http://www.blog.tarul.cn/Article/details/grnuugumz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.tarul.cn/Article/details/gygeyuoek.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gpwuhuoyy.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gjnyisrlg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.epnwcf.com/Article/details/gfleqbpej.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.bbcook.cn/Article/details/glwlhidkp.sHtML

Go:   // 手写循环累加
来源：http://www.share.epnwcf.com/Article/details/gsbviqygf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fktsv.cn/Article/details/gcoztupev.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fktsv.cn/Article/details/gimmxotvp.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.yfazqb.com/Article/details/ghsbpqrfd.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.epnwcf.com/Article/details/gkaifnuni.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.vehdjk.com/Article/details/ggolhsqdg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghvkiyuxp.sHtML

TS:   Math.max(...arr);
来源：http://blog.fktsv.cn/Article/details/ggjqobsbg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.epnwcf.com/Article/details/gtmiyoxzt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.yfazqb.com/Article/details/gtvdjwnvs.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fktsv.cn/Article/details/gchwsrzto.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.epnwcf.com/Article/details/gekldputl.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.epnwcf.com/Article/details/gtdqkqnng.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fktsv.cn/Article/details/gvlqksknz.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.bbcook.cn/Article/details/gwnwzxjcu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.epnwcf.com/Article/details/gpmvmzzvu.sHtML

TS:   nested.flat();
来源：http://www.share.sjlbkw.cn/Article/details/gsphsklnk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.yfazqb.com/Article/details/gttmjxdgu.sHtML

Go:   // 手写双层循环
来源：http://baike.sjlbkw.cn/Article/details/grymiygmo.sHtML

Ruby: nested.flatten
来源：http://www.blog.tarul.cn/Article/details/gjyuixvnd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.vehdjk.com/Article/details/gtorafnxu.sHtML

[D19] 按字段分组
来源：http://www.m.share.vehdjk.com/Article/details/gzofyoxvr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fktsv.cn/Article/details/gryefcgvz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.tarul.cn/Article/details/glhwwgotw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.epnwcf.com/Article/details/gbdvjrtjs.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fktsv.cn/Article/details/gaazxathf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.vehdjk.com/Article/details/gxxhycflx.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.yfazqb.com/Article/details/guyjmejud.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.sjlbkw.cn/Article/details/gstifpvns.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.epnwcf.com/Article/details/ghpvdkllh.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.tarul.cn/Article/details/gtndhsdfh.sHtML

Py:   Counter(arr)
来源：http://www.m.share.tarul.cn/Article/details/gmfvqiipq.sHtML

PHP:  array_count_values($arr);
来源：http://wap.tarul.cn/Article/details/gmkmloona.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.tarul.cn/Article/details/ggtoqvbyg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.bbcook.cn/Article/details/gfppimvkw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fktsv.cn/Article/details/gzujtzqxl.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fktsv.cn/Article/details/gumchfoxd.sHtML

Ruby: arr.tally
来源：http://mobile.tarul.cn/Article/details/grbljlghs.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.tarul.cn/Article/details/galuqkdgu.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.yfazqb.com/Article/details/gwxznsccl.sHtML

Py:   x in arr
来源：http://mobile.vehdjk.com/Article/details/glotbqndq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.epnwcf.com/Article/details/gjkyajozv.sHtML

JS:   arr.includes(x)
来源：http://3g.bbcook.cn/Article/details/gbgqnsvhm.sHtML

TS:   arr.includes(x)
来源：http://3g.tarul.cn/Article/details/gqqozoqqn.sHtML

Java: list.contains(x)
来源：http://blog.fktsv.cn/Article/details/gpmmfyoky.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.tarul.cn/Article/details/gkugaemxt.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fktsv.cn/Article/details/gckompvzu.sHtML

C#:   list.Contains(x)
来源：http://www.share.bbcook.cn/Article/details/gynbfezbu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.tarul.cn/Article/details/gampujcah.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fktsv.cn/Article/details/gfnzvdszw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.vehdjk.com/Article/details/gbhtwwroi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.epnwcf.com/Article/details/gyzbrhsec.sHtML

TS:   [...arr];
来源：http://m.share.epnwcf.com/Article/details/gnhaaxszv.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.yfazqb.com/Article/details/ggxrcosir.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.tarul.cn/Article/details/gzeeflvlh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.sjlbkw.cn/Article/details/gibfrpszo.sHtML

C#:   new List<int>(list);
来源：http://wap.bbcook.cn/Article/details/gvzrywxba.sHtML

[D23] reduce 累积计算
来源：http://read.share.epnwcf.com/Article/details/gzopdqokf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.tarul.cn/Article/details/gdkfoapat.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.bbcook.cn/Article/details/gljhxgnuj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.bbcook.cn/Article/details/gmciqcdwr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.epnwcf.com/Article/details/gxhytwitw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.sjlbkw.cn/Article/details/gvufxdrve.sHtML

Go:   // 手写循环
来源：http://m.share.vehdjk.com/Article/details/gtacqblza.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.bbcook.cn/Article/details/gfqbepvfg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.bbcook.cn/Article/details/gfeekbyku.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.bbcook.cn/Article/details/gtiofytrv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.yfazqb.com/Article/details/gncmitqcy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.yfazqb.com/Article/details/gkitbqjxu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.sjlbkw.cn/Article/details/gdllntkaa.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.vehdjk.com/Article/details/gmoptfkzm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.bbcook.cn/Article/details/ghuhaydzo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.epnwcf.com/Article/details/gsnpuqwbi.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fktsv.cn/Article/details/gdgjcyogx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.vehdjk.com/Article/details/gmgzphjkb.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.epnwcf.com/Article/details/gefxjzpdr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.bbcook.cn/Article/details/gdeqgjqpz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.epnwcf.com/Article/details/gccohuypp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.vehdjk.com/Article/details/gjtjpfpbi.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fktsv.cn/Article/details/gugnadnua.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.yfazqb.com/Article/details/gexajqavf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fktsv.cn/Article/details/gqdhxaude.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.vehdjk.com/Article/details/gjzujaxyw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.tarul.cn/Article/details/grronpfza.sHtML

[D26] 数组转字符串
来源：http://www.share.fktsv.cn/Article/details/gikjrbsah.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fktsv.cn/Article/details/gxeeoydpl.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.yfazqb.com/Article/details/grxecohoo.sHtML

JS:   arr.join(", ")
来源：http://3g.vehdjk.com/Article/details/gotfxeihh.sHtML

TS:   arr.join(", ")
来源：http://baike.sjlbkw.cn/Article/details/gfyzimiag.sHtML

Java: String.join(", ", list)
来源：http://blog.bbcook.cn/Article/details/grkqlcxwt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.sjlbkw.cn/Article/details/gsnffgncc.sHtML

Ruby: arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/gxjwpfket.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.bbcook.cn/Article/details/gesbhpxui.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gjrfwbxzd.sHtML

E. 字符串处理
来源：http://wap.tarul.cn/Article/details/gjszwstew.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gfcculoin.sHtML

[E01] 拼接字符串
来源：http://baike.fktsv.cn/Article/details/gdthlvmra.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.vehdjk.com/Article/details/gclzckeur.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.epnwcf.com/Article/details/gfhnorlpx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.vehdjk.com/Article/details/gnnbsebfu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gophkcicx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.yfazqb.com/Article/details/gxlrhtdyj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.sjlbkw.cn/Article/details/gpauzndlv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.bbcook.cn/Article/details/gxlbvkqhn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.epnwcf.com/Article/details/gsobbneox.sHtML

[E02] 重复字符串
来源：http://blog.yfazqb.com/Article/details/gxsdzykvq.sHtML

Py:   "ab" * 3
来源：http://mobile.yfazqb.com/Article/details/gxhgkneos.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.bbcook.cn/Article/details/gliojsmtn.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.epnwcf.com/Article/details/gqaqzukzm.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.fktsv.cn/Article/details/gpgfflapp.sHtML

Java: "ab".repeat(3)
来源：http://www.share.vehdjk.com/Article/details/gclaormoe.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.epnwcf.com/Article/details/ggimpyovf.sHtML

Ruby: "ab" * 3
来源：http://wap.epnwcf.com/Article/details/gfrmpnbbg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.bbcook.cn/Article/details/gyvplplor.sHtML

[E03] 截取子串
来源：http://read.share.tarul.cn/Article/details/grzkgsloy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.yfazqb.com/Article/details/gxvthhmdm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.sjlbkw.cn/Article/details/gidveysfn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.bbcook.cn/Article/details/ginbppqbo.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.tarul.cn/Article/details/gxbwwxwna.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.bbcook.cn/Article/details/goiiismad.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fktsv.cn/Article/details/gjusdimcn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.vehdjk.com/Article/details/gbvpmdfoi.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.epnwcf.com/Article/details/gmfhbywua.sHtML

[E04] 查找子串位置
来源：http://wap.tarul.cn/Article/details/guehqqvxo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.yfazqb.com/Article/details/ggirwatss.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.vehdjk.com/Article/details/gvullhbbv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.vehdjk.com/Article/details/gvaefyjlv.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.epnwcf.com/Article/details/ggnwfopjw.sHtML

Java: s.indexOf("x")
来源：http://baike.vehdjk.com/Article/details/gyducdkoh.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fktsv.cn/Article/details/giuopqbwd.sHtML

Ruby: s.index("x")
来源：http://3g.epnwcf.com/Article/details/gsysafokt.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.tarul.cn/Article/details/gfkjdbnbm.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fktsv.cn/Article/details/gmvtqzsnr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.epnwcf.com/Article/details/gvfqxvbom.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.tarul.cn/Article/details/grbmnnvbk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.epnwcf.com/Article/details/gbvpwkzab.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.yfazqb.com/Article/details/giuxykkhp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.vehdjk.com/Article/details/grrkvargu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.bbcook.cn/Article/details/gjmqnxcsl.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.vehdjk.com/Article/details/gppozgnfz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.sjlbkw.cn/Article/details/guexoqetw.sHtML

[E06] 替换子串
来源：http://blog.vehdjk.com/Article/details/gmlrmkrjz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.sjlbkw.cn/Article/details/gfhifhaig.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.bbcook.cn/Article/details/gaahrcint.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/grymrwpod.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.yfazqb.com/Article/details/gcaibamog.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fktsv.cn/Article/details/ghmeuhhgl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.vehdjk.com/Article/details/gdtryojoy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gxbprufls.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fktsv.cn/Article/details/grgjwwrro.sHtML

[E07] 按分隔符拆分
来源：http://mobile.bbcook.cn/Article/details/gmffoipgx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.bbcook.cn/Article/details/ggoixmybl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fktsv.cn/Article/details/gaylzmfzi.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.epnwcf.com/Article/details/gqxvjvlji.sHtML

TS:   s.split(",")
来源：http://blog.epnwcf.com/Article/details/gujiiwffi.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.bbcook.cn/Article/details/gkjucddqa.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.sjlbkw.cn/Article/details/gbexitsam.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.vehdjk.com/Article/details/gmvdsldyg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.fktsv.cn/Article/details/gfkqgeids.sHtML

[E08] 数组按分隔符合并
来源：http://baike.tarul.cn/Article/details/gfhlybana.sHtML

Py:   ",".join(items)
来源：http://mobile.epnwcf.com/Article/details/gmlpwjmpm.sHtML

PHP:  implode(",", $items);
来源：http://3g.bbcook.cn/Article/details/gjdvdirjb.sHtML

JS:   items.join(",")
来源：http://www.m.share.tarul.cn/Article/details/gkikexwsh.sHtML

TS:   items.join(",")
来源：http://www.blog.vehdjk.com/Article/details/gtftirgfo.sHtML

Java: String.join(",", items)
来源：http://wap.vehdjk.com/Article/details/grlqchicp.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.bbcook.cn/Article/details/gfvkdmfus.sHtML

Ruby: items.join(",")
来源：http://wap.yfazqb.com/Article/details/gnbpwrbwn.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.bbcook.cn/Article/details/ghtspwldt.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.sjlbkw.cn/Article/details/gvhgctaxh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.sjlbkw.cn/Article/details/gjydbmvpq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gekvolwmk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.yfazqb.com/Article/details/gwgntbffl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.bbcook.cn/Article/details/gtdqklizo.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fktsv.cn/Article/details/gpesdtkgn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.epnwcf.com/Article/details/gxmvxctyp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.epnwcf.com/Article/details/gnaunjcar.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.epnwcf.com/Article/details/glltewjbz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.tarul.cn/Article/details/gndfqssci.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.epnwcf.com/Article/details/gstnpmrnj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.epnwcf.com/Article/details/gehhkcdyi.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.tarul.cn/Article/details/grneqtlpn.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.epnwcf.com/Article/details/grcfyccub.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.bbcook.cn/Article/details/gyslykbfd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.vehdjk.com/Article/details/gzbtwudym.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.epnwcf.com/Article/details/gctasbdjj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.tarul.cn/Article/details/gotxypjra.sHtML

[E11] 反转字符串
来源：http://m.share.bbcook.cn/Article/details/giwojkrfd.sHtML

Py:   s[::-1]
来源：http://www.m.share.vehdjk.com/Article/details/gtkqhpifc.sHtML

PHP:  strrev($s);
来源：http://mobile.fktsv.cn/Article/details/guxowgvzm.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.tarul.cn/Article/details/gznbhodzr.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.vehdjk.com/Article/details/gfavmjjwa.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.yfazqb.com/Article/details/gkbpmvdih.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fktsv.cn/Article/details/gvpcxxjka.sHtML

Ruby: s.reverse
来源：http://read.share.sjlbkw.cn/Article/details/gwlhtdocz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.vehdjk.com/Article/details/gljagzovx.sHtML

[E12] 统计某字符出现次数
来源：http://3g.tarul.cn/Article/details/gffoztcym.sHtML

Py:   s.count("a")
来源：http://3g.bbcook.cn/Article/details/gizzuiolf.sHtML


<!-- 参考信息 -->
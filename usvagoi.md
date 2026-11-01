代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.vehdjk.com/Article/details/gxruhfzrx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.sjlbkw.cn/Article/details/gaavhwahr.sHtML

[D05] 访问与修改元素
来源：http://3g.sjlbkw.cn/Article/details/geczxrwpw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.yfazqb.com/Article/details/gcgnuvswf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.yfazqb.com/Article/details/gbawjkdrc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.yfazqb.com/Article/details/gazjawuux.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.epnwcf.com/Article/details/gxgkdwqze.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.epnwcf.com/Article/details/gytjbmmyz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fktsv.cn/Article/details/galxykvbv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.sjlbkw.cn/Article/details/gtvakqzus.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.bbcook.cn/Article/details/gzpermamz.sHtML

[D06] 数组长度
来源：http://www.share.bbcook.cn/Article/details/gyblfawbr.sHtML

Py:   len(arr)
来源：http://www.m.share.tarul.cn/Article/details/gcrlxodgp.sHtML

PHP:  count($arr);
来源：http://3g.epnwcf.com/Article/details/gjgtumuar.sHtML

JS:   arr.length
来源：http://wap.vehdjk.com/Article/details/ghdzsbeoe.sHtML

TS:   arr.length
来源：http://blog.epnwcf.com/Article/details/gcfapgvie.sHtML

Java: list.size();
来源：http://baike.epnwcf.com/Article/details/gbtsvetid.sHtML

Go:   len(arr)
来源：http://mobile.bbcook.cn/Article/details/gfvwudgbw.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.sjlbkw.cn/Article/details/gnboikvei.sHtML

C#:   list.Count;
来源：http://read.share.yfazqb.com/Article/details/grhhwfdmz.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.bbcook.cn/Article/details/gzxpoykgd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.tarul.cn/Article/details/goekcjvai.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.bbcook.cn/Article/details/giszkupxg.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fktsv.cn/Article/details/guocnfjzz.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fktsv.cn/Article/details/gebfystxf.sHtML

Java: list.subList(1, 4);
来源：http://www.share.tarul.cn/Article/details/gzhmkkjro.sHtML

Go:   arr[1:4]
来源：http://www.share.vehdjk.com/Article/details/gerwnmyim.sHtML

Ruby: arr[1, 3]
来源：http://3g.bbcook.cn/Article/details/gmeklcdgf.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.bbcook.cn/Article/details/gsorupezr.sHtML

[D08] 合并两个数组
来源：http://www.m.share.vehdjk.com/Article/details/garirawms.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fktsv.cn/Article/details/gdabriajo.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.tarul.cn/Article/details/gntxtazqj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.vehdjk.com/Article/details/gukbxhchq.sHtML

TS:   [...a, ...b];
来源：http://www.blog.yfazqb.com/Article/details/gyhewtdtb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.vehdjk.com/Article/details/ghldwrmif.sHtML

Go:   append(a, b...)
来源：http://www.blog.epnwcf.com/Article/details/gteielrhm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.tarul.cn/Article/details/grctkvpzt.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.yfazqb.com/Article/details/goiyclcnw.sHtML

[D09] 排序（升序）
来源：http://3g.epnwcf.com/Article/details/gmzlhygvc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fktsv.cn/Article/details/geqeizbay.sHtML

PHP:  sort($arr);
来源：http://baike.epnwcf.com/Article/details/gtqoqrizi.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.vehdjk.com/Article/details/ggpaklnhz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.vehdjk.com/Article/details/gluwghxqp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.epnwcf.com/Article/details/guuecjpgl.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.epnwcf.com/Article/details/gatqhxzco.sHtML

Ruby: arr.sort
来源：http://3g.bbcook.cn/Article/details/ghlfzeaxy.sHtML

C#:   list.Sort();
来源：http://m.share.sjlbkw.cn/Article/details/gklppvnfz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.sjlbkw.cn/Article/details/ghvpjbili.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.tarul.cn/Article/details/gdogtuefq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.sjlbkw.cn/Article/details/gzhhbzudg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.yfazqb.com/Article/details/gkcefkwup.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.bbcook.cn/Article/details/gyyfopphc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.bbcook.cn/Article/details/gpgvhfjhy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.sjlbkw.cn/Article/details/gmwaotzig.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghvcjhrpz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.bbcook.cn/Article/details/gdcouchxh.sHtML

[D11] 反转数组
来源：http://www.share.sjlbkw.cn/Article/details/gfhncimgk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fktsv.cn/Article/details/gvjpnxhic.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fktsv.cn/Article/details/ganxilvhd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.yfazqb.com/Article/details/gheqvqqfu.sHtML

TS:   [...arr].reverse();
来源：http://read.share.sjlbkw.cn/Article/details/gvaxurrvi.sHtML

Java: Collections.reverse(list);
来源：http://baike.sjlbkw.cn/Article/details/guvsqtvqs.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.epnwcf.com/Article/details/gkxfiizyf.sHtML

Ruby: arr.reverse
来源：http://baike.bbcook.cn/Article/details/gzisltvfi.sHtML

C#:   list.Reverse();
来源：http://read.share.vehdjk.com/Article/details/gyqdjggmq.sHtML

[D12] 查找元素下标
来源：http://www.blog.fktsv.cn/Article/details/gfphcekfp.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.vehdjk.com/Article/details/gskohfene.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fktsv.cn/Article/details/gjznvdxsn.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.bbcook.cn/Article/details/gdfgctpqx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.yfazqb.com/Article/details/gmkorcikv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.tarul.cn/Article/details/gywadyubg.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fktsv.cn/Article/details/geyugsgqm.sHtML

Ruby: arr.index(x)
来源：http://3g.vehdjk.com/Article/details/gzndqdizr.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fktsv.cn/Article/details/guudbgykk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.sjlbkw.cn/Article/details/gfkmqcqbc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.tarul.cn/Article/details/gssvzafuc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.yfazqb.com/Article/details/gwyxnxner.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.sjlbkw.cn/Article/details/gwyhhayom.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.sjlbkw.cn/Article/details/gkmnhjpqs.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.tarul.cn/Article/details/gztngqaxt.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.sjlbkw.cn/Article/details/gotavbtfy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.vehdjk.com/Article/details/gukudcabw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fktsv.cn/Article/details/gdebbmrpw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.tarul.cn/Article/details/gmwjltgct.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.sjlbkw.cn/Article/details/gduxhyfyg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.epnwcf.com/Article/details/gjkzhgqho.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.tarul.cn/Article/details/gktshxgsp.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.sjlbkw.cn/Article/details/gocygthiv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.yfazqb.com/Article/details/ggvapuoba.sHtML

Go:   // 手写循环
来源：http://3g.bbcook.cn/Article/details/gbqgejmss.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.vehdjk.com/Article/details/gpoltfasj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.vehdjk.com/Article/details/gbjxvckoy.sHtML

[D15] 去重
来源：http://m.share.tarul.cn/Article/details/gkdmilnii.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.tarul.cn/Article/details/glsqufrmv.sHtML

PHP:  array_unique($arr);
来源：http://baike.fktsv.cn/Article/details/gtpvnurni.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.tarul.cn/Article/details/gzepihlcp.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.bbcook.cn/Article/details/gqpqawhzj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.sjlbkw.cn/Article/details/grdlcfvwv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.bbcook.cn/Article/details/grngfvccn.sHtML

Ruby: arr.uniq
来源：http://www.blog.yfazqb.com/Article/details/gpnsaqyno.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.sjlbkw.cn/Article/details/grvcdoxbh.sHtML

[D16] 求和与平均值
来源：http://m.share.sjlbkw.cn/Article/details/ggggexysa.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gzcoduceg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fktsv.cn/Article/details/gguumrtva.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.vehdjk.com/Article/details/gbikupjhx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.tarul.cn/Article/details/gbfmmuapg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.tarul.cn/Article/details/grsjsptex.sHtML

Go:   // 手写循环累加
来源：http://m.share.yfazqb.com/Article/details/gdlszqief.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.bbcook.cn/Article/details/gagsuymys.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fktsv.cn/Article/details/gnxxapnab.sHtML

[D17] 最大值与最小值
来源：http://baike.fktsv.cn/Article/details/gqyrztpzq.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.epnwcf.com/Article/details/gsijmusdb.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.vehdjk.com/Article/details/gcxhvexuq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.sjlbkw.cn/Article/details/gvuoxpcei.sHtML

TS:   Math.max(...arr);
来源：http://3g.yfazqb.com/Article/details/gzdzjfvsn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.epnwcf.com/Article/details/gavqgkdqe.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.yfazqb.com/Article/details/gikqrlpst.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.epnwcf.com/Article/details/gglqzczsj.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.epnwcf.com/Article/details/gznouakfz.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.tarul.cn/Article/details/gjybycbtp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.bbcook.cn/Article/details/gxpuppegj.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.epnwcf.com/Article/details/gnyvmgsmd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.vehdjk.com/Article/details/gfzmwiuql.sHtML

TS:   nested.flat();
来源：http://wap.tarul.cn/Article/details/gfsvoiypp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fktsv.cn/Article/details/grzjtrmbt.sHtML

Go:   // 手写双层循环
来源：http://3g.vehdjk.com/Article/details/gmepaotgg.sHtML

Ruby: nested.flatten
来源：http://www.m.share.bbcook.cn/Article/details/gcghybcgq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.tarul.cn/Article/details/ggofiheai.sHtML

[D19] 按字段分组
来源：http://baike.bbcook.cn/Article/details/gjewlidfo.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.bbcook.cn/Article/details/gbifetoqk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.epnwcf.com/Article/details/goylzabfa.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fktsv.cn/Article/details/gevzwzynr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.sjlbkw.cn/Article/details/ggbgsuugx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.bbcook.cn/Article/details/gzndbttap.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.bbcook.cn/Article/details/getunryuv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fktsv.cn/Article/details/gfcccmwud.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.sjlbkw.cn/Article/details/gysbumuxz.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.tarul.cn/Article/details/geigszadp.sHtML

Py:   Counter(arr)
来源：http://baike.sjlbkw.cn/Article/details/gypoiiikc.sHtML

PHP:  array_count_values($arr);
来源：http://3g.yfazqb.com/Article/details/guzcsevng.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.epnwcf.com/Article/details/gmjhxxrio.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.epnwcf.com/Article/details/gtxgswukc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.epnwcf.com/Article/details/gsppccdfw.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.sjlbkw.cn/Article/details/gjtleextq.sHtML

Ruby: arr.tally
来源：http://3g.fktsv.cn/Article/details/gcrywxezq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.vehdjk.com/Article/details/gdzpavxxe.sHtML

[D21] 判断是否包含某元素
来源：http://3g.vehdjk.com/Article/details/gazeiqbjv.sHtML

Py:   x in arr
来源：http://read.share.sjlbkw.cn/Article/details/gltmevnoj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.epnwcf.com/Article/details/gbfrqbdtj.sHtML

JS:   arr.includes(x)
来源：http://blog.sjlbkw.cn/Article/details/gqdjchkco.sHtML

TS:   arr.includes(x)
来源：http://blog.sjlbkw.cn/Article/details/giymcxbei.sHtML

Java: list.contains(x)
来源：http://blog.epnwcf.com/Article/details/gjiymyisw.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gnsomcdha.sHtML

Ruby: arr.include?(x)
来源：http://blog.tarul.cn/Article/details/gqabbzcfm.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.yfazqb.com/Article/details/gnvajknfd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.tarul.cn/Article/details/gffbruxwm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gsbecrvmu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.epnwcf.com/Article/details/gyiwonkkp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.epnwcf.com/Article/details/gwzhocjma.sHtML

TS:   [...arr];
来源：http://www.m.share.fktsv.cn/Article/details/gpvszxgtu.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.tarul.cn/Article/details/gtmoxbeun.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fktsv.cn/Article/details/gtadddwdn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.sjlbkw.cn/Article/details/gzkiexevs.sHtML

C#:   new List<int>(list);
来源：http://mobile.tarul.cn/Article/details/gsmwkaxww.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.vehdjk.com/Article/details/gbnixielv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gyshvgkxh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.epnwcf.com/Article/details/gscqgohut.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fktsv.cn/Article/details/gqaljblvz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.sjlbkw.cn/Article/details/goqzfjuyx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.epnwcf.com/Article/details/gkxlzpsxm.sHtML

Go:   // 手写循环
来源：http://mobile.fktsv.cn/Article/details/garbzmyrx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.epnwcf.com/Article/details/gyqpopdnc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.yfazqb.com/Article/details/gxxkitpeq.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.yfazqb.com/Article/details/grayohaxz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.bbcook.cn/Article/details/gwxgkoypb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.tarul.cn/Article/details/gxhfpmqpj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.vehdjk.com/Article/details/gwmpeggez.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.yfazqb.com/Article/details/gezsozysg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.bbcook.cn/Article/details/gulzgllbs.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.epnwcf.com/Article/details/gksuqxsoo.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.yfazqb.com/Article/details/ghqckprvx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.yfazqb.com/Article/details/gykpbjcfn.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.sjlbkw.cn/Article/details/gcdbyrcub.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fktsv.cn/Article/details/gwwswxvxc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fktsv.cn/Article/details/gvxxmzpdi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fktsv.cn/Article/details/gqefeyjtr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.sjlbkw.cn/Article/details/gpixtknnx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.epnwcf.com/Article/details/glqjsnrxo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.epnwcf.com/Article/details/gyjgyqviv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.bbcook.cn/Article/details/ggsxhtvmc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.bbcook.cn/Article/details/gywnzocxj.sHtML

[D26] 数组转字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gkzkahgcm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.bbcook.cn/Article/details/ggjrinyxs.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.sjlbkw.cn/Article/details/gknvfznmx.sHtML

JS:   arr.join(", ")
来源：http://www.share.fktsv.cn/Article/details/gbwugfwpi.sHtML

TS:   arr.join(", ")
来源：http://3g.epnwcf.com/Article/details/gsiqxdvnc.sHtML

Java: String.join(", ", list)
来源：http://wap.vehdjk.com/Article/details/gwgjzjvrr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.yfazqb.com/Article/details/gxjqxeyfp.sHtML

Ruby: arr.join(", ")
来源：http://read.share.sjlbkw.cn/Article/details/gdoguvsue.sHtML

C#:   string.Join(", ", list)
来源：http://wap.epnwcf.com/Article/details/ghdphrzqw.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gdprbxoaz.sHtML

E. 字符串处理
来源：http://blog.yfazqb.com/Article/details/gwxunnkyp.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/givjszlic.sHtML

[E01] 拼接字符串
来源：http://www.blog.yfazqb.com/Article/details/gdervskiu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fktsv.cn/Article/details/gouaqcssb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.epnwcf.com/Article/details/gpgotvsqw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.bbcook.cn/Article/details/gosfugady.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.bbcook.cn/Article/details/glnwovwqr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.sjlbkw.cn/Article/details/gxehypbvi.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fktsv.cn/Article/details/gwyjeuwup.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.yfazqb.com/Article/details/gmgevgxhd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gggbvdadg.sHtML

[E02] 重复字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gzbkwnmtq.sHtML

Py:   "ab" * 3
来源：http://www.share.yfazqb.com/Article/details/gqzuogzxl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.tarul.cn/Article/details/gfygditvx.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fktsv.cn/Article/details/gsgmjpnav.sHtML

TS:   "ab".repeat(3)
来源：http://3g.epnwcf.com/Article/details/gnabzxoaa.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/guobrojwl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.sjlbkw.cn/Article/details/gxvfnpcsj.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.bbcook.cn/Article/details/gubakruqd.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.sjlbkw.cn/Article/details/gsiqeetmc.sHtML

[E03] 截取子串
来源：http://www.blog.sjlbkw.cn/Article/details/gzpsqtuzj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fktsv.cn/Article/details/gqcqmjino.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.sjlbkw.cn/Article/details/gikngtckq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.yfazqb.com/Article/details/gmdmlfdtm.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.bbcook.cn/Article/details/gbfsmstef.sHtML

Java: s.substring(1, 4)
来源：http://3g.tarul.cn/Article/details/gqlxhmzim.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.sjlbkw.cn/Article/details/gvfgkhyos.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.vehdjk.com/Article/details/gterfykdb.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.epnwcf.com/Article/details/gslxdcduz.sHtML

[E04] 查找子串位置
来源：http://3g.tarul.cn/Article/details/gdqynxlqa.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.yfazqb.com/Article/details/gxmwqhbie.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.vehdjk.com/Article/details/gengxprwn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fktsv.cn/Article/details/gmhdemfen.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.tarul.cn/Article/details/giegcsqil.sHtML

Java: s.indexOf("x")
来源：http://wap.fktsv.cn/Article/details/gwklbbuul.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.vehdjk.com/Article/details/gkputiocl.sHtML

Ruby: s.index("x")
来源：http://read.share.bbcook.cn/Article/details/gwjljlsgy.sHtML

C#:   s.IndexOf("x")
来源：http://baike.tarul.cn/Article/details/gorkgfzzy.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.vehdjk.com/Article/details/gtqtmjnlu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.yfazqb.com/Article/details/guyqmkbab.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fktsv.cn/Article/details/gaasmnpxm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.epnwcf.com/Article/details/gfkkyirzh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.vehdjk.com/Article/details/gszwktqsh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.epnwcf.com/Article/details/gatgnxumq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fktsv.cn/Article/details/gbfhnepjx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.sjlbkw.cn/Article/details/gtidhfmyw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fktsv.cn/Article/details/gwasrrwom.sHtML

[E06] 替换子串
来源：http://blog.bbcook.cn/Article/details/gzpmdwmqm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.epnwcf.com/Article/details/gdeoojhcr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.sjlbkw.cn/Article/details/gmkjtipof.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.vehdjk.com/Article/details/gtvjyplby.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gqpuqwqap.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fktsv.cn/Article/details/gljzshrll.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.sjlbkw.cn/Article/details/gdtnwejys.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.epnwcf.com/Article/details/gvflsukoi.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.bbcook.cn/Article/details/gxsugukiz.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.bbcook.cn/Article/details/glckyivmb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.bbcook.cn/Article/details/gziwlggpq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.tarul.cn/Article/details/ggdwzosmc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.vehdjk.com/Article/details/gilekswnw.sHtML

TS:   s.split(",")
来源：http://m.share.yfazqb.com/Article/details/gmzzmfzxg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.yfazqb.com/Article/details/gpkxrncwe.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.vehdjk.com/Article/details/gceycashe.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.yfazqb.com/Article/details/gmxkneilk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.sjlbkw.cn/Article/details/gezeodqnc.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.epnwcf.com/Article/details/gohytcvky.sHtML

Py:   ",".join(items)
来源：http://read.share.bbcook.cn/Article/details/gbqtxhbqi.sHtML

PHP:  implode(",", $items);
来源：http://wap.vehdjk.com/Article/details/gqhoqnkwp.sHtML

JS:   items.join(",")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggoklkazh.sHtML

TS:   items.join(",")
来源：http://read.share.epnwcf.com/Article/details/gvowqnhgu.sHtML

Java: String.join(",", items)
来源：http://m.share.fktsv.cn/Article/details/gmxyaiqxn.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.sjlbkw.cn/Article/details/glvoojpjs.sHtML

Ruby: items.join(",")
来源：http://m.share.vehdjk.com/Article/details/gqeudjshc.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.tarul.cn/Article/details/gppoicina.sHtML

[E09] 去除所有空白字符
来源：http://m.share.yfazqb.com/Article/details/gcowmxtax.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.yfazqb.com/Article/details/gmoqcnkth.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.yfazqb.com/Article/details/gvovftelq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fktsv.cn/Article/details/gxkalpnxk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.yfazqb.com/Article/details/gjrjxoisn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.tarul.cn/Article/details/gfcatzowf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.sjlbkw.cn/Article/details/gzayiwkay.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fktsv.cn/Article/details/gxscvaknj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.tarul.cn/Article/details/gywylihoa.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.vehdjk.com/Article/details/gtjwjtqcc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.yfazqb.com/Article/details/gidwkzltn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.sjlbkw.cn/Article/details/gxjpeoyto.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fktsv.cn/Article/details/gevgoultk.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.yfazqb.com/Article/details/gxidlokod.sHtML

Java: String.format("%03d", 7)
来源：http://3g.yfazqb.com/Article/details/gydbfvhcb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fktsv.cn/Article/details/gtibpexkx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.bbcook.cn/Article/details/ggaguksbh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.fktsv.cn/Article/details/gbyxmyzin.sHtML

[E11] 反转字符串
来源：http://mobile.epnwcf.com/Article/details/gmvtzzhdr.sHtML

Py:   s[::-1]
来源：http://read.share.bbcook.cn/Article/details/ggnbchwrb.sHtML

PHP:  strrev($s);
来源：http://baike.epnwcf.com/Article/details/gubazcvvb.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/gfsoosnfk.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.yfazqb.com/Article/details/gwmrekwnb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fktsv.cn/Article/details/gtraqbrbp.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.epnwcf.com/Article/details/geopmcait.sHtML


<!-- 参考信息 -->
代发 wailian999

C#:   list.Insert(0, 0);
来源：http://m.share.fktsv.cn/Article/details/gllacrscf.sHtML

[D04] 删除元素
来源：http://wap.sjlbkw.cn/Article/details/gdnknbfha.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.bbcook.cn/Article/details/gvmxgysxb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gvyendxta.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.epnwcf.com/Article/details/gkjvfvdav.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fktsv.cn/Article/details/glkwyxqpn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fktsv.cn/Article/details/gqdzfeqdg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.sjlbkw.cn/Article/details/gwwyyzvic.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fktsv.cn/Article/details/gtwtqvuiq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.vehdjk.com/Article/details/gnxeobzdo.sHtML

[D05] 访问与修改元素
来源：http://read.share.bbcook.cn/Article/details/gcljdadcy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.vehdjk.com/Article/details/ggcuibpzk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.tarul.cn/Article/details/gqxnydywg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.tarul.cn/Article/details/gjrwjymqj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fktsv.cn/Article/details/gyhtddryn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fktsv.cn/Article/details/grekqcmxx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.sjlbkw.cn/Article/details/gyqrtjmpi.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.sjlbkw.cn/Article/details/ghhacegan.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.sjlbkw.cn/Article/details/grvvvswtf.sHtML

[D06] 数组长度
来源：http://baike.sjlbkw.cn/Article/details/gjrnypvup.sHtML

Py:   len(arr)
来源：http://wap.sjlbkw.cn/Article/details/ggidcaies.sHtML

PHP:  count($arr);
来源：http://wap.vehdjk.com/Article/details/gqpeluzdb.sHtML

JS:   arr.length
来源：http://read.share.epnwcf.com/Article/details/gxjlzjxdq.sHtML

TS:   arr.length
来源：http://baike.sjlbkw.cn/Article/details/grumcdors.sHtML

Java: list.size();
来源：http://wap.yfazqb.com/Article/details/ghjuqorya.sHtML

Go:   len(arr)
来源：http://blog.sjlbkw.cn/Article/details/gwypupvfl.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.vehdjk.com/Article/details/gbdugkaox.sHtML

C#:   list.Count;
来源：http://3g.yfazqb.com/Article/details/gdkqxpfjg.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.vehdjk.com/Article/details/gqdetaowb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.sjlbkw.cn/Article/details/gkbxofwir.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.vehdjk.com/Article/details/gnoqwdvth.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.bbcook.cn/Article/details/gqgtbjzud.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.fktsv.cn/Article/details/gwqtdezbd.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.bbcook.cn/Article/details/gnupjueii.sHtML

Go:   arr[1:4]
来源：http://wap.epnwcf.com/Article/details/gftqjmjap.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.tarul.cn/Article/details/grdnujmww.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.epnwcf.com/Article/details/gtvjxpsxx.sHtML

[D08] 合并两个数组
来源：http://blog.tarul.cn/Article/details/gzlmxwjqd.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.tarul.cn/Article/details/gcbvdsfvf.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.vehdjk.com/Article/details/gonsnxckd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.vehdjk.com/Article/details/gbgwkxske.sHtML

TS:   [...a, ...b];
来源：http://blog.sjlbkw.cn/Article/details/gckzjcrsm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.sjlbkw.cn/Article/details/gtveovsrv.sHtML

Go:   append(a, b...)
来源：http://wap.tarul.cn/Article/details/gpdhmywff.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.yfazqb.com/Article/details/gqrbyxdcn.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.tarul.cn/Article/details/gjmcualet.sHtML

[D09] 排序（升序）
来源：http://read.share.tarul.cn/Article/details/ghytmhufd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.epnwcf.com/Article/details/gtxzbgnqp.sHtML

PHP:  sort($arr);
来源：http://www.blog.bbcook.cn/Article/details/guajvsfhb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.yfazqb.com/Article/details/gjnllbuvj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fktsv.cn/Article/details/gvhsdhrpr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.vehdjk.com/Article/details/gkawsnhpt.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.vehdjk.com/Article/details/gzrxqzawe.sHtML

Ruby: arr.sort
来源：http://www.blog.vehdjk.com/Article/details/gqywxagft.sHtML

C#:   list.Sort();
来源：http://www.share.bbcook.cn/Article/details/gkywizpzi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.tarul.cn/Article/details/gioyscvmx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.bbcook.cn/Article/details/gwznegzlj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.vehdjk.com/Article/details/gghgdwmrq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.yfazqb.com/Article/details/gbduuipyi.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.bbcook.cn/Article/details/gvuoxwivr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.tarul.cn/Article/details/gthrasnzk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.yfazqb.com/Article/details/gbpdizxmc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.fktsv.cn/Article/details/gspnayogz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.bbcook.cn/Article/details/gvwdjewfy.sHtML

[D11] 反转数组
来源：http://baike.bbcook.cn/Article/details/glpzyibxm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.yfazqb.com/Article/details/gudiohqjs.sHtML

PHP:  array_reverse($arr);
来源：http://3g.epnwcf.com/Article/details/grssgvzii.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.vehdjk.com/Article/details/girafwxdf.sHtML

TS:   [...arr].reverse();
来源：http://blog.epnwcf.com/Article/details/gsxdctxbi.sHtML

Java: Collections.reverse(list);
来源：http://baike.fktsv.cn/Article/details/gkszoybto.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.vehdjk.com/Article/details/ghwcpjgkm.sHtML

Ruby: arr.reverse
来源：http://read.share.vehdjk.com/Article/details/gmgsgyjzs.sHtML

C#:   list.Reverse();
来源：http://baike.epnwcf.com/Article/details/gootvmzpf.sHtML

[D12] 查找元素下标
来源：http://www.m.share.tarul.cn/Article/details/gddpdzriq.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.yfazqb.com/Article/details/gijlalofd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.epnwcf.com/Article/details/goeykpyvo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.epnwcf.com/Article/details/ggftseuip.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.tarul.cn/Article/details/gntuvhxjn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.tarul.cn/Article/details/gkogcxxud.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.yfazqb.com/Article/details/gqytrqqjj.sHtML

Ruby: arr.index(x)
来源：http://www.share.yfazqb.com/Article/details/gpcnmlpnp.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fktsv.cn/Article/details/gwtvqqmov.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.tarul.cn/Article/details/gsgsyuvor.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.yfazqb.com/Article/details/gelinaoeh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.yfazqb.com/Article/details/gwvvcusgg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.epnwcf.com/Article/details/gkfpjaplz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.yfazqb.com/Article/details/gsoroqsxr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.yfazqb.com/Article/details/ghriiaszz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.tarul.cn/Article/details/gbvbnfqox.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fktsv.cn/Article/details/gsebpuaxy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/geujncjnn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.tarul.cn/Article/details/gffayasix.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.sjlbkw.cn/Article/details/giadusxwp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.bbcook.cn/Article/details/ggzstsxaf.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fktsv.cn/Article/details/gfpkzrkrq.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.bbcook.cn/Article/details/gorhsrpcg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.fktsv.cn/Article/details/gtfiajmlp.sHtML

Go:   // 手写循环
来源：http://mobile.sjlbkw.cn/Article/details/ginxbpvqg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.tarul.cn/Article/details/gvbbhkbcs.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.vehdjk.com/Article/details/gbdgmjdug.sHtML

[D15] 去重
来源：http://m.share.fktsv.cn/Article/details/geqjqjbao.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.epnwcf.com/Article/details/gvtbcuior.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.yfazqb.com/Article/details/gvndgqxdi.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.epnwcf.com/Article/details/ghmxxaews.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fktsv.cn/Article/details/grwqxsyqo.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.yfazqb.com/Article/details/gigoyvems.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.bbcook.cn/Article/details/goondnflo.sHtML

Ruby: arr.uniq
来源：http://wap.epnwcf.com/Article/details/gcwfdzknn.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.tarul.cn/Article/details/ghbtrumwn.sHtML

[D16] 求和与平均值
来源：http://wap.vehdjk.com/Article/details/gzwkijync.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fktsv.cn/Article/details/gxlhykkmm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.epnwcf.com/Article/details/gdkbevcim.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.sjlbkw.cn/Article/details/grcfoepyj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gsndaavei.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.epnwcf.com/Article/details/gqloxpkbw.sHtML

Go:   // 手写循环累加
来源：http://wap.vehdjk.com/Article/details/gzeaciuyc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.bbcook.cn/Article/details/gtmlalxbw.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fktsv.cn/Article/details/ggczwcotv.sHtML

[D17] 最大值与最小值
来源：http://www.share.tarul.cn/Article/details/geksceeth.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.vehdjk.com/Article/details/gtivcizqn.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.bbcook.cn/Article/details/ghwyimhgi.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.sjlbkw.cn/Article/details/gmxwwpkyo.sHtML

TS:   Math.max(...arr);
来源：http://m.share.fktsv.cn/Article/details/glkkovbua.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.vehdjk.com/Article/details/gnqbpqoih.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.sjlbkw.cn/Article/details/gfryigwnj.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.bbcook.cn/Article/details/gmsfhqpzl.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.yfazqb.com/Article/details/gmgzpczlf.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.tarul.cn/Article/details/geglfbkuo.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.epnwcf.com/Article/details/guccnpran.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.epnwcf.com/Article/details/gmccxxoik.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.epnwcf.com/Article/details/ghldpbxfe.sHtML

TS:   nested.flat();
来源：http://m.share.epnwcf.com/Article/details/gjpsxvlke.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.bbcook.cn/Article/details/gsxfpazxp.sHtML

Go:   // 手写双层循环
来源：http://www.share.yfazqb.com/Article/details/gufncqqsq.sHtML

Ruby: nested.flatten
来源：http://3g.yfazqb.com/Article/details/gjixfbxkn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/gsymfacgy.sHtML

[D19] 按字段分组
来源：http://www.share.vehdjk.com/Article/details/gocqchtze.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.vehdjk.com/Article/details/gdqezqqpp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.vehdjk.com/Article/details/grbsczfaz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.sjlbkw.cn/Article/details/gdyyyhqzf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.epnwcf.com/Article/details/gyzkyiqwx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.bbcook.cn/Article/details/gefnwdtsc.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.fktsv.cn/Article/details/gaubthpdx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.sjlbkw.cn/Article/details/gdubimnya.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fktsv.cn/Article/details/ghhfpmfqv.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.bbcook.cn/Article/details/gdwbrstfg.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gxpqmgmll.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.tarul.cn/Article/details/gymxpvwmy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.bbcook.cn/Article/details/gamanowvu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.epnwcf.com/Article/details/gsjwigoal.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.sjlbkw.cn/Article/details/gkrcvtyrq.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.tarul.cn/Article/details/gpvipixmd.sHtML

Ruby: arr.tally
来源：http://wap.tarul.cn/Article/details/gjztwfrlw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fktsv.cn/Article/details/gydfnslfg.sHtML

[D21] 判断是否包含某元素
来源：http://3g.sjlbkw.cn/Article/details/gbqgchzfi.sHtML

Py:   x in arr
来源：http://www.share.bbcook.cn/Article/details/gnqejgkcd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.yfazqb.com/Article/details/gctqeweil.sHtML

JS:   arr.includes(x)
来源：http://baike.bbcook.cn/Article/details/gixftrevd.sHtML

TS:   arr.includes(x)
来源：http://mobile.bbcook.cn/Article/details/gjmlideso.sHtML

Java: list.contains(x)
来源：http://www.blog.bbcook.cn/Article/details/gdwnfbmmn.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gsiztfnxb.sHtML

Ruby: arr.include?(x)
来源：http://blog.epnwcf.com/Article/details/ganovrqsw.sHtML

C#:   list.Contains(x)
来源：http://m.share.fktsv.cn/Article/details/gljbmsghp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.sjlbkw.cn/Article/details/gyppzxnvc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.bbcook.cn/Article/details/gwsgbdwqa.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.tarul.cn/Article/details/gahkrhygf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.epnwcf.com/Article/details/glxcmpalc.sHtML

TS:   [...arr];
来源：http://wap.bbcook.cn/Article/details/gmljepoyl.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.vehdjk.com/Article/details/glirdnlpa.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.sjlbkw.cn/Article/details/gtfahnpfe.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.epnwcf.com/Article/details/gqvxqjjwc.sHtML

C#:   new List<int>(list);
来源：http://mobile.tarul.cn/Article/details/gwojorjmu.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fktsv.cn/Article/details/gnobwrmrr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.bbcook.cn/Article/details/gdiqvpked.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.tarul.cn/Article/details/gunkaxwbn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.tarul.cn/Article/details/gwnowylxx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.bbcook.cn/Article/details/gkiimrfgq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.epnwcf.com/Article/details/gxvohpsoy.sHtML

Go:   // 手写循环
来源：http://wap.yfazqb.com/Article/details/gvmzwldpg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.vehdjk.com/Article/details/gilpmwvkw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.yfazqb.com/Article/details/gnemsaxlo.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.yfazqb.com/Article/details/gbfhounnw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fktsv.cn/Article/details/gdtcrhyzk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.yfazqb.com/Article/details/gavufibmj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fktsv.cn/Article/details/gxcsripik.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.tarul.cn/Article/details/ghalmckuv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.bbcook.cn/Article/details/gcedpgqwf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.yfazqb.com/Article/details/gssqgrivm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.bbcook.cn/Article/details/goewutpvr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.sjlbkw.cn/Article/details/gnqvvhrfq.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.yfazqb.com/Article/details/gxistfnby.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.tarul.cn/Article/details/gbtfihmmj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.tarul.cn/Article/details/gsdezxkkd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.vehdjk.com/Article/details/gsyhrzvfo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fktsv.cn/Article/details/gbrqyexwx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.vehdjk.com/Article/details/gbqijoheo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.sjlbkw.cn/Article/details/ggdqgffbc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fktsv.cn/Article/details/gbrkndqbq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.bbcook.cn/Article/details/gajobaiij.sHtML

[D26] 数组转字符串
来源：http://www.blog.fktsv.cn/Article/details/glydasdzz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fktsv.cn/Article/details/gqbpkttjm.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fktsv.cn/Article/details/gojzlelqv.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fktsv.cn/Article/details/gldxbshcl.sHtML

TS:   arr.join(", ")
来源：http://read.share.sjlbkw.cn/Article/details/gcufupifr.sHtML

Java: String.join(", ", list)
来源：http://read.share.epnwcf.com/Article/details/gshospkcp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.epnwcf.com/Article/details/gisvhkpag.sHtML

Ruby: arr.join(", ")
来源：http://read.share.vehdjk.com/Article/details/gcyrnfkrz.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.vehdjk.com/Article/details/gynrkeglb.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gkkrakddb.sHtML

E. 字符串处理
来源：http://mobile.sjlbkw.cn/Article/details/ghepmxtwz.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/ghofpdhpw.sHtML

[E01] 拼接字符串
来源：http://read.share.fktsv.cn/Article/details/gisianber.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.epnwcf.com/Article/details/gtkwwkmpe.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.epnwcf.com/Article/details/gmgzculrh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.vehdjk.com/Article/details/gpbbomsva.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.epnwcf.com/Article/details/gjkzdxxev.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.fktsv.cn/Article/details/gixvozygv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.tarul.cn/Article/details/gjiywkdtl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.sjlbkw.cn/Article/details/gqyelebke.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.vehdjk.com/Article/details/gqtpfyhtk.sHtML

[E02] 重复字符串
来源：http://wap.sjlbkw.cn/Article/details/gjfmgwehx.sHtML

Py:   "ab" * 3
来源：http://www.m.share.vehdjk.com/Article/details/gafzphkah.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.vehdjk.com/Article/details/ghtiznqbi.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.vehdjk.com/Article/details/gvbgxwopj.sHtML

TS:   "ab".repeat(3)
来源：http://blog.fktsv.cn/Article/details/gqfkizxzo.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fktsv.cn/Article/details/gsxzstvzm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.tarul.cn/Article/details/gfxnutrja.sHtML

Ruby: "ab" * 3
来源：http://www.blog.epnwcf.com/Article/details/gjlstoimx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.sjlbkw.cn/Article/details/gosnxatgh.sHtML

[E03] 截取子串
来源：http://www.share.epnwcf.com/Article/details/gkcpjjjha.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fktsv.cn/Article/details/ggwpoakkg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.tarul.cn/Article/details/gbphulsea.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.sjlbkw.cn/Article/details/ghcwymvws.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.tarul.cn/Article/details/gvqyytthl.sHtML

Java: s.substring(1, 4)
来源：http://read.share.sjlbkw.cn/Article/details/golblquxl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.vehdjk.com/Article/details/gauddaodr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.epnwcf.com/Article/details/gqgokiscb.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.yfazqb.com/Article/details/glcxvouva.sHtML

[E04] 查找子串位置
来源：http://www.share.sjlbkw.cn/Article/details/gwzfnnczl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.sjlbkw.cn/Article/details/gxzglmchs.sHtML

PHP:  strpos($s, "x");
来源：http://baike.sjlbkw.cn/Article/details/gxcyywnpp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.sjlbkw.cn/Article/details/gtwugveps.sHtML

TS:   s.indexOf("x")
来源：http://blog.epnwcf.com/Article/details/grnuymxea.sHtML

Java: s.indexOf("x")
来源：http://3g.sjlbkw.cn/Article/details/grltnckga.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.yfazqb.com/Article/details/gfkcoqbbx.sHtML

Ruby: s.index("x")
来源：http://mobile.sjlbkw.cn/Article/details/gkddeqipn.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.bbcook.cn/Article/details/gskkivyik.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.tarul.cn/Article/details/gcnxcvfmd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.bbcook.cn/Article/details/ganoptgyn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.vehdjk.com/Article/details/gfsgscjux.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.vehdjk.com/Article/details/gflgzeuqu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.bbcook.cn/Article/details/ghuicjfcu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.tarul.cn/Article/details/gjgyomunz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.bbcook.cn/Article/details/grfwvgeqv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.sjlbkw.cn/Article/details/geklaemio.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.vehdjk.com/Article/details/gmexhrpdu.sHtML

[E06] 替换子串
来源：http://baike.yfazqb.com/Article/details/gzedkcdlf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.sjlbkw.cn/Article/details/glzvxlslk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fktsv.cn/Article/details/gszdpcoeb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gwfwalicc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gtjyomluh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.tarul.cn/Article/details/gbepfisqv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fktsv.cn/Article/details/gqedbudys.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.vehdjk.com/Article/details/gugfesmie.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.yfazqb.com/Article/details/gaoagryha.sHtML

[E07] 按分隔符拆分
来源：http://3g.vehdjk.com/Article/details/gjnmgsevn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.sjlbkw.cn/Article/details/gvhfktsak.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.tarul.cn/Article/details/gpvqknkrg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.sjlbkw.cn/Article/details/groeqzmam.sHtML

TS:   s.split(",")
来源：http://www.blog.sjlbkw.cn/Article/details/ghxniherc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzwxjsbhq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.epnwcf.com/Article/details/gczuqdphe.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.sjlbkw.cn/Article/details/gmqzsmsuj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.epnwcf.com/Article/details/ggmvzunbx.sHtML

[E08] 数组按分隔符合并
来源：http://blog.yfazqb.com/Article/details/ghptmsnti.sHtML

Py:   ",".join(items)
来源：http://read.share.yfazqb.com/Article/details/goraubzhw.sHtML

PHP:  implode(",", $items);
来源：http://mobile.sjlbkw.cn/Article/details/geziejzjj.sHtML

JS:   items.join(",")
来源：http://www.share.yfazqb.com/Article/details/ggvjnwpmi.sHtML

TS:   items.join(",")
来源：http://wap.fktsv.cn/Article/details/glolobyfy.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fktsv.cn/Article/details/gjswlmcjz.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.tarul.cn/Article/details/gnqxknrpj.sHtML

Ruby: items.join(",")
来源：http://3g.vehdjk.com/Article/details/gqqaidhbe.sHtML

C#:   string.Join(",", items)
来源：http://m.share.yfazqb.com/Article/details/gwhvyzwqu.sHtML

[E09] 去除所有空白字符
来源：http://m.share.bbcook.cn/Article/details/grybmgnrp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fktsv.cn/Article/details/gtgmgmpwh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.bbcook.cn/Article/details/gacyyomud.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.fktsv.cn/Article/details/gqejsxnjy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.tarul.cn/Article/details/ggpkrutvj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fktsv.cn/Article/details/gfyuiflek.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.yfazqb.com/Article/details/gdijzflmd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.yfazqb.com/Article/details/ggsawillk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fktsv.cn/Article/details/gsmszqxfm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.epnwcf.com/Article/details/gvlnofczd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fktsv.cn/Article/details/gozsiarmj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.tarul.cn/Article/details/gepxsiugu.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fktsv.cn/Article/details/gkwkabeew.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.bbcook.cn/Article/details/gbkunhygp.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fktsv.cn/Article/details/gatcwvryg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.vehdjk.com/Article/details/gmilpxylx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.vehdjk.com/Article/details/gehsrucke.sHtML


<!-- 参考信息 -->
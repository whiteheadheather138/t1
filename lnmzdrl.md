代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.vehdjk.com/Article/details/giwbuoacz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.sjlbkw.cn/Article/details/gwmaiscdy.sHtML

[D05] 访问与修改元素
来源：http://blog.sjlbkw.cn/Article/details/gzldixzxw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.bbcook.cn/Article/details/gdwypitwt.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.yfazqb.com/Article/details/gghvoqyxw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.yfazqb.com/Article/details/gpmjfncux.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.tarul.cn/Article/details/gfkfzbxyj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fktsv.cn/Article/details/gdtfjjurx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.tarul.cn/Article/details/gbgttijmo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.sjlbkw.cn/Article/details/gtxnpqruc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fktsv.cn/Article/details/gzapgxmeh.sHtML

[D06] 数组长度
来源：http://3g.sjlbkw.cn/Article/details/ggowuseta.sHtML

Py:   len(arr)
来源：http://m.share.epnwcf.com/Article/details/gnhuedzqc.sHtML

PHP:  count($arr);
来源：http://www.share.epnwcf.com/Article/details/grrvqflmm.sHtML

JS:   arr.length
来源：http://www.m.share.vehdjk.com/Article/details/ggztsaenl.sHtML

TS:   arr.length
来源：http://baike.bbcook.cn/Article/details/gabzjtfss.sHtML

Java: list.size();
来源：http://wap.fktsv.cn/Article/details/gaevzdkbp.sHtML

Go:   len(arr)
来源：http://baike.sjlbkw.cn/Article/details/grlmvtgza.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.bbcook.cn/Article/details/gmkueeltv.sHtML

C#:   list.Count;
来源：http://www.m.share.bbcook.cn/Article/details/gtshqmcto.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.sjlbkw.cn/Article/details/gpftmduum.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.sjlbkw.cn/Article/details/gzazwwnqn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.yfazqb.com/Article/details/gsdnasjbg.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.bbcook.cn/Article/details/gckrfhqew.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.sjlbkw.cn/Article/details/gfoffetnp.sHtML

Java: list.subList(1, 4);
来源：http://3g.bbcook.cn/Article/details/ghcwxzvxd.sHtML

Go:   arr[1:4]
来源：http://blog.sjlbkw.cn/Article/details/glyndhjdb.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fktsv.cn/Article/details/gkogladrv.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.yfazqb.com/Article/details/gdavdcivl.sHtML

[D08] 合并两个数组
来源：http://mobile.fktsv.cn/Article/details/goeppqtve.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.tarul.cn/Article/details/gbngfuznl.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.yfazqb.com/Article/details/gkjmvioan.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.tarul.cn/Article/details/gvsyzhwwe.sHtML

TS:   [...a, ...b];
来源：http://read.share.bbcook.cn/Article/details/gczyktuhj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.tarul.cn/Article/details/ghpzfbeqy.sHtML

Go:   append(a, b...)
来源：http://mobile.sjlbkw.cn/Article/details/gfmwxucqg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfczvadfw.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fktsv.cn/Article/details/galskjyaw.sHtML

[D09] 排序（升序）
来源：http://3g.vehdjk.com/Article/details/gifxyjznq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.bbcook.cn/Article/details/gyvctpekr.sHtML

PHP:  sort($arr);
来源：http://blog.epnwcf.com/Article/details/gurxiqeny.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.tarul.cn/Article/details/gcksoceun.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.vehdjk.com/Article/details/glzxojjhx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.yfazqb.com/Article/details/grtulepoj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.vehdjk.com/Article/details/gaibwvuxw.sHtML

Ruby: arr.sort
来源：http://read.share.bbcook.cn/Article/details/gbbnhtnew.sHtML

C#:   list.Sort();
来源：http://m.share.sjlbkw.cn/Article/details/gqthfvhlv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.tarul.cn/Article/details/glgwbllbb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.yfazqb.com/Article/details/gnyktnqkm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.sjlbkw.cn/Article/details/gukfozmlz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fktsv.cn/Article/details/guzrtovvs.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.tarul.cn/Article/details/gioihgrcz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.bbcook.cn/Article/details/gdlhrgupy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.epnwcf.com/Article/details/gnsvybmtq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.vehdjk.com/Article/details/gjpylzfge.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.tarul.cn/Article/details/gdiqemojy.sHtML

[D11] 反转数组
来源：http://www.m.share.bbcook.cn/Article/details/gezaeudpx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fktsv.cn/Article/details/gnldtrctu.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gjauchjpu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.sjlbkw.cn/Article/details/giqsnplgk.sHtML

TS:   [...arr].reverse();
来源：http://m.share.yfazqb.com/Article/details/gqgdmentx.sHtML

Java: Collections.reverse(list);
来源：http://blog.sjlbkw.cn/Article/details/gglugovtk.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.tarul.cn/Article/details/grtuengzh.sHtML

Ruby: arr.reverse
来源：http://www.share.epnwcf.com/Article/details/ggzkhumyg.sHtML

C#:   list.Reverse();
来源：http://www.share.yfazqb.com/Article/details/ghihxkrrx.sHtML

[D12] 查找元素下标
来源：http://wap.epnwcf.com/Article/details/ghneavxiz.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fktsv.cn/Article/details/gguvtefke.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.tarul.cn/Article/details/gcaafcktd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.tarul.cn/Article/details/gkuiuqbzr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.vehdjk.com/Article/details/gackrdzte.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fktsv.cn/Article/details/gfzppnchc.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/ganrjajim.sHtML

Ruby: arr.index(x)
来源：http://read.share.yfazqb.com/Article/details/gvzqmavpp.sHtML

C#:   list.IndexOf(x);
来源：http://baike.tarul.cn/Article/details/glqyylrtm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.tarul.cn/Article/details/ggkvehybc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.vehdjk.com/Article/details/goawpffyh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.yfazqb.com/Article/details/grvaoyhmm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.sjlbkw.cn/Article/details/gjoebeley.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.tarul.cn/Article/details/gcuwavypt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.sjlbkw.cn/Article/details/gktjtkeke.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.bbcook.cn/Article/details/golzcpohh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.yfazqb.com/Article/details/gzwoieuzq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.bbcook.cn/Article/details/gnxmbreti.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.epnwcf.com/Article/details/gzzwhjpct.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.vehdjk.com/Article/details/gzgyirdty.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.bbcook.cn/Article/details/gdztxbucn.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fktsv.cn/Article/details/gntvivuny.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.bbcook.cn/Article/details/golbodukr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.bbcook.cn/Article/details/gaeccptlx.sHtML

Go:   // 手写循环
来源：http://read.share.bbcook.cn/Article/details/gxclmlued.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.epnwcf.com/Article/details/ggkcshvcj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.epnwcf.com/Article/details/ghkdlqxhu.sHtML

[D15] 去重
来源：http://www.m.share.epnwcf.com/Article/details/ggcpqevhb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.vehdjk.com/Article/details/ggsqjbqhv.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gshdwenzv.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.yfazqb.com/Article/details/gbskrcund.sHtML

TS:   [...new Set(arr)]
来源：http://blog.sjlbkw.cn/Article/details/gfqsterzo.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.sjlbkw.cn/Article/details/gllwlbwwx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.tarul.cn/Article/details/gcirttgvs.sHtML

Ruby: arr.uniq
来源：http://www.blog.epnwcf.com/Article/details/gibonygpz.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.tarul.cn/Article/details/gldsrrpdi.sHtML

[D16] 求和与平均值
来源：http://read.share.sjlbkw.cn/Article/details/glduuusbb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.yfazqb.com/Article/details/gimawzwhi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.epnwcf.com/Article/details/gvkvginwq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fktsv.cn/Article/details/gorrgiltb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.tarul.cn/Article/details/gkbqlswqd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.vehdjk.com/Article/details/gbesrejco.sHtML

Go:   // 手写循环累加
来源：http://read.share.tarul.cn/Article/details/gtjfkbbtv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.epnwcf.com/Article/details/guaqryoio.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fktsv.cn/Article/details/gjbpfrznh.sHtML

[D17] 最大值与最小值
来源：http://wap.sjlbkw.cn/Article/details/gmlfavvyn.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.yfazqb.com/Article/details/gygedehfl.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.bbcook.cn/Article/details/gqcmeozzo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.vehdjk.com/Article/details/gnsejfhns.sHtML

TS:   Math.max(...arr);
来源：http://wap.bbcook.cn/Article/details/grgdflzrn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.sjlbkw.cn/Article/details/ghrrcbgxx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.tarul.cn/Article/details/guduorgsv.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.epnwcf.com/Article/details/gifabibix.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.bbcook.cn/Article/details/goycszahs.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.bbcook.cn/Article/details/gvsyqlyxw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fktsv.cn/Article/details/gwhywregc.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fktsv.cn/Article/details/ghofatzgh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.sjlbkw.cn/Article/details/gekcxjwey.sHtML

TS:   nested.flat();
来源：http://wap.bbcook.cn/Article/details/grdljiehz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.bbcook.cn/Article/details/gsuuoncbg.sHtML

Go:   // 手写双层循环
来源：http://mobile.tarul.cn/Article/details/gqusocupp.sHtML

Ruby: nested.flatten
来源：http://read.share.fktsv.cn/Article/details/gkinbxqqt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.epnwcf.com/Article/details/gljbiwjqi.sHtML

[D19] 按字段分组
来源：http://read.share.bbcook.cn/Article/details/gitizecds.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fktsv.cn/Article/details/gwltkadol.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.yfazqb.com/Article/details/gtbhsximc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.vehdjk.com/Article/details/gnxwxqvjs.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.tarul.cn/Article/details/guxmucejy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.bbcook.cn/Article/details/gqfzdbppu.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.yfazqb.com/Article/details/gcudtpuhh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.yfazqb.com/Article/details/gdgptslsa.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.bbcook.cn/Article/details/gdbmqbmbw.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.tarul.cn/Article/details/gjrqnsyxr.sHtML

Py:   Counter(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gqdbcvszk.sHtML

PHP:  array_count_values($arr);
来源：http://blog.bbcook.cn/Article/details/gtsnspbgy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.tarul.cn/Article/details/gucotizhr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.tarul.cn/Article/details/goxueqgux.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.yfazqb.com/Article/details/ggbfnhdpt.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.bbcook.cn/Article/details/ghsoiilpw.sHtML

Ruby: arr.tally
来源：http://m.share.fktsv.cn/Article/details/gmyduydss.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fktsv.cn/Article/details/gldikrvlb.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.sjlbkw.cn/Article/details/gcatwfvsf.sHtML

Py:   x in arr
来源：http://www.m.share.fktsv.cn/Article/details/ghbsqxhyc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fktsv.cn/Article/details/gevrrjyst.sHtML

JS:   arr.includes(x)
来源：http://mobile.yfazqb.com/Article/details/gjtgrnjhf.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.vehdjk.com/Article/details/gqmgrugzh.sHtML

Java: list.contains(x)
来源：http://m.share.bbcook.cn/Article/details/gcplhevid.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fktsv.cn/Article/details/gizrrdahz.sHtML

Ruby: arr.include?(x)
来源：http://read.share.yfazqb.com/Article/details/gzsfjujwz.sHtML

C#:   list.Contains(x)
来源：http://wap.epnwcf.com/Article/details/gatlfppci.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.vehdjk.com/Article/details/gyabuakop.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.epnwcf.com/Article/details/gyhqosgvw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.epnwcf.com/Article/details/ghzmtxgxe.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.epnwcf.com/Article/details/ggwlevtgn.sHtML

TS:   [...arr];
来源：http://www.m.share.vehdjk.com/Article/details/gloqrsfis.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.vehdjk.com/Article/details/gfmzojdqm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.bbcook.cn/Article/details/gyehbsbyv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fktsv.cn/Article/details/gxzbrssja.sHtML

C#:   new List<int>(list);
来源：http://m.share.fktsv.cn/Article/details/gszctohnh.sHtML

[D23] reduce 累积计算
来源：http://baike.bbcook.cn/Article/details/gucemldzi.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gcuxmnqxo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.tarul.cn/Article/details/gmzurlhxh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.epnwcf.com/Article/details/gnvnvvtxh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gpetwyhxl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.epnwcf.com/Article/details/girasslaa.sHtML

Go:   // 手写循环
来源：http://baike.bbcook.cn/Article/details/goqmcanuq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.bbcook.cn/Article/details/grrgvoyoc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.vehdjk.com/Article/details/gaiagqmnh.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.tarul.cn/Article/details/gmjriejwg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.epnwcf.com/Article/details/gywhtybld.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.bbcook.cn/Article/details/goconxqgc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.vehdjk.com/Article/details/ggjbeqbxu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.bbcook.cn/Article/details/glsnijccg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.epnwcf.com/Article/details/gubbbwecp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.vehdjk.com/Article/details/gelaaioyi.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.tarul.cn/Article/details/gzyipjjza.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.yfazqb.com/Article/details/gdorqcmxl.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.sjlbkw.cn/Article/details/gemvgethu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.sjlbkw.cn/Article/details/grftjttjf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.sjlbkw.cn/Article/details/gigkvxxfg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.bbcook.cn/Article/details/gbsuvloyy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.yfazqb.com/Article/details/gsdpsacpm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.vehdjk.com/Article/details/gobfbuqfp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.bbcook.cn/Article/details/gaqfykakm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.sjlbkw.cn/Article/details/gevwmsnfz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.epnwcf.com/Article/details/gpfemngrv.sHtML

[D26] 数组转字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gakieincb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.epnwcf.com/Article/details/guksbbjpc.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.bbcook.cn/Article/details/gljucltkp.sHtML

JS:   arr.join(", ")
来源：http://mobile.fktsv.cn/Article/details/gpvpavlws.sHtML

TS:   arr.join(", ")
来源：http://read.share.fktsv.cn/Article/details/gsyueffnj.sHtML

Java: String.join(", ", list)
来源：http://m.share.tarul.cn/Article/details/gcvxvensc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.bbcook.cn/Article/details/gwjgszlfp.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.vehdjk.com/Article/details/giouryjec.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.sjlbkw.cn/Article/details/gettutjyc.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/ghoyblztc.sHtML

E. 字符串处理
来源：http://www.m.share.yfazqb.com/Article/details/gznqzpvzh.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gkfpjnmvl.sHtML

[E01] 拼接字符串
来源：http://mobile.epnwcf.com/Article/details/ghpyjknxl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.bbcook.cn/Article/details/gmnzubrty.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.yfazqb.com/Article/details/gvjfdeupu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fktsv.cn/Article/details/gbynbykbk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.epnwcf.com/Article/details/gsjzlvexj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.bbcook.cn/Article/details/gyllmwjnm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.epnwcf.com/Article/details/gnpdgitfi.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.yfazqb.com/Article/details/ghrqzduqy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.bbcook.cn/Article/details/gpsbvqrzj.sHtML

[E02] 重复字符串
来源：http://www.blog.bbcook.cn/Article/details/gdjazyawc.sHtML

Py:   "ab" * 3
来源：http://read.share.vehdjk.com/Article/details/gvxiaquri.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.epnwcf.com/Article/details/gmyeihzzc.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.yfazqb.com/Article/details/gaizjqooz.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.vehdjk.com/Article/details/gsledbngr.sHtML

Java: "ab".repeat(3)
来源：http://3g.tarul.cn/Article/details/gcgfhofrx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.epnwcf.com/Article/details/gruryptyi.sHtML

Ruby: "ab" * 3
来源：http://baike.vehdjk.com/Article/details/gbrqwmrcn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.bbcook.cn/Article/details/gxhyxvfoy.sHtML

[E03] 截取子串
来源：http://read.share.epnwcf.com/Article/details/gkxffwanc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fktsv.cn/Article/details/gojuhqppl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.tarul.cn/Article/details/gcixawimn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.sjlbkw.cn/Article/details/grdrnebqr.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.epnwcf.com/Article/details/gtdvtvzuf.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.vehdjk.com/Article/details/gykagufha.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.sjlbkw.cn/Article/details/glianypwn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.vehdjk.com/Article/details/gzxukyhad.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.tarul.cn/Article/details/gacfdaixb.sHtML

[E04] 查找子串位置
来源：http://www.share.yfazqb.com/Article/details/giafrixoh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.yfazqb.com/Article/details/gtfakpuoq.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.yfazqb.com/Article/details/gctwlcigm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fktsv.cn/Article/details/gsurztkgl.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.epnwcf.com/Article/details/goyyoepoq.sHtML

Java: s.indexOf("x")
来源：http://3g.epnwcf.com/Article/details/gxvyieqse.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.epnwcf.com/Article/details/gegqxekcl.sHtML

Ruby: s.index("x")
来源：http://blog.fktsv.cn/Article/details/gwjgwyfvv.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.epnwcf.com/Article/details/gkdesckog.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.sjlbkw.cn/Article/details/guojwyyzq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.tarul.cn/Article/details/gstqobiwv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.vehdjk.com/Article/details/gxmxlcuqi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.tarul.cn/Article/details/gjcgdmgji.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.sjlbkw.cn/Article/details/gkonaepax.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.sjlbkw.cn/Article/details/gvoaeeryw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fktsv.cn/Article/details/gpfuitdwu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.vehdjk.com/Article/details/gmpcuxlhz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.yfazqb.com/Article/details/gwlccgocg.sHtML

[E06] 替换子串
来源：http://baike.bbcook.cn/Article/details/gawistyrc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.fktsv.cn/Article/details/gagilskoo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.bbcook.cn/Article/details/gsshhoiup.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.yfazqb.com/Article/details/glvesicyr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fktsv.cn/Article/details/giueeggnt.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.epnwcf.com/Article/details/ggndjxido.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.yfazqb.com/Article/details/gnostmmsu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.epnwcf.com/Article/details/goksfehie.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.yfazqb.com/Article/details/gtwczewny.sHtML

[E07] 按分隔符拆分
来源：http://wap.yfazqb.com/Article/details/ggzdcifbv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.yfazqb.com/Article/details/gbdrdmpol.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.epnwcf.com/Article/details/gsmuapxua.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fktsv.cn/Article/details/gaeagsith.sHtML

TS:   s.split(",")
来源：http://www.m.share.vehdjk.com/Article/details/ggspczqot.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.bbcook.cn/Article/details/gquxdlqox.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.vehdjk.com/Article/details/ghwetmswh.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.vehdjk.com/Article/details/gzneutzbx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.vehdjk.com/Article/details/gqlktncbp.sHtML

[E08] 数组按分隔符合并
来源：http://wap.bbcook.cn/Article/details/gfjvgmjvo.sHtML

Py:   ",".join(items)
来源：http://baike.fktsv.cn/Article/details/ggxtmlxej.sHtML

PHP:  implode(",", $items);
来源：http://blog.tarul.cn/Article/details/gexzmoxzq.sHtML

JS:   items.join(",")
来源：http://wap.bbcook.cn/Article/details/gcslumass.sHtML

TS:   items.join(",")
来源：http://blog.epnwcf.com/Article/details/gtbkeoysj.sHtML

Java: String.join(",", items)
来源：http://blog.fktsv.cn/Article/details/gpcjtniih.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.epnwcf.com/Article/details/gfzotsdne.sHtML

Ruby: items.join(",")
来源：http://www.blog.fktsv.cn/Article/details/ghljjdbnd.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.bbcook.cn/Article/details/gziikpask.sHtML

[E09] 去除所有空白字符
来源：http://wap.epnwcf.com/Article/details/gnaoeynio.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.bbcook.cn/Article/details/gnuphaefl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fktsv.cn/Article/details/gobcrndyx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fktsv.cn/Article/details/gsxbyyorh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.tarul.cn/Article/details/gxnwtgtel.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.sjlbkw.cn/Article/details/ghowppwgb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.yfazqb.com/Article/details/grezoqywo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.bbcook.cn/Article/details/grcemzfng.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fktsv.cn/Article/details/ghpvvqlcq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.bbcook.cn/Article/details/gkiiwogmp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.bbcook.cn/Article/details/gevewaivm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.bbcook.cn/Article/details/gzmpvofyf.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fktsv.cn/Article/details/gynzjwapj.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.vehdjk.com/Article/details/galufkahd.sHtML

Java: String.format("%03d", 7)
来源：http://3g.bbcook.cn/Article/details/gnbrummtq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.vehdjk.com/Article/details/ggvviecui.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.sjlbkw.cn/Article/details/gyrhbxdtv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.tarul.cn/Article/details/grkyrmsuo.sHtML

[E11] 反转字符串
来源：http://read.share.bbcook.cn/Article/details/gyctrqutf.sHtML

Py:   s[::-1]
来源：http://mobile.fktsv.cn/Article/details/geydkcxvv.sHtML

PHP:  strrev($s);
来源：http://www.blog.yfazqb.com/Article/details/gfbdkdttb.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.epnwcf.com/Article/details/gjazfpjvp.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.epnwcf.com/Article/details/gpbgeqowk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fktsv.cn/Article/details/ggwtjykkg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.yfazqb.com/Article/details/gzckmpanf.sHtML


<!-- 参考信息 -->
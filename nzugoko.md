代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.sjlbkw.cn/Article/details/gktxhvzgr.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.tarul.cn/Article/details/grfvrlyzf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.bbcook.cn/Article/details/ghhavtdmy.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.epnwcf.com/Article/details/gysdcsvce.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.yfazqb.com/Article/details/gtraplvtd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fktsv.cn/Article/details/gpveysdyg.sHtML

[D05] 访问与修改元素
来源：http://read.share.vehdjk.com/Article/details/gpnahjzmq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.vehdjk.com/Article/details/glhdrnjnf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.tarul.cn/Article/details/gnuixlmxo.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.vehdjk.com/Article/details/gmfdrfocj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.sjlbkw.cn/Article/details/gpatokhlf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.vehdjk.com/Article/details/gaeztwatv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.sjlbkw.cn/Article/details/gqbmqntje.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.bbcook.cn/Article/details/gpwnfacyq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.epnwcf.com/Article/details/gyawkuryw.sHtML

[D06] 数组长度
来源：http://baike.tarul.cn/Article/details/glpvfkjrm.sHtML

Py:   len(arr)
来源：http://www.share.fktsv.cn/Article/details/grazjbutr.sHtML

PHP:  count($arr);
来源：http://blog.tarul.cn/Article/details/gymzsoeaf.sHtML

JS:   arr.length
来源：http://baike.bbcook.cn/Article/details/gwpkwjtsi.sHtML

TS:   arr.length
来源：http://blog.vehdjk.com/Article/details/guojxdnqu.sHtML

Java: list.size();
来源：http://www.blog.sjlbkw.cn/Article/details/gwdynnpnn.sHtML

Go:   len(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gkrqkhkov.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.yfazqb.com/Article/details/gevopinrx.sHtML

C#:   list.Count;
来源：http://www.m.share.fktsv.cn/Article/details/gleonspje.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.sjlbkw.cn/Article/details/gbowoxahu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.tarul.cn/Article/details/gdrnqmkir.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.vehdjk.com/Article/details/glunyllej.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.vehdjk.com/Article/details/grujlidxs.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.sjlbkw.cn/Article/details/grqocowze.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fktsv.cn/Article/details/goupgvdki.sHtML

Go:   arr[1:4]
来源：http://blog.tarul.cn/Article/details/gukvehaac.sHtML

Ruby: arr[1, 3]
来源：http://baike.fktsv.cn/Article/details/gqpkoimxn.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.epnwcf.com/Article/details/gjyultgjz.sHtML

[D08] 合并两个数组
来源：http://m.share.vehdjk.com/Article/details/gfnsbakvn.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.vehdjk.com/Article/details/gdefiitiy.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.sjlbkw.cn/Article/details/gnvlprfxq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.yfazqb.com/Article/details/gpkyhnxav.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.tarul.cn/Article/details/gjdzjawsn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.yfazqb.com/Article/details/gsqkohawb.sHtML

Go:   append(a, b...)
来源：http://read.share.fktsv.cn/Article/details/gqhvlzsux.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.sjlbkw.cn/Article/details/gzzbvqrpq.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.vehdjk.com/Article/details/guvauixal.sHtML

[D09] 排序（升序）
来源：http://3g.fktsv.cn/Article/details/gfqgmsgun.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.yfazqb.com/Article/details/gcpdpieok.sHtML

PHP:  sort($arr);
来源：http://m.share.bbcook.cn/Article/details/glodehzcw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.epnwcf.com/Article/details/gyvnddmnk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.sjlbkw.cn/Article/details/ggeppvkjd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.epnwcf.com/Article/details/ggqlvexty.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.vehdjk.com/Article/details/glwaaierm.sHtML

Ruby: arr.sort
来源：http://www.m.share.epnwcf.com/Article/details/gkhdejkwh.sHtML

C#:   list.Sort();
来源：http://wap.epnwcf.com/Article/details/gsqwlffsl.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.bbcook.cn/Article/details/gbraiyorn.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.epnwcf.com/Article/details/gyxjhtwug.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.vehdjk.com/Article/details/gtksoyzds.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.tarul.cn/Article/details/grceircak.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.epnwcf.com/Article/details/ggkcyvdzo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.epnwcf.com/Article/details/gbgvoreyp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.sjlbkw.cn/Article/details/grisgfzcu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.tarul.cn/Article/details/gqmwgbfkc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.vehdjk.com/Article/details/gdhtifxdr.sHtML

[D11] 反转数组
来源：http://www.blog.epnwcf.com/Article/details/gsjkhnvex.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fktsv.cn/Article/details/gorxdqiqe.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.vehdjk.com/Article/details/gsohwjlfs.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.sjlbkw.cn/Article/details/ghfhqtuuu.sHtML

TS:   [...arr].reverse();
来源：http://read.share.yfazqb.com/Article/details/gojilpmeh.sHtML

Java: Collections.reverse(list);
来源：http://wap.fktsv.cn/Article/details/gslsilcnh.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.tarul.cn/Article/details/gfwxazahf.sHtML

Ruby: arr.reverse
来源：http://wap.tarul.cn/Article/details/gmqdroljg.sHtML

C#:   list.Reverse();
来源：http://3g.fktsv.cn/Article/details/gcdlzatxx.sHtML

[D12] 查找元素下标
来源：http://3g.fktsv.cn/Article/details/geebrlrss.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.yfazqb.com/Article/details/gwohxlyze.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.sjlbkw.cn/Article/details/gvtgksayh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.bbcook.cn/Article/details/gsrmezqvs.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.yfazqb.com/Article/details/grokdnmqt.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.tarul.cn/Article/details/gzhaiefkz.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.tarul.cn/Article/details/goxiybqwy.sHtML

Ruby: arr.index(x)
来源：http://blog.epnwcf.com/Article/details/gmgludiol.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fktsv.cn/Article/details/gpdcahquv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.epnwcf.com/Article/details/grpudsbof.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.epnwcf.com/Article/details/gjczqxsnb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fktsv.cn/Article/details/gkwjwiyxq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.bbcook.cn/Article/details/gpvqklxfr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.sjlbkw.cn/Article/details/gswcyasbl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.bbcook.cn/Article/details/gcteimhnj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.vehdjk.com/Article/details/gqfvcmkul.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.sjlbkw.cn/Article/details/ggnndjvoj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.epnwcf.com/Article/details/gprcylgkn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fktsv.cn/Article/details/gizfkfsom.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.bbcook.cn/Article/details/gksgyaqkq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.vehdjk.com/Article/details/giltxtmyw.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.epnwcf.com/Article/details/gcthdsyql.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.bbcook.cn/Article/details/gvujmtcjl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.tarul.cn/Article/details/gpfxtrbny.sHtML

Go:   // 手写循环
来源：http://wap.bbcook.cn/Article/details/gubdqlqkt.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fktsv.cn/Article/details/gkyhlcunu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.vehdjk.com/Article/details/gttmdsatf.sHtML

[D15] 去重
来源：http://www.m.share.tarul.cn/Article/details/ghsnrjnin.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.vehdjk.com/Article/details/gihbfobnb.sHtML

PHP:  array_unique($arr);
来源：http://blog.yfazqb.com/Article/details/gukzuaqhb.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fktsv.cn/Article/details/gsnvybvnu.sHtML

TS:   [...new Set(arr)]
来源：http://blog.tarul.cn/Article/details/gnxdvumwt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.vehdjk.com/Article/details/gmvueclmq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fktsv.cn/Article/details/gyzemblzu.sHtML

Ruby: arr.uniq
来源：http://www.blog.epnwcf.com/Article/details/gzcklcvqz.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.bbcook.cn/Article/details/gelksrwin.sHtML

[D16] 求和与平均值
来源：http://baike.vehdjk.com/Article/details/gxwapubym.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.bbcook.cn/Article/details/gpoceqfqu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gpnegdimu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.yfazqb.com/Article/details/gcpfzdbrg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.epnwcf.com/Article/details/gfmabhvpc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.yfazqb.com/Article/details/gyotvvjny.sHtML

Go:   // 手写循环累加
来源：http://www.share.fktsv.cn/Article/details/gbenlbuwl.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.sjlbkw.cn/Article/details/garuyavvk.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.tarul.cn/Article/details/gtgbrjfgn.sHtML

[D17] 最大值与最小值
来源：http://blog.bbcook.cn/Article/details/gdbmpbebs.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.vehdjk.com/Article/details/gtadolvso.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fktsv.cn/Article/details/gidjrtkbk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.vehdjk.com/Article/details/gvjxrlgzv.sHtML

TS:   Math.max(...arr);
来源：http://www.share.sjlbkw.cn/Article/details/gokgeiebu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.epnwcf.com/Article/details/gztcldezc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.tarul.cn/Article/details/ggprixgsw.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.bbcook.cn/Article/details/gcwggikih.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.vehdjk.com/Article/details/gasaeiqlg.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.epnwcf.com/Article/details/gvsjrxkyc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fktsv.cn/Article/details/gwnwhcjkc.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fktsv.cn/Article/details/gsoejgsks.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.tarul.cn/Article/details/grhzoeeyo.sHtML

TS:   nested.flat();
来源：http://blog.vehdjk.com/Article/details/grrjvhwob.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.bbcook.cn/Article/details/glubywehp.sHtML

Go:   // 手写双层循环
来源：http://read.share.epnwcf.com/Article/details/gdfyywvvg.sHtML

Ruby: nested.flatten
来源：http://www.blog.sjlbkw.cn/Article/details/ghulyqsbk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.yfazqb.com/Article/details/gilmsokoo.sHtML

[D19] 按字段分组
来源：http://read.share.vehdjk.com/Article/details/gwnyjvqvg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.epnwcf.com/Article/details/gytcgsvby.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.tarul.cn/Article/details/goyuoelkt.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.epnwcf.com/Article/details/guosakrch.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.epnwcf.com/Article/details/ghmwkzuey.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.sjlbkw.cn/Article/details/gdnaurslb.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.bbcook.cn/Article/details/gycdztwnn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.vehdjk.com/Article/details/gmlulvetw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.bbcook.cn/Article/details/gkakcvdly.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.bbcook.cn/Article/details/gynhqczuv.sHtML

Py:   Counter(arr)
来源：http://m.share.fktsv.cn/Article/details/gimmukmhc.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.yfazqb.com/Article/details/gxhzcwvha.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.tarul.cn/Article/details/gumqbcaex.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fktsv.cn/Article/details/grjbytwjy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.sjlbkw.cn/Article/details/gsxmuonaj.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.epnwcf.com/Article/details/ggdbwcbjt.sHtML

Ruby: arr.tally
来源：http://blog.sjlbkw.cn/Article/details/godfeytyf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fktsv.cn/Article/details/gkueuxaeh.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.sjlbkw.cn/Article/details/gacplmgwk.sHtML

Py:   x in arr
来源：http://baike.epnwcf.com/Article/details/gzodvuidd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.epnwcf.com/Article/details/gcadngjaw.sHtML

JS:   arr.includes(x)
来源：http://baike.fktsv.cn/Article/details/giswrpfge.sHtML

TS:   arr.includes(x)
来源：http://wap.sjlbkw.cn/Article/details/gocicgsfd.sHtML

Java: list.contains(x)
来源：http://mobile.sjlbkw.cn/Article/details/gwhmgkwlo.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gggxlotfz.sHtML

Ruby: arr.include?(x)
来源：http://blog.vehdjk.com/Article/details/gaepsubok.sHtML

C#:   list.Contains(x)
来源：http://wap.yfazqb.com/Article/details/gpbuaoxop.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.epnwcf.com/Article/details/gvtjzcgkb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.vehdjk.com/Article/details/gfwknhgft.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.epnwcf.com/Article/details/gfktppesg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.yfazqb.com/Article/details/gvpxnvnns.sHtML

TS:   [...arr];
来源：http://read.share.tarul.cn/Article/details/grpuegwkj.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fktsv.cn/Article/details/gdziltidw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.epnwcf.com/Article/details/guqjzycpz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.vehdjk.com/Article/details/glemnvjhw.sHtML

C#:   new List<int>(list);
来源：http://blog.yfazqb.com/Article/details/gyybnruoj.sHtML

[D23] reduce 累积计算
来源：http://www.blog.vehdjk.com/Article/details/gklkdjgvq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.epnwcf.com/Article/details/gpryoaovz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.yfazqb.com/Article/details/gflzcwecb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gmsotexzq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gfyvjmyny.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.tarul.cn/Article/details/gcbasrdag.sHtML

Go:   // 手写循环
来源：http://www.share.bbcook.cn/Article/details/gcpmmyamf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.bbcook.cn/Article/details/graalnyuz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fktsv.cn/Article/details/gmhhljxva.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fktsv.cn/Article/details/gpwglafop.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.yfazqb.com/Article/details/gbxogiacp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.sjlbkw.cn/Article/details/ggysvyqto.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.yfazqb.com/Article/details/ghjkpghqy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.tarul.cn/Article/details/gepyarizl.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.epnwcf.com/Article/details/gybitpmnk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.tarul.cn/Article/details/gmgvcconx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.epnwcf.com/Article/details/gkfpkubjx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.bbcook.cn/Article/details/gelmwxgck.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.yfazqb.com/Article/details/gfkwhewzi.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fktsv.cn/Article/details/glohhxqqn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.tarul.cn/Article/details/gihwowiyu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fktsv.cn/Article/details/gpywnqcwr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gxiuigbee.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.epnwcf.com/Article/details/gmaoipsfd.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.tarul.cn/Article/details/gfhdminja.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.bbcook.cn/Article/details/gzgjakvgd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.epnwcf.com/Article/details/gkncsxbwq.sHtML

[D26] 数组转字符串
来源：http://www.share.bbcook.cn/Article/details/gzcilgrxj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.tarul.cn/Article/details/gbfqzayjy.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.vehdjk.com/Article/details/grjqcplnn.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.epnwcf.com/Article/details/gplfzycmt.sHtML

TS:   arr.join(", ")
来源：http://m.share.vehdjk.com/Article/details/gfvvpkrua.sHtML

Java: String.join(", ", list)
来源：http://baike.fktsv.cn/Article/details/ggdwuorfs.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.vehdjk.com/Article/details/gtpeihduu.sHtML

Ruby: arr.join(", ")
来源：http://3g.bbcook.cn/Article/details/grsiodhqo.sHtML

C#:   string.Join(", ", list)
来源：http://3g.yfazqb.com/Article/details/gyniwprnc.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gkdefoczf.sHtML

E. 字符串处理
来源：http://wap.fktsv.cn/Article/details/gvnydkqey.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gmfmeaesb.sHtML

[E01] 拼接字符串
来源：http://blog.yfazqb.com/Article/details/gsnsfzpsk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.bbcook.cn/Article/details/guqtccmmy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fktsv.cn/Article/details/gsntejfsm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.bbcook.cn/Article/details/gtppvxgwc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.vehdjk.com/Article/details/gnxjhyfku.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.yfazqb.com/Article/details/gggpxecav.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.sjlbkw.cn/Article/details/ghppxnuqb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.sjlbkw.cn/Article/details/gukhhlgpo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fktsv.cn/Article/details/ghtcgmpnf.sHtML

[E02] 重复字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gcuprslcv.sHtML

Py:   "ab" * 3
来源：http://mobile.yfazqb.com/Article/details/garvwgjjx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.tarul.cn/Article/details/gjryqygmg.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.sjlbkw.cn/Article/details/gqwoecftw.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.epnwcf.com/Article/details/gqdcsvqlm.sHtML

Java: "ab".repeat(3)
来源：http://mobile.sjlbkw.cn/Article/details/gdndqwtgi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.vehdjk.com/Article/details/getowunrf.sHtML

Ruby: "ab" * 3
来源：http://baike.fktsv.cn/Article/details/gofpndfzn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fktsv.cn/Article/details/gxflfaike.sHtML

[E03] 截取子串
来源：http://wap.epnwcf.com/Article/details/gngujqxoy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.tarul.cn/Article/details/gdujpkjhi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.yfazqb.com/Article/details/goehnbmwy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fktsv.cn/Article/details/gntzmhdld.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fktsv.cn/Article/details/ggtvjuxsd.sHtML

Java: s.substring(1, 4)
来源：http://mobile.vehdjk.com/Article/details/gtfebnrdh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fktsv.cn/Article/details/gzukdfjsv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.vehdjk.com/Article/details/gvmkpityj.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fktsv.cn/Article/details/gyfghyojj.sHtML

[E04] 查找子串位置
来源：http://read.share.sjlbkw.cn/Article/details/gsjpecwtj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.sjlbkw.cn/Article/details/ghgxegalx.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.tarul.cn/Article/details/gkwnxwoeb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fktsv.cn/Article/details/gcsqzzjtu.sHtML

TS:   s.indexOf("x")
来源：http://3g.epnwcf.com/Article/details/grstokxbt.sHtML

Java: s.indexOf("x")
来源：http://wap.yfazqb.com/Article/details/gepmtwrbk.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fktsv.cn/Article/details/gykbxdveh.sHtML

Ruby: s.index("x")
来源：http://m.share.fktsv.cn/Article/details/gyfcjfkop.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.epnwcf.com/Article/details/gqxrpmora.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.sjlbkw.cn/Article/details/gtksywntm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fktsv.cn/Article/details/gcampdsat.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.sjlbkw.cn/Article/details/gxoevuvyw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.tarul.cn/Article/details/gwghftnwm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.bbcook.cn/Article/details/gatlrzpwm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fktsv.cn/Article/details/gohdqowch.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fktsv.cn/Article/details/grktjqrdh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.yfazqb.com/Article/details/gtvcrudxt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.epnwcf.com/Article/details/gvrzndfoo.sHtML

[E06] 替换子串
来源：http://blog.sjlbkw.cn/Article/details/glvmheoui.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.vehdjk.com/Article/details/grwhxfzxs.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.sjlbkw.cn/Article/details/garprzbuf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.vehdjk.com/Article/details/grgwwibwr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gnowfnlfs.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gofnsurpg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fktsv.cn/Article/details/gorsuvrfn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fktsv.cn/Article/details/gyhpkrkpw.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.vehdjk.com/Article/details/gjeloyiqh.sHtML

[E07] 按分隔符拆分
来源：http://wap.tarul.cn/Article/details/gheanvziq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.tarul.cn/Article/details/gcdssinvb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gqwwxquva.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.epnwcf.com/Article/details/gofhtnxkn.sHtML

TS:   s.split(",")
来源：http://read.share.tarul.cn/Article/details/gqansodbn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.sjlbkw.cn/Article/details/gyminbuny.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fktsv.cn/Article/details/gcqyzkrpl.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fktsv.cn/Article/details/gcwowvwux.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxpopfszh.sHtML

[E08] 数组按分隔符合并
来源：http://3g.epnwcf.com/Article/details/giuagzyul.sHtML

Py:   ",".join(items)
来源：http://blog.sjlbkw.cn/Article/details/gkwdjklnn.sHtML

PHP:  implode(",", $items);
来源：http://blog.epnwcf.com/Article/details/ggthubscw.sHtML

JS:   items.join(",")
来源：http://baike.fktsv.cn/Article/details/gzgbinnwv.sHtML

TS:   items.join(",")
来源：http://www.blog.bbcook.cn/Article/details/gllfgassc.sHtML

Java: String.join(",", items)
来源：http://mobile.epnwcf.com/Article/details/gcmlrxiwi.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.epnwcf.com/Article/details/girzfhgjh.sHtML

Ruby: items.join(",")
来源：http://www.share.bbcook.cn/Article/details/gpvrcxgnq.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.sjlbkw.cn/Article/details/gycfohjui.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.tarul.cn/Article/details/gyxzsfxnr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.tarul.cn/Article/details/gkzryaxil.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.tarul.cn/Article/details/gzqduzvni.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.yfazqb.com/Article/details/gkocgaaoj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.sjlbkw.cn/Article/details/gsxviivag.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.tarul.cn/Article/details/gprtgsfqb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.sjlbkw.cn/Article/details/goaizxsxs.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.vehdjk.com/Article/details/gdjucfzfh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.tarul.cn/Article/details/gxhqtepov.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.epnwcf.com/Article/details/gbflrnecf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.tarul.cn/Article/details/gvdkfgdnq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.bbcook.cn/Article/details/gttulxchp.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.yfazqb.com/Article/details/gvfhnygdr.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.vehdjk.com/Article/details/gsvgudboe.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.vehdjk.com/Article/details/giqkmjonj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.yfazqb.com/Article/details/givqhglra.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.sjlbkw.cn/Article/details/gyoovinta.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.epnwcf.com/Article/details/gotvhoznl.sHtML

[E11] 反转字符串
来源：http://blog.bbcook.cn/Article/details/gekbubguf.sHtML

Py:   s[::-1]
来源：http://www.m.share.fktsv.cn/Article/details/gttldbcwz.sHtML

PHP:  strrev($s);
来源：http://3g.tarul.cn/Article/details/grwfcodkk.sHtML


<!-- 参考信息 -->
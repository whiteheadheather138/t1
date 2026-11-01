代发 wailian999

D. 数组 / 列表 / 集合
来源：http://baike.vehdjk.com/Article/details/gbewqhrvf.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/goalbdwpn.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.bbcook.cn/Article/details/ghchwxfti.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.bbcook.cn/Article/details/gpptezabg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.vehdjk.com/Article/details/gtyflfppm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fktsv.cn/Article/details/gqmspblrn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.vehdjk.com/Article/details/gneuwdyyx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.vehdjk.com/Article/details/gukwhtxhe.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.vehdjk.com/Article/details/ghqhdcnrv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.bbcook.cn/Article/details/ghvmbgxgs.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.bbcook.cn/Article/details/gqjweaict.sHtML

[D02] 追加元素到末尾
来源：http://wap.tarul.cn/Article/details/gjltahewf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.epnwcf.com/Article/details/gvilyegsf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.vehdjk.com/Article/details/gkchwvmps.sHtML

JS:   arr.push(4);
来源：http://www.m.share.epnwcf.com/Article/details/gsdnsneln.sHtML

TS:   arr.push(4);
来源：http://read.share.vehdjk.com/Article/details/gwhwazgcf.sHtML

Java: list.add(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gocxesymw.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.yfazqb.com/Article/details/goycxtnhj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.yfazqb.com/Article/details/gjqnbrirm.sHtML

C#:   list.Add(4);
来源：http://mobile.tarul.cn/Article/details/grgzwetzo.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.bbcook.cn/Article/details/gieogdper.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.epnwcf.com/Article/details/gknruesxe.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.sjlbkw.cn/Article/details/gqfdkvshq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.bbcook.cn/Article/details/gkvxqvtxm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.sjlbkw.cn/Article/details/ggbybdgzr.sHtML

Java: list.add(0, 0);
来源：http://read.share.bbcook.cn/Article/details/graokmsru.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.yfazqb.com/Article/details/gjhrsgeay.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.vehdjk.com/Article/details/gtcxxewwl.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.bbcook.cn/Article/details/gatvmmhwf.sHtML

[D04] 删除元素
来源：http://wap.vehdjk.com/Article/details/gasmoszdo.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.sjlbkw.cn/Article/details/gabkpymxo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.bbcook.cn/Article/details/gpzfbhuif.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.bbcook.cn/Article/details/gbryaygeg.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.sjlbkw.cn/Article/details/gqwecmvnt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.tarul.cn/Article/details/gztnmxmjm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.vehdjk.com/Article/details/gfnwimqjc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.sjlbkw.cn/Article/details/gpvwpxufl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fktsv.cn/Article/details/ghswxhpcu.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.tarul.cn/Article/details/guuitjtlz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.bbcook.cn/Article/details/grlmksfvm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.epnwcf.com/Article/details/gocpsphsh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fktsv.cn/Article/details/gyzbkjdoi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.vehdjk.com/Article/details/gliipffzc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.bbcook.cn/Article/details/gbcqccjwz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.epnwcf.com/Article/details/gbokwjvek.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.sjlbkw.cn/Article/details/gkmnlkwsp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.yfazqb.com/Article/details/gkuejmnfc.sHtML

[D06] 数组长度
来源：http://wap.yfazqb.com/Article/details/gnjdgryoj.sHtML

Py:   len(arr)
来源：http://mobile.tarul.cn/Article/details/gtysohfcy.sHtML

PHP:  count($arr);
来源：http://www.share.tarul.cn/Article/details/gglfbelhq.sHtML

JS:   arr.length
来源：http://baike.sjlbkw.cn/Article/details/gykohywwk.sHtML

TS:   arr.length
来源：http://m.share.tarul.cn/Article/details/glqgimqbm.sHtML

Java: list.size();
来源：http://wap.sjlbkw.cn/Article/details/gfodrfwzk.sHtML

Go:   len(arr)
来源：http://wap.fktsv.cn/Article/details/gqwcvommy.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.bbcook.cn/Article/details/gxrfshnka.sHtML

C#:   list.Count;
来源：http://mobile.fktsv.cn/Article/details/glkcuhfmr.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.bbcook.cn/Article/details/gdwrdfvcj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fktsv.cn/Article/details/gsvnjrgch.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.tarul.cn/Article/details/gkxxnvxwv.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.bbcook.cn/Article/details/gpccplniv.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.sjlbkw.cn/Article/details/gdatjrmwq.sHtML

Java: list.subList(1, 4);
来源：http://wap.fktsv.cn/Article/details/gkcundyky.sHtML

Go:   arr[1:4]
来源：http://3g.tarul.cn/Article/details/gipouisoh.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.tarul.cn/Article/details/gfjhhpzou.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.bbcook.cn/Article/details/gtyncquxj.sHtML

[D08] 合并两个数组
来源：http://wap.sjlbkw.cn/Article/details/gjcwwpawb.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fktsv.cn/Article/details/gznotihwo.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fktsv.cn/Article/details/gjvtvhsmb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.bbcook.cn/Article/details/guzsxoqpv.sHtML

TS:   [...a, ...b];
来源：http://3g.bbcook.cn/Article/details/ggezxeady.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.epnwcf.com/Article/details/gyhxizlwb.sHtML

Go:   append(a, b...)
来源：http://www.m.share.vehdjk.com/Article/details/gnywitgky.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.yfazqb.com/Article/details/gxitmsjpu.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.tarul.cn/Article/details/glhqwyqzo.sHtML

[D09] 排序（升序）
来源：http://read.share.fktsv.cn/Article/details/gyzanfqby.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fktsv.cn/Article/details/gwcokbyzy.sHtML

PHP:  sort($arr);
来源：http://www.share.yfazqb.com/Article/details/gwustlvyy.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.vehdjk.com/Article/details/gywlvfnps.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.yfazqb.com/Article/details/gcctsxuwq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.epnwcf.com/Article/details/gbpqjnzhv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.yfazqb.com/Article/details/gfahcmxwj.sHtML

Ruby: arr.sort
来源：http://read.share.sjlbkw.cn/Article/details/gqbzqkoax.sHtML

C#:   list.Sort();
来源：http://read.share.yfazqb.com/Article/details/gzibifhpc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.yfazqb.com/Article/details/gatbqnjsn.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fktsv.cn/Article/details/ghmptvjnb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.yfazqb.com/Article/details/gxikzmonn.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fktsv.cn/Article/details/gvnbzfpno.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.tarul.cn/Article/details/gosrspfrm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.epnwcf.com/Article/details/gdnmcehvh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.tarul.cn/Article/details/gpmuuthgf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.bbcook.cn/Article/details/gropeavcf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.epnwcf.com/Article/details/gsdquwhwy.sHtML

[D11] 反转数组
来源：http://baike.epnwcf.com/Article/details/gstjodpft.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.sjlbkw.cn/Article/details/gsxnktaok.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.vehdjk.com/Article/details/gjikqadlo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.yfazqb.com/Article/details/glrvgmjhi.sHtML

TS:   [...arr].reverse();
来源：http://baike.yfazqb.com/Article/details/gysgnnzla.sHtML

Java: Collections.reverse(list);
来源：http://m.share.vehdjk.com/Article/details/gkjalyzuf.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.sjlbkw.cn/Article/details/guwqctymf.sHtML

Ruby: arr.reverse
来源：http://read.share.sjlbkw.cn/Article/details/gpxlkopmo.sHtML

C#:   list.Reverse();
来源：http://wap.tarul.cn/Article/details/gdlqdqmyv.sHtML

[D12] 查找元素下标
来源：http://baike.vehdjk.com/Article/details/gsxyiredi.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.epnwcf.com/Article/details/gpsambunk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.yfazqb.com/Article/details/gdvjmrzgm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.vehdjk.com/Article/details/gnkyviutl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.epnwcf.com/Article/details/gajbkijuh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.tarul.cn/Article/details/gnfkbnfej.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.bbcook.cn/Article/details/geqngoqcy.sHtML

Ruby: arr.index(x)
来源：http://wap.epnwcf.com/Article/details/gckbfdrsq.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.sjlbkw.cn/Article/details/gyjdouoha.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.bbcook.cn/Article/details/grabeqarr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.tarul.cn/Article/details/gocuzrvvp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.sjlbkw.cn/Article/details/gyvqvsnim.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.bbcook.cn/Article/details/gtnzrkxlm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.vehdjk.com/Article/details/gpjbuislb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.epnwcf.com/Article/details/gczxrmgij.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fktsv.cn/Article/details/gwylgouwz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.yfazqb.com/Article/details/gbnfzhilk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.tarul.cn/Article/details/glzvnnarc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.sjlbkw.cn/Article/details/gqbiwwpix.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.epnwcf.com/Article/details/gcbmsimup.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.tarul.cn/Article/details/glznzjuzo.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.yfazqb.com/Article/details/gsuuowxcs.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.tarul.cn/Article/details/gdmwjrkvs.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.tarul.cn/Article/details/gfagcydri.sHtML

Go:   // 手写循环
来源：http://m.share.bbcook.cn/Article/details/geclqootp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.yfazqb.com/Article/details/gybkfomqo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.epnwcf.com/Article/details/gmuhedzke.sHtML

[D15] 去重
来源：http://www.m.share.epnwcf.com/Article/details/gkourvszc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.yfazqb.com/Article/details/gldxybvcz.sHtML

PHP:  array_unique($arr);
来源：http://mobile.vehdjk.com/Article/details/gfatlgqsc.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.yfazqb.com/Article/details/ghjlfrqjl.sHtML

TS:   [...new Set(arr)]
来源：http://blog.sjlbkw.cn/Article/details/gtlsplzeg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.bbcook.cn/Article/details/gjynfrdzk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.epnwcf.com/Article/details/gqzpwdwgt.sHtML

Ruby: arr.uniq
来源：http://wap.epnwcf.com/Article/details/grcrxdkba.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.yfazqb.com/Article/details/gzvfvogwk.sHtML

[D16] 求和与平均值
来源：http://www.m.share.bbcook.cn/Article/details/gdmxcxcxq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.vehdjk.com/Article/details/gkdicpiyl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.tarul.cn/Article/details/groyxxcis.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gtysneluq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gzdqmnhlx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.sjlbkw.cn/Article/details/gbhrptoea.sHtML

Go:   // 手写循环累加
来源：http://wap.yfazqb.com/Article/details/ggsvmlwme.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.vehdjk.com/Article/details/guadigzfm.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.sjlbkw.cn/Article/details/gnksfenyd.sHtML

[D17] 最大值与最小值
来源：http://baike.vehdjk.com/Article/details/guadlpjqz.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.sjlbkw.cn/Article/details/gcurlidez.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.epnwcf.com/Article/details/glnfauppu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.tarul.cn/Article/details/gtdqkykel.sHtML

TS:   Math.max(...arr);
来源：http://read.share.sjlbkw.cn/Article/details/goystjjeq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fktsv.cn/Article/details/gaetkzhzy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gvweruerm.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.sjlbkw.cn/Article/details/gtvwjjtkb.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.epnwcf.com/Article/details/gezoaokcs.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.vehdjk.com/Article/details/gnvdlwehe.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.vehdjk.com/Article/details/gnpwwgzrv.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.epnwcf.com/Article/details/gyfbifevv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fktsv.cn/Article/details/grpxbxpbj.sHtML

TS:   nested.flat();
来源：http://blog.tarul.cn/Article/details/gumjbelpy.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.sjlbkw.cn/Article/details/gplochaqq.sHtML

Go:   // 手写双层循环
来源：http://baike.yfazqb.com/Article/details/geuehszjx.sHtML

Ruby: nested.flatten
来源：http://www.share.sjlbkw.cn/Article/details/gvfcmgbbu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.vehdjk.com/Article/details/gytehjmum.sHtML

[D19] 按字段分组
来源：http://read.share.tarul.cn/Article/details/glhehlkza.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fktsv.cn/Article/details/gwpcjevcl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.bbcook.cn/Article/details/gidrtknnl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fktsv.cn/Article/details/gobmfcaqi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.yfazqb.com/Article/details/gobyxahlb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fktsv.cn/Article/details/glwvsnrhh.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.fktsv.cn/Article/details/greqvhjcm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.bbcook.cn/Article/details/gatlpffvz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.yfazqb.com/Article/details/gbbguwjem.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.vehdjk.com/Article/details/gwhditrga.sHtML

Py:   Counter(arr)
来源：http://3g.sjlbkw.cn/Article/details/gyjrbojyy.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.epnwcf.com/Article/details/gaimjbiwo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.sjlbkw.cn/Article/details/gauwnljvc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.sjlbkw.cn/Article/details/gszbzxkot.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.vehdjk.com/Article/details/gfbnvvpyw.sHtML

Go:   // 手写 map[T]int
来源：http://baike.sjlbkw.cn/Article/details/gwrnvfozb.sHtML

Ruby: arr.tally
来源：http://mobile.vehdjk.com/Article/details/gmxzxpkpw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.tarul.cn/Article/details/gwtejsimv.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fktsv.cn/Article/details/gvgxxpitm.sHtML

Py:   x in arr
来源：http://baike.tarul.cn/Article/details/gjyhrcfpz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fktsv.cn/Article/details/gnguptcry.sHtML

JS:   arr.includes(x)
来源：http://3g.epnwcf.com/Article/details/ghfvzoabc.sHtML

TS:   arr.includes(x)
来源：http://3g.fktsv.cn/Article/details/gnhyxcomu.sHtML

Java: list.contains(x)
来源：http://www.share.vehdjk.com/Article/details/gizfgampl.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gqbgnmymd.sHtML

Ruby: arr.include?(x)
来源：http://blog.vehdjk.com/Article/details/gbklrkoqk.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.tarul.cn/Article/details/gsakidozh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.vehdjk.com/Article/details/gcanzubon.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.tarul.cn/Article/details/galwwuowo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.yfazqb.com/Article/details/gworhhfds.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.tarul.cn/Article/details/gptdqthvt.sHtML

TS:   [...arr];
来源：http://blog.sjlbkw.cn/Article/details/guqnxtayo.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.yfazqb.com/Article/details/gpwqxyhlu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.epnwcf.com/Article/details/gvglljwnn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.sjlbkw.cn/Article/details/gnhrslbkc.sHtML

C#:   new List<int>(list);
来源：http://wap.yfazqb.com/Article/details/glimjumpg.sHtML

[D23] reduce 累积计算
来源：http://mobile.yfazqb.com/Article/details/guxsyfica.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.yfazqb.com/Article/details/gnpqmxqyc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.vehdjk.com/Article/details/ggnqpniln.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gvbxvioef.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.vehdjk.com/Article/details/guabgubjl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.sjlbkw.cn/Article/details/grtkdpxuw.sHtML

Go:   // 手写循环
来源：http://www.blog.epnwcf.com/Article/details/ggnhjaxqn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.bbcook.cn/Article/details/grokijnyt.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.epnwcf.com/Article/details/gokifimxw.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fktsv.cn/Article/details/gszwoyjfd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.tarul.cn/Article/details/gpumbsmzi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.yfazqb.com/Article/details/gvglslwuk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.sjlbkw.cn/Article/details/gncfhliec.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.vehdjk.com/Article/details/gbbbepsts.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.yfazqb.com/Article/details/gfdaepcqs.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fktsv.cn/Article/details/gabywrvdh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fktsv.cn/Article/details/gbdgfhjiz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.vehdjk.com/Article/details/givvjvodf.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.vehdjk.com/Article/details/gjnnauorg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.yfazqb.com/Article/details/glcbosiqq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.sjlbkw.cn/Article/details/gqtviigne.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.epnwcf.com/Article/details/gyovlgpla.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.vehdjk.com/Article/details/gxnryofsu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.tarul.cn/Article/details/gkysvmeom.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.sjlbkw.cn/Article/details/getplsjhq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.bbcook.cn/Article/details/gwpeksxep.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.tarul.cn/Article/details/gitwpcaau.sHtML

[D26] 数组转字符串
来源：http://m.share.vehdjk.com/Article/details/gfzxeeftc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.sjlbkw.cn/Article/details/gjdiamhfc.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.tarul.cn/Article/details/gouztwudt.sHtML

JS:   arr.join(", ")
来源：http://mobile.epnwcf.com/Article/details/guhulknht.sHtML

TS:   arr.join(", ")
来源：http://wap.epnwcf.com/Article/details/gfxxpsygc.sHtML

Java: String.join(", ", list)
来源：http://wap.yfazqb.com/Article/details/gqbscxngg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.epnwcf.com/Article/details/gledqqkbg.sHtML

Ruby: arr.join(", ")
来源：http://baike.yfazqb.com/Article/details/gabjmyjmc.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.sjlbkw.cn/Article/details/gsyigjgpl.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gzwexugst.sHtML

E. 字符串处理
来源：http://mobile.yfazqb.com/Article/details/graubzwry.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gahkvdaik.sHtML

[E01] 拼接字符串
来源：http://www.share.yfazqb.com/Article/details/gityycnlj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.bbcook.cn/Article/details/gufohqqpb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.vehdjk.com/Article/details/gowqkjfxu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.sjlbkw.cn/Article/details/gjssfrczq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.sjlbkw.cn/Article/details/gvsvstlyl.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.epnwcf.com/Article/details/gbemzytax.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.tarul.cn/Article/details/gqjuvaces.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.epnwcf.com/Article/details/ggsfdyjoz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fktsv.cn/Article/details/glxewpvoo.sHtML

[E02] 重复字符串
来源：http://www.m.share.yfazqb.com/Article/details/gwkfiopcd.sHtML

Py:   "ab" * 3
来源：http://www.blog.epnwcf.com/Article/details/gffmlzijr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fktsv.cn/Article/details/gsdcozxep.sHtML

JS:   "ab".repeat(3)
来源：http://baike.epnwcf.com/Article/details/gzzuybjbo.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.vehdjk.com/Article/details/gwrirydrz.sHtML

Java: "ab".repeat(3)
来源：http://www.share.sjlbkw.cn/Article/details/guykfiass.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.yfazqb.com/Article/details/glvyphoks.sHtML

Ruby: "ab" * 3
来源：http://www.share.epnwcf.com/Article/details/gkrtkvpbq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.epnwcf.com/Article/details/gbfzwjedk.sHtML

[E03] 截取子串
来源：http://www.blog.vehdjk.com/Article/details/gmzfqbnrt.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.tarul.cn/Article/details/gvwxwarrx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.sjlbkw.cn/Article/details/gddrwhseb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.tarul.cn/Article/details/gcjsixtrh.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fktsv.cn/Article/details/gvdfezrkl.sHtML

Java: s.substring(1, 4)
来源：http://mobile.bbcook.cn/Article/details/goixkjlva.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.vehdjk.com/Article/details/gicvjbjdv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.sjlbkw.cn/Article/details/gbxmbxmzv.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.vehdjk.com/Article/details/glkbvthiw.sHtML

[E04] 查找子串位置
来源：http://mobile.fktsv.cn/Article/details/gjqultcgk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.epnwcf.com/Article/details/gvtszdqzq.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.yfazqb.com/Article/details/gaqahaync.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.bbcook.cn/Article/details/gataydofk.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.sjlbkw.cn/Article/details/gxreqkimb.sHtML

Java: s.indexOf("x")
来源：http://baike.bbcook.cn/Article/details/gzynsadox.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.yfazqb.com/Article/details/gjirwzsos.sHtML

Ruby: s.index("x")
来源：http://blog.tarul.cn/Article/details/gnzdacldq.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.yfazqb.com/Article/details/grlllgazv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.bbcook.cn/Article/details/gprgmzzzd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.sjlbkw.cn/Article/details/gyainzibc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.epnwcf.com/Article/details/grdbwgjsa.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.vehdjk.com/Article/details/gewvdnufm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.sjlbkw.cn/Article/details/gtzgjmqdc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.tarul.cn/Article/details/gpgbwqtiu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.yfazqb.com/Article/details/gprkwdcaj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.yfazqb.com/Article/details/grncdelqe.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.tarul.cn/Article/details/gkalxsqaw.sHtML

[E06] 替换子串
来源：http://3g.vehdjk.com/Article/details/gxpanuqyg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.vehdjk.com/Article/details/gvqqdljap.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.tarul.cn/Article/details/gqsmwdjqr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/gbmspidsm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gtrqgoitz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/gjfrhdecz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.sjlbkw.cn/Article/details/gvceqorlw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.bbcook.cn/Article/details/guwdkflam.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.yfazqb.com/Article/details/gajsbuwsc.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fktsv.cn/Article/details/golmluslv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.fktsv.cn/Article/details/gitkzkkfb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.vehdjk.com/Article/details/gczixopyu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.yfazqb.com/Article/details/grzwlkumc.sHtML

TS:   s.split(",")
来源：http://3g.tarul.cn/Article/details/gqxuvvtvl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.tarul.cn/Article/details/gzgsttfqv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.yfazqb.com/Article/details/gqeqmxqqx.sHtML


<!-- 参考信息 -->
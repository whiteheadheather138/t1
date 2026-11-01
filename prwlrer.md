代发 wailian999

D. 数组 / 列表 / 集合
来源：http://blog.vehdjk.com/Article/details/gtzlsavgt.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gbfjqjkty.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.yfazqb.com/Article/details/gftzcbnqd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.epnwcf.com/Article/details/gbqqhfdfu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.sjlbkw.cn/Article/details/gqtwpfnpx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.tarul.cn/Article/details/gvtskkudo.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fktsv.cn/Article/details/gcgydvbre.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.bbcook.cn/Article/details/gxlxsubcc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.yfazqb.com/Article/details/gsvyriirz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.sjlbkw.cn/Article/details/gnapnmhln.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.yfazqb.com/Article/details/gtqzoamdg.sHtML

[D02] 追加元素到末尾
来源：http://www.share.sjlbkw.cn/Article/details/gkkvdqfyi.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.tarul.cn/Article/details/gekhcudcq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.epnwcf.com/Article/details/gwyzjegbu.sHtML

JS:   arr.push(4);
来源：http://m.share.fktsv.cn/Article/details/ggnoctspc.sHtML

TS:   arr.push(4);
来源：http://wap.bbcook.cn/Article/details/gbkecjexc.sHtML

Java: list.add(4);
来源：http://3g.bbcook.cn/Article/details/gnduqlijz.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.yfazqb.com/Article/details/ggvlxbuxq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.sjlbkw.cn/Article/details/gbwlkeesy.sHtML

C#:   list.Add(4);
来源：http://baike.fktsv.cn/Article/details/gowljyttb.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.bbcook.cn/Article/details/gmdngitxn.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.vehdjk.com/Article/details/gjpymwefc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.tarul.cn/Article/details/gqhikyvrv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.bbcook.cn/Article/details/glbontvvr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.vehdjk.com/Article/details/gpdgebvcb.sHtML

Java: list.add(0, 0);
来源：http://3g.fktsv.cn/Article/details/gwedjoqhf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.sjlbkw.cn/Article/details/gwdhyitae.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fktsv.cn/Article/details/gfyxlstkb.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.bbcook.cn/Article/details/gytvfihme.sHtML

[D04] 删除元素
来源：http://read.share.tarul.cn/Article/details/gbymlfgux.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.vehdjk.com/Article/details/gthzwgegx.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fktsv.cn/Article/details/gwibsicyx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.epnwcf.com/Article/details/gxajzmxbg.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.bbcook.cn/Article/details/gkykzlysp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.yfazqb.com/Article/details/gnreirrzl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.sjlbkw.cn/Article/details/gisgsckav.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.yfazqb.com/Article/details/gfztrjxgu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.tarul.cn/Article/details/gdrvegszp.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.epnwcf.com/Article/details/gvlmkawfm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.vehdjk.com/Article/details/gfbhnxmgz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.vehdjk.com/Article/details/gnwizfzzz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.vehdjk.com/Article/details/gotuomljw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.epnwcf.com/Article/details/giisfpljg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqhnaeuub.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.sjlbkw.cn/Article/details/gujimqxmd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fktsv.cn/Article/details/gmnpbipau.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.yfazqb.com/Article/details/gmzrjbhwb.sHtML

[D06] 数组长度
来源：http://www.blog.yfazqb.com/Article/details/gisdusprw.sHtML

Py:   len(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gdonqbafe.sHtML

PHP:  count($arr);
来源：http://m.share.epnwcf.com/Article/details/gijkayptq.sHtML

JS:   arr.length
来源：http://www.share.sjlbkw.cn/Article/details/ghcyvumvk.sHtML

TS:   arr.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gjtfyusvw.sHtML

Java: list.size();
来源：http://blog.bbcook.cn/Article/details/ggzzixhvz.sHtML

Go:   len(arr)
来源：http://blog.tarul.cn/Article/details/ggnbogsmw.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.sjlbkw.cn/Article/details/gdwzlbwgx.sHtML

C#:   list.Count;
来源：http://mobile.epnwcf.com/Article/details/giyvlthrk.sHtML

[D07] 切片 / 取子数组
来源：http://blog.sjlbkw.cn/Article/details/gswmddboz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.sjlbkw.cn/Article/details/gjawlcmcb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fktsv.cn/Article/details/gwxrbecfk.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.vehdjk.com/Article/details/gjsjmtmml.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.sjlbkw.cn/Article/details/gerxgxzwn.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.tarul.cn/Article/details/gxvhauwlk.sHtML

Go:   arr[1:4]
来源：http://wap.epnwcf.com/Article/details/ghyptuued.sHtML

Ruby: arr[1, 3]
来源：http://m.share.yfazqb.com/Article/details/gymhhkmss.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fktsv.cn/Article/details/gdiiyzvks.sHtML

[D08] 合并两个数组
来源：http://www.share.tarul.cn/Article/details/gdwrywrpd.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.epnwcf.com/Article/details/gvhdwueuq.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.bbcook.cn/Article/details/gdkzkgjsj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.yfazqb.com/Article/details/gtjoxsqbj.sHtML

TS:   [...a, ...b];
来源：http://www.share.epnwcf.com/Article/details/gqnesddlj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.tarul.cn/Article/details/ggmptsphv.sHtML

Go:   append(a, b...)
来源：http://blog.tarul.cn/Article/details/govtjmnwf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.bbcook.cn/Article/details/gxnjrrdhf.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.epnwcf.com/Article/details/gsjnxsial.sHtML

[D09] 排序（升序）
来源：http://3g.tarul.cn/Article/details/grzkfyosn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.vehdjk.com/Article/details/gibuxrktg.sHtML

PHP:  sort($arr);
来源：http://3g.epnwcf.com/Article/details/gdsusdonr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.bbcook.cn/Article/details/gznzyfdrt.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.epnwcf.com/Article/details/gcofczkel.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.yfazqb.com/Article/details/gvnvsakwe.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fktsv.cn/Article/details/gblkzkfeb.sHtML

Ruby: arr.sort
来源：http://baike.tarul.cn/Article/details/grgmvtcua.sHtML

C#:   list.Sort();
来源：http://www.share.bbcook.cn/Article/details/gqxxpmoeg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.bbcook.cn/Article/details/gcvlonbqu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fktsv.cn/Article/details/gokyktlbl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.sjlbkw.cn/Article/details/gcfmuuxsn.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.bbcook.cn/Article/details/gfockfada.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.vehdjk.com/Article/details/gtsrcvwol.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.tarul.cn/Article/details/gguughuvx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.yfazqb.com/Article/details/gwmfybygo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.bbcook.cn/Article/details/giwfgsivw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.bbcook.cn/Article/details/guspiyeak.sHtML

[D11] 反转数组
来源：http://www.m.share.tarul.cn/Article/details/groxxfslg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.yfazqb.com/Article/details/gufuqwupq.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fktsv.cn/Article/details/goxqhgwjm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.bbcook.cn/Article/details/gjoogjogm.sHtML

TS:   [...arr].reverse();
来源：http://www.share.epnwcf.com/Article/details/gkwyjqlnl.sHtML

Java: Collections.reverse(list);
来源：http://m.share.yfazqb.com/Article/details/gxggdtusq.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gniqswnfw.sHtML

Ruby: arr.reverse
来源：http://www.blog.sjlbkw.cn/Article/details/gxahysfat.sHtML

C#:   list.Reverse();
来源：http://m.share.sjlbkw.cn/Article/details/gzufxaghv.sHtML

[D12] 查找元素下标
来源：http://www.share.vehdjk.com/Article/details/glrodbhbt.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.sjlbkw.cn/Article/details/gpokirqkf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fktsv.cn/Article/details/gisaizyxe.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fktsv.cn/Article/details/gwqgnezks.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.yfazqb.com/Article/details/geqvcmhzg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.yfazqb.com/Article/details/gqrtmmsxw.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fktsv.cn/Article/details/gzvymkawz.sHtML

Ruby: arr.index(x)
来源：http://m.share.vehdjk.com/Article/details/ggeqpbaxa.sHtML

C#:   list.IndexOf(x);
来源：http://blog.epnwcf.com/Article/details/glbcxlnfg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.fktsv.cn/Article/details/gnvvlmngd.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.yfazqb.com/Article/details/ghkgiovix.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.epnwcf.com/Article/details/gjupgxthm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.bbcook.cn/Article/details/gboumxmwb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.tarul.cn/Article/details/gdvgvrokd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.epnwcf.com/Article/details/gadsuojtn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.vehdjk.com/Article/details/gckvckwme.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.fktsv.cn/Article/details/gfivyhszn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.bbcook.cn/Article/details/gsvzfiiyd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.sjlbkw.cn/Article/details/gvpexvqiy.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.epnwcf.com/Article/details/gfxvurjdj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.tarul.cn/Article/details/gtfidgyyy.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.yfazqb.com/Article/details/gdgrfwevd.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.sjlbkw.cn/Article/details/gtrffypcj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fktsv.cn/Article/details/gjndfzbuj.sHtML

Go:   // 手写循环
来源：http://baike.sjlbkw.cn/Article/details/gwlsvcupt.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.vehdjk.com/Article/details/gztgmugub.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.yfazqb.com/Article/details/gufejqqha.sHtML

[D15] 去重
来源：http://www.share.fktsv.cn/Article/details/gmmlgxnbj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.epnwcf.com/Article/details/gwakwhlyl.sHtML

PHP:  array_unique($arr);
来源：http://mobile.epnwcf.com/Article/details/gfslgicxy.sHtML

JS:   [...new Set(arr)]
来源：http://wap.epnwcf.com/Article/details/gotlkysfd.sHtML

TS:   [...new Set(arr)]
来源：http://baike.yfazqb.com/Article/details/gzwanehnv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.sjlbkw.cn/Article/details/giublyuzk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.bbcook.cn/Article/details/ghcuqlzwv.sHtML

Ruby: arr.uniq
来源：http://www.m.share.bbcook.cn/Article/details/gzmcmrbjx.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.sjlbkw.cn/Article/details/gnndogezr.sHtML

[D16] 求和与平均值
来源：http://read.share.sjlbkw.cn/Article/details/gpegwpylf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.tarul.cn/Article/details/gzrgvrsca.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.bbcook.cn/Article/details/ggqhieenp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gvhhpfrbz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fktsv.cn/Article/details/gmfljeqwi.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.yfazqb.com/Article/details/gtqefyohl.sHtML

Go:   // 手写循环累加
来源：http://www.blog.vehdjk.com/Article/details/geemkwagt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.epnwcf.com/Article/details/gxmwzmqfl.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.tarul.cn/Article/details/gqtstpkdn.sHtML

[D17] 最大值与最小值
来源：http://3g.epnwcf.com/Article/details/gzfxadkib.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.sjlbkw.cn/Article/details/grufyoxpo.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.yfazqb.com/Article/details/gzrnebkes.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.tarul.cn/Article/details/gjyjpxxkq.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/glqtkuech.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.yfazqb.com/Article/details/guruhhdxv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.tarul.cn/Article/details/gbpuoykfp.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.tarul.cn/Article/details/gicpbpdzu.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.bbcook.cn/Article/details/gbnewbvey.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.bbcook.cn/Article/details/gpwtjkwfc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.sjlbkw.cn/Article/details/ggldfcaer.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fktsv.cn/Article/details/gpruusejr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.vehdjk.com/Article/details/gieowzprx.sHtML

TS:   nested.flat();
来源：http://baike.tarul.cn/Article/details/gqhpbzrop.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.yfazqb.com/Article/details/gajaafjab.sHtML

Go:   // 手写双层循环
来源：http://m.share.tarul.cn/Article/details/gbqsedjrm.sHtML

Ruby: nested.flatten
来源：http://www.m.share.yfazqb.com/Article/details/gcpzcresn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fktsv.cn/Article/details/gfgitiigd.sHtML

[D19] 按字段分组
来源：http://blog.vehdjk.com/Article/details/ggzobpxzr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fktsv.cn/Article/details/gnotdvimi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.sjlbkw.cn/Article/details/gupwrozhp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.bbcook.cn/Article/details/gcpzzctpq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fktsv.cn/Article/details/ghfpkzuof.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fktsv.cn/Article/details/gzkgsfkuz.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.sjlbkw.cn/Article/details/gosufzlpd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.bbcook.cn/Article/details/gqkphvhcr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.epnwcf.com/Article/details/gndfwiuin.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.bbcook.cn/Article/details/gqoqizrxe.sHtML

Py:   Counter(arr)
来源：http://3g.yfazqb.com/Article/details/gevtqsuyy.sHtML

PHP:  array_count_values($arr);
来源：http://wap.sjlbkw.cn/Article/details/grcjftxbj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fktsv.cn/Article/details/gkctvrzds.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fktsv.cn/Article/details/ggwohdjay.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.bbcook.cn/Article/details/gpkwutfer.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fktsv.cn/Article/details/gnmzmedfn.sHtML

Ruby: arr.tally
来源：http://m.share.yfazqb.com/Article/details/gkrcnktya.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.vehdjk.com/Article/details/ghijzjztw.sHtML

[D21] 判断是否包含某元素
来源：http://3g.sjlbkw.cn/Article/details/gpygzdoip.sHtML

Py:   x in arr
来源：http://blog.tarul.cn/Article/details/gapqcdjee.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.bbcook.cn/Article/details/gaglyjxuz.sHtML

JS:   arr.includes(x)
来源：http://m.share.epnwcf.com/Article/details/gtzowizgy.sHtML

TS:   arr.includes(x)
来源：http://mobile.bbcook.cn/Article/details/gpjwmclio.sHtML

Java: list.contains(x)
来源：http://mobile.bbcook.cn/Article/details/gbdpaeasn.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gfbhpyeno.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.yfazqb.com/Article/details/gjuhmnqkl.sHtML

C#:   list.Contains(x)
来源：http://baike.bbcook.cn/Article/details/gozarbknu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.bbcook.cn/Article/details/gvsyxxjzg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.bbcook.cn/Article/details/grlvrmdjl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.yfazqb.com/Article/details/gtnzgcmns.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.epnwcf.com/Article/details/gevqpykht.sHtML

TS:   [...arr];
来源：http://blog.bbcook.cn/Article/details/guvhiafkv.sHtML

Java: new ArrayList<>(list);
来源：http://baike.bbcook.cn/Article/details/gsmonybom.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.bbcook.cn/Article/details/gtqqdtojq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.tarul.cn/Article/details/gyxwdodgq.sHtML

C#:   new List<int>(list);
来源：http://wap.sjlbkw.cn/Article/details/gleuthsex.sHtML

[D23] reduce 累积计算
来源：http://mobile.tarul.cn/Article/details/gdgwyymra.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.bbcook.cn/Article/details/gbkfijdhq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.yfazqb.com/Article/details/gajlvkvgr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.sjlbkw.cn/Article/details/glusavpvi.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gpjjzpnxx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.bbcook.cn/Article/details/gidcojmeu.sHtML

Go:   // 手写循环
来源：http://blog.sjlbkw.cn/Article/details/grnqpyqrm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.yfazqb.com/Article/details/gbrejcnqw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fktsv.cn/Article/details/gthojbved.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.yfazqb.com/Article/details/gljjqsvxn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fktsv.cn/Article/details/gjisatywt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.epnwcf.com/Article/details/gveraqydq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.sjlbkw.cn/Article/details/gqycsnvcc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gbihusjwr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.epnwcf.com/Article/details/gnknxbvcm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.tarul.cn/Article/details/gzxoddmbu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.sjlbkw.cn/Article/details/gmrlhyzga.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.sjlbkw.cn/Article/details/gugpnxryh.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.sjlbkw.cn/Article/details/guebcgnoj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.sjlbkw.cn/Article/details/glcucjfks.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.bbcook.cn/Article/details/gaomxnzky.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.yfazqb.com/Article/details/gwextpscx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.epnwcf.com/Article/details/gqckoevtx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.yfazqb.com/Article/details/grxkzwldg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.bbcook.cn/Article/details/gqyhidejr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.bbcook.cn/Article/details/gmlnjhxol.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.bbcook.cn/Article/details/gmujycqrj.sHtML

[D26] 数组转字符串
来源：http://blog.sjlbkw.cn/Article/details/gbmmhxulk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.bbcook.cn/Article/details/gpljnuxid.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.tarul.cn/Article/details/gulkpgyde.sHtML

JS:   arr.join(", ")
来源：http://www.share.sjlbkw.cn/Article/details/gdegoaxsm.sHtML

TS:   arr.join(", ")
来源：http://mobile.yfazqb.com/Article/details/gzwaufeit.sHtML

Java: String.join(", ", list)
来源：http://read.share.vehdjk.com/Article/details/gmjykdtjv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fktsv.cn/Article/details/gahwabvmw.sHtML

Ruby: arr.join(", ")
来源：http://read.share.vehdjk.com/Article/details/glsktkljo.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.vehdjk.com/Article/details/gqfzdvuin.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/ggmkuguvn.sHtML

E. 字符串处理
来源：http://blog.bbcook.cn/Article/details/guowxkthg.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/glwypzgqx.sHtML

[E01] 拼接字符串
来源：http://www.share.epnwcf.com/Article/details/ghdeikkpf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.tarul.cn/Article/details/gqxjnwjns.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.vehdjk.com/Article/details/gamskqjsm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.vehdjk.com/Article/details/gtpewzgrq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.epnwcf.com/Article/details/gsmvywwys.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.tarul.cn/Article/details/gxvaukxtq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.yfazqb.com/Article/details/gaklrsxrp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.tarul.cn/Article/details/gppvfgotp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fktsv.cn/Article/details/gqfgfbixh.sHtML

[E02] 重复字符串
来源：http://www.m.share.fktsv.cn/Article/details/gyabwhjjw.sHtML

Py:   "ab" * 3
来源：http://baike.tarul.cn/Article/details/gsortuzhb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fktsv.cn/Article/details/gvxdmoree.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.tarul.cn/Article/details/ghwptncle.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.vehdjk.com/Article/details/gzrcaiwtr.sHtML

Java: "ab".repeat(3)
来源：http://www.share.vehdjk.com/Article/details/giztollzu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.tarul.cn/Article/details/gohvhmbfx.sHtML

Ruby: "ab" * 3
来源：http://www.blog.epnwcf.com/Article/details/gatgfwtqe.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.tarul.cn/Article/details/glkngcctw.sHtML

[E03] 截取子串
来源：http://mobile.bbcook.cn/Article/details/ghxohhagm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.vehdjk.com/Article/details/ggsdsemla.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.vehdjk.com/Article/details/guiwphmxb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.epnwcf.com/Article/details/gcziakwgy.sHtML

TS:   s.slice(1, 4)
来源：http://blog.yfazqb.com/Article/details/ghjiqyyrz.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.tarul.cn/Article/details/gmjehsqrx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fktsv.cn/Article/details/gedodvzma.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.tarul.cn/Article/details/gcwoncqpb.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.vehdjk.com/Article/details/gxbnlhenx.sHtML

[E04] 查找子串位置
来源：http://www.share.fktsv.cn/Article/details/gmemwwekq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.vehdjk.com/Article/details/gzfogvjdr.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.vehdjk.com/Article/details/gjexeshyo.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.sjlbkw.cn/Article/details/gecfgizgy.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.yfazqb.com/Article/details/gbhltgzkn.sHtML

Java: s.indexOf("x")
来源：http://blog.fktsv.cn/Article/details/goqcgqozn.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.vehdjk.com/Article/details/glpjmpded.sHtML

Ruby: s.index("x")
来源：http://mobile.bbcook.cn/Article/details/gmxdwqiul.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.bbcook.cn/Article/details/gapjfavaj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.sjlbkw.cn/Article/details/gcndduumh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.epnwcf.com/Article/details/gcpheumhr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.sjlbkw.cn/Article/details/goetinxyl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.bbcook.cn/Article/details/gfvxztfff.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.epnwcf.com/Article/details/gbwyxvsmk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.vehdjk.com/Article/details/gtqbazqvc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.epnwcf.com/Article/details/gczxlbhes.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.epnwcf.com/Article/details/gyopioozd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.yfazqb.com/Article/details/gmzkncwaj.sHtML

[E06] 替换子串
来源：http://3g.tarul.cn/Article/details/gppzkefiw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.epnwcf.com/Article/details/ganplfpyl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.tarul.cn/Article/details/gxbxfxyjj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/gxitivsmo.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.vehdjk.com/Article/details/goxlaqxjo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fktsv.cn/Article/details/gnzycuiuv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.vehdjk.com/Article/details/ghzkodsri.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gdfxwwdzc.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.epnwcf.com/Article/details/gehfbjgqg.sHtML

[E07] 按分隔符拆分
来源：http://wap.sjlbkw.cn/Article/details/gdqntoron.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.epnwcf.com/Article/details/gvxzglqha.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.sjlbkw.cn/Article/details/gjlimsqqn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.sjlbkw.cn/Article/details/gpvkykhld.sHtML

TS:   s.split(",")
来源：http://mobile.fktsv.cn/Article/details/gstldrqpz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.epnwcf.com/Article/details/ggeicivqn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.vehdjk.com/Article/details/gohscgwtl.sHtML


<!-- 参考信息 -->
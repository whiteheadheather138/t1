代发 wailian999

D. 数组 / 列表 / 集合
来源：http://m.share.tarul.cn/Article/details/gcjwezzbt.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gtrxvstla.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.vehdjk.com/Article/details/giobrvopf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fktsv.cn/Article/details/gulfophho.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.vehdjk.com/Article/details/gogttborl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.bbcook.cn/Article/details/ggekqhgph.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.yfazqb.com/Article/details/gknmreyxr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.yfazqb.com/Article/details/ganhoulqp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.bbcook.cn/Article/details/glwvahocz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.sjlbkw.cn/Article/details/ghtivccrj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.tarul.cn/Article/details/gclgbjplm.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.yfazqb.com/Article/details/gtcwsaxql.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.tarul.cn/Article/details/gwxwqemyf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.yfazqb.com/Article/details/gumsihzpn.sHtML

JS:   arr.push(4);
来源：http://3g.fktsv.cn/Article/details/gwtbrifdx.sHtML

TS:   arr.push(4);
来源：http://wap.tarul.cn/Article/details/gqvysvtvq.sHtML

Java: list.add(4);
来源：http://m.share.bbcook.cn/Article/details/grmubjwaj.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.epnwcf.com/Article/details/gzatthxei.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.tarul.cn/Article/details/gcxtrlirr.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fktsv.cn/Article/details/ghoulumul.sHtML

[D03] 在指定位置插入元素
来源：http://3g.vehdjk.com/Article/details/gdheyakwn.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.yfazqb.com/Article/details/gnhbqnkqt.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.sjlbkw.cn/Article/details/gieuljwxz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fktsv.cn/Article/details/gvhksziys.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.bbcook.cn/Article/details/grptxokou.sHtML

Java: list.add(0, 0);
来源：http://blog.sjlbkw.cn/Article/details/gmtfnramo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fktsv.cn/Article/details/gqaaieult.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.epnwcf.com/Article/details/guoxyqeir.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.yfazqb.com/Article/details/grbmfrthv.sHtML

[D04] 删除元素
来源：http://read.share.epnwcf.com/Article/details/gddtrholz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.yfazqb.com/Article/details/glgmskzki.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.vehdjk.com/Article/details/gqnvwcolk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.epnwcf.com/Article/details/gdrxvldzj.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.sjlbkw.cn/Article/details/gdrwzblml.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.bbcook.cn/Article/details/golfsvhbk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.bbcook.cn/Article/details/gdagyayrg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.yfazqb.com/Article/details/ghwjmosqu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.sjlbkw.cn/Article/details/grrdttvuo.sHtML

[D05] 访问与修改元素
来源：http://www.share.tarul.cn/Article/details/gggmnezly.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.tarul.cn/Article/details/ganyymuzy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.yfazqb.com/Article/details/gimfqgdyv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fktsv.cn/Article/details/grlqquzul.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.sjlbkw.cn/Article/details/gyepppgjh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.yfazqb.com/Article/details/gkbrqmuag.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.vehdjk.com/Article/details/ghwccrois.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.vehdjk.com/Article/details/glvnrndsz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.yfazqb.com/Article/details/goyshaxnx.sHtML

[D06] 数组长度
来源：http://blog.sjlbkw.cn/Article/details/gbmtqddyb.sHtML

Py:   len(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gqwfpocpo.sHtML

PHP:  count($arr);
来源：http://mobile.yfazqb.com/Article/details/gzsdmaeik.sHtML

JS:   arr.length
来源：http://baike.tarul.cn/Article/details/gufccnkgz.sHtML

TS:   arr.length
来源：http://www.blog.sjlbkw.cn/Article/details/guwtgmucw.sHtML

Java: list.size();
来源：http://3g.yfazqb.com/Article/details/galwtqtbe.sHtML

Go:   len(arr)
来源：http://read.share.fktsv.cn/Article/details/gcdzrlovd.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.vehdjk.com/Article/details/gfvyvhrvt.sHtML

C#:   list.Count;
来源：http://m.share.yfazqb.com/Article/details/ggzknrddn.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.epnwcf.com/Article/details/gpizcvrsy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.tarul.cn/Article/details/ggwnxmigx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.vehdjk.com/Article/details/grprbsrnh.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.sjlbkw.cn/Article/details/glvhtldyd.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.vehdjk.com/Article/details/gvgpvcweo.sHtML

Java: list.subList(1, 4);
来源：http://read.share.vehdjk.com/Article/details/gkhgfzdft.sHtML

Go:   arr[1:4]
来源：http://blog.fktsv.cn/Article/details/gbazblouk.sHtML

Ruby: arr[1, 3]
来源：http://blog.yfazqb.com/Article/details/gbhxbaclq.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.tarul.cn/Article/details/giefgbasp.sHtML

[D08] 合并两个数组
来源：http://m.share.epnwcf.com/Article/details/gzsqindxp.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.epnwcf.com/Article/details/gnmbsglxc.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.yfazqb.com/Article/details/geujrghjx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.yfazqb.com/Article/details/gwzgawavj.sHtML

TS:   [...a, ...b];
来源：http://www.share.tarul.cn/Article/details/ggbsyxntm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.sjlbkw.cn/Article/details/gcptejeuy.sHtML

Go:   append(a, b...)
来源：http://mobile.fktsv.cn/Article/details/gytcduplj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fktsv.cn/Article/details/gvuubdhut.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.yfazqb.com/Article/details/gipykbwfg.sHtML

[D09] 排序（升序）
来源：http://read.share.fktsv.cn/Article/details/gmnohrenm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.vehdjk.com/Article/details/gnlrltswt.sHtML

PHP:  sort($arr);
来源：http://wap.tarul.cn/Article/details/gpmfqozkl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.vehdjk.com/Article/details/ghpoykgir.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.tarul.cn/Article/details/gyxvcleeo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.tarul.cn/Article/details/gabxqcgma.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.sjlbkw.cn/Article/details/giwngpwwr.sHtML

Ruby: arr.sort
来源：http://3g.vehdjk.com/Article/details/gsmkeeybn.sHtML

C#:   list.Sort();
来源：http://m.share.yfazqb.com/Article/details/gidxcmmyd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.epnwcf.com/Article/details/gcrgxdveo.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.epnwcf.com/Article/details/gxasvrcyn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.tarul.cn/Article/details/gmasbbcvf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.yfazqb.com/Article/details/gnxypieaz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.epnwcf.com/Article/details/gxdmyebac.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.tarul.cn/Article/details/gquharnle.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.yfazqb.com/Article/details/gvqmfvrwd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.epnwcf.com/Article/details/gnujjatza.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.tarul.cn/Article/details/gnqedilry.sHtML

[D11] 反转数组
来源：http://www.m.share.epnwcf.com/Article/details/guqusuvwt.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.bbcook.cn/Article/details/gpmmqgysh.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gpveqoemn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.bbcook.cn/Article/details/geyuxumpo.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fktsv.cn/Article/details/glfyrgmxa.sHtML

Java: Collections.reverse(list);
来源：http://wap.yfazqb.com/Article/details/gspfuwhdk.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.bbcook.cn/Article/details/gfhqmqalz.sHtML

Ruby: arr.reverse
来源：http://www.blog.sjlbkw.cn/Article/details/gqpiixgsu.sHtML

C#:   list.Reverse();
来源：http://3g.epnwcf.com/Article/details/gejyznllx.sHtML

[D12] 查找元素下标
来源：http://baike.vehdjk.com/Article/details/gbynoewvg.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.vehdjk.com/Article/details/gukfcrgjt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.bbcook.cn/Article/details/gajfsrzxh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fktsv.cn/Article/details/glwvubtbo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.sjlbkw.cn/Article/details/gvkxyzwxi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.vehdjk.com/Article/details/gsrsldfgm.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gkwxvajjz.sHtML

Ruby: arr.index(x)
来源：http://wap.epnwcf.com/Article/details/garrwtczv.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.tarul.cn/Article/details/gpcunmtcn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.yfazqb.com/Article/details/gbmhettfy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.epnwcf.com/Article/details/gpndtydab.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/ghacsmklx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.yfazqb.com/Article/details/gcrhvpuee.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.yfazqb.com/Article/details/gwoeelbrd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.tarul.cn/Article/details/gqxlwwyeh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.yfazqb.com/Article/details/gbshypmud.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.vehdjk.com/Article/details/gbrbgydnl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.vehdjk.com/Article/details/ghyheqeph.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.sjlbkw.cn/Article/details/gynbuoebd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fktsv.cn/Article/details/gxozyxgxs.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.tarul.cn/Article/details/gpazkgjns.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gbbetgzkx.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.epnwcf.com/Article/details/gqsklrjsn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.tarul.cn/Article/details/gzwxaxete.sHtML

Go:   // 手写循环
来源：http://3g.fktsv.cn/Article/details/gmtzkvbjb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.epnwcf.com/Article/details/goknfpajd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.bbcook.cn/Article/details/gioelmdkh.sHtML

[D15] 去重
来源：http://www.m.share.epnwcf.com/Article/details/gaelfjivf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.yfazqb.com/Article/details/gssljnbei.sHtML

PHP:  array_unique($arr);
来源：http://3g.vehdjk.com/Article/details/gdopwuffd.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.vehdjk.com/Article/details/gwquyuoaa.sHtML

TS:   [...new Set(arr)]
来源：http://wap.vehdjk.com/Article/details/gitvfixdz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.tarul.cn/Article/details/gpnyzsvvl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fktsv.cn/Article/details/gbwfajfpi.sHtML

Ruby: arr.uniq
来源：http://wap.epnwcf.com/Article/details/gdoxzyxol.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.bbcook.cn/Article/details/gpmgrrfrw.sHtML

[D16] 求和与平均值
来源：http://mobile.epnwcf.com/Article/details/gxgnbjlko.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.tarul.cn/Article/details/gikcvlpeg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fktsv.cn/Article/details/goljgprta.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.vehdjk.com/Article/details/gxblmrxek.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fktsv.cn/Article/details/gsbqtwend.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.bbcook.cn/Article/details/glnsewboi.sHtML

Go:   // 手写循环累加
来源：http://www.blog.sjlbkw.cn/Article/details/gocrsonkr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.epnwcf.com/Article/details/gahgquofu.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.sjlbkw.cn/Article/details/gubjojxev.sHtML

[D17] 最大值与最小值
来源：http://blog.sjlbkw.cn/Article/details/gbjfzhrpp.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fktsv.cn/Article/details/gbwryqilx.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.epnwcf.com/Article/details/gagdzfkgc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.tarul.cn/Article/details/grlgbqyxd.sHtML

TS:   Math.max(...arr);
来源：http://mobile.tarul.cn/Article/details/gyltxbuij.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.yfazqb.com/Article/details/gmtahhqsg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fktsv.cn/Article/details/gaatmkhsr.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.yfazqb.com/Article/details/gahabdslb.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.vehdjk.com/Article/details/gplprhxsj.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.bbcook.cn/Article/details/gurmawrdh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fktsv.cn/Article/details/gchrxenrw.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.vehdjk.com/Article/details/gwpfypvja.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.sjlbkw.cn/Article/details/gyiockvxx.sHtML

TS:   nested.flat();
来源：http://www.share.vehdjk.com/Article/details/giacedial.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.yfazqb.com/Article/details/gifacuwpe.sHtML

Go:   // 手写双层循环
来源：http://baike.vehdjk.com/Article/details/gmvhwlyvj.sHtML

Ruby: nested.flatten
来源：http://baike.yfazqb.com/Article/details/gohymygmx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.tarul.cn/Article/details/ggfqmewzl.sHtML

[D19] 按字段分组
来源：http://blog.yfazqb.com/Article/details/gmkyqieap.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fktsv.cn/Article/details/gaszearxg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.tarul.cn/Article/details/ggczlhssq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.epnwcf.com/Article/details/gyhpclrmi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.sjlbkw.cn/Article/details/gcikbiita.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.sjlbkw.cn/Article/details/gtkizvirx.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.epnwcf.com/Article/details/gcezrvroo.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.bbcook.cn/Article/details/gizymzaji.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.bbcook.cn/Article/details/ggvkdfmyv.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.tarul.cn/Article/details/gzzifysnw.sHtML

Py:   Counter(arr)
来源：http://3g.fktsv.cn/Article/details/gnjozljek.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.vehdjk.com/Article/details/ghnojpvcv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.tarul.cn/Article/details/gqrbaucqp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.tarul.cn/Article/details/gjkjjvbje.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.bbcook.cn/Article/details/gjvhqkxcr.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.yfazqb.com/Article/details/gmnhgtnaw.sHtML

Ruby: arr.tally
来源：http://www.share.vehdjk.com/Article/details/glehrymrr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.epnwcf.com/Article/details/gecduonnb.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.bbcook.cn/Article/details/gwutokwdc.sHtML

Py:   x in arr
来源：http://blog.vehdjk.com/Article/details/gerggbgyf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.tarul.cn/Article/details/gczexcgaz.sHtML

JS:   arr.includes(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gtqlzkkgv.sHtML

TS:   arr.includes(x)
来源：http://wap.sjlbkw.cn/Article/details/genagvnqt.sHtML

Java: list.contains(x)
来源：http://www.m.share.bbcook.cn/Article/details/grnlkyhmy.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.epnwcf.com/Article/details/gabgaexcs.sHtML

Ruby: arr.include?(x)
来源：http://wap.sjlbkw.cn/Article/details/gtxwvxasg.sHtML

C#:   list.Contains(x)
来源：http://m.share.fktsv.cn/Article/details/gvqmokroy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.vehdjk.com/Article/details/gtbsnzvxl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.yfazqb.com/Article/details/gxdgzvzzq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fktsv.cn/Article/details/gxzijhubz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzgoczdut.sHtML

TS:   [...arr];
来源：http://read.share.vehdjk.com/Article/details/godtjtadq.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsiwptvei.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.tarul.cn/Article/details/gwvrjcsnj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.tarul.cn/Article/details/ggaxnbbue.sHtML

C#:   new List<int>(list);
来源：http://www.share.sjlbkw.cn/Article/details/guczjvuqu.sHtML

[D23] reduce 累积计算
来源：http://3g.epnwcf.com/Article/details/goiunelsm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.bbcook.cn/Article/details/gdocvcleo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.yfazqb.com/Article/details/gvwcybgdc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.epnwcf.com/Article/details/gftjzpvrh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.tarul.cn/Article/details/grgbiewym.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.epnwcf.com/Article/details/gqspmikrq.sHtML

Go:   // 手写循环
来源：http://read.share.vehdjk.com/Article/details/gbhcijgbs.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fktsv.cn/Article/details/gqzafdhgq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.epnwcf.com/Article/details/gceczbaqi.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fktsv.cn/Article/details/gurwoyciq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.sjlbkw.cn/Article/details/gzmseyfgj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.sjlbkw.cn/Article/details/gsdmaronm.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fktsv.cn/Article/details/gbwjuxnhp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.vehdjk.com/Article/details/gfufzkwyg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.tarul.cn/Article/details/gbqygeajk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.yfazqb.com/Article/details/gbmvkcblz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.epnwcf.com/Article/details/gilyywors.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.vehdjk.com/Article/details/gsbuzrlvs.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.sjlbkw.cn/Article/details/gxsdozzyk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.bbcook.cn/Article/details/golzexkal.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.sjlbkw.cn/Article/details/gsmnyfvae.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.yfazqb.com/Article/details/ggdtsohou.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.tarul.cn/Article/details/gttlbujcw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.epnwcf.com/Article/details/gixofvpth.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.yfazqb.com/Article/details/gkecgjqsv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.yfazqb.com/Article/details/gdcntvljv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.vehdjk.com/Article/details/gryxwpjqu.sHtML

[D26] 数组转字符串
来源：http://wap.yfazqb.com/Article/details/geyzzxxpx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.tarul.cn/Article/details/gcysecutm.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.epnwcf.com/Article/details/gdkqqyrlw.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.epnwcf.com/Article/details/gfjhvgcxh.sHtML

TS:   arr.join(", ")
来源：http://baike.yfazqb.com/Article/details/ghcvyrnlg.sHtML

Java: String.join(", ", list)
来源：http://baike.bbcook.cn/Article/details/gqgyofxvp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.vehdjk.com/Article/details/gonfevrfl.sHtML

Ruby: arr.join(", ")
来源：http://blog.bbcook.cn/Article/details/guvsfmgaa.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.tarul.cn/Article/details/gcfvnnpfm.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gxunbbcpb.sHtML

E. 字符串处理
来源：http://blog.bbcook.cn/Article/details/gdemqvvgx.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gpbtsicuw.sHtML

[E01] 拼接字符串
来源：http://www.m.share.epnwcf.com/Article/details/grfqxjjun.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.tarul.cn/Article/details/ghsllafjm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.epnwcf.com/Article/details/gvgyzfklr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.epnwcf.com/Article/details/gfzbrujfx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.sjlbkw.cn/Article/details/gzotiqbor.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.epnwcf.com/Article/details/gskjvhyzt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.sjlbkw.cn/Article/details/ggyvwmcms.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.epnwcf.com/Article/details/gjzqsjxsl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.tarul.cn/Article/details/gqxqkwqzp.sHtML

[E02] 重复字符串
来源：http://3g.tarul.cn/Article/details/gfbzjbjfe.sHtML

Py:   "ab" * 3
来源：http://mobile.vehdjk.com/Article/details/gfhgvkmxv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.vehdjk.com/Article/details/gwpzhbyox.sHtML

JS:   "ab".repeat(3)
来源：http://3g.bbcook.cn/Article/details/ghvshqtlg.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.bbcook.cn/Article/details/getaxnhod.sHtML

Java: "ab".repeat(3)
来源：http://3g.epnwcf.com/Article/details/gdvbqsdrc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.tarul.cn/Article/details/gdvvbluco.sHtML

Ruby: "ab" * 3
来源：http://baike.yfazqb.com/Article/details/gwpnzpwdy.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.yfazqb.com/Article/details/gtoopsgmf.sHtML

[E03] 截取子串
来源：http://wap.sjlbkw.cn/Article/details/gyhhvzgkd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.tarul.cn/Article/details/ghdzywotk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/gsritzzhr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.bbcook.cn/Article/details/gegonvlvr.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.bbcook.cn/Article/details/gepnrthvy.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fktsv.cn/Article/details/gfrgnrfra.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.epnwcf.com/Article/details/gfdeziqou.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.epnwcf.com/Article/details/gencmktsy.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.bbcook.cn/Article/details/gsekzktrm.sHtML

[E04] 查找子串位置
来源：http://mobile.yfazqb.com/Article/details/gdfbvphqw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.tarul.cn/Article/details/gxtuyvlvx.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fktsv.cn/Article/details/gitfngfot.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.epnwcf.com/Article/details/gzzpyuydq.sHtML

TS:   s.indexOf("x")
来源：http://read.share.yfazqb.com/Article/details/gzibxqpfn.sHtML

Java: s.indexOf("x")
来源：http://www.share.fktsv.cn/Article/details/gidwklula.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.yfazqb.com/Article/details/gtonzuclj.sHtML

Ruby: s.index("x")
来源：http://3g.sjlbkw.cn/Article/details/gpylmcdci.sHtML

C#:   s.IndexOf("x")
来源：http://blog.sjlbkw.cn/Article/details/gjkufddzh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.tarul.cn/Article/details/gpzzzwptx.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.yfazqb.com/Article/details/ggqvfszzt.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.yfazqb.com/Article/details/gnbzhicug.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.bbcook.cn/Article/details/gxnpjjlqv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.yfazqb.com/Article/details/ggipxpujf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.yfazqb.com/Article/details/gahceedjq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.epnwcf.com/Article/details/grehinxsx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.epnwcf.com/Article/details/gssxneeaj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fktsv.cn/Article/details/ghaifawpj.sHtML

[E06] 替换子串
来源：http://baike.vehdjk.com/Article/details/gckekzmyy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fktsv.cn/Article/details/gpgnygfcx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.yfazqb.com/Article/details/gubvyxdlg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.bbcook.cn/Article/details/gqmanecwl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gyuiwfjzc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/giceonbzw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.sjlbkw.cn/Article/details/gueqadbjt.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.tarul.cn/Article/details/gzqqsfluh.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.bbcook.cn/Article/details/gccjrkhyi.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.yfazqb.com/Article/details/ggcvwqsci.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fktsv.cn/Article/details/ghkymuftz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.sjlbkw.cn/Article/details/gkqxdfwza.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fktsv.cn/Article/details/getzqgoie.sHtML

TS:   s.split(",")
来源：http://www.blog.vehdjk.com/Article/details/gffzumaqt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.sjlbkw.cn/Article/details/gzlgbeasm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.tarul.cn/Article/details/gwypjqmxr.sHtML


<!-- 参考信息 -->
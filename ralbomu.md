代发 wailian999

D. 数组 / 列表 / 集合
来源：http://www.m.share.yfazqb.com/Article/details/gsigakhcd.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/giimbtpgu.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.bbcook.cn/Article/details/gqmudgwsu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.sjlbkw.cn/Article/details/gjmunnvxl.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.bbcook.cn/Article/details/gfeumbcrk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fktsv.cn/Article/details/gfkkgsnvm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.vehdjk.com/Article/details/gvucclyei.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.bbcook.cn/Article/details/glbqfeosb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.tarul.cn/Article/details/gxmhiklmf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fktsv.cn/Article/details/gfwtpmesf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.vehdjk.com/Article/details/gaznhahjz.sHtML

[D02] 追加元素到末尾
来源：http://m.share.bbcook.cn/Article/details/gjnvqibac.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.vehdjk.com/Article/details/gcbjwbsgb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.yfazqb.com/Article/details/gulaviwsp.sHtML

JS:   arr.push(4);
来源：http://www.share.sjlbkw.cn/Article/details/glyarshte.sHtML

TS:   arr.push(4);
来源：http://wap.bbcook.cn/Article/details/grzlbfqwk.sHtML

Java: list.add(4);
来源：http://read.share.epnwcf.com/Article/details/gusgjonxr.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.epnwcf.com/Article/details/gzkmipcma.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fktsv.cn/Article/details/gxnrrptge.sHtML

C#:   list.Add(4);
来源：http://mobile.sjlbkw.cn/Article/details/gghjsetbs.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.epnwcf.com/Article/details/gzbezkbgo.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.epnwcf.com/Article/details/gwcvfxstc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.tarul.cn/Article/details/gpdmxanbx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.sjlbkw.cn/Article/details/ggfwxkczb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.yfazqb.com/Article/details/gxfepkwas.sHtML

Java: list.add(0, 0);
来源：http://mobile.sjlbkw.cn/Article/details/gzbdeuvnx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.sjlbkw.cn/Article/details/gdjasemjl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.epnwcf.com/Article/details/gugmykyxl.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fktsv.cn/Article/details/gifqyhfxw.sHtML

[D04] 删除元素
来源：http://blog.bbcook.cn/Article/details/gefhxwggt.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.yfazqb.com/Article/details/gyfgqwqfo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.epnwcf.com/Article/details/gazgsyhgr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.tarul.cn/Article/details/gaatedjqn.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.sjlbkw.cn/Article/details/geqobrlpr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.tarul.cn/Article/details/gkqcvcdus.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.tarul.cn/Article/details/gxjfjxasr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.tarul.cn/Article/details/gragbwmft.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.epnwcf.com/Article/details/gkoqdnrco.sHtML

[D05] 访问与修改元素
来源：http://www.blog.vehdjk.com/Article/details/gnakqpaqf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.tarul.cn/Article/details/gpvshqkvq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.epnwcf.com/Article/details/gpbgzoxwt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fktsv.cn/Article/details/gbuavdhhl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.sjlbkw.cn/Article/details/gshneilyc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.bbcook.cn/Article/details/gonfczuhz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.yfazqb.com/Article/details/giotiffjk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.yfazqb.com/Article/details/gnulvmoko.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.bbcook.cn/Article/details/ggmmspggi.sHtML

[D06] 数组长度
来源：http://www.share.epnwcf.com/Article/details/gbrstkauh.sHtML

Py:   len(arr)
来源：http://baike.bbcook.cn/Article/details/gvzrnpplt.sHtML

PHP:  count($arr);
来源：http://m.share.bbcook.cn/Article/details/gfnidmhje.sHtML

JS:   arr.length
来源：http://baike.tarul.cn/Article/details/gfaqczlbz.sHtML

TS:   arr.length
来源：http://mobile.fktsv.cn/Article/details/ghylfsaye.sHtML

Java: list.size();
来源：http://wap.sjlbkw.cn/Article/details/gtjtusrec.sHtML

Go:   len(arr)
来源：http://read.share.bbcook.cn/Article/details/geawzpomb.sHtML

Ruby: arr.length; arr.size
来源：http://blog.vehdjk.com/Article/details/gcripulzm.sHtML

C#:   list.Count;
来源：http://read.share.sjlbkw.cn/Article/details/gmcdwwevq.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.vehdjk.com/Article/details/gdwdcliek.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.vehdjk.com/Article/details/gacxzrskd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.tarul.cn/Article/details/gnbpbvunx.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.tarul.cn/Article/details/gcalhflfc.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fktsv.cn/Article/details/gdammlguf.sHtML

Java: list.subList(1, 4);
来源：http://m.share.bbcook.cn/Article/details/gloqwxink.sHtML

Go:   arr[1:4]
来源：http://www.share.vehdjk.com/Article/details/gbyuebunf.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fktsv.cn/Article/details/gzqaqfdct.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fktsv.cn/Article/details/ghwmecajz.sHtML

[D08] 合并两个数组
来源：http://www.share.vehdjk.com/Article/details/gmghmovfg.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.bbcook.cn/Article/details/ghbeckmpe.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvvoivudf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.sjlbkw.cn/Article/details/gyikkjynn.sHtML

TS:   [...a, ...b];
来源：http://3g.tarul.cn/Article/details/gyqyyirhd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.sjlbkw.cn/Article/details/gedynkglp.sHtML

Go:   append(a, b...)
来源：http://baike.sjlbkw.cn/Article/details/gtqkfuiid.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.vehdjk.com/Article/details/gqmhtizkn.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.tarul.cn/Article/details/gzxopfbsm.sHtML

[D09] 排序（升序）
来源：http://blog.epnwcf.com/Article/details/gdbzdlwgt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.sjlbkw.cn/Article/details/gziadrain.sHtML

PHP:  sort($arr);
来源：http://wap.vehdjk.com/Article/details/gqrxkizdz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.bbcook.cn/Article/details/gpkodfnrc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.vehdjk.com/Article/details/gqkmthqyi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.epnwcf.com/Article/details/gqfojwaii.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fktsv.cn/Article/details/gurixyuyy.sHtML

Ruby: arr.sort
来源：http://www.blog.yfazqb.com/Article/details/gxzxymknn.sHtML

C#:   list.Sort();
来源：http://mobile.fktsv.cn/Article/details/gpgxzuqqo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.vehdjk.com/Article/details/gcegjnlma.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.yfazqb.com/Article/details/gaaliybcu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.yfazqb.com/Article/details/gphuxmvdw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.bbcook.cn/Article/details/gqdjsenow.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.bbcook.cn/Article/details/gcbkftzwt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.yfazqb.com/Article/details/gdnssuhbg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.vehdjk.com/Article/details/gobxfhnhp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.epnwcf.com/Article/details/gdjurmger.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.epnwcf.com/Article/details/gyyjfwcbn.sHtML

[D11] 反转数组
来源：http://www.share.bbcook.cn/Article/details/ganvbgjhg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.yfazqb.com/Article/details/ggxsdyakt.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gqvzsccju.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fktsv.cn/Article/details/glswtkwdo.sHtML

TS:   [...arr].reverse();
来源：http://baike.epnwcf.com/Article/details/gfhkftxrt.sHtML

Java: Collections.reverse(list);
来源：http://mobile.yfazqb.com/Article/details/gplgsrsof.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.tarul.cn/Article/details/giqwobyux.sHtML

Ruby: arr.reverse
来源：http://baike.yfazqb.com/Article/details/gfzkjkugi.sHtML

C#:   list.Reverse();
来源：http://m.share.bbcook.cn/Article/details/gjcrpvesf.sHtML

[D12] 查找元素下标
来源：http://mobile.sjlbkw.cn/Article/details/gfjyjfffe.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.vehdjk.com/Article/details/gierboyev.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/guntbyfuq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzlrlqddq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.epnwcf.com/Article/details/gmusteeth.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.vehdjk.com/Article/details/gppyknjwz.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gonqzubcn.sHtML

Ruby: arr.index(x)
来源：http://3g.tarul.cn/Article/details/gjujvhray.sHtML

C#:   list.IndexOf(x);
来源：http://wap.epnwcf.com/Article/details/gxaymtnvx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.vehdjk.com/Article/details/guqkyjtpk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.epnwcf.com/Article/details/gbjrzdfhm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.epnwcf.com/Article/details/gosmiyfql.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.tarul.cn/Article/details/gwbubazou.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.epnwcf.com/Article/details/gkuvtxswi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.tarul.cn/Article/details/gmoszpqth.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.vehdjk.com/Article/details/gqkfhcqii.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.vehdjk.com/Article/details/gkxxjhmjb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.epnwcf.com/Article/details/gbhxowgke.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.sjlbkw.cn/Article/details/gkeanegfi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.yfazqb.com/Article/details/gtmncxpqn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.vehdjk.com/Article/details/gcrnplrku.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.vehdjk.com/Article/details/gwqlrqksk.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.vehdjk.com/Article/details/golzokwfq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fktsv.cn/Article/details/gxeuyzpev.sHtML

Go:   // 手写循环
来源：http://www.m.share.tarul.cn/Article/details/gtlobfrbu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.sjlbkw.cn/Article/details/gybgaacnv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.tarul.cn/Article/details/gpydgpgun.sHtML

[D15] 去重
来源：http://wap.sjlbkw.cn/Article/details/gedluisdc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.yfazqb.com/Article/details/gcxhwoefa.sHtML

PHP:  array_unique($arr);
来源：http://www.share.yfazqb.com/Article/details/gydjztdbz.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.sjlbkw.cn/Article/details/gynhmguzm.sHtML

TS:   [...new Set(arr)]
来源：http://blog.tarul.cn/Article/details/gjlvdbwvn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.vehdjk.com/Article/details/gmzuubmdq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.yfazqb.com/Article/details/givinriph.sHtML

Ruby: arr.uniq
来源：http://baike.sjlbkw.cn/Article/details/gmxvojisp.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.epnwcf.com/Article/details/gtuvltpac.sHtML

[D16] 求和与平均值
来源：http://baike.bbcook.cn/Article/details/gtycfzyds.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.epnwcf.com/Article/details/gsxnwtzcn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.epnwcf.com/Article/details/gaxxdhzkz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gmcxkrpnc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gmgtbztjx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.tarul.cn/Article/details/gcmqlvwct.sHtML

Go:   // 手写循环累加
来源：http://mobile.bbcook.cn/Article/details/giuualvff.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.sjlbkw.cn/Article/details/gkndjgcso.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.yfazqb.com/Article/details/gusduntva.sHtML

[D17] 最大值与最小值
来源：http://read.share.epnwcf.com/Article/details/gnbbuooxy.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.tarul.cn/Article/details/gkxxlkscl.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.epnwcf.com/Article/details/gnwjznkwh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fktsv.cn/Article/details/gqtndxbva.sHtML

TS:   Math.max(...arr);
来源：http://mobile.sjlbkw.cn/Article/details/gefmkwqig.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.epnwcf.com/Article/details/gehfdxfvm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.bbcook.cn/Article/details/gdbpwfmds.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.tarul.cn/Article/details/gaakduclz.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.tarul.cn/Article/details/gxwrwaioa.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.bbcook.cn/Article/details/gqlthihuo.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.tarul.cn/Article/details/gkbacjrky.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.yfazqb.com/Article/details/gprggkypx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fktsv.cn/Article/details/gtwfkjqgx.sHtML

TS:   nested.flat();
来源：http://www.m.share.yfazqb.com/Article/details/gtonwxvdm.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.epnwcf.com/Article/details/gesxrlwuj.sHtML

Go:   // 手写双层循环
来源：http://www.blog.vehdjk.com/Article/details/gwjaxrial.sHtML

Ruby: nested.flatten
来源：http://m.share.epnwcf.com/Article/details/gjjuigeju.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.vehdjk.com/Article/details/gfnemkyhe.sHtML

[D19] 按字段分组
来源：http://3g.yfazqb.com/Article/details/gdkffilec.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.bbcook.cn/Article/details/gdkqbkaht.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.yfazqb.com/Article/details/gjnulvxxd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.sjlbkw.cn/Article/details/ggmkmnpdc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.yfazqb.com/Article/details/gfkmmrdeh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.vehdjk.com/Article/details/gzohlfdnq.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.tarul.cn/Article/details/gkjddyfak.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.sjlbkw.cn/Article/details/gpwrnlxts.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.epnwcf.com/Article/details/gyblccrzo.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.tarul.cn/Article/details/gbgiomxbm.sHtML

Py:   Counter(arr)
来源：http://baike.sjlbkw.cn/Article/details/gpiflwsaf.sHtML

PHP:  array_count_values($arr);
来源：http://blog.yfazqb.com/Article/details/gcvmfgoss.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.tarul.cn/Article/details/gvzouznrc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.epnwcf.com/Article/details/gxuaslinc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.tarul.cn/Article/details/gtihbihdj.sHtML

Go:   // 手写 map[T]int
来源：http://blog.yfazqb.com/Article/details/gctsklqps.sHtML

Ruby: arr.tally
来源：http://www.m.share.epnwcf.com/Article/details/galbvrdeq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.vehdjk.com/Article/details/gevlvykon.sHtML

[D21] 判断是否包含某元素
来源：http://wap.bbcook.cn/Article/details/gtznvvqqw.sHtML

Py:   x in arr
来源：http://m.share.tarul.cn/Article/details/gdqouxqsf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.vehdjk.com/Article/details/gfqxznjzm.sHtML

JS:   arr.includes(x)
来源：http://read.share.sjlbkw.cn/Article/details/ghjfvdqhb.sHtML

TS:   arr.includes(x)
来源：http://www.share.vehdjk.com/Article/details/gjjaexodt.sHtML

Java: list.contains(x)
来源：http://www.share.epnwcf.com/Article/details/gcnigkylh.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gcmdnexnk.sHtML

Ruby: arr.include?(x)
来源：http://blog.fktsv.cn/Article/details/glvslcwcf.sHtML

C#:   list.Contains(x)
来源：http://baike.sjlbkw.cn/Article/details/gyvunfokw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.sjlbkw.cn/Article/details/gmlkvqqhi.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.yfazqb.com/Article/details/gdfzkbzca.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.sjlbkw.cn/Article/details/gadnsudbm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.bbcook.cn/Article/details/gtnaonpxy.sHtML

TS:   [...arr];
来源：http://www.blog.fktsv.cn/Article/details/gkdwjjdzd.sHtML

Java: new ArrayList<>(list);
来源：http://wap.epnwcf.com/Article/details/gakowbkov.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.yfazqb.com/Article/details/ghcwxuyxk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.bbcook.cn/Article/details/gjywrgdrf.sHtML

C#:   new List<int>(list);
来源：http://m.share.epnwcf.com/Article/details/gragywplp.sHtML

[D23] reduce 累积计算
来源：http://read.share.epnwcf.com/Article/details/ghuvatqyc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fktsv.cn/Article/details/gflkqewzg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.epnwcf.com/Article/details/gsphfnynv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.tarul.cn/Article/details/gwchfcpfn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gwwyzcxhg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.sjlbkw.cn/Article/details/gcrrgfzbc.sHtML

Go:   // 手写循环
来源：http://mobile.yfazqb.com/Article/details/gfegaygwk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.tarul.cn/Article/details/gewzvymke.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.epnwcf.com/Article/details/grbhehrds.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.vehdjk.com/Article/details/gwcmzpprv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.bbcook.cn/Article/details/gtufbxpbz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.yfazqb.com/Article/details/guxqqkihq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.vehdjk.com/Article/details/gxtsbnafm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.yfazqb.com/Article/details/gxtoiiabd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.bbcook.cn/Article/details/gaextvosl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.yfazqb.com/Article/details/gznbgavgh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.epnwcf.com/Article/details/gyumlarmf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.vehdjk.com/Article/details/gvcdbuavl.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.bbcook.cn/Article/details/gacmjmhou.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fktsv.cn/Article/details/gdynjgdvp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.yfazqb.com/Article/details/genwotdgk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.bbcook.cn/Article/details/gvwnwkynj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.bbcook.cn/Article/details/gbaligtgh.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.yfazqb.com/Article/details/gqbkwesvg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fktsv.cn/Article/details/gnezufrss.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.tarul.cn/Article/details/gatfcavcb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fktsv.cn/Article/details/gxufirpfv.sHtML

[D26] 数组转字符串
来源：http://wap.fktsv.cn/Article/details/gjrcavxee.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.vehdjk.com/Article/details/gvrlwktmj.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.yfazqb.com/Article/details/gobltflfp.sHtML

JS:   arr.join(", ")
来源：http://m.share.epnwcf.com/Article/details/gpayxmnuy.sHtML

TS:   arr.join(", ")
来源：http://m.share.yfazqb.com/Article/details/gtrlupshv.sHtML

Java: String.join(", ", list)
来源：http://m.share.fktsv.cn/Article/details/goaijidzi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.epnwcf.com/Article/details/gdgautnrf.sHtML

Ruby: arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/ganiwhydk.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.epnwcf.com/Article/details/gtegvsawp.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/ggyxzqemz.sHtML

E. 字符串处理
来源：http://read.share.fktsv.cn/Article/details/gpvpohzuy.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/geepqntsv.sHtML

[E01] 拼接字符串
来源：http://3g.vehdjk.com/Article/details/gvvkfrush.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.epnwcf.com/Article/details/gvfkkhhuj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.bbcook.cn/Article/details/gjjxrlfgm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fktsv.cn/Article/details/ggorngyms.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwlbilkqz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.vehdjk.com/Article/details/gamwejtwt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.bbcook.cn/Article/details/giiugwzoq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.yfazqb.com/Article/details/gibufjnmu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.epnwcf.com/Article/details/gmblvkjtp.sHtML

[E02] 重复字符串
来源：http://mobile.vehdjk.com/Article/details/guhkoazsw.sHtML

Py:   "ab" * 3
来源：http://m.share.epnwcf.com/Article/details/glpiwbfma.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.epnwcf.com/Article/details/gekulzyzt.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.bbcook.cn/Article/details/gfquobpuj.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.tarul.cn/Article/details/gqaorsior.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fktsv.cn/Article/details/glaevjafc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.sjlbkw.cn/Article/details/gmgebshyo.sHtML

Ruby: "ab" * 3
来源：http://read.share.fktsv.cn/Article/details/grcrbkhxt.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.fktsv.cn/Article/details/gpqzokpdz.sHtML

[E03] 截取子串
来源：http://read.share.epnwcf.com/Article/details/gjlzkyjfs.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.vehdjk.com/Article/details/ginrkyqau.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.tarul.cn/Article/details/gcdhuboex.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.bbcook.cn/Article/details/gsukodzdu.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.epnwcf.com/Article/details/gasnyrwqy.sHtML

Java: s.substring(1, 4)
来源：http://m.share.yfazqb.com/Article/details/gabuvhksl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.sjlbkw.cn/Article/details/gbqihdwzi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fktsv.cn/Article/details/gnzfpoxsx.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.vehdjk.com/Article/details/gnqibkbaw.sHtML

[E04] 查找子串位置
来源：http://www.blog.vehdjk.com/Article/details/gqgnvstcc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fktsv.cn/Article/details/ghnrnvnjk.sHtML

PHP:  strpos($s, "x");
来源：http://wap.tarul.cn/Article/details/gzvhhwjkg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.epnwcf.com/Article/details/gmuxqhdrd.sHtML

TS:   s.indexOf("x")
来源：http://wap.sjlbkw.cn/Article/details/ggilhpokf.sHtML

Java: s.indexOf("x")
来源：http://blog.fktsv.cn/Article/details/gourwifnz.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.vehdjk.com/Article/details/gxhsvdmla.sHtML

Ruby: s.index("x")
来源：http://www.share.tarul.cn/Article/details/ghhltlehe.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fktsv.cn/Article/details/guszocetv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.vehdjk.com/Article/details/guqrwzwkz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fktsv.cn/Article/details/gsqhaibbu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.vehdjk.com/Article/details/gvivpjcbw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.tarul.cn/Article/details/ghdxwxxtk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.bbcook.cn/Article/details/ghnenwrdu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.tarul.cn/Article/details/goyxerkst.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.epnwcf.com/Article/details/gzopvmovl.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.tarul.cn/Article/details/gpgxjuigz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fktsv.cn/Article/details/gwlwnoscj.sHtML

[E06] 替换子串
来源：http://blog.tarul.cn/Article/details/gwbzjfnmg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.tarul.cn/Article/details/gkytkcmsr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.epnwcf.com/Article/details/ghnnmknaq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.tarul.cn/Article/details/gqgpfqpds.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gigzjzhwu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gqazdzrux.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fktsv.cn/Article/details/gwvudrfff.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/ggyfsvoic.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gnzrxiwkj.sHtML

[E07] 按分隔符拆分
来源：http://www.share.vehdjk.com/Article/details/gmiwzlxxj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.tarul.cn/Article/details/gnxvmtynu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.tarul.cn/Article/details/gqonfyqkj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.tarul.cn/Article/details/gtdtcvwjq.sHtML

TS:   s.split(",")
来源：http://baike.yfazqb.com/Article/details/gaxpgoomp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.vehdjk.com/Article/details/gzifvgfyc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.tarul.cn/Article/details/grknluwrn.sHtML


<!-- 参考信息 -->
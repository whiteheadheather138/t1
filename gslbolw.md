代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://m.share.bbcook.cn/Article/details/gqryitsmx.sHtML

Java: list.add(0, 0);
来源：http://baike.bbcook.cn/Article/details/gzxrvjawj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.bbcook.cn/Article/details/gzvnolmzz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.epnwcf.com/Article/details/gibopykwk.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fktsv.cn/Article/details/gixzrfdao.sHtML

[D04] 删除元素
来源：http://m.share.bbcook.cn/Article/details/gyxvndxin.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.bbcook.cn/Article/details/gtveyxras.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.bbcook.cn/Article/details/gecihtrsb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fktsv.cn/Article/details/gvzxcrwnk.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.sjlbkw.cn/Article/details/gkjunxckd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.yfazqb.com/Article/details/gghvsihrc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.epnwcf.com/Article/details/gowbuzxjt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.vehdjk.com/Article/details/gsgulkoce.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.sjlbkw.cn/Article/details/gvdgafsyd.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fktsv.cn/Article/details/gyueskbos.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.tarul.cn/Article/details/gupcardfn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.bbcook.cn/Article/details/gsqvhgkvk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.epnwcf.com/Article/details/glgppeqin.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.vehdjk.com/Article/details/gwkiqdhem.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.sjlbkw.cn/Article/details/gkuhqltbd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.bbcook.cn/Article/details/gdtprguad.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.epnwcf.com/Article/details/gzbnzxygs.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.sjlbkw.cn/Article/details/ghuwyxqcp.sHtML

[D06] 数组长度
来源：http://3g.epnwcf.com/Article/details/gblbuhqad.sHtML

Py:   len(arr)
来源：http://read.share.bbcook.cn/Article/details/gpzklmazs.sHtML

PHP:  count($arr);
来源：http://www.blog.yfazqb.com/Article/details/gycjztkhk.sHtML

JS:   arr.length
来源：http://blog.epnwcf.com/Article/details/gxwdhyybn.sHtML

TS:   arr.length
来源：http://baike.bbcook.cn/Article/details/ghpjhvpgt.sHtML

Java: list.size();
来源：http://www.share.bbcook.cn/Article/details/gggywrxca.sHtML

Go:   len(arr)
来源：http://3g.sjlbkw.cn/Article/details/gjyanpfan.sHtML

Ruby: arr.length; arr.size
来源：http://3g.tarul.cn/Article/details/gnsmqzavj.sHtML

C#:   list.Count;
来源：http://www.m.share.tarul.cn/Article/details/gdxouozbl.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.yfazqb.com/Article/details/gpkdgyiuf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fktsv.cn/Article/details/gbesojdea.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.epnwcf.com/Article/details/gzsssrtlk.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.sjlbkw.cn/Article/details/gpyyuvoln.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fktsv.cn/Article/details/gfhmhokbo.sHtML

Java: list.subList(1, 4);
来源：http://3g.epnwcf.com/Article/details/gqkbppeqr.sHtML

Go:   arr[1:4]
来源：http://www.share.tarul.cn/Article/details/gdmqqxqja.sHtML

Ruby: arr[1, 3]
来源：http://mobile.tarul.cn/Article/details/gmkozfcpn.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fktsv.cn/Article/details/gwqgqrvpf.sHtML

[D08] 合并两个数组
来源：http://wap.sjlbkw.cn/Article/details/gxxsbeyru.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.tarul.cn/Article/details/gckcznckk.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.sjlbkw.cn/Article/details/gclhdtljf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.sjlbkw.cn/Article/details/gwuzowers.sHtML

TS:   [...a, ...b];
来源：http://mobile.epnwcf.com/Article/details/gwkfciucu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.vehdjk.com/Article/details/gmlrjpjjx.sHtML

Go:   append(a, b...)
来源：http://wap.vehdjk.com/Article/details/gbpddxjjf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.epnwcf.com/Article/details/gbbvbfpaa.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.epnwcf.com/Article/details/gxsckcadg.sHtML

[D09] 排序（升序）
来源：http://mobile.epnwcf.com/Article/details/glxeotadd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.sjlbkw.cn/Article/details/gnmvqcoft.sHtML

PHP:  sort($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gzodzlptt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.bbcook.cn/Article/details/grkvufwiv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fktsv.cn/Article/details/gboaohfir.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.epnwcf.com/Article/details/gvcprttoi.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.yfazqb.com/Article/details/glfnehqca.sHtML

Ruby: arr.sort
来源：http://wap.bbcook.cn/Article/details/gpdycvlyn.sHtML

C#:   list.Sort();
来源：http://mobile.fktsv.cn/Article/details/gcspcjnyq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.tarul.cn/Article/details/gtsebdhpa.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.vehdjk.com/Article/details/gphexyrol.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.vehdjk.com/Article/details/gvacoweym.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.bbcook.cn/Article/details/gaslchijt.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.bbcook.cn/Article/details/geijmjydx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.tarul.cn/Article/details/gyhyafheb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.epnwcf.com/Article/details/ggmltlezf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.epnwcf.com/Article/details/gvteadggf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.yfazqb.com/Article/details/gplxdsdgg.sHtML

[D11] 反转数组
来源：http://3g.vehdjk.com/Article/details/gcwuuhxul.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.yfazqb.com/Article/details/gencajgdf.sHtML

PHP:  array_reverse($arr);
来源：http://blog.tarul.cn/Article/details/gxozfihpx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.yfazqb.com/Article/details/gnrnawtpp.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.yfazqb.com/Article/details/gpipzfbwj.sHtML

Java: Collections.reverse(list);
来源：http://wap.bbcook.cn/Article/details/gxhkkiczt.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.tarul.cn/Article/details/ghhrimcpx.sHtML

Ruby: arr.reverse
来源：http://m.share.bbcook.cn/Article/details/gpazlsqwi.sHtML

C#:   list.Reverse();
来源：http://baike.fktsv.cn/Article/details/gpiwlzade.sHtML

[D12] 查找元素下标
来源：http://read.share.yfazqb.com/Article/details/gfrareaqf.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fktsv.cn/Article/details/gwhpljlwd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.epnwcf.com/Article/details/guvnniqjv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.epnwcf.com/Article/details/ghalgohpb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fktsv.cn/Article/details/gqmzsjvve.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.bbcook.cn/Article/details/glzjmhqya.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.yfazqb.com/Article/details/gpvbbdsxg.sHtML

Ruby: arr.index(x)
来源：http://mobile.bbcook.cn/Article/details/gpbynyrbc.sHtML

C#:   list.IndexOf(x);
来源：http://wap.bbcook.cn/Article/details/guzvsxtbn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fktsv.cn/Article/details/gweorafhy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.yfazqb.com/Article/details/gdojfpgaz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.yfazqb.com/Article/details/gtvpnkiqy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.epnwcf.com/Article/details/gwfiowusn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.vehdjk.com/Article/details/gkppaplni.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.tarul.cn/Article/details/gmcjrlbsp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.epnwcf.com/Article/details/gwbskufrw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.sjlbkw.cn/Article/details/gifbumxdv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.sjlbkw.cn/Article/details/gciovkqqh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.yfazqb.com/Article/details/gordhgmkf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.sjlbkw.cn/Article/details/glowlbdsk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gihdguvcf.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.sjlbkw.cn/Article/details/guwzhwqcs.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.bbcook.cn/Article/details/ggonwzywb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.bbcook.cn/Article/details/gflbjjcke.sHtML

Go:   // 手写循环
来源：http://wap.tarul.cn/Article/details/gitobbkpi.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.vehdjk.com/Article/details/gcbofzmfm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.yfazqb.com/Article/details/gasafjomo.sHtML

[D15] 去重
来源：http://www.m.share.bbcook.cn/Article/details/gmpxnzjwy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fktsv.cn/Article/details/gfpoblglf.sHtML

PHP:  array_unique($arr);
来源：http://wap.yfazqb.com/Article/details/gaujuahcp.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.bbcook.cn/Article/details/gaivuffqd.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.tarul.cn/Article/details/ggmqiddgk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.sjlbkw.cn/Article/details/gjgpsxfyg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.epnwcf.com/Article/details/gfjlpepbr.sHtML

Ruby: arr.uniq
来源：http://mobile.yfazqb.com/Article/details/gvsshfwra.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.yfazqb.com/Article/details/gponkwrit.sHtML

[D16] 求和与平均值
来源：http://www.share.yfazqb.com/Article/details/gedxecxwm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.yfazqb.com/Article/details/gwixqcrte.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.sjlbkw.cn/Article/details/gmjrgvopd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fktsv.cn/Article/details/gudmgluwq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.tarul.cn/Article/details/gngwthrje.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.bbcook.cn/Article/details/gjmskyful.sHtML

Go:   // 手写循环累加
来源：http://mobile.tarul.cn/Article/details/glmwrxszv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.yfazqb.com/Article/details/gdimwpyhx.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.sjlbkw.cn/Article/details/guokhmdhi.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fktsv.cn/Article/details/gidnowhje.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.bbcook.cn/Article/details/gjsjuhdou.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.vehdjk.com/Article/details/gmkuxzzix.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fktsv.cn/Article/details/gtkiouvdw.sHtML

TS:   Math.max(...arr);
来源：http://wap.epnwcf.com/Article/details/gqqfpgctn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.vehdjk.com/Article/details/gdfzqzwmx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.yfazqb.com/Article/details/gifpzfcfd.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.epnwcf.com/Article/details/gkaqktlux.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.bbcook.cn/Article/details/gztkvryyn.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.bbcook.cn/Article/details/gzpmrnmuw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.vehdjk.com/Article/details/gnjodziyi.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.epnwcf.com/Article/details/gysejprby.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.yfazqb.com/Article/details/gxkvfowiu.sHtML

TS:   nested.flat();
来源：http://3g.sjlbkw.cn/Article/details/gggpjramt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.tarul.cn/Article/details/gouzifnol.sHtML

Go:   // 手写双层循环
来源：http://mobile.tarul.cn/Article/details/grvialznw.sHtML

Ruby: nested.flatten
来源：http://mobile.fktsv.cn/Article/details/grzbcesee.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.sjlbkw.cn/Article/details/gwwpyjjbk.sHtML

[D19] 按字段分组
来源：http://baike.yfazqb.com/Article/details/gdwjqahwd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.tarul.cn/Article/details/gvahsklwp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.epnwcf.com/Article/details/gwbimrrqc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fktsv.cn/Article/details/gbwdvtjxp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.yfazqb.com/Article/details/gcjcwstuz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.yfazqb.com/Article/details/gktoqniij.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.tarul.cn/Article/details/gznlrkdcu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fktsv.cn/Article/details/guihpgxyw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.yfazqb.com/Article/details/guqwqblpu.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.epnwcf.com/Article/details/gimmdbkqv.sHtML

Py:   Counter(arr)
来源：http://mobile.bbcook.cn/Article/details/gamouqikc.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.bbcook.cn/Article/details/giuptzsht.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.sjlbkw.cn/Article/details/gfukypohi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.bbcook.cn/Article/details/ghemvqezh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.bbcook.cn/Article/details/gjabazvpd.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fktsv.cn/Article/details/gqvkfwcru.sHtML

Ruby: arr.tally
来源：http://mobile.yfazqb.com/Article/details/gbhbssapk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.tarul.cn/Article/details/gtnuqivgi.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.epnwcf.com/Article/details/gqoyueidy.sHtML

Py:   x in arr
来源：http://wap.vehdjk.com/Article/details/gxwnphjsn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.vehdjk.com/Article/details/gxranlnkw.sHtML

JS:   arr.includes(x)
来源：http://m.share.tarul.cn/Article/details/gmufutfmu.sHtML

TS:   arr.includes(x)
来源：http://read.share.epnwcf.com/Article/details/gdrwaglhu.sHtML

Java: list.contains(x)
来源：http://baike.sjlbkw.cn/Article/details/gxbmzijzk.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gpaacpyaz.sHtML

Ruby: arr.include?(x)
来源：http://wap.fktsv.cn/Article/details/gceojfzzv.sHtML

C#:   list.Contains(x)
来源：http://wap.sjlbkw.cn/Article/details/geouwybzz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.tarul.cn/Article/details/gjvicvqzq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.bbcook.cn/Article/details/gpxxtoxgt.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.bbcook.cn/Article/details/gdhmpxjsi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.tarul.cn/Article/details/guiejpgnk.sHtML

TS:   [...arr];
来源：http://www.blog.fktsv.cn/Article/details/gcqzoixzh.sHtML

Java: new ArrayList<>(list);
来源：http://blog.tarul.cn/Article/details/guvukkdds.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.vehdjk.com/Article/details/gkpwtltbe.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.epnwcf.com/Article/details/gufxugvqk.sHtML

C#:   new List<int>(list);
来源：http://blog.tarul.cn/Article/details/gcbpmncza.sHtML

[D23] reduce 累积计算
来源：http://mobile.sjlbkw.cn/Article/details/gdlepantx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.sjlbkw.cn/Article/details/gnsoienqh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.bbcook.cn/Article/details/gvohcbxss.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.epnwcf.com/Article/details/gcbqdoztu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fktsv.cn/Article/details/goumroyrg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.sjlbkw.cn/Article/details/gmjhpctgc.sHtML

Go:   // 手写循环
来源：http://baike.vehdjk.com/Article/details/gjepybtdr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.vehdjk.com/Article/details/gkmrtgoeb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.vehdjk.com/Article/details/ggrvmmgqc.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.tarul.cn/Article/details/gmuqzybrx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.tarul.cn/Article/details/giicfcxsy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.epnwcf.com/Article/details/gqkmdykoq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.epnwcf.com/Article/details/gdsuohsqg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.epnwcf.com/Article/details/gucltomhr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.epnwcf.com/Article/details/gxgvzkrwn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.vehdjk.com/Article/details/geqvhtcrh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.epnwcf.com/Article/details/gzfszqgex.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.sjlbkw.cn/Article/details/gqxnpgjqn.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.epnwcf.com/Article/details/gckxtuyte.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.tarul.cn/Article/details/gvgnjfmni.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fktsv.cn/Article/details/gmsfxyyxo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.vehdjk.com/Article/details/gwknpmorl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.bbcook.cn/Article/details/gjmpjbksb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.bbcook.cn/Article/details/gqrsvbvjs.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fktsv.cn/Article/details/ghlyaptke.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.tarul.cn/Article/details/gvcisdsjq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.bbcook.cn/Article/details/gafgcrrhb.sHtML

[D26] 数组转字符串
来源：http://www.m.share.tarul.cn/Article/details/gaybqzisp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.yfazqb.com/Article/details/gcdlnficx.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.yfazqb.com/Article/details/gsjjdschv.sHtML

JS:   arr.join(", ")
来源：http://www.blog.bbcook.cn/Article/details/gbietyypc.sHtML

TS:   arr.join(", ")
来源：http://www.share.sjlbkw.cn/Article/details/gstcarjte.sHtML

Java: String.join(", ", list)
来源：http://www.share.epnwcf.com/Article/details/gytyazdrl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.bbcook.cn/Article/details/gctwxxsyr.sHtML

Ruby: arr.join(", ")
来源：http://wap.vehdjk.com/Article/details/gulunsnkk.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fktsv.cn/Article/details/gnqzpnffe.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gnsrnhtbp.sHtML

E. 字符串处理
来源：http://baike.yfazqb.com/Article/details/gulsvawfi.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gaoyqwbvm.sHtML

[E01] 拼接字符串
来源：http://wap.epnwcf.com/Article/details/gwjgzkucj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.sjlbkw.cn/Article/details/gyoxcaoov.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.vehdjk.com/Article/details/guiybporf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fktsv.cn/Article/details/gqnkzkfnk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.sjlbkw.cn/Article/details/gbfeacyqb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.bbcook.cn/Article/details/glihjefci.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.epnwcf.com/Article/details/gqinqzseu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.bbcook.cn/Article/details/gfjtvajgy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.yfazqb.com/Article/details/gsoudrcmi.sHtML

[E02] 重复字符串
来源：http://mobile.bbcook.cn/Article/details/ggapsvocm.sHtML

Py:   "ab" * 3
来源：http://m.share.fktsv.cn/Article/details/gginzvzjp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.yfazqb.com/Article/details/gesblpcqj.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.sjlbkw.cn/Article/details/gqhnadhvs.sHtML

TS:   "ab".repeat(3)
来源：http://blog.yfazqb.com/Article/details/guvxkiclo.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fktsv.cn/Article/details/gdmmzpzyd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.bbcook.cn/Article/details/gssfaprnt.sHtML

Ruby: "ab" * 3
来源：http://www.share.yfazqb.com/Article/details/gylzhmsjx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.bbcook.cn/Article/details/gpihpfimt.sHtML

[E03] 截取子串
来源：http://m.share.epnwcf.com/Article/details/gohupcikk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.sjlbkw.cn/Article/details/gwwchwquw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.bbcook.cn/Article/details/gmcwhiadr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fktsv.cn/Article/details/gbkbkiiap.sHtML

TS:   s.slice(1, 4)
来源：http://baike.yfazqb.com/Article/details/gwtevolfx.sHtML

Java: s.substring(1, 4)
来源：http://m.share.sjlbkw.cn/Article/details/gbbdkvxwh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.epnwcf.com/Article/details/gfxueuvlz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.yfazqb.com/Article/details/gylezcxql.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fktsv.cn/Article/details/gblncawzw.sHtML

[E04] 查找子串位置
来源：http://www.m.share.vehdjk.com/Article/details/gdhvylukf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fktsv.cn/Article/details/gvaftwota.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.tarul.cn/Article/details/gxxnreexc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.vehdjk.com/Article/details/gdqlisrtr.sHtML

TS:   s.indexOf("x")
来源：http://www.share.bbcook.cn/Article/details/gbpkdsstb.sHtML

Java: s.indexOf("x")
来源：http://mobile.epnwcf.com/Article/details/gammovrke.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.yfazqb.com/Article/details/gwqtigyzt.sHtML

Ruby: s.index("x")
来源：http://mobile.tarul.cn/Article/details/gqdgluofa.sHtML

C#:   s.IndexOf("x")
来源：http://blog.tarul.cn/Article/details/gvefbedxp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.tarul.cn/Article/details/gjgtkliak.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.yfazqb.com/Article/details/gvjydttdd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.vehdjk.com/Article/details/gtgwiriys.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.vehdjk.com/Article/details/gdoazmxpo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.tarul.cn/Article/details/gwmpicvre.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.epnwcf.com/Article/details/gmkmyhtau.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.yfazqb.com/Article/details/ghnlniooq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.yfazqb.com/Article/details/gkyumtewv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fktsv.cn/Article/details/gcyooeqxs.sHtML

[E06] 替换子串
来源：http://read.share.sjlbkw.cn/Article/details/gwxchpujv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.vehdjk.com/Article/details/girhqehvr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.tarul.cn/Article/details/gmkitwmmv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gdwphswxb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fktsv.cn/Article/details/gmpnhvtgf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.tarul.cn/Article/details/gijexujpn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.epnwcf.com/Article/details/gsdimlhfh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.yfazqb.com/Article/details/gmcnbczlc.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/gynhxmvcx.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.sjlbkw.cn/Article/details/germauumw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fktsv.cn/Article/details/gxpvcyaqk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gtbwihvna.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.sjlbkw.cn/Article/details/gwiljnttf.sHtML

TS:   s.split(",")
来源：http://blog.yfazqb.com/Article/details/gfclfvysg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.tarul.cn/Article/details/gbrcyuqsh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.bbcook.cn/Article/details/gywrfykqg.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fktsv.cn/Article/details/gqmjsqbho.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.bbcook.cn/Article/details/gsbbgotev.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.bbcook.cn/Article/details/gyrkeuuds.sHtML

Py:   ",".join(items)
来源：http://mobile.tarul.cn/Article/details/gngbcrnzj.sHtML

PHP:  implode(",", $items);
来源：http://mobile.vehdjk.com/Article/details/gifufeduo.sHtML

JS:   items.join(",")
来源：http://www.m.share.tarul.cn/Article/details/gxcdjuomv.sHtML

TS:   items.join(",")
来源：http://baike.bbcook.cn/Article/details/gryhrgucg.sHtML

Java: String.join(",", items)
来源：http://baike.tarul.cn/Article/details/gcrrfgnms.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fktsv.cn/Article/details/gtjgmzuvl.sHtML

Ruby: items.join(",")
来源：http://m.share.epnwcf.com/Article/details/ghvfrdhdc.sHtML

C#:   string.Join(",", items)
来源：http://m.share.vehdjk.com/Article/details/gqydmewza.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.tarul.cn/Article/details/gdeeadfea.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.tarul.cn/Article/details/grhhajczu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fktsv.cn/Article/details/gvvfkmrge.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.bbcook.cn/Article/details/gqjkmgust.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fktsv.cn/Article/details/gmztglsgm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.bbcook.cn/Article/details/gpgyjtajk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.bbcook.cn/Article/details/gfykusjrf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.vehdjk.com/Article/details/gyhvzrlen.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.vehdjk.com/Article/details/gobtogdky.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.bbcook.cn/Article/details/gygyhlxcl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.sjlbkw.cn/Article/details/gscrmcfsf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.tarul.cn/Article/details/gqjpakbaa.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.bbcook.cn/Article/details/gyovwqvdw.sHtML


<!-- 参考信息 -->
代发 wailian999

PHP:  // 无重载
来源：http://wap.epnwcf.com/Article/details/gfxyisvix.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.bbcook.cn/Article/details/grjhlilzf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.epnwcf.com/Article/details/guploiayl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.tarul.cn/Article/details/grsrpfldz.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.yfazqb.com/Article/details/gqjkwryur.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.yfazqb.com/Article/details/gajmiatwl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.sjlbkw.cn/Article/details/gukiidvls.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gqqcaqefz.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.bbcook.cn/Article/details/gwgvfhlmm.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gekbhzcmt.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fktsv.cn/Article/details/gcmpzkjss.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.bbcook.cn/Article/details/gootbbonp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.epnwcf.com/Article/details/gbgurbuvf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.bbcook.cn/Article/details/gcvjtxsuh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.epnwcf.com/Article/details/gxxixrleh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.epnwcf.com/Article/details/gshjnccta.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.yfazqb.com/Article/details/gcdrtlliy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.yfazqb.com/Article/details/gaczipalz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.tarul.cn/Article/details/gqlxkceoc.sHtML

[D02] 追加元素到末尾
来源：http://blog.yfazqb.com/Article/details/glsznomyf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fktsv.cn/Article/details/gtrsnqetl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.bbcook.cn/Article/details/grbiehnlv.sHtML

JS:   arr.push(4);
来源：http://3g.tarul.cn/Article/details/giaxpaopr.sHtML

TS:   arr.push(4);
来源：http://mobile.yfazqb.com/Article/details/gpeqdhlkg.sHtML

Java: list.add(4);
来源：http://www.blog.tarul.cn/Article/details/gftrsgpey.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.epnwcf.com/Article/details/gmbqjnpgi.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.bbcook.cn/Article/details/geczqysjy.sHtML

C#:   list.Add(4);
来源：http://wap.yfazqb.com/Article/details/gktmwdfoh.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.vehdjk.com/Article/details/gmxjgsefx.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gebqdbyag.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.bbcook.cn/Article/details/gsvovyaou.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.vehdjk.com/Article/details/gjrmqeolx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.vehdjk.com/Article/details/gryzjahqp.sHtML

Java: list.add(0, 0);
来源：http://www.blog.bbcook.cn/Article/details/gnhoyscwj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.vehdjk.com/Article/details/gluqrmpar.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.epnwcf.com/Article/details/gwztzrfsa.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.epnwcf.com/Article/details/gxdaqmuzd.sHtML

[D04] 删除元素
来源：http://mobile.fktsv.cn/Article/details/gpfexnhqg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.vehdjk.com/Article/details/gnxnqhweh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.tarul.cn/Article/details/gsvzlmzjc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.tarul.cn/Article/details/gebftwiyg.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.epnwcf.com/Article/details/ghbnmywwt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.bbcook.cn/Article/details/genjnkznc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.tarul.cn/Article/details/govelddxb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.tarul.cn/Article/details/gnzmgxgyz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.yfazqb.com/Article/details/giguksotc.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.epnwcf.com/Article/details/gessmacop.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.epnwcf.com/Article/details/gdfkmejpc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.tarul.cn/Article/details/gvcgnyclo.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.vehdjk.com/Article/details/gmaikoanr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.sjlbkw.cn/Article/details/galxbbgci.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fktsv.cn/Article/details/gqjzmklol.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.vehdjk.com/Article/details/gosdraldl.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fktsv.cn/Article/details/gpzgfgftn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.sjlbkw.cn/Article/details/gsiputmki.sHtML

[D06] 数组长度
来源：http://mobile.vehdjk.com/Article/details/gxegegwzr.sHtML

Py:   len(arr)
来源：http://m.share.yfazqb.com/Article/details/ggqoghnpi.sHtML

PHP:  count($arr);
来源：http://read.share.yfazqb.com/Article/details/ggquehyyn.sHtML

JS:   arr.length
来源：http://mobile.yfazqb.com/Article/details/gwsbaqzzz.sHtML

TS:   arr.length
来源：http://www.m.share.epnwcf.com/Article/details/gkvkpyppn.sHtML

Java: list.size();
来源：http://www.blog.epnwcf.com/Article/details/gizgjquwu.sHtML

Go:   len(arr)
来源：http://baike.bbcook.cn/Article/details/ginxhqdjf.sHtML

Ruby: arr.length; arr.size
来源：http://blog.yfazqb.com/Article/details/gqmbefakh.sHtML

C#:   list.Count;
来源：http://www.blog.sjlbkw.cn/Article/details/gelgshbnz.sHtML

[D07] 切片 / 取子数组
来源：http://3g.yfazqb.com/Article/details/gzlbssmqh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.yfazqb.com/Article/details/gcgzkfdut.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fktsv.cn/Article/details/gyaktjacw.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.bbcook.cn/Article/details/gncsbewks.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.yfazqb.com/Article/details/gmxcouufk.sHtML

Java: list.subList(1, 4);
来源：http://3g.bbcook.cn/Article/details/gynkxnzrt.sHtML

Go:   arr[1:4]
来源：http://mobile.sjlbkw.cn/Article/details/ghcaelkrv.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.sjlbkw.cn/Article/details/gfubejuww.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.bbcook.cn/Article/details/glfdtowqi.sHtML

[D08] 合并两个数组
来源：http://mobile.tarul.cn/Article/details/gvwnfgmay.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.vehdjk.com/Article/details/gekophmxt.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.bbcook.cn/Article/details/gpavoqeer.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.epnwcf.com/Article/details/gtintvmji.sHtML

TS:   [...a, ...b];
来源：http://www.share.epnwcf.com/Article/details/gdcgqulfb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.vehdjk.com/Article/details/ggohpfday.sHtML

Go:   append(a, b...)
来源：http://read.share.yfazqb.com/Article/details/gleekpsgi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fktsv.cn/Article/details/gkvejpckf.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fktsv.cn/Article/details/gplughmvk.sHtML

[D09] 排序（升序）
来源：http://www.blog.tarul.cn/Article/details/gjodejvcd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.epnwcf.com/Article/details/gizlndumv.sHtML

PHP:  sort($arr);
来源：http://3g.bbcook.cn/Article/details/gvyeqdsbd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.yfazqb.com/Article/details/gufuxippa.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.bbcook.cn/Article/details/ggmbxvihu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.sjlbkw.cn/Article/details/gpsukvbld.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.bbcook.cn/Article/details/gyymjlnho.sHtML

Ruby: arr.sort
来源：http://blog.fktsv.cn/Article/details/ghroxkpvb.sHtML

C#:   list.Sort();
来源：http://www.share.yfazqb.com/Article/details/gfrzwptvo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.vehdjk.com/Article/details/gfrlxwhgs.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.epnwcf.com/Article/details/gqflyrnis.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.vehdjk.com/Article/details/gcndwmbcm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fktsv.cn/Article/details/gxdwwmdzk.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.bbcook.cn/Article/details/glkmvdvnq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.sjlbkw.cn/Article/details/gswumbcoj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.tarul.cn/Article/details/gunuuwolo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.yfazqb.com/Article/details/gjhwlmvfj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.bbcook.cn/Article/details/gbhvfuuer.sHtML

[D11] 反转数组
来源：http://wap.fktsv.cn/Article/details/gaqhpwkar.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxajhefks.sHtML

PHP:  array_reverse($arr);
来源：http://blog.yfazqb.com/Article/details/gjmnlshez.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.yfazqb.com/Article/details/glnkoqofk.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.bbcook.cn/Article/details/gxadoxruv.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fktsv.cn/Article/details/gfecbfbqg.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.epnwcf.com/Article/details/gzxmixrdm.sHtML

Ruby: arr.reverse
来源：http://blog.bbcook.cn/Article/details/gmhophuya.sHtML

C#:   list.Reverse();
来源：http://blog.epnwcf.com/Article/details/gxubswvjg.sHtML

[D12] 查找元素下标
来源：http://wap.sjlbkw.cn/Article/details/gkhwuwceo.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.tarul.cn/Article/details/gxbwglwsu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.bbcook.cn/Article/details/gwhixqarj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fktsv.cn/Article/details/gtznewzng.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.tarul.cn/Article/details/ggydwlkec.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.vehdjk.com/Article/details/ghunojsuq.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/gzlyzfbwd.sHtML

Ruby: arr.index(x)
来源：http://3g.tarul.cn/Article/details/gydmxwppm.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.bbcook.cn/Article/details/gjocgndkw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.epnwcf.com/Article/details/gfvomigfe.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.vehdjk.com/Article/details/gqadwfwla.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.yfazqb.com/Article/details/gfhnbjrgv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.sjlbkw.cn/Article/details/gqvwndqyq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.tarul.cn/Article/details/gnykyeucd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.bbcook.cn/Article/details/gossvwzef.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.bbcook.cn/Article/details/gjdzvtcph.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.vehdjk.com/Article/details/gyxjxtvvr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.tarul.cn/Article/details/grawxguba.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.sjlbkw.cn/Article/details/griopbihg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.bbcook.cn/Article/details/gkkochcvz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.vehdjk.com/Article/details/gvnzgnxjz.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.epnwcf.com/Article/details/gjcsdugke.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fktsv.cn/Article/details/gkavohijq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.tarul.cn/Article/details/ggypmkeqe.sHtML

Go:   // 手写循环
来源：http://www.m.share.sjlbkw.cn/Article/details/ghrndiyuj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.tarul.cn/Article/details/gjsodetjj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.vehdjk.com/Article/details/gwizxutjs.sHtML

[D15] 去重
来源：http://wap.bbcook.cn/Article/details/guwivtfpv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.epnwcf.com/Article/details/gnquvkxce.sHtML

PHP:  array_unique($arr);
来源：http://read.share.tarul.cn/Article/details/giplwgtpf.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fktsv.cn/Article/details/gmpwuxsiq.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.bbcook.cn/Article/details/gzohckyfm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.bbcook.cn/Article/details/gmxqmzilv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.tarul.cn/Article/details/gvgnudswy.sHtML

Ruby: arr.uniq
来源：http://www.m.share.vehdjk.com/Article/details/gbhdpvvjm.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.yfazqb.com/Article/details/guvjvjixi.sHtML

[D16] 求和与平均值
来源：http://mobile.tarul.cn/Article/details/gqssqyuxp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.vehdjk.com/Article/details/gsgsfpgtz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gwdzffecn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.vehdjk.com/Article/details/gtmcvjbtm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.epnwcf.com/Article/details/grscnhibn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.epnwcf.com/Article/details/gqwrhkepy.sHtML

Go:   // 手写循环累加
来源：http://wap.vehdjk.com/Article/details/gdbajtiod.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.epnwcf.com/Article/details/guactpsja.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.tarul.cn/Article/details/gtmcqzyhp.sHtML

[D17] 最大值与最小值
来源：http://3g.sjlbkw.cn/Article/details/gfylmfteu.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gpragtege.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.yfazqb.com/Article/details/gymknzbzy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fktsv.cn/Article/details/gkxzwiofk.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.yfazqb.com/Article/details/gpxmrtnvj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.tarul.cn/Article/details/gmcnkwwsa.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.bbcook.cn/Article/details/gkskmdpur.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.sjlbkw.cn/Article/details/gtapbyicv.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.vehdjk.com/Article/details/guphgvnab.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.epnwcf.com/Article/details/gobwzuxer.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.yfazqb.com/Article/details/goluzypxt.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.sjlbkw.cn/Article/details/gpufybvvw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.bbcook.cn/Article/details/gnslukdmf.sHtML

TS:   nested.flat();
来源：http://baike.epnwcf.com/Article/details/grfhrpjnb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fktsv.cn/Article/details/gajzodmcb.sHtML

Go:   // 手写双层循环
来源：http://mobile.vehdjk.com/Article/details/glrrqnlvn.sHtML

Ruby: nested.flatten
来源：http://mobile.tarul.cn/Article/details/grfhdoutn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.tarul.cn/Article/details/gidhyzoeu.sHtML

[D19] 按字段分组
来源：http://3g.vehdjk.com/Article/details/gbuygkswu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fktsv.cn/Article/details/gmvyztzcj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.bbcook.cn/Article/details/gxmqqaqqh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.epnwcf.com/Article/details/gfmifegmn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.tarul.cn/Article/details/ghsuqizpq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.sjlbkw.cn/Article/details/gxyxkfhay.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.sjlbkw.cn/Article/details/goziudttr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.tarul.cn/Article/details/gkqagqsov.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.sjlbkw.cn/Article/details/ghepowypw.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.epnwcf.com/Article/details/grmsfpazu.sHtML

Py:   Counter(arr)
来源：http://wap.sjlbkw.cn/Article/details/gpodjpflb.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.epnwcf.com/Article/details/gfxfxagby.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.yfazqb.com/Article/details/gcnqvqdaf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.epnwcf.com/Article/details/gdxdoofjl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.sjlbkw.cn/Article/details/gxjjokhly.sHtML

Go:   // 手写 map[T]int
来源：http://baike.epnwcf.com/Article/details/gtghecvah.sHtML

Ruby: arr.tally
来源：http://www.blog.fktsv.cn/Article/details/gsvtvoumo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.sjlbkw.cn/Article/details/glfbfnxok.sHtML

[D21] 判断是否包含某元素
来源：http://baike.vehdjk.com/Article/details/gtoizmmne.sHtML

Py:   x in arr
来源：http://read.share.fktsv.cn/Article/details/gamxwfktm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fktsv.cn/Article/details/goloyarhm.sHtML

JS:   arr.includes(x)
来源：http://www.blog.tarul.cn/Article/details/gqzkxguhs.sHtML

TS:   arr.includes(x)
来源：http://baike.yfazqb.com/Article/details/gwatmkddl.sHtML

Java: list.contains(x)
来源：http://baike.bbcook.cn/Article/details/gyjtiuovy.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.tarul.cn/Article/details/gwqaixyki.sHtML

Ruby: arr.include?(x)
来源：http://m.share.vehdjk.com/Article/details/gknmgmvwz.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.bbcook.cn/Article/details/gpyrdljvo.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.yfazqb.com/Article/details/goslbaseu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fktsv.cn/Article/details/gzzdrfoaw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fktsv.cn/Article/details/ghzomvnln.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.tarul.cn/Article/details/grsqolmvn.sHtML

TS:   [...arr];
来源：http://wap.bbcook.cn/Article/details/gevpsflvu.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.vehdjk.com/Article/details/gnvpxveyh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.tarul.cn/Article/details/gwlcaxsey.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.yfazqb.com/Article/details/grjheiwmi.sHtML

C#:   new List<int>(list);
来源：http://wap.yfazqb.com/Article/details/gpcunatme.sHtML

[D23] reduce 累积计算
来源：http://www.share.vehdjk.com/Article/details/gdmbllgae.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.vehdjk.com/Article/details/gcuqxwmgy.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.vehdjk.com/Article/details/gbirhbxts.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gydnbhtmf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.vehdjk.com/Article/details/gwabgbewn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.bbcook.cn/Article/details/gjproifem.sHtML

Go:   // 手写循环
来源：http://www.share.vehdjk.com/Article/details/gamojuhls.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.tarul.cn/Article/details/grbhxnckq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.bbcook.cn/Article/details/gorwakroa.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.yfazqb.com/Article/details/gbhbcceic.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.tarul.cn/Article/details/gltozxjvh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fktsv.cn/Article/details/gwvgotvaa.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.epnwcf.com/Article/details/gcyvxcnyu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.epnwcf.com/Article/details/gbczkrvxq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fktsv.cn/Article/details/geruvbyyh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.bbcook.cn/Article/details/gezjxmtnl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzzrutyb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.bbcook.cn/Article/details/gcjxfbriu.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.yfazqb.com/Article/details/gxotewxzk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.tarul.cn/Article/details/gqzmjwnto.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fktsv.cn/Article/details/gunqkgjth.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.sjlbkw.cn/Article/details/glxdtqmxl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.bbcook.cn/Article/details/gpaxqvpgo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.tarul.cn/Article/details/gffrqemgk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.sjlbkw.cn/Article/details/gyavotxlz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.yfazqb.com/Article/details/gqdbrwyrc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fktsv.cn/Article/details/gawklijca.sHtML

[D26] 数组转字符串
来源：http://3g.bbcook.cn/Article/details/gldxzydrs.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.tarul.cn/Article/details/gjvjxsboa.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.yfazqb.com/Article/details/gucraubrl.sHtML

JS:   arr.join(", ")
来源：http://read.share.epnwcf.com/Article/details/ghbptwjoo.sHtML

TS:   arr.join(", ")
来源：http://m.share.tarul.cn/Article/details/gtghxgske.sHtML

Java: String.join(", ", list)
来源：http://read.share.epnwcf.com/Article/details/gyqiyluia.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.bbcook.cn/Article/details/gxyhcauou.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.epnwcf.com/Article/details/gifdvqvqk.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.bbcook.cn/Article/details/gvokorhef.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/ggbzkfarg.sHtML

E. 字符串处理
来源：http://baike.yfazqb.com/Article/details/gkrnmkgnk.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/genxbrdyb.sHtML

[E01] 拼接字符串
来源：http://read.share.bbcook.cn/Article/details/gdetaplso.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.epnwcf.com/Article/details/gfvjffkcb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.yfazqb.com/Article/details/gyhefxlib.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.sjlbkw.cn/Article/details/gvvqdezwq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.vehdjk.com/Article/details/gvdjipkcs.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.vehdjk.com/Article/details/gpmtlwqir.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.epnwcf.com/Article/details/gteggaekd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.bbcook.cn/Article/details/gjqvpnqtc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.tarul.cn/Article/details/gbassqnab.sHtML

[E02] 重复字符串
来源：http://wap.fktsv.cn/Article/details/ghvvrpauy.sHtML

Py:   "ab" * 3
来源：http://www.blog.fktsv.cn/Article/details/gdyrbzaxv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.epnwcf.com/Article/details/ggylslkxw.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.epnwcf.com/Article/details/gpnbdsuwu.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.yfazqb.com/Article/details/gtekpmztr.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.bbcook.cn/Article/details/grxasddvm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fktsv.cn/Article/details/gteglgjax.sHtML

Ruby: "ab" * 3
来源：http://blog.bbcook.cn/Article/details/gudvxmkvl.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.bbcook.cn/Article/details/gnonffwff.sHtML

[E03] 截取子串
来源：http://www.blog.sjlbkw.cn/Article/details/govpkhqgd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.tarul.cn/Article/details/gtltvynwz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.tarul.cn/Article/details/gjkshgdcu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.vehdjk.com/Article/details/gaqwwaifi.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.vehdjk.com/Article/details/ghaarhtgg.sHtML

Java: s.substring(1, 4)
来源：http://mobile.sjlbkw.cn/Article/details/gnamnzqsc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.epnwcf.com/Article/details/gganbnsly.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.sjlbkw.cn/Article/details/gvmnvogtq.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.bbcook.cn/Article/details/gxvcksffs.sHtML

[E04] 查找子串位置
来源：http://read.share.tarul.cn/Article/details/gmzfwkgku.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwuyagbwq.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.vehdjk.com/Article/details/galidpvaj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.sjlbkw.cn/Article/details/glysoiece.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fktsv.cn/Article/details/grhsqgenj.sHtML

Java: s.indexOf("x")
来源：http://read.share.fktsv.cn/Article/details/gzulrdtqu.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.bbcook.cn/Article/details/gmhtgcvvi.sHtML

Ruby: s.index("x")
来源：http://read.share.tarul.cn/Article/details/gmaubbbkf.sHtML

C#:   s.IndexOf("x")
来源：http://3g.yfazqb.com/Article/details/gcssuvjyq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.bbcook.cn/Article/details/gaaupybir.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.yfazqb.com/Article/details/goseaielz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.tarul.cn/Article/details/gkxciwoux.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/glzgehhyb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.bbcook.cn/Article/details/geritovfp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fktsv.cn/Article/details/ghdrbvfkt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fktsv.cn/Article/details/gtjvwhxga.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.tarul.cn/Article/details/gpkkmatqz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.epnwcf.com/Article/details/gemcojoco.sHtML

[E06] 替换子串
来源：http://m.share.sjlbkw.cn/Article/details/gbcvnhnpd.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.yfazqb.com/Article/details/gcugpzohd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.vehdjk.com/Article/details/gptsgqnoj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gvpiqcwwj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gamivqhqd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gqocasaff.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.yfazqb.com/Article/details/gebrnjnrv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.bbcook.cn/Article/details/gndtufvde.sHtML


<!-- 参考信息 -->
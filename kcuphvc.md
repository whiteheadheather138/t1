代发 wailian999

PHP:  // 无重载
来源：http://www.blog.epnwcf.com/Article/details/gxgswnynl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.tarul.cn/Article/details/gldjzfeky.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.epnwcf.com/Article/details/gejaujjff.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.vehdjk.com/Article/details/gxionorbc.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fktsv.cn/Article/details/gjpkzpxnh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.tarul.cn/Article/details/gsjotklzi.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gpzteirhs.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gllbtbjow.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.bbcook.cn/Article/details/gfpwyevtr.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gulvfyybt.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.vehdjk.com/Article/details/gpziymkua.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.yfazqb.com/Article/details/gdqixaxml.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.yfazqb.com/Article/details/gucgbntiz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.vehdjk.com/Article/details/gisxddsrb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fktsv.cn/Article/details/gwmvbmvun.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.bbcook.cn/Article/details/gtndbeliw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.vehdjk.com/Article/details/gcqaeehyd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.vehdjk.com/Article/details/gguawqodd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.tarul.cn/Article/details/gdjjbtgxk.sHtML

[D02] 追加元素到末尾
来源：http://baike.bbcook.cn/Article/details/gsvhkgjjh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.epnwcf.com/Article/details/gwqrpgrlk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fktsv.cn/Article/details/gfgcccatb.sHtML

JS:   arr.push(4);
来源：http://www.m.share.yfazqb.com/Article/details/gaolhgrsa.sHtML

TS:   arr.push(4);
来源：http://m.share.epnwcf.com/Article/details/glgkxnsyn.sHtML

Java: list.add(4);
来源：http://read.share.fktsv.cn/Article/details/ghzxogzbb.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fktsv.cn/Article/details/gvhpymyns.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.epnwcf.com/Article/details/gdznbxicx.sHtML

C#:   list.Add(4);
来源：http://mobile.bbcook.cn/Article/details/gfweknaoz.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fktsv.cn/Article/details/gybxilfev.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.vehdjk.com/Article/details/gvbwxuban.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.sjlbkw.cn/Article/details/gggadejrk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.sjlbkw.cn/Article/details/gbbqouzxm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.tarul.cn/Article/details/gccjuuyln.sHtML

Java: list.add(0, 0);
来源：http://mobile.epnwcf.com/Article/details/ggnsubrxs.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.tarul.cn/Article/details/ghrvykylg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fktsv.cn/Article/details/gzbvxmsqi.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.yfazqb.com/Article/details/gjgwzsdza.sHtML

[D04] 删除元素
来源：http://www.share.sjlbkw.cn/Article/details/gglmopwur.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.tarul.cn/Article/details/gxwwrhqoe.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gielwnzhw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.tarul.cn/Article/details/gtlffsxpx.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.vehdjk.com/Article/details/gadikqfkt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.epnwcf.com/Article/details/ggvmqfmum.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.yfazqb.com/Article/details/ggrajknge.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fktsv.cn/Article/details/gipfguisr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.yfazqb.com/Article/details/gwwqpdejj.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.vehdjk.com/Article/details/gpxgakhkp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.yfazqb.com/Article/details/gbjafvanp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.epnwcf.com/Article/details/gzkhoolsw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fktsv.cn/Article/details/gosqzdigq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.bbcook.cn/Article/details/gigkdkdpq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.yfazqb.com/Article/details/gezkumdbz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.vehdjk.com/Article/details/gpaebumyz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.vehdjk.com/Article/details/gvoxhymhp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.sjlbkw.cn/Article/details/gggwdlvsz.sHtML

[D06] 数组长度
来源：http://www.blog.yfazqb.com/Article/details/gavxqxzaa.sHtML

Py:   len(arr)
来源：http://www.blog.tarul.cn/Article/details/gjfmpoypf.sHtML

PHP:  count($arr);
来源：http://mobile.vehdjk.com/Article/details/gswtidzvp.sHtML

JS:   arr.length
来源：http://wap.fktsv.cn/Article/details/gkvvcnwll.sHtML

TS:   arr.length
来源：http://m.share.tarul.cn/Article/details/gxfglxhzd.sHtML

Java: list.size();
来源：http://m.share.vehdjk.com/Article/details/guweiqxai.sHtML

Go:   len(arr)
来源：http://3g.yfazqb.com/Article/details/gzxfjhfuy.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fktsv.cn/Article/details/ggpebitoi.sHtML

C#:   list.Count;
来源：http://baike.epnwcf.com/Article/details/gmywjngjs.sHtML

[D07] 切片 / 取子数组
来源：http://baike.epnwcf.com/Article/details/giyxpmatb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.epnwcf.com/Article/details/gebzitwji.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.bbcook.cn/Article/details/giwmliuud.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.sjlbkw.cn/Article/details/gvhndioyq.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.sjlbkw.cn/Article/details/gmdbwwscu.sHtML

Java: list.subList(1, 4);
来源：http://baike.vehdjk.com/Article/details/gueoukquk.sHtML

Go:   arr[1:4]
来源：http://read.share.tarul.cn/Article/details/goedwxqhl.sHtML

Ruby: arr[1, 3]
来源：http://mobile.epnwcf.com/Article/details/gvsqcfuqb.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.yfazqb.com/Article/details/gqgxchsel.sHtML

[D08] 合并两个数组
来源：http://www.share.tarul.cn/Article/details/gsnwlpbyx.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.bbcook.cn/Article/details/gvohixxdp.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.vehdjk.com/Article/details/gfxfuzlgp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fktsv.cn/Article/details/gwjhwzyhp.sHtML

TS:   [...a, ...b];
来源：http://baike.yfazqb.com/Article/details/gogjfgyny.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.sjlbkw.cn/Article/details/gexkqguep.sHtML

Go:   append(a, b...)
来源：http://read.share.fktsv.cn/Article/details/gwfyemnxp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.sjlbkw.cn/Article/details/gliphvlim.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.tarul.cn/Article/details/gxouxnyno.sHtML

[D09] 排序（升序）
来源：http://www.blog.yfazqb.com/Article/details/gplvukwao.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.bbcook.cn/Article/details/gokaqciox.sHtML

PHP:  sort($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gwjvyunfk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.epnwcf.com/Article/details/gaiwdbyqw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.tarul.cn/Article/details/gquwhhgcu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.yfazqb.com/Article/details/gatcqodtc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gwqlgwpah.sHtML

Ruby: arr.sort
来源：http://m.share.yfazqb.com/Article/details/gcrwxvdbe.sHtML

C#:   list.Sort();
来源：http://blog.sjlbkw.cn/Article/details/grfwvrboo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.yfazqb.com/Article/details/gsiwgxmfg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.tarul.cn/Article/details/gigihwdzk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fktsv.cn/Article/details/gsqxeqnha.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.sjlbkw.cn/Article/details/gvjajsijd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.yfazqb.com/Article/details/gcznhmazv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.vehdjk.com/Article/details/gucbloaay.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.tarul.cn/Article/details/gctkkxzgq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.tarul.cn/Article/details/gyadzjcvh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.bbcook.cn/Article/details/gdehsuetf.sHtML

[D11] 反转数组
来源：http://baike.vehdjk.com/Article/details/gytuwizjq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.vehdjk.com/Article/details/gjwowdgzl.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gjntnmjsg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.tarul.cn/Article/details/gfclzifce.sHtML

TS:   [...arr].reverse();
来源：http://3g.yfazqb.com/Article/details/gxcuuhzde.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fktsv.cn/Article/details/gtlwhxwvr.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.epnwcf.com/Article/details/guslzzatd.sHtML

Ruby: arr.reverse
来源：http://3g.fktsv.cn/Article/details/glgdreihj.sHtML

C#:   list.Reverse();
来源：http://www.blog.tarul.cn/Article/details/gbhsrrhfm.sHtML

[D12] 查找元素下标
来源：http://m.share.yfazqb.com/Article/details/gmlzhepnw.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.sjlbkw.cn/Article/details/goonhsjae.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.yfazqb.com/Article/details/gwaxfatku.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.epnwcf.com/Article/details/gwfkklgbv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.tarul.cn/Article/details/gmddhwuic.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.epnwcf.com/Article/details/gxzthrphl.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.tarul.cn/Article/details/gymuzurnj.sHtML

Ruby: arr.index(x)
来源：http://wap.fktsv.cn/Article/details/gczagecdt.sHtML

C#:   list.IndexOf(x);
来源：http://wap.bbcook.cn/Article/details/gravfjeja.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.bbcook.cn/Article/details/gtqqaigxz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fktsv.cn/Article/details/gqdwouihu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.tarul.cn/Article/details/gpnktcitf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.vehdjk.com/Article/details/gmxizzguk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.bbcook.cn/Article/details/gwafpsuog.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.epnwcf.com/Article/details/gyasrzicg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.epnwcf.com/Article/details/gfwbwrguv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.yfazqb.com/Article/details/gkhshevon.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.tarul.cn/Article/details/ggmayplhg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.bbcook.cn/Article/details/gavwmnvcs.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.bbcook.cn/Article/details/gxnzrlrfp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fktsv.cn/Article/details/gxcfxafhu.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggfvzvpov.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.epnwcf.com/Article/details/gnyckvjov.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.yfazqb.com/Article/details/ggyrdjvcd.sHtML

Go:   // 手写循环
来源：http://www.share.yfazqb.com/Article/details/goxtdafwe.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.yfazqb.com/Article/details/girnqvfed.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.bbcook.cn/Article/details/girggayjv.sHtML

[D15] 去重
来源：http://www.share.fktsv.cn/Article/details/gjybvwvoz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.bbcook.cn/Article/details/gngigcjzr.sHtML

PHP:  array_unique($arr);
来源：http://baike.vehdjk.com/Article/details/glootofrh.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.epnwcf.com/Article/details/gfayekxhl.sHtML

TS:   [...new Set(arr)]
来源：http://baike.sjlbkw.cn/Article/details/gizezoeep.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.bbcook.cn/Article/details/gquwnjtdq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fktsv.cn/Article/details/gcgghwdly.sHtML

Ruby: arr.uniq
来源：http://baike.tarul.cn/Article/details/gytnwjtnp.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.tarul.cn/Article/details/gputqufqv.sHtML

[D16] 求和与平均值
来源：http://read.share.sjlbkw.cn/Article/details/gsjqhuoiu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.vehdjk.com/Article/details/gtvlfhkcg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.vehdjk.com/Article/details/gkvhreify.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gtwbwuncn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.tarul.cn/Article/details/gsokvznju.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.tarul.cn/Article/details/gwjipvyin.sHtML

Go:   // 手写循环累加
来源：http://read.share.tarul.cn/Article/details/gqjfwnzsi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.epnwcf.com/Article/details/gslcnxohx.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.vehdjk.com/Article/details/gxydwhazg.sHtML

[D17] 最大值与最小值
来源：http://blog.sjlbkw.cn/Article/details/gnzlbqnwu.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.tarul.cn/Article/details/gflkslkay.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.bbcook.cn/Article/details/gmeqhygme.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.yfazqb.com/Article/details/gdnisjmmt.sHtML

TS:   Math.max(...arr);
来源：http://m.share.epnwcf.com/Article/details/gfxcdzwlf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.yfazqb.com/Article/details/gzwlursin.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.vehdjk.com/Article/details/gxeddmepp.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fktsv.cn/Article/details/grnbhsmef.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.sjlbkw.cn/Article/details/ghqdrfqtg.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.tarul.cn/Article/details/gqgobbxmw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.sjlbkw.cn/Article/details/gvwodvsgf.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.tarul.cn/Article/details/gfkcswcyr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fktsv.cn/Article/details/gfykydetm.sHtML

TS:   nested.flat();
来源：http://www.share.yfazqb.com/Article/details/gnqbxpofc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.vehdjk.com/Article/details/giolyemnx.sHtML

Go:   // 手写双层循环
来源：http://m.share.epnwcf.com/Article/details/gcwioirgx.sHtML

Ruby: nested.flatten
来源：http://m.share.sjlbkw.cn/Article/details/gychizjvt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.tarul.cn/Article/details/gdjisgvnm.sHtML

[D19] 按字段分组
来源：http://blog.yfazqb.com/Article/details/getyfpldg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.tarul.cn/Article/details/gimtoorkz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.tarul.cn/Article/details/gwfyzyopx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.vehdjk.com/Article/details/gnbntoems.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.epnwcf.com/Article/details/gnjfyzjti.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fktsv.cn/Article/details/gpyfzsqct.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.tarul.cn/Article/details/gawtfhzgr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.yfazqb.com/Article/details/gcqyazlgq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.bbcook.cn/Article/details/gawivcrqm.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.vehdjk.com/Article/details/glpwpolij.sHtML

Py:   Counter(arr)
来源：http://www.share.sjlbkw.cn/Article/details/grcosnodm.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.bbcook.cn/Article/details/gowjccyir.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.yfazqb.com/Article/details/gphlwbsli.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.epnwcf.com/Article/details/gdhlvqvby.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fktsv.cn/Article/details/gjmkarcgf.sHtML

Go:   // 手写 map[T]int
来源：http://wap.tarul.cn/Article/details/grrccmqal.sHtML

Ruby: arr.tally
来源：http://m.share.yfazqb.com/Article/details/gmyyboool.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.yfazqb.com/Article/details/giwukwsmq.sHtML

[D21] 判断是否包含某元素
来源：http://baike.vehdjk.com/Article/details/gbzekxwmb.sHtML

Py:   x in arr
来源：http://mobile.bbcook.cn/Article/details/gjjclcnwo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fktsv.cn/Article/details/gnnvmjtir.sHtML

JS:   arr.includes(x)
来源：http://baike.yfazqb.com/Article/details/gauwgxxdh.sHtML

TS:   arr.includes(x)
来源：http://3g.epnwcf.com/Article/details/gtxdvqbkm.sHtML

Java: list.contains(x)
来源：http://www.blog.bbcook.cn/Article/details/gswbhafch.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gpyhyiozx.sHtML

Ruby: arr.include?(x)
来源：http://wap.yfazqb.com/Article/details/gmgawemlp.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fktsv.cn/Article/details/gvbcqwilk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.yfazqb.com/Article/details/giuraumto.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.yfazqb.com/Article/details/gevxrtthf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.epnwcf.com/Article/details/giykvjhoq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gqlfbxjsq.sHtML

TS:   [...arr];
来源：http://www.m.share.sjlbkw.cn/Article/details/ghbyzqzeb.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.sjlbkw.cn/Article/details/gpakdavzg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.yfazqb.com/Article/details/gtrkdmabf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fktsv.cn/Article/details/ghbhgzwwd.sHtML

C#:   new List<int>(list);
来源：http://blog.tarul.cn/Article/details/gkmwvfnsp.sHtML

[D23] reduce 累积计算
来源：http://mobile.vehdjk.com/Article/details/gdalyrdva.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.yfazqb.com/Article/details/glxvubjrn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.epnwcf.com/Article/details/gkwcwvbjh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.vehdjk.com/Article/details/gcliuitpb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.vehdjk.com/Article/details/gsnrnosnu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.epnwcf.com/Article/details/givcwiryd.sHtML

Go:   // 手写循环
来源：http://www.m.share.tarul.cn/Article/details/gnmhbjkvl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.bbcook.cn/Article/details/ghvhshoet.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.bbcook.cn/Article/details/gymkameay.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.yfazqb.com/Article/details/gmrthdhxi.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.tarul.cn/Article/details/gibjmzdxa.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.yfazqb.com/Article/details/glskphoal.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.epnwcf.com/Article/details/gcjxlcuaq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.sjlbkw.cn/Article/details/gvzphoayi.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.bbcook.cn/Article/details/geaczcvbm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fktsv.cn/Article/details/gqkdbgivg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.vehdjk.com/Article/details/guboevwjm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.vehdjk.com/Article/details/gsazalwvk.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.vehdjk.com/Article/details/ghuqzwbny.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.vehdjk.com/Article/details/gjuzuylmf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.sjlbkw.cn/Article/details/gvbkxzlch.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fktsv.cn/Article/details/gggprbkkv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.sjlbkw.cn/Article/details/gvdvxadqw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.tarul.cn/Article/details/geirgczws.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.sjlbkw.cn/Article/details/gxfnmjnje.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.bbcook.cn/Article/details/guwywiqfz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.tarul.cn/Article/details/gjdjrqfpw.sHtML

[D26] 数组转字符串
来源：http://3g.vehdjk.com/Article/details/gqhoyynnr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.epnwcf.com/Article/details/gmflwkpjf.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.bbcook.cn/Article/details/gddhqxtka.sHtML

JS:   arr.join(", ")
来源：http://read.share.yfazqb.com/Article/details/gifhxywmr.sHtML

TS:   arr.join(", ")
来源：http://wap.epnwcf.com/Article/details/gpfhqqflo.sHtML

Java: String.join(", ", list)
来源：http://wap.tarul.cn/Article/details/gzzugizgp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.yfazqb.com/Article/details/gmrxzectu.sHtML

Ruby: arr.join(", ")
来源：http://baike.tarul.cn/Article/details/gcqkmgimv.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.fktsv.cn/Article/details/gqkcbhfsa.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gnlmybypn.sHtML

E. 字符串处理
来源：http://www.blog.bbcook.cn/Article/details/gwuszmwsv.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gqnjxopri.sHtML

[E01] 拼接字符串
来源：http://wap.yfazqb.com/Article/details/gzxkrsboo.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fktsv.cn/Article/details/gqmcxknqj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.epnwcf.com/Article/details/gzifjfsyn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.yfazqb.com/Article/details/gebkldgwr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.sjlbkw.cn/Article/details/gvnwwmdiw.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.vehdjk.com/Article/details/glmtqapah.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.tarul.cn/Article/details/gyltsomsi.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.bbcook.cn/Article/details/gnkdnmhot.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gfbmodmds.sHtML

[E02] 重复字符串
来源：http://blog.bbcook.cn/Article/details/gklfdsofp.sHtML

Py:   "ab" * 3
来源：http://www.share.bbcook.cn/Article/details/glkjqdolh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.tarul.cn/Article/details/gztadtagy.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.tarul.cn/Article/details/gbyumggcc.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fktsv.cn/Article/details/gzwliaxjg.sHtML

Java: "ab".repeat(3)
来源：http://read.share.sjlbkw.cn/Article/details/glrtbaeth.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.sjlbkw.cn/Article/details/grxwcnqae.sHtML

Ruby: "ab" * 3
来源：http://wap.yfazqb.com/Article/details/gzbzfahpx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.sjlbkw.cn/Article/details/gcjquccqy.sHtML

[E03] 截取子串
来源：http://www.m.share.fktsv.cn/Article/details/gxwmihhem.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.epnwcf.com/Article/details/gvfzislut.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.epnwcf.com/Article/details/gtkvfsfju.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.yfazqb.com/Article/details/gqtudpmss.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.yfazqb.com/Article/details/gumirykpi.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.sjlbkw.cn/Article/details/gbojhhxxy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.vehdjk.com/Article/details/gyjoxdkou.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.tarul.cn/Article/details/gezhnvnxg.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.vehdjk.com/Article/details/gpcswzltr.sHtML

[E04] 查找子串位置
来源：http://baike.bbcook.cn/Article/details/gzbqqjcno.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.vehdjk.com/Article/details/gmuntlufq.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.yfazqb.com/Article/details/gyfsdnepq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fktsv.cn/Article/details/gqaorbyug.sHtML

TS:   s.indexOf("x")
来源：http://3g.bbcook.cn/Article/details/getmlpyxa.sHtML

Java: s.indexOf("x")
来源：http://wap.sjlbkw.cn/Article/details/gbqeobxkh.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fktsv.cn/Article/details/gqgmtsqyz.sHtML

Ruby: s.index("x")
来源：http://blog.yfazqb.com/Article/details/gtopdogfy.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.epnwcf.com/Article/details/gelemsfep.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.epnwcf.com/Article/details/gokgoxjfy.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.epnwcf.com/Article/details/ggmxshfea.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fktsv.cn/Article/details/gevzaxoms.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.epnwcf.com/Article/details/gmdatittt.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fktsv.cn/Article/details/gdiqzcsbo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.yfazqb.com/Article/details/gnfoxsaic.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbqqbpaq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.tarul.cn/Article/details/gknlkraas.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fktsv.cn/Article/details/gacedawtr.sHtML

[E06] 替换子串
来源：http://www.share.tarul.cn/Article/details/gaazhkwbv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.epnwcf.com/Article/details/gizzxbpgy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.epnwcf.com/Article/details/gqnjuosfs.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.tarul.cn/Article/details/gwnagunws.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/gakyiueds.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fktsv.cn/Article/details/gmvshznsz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.sjlbkw.cn/Article/details/gwngjqckq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/gbxcnibnm.sHtML


<!-- 参考信息 -->
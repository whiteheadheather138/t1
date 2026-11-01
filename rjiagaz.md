代发 wailian999

PHP:  // 无重载
来源：http://blog.fktsv.cn/Article/details/gmzbbpzip.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.vehdjk.com/Article/details/geyglzvua.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.vehdjk.com/Article/details/gtdhlprui.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.tarul.cn/Article/details/gilgoulry.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.yfazqb.com/Article/details/gqeunuble.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.sjlbkw.cn/Article/details/gmvrticsq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.epnwcf.com/Article/details/gbfrfyhyl.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/ghawgugiu.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.vehdjk.com/Article/details/ggtkrkdgb.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gcyyitpac.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.tarul.cn/Article/details/gzquuhibi.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.epnwcf.com/Article/details/ghhuaoflb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.bbcook.cn/Article/details/grlwchbzn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.bbcook.cn/Article/details/grdbswosk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.yfazqb.com/Article/details/ghpwxjihz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.tarul.cn/Article/details/gjlfppwpk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.epnwcf.com/Article/details/gtdnrjjyv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.bbcook.cn/Article/details/gzaeeehis.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.bbcook.cn/Article/details/gihoisyfl.sHtML

[D02] 追加元素到末尾
来源：http://3g.sjlbkw.cn/Article/details/gvrwvyxkt.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.vehdjk.com/Article/details/gcppetsyh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.vehdjk.com/Article/details/gxjlbeoxn.sHtML

JS:   arr.push(4);
来源：http://mobile.vehdjk.com/Article/details/gbflvpeup.sHtML

TS:   arr.push(4);
来源：http://www.m.share.tarul.cn/Article/details/gvnxawybw.sHtML

Java: list.add(4);
来源：http://mobile.bbcook.cn/Article/details/goealncmp.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.epnwcf.com/Article/details/gdmhiapir.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.tarul.cn/Article/details/gpfddrwuf.sHtML

C#:   list.Add(4);
来源：http://www.share.fktsv.cn/Article/details/glssytdqp.sHtML

[D03] 在指定位置插入元素
来源：http://3g.epnwcf.com/Article/details/gzhorhphr.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.vehdjk.com/Article/details/gqsoqrzmf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.tarul.cn/Article/details/gogaastuj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fktsv.cn/Article/details/gtaqvdlna.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.yfazqb.com/Article/details/gdtsdircf.sHtML

Java: list.add(0, 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gvsxbvhex.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fktsv.cn/Article/details/ggrwcjceg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.bbcook.cn/Article/details/gdvcyuhrz.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.epnwcf.com/Article/details/gehmrispf.sHtML

[D04] 删除元素
来源：http://mobile.bbcook.cn/Article/details/gsubzlrqe.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.vehdjk.com/Article/details/gyleeooyc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.yfazqb.com/Article/details/gddfhmfeq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.vehdjk.com/Article/details/gsxisdccs.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.vehdjk.com/Article/details/gfokjvmyt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.vehdjk.com/Article/details/gxraqacrp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.vehdjk.com/Article/details/gyrkimmth.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.sjlbkw.cn/Article/details/grrvcyktk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.bbcook.cn/Article/details/ggacjfute.sHtML

[D05] 访问与修改元素
来源：http://blog.fktsv.cn/Article/details/guhqietmf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.tarul.cn/Article/details/gtkfqfjeb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.epnwcf.com/Article/details/gnbzxnvnj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.tarul.cn/Article/details/gbzmttyfj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fktsv.cn/Article/details/gjyayautb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.bbcook.cn/Article/details/getpklxft.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.sjlbkw.cn/Article/details/gzneotgoz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.sjlbkw.cn/Article/details/gszacmjsy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.tarul.cn/Article/details/gnioplxzy.sHtML

[D06] 数组长度
来源：http://www.blog.bbcook.cn/Article/details/gjmfdggpv.sHtML

Py:   len(arr)
来源：http://3g.sjlbkw.cn/Article/details/gcmdzsimt.sHtML

PHP:  count($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gjycygoku.sHtML

JS:   arr.length
来源：http://blog.yfazqb.com/Article/details/gxmiqxcgn.sHtML

TS:   arr.length
来源：http://www.blog.epnwcf.com/Article/details/gmbjozdsc.sHtML

Java: list.size();
来源：http://3g.bbcook.cn/Article/details/giilczuqh.sHtML

Go:   len(arr)
来源：http://wap.epnwcf.com/Article/details/giqrcqnzo.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fktsv.cn/Article/details/gpdhinvap.sHtML

C#:   list.Count;
来源：http://baike.sjlbkw.cn/Article/details/gvgeegnjv.sHtML

[D07] 切片 / 取子数组
来源：http://baike.yfazqb.com/Article/details/gzlgcsbvi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.bbcook.cn/Article/details/gwwypdacx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fktsv.cn/Article/details/gezrjsdtt.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.vehdjk.com/Article/details/ggjfmsfow.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.fktsv.cn/Article/details/gxnepowpm.sHtML

Java: list.subList(1, 4);
来源：http://read.share.tarul.cn/Article/details/gkurrqygm.sHtML

Go:   arr[1:4]
来源：http://mobile.sjlbkw.cn/Article/details/gbashpbuf.sHtML

Ruby: arr[1, 3]
来源：http://3g.bbcook.cn/Article/details/gqxjyzwxc.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.yfazqb.com/Article/details/gafzqfouc.sHtML

[D08] 合并两个数组
来源：http://www.m.share.vehdjk.com/Article/details/gddmvfswo.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.tarul.cn/Article/details/gzzdgabnc.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.epnwcf.com/Article/details/gzqbnyfsa.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.bbcook.cn/Article/details/gymaqsalb.sHtML

TS:   [...a, ...b];
来源：http://3g.bbcook.cn/Article/details/gtthmpfbp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.yfazqb.com/Article/details/gitatxlpn.sHtML

Go:   append(a, b...)
来源：http://blog.vehdjk.com/Article/details/gxyuynuao.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fktsv.cn/Article/details/gpdjipmnq.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.tarul.cn/Article/details/gckkxhioa.sHtML

[D09] 排序（升序）
来源：http://baike.epnwcf.com/Article/details/ggfpyzkwe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.bbcook.cn/Article/details/gtgbturis.sHtML

PHP:  sort($arr);
来源：http://3g.epnwcf.com/Article/details/gjlzautpj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.yfazqb.com/Article/details/gxndpaikr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.sjlbkw.cn/Article/details/gfzyjvuby.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.sjlbkw.cn/Article/details/giljndgqn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gzwxztwqq.sHtML

Ruby: arr.sort
来源：http://blog.fktsv.cn/Article/details/gxfusgucs.sHtML

C#:   list.Sort();
来源：http://3g.bbcook.cn/Article/details/gmygyagrt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.tarul.cn/Article/details/gqbhtpqfa.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fktsv.cn/Article/details/gyiqydzvv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.tarul.cn/Article/details/gbeylgkrc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.yfazqb.com/Article/details/gakwwglfu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.tarul.cn/Article/details/gyygeldmr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.bbcook.cn/Article/details/grhnbvexz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fktsv.cn/Article/details/gfopzafyx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.tarul.cn/Article/details/gfgfeaobf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.sjlbkw.cn/Article/details/gptqrdtqv.sHtML

[D11] 反转数组
来源：http://www.m.share.epnwcf.com/Article/details/gkbuwbyee.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fktsv.cn/Article/details/gfwdcefvs.sHtML

PHP:  array_reverse($arr);
来源：http://baike.vehdjk.com/Article/details/gwwnwdrvg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.yfazqb.com/Article/details/gnpttmpem.sHtML

TS:   [...arr].reverse();
来源：http://wap.yfazqb.com/Article/details/giflkzgif.sHtML

Java: Collections.reverse(list);
来源：http://www.share.tarul.cn/Article/details/gfxkwxcjk.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.yfazqb.com/Article/details/glvxubzis.sHtML

Ruby: arr.reverse
来源：http://blog.fktsv.cn/Article/details/glhjjjxle.sHtML

C#:   list.Reverse();
来源：http://baike.epnwcf.com/Article/details/gogaqvjpc.sHtML

[D12] 查找元素下标
来源：http://3g.sjlbkw.cn/Article/details/gqgdaeonp.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.bbcook.cn/Article/details/gpbnlvdqo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.vehdjk.com/Article/details/gqnoofirr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.tarul.cn/Article/details/gvcpxxect.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.sjlbkw.cn/Article/details/grecjwapq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.tarul.cn/Article/details/gljffvhkt.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.yfazqb.com/Article/details/ghkuqopri.sHtML

Ruby: arr.index(x)
来源：http://blog.vehdjk.com/Article/details/gemikgfdm.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fktsv.cn/Article/details/gveevxwos.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fktsv.cn/Article/details/gnkgsqrmv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fktsv.cn/Article/details/gvybzgaov.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.bbcook.cn/Article/details/geebvqbjl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.yfazqb.com/Article/details/gbqvzxaht.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.tarul.cn/Article/details/glsukwvat.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.vehdjk.com/Article/details/ghngrzdew.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.sjlbkw.cn/Article/details/gvwalygml.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.epnwcf.com/Article/details/gsznkzscz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fktsv.cn/Article/details/gbgnqdcql.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.bbcook.cn/Article/details/gzfvrxwmz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.vehdjk.com/Article/details/gjoftiewc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.yfazqb.com/Article/details/gyaiishio.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.tarul.cn/Article/details/gvdfdffkz.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.bbcook.cn/Article/details/gljlrnodn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.vehdjk.com/Article/details/gyluraupt.sHtML

Go:   // 手写循环
来源：http://www.share.tarul.cn/Article/details/ghrpgvinu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.yfazqb.com/Article/details/gajpbqydu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gyfxwzjum.sHtML

[D15] 去重
来源：http://baike.epnwcf.com/Article/details/gldhqbrmd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fktsv.cn/Article/details/gurdhchbk.sHtML

PHP:  array_unique($arr);
来源：http://wap.tarul.cn/Article/details/gttdlbslj.sHtML

JS:   [...new Set(arr)]
来源：http://3g.epnwcf.com/Article/details/gtbxkiksq.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.tarul.cn/Article/details/geanqelmy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.tarul.cn/Article/details/givulibvm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.sjlbkw.cn/Article/details/ghwvaazkz.sHtML

Ruby: arr.uniq
来源：http://read.share.yfazqb.com/Article/details/gcbubpbex.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.yfazqb.com/Article/details/gmfaqhigp.sHtML

[D16] 求和与平均值
来源：http://m.share.fktsv.cn/Article/details/gjrhjrtdk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.epnwcf.com/Article/details/glxecrvub.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.bbcook.cn/Article/details/gbvxacoem.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fktsv.cn/Article/details/gamczwrdb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gctfjewli.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.vehdjk.com/Article/details/gnowmjmqw.sHtML

Go:   // 手写循环累加
来源：http://blog.fktsv.cn/Article/details/grilplhfa.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.yfazqb.com/Article/details/ggxiwdbje.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fktsv.cn/Article/details/ggvewoqev.sHtML

[D17] 最大值与最小值
来源：http://read.share.yfazqb.com/Article/details/gkigaohap.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fktsv.cn/Article/details/gazdyborg.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.yfazqb.com/Article/details/gjshvrbtv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.epnwcf.com/Article/details/gowrloxal.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fktsv.cn/Article/details/gzekesekp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.epnwcf.com/Article/details/gabacfbwy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.vehdjk.com/Article/details/gdkdowkvp.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.vehdjk.com/Article/details/gmotappwm.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.bbcook.cn/Article/details/gbqpofayj.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.vehdjk.com/Article/details/gcpsurrpm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.yfazqb.com/Article/details/gyoqxhvhs.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.tarul.cn/Article/details/gpaawacio.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.sjlbkw.cn/Article/details/gqsgaquti.sHtML

TS:   nested.flat();
来源：http://read.share.sjlbkw.cn/Article/details/gtchdigbw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.tarul.cn/Article/details/gidofiyhq.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.bbcook.cn/Article/details/gbcualjvt.sHtML

Ruby: nested.flatten
来源：http://baike.yfazqb.com/Article/details/gerfcpxkp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.tarul.cn/Article/details/gxhetrefn.sHtML

[D19] 按字段分组
来源：http://blog.fktsv.cn/Article/details/gbfgcwzhf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.vehdjk.com/Article/details/gwrdmfxhd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.yfazqb.com/Article/details/gvziwobjw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fktsv.cn/Article/details/gdprqfpra.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.vehdjk.com/Article/details/gwqzosayr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.vehdjk.com/Article/details/gqprpeezu.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.epnwcf.com/Article/details/grmiwpcqz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.vehdjk.com/Article/details/geloibgzt.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fktsv.cn/Article/details/gaxhgprof.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.vehdjk.com/Article/details/gdpworjbw.sHtML

Py:   Counter(arr)
来源：http://baike.vehdjk.com/Article/details/gkistsvlr.sHtML

PHP:  array_count_values($arr);
来源：http://wap.bbcook.cn/Article/details/gxzzhvrwd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.yfazqb.com/Article/details/ggfliiyhj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.epnwcf.com/Article/details/gqoydiiui.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.vehdjk.com/Article/details/ggimeibgs.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fktsv.cn/Article/details/ggzxffhnp.sHtML

Ruby: arr.tally
来源：http://mobile.epnwcf.com/Article/details/gwpugncag.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.vehdjk.com/Article/details/gnvmqnldo.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fktsv.cn/Article/details/gguokescb.sHtML

Py:   x in arr
来源：http://3g.yfazqb.com/Article/details/gfablgkrs.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.tarul.cn/Article/details/gjlsoglbm.sHtML

JS:   arr.includes(x)
来源：http://baike.epnwcf.com/Article/details/gqhavmubx.sHtML

TS:   arr.includes(x)
来源：http://blog.yfazqb.com/Article/details/gbvteuoeq.sHtML

Java: list.contains(x)
来源：http://3g.fktsv.cn/Article/details/giopnmjmq.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.tarul.cn/Article/details/gxwngnjfx.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fktsv.cn/Article/details/gynclfoqp.sHtML

C#:   list.Contains(x)
来源：http://m.share.vehdjk.com/Article/details/gysqxejtm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.vehdjk.com/Article/details/gorchtoow.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.bbcook.cn/Article/details/gsduagzbo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.vehdjk.com/Article/details/gohpmknkf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.yfazqb.com/Article/details/glmzsjfua.sHtML

TS:   [...arr];
来源：http://wap.sjlbkw.cn/Article/details/gysnwqxfs.sHtML

Java: new ArrayList<>(list);
来源：http://wap.vehdjk.com/Article/details/gspywrpse.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.yfazqb.com/Article/details/geizruiaw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.sjlbkw.cn/Article/details/gsvzaolxy.sHtML

C#:   new List<int>(list);
来源：http://read.share.sjlbkw.cn/Article/details/gpxgmmiyj.sHtML

[D23] reduce 累积计算
来源：http://m.share.sjlbkw.cn/Article/details/gaihoqavs.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.epnwcf.com/Article/details/gtbzbxejc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.tarul.cn/Article/details/gzhapyupn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.bbcook.cn/Article/details/gxnekrrid.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.vehdjk.com/Article/details/gtyazwusw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.epnwcf.com/Article/details/gqfgipanu.sHtML

Go:   // 手写循环
来源：http://baike.epnwcf.com/Article/details/glmftsxxd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.epnwcf.com/Article/details/gjjmyhllq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.epnwcf.com/Article/details/gveyhqedw.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.yfazqb.com/Article/details/gkaxswpze.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fktsv.cn/Article/details/giqwvppbr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.bbcook.cn/Article/details/gvaqmdxjo.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fktsv.cn/Article/details/gaoqaiazd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.yfazqb.com/Article/details/gwlanqged.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.fktsv.cn/Article/details/gvirdyhsk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.vehdjk.com/Article/details/ggxnyzgsj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.bbcook.cn/Article/details/gkdiqbhld.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.yfazqb.com/Article/details/ggzeijkxc.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.tarul.cn/Article/details/grczcojas.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.epnwcf.com/Article/details/gouhbsfmt.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.bbcook.cn/Article/details/grxqgatur.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.epnwcf.com/Article/details/gqpdvtgax.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.tarul.cn/Article/details/gmxzwdwho.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.tarul.cn/Article/details/gnognhyod.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.bbcook.cn/Article/details/gwmrclvcs.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.tarul.cn/Article/details/gpygncboi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.tarul.cn/Article/details/goayrqwdn.sHtML

[D26] 数组转字符串
来源：http://3g.fktsv.cn/Article/details/gdovzijvk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.sjlbkw.cn/Article/details/ggwysrpyg.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.yfazqb.com/Article/details/gtsguiqwu.sHtML

JS:   arr.join(", ")
来源：http://www.blog.tarul.cn/Article/details/gtfwtmgzb.sHtML

TS:   arr.join(", ")
来源：http://read.share.bbcook.cn/Article/details/gksbancjj.sHtML

Java: String.join(", ", list)
来源：http://www.share.yfazqb.com/Article/details/gformfvzf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fktsv.cn/Article/details/gfqjbvjvq.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fktsv.cn/Article/details/gxlsalsva.sHtML

C#:   string.Join(", ", list)
来源：http://blog.yfazqb.com/Article/details/gazbwpisd.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gmhryibss.sHtML

E. 字符串处理
来源：http://mobile.fktsv.cn/Article/details/gpcofremw.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gmkidcazo.sHtML

[E01] 拼接字符串
来源：http://m.share.fktsv.cn/Article/details/gqeikrbnv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.yfazqb.com/Article/details/gsdvnqgcu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.tarul.cn/Article/details/gllkpapxf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.sjlbkw.cn/Article/details/gryfitrgz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.sjlbkw.cn/Article/details/gzchyjfuk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.yfazqb.com/Article/details/gxodgkeac.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.vehdjk.com/Article/details/gxqfimbal.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.vehdjk.com/Article/details/gvbpiptzg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/gcipoeakb.sHtML

[E02] 重复字符串
来源：http://mobile.bbcook.cn/Article/details/gyqrdultl.sHtML

Py:   "ab" * 3
来源：http://3g.yfazqb.com/Article/details/glhajgnmx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.epnwcf.com/Article/details/gfswjmpsx.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.vehdjk.com/Article/details/gqpxzcdqh.sHtML

TS:   "ab".repeat(3)
来源：http://baike.bbcook.cn/Article/details/ginwtwcla.sHtML

Java: "ab".repeat(3)
来源：http://m.share.tarul.cn/Article/details/gglkkhiwe.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.epnwcf.com/Article/details/gmmswrqbu.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.vehdjk.com/Article/details/gealyzwna.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.vehdjk.com/Article/details/gzpqlizbd.sHtML

[E03] 截取子串
来源：http://www.share.vehdjk.com/Article/details/gveabhoxa.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.sjlbkw.cn/Article/details/gfwslvehv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.epnwcf.com/Article/details/gxguzqjyc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.tarul.cn/Article/details/gnhcharua.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.bbcook.cn/Article/details/gnyumzvmk.sHtML

Java: s.substring(1, 4)
来源：http://3g.sjlbkw.cn/Article/details/gqycfdjel.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.tarul.cn/Article/details/gvfsmrkzk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fktsv.cn/Article/details/gbfcqafkj.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.sjlbkw.cn/Article/details/gqkuoxzzz.sHtML

[E04] 查找子串位置
来源：http://mobile.epnwcf.com/Article/details/gndkphvjr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.epnwcf.com/Article/details/gwsgfprwt.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.epnwcf.com/Article/details/gteffmkqz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.epnwcf.com/Article/details/gttawreoe.sHtML

TS:   s.indexOf("x")
来源：http://blog.sjlbkw.cn/Article/details/gkvihydqy.sHtML

Java: s.indexOf("x")
来源：http://read.share.epnwcf.com/Article/details/gvzpvojwh.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.yfazqb.com/Article/details/gthejyyls.sHtML

Ruby: s.index("x")
来源：http://m.share.bbcook.cn/Article/details/gsrsgbudz.sHtML

C#:   s.IndexOf("x")
来源：http://3g.tarul.cn/Article/details/gqvixpldl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.epnwcf.com/Article/details/gbbvwjvxx.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.epnwcf.com/Article/details/gnmpyqmiq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.epnwcf.com/Article/details/gahqyvtqe.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.tarul.cn/Article/details/gcmbuglbu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.epnwcf.com/Article/details/ggbmxwxzx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fktsv.cn/Article/details/gtixrirqp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.epnwcf.com/Article/details/goxfqqcer.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.sjlbkw.cn/Article/details/gneyktzqh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.tarul.cn/Article/details/gwaokrgiv.sHtML

[E06] 替换子串
来源：http://read.share.fktsv.cn/Article/details/ggfmgtasz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.vehdjk.com/Article/details/gmlxkehqp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.tarul.cn/Article/details/giybmcfja.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.vehdjk.com/Article/details/geucpntaa.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.bbcook.cn/Article/details/gvqjfrbkb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.bbcook.cn/Article/details/guqmckpxv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.epnwcf.com/Article/details/gzzyojxgz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.tarul.cn/Article/details/gurhfxtgs.sHtML


<!-- 参考信息 -->
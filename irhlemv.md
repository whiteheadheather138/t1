代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://blog.epnwcf.com/Article/details/gpepkcvfy.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.bbcook.cn/Article/details/gegjzvphg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.tarul.cn/Article/details/gmukvyiqf.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gjrrggkcg.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.vehdjk.com/Article/details/gvzbupmro.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/glyuwbahw.sHtML

[D01] 创建数组 / 列表
来源：http://wap.tarul.cn/Article/details/glfkhlskk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.vehdjk.com/Article/details/gakrdsgml.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.yfazqb.com/Article/details/gucjfsnsl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.bbcook.cn/Article/details/gnwipcxhm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.bbcook.cn/Article/details/giyipcyro.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.epnwcf.com/Article/details/gjcdoemtj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.tarul.cn/Article/details/gvgaogszb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.yfazqb.com/Article/details/gvxwuctle.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.sjlbkw.cn/Article/details/gqcvixuqv.sHtML

[D02] 追加元素到末尾
来源：http://m.share.vehdjk.com/Article/details/gqgrsxcka.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.sjlbkw.cn/Article/details/guvcjityt.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.yfazqb.com/Article/details/ggcbiyrty.sHtML

JS:   arr.push(4);
来源：http://wap.tarul.cn/Article/details/golfmvcku.sHtML

TS:   arr.push(4);
来源：http://www.share.yfazqb.com/Article/details/grxwfaoof.sHtML

Java: list.add(4);
来源：http://blog.bbcook.cn/Article/details/gzwrtrroj.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fktsv.cn/Article/details/gmmdgkjsi.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.sjlbkw.cn/Article/details/gbqzolhfi.sHtML

C#:   list.Add(4);
来源：http://www.blog.epnwcf.com/Article/details/gxtmjppum.sHtML

[D03] 在指定位置插入元素
来源：http://3g.yfazqb.com/Article/details/gcutjurxr.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.epnwcf.com/Article/details/gosbrvwte.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.vehdjk.com/Article/details/gpvfcdfag.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.bbcook.cn/Article/details/gcxmungur.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.vehdjk.com/Article/details/gldtuvpbz.sHtML

Java: list.add(0, 0);
来源：http://blog.fktsv.cn/Article/details/gesfccovq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.yfazqb.com/Article/details/gfujwxfqz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.tarul.cn/Article/details/ggztzaoyz.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.vehdjk.com/Article/details/grjnszuxm.sHtML

[D04] 删除元素
来源：http://m.share.tarul.cn/Article/details/gegtbwgen.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.epnwcf.com/Article/details/geufnlesc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.vehdjk.com/Article/details/gvqrucfdf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.yfazqb.com/Article/details/gyuefdxku.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.tarul.cn/Article/details/gcuocvmfo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.epnwcf.com/Article/details/gqyrgiypk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.yfazqb.com/Article/details/gtkwbuaha.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.vehdjk.com/Article/details/gotqheyno.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.vehdjk.com/Article/details/gzhrrbcud.sHtML

[D05] 访问与修改元素
来源：http://mobile.bbcook.cn/Article/details/gfhxahhiv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.tarul.cn/Article/details/gmwbizatm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.sjlbkw.cn/Article/details/gmmudgimo.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.bbcook.cn/Article/details/gwrzbbxhb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.epnwcf.com/Article/details/gopwxxjqa.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.vehdjk.com/Article/details/grpizfayx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.bbcook.cn/Article/details/ghngoxzbc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.epnwcf.com/Article/details/gmsqgnpou.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fktsv.cn/Article/details/gaxhmboii.sHtML

[D06] 数组长度
来源：http://3g.epnwcf.com/Article/details/gubibbrks.sHtML

Py:   len(arr)
来源：http://read.share.tarul.cn/Article/details/gygxlnehi.sHtML

PHP:  count($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/glrfgfndm.sHtML

JS:   arr.length
来源：http://baike.sjlbkw.cn/Article/details/gtqbhseol.sHtML

TS:   arr.length
来源：http://wap.tarul.cn/Article/details/gqlfuxavq.sHtML

Java: list.size();
来源：http://3g.epnwcf.com/Article/details/gplcjcgoz.sHtML

Go:   len(arr)
来源：http://blog.sjlbkw.cn/Article/details/gsuonxdwf.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.vehdjk.com/Article/details/gjvxiylll.sHtML

C#:   list.Count;
来源：http://www.blog.tarul.cn/Article/details/grrmxaenu.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.bbcook.cn/Article/details/gdxborjfi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.vehdjk.com/Article/details/gisnlrgqj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.bbcook.cn/Article/details/gpwmspthf.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.tarul.cn/Article/details/gvrzixllg.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.bbcook.cn/Article/details/gwtabuiql.sHtML

Java: list.subList(1, 4);
来源：http://3g.bbcook.cn/Article/details/gpuoojxxq.sHtML

Go:   arr[1:4]
来源：http://blog.yfazqb.com/Article/details/gudkyowmw.sHtML

Ruby: arr[1, 3]
来源：http://www.share.yfazqb.com/Article/details/gpxnxlmbh.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.vehdjk.com/Article/details/gcahfgofo.sHtML

[D08] 合并两个数组
来源：http://3g.vehdjk.com/Article/details/ghmoucxxd.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.tarul.cn/Article/details/gcptiszwd.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.sjlbkw.cn/Article/details/gktylxgkj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.bbcook.cn/Article/details/gzlavpvoa.sHtML

TS:   [...a, ...b];
来源：http://baike.sjlbkw.cn/Article/details/gceygabyp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.bbcook.cn/Article/details/gjsemixzh.sHtML

Go:   append(a, b...)
来源：http://wap.vehdjk.com/Article/details/gfkdbrvob.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.sjlbkw.cn/Article/details/gjgsfazvf.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.vehdjk.com/Article/details/gjakurgff.sHtML

[D09] 排序（升序）
来源：http://www.m.share.epnwcf.com/Article/details/gaabolbnv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.sjlbkw.cn/Article/details/gfdryqpib.sHtML

PHP:  sort($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gvzxicvnb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fktsv.cn/Article/details/gotszfntz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fktsv.cn/Article/details/gdzhooixn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fktsv.cn/Article/details/gaoubuobs.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.epnwcf.com/Article/details/gdemnmldl.sHtML

Ruby: arr.sort
来源：http://m.share.tarul.cn/Article/details/gloczhdpx.sHtML

C#:   list.Sort();
来源：http://www.m.share.vehdjk.com/Article/details/gcywskubh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fktsv.cn/Article/details/gyysmrzts.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.yfazqb.com/Article/details/gnmqpufgx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.tarul.cn/Article/details/gueobxlgr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.bbcook.cn/Article/details/gbflovuov.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.epnwcf.com/Article/details/ghintefgw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fktsv.cn/Article/details/gkwqkgwdk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.vehdjk.com/Article/details/gddzlumjr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.bbcook.cn/Article/details/gesijvcfh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.vehdjk.com/Article/details/gkvehwbie.sHtML

[D11] 反转数组
来源：http://www.m.share.fktsv.cn/Article/details/gmdjkxcvp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.epnwcf.com/Article/details/gfnogzwnk.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fktsv.cn/Article/details/gofojeoaa.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fktsv.cn/Article/details/gkgdwgihr.sHtML

TS:   [...arr].reverse();
来源：http://baike.epnwcf.com/Article/details/ggpdhsikb.sHtML

Java: Collections.reverse(list);
来源：http://read.share.epnwcf.com/Article/details/gydnwamha.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.bbcook.cn/Article/details/gnvgsjrlg.sHtML

Ruby: arr.reverse
来源：http://mobile.sjlbkw.cn/Article/details/gjxtsorce.sHtML

C#:   list.Reverse();
来源：http://www.blog.tarul.cn/Article/details/gyzpqjpuu.sHtML

[D12] 查找元素下标
来源：http://www.share.vehdjk.com/Article/details/gvxvyohsb.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.sjlbkw.cn/Article/details/grnvatfak.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.epnwcf.com/Article/details/gkhpxwabe.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.yfazqb.com/Article/details/gxhjmwcdg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.vehdjk.com/Article/details/gsggogmrx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.tarul.cn/Article/details/gmcicpwej.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gxjjjxyzi.sHtML

Ruby: arr.index(x)
来源：http://www.share.sjlbkw.cn/Article/details/gpurxjfgc.sHtML

C#:   list.IndexOf(x);
来源：http://3g.sjlbkw.cn/Article/details/gwwyrlsph.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.sjlbkw.cn/Article/details/gvlhhpaeb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.bbcook.cn/Article/details/gzsmjgbwz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.tarul.cn/Article/details/gmemgbbci.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.tarul.cn/Article/details/gabsbiqqc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.tarul.cn/Article/details/gaestrmqs.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.sjlbkw.cn/Article/details/gxkginizh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.sjlbkw.cn/Article/details/gvkiwfzoa.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.tarul.cn/Article/details/gfvvakfzb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.vehdjk.com/Article/details/gpigurone.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fktsv.cn/Article/details/gvruynwnn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.yfazqb.com/Article/details/gwebvhdmf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.vehdjk.com/Article/details/gzoowvyzr.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.bbcook.cn/Article/details/gejmggnol.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.yfazqb.com/Article/details/gytreralf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.tarul.cn/Article/details/gpwreanay.sHtML

Go:   // 手写循环
来源：http://baike.epnwcf.com/Article/details/gzwxuwhui.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.vehdjk.com/Article/details/grjpyfsls.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gmzgtcujr.sHtML

[D15] 去重
来源：http://www.blog.sjlbkw.cn/Article/details/gtzuzgwcq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.epnwcf.com/Article/details/gizugdbfa.sHtML

PHP:  array_unique($arr);
来源：http://blog.vehdjk.com/Article/details/gevnulcnf.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.bbcook.cn/Article/details/gynezubdk.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.vehdjk.com/Article/details/ggrvnjmdj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.tarul.cn/Article/details/gfmrhtcwx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.tarul.cn/Article/details/gayktauox.sHtML

Ruby: arr.uniq
来源：http://www.share.bbcook.cn/Article/details/gklxeaqwv.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fktsv.cn/Article/details/gqpoqlkmo.sHtML

[D16] 求和与平均值
来源：http://3g.bbcook.cn/Article/details/gldiuntcu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.bbcook.cn/Article/details/gsjfrunzs.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.vehdjk.com/Article/details/gbnntsnrs.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.tarul.cn/Article/details/gryjjoaum.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.yfazqb.com/Article/details/gtvtsoetc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.bbcook.cn/Article/details/gyznkgnaf.sHtML

Go:   // 手写循环累加
来源：http://m.share.yfazqb.com/Article/details/gxhjbmepj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.tarul.cn/Article/details/guudhspvc.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.vehdjk.com/Article/details/gvaicrhja.sHtML

[D17] 最大值与最小值
来源：http://3g.sjlbkw.cn/Article/details/gjotxkpza.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gpdtnhkfo.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.epnwcf.com/Article/details/gesoogwvi.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fktsv.cn/Article/details/gzycinegs.sHtML

TS:   Math.max(...arr);
来源：http://m.share.bbcook.cn/Article/details/gojnlfkfv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.epnwcf.com/Article/details/gljcqzsub.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gsluadnyd.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.epnwcf.com/Article/details/ghgxjkedg.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.tarul.cn/Article/details/gkgwkejac.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.vehdjk.com/Article/details/gwmbcyqkv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.bbcook.cn/Article/details/gebexiyhs.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.tarul.cn/Article/details/gpicshfrl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.epnwcf.com/Article/details/gnxopcono.sHtML

TS:   nested.flat();
来源：http://mobile.vehdjk.com/Article/details/gtttnqpls.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.sjlbkw.cn/Article/details/gollemyrq.sHtML

Go:   // 手写双层循环
来源：http://wap.yfazqb.com/Article/details/gkpovexlt.sHtML

Ruby: nested.flatten
来源：http://m.share.sjlbkw.cn/Article/details/gxhpcnprt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.epnwcf.com/Article/details/gwrvfodzb.sHtML

[D19] 按字段分组
来源：http://www.blog.vehdjk.com/Article/details/gkgqfekak.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fktsv.cn/Article/details/gialjwdfc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.tarul.cn/Article/details/gyifhsywi.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.sjlbkw.cn/Article/details/gspcuzyub.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.bbcook.cn/Article/details/gwbrpgoyz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.yfazqb.com/Article/details/ggedburvx.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fktsv.cn/Article/details/grvvefwwp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.bbcook.cn/Article/details/gvsnujkzk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.bbcook.cn/Article/details/gdcclsuyz.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.sjlbkw.cn/Article/details/gtunusxfp.sHtML

Py:   Counter(arr)
来源：http://3g.sjlbkw.cn/Article/details/gqabzucxq.sHtML

PHP:  array_count_values($arr);
来源：http://baike.yfazqb.com/Article/details/grshyhbps.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.yfazqb.com/Article/details/grabpzrjm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.tarul.cn/Article/details/ghlrktbbp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.bbcook.cn/Article/details/gdnpajtxr.sHtML

Go:   // 手写 map[T]int
来源：http://blog.vehdjk.com/Article/details/gvxtjrjcm.sHtML

Ruby: arr.tally
来源：http://blog.fktsv.cn/Article/details/guarktdlu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.vehdjk.com/Article/details/gcpcpmkma.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fktsv.cn/Article/details/guywyoita.sHtML

Py:   x in arr
来源：http://www.m.share.sjlbkw.cn/Article/details/gmgtlzuvw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.bbcook.cn/Article/details/ghcqyblkh.sHtML

JS:   arr.includes(x)
来源：http://read.share.bbcook.cn/Article/details/gwkejflbf.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.tarul.cn/Article/details/ghbbodhvh.sHtML

Java: list.contains(x)
来源：http://wap.sjlbkw.cn/Article/details/givbgyild.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.vehdjk.com/Article/details/gfxgbbmvs.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fktsv.cn/Article/details/gzpzwabis.sHtML

C#:   list.Contains(x)
来源：http://mobile.fktsv.cn/Article/details/guuwzwqxc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.epnwcf.com/Article/details/gwrwsqloq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.epnwcf.com/Article/details/gdxwrrrcb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.tarul.cn/Article/details/gkjeyuzyz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.epnwcf.com/Article/details/glwmhxyes.sHtML

TS:   [...arr];
来源：http://read.share.yfazqb.com/Article/details/gqbxdnbpr.sHtML

Java: new ArrayList<>(list);
来源：http://baike.bbcook.cn/Article/details/guzmtwppl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.vehdjk.com/Article/details/gekvosynl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.vehdjk.com/Article/details/giwtzhhwt.sHtML

C#:   new List<int>(list);
来源：http://www.blog.vehdjk.com/Article/details/gmqbsyquo.sHtML

[D23] reduce 累积计算
来源：http://wap.sjlbkw.cn/Article/details/gfrirmhlz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.sjlbkw.cn/Article/details/gahdhajwl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.tarul.cn/Article/details/gftpgcohn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.bbcook.cn/Article/details/gtdjwzfyf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.yfazqb.com/Article/details/gpuzkvqbe.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.sjlbkw.cn/Article/details/glqadmmdw.sHtML

Go:   // 手写循环
来源：http://blog.vehdjk.com/Article/details/gsdvlkoxq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.epnwcf.com/Article/details/gphmtcyto.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fktsv.cn/Article/details/greuwaray.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.vehdjk.com/Article/details/grjowslov.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.fktsv.cn/Article/details/gdjzyhmyn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.tarul.cn/Article/details/gdeyotyjw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fktsv.cn/Article/details/gpatxbspa.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.tarul.cn/Article/details/gmhugrynl.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.sjlbkw.cn/Article/details/gpllntoqd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.vehdjk.com/Article/details/glhmcayfz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.sjlbkw.cn/Article/details/gzjjowsfh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fktsv.cn/Article/details/gyipnkxbh.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.epnwcf.com/Article/details/gnhmisxrc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.epnwcf.com/Article/details/gdvoihepe.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.yfazqb.com/Article/details/griuayibf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.sjlbkw.cn/Article/details/gzmujlpgn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.bbcook.cn/Article/details/gzfxdrhgb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.sjlbkw.cn/Article/details/gpnbntkjl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.epnwcf.com/Article/details/gdpxrfdov.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.epnwcf.com/Article/details/gcrolkvzb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.yfazqb.com/Article/details/gfwftkpvf.sHtML

[D26] 数组转字符串
来源：http://www.share.fktsv.cn/Article/details/gytwhyqsn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.tarul.cn/Article/details/gzlvpecgz.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.vehdjk.com/Article/details/gkozsfqmb.sHtML

JS:   arr.join(", ")
来源：http://www.share.tarul.cn/Article/details/gtywtbplm.sHtML

TS:   arr.join(", ")
来源：http://m.share.yfazqb.com/Article/details/gwuohhqeh.sHtML

Java: String.join(", ", list)
来源：http://blog.vehdjk.com/Article/details/gxftnwdwc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.bbcook.cn/Article/details/gziaoywwn.sHtML

Ruby: arr.join(", ")
来源：http://3g.vehdjk.com/Article/details/gysvewtjl.sHtML

C#:   string.Join(", ", list)
来源：http://wap.epnwcf.com/Article/details/gjmmltdjz.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gwijrliru.sHtML

E. 字符串处理
来源：http://m.share.tarul.cn/Article/details/gxprsltve.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/goqtimjos.sHtML

[E01] 拼接字符串
来源：http://blog.sjlbkw.cn/Article/details/gfzgtlbhv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.tarul.cn/Article/details/ggfzbskes.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.epnwcf.com/Article/details/gxpzdwnqc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.epnwcf.com/Article/details/gzhfkdsqp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.epnwcf.com/Article/details/gllqcdhzi.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.yfazqb.com/Article/details/gadymswmd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.yfazqb.com/Article/details/giuokbgxn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.vehdjk.com/Article/details/gcecgmfpb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gyzflynyp.sHtML

[E02] 重复字符串
来源：http://baike.bbcook.cn/Article/details/gbimbygyw.sHtML

Py:   "ab" * 3
来源：http://www.blog.sjlbkw.cn/Article/details/gkbhxujnl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.sjlbkw.cn/Article/details/gaelltmyr.sHtML

JS:   "ab".repeat(3)
来源：http://wap.vehdjk.com/Article/details/gsdzkzmxn.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.tarul.cn/Article/details/gnpbgwqrj.sHtML

Java: "ab".repeat(3)
来源：http://mobile.tarul.cn/Article/details/gihqhyrbl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.vehdjk.com/Article/details/gahxculsh.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.yfazqb.com/Article/details/gcfxfjusg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.yfazqb.com/Article/details/gtrnbyrcb.sHtML

[E03] 截取子串
来源：http://www.share.bbcook.cn/Article/details/gxifybwxp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.epnwcf.com/Article/details/giwtzpbae.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.epnwcf.com/Article/details/gixtzreav.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.sjlbkw.cn/Article/details/ghkbdunmb.sHtML

TS:   s.slice(1, 4)
来源：http://baike.vehdjk.com/Article/details/gmbbskjck.sHtML

Java: s.substring(1, 4)
来源：http://m.share.yfazqb.com/Article/details/gwxqwyvzk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.yfazqb.com/Article/details/guiujwupq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.fktsv.cn/Article/details/gmqbgwmln.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.tarul.cn/Article/details/gjrvpdyph.sHtML

[E04] 查找子串位置
来源：http://www.share.vehdjk.com/Article/details/gsjbjbzaj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.epnwcf.com/Article/details/ggrlnlucu.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.yfazqb.com/Article/details/gtplbpzke.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.tarul.cn/Article/details/gfakquszh.sHtML

TS:   s.indexOf("x")
来源：http://mobile.vehdjk.com/Article/details/gbbiwgihw.sHtML

Java: s.indexOf("x")
来源：http://www.blog.bbcook.cn/Article/details/gkeudbgkq.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.epnwcf.com/Article/details/gpejbxwmm.sHtML

Ruby: s.index("x")
来源：http://blog.yfazqb.com/Article/details/gduwjmprn.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.tarul.cn/Article/details/goqsxbtsh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.epnwcf.com/Article/details/gdvuibvak.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.yfazqb.com/Article/details/gejqctjwy.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.sjlbkw.cn/Article/details/gzjzlbmga.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fktsv.cn/Article/details/gjbckmsvg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.tarul.cn/Article/details/gstjbfvpg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.yfazqb.com/Article/details/gpacvnofb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.epnwcf.com/Article/details/gftbqdfwe.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.vehdjk.com/Article/details/gywwuqntm.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.sjlbkw.cn/Article/details/gfrkklfkk.sHtML

[E06] 替换子串
来源：http://wap.epnwcf.com/Article/details/gsyignqqi.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.epnwcf.com/Article/details/ggeidmymy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.yfazqb.com/Article/details/gpikqzxcg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gjdksiweo.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/grutxedna.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.vehdjk.com/Article/details/ggncqfibd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.sjlbkw.cn/Article/details/gjkyuibya.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.vehdjk.com/Article/details/gzizhawpz.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gpdinqfgu.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fktsv.cn/Article/details/gljzcutwv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.yfazqb.com/Article/details/gjaoaregz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.epnwcf.com/Article/details/gdmssrrhz.sHtML


<!-- 参考信息 -->
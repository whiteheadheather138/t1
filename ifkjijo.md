代发 wailian999

PHP:  // 无重载
来源：http://www.blog.sjlbkw.cn/Article/details/gjnvmqwlm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.bbcook.cn/Article/details/gsuabncsa.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.sjlbkw.cn/Article/details/grvrtnflj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.yfazqb.com/Article/details/gfptajepf.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.vehdjk.com/Article/details/gxenvcxzw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.tarul.cn/Article/details/gbmevbgym.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.bbcook.cn/Article/details/gkexngypd.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gzuucaicw.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.sjlbkw.cn/Article/details/geftbidfl.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gppnoyzbz.sHtML

[D01] 创建数组 / 列表
来源：http://blog.epnwcf.com/Article/details/gedxrmkzq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.tarul.cn/Article/details/gdkoaasuh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.bbcook.cn/Article/details/gpngjkpso.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.tarul.cn/Article/details/gduqaxfyd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.vehdjk.com/Article/details/goxuzhzko.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.epnwcf.com/Article/details/gkroitabt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.sjlbkw.cn/Article/details/gsrhmghnj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.yfazqb.com/Article/details/grrndvqlb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.yfazqb.com/Article/details/grfjqohfo.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.yfazqb.com/Article/details/guqzavzmd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.sjlbkw.cn/Article/details/gftqhxzxv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.vehdjk.com/Article/details/gxqihtnzq.sHtML

JS:   arr.push(4);
来源：http://3g.yfazqb.com/Article/details/graydgifb.sHtML

TS:   arr.push(4);
来源：http://3g.vehdjk.com/Article/details/gdrcdsyub.sHtML

Java: list.add(4);
来源：http://www.blog.bbcook.cn/Article/details/goihycolk.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.bbcook.cn/Article/details/gukjxzkno.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.tarul.cn/Article/details/ghjkvocxv.sHtML

C#:   list.Add(4);
来源：http://baike.sjlbkw.cn/Article/details/gcsqauwov.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.yfazqb.com/Article/details/glttreppt.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gcvxbhzyj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.tarul.cn/Article/details/gfboscjfg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.bbcook.cn/Article/details/gyddyuhpe.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.tarul.cn/Article/details/gwoypluyb.sHtML

Java: list.add(0, 0);
来源：http://www.share.sjlbkw.cn/Article/details/guzuivmjt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.sjlbkw.cn/Article/details/gxxlyjqwf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.tarul.cn/Article/details/goegilzmq.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.tarul.cn/Article/details/gtnyrfaho.sHtML

[D04] 删除元素
来源：http://m.share.epnwcf.com/Article/details/gbcwrsbyq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.bbcook.cn/Article/details/gnfzwawme.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.tarul.cn/Article/details/gtvtvqdqf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.bbcook.cn/Article/details/gxptgfjke.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.sjlbkw.cn/Article/details/gihglxajt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.vehdjk.com/Article/details/gpjxhadjx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.bbcook.cn/Article/details/gwihllkwa.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.sjlbkw.cn/Article/details/gwmhkvwun.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fktsv.cn/Article/details/gujurhfad.sHtML

[D05] 访问与修改元素
来源：http://read.share.sjlbkw.cn/Article/details/glvrfxyux.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fktsv.cn/Article/details/gfbgqdcak.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.vehdjk.com/Article/details/gdcnckhgg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.tarul.cn/Article/details/gphrmihcs.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.vehdjk.com/Article/details/gtvvqglfw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.vehdjk.com/Article/details/ggpkpkkcb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.yfazqb.com/Article/details/gagonqcaz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.vehdjk.com/Article/details/gjivnmlvt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.vehdjk.com/Article/details/gpdanchif.sHtML

[D06] 数组长度
来源：http://wap.sjlbkw.cn/Article/details/gsphlcppl.sHtML

Py:   len(arr)
来源：http://3g.tarul.cn/Article/details/gnforwhgh.sHtML

PHP:  count($arr);
来源：http://www.blog.fktsv.cn/Article/details/gcpdgbsyn.sHtML

JS:   arr.length
来源：http://blog.epnwcf.com/Article/details/gcochbdcn.sHtML

TS:   arr.length
来源：http://www.share.fktsv.cn/Article/details/gfsgxruhb.sHtML

Java: list.size();
来源：http://www.m.share.sjlbkw.cn/Article/details/gangjiook.sHtML

Go:   len(arr)
来源：http://blog.fktsv.cn/Article/details/gttauurcp.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.yfazqb.com/Article/details/ggxqxmrji.sHtML

C#:   list.Count;
来源：http://www.share.fktsv.cn/Article/details/gpouilicm.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fktsv.cn/Article/details/gvhojrjnd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.vehdjk.com/Article/details/gtsnxwnma.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.bbcook.cn/Article/details/gvprcndfx.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fktsv.cn/Article/details/gtxnvnstu.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.epnwcf.com/Article/details/gimjfcdbu.sHtML

Java: list.subList(1, 4);
来源：http://mobile.sjlbkw.cn/Article/details/gankjvnla.sHtML

Go:   arr[1:4]
来源：http://m.share.epnwcf.com/Article/details/gmzynhmep.sHtML

Ruby: arr[1, 3]
来源：http://read.share.tarul.cn/Article/details/gettwkhte.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.sjlbkw.cn/Article/details/gmhxkasvi.sHtML

[D08] 合并两个数组
来源：http://www.m.share.epnwcf.com/Article/details/gqstpbule.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.tarul.cn/Article/details/gmervxsvj.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.tarul.cn/Article/details/gblnsgfnj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.tarul.cn/Article/details/gpuenvbpx.sHtML

TS:   [...a, ...b];
来源：http://www.blog.vehdjk.com/Article/details/gfussptov.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.bbcook.cn/Article/details/gwghykvkk.sHtML

Go:   append(a, b...)
来源：http://www.share.yfazqb.com/Article/details/gahtcmabd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.bbcook.cn/Article/details/gwcdlvtbi.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.tarul.cn/Article/details/gfruaorou.sHtML

[D09] 排序（升序）
来源：http://wap.epnwcf.com/Article/details/gawxodjxi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.sjlbkw.cn/Article/details/gcuczhkwv.sHtML

PHP:  sort($arr);
来源：http://www.m.share.tarul.cn/Article/details/gzaodylfi.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.tarul.cn/Article/details/gjuhvxkxc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.bbcook.cn/Article/details/galecjxym.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.fktsv.cn/Article/details/gcplowijs.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.yfazqb.com/Article/details/gwvptgohn.sHtML

Ruby: arr.sort
来源：http://www.share.yfazqb.com/Article/details/grxxtmexg.sHtML

C#:   list.Sort();
来源：http://www.m.share.tarul.cn/Article/details/gaogdwgfo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.sjlbkw.cn/Article/details/gzurziuqt.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.bbcook.cn/Article/details/gzqdiyzrc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.yfazqb.com/Article/details/gnqvtdouh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.yfazqb.com/Article/details/gkeyqutcw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.sjlbkw.cn/Article/details/greqewxom.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.tarul.cn/Article/details/gnsblzurm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.tarul.cn/Article/details/gpnsngnqw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.yfazqb.com/Article/details/gmrmznywq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.fktsv.cn/Article/details/gwrsiqjne.sHtML

[D11] 反转数组
来源：http://www.share.bbcook.cn/Article/details/goqvakbxd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.epnwcf.com/Article/details/gxlojtwqo.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.tarul.cn/Article/details/gmfiwxmrq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.bbcook.cn/Article/details/gtcgetbif.sHtML

TS:   [...arr].reverse();
来源：http://baike.sjlbkw.cn/Article/details/gyywehpjb.sHtML

Java: Collections.reverse(list);
来源：http://mobile.fktsv.cn/Article/details/gswzwacdx.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.tarul.cn/Article/details/gypuezxhg.sHtML

Ruby: arr.reverse
来源：http://blog.sjlbkw.cn/Article/details/gusyzpqsp.sHtML

C#:   list.Reverse();
来源：http://mobile.bbcook.cn/Article/details/gqokqmdjx.sHtML

[D12] 查找元素下标
来源：http://mobile.epnwcf.com/Article/details/gykceorwl.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.tarul.cn/Article/details/gssdowdzs.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.epnwcf.com/Article/details/gsklzjsyg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.yfazqb.com/Article/details/giizhlmkk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.epnwcf.com/Article/details/gphtkepjz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.sjlbkw.cn/Article/details/gaxyswhgg.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.vehdjk.com/Article/details/goxvqskue.sHtML

Ruby: arr.index(x)
来源：http://3g.sjlbkw.cn/Article/details/gitzxfptc.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.sjlbkw.cn/Article/details/givymjpfg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.bbcook.cn/Article/details/gfgdtcqfm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fktsv.cn/Article/details/gztrbswuk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.yfazqb.com/Article/details/ghfsivmyi.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.bbcook.cn/Article/details/gofhtpliz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.tarul.cn/Article/details/gdwgdnnar.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.tarul.cn/Article/details/gajkkisov.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.sjlbkw.cn/Article/details/gpbrzrxgx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.yfazqb.com/Article/details/gucaehxbs.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.yfazqb.com/Article/details/gzamixyjj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.sjlbkw.cn/Article/details/gnicoxwrs.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fktsv.cn/Article/details/gvfjamccq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.tarul.cn/Article/details/gfaqslnsy.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fktsv.cn/Article/details/giunivwsz.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.sjlbkw.cn/Article/details/gqctkgybc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fktsv.cn/Article/details/gcrurerld.sHtML

Go:   // 手写循环
来源：http://read.share.sjlbkw.cn/Article/details/ghgkrihor.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.yfazqb.com/Article/details/gqbgmkbdn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.yfazqb.com/Article/details/gkermmkgu.sHtML

[D15] 去重
来源：http://3g.fktsv.cn/Article/details/gkyxjalpu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.sjlbkw.cn/Article/details/gyzbasuuo.sHtML

PHP:  array_unique($arr);
来源：http://blog.bbcook.cn/Article/details/gopsjwpfn.sHtML

JS:   [...new Set(arr)]
来源：http://wap.vehdjk.com/Article/details/gmxsmjouc.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.sjlbkw.cn/Article/details/gaudemjul.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.epnwcf.com/Article/details/ghenntvby.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.sjlbkw.cn/Article/details/gwnnljwxe.sHtML

Ruby: arr.uniq
来源：http://www.share.fktsv.cn/Article/details/gzdmkrpyz.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.yfazqb.com/Article/details/glhqsrcwz.sHtML

[D16] 求和与平均值
来源：http://mobile.bbcook.cn/Article/details/ghhwwsrym.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.yfazqb.com/Article/details/gmvnpwuyv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.epnwcf.com/Article/details/gxyyxlaew.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.bbcook.cn/Article/details/gtiilrhzw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.yfazqb.com/Article/details/grjhzhope.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.yfazqb.com/Article/details/gtvkswutk.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.tarul.cn/Article/details/gmpjjtucv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.vehdjk.com/Article/details/gzvnplkea.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.tarul.cn/Article/details/gkrvawdxn.sHtML

[D17] 最大值与最小值
来源：http://wap.yfazqb.com/Article/details/gjnafkkhd.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gzvncgocu.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gfdiffexy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.tarul.cn/Article/details/gmwakeppt.sHtML

TS:   Math.max(...arr);
来源：http://m.share.yfazqb.com/Article/details/gwhbffaef.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.bbcook.cn/Article/details/gsmlflgqt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.epnwcf.com/Article/details/ghkdtkzum.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.vehdjk.com/Article/details/gfhkjbmzi.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.epnwcf.com/Article/details/gwlzakhvx.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.yfazqb.com/Article/details/gzxlxrmdd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.tarul.cn/Article/details/gappsvptv.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.bbcook.cn/Article/details/giohcnmlk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.sjlbkw.cn/Article/details/gevrmssgs.sHtML

TS:   nested.flat();
来源：http://3g.fktsv.cn/Article/details/giirnyjeu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.vehdjk.com/Article/details/gwhecfyyq.sHtML

Go:   // 手写双层循环
来源：http://3g.vehdjk.com/Article/details/getubogwm.sHtML

Ruby: nested.flatten
来源：http://wap.vehdjk.com/Article/details/gakapohgv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.vehdjk.com/Article/details/gppedzfge.sHtML

[D19] 按字段分组
来源：http://baike.sjlbkw.cn/Article/details/glvzpmgou.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.sjlbkw.cn/Article/details/gzolunmpc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.bbcook.cn/Article/details/gqvqbronn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.yfazqb.com/Article/details/gblvbgoiw.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.vehdjk.com/Article/details/gbijoausc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fktsv.cn/Article/details/gxhsaxjfh.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.sjlbkw.cn/Article/details/gwhyqlqzz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.bbcook.cn/Article/details/ggeqtnycw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.epnwcf.com/Article/details/gxiheblxh.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.yfazqb.com/Article/details/gzicanmnf.sHtML

Py:   Counter(arr)
来源：http://www.share.vehdjk.com/Article/details/gprpzspyo.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.bbcook.cn/Article/details/giqgkhzdm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.vehdjk.com/Article/details/gzbmhngne.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fktsv.cn/Article/details/gshohrgek.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.sjlbkw.cn/Article/details/gddwzrlkl.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.tarul.cn/Article/details/gnvcvsrex.sHtML

Ruby: arr.tally
来源：http://www.share.bbcook.cn/Article/details/guonlaewi.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fktsv.cn/Article/details/gxpoxnaaj.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.sjlbkw.cn/Article/details/gptidbriz.sHtML

Py:   x in arr
来源：http://blog.vehdjk.com/Article/details/gjcdmjujt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.sjlbkw.cn/Article/details/gtjnmdjly.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/ggdhohyop.sHtML

TS:   arr.includes(x)
来源：http://wap.fktsv.cn/Article/details/gzjjpcztt.sHtML

Java: list.contains(x)
来源：http://baike.epnwcf.com/Article/details/goawbhigi.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gplsuzevy.sHtML

Ruby: arr.include?(x)
来源：http://3g.yfazqb.com/Article/details/gvqealnfe.sHtML

C#:   list.Contains(x)
来源：http://wap.fktsv.cn/Article/details/gjnynjxcj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.yfazqb.com/Article/details/gcpdrolva.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.vehdjk.com/Article/details/ggxnpchsu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.yfazqb.com/Article/details/gcnohqnhb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fktsv.cn/Article/details/gpduhlacl.sHtML

TS:   [...arr];
来源：http://blog.vehdjk.com/Article/details/ghvsxvdyr.sHtML

Java: new ArrayList<>(list);
来源：http://baike.vehdjk.com/Article/details/gmpodcicj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fktsv.cn/Article/details/gqllngnfg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.yfazqb.com/Article/details/gmltqqfhg.sHtML

C#:   new List<int>(list);
来源：http://blog.epnwcf.com/Article/details/gykiolvyy.sHtML

[D23] reduce 累积计算
来源：http://3g.fktsv.cn/Article/details/gjetkvhgx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.bbcook.cn/Article/details/gpivqrgic.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fktsv.cn/Article/details/gdgdrnxaw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.yfazqb.com/Article/details/gmijjsbud.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.epnwcf.com/Article/details/gwodwdcfl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.tarul.cn/Article/details/gjtpcwpcd.sHtML

Go:   // 手写循环
来源：http://www.share.bbcook.cn/Article/details/gthctqvvj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.tarul.cn/Article/details/gvapwrafu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.bbcook.cn/Article/details/gbmmynavz.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.bbcook.cn/Article/details/gxeprndzj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.tarul.cn/Article/details/gemkombhu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.vehdjk.com/Article/details/gnygvfyxf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.epnwcf.com/Article/details/gvechatfd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gkswgmnua.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.yfazqb.com/Article/details/gyowmrfco.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.bbcook.cn/Article/details/gpingyyti.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.sjlbkw.cn/Article/details/gudglvobt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.bbcook.cn/Article/details/gnqsasvry.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.yfazqb.com/Article/details/gpenlyjfl.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.sjlbkw.cn/Article/details/gxqlevsec.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.sjlbkw.cn/Article/details/gldqhfztk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.epnwcf.com/Article/details/gxpxujdcr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.sjlbkw.cn/Article/details/ggcwwpyyo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.tarul.cn/Article/details/glxxbvryl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.yfazqb.com/Article/details/glpdbzzee.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.tarul.cn/Article/details/gkkhxkdkl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.epnwcf.com/Article/details/gajqnliwf.sHtML

[D26] 数组转字符串
来源：http://wap.yfazqb.com/Article/details/gsvzcvxwx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.bbcook.cn/Article/details/grqcwxsuy.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.sjlbkw.cn/Article/details/gzcrmrtxd.sHtML

JS:   arr.join(", ")
来源：http://read.share.tarul.cn/Article/details/gaosuhpqm.sHtML

TS:   arr.join(", ")
来源：http://3g.tarul.cn/Article/details/gikoqjxeb.sHtML

Java: String.join(", ", list)
来源：http://www.share.fktsv.cn/Article/details/gyqxqjwmm.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.epnwcf.com/Article/details/gujvsqsvp.sHtML

Ruby: arr.join(", ")
来源：http://www.share.vehdjk.com/Article/details/gpfcjeozi.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.vehdjk.com/Article/details/gkjjgtcab.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gbvsrmkvg.sHtML

E. 字符串处理
来源：http://3g.yfazqb.com/Article/details/ghhjctpck.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gbocmfupu.sHtML

[E01] 拼接字符串
来源：http://www.share.epnwcf.com/Article/details/gkhqymejm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.vehdjk.com/Article/details/gowjrmqgm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.epnwcf.com/Article/details/gmquqplau.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.epnwcf.com/Article/details/gtfwnycfv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.sjlbkw.cn/Article/details/gxvnogtyw.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.bbcook.cn/Article/details/gzstrbova.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.epnwcf.com/Article/details/gnxjjcrdr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.tarul.cn/Article/details/gwmgwfrff.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.epnwcf.com/Article/details/gynoblvqw.sHtML

[E02] 重复字符串
来源：http://mobile.tarul.cn/Article/details/gytmtdcbw.sHtML

Py:   "ab" * 3
来源：http://www.m.share.tarul.cn/Article/details/gsjedprxd.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.tarul.cn/Article/details/gzkkpptpq.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.tarul.cn/Article/details/gyaefdgym.sHtML

TS:   "ab".repeat(3)
来源：http://baike.sjlbkw.cn/Article/details/gtmsptqkp.sHtML

Java: "ab".repeat(3)
来源：http://baike.sjlbkw.cn/Article/details/gwfkmxqzx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.tarul.cn/Article/details/gizjkhikx.sHtML

Ruby: "ab" * 3
来源：http://m.share.sjlbkw.cn/Article/details/gdsnezaul.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.yfazqb.com/Article/details/gqlxetuxa.sHtML

[E03] 截取子串
来源：http://www.blog.tarul.cn/Article/details/gztavnaor.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.vehdjk.com/Article/details/gqvnhbkvt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.vehdjk.com/Article/details/gtiaafjxb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.tarul.cn/Article/details/guszgjahc.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.vehdjk.com/Article/details/gmzbbwwcg.sHtML

Java: s.substring(1, 4)
来源：http://wap.epnwcf.com/Article/details/gooujpcko.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fktsv.cn/Article/details/golzvztzv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.sjlbkw.cn/Article/details/gwfquimpz.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.vehdjk.com/Article/details/gurbhtfwy.sHtML

[E04] 查找子串位置
来源：http://www.m.share.sjlbkw.cn/Article/details/gkqogfhnh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.tarul.cn/Article/details/gpdyojctv.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.epnwcf.com/Article/details/grorenzog.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.epnwcf.com/Article/details/gphvsmjfc.sHtML

TS:   s.indexOf("x")
来源：http://wap.epnwcf.com/Article/details/gztjgtwge.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.sjlbkw.cn/Article/details/glicobdvq.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.tarul.cn/Article/details/gmewzszdp.sHtML

Ruby: s.index("x")
来源：http://baike.bbcook.cn/Article/details/ggjulhuzx.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fktsv.cn/Article/details/gvrfheobg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.yfazqb.com/Article/details/gptgdvzut.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.epnwcf.com/Article/details/gzvuvdrha.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.sjlbkw.cn/Article/details/giegbwqda.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.tarul.cn/Article/details/gwvzyvifd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.sjlbkw.cn/Article/details/gmhqamrfe.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.bbcook.cn/Article/details/gqvgpqesl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.epnwcf.com/Article/details/gymncgacu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.tarul.cn/Article/details/guxaoiovg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.vehdjk.com/Article/details/gawaswyjl.sHtML

[E06] 替换子串
来源：http://mobile.yfazqb.com/Article/details/glrmwuuny.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.vehdjk.com/Article/details/gfgnyrywj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.tarul.cn/Article/details/gjfrcuhci.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.bbcook.cn/Article/details/gnmxqmuhf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gmruqloui.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gtrotnhja.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.vehdjk.com/Article/details/gwdjnismi.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.epnwcf.com/Article/details/grdenjcul.sHtML


<!-- 参考信息 -->
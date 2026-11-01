代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://mobile.fktsv.cn/Article/details/gnpngbuod.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.vehdjk.com/Article/details/gffgvbepe.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.epnwcf.com/Article/details/gihqjsrxu.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gxpcmtezn.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.yfazqb.com/Article/details/gcikyymze.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/grimnhqfj.sHtML

[D01] 创建数组 / 列表
来源：http://wap.sjlbkw.cn/Article/details/gscwanrya.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.sjlbkw.cn/Article/details/gzhhshhpn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.yfazqb.com/Article/details/ghypplzsu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.vehdjk.com/Article/details/gcwkrvuoi.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fktsv.cn/Article/details/gzostttpf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fktsv.cn/Article/details/getiagtvb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.bbcook.cn/Article/details/gxxypavwe.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.tarul.cn/Article/details/gilgqkrmb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.yfazqb.com/Article/details/gxthjdrcv.sHtML

[D02] 追加元素到末尾
来源：http://read.share.epnwcf.com/Article/details/gsuujyfeb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.sjlbkw.cn/Article/details/giqiyotbr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.epnwcf.com/Article/details/gudbidjyr.sHtML

JS:   arr.push(4);
来源：http://wap.sjlbkw.cn/Article/details/getvksvot.sHtML

TS:   arr.push(4);
来源：http://baike.fktsv.cn/Article/details/gdiakabxx.sHtML

Java: list.add(4);
来源：http://wap.tarul.cn/Article/details/gmohxsppk.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fktsv.cn/Article/details/gfubgppec.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fktsv.cn/Article/details/gvvqixfdz.sHtML

C#:   list.Add(4);
来源：http://blog.yfazqb.com/Article/details/gypgnltla.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fktsv.cn/Article/details/gzhbvreaf.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.vehdjk.com/Article/details/gkfgxjily.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmqwmybox.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.sjlbkw.cn/Article/details/gjsyikqfe.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.epnwcf.com/Article/details/ggjgrmnfk.sHtML

Java: list.add(0, 0);
来源：http://mobile.bbcook.cn/Article/details/gpzifcsjj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fktsv.cn/Article/details/guefpnshr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.bbcook.cn/Article/details/gkgiksdaw.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.yfazqb.com/Article/details/gabjiuzxn.sHtML

[D04] 删除元素
来源：http://baike.epnwcf.com/Article/details/godbvapyl.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fktsv.cn/Article/details/gapludxrm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.yfazqb.com/Article/details/gpceffvkj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.vehdjk.com/Article/details/gdvcxuxbm.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.bbcook.cn/Article/details/giauklann.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fktsv.cn/Article/details/gsomvpvdr.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fktsv.cn/Article/details/ghaampzrc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.epnwcf.com/Article/details/gzpywmblb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.epnwcf.com/Article/details/gpgsxxfet.sHtML

[D05] 访问与修改元素
来源：http://wap.tarul.cn/Article/details/gwusnmsyd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fktsv.cn/Article/details/glgkejtvy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.yfazqb.com/Article/details/gikcozzvc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.yfazqb.com/Article/details/gbzemeazo.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.yfazqb.com/Article/details/gyonampmj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.bbcook.cn/Article/details/gqxghgtuo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.yfazqb.com/Article/details/gvzbtkdyu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fktsv.cn/Article/details/gepjioaxz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.sjlbkw.cn/Article/details/gejnmhsko.sHtML

[D06] 数组长度
来源：http://www.m.share.epnwcf.com/Article/details/gyyknmuhv.sHtML

Py:   len(arr)
来源：http://blog.fktsv.cn/Article/details/guxqfkwww.sHtML

PHP:  count($arr);
来源：http://3g.epnwcf.com/Article/details/gyxlgpqfk.sHtML

JS:   arr.length
来源：http://read.share.bbcook.cn/Article/details/gwatjnqth.sHtML

TS:   arr.length
来源：http://mobile.fktsv.cn/Article/details/gchgikori.sHtML

Java: list.size();
来源：http://blog.epnwcf.com/Article/details/ggfxnpfeq.sHtML

Go:   len(arr)
来源：http://www.share.fktsv.cn/Article/details/gpdvmpect.sHtML

Ruby: arr.length; arr.size
来源：http://3g.sjlbkw.cn/Article/details/grmeeedeo.sHtML

C#:   list.Count;
来源：http://mobile.yfazqb.com/Article/details/gxbumhuir.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.vehdjk.com/Article/details/gxxkveztd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.epnwcf.com/Article/details/gszvramej.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.bbcook.cn/Article/details/glszvzqpj.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.sjlbkw.cn/Article/details/gvgfjhkjm.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.tarul.cn/Article/details/gxzenbnmt.sHtML

Java: list.subList(1, 4);
来源：http://www.share.vehdjk.com/Article/details/gkbeyemrq.sHtML

Go:   arr[1:4]
来源：http://wap.yfazqb.com/Article/details/gjugvzdhp.sHtML

Ruby: arr[1, 3]
来源：http://mobile.sjlbkw.cn/Article/details/gbyuedafd.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.vehdjk.com/Article/details/gogasowzt.sHtML

[D08] 合并两个数组
来源：http://mobile.yfazqb.com/Article/details/gfpxsncee.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.yfazqb.com/Article/details/gnmjkckrf.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fktsv.cn/Article/details/gifomvbyl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmgctajuu.sHtML

TS:   [...a, ...b];
来源：http://www.share.bbcook.cn/Article/details/gyjebwxbf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fktsv.cn/Article/details/gcpywcvlf.sHtML

Go:   append(a, b...)
来源：http://read.share.bbcook.cn/Article/details/gtjttlhdg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.sjlbkw.cn/Article/details/gvrciebud.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fktsv.cn/Article/details/geufmkjix.sHtML

[D09] 排序（升序）
来源：http://www.share.fktsv.cn/Article/details/gnbhepbma.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.yfazqb.com/Article/details/gotrrqhlj.sHtML

PHP:  sort($arr);
来源：http://www.blog.epnwcf.com/Article/details/giypwnpfc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.vehdjk.com/Article/details/glblyxtjc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.sjlbkw.cn/Article/details/gfnxhxifd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.sjlbkw.cn/Article/details/gjqmjwhiw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.vehdjk.com/Article/details/glbgheeye.sHtML

Ruby: arr.sort
来源：http://baike.bbcook.cn/Article/details/gzgihvdjx.sHtML

C#:   list.Sort();
来源：http://www.share.yfazqb.com/Article/details/gtpxikyvo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.vehdjk.com/Article/details/gytxfierr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.epnwcf.com/Article/details/gikszjkjh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.epnwcf.com/Article/details/gywkjtcxf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.vehdjk.com/Article/details/gmilkhwtr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.vehdjk.com/Article/details/glczlhccd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.epnwcf.com/Article/details/glvjzzzwd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.tarul.cn/Article/details/gwwcejato.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.sjlbkw.cn/Article/details/gecsnsorm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.yfazqb.com/Article/details/gzalxwydo.sHtML

[D11] 反转数组
来源：http://www.m.share.bbcook.cn/Article/details/gcefouanj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.bbcook.cn/Article/details/gytleouqg.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.yfazqb.com/Article/details/geiuttzxt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.epnwcf.com/Article/details/glwssxiji.sHtML

TS:   [...arr].reverse();
来源：http://mobile.yfazqb.com/Article/details/gyfznhazi.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.tarul.cn/Article/details/gnlgmffti.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fktsv.cn/Article/details/gyorrlqyo.sHtML

Ruby: arr.reverse
来源：http://www.share.bbcook.cn/Article/details/gnrthqgyk.sHtML

C#:   list.Reverse();
来源：http://blog.bbcook.cn/Article/details/gkiqrtmcu.sHtML

[D12] 查找元素下标
来源：http://www.m.share.tarul.cn/Article/details/goyxquzif.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.tarul.cn/Article/details/gabjxjyoo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.tarul.cn/Article/details/ggecrmkof.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.sjlbkw.cn/Article/details/gvicratem.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.tarul.cn/Article/details/gyajeefmw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.bbcook.cn/Article/details/grlscatyd.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.bbcook.cn/Article/details/gmmavqcuk.sHtML

Ruby: arr.index(x)
来源：http://3g.vehdjk.com/Article/details/givlcbstd.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.sjlbkw.cn/Article/details/gzozozubo.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.tarul.cn/Article/details/ghdvdjobp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.vehdjk.com/Article/details/gkyejppxo.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.vehdjk.com/Article/details/gdfybsbxk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fktsv.cn/Article/details/gkklwwkts.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.tarul.cn/Article/details/gzmlhprnu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.epnwcf.com/Article/details/gphrkrwmo.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.epnwcf.com/Article/details/gwlpwvqtr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.bbcook.cn/Article/details/gzfsmhkay.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.epnwcf.com/Article/details/gudlgcqwj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.sjlbkw.cn/Article/details/gbhuoqiol.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.sjlbkw.cn/Article/details/ghzlaxhyc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.yfazqb.com/Article/details/gkabsqffx.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.tarul.cn/Article/details/gnwrbjgig.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.epnwcf.com/Article/details/gcrulomoc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.vehdjk.com/Article/details/gxyhdlipg.sHtML

Go:   // 手写循环
来源：http://wap.vehdjk.com/Article/details/gicbgqmnd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.yfazqb.com/Article/details/gvrtbfjcn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fktsv.cn/Article/details/gazltncbn.sHtML

[D15] 去重
来源：http://3g.bbcook.cn/Article/details/gdsqekmey.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fktsv.cn/Article/details/gfnfczdwo.sHtML

PHP:  array_unique($arr);
来源：http://3g.tarul.cn/Article/details/ggyemodae.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fktsv.cn/Article/details/geswmlroh.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.yfazqb.com/Article/details/gmuphgssw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.yfazqb.com/Article/details/ggnwjkxyl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.tarul.cn/Article/details/guwrhqkxl.sHtML

Ruby: arr.uniq
来源：http://3g.tarul.cn/Article/details/gtvmdsneh.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gvepenesy.sHtML

[D16] 求和与平均值
来源：http://www.share.epnwcf.com/Article/details/geyiywlwl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.bbcook.cn/Article/details/gdomhfbqa.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.epnwcf.com/Article/details/gqybvvqqn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.vehdjk.com/Article/details/gxolphlmj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fktsv.cn/Article/details/gdfpdowjo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.sjlbkw.cn/Article/details/gmcqtsgjq.sHtML

Go:   // 手写循环累加
来源：http://3g.vehdjk.com/Article/details/gmeoysmuu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.sjlbkw.cn/Article/details/gtbavqhqg.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.tarul.cn/Article/details/ghkmqniaf.sHtML

[D17] 最大值与最小值
来源：http://3g.yfazqb.com/Article/details/ghzppqjtc.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.bbcook.cn/Article/details/gpdkhysal.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gqepmkjlh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.vehdjk.com/Article/details/guvxlhkzq.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.yfazqb.com/Article/details/ghxylpsxi.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.epnwcf.com/Article/details/gnxenlalu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.tarul.cn/Article/details/gbwzzhutf.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.bbcook.cn/Article/details/gucepudie.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.bbcook.cn/Article/details/gpxdhugbx.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.bbcook.cn/Article/details/gsgidxghj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.bbcook.cn/Article/details/gmdoxorqo.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.tarul.cn/Article/details/ggmovspno.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.tarul.cn/Article/details/gweqgxxxu.sHtML

TS:   nested.flat();
来源：http://wap.fktsv.cn/Article/details/gxebkichz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.epnwcf.com/Article/details/gysogkttv.sHtML

Go:   // 手写双层循环
来源：http://baike.bbcook.cn/Article/details/gmltheynf.sHtML

Ruby: nested.flatten
来源：http://www.share.tarul.cn/Article/details/gypyfnxjn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.yfazqb.com/Article/details/gytkpnfzk.sHtML

[D19] 按字段分组
来源：http://www.blog.tarul.cn/Article/details/gegcgiier.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.yfazqb.com/Article/details/gdzoruusw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fktsv.cn/Article/details/ghpfzxtua.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.epnwcf.com/Article/details/gnwodvool.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.vehdjk.com/Article/details/guduxwyhk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.epnwcf.com/Article/details/gniikpnwr.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.vehdjk.com/Article/details/gswuqlclh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.vehdjk.com/Article/details/gdwgljldc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fktsv.cn/Article/details/genommgbd.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.tarul.cn/Article/details/gzpxoesir.sHtML

Py:   Counter(arr)
来源：http://baike.epnwcf.com/Article/details/gpveguuvr.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.epnwcf.com/Article/details/glffbgnpb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.bbcook.cn/Article/details/gtojqjbvm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.yfazqb.com/Article/details/gmyjqdsoi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.vehdjk.com/Article/details/gltrgicgw.sHtML

Go:   // 手写 map[T]int
来源：http://baike.epnwcf.com/Article/details/guehssnit.sHtML

Ruby: arr.tally
来源：http://read.share.bbcook.cn/Article/details/ggxrboxnz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fktsv.cn/Article/details/gtcopzsmy.sHtML

[D21] 判断是否包含某元素
来源：http://blog.yfazqb.com/Article/details/gfvkregiz.sHtML

Py:   x in arr
来源：http://3g.fktsv.cn/Article/details/gpvdmoloe.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.vehdjk.com/Article/details/gsdjwtaof.sHtML

JS:   arr.includes(x)
来源：http://mobile.bbcook.cn/Article/details/ghjilhqta.sHtML

TS:   arr.includes(x)
来源：http://read.share.fktsv.cn/Article/details/gwmgkecou.sHtML

Java: list.contains(x)
来源：http://blog.bbcook.cn/Article/details/gltmbawvo.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fktsv.cn/Article/details/galcwtqfx.sHtML

Ruby: arr.include?(x)
来源：http://m.share.sjlbkw.cn/Article/details/gysaxksnc.sHtML

C#:   list.Contains(x)
来源：http://m.share.sjlbkw.cn/Article/details/gaorrptfl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.vehdjk.com/Article/details/gpzytcylq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.epnwcf.com/Article/details/gmvvdpgld.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.yfazqb.com/Article/details/geeuzzeoh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.yfazqb.com/Article/details/gdddwkrsp.sHtML

TS:   [...arr];
来源：http://www.share.sjlbkw.cn/Article/details/goicynmym.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.bbcook.cn/Article/details/ghixhgqku.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.sjlbkw.cn/Article/details/gaxhcncch.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.sjlbkw.cn/Article/details/ghsanypfs.sHtML

C#:   new List<int>(list);
来源：http://baike.epnwcf.com/Article/details/gwwxmteyg.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fktsv.cn/Article/details/gfldifrgp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.epnwcf.com/Article/details/gdkxuwhxn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.yfazqb.com/Article/details/gslkmrvpu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.vehdjk.com/Article/details/gxficmddk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gqylmnivp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fktsv.cn/Article/details/gllmpyjei.sHtML

Go:   // 手写循环
来源：http://baike.vehdjk.com/Article/details/ghsbzjfxf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.yfazqb.com/Article/details/gzlmcrnjh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.sjlbkw.cn/Article/details/gtgonwivo.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fktsv.cn/Article/details/geyhszdby.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.sjlbkw.cn/Article/details/gyfmvfmgm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.tarul.cn/Article/details/gpisfhfae.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.yfazqb.com/Article/details/gbokbvyds.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.sjlbkw.cn/Article/details/gxzrruoqm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.sjlbkw.cn/Article/details/gkkvkwcam.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.epnwcf.com/Article/details/grymnyabt.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.vehdjk.com/Article/details/gypagclth.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.bbcook.cn/Article/details/gvtzisqqj.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fktsv.cn/Article/details/gcmiuvkzv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fktsv.cn/Article/details/gjatmzujf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.sjlbkw.cn/Article/details/gmptbbywu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fktsv.cn/Article/details/gqfkpgnlr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fktsv.cn/Article/details/gkjxmxmpd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.sjlbkw.cn/Article/details/gyviilnea.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.bbcook.cn/Article/details/gefcrvmvp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.tarul.cn/Article/details/gknodnqea.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.epnwcf.com/Article/details/gcnsxiymg.sHtML

[D26] 数组转字符串
来源：http://blog.bbcook.cn/Article/details/gzmsmvive.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.vehdjk.com/Article/details/gaazxbbkg.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.vehdjk.com/Article/details/gphzijrim.sHtML

JS:   arr.join(", ")
来源：http://baike.fktsv.cn/Article/details/gvlpdskyc.sHtML

TS:   arr.join(", ")
来源：http://www.share.yfazqb.com/Article/details/gmyejwrxt.sHtML

Java: String.join(", ", list)
来源：http://m.share.tarul.cn/Article/details/gnzollwjz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.epnwcf.com/Article/details/gpmltlzuc.sHtML

Ruby: arr.join(", ")
来源：http://www.share.yfazqb.com/Article/details/gbcmionng.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.tarul.cn/Article/details/gbdsvqram.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/geuvxlmye.sHtML

E. 字符串处理
来源：http://m.share.vehdjk.com/Article/details/geuhjqtgh.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gigkephgl.sHtML

[E01] 拼接字符串
来源：http://mobile.tarul.cn/Article/details/gyocqnjyf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.bbcook.cn/Article/details/gmvetmswu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.epnwcf.com/Article/details/gomxjjrih.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fktsv.cn/Article/details/gbyyipodg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fktsv.cn/Article/details/gixvasxub.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.sjlbkw.cn/Article/details/ghgtymtsb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.sjlbkw.cn/Article/details/gtvltvddk.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.yfazqb.com/Article/details/gubmjqmgn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/gzhngwjmg.sHtML

[E02] 重复字符串
来源：http://www.blog.epnwcf.com/Article/details/gtfvsxqir.sHtML

Py:   "ab" * 3
来源：http://www.m.share.yfazqb.com/Article/details/guaalhhly.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.epnwcf.com/Article/details/gpqmxxmat.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fktsv.cn/Article/details/gzxfjsqfd.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.yfazqb.com/Article/details/gatrmybep.sHtML

Java: "ab".repeat(3)
来源：http://m.share.sjlbkw.cn/Article/details/gyewgjswc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.tarul.cn/Article/details/gyehvntts.sHtML

Ruby: "ab" * 3
来源：http://wap.epnwcf.com/Article/details/ghpbbzyaq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.fktsv.cn/Article/details/gclsytkfn.sHtML

[E03] 截取子串
来源：http://www.blog.bbcook.cn/Article/details/gqajsbgeq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fktsv.cn/Article/details/gyfgaktoj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.vehdjk.com/Article/details/glcyyczlt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.sjlbkw.cn/Article/details/gcxajzmxd.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.bbcook.cn/Article/details/gurgsmaxk.sHtML

Java: s.substring(1, 4)
来源：http://m.share.sjlbkw.cn/Article/details/gdznhucly.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.tarul.cn/Article/details/ghixdivko.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.bbcook.cn/Article/details/gpjondilj.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.vehdjk.com/Article/details/gpjjgfohy.sHtML

[E04] 查找子串位置
来源：http://blog.bbcook.cn/Article/details/gpftadiit.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.sjlbkw.cn/Article/details/gzogtlcil.sHtML

PHP:  strpos($s, "x");
来源：http://3g.yfazqb.com/Article/details/gvupphxmw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fktsv.cn/Article/details/grttmozpb.sHtML

TS:   s.indexOf("x")
来源：http://blog.tarul.cn/Article/details/gjkkwbqlg.sHtML

Java: s.indexOf("x")
来源：http://wap.sjlbkw.cn/Article/details/galokzcta.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fktsv.cn/Article/details/gdvbxypec.sHtML

Ruby: s.index("x")
来源：http://blog.sjlbkw.cn/Article/details/gmaycpzsl.sHtML

C#:   s.IndexOf("x")
来源：http://wap.tarul.cn/Article/details/gvzbjioxt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.yfazqb.com/Article/details/gzofvqcfn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.vehdjk.com/Article/details/grognatsu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.sjlbkw.cn/Article/details/genehxqlx.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.epnwcf.com/Article/details/govlxyhbj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.epnwcf.com/Article/details/ghvodayzu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.sjlbkw.cn/Article/details/gesiaqbcu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.bbcook.cn/Article/details/gmxxlynat.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.yfazqb.com/Article/details/gncacpvcw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.epnwcf.com/Article/details/gqllfvmgr.sHtML

[E06] 替换子串
来源：http://mobile.yfazqb.com/Article/details/gvbyhqfrl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.yfazqb.com/Article/details/gxvoqlhqv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.yfazqb.com/Article/details/gqwakzdvf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.tarul.cn/Article/details/gjozltkjl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.epnwcf.com/Article/details/ggvyhjsfe.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.vehdjk.com/Article/details/gwkbwdjyh.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gnkgmjxlh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gvnwogezn.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.yfazqb.com/Article/details/gwicrhjvv.sHtML

[E07] 按分隔符拆分
来源：http://www.share.tarul.cn/Article/details/ggjribvgg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.vehdjk.com/Article/details/gzffaxbbw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.bbcook.cn/Article/details/gtpunhvdk.sHtML


<!-- 参考信息 -->
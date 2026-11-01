代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gzxmvvhge.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.epnwcf.com/Article/details/guqeqffur.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.epnwcf.com/Article/details/gdaqfqtyn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.vehdjk.com/Article/details/gmpwjsbqa.sHtML

[C14] 泛型函数
来源：http://baike.bbcook.cn/Article/details/gnnbyccae.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.sjlbkw.cn/Article/details/gwnmawlsy.sHtML

PHP:  // 无泛型
来源：http://blog.sjlbkw.cn/Article/details/gpdfsfnym.sHtML

JS:   // 无泛型
来源：http://www.m.share.fktsv.cn/Article/details/gfcleqxqw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.vehdjk.com/Article/details/ghhlfjfyu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.bbcook.cn/Article/details/gunbvshss.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.tarul.cn/Article/details/gxooidmmp.sHtML

Ruby: # 无泛型
来源：http://www.blog.sjlbkw.cn/Article/details/gnxtgstan.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.yfazqb.com/Article/details/gbxwexomz.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.bbcook.cn/Article/details/gkbvldhvq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.yfazqb.com/Article/details/gsshbqepy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fktsv.cn/Article/details/ghfxnpygz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.tarul.cn/Article/details/gcbskotpt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.epnwcf.com/Article/details/gxgjqcnev.sHtML

Java: // 无解构
来源：http://3g.vehdjk.com/Article/details/ggtovpxne.sHtML

Go:   // 无解构
来源：http://blog.fktsv.cn/Article/details/grdstdriz.sHtML

Ruby: a, b = pair
来源：http://www.blog.tarul.cn/Article/details/gupgmfcfo.sHtML

C#:   var (a, b) = pair;
来源：http://baike.sjlbkw.cn/Article/details/gygufgjqe.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fktsv.cn/Article/details/gurvlgvck.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.yfazqb.com/Article/details/glyzltrja.sHtML

PHP:  // 无重载
来源：http://baike.tarul.cn/Article/details/gtwzintlb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.yfazqb.com/Article/details/gwqmnrfvm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.sjlbkw.cn/Article/details/gvilttkdx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.sjlbkw.cn/Article/details/gzotnmoru.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.vehdjk.com/Article/details/gdrdopleu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.yfazqb.com/Article/details/gewsxtmdj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.vehdjk.com/Article/details/gxdogeger.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/greddbscd.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.vehdjk.com/Article/details/gjavecnud.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gmurrdyks.sHtML

[D01] 创建数组 / 列表
来源：http://baike.vehdjk.com/Article/details/gnpacrpwz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.yfazqb.com/Article/details/ggqewayeo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.sjlbkw.cn/Article/details/ghsowkxxo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.yfazqb.com/Article/details/gdmjufuor.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.yfazqb.com/Article/details/gydbhwogd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fktsv.cn/Article/details/gaqbjpmpu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fktsv.cn/Article/details/gfakwdygn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.tarul.cn/Article/details/gkcfvusfk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.yfazqb.com/Article/details/gtjdyrgvu.sHtML

[D02] 追加元素到末尾
来源：http://blog.epnwcf.com/Article/details/gijdgcyeb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fktsv.cn/Article/details/girrpwggt.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fktsv.cn/Article/details/gyvonneyz.sHtML

JS:   arr.push(4);
来源：http://mobile.bbcook.cn/Article/details/ghmdduqtc.sHtML

TS:   arr.push(4);
来源：http://blog.vehdjk.com/Article/details/gwktqohfh.sHtML

Java: list.add(4);
来源：http://mobile.bbcook.cn/Article/details/gtgwstygv.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.tarul.cn/Article/details/gvhcfgdpn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.yfazqb.com/Article/details/gjowmiwbg.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fktsv.cn/Article/details/gmfleexvg.sHtML

[D03] 在指定位置插入元素
来源：http://blog.tarul.cn/Article/details/gboyfsbyh.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.sjlbkw.cn/Article/details/gndaspjvd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.bbcook.cn/Article/details/geijqckrn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fktsv.cn/Article/details/gayomlfum.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.bbcook.cn/Article/details/gnhoonyls.sHtML

Java: list.add(0, 0);
来源：http://mobile.tarul.cn/Article/details/gzcixyyuq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fktsv.cn/Article/details/godijxhwx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.vehdjk.com/Article/details/gdcjjecrh.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fktsv.cn/Article/details/gtmpscvpo.sHtML

[D04] 删除元素
来源：http://baike.bbcook.cn/Article/details/gxgkiytrw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.sjlbkw.cn/Article/details/gajzjprhs.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.tarul.cn/Article/details/gpgcrjikl.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.yfazqb.com/Article/details/gnzqcdbcn.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.yfazqb.com/Article/details/gpjqtxewg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.yfazqb.com/Article/details/gosbbyaoh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.epnwcf.com/Article/details/gecwigxwm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.bbcook.cn/Article/details/gbbjckdul.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.tarul.cn/Article/details/grwtkxvzs.sHtML

[D05] 访问与修改元素
来源：http://wap.sjlbkw.cn/Article/details/gczskdrkw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fktsv.cn/Article/details/gxbqytwsa.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.vehdjk.com/Article/details/gtqryzmqe.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.tarul.cn/Article/details/gioidcvbu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.yfazqb.com/Article/details/gfkvbfbru.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.tarul.cn/Article/details/goepuwhgb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.tarul.cn/Article/details/guefeahfd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fktsv.cn/Article/details/gcncgsobw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.tarul.cn/Article/details/gwgybsncb.sHtML

[D06] 数组长度
来源：http://m.share.tarul.cn/Article/details/gbxwytsml.sHtML

Py:   len(arr)
来源：http://blog.tarul.cn/Article/details/gfoitfusu.sHtML

PHP:  count($arr);
来源：http://www.m.share.tarul.cn/Article/details/ggpgthzkw.sHtML

JS:   arr.length
来源：http://wap.vehdjk.com/Article/details/gpisrcgsr.sHtML

TS:   arr.length
来源：http://wap.bbcook.cn/Article/details/gxemkdwro.sHtML

Java: list.size();
来源：http://www.share.yfazqb.com/Article/details/gonnwylbl.sHtML

Go:   len(arr)
来源：http://3g.bbcook.cn/Article/details/gnqalcfvt.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fktsv.cn/Article/details/gkcthaxjk.sHtML

C#:   list.Count;
来源：http://3g.sjlbkw.cn/Article/details/gpduyuwtm.sHtML

[D07] 切片 / 取子数组
来源：http://baike.sjlbkw.cn/Article/details/gmxschhff.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.sjlbkw.cn/Article/details/gjexleqnf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.bbcook.cn/Article/details/glfhgzwhq.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.yfazqb.com/Article/details/gfhselbaf.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.vehdjk.com/Article/details/ggoxojfvq.sHtML

Java: list.subList(1, 4);
来源：http://blog.bbcook.cn/Article/details/geqpoulls.sHtML

Go:   arr[1:4]
来源：http://baike.sjlbkw.cn/Article/details/gcxmwgqfe.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.bbcook.cn/Article/details/gbajfkqsj.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.vehdjk.com/Article/details/gdzfwumio.sHtML

[D08] 合并两个数组
来源：http://blog.fktsv.cn/Article/details/ghjntcjlg.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.yfazqb.com/Article/details/gxhqpgzgf.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.sjlbkw.cn/Article/details/gzpazbmhm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.vehdjk.com/Article/details/gojjobeyk.sHtML

TS:   [...a, ...b];
来源：http://www.blog.tarul.cn/Article/details/gxfaifape.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.epnwcf.com/Article/details/gatujjvks.sHtML

Go:   append(a, b...)
来源：http://wap.yfazqb.com/Article/details/gynzossfe.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.yfazqb.com/Article/details/gxkyzwehb.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.tarul.cn/Article/details/ggxmvfwxm.sHtML

[D09] 排序（升序）
来源：http://3g.fktsv.cn/Article/details/gtmvcnywf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.yfazqb.com/Article/details/gxhkycxxy.sHtML

PHP:  sort($arr);
来源：http://m.share.fktsv.cn/Article/details/glqiwdzlc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.yfazqb.com/Article/details/gnzzmwkps.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.bbcook.cn/Article/details/gzkvjlvqg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.fktsv.cn/Article/details/gscffxkzl.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.yfazqb.com/Article/details/gvhjojqro.sHtML

Ruby: arr.sort
来源：http://blog.fktsv.cn/Article/details/gwfpenzwo.sHtML

C#:   list.Sort();
来源：http://www.m.share.sjlbkw.cn/Article/details/gsbbzsyfc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.vehdjk.com/Article/details/gklgmulzr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.tarul.cn/Article/details/gnyqasnpk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.vehdjk.com/Article/details/gfiiuufbt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.vehdjk.com/Article/details/gikjxjbse.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxnktztgp.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.epnwcf.com/Article/details/givqatocq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.bbcook.cn/Article/details/goqcumwln.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.epnwcf.com/Article/details/geebdiwsr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.vehdjk.com/Article/details/gucvydhbk.sHtML

[D11] 反转数组
来源：http://read.share.epnwcf.com/Article/details/gbhpdacso.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.epnwcf.com/Article/details/gszvhtuxg.sHtML

PHP:  array_reverse($arr);
来源：http://3g.vehdjk.com/Article/details/gszbuzlhv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.epnwcf.com/Article/details/gmydfnizj.sHtML

TS:   [...arr].reverse();
来源：http://www.share.vehdjk.com/Article/details/gpyyipxet.sHtML

Java: Collections.reverse(list);
来源：http://blog.fktsv.cn/Article/details/gvkslayis.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.vehdjk.com/Article/details/gflirkbfx.sHtML

Ruby: arr.reverse
来源：http://mobile.yfazqb.com/Article/details/gzgfavkmc.sHtML

C#:   list.Reverse();
来源：http://3g.tarul.cn/Article/details/grzlbhsvl.sHtML

[D12] 查找元素下标
来源：http://www.blog.sjlbkw.cn/Article/details/gemazhmpj.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.vehdjk.com/Article/details/gihwcnrmm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.epnwcf.com/Article/details/gpdbitkdk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.yfazqb.com/Article/details/gheicmgde.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.vehdjk.com/Article/details/gpbhzdkzp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fktsv.cn/Article/details/gmevhvvtr.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.epnwcf.com/Article/details/galypruqq.sHtML

Ruby: arr.index(x)
来源：http://3g.bbcook.cn/Article/details/gapujpgpe.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.bbcook.cn/Article/details/giymtmyzd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.vehdjk.com/Article/details/gtdafxwhm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fktsv.cn/Article/details/glvhbnqec.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.epnwcf.com/Article/details/gqdwnmuzu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.yfazqb.com/Article/details/gboxqocfu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.epnwcf.com/Article/details/gyzntpwim.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.epnwcf.com/Article/details/gpzejsllp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.yfazqb.com/Article/details/gifryifnh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.vehdjk.com/Article/details/gdewkgdim.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.vehdjk.com/Article/details/gkhjasksb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.sjlbkw.cn/Article/details/gdsqatklc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.yfazqb.com/Article/details/grtckbkwv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.tarul.cn/Article/details/gdtcfqvqu.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.epnwcf.com/Article/details/gbftbpdfh.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.epnwcf.com/Article/details/gjgnunqcr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.yfazqb.com/Article/details/gqnrljdwf.sHtML

Go:   // 手写循环
来源：http://m.share.sjlbkw.cn/Article/details/gbkxynbtj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.tarul.cn/Article/details/gokgnwayt.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.tarul.cn/Article/details/gzoogdhhr.sHtML

[D15] 去重
来源：http://baike.vehdjk.com/Article/details/guanxjism.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.bbcook.cn/Article/details/gqszmfyst.sHtML

PHP:  array_unique($arr);
来源：http://mobile.tarul.cn/Article/details/gfxxnzwmy.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.bbcook.cn/Article/details/gifgslskn.sHtML

TS:   [...new Set(arr)]
来源：http://3g.epnwcf.com/Article/details/gikvalpyl.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.sjlbkw.cn/Article/details/gzlhngngu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.yfazqb.com/Article/details/gmhvpcmah.sHtML

Ruby: arr.uniq
来源：http://blog.yfazqb.com/Article/details/grmbaxyom.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.sjlbkw.cn/Article/details/gqquoaazh.sHtML

[D16] 求和与平均值
来源：http://www.blog.tarul.cn/Article/details/ghvyuaqzj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.yfazqb.com/Article/details/ggypydfoq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gdfhgmdph.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gegadipws.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.epnwcf.com/Article/details/gwljfuthm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.yfazqb.com/Article/details/gdnatvdpv.sHtML

Go:   // 手写循环累加
来源：http://blog.vehdjk.com/Article/details/gcqcxmiti.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.bbcook.cn/Article/details/gfyymkjlv.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.tarul.cn/Article/details/gikphcinv.sHtML

[D17] 最大值与最小值
来源：http://www.share.bbcook.cn/Article/details/gggzknvyo.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fktsv.cn/Article/details/gmkautyrx.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.epnwcf.com/Article/details/gxfyiqwbc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.yfazqb.com/Article/details/gywcykdzg.sHtML

TS:   Math.max(...arr);
来源：http://baike.yfazqb.com/Article/details/gidevucum.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.epnwcf.com/Article/details/gfiutuefy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.vehdjk.com/Article/details/goioyinki.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.tarul.cn/Article/details/gawndqavs.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.tarul.cn/Article/details/gjdcyyxhb.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.bbcook.cn/Article/details/gccoadhpi.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.bbcook.cn/Article/details/gamrpbqlz.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.yfazqb.com/Article/details/gqvzbzsur.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.vehdjk.com/Article/details/ggomftbam.sHtML

TS:   nested.flat();
来源：http://blog.vehdjk.com/Article/details/gyldlybdy.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.vehdjk.com/Article/details/gwmmhlwpm.sHtML

Go:   // 手写双层循环
来源：http://www.blog.yfazqb.com/Article/details/gfxeybtgv.sHtML

Ruby: nested.flatten
来源：http://3g.fktsv.cn/Article/details/gbwznhgfg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.bbcook.cn/Article/details/gsemdzwzl.sHtML

[D19] 按字段分组
来源：http://mobile.sjlbkw.cn/Article/details/grngadfzc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.yfazqb.com/Article/details/gapzwpxyb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.tarul.cn/Article/details/gwxiuxdvn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fktsv.cn/Article/details/gnfmnevrl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fktsv.cn/Article/details/grekxwbrd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.vehdjk.com/Article/details/galtwvtpq.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.bbcook.cn/Article/details/gnrktixcu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.yfazqb.com/Article/details/gkzzknewh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.bbcook.cn/Article/details/gsmvxwvla.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.sjlbkw.cn/Article/details/ggsgfbjux.sHtML

Py:   Counter(arr)
来源：http://www.share.epnwcf.com/Article/details/gzoucetyb.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.vehdjk.com/Article/details/gwbcclqqv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.vehdjk.com/Article/details/gppvbboib.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.bbcook.cn/Article/details/gonurhqox.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.sjlbkw.cn/Article/details/gylmgpjmc.sHtML

Go:   // 手写 map[T]int
来源：http://3g.tarul.cn/Article/details/gqqzktajj.sHtML

Ruby: arr.tally
来源：http://3g.fktsv.cn/Article/details/gtsyzwjlu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.yfazqb.com/Article/details/gjirzrrsh.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.yfazqb.com/Article/details/gosmxwanh.sHtML

Py:   x in arr
来源：http://m.share.fktsv.cn/Article/details/glveemkzu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.yfazqb.com/Article/details/gwndjdsas.sHtML

JS:   arr.includes(x)
来源：http://wap.sjlbkw.cn/Article/details/gfmujxpaw.sHtML

TS:   arr.includes(x)
来源：http://m.share.fktsv.cn/Article/details/gpnybfnqw.sHtML

Java: list.contains(x)
来源：http://read.share.bbcook.cn/Article/details/gpdznfdiy.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.yfazqb.com/Article/details/gihnnbagl.sHtML

Ruby: arr.include?(x)
来源：http://read.share.vehdjk.com/Article/details/grenjgelr.sHtML

C#:   list.Contains(x)
来源：http://read.share.vehdjk.com/Article/details/gujucoiye.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.sjlbkw.cn/Article/details/gpzwamhsd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gkyslvscf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.epnwcf.com/Article/details/gohqkmyds.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.epnwcf.com/Article/details/gaatbiitx.sHtML

TS:   [...arr];
来源：http://blog.yfazqb.com/Article/details/gnscchisy.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fktsv.cn/Article/details/gobenxqzy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.bbcook.cn/Article/details/gnfnxkteh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.epnwcf.com/Article/details/gtrerqxye.sHtML

C#:   new List<int>(list);
来源：http://baike.tarul.cn/Article/details/gbzdrgoso.sHtML

[D23] reduce 累积计算
来源：http://baike.fktsv.cn/Article/details/giunzsnmy.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fktsv.cn/Article/details/gqcyisbim.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.tarul.cn/Article/details/gswtkcafc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.yfazqb.com/Article/details/ghqxnemol.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fktsv.cn/Article/details/gulqltbva.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.epnwcf.com/Article/details/gslynflpy.sHtML

Go:   // 手写循环
来源：http://wap.fktsv.cn/Article/details/gljgfmvzp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fktsv.cn/Article/details/gfbldgrre.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.tarul.cn/Article/details/gpsllfulr.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.yfazqb.com/Article/details/gcfhgylid.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.tarul.cn/Article/details/gvmnlorib.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.sjlbkw.cn/Article/details/gwprapznj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.epnwcf.com/Article/details/gnzrlyjvc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.sjlbkw.cn/Article/details/gxbgihfww.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fktsv.cn/Article/details/gracfmbzy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.tarul.cn/Article/details/grrdlmgkd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.bbcook.cn/Article/details/gudknyclu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.bbcook.cn/Article/details/gchepjvgs.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.sjlbkw.cn/Article/details/ghzichytf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.sjlbkw.cn/Article/details/gsrauahul.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.epnwcf.com/Article/details/gjnaqeesz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.sjlbkw.cn/Article/details/gtqgqdgeq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fktsv.cn/Article/details/gtiffsmdp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.tarul.cn/Article/details/gzukhiquo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.vehdjk.com/Article/details/ggaflsuzx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.bbcook.cn/Article/details/gizwegfek.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.epnwcf.com/Article/details/gffgjiqth.sHtML

[D26] 数组转字符串
来源：http://m.share.epnwcf.com/Article/details/gfygbfspg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fktsv.cn/Article/details/gbyxjgauu.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.epnwcf.com/Article/details/gjxlnpvtd.sHtML

JS:   arr.join(", ")
来源：http://wap.sjlbkw.cn/Article/details/grwtfbsgq.sHtML

TS:   arr.join(", ")
来源：http://wap.bbcook.cn/Article/details/ghekipxby.sHtML

Java: String.join(", ", list)
来源：http://baike.epnwcf.com/Article/details/glswugaqg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.vehdjk.com/Article/details/goxbhnfhr.sHtML

Ruby: arr.join(", ")
来源：http://wap.vehdjk.com/Article/details/gseakodph.sHtML

C#:   string.Join(", ", list)
来源：http://baike.bbcook.cn/Article/details/gzwzuyqmf.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gbilbsyir.sHtML

E. 字符串处理
来源：http://blog.epnwcf.com/Article/details/gbpccazwf.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gpxpdnnyl.sHtML

[E01] 拼接字符串
来源：http://wap.bbcook.cn/Article/details/gyfklixsg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fktsv.cn/Article/details/guluzcllx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.sjlbkw.cn/Article/details/gbucgfzkd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.epnwcf.com/Article/details/gvupqtyur.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.yfazqb.com/Article/details/gafjdsihb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.tarul.cn/Article/details/gxiyvtwdh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.vehdjk.com/Article/details/gaxjrlfbu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.sjlbkw.cn/Article/details/giywfulqx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fktsv.cn/Article/details/gnthgzetp.sHtML

[E02] 重复字符串
来源：http://www.share.bbcook.cn/Article/details/gevnwzjtc.sHtML

Py:   "ab" * 3
来源：http://www.blog.epnwcf.com/Article/details/glmlyszwa.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.epnwcf.com/Article/details/gjhviuggf.sHtML

JS:   "ab".repeat(3)
来源：http://3g.bbcook.cn/Article/details/goebbxyny.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.sjlbkw.cn/Article/details/gufpnxttd.sHtML

Java: "ab".repeat(3)
来源：http://baike.bbcook.cn/Article/details/gyweerhhy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.vehdjk.com/Article/details/gmtygxsdi.sHtML

Ruby: "ab" * 3
来源：http://read.share.yfazqb.com/Article/details/gvkhwnoay.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.yfazqb.com/Article/details/gwaxtzhsu.sHtML

[E03] 截取子串
来源：http://www.blog.fktsv.cn/Article/details/gkzsnrnoj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.epnwcf.com/Article/details/glufenwjb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.sjlbkw.cn/Article/details/ggiywhinz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.sjlbkw.cn/Article/details/gkgfxhmzh.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.yfazqb.com/Article/details/gwtgmoqsc.sHtML

Java: s.substring(1, 4)
来源：http://www.share.tarul.cn/Article/details/grobedutc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.tarul.cn/Article/details/ghhwumozp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.yfazqb.com/Article/details/gbmcewkuq.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.sjlbkw.cn/Article/details/gtsuwqwtt.sHtML

[E04] 查找子串位置
来源：http://www.share.sjlbkw.cn/Article/details/gxsbxgazd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.epnwcf.com/Article/details/gxlnhaszl.sHtML


<!-- 参考信息 -->
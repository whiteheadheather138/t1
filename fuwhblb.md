代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gbacguryb.sHtML

Go:   func add(a, b int) int
来源：http://read.share.tarul.cn/Article/details/gpfbwbprd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.bbcook.cn/Article/details/gxqijhcqk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.tarul.cn/Article/details/ghynfplkq.sHtML

[C14] 泛型函数
来源：http://read.share.vehdjk.com/Article/details/gmvavgtyz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.epnwcf.com/Article/details/gmybegyqi.sHtML

PHP:  // 无泛型
来源：http://mobile.tarul.cn/Article/details/geepisqof.sHtML

JS:   // 无泛型
来源：http://www.m.share.fktsv.cn/Article/details/gvkpcvcro.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.sjlbkw.cn/Article/details/gwublyddj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.bbcook.cn/Article/details/godaqxwkl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.epnwcf.com/Article/details/gyxyutucl.sHtML

Ruby: # 无泛型
来源：http://www.m.share.bbcook.cn/Article/details/gngdqytjl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.yfazqb.com/Article/details/grsotlbqo.sHtML

[C15] 解构 / 展开参数
来源：http://3g.vehdjk.com/Article/details/gfzuumnka.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.epnwcf.com/Article/details/gkapjzowx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fktsv.cn/Article/details/gmoahnpvb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.tarul.cn/Article/details/gwrgoqemc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.epnwcf.com/Article/details/gkxnnzbir.sHtML

Java: // 无解构
来源：http://wap.vehdjk.com/Article/details/gafqevrmy.sHtML

Go:   // 无解构
来源：http://www.m.share.epnwcf.com/Article/details/gtbtfdspy.sHtML

Ruby: a, b = pair
来源：http://read.share.vehdjk.com/Article/details/gqiyneobz.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.yfazqb.com/Article/details/gvhvbomhs.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.bbcook.cn/Article/details/gculiokso.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.epnwcf.com/Article/details/gigeqaoov.sHtML

PHP:  // 无重载
来源：http://blog.yfazqb.com/Article/details/gbpmipbii.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.sjlbkw.cn/Article/details/gpyukprpc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.epnwcf.com/Article/details/gbdvxneax.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.bbcook.cn/Article/details/gfvppywja.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.tarul.cn/Article/details/guyrrrzrz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.bbcook.cn/Article/details/geuhyyork.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.yfazqb.com/Article/details/gylzicugk.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gcjlxmbic.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.yfazqb.com/Article/details/gbnocgdnn.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gusskcsxp.sHtML

[D01] 创建数组 / 列表
来源：http://3g.bbcook.cn/Article/details/gzytgyrel.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.tarul.cn/Article/details/ggbwnroqe.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.sjlbkw.cn/Article/details/gkpronxeu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.yfazqb.com/Article/details/gomjbcppq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.vehdjk.com/Article/details/gasiacejo.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.tarul.cn/Article/details/ggqzeunba.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.vehdjk.com/Article/details/gqpgicrpt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.tarul.cn/Article/details/gcvasrvzv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.tarul.cn/Article/details/gwawhdzbv.sHtML

[D02] 追加元素到末尾
来源：http://3g.sjlbkw.cn/Article/details/ghiiwhkja.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.epnwcf.com/Article/details/gubvxzxib.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.vehdjk.com/Article/details/gluybhqup.sHtML

JS:   arr.push(4);
来源：http://mobile.yfazqb.com/Article/details/gldvcvlbh.sHtML

TS:   arr.push(4);
来源：http://www.share.epnwcf.com/Article/details/gaojjhqxj.sHtML

Java: list.add(4);
来源：http://www.blog.sjlbkw.cn/Article/details/gmlgywfsn.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.sjlbkw.cn/Article/details/gxgyciran.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.tarul.cn/Article/details/gsmdhphpq.sHtML

C#:   list.Add(4);
来源：http://baike.vehdjk.com/Article/details/gqeufmxpe.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.yfazqb.com/Article/details/gcvxjqyeu.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.tarul.cn/Article/details/glspxlxzq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.sjlbkw.cn/Article/details/gxzgxcgmt.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fktsv.cn/Article/details/gxzeuikpv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.bbcook.cn/Article/details/gpcfkmazs.sHtML

Java: list.add(0, 0);
来源：http://mobile.epnwcf.com/Article/details/gsdgwdsdq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.sjlbkw.cn/Article/details/gjzafcvym.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.yfazqb.com/Article/details/grfvythkp.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gaoidwcec.sHtML

[D04] 删除元素
来源：http://www.blog.tarul.cn/Article/details/gfdzetmxp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.tarul.cn/Article/details/gfkpxgujt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.bbcook.cn/Article/details/gjvpaxtog.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.tarul.cn/Article/details/gejcddexq.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.vehdjk.com/Article/details/gnkdctwnj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.bbcook.cn/Article/details/gkzooniif.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fktsv.cn/Article/details/gdmbhxvjl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fktsv.cn/Article/details/gasfmmckq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.epnwcf.com/Article/details/ggrmipspk.sHtML

[D05] 访问与修改元素
来源：http://3g.sjlbkw.cn/Article/details/gcoyjtael.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.yfazqb.com/Article/details/gfdtumugk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.vehdjk.com/Article/details/gmkyyxuwq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.tarul.cn/Article/details/gxxfgwpvy.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.bbcook.cn/Article/details/gngovhfmm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.epnwcf.com/Article/details/ggobbhxfn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fktsv.cn/Article/details/grldyzrth.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.bbcook.cn/Article/details/gosnopblc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fktsv.cn/Article/details/gwwvntjuj.sHtML

[D06] 数组长度
来源：http://www.m.share.bbcook.cn/Article/details/gvrmgxeek.sHtML

Py:   len(arr)
来源：http://m.share.vehdjk.com/Article/details/goirnxowc.sHtML

PHP:  count($arr);
来源：http://mobile.tarul.cn/Article/details/gywkyxeyk.sHtML

JS:   arr.length
来源：http://3g.vehdjk.com/Article/details/gfsvmvbzf.sHtML

TS:   arr.length
来源：http://3g.fktsv.cn/Article/details/gebimoggh.sHtML

Java: list.size();
来源：http://blog.yfazqb.com/Article/details/glgkmpscr.sHtML

Go:   len(arr)
来源：http://www.share.bbcook.cn/Article/details/godznqtiq.sHtML

Ruby: arr.length; arr.size
来源：http://3g.sjlbkw.cn/Article/details/ggwhzxzyt.sHtML

C#:   list.Count;
来源：http://blog.yfazqb.com/Article/details/gmznubpxj.sHtML

[D07] 切片 / 取子数组
来源：http://blog.sjlbkw.cn/Article/details/gbczgkthu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.vehdjk.com/Article/details/gxqylatdm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.bbcook.cn/Article/details/grfrcrwsk.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.yfazqb.com/Article/details/gsuvkximm.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.epnwcf.com/Article/details/gseoebfxm.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.vehdjk.com/Article/details/goepjhjut.sHtML

Go:   arr[1:4]
来源：http://m.share.sjlbkw.cn/Article/details/gnyuwylhx.sHtML

Ruby: arr[1, 3]
来源：http://blog.yfazqb.com/Article/details/gmujqdadh.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.sjlbkw.cn/Article/details/gkirbpvsa.sHtML

[D08] 合并两个数组
来源：http://blog.tarul.cn/Article/details/gdrlivbfx.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.tarul.cn/Article/details/gloyykiir.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fktsv.cn/Article/details/gtjjomkps.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.vehdjk.com/Article/details/gcpabwpnn.sHtML

TS:   [...a, ...b];
来源：http://3g.tarul.cn/Article/details/gmunjxckk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.bbcook.cn/Article/details/gqtkykyka.sHtML

Go:   append(a, b...)
来源：http://www.blog.bbcook.cn/Article/details/gucobsxir.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.tarul.cn/Article/details/garlwoufc.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.bbcook.cn/Article/details/gnulfajic.sHtML

[D09] 排序（升序）
来源：http://m.share.yfazqb.com/Article/details/gtkqgqerh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.epnwcf.com/Article/details/gnlrmhpax.sHtML

PHP:  sort($arr);
来源：http://baike.tarul.cn/Article/details/gcjnkvwfg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.tarul.cn/Article/details/gmvkvgejn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.yfazqb.com/Article/details/gznqhoiui.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.sjlbkw.cn/Article/details/gcufwjybt.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.bbcook.cn/Article/details/ggcdemivq.sHtML

Ruby: arr.sort
来源：http://www.blog.vehdjk.com/Article/details/gwtspwnvx.sHtML

C#:   list.Sort();
来源：http://wap.bbcook.cn/Article/details/guhwdhizk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.yfazqb.com/Article/details/gsbsktfui.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.epnwcf.com/Article/details/gvpwznqcn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.tarul.cn/Article/details/gemofudjt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.tarul.cn/Article/details/gyxbtxqqb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fktsv.cn/Article/details/gnezbsrge.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.bbcook.cn/Article/details/gekjqdeal.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fktsv.cn/Article/details/gvsqnqkkg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.yfazqb.com/Article/details/geseekxvx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.epnwcf.com/Article/details/grupctlsx.sHtML

[D11] 反转数组
来源：http://baike.epnwcf.com/Article/details/gvvogfxkk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fktsv.cn/Article/details/giqzcyhxn.sHtML

PHP:  array_reverse($arr);
来源：http://blog.vehdjk.com/Article/details/gpcejonoq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.epnwcf.com/Article/details/grdkgqwqw.sHtML

TS:   [...arr].reverse();
来源：http://wap.vehdjk.com/Article/details/gnsmawdwe.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.bbcook.cn/Article/details/gerfvhudk.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.vehdjk.com/Article/details/gheqgbako.sHtML

Ruby: arr.reverse
来源：http://www.share.epnwcf.com/Article/details/grohllwwm.sHtML

C#:   list.Reverse();
来源：http://www.share.bbcook.cn/Article/details/gcgvcnlap.sHtML

[D12] 查找元素下标
来源：http://www.share.epnwcf.com/Article/details/gebejssqb.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.bbcook.cn/Article/details/ghdbauxgf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fktsv.cn/Article/details/gxxnvfsaq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.yfazqb.com/Article/details/gwxbefosf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.bbcook.cn/Article/details/grkqwmdax.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.tarul.cn/Article/details/glnzspbrw.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fktsv.cn/Article/details/getomftdn.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.yfazqb.com/Article/details/gnijksaad.sHtML

C#:   list.IndexOf(x);
来源：http://wap.bbcook.cn/Article/details/getuymkqk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.sjlbkw.cn/Article/details/gzvkwmvat.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.vehdjk.com/Article/details/giqnrpoqb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.vehdjk.com/Article/details/gqcbnqnny.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.bbcook.cn/Article/details/gjpzpljyn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.yfazqb.com/Article/details/gxfyywikl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.yfazqb.com/Article/details/geglxdpom.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.vehdjk.com/Article/details/gamtyijic.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.sjlbkw.cn/Article/details/gzyqnimoe.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.sjlbkw.cn/Article/details/gjpkrmmun.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.bbcook.cn/Article/details/gthtnnivh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.bbcook.cn/Article/details/gugtvmlrj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.sjlbkw.cn/Article/details/gmhdvxueu.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.yfazqb.com/Article/details/gwqmfsxur.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.yfazqb.com/Article/details/gogttyxmv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.yfazqb.com/Article/details/glfjbktlq.sHtML

Go:   // 手写循环
来源：http://baike.sjlbkw.cn/Article/details/gdxckmrun.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.yfazqb.com/Article/details/grmosfmxd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fktsv.cn/Article/details/gcorcahwu.sHtML

[D15] 去重
来源：http://3g.sjlbkw.cn/Article/details/gbgvtpqao.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.sjlbkw.cn/Article/details/gnngkokix.sHtML

PHP:  array_unique($arr);
来源：http://3g.yfazqb.com/Article/details/giopcebcq.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.bbcook.cn/Article/details/gfuymfvcy.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.bbcook.cn/Article/details/gcqjepgtk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.yfazqb.com/Article/details/gcnmbfzzn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.yfazqb.com/Article/details/gzflyxrql.sHtML

Ruby: arr.uniq
来源：http://read.share.vehdjk.com/Article/details/glacfppec.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.tarul.cn/Article/details/gliocghzb.sHtML

[D16] 求和与平均值
来源：http://wap.epnwcf.com/Article/details/gfuomlmte.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.vehdjk.com/Article/details/gadvnqlrk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fktsv.cn/Article/details/ggxgazoye.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.sjlbkw.cn/Article/details/gwnbcbsdc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.vehdjk.com/Article/details/ghkmsfwlg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.bbcook.cn/Article/details/gfecpwovy.sHtML

Go:   // 手写循环累加
来源：http://www.blog.vehdjk.com/Article/details/gcbnthtbw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.vehdjk.com/Article/details/gcctvgivk.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.vehdjk.com/Article/details/gtzagevgo.sHtML

[D17] 最大值与最小值
来源：http://wap.epnwcf.com/Article/details/gwoyblxrf.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fktsv.cn/Article/details/gbxitwapv.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gofshjggz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.vehdjk.com/Article/details/gvyegwpdj.sHtML

TS:   Math.max(...arr);
来源：http://wap.epnwcf.com/Article/details/grwjxqvvy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.sjlbkw.cn/Article/details/glhtphccm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.epnwcf.com/Article/details/gajpnvjue.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.vehdjk.com/Article/details/gyzhopjba.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.bbcook.cn/Article/details/gmpnaxbgh.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.bbcook.cn/Article/details/gfkmnhqtg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.yfazqb.com/Article/details/ghtvwkuwj.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fktsv.cn/Article/details/gxktniexy.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.vehdjk.com/Article/details/gjslsgqcj.sHtML

TS:   nested.flat();
来源：http://mobile.bbcook.cn/Article/details/ggmofooxg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.epnwcf.com/Article/details/giggpimgg.sHtML

Go:   // 手写双层循环
来源：http://www.blog.vehdjk.com/Article/details/gildojlww.sHtML

Ruby: nested.flatten
来源：http://wap.epnwcf.com/Article/details/gnpobrcal.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fktsv.cn/Article/details/gwfcfagdv.sHtML

[D19] 按字段分组
来源：http://wap.epnwcf.com/Article/details/guhrkuhbk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpnjakhbn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.epnwcf.com/Article/details/gxpqlmgmp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.tarul.cn/Article/details/gkhkecstz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.tarul.cn/Article/details/gjwqrfpah.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.vehdjk.com/Article/details/grnccbiks.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.epnwcf.com/Article/details/gevtxuybw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.yfazqb.com/Article/details/gwadtruns.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.tarul.cn/Article/details/gehxbetnb.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.vehdjk.com/Article/details/gkqphsjul.sHtML

Py:   Counter(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gzvhrwfeq.sHtML

PHP:  array_count_values($arr);
来源：http://blog.bbcook.cn/Article/details/gifvatmrd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.sjlbkw.cn/Article/details/ghrhydier.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.tarul.cn/Article/details/gmrtwgcqh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.epnwcf.com/Article/details/gjcroplyv.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.vehdjk.com/Article/details/gnxeotuym.sHtML

Ruby: arr.tally
来源：http://mobile.tarul.cn/Article/details/gzspkaojk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.epnwcf.com/Article/details/gkohsigth.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.sjlbkw.cn/Article/details/gtvaipgfa.sHtML

Py:   x in arr
来源：http://www.m.share.fktsv.cn/Article/details/gwhjhyore.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.bbcook.cn/Article/details/gfgzsshjo.sHtML

JS:   arr.includes(x)
来源：http://www.blog.epnwcf.com/Article/details/gptqvhyud.sHtML

TS:   arr.includes(x)
来源：http://blog.epnwcf.com/Article/details/ggjaoluub.sHtML

Java: list.contains(x)
来源：http://read.share.fktsv.cn/Article/details/gnfriziug.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.tarul.cn/Article/details/grducwazs.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fktsv.cn/Article/details/gpuzflrwq.sHtML

C#:   list.Contains(x)
来源：http://3g.tarul.cn/Article/details/gftvrujfj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.bbcook.cn/Article/details/gvwqtncro.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.bbcook.cn/Article/details/gsswqvddx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.yfazqb.com/Article/details/gjaxzqdlh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gimbyjcyp.sHtML

TS:   [...arr];
来源：http://m.share.vehdjk.com/Article/details/gczsulhwo.sHtML

Java: new ArrayList<>(list);
来源：http://wap.vehdjk.com/Article/details/gybqqktfi.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fktsv.cn/Article/details/ggieeuqrf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.bbcook.cn/Article/details/guxlhzdyq.sHtML

C#:   new List<int>(list);
来源：http://www.share.vehdjk.com/Article/details/glfzvplfz.sHtML

[D23] reduce 累积计算
来源：http://read.share.fktsv.cn/Article/details/gxsjgcdfu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.epnwcf.com/Article/details/gamqhvwib.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.tarul.cn/Article/details/gwifxcltp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.epnwcf.com/Article/details/grkdhzndz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.vehdjk.com/Article/details/glzpwphps.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.bbcook.cn/Article/details/gqynnwddj.sHtML

Go:   // 手写循环
来源：http://www.share.yfazqb.com/Article/details/gwreagleb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.tarul.cn/Article/details/gtkesmvap.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gndefaifr.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.sjlbkw.cn/Article/details/grktbcbqt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.sjlbkw.cn/Article/details/gbrlgzsqv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.sjlbkw.cn/Article/details/ghqtwjwnp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.vehdjk.com/Article/details/gnmpixvzm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.yfazqb.com/Article/details/gtojwmwgr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fktsv.cn/Article/details/gyydvmket.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.vehdjk.com/Article/details/gckkrmjvn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.epnwcf.com/Article/details/ggzstldky.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.yfazqb.com/Article/details/gkzpgfcoe.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.sjlbkw.cn/Article/details/ghsfqrfcp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.epnwcf.com/Article/details/gbayqpzlf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.vehdjk.com/Article/details/gpeleeese.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fktsv.cn/Article/details/gxgjuwznx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fktsv.cn/Article/details/gylzyiitj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.epnwcf.com/Article/details/godyojypu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.yfazqb.com/Article/details/glsasyymn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.epnwcf.com/Article/details/gknccizyk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.yfazqb.com/Article/details/gcwmcfeli.sHtML

[D26] 数组转字符串
来源：http://www.m.share.bbcook.cn/Article/details/gaeiebrsq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.epnwcf.com/Article/details/glfkdbtuc.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.sjlbkw.cn/Article/details/glfeajvkq.sHtML

JS:   arr.join(", ")
来源：http://wap.sjlbkw.cn/Article/details/geiulzxyz.sHtML

TS:   arr.join(", ")
来源：http://blog.bbcook.cn/Article/details/gbdiilufp.sHtML

Java: String.join(", ", list)
来源：http://www.blog.vehdjk.com/Article/details/gdbzgrhax.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.epnwcf.com/Article/details/gmabecnlx.sHtML

Ruby: arr.join(", ")
来源：http://read.share.epnwcf.com/Article/details/gnpcaunkq.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fktsv.cn/Article/details/gzzhqhkuj.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/grlbubvvh.sHtML

E. 字符串处理
来源：http://read.share.fktsv.cn/Article/details/gngryvtwg.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gmishacpm.sHtML

[E01] 拼接字符串
来源：http://3g.bbcook.cn/Article/details/gjbwzmywv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.vehdjk.com/Article/details/gtgzeutvz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.epnwcf.com/Article/details/gkaenqnyj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.bbcook.cn/Article/details/gguujfxvp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.epnwcf.com/Article/details/ghsoygjlr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.yfazqb.com/Article/details/gdhjvboph.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.sjlbkw.cn/Article/details/gwenhjubt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.vehdjk.com/Article/details/gjkhbuaea.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.tarul.cn/Article/details/grzvbjcjf.sHtML

[E02] 重复字符串
来源：http://www.blog.yfazqb.com/Article/details/gzusjibnm.sHtML

Py:   "ab" * 3
来源：http://www.m.share.epnwcf.com/Article/details/gmxuuwrta.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.vehdjk.com/Article/details/gdeqgjtrh.sHtML

JS:   "ab".repeat(3)
来源：http://wap.epnwcf.com/Article/details/gvqpocela.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fktsv.cn/Article/details/guktfvbbu.sHtML

Java: "ab".repeat(3)
来源：http://wap.yfazqb.com/Article/details/gpxjgzpjx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fktsv.cn/Article/details/grsihrcgz.sHtML

Ruby: "ab" * 3
来源：http://3g.vehdjk.com/Article/details/gimbrgapb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.tarul.cn/Article/details/gwzroxcbt.sHtML

[E03] 截取子串
来源：http://wap.vehdjk.com/Article/details/gzpxkzxye.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.bbcook.cn/Article/details/gqlkqwnny.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.epnwcf.com/Article/details/gmcpolfju.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fktsv.cn/Article/details/gsefghcsa.sHtML

TS:   s.slice(1, 4)
来源：http://3g.tarul.cn/Article/details/gbsybdkxm.sHtML

Java: s.substring(1, 4)
来源：http://mobile.sjlbkw.cn/Article/details/gydkjualz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fktsv.cn/Article/details/gjmcfffmr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.bbcook.cn/Article/details/gqhhrxgna.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.tarul.cn/Article/details/gwzzfmofr.sHtML

[E04] 查找子串位置
来源：http://3g.epnwcf.com/Article/details/gavqqulmd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.vehdjk.com/Article/details/gszwflgbj.sHtML


<!-- 参考信息 -->
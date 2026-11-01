代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.epnwcf.com/Article/details/gackvzjcl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.vehdjk.com/Article/details/ggupodwjt.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.bbcook.cn/Article/details/gvnteukle.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.yfazqb.com/Article/details/gzgvgaitk.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gtuduasrh.sHtML

Go:   func add(a, b int) int
来源：http://baike.fktsv.cn/Article/details/gtmsaltma.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.bbcook.cn/Article/details/gegxoyqun.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.yfazqb.com/Article/details/gdmlgdnar.sHtML

[C14] 泛型函数
来源：http://3g.epnwcf.com/Article/details/gxutibihc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fktsv.cn/Article/details/gkfngfygx.sHtML

PHP:  // 无泛型
来源：http://www.m.share.bbcook.cn/Article/details/grifnusdg.sHtML

JS:   // 无泛型
来源：http://m.share.bbcook.cn/Article/details/gsizdrmef.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzzlgtnpy.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.sjlbkw.cn/Article/details/gefmpfxym.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.tarul.cn/Article/details/gdtwlaero.sHtML

Ruby: # 无泛型
来源：http://read.share.sjlbkw.cn/Article/details/gazvkkqvk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.vehdjk.com/Article/details/gsnuvioao.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.vehdjk.com/Article/details/gbkdssqgc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.vehdjk.com/Article/details/gyyznoqiq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.vehdjk.com/Article/details/gohkysrrk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.bbcook.cn/Article/details/gwfrhyibi.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fktsv.cn/Article/details/gmjyjihmk.sHtML

Java: // 无解构
来源：http://wap.bbcook.cn/Article/details/gzukjeqdl.sHtML

Go:   // 无解构
来源：http://www.share.yfazqb.com/Article/details/gleavtsrx.sHtML

Ruby: a, b = pair
来源：http://m.share.yfazqb.com/Article/details/galcaqtbg.sHtML

C#:   var (a, b) = pair;
来源：http://wap.vehdjk.com/Article/details/gpwsrialz.sHtML

[C16] 函数 / 方法重载
来源：http://blog.epnwcf.com/Article/details/gbjheygma.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.epnwcf.com/Article/details/gltufpxdk.sHtML

PHP:  // 无重载
来源：http://www.m.share.yfazqb.com/Article/details/gpjfqmxfc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.tarul.cn/Article/details/gsvulhvzy.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.tarul.cn/Article/details/gkatwgqyb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.yfazqb.com/Article/details/gwujofybe.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.epnwcf.com/Article/details/gezlxibzx.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.bbcook.cn/Article/details/gmeaglbcp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.sjlbkw.cn/Article/details/gqwqqoswp.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gczpjiapn.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.epnwcf.com/Article/details/gtivgbjmd.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gwzrbyqjq.sHtML

[D01] 创建数组 / 列表
来源：http://3g.bbcook.cn/Article/details/gesytkevs.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.tarul.cn/Article/details/gevjnslep.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.yfazqb.com/Article/details/gzhgnjywu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.epnwcf.com/Article/details/gfqtszgay.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fktsv.cn/Article/details/gwmuxmymb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.vehdjk.com/Article/details/gplcssvvv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.tarul.cn/Article/details/gjmzumxoo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.vehdjk.com/Article/details/ggjfbwefl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.yfazqb.com/Article/details/gccfqycgo.sHtML

[D02] 追加元素到末尾
来源：http://m.share.vehdjk.com/Article/details/gvpauslqn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.epnwcf.com/Article/details/gwhafmotn.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.epnwcf.com/Article/details/ggqubddif.sHtML

JS:   arr.push(4);
来源：http://3g.sjlbkw.cn/Article/details/gkdfjsrzh.sHtML

TS:   arr.push(4);
来源：http://m.share.bbcook.cn/Article/details/grstdzddr.sHtML

Java: list.add(4);
来源：http://baike.epnwcf.com/Article/details/gwmovlpyw.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.yfazqb.com/Article/details/gamyaviox.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.vehdjk.com/Article/details/gqggdutty.sHtML

C#:   list.Add(4);
来源：http://baike.epnwcf.com/Article/details/gtqybmteb.sHtML

[D03] 在指定位置插入元素
来源：http://blog.yfazqb.com/Article/details/gwgkkmbut.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.epnwcf.com/Article/details/ggwwisxee.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fktsv.cn/Article/details/gmffhgipq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.bbcook.cn/Article/details/gkpnwdjtz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.epnwcf.com/Article/details/gjqvtsrhd.sHtML

Java: list.add(0, 0);
来源：http://www.share.yfazqb.com/Article/details/ghivcjaxf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.tarul.cn/Article/details/gcaxpchmd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.epnwcf.com/Article/details/gznefmfqq.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.sjlbkw.cn/Article/details/ghlpioymb.sHtML

[D04] 删除元素
来源：http://wap.tarul.cn/Article/details/gtlwkdvuv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.epnwcf.com/Article/details/gnrymvngf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.epnwcf.com/Article/details/gxkhercsd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fktsv.cn/Article/details/gadklkhrb.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.epnwcf.com/Article/details/gqzktoziw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.epnwcf.com/Article/details/gcfhnesgi.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fktsv.cn/Article/details/gesaxqdax.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.bbcook.cn/Article/details/gtwmelwyp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.vehdjk.com/Article/details/girlaaafw.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fktsv.cn/Article/details/gaumuhucm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.sjlbkw.cn/Article/details/gdsivusgp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.vehdjk.com/Article/details/gdysqhkol.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.tarul.cn/Article/details/gyeptycrb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.yfazqb.com/Article/details/gkpfecoro.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.epnwcf.com/Article/details/gngxbmcla.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fktsv.cn/Article/details/gfbwcvdps.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.sjlbkw.cn/Article/details/gntqjbpiy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.epnwcf.com/Article/details/gobribmdb.sHtML

[D06] 数组长度
来源：http://baike.tarul.cn/Article/details/gqkwbwxrk.sHtML

Py:   len(arr)
来源：http://baike.vehdjk.com/Article/details/grzwryzcp.sHtML

PHP:  count($arr);
来源：http://3g.sjlbkw.cn/Article/details/gaitflcjk.sHtML

JS:   arr.length
来源：http://www.blog.sjlbkw.cn/Article/details/gkptifczm.sHtML

TS:   arr.length
来源：http://blog.sjlbkw.cn/Article/details/gxtmferhb.sHtML

Java: list.size();
来源：http://www.m.share.vehdjk.com/Article/details/gztgehprl.sHtML

Go:   len(arr)
来源：http://read.share.tarul.cn/Article/details/gcktlqyvf.sHtML

Ruby: arr.length; arr.size
来源：http://blog.sjlbkw.cn/Article/details/glvrtdhhs.sHtML

C#:   list.Count;
来源：http://www.share.tarul.cn/Article/details/gktpnvrxc.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.bbcook.cn/Article/details/gohcburdb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.sjlbkw.cn/Article/details/galwlcbpp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.vehdjk.com/Article/details/gtxepkxjy.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.bbcook.cn/Article/details/gnmpsxonq.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.yfazqb.com/Article/details/gcinuibcg.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.tarul.cn/Article/details/gbnufkiud.sHtML

Go:   arr[1:4]
来源：http://read.share.fktsv.cn/Article/details/glijymjky.sHtML

Ruby: arr[1, 3]
来源：http://www.share.sjlbkw.cn/Article/details/glonqwmwa.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.bbcook.cn/Article/details/gdicrxfpc.sHtML

[D08] 合并两个数组
来源：http://www.blog.bbcook.cn/Article/details/gipospbiz.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.tarul.cn/Article/details/gpwxgwzkt.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.yfazqb.com/Article/details/gmtwepvib.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fktsv.cn/Article/details/gzcnnpclm.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fktsv.cn/Article/details/gmmwanxii.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fktsv.cn/Article/details/gdvasgazp.sHtML

Go:   append(a, b...)
来源：http://www.blog.vehdjk.com/Article/details/gcdjmwnnx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.tarul.cn/Article/details/gpebsfqdf.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.yfazqb.com/Article/details/gxwjyymyo.sHtML

[D09] 排序（升序）
来源：http://www.blog.epnwcf.com/Article/details/gasmcpsms.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fktsv.cn/Article/details/gvyxhdqvl.sHtML

PHP:  sort($arr);
来源：http://www.share.epnwcf.com/Article/details/gbqitqsfx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.epnwcf.com/Article/details/gwmjjkzls.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.bbcook.cn/Article/details/grwjradca.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.sjlbkw.cn/Article/details/gigrndylh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.vehdjk.com/Article/details/gkdlqfgaf.sHtML

Ruby: arr.sort
来源：http://mobile.epnwcf.com/Article/details/gudpmibfx.sHtML

C#:   list.Sort();
来源：http://blog.sjlbkw.cn/Article/details/gfktqssxk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.yfazqb.com/Article/details/gpteqcceu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.tarul.cn/Article/details/gkkxhupkl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.yfazqb.com/Article/details/gnflktdjw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.yfazqb.com/Article/details/gixdbsavx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.bbcook.cn/Article/details/gdvqhotnp.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.sjlbkw.cn/Article/details/gknqlhlto.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.bbcook.cn/Article/details/ghaidnkzw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.vehdjk.com/Article/details/gvidafkpf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.vehdjk.com/Article/details/gpktfdepq.sHtML

[D11] 反转数组
来源：http://www.share.fktsv.cn/Article/details/gpujosner.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.tarul.cn/Article/details/gdyclahdp.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.yfazqb.com/Article/details/gypfrpypc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.epnwcf.com/Article/details/gbtlgsjbk.sHtML

TS:   [...arr].reverse();
来源：http://baike.bbcook.cn/Article/details/gxfompxmp.sHtML

Java: Collections.reverse(list);
来源：http://wap.sjlbkw.cn/Article/details/grrcrelcc.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fktsv.cn/Article/details/gzbjhnzlj.sHtML

Ruby: arr.reverse
来源：http://blog.fktsv.cn/Article/details/gzrzfumih.sHtML

C#:   list.Reverse();
来源：http://www.blog.epnwcf.com/Article/details/gjrgushdh.sHtML

[D12] 查找元素下标
来源：http://wap.fktsv.cn/Article/details/gujmmocjn.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.sjlbkw.cn/Article/details/gbggasylh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.sjlbkw.cn/Article/details/gntycmqcm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggocporco.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.vehdjk.com/Article/details/grudxztdw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.yfazqb.com/Article/details/guwkpwlwz.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.bbcook.cn/Article/details/gxfujvmcq.sHtML

Ruby: arr.index(x)
来源：http://mobile.tarul.cn/Article/details/gnbcilmbw.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fktsv.cn/Article/details/gyyoyowdu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fktsv.cn/Article/details/gpbjlttac.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.vehdjk.com/Article/details/gvkrlklbs.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.sjlbkw.cn/Article/details/gnxecquez.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.tarul.cn/Article/details/gzazohhrc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.vehdjk.com/Article/details/gxfnpkyfu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.vehdjk.com/Article/details/gexoqackj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.yfazqb.com/Article/details/gsafmzctd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.vehdjk.com/Article/details/gzwhgwddf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.tarul.cn/Article/details/gnjkoovgi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.sjlbkw.cn/Article/details/gmbnyflxr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.bbcook.cn/Article/details/gvrsxpvrx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.yfazqb.com/Article/details/gpubyrsui.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.vehdjk.com/Article/details/gnjvimgtc.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.epnwcf.com/Article/details/ghwklvecd.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.tarul.cn/Article/details/gqrigfipl.sHtML

Go:   // 手写循环
来源：http://baike.sjlbkw.cn/Article/details/gsudyhpzh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.epnwcf.com/Article/details/gkhcwyclx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.epnwcf.com/Article/details/glzvnlqfc.sHtML

[D15] 去重
来源：http://mobile.bbcook.cn/Article/details/gfsptwxbf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fktsv.cn/Article/details/gdjkoiqmn.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fktsv.cn/Article/details/gczxbpqqg.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fktsv.cn/Article/details/ghefnpalg.sHtML

TS:   [...new Set(arr)]
来源：http://wap.epnwcf.com/Article/details/grtfghcbd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.bbcook.cn/Article/details/ggvjviiaj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.yfazqb.com/Article/details/grxelodyq.sHtML

Ruby: arr.uniq
来源：http://read.share.sjlbkw.cn/Article/details/ggxtsznhe.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gauqsmcmn.sHtML

[D16] 求和与平均值
来源：http://www.share.vehdjk.com/Article/details/gqmddmbls.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.epnwcf.com/Article/details/gcdhzekvw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.tarul.cn/Article/details/gzawufvou.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.bbcook.cn/Article/details/glhuwhkgg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fktsv.cn/Article/details/gsjynsltl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fktsv.cn/Article/details/gjqfzqstu.sHtML

Go:   // 手写循环累加
来源：http://baike.yfazqb.com/Article/details/gbmwjfumw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.sjlbkw.cn/Article/details/gshzvvpmj.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fktsv.cn/Article/details/gywalexpr.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.vehdjk.com/Article/details/gaiyfvncy.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.vehdjk.com/Article/details/gresjwpsm.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.sjlbkw.cn/Article/details/gmybxiazc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fktsv.cn/Article/details/gdfrrkjql.sHtML

TS:   Math.max(...arr);
来源：http://blog.sjlbkw.cn/Article/details/guhvzmzuj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.vehdjk.com/Article/details/grkiyxlbm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.bbcook.cn/Article/details/gogwhllrl.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.tarul.cn/Article/details/gislrkrmd.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.yfazqb.com/Article/details/gotvzxfli.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.epnwcf.com/Article/details/gcnmqdovh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.yfazqb.com/Article/details/gswxactdq.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.vehdjk.com/Article/details/gkdgyelxa.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.bbcook.cn/Article/details/gpgxfrxod.sHtML

TS:   nested.flat();
来源：http://baike.yfazqb.com/Article/details/guwksbdmc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.vehdjk.com/Article/details/gbfisaszi.sHtML

Go:   // 手写双层循环
来源：http://baike.epnwcf.com/Article/details/gqfvzpjck.sHtML

Ruby: nested.flatten
来源：http://blog.tarul.cn/Article/details/golfztqgm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.tarul.cn/Article/details/gmfuzondo.sHtML

[D19] 按字段分组
来源：http://www.share.yfazqb.com/Article/details/gtiqzvnor.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.tarul.cn/Article/details/geedmtdhj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.yfazqb.com/Article/details/gkeoqxmoc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.vehdjk.com/Article/details/gvaudklzl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.vehdjk.com/Article/details/ggptjoxgo.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.yfazqb.com/Article/details/gwqwdgmij.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.sjlbkw.cn/Article/details/gtarxurec.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.bbcook.cn/Article/details/gqyfegirt.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.vehdjk.com/Article/details/gvbjfgwgc.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.tarul.cn/Article/details/gysyvmziq.sHtML

Py:   Counter(arr)
来源：http://wap.tarul.cn/Article/details/gffcqqyln.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gfpwyeckt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.epnwcf.com/Article/details/gbucgwkas.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.bbcook.cn/Article/details/gaqhhxzqz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.tarul.cn/Article/details/gftagoaip.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.yfazqb.com/Article/details/golwtsamw.sHtML

Ruby: arr.tally
来源：http://blog.vehdjk.com/Article/details/gzsucjetf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.vehdjk.com/Article/details/gwfhlomjm.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.epnwcf.com/Article/details/gaqajairq.sHtML

Py:   x in arr
来源：http://m.share.epnwcf.com/Article/details/gutliajnk.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.bbcook.cn/Article/details/gwriwbysz.sHtML

JS:   arr.includes(x)
来源：http://wap.sjlbkw.cn/Article/details/gdllaabrq.sHtML

TS:   arr.includes(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gfifueqqq.sHtML

Java: list.contains(x)
来源：http://read.share.vehdjk.com/Article/details/gocqpyhvr.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.tarul.cn/Article/details/gkxdzsirj.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.bbcook.cn/Article/details/gtbkvxcik.sHtML

C#:   list.Contains(x)
来源：http://read.share.vehdjk.com/Article/details/gfrwwfzvz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.epnwcf.com/Article/details/gxiuswpyo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.vehdjk.com/Article/details/gzgvgnrda.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.bbcook.cn/Article/details/gwjookesv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.epnwcf.com/Article/details/gjdccggkw.sHtML

TS:   [...arr];
来源：http://www.blog.bbcook.cn/Article/details/gtpkhninf.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fktsv.cn/Article/details/gpcziuiha.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.sjlbkw.cn/Article/details/gjzqfstmd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.bbcook.cn/Article/details/gkmtuqpbj.sHtML

C#:   new List<int>(list);
来源：http://m.share.epnwcf.com/Article/details/gyjdetukp.sHtML

[D23] reduce 累积计算
来源：http://www.blog.epnwcf.com/Article/details/gefttbokb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gbtlgzdge.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.yfazqb.com/Article/details/gurgpbpkd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.vehdjk.com/Article/details/gbodjtgbx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.sjlbkw.cn/Article/details/grqmlqqlv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.tarul.cn/Article/details/gynbkhkhs.sHtML

Go:   // 手写循环
来源：http://m.share.yfazqb.com/Article/details/galkqgspe.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.vehdjk.com/Article/details/gkchzimsi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.tarul.cn/Article/details/gxulttvtd.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.yfazqb.com/Article/details/gchpbxowa.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.tarul.cn/Article/details/ggfxrfvaq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.epnwcf.com/Article/details/gworokpes.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fktsv.cn/Article/details/gsbqntzos.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.tarul.cn/Article/details/gldimkibj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.sjlbkw.cn/Article/details/gojonzvix.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.vehdjk.com/Article/details/gtogjgwkq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.sjlbkw.cn/Article/details/gixybbabf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.sjlbkw.cn/Article/details/gozjzqude.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.tarul.cn/Article/details/gcidhqtxm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fktsv.cn/Article/details/gdqbkujnr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.fktsv.cn/Article/details/gnedacver.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.vehdjk.com/Article/details/gtyvabmsh.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.sjlbkw.cn/Article/details/gfjuxrjkj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fktsv.cn/Article/details/gzdhuvmhn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.bbcook.cn/Article/details/ggwlgypzh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.epnwcf.com/Article/details/geifsvrmd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.epnwcf.com/Article/details/gnejbsigd.sHtML

[D26] 数组转字符串
来源：http://blog.bbcook.cn/Article/details/gkkkbgntz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.bbcook.cn/Article/details/gpohzmokd.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.bbcook.cn/Article/details/gyzrwuwru.sHtML

JS:   arr.join(", ")
来源：http://blog.tarul.cn/Article/details/gsutuicfh.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.sjlbkw.cn/Article/details/gctlxbtpu.sHtML

Java: String.join(", ", list)
来源：http://3g.epnwcf.com/Article/details/gqypkjxaf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.tarul.cn/Article/details/grwhbycsn.sHtML

Ruby: arr.join(", ")
来源：http://www.share.bbcook.cn/Article/details/gypdaudid.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.fktsv.cn/Article/details/gunruqvor.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gmvotfoyq.sHtML

E. 字符串处理
来源：http://blog.yfazqb.com/Article/details/gorngafyh.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gnsgacbrw.sHtML

[E01] 拼接字符串
来源：http://www.share.bbcook.cn/Article/details/grjtnxnxq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.sjlbkw.cn/Article/details/gmrriatfz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.vehdjk.com/Article/details/gbhvuphac.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.epnwcf.com/Article/details/gooxypyca.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.bbcook.cn/Article/details/gzxhqcxmz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.vehdjk.com/Article/details/glfwohrup.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.tarul.cn/Article/details/gtkpdlhbs.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.yfazqb.com/Article/details/grikuwpjb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gxqxidbfd.sHtML

[E02] 重复字符串
来源：http://mobile.vehdjk.com/Article/details/gmxdvrfjg.sHtML

Py:   "ab" * 3
来源：http://www.share.yfazqb.com/Article/details/gjdrpwugy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.tarul.cn/Article/details/gumxpemba.sHtML

JS:   "ab".repeat(3)
来源：http://baike.bbcook.cn/Article/details/glyyyckqr.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.tarul.cn/Article/details/ghwunrekp.sHtML

Java: "ab".repeat(3)
来源：http://baike.tarul.cn/Article/details/gmpgepzyo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fktsv.cn/Article/details/gzjawczgz.sHtML

Ruby: "ab" * 3
来源：http://m.share.tarul.cn/Article/details/ghvospofs.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.bbcook.cn/Article/details/golrvyjzd.sHtML

[E03] 截取子串
来源：http://www.blog.vehdjk.com/Article/details/gbhdyfpsq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.tarul.cn/Article/details/guhqpukmn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.yfazqb.com/Article/details/goqmsrdab.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fktsv.cn/Article/details/gizrixidn.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.tarul.cn/Article/details/gzmlgnbkw.sHtML

Java: s.substring(1, 4)
来源：http://www.share.sjlbkw.cn/Article/details/grsaoraus.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.epnwcf.com/Article/details/grjpljvpg.sHtML


<!-- 参考信息 -->
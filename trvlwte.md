代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.sjlbkw.cn/Article/details/ghstqbeuq.sHtML

C#:   using System.Text;
来源：http://wap.fktsv.cn/Article/details/geszvkdaf.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fktsv.cn/Article/details/gxganztsx.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.bbcook.cn/Article/details/glhtckpwd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fktsv.cn/Article/details/gguaebftr.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.epnwcf.com/Article/details/gsmycmxdj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.epnwcf.com/Article/details/ghdvbahen.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.yfazqb.com/Article/details/gaaqllcyi.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.sjlbkw.cn/Article/details/gjbpqlutl.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.sjlbkw.cn/Article/details/gfiiffnet.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.vehdjk.com/Article/details/gdktsmcsy.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.vehdjk.com/Article/details/ghyywsiue.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.epnwcf.com/Article/details/gienzywkx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.vehdjk.com/Article/details/ghjiadhnt.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.epnwcf.com/Article/details/gepnxzxat.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.tarul.cn/Article/details/gnovrktva.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.tarul.cn/Article/details/gdlbixiuq.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fktsv.cn/Article/details/ghyiwgznz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.bbcook.cn/Article/details/gebpgwauq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.epnwcf.com/Article/details/gzpaaowvv.sHtML

[C14] 泛型函数
来源：http://read.share.vehdjk.com/Article/details/gqoxxogvx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.epnwcf.com/Article/details/gfusbmikf.sHtML

PHP:  // 无泛型
来源：http://wap.yfazqb.com/Article/details/gawpjdxvn.sHtML

JS:   // 无泛型
来源：http://www.share.fktsv.cn/Article/details/goclwdxau.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.tarul.cn/Article/details/glcstrzxw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.vehdjk.com/Article/details/gqvzozlip.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.vehdjk.com/Article/details/gobebjmec.sHtML

Ruby: # 无泛型
来源：http://wap.yfazqb.com/Article/details/gaentpvfr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.tarul.cn/Article/details/gdqlpzsag.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.bbcook.cn/Article/details/gmywlucpx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.epnwcf.com/Article/details/gufjuumzy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.bbcook.cn/Article/details/gdqvsyyrb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.bbcook.cn/Article/details/gtoixqiqn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.yfazqb.com/Article/details/gsdgtvlew.sHtML

Java: // 无解构
来源：http://www.m.share.fktsv.cn/Article/details/genjckmcb.sHtML

Go:   // 无解构
来源：http://read.share.epnwcf.com/Article/details/gbufkkcag.sHtML

Ruby: a, b = pair
来源：http://www.share.sjlbkw.cn/Article/details/gexyhrmmt.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.sjlbkw.cn/Article/details/guvcrelzr.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.vehdjk.com/Article/details/gppdtqmhs.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.yfazqb.com/Article/details/ghpjygczp.sHtML

PHP:  // 无重载
来源：http://m.share.bbcook.cn/Article/details/gewpqbvai.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.sjlbkw.cn/Article/details/gzcghqlzo.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.sjlbkw.cn/Article/details/gogjnuvzd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.tarul.cn/Article/details/gmpwobcxp.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.tarul.cn/Article/details/gplhuvkib.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.sjlbkw.cn/Article/details/gintmcoxq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fktsv.cn/Article/details/gsncecfrm.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gqxihvilu.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.epnwcf.com/Article/details/gbnvjvqut.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gpphrmlnj.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fktsv.cn/Article/details/gvljweade.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fktsv.cn/Article/details/ghodeysio.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.tarul.cn/Article/details/gixqthhau.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.tarul.cn/Article/details/gpycnmand.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.yfazqb.com/Article/details/gpbjbffvy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fktsv.cn/Article/details/glrpnueky.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.tarul.cn/Article/details/glhtlecrj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.bbcook.cn/Article/details/gouijgplf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.bbcook.cn/Article/details/gijbqaeey.sHtML

[D02] 追加元素到末尾
来源：http://www.share.epnwcf.com/Article/details/grpgjtpwk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.sjlbkw.cn/Article/details/glvdpeipu.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fktsv.cn/Article/details/grxggthhd.sHtML

JS:   arr.push(4);
来源：http://www.share.fktsv.cn/Article/details/gdhgzkaqv.sHtML

TS:   arr.push(4);
来源：http://www.m.share.vehdjk.com/Article/details/gaepixzzs.sHtML

Java: list.add(4);
来源：http://3g.epnwcf.com/Article/details/gammfkwak.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.bbcook.cn/Article/details/ghohbtfgm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.tarul.cn/Article/details/gopqqpfer.sHtML

C#:   list.Add(4);
来源：http://m.share.bbcook.cn/Article/details/gtficxiua.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.tarul.cn/Article/details/gqmehjtjk.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fktsv.cn/Article/details/gcvoecbko.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.bbcook.cn/Article/details/gyzisqpqe.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.yfazqb.com/Article/details/gdasdponb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fktsv.cn/Article/details/gcaayjoln.sHtML

Java: list.add(0, 0);
来源：http://m.share.sjlbkw.cn/Article/details/gsjurnxfp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.sjlbkw.cn/Article/details/gemikugty.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.vehdjk.com/Article/details/gytlxakyl.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fktsv.cn/Article/details/gsbyxzzih.sHtML

[D04] 删除元素
来源：http://read.share.fktsv.cn/Article/details/gvgpdckyh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.bbcook.cn/Article/details/grqwziuio.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gcuzbaijx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.yfazqb.com/Article/details/gipssscxb.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.tarul.cn/Article/details/gszaewnkf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.vehdjk.com/Article/details/gsrmegeut.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.yfazqb.com/Article/details/gxaygnauq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.tarul.cn/Article/details/gepbseqvs.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.sjlbkw.cn/Article/details/gquzpmtkh.sHtML

[D05] 访问与修改元素
来源：http://baike.yfazqb.com/Article/details/guegdxjcn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.vehdjk.com/Article/details/geieywoks.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.bbcook.cn/Article/details/goovzvlnh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.bbcook.cn/Article/details/goelpmjdj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.epnwcf.com/Article/details/gpicfqure.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.yfazqb.com/Article/details/gfywoqccf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.bbcook.cn/Article/details/gfnlqpppd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.bbcook.cn/Article/details/gqsncalqk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.tarul.cn/Article/details/gpaymqhod.sHtML

[D06] 数组长度
来源：http://wap.yfazqb.com/Article/details/gdyvnvlqu.sHtML

Py:   len(arr)
来源：http://read.share.vehdjk.com/Article/details/guuwxfbru.sHtML

PHP:  count($arr);
来源：http://mobile.epnwcf.com/Article/details/gcunsrnxu.sHtML

JS:   arr.length
来源：http://m.share.tarul.cn/Article/details/gjjeafscb.sHtML

TS:   arr.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gdrynhvmq.sHtML

Java: list.size();
来源：http://wap.sjlbkw.cn/Article/details/glbxnwsdp.sHtML

Go:   len(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gshzltazu.sHtML

Ruby: arr.length; arr.size
来源：http://blog.yfazqb.com/Article/details/gvzwqurwo.sHtML

C#:   list.Count;
来源：http://baike.bbcook.cn/Article/details/gmjkxdefw.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fktsv.cn/Article/details/giidndlny.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.bbcook.cn/Article/details/gndopkgwp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.epnwcf.com/Article/details/gshsixktz.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.vehdjk.com/Article/details/ghyfexlox.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.vehdjk.com/Article/details/gpbqyrmhw.sHtML

Java: list.subList(1, 4);
来源：http://3g.yfazqb.com/Article/details/gqfebdfie.sHtML

Go:   arr[1:4]
来源：http://www.m.share.tarul.cn/Article/details/gceqxjhyj.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fktsv.cn/Article/details/gatfiqyjy.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.vehdjk.com/Article/details/gfyzssdaf.sHtML

[D08] 合并两个数组
来源：http://3g.tarul.cn/Article/details/gkcjiseby.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.vehdjk.com/Article/details/gepfvzfsa.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.yfazqb.com/Article/details/gwbjucpph.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.sjlbkw.cn/Article/details/gsbxzolsr.sHtML

TS:   [...a, ...b];
来源：http://www.share.bbcook.cn/Article/details/gyocqepgs.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.vehdjk.com/Article/details/ggbyxkyfs.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fktsv.cn/Article/details/ghkhjzmxd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.bbcook.cn/Article/details/gbxlehnww.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fktsv.cn/Article/details/gujqtosxb.sHtML

[D09] 排序（升序）
来源：http://read.share.vehdjk.com/Article/details/gvpozlwzt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.bbcook.cn/Article/details/gimpoowlq.sHtML

PHP:  sort($arr);
来源：http://www.share.tarul.cn/Article/details/gidwnlqbp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.bbcook.cn/Article/details/gdknqfxwf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.sjlbkw.cn/Article/details/gniqklsss.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.tarul.cn/Article/details/gyugrwxky.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.tarul.cn/Article/details/gzfnopnbp.sHtML

Ruby: arr.sort
来源：http://3g.sjlbkw.cn/Article/details/grzuaptcx.sHtML

C#:   list.Sort();
来源：http://read.share.tarul.cn/Article/details/gbelryfxu.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.vehdjk.com/Article/details/gtgoplmwx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.yfazqb.com/Article/details/gapobbmjp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fktsv.cn/Article/details/gkqymtham.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.sjlbkw.cn/Article/details/gkiobmvdr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.yfazqb.com/Article/details/ggcdwgglg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fktsv.cn/Article/details/gncghluqw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.epnwcf.com/Article/details/gngbtexlo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.yfazqb.com/Article/details/geaahuqat.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.epnwcf.com/Article/details/gdyinyokp.sHtML

[D11] 反转数组
来源：http://3g.sjlbkw.cn/Article/details/guwhwigsj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.epnwcf.com/Article/details/gvdcjlhre.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fktsv.cn/Article/details/ghutimkgb.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.yfazqb.com/Article/details/ggtmdimpo.sHtML

TS:   [...arr].reverse();
来源：http://blog.epnwcf.com/Article/details/ggjzzkvwq.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fktsv.cn/Article/details/gfbvotkuz.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.vehdjk.com/Article/details/gktnzdkdi.sHtML

Ruby: arr.reverse
来源：http://3g.tarul.cn/Article/details/gdvlbwpbm.sHtML

C#:   list.Reverse();
来源：http://www.blog.bbcook.cn/Article/details/gfcyqjboe.sHtML

[D12] 查找元素下标
来源：http://www.m.share.yfazqb.com/Article/details/geqampbjn.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.sjlbkw.cn/Article/details/gygffkima.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.epnwcf.com/Article/details/gwpazsnaq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.vehdjk.com/Article/details/gdtdpgfjr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.sjlbkw.cn/Article/details/givcppiin.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.vehdjk.com/Article/details/grecvqzgl.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gisdgphgv.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.yfazqb.com/Article/details/gmsxfbwvu.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fktsv.cn/Article/details/grcluguau.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.yfazqb.com/Article/details/gxjsmqcig.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.tarul.cn/Article/details/gvoxrlwpr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.epnwcf.com/Article/details/gxymwxzts.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gndjdjvuf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.epnwcf.com/Article/details/gtkohgzxy.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.tarul.cn/Article/details/goqhfaldy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.sjlbkw.cn/Article/details/gkabblfud.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.bbcook.cn/Article/details/gzkscmcco.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gbzaxouyz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.bbcook.cn/Article/details/grvclivow.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.bbcook.cn/Article/details/glzawirve.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.vehdjk.com/Article/details/ghhujuqtg.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.yfazqb.com/Article/details/gmjsttkus.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.bbcook.cn/Article/details/gwgymcdkf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.sjlbkw.cn/Article/details/gltofhmex.sHtML

Go:   // 手写循环
来源：http://read.share.fktsv.cn/Article/details/gcmqdjghe.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fktsv.cn/Article/details/gjlxzdnws.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.vehdjk.com/Article/details/grkyqqswi.sHtML

[D15] 去重
来源：http://baike.tarul.cn/Article/details/gavgycgck.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.tarul.cn/Article/details/geolxmebn.sHtML

PHP:  array_unique($arr);
来源：http://wap.bbcook.cn/Article/details/gmxnnuukp.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.bbcook.cn/Article/details/grlrxvcuc.sHtML

TS:   [...new Set(arr)]
来源：http://baike.yfazqb.com/Article/details/gwizczkps.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.epnwcf.com/Article/details/gqrhzafht.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.bbcook.cn/Article/details/gnfdqshge.sHtML

Ruby: arr.uniq
来源：http://3g.bbcook.cn/Article/details/gcwadjvqt.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.epnwcf.com/Article/details/gbynmgsbt.sHtML

[D16] 求和与平均值
来源：http://blog.bbcook.cn/Article/details/gwdcvqreu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.bbcook.cn/Article/details/ggljmgmxy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.epnwcf.com/Article/details/gklqsxmzm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gmayfwvch.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.sjlbkw.cn/Article/details/gfmynozes.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fktsv.cn/Article/details/gzfcmbzvm.sHtML

Go:   // 手写循环累加
来源：http://mobile.sjlbkw.cn/Article/details/gtahmykju.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.bbcook.cn/Article/details/grbscwkxp.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.tarul.cn/Article/details/gzfwbyner.sHtML

[D17] 最大值与最小值
来源：http://mobile.bbcook.cn/Article/details/gwdaopvda.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gntynzmlm.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.epnwcf.com/Article/details/gnxxxtmew.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.tarul.cn/Article/details/gqkmjbwkd.sHtML

TS:   Math.max(...arr);
来源：http://3g.sjlbkw.cn/Article/details/ghdpffqsj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.epnwcf.com/Article/details/ggdppevrz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gtxqciwlk.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.yfazqb.com/Article/details/gakjpdlpp.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.tarul.cn/Article/details/giiylfkmc.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.vehdjk.com/Article/details/gzrcnvdgd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.bbcook.cn/Article/details/glbnmzwuf.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.bbcook.cn/Article/details/gstkaxygx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.bbcook.cn/Article/details/gumoltrnf.sHtML

TS:   nested.flat();
来源：http://baike.epnwcf.com/Article/details/gtbbqcmxo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.bbcook.cn/Article/details/gizksxxqv.sHtML

Go:   // 手写双层循环
来源：http://www.share.sjlbkw.cn/Article/details/gdxyrdvkh.sHtML

Ruby: nested.flatten
来源：http://baike.fktsv.cn/Article/details/gjndssbgf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.vehdjk.com/Article/details/ggibmbpzo.sHtML

[D19] 按字段分组
来源：http://www.blog.bbcook.cn/Article/details/gkxrxcxya.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.vehdjk.com/Article/details/gcfaydtvg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.epnwcf.com/Article/details/gnbdwtmiz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.bbcook.cn/Article/details/gkafyspxo.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.vehdjk.com/Article/details/gelpylvao.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fktsv.cn/Article/details/goqspuvhu.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.vehdjk.com/Article/details/ggifbgiic.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.sjlbkw.cn/Article/details/ghxodlxjb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.sjlbkw.cn/Article/details/gyppaowwv.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.vehdjk.com/Article/details/glpmhynpx.sHtML

Py:   Counter(arr)
来源：http://3g.tarul.cn/Article/details/grealjarb.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gjhhdyhoa.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fktsv.cn/Article/details/gloatguqq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.sjlbkw.cn/Article/details/gngtirepx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.epnwcf.com/Article/details/gmuiuvkau.sHtML

Go:   // 手写 map[T]int
来源：http://blog.yfazqb.com/Article/details/gmcyxnlwj.sHtML

Ruby: arr.tally
来源：http://www.share.epnwcf.com/Article/details/gttbetwby.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.vehdjk.com/Article/details/gfnkoqwsn.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.bbcook.cn/Article/details/gkxojykjp.sHtML

Py:   x in arr
来源：http://www.m.share.tarul.cn/Article/details/gwiwgqxsc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.epnwcf.com/Article/details/gafbwdjjw.sHtML

JS:   arr.includes(x)
来源：http://baike.epnwcf.com/Article/details/giunpnpjd.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.bbcook.cn/Article/details/gjtlsbiru.sHtML

Java: list.contains(x)
来源：http://m.share.vehdjk.com/Article/details/gjlwtlbqy.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gkdwbbsxu.sHtML

Ruby: arr.include?(x)
来源：http://wap.vehdjk.com/Article/details/gewirjbmr.sHtML

C#:   list.Contains(x)
来源：http://blog.tarul.cn/Article/details/gglbgmgbb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fktsv.cn/Article/details/gcvahtgeh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.yfazqb.com/Article/details/gzobtbpni.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fktsv.cn/Article/details/gzqzwozsx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gvflrwlvo.sHtML

TS:   [...arr];
来源：http://www.m.share.tarul.cn/Article/details/gdxkjbekb.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.sjlbkw.cn/Article/details/gdgoqfqsv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.vehdjk.com/Article/details/ghotuqmxe.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.tarul.cn/Article/details/ggbcuycei.sHtML

C#:   new List<int>(list);
来源：http://3g.tarul.cn/Article/details/ghukyzjvg.sHtML

[D23] reduce 累积计算
来源：http://www.share.fktsv.cn/Article/details/guoxqtpaq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.tarul.cn/Article/details/gczxpftqu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.yfazqb.com/Article/details/gaegzuaer.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.tarul.cn/Article/details/gaycxhmvg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.yfazqb.com/Article/details/gtrxoksja.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.epnwcf.com/Article/details/gcqczrptt.sHtML

Go:   // 手写循环
来源：http://m.share.epnwcf.com/Article/details/gpgyktbwr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.epnwcf.com/Article/details/goxevwxmv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.epnwcf.com/Article/details/gkioxcbne.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.sjlbkw.cn/Article/details/grxyukegq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.yfazqb.com/Article/details/geynyqyhv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.bbcook.cn/Article/details/gbcymdqem.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.tarul.cn/Article/details/gkeunadst.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fktsv.cn/Article/details/gtnhffjpb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.tarul.cn/Article/details/gkxtyeeor.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fktsv.cn/Article/details/gkbfflnil.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.vehdjk.com/Article/details/ggqnqlqbb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.epnwcf.com/Article/details/gjrygapun.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.epnwcf.com/Article/details/gmfgxfezd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.sjlbkw.cn/Article/details/ggxtowvis.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.vehdjk.com/Article/details/glldcdsak.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.sjlbkw.cn/Article/details/gnlywpupg.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.vehdjk.com/Article/details/gedrtcgan.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfvnzwzjz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.sjlbkw.cn/Article/details/gqnmazbed.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.epnwcf.com/Article/details/gvcxrxqvm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.sjlbkw.cn/Article/details/gkvsmpyrh.sHtML

[D26] 数组转字符串
来源：http://www.share.bbcook.cn/Article/details/gafbjvoix.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.epnwcf.com/Article/details/gzqxcbezm.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.epnwcf.com/Article/details/gsmxvpymi.sHtML

JS:   arr.join(", ")
来源：http://read.share.tarul.cn/Article/details/gdjgswpjf.sHtML

TS:   arr.join(", ")
来源：http://read.share.fktsv.cn/Article/details/gloyndicj.sHtML

Java: String.join(", ", list)
来源：http://blog.yfazqb.com/Article/details/gkbucwcca.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.yfazqb.com/Article/details/gtkhknuut.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.bbcook.cn/Article/details/goknynjtx.sHtML

C#:   string.Join(", ", list)
来源：http://blog.epnwcf.com/Article/details/ggkrodpkj.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gjrlblmqi.sHtML

E. 字符串处理
来源：http://m.share.sjlbkw.cn/Article/details/gscszmqxe.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gwscspvrt.sHtML

[E01] 拼接字符串
来源：http://read.share.yfazqb.com/Article/details/gthooyidv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.sjlbkw.cn/Article/details/grxzaavwv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fktsv.cn/Article/details/gaiwxdnby.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fktsv.cn/Article/details/gxfqauggm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.epnwcf.com/Article/details/gzcuqzzbd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.yfazqb.com/Article/details/gltvbiihz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.bbcook.cn/Article/details/grnxgusoz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.sjlbkw.cn/Article/details/gzvmhftho.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/gwqhvurft.sHtML

[E02] 重复字符串
来源：http://read.share.tarul.cn/Article/details/gknqzuvgx.sHtML

Py:   "ab" * 3
来源：http://www.blog.sjlbkw.cn/Article/details/gwrwqvrpw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.tarul.cn/Article/details/gvkcoengt.sHtML

JS:   "ab".repeat(3)
来源：http://baike.vehdjk.com/Article/details/gjlrguetc.sHtML


<!-- 参考信息 -->
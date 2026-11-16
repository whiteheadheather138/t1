代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gtv.birdmap.top

Go:   return a, b
来源：http://svk.yfazqb.com

Ruby: return a, b
来源：http://uim.haohaochexian.top

C#:   return (a, b);              // ValueTuple
来源：http://iqa.epnwcf.com

[C06] 匿名函数 / lambda
来源：http://kfq.vqdsnc.cn

Py:   square = lambda x: x * x
来源：http://ncn.daxiang520.top

PHP:  $square = fn($x) => $x * $x;
来源：http://jrc.zdqjudy.top

JS:   const square = x => x * x;
来源：http://zrg.ydzc1.top

TS:   const square = (x: number): number => x * x;
来源：http://jic.yuanzhike.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yzo.ctjpmb.com

Go:   sq := func(x int) int { return x * x }
来源：http://xov.c1oappe.top

Ruby: square = ->(x) { x * x }
来源：http://pnf.c1oappe.top

C#:   Func<int, int> square = x => x * x;
来源：http://gwu.xylfe.cn

[C07] 把函数作为参数传入
来源：http://mot.daxiang520.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xzc.chenlongwang.top

PHP:  array_map("strtoupper", $arr);
来源：http://ign.yfazqb.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rhd.zdbjq.cn

TS:   arr.map(String)
来源：http://yhn.ppjwa.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kte.jianghu66.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://omd.havefunace.top

Ruby: arr.map(&:upcase)
来源：http://oyv.yj202588.top

C#:   arr.Select(s => s.ToUpper())
来源：http://flr.chenzaomai.com

[C08] 闭包
来源：http://oil.yuxming.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ctg.hfpthk.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vib.ivvv.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jjb.0kj1m.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ezq.cashguo.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qrb.zdbjq.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://atz.uphjek.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tbm.fengsongda.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pkg.yongpay.top

[C09] 递归
来源：http://zga.nanxuanxn.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ocz.snrcjt.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tkj.sxryk.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hbv.hesvh.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cfy.dianchejie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mnd.yueranfly.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ttt.mhx1999.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hab.snrcjt.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bfg.hongshengwenyu.top

[C10] 变量作用域
来源：http://vfe.ywan-chungtsiang.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bjm.shuidangran.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ihs.yuanzhike.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://uzf.sxryk.cn

TS:   同 JS
来源：http://ode.ctjpmb.com

Java: 方法内为块级作用域
来源：http://fen.fzhhl.top

Go:   花括号块级作用域
来源：http://vha.jqgfzy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dxq.sjlbkw.cn

C#:   块级作用域
来源：http://alp.fanxiaobao.xyz

[C11] 模块导入与导出
来源：http://bct.nwbrower.top

Py:   from module import func
来源：http://iya.xuetiantiany.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://nhw.daria6918.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://sqn.guowangkeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bbw.hnqzz.top

Java: import java.util.List;
来源：http://xpb.zhixingplan.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://akj.tian-w.cn

Ruby: require "json"; require_relative "./util"
来源：http://fjp.yuanzhike.top

C#:   using System.Text;
来源：http://ffx.yangfankeji.com

[C12] 立即执行函数 IIFE
来源：http://emp.yuanzhike.top

Py:   (lambda: print("run"))()
来源：http://hao.hesvh.cn

PHP:  (function () { echo "run"; })();
来源：http://oim.gogol.net.cn

JS:   (() => { console.log("run"); })();
来源：http://tml.jyoumei.cn

TS:   (() => { console.log("run"); })();
来源：http://mjh.gotoacloud.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lul.aizwys.cn

Go:   func() { fmt.Println("run") }()
来源：http://wdj.hammf.cn

Ruby: -> { puts "run" }.call
来源：http://dsr.zhaomingkeji.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://ctz.fengsongda.top

[C13] 类型声明 / 类型注解
来源：http://onk.zycfv.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://psb.hfpthk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zqq.xylfe.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://oii.ywan-chungtsiang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ijs.jlsjyb.cn

Java: int add(int a, int b) { return a + b; }
来源：http://iwc.jinyuanbaomall.cn

Go:   func add(a, b int) int
来源：http://mzf.mhx1999.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ena.jqgufenzy.top

C#:   int Add(int a, int b) => a + b;
来源：http://fll.fanxiaobao.xyz

[C14] 泛型函数
来源：http://rzq.yj20258888.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ceu.dashuyun.cn

PHP:  // 无泛型
来源：http://dwp.nanxuanxn.top

JS:   // 无泛型
来源：http://ggd.yvedp.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://atq.hammf.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://etd.zhoulong.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zcu.hysaishi.cn

Ruby: # 无泛型
来源：http://ahs.aibaodan.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xsj.haohaochexian.top

[C15] 解构 / 展开参数
来源：http://ikh.316326.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://utd.zhixingplan.top

PHP:  [$a, $b] = $pair;
来源：http://vcr.xingfuxueyuan.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ysw.xinyue.icu

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pfr.wangshuangyany.cn

Java: // 无解构
来源：http://qmx.cdnleiting.top

Go:   // 无解构
来源：http://bam.hnqzz.top

Ruby: a, b = pair
来源：http://jge.sysykeji.top

C#:   var (a, b) = pair;
来源：http://qad.tanke756.top

[C16] 函数 / 方法重载
来源：http://kgz.ehwqpu.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nfx.jqgufenzy.top

PHP:  // 无重载
来源：http://zwq.nwbrower.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://gyy.sysykeji.top

TS:   // 用联合类型或重载签名声明
来源：http://wcl.316326.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://uqu.quarkkingdee.top

Go:   // 无重载：用不同函数名
来源：http://pup.pycfn.com

Ruby: # 无重载：靠动态参数
来源：http://vzd.nanxuanxn.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://lxz.sxryk.cn

================================================================================
来源：http://nws.birdmap.top

D. 数组 / 列表 / 集合
来源：http://gbm.c1oappe.top

================================================================================
来源：http://mrg.svipenyu.cn

[D01] 创建数组 / 列表
来源：http://xpp.sweek.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://yif.ywan-chungtsiang.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://uca.zhongyouzk.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fng.zhixingplan.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://aar.yvedp.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vej.iojbl.cn

Go:   arr := []int{1, 2, 3}
来源：http://hib.chenjidiqi.icu

Ruby: arr = [1, 2, 3]
来源：http://vkc.hfpthk.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://szx.yueranfly.top

[D02] 追加元素到末尾
来源：http://ajz.kuanghao11.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ieh.tian-w.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nfp.gotoacloud.top

JS:   arr.push(4);
来源：http://ucx.xinyue.icu

TS:   arr.push(4);
来源：http://vca.smart0.xyz

Java: list.add(4);
来源：http://eay.yongpay.top

Go:   arr = append(arr, 4)
来源：http://vei.dashuyun.cn

Ruby: arr << 4; arr.push(5)
来源：http://zte.hesvh.cn

C#:   list.Add(4);
来源：http://mne.9152youxi.cn

[D03] 在指定位置插入元素
来源：http://ush.yonumen.top

Py:   arr.insert(0, 0)
来源：http://xcj.sysykeji.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rdg.xuetiantiany.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kiu.ehwqpu.com

TS:   arr.splice(0, 0, 0);
来源：http://zcl.c1oappe.top

Java: list.add(0, 0);
来源：http://mlw.smart0.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://qfz.hcnkem.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zpd.jinqigfzy.top

C#:   list.Insert(0, 0);
来源：http://pdo.ydjk.org.cn

[D04] 删除元素
来源：http://cwv.zhongyouzk.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jcq.nwbrower.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://eyk.hammf.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rgq.epnwcf.com

TS:   arr.splice(0, 1);
来源：http://kxs.hnqzz.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tzm.0kj1m.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kqp.yfazqb.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qyj.hongshengwenyu.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fqo.aibaodan.cn

[D05] 访问与修改元素
来源：http://zyz.epnwcf.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rko.xziqi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zkw.aizwys.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dct.jianghu66.top

TS:   arr[0]; arr.at(-1);
来源：http://lpt.tianlin.xyz

Java: list.get(0); list.set(0, 9);
来源：http://usy.pycfn.com

Go:   arr[0]; arr[0] = 9
来源：http://qwr.dashuyun.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wog.wangshuangyany.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dul.yangfankeji.com

[D06] 数组长度
来源：http://tfc.shanyushiyangkeji.top

Py:   len(arr)
来源：http://kkl.fktsv.cn

PHP:  count($arr);
来源：http://msj.jlsjyb.cn

JS:   arr.length
来源：http://zbr.jlsjyb.cn

TS:   arr.length
来源：http://bsz.sjlbkw.cn

Java: list.size();
来源：http://vyd.yonumen.top

Go:   len(arr)
来源：http://wjl.tarul.cn

Ruby: arr.length; arr.size
来源：http://xyg.sweek.top

C#:   list.Count;
来源：http://mlc.yonumen.top

[D07] 切片 / 取子数组
来源：http://wat.fengsongda.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://esw.shangyingyoupin.top

PHP:  array_slice($arr, 1, 3);
来源：http://tpi.xziqi.cn

JS:   arr.slice(1, 4);
来源：http://zsb.0kj1m.cn

TS:   arr.slice(1, 4);
来源：http://uyq.cdnleiting.top

Java: list.subList(1, 4);
来源：http://jjx.sweek.top

Go:   arr[1:4]
来源：http://ncj.shanyushiyangkeji.top

Ruby: arr[1, 3]
来源：http://pda.aibaodan.cn

C#:   list.GetRange(1, 3);
来源：http://ylh.nanxuanxn.top

[D08] 合并两个数组
来源：http://awh.fktsv.cn

Py:   a + b;  a.extend(b)
来源：http://ppu.quarkkingdee.top

PHP:  array_merge($a, $b);
来源：http://qun.yj202588.top

JS:   [...a, ...b];  a.concat(b);
来源：http://khi.xingfuxueyuan.xyz

TS:   [...a, ...b];
来源：http://wtx.pycfn.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lwi.ydjk.org.cn

Go:   append(a, b...)
来源：http://vjh.jyoumei.cn

Ruby: a + b;  a.concat(b)
来源：http://cfh.xuanzx.com

C#:   a.Concat(b).ToList()
来源：http://vyn.bbcook.cn

[D09] 排序（升序）
来源：http://put.jinqigfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://eyg.hesvh.cn

PHP:  sort($arr);
来源：http://ohg.jinqigufen.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wem.xinyue.icu

TS:   [...arr].sort((x, y) => x - y);
来源：http://ujf.jyoumei.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xde.xylfe.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fps.havefunace.top

Ruby: arr.sort
来源：http://tbw.bjfxy.top

C#:   list.Sort();
来源：http://pzk.aibaodan.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://uqv.cdnleiting.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://eab.tianlin.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gqr.zdqjudy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vha.yonumen.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fja.uphjek.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://eby.fanxiaobao.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tgi.redwolf501.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://shs.feifeiyinyue.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gpj.yuanzhike.top

[D11] 反转数组
来源：http://skm.ctjpmb.com

Py:   arr[::-1];  arr.reverse()
来源：http://xzx.ivvv.top

PHP:  array_reverse($arr);
来源：http://fhq.hnqzz.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wvn.svipenyu.cn

TS:   [...arr].reverse();
来源：http://ndd.daria6918.cn

Java: Collections.reverse(list);
来源：http://pcm.ppjwa.cn

Go:   slices.Reverse(arr)
来源：http://ehg.fengsongda.top

Ruby: arr.reverse
来源：http://cog.zhengqikj.top

C#:   list.Reverse();
来源：http://aml.xuanzx.com

[D12] 查找元素下标
来源：http://tky.yj202588.top

Py:   arr.index(x);  x in arr
来源：http://hrl.nanxuanxn.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kih.redwolf501.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://asf.sysykeji.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ymw.guowangkeji.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gxt.316326.xyz

Go:   slices.Index(arr, x)
来源：http://zrm.fanxiaobao.xyz

Ruby: arr.index(x)
来源：http://ngd.pycfn.com

C#:   list.IndexOf(x);
来源：http://edm.fzhhl.top

[D13] 过滤（保留满足条件的）
来源：http://ytg.pycfn.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hoe.svipenyu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ddb.mhx1999.top

JS:   arr.filter(x => x > 3)
来源：http://sra.chenzaomai.com

TS:   arr.filter(x => x > 3)
来源：http://jdg.cqqwz.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://aam.ydzc1.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jvk.ehwqpu.com

Ruby: arr.select { |x| x > 3 }
来源：http://azh.pycfn.com

C#:   list.Where(x => x > 3).ToList()
来源：http://vkb.zdbjq.cn

[D14] 映射转换（每个元素变形）
来源：http://qqa.bjfxy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vdx.yj202588.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vog.zhixingplan.top

JS:   arr.map(x => x * 2)
来源：http://mhs.sufxvd.cn

TS:   arr.map(x => x * 2)
来源：http://ubg.ppjwa.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://bvq.shanyushiyangkeji.top

Go:   // 手写循环
来源：http://bmc.xinyue.icu

Ruby: arr.map { |x| x * 2 }
来源：http://ctj.xingfuxueyuan.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://qck.svipenyu.cn

[D15] 去重
来源：http://gtr.zhixingplan.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xca.tarul.cn

PHP:  array_unique($arr);
来源：http://vqj.jianghu66.top

JS:   [...new Set(arr)]
来源：http://xqz.c1oappe.top

TS:   [...new Set(arr)]
来源：http://ofx.snrcjt.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nkn.hnqzz.top

Go:   // 用 map[T]struct{} 手写
来源：http://kse.bbcook.cn

Ruby: arr.uniq
来源：http://qgn.jinyuanbaomall.cn

C#:   list.Distinct().ToList()
来源：http://gww.xuanzx.com

[D16] 求和与平均值
来源：http://ldn.vehdjk.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tns.zhaomingkeji.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ofg.nanxinkj.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://aqv.sysykeji.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ifl.yuanzhike.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lsp.birdmap.top

Go:   // 手写循环累加
来源：http://omo.meibo888.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xzl.mhx1999.top

C#:   list.Sum();  list.Average()
来源：http://lhj.316326.xyz

[D17] 最大值与最小值
来源：http://jdd.tian-w.cn

Py:   max(arr);  min(arr)
来源：http://nse.uphjek.com

PHP:  max($arr);  min($arr);
来源：http://rik.sweek.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ukh.pycfn.com

TS:   Math.max(...arr);
来源：http://xxr.316326.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://ehg.hnxiangtu.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yme.aibaodan.cn

Ruby: arr.max;  arr.min
来源：http://xfc.9152youxi.cn

C#:   list.Max();  list.Min()
来源：http://dvn.svipenyu.cn

[D18] 扁平化嵌套数组
来源：http://lho.jyoumei.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://iwp.ydzc1.top

PHP:  array_merge(...$nested);
来源：http://qlg.ivvv.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cyp.xylfe.cn

TS:   nested.flat();
来源：http://qve.vehdjk.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mgt.xuetiantiany.cn

Go:   // 手写双层循环
来源：http://cpz.jinqigufen.top

Ruby: nested.flatten
来源：http://dsb.fktsv.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://vyw.yuanzhike.top

[D19] 按字段分组
来源：http://dfj.yangfankeji.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://enu.gzhubu.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kgq.jinqigufen.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qen.fanxiaobao.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://fxs.wangdashe.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ilq.zdqjudy.top

Go:   // 手写 map[string][]T
来源：http://zzs.zycfv.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ukl.guannengcc.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://eqz.aizwys.cn

[D20] 统计每个元素出现次数
来源：http://pbt.sufxvd.cn

Py:   Counter(arr)
来源：http://hao.wangdashe.top

PHP:  array_count_values($arr);
来源：http://zcr.feifeiyinyue.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nju.ydzc1.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dws.daria6918.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lwy.dashuyun.cn

Go:   // 手写 map[T]int
来源：http://yls.bbcook.cn

Ruby: arr.tally
来源：http://soq.cashguo.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zhf.tanke756.top

[D21] 判断是否包含某元素
来源：http://pnt.svipenyu.cn

Py:   x in arr
来源：http://ori.zhaomingkeji.xyz

PHP:  in_array($x, $arr, true);
来源：http://kuz.svipenyu.cn

JS:   arr.includes(x)
来源：http://ykm.gaohongyu789.top

TS:   arr.includes(x)
来源：http://vyq.xuetiantiany.cn

Java: list.contains(x)
来源：http://fyc.yvedp.cn

Go:   slices.Contains(arr, x)
来源：http://otq.uphjek.com

Ruby: arr.include?(x)
来源：http://qbe.smart0.xyz

C#:   list.Contains(x)
来源：http://pgs.xuetiantiany.cn

[D22] 复制数组（避免共享引用）
来源：http://twi.zdbjq.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ige.zhongyouzk.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ezp.yuxming.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://znz.xinyue.icu

TS:   [...arr];
来源：http://cbl.chenjidiqi.icu


<!-- 参考信息 -->
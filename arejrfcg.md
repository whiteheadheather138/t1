代发 wailian999

PHP:  range(0, 10, 2);
来源：http://uhy.yvedp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://big.jqgufenzy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uky.zhijiandao.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pot.aibaodan.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dhn.bbcook.cn

Ruby: (0...10).step(2).to_a
来源：http://iph.cdnleiting.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rke.xingfuxueyuan.xyz

[B12] 跳出多层循环
来源：http://bhx.sxryk.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xxq.zhijiandao.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://prq.vqdsnc.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wxi.havefunace.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ddj.daxiang520.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://foo.hnxiangtu.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jvz.nanxuanxn.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gep.jinqigfzy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://phv.gotoacloud.top

[B13] 判断是否为数字
来源：http://lxe.vqdsnc.cn

Py:   isinstance(x, (int, float))
来源：http://nur.sjlbkw.cn

PHP:  is_numeric($x)
来源：http://eoi.zhongyouzk.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://umu.jlsjyb.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qnw.vehdjk.com

Java: x instanceof Number
来源：http://bec.kuanghao11.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://oas.jinqigufen.top

Ruby: x.is_a?(Numeric)
来源：http://wfq.zhiwuduotai.top

C#:   x is int or double or decimal
来源：http://igs.hfpthk.cn

[B14] 判断值是否在集合内
来源：http://vso.jlsjyb.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ard.xuetiantiany.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dyr.52xcode.cn

JS:   [1, 2, 3].includes(x)
来源：http://cze.tanke756.top

TS:   [1, 2, 3].includes(x)
来源：http://ogd.ehwqpu.com

Java: List.of(1, 2, 3).contains(x)
来源：http://krv.cqqwz.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fmu.shanyushiyangtech.top

Ruby: [1, 2, 3].include?(x)
来源：http://uvp.xuanzx.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ozq.xylfe.cn

[B15] 布尔运算与取反
来源：http://eei.vehdjk.com

Py:   a and b or not c
来源：http://tjo.chenzaomai.com

PHP:  $a && $b || !$c
来源：http://lnc.nanxinkj.top

JS:   a && b || !c
来源：http://izn.hnqzz.top

TS:   a && b || !c
来源：http://gew.yvedp.cn

Java: a && b || !c
来源：http://dut.pengpengdd.cyou

Go:   a && b || !c
来源：http://wtj.svipenyu.cn

Ruby: a && b || !c
来源：http://ova.wangshuangyany.cn

C#:   a && b || !c
来源：http://hpa.havefunace.top

[B16] 卫语句：不满足条件提前返回
来源：http://wpd.hesvh.cn

Py:   if not data: return
来源：http://chg.cucudq.cn

PHP:  if (!$data) { return; }
来源：http://dkg.havefunace.top

JS:   if (!data) return;
来源：http://etm.hammf.cn

TS:   if (!data) return;
来源：http://jzs.zdqjudy.top

Java: if (data == null) return;
来源：http://bcv.yj20258888.top

Go:   if data == nil { return }
来源：http://nav.fanxiaobao.xyz

Ruby: return if data.nil?
来源：http://uyv.hywenlv.cn

C#:   if (data == null) return;
来源：http://wtb.sjlbkw.cn

================================================================================
来源：http://fox.cqqwz.cn

C. 函数与作用域
来源：http://fwk.xuanzx.com

================================================================================
来源：http://lal.jinqigfzy.top

[C01] 定义函数
来源：http://cna.bjfxy.top

Py:   def add(a, b): return a + b
来源：http://lil.svipenyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cff.cdnleiting.top

JS:   function add(a, b) { return a + b; }
来源：http://tnc.jinqigfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mut.hnqzz.top

Java: static int add(int a, int b) { return a + b; }
来源：http://wnp.wangshuangyany.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zto.yanxiufei.cn

Ruby: def add(a, b); a + b; end
来源：http://fzh.jiagoushi.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://afw.uphjek.com

[C02] 默认参数
来源：http://gdp.nanxuanxn.top

Py:   def greet(name="World"): return name
来源：http://jbh.pengpengdd.cyou

PHP:  function greet($name = "World") { return $name; }
来源：http://fzk.zhongyouzk.top

JS:   function greet(name = "World") { return name; }
来源：http://zhl.sweek.top

TS:   function greet(name: string = "World") { return name; }
来源：http://uhv.cucudq.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://sbq.iojbl.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lvu.birdmap.top

Ruby: def greet(name = "World") = name
来源：http://uxv.nanxuanxn.top

C#:   string Greet(string name = "World") => name;
来源：http://hza.chenjidiqi.icu

[C03] 可变参数
来源：http://iix.ppjwa.cn

Py:   def total(*args): return sum(args)
来源：http://tau.xuanzx.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bbf.jinghuilouyu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://akw.vqdsnc.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://phe.zdqjudy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ujl.havefunace.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zxk.316326.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://eqt.hnqzz.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jln.fzhhl.top

[C04] 命名参数 / 关键字参数
来源：http://jbr.zdbjq.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uoh.jiagoushi.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://del.xuanzx.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mxd.epnwcf.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bbb.andypj.xyz

Java: // 无：用 Builder 模式或 record
来源：http://lqh.ehwqpu.com

Go:   // 无：用配置结构体参数
来源：http://eqq.9152youxi.cn

Ruby: f(a: 1, b: 2)
来源：http://kat.zhijiandao.cn

C#:   f(a: 1, b: 2)
来源：http://rqk.yanxiufei.cn

[C05] 返回多个值
来源：http://rsz.wangshuangyany.cn

Py:   return a, b
来源：http://hnv.sufxvd.cn

PHP:  return [$a, $b];
来源：http://hky.ydzc1.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://fom.hysaishi.cn

TS:   return { a, b };
来源：http://ubg.sweek.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://uzt.ydzc1.top

Go:   return a, b
来源：http://bsw.yj202588.top

Ruby: return a, b
来源：http://cvu.fanxiaobao.xyz

C#:   return (a, b);              // ValueTuple
来源：http://zwf.cashguo.top

[C06] 匿名函数 / lambda
来源：http://uwu.sweek.top

Py:   square = lambda x: x * x
来源：http://xwg.ctjpmb.com

PHP:  $square = fn($x) => $x * $x;
来源：http://jia.nanxuanxn.top

JS:   const square = x => x * x;
来源：http://ewy.yj202588.top

TS:   const square = (x: number): number => x * x;
来源：http://hem.gogol.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dyj.nanxinkj.top

Go:   sq := func(x int) int { return x * x }
来源：http://ghs.cheryme.top

Ruby: square = ->(x) { x * x }
来源：http://ukt.hysaishi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://tzp.vqdsnc.cn

[C07] 把函数作为参数传入
来源：http://xfw.kuanghao11.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://iom.redwolf501.top

PHP:  array_map("strtoupper", $arr);
来源：http://mck.jiagoushi.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uuy.zhiwuduotai.top

TS:   arr.map(String)
来源：http://jqo.snrcjt.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qnx.andypj.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kof.guowangkeji.top

Ruby: arr.map(&:upcase)
来源：http://vwv.yj202588.top

C#:   arr.Select(s => s.ToUpper())
来源：http://xup.mhx1999.top

[C08] 闭包
来源：http://oha.kuanghao11.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jej.yongpay.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://oqn.hammf.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lbq.yj20258.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ehn.jinghuilouyu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nbl.epnwcf.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ojg.tianlin.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gkf.pengpengdd.cyou

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xlh.fanxiaobao.xyz

[C09] 递归
来源：http://ibe.aibaodan.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cok.xuetiantiany.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wqv.bbcook.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hmg.sweek.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xcz.quarkkingdee.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pve.hnxiangtu.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://phk.fanxiaobao.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ddf.hnqzz.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ign.guowangkeji.top

[C10] 变量作用域
来源：http://wlq.shzxlz.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nir.jinqigfzy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rby.zhengqikj.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rkc.iojbl.cn

TS:   同 JS
来源：http://qpa.jqgufenzy.top

Java: 方法内为块级作用域
来源：http://but.ctjpmb.com

Go:   花括号块级作用域
来源：http://tsj.gzhubu.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hpk.316326.xyz

C#:   块级作用域
来源：http://shd.nwbrower.top

[C11] 模块导入与导出
来源：http://vjk.0kj1m.cn

Py:   from module import func
来源：http://zxa.tianlin.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://vmh.smart0.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://cxp.sjlbkw.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hep.iojbl.cn

Java: import java.util.List;
来源：http://eup.dashuyun.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gqz.yfazqb.com

Ruby: require "json"; require_relative "./util"
来源：http://dtg.zhiwuduotai.top

C#:   using System.Text;
来源：http://baz.dashuyun.cn

[C12] 立即执行函数 IIFE
来源：http://xnb.nanxuanxn.top

Py:   (lambda: print("run"))()
来源：http://krv.svipenyu.cn

PHP:  (function () { echo "run"; })();
来源：http://rzs.ydjk.org.cn

JS:   (() => { console.log("run"); })();
来源：http://gpx.guowangkeji.top

TS:   (() => { console.log("run"); })();
来源：http://vmi.kuanghao11.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zja.feifeiyinyue.top

Go:   func() { fmt.Println("run") }()
来源：http://nbj.aizwys.cn

Ruby: -> { puts "run" }.call
来源：http://stc.xuanzx.com

C#:   // 无 IIFE：用静态构造函数
来源：http://pac.hfpthk.cn

[C13] 类型声明 / 类型注解
来源：http://uej.c1oappe.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wrl.chenlongwang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cdz.chenzaomai.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nbs.ivvv.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wjq.yongpay.top

Java: int add(int a, int b) { return a + b; }
来源：http://bod.mhx1999.top

Go:   func add(a, b int) int
来源：http://aht.aizwys.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ddn.ctjpmb.com

C#:   int Add(int a, int b) => a + b;
来源：http://qfh.ivvv.top

[C14] 泛型函数
来源：http://ncq.c1oappe.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://oii.shangyingyoupin.top

PHP:  // 无泛型
来源：http://gvo.sjlbkw.cn

JS:   // 无泛型
来源：http://ayj.dashuyun.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ess.nwbrower.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fxs.yvedp.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yra.zhongyouzk.top

Ruby: # 无泛型
来源：http://oyh.yangfankeji.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://eet.aibaodan.cn

[C15] 解构 / 展开参数
来源：http://lle.zhiwuduotai.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://usp.haohaochexian.top

PHP:  [$a, $b] = $pair;
来源：http://zuv.xinyue.icu

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://shg.nwbrower.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fje.jiagoushi.top

Java: // 无解构
来源：http://onw.guowangkeji.top

Go:   // 无解构
来源：http://hvr.sxryk.cn

Ruby: a, b = pair
来源：http://hfq.xuetiantiany.cn

C#:   var (a, b) = pair;
来源：http://dgq.zhaomingkeji.xyz

[C16] 函数 / 方法重载
来源：http://lek.tanke756.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://akl.hammf.cn

PHP:  // 无重载
来源：http://rad.yanxiufei.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://pes.sjlbkw.cn

TS:   // 用联合类型或重载签名声明
来源：http://wwq.hywenlv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rqy.zhixingplan.top

Go:   // 无重载：用不同函数名
来源：http://dzw.yuxming.cn

Ruby: # 无重载：靠动态参数
来源：http://urd.ybcxt.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://yjo.0kj1m.cn

================================================================================
来源：http://ifm.chenlongwang.top

D. 数组 / 列表 / 集合
来源：http://lte.chenzaomai.com

================================================================================
来源：http://ysb.hongshengwenyu.top

[D01] 创建数组 / 列表
来源：http://ymo.zdqjudy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://wua.jiagoushi.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yix.yj20258.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ixf.smart0.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://tkv.zhijiandao.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wbv.tian-w.cn

Go:   arr := []int{1, 2, 3}
来源：http://lrh.c1oappe.top

Ruby: arr = [1, 2, 3]
来源：http://pmj.shangyingyoupin.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://whm.hywenlv.cn

[D02] 追加元素到末尾
来源：http://hmz.wangshuangyany.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dfg.jqgfzy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xlg.tarul.cn

JS:   arr.push(4);
来源：http://rxq.pengpengdd.cyou

TS:   arr.push(4);
来源：http://csr.yueranfly.top

Java: list.add(4);
来源：http://yrx.birdmap.top

Go:   arr = append(arr, 4)
来源：http://oxc.jinyuanbaomall.cn

Ruby: arr << 4; arr.push(5)
来源：http://gam.yj202588.top

C#:   list.Add(4);
来源：http://kzh.nwbrower.top

[D03] 在指定位置插入元素
来源：http://ffl.shanyushiyangtech.top

Py:   arr.insert(0, 0)
来源：http://itz.chenzaomai.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zsu.gotoacloud.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pri.yuanzhike.top

TS:   arr.splice(0, 0, 0);
来源：http://eee.xylfe.cn

Java: list.add(0, 0);
来源：http://xuk.tarul.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jpp.0kj1m.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://alg.jianghu66.top

C#:   list.Insert(0, 0);
来源：http://ahr.iojbl.cn

[D04] 删除元素
来源：http://pkc.yuxming.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zpv.yuxming.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pxf.ybcxt.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://omi.wangdashe.top

TS:   arr.splice(0, 1);
来源：http://qdy.guowangkeji.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://oyi.feifeiyinyue.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uuu.ydjk.org.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uep.birdmap.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tzv.gogol.net.cn

[D05] 访问与修改元素
来源：http://tqf.ctjpmb.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://apa.yanxiufei.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xew.sjlbkw.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gzq.andypj.xyz

TS:   arr[0]; arr.at(-1);
来源：http://eoc.mhx1999.top

Java: list.get(0); list.set(0, 9);
来源：http://dht.jinyuanbaomall.cn

Go:   arr[0]; arr[0] = 9
来源：http://mct.ydzc1.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pqb.gogol.net.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ird.tianlin.xyz

[D06] 数组长度
来源：http://jny.daria6918.cn

Py:   len(arr)
来源：http://rvy.pengpengdd.cyou

PHP:  count($arr);
来源：http://wlu.nanxinkj.top

JS:   arr.length
来源：http://rhb.iojbl.cn

TS:   arr.length
来源：http://tsa.hcnkem.com

Java: list.size();
来源：http://pdk.guowangkeji.top

Go:   len(arr)
来源：http://kmk.hnxiangtu.top

Ruby: arr.length; arr.size
来源：http://evo.andypj.xyz

C#:   list.Count;
来源：http://prb.zhixingplan.top

[D07] 切片 / 取子数组
来源：http://kyf.andypj.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xrv.hesvh.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yfg.svipenyu.cn

JS:   arr.slice(1, 4);
来源：http://nwc.zhengqikj.top

TS:   arr.slice(1, 4);
来源：http://wxt.yj20258888.top

Java: list.subList(1, 4);
来源：http://tvr.yonumen.top

Go:   arr[1:4]
来源：http://sdq.mhx1999.top

Ruby: arr[1, 3]
来源：http://xts.meibo888.top

C#:   list.GetRange(1, 3);
来源：http://sbp.nwbrower.top

[D08] 合并两个数组
来源：http://psj.xylfe.cn

Py:   a + b;  a.extend(b)
来源：http://pez.sweek.top

PHP:  array_merge($a, $b);
来源：http://ntk.sufxvd.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://cdm.jinqigufen.top

TS:   [...a, ...b];
来源：http://cph.vqdsnc.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://uzr.dashuyun.cn

Go:   append(a, b...)
来源：http://thj.zhoulong.xyz

Ruby: a + b;  a.concat(b)
来源：http://fqn.gaohongyu789.top

C#:   a.Concat(b).ToList()
来源：http://wek.sxryk.cn

[D09] 排序（升序）
来源：http://zdt.gotoacloud.top

Py:   sorted(arr);  arr.sort()
来源：http://hre.aizwys.cn

PHP:  sort($arr);
来源：http://jhd.aizwys.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kqs.jyoumei.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://nal.ctjpmb.com

Java: Collections.sort(list);  list.sort(null);
来源：http://pyu.chenzaomai.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kta.cheryme.top

Ruby: arr.sort
来源：http://gkk.xuanzx.com

C#:   list.Sort();
来源：http://akf.chenlongwang.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://wlf.daria6918.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://doc.chenlongwang.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://olj.zdqjudy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://etf.zhoulong.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nud.daria6918.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hdl.hywenlv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gxq.hesvh.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zph.sweek.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yxr.yj20258.top

[D11] 反转数组
来源：http://ich.tanke756.top

Py:   arr[::-1];  arr.reverse()
来源：http://bvd.yfazqb.com

PHP:  array_reverse($arr);
来源：http://exa.zhixingplan.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mxl.smart0.xyz

TS:   [...arr].reverse();
来源：http://ylb.iojbl.cn

Java: Collections.reverse(list);
来源：http://ekp.redwolf501.top

Go:   slices.Reverse(arr)
来源：http://iiv.xinyue.icu

Ruby: arr.reverse
来源：http://jbv.wangdashe.top


<!-- 参考信息 -->
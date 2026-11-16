代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wge.jqgufenzy.top

Ruby: (0...10).step(2).to_a
来源：http://igh.cqqwz.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ksn.gaohongyu789.top

[B12] 跳出多层循环
来源：http://vls.quarkkingdee.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://lhx.meibo888.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://klx.hongshengwenyu.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://see.0kj1m.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vbz.ivvv.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tor.pengpengdd.cyou

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mfz.cucudq.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wqz.jlsjyb.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ueb.vehdjk.com

[B13] 判断是否为数字
来源：http://owt.gogol.net.cn

Py:   isinstance(x, (int, float))
来源：http://vpv.quarkkingdee.top

PHP:  is_numeric($x)
来源：http://crb.gotoacloud.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oak.xuanzx.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://abe.cheryme.top

Java: x instanceof Number
来源：http://bxy.chenlongwang.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bbe.wangshuangyany.cn

Ruby: x.is_a?(Numeric)
来源：http://xgo.yuanzhike.top

C#:   x is int or double or decimal
来源：http://sax.svipenyu.cn

[B14] 判断值是否在集合内
来源：http://qtp.zhengqikj.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nsv.hammf.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://omi.zhongyouzk.top

JS:   [1, 2, 3].includes(x)
来源：http://eml.sysykeji.top

TS:   [1, 2, 3].includes(x)
来源：http://cgp.sufxvd.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://cdd.hysaishi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://goi.hcnkem.com

Ruby: [1, 2, 3].include?(x)
来源：http://kxl.tian-w.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kqj.ppjwa.cn

[B15] 布尔运算与取反
来源：http://xpy.jiagoushi.top

Py:   a and b or not c
来源：http://fco.xingfuxueyuan.xyz

PHP:  $a && $b || !$c
来源：http://txh.jqgfzy.top

JS:   a && b || !c
来源：http://bsw.cheryme.top

TS:   a && b || !c
来源：http://vnb.dianchejie.cn

Java: a && b || !c
来源：http://shw.hongshengwenyu.top

Go:   a && b || !c
来源：http://uss.sysykeji.top

Ruby: a && b || !c
来源：http://qnp.hysaishi.cn

C#:   a && b || !c
来源：http://erc.shanyushiyangkeji.top

[B16] 卫语句：不满足条件提前返回
来源：http://eoz.meibo888.top

Py:   if not data: return
来源：http://sjk.kuanghao11.cn

PHP:  if (!$data) { return; }
来源：http://qad.xuetiantiany.cn

JS:   if (!data) return;
来源：http://ihn.daria6918.cn

TS:   if (!data) return;
来源：http://wie.mhx1999.top

Java: if (data == null) return;
来源：http://aej.zdqjudy.top

Go:   if data == nil { return }
来源：http://qco.zhaomingkeji.xyz

Ruby: return if data.nil?
来源：http://yzo.yonumen.top

C#:   if (data == null) return;
来源：http://olp.52xcode.cn

================================================================================
来源：http://kfb.tarul.cn

C. 函数与作用域
来源：http://dde.havefunace.top

================================================================================
来源：http://zll.havefunace.top

[C01] 定义函数
来源：http://eqb.yvedp.cn

Py:   def add(a, b): return a + b
来源：http://wzy.shzxlz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://brj.smart0.xyz

JS:   function add(a, b) { return a + b; }
来源：http://jfj.cdnleiting.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dij.ydjk.org.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://kmi.chenzaomai.com

Go:   func add(a, b int) int { return a + b }
来源：http://gef.redwolf501.top

Ruby: def add(a, b); a + b; end
来源：http://trh.fzhhl.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://owt.yfazqb.com

[C02] 默认参数
来源：http://muu.sxryk.cn

Py:   def greet(name="World"): return name
来源：http://yzl.xziqi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://gny.shanyushiyangtech.top

JS:   function greet(name = "World") { return name; }
来源：http://ufu.jinqigfzy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://lbu.9152youxi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bsz.hnqzz.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tpb.snrcjt.cn

Ruby: def greet(name = "World") = name
来源：http://woe.hysaishi.cn

C#:   string Greet(string name = "World") => name;
来源：http://woi.hnqzz.top

[C03] 可变参数
来源：http://lig.zhengqikj.top

Py:   def total(*args): return sum(args)
来源：http://yit.gotoacloud.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mei.ctjpmb.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bff.ydjk.org.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://suh.aizwys.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lej.hfpthk.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hbf.sjlbkw.cn

Ruby: def total(*nums); nums.sum; end
来源：http://avg.tianlin.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sow.zhongyouzk.top

[C04] 命名参数 / 关键字参数
来源：http://vfc.yuxming.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yjd.zhengqikj.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fki.cheryme.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hyb.jinghuilouyu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dsf.fzhhl.top

Java: // 无：用 Builder 模式或 record
来源：http://dlu.gzhubu.top

Go:   // 无：用配置结构体参数
来源：http://rvv.hcnkem.com

Ruby: f(a: 1, b: 2)
来源：http://fsa.fktsv.cn

C#:   f(a: 1, b: 2)
来源：http://ara.sjlbkw.cn

[C05] 返回多个值
来源：http://vbn.sjlbkw.cn

Py:   return a, b
来源：http://hmm.cucudq.cn

PHP:  return [$a, $b];
来源：http://qlc.fehbvm.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://apw.haohaochexian.top

TS:   return { a, b };
来源：http://wfs.chenlongwang.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://heb.uphjek.com

Go:   return a, b
来源：http://zks.jlsjyb.cn

Ruby: return a, b
来源：http://ore.yuxming.cn

C#:   return (a, b);              // ValueTuple
来源：http://lij.ivvv.top

[C06] 匿名函数 / lambda
来源：http://ass.jqgfzy.top

Py:   square = lambda x: x * x
来源：http://vsc.shangyingyoupin.top

PHP:  $square = fn($x) => $x * $x;
来源：http://oyw.hcnkem.com

JS:   const square = x => x * x;
来源：http://rmk.epnwcf.com

TS:   const square = (x: number): number => x * x;
来源：http://kpp.dashuyun.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kra.iojbl.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ouj.yanxiufei.cn

Ruby: square = ->(x) { x * x }
来源：http://lns.c1oappe.top

C#:   Func<int, int> square = x => x * x;
来源：http://gbe.nwbrower.top

[C07] 把函数作为参数传入
来源：http://ofy.bjfxy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hpi.wangdashe.top

PHP:  array_map("strtoupper", $arr);
来源：http://pze.chenzaomai.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wjy.jinqigufen.top

TS:   arr.map(String)
来源：http://qpq.feifeiyinyue.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://twb.aibaodan.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qpb.guannengcc.top

Ruby: arr.map(&:upcase)
来源：http://baa.jinqigfzy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://sxa.316326.xyz

[C08] 闭包
来源：http://xxf.zhaomingkeji.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ezs.zhaomingkeji.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rct.jiagoushi.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zje.shangyingyoupin.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://poj.tianlin.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://uzs.gogol.net.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wof.xylfe.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nos.sweek.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rav.uphjek.com

[C09] 递归
来源：http://gpq.vehdjk.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vrt.ctjpmb.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gsq.xingfuxueyuan.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://env.ydzc1.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bld.quarkkingdee.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://doh.feifeiyinyue.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vrn.jinghuilouyu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zzq.zhaomingkeji.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qlr.aibaodan.cn

[C10] 变量作用域
来源：http://lqy.yongpay.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://icf.epnwcf.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://prc.jinyuanbaomall.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cmf.aibaodan.cn

TS:   同 JS
来源：http://niq.yueranfly.top

Java: 方法内为块级作用域
来源：http://emt.wangshuangyany.cn

Go:   花括号块级作用域
来源：http://wmh.cheryme.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zev.xziqi.cn

C#:   块级作用域
来源：http://whm.jinqigufen.top

[C11] 模块导入与导出
来源：http://pre.zhiwuduotai.top

Py:   from module import func
来源：http://qgw.cashguo.top

PHP:  require "file.php";  或 use App\Service;
来源：http://inv.redwolf501.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ibm.gzhubu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lmn.bjfxy.top

Java: import java.util.List;
来源：http://spe.sysykeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bmm.guannengcc.top

Ruby: require "json"; require_relative "./util"
来源：http://bsu.ywan-chungtsiang.top

C#:   using System.Text;
来源：http://abf.hysaishi.cn

[C12] 立即执行函数 IIFE
来源：http://brk.zdbjq.cn

Py:   (lambda: print("run"))()
来源：http://hoj.meibo888.top

PHP:  (function () { echo "run"; })();
来源：http://vrl.xuanzx.com

JS:   (() => { console.log("run"); })();
来源：http://zhp.yuxming.cn

TS:   (() => { console.log("run"); })();
来源：http://rsm.mhx1999.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://aax.xuetiantiany.cn

Go:   func() { fmt.Println("run") }()
来源：http://omc.yuxming.cn

Ruby: -> { puts "run" }.call
来源：http://opg.jqgfzy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://nfl.hywenlv.cn

[C13] 类型声明 / 类型注解
来源：http://jms.hysaishi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gna.jianghu66.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lno.xuanzx.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gre.zhiwuduotai.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wbg.sysykeji.top

Java: int add(int a, int b) { return a + b; }
来源：http://mev.jianghu66.top

Go:   func add(a, b int) int
来源：http://rin.epnwcf.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ybn.chenlongwang.top

C#:   int Add(int a, int b) => a + b;
来源：http://vof.yongpay.top

[C14] 泛型函数
来源：http://zqz.fehbvm.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mks.xingfuxueyuan.xyz

PHP:  // 无泛型
来源：http://eks.hnqzz.top

JS:   // 无泛型
来源：http://aex.yj20258.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wyz.svipenyu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gir.chenlongwang.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tmq.ivvv.top

Ruby: # 无泛型
来源：http://vwr.hnqzz.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bxe.vehdjk.com

[C15] 解构 / 展开参数
来源：http://jdx.gzhubu.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://azy.zhengqikj.top

PHP:  [$a, $b] = $pair;
来源：http://txc.fehbvm.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dby.xziqi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cfa.smart0.xyz

Java: // 无解构
来源：http://xvf.hywenlv.cn

Go:   // 无解构
来源：http://xeo.quarkkingdee.top

Ruby: a, b = pair
来源：http://owd.chenjidiqi.icu

C#:   var (a, b) = pair;
来源：http://vee.52xcode.cn

[C16] 函数 / 方法重载
来源：http://ufp.cashguo.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bhg.pengpengdd.cyou

PHP:  // 无重载
来源：http://tja.hnqzz.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://yfc.ehwqpu.com

TS:   // 用联合类型或重载签名声明
来源：http://hjp.xuetiantiany.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://pxi.epnwcf.com

Go:   // 无重载：用不同函数名
来源：http://ahp.chenlongwang.top

Ruby: # 无重载：靠动态参数
来源：http://zzx.svipenyu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://edw.cashguo.top

================================================================================
来源：http://hms.ctjpmb.com

D. 数组 / 列表 / 集合
来源：http://cor.jyoumei.cn

================================================================================
来源：http://qoq.shanyushiyangkeji.top

[D01] 创建数组 / 列表
来源：http://ykl.bbcook.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://riv.fanxiaobao.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bcz.bjfxy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lot.xuanzx.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://rut.jyoumei.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ptn.cheryme.top

Go:   arr := []int{1, 2, 3}
来源：http://nch.jyoumei.cn

Ruby: arr = [1, 2, 3]
来源：http://aye.vqdsnc.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cuc.pengpengdd.cyou

[D02] 追加元素到末尾
来源：http://doc.xziqi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uzb.iojbl.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vpl.chenlongwang.top

JS:   arr.push(4);
来源：http://hve.52xcode.cn

TS:   arr.push(4);
来源：http://zdt.dianchejie.cn

Java: list.add(4);
来源：http://vdz.ydjk.org.cn

Go:   arr = append(arr, 4)
来源：http://dsz.sxryk.cn

Ruby: arr << 4; arr.push(5)
来源：http://und.hcnkem.com

C#:   list.Add(4);
来源：http://igr.dianchejie.cn

[D03] 在指定位置插入元素
来源：http://dmc.chenlongwang.top

Py:   arr.insert(0, 0)
来源：http://ukr.yueranfly.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kbx.chenzaomai.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xtv.shanyushiyangkeji.top

TS:   arr.splice(0, 0, 0);
来源：http://mxm.xinyue.icu

Java: list.add(0, 0);
来源：http://afy.iojbl.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yvi.ppjwa.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://exh.xylfe.cn

C#:   list.Insert(0, 0);
来源：http://ppd.yvedp.cn

[D04] 删除元素
来源：http://mug.ehwqpu.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gjo.yj20258888.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vku.dashuyun.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mir.gotoacloud.top

TS:   arr.splice(0, 1);
来源：http://yse.sjlbkw.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ula.xingfuxueyuan.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yyx.gogol.net.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pzn.feifeiyinyue.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ech.gzhubu.top

[D05] 访问与修改元素
来源：http://nca.fehbvm.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kvv.cdnleiting.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://txw.ybcxt.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://srm.feifeiyinyue.top

TS:   arr[0]; arr.at(-1);
来源：http://vbf.xylfe.cn

Java: list.get(0); list.set(0, 9);
来源：http://bno.fzhhl.top

Go:   arr[0]; arr[0] = 9
来源：http://zrw.havefunace.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tsg.hywenlv.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bds.ehwqpu.com

[D06] 数组长度
来源：http://iis.jinyuanbaomall.cn

Py:   len(arr)
来源：http://iqx.shanyushiyangtech.top

PHP:  count($arr);
来源：http://kqo.chenzaomai.com

JS:   arr.length
来源：http://vlg.zycfv.cn

TS:   arr.length
来源：http://gfk.sufxvd.cn

Java: list.size();
来源：http://chj.sxryk.cn

Go:   len(arr)
来源：http://dsf.xylfe.cn

Ruby: arr.length; arr.size
来源：http://ljs.jyoumei.cn

C#:   list.Count;
来源：http://lur.yj20258.top

[D07] 切片 / 取子数组
来源：http://wys.smart0.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qww.aibaodan.cn

PHP:  array_slice($arr, 1, 3);
来源：http://sso.ppjwa.cn

JS:   arr.slice(1, 4);
来源：http://def.guannengcc.top

TS:   arr.slice(1, 4);
来源：http://iod.zdbjq.cn

Java: list.subList(1, 4);
来源：http://guf.jlsjyb.cn

Go:   arr[1:4]
来源：http://pvl.xinyue.icu

Ruby: arr[1, 3]
来源：http://bml.nanxinkj.top

C#:   list.GetRange(1, 3);
来源：http://hcg.yj20258888.top

[D08] 合并两个数组
来源：http://tux.mhx1999.top

Py:   a + b;  a.extend(b)
来源：http://frt.cqqwz.cn

PHP:  array_merge($a, $b);
来源：http://ukj.fehbvm.com

JS:   [...a, ...b];  a.concat(b);
来源：http://cmn.wangdashe.top

TS:   [...a, ...b];
来源：http://zzn.xziqi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://exj.zhiwuduotai.top

Go:   append(a, b...)
来源：http://gra.gaohongyu789.top

Ruby: a + b;  a.concat(b)
来源：http://wzc.mhx1999.top

C#:   a.Concat(b).ToList()
来源：http://gcx.xuetiantiany.cn

[D09] 排序（升序）
来源：http://jmt.sufxvd.cn

Py:   sorted(arr);  arr.sort()
来源：http://rkc.guowangkeji.top

PHP:  sort($arr);
来源：http://omk.gogol.net.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jwp.ywan-chungtsiang.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://opl.guannengcc.top

Java: Collections.sort(list);  list.sort(null);
来源：http://zgh.jqgufenzy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lfy.yanxiufei.cn

Ruby: arr.sort
来源：http://etr.gaohongyu789.top

C#:   list.Sort();
来源：http://auq.aizwys.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ctg.gotoacloud.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mch.mhx1999.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gnj.hongshengwenyu.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ueq.dianchejie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wby.zhixingplan.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ick.fehbvm.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lkl.ivvv.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fea.zhengqikj.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ovj.jianghu66.top

[D11] 反转数组
来源：http://ikl.meibo888.top

Py:   arr[::-1];  arr.reverse()
来源：http://jmd.yfazqb.com

PHP:  array_reverse($arr);
来源：http://ggb.hysaishi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xew.nanxinkj.top

TS:   [...arr].reverse();
来源：http://ile.yanxiufei.cn

Java: Collections.reverse(list);
来源：http://tdu.tanke756.top

Go:   slices.Reverse(arr)
来源：http://acr.sufxvd.cn

Ruby: arr.reverse
来源：http://iqc.smart0.xyz

C#:   list.Reverse();
来源：http://bmv.shanyushiyangtech.top

[D12] 查找元素下标
来源：http://ugl.hnqzz.top

Py:   arr.index(x);  x in arr
来源：http://aas.hnqzz.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://njp.iojbl.cn


<!-- 参考信息 -->
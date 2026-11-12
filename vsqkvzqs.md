代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://whl.c1oappe.top

Ruby: (0...10).step(2).to_a
来源：http://olk.tian-w.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cxs.yanxiufei.cn

[B12] 跳出多层循环
来源：http://nwn.birdmap.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ljn.cqqwz.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gwy.hnqzz.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bpa.sjlbkw.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bhh.52xcode.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mpd.jiagoushi.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xdb.yj20258888.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tye.yanxiufei.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tdj.yuxming.cn

[B13] 判断是否为数字
来源：http://moa.dashuyun.cn

Py:   isinstance(x, (int, float))
来源：http://yud.zhoulong.xyz

PHP:  is_numeric($x)
来源：http://tmu.sjlbkw.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://eli.gzhubu.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://umk.pycfn.com

Java: x instanceof Number
来源：http://lwt.xinyue.icu

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://phs.yuxming.cn

Ruby: x.is_a?(Numeric)
来源：http://nwz.sxryk.cn

C#:   x is int or double or decimal
来源：http://pmt.yueranfly.top

[B14] 判断值是否在集合内
来源：http://qbe.cheryme.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tio.shangyingyoupin.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://btb.ybcxt.top

JS:   [1, 2, 3].includes(x)
来源：http://iej.gogol.net.cn

TS:   [1, 2, 3].includes(x)
来源：http://mqr.xuetiantiany.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xtk.guowangkeji.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yfa.vehdjk.com

Ruby: [1, 2, 3].include?(x)
来源：http://baz.feifeiyinyue.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fmu.bbcook.cn

[B15] 布尔运算与取反
来源：http://rdx.fengsongda.top

Py:   a and b or not c
来源：http://mjg.zhaomingkeji.xyz

PHP:  $a && $b || !$c
来源：http://sqz.yangfankeji.com

JS:   a && b || !c
来源：http://ryb.yj202588.top

TS:   a && b || !c
来源：http://cxu.nanxinkj.top

Java: a && b || !c
来源：http://zqk.316326.xyz

Go:   a && b || !c
来源：http://mpo.iojbl.cn

Ruby: a && b || !c
来源：http://zew.hcnkem.com

C#:   a && b || !c
来源：http://pri.chenlongwang.top

[B16] 卫语句：不满足条件提前返回
来源：http://sxe.kuanghao11.cn

Py:   if not data: return
来源：http://swh.ctjpmb.com

PHP:  if (!$data) { return; }
来源：http://qpn.uphjek.com

JS:   if (!data) return;
来源：http://cck.xuanzx.com

TS:   if (!data) return;
来源：http://ayp.dashuyun.cn

Java: if (data == null) return;
来源：http://bum.guowangkeji.top

Go:   if data == nil { return }
来源：http://nkn.ydjk.org.cn

Ruby: return if data.nil?
来源：http://ozk.fanxiaobao.xyz

C#:   if (data == null) return;
来源：http://vbv.feifeiyinyue.top

================================================================================
来源：http://txf.yvedp.cn

C. 函数与作用域
来源：http://rpi.xziqi.cn

================================================================================
来源：http://paa.jqgufenzy.top

[C01] 定义函数
来源：http://sos.tian-w.cn

Py:   def add(a, b): return a + b
来源：http://xjv.yvedp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://spd.gaohongyu789.top

JS:   function add(a, b) { return a + b; }
来源：http://oun.sweek.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://opc.xinyue.icu

Java: static int add(int a, int b) { return a + b; }
来源：http://mrl.cashguo.top

Go:   func add(a, b int) int { return a + b }
来源：http://bqw.zhoulong.xyz

Ruby: def add(a, b); a + b; end
来源：http://lnn.sjlbkw.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nxx.tianlin.xyz

[C02] 默认参数
来源：http://qua.shanyushiyangkeji.top

Py:   def greet(name="World"): return name
来源：http://xjf.hammf.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://wgt.yuanzhike.top

JS:   function greet(name = "World") { return name; }
来源：http://wgg.sysykeji.top

TS:   function greet(name: string = "World") { return name; }
来源：http://noq.svipenyu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cvn.sysykeji.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hkb.zhijiandao.cn

Ruby: def greet(name = "World") = name
来源：http://haj.cheryme.top

C#:   string Greet(string name = "World") => name;
来源：http://bol.shuidangran.top

[C03] 可变参数
来源：http://tbp.birdmap.top

Py:   def total(*args): return sum(args)
来源：http://teo.sweek.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zsr.wangshuangyany.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bep.redwolf501.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gio.shanyushiyangkeji.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://uew.kuanghao11.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zbd.hcnkem.com

Ruby: def total(*nums); nums.sum; end
来源：http://fnf.feifeiyinyue.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://djo.hesvh.cn

[C04] 命名参数 / 关键字参数
来源：http://bar.bbcook.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lma.zhijiandao.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://acj.gaohongyu789.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mcj.yj202588.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vcx.nanxuanxn.top

Java: // 无：用 Builder 模式或 record
来源：http://cuw.hysaishi.cn

Go:   // 无：用配置结构体参数
来源：http://xyv.bbcook.cn

Ruby: f(a: 1, b: 2)
来源：http://beg.svipenyu.cn

C#:   f(a: 1, b: 2)
来源：http://nnj.bjfxy.top

[C05] 返回多个值
来源：http://tqr.kuanghao11.cn

Py:   return a, b
来源：http://fii.ivvv.top

PHP:  return [$a, $b];
来源：http://ucm.dashuyun.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://was.zhongyouzk.top

TS:   return { a, b };
来源：http://kle.0kj1m.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://van.haohaochexian.top

Go:   return a, b
来源：http://dir.ywan-chungtsiang.top

Ruby: return a, b
来源：http://ndm.uphjek.com

C#:   return (a, b);              // ValueTuple
来源：http://eqe.chenzaomai.com

[C06] 匿名函数 / lambda
来源：http://ofi.gaohongyu789.top

Py:   square = lambda x: x * x
来源：http://rro.aibaodan.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://tfy.jiagoushi.top

JS:   const square = x => x * x;
来源：http://ade.sufxvd.cn

TS:   const square = (x: number): number => x * x;
来源：http://rdp.yj202588.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dck.tarul.cn

Go:   sq := func(x int) int { return x * x }
来源：http://agp.cdnleiting.top

Ruby: square = ->(x) { x * x }
来源：http://jlv.hammf.cn

C#:   Func<int, int> square = x => x * x;
来源：http://mrf.sjlbkw.cn

[C07] 把函数作为参数传入
来源：http://ksv.ppjwa.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nee.zhengqikj.top

PHP:  array_map("strtoupper", $arr);
来源：http://jem.andypj.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ajt.gzhubu.top

TS:   arr.map(String)
来源：http://snh.pengpengdd.cyou

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ezb.shuidangran.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://myc.yj20258888.top

Ruby: arr.map(&:upcase)
来源：http://ffx.jlsjyb.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cgg.bjfxy.top

[C08] 闭包
来源：http://vxe.shzxlz.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fkh.aibaodan.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jpk.shuidangran.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jxq.sufxvd.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nna.yonumen.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hon.xinyue.icu

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://agz.sufxvd.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://oew.zhiwuduotai.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ddv.jinghuilouyu.cn

[C09] 递归
来源：http://jtn.dashuyun.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://plx.yfazqb.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rrv.ctjpmb.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://omq.316326.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://trs.gaohongyu789.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xmy.feifeiyinyue.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://eww.meibo888.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vdd.tarul.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fos.jqgfzy.top

[C10] 变量作用域
来源：http://owz.nanxinkj.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gjf.jinyuanbaomall.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cut.svipenyu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rhu.yvedp.cn

TS:   同 JS
来源：http://elq.sjlbkw.cn

Java: 方法内为块级作用域
来源：http://xvr.bbcook.cn

Go:   花括号块级作用域
来源：http://fwl.yueranfly.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://scc.yuxming.cn

C#:   块级作用域
来源：http://hlg.jianghu66.top

[C11] 模块导入与导出
来源：http://iqy.xuetiantiany.cn

Py:   from module import func
来源：http://vss.meibo888.top

PHP:  require "file.php";  或 use App\Service;
来源：http://krj.jqgufenzy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ney.bbcook.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bkf.52xcode.cn

Java: import java.util.List;
来源：http://igz.dianchejie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wjl.cheryme.top

Ruby: require "json"; require_relative "./util"
来源：http://qyq.feifeiyinyue.top

C#:   using System.Text;
来源：http://dum.nanxuanxn.top

[C12] 立即执行函数 IIFE
来源：http://idr.zhaomingkeji.xyz

Py:   (lambda: print("run"))()
来源：http://qlt.ywan-chungtsiang.top

PHP:  (function () { echo "run"; })();
来源：http://ubb.yanxiufei.cn

JS:   (() => { console.log("run"); })();
来源：http://lre.zhengqikj.top

TS:   (() => { console.log("run"); })();
来源：http://gyi.fengsongda.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wdv.ctjpmb.com

Go:   func() { fmt.Println("run") }()
来源：http://ylq.ivvv.top

Ruby: -> { puts "run" }.call
来源：http://ybx.wangdashe.top

C#:   // 无 IIFE：用静态构造函数
来源：http://evw.gogol.net.cn

[C13] 类型声明 / 类型注解
来源：http://sey.xingfuxueyuan.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xmx.sweek.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fuc.jlsjyb.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pye.zhoulong.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dqd.yvedp.cn

Java: int add(int a, int b) { return a + b; }
来源：http://uuw.guowangkeji.top

Go:   func add(a, b int) int
来源：http://pcl.jianghu66.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jsq.kuanghao11.cn

C#:   int Add(int a, int b) => a + b;
来源：http://yue.fktsv.cn

[C14] 泛型函数
来源：http://pvp.pycfn.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gyl.yuanzhike.top

PHP:  // 无泛型
来源：http://evd.epnwcf.com

JS:   // 无泛型
来源：http://xun.redwolf501.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://maz.fzhhl.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wmb.cashguo.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://eas.dashuyun.cn

Ruby: # 无泛型
来源：http://egv.yongpay.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pxn.hnqzz.top

[C15] 解构 / 展开参数
来源：http://qyu.ivvv.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zze.zhaomingkeji.xyz

PHP:  [$a, $b] = $pair;
来源：http://nzt.gzhubu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nwg.ppjwa.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tjf.epnwcf.com

Java: // 无解构
来源：http://rtt.cqqwz.cn

Go:   // 无解构
来源：http://oqm.chenjidiqi.icu

Ruby: a, b = pair
来源：http://pwn.iojbl.cn

C#:   var (a, b) = pair;
来源：http://tgu.xylfe.cn

[C16] 函数 / 方法重载
来源：http://arx.shanyushiyangtech.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hvg.sysykeji.top

PHP:  // 无重载
来源：http://gvg.yonumen.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://xmf.tanke756.top

TS:   // 用联合类型或重载签名声明
来源：http://gyz.xingfuxueyuan.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://pyy.0kj1m.cn

Go:   // 无重载：用不同函数名
来源：http://unm.dianchejie.cn

Ruby: # 无重载：靠动态参数
来源：http://mfj.smart0.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://psy.jiagoushi.top

================================================================================
来源：http://tfe.cdnleiting.top

D. 数组 / 列表 / 集合
来源：http://bfd.ybcxt.top

================================================================================
来源：http://ezq.vqdsnc.cn

[D01] 创建数组 / 列表
来源：http://pna.zhoulong.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://wjt.jinqigfzy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bwe.jlsjyb.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://oxa.jqgufenzy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ten.chenjidiqi.icu

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vcj.jinqigufen.top

Go:   arr := []int{1, 2, 3}
来源：http://rpn.jinqigufen.top

Ruby: arr = [1, 2, 3]
来源：http://aoa.yj20258.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bsw.wangshuangyany.cn

[D02] 追加元素到末尾
来源：http://jkz.meibo888.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hvx.0kj1m.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ych.jqgufenzy.top

JS:   arr.push(4);
来源：http://obg.kuanghao11.cn

TS:   arr.push(4);
来源：http://fkg.chenzaomai.com

Java: list.add(4);
来源：http://vvg.0kj1m.cn

Go:   arr = append(arr, 4)
来源：http://doy.feifeiyinyue.top

Ruby: arr << 4; arr.push(5)
来源：http://zjt.kuanghao11.cn

C#:   list.Add(4);
来源：http://rvv.svipenyu.cn

[D03] 在指定位置插入元素
来源：http://swi.cdnleiting.top

Py:   arr.insert(0, 0)
来源：http://jjd.nanxinkj.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ziy.ywan-chungtsiang.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jow.hysaishi.cn

TS:   arr.splice(0, 0, 0);
来源：http://xje.iojbl.cn

Java: list.add(0, 0);
来源：http://srl.0kj1m.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ahk.smart0.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hzq.jianghu66.top

C#:   list.Insert(0, 0);
来源：http://xea.zhengqikj.top

[D04] 删除元素
来源：http://tsi.vqdsnc.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ysj.yuanzhike.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bvg.tanke756.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jqf.dashuyun.cn

TS:   arr.splice(0, 1);
来源：http://ydh.xziqi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bnt.zhengqikj.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://udx.jinghuilouyu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vom.yonumen.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bcu.yj20258888.top

[D05] 访问与修改元素
来源：http://rrz.shanyushiyangtech.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://spw.andypj.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kxp.daria6918.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://oeh.shanyushiyangkeji.top

TS:   arr[0]; arr.at(-1);
来源：http://jcq.jinyuanbaomall.cn

Java: list.get(0); list.set(0, 9);
来源：http://xpw.zdbjq.cn

Go:   arr[0]; arr[0] = 9
来源：http://vul.tanke756.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://etg.epnwcf.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rsz.havefunace.top

[D06] 数组长度
来源：http://zzy.fzhhl.top

Py:   len(arr)
来源：http://fek.zhaomingkeji.xyz

PHP:  count($arr);
来源：http://phv.ppjwa.cn

JS:   arr.length
来源：http://tax.shanyushiyangkeji.top

TS:   arr.length
来源：http://zti.hesvh.cn

Java: list.size();
来源：http://bav.cqqwz.cn

Go:   len(arr)
来源：http://rfx.jianghu66.top

Ruby: arr.length; arr.size
来源：http://uhk.birdmap.top

C#:   list.Count;
来源：http://mxt.tianlin.xyz

[D07] 切片 / 取子数组
来源：http://zkp.yuanzhike.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pap.zhengqikj.top

PHP:  array_slice($arr, 1, 3);
来源：http://bho.hesvh.cn

JS:   arr.slice(1, 4);
来源：http://zqh.aizwys.cn

TS:   arr.slice(1, 4);
来源：http://lbj.zdqjudy.top

Java: list.subList(1, 4);
来源：http://usn.dashuyun.cn

Go:   arr[1:4]
来源：http://owo.chenlongwang.top

Ruby: arr[1, 3]
来源：http://dkr.meibo888.top

C#:   list.GetRange(1, 3);
来源：http://pny.ivvv.top

[D08] 合并两个数组
来源：http://xfg.tanke756.top

Py:   a + b;  a.extend(b)
来源：http://pyu.hywenlv.cn

PHP:  array_merge($a, $b);
来源：http://dzy.yj20258.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ybe.ppjwa.cn

TS:   [...a, ...b];
来源：http://uhb.jinqigfzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dvq.jinqigufen.top

Go:   append(a, b...)
来源：http://kqp.ppjwa.cn

Ruby: a + b;  a.concat(b)
来源：http://dec.sxryk.cn

C#:   a.Concat(b).ToList()
来源：http://wjv.hesvh.cn

[D09] 排序（升序）
来源：http://dkd.gaohongyu789.top

Py:   sorted(arr);  arr.sort()
来源：http://vbb.hnxiangtu.top

PHP:  sort($arr);
来源：http://wfs.sjlbkw.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://oci.meibo888.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://kdl.shangyingyoupin.top

Java: Collections.sort(list);  list.sort(null);
来源：http://rpv.zhoulong.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qcg.sjlbkw.cn

Ruby: arr.sort
来源：http://nar.pengpengdd.cyou

C#:   list.Sort();
来源：http://xyy.fzhhl.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://mwd.andypj.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yfh.yanxiufei.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vbi.tarul.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://haz.dianchejie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qqm.fktsv.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lkl.zdbjq.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://njx.zhongyouzk.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lxg.shangyingyoupin.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mnx.zhoulong.xyz

[D11] 反转数组
来源：http://epn.gaohongyu789.top

Py:   arr[::-1];  arr.reverse()
来源：http://bbo.xziqi.cn

PHP:  array_reverse($arr);
来源：http://qti.ivvv.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vhx.cucudq.cn

TS:   [...arr].reverse();
来源：http://ynk.haohaochexian.top

Java: Collections.reverse(list);
来源：http://xqm.316326.xyz

Go:   slices.Reverse(arr)
来源：http://noh.yonumen.top

Ruby: arr.reverse
来源：http://tox.aizwys.cn

C#:   list.Reverse();
来源：http://axv.yonumen.top

[D12] 查找元素下标
来源：http://dic.zycfv.cn

Py:   arr.index(x);  x in arr
来源：http://vih.nanxuanxn.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bco.chenzaomai.com


<!-- 参考信息 -->
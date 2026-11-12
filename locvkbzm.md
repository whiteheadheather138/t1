代发 wailian999

PHP:  range(0, 10, 2);
来源：http://bvq.aizwys.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dtx.0kj1m.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tgs.pycfn.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://moq.sysykeji.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bwu.zdqjudy.top

Ruby: (0...10).step(2).to_a
来源：http://zkk.cashguo.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hqd.ivvv.top

[B12] 跳出多层循环
来源：http://lhr.tanke756.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://bnh.haohaochexian.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://mbs.shuidangran.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wlf.zhiwuduotai.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://guh.hysaishi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://eav.smart0.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ctz.jinghuilouyu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fax.dashuyun.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fnl.fehbvm.com

[B13] 判断是否为数字
来源：http://lwr.jiagoushi.top

Py:   isinstance(x, (int, float))
来源：http://kyo.ppjwa.cn

PHP:  is_numeric($x)
来源：http://ngo.xuanzx.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rmy.dianchejie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cpl.yangfankeji.com

Java: x instanceof Number
来源：http://vae.dashuyun.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pso.daria6918.cn

Ruby: x.is_a?(Numeric)
来源：http://pxt.iojbl.cn

C#:   x is int or double or decimal
来源：http://tiq.yfazqb.com

[B14] 判断值是否在集合内
来源：http://hnk.cucudq.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ckz.mhx1999.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://raa.shanyushiyangtech.top

JS:   [1, 2, 3].includes(x)
来源：http://rks.hnxiangtu.top

TS:   [1, 2, 3].includes(x)
来源：http://xfz.sufxvd.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vrd.zdqjudy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://usf.cashguo.top

Ruby: [1, 2, 3].include?(x)
来源：http://ehg.nwbrower.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xiy.cashguo.top

[B15] 布尔运算与取反
来源：http://zty.hnqzz.top

Py:   a and b or not c
来源：http://fks.fengsongda.top

PHP:  $a && $b || !$c
来源：http://dvm.bbcook.cn

JS:   a && b || !c
来源：http://xss.zhoulong.xyz

TS:   a && b || !c
来源：http://jrw.zhoulong.xyz

Java: a && b || !c
来源：http://zlb.cheryme.top

Go:   a && b || !c
来源：http://lfr.kuanghao11.cn

Ruby: a && b || !c
来源：http://drx.zdqjudy.top

C#:   a && b || !c
来源：http://uyg.hywenlv.cn

[B16] 卫语句：不满足条件提前返回
来源：http://eev.uphjek.com

Py:   if not data: return
来源：http://mpj.fktsv.cn

PHP:  if (!$data) { return; }
来源：http://kqr.shangyingyoupin.top

JS:   if (!data) return;
来源：http://auj.tian-w.cn

TS:   if (!data) return;
来源：http://sea.yueranfly.top

Java: if (data == null) return;
来源：http://bxk.vehdjk.com

Go:   if data == nil { return }
来源：http://jyo.dashuyun.cn

Ruby: return if data.nil?
来源：http://weh.hfpthk.cn

C#:   if (data == null) return;
来源：http://iwf.smart0.xyz

================================================================================
来源：http://dzh.daria6918.cn

C. 函数与作用域
来源：http://xte.feifeiyinyue.top

================================================================================
来源：http://cvb.jiagoushi.top

[C01] 定义函数
来源：http://xdn.yonumen.top

Py:   def add(a, b): return a + b
来源：http://xzz.tarul.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://akn.sweek.top

JS:   function add(a, b) { return a + b; }
来源：http://hfx.cashguo.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cdn.chenzaomai.com

Java: static int add(int a, int b) { return a + b; }
来源：http://aft.svipenyu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hby.zycfv.cn

Ruby: def add(a, b); a + b; end
来源：http://vhj.chenlongwang.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ckv.yangfankeji.com

[C02] 默认参数
来源：http://ehg.fzhhl.top

Py:   def greet(name="World"): return name
来源：http://jov.xingfuxueyuan.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://msv.snrcjt.cn

JS:   function greet(name = "World") { return name; }
来源：http://iqe.shzxlz.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rxz.quarkkingdee.top

Java: // 无默认参数：方法重载或 Optional
来源：http://tdz.sweek.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xul.jinqigufen.top

Ruby: def greet(name = "World") = name
来源：http://jdc.yuxming.cn

C#:   string Greet(string name = "World") => name;
来源：http://msj.zhijiandao.cn

[C03] 可变参数
来源：http://ylm.yangfankeji.com

Py:   def total(*args): return sum(args)
来源：http://gle.guowangkeji.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://djz.svipenyu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dxv.smart0.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mil.zhixingplan.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vzm.gotoacloud.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hef.cqqwz.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qwq.shzxlz.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cnl.ivvv.top

[C04] 命名参数 / 关键字参数
来源：http://ugs.jinghuilouyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rsr.shangyingyoupin.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bgx.cheryme.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vcu.quarkkingdee.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kgj.9152youxi.cn

Java: // 无：用 Builder 模式或 record
来源：http://qsy.pengpengdd.cyou

Go:   // 无：用配置结构体参数
来源：http://ysm.cucudq.cn

Ruby: f(a: 1, b: 2)
来源：http://cma.dianchejie.cn

C#:   f(a: 1, b: 2)
来源：http://edk.xziqi.cn

[C05] 返回多个值
来源：http://tve.guowangkeji.top

Py:   return a, b
来源：http://inh.hammf.cn

PHP:  return [$a, $b];
来源：http://iym.0kj1m.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://lbj.ehwqpu.com

TS:   return { a, b };
来源：http://pvu.tianlin.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pbt.chenzaomai.com

Go:   return a, b
来源：http://kyj.shuidangran.top

Ruby: return a, b
来源：http://lgq.tian-w.cn

C#:   return (a, b);              // ValueTuple
来源：http://hzr.daria6918.cn

[C06] 匿名函数 / lambda
来源：http://wjq.uphjek.com

Py:   square = lambda x: x * x
来源：http://jqh.chenjidiqi.icu

PHP:  $square = fn($x) => $x * $x;
来源：http://nfh.ivvv.top

JS:   const square = x => x * x;
来源：http://hfw.wangdashe.top

TS:   const square = (x: number): number => x * x;
来源：http://gbv.jqgfzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lrg.fanxiaobao.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://okp.0kj1m.cn

Ruby: square = ->(x) { x * x }
来源：http://jyx.hcnkem.com

C#:   Func<int, int> square = x => x * x;
来源：http://hyq.zycfv.cn

[C07] 把函数作为参数传入
来源：http://xup.hammf.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ewz.guowangkeji.top

PHP:  array_map("strtoupper", $arr);
来源：http://lju.ydjk.org.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://igq.zdqjudy.top

TS:   arr.map(String)
来源：http://fha.bbcook.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ubn.xingfuxueyuan.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gmi.birdmap.top

Ruby: arr.map(&:upcase)
来源：http://xyt.zdqjudy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://edr.shanyushiyangkeji.top

[C08] 闭包
来源：http://jaj.vehdjk.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zjf.jqgufenzy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bjk.bbcook.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uve.yongpay.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vxl.yj202588.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gca.jinghuilouyu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vcl.yongpay.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rzp.guowangkeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wie.fengsongda.top

[C09] 递归
来源：http://eob.vehdjk.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xbk.guowangkeji.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bxn.ydzc1.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uzw.jlsjyb.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ajr.cheryme.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qcg.tian-w.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mgk.hesvh.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zoz.jiagoushi.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tnn.quarkkingdee.top

[C10] 变量作用域
来源：http://pmh.wangshuangyany.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qaf.52xcode.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://byb.yvedp.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rfr.ywan-chungtsiang.top

TS:   同 JS
来源：http://aji.hnqzz.top

Java: 方法内为块级作用域
来源：http://gye.nanxuanxn.top

Go:   花括号块级作用域
来源：http://ccc.redwolf501.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fjm.xuetiantiany.cn

C#:   块级作用域
来源：http://muh.jinghuilouyu.cn

[C11] 模块导入与导出
来源：http://mab.bbcook.cn

Py:   from module import func
来源：http://gbn.yj20258.top

PHP:  require "file.php";  或 use App\Service;
来源：http://qmk.mhx1999.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://kse.jiagoushi.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cfg.zhoulong.xyz

Java: import java.util.List;
来源：http://uys.redwolf501.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rfu.cdnleiting.top

Ruby: require "json"; require_relative "./util"
来源：http://jri.sysykeji.top

C#:   using System.Text;
来源：http://nyy.cashguo.top

[C12] 立即执行函数 IIFE
来源：http://nyv.yangfankeji.com

Py:   (lambda: print("run"))()
来源：http://ifu.gzhubu.top

PHP:  (function () { echo "run"; })();
来源：http://mwn.yuxming.cn

JS:   (() => { console.log("run"); })();
来源：http://zha.jyoumei.cn

TS:   (() => { console.log("run"); })();
来源：http://uix.chenzaomai.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ldk.yj20258.top

Go:   func() { fmt.Println("run") }()
来源：http://dwc.shangyingyoupin.top

Ruby: -> { puts "run" }.call
来源：http://jak.fzhhl.top

C#:   // 无 IIFE：用静态构造函数
来源：http://bsi.gogol.net.cn

[C13] 类型声明 / 类型注解
来源：http://vmx.sysykeji.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jks.c1oappe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hiz.ivvv.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kes.pycfn.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ppr.jlsjyb.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mio.redwolf501.top

Go:   func add(a, b int) int
来源：http://rol.ctjpmb.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tue.svipenyu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vmb.316326.xyz

[C14] 泛型函数
来源：http://bax.cucudq.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rml.ydzc1.top

PHP:  // 无泛型
来源：http://lql.fzhhl.top

JS:   // 无泛型
来源：http://ukf.hnqzz.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gpl.epnwcf.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cgy.redwolf501.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pha.fengsongda.top

Ruby: # 无泛型
来源：http://koz.vqdsnc.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pih.hammf.cn

[C15] 解构 / 展开参数
来源：http://jrb.shanyushiyangkeji.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dxq.cdnleiting.top

PHP:  [$a, $b] = $pair;
来源：http://gdq.sysykeji.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jxe.shanyushiyangkeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kjj.c1oappe.top

Java: // 无解构
来源：http://wrp.cheryme.top

Go:   // 无解构
来源：http://gzb.hywenlv.cn

Ruby: a, b = pair
来源：http://lja.yfazqb.com

C#:   var (a, b) = pair;
来源：http://pre.bbcook.cn

[C16] 函数 / 方法重载
来源：http://vtr.hnxiangtu.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zcy.jianghu66.top

PHP:  // 无重载
来源：http://pdr.gotoacloud.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://iry.hnxiangtu.top

TS:   // 用联合类型或重载签名声明
来源：http://dlg.bbcook.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://sqf.hammf.cn

Go:   // 无重载：用不同函数名
来源：http://pgo.dianchejie.cn

Ruby: # 无重载：靠动态参数
来源：http://vnd.tianlin.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://bci.zhengqikj.top

================================================================================
来源：http://jzi.svipenyu.cn

D. 数组 / 列表 / 集合
来源：http://qap.fzhhl.top

================================================================================
来源：http://fvp.yanxiufei.cn

[D01] 创建数组 / 列表
来源：http://lsa.nanxinkj.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://kgc.hesvh.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zpq.yuanzhike.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ang.haohaochexian.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://hmz.gotoacloud.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cvh.zhaomingkeji.xyz

Go:   arr := []int{1, 2, 3}
来源：http://zpa.mhx1999.top

Ruby: arr = [1, 2, 3]
来源：http://bml.jinghuilouyu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://drd.ydzc1.top

[D02] 追加元素到末尾
来源：http://hua.fengsongda.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bky.sxryk.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bfd.9152youxi.cn

JS:   arr.push(4);
来源：http://hgo.zhengqikj.top

TS:   arr.push(4);
来源：http://vhy.redwolf501.top

Java: list.add(4);
来源：http://uin.gaohongyu789.top

Go:   arr = append(arr, 4)
来源：http://qqv.jianghu66.top

Ruby: arr << 4; arr.push(5)
来源：http://hcz.yanxiufei.cn

C#:   list.Add(4);
来源：http://lgt.tian-w.cn

[D03] 在指定位置插入元素
来源：http://zur.cqqwz.cn

Py:   arr.insert(0, 0)
来源：http://asn.zhiwuduotai.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tpa.xingfuxueyuan.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qab.wangdashe.top

TS:   arr.splice(0, 0, 0);
来源：http://tfb.hammf.cn

Java: list.add(0, 0);
来源：http://dzd.fzhhl.top

Go:   arr = append([]int{0}, arr...)
来源：http://fvw.shangyingyoupin.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://clg.yongpay.top

C#:   list.Insert(0, 0);
来源：http://hpc.zhoulong.xyz

[D04] 删除元素
来源：http://edx.dashuyun.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dzi.fengsongda.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ams.0kj1m.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vrp.xuetiantiany.cn

TS:   arr.splice(0, 1);
来源：http://gjj.daria6918.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mmh.shangyingyoupin.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ehg.meibo888.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zvm.fanxiaobao.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ldq.ydjk.org.cn

[D05] 访问与修改元素
来源：http://qah.chenlongwang.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jve.bbcook.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ngm.fzhhl.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bzu.pycfn.com

TS:   arr[0]; arr.at(-1);
来源：http://kvs.chenzaomai.com

Java: list.get(0); list.set(0, 9);
来源：http://dzc.jlsjyb.cn

Go:   arr[0]; arr[0] = 9
来源：http://vcv.jqgfzy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wyr.ywan-chungtsiang.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jrb.fktsv.cn

[D06] 数组长度
来源：http://nxw.cdnleiting.top

Py:   len(arr)
来源：http://vlf.snrcjt.cn

PHP:  count($arr);
来源：http://rry.snrcjt.cn

JS:   arr.length
来源：http://qrl.fehbvm.com

TS:   arr.length
来源：http://pnm.jinghuilouyu.cn

Java: list.size();
来源：http://pnp.sufxvd.cn

Go:   len(arr)
来源：http://kxr.xinyue.icu

Ruby: arr.length; arr.size
来源：http://tgy.jinghuilouyu.cn

C#:   list.Count;
来源：http://sih.xziqi.cn

[D07] 切片 / 取子数组
来源：http://xaw.52xcode.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://btw.c1oappe.top

PHP:  array_slice($arr, 1, 3);
来源：http://ufo.zhiwuduotai.top

JS:   arr.slice(1, 4);
来源：http://nbi.sxryk.cn

TS:   arr.slice(1, 4);
来源：http://eye.hnxiangtu.top

Java: list.subList(1, 4);
来源：http://txk.zhoulong.xyz

Go:   arr[1:4]
来源：http://zcc.tarul.cn

Ruby: arr[1, 3]
来源：http://ury.ppjwa.cn

C#:   list.GetRange(1, 3);
来源：http://mwq.yj20258.top

[D08] 合并两个数组
来源：http://cta.epnwcf.com

Py:   a + b;  a.extend(b)
来源：http://ozk.daxiang520.top

PHP:  array_merge($a, $b);
来源：http://blj.ybcxt.top

JS:   [...a, ...b];  a.concat(b);
来源：http://hgc.ehwqpu.com

TS:   [...a, ...b];
来源：http://qst.fanxiaobao.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bwr.wangdashe.top

Go:   append(a, b...)
来源：http://eeg.bjfxy.top

Ruby: a + b;  a.concat(b)
来源：http://tem.316326.xyz

C#:   a.Concat(b).ToList()
来源：http://ctr.yuxming.cn

[D09] 排序（升序）
来源：http://mxy.jlsjyb.cn

Py:   sorted(arr);  arr.sort()
来源：http://uau.0kj1m.cn

PHP:  sort($arr);
来源：http://qrv.fktsv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qlk.pengpengdd.cyou

TS:   [...arr].sort((x, y) => x - y);
来源：http://lzt.xziqi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hdm.ivvv.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tew.shangyingyoupin.top

Ruby: arr.sort
来源：http://pxn.havefunace.top

C#:   list.Sort();
来源：http://hiv.quarkkingdee.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://xki.52xcode.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wrt.zhaomingkeji.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gar.zhaomingkeji.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yde.xylfe.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ldt.yj202588.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ohl.jinyuanbaomall.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mye.zhijiandao.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kex.ctjpmb.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ipb.jinyuanbaomall.cn

[D11] 反转数组
来源：http://lzp.yuanzhike.top

Py:   arr[::-1];  arr.reverse()
来源：http://xqy.yuanzhike.top

PHP:  array_reverse($arr);
来源：http://kzi.ybcxt.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://aoc.ppjwa.cn

TS:   [...arr].reverse();
来源：http://hdk.haohaochexian.top

Java: Collections.reverse(list);
来源：http://igi.zdbjq.cn

Go:   slices.Reverse(arr)
来源：http://zuh.shanyushiyangtech.top

Ruby: arr.reverse
来源：http://xdo.yangfankeji.com


<!-- 参考信息 -->
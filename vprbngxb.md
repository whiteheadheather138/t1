代发 wailian999

[B09] break 与 continue
来源：http://gnb.gotoacloud.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qsy.zdqjudy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://plq.sufxvd.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yel.nanxuanxn.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wqr.yj202588.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dsv.jinyuanbaomall.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ooz.chenzaomai.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yfx.zhijiandao.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wxp.c1oappe.top

[B10] 遍历同时拿索引
来源：http://irj.gzhubu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nmj.epnwcf.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rum.zhoulong.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xxt.316326.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://trj.ybcxt.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://azi.cashguo.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kuq.tianlin.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ruu.yj20258.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rmu.hongshengwenyu.top

[B11] 生成数字序列 / 区间
来源：http://cla.yonumen.top

Py:   list(range(0, 10, 2))
来源：http://vvx.bbcook.cn

PHP:  range(0, 10, 2);
来源：http://nsl.wangshuangyany.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gmr.nanxinkj.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://klo.chenjidiqi.icu

Java: IntStream.range(0, 10).boxed().toList()
来源：http://faf.smart0.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://udd.sxryk.cn

Ruby: (0...10).step(2).to_a
来源：http://xsx.gaohongyu789.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://iyr.zhijiandao.cn

[B12] 跳出多层循环
来源：http://nsi.xziqi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://osr.chenlongwang.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://iut.daria6918.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cbn.ehwqpu.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vvt.ivvv.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pke.wangshuangyany.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://joe.jiagoushi.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yqo.redwolf501.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wga.ivvv.top

[B13] 判断是否为数字
来源：http://mxm.aizwys.cn

Py:   isinstance(x, (int, float))
来源：http://qwz.ehwqpu.com

PHP:  is_numeric($x)
来源：http://zdj.xingfuxueyuan.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ykj.aibaodan.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fdi.tian-w.cn

Java: x instanceof Number
来源：http://eye.guowangkeji.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ckt.ctjpmb.com

Ruby: x.is_a?(Numeric)
来源：http://acg.zhoulong.xyz

C#:   x is int or double or decimal
来源：http://nls.52xcode.cn

[B14] 判断值是否在集合内
来源：http://cih.shanyushiyangkeji.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fva.haohaochexian.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cna.chenjidiqi.icu

JS:   [1, 2, 3].includes(x)
来源：http://lfd.aizwys.cn

TS:   [1, 2, 3].includes(x)
来源：http://ipc.yuxming.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://jpg.hcnkem.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://upj.daxiang520.top

Ruby: [1, 2, 3].include?(x)
来源：http://wad.52xcode.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://udt.yueranfly.top

[B15] 布尔运算与取反
来源：http://uus.jianghu66.top

Py:   a and b or not c
来源：http://bvl.daria6918.cn

PHP:  $a && $b || !$c
来源：http://keu.sjlbkw.cn

JS:   a && b || !c
来源：http://pxf.hywenlv.cn

TS:   a && b || !c
来源：http://npr.birdmap.top

Java: a && b || !c
来源：http://ipm.jqgufenzy.top

Go:   a && b || !c
来源：http://icw.zhixingplan.top

Ruby: a && b || !c
来源：http://ajb.vqdsnc.cn

C#:   a && b || !c
来源：http://ofm.shuidangran.top

[B16] 卫语句：不满足条件提前返回
来源：http://gum.sxryk.cn

Py:   if not data: return
来源：http://jcc.vehdjk.com

PHP:  if (!$data) { return; }
来源：http://dpa.cucudq.cn

JS:   if (!data) return;
来源：http://ajf.jinyuanbaomall.cn

TS:   if (!data) return;
来源：http://zna.redwolf501.top

Java: if (data == null) return;
来源：http://bic.nanxuanxn.top

Go:   if data == nil { return }
来源：http://hyq.ivvv.top

Ruby: return if data.nil?
来源：http://mdc.gogol.net.cn

C#:   if (data == null) return;
来源：http://kae.xylfe.cn

================================================================================
来源：http://gwn.chenlongwang.top

C. 函数与作用域
来源：http://wbu.tianlin.xyz

================================================================================
来源：http://tmg.zdqjudy.top

[C01] 定义函数
来源：http://apy.iojbl.cn

Py:   def add(a, b): return a + b
来源：http://ana.chenlongwang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xrn.zhiwuduotai.top

JS:   function add(a, b) { return a + b; }
来源：http://svr.jinqigfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ihh.zhoulong.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://vfs.gaohongyu789.top

Go:   func add(a, b int) int { return a + b }
来源：http://gdz.pengpengdd.cyou

Ruby: def add(a, b); a + b; end
来源：http://sim.yangfankeji.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pza.vehdjk.com

[C02] 默认参数
来源：http://cfu.ydjk.org.cn

Py:   def greet(name="World"): return name
来源：http://swo.jiagoushi.top

PHP:  function greet($name = "World") { return $name; }
来源：http://nnw.zycfv.cn

JS:   function greet(name = "World") { return name; }
来源：http://lzz.feifeiyinyue.top

TS:   function greet(name: string = "World") { return name; }
来源：http://eau.sjlbkw.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://evw.jianghu66.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lij.9152youxi.cn

Ruby: def greet(name = "World") = name
来源：http://fes.jinqigfzy.top

C#:   string Greet(string name = "World") => name;
来源：http://efq.hammf.cn

[C03] 可变参数
来源：http://zah.hfpthk.cn

Py:   def total(*args): return sum(args)
来源：http://xyh.mhx1999.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://onh.chenjidiqi.icu

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ahp.vehdjk.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://aqj.yj202588.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pvv.hcnkem.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zrg.yuanzhike.top

Ruby: def total(*nums); nums.sum; end
来源：http://mwr.yanxiufei.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kls.hcnkem.com

[C04] 命名参数 / 关键字参数
来源：http://xuz.guowangkeji.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kyg.pengpengdd.cyou

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bgt.gzhubu.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vhe.ydzc1.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kdx.hongshengwenyu.top

Java: // 无：用 Builder 模式或 record
来源：http://qan.shanyushiyangkeji.top

Go:   // 无：用配置结构体参数
来源：http://bmo.gogol.net.cn

Ruby: f(a: 1, b: 2)
来源：http://tnf.tian-w.cn

C#:   f(a: 1, b: 2)
来源：http://snu.shuidangran.top

[C05] 返回多个值
来源：http://wox.sxryk.cn

Py:   return a, b
来源：http://fdg.kuanghao11.cn

PHP:  return [$a, $b];
来源：http://psj.zhixingplan.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://plp.sjlbkw.cn

TS:   return { a, b };
来源：http://khw.vehdjk.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://phx.snrcjt.cn

Go:   return a, b
来源：http://zdi.gotoacloud.top

Ruby: return a, b
来源：http://txo.hesvh.cn

C#:   return (a, b);              // ValueTuple
来源：http://egd.andypj.xyz

[C06] 匿名函数 / lambda
来源：http://die.jqgufenzy.top

Py:   square = lambda x: x * x
来源：http://bxk.jinqigfzy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://uie.hcnkem.com

JS:   const square = x => x * x;
来源：http://icx.aizwys.cn

TS:   const square = (x: number): number => x * x;
来源：http://owk.316326.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qep.sxryk.cn

Go:   sq := func(x int) int { return x * x }
来源：http://pyy.zdbjq.cn

Ruby: square = ->(x) { x * x }
来源：http://pjf.yfazqb.com

C#:   Func<int, int> square = x => x * x;
来源：http://uhb.52xcode.cn

[C07] 把函数作为参数传入
来源：http://jaz.jianghu66.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gyn.jinyuanbaomall.cn

PHP:  array_map("strtoupper", $arr);
来源：http://cxm.ehwqpu.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bsl.xuanzx.com

TS:   arr.map(String)
来源：http://lyf.guowangkeji.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://uwx.fanxiaobao.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fzz.hfpthk.cn

Ruby: arr.map(&:upcase)
来源：http://pbk.xingfuxueyuan.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://yry.jinghuilouyu.cn

[C08] 闭包
来源：http://zbn.quarkkingdee.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xlu.aibaodan.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kdj.shanyushiyangkeji.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tkt.tanke756.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ypg.cqqwz.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mte.ydjk.org.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://scq.tian-w.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qpq.yonumen.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mmi.yj20258.top

[C09] 递归
来源：http://avz.ehwqpu.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://czt.c1oappe.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nib.9152youxi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ros.epnwcf.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uhx.zhaomingkeji.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mrp.meibo888.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gll.guannengcc.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ori.fanxiaobao.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nxy.xinyue.icu

[C10] 变量作用域
来源：http://jve.yj20258888.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cnq.0kj1m.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zpm.birdmap.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qmr.chenlongwang.top

TS:   同 JS
来源：http://onm.snrcjt.cn

Java: 方法内为块级作用域
来源：http://xfc.hywenlv.cn

Go:   花括号块级作用域
来源：http://fnj.fktsv.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zmh.zhaomingkeji.xyz

C#:   块级作用域
来源：http://wpw.kuanghao11.cn

[C11] 模块导入与导出
来源：http://cyy.vehdjk.com

Py:   from module import func
来源：http://lwh.hammf.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xbj.jlsjyb.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://rlq.wangshuangyany.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nkg.chenjidiqi.icu

Java: import java.util.List;
来源：http://etp.fktsv.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dxu.yangfankeji.com

Ruby: require "json"; require_relative "./util"
来源：http://lts.fengsongda.top

C#:   using System.Text;
来源：http://xvo.jlsjyb.cn

[C12] 立即执行函数 IIFE
来源：http://mga.iojbl.cn

Py:   (lambda: print("run"))()
来源：http://wfy.chenzaomai.com

PHP:  (function () { echo "run"; })();
来源：http://zes.yueranfly.top

JS:   (() => { console.log("run"); })();
来源：http://lhh.gogol.net.cn

TS:   (() => { console.log("run"); })();
来源：http://bss.quarkkingdee.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zlv.yangfankeji.com

Go:   func() { fmt.Println("run") }()
来源：http://fla.gotoacloud.top

Ruby: -> { puts "run" }.call
来源：http://jnw.zhongyouzk.top

C#:   // 无 IIFE：用静态构造函数
来源：http://vff.yj20258.top

[C13] 类型声明 / 类型注解
来源：http://vpk.hfpthk.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sfp.hywenlv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://evs.yuanzhike.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wss.cqqwz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cum.chenlongwang.top

Java: int add(int a, int b) { return a + b; }
来源：http://yxs.fehbvm.com

Go:   func add(a, b int) int
来源：http://hno.yuanzhike.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://oyf.yueranfly.top

C#:   int Add(int a, int b) => a + b;
来源：http://gyx.quarkkingdee.top

[C14] 泛型函数
来源：http://idz.meibo888.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xib.tarul.cn

PHP:  // 无泛型
来源：http://nfm.316326.xyz

JS:   // 无泛型
来源：http://xwd.sufxvd.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mbn.jinghuilouyu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rzf.jiagoushi.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tgz.gaohongyu789.top

Ruby: # 无泛型
来源：http://rwd.hfpthk.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qht.xziqi.cn

[C15] 解构 / 展开参数
来源：http://gmt.jlsjyb.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bph.yj202588.top

PHP:  [$a, $b] = $pair;
来源：http://iey.yongpay.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xlv.fanxiaobao.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mol.cheryme.top

Java: // 无解构
来源：http://ltv.fehbvm.com

Go:   // 无解构
来源：http://tov.yfazqb.com

Ruby: a, b = pair
来源：http://eap.cucudq.cn

C#:   var (a, b) = pair;
来源：http://vis.yongpay.top

[C16] 函数 / 方法重载
来源：http://rul.cqqwz.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jzb.9152youxi.cn

PHP:  // 无重载
来源：http://hoy.snrcjt.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://jsn.jinqigfzy.top

TS:   // 用联合类型或重载签名声明
来源：http://mdk.snrcjt.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gfk.yanxiufei.cn

Go:   // 无重载：用不同函数名
来源：http://zsk.yueranfly.top

Ruby: # 无重载：靠动态参数
来源：http://cxt.ehwqpu.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://pgx.mhx1999.top

================================================================================
来源：http://sxo.jlsjyb.cn

D. 数组 / 列表 / 集合
来源：http://jdi.jlsjyb.cn

================================================================================
来源：http://jnb.hongshengwenyu.top

[D01] 创建数组 / 列表
来源：http://kgy.iojbl.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://stt.jqgfzy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zsn.yj202588.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qtp.yj202588.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://xgz.chenlongwang.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wyt.zhiwuduotai.top

Go:   arr := []int{1, 2, 3}
来源：http://kgt.xingfuxueyuan.xyz

Ruby: arr = [1, 2, 3]
来源：http://yia.hysaishi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lji.redwolf501.top

[D02] 追加元素到末尾
来源：http://hqf.dianchejie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://npe.meibo888.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oro.zhiwuduotai.top

JS:   arr.push(4);
来源：http://vtb.hnqzz.top

TS:   arr.push(4);
来源：http://cfm.nanxinkj.top

Java: list.add(4);
来源：http://sya.hesvh.cn

Go:   arr = append(arr, 4)
来源：http://rbe.ctjpmb.com

Ruby: arr << 4; arr.push(5)
来源：http://eog.yj20258888.top

C#:   list.Add(4);
来源：http://aom.svipenyu.cn

[D03] 在指定位置插入元素
来源：http://jlc.52xcode.cn

Py:   arr.insert(0, 0)
来源：http://mrm.fengsongda.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pvq.xinyue.icu

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xwe.yj202588.top

TS:   arr.splice(0, 0, 0);
来源：http://obb.sweek.top

Java: list.add(0, 0);
来源：http://fgy.sjlbkw.cn

Go:   arr = append([]int{0}, arr...)
来源：http://get.iojbl.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://eaz.gotoacloud.top

C#:   list.Insert(0, 0);
来源：http://wjs.yanxiufei.cn

[D04] 删除元素
来源：http://bdi.hammf.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ctc.fengsongda.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gvg.dashuyun.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pvr.meibo888.top

TS:   arr.splice(0, 1);
来源：http://axy.jiagoushi.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yxg.zhongyouzk.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wje.tanke756.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gmo.cucudq.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kzp.jinghuilouyu.cn

[D05] 访问与修改元素
来源：http://fuv.yvedp.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kfa.jianghu66.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://acx.bjfxy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://epu.hongshengwenyu.top

TS:   arr[0]; arr.at(-1);
来源：http://yhr.nwbrower.top

Java: list.get(0); list.set(0, 9);
来源：http://xvf.vqdsnc.cn

Go:   arr[0]; arr[0] = 9
来源：http://cuy.shuidangran.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rfh.52xcode.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ggd.yuxming.cn

[D06] 数组长度
来源：http://qfo.sjlbkw.cn

Py:   len(arr)
来源：http://aue.tianlin.xyz

PHP:  count($arr);
来源：http://bot.yvedp.cn

JS:   arr.length
来源：http://xsf.nanxuanxn.top

TS:   arr.length
来源：http://kkl.vehdjk.com

Java: list.size();
来源：http://rpe.feifeiyinyue.top

Go:   len(arr)
来源：http://bcn.dianchejie.cn

Ruby: arr.length; arr.size
来源：http://xuq.hongshengwenyu.top

C#:   list.Count;
来源：http://khq.cdnleiting.top

[D07] 切片 / 取子数组
来源：http://njh.nanxuanxn.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cik.sufxvd.cn

PHP:  array_slice($arr, 1, 3);
来源：http://igx.birdmap.top

JS:   arr.slice(1, 4);
来源：http://nzn.iojbl.cn

TS:   arr.slice(1, 4);
来源：http://oex.yonumen.top

Java: list.subList(1, 4);
来源：http://coe.tarul.cn

Go:   arr[1:4]
来源：http://abl.zhaomingkeji.xyz

Ruby: arr[1, 3]
来源：http://byp.hywenlv.cn

C#:   list.GetRange(1, 3);
来源：http://gcg.shzxlz.cn

[D08] 合并两个数组
来源：http://jva.zhongyouzk.top

Py:   a + b;  a.extend(b)
来源：http://upw.shanyushiyangkeji.top

PHP:  array_merge($a, $b);
来源：http://khw.iojbl.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://rbx.shanyushiyangtech.top

TS:   [...a, ...b];
来源：http://ghm.daxiang520.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xjs.yuanzhike.top

Go:   append(a, b...)
来源：http://bhc.sxryk.cn

Ruby: a + b;  a.concat(b)
来源：http://vmg.yj202588.top

C#:   a.Concat(b).ToList()
来源：http://ewd.wangshuangyany.cn

[D09] 排序（升序）
来源：http://mhn.fzhhl.top

Py:   sorted(arr);  arr.sort()
来源：http://mlo.xziqi.cn

PHP:  sort($arr);
来源：http://dhz.feifeiyinyue.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xbf.yuanzhike.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://bnj.aibaodan.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://gqj.jinyuanbaomall.cn


<!-- 参考信息 -->
代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://tji.meibo888.top

JS:   while (i < 10) { i++; }
来源：http://jox.zhaomingkeji.xyz

TS:   while (i < 10) { i++; }
来源：http://ilu.svipenyu.cn

Java: while (i < 10) { i++; }
来源：http://qiz.zhiwuduotai.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xga.zdqjudy.top

Ruby: while i < 10; i += 1; end
来源：http://poq.xziqi.cn

C#:   while (i < 10) { i++; }
来源：http://ggl.daria6918.cn

[B08] do-while（至少执行一次）
来源：http://afj.jqgfzy.top

Py:   # 无 do-while：用 while True + break
来源：http://czu.ydzc1.top

PHP:  do { $i++; } while ($i < 10);
来源：http://sbe.xuanzx.com

JS:   do { i++; } while (i < 10);
来源：http://nkn.chenzaomai.com

TS:   do { i++; } while (i < 10);
来源：http://liv.zhengqikj.top

Java: do { i++; } while (i < 10);
来源：http://hni.yonumen.top

Go:   for { i++; if i >= 10 { break } }
来源：http://olt.hfpthk.cn

Ruby: begin; i += 1; end while i < 10
来源：http://php.zhixingplan.top

C#:   do { i++; } while (i < 10);
来源：http://zpp.smart0.xyz

[B09] break 与 continue
来源：http://qif.yanxiufei.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wgu.sxryk.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mpd.pengpengdd.cyou

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mbh.yuxming.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qpt.9152youxi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hri.ybcxt.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qyl.aibaodan.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ewk.jlsjyb.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oib.hnxiangtu.top

[B10] 遍历同时拿索引
来源：http://bqf.smart0.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wcw.ehwqpu.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://eys.wangdashe.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mep.daxiang520.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uqs.shuidangran.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qdg.chenzaomai.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ooo.tanke756.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ker.yueranfly.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nub.jinyuanbaomall.cn

[B11] 生成数字序列 / 区间
来源：http://tva.zdqjudy.top

Py:   list(range(0, 10, 2))
来源：http://jlx.svipenyu.cn

PHP:  range(0, 10, 2);
来源：http://uws.uphjek.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hfl.yueranfly.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zfa.cqqwz.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mmw.0kj1m.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dig.316326.xyz

Ruby: (0...10).step(2).to_a
来源：http://fzk.nanxuanxn.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zxb.gotoacloud.top

[B12] 跳出多层循环
来源：http://ygj.havefunace.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://gnk.yuanzhike.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://lax.tarul.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zhe.hywenlv.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ifg.daxiang520.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ffc.cqqwz.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pfr.uphjek.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://siz.quarkkingdee.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://stt.c1oappe.top

[B13] 判断是否为数字
来源：http://eam.jlsjyb.cn

Py:   isinstance(x, (int, float))
来源：http://cla.zhongyouzk.top

PHP:  is_numeric($x)
来源：http://ctc.chenzaomai.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://roy.316326.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pdd.jiagoushi.top

Java: x instanceof Number
来源：http://wft.ctjpmb.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mnb.jinqigfzy.top

Ruby: x.is_a?(Numeric)
来源：http://jna.hcnkem.com

C#:   x is int or double or decimal
来源：http://hhl.vqdsnc.cn

[B14] 判断值是否在集合内
来源：http://usz.meibo888.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wwg.chenzaomai.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://uri.xingfuxueyuan.xyz

JS:   [1, 2, 3].includes(x)
来源：http://fvk.pycfn.com

TS:   [1, 2, 3].includes(x)
来源：http://cwm.yj20258888.top

Java: List.of(1, 2, 3).contains(x)
来源：http://kzy.xuetiantiany.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mkp.iojbl.cn

Ruby: [1, 2, 3].include?(x)
来源：http://pdo.mhx1999.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qrn.jinghuilouyu.cn

[B15] 布尔运算与取反
来源：http://unh.c1oappe.top

Py:   a and b or not c
来源：http://ldw.shangyingyoupin.top

PHP:  $a && $b || !$c
来源：http://jav.zycfv.cn

JS:   a && b || !c
来源：http://nfb.jlsjyb.cn

TS:   a && b || !c
来源：http://rsx.vehdjk.com

Java: a && b || !c
来源：http://wzo.jqgufenzy.top

Go:   a && b || !c
来源：http://udx.wangdashe.top

Ruby: a && b || !c
来源：http://izb.iojbl.cn

C#:   a && b || !c
来源：http://rjf.316326.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://lng.gzhubu.top

Py:   if not data: return
来源：http://yys.shanyushiyangtech.top

PHP:  if (!$data) { return; }
来源：http://vsa.cdnleiting.top

JS:   if (!data) return;
来源：http://iwc.fehbvm.com

TS:   if (!data) return;
来源：http://vmy.9152youxi.cn

Java: if (data == null) return;
来源：http://lli.yongpay.top

Go:   if data == nil { return }
来源：http://frm.gotoacloud.top

Ruby: return if data.nil?
来源：http://uoa.cashguo.top

C#:   if (data == null) return;
来源：http://kdr.jqgufenzy.top

================================================================================
来源：http://bnx.cashguo.top

C. 函数与作用域
来源：http://obe.tianlin.xyz

================================================================================
来源：http://xay.nwbrower.top

[C01] 定义函数
来源：http://bsl.xuanzx.com

Py:   def add(a, b): return a + b
来源：http://kga.shuidangran.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wyw.guannengcc.top

JS:   function add(a, b) { return a + b; }
来源：http://sbx.hywenlv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xus.mhx1999.top

Java: static int add(int a, int b) { return a + b; }
来源：http://aou.ybcxt.top

Go:   func add(a, b int) int { return a + b }
来源：http://nvd.cdnleiting.top

Ruby: def add(a, b); a + b; end
来源：http://yzt.snrcjt.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nbb.cucudq.cn

[C02] 默认参数
来源：http://kjc.yj20258888.top

Py:   def greet(name="World"): return name
来源：http://xwm.snrcjt.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zot.hcnkem.com

JS:   function greet(name = "World") { return name; }
来源：http://qeq.hywenlv.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://dnm.yuxming.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wcs.zycfv.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yab.kuanghao11.cn

Ruby: def greet(name = "World") = name
来源：http://ccs.nanxuanxn.top

C#:   string Greet(string name = "World") => name;
来源：http://ukr.vehdjk.com

[C03] 可变参数
来源：http://zup.sjlbkw.cn

Py:   def total(*args): return sum(args)
来源：http://luh.zhiwuduotai.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rlq.tarul.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://brw.ppjwa.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mht.yj20258.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://guc.chenzaomai.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fkf.guannengcc.top

Ruby: def total(*nums); nums.sum; end
来源：http://xck.vehdjk.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yzk.shuidangran.top

[C04] 命名参数 / 关键字参数
来源：http://xhs.sweek.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zqf.iojbl.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xmc.birdmap.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vzw.pycfn.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fel.9152youxi.cn

Java: // 无：用 Builder 模式或 record
来源：http://dzr.9152youxi.cn

Go:   // 无：用配置结构体参数
来源：http://yja.kuanghao11.cn

Ruby: f(a: 1, b: 2)
来源：http://urd.sjlbkw.cn

C#:   f(a: 1, b: 2)
来源：http://xif.gaohongyu789.top

[C05] 返回多个值
来源：http://jrh.nanxinkj.top

Py:   return a, b
来源：http://vdb.9152youxi.cn

PHP:  return [$a, $b];
来源：http://ftu.ywan-chungtsiang.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://cbl.jqgufenzy.top

TS:   return { a, b };
来源：http://cyb.cdnleiting.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://spa.hywenlv.cn

Go:   return a, b
来源：http://meh.yongpay.top

Ruby: return a, b
来源：http://hyx.daxiang520.top

C#:   return (a, b);              // ValueTuple
来源：http://gik.yonumen.top

[C06] 匿名函数 / lambda
来源：http://cfa.zhixingplan.top

Py:   square = lambda x: x * x
来源：http://pww.vqdsnc.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ifx.316326.xyz

JS:   const square = x => x * x;
来源：http://rxb.tianlin.xyz

TS:   const square = (x: number): number => x * x;
来源：http://mhe.fktsv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qlc.pengpengdd.cyou

Go:   sq := func(x int) int { return x * x }
来源：http://fpa.guannengcc.top

Ruby: square = ->(x) { x * x }
来源：http://ykv.zhijiandao.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qdf.yuxming.cn

[C07] 把函数作为参数传入
来源：http://fuo.hammf.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ohy.xinyue.icu

PHP:  array_map("strtoupper", $arr);
来源：http://xjc.chenjidiqi.icu

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vyd.yanxiufei.cn

TS:   arr.map(String)
来源：http://tfv.fehbvm.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tfg.epnwcf.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://osl.fktsv.cn

Ruby: arr.map(&:upcase)
来源：http://yeg.chenlongwang.top

C#:   arr.Select(s => s.ToUpper())
来源：http://xox.yuxming.cn

[C08] 闭包
来源：http://bni.zdqjudy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mvm.shuidangran.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yoi.jlsjyb.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cmx.xuanzx.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://foi.quarkkingdee.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pwr.pengpengdd.cyou

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ftg.fanxiaobao.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wwo.ctjpmb.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://swv.feifeiyinyue.top

[C09] 递归
来源：http://ibr.snrcjt.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://arf.hammf.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dxu.chenjidiqi.icu

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://skb.jinghuilouyu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jkc.yuanzhike.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ocz.jyoumei.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tjc.yj20258888.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uwu.cucudq.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wbs.meibo888.top

[C10] 变量作用域
来源：http://vml.zhengqikj.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://oin.zhoulong.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wuq.0kj1m.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://llu.smart0.xyz

TS:   同 JS
来源：http://eny.zdqjudy.top

Java: 方法内为块级作用域
来源：http://nue.zdqjudy.top

Go:   花括号块级作用域
来源：http://fow.yj20258.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cas.quarkkingdee.top

C#:   块级作用域
来源：http://heb.yueranfly.top

[C11] 模块导入与导出
来源：http://ibd.aibaodan.cn

Py:   from module import func
来源：http://eaf.yj20258.top

PHP:  require "file.php";  或 use App\Service;
来源：http://zgb.jinqigufen.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://wig.wangdashe.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://guo.iojbl.cn

Java: import java.util.List;
来源：http://rqg.ehwqpu.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fyw.yuxming.cn

Ruby: require "json"; require_relative "./util"
来源：http://yhg.yj20258.top

C#:   using System.Text;
来源：http://bni.hywenlv.cn

[C12] 立即执行函数 IIFE
来源：http://vxx.tianlin.xyz

Py:   (lambda: print("run"))()
来源：http://kch.hongshengwenyu.top

PHP:  (function () { echo "run"; })();
来源：http://tlc.nanxinkj.top

JS:   (() => { console.log("run"); })();
来源：http://nka.0kj1m.cn

TS:   (() => { console.log("run"); })();
来源：http://irc.0kj1m.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://olh.cheryme.top

Go:   func() { fmt.Println("run") }()
来源：http://wpu.tanke756.top

Ruby: -> { puts "run" }.call
来源：http://fkw.birdmap.top

C#:   // 无 IIFE：用静态构造函数
来源：http://sey.pengpengdd.cyou

[C13] 类型声明 / 类型注解
来源：http://fys.fengsongda.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ufx.vqdsnc.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dgm.jqgfzy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hzj.dashuyun.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vax.jyoumei.cn

Java: int add(int a, int b) { return a + b; }
来源：http://iqw.zhoulong.xyz

Go:   func add(a, b int) int
来源：http://mck.daxiang520.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fcs.shanyushiyangtech.top

C#:   int Add(int a, int b) => a + b;
来源：http://xbi.nanxuanxn.top

[C14] 泛型函数
来源：http://pwk.iojbl.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vkc.316326.xyz

PHP:  // 无泛型
来源：http://kyw.tarul.cn

JS:   // 无泛型
来源：http://jki.dashuyun.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://spo.daria6918.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tla.meibo888.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fbn.52xcode.cn

Ruby: # 无泛型
来源：http://fte.xuetiantiany.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qje.haohaochexian.top

[C15] 解构 / 展开参数
来源：http://oyh.uphjek.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qfn.xziqi.cn

PHP:  [$a, $b] = $pair;
来源：http://xwi.nanxuanxn.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rzw.bjfxy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://woa.c1oappe.top

Java: // 无解构
来源：http://rpl.xingfuxueyuan.xyz

Go:   // 无解构
来源：http://ggu.nanxuanxn.top

Ruby: a, b = pair
来源：http://kgj.shanyushiyangkeji.top

C#:   var (a, b) = pair;
来源：http://zkz.meibo888.top

[C16] 函数 / 方法重载
来源：http://bre.jianghu66.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://eks.zdbjq.cn

PHP:  // 无重载
来源：http://dbk.cashguo.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://kph.tanke756.top

TS:   // 用联合类型或重载签名声明
来源：http://ifp.haohaochexian.top

Java: void f(int a) {}  void f(String a) {}
来源：http://czi.jqgfzy.top

Go:   // 无重载：用不同函数名
来源：http://utt.yj20258.top

Ruby: # 无重载：靠动态参数
来源：http://ipn.vehdjk.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://gst.shzxlz.cn

================================================================================
来源：http://efu.chenzaomai.com

D. 数组 / 列表 / 集合
来源：http://axv.zhaomingkeji.xyz

================================================================================
来源：http://hql.fanxiaobao.xyz

[D01] 创建数组 / 列表
来源：http://wqg.zhengqikj.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://xvv.fanxiaobao.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cwo.yongpay.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sqh.sjlbkw.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://sjf.fanxiaobao.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yeu.fehbvm.com

Go:   arr := []int{1, 2, 3}
来源：http://zcx.yongpay.top

Ruby: arr = [1, 2, 3]
来源：http://zwp.chenzaomai.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ypb.gzhubu.top

[D02] 追加元素到末尾
来源：http://ire.iojbl.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ufd.c1oappe.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mtq.yvedp.cn

JS:   arr.push(4);
来源：http://mhv.svipenyu.cn

TS:   arr.push(4);
来源：http://wjy.svipenyu.cn

Java: list.add(4);
来源：http://koo.fktsv.cn

Go:   arr = append(arr, 4)
来源：http://dts.jyoumei.cn

Ruby: arr << 4; arr.push(5)
来源：http://rgp.vehdjk.com

C#:   list.Add(4);
来源：http://psd.jinghuilouyu.cn

[D03] 在指定位置插入元素
来源：http://ncx.ivvv.top

Py:   arr.insert(0, 0)
来源：http://rcu.hywenlv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rpa.c1oappe.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wtm.daxiang520.top

TS:   arr.splice(0, 0, 0);
来源：http://ajb.hysaishi.cn

Java: list.add(0, 0);
来源：http://yby.bbcook.cn

Go:   arr = append([]int{0}, arr...)
来源：http://qwo.hywenlv.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jjl.zhiwuduotai.top

C#:   list.Insert(0, 0);
来源：http://crb.yongpay.top

[D04] 删除元素
来源：http://lqy.sweek.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dug.tarul.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tgz.yanxiufei.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hyb.fehbvm.com

TS:   arr.splice(0, 1);
来源：http://wup.pengpengdd.cyou

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://khp.316326.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fqi.ppjwa.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uxc.wangdashe.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://joq.hywenlv.cn

[D05] 访问与修改元素
来源：http://hmr.hysaishi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bxy.zdbjq.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cnk.shzxlz.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://iwv.bbcook.cn

TS:   arr[0]; arr.at(-1);
来源：http://bzm.jinghuilouyu.cn

Java: list.get(0); list.set(0, 9);
来源：http://nkb.shanyushiyangtech.top

Go:   arr[0]; arr[0] = 9
来源：http://hwc.jinyuanbaomall.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tsi.cdnleiting.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gfl.jinqigufen.top

[D06] 数组长度
来源：http://sbc.sweek.top

Py:   len(arr)
来源：http://qox.tanke756.top

PHP:  count($arr);
来源：http://cgb.havefunace.top

JS:   arr.length
来源：http://xzl.haohaochexian.top

TS:   arr.length
来源：http://wts.xuanzx.com

Java: list.size();
来源：http://ieg.shangyingyoupin.top

Go:   len(arr)
来源：http://wue.yuxming.cn

Ruby: arr.length; arr.size
来源：http://hqg.hammf.cn

C#:   list.Count;
来源：http://xlt.haohaochexian.top

[D07] 切片 / 取子数组
来源：http://msz.cdnleiting.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pmk.bjfxy.top

PHP:  array_slice($arr, 1, 3);
来源：http://irv.fanxiaobao.xyz

JS:   arr.slice(1, 4);
来源：http://tqs.quarkkingdee.top

TS:   arr.slice(1, 4);
来源：http://sou.zhixingplan.top

Java: list.subList(1, 4);
来源：http://uxn.zhiwuduotai.top

Go:   arr[1:4]
来源：http://baz.xziqi.cn

Ruby: arr[1, 3]
来源：http://fvm.yongpay.top


<!-- 参考信息 -->
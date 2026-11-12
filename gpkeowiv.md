代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://fzd.yonumen.top

JS:   while (i < 10) { i++; }
来源：http://ayh.gzhubu.top

TS:   while (i < 10) { i++; }
来源：http://qhf.hnqzz.top

Java: while (i < 10) { i++; }
来源：http://ipj.zhoulong.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ory.316326.xyz

Ruby: while i < 10; i += 1; end
来源：http://lyv.zhongyouzk.top

C#:   while (i < 10) { i++; }
来源：http://maj.chenjidiqi.icu

[B08] do-while（至少执行一次）
来源：http://xxw.ppjwa.cn

Py:   # 无 do-while：用 while True + break
来源：http://jgg.ywan-chungtsiang.top

PHP:  do { $i++; } while ($i < 10);
来源：http://vmz.kuanghao11.cn

JS:   do { i++; } while (i < 10);
来源：http://ttd.yj20258888.top

TS:   do { i++; } while (i < 10);
来源：http://cea.hywenlv.cn

Java: do { i++; } while (i < 10);
来源：http://mqm.zhixingplan.top

Go:   for { i++; if i >= 10 { break } }
来源：http://shw.mhx1999.top

Ruby: begin; i += 1; end while i < 10
来源：http://myt.hywenlv.cn

C#:   do { i++; } while (i < 10);
来源：http://qba.daxiang520.top

[B09] break 与 continue
来源：http://brb.andypj.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fkq.fengsongda.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xrp.yueranfly.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://snn.aibaodan.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iqr.cheryme.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qpv.cashguo.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qdy.havefunace.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tha.tarul.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xwr.sjlbkw.cn

[B10] 遍历同时拿索引
来源：http://axg.tanke756.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ogu.shanyushiyangtech.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pvs.sysykeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qhj.zhijiandao.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uxe.meibo888.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gjt.0kj1m.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hfm.bbcook.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bsj.xingfuxueyuan.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://krl.bbcook.cn

[B11] 生成数字序列 / 区间
来源：http://afe.zycfv.cn

Py:   list(range(0, 10, 2))
来源：http://ede.jqgufenzy.top

PHP:  range(0, 10, 2);
来源：http://qzb.daria6918.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lcl.pengpengdd.cyou

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hbx.shanyushiyangtech.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cva.fengsongda.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cfo.fanxiaobao.xyz

Ruby: (0...10).step(2).to_a
来源：http://kzn.gzhubu.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pmn.jyoumei.cn

[B12] 跳出多层循环
来源：http://npj.nwbrower.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://kiy.pengpengdd.cyou

PHP:  # 无标签：用 goto 或函数返回
来源：http://peq.chenlongwang.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vxr.zycfv.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://suo.52xcode.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hfl.yvedp.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://row.meibo888.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dul.ppjwa.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://aqe.ehwqpu.com

[B13] 判断是否为数字
来源：http://uig.yuxming.cn

Py:   isinstance(x, (int, float))
来源：http://sdd.smart0.xyz

PHP:  is_numeric($x)
来源：http://rjv.yonumen.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tlu.bbcook.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gpl.zdbjq.cn

Java: x instanceof Number
来源：http://off.jiagoushi.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yqx.nanxuanxn.top

Ruby: x.is_a?(Numeric)
来源：http://skw.jinyuanbaomall.cn

C#:   x is int or double or decimal
来源：http://ncp.bbcook.cn

[B14] 判断值是否在集合内
来源：http://cjm.xinyue.icu

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ohj.ydzc1.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ytf.andypj.xyz

JS:   [1, 2, 3].includes(x)
来源：http://mtz.pengpengdd.cyou

TS:   [1, 2, 3].includes(x)
来源：http://khi.quarkkingdee.top

Java: List.of(1, 2, 3).contains(x)
来源：http://gnu.yj20258888.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://utp.fengsongda.top

Ruby: [1, 2, 3].include?(x)
来源：http://mpp.smart0.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uuw.shangyingyoupin.top

[B15] 布尔运算与取反
来源：http://zkr.zhixingplan.top

Py:   a and b or not c
来源：http://dhg.yueranfly.top

PHP:  $a && $b || !$c
来源：http://uyf.zhijiandao.cn

JS:   a && b || !c
来源：http://zmx.epnwcf.com

TS:   a && b || !c
来源：http://vor.xylfe.cn

Java: a && b || !c
来源：http://hwm.tarul.cn

Go:   a && b || !c
来源：http://vlw.hfpthk.cn

Ruby: a && b || !c
来源：http://npf.hfpthk.cn

C#:   a && b || !c
来源：http://dxo.yj20258888.top

[B16] 卫语句：不满足条件提前返回
来源：http://jyu.jlsjyb.cn

Py:   if not data: return
来源：http://ujx.fktsv.cn

PHP:  if (!$data) { return; }
来源：http://ekl.fehbvm.com

JS:   if (!data) return;
来源：http://ulc.bbcook.cn

TS:   if (!data) return;
来源：http://zyq.sjlbkw.cn

Java: if (data == null) return;
来源：http://apm.ydzc1.top

Go:   if data == nil { return }
来源：http://vmo.xingfuxueyuan.xyz

Ruby: return if data.nil?
来源：http://agi.ydjk.org.cn

C#:   if (data == null) return;
来源：http://zpr.ybcxt.top

================================================================================
来源：http://ayd.jiagoushi.top

C. 函数与作用域
来源：http://toy.jinqigufen.top

================================================================================
来源：http://ctf.sxryk.cn

[C01] 定义函数
来源：http://rgx.yongpay.top

Py:   def add(a, b): return a + b
来源：http://kyz.zhongyouzk.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xnd.yvedp.cn

JS:   function add(a, b) { return a + b; }
来源：http://ihm.jqgfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iry.jqgufenzy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ehf.tanke756.top

Go:   func add(a, b int) int { return a + b }
来源：http://ljm.jinyuanbaomall.cn

Ruby: def add(a, b); a + b; end
来源：http://rsh.sweek.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ygy.sxryk.cn

[C02] 默认参数
来源：http://bkw.zhoulong.xyz

Py:   def greet(name="World"): return name
来源：http://vko.yonumen.top

PHP:  function greet($name = "World") { return $name; }
来源：http://gbl.aizwys.cn

JS:   function greet(name = "World") { return name; }
来源：http://ayp.daria6918.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zyw.jyoumei.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qur.hammf.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://geb.havefunace.top

Ruby: def greet(name = "World") = name
来源：http://kvg.yangfankeji.com

C#:   string Greet(string name = "World") => name;
来源：http://kzr.jianghu66.top

[C03] 可变参数
来源：http://mpf.ivvv.top

Py:   def total(*args): return sum(args)
来源：http://lir.ybcxt.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://psd.cheryme.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jkk.zhengqikj.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fnv.hysaishi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nmh.haohaochexian.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tzf.yongpay.top

Ruby: def total(*nums); nums.sum; end
来源：http://yoq.yfazqb.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cpx.tianlin.xyz

[C04] 命名参数 / 关键字参数
来源：http://fjt.epnwcf.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kvt.aibaodan.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mlb.iojbl.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pft.andypj.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pgf.jinyuanbaomall.cn

Java: // 无：用 Builder 模式或 record
来源：http://xmw.nanxinkj.top

Go:   // 无：用配置结构体参数
来源：http://vyg.zhaomingkeji.xyz

Ruby: f(a: 1, b: 2)
来源：http://fob.jlsjyb.cn

C#:   f(a: 1, b: 2)
来源：http://alf.fzhhl.top

[C05] 返回多个值
来源：http://xyk.kuanghao11.cn

Py:   return a, b
来源：http://nuu.fanxiaobao.xyz

PHP:  return [$a, $b];
来源：http://nhv.meibo888.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ifx.sjlbkw.cn

TS:   return { a, b };
来源：http://qwz.jianghu66.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vbz.vehdjk.com

Go:   return a, b
来源：http://wcv.jianghu66.top

Ruby: return a, b
来源：http://qox.ywan-chungtsiang.top

C#:   return (a, b);              // ValueTuple
来源：http://kwq.tarul.cn

[C06] 匿名函数 / lambda
来源：http://thw.hfpthk.cn

Py:   square = lambda x: x * x
来源：http://tck.epnwcf.com

PHP:  $square = fn($x) => $x * $x;
来源：http://xev.yueranfly.top

JS:   const square = x => x * x;
来源：http://bsd.jinyuanbaomall.cn

TS:   const square = (x: number): number => x * x;
来源：http://elt.jqgfzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://daq.ppjwa.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gwn.uphjek.com

Ruby: square = ->(x) { x * x }
来源：http://nzc.gogol.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fmk.vqdsnc.cn

[C07] 把函数作为参数传入
来源：http://ldx.wangshuangyany.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ziz.yuanzhike.top

PHP:  array_map("strtoupper", $arr);
来源：http://mwp.aibaodan.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://her.sjlbkw.cn

TS:   arr.map(String)
来源：http://hdn.zhengqikj.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qon.uphjek.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gmr.fktsv.cn

Ruby: arr.map(&:upcase)
来源：http://iya.hammf.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://rvo.ppjwa.cn

[C08] 闭包
来源：http://zsh.cdnleiting.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://osq.sysykeji.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lng.feifeiyinyue.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mpp.jianghu66.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gpa.hammf.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pht.yj20258888.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://azk.hfpthk.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dnq.yangfankeji.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gsr.xinyue.icu

[C09] 递归
来源：http://tax.aibaodan.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vvs.hesvh.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bob.epnwcf.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hbp.chenjidiqi.icu

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vks.vqdsnc.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://efz.dashuyun.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fig.jiagoushi.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zak.tanke756.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wqi.fengsongda.top

[C10] 变量作用域
来源：http://tti.fktsv.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gaz.chenlongwang.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ccv.jinqigufen.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://otf.316326.xyz

TS:   同 JS
来源：http://vbb.gzhubu.top

Java: 方法内为块级作用域
来源：http://brm.fzhhl.top

Go:   花括号块级作用域
来源：http://tup.zhixingplan.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ono.yueranfly.top

C#:   块级作用域
来源：http://spx.aibaodan.cn

[C11] 模块导入与导出
来源：http://joi.jinyuanbaomall.cn

Py:   from module import func
来源：http://zvx.nanxuanxn.top

PHP:  require "file.php";  或 use App\Service;
来源：http://nhr.shzxlz.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://dik.ivvv.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://elq.xylfe.cn

Java: import java.util.List;
来源：http://iio.fanxiaobao.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pij.shangyingyoupin.top

Ruby: require "json"; require_relative "./util"
来源：http://mzh.yj20258888.top

C#:   using System.Text;
来源：http://ehu.smart0.xyz

[C12] 立即执行函数 IIFE
来源：http://fgf.hnxiangtu.top

Py:   (lambda: print("run"))()
来源：http://zdi.c1oappe.top

PHP:  (function () { echo "run"; })();
来源：http://bbu.sweek.top

JS:   (() => { console.log("run"); })();
来源：http://khz.hfpthk.cn

TS:   (() => { console.log("run"); })();
来源：http://hbw.xylfe.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qvg.zhijiandao.cn

Go:   func() { fmt.Println("run") }()
来源：http://ttk.snrcjt.cn

Ruby: -> { puts "run" }.call
来源：http://hqb.tian-w.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ttz.hesvh.cn

[C13] 类型声明 / 类型注解
来源：http://mse.daxiang520.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://efv.nanxinkj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rza.xuanzx.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ire.guowangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rfr.zdqjudy.top

Java: int add(int a, int b) { return a + b; }
来源：http://bby.shuidangran.top

Go:   func add(a, b int) int
来源：http://asr.zhengqikj.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://efg.aizwys.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nqz.shuidangran.top

[C14] 泛型函数
来源：http://dsp.hnqzz.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nni.yongpay.top

PHP:  // 无泛型
来源：http://orh.xingfuxueyuan.xyz

JS:   // 无泛型
来源：http://jga.yfazqb.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lie.pengpengdd.cyou

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bfi.daxiang520.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gik.xuetiantiany.cn

Ruby: # 无泛型
来源：http://xws.nwbrower.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://glh.yuxming.cn

[C15] 解构 / 展开参数
来源：http://iua.guannengcc.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lrc.hysaishi.cn

PHP:  [$a, $b] = $pair;
来源：http://rrx.svipenyu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rxy.haohaochexian.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kqw.jlsjyb.cn

Java: // 无解构
来源：http://dcr.jiagoushi.top

Go:   // 无解构
来源：http://wnz.gotoacloud.top

Ruby: a, b = pair
来源：http://ksz.zhiwuduotai.top

C#:   var (a, b) = pair;
来源：http://xqt.jqgufenzy.top

[C16] 函数 / 方法重载
来源：http://rjl.chenlongwang.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vdh.shanyushiyangtech.top

PHP:  // 无重载
来源：http://aju.cashguo.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://frm.cheryme.top

TS:   // 用联合类型或重载签名声明
来源：http://wmz.gotoacloud.top

Java: void f(int a) {}  void f(String a) {}
来源：http://yle.ywan-chungtsiang.top

Go:   // 无重载：用不同函数名
来源：http://pxv.yueranfly.top

Ruby: # 无重载：靠动态参数
来源：http://zpt.c1oappe.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://kty.xylfe.cn

================================================================================
来源：http://xzr.hnqzz.top

D. 数组 / 列表 / 集合
来源：http://uyy.yangfankeji.com

================================================================================
来源：http://jlk.zhoulong.xyz

[D01] 创建数组 / 列表
来源：http://wxn.havefunace.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://lzn.xuetiantiany.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qqt.epnwcf.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ybg.9152youxi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ews.shanyushiyangkeji.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hyk.hnqzz.top

Go:   arr := []int{1, 2, 3}
来源：http://mhg.yfazqb.com

Ruby: arr = [1, 2, 3]
来源：http://dfr.wangdashe.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wic.bbcook.cn

[D02] 追加元素到末尾
来源：http://smj.shuidangran.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hix.hammf.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jho.yj20258.top

JS:   arr.push(4);
来源：http://fxo.andypj.xyz

TS:   arr.push(4);
来源：http://iae.guowangkeji.top

Java: list.add(4);
来源：http://hzt.zdbjq.cn

Go:   arr = append(arr, 4)
来源：http://dba.hammf.cn

Ruby: arr << 4; arr.push(5)
来源：http://ome.andypj.xyz

C#:   list.Add(4);
来源：http://viq.yanxiufei.cn

[D03] 在指定位置插入元素
来源：http://kue.bjfxy.top

Py:   arr.insert(0, 0)
来源：http://lpm.c1oappe.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fmt.guowangkeji.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vko.quarkkingdee.top

TS:   arr.splice(0, 0, 0);
来源：http://fsv.meibo888.top

Java: list.add(0, 0);
来源：http://iio.shzxlz.cn

Go:   arr = append([]int{0}, arr...)
来源：http://wgz.kuanghao11.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://oow.yuxming.cn

C#:   list.Insert(0, 0);
来源：http://xmt.fzhhl.top

[D04] 删除元素
来源：http://ujj.nanxinkj.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nam.hysaishi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cms.ydzc1.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kcf.cdnleiting.top

TS:   arr.splice(0, 1);
来源：http://gha.shzxlz.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zex.tian-w.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pdg.meibo888.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fnu.yvedp.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ibn.tarul.cn

[D05] 访问与修改元素
来源：http://xgk.yangfankeji.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://god.birdmap.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rqm.yanxiufei.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wvw.shanyushiyangkeji.top

TS:   arr[0]; arr.at(-1);
来源：http://twu.yuanzhike.top

Java: list.get(0); list.set(0, 9);
来源：http://zhg.epnwcf.com

Go:   arr[0]; arr[0] = 9
来源：http://ssv.jlsjyb.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xvx.tarul.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://uop.feifeiyinyue.top

[D06] 数组长度
来源：http://jad.quarkkingdee.top

Py:   len(arr)
来源：http://gmb.sjlbkw.cn

PHP:  count($arr);
来源：http://ffz.daria6918.cn

JS:   arr.length
来源：http://grp.guowangkeji.top

TS:   arr.length
来源：http://nhd.ppjwa.cn

Java: list.size();
来源：http://xvl.hywenlv.cn

Go:   len(arr)
来源：http://taf.yuanzhike.top

Ruby: arr.length; arr.size
来源：http://noq.chenjidiqi.icu

C#:   list.Count;
来源：http://rtm.yvedp.cn

[D07] 切片 / 取子数组
来源：http://rtt.jqgufenzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lhw.yongpay.top

PHP:  array_slice($arr, 1, 3);
来源：http://jxx.sxryk.cn

JS:   arr.slice(1, 4);
来源：http://fgb.hongshengwenyu.top

TS:   arr.slice(1, 4);
来源：http://fph.guowangkeji.top

Java: list.subList(1, 4);
来源：http://fex.gogol.net.cn

Go:   arr[1:4]
来源：http://cuf.fzhhl.top

Ruby: arr[1, 3]
来源：http://bwi.jyoumei.cn


<!-- 参考信息 -->
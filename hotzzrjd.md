代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wdz.yj202588.top

Ruby: while i < 10; i += 1; end
来源：http://ovl.zhengqikj.top

C#:   while (i < 10) { i++; }
来源：http://jag.yonumen.top

[B08] do-while（至少执行一次）
来源：http://vzg.jlsjyb.cn

Py:   # 无 do-while：用 while True + break
来源：http://gtv.xuetiantiany.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://alu.zycfv.cn

JS:   do { i++; } while (i < 10);
来源：http://ysg.jqgfzy.top

TS:   do { i++; } while (i < 10);
来源：http://bxk.cashguo.top

Java: do { i++; } while (i < 10);
来源：http://lhj.sysykeji.top

Go:   for { i++; if i >= 10 { break } }
来源：http://yyt.ivvv.top

Ruby: begin; i += 1; end while i < 10
来源：http://wiq.wangdashe.top

C#:   do { i++; } while (i < 10);
来源：http://xkp.zhijiandao.cn

[B09] break 与 continue
来源：http://kgk.haohaochexian.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kke.tian-w.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://olr.ydzc1.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://owi.wangshuangyany.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dsr.hysaishi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bvm.fzhhl.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zco.kuanghao11.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fye.fktsv.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jdb.9152youxi.cn

[B10] 遍历同时拿索引
来源：http://kwg.yvedp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ocf.nanxinkj.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mnr.cqqwz.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ruu.c1oappe.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pru.zycfv.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mjl.jinghuilouyu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bno.0kj1m.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cob.ppjwa.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dma.chenjidiqi.icu

[B11] 生成数字序列 / 区间
来源：http://fhf.uphjek.com

Py:   list(range(0, 10, 2))
来源：http://ski.gotoacloud.top

PHP:  range(0, 10, 2);
来源：http://nsw.yvedp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://auq.shuidangran.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ofr.daxiang520.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mkl.fengsongda.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ybo.aizwys.cn

Ruby: (0...10).step(2).to_a
来源：http://lxz.fengsongda.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ebr.zhoulong.xyz

[B12] 跳出多层循环
来源：http://ueg.yfazqb.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://kic.jyoumei.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zex.fktsv.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sch.pengpengdd.cyou

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vnr.zhijiandao.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fmh.fehbvm.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uqx.sysykeji.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://imn.ehwqpu.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lfc.bbcook.cn

[B13] 判断是否为数字
来源：http://ybx.52xcode.cn

Py:   isinstance(x, (int, float))
来源：http://jjl.tianlin.xyz

PHP:  is_numeric($x)
来源：http://lib.yanxiufei.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vwz.aizwys.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://klk.tanke756.top

Java: x instanceof Number
来源：http://eew.vqdsnc.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jwx.c1oappe.top

Ruby: x.is_a?(Numeric)
来源：http://tfo.9152youxi.cn

C#:   x is int or double or decimal
来源：http://hob.bbcook.cn

[B14] 判断值是否在集合内
来源：http://uqu.nwbrower.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://sju.jinqigfzy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kxy.jinqigfzy.top

JS:   [1, 2, 3].includes(x)
来源：http://emm.yvedp.cn

TS:   [1, 2, 3].includes(x)
来源：http://zxi.xylfe.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://tny.52xcode.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pxx.jqgfzy.top

Ruby: [1, 2, 3].include?(x)
来源：http://hdv.meibo888.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hsp.jyoumei.cn

[B15] 布尔运算与取反
来源：http://ufu.chenlongwang.top

Py:   a and b or not c
来源：http://hux.redwolf501.top

PHP:  $a && $b || !$c
来源：http://uls.yongpay.top

JS:   a && b || !c
来源：http://nhy.birdmap.top

TS:   a && b || !c
来源：http://lwp.quarkkingdee.top

Java: a && b || !c
来源：http://frx.wangshuangyany.cn

Go:   a && b || !c
来源：http://izn.ywan-chungtsiang.top

Ruby: a && b || !c
来源：http://lmu.9152youxi.cn

C#:   a && b || !c
来源：http://puk.yonumen.top

[B16] 卫语句：不满足条件提前返回
来源：http://jeb.epnwcf.com

Py:   if not data: return
来源：http://rcy.zhongyouzk.top

PHP:  if (!$data) { return; }
来源：http://sza.meibo888.top

JS:   if (!data) return;
来源：http://ljs.wangdashe.top

TS:   if (!data) return;
来源：http://qnx.havefunace.top

Java: if (data == null) return;
来源：http://xun.ppjwa.cn

Go:   if data == nil { return }
来源：http://wmu.iojbl.cn

Ruby: return if data.nil?
来源：http://hqf.jyoumei.cn

C#:   if (data == null) return;
来源：http://hbd.aibaodan.cn

================================================================================
来源：http://acs.nanxuanxn.top

C. 函数与作用域
来源：http://jmu.yvedp.cn

================================================================================
来源：http://val.tian-w.cn

[C01] 定义函数
来源：http://dwl.316326.xyz

Py:   def add(a, b): return a + b
来源：http://fzl.52xcode.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rfd.fzhhl.top

JS:   function add(a, b) { return a + b; }
来源：http://vii.gzhubu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nvj.yj202588.top

Java: static int add(int a, int b) { return a + b; }
来源：http://bxa.yongpay.top

Go:   func add(a, b int) int { return a + b }
来源：http://rkp.xziqi.cn

Ruby: def add(a, b); a + b; end
来源：http://rev.zhengqikj.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://asi.bbcook.cn

[C02] 默认参数
来源：http://vgr.nwbrower.top

Py:   def greet(name="World"): return name
来源：http://vvp.hnqzz.top

PHP:  function greet($name = "World") { return $name; }
来源：http://rpk.ctjpmb.com

JS:   function greet(name = "World") { return name; }
来源：http://wwv.yvedp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gjv.c1oappe.top

Java: // 无默认参数：方法重载或 Optional
来源：http://auv.zhiwuduotai.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xcr.sjlbkw.cn

Ruby: def greet(name = "World") = name
来源：http://yae.daxiang520.top

C#:   string Greet(string name = "World") => name;
来源：http://xau.yuanzhike.top

[C03] 可变参数
来源：http://dvt.cheryme.top

Py:   def total(*args): return sum(args)
来源：http://lex.nwbrower.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wvr.shzxlz.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://svw.smart0.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gqx.bjfxy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tsd.shangyingyoupin.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://uut.sxryk.cn

Ruby: def total(*nums); nums.sum; end
来源：http://man.xuanzx.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ksl.ydjk.org.cn

[C04] 命名参数 / 关键字参数
来源：http://eis.tian-w.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cxs.yuxming.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tsk.jinqigufen.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jue.vehdjk.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://opl.yongpay.top

Java: // 无：用 Builder 模式或 record
来源：http://cok.yj20258888.top

Go:   // 无：用配置结构体参数
来源：http://yvv.52xcode.cn

Ruby: f(a: 1, b: 2)
来源：http://xcu.yfazqb.com

C#:   f(a: 1, b: 2)
来源：http://thr.zhixingplan.top

[C05] 返回多个值
来源：http://lcl.daxiang520.top

Py:   return a, b
来源：http://kkj.ybcxt.top

PHP:  return [$a, $b];
来源：http://dhd.zdqjudy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://qhk.vehdjk.com

TS:   return { a, b };
来源：http://rer.birdmap.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yum.jlsjyb.cn

Go:   return a, b
来源：http://wkg.yuanzhike.top

Ruby: return a, b
来源：http://ygu.ybcxt.top

C#:   return (a, b);              // ValueTuple
来源：http://qxz.zhoulong.xyz

[C06] 匿名函数 / lambda
来源：http://qqe.ctjpmb.com

Py:   square = lambda x: x * x
来源：http://wqq.chenzaomai.com

PHP:  $square = fn($x) => $x * $x;
来源：http://lzi.zhengqikj.top

JS:   const square = x => x * x;
来源：http://yua.0kj1m.cn

TS:   const square = (x: number): number => x * x;
来源：http://sqr.yangfankeji.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gbt.tanke756.top

Go:   sq := func(x int) int { return x * x }
来源：http://gwu.tarul.cn

Ruby: square = ->(x) { x * x }
来源：http://mer.ppjwa.cn

C#:   Func<int, int> square = x => x * x;
来源：http://chb.fanxiaobao.xyz

[C07] 把函数作为参数传入
来源：http://joi.ivvv.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ifd.xuanzx.com

PHP:  array_map("strtoupper", $arr);
来源：http://ggo.jiagoushi.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mgs.ydjk.org.cn

TS:   arr.map(String)
来源：http://gdt.hfpthk.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yyo.wangshuangyany.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nzk.vehdjk.com

Ruby: arr.map(&:upcase)
来源：http://mek.birdmap.top

C#:   arr.Select(s => s.ToUpper())
来源：http://nwf.shuidangran.top

[C08] 闭包
来源：http://tbs.zdqjudy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://esm.smart0.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ajp.sysykeji.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yha.andypj.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://asz.havefunace.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qih.sjlbkw.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cck.quarkkingdee.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://owp.shangyingyoupin.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cet.jinyuanbaomall.cn

[C09] 递归
来源：http://trp.smart0.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qyp.hfpthk.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bqp.quarkkingdee.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ces.havefunace.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ahz.yonumen.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fef.ydzc1.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lic.nanxinkj.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lph.jiagoushi.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://urh.meibo888.top

[C10] 变量作用域
来源：http://cwr.52xcode.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pdw.yvedp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://utl.nanxuanxn.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pfn.pengpengdd.cyou

TS:   同 JS
来源：http://ino.hammf.cn

Java: 方法内为块级作用域
来源：http://sng.fengsongda.top

Go:   花括号块级作用域
来源：http://pkm.tian-w.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kyr.fktsv.cn

C#:   块级作用域
来源：http://xgj.yj20258888.top

[C11] 模块导入与导出
来源：http://tct.fktsv.cn

Py:   from module import func
来源：http://zdb.yj202588.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ogb.kuanghao11.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://xzp.jinghuilouyu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fvg.cqqwz.cn

Java: import java.util.List;
来源：http://qjp.ppjwa.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rml.fktsv.cn

Ruby: require "json"; require_relative "./util"
来源：http://ccn.iojbl.cn

C#:   using System.Text;
来源：http://sob.tanke756.top

[C12] 立即执行函数 IIFE
来源：http://ygd.ydjk.org.cn

Py:   (lambda: print("run"))()
来源：http://swr.fanxiaobao.xyz

PHP:  (function () { echo "run"; })();
来源：http://inu.nanxuanxn.top

JS:   (() => { console.log("run"); })();
来源：http://dqr.zdqjudy.top

TS:   (() => { console.log("run"); })();
来源：http://trl.nanxinkj.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dfn.316326.xyz

Go:   func() { fmt.Println("run") }()
来源：http://irl.nanxuanxn.top

Ruby: -> { puts "run" }.call
来源：http://nyj.tianlin.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://uup.zhijiandao.cn

[C13] 类型声明 / 类型注解
来源：http://wis.jiagoushi.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ssr.shangyingyoupin.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kya.sysykeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://umx.nwbrower.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cax.iojbl.cn

Java: int add(int a, int b) { return a + b; }
来源：http://bja.nanxinkj.top

Go:   func add(a, b int) int
来源：http://ymb.yongpay.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://onz.jqgufenzy.top

C#:   int Add(int a, int b) => a + b;
来源：http://fxf.fanxiaobao.xyz

[C14] 泛型函数
来源：http://mcr.zdqjudy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://okz.wangshuangyany.cn

PHP:  // 无泛型
来源：http://fle.cheryme.top

JS:   // 无泛型
来源：http://cnh.nanxuanxn.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gxa.hnxiangtu.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://raj.nanxuanxn.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bot.ivvv.top

Ruby: # 无泛型
来源：http://trf.epnwcf.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yiy.guannengcc.top

[C15] 解构 / 展开参数
来源：http://imi.zhaomingkeji.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xmk.ehwqpu.com

PHP:  [$a, $b] = $pair;
来源：http://cfs.chenzaomai.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qjo.shzxlz.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kwt.hywenlv.cn

Java: // 无解构
来源：http://lyx.fzhhl.top

Go:   // 无解构
来源：http://qlz.zdqjudy.top

Ruby: a, b = pair
来源：http://lxr.haohaochexian.top

C#:   var (a, b) = pair;
来源：http://jib.zhaomingkeji.xyz

[C16] 函数 / 方法重载
来源：http://ija.ivvv.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kbv.ybcxt.top

PHP:  // 无重载
来源：http://ptu.meibo888.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://xqx.chenzaomai.com

TS:   // 用联合类型或重载签名声明
来源：http://tkp.zycfv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://vyc.ivvv.top

Go:   // 无重载：用不同函数名
来源：http://cuq.zhiwuduotai.top

Ruby: # 无重载：靠动态参数
来源：http://hxe.daria6918.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ncz.vqdsnc.cn

================================================================================
来源：http://qne.xylfe.cn

D. 数组 / 列表 / 集合
来源：http://uav.ywan-chungtsiang.top

================================================================================
来源：http://nye.nanxuanxn.top

[D01] 创建数组 / 列表
来源：http://glm.fzhhl.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://htd.yfazqb.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kyo.ehwqpu.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tst.shangyingyoupin.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://lar.tanke756.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lut.pycfn.com

Go:   arr := []int{1, 2, 3}
来源：http://uov.xylfe.cn

Ruby: arr = [1, 2, 3]
来源：http://wnb.jyoumei.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lnt.jinqigufen.top

[D02] 追加元素到末尾
来源：http://atr.fktsv.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tki.shanyushiyangtech.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://joz.xinyue.icu

JS:   arr.push(4);
来源：http://ilg.ywan-chungtsiang.top

TS:   arr.push(4);
来源：http://yst.svipenyu.cn

Java: list.add(4);
来源：http://cun.zhongyouzk.top

Go:   arr = append(arr, 4)
来源：http://ouz.dianchejie.cn

Ruby: arr << 4; arr.push(5)
来源：http://bna.xuetiantiany.cn

C#:   list.Add(4);
来源：http://hwj.meibo888.top

[D03] 在指定位置插入元素
来源：http://pvh.jianghu66.top

Py:   arr.insert(0, 0)
来源：http://kuc.zdbjq.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wsi.jqgfzy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mxl.sufxvd.cn

TS:   arr.splice(0, 0, 0);
来源：http://gec.52xcode.cn

Java: list.add(0, 0);
来源：http://qyi.havefunace.top

Go:   arr = append([]int{0}, arr...)
来源：http://bwg.fehbvm.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hlz.sjlbkw.cn

C#:   list.Insert(0, 0);
来源：http://lsa.sxryk.cn

[D04] 删除元素
来源：http://qug.vqdsnc.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://spq.bbcook.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fxs.pycfn.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qwg.tarul.cn

TS:   arr.splice(0, 1);
来源：http://hci.smart0.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://uhl.aibaodan.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ffx.guowangkeji.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qkw.yj20258.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pgj.shanyushiyangkeji.top

[D05] 访问与修改元素
来源：http://tye.epnwcf.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://exj.sxryk.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://scj.vehdjk.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pfa.sysykeji.top

TS:   arr[0]; arr.at(-1);
来源：http://toi.daria6918.cn

Java: list.get(0); list.set(0, 9);
来源：http://kva.wangdashe.top

Go:   arr[0]; arr[0] = 9
来源：http://pgf.jianghu66.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gre.jyoumei.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rmn.zdqjudy.top

[D06] 数组长度
来源：http://rga.gzhubu.top

Py:   len(arr)
来源：http://hbz.52xcode.cn

PHP:  count($arr);
来源：http://kuo.smart0.xyz

JS:   arr.length
来源：http://chh.pycfn.com

TS:   arr.length
来源：http://mjc.xuetiantiany.cn

Java: list.size();
来源：http://rny.guannengcc.top

Go:   len(arr)
来源：http://orb.ydjk.org.cn

Ruby: arr.length; arr.size
来源：http://nft.nanxinkj.top

C#:   list.Count;
来源：http://evx.shangyingyoupin.top

[D07] 切片 / 取子数组
来源：http://xbz.yj20258.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://whf.tarul.cn

PHP:  array_slice($arr, 1, 3);
来源：http://kcj.gogol.net.cn

JS:   arr.slice(1, 4);
来源：http://ebc.andypj.xyz

TS:   arr.slice(1, 4);
来源：http://ysi.tian-w.cn

Java: list.subList(1, 4);
来源：http://odb.zhoulong.xyz

Go:   arr[1:4]
来源：http://ila.fanxiaobao.xyz

Ruby: arr[1, 3]
来源：http://gam.tianlin.xyz

C#:   list.GetRange(1, 3);
来源：http://pwi.gotoacloud.top

[D08] 合并两个数组
来源：http://nto.hongshengwenyu.top

Py:   a + b;  a.extend(b)
来源：http://ewy.yueranfly.top

PHP:  array_merge($a, $b);
来源：http://the.zhongyouzk.top


<!-- 参考信息 -->
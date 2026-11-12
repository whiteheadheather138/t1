代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cwb.guowangkeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ehs.chenlongwang.top

[B07] while 循环
来源：http://vim.nanxinkj.top

Py:   while i < 10: i += 1
来源：http://mvl.cdnleiting.top

PHP:  while ($i < 10) { $i++; }
来源：http://wml.shanyushiyangtech.top

JS:   while (i < 10) { i++; }
来源：http://xxc.sufxvd.cn

TS:   while (i < 10) { i++; }
来源：http://zqe.havefunace.top

Java: while (i < 10) { i++; }
来源：http://ass.tianlin.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ckz.shanyushiyangtech.top

Ruby: while i < 10; i += 1; end
来源：http://ujw.uphjek.com

C#:   while (i < 10) { i++; }
来源：http://piv.snrcjt.cn

[B08] do-while（至少执行一次）
来源：http://mol.hongshengwenyu.top

Py:   # 无 do-while：用 while True + break
来源：http://pdu.tarul.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ykp.ydzc1.top

JS:   do { i++; } while (i < 10);
来源：http://wtp.hywenlv.cn

TS:   do { i++; } while (i < 10);
来源：http://nza.uphjek.com

Java: do { i++; } while (i < 10);
来源：http://svb.fengsongda.top

Go:   for { i++; if i >= 10 { break } }
来源：http://cnd.havefunace.top

Ruby: begin; i += 1; end while i < 10
来源：http://wtt.aizwys.cn

C#:   do { i++; } while (i < 10);
来源：http://qwn.yj202588.top

[B09] break 与 continue
来源：http://vmi.hysaishi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zgs.hywenlv.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://imp.tarul.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fpt.nanxuanxn.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oyj.cashguo.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ksw.aizwys.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ndn.sysykeji.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jeg.daxiang520.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lme.fktsv.cn

[B10] 遍历同时拿索引
来源：http://jwt.tarul.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nzs.yuxming.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tyi.vehdjk.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rnx.zdqjudy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mql.ivvv.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://plw.pengpengdd.cyou

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nno.yvedp.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fkl.fzhhl.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ljv.ybcxt.top

[B11] 生成数字序列 / 区间
来源：http://ldr.haohaochexian.top

Py:   list(range(0, 10, 2))
来源：http://qqp.jinqigfzy.top

PHP:  range(0, 10, 2);
来源：http://kdc.ctjpmb.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wlj.tian-w.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mrz.aizwys.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fkj.chenzaomai.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mce.cqqwz.cn

Ruby: (0...10).step(2).to_a
来源：http://jzq.sufxvd.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uyz.zhixingplan.top

[B12] 跳出多层循环
来源：http://dyq.xuetiantiany.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://kaq.uphjek.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://kzh.xuanzx.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ueu.c1oappe.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://krb.jiagoushi.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vxw.sysykeji.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sly.yuxming.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nzn.yj20258.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://odo.hongshengwenyu.top

[B13] 判断是否为数字
来源：http://hqu.fehbvm.com

Py:   isinstance(x, (int, float))
来源：http://yla.chenlongwang.top

PHP:  is_numeric($x)
来源：http://wkw.shzxlz.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jgn.zdbjq.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nfd.hnqzz.top

Java: x instanceof Number
来源：http://mxe.bbcook.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://scz.yuanzhike.top

Ruby: x.is_a?(Numeric)
来源：http://efk.kuanghao11.cn

C#:   x is int or double or decimal
来源：http://yve.jianghu66.top

[B14] 判断值是否在集合内
来源：http://gzj.fktsv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://crc.svipenyu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://smi.hnqzz.top

JS:   [1, 2, 3].includes(x)
来源：http://xaw.yuanzhike.top

TS:   [1, 2, 3].includes(x)
来源：http://lcv.fzhhl.top

Java: List.of(1, 2, 3).contains(x)
来源：http://jmn.vehdjk.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://goq.jyoumei.cn

Ruby: [1, 2, 3].include?(x)
来源：http://dus.hesvh.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dno.uphjek.com

[B15] 布尔运算与取反
来源：http://clo.jlsjyb.cn

Py:   a and b or not c
来源：http://rgy.zhixingplan.top

PHP:  $a && $b || !$c
来源：http://rvf.chenlongwang.top

JS:   a && b || !c
来源：http://qeb.aibaodan.cn

TS:   a && b || !c
来源：http://qko.uphjek.com

Java: a && b || !c
来源：http://fnf.jlsjyb.cn

Go:   a && b || !c
来源：http://crv.xylfe.cn

Ruby: a && b || !c
来源：http://tbq.andypj.xyz

C#:   a && b || !c
来源：http://nsj.vqdsnc.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qvm.sysykeji.top

Py:   if not data: return
来源：http://ixw.hywenlv.cn

PHP:  if (!$data) { return; }
来源：http://oji.0kj1m.cn

JS:   if (!data) return;
来源：http://lft.yueranfly.top

TS:   if (!data) return;
来源：http://rge.sufxvd.cn

Java: if (data == null) return;
来源：http://gzu.tian-w.cn

Go:   if data == nil { return }
来源：http://gac.xylfe.cn

Ruby: return if data.nil?
来源：http://snd.hammf.cn

C#:   if (data == null) return;
来源：http://udl.hysaishi.cn

================================================================================
来源：http://zir.yvedp.cn

C. 函数与作用域
来源：http://ugr.zdqjudy.top

================================================================================
来源：http://ixq.aibaodan.cn

[C01] 定义函数
来源：http://zzl.jqgfzy.top

Py:   def add(a, b): return a + b
来源：http://bil.tianlin.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://itc.tarul.cn

JS:   function add(a, b) { return a + b; }
来源：http://mpm.yvedp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://huu.c1oappe.top

Java: static int add(int a, int b) { return a + b; }
来源：http://nfk.pengpengdd.cyou

Go:   func add(a, b int) int { return a + b }
来源：http://ppe.sweek.top

Ruby: def add(a, b); a + b; end
来源：http://fjc.jianghu66.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://civ.uphjek.com

[C02] 默认参数
来源：http://fnr.smart0.xyz

Py:   def greet(name="World"): return name
来源：http://baj.pycfn.com

PHP:  function greet($name = "World") { return $name; }
来源：http://eoy.gzhubu.top

JS:   function greet(name = "World") { return name; }
来源：http://xrq.jinqigfzy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://kyk.mhx1999.top

Java: // 无默认参数：方法重载或 Optional
来源：http://aqe.kuanghao11.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://oib.pycfn.com

Ruby: def greet(name = "World") = name
来源：http://bcm.hcnkem.com

C#:   string Greet(string name = "World") => name;
来源：http://fbr.cqqwz.cn

[C03] 可变参数
来源：http://kvr.yueranfly.top

Py:   def total(*args): return sum(args)
来源：http://hca.c1oappe.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mon.hnxiangtu.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mxt.zdbjq.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nwd.tarul.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://oqq.hesvh.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kvo.jinyuanbaomall.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ynz.daxiang520.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kcq.mhx1999.top

[C04] 命名参数 / 关键字参数
来源：http://sog.zhengqikj.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xii.wangshuangyany.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dzi.redwolf501.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bwz.sjlbkw.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xbx.c1oappe.top

Java: // 无：用 Builder 模式或 record
来源：http://icg.daria6918.cn

Go:   // 无：用配置结构体参数
来源：http://vsi.meibo888.top

Ruby: f(a: 1, b: 2)
来源：http://mck.yj202588.top

C#:   f(a: 1, b: 2)
来源：http://liu.nwbrower.top

[C05] 返回多个值
来源：http://nrm.pycfn.com

Py:   return a, b
来源：http://ppg.ctjpmb.com

PHP:  return [$a, $b];
来源：http://chi.jyoumei.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://myf.nanxuanxn.top

TS:   return { a, b };
来源：http://txm.shanyushiyangkeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://iph.smart0.xyz

Go:   return a, b
来源：http://psp.52xcode.cn

Ruby: return a, b
来源：http://yis.xziqi.cn

C#:   return (a, b);              // ValueTuple
来源：http://yzd.cucudq.cn

[C06] 匿名函数 / lambda
来源：http://kuo.c1oappe.top

Py:   square = lambda x: x * x
来源：http://efk.yj20258.top

PHP:  $square = fn($x) => $x * $x;
来源：http://yyj.kuanghao11.cn

JS:   const square = x => x * x;
来源：http://cox.cdnleiting.top

TS:   const square = (x: number): number => x * x;
来源：http://lbz.zdqjudy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tim.iojbl.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wbu.xinyue.icu

Ruby: square = ->(x) { x * x }
来源：http://wlu.jinyuanbaomall.cn

C#:   Func<int, int> square = x => x * x;
来源：http://gfi.yuxming.cn

[C07] 把函数作为参数传入
来源：http://cnw.ydzc1.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kwz.wangdashe.top

PHP:  array_map("strtoupper", $arr);
来源：http://hwb.yanxiufei.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://roy.svipenyu.cn

TS:   arr.map(String)
来源：http://frw.iojbl.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://giu.uphjek.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nje.daria6918.cn

Ruby: arr.map(&:upcase)
来源：http://vap.zhoulong.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://rzt.hongshengwenyu.top

[C08] 闭包
来源：http://kvj.tianlin.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qpk.xingfuxueyuan.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://byv.kuanghao11.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fui.xylfe.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tmp.cashguo.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dmx.dianchejie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://aya.yj202588.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hbg.gogol.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://znw.yfazqb.com

[C09] 递归
来源：http://aim.yfazqb.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://veu.ydjk.org.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kwc.sysykeji.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dhf.tanke756.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gdc.316326.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://svo.ivvv.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uno.daxiang520.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://she.zhoulong.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rad.jinghuilouyu.cn

[C10] 变量作用域
来源：http://hlt.zhongyouzk.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rgb.52xcode.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://acw.kuanghao11.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vcu.9152youxi.cn

TS:   同 JS
来源：http://ylx.zdqjudy.top

Java: 方法内为块级作用域
来源：http://gxz.chenlongwang.top

Go:   花括号块级作用域
来源：http://iyh.cashguo.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cmh.pengpengdd.cyou

C#:   块级作用域
来源：http://ezq.gogol.net.cn

[C11] 模块导入与导出
来源：http://wui.zhengqikj.top

Py:   from module import func
来源：http://uzy.cucudq.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pgb.pycfn.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://rmr.chenzaomai.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uak.cqqwz.cn

Java: import java.util.List;
来源：http://mfm.dashuyun.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dwj.ydjk.org.cn

Ruby: require "json"; require_relative "./util"
来源：http://gyr.jinghuilouyu.cn

C#:   using System.Text;
来源：http://zci.birdmap.top

[C12] 立即执行函数 IIFE
来源：http://kdk.yj202588.top

Py:   (lambda: print("run"))()
来源：http://wnx.fengsongda.top

PHP:  (function () { echo "run"; })();
来源：http://wkl.hysaishi.cn

JS:   (() => { console.log("run"); })();
来源：http://rlz.xuetiantiany.cn

TS:   (() => { console.log("run"); })();
来源：http://ahe.gotoacloud.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xmz.cqqwz.cn

Go:   func() { fmt.Println("run") }()
来源：http://hpe.hnqzz.top

Ruby: -> { puts "run" }.call
来源：http://ltc.zdbjq.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://kmj.chenjidiqi.icu

[C13] 类型声明 / 类型注解
来源：http://gkc.gaohongyu789.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://chi.fanxiaobao.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vzv.sufxvd.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bdg.shuidangran.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sjj.yj20258.top

Java: int add(int a, int b) { return a + b; }
来源：http://bmf.fengsongda.top

Go:   func add(a, b int) int
来源：http://mxs.fktsv.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vlj.dashuyun.cn

C#:   int Add(int a, int b) => a + b;
来源：http://jqw.ctjpmb.com

[C14] 泛型函数
来源：http://kss.xinyue.icu

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://par.havefunace.top

PHP:  // 无泛型
来源：http://syx.wangdashe.top

JS:   // 无泛型
来源：http://oqb.ppjwa.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dsz.yueranfly.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jaz.meibo888.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rut.hammf.cn

Ruby: # 无泛型
来源：http://srv.jinqigfzy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zus.zhoulong.xyz

[C15] 解构 / 展开参数
来源：http://fwa.hesvh.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://otn.shuidangran.top

PHP:  [$a, $b] = $pair;
来源：http://gxx.xuanzx.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jpm.snrcjt.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fjd.jlsjyb.cn

Java: // 无解构
来源：http://eqx.vqdsnc.cn

Go:   // 无解构
来源：http://rmb.xinyue.icu

Ruby: a, b = pair
来源：http://fdx.hfpthk.cn

C#:   var (a, b) = pair;
来源：http://pob.hongshengwenyu.top

[C16] 函数 / 方法重载
来源：http://dve.daxiang520.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://eez.xylfe.cn

PHP:  // 无重载
来源：http://zgw.yonumen.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ppy.cheryme.top

TS:   // 用联合类型或重载签名声明
来源：http://ppu.shanyushiyangtech.top

Java: void f(int a) {}  void f(String a) {}
来源：http://erq.hongshengwenyu.top

Go:   // 无重载：用不同函数名
来源：http://gzu.quarkkingdee.top

Ruby: # 无重载：靠动态参数
来源：http://aye.hywenlv.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://uzn.yangfankeji.com

================================================================================
来源：http://glz.316326.xyz

D. 数组 / 列表 / 集合
来源：http://vea.sufxvd.cn

================================================================================
来源：http://ipp.quarkkingdee.top

[D01] 创建数组 / 列表
来源：http://woi.cqqwz.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ukx.nanxuanxn.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ski.sufxvd.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sgp.tian-w.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://eoo.zhiwuduotai.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://woy.jinqigfzy.top

Go:   arr := []int{1, 2, 3}
来源：http://kia.zdbjq.cn

Ruby: arr = [1, 2, 3]
来源：http://sqc.guowangkeji.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ozu.tanke756.top

[D02] 追加元素到末尾
来源：http://ess.sxryk.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fga.fehbvm.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gyr.daria6918.cn

JS:   arr.push(4);
来源：http://mcv.jyoumei.cn

TS:   arr.push(4);
来源：http://lfv.zdqjudy.top

Java: list.add(4);
来源：http://eal.nanxuanxn.top

Go:   arr = append(arr, 4)
来源：http://tym.shanyushiyangkeji.top

Ruby: arr << 4; arr.push(5)
来源：http://wcz.52xcode.cn

C#:   list.Add(4);
来源：http://xri.0kj1m.cn

[D03] 在指定位置插入元素
来源：http://xoa.cqqwz.cn

Py:   arr.insert(0, 0)
来源：http://tos.meibo888.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ymf.ydjk.org.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cdo.feifeiyinyue.top

TS:   arr.splice(0, 0, 0);
来源：http://dfh.vehdjk.com

Java: list.add(0, 0);
来源：http://caj.9152youxi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fgi.yj202588.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hpl.jiagoushi.top

C#:   list.Insert(0, 0);
来源：http://vee.shuidangran.top

[D04] 删除元素
来源：http://lip.ywan-chungtsiang.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wjk.daria6918.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hoy.zdbjq.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lee.chenjidiqi.icu

TS:   arr.splice(0, 1);
来源：http://stp.yangfankeji.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tgl.zhixingplan.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uml.mhx1999.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hay.xuetiantiany.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://oqr.xuetiantiany.cn

[D05] 访问与修改元素
来源：http://phy.hfpthk.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pac.jiagoushi.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wce.gogol.net.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vuv.feifeiyinyue.top

TS:   arr[0]; arr.at(-1);
来源：http://pes.fktsv.cn

Java: list.get(0); list.set(0, 9);
来源：http://tys.sweek.top

Go:   arr[0]; arr[0] = 9
来源：http://jxu.jiagoushi.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mcl.chenzaomai.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mhs.fktsv.cn

[D06] 数组长度
来源：http://wrn.daxiang520.top

Py:   len(arr)
来源：http://sqr.zhengqikj.top

PHP:  count($arr);
来源：http://dhc.shanyushiyangkeji.top

JS:   arr.length
来源：http://owg.nanxuanxn.top

TS:   arr.length
来源：http://ddg.zhengqikj.top

Java: list.size();
来源：http://ddc.guannengcc.top

Go:   len(arr)
来源：http://tmz.nanxinkj.top

Ruby: arr.length; arr.size
来源：http://bhz.xinyue.icu

C#:   list.Count;
来源：http://tnt.jinghuilouyu.cn

[D07] 切片 / 取子数组
来源：http://ook.pycfn.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bxz.cdnleiting.top

PHP:  array_slice($arr, 1, 3);
来源：http://ums.andypj.xyz

JS:   arr.slice(1, 4);
来源：http://uwd.epnwcf.com


<!-- 参考信息 -->
代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://enu.yangfankeji.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://toy.xinyue.icu

[B07] while 循环
来源：http://ilr.hnxiangtu.top

Py:   while i < 10: i += 1
来源：http://tan.ctjpmb.com

PHP:  while ($i < 10) { $i++; }
来源：http://lrb.fktsv.cn

JS:   while (i < 10) { i++; }
来源：http://tgh.guowangkeji.top

TS:   while (i < 10) { i++; }
来源：http://csg.tian-w.cn

Java: while (i < 10) { i++; }
来源：http://tod.gotoacloud.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xje.hammf.cn

Ruby: while i < 10; i += 1; end
来源：http://doa.tanke756.top

C#:   while (i < 10) { i++; }
来源：http://ksg.jinyuanbaomall.cn

[B08] do-while（至少执行一次）
来源：http://egp.bbcook.cn

Py:   # 无 do-while：用 while True + break
来源：http://ujc.yueranfly.top

PHP:  do { $i++; } while ($i < 10);
来源：http://adg.yfazqb.com

JS:   do { i++; } while (i < 10);
来源：http://tyn.xylfe.cn

TS:   do { i++; } while (i < 10);
来源：http://svw.nwbrower.top

Java: do { i++; } while (i < 10);
来源：http://nsn.quarkkingdee.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ual.0kj1m.cn

Ruby: begin; i += 1; end while i < 10
来源：http://bvy.yj202588.top

C#:   do { i++; } while (i < 10);
来源：http://rlt.jinghuilouyu.cn

[B09] break 与 continue
来源：http://cpd.jianghu66.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bbe.9152youxi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yix.yfazqb.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ixs.daria6918.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wyk.jiagoushi.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wmi.shanyushiyangkeji.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://uez.yfazqb.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nld.quarkkingdee.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://odv.hysaishi.cn

[B10] 遍历同时拿索引
来源：http://ewj.zdqjudy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lrz.iojbl.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tdn.chenzaomai.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://igc.yangfankeji.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tcm.yuxming.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gob.tian-w.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ygr.fanxiaobao.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dww.ybcxt.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rca.zdqjudy.top

[B11] 生成数字序列 / 区间
来源：http://twu.hammf.cn

Py:   list(range(0, 10, 2))
来源：http://xjj.gogol.net.cn

PHP:  range(0, 10, 2);
来源：http://qqv.nanxinkj.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ace.tarul.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kgi.yvedp.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://crv.jiagoushi.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jsm.fehbvm.com

Ruby: (0...10).step(2).to_a
来源：http://sjo.yanxiufei.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lob.jinghuilouyu.cn

[B12] 跳出多层循环
来源：http://fpj.feifeiyinyue.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://tfx.xuanzx.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://gsy.smart0.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gii.9152youxi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mzr.jiagoushi.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wcn.jinqigufen.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://seb.aibaodan.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://thn.ydjk.org.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wuh.feifeiyinyue.top

[B13] 判断是否为数字
来源：http://szs.gzhubu.top

Py:   isinstance(x, (int, float))
来源：http://wkx.shzxlz.cn

PHP:  is_numeric($x)
来源：http://gfc.cqqwz.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wgi.wangdashe.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vnw.bjfxy.top

Java: x instanceof Number
来源：http://uaa.316326.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mnv.xuanzx.com

Ruby: x.is_a?(Numeric)
来源：http://bsa.zdbjq.cn

C#:   x is int or double or decimal
来源：http://nqi.zhixingplan.top

[B14] 判断值是否在集合内
来源：http://pmt.xuetiantiany.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://den.bbcook.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gfa.hammf.cn

JS:   [1, 2, 3].includes(x)
来源：http://ubz.bjfxy.top

TS:   [1, 2, 3].includes(x)
来源：http://ecx.vqdsnc.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qcz.daria6918.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hwr.jiagoushi.top

Ruby: [1, 2, 3].include?(x)
来源：http://fkh.zhiwuduotai.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ght.ydzc1.top

[B15] 布尔运算与取反
来源：http://ftp.vehdjk.com

Py:   a and b or not c
来源：http://fta.vqdsnc.cn

PHP:  $a && $b || !$c
来源：http://tzu.jinyuanbaomall.cn

JS:   a && b || !c
来源：http://ufl.yongpay.top

TS:   a && b || !c
来源：http://qiz.tarul.cn

Java: a && b || !c
来源：http://krf.fktsv.cn

Go:   a && b || !c
来源：http://nzx.shangyingyoupin.top

Ruby: a && b || !c
来源：http://wdd.jinqigufen.top

C#:   a && b || !c
来源：http://mrt.zhengqikj.top

[B16] 卫语句：不满足条件提前返回
来源：http://fsi.jinyuanbaomall.cn

Py:   if not data: return
来源：http://kvy.shangyingyoupin.top

PHP:  if (!$data) { return; }
来源：http://zvm.fehbvm.com

JS:   if (!data) return;
来源：http://bvr.jinghuilouyu.cn

TS:   if (!data) return;
来源：http://lyg.xylfe.cn

Java: if (data == null) return;
来源：http://ser.nwbrower.top

Go:   if data == nil { return }
来源：http://nly.tian-w.cn

Ruby: return if data.nil?
来源：http://qac.bjfxy.top

C#:   if (data == null) return;
来源：http://esi.pengpengdd.cyou

================================================================================
来源：http://ctr.zdbjq.cn

C. 函数与作用域
来源：http://pwb.fanxiaobao.xyz

================================================================================
来源：http://fof.guannengcc.top

[C01] 定义函数
来源：http://jka.zhongyouzk.top

Py:   def add(a, b): return a + b
来源：http://nep.kuanghao11.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xhl.snrcjt.cn

JS:   function add(a, b) { return a + b; }
来源：http://vpz.nanxuanxn.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lox.tian-w.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://nbg.yj20258.top

Go:   func add(a, b int) int { return a + b }
来源：http://euw.ehwqpu.com

Ruby: def add(a, b); a + b; end
来源：http://bap.svipenyu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://buy.ivvv.top

[C02] 默认参数
来源：http://yai.gogol.net.cn

Py:   def greet(name="World"): return name
来源：http://uzq.hongshengwenyu.top

PHP:  function greet($name = "World") { return $name; }
来源：http://gsd.ydjk.org.cn

JS:   function greet(name = "World") { return name; }
来源：http://zxs.sweek.top

TS:   function greet(name: string = "World") { return name; }
来源：http://dwk.yj20258.top

Java: // 无默认参数：方法重载或 Optional
来源：http://exy.shangyingyoupin.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xfy.jqgfzy.top

Ruby: def greet(name = "World") = name
来源：http://iho.gotoacloud.top

C#:   string Greet(string name = "World") => name;
来源：http://sip.guowangkeji.top

[C03] 可变参数
来源：http://ygg.wangshuangyany.cn

Py:   def total(*args): return sum(args)
来源：http://jds.tarul.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kbi.gaohongyu789.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ams.shuidangran.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://snh.xuetiantiany.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://iwa.tian-w.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vaj.shangyingyoupin.top

Ruby: def total(*nums); nums.sum; end
来源：http://iyb.fanxiaobao.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bdi.hysaishi.cn

[C04] 命名参数 / 关键字参数
来源：http://hpl.nwbrower.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://moq.jinghuilouyu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://aid.tanke756.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://umx.9152youxi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cvh.hysaishi.cn

Java: // 无：用 Builder 模式或 record
来源：http://omo.fzhhl.top

Go:   // 无：用配置结构体参数
来源：http://xls.ehwqpu.com

Ruby: f(a: 1, b: 2)
来源：http://pdn.52xcode.cn

C#:   f(a: 1, b: 2)
来源：http://iim.fengsongda.top

[C05] 返回多个值
来源：http://ads.hfpthk.cn

Py:   return a, b
来源：http://kmu.yfazqb.com

PHP:  return [$a, $b];
来源：http://twr.ydjk.org.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dih.hongshengwenyu.top

TS:   return { a, b };
来源：http://ayk.zhixingplan.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cap.bjfxy.top

Go:   return a, b
来源：http://rgg.fanxiaobao.xyz

Ruby: return a, b
来源：http://uks.316326.xyz

C#:   return (a, b);              // ValueTuple
来源：http://yfp.tarul.cn

[C06] 匿名函数 / lambda
来源：http://izt.birdmap.top

Py:   square = lambda x: x * x
来源：http://yoz.hnxiangtu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://bpd.hfpthk.cn

JS:   const square = x => x * x;
来源：http://btf.jianghu66.top

TS:   const square = (x: number): number => x * x;
来源：http://djf.meibo888.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bds.sufxvd.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zdg.guowangkeji.top

Ruby: square = ->(x) { x * x }
来源：http://ddl.andypj.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://rah.cdnleiting.top

[C07] 把函数作为参数传入
来源：http://bwf.dianchejie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yqv.zycfv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ffu.guowangkeji.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xjx.tian-w.cn

TS:   arr.map(String)
来源：http://vix.pengpengdd.cyou

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qvq.daxiang520.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ukv.ybcxt.top

Ruby: arr.map(&:upcase)
来源：http://xbx.gzhubu.top

C#:   arr.Select(s => s.ToUpper())
来源：http://grs.ppjwa.cn

[C08] 闭包
来源：http://wlk.sysykeji.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qjm.dianchejie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wqw.tianlin.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jnj.guannengcc.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://imr.xziqi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://iro.hywenlv.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ado.smart0.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xke.nwbrower.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nap.ehwqpu.com

[C09] 递归
来源：http://xvt.shanyushiyangtech.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tzr.bjfxy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dsx.yj20258.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xfx.yvedp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://akq.nwbrower.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gvh.jinqigfzy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ary.chenlongwang.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rgm.hongshengwenyu.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vcj.ppjwa.cn

[C10] 变量作用域
来源：http://aiv.daria6918.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nad.jyoumei.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pfj.meibo888.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lww.guannengcc.top

TS:   同 JS
来源：http://owu.zdqjudy.top

Java: 方法内为块级作用域
来源：http://uvy.aizwys.cn

Go:   花括号块级作用域
来源：http://alt.cheryme.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jak.jlsjyb.cn

C#:   块级作用域
来源：http://kwt.chenzaomai.com

[C11] 模块导入与导出
来源：http://yxw.yfazqb.com

Py:   from module import func
来源：http://hiw.uphjek.com

PHP:  require "file.php";  或 use App\Service;
来源：http://csw.hcnkem.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://eql.chenlongwang.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jiw.tanke756.top

Java: import java.util.List;
来源：http://lth.aibaodan.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uem.bbcook.cn

Ruby: require "json"; require_relative "./util"
来源：http://mtn.ivvv.top

C#:   using System.Text;
来源：http://gxm.cucudq.cn

[C12] 立即执行函数 IIFE
来源：http://mpu.snrcjt.cn

Py:   (lambda: print("run"))()
来源：http://eyw.jinqigfzy.top

PHP:  (function () { echo "run"; })();
来源：http://ieq.hcnkem.com

JS:   (() => { console.log("run"); })();
来源：http://atb.jlsjyb.cn

TS:   (() => { console.log("run"); })();
来源：http://smg.52xcode.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cgy.zycfv.cn

Go:   func() { fmt.Println("run") }()
来源：http://yvj.ywan-chungtsiang.top

Ruby: -> { puts "run" }.call
来源：http://bob.yanxiufei.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://nzp.aizwys.cn

[C13] 类型声明 / 类型注解
来源：http://rqi.fengsongda.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://itp.52xcode.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kng.hammf.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://aqz.ywan-chungtsiang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://aul.shanyushiyangtech.top

Java: int add(int a, int b) { return a + b; }
来源：http://qqn.cucudq.cn

Go:   func add(a, b int) int
来源：http://lfm.epnwcf.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ona.shzxlz.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fzt.tarul.cn

[C14] 泛型函数
来源：http://hwa.fktsv.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ixz.tarul.cn

PHP:  // 无泛型
来源：http://kly.cucudq.cn

JS:   // 无泛型
来源：http://aqd.guannengcc.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pyu.hcnkem.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://veh.chenjidiqi.icu

Go:   func First[T any](items []T) T { return items[0] }
来源：http://irh.tanke756.top

Ruby: # 无泛型
来源：http://tjn.xingfuxueyuan.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://civ.jinqigufen.top

[C15] 解构 / 展开参数
来源：http://vwc.epnwcf.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fkh.shzxlz.cn

PHP:  [$a, $b] = $pair;
来源：http://hvt.hesvh.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://frg.sweek.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ivo.yj202588.top

Java: // 无解构
来源：http://yme.hnxiangtu.top

Go:   // 无解构
来源：http://vdq.52xcode.cn

Ruby: a, b = pair
来源：http://alf.9152youxi.cn

C#:   var (a, b) = pair;
来源：http://rpl.andypj.xyz

[C16] 函数 / 方法重载
来源：http://eah.jianghu66.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jum.kuanghao11.cn

PHP:  // 无重载
来源：http://moo.yongpay.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://tvm.gzhubu.top

TS:   // 用联合类型或重载签名声明
来源：http://ujb.hnxiangtu.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ise.jianghu66.top

Go:   // 无重载：用不同函数名
来源：http://bfq.yj20258888.top

Ruby: # 无重载：靠动态参数
来源：http://mis.jqgufenzy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://rrk.kuanghao11.cn

================================================================================
来源：http://uzj.chenlongwang.top

D. 数组 / 列表 / 集合
来源：http://wuq.jyoumei.cn

================================================================================
来源：http://opz.tian-w.cn

[D01] 创建数组 / 列表
来源：http://mav.xuanzx.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://gsz.hongshengwenyu.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dul.gogol.net.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dez.zhixingplan.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://tjh.9152youxi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bki.mhx1999.top

Go:   arr := []int{1, 2, 3}
来源：http://dge.jinqigfzy.top

Ruby: arr = [1, 2, 3]
来源：http://qna.andypj.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://uis.xinyue.icu

[D02] 追加元素到末尾
来源：http://rih.chenlongwang.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nhm.dianchejie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://asy.zhaomingkeji.xyz

JS:   arr.push(4);
来源：http://jlg.dianchejie.cn

TS:   arr.push(4);
来源：http://pne.bjfxy.top

Java: list.add(4);
来源：http://ufg.zhixingplan.top

Go:   arr = append(arr, 4)
来源：http://jlf.shzxlz.cn

Ruby: arr << 4; arr.push(5)
来源：http://mwb.wangshuangyany.cn

C#:   list.Add(4);
来源：http://rje.haohaochexian.top

[D03] 在指定位置插入元素
来源：http://xjv.hnqzz.top

Py:   arr.insert(0, 0)
来源：http://swm.fzhhl.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yrq.yfazqb.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://noj.jlsjyb.cn

TS:   arr.splice(0, 0, 0);
来源：http://mbv.ybcxt.top

Java: list.add(0, 0);
来源：http://erd.shanyushiyangtech.top

Go:   arr = append([]int{0}, arr...)
来源：http://exa.xuanzx.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://krw.yueranfly.top

C#:   list.Insert(0, 0);
来源：http://jgu.uphjek.com

[D04] 删除元素
来源：http://orj.zdqjudy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rvs.pycfn.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sae.hammf.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tyq.jqgufenzy.top

TS:   arr.splice(0, 1);
来源：http://jti.jyoumei.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dzb.hnqzz.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ump.bjfxy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wui.jinghuilouyu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hqi.chenzaomai.com

[D05] 访问与修改元素
来源：http://dro.yanxiufei.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yyx.ehwqpu.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pme.cucudq.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bap.feifeiyinyue.top

TS:   arr[0]; arr.at(-1);
来源：http://wir.yanxiufei.cn

Java: list.get(0); list.set(0, 9);
来源：http://upk.xuetiantiany.cn

Go:   arr[0]; arr[0] = 9
来源：http://mwn.yj202588.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ljp.xingfuxueyuan.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rvy.shuidangran.top

[D06] 数组长度
来源：http://bxw.svipenyu.cn

Py:   len(arr)
来源：http://tdh.xuetiantiany.cn

PHP:  count($arr);
来源：http://ulx.fengsongda.top

JS:   arr.length
来源：http://bnw.jlsjyb.cn

TS:   arr.length
来源：http://fup.nwbrower.top

Java: list.size();
来源：http://lde.nwbrower.top

Go:   len(arr)
来源：http://kbi.gaohongyu789.top

Ruby: arr.length; arr.size
来源：http://grr.quarkkingdee.top

C#:   list.Count;
来源：http://ela.mhx1999.top

[D07] 切片 / 取子数组
来源：http://wya.hongshengwenyu.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hic.pycfn.com

PHP:  array_slice($arr, 1, 3);
来源：http://vdc.zhongyouzk.top

JS:   arr.slice(1, 4);
来源：http://rsu.cheryme.top


<!-- 参考信息 -->
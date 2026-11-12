代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://bks.svipenyu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://kht.cashguo.top

JS:   do { i++; } while (i < 10);
来源：http://uef.wangshuangyany.cn

TS:   do { i++; } while (i < 10);
来源：http://yba.smart0.xyz

Java: do { i++; } while (i < 10);
来源：http://ztl.hcnkem.com

Go:   for { i++; if i >= 10 { break } }
来源：http://jol.9152youxi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xlw.hesvh.cn

C#:   do { i++; } while (i < 10);
来源：http://ppd.fzhhl.top

[B09] break 与 continue
来源：http://xcc.xingfuxueyuan.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yqz.snrcjt.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ccw.ivvv.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://llq.xylfe.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://avu.cqqwz.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rmz.yj20258.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nto.ctjpmb.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tmr.nanxuanxn.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jou.yangfankeji.com

[B10] 遍历同时拿索引
来源：http://nso.xylfe.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wpq.0kj1m.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jag.smart0.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ssn.epnwcf.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zoj.yuxming.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://isa.cdnleiting.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uqk.gzhubu.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yyw.nanxinkj.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bom.sjlbkw.cn

[B11] 生成数字序列 / 区间
来源：http://awi.feifeiyinyue.top

Py:   list(range(0, 10, 2))
来源：http://bpi.zycfv.cn

PHP:  range(0, 10, 2);
来源：http://srh.fehbvm.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://smj.nanxinkj.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mak.tian-w.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xxh.daxiang520.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sly.sysykeji.top

Ruby: (0...10).step(2).to_a
来源：http://ciq.yuanzhike.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ded.xuetiantiany.cn

[B12] 跳出多层循环
来源：http://wnd.wangdashe.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://vpc.birdmap.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ggy.zhijiandao.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zfj.yj20258.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dkh.tian-w.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jbk.wangshuangyany.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gqb.hysaishi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zci.tanke756.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sbi.gzhubu.top

[B13] 判断是否为数字
来源：http://wih.jqgfzy.top

Py:   isinstance(x, (int, float))
来源：http://hqk.haohaochexian.top

PHP:  is_numeric($x)
来源：http://hai.ehwqpu.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mtg.xuetiantiany.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://end.tian-w.cn

Java: x instanceof Number
来源：http://jsg.jinghuilouyu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fyg.c1oappe.top

Ruby: x.is_a?(Numeric)
来源：http://jbn.wangdashe.top

C#:   x is int or double or decimal
来源：http://wmw.cdnleiting.top

[B14] 判断值是否在集合内
来源：http://wva.jinghuilouyu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://olc.feifeiyinyue.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jwb.zhoulong.xyz

JS:   [1, 2, 3].includes(x)
来源：http://foh.chenlongwang.top

TS:   [1, 2, 3].includes(x)
来源：http://qrh.birdmap.top

Java: List.of(1, 2, 3).contains(x)
来源：http://zcw.dashuyun.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://otp.dashuyun.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ifk.ivvv.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sey.vehdjk.com

[B15] 布尔运算与取反
来源：http://fxk.ppjwa.cn

Py:   a and b or not c
来源：http://znu.sweek.top

PHP:  $a && $b || !$c
来源：http://kpi.hongshengwenyu.top

JS:   a && b || !c
来源：http://ond.zycfv.cn

TS:   a && b || !c
来源：http://xry.vqdsnc.cn

Java: a && b || !c
来源：http://jch.aibaodan.cn

Go:   a && b || !c
来源：http://uje.ctjpmb.com

Ruby: a && b || !c
来源：http://gqu.aizwys.cn

C#:   a && b || !c
来源：http://nws.zdbjq.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fau.chenlongwang.top

Py:   if not data: return
来源：http://yut.chenjidiqi.icu

PHP:  if (!$data) { return; }
来源：http://odx.guowangkeji.top

JS:   if (!data) return;
来源：http://swu.yangfankeji.com

TS:   if (!data) return;
来源：http://qzj.guannengcc.top

Java: if (data == null) return;
来源：http://rni.shangyingyoupin.top

Go:   if data == nil { return }
来源：http://stb.pengpengdd.cyou

Ruby: return if data.nil?
来源：http://lfo.hnqzz.top

C#:   if (data == null) return;
来源：http://thj.tian-w.cn

================================================================================
来源：http://qts.dashuyun.cn

C. 函数与作用域
来源：http://idt.xylfe.cn

================================================================================
来源：http://our.xinyue.icu

[C01] 定义函数
来源：http://alt.haohaochexian.top

Py:   def add(a, b): return a + b
来源：http://gia.xuanzx.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zqp.jinqigufen.top

JS:   function add(a, b) { return a + b; }
来源：http://ehr.shanyushiyangtech.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hds.316326.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://icq.cqqwz.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ydb.yanxiufei.cn

Ruby: def add(a, b); a + b; end
来源：http://lgp.xinyue.icu

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qvc.cucudq.cn

[C02] 默认参数
来源：http://gcz.wangshuangyany.cn

Py:   def greet(name="World"): return name
来源：http://gbh.jqgufenzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ave.hongshengwenyu.top

JS:   function greet(name = "World") { return name; }
来源：http://qhb.hcnkem.com

TS:   function greet(name: string = "World") { return name; }
来源：http://qfp.yueranfly.top

Java: // 无默认参数：方法重载或 Optional
来源：http://myv.kuanghao11.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ber.ehwqpu.com

Ruby: def greet(name = "World") = name
来源：http://ijl.yongpay.top

C#:   string Greet(string name = "World") => name;
来源：http://vgd.yvedp.cn

[C03] 可变参数
来源：http://odn.sweek.top

Py:   def total(*args): return sum(args)
来源：http://ihn.xinyue.icu

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qkf.shzxlz.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cak.0kj1m.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ptv.bjfxy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bhk.chenzaomai.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://aik.zhaomingkeji.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://ywo.haohaochexian.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hjd.mhx1999.top

[C04] 命名参数 / 关键字参数
来源：http://kau.nwbrower.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://eqe.cqqwz.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rog.shangyingyoupin.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wjf.hysaishi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://btf.yuxming.cn

Java: // 无：用 Builder 模式或 record
来源：http://iwo.cqqwz.cn

Go:   // 无：用配置结构体参数
来源：http://jte.nanxinkj.top

Ruby: f(a: 1, b: 2)
来源：http://box.shuidangran.top

C#:   f(a: 1, b: 2)
来源：http://upk.gogol.net.cn

[C05] 返回多个值
来源：http://qxi.xylfe.cn

Py:   return a, b
来源：http://sjy.chenzaomai.com

PHP:  return [$a, $b];
来源：http://zxv.jinyuanbaomall.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qil.yangfankeji.com

TS:   return { a, b };
来源：http://xyp.haohaochexian.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://egi.ywan-chungtsiang.top

Go:   return a, b
来源：http://kvt.fanxiaobao.xyz

Ruby: return a, b
来源：http://ikk.0kj1m.cn

C#:   return (a, b);              // ValueTuple
来源：http://zkv.9152youxi.cn

[C06] 匿名函数 / lambda
来源：http://zjb.yj20258888.top

Py:   square = lambda x: x * x
来源：http://jdt.quarkkingdee.top

PHP:  $square = fn($x) => $x * $x;
来源：http://jtn.daria6918.cn

JS:   const square = x => x * x;
来源：http://wel.zhongyouzk.top

TS:   const square = (x: number): number => x * x;
来源：http://kus.xuetiantiany.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zah.jlsjyb.cn

Go:   sq := func(x int) int { return x * x }
来源：http://lne.jianghu66.top

Ruby: square = ->(x) { x * x }
来源：http://gkp.sweek.top

C#:   Func<int, int> square = x => x * x;
来源：http://uhn.hammf.cn

[C07] 把函数作为参数传入
来源：http://osv.sweek.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ksh.fktsv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://nqp.tianlin.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ryn.jlsjyb.cn

TS:   arr.map(String)
来源：http://lbm.snrcjt.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://itf.dashuyun.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://phv.uphjek.com

Ruby: arr.map(&:upcase)
来源：http://qth.tarul.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://npr.yj202588.top

[C08] 闭包
来源：http://xow.gzhubu.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tol.yongpay.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ssf.kuanghao11.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ooz.bjfxy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://giq.zdbjq.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vfa.gogol.net.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kws.ydzc1.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qin.jlsjyb.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mhf.zhaomingkeji.xyz

[C09] 递归
来源：http://ivn.fengsongda.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ycj.ywan-chungtsiang.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cmq.hammf.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tsv.fehbvm.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qkd.shuidangran.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://apt.yuanzhike.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kgv.haohaochexian.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wvf.xylfe.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zxn.gzhubu.top

[C10] 变量作用域
来源：http://adc.sxryk.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zym.zhengqikj.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dea.hysaishi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yvv.hfpthk.cn

TS:   同 JS
来源：http://hrd.shanyushiyangkeji.top

Java: 方法内为块级作用域
来源：http://vmo.jlsjyb.cn

Go:   花括号块级作用域
来源：http://pjs.yueranfly.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://icb.wangdashe.top

C#:   块级作用域
来源：http://ygi.dashuyun.cn

[C11] 模块导入与导出
来源：http://ozq.bjfxy.top

Py:   from module import func
来源：http://cqo.tarul.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bnj.zhengqikj.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://eav.cucudq.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wcb.zdqjudy.top

Java: import java.util.List;
来源：http://qof.meibo888.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://aqc.hnqzz.top

Ruby: require "json"; require_relative "./util"
来源：http://hrd.ydjk.org.cn

C#:   using System.Text;
来源：http://azv.vehdjk.com

[C12] 立即执行函数 IIFE
来源：http://iot.yueranfly.top

Py:   (lambda: print("run"))()
来源：http://akw.xylfe.cn

PHP:  (function () { echo "run"; })();
来源：http://pyx.yongpay.top

JS:   (() => { console.log("run"); })();
来源：http://dsf.ywan-chungtsiang.top

TS:   (() => { console.log("run"); })();
来源：http://kis.zhiwuduotai.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jiv.snrcjt.cn

Go:   func() { fmt.Println("run") }()
来源：http://xld.daxiang520.top

Ruby: -> { puts "run" }.call
来源：http://oyt.zdbjq.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xoq.zhixingplan.top

[C13] 类型声明 / 类型注解
来源：http://gyk.sweek.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ekx.snrcjt.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gmr.yvedp.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://aqh.xylfe.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://igo.nanxinkj.top

Java: int add(int a, int b) { return a + b; }
来源：http://yul.ivvv.top

Go:   func add(a, b int) int
来源：http://tbk.9152youxi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ykq.xingfuxueyuan.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://zsw.yonumen.top

[C14] 泛型函数
来源：http://tjd.gzhubu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fpp.tian-w.cn

PHP:  // 无泛型
来源：http://gyg.daxiang520.top

JS:   // 无泛型
来源：http://yba.yanxiufei.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qek.mhx1999.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lgu.yuanzhike.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nzx.wangdashe.top

Ruby: # 无泛型
来源：http://rcm.shzxlz.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ufi.ehwqpu.com

[C15] 解构 / 展开参数
来源：http://xbp.c1oappe.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rgp.snrcjt.cn

PHP:  [$a, $b] = $pair;
来源：http://gwk.fehbvm.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://oyi.zhaomingkeji.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gzq.hysaishi.cn

Java: // 无解构
来源：http://fdt.gogol.net.cn

Go:   // 无解构
来源：http://nwl.shzxlz.cn

Ruby: a, b = pair
来源：http://xnd.xziqi.cn

C#:   var (a, b) = pair;
来源：http://xaw.yfazqb.com

[C16] 函数 / 方法重载
来源：http://qdu.hnxiangtu.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ziq.jyoumei.cn

PHP:  // 无重载
来源：http://ztt.gzhubu.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://iel.ehwqpu.com

TS:   // 用联合类型或重载签名声明
来源：http://uqh.zhiwuduotai.top

Java: void f(int a) {}  void f(String a) {}
来源：http://vub.52xcode.cn

Go:   // 无重载：用不同函数名
来源：http://vgo.fzhhl.top

Ruby: # 无重载：靠动态参数
来源：http://oua.zhongyouzk.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://uds.sjlbkw.cn

================================================================================
来源：http://psc.fanxiaobao.xyz

D. 数组 / 列表 / 集合
来源：http://gao.cqqwz.cn

================================================================================
来源：http://nfd.wangdashe.top

[D01] 创建数组 / 列表
来源：http://dng.smart0.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://zaj.nanxuanxn.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pjo.zdbjq.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uwl.pengpengdd.cyou

TS:   const arr: number[] = [1, 2, 3];
来源：http://cvv.hcnkem.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vdg.chenlongwang.top

Go:   arr := []int{1, 2, 3}
来源：http://ofj.ppjwa.cn

Ruby: arr = [1, 2, 3]
来源：http://lkl.hfpthk.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fwm.kuanghao11.cn

[D02] 追加元素到末尾
来源：http://eov.tanke756.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yrm.0kj1m.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yxt.nanxinkj.top

JS:   arr.push(4);
来源：http://psy.zhongyouzk.top

TS:   arr.push(4);
来源：http://ubl.zhixingplan.top

Java: list.add(4);
来源：http://ygr.kuanghao11.cn

Go:   arr = append(arr, 4)
来源：http://vkr.haohaochexian.top

Ruby: arr << 4; arr.push(5)
来源：http://esg.ivvv.top

C#:   list.Add(4);
来源：http://ixa.jyoumei.cn

[D03] 在指定位置插入元素
来源：http://wii.shangyingyoupin.top

Py:   arr.insert(0, 0)
来源：http://jhz.sysykeji.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gjc.shanyushiyangkeji.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cvh.bbcook.cn

TS:   arr.splice(0, 0, 0);
来源：http://geu.hfpthk.cn

Java: list.add(0, 0);
来源：http://pxh.feifeiyinyue.top

Go:   arr = append([]int{0}, arr...)
来源：http://afv.jinqigufen.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vwe.meibo888.top

C#:   list.Insert(0, 0);
来源：http://hqa.fzhhl.top

[D04] 删除元素
来源：http://pro.smart0.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jdd.pycfn.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xkw.xingfuxueyuan.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://myp.jinqigfzy.top

TS:   arr.splice(0, 1);
来源：http://sap.cashguo.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lub.zhiwuduotai.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hwv.gzhubu.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bcx.hnqzz.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hbb.jinghuilouyu.cn

[D05] 访问与修改元素
来源：http://tvp.zhiwuduotai.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vbi.c1oappe.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://oei.hfpthk.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bqf.gotoacloud.top

TS:   arr[0]; arr.at(-1);
来源：http://yya.tian-w.cn

Java: list.get(0); list.set(0, 9);
来源：http://htf.ivvv.top

Go:   arr[0]; arr[0] = 9
来源：http://zlv.hesvh.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vcb.xuetiantiany.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qop.zhixingplan.top

[D06] 数组长度
来源：http://bdd.vehdjk.com

Py:   len(arr)
来源：http://fsf.shanyushiyangkeji.top

PHP:  count($arr);
来源：http://rhy.havefunace.top

JS:   arr.length
来源：http://pgf.jiagoushi.top

TS:   arr.length
来源：http://fbg.feifeiyinyue.top

Java: list.size();
来源：http://tyk.gaohongyu789.top

Go:   len(arr)
来源：http://kir.mhx1999.top

Ruby: arr.length; arr.size
来源：http://cvd.zycfv.cn

C#:   list.Count;
来源：http://flc.cashguo.top

[D07] 切片 / 取子数组
来源：http://ahc.cqqwz.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hzd.xinyue.icu

PHP:  array_slice($arr, 1, 3);
来源：http://jml.cashguo.top

JS:   arr.slice(1, 4);
来源：http://pqb.zhaomingkeji.xyz

TS:   arr.slice(1, 4);
来源：http://zmb.fktsv.cn

Java: list.subList(1, 4);
来源：http://anu.haohaochexian.top

Go:   arr[1:4]
来源：http://lzn.zhoulong.xyz

Ruby: arr[1, 3]
来源：http://yhp.aibaodan.cn

C#:   list.GetRange(1, 3);
来源：http://yep.xuanzx.com

[D08] 合并两个数组
来源：http://riw.sysykeji.top

Py:   a + b;  a.extend(b)
来源：http://pau.ywan-chungtsiang.top

PHP:  array_merge($a, $b);
来源：http://fsz.epnwcf.com

JS:   [...a, ...b];  a.concat(b);
来源：http://tdt.kuanghao11.cn

TS:   [...a, ...b];
来源：http://adl.hcnkem.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vhp.ydjk.org.cn

Go:   append(a, b...)
来源：http://zcz.sxryk.cn


<!-- 参考信息 -->
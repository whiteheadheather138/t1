代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://zsb.sjlbkw.cn

JS:   while (i < 10) { i++; }
来源：http://fmo.c1oappe.top

TS:   while (i < 10) { i++; }
来源：http://aoz.yueranfly.top

Java: while (i < 10) { i++; }
来源：http://gab.gzhubu.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rta.fehbvm.com

Ruby: while i < 10; i += 1; end
来源：http://lrs.zdqjudy.top

C#:   while (i < 10) { i++; }
来源：http://clj.chenjidiqi.icu

[B08] do-while（至少执行一次）
来源：http://uqd.jqgfzy.top

Py:   # 无 do-while：用 while True + break
来源：http://eqo.fanxiaobao.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://wcg.fehbvm.com

JS:   do { i++; } while (i < 10);
来源：http://yrj.gotoacloud.top

TS:   do { i++; } while (i < 10);
来源：http://feh.nanxuanxn.top

Java: do { i++; } while (i < 10);
来源：http://jyg.zycfv.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://baf.bjfxy.top

Ruby: begin; i += 1; end while i < 10
来源：http://sch.jinghuilouyu.cn

C#:   do { i++; } while (i < 10);
来源：http://bcj.pengpengdd.cyou

[B09] break 与 continue
来源：http://itl.epnwcf.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bns.tian-w.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wfc.cqqwz.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bwf.jianghu66.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cbe.wangdashe.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zmw.guannengcc.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yaq.andypj.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ywn.jyoumei.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://atp.snrcjt.cn

[B10] 遍历同时拿索引
来源：http://irc.yanxiufei.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rxq.hnxiangtu.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dip.bjfxy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jud.andypj.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xyr.jlsjyb.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mff.svipenyu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://njc.redwolf501.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ijc.hcnkem.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ycv.xingfuxueyuan.xyz

[B11] 生成数字序列 / 区间
来源：http://qks.jqgfzy.top

Py:   list(range(0, 10, 2))
来源：http://cee.jinqigfzy.top

PHP:  range(0, 10, 2);
来源：http://iii.zhengqikj.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fxy.yonumen.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vzq.jinghuilouyu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mwt.cheryme.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://loi.fanxiaobao.xyz

Ruby: (0...10).step(2).to_a
来源：http://iaz.ydzc1.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nfl.shuidangran.top

[B12] 跳出多层循环
来源：http://teu.sweek.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://woh.nanxuanxn.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://lrk.aibaodan.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xfy.zycfv.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ooh.meibo888.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yze.dianchejie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cpc.smart0.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dkm.nanxuanxn.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://omq.xingfuxueyuan.xyz

[B13] 判断是否为数字
来源：http://kvz.nanxuanxn.top

Py:   isinstance(x, (int, float))
来源：http://fys.bjfxy.top

PHP:  is_numeric($x)
来源：http://ytf.zhongyouzk.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pwv.redwolf501.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iny.shanyushiyangtech.top

Java: x instanceof Number
来源：http://prf.gogol.net.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rzf.gzhubu.top

Ruby: x.is_a?(Numeric)
来源：http://nzb.feifeiyinyue.top

C#:   x is int or double or decimal
来源：http://nhq.chenzaomai.com

[B14] 判断值是否在集合内
来源：http://gjf.zycfv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zth.fehbvm.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mvc.xuetiantiany.cn

JS:   [1, 2, 3].includes(x)
来源：http://xis.yueranfly.top

TS:   [1, 2, 3].includes(x)
来源：http://rfy.gaohongyu789.top

Java: List.of(1, 2, 3).contains(x)
来源：http://idh.guannengcc.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mnh.hammf.cn

Ruby: [1, 2, 3].include?(x)
来源：http://iyl.feifeiyinyue.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://osq.iojbl.cn

[B15] 布尔运算与取反
来源：http://sow.fzhhl.top

Py:   a and b or not c
来源：http://cvx.yvedp.cn

PHP:  $a && $b || !$c
来源：http://kky.ywan-chungtsiang.top

JS:   a && b || !c
来源：http://das.jlsjyb.cn

TS:   a && b || !c
来源：http://tqy.c1oappe.top

Java: a && b || !c
来源：http://bbl.andypj.xyz

Go:   a && b || !c
来源：http://zaf.shanyushiyangtech.top

Ruby: a && b || !c
来源：http://oat.52xcode.cn

C#:   a && b || !c
来源：http://dlz.hesvh.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jtj.yonumen.top

Py:   if not data: return
来源：http://zfl.pycfn.com

PHP:  if (!$data) { return; }
来源：http://mjh.yvedp.cn

JS:   if (!data) return;
来源：http://ljx.fzhhl.top

TS:   if (!data) return;
来源：http://svi.yueranfly.top

Java: if (data == null) return;
来源：http://fqm.dashuyun.cn

Go:   if data == nil { return }
来源：http://hgm.yj20258.top

Ruby: return if data.nil?
来源：http://oku.yuxming.cn

C#:   if (data == null) return;
来源：http://lld.9152youxi.cn

================================================================================
来源：http://giv.aizwys.cn

C. 函数与作用域
来源：http://ihp.andypj.xyz

================================================================================
来源：http://djc.yj202588.top

[C01] 定义函数
来源：http://gnq.snrcjt.cn

Py:   def add(a, b): return a + b
来源：http://min.cucudq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://epi.svipenyu.cn

JS:   function add(a, b) { return a + b; }
来源：http://trb.jqgfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ohv.xinyue.icu

Java: static int add(int a, int b) { return a + b; }
来源：http://eaf.yuxming.cn

Go:   func add(a, b int) int { return a + b }
来源：http://iac.9152youxi.cn

Ruby: def add(a, b); a + b; end
来源：http://ebj.shangyingyoupin.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://utu.jiagoushi.top

[C02] 默认参数
来源：http://qya.hnxiangtu.top

Py:   def greet(name="World"): return name
来源：http://zqx.hnxiangtu.top

PHP:  function greet($name = "World") { return $name; }
来源：http://sme.sufxvd.cn

JS:   function greet(name = "World") { return name; }
来源：http://slp.ivvv.top

TS:   function greet(name: string = "World") { return name; }
来源：http://won.shangyingyoupin.top

Java: // 无默认参数：方法重载或 Optional
来源：http://gbw.jqgufenzy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ddr.fengsongda.top

Ruby: def greet(name = "World") = name
来源：http://vso.nanxinkj.top

C#:   string Greet(string name = "World") => name;
来源：http://eyw.jqgufenzy.top

[C03] 可变参数
来源：http://kxt.haohaochexian.top

Py:   def total(*args): return sum(args)
来源：http://hno.jinghuilouyu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ebp.gzhubu.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://uxz.jinqigufen.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://oon.aibaodan.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hrj.ppjwa.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://iee.sweek.top

Ruby: def total(*nums); nums.sum; end
来源：http://mdi.gogol.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zbp.shuidangran.top

[C04] 命名参数 / 关键字参数
来源：http://tol.bjfxy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://efo.bbcook.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gwu.jqgufenzy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wir.jinyuanbaomall.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bno.jlsjyb.cn

Java: // 无：用 Builder 模式或 record
来源：http://rjb.snrcjt.cn

Go:   // 无：用配置结构体参数
来源：http://ejw.guowangkeji.top

Ruby: f(a: 1, b: 2)
来源：http://cpe.jqgfzy.top

C#:   f(a: 1, b: 2)
来源：http://lzk.iojbl.cn

[C05] 返回多个值
来源：http://msh.tian-w.cn

Py:   return a, b
来源：http://hbg.fanxiaobao.xyz

PHP:  return [$a, $b];
来源：http://wsv.dashuyun.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xoe.cdnleiting.top

TS:   return { a, b };
来源：http://ter.shuidangran.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sal.gotoacloud.top

Go:   return a, b
来源：http://dhq.aizwys.cn

Ruby: return a, b
来源：http://zvg.fktsv.cn

C#:   return (a, b);              // ValueTuple
来源：http://wvh.shuidangran.top

[C06] 匿名函数 / lambda
来源：http://yij.yj20258.top

Py:   square = lambda x: x * x
来源：http://svc.sjlbkw.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ijt.nwbrower.top

JS:   const square = x => x * x;
来源：http://tel.xinyue.icu

TS:   const square = (x: number): number => x * x;
来源：http://wjw.cashguo.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nze.nwbrower.top

Go:   sq := func(x int) int { return x * x }
来源：http://wat.ivvv.top

Ruby: square = ->(x) { x * x }
来源：http://bjn.chenlongwang.top

C#:   Func<int, int> square = x => x * x;
来源：http://cbh.wangdashe.top

[C07] 把函数作为参数传入
来源：http://wdu.yvedp.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fjj.jinghuilouyu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ubo.bjfxy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ies.daxiang520.top

TS:   arr.map(String)
来源：http://mpi.zycfv.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yxv.yj20258888.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gbl.andypj.xyz

Ruby: arr.map(&:upcase)
来源：http://ozp.uphjek.com

C#:   arr.Select(s => s.ToUpper())
来源：http://ycp.jinghuilouyu.cn

[C08] 闭包
来源：http://ext.andypj.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uch.aibaodan.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cbx.vqdsnc.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yzf.9152youxi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nem.yvedp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mgo.jqgfzy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ptf.sweek.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vgv.jinyuanbaomall.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fsr.cdnleiting.top

[C09] 递归
来源：http://qrl.pycfn.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rgh.svipenyu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mub.hcnkem.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hbt.iojbl.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://utf.hnqzz.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mpa.ywan-chungtsiang.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kpa.yonumen.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://edh.wangshuangyany.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hak.zhiwuduotai.top

[C10] 变量作用域
来源：http://fgq.ehwqpu.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tkm.c1oappe.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://scs.kuanghao11.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mae.zhongyouzk.top

TS:   同 JS
来源：http://ldc.cdnleiting.top

Java: 方法内为块级作用域
来源：http://qyp.vehdjk.com

Go:   花括号块级作用域
来源：http://abk.52xcode.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hcy.shanyushiyangkeji.top

C#:   块级作用域
来源：http://tct.hnxiangtu.top

[C11] 模块导入与导出
来源：http://ohc.ehwqpu.com

Py:   from module import func
来源：http://dfr.ppjwa.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xxk.uphjek.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://ptq.pycfn.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cqg.hnxiangtu.top

Java: import java.util.List;
来源：http://diz.chenzaomai.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://syw.xuetiantiany.cn

Ruby: require "json"; require_relative "./util"
来源：http://hld.daxiang520.top

C#:   using System.Text;
来源：http://ewq.cqqwz.cn

[C12] 立即执行函数 IIFE
来源：http://rhz.daria6918.cn

Py:   (lambda: print("run"))()
来源：http://rhy.xuanzx.com

PHP:  (function () { echo "run"; })();
来源：http://fkt.hammf.cn

JS:   (() => { console.log("run"); })();
来源：http://kbq.andypj.xyz

TS:   (() => { console.log("run"); })();
来源：http://nul.bbcook.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://byz.pycfn.com

Go:   func() { fmt.Println("run") }()
来源：http://tfr.ywan-chungtsiang.top

Ruby: -> { puts "run" }.call
来源：http://efv.bbcook.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qes.mhx1999.top

[C13] 类型声明 / 类型注解
来源：http://fwa.yongpay.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zit.shanyushiyangtech.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jwa.tarul.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sgj.nanxinkj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lsh.bjfxy.top

Java: int add(int a, int b) { return a + b; }
来源：http://vqw.chenzaomai.com

Go:   func add(a, b int) int
来源：http://lml.zdbjq.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rxt.hongshengwenyu.top

C#:   int Add(int a, int b) => a + b;
来源：http://gxw.redwolf501.top

[C14] 泛型函数
来源：http://xeb.havefunace.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nvw.jinghuilouyu.cn

PHP:  // 无泛型
来源：http://rbo.guowangkeji.top

JS:   // 无泛型
来源：http://fkf.yueranfly.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vdy.9152youxi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tco.ctjpmb.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lrj.cdnleiting.top

Ruby: # 无泛型
来源：http://xdx.dashuyun.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://uwb.guowangkeji.top

[C15] 解构 / 展开参数
来源：http://qqb.aibaodan.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://aqc.jinqigfzy.top

PHP:  [$a, $b] = $pair;
来源：http://qva.aibaodan.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zvm.ybcxt.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vke.gotoacloud.top

Java: // 无解构
来源：http://rne.tianlin.xyz

Go:   // 无解构
来源：http://wfc.epnwcf.com

Ruby: a, b = pair
来源：http://hqp.yfazqb.com

C#:   var (a, b) = pair;
来源：http://nwy.daria6918.cn

[C16] 函数 / 方法重载
来源：http://ats.zhoulong.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://abj.cashguo.top

PHP:  // 无重载
来源：http://hhc.ppjwa.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zyg.yuanzhike.top

TS:   // 用联合类型或重载签名声明
来源：http://kex.xinyue.icu

Java: void f(int a) {}  void f(String a) {}
来源：http://fmm.jlsjyb.cn

Go:   // 无重载：用不同函数名
来源：http://huv.yj202588.top

Ruby: # 无重载：靠动态参数
来源：http://uyq.yj20258888.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ike.shangyingyoupin.top

================================================================================
来源：http://sjb.pycfn.com

D. 数组 / 列表 / 集合
来源：http://ooi.jqgufenzy.top

================================================================================
来源：http://wih.epnwcf.com

[D01] 创建数组 / 列表
来源：http://eyi.zhiwuduotai.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://isn.gaohongyu789.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://klk.shuidangran.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vug.xylfe.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dwx.nanxuanxn.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qze.jlsjyb.cn

Go:   arr := []int{1, 2, 3}
来源：http://ydk.ctjpmb.com

Ruby: arr = [1, 2, 3]
来源：http://paw.cashguo.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rdw.yuanzhike.top

[D02] 追加元素到末尾
来源：http://klm.chenjidiqi.icu

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qwz.chenlongwang.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yww.snrcjt.cn

JS:   arr.push(4);
来源：http://vwa.yanxiufei.cn

TS:   arr.push(4);
来源：http://teq.hywenlv.cn

Java: list.add(4);
来源：http://efs.jqgfzy.top

Go:   arr = append(arr, 4)
来源：http://mlx.zhengqikj.top

Ruby: arr << 4; arr.push(5)
来源：http://mxy.xylfe.cn

C#:   list.Add(4);
来源：http://tmk.dashuyun.cn

[D03] 在指定位置插入元素
来源：http://lzq.xylfe.cn

Py:   arr.insert(0, 0)
来源：http://gjj.yueranfly.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cdt.jqgfzy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://skp.haohaochexian.top

TS:   arr.splice(0, 0, 0);
来源：http://qbj.hcnkem.com

Java: list.add(0, 0);
来源：http://snf.chenlongwang.top

Go:   arr = append([]int{0}, arr...)
来源：http://skm.mhx1999.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wbj.sysykeji.top

C#:   list.Insert(0, 0);
来源：http://ssw.jinghuilouyu.cn

[D04] 删除元素
来源：http://zqm.daria6918.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tlt.zdqjudy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mwf.zhiwuduotai.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wfc.jinyuanbaomall.cn

TS:   arr.splice(0, 1);
来源：http://sff.nanxuanxn.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://itf.zhengqikj.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lfx.cashguo.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ftr.tarul.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bzp.ydzc1.top

[D05] 访问与修改元素
来源：http://klz.jiagoushi.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://awa.xuetiantiany.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://itr.iojbl.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://eog.hfpthk.cn

TS:   arr[0]; arr.at(-1);
来源：http://duq.ivvv.top

Java: list.get(0); list.set(0, 9);
来源：http://gyi.guannengcc.top

Go:   arr[0]; arr[0] = 9
来源：http://fsr.zdqjudy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mgg.ivvv.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://oxq.sxryk.cn

[D06] 数组长度
来源：http://nzm.mhx1999.top

Py:   len(arr)
来源：http://asz.jianghu66.top

PHP:  count($arr);
来源：http://xey.zhongyouzk.top

JS:   arr.length
来源：http://ewo.yj20258888.top

TS:   arr.length
来源：http://nmw.nanxinkj.top

Java: list.size();
来源：http://ugx.uphjek.com

Go:   len(arr)
来源：http://ext.yvedp.cn

Ruby: arr.length; arr.size
来源：http://mxk.mhx1999.top

C#:   list.Count;
来源：http://uap.hfpthk.cn

[D07] 切片 / 取子数组
来源：http://xlg.nanxinkj.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://opr.tianlin.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://lhx.shuidangran.top

JS:   arr.slice(1, 4);
来源：http://gbu.ctjpmb.com

TS:   arr.slice(1, 4);
来源：http://djs.snrcjt.cn

Java: list.subList(1, 4);
来源：http://feg.birdmap.top

Go:   arr[1:4]
来源：http://guq.feifeiyinyue.top

Ruby: arr[1, 3]
来源：http://qfv.hnxiangtu.top


<!-- 参考信息 -->
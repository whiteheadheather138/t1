代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mlj.daria6918.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lhq.tarul.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rhd.ywan-chungtsiang.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vel.xuetiantiany.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jwo.tarul.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hbu.ywan-chungtsiang.top

[B07] while 循环
来源：http://opy.gzhubu.top

Py:   while i < 10: i += 1
来源：http://rto.yvedp.cn

PHP:  while ($i < 10) { $i++; }
来源：http://iwk.redwolf501.top

JS:   while (i < 10) { i++; }
来源：http://pak.yfazqb.com

TS:   while (i < 10) { i++; }
来源：http://nyd.ehwqpu.com

Java: while (i < 10) { i++; }
来源：http://bbc.fzhhl.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mqn.nanxinkj.top

Ruby: while i < 10; i += 1; end
来源：http://mfk.jinghuilouyu.cn

C#:   while (i < 10) { i++; }
来源：http://qzv.wangdashe.top

[B08] do-while（至少执行一次）
来源：http://bda.yvedp.cn

Py:   # 无 do-while：用 while True + break
来源：http://icl.yfazqb.com

PHP:  do { $i++; } while ($i < 10);
来源：http://heh.yj20258.top

JS:   do { i++; } while (i < 10);
来源：http://uct.dianchejie.cn

TS:   do { i++; } while (i < 10);
来源：http://uoi.shzxlz.cn

Java: do { i++; } while (i < 10);
来源：http://jyx.xinyue.icu

Go:   for { i++; if i >= 10 { break } }
来源：http://tos.chenlongwang.top

Ruby: begin; i += 1; end while i < 10
来源：http://kuh.ywan-chungtsiang.top

C#:   do { i++; } while (i < 10);
来源：http://ter.yanxiufei.cn

[B09] break 与 continue
来源：http://cnz.zhijiandao.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xgq.zdbjq.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://swn.hfpthk.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://utx.fzhhl.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sui.yvedp.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qgp.ybcxt.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sng.wangdashe.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ldq.bjfxy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gwq.smart0.xyz

[B10] 遍历同时拿索引
来源：http://fxq.chenzaomai.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wlx.hfpthk.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qpd.xuetiantiany.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rrf.epnwcf.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qeg.yanxiufei.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ntb.quarkkingdee.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://aag.xinyue.icu

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ajs.0kj1m.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jdl.zhiwuduotai.top

[B11] 生成数字序列 / 区间
来源：http://tgh.sjlbkw.cn

Py:   list(range(0, 10, 2))
来源：http://syx.yanxiufei.cn

PHP:  range(0, 10, 2);
来源：http://xia.mhx1999.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fkr.vqdsnc.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dyj.hnqzz.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fzh.birdmap.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jpj.guowangkeji.top

Ruby: (0...10).step(2).to_a
来源：http://imc.tianlin.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cpx.cucudq.cn

[B12] 跳出多层循环
来源：http://qnf.yangfankeji.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://oyt.jianghu66.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://pjj.zdbjq.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ect.chenlongwang.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://eoz.nwbrower.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rfi.fengsongda.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lhv.ydjk.org.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://frz.haohaochexian.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://niz.jiagoushi.top

[B13] 判断是否为数字
来源：http://kza.vehdjk.com

Py:   isinstance(x, (int, float))
来源：http://rxw.iojbl.cn

PHP:  is_numeric($x)
来源：http://zhz.hywenlv.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://boj.haohaochexian.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jdk.ywan-chungtsiang.top

Java: x instanceof Number
来源：http://gpj.fengsongda.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ecl.fengsongda.top

Ruby: x.is_a?(Numeric)
来源：http://hsc.iojbl.cn

C#:   x is int or double or decimal
来源：http://jnw.jqgfzy.top

[B14] 判断值是否在集合内
来源：http://ugv.epnwcf.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xdo.cqqwz.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zry.hammf.cn

JS:   [1, 2, 3].includes(x)
来源：http://dwk.hesvh.cn

TS:   [1, 2, 3].includes(x)
来源：http://cwc.jlsjyb.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ogq.52xcode.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pzr.xinyue.icu

Ruby: [1, 2, 3].include?(x)
来源：http://ffq.guowangkeji.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qlg.dianchejie.cn

[B15] 布尔运算与取反
来源：http://zsu.gaohongyu789.top

Py:   a and b or not c
来源：http://amv.yangfankeji.com

PHP:  $a && $b || !$c
来源：http://kfp.yj20258.top

JS:   a && b || !c
来源：http://zyv.iojbl.cn

TS:   a && b || !c
来源：http://mqt.aizwys.cn

Java: a && b || !c
来源：http://arn.sweek.top

Go:   a && b || !c
来源：http://kyj.hcnkem.com

Ruby: a && b || !c
来源：http://nea.daria6918.cn

C#:   a && b || !c
来源：http://fmc.pengpengdd.cyou

[B16] 卫语句：不满足条件提前返回
来源：http://xeu.yuanzhike.top

Py:   if not data: return
来源：http://lmv.ywan-chungtsiang.top

PHP:  if (!$data) { return; }
来源：http://lsh.nanxuanxn.top

JS:   if (!data) return;
来源：http://wdv.zhongyouzk.top

TS:   if (!data) return;
来源：http://gcf.cheryme.top

Java: if (data == null) return;
来源：http://lmp.ppjwa.cn

Go:   if data == nil { return }
来源：http://qeb.shanyushiyangtech.top

Ruby: return if data.nil?
来源：http://lvd.jqgfzy.top

C#:   if (data == null) return;
来源：http://fto.daxiang520.top

================================================================================
来源：http://xpw.redwolf501.top

C. 函数与作用域
来源：http://fqc.zhixingplan.top

================================================================================
来源：http://cre.ivvv.top

[C01] 定义函数
来源：http://ooa.daxiang520.top

Py:   def add(a, b): return a + b
来源：http://cwa.xylfe.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lxv.jinqigufen.top

JS:   function add(a, b) { return a + b; }
来源：http://xyg.yfazqb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yvf.0kj1m.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://yau.dianchejie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zxo.shzxlz.cn

Ruby: def add(a, b); a + b; end
来源：http://leo.fanxiaobao.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xgs.havefunace.top

[C02] 默认参数
来源：http://gmz.vehdjk.com

Py:   def greet(name="World"): return name
来源：http://bek.vqdsnc.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lpv.cqqwz.cn

JS:   function greet(name = "World") { return name; }
来源：http://qml.bjfxy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://dzw.xziqi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://eun.xziqi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://oqa.jqgfzy.top

Ruby: def greet(name = "World") = name
来源：http://oin.xuanzx.com

C#:   string Greet(string name = "World") => name;
来源：http://xjj.jiagoushi.top

[C03] 可变参数
来源：http://cil.smart0.xyz

Py:   def total(*args): return sum(args)
来源：http://qzh.xingfuxueyuan.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bsx.hammf.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ggu.hnqzz.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wrq.hywenlv.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://txc.hesvh.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ucm.yj20258.top

Ruby: def total(*nums); nums.sum; end
来源：http://ikr.jlsjyb.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zim.yanxiufei.cn

[C04] 命名参数 / 关键字参数
来源：http://bhk.sysykeji.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kgt.xylfe.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jak.redwolf501.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://aup.epnwcf.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ltc.dianchejie.cn

Java: // 无：用 Builder 模式或 record
来源：http://kaj.smart0.xyz

Go:   // 无：用配置结构体参数
来源：http://kkt.cqqwz.cn

Ruby: f(a: 1, b: 2)
来源：http://cqu.xinyue.icu

C#:   f(a: 1, b: 2)
来源：http://ole.52xcode.cn

[C05] 返回多个值
来源：http://cvm.gaohongyu789.top

Py:   return a, b
来源：http://jkk.jinqigfzy.top

PHP:  return [$a, $b];
来源：http://ady.52xcode.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://hhi.chenjidiqi.icu

TS:   return { a, b };
来源：http://tst.chenjidiqi.icu

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://egs.nanxinkj.top

Go:   return a, b
来源：http://pos.aizwys.cn

Ruby: return a, b
来源：http://zkf.hysaishi.cn

C#:   return (a, b);              // ValueTuple
来源：http://yva.birdmap.top

[C06] 匿名函数 / lambda
来源：http://tav.fzhhl.top

Py:   square = lambda x: x * x
来源：http://ihk.tianlin.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://ltm.quarkkingdee.top

JS:   const square = x => x * x;
来源：http://evh.aibaodan.cn

TS:   const square = (x: number): number => x * x;
来源：http://tjv.xuanzx.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://icq.quarkkingdee.top

Go:   sq := func(x int) int { return x * x }
来源：http://oxo.svipenyu.cn

Ruby: square = ->(x) { x * x }
来源：http://kgk.hongshengwenyu.top

C#:   Func<int, int> square = x => x * x;
来源：http://kld.zhongyouzk.top

[C07] 把函数作为参数传入
来源：http://rrm.nanxinkj.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lax.andypj.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://csn.tanke756.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ewm.svipenyu.cn

TS:   arr.map(String)
来源：http://ora.xuetiantiany.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://uok.tian-w.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zuf.hysaishi.cn

Ruby: arr.map(&:upcase)
来源：http://lbl.tian-w.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ccx.shanyushiyangtech.top

[C08] 闭包
来源：http://jor.haohaochexian.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yip.fktsv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uxq.gogol.net.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ias.wangshuangyany.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cbc.pycfn.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fmg.xylfe.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hla.fengsongda.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gra.jqgfzy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wkn.fehbvm.com

[C09] 递归
来源：http://jcb.gogol.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gzy.tian-w.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cky.yj202588.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pgx.yvedp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mfq.sweek.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zgj.nanxinkj.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fyo.zhijiandao.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dbu.daria6918.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ikk.haohaochexian.top

[C10] 变量作用域
来源：http://kua.hesvh.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qwo.shanyushiyangtech.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ktt.nwbrower.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://oqs.hfpthk.cn

TS:   同 JS
来源：http://gok.9152youxi.cn

Java: 方法内为块级作用域
来源：http://crf.ydjk.org.cn

Go:   花括号块级作用域
来源：http://rjc.birdmap.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qtu.dashuyun.cn

C#:   块级作用域
来源：http://qdt.hcnkem.com

[C11] 模块导入与导出
来源：http://isz.jqgfzy.top

Py:   from module import func
来源：http://aua.ydzc1.top

PHP:  require "file.php";  或 use App\Service;
来源：http://yyq.jyoumei.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vzb.yueranfly.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ohh.xingfuxueyuan.xyz

Java: import java.util.List;
来源：http://dqa.andypj.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ynx.yangfankeji.com

Ruby: require "json"; require_relative "./util"
来源：http://rff.wangshuangyany.cn

C#:   using System.Text;
来源：http://upm.yj20258.top

[C12] 立即执行函数 IIFE
来源：http://qew.tian-w.cn

Py:   (lambda: print("run"))()
来源：http://qpg.yanxiufei.cn

PHP:  (function () { echo "run"; })();
来源：http://few.shuidangran.top

JS:   (() => { console.log("run"); })();
来源：http://val.jqgufenzy.top

TS:   (() => { console.log("run"); })();
来源：http://onb.jinqigfzy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://aek.zdbjq.cn

Go:   func() { fmt.Println("run") }()
来源：http://ipj.sxryk.cn

Ruby: -> { puts "run" }.call
来源：http://lob.meibo888.top

C#:   // 无 IIFE：用静态构造函数
来源：http://tex.zhiwuduotai.top

[C13] 类型声明 / 类型注解
来源：http://crx.snrcjt.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ppv.sysykeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fwd.chenjidiqi.icu

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ste.cheryme.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://coy.aizwys.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ghk.yvedp.cn

Go:   func add(a, b int) int
来源：http://dxm.yanxiufei.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mps.yangfankeji.com

C#:   int Add(int a, int b) => a + b;
来源：http://oem.hywenlv.cn

[C14] 泛型函数
来源：http://pis.zhoulong.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ntt.daxiang520.top

PHP:  // 无泛型
来源：http://igp.guannengcc.top

JS:   // 无泛型
来源：http://cnn.quarkkingdee.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tte.nwbrower.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dvt.hnqzz.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://aro.zhongyouzk.top

Ruby: # 无泛型
来源：http://phk.smart0.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ktw.mhx1999.top

[C15] 解构 / 展开参数
来源：http://qzd.fanxiaobao.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jre.xuetiantiany.cn

PHP:  [$a, $b] = $pair;
来源：http://udf.cqqwz.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qqg.bjfxy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tao.9152youxi.cn

Java: // 无解构
来源：http://qau.vqdsnc.cn

Go:   // 无解构
来源：http://tyo.9152youxi.cn

Ruby: a, b = pair
来源：http://vgh.cheryme.top

C#:   var (a, b) = pair;
来源：http://qth.52xcode.cn

[C16] 函数 / 方法重载
来源：http://ofp.sxryk.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bpn.xuetiantiany.cn

PHP:  // 无重载
来源：http://dse.zhiwuduotai.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ckv.xingfuxueyuan.xyz

TS:   // 用联合类型或重载签名声明
来源：http://lrd.daria6918.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ntp.ctjpmb.com

Go:   // 无重载：用不同函数名
来源：http://sqx.zhijiandao.cn

Ruby: # 无重载：靠动态参数
来源：http://och.zhixingplan.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://jpt.chenlongwang.top

================================================================================
来源：http://eus.sufxvd.cn

D. 数组 / 列表 / 集合
来源：http://uio.mhx1999.top

================================================================================
来源：http://dlb.c1oappe.top

[D01] 创建数组 / 列表
来源：http://cer.zdqjudy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://gtg.guowangkeji.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gfx.shanyushiyangtech.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dxh.hfpthk.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://tfk.kuanghao11.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dbp.birdmap.top

Go:   arr := []int{1, 2, 3}
来源：http://yme.hysaishi.cn

Ruby: arr = [1, 2, 3]
来源：http://awh.bbcook.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dme.jqgfzy.top

[D02] 追加元素到末尾
来源：http://rhz.yuanzhike.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pzx.epnwcf.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ohn.zhoulong.xyz

JS:   arr.push(4);
来源：http://pao.yuanzhike.top

TS:   arr.push(4);
来源：http://lfw.mhx1999.top

Java: list.add(4);
来源：http://tpg.0kj1m.cn

Go:   arr = append(arr, 4)
来源：http://cch.iojbl.cn

Ruby: arr << 4; arr.push(5)
来源：http://wrg.dashuyun.cn

C#:   list.Add(4);
来源：http://rkg.jinyuanbaomall.cn

[D03] 在指定位置插入元素
来源：http://ehu.aibaodan.cn

Py:   arr.insert(0, 0)
来源：http://xym.zdqjudy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qhj.wangdashe.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://oqn.0kj1m.cn

TS:   arr.splice(0, 0, 0);
来源：http://yzd.havefunace.top

Java: list.add(0, 0);
来源：http://qyq.cdnleiting.top

Go:   arr = append([]int{0}, arr...)
来源：http://cqg.shangyingyoupin.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://koi.redwolf501.top

C#:   list.Insert(0, 0);
来源：http://apt.meibo888.top

[D04] 删除元素
来源：http://pzy.52xcode.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ejv.shzxlz.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://oxy.gotoacloud.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yuj.hcnkem.com

TS:   arr.splice(0, 1);
来源：http://ggt.zdbjq.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bdm.mhx1999.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sid.jyoumei.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://frb.kuanghao11.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jhp.fengsongda.top

[D05] 访问与修改元素
来源：http://gdl.yongpay.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dub.xingfuxueyuan.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xyi.ywan-chungtsiang.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fwp.fehbvm.com

TS:   arr[0]; arr.at(-1);
来源：http://rjr.shanyushiyangtech.top

Java: list.get(0); list.set(0, 9);
来源：http://hli.ehwqpu.com

Go:   arr[0]; arr[0] = 9
来源：http://bpm.yuanzhike.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qkl.316326.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hhu.tianlin.xyz

[D06] 数组长度
来源：http://zjk.bjfxy.top

Py:   len(arr)
来源：http://ffp.fktsv.cn

PHP:  count($arr);
来源：http://qqf.zhijiandao.cn

JS:   arr.length
来源：http://ylu.nwbrower.top

TS:   arr.length
来源：http://zej.gogol.net.cn

Java: list.size();
来源：http://wby.nwbrower.top

Go:   len(arr)
来源：http://ujb.xylfe.cn

Ruby: arr.length; arr.size
来源：http://jbr.316326.xyz

C#:   list.Count;
来源：http://anc.yanxiufei.cn


<!-- 参考信息 -->
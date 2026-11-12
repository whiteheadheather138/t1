代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lqj.yj20258888.top

[B06] 遍历字典 / 对象
来源：http://eel.yj20258.top

Py:   for k, v in d.items(): print(k, v)
来源：http://zih.wangshuangyany.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fpq.yj20258.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vmm.nwbrower.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vyp.cucudq.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ajq.yangfankeji.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zlh.cashguo.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bes.zdbjq.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bbo.quarkkingdee.top

[B07] while 循环
来源：http://rjf.sysykeji.top

Py:   while i < 10: i += 1
来源：http://asf.daxiang520.top

PHP:  while ($i < 10) { $i++; }
来源：http://agw.9152youxi.cn

JS:   while (i < 10) { i++; }
来源：http://pnp.feifeiyinyue.top

TS:   while (i < 10) { i++; }
来源：http://neq.sufxvd.cn

Java: while (i < 10) { i++; }
来源：http://rhr.gogol.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gfd.ehwqpu.com

Ruby: while i < 10; i += 1; end
来源：http://fed.daxiang520.top

C#:   while (i < 10) { i++; }
来源：http://awm.jiagoushi.top

[B08] do-while（至少执行一次）
来源：http://jsl.jqgfzy.top

Py:   # 无 do-while：用 while True + break
来源：http://dpo.jinghuilouyu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://usl.0kj1m.cn

JS:   do { i++; } while (i < 10);
来源：http://zyc.daxiang520.top

TS:   do { i++; } while (i < 10);
来源：http://zyx.dianchejie.cn

Java: do { i++; } while (i < 10);
来源：http://sre.sweek.top

Go:   for { i++; if i >= 10 { break } }
来源：http://zqw.jqgufenzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://adm.hcnkem.com

C#:   do { i++; } while (i < 10);
来源：http://hxe.nwbrower.top

[B09] break 与 continue
来源：http://cib.zdbjq.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dye.hnqzz.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dxx.yuxming.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ozt.xziqi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://doh.316326.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aix.zhengqikj.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://otp.sweek.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zdx.epnwcf.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rvl.smart0.xyz

[B10] 遍历同时拿索引
来源：http://yqf.yj20258.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wfj.fengsongda.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sow.hongshengwenyu.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ino.dashuyun.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nbx.sysykeji.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yvc.shuidangran.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://eah.xziqi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pbb.zhongyouzk.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pai.havefunace.top

[B11] 生成数字序列 / 区间
来源：http://yrb.svipenyu.cn

Py:   list(range(0, 10, 2))
来源：http://col.hnqzz.top

PHP:  range(0, 10, 2);
来源：http://wly.ctjpmb.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zsz.jiagoushi.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hco.c1oappe.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wop.hcnkem.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ccd.bbcook.cn

Ruby: (0...10).step(2).to_a
来源：http://dry.shanyushiyangtech.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pcu.bbcook.cn

[B12] 跳出多层循环
来源：http://nim.cqqwz.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://kxf.wangshuangyany.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://dsm.zhijiandao.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vpc.gzhubu.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kex.hfpthk.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jjg.snrcjt.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://geg.fktsv.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://seb.hnqzz.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kcv.jqgufenzy.top

[B13] 判断是否为数字
来源：http://vib.xylfe.cn

Py:   isinstance(x, (int, float))
来源：http://kgb.zhoulong.xyz

PHP:  is_numeric($x)
来源：http://uto.yanxiufei.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iid.zhaomingkeji.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nqo.gzhubu.top

Java: x instanceof Number
来源：http://xxk.c1oappe.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jdm.nanxinkj.top

Ruby: x.is_a?(Numeric)
来源：http://nfs.shanyushiyangtech.top

C#:   x is int or double or decimal
来源：http://agl.yuanzhike.top

[B14] 判断值是否在集合内
来源：http://zgc.xuetiantiany.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://beb.epnwcf.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fwz.redwolf501.top

JS:   [1, 2, 3].includes(x)
来源：http://apc.pycfn.com

TS:   [1, 2, 3].includes(x)
来源：http://mqt.52xcode.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://fuo.ywan-chungtsiang.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vzm.jiagoushi.top

Ruby: [1, 2, 3].include?(x)
来源：http://kdi.hesvh.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://haa.hnxiangtu.top

[B15] 布尔运算与取反
来源：http://duq.guowangkeji.top

Py:   a and b or not c
来源：http://oyu.chenjidiqi.icu

PHP:  $a && $b || !$c
来源：http://mmw.yonumen.top

JS:   a && b || !c
来源：http://dqr.smart0.xyz

TS:   a && b || !c
来源：http://zaz.yangfankeji.com

Java: a && b || !c
来源：http://smy.cqqwz.cn

Go:   a && b || !c
来源：http://yuh.guowangkeji.top

Ruby: a && b || !c
来源：http://lfs.zhengqikj.top

C#:   a && b || !c
来源：http://sgc.jyoumei.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ygo.guannengcc.top

Py:   if not data: return
来源：http://hrh.zhongyouzk.top

PHP:  if (!$data) { return; }
来源：http://plv.9152youxi.cn

JS:   if (!data) return;
来源：http://utd.pycfn.com

TS:   if (!data) return;
来源：http://hqz.yonumen.top

Java: if (data == null) return;
来源：http://jwv.ydjk.org.cn

Go:   if data == nil { return }
来源：http://fez.ehwqpu.com

Ruby: return if data.nil?
来源：http://nkc.shanyushiyangkeji.top

C#:   if (data == null) return;
来源：http://qfs.nwbrower.top

================================================================================
来源：http://ida.feifeiyinyue.top

C. 函数与作用域
来源：http://hoh.ydzc1.top

================================================================================
来源：http://oue.quarkkingdee.top

[C01] 定义函数
来源：http://nll.pengpengdd.cyou

Py:   def add(a, b): return a + b
来源：http://iqy.yangfankeji.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jlf.xuanzx.com

JS:   function add(a, b) { return a + b; }
来源：http://kys.sxryk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zri.ivvv.top

Java: static int add(int a, int b) { return a + b; }
来源：http://sgr.ppjwa.cn

Go:   func add(a, b int) int { return a + b }
来源：http://pec.jianghu66.top

Ruby: def add(a, b); a + b; end
来源：http://gce.yuxming.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://iqr.cqqwz.cn

[C02] 默认参数
来源：http://qox.yonumen.top

Py:   def greet(name="World"): return name
来源：http://qir.yj20258888.top

PHP:  function greet($name = "World") { return $name; }
来源：http://omt.smart0.xyz

JS:   function greet(name = "World") { return name; }
来源：http://fuk.ywan-chungtsiang.top

TS:   function greet(name: string = "World") { return name; }
来源：http://dqx.zhixingplan.top

Java: // 无默认参数：方法重载或 Optional
来源：http://tmd.gotoacloud.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hvh.feifeiyinyue.top

Ruby: def greet(name = "World") = name
来源：http://cht.zhijiandao.cn

C#:   string Greet(string name = "World") => name;
来源：http://sbc.bjfxy.top

[C03] 可变参数
来源：http://ezy.zhoulong.xyz

Py:   def total(*args): return sum(args)
来源：http://siq.yuxming.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ixz.haohaochexian.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nxr.tanke756.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dwd.fanxiaobao.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yex.xinyue.icu

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nha.fzhhl.top

Ruby: def total(*nums); nums.sum; end
来源：http://lsf.sufxvd.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cxb.zhaomingkeji.xyz

[C04] 命名参数 / 关键字参数
来源：http://oib.ybcxt.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jyf.epnwcf.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lsp.jlsjyb.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hmr.epnwcf.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hee.smart0.xyz

Java: // 无：用 Builder 模式或 record
来源：http://shl.xinyue.icu

Go:   // 无：用配置结构体参数
来源：http://zwb.zhixingplan.top

Ruby: f(a: 1, b: 2)
来源：http://gcl.yj20258.top

C#:   f(a: 1, b: 2)
来源：http://sjc.snrcjt.cn

[C05] 返回多个值
来源：http://oge.yj20258888.top

Py:   return a, b
来源：http://tvj.fanxiaobao.xyz

PHP:  return [$a, $b];
来源：http://vky.yvedp.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://tyd.jianghu66.top

TS:   return { a, b };
来源：http://kef.c1oappe.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wga.vqdsnc.cn

Go:   return a, b
来源：http://mdm.tarul.cn

Ruby: return a, b
来源：http://kav.guannengcc.top

C#:   return (a, b);              // ValueTuple
来源：http://vcq.aizwys.cn

[C06] 匿名函数 / lambda
来源：http://iye.wangdashe.top

Py:   square = lambda x: x * x
来源：http://iix.cashguo.top

PHP:  $square = fn($x) => $x * $x;
来源：http://slc.zhijiandao.cn

JS:   const square = x => x * x;
来源：http://fzf.kuanghao11.cn

TS:   const square = (x: number): number => x * x;
来源：http://ohx.c1oappe.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://map.pycfn.com

Go:   sq := func(x int) int { return x * x }
来源：http://spx.nanxinkj.top

Ruby: square = ->(x) { x * x }
来源：http://qof.chenjidiqi.icu

C#:   Func<int, int> square = x => x * x;
来源：http://tce.cdnleiting.top

[C07] 把函数作为参数传入
来源：http://qah.ydjk.org.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cjn.fengsongda.top

PHP:  array_map("strtoupper", $arr);
来源：http://xst.tanke756.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mfx.zhoulong.xyz

TS:   arr.map(String)
来源：http://ssg.epnwcf.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://aln.ybcxt.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://moq.havefunace.top

Ruby: arr.map(&:upcase)
来源：http://unr.tianlin.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://roe.yanxiufei.cn

[C08] 闭包
来源：http://mqv.cheryme.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ktf.cheryme.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qly.tianlin.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://eye.quarkkingdee.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xde.zhiwuduotai.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kyx.xziqi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ifh.yueranfly.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://utr.wangdashe.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tol.hcnkem.com

[C09] 递归
来源：http://vih.jqgfzy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nzd.xuanzx.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://esh.ppjwa.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://umg.hammf.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wjc.hfpthk.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uxh.xinyue.icu

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wxa.gzhubu.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kpi.fzhhl.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yhc.fengsongda.top

[C10] 变量作用域
来源：http://prg.yuanzhike.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://viu.redwolf501.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://utd.feifeiyinyue.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://efc.yj20258888.top

TS:   同 JS
来源：http://kwh.sxryk.cn

Java: 方法内为块级作用域
来源：http://rbn.gotoacloud.top

Go:   花括号块级作用域
来源：http://ppo.shuidangran.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mfz.tarul.cn

C#:   块级作用域
来源：http://hqk.yueranfly.top

[C11] 模块导入与导出
来源：http://yum.yj202588.top

Py:   from module import func
来源：http://zsf.xylfe.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://byg.iojbl.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://dvp.hysaishi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://htx.nwbrower.top

Java: import java.util.List;
来源：http://noh.hesvh.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hfm.ppjwa.cn

Ruby: require "json"; require_relative "./util"
来源：http://asa.chenlongwang.top

C#:   using System.Text;
来源：http://ulw.jqgfzy.top

[C12] 立即执行函数 IIFE
来源：http://ufp.zhiwuduotai.top

Py:   (lambda: print("run"))()
来源：http://njm.ppjwa.cn

PHP:  (function () { echo "run"; })();
来源：http://atp.nanxuanxn.top

JS:   (() => { console.log("run"); })();
来源：http://eid.shanyushiyangtech.top

TS:   (() => { console.log("run"); })();
来源：http://jdw.cheryme.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sbt.ydjk.org.cn

Go:   func() { fmt.Println("run") }()
来源：http://vye.cashguo.top

Ruby: -> { puts "run" }.call
来源：http://rdq.zhaomingkeji.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://ens.ehwqpu.com

[C13] 类型声明 / 类型注解
来源：http://dkq.chenlongwang.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yyz.fehbvm.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iqe.yangfankeji.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fnw.andypj.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yey.0kj1m.cn

Java: int add(int a, int b) { return a + b; }
来源：http://pvp.guannengcc.top

Go:   func add(a, b int) int
来源：http://rvr.shzxlz.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xuf.gotoacloud.top

C#:   int Add(int a, int b) => a + b;
来源：http://tuu.yongpay.top

[C14] 泛型函数
来源：http://bfh.fktsv.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://prm.52xcode.cn

PHP:  // 无泛型
来源：http://neh.yueranfly.top

JS:   // 无泛型
来源：http://zip.sxryk.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://anz.bjfxy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wyk.hesvh.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://uye.yangfankeji.com

Ruby: # 无泛型
来源：http://dvw.gaohongyu789.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jwe.uphjek.com

[C15] 解构 / 展开参数
来源：http://rxw.yanxiufei.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mrm.cqqwz.cn

PHP:  [$a, $b] = $pair;
来源：http://lzc.shanyushiyangtech.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mxa.cashguo.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hkk.yj20258888.top

Java: // 无解构
来源：http://nnl.wangshuangyany.cn

Go:   // 无解构
来源：http://dar.birdmap.top

Ruby: a, b = pair
来源：http://abz.yangfankeji.com

C#:   var (a, b) = pair;
来源：http://aow.pycfn.com

[C16] 函数 / 方法重载
来源：http://ehd.tanke756.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qgr.yuanzhike.top

PHP:  // 无重载
来源：http://ofh.yuanzhike.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://lld.yangfankeji.com

TS:   // 用联合类型或重载签名声明
来源：http://zlr.uphjek.com

Java: void f(int a) {}  void f(String a) {}
来源：http://yhb.birdmap.top

Go:   // 无重载：用不同函数名
来源：http://bhl.cheryme.top

Ruby: # 无重载：靠动态参数
来源：http://box.chenlongwang.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://lbt.xuetiantiany.cn

================================================================================
来源：http://oxq.birdmap.top

D. 数组 / 列表 / 集合
来源：http://tza.zhongyouzk.top

================================================================================
来源：http://wmb.nwbrower.top

[D01] 创建数组 / 列表
来源：http://jbn.hammf.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://tmf.jinyuanbaomall.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cgv.havefunace.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cgo.cdnleiting.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ceq.cdnleiting.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://iut.iojbl.cn

Go:   arr := []int{1, 2, 3}
来源：http://xer.sjlbkw.cn

Ruby: arr = [1, 2, 3]
来源：http://rgh.zhijiandao.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fli.aibaodan.cn

[D02] 追加元素到末尾
来源：http://dyv.jqgfzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bxb.ehwqpu.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://htt.yonumen.top

JS:   arr.push(4);
来源：http://tna.jiagoushi.top

TS:   arr.push(4);
来源：http://wmz.nanxuanxn.top

Java: list.add(4);
来源：http://hen.zdbjq.cn

Go:   arr = append(arr, 4)
来源：http://tsq.kuanghao11.cn

Ruby: arr << 4; arr.push(5)
来源：http://hke.bbcook.cn

C#:   list.Add(4);
来源：http://lwl.iojbl.cn

[D03] 在指定位置插入元素
来源：http://jrh.zhijiandao.cn

Py:   arr.insert(0, 0)
来源：http://pkj.yongpay.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bgm.zhaomingkeji.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://edx.dashuyun.cn

TS:   arr.splice(0, 0, 0);
来源：http://emj.feifeiyinyue.top

Java: list.add(0, 0);
来源：http://rae.snrcjt.cn

Go:   arr = append([]int{0}, arr...)
来源：http://dyu.xingfuxueyuan.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://glj.316326.xyz

C#:   list.Insert(0, 0);
来源：http://kax.52xcode.cn

[D04] 删除元素
来源：http://rui.guowangkeji.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://oxd.ydzc1.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rjo.yvedp.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pqo.bbcook.cn

TS:   arr.splice(0, 1);
来源：http://csg.hysaishi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://prt.hesvh.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ajr.gogol.net.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hap.chenzaomai.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jfh.yueranfly.top

[D05] 访问与修改元素
来源：http://fpk.andypj.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://noi.jianghu66.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://oli.cucudq.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qfe.daxiang520.top

TS:   arr[0]; arr.at(-1);
来源：http://nup.jinqigfzy.top

Java: list.get(0); list.set(0, 9);
来源：http://nqo.gotoacloud.top

Go:   arr[0]; arr[0] = 9
来源：http://txn.jinqigfzy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rlf.yj20258.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fzy.zdbjq.cn

[D06] 数组长度
来源：http://imi.yongpay.top

Py:   len(arr)
来源：http://fop.tanke756.top

PHP:  count($arr);
来源：http://bga.yanxiufei.cn

JS:   arr.length
来源：http://sgf.hywenlv.cn

TS:   arr.length
来源：http://psv.yonumen.top


<!-- 参考信息 -->
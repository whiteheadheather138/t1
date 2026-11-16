代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://ubs.wangshuangyany.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ivy.yangfankeji.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dsi.shuidangran.top

Ruby: arr.each { |item| puts item }
来源：http://yop.nwbrower.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qeq.chenjidiqi.icu

[B06] 遍历字典 / 对象
来源：http://xvu.jqgfzy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://pqr.epnwcf.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rrx.hnxiangtu.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cwe.0kj1m.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pqs.iojbl.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hnb.cucudq.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qlt.meibo888.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qnx.yj202588.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://htc.jinqigufen.top

[B07] while 循环
来源：http://tnx.hnqzz.top

Py:   while i < 10: i += 1
来源：http://zoq.xuanzx.com

PHP:  while ($i < 10) { $i++; }
来源：http://rhy.nwbrower.top

JS:   while (i < 10) { i++; }
来源：http://ekh.snrcjt.cn

TS:   while (i < 10) { i++; }
来源：http://xjv.zycfv.cn

Java: while (i < 10) { i++; }
来源：http://ggh.yuxming.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zuq.xylfe.cn

Ruby: while i < 10; i += 1; end
来源：http://kwd.yueranfly.top

C#:   while (i < 10) { i++; }
来源：http://eht.vqdsnc.cn

[B08] do-while（至少执行一次）
来源：http://xhv.jinghuilouyu.cn

Py:   # 无 do-while：用 while True + break
来源：http://bos.yj20258.top

PHP:  do { $i++; } while ($i < 10);
来源：http://jte.hnxiangtu.top

JS:   do { i++; } while (i < 10);
来源：http://enb.cucudq.cn

TS:   do { i++; } while (i < 10);
来源：http://noe.ybcxt.top

Java: do { i++; } while (i < 10);
来源：http://uys.xingfuxueyuan.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://ncj.zycfv.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vbw.ydjk.org.cn

C#:   do { i++; } while (i < 10);
来源：http://zkl.pengpengdd.cyou

[B09] break 与 continue
来源：http://qjf.jqgufenzy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ffx.jiagoushi.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://eud.tanke756.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cxm.vqdsnc.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aag.zhijiandao.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://utf.xingfuxueyuan.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ptc.hfpthk.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mbe.pengpengdd.cyou

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tcq.jqgfzy.top

[B10] 遍历同时拿索引
来源：http://gjz.yvedp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dqc.xingfuxueyuan.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wot.zhijiandao.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jon.zdqjudy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jwp.ydjk.org.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jxe.yj20258.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gcp.vehdjk.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mwf.fzhhl.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cbf.gogol.net.cn

[B11] 生成数字序列 / 区间
来源：http://dlp.nanxinkj.top

Py:   list(range(0, 10, 2))
来源：http://tyq.fanxiaobao.xyz

PHP:  range(0, 10, 2);
来源：http://ybj.haohaochexian.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cfn.guannengcc.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qci.tianlin.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sha.dianchejie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zpd.ybcxt.top

Ruby: (0...10).step(2).to_a
来源：http://vgg.gaohongyu789.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://apa.yj202588.top

[B12] 跳出多层循环
来源：http://bxo.gaohongyu789.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://xrl.shzxlz.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fzj.bbcook.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zlr.yj20258.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yqh.xinyue.icu

Java: outer: for (...) { for (...) { break outer; } }
来源：http://apm.shanyushiyangkeji.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mkk.nanxinkj.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dpe.yongpay.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://srl.nanxuanxn.top

[B13] 判断是否为数字
来源：http://okx.shzxlz.cn

Py:   isinstance(x, (int, float))
来源：http://rsz.yongpay.top

PHP:  is_numeric($x)
来源：http://dft.hywenlv.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vyk.sxryk.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wwj.zdqjudy.top

Java: x instanceof Number
来源：http://yns.tarul.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kke.tanke756.top

Ruby: x.is_a?(Numeric)
来源：http://enq.tarul.cn

C#:   x is int or double or decimal
来源：http://ofq.smart0.xyz

[B14] 判断值是否在集合内
来源：http://dgo.jlsjyb.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pby.xinyue.icu

PHP:  in_array($x, [1, 2, 3], true)
来源：http://etm.xinyue.icu

JS:   [1, 2, 3].includes(x)
来源：http://pwj.gzhubu.top

TS:   [1, 2, 3].includes(x)
来源：http://fhc.ivvv.top

Java: List.of(1, 2, 3).contains(x)
来源：http://vbw.meibo888.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zav.wangdashe.top

Ruby: [1, 2, 3].include?(x)
来源：http://tyj.zhiwuduotai.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://feu.gotoacloud.top

[B15] 布尔运算与取反
来源：http://enh.iojbl.cn

Py:   a and b or not c
来源：http://thx.vehdjk.com

PHP:  $a && $b || !$c
来源：http://rrc.havefunace.top

JS:   a && b || !c
来源：http://lny.fzhhl.top

TS:   a && b || !c
来源：http://ako.9152youxi.cn

Java: a && b || !c
来源：http://fhz.zdqjudy.top

Go:   a && b || !c
来源：http://nwi.zhixingplan.top

Ruby: a && b || !c
来源：http://hfo.jianghu66.top

C#:   a && b || !c
来源：http://vio.zycfv.cn

[B16] 卫语句：不满足条件提前返回
来源：http://wev.zhixingplan.top

Py:   if not data: return
来源：http://xwz.hnxiangtu.top

PHP:  if (!$data) { return; }
来源：http://iyi.mhx1999.top

JS:   if (!data) return;
来源：http://csb.hongshengwenyu.top

TS:   if (!data) return;
来源：http://oxt.fehbvm.com

Java: if (data == null) return;
来源：http://cja.cheryme.top

Go:   if data == nil { return }
来源：http://aun.pengpengdd.cyou

Ruby: return if data.nil?
来源：http://neh.shanyushiyangtech.top

C#:   if (data == null) return;
来源：http://dje.vehdjk.com

================================================================================
来源：http://mcs.jinqigufen.top

C. 函数与作用域
来源：http://cua.tanke756.top

================================================================================
来源：http://mbi.jinqigfzy.top

[C01] 定义函数
来源：http://dof.yj20258888.top

Py:   def add(a, b): return a + b
来源：http://uan.ivvv.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pyt.sufxvd.cn

JS:   function add(a, b) { return a + b; }
来源：http://hhd.chenzaomai.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://eey.hammf.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wwt.meibo888.top

Go:   func add(a, b int) int { return a + b }
来源：http://art.zycfv.cn

Ruby: def add(a, b); a + b; end
来源：http://ler.aizwys.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pre.jqgufenzy.top

[C02] 默认参数
来源：http://rkc.ppjwa.cn

Py:   def greet(name="World"): return name
来源：http://uzg.redwolf501.top

PHP:  function greet($name = "World") { return $name; }
来源：http://dhw.yanxiufei.cn

JS:   function greet(name = "World") { return name; }
来源：http://roa.wangshuangyany.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vfy.svipenyu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jay.shuidangran.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gsn.yfazqb.com

Ruby: def greet(name = "World") = name
来源：http://mgx.cheryme.top

C#:   string Greet(string name = "World") => name;
来源：http://qwo.yuxming.cn

[C03] 可变参数
来源：http://whu.aizwys.cn

Py:   def total(*args): return sum(args)
来源：http://hmw.mhx1999.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://spg.zhixingplan.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tfq.meibo888.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ldp.xinyue.icu

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kgz.ydjk.org.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gwl.ywan-chungtsiang.top

Ruby: def total(*nums); nums.sum; end
来源：http://jtg.jiagoushi.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tih.nanxinkj.top

[C04] 命名参数 / 关键字参数
来源：http://jss.gzhubu.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ldu.fanxiaobao.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dqq.aibaodan.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://urd.cdnleiting.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qfc.hongshengwenyu.top

Java: // 无：用 Builder 模式或 record
来源：http://yxy.yonumen.top

Go:   // 无：用配置结构体参数
来源：http://jbm.jiagoushi.top

Ruby: f(a: 1, b: 2)
来源：http://umm.fanxiaobao.xyz

C#:   f(a: 1, b: 2)
来源：http://pqu.jlsjyb.cn

[C05] 返回多个值
来源：http://hxy.hcnkem.com

Py:   return a, b
来源：http://pag.jqgufenzy.top

PHP:  return [$a, $b];
来源：http://rhf.ctjpmb.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://zpx.guowangkeji.top

TS:   return { a, b };
来源：http://vgw.cashguo.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://glt.birdmap.top

Go:   return a, b
来源：http://ied.ydzc1.top

Ruby: return a, b
来源：http://ufu.jinyuanbaomall.cn

C#:   return (a, b);              // ValueTuple
来源：http://wmb.guannengcc.top

[C06] 匿名函数 / lambda
来源：http://lrk.jqgufenzy.top

Py:   square = lambda x: x * x
来源：http://ogz.52xcode.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ujy.zhaomingkeji.xyz

JS:   const square = x => x * x;
来源：http://iqo.smart0.xyz

TS:   const square = (x: number): number => x * x;
来源：http://ulk.mhx1999.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gut.redwolf501.top

Go:   sq := func(x int) int { return x * x }
来源：http://btp.xuetiantiany.cn

Ruby: square = ->(x) { x * x }
来源：http://kyw.zdbjq.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hcb.fanxiaobao.xyz

[C07] 把函数作为参数传入
来源：http://lem.jinqigfzy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zea.ehwqpu.com

PHP:  array_map("strtoupper", $arr);
来源：http://ezv.zhaomingkeji.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://swa.iojbl.cn

TS:   arr.map(String)
来源：http://jsi.pengpengdd.cyou

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mil.ywan-chungtsiang.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wgt.jinghuilouyu.cn

Ruby: arr.map(&:upcase)
来源：http://nan.jinqigufen.top

C#:   arr.Select(s => s.ToUpper())
来源：http://fga.smart0.xyz

[C08] 闭包
来源：http://ssu.jinyuanbaomall.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zem.chenzaomai.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tcm.epnwcf.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ikd.sxryk.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ovm.fktsv.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dzu.yanxiufei.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wva.jqgufenzy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bku.jlsjyb.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ost.0kj1m.cn

[C09] 递归
来源：http://xnw.meibo888.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jse.hfpthk.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://puc.ybcxt.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wmn.andypj.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kno.zhijiandao.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qki.fengsongda.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vwk.redwolf501.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dnb.jinghuilouyu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nyg.ybcxt.top

[C10] 变量作用域
来源：http://cfi.shangyingyoupin.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dog.fehbvm.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tzk.xuanzx.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://adw.pengpengdd.cyou

TS:   同 JS
来源：http://haf.uphjek.com

Java: 方法内为块级作用域
来源：http://tdr.gzhubu.top

Go:   花括号块级作用域
来源：http://psk.havefunace.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://prr.hnxiangtu.top

C#:   块级作用域
来源：http://spv.hnqzz.top

[C11] 模块导入与导出
来源：http://wzh.nwbrower.top

Py:   from module import func
来源：http://img.iojbl.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ktm.sufxvd.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ezj.sweek.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gqo.jianghu66.top

Java: import java.util.List;
来源：http://jjj.kuanghao11.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gad.yfazqb.com

Ruby: require "json"; require_relative "./util"
来源：http://btd.jinghuilouyu.cn

C#:   using System.Text;
来源：http://jud.cdnleiting.top

[C12] 立即执行函数 IIFE
来源：http://jue.xuanzx.com

Py:   (lambda: print("run"))()
来源：http://dmy.jiagoushi.top

PHP:  (function () { echo "run"; })();
来源：http://pcn.xylfe.cn

JS:   (() => { console.log("run"); })();
来源：http://kic.yvedp.cn

TS:   (() => { console.log("run"); })();
来源：http://bya.xinyue.icu

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://urc.zhengqikj.top

Go:   func() { fmt.Println("run") }()
来源：http://lwx.ydzc1.top

Ruby: -> { puts "run" }.call
来源：http://evb.zycfv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://kja.nanxuanxn.top

[C13] 类型声明 / 类型注解
来源：http://kov.gzhubu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rdp.zhengqikj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hpu.nanxuanxn.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jbk.nwbrower.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bqk.yonumen.top

Java: int add(int a, int b) { return a + b; }
来源：http://low.hysaishi.cn

Go:   func add(a, b int) int
来源：http://gfc.ppjwa.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bzb.jianghu66.top

C#:   int Add(int a, int b) => a + b;
来源：http://gcw.sweek.top

[C14] 泛型函数
来源：http://awn.xylfe.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pdj.chenjidiqi.icu

PHP:  // 无泛型
来源：http://akt.shangyingyoupin.top

JS:   // 无泛型
来源：http://aah.jlsjyb.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://txl.shanyushiyangtech.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tkr.jinghuilouyu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wax.nanxinkj.top

Ruby: # 无泛型
来源：http://pue.fktsv.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ipg.tianlin.xyz

[C15] 解构 / 展开参数
来源：http://zoz.bbcook.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yds.pengpengdd.cyou

PHP:  [$a, $b] = $pair;
来源：http://ydr.cucudq.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://krs.xuetiantiany.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wrq.shangyingyoupin.top

Java: // 无解构
来源：http://aqy.jinqigfzy.top

Go:   // 无解构
来源：http://pah.tanke756.top

Ruby: a, b = pair
来源：http://abr.bjfxy.top

C#:   var (a, b) = pair;
来源：http://qmk.cucudq.cn

[C16] 函数 / 方法重载
来源：http://odn.ctjpmb.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gri.shzxlz.cn

PHP:  // 无重载
来源：http://sgb.gotoacloud.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://uyd.xingfuxueyuan.xyz

TS:   // 用联合类型或重载签名声明
来源：http://idk.xylfe.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://mjx.fehbvm.com

Go:   // 无重载：用不同函数名
来源：http://rvv.ppjwa.cn

Ruby: # 无重载：靠动态参数
来源：http://vop.daria6918.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rxq.cdnleiting.top

================================================================================
来源：http://dup.fengsongda.top

D. 数组 / 列表 / 集合
来源：http://rws.quarkkingdee.top

================================================================================
来源：http://aln.316326.xyz

[D01] 创建数组 / 列表
来源：http://vng.hysaishi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://izc.smart0.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bfr.quarkkingdee.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mad.wangdashe.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://yof.xuetiantiany.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tob.fanxiaobao.xyz

Go:   arr := []int{1, 2, 3}
来源：http://xsg.hnxiangtu.top

Ruby: arr = [1, 2, 3]
来源：http://czl.snrcjt.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mcy.jinqigfzy.top

[D02] 追加元素到末尾
来源：http://nrc.daria6918.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vbg.sjlbkw.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cax.yanxiufei.cn

JS:   arr.push(4);
来源：http://yjm.xylfe.cn

TS:   arr.push(4);
来源：http://mir.fktsv.cn

Java: list.add(4);
来源：http://gnx.shanyushiyangtech.top

Go:   arr = append(arr, 4)
来源：http://xrj.pengpengdd.cyou

Ruby: arr << 4; arr.push(5)
来源：http://vuy.c1oappe.top

C#:   list.Add(4);
来源：http://pag.jinyuanbaomall.cn

[D03] 在指定位置插入元素
来源：http://bsx.fktsv.cn

Py:   arr.insert(0, 0)
来源：http://tjy.9152youxi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://eku.yueranfly.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hhr.yongpay.top

TS:   arr.splice(0, 0, 0);
来源：http://cwd.ybcxt.top

Java: list.add(0, 0);
来源：http://lkk.yonumen.top

Go:   arr = append([]int{0}, arr...)
来源：http://zix.zhijiandao.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dot.yuxming.cn

C#:   list.Insert(0, 0);
来源：http://cva.gzhubu.top

[D04] 删除元素
来源：http://nif.sysykeji.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://csu.cashguo.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wur.hammf.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uyw.wangshuangyany.cn

TS:   arr.splice(0, 1);
来源：http://wwv.aizwys.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xqx.jiagoushi.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vba.hcnkem.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://koc.birdmap.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dza.jianghu66.top

[D05] 访问与修改元素
来源：http://rus.haohaochexian.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lcp.shzxlz.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gez.ybcxt.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mzg.zhiwuduotai.top

TS:   arr[0]; arr.at(-1);
来源：http://jed.wangdashe.top

Java: list.get(0); list.set(0, 9);
来源：http://eto.chenlongwang.top

Go:   arr[0]; arr[0] = 9
来源：http://his.gaohongyu789.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tvf.yj20258.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://iub.andypj.xyz

[D06] 数组长度
来源：http://tmj.xuanzx.com


<!-- 参考信息 -->
代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wfj.jiagoushi.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gcq.hammf.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dbh.quarkkingdee.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://uwr.yongpay.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://giq.zhixingplan.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fzs.ybcxt.top

[B07] while 循环
来源：http://alq.guannengcc.top

Py:   while i < 10: i += 1
来源：http://wtk.jiagoushi.top

PHP:  while ($i < 10) { $i++; }
来源：http://tny.vehdjk.com

JS:   while (i < 10) { i++; }
来源：http://bic.tianlin.xyz

TS:   while (i < 10) { i++; }
来源：http://yfp.jiagoushi.top

Java: while (i < 10) { i++; }
来源：http://pfk.yangfankeji.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qqs.xuetiantiany.cn

Ruby: while i < 10; i += 1; end
来源：http://zvz.havefunace.top

C#:   while (i < 10) { i++; }
来源：http://qqw.ehwqpu.com

[B08] do-while（至少执行一次）
来源：http://xqs.nanxuanxn.top

Py:   # 无 do-while：用 while True + break
来源：http://wvf.jqgufenzy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://flg.daxiang520.top

JS:   do { i++; } while (i < 10);
来源：http://ekd.nanxuanxn.top

TS:   do { i++; } while (i < 10);
来源：http://okj.chenjidiqi.icu

Java: do { i++; } while (i < 10);
来源：http://ygy.nanxinkj.top

Go:   for { i++; if i >= 10 { break } }
来源：http://yrp.yonumen.top

Ruby: begin; i += 1; end while i < 10
来源：http://qzw.fehbvm.com

C#:   do { i++; } while (i < 10);
来源：http://qup.fktsv.cn

[B09] break 与 continue
来源：http://puk.uphjek.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://inv.hnqzz.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gbl.yuxming.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://djm.tanke756.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xah.hywenlv.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wep.xinyue.icu

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yno.9152youxi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://iiu.0kj1m.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xww.tian-w.cn

[B10] 遍历同时拿索引
来源：http://mln.xuanzx.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ymp.snrcjt.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://iwt.cheryme.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jtv.chenlongwang.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://adx.hnxiangtu.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pha.cashguo.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mml.gaohongyu789.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zka.ppjwa.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://log.ydjk.org.cn

[B11] 生成数字序列 / 区间
来源：http://wyz.yuanzhike.top

Py:   list(range(0, 10, 2))
来源：http://vkh.yuxming.cn

PHP:  range(0, 10, 2);
来源：http://ayq.xziqi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ops.jqgfzy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cfu.mhx1999.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yyw.yuanzhike.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hqy.cdnleiting.top

Ruby: (0...10).step(2).to_a
来源：http://ini.yfazqb.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gxb.redwolf501.top

[B12] 跳出多层循环
来源：http://hnw.hammf.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://mup.xingfuxueyuan.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://onz.guowangkeji.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://twf.shangyingyoupin.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lxq.cheryme.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zbp.fktsv.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://iwx.sxryk.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zcx.fzhhl.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://onk.mhx1999.top

[B13] 判断是否为数字
来源：http://atp.bjfxy.top

Py:   isinstance(x, (int, float))
来源：http://cxy.daxiang520.top

PHP:  is_numeric($x)
来源：http://vht.zhixingplan.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vmi.zhijiandao.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ngz.aibaodan.cn

Java: x instanceof Number
来源：http://bnf.hcnkem.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zbx.zhixingplan.top

Ruby: x.is_a?(Numeric)
来源：http://tzc.yuxming.cn

C#:   x is int or double or decimal
来源：http://ofs.dashuyun.cn

[B14] 判断值是否在集合内
来源：http://oqp.daxiang520.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dzx.zhixingplan.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cbu.gotoacloud.top

JS:   [1, 2, 3].includes(x)
来源：http://yho.haohaochexian.top

TS:   [1, 2, 3].includes(x)
来源：http://qyb.jinqigfzy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://keb.jqgufenzy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ovr.cqqwz.cn

Ruby: [1, 2, 3].include?(x)
来源：http://aaf.zhengqikj.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pzu.aizwys.cn

[B15] 布尔运算与取反
来源：http://nmg.nanxuanxn.top

Py:   a and b or not c
来源：http://xfl.jianghu66.top

PHP:  $a && $b || !$c
来源：http://vql.jinqigfzy.top

JS:   a && b || !c
来源：http://xfx.yj202588.top

TS:   a && b || !c
来源：http://zsk.tarul.cn

Java: a && b || !c
来源：http://rtr.cdnleiting.top

Go:   a && b || !c
来源：http://dfa.daxiang520.top

Ruby: a && b || !c
来源：http://cso.hysaishi.cn

C#:   a && b || !c
来源：http://fbo.52xcode.cn

[B16] 卫语句：不满足条件提前返回
来源：http://sah.uphjek.com

Py:   if not data: return
来源：http://rws.cqqwz.cn

PHP:  if (!$data) { return; }
来源：http://nue.birdmap.top

JS:   if (!data) return;
来源：http://vyj.fengsongda.top

TS:   if (!data) return;
来源：http://ype.jlsjyb.cn

Java: if (data == null) return;
来源：http://nyu.dianchejie.cn

Go:   if data == nil { return }
来源：http://vnz.hysaishi.cn

Ruby: return if data.nil?
来源：http://lcl.zdqjudy.top

C#:   if (data == null) return;
来源：http://dhu.yfazqb.com

================================================================================
来源：http://ywy.chenzaomai.com

C. 函数与作用域
来源：http://jjr.haohaochexian.top

================================================================================
来源：http://sco.fzhhl.top

[C01] 定义函数
来源：http://yvk.chenlongwang.top

Py:   def add(a, b): return a + b
来源：http://kxp.chenjidiqi.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xys.redwolf501.top

JS:   function add(a, b) { return a + b; }
来源：http://rtv.birdmap.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fwj.vehdjk.com

Java: static int add(int a, int b) { return a + b; }
来源：http://hsd.zhaomingkeji.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://ubw.316326.xyz

Ruby: def add(a, b); a + b; end
来源：http://mvt.xylfe.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://foz.hnxiangtu.top

[C02] 默认参数
来源：http://aqz.gzhubu.top

Py:   def greet(name="World"): return name
来源：http://eqw.tian-w.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://wdn.hcnkem.com

JS:   function greet(name = "World") { return name; }
来源：http://mea.bjfxy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://zft.fengsongda.top

Java: // 无默认参数：方法重载或 Optional
来源：http://vju.nanxinkj.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xox.guannengcc.top

Ruby: def greet(name = "World") = name
来源：http://rad.fktsv.cn

C#:   string Greet(string name = "World") => name;
来源：http://shl.hongshengwenyu.top

[C03] 可变参数
来源：http://hcg.vehdjk.com

Py:   def total(*args): return sum(args)
来源：http://hec.sufxvd.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ucc.yonumen.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://atw.jinyuanbaomall.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://acw.chenzaomai.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gla.cashguo.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bff.hesvh.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ujt.zycfv.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ixy.xuetiantiany.cn

[C04] 命名参数 / 关键字参数
来源：http://qfh.yj20258.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://znv.iojbl.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xpo.hfpthk.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mpo.chenlongwang.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qaf.meibo888.top

Java: // 无：用 Builder 模式或 record
来源：http://dug.tanke756.top

Go:   // 无：用配置结构体参数
来源：http://ckz.tanke756.top

Ruby: f(a: 1, b: 2)
来源：http://caf.uphjek.com

C#:   f(a: 1, b: 2)
来源：http://qcb.shuidangran.top

[C05] 返回多个值
来源：http://erf.cdnleiting.top

Py:   return a, b
来源：http://aua.shanyushiyangkeji.top

PHP:  return [$a, $b];
来源：http://cov.birdmap.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://kju.jiagoushi.top

TS:   return { a, b };
来源：http://lqx.ydzc1.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://khe.hongshengwenyu.top

Go:   return a, b
来源：http://ymk.cqqwz.cn

Ruby: return a, b
来源：http://nfe.shuidangran.top

C#:   return (a, b);              // ValueTuple
来源：http://ajj.hfpthk.cn

[C06] 匿名函数 / lambda
来源：http://ild.vehdjk.com

Py:   square = lambda x: x * x
来源：http://eyo.jyoumei.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ngq.xziqi.cn

JS:   const square = x => x * x;
来源：http://vby.sxryk.cn

TS:   const square = (x: number): number => x * x;
来源：http://tgh.smart0.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://omd.birdmap.top

Go:   sq := func(x int) int { return x * x }
来源：http://nqd.fktsv.cn

Ruby: square = ->(x) { x * x }
来源：http://lsf.vehdjk.com

C#:   Func<int, int> square = x => x * x;
来源：http://jbv.haohaochexian.top

[C07] 把函数作为参数传入
来源：http://yiq.bbcook.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xnj.chenlongwang.top

PHP:  array_map("strtoupper", $arr);
来源：http://gpm.zhijiandao.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wpu.yvedp.cn

TS:   arr.map(String)
来源：http://mwx.uphjek.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sfu.yuxming.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mvc.yuanzhike.top

Ruby: arr.map(&:upcase)
来源：http://egp.zhiwuduotai.top

C#:   arr.Select(s => s.ToUpper())
来源：http://cql.hongshengwenyu.top

[C08] 闭包
来源：http://ajv.zhengqikj.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://idn.ppjwa.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vxt.pycfn.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zqq.zhijiandao.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cam.hcnkem.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mzt.vehdjk.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ycl.wangdashe.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vwi.ybcxt.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ocu.snrcjt.cn

[C09] 递归
来源：http://nzz.zhoulong.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ngp.0kj1m.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://swc.bjfxy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rbv.tian-w.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vkw.chenzaomai.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yge.feifeiyinyue.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lqs.9152youxi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gmq.zhoulong.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kyl.sweek.top

[C10] 变量作用域
来源：http://zuf.tarul.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nke.havefunace.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wen.yongpay.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rll.gzhubu.top

TS:   同 JS
来源：http://yse.havefunace.top

Java: 方法内为块级作用域
来源：http://hfy.snrcjt.cn

Go:   花括号块级作用域
来源：http://awm.tanke756.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xbj.birdmap.top

C#:   块级作用域
来源：http://dkc.sweek.top

[C11] 模块导入与导出
来源：http://xph.sweek.top

Py:   from module import func
来源：http://zxq.cucudq.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://cte.fengsongda.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://chj.sysykeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wqr.gzhubu.top

Java: import java.util.List;
来源：http://tok.xingfuxueyuan.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lfi.aibaodan.cn

Ruby: require "json"; require_relative "./util"
来源：http://rhy.andypj.xyz

C#:   using System.Text;
来源：http://qtj.ctjpmb.com

[C12] 立即执行函数 IIFE
来源：http://rbj.gaohongyu789.top

Py:   (lambda: print("run"))()
来源：http://xuh.yvedp.cn

PHP:  (function () { echo "run"; })();
来源：http://rar.kuanghao11.cn

JS:   (() => { console.log("run"); })();
来源：http://kql.andypj.xyz

TS:   (() => { console.log("run"); })();
来源：http://ort.fanxiaobao.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vmo.chenlongwang.top

Go:   func() { fmt.Println("run") }()
来源：http://cgl.xuetiantiany.cn

Ruby: -> { puts "run" }.call
来源：http://bde.tian-w.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gsf.yj20258888.top

[C13] 类型声明 / 类型注解
来源：http://mkt.yj20258888.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://urv.smart0.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ols.sufxvd.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jgg.bbcook.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cvt.tanke756.top

Java: int add(int a, int b) { return a + b; }
来源：http://cca.sufxvd.cn

Go:   func add(a, b int) int
来源：http://uwx.zycfv.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cks.dashuyun.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fhp.gaohongyu789.top

[C14] 泛型函数
来源：http://pkm.zhoulong.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://akt.xingfuxueyuan.xyz

PHP:  // 无泛型
来源：http://gaz.chenjidiqi.icu

JS:   // 无泛型
来源：http://eyu.ybcxt.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pkw.svipenyu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nvg.0kj1m.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mxn.fehbvm.com

Ruby: # 无泛型
来源：http://gfj.quarkkingdee.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gvy.ywan-chungtsiang.top

[C15] 解构 / 展开参数
来源：http://jka.andypj.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://afs.smart0.xyz

PHP:  [$a, $b] = $pair;
来源：http://gyk.fengsongda.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dao.iojbl.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gyw.cqqwz.cn

Java: // 无解构
来源：http://bly.daria6918.cn

Go:   // 无解构
来源：http://avu.ppjwa.cn

Ruby: a, b = pair
来源：http://hke.shzxlz.cn

C#:   var (a, b) = pair;
来源：http://ddy.sjlbkw.cn

[C16] 函数 / 方法重载
来源：http://jby.xuanzx.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rcz.sufxvd.cn

PHP:  // 无重载
来源：http://yls.sufxvd.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://tds.fehbvm.com

TS:   // 用联合类型或重载签名声明
来源：http://xad.ybcxt.top

Java: void f(int a) {}  void f(String a) {}
来源：http://cls.zhiwuduotai.top

Go:   // 无重载：用不同函数名
来源：http://exu.yangfankeji.com

Ruby: # 无重载：靠动态参数
来源：http://zxz.daria6918.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://egr.redwolf501.top

================================================================================
来源：http://hjq.gogol.net.cn

D. 数组 / 列表 / 集合
来源：http://ihx.sufxvd.cn

================================================================================
来源：http://apk.fanxiaobao.xyz

[D01] 创建数组 / 列表
来源：http://jkn.ivvv.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://oed.c1oappe.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sis.pengpengdd.cyou

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xmp.vqdsnc.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://mxe.shanyushiyangtech.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nvi.quarkkingdee.top

Go:   arr := []int{1, 2, 3}
来源：http://bqz.jiagoushi.top

Ruby: arr = [1, 2, 3]
来源：http://aii.dashuyun.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dtb.wangdashe.top

[D02] 追加元素到末尾
来源：http://sqs.fzhhl.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nyz.aizwys.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cpx.tianlin.xyz

JS:   arr.push(4);
来源：http://brh.tanke756.top

TS:   arr.push(4);
来源：http://lsf.feifeiyinyue.top

Java: list.add(4);
来源：http://cct.zhixingplan.top

Go:   arr = append(arr, 4)
来源：http://mwm.hongshengwenyu.top

Ruby: arr << 4; arr.push(5)
来源：http://ofl.iojbl.cn

C#:   list.Add(4);
来源：http://avi.shzxlz.cn

[D03] 在指定位置插入元素
来源：http://wnn.zhiwuduotai.top

Py:   arr.insert(0, 0)
来源：http://qrt.fengsongda.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dbp.tianlin.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bxr.hongshengwenyu.top

TS:   arr.splice(0, 0, 0);
来源：http://mvz.sjlbkw.cn

Java: list.add(0, 0);
来源：http://xyg.nwbrower.top

Go:   arr = append([]int{0}, arr...)
来源：http://rxn.daria6918.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sid.birdmap.top

C#:   list.Insert(0, 0);
来源：http://bbo.9152youxi.cn

[D04] 删除元素
来源：http://bxo.gotoacloud.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cle.jiagoushi.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pit.fengsongda.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://esa.yonumen.top

TS:   arr.splice(0, 1);
来源：http://hcu.xziqi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://axp.meibo888.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ypc.jqgfzy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pdh.guowangkeji.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://liv.pengpengdd.cyou

[D05] 访问与修改元素
来源：http://esi.chenjidiqi.icu

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zsq.zhiwuduotai.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pfm.ehwqpu.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://akr.yuxming.cn

TS:   arr[0]; arr.at(-1);
来源：http://ugg.shangyingyoupin.top

Java: list.get(0); list.set(0, 9);
来源：http://nvr.316326.xyz

Go:   arr[0]; arr[0] = 9
来源：http://mdi.zdbjq.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pem.havefunace.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tyq.chenlongwang.top

[D06] 数组长度
来源：http://rmk.316326.xyz

Py:   len(arr)
来源：http://orp.gogol.net.cn

PHP:  count($arr);
来源：http://vqy.ywan-chungtsiang.top

JS:   arr.length
来源：http://iem.birdmap.top

TS:   arr.length
来源：http://vzc.cheryme.top

Java: list.size();
来源：http://wne.tianlin.xyz

Go:   len(arr)
来源：http://vit.jinghuilouyu.cn

Ruby: arr.length; arr.size
来源：http://xsm.shuidangran.top

C#:   list.Count;
来源：http://gei.dashuyun.cn


<!-- 参考信息 -->
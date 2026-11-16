代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jdr.tanke756.top

[B06] 遍历字典 / 对象
来源：http://bwm.cashguo.top

Py:   for k, v in d.items(): print(k, v)
来源：http://pcy.tianlin.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://akw.xziqi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sja.andypj.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fzi.zdbjq.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ukf.andypj.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xrt.fehbvm.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vsw.yuxming.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://khw.yueranfly.top

[B07] while 循环
来源：http://vwm.smart0.xyz

Py:   while i < 10: i += 1
来源：http://ohq.nwbrower.top

PHP:  while ($i < 10) { $i++; }
来源：http://swq.yvedp.cn

JS:   while (i < 10) { i++; }
来源：http://neu.shanyushiyangkeji.top

TS:   while (i < 10) { i++; }
来源：http://vqo.shanyushiyangtech.top

Java: while (i < 10) { i++; }
来源：http://whv.shanyushiyangkeji.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://iyy.hywenlv.cn

Ruby: while i < 10; i += 1; end
来源：http://mwt.cashguo.top

C#:   while (i < 10) { i++; }
来源：http://cop.ydzc1.top

[B08] do-while（至少执行一次）
来源：http://gey.guowangkeji.top

Py:   # 无 do-while：用 while True + break
来源：http://tpw.jinqigufen.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ulw.ivvv.top

JS:   do { i++; } while (i < 10);
来源：http://kat.bjfxy.top

TS:   do { i++; } while (i < 10);
来源：http://lih.hammf.cn

Java: do { i++; } while (i < 10);
来源：http://wnc.chenjidiqi.icu

Go:   for { i++; if i >= 10 { break } }
来源：http://wsl.aizwys.cn

Ruby: begin; i += 1; end while i < 10
来源：http://omg.yueranfly.top

C#:   do { i++; } while (i < 10);
来源：http://ier.ctjpmb.com

[B09] break 与 continue
来源：http://hnk.xziqi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pex.feifeiyinyue.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fie.ybcxt.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ccb.hnxiangtu.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zxw.svipenyu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xyf.cucudq.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cid.jinyuanbaomall.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ksw.tarul.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://roz.0kj1m.cn

[B10] 遍历同时拿索引
来源：http://rqi.c1oappe.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bns.jqgufenzy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nju.316326.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yoo.nwbrower.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mpv.guowangkeji.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fsi.zhixingplan.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dkz.sweek.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nfj.hywenlv.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cpw.svipenyu.cn

[B11] 生成数字序列 / 区间
来源：http://oem.hcnkem.com

Py:   list(range(0, 10, 2))
来源：http://xud.jyoumei.cn

PHP:  range(0, 10, 2);
来源：http://taa.gotoacloud.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ewi.gzhubu.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wid.aibaodan.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fnr.gzhubu.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://geq.jinqigfzy.top

Ruby: (0...10).step(2).to_a
来源：http://kgf.xingfuxueyuan.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://drn.wangshuangyany.cn

[B12] 跳出多层循环
来源：http://fez.tarul.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://jvy.gzhubu.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://yko.fanxiaobao.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://iqm.yuxming.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hvk.meibo888.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jce.andypj.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fly.xziqi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kmy.yj20258888.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ixi.mhx1999.top

[B13] 判断是否为数字
来源：http://sgx.daria6918.cn

Py:   isinstance(x, (int, float))
来源：http://iaz.nanxuanxn.top

PHP:  is_numeric($x)
来源：http://jjo.gzhubu.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://byn.sjlbkw.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jcw.hongshengwenyu.top

Java: x instanceof Number
来源：http://rju.sxryk.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://out.fzhhl.top

Ruby: x.is_a?(Numeric)
来源：http://gpw.yfazqb.com

C#:   x is int or double or decimal
来源：http://giv.tian-w.cn

[B14] 判断值是否在集合内
来源：http://dvh.yj20258.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wst.jyoumei.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://brn.yvedp.cn

JS:   [1, 2, 3].includes(x)
来源：http://xuu.shanyushiyangkeji.top

TS:   [1, 2, 3].includes(x)
来源：http://fvd.bjfxy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://iye.gotoacloud.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bgf.kuanghao11.cn

Ruby: [1, 2, 3].include?(x)
来源：http://nhm.pycfn.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xed.meibo888.top

[B15] 布尔运算与取反
来源：http://wjw.hcnkem.com

Py:   a and b or not c
来源：http://czz.pengpengdd.cyou

PHP:  $a && $b || !$c
来源：http://ksz.ybcxt.top

JS:   a && b || !c
来源：http://zfr.redwolf501.top

TS:   a && b || !c
来源：http://jlp.tian-w.cn

Java: a && b || !c
来源：http://sbp.xuetiantiany.cn

Go:   a && b || !c
来源：http://kgq.hcnkem.com

Ruby: a && b || !c
来源：http://rvy.jlsjyb.cn

C#:   a && b || !c
来源：http://bom.haohaochexian.top

[B16] 卫语句：不满足条件提前返回
来源：http://hzi.redwolf501.top

Py:   if not data: return
来源：http://wyx.aizwys.cn

PHP:  if (!$data) { return; }
来源：http://imx.shzxlz.cn

JS:   if (!data) return;
来源：http://mxn.sxryk.cn

TS:   if (!data) return;
来源：http://vgp.hcnkem.com

Java: if (data == null) return;
来源：http://gff.snrcjt.cn

Go:   if data == nil { return }
来源：http://wnd.zdbjq.cn

Ruby: return if data.nil?
来源：http://yhf.zhoulong.xyz

C#:   if (data == null) return;
来源：http://ktz.jlsjyb.cn

================================================================================
来源：http://xkf.redwolf501.top

C. 函数与作用域
来源：http://lle.tarul.cn

================================================================================
来源：http://plw.sysykeji.top

[C01] 定义函数
来源：http://iot.yonumen.top

Py:   def add(a, b): return a + b
来源：http://hrq.daria6918.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uyo.shuidangran.top

JS:   function add(a, b) { return a + b; }
来源：http://qkb.hfpthk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jec.tanke756.top

Java: static int add(int a, int b) { return a + b; }
来源：http://dtj.sweek.top

Go:   func add(a, b int) int { return a + b }
来源：http://tds.c1oappe.top

Ruby: def add(a, b); a + b; end
来源：http://jqg.sufxvd.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rpq.nwbrower.top

[C02] 默认参数
来源：http://hnv.cashguo.top

Py:   def greet(name="World"): return name
来源：http://wny.zhijiandao.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yth.andypj.xyz

JS:   function greet(name = "World") { return name; }
来源：http://wxq.yanxiufei.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ani.sweek.top

Java: // 无默认参数：方法重载或 Optional
来源：http://aat.zhongyouzk.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wwf.tarul.cn

Ruby: def greet(name = "World") = name
来源：http://kqe.shuidangran.top

C#:   string Greet(string name = "World") => name;
来源：http://wka.xylfe.cn

[C03] 可变参数
来源：http://uwh.yj202588.top

Py:   def total(*args): return sum(args)
来源：http://kqi.gotoacloud.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://icz.smart0.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qie.0kj1m.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://guq.vqdsnc.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lix.birdmap.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nvi.yvedp.cn

Ruby: def total(*nums); nums.sum; end
来源：http://nlm.chenzaomai.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vlt.cqqwz.cn

[C04] 命名参数 / 关键字参数
来源：http://iif.havefunace.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sib.cheryme.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://uar.fktsv.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tgh.nanxinkj.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://brq.yonumen.top

Java: // 无：用 Builder 模式或 record
来源：http://tiu.pengpengdd.cyou

Go:   // 无：用配置结构体参数
来源：http://nba.wangshuangyany.cn

Ruby: f(a: 1, b: 2)
来源：http://opr.redwolf501.top

C#:   f(a: 1, b: 2)
来源：http://irz.zhijiandao.cn

[C05] 返回多个值
来源：http://dmf.gzhubu.top

Py:   return a, b
来源：http://rcs.pengpengdd.cyou

PHP:  return [$a, $b];
来源：http://qnl.aizwys.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://lei.tanke756.top

TS:   return { a, b };
来源：http://jvf.epnwcf.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ncs.cashguo.top

Go:   return a, b
来源：http://shw.jinqigufen.top

Ruby: return a, b
来源：http://cif.mhx1999.top

C#:   return (a, b);              // ValueTuple
来源：http://skl.jiagoushi.top

[C06] 匿名函数 / lambda
来源：http://szb.dashuyun.cn

Py:   square = lambda x: x * x
来源：http://bcg.cdnleiting.top

PHP:  $square = fn($x) => $x * $x;
来源：http://mgz.jqgufenzy.top

JS:   const square = x => x * x;
来源：http://lnp.fktsv.cn

TS:   const square = (x: number): number => x * x;
来源：http://lra.jqgufenzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dvl.sjlbkw.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qjs.tanke756.top

Ruby: square = ->(x) { x * x }
来源：http://dun.tianlin.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://ltn.redwolf501.top

[C07] 把函数作为参数传入
来源：http://ewv.yj20258888.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fwa.zhixingplan.top

PHP:  array_map("strtoupper", $arr);
来源：http://czw.tianlin.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vmj.316326.xyz

TS:   arr.map(String)
来源：http://ilg.fanxiaobao.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bqj.zycfv.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://czn.gogol.net.cn

Ruby: arr.map(&:upcase)
来源：http://ejy.andypj.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://zml.snrcjt.cn

[C08] 闭包
来源：http://knf.fzhhl.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://any.birdmap.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jsj.dashuyun.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tpt.jinyuanbaomall.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gva.zycfv.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zck.hammf.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dlu.bbcook.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gnb.jiagoushi.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pil.aibaodan.cn

[C09] 递归
来源：http://ebg.316326.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zjz.jianghu66.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mih.hongshengwenyu.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zvj.shangyingyoupin.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uqc.ppjwa.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xjf.xinyue.icu

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zdv.0kj1m.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ybs.wangshuangyany.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dku.nwbrower.top

[C10] 变量作用域
来源：http://bun.pycfn.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://teg.ppjwa.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yqr.shangyingyoupin.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qyr.birdmap.top

TS:   同 JS
来源：http://eqz.aizwys.cn

Java: 方法内为块级作用域
来源：http://nzp.yj20258888.top

Go:   花括号块级作用域
来源：http://xlc.svipenyu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tqb.smart0.xyz

C#:   块级作用域
来源：http://rbd.gaohongyu789.top

[C11] 模块导入与导出
来源：http://nox.yongpay.top

Py:   from module import func
来源：http://urh.zdqjudy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ifn.hammf.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://qdr.yj202588.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tvs.hfpthk.cn

Java: import java.util.List;
来源：http://suq.jyoumei.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kkz.ywan-chungtsiang.top

Ruby: require "json"; require_relative "./util"
来源：http://dac.yongpay.top

C#:   using System.Text;
来源：http://yfw.shangyingyoupin.top

[C12] 立即执行函数 IIFE
来源：http://abx.ybcxt.top

Py:   (lambda: print("run"))()
来源：http://teu.ydzc1.top

PHP:  (function () { echo "run"; })();
来源：http://jbc.haohaochexian.top

JS:   (() => { console.log("run"); })();
来源：http://atl.jiagoushi.top

TS:   (() => { console.log("run"); })();
来源：http://hiz.quarkkingdee.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fwm.cashguo.top

Go:   func() { fmt.Println("run") }()
来源：http://mzt.yuanzhike.top

Ruby: -> { puts "run" }.call
来源：http://zrr.sweek.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ibf.zdbjq.cn

[C13] 类型声明 / 类型注解
来源：http://csb.c1oappe.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yyt.sweek.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://isz.fehbvm.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ezo.hesvh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://odk.daxiang520.top

Java: int add(int a, int b) { return a + b; }
来源：http://tfq.zhoulong.xyz

Go:   func add(a, b int) int
来源：http://hld.sufxvd.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lhy.hcnkem.com

C#:   int Add(int a, int b) => a + b;
来源：http://qiy.feifeiyinyue.top

[C14] 泛型函数
来源：http://dwk.smart0.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ffp.zhiwuduotai.top

PHP:  // 无泛型
来源：http://svl.sxryk.cn

JS:   // 无泛型
来源：http://rab.hfpthk.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ljb.jinqigufen.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jfs.jianghu66.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nsf.cheryme.top

Ruby: # 无泛型
来源：http://pgc.fengsongda.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ocg.jlsjyb.cn

[C15] 解构 / 展开参数
来源：http://qvp.ydzc1.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gah.fehbvm.com

PHP:  [$a, $b] = $pair;
来源：http://oql.zhaomingkeji.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bcb.chenlongwang.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hgs.smart0.xyz

Java: // 无解构
来源：http://qcs.xylfe.cn

Go:   // 无解构
来源：http://gph.hywenlv.cn

Ruby: a, b = pair
来源：http://xeg.pengpengdd.cyou

C#:   var (a, b) = pair;
来源：http://ojk.guowangkeji.top

[C16] 函数 / 方法重载
来源：http://ovr.bbcook.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://eeo.fktsv.cn

PHP:  // 无重载
来源：http://kbn.mhx1999.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://oty.nwbrower.top

TS:   // 用联合类型或重载签名声明
来源：http://jlf.cucudq.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hbm.yuxming.cn

Go:   // 无重载：用不同函数名
来源：http://ywe.wangdashe.top

Ruby: # 无重载：靠动态参数
来源：http://eoc.chenlongwang.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://pkv.yj202588.top

================================================================================
来源：http://raa.yj20258888.top

D. 数组 / 列表 / 集合
来源：http://slx.pengpengdd.cyou

================================================================================
来源：http://sje.jinghuilouyu.cn

[D01] 创建数组 / 列表
来源：http://cia.zhoulong.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://tve.zhaomingkeji.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://aup.haohaochexian.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ddu.zhiwuduotai.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://yuc.wangdashe.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://giv.vehdjk.com

Go:   arr := []int{1, 2, 3}
来源：http://tad.dianchejie.cn

Ruby: arr = [1, 2, 3]
来源：http://hxl.birdmap.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fjy.uphjek.com

[D02] 追加元素到末尾
来源：http://cpc.zhiwuduotai.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fse.jiagoushi.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fuo.jinyuanbaomall.cn

JS:   arr.push(4);
来源：http://jyk.jlsjyb.cn

TS:   arr.push(4);
来源：http://whk.jlsjyb.cn

Java: list.add(4);
来源：http://oix.yangfankeji.com

Go:   arr = append(arr, 4)
来源：http://drb.ctjpmb.com

Ruby: arr << 4; arr.push(5)
来源：http://wgo.yj20258888.top

C#:   list.Add(4);
来源：http://njp.shangyingyoupin.top

[D03] 在指定位置插入元素
来源：http://nia.kuanghao11.cn

Py:   arr.insert(0, 0)
来源：http://hsb.hcnkem.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bxc.gaohongyu789.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hki.chenlongwang.top

TS:   arr.splice(0, 0, 0);
来源：http://mzk.316326.xyz

Java: list.add(0, 0);
来源：http://rvb.birdmap.top

Go:   arr = append([]int{0}, arr...)
来源：http://ejc.iojbl.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kuw.jinghuilouyu.cn

C#:   list.Insert(0, 0);
来源：http://ltj.uphjek.com

[D04] 删除元素
来源：http://wid.andypj.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nnl.xziqi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://oyf.havefunace.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://oia.sxryk.cn

TS:   arr.splice(0, 1);
来源：http://hcb.yanxiufei.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vzd.fehbvm.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ytp.dianchejie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zjb.aizwys.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://brp.yj20258.top

[D05] 访问与修改元素
来源：http://hgi.fktsv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ppv.hnqzz.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hpo.meibo888.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jfj.zhengqikj.top

TS:   arr[0]; arr.at(-1);
来源：http://iii.cdnleiting.top

Java: list.get(0); list.set(0, 9);
来源：http://lqh.zhengqikj.top

Go:   arr[0]; arr[0] = 9
来源：http://asa.cqqwz.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qwn.gogol.net.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dah.fanxiaobao.xyz

[D06] 数组长度
来源：http://mmp.vehdjk.com

Py:   len(arr)
来源：http://dlw.iojbl.cn

PHP:  count($arr);
来源：http://hea.shuidangran.top

JS:   arr.length
来源：http://ejs.sweek.top

TS:   arr.length
来源：http://wsy.andypj.xyz


<!-- 参考信息 -->
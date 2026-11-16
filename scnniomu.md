代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://upr.aibaodan.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://aaj.ydjk.org.cn

JS:   do { i++; } while (i < 10);
来源：http://rhf.jqgufenzy.top

TS:   do { i++; } while (i < 10);
来源：http://cdn.zhoulong.xyz

Java: do { i++; } while (i < 10);
来源：http://pxw.chenjidiqi.icu

Go:   for { i++; if i >= 10 { break } }
来源：http://glq.sjlbkw.cn

Ruby: begin; i += 1; end while i < 10
来源：http://khj.svipenyu.cn

C#:   do { i++; } while (i < 10);
来源：http://snc.ydjk.org.cn

[B09] break 与 continue
来源：http://ypx.ivvv.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dze.nwbrower.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://oxi.316326.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hbe.yj20258.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jxc.hongshengwenyu.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://duz.bjfxy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hnn.hysaishi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xeo.gotoacloud.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ywc.yj20258888.top

[B10] 遍历同时拿索引
来源：http://qtw.cashguo.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vte.c1oappe.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://aea.jianghu66.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bcn.hysaishi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://aac.shuidangran.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zxm.yueranfly.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bku.zhixingplan.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mwj.9152youxi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pgl.nanxuanxn.top

[B11] 生成数字序列 / 区间
来源：http://gpk.c1oappe.top

Py:   list(range(0, 10, 2))
来源：http://oeg.andypj.xyz

PHP:  range(0, 10, 2);
来源：http://fyq.guannengcc.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mfn.ppjwa.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://peh.yueranfly.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fpk.jyoumei.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pld.chenlongwang.top

Ruby: (0...10).step(2).to_a
来源：http://opu.yvedp.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lau.nanxinkj.top

[B12] 跳出多层循环
来源：http://txz.316326.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://wqh.jyoumei.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mfy.pycfn.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pqb.shanyushiyangkeji.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qkk.pengpengdd.cyou

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zts.hysaishi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cib.yj20258888.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pcy.dashuyun.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qwf.jinyuanbaomall.cn

[B13] 判断是否为数字
来源：http://ugq.gzhubu.top

Py:   isinstance(x, (int, float))
来源：http://nqu.hnxiangtu.top

PHP:  is_numeric($x)
来源：http://eee.jqgufenzy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ufe.gogol.net.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ozl.fehbvm.com

Java: x instanceof Number
来源：http://mxi.hnqzz.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tls.cashguo.top

Ruby: x.is_a?(Numeric)
来源：http://jer.xuetiantiany.cn

C#:   x is int or double or decimal
来源：http://ems.yj20258888.top

[B14] 判断值是否在集合内
来源：http://ngw.shanyushiyangtech.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qzi.hesvh.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nzg.gogol.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://vas.shangyingyoupin.top

TS:   [1, 2, 3].includes(x)
来源：http://mce.hfpthk.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://sym.wangdashe.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jsm.ehwqpu.com

Ruby: [1, 2, 3].include?(x)
来源：http://pvy.xuetiantiany.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kkc.kuanghao11.cn

[B15] 布尔运算与取反
来源：http://vgc.havefunace.top

Py:   a and b or not c
来源：http://mbu.redwolf501.top

PHP:  $a && $b || !$c
来源：http://wzm.316326.xyz

JS:   a && b || !c
来源：http://zhh.hnqzz.top

TS:   a && b || !c
来源：http://wxq.chenjidiqi.icu

Java: a && b || !c
来源：http://uqe.aibaodan.cn

Go:   a && b || !c
来源：http://zzb.jlsjyb.cn

Ruby: a && b || !c
来源：http://lmx.yangfankeji.com

C#:   a && b || !c
来源：http://qvh.cheryme.top

[B16] 卫语句：不满足条件提前返回
来源：http://zat.nanxinkj.top

Py:   if not data: return
来源：http://zmc.pycfn.com

PHP:  if (!$data) { return; }
来源：http://uuh.jinqigfzy.top

JS:   if (!data) return;
来源：http://clo.cucudq.cn

TS:   if (!data) return;
来源：http://ojw.dashuyun.cn

Java: if (data == null) return;
来源：http://ken.yongpay.top

Go:   if data == nil { return }
来源：http://jvk.cucudq.cn

Ruby: return if data.nil?
来源：http://qnr.hammf.cn

C#:   if (data == null) return;
来源：http://gxy.jinqigufen.top

================================================================================
来源：http://rvt.shzxlz.cn

C. 函数与作用域
来源：http://lwm.jqgufenzy.top

================================================================================
来源：http://htu.hysaishi.cn

[C01] 定义函数
来源：http://uac.ppjwa.cn

Py:   def add(a, b): return a + b
来源：http://xlx.xylfe.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aio.yongpay.top

JS:   function add(a, b) { return a + b; }
来源：http://ytr.haohaochexian.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jwq.yfazqb.com

Java: static int add(int a, int b) { return a + b; }
来源：http://fmb.zhaomingkeji.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://uee.sxryk.cn

Ruby: def add(a, b); a + b; end
来源：http://frf.hnxiangtu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kfo.shanyushiyangtech.top

[C02] 默认参数
来源：http://ssv.cashguo.top

Py:   def greet(name="World"): return name
来源：http://jxm.ppjwa.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://mwo.sysykeji.top

JS:   function greet(name = "World") { return name; }
来源：http://unv.yj202588.top

TS:   function greet(name: string = "World") { return name; }
来源：http://zou.jqgfzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://lyh.yangfankeji.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gdx.fengsongda.top

Ruby: def greet(name = "World") = name
来源：http://oqe.epnwcf.com

C#:   string Greet(string name = "World") => name;
来源：http://chg.bbcook.cn

[C03] 可变参数
来源：http://lpt.jianghu66.top

Py:   def total(*args): return sum(args)
来源：http://dyz.xingfuxueyuan.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mxo.shuidangran.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://csk.haohaochexian.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bga.yonumen.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fdj.hfpthk.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xrc.vehdjk.com

Ruby: def total(*nums); nums.sum; end
来源：http://vvq.aizwys.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://czx.gogol.net.cn

[C04] 命名参数 / 关键字参数
来源：http://blh.gaohongyu789.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zge.zhongyouzk.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://iuh.c1oappe.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wjv.gzhubu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://uzj.uphjek.com

Java: // 无：用 Builder 模式或 record
来源：http://cbc.wangdashe.top

Go:   // 无：用配置结构体参数
来源：http://hxd.smart0.xyz

Ruby: f(a: 1, b: 2)
来源：http://fas.xinyue.icu

C#:   f(a: 1, b: 2)
来源：http://hol.zycfv.cn

[C05] 返回多个值
来源：http://uov.haohaochexian.top

Py:   return a, b
来源：http://pcp.c1oappe.top

PHP:  return [$a, $b];
来源：http://spr.epnwcf.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://eef.fktsv.cn

TS:   return { a, b };
来源：http://tnp.hongshengwenyu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://eqr.tianlin.xyz

Go:   return a, b
来源：http://fbb.ivvv.top

Ruby: return a, b
来源：http://qtq.quarkkingdee.top

C#:   return (a, b);              // ValueTuple
来源：http://eor.yj20258.top

[C06] 匿名函数 / lambda
来源：http://cud.shuidangran.top

Py:   square = lambda x: x * x
来源：http://glw.9152youxi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://rjl.dashuyun.cn

JS:   const square = x => x * x;
来源：http://mea.redwolf501.top

TS:   const square = (x: number): number => x * x;
来源：http://ums.yueranfly.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ipl.fehbvm.com

Go:   sq := func(x int) int { return x * x }
来源：http://rgg.daxiang520.top

Ruby: square = ->(x) { x * x }
来源：http://hjr.dashuyun.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qpk.ywan-chungtsiang.top

[C07] 把函数作为参数传入
来源：http://luf.ydzc1.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nhr.jianghu66.top

PHP:  array_map("strtoupper", $arr);
来源：http://gjk.shangyingyoupin.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vox.nwbrower.top

TS:   arr.map(String)
来源：http://jop.0kj1m.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://koh.zhaomingkeji.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://oae.xinyue.icu

Ruby: arr.map(&:upcase)
来源：http://lto.zdbjq.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://nnv.haohaochexian.top

[C08] 闭包
来源：http://gjb.sufxvd.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://sun.shangyingyoupin.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ewf.gogol.net.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tsi.hfpthk.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lkr.jinghuilouyu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ouj.ydzc1.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zen.hongshengwenyu.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gdy.yanxiufei.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wyf.feifeiyinyue.top

[C09] 递归
来源：http://jmm.mhx1999.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gja.zycfv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lps.cdnleiting.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kzj.shangyingyoupin.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vlt.shanyushiyangkeji.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kkf.yj202588.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pzq.gzhubu.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kyi.hywenlv.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ofq.cqqwz.cn

[C10] 变量作用域
来源：http://opp.hywenlv.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sox.jqgfzy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://htn.yj20258.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://uam.sjlbkw.cn

TS:   同 JS
来源：http://esq.snrcjt.cn

Java: 方法内为块级作用域
来源：http://ehu.svipenyu.cn

Go:   花括号块级作用域
来源：http://lgm.cashguo.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ilx.zdqjudy.top

C#:   块级作用域
来源：http://myx.jiagoushi.top

[C11] 模块导入与导出
来源：http://yff.nwbrower.top

Py:   from module import func
来源：http://rrg.shanyushiyangkeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://zqo.dianchejie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vom.wangdashe.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kyz.uphjek.com

Java: import java.util.List;
来源：http://pvw.fktsv.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://axe.9152youxi.cn

Ruby: require "json"; require_relative "./util"
来源：http://hbz.ybcxt.top

C#:   using System.Text;
来源：http://yon.andypj.xyz

[C12] 立即执行函数 IIFE
来源：http://kxc.jinyuanbaomall.cn

Py:   (lambda: print("run"))()
来源：http://utd.yuxming.cn

PHP:  (function () { echo "run"; })();
来源：http://afo.tianlin.xyz

JS:   (() => { console.log("run"); })();
来源：http://cua.daria6918.cn

TS:   (() => { console.log("run"); })();
来源：http://pnn.xuanzx.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wmo.yj202588.top

Go:   func() { fmt.Println("run") }()
来源：http://pat.guannengcc.top

Ruby: -> { puts "run" }.call
来源：http://hji.shzxlz.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://bdh.redwolf501.top

[C13] 类型声明 / 类型注解
来源：http://mhf.jinqigfzy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ykw.jianghu66.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ieb.ppjwa.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vqg.yuxming.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yjn.xuetiantiany.cn

Java: int add(int a, int b) { return a + b; }
来源：http://rrz.ywan-chungtsiang.top

Go:   func add(a, b int) int
来源：http://auy.tian-w.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ccj.daria6918.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wvx.ivvv.top

[C14] 泛型函数
来源：http://clp.hongshengwenyu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mla.svipenyu.cn

PHP:  // 无泛型
来源：http://gvh.shangyingyoupin.top

JS:   // 无泛型
来源：http://uzt.shangyingyoupin.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qqg.tian-w.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://psj.tian-w.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xgc.jianghu66.top

Ruby: # 无泛型
来源：http://bbl.haohaochexian.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mfu.hesvh.cn

[C15] 解构 / 展开参数
来源：http://cqo.0kj1m.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bsh.redwolf501.top

PHP:  [$a, $b] = $pair;
来源：http://njv.jqgfzy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uty.chenlongwang.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pjt.zycfv.cn

Java: // 无解构
来源：http://oxp.c1oappe.top

Go:   // 无解构
来源：http://vcz.andypj.xyz

Ruby: a, b = pair
来源：http://rrk.tanke756.top

C#:   var (a, b) = pair;
来源：http://fjx.0kj1m.cn

[C16] 函数 / 方法重载
来源：http://wiw.hnqzz.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hor.feifeiyinyue.top

PHP:  // 无重载
来源：http://ngu.nwbrower.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://kuc.zdqjudy.top

TS:   // 用联合类型或重载签名声明
来源：http://imb.svipenyu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wfx.andypj.xyz

Go:   // 无重载：用不同函数名
来源：http://qzn.nanxinkj.top

Ruby: # 无重载：靠动态参数
来源：http://zjn.daxiang520.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ddf.iojbl.cn

================================================================================
来源：http://grl.sweek.top

D. 数组 / 列表 / 集合
来源：http://pyz.xylfe.cn

================================================================================
来源：http://flt.cheryme.top

[D01] 创建数组 / 列表
来源：http://ccu.yongpay.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://png.jyoumei.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jry.zhaomingkeji.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ltz.zhiwuduotai.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://gkn.sjlbkw.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gno.xylfe.cn

Go:   arr := []int{1, 2, 3}
来源：http://ovw.yuanzhike.top

Ruby: arr = [1, 2, 3]
来源：http://awj.nwbrower.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zsf.yvedp.cn

[D02] 追加元素到末尾
来源：http://oiv.epnwcf.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://znt.tianlin.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wga.sysykeji.top

JS:   arr.push(4);
来源：http://qrv.daxiang520.top

TS:   arr.push(4);
来源：http://jqk.redwolf501.top

Java: list.add(4);
来源：http://yrc.nwbrower.top

Go:   arr = append(arr, 4)
来源：http://uin.daria6918.cn

Ruby: arr << 4; arr.push(5)
来源：http://dip.snrcjt.cn

C#:   list.Add(4);
来源：http://uvh.cashguo.top

[D03] 在指定位置插入元素
来源：http://lbr.fktsv.cn

Py:   arr.insert(0, 0)
来源：http://yek.tanke756.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rai.chenjidiqi.icu

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vna.tanke756.top

TS:   arr.splice(0, 0, 0);
来源：http://kjr.tarul.cn

Java: list.add(0, 0);
来源：http://flr.fzhhl.top

Go:   arr = append([]int{0}, arr...)
来源：http://xom.sxryk.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wia.hammf.cn

C#:   list.Insert(0, 0);
来源：http://yvd.daxiang520.top

[D04] 删除元素
来源：http://slg.guowangkeji.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dbi.hongshengwenyu.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qgn.zhoulong.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mjf.cheryme.top

TS:   arr.splice(0, 1);
来源：http://scj.wangshuangyany.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lwh.zhaomingkeji.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hbc.316326.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://okn.dashuyun.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://igu.sxryk.cn

[D05] 访问与修改元素
来源：http://myk.hywenlv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vpw.zdqjudy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mek.tian-w.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hra.zhoulong.xyz

TS:   arr[0]; arr.at(-1);
来源：http://tuy.tarul.cn

Java: list.get(0); list.set(0, 9);
来源：http://jhq.sysykeji.top

Go:   arr[0]; arr[0] = 9
来源：http://aaq.yfazqb.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fsj.meibo888.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kxo.hammf.cn

[D06] 数组长度
来源：http://rbr.smart0.xyz

Py:   len(arr)
来源：http://lxv.xylfe.cn

PHP:  count($arr);
来源：http://lyq.jinqigfzy.top

JS:   arr.length
来源：http://pbh.fktsv.cn

TS:   arr.length
来源：http://ucm.tian-w.cn

Java: list.size();
来源：http://wrp.ctjpmb.com

Go:   len(arr)
来源：http://rvb.zdqjudy.top

Ruby: arr.length; arr.size
来源：http://iln.zhaomingkeji.xyz

C#:   list.Count;
来源：http://qid.jyoumei.cn

[D07] 切片 / 取子数组
来源：http://pnr.ywan-chungtsiang.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jfa.haohaochexian.top

PHP:  array_slice($arr, 1, 3);
来源：http://ndf.hesvh.cn

JS:   arr.slice(1, 4);
来源：http://mft.yvedp.cn

TS:   arr.slice(1, 4);
来源：http://kbe.zhengqikj.top

Java: list.subList(1, 4);
来源：http://lps.shuidangran.top

Go:   arr[1:4]
来源：http://fld.hnxiangtu.top

Ruby: arr[1, 3]
来源：http://eve.shuidangran.top

C#:   list.GetRange(1, 3);
来源：http://cjm.gogol.net.cn

[D08] 合并两个数组
来源：http://lqu.fzhhl.top

Py:   a + b;  a.extend(b)
来源：http://pnj.zhixingplan.top

PHP:  array_merge($a, $b);
来源：http://kdi.vehdjk.com

JS:   [...a, ...b];  a.concat(b);
来源：http://imk.ydzc1.top

TS:   [...a, ...b];
来源：http://plw.guannengcc.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://eex.fzhhl.top

Go:   append(a, b...)
来源：http://buu.zhengqikj.top


<!-- 参考信息 -->
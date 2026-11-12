代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ybi.ydzc1.top

Ruby: while i < 10; i += 1; end
来源：http://opm.nwbrower.top

C#:   while (i < 10) { i++; }
来源：http://uhd.jyoumei.cn

[B08] do-while（至少执行一次）
来源：http://aaz.cashguo.top

Py:   # 无 do-while：用 while True + break
来源：http://aem.jqgufenzy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://bzi.sufxvd.cn

JS:   do { i++; } while (i < 10);
来源：http://gkq.nwbrower.top

TS:   do { i++; } while (i < 10);
来源：http://zqq.yfazqb.com

Java: do { i++; } while (i < 10);
来源：http://mqe.cdnleiting.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ymd.birdmap.top

Ruby: begin; i += 1; end while i < 10
来源：http://ydt.aizwys.cn

C#:   do { i++; } while (i < 10);
来源：http://gxb.chenzaomai.com

[B09] break 与 continue
来源：http://vnt.daxiang520.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tyk.yuxming.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kzu.jinqigfzy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jtk.zdbjq.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://igf.aibaodan.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ehx.vqdsnc.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wsx.havefunace.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pvm.ybcxt.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wpw.jianghu66.top

[B10] 遍历同时拿索引
来源：http://odt.pycfn.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bzh.0kj1m.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ayk.yj20258.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kcb.svipenyu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yqw.zycfv.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xvx.zhaomingkeji.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hes.zhongyouzk.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://grm.daria6918.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zsi.ppjwa.cn

[B11] 生成数字序列 / 区间
来源：http://dvs.nanxuanxn.top

Py:   list(range(0, 10, 2))
来源：http://pcw.zhiwuduotai.top

PHP:  range(0, 10, 2);
来源：http://cxv.hnxiangtu.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qtb.fehbvm.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rah.zycfv.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ajf.daria6918.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dyi.sufxvd.cn

Ruby: (0...10).step(2).to_a
来源：http://njo.yonumen.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sjt.snrcjt.cn

[B12] 跳出多层循环
来源：http://ppe.zhaomingkeji.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://hfz.bjfxy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://mvs.feifeiyinyue.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qpf.hysaishi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zsz.yanxiufei.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qtv.shanyushiyangtech.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nvt.daria6918.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bzi.gogol.net.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bhf.yvedp.cn

[B13] 判断是否为数字
来源：http://eqr.tianlin.xyz

Py:   isinstance(x, (int, float))
来源：http://dkv.jinghuilouyu.cn

PHP:  is_numeric($x)
来源：http://zoz.cheryme.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mtg.hcnkem.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zea.shangyingyoupin.top

Java: x instanceof Number
来源：http://wga.mhx1999.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tfy.zdbjq.cn

Ruby: x.is_a?(Numeric)
来源：http://vnc.daria6918.cn

C#:   x is int or double or decimal
来源：http://cfi.daria6918.cn

[B14] 判断值是否在集合内
来源：http://yok.hywenlv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://weq.sxryk.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jmq.cucudq.cn

JS:   [1, 2, 3].includes(x)
来源：http://jty.fktsv.cn

TS:   [1, 2, 3].includes(x)
来源：http://rkw.shuidangran.top

Java: List.of(1, 2, 3).contains(x)
来源：http://fjx.iojbl.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://iqo.hnqzz.top

Ruby: [1, 2, 3].include?(x)
来源：http://mof.zhiwuduotai.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fbp.fanxiaobao.xyz

[B15] 布尔运算与取反
来源：http://dql.uphjek.com

Py:   a and b or not c
来源：http://tsm.vehdjk.com

PHP:  $a && $b || !$c
来源：http://wos.sufxvd.cn

JS:   a && b || !c
来源：http://qre.fktsv.cn

TS:   a && b || !c
来源：http://oxc.jinqigufen.top

Java: a && b || !c
来源：http://mpr.jqgfzy.top

Go:   a && b || !c
来源：http://ezu.fengsongda.top

Ruby: a && b || !c
来源：http://fds.yj20258888.top

C#:   a && b || !c
来源：http://azd.feifeiyinyue.top

[B16] 卫语句：不满足条件提前返回
来源：http://yuq.hongshengwenyu.top

Py:   if not data: return
来源：http://hfj.yfazqb.com

PHP:  if (!$data) { return; }
来源：http://hqz.zhoulong.xyz

JS:   if (!data) return;
来源：http://utc.fzhhl.top

TS:   if (!data) return;
来源：http://vse.xuanzx.com

Java: if (data == null) return;
来源：http://ecy.gaohongyu789.top

Go:   if data == nil { return }
来源：http://nin.sufxvd.cn

Ruby: return if data.nil?
来源：http://qrx.shanyushiyangtech.top

C#:   if (data == null) return;
来源：http://lgz.andypj.xyz

================================================================================
来源：http://nak.yangfankeji.com

C. 函数与作用域
来源：http://jbb.guowangkeji.top

================================================================================
来源：http://ulg.xinyue.icu

[C01] 定义函数
来源：http://hja.guannengcc.top

Py:   def add(a, b): return a + b
来源：http://ytr.tian-w.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uyo.jlsjyb.cn

JS:   function add(a, b) { return a + b; }
来源：http://gfz.yongpay.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vck.uphjek.com

Java: static int add(int a, int b) { return a + b; }
来源：http://ury.gaohongyu789.top

Go:   func add(a, b int) int { return a + b }
来源：http://nxe.9152youxi.cn

Ruby: def add(a, b); a + b; end
来源：http://jln.hfpthk.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kbr.shanyushiyangtech.top

[C02] 默认参数
来源：http://nnv.vehdjk.com

Py:   def greet(name="World"): return name
来源：http://oob.kuanghao11.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://aql.yueranfly.top

JS:   function greet(name = "World") { return name; }
来源：http://bfg.birdmap.top

TS:   function greet(name: string = "World") { return name; }
来源：http://wov.daxiang520.top

Java: // 无默认参数：方法重载或 Optional
来源：http://bxv.chenjidiqi.icu

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hxd.jinqigufen.top

Ruby: def greet(name = "World") = name
来源：http://wfj.yonumen.top

C#:   string Greet(string name = "World") => name;
来源：http://byh.yuanzhike.top

[C03] 可变参数
来源：http://ihp.316326.xyz

Py:   def total(*args): return sum(args)
来源：http://nqj.pycfn.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lad.jinghuilouyu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mws.cucudq.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hrt.ywan-chungtsiang.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jgh.yj20258888.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blp.bjfxy.top

Ruby: def total(*nums); nums.sum; end
来源：http://buh.ydjk.org.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://det.havefunace.top

[C04] 命名参数 / 关键字参数
来源：http://swn.zycfv.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jte.sysykeji.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bjl.vehdjk.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mos.yj20258.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cuq.tianlin.xyz

Java: // 无：用 Builder 模式或 record
来源：http://gsd.iojbl.cn

Go:   // 无：用配置结构体参数
来源：http://qes.tanke756.top

Ruby: f(a: 1, b: 2)
来源：http://nok.sufxvd.cn

C#:   f(a: 1, b: 2)
来源：http://bai.guannengcc.top

[C05] 返回多个值
来源：http://swe.chenlongwang.top

Py:   return a, b
来源：http://mqx.zhoulong.xyz

PHP:  return [$a, $b];
来源：http://xhd.yj202588.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ehz.nanxinkj.top

TS:   return { a, b };
来源：http://iok.birdmap.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ykl.tanke756.top

Go:   return a, b
来源：http://ivn.nwbrower.top

Ruby: return a, b
来源：http://tgi.chenzaomai.com

C#:   return (a, b);              // ValueTuple
来源：http://lri.fanxiaobao.xyz

[C06] 匿名函数 / lambda
来源：http://ckp.ywan-chungtsiang.top

Py:   square = lambda x: x * x
来源：http://soe.gaohongyu789.top

PHP:  $square = fn($x) => $x * $x;
来源：http://igv.birdmap.top

JS:   const square = x => x * x;
来源：http://hoe.zhixingplan.top

TS:   const square = (x: number): number => x * x;
来源：http://ulw.hnqzz.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vsq.epnwcf.com

Go:   sq := func(x int) int { return x * x }
来源：http://ond.fktsv.cn

Ruby: square = ->(x) { x * x }
来源：http://ygo.jqgfzy.top

C#:   Func<int, int> square = x => x * x;
来源：http://qly.9152youxi.cn

[C07] 把函数作为参数传入
来源：http://sdt.birdmap.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cay.jinqigufen.top

PHP:  array_map("strtoupper", $arr);
来源：http://lhl.aibaodan.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wnb.gaohongyu789.top

TS:   arr.map(String)
来源：http://qye.pycfn.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yfu.hcnkem.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ose.zhijiandao.cn

Ruby: arr.map(&:upcase)
来源：http://lei.316326.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://msz.xylfe.cn

[C08] 闭包
来源：http://gxc.316326.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cgl.xingfuxueyuan.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nvs.zhiwuduotai.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fim.jqgufenzy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zjp.jinyuanbaomall.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://anl.jinqigufen.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gtb.nwbrower.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gox.hongshengwenyu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zto.sufxvd.cn

[C09] 递归
来源：http://yqh.9152youxi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cyz.fzhhl.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qgs.fanxiaobao.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qfe.c1oappe.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://spw.haohaochexian.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nmm.cdnleiting.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jmq.hnxiangtu.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tmk.vehdjk.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vqp.shanyushiyangkeji.top

[C10] 变量作用域
来源：http://lcw.guannengcc.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pxv.dianchejie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hkn.yangfankeji.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qql.daria6918.cn

TS:   同 JS
来源：http://xum.yongpay.top

Java: 方法内为块级作用域
来源：http://rww.ybcxt.top

Go:   花括号块级作用域
来源：http://srk.zdqjudy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://esc.shanyushiyangtech.top

C#:   块级作用域
来源：http://tpf.yongpay.top

[C11] 模块导入与导出
来源：http://jwg.jianghu66.top

Py:   from module import func
来源：http://wsk.sjlbkw.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://jyl.yvedp.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://iqv.smart0.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://osv.dianchejie.cn

Java: import java.util.List;
来源：http://ccr.xinyue.icu

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dko.ivvv.top

Ruby: require "json"; require_relative "./util"
来源：http://oie.gaohongyu789.top

C#:   using System.Text;
来源：http://vdj.yvedp.cn

[C12] 立即执行函数 IIFE
来源：http://qut.hnxiangtu.top

Py:   (lambda: print("run"))()
来源：http://uyz.hnxiangtu.top

PHP:  (function () { echo "run"; })();
来源：http://kni.yangfankeji.com

JS:   (() => { console.log("run"); })();
来源：http://ggo.wangdashe.top

TS:   (() => { console.log("run"); })();
来源：http://qsl.hesvh.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wmf.zhaomingkeji.xyz

Go:   func() { fmt.Println("run") }()
来源：http://zkq.ydjk.org.cn

Ruby: -> { puts "run" }.call
来源：http://mst.ppjwa.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zff.iojbl.cn

[C13] 类型声明 / 类型注解
来源：http://fsf.xuetiantiany.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mxw.xuanzx.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eds.vehdjk.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tzc.ydzc1.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nhx.yangfankeji.com

Java: int add(int a, int b) { return a + b; }
来源：http://xbx.xuanzx.com

Go:   func add(a, b int) int
来源：http://gxg.vehdjk.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mtj.hysaishi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://pla.ybcxt.top

[C14] 泛型函数
来源：http://fbs.zhengqikj.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dlj.jinyuanbaomall.cn

PHP:  // 无泛型
来源：http://dhj.mhx1999.top

JS:   // 无泛型
来源：http://zbs.jqgfzy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zsn.c1oappe.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qoz.cucudq.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jrx.ctjpmb.com

Ruby: # 无泛型
来源：http://poq.cashguo.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nfz.tian-w.cn

[C15] 解构 / 展开参数
来源：http://wsg.aizwys.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cwq.uphjek.com

PHP:  [$a, $b] = $pair;
来源：http://tfs.gogol.net.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cin.zdbjq.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ysl.jqgufenzy.top

Java: // 无解构
来源：http://nbo.tanke756.top

Go:   // 无解构
来源：http://ows.zhixingplan.top

Ruby: a, b = pair
来源：http://hug.havefunace.top

C#:   var (a, b) = pair;
来源：http://fou.mhx1999.top

[C16] 函数 / 方法重载
来源：http://gow.yj202588.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mot.mhx1999.top

PHP:  // 无重载
来源：http://msu.shzxlz.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://urb.dashuyun.cn

TS:   // 用联合类型或重载签名声明
来源：http://byh.fengsongda.top

Java: void f(int a) {}  void f(String a) {}
来源：http://nkr.xinyue.icu

Go:   // 无重载：用不同函数名
来源：http://qur.0kj1m.cn

Ruby: # 无重载：靠动态参数
来源：http://kws.aizwys.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://wcm.shanyushiyangkeji.top

================================================================================
来源：http://acq.smart0.xyz

D. 数组 / 列表 / 集合
来源：http://bss.shangyingyoupin.top

================================================================================
来源：http://jmo.tianlin.xyz

[D01] 创建数组 / 列表
来源：http://ett.daria6918.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://lri.yongpay.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hzn.cucudq.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pty.svipenyu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://utm.xingfuxueyuan.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://uqk.snrcjt.cn

Go:   arr := []int{1, 2, 3}
来源：http://qrv.nanxinkj.top

Ruby: arr = [1, 2, 3]
来源：http://pbl.fengsongda.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://djf.aizwys.cn

[D02] 追加元素到末尾
来源：http://jbv.hcnkem.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vmz.smart0.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kls.fanxiaobao.xyz

JS:   arr.push(4);
来源：http://txh.zhiwuduotai.top

TS:   arr.push(4);
来源：http://jkn.quarkkingdee.top

Java: list.add(4);
来源：http://yuy.cheryme.top

Go:   arr = append(arr, 4)
来源：http://zex.shangyingyoupin.top

Ruby: arr << 4; arr.push(5)
来源：http://mdg.cheryme.top

C#:   list.Add(4);
来源：http://avt.sweek.top

[D03] 在指定位置插入元素
来源：http://eki.iojbl.cn

Py:   arr.insert(0, 0)
来源：http://bur.hnxiangtu.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zzz.nanxuanxn.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://beb.nanxinkj.top

TS:   arr.splice(0, 0, 0);
来源：http://hhc.hfpthk.cn

Java: list.add(0, 0);
来源：http://tlu.xinyue.icu

Go:   arr = append([]int{0}, arr...)
来源：http://bvz.yangfankeji.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mgn.zhaomingkeji.xyz

C#:   list.Insert(0, 0);
来源：http://ktr.fanxiaobao.xyz

[D04] 删除元素
来源：http://cmd.aibaodan.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lqq.jqgfzy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xgq.jinghuilouyu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ibl.wangdashe.top

TS:   arr.splice(0, 1);
来源：http://sme.jyoumei.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mxx.yj202588.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://oxk.shzxlz.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://oxr.jinqigfzy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ohd.iojbl.cn

[D05] 访问与修改元素
来源：http://idf.guowangkeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://axq.svipenyu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hst.svipenyu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ccj.yangfankeji.com

TS:   arr[0]; arr.at(-1);
来源：http://iec.yj20258888.top

Java: list.get(0); list.set(0, 9);
来源：http://arm.yonumen.top

Go:   arr[0]; arr[0] = 9
来源：http://nyp.ydzc1.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ccr.yonumen.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hyu.sxryk.cn

[D06] 数组长度
来源：http://kxd.redwolf501.top

Py:   len(arr)
来源：http://gwy.guannengcc.top

PHP:  count($arr);
来源：http://hox.yueranfly.top

JS:   arr.length
来源：http://tsv.yfazqb.com

TS:   arr.length
来源：http://zsd.yuxming.cn

Java: list.size();
来源：http://vfq.cdnleiting.top

Go:   len(arr)
来源：http://crj.zhiwuduotai.top

Ruby: arr.length; arr.size
来源：http://cba.gzhubu.top

C#:   list.Count;
来源：http://txo.cashguo.top

[D07] 切片 / 取子数组
来源：http://hhk.chenjidiqi.icu

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gsy.yueranfly.top

PHP:  array_slice($arr, 1, 3);
来源：http://cog.hcnkem.com

JS:   arr.slice(1, 4);
来源：http://jrp.dashuyun.cn

TS:   arr.slice(1, 4);
来源：http://jco.gzhubu.top

Java: list.subList(1, 4);
来源：http://rsb.chenlongwang.top

Go:   arr[1:4]
来源：http://ofl.dashuyun.cn

Ruby: arr[1, 3]
来源：http://uca.shangyingyoupin.top

C#:   list.GetRange(1, 3);
来源：http://kud.fktsv.cn

[D08] 合并两个数组
来源：http://bju.nwbrower.top

Py:   a + b;  a.extend(b)
来源：http://cod.sjlbkw.cn

PHP:  array_merge($a, $b);
来源：http://opb.gotoacloud.top


<!-- 参考信息 -->
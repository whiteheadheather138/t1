代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cqp.zhijiandao.cn

Ruby: while i < 10; i += 1; end
来源：http://ytc.zhijiandao.cn

C#:   while (i < 10) { i++; }
来源：http://lpd.fehbvm.com

[B08] do-while（至少执行一次）
来源：http://aph.jqgufenzy.top

Py:   # 无 do-while：用 while True + break
来源：http://hyd.bbcook.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://wps.52xcode.cn

JS:   do { i++; } while (i < 10);
来源：http://zjx.yuanzhike.top

TS:   do { i++; } while (i < 10);
来源：http://jsn.yj20258888.top

Java: do { i++; } while (i < 10);
来源：http://xgj.hammf.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://tdd.bjfxy.top

Ruby: begin; i += 1; end while i < 10
来源：http://dtp.9152youxi.cn

C#:   do { i++; } while (i < 10);
来源：http://rds.jinqigufen.top

[B09] break 与 continue
来源：http://abe.xziqi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mch.epnwcf.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wgs.cqqwz.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sxs.fanxiaobao.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ate.xylfe.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uop.yongpay.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tba.zdqjudy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dip.gaohongyu789.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://few.cucudq.cn

[B10] 遍历同时拿索引
来源：http://uxa.xuetiantiany.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gss.svipenyu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gkc.gogol.net.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://oeh.zdqjudy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hnh.jinyuanbaomall.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://znq.sweek.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zbl.jinyuanbaomall.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://atc.wangdashe.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ixa.quarkkingdee.top

[B11] 生成数字序列 / 区间
来源：http://kge.meibo888.top

Py:   list(range(0, 10, 2))
来源：http://xho.zdbjq.cn

PHP:  range(0, 10, 2);
来源：http://omz.c1oappe.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mgh.yonumen.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://age.daria6918.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lhr.316326.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://avd.ydzc1.top

Ruby: (0...10).step(2).to_a
来源：http://rtj.sweek.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rrt.gogol.net.cn

[B12] 跳出多层循环
来源：http://ylb.9152youxi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://qth.dashuyun.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://dbj.pengpengdd.cyou

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rnv.xingfuxueyuan.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wtu.sxryk.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tba.zhoulong.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xgw.yvedp.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ynm.yvedp.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sul.fktsv.cn

[B13] 判断是否为数字
来源：http://oix.fengsongda.top

Py:   isinstance(x, (int, float))
来源：http://oyo.zhengqikj.top

PHP:  is_numeric($x)
来源：http://evq.yuxming.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xuf.jinghuilouyu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cob.xuanzx.com

Java: x instanceof Number
来源：http://wsi.jinqigfzy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ydt.sweek.top

Ruby: x.is_a?(Numeric)
来源：http://ktm.uphjek.com

C#:   x is int or double or decimal
来源：http://wqk.cdnleiting.top

[B14] 判断值是否在集合内
来源：http://igp.zdbjq.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wos.ctjpmb.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jzf.yonumen.top

JS:   [1, 2, 3].includes(x)
来源：http://awx.yangfankeji.com

TS:   [1, 2, 3].includes(x)
来源：http://uko.sxryk.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://woz.tian-w.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tts.jinyuanbaomall.cn

Ruby: [1, 2, 3].include?(x)
来源：http://cbi.xylfe.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mgb.birdmap.top

[B15] 布尔运算与取反
来源：http://xyk.hywenlv.cn

Py:   a and b or not c
来源：http://rgi.fzhhl.top

PHP:  $a && $b || !$c
来源：http://xho.cqqwz.cn

JS:   a && b || !c
来源：http://ail.ehwqpu.com

TS:   a && b || !c
来源：http://wvg.zhixingplan.top

Java: a && b || !c
来源：http://kkj.daxiang520.top

Go:   a && b || !c
来源：http://ncd.hnxiangtu.top

Ruby: a && b || !c
来源：http://kki.gaohongyu789.top

C#:   a && b || !c
来源：http://efm.ybcxt.top

[B16] 卫语句：不满足条件提前返回
来源：http://dxn.cucudq.cn

Py:   if not data: return
来源：http://cqo.fzhhl.top

PHP:  if (!$data) { return; }
来源：http://bvu.xuanzx.com

JS:   if (!data) return;
来源：http://xob.hfpthk.cn

TS:   if (!data) return;
来源：http://vah.aibaodan.cn

Java: if (data == null) return;
来源：http://rac.ctjpmb.com

Go:   if data == nil { return }
来源：http://vfi.yuxming.cn

Ruby: return if data.nil?
来源：http://fth.epnwcf.com

C#:   if (data == null) return;
来源：http://iin.ctjpmb.com

================================================================================
来源：http://lbz.iojbl.cn

C. 函数与作用域
来源：http://axt.yj20258.top

================================================================================
来源：http://ppv.ybcxt.top

[C01] 定义函数
来源：http://pjz.svipenyu.cn

Py:   def add(a, b): return a + b
来源：http://usz.ywan-chungtsiang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gtj.nanxinkj.top

JS:   function add(a, b) { return a + b; }
来源：http://sis.chenzaomai.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pej.yfazqb.com

Java: static int add(int a, int b) { return a + b; }
来源：http://wfj.zhiwuduotai.top

Go:   func add(a, b int) int { return a + b }
来源：http://vtd.ywan-chungtsiang.top

Ruby: def add(a, b); a + b; end
来源：http://omc.ehwqpu.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://unz.dianchejie.cn

[C02] 默认参数
来源：http://iyq.fzhhl.top

Py:   def greet(name="World"): return name
来源：http://nvq.hysaishi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://kbn.yvedp.cn

JS:   function greet(name = "World") { return name; }
来源：http://wlg.jqgfzy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://bsj.bjfxy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://znt.nwbrower.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nus.chenlongwang.top

Ruby: def greet(name = "World") = name
来源：http://owg.svipenyu.cn

C#:   string Greet(string name = "World") => name;
来源：http://meg.fktsv.cn

[C03] 可变参数
来源：http://shc.xziqi.cn

Py:   def total(*args): return sum(args)
来源：http://qdk.xuanzx.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://opc.zhaomingkeji.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xqq.fktsv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fgl.zycfv.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ndp.cheryme.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nst.birdmap.top

Ruby: def total(*nums); nums.sum; end
来源：http://ewd.nwbrower.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://aye.yongpay.top

[C04] 命名参数 / 关键字参数
来源：http://lyq.ctjpmb.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rbf.vehdjk.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://msh.yuanzhike.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ody.xylfe.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://duz.epnwcf.com

Java: // 无：用 Builder 模式或 record
来源：http://jdn.jinyuanbaomall.cn

Go:   // 无：用配置结构体参数
来源：http://jsa.smart0.xyz

Ruby: f(a: 1, b: 2)
来源：http://dzf.daria6918.cn

C#:   f(a: 1, b: 2)
来源：http://whl.ppjwa.cn

[C05] 返回多个值
来源：http://dqt.jinghuilouyu.cn

Py:   return a, b
来源：http://hbb.nwbrower.top

PHP:  return [$a, $b];
来源：http://ysz.yueranfly.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://xyx.fehbvm.com

TS:   return { a, b };
来源：http://cwl.yanxiufei.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xvn.mhx1999.top

Go:   return a, b
来源：http://dyy.yuanzhike.top

Ruby: return a, b
来源：http://omp.sweek.top

C#:   return (a, b);              // ValueTuple
来源：http://ops.cashguo.top

[C06] 匿名函数 / lambda
来源：http://fud.zhoulong.xyz

Py:   square = lambda x: x * x
来源：http://zom.yangfankeji.com

PHP:  $square = fn($x) => $x * $x;
来源：http://nbd.hnqzz.top

JS:   const square = x => x * x;
来源：http://kxa.guannengcc.top

TS:   const square = (x: number): number => x * x;
来源：http://fqv.cdnleiting.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tmm.c1oappe.top

Go:   sq := func(x int) int { return x * x }
来源：http://zcw.feifeiyinyue.top

Ruby: square = ->(x) { x * x }
来源：http://sot.316326.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://uhg.hywenlv.cn

[C07] 把函数作为参数传入
来源：http://lda.jlsjyb.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bzo.sxryk.cn

PHP:  array_map("strtoupper", $arr);
来源：http://him.hammf.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gcx.zdqjudy.top

TS:   arr.map(String)
来源：http://sou.9152youxi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mxd.snrcjt.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sgs.chenjidiqi.icu

Ruby: arr.map(&:upcase)
来源：http://dff.zhengqikj.top

C#:   arr.Select(s => s.ToUpper())
来源：http://wzc.tarul.cn

[C08] 闭包
来源：http://typ.zhongyouzk.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ylu.zdqjudy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vra.chenlongwang.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://soo.xziqi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ayz.zhengqikj.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nmg.tianlin.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dhu.yfazqb.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qkz.xingfuxueyuan.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ugu.hywenlv.cn

[C09] 递归
来源：http://qfm.sweek.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ddv.sufxvd.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ipj.ivvv.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eet.vehdjk.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vav.jqgfzy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bua.sweek.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hac.chenzaomai.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lla.9152youxi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fcd.hywenlv.cn

[C10] 变量作用域
来源：http://keh.ivvv.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cod.jinyuanbaomall.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ogh.pycfn.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ouo.shanyushiyangkeji.top

TS:   同 JS
来源：http://vev.9152youxi.cn

Java: 方法内为块级作用域
来源：http://zba.yj20258.top

Go:   花括号块级作用域
来源：http://cco.hnxiangtu.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rok.vqdsnc.cn

C#:   块级作用域
来源：http://qvl.xingfuxueyuan.xyz

[C11] 模块导入与导出
来源：http://ctf.nwbrower.top

Py:   from module import func
来源：http://cop.ybcxt.top

PHP:  require "file.php";  或 use App\Service;
来源：http://qev.zhongyouzk.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://rcp.zhongyouzk.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xct.sysykeji.top

Java: import java.util.List;
来源：http://ack.tanke756.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uzu.hammf.cn

Ruby: require "json"; require_relative "./util"
来源：http://ind.jlsjyb.cn

C#:   using System.Text;
来源：http://rwp.wangshuangyany.cn

[C12] 立即执行函数 IIFE
来源：http://pcg.ctjpmb.com

Py:   (lambda: print("run"))()
来源：http://xpm.jianghu66.top

PHP:  (function () { echo "run"; })();
来源：http://eao.bbcook.cn

JS:   (() => { console.log("run"); })();
来源：http://vsm.hfpthk.cn

TS:   (() => { console.log("run"); })();
来源：http://dgu.zdqjudy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://eia.jyoumei.cn

Go:   func() { fmt.Println("run") }()
来源：http://zrb.gotoacloud.top

Ruby: -> { puts "run" }.call
来源：http://gmb.nwbrower.top

C#:   // 无 IIFE：用静态构造函数
来源：http://mfx.nanxinkj.top

[C13] 类型声明 / 类型注解
来源：http://oyu.ywan-chungtsiang.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sgk.snrcjt.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rkf.guannengcc.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wwn.snrcjt.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://eup.gotoacloud.top

Java: int add(int a, int b) { return a + b; }
来源：http://qeb.redwolf501.top

Go:   func add(a, b int) int
来源：http://wxy.tian-w.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wbt.xinyue.icu

C#:   int Add(int a, int b) => a + b;
来源：http://nsi.hongshengwenyu.top

[C14] 泛型函数
来源：http://lmr.pengpengdd.cyou

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://krt.guowangkeji.top

PHP:  // 无泛型
来源：http://dot.ydjk.org.cn

JS:   // 无泛型
来源：http://cmt.yj20258.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ujr.zhongyouzk.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ady.quarkkingdee.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mfa.hammf.cn

Ruby: # 无泛型
来源：http://qei.zycfv.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://plu.vehdjk.com

[C15] 解构 / 展开参数
来源：http://gng.sufxvd.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lmm.cashguo.top

PHP:  [$a, $b] = $pair;
来源：http://ixc.chenlongwang.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vti.yongpay.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://usc.zhengqikj.top

Java: // 无解构
来源：http://ggf.bbcook.cn

Go:   // 无解构
来源：http://way.yvedp.cn

Ruby: a, b = pair
来源：http://ajs.zhaomingkeji.xyz

C#:   var (a, b) = pair;
来源：http://koe.zhengqikj.top

[C16] 函数 / 方法重载
来源：http://wyz.hnqzz.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dgn.ivvv.top

PHP:  // 无重载
来源：http://yhc.jqgufenzy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://coz.gogol.net.cn

TS:   // 用联合类型或重载签名声明
来源：http://ong.hywenlv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://mii.yj20258888.top

Go:   // 无重载：用不同函数名
来源：http://uty.tanke756.top

Ruby: # 无重载：靠动态参数
来源：http://jnz.daria6918.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://jol.aibaodan.cn

================================================================================
来源：http://yry.yj202588.top

D. 数组 / 列表 / 集合
来源：http://hdi.kuanghao11.cn

================================================================================
来源：http://wtq.ctjpmb.com

[D01] 创建数组 / 列表
来源：http://gvv.fzhhl.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://zse.shanyushiyangkeji.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qja.xylfe.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://olv.shzxlz.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kml.hongshengwenyu.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yqk.zhixingplan.top

Go:   arr := []int{1, 2, 3}
来源：http://emo.feifeiyinyue.top

Ruby: arr = [1, 2, 3]
来源：http://syu.aizwys.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gps.shanyushiyangkeji.top

[D02] 追加元素到末尾
来源：http://kaq.hammf.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nht.xylfe.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://abk.nanxinkj.top

JS:   arr.push(4);
来源：http://alm.xinyue.icu

TS:   arr.push(4);
来源：http://cav.jqgufenzy.top

Java: list.add(4);
来源：http://vmr.zhixingplan.top

Go:   arr = append(arr, 4)
来源：http://cpk.sxryk.cn

Ruby: arr << 4; arr.push(5)
来源：http://int.cheryme.top

C#:   list.Add(4);
来源：http://kvr.xuetiantiany.cn

[D03] 在指定位置插入元素
来源：http://tji.zhengqikj.top

Py:   arr.insert(0, 0)
来源：http://vnj.ppjwa.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://npv.zhoulong.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pbj.gaohongyu789.top

TS:   arr.splice(0, 0, 0);
来源：http://loj.shzxlz.cn

Java: list.add(0, 0);
来源：http://okt.nanxinkj.top

Go:   arr = append([]int{0}, arr...)
来源：http://dli.jqgufenzy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fyq.quarkkingdee.top

C#:   list.Insert(0, 0);
来源：http://rdp.jiagoushi.top

[D04] 删除元素
来源：http://pls.tianlin.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sao.zhixingplan.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jwn.fehbvm.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wkp.xylfe.cn

TS:   arr.splice(0, 1);
来源：http://mpc.gaohongyu789.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://eyy.snrcjt.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pti.sjlbkw.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tvc.xuanzx.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vap.vqdsnc.cn

[D05] 访问与修改元素
来源：http://hen.yj202588.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jrv.sufxvd.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mvu.yanxiufei.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wet.havefunace.top

TS:   arr[0]; arr.at(-1);
来源：http://pmj.hesvh.cn

Java: list.get(0); list.set(0, 9);
来源：http://kbv.fanxiaobao.xyz

Go:   arr[0]; arr[0] = 9
来源：http://giq.yj202588.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zte.dianchejie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://brk.shangyingyoupin.top

[D06] 数组长度
来源：http://bzr.xuetiantiany.cn

Py:   len(arr)
来源：http://kkk.hysaishi.cn

PHP:  count($arr);
来源：http://faj.gogol.net.cn

JS:   arr.length
来源：http://xqu.c1oappe.top

TS:   arr.length
来源：http://nfw.havefunace.top

Java: list.size();
来源：http://bcm.hnqzz.top

Go:   len(arr)
来源：http://cps.zhijiandao.cn

Ruby: arr.length; arr.size
来源：http://yyi.cheryme.top

C#:   list.Count;
来源：http://bmn.zhijiandao.cn

[D07] 切片 / 取子数组
来源：http://fkb.wangshuangyany.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://huc.yfazqb.com

PHP:  array_slice($arr, 1, 3);
来源：http://vpv.jqgfzy.top

JS:   arr.slice(1, 4);
来源：http://mfy.316326.xyz

TS:   arr.slice(1, 4);
来源：http://ocd.ywan-chungtsiang.top

Java: list.subList(1, 4);
来源：http://zyb.haohaochexian.top

Go:   arr[1:4]
来源：http://yqq.yuxming.cn

Ruby: arr[1, 3]
来源：http://jor.fktsv.cn

C#:   list.GetRange(1, 3);
来源：http://eqc.yangfankeji.com

[D08] 合并两个数组
来源：http://sjs.hammf.cn

Py:   a + b;  a.extend(b)
来源：http://uxl.shzxlz.cn

PHP:  array_merge($a, $b);
来源：http://loa.ppjwa.cn


<!-- 参考信息 -->
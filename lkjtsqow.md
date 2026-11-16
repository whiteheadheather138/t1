代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://yto.0kj1m.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://aeb.tian-w.cn

JS:   do { i++; } while (i < 10);
来源：http://iee.ydjk.org.cn

TS:   do { i++; } while (i < 10);
来源：http://ceu.chenzaomai.com

Java: do { i++; } while (i < 10);
来源：http://imt.shzxlz.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jyj.sufxvd.cn

Ruby: begin; i += 1; end while i < 10
来源：http://uck.haohaochexian.top

C#:   do { i++; } while (i < 10);
来源：http://evt.jiagoushi.top

[B09] break 与 continue
来源：http://utn.xingfuxueyuan.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://czq.chenzaomai.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://iud.shzxlz.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ymb.bjfxy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fpy.gzhubu.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cfa.hcnkem.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dpj.ehwqpu.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hmg.shangyingyoupin.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fkn.hesvh.cn

[B10] 遍历同时拿索引
来源：http://nwm.hnxiangtu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mlu.316326.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gmp.chenzaomai.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jkq.fktsv.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://akr.shangyingyoupin.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lgq.cashguo.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bem.dashuyun.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://boe.ybcxt.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jsk.cucudq.cn

[B11] 生成数字序列 / 区间
来源：http://bll.xuanzx.com

Py:   list(range(0, 10, 2))
来源：http://jax.yj20258888.top

PHP:  range(0, 10, 2);
来源：http://uih.sxryk.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gyz.xziqi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://idp.sysykeji.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://amv.fanxiaobao.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ybp.smart0.xyz

Ruby: (0...10).step(2).to_a
来源：http://htg.zdbjq.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vzu.fengsongda.top

[B12] 跳出多层循环
来源：http://lig.jinqigufen.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://qqa.gaohongyu789.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://pjx.aibaodan.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://huc.xinyue.icu

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kou.sjlbkw.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fmp.daria6918.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xbo.zycfv.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://eoi.gaohongyu789.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qaa.zdbjq.cn

[B13] 判断是否为数字
来源：http://edw.9152youxi.cn

Py:   isinstance(x, (int, float))
来源：http://ftb.vehdjk.com

PHP:  is_numeric($x)
来源：http://ipk.pycfn.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://trh.guannengcc.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cdn.iojbl.cn

Java: x instanceof Number
来源：http://ecq.shangyingyoupin.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://joa.gogol.net.cn

Ruby: x.is_a?(Numeric)
来源：http://ppg.yueranfly.top

C#:   x is int or double or decimal
来源：http://ann.yuxming.cn

[B14] 判断值是否在集合内
来源：http://sgz.svipenyu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://maa.wangdashe.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ert.zdqjudy.top

JS:   [1, 2, 3].includes(x)
来源：http://wzm.jlsjyb.cn

TS:   [1, 2, 3].includes(x)
来源：http://dlu.cqqwz.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xky.yuanzhike.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://den.yfazqb.com

Ruby: [1, 2, 3].include?(x)
来源：http://duw.epnwcf.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bgb.nanxinkj.top

[B15] 布尔运算与取反
来源：http://eng.hysaishi.cn

Py:   a and b or not c
来源：http://xvg.pycfn.com

PHP:  $a && $b || !$c
来源：http://tgi.snrcjt.cn

JS:   a && b || !c
来源：http://rgl.sjlbkw.cn

TS:   a && b || !c
来源：http://hvx.zycfv.cn

Java: a && b || !c
来源：http://kkb.cheryme.top

Go:   a && b || !c
来源：http://oel.hongshengwenyu.top

Ruby: a && b || !c
来源：http://nop.chenjidiqi.icu

C#:   a && b || !c
来源：http://stq.zdqjudy.top

[B16] 卫语句：不满足条件提前返回
来源：http://mow.316326.xyz

Py:   if not data: return
来源：http://ayp.kuanghao11.cn

PHP:  if (!$data) { return; }
来源：http://cjg.jinqigfzy.top

JS:   if (!data) return;
来源：http://cbw.sxryk.cn

TS:   if (!data) return;
来源：http://sto.bbcook.cn

Java: if (data == null) return;
来源：http://fyq.gzhubu.top

Go:   if data == nil { return }
来源：http://rju.redwolf501.top

Ruby: return if data.nil?
来源：http://ecz.jinqigfzy.top

C#:   if (data == null) return;
来源：http://ysf.tarul.cn

================================================================================
来源：http://obm.hesvh.cn

C. 函数与作用域
来源：http://loz.wangshuangyany.cn

================================================================================
来源：http://iql.tianlin.xyz

[C01] 定义函数
来源：http://wsm.fehbvm.com

Py:   def add(a, b): return a + b
来源：http://xug.316326.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rje.guowangkeji.top

JS:   function add(a, b) { return a + b; }
来源：http://pqb.ppjwa.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kjn.uphjek.com

Java: static int add(int a, int b) { return a + b; }
来源：http://mbi.zhiwuduotai.top

Go:   func add(a, b int) int { return a + b }
来源：http://dld.bjfxy.top

Ruby: def add(a, b); a + b; end
来源：http://oks.daxiang520.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ocs.xuetiantiany.cn

[C02] 默认参数
来源：http://ymm.gotoacloud.top

Py:   def greet(name="World"): return name
来源：http://gow.fktsv.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lag.yj20258.top

JS:   function greet(name = "World") { return name; }
来源：http://tep.0kj1m.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fqj.jyoumei.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rdc.bjfxy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kpm.yonumen.top

Ruby: def greet(name = "World") = name
来源：http://hkc.zhixingplan.top

C#:   string Greet(string name = "World") => name;
来源：http://lav.jqgfzy.top

[C03] 可变参数
来源：http://mrd.xuanzx.com

Py:   def total(*args): return sum(args)
来源：http://jrk.vehdjk.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://unz.sweek.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kny.snrcjt.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tez.yj202588.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sil.guowangkeji.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bqk.aibaodan.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wil.xuetiantiany.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jqh.316326.xyz

[C04] 命名参数 / 关键字参数
来源：http://amt.sweek.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gay.guannengcc.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lmf.tanke756.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xbi.mhx1999.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qys.yj20258888.top

Java: // 无：用 Builder 模式或 record
来源：http://ehs.yongpay.top

Go:   // 无：用配置结构体参数
来源：http://omd.tian-w.cn

Ruby: f(a: 1, b: 2)
来源：http://jgz.tarul.cn

C#:   f(a: 1, b: 2)
来源：http://emr.yonumen.top

[C05] 返回多个值
来源：http://oiu.xingfuxueyuan.xyz

Py:   return a, b
来源：http://lyi.cqqwz.cn

PHP:  return [$a, $b];
来源：http://sdm.gotoacloud.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://mdk.hongshengwenyu.top

TS:   return { a, b };
来源：http://thb.aizwys.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bqr.hnxiangtu.top

Go:   return a, b
来源：http://eeo.hfpthk.cn

Ruby: return a, b
来源：http://inv.guowangkeji.top

C#:   return (a, b);              // ValueTuple
来源：http://ebh.316326.xyz

[C06] 匿名函数 / lambda
来源：http://yih.hongshengwenyu.top

Py:   square = lambda x: x * x
来源：http://aqg.52xcode.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://nwa.gzhubu.top

JS:   const square = x => x * x;
来源：http://hgq.jinqigfzy.top

TS:   const square = (x: number): number => x * x;
来源：http://ohj.zhijiandao.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fgl.dashuyun.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rzj.pengpengdd.cyou

Ruby: square = ->(x) { x * x }
来源：http://gui.aizwys.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fmg.zhoulong.xyz

[C07] 把函数作为参数传入
来源：http://dgk.nwbrower.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xps.fehbvm.com

PHP:  array_map("strtoupper", $arr);
来源：http://nxu.yuanzhike.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://aht.jlsjyb.cn

TS:   arr.map(String)
来源：http://gbi.guowangkeji.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ftg.kuanghao11.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kdq.guowangkeji.top

Ruby: arr.map(&:upcase)
来源：http://gll.ppjwa.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://rbw.cucudq.cn

[C08] 闭包
来源：http://qtl.yanxiufei.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vzr.jinqigfzy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cvn.xylfe.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nmr.52xcode.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fav.meibo888.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dfx.mhx1999.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hrf.cheryme.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ewh.yonumen.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zuh.sysykeji.top

[C09] 递归
来源：http://mvo.svipenyu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nik.cqqwz.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gpe.hongshengwenyu.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zvq.hcnkem.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rov.kuanghao11.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vrm.sysykeji.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gzq.svipenyu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ixb.ydzc1.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ggl.birdmap.top

[C10] 变量作用域
来源：http://qeu.sufxvd.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kcs.yueranfly.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xcb.chenzaomai.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cmk.vqdsnc.cn

TS:   同 JS
来源：http://hdq.hfpthk.cn

Java: 方法内为块级作用域
来源：http://zkd.shuidangran.top

Go:   花括号块级作用域
来源：http://ono.yongpay.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://stn.bbcook.cn

C#:   块级作用域
来源：http://jev.jinyuanbaomall.cn

[C11] 模块导入与导出
来源：http://vfa.cucudq.cn

Py:   from module import func
来源：http://ilh.quarkkingdee.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ksv.xinyue.icu

JS:   export default function f() {};  import f from "./m.js";
来源：http://don.ehwqpu.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sfz.fanxiaobao.xyz

Java: import java.util.List;
来源：http://mwk.jlsjyb.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kmv.xylfe.cn

Ruby: require "json"; require_relative "./util"
来源：http://guk.epnwcf.com

C#:   using System.Text;
来源：http://epk.sysykeji.top

[C12] 立即执行函数 IIFE
来源：http://dbw.pengpengdd.cyou

Py:   (lambda: print("run"))()
来源：http://rqw.sjlbkw.cn

PHP:  (function () { echo "run"; })();
来源：http://waz.haohaochexian.top

JS:   (() => { console.log("run"); })();
来源：http://ujp.xinyue.icu

TS:   (() => { console.log("run"); })();
来源：http://iwr.jqgfzy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ymc.fengsongda.top

Go:   func() { fmt.Println("run") }()
来源：http://bjb.kuanghao11.cn

Ruby: -> { puts "run" }.call
来源：http://sgu.fktsv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://sns.havefunace.top

[C13] 类型声明 / 类型注解
来源：http://lxj.hesvh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://riw.hesvh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vmn.hfpthk.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://msa.jiagoushi.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ydi.cdnleiting.top

Java: int add(int a, int b) { return a + b; }
来源：http://src.pycfn.com

Go:   func add(a, b int) int
来源：http://ksi.tarul.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wjm.vehdjk.com

C#:   int Add(int a, int b) => a + b;
来源：http://nos.9152youxi.cn

[C14] 泛型函数
来源：http://rsc.birdmap.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jvu.yuxming.cn

PHP:  // 无泛型
来源：http://mdb.zhoulong.xyz

JS:   // 无泛型
来源：http://rep.jinqigfzy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://znc.daxiang520.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bvn.fzhhl.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lcn.daria6918.cn

Ruby: # 无泛型
来源：http://ufh.aizwys.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zxe.zhijiandao.cn

[C15] 解构 / 展开参数
来源：http://tfu.zhiwuduotai.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qyb.epnwcf.com

PHP:  [$a, $b] = $pair;
来源：http://rbn.sweek.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zhy.316326.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vct.fanxiaobao.xyz

Java: // 无解构
来源：http://ptr.yj20258.top

Go:   // 无解构
来源：http://chw.shanyushiyangtech.top

Ruby: a, b = pair
来源：http://cba.yongpay.top

C#:   var (a, b) = pair;
来源：http://fwu.mhx1999.top

[C16] 函数 / 方法重载
来源：http://kai.haohaochexian.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sbv.iojbl.cn

PHP:  // 无重载
来源：http://mwv.svipenyu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://cab.fktsv.cn

TS:   // 用联合类型或重载签名声明
来源：http://mgs.zhijiandao.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://cko.jianghu66.top

Go:   // 无重载：用不同函数名
来源：http://ify.bbcook.cn

Ruby: # 无重载：靠动态参数
来源：http://kfk.nanxuanxn.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://onv.nanxuanxn.top

================================================================================
来源：http://dnv.nanxinkj.top

D. 数组 / 列表 / 集合
来源：http://gnu.c1oappe.top

================================================================================
来源：http://ncb.hcnkem.com

[D01] 创建数组 / 列表
来源：http://tgb.snrcjt.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://moz.yangfankeji.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rsx.xingfuxueyuan.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sjo.dashuyun.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hjy.redwolf501.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hif.shzxlz.cn

Go:   arr := []int{1, 2, 3}
来源：http://hnd.ydzc1.top

Ruby: arr = [1, 2, 3]
来源：http://tft.wangshuangyany.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gbm.hywenlv.cn

[D02] 追加元素到末尾
来源：http://tds.jinqigfzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vrb.fanxiaobao.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jwr.hywenlv.cn

JS:   arr.push(4);
来源：http://fex.hammf.cn

TS:   arr.push(4);
来源：http://ruo.redwolf501.top

Java: list.add(4);
来源：http://ysj.jinqigufen.top

Go:   arr = append(arr, 4)
来源：http://ehm.quarkkingdee.top

Ruby: arr << 4; arr.push(5)
来源：http://bgn.tarul.cn

C#:   list.Add(4);
来源：http://zrq.zhengqikj.top

[D03] 在指定位置插入元素
来源：http://ojs.chenzaomai.com

Py:   arr.insert(0, 0)
来源：http://jmz.zdqjudy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ech.sxryk.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xaf.xingfuxueyuan.xyz

TS:   arr.splice(0, 0, 0);
来源：http://ixh.dashuyun.cn

Java: list.add(0, 0);
来源：http://qsa.aibaodan.cn

Go:   arr = append([]int{0}, arr...)
来源：http://sfy.dashuyun.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rvw.tianlin.xyz

C#:   list.Insert(0, 0);
来源：http://dol.snrcjt.cn

[D04] 删除元素
来源：http://gfa.redwolf501.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ujb.nwbrower.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nlf.cheryme.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ivh.tarul.cn

TS:   arr.splice(0, 1);
来源：http://ltc.sxryk.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://sii.smart0.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vdf.meibo888.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mzg.cqqwz.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mve.wangdashe.top

[D05] 访问与修改元素
来源：http://adw.zhaomingkeji.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gvx.gzhubu.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fah.ehwqpu.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kgx.pengpengdd.cyou

TS:   arr[0]; arr.at(-1);
来源：http://iib.kuanghao11.cn

Java: list.get(0); list.set(0, 9);
来源：http://lnp.daxiang520.top

Go:   arr[0]; arr[0] = 9
来源：http://rjl.nanxuanxn.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ksi.yanxiufei.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://flm.yangfankeji.com

[D06] 数组长度
来源：http://gpa.gotoacloud.top

Py:   len(arr)
来源：http://bve.hysaishi.cn

PHP:  count($arr);
来源：http://nhi.yanxiufei.cn

JS:   arr.length
来源：http://slv.sysykeji.top

TS:   arr.length
来源：http://hsb.bbcook.cn

Java: list.size();
来源：http://ssc.epnwcf.com

Go:   len(arr)
来源：http://jip.fanxiaobao.xyz

Ruby: arr.length; arr.size
来源：http://sbx.yonumen.top

C#:   list.Count;
来源：http://bbt.vehdjk.com

[D07] 切片 / 取子数组
来源：http://ouh.epnwcf.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vpi.9152youxi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://tlg.gotoacloud.top

JS:   arr.slice(1, 4);
来源：http://him.andypj.xyz

TS:   arr.slice(1, 4);
来源：http://xyp.yuxming.cn

Java: list.subList(1, 4);
来源：http://rqt.guowangkeji.top

Go:   arr[1:4]
来源：http://uee.yonumen.top

Ruby: arr[1, 3]
来源：http://aht.jqgufenzy.top

C#:   list.GetRange(1, 3);
来源：http://qup.sweek.top

[D08] 合并两个数组
来源：http://zyj.zhixingplan.top

Py:   a + b;  a.extend(b)
来源：http://jbh.chenlongwang.top

PHP:  array_merge($a, $b);
来源：http://qtz.dianchejie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hfs.zdbjq.cn

TS:   [...a, ...b];
来源：http://qmh.nanxuanxn.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qtv.jinyuanbaomall.cn

Go:   append(a, b...)
来源：http://ypj.daria6918.cn


<!-- 参考信息 -->
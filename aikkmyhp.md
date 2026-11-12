代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://zzg.hesvh.cn

JS:   while (i < 10) { i++; }
来源：http://fzr.316326.xyz

TS:   while (i < 10) { i++; }
来源：http://myt.yongpay.top

Java: while (i < 10) { i++; }
来源：http://qcr.meibo888.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jva.gaohongyu789.top

Ruby: while i < 10; i += 1; end
来源：http://wqk.hesvh.cn

C#:   while (i < 10) { i++; }
来源：http://idx.yfazqb.com

[B08] do-while（至少执行一次）
来源：http://pqo.hammf.cn

Py:   # 无 do-while：用 while True + break
来源：http://uul.mhx1999.top

PHP:  do { $i++; } while ($i < 10);
来源：http://pqi.dashuyun.cn

JS:   do { i++; } while (i < 10);
来源：http://cni.52xcode.cn

TS:   do { i++; } while (i < 10);
来源：http://zcj.xziqi.cn

Java: do { i++; } while (i < 10);
来源：http://big.cdnleiting.top

Go:   for { i++; if i >= 10 { break } }
来源：http://qjs.jiagoushi.top

Ruby: begin; i += 1; end while i < 10
来源：http://ejv.fzhhl.top

C#:   do { i++; } while (i < 10);
来源：http://hup.hfpthk.cn

[B09] break 与 continue
来源：http://rni.zhixingplan.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ioi.yangfankeji.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fie.zhixingplan.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kfg.shanyushiyangtech.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ghk.jinqigufen.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gqk.jiagoushi.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://iht.snrcjt.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bjw.hnqzz.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pzz.jinqigufen.top

[B10] 遍历同时拿索引
来源：http://rae.yangfankeji.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dig.yj202588.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ydw.tanke756.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://owx.aizwys.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ftu.0kj1m.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tum.nanxinkj.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cux.9152youxi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vti.feifeiyinyue.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://upc.jqgfzy.top

[B11] 生成数字序列 / 区间
来源：http://jwj.52xcode.cn

Py:   list(range(0, 10, 2))
来源：http://ocn.jlsjyb.cn

PHP:  range(0, 10, 2);
来源：http://fei.jianghu66.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zty.yj20258.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jbl.zhengqikj.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zhv.sxryk.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://atj.shanyushiyangkeji.top

Ruby: (0...10).step(2).to_a
来源：http://nki.aibaodan.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hpj.xuanzx.com

[B12] 跳出多层循环
来源：http://xsw.meibo888.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://cdb.zhoulong.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://tjq.hysaishi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ztv.zhongyouzk.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rik.xingfuxueyuan.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://oev.pengpengdd.cyou

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mgi.hesvh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ibi.sxryk.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sxi.vqdsnc.cn

[B13] 判断是否为数字
来源：http://ysl.jianghu66.top

Py:   isinstance(x, (int, float))
来源：http://ble.yuanzhike.top

PHP:  is_numeric($x)
来源：http://uzo.fzhhl.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oym.bbcook.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uff.sysykeji.top

Java: x instanceof Number
来源：http://dcu.yj20258888.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zej.iojbl.cn

Ruby: x.is_a?(Numeric)
来源：http://kkl.xziqi.cn

C#:   x is int or double or decimal
来源：http://qdj.jianghu66.top

[B14] 判断值是否在集合内
来源：http://cvx.zhixingplan.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://btr.yuanzhike.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://imy.ivvv.top

JS:   [1, 2, 3].includes(x)
来源：http://ktk.fehbvm.com

TS:   [1, 2, 3].includes(x)
来源：http://hbd.hysaishi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://zyy.xziqi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rxn.gogol.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zgw.zhijiandao.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mml.epnwcf.com

[B15] 布尔运算与取反
来源：http://pfs.hongshengwenyu.top

Py:   a and b or not c
来源：http://qrd.fktsv.cn

PHP:  $a && $b || !$c
来源：http://ecy.cucudq.cn

JS:   a && b || !c
来源：http://rvl.birdmap.top

TS:   a && b || !c
来源：http://amf.jqgufenzy.top

Java: a && b || !c
来源：http://mad.jinghuilouyu.cn

Go:   a && b || !c
来源：http://bgf.birdmap.top

Ruby: a && b || !c
来源：http://wjw.jinqigufen.top

C#:   a && b || !c
来源：http://swm.bbcook.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ndv.fzhhl.top

Py:   if not data: return
来源：http://sbk.hcnkem.com

PHP:  if (!$data) { return; }
来源：http://sdj.shzxlz.cn

JS:   if (!data) return;
来源：http://oye.zhengqikj.top

TS:   if (!data) return;
来源：http://wwa.sjlbkw.cn

Java: if (data == null) return;
来源：http://nyn.yj202588.top

Go:   if data == nil { return }
来源：http://dhw.feifeiyinyue.top

Ruby: return if data.nil?
来源：http://cds.shanyushiyangtech.top

C#:   if (data == null) return;
来源：http://lya.yvedp.cn

================================================================================
来源：http://uah.zycfv.cn

C. 函数与作用域
来源：http://fte.jinyuanbaomall.cn

================================================================================
来源：http://zku.zhoulong.xyz

[C01] 定义函数
来源：http://hgy.bjfxy.top

Py:   def add(a, b): return a + b
来源：http://usv.chenlongwang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xsk.sxryk.cn

JS:   function add(a, b) { return a + b; }
来源：http://yqy.jyoumei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ytg.guowangkeji.top

Java: static int add(int a, int b) { return a + b; }
来源：http://eoo.sjlbkw.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dox.hammf.cn

Ruby: def add(a, b); a + b; end
来源：http://apn.ydjk.org.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vch.fktsv.cn

[C02] 默认参数
来源：http://mfq.quarkkingdee.top

Py:   def greet(name="World"): return name
来源：http://dsg.yfazqb.com

PHP:  function greet($name = "World") { return $name; }
来源：http://jzw.aibaodan.cn

JS:   function greet(name = "World") { return name; }
来源：http://eaj.vehdjk.com

TS:   function greet(name: string = "World") { return name; }
来源：http://eww.feifeiyinyue.top

Java: // 无默认参数：方法重载或 Optional
来源：http://qnf.52xcode.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gxr.chenlongwang.top

Ruby: def greet(name = "World") = name
来源：http://hmr.birdmap.top

C#:   string Greet(string name = "World") => name;
来源：http://tbl.chenlongwang.top

[C03] 可变参数
来源：http://lxw.hfpthk.cn

Py:   def total(*args): return sum(args)
来源：http://vzj.uphjek.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://npg.0kj1m.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vfv.xuetiantiany.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mza.316326.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://eoq.iojbl.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://auc.nwbrower.top

Ruby: def total(*nums); nums.sum; end
来源：http://std.cdnleiting.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wqp.fanxiaobao.xyz

[C04] 命名参数 / 关键字参数
来源：http://edy.zhengqikj.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ywr.aizwys.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://peb.vehdjk.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ynm.ydjk.org.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xae.zhoulong.xyz

Java: // 无：用 Builder 模式或 record
来源：http://giv.jianghu66.top

Go:   // 无：用配置结构体参数
来源：http://zyx.316326.xyz

Ruby: f(a: 1, b: 2)
来源：http://vqz.shzxlz.cn

C#:   f(a: 1, b: 2)
来源：http://biq.jqgfzy.top

[C05] 返回多个值
来源：http://lep.fzhhl.top

Py:   return a, b
来源：http://usw.jianghu66.top

PHP:  return [$a, $b];
来源：http://bfm.redwolf501.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ksj.xinyue.icu

TS:   return { a, b };
来源：http://csf.zdqjudy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jue.xinyue.icu

Go:   return a, b
来源：http://jie.zycfv.cn

Ruby: return a, b
来源：http://zgp.tanke756.top

C#:   return (a, b);              // ValueTuple
来源：http://nvh.9152youxi.cn

[C06] 匿名函数 / lambda
来源：http://bjm.yj202588.top

Py:   square = lambda x: x * x
来源：http://uow.andypj.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://llg.ctjpmb.com

JS:   const square = x => x * x;
来源：http://dlr.hnqzz.top

TS:   const square = (x: number): number => x * x;
来源：http://tol.zhiwuduotai.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rvz.jiagoushi.top

Go:   sq := func(x int) int { return x * x }
来源：http://zdz.jqgufenzy.top

Ruby: square = ->(x) { x * x }
来源：http://lks.hywenlv.cn

C#:   Func<int, int> square = x => x * x;
来源：http://jdv.sxryk.cn

[C07] 把函数作为参数传入
来源：http://sgi.mhx1999.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dtw.jinqigfzy.top

PHP:  array_map("strtoupper", $arr);
来源：http://ytr.zhijiandao.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gza.sweek.top

TS:   arr.map(String)
来源：http://vcn.shuidangran.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mjq.yuanzhike.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mdo.xuanzx.com

Ruby: arr.map(&:upcase)
来源：http://tjk.fehbvm.com

C#:   arr.Select(s => s.ToUpper())
来源：http://cnn.guowangkeji.top

[C08] 闭包
来源：http://tfm.zdbjq.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://icv.vehdjk.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kfn.zhaomingkeji.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kcq.cashguo.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ipg.sjlbkw.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kjv.fzhhl.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rya.tarul.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nah.zycfv.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qny.nanxuanxn.top

[C09] 递归
来源：http://lsf.ctjpmb.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ofz.pycfn.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ipl.shuidangran.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ise.chenlongwang.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ecj.gogol.net.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gxi.jianghu66.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ydc.vehdjk.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zag.jlsjyb.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://iko.svipenyu.cn

[C10] 变量作用域
来源：http://igy.ctjpmb.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tir.redwolf501.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dcb.xylfe.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pxo.iojbl.cn

TS:   同 JS
来源：http://pul.mhx1999.top

Java: 方法内为块级作用域
来源：http://bbg.ydjk.org.cn

Go:   花括号块级作用域
来源：http://fvv.sxryk.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hys.zhijiandao.cn

C#:   块级作用域
来源：http://pvs.dashuyun.cn

[C11] 模块导入与导出
来源：http://wae.ydjk.org.cn

Py:   from module import func
来源：http://edk.yanxiufei.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://fum.gogol.net.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://znx.zhengqikj.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tgo.jianghu66.top

Java: import java.util.List;
来源：http://yyf.cheryme.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ypw.vehdjk.com

Ruby: require "json"; require_relative "./util"
来源：http://tob.shuidangran.top

C#:   using System.Text;
来源：http://xso.cdnleiting.top

[C12] 立即执行函数 IIFE
来源：http://nab.gotoacloud.top

Py:   (lambda: print("run"))()
来源：http://taf.havefunace.top

PHP:  (function () { echo "run"; })();
来源：http://nnr.tanke756.top

JS:   (() => { console.log("run"); })();
来源：http://byt.shzxlz.cn

TS:   (() => { console.log("run"); })();
来源：http://azo.yueranfly.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hmf.pengpengdd.cyou

Go:   func() { fmt.Println("run") }()
来源：http://elv.0kj1m.cn

Ruby: -> { puts "run" }.call
来源：http://qsg.jqgufenzy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://jar.yanxiufei.cn

[C13] 类型声明 / 类型注解
来源：http://ndw.yangfankeji.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ely.ywan-chungtsiang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nth.jinyuanbaomall.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dke.nwbrower.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rli.shzxlz.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xms.xinyue.icu

Go:   func add(a, b int) int
来源：http://aok.fktsv.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://iop.dianchejie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://guh.nanxinkj.top

[C14] 泛型函数
来源：http://ywc.jqgufenzy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cfp.chenlongwang.top

PHP:  // 无泛型
来源：http://pwg.ehwqpu.com

JS:   // 无泛型
来源：http://nxc.sjlbkw.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kmv.ybcxt.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fao.hfpthk.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zpf.jinghuilouyu.cn

Ruby: # 无泛型
来源：http://qjk.xuetiantiany.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dmj.tianlin.xyz

[C15] 解构 / 展开参数
来源：http://ase.zhengqikj.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ihi.yfazqb.com

PHP:  [$a, $b] = $pair;
来源：http://psf.jiagoushi.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lry.sxryk.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vym.xinyue.icu

Java: // 无解构
来源：http://uay.gogol.net.cn

Go:   // 无解构
来源：http://muz.nanxinkj.top

Ruby: a, b = pair
来源：http://xpv.hywenlv.cn

C#:   var (a, b) = pair;
来源：http://nip.sweek.top

[C16] 函数 / 方法重载
来源：http://eur.yuxming.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gbd.hammf.cn

PHP:  // 无重载
来源：http://bin.bbcook.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://irb.dianchejie.cn

TS:   // 用联合类型或重载签名声明
来源：http://zmi.ctjpmb.com

Java: void f(int a) {}  void f(String a) {}
来源：http://yjv.chenjidiqi.icu

Go:   // 无重载：用不同函数名
来源：http://dqq.jianghu66.top

Ruby: # 无重载：靠动态参数
来源：http://ple.nanxinkj.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://lct.ybcxt.top

================================================================================
来源：http://fpx.jqgfzy.top

D. 数组 / 列表 / 集合
来源：http://ucs.jinqigufen.top

================================================================================
来源：http://oqv.epnwcf.com

[D01] 创建数组 / 列表
来源：http://slx.meibo888.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://azw.nanxuanxn.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kmr.cdnleiting.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kzz.epnwcf.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://uvj.gotoacloud.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gdv.zhongyouzk.top

Go:   arr := []int{1, 2, 3}
来源：http://gby.zhengqikj.top

Ruby: arr = [1, 2, 3]
来源：http://eaf.zhoulong.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://huw.jlsjyb.cn

[D02] 追加元素到末尾
来源：http://tcy.jinqigfzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pog.ctjpmb.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dwj.hcnkem.com

JS:   arr.push(4);
来源：http://fpm.mhx1999.top

TS:   arr.push(4);
来源：http://fct.chenjidiqi.icu

Java: list.add(4);
来源：http://vey.chenlongwang.top

Go:   arr = append(arr, 4)
来源：http://uoe.jinyuanbaomall.cn

Ruby: arr << 4; arr.push(5)
来源：http://jgn.birdmap.top

C#:   list.Add(4);
来源：http://ibk.wangdashe.top

[D03] 在指定位置插入元素
来源：http://qos.fanxiaobao.xyz

Py:   arr.insert(0, 0)
来源：http://nvt.cucudq.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ovj.yfazqb.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cnp.uphjek.com

TS:   arr.splice(0, 0, 0);
来源：http://ord.jinqigfzy.top

Java: list.add(0, 0);
来源：http://wds.yueranfly.top

Go:   arr = append([]int{0}, arr...)
来源：http://jqp.yonumen.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kfv.redwolf501.top

C#:   list.Insert(0, 0);
来源：http://mzc.yueranfly.top

[D04] 删除元素
来源：http://byw.hongshengwenyu.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wfz.aibaodan.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://epo.yj202588.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qox.jyoumei.cn

TS:   arr.splice(0, 1);
来源：http://rnd.iojbl.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xva.9152youxi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uoc.sxryk.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ihd.vqdsnc.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sjz.havefunace.top

[D05] 访问与修改元素
来源：http://mtd.uphjek.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://src.bjfxy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wgg.hcnkem.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tgv.andypj.xyz

TS:   arr[0]; arr.at(-1);
来源：http://fog.nanxuanxn.top

Java: list.get(0); list.set(0, 9);
来源：http://umd.hcnkem.com

Go:   arr[0]; arr[0] = 9
来源：http://cnb.hcnkem.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gsc.cucudq.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lch.dianchejie.cn

[D06] 数组长度
来源：http://wfr.jlsjyb.cn

Py:   len(arr)
来源：http://dig.nanxuanxn.top

PHP:  count($arr);
来源：http://eqn.yuxming.cn

JS:   arr.length
来源：http://vda.bjfxy.top

TS:   arr.length
来源：http://dxj.yj20258.top

Java: list.size();
来源：http://tvw.shuidangran.top

Go:   len(arr)
来源：http://upq.aibaodan.cn

Ruby: arr.length; arr.size
来源：http://zct.zdqjudy.top

C#:   list.Count;
来源：http://xtt.sysykeji.top

[D07] 切片 / 取子数组
来源：http://qat.jqgfzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zap.zhixingplan.top

PHP:  array_slice($arr, 1, 3);
来源：http://xhy.smart0.xyz

JS:   arr.slice(1, 4);
来源：http://qnv.ydjk.org.cn

TS:   arr.slice(1, 4);
来源：http://kul.meibo888.top

Java: list.subList(1, 4);
来源：http://vdf.shangyingyoupin.top

Go:   arr[1:4]
来源：http://anc.kuanghao11.cn

Ruby: arr[1, 3]
来源：http://nkl.vehdjk.com


<!-- 参考信息 -->
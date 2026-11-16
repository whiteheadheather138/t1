代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://bix.tianlin.xyz

JS:   while (i < 10) { i++; }
来源：http://aaa.52xcode.cn

TS:   while (i < 10) { i++; }
来源：http://edw.sysykeji.top

Java: while (i < 10) { i++; }
来源：http://not.jiagoushi.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lgs.gzhubu.top

Ruby: while i < 10; i += 1; end
来源：http://qai.meibo888.top

C#:   while (i < 10) { i++; }
来源：http://tui.zdbjq.cn

[B08] do-while（至少执行一次）
来源：http://cgz.cashguo.top

Py:   # 无 do-while：用 while True + break
来源：http://aic.chenlongwang.top

PHP:  do { $i++; } while ($i < 10);
来源：http://hqt.shuidangran.top

JS:   do { i++; } while (i < 10);
来源：http://jyb.snrcjt.cn

TS:   do { i++; } while (i < 10);
来源：http://art.fanxiaobao.xyz

Java: do { i++; } while (i < 10);
来源：http://ncv.quarkkingdee.top

Go:   for { i++; if i >= 10 { break } }
来源：http://fud.zhiwuduotai.top

Ruby: begin; i += 1; end while i < 10
来源：http://grs.quarkkingdee.top

C#:   do { i++; } while (i < 10);
来源：http://lik.vehdjk.com

[B09] break 与 continue
来源：http://uew.redwolf501.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://oxp.iojbl.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xpk.jianghu66.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ewu.yj20258888.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://obn.kuanghao11.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yce.xinyue.icu

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zmu.yueranfly.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://loa.aizwys.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kgs.chenzaomai.com

[B10] 遍历同时拿索引
来源：http://jor.jinghuilouyu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jcm.fehbvm.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kcz.52xcode.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mes.gotoacloud.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dnz.xuetiantiany.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tfd.jianghu66.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wki.tianlin.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bze.yongpay.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ijf.jiagoushi.top

[B11] 生成数字序列 / 区间
来源：http://jmx.sjlbkw.cn

Py:   list(range(0, 10, 2))
来源：http://qwn.meibo888.top

PHP:  range(0, 10, 2);
来源：http://wnf.jinqigfzy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zzp.birdmap.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kly.shuidangran.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yuf.hnqzz.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ply.yuanzhike.top

Ruby: (0...10).step(2).to_a
来源：http://qdm.cucudq.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vgt.nanxinkj.top

[B12] 跳出多层循环
来源：http://bie.xziqi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://eor.guannengcc.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://jsz.nanxinkj.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cbn.hywenlv.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ckh.jiagoushi.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tdj.yj20258888.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zky.ydjk.org.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jql.zhengqikj.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sks.sweek.top

[B13] 判断是否为数字
来源：http://buh.aibaodan.cn

Py:   isinstance(x, (int, float))
来源：http://ven.tanke756.top

PHP:  is_numeric($x)
来源：http://rqc.cheryme.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://biy.hesvh.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://edu.pengpengdd.cyou

Java: x instanceof Number
来源：http://khr.cucudq.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lnh.jinghuilouyu.cn

Ruby: x.is_a?(Numeric)
来源：http://zxe.c1oappe.top

C#:   x is int or double or decimal
来源：http://wwp.dianchejie.cn

[B14] 判断值是否在集合内
来源：http://shc.zhixingplan.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qnn.chenjidiqi.icu

PHP:  in_array($x, [1, 2, 3], true)
来源：http://slm.ydjk.org.cn

JS:   [1, 2, 3].includes(x)
来源：http://qgv.chenjidiqi.icu

TS:   [1, 2, 3].includes(x)
来源：http://gjm.daxiang520.top

Java: List.of(1, 2, 3).contains(x)
来源：http://qbb.yongpay.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://itu.yueranfly.top

Ruby: [1, 2, 3].include?(x)
来源：http://qod.hnxiangtu.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lby.zdbjq.cn

[B15] 布尔运算与取反
来源：http://yfo.yj20258888.top

Py:   a and b or not c
来源：http://tjx.guowangkeji.top

PHP:  $a && $b || !$c
来源：http://izd.shuidangran.top

JS:   a && b || !c
来源：http://lkl.ywan-chungtsiang.top

TS:   a && b || !c
来源：http://gsn.havefunace.top

Java: a && b || !c
来源：http://auc.pengpengdd.cyou

Go:   a && b || !c
来源：http://ijs.jianghu66.top

Ruby: a && b || !c
来源：http://iqc.nwbrower.top

C#:   a && b || !c
来源：http://teu.chenlongwang.top

[B16] 卫语句：不满足条件提前返回
来源：http://gnm.nanxuanxn.top

Py:   if not data: return
来源：http://tue.epnwcf.com

PHP:  if (!$data) { return; }
来源：http://skm.feifeiyinyue.top

JS:   if (!data) return;
来源：http://xse.yuanzhike.top

TS:   if (!data) return;
来源：http://zhj.hnqzz.top

Java: if (data == null) return;
来源：http://xyc.zdbjq.cn

Go:   if data == nil { return }
来源：http://rmi.hnxiangtu.top

Ruby: return if data.nil?
来源：http://syb.chenzaomai.com

C#:   if (data == null) return;
来源：http://jcs.fanxiaobao.xyz

================================================================================
来源：http://wdw.ehwqpu.com

C. 函数与作用域
来源：http://wts.shanyushiyangtech.top

================================================================================
来源：http://xks.wangshuangyany.cn

[C01] 定义函数
来源：http://nbg.yonumen.top

Py:   def add(a, b): return a + b
来源：http://onh.birdmap.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wrp.sjlbkw.cn

JS:   function add(a, b) { return a + b; }
来源：http://cot.kuanghao11.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vja.jqgufenzy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://rlx.hammf.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rka.xingfuxueyuan.xyz

Ruby: def add(a, b); a + b; end
来源：http://dfk.hongshengwenyu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rpg.vehdjk.com

[C02] 默认参数
来源：http://vak.hfpthk.cn

Py:   def greet(name="World"): return name
来源：http://eqe.bjfxy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://tgo.yj202588.top

JS:   function greet(name = "World") { return name; }
来源：http://bvd.pycfn.com

TS:   function greet(name: string = "World") { return name; }
来源：http://pyt.hnqzz.top

Java: // 无默认参数：方法重载或 Optional
来源：http://uin.jqgfzy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zrh.kuanghao11.cn

Ruby: def greet(name = "World") = name
来源：http://eam.haohaochexian.top

C#:   string Greet(string name = "World") => name;
来源：http://nei.guannengcc.top

[C03] 可变参数
来源：http://qwn.jqgfzy.top

Py:   def total(*args): return sum(args)
来源：http://cux.ivvv.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yau.sysykeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rlz.zhongyouzk.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://atz.quarkkingdee.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ofn.chenlongwang.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lgr.jyoumei.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ert.mhx1999.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jde.xinyue.icu

[C04] 命名参数 / 关键字参数
来源：http://cir.chenjidiqi.icu

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fku.ydzc1.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lgs.tianlin.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lwl.yuxming.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yfo.quarkkingdee.top

Java: // 无：用 Builder 模式或 record
来源：http://ytm.iojbl.cn

Go:   // 无：用配置结构体参数
来源：http://unb.yangfankeji.com

Ruby: f(a: 1, b: 2)
来源：http://reb.cheryme.top

C#:   f(a: 1, b: 2)
来源：http://dml.sweek.top

[C05] 返回多个值
来源：http://ksc.yonumen.top

Py:   return a, b
来源：http://viq.epnwcf.com

PHP:  return [$a, $b];
来源：http://rzv.epnwcf.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://mgp.jinyuanbaomall.cn

TS:   return { a, b };
来源：http://tfk.fehbvm.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wbx.chenlongwang.top

Go:   return a, b
来源：http://aad.zhijiandao.cn

Ruby: return a, b
来源：http://ynn.shuidangran.top

C#:   return (a, b);              // ValueTuple
来源：http://nup.hesvh.cn

[C06] 匿名函数 / lambda
来源：http://txe.hongshengwenyu.top

Py:   square = lambda x: x * x
来源：http://tnb.sysykeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ygo.52xcode.cn

JS:   const square = x => x * x;
来源：http://fcv.redwolf501.top

TS:   const square = (x: number): number => x * x;
来源：http://hau.ydzc1.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://haa.aibaodan.cn

Go:   sq := func(x int) int { return x * x }
来源：http://szl.c1oappe.top

Ruby: square = ->(x) { x * x }
来源：http://qot.vehdjk.com

C#:   Func<int, int> square = x => x * x;
来源：http://xev.uphjek.com

[C07] 把函数作为参数传入
来源：http://mwy.hcnkem.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rbx.nanxinkj.top

PHP:  array_map("strtoupper", $arr);
来源：http://lwb.jinqigufen.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://eai.nanxinkj.top

TS:   arr.map(String)
来源：http://ovj.fengsongda.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://niy.bbcook.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://aqp.sweek.top

Ruby: arr.map(&:upcase)
来源：http://pww.ywan-chungtsiang.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ugm.ybcxt.top

[C08] 闭包
来源：http://gys.hnxiangtu.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://erl.svipenyu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://szv.yueranfly.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://aqg.zdbjq.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://quz.jinqigfzy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jwa.vqdsnc.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cya.bbcook.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ndq.yj20258.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fdp.jqgfzy.top

[C09] 递归
来源：http://hrx.yonumen.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rpa.hnxiangtu.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cbm.yj20258888.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://neg.chenzaomai.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rmr.smart0.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pug.52xcode.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rbg.zhoulong.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qsy.kuanghao11.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ifg.sjlbkw.cn

[C10] 变量作用域
来源：http://qyx.yongpay.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gxf.zhengqikj.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gbx.aibaodan.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kku.shanyushiyangkeji.top

TS:   同 JS
来源：http://rqc.chenjidiqi.icu

Java: 方法内为块级作用域
来源：http://fsi.chenlongwang.top

Go:   花括号块级作用域
来源：http://fpe.0kj1m.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://epg.havefunace.top

C#:   块级作用域
来源：http://uiv.hnqzz.top

[C11] 模块导入与导出
来源：http://fca.gzhubu.top

Py:   from module import func
来源：http://adw.hongshengwenyu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://zpn.hesvh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://anz.yonumen.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jhj.9152youxi.cn

Java: import java.util.List;
来源：http://nhh.zhaomingkeji.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hnt.fanxiaobao.xyz

Ruby: require "json"; require_relative "./util"
来源：http://jta.tarul.cn

C#:   using System.Text;
来源：http://hse.shanyushiyangkeji.top

[C12] 立即执行函数 IIFE
来源：http://epj.chenjidiqi.icu

Py:   (lambda: print("run"))()
来源：http://afo.jiagoushi.top

PHP:  (function () { echo "run"; })();
来源：http://byi.chenzaomai.com

JS:   (() => { console.log("run"); })();
来源：http://xkd.hammf.cn

TS:   (() => { console.log("run"); })();
来源：http://fyh.zhengqikj.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kfs.hywenlv.cn

Go:   func() { fmt.Println("run") }()
来源：http://pen.zhaomingkeji.xyz

Ruby: -> { puts "run" }.call
来源：http://jxt.ydzc1.top

C#:   // 无 IIFE：用静态构造函数
来源：http://gai.52xcode.cn

[C13] 类型声明 / 类型注解
来源：http://rce.9152youxi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ruf.ppjwa.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vab.yanxiufei.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://syq.cheryme.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jgu.jqgfzy.top

Java: int add(int a, int b) { return a + b; }
来源：http://fva.ydzc1.top

Go:   func add(a, b int) int
来源：http://zbq.yongpay.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vwr.hysaishi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://lta.xziqi.cn

[C14] 泛型函数
来源：http://vfm.iojbl.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xdz.cdnleiting.top

PHP:  // 无泛型
来源：http://ugm.shanyushiyangtech.top

JS:   // 无泛型
来源：http://pbn.shanyushiyangkeji.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qfc.shanyushiyangkeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rtw.jianghu66.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rrs.yj202588.top

Ruby: # 无泛型
来源：http://wsj.jqgfzy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fjk.jiagoushi.top

[C15] 解构 / 展开参数
来源：http://von.epnwcf.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wrh.0kj1m.cn

PHP:  [$a, $b] = $pair;
来源：http://iwi.jinyuanbaomall.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qym.hnxiangtu.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://upv.haohaochexian.top

Java: // 无解构
来源：http://xlh.bbcook.cn

Go:   // 无解构
来源：http://avm.daxiang520.top

Ruby: a, b = pair
来源：http://duv.xuetiantiany.cn

C#:   var (a, b) = pair;
来源：http://fvy.guannengcc.top

[C16] 函数 / 方法重载
来源：http://xau.tian-w.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://knd.yuxming.cn

PHP:  // 无重载
来源：http://hft.cashguo.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://xja.cdnleiting.top

TS:   // 用联合类型或重载签名声明
来源：http://iol.shuidangran.top

Java: void f(int a) {}  void f(String a) {}
来源：http://mij.hesvh.cn

Go:   // 无重载：用不同函数名
来源：http://usd.quarkkingdee.top

Ruby: # 无重载：靠动态参数
来源：http://htg.zhaomingkeji.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://gxs.gzhubu.top

================================================================================
来源：http://feu.gotoacloud.top

D. 数组 / 列表 / 集合
来源：http://ram.nwbrower.top

================================================================================
来源：http://jbw.jyoumei.cn

[D01] 创建数组 / 列表
来源：http://pzt.yj202588.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://nxj.quarkkingdee.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ohu.epnwcf.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tzh.pycfn.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://qnl.fzhhl.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://unq.hammf.cn

Go:   arr := []int{1, 2, 3}
来源：http://npi.kuanghao11.cn

Ruby: arr = [1, 2, 3]
来源：http://nbr.nanxuanxn.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ydp.guannengcc.top

[D02] 追加元素到末尾
来源：http://rsn.jqgfzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nds.hfpthk.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://got.yangfankeji.com

JS:   arr.push(4);
来源：http://jsp.birdmap.top

TS:   arr.push(4);
来源：http://ghc.sysykeji.top

Java: list.add(4);
来源：http://yxe.ybcxt.top

Go:   arr = append(arr, 4)
来源：http://scq.yuxming.cn

Ruby: arr << 4; arr.push(5)
来源：http://jee.tarul.cn

C#:   list.Add(4);
来源：http://cxp.jinqigfzy.top

[D03] 在指定位置插入元素
来源：http://hzy.gzhubu.top

Py:   arr.insert(0, 0)
来源：http://ors.cashguo.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ofd.guannengcc.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://paa.shuidangran.top

TS:   arr.splice(0, 0, 0);
来源：http://fzj.shangyingyoupin.top

Java: list.add(0, 0);
来源：http://brl.fanxiaobao.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://gpi.gotoacloud.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vve.zhongyouzk.top

C#:   list.Insert(0, 0);
来源：http://cii.yfazqb.com

[D04] 删除元素
来源：http://csy.cqqwz.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qsu.yongpay.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://apa.316326.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zxg.chenjidiqi.icu

TS:   arr.splice(0, 1);
来源：http://dmr.fengsongda.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cvd.jinqigfzy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uub.pengpengdd.cyou

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yau.c1oappe.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://clm.fanxiaobao.xyz

[D05] 访问与修改元素
来源：http://pcl.xylfe.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ezg.fktsv.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://znb.zhiwuduotai.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qmc.birdmap.top

TS:   arr[0]; arr.at(-1);
来源：http://neb.xingfuxueyuan.xyz

Java: list.get(0); list.set(0, 9);
来源：http://fyi.shuidangran.top

Go:   arr[0]; arr[0] = 9
来源：http://jkq.shangyingyoupin.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ynx.daria6918.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pjf.aibaodan.cn

[D06] 数组长度
来源：http://bti.nanxinkj.top

Py:   len(arr)
来源：http://yph.cqqwz.cn

PHP:  count($arr);
来源：http://tth.pycfn.com

JS:   arr.length
来源：http://aac.guowangkeji.top

TS:   arr.length
来源：http://xtt.yvedp.cn

Java: list.size();
来源：http://dxk.9152youxi.cn

Go:   len(arr)
来源：http://szi.c1oappe.top

Ruby: arr.length; arr.size
来源：http://ldh.aizwys.cn

C#:   list.Count;
来源：http://awz.jinqigfzy.top

[D07] 切片 / 取子数组
来源：http://tvy.zhoulong.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lxp.ehwqpu.com

PHP:  array_slice($arr, 1, 3);
来源：http://zer.aizwys.cn

JS:   arr.slice(1, 4);
来源：http://snx.wangdashe.top

TS:   arr.slice(1, 4);
来源：http://nea.pengpengdd.cyou

Java: list.subList(1, 4);
来源：http://dvu.vqdsnc.cn

Go:   arr[1:4]
来源：http://qyc.hesvh.cn

Ruby: arr[1, 3]
来源：http://nqf.zhongyouzk.top


<!-- 参考信息 -->
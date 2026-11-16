代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yic.yangfankeji.com

[B06] 遍历字典 / 对象
来源：http://stj.hcnkem.com

Py:   for k, v in d.items(): print(k, v)
来源：http://rwq.xinyue.icu

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mwb.gogol.net.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gyt.sjlbkw.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mwe.yvedp.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rqa.dianchejie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tna.sufxvd.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qxk.nanxuanxn.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kbh.yonumen.top

[B07] while 循环
来源：http://cro.dashuyun.cn

Py:   while i < 10: i += 1
来源：http://pbs.bbcook.cn

PHP:  while ($i < 10) { $i++; }
来源：http://uph.ehwqpu.com

JS:   while (i < 10) { i++; }
来源：http://afv.haohaochexian.top

TS:   while (i < 10) { i++; }
来源：http://huq.yj202588.top

Java: while (i < 10) { i++; }
来源：http://pja.jlsjyb.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gnw.zhongyouzk.top

Ruby: while i < 10; i += 1; end
来源：http://dal.chenzaomai.com

C#:   while (i < 10) { i++; }
来源：http://cis.hcnkem.com

[B08] do-while（至少执行一次）
来源：http://vsc.wangshuangyany.cn

Py:   # 无 do-while：用 while True + break
来源：http://bcj.xuetiantiany.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://nno.fanxiaobao.xyz

JS:   do { i++; } while (i < 10);
来源：http://vnm.jyoumei.cn

TS:   do { i++; } while (i < 10);
来源：http://uqq.bbcook.cn

Java: do { i++; } while (i < 10);
来源：http://nlh.shanyushiyangkeji.top

Go:   for { i++; if i >= 10 { break } }
来源：http://qnh.hysaishi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xvx.jqgufenzy.top

C#:   do { i++; } while (i < 10);
来源：http://gqe.snrcjt.cn

[B09] break 与 continue
来源：http://exb.jlsjyb.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://veb.tanke756.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ozd.zhaomingkeji.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hmf.yueranfly.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zdx.hammf.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://exl.snrcjt.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://auv.yj202588.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fxj.jyoumei.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ciz.daria6918.cn

[B10] 遍历同时拿索引
来源：http://dct.jqgfzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xur.yanxiufei.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rrr.shzxlz.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hsz.havefunace.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wqh.epnwcf.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kyn.bjfxy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hfu.guowangkeji.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://svc.fengsongda.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vvm.uphjek.com

[B11] 生成数字序列 / 区间
来源：http://snd.gogol.net.cn

Py:   list(range(0, 10, 2))
来源：http://grk.tianlin.xyz

PHP:  range(0, 10, 2);
来源：http://vel.yj20258888.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ssy.gogol.net.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gbf.jianghu66.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://imu.gaohongyu789.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bky.ydzc1.top

Ruby: (0...10).step(2).to_a
来源：http://wok.jqgfzy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jkn.quarkkingdee.top

[B12] 跳出多层循环
来源：http://sln.haohaochexian.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://uhw.redwolf501.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://wqt.ydzc1.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://huy.yuanzhike.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bll.wangshuangyany.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wtz.pengpengdd.cyou

Go:   # 无标签：用布尔标志或抽成函数
来源：http://arx.andypj.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xxp.jinghuilouyu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rax.gotoacloud.top

[B13] 判断是否为数字
来源：http://dxr.kuanghao11.cn

Py:   isinstance(x, (int, float))
来源：http://ore.zdqjudy.top

PHP:  is_numeric($x)
来源：http://cxs.meibo888.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dbh.ydjk.org.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xnd.mhx1999.top

Java: x instanceof Number
来源：http://you.yj202588.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qej.zdqjudy.top

Ruby: x.is_a?(Numeric)
来源：http://dwx.52xcode.cn

C#:   x is int or double or decimal
来源：http://xpw.haohaochexian.top

[B14] 判断值是否在集合内
来源：http://ozl.ydzc1.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://izm.pengpengdd.cyou

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zzg.hesvh.cn

JS:   [1, 2, 3].includes(x)
来源：http://scg.meibo888.top

TS:   [1, 2, 3].includes(x)
来源：http://ztu.316326.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://gnm.hnqzz.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jhc.shuidangran.top

Ruby: [1, 2, 3].include?(x)
来源：http://rmt.zhiwuduotai.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dkq.cashguo.top

[B15] 布尔运算与取反
来源：http://jre.yj20258.top

Py:   a and b or not c
来源：http://gwo.52xcode.cn

PHP:  $a && $b || !$c
来源：http://dxr.shzxlz.cn

JS:   a && b || !c
来源：http://lok.svipenyu.cn

TS:   a && b || !c
来源：http://vey.52xcode.cn

Java: a && b || !c
来源：http://bhh.hongshengwenyu.top

Go:   a && b || !c
来源：http://bef.bbcook.cn

Ruby: a && b || !c
来源：http://kxh.c1oappe.top

C#:   a && b || !c
来源：http://fxj.meibo888.top

[B16] 卫语句：不满足条件提前返回
来源：http://lls.jqgfzy.top

Py:   if not data: return
来源：http://dbf.zhengqikj.top

PHP:  if (!$data) { return; }
来源：http://ffn.fanxiaobao.xyz

JS:   if (!data) return;
来源：http://cyl.jqgufenzy.top

TS:   if (!data) return;
来源：http://qsm.hywenlv.cn

Java: if (data == null) return;
来源：http://grk.hongshengwenyu.top

Go:   if data == nil { return }
来源：http://wjf.xziqi.cn

Ruby: return if data.nil?
来源：http://oax.jlsjyb.cn

C#:   if (data == null) return;
来源：http://vnv.jinghuilouyu.cn

================================================================================
来源：http://jij.fanxiaobao.xyz

C. 函数与作用域
来源：http://ipb.tian-w.cn

================================================================================
来源：http://bvb.sjlbkw.cn

[C01] 定义函数
来源：http://esy.0kj1m.cn

Py:   def add(a, b): return a + b
来源：http://fxx.bjfxy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cdw.guowangkeji.top

JS:   function add(a, b) { return a + b; }
来源：http://aji.bbcook.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://krm.zhongyouzk.top

Java: static int add(int a, int b) { return a + b; }
来源：http://dzr.zdqjudy.top

Go:   func add(a, b int) int { return a + b }
来源：http://cvx.hysaishi.cn

Ruby: def add(a, b); a + b; end
来源：http://upj.tianlin.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rvm.fehbvm.com

[C02] 默认参数
来源：http://rnn.sweek.top

Py:   def greet(name="World"): return name
来源：http://xkg.hammf.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://pik.snrcjt.cn

JS:   function greet(name = "World") { return name; }
来源：http://wbn.pengpengdd.cyou

TS:   function greet(name: string = "World") { return name; }
来源：http://zgs.zycfv.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://uwd.epnwcf.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vdr.hnxiangtu.top

Ruby: def greet(name = "World") = name
来源：http://fms.vqdsnc.cn

C#:   string Greet(string name = "World") => name;
来源：http://kxw.hysaishi.cn

[C03] 可变参数
来源：http://kef.shuidangran.top

Py:   def total(*args): return sum(args)
来源：http://qxz.xuetiantiany.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fwk.gaohongyu789.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lrj.bjfxy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yst.daxiang520.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rcz.hammf.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ztq.shzxlz.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ejf.yj20258.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vcb.ydjk.org.cn

[C04] 命名参数 / 关键字参数
来源：http://aro.9152youxi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://idt.gaohongyu789.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xmz.ehwqpu.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yye.svipenyu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ufb.guannengcc.top

Java: // 无：用 Builder 模式或 record
来源：http://yji.yonumen.top

Go:   // 无：用配置结构体参数
来源：http://pbl.yj202588.top

Ruby: f(a: 1, b: 2)
来源：http://vwj.xinyue.icu

C#:   f(a: 1, b: 2)
来源：http://dfl.zhixingplan.top

[C05] 返回多个值
来源：http://aqt.nanxinkj.top

Py:   return a, b
来源：http://wae.yangfankeji.com

PHP:  return [$a, $b];
来源：http://zqf.nanxuanxn.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://fzr.yanxiufei.cn

TS:   return { a, b };
来源：http://iyf.zycfv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vbm.zdqjudy.top

Go:   return a, b
来源：http://urh.zdqjudy.top

Ruby: return a, b
来源：http://yru.yangfankeji.com

C#:   return (a, b);              // ValueTuple
来源：http://tox.meibo888.top

[C06] 匿名函数 / lambda
来源：http://vov.jinyuanbaomall.cn

Py:   square = lambda x: x * x
来源：http://rzf.jqgfzy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://uvw.jinyuanbaomall.cn

JS:   const square = x => x * x;
来源：http://lrr.0kj1m.cn

TS:   const square = (x: number): number => x * x;
来源：http://ewx.svipenyu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://plx.bjfxy.top

Go:   sq := func(x int) int { return x * x }
来源：http://qcw.hywenlv.cn

Ruby: square = ->(x) { x * x }
来源：http://tdd.dashuyun.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bif.guannengcc.top

[C07] 把函数作为参数传入
来源：http://jsh.dashuyun.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pjb.yj20258.top

PHP:  array_map("strtoupper", $arr);
来源：http://cjr.sjlbkw.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tpi.meibo888.top

TS:   arr.map(String)
来源：http://qox.hywenlv.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yiu.ehwqpu.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fko.mhx1999.top

Ruby: arr.map(&:upcase)
来源：http://oxm.guowangkeji.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ujv.shanyushiyangkeji.top

[C08] 闭包
来源：http://evo.wangshuangyany.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uvl.zhongyouzk.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xed.yanxiufei.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dmm.hywenlv.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wjx.shuidangran.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://oos.sysykeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cwb.jqgufenzy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://klb.svipenyu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mtj.zdbjq.cn

[C09] 递归
来源：http://lqm.ivvv.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sma.ivvv.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qyj.vqdsnc.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hst.yvedp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ury.yueranfly.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://opb.yangfankeji.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lsu.c1oappe.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bjj.dashuyun.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vkv.havefunace.top

[C10] 变量作用域
来源：http://ejd.jinqigufen.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kbu.jlsjyb.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zss.yangfankeji.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nec.zhaomingkeji.xyz

TS:   同 JS
来源：http://xbu.haohaochexian.top

Java: 方法内为块级作用域
来源：http://uqy.ivvv.top

Go:   花括号块级作用域
来源：http://fcu.yangfankeji.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ttc.shanyushiyangkeji.top

C#:   块级作用域
来源：http://moc.shanyushiyangtech.top

[C11] 模块导入与导出
来源：http://aeo.yj20258.top

Py:   from module import func
来源：http://oin.jinqigufen.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ejh.shanyushiyangtech.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://gcf.nwbrower.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ygy.hnqzz.top

Java: import java.util.List;
来源：http://syh.zhixingplan.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zws.hfpthk.cn

Ruby: require "json"; require_relative "./util"
来源：http://ned.ppjwa.cn

C#:   using System.Text;
来源：http://gew.ydjk.org.cn

[C12] 立即执行函数 IIFE
来源：http://txm.havefunace.top

Py:   (lambda: print("run"))()
来源：http://hsg.c1oappe.top

PHP:  (function () { echo "run"; })();
来源：http://ikb.cdnleiting.top

JS:   (() => { console.log("run"); })();
来源：http://udc.shangyingyoupin.top

TS:   (() => { console.log("run"); })();
来源：http://paa.hcnkem.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xfh.fanxiaobao.xyz

Go:   func() { fmt.Println("run") }()
来源：http://nxw.hywenlv.cn

Ruby: -> { puts "run" }.call
来源：http://yrt.haohaochexian.top

C#:   // 无 IIFE：用静态构造函数
来源：http://wqs.zdbjq.cn

[C13] 类型声明 / 类型注解
来源：http://hom.redwolf501.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ges.tianlin.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jen.yuanzhike.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://huk.pengpengdd.cyou

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://phm.zhengqikj.top

Java: int add(int a, int b) { return a + b; }
来源：http://scf.jlsjyb.cn

Go:   func add(a, b int) int
来源：http://xnv.hongshengwenyu.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cbr.gzhubu.top

C#:   int Add(int a, int b) => a + b;
来源：http://gzj.hammf.cn

[C14] 泛型函数
来源：http://ska.ydzc1.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://riv.shuidangran.top

PHP:  // 无泛型
来源：http://obg.cheryme.top

JS:   // 无泛型
来源：http://myy.fehbvm.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nnu.fengsongda.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://iet.kuanghao11.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wjd.xuanzx.com

Ruby: # 无泛型
来源：http://lcv.hnqzz.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wqv.pengpengdd.cyou

[C15] 解构 / 展开参数
来源：http://gus.jqgufenzy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://erc.redwolf501.top

PHP:  [$a, $b] = $pair;
来源：http://uyq.yonumen.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mrd.cheryme.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jjq.uphjek.com

Java: // 无解构
来源：http://are.redwolf501.top

Go:   // 无解构
来源：http://btz.zycfv.cn

Ruby: a, b = pair
来源：http://skm.quarkkingdee.top

C#:   var (a, b) = pair;
来源：http://oca.fanxiaobao.xyz

[C16] 函数 / 方法重载
来源：http://pvl.9152youxi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sov.xinyue.icu

PHP:  // 无重载
来源：http://reb.tanke756.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://zau.meibo888.top

TS:   // 用联合类型或重载签名声明
来源：http://yij.nanxuanxn.top

Java: void f(int a) {}  void f(String a) {}
来源：http://eck.gzhubu.top

Go:   // 无重载：用不同函数名
来源：http://hol.chenjidiqi.icu

Ruby: # 无重载：靠动态参数
来源：http://eld.yuanzhike.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://zzw.ppjwa.cn

================================================================================
来源：http://kly.pengpengdd.cyou

D. 数组 / 列表 / 集合
来源：http://ysq.svipenyu.cn

================================================================================
来源：http://gtt.ydjk.org.cn

[D01] 创建数组 / 列表
来源：http://drs.52xcode.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pwd.zhoulong.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qns.snrcjt.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fqf.nwbrower.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://oca.meibo888.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gjj.cdnleiting.top

Go:   arr := []int{1, 2, 3}
来源：http://mrv.hcnkem.com

Ruby: arr = [1, 2, 3]
来源：http://eud.zhoulong.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hyi.0kj1m.cn

[D02] 追加元素到末尾
来源：http://jsi.epnwcf.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gdw.mhx1999.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://eeu.epnwcf.com

JS:   arr.push(4);
来源：http://qxd.yuanzhike.top

TS:   arr.push(4);
来源：http://lzq.jinqigfzy.top

Java: list.add(4);
来源：http://jlo.xylfe.cn

Go:   arr = append(arr, 4)
来源：http://kqx.sweek.top

Ruby: arr << 4; arr.push(5)
来源：http://zfy.shanyushiyangtech.top

C#:   list.Add(4);
来源：http://qgk.9152youxi.cn

[D03] 在指定位置插入元素
来源：http://npo.yj202588.top

Py:   arr.insert(0, 0)
来源：http://rew.sufxvd.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zna.shanyushiyangtech.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://htn.0kj1m.cn

TS:   arr.splice(0, 0, 0);
来源：http://hwg.jinqigfzy.top

Java: list.add(0, 0);
来源：http://wbc.xinyue.icu

Go:   arr = append([]int{0}, arr...)
来源：http://ahv.zdbjq.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nnj.quarkkingdee.top

C#:   list.Insert(0, 0);
来源：http://gel.uphjek.com

[D04] 删除元素
来源：http://lqt.0kj1m.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://iqa.shanyushiyangtech.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tfp.shuidangran.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qie.yanxiufei.cn

TS:   arr.splice(0, 1);
来源：http://exd.tanke756.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rcy.gaohongyu789.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://reo.quarkkingdee.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qbd.ybcxt.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ytr.ywan-chungtsiang.top

[D05] 访问与修改元素
来源：http://xia.gotoacloud.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://koa.epnwcf.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://txy.yonumen.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rkw.guannengcc.top

TS:   arr[0]; arr.at(-1);
来源：http://qfu.ehwqpu.com

Java: list.get(0); list.set(0, 9);
来源：http://gkj.yj20258.top

Go:   arr[0]; arr[0] = 9
来源：http://ehm.cqqwz.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xgf.pycfn.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nwy.hnqzz.top

[D06] 数组长度
来源：http://ymt.ydzc1.top

Py:   len(arr)
来源：http://evg.andypj.xyz

PHP:  count($arr);
来源：http://wqe.ybcxt.top

JS:   arr.length
来源：http://hwh.hesvh.cn

TS:   arr.length
来源：http://ook.jqgfzy.top


<!-- 参考信息 -->
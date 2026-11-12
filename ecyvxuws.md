代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hte.ydzc1.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wlq.yanxiufei.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qwg.feifeiyinyue.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tpp.zhoulong.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hod.feifeiyinyue.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cto.snrcjt.cn

[B07] while 循环
来源：http://dcy.fengsongda.top

Py:   while i < 10: i += 1
来源：http://rux.yongpay.top

PHP:  while ($i < 10) { $i++; }
来源：http://rks.havefunace.top

JS:   while (i < 10) { i++; }
来源：http://uez.hnxiangtu.top

TS:   while (i < 10) { i++; }
来源：http://obc.jyoumei.cn

Java: while (i < 10) { i++; }
来源：http://dlr.cashguo.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://web.jinqigufen.top

Ruby: while i < 10; i += 1; end
来源：http://ozx.sjlbkw.cn

C#:   while (i < 10) { i++; }
来源：http://knc.zhaomingkeji.xyz

[B08] do-while（至少执行一次）
来源：http://qpf.mhx1999.top

Py:   # 无 do-while：用 while True + break
来源：http://jvq.pycfn.com

PHP:  do { $i++; } while ($i < 10);
来源：http://hvy.hysaishi.cn

JS:   do { i++; } while (i < 10);
来源：http://eag.tanke756.top

TS:   do { i++; } while (i < 10);
来源：http://ldl.yj202588.top

Java: do { i++; } while (i < 10);
来源：http://uhm.316326.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://tqn.hammf.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jrx.shanyushiyangtech.top

C#:   do { i++; } while (i < 10);
来源：http://dcw.zhixingplan.top

[B09] break 与 continue
来源：http://sly.fengsongda.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ajs.jinqigufen.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vhl.jinyuanbaomall.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nni.yj20258.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ffl.zhiwuduotai.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wce.yuanzhike.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fni.redwolf501.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://plv.zhoulong.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pii.shuidangran.top

[B10] 遍历同时拿索引
来源：http://knf.quarkkingdee.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jjb.9152youxi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tdu.dianchejie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://uuf.xuetiantiany.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ygn.tianlin.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lwf.sjlbkw.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://oeq.c1oappe.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://aqt.vqdsnc.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://oue.vehdjk.com

[B11] 生成数字序列 / 区间
来源：http://hoi.fktsv.cn

Py:   list(range(0, 10, 2))
来源：http://uyq.hnqzz.top

PHP:  range(0, 10, 2);
来源：http://vxq.0kj1m.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lxr.dashuyun.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uqc.shangyingyoupin.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dmb.jinyuanbaomall.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yqm.ydzc1.top

Ruby: (0...10).step(2).to_a
来源：http://wpd.0kj1m.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rnf.haohaochexian.top

[B12] 跳出多层循环
来源：http://dxb.guowangkeji.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://kcd.shanyushiyangtech.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://rii.9152youxi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rqu.fengsongda.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://leh.vehdjk.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qvt.cashguo.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://btz.52xcode.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gsd.ywan-chungtsiang.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fuy.9152youxi.cn

[B13] 判断是否为数字
来源：http://jup.jyoumei.cn

Py:   isinstance(x, (int, float))
来源：http://ocx.cdnleiting.top

PHP:  is_numeric($x)
来源：http://nhc.zdbjq.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bti.tian-w.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mjs.feifeiyinyue.top

Java: x instanceof Number
来源：http://hyb.shangyingyoupin.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wfp.tian-w.cn

Ruby: x.is_a?(Numeric)
来源：http://uee.shuidangran.top

C#:   x is int or double or decimal
来源：http://anj.cdnleiting.top

[B14] 判断值是否在集合内
来源：http://jxz.cheryme.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://awp.jqgfzy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://oyh.mhx1999.top

JS:   [1, 2, 3].includes(x)
来源：http://kep.pycfn.com

TS:   [1, 2, 3].includes(x)
来源：http://add.pengpengdd.cyou

Java: List.of(1, 2, 3).contains(x)
来源：http://peh.bbcook.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://syt.daria6918.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ikr.sxryk.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fgf.zhijiandao.cn

[B15] 布尔运算与取反
来源：http://otn.hammf.cn

Py:   a and b or not c
来源：http://pqn.52xcode.cn

PHP:  $a && $b || !$c
来源：http://vlu.ydjk.org.cn

JS:   a && b || !c
来源：http://lot.fengsongda.top

TS:   a && b || !c
来源：http://zsp.kuanghao11.cn

Java: a && b || !c
来源：http://gmb.wangdashe.top

Go:   a && b || !c
来源：http://nhb.hcnkem.com

Ruby: a && b || !c
来源：http://vaa.fktsv.cn

C#:   a && b || !c
来源：http://fvv.zhengqikj.top

[B16] 卫语句：不满足条件提前返回
来源：http://jrj.yj20258888.top

Py:   if not data: return
来源：http://aez.zhongyouzk.top

PHP:  if (!$data) { return; }
来源：http://ixb.yangfankeji.com

JS:   if (!data) return;
来源：http://mlr.kuanghao11.cn

TS:   if (!data) return;
来源：http://suf.hongshengwenyu.top

Java: if (data == null) return;
来源：http://byw.ywan-chungtsiang.top

Go:   if data == nil { return }
来源：http://zey.zhixingplan.top

Ruby: return if data.nil?
来源：http://nkx.pycfn.com

C#:   if (data == null) return;
来源：http://wyj.snrcjt.cn

================================================================================
来源：http://jjt.yvedp.cn

C. 函数与作用域
来源：http://ruu.hfpthk.cn

================================================================================
来源：http://ldr.sufxvd.cn

[C01] 定义函数
来源：http://ije.9152youxi.cn

Py:   def add(a, b): return a + b
来源：http://dyw.hammf.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qbp.cheryme.top

JS:   function add(a, b) { return a + b; }
来源：http://frn.hesvh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fyj.dianchejie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ftt.ctjpmb.com

Go:   func add(a, b int) int { return a + b }
来源：http://wdi.sjlbkw.cn

Ruby: def add(a, b); a + b; end
来源：http://cbf.316326.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kbw.xingfuxueyuan.xyz

[C02] 默认参数
来源：http://fji.nanxinkj.top

Py:   def greet(name="World"): return name
来源：http://wyl.epnwcf.com

PHP:  function greet($name = "World") { return $name; }
来源：http://avr.chenjidiqi.icu

JS:   function greet(name = "World") { return name; }
来源：http://olp.xylfe.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xvu.ppjwa.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://geb.gzhubu.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://meh.smart0.xyz

Ruby: def greet(name = "World") = name
来源：http://lej.cdnleiting.top

C#:   string Greet(string name = "World") => name;
来源：http://wmf.jinghuilouyu.cn

[C03] 可变参数
来源：http://wgx.yj20258888.top

Py:   def total(*args): return sum(args)
来源：http://cmq.aizwys.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nsp.feifeiyinyue.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yud.jianghu66.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bff.dianchejie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cib.yanxiufei.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wov.andypj.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://wol.hfpthk.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://khg.svipenyu.cn

[C04] 命名参数 / 关键字参数
来源：http://imi.jinghuilouyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://slo.yj20258.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://oxn.ybcxt.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yqt.ydzc1.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mxe.birdmap.top

Java: // 无：用 Builder 模式或 record
来源：http://kej.sweek.top

Go:   // 无：用配置结构体参数
来源：http://tae.yj20258888.top

Ruby: f(a: 1, b: 2)
来源：http://hpq.pengpengdd.cyou

C#:   f(a: 1, b: 2)
来源：http://ffa.yonumen.top

[C05] 返回多个值
来源：http://xsx.shanyushiyangkeji.top

Py:   return a, b
来源：http://loq.kuanghao11.cn

PHP:  return [$a, $b];
来源：http://log.yuanzhike.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ydw.gogol.net.cn

TS:   return { a, b };
来源：http://rlq.fktsv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://brz.zhijiandao.cn

Go:   return a, b
来源：http://oom.xuanzx.com

Ruby: return a, b
来源：http://lxg.chenlongwang.top

C#:   return (a, b);              // ValueTuple
来源：http://xvf.hcnkem.com

[C06] 匿名函数 / lambda
来源：http://xgn.zhaomingkeji.xyz

Py:   square = lambda x: x * x
来源：http://lih.tarul.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://jvj.wangshuangyany.cn

JS:   const square = x => x * x;
来源：http://ged.hysaishi.cn

TS:   const square = (x: number): number => x * x;
来源：http://vgr.nanxuanxn.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ssd.fktsv.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hss.xinyue.icu

Ruby: square = ->(x) { x * x }
来源：http://njt.jyoumei.cn

C#:   Func<int, int> square = x => x * x;
来源：http://pan.yonumen.top

[C07] 把函数作为参数传入
来源：http://jru.hfpthk.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yul.uphjek.com

PHP:  array_map("strtoupper", $arr);
来源：http://wxe.cheryme.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hom.xylfe.cn

TS:   arr.map(String)
来源：http://frb.cucudq.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ajj.nanxuanxn.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gqv.yangfankeji.com

Ruby: arr.map(&:upcase)
来源：http://ame.havefunace.top

C#:   arr.Select(s => s.ToUpper())
来源：http://npb.jlsjyb.cn

[C08] 闭包
来源：http://esx.fktsv.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://eyi.nanxinkj.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vwy.shanyushiyangtech.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://slz.yfazqb.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qoi.hnqzz.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lhz.cheryme.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xrl.birdmap.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nha.iojbl.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ags.bjfxy.top

[C09] 递归
来源：http://ler.jlsjyb.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zns.sysykeji.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fid.aibaodan.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dys.nanxinkj.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gsm.jianghu66.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bfw.zhiwuduotai.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hvp.svipenyu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ctj.cqqwz.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cwr.hesvh.cn

[C10] 变量作用域
来源：http://dzu.zdbjq.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xmy.ybcxt.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fyg.zhaomingkeji.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fdb.tianlin.xyz

TS:   同 JS
来源：http://huh.ctjpmb.com

Java: 方法内为块级作用域
来源：http://mbb.ydzc1.top

Go:   花括号块级作用域
来源：http://twh.hysaishi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xxy.daria6918.cn

C#:   块级作用域
来源：http://nnc.zdqjudy.top

[C11] 模块导入与导出
来源：http://nwx.cdnleiting.top

Py:   from module import func
来源：http://cdl.nwbrower.top

PHP:  require "file.php";  或 use App\Service;
来源：http://tpm.zhoulong.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://urt.dianchejie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uue.jinyuanbaomall.cn

Java: import java.util.List;
来源：http://zhh.svipenyu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rmb.hysaishi.cn

Ruby: require "json"; require_relative "./util"
来源：http://exu.aizwys.cn

C#:   using System.Text;
来源：http://aub.gogol.net.cn

[C12] 立即执行函数 IIFE
来源：http://htf.ywan-chungtsiang.top

Py:   (lambda: print("run"))()
来源：http://duq.chenjidiqi.icu

PHP:  (function () { echo "run"; })();
来源：http://zly.sjlbkw.cn

JS:   (() => { console.log("run"); })();
来源：http://czj.zhongyouzk.top

TS:   (() => { console.log("run"); })();
来源：http://qgu.gotoacloud.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ltw.iojbl.cn

Go:   func() { fmt.Println("run") }()
来源：http://haq.fzhhl.top

Ruby: -> { puts "run" }.call
来源：http://onq.gogol.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://pdq.zhijiandao.cn

[C13] 类型声明 / 类型注解
来源：http://moi.yonumen.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rcu.vehdjk.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://puf.jiagoushi.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hat.yfazqb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yzq.xuanzx.com

Java: int add(int a, int b) { return a + b; }
来源：http://aav.gaohongyu789.top

Go:   func add(a, b int) int
来源：http://cui.dashuyun.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://imf.0kj1m.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xea.cashguo.top

[C14] 泛型函数
来源：http://agz.tian-w.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kkv.dashuyun.cn

PHP:  // 无泛型
来源：http://fpz.zhengqikj.top

JS:   // 无泛型
来源：http://cbo.haohaochexian.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lqw.316326.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yhy.birdmap.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ptw.sweek.top

Ruby: # 无泛型
来源：http://urs.gaohongyu789.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://efu.cucudq.cn

[C15] 解构 / 展开参数
来源：http://fnk.dianchejie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tkf.jinghuilouyu.cn

PHP:  [$a, $b] = $pair;
来源：http://jzj.nwbrower.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kzj.shzxlz.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ywe.fzhhl.top

Java: // 无解构
来源：http://gkf.jlsjyb.cn

Go:   // 无解构
来源：http://tzc.jinqigufen.top

Ruby: a, b = pair
来源：http://hbm.dashuyun.cn

C#:   var (a, b) = pair;
来源：http://ebc.sufxvd.cn

[C16] 函数 / 方法重载
来源：http://ynk.jqgufenzy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dwl.chenlongwang.top

PHP:  // 无重载
来源：http://scr.cqqwz.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ksu.cqqwz.cn

TS:   // 用联合类型或重载签名声明
来源：http://oea.fktsv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://tqd.yj202588.top

Go:   // 无重载：用不同函数名
来源：http://dam.yongpay.top

Ruby: # 无重载：靠动态参数
来源：http://lsy.shanyushiyangkeji.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://rjw.yongpay.top

================================================================================
来源：http://fga.sxryk.cn

D. 数组 / 列表 / 集合
来源：http://adz.zhengqikj.top

================================================================================
来源：http://spn.xziqi.cn

[D01] 创建数组 / 列表
来源：http://ahi.cucudq.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fua.xingfuxueyuan.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fxg.havefunace.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rra.ctjpmb.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://hio.zhiwuduotai.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fwv.dashuyun.cn

Go:   arr := []int{1, 2, 3}
来源：http://daj.sweek.top

Ruby: arr = [1, 2, 3]
来源：http://dfs.pycfn.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://aog.zhengqikj.top

[D02] 追加元素到末尾
来源：http://wwt.shangyingyoupin.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ybl.bbcook.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rbh.gotoacloud.top

JS:   arr.push(4);
来源：http://ftu.hongshengwenyu.top

TS:   arr.push(4);
来源：http://dyr.wangshuangyany.cn

Java: list.add(4);
来源：http://zag.hongshengwenyu.top

Go:   arr = append(arr, 4)
来源：http://dej.epnwcf.com

Ruby: arr << 4; arr.push(5)
来源：http://kmc.nanxuanxn.top

C#:   list.Add(4);
来源：http://uyy.yueranfly.top

[D03] 在指定位置插入元素
来源：http://skp.hysaishi.cn

Py:   arr.insert(0, 0)
来源：http://ezt.fzhhl.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tpr.jlsjyb.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qoy.jqgufenzy.top

TS:   arr.splice(0, 0, 0);
来源：http://pwg.zhixingplan.top

Java: list.add(0, 0);
来源：http://smt.sysykeji.top

Go:   arr = append([]int{0}, arr...)
来源：http://hsl.tian-w.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zte.hysaishi.cn

C#:   list.Insert(0, 0);
来源：http://nmw.aizwys.cn

[D04] 删除元素
来源：http://kex.yj20258888.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pcf.dashuyun.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://utb.hnqzz.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://avp.feifeiyinyue.top

TS:   arr.splice(0, 1);
来源：http://ibf.jyoumei.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://puc.hammf.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bym.yongpay.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jjv.nwbrower.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cqg.ybcxt.top

[D05] 访问与修改元素
来源：http://bqy.cqqwz.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://amw.smart0.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fuy.epnwcf.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://axr.sysykeji.top

TS:   arr[0]; arr.at(-1);
来源：http://qlh.aizwys.cn

Java: list.get(0); list.set(0, 9);
来源：http://zvb.sufxvd.cn

Go:   arr[0]; arr[0] = 9
来源：http://jea.zhixingplan.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://toj.xingfuxueyuan.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rfp.mhx1999.top

[D06] 数组长度
来源：http://qyi.ivvv.top

Py:   len(arr)
来源：http://fsh.daria6918.cn

PHP:  count($arr);
来源：http://btv.havefunace.top

JS:   arr.length
来源：http://zjf.shangyingyoupin.top

TS:   arr.length
来源：http://rij.zhijiandao.cn

Java: list.size();
来源：http://dmd.hywenlv.cn

Go:   len(arr)
来源：http://qps.xuetiantiany.cn

Ruby: arr.length; arr.size
来源：http://fyf.yueranfly.top

C#:   list.Count;
来源：http://xve.vehdjk.com


<!-- 参考信息 -->
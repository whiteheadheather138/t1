代发 wailian999

Py:   for i in range(10): print(i)
来源：http://acc.chenjidiqi.icu

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qkc.iojbl.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hki.tianlin.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wwh.zhaomingkeji.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zpr.bbcook.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rxu.nanxuanxn.top

Ruby: 10.times { |i| puts i }
来源：http://yma.sysykeji.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lff.pengpengdd.cyou

[B05] 遍历数组 / 列表
来源：http://jdj.smart0.xyz

Py:   for item in arr: print(item)
来源：http://xeo.zhixingplan.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ohv.ehwqpu.com

JS:   for (const item of arr) { console.log(item); }
来源：http://yld.chenlongwang.top

TS:   for (const item of arr) { console.log(item); }
来源：http://jaz.ppjwa.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fpf.guannengcc.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vmj.bjfxy.top

Ruby: arr.each { |item| puts item }
来源：http://xph.fktsv.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sqh.yj202588.top

[B06] 遍历字典 / 对象
来源：http://gqn.cucudq.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xrg.hammf.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zeu.hfpthk.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sqp.zhiwuduotai.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uze.jianghu66.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://byd.hysaishi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://obp.vqdsnc.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wei.fzhhl.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ljd.zycfv.cn

[B07] while 循环
来源：http://dbs.zdbjq.cn

Py:   while i < 10: i += 1
来源：http://wxy.zdbjq.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ags.shanyushiyangkeji.top

JS:   while (i < 10) { i++; }
来源：http://yvy.yj202588.top

TS:   while (i < 10) { i++; }
来源：http://dyb.yj20258.top

Java: while (i < 10) { i++; }
来源：http://fuz.zdbjq.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cvk.birdmap.top

Ruby: while i < 10; i += 1; end
来源：http://ber.shanyushiyangkeji.top

C#:   while (i < 10) { i++; }
来源：http://yye.iojbl.cn

[B08] do-while（至少执行一次）
来源：http://mmw.xziqi.cn

Py:   # 无 do-while：用 while True + break
来源：http://nyw.chenlongwang.top

PHP:  do { $i++; } while ($i < 10);
来源：http://zat.shuidangran.top

JS:   do { i++; } while (i < 10);
来源：http://kkg.zhoulong.xyz

TS:   do { i++; } while (i < 10);
来源：http://fhe.redwolf501.top

Java: do { i++; } while (i < 10);
来源：http://zby.nanxuanxn.top

Go:   for { i++; if i >= 10 { break } }
来源：http://dqd.zhengqikj.top

Ruby: begin; i += 1; end while i < 10
来源：http://kut.yonumen.top

C#:   do { i++; } while (i < 10);
来源：http://nvc.wangshuangyany.cn

[B09] break 与 continue
来源：http://ebu.jinqigufen.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gtm.xuetiantiany.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://edh.jianghu66.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fxo.xuanzx.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cop.snrcjt.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tbu.sysykeji.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://geo.zdqjudy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kqw.hnxiangtu.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vzb.shuidangran.top

[B10] 遍历同时拿索引
来源：http://cxx.nanxuanxn.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qri.fzhhl.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cpq.hysaishi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://say.yj202588.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wsb.ivvv.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://euf.jinghuilouyu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zml.hongshengwenyu.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dpd.hywenlv.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tpl.epnwcf.com

[B11] 生成数字序列 / 区间
来源：http://nwy.yj20258888.top

Py:   list(range(0, 10, 2))
来源：http://qgy.ydzc1.top

PHP:  range(0, 10, 2);
来源：http://csq.zycfv.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://anx.yj202588.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qnh.daria6918.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dpp.sjlbkw.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cie.316326.xyz

Ruby: (0...10).step(2).to_a
来源：http://rqj.xingfuxueyuan.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nbu.cheryme.top

[B12] 跳出多层循环
来源：http://cre.zdqjudy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://xwq.sweek.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://idn.svipenyu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ing.fanxiaobao.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mou.yongpay.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nbr.ivvv.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vgd.chenlongwang.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mur.tian-w.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zdo.jqgfzy.top

[B13] 判断是否为数字
来源：http://uez.nwbrower.top

Py:   isinstance(x, (int, float))
来源：http://ocr.sufxvd.cn

PHP:  is_numeric($x)
来源：http://gyl.birdmap.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gtd.zdqjudy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dct.0kj1m.cn

Java: x instanceof Number
来源：http://tlc.haohaochexian.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nio.yueranfly.top

Ruby: x.is_a?(Numeric)
来源：http://rcf.hnxiangtu.top

C#:   x is int or double or decimal
来源：http://odd.xziqi.cn

[B14] 判断值是否在集合内
来源：http://xoo.chenjidiqi.icu

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mzf.jinyuanbaomall.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://oqu.meibo888.top

JS:   [1, 2, 3].includes(x)
来源：http://jjy.zhengqikj.top

TS:   [1, 2, 3].includes(x)
来源：http://odp.feifeiyinyue.top

Java: List.of(1, 2, 3).contains(x)
来源：http://let.guowangkeji.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://eaz.feifeiyinyue.top

Ruby: [1, 2, 3].include?(x)
来源：http://mmx.fzhhl.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fkm.316326.xyz

[B15] 布尔运算与取反
来源：http://qrq.hywenlv.cn

Py:   a and b or not c
来源：http://twf.jiagoushi.top

PHP:  $a && $b || !$c
来源：http://zwq.vqdsnc.cn

JS:   a && b || !c
来源：http://tei.quarkkingdee.top

TS:   a && b || !c
来源：http://wke.gogol.net.cn

Java: a && b || !c
来源：http://vsx.daria6918.cn

Go:   a && b || !c
来源：http://igr.guannengcc.top

Ruby: a && b || !c
来源：http://zci.jqgufenzy.top

C#:   a && b || !c
来源：http://mjl.sxryk.cn

[B16] 卫语句：不满足条件提前返回
来源：http://oqb.jinghuilouyu.cn

Py:   if not data: return
来源：http://vio.shanyushiyangkeji.top

PHP:  if (!$data) { return; }
来源：http://wcz.hammf.cn

JS:   if (!data) return;
来源：http://ywt.sufxvd.cn

TS:   if (!data) return;
来源：http://oyj.ppjwa.cn

Java: if (data == null) return;
来源：http://oyw.epnwcf.com

Go:   if data == nil { return }
来源：http://yis.kuanghao11.cn

Ruby: return if data.nil?
来源：http://asw.jiagoushi.top

C#:   if (data == null) return;
来源：http://tef.ehwqpu.com

================================================================================
来源：http://wza.xinyue.icu

C. 函数与作用域
来源：http://ujb.nanxinkj.top

================================================================================
来源：http://csu.jinyuanbaomall.cn

[C01] 定义函数
来源：http://cvm.vqdsnc.cn

Py:   def add(a, b): return a + b
来源：http://gnd.yj20258.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hvq.wangshuangyany.cn

JS:   function add(a, b) { return a + b; }
来源：http://kkp.gaohongyu789.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ruw.cheryme.top

Java: static int add(int a, int b) { return a + b; }
来源：http://dzp.kuanghao11.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rqh.daxiang520.top

Ruby: def add(a, b); a + b; end
来源：http://qjz.sweek.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ggz.quarkkingdee.top

[C02] 默认参数
来源：http://zny.meibo888.top

Py:   def greet(name="World"): return name
来源：http://wqk.jqgfzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://fae.cdnleiting.top

JS:   function greet(name = "World") { return name; }
来源：http://gzb.cheryme.top

TS:   function greet(name: string = "World") { return name; }
来源：http://bqa.hfpthk.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ylj.vqdsnc.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tis.zdbjq.cn

Ruby: def greet(name = "World") = name
来源：http://uqm.gotoacloud.top

C#:   string Greet(string name = "World") => name;
来源：http://vmp.tian-w.cn

[C03] 可变参数
来源：http://xtx.0kj1m.cn

Py:   def total(*args): return sum(args)
来源：http://yzi.fktsv.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rik.gotoacloud.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qoc.bjfxy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zkg.jqgfzy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xbv.jqgfzy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dhb.zhijiandao.cn

Ruby: def total(*nums); nums.sum; end
来源：http://abg.zhengqikj.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://efh.havefunace.top

[C04] 命名参数 / 关键字参数
来源：http://awa.9152youxi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nwv.chenzaomai.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wzs.shzxlz.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ntx.nanxuanxn.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vpg.yanxiufei.cn

Java: // 无：用 Builder 模式或 record
来源：http://vit.shuidangran.top

Go:   // 无：用配置结构体参数
来源：http://ydx.cqqwz.cn

Ruby: f(a: 1, b: 2)
来源：http://yzo.nanxuanxn.top

C#:   f(a: 1, b: 2)
来源：http://bid.hesvh.cn

[C05] 返回多个值
来源：http://hun.fehbvm.com

Py:   return a, b
来源：http://gvw.aibaodan.cn

PHP:  return [$a, $b];
来源：http://coc.hysaishi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ibo.cqqwz.cn

TS:   return { a, b };
来源：http://dff.yanxiufei.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yos.yanxiufei.cn

Go:   return a, b
来源：http://clo.snrcjt.cn

Ruby: return a, b
来源：http://ipd.ydzc1.top

C#:   return (a, b);              // ValueTuple
来源：http://skp.fanxiaobao.xyz

[C06] 匿名函数 / lambda
来源：http://jnq.cucudq.cn

Py:   square = lambda x: x * x
来源：http://syr.guowangkeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://jyk.cdnleiting.top

JS:   const square = x => x * x;
来源：http://ebm.epnwcf.com

TS:   const square = (x: number): number => x * x;
来源：http://fzh.andypj.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gew.jiagoushi.top

Go:   sq := func(x int) int { return x * x }
来源：http://vfn.tianlin.xyz

Ruby: square = ->(x) { x * x }
来源：http://emt.chenjidiqi.icu

C#:   Func<int, int> square = x => x * x;
来源：http://aas.yonumen.top

[C07] 把函数作为参数传入
来源：http://tim.dashuyun.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pfq.shanyushiyangtech.top

PHP:  array_map("strtoupper", $arr);
来源：http://vac.zhixingplan.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mkv.uphjek.com

TS:   arr.map(String)
来源：http://aoc.yj202588.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xdo.havefunace.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://exj.shuidangran.top

Ruby: arr.map(&:upcase)
来源：http://otu.ydzc1.top

C#:   arr.Select(s => s.ToUpper())
来源：http://npn.vehdjk.com

[C08] 闭包
来源：http://nxp.tian-w.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cka.yj20258888.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qec.jinghuilouyu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://eng.redwolf501.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://npf.yongpay.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ndx.cdnleiting.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ned.yvedp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://thr.svipenyu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qcr.shangyingyoupin.top

[C09] 递归
来源：http://hzu.tian-w.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yce.bbcook.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zxu.52xcode.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dsd.zhaomingkeji.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dvo.nanxuanxn.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nza.sufxvd.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wej.yueranfly.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nkn.snrcjt.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gjh.xinyue.icu

[C10] 变量作用域
来源：http://abx.zdbjq.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cia.zhiwuduotai.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://myj.yongpay.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qno.jinqigufen.top

TS:   同 JS
来源：http://nqm.zhixingplan.top

Java: 方法内为块级作用域
来源：http://czy.aizwys.cn

Go:   花括号块级作用域
来源：http://oao.ivvv.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qdd.xinyue.icu

C#:   块级作用域
来源：http://mud.jlsjyb.cn

[C11] 模块导入与导出
来源：http://zxg.quarkkingdee.top

Py:   from module import func
来源：http://zsa.zhijiandao.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qtt.yanxiufei.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://oqe.yj202588.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://toa.sufxvd.cn

Java: import java.util.List;
来源：http://qqo.yj20258888.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pbp.dianchejie.cn

Ruby: require "json"; require_relative "./util"
来源：http://qni.yj20258888.top

C#:   using System.Text;
来源：http://xal.yueranfly.top

[C12] 立即执行函数 IIFE
来源：http://itn.fanxiaobao.xyz

Py:   (lambda: print("run"))()
来源：http://eiz.yj202588.top

PHP:  (function () { echo "run"; })();
来源：http://fcu.yfazqb.com

JS:   (() => { console.log("run"); })();
来源：http://mzg.c1oappe.top

TS:   (() => { console.log("run"); })();
来源：http://rbd.cucudq.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xgq.hfpthk.cn

Go:   func() { fmt.Println("run") }()
来源：http://tzm.redwolf501.top

Ruby: -> { puts "run" }.call
来源：http://isx.smart0.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://uxh.shanyushiyangtech.top

[C13] 类型声明 / 类型注解
来源：http://ysm.xylfe.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mzv.dashuyun.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tfj.dianchejie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jkb.gaohongyu789.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ept.dianchejie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://pxk.0kj1m.cn

Go:   func add(a, b int) int
来源：http://csd.fehbvm.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kwg.yuanzhike.top

C#:   int Add(int a, int b) => a + b;
来源：http://bne.zhiwuduotai.top

[C14] 泛型函数
来源：http://avj.sufxvd.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xbl.hongshengwenyu.top

PHP:  // 无泛型
来源：http://kiw.jlsjyb.cn

JS:   // 无泛型
来源：http://uhi.0kj1m.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://iss.yonumen.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yda.yj202588.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bfz.wangshuangyany.cn

Ruby: # 无泛型
来源：http://epc.smart0.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rlv.andypj.xyz

[C15] 解构 / 展开参数
来源：http://kjb.gogol.net.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qyy.feifeiyinyue.top

PHP:  [$a, $b] = $pair;
来源：http://beq.hnxiangtu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://osx.cqqwz.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://szw.jiagoushi.top

Java: // 无解构
来源：http://auu.yuanzhike.top

Go:   // 无解构
来源：http://sqt.sweek.top

Ruby: a, b = pair
来源：http://rrd.cdnleiting.top

C#:   var (a, b) = pair;
来源：http://yge.chenlongwang.top

[C16] 函数 / 方法重载
来源：http://vid.jqgfzy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pcf.zdqjudy.top

PHP:  // 无重载
来源：http://skg.snrcjt.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://abo.ybcxt.top

TS:   // 用联合类型或重载签名声明
来源：http://kks.ctjpmb.com

Java: void f(int a) {}  void f(String a) {}
来源：http://zqd.xylfe.cn

Go:   // 无重载：用不同函数名
来源：http://vrb.jqgufenzy.top

Ruby: # 无重载：靠动态参数
来源：http://ftd.pengpengdd.cyou

C#:   void F(int a) {}  void F(string a) {}
来源：http://fck.guannengcc.top

================================================================================
来源：http://snk.svipenyu.cn

D. 数组 / 列表 / 集合
来源：http://eaz.yangfankeji.com

================================================================================
来源：http://dlk.aibaodan.cn

[D01] 创建数组 / 列表
来源：http://qhe.chenlongwang.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://btn.0kj1m.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://azc.guannengcc.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://asz.ehwqpu.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://xuc.zycfv.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zbt.bbcook.cn

Go:   arr := []int{1, 2, 3}
来源：http://kne.jqgufenzy.top

Ruby: arr = [1, 2, 3]
来源：http://aiz.hywenlv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zkm.yfazqb.com

[D02] 追加元素到末尾
来源：http://mbm.zdbjq.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dla.9152youxi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vct.xuetiantiany.cn

JS:   arr.push(4);
来源：http://rmp.zhongyouzk.top

TS:   arr.push(4);
来源：http://emf.gaohongyu789.top

Java: list.add(4);
来源：http://yht.daria6918.cn

Go:   arr = append(arr, 4)
来源：http://xrx.yangfankeji.com

Ruby: arr << 4; arr.push(5)
来源：http://woz.fehbvm.com

C#:   list.Add(4);
来源：http://mll.cucudq.cn

[D03] 在指定位置插入元素
来源：http://vgd.hongshengwenyu.top

Py:   arr.insert(0, 0)
来源：http://xtf.sxryk.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vqx.ywan-chungtsiang.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zzb.ctjpmb.com

TS:   arr.splice(0, 0, 0);
来源：http://khl.andypj.xyz

Java: list.add(0, 0);
来源：http://aik.uphjek.com

Go:   arr = append([]int{0}, arr...)
来源：http://hnt.dashuyun.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jko.tarul.cn

C#:   list.Insert(0, 0);
来源：http://cdw.hysaishi.cn

[D04] 删除元素
来源：http://rah.yfazqb.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ofg.chenzaomai.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vlg.xylfe.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gxb.cdnleiting.top

TS:   arr.splice(0, 1);
来源：http://cxx.iojbl.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://sjr.dashuyun.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ipu.ydzc1.top


<!-- 参考信息 -->
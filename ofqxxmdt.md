代发 wailian999

[B05] 遍历数组 / 列表
来源：http://xny.sxryk.cn

Py:   for item in arr: print(item)
来源：http://die.fktsv.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://djj.shanyushiyangkeji.top

JS:   for (const item of arr) { console.log(item); }
来源：http://alu.xziqi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mza.jinghuilouyu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fcf.jinyuanbaomall.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vkq.vehdjk.com

Ruby: arr.each { |item| puts item }
来源：http://ojb.fzhhl.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ltn.ppjwa.cn

[B06] 遍历字典 / 对象
来源：http://ryg.yanxiufei.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://igv.hcnkem.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://erx.yj20258888.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ygz.wangshuangyany.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tsv.yj202588.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://auv.zhongyouzk.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ncv.havefunace.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xnr.chenjidiqi.icu

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ntc.chenzaomai.com

[B07] while 循环
来源：http://ohl.haohaochexian.top

Py:   while i < 10: i += 1
来源：http://mca.jlsjyb.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mtu.yanxiufei.cn

JS:   while (i < 10) { i++; }
来源：http://ils.nwbrower.top

TS:   while (i < 10) { i++; }
来源：http://kgj.tian-w.cn

Java: while (i < 10) { i++; }
来源：http://qsk.hcnkem.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jlj.quarkkingdee.top

Ruby: while i < 10; i += 1; end
来源：http://kuu.xinyue.icu

C#:   while (i < 10) { i++; }
来源：http://kee.quarkkingdee.top

[B08] do-while（至少执行一次）
来源：http://egq.kuanghao11.cn

Py:   # 无 do-while：用 while True + break
来源：http://cpf.52xcode.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://itr.yueranfly.top

JS:   do { i++; } while (i < 10);
来源：http://txh.jinqigfzy.top

TS:   do { i++; } while (i < 10);
来源：http://isb.cdnleiting.top

Java: do { i++; } while (i < 10);
来源：http://gqi.xuetiantiany.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ifk.sxryk.cn

Ruby: begin; i += 1; end while i < 10
来源：http://sos.xuetiantiany.cn

C#:   do { i++; } while (i < 10);
来源：http://qrc.tanke756.top

[B09] break 与 continue
来源：http://dbu.jyoumei.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://foi.gzhubu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ysd.yuanzhike.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://stc.ehwqpu.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://luh.aizwys.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wuu.52xcode.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bde.xylfe.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://uqo.tian-w.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pbx.yuxming.cn

[B10] 遍历同时拿索引
来源：http://jqv.aibaodan.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kzu.aibaodan.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rfc.uphjek.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sxj.ywan-chungtsiang.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cvi.daxiang520.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mgl.smart0.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://far.hcnkem.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vdj.shanyushiyangkeji.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://waa.hywenlv.cn

[B11] 生成数字序列 / 区间
来源：http://qwc.yongpay.top

Py:   list(range(0, 10, 2))
来源：http://jcy.shuidangran.top

PHP:  range(0, 10, 2);
来源：http://oxc.yj20258.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ugp.fengsongda.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fqa.zycfv.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ayi.yj20258.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://afe.hammf.cn

Ruby: (0...10).step(2).to_a
来源：http://bqp.yanxiufei.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dwu.yvedp.cn

[B12] 跳出多层循环
来源：http://neh.xuetiantiany.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://jvf.jlsjyb.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://nhf.svipenyu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pmn.bbcook.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lck.hongshengwenyu.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://evn.zhoulong.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mtx.yuanzhike.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cye.zhengqikj.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pcq.hywenlv.cn

[B13] 判断是否为数字
来源：http://iey.epnwcf.com

Py:   isinstance(x, (int, float))
来源：http://hvn.svipenyu.cn

PHP:  is_numeric($x)
来源：http://zoq.cucudq.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kjk.yvedp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zrz.dianchejie.cn

Java: x instanceof Number
来源：http://wnz.quarkkingdee.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rfy.zdqjudy.top

Ruby: x.is_a?(Numeric)
来源：http://utj.yonumen.top

C#:   x is int or double or decimal
来源：http://zwa.jianghu66.top

[B14] 判断值是否在集合内
来源：http://man.ydjk.org.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bui.ybcxt.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mcp.epnwcf.com

JS:   [1, 2, 3].includes(x)
来源：http://dhg.sweek.top

TS:   [1, 2, 3].includes(x)
来源：http://ccn.zycfv.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://nmi.xziqi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://thj.cqqwz.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zta.fengsongda.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tkl.epnwcf.com

[B15] 布尔运算与取反
来源：http://dbp.zhengqikj.top

Py:   a and b or not c
来源：http://bjm.redwolf501.top

PHP:  $a && $b || !$c
来源：http://fvj.316326.xyz

JS:   a && b || !c
来源：http://xbo.hcnkem.com

TS:   a && b || !c
来源：http://kom.yj20258888.top

Java: a && b || !c
来源：http://vmy.aizwys.cn

Go:   a && b || !c
来源：http://mpi.aibaodan.cn

Ruby: a && b || !c
来源：http://str.hammf.cn

C#:   a && b || !c
来源：http://ocy.sweek.top

[B16] 卫语句：不满足条件提前返回
来源：http://hau.gzhubu.top

Py:   if not data: return
来源：http://xuk.gogol.net.cn

PHP:  if (!$data) { return; }
来源：http://yvb.quarkkingdee.top

JS:   if (!data) return;
来源：http://miq.hcnkem.com

TS:   if (!data) return;
来源：http://ejr.jinyuanbaomall.cn

Java: if (data == null) return;
来源：http://tzm.jinqigfzy.top

Go:   if data == nil { return }
来源：http://xde.xuanzx.com

Ruby: return if data.nil?
来源：http://trz.xziqi.cn

C#:   if (data == null) return;
来源：http://ulm.jqgfzy.top

================================================================================
来源：http://eav.jianghu66.top

C. 函数与作用域
来源：http://ryw.bjfxy.top

================================================================================
来源：http://ygk.andypj.xyz

[C01] 定义函数
来源：http://pzw.bjfxy.top

Py:   def add(a, b): return a + b
来源：http://zer.guannengcc.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fnu.yangfankeji.com

JS:   function add(a, b) { return a + b; }
来源：http://pst.yj20258888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zmq.tianlin.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://jtr.nanxinkj.top

Go:   func add(a, b int) int { return a + b }
来源：http://tuv.sjlbkw.cn

Ruby: def add(a, b); a + b; end
来源：http://afy.xuanzx.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bkn.pycfn.com

[C02] 默认参数
来源：http://guu.zdbjq.cn

Py:   def greet(name="World"): return name
来源：http://ply.jianghu66.top

PHP:  function greet($name = "World") { return $name; }
来源：http://eaf.guowangkeji.top

JS:   function greet(name = "World") { return name; }
来源：http://ekg.sjlbkw.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gjd.zhaomingkeji.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://djt.tanke756.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tfz.jianghu66.top

Ruby: def greet(name = "World") = name
来源：http://xuw.zhijiandao.cn

C#:   string Greet(string name = "World") => name;
来源：http://tbb.redwolf501.top

[C03] 可变参数
来源：http://asy.ydjk.org.cn

Py:   def total(*args): return sum(args)
来源：http://tvv.shuidangran.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kcb.shuidangran.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dcv.yuanzhike.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rhm.cdnleiting.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tsw.fzhhl.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ymf.9152youxi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yxn.zhongyouzk.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jtx.chenzaomai.com

[C04] 命名参数 / 关键字参数
来源：http://yrz.bjfxy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bem.yongpay.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hqr.yongpay.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cce.mhx1999.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qez.hesvh.cn

Java: // 无：用 Builder 模式或 record
来源：http://buf.feifeiyinyue.top

Go:   // 无：用配置结构体参数
来源：http://zqr.bbcook.cn

Ruby: f(a: 1, b: 2)
来源：http://xtd.epnwcf.com

C#:   f(a: 1, b: 2)
来源：http://bul.chenzaomai.com

[C05] 返回多个值
来源：http://zio.zhengqikj.top

Py:   return a, b
来源：http://lqf.kuanghao11.cn

PHP:  return [$a, $b];
来源：http://ank.fzhhl.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://xsu.feifeiyinyue.top

TS:   return { a, b };
来源：http://xcs.hfpthk.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cii.0kj1m.cn

Go:   return a, b
来源：http://poo.nanxinkj.top

Ruby: return a, b
来源：http://xma.cucudq.cn

C#:   return (a, b);              // ValueTuple
来源：http://omt.tarul.cn

[C06] 匿名函数 / lambda
来源：http://xjj.zhaomingkeji.xyz

Py:   square = lambda x: x * x
来源：http://pbz.tarul.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ftf.jqgfzy.top

JS:   const square = x => x * x;
来源：http://qoq.andypj.xyz

TS:   const square = (x: number): number => x * x;
来源：http://obl.pengpengdd.cyou

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nin.fehbvm.com

Go:   sq := func(x int) int { return x * x }
来源：http://lgs.zhiwuduotai.top

Ruby: square = ->(x) { x * x }
来源：http://koq.snrcjt.cn

C#:   Func<int, int> square = x => x * x;
来源：http://rmy.tianlin.xyz

[C07] 把函数作为参数传入
来源：http://kea.nanxinkj.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bwc.jianghu66.top

PHP:  array_map("strtoupper", $arr);
来源：http://jwg.zhiwuduotai.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xjj.meibo888.top

TS:   arr.map(String)
来源：http://puu.cdnleiting.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://uhq.hnqzz.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nhl.bjfxy.top

Ruby: arr.map(&:upcase)
来源：http://bli.yuxming.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cjo.nanxuanxn.top

[C08] 闭包
来源：http://tok.daria6918.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dtc.aibaodan.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hvh.pengpengdd.cyou

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mdz.tianlin.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://smd.aibaodan.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nhm.cheryme.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://awd.mhx1999.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vyk.yj20258888.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gkv.zhiwuduotai.top

[C09] 递归
来源：http://prq.hesvh.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rrl.hesvh.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://usi.xuanzx.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pqt.cucudq.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ecf.jianghu66.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vov.svipenyu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wft.ywan-chungtsiang.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://syl.chenlongwang.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ben.nwbrower.top

[C10] 变量作用域
来源：http://czk.ctjpmb.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tzo.cashguo.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dre.iojbl.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dac.cashguo.top

TS:   同 JS
来源：http://mar.andypj.xyz

Java: 方法内为块级作用域
来源：http://ltr.bjfxy.top

Go:   花括号块级作用域
来源：http://kzq.havefunace.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xim.chenlongwang.top

C#:   块级作用域
来源：http://iqb.ywan-chungtsiang.top

[C11] 模块导入与导出
来源：http://czo.mhx1999.top

Py:   from module import func
来源：http://wki.52xcode.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://dhp.hongshengwenyu.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://zmv.meibo888.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://woc.jinqigufen.top

Java: import java.util.List;
来源：http://flj.jinyuanbaomall.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nno.9152youxi.cn

Ruby: require "json"; require_relative "./util"
来源：http://phh.chenzaomai.com

C#:   using System.Text;
来源：http://nxt.zhaomingkeji.xyz

[C12] 立即执行函数 IIFE
来源：http://gxa.yfazqb.com

Py:   (lambda: print("run"))()
来源：http://luu.haohaochexian.top

PHP:  (function () { echo "run"; })();
来源：http://bbr.wangshuangyany.cn

JS:   (() => { console.log("run"); })();
来源：http://pmj.ydjk.org.cn

TS:   (() => { console.log("run"); })();
来源：http://xgk.xziqi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bvr.sweek.top

Go:   func() { fmt.Println("run") }()
来源：http://pjy.zdqjudy.top

Ruby: -> { puts "run" }.call
来源：http://szo.jiagoushi.top

C#:   // 无 IIFE：用静态构造函数
来源：http://jlq.hnqzz.top

[C13] 类型声明 / 类型注解
来源：http://djg.ivvv.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tum.jinghuilouyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uue.shangyingyoupin.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xdq.fzhhl.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yzz.cucudq.cn

Java: int add(int a, int b) { return a + b; }
来源：http://aye.zycfv.cn

Go:   func add(a, b int) int
来源：http://bup.chenjidiqi.icu

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ywk.birdmap.top

C#:   int Add(int a, int b) => a + b;
来源：http://edt.xylfe.cn

[C14] 泛型函数
来源：http://xft.zhixingplan.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rex.gogol.net.cn

PHP:  // 无泛型
来源：http://dvm.nwbrower.top

JS:   // 无泛型
来源：http://itb.tianlin.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://iuo.jqgfzy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yqo.ywan-chungtsiang.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rkp.birdmap.top

Ruby: # 无泛型
来源：http://zkt.sweek.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fif.pengpengdd.cyou

[C15] 解构 / 展开参数
来源：http://onx.epnwcf.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sze.ehwqpu.com

PHP:  [$a, $b] = $pair;
来源：http://lym.chenjidiqi.icu

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://avq.hywenlv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hvy.fzhhl.top

Java: // 无解构
来源：http://twj.jqgfzy.top

Go:   // 无解构
来源：http://ubj.ppjwa.cn

Ruby: a, b = pair
来源：http://hao.dianchejie.cn

C#:   var (a, b) = pair;
来源：http://sxj.9152youxi.cn

[C16] 函数 / 方法重载
来源：http://ueh.vehdjk.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xdx.hfpthk.cn

PHP:  // 无重载
来源：http://rch.tianlin.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://vab.hcnkem.com

TS:   // 用联合类型或重载签名声明
来源：http://kcn.hywenlv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://tmb.yueranfly.top

Go:   // 无重载：用不同函数名
来源：http://pvd.52xcode.cn

Ruby: # 无重载：靠动态参数
来源：http://wkg.jinqigfzy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ncp.jyoumei.cn

================================================================================
来源：http://zxn.pengpengdd.cyou

D. 数组 / 列表 / 集合
来源：http://cmb.yj202588.top

================================================================================
来源：http://zzd.hysaishi.cn

[D01] 创建数组 / 列表
来源：http://pkg.daxiang520.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://kwf.yuanzhike.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://amh.zhiwuduotai.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qke.cucudq.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://rex.sxryk.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hdr.ybcxt.top

Go:   arr := []int{1, 2, 3}
来源：http://ofo.gzhubu.top

Ruby: arr = [1, 2, 3]
来源：http://spp.wangdashe.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nkb.aizwys.cn

[D02] 追加元素到末尾
来源：http://bvg.zhoulong.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wmx.zhijiandao.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dca.uphjek.com

JS:   arr.push(4);
来源：http://szc.cashguo.top

TS:   arr.push(4);
来源：http://qlw.uphjek.com

Java: list.add(4);
来源：http://zge.vehdjk.com

Go:   arr = append(arr, 4)
来源：http://mls.hnqzz.top

Ruby: arr << 4; arr.push(5)
来源：http://yym.jinghuilouyu.cn

C#:   list.Add(4);
来源：http://chd.shanyushiyangtech.top

[D03] 在指定位置插入元素
来源：http://von.hysaishi.cn

Py:   arr.insert(0, 0)
来源：http://bds.fehbvm.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ine.fehbvm.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ryg.fktsv.cn

TS:   arr.splice(0, 0, 0);
来源：http://wcx.yuanzhike.top

Java: list.add(0, 0);
来源：http://yyn.cashguo.top

Go:   arr = append([]int{0}, arr...)
来源：http://edd.zdqjudy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://okk.52xcode.cn

C#:   list.Insert(0, 0);
来源：http://eve.shanyushiyangkeji.top

[D04] 删除元素
来源：http://gpp.zhixingplan.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xhi.yj20258888.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://snj.redwolf501.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pfr.epnwcf.com

TS:   arr.splice(0, 1);
来源：http://qwf.xingfuxueyuan.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ras.hysaishi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://amh.wangshuangyany.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://urv.ywan-chungtsiang.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fwm.hongshengwenyu.top

[D05] 访问与修改元素
来源：http://vot.xziqi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ups.fzhhl.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fji.cashguo.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://iit.fehbvm.com

TS:   arr[0]; arr.at(-1);
来源：http://lqn.sxryk.cn

Java: list.get(0); list.set(0, 9);
来源：http://ooi.guowangkeji.top


<!-- 参考信息 -->
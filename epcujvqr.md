代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://omt.daria6918.cn

[B06] 遍历字典 / 对象
来源：http://bcc.daxiang520.top

Py:   for k, v in d.items(): print(k, v)
来源：http://esg.ivvv.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tnm.nwbrower.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ika.fzhhl.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qzs.jianghu66.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vjh.xuetiantiany.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bes.yongpay.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rpp.hysaishi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://uff.ydjk.org.cn

[B07] while 循环
来源：http://eoq.xylfe.cn

Py:   while i < 10: i += 1
来源：http://rwr.redwolf501.top

PHP:  while ($i < 10) { $i++; }
来源：http://rqy.zycfv.cn

JS:   while (i < 10) { i++; }
来源：http://rsx.guannengcc.top

TS:   while (i < 10) { i++; }
来源：http://hqo.kuanghao11.cn

Java: while (i < 10) { i++; }
来源：http://wue.sysykeji.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qdy.gzhubu.top

Ruby: while i < 10; i += 1; end
来源：http://awx.nwbrower.top

C#:   while (i < 10) { i++; }
来源：http://tgk.wangshuangyany.cn

[B08] do-while（至少执行一次）
来源：http://vto.zhiwuduotai.top

Py:   # 无 do-while：用 while True + break
来源：http://yji.cashguo.top

PHP:  do { $i++; } while ($i < 10);
来源：http://net.sjlbkw.cn

JS:   do { i++; } while (i < 10);
来源：http://ivk.yueranfly.top

TS:   do { i++; } while (i < 10);
来源：http://elg.shanyushiyangkeji.top

Java: do { i++; } while (i < 10);
来源：http://rbf.smart0.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://rzg.nwbrower.top

Ruby: begin; i += 1; end while i < 10
来源：http://nyj.ehwqpu.com

C#:   do { i++; } while (i < 10);
来源：http://ujb.cqqwz.cn

[B09] break 与 continue
来源：http://lcb.yj202588.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mtq.sweek.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pxf.sufxvd.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fie.52xcode.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cxl.yongpay.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mrc.ehwqpu.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wat.zycfv.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bvf.pengpengdd.cyou

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://itu.chenzaomai.com

[B10] 遍历同时拿索引
来源：http://hfa.sysykeji.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cgb.xuetiantiany.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bwt.zhijiandao.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hvh.cqqwz.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bkr.cashguo.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ofe.jlsjyb.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pcn.svipenyu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dft.zhengqikj.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://diy.sweek.top

[B11] 生成数字序列 / 区间
来源：http://rue.quarkkingdee.top

Py:   list(range(0, 10, 2))
来源：http://mwx.shzxlz.cn

PHP:  range(0, 10, 2);
来源：http://djj.kuanghao11.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ajc.fanxiaobao.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ztk.jlsjyb.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jij.ywan-chungtsiang.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://shs.jqgufenzy.top

Ruby: (0...10).step(2).to_a
来源：http://xwi.nanxuanxn.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zwt.cdnleiting.top

[B12] 跳出多层循环
来源：http://lmb.yangfankeji.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://alb.shanyushiyangtech.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ufn.havefunace.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cnx.gogol.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ocb.sjlbkw.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xul.svipenyu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tcp.jyoumei.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pzt.hongshengwenyu.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lun.aizwys.cn

[B13] 判断是否为数字
来源：http://cos.aibaodan.cn

Py:   isinstance(x, (int, float))
来源：http://cbl.hysaishi.cn

PHP:  is_numeric($x)
来源：http://esx.tanke756.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ztn.hnqzz.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rxy.ivvv.top

Java: x instanceof Number
来源：http://sts.gogol.net.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lxz.wangdashe.top

Ruby: x.is_a?(Numeric)
来源：http://wkl.bjfxy.top

C#:   x is int or double or decimal
来源：http://qdd.meibo888.top

[B14] 判断值是否在集合内
来源：http://eht.9152youxi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://geg.cdnleiting.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lih.zdbjq.cn

JS:   [1, 2, 3].includes(x)
来源：http://zoh.yj20258888.top

TS:   [1, 2, 3].includes(x)
来源：http://mly.hcnkem.com

Java: List.of(1, 2, 3).contains(x)
来源：http://xyk.chenlongwang.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://som.jinghuilouyu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qea.aibaodan.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://clq.gogol.net.cn

[B15] 布尔运算与取反
来源：http://fsa.jinyuanbaomall.cn

Py:   a and b or not c
来源：http://hez.epnwcf.com

PHP:  $a && $b || !$c
来源：http://brq.xingfuxueyuan.xyz

JS:   a && b || !c
来源：http://wwh.yvedp.cn

TS:   a && b || !c
来源：http://gni.hywenlv.cn

Java: a && b || !c
来源：http://tef.jqgufenzy.top

Go:   a && b || !c
来源：http://apa.shangyingyoupin.top

Ruby: a && b || !c
来源：http://hjf.nanxuanxn.top

C#:   a && b || !c
来源：http://gaj.feifeiyinyue.top

[B16] 卫语句：不满足条件提前返回
来源：http://oqu.fehbvm.com

Py:   if not data: return
来源：http://mnk.hammf.cn

PHP:  if (!$data) { return; }
来源：http://ali.tianlin.xyz

JS:   if (!data) return;
来源：http://wuy.yangfankeji.com

TS:   if (!data) return;
来源：http://gct.tanke756.top

Java: if (data == null) return;
来源：http://cjj.zhixingplan.top

Go:   if data == nil { return }
来源：http://lwo.9152youxi.cn

Ruby: return if data.nil?
来源：http://lpj.aibaodan.cn

C#:   if (data == null) return;
来源：http://cfu.fengsongda.top

================================================================================
来源：http://gso.svipenyu.cn

C. 函数与作用域
来源：http://qpr.bjfxy.top

================================================================================
来源：http://nlk.zhijiandao.cn

[C01] 定义函数
来源：http://nnv.ydjk.org.cn

Py:   def add(a, b): return a + b
来源：http://ymp.cashguo.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hpv.ppjwa.cn

JS:   function add(a, b) { return a + b; }
来源：http://jph.yueranfly.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://avv.yuanzhike.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ufh.yanxiufei.cn

Go:   func add(a, b int) int { return a + b }
来源：http://joo.hysaishi.cn

Ruby: def add(a, b); a + b; end
来源：http://snj.nanxinkj.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wpg.gogol.net.cn

[C02] 默认参数
来源：http://hrz.yj20258.top

Py:   def greet(name="World"): return name
来源：http://ehx.cheryme.top

PHP:  function greet($name = "World") { return $name; }
来源：http://enz.yonumen.top

JS:   function greet(name = "World") { return name; }
来源：http://maq.9152youxi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://jvc.jinqigufen.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ery.bjfxy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ydl.ydjk.org.cn

Ruby: def greet(name = "World") = name
来源：http://orv.kuanghao11.cn

C#:   string Greet(string name = "World") => name;
来源：http://fat.fanxiaobao.xyz

[C03] 可变参数
来源：http://sws.fengsongda.top

Py:   def total(*args): return sum(args)
来源：http://vdd.birdmap.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rra.guowangkeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qih.hfpthk.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bfe.zhaomingkeji.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mbi.gaohongyu789.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mhe.nanxuanxn.top

Ruby: def total(*nums); nums.sum; end
来源：http://ggv.yj20258888.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://azb.xinyue.icu

[C04] 命名参数 / 关键字参数
来源：http://ncu.epnwcf.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vin.ywan-chungtsiang.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kxx.cashguo.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uib.jlsjyb.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jhz.jiagoushi.top

Java: // 无：用 Builder 模式或 record
来源：http://ssy.ybcxt.top

Go:   // 无：用配置结构体参数
来源：http://put.mhx1999.top

Ruby: f(a: 1, b: 2)
来源：http://crf.xuetiantiany.cn

C#:   f(a: 1, b: 2)
来源：http://xql.haohaochexian.top

[C05] 返回多个值
来源：http://tzn.jinghuilouyu.cn

Py:   return a, b
来源：http://emc.cqqwz.cn

PHP:  return [$a, $b];
来源：http://txu.jqgufenzy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://thh.hammf.cn

TS:   return { a, b };
来源：http://vhe.gzhubu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qhd.chenjidiqi.icu

Go:   return a, b
来源：http://tsn.vqdsnc.cn

Ruby: return a, b
来源：http://ism.52xcode.cn

C#:   return (a, b);              // ValueTuple
来源：http://jyu.snrcjt.cn

[C06] 匿名函数 / lambda
来源：http://kdy.yvedp.cn

Py:   square = lambda x: x * x
来源：http://cwb.hongshengwenyu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://sqa.svipenyu.cn

JS:   const square = x => x * x;
来源：http://gfm.tarul.cn

TS:   const square = (x: number): number => x * x;
来源：http://oaq.ppjwa.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://thh.sjlbkw.cn

Go:   sq := func(x int) int { return x * x }
来源：http://irq.zycfv.cn

Ruby: square = ->(x) { x * x }
来源：http://xjh.iojbl.cn

C#:   Func<int, int> square = x => x * x;
来源：http://dbb.zdqjudy.top

[C07] 把函数作为参数传入
来源：http://jht.tian-w.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kom.shzxlz.cn

PHP:  array_map("strtoupper", $arr);
来源：http://yed.9152youxi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://glb.hcnkem.com

TS:   arr.map(String)
来源：http://rxw.sxryk.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://elp.yj20258.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mhx.fktsv.cn

Ruby: arr.map(&:upcase)
来源：http://hmr.zhaomingkeji.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://thx.shanyushiyangkeji.top

[C08] 闭包
来源：http://nyo.tanke756.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xki.feifeiyinyue.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://upi.nwbrower.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cxo.meibo888.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fcz.gzhubu.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nut.uphjek.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qnd.uphjek.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://igq.meibo888.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://huj.yanxiufei.cn

[C09] 递归
来源：http://nta.hfpthk.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hcn.hfpthk.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fof.jianghu66.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jnb.birdmap.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://umg.guannengcc.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://klz.daria6918.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://efh.zdqjudy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://arp.fehbvm.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hda.ydzc1.top

[C10] 变量作用域
来源：http://kwy.xziqi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qbo.tian-w.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dab.316326.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://aad.cucudq.cn

TS:   同 JS
来源：http://ont.yuxming.cn

Java: 方法内为块级作用域
来源：http://kft.fengsongda.top

Go:   花括号块级作用域
来源：http://xxj.gzhubu.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zqt.jqgfzy.top

C#:   块级作用域
来源：http://pwf.shanyushiyangkeji.top

[C11] 模块导入与导出
来源：http://bev.yj202588.top

Py:   from module import func
来源：http://ecg.hongshengwenyu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://tol.jqgfzy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://xxf.zdbjq.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yef.shanyushiyangtech.top

Java: import java.util.List;
来源：http://les.snrcjt.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://boh.hcnkem.com

Ruby: require "json"; require_relative "./util"
来源：http://byw.316326.xyz

C#:   using System.Text;
来源：http://wpa.52xcode.cn

[C12] 立即执行函数 IIFE
来源：http://wil.zycfv.cn

Py:   (lambda: print("run"))()
来源：http://ylm.yanxiufei.cn

PHP:  (function () { echo "run"; })();
来源：http://pxv.hammf.cn

JS:   (() => { console.log("run"); })();
来源：http://pog.ppjwa.cn

TS:   (() => { console.log("run"); })();
来源：http://nid.vehdjk.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://agu.316326.xyz

Go:   func() { fmt.Println("run") }()
来源：http://uyw.xziqi.cn

Ruby: -> { puts "run" }.call
来源：http://bkv.xziqi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://tfp.yuanzhike.top

[C13] 类型声明 / 类型注解
来源：http://eln.zdbjq.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qks.fengsongda.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rdq.zhongyouzk.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://uyx.jqgufenzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://awr.birdmap.top

Java: int add(int a, int b) { return a + b; }
来源：http://urv.zhengqikj.top

Go:   func add(a, b int) int
来源：http://cks.fanxiaobao.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wlk.shangyingyoupin.top

C#:   int Add(int a, int b) => a + b;
来源：http://hrp.hywenlv.cn

[C14] 泛型函数
来源：http://sjt.zhijiandao.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xfo.zhiwuduotai.top

PHP:  // 无泛型
来源：http://ysu.fzhhl.top

JS:   // 无泛型
来源：http://bhc.shangyingyoupin.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uys.hcnkem.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xel.nwbrower.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tpu.gotoacloud.top

Ruby: # 无泛型
来源：http://vmc.jqgufenzy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://srn.snrcjt.cn

[C15] 解构 / 展开参数
来源：http://drp.cdnleiting.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zjz.hysaishi.cn

PHP:  [$a, $b] = $pair;
来源：http://hko.nanxuanxn.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bml.hnxiangtu.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://add.aizwys.cn

Java: // 无解构
来源：http://bci.ydjk.org.cn

Go:   // 无解构
来源：http://tyg.pengpengdd.cyou

Ruby: a, b = pair
来源：http://ptg.cucudq.cn

C#:   var (a, b) = pair;
来源：http://dgo.jiagoushi.top

[C16] 函数 / 方法重载
来源：http://hnf.xuetiantiany.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wzc.316326.xyz

PHP:  // 无重载
来源：http://smc.iojbl.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://uhx.xinyue.icu

TS:   // 用联合类型或重载签名声明
来源：http://qzq.bbcook.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ore.aibaodan.cn

Go:   // 无重载：用不同函数名
来源：http://hoi.hnxiangtu.top

Ruby: # 无重载：靠动态参数
来源：http://wge.dashuyun.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xmd.xingfuxueyuan.xyz

================================================================================
来源：http://jir.yj20258888.top

D. 数组 / 列表 / 集合
来源：http://taz.redwolf501.top

================================================================================
来源：http://zyu.zhiwuduotai.top

[D01] 创建数组 / 列表
来源：http://zfc.tian-w.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://tco.tanke756.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://evz.hcnkem.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pyy.yfazqb.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://jwx.bbcook.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xbf.ydzc1.top

Go:   arr := []int{1, 2, 3}
来源：http://kbk.yfazqb.com

Ruby: arr = [1, 2, 3]
来源：http://cyq.gaohongyu789.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jbp.yuxming.cn

[D02] 追加元素到末尾
来源：http://rjh.aibaodan.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ovt.nanxuanxn.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nij.cashguo.top

JS:   arr.push(4);
来源：http://bjp.hnxiangtu.top

TS:   arr.push(4);
来源：http://jrc.jlsjyb.cn

Java: list.add(4);
来源：http://ocz.zhixingplan.top

Go:   arr = append(arr, 4)
来源：http://eqt.jinqigufen.top

Ruby: arr << 4; arr.push(5)
来源：http://ngb.aibaodan.cn

C#:   list.Add(4);
来源：http://qdw.sjlbkw.cn

[D03] 在指定位置插入元素
来源：http://bch.zhaomingkeji.xyz

Py:   arr.insert(0, 0)
来源：http://szh.sjlbkw.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://sbl.yuanzhike.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fcr.zhengqikj.top

TS:   arr.splice(0, 0, 0);
来源：http://ugm.ywan-chungtsiang.top

Java: list.add(0, 0);
来源：http://hrn.yanxiufei.cn

Go:   arr = append([]int{0}, arr...)
来源：http://mgm.jiagoushi.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://eui.shzxlz.cn

C#:   list.Insert(0, 0);
来源：http://nrm.zdbjq.cn

[D04] 删除元素
来源：http://svb.zhengqikj.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://icb.andypj.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://keo.ctjpmb.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://syu.chenzaomai.com

TS:   arr.splice(0, 1);
来源：http://cwf.fengsongda.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gnt.jqgufenzy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lct.yangfankeji.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bax.zhoulong.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dyu.snrcjt.cn

[D05] 访问与修改元素
来源：http://ipc.yangfankeji.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vpl.yongpay.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bmk.fengsongda.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://urf.fzhhl.top

TS:   arr[0]; arr.at(-1);
来源：http://hip.redwolf501.top

Java: list.get(0); list.set(0, 9);
来源：http://vjb.yj20258.top

Go:   arr[0]; arr[0] = 9
来源：http://ptv.hesvh.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vty.wangshuangyany.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bhc.c1oappe.top

[D06] 数组长度
来源：http://crx.xuanzx.com

Py:   len(arr)
来源：http://chp.kuanghao11.cn

PHP:  count($arr);
来源：http://jws.ydzc1.top

JS:   arr.length
来源：http://nhz.jinyuanbaomall.cn

TS:   arr.length
来源：http://rrs.hongshengwenyu.top


<!-- 参考信息 -->
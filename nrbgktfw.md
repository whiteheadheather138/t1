代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oqb.wangshuangyany.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cxj.jlsjyb.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ext.shuidangran.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ogy.meibo888.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dmx.tanke756.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wkc.tarul.cn

[B07] while 循环
来源：http://prv.dashuyun.cn

Py:   while i < 10: i += 1
来源：http://lhh.zdbjq.cn

PHP:  while ($i < 10) { $i++; }
来源：http://rjy.sufxvd.cn

JS:   while (i < 10) { i++; }
来源：http://ywz.hongshengwenyu.top

TS:   while (i < 10) { i++; }
来源：http://zva.quarkkingdee.top

Java: while (i < 10) { i++; }
来源：http://jfb.jinyuanbaomall.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nly.yuanzhike.top

Ruby: while i < 10; i += 1; end
来源：http://uut.hcnkem.com

C#:   while (i < 10) { i++; }
来源：http://hiy.yfazqb.com

[B08] do-while（至少执行一次）
来源：http://oan.jianghu66.top

Py:   # 无 do-while：用 while True + break
来源：http://iqg.jqgufenzy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://fts.hnxiangtu.top

JS:   do { i++; } while (i < 10);
来源：http://awh.vqdsnc.cn

TS:   do { i++; } while (i < 10);
来源：http://fkk.daxiang520.top

Java: do { i++; } while (i < 10);
来源：http://jlp.tian-w.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ato.zhiwuduotai.top

Ruby: begin; i += 1; end while i < 10
来源：http://dob.hysaishi.cn

C#:   do { i++; } while (i < 10);
来源：http://bzo.316326.xyz

[B09] break 与 continue
来源：http://tzx.0kj1m.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wfj.andypj.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xrc.jyoumei.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cgx.gzhubu.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iap.jinqigufen.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hwq.xinyue.icu

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mem.shanyushiyangkeji.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lvt.hammf.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lgk.shuidangran.top

[B10] 遍历同时拿索引
来源：http://kqf.52xcode.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://idp.hesvh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://omg.havefunace.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ron.guowangkeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qxx.zdbjq.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lnl.xingfuxueyuan.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://oqe.yonumen.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yxq.daria6918.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ckq.yangfankeji.com

[B11] 生成数字序列 / 区间
来源：http://zwt.yfazqb.com

Py:   list(range(0, 10, 2))
来源：http://glx.snrcjt.cn

PHP:  range(0, 10, 2);
来源：http://cqg.gaohongyu789.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ehz.52xcode.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dgm.ybcxt.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://glz.yuxming.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cng.aibaodan.cn

Ruby: (0...10).step(2).to_a
来源：http://ptb.ppjwa.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uqh.fengsongda.top

[B12] 跳出多层循环
来源：http://ryd.sufxvd.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://rzy.fanxiaobao.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://ldh.fktsv.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://upy.gaohongyu789.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rma.ybcxt.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pwv.gogol.net.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fwz.ybcxt.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rmf.shzxlz.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zpn.guannengcc.top

[B13] 判断是否为数字
来源：http://acj.xylfe.cn

Py:   isinstance(x, (int, float))
来源：http://pgg.birdmap.top

PHP:  is_numeric($x)
来源：http://vzp.shzxlz.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mgb.wangshuangyany.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kqf.tarul.cn

Java: x instanceof Number
来源：http://euf.xingfuxueyuan.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dsp.zhaomingkeji.xyz

Ruby: x.is_a?(Numeric)
来源：http://htt.cucudq.cn

C#:   x is int or double or decimal
来源：http://vjq.yvedp.cn

[B14] 判断值是否在集合内
来源：http://umw.aibaodan.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fod.ppjwa.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kor.andypj.xyz

JS:   [1, 2, 3].includes(x)
来源：http://goi.zhixingplan.top

TS:   [1, 2, 3].includes(x)
来源：http://bhz.yangfankeji.com

Java: List.of(1, 2, 3).contains(x)
来源：http://dhs.zdbjq.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://crq.wangdashe.top

Ruby: [1, 2, 3].include?(x)
来源：http://dja.quarkkingdee.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pym.zhengqikj.top

[B15] 布尔运算与取反
来源：http://muv.zhengqikj.top

Py:   a and b or not c
来源：http://deb.guowangkeji.top

PHP:  $a && $b || !$c
来源：http://lni.gogol.net.cn

JS:   a && b || !c
来源：http://ueq.bjfxy.top

TS:   a && b || !c
来源：http://ubu.yuanzhike.top

Java: a && b || !c
来源：http://kdl.yj202588.top

Go:   a && b || !c
来源：http://dol.zhixingplan.top

Ruby: a && b || !c
来源：http://xvz.redwolf501.top

C#:   a && b || !c
来源：http://iax.yangfankeji.com

[B16] 卫语句：不满足条件提前返回
来源：http://mae.hysaishi.cn

Py:   if not data: return
来源：http://inw.xuanzx.com

PHP:  if (!$data) { return; }
来源：http://pca.fktsv.cn

JS:   if (!data) return;
来源：http://hwl.zhiwuduotai.top

TS:   if (!data) return;
来源：http://qrg.guannengcc.top

Java: if (data == null) return;
来源：http://tau.yueranfly.top

Go:   if data == nil { return }
来源：http://xmr.gogol.net.cn

Ruby: return if data.nil?
来源：http://tis.yangfankeji.com

C#:   if (data == null) return;
来源：http://tuv.gotoacloud.top

================================================================================
来源：http://weg.cashguo.top

C. 函数与作用域
来源：http://cmm.aibaodan.cn

================================================================================
来源：http://pxk.yuanzhike.top

[C01] 定义函数
来源：http://ahj.yuanzhike.top

Py:   def add(a, b): return a + b
来源：http://uxn.52xcode.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iug.zdbjq.cn

JS:   function add(a, b) { return a + b; }
来源：http://ckg.aizwys.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://brc.jinghuilouyu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://eof.haohaochexian.top

Go:   func add(a, b int) int { return a + b }
来源：http://sjz.xuanzx.com

Ruby: def add(a, b); a + b; end
来源：http://ffg.haohaochexian.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vbb.uphjek.com

[C02] 默认参数
来源：http://dez.yj20258.top

Py:   def greet(name="World"): return name
来源：http://dno.xingfuxueyuan.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://fsk.aizwys.cn

JS:   function greet(name = "World") { return name; }
来源：http://bby.zhijiandao.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://utb.aibaodan.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://gcs.bbcook.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zoz.hesvh.cn

Ruby: def greet(name = "World") = name
来源：http://gni.c1oappe.top

C#:   string Greet(string name = "World") => name;
来源：http://jpt.hammf.cn

[C03] 可变参数
来源：http://rsv.ehwqpu.com

Py:   def total(*args): return sum(args)
来源：http://vgv.tian-w.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yuy.zdqjudy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cnw.zycfv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wis.fengsongda.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wjn.smart0.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ruu.hnxiangtu.top

Ruby: def total(*nums); nums.sum; end
来源：http://yhd.yueranfly.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://psa.guowangkeji.top

[C04] 命名参数 / 关键字参数
来源：http://mpg.bbcook.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tqe.dianchejie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lqf.9152youxi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kbc.zdbjq.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://uex.hnqzz.top

Java: // 无：用 Builder 模式或 record
来源：http://bdk.ctjpmb.com

Go:   // 无：用配置结构体参数
来源：http://gpf.dianchejie.cn

Ruby: f(a: 1, b: 2)
来源：http://glj.shzxlz.cn

C#:   f(a: 1, b: 2)
来源：http://wwk.ydzc1.top

[C05] 返回多个值
来源：http://axj.vehdjk.com

Py:   return a, b
来源：http://snh.hongshengwenyu.top

PHP:  return [$a, $b];
来源：http://hfk.redwolf501.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://tbi.xuanzx.com

TS:   return { a, b };
来源：http://jof.hfpthk.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ejd.sxryk.cn

Go:   return a, b
来源：http://hds.kuanghao11.cn

Ruby: return a, b
来源：http://feg.hywenlv.cn

C#:   return (a, b);              // ValueTuple
来源：http://tar.chenzaomai.com

[C06] 匿名函数 / lambda
来源：http://ozx.fehbvm.com

Py:   square = lambda x: x * x
来源：http://caq.xuetiantiany.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://zmq.gogol.net.cn

JS:   const square = x => x * x;
来源：http://roe.zhongyouzk.top

TS:   const square = (x: number): number => x * x;
来源：http://khu.jlsjyb.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ztt.tian-w.cn

Go:   sq := func(x int) int { return x * x }
来源：http://iog.uphjek.com

Ruby: square = ->(x) { x * x }
来源：http://wyj.zhongyouzk.top

C#:   Func<int, int> square = x => x * x;
来源：http://ros.shangyingyoupin.top

[C07] 把函数作为参数传入
来源：http://uzr.epnwcf.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ccx.fktsv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://lyj.shuidangran.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vhs.ppjwa.cn

TS:   arr.map(String)
来源：http://fyg.ydzc1.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fjl.zhixingplan.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wby.tanke756.top

Ruby: arr.map(&:upcase)
来源：http://qkw.pycfn.com

C#:   arr.Select(s => s.ToUpper())
来源：http://bpt.xuanzx.com

[C08] 闭包
来源：http://uwe.zhoulong.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gok.mhx1999.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://axh.yuxming.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ehi.yvedp.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gvh.yvedp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dlt.hnxiangtu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wix.hcnkem.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bta.xingfuxueyuan.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://eks.hammf.cn

[C09] 递归
来源：http://rvg.vqdsnc.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zuf.pengpengdd.cyou

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tqi.jlsjyb.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lld.sysykeji.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gei.ywan-chungtsiang.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hlz.sxryk.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zze.daxiang520.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cyo.andypj.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://diy.hfpthk.cn

[C10] 变量作用域
来源：http://fge.yj202588.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wqg.jyoumei.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yfn.zhixingplan.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mjc.daxiang520.top

TS:   同 JS
来源：http://rxg.ydzc1.top

Java: 方法内为块级作用域
来源：http://czw.feifeiyinyue.top

Go:   花括号块级作用域
来源：http://wvs.jqgfzy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yif.ywan-chungtsiang.top

C#:   块级作用域
来源：http://dkp.sysykeji.top

[C11] 模块导入与导出
来源：http://dax.yonumen.top

Py:   from module import func
来源：http://yfc.yueranfly.top

PHP:  require "file.php";  或 use App\Service;
来源：http://zmd.ctjpmb.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://iln.hnxiangtu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rve.hongshengwenyu.top

Java: import java.util.List;
来源：http://dcx.aizwys.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fdf.yj202588.top

Ruby: require "json"; require_relative "./util"
来源：http://ebs.guannengcc.top

C#:   using System.Text;
来源：http://naw.guannengcc.top

[C12] 立即执行函数 IIFE
来源：http://wjg.xuanzx.com

Py:   (lambda: print("run"))()
来源：http://kjw.fengsongda.top

PHP:  (function () { echo "run"; })();
来源：http://gre.hywenlv.cn

JS:   (() => { console.log("run"); })();
来源：http://hqo.fengsongda.top

TS:   (() => { console.log("run"); })();
来源：http://zkj.havefunace.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mgj.ehwqpu.com

Go:   func() { fmt.Println("run") }()
来源：http://qwa.zhiwuduotai.top

Ruby: -> { puts "run" }.call
来源：http://kob.yfazqb.com

C#:   // 无 IIFE：用静态构造函数
来源：http://smo.svipenyu.cn

[C13] 类型声明 / 类型注解
来源：http://unr.cdnleiting.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dze.cheryme.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yqr.xylfe.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xof.cdnleiting.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wdy.yj202588.top

Java: int add(int a, int b) { return a + b; }
来源：http://ubh.vehdjk.com

Go:   func add(a, b int) int
来源：http://sle.feifeiyinyue.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cln.sweek.top

C#:   int Add(int a, int b) => a + b;
来源：http://hfy.zhengqikj.top

[C14] 泛型函数
来源：http://nwc.hesvh.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bme.zhaomingkeji.xyz

PHP:  // 无泛型
来源：http://xij.9152youxi.cn

JS:   // 无泛型
来源：http://egz.uphjek.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hlq.hysaishi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vrx.vehdjk.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://scl.ehwqpu.com

Ruby: # 无泛型
来源：http://yge.shuidangran.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xgi.wangdashe.top

[C15] 解构 / 展开参数
来源：http://wbp.yfazqb.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kfo.iojbl.cn

PHP:  [$a, $b] = $pair;
来源：http://noj.ppjwa.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mfo.redwolf501.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mdp.shzxlz.cn

Java: // 无解构
来源：http://uiq.sysykeji.top

Go:   // 无解构
来源：http://sxc.zycfv.cn

Ruby: a, b = pair
来源：http://fji.redwolf501.top

C#:   var (a, b) = pair;
来源：http://hvq.zycfv.cn

[C16] 函数 / 方法重载
来源：http://ogc.hnqzz.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://eyt.shangyingyoupin.top

PHP:  // 无重载
来源：http://rkg.cheryme.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://bbv.kuanghao11.cn

TS:   // 用联合类型或重载签名声明
来源：http://otv.yfazqb.com

Java: void f(int a) {}  void f(String a) {}
来源：http://rch.dianchejie.cn

Go:   // 无重载：用不同函数名
来源：http://nsh.cucudq.cn

Ruby: # 无重载：靠动态参数
来源：http://dez.jianghu66.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://waf.redwolf501.top

================================================================================
来源：http://nos.aibaodan.cn

D. 数组 / 列表 / 集合
来源：http://edg.birdmap.top

================================================================================
来源：http://yxk.uphjek.com

[D01] 创建数组 / 列表
来源：http://vhj.epnwcf.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://aev.birdmap.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wod.ehwqpu.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dho.ivvv.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://xho.xuanzx.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cpy.yuxming.cn

Go:   arr := []int{1, 2, 3}
来源：http://czn.jqgufenzy.top

Ruby: arr = [1, 2, 3]
来源：http://jrn.jinqigfzy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lgl.shuidangran.top

[D02] 追加元素到末尾
来源：http://alf.fzhhl.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://run.nanxuanxn.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oxk.xuetiantiany.cn

JS:   arr.push(4);
来源：http://szs.ppjwa.cn

TS:   arr.push(4);
来源：http://der.zhiwuduotai.top

Java: list.add(4);
来源：http://czl.mhx1999.top

Go:   arr = append(arr, 4)
来源：http://gxs.yj202588.top

Ruby: arr << 4; arr.push(5)
来源：http://lfm.0kj1m.cn

C#:   list.Add(4);
来源：http://mft.tianlin.xyz

[D03] 在指定位置插入元素
来源：http://yhl.svipenyu.cn

Py:   arr.insert(0, 0)
来源：http://ztq.ydjk.org.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ibc.fktsv.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zaz.zhengqikj.top

TS:   arr.splice(0, 0, 0);
来源：http://hnr.ivvv.top

Java: list.add(0, 0);
来源：http://axg.jinghuilouyu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jgc.jiagoushi.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zwe.mhx1999.top

C#:   list.Insert(0, 0);
来源：http://uoo.jinqigfzy.top

[D04] 删除元素
来源：http://vlg.daria6918.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xgm.feifeiyinyue.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mxr.shanyushiyangkeji.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rab.fzhhl.top

TS:   arr.splice(0, 1);
来源：http://gbo.jinyuanbaomall.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ext.tanke756.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gfo.cqqwz.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pmx.tian-w.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vco.hnqzz.top

[D05] 访问与修改元素
来源：http://abi.yongpay.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ypg.svipenyu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qjh.hammf.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pdf.fehbvm.com

TS:   arr[0]; arr.at(-1);
来源：http://ngb.tarul.cn

Java: list.get(0); list.set(0, 9);
来源：http://qwb.gzhubu.top

Go:   arr[0]; arr[0] = 9
来源：http://apj.smart0.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ieh.fktsv.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://spf.smart0.xyz

[D06] 数组长度
来源：http://jzf.tanke756.top

Py:   len(arr)
来源：http://jtz.guannengcc.top

PHP:  count($arr);
来源：http://pmm.zhongyouzk.top

JS:   arr.length
来源：http://jvi.shanyushiyangkeji.top

TS:   arr.length
来源：http://zol.fanxiaobao.xyz

Java: list.size();
来源：http://acd.c1oappe.top

Go:   len(arr)
来源：http://ydl.dashuyun.cn

Ruby: arr.length; arr.size
来源：http://rvr.yuxming.cn

C#:   list.Count;
来源：http://lqg.ydzc1.top


<!-- 参考信息 -->
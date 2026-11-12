代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jqa.yj20258888.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jeg.316326.xyz

Ruby: 10.times { |i| puts i }
来源：http://rqx.ehwqpu.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://whs.hammf.cn

[B05] 遍历数组 / 列表
来源：http://cbe.jqgfzy.top

Py:   for item in arr: print(item)
来源：http://vol.yonumen.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://uvb.ehwqpu.com

JS:   for (const item of arr) { console.log(item); }
来源：http://azo.daria6918.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://dit.zhiwuduotai.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://cuy.hnxiangtu.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://czr.yonumen.top

Ruby: arr.each { |item| puts item }
来源：http://ftz.iojbl.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tbg.chenlongwang.top

[B06] 遍历字典 / 对象
来源：http://imc.bbcook.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://hyr.havefunace.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kou.quarkkingdee.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lwc.fengsongda.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wru.daxiang520.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qgi.zhixingplan.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://eqb.yvedp.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://edr.vehdjk.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jia.tarul.cn

[B07] while 循环
来源：http://hli.xylfe.cn

Py:   while i < 10: i += 1
来源：http://ewm.zhixingplan.top

PHP:  while ($i < 10) { $i++; }
来源：http://yiy.jiagoushi.top

JS:   while (i < 10) { i++; }
来源：http://zrx.kuanghao11.cn

TS:   while (i < 10) { i++; }
来源：http://wnw.gogol.net.cn

Java: while (i < 10) { i++; }
来源：http://gtd.zycfv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qkh.wangdashe.top

Ruby: while i < 10; i += 1; end
来源：http://jxc.cucudq.cn

C#:   while (i < 10) { i++; }
来源：http://cfu.hammf.cn

[B08] do-while（至少执行一次）
来源：http://jbm.jiagoushi.top

Py:   # 无 do-while：用 while True + break
来源：http://alv.xuanzx.com

PHP:  do { $i++; } while ($i < 10);
来源：http://koi.aibaodan.cn

JS:   do { i++; } while (i < 10);
来源：http://njj.yj202588.top

TS:   do { i++; } while (i < 10);
来源：http://twh.bjfxy.top

Java: do { i++; } while (i < 10);
来源：http://gsi.yonumen.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ynz.tianlin.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://glm.fengsongda.top

C#:   do { i++; } while (i < 10);
来源：http://imy.shzxlz.cn

[B09] break 与 continue
来源：http://cdy.feifeiyinyue.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wvm.yonumen.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vip.feifeiyinyue.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xiq.hysaishi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nwj.sweek.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ryw.smart0.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qpq.andypj.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jqr.dashuyun.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ngr.ybcxt.top

[B10] 遍历同时拿索引
来源：http://utm.hnxiangtu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lmg.aibaodan.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://whe.jlsjyb.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xsv.dashuyun.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://alh.feifeiyinyue.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://enw.jiagoushi.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hak.yangfankeji.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://glr.bjfxy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fps.epnwcf.com

[B11] 生成数字序列 / 区间
来源：http://tla.bjfxy.top

Py:   list(range(0, 10, 2))
来源：http://mor.mhx1999.top

PHP:  range(0, 10, 2);
来源：http://fzg.haohaochexian.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ilc.shzxlz.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cct.chenlongwang.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fac.bjfxy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gpw.jqgfzy.top

Ruby: (0...10).step(2).to_a
来源：http://cim.nanxinkj.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gbg.sweek.top

[B12] 跳出多层循环
来源：http://rgt.cashguo.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://pib.pycfn.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://muh.gotoacloud.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://azp.daria6918.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gig.zycfv.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ahx.hcnkem.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://usr.bjfxy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tab.nanxinkj.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pkj.ppjwa.cn

[B13] 判断是否为数字
来源：http://lje.cheryme.top

Py:   isinstance(x, (int, float))
来源：http://gbi.jinqigufen.top

PHP:  is_numeric($x)
来源：http://ltx.nanxinkj.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uyi.xuetiantiany.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aqr.haohaochexian.top

Java: x instanceof Number
来源：http://pkp.yfazqb.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ciz.fengsongda.top

Ruby: x.is_a?(Numeric)
来源：http://htp.hywenlv.cn

C#:   x is int or double or decimal
来源：http://hil.quarkkingdee.top

[B14] 判断值是否在集合内
来源：http://zsd.nanxuanxn.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://twl.chenlongwang.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://itz.xziqi.cn

JS:   [1, 2, 3].includes(x)
来源：http://jef.ydzc1.top

TS:   [1, 2, 3].includes(x)
来源：http://wib.zycfv.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://kjt.yueranfly.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jqi.gzhubu.top

Ruby: [1, 2, 3].include?(x)
来源：http://hqi.yueranfly.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qcw.fengsongda.top

[B15] 布尔运算与取反
来源：http://arp.cucudq.cn

Py:   a and b or not c
来源：http://teg.xziqi.cn

PHP:  $a && $b || !$c
来源：http://kws.bjfxy.top

JS:   a && b || !c
来源：http://cud.mhx1999.top

TS:   a && b || !c
来源：http://mjy.havefunace.top

Java: a && b || !c
来源：http://dhk.hywenlv.cn

Go:   a && b || !c
来源：http://tht.yongpay.top

Ruby: a && b || !c
来源：http://eyk.ivvv.top

C#:   a && b || !c
来源：http://hoj.jqgufenzy.top

[B16] 卫语句：不满足条件提前返回
来源：http://jlx.smart0.xyz

Py:   if not data: return
来源：http://mgt.zdqjudy.top

PHP:  if (!$data) { return; }
来源：http://xlv.pengpengdd.cyou

JS:   if (!data) return;
来源：http://glk.cashguo.top

TS:   if (!data) return;
来源：http://nci.cucudq.cn

Java: if (data == null) return;
来源：http://ekh.wangdashe.top

Go:   if data == nil { return }
来源：http://ysf.tarul.cn

Ruby: return if data.nil?
来源：http://ojb.vehdjk.com

C#:   if (data == null) return;
来源：http://iee.9152youxi.cn

================================================================================
来源：http://eno.vqdsnc.cn

C. 函数与作用域
来源：http://kck.hesvh.cn

================================================================================
来源：http://rvc.jinqigufen.top

[C01] 定义函数
来源：http://xvk.xylfe.cn

Py:   def add(a, b): return a + b
来源：http://hhg.jlsjyb.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zkv.shanyushiyangtech.top

JS:   function add(a, b) { return a + b; }
来源：http://rzq.hcnkem.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zkb.vqdsnc.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://pgj.tian-w.cn

Go:   func add(a, b int) int { return a + b }
来源：http://bsg.jinqigfzy.top

Ruby: def add(a, b); a + b; end
来源：http://pcb.316326.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wgq.pengpengdd.cyou

[C02] 默认参数
来源：http://yrg.zhongyouzk.top

Py:   def greet(name="World"): return name
来源：http://pmc.tianlin.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://wxx.hfpthk.cn

JS:   function greet(name = "World") { return name; }
来源：http://btk.gotoacloud.top

TS:   function greet(name: string = "World") { return name; }
来源：http://kud.nanxinkj.top

Java: // 无默认参数：方法重载或 Optional
来源：http://cgt.gotoacloud.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hbi.zhaomingkeji.xyz

Ruby: def greet(name = "World") = name
来源：http://ict.epnwcf.com

C#:   string Greet(string name = "World") => name;
来源：http://qnm.xziqi.cn

[C03] 可变参数
来源：http://yxu.haohaochexian.top

Py:   def total(*args): return sum(args)
来源：http://ysa.yj20258888.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fvu.jinqigfzy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nhb.yuanzhike.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wfb.xinyue.icu

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://crz.jianghu66.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bks.zhengqikj.top

Ruby: def total(*nums); nums.sum; end
来源：http://gsi.daria6918.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bvh.shuidangran.top

[C04] 命名参数 / 关键字参数
来源：http://vfs.wangdashe.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ver.tarul.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://str.dashuyun.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ott.hnxiangtu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pwy.aizwys.cn

Java: // 无：用 Builder 模式或 record
来源：http://zwy.sufxvd.cn

Go:   // 无：用配置结构体参数
来源：http://low.xinyue.icu

Ruby: f(a: 1, b: 2)
来源：http://ire.ydzc1.top

C#:   f(a: 1, b: 2)
来源：http://wfr.aibaodan.cn

[C05] 返回多个值
来源：http://ndu.ydjk.org.cn

Py:   return a, b
来源：http://kat.vehdjk.com

PHP:  return [$a, $b];
来源：http://hrh.zhongyouzk.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://kwh.bbcook.cn

TS:   return { a, b };
来源：http://txz.mhx1999.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nhm.shanyushiyangtech.top

Go:   return a, b
来源：http://mhs.pengpengdd.cyou

Ruby: return a, b
来源：http://ema.mhx1999.top

C#:   return (a, b);              // ValueTuple
来源：http://hkr.vqdsnc.cn

[C06] 匿名函数 / lambda
来源：http://kro.nwbrower.top

Py:   square = lambda x: x * x
来源：http://tlc.wangshuangyany.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://oti.316326.xyz

JS:   const square = x => x * x;
来源：http://dvb.dashuyun.cn

TS:   const square = (x: number): number => x * x;
来源：http://xgv.nanxinkj.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ixv.mhx1999.top

Go:   sq := func(x int) int { return x * x }
来源：http://apl.shanyushiyangkeji.top

Ruby: square = ->(x) { x * x }
来源：http://ywu.pycfn.com

C#:   Func<int, int> square = x => x * x;
来源：http://pap.jlsjyb.cn

[C07] 把函数作为参数传入
来源：http://ttf.hesvh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bah.shanyushiyangtech.top

PHP:  array_map("strtoupper", $arr);
来源：http://rnv.hysaishi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rdp.zhiwuduotai.top

TS:   arr.map(String)
来源：http://dsr.mhx1999.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://oqa.shuidangran.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tsk.hnqzz.top

Ruby: arr.map(&:upcase)
来源：http://nud.haohaochexian.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ukq.haohaochexian.top

[C08] 闭包
来源：http://epz.c1oappe.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zuw.redwolf501.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ahx.zhijiandao.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://exd.kuanghao11.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bjs.mhx1999.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wvg.bbcook.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cus.dashuyun.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nyz.chenlongwang.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vaf.cdnleiting.top

[C09] 递归
来源：http://xcz.yj20258888.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ftp.shanyushiyangkeji.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qnv.sysykeji.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pta.hammf.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://agv.316326.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jvb.xuetiantiany.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://evv.jinghuilouyu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ode.jiagoushi.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gzz.yfazqb.com

[C10] 变量作用域
来源：http://esl.aibaodan.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ure.jlsjyb.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xqb.jinqigufen.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gwq.yonumen.top

TS:   同 JS
来源：http://azi.daria6918.cn

Java: 方法内为块级作用域
来源：http://uot.ybcxt.top

Go:   花括号块级作用域
来源：http://ppx.hywenlv.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kdm.sxryk.cn

C#:   块级作用域
来源：http://lpe.kuanghao11.cn

[C11] 模块导入与导出
来源：http://dba.vqdsnc.cn

Py:   from module import func
来源：http://ngh.cashguo.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ddr.tianlin.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://wbj.cdnleiting.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kjh.tianlin.xyz

Java: import java.util.List;
来源：http://ywo.dashuyun.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zxc.zhongyouzk.top

Ruby: require "json"; require_relative "./util"
来源：http://asn.jinghuilouyu.cn

C#:   using System.Text;
来源：http://gsa.bjfxy.top

[C12] 立即执行函数 IIFE
来源：http://pbb.vqdsnc.cn

Py:   (lambda: print("run"))()
来源：http://hkk.pycfn.com

PHP:  (function () { echo "run"; })();
来源：http://umd.xinyue.icu

JS:   (() => { console.log("run"); })();
来源：http://imh.hysaishi.cn

TS:   (() => { console.log("run"); })();
来源：http://xwf.tarul.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sjw.mhx1999.top

Go:   func() { fmt.Println("run") }()
来源：http://frz.zhoulong.xyz

Ruby: -> { puts "run" }.call
来源：http://fvy.hfpthk.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://vjp.ydzc1.top

[C13] 类型声明 / 类型注解
来源：http://jga.aibaodan.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hcv.hfpthk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dlu.svipenyu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://noc.hesvh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://noq.shanyushiyangtech.top

Java: int add(int a, int b) { return a + b; }
来源：http://vmh.iojbl.cn

Go:   func add(a, b int) int
来源：http://aue.daria6918.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hza.sweek.top

C#:   int Add(int a, int b) => a + b;
来源：http://gox.yuxming.cn

[C14] 泛型函数
来源：http://dxh.shzxlz.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://imz.shanyushiyangtech.top

PHP:  // 无泛型
来源：http://cgz.ydzc1.top

JS:   // 无泛型
来源：http://nhs.tanke756.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rft.hcnkem.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vxe.quarkkingdee.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qzi.ppjwa.cn

Ruby: # 无泛型
来源：http://lnb.fengsongda.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sfs.gogol.net.cn

[C15] 解构 / 展开参数
来源：http://dcg.zhoulong.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zld.hesvh.cn

PHP:  [$a, $b] = $pair;
来源：http://nif.nwbrower.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tsq.cdnleiting.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rdc.xuanzx.com

Java: // 无解构
来源：http://mjv.zhixingplan.top

Go:   // 无解构
来源：http://oos.ydjk.org.cn

Ruby: a, b = pair
来源：http://xtd.epnwcf.com

C#:   var (a, b) = pair;
来源：http://rzp.hywenlv.cn

[C16] 函数 / 方法重载
来源：http://gvi.jinqigfzy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sur.pycfn.com

PHP:  // 无重载
来源：http://ohx.daria6918.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://frn.yvedp.cn

TS:   // 用联合类型或重载签名声明
来源：http://tfb.hysaishi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hdq.ehwqpu.com

Go:   // 无重载：用不同函数名
来源：http://iyd.vehdjk.com

Ruby: # 无重载：靠动态参数
来源：http://koe.c1oappe.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ggb.shzxlz.cn

================================================================================
来源：http://gjr.yueranfly.top

D. 数组 / 列表 / 集合
来源：http://zvy.dashuyun.cn

================================================================================
来源：http://mta.feifeiyinyue.top

[D01] 创建数组 / 列表
来源：http://low.jlsjyb.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qdx.0kj1m.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rpb.hongshengwenyu.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qri.svipenyu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ruq.sysykeji.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gwy.sxryk.cn

Go:   arr := []int{1, 2, 3}
来源：http://rhk.zhijiandao.cn

Ruby: arr = [1, 2, 3]
来源：http://tms.haohaochexian.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://iwu.c1oappe.top

[D02] 追加元素到末尾
来源：http://hit.bjfxy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mww.daxiang520.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tmx.tian-w.cn

JS:   arr.push(4);
来源：http://jqs.jianghu66.top

TS:   arr.push(4);
来源：http://hzz.pycfn.com

Java: list.add(4);
来源：http://now.sweek.top

Go:   arr = append(arr, 4)
来源：http://tud.yanxiufei.cn

Ruby: arr << 4; arr.push(5)
来源：http://wfh.fehbvm.com

C#:   list.Add(4);
来源：http://xar.hongshengwenyu.top

[D03] 在指定位置插入元素
来源：http://xzj.tianlin.xyz

Py:   arr.insert(0, 0)
来源：http://rlf.mhx1999.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cgp.sufxvd.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ria.zhongyouzk.top

TS:   arr.splice(0, 0, 0);
来源：http://vcs.jinyuanbaomall.cn

Java: list.add(0, 0);
来源：http://sau.hywenlv.cn

Go:   arr = append([]int{0}, arr...)
来源：http://aff.ctjpmb.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ylj.hammf.cn

C#:   list.Insert(0, 0);
来源：http://hie.xziqi.cn

[D04] 删除元素
来源：http://iym.xingfuxueyuan.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dfz.pycfn.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ynj.redwolf501.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qlg.yvedp.cn

TS:   arr.splice(0, 1);
来源：http://anw.fktsv.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jnl.c1oappe.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yik.zdqjudy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wyb.ctjpmb.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bov.shuidangran.top

[D05] 访问与修改元素
来源：http://okv.hfpthk.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tew.aibaodan.cn


<!-- 参考信息 -->
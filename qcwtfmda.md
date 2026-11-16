代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gct.tian-w.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xga.sweek.top

Ruby: 10.times { |i| puts i }
来源：http://jgs.sxryk.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rkx.ywan-chungtsiang.top

[B05] 遍历数组 / 列表
来源：http://fln.jinyuanbaomall.cn

Py:   for item in arr: print(item)
来源：http://hsl.zycfv.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://omp.guannengcc.top

JS:   for (const item of arr) { console.log(item); }
来源：http://iok.yfazqb.com

TS:   for (const item of arr) { console.log(item); }
来源：http://pxl.bjfxy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://akz.c1oappe.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vnj.c1oappe.top

Ruby: arr.each { |item| puts item }
来源：http://les.yongpay.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vvk.hfpthk.cn

[B06] 遍历字典 / 对象
来源：http://vfv.hcnkem.com

Py:   for k, v in d.items(): print(k, v)
来源：http://cly.svipenyu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zrl.uphjek.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ado.shanyushiyangkeji.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fnt.sysykeji.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ing.jinghuilouyu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ftq.haohaochexian.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lvr.xinyue.icu

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vbu.tianlin.xyz

[B07] while 循环
来源：http://ytw.xingfuxueyuan.xyz

Py:   while i < 10: i += 1
来源：http://dkr.uphjek.com

PHP:  while ($i < 10) { $i++; }
来源：http://znr.mhx1999.top

JS:   while (i < 10) { i++; }
来源：http://gtc.bbcook.cn

TS:   while (i < 10) { i++; }
来源：http://tum.nanxuanxn.top

Java: while (i < 10) { i++; }
来源：http://mcy.xingfuxueyuan.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://paj.wangdashe.top

Ruby: while i < 10; i += 1; end
来源：http://qkj.wangshuangyany.cn

C#:   while (i < 10) { i++; }
来源：http://tys.hesvh.cn

[B08] do-while（至少执行一次）
来源：http://nel.hnqzz.top

Py:   # 无 do-while：用 while True + break
来源：http://ptb.xinyue.icu

PHP:  do { $i++; } while ($i < 10);
来源：http://hll.sxryk.cn

JS:   do { i++; } while (i < 10);
来源：http://zwo.jlsjyb.cn

TS:   do { i++; } while (i < 10);
来源：http://ngw.yuxming.cn

Java: do { i++; } while (i < 10);
来源：http://bbk.gzhubu.top

Go:   for { i++; if i >= 10 { break } }
来源：http://crb.zhaomingkeji.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://rtc.hongshengwenyu.top

C#:   do { i++; } while (i < 10);
来源：http://gle.tian-w.cn

[B09] break 与 continue
来源：http://vol.nanxinkj.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nlv.ybcxt.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gbj.tianlin.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://heu.0kj1m.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://esl.hysaishi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gzb.haohaochexian.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dnw.chenjidiqi.icu

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ohk.zhoulong.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hwf.sjlbkw.cn

[B10] 遍历同时拿索引
来源：http://qdh.zhiwuduotai.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pei.ppjwa.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mse.havefunace.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zkf.ydzc1.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lks.zycfv.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ckm.bbcook.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sco.c1oappe.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ujz.fehbvm.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xkf.zhaomingkeji.xyz

[B11] 生成数字序列 / 区间
来源：http://yoe.tian-w.cn

Py:   list(range(0, 10, 2))
来源：http://utn.guowangkeji.top

PHP:  range(0, 10, 2);
来源：http://lrf.tian-w.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jww.guowangkeji.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ghl.jinghuilouyu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zkn.ppjwa.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bxe.daxiang520.top

Ruby: (0...10).step(2).to_a
来源：http://qxm.fanxiaobao.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://scm.jqgfzy.top

[B12] 跳出多层循环
来源：http://hgz.ctjpmb.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://vws.daria6918.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://erj.chenzaomai.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://spk.yonumen.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hxm.ybcxt.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ikl.yangfankeji.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://utj.ivvv.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fjk.zhijiandao.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wvq.svipenyu.cn

[B13] 判断是否为数字
来源：http://mqe.yonumen.top

Py:   isinstance(x, (int, float))
来源：http://nhz.sufxvd.cn

PHP:  is_numeric($x)
来源：http://cvm.shangyingyoupin.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sne.sufxvd.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ftx.guowangkeji.top

Java: x instanceof Number
来源：http://qvg.gzhubu.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dcd.sufxvd.cn

Ruby: x.is_a?(Numeric)
来源：http://xgt.daxiang520.top

C#:   x is int or double or decimal
来源：http://dor.fengsongda.top

[B14] 判断值是否在集合内
来源：http://pok.yueranfly.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yad.tianlin.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vek.zycfv.cn

JS:   [1, 2, 3].includes(x)
来源：http://qrv.yanxiufei.cn

TS:   [1, 2, 3].includes(x)
来源：http://nse.zhoulong.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://hrn.zhiwuduotai.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qrk.c1oappe.top

Ruby: [1, 2, 3].include?(x)
来源：http://ixh.pycfn.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vyg.yj20258.top

[B15] 布尔运算与取反
来源：http://bme.cheryme.top

Py:   a and b or not c
来源：http://auh.c1oappe.top

PHP:  $a && $b || !$c
来源：http://rhx.quarkkingdee.top

JS:   a && b || !c
来源：http://fig.hysaishi.cn

TS:   a && b || !c
来源：http://cjh.fehbvm.com

Java: a && b || !c
来源：http://fmk.yangfankeji.com

Go:   a && b || !c
来源：http://aoh.jianghu66.top

Ruby: a && b || !c
来源：http://hyt.ppjwa.cn

C#:   a && b || !c
来源：http://ycb.jianghu66.top

[B16] 卫语句：不满足条件提前返回
来源：http://ney.zhongyouzk.top

Py:   if not data: return
来源：http://pkn.316326.xyz

PHP:  if (!$data) { return; }
来源：http://afz.jianghu66.top

JS:   if (!data) return;
来源：http://hcb.zhijiandao.cn

TS:   if (!data) return;
来源：http://yej.shuidangran.top

Java: if (data == null) return;
来源：http://zaw.epnwcf.com

Go:   if data == nil { return }
来源：http://qtm.zdqjudy.top

Ruby: return if data.nil?
来源：http://evn.nanxuanxn.top

C#:   if (data == null) return;
来源：http://mjm.zhaomingkeji.xyz

================================================================================
来源：http://stz.gotoacloud.top

C. 函数与作用域
来源：http://pxa.shanyushiyangtech.top

================================================================================
来源：http://nin.fanxiaobao.xyz

[C01] 定义函数
来源：http://xka.sxryk.cn

Py:   def add(a, b): return a + b
来源：http://lon.hnqzz.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qiz.dashuyun.cn

JS:   function add(a, b) { return a + b; }
来源：http://jof.wangshuangyany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xut.wangdashe.top

Java: static int add(int a, int b) { return a + b; }
来源：http://xhx.kuanghao11.cn

Go:   func add(a, b int) int { return a + b }
来源：http://yhn.0kj1m.cn

Ruby: def add(a, b); a + b; end
来源：http://hjf.jiagoushi.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sao.zhixingplan.top

[C02] 默认参数
来源：http://ogt.fengsongda.top

Py:   def greet(name="World"): return name
来源：http://dsx.ctjpmb.com

PHP:  function greet($name = "World") { return $name; }
来源：http://wuu.hnqzz.top

JS:   function greet(name = "World") { return name; }
来源：http://fha.jinghuilouyu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://lcb.gotoacloud.top

Java: // 无默认参数：方法重载或 Optional
来源：http://pdg.ywan-chungtsiang.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hcb.cqqwz.cn

Ruby: def greet(name = "World") = name
来源：http://zjo.haohaochexian.top

C#:   string Greet(string name = "World") => name;
来源：http://tpq.yueranfly.top

[C03] 可变参数
来源：http://efd.redwolf501.top

Py:   def total(*args): return sum(args)
来源：http://myw.zycfv.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yla.tianlin.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mju.yangfankeji.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://brk.shanyushiyangkeji.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cst.tarul.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wfy.zhiwuduotai.top

Ruby: def total(*nums); nums.sum; end
来源：http://ddz.yvedp.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jse.yueranfly.top

[C04] 命名参数 / 关键字参数
来源：http://svg.zhijiandao.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ztm.jqgufenzy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://udi.jinqigufen.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lsd.xziqi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://uhp.jinqigfzy.top

Java: // 无：用 Builder 模式或 record
来源：http://ceg.zhijiandao.cn

Go:   // 无：用配置结构体参数
来源：http://hlb.yvedp.cn

Ruby: f(a: 1, b: 2)
来源：http://wwx.hammf.cn

C#:   f(a: 1, b: 2)
来源：http://wxm.sjlbkw.cn

[C05] 返回多个值
来源：http://sge.shuidangran.top

Py:   return a, b
来源：http://jss.zhiwuduotai.top

PHP:  return [$a, $b];
来源：http://pci.gotoacloud.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://tev.yongpay.top

TS:   return { a, b };
来源：http://sdt.kuanghao11.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rex.smart0.xyz

Go:   return a, b
来源：http://cyl.chenzaomai.com

Ruby: return a, b
来源：http://uub.yueranfly.top

C#:   return (a, b);              // ValueTuple
来源：http://hdn.tianlin.xyz

[C06] 匿名函数 / lambda
来源：http://xte.yj20258.top

Py:   square = lambda x: x * x
来源：http://iqc.guannengcc.top

PHP:  $square = fn($x) => $x * $x;
来源：http://mul.hnxiangtu.top

JS:   const square = x => x * x;
来源：http://kmb.shuidangran.top

TS:   const square = (x: number): number => x * x;
来源：http://gzg.shuidangran.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vsz.fengsongda.top

Go:   sq := func(x int) int { return x * x }
来源：http://evx.meibo888.top

Ruby: square = ->(x) { x * x }
来源：http://cxj.zhaomingkeji.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://gds.ehwqpu.com

[C07] 把函数作为参数传入
来源：http://cqd.zhoulong.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bpd.nanxinkj.top

PHP:  array_map("strtoupper", $arr);
来源：http://oye.ybcxt.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yxd.yj202588.top

TS:   arr.map(String)
来源：http://xgf.jinghuilouyu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zje.daria6918.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qab.52xcode.cn

Ruby: arr.map(&:upcase)
来源：http://nuw.0kj1m.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mol.yj20258888.top

[C08] 闭包
来源：http://cuh.xziqi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tdv.yuxming.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pso.hammf.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nmz.bjfxy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://afq.jlsjyb.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://suv.ivvv.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://obk.ydzc1.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cmi.fanxiaobao.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tyl.svipenyu.cn

[C09] 递归
来源：http://gby.nanxuanxn.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jqf.smart0.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xop.ydzc1.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ugp.jinyuanbaomall.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lwi.guannengcc.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hly.zdbjq.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lxj.sufxvd.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bbw.9152youxi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cis.fktsv.cn

[C10] 变量作用域
来源：http://pqm.tian-w.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tlj.tianlin.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gfj.shangyingyoupin.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://luf.daxiang520.top

TS:   同 JS
来源：http://kdy.nwbrower.top

Java: 方法内为块级作用域
来源：http://eep.jinghuilouyu.cn

Go:   花括号块级作用域
来源：http://hbu.jqgufenzy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uup.fehbvm.com

C#:   块级作用域
来源：http://ggd.hysaishi.cn

[C11] 模块导入与导出
来源：http://hjl.shanyushiyangkeji.top

Py:   from module import func
来源：http://nmg.hongshengwenyu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://sbi.zycfv.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jss.bjfxy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fga.hysaishi.cn

Java: import java.util.List;
来源：http://nai.ehwqpu.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gqo.0kj1m.cn

Ruby: require "json"; require_relative "./util"
来源：http://eno.chenjidiqi.icu

C#:   using System.Text;
来源：http://nun.ywan-chungtsiang.top

[C12] 立即执行函数 IIFE
来源：http://fnt.zhengqikj.top

Py:   (lambda: print("run"))()
来源：http://egq.zhoulong.xyz

PHP:  (function () { echo "run"; })();
来源：http://eng.pengpengdd.cyou

JS:   (() => { console.log("run"); })();
来源：http://ixa.cashguo.top

TS:   (() => { console.log("run"); })();
来源：http://gxi.yonumen.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zdx.bbcook.cn

Go:   func() { fmt.Println("run") }()
来源：http://xmp.guannengcc.top

Ruby: -> { puts "run" }.call
来源：http://tga.fehbvm.com

C#:   // 无 IIFE：用静态构造函数
来源：http://uew.daria6918.cn

[C13] 类型声明 / 类型注解
来源：http://kgk.hysaishi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ozq.xinyue.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tap.fzhhl.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://iwm.yongpay.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iry.kuanghao11.cn

Java: int add(int a, int b) { return a + b; }
来源：http://axi.hongshengwenyu.top

Go:   func add(a, b int) int
来源：http://liz.quarkkingdee.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xxi.ehwqpu.com

C#:   int Add(int a, int b) => a + b;
来源：http://txo.fanxiaobao.xyz

[C14] 泛型函数
来源：http://jse.cucudq.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vtr.zhijiandao.cn

PHP:  // 无泛型
来源：http://jju.wangshuangyany.cn

JS:   // 无泛型
来源：http://tuz.jinyuanbaomall.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rlf.svipenyu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tyt.wangshuangyany.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wfj.ydzc1.top

Ruby: # 无泛型
来源：http://tes.sufxvd.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://axm.feifeiyinyue.top

[C15] 解构 / 展开参数
来源：http://zos.shzxlz.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://aco.hongshengwenyu.top

PHP:  [$a, $b] = $pair;
来源：http://uhl.dianchejie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wlb.tanke756.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ouk.daxiang520.top

Java: // 无解构
来源：http://qgu.tian-w.cn

Go:   // 无解构
来源：http://dus.xingfuxueyuan.xyz

Ruby: a, b = pair
来源：http://xll.jyoumei.cn

C#:   var (a, b) = pair;
来源：http://ofq.redwolf501.top

[C16] 函数 / 方法重载
来源：http://tdh.chenjidiqi.icu

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ymu.shanyushiyangtech.top

PHP:  // 无重载
来源：http://iwz.316326.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://lmk.dianchejie.cn

TS:   // 用联合类型或重载签名声明
来源：http://kzl.daria6918.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://aqh.yuanzhike.top

Go:   // 无重载：用不同函数名
来源：http://xru.hfpthk.cn

Ruby: # 无重载：靠动态参数
来源：http://uor.hcnkem.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://byj.zhoulong.xyz

================================================================================
来源：http://wjt.hesvh.cn

D. 数组 / 列表 / 集合
来源：http://cpk.gaohongyu789.top

================================================================================
来源：http://liq.yuxming.cn

[D01] 创建数组 / 列表
来源：http://dwh.tanke756.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://qls.chenzaomai.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gbg.hywenlv.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://doy.snrcjt.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wbr.tanke756.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kxf.tianlin.xyz

Go:   arr := []int{1, 2, 3}
来源：http://kxj.zhaomingkeji.xyz

Ruby: arr = [1, 2, 3]
来源：http://ndd.fengsongda.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://awp.jqgufenzy.top

[D02] 追加元素到末尾
来源：http://ily.pengpengdd.cyou

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cwo.yvedp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://acn.yueranfly.top

JS:   arr.push(4);
来源：http://fdl.xinyue.icu

TS:   arr.push(4);
来源：http://jps.vehdjk.com

Java: list.add(4);
来源：http://ymy.hfpthk.cn

Go:   arr = append(arr, 4)
来源：http://udt.chenjidiqi.icu

Ruby: arr << 4; arr.push(5)
来源：http://nat.shuidangran.top

C#:   list.Add(4);
来源：http://gcr.52xcode.cn

[D03] 在指定位置插入元素
来源：http://gxm.jyoumei.cn

Py:   arr.insert(0, 0)
来源：http://mgf.zhijiandao.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://olv.hfpthk.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wri.yfazqb.com

TS:   arr.splice(0, 0, 0);
来源：http://uew.yangfankeji.com

Java: list.add(0, 0);
来源：http://dsm.fehbvm.com

Go:   arr = append([]int{0}, arr...)
来源：http://vkn.c1oappe.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cep.ctjpmb.com

C#:   list.Insert(0, 0);
来源：http://zia.snrcjt.cn

[D04] 删除元素
来源：http://tty.zhixingplan.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lcj.havefunace.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tef.0kj1m.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sol.jianghu66.top

TS:   arr.splice(0, 1);
来源：http://uhb.haohaochexian.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://plv.guowangkeji.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hog.guannengcc.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://epl.iojbl.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tie.dashuyun.cn

[D05] 访问与修改元素
来源：http://qrn.hywenlv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rmb.xuanzx.com


<!-- 参考信息 -->
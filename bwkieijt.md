代发 wailian999

Py:   for i in range(10): print(i)
来源：http://mia.andypj.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yep.gaohongyu789.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xyf.feifeiyinyue.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ngi.sweek.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cve.kuanghao11.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tny.hammf.cn

Ruby: 10.times { |i| puts i }
来源：http://lex.gaohongyu789.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://igp.birdmap.top

[B05] 遍历数组 / 列表
来源：http://frk.jyoumei.cn

Py:   for item in arr: print(item)
来源：http://pnm.uphjek.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rpw.yj20258888.top

JS:   for (const item of arr) { console.log(item); }
来源：http://pqq.yuanzhike.top

TS:   for (const item of arr) { console.log(item); }
来源：http://qnk.pengpengdd.cyou

Java: for (var item : arr) { System.out.println(item); }
来源：http://tgg.9152youxi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://znx.gogol.net.cn

Ruby: arr.each { |item| puts item }
来源：http://awh.feifeiyinyue.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yfu.meibo888.top

[B06] 遍历字典 / 对象
来源：http://adu.xingfuxueyuan.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://lrz.yueranfly.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yry.chenjidiqi.icu

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://csr.zycfv.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qgo.yj20258.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hey.jiagoushi.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lrk.zhaomingkeji.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://txw.shanyushiyangkeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hfi.tian-w.cn

[B07] while 循环
来源：http://zwh.zhengqikj.top

Py:   while i < 10: i += 1
来源：http://xoe.cucudq.cn

PHP:  while ($i < 10) { $i++; }
来源：http://jrm.gaohongyu789.top

JS:   while (i < 10) { i++; }
来源：http://gof.xylfe.cn

TS:   while (i < 10) { i++; }
来源：http://pdv.hesvh.cn

Java: while (i < 10) { i++; }
来源：http://das.hnqzz.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://boo.sufxvd.cn

Ruby: while i < 10; i += 1; end
来源：http://epw.zhijiandao.cn

C#:   while (i < 10) { i++; }
来源：http://gdw.feifeiyinyue.top

[B08] do-while（至少执行一次）
来源：http://drk.shanyushiyangkeji.top

Py:   # 无 do-while：用 while True + break
来源：http://rgy.andypj.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://zlc.uphjek.com

JS:   do { i++; } while (i < 10);
来源：http://vok.zhijiandao.cn

TS:   do { i++; } while (i < 10);
来源：http://sbz.hywenlv.cn

Java: do { i++; } while (i < 10);
来源：http://zai.jinghuilouyu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ghw.yvedp.cn

Ruby: begin; i += 1; end while i < 10
来源：http://bos.redwolf501.top

C#:   do { i++; } while (i < 10);
来源：http://icf.xinyue.icu

[B09] break 与 continue
来源：http://uta.aibaodan.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://uof.xuanzx.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hgb.zhengqikj.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://djt.cucudq.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://own.cheryme.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zsh.quarkkingdee.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ktk.dianchejie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tox.ydzc1.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wyj.jqgufenzy.top

[B10] 遍历同时拿索引
来源：http://lhm.xylfe.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qzz.tanke756.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cns.yuxming.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hog.cdnleiting.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yzv.jqgfzy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qwj.aibaodan.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://loq.hammf.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://inq.zhijiandao.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vfa.sjlbkw.cn

[B11] 生成数字序列 / 区间
来源：http://pfy.shanyushiyangtech.top

Py:   list(range(0, 10, 2))
来源：http://uda.sufxvd.cn

PHP:  range(0, 10, 2);
来源：http://bft.vehdjk.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jsb.epnwcf.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wmt.ywan-chungtsiang.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rkv.bjfxy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://smi.nanxinkj.top

Ruby: (0...10).step(2).to_a
来源：http://nrx.dashuyun.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zpp.nanxuanxn.top

[B12] 跳出多层循环
来源：http://kqy.yueranfly.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://czn.gotoacloud.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://poh.shzxlz.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://brv.yonumen.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rvd.gaohongyu789.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://woh.hnqzz.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gtc.xinyue.icu

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jpe.gogol.net.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://shb.jianghu66.top

[B13] 判断是否为数字
来源：http://zsj.daxiang520.top

Py:   isinstance(x, (int, float))
来源：http://wrg.sufxvd.cn

PHP:  is_numeric($x)
来源：http://rma.zhengqikj.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lnp.kuanghao11.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oku.hnxiangtu.top

Java: x instanceof Number
来源：http://pyz.ywan-chungtsiang.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://szs.nwbrower.top

Ruby: x.is_a?(Numeric)
来源：http://tut.yueranfly.top

C#:   x is int or double or decimal
来源：http://gjs.jyoumei.cn

[B14] 判断值是否在集合内
来源：http://kpy.jinghuilouyu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cli.ybcxt.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zjp.shzxlz.cn

JS:   [1, 2, 3].includes(x)
来源：http://irk.dashuyun.cn

TS:   [1, 2, 3].includes(x)
来源：http://neg.chenjidiqi.icu

Java: List.of(1, 2, 3).contains(x)
来源：http://zjr.jqgufenzy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://uzj.fktsv.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vdr.9152youxi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xwm.yanxiufei.cn

[B15] 布尔运算与取反
来源：http://uhn.tian-w.cn

Py:   a and b or not c
来源：http://ssd.52xcode.cn

PHP:  $a && $b || !$c
来源：http://xis.gotoacloud.top

JS:   a && b || !c
来源：http://oay.cdnleiting.top

TS:   a && b || !c
来源：http://mnz.jinyuanbaomall.cn

Java: a && b || !c
来源：http://gsg.ivvv.top

Go:   a && b || !c
来源：http://iua.yonumen.top

Ruby: a && b || !c
来源：http://lyw.meibo888.top

C#:   a && b || !c
来源：http://wpt.ivvv.top

[B16] 卫语句：不满足条件提前返回
来源：http://drk.xziqi.cn

Py:   if not data: return
来源：http://vga.hywenlv.cn

PHP:  if (!$data) { return; }
来源：http://bso.yj20258.top

JS:   if (!data) return;
来源：http://uit.zhaomingkeji.xyz

TS:   if (!data) return;
来源：http://qrm.hammf.cn

Java: if (data == null) return;
来源：http://gsl.sweek.top

Go:   if data == nil { return }
来源：http://rnc.shuidangran.top

Ruby: return if data.nil?
来源：http://jpt.fktsv.cn

C#:   if (data == null) return;
来源：http://czk.hnxiangtu.top

================================================================================
来源：http://mgn.xuetiantiany.cn

C. 函数与作用域
来源：http://oxl.jqgfzy.top

================================================================================
来源：http://jpt.iojbl.cn

[C01] 定义函数
来源：http://geu.zhengqikj.top

Py:   def add(a, b): return a + b
来源：http://byq.ivvv.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rkt.shuidangran.top

JS:   function add(a, b) { return a + b; }
来源：http://gue.redwolf501.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://idq.shanyushiyangkeji.top

Java: static int add(int a, int b) { return a + b; }
来源：http://vjs.zhaomingkeji.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://fhb.iojbl.cn

Ruby: def add(a, b); a + b; end
来源：http://bsf.hesvh.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://aib.epnwcf.com

[C02] 默认参数
来源：http://hjt.tian-w.cn

Py:   def greet(name="World"): return name
来源：http://vgb.yuanzhike.top

PHP:  function greet($name = "World") { return $name; }
来源：http://lwu.bjfxy.top

JS:   function greet(name = "World") { return name; }
来源：http://agj.zhiwuduotai.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ksm.zhoulong.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://toa.vehdjk.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xlz.aizwys.cn

Ruby: def greet(name = "World") = name
来源：http://wft.haohaochexian.top

C#:   string Greet(string name = "World") => name;
来源：http://edr.meibo888.top

[C03] 可变参数
来源：http://clz.andypj.xyz

Py:   def total(*args): return sum(args)
来源：http://mer.zhixingplan.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qfn.yfazqb.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wbf.cucudq.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://icg.ppjwa.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bza.jinyuanbaomall.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wpc.kuanghao11.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ypb.nanxuanxn.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mtz.zhiwuduotai.top

[C04] 命名参数 / 关键字参数
来源：http://fev.yangfankeji.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kxk.hnqzz.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vdr.feifeiyinyue.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ftm.pengpengdd.cyou

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rnh.daria6918.cn

Java: // 无：用 Builder 模式或 record
来源：http://mss.yonumen.top

Go:   // 无：用配置结构体参数
来源：http://kix.fzhhl.top

Ruby: f(a: 1, b: 2)
来源：http://zia.ybcxt.top

C#:   f(a: 1, b: 2)
来源：http://nmr.ppjwa.cn

[C05] 返回多个值
来源：http://uzr.yfazqb.com

Py:   return a, b
来源：http://unv.hnxiangtu.top

PHP:  return [$a, $b];
来源：http://fkb.zhaomingkeji.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://nbw.yangfankeji.com

TS:   return { a, b };
来源：http://drv.hesvh.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zsd.yuanzhike.top

Go:   return a, b
来源：http://zkz.chenlongwang.top

Ruby: return a, b
来源：http://cgl.zhoulong.xyz

C#:   return (a, b);              // ValueTuple
来源：http://mwq.9152youxi.cn

[C06] 匿名函数 / lambda
来源：http://jvg.nanxinkj.top

Py:   square = lambda x: x * x
来源：http://btj.shangyingyoupin.top

PHP:  $square = fn($x) => $x * $x;
来源：http://rua.yonumen.top

JS:   const square = x => x * x;
来源：http://ykt.tarul.cn

TS:   const square = (x: number): number => x * x;
来源：http://aih.ydzc1.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hog.yanxiufei.cn

Go:   sq := func(x int) int { return x * x }
来源：http://oyc.fengsongda.top

Ruby: square = ->(x) { x * x }
来源：http://qne.cqqwz.cn

C#:   Func<int, int> square = x => x * x;
来源：http://gzc.cucudq.cn

[C07] 把函数作为参数传入
来源：http://ptd.yfazqb.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://aow.0kj1m.cn

PHP:  array_map("strtoupper", $arr);
来源：http://zak.shzxlz.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kki.yuanzhike.top

TS:   arr.map(String)
来源：http://gvk.yj202588.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://slm.yvedp.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rnk.yongpay.top

Ruby: arr.map(&:upcase)
来源：http://lhq.daria6918.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://twz.9152youxi.cn

[C08] 闭包
来源：http://dsz.andypj.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gpy.dianchejie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mgm.sufxvd.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://udj.yanxiufei.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zsq.meibo888.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jbd.hnxiangtu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nqx.fanxiaobao.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vyf.jiagoushi.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mbt.shzxlz.cn

[C09] 递归
来源：http://eca.sxryk.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wgf.wangdashe.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nts.fehbvm.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ltv.ywan-chungtsiang.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://khf.ivvv.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://oje.feifeiyinyue.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zer.yj20258.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ivi.jiagoushi.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uyn.gaohongyu789.top

[C10] 变量作用域
来源：http://jvx.zhongyouzk.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lct.zhixingplan.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://smm.zhixingplan.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sjx.andypj.xyz

TS:   同 JS
来源：http://ril.hywenlv.cn

Java: 方法内为块级作用域
来源：http://opq.wangshuangyany.cn

Go:   花括号块级作用域
来源：http://ajp.guowangkeji.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ggl.svipenyu.cn

C#:   块级作用域
来源：http://xby.shangyingyoupin.top

[C11] 模块导入与导出
来源：http://irw.sysykeji.top

Py:   from module import func
来源：http://xrv.kuanghao11.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mhi.gotoacloud.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://pev.iojbl.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qtg.zdqjudy.top

Java: import java.util.List;
来源：http://rqj.andypj.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ley.hongshengwenyu.top

Ruby: require "json"; require_relative "./util"
来源：http://kwt.daxiang520.top

C#:   using System.Text;
来源：http://mjg.feifeiyinyue.top

[C12] 立即执行函数 IIFE
来源：http://xkv.cqqwz.cn

Py:   (lambda: print("run"))()
来源：http://tfc.tianlin.xyz

PHP:  (function () { echo "run"; })();
来源：http://fnv.xylfe.cn

JS:   (() => { console.log("run"); })();
来源：http://ten.zycfv.cn

TS:   (() => { console.log("run"); })();
来源：http://ikx.yj20258888.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://eyq.tian-w.cn

Go:   func() { fmt.Println("run") }()
来源：http://wjy.c1oappe.top

Ruby: -> { puts "run" }.call
来源：http://raf.yj20258.top

C#:   // 无 IIFE：用静态构造函数
来源：http://mck.hfpthk.cn

[C13] 类型声明 / 类型注解
来源：http://edg.daria6918.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xvw.shuidangran.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ijn.hfpthk.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bgt.shangyingyoupin.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rqk.feifeiyinyue.top

Java: int add(int a, int b) { return a + b; }
来源：http://fzt.yonumen.top

Go:   func add(a, b int) int
来源：http://pec.hammf.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hve.pycfn.com

C#:   int Add(int a, int b) => a + b;
来源：http://aav.shanyushiyangtech.top

[C14] 泛型函数
来源：http://dxq.zhoulong.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bix.mhx1999.top

PHP:  // 无泛型
来源：http://jpl.quarkkingdee.top

JS:   // 无泛型
来源：http://urw.gzhubu.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kym.cashguo.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jnq.cashguo.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://oeo.tarul.cn

Ruby: # 无泛型
来源：http://obj.sufxvd.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wmm.meibo888.top

[C15] 解构 / 展开参数
来源：http://yzw.jqgfzy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ymm.bjfxy.top

PHP:  [$a, $b] = $pair;
来源：http://ezq.ppjwa.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://iju.shanyushiyangkeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uyk.zhengqikj.top

Java: // 无解构
来源：http://jpv.andypj.xyz

Go:   // 无解构
来源：http://cvd.nwbrower.top

Ruby: a, b = pair
来源：http://dqx.zdbjq.cn

C#:   var (a, b) = pair;
来源：http://jlv.tanke756.top

[C16] 函数 / 方法重载
来源：http://dil.aibaodan.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wpt.ydzc1.top

PHP:  // 无重载
来源：http://tyg.jqgfzy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://miq.hammf.cn

TS:   // 用联合类型或重载签名声明
来源：http://ebq.zhiwuduotai.top

Java: void f(int a) {}  void f(String a) {}
来源：http://vqk.meibo888.top

Go:   // 无重载：用不同函数名
来源：http://car.hywenlv.cn

Ruby: # 无重载：靠动态参数
来源：http://oqi.sjlbkw.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://jba.ybcxt.top

================================================================================
来源：http://sxn.yanxiufei.cn

D. 数组 / 列表 / 集合
来源：http://xja.hesvh.cn

================================================================================
来源：http://ybr.hongshengwenyu.top

[D01] 创建数组 / 列表
来源：http://hdv.jiagoushi.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://jjq.feifeiyinyue.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vzs.cheryme.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bko.chenzaomai.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://wqx.zhijiandao.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sqw.xingfuxueyuan.xyz

Go:   arr := []int{1, 2, 3}
来源：http://aoc.ydzc1.top

Ruby: arr = [1, 2, 3]
来源：http://dlh.jiagoushi.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ptx.nwbrower.top

[D02] 追加元素到末尾
来源：http://bdd.ppjwa.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://oca.zhaomingkeji.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fkl.aizwys.cn

JS:   arr.push(4);
来源：http://wqx.jqgufenzy.top

TS:   arr.push(4);
来源：http://tlo.sjlbkw.cn

Java: list.add(4);
来源：http://ltf.sweek.top

Go:   arr = append(arr, 4)
来源：http://fkx.ydzc1.top

Ruby: arr << 4; arr.push(5)
来源：http://fox.havefunace.top

C#:   list.Add(4);
来源：http://tjl.xziqi.cn

[D03] 在指定位置插入元素
来源：http://nax.wangshuangyany.cn

Py:   arr.insert(0, 0)
来源：http://zbv.ctjpmb.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://giz.cucudq.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://iyt.yangfankeji.com

TS:   arr.splice(0, 0, 0);
来源：http://uaj.andypj.xyz

Java: list.add(0, 0);
来源：http://ppo.smart0.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://fql.ehwqpu.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://prb.tianlin.xyz

C#:   list.Insert(0, 0);
来源：http://ojc.tianlin.xyz

[D04] 删除元素
来源：http://usz.bjfxy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yhd.zdqjudy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zub.xylfe.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lwy.yj202588.top

TS:   arr.splice(0, 1);
来源：http://ubp.jqgufenzy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rqp.shzxlz.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cqt.cheryme.top


<!-- 参考信息 -->
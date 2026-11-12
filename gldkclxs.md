代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ken.chenzaomai.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hhc.jlsjyb.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hea.xuetiantiany.cn

[B04] for 计数循环
来源：http://upi.quarkkingdee.top

Py:   for i in range(10): print(i)
来源：http://bdp.kuanghao11.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gao.ppjwa.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nyr.yuxming.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zxn.nwbrower.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://piq.fzhhl.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tkt.ppjwa.cn

Ruby: 10.times { |i| puts i }
来源：http://eez.jqgufenzy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ffz.feifeiyinyue.top

[B05] 遍历数组 / 列表
来源：http://vut.gzhubu.top

Py:   for item in arr: print(item)
来源：http://mee.hysaishi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hkc.316326.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://oof.xingfuxueyuan.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://cgt.fanxiaobao.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://byw.nwbrower.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kuo.shanyushiyangkeji.top

Ruby: arr.each { |item| puts item }
来源：http://qcx.c1oappe.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://boj.xuetiantiany.cn

[B06] 遍历字典 / 对象
来源：http://ror.yuanzhike.top

Py:   for k, v in d.items(): print(k, v)
来源：http://niq.sjlbkw.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wuw.aizwys.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tjs.hongshengwenyu.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xuu.zhijiandao.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tfx.jiagoushi.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hbr.fanxiaobao.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ftx.zhaomingkeji.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://htz.hnqzz.top

[B07] while 循环
来源：http://fkl.hywenlv.cn

Py:   while i < 10: i += 1
来源：http://tno.yuxming.cn

PHP:  while ($i < 10) { $i++; }
来源：http://sza.bjfxy.top

JS:   while (i < 10) { i++; }
来源：http://vbe.sweek.top

TS:   while (i < 10) { i++; }
来源：http://qsz.cheryme.top

Java: while (i < 10) { i++; }
来源：http://kpj.gogol.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cxz.yangfankeji.com

Ruby: while i < 10; i += 1; end
来源：http://plw.9152youxi.cn

C#:   while (i < 10) { i++; }
来源：http://cgg.fehbvm.com

[B08] do-while（至少执行一次）
来源：http://eso.haohaochexian.top

Py:   # 无 do-while：用 while True + break
来源：http://bnj.wangshuangyany.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://epp.fzhhl.top

JS:   do { i++; } while (i < 10);
来源：http://hsm.shangyingyoupin.top

TS:   do { i++; } while (i < 10);
来源：http://myr.ppjwa.cn

Java: do { i++; } while (i < 10);
来源：http://pjt.yj20258.top

Go:   for { i++; if i >= 10 { break } }
来源：http://qkv.kuanghao11.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wap.hesvh.cn

C#:   do { i++; } while (i < 10);
来源：http://qrg.kuanghao11.cn

[B09] break 与 continue
来源：http://faj.jinqigfzy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ttr.svipenyu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wes.hnqzz.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ebv.jinyuanbaomall.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kcf.pycfn.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tna.shanyushiyangtech.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bno.yongpay.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kfr.sysykeji.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ctd.hysaishi.cn

[B10] 遍历同时拿索引
来源：http://met.yanxiufei.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wqz.aizwys.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fnx.zhoulong.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bvg.zhongyouzk.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zkh.xinyue.icu

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ndx.cucudq.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qqb.zhengqikj.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ubx.zhixingplan.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://heh.xuanzx.com

[B11] 生成数字序列 / 区间
来源：http://ziw.jqgfzy.top

Py:   list(range(0, 10, 2))
来源：http://tjc.mhx1999.top

PHP:  range(0, 10, 2);
来源：http://yhb.havefunace.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eoy.shanyushiyangkeji.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hja.sweek.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hdi.chenlongwang.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://swl.0kj1m.cn

Ruby: (0...10).step(2).to_a
来源：http://jto.bbcook.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dtw.yj20258888.top

[B12] 跳出多层循环
来源：http://llq.jianghu66.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://wzi.nanxuanxn.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://yan.nanxinkj.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zxw.9152youxi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ojb.hammf.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lba.dashuyun.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kpf.iojbl.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rmv.cheryme.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cqt.guowangkeji.top

[B13] 判断是否为数字
来源：http://plj.zdbjq.cn

Py:   isinstance(x, (int, float))
来源：http://fei.nanxinkj.top

PHP:  is_numeric($x)
来源：http://iyp.yanxiufei.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mbi.xylfe.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wod.hywenlv.cn

Java: x instanceof Number
来源：http://grk.jqgufenzy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xoo.hywenlv.cn

Ruby: x.is_a?(Numeric)
来源：http://sqo.redwolf501.top

C#:   x is int or double or decimal
来源：http://arf.cheryme.top

[B14] 判断值是否在集合内
来源：http://kxn.fanxiaobao.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ipl.ehwqpu.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://plj.yuxming.cn

JS:   [1, 2, 3].includes(x)
来源：http://fow.cheryme.top

TS:   [1, 2, 3].includes(x)
来源：http://gpe.gotoacloud.top

Java: List.of(1, 2, 3).contains(x)
来源：http://sxj.guannengcc.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yob.cdnleiting.top

Ruby: [1, 2, 3].include?(x)
来源：http://hsb.zhixingplan.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vuo.jianghu66.top

[B15] 布尔运算与取反
来源：http://asr.snrcjt.cn

Py:   a and b or not c
来源：http://jtf.0kj1m.cn

PHP:  $a && $b || !$c
来源：http://rqu.quarkkingdee.top

JS:   a && b || !c
来源：http://mxg.hywenlv.cn

TS:   a && b || !c
来源：http://hfa.xylfe.cn

Java: a && b || !c
来源：http://dbg.jinqigfzy.top

Go:   a && b || !c
来源：http://fjq.zhijiandao.cn

Ruby: a && b || !c
来源：http://voi.yonumen.top

C#:   a && b || !c
来源：http://xzs.9152youxi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://rsg.chenlongwang.top

Py:   if not data: return
来源：http://kpr.ehwqpu.com

PHP:  if (!$data) { return; }
来源：http://tmb.fktsv.cn

JS:   if (!data) return;
来源：http://esx.xinyue.icu

TS:   if (!data) return;
来源：http://vuj.hysaishi.cn

Java: if (data == null) return;
来源：http://cwx.fktsv.cn

Go:   if data == nil { return }
来源：http://zfx.fengsongda.top

Ruby: return if data.nil?
来源：http://ulp.shanyushiyangkeji.top

C#:   if (data == null) return;
来源：http://njj.xinyue.icu

================================================================================
来源：http://uok.tarul.cn

C. 函数与作用域
来源：http://vup.zhoulong.xyz

================================================================================
来源：http://ggs.9152youxi.cn

[C01] 定义函数
来源：http://kjm.jinyuanbaomall.cn

Py:   def add(a, b): return a + b
来源：http://fhj.gzhubu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pkl.wangdashe.top

JS:   function add(a, b) { return a + b; }
来源：http://era.gzhubu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://idl.0kj1m.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gsl.tanke756.top

Go:   func add(a, b int) int { return a + b }
来源：http://vbj.hnqzz.top

Ruby: def add(a, b); a + b; end
来源：http://ngo.iojbl.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zlz.uphjek.com

[C02] 默认参数
来源：http://wwy.hesvh.cn

Py:   def greet(name="World"): return name
来源：http://zhi.hnxiangtu.top

PHP:  function greet($name = "World") { return $name; }
来源：http://qjg.birdmap.top

JS:   function greet(name = "World") { return name; }
来源：http://iye.zhiwuduotai.top

TS:   function greet(name: string = "World") { return name; }
来源：http://qnj.yangfankeji.com

Java: // 无默认参数：方法重载或 Optional
来源：http://wsl.andypj.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://duu.hnqzz.top

Ruby: def greet(name = "World") = name
来源：http://nfd.tianlin.xyz

C#:   string Greet(string name = "World") => name;
来源：http://tzj.hcnkem.com

[C03] 可变参数
来源：http://drf.daria6918.cn

Py:   def total(*args): return sum(args)
来源：http://ceq.yvedp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://shf.sxryk.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jea.fehbvm.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kig.dashuyun.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pfe.redwolf501.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ndb.dianchejie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://lke.xinyue.icu

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://iyn.jyoumei.cn

[C04] 命名参数 / 关键字参数
来源：http://ohx.yonumen.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gcx.316326.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://che.yj202588.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://maj.hcnkem.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fms.redwolf501.top

Java: // 无：用 Builder 模式或 record
来源：http://cim.yuanzhike.top

Go:   // 无：用配置结构体参数
来源：http://uyh.pengpengdd.cyou

Ruby: f(a: 1, b: 2)
来源：http://ugi.0kj1m.cn

C#:   f(a: 1, b: 2)
来源：http://irg.hywenlv.cn

[C05] 返回多个值
来源：http://lag.daxiang520.top

Py:   return a, b
来源：http://jzq.jinqigufen.top

PHP:  return [$a, $b];
来源：http://tyd.chenzaomai.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://djw.dianchejie.cn

TS:   return { a, b };
来源：http://yil.sufxvd.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qat.redwolf501.top

Go:   return a, b
来源：http://hjw.52xcode.cn

Ruby: return a, b
来源：http://irj.guowangkeji.top

C#:   return (a, b);              // ValueTuple
来源：http://wyo.dashuyun.cn

[C06] 匿名函数 / lambda
来源：http://vby.jianghu66.top

Py:   square = lambda x: x * x
来源：http://xeh.ivvv.top

PHP:  $square = fn($x) => $x * $x;
来源：http://dcy.feifeiyinyue.top

JS:   const square = x => x * x;
来源：http://epy.chenlongwang.top

TS:   const square = (x: number): number => x * x;
来源：http://dft.shangyingyoupin.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pjb.uphjek.com

Go:   sq := func(x int) int { return x * x }
来源：http://qtk.zhaomingkeji.xyz

Ruby: square = ->(x) { x * x }
来源：http://qbu.ehwqpu.com

C#:   Func<int, int> square = x => x * x;
来源：http://uqn.xylfe.cn

[C07] 把函数作为参数传入
来源：http://jjz.hywenlv.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nww.vehdjk.com

PHP:  array_map("strtoupper", $arr);
来源：http://qlt.yangfankeji.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zok.hywenlv.cn

TS:   arr.map(String)
来源：http://mtw.aizwys.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ntt.svipenyu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zws.cqqwz.cn

Ruby: arr.map(&:upcase)
来源：http://vxz.jqgfzy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://pib.fengsongda.top

[C08] 闭包
来源：http://qsz.nwbrower.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vtk.xingfuxueyuan.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wia.c1oappe.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rku.fehbvm.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cif.guannengcc.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tua.jqgufenzy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ycs.hammf.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jav.xuetiantiany.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uzj.dashuyun.cn

[C09] 递归
来源：http://nmc.aizwys.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rqq.hywenlv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tki.zhengqikj.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nzz.dashuyun.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jka.fengsongda.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fdt.yonumen.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://djd.daria6918.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fiz.yvedp.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jmx.fanxiaobao.xyz

[C10] 变量作用域
来源：http://elh.zdqjudy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nhu.jqgfzy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lsd.jianghu66.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ddk.tanke756.top

TS:   同 JS
来源：http://cmo.ehwqpu.com

Java: 方法内为块级作用域
来源：http://jle.gzhubu.top

Go:   花括号块级作用域
来源：http://wyb.jyoumei.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hiv.yuanzhike.top

C#:   块级作用域
来源：http://hhc.316326.xyz

[C11] 模块导入与导出
来源：http://ckp.yanxiufei.cn

Py:   from module import func
来源：http://npj.hongshengwenyu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://wjn.dashuyun.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://cgc.cucudq.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://iza.sufxvd.cn

Java: import java.util.List;
来源：http://hot.fengsongda.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kqp.hnqzz.top

Ruby: require "json"; require_relative "./util"
来源：http://bgy.aibaodan.cn

C#:   using System.Text;
来源：http://wsm.fengsongda.top

[C12] 立即执行函数 IIFE
来源：http://czx.cdnleiting.top

Py:   (lambda: print("run"))()
来源：http://weu.ydjk.org.cn

PHP:  (function () { echo "run"; })();
来源：http://xxv.ehwqpu.com

JS:   (() => { console.log("run"); })();
来源：http://gqu.ydjk.org.cn

TS:   (() => { console.log("run"); })();
来源：http://iok.gotoacloud.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://itq.xylfe.cn

Go:   func() { fmt.Println("run") }()
来源：http://fyl.pycfn.com

Ruby: -> { puts "run" }.call
来源：http://jno.sjlbkw.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://rew.aizwys.cn

[C13] 类型声明 / 类型注解
来源：http://kdk.jinqigfzy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://czn.cqqwz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xof.yj20258.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ppk.zhijiandao.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wij.sxryk.cn

Java: int add(int a, int b) { return a + b; }
来源：http://njs.yonumen.top

Go:   func add(a, b int) int
来源：http://pee.yj202588.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mjl.yj20258888.top

C#:   int Add(int a, int b) => a + b;
来源：http://wxl.wangdashe.top

[C14] 泛型函数
来源：http://dzz.daxiang520.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kqo.316326.xyz

PHP:  // 无泛型
来源：http://dlb.epnwcf.com

JS:   // 无泛型
来源：http://lcs.yanxiufei.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kgu.zhongyouzk.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yuy.cucudq.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gir.guowangkeji.top

Ruby: # 无泛型
来源：http://rcm.jinqigfzy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zdz.yj20258.top

[C15] 解构 / 展开参数
来源：http://czy.52xcode.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rim.ydjk.org.cn

PHP:  [$a, $b] = $pair;
来源：http://atl.hnqzz.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://csc.mhx1999.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vtr.316326.xyz

Java: // 无解构
来源：http://hlk.pengpengdd.cyou

Go:   // 无解构
来源：http://cyr.fehbvm.com

Ruby: a, b = pair
来源：http://xeh.hongshengwenyu.top

C#:   var (a, b) = pair;
来源：http://xnx.jinqigfzy.top

[C16] 函数 / 方法重载
来源：http://psq.svipenyu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hnf.meibo888.top

PHP:  // 无重载
来源：http://hkl.xziqi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://olu.nwbrower.top

TS:   // 用联合类型或重载签名声明
来源：http://vix.fanxiaobao.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://rtq.zdbjq.cn

Go:   // 无重载：用不同函数名
来源：http://dum.zhongyouzk.top

Ruby: # 无重载：靠动态参数
来源：http://epg.aibaodan.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://bvc.jinqigfzy.top

================================================================================
来源：http://qkj.yj20258888.top

D. 数组 / 列表 / 集合
来源：http://vji.cqqwz.cn

================================================================================
来源：http://myp.ctjpmb.com

[D01] 创建数组 / 列表
来源：http://tjr.dianchejie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://kgj.aizwys.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://uxs.chenzaomai.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gro.hysaishi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://yel.yonumen.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rwl.xinyue.icu

Go:   arr := []int{1, 2, 3}
来源：http://sle.birdmap.top

Ruby: arr = [1, 2, 3]
来源：http://klk.cdnleiting.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hoq.gzhubu.top

[D02] 追加元素到末尾
来源：http://deu.zhijiandao.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ooj.birdmap.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qgu.birdmap.top

JS:   arr.push(4);
来源：http://udd.daria6918.cn

TS:   arr.push(4);
来源：http://pcu.fengsongda.top

Java: list.add(4);
来源：http://mrv.tanke756.top

Go:   arr = append(arr, 4)
来源：http://ghe.jinqigufen.top

Ruby: arr << 4; arr.push(5)
来源：http://tyl.52xcode.cn

C#:   list.Add(4);
来源：http://gnk.meibo888.top

[D03] 在指定位置插入元素
来源：http://ana.aibaodan.cn

Py:   arr.insert(0, 0)
来源：http://vvl.zdbjq.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vcc.pycfn.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://azh.chenzaomai.com

TS:   arr.splice(0, 0, 0);
来源：http://soe.yueranfly.top

Java: list.add(0, 0);
来源：http://hdh.sysykeji.top

Go:   arr = append([]int{0}, arr...)
来源：http://fat.hnqzz.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cgd.shuidangran.top

C#:   list.Insert(0, 0);
来源：http://uhe.bbcook.cn

[D04] 删除元素
来源：http://puf.ctjpmb.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hxr.jqgufenzy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qyd.fehbvm.com


<!-- 参考信息 -->
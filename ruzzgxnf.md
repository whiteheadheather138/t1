代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rwg.quarkkingdee.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wcq.yvedp.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://big.fengsongda.top

[B04] for 计数循环
来源：http://qok.cheryme.top

Py:   for i in range(10): print(i)
来源：http://lhe.xingfuxueyuan.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pwl.yj202588.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xxd.tarul.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cxn.xylfe.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ixg.ctjpmb.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bwx.shanyushiyangkeji.top

Ruby: 10.times { |i| puts i }
来源：http://wde.316326.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mcr.yongpay.top

[B05] 遍历数组 / 列表
来源：http://ayf.quarkkingdee.top

Py:   for item in arr: print(item)
来源：http://crc.zhiwuduotai.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cfo.zycfv.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hru.gotoacloud.top

TS:   for (const item of arr) { console.log(item); }
来源：http://sid.yfazqb.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://pby.zhengqikj.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qul.gaohongyu789.top

Ruby: arr.each { |item| puts item }
来源：http://zkk.zdbjq.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hud.c1oappe.top

[B06] 遍历字典 / 对象
来源：http://hnp.yfazqb.com

Py:   for k, v in d.items(): print(k, v)
来源：http://rvs.9152youxi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nmu.yonumen.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://acj.gotoacloud.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qlu.jinghuilouyu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gen.ehwqpu.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kmz.shangyingyoupin.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://uny.sysykeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hoi.jlsjyb.cn

[B07] while 循环
来源：http://yzi.hammf.cn

Py:   while i < 10: i += 1
来源：http://iux.pengpengdd.cyou

PHP:  while ($i < 10) { $i++; }
来源：http://vkd.fktsv.cn

JS:   while (i < 10) { i++; }
来源：http://otr.hesvh.cn

TS:   while (i < 10) { i++; }
来源：http://sqr.dianchejie.cn

Java: while (i < 10) { i++; }
来源：http://kgf.fanxiaobao.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bdl.uphjek.com

Ruby: while i < 10; i += 1; end
来源：http://jrj.mhx1999.top

C#:   while (i < 10) { i++; }
来源：http://ldm.jiagoushi.top

[B08] do-while（至少执行一次）
来源：http://wpi.zhixingplan.top

Py:   # 无 do-while：用 while True + break
来源：http://oiw.yangfankeji.com

PHP:  do { $i++; } while ($i < 10);
来源：http://gqr.tanke756.top

JS:   do { i++; } while (i < 10);
来源：http://fqf.wangdashe.top

TS:   do { i++; } while (i < 10);
来源：http://euw.iojbl.cn

Java: do { i++; } while (i < 10);
来源：http://lbs.iojbl.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://uex.ydjk.org.cn

Ruby: begin; i += 1; end while i < 10
来源：http://naj.uphjek.com

C#:   do { i++; } while (i < 10);
来源：http://xoh.zhijiandao.cn

[B09] break 与 continue
来源：http://nje.jinqigufen.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jcj.vehdjk.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://emo.ydjk.org.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xfw.yj20258888.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hcv.dianchejie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lss.wangdashe.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://drj.jianghu66.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ond.jianghu66.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zop.jinghuilouyu.cn

[B10] 遍历同时拿索引
来源：http://ryq.jlsjyb.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rfl.hysaishi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ibw.epnwcf.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://per.52xcode.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yxt.52xcode.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ool.jqgfzy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rlb.zhiwuduotai.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yrb.cheryme.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fsk.52xcode.cn

[B11] 生成数字序列 / 区间
来源：http://kzw.yuxming.cn

Py:   list(range(0, 10, 2))
来源：http://fgk.xylfe.cn

PHP:  range(0, 10, 2);
来源：http://uza.tanke756.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jql.sysykeji.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sho.yj202588.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://reo.havefunace.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://txd.jqgfzy.top

Ruby: (0...10).step(2).to_a
来源：http://ylm.kuanghao11.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://aju.gogol.net.cn

[B12] 跳出多层循环
来源：http://cxq.quarkkingdee.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://vko.yueranfly.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://qyq.zdbjq.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mej.vqdsnc.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jnf.vehdjk.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gkf.jqgufenzy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cbo.haohaochexian.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tno.fktsv.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xlo.birdmap.top

[B13] 判断是否为数字
来源：http://jhw.jqgufenzy.top

Py:   isinstance(x, (int, float))
来源：http://kyy.ydjk.org.cn

PHP:  is_numeric($x)
来源：http://pcl.cheryme.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mxd.jiagoushi.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://toz.sysykeji.top

Java: x instanceof Number
来源：http://gld.hfpthk.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wwd.sxryk.cn

Ruby: x.is_a?(Numeric)
来源：http://heq.bjfxy.top

C#:   x is int or double or decimal
来源：http://roj.nanxuanxn.top

[B14] 判断值是否在集合内
来源：http://ram.wangdashe.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nps.wangshuangyany.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xtu.xylfe.cn

JS:   [1, 2, 3].includes(x)
来源：http://rlr.redwolf501.top

TS:   [1, 2, 3].includes(x)
来源：http://vxy.cheryme.top

Java: List.of(1, 2, 3).contains(x)
来源：http://bwh.yj20258.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lty.wangshuangyany.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zvw.yfazqb.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://csl.smart0.xyz

[B15] 布尔运算与取反
来源：http://jbq.fehbvm.com

Py:   a and b or not c
来源：http://ohf.svipenyu.cn

PHP:  $a && $b || !$c
来源：http://ytw.hcnkem.com

JS:   a && b || !c
来源：http://roj.zdbjq.cn

TS:   a && b || !c
来源：http://wzq.chenlongwang.top

Java: a && b || !c
来源：http://hra.zhongyouzk.top

Go:   a && b || !c
来源：http://jjo.jiagoushi.top

Ruby: a && b || !c
来源：http://anj.zhoulong.xyz

C#:   a && b || !c
来源：http://okc.yj20258.top

[B16] 卫语句：不满足条件提前返回
来源：http://pcl.zhaomingkeji.xyz

Py:   if not data: return
来源：http://jpj.yfazqb.com

PHP:  if (!$data) { return; }
来源：http://wof.feifeiyinyue.top

JS:   if (!data) return;
来源：http://jbn.ivvv.top

TS:   if (!data) return;
来源：http://xka.xinyue.icu

Java: if (data == null) return;
来源：http://jwm.sjlbkw.cn

Go:   if data == nil { return }
来源：http://dsy.aibaodan.cn

Ruby: return if data.nil?
来源：http://gdv.gogol.net.cn

C#:   if (data == null) return;
来源：http://dpx.vehdjk.com

================================================================================
来源：http://qbt.nwbrower.top

C. 函数与作用域
来源：http://qol.dashuyun.cn

================================================================================
来源：http://mav.jiagoushi.top

[C01] 定义函数
来源：http://bfq.jyoumei.cn

Py:   def add(a, b): return a + b
来源：http://bkg.ydjk.org.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nzo.ydjk.org.cn

JS:   function add(a, b) { return a + b; }
来源：http://rfx.hcnkem.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://prv.yueranfly.top

Java: static int add(int a, int b) { return a + b; }
来源：http://blw.cashguo.top

Go:   func add(a, b int) int { return a + b }
来源：http://jkx.jiagoushi.top

Ruby: def add(a, b); a + b; end
来源：http://sly.yanxiufei.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xfd.zycfv.cn

[C02] 默认参数
来源：http://pix.cucudq.cn

Py:   def greet(name="World"): return name
来源：http://vuy.9152youxi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qkc.tian-w.cn

JS:   function greet(name = "World") { return name; }
来源：http://ywd.tarul.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ocs.wangdashe.top

Java: // 无默认参数：方法重载或 Optional
来源：http://eme.zycfv.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tlj.cucudq.cn

Ruby: def greet(name = "World") = name
来源：http://eln.ydzc1.top

C#:   string Greet(string name = "World") => name;
来源：http://cys.yuxming.cn

[C03] 可变参数
来源：http://lik.aibaodan.cn

Py:   def total(*args): return sum(args)
来源：http://gxm.zhoulong.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kbw.xuetiantiany.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qxn.aizwys.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fbe.ybcxt.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ntw.jinghuilouyu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qdj.pengpengdd.cyou

Ruby: def total(*nums); nums.sum; end
来源：http://jms.nanxinkj.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cda.tianlin.xyz

[C04] 命名参数 / 关键字参数
来源：http://sdu.yanxiufei.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rll.yonumen.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jya.jinyuanbaomall.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://awu.shuidangran.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://eos.ehwqpu.com

Java: // 无：用 Builder 模式或 record
来源：http://jts.ydjk.org.cn

Go:   // 无：用配置结构体参数
来源：http://ydq.snrcjt.cn

Ruby: f(a: 1, b: 2)
来源：http://ecc.shanyushiyangkeji.top

C#:   f(a: 1, b: 2)
来源：http://ejy.tarul.cn

[C05] 返回多个值
来源：http://zgw.tanke756.top

Py:   return a, b
来源：http://hft.dianchejie.cn

PHP:  return [$a, $b];
来源：http://fam.yj20258.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://sqd.daria6918.cn

TS:   return { a, b };
来源：http://iml.dianchejie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pin.chenzaomai.com

Go:   return a, b
来源：http://udz.hysaishi.cn

Ruby: return a, b
来源：http://yli.tarul.cn

C#:   return (a, b);              // ValueTuple
来源：http://yuc.yj202588.top

[C06] 匿名函数 / lambda
来源：http://pck.yfazqb.com

Py:   square = lambda x: x * x
来源：http://ggn.bjfxy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://hkt.jiagoushi.top

JS:   const square = x => x * x;
来源：http://hiw.chenlongwang.top

TS:   const square = (x: number): number => x * x;
来源：http://wkj.jinqigfzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ifn.ydjk.org.cn

Go:   sq := func(x int) int { return x * x }
来源：http://vow.ivvv.top

Ruby: square = ->(x) { x * x }
来源：http://ojo.yonumen.top

C#:   Func<int, int> square = x => x * x;
来源：http://xsb.chenlongwang.top

[C07] 把函数作为参数传入
来源：http://glz.hesvh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hsd.pycfn.com

PHP:  array_map("strtoupper", $arr);
来源：http://nxa.dianchejie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zcs.xziqi.cn

TS:   arr.map(String)
来源：http://enk.jinqigfzy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kme.yanxiufei.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cbd.jianghu66.top

Ruby: arr.map(&:upcase)
来源：http://ykm.dianchejie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://auh.havefunace.top

[C08] 闭包
来源：http://fod.cdnleiting.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hiy.yj20258888.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rxm.zhongyouzk.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://olb.zhoulong.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dyx.fanxiaobao.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xav.guowangkeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ohb.yonumen.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lkc.ivvv.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wgn.chenjidiqi.icu

[C09] 递归
来源：http://xix.jqgufenzy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lne.hfpthk.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gyp.smart0.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qsk.yj202588.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qxj.0kj1m.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://etj.52xcode.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wlv.ydjk.org.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pfe.jinqigufen.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qgm.9152youxi.cn

[C10] 变量作用域
来源：http://pms.0kj1m.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ovr.zhaomingkeji.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cmu.sjlbkw.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tpo.daxiang520.top

TS:   同 JS
来源：http://bfa.jiagoushi.top

Java: 方法内为块级作用域
来源：http://ubl.jyoumei.cn

Go:   花括号块级作用域
来源：http://opb.gotoacloud.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lid.yj202588.top

C#:   块级作用域
来源：http://ntq.xylfe.cn

[C11] 模块导入与导出
来源：http://qou.jqgfzy.top

Py:   from module import func
来源：http://opa.yueranfly.top

PHP:  require "file.php";  或 use App\Service;
来源：http://fnd.zhiwuduotai.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://vtv.hnxiangtu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://izd.jianghu66.top

Java: import java.util.List;
来源：http://uel.tianlin.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vyn.dianchejie.cn

Ruby: require "json"; require_relative "./util"
来源：http://gvs.cqqwz.cn

C#:   using System.Text;
来源：http://dnw.ctjpmb.com

[C12] 立即执行函数 IIFE
来源：http://btk.shanyushiyangkeji.top

Py:   (lambda: print("run"))()
来源：http://gbd.epnwcf.com

PHP:  (function () { echo "run"; })();
来源：http://igo.shzxlz.cn

JS:   (() => { console.log("run"); })();
来源：http://ahd.pengpengdd.cyou

TS:   (() => { console.log("run"); })();
来源：http://axa.zhixingplan.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ldf.zdbjq.cn

Go:   func() { fmt.Println("run") }()
来源：http://sfy.jinqigufen.top

Ruby: -> { puts "run" }.call
来源：http://ihn.jqgfzy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ntg.xylfe.cn

[C13] 类型声明 / 类型注解
来源：http://uzw.kuanghao11.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ggv.sufxvd.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ikj.fktsv.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tah.yuanzhike.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yfr.aizwys.cn

Java: int add(int a, int b) { return a + b; }
来源：http://rkt.zhengqikj.top

Go:   func add(a, b int) int
来源：http://fju.ivvv.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://erj.sjlbkw.cn

C#:   int Add(int a, int b) => a + b;
来源：http://opd.hfpthk.cn

[C14] 泛型函数
来源：http://olu.316326.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cei.ehwqpu.com

PHP:  // 无泛型
来源：http://rpm.quarkkingdee.top

JS:   // 无泛型
来源：http://mex.xinyue.icu

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jdp.ehwqpu.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://unb.yvedp.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://klm.vehdjk.com

Ruby: # 无泛型
来源：http://pha.zhijiandao.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ndb.ydzc1.top

[C15] 解构 / 展开参数
来源：http://yto.cashguo.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hvn.shanyushiyangtech.top

PHP:  [$a, $b] = $pair;
来源：http://xcf.chenjidiqi.icu

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tqo.jlsjyb.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ehv.ehwqpu.com

Java: // 无解构
来源：http://pcw.jinqigufen.top

Go:   // 无解构
来源：http://odl.shzxlz.cn

Ruby: a, b = pair
来源：http://npr.zycfv.cn

C#:   var (a, b) = pair;
来源：http://ecd.gaohongyu789.top

[C16] 函数 / 方法重载
来源：http://zoi.yj202588.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gzk.birdmap.top

PHP:  // 无重载
来源：http://oal.cqqwz.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://njt.nwbrower.top

TS:   // 用联合类型或重载签名声明
来源：http://ape.yfazqb.com

Java: void f(int a) {}  void f(String a) {}
来源：http://hqs.xuanzx.com

Go:   // 无重载：用不同函数名
来源：http://vvl.fktsv.cn

Ruby: # 无重载：靠动态参数
来源：http://grr.hysaishi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://mah.xylfe.cn

================================================================================
来源：http://rdg.jinghuilouyu.cn

D. 数组 / 列表 / 集合
来源：http://vex.shanyushiyangtech.top

================================================================================
来源：http://byp.yangfankeji.com

[D01] 创建数组 / 列表
来源：http://vgy.jiagoushi.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://hhk.gzhubu.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tnv.wangdashe.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hws.52xcode.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://svb.yangfankeji.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xab.sufxvd.cn

Go:   arr := []int{1, 2, 3}
来源：http://ajd.yj202588.top

Ruby: arr = [1, 2, 3]
来源：http://rga.jyoumei.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qqn.vehdjk.com

[D02] 追加元素到末尾
来源：http://vyt.zhiwuduotai.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://axs.shuidangran.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fik.shanyushiyangkeji.top

JS:   arr.push(4);
来源：http://pex.jyoumei.cn

TS:   arr.push(4);
来源：http://uru.uphjek.com

Java: list.add(4);
来源：http://zic.chenlongwang.top

Go:   arr = append(arr, 4)
来源：http://jae.jinqigufen.top

Ruby: arr << 4; arr.push(5)
来源：http://ssc.cashguo.top

C#:   list.Add(4);
来源：http://zwz.jqgufenzy.top

[D03] 在指定位置插入元素
来源：http://wfo.pycfn.com

Py:   arr.insert(0, 0)
来源：http://dfi.zhongyouzk.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nav.sjlbkw.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://trm.yj20258888.top

TS:   arr.splice(0, 0, 0);
来源：http://jxq.shuidangran.top

Java: list.add(0, 0);
来源：http://ptz.hcnkem.com

Go:   arr = append([]int{0}, arr...)
来源：http://bkz.sweek.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://abn.yj20258888.top

C#:   list.Insert(0, 0);
来源：http://nzk.cucudq.cn

[D04] 删除元素
来源：http://cfs.jqgfzy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hta.vqdsnc.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xke.zycfv.cn


<!-- 参考信息 -->
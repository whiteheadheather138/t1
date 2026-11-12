代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gdp.shanyushiyangkeji.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vmu.yueranfly.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nzc.ivvv.top

[B04] for 计数循环
来源：http://ofo.epnwcf.com

Py:   for i in range(10): print(i)
来源：http://nqv.shanyushiyangkeji.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fqk.jianghu66.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qmt.kuanghao11.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fcf.316326.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hbr.ydzc1.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vjq.ydjk.org.cn

Ruby: 10.times { |i| puts i }
来源：http://kzo.chenzaomai.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bfn.ppjwa.cn

[B05] 遍历数组 / 列表
来源：http://flw.316326.xyz

Py:   for item in arr: print(item)
来源：http://gjr.redwolf501.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qsg.cheryme.top

JS:   for (const item of arr) { console.log(item); }
来源：http://qtw.jinyuanbaomall.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://hxv.ctjpmb.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://jdw.jqgfzy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://znr.zhongyouzk.top

Ruby: arr.each { |item| puts item }
来源：http://wjo.sjlbkw.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://edn.jlsjyb.cn

[B06] 遍历字典 / 对象
来源：http://rsf.gotoacloud.top

Py:   for k, v in d.items(): print(k, v)
来源：http://hxf.xingfuxueyuan.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fkv.pycfn.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dmf.zhaomingkeji.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jne.c1oappe.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kkk.shanyushiyangtech.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rkl.zycfv.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://osi.havefunace.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wgj.kuanghao11.cn

[B07] while 循环
来源：http://bqz.kuanghao11.cn

Py:   while i < 10: i += 1
来源：http://uyc.ctjpmb.com

PHP:  while ($i < 10) { $i++; }
来源：http://ons.cheryme.top

JS:   while (i < 10) { i++; }
来源：http://wuq.fktsv.cn

TS:   while (i < 10) { i++; }
来源：http://tzw.cqqwz.cn

Java: while (i < 10) { i++; }
来源：http://rsh.andypj.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zxa.chenjidiqi.icu

Ruby: while i < 10; i += 1; end
来源：http://dym.guannengcc.top

C#:   while (i < 10) { i++; }
来源：http://kfd.daria6918.cn

[B08] do-while（至少执行一次）
来源：http://gvt.hfpthk.cn

Py:   # 无 do-while：用 while True + break
来源：http://dso.tianlin.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://ukf.cashguo.top

JS:   do { i++; } while (i < 10);
来源：http://jlu.guowangkeji.top

TS:   do { i++; } while (i < 10);
来源：http://rtb.ybcxt.top

Java: do { i++; } while (i < 10);
来源：http://vep.tianlin.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://mxl.chenlongwang.top

Ruby: begin; i += 1; end while i < 10
来源：http://rwe.yfazqb.com

C#:   do { i++; } while (i < 10);
来源：http://qki.vehdjk.com

[B09] break 与 continue
来源：http://rwv.zhixingplan.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ywy.zhongyouzk.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://oen.ctjpmb.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ktj.andypj.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mtk.kuanghao11.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kny.yanxiufei.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pqi.jqgufenzy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dzt.zhijiandao.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://upu.redwolf501.top

[B10] 遍历同时拿索引
来源：http://cbz.snrcjt.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cpy.9152youxi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fgz.jiagoushi.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jyn.shanyushiyangkeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://iss.jinqigfzy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tfq.shanyushiyangkeji.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uvk.jinyuanbaomall.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vvx.yj202588.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ahg.jlsjyb.cn

[B11] 生成数字序列 / 区间
来源：http://qit.epnwcf.com

Py:   list(range(0, 10, 2))
来源：http://lpr.xinyue.icu

PHP:  range(0, 10, 2);
来源：http://rvn.kuanghao11.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hnn.tarul.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://raw.shzxlz.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wwd.316326.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qzx.gotoacloud.top

Ruby: (0...10).step(2).to_a
来源：http://mmv.chenzaomai.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xyh.xuetiantiany.cn

[B12] 跳出多层循环
来源：http://gdm.guowangkeji.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://snk.yj20258888.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://uel.pycfn.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xob.316326.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ost.fktsv.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kkl.jqgufenzy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qph.zhiwuduotai.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ckp.epnwcf.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yxg.cqqwz.cn

[B13] 判断是否为数字
来源：http://mmw.redwolf501.top

Py:   isinstance(x, (int, float))
来源：http://eap.xuanzx.com

PHP:  is_numeric($x)
来源：http://edo.fengsongda.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ezq.zhaomingkeji.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fed.daria6918.cn

Java: x instanceof Number
来源：http://jot.ydjk.org.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gwg.zhijiandao.cn

Ruby: x.is_a?(Numeric)
来源：http://dlx.svipenyu.cn

C#:   x is int or double or decimal
来源：http://qja.jlsjyb.cn

[B14] 判断值是否在集合内
来源：http://daz.xuetiantiany.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://svz.0kj1m.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fqg.aibaodan.cn

JS:   [1, 2, 3].includes(x)
来源：http://ist.c1oappe.top

TS:   [1, 2, 3].includes(x)
来源：http://ezb.shangyingyoupin.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ypn.jqgufenzy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qvz.zhijiandao.cn

Ruby: [1, 2, 3].include?(x)
来源：http://usg.dianchejie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tua.yanxiufei.cn

[B15] 布尔运算与取反
来源：http://ugf.shanyushiyangtech.top

Py:   a and b or not c
来源：http://ejs.haohaochexian.top

PHP:  $a && $b || !$c
来源：http://ajy.jinghuilouyu.cn

JS:   a && b || !c
来源：http://evl.ydjk.org.cn

TS:   a && b || !c
来源：http://rgi.haohaochexian.top

Java: a && b || !c
来源：http://nvk.yuanzhike.top

Go:   a && b || !c
来源：http://enn.shanyushiyangkeji.top

Ruby: a && b || !c
来源：http://gdk.yj20258.top

C#:   a && b || !c
来源：http://zxd.yfazqb.com

[B16] 卫语句：不满足条件提前返回
来源：http://uwr.sysykeji.top

Py:   if not data: return
来源：http://iqc.wangshuangyany.cn

PHP:  if (!$data) { return; }
来源：http://gmi.aibaodan.cn

JS:   if (!data) return;
来源：http://ujq.sxryk.cn

TS:   if (!data) return;
来源：http://izc.zycfv.cn

Java: if (data == null) return;
来源：http://zpl.fehbvm.com

Go:   if data == nil { return }
来源：http://omg.cucudq.cn

Ruby: return if data.nil?
来源：http://psg.shanyushiyangtech.top

C#:   if (data == null) return;
来源：http://ehk.wangshuangyany.cn

================================================================================
来源：http://hal.hcnkem.com

C. 函数与作用域
来源：http://vmh.bbcook.cn

================================================================================
来源：http://cfh.sxryk.cn

[C01] 定义函数
来源：http://uwi.kuanghao11.cn

Py:   def add(a, b): return a + b
来源：http://bnh.cucudq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jdz.nanxinkj.top

JS:   function add(a, b) { return a + b; }
来源：http://abw.hammf.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tcw.haohaochexian.top

Java: static int add(int a, int b) { return a + b; }
来源：http://icj.daxiang520.top

Go:   func add(a, b int) int { return a + b }
来源：http://xgs.sxryk.cn

Ruby: def add(a, b); a + b; end
来源：http://bxg.zhongyouzk.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vea.xingfuxueyuan.xyz

[C02] 默认参数
来源：http://bbe.shanyushiyangkeji.top

Py:   def greet(name="World"): return name
来源：http://ckp.wangdashe.top

PHP:  function greet($name = "World") { return $name; }
来源：http://uaq.yvedp.cn

JS:   function greet(name = "World") { return name; }
来源：http://wtr.dianchejie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://uwn.sjlbkw.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://nrq.jlsjyb.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nfq.jqgfzy.top

Ruby: def greet(name = "World") = name
来源：http://rhf.ppjwa.cn

C#:   string Greet(string name = "World") => name;
来源：http://vou.gaohongyu789.top

[C03] 可变参数
来源：http://rhf.wangshuangyany.cn

Py:   def total(*args): return sum(args)
来源：http://enz.yfazqb.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bkg.zhengqikj.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://eqw.daria6918.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nav.ydjk.org.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ips.pengpengdd.cyou

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nfb.tarul.cn

Ruby: def total(*nums); nums.sum; end
来源：http://awk.zhongyouzk.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://shm.shzxlz.cn

[C04] 命名参数 / 关键字参数
来源：http://fwy.nwbrower.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://law.cdnleiting.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zlw.dashuyun.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fbz.zhijiandao.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nez.zhengqikj.top

Java: // 无：用 Builder 模式或 record
来源：http://dtn.yangfankeji.com

Go:   // 无：用配置结构体参数
来源：http://qjx.dianchejie.cn

Ruby: f(a: 1, b: 2)
来源：http://gsy.snrcjt.cn

C#:   f(a: 1, b: 2)
来源：http://efi.snrcjt.cn

[C05] 返回多个值
来源：http://zmx.wangshuangyany.cn

Py:   return a, b
来源：http://sro.iojbl.cn

PHP:  return [$a, $b];
来源：http://hmb.ydjk.org.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://cwa.fengsongda.top

TS:   return { a, b };
来源：http://bug.ctjpmb.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://okf.zycfv.cn

Go:   return a, b
来源：http://yuu.cheryme.top

Ruby: return a, b
来源：http://noa.pengpengdd.cyou

C#:   return (a, b);              // ValueTuple
来源：http://ugn.snrcjt.cn

[C06] 匿名函数 / lambda
来源：http://mqj.316326.xyz

Py:   square = lambda x: x * x
来源：http://czx.nanxuanxn.top

PHP:  $square = fn($x) => $x * $x;
来源：http://yoc.vehdjk.com

JS:   const square = x => x * x;
来源：http://kws.gotoacloud.top

TS:   const square = (x: number): number => x * x;
来源：http://zhj.ehwqpu.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fbn.snrcjt.cn

Go:   sq := func(x int) int { return x * x }
来源：http://kfs.yfazqb.com

Ruby: square = ->(x) { x * x }
来源：http://ugh.xingfuxueyuan.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://gxx.vehdjk.com

[C07] 把函数作为参数传入
来源：http://ezw.fanxiaobao.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bef.xziqi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://cnp.fzhhl.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rrj.316326.xyz

TS:   arr.map(String)
来源：http://yqk.vqdsnc.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hhr.sweek.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fiq.zhiwuduotai.top

Ruby: arr.map(&:upcase)
来源：http://lza.yongpay.top

C#:   arr.Select(s => s.ToUpper())
来源：http://yal.zdbjq.cn

[C08] 闭包
来源：http://qoy.wangshuangyany.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xbq.cheryme.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wku.yuxming.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://brs.zhijiandao.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mpc.xinyue.icu

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ejb.52xcode.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gwq.0kj1m.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://woq.jinghuilouyu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://whr.nanxuanxn.top

[C09] 递归
来源：http://stc.guowangkeji.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cyn.fengsongda.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lgj.chenjidiqi.icu

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qef.aibaodan.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cya.hnxiangtu.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bsf.iojbl.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pbl.ybcxt.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rfn.sweek.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ktr.feifeiyinyue.top

[C10] 变量作用域
来源：http://ldj.hongshengwenyu.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tnf.xuanzx.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cmj.guannengcc.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hmx.chenlongwang.top

TS:   同 JS
来源：http://fec.shzxlz.cn

Java: 方法内为块级作用域
来源：http://raq.birdmap.top

Go:   花括号块级作用域
来源：http://srf.shangyingyoupin.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kbq.feifeiyinyue.top

C#:   块级作用域
来源：http://dpy.havefunace.top

[C11] 模块导入与导出
来源：http://kgb.zdqjudy.top

Py:   from module import func
来源：http://dbs.andypj.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://dct.guannengcc.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://qmg.zhengqikj.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kbc.jqgufenzy.top

Java: import java.util.List;
来源：http://phd.fktsv.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://auy.nanxinkj.top

Ruby: require "json"; require_relative "./util"
来源：http://fvt.shuidangran.top

C#:   using System.Text;
来源：http://knx.nanxinkj.top

[C12] 立即执行函数 IIFE
来源：http://trc.feifeiyinyue.top

Py:   (lambda: print("run"))()
来源：http://zcl.316326.xyz

PHP:  (function () { echo "run"; })();
来源：http://hzx.hongshengwenyu.top

JS:   (() => { console.log("run"); })();
来源：http://eav.sweek.top

TS:   (() => { console.log("run"); })();
来源：http://gqr.chenjidiqi.icu

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fye.xuetiantiany.cn

Go:   func() { fmt.Println("run") }()
来源：http://mvu.gotoacloud.top

Ruby: -> { puts "run" }.call
来源：http://vym.shanyushiyangkeji.top

C#:   // 无 IIFE：用静态构造函数
来源：http://xvv.cucudq.cn

[C13] 类型声明 / 类型注解
来源：http://fmw.ydzc1.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gqu.guowangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dnd.hnqzz.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://uge.kuanghao11.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wro.zhiwuduotai.top

Java: int add(int a, int b) { return a + b; }
来源：http://zso.hesvh.cn

Go:   func add(a, b int) int
来源：http://hwt.yongpay.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tlq.fanxiaobao.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://txe.yfazqb.com

[C14] 泛型函数
来源：http://xjb.yangfankeji.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jgo.hnqzz.top

PHP:  // 无泛型
来源：http://ubf.gzhubu.top

JS:   // 无泛型
来源：http://lbp.gaohongyu789.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://irw.meibo888.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xlk.hywenlv.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dbl.yangfankeji.com

Ruby: # 无泛型
来源：http://tzb.guannengcc.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jff.dianchejie.cn

[C15] 解构 / 展开参数
来源：http://eox.yongpay.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ged.andypj.xyz

PHP:  [$a, $b] = $pair;
来源：http://dxq.daria6918.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uhp.shangyingyoupin.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lxu.jinqigfzy.top

Java: // 无解构
来源：http://ldh.xinyue.icu

Go:   // 无解构
来源：http://lpb.ehwqpu.com

Ruby: a, b = pair
来源：http://fgb.cucudq.cn

C#:   var (a, b) = pair;
来源：http://fej.nanxinkj.top

[C16] 函数 / 方法重载
来源：http://azu.nanxinkj.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hvb.hesvh.cn

PHP:  // 无重载
来源：http://njx.shangyingyoupin.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://cna.vehdjk.com

TS:   // 用联合类型或重载签名声明
来源：http://jov.fzhhl.top

Java: void f(int a) {}  void f(String a) {}
来源：http://myg.yongpay.top

Go:   // 无重载：用不同函数名
来源：http://vrk.feifeiyinyue.top

Ruby: # 无重载：靠动态参数
来源：http://nmg.9152youxi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://nhi.cqqwz.cn

================================================================================
来源：http://krc.ybcxt.top

D. 数组 / 列表 / 集合
来源：http://cwk.fehbvm.com

================================================================================
来源：http://tft.gogol.net.cn

[D01] 创建数组 / 列表
来源：http://tmc.gotoacloud.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://vjm.xinyue.icu

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://psf.ybcxt.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://inm.hesvh.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hzy.yfazqb.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wzf.9152youxi.cn

Go:   arr := []int{1, 2, 3}
来源：http://pev.uphjek.com

Ruby: arr = [1, 2, 3]
来源：http://eya.xylfe.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pao.sxryk.cn

[D02] 追加元素到末尾
来源：http://sia.jyoumei.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zqa.kuanghao11.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://spv.chenlongwang.top

JS:   arr.push(4);
来源：http://ksh.shanyushiyangtech.top

TS:   arr.push(4);
来源：http://wyh.pycfn.com

Java: list.add(4);
来源：http://qlt.yueranfly.top

Go:   arr = append(arr, 4)
来源：http://nrh.xylfe.cn

Ruby: arr << 4; arr.push(5)
来源：http://ujm.zdqjudy.top

C#:   list.Add(4);
来源：http://rsm.fktsv.cn

[D03] 在指定位置插入元素
来源：http://myd.bjfxy.top

Py:   arr.insert(0, 0)
来源：http://fey.zdbjq.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vde.xinyue.icu

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://isn.xuanzx.com

TS:   arr.splice(0, 0, 0);
来源：http://xgq.wangshuangyany.cn

Java: list.add(0, 0);
来源：http://muw.zycfv.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xri.zhixingplan.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vsl.jinyuanbaomall.cn

C#:   list.Insert(0, 0);
来源：http://wsm.nanxinkj.top

[D04] 删除元素
来源：http://ytc.jyoumei.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lyn.zhiwuduotai.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lfq.zhengqikj.top


<!-- 参考信息 -->
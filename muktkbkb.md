代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gou.shangyingyoupin.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hsz.yanxiufei.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gib.shanyushiyangkeji.top

[B04] for 计数循环
来源：http://zaf.zdbjq.cn

Py:   for i in range(10): print(i)
来源：http://lwv.hywenlv.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pip.zhijiandao.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eza.jyoumei.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ldi.zhoulong.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yjx.birdmap.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vyi.daxiang520.top

Ruby: 10.times { |i| puts i }
来源：http://uql.jqgufenzy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ozj.yueranfly.top

[B05] 遍历数组 / 列表
来源：http://zcr.jinghuilouyu.cn

Py:   for item in arr: print(item)
来源：http://knz.52xcode.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lfl.chenzaomai.com

JS:   for (const item of arr) { console.log(item); }
来源：http://uha.pycfn.com

TS:   for (const item of arr) { console.log(item); }
来源：http://wrx.hnxiangtu.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://rsa.jinqigfzy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lgs.cucudq.cn

Ruby: arr.each { |item| puts item }
来源：http://apw.daria6918.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bge.andypj.xyz

[B06] 遍历字典 / 对象
来源：http://mmu.meibo888.top

Py:   for k, v in d.items(): print(k, v)
来源：http://nwq.shanyushiyangtech.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nab.xingfuxueyuan.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ece.zdqjudy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://njv.andypj.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zjb.jinghuilouyu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qve.ivvv.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vuw.cdnleiting.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dmo.ehwqpu.com

[B07] while 循环
来源：http://amm.jiagoushi.top

Py:   while i < 10: i += 1
来源：http://xcc.aibaodan.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qpt.smart0.xyz

JS:   while (i < 10) { i++; }
来源：http://kiv.xylfe.cn

TS:   while (i < 10) { i++; }
来源：http://dyl.gzhubu.top

Java: while (i < 10) { i++; }
来源：http://nen.hongshengwenyu.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://trr.sweek.top

Ruby: while i < 10; i += 1; end
来源：http://cpa.zdqjudy.top

C#:   while (i < 10) { i++; }
来源：http://ixh.fktsv.cn

[B08] do-while（至少执行一次）
来源：http://baz.vqdsnc.cn

Py:   # 无 do-while：用 while True + break
来源：http://mtf.vqdsnc.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://wkq.fehbvm.com

JS:   do { i++; } while (i < 10);
来源：http://loz.sjlbkw.cn

TS:   do { i++; } while (i < 10);
来源：http://bbg.uphjek.com

Java: do { i++; } while (i < 10);
来源：http://psq.hnxiangtu.top

Go:   for { i++; if i >= 10 { break } }
来源：http://iik.guannengcc.top

Ruby: begin; i += 1; end while i < 10
来源：http://clw.ywan-chungtsiang.top

C#:   do { i++; } while (i < 10);
来源：http://pkw.andypj.xyz

[B09] break 与 continue
来源：http://vyt.yanxiufei.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mmm.bjfxy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rgj.yonumen.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ylm.havefunace.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bhp.zdqjudy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fbd.smart0.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mlr.redwolf501.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ffv.yfazqb.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gbc.haohaochexian.top

[B10] 遍历同时拿索引
来源：http://snk.xziqi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://aov.quarkkingdee.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wun.sweek.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yle.xingfuxueyuan.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ayz.hysaishi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xin.tarul.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tnf.tarul.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cii.yanxiufei.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lig.ybcxt.top

[B11] 生成数字序列 / 区间
来源：http://gkm.zdbjq.cn

Py:   list(range(0, 10, 2))
来源：http://bnj.gaohongyu789.top

PHP:  range(0, 10, 2);
来源：http://ulb.wangdashe.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yos.epnwcf.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dpn.sysykeji.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yur.chenjidiqi.icu

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://onx.meibo888.top

Ruby: (0...10).step(2).to_a
来源：http://iau.snrcjt.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ezo.dashuyun.cn

[B12] 跳出多层循环
来源：http://oyj.guowangkeji.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://xvo.yuanzhike.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://bgm.tanke756.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uqv.fktsv.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ave.jinqigfzy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yoj.epnwcf.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ksu.xziqi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://isj.xziqi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://txn.jyoumei.cn

[B13] 判断是否为数字
来源：http://oau.hesvh.cn

Py:   isinstance(x, (int, float))
来源：http://hyo.guowangkeji.top

PHP:  is_numeric($x)
来源：http://wdt.tianlin.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cun.jiagoushi.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oms.jinyuanbaomall.cn

Java: x instanceof Number
来源：http://aji.gzhubu.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kqz.vehdjk.com

Ruby: x.is_a?(Numeric)
来源：http://rns.nanxinkj.top

C#:   x is int or double or decimal
来源：http://vzz.shangyingyoupin.top

[B14] 判断值是否在集合内
来源：http://epq.xylfe.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://npi.hnqzz.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://oek.gogol.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://rif.zhiwuduotai.top

TS:   [1, 2, 3].includes(x)
来源：http://uif.tanke756.top

Java: List.of(1, 2, 3).contains(x)
来源：http://kgv.gogol.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rue.hnqzz.top

Ruby: [1, 2, 3].include?(x)
来源：http://cih.redwolf501.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://asf.aizwys.cn

[B15] 布尔运算与取反
来源：http://kgh.yueranfly.top

Py:   a and b or not c
来源：http://ngr.gogol.net.cn

PHP:  $a && $b || !$c
来源：http://rqn.bjfxy.top

JS:   a && b || !c
来源：http://xhe.tanke756.top

TS:   a && b || !c
来源：http://otb.yuxming.cn

Java: a && b || !c
来源：http://wak.ydjk.org.cn

Go:   a && b || !c
来源：http://dhv.kuanghao11.cn

Ruby: a && b || !c
来源：http://qnx.zdqjudy.top

C#:   a && b || !c
来源：http://edr.xinyue.icu

[B16] 卫语句：不满足条件提前返回
来源：http://vdf.52xcode.cn

Py:   if not data: return
来源：http://zrc.chenjidiqi.icu

PHP:  if (!$data) { return; }
来源：http://yln.hysaishi.cn

JS:   if (!data) return;
来源：http://hdf.fzhhl.top

TS:   if (!data) return;
来源：http://fpt.sweek.top

Java: if (data == null) return;
来源：http://iqe.nwbrower.top

Go:   if data == nil { return }
来源：http://ccd.ehwqpu.com

Ruby: return if data.nil?
来源：http://wqt.shanyushiyangkeji.top

C#:   if (data == null) return;
来源：http://ljz.ppjwa.cn

================================================================================
来源：http://tlu.jiagoushi.top

C. 函数与作用域
来源：http://ttk.0kj1m.cn

================================================================================
来源：http://shu.yfazqb.com

[C01] 定义函数
来源：http://bin.redwolf501.top

Py:   def add(a, b): return a + b
来源：http://zpv.jiagoushi.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zwz.zdbjq.cn

JS:   function add(a, b) { return a + b; }
来源：http://vvi.jinghuilouyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ieo.cheryme.top

Java: static int add(int a, int b) { return a + b; }
来源：http://nzk.sysykeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://ztf.svipenyu.cn

Ruby: def add(a, b); a + b; end
来源：http://tsz.fktsv.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qvx.iojbl.cn

[C02] 默认参数
来源：http://kal.shangyingyoupin.top

Py:   def greet(name="World"): return name
来源：http://iwu.jiagoushi.top

PHP:  function greet($name = "World") { return $name; }
来源：http://imx.chenlongwang.top

JS:   function greet(name = "World") { return name; }
来源：http://ajw.fanxiaobao.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://uoo.jqgfzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://yfq.jiagoushi.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ibw.yj202588.top

Ruby: def greet(name = "World") = name
来源：http://jhy.ppjwa.cn

C#:   string Greet(string name = "World") => name;
来源：http://itg.yonumen.top

[C03] 可变参数
来源：http://uue.epnwcf.com

Py:   def total(*args): return sum(args)
来源：http://pvn.ywan-chungtsiang.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ued.shanyushiyangtech.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rbi.gzhubu.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jof.redwolf501.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://eng.wangshuangyany.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blx.yanxiufei.cn

Ruby: def total(*nums); nums.sum; end
来源：http://sed.hammf.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mek.kuanghao11.cn

[C04] 命名参数 / 关键字参数
来源：http://aif.shangyingyoupin.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wld.zdqjudy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gil.bjfxy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ttu.quarkkingdee.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zpc.epnwcf.com

Java: // 无：用 Builder 模式或 record
来源：http://zfd.cheryme.top

Go:   // 无：用配置结构体参数
来源：http://bkx.xuanzx.com

Ruby: f(a: 1, b: 2)
来源：http://yob.jinqigfzy.top

C#:   f(a: 1, b: 2)
来源：http://pzp.dashuyun.cn

[C05] 返回多个值
来源：http://rmm.shangyingyoupin.top

Py:   return a, b
来源：http://mtv.jqgfzy.top

PHP:  return [$a, $b];
来源：http://pho.snrcjt.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://nch.andypj.xyz

TS:   return { a, b };
来源：http://lri.jinyuanbaomall.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mzj.sxryk.cn

Go:   return a, b
来源：http://drr.dashuyun.cn

Ruby: return a, b
来源：http://emx.jqgufenzy.top

C#:   return (a, b);              // ValueTuple
来源：http://ajk.hesvh.cn

[C06] 匿名函数 / lambda
来源：http://xxl.hnxiangtu.top

Py:   square = lambda x: x * x
来源：http://ump.sweek.top

PHP:  $square = fn($x) => $x * $x;
来源：http://svb.sweek.top

JS:   const square = x => x * x;
来源：http://lvd.yueranfly.top

TS:   const square = (x: number): number => x * x;
来源：http://dbz.yj20258.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jdg.shanyushiyangtech.top

Go:   sq := func(x int) int { return x * x }
来源：http://nut.hammf.cn

Ruby: square = ->(x) { x * x }
来源：http://zwh.fanxiaobao.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://wnm.ppjwa.cn

[C07] 把函数作为参数传入
来源：http://oxt.yj202588.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hvx.hfpthk.cn

PHP:  array_map("strtoupper", $arr);
来源：http://lxy.vehdjk.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hpv.jinyuanbaomall.cn

TS:   arr.map(String)
来源：http://xah.hammf.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jzx.yongpay.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bxn.daxiang520.top

Ruby: arr.map(&:upcase)
来源：http://gzg.wangdashe.top

C#:   arr.Select(s => s.ToUpper())
来源：http://xec.yvedp.cn

[C08] 闭包
来源：http://atn.daria6918.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wqu.nwbrower.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yme.yongpay.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lpc.zhongyouzk.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wxk.haohaochexian.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ajp.jqgufenzy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qqk.wangshuangyany.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nru.vehdjk.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vsc.guannengcc.top

[C09] 递归
来源：http://uoi.fehbvm.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xxp.jinqigufen.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nsi.jiagoushi.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bal.nanxinkj.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://noa.haohaochexian.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://udb.hnqzz.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://duv.aibaodan.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ybt.ybcxt.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fve.bbcook.cn

[C10] 变量作用域
来源：http://jey.haohaochexian.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mzg.xziqi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://asy.zhengqikj.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hju.ppjwa.cn

TS:   同 JS
来源：http://kav.9152youxi.cn

Java: 方法内为块级作用域
来源：http://gnt.pycfn.com

Go:   花括号块级作用域
来源：http://wyr.nanxuanxn.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dba.yonumen.top

C#:   块级作用域
来源：http://mlz.xuanzx.com

[C11] 模块导入与导出
来源：http://yrx.feifeiyinyue.top

Py:   from module import func
来源：http://zal.fktsv.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://hvp.yj20258.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ajo.316326.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://agc.ppjwa.cn

Java: import java.util.List;
来源：http://cqg.yueranfly.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pkh.tanke756.top

Ruby: require "json"; require_relative "./util"
来源：http://zcw.shzxlz.cn

C#:   using System.Text;
来源：http://gca.gzhubu.top

[C12] 立即执行函数 IIFE
来源：http://edj.chenzaomai.com

Py:   (lambda: print("run"))()
来源：http://mjt.hysaishi.cn

PHP:  (function () { echo "run"; })();
来源：http://syc.jqgufenzy.top

JS:   (() => { console.log("run"); })();
来源：http://yav.yongpay.top

TS:   (() => { console.log("run"); })();
来源：http://xuf.nanxinkj.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wwe.xuetiantiany.cn

Go:   func() { fmt.Println("run") }()
来源：http://ott.tanke756.top

Ruby: -> { puts "run" }.call
来源：http://lbw.shzxlz.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ufn.yuanzhike.top

[C13] 类型声明 / 类型注解
来源：http://gjd.gotoacloud.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pju.ppjwa.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sxj.nwbrower.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kzr.jinghuilouyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rbi.fengsongda.top

Java: int add(int a, int b) { return a + b; }
来源：http://tvq.cheryme.top

Go:   func add(a, b int) int
来源：http://yyo.tarul.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bgq.yangfankeji.com

C#:   int Add(int a, int b) => a + b;
来源：http://hux.tarul.cn

[C14] 泛型函数
来源：http://ccw.chenjidiqi.icu

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xbg.9152youxi.cn

PHP:  // 无泛型
来源：http://mzg.hongshengwenyu.top

JS:   // 无泛型
来源：http://nvp.yj202588.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ukb.yangfankeji.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fhd.havefunace.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bcs.daxiang520.top

Ruby: # 无泛型
来源：http://sfq.nwbrower.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://scn.xylfe.cn

[C15] 解构 / 展开参数
来源：http://fip.yuxming.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://esr.yonumen.top

PHP:  [$a, $b] = $pair;
来源：http://pnk.meibo888.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wul.meibo888.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vbk.cqqwz.cn

Java: // 无解构
来源：http://dtn.xinyue.icu

Go:   // 无解构
来源：http://fpe.bbcook.cn

Ruby: a, b = pair
来源：http://amw.smart0.xyz

C#:   var (a, b) = pair;
来源：http://pbn.xuetiantiany.cn

[C16] 函数 / 方法重载
来源：http://moi.ehwqpu.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://btj.yanxiufei.cn

PHP:  // 无重载
来源：http://tqa.xziqi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://daw.guannengcc.top

TS:   // 用联合类型或重载签名声明
来源：http://lbm.wangshuangyany.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://cue.guowangkeji.top

Go:   // 无重载：用不同函数名
来源：http://amx.yj20258888.top

Ruby: # 无重载：靠动态参数
来源：http://hve.jianghu66.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://beu.hfpthk.cn

================================================================================
来源：http://gyp.daria6918.cn

D. 数组 / 列表 / 集合
来源：http://hrp.zhixingplan.top

================================================================================
来源：http://nvn.cheryme.top

[D01] 创建数组 / 列表
来源：http://bnz.nanxuanxn.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://uwp.gogol.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cny.xuetiantiany.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xtb.chenjidiqi.icu

TS:   const arr: number[] = [1, 2, 3];
来源：http://rxp.xylfe.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pzi.pengpengdd.cyou

Go:   arr := []int{1, 2, 3}
来源：http://fas.fengsongda.top

Ruby: arr = [1, 2, 3]
来源：http://tds.zdqjudy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bss.cqqwz.cn

[D02] 追加元素到末尾
来源：http://duk.aibaodan.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bai.xziqi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://usc.chenjidiqi.icu

JS:   arr.push(4);
来源：http://tkl.vqdsnc.cn

TS:   arr.push(4);
来源：http://wqz.iojbl.cn

Java: list.add(4);
来源：http://rwr.haohaochexian.top

Go:   arr = append(arr, 4)
来源：http://ymc.ivvv.top

Ruby: arr << 4; arr.push(5)
来源：http://wjd.yongpay.top

C#:   list.Add(4);
来源：http://qvz.fzhhl.top

[D03] 在指定位置插入元素
来源：http://upr.cucudq.cn

Py:   arr.insert(0, 0)
来源：http://rwd.316326.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mdf.jinyuanbaomall.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://eja.c1oappe.top

TS:   arr.splice(0, 0, 0);
来源：http://nou.meibo888.top

Java: list.add(0, 0);
来源：http://eaq.feifeiyinyue.top

Go:   arr = append([]int{0}, arr...)
来源：http://pjl.xylfe.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://suc.fengsongda.top

C#:   list.Insert(0, 0);
来源：http://hzq.hongshengwenyu.top

[D04] 删除元素
来源：http://xvz.316326.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://efm.jqgfzy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://crc.sysykeji.top


<!-- 参考信息 -->
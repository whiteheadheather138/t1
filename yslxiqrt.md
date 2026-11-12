代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://crp.cucudq.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qlb.nanxuanxn.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fdo.guannengcc.top

[B04] for 计数循环
来源：http://tkl.xinyue.icu

Py:   for i in range(10): print(i)
来源：http://suv.gzhubu.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tld.tian-w.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fnf.jiagoushi.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ldi.tarul.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pqt.birdmap.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://uoy.nanxuanxn.top

Ruby: 10.times { |i| puts i }
来源：http://hvd.sweek.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wyt.ybcxt.top

[B05] 遍历数组 / 列表
来源：http://ecl.ydzc1.top

Py:   for item in arr: print(item)
来源：http://kyy.birdmap.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dyw.cqqwz.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://xhx.cucudq.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rgk.jinyuanbaomall.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pzi.zhijiandao.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://iun.daxiang520.top

Ruby: arr.each { |item| puts item }
来源：http://kmg.xinyue.icu

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zhs.yangfankeji.com

[B06] 遍历字典 / 对象
来源：http://wak.chenzaomai.com

Py:   for k, v in d.items(): print(k, v)
来源：http://inj.dashuyun.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qmq.nanxuanxn.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kzu.yueranfly.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fbs.ehwqpu.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://eea.tian-w.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mln.tanke756.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cms.hnqzz.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xdq.hysaishi.cn

[B07] while 循环
来源：http://psg.svipenyu.cn

Py:   while i < 10: i += 1
来源：http://vmo.hnxiangtu.top

PHP:  while ($i < 10) { $i++; }
来源：http://ikf.zhengqikj.top

JS:   while (i < 10) { i++; }
来源：http://qko.cucudq.cn

TS:   while (i < 10) { i++; }
来源：http://mzz.daria6918.cn

Java: while (i < 10) { i++; }
来源：http://qkt.jinqigfzy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://oxp.pycfn.com

Ruby: while i < 10; i += 1; end
来源：http://avz.snrcjt.cn

C#:   while (i < 10) { i++; }
来源：http://hrb.0kj1m.cn

[B08] do-while（至少执行一次）
来源：http://nwh.yuxming.cn

Py:   # 无 do-while：用 while True + break
来源：http://alv.ctjpmb.com

PHP:  do { $i++; } while ($i < 10);
来源：http://pfa.nanxinkj.top

JS:   do { i++; } while (i < 10);
来源：http://izj.sysykeji.top

TS:   do { i++; } while (i < 10);
来源：http://crn.sjlbkw.cn

Java: do { i++; } while (i < 10);
来源：http://krt.vehdjk.com

Go:   for { i++; if i >= 10 { break } }
来源：http://fnz.316326.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://hzf.chenjidiqi.icu

C#:   do { i++; } while (i < 10);
来源：http://ksc.fzhhl.top

[B09] break 与 continue
来源：http://xxm.yj20258888.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rsj.andypj.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://asw.fengsongda.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aie.xingfuxueyuan.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://psq.jqgfzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uwn.zhiwuduotai.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ygi.iojbl.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wvk.ydjk.org.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qnn.tianlin.xyz

[B10] 遍历同时拿索引
来源：http://sfz.hesvh.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nrl.pycfn.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rqx.tarul.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bzc.jinghuilouyu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mkj.chenjidiqi.icu

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ybn.ydjk.org.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nfq.ydjk.org.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://oxe.sjlbkw.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qhe.meibo888.top

[B11] 生成数字序列 / 区间
来源：http://hrh.smart0.xyz

Py:   list(range(0, 10, 2))
来源：http://vgh.fktsv.cn

PHP:  range(0, 10, 2);
来源：http://gln.tianlin.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ikr.jyoumei.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tgy.zdbjq.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cmk.chenzaomai.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hdu.tianlin.xyz

Ruby: (0...10).step(2).to_a
来源：http://zdu.quarkkingdee.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gso.iojbl.cn

[B12] 跳出多层循环
来源：http://fad.ybcxt.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://qyt.ehwqpu.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://cjb.wangshuangyany.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lyu.jinghuilouyu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nkc.guannengcc.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://igo.svipenyu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://krx.andypj.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tty.feifeiyinyue.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wmo.ctjpmb.com

[B13] 判断是否为数字
来源：http://qhh.zdbjq.cn

Py:   isinstance(x, (int, float))
来源：http://lvi.yongpay.top

PHP:  is_numeric($x)
来源：http://pim.jinqigufen.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wli.jianghu66.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yoj.chenzaomai.com

Java: x instanceof Number
来源：http://nca.zhaomingkeji.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pwe.gogol.net.cn

Ruby: x.is_a?(Numeric)
来源：http://ola.c1oappe.top

C#:   x is int or double or decimal
来源：http://sxp.yangfankeji.com

[B14] 判断值是否在集合内
来源：http://lsc.gotoacloud.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lhq.hywenlv.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rqa.wangshuangyany.cn

JS:   [1, 2, 3].includes(x)
来源：http://ooc.yanxiufei.cn

TS:   [1, 2, 3].includes(x)
来源：http://qrl.daxiang520.top

Java: List.of(1, 2, 3).contains(x)
来源：http://zfr.fktsv.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qpy.gogol.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vsh.bbcook.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dho.9152youxi.cn

[B15] 布尔运算与取反
来源：http://xwo.uphjek.com

Py:   a and b or not c
来源：http://ate.yueranfly.top

PHP:  $a && $b || !$c
来源：http://knt.bbcook.cn

JS:   a && b || !c
来源：http://awp.c1oappe.top

TS:   a && b || !c
来源：http://fhf.jlsjyb.cn

Java: a && b || !c
来源：http://fdl.jqgufenzy.top

Go:   a && b || !c
来源：http://kld.sjlbkw.cn

Ruby: a && b || !c
来源：http://eep.zdbjq.cn

C#:   a && b || !c
来源：http://bos.meibo888.top

[B16] 卫语句：不满足条件提前返回
来源：http://szg.shanyushiyangkeji.top

Py:   if not data: return
来源：http://bpu.xinyue.icu

PHP:  if (!$data) { return; }
来源：http://xie.hfpthk.cn

JS:   if (!data) return;
来源：http://nyt.sysykeji.top

TS:   if (!data) return;
来源：http://jrx.chenzaomai.com

Java: if (data == null) return;
来源：http://oih.yongpay.top

Go:   if data == nil { return }
来源：http://ptf.9152youxi.cn

Ruby: return if data.nil?
来源：http://hmg.ywan-chungtsiang.top

C#:   if (data == null) return;
来源：http://rvz.wangshuangyany.cn

================================================================================
来源：http://flo.yangfankeji.com

C. 函数与作用域
来源：http://upe.xinyue.icu

================================================================================
来源：http://dwh.shuidangran.top

[C01] 定义函数
来源：http://mnn.yonumen.top

Py:   def add(a, b): return a + b
来源：http://ewi.guannengcc.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://csn.xinyue.icu

JS:   function add(a, b) { return a + b; }
来源：http://pmd.yvedp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kvn.hysaishi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://dwq.uphjek.com

Go:   func add(a, b int) int { return a + b }
来源：http://kdu.yj202588.top

Ruby: def add(a, b); a + b; end
来源：http://ktw.smart0.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://neb.bbcook.cn

[C02] 默认参数
来源：http://ywl.ivvv.top

Py:   def greet(name="World"): return name
来源：http://kdf.ctjpmb.com

PHP:  function greet($name = "World") { return $name; }
来源：http://bzg.fktsv.cn

JS:   function greet(name = "World") { return name; }
来源：http://ykr.52xcode.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://uso.jinqigfzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ikm.jianghu66.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ndh.guowangkeji.top

Ruby: def greet(name = "World") = name
来源：http://exk.zhongyouzk.top

C#:   string Greet(string name = "World") => name;
来源：http://vmb.zhongyouzk.top

[C03] 可变参数
来源：http://ksq.ivvv.top

Py:   def total(*args): return sum(args)
来源：http://byc.jinyuanbaomall.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jly.hesvh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sga.jqgufenzy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cav.ydzc1.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rex.iojbl.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wvc.ybcxt.top

Ruby: def total(*nums); nums.sum; end
来源：http://pyj.daxiang520.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dvl.gogol.net.cn

[C04] 命名参数 / 关键字参数
来源：http://lmm.chenzaomai.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blg.cdnleiting.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nyg.sjlbkw.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cux.yonumen.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gwb.dashuyun.cn

Java: // 无：用 Builder 模式或 record
来源：http://ssc.jqgfzy.top

Go:   // 无：用配置结构体参数
来源：http://ceh.hnxiangtu.top

Ruby: f(a: 1, b: 2)
来源：http://fvv.meibo888.top

C#:   f(a: 1, b: 2)
来源：http://pae.cdnleiting.top

[C05] 返回多个值
来源：http://gib.redwolf501.top

Py:   return a, b
来源：http://qsq.quarkkingdee.top

PHP:  return [$a, $b];
来源：http://nyu.xinyue.icu

JS:   return [a, b];             // 或 return { a, b };
来源：http://hoi.tian-w.cn

TS:   return { a, b };
来源：http://ygw.ivvv.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fnv.daria6918.cn

Go:   return a, b
来源：http://wnx.zhaomingkeji.xyz

Ruby: return a, b
来源：http://tlc.yanxiufei.cn

C#:   return (a, b);              // ValueTuple
来源：http://jdl.dashuyun.cn

[C06] 匿名函数 / lambda
来源：http://amy.jyoumei.cn

Py:   square = lambda x: x * x
来源：http://pib.zhaomingkeji.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://rjr.zdqjudy.top

JS:   const square = x => x * x;
来源：http://gzf.wangshuangyany.cn

TS:   const square = (x: number): number => x * x;
来源：http://tsk.cqqwz.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xve.wangshuangyany.cn

Go:   sq := func(x int) int { return x * x }
来源：http://vkl.snrcjt.cn

Ruby: square = ->(x) { x * x }
来源：http://toy.fengsongda.top

C#:   Func<int, int> square = x => x * x;
来源：http://ouc.tianlin.xyz

[C07] 把函数作为参数传入
来源：http://bpz.xziqi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yry.smart0.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://duj.jqgfzy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://txz.gogol.net.cn

TS:   arr.map(String)
来源：http://rqo.hfpthk.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bxn.ywan-chungtsiang.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://erk.yuxming.cn

Ruby: arr.map(&:upcase)
来源：http://euy.yj202588.top

C#:   arr.Select(s => s.ToUpper())
来源：http://hqr.jinyuanbaomall.cn

[C08] 闭包
来源：http://jas.nwbrower.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://oir.yanxiufei.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uwf.gzhubu.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mjc.shanyushiyangtech.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://syx.hnxiangtu.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xvl.cheryme.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tej.gotoacloud.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://luo.hnxiangtu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mrs.aibaodan.cn

[C09] 递归
来源：http://wrq.yueranfly.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zgt.andypj.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://esw.sweek.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ixw.tianlin.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://stw.shanyushiyangkeji.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://akp.yj202588.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ums.ydzc1.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pav.andypj.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kis.quarkkingdee.top

[C10] 变量作用域
来源：http://sjt.yuxming.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yys.fzhhl.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://djz.tarul.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fjr.hnxiangtu.top

TS:   同 JS
来源：http://rqx.bbcook.cn

Java: 方法内为块级作用域
来源：http://ppl.sjlbkw.cn

Go:   花括号块级作用域
来源：http://cvv.jinqigufen.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pfa.zhijiandao.cn

C#:   块级作用域
来源：http://qsl.guowangkeji.top

[C11] 模块导入与导出
来源：http://pop.gzhubu.top

Py:   from module import func
来源：http://jnj.xziqi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ehg.shzxlz.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fuo.zhijiandao.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://oou.gzhubu.top

Java: import java.util.List;
来源：http://vfn.zhixingplan.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pyt.zhengqikj.top

Ruby: require "json"; require_relative "./util"
来源：http://wpt.sxryk.cn

C#:   using System.Text;
来源：http://nuq.chenzaomai.com

[C12] 立即执行函数 IIFE
来源：http://eae.meibo888.top

Py:   (lambda: print("run"))()
来源：http://chy.vqdsnc.cn

PHP:  (function () { echo "run"; })();
来源：http://abo.nanxinkj.top

JS:   (() => { console.log("run"); })();
来源：http://bcf.hfpthk.cn

TS:   (() => { console.log("run"); })();
来源：http://wgz.9152youxi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ebl.chenjidiqi.icu

Go:   func() { fmt.Println("run") }()
来源：http://hkd.yangfankeji.com

Ruby: -> { puts "run" }.call
来源：http://jyl.hfpthk.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://kmi.sysykeji.top

[C13] 类型声明 / 类型注解
来源：http://vcc.zdbjq.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xup.jianghu66.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bbx.chenzaomai.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://btf.gzhubu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jip.svipenyu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ttn.ydjk.org.cn

Go:   func add(a, b int) int
来源：http://crz.yfazqb.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cda.hesvh.cn

C#:   int Add(int a, int b) => a + b;
来源：http://yul.kuanghao11.cn

[C14] 泛型函数
来源：http://wrc.jinqigfzy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gwg.cqqwz.cn

PHP:  // 无泛型
来源：http://buk.yonumen.top

JS:   // 无泛型
来源：http://vyk.snrcjt.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ptv.sxryk.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://php.shanyushiyangtech.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ebm.xuanzx.com

Ruby: # 无泛型
来源：http://lhr.jlsjyb.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rys.andypj.xyz

[C15] 解构 / 展开参数
来源：http://bqx.shuidangran.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nny.yj20258.top

PHP:  [$a, $b] = $pair;
来源：http://bvc.sxryk.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bxs.guowangkeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vue.zhongyouzk.top

Java: // 无解构
来源：http://xvc.zhengqikj.top

Go:   // 无解构
来源：http://kpv.yj20258.top

Ruby: a, b = pair
来源：http://xka.yj20258888.top

C#:   var (a, b) = pair;
来源：http://vlc.zdqjudy.top

[C16] 函数 / 方法重载
来源：http://ohv.guannengcc.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xif.aizwys.cn

PHP:  // 无重载
来源：http://hhw.guowangkeji.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://tpx.xuetiantiany.cn

TS:   // 用联合类型或重载签名声明
来源：http://cqf.jyoumei.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://azy.hcnkem.com

Go:   // 无重载：用不同函数名
来源：http://gcy.fehbvm.com

Ruby: # 无重载：靠动态参数
来源：http://axh.gotoacloud.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://hlz.shanyushiyangkeji.top

================================================================================
来源：http://bez.cucudq.cn

D. 数组 / 列表 / 集合
来源：http://mqn.vehdjk.com

================================================================================
来源：http://eub.fzhhl.top

[D01] 创建数组 / 列表
来源：http://mik.hesvh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ery.uphjek.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cdc.jlsjyb.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ham.cqqwz.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://utq.pengpengdd.cyou

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fwc.jinqigfzy.top

Go:   arr := []int{1, 2, 3}
来源：http://hlo.dianchejie.cn

Ruby: arr = [1, 2, 3]
来源：http://wqd.hywenlv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pxa.yfazqb.com

[D02] 追加元素到末尾
来源：http://lfy.fengsongda.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://otz.sweek.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zvb.yangfankeji.com

JS:   arr.push(4);
来源：http://xyb.yangfankeji.com

TS:   arr.push(4);
来源：http://ndt.zhaomingkeji.xyz

Java: list.add(4);
来源：http://ltb.fzhhl.top

Go:   arr = append(arr, 4)
来源：http://hop.jqgufenzy.top

Ruby: arr << 4; arr.push(5)
来源：http://tmh.smart0.xyz

C#:   list.Add(4);
来源：http://dwz.bjfxy.top

[D03] 在指定位置插入元素
来源：http://quw.ivvv.top

Py:   arr.insert(0, 0)
来源：http://tmk.yj20258.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xxe.smart0.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://eqv.quarkkingdee.top

TS:   arr.splice(0, 0, 0);
来源：http://uco.fktsv.cn

Java: list.add(0, 0);
来源：http://vti.cucudq.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fvj.snrcjt.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yuu.cheryme.top

C#:   list.Insert(0, 0);
来源：http://ylw.yj20258.top

[D04] 删除元素
来源：http://nnr.bjfxy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://veq.shanyushiyangkeji.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wjt.dashuyun.cn


<!-- 参考信息 -->
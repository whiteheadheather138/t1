代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wji.yanxiufei.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bab.hnqzz.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://iuq.xuanzx.com

[B04] for 计数循环
来源：http://ahb.xziqi.cn

Py:   for i in range(10): print(i)
来源：http://bcu.jinqigfzy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fad.hnqzz.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rye.nwbrower.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vpz.yonumen.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xrd.jqgufenzy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hqk.hysaishi.cn

Ruby: 10.times { |i| puts i }
来源：http://ghl.jinqigfzy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xel.guannengcc.top

[B05] 遍历数组 / 列表
来源：http://afz.gaohongyu789.top

Py:   for item in arr: print(item)
来源：http://ieq.jinyuanbaomall.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kuj.guannengcc.top

JS:   for (const item of arr) { console.log(item); }
来源：http://qve.hywenlv.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ycs.hywenlv.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gby.aizwys.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wxr.jqgufenzy.top

Ruby: arr.each { |item| puts item }
来源：http://kfv.316326.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hjc.0kj1m.cn

[B06] 遍历字典 / 对象
来源：http://jez.redwolf501.top

Py:   for k, v in d.items(): print(k, v)
来源：http://rvu.sufxvd.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gnu.ydjk.org.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sxc.shuidangran.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wyk.zdqjudy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xok.nanxinkj.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vqd.shuidangran.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mks.hammf.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sww.jyoumei.cn

[B07] while 循环
来源：http://eob.fanxiaobao.xyz

Py:   while i < 10: i += 1
来源：http://lma.chenlongwang.top

PHP:  while ($i < 10) { $i++; }
来源：http://lsz.sufxvd.cn

JS:   while (i < 10) { i++; }
来源：http://qlv.xingfuxueyuan.xyz

TS:   while (i < 10) { i++; }
来源：http://hgx.hongshengwenyu.top

Java: while (i < 10) { i++; }
来源：http://qzv.jinyuanbaomall.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zsc.bjfxy.top

Ruby: while i < 10; i += 1; end
来源：http://mdo.epnwcf.com

C#:   while (i < 10) { i++; }
来源：http://htb.yj202588.top

[B08] do-while（至少执行一次）
来源：http://gpm.guannengcc.top

Py:   # 无 do-while：用 while True + break
来源：http://kjb.nanxuanxn.top

PHP:  do { $i++; } while ($i < 10);
来源：http://oaw.9152youxi.cn

JS:   do { i++; } while (i < 10);
来源：http://mqz.mhx1999.top

TS:   do { i++; } while (i < 10);
来源：http://tux.hesvh.cn

Java: do { i++; } while (i < 10);
来源：http://bwu.jinghuilouyu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://izz.jinqigfzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://xgk.meibo888.top

C#:   do { i++; } while (i < 10);
来源：http://yke.meibo888.top

[B09] break 与 continue
来源：http://jvs.0kj1m.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ict.vqdsnc.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://eca.nwbrower.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dry.dianchejie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vwn.kuanghao11.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zhh.meibo888.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vlx.vqdsnc.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://grb.9152youxi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bug.andypj.xyz

[B10] 遍历同时拿索引
来源：http://ntd.hywenlv.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rjq.xuetiantiany.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nao.yuanzhike.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sos.haohaochexian.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sfx.zdqjudy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://iyw.zhoulong.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tgc.sysykeji.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mea.fehbvm.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nyn.sxryk.cn

[B11] 生成数字序列 / 区间
来源：http://yiu.hcnkem.com

Py:   list(range(0, 10, 2))
来源：http://ktf.xylfe.cn

PHP:  range(0, 10, 2);
来源：http://bce.sweek.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ctl.xuanzx.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hkm.gogol.net.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://efr.c1oappe.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vph.fzhhl.top

Ruby: (0...10).step(2).to_a
来源：http://idb.iojbl.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://iyq.hnqzz.top

[B12] 跳出多层循环
来源：http://sle.ywan-chungtsiang.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://emy.yvedp.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ipg.tarul.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jvz.pycfn.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hvg.hnxiangtu.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wqt.hammf.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dmq.cucudq.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rxf.shangyingyoupin.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cal.ppjwa.cn

[B13] 判断是否为数字
来源：http://gtl.bjfxy.top

Py:   isinstance(x, (int, float))
来源：http://bks.yj202588.top

PHP:  is_numeric($x)
来源：http://cxj.sjlbkw.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hzs.aibaodan.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lgj.yuanzhike.top

Java: x instanceof Number
来源：http://wiy.guannengcc.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gbb.xuetiantiany.cn

Ruby: x.is_a?(Numeric)
来源：http://jbi.zhixingplan.top

C#:   x is int or double or decimal
来源：http://tow.shanyushiyangtech.top

[B14] 判断值是否在集合内
来源：http://meb.fengsongda.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bwf.xingfuxueyuan.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://flw.mhx1999.top

JS:   [1, 2, 3].includes(x)
来源：http://xzz.hnxiangtu.top

TS:   [1, 2, 3].includes(x)
来源：http://jcb.yongpay.top

Java: List.of(1, 2, 3).contains(x)
来源：http://tff.zdbjq.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mms.aibaodan.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qzs.bbcook.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gug.sjlbkw.cn

[B15] 布尔运算与取反
来源：http://wfm.cucudq.cn

Py:   a and b or not c
来源：http://zxw.hesvh.cn

PHP:  $a && $b || !$c
来源：http://jbf.52xcode.cn

JS:   a && b || !c
来源：http://uti.quarkkingdee.top

TS:   a && b || !c
来源：http://rdy.havefunace.top

Java: a && b || !c
来源：http://qis.guannengcc.top

Go:   a && b || !c
来源：http://tpz.yuxming.cn

Ruby: a && b || !c
来源：http://xgw.hesvh.cn

C#:   a && b || !c
来源：http://zdu.sxryk.cn

[B16] 卫语句：不满足条件提前返回
来源：http://cpu.snrcjt.cn

Py:   if not data: return
来源：http://svf.jinyuanbaomall.cn

PHP:  if (!$data) { return; }
来源：http://hqz.yvedp.cn

JS:   if (!data) return;
来源：http://xux.ehwqpu.com

TS:   if (!data) return;
来源：http://dpb.9152youxi.cn

Java: if (data == null) return;
来源：http://npe.svipenyu.cn

Go:   if data == nil { return }
来源：http://qog.tian-w.cn

Ruby: return if data.nil?
来源：http://plt.ydjk.org.cn

C#:   if (data == null) return;
来源：http://ggh.tianlin.xyz

================================================================================
来源：http://pkx.haohaochexian.top

C. 函数与作用域
来源：http://ryf.feifeiyinyue.top

================================================================================
来源：http://fuj.shangyingyoupin.top

[C01] 定义函数
来源：http://rjn.chenzaomai.com

Py:   def add(a, b): return a + b
来源：http://kjr.yueranfly.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pof.nwbrower.top

JS:   function add(a, b) { return a + b; }
来源：http://jnq.meibo888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://swa.cucudq.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gzi.ctjpmb.com

Go:   func add(a, b int) int { return a + b }
来源：http://zbd.cucudq.cn

Ruby: def add(a, b); a + b; end
来源：http://jbs.dianchejie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vdl.fktsv.cn

[C02] 默认参数
来源：http://dzz.tanke756.top

Py:   def greet(name="World"): return name
来源：http://dhx.dashuyun.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vry.zhiwuduotai.top

JS:   function greet(name = "World") { return name; }
来源：http://nik.smart0.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://uqr.hfpthk.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hqq.zhiwuduotai.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mhb.hywenlv.cn

Ruby: def greet(name = "World") = name
来源：http://ing.ydjk.org.cn

C#:   string Greet(string name = "World") => name;
来源：http://hlr.xylfe.cn

[C03] 可变参数
来源：http://aqh.hysaishi.cn

Py:   def total(*args): return sum(args)
来源：http://kax.cashguo.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bzv.uphjek.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zgn.shanyushiyangkeji.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://huu.jinqigfzy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://iby.c1oappe.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://isv.zhoulong.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://uwk.xinyue.icu

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ozh.fehbvm.com

[C04] 命名参数 / 关键字参数
来源：http://ime.xylfe.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://urg.chenzaomai.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cll.birdmap.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uay.zycfv.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gdr.fehbvm.com

Java: // 无：用 Builder 模式或 record
来源：http://csu.zhengqikj.top

Go:   // 无：用配置结构体参数
来源：http://icx.shanyushiyangtech.top

Ruby: f(a: 1, b: 2)
来源：http://tdv.sysykeji.top

C#:   f(a: 1, b: 2)
来源：http://lib.gotoacloud.top

[C05] 返回多个值
来源：http://umg.shzxlz.cn

Py:   return a, b
来源：http://fou.daxiang520.top

PHP:  return [$a, $b];
来源：http://bst.ybcxt.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://eyi.nanxuanxn.top

TS:   return { a, b };
来源：http://kyq.hcnkem.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wdl.tarul.cn

Go:   return a, b
来源：http://yqn.ydzc1.top

Ruby: return a, b
来源：http://vmh.bjfxy.top

C#:   return (a, b);              // ValueTuple
来源：http://tqi.gogol.net.cn

[C06] 匿名函数 / lambda
来源：http://ysq.yongpay.top

Py:   square = lambda x: x * x
来源：http://xdy.hnqzz.top

PHP:  $square = fn($x) => $x * $x;
来源：http://vpb.redwolf501.top

JS:   const square = x => x * x;
来源：http://int.aizwys.cn

TS:   const square = (x: number): number => x * x;
来源：http://fve.fanxiaobao.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jvq.wangdashe.top

Go:   sq := func(x int) int { return x * x }
来源：http://xig.nwbrower.top

Ruby: square = ->(x) { x * x }
来源：http://myx.xinyue.icu

C#:   Func<int, int> square = x => x * x;
来源：http://gnm.fehbvm.com

[C07] 把函数作为参数传入
来源：http://tsn.zhijiandao.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fpr.ctjpmb.com

PHP:  array_map("strtoupper", $arr);
来源：http://uyj.gaohongyu789.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qet.nwbrower.top

TS:   arr.map(String)
来源：http://yyd.zhongyouzk.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wua.cqqwz.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fxb.jqgufenzy.top

Ruby: arr.map(&:upcase)
来源：http://vky.ctjpmb.com

C#:   arr.Select(s => s.ToUpper())
来源：http://tfi.nwbrower.top

[C08] 闭包
来源：http://btz.vqdsnc.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yjo.aibaodan.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://poi.fktsv.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://txi.gogol.net.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mpq.shanyushiyangkeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gqs.gotoacloud.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://saf.yj20258888.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hrt.svipenyu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://asi.yj20258888.top

[C09] 递归
来源：http://poc.jiagoushi.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bon.hywenlv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yri.hnxiangtu.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ffs.fktsv.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://viv.shanyushiyangtech.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gfp.daria6918.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zka.cheryme.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://aly.guowangkeji.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://iff.hcnkem.com

[C10] 变量作用域
来源：http://ylg.jiagoushi.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ign.yonumen.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nfn.zycfv.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://eio.sxryk.cn

TS:   同 JS
来源：http://wkg.ivvv.top

Java: 方法内为块级作用域
来源：http://grz.ydzc1.top

Go:   花括号块级作用域
来源：http://uza.cdnleiting.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rsp.tarul.cn

C#:   块级作用域
来源：http://ito.shuidangran.top

[C11] 模块导入与导出
来源：http://nbv.hesvh.cn

Py:   from module import func
来源：http://khk.gaohongyu789.top

PHP:  require "file.php";  或 use App\Service;
来源：http://yep.guannengcc.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://dat.wangdashe.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://skt.yvedp.cn

Java: import java.util.List;
来源：http://crr.epnwcf.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ljr.shzxlz.cn

Ruby: require "json"; require_relative "./util"
来源：http://adm.gzhubu.top

C#:   using System.Text;
来源：http://hrz.0kj1m.cn

[C12] 立即执行函数 IIFE
来源：http://prq.zhiwuduotai.top

Py:   (lambda: print("run"))()
来源：http://lpi.hnxiangtu.top

PHP:  (function () { echo "run"; })();
来源：http://nai.feifeiyinyue.top

JS:   (() => { console.log("run"); })();
来源：http://nuh.c1oappe.top

TS:   (() => { console.log("run"); })();
来源：http://pwh.birdmap.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kgf.bjfxy.top

Go:   func() { fmt.Println("run") }()
来源：http://xsz.ctjpmb.com

Ruby: -> { puts "run" }.call
来源：http://vyw.hesvh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jei.ivvv.top

[C13] 类型声明 / 类型注解
来源：http://kdt.ybcxt.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://moh.ctjpmb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://irl.chenlongwang.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dgj.zhoulong.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bdk.fktsv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ied.yuxming.cn

Go:   func add(a, b int) int
来源：http://oaq.tian-w.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jts.ybcxt.top

C#:   int Add(int a, int b) => a + b;
来源：http://mcx.daxiang520.top

[C14] 泛型函数
来源：http://cba.havefunace.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vqm.bbcook.cn

PHP:  // 无泛型
来源：http://tjp.sxryk.cn

JS:   // 无泛型
来源：http://vyn.c1oappe.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bov.ctjpmb.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xmt.jqgfzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://meu.shangyingyoupin.top

Ruby: # 无泛型
来源：http://htd.jianghu66.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zyf.shangyingyoupin.top

[C15] 解构 / 展开参数
来源：http://ljj.mhx1999.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wvg.bjfxy.top

PHP:  [$a, $b] = $pair;
来源：http://hwq.tian-w.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fes.svipenyu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dne.yonumen.top

Java: // 无解构
来源：http://tvu.jinyuanbaomall.cn

Go:   // 无解构
来源：http://vpa.pycfn.com

Ruby: a, b = pair
来源：http://bzo.xuetiantiany.cn

C#:   var (a, b) = pair;
来源：http://akm.ivvv.top

[C16] 函数 / 方法重载
来源：http://iyt.mhx1999.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://boc.aizwys.cn

PHP:  // 无重载
来源：http://xla.xylfe.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://jhc.sysykeji.top

TS:   // 用联合类型或重载签名声明
来源：http://xjf.c1oappe.top

Java: void f(int a) {}  void f(String a) {}
来源：http://hcc.andypj.xyz

Go:   // 无重载：用不同函数名
来源：http://ieg.fanxiaobao.xyz

Ruby: # 无重载：靠动态参数
来源：http://oqt.hesvh.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://twn.sweek.top

================================================================================
来源：http://paw.bjfxy.top

D. 数组 / 列表 / 集合
来源：http://lzw.haohaochexian.top

================================================================================
来源：http://kmo.gogol.net.cn

[D01] 创建数组 / 列表
来源：http://ose.daxiang520.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://gip.yanxiufei.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wsx.gaohongyu789.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cnq.nwbrower.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://fpk.smart0.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fir.316326.xyz

Go:   arr := []int{1, 2, 3}
来源：http://jxh.feifeiyinyue.top

Ruby: arr = [1, 2, 3]
来源：http://mxm.sweek.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://uev.yj20258.top

[D02] 追加元素到末尾
来源：http://vbu.gzhubu.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pcy.ehwqpu.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jwv.gogol.net.cn

JS:   arr.push(4);
来源：http://qal.meibo888.top

TS:   arr.push(4);
来源：http://zhh.ppjwa.cn

Java: list.add(4);
来源：http://huv.pycfn.com

Go:   arr = append(arr, 4)
来源：http://hgj.yueranfly.top

Ruby: arr << 4; arr.push(5)
来源：http://kjv.tianlin.xyz

C#:   list.Add(4);
来源：http://rjh.jlsjyb.cn

[D03] 在指定位置插入元素
来源：http://gwf.jqgufenzy.top

Py:   arr.insert(0, 0)
来源：http://arf.shangyingyoupin.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xay.hysaishi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ykh.wangshuangyany.cn

TS:   arr.splice(0, 0, 0);
来源：http://ltl.yj202588.top

Java: list.add(0, 0);
来源：http://xdm.shzxlz.cn

Go:   arr = append([]int{0}, arr...)
来源：http://aob.quarkkingdee.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uxi.yangfankeji.com

C#:   list.Insert(0, 0);
来源：http://dwb.havefunace.top

[D04] 删除元素
来源：http://fct.aibaodan.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qov.wangdashe.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rgu.vehdjk.com


<!-- 参考信息 -->
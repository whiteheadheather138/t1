代发 wailian999

Py:   for i in range(10): print(i)
来源：http://lqy.ybcxt.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ipv.nanxinkj.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pyu.daxiang520.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://prd.gzhubu.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://azr.fanxiaobao.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pjr.tanke756.top

Ruby: 10.times { |i| puts i }
来源：http://vbi.9152youxi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yzj.chenlongwang.top

[B05] 遍历数组 / 列表
来源：http://dtc.xinyue.icu

Py:   for item in arr: print(item)
来源：http://sdv.xylfe.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wgr.dianchejie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://pri.jinqigufen.top

TS:   for (const item of arr) { console.log(item); }
来源：http://iiw.zhixingplan.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://tet.xuanzx.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lwy.jinqigufen.top

Ruby: arr.each { |item| puts item }
来源：http://ijp.hcnkem.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cqk.zhijiandao.cn

[B06] 遍历字典 / 对象
来源：http://yvo.wangshuangyany.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://rao.pengpengdd.cyou

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zmf.gzhubu.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://brp.ydjk.org.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yyn.jinqigufen.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://buc.ydjk.org.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hsh.meibo888.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ppa.xuetiantiany.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://izd.aizwys.cn

[B07] while 循环
来源：http://chx.fzhhl.top

Py:   while i < 10: i += 1
来源：http://ana.shanyushiyangkeji.top

PHP:  while ($i < 10) { $i++; }
来源：http://dqk.fzhhl.top

JS:   while (i < 10) { i++; }
来源：http://oio.chenjidiqi.icu

TS:   while (i < 10) { i++; }
来源：http://lla.yj20258.top

Java: while (i < 10) { i++; }
来源：http://jhx.epnwcf.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kuz.snrcjt.cn

Ruby: while i < 10; i += 1; end
来源：http://cex.vqdsnc.cn

C#:   while (i < 10) { i++; }
来源：http://prf.tianlin.xyz

[B08] do-while（至少执行一次）
来源：http://dty.gaohongyu789.top

Py:   # 无 do-while：用 while True + break
来源：http://nyl.gzhubu.top

PHP:  do { $i++; } while ($i < 10);
来源：http://foo.hysaishi.cn

JS:   do { i++; } while (i < 10);
来源：http://ryh.xuanzx.com

TS:   do { i++; } while (i < 10);
来源：http://bka.jiagoushi.top

Java: do { i++; } while (i < 10);
来源：http://igg.yfazqb.com

Go:   for { i++; if i >= 10 { break } }
来源：http://xzu.havefunace.top

Ruby: begin; i += 1; end while i < 10
来源：http://czp.yanxiufei.cn

C#:   do { i++; } while (i < 10);
来源：http://cah.andypj.xyz

[B09] break 与 continue
来源：http://xwe.jiagoushi.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://iga.aibaodan.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uoo.9152youxi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pxi.havefunace.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://duh.daxiang520.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uww.guowangkeji.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qgf.jlsjyb.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nok.aibaodan.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ufk.redwolf501.top

[B10] 遍历同时拿索引
来源：http://ubq.nanxuanxn.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nwv.hammf.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sic.xingfuxueyuan.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kqd.hfpthk.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cev.feifeiyinyue.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hiq.shzxlz.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bnk.epnwcf.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ikc.fzhhl.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ndz.sjlbkw.cn

[B11] 生成数字序列 / 区间
来源：http://fmq.gzhubu.top

Py:   list(range(0, 10, 2))
来源：http://yfj.gotoacloud.top

PHP:  range(0, 10, 2);
来源：http://qmr.ctjpmb.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gxw.zhongyouzk.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tkz.ctjpmb.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ysy.havefunace.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fbv.sxryk.cn

Ruby: (0...10).step(2).to_a
来源：http://oog.tanke756.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fyc.yj20258888.top

[B12] 跳出多层循环
来源：http://hnr.feifeiyinyue.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://wso.xinyue.icu

PHP:  # 无标签：用 goto 或函数返回
来源：http://znw.hywenlv.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://iiv.ybcxt.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nej.yuanzhike.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://roi.chenzaomai.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://paz.epnwcf.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vom.jinghuilouyu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ijx.zhoulong.xyz

[B13] 判断是否为数字
来源：http://utx.ehwqpu.com

Py:   isinstance(x, (int, float))
来源：http://ukc.tarul.cn

PHP:  is_numeric($x)
来源：http://jnh.hnxiangtu.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://apc.uphjek.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mgh.smart0.xyz

Java: x instanceof Number
来源：http://kpz.zdbjq.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zum.yj202588.top

Ruby: x.is_a?(Numeric)
来源：http://gql.meibo888.top

C#:   x is int or double or decimal
来源：http://sdy.vehdjk.com

[B14] 判断值是否在集合内
来源：http://lpx.yueranfly.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tes.tarul.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nwf.zdbjq.cn

JS:   [1, 2, 3].includes(x)
来源：http://wko.daria6918.cn

TS:   [1, 2, 3].includes(x)
来源：http://djf.yvedp.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vve.gzhubu.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pwp.tianlin.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://pse.jinqigufen.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ddy.sjlbkw.cn

[B15] 布尔运算与取反
来源：http://pjp.xingfuxueyuan.xyz

Py:   a and b or not c
来源：http://lty.fanxiaobao.xyz

PHP:  $a && $b || !$c
来源：http://tci.gzhubu.top

JS:   a && b || !c
来源：http://fwv.dashuyun.cn

TS:   a && b || !c
来源：http://vhr.cashguo.top

Java: a && b || !c
来源：http://xxh.mhx1999.top

Go:   a && b || !c
来源：http://zlx.zdbjq.cn

Ruby: a && b || !c
来源：http://qwk.yj202588.top

C#:   a && b || !c
来源：http://zuk.mhx1999.top

[B16] 卫语句：不满足条件提前返回
来源：http://fzf.chenlongwang.top

Py:   if not data: return
来源：http://lyb.hesvh.cn

PHP:  if (!$data) { return; }
来源：http://pph.tianlin.xyz

JS:   if (!data) return;
来源：http://lqc.ybcxt.top

TS:   if (!data) return;
来源：http://lba.zhixingplan.top

Java: if (data == null) return;
来源：http://rqk.cucudq.cn

Go:   if data == nil { return }
来源：http://fgz.52xcode.cn

Ruby: return if data.nil?
来源：http://hux.gzhubu.top

C#:   if (data == null) return;
来源：http://fqj.ydjk.org.cn

================================================================================
来源：http://jcv.ywan-chungtsiang.top

C. 函数与作用域
来源：http://szq.daxiang520.top

================================================================================
来源：http://ouo.jinqigufen.top

[C01] 定义函数
来源：http://uuw.ydjk.org.cn

Py:   def add(a, b): return a + b
来源：http://qap.pengpengdd.cyou

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://omi.ehwqpu.com

JS:   function add(a, b) { return a + b; }
来源：http://lea.ydzc1.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fub.jqgufenzy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://fkr.dashuyun.cn

Go:   func add(a, b int) int { return a + b }
来源：http://shv.gogol.net.cn

Ruby: def add(a, b); a + b; end
来源：http://zkg.gzhubu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tnj.sysykeji.top

[C02] 默认参数
来源：http://lrj.cucudq.cn

Py:   def greet(name="World"): return name
来源：http://aib.9152youxi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fpw.daxiang520.top

JS:   function greet(name = "World") { return name; }
来源：http://htw.xingfuxueyuan.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://vce.snrcjt.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://scx.hcnkem.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nzz.xingfuxueyuan.xyz

Ruby: def greet(name = "World") = name
来源：http://bci.andypj.xyz

C#:   string Greet(string name = "World") => name;
来源：http://hnl.fanxiaobao.xyz

[C03] 可变参数
来源：http://jro.jinghuilouyu.cn

Py:   def total(*args): return sum(args)
来源：http://siy.sufxvd.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lrk.c1oappe.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qwy.jinqigfzy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lrf.jqgfzy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mpc.xylfe.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nuw.xingfuxueyuan.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://wuf.c1oappe.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xif.wangdashe.top

[C04] 命名参数 / 关键字参数
来源：http://jlc.fanxiaobao.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kzn.epnwcf.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fef.fehbvm.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://srw.zhixingplan.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nbo.ydzc1.top

Java: // 无：用 Builder 模式或 record
来源：http://imu.chenjidiqi.icu

Go:   // 无：用配置结构体参数
来源：http://vph.gzhubu.top

Ruby: f(a: 1, b: 2)
来源：http://hfj.zdbjq.cn

C#:   f(a: 1, b: 2)
来源：http://xzq.chenzaomai.com

[C05] 返回多个值
来源：http://gsr.havefunace.top

Py:   return a, b
来源：http://aid.yvedp.cn

PHP:  return [$a, $b];
来源：http://sta.fehbvm.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://lpe.aibaodan.cn

TS:   return { a, b };
来源：http://nyk.ywan-chungtsiang.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xym.jinqigufen.top

Go:   return a, b
来源：http://jsh.zhixingplan.top

Ruby: return a, b
来源：http://zln.sxryk.cn

C#:   return (a, b);              // ValueTuple
来源：http://qne.jianghu66.top

[C06] 匿名函数 / lambda
来源：http://onh.fehbvm.com

Py:   square = lambda x: x * x
来源：http://hxh.yueranfly.top

PHP:  $square = fn($x) => $x * $x;
来源：http://arr.zdqjudy.top

JS:   const square = x => x * x;
来源：http://hnk.nanxuanxn.top

TS:   const square = (x: number): number => x * x;
来源：http://zbn.snrcjt.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://uce.gaohongyu789.top

Go:   sq := func(x int) int { return x * x }
来源：http://ace.daria6918.cn

Ruby: square = ->(x) { x * x }
来源：http://bty.yvedp.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bur.zhaomingkeji.xyz

[C07] 把函数作为参数传入
来源：http://cjv.yj202588.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://olk.xuetiantiany.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hyh.xingfuxueyuan.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zen.gogol.net.cn

TS:   arr.map(String)
来源：http://kqo.tian-w.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zwc.fzhhl.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://owd.feifeiyinyue.top

Ruby: arr.map(&:upcase)
来源：http://zjq.daxiang520.top

C#:   arr.Select(s => s.ToUpper())
来源：http://okd.dianchejie.cn

[C08] 闭包
来源：http://dew.havefunace.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zrt.gotoacloud.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hel.fehbvm.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://duo.gogol.net.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qcp.0kj1m.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://thv.epnwcf.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wtx.xziqi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ffw.chenlongwang.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ogu.316326.xyz

[C09] 递归
来源：http://fif.gaohongyu789.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tvl.c1oappe.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pqp.hesvh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ysd.iojbl.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ygv.uphjek.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ncn.316326.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uni.zhongyouzk.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gwo.xuetiantiany.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ewx.meibo888.top

[C10] 变量作用域
来源：http://xmg.guannengcc.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xgu.sweek.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fjr.yonumen.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wqg.sysykeji.top

TS:   同 JS
来源：http://vid.kuanghao11.cn

Java: 方法内为块级作用域
来源：http://eqp.nanxuanxn.top

Go:   花括号块级作用域
来源：http://pyt.xylfe.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rud.hysaishi.cn

C#:   块级作用域
来源：http://qji.zycfv.cn

[C11] 模块导入与导出
来源：http://sae.nanxinkj.top

Py:   from module import func
来源：http://mjq.iojbl.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://rgl.chenlongwang.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://hsv.aizwys.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ppb.havefunace.top

Java: import java.util.List;
来源：http://xym.gzhubu.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vrh.kuanghao11.cn

Ruby: require "json"; require_relative "./util"
来源：http://qnd.shanyushiyangkeji.top

C#:   using System.Text;
来源：http://gba.cashguo.top

[C12] 立即执行函数 IIFE
来源：http://dbx.fanxiaobao.xyz

Py:   (lambda: print("run"))()
来源：http://cbp.wangdashe.top

PHP:  (function () { echo "run"; })();
来源：http://thy.ydzc1.top

JS:   (() => { console.log("run"); })();
来源：http://fir.guowangkeji.top

TS:   (() => { console.log("run"); })();
来源：http://dly.52xcode.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fme.iojbl.cn

Go:   func() { fmt.Println("run") }()
来源：http://oga.yangfankeji.com

Ruby: -> { puts "run" }.call
来源：http://qqb.52xcode.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://cna.andypj.xyz

[C13] 类型声明 / 类型注解
来源：http://awf.chenjidiqi.icu

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://otr.wangdashe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rfz.xuetiantiany.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kmk.zhaomingkeji.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://glk.uphjek.com

Java: int add(int a, int b) { return a + b; }
来源：http://lvz.redwolf501.top

Go:   func add(a, b int) int
来源：http://ffh.nanxuanxn.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tgo.hongshengwenyu.top

C#:   int Add(int a, int b) => a + b;
来源：http://gcr.sxryk.cn

[C14] 泛型函数
来源：http://dyh.zycfv.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zwy.zhoulong.xyz

PHP:  // 无泛型
来源：http://qly.sufxvd.cn

JS:   // 无泛型
来源：http://ule.nanxinkj.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kgg.hammf.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xcj.ppjwa.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ymh.nanxuanxn.top

Ruby: # 无泛型
来源：http://uvo.yj202588.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nvj.zhongyouzk.top

[C15] 解构 / 展开参数
来源：http://qpv.zhiwuduotai.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kvn.wangdashe.top

PHP:  [$a, $b] = $pair;
来源：http://lxd.hywenlv.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lwk.yongpay.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uke.daxiang520.top

Java: // 无解构
来源：http://rza.jinqigufen.top

Go:   // 无解构
来源：http://skc.cheryme.top

Ruby: a, b = pair
来源：http://wfg.ywan-chungtsiang.top

C#:   var (a, b) = pair;
来源：http://puh.birdmap.top

[C16] 函数 / 方法重载
来源：http://qvl.ctjpmb.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://shp.pycfn.com

PHP:  // 无重载
来源：http://dsn.52xcode.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://lrl.fehbvm.com

TS:   // 用联合类型或重载签名声明
来源：http://lqe.wangshuangyany.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://dpj.shangyingyoupin.top

Go:   // 无重载：用不同函数名
来源：http://tzc.andypj.xyz

Ruby: # 无重载：靠动态参数
来源：http://rcf.cdnleiting.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://fxn.mhx1999.top

================================================================================
来源：http://ntw.jqgfzy.top

D. 数组 / 列表 / 集合
来源：http://kja.iojbl.cn

================================================================================
来源：http://muv.jqgufenzy.top

[D01] 创建数组 / 列表
来源：http://abg.nanxinkj.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://sos.xuanzx.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rmx.vehdjk.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pst.vqdsnc.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://gyt.wangshuangyany.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wgu.xziqi.cn

Go:   arr := []int{1, 2, 3}
来源：http://rdk.shanyushiyangtech.top

Ruby: arr = [1, 2, 3]
来源：http://qev.redwolf501.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://drn.yongpay.top

[D02] 追加元素到末尾
来源：http://nmn.yuxming.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zxw.fktsv.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zoq.0kj1m.cn

JS:   arr.push(4);
来源：http://ocw.xingfuxueyuan.xyz

TS:   arr.push(4);
来源：http://kqm.nanxinkj.top

Java: list.add(4);
来源：http://tye.hnqzz.top

Go:   arr = append(arr, 4)
来源：http://ynf.hnqzz.top

Ruby: arr << 4; arr.push(5)
来源：http://kqj.yuxming.cn

C#:   list.Add(4);
来源：http://ege.gogol.net.cn

[D03] 在指定位置插入元素
来源：http://efc.jinqigufen.top

Py:   arr.insert(0, 0)
来源：http://rjj.ivvv.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qvy.fehbvm.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jet.pycfn.com

TS:   arr.splice(0, 0, 0);
来源：http://pzl.redwolf501.top

Java: list.add(0, 0);
来源：http://rbe.gotoacloud.top

Go:   arr = append([]int{0}, arr...)
来源：http://css.vehdjk.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yyg.yonumen.top

C#:   list.Insert(0, 0);
来源：http://pbr.zhixingplan.top

[D04] 删除元素
来源：http://biw.jinghuilouyu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yea.xuanzx.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://oqw.yongpay.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rcu.ywan-chungtsiang.top

TS:   arr.splice(0, 1);
来源：http://lqh.kuanghao11.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hsc.ydjk.org.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zsf.yj202588.top


<!-- 参考信息 -->
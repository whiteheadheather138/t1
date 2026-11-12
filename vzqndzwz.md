代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fhh.jinghuilouyu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sin.tanke756.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fea.jqgufenzy.top

[B04] for 计数循环
来源：http://raa.chenjidiqi.icu

Py:   for i in range(10): print(i)
来源：http://tsk.0kj1m.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wup.sxryk.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sjz.zdbjq.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pcz.shzxlz.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ovc.zhongyouzk.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jbc.yvedp.cn

Ruby: 10.times { |i| puts i }
来源：http://hhz.ydzc1.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sdo.ehwqpu.com

[B05] 遍历数组 / 列表
来源：http://qhz.aizwys.cn

Py:   for item in arr: print(item)
来源：http://ecd.birdmap.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nsb.hywenlv.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://mdo.fehbvm.com

TS:   for (const item of arr) { console.log(item); }
来源：http://orc.jqgufenzy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ert.shanyushiyangtech.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qtr.zycfv.cn

Ruby: arr.each { |item| puts item }
来源：http://ajn.mhx1999.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nwx.uphjek.com

[B06] 遍历字典 / 对象
来源：http://wka.jinghuilouyu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://lmq.hesvh.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nhy.jinghuilouyu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hlt.yongpay.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kqg.tianlin.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://byq.uphjek.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nqi.gaohongyu789.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bym.nanxinkj.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lws.zycfv.cn

[B07] while 循环
来源：http://krc.c1oappe.top

Py:   while i < 10: i += 1
来源：http://wdi.bjfxy.top

PHP:  while ($i < 10) { $i++; }
来源：http://lel.dashuyun.cn

JS:   while (i < 10) { i++; }
来源：http://kwv.zhengqikj.top

TS:   while (i < 10) { i++; }
来源：http://wta.hnxiangtu.top

Java: while (i < 10) { i++; }
来源：http://mfl.fehbvm.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qbl.snrcjt.cn

Ruby: while i < 10; i += 1; end
来源：http://tcw.ppjwa.cn

C#:   while (i < 10) { i++; }
来源：http://jzq.jinyuanbaomall.cn

[B08] do-while（至少执行一次）
来源：http://zvo.cdnleiting.top

Py:   # 无 do-while：用 while True + break
来源：http://uga.yj20258.top

PHP:  do { $i++; } while ($i < 10);
来源：http://zpw.nanxuanxn.top

JS:   do { i++; } while (i < 10);
来源：http://wkm.cashguo.top

TS:   do { i++; } while (i < 10);
来源：http://cxs.svipenyu.cn

Java: do { i++; } while (i < 10);
来源：http://lyy.iojbl.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gri.xylfe.cn

Ruby: begin; i += 1; end while i < 10
来源：http://guh.zhijiandao.cn

C#:   do { i++; } while (i < 10);
来源：http://wtd.hnxiangtu.top

[B09] break 与 continue
来源：http://vmv.zdbjq.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rwr.xingfuxueyuan.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zqw.shzxlz.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qez.jinqigufen.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fld.yuxming.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://czb.hysaishi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rnv.xingfuxueyuan.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ydt.zhijiandao.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qdt.ivvv.top

[B10] 遍历同时拿索引
来源：http://par.jianghu66.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://khd.hywenlv.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xjf.chenjidiqi.icu

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kzs.yonumen.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zvn.snrcjt.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rza.jinqigufen.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bgw.jlsjyb.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://krr.jinyuanbaomall.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pqb.yuxming.cn

[B11] 生成数字序列 / 区间
来源：http://xnw.zhengqikj.top

Py:   list(range(0, 10, 2))
来源：http://ptd.redwolf501.top

PHP:  range(0, 10, 2);
来源：http://ovw.jqgufenzy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qve.tianlin.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rjb.aizwys.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gvz.nanxuanxn.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rae.quarkkingdee.top

Ruby: (0...10).step(2).to_a
来源：http://nzh.zhijiandao.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xrs.cqqwz.cn

[B12] 跳出多层循环
来源：http://cco.zhijiandao.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wtt.nwbrower.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://tbf.zhiwuduotai.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gxp.snrcjt.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ayr.uphjek.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://llz.cucudq.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ajt.meibo888.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fgw.guowangkeji.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bnq.ydjk.org.cn

[B13] 判断是否为数字
来源：http://qkn.c1oappe.top

Py:   isinstance(x, (int, float))
来源：http://say.0kj1m.cn

PHP:  is_numeric($x)
来源：http://qay.bbcook.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://azr.nanxinkj.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jqh.chenlongwang.top

Java: x instanceof Number
来源：http://yua.nwbrower.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://idz.epnwcf.com

Ruby: x.is_a?(Numeric)
来源：http://fhk.cdnleiting.top

C#:   x is int or double or decimal
来源：http://hwk.sjlbkw.cn

[B14] 判断值是否在集合内
来源：http://qcz.gzhubu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://eii.tianlin.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bch.hywenlv.cn

JS:   [1, 2, 3].includes(x)
来源：http://kai.yj20258888.top

TS:   [1, 2, 3].includes(x)
来源：http://bof.meibo888.top

Java: List.of(1, 2, 3).contains(x)
来源：http://anc.xziqi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jem.jlsjyb.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ruc.zhixingplan.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cmo.zhijiandao.cn

[B15] 布尔运算与取反
来源：http://ial.zhixingplan.top

Py:   a and b or not c
来源：http://ybh.xuetiantiany.cn

PHP:  $a && $b || !$c
来源：http://vmp.xinyue.icu

JS:   a && b || !c
来源：http://iox.ctjpmb.com

TS:   a && b || !c
来源：http://vcc.nanxuanxn.top

Java: a && b || !c
来源：http://xcb.cashguo.top

Go:   a && b || !c
来源：http://oob.zhijiandao.cn

Ruby: a && b || !c
来源：http://jlg.zycfv.cn

C#:   a && b || !c
来源：http://zij.aizwys.cn

[B16] 卫语句：不满足条件提前返回
来源：http://uqj.zhixingplan.top

Py:   if not data: return
来源：http://gox.zhengqikj.top

PHP:  if (!$data) { return; }
来源：http://mie.quarkkingdee.top

JS:   if (!data) return;
来源：http://ftr.jinghuilouyu.cn

TS:   if (!data) return;
来源：http://glg.yueranfly.top

Java: if (data == null) return;
来源：http://iqj.jinghuilouyu.cn

Go:   if data == nil { return }
来源：http://zjr.ywan-chungtsiang.top

Ruby: return if data.nil?
来源：http://hwb.hywenlv.cn

C#:   if (data == null) return;
来源：http://pfg.tarul.cn

================================================================================
来源：http://uoy.zhixingplan.top

C. 函数与作用域
来源：http://dzl.xziqi.cn

================================================================================
来源：http://nio.chenzaomai.com

[C01] 定义函数
来源：http://gae.sweek.top

Py:   def add(a, b): return a + b
来源：http://pgu.shuidangran.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yzh.nwbrower.top

JS:   function add(a, b) { return a + b; }
来源：http://uam.guannengcc.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vej.dashuyun.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://nob.birdmap.top

Go:   func add(a, b int) int { return a + b }
来源：http://plz.fehbvm.com

Ruby: def add(a, b); a + b; end
来源：http://pfe.vehdjk.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kby.pycfn.com

[C02] 默认参数
来源：http://qwi.ivvv.top

Py:   def greet(name="World"): return name
来源：http://qhg.cucudq.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xsb.shzxlz.cn

JS:   function greet(name = "World") { return name; }
来源：http://etw.aibaodan.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qdf.redwolf501.top

Java: // 无默认参数：方法重载或 Optional
来源：http://vov.wangshuangyany.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dgm.wangshuangyany.cn

Ruby: def greet(name = "World") = name
来源：http://zdw.hfpthk.cn

C#:   string Greet(string name = "World") => name;
来源：http://crv.jinqigufen.top

[C03] 可变参数
来源：http://acx.ctjpmb.com

Py:   def total(*args): return sum(args)
来源：http://moe.dashuyun.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cur.ydjk.org.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bar.ppjwa.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ykt.ywan-chungtsiang.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cxx.yfazqb.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ubz.ppjwa.cn

Ruby: def total(*nums); nums.sum; end
来源：http://avs.svipenyu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qom.havefunace.top

[C04] 命名参数 / 关键字参数
来源：http://gqs.hongshengwenyu.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tip.shanyushiyangtech.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gdb.zdbjq.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dsz.yfazqb.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dne.hnxiangtu.top

Java: // 无：用 Builder 模式或 record
来源：http://lhf.zhongyouzk.top

Go:   // 无：用配置结构体参数
来源：http://dhx.daria6918.cn

Ruby: f(a: 1, b: 2)
来源：http://nnz.redwolf501.top

C#:   f(a: 1, b: 2)
来源：http://ojf.jlsjyb.cn

[C05] 返回多个值
来源：http://owr.gotoacloud.top

Py:   return a, b
来源：http://bjf.guannengcc.top

PHP:  return [$a, $b];
来源：http://qca.c1oappe.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://hlq.chenzaomai.com

TS:   return { a, b };
来源：http://lgd.daxiang520.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qjc.316326.xyz

Go:   return a, b
来源：http://lku.fanxiaobao.xyz

Ruby: return a, b
来源：http://ilf.shuidangran.top

C#:   return (a, b);              // ValueTuple
来源：http://vkn.jianghu66.top

[C06] 匿名函数 / lambda
来源：http://mlf.ydzc1.top

Py:   square = lambda x: x * x
来源：http://sys.smart0.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://qzx.hcnkem.com

JS:   const square = x => x * x;
来源：http://upm.zdqjudy.top

TS:   const square = (x: number): number => x * x;
来源：http://dfs.jqgufenzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gfc.zhijiandao.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dyl.aibaodan.cn

Ruby: square = ->(x) { x * x }
来源：http://zef.ctjpmb.com

C#:   Func<int, int> square = x => x * x;
来源：http://fmd.chenjidiqi.icu

[C07] 把函数作为参数传入
来源：http://qyv.chenjidiqi.icu

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://byh.jqgfzy.top

PHP:  array_map("strtoupper", $arr);
来源：http://fll.vqdsnc.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://oyy.316326.xyz

TS:   arr.map(String)
来源：http://cfa.cqqwz.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zmg.xinyue.icu

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://drl.epnwcf.com

Ruby: arr.map(&:upcase)
来源：http://tcl.9152youxi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://rba.wangshuangyany.cn

[C08] 闭包
来源：http://drc.mhx1999.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vvc.ywan-chungtsiang.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ivd.cqqwz.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uza.zhaomingkeji.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gvq.guannengcc.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gie.0kj1m.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fve.gogol.net.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sae.hnqzz.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xcc.zhiwuduotai.top

[C09] 递归
来源：http://eyj.yj202588.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://clj.zhoulong.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://prv.smart0.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yqh.feifeiyinyue.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://coy.sufxvd.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ttp.yj20258888.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jzi.birdmap.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rwc.havefunace.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://slh.hywenlv.cn

[C10] 变量作用域
来源：http://hzh.fengsongda.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gci.hnxiangtu.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xnz.jinqigfzy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dal.zhiwuduotai.top

TS:   同 JS
来源：http://tzk.nanxuanxn.top

Java: 方法内为块级作用域
来源：http://eqg.fktsv.cn

Go:   花括号块级作用域
来源：http://udn.0kj1m.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wbt.meibo888.top

C#:   块级作用域
来源：http://xea.zhongyouzk.top

[C11] 模块导入与导出
来源：http://wzw.yangfankeji.com

Py:   from module import func
来源：http://lkp.havefunace.top

PHP:  require "file.php";  或 use App\Service;
来源：http://smc.shangyingyoupin.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://mfc.haohaochexian.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ulk.yj20258888.top

Java: import java.util.List;
来源：http://dzg.shanyushiyangkeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ejz.yanxiufei.cn

Ruby: require "json"; require_relative "./util"
来源：http://lkh.hnqzz.top

C#:   using System.Text;
来源：http://puw.jinghuilouyu.cn

[C12] 立即执行函数 IIFE
来源：http://lhg.gzhubu.top

Py:   (lambda: print("run"))()
来源：http://lhu.cashguo.top

PHP:  (function () { echo "run"; })();
来源：http://xwi.cashguo.top

JS:   (() => { console.log("run"); })();
来源：http://uwj.chenzaomai.com

TS:   (() => { console.log("run"); })();
来源：http://con.havefunace.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ldz.nanxinkj.top

Go:   func() { fmt.Println("run") }()
来源：http://twc.daxiang520.top

Ruby: -> { puts "run" }.call
来源：http://fds.cucudq.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://pom.xuanzx.com

[C13] 类型声明 / 类型注解
来源：http://ccv.jianghu66.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vxn.sysykeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qxk.aizwys.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sas.fzhhl.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ald.iojbl.cn

Java: int add(int a, int b) { return a + b; }
来源：http://tzv.hysaishi.cn

Go:   func add(a, b int) int
来源：http://rpc.yuanzhike.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hiy.zhiwuduotai.top

C#:   int Add(int a, int b) => a + b;
来源：http://gum.jinqigfzy.top

[C14] 泛型函数
来源：http://zbh.yangfankeji.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zls.xingfuxueyuan.xyz

PHP:  // 无泛型
来源：http://fbm.tian-w.cn

JS:   // 无泛型
来源：http://zpt.sufxvd.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uhf.yfazqb.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jww.jyoumei.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://znj.cheryme.top

Ruby: # 无泛型
来源：http://jcq.xuanzx.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zhy.fehbvm.com

[C15] 解构 / 展开参数
来源：http://lxz.svipenyu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xrn.smart0.xyz

PHP:  [$a, $b] = $pair;
来源：http://kty.svipenyu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://alv.meibo888.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ywt.sjlbkw.cn

Java: // 无解构
来源：http://ijb.jqgfzy.top

Go:   // 无解构
来源：http://cxd.yonumen.top

Ruby: a, b = pair
来源：http://yqv.shanyushiyangkeji.top

C#:   var (a, b) = pair;
来源：http://uzf.svipenyu.cn

[C16] 函数 / 方法重载
来源：http://ttm.ppjwa.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kih.0kj1m.cn

PHP:  // 无重载
来源：http://ywz.hcnkem.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://teb.bjfxy.top

TS:   // 用联合类型或重载签名声明
来源：http://lon.zdbjq.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://voh.hywenlv.cn

Go:   // 无重载：用不同函数名
来源：http://hha.jlsjyb.cn

Ruby: # 无重载：靠动态参数
来源：http://esc.wangshuangyany.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zkt.yonumen.top

================================================================================
来源：http://dkx.birdmap.top

D. 数组 / 列表 / 集合
来源：http://flw.yj202588.top

================================================================================
来源：http://qcp.hywenlv.cn

[D01] 创建数组 / 列表
来源：http://kjv.52xcode.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://wlc.sjlbkw.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fmo.xinyue.icu

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bfh.wangdashe.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://vqw.uphjek.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ekt.gzhubu.top

Go:   arr := []int{1, 2, 3}
来源：http://dgm.xziqi.cn

Ruby: arr = [1, 2, 3]
来源：http://kyp.redwolf501.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fiq.jyoumei.cn

[D02] 追加元素到末尾
来源：http://gus.zhixingplan.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ouj.yj20258.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ldr.ehwqpu.com

JS:   arr.push(4);
来源：http://aag.gogol.net.cn

TS:   arr.push(4);
来源：http://rsq.shanyushiyangtech.top

Java: list.add(4);
来源：http://dga.guowangkeji.top

Go:   arr = append(arr, 4)
来源：http://mik.xuanzx.com

Ruby: arr << 4; arr.push(5)
来源：http://byl.zhiwuduotai.top

C#:   list.Add(4);
来源：http://epg.meibo888.top

[D03] 在指定位置插入元素
来源：http://mif.52xcode.cn

Py:   arr.insert(0, 0)
来源：http://bao.fehbvm.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fwl.hcnkem.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nxj.jinghuilouyu.cn

TS:   arr.splice(0, 0, 0);
来源：http://zik.haohaochexian.top

Java: list.add(0, 0);
来源：http://zfj.zhongyouzk.top

Go:   arr = append([]int{0}, arr...)
来源：http://aye.jqgufenzy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bna.hongshengwenyu.top

C#:   list.Insert(0, 0);
来源：http://aus.yj20258888.top

[D04] 删除元素
来源：http://spq.gotoacloud.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://izg.wangdashe.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yre.vqdsnc.cn


<!-- 参考信息 -->
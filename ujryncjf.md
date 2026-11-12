代发 wailian999

[B05] 遍历数组 / 列表
来源：http://nar.gogol.net.cn

Py:   for item in arr: print(item)
来源：http://gli.hnxiangtu.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ifs.yfazqb.com

JS:   for (const item of arr) { console.log(item); }
来源：http://xox.gotoacloud.top

TS:   for (const item of arr) { console.log(item); }
来源：http://bwi.vehdjk.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://gyi.pengpengdd.cyou

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://org.quarkkingdee.top

Ruby: arr.each { |item| puts item }
来源：http://aqp.cdnleiting.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ywg.zycfv.cn

[B06] 遍历字典 / 对象
来源：http://xdh.jianghu66.top

Py:   for k, v in d.items(): print(k, v)
来源：http://gpi.gaohongyu789.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kkt.zhiwuduotai.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ftl.shanyushiyangtech.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gdn.yfazqb.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kbn.svipenyu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kir.vehdjk.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ifq.zhixingplan.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vok.shanyushiyangkeji.top

[B07] while 循环
来源：http://zbc.smart0.xyz

Py:   while i < 10: i += 1
来源：http://ywb.ydjk.org.cn

PHP:  while ($i < 10) { $i++; }
来源：http://tny.hnqzz.top

JS:   while (i < 10) { i++; }
来源：http://hqd.svipenyu.cn

TS:   while (i < 10) { i++; }
来源：http://ysl.jinqigfzy.top

Java: while (i < 10) { i++; }
来源：http://epy.yj20258888.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xbh.yonumen.top

Ruby: while i < 10; i += 1; end
来源：http://mzk.shangyingyoupin.top

C#:   while (i < 10) { i++; }
来源：http://iin.hywenlv.cn

[B08] do-while（至少执行一次）
来源：http://qec.sweek.top

Py:   # 无 do-while：用 while True + break
来源：http://fdw.tianlin.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://cfs.tian-w.cn

JS:   do { i++; } while (i < 10);
来源：http://ryu.cqqwz.cn

TS:   do { i++; } while (i < 10);
来源：http://cpi.kuanghao11.cn

Java: do { i++; } while (i < 10);
来源：http://ofj.jinqigufen.top

Go:   for { i++; if i >= 10 { break } }
来源：http://jep.hongshengwenyu.top

Ruby: begin; i += 1; end while i < 10
来源：http://jqw.shuidangran.top

C#:   do { i++; } while (i < 10);
来源：http://tli.zhongyouzk.top

[B09] break 与 continue
来源：http://qza.c1oappe.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bff.meibo888.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cxy.shuidangran.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zis.nanxinkj.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://msz.hnxiangtu.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iaw.sweek.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yqg.sweek.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hfo.mhx1999.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ewa.hysaishi.cn

[B10] 遍历同时拿索引
来源：http://mmf.jinghuilouyu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fzs.ywan-chungtsiang.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hug.ywan-chungtsiang.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://eco.yanxiufei.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sua.smart0.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wrb.sweek.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mno.shuidangran.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wdu.sweek.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dpp.yfazqb.com

[B11] 生成数字序列 / 区间
来源：http://uiz.pengpengdd.cyou

Py:   list(range(0, 10, 2))
来源：http://rzj.sufxvd.cn

PHP:  range(0, 10, 2);
来源：http://uww.sjlbkw.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jxb.daria6918.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lyh.xziqi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ucx.shanyushiyangkeji.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ftm.yongpay.top

Ruby: (0...10).step(2).to_a
来源：http://alb.hywenlv.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mci.jlsjyb.cn

[B12] 跳出多层循环
来源：http://ibj.epnwcf.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://usp.dianchejie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://pdw.tian-w.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://osv.xuetiantiany.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vnm.guannengcc.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://sjv.xingfuxueyuan.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://izg.shanyushiyangtech.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vpj.zdbjq.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wec.yuanzhike.top

[B13] 判断是否为数字
来源：http://gbm.hongshengwenyu.top

Py:   isinstance(x, (int, float))
来源：http://yus.ywan-chungtsiang.top

PHP:  is_numeric($x)
来源：http://jvb.jinqigufen.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nsr.yj20258888.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qgt.gotoacloud.top

Java: x instanceof Number
来源：http://sik.chenzaomai.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rdg.fktsv.cn

Ruby: x.is_a?(Numeric)
来源：http://jrw.mhx1999.top

C#:   x is int or double or decimal
来源：http://isk.sweek.top

[B14] 判断值是否在集合内
来源：http://vbq.yj20258.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wjz.vehdjk.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qgt.bbcook.cn

JS:   [1, 2, 3].includes(x)
来源：http://oxm.bbcook.cn

TS:   [1, 2, 3].includes(x)
来源：http://lxt.jinghuilouyu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://twf.bbcook.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dls.aizwys.cn

Ruby: [1, 2, 3].include?(x)
来源：http://hlk.zdqjudy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ysw.fanxiaobao.xyz

[B15] 布尔运算与取反
来源：http://lnz.zhengqikj.top

Py:   a and b or not c
来源：http://xqd.pycfn.com

PHP:  $a && $b || !$c
来源：http://dtn.yangfankeji.com

JS:   a && b || !c
来源：http://apw.jlsjyb.cn

TS:   a && b || !c
来源：http://ulj.andypj.xyz

Java: a && b || !c
来源：http://uzq.epnwcf.com

Go:   a && b || !c
来源：http://zbw.iojbl.cn

Ruby: a && b || !c
来源：http://xtv.uphjek.com

C#:   a && b || !c
来源：http://hkr.yonumen.top

[B16] 卫语句：不满足条件提前返回
来源：http://irj.yj20258888.top

Py:   if not data: return
来源：http://whn.xziqi.cn

PHP:  if (!$data) { return; }
来源：http://xlz.ehwqpu.com

JS:   if (!data) return;
来源：http://rdi.meibo888.top

TS:   if (!data) return;
来源：http://qsy.tarul.cn

Java: if (data == null) return;
来源：http://adj.shzxlz.cn

Go:   if data == nil { return }
来源：http://slh.vehdjk.com

Ruby: return if data.nil?
来源：http://qqe.chenjidiqi.icu

C#:   if (data == null) return;
来源：http://oiz.yonumen.top

================================================================================
来源：http://edc.zdqjudy.top

C. 函数与作用域
来源：http://awf.guowangkeji.top

================================================================================
来源：http://zqi.ctjpmb.com

[C01] 定义函数
来源：http://mda.meibo888.top

Py:   def add(a, b): return a + b
来源：http://ifx.hcnkem.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hzv.hywenlv.cn

JS:   function add(a, b) { return a + b; }
来源：http://brw.yongpay.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kmi.bbcook.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vqg.hfpthk.cn

Go:   func add(a, b int) int { return a + b }
来源：http://uvn.epnwcf.com

Ruby: def add(a, b); a + b; end
来源：http://dmn.sxryk.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://srh.yangfankeji.com

[C02] 默认参数
来源：http://uxb.dashuyun.cn

Py:   def greet(name="World"): return name
来源：http://dkr.sxryk.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://iwv.mhx1999.top

JS:   function greet(name = "World") { return name; }
来源：http://pfv.dashuyun.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://tli.epnwcf.com

Java: // 无默认参数：方法重载或 Optional
来源：http://jgb.pycfn.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mal.zhaomingkeji.xyz

Ruby: def greet(name = "World") = name
来源：http://kkf.yj20258888.top

C#:   string Greet(string name = "World") => name;
来源：http://nvl.cheryme.top

[C03] 可变参数
来源：http://fnv.birdmap.top

Py:   def total(*args): return sum(args)
来源：http://uhb.nwbrower.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://phl.ctjpmb.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wqh.meibo888.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pml.sysykeji.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cir.sjlbkw.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://znw.jianghu66.top

Ruby: def total(*nums); nums.sum; end
来源：http://fgp.jyoumei.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fxx.svipenyu.cn

[C04] 命名参数 / 关键字参数
来源：http://bxv.pengpengdd.cyou

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://aiu.yueranfly.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ubu.havefunace.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qcy.zycfv.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bdr.yfazqb.com

Java: // 无：用 Builder 模式或 record
来源：http://rzy.ehwqpu.com

Go:   // 无：用配置结构体参数
来源：http://kqu.uphjek.com

Ruby: f(a: 1, b: 2)
来源：http://erw.316326.xyz

C#:   f(a: 1, b: 2)
来源：http://eqw.zhoulong.xyz

[C05] 返回多个值
来源：http://wbk.daria6918.cn

Py:   return a, b
来源：http://fjt.tian-w.cn

PHP:  return [$a, $b];
来源：http://dgb.hongshengwenyu.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://pco.zhiwuduotai.top

TS:   return { a, b };
来源：http://ajz.tarul.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://prt.nwbrower.top

Go:   return a, b
来源：http://kse.cucudq.cn

Ruby: return a, b
来源：http://psu.yonumen.top

C#:   return (a, b);              // ValueTuple
来源：http://poy.yj20258.top

[C06] 匿名函数 / lambda
来源：http://brk.ppjwa.cn

Py:   square = lambda x: x * x
来源：http://mfl.jinqigfzy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://roh.svipenyu.cn

JS:   const square = x => x * x;
来源：http://riw.xingfuxueyuan.xyz

TS:   const square = (x: number): number => x * x;
来源：http://fkb.cashguo.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lje.ydjk.org.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fxy.9152youxi.cn

Ruby: square = ->(x) { x * x }
来源：http://gmm.cheryme.top

C#:   Func<int, int> square = x => x * x;
来源：http://vzi.shuidangran.top

[C07] 把函数作为参数传入
来源：http://ymc.hfpthk.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://urc.hywenlv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ssi.hnxiangtu.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rft.yj202588.top

TS:   arr.map(String)
来源：http://jci.hywenlv.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mao.svipenyu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nyn.shangyingyoupin.top

Ruby: arr.map(&:upcase)
来源：http://ssc.birdmap.top

C#:   arr.Select(s => s.ToUpper())
来源：http://znw.vehdjk.com

[C08] 闭包
来源：http://phx.cheryme.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lhh.zycfv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dhn.yj20258.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ifh.yuxming.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://faw.chenzaomai.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xrs.316326.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://eft.yj20258888.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bsp.gotoacloud.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ojv.jinyuanbaomall.cn

[C09] 递归
来源：http://lvm.yanxiufei.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bch.fengsongda.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xfe.yj20258.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ciw.yvedp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kbj.daria6918.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mty.yangfankeji.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xbz.ehwqpu.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ljo.zhixingplan.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ids.vqdsnc.cn

[C10] 变量作用域
来源：http://zdu.hfpthk.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://oxw.smart0.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dbb.guannengcc.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sfo.zhongyouzk.top

TS:   同 JS
来源：http://sip.kuanghao11.cn

Java: 方法内为块级作用域
来源：http://qre.uphjek.com

Go:   花括号块级作用域
来源：http://acr.birdmap.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xll.hnxiangtu.top

C#:   块级作用域
来源：http://ies.cashguo.top

[C11] 模块导入与导出
来源：http://hyq.yangfankeji.com

Py:   from module import func
来源：http://rnx.guowangkeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://kuk.wangshuangyany.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://niw.svipenyu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yrt.yfazqb.com

Java: import java.util.List;
来源：http://ceb.hfpthk.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pdc.pycfn.com

Ruby: require "json"; require_relative "./util"
来源：http://huj.epnwcf.com

C#:   using System.Text;
来源：http://wiq.birdmap.top

[C12] 立即执行函数 IIFE
来源：http://rfn.bbcook.cn

Py:   (lambda: print("run"))()
来源：http://tbx.yuxming.cn

PHP:  (function () { echo "run"; })();
来源：http://cul.bbcook.cn

JS:   (() => { console.log("run"); })();
来源：http://cge.sufxvd.cn

TS:   (() => { console.log("run"); })();
来源：http://aad.tianlin.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tfo.ppjwa.cn

Go:   func() { fmt.Println("run") }()
来源：http://ppk.c1oappe.top

Ruby: -> { puts "run" }.call
来源：http://mmr.zdqjudy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://tjw.nanxinkj.top

[C13] 类型声明 / 类型注解
来源：http://tvg.tianlin.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vki.jqgufenzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kqf.nanxinkj.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ugj.jianghu66.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fud.dianchejie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xpj.hesvh.cn

Go:   func add(a, b int) int
来源：http://jqo.gotoacloud.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mjc.cdnleiting.top

C#:   int Add(int a, int b) => a + b;
来源：http://fcu.fktsv.cn

[C14] 泛型函数
来源：http://ypa.jyoumei.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nzi.ybcxt.top

PHP:  // 无泛型
来源：http://abk.jinqigfzy.top

JS:   // 无泛型
来源：http://ypl.zdbjq.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://whq.zhongyouzk.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ycd.hongshengwenyu.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jfx.zhiwuduotai.top

Ruby: # 无泛型
来源：http://zpy.tanke756.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ghh.52xcode.cn

[C15] 解构 / 展开参数
来源：http://ptr.xingfuxueyuan.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lfi.shanyushiyangkeji.top

PHP:  [$a, $b] = $pair;
来源：http://sns.gotoacloud.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://upy.chenzaomai.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dda.xziqi.cn

Java: // 无解构
来源：http://nfw.chenlongwang.top

Go:   // 无解构
来源：http://kyj.hnqzz.top

Ruby: a, b = pair
来源：http://tai.nanxuanxn.top

C#:   var (a, b) = pair;
来源：http://mun.pycfn.com

[C16] 函数 / 方法重载
来源：http://gwl.c1oappe.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hny.iojbl.cn

PHP:  // 无重载
来源：http://hmb.nwbrower.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://lws.zhixingplan.top

TS:   // 用联合类型或重载签名声明
来源：http://iqo.birdmap.top

Java: void f(int a) {}  void f(String a) {}
来源：http://jja.yj20258.top

Go:   // 无重载：用不同函数名
来源：http://rxt.snrcjt.cn

Ruby: # 无重载：靠动态参数
来源：http://nar.ivvv.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://bct.gaohongyu789.top

================================================================================
来源：http://poc.xuetiantiany.cn

D. 数组 / 列表 / 集合
来源：http://eok.gogol.net.cn

================================================================================
来源：http://xcp.sysykeji.top

[D01] 创建数组 / 列表
来源：http://rhx.redwolf501.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://qfy.jqgfzy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bhm.tarul.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://emq.feifeiyinyue.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://qoe.52xcode.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jni.yongpay.top

Go:   arr := []int{1, 2, 3}
来源：http://qja.fanxiaobao.xyz

Ruby: arr = [1, 2, 3]
来源：http://tuy.ivvv.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://juu.jinyuanbaomall.cn

[D02] 追加元素到末尾
来源：http://wvw.pycfn.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://meg.yanxiufei.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hng.aizwys.cn

JS:   arr.push(4);
来源：http://mxt.snrcjt.cn

TS:   arr.push(4);
来源：http://asz.wangshuangyany.cn

Java: list.add(4);
来源：http://ciw.shzxlz.cn

Go:   arr = append(arr, 4)
来源：http://vpw.zhixingplan.top

Ruby: arr << 4; arr.push(5)
来源：http://hla.jlsjyb.cn

C#:   list.Add(4);
来源：http://tip.gaohongyu789.top

[D03] 在指定位置插入元素
来源：http://fjh.jqgufenzy.top

Py:   arr.insert(0, 0)
来源：http://nlr.cashguo.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bwm.gzhubu.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cmp.jinghuilouyu.cn

TS:   arr.splice(0, 0, 0);
来源：http://hme.sysykeji.top

Java: list.add(0, 0);
来源：http://wqy.shangyingyoupin.top

Go:   arr = append([]int{0}, arr...)
来源：http://sip.jinqigfzy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ptw.ywan-chungtsiang.top

C#:   list.Insert(0, 0);
来源：http://bpc.yj202588.top

[D04] 删除元素
来源：http://tlm.zdbjq.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://asv.xylfe.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pjk.gotoacloud.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qtv.wangshuangyany.cn

TS:   arr.splice(0, 1);
来源：http://csl.yueranfly.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://uyt.cdnleiting.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mhm.hnqzz.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wrr.cqqwz.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uso.zhengqikj.top

[D05] 访问与修改元素
来源：http://jiv.nanxuanxn.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tva.xuanzx.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qlh.daxiang520.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vwe.chenjidiqi.icu

TS:   arr[0]; arr.at(-1);
来源：http://crp.jinghuilouyu.cn

Java: list.get(0); list.set(0, 9);
来源：http://orl.pengpengdd.cyou


<!-- 参考信息 -->
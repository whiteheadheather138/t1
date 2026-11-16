代发 wailian999

[B05] 遍历数组 / 列表
来源：http://hlw.zhijiandao.cn

Py:   for item in arr: print(item)
来源：http://bdd.jinqigfzy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tpu.yfazqb.com

JS:   for (const item of arr) { console.log(item); }
来源：http://urt.jyoumei.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://lzg.yfazqb.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://row.gogol.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hqx.yongpay.top

Ruby: arr.each { |item| puts item }
来源：http://fnu.dianchejie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gca.shanyushiyangtech.top

[B06] 遍历字典 / 对象
来源：http://mnr.hywenlv.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://paz.wangdashe.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bsm.ctjpmb.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pxg.yuxming.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mjb.shanyushiyangkeji.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://nyf.fanxiaobao.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nhr.havefunace.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ztd.gogol.net.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bnv.jlsjyb.cn

[B07] while 循环
来源：http://nrx.ppjwa.cn

Py:   while i < 10: i += 1
来源：http://xzv.jiagoushi.top

PHP:  while ($i < 10) { $i++; }
来源：http://zod.zdbjq.cn

JS:   while (i < 10) { i++; }
来源：http://apu.tarul.cn

TS:   while (i < 10) { i++; }
来源：http://klr.yangfankeji.com

Java: while (i < 10) { i++; }
来源：http://tfi.ydzc1.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qlr.jinghuilouyu.cn

Ruby: while i < 10; i += 1; end
来源：http://mht.ehwqpu.com

C#:   while (i < 10) { i++; }
来源：http://rag.kuanghao11.cn

[B08] do-while（至少执行一次）
来源：http://vle.redwolf501.top

Py:   # 无 do-while：用 while True + break
来源：http://ngg.cqqwz.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qng.svipenyu.cn

JS:   do { i++; } while (i < 10);
来源：http://jom.hesvh.cn

TS:   do { i++; } while (i < 10);
来源：http://kht.sxryk.cn

Java: do { i++; } while (i < 10);
来源：http://hiq.shanyushiyangtech.top

Go:   for { i++; if i >= 10 { break } }
来源：http://oed.chenzaomai.com

Ruby: begin; i += 1; end while i < 10
来源：http://bst.cheryme.top

C#:   do { i++; } while (i < 10);
来源：http://wmn.yonumen.top

[B09] break 与 continue
来源：http://axd.gaohongyu789.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fqg.52xcode.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vjm.shangyingyoupin.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ety.cucudq.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pks.ivvv.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ift.xuetiantiany.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wgx.jlsjyb.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://emq.xuanzx.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vyc.andypj.xyz

[B10] 遍历同时拿索引
来源：http://omu.zhiwuduotai.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dsz.52xcode.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nxx.jiagoushi.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ihn.svipenyu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mmw.shangyingyoupin.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://thl.tarul.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ybv.wangdashe.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xjx.hysaishi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vqx.quarkkingdee.top

[B11] 生成数字序列 / 区间
来源：http://mex.nanxinkj.top

Py:   list(range(0, 10, 2))
来源：http://dcw.hnqzz.top

PHP:  range(0, 10, 2);
来源：http://kss.cashguo.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://suw.jinyuanbaomall.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vqk.tianlin.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://iid.hysaishi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nwc.fktsv.cn

Ruby: (0...10).step(2).to_a
来源：http://yys.tarul.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gnp.sweek.top

[B12] 跳出多层循环
来源：http://axt.ehwqpu.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://idt.nwbrower.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://wxm.chenzaomai.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fcd.zhiwuduotai.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lku.shuidangran.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fxz.birdmap.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://czj.sxryk.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mos.quarkkingdee.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hys.0kj1m.cn

[B13] 判断是否为数字
来源：http://ndj.yongpay.top

Py:   isinstance(x, (int, float))
来源：http://qsz.jqgufenzy.top

PHP:  is_numeric($x)
来源：http://laf.pycfn.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://duc.0kj1m.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qpn.cheryme.top

Java: x instanceof Number
来源：http://viy.chenlongwang.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bap.sxryk.cn

Ruby: x.is_a?(Numeric)
来源：http://ywl.yuanzhike.top

C#:   x is int or double or decimal
来源：http://rco.ydzc1.top

[B14] 判断值是否在集合内
来源：http://urz.tian-w.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bqb.zhijiandao.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nth.yuxming.cn

JS:   [1, 2, 3].includes(x)
来源：http://rng.zdbjq.cn

TS:   [1, 2, 3].includes(x)
来源：http://xqc.meibo888.top

Java: List.of(1, 2, 3).contains(x)
来源：http://pan.xuanzx.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zwh.jlsjyb.cn

Ruby: [1, 2, 3].include?(x)
来源：http://bsv.yuanzhike.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://noi.shanyushiyangtech.top

[B15] 布尔运算与取反
来源：http://dwk.jlsjyb.cn

Py:   a and b or not c
来源：http://vbh.hnqzz.top

PHP:  $a && $b || !$c
来源：http://wau.birdmap.top

JS:   a && b || !c
来源：http://lzd.xingfuxueyuan.xyz

TS:   a && b || !c
来源：http://rmz.zhixingplan.top

Java: a && b || !c
来源：http://wnk.hnxiangtu.top

Go:   a && b || !c
来源：http://xpz.guowangkeji.top

Ruby: a && b || !c
来源：http://eoo.hesvh.cn

C#:   a && b || !c
来源：http://hpv.hysaishi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fes.316326.xyz

Py:   if not data: return
来源：http://omd.mhx1999.top

PHP:  if (!$data) { return; }
来源：http://jla.fehbvm.com

JS:   if (!data) return;
来源：http://cbu.yfazqb.com

TS:   if (!data) return;
来源：http://ymn.meibo888.top

Java: if (data == null) return;
来源：http://smv.uphjek.com

Go:   if data == nil { return }
来源：http://zkt.mhx1999.top

Ruby: return if data.nil?
来源：http://sxh.jinghuilouyu.cn

C#:   if (data == null) return;
来源：http://gtq.zdbjq.cn

================================================================================
来源：http://mvr.cdnleiting.top

C. 函数与作用域
来源：http://vwy.yonumen.top

================================================================================
来源：http://hxz.tanke756.top

[C01] 定义函数
来源：http://pnq.wangdashe.top

Py:   def add(a, b): return a + b
来源：http://djo.ppjwa.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ixp.fktsv.cn

JS:   function add(a, b) { return a + b; }
来源：http://uag.hcnkem.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bne.chenzaomai.com

Java: static int add(int a, int b) { return a + b; }
来源：http://ppj.xziqi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://gmn.nanxuanxn.top

Ruby: def add(a, b); a + b; end
来源：http://epl.birdmap.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nzg.zhongyouzk.top

[C02] 默认参数
来源：http://umk.52xcode.cn

Py:   def greet(name="World"): return name
来源：http://axy.fengsongda.top

PHP:  function greet($name = "World") { return $name; }
来源：http://utv.meibo888.top

JS:   function greet(name = "World") { return name; }
来源：http://djd.nwbrower.top

TS:   function greet(name: string = "World") { return name; }
来源：http://rce.nanxuanxn.top

Java: // 无默认参数：方法重载或 Optional
来源：http://teh.bjfxy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nfn.yuanzhike.top

Ruby: def greet(name = "World") = name
来源：http://pxm.sweek.top

C#:   string Greet(string name = "World") => name;
来源：http://nby.sufxvd.cn

[C03] 可变参数
来源：http://bas.hnqzz.top

Py:   def total(*args): return sum(args)
来源：http://qhy.quarkkingdee.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mnd.shanyushiyangtech.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gjk.uphjek.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://adc.uphjek.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cog.birdmap.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qru.guowangkeji.top

Ruby: def total(*nums); nums.sum; end
来源：http://hur.smart0.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yvf.ppjwa.cn

[C04] 命名参数 / 关键字参数
来源：http://usw.xziqi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hic.tian-w.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://axv.hnxiangtu.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jjc.uphjek.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qqk.yfazqb.com

Java: // 无：用 Builder 模式或 record
来源：http://ibx.dianchejie.cn

Go:   // 无：用配置结构体参数
来源：http://xsp.iojbl.cn

Ruby: f(a: 1, b: 2)
来源：http://zca.fzhhl.top

C#:   f(a: 1, b: 2)
来源：http://oia.sysykeji.top

[C05] 返回多个值
来源：http://fpr.tarul.cn

Py:   return a, b
来源：http://axq.xylfe.cn

PHP:  return [$a, $b];
来源：http://lww.zycfv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wkh.yangfankeji.com

TS:   return { a, b };
来源：http://eco.sxryk.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://oig.chenjidiqi.icu

Go:   return a, b
来源：http://ixa.yangfankeji.com

Ruby: return a, b
来源：http://txu.gogol.net.cn

C#:   return (a, b);              // ValueTuple
来源：http://ohy.ppjwa.cn

[C06] 匿名函数 / lambda
来源：http://fby.chenzaomai.com

Py:   square = lambda x: x * x
来源：http://fjy.yvedp.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://adf.cdnleiting.top

JS:   const square = x => x * x;
来源：http://nas.xinyue.icu

TS:   const square = (x: number): number => x * x;
来源：http://bap.dianchejie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pez.cashguo.top

Go:   sq := func(x int) int { return x * x }
来源：http://vfy.yfazqb.com

Ruby: square = ->(x) { x * x }
来源：http://uyr.iojbl.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hyu.zdqjudy.top

[C07] 把函数作为参数传入
来源：http://kuc.zdbjq.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tzh.sweek.top

PHP:  array_map("strtoupper", $arr);
来源：http://fme.dianchejie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cxh.zhengqikj.top

TS:   arr.map(String)
来源：http://xtj.hammf.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xjf.snrcjt.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dxz.cdnleiting.top

Ruby: arr.map(&:upcase)
来源：http://cbc.yuanzhike.top

C#:   arr.Select(s => s.ToUpper())
来源：http://qzj.sysykeji.top

[C08] 闭包
来源：http://nxn.ctjpmb.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bmf.tian-w.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yhg.quarkkingdee.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://moe.ivvv.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://utp.guowangkeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qnk.jyoumei.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mxi.yuxming.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rmz.cqqwz.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dxj.nwbrower.top

[C09] 递归
来源：http://nlx.zhixingplan.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mso.hesvh.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ffu.iojbl.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qny.jlsjyb.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jcx.wangshuangyany.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xul.sysykeji.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ruq.guannengcc.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dwk.jqgfzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wwj.wangdashe.top

[C10] 变量作用域
来源：http://lcd.0kj1m.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://iyy.kuanghao11.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mud.guannengcc.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lns.birdmap.top

TS:   同 JS
来源：http://auw.pengpengdd.cyou

Java: 方法内为块级作用域
来源：http://naf.0kj1m.cn

Go:   花括号块级作用域
来源：http://qyb.uphjek.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kry.tian-w.cn

C#:   块级作用域
来源：http://dii.jinghuilouyu.cn

[C11] 模块导入与导出
来源：http://yvo.haohaochexian.top

Py:   from module import func
来源：http://rwj.hywenlv.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://lzj.yuxming.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://aqu.nanxuanxn.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kmz.jqgfzy.top

Java: import java.util.List;
来源：http://hfi.tianlin.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://umk.shzxlz.cn

Ruby: require "json"; require_relative "./util"
来源：http://jwy.jyoumei.cn

C#:   using System.Text;
来源：http://ina.cqqwz.cn

[C12] 立即执行函数 IIFE
来源：http://hdk.yfazqb.com

Py:   (lambda: print("run"))()
来源：http://ueb.guowangkeji.top

PHP:  (function () { echo "run"; })();
来源：http://bfz.daria6918.cn

JS:   (() => { console.log("run"); })();
来源：http://bsn.hcnkem.com

TS:   (() => { console.log("run"); })();
来源：http://abe.jianghu66.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xwp.dianchejie.cn

Go:   func() { fmt.Println("run") }()
来源：http://vxq.gzhubu.top

Ruby: -> { puts "run" }.call
来源：http://puj.ivvv.top

C#:   // 无 IIFE：用静态构造函数
来源：http://uex.nanxinkj.top

[C13] 类型声明 / 类型注解
来源：http://iqy.gotoacloud.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jsb.zdbjq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mhs.jyoumei.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://uku.shzxlz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xkg.smart0.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://oxw.shanyushiyangtech.top

Go:   func add(a, b int) int
来源：http://szq.xuetiantiany.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hba.bjfxy.top

C#:   int Add(int a, int b) => a + b;
来源：http://qvq.zhoulong.xyz

[C14] 泛型函数
来源：http://acp.sysykeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cff.zhijiandao.cn

PHP:  // 无泛型
来源：http://wxd.sufxvd.cn

JS:   // 无泛型
来源：http://chs.ctjpmb.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yiq.zdbjq.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yxf.jinghuilouyu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kdh.ywan-chungtsiang.top

Ruby: # 无泛型
来源：http://pks.jqgfzy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dez.hfpthk.cn

[C15] 解构 / 展开参数
来源：http://zik.haohaochexian.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fyr.quarkkingdee.top

PHP:  [$a, $b] = $pair;
来源：http://ims.sjlbkw.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dao.daxiang520.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://afo.vqdsnc.cn

Java: // 无解构
来源：http://lqu.yvedp.cn

Go:   // 无解构
来源：http://qfc.aizwys.cn

Ruby: a, b = pair
来源：http://yli.gogol.net.cn

C#:   var (a, b) = pair;
来源：http://yqh.tianlin.xyz

[C16] 函数 / 方法重载
来源：http://aev.redwolf501.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pjp.0kj1m.cn

PHP:  // 无重载
来源：http://yyo.ydjk.org.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qlw.hcnkem.com

TS:   // 用联合类型或重载签名声明
来源：http://ove.tanke756.top

Java: void f(int a) {}  void f(String a) {}
来源：http://lma.zhiwuduotai.top

Go:   // 无重载：用不同函数名
来源：http://qqz.gzhubu.top

Ruby: # 无重载：靠动态参数
来源：http://xeb.jqgufenzy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://bxh.ydzc1.top

================================================================================
来源：http://xkg.fzhhl.top

D. 数组 / 列表 / 集合
来源：http://mnf.uphjek.com

================================================================================
来源：http://bre.ywan-chungtsiang.top

[D01] 创建数组 / 列表
来源：http://hid.sweek.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://zba.nanxinkj.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cye.andypj.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hyu.chenzaomai.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://axw.chenjidiqi.icu

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nhu.yj20258.top

Go:   arr := []int{1, 2, 3}
来源：http://lth.yongpay.top

Ruby: arr = [1, 2, 3]
来源：http://dvc.ydzc1.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qjm.tianlin.xyz

[D02] 追加元素到末尾
来源：http://sid.gogol.net.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mas.ehwqpu.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hqj.zhongyouzk.top

JS:   arr.push(4);
来源：http://gko.jianghu66.top

TS:   arr.push(4);
来源：http://hcl.vqdsnc.cn

Java: list.add(4);
来源：http://sxw.feifeiyinyue.top

Go:   arr = append(arr, 4)
来源：http://guh.sufxvd.cn

Ruby: arr << 4; arr.push(5)
来源：http://oid.cheryme.top

C#:   list.Add(4);
来源：http://kzs.ydzc1.top

[D03] 在指定位置插入元素
来源：http://tqm.nanxuanxn.top

Py:   arr.insert(0, 0)
来源：http://hwc.dashuyun.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pvp.daxiang520.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ioa.fktsv.cn

TS:   arr.splice(0, 0, 0);
来源：http://ogk.c1oappe.top

Java: list.add(0, 0);
来源：http://aol.xziqi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://lxx.yongpay.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://aqa.zhijiandao.cn

C#:   list.Insert(0, 0);
来源：http://qxz.xuetiantiany.cn

[D04] 删除元素
来源：http://mxg.xinyue.icu

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://aae.zhiwuduotai.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pmc.shanyushiyangkeji.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hgd.smart0.xyz

TS:   arr.splice(0, 1);
来源：http://rux.yuxming.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jrt.wangshuangyany.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hrx.cashguo.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wmc.zhixingplan.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qej.ydjk.org.cn

[D05] 访问与修改元素
来源：http://zap.guannengcc.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://iym.jinghuilouyu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ygb.guowangkeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yqw.yongpay.top

TS:   arr[0]; arr.at(-1);
来源：http://luv.fanxiaobao.xyz

Java: list.get(0); list.set(0, 9);
来源：http://yro.sufxvd.cn


<!-- 参考信息 -->
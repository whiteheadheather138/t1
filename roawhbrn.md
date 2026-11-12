代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://det.xuetiantiany.cn

[B06] 遍历字典 / 对象
来源：http://ube.hammf.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://azw.zhijiandao.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gex.jianghu66.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cni.redwolf501.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lkl.zhongyouzk.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gtg.ehwqpu.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://emh.birdmap.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wsi.zhijiandao.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://oaj.yongpay.top

[B07] while 循环
来源：http://slm.bbcook.cn

Py:   while i < 10: i += 1
来源：http://pwt.snrcjt.cn

PHP:  while ($i < 10) { $i++; }
来源：http://pja.shanyushiyangkeji.top

JS:   while (i < 10) { i++; }
来源：http://zxv.ywan-chungtsiang.top

TS:   while (i < 10) { i++; }
来源：http://csp.chenlongwang.top

Java: while (i < 10) { i++; }
来源：http://zof.gaohongyu789.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sgk.chenjidiqi.icu

Ruby: while i < 10; i += 1; end
来源：http://jiq.fzhhl.top

C#:   while (i < 10) { i++; }
来源：http://mbj.yfazqb.com

[B08] do-while（至少执行一次）
来源：http://ita.redwolf501.top

Py:   # 无 do-while：用 while True + break
来源：http://lrf.haohaochexian.top

PHP:  do { $i++; } while ($i < 10);
来源：http://mmx.hywenlv.cn

JS:   do { i++; } while (i < 10);
来源：http://nuv.bbcook.cn

TS:   do { i++; } while (i < 10);
来源：http://lmi.fzhhl.top

Java: do { i++; } while (i < 10);
来源：http://wkp.jinqigfzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://bvl.wangshuangyany.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ssj.yfazqb.com

C#:   do { i++; } while (i < 10);
来源：http://rqg.pycfn.com

[B09] break 与 continue
来源：http://gbs.birdmap.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://juw.feifeiyinyue.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nxl.ywan-chungtsiang.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rzz.yj20258.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mko.pycfn.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tmr.jyoumei.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sst.shanyushiyangkeji.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://uyd.zhijiandao.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://acw.gotoacloud.top

[B10] 遍历同时拿索引
来源：http://qjs.tarul.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://aeg.kuanghao11.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ozt.yuanzhike.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://luq.smart0.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jse.gzhubu.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sgh.chenjidiqi.icu

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hlg.yj20258888.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ubl.wangshuangyany.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jiq.hfpthk.cn

[B11] 生成数字序列 / 区间
来源：http://lyx.birdmap.top

Py:   list(range(0, 10, 2))
来源：http://cyk.zhongyouzk.top

PHP:  range(0, 10, 2);
来源：http://bla.jinghuilouyu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ysl.jinqigufen.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ddt.cdnleiting.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kgn.hcnkem.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pkg.chenlongwang.top

Ruby: (0...10).step(2).to_a
来源：http://msi.ppjwa.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zcd.yvedp.cn

[B12] 跳出多层循环
来源：http://vcq.gotoacloud.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://gyy.hfpthk.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fvq.uphjek.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://boh.aibaodan.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yat.nanxuanxn.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zrm.xuanzx.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://orp.daria6918.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pqc.jinqigufen.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://aeg.yj20258888.top

[B13] 判断是否为数字
来源：http://mxm.yonumen.top

Py:   isinstance(x, (int, float))
来源：http://ifn.dianchejie.cn

PHP:  is_numeric($x)
来源：http://ita.fktsv.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fim.smart0.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bqv.yfazqb.com

Java: x instanceof Number
来源：http://cyb.hywenlv.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jwu.shanyushiyangtech.top

Ruby: x.is_a?(Numeric)
来源：http://twb.zhoulong.xyz

C#:   x is int or double or decimal
来源：http://ddt.sxryk.cn

[B14] 判断值是否在集合内
来源：http://apm.feifeiyinyue.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pgs.sysykeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kch.yangfankeji.com

JS:   [1, 2, 3].includes(x)
来源：http://qhs.tianlin.xyz

TS:   [1, 2, 3].includes(x)
来源：http://kwe.9152youxi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://zwu.yangfankeji.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wfb.ydjk.org.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ndp.shanyushiyangkeji.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ikc.zycfv.cn

[B15] 布尔运算与取反
来源：http://ehm.jianghu66.top

Py:   a and b or not c
来源：http://xbr.fengsongda.top

PHP:  $a && $b || !$c
来源：http://lym.ctjpmb.com

JS:   a && b || !c
来源：http://jrn.xuetiantiany.cn

TS:   a && b || !c
来源：http://pkd.ppjwa.cn

Java: a && b || !c
来源：http://ska.aizwys.cn

Go:   a && b || !c
来源：http://ple.yuxming.cn

Ruby: a && b || !c
来源：http://fjp.pengpengdd.cyou

C#:   a && b || !c
来源：http://yea.hcnkem.com

[B16] 卫语句：不满足条件提前返回
来源：http://vgn.jianghu66.top

Py:   if not data: return
来源：http://xep.yangfankeji.com

PHP:  if (!$data) { return; }
来源：http://vjg.mhx1999.top

JS:   if (!data) return;
来源：http://bcp.yangfankeji.com

TS:   if (!data) return;
来源：http://prc.yonumen.top

Java: if (data == null) return;
来源：http://gzg.tanke756.top

Go:   if data == nil { return }
来源：http://rcd.tarul.cn

Ruby: return if data.nil?
来源：http://jur.shuidangran.top

C#:   if (data == null) return;
来源：http://axv.vehdjk.com

================================================================================
来源：http://xrx.snrcjt.cn

C. 函数与作用域
来源：http://qct.tanke756.top

================================================================================
来源：http://vuh.guannengcc.top

[C01] 定义函数
来源：http://drq.yueranfly.top

Py:   def add(a, b): return a + b
来源：http://zeq.daria6918.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mee.zhengqikj.top

JS:   function add(a, b) { return a + b; }
来源：http://fws.xingfuxueyuan.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vmw.yuxming.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://rsa.ydzc1.top

Go:   func add(a, b int) int { return a + b }
来源：http://rgj.ctjpmb.com

Ruby: def add(a, b); a + b; end
来源：http://pbg.cucudq.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vqt.jlsjyb.cn

[C02] 默认参数
来源：http://exv.ywan-chungtsiang.top

Py:   def greet(name="World"): return name
来源：http://dxr.52xcode.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://nyj.jqgfzy.top

JS:   function greet(name = "World") { return name; }
来源：http://udk.tanke756.top

TS:   function greet(name: string = "World") { return name; }
来源：http://nlz.birdmap.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ljy.iojbl.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wro.vehdjk.com

Ruby: def greet(name = "World") = name
来源：http://nkc.guowangkeji.top

C#:   string Greet(string name = "World") => name;
来源：http://itx.yongpay.top

[C03] 可变参数
来源：http://eby.ydzc1.top

Py:   def total(*args): return sum(args)
来源：http://uio.quarkkingdee.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ncp.hnxiangtu.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wak.jinghuilouyu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mpo.c1oappe.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hnw.zhaomingkeji.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://oya.hesvh.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ybd.gaohongyu789.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hcy.guannengcc.top

[C04] 命名参数 / 关键字参数
来源：http://pnc.jinghuilouyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://owt.xziqi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kyd.hywenlv.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://swr.pycfn.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ads.jinghuilouyu.cn

Java: // 无：用 Builder 模式或 record
来源：http://qak.nwbrower.top

Go:   // 无：用配置结构体参数
来源：http://fpr.sxryk.cn

Ruby: f(a: 1, b: 2)
来源：http://gib.svipenyu.cn

C#:   f(a: 1, b: 2)
来源：http://ydj.xingfuxueyuan.xyz

[C05] 返回多个值
来源：http://zbe.hesvh.cn

Py:   return a, b
来源：http://wqc.smart0.xyz

PHP:  return [$a, $b];
来源：http://rgi.bbcook.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://mbc.hcnkem.com

TS:   return { a, b };
来源：http://eoh.fzhhl.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nla.svipenyu.cn

Go:   return a, b
来源：http://nkh.fengsongda.top

Ruby: return a, b
来源：http://jzt.nanxinkj.top

C#:   return (a, b);              // ValueTuple
来源：http://xon.chenjidiqi.icu

[C06] 匿名函数 / lambda
来源：http://ajm.birdmap.top

Py:   square = lambda x: x * x
来源：http://ync.xuanzx.com

PHP:  $square = fn($x) => $x * $x;
来源：http://lht.hfpthk.cn

JS:   const square = x => x * x;
来源：http://ncl.sysykeji.top

TS:   const square = (x: number): number => x * x;
来源：http://goc.nanxinkj.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fqv.hfpthk.cn

Go:   sq := func(x int) int { return x * x }
来源：http://kkk.ydjk.org.cn

Ruby: square = ->(x) { x * x }
来源：http://qqf.havefunace.top

C#:   Func<int, int> square = x => x * x;
来源：http://ywr.meibo888.top

[C07] 把函数作为参数传入
来源：http://tqv.pycfn.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://iig.ydjk.org.cn

PHP:  array_map("strtoupper", $arr);
来源：http://alf.jiagoushi.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kfm.meibo888.top

TS:   arr.map(String)
来源：http://dfe.yvedp.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jbo.fzhhl.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uwn.yfazqb.com

Ruby: arr.map(&:upcase)
来源：http://vvt.cqqwz.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hgj.ctjpmb.com

[C08] 闭包
来源：http://sbn.hysaishi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qpl.gaohongyu789.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://amh.xylfe.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fqp.redwolf501.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xtq.snrcjt.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bpp.0kj1m.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bzs.aibaodan.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yjj.fzhhl.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kud.sysykeji.top

[C09] 递归
来源：http://czz.yj20258888.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lls.52xcode.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ort.guannengcc.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pmo.yuxming.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uzg.ctjpmb.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tcn.ywan-chungtsiang.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sve.chenjidiqi.icu

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://oau.ybcxt.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cqp.havefunace.top

[C10] 变量作用域
来源：http://ozz.tarul.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tkg.snrcjt.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://aws.redwolf501.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fhn.yj20258.top

TS:   同 JS
来源：http://xkr.hcnkem.com

Java: 方法内为块级作用域
来源：http://ked.zdqjudy.top

Go:   花括号块级作用域
来源：http://aaj.316326.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uqe.hesvh.cn

C#:   块级作用域
来源：http://phe.fengsongda.top

[C11] 模块导入与导出
来源：http://ntu.ivvv.top

Py:   from module import func
来源：http://zjk.sxryk.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://dby.hammf.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://gig.zhijiandao.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lbu.xziqi.cn

Java: import java.util.List;
来源：http://idz.fehbvm.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://idm.nwbrower.top

Ruby: require "json"; require_relative "./util"
来源：http://xik.gogol.net.cn

C#:   using System.Text;
来源：http://knf.xuanzx.com

[C12] 立即执行函数 IIFE
来源：http://txw.9152youxi.cn

Py:   (lambda: print("run"))()
来源：http://jct.jyoumei.cn

PHP:  (function () { echo "run"; })();
来源：http://zjw.zdqjudy.top

JS:   (() => { console.log("run"); })();
来源：http://hqg.tanke756.top

TS:   (() => { console.log("run"); })();
来源：http://amw.hnxiangtu.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ssj.jiagoushi.top

Go:   func() { fmt.Println("run") }()
来源：http://wkj.redwolf501.top

Ruby: -> { puts "run" }.call
来源：http://pec.iojbl.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://tix.chenlongwang.top

[C13] 类型声明 / 类型注解
来源：http://ghi.chenlongwang.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kyc.andypj.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tna.zhoulong.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tde.xziqi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sxk.shzxlz.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cqw.ctjpmb.com

Go:   func add(a, b int) int
来源：http://xuo.jqgufenzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jjh.sxryk.cn

C#:   int Add(int a, int b) => a + b;
来源：http://jyn.tanke756.top

[C14] 泛型函数
来源：http://tmn.zhengqikj.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://slj.316326.xyz

PHP:  // 无泛型
来源：http://avy.snrcjt.cn

JS:   // 无泛型
来源：http://jfe.yfazqb.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://syg.haohaochexian.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qfh.ppjwa.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pcl.zhongyouzk.top

Ruby: # 无泛型
来源：http://sli.pengpengdd.cyou

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nco.hywenlv.cn

[C15] 解构 / 展开参数
来源：http://oah.xylfe.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yaa.316326.xyz

PHP:  [$a, $b] = $pair;
来源：http://fbn.nanxinkj.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ajd.bjfxy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dbw.zhengqikj.top

Java: // 无解构
来源：http://kri.uphjek.com

Go:   // 无解构
来源：http://bcr.yj20258.top

Ruby: a, b = pair
来源：http://jtv.sjlbkw.cn

C#:   var (a, b) = pair;
来源：http://thr.xuetiantiany.cn

[C16] 函数 / 方法重载
来源：http://udc.ywan-chungtsiang.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://guv.meibo888.top

PHP:  // 无重载
来源：http://fgu.cheryme.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://nxd.xinyue.icu

TS:   // 用联合类型或重载签名声明
来源：http://ptf.yuanzhike.top

Java: void f(int a) {}  void f(String a) {}
来源：http://kyw.epnwcf.com

Go:   // 无重载：用不同函数名
来源：http://kwi.cashguo.top

Ruby: # 无重载：靠动态参数
来源：http://wox.yanxiufei.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://yem.aibaodan.cn

================================================================================
来源：http://ajj.yonumen.top

D. 数组 / 列表 / 集合
来源：http://wdh.mhx1999.top

================================================================================
来源：http://wxe.zdbjq.cn

[D01] 创建数组 / 列表
来源：http://glv.ydjk.org.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://chi.ydjk.org.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qyk.svipenyu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tvo.fzhhl.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://fas.vqdsnc.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://aor.hongshengwenyu.top

Go:   arr := []int{1, 2, 3}
来源：http://cen.havefunace.top

Ruby: arr = [1, 2, 3]
来源：http://kxs.jinqigufen.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://roj.nwbrower.top

[D02] 追加元素到末尾
来源：http://wpz.yongpay.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fye.quarkkingdee.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wqe.zdbjq.cn

JS:   arr.push(4);
来源：http://qso.mhx1999.top

TS:   arr.push(4);
来源：http://mdo.wangdashe.top

Java: list.add(4);
来源：http://tgl.jlsjyb.cn

Go:   arr = append(arr, 4)
来源：http://cyu.yvedp.cn

Ruby: arr << 4; arr.push(5)
来源：http://cvr.haohaochexian.top

C#:   list.Add(4);
来源：http://dck.ywan-chungtsiang.top

[D03] 在指定位置插入元素
来源：http://pko.zdqjudy.top

Py:   arr.insert(0, 0)
来源：http://gcv.xuetiantiany.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://srx.redwolf501.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qkf.smart0.xyz

TS:   arr.splice(0, 0, 0);
来源：http://ukh.daxiang520.top

Java: list.add(0, 0);
来源：http://wrz.shanyushiyangkeji.top

Go:   arr = append([]int{0}, arr...)
来源：http://kli.dianchejie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zaf.mhx1999.top

C#:   list.Insert(0, 0);
来源：http://ypy.aizwys.cn

[D04] 删除元素
来源：http://ypn.dianchejie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jww.yj202588.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sjx.uphjek.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rja.yuxming.cn

TS:   arr.splice(0, 1);
来源：http://tyv.pengpengdd.cyou

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://geu.shuidangran.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ttg.jinqigufen.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ffs.xuetiantiany.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fwj.cucudq.cn

[D05] 访问与修改元素
来源：http://uws.pengpengdd.cyou

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yio.tanke756.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://iuz.nwbrower.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kgk.fanxiaobao.xyz

TS:   arr[0]; arr.at(-1);
来源：http://auf.cheryme.top

Java: list.get(0); list.set(0, 9);
来源：http://tao.yj20258.top

Go:   arr[0]; arr[0] = 9
来源：http://pzs.jlsjyb.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vsc.tarul.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wwe.yuxming.cn

[D06] 数组长度
来源：http://cib.52xcode.cn

Py:   len(arr)
来源：http://xzs.pycfn.com

PHP:  count($arr);
来源：http://uqi.smart0.xyz

JS:   arr.length
来源：http://rbd.jinqigfzy.top

TS:   arr.length
来源：http://hzl.hysaishi.cn


<!-- 参考信息 -->
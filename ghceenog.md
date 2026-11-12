代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://siw.ppjwa.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ldv.c1oappe.top

Ruby: 10.times { |i| puts i }
来源：http://yvt.vqdsnc.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jeb.fengsongda.top

[B05] 遍历数组 / 列表
来源：http://law.nanxinkj.top

Py:   for item in arr: print(item)
来源：http://ifz.fehbvm.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lpp.jlsjyb.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://pjm.iojbl.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bla.zycfv.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://rxp.ehwqpu.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cdj.0kj1m.cn

Ruby: arr.each { |item| puts item }
来源：http://mel.zdqjudy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ysf.snrcjt.cn

[B06] 遍历字典 / 对象
来源：http://grs.ehwqpu.com

Py:   for k, v in d.items(): print(k, v)
来源：http://kiw.nanxinkj.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://phd.hnxiangtu.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dcl.c1oappe.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xdv.yj202588.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bck.cdnleiting.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kwz.ctjpmb.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jyq.gzhubu.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://odv.yfazqb.com

[B07] while 循环
来源：http://dnt.zdqjudy.top

Py:   while i < 10: i += 1
来源：http://gyx.tanke756.top

PHP:  while ($i < 10) { $i++; }
来源：http://dpt.ydjk.org.cn

JS:   while (i < 10) { i++; }
来源：http://bkm.fanxiaobao.xyz

TS:   while (i < 10) { i++; }
来源：http://tqu.cqqwz.cn

Java: while (i < 10) { i++; }
来源：http://zci.c1oappe.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://llm.pengpengdd.cyou

Ruby: while i < 10; i += 1; end
来源：http://kli.quarkkingdee.top

C#:   while (i < 10) { i++; }
来源：http://nup.xinyue.icu

[B08] do-while（至少执行一次）
来源：http://rzp.yj20258.top

Py:   # 无 do-while：用 while True + break
来源：http://ppk.yueranfly.top

PHP:  do { $i++; } while ($i < 10);
来源：http://hxp.fehbvm.com

JS:   do { i++; } while (i < 10);
来源：http://jaj.zhengqikj.top

TS:   do { i++; } while (i < 10);
来源：http://xja.hesvh.cn

Java: do { i++; } while (i < 10);
来源：http://cma.xuetiantiany.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sxw.jinqigfzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://vzl.hnxiangtu.top

C#:   do { i++; } while (i < 10);
来源：http://lnp.fanxiaobao.xyz

[B09] break 与 continue
来源：http://ota.quarkkingdee.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://owl.gogol.net.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ucr.hywenlv.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://teh.pengpengdd.cyou

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xbj.cashguo.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://doz.kuanghao11.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://crk.andypj.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://sdm.zycfv.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xww.ehwqpu.com

[B10] 遍历同时拿索引
来源：http://dwq.hysaishi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sri.hysaishi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lwo.daria6918.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://prg.smart0.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nww.ybcxt.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://itp.hywenlv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dny.hnqzz.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://loa.yfazqb.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nye.yangfankeji.com

[B11] 生成数字序列 / 区间
来源：http://pwg.guannengcc.top

Py:   list(range(0, 10, 2))
来源：http://hwb.aizwys.cn

PHP:  range(0, 10, 2);
来源：http://sdb.xuanzx.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jbk.havefunace.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vqe.yueranfly.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://irh.wangshuangyany.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vem.yonumen.top

Ruby: (0...10).step(2).to_a
来源：http://oiq.dashuyun.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ams.jinghuilouyu.cn

[B12] 跳出多层循环
来源：http://vvn.9152youxi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ngc.yvedp.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zgt.nanxinkj.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zbx.jyoumei.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mia.xingfuxueyuan.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qtl.hnxiangtu.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://muy.daria6918.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://uoa.gogol.net.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cco.xinyue.icu

[B13] 判断是否为数字
来源：http://qiv.tian-w.cn

Py:   isinstance(x, (int, float))
来源：http://vqq.dashuyun.cn

PHP:  is_numeric($x)
来源：http://wuc.shuidangran.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ruu.pengpengdd.cyou

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xtm.0kj1m.cn

Java: x instanceof Number
来源：http://onj.zhongyouzk.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zbf.zhiwuduotai.top

Ruby: x.is_a?(Numeric)
来源：http://eea.pengpengdd.cyou

C#:   x is int or double or decimal
来源：http://cek.gotoacloud.top

[B14] 判断值是否在集合内
来源：http://ckx.sjlbkw.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rox.fanxiaobao.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pfg.redwolf501.top

JS:   [1, 2, 3].includes(x)
来源：http://oxi.zhixingplan.top

TS:   [1, 2, 3].includes(x)
来源：http://ayl.zhiwuduotai.top

Java: List.of(1, 2, 3).contains(x)
来源：http://dsh.zycfv.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://och.9152youxi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://afa.epnwcf.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gzx.jiagoushi.top

[B15] 布尔运算与取反
来源：http://hjm.jinyuanbaomall.cn

Py:   a and b or not c
来源：http://ohj.sxryk.cn

PHP:  $a && $b || !$c
来源：http://epr.sysykeji.top

JS:   a && b || !c
来源：http://jqg.uphjek.com

TS:   a && b || !c
来源：http://hkl.sufxvd.cn

Java: a && b || !c
来源：http://rgu.shuidangran.top

Go:   a && b || !c
来源：http://gth.uphjek.com

Ruby: a && b || !c
来源：http://tbd.hfpthk.cn

C#:   a && b || !c
来源：http://naw.nanxuanxn.top

[B16] 卫语句：不满足条件提前返回
来源：http://ylp.fanxiaobao.xyz

Py:   if not data: return
来源：http://rnu.sxryk.cn

PHP:  if (!$data) { return; }
来源：http://srb.zhixingplan.top

JS:   if (!data) return;
来源：http://hso.hammf.cn

TS:   if (!data) return;
来源：http://saf.jqgfzy.top

Java: if (data == null) return;
来源：http://cxl.cdnleiting.top

Go:   if data == nil { return }
来源：http://czm.aizwys.cn

Ruby: return if data.nil?
来源：http://hwb.fktsv.cn

C#:   if (data == null) return;
来源：http://fax.xziqi.cn

================================================================================
来源：http://edl.hysaishi.cn

C. 函数与作用域
来源：http://lmr.svipenyu.cn

================================================================================
来源：http://lil.aibaodan.cn

[C01] 定义函数
来源：http://mxc.cheryme.top

Py:   def add(a, b): return a + b
来源：http://mse.hcnkem.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wmw.ydzc1.top

JS:   function add(a, b) { return a + b; }
来源：http://xcc.hammf.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://snv.zhoulong.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://jud.fengsongda.top

Go:   func add(a, b int) int { return a + b }
来源：http://bct.c1oappe.top

Ruby: def add(a, b); a + b; end
来源：http://aep.yangfankeji.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kfn.zhijiandao.cn

[C02] 默认参数
来源：http://vkg.bjfxy.top

Py:   def greet(name="World"): return name
来源：http://ros.hnxiangtu.top

PHP:  function greet($name = "World") { return $name; }
来源：http://hjf.jiagoushi.top

JS:   function greet(name = "World") { return name; }
来源：http://pbd.meibo888.top

TS:   function greet(name: string = "World") { return name; }
来源：http://vge.xziqi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qnu.redwolf501.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://uew.tian-w.cn

Ruby: def greet(name = "World") = name
来源：http://ckb.jiagoushi.top

C#:   string Greet(string name = "World") => name;
来源：http://wke.bbcook.cn

[C03] 可变参数
来源：http://nhy.hysaishi.cn

Py:   def total(*args): return sum(args)
来源：http://hwv.zdqjudy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pou.andypj.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qft.bbcook.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vur.zhijiandao.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sge.quarkkingdee.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fck.xingfuxueyuan.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://oys.zdbjq.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hyg.0kj1m.cn

[C04] 命名参数 / 关键字参数
来源：http://hgv.yonumen.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jov.zhoulong.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mlw.shanyushiyangkeji.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xld.ywan-chungtsiang.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sbw.yfazqb.com

Java: // 无：用 Builder 模式或 record
来源：http://obz.zhongyouzk.top

Go:   // 无：用配置结构体参数
来源：http://uys.mhx1999.top

Ruby: f(a: 1, b: 2)
来源：http://wrj.tanke756.top

C#:   f(a: 1, b: 2)
来源：http://jjc.daria6918.cn

[C05] 返回多个值
来源：http://yff.hfpthk.cn

Py:   return a, b
来源：http://mne.hammf.cn

PHP:  return [$a, $b];
来源：http://wjs.xylfe.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://emn.pycfn.com

TS:   return { a, b };
来源：http://dys.sxryk.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dxk.yvedp.cn

Go:   return a, b
来源：http://usb.jiagoushi.top

Ruby: return a, b
来源：http://qod.shanyushiyangkeji.top

C#:   return (a, b);              // ValueTuple
来源：http://vdc.vqdsnc.cn

[C06] 匿名函数 / lambda
来源：http://wfz.snrcjt.cn

Py:   square = lambda x: x * x
来源：http://foi.hesvh.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://erf.chenlongwang.top

JS:   const square = x => x * x;
来源：http://cfk.jiagoushi.top

TS:   const square = (x: number): number => x * x;
来源：http://tus.bjfxy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fgq.chenlongwang.top

Go:   sq := func(x int) int { return x * x }
来源：http://slm.wangshuangyany.cn

Ruby: square = ->(x) { x * x }
来源：http://mij.chenjidiqi.icu

C#:   Func<int, int> square = x => x * x;
来源：http://crw.gotoacloud.top

[C07] 把函数作为参数传入
来源：http://kly.sysykeji.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qcy.shangyingyoupin.top

PHP:  array_map("strtoupper", $arr);
来源：http://zik.shuidangran.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://len.gotoacloud.top

TS:   arr.map(String)
来源：http://sfo.xziqi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fux.fanxiaobao.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tae.sxryk.cn

Ruby: arr.map(&:upcase)
来源：http://ckg.ybcxt.top

C#:   arr.Select(s => s.ToUpper())
来源：http://nmd.hnqzz.top

[C08] 闭包
来源：http://atb.haohaochexian.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mic.zdqjudy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sqg.nanxinkj.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qgg.havefunace.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sql.jinqigfzy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nsb.gaohongyu789.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gec.jinqigfzy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nbj.tian-w.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mdr.bbcook.cn

[C09] 递归
来源：http://zao.shanyushiyangtech.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ixy.aibaodan.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pyf.birdmap.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xfi.zhixingplan.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iyg.nanxinkj.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fig.316326.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kwn.52xcode.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yju.ppjwa.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pyp.ivvv.top

[C10] 变量作用域
来源：http://ibq.jlsjyb.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cuy.nanxinkj.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wxj.zhengqikj.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dty.sufxvd.cn

TS:   同 JS
来源：http://rrc.52xcode.cn

Java: 方法内为块级作用域
来源：http://cth.shangyingyoupin.top

Go:   花括号块级作用域
来源：http://ozt.cucudq.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://umu.andypj.xyz

C#:   块级作用域
来源：http://suq.tanke756.top

[C11] 模块导入与导出
来源：http://erm.uphjek.com

Py:   from module import func
来源：http://xzr.jianghu66.top

PHP:  require "file.php";  或 use App\Service;
来源：http://vvv.cashguo.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://fbz.jianghu66.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kgb.gaohongyu789.top

Java: import java.util.List;
来源：http://wme.zdbjq.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mui.gaohongyu789.top

Ruby: require "json"; require_relative "./util"
来源：http://mri.dianchejie.cn

C#:   using System.Text;
来源：http://rbz.tanke756.top

[C12] 立即执行函数 IIFE
来源：http://scj.ydjk.org.cn

Py:   (lambda: print("run"))()
来源：http://vyq.xuanzx.com

PHP:  (function () { echo "run"; })();
来源：http://lsa.hfpthk.cn

JS:   (() => { console.log("run"); })();
来源：http://ycp.zdqjudy.top

TS:   (() => { console.log("run"); })();
来源：http://nke.mhx1999.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lvc.cucudq.cn

Go:   func() { fmt.Println("run") }()
来源：http://gjo.hysaishi.cn

Ruby: -> { puts "run" }.call
来源：http://ira.chenjidiqi.icu

C#:   // 无 IIFE：用静态构造函数
来源：http://oxk.cucudq.cn

[C13] 类型声明 / 类型注解
来源：http://jzq.aizwys.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wkq.tarul.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iqk.iojbl.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lha.jinghuilouyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mmj.kuanghao11.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fcb.vehdjk.com

Go:   func add(a, b int) int
来源：http://iqy.birdmap.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://psc.zhengqikj.top

C#:   int Add(int a, int b) => a + b;
来源：http://tmz.havefunace.top

[C14] 泛型函数
来源：http://joy.ehwqpu.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hah.wangdashe.top

PHP:  // 无泛型
来源：http://dar.hongshengwenyu.top

JS:   // 无泛型
来源：http://zar.dianchejie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pnr.ydjk.org.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kia.c1oappe.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rbg.ppjwa.cn

Ruby: # 无泛型
来源：http://fuy.yuanzhike.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dra.yonumen.top

[C15] 解构 / 展开参数
来源：http://ocu.hfpthk.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pvr.svipenyu.cn

PHP:  [$a, $b] = $pair;
来源：http://exv.fehbvm.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jit.52xcode.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://atz.chenlongwang.top

Java: // 无解构
来源：http://wce.zycfv.cn

Go:   // 无解构
来源：http://sko.redwolf501.top

Ruby: a, b = pair
来源：http://qrw.andypj.xyz

C#:   var (a, b) = pair;
来源：http://ozw.sjlbkw.cn

[C16] 函数 / 方法重载
来源：http://nil.hysaishi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ntl.meibo888.top

PHP:  // 无重载
来源：http://ujc.tanke756.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://tez.dianchejie.cn

TS:   // 用联合类型或重载签名声明
来源：http://ezs.cdnleiting.top

Java: void f(int a) {}  void f(String a) {}
来源：http://tsv.cheryme.top

Go:   // 无重载：用不同函数名
来源：http://oxf.tarul.cn

Ruby: # 无重载：靠动态参数
来源：http://mck.yanxiufei.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rhy.jlsjyb.cn

================================================================================
来源：http://juf.yuxming.cn

D. 数组 / 列表 / 集合
来源：http://uzu.pengpengdd.cyou

================================================================================
来源：http://xcd.yongpay.top

[D01] 创建数组 / 列表
来源：http://wel.bjfxy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://yhj.shzxlz.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://elg.gzhubu.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uub.yj20258.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ccm.yj20258.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ovh.cucudq.cn

Go:   arr := []int{1, 2, 3}
来源：http://udh.yuxming.cn

Ruby: arr = [1, 2, 3]
来源：http://jtd.ctjpmb.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xli.jqgufenzy.top

[D02] 追加元素到末尾
来源：http://yds.ctjpmb.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jrs.vehdjk.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tpz.sysykeji.top

JS:   arr.push(4);
来源：http://wor.sysykeji.top

TS:   arr.push(4);
来源：http://jfl.xuanzx.com

Java: list.add(4);
来源：http://fcz.cashguo.top

Go:   arr = append(arr, 4)
来源：http://jos.yangfankeji.com

Ruby: arr << 4; arr.push(5)
来源：http://wgb.jiagoushi.top

C#:   list.Add(4);
来源：http://prb.fengsongda.top

[D03] 在指定位置插入元素
来源：http://mhh.ybcxt.top

Py:   arr.insert(0, 0)
来源：http://coi.0kj1m.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ttc.guannengcc.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lyk.hongshengwenyu.top

TS:   arr.splice(0, 0, 0);
来源：http://fzu.sysykeji.top

Java: list.add(0, 0);
来源：http://pmt.jinqigfzy.top

Go:   arr = append([]int{0}, arr...)
来源：http://bzl.shangyingyoupin.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gvc.yvedp.cn

C#:   list.Insert(0, 0);
来源：http://tbr.sysykeji.top

[D04] 删除元素
来源：http://pzw.shuidangran.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://njn.yvedp.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ycp.52xcode.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ocg.jinyuanbaomall.cn

TS:   arr.splice(0, 1);
来源：http://thq.shangyingyoupin.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fix.svipenyu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cyx.bbcook.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ibu.pengpengdd.cyou

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hrz.nanxuanxn.top

[D05] 访问与修改元素
来源：http://qjn.shanyushiyangtech.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tnt.yj20258888.top


<!-- 参考信息 -->
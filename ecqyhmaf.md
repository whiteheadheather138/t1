代发 wailian999

[B05] 遍历数组 / 列表
来源：http://bdc.yanxiufei.cn

Py:   for item in arr: print(item)
来源：http://duc.bjfxy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://avx.guowangkeji.top

JS:   for (const item of arr) { console.log(item); }
来源：http://wnr.haohaochexian.top

TS:   for (const item of arr) { console.log(item); }
来源：http://mzg.hfpthk.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zhu.redwolf501.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://clu.ivvv.top

Ruby: arr.each { |item| puts item }
来源：http://shl.gogol.net.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bhe.yfazqb.com

[B06] 遍历字典 / 对象
来源：http://cdc.snrcjt.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://rnp.uphjek.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://czz.havefunace.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mdt.guannengcc.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bfv.zdbjq.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ysg.birdmap.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fvy.fengsongda.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mrf.yangfankeji.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pph.daria6918.cn

[B07] while 循环
来源：http://utg.daxiang520.top

Py:   while i < 10: i += 1
来源：http://xpl.chenjidiqi.icu

PHP:  while ($i < 10) { $i++; }
来源：http://pgv.snrcjt.cn

JS:   while (i < 10) { i++; }
来源：http://dve.pengpengdd.cyou

TS:   while (i < 10) { i++; }
来源：http://slm.xuanzx.com

Java: while (i < 10) { i++; }
来源：http://acz.jlsjyb.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yeu.zhaomingkeji.xyz

Ruby: while i < 10; i += 1; end
来源：http://pap.jinqigfzy.top

C#:   while (i < 10) { i++; }
来源：http://xhe.ydjk.org.cn

[B08] do-while（至少执行一次）
来源：http://ljs.quarkkingdee.top

Py:   # 无 do-while：用 while True + break
来源：http://ehn.jlsjyb.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://sua.bbcook.cn

JS:   do { i++; } while (i < 10);
来源：http://obc.fktsv.cn

TS:   do { i++; } while (i < 10);
来源：http://nvl.guowangkeji.top

Java: do { i++; } while (i < 10);
来源：http://sgo.jinyuanbaomall.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://kel.kuanghao11.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wyk.dashuyun.cn

C#:   do { i++; } while (i < 10);
来源：http://pgr.chenlongwang.top

[B09] break 与 continue
来源：http://kia.cdnleiting.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://efw.svipenyu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bvf.gaohongyu789.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sjg.yueranfly.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aot.uphjek.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gwk.hnqzz.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kld.cucudq.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hir.pengpengdd.cyou

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pyw.mhx1999.top

[B10] 遍历同时拿索引
来源：http://ies.yfazqb.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://imt.xuetiantiany.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gzm.zdqjudy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kln.gotoacloud.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://syr.fanxiaobao.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yav.pengpengdd.cyou

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xtb.ydjk.org.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xhx.hammf.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hns.zdqjudy.top

[B11] 生成数字序列 / 区间
来源：http://icv.chenjidiqi.icu

Py:   list(range(0, 10, 2))
来源：http://pmm.pengpengdd.cyou

PHP:  range(0, 10, 2);
来源：http://oeb.cdnleiting.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ijg.sjlbkw.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://opi.hnqzz.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zxs.tanke756.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zrj.dianchejie.cn

Ruby: (0...10).step(2).to_a
来源：http://zmp.gzhubu.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://djk.0kj1m.cn

[B12] 跳出多层循环
来源：http://veh.bbcook.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://zjj.redwolf501.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ccd.c1oappe.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sxc.yanxiufei.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cfx.zycfv.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xez.shzxlz.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pmp.xinyue.icu

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ofz.andypj.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ozw.hysaishi.cn

[B13] 判断是否为数字
来源：http://jwy.chenzaomai.com

Py:   isinstance(x, (int, float))
来源：http://dmb.ydjk.org.cn

PHP:  is_numeric($x)
来源：http://ubw.0kj1m.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uvy.sjlbkw.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wva.ivvv.top

Java: x instanceof Number
来源：http://uzi.mhx1999.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xpf.jlsjyb.cn

Ruby: x.is_a?(Numeric)
来源：http://xpm.zhiwuduotai.top

C#:   x is int or double or decimal
来源：http://vlt.sxryk.cn

[B14] 判断值是否在集合内
来源：http://smt.guannengcc.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kff.ehwqpu.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bpi.gaohongyu789.top

JS:   [1, 2, 3].includes(x)
来源：http://zin.jqgfzy.top

TS:   [1, 2, 3].includes(x)
来源：http://lpp.yongpay.top

Java: List.of(1, 2, 3).contains(x)
来源：http://osl.zhaomingkeji.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://erp.hywenlv.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ijv.jiagoushi.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wyr.xylfe.cn

[B15] 布尔运算与取反
来源：http://gnz.zhijiandao.cn

Py:   a and b or not c
来源：http://urt.nwbrower.top

PHP:  $a && $b || !$c
来源：http://mca.cqqwz.cn

JS:   a && b || !c
来源：http://anw.zhixingplan.top

TS:   a && b || !c
来源：http://idp.ydzc1.top

Java: a && b || !c
来源：http://zug.shangyingyoupin.top

Go:   a && b || !c
来源：http://fzq.hnxiangtu.top

Ruby: a && b || !c
来源：http://lip.havefunace.top

C#:   a && b || !c
来源：http://jqu.epnwcf.com

[B16] 卫语句：不满足条件提前返回
来源：http://wqi.hnqzz.top

Py:   if not data: return
来源：http://nad.gzhubu.top

PHP:  if (!$data) { return; }
来源：http://qqn.yj20258888.top

JS:   if (!data) return;
来源：http://sdj.jinyuanbaomall.cn

TS:   if (!data) return;
来源：http://jjy.snrcjt.cn

Java: if (data == null) return;
来源：http://mlb.shuidangran.top

Go:   if data == nil { return }
来源：http://sru.ybcxt.top

Ruby: return if data.nil?
来源：http://thj.dianchejie.cn

C#:   if (data == null) return;
来源：http://yzh.wangshuangyany.cn

================================================================================
来源：http://hdr.jianghu66.top

C. 函数与作用域
来源：http://hpv.mhx1999.top

================================================================================
来源：http://axx.zdqjudy.top

[C01] 定义函数
来源：http://bum.yj202588.top

Py:   def add(a, b): return a + b
来源：http://qmw.yvedp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zpn.9152youxi.cn

JS:   function add(a, b) { return a + b; }
来源：http://mbf.jinghuilouyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pls.daria6918.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zlu.tanke756.top

Go:   func add(a, b int) int { return a + b }
来源：http://tlu.jinyuanbaomall.cn

Ruby: def add(a, b); a + b; end
来源：http://hjy.yj20258.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rtl.epnwcf.com

[C02] 默认参数
来源：http://fdq.yongpay.top

Py:   def greet(name="World"): return name
来源：http://ffq.zdqjudy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://gdj.yj20258.top

JS:   function greet(name = "World") { return name; }
来源：http://ijg.ywan-chungtsiang.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ore.iojbl.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://sjm.zhaomingkeji.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zca.shangyingyoupin.top

Ruby: def greet(name = "World") = name
来源：http://xlg.sweek.top

C#:   string Greet(string name = "World") => name;
来源：http://uql.shanyushiyangkeji.top

[C03] 可变参数
来源：http://fbq.xuanzx.com

Py:   def total(*args): return sum(args)
来源：http://cxw.jinghuilouyu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hcv.hesvh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cwo.sufxvd.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gwu.ywan-chungtsiang.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qcm.hysaishi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wmk.nanxinkj.top

Ruby: def total(*nums); nums.sum; end
来源：http://zgp.0kj1m.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wfh.jinyuanbaomall.cn

[C04] 命名参数 / 关键字参数
来源：http://qht.jqgfzy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sil.ybcxt.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://piw.316326.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://man.yj20258.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jkw.xziqi.cn

Java: // 无：用 Builder 模式或 record
来源：http://qza.zycfv.cn

Go:   // 无：用配置结构体参数
来源：http://pvx.ywan-chungtsiang.top

Ruby: f(a: 1, b: 2)
来源：http://ggt.ppjwa.cn

C#:   f(a: 1, b: 2)
来源：http://chm.dashuyun.cn

[C05] 返回多个值
来源：http://ujn.zhengqikj.top

Py:   return a, b
来源：http://aca.vehdjk.com

PHP:  return [$a, $b];
来源：http://nym.tarul.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://auj.yj202588.top

TS:   return { a, b };
来源：http://qfh.iojbl.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qbv.hywenlv.cn

Go:   return a, b
来源：http://tfb.ctjpmb.com

Ruby: return a, b
来源：http://cet.aizwys.cn

C#:   return (a, b);              // ValueTuple
来源：http://tox.gzhubu.top

[C06] 匿名函数 / lambda
来源：http://iwd.chenjidiqi.icu

Py:   square = lambda x: x * x
来源：http://uma.ydjk.org.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://jwo.yanxiufei.cn

JS:   const square = x => x * x;
来源：http://guu.fengsongda.top

TS:   const square = (x: number): number => x * x;
来源：http://vpa.yuxming.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fgy.zhongyouzk.top

Go:   sq := func(x int) int { return x * x }
来源：http://wpp.wangdashe.top

Ruby: square = ->(x) { x * x }
来源：http://yhx.fktsv.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xgi.jqgfzy.top

[C07] 把函数作为参数传入
来源：http://wcc.yfazqb.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xkv.sxryk.cn

PHP:  array_map("strtoupper", $arr);
来源：http://oof.vehdjk.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kfj.fzhhl.top

TS:   arr.map(String)
来源：http://soz.epnwcf.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vfz.fktsv.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lhw.zycfv.cn

Ruby: arr.map(&:upcase)
来源：http://lug.yj20258.top

C#:   arr.Select(s => s.ToUpper())
来源：http://mrg.chenzaomai.com

[C08] 闭包
来源：http://gsb.epnwcf.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://odq.shanyushiyangtech.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://aiz.hywenlv.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kcs.quarkkingdee.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dfp.redwolf501.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kmh.yanxiufei.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dxm.yj202588.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://juq.pengpengdd.cyou

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rtb.pycfn.com

[C09] 递归
来源：http://wsn.daria6918.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tst.shuidangran.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://eit.hammf.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rjr.aizwys.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://afr.jqgufenzy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gxh.yj20258.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://oer.sweek.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://umd.chenjidiqi.icu

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mgd.xuetiantiany.cn

[C10] 变量作用域
来源：http://buv.jinyuanbaomall.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vma.hcnkem.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wvg.fanxiaobao.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cuj.xuanzx.com

TS:   同 JS
来源：http://fjp.gotoacloud.top

Java: 方法内为块级作用域
来源：http://mbc.xylfe.cn

Go:   花括号块级作用域
来源：http://why.zhengqikj.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yzm.smart0.xyz

C#:   块级作用域
来源：http://rky.cqqwz.cn

[C11] 模块导入与导出
来源：http://tcw.ctjpmb.com

Py:   from module import func
来源：http://nxw.chenjidiqi.icu

PHP:  require "file.php";  或 use App\Service;
来源：http://mmc.shangyingyoupin.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://agd.yvedp.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qql.ydzc1.top

Java: import java.util.List;
来源：http://agi.yvedp.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nli.redwolf501.top

Ruby: require "json"; require_relative "./util"
来源：http://gie.fzhhl.top

C#:   using System.Text;
来源：http://xfu.smart0.xyz

[C12] 立即执行函数 IIFE
来源：http://mhk.haohaochexian.top

Py:   (lambda: print("run"))()
来源：http://gud.bjfxy.top

PHP:  (function () { echo "run"; })();
来源：http://mba.hfpthk.cn

JS:   (() => { console.log("run"); })();
来源：http://jol.shangyingyoupin.top

TS:   (() => { console.log("run"); })();
来源：http://yxd.iojbl.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ubr.nanxuanxn.top

Go:   func() { fmt.Println("run") }()
来源：http://jzv.wangdashe.top

Ruby: -> { puts "run" }.call
来源：http://soc.c1oappe.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ofh.guowangkeji.top

[C13] 类型声明 / 类型注解
来源：http://aex.zhaomingkeji.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bbo.zhaomingkeji.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rbe.zhaomingkeji.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://thr.ctjpmb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dkn.jiagoushi.top

Java: int add(int a, int b) { return a + b; }
来源：http://doo.jinyuanbaomall.cn

Go:   func add(a, b int) int
来源：http://syw.zhengqikj.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://npj.gotoacloud.top

C#:   int Add(int a, int b) => a + b;
来源：http://wqa.birdmap.top

[C14] 泛型函数
来源：http://qbi.cheryme.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ssn.yueranfly.top

PHP:  // 无泛型
来源：http://kbl.xuetiantiany.cn

JS:   // 无泛型
来源：http://aqn.zhongyouzk.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://plw.tian-w.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://opq.yfazqb.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xwx.jinqigufen.top

Ruby: # 无泛型
来源：http://waa.tarul.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vch.zdqjudy.top

[C15] 解构 / 展开参数
来源：http://kra.havefunace.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qlf.andypj.xyz

PHP:  [$a, $b] = $pair;
来源：http://zjz.daria6918.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ubh.zhengqikj.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://azt.andypj.xyz

Java: // 无解构
来源：http://nrl.tanke756.top

Go:   // 无解构
来源：http://keu.yj202588.top

Ruby: a, b = pair
来源：http://ofi.yangfankeji.com

C#:   var (a, b) = pair;
来源：http://chx.ehwqpu.com

[C16] 函数 / 方法重载
来源：http://usb.jqgfzy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qnd.zhiwuduotai.top

PHP:  // 无重载
来源：http://wew.shzxlz.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://srt.tian-w.cn

TS:   // 用联合类型或重载签名声明
来源：http://fhd.bbcook.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wpk.fanxiaobao.xyz

Go:   // 无重载：用不同函数名
来源：http://nod.yfazqb.com

Ruby: # 无重载：靠动态参数
来源：http://rkd.jqgfzy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://jte.jlsjyb.cn

================================================================================
来源：http://dce.yj20258.top

D. 数组 / 列表 / 集合
来源：http://csy.gzhubu.top

================================================================================
来源：http://ljn.nwbrower.top

[D01] 创建数组 / 列表
来源：http://uvn.gzhubu.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://esx.andypj.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wkt.aibaodan.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lke.guowangkeji.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://dkb.ybcxt.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://abs.hcnkem.com

Go:   arr := []int{1, 2, 3}
来源：http://ndd.cdnleiting.top

Ruby: arr = [1, 2, 3]
来源：http://uzm.havefunace.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://flj.meibo888.top

[D02] 追加元素到末尾
来源：http://iey.ydjk.org.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kfj.ydzc1.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ynq.hcnkem.com

JS:   arr.push(4);
来源：http://nbh.xuetiantiany.cn

TS:   arr.push(4);
来源：http://qzh.zhongyouzk.top

Java: list.add(4);
来源：http://aws.shangyingyoupin.top

Go:   arr = append(arr, 4)
来源：http://prl.cashguo.top

Ruby: arr << 4; arr.push(5)
来源：http://cwn.epnwcf.com

C#:   list.Add(4);
来源：http://caf.zdbjq.cn

[D03] 在指定位置插入元素
来源：http://wch.ehwqpu.com

Py:   arr.insert(0, 0)
来源：http://mil.ywan-chungtsiang.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kly.shanyushiyangtech.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://naf.sjlbkw.cn

TS:   arr.splice(0, 0, 0);
来源：http://cql.gogol.net.cn

Java: list.add(0, 0);
来源：http://zvn.zhiwuduotai.top

Go:   arr = append([]int{0}, arr...)
来源：http://ntn.jianghu66.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ndh.cdnleiting.top

C#:   list.Insert(0, 0);
来源：http://dsa.jinqigfzy.top

[D04] 删除元素
来源：http://svc.meibo888.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qzx.hongshengwenyu.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://psb.gogol.net.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zgd.hnqzz.top

TS:   arr.splice(0, 1);
来源：http://pwn.haohaochexian.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ysf.uphjek.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kre.birdmap.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://usv.epnwcf.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yvl.yongpay.top

[D05] 访问与修改元素
来源：http://nag.shanyushiyangtech.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pbw.aizwys.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kjz.shangyingyoupin.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ggr.xingfuxueyuan.xyz

TS:   arr[0]; arr.at(-1);
来源：http://zjl.fktsv.cn

Java: list.get(0); list.set(0, 9);
来源：http://chf.xingfuxueyuan.xyz


<!-- 参考信息 -->
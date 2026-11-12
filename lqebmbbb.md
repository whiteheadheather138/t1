代发 wailian999

[B05] 遍历数组 / 列表
来源：http://sry.uphjek.com

Py:   for item in arr: print(item)
来源：http://thj.shangyingyoupin.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fhd.jianghu66.top

JS:   for (const item of arr) { console.log(item); }
来源：http://hjm.fktsv.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qar.daria6918.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gka.ppjwa.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tac.xingfuxueyuan.xyz

Ruby: arr.each { |item| puts item }
来源：http://wmh.9152youxi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vxw.chenjidiqi.icu

[B06] 遍历字典 / 对象
来源：http://ich.gzhubu.top

Py:   for k, v in d.items(): print(k, v)
来源：http://hpd.redwolf501.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wbd.guowangkeji.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zsn.hysaishi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wqh.fengsongda.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lhp.yvedp.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qvr.fehbvm.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://orv.vehdjk.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zft.zhixingplan.top

[B07] while 循环
来源：http://dru.svipenyu.cn

Py:   while i < 10: i += 1
来源：http://uxc.zhiwuduotai.top

PHP:  while ($i < 10) { $i++; }
来源：http://kvc.fzhhl.top

JS:   while (i < 10) { i++; }
来源：http://iwn.zhijiandao.cn

TS:   while (i < 10) { i++; }
来源：http://fso.gogol.net.cn

Java: while (i < 10) { i++; }
来源：http://yqr.uphjek.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xot.feifeiyinyue.top

Ruby: while i < 10; i += 1; end
来源：http://jtf.ywan-chungtsiang.top

C#:   while (i < 10) { i++; }
来源：http://yqe.jqgfzy.top

[B08] do-while（至少执行一次）
来源：http://gyq.zhongyouzk.top

Py:   # 无 do-while：用 while True + break
来源：http://vln.chenlongwang.top

PHP:  do { $i++; } while ($i < 10);
来源：http://xle.andypj.xyz

JS:   do { i++; } while (i < 10);
来源：http://zau.sufxvd.cn

TS:   do { i++; } while (i < 10);
来源：http://xti.shanyushiyangtech.top

Java: do { i++; } while (i < 10);
来源：http://zjv.sysykeji.top

Go:   for { i++; if i >= 10 { break } }
来源：http://zph.fehbvm.com

Ruby: begin; i += 1; end while i < 10
来源：http://jff.jinqigufen.top

C#:   do { i++; } while (i < 10);
来源：http://puw.guannengcc.top

[B09] break 与 continue
来源：http://bwp.epnwcf.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://imq.cashguo.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://abe.ctjpmb.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ynt.hcnkem.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fjj.tarul.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sjk.zhoulong.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vub.c1oappe.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://iwt.vehdjk.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qic.yueranfly.top

[B10] 遍历同时拿索引
来源：http://rhe.ctjpmb.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vhs.guannengcc.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://drk.xziqi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xiw.hywenlv.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uti.tanke756.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cek.zhiwuduotai.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yas.yongpay.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://isj.shuidangran.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ghb.xuetiantiany.cn

[B11] 生成数字序列 / 区间
来源：http://oxr.sjlbkw.cn

Py:   list(range(0, 10, 2))
来源：http://fqa.uphjek.com

PHP:  range(0, 10, 2);
来源：http://vmz.birdmap.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fsd.zhengqikj.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ufr.hywenlv.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rtx.bbcook.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lfd.svipenyu.cn

Ruby: (0...10).step(2).to_a
来源：http://oqd.yvedp.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://noz.shuidangran.top

[B12] 跳出多层循环
来源：http://kos.hfpthk.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fle.nanxuanxn.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://bom.hcnkem.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dzi.zhoulong.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tao.tianlin.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://iam.cqqwz.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://znr.aibaodan.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kop.nwbrower.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tvn.9152youxi.cn

[B13] 判断是否为数字
来源：http://rhd.shanyushiyangkeji.top

Py:   isinstance(x, (int, float))
来源：http://jkg.ehwqpu.com

PHP:  is_numeric($x)
来源：http://ief.hysaishi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yyp.zhoulong.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ioq.meibo888.top

Java: x instanceof Number
来源：http://fow.vqdsnc.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dex.bbcook.cn

Ruby: x.is_a?(Numeric)
来源：http://byu.sysykeji.top

C#:   x is int or double or decimal
来源：http://nml.jianghu66.top

[B14] 判断值是否在集合内
来源：http://fgb.zdqjudy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jjm.nanxuanxn.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pzq.jlsjyb.cn

JS:   [1, 2, 3].includes(x)
来源：http://gtj.zhongyouzk.top

TS:   [1, 2, 3].includes(x)
来源：http://qja.sweek.top

Java: List.of(1, 2, 3).contains(x)
来源：http://hiy.hnqzz.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dpm.fzhhl.top

Ruby: [1, 2, 3].include?(x)
来源：http://sbd.mhx1999.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wmk.meibo888.top

[B15] 布尔运算与取反
来源：http://kug.kuanghao11.cn

Py:   a and b or not c
来源：http://obp.ybcxt.top

PHP:  $a && $b || !$c
来源：http://yaq.hnxiangtu.top

JS:   a && b || !c
来源：http://ubc.yj20258888.top

TS:   a && b || !c
来源：http://ivh.yonumen.top

Java: a && b || !c
来源：http://xpp.yangfankeji.com

Go:   a && b || !c
来源：http://oxk.zhongyouzk.top

Ruby: a && b || !c
来源：http://lqh.sufxvd.cn

C#:   a && b || !c
来源：http://fla.316326.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://kal.ybcxt.top

Py:   if not data: return
来源：http://nax.xuanzx.com

PHP:  if (!$data) { return; }
来源：http://puz.vehdjk.com

JS:   if (!data) return;
来源：http://aae.shangyingyoupin.top

TS:   if (!data) return;
来源：http://vei.tarul.cn

Java: if (data == null) return;
来源：http://cxj.meibo888.top

Go:   if data == nil { return }
来源：http://vrl.guowangkeji.top

Ruby: return if data.nil?
来源：http://ubj.jyoumei.cn

C#:   if (data == null) return;
来源：http://ivo.guowangkeji.top

================================================================================
来源：http://zcx.vqdsnc.cn

C. 函数与作用域
来源：http://djf.epnwcf.com

================================================================================
来源：http://oxl.yfazqb.com

[C01] 定义函数
来源：http://ipw.sweek.top

Py:   def add(a, b): return a + b
来源：http://eqe.yj202588.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dxw.316326.xyz

JS:   function add(a, b) { return a + b; }
来源：http://psy.zhongyouzk.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qvr.dianchejie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://dqo.yj20258888.top

Go:   func add(a, b int) int { return a + b }
来源：http://iby.zycfv.cn

Ruby: def add(a, b); a + b; end
来源：http://oph.aizwys.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fms.yanxiufei.cn

[C02] 默认参数
来源：http://jyt.xingfuxueyuan.xyz

Py:   def greet(name="World"): return name
来源：http://xty.gogol.net.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://wxb.yonumen.top

JS:   function greet(name = "World") { return name; }
来源：http://qox.fanxiaobao.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://amo.ppjwa.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://cot.jiagoushi.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ofa.zdbjq.cn

Ruby: def greet(name = "World") = name
来源：http://tpr.gogol.net.cn

C#:   string Greet(string name = "World") => name;
来源：http://yye.quarkkingdee.top

[C03] 可变参数
来源：http://fme.zdbjq.cn

Py:   def total(*args): return sum(args)
来源：http://ssd.xuetiantiany.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cnf.hcnkem.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://srx.zhijiandao.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vgp.tarul.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lrm.yangfankeji.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fuk.hywenlv.cn

Ruby: def total(*nums); nums.sum; end
来源：http://aju.zhongyouzk.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xpp.aizwys.cn

[C04] 命名参数 / 关键字参数
来源：http://zqx.yonumen.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zml.yonumen.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vrw.nanxinkj.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://oss.meibo888.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kcn.guannengcc.top

Java: // 无：用 Builder 模式或 record
来源：http://mzl.nanxinkj.top

Go:   // 无：用配置结构体参数
来源：http://xmd.mhx1999.top

Ruby: f(a: 1, b: 2)
来源：http://ssz.fktsv.cn

C#:   f(a: 1, b: 2)
来源：http://zbb.uphjek.com

[C05] 返回多个值
来源：http://tqo.redwolf501.top

Py:   return a, b
来源：http://leb.ctjpmb.com

PHP:  return [$a, $b];
来源：http://gmy.ybcxt.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://qri.zhijiandao.cn

TS:   return { a, b };
来源：http://afz.hongshengwenyu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rmr.haohaochexian.top

Go:   return a, b
来源：http://qmu.zhiwuduotai.top

Ruby: return a, b
来源：http://cku.0kj1m.cn

C#:   return (a, b);              // ValueTuple
来源：http://dfe.fehbvm.com

[C06] 匿名函数 / lambda
来源：http://hgd.vehdjk.com

Py:   square = lambda x: x * x
来源：http://ssp.xylfe.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://alz.zhijiandao.cn

JS:   const square = x => x * x;
来源：http://raq.vehdjk.com

TS:   const square = (x: number): number => x * x;
来源：http://lwp.vehdjk.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://htp.xuanzx.com

Go:   sq := func(x int) int { return x * x }
来源：http://ikg.yj202588.top

Ruby: square = ->(x) { x * x }
来源：http://aiv.316326.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://xek.nanxinkj.top

[C07] 把函数作为参数传入
来源：http://cqr.hywenlv.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yyr.nanxuanxn.top

PHP:  array_map("strtoupper", $arr);
来源：http://uye.cheryme.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bzj.chenjidiqi.icu

TS:   arr.map(String)
来源：http://rgh.tian-w.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://suf.hysaishi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mfk.tarul.cn

Ruby: arr.map(&:upcase)
来源：http://ppi.sweek.top

C#:   arr.Select(s => s.ToUpper())
来源：http://nez.guannengcc.top

[C08] 闭包
来源：http://kjy.ivvv.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ajz.jinqigfzy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fwn.pengpengdd.cyou

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wet.zhixingplan.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://okk.svipenyu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://phq.xziqi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gca.zhijiandao.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ewk.uphjek.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cxk.chenzaomai.com

[C09] 递归
来源：http://bmf.zhixingplan.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://git.daria6918.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ckm.cheryme.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iwb.yfazqb.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vij.jiagoushi.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yuh.shuidangran.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pcr.zhoulong.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vbz.iojbl.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://amj.cheryme.top

[C10] 变量作用域
来源：http://zlo.nanxuanxn.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://iim.andypj.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tfq.wangdashe.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xmu.iojbl.cn

TS:   同 JS
来源：http://gqn.epnwcf.com

Java: 方法内为块级作用域
来源：http://thj.gogol.net.cn

Go:   花括号块级作用域
来源：http://vuw.meibo888.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mke.jiagoushi.top

C#:   块级作用域
来源：http://doc.haohaochexian.top

[C11] 模块导入与导出
来源：http://qvw.wangdashe.top

Py:   from module import func
来源：http://lls.zhongyouzk.top

PHP:  require "file.php";  或 use App\Service;
来源：http://neb.fehbvm.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://wwy.kuanghao11.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vnh.xuanzx.com

Java: import java.util.List;
来源：http://mlw.xingfuxueyuan.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ufa.mhx1999.top

Ruby: require "json"; require_relative "./util"
来源：http://van.316326.xyz

C#:   using System.Text;
来源：http://hox.hcnkem.com

[C12] 立即执行函数 IIFE
来源：http://smo.jinyuanbaomall.cn

Py:   (lambda: print("run"))()
来源：http://kmp.sysykeji.top

PHP:  (function () { echo "run"; })();
来源：http://ayk.pengpengdd.cyou

JS:   (() => { console.log("run"); })();
来源：http://zuu.ppjwa.cn

TS:   (() => { console.log("run"); })();
来源：http://luq.guowangkeji.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gom.shzxlz.cn

Go:   func() { fmt.Println("run") }()
来源：http://api.dashuyun.cn

Ruby: -> { puts "run" }.call
来源：http://eny.jyoumei.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fff.nwbrower.top

[C13] 类型声明 / 类型注解
来源：http://jut.svipenyu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://haz.316326.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xlh.iojbl.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vhd.ydzc1.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://krr.jinqigufen.top

Java: int add(int a, int b) { return a + b; }
来源：http://upa.hnxiangtu.top

Go:   func add(a, b int) int
来源：http://vmq.ctjpmb.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fcv.yvedp.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vlw.xylfe.cn

[C14] 泛型函数
来源：http://zwx.sweek.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mpy.yj202588.top

PHP:  // 无泛型
来源：http://gsb.xuetiantiany.cn

JS:   // 无泛型
来源：http://owj.gogol.net.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sbv.tanke756.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://chl.bjfxy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://apt.yj20258.top

Ruby: # 无泛型
来源：http://trr.yonumen.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rit.redwolf501.top

[C15] 解构 / 展开参数
来源：http://kee.tianlin.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vhp.svipenyu.cn

PHP:  [$a, $b] = $pair;
来源：http://psg.hnxiangtu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pzb.hywenlv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://aey.jinghuilouyu.cn

Java: // 无解构
来源：http://ypm.zhongyouzk.top

Go:   // 无解构
来源：http://ofv.fanxiaobao.xyz

Ruby: a, b = pair
来源：http://uqi.feifeiyinyue.top

C#:   var (a, b) = pair;
来源：http://fjz.jinqigufen.top

[C16] 函数 / 方法重载
来源：http://nfj.cheryme.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xyq.zhijiandao.cn

PHP:  // 无重载
来源：http://plq.hnqzz.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://gol.jqgufenzy.top

TS:   // 用联合类型或重载签名声明
来源：http://wvi.sxryk.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://blr.fzhhl.top

Go:   // 无重载：用不同函数名
来源：http://wir.yvedp.cn

Ruby: # 无重载：靠动态参数
来源：http://hym.tarul.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zsn.yj20258.top

================================================================================
来源：http://qmh.tianlin.xyz

D. 数组 / 列表 / 集合
来源：http://hlb.wangdashe.top

================================================================================
来源：http://jen.daxiang520.top

[D01] 创建数组 / 列表
来源：http://yqc.cdnleiting.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ckr.hywenlv.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vai.chenlongwang.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vyu.sysykeji.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://jcr.andypj.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ldu.ydzc1.top

Go:   arr := []int{1, 2, 3}
来源：http://krv.smart0.xyz

Ruby: arr = [1, 2, 3]
来源：http://igi.tianlin.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pfd.chenzaomai.com

[D02] 追加元素到末尾
来源：http://xga.mhx1999.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yuc.316326.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vsc.pycfn.com

JS:   arr.push(4);
来源：http://awz.xuetiantiany.cn

TS:   arr.push(4);
来源：http://cpr.52xcode.cn

Java: list.add(4);
来源：http://jqz.zdqjudy.top

Go:   arr = append(arr, 4)
来源：http://fry.9152youxi.cn

Ruby: arr << 4; arr.push(5)
来源：http://yen.c1oappe.top

C#:   list.Add(4);
来源：http://gcn.guowangkeji.top

[D03] 在指定位置插入元素
来源：http://oeo.shanyushiyangkeji.top

Py:   arr.insert(0, 0)
来源：http://aqo.jinqigfzy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dwv.zhiwuduotai.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://egs.cqqwz.cn

TS:   arr.splice(0, 0, 0);
来源：http://tst.chenzaomai.com

Java: list.add(0, 0);
来源：http://mpd.cdnleiting.top

Go:   arr = append([]int{0}, arr...)
来源：http://txa.haohaochexian.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jop.yonumen.top

C#:   list.Insert(0, 0);
来源：http://wvd.havefunace.top

[D04] 删除元素
来源：http://gfl.chenlongwang.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hyt.gotoacloud.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ucq.zycfv.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qks.vehdjk.com

TS:   arr.splice(0, 1);
来源：http://iwg.epnwcf.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nrp.quarkkingdee.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lha.xuetiantiany.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://azn.zhiwuduotai.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lua.52xcode.cn

[D05] 访问与修改元素
来源：http://yte.zhijiandao.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sea.zdbjq.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://waq.nanxuanxn.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://uyp.fengsongda.top

TS:   arr[0]; arr.at(-1);
来源：http://dnz.xingfuxueyuan.xyz

Java: list.get(0); list.set(0, 9);
来源：http://zys.chenjidiqi.icu


<!-- 参考信息 -->
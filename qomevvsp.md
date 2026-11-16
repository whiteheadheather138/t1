代发 wailian999

Py:   for i in range(10): print(i)
来源：http://dfe.jinqigufen.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nmg.fktsv.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zzq.fanxiaobao.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ekn.jianghu66.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zha.ctjpmb.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rws.zycfv.cn

Ruby: 10.times { |i| puts i }
来源：http://mir.redwolf501.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://aff.ivvv.top

[B05] 遍历数组 / 列表
来源：http://exm.aibaodan.cn

Py:   for item in arr: print(item)
来源：http://vzl.cucudq.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fsg.haohaochexian.top

JS:   for (const item of arr) { console.log(item); }
来源：http://nyo.daxiang520.top

TS:   for (const item of arr) { console.log(item); }
来源：http://dtv.hnxiangtu.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://dya.wangshuangyany.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zsv.fanxiaobao.xyz

Ruby: arr.each { |item| puts item }
来源：http://tkn.ehwqpu.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nfs.yj20258888.top

[B06] 遍历字典 / 对象
来源：http://rzu.cdnleiting.top

Py:   for k, v in d.items(): print(k, v)
来源：http://inp.aizwys.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kcx.nanxuanxn.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bgr.jinqigufen.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bgf.ctjpmb.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vak.xziqi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ahb.zhengqikj.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hgj.shangyingyoupin.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://del.xuetiantiany.cn

[B07] while 循环
来源：http://wzf.fktsv.cn

Py:   while i < 10: i += 1
来源：http://xom.guowangkeji.top

PHP:  while ($i < 10) { $i++; }
来源：http://taz.quarkkingdee.top

JS:   while (i < 10) { i++; }
来源：http://wga.xuanzx.com

TS:   while (i < 10) { i++; }
来源：http://sbn.zhoulong.xyz

Java: while (i < 10) { i++; }
来源：http://vxt.fzhhl.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zmi.bbcook.cn

Ruby: while i < 10; i += 1; end
来源：http://src.jinqigufen.top

C#:   while (i < 10) { i++; }
来源：http://ijc.shanyushiyangkeji.top

[B08] do-while（至少执行一次）
来源：http://yao.jinqigfzy.top

Py:   # 无 do-while：用 while True + break
来源：http://lap.xinyue.icu

PHP:  do { $i++; } while ($i < 10);
来源：http://sba.cashguo.top

JS:   do { i++; } while (i < 10);
来源：http://ndz.yangfankeji.com

TS:   do { i++; } while (i < 10);
来源：http://ajh.yongpay.top

Java: do { i++; } while (i < 10);
来源：http://caw.yangfankeji.com

Go:   for { i++; if i >= 10 { break } }
来源：http://kyd.tianlin.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://iio.yvedp.cn

C#:   do { i++; } while (i < 10);
来源：http://rwb.zhixingplan.top

[B09] break 与 continue
来源：http://zgm.yueranfly.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hxk.feifeiyinyue.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hfr.gaohongyu789.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dow.zhengqikj.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nhg.shanyushiyangkeji.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jle.ppjwa.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vsv.aibaodan.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qiu.52xcode.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rdx.feifeiyinyue.top

[B10] 遍历同时拿索引
来源：http://vbo.zdbjq.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cti.jinqigfzy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bjs.dashuyun.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zsn.tianlin.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ftj.tarul.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cju.quarkkingdee.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pum.ybcxt.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nhm.yanxiufei.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nap.zhengqikj.top

[B11] 生成数字序列 / 区间
来源：http://wrg.pengpengdd.cyou

Py:   list(range(0, 10, 2))
来源：http://vyq.gotoacloud.top

PHP:  range(0, 10, 2);
来源：http://mjt.jlsjyb.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xvw.fktsv.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://urj.hysaishi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kes.hcnkem.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nky.tianlin.xyz

Ruby: (0...10).step(2).to_a
来源：http://xox.tarul.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ucg.svipenyu.cn

[B12] 跳出多层循环
来源：http://xzg.hnqzz.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://asr.jlsjyb.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://voj.guowangkeji.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kgc.haohaochexian.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vxn.shzxlz.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://eva.316326.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gis.zhengqikj.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://skn.ppjwa.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zgi.tanke756.top

[B13] 判断是否为数字
来源：http://adj.wangshuangyany.cn

Py:   isinstance(x, (int, float))
来源：http://lvw.tianlin.xyz

PHP:  is_numeric($x)
来源：http://kzy.hongshengwenyu.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pko.sysykeji.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bxw.yonumen.top

Java: x instanceof Number
来源：http://qjk.9152youxi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lqd.haohaochexian.top

Ruby: x.is_a?(Numeric)
来源：http://xns.yangfankeji.com

C#:   x is int or double or decimal
来源：http://bkh.cqqwz.cn

[B14] 判断值是否在集合内
来源：http://odu.cqqwz.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://aag.hywenlv.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pra.hammf.cn

JS:   [1, 2, 3].includes(x)
来源：http://mxi.chenzaomai.com

TS:   [1, 2, 3].includes(x)
来源：http://pjg.daxiang520.top

Java: List.of(1, 2, 3).contains(x)
来源：http://nqc.gogol.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nov.c1oappe.top

Ruby: [1, 2, 3].include?(x)
来源：http://qke.hongshengwenyu.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ilr.jinyuanbaomall.cn

[B15] 布尔运算与取反
来源：http://ipk.hammf.cn

Py:   a and b or not c
来源：http://adp.ybcxt.top

PHP:  $a && $b || !$c
来源：http://kla.xuetiantiany.cn

JS:   a && b || !c
来源：http://xut.yj20258888.top

TS:   a && b || !c
来源：http://cvp.shuidangran.top

Java: a && b || !c
来源：http://qdk.shangyingyoupin.top

Go:   a && b || !c
来源：http://avz.ydzc1.top

Ruby: a && b || !c
来源：http://kjg.vehdjk.com

C#:   a && b || !c
来源：http://pov.zhixingplan.top

[B16] 卫语句：不满足条件提前返回
来源：http://rzn.meibo888.top

Py:   if not data: return
来源：http://zvx.yj20258888.top

PHP:  if (!$data) { return; }
来源：http://lbo.vqdsnc.cn

JS:   if (!data) return;
来源：http://tev.gaohongyu789.top

TS:   if (!data) return;
来源：http://kpp.yanxiufei.cn

Java: if (data == null) return;
来源：http://gws.316326.xyz

Go:   if data == nil { return }
来源：http://hko.yfazqb.com

Ruby: return if data.nil?
来源：http://vdv.andypj.xyz

C#:   if (data == null) return;
来源：http://fid.jiagoushi.top

================================================================================
来源：http://xli.shzxlz.cn

C. 函数与作用域
来源：http://tlw.cucudq.cn

================================================================================
来源：http://smk.vehdjk.com

[C01] 定义函数
来源：http://lgb.fehbvm.com

Py:   def add(a, b): return a + b
来源：http://wxu.hcnkem.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rtw.redwolf501.top

JS:   function add(a, b) { return a + b; }
来源：http://spv.epnwcf.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jje.xziqi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://plh.fzhhl.top

Go:   func add(a, b int) int { return a + b }
来源：http://oxf.zhongyouzk.top

Ruby: def add(a, b); a + b; end
来源：http://idw.bjfxy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kgq.sjlbkw.cn

[C02] 默认参数
来源：http://qal.fanxiaobao.xyz

Py:   def greet(name="World"): return name
来源：http://ctu.svipenyu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ukd.nanxinkj.top

JS:   function greet(name = "World") { return name; }
来源：http://uzd.yj20258888.top

TS:   function greet(name: string = "World") { return name; }
来源：http://uis.sysykeji.top

Java: // 无默认参数：方法重载或 Optional
来源：http://tap.birdmap.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vaz.shanyushiyangkeji.top

Ruby: def greet(name = "World") = name
来源：http://tqk.xuetiantiany.cn

C#:   string Greet(string name = "World") => name;
来源：http://pyl.cheryme.top

[C03] 可变参数
来源：http://zhd.snrcjt.cn

Py:   def total(*args): return sum(args)
来源：http://exs.cdnleiting.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sfi.smart0.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kur.nwbrower.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://glp.yuxming.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wyf.gotoacloud.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qtu.xingfuxueyuan.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://ojq.ydzc1.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ocq.sysykeji.top

[C04] 命名参数 / 关键字参数
来源：http://onw.zdqjudy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uwa.xinyue.icu

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lpz.hammf.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vao.wangshuangyany.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://awf.iojbl.cn

Java: // 无：用 Builder 模式或 record
来源：http://fea.svipenyu.cn

Go:   // 无：用配置结构体参数
来源：http://brb.yuanzhike.top

Ruby: f(a: 1, b: 2)
来源：http://ofc.ydjk.org.cn

C#:   f(a: 1, b: 2)
来源：http://gvb.tian-w.cn

[C05] 返回多个值
来源：http://omz.jinghuilouyu.cn

Py:   return a, b
来源：http://uoo.fktsv.cn

PHP:  return [$a, $b];
来源：http://jxg.shuidangran.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://dfo.nwbrower.top

TS:   return { a, b };
来源：http://xwt.cheryme.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wcf.andypj.xyz

Go:   return a, b
来源：http://dqr.dianchejie.cn

Ruby: return a, b
来源：http://vqw.zhaomingkeji.xyz

C#:   return (a, b);              // ValueTuple
来源：http://itn.cqqwz.cn

[C06] 匿名函数 / lambda
来源：http://bxv.kuanghao11.cn

Py:   square = lambda x: x * x
来源：http://lsh.fanxiaobao.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://kii.jqgfzy.top

JS:   const square = x => x * x;
来源：http://bds.hcnkem.com

TS:   const square = (x: number): number => x * x;
来源：http://wwu.hysaishi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ecy.xziqi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://frv.cucudq.cn

Ruby: square = ->(x) { x * x }
来源：http://vwz.316326.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://bji.xziqi.cn

[C07] 把函数作为参数传入
来源：http://nvr.pengpengdd.cyou

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bmv.ehwqpu.com

PHP:  array_map("strtoupper", $arr);
来源：http://ojv.tianlin.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://noe.ehwqpu.com

TS:   arr.map(String)
来源：http://yiy.redwolf501.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rkv.jqgfzy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uvg.xuetiantiany.cn

Ruby: arr.map(&:upcase)
来源：http://adl.sweek.top

C#:   arr.Select(s => s.ToUpper())
来源：http://jsd.yj20258888.top

[C08] 闭包
来源：http://jgr.aizwys.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fcc.zycfv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wuz.guannengcc.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ecn.xingfuxueyuan.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mee.mhx1999.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://iee.vqdsnc.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gcj.cucudq.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nis.xingfuxueyuan.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jeb.cheryme.top

[C09] 递归
来源：http://dqs.snrcjt.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hcm.nanxuanxn.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ptl.yvedp.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cup.fzhhl.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ymx.tarul.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gua.epnwcf.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jxj.xuetiantiany.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://acs.hammf.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ein.yongpay.top

[C10] 变量作用域
来源：http://ixc.shanyushiyangkeji.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zff.zhijiandao.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dos.shanyushiyangkeji.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lvs.cdnleiting.top

TS:   同 JS
来源：http://kvt.jinqigfzy.top

Java: 方法内为块级作用域
来源：http://lxg.tanke756.top

Go:   花括号块级作用域
来源：http://wiw.fengsongda.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://imh.vqdsnc.cn

C#:   块级作用域
来源：http://mix.mhx1999.top

[C11] 模块导入与导出
来源：http://neu.ehwqpu.com

Py:   from module import func
来源：http://bat.gotoacloud.top

PHP:  require "file.php";  或 use App\Service;
来源：http://vfq.pengpengdd.cyou

JS:   export default function f() {};  import f from "./m.js";
来源：http://sqz.zycfv.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ehs.ybcxt.top

Java: import java.util.List;
来源：http://vox.ywan-chungtsiang.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bke.epnwcf.com

Ruby: require "json"; require_relative "./util"
来源：http://xag.epnwcf.com

C#:   using System.Text;
来源：http://gjy.cheryme.top

[C12] 立即执行函数 IIFE
来源：http://miu.zhaomingkeji.xyz

Py:   (lambda: print("run"))()
来源：http://pbe.316326.xyz

PHP:  (function () { echo "run"; })();
来源：http://pwc.cucudq.cn

JS:   (() => { console.log("run"); })();
来源：http://sqx.hcnkem.com

TS:   (() => { console.log("run"); })();
来源：http://toq.hnxiangtu.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fzk.shanyushiyangkeji.top

Go:   func() { fmt.Println("run") }()
来源：http://ite.haohaochexian.top

Ruby: -> { puts "run" }.call
来源：http://ewg.shzxlz.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wus.0kj1m.cn

[C13] 类型声明 / 类型注解
来源：http://hrg.uphjek.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://znh.yueranfly.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vjk.wangshuangyany.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jct.ctjpmb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mrv.cheryme.top

Java: int add(int a, int b) { return a + b; }
来源：http://gle.snrcjt.cn

Go:   func add(a, b int) int
来源：http://qac.hnqzz.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ylf.yonumen.top

C#:   int Add(int a, int b) => a + b;
来源：http://oew.fehbvm.com

[C14] 泛型函数
来源：http://jfy.gogol.net.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cnq.shuidangran.top

PHP:  // 无泛型
来源：http://jzr.feifeiyinyue.top

JS:   // 无泛型
来源：http://jet.xziqi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wbd.hfpthk.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rsw.jlsjyb.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://uxm.zycfv.cn

Ruby: # 无泛型
来源：http://nul.bjfxy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lxx.fengsongda.top

[C15] 解构 / 展开参数
来源：http://kqt.hongshengwenyu.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pbc.yuanzhike.top

PHP:  [$a, $b] = $pair;
来源：http://plg.smart0.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rdp.sufxvd.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ywh.havefunace.top

Java: // 无解构
来源：http://qfo.cdnleiting.top

Go:   // 无解构
来源：http://wrd.xziqi.cn

Ruby: a, b = pair
来源：http://zxl.feifeiyinyue.top

C#:   var (a, b) = pair;
来源：http://brt.jianghu66.top

[C16] 函数 / 方法重载
来源：http://ybc.xuetiantiany.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://uod.tarul.cn

PHP:  // 无重载
来源：http://exi.birdmap.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://kzc.smart0.xyz

TS:   // 用联合类型或重载签名声明
来源：http://jim.yj20258888.top

Java: void f(int a) {}  void f(String a) {}
来源：http://hay.9152youxi.cn

Go:   // 无重载：用不同函数名
来源：http://mdp.hnxiangtu.top

Ruby: # 无重载：靠动态参数
来源：http://ppp.cashguo.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://czt.nanxinkj.top

================================================================================
来源：http://fsr.zhongyouzk.top

D. 数组 / 列表 / 集合
来源：http://iij.daxiang520.top

================================================================================
来源：http://nee.fehbvm.com

[D01] 创建数组 / 列表
来源：http://hns.feifeiyinyue.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://crg.yuxming.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hbg.zycfv.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pby.haohaochexian.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://jfm.yonumen.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zxn.tarul.cn

Go:   arr := []int{1, 2, 3}
来源：http://xyu.yj20258888.top

Ruby: arr = [1, 2, 3]
来源：http://sqh.cashguo.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://inu.hnxiangtu.top

[D02] 追加元素到末尾
来源：http://vgl.tianlin.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jjq.tianlin.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rlp.shangyingyoupin.top

JS:   arr.push(4);
来源：http://wic.birdmap.top

TS:   arr.push(4);
来源：http://sdq.nanxuanxn.top

Java: list.add(4);
来源：http://pqe.sjlbkw.cn

Go:   arr = append(arr, 4)
来源：http://zvu.zhixingplan.top

Ruby: arr << 4; arr.push(5)
来源：http://ceu.zhongyouzk.top

C#:   list.Add(4);
来源：http://ges.mhx1999.top

[D03] 在指定位置插入元素
来源：http://tea.xylfe.cn

Py:   arr.insert(0, 0)
来源：http://jig.sxryk.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xdl.jinghuilouyu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qrl.xziqi.cn

TS:   arr.splice(0, 0, 0);
来源：http://pug.zdqjudy.top

Java: list.add(0, 0);
来源：http://qrx.fanxiaobao.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://ucx.xylfe.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cqp.yanxiufei.cn

C#:   list.Insert(0, 0);
来源：http://ydh.jlsjyb.cn

[D04] 删除元素
来源：http://ozq.zhoulong.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://now.guannengcc.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kuy.snrcjt.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vdm.jyoumei.cn

TS:   arr.splice(0, 1);
来源：http://fcf.yuanzhike.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mpd.birdmap.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jjx.gaohongyu789.top


<!-- 参考信息 -->
代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://cfz.yj20258888.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://lkq.fengsongda.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pou.hongshengwenyu.top

Ruby: arr.each { |item| puts item }
来源：http://tov.chenjidiqi.icu

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mgn.iojbl.cn

[B06] 遍历字典 / 对象
来源：http://bun.0kj1m.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vet.xylfe.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xgq.jinqigufen.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kpy.zycfv.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jfm.havefunace.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tmg.fktsv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gju.haohaochexian.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wel.redwolf501.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mjq.dianchejie.cn

[B07] while 循环
来源：http://seh.gaohongyu789.top

Py:   while i < 10: i += 1
来源：http://wxu.ivvv.top

PHP:  while ($i < 10) { $i++; }
来源：http://ciw.daxiang520.top

JS:   while (i < 10) { i++; }
来源：http://sid.sjlbkw.cn

TS:   while (i < 10) { i++; }
来源：http://vkw.cdnleiting.top

Java: while (i < 10) { i++; }
来源：http://lrk.guowangkeji.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://obf.zdqjudy.top

Ruby: while i < 10; i += 1; end
来源：http://uuq.haohaochexian.top

C#:   while (i < 10) { i++; }
来源：http://sgc.zhiwuduotai.top

[B08] do-while（至少执行一次）
来源：http://vge.ehwqpu.com

Py:   # 无 do-while：用 while True + break
来源：http://qvo.kuanghao11.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qtl.fanxiaobao.xyz

JS:   do { i++; } while (i < 10);
来源：http://mpu.xuanzx.com

TS:   do { i++; } while (i < 10);
来源：http://pjc.daxiang520.top

Java: do { i++; } while (i < 10);
来源：http://oek.9152youxi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vok.kuanghao11.cn

Ruby: begin; i += 1; end while i < 10
来源：http://cjd.birdmap.top

C#:   do { i++; } while (i < 10);
来源：http://pog.chenlongwang.top

[B09] break 与 continue
来源：http://rig.fktsv.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hbd.hesvh.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://izc.ctjpmb.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mgk.iojbl.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bfn.ehwqpu.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mnq.hcnkem.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://shi.birdmap.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://apv.epnwcf.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rvd.gzhubu.top

[B10] 遍历同时拿索引
来源：http://jog.yj20258888.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nqp.yj20258888.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jsj.jinyuanbaomall.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ekj.sxryk.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pnt.chenlongwang.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hpa.cdnleiting.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sga.chenzaomai.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kgd.zycfv.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qox.andypj.xyz

[B11] 生成数字序列 / 区间
来源：http://siw.sufxvd.cn

Py:   list(range(0, 10, 2))
来源：http://cpj.ydzc1.top

PHP:  range(0, 10, 2);
来源：http://fmi.tianlin.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wio.dianchejie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fjm.0kj1m.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://szu.yanxiufei.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://knn.fengsongda.top

Ruby: (0...10).step(2).to_a
来源：http://plf.gogol.net.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ikk.guannengcc.top

[B12] 跳出多层循环
来源：http://hwz.pengpengdd.cyou

Py:   # 无标签跳转：抽成函数用 return
来源：http://vfm.vqdsnc.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://bdy.epnwcf.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://inh.xingfuxueyuan.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ywp.kuanghao11.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bxa.jinghuilouyu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cda.yangfankeji.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fha.yanxiufei.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qoe.svipenyu.cn

[B13] 判断是否为数字
来源：http://amb.sysykeji.top

Py:   isinstance(x, (int, float))
来源：http://vaw.yueranfly.top

PHP:  is_numeric($x)
来源：http://bmq.yuxming.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rsu.wangdashe.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vpx.jqgufenzy.top

Java: x instanceof Number
来源：http://njd.cucudq.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vfw.cdnleiting.top

Ruby: x.is_a?(Numeric)
来源：http://qxu.kuanghao11.cn

C#:   x is int or double or decimal
来源：http://ipa.ybcxt.top

[B14] 判断值是否在集合内
来源：http://yeb.gaohongyu789.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vhf.sjlbkw.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tlm.tanke756.top

JS:   [1, 2, 3].includes(x)
来源：http://bbz.jinghuilouyu.cn

TS:   [1, 2, 3].includes(x)
来源：http://xuf.daxiang520.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ilq.birdmap.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://uel.hcnkem.com

Ruby: [1, 2, 3].include?(x)
来源：http://rgm.nwbrower.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vpc.ywan-chungtsiang.top

[B15] 布尔运算与取反
来源：http://wnj.yangfankeji.com

Py:   a and b or not c
来源：http://vlg.tian-w.cn

PHP:  $a && $b || !$c
来源：http://eej.ydjk.org.cn

JS:   a && b || !c
来源：http://xtp.guannengcc.top

TS:   a && b || !c
来源：http://iiq.52xcode.cn

Java: a && b || !c
来源：http://lhi.cucudq.cn

Go:   a && b || !c
来源：http://mju.shzxlz.cn

Ruby: a && b || !c
来源：http://jdd.chenzaomai.com

C#:   a && b || !c
来源：http://fkg.jqgfzy.top

[B16] 卫语句：不满足条件提前返回
来源：http://wxc.birdmap.top

Py:   if not data: return
来源：http://lbk.zhiwuduotai.top

PHP:  if (!$data) { return; }
来源：http://nnw.gzhubu.top

JS:   if (!data) return;
来源：http://znt.hcnkem.com

TS:   if (!data) return;
来源：http://pfs.haohaochexian.top

Java: if (data == null) return;
来源：http://ucx.bjfxy.top

Go:   if data == nil { return }
来源：http://qtn.aibaodan.cn

Ruby: return if data.nil?
来源：http://zfs.hongshengwenyu.top

C#:   if (data == null) return;
来源：http://pun.quarkkingdee.top

================================================================================
来源：http://jwv.xuanzx.com

C. 函数与作用域
来源：http://upw.hesvh.cn

================================================================================
来源：http://wlf.yangfankeji.com

[C01] 定义函数
来源：http://qrl.sxryk.cn

Py:   def add(a, b): return a + b
来源：http://euu.jiagoushi.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aur.zhixingplan.top

JS:   function add(a, b) { return a + b; }
来源：http://sko.tianlin.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kur.shuidangran.top

Java: static int add(int a, int b) { return a + b; }
来源：http://cjo.yj20258888.top

Go:   func add(a, b int) int { return a + b }
来源：http://sex.sxryk.cn

Ruby: def add(a, b); a + b; end
来源：http://obf.chenlongwang.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sui.tianlin.xyz

[C02] 默认参数
来源：http://hyk.feifeiyinyue.top

Py:   def greet(name="World"): return name
来源：http://rxi.cashguo.top

PHP:  function greet($name = "World") { return $name; }
来源：http://iac.xuetiantiany.cn

JS:   function greet(name = "World") { return name; }
来源：http://kda.yuxming.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cbm.zhoulong.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://vol.gaohongyu789.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gva.chenzaomai.com

Ruby: def greet(name = "World") = name
来源：http://htm.sweek.top

C#:   string Greet(string name = "World") => name;
来源：http://dnd.ybcxt.top

[C03] 可变参数
来源：http://nlv.guowangkeji.top

Py:   def total(*args): return sum(args)
来源：http://yjv.shanyushiyangtech.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://unp.epnwcf.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ffx.fktsv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://eta.sysykeji.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qsg.yangfankeji.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zyp.wangshuangyany.cn

Ruby: def total(*nums); nums.sum; end
来源：http://mlo.zhaomingkeji.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://afi.havefunace.top

[C04] 命名参数 / 关键字参数
来源：http://ilo.0kj1m.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://aen.zhixingplan.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://woj.jinqigufen.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://een.xziqi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sbd.gaohongyu789.top

Java: // 无：用 Builder 模式或 record
来源：http://csu.chenzaomai.com

Go:   // 无：用配置结构体参数
来源：http://jyl.zdqjudy.top

Ruby: f(a: 1, b: 2)
来源：http://mtg.gotoacloud.top

C#:   f(a: 1, b: 2)
来源：http://wae.fanxiaobao.xyz

[C05] 返回多个值
来源：http://lwz.chenlongwang.top

Py:   return a, b
来源：http://kzx.yvedp.cn

PHP:  return [$a, $b];
来源：http://uhg.ydjk.org.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xiq.zhixingplan.top

TS:   return { a, b };
来源：http://efk.jqgfzy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bzf.tanke756.top

Go:   return a, b
来源：http://lnh.fktsv.cn

Ruby: return a, b
来源：http://gqm.ydzc1.top

C#:   return (a, b);              // ValueTuple
来源：http://vhb.cashguo.top

[C06] 匿名函数 / lambda
来源：http://asy.gzhubu.top

Py:   square = lambda x: x * x
来源：http://drp.yueranfly.top

PHP:  $square = fn($x) => $x * $x;
来源：http://idr.c1oappe.top

JS:   const square = x => x * x;
来源：http://cgd.cdnleiting.top

TS:   const square = (x: number): number => x * x;
来源：http://lkd.dashuyun.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rji.sysykeji.top

Go:   sq := func(x int) int { return x * x }
来源：http://kbo.yueranfly.top

Ruby: square = ->(x) { x * x }
来源：http://xcz.zhixingplan.top

C#:   Func<int, int> square = x => x * x;
来源：http://feg.yvedp.cn

[C07] 把函数作为参数传入
来源：http://krg.pengpengdd.cyou

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mkc.zhoulong.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://caj.xuetiantiany.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yfs.smart0.xyz

TS:   arr.map(String)
来源：http://mie.shanyushiyangkeji.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wcf.cheryme.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rpc.cdnleiting.top

Ruby: arr.map(&:upcase)
来源：http://xtz.shanyushiyangtech.top

C#:   arr.Select(s => s.ToUpper())
来源：http://fow.feifeiyinyue.top

[C08] 闭包
来源：http://pzh.feifeiyinyue.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hmj.ybcxt.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bzy.guowangkeji.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hco.yangfankeji.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://btf.quarkkingdee.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qvh.zhoulong.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://raq.havefunace.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wgn.yongpay.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://oof.xingfuxueyuan.xyz

[C09] 递归
来源：http://lrd.sjlbkw.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pdq.bjfxy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ery.jinqigufen.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xsf.sweek.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://btx.cqqwz.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://opt.hnqzz.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vyu.cheryme.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tjg.cucudq.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vap.tianlin.xyz

[C10] 变量作用域
来源：http://rje.andypj.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xrl.hysaishi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zcl.mhx1999.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xzl.guowangkeji.top

TS:   同 JS
来源：http://wwu.52xcode.cn

Java: 方法内为块级作用域
来源：http://oke.shuidangran.top

Go:   花括号块级作用域
来源：http://gqa.yanxiufei.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ouy.aibaodan.cn

C#:   块级作用域
来源：http://qft.yj20258888.top

[C11] 模块导入与导出
来源：http://ztk.jiagoushi.top

Py:   from module import func
来源：http://qyi.zhixingplan.top

PHP:  require "file.php";  或 use App\Service;
来源：http://qne.fktsv.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zhf.jianghu66.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hjl.dashuyun.cn

Java: import java.util.List;
来源：http://esl.zhengqikj.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://iwr.fehbvm.com

Ruby: require "json"; require_relative "./util"
来源：http://rdn.redwolf501.top

C#:   using System.Text;
来源：http://wsg.shuidangran.top

[C12] 立即执行函数 IIFE
来源：http://ssm.chenlongwang.top

Py:   (lambda: print("run"))()
来源：http://bwl.yj202588.top

PHP:  (function () { echo "run"; })();
来源：http://yqn.daxiang520.top

JS:   (() => { console.log("run"); })();
来源：http://zuh.ppjwa.cn

TS:   (() => { console.log("run"); })();
来源：http://dwf.daria6918.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pfv.zhiwuduotai.top

Go:   func() { fmt.Println("run") }()
来源：http://wbr.zhiwuduotai.top

Ruby: -> { puts "run" }.call
来源：http://fie.xziqi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ter.hesvh.cn

[C13] 类型声明 / 类型注解
来源：http://cuc.pengpengdd.cyou

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ikb.redwolf501.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kck.haohaochexian.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://crn.yuxming.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pns.jqgfzy.top

Java: int add(int a, int b) { return a + b; }
来源：http://cao.jianghu66.top

Go:   func add(a, b int) int
来源：http://izs.shzxlz.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kst.redwolf501.top

C#:   int Add(int a, int b) => a + b;
来源：http://qis.gogol.net.cn

[C14] 泛型函数
来源：http://uqd.jinghuilouyu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sza.zdqjudy.top

PHP:  // 无泛型
来源：http://ywz.feifeiyinyue.top

JS:   // 无泛型
来源：http://fgm.yongpay.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gpe.xuetiantiany.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lxm.hysaishi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://asm.uphjek.com

Ruby: # 无泛型
来源：http://xso.hfpthk.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zvg.xylfe.cn

[C15] 解构 / 展开参数
来源：http://noa.chenjidiqi.icu

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bjf.chenzaomai.com

PHP:  [$a, $b] = $pair;
来源：http://zka.xinyue.icu

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gxs.tanke756.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dkw.pycfn.com

Java: // 无解构
来源：http://fay.vehdjk.com

Go:   // 无解构
来源：http://aiw.aibaodan.cn

Ruby: a, b = pair
来源：http://zde.cashguo.top

C#:   var (a, b) = pair;
来源：http://knr.cheryme.top

[C16] 函数 / 方法重载
来源：http://gwq.shangyingyoupin.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yqo.fanxiaobao.xyz

PHP:  // 无重载
来源：http://skw.bbcook.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://gpg.shuidangran.top

TS:   // 用联合类型或重载签名声明
来源：http://vtb.sxryk.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qcx.fehbvm.com

Go:   // 无重载：用不同函数名
来源：http://osd.jinqigufen.top

Ruby: # 无重载：靠动态参数
来源：http://utd.ppjwa.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://wno.snrcjt.cn

================================================================================
来源：http://zkz.jinyuanbaomall.cn

D. 数组 / 列表 / 集合
来源：http://una.jinghuilouyu.cn

================================================================================
来源：http://zrs.nanxuanxn.top

[D01] 创建数组 / 列表
来源：http://zok.nanxinkj.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://wrx.dashuyun.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nuu.redwolf501.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ytu.cucudq.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://qrc.0kj1m.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://evc.jinqigufen.top

Go:   arr := []int{1, 2, 3}
来源：http://slc.zdqjudy.top

Ruby: arr = [1, 2, 3]
来源：http://tjt.gotoacloud.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://uix.vqdsnc.cn

[D02] 追加元素到末尾
来源：http://hbe.pycfn.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://laz.hesvh.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jvm.9152youxi.cn

JS:   arr.push(4);
来源：http://ukt.tian-w.cn

TS:   arr.push(4);
来源：http://jkx.c1oappe.top

Java: list.add(4);
来源：http://zju.quarkkingdee.top

Go:   arr = append(arr, 4)
来源：http://whh.ppjwa.cn

Ruby: arr << 4; arr.push(5)
来源：http://hfi.gogol.net.cn

C#:   list.Add(4);
来源：http://oqm.mhx1999.top

[D03] 在指定位置插入元素
来源：http://lfk.feifeiyinyue.top

Py:   arr.insert(0, 0)
来源：http://plw.zhiwuduotai.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://amg.vqdsnc.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kua.gzhubu.top

TS:   arr.splice(0, 0, 0);
来源：http://fki.yongpay.top

Java: list.add(0, 0);
来源：http://oan.fehbvm.com

Go:   arr = append([]int{0}, arr...)
来源：http://qsd.yanxiufei.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://goi.guannengcc.top

C#:   list.Insert(0, 0);
来源：http://udf.feifeiyinyue.top

[D04] 删除元素
来源：http://nil.birdmap.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rsi.ppjwa.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hlb.ctjpmb.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yrd.cashguo.top

TS:   arr.splice(0, 1);
来源：http://zyw.9152youxi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tbx.hongshengwenyu.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://quj.xuanzx.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ppl.nanxuanxn.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tsq.zhaomingkeji.xyz

[D05] 访问与修改元素
来源：http://osm.smart0.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bcc.jianghu66.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baq.epnwcf.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cjl.sxryk.cn

TS:   arr[0]; arr.at(-1);
来源：http://rhc.wangdashe.top

Java: list.get(0); list.set(0, 9);
来源：http://czb.kuanghao11.cn

Go:   arr[0]; arr[0] = 9
来源：http://vov.fktsv.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bsv.yj202588.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lcp.yj20258.top

[D06] 数组长度
来源：http://cfb.ywan-chungtsiang.top


<!-- 参考信息 -->
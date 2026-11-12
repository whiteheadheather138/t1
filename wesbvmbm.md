代发 wailian999

[B05] 遍历数组 / 列表
来源：http://nuw.sjlbkw.cn

Py:   for item in arr: print(item)
来源：http://ejo.sysykeji.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vcx.iojbl.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://usx.pycfn.com

TS:   for (const item of arr) { console.log(item); }
来源：http://mta.zhiwuduotai.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://pwp.vqdsnc.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hhf.sxryk.cn

Ruby: arr.each { |item| puts item }
来源：http://lno.0kj1m.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kvz.cashguo.top

[B06] 遍历字典 / 对象
来源：http://wtr.zhoulong.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://mao.uphjek.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cye.hesvh.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oni.shangyingyoupin.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dsa.yueranfly.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xdc.zhongyouzk.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xwv.fengsongda.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://avp.chenzaomai.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://uaa.snrcjt.cn

[B07] while 循环
来源：http://vmn.sjlbkw.cn

Py:   while i < 10: i += 1
来源：http://cmb.yvedp.cn

PHP:  while ($i < 10) { $i++; }
来源：http://gtc.0kj1m.cn

JS:   while (i < 10) { i++; }
来源：http://auv.uphjek.com

TS:   while (i < 10) { i++; }
来源：http://pby.chenjidiqi.icu

Java: while (i < 10) { i++; }
来源：http://fmj.yangfankeji.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vbv.zhoulong.xyz

Ruby: while i < 10; i += 1; end
来源：http://xoj.316326.xyz

C#:   while (i < 10) { i++; }
来源：http://cak.bjfxy.top

[B08] do-while（至少执行一次）
来源：http://ohv.cdnleiting.top

Py:   # 无 do-while：用 while True + break
来源：http://lhy.xingfuxueyuan.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://nuz.mhx1999.top

JS:   do { i++; } while (i < 10);
来源：http://uzl.vehdjk.com

TS:   do { i++; } while (i < 10);
来源：http://ieu.yonumen.top

Java: do { i++; } while (i < 10);
来源：http://ypv.zdqjudy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://wwc.vehdjk.com

Ruby: begin; i += 1; end while i < 10
来源：http://ofd.guannengcc.top

C#:   do { i++; } while (i < 10);
来源：http://sum.shangyingyoupin.top

[B09] break 与 continue
来源：http://yhx.tianlin.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fjo.aizwys.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qfu.zhongyouzk.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jwb.hcnkem.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vln.9152youxi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jtl.0kj1m.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://aem.0kj1m.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://icw.aibaodan.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fqm.yj20258888.top

[B10] 遍历同时拿索引
来源：http://fhk.dashuyun.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dqp.jlsjyb.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vsn.jqgfzy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ibn.kuanghao11.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://eoq.aizwys.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hhm.daxiang520.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bhj.jinqigufen.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sjt.ydzc1.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://not.zhongyouzk.top

[B11] 生成数字序列 / 区间
来源：http://pji.hammf.cn

Py:   list(range(0, 10, 2))
来源：http://cka.snrcjt.cn

PHP:  range(0, 10, 2);
来源：http://tht.feifeiyinyue.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://log.ehwqpu.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jbq.dashuyun.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rqr.fktsv.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dgr.xziqi.cn

Ruby: (0...10).step(2).to_a
来源：http://ebr.zhoulong.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vhe.jiagoushi.top

[B12] 跳出多层循环
来源：http://emm.zhaomingkeji.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://uoe.zdqjudy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://xqy.kuanghao11.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://atj.epnwcf.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zpf.hcnkem.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fif.shzxlz.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nit.zhijiandao.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pym.jqgfzy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ndx.svipenyu.cn

[B13] 判断是否为数字
来源：http://kaw.cheryme.top

Py:   isinstance(x, (int, float))
来源：http://ybm.svipenyu.cn

PHP:  is_numeric($x)
来源：http://gjk.xuetiantiany.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xzm.ivvv.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://avf.ydzc1.top

Java: x instanceof Number
来源：http://lcl.vehdjk.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://clu.jinyuanbaomall.cn

Ruby: x.is_a?(Numeric)
来源：http://xoc.jinqigfzy.top

C#:   x is int or double or decimal
来源：http://jhr.jinqigfzy.top

[B14] 判断值是否在集合内
来源：http://njx.zhengqikj.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vmi.ehwqpu.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ker.tarul.cn

JS:   [1, 2, 3].includes(x)
来源：http://epa.ctjpmb.com

TS:   [1, 2, 3].includes(x)
来源：http://otc.yongpay.top

Java: List.of(1, 2, 3).contains(x)
来源：http://mpz.gaohongyu789.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kwp.zhongyouzk.top

Ruby: [1, 2, 3].include?(x)
来源：http://cpt.xylfe.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zqq.vehdjk.com

[B15] 布尔运算与取反
来源：http://caj.yanxiufei.cn

Py:   a and b or not c
来源：http://nyt.cashguo.top

PHP:  $a && $b || !$c
来源：http://kht.sweek.top

JS:   a && b || !c
来源：http://vli.sysykeji.top

TS:   a && b || !c
来源：http://qxf.daria6918.cn

Java: a && b || !c
来源：http://jim.hywenlv.cn

Go:   a && b || !c
来源：http://yqt.haohaochexian.top

Ruby: a && b || !c
来源：http://vms.fzhhl.top

C#:   a && b || !c
来源：http://oge.yanxiufei.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zfv.fzhhl.top

Py:   if not data: return
来源：http://wml.0kj1m.cn

PHP:  if (!$data) { return; }
来源：http://vrv.xingfuxueyuan.xyz

JS:   if (!data) return;
来源：http://tnt.sufxvd.cn

TS:   if (!data) return;
来源：http://czb.ydzc1.top

Java: if (data == null) return;
来源：http://zco.vqdsnc.cn

Go:   if data == nil { return }
来源：http://xdq.gaohongyu789.top

Ruby: return if data.nil?
来源：http://adk.meibo888.top

C#:   if (data == null) return;
来源：http://qjm.pycfn.com

================================================================================
来源：http://voh.hcnkem.com

C. 函数与作用域
来源：http://xot.gotoacloud.top

================================================================================
来源：http://kli.ctjpmb.com

[C01] 定义函数
来源：http://tbd.cdnleiting.top

Py:   def add(a, b): return a + b
来源：http://ibf.havefunace.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gqb.bjfxy.top

JS:   function add(a, b) { return a + b; }
来源：http://stk.52xcode.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gsx.xingfuxueyuan.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://wox.jinghuilouyu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xmw.ywan-chungtsiang.top

Ruby: def add(a, b); a + b; end
来源：http://mak.hnqzz.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sug.jyoumei.cn

[C02] 默认参数
来源：http://qhe.yvedp.cn

Py:   def greet(name="World"): return name
来源：http://ssr.nanxuanxn.top

PHP:  function greet($name = "World") { return $name; }
来源：http://bkw.andypj.xyz

JS:   function greet(name = "World") { return name; }
来源：http://via.jinqigufen.top

TS:   function greet(name: string = "World") { return name; }
来源：http://pzh.ybcxt.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ihp.vqdsnc.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hgs.316326.xyz

Ruby: def greet(name = "World") = name
来源：http://hsk.hesvh.cn

C#:   string Greet(string name = "World") => name;
来源：http://kid.gzhubu.top

[C03] 可变参数
来源：http://sul.tarul.cn

Py:   def total(*args): return sum(args)
来源：http://kgg.yueranfly.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lbu.tianlin.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pam.cheryme.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dmz.shzxlz.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tyc.shanyushiyangkeji.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yph.xingfuxueyuan.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://dag.epnwcf.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://scl.yonumen.top

[C04] 命名参数 / 关键字参数
来源：http://ktc.yj20258.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rjh.yuanzhike.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dag.zhoulong.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mxd.chenzaomai.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rte.epnwcf.com

Java: // 无：用 Builder 模式或 record
来源：http://qca.zdbjq.cn

Go:   // 无：用配置结构体参数
来源：http://mwj.meibo888.top

Ruby: f(a: 1, b: 2)
来源：http://nnh.yuanzhike.top

C#:   f(a: 1, b: 2)
来源：http://ubx.zhoulong.xyz

[C05] 返回多个值
来源：http://aob.gotoacloud.top

Py:   return a, b
来源：http://rbd.jianghu66.top

PHP:  return [$a, $b];
来源：http://upm.shuidangran.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://uvm.zhijiandao.cn

TS:   return { a, b };
来源：http://ojy.daria6918.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ljy.xuetiantiany.cn

Go:   return a, b
来源：http://any.bbcook.cn

Ruby: return a, b
来源：http://glm.zhixingplan.top

C#:   return (a, b);              // ValueTuple
来源：http://xct.zhoulong.xyz

[C06] 匿名函数 / lambda
来源：http://xbi.jqgfzy.top

Py:   square = lambda x: x * x
来源：http://mud.fehbvm.com

PHP:  $square = fn($x) => $x * $x;
来源：http://vxr.wangdashe.top

JS:   const square = x => x * x;
来源：http://mjc.sxryk.cn

TS:   const square = (x: number): number => x * x;
来源：http://spo.zhijiandao.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ycr.sweek.top

Go:   sq := func(x int) int { return x * x }
来源：http://bwy.tian-w.cn

Ruby: square = ->(x) { x * x }
来源：http://whh.yongpay.top

C#:   Func<int, int> square = x => x * x;
来源：http://qxv.tianlin.xyz

[C07] 把函数作为参数传入
来源：http://vas.uphjek.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ftg.yuxming.cn

PHP:  array_map("strtoupper", $arr);
来源：http://czs.svipenyu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://alj.zhongyouzk.top

TS:   arr.map(String)
来源：http://rnz.nanxinkj.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mwh.hnxiangtu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wro.9152youxi.cn

Ruby: arr.map(&:upcase)
来源：http://nfs.gaohongyu789.top

C#:   arr.Select(s => s.ToUpper())
来源：http://juo.tianlin.xyz

[C08] 闭包
来源：http://pbg.ybcxt.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bae.zhengqikj.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jwb.shuidangran.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qxc.cqqwz.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ame.meibo888.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://esg.zdbjq.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fsi.tarul.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://elo.hongshengwenyu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uqe.zhixingplan.top

[C09] 递归
来源：http://fnd.zdbjq.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pwx.52xcode.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nvc.shanyushiyangtech.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tez.yongpay.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tqs.vqdsnc.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hwh.zhiwuduotai.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hal.daxiang520.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qtc.fehbvm.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ihm.xuetiantiany.cn

[C10] 变量作用域
来源：http://gxj.snrcjt.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://urk.svipenyu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mvg.pycfn.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lfh.chenlongwang.top

TS:   同 JS
来源：http://oji.bjfxy.top

Java: 方法内为块级作用域
来源：http://dcm.xylfe.cn

Go:   花括号块级作用域
来源：http://mpy.mhx1999.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bes.wangdashe.top

C#:   块级作用域
来源：http://atq.havefunace.top

[C11] 模块导入与导出
来源：http://hzh.shzxlz.cn

Py:   from module import func
来源：http://wku.jiagoushi.top

PHP:  require "file.php";  或 use App\Service;
来源：http://qjh.ybcxt.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://qyd.daxiang520.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lcg.jlsjyb.cn

Java: import java.util.List;
来源：http://irz.nwbrower.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vyy.sweek.top

Ruby: require "json"; require_relative "./util"
来源：http://btf.c1oappe.top

C#:   using System.Text;
来源：http://eir.zdqjudy.top

[C12] 立即执行函数 IIFE
来源：http://sso.jqgfzy.top

Py:   (lambda: print("run"))()
来源：http://tcv.zycfv.cn

PHP:  (function () { echo "run"; })();
来源：http://tco.shzxlz.cn

JS:   (() => { console.log("run"); })();
来源：http://sha.hywenlv.cn

TS:   (() => { console.log("run"); })();
来源：http://eoj.cashguo.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bqk.hcnkem.com

Go:   func() { fmt.Println("run") }()
来源：http://jbm.vqdsnc.cn

Ruby: -> { puts "run" }.call
来源：http://djn.andypj.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://ncv.fanxiaobao.xyz

[C13] 类型声明 / 类型注解
来源：http://opy.jlsjyb.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://egj.bbcook.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dsu.hongshengwenyu.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://unl.chenzaomai.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mey.52xcode.cn

Java: int add(int a, int b) { return a + b; }
来源：http://aib.hnxiangtu.top

Go:   func add(a, b int) int
来源：http://zmu.9152youxi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tws.aibaodan.cn

C#:   int Add(int a, int b) => a + b;
来源：http://oop.uphjek.com

[C14] 泛型函数
来源：http://fle.cheryme.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://goy.vqdsnc.cn

PHP:  // 无泛型
来源：http://ajz.tian-w.cn

JS:   // 无泛型
来源：http://rtm.sjlbkw.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nvs.gaohongyu789.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tdh.xziqi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://aud.cashguo.top

Ruby: # 无泛型
来源：http://bmi.cashguo.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nms.epnwcf.com

[C15] 解构 / 展开参数
来源：http://feg.cqqwz.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cle.fengsongda.top

PHP:  [$a, $b] = $pair;
来源：http://yba.gogol.net.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xep.hnxiangtu.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jfp.sweek.top

Java: // 无解构
来源：http://acu.gzhubu.top

Go:   // 无解构
来源：http://cqq.hnqzz.top

Ruby: a, b = pair
来源：http://fea.gaohongyu789.top

C#:   var (a, b) = pair;
来源：http://fuq.chenjidiqi.icu

[C16] 函数 / 方法重载
来源：http://uvu.epnwcf.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cup.xuetiantiany.cn

PHP:  // 无重载
来源：http://uzz.xinyue.icu

JS:   // 无重载：靠 arguments.length 分支
来源：http://uqn.wangdashe.top

TS:   // 用联合类型或重载签名声明
来源：http://ioo.zhijiandao.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://nyu.epnwcf.com

Go:   // 无重载：用不同函数名
来源：http://lpw.mhx1999.top

Ruby: # 无重载：靠动态参数
来源：http://gid.hfpthk.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ymd.wangdashe.top

================================================================================
来源：http://non.cashguo.top

D. 数组 / 列表 / 集合
来源：http://onj.hnxiangtu.top

================================================================================
来源：http://sci.chenlongwang.top

[D01] 创建数组 / 列表
来源：http://qxd.chenjidiqi.icu

Py:   arr = [1, 2, 3];  empty = []
来源：http://cix.ehwqpu.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cxq.xingfuxueyuan.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://isc.jinqigfzy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://hxc.cheryme.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://quq.zhijiandao.cn

Go:   arr := []int{1, 2, 3}
来源：http://fbe.zhoulong.xyz

Ruby: arr = [1, 2, 3]
来源：http://ktv.yj20258.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hjc.xuanzx.com

[D02] 追加元素到末尾
来源：http://lrm.ehwqpu.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ent.jqgfzy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kzq.hfpthk.cn

JS:   arr.push(4);
来源：http://lvq.fanxiaobao.xyz

TS:   arr.push(4);
来源：http://vxm.nanxinkj.top

Java: list.add(4);
来源：http://xbd.wangshuangyany.cn

Go:   arr = append(arr, 4)
来源：http://jsg.ctjpmb.com

Ruby: arr << 4; arr.push(5)
来源：http://dwl.hysaishi.cn

C#:   list.Add(4);
来源：http://gqu.ywan-chungtsiang.top

[D03] 在指定位置插入元素
来源：http://iwg.cucudq.cn

Py:   arr.insert(0, 0)
来源：http://swt.pengpengdd.cyou

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pcv.zhijiandao.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hoc.sjlbkw.cn

TS:   arr.splice(0, 0, 0);
来源：http://qyy.c1oappe.top

Java: list.add(0, 0);
来源：http://lbm.ctjpmb.com

Go:   arr = append([]int{0}, arr...)
来源：http://est.tanke756.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wmg.smart0.xyz

C#:   list.Insert(0, 0);
来源：http://iav.jlsjyb.cn

[D04] 删除元素
来源：http://ook.jinghuilouyu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://icj.tianlin.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tph.aibaodan.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kef.daxiang520.top

TS:   arr.splice(0, 1);
来源：http://jum.yuanzhike.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qai.gzhubu.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vlt.kuanghao11.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://euh.yonumen.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gxx.vqdsnc.cn

[D05] 访问与修改元素
来源：http://qsu.zdqjudy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://syf.wangdashe.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rrc.yj20258888.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kje.tarul.cn

TS:   arr[0]; arr.at(-1);
来源：http://xiw.svipenyu.cn

Java: list.get(0); list.set(0, 9);
来源：http://tlw.zhoulong.xyz


<!-- 参考信息 -->
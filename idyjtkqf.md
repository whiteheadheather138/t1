代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://teu.sufxvd.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://iec.wangshuangyany.cn

JS:   do { i++; } while (i < 10);
来源：http://cxv.cashguo.top

TS:   do { i++; } while (i < 10);
来源：http://bap.vqdsnc.cn

Java: do { i++; } while (i < 10);
来源：http://buf.jiagoushi.top

Go:   for { i++; if i >= 10 { break } }
来源：http://nsk.tianlin.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://wnh.dianchejie.cn

C#:   do { i++; } while (i < 10);
来源：http://xdi.nanxinkj.top

[B09] break 与 continue
来源：http://tps.andypj.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gtm.chenlongwang.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://acb.epnwcf.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://acy.shuidangran.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xkt.bbcook.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cqi.smart0.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ezq.shzxlz.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hfh.kuanghao11.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ozw.9152youxi.cn

[B10] 遍历同时拿索引
来源：http://mry.ybcxt.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://byq.hcnkem.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yfs.yuanzhike.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vvc.fengsongda.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lts.yj20258888.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zwr.yanxiufei.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vba.guowangkeji.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hgf.0kj1m.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dvq.jiagoushi.top

[B11] 生成数字序列 / 区间
来源：http://sew.dashuyun.cn

Py:   list(range(0, 10, 2))
来源：http://plu.ehwqpu.com

PHP:  range(0, 10, 2);
来源：http://ivs.jqgufenzy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hou.hcnkem.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zjd.jyoumei.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pnz.shuidangran.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fbe.vehdjk.com

Ruby: (0...10).step(2).to_a
来源：http://hdc.zhengqikj.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nbp.ybcxt.top

[B12] 跳出多层循环
来源：http://wjk.9152youxi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://uqs.cqqwz.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fwq.yanxiufei.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tty.yj20258.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mvq.yonumen.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bar.shangyingyoupin.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://whe.yuanzhike.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bji.yvedp.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ghw.jlsjyb.cn

[B13] 判断是否为数字
来源：http://dwz.snrcjt.cn

Py:   isinstance(x, (int, float))
来源：http://qwn.yangfankeji.com

PHP:  is_numeric($x)
来源：http://avz.snrcjt.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wxn.yanxiufei.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lkw.shzxlz.cn

Java: x instanceof Number
来源：http://nfi.tian-w.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qnf.nwbrower.top

Ruby: x.is_a?(Numeric)
来源：http://lbq.9152youxi.cn

C#:   x is int or double or decimal
来源：http://jny.sweek.top

[B14] 判断值是否在集合内
来源：http://vgp.jinyuanbaomall.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://thz.hnqzz.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yyd.yangfankeji.com

JS:   [1, 2, 3].includes(x)
来源：http://vwn.c1oappe.top

TS:   [1, 2, 3].includes(x)
来源：http://bpw.pycfn.com

Java: List.of(1, 2, 3).contains(x)
来源：http://oye.redwolf501.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hgt.sjlbkw.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ajf.yanxiufei.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ilp.cashguo.top

[B15] 布尔运算与取反
来源：http://kaj.bbcook.cn

Py:   a and b or not c
来源：http://tjr.ydjk.org.cn

PHP:  $a && $b || !$c
来源：http://cmx.ivvv.top

JS:   a && b || !c
来源：http://tmt.mhx1999.top

TS:   a && b || !c
来源：http://apz.ywan-chungtsiang.top

Java: a && b || !c
来源：http://ygu.yuanzhike.top

Go:   a && b || !c
来源：http://cfs.0kj1m.cn

Ruby: a && b || !c
来源：http://mlg.daxiang520.top

C#:   a && b || !c
来源：http://rpr.chenjidiqi.icu

[B16] 卫语句：不满足条件提前返回
来源：http://nnq.ppjwa.cn

Py:   if not data: return
来源：http://pmg.cdnleiting.top

PHP:  if (!$data) { return; }
来源：http://ady.fzhhl.top

JS:   if (!data) return;
来源：http://ihc.mhx1999.top

TS:   if (!data) return;
来源：http://yeo.chenzaomai.com

Java: if (data == null) return;
来源：http://eyh.zhijiandao.cn

Go:   if data == nil { return }
来源：http://gvs.sysykeji.top

Ruby: return if data.nil?
来源：http://lap.chenjidiqi.icu

C#:   if (data == null) return;
来源：http://goc.jinghuilouyu.cn

================================================================================
来源：http://vcu.yvedp.cn

C. 函数与作用域
来源：http://xvw.ehwqpu.com

================================================================================
来源：http://fde.nanxinkj.top

[C01] 定义函数
来源：http://ipp.nwbrower.top

Py:   def add(a, b): return a + b
来源：http://wmu.yj202588.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://avp.hongshengwenyu.top

JS:   function add(a, b) { return a + b; }
来源：http://kuj.dianchejie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sbg.jiagoushi.top

Java: static int add(int a, int b) { return a + b; }
来源：http://sdw.andypj.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://vof.ehwqpu.com

Ruby: def add(a, b); a + b; end
来源：http://ydo.aibaodan.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nrb.jianghu66.top

[C02] 默认参数
来源：http://uok.pycfn.com

Py:   def greet(name="World"): return name
来源：http://pmd.ydzc1.top

PHP:  function greet($name = "World") { return $name; }
来源：http://urv.snrcjt.cn

JS:   function greet(name = "World") { return name; }
来源：http://nrd.cucudq.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wax.xziqi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qto.316326.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tkw.iojbl.cn

Ruby: def greet(name = "World") = name
来源：http://lfp.yueranfly.top

C#:   string Greet(string name = "World") => name;
来源：http://iyv.chenjidiqi.icu

[C03] 可变参数
来源：http://xac.smart0.xyz

Py:   def total(*args): return sum(args)
来源：http://dcr.gzhubu.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ufe.cashguo.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mwq.jinqigufen.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://eip.vehdjk.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yvk.zhiwuduotai.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wkz.fehbvm.com

Ruby: def total(*nums); nums.sum; end
来源：http://xah.zycfv.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cgv.gotoacloud.top

[C04] 命名参数 / 关键字参数
来源：http://vtu.yuxming.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://amu.ivvv.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pff.nwbrower.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ice.xingfuxueyuan.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zql.fehbvm.com

Java: // 无：用 Builder 模式或 record
来源：http://qyh.yvedp.cn

Go:   // 无：用配置结构体参数
来源：http://eqp.yuxming.cn

Ruby: f(a: 1, b: 2)
来源：http://wmj.vehdjk.com

C#:   f(a: 1, b: 2)
来源：http://pad.zhaomingkeji.xyz

[C05] 返回多个值
来源：http://hln.chenzaomai.com

Py:   return a, b
来源：http://jmj.bjfxy.top

PHP:  return [$a, $b];
来源：http://vsl.zhengqikj.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://phg.hammf.cn

TS:   return { a, b };
来源：http://bej.bjfxy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sye.birdmap.top

Go:   return a, b
来源：http://sgh.pycfn.com

Ruby: return a, b
来源：http://qfy.jiagoushi.top

C#:   return (a, b);              // ValueTuple
来源：http://qsz.cucudq.cn

[C06] 匿名函数 / lambda
来源：http://wcd.hesvh.cn

Py:   square = lambda x: x * x
来源：http://rbc.jlsjyb.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xyp.yuxming.cn

JS:   const square = x => x * x;
来源：http://tyz.hnxiangtu.top

TS:   const square = (x: number): number => x * x;
来源：http://eey.0kj1m.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qho.dashuyun.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jtz.jiagoushi.top

Ruby: square = ->(x) { x * x }
来源：http://uem.dianchejie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://vtq.uphjek.com

[C07] 把函数作为参数传入
来源：http://ymg.wangdashe.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vxd.nwbrower.top

PHP:  array_map("strtoupper", $arr);
来源：http://uip.gotoacloud.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xsr.zhengqikj.top

TS:   arr.map(String)
来源：http://lvg.yangfankeji.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hji.sufxvd.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zpi.smart0.xyz

Ruby: arr.map(&:upcase)
来源：http://rzs.nanxuanxn.top

C#:   arr.Select(s => s.ToUpper())
来源：http://rho.jinyuanbaomall.cn

[C08] 闭包
来源：http://ryl.jinghuilouyu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jth.yfazqb.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uqj.wangdashe.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dhv.chenjidiqi.icu

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nrv.yj202588.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://eof.ywan-chungtsiang.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ies.dianchejie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fyu.jiagoushi.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ngo.wangdashe.top

[C09] 递归
来源：http://ecz.zhijiandao.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://afm.cucudq.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sxi.tianlin.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ghx.jiagoushi.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qvc.hnqzz.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://diw.jlsjyb.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://oos.yj20258.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jhq.smart0.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wxc.hongshengwenyu.top

[C10] 变量作用域
来源：http://xjf.uphjek.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://aze.wangshuangyany.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mxk.yanxiufei.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://huj.xziqi.cn

TS:   同 JS
来源：http://mdi.zhijiandao.cn

Java: 方法内为块级作用域
来源：http://dwk.feifeiyinyue.top

Go:   花括号块级作用域
来源：http://jsk.xziqi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qah.yuanzhike.top

C#:   块级作用域
来源：http://bey.yongpay.top

[C11] 模块导入与导出
来源：http://szg.ydjk.org.cn

Py:   from module import func
来源：http://mcf.zycfv.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://kdr.ctjpmb.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://jpu.sxryk.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kgz.cucudq.cn

Java: import java.util.List;
来源：http://zys.shzxlz.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ith.guowangkeji.top

Ruby: require "json"; require_relative "./util"
来源：http://oqb.birdmap.top

C#:   using System.Text;
来源：http://gcs.shanyushiyangkeji.top

[C12] 立即执行函数 IIFE
来源：http://lyo.zdbjq.cn

Py:   (lambda: print("run"))()
来源：http://tlf.guannengcc.top

PHP:  (function () { echo "run"; })();
来源：http://zcu.yonumen.top

JS:   (() => { console.log("run"); })();
来源：http://urp.chenzaomai.com

TS:   (() => { console.log("run"); })();
来源：http://unj.ydjk.org.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://iad.fzhhl.top

Go:   func() { fmt.Println("run") }()
来源：http://wov.zhijiandao.cn

Ruby: -> { puts "run" }.call
来源：http://upi.pycfn.com

C#:   // 无 IIFE：用静态构造函数
来源：http://iif.yuanzhike.top

[C13] 类型声明 / 类型注解
来源：http://kkb.jianghu66.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mas.ydzc1.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://efu.shangyingyoupin.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kzv.zhixingplan.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vun.vqdsnc.cn

Java: int add(int a, int b) { return a + b; }
来源：http://hgd.yfazqb.com

Go:   func add(a, b int) int
来源：http://sfp.kuanghao11.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wqh.yuxming.cn

C#:   int Add(int a, int b) => a + b;
来源：http://amg.shangyingyoupin.top

[C14] 泛型函数
来源：http://pvw.shuidangran.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ecm.quarkkingdee.top

PHP:  // 无泛型
来源：http://oqq.nanxuanxn.top

JS:   // 无泛型
来源：http://eha.ydzc1.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://axx.kuanghao11.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xwb.gogol.net.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pxc.gaohongyu789.top

Ruby: # 无泛型
来源：http://zdy.shanyushiyangkeji.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://toq.dianchejie.cn

[C15] 解构 / 展开参数
来源：http://brd.zdqjudy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rpu.cdnleiting.top

PHP:  [$a, $b] = $pair;
来源：http://zkk.yanxiufei.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lzn.yfazqb.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xcz.hnqzz.top

Java: // 无解构
来源：http://hdg.gogol.net.cn

Go:   // 无解构
来源：http://euj.aizwys.cn

Ruby: a, b = pair
来源：http://mhe.fzhhl.top

C#:   var (a, b) = pair;
来源：http://rqd.jiagoushi.top

[C16] 函数 / 方法重载
来源：http://que.chenjidiqi.icu

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gcd.xuanzx.com

PHP:  // 无重载
来源：http://wqp.0kj1m.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://wqo.jqgufenzy.top

TS:   // 用联合类型或重载签名声明
来源：http://epr.ctjpmb.com

Java: void f(int a) {}  void f(String a) {}
来源：http://rpc.shanyushiyangkeji.top

Go:   // 无重载：用不同函数名
来源：http://gps.svipenyu.cn

Ruby: # 无重载：靠动态参数
来源：http://egq.yvedp.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://bgl.bbcook.cn

================================================================================
来源：http://enl.hnxiangtu.top

D. 数组 / 列表 / 集合
来源：http://wgg.andypj.xyz

================================================================================
来源：http://blg.pycfn.com

[D01] 创建数组 / 列表
来源：http://oem.bjfxy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ubf.xinyue.icu

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://swr.cheryme.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hfk.xingfuxueyuan.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://xgb.yonumen.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bqo.ivvv.top

Go:   arr := []int{1, 2, 3}
来源：http://mza.nwbrower.top

Ruby: arr = [1, 2, 3]
来源：http://lfb.jiagoushi.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://foe.cashguo.top

[D02] 追加元素到末尾
来源：http://aqs.sweek.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lup.meibo888.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://brn.gaohongyu789.top

JS:   arr.push(4);
来源：http://ack.zhijiandao.cn

TS:   arr.push(4);
来源：http://qkd.jlsjyb.cn

Java: list.add(4);
来源：http://hok.tarul.cn

Go:   arr = append(arr, 4)
来源：http://jty.xuanzx.com

Ruby: arr << 4; arr.push(5)
来源：http://qoi.gogol.net.cn

C#:   list.Add(4);
来源：http://tah.cashguo.top

[D03] 在指定位置插入元素
来源：http://yce.ctjpmb.com

Py:   arr.insert(0, 0)
来源：http://mqv.fehbvm.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gyf.zdqjudy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hrb.wangshuangyany.cn

TS:   arr.splice(0, 0, 0);
来源：http://jta.chenzaomai.com

Java: list.add(0, 0);
来源：http://flx.hcnkem.com

Go:   arr = append([]int{0}, arr...)
来源：http://jvs.fanxiaobao.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jap.tarul.cn

C#:   list.Insert(0, 0);
来源：http://shp.hnqzz.top

[D04] 删除元素
来源：http://vih.fengsongda.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gqv.xingfuxueyuan.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vju.vehdjk.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cde.fktsv.cn

TS:   arr.splice(0, 1);
来源：http://hqe.nwbrower.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ezg.uphjek.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gmk.c1oappe.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vtt.sufxvd.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vnu.smart0.xyz

[D05] 访问与修改元素
来源：http://ojo.9152youxi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cxr.dashuyun.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tjv.nanxuanxn.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qno.yvedp.cn

TS:   arr[0]; arr.at(-1);
来源：http://mga.havefunace.top

Java: list.get(0); list.set(0, 9);
来源：http://wby.yanxiufei.cn

Go:   arr[0]; arr[0] = 9
来源：http://snt.nanxinkj.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kpj.ywan-chungtsiang.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bow.shangyingyoupin.top

[D06] 数组长度
来源：http://sdy.epnwcf.com

Py:   len(arr)
来源：http://fvo.andypj.xyz

PHP:  count($arr);
来源：http://xqz.fehbvm.com

JS:   arr.length
来源：http://ooh.zdqjudy.top

TS:   arr.length
来源：http://bzf.dashuyun.cn

Java: list.size();
来源：http://qkw.dashuyun.cn

Go:   len(arr)
来源：http://tey.gzhubu.top

Ruby: arr.length; arr.size
来源：http://dfr.cashguo.top

C#:   list.Count;
来源：http://ioy.nanxuanxn.top

[D07] 切片 / 取子数组
来源：http://wnu.guowangkeji.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://grl.sufxvd.cn

PHP:  array_slice($arr, 1, 3);
来源：http://lsw.fehbvm.com

JS:   arr.slice(1, 4);
来源：http://xbw.aizwys.cn

TS:   arr.slice(1, 4);
来源：http://uvb.vehdjk.com

Java: list.subList(1, 4);
来源：http://xpg.tarul.cn

Go:   arr[1:4]
来源：http://nts.ppjwa.cn

Ruby: arr[1, 3]
来源：http://myn.aizwys.cn

C#:   list.GetRange(1, 3);
来源：http://ucv.52xcode.cn

[D08] 合并两个数组
来源：http://kaq.havefunace.top

Py:   a + b;  a.extend(b)
来源：http://ehc.ctjpmb.com

PHP:  array_merge($a, $b);
来源：http://efd.sxryk.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gcx.52xcode.cn

TS:   [...a, ...b];
来源：http://xgo.tanke756.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pkm.zhengqikj.top

Go:   append(a, b...)
来源：http://zmi.gzhubu.top


<!-- 参考信息 -->
代发 wailian999

[B09] break 与 continue
来源：http://npp.shanyushiyangtech.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rfp.haohaochexian.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jzg.yangfankeji.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tvb.zycfv.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wjj.shanyushiyangkeji.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lht.ywan-chungtsiang.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://iwx.hammf.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://sra.hnxiangtu.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ric.shuidangran.top

[B10] 遍历同时拿索引
来源：http://gwv.quarkkingdee.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jvn.feifeiyinyue.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bno.mhx1999.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ntm.hammf.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wad.wangshuangyany.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xqp.0kj1m.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vux.sjlbkw.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ptk.cheryme.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://soh.jyoumei.cn

[B11] 生成数字序列 / 区间
来源：http://eve.zdqjudy.top

Py:   list(range(0, 10, 2))
来源：http://mqp.cheryme.top

PHP:  range(0, 10, 2);
来源：http://ytb.yj202588.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vqj.52xcode.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bvh.0kj1m.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://htt.ehwqpu.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cdt.zdqjudy.top

Ruby: (0...10).step(2).to_a
来源：http://tak.jqgufenzy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://spo.smart0.xyz

[B12] 跳出多层循环
来源：http://upp.wangshuangyany.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://lja.hnxiangtu.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://trv.yonumen.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hra.c1oappe.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://uev.fktsv.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nwv.ctjpmb.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zgj.yuxming.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ofz.guannengcc.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://obd.0kj1m.cn

[B13] 判断是否为数字
来源：http://bym.yueranfly.top

Py:   isinstance(x, (int, float))
来源：http://pja.snrcjt.cn

PHP:  is_numeric($x)
来源：http://tun.fanxiaobao.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://esn.fehbvm.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dea.yueranfly.top

Java: x instanceof Number
来源：http://ofl.shangyingyoupin.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sgt.xuetiantiany.cn

Ruby: x.is_a?(Numeric)
来源：http://brd.zhaomingkeji.xyz

C#:   x is int or double or decimal
来源：http://abo.yj20258888.top

[B14] 判断值是否在集合内
来源：http://osh.jqgufenzy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://woz.sufxvd.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ayr.xinyue.icu

JS:   [1, 2, 3].includes(x)
来源：http://gsx.ydzc1.top

TS:   [1, 2, 3].includes(x)
来源：http://uus.vehdjk.com

Java: List.of(1, 2, 3).contains(x)
来源：http://val.bbcook.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ejs.iojbl.cn

Ruby: [1, 2, 3].include?(x)
来源：http://obb.vqdsnc.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nsj.yanxiufei.cn

[B15] 布尔运算与取反
来源：http://wli.sysykeji.top

Py:   a and b or not c
来源：http://htp.ydzc1.top

PHP:  $a && $b || !$c
来源：http://yar.yuxming.cn

JS:   a && b || !c
来源：http://kvw.chenlongwang.top

TS:   a && b || !c
来源：http://ups.tian-w.cn

Java: a && b || !c
来源：http://dkq.sxryk.cn

Go:   a && b || !c
来源：http://xyh.tanke756.top

Ruby: a && b || !c
来源：http://znh.jinqigufen.top

C#:   a && b || !c
来源：http://lbw.dianchejie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lgo.yuxming.cn

Py:   if not data: return
来源：http://sqi.cucudq.cn

PHP:  if (!$data) { return; }
来源：http://kzn.yj20258.top

JS:   if (!data) return;
来源：http://jfu.yueranfly.top

TS:   if (!data) return;
来源：http://ngx.yongpay.top

Java: if (data == null) return;
来源：http://ajg.shangyingyoupin.top

Go:   if data == nil { return }
来源：http://ozq.hywenlv.cn

Ruby: return if data.nil?
来源：http://mqr.kuanghao11.cn

C#:   if (data == null) return;
来源：http://voi.yangfankeji.com

================================================================================
来源：http://yeo.zhaomingkeji.xyz

C. 函数与作用域
来源：http://cif.meibo888.top

================================================================================
来源：http://zoo.ydjk.org.cn

[C01] 定义函数
来源：http://bzb.zdbjq.cn

Py:   def add(a, b): return a + b
来源：http://bbi.snrcjt.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dit.hfpthk.cn

JS:   function add(a, b) { return a + b; }
来源：http://bfy.ehwqpu.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hjg.redwolf501.top

Java: static int add(int a, int b) { return a + b; }
来源：http://vnu.9152youxi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jvu.hnxiangtu.top

Ruby: def add(a, b); a + b; end
来源：http://cmv.c1oappe.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ijv.ydjk.org.cn

[C02] 默认参数
来源：http://zlu.xziqi.cn

Py:   def greet(name="World"): return name
来源：http://lan.sweek.top

PHP:  function greet($name = "World") { return $name; }
来源：http://qeu.cqqwz.cn

JS:   function greet(name = "World") { return name; }
来源：http://oqm.dianchejie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://dgc.chenzaomai.com

Java: // 无默认参数：方法重载或 Optional
来源：http://pqu.jinghuilouyu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gtw.nwbrower.top

Ruby: def greet(name = "World") = name
来源：http://adk.hysaishi.cn

C#:   string Greet(string name = "World") => name;
来源：http://vpc.sweek.top

[C03] 可变参数
来源：http://lks.zhoulong.xyz

Py:   def total(*args): return sum(args)
来源：http://oiv.smart0.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bmi.yongpay.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sye.pycfn.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://swm.sysykeji.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vyx.xuanzx.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zxy.tian-w.cn

Ruby: def total(*nums); nums.sum; end
来源：http://quq.316326.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rko.haohaochexian.top

[C04] 命名参数 / 关键字参数
来源：http://czb.hnxiangtu.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://izk.yonumen.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lkz.316326.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ago.jinyuanbaomall.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jbp.guowangkeji.top

Java: // 无：用 Builder 模式或 record
来源：http://pwp.hnxiangtu.top

Go:   // 无：用配置结构体参数
来源：http://rzn.pycfn.com

Ruby: f(a: 1, b: 2)
来源：http://ptv.zdqjudy.top

C#:   f(a: 1, b: 2)
来源：http://hqe.hongshengwenyu.top

[C05] 返回多个值
来源：http://huv.snrcjt.cn

Py:   return a, b
来源：http://gqi.zhoulong.xyz

PHP:  return [$a, $b];
来源：http://vtm.daria6918.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yop.jianghu66.top

TS:   return { a, b };
来源：http://kjk.chenjidiqi.icu

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://reh.havefunace.top

Go:   return a, b
来源：http://myn.jlsjyb.cn

Ruby: return a, b
来源：http://csk.jlsjyb.cn

C#:   return (a, b);              // ValueTuple
来源：http://lqg.mhx1999.top

[C06] 匿名函数 / lambda
来源：http://ddz.vqdsnc.cn

Py:   square = lambda x: x * x
来源：http://uxl.fanxiaobao.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://hbz.shanyushiyangkeji.top

JS:   const square = x => x * x;
来源：http://owz.cashguo.top

TS:   const square = (x: number): number => x * x;
来源：http://ckd.mhx1999.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mks.tarul.cn

Go:   sq := func(x int) int { return x * x }
来源：http://irp.vqdsnc.cn

Ruby: square = ->(x) { x * x }
来源：http://hpa.chenjidiqi.icu

C#:   Func<int, int> square = x => x * x;
来源：http://udz.nanxuanxn.top

[C07] 把函数作为参数传入
来源：http://raj.mhx1999.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://avc.jyoumei.cn

PHP:  array_map("strtoupper", $arr);
来源：http://mte.guowangkeji.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jka.quarkkingdee.top

TS:   arr.map(String)
来源：http://kfi.fzhhl.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fjm.yfazqb.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jil.tianlin.xyz

Ruby: arr.map(&:upcase)
来源：http://xhd.yj202588.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ryn.xylfe.cn

[C08] 闭包
来源：http://ynb.haohaochexian.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gff.tanke756.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pay.jinghuilouyu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vce.fehbvm.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fbe.cqqwz.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hcm.hfpthk.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zvx.pycfn.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zkf.yangfankeji.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mxi.yanxiufei.cn

[C09] 递归
来源：http://zut.nanxinkj.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pzj.zhaomingkeji.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qfi.nanxinkj.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wmd.zhijiandao.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rfa.epnwcf.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dcg.birdmap.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vfx.jianghu66.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://feu.chenzaomai.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kda.sweek.top

[C10] 变量作用域
来源：http://imh.yuxming.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kvf.hnxiangtu.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mod.gotoacloud.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hgh.yfazqb.com

TS:   同 JS
来源：http://wgk.jianghu66.top

Java: 方法内为块级作用域
来源：http://wzr.nanxinkj.top

Go:   花括号块级作用域
来源：http://zrx.hcnkem.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gjc.yj20258.top

C#:   块级作用域
来源：http://bha.svipenyu.cn

[C11] 模块导入与导出
来源：http://gsu.xziqi.cn

Py:   from module import func
来源：http://hli.ehwqpu.com

PHP:  require "file.php";  或 use App\Service;
来源：http://oqr.chenlongwang.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://vqp.chenjidiqi.icu

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ijb.uphjek.com

Java: import java.util.List;
来源：http://wgc.gotoacloud.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dgw.sxryk.cn

Ruby: require "json"; require_relative "./util"
来源：http://xra.shangyingyoupin.top

C#:   using System.Text;
来源：http://awq.jlsjyb.cn

[C12] 立即执行函数 IIFE
来源：http://dwz.jqgufenzy.top

Py:   (lambda: print("run"))()
来源：http://ize.vqdsnc.cn

PHP:  (function () { echo "run"; })();
来源：http://mcr.vehdjk.com

JS:   (() => { console.log("run"); })();
来源：http://jcm.fanxiaobao.xyz

TS:   (() => { console.log("run"); })();
来源：http://eei.gogol.net.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yhy.shangyingyoupin.top

Go:   func() { fmt.Println("run") }()
来源：http://aqw.yj20258888.top

Ruby: -> { puts "run" }.call
来源：http://ped.guowangkeji.top

C#:   // 无 IIFE：用静态构造函数
来源：http://eut.wangshuangyany.cn

[C13] 类型声明 / 类型注解
来源：http://whz.andypj.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pyf.sufxvd.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://seh.yj20258.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wzj.gzhubu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jaa.jiagoushi.top

Java: int add(int a, int b) { return a + b; }
来源：http://mot.cqqwz.cn

Go:   func add(a, b int) int
来源：http://jpi.fzhhl.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mlh.meibo888.top

C#:   int Add(int a, int b) => a + b;
来源：http://lkm.jlsjyb.cn

[C14] 泛型函数
来源：http://cpo.hywenlv.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ght.zhiwuduotai.top

PHP:  // 无泛型
来源：http://isy.svipenyu.cn

JS:   // 无泛型
来源：http://qxk.sweek.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mea.zhoulong.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cjz.xziqi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hip.vehdjk.com

Ruby: # 无泛型
来源：http://pal.guannengcc.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://adb.yuxming.cn

[C15] 解构 / 展开参数
来源：http://mvh.hesvh.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ewf.aibaodan.cn

PHP:  [$a, $b] = $pair;
来源：http://exf.tian-w.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kke.jqgfzy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mog.pengpengdd.cyou

Java: // 无解构
来源：http://rpz.nanxinkj.top

Go:   // 无解构
来源：http://idq.hysaishi.cn

Ruby: a, b = pair
来源：http://ivf.zdqjudy.top

C#:   var (a, b) = pair;
来源：http://uki.xylfe.cn

[C16] 函数 / 方法重载
来源：http://fgp.jqgufenzy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://clc.chenlongwang.top

PHP:  // 无重载
来源：http://jby.zhiwuduotai.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://gyg.zhoulong.xyz

TS:   // 用联合类型或重载签名声明
来源：http://knn.uphjek.com

Java: void f(int a) {}  void f(String a) {}
来源：http://zmb.sysykeji.top

Go:   // 无重载：用不同函数名
来源：http://orh.yvedp.cn

Ruby: # 无重载：靠动态参数
来源：http://tka.zhongyouzk.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://fzq.ydjk.org.cn

================================================================================
来源：http://dyc.birdmap.top

D. 数组 / 列表 / 集合
来源：http://qkf.316326.xyz

================================================================================
来源：http://ojk.hnqzz.top

[D01] 创建数组 / 列表
来源：http://oev.shuidangran.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://rlg.ydzc1.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qst.quarkkingdee.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mba.xziqi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://tua.andypj.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nmo.redwolf501.top

Go:   arr := []int{1, 2, 3}
来源：http://vmx.zhaomingkeji.xyz

Ruby: arr = [1, 2, 3]
来源：http://stm.daria6918.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ued.shuidangran.top

[D02] 追加元素到末尾
来源：http://wdz.ywan-chungtsiang.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tcq.jyoumei.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sdt.jqgufenzy.top

JS:   arr.push(4);
来源：http://oqu.zdqjudy.top

TS:   arr.push(4);
来源：http://ssi.snrcjt.cn

Java: list.add(4);
来源：http://kko.aizwys.cn

Go:   arr = append(arr, 4)
来源：http://vwo.zhongyouzk.top

Ruby: arr << 4; arr.push(5)
来源：http://idc.zhongyouzk.top

C#:   list.Add(4);
来源：http://cus.birdmap.top

[D03] 在指定位置插入元素
来源：http://jjb.yj20258.top

Py:   arr.insert(0, 0)
来源：http://nln.c1oappe.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://klz.yanxiufei.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wuv.pycfn.com

TS:   arr.splice(0, 0, 0);
来源：http://jvx.havefunace.top

Java: list.add(0, 0);
来源：http://nzk.hywenlv.cn

Go:   arr = append([]int{0}, arr...)
来源：http://smv.nwbrower.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ici.ehwqpu.com

C#:   list.Insert(0, 0);
来源：http://utc.xinyue.icu

[D04] 删除元素
来源：http://npf.zhixingplan.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gfz.pycfn.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hxl.cdnleiting.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wpr.0kj1m.cn

TS:   arr.splice(0, 1);
来源：http://pvu.jlsjyb.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://smd.zhiwuduotai.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://scu.9152youxi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gqe.ppjwa.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ytf.ybcxt.top

[D05] 访问与修改元素
来源：http://ing.zdqjudy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gam.quarkkingdee.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qvi.aibaodan.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://guk.52xcode.cn

TS:   arr[0]; arr.at(-1);
来源：http://bkf.yj20258.top

Java: list.get(0); list.set(0, 9);
来源：http://eld.iojbl.cn

Go:   arr[0]; arr[0] = 9
来源：http://qxz.bbcook.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rnq.gzhubu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mfm.cheryme.top

[D06] 数组长度
来源：http://abj.guannengcc.top

Py:   len(arr)
来源：http://rhk.yj202588.top

PHP:  count($arr);
来源：http://gxt.hesvh.cn

JS:   arr.length
来源：http://kyo.aibaodan.cn

TS:   arr.length
来源：http://cgv.cdnleiting.top

Java: list.size();
来源：http://whp.tian-w.cn

Go:   len(arr)
来源：http://zza.52xcode.cn

Ruby: arr.length; arr.size
来源：http://hya.yfazqb.com

C#:   list.Count;
来源：http://jcg.0kj1m.cn

[D07] 切片 / 取子数组
来源：http://baj.sweek.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://anz.52xcode.cn

PHP:  array_slice($arr, 1, 3);
来源：http://bbh.yonumen.top

JS:   arr.slice(1, 4);
来源：http://fja.ydzc1.top

TS:   arr.slice(1, 4);
来源：http://zfr.hfpthk.cn

Java: list.subList(1, 4);
来源：http://ycm.gzhubu.top

Go:   arr[1:4]
来源：http://tcj.shanyushiyangtech.top

Ruby: arr[1, 3]
来源：http://dbq.9152youxi.cn

C#:   list.GetRange(1, 3);
来源：http://szb.shanyushiyangkeji.top

[D08] 合并两个数组
来源：http://nkg.tanke756.top

Py:   a + b;  a.extend(b)
来源：http://azp.yangfankeji.com

PHP:  array_merge($a, $b);
来源：http://eju.shangyingyoupin.top

JS:   [...a, ...b];  a.concat(b);
来源：http://mgp.gogol.net.cn

TS:   [...a, ...b];
来源：http://lpp.xylfe.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://apu.quarkkingdee.top

Go:   append(a, b...)
来源：http://rse.yfazqb.com

Ruby: a + b;  a.concat(b)
来源：http://zkf.fengsongda.top

C#:   a.Concat(b).ToList()
来源：http://ezs.smart0.xyz

[D09] 排序（升序）
来源：http://avh.fktsv.cn

Py:   sorted(arr);  arr.sort()
来源：http://iho.yj202588.top

PHP:  sort($arr);
来源：http://dhj.gzhubu.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://smz.cdnleiting.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://vpk.cdnleiting.top

Java: Collections.sort(list);  list.sort(null);
来源：http://hcq.ywan-chungtsiang.top


<!-- 参考信息 -->
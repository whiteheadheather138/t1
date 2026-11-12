代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://kbi.tanke756.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ddr.fktsv.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zjj.hongshengwenyu.top

C#:   do { i++; } while (i < 10);
来源：http://jie.cucudq.cn

[B09] break 与 continue
来源：http://isn.yuanzhike.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ypf.cashguo.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kgd.jlsjyb.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xoe.sweek.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xrx.chenlongwang.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rma.yuanzhike.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zbz.jinqigfzy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xpv.chenjidiqi.icu

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qnn.jlsjyb.cn

[B10] 遍历同时拿索引
来源：http://okj.yvedp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kwp.chenzaomai.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hfd.uphjek.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vng.feifeiyinyue.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hcq.ppjwa.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qvj.zhiwuduotai.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://iuh.vqdsnc.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kpx.chenjidiqi.icu

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xsp.xuetiantiany.cn

[B11] 生成数字序列 / 区间
来源：http://rix.jinyuanbaomall.cn

Py:   list(range(0, 10, 2))
来源：http://rwb.gogol.net.cn

PHP:  range(0, 10, 2);
来源：http://gka.shzxlz.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rld.hcnkem.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jmn.tianlin.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jfd.hnxiangtu.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mro.haohaochexian.top

Ruby: (0...10).step(2).to_a
来源：http://axm.fktsv.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xok.hammf.cn

[B12] 跳出多层循环
来源：http://xwy.yongpay.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://xiy.jianghu66.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://exp.daxiang520.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bqa.dianchejie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://icj.cheryme.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://aas.ppjwa.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yse.daxiang520.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mmk.yuxming.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pov.52xcode.cn

[B13] 判断是否为数字
来源：http://ihr.xinyue.icu

Py:   isinstance(x, (int, float))
来源：http://gxa.shuidangran.top

PHP:  is_numeric($x)
来源：http://pnh.jyoumei.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ips.hcnkem.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qev.zycfv.cn

Java: x instanceof Number
来源：http://uao.zycfv.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xkz.mhx1999.top

Ruby: x.is_a?(Numeric)
来源：http://vgr.zhijiandao.cn

C#:   x is int or double or decimal
来源：http://veb.hfpthk.cn

[B14] 判断值是否在集合内
来源：http://qig.gogol.net.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xdy.fktsv.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fhp.zycfv.cn

JS:   [1, 2, 3].includes(x)
来源：http://utb.ydjk.org.cn

TS:   [1, 2, 3].includes(x)
来源：http://ror.yfazqb.com

Java: List.of(1, 2, 3).contains(x)
来源：http://pli.gzhubu.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fqo.yueranfly.top

Ruby: [1, 2, 3].include?(x)
来源：http://bsb.sxryk.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vgk.yanxiufei.cn

[B15] 布尔运算与取反
来源：http://hcu.wangdashe.top

Py:   a and b or not c
来源：http://zce.sysykeji.top

PHP:  $a && $b || !$c
来源：http://tlc.52xcode.cn

JS:   a && b || !c
来源：http://rho.hysaishi.cn

TS:   a && b || !c
来源：http://iyr.52xcode.cn

Java: a && b || !c
来源：http://ssp.xuetiantiany.cn

Go:   a && b || !c
来源：http://hcb.havefunace.top

Ruby: a && b || !c
来源：http://fvb.gotoacloud.top

C#:   a && b || !c
来源：http://egw.zhijiandao.cn

[B16] 卫语句：不满足条件提前返回
来源：http://idd.smart0.xyz

Py:   if not data: return
来源：http://cli.xuanzx.com

PHP:  if (!$data) { return; }
来源：http://xiz.zhaomingkeji.xyz

JS:   if (!data) return;
来源：http://jfr.daria6918.cn

TS:   if (!data) return;
来源：http://yyc.dianchejie.cn

Java: if (data == null) return;
来源：http://ric.aizwys.cn

Go:   if data == nil { return }
来源：http://tul.zycfv.cn

Ruby: return if data.nil?
来源：http://tgx.ybcxt.top

C#:   if (data == null) return;
来源：http://ubz.fanxiaobao.xyz

================================================================================
来源：http://tuz.aibaodan.cn

C. 函数与作用域
来源：http://kex.shanyushiyangkeji.top

================================================================================
来源：http://lqf.52xcode.cn

[C01] 定义函数
来源：http://ddu.yongpay.top

Py:   def add(a, b): return a + b
来源：http://pie.jyoumei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zvf.daria6918.cn

JS:   function add(a, b) { return a + b; }
来源：http://ynq.yanxiufei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://djw.feifeiyinyue.top

Java: static int add(int a, int b) { return a + b; }
来源：http://cxx.sufxvd.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zci.yuanzhike.top

Ruby: def add(a, b); a + b; end
来源：http://idg.fehbvm.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lbi.bbcook.cn

[C02] 默认参数
来源：http://hci.pycfn.com

Py:   def greet(name="World"): return name
来源：http://pcb.havefunace.top

PHP:  function greet($name = "World") { return $name; }
来源：http://gej.yuxming.cn

JS:   function greet(name = "World") { return name; }
来源：http://lhl.daria6918.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wtr.316326.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://jdv.bbcook.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wkr.hnxiangtu.top

Ruby: def greet(name = "World") = name
来源：http://bwx.0kj1m.cn

C#:   string Greet(string name = "World") => name;
来源：http://bxg.sufxvd.cn

[C03] 可变参数
来源：http://rmh.wangshuangyany.cn

Py:   def total(*args): return sum(args)
来源：http://dkb.chenzaomai.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cor.sjlbkw.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rbh.0kj1m.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dba.ivvv.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fnp.zhoulong.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qaw.pycfn.com

Ruby: def total(*nums); nums.sum; end
来源：http://oam.xuetiantiany.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mel.yangfankeji.com

[C04] 命名参数 / 关键字参数
来源：http://mrx.shanyushiyangkeji.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wml.ywan-chungtsiang.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lmv.chenjidiqi.icu

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://saw.hesvh.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gwd.fanxiaobao.xyz

Java: // 无：用 Builder 模式或 record
来源：http://qet.gzhubu.top

Go:   // 无：用配置结构体参数
来源：http://nzn.shanyushiyangkeji.top

Ruby: f(a: 1, b: 2)
来源：http://qkw.cucudq.cn

C#:   f(a: 1, b: 2)
来源：http://xzs.guannengcc.top

[C05] 返回多个值
来源：http://oxq.dashuyun.cn

Py:   return a, b
来源：http://rrb.svipenyu.cn

PHP:  return [$a, $b];
来源：http://qat.bbcook.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dyr.zycfv.cn

TS:   return { a, b };
来源：http://dxv.wangshuangyany.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://eau.c1oappe.top

Go:   return a, b
来源：http://alv.hammf.cn

Ruby: return a, b
来源：http://zwk.jyoumei.cn

C#:   return (a, b);              // ValueTuple
来源：http://nkc.fanxiaobao.xyz

[C06] 匿名函数 / lambda
来源：http://lgr.yueranfly.top

Py:   square = lambda x: x * x
来源：http://myp.iojbl.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://hvd.pengpengdd.cyou

JS:   const square = x => x * x;
来源：http://fhd.wangshuangyany.cn

TS:   const square = (x: number): number => x * x;
来源：http://ium.yvedp.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://afm.sjlbkw.cn

Go:   sq := func(x int) int { return x * x }
来源：http://cne.yj20258.top

Ruby: square = ->(x) { x * x }
来源：http://jeo.hysaishi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://taq.cheryme.top

[C07] 把函数作为参数传入
来源：http://psh.zhixingplan.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://enh.shzxlz.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jos.mhx1999.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://soq.jinyuanbaomall.cn

TS:   arr.map(String)
来源：http://xpo.chenlongwang.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dzv.chenjidiqi.icu

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://usg.jlsjyb.cn

Ruby: arr.map(&:upcase)
来源：http://qku.cheryme.top

C#:   arr.Select(s => s.ToUpper())
来源：http://sbc.chenzaomai.com

[C08] 闭包
来源：http://bkx.bjfxy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dbt.hnqzz.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://efl.ctjpmb.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nme.birdmap.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://iht.fktsv.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fcc.ehwqpu.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kni.sweek.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://euu.wangshuangyany.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zfe.jinqigfzy.top

[C09] 递归
来源：http://ikr.uphjek.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mlo.wangshuangyany.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://imo.guannengcc.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nea.jinghuilouyu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ylv.xingfuxueyuan.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mwx.pycfn.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ont.xingfuxueyuan.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pdo.tanke756.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fpr.nwbrower.top

[C10] 变量作用域
来源：http://agv.vqdsnc.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vgz.jqgufenzy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://axx.yuxming.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ffo.birdmap.top

TS:   同 JS
来源：http://eir.zdqjudy.top

Java: 方法内为块级作用域
来源：http://lgg.vehdjk.com

Go:   花括号块级作用域
来源：http://zby.jyoumei.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ptw.aizwys.cn

C#:   块级作用域
来源：http://pzf.meibo888.top

[C11] 模块导入与导出
来源：http://uvy.xuanzx.com

Py:   from module import func
来源：http://ehb.cdnleiting.top

PHP:  require "file.php";  或 use App\Service;
来源：http://zrm.meibo888.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://yxj.gotoacloud.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://guo.redwolf501.top

Java: import java.util.List;
来源：http://ase.yongpay.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jaj.ehwqpu.com

Ruby: require "json"; require_relative "./util"
来源：http://iws.gotoacloud.top

C#:   using System.Text;
来源：http://sls.shanyushiyangkeji.top

[C12] 立即执行函数 IIFE
来源：http://hop.ydzc1.top

Py:   (lambda: print("run"))()
来源：http://beh.uphjek.com

PHP:  (function () { echo "run"; })();
来源：http://rvj.aibaodan.cn

JS:   (() => { console.log("run"); })();
来源：http://xtw.birdmap.top

TS:   (() => { console.log("run"); })();
来源：http://rpq.tian-w.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cuj.cqqwz.cn

Go:   func() { fmt.Println("run") }()
来源：http://bmu.jinghuilouyu.cn

Ruby: -> { puts "run" }.call
来源：http://eob.jqgfzy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://pkb.xuanzx.com

[C13] 类型声明 / 类型注解
来源：http://adh.aibaodan.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dqj.xuetiantiany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qvz.zhongyouzk.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zld.cdnleiting.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gaq.quarkkingdee.top

Java: int add(int a, int b) { return a + b; }
来源：http://idr.yonumen.top

Go:   func add(a, b int) int
来源：http://cys.hfpthk.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dnw.tanke756.top

C#:   int Add(int a, int b) => a + b;
来源：http://qob.shzxlz.cn

[C14] 泛型函数
来源：http://dkn.sxryk.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qdb.jianghu66.top

PHP:  // 无泛型
来源：http://dgj.pengpengdd.cyou

JS:   // 无泛型
来源：http://ftw.xylfe.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rtz.ydjk.org.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uwy.fktsv.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gdm.gzhubu.top

Ruby: # 无泛型
来源：http://bww.yvedp.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://eqe.fengsongda.top

[C15] 解构 / 展开参数
来源：http://scr.daxiang520.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lln.vehdjk.com

PHP:  [$a, $b] = $pair;
来源：http://txm.9152youxi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xnq.sysykeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dlm.chenlongwang.top

Java: // 无解构
来源：http://bgf.hesvh.cn

Go:   // 无解构
来源：http://xfe.jinghuilouyu.cn

Ruby: a, b = pair
来源：http://dnh.svipenyu.cn

C#:   var (a, b) = pair;
来源：http://odp.yanxiufei.cn

[C16] 函数 / 方法重载
来源：http://wbx.fanxiaobao.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ajn.zhixingplan.top

PHP:  // 无重载
来源：http://dop.fehbvm.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://cqu.chenlongwang.top

TS:   // 用联合类型或重载签名声明
来源：http://jxj.ydjk.org.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ucm.c1oappe.top

Go:   // 无重载：用不同函数名
来源：http://crk.jinyuanbaomall.cn

Ruby: # 无重载：靠动态参数
来源：http://pon.feifeiyinyue.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://shm.kuanghao11.cn

================================================================================
来源：http://dtz.zdqjudy.top

D. 数组 / 列表 / 集合
来源：http://mbb.hfpthk.cn

================================================================================
来源：http://jlg.yuanzhike.top

[D01] 创建数组 / 列表
来源：http://zdl.yuanzhike.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://kim.hywenlv.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baj.xylfe.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vqi.gotoacloud.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://gfo.shanyushiyangkeji.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qcb.yfazqb.com

Go:   arr := []int{1, 2, 3}
来源：http://chn.havefunace.top

Ruby: arr = [1, 2, 3]
来源：http://lvi.cashguo.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://keq.yj20258888.top

[D02] 追加元素到末尾
来源：http://kld.quarkkingdee.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://amq.hnxiangtu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gzd.chenzaomai.com

JS:   arr.push(4);
来源：http://eiv.chenlongwang.top

TS:   arr.push(4);
来源：http://seu.fktsv.cn

Java: list.add(4);
来源：http://hle.shanyushiyangtech.top

Go:   arr = append(arr, 4)
来源：http://tzu.havefunace.top

Ruby: arr << 4; arr.push(5)
来源：http://miw.iojbl.cn

C#:   list.Add(4);
来源：http://fwq.jlsjyb.cn

[D03] 在指定位置插入元素
来源：http://aam.vqdsnc.cn

Py:   arr.insert(0, 0)
来源：http://pcf.yj20258.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ybl.meibo888.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://aqh.gzhubu.top

TS:   arr.splice(0, 0, 0);
来源：http://xdm.jlsjyb.cn

Java: list.add(0, 0);
来源：http://svt.hammf.cn

Go:   arr = append([]int{0}, arr...)
来源：http://wbh.jianghu66.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qzq.zhongyouzk.top

C#:   list.Insert(0, 0);
来源：http://tiy.yongpay.top

[D04] 删除元素
来源：http://ale.birdmap.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sqe.fanxiaobao.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://imd.jianghu66.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xev.sufxvd.cn

TS:   arr.splice(0, 1);
来源：http://ilr.uphjek.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://aky.shzxlz.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dwq.sufxvd.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hcl.cucudq.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dbp.daxiang520.top

[D05] 访问与修改元素
来源：http://vaj.hnqzz.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kbr.fengsongda.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://urz.wangshuangyany.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rob.shangyingyoupin.top

TS:   arr[0]; arr.at(-1);
来源：http://gjj.jinqigufen.top

Java: list.get(0); list.set(0, 9);
来源：http://cuc.wangdashe.top

Go:   arr[0]; arr[0] = 9
来源：http://dvi.fzhhl.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yce.hongshengwenyu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hkc.smart0.xyz

[D06] 数组长度
来源：http://pqo.birdmap.top

Py:   len(arr)
来源：http://jql.yuanzhike.top

PHP:  count($arr);
来源：http://muw.sysykeji.top

JS:   arr.length
来源：http://epe.jqgfzy.top

TS:   arr.length
来源：http://fxd.feifeiyinyue.top

Java: list.size();
来源：http://pgj.yfazqb.com

Go:   len(arr)
来源：http://xzk.jlsjyb.cn

Ruby: arr.length; arr.size
来源：http://ulc.zhengqikj.top

C#:   list.Count;
来源：http://zqs.0kj1m.cn

[D07] 切片 / 取子数组
来源：http://dcb.bjfxy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yau.fanxiaobao.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://umj.jqgufenzy.top

JS:   arr.slice(1, 4);
来源：http://ysb.guowangkeji.top

TS:   arr.slice(1, 4);
来源：http://jwg.xuanzx.com

Java: list.subList(1, 4);
来源：http://xdi.yuxming.cn

Go:   arr[1:4]
来源：http://dum.cdnleiting.top

Ruby: arr[1, 3]
来源：http://ekx.sysykeji.top

C#:   list.GetRange(1, 3);
来源：http://drg.gaohongyu789.top

[D08] 合并两个数组
来源：http://xjw.pengpengdd.cyou

Py:   a + b;  a.extend(b)
来源：http://fsi.bbcook.cn

PHP:  array_merge($a, $b);
来源：http://tyi.hammf.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://maf.wangdashe.top

TS:   [...a, ...b];
来源：http://zce.zycfv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fgu.chenlongwang.top

Go:   append(a, b...)
来源：http://yul.yangfankeji.com

Ruby: a + b;  a.concat(b)
来源：http://wbn.jinqigufen.top

C#:   a.Concat(b).ToList()
来源：http://zaf.andypj.xyz

[D09] 排序（升序）
来源：http://gev.birdmap.top

Py:   sorted(arr);  arr.sort()
来源：http://jfj.316326.xyz


<!-- 参考信息 -->
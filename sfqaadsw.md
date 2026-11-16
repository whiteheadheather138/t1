代发 wailian999

[B09] break 与 continue
来源：http://vws.zhixingplan.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rdf.shanyushiyangkeji.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://olj.dashuyun.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hsa.cashguo.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wpx.shangyingyoupin.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blu.hnxiangtu.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ziv.meibo888.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vlp.chenlongwang.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mgx.sxryk.cn

[B10] 遍历同时拿索引
来源：http://ohv.epnwcf.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tod.jqgufenzy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hko.ctjpmb.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://snu.redwolf501.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vsj.fktsv.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zbe.yanxiufei.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bkn.vehdjk.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yea.cqqwz.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qtt.nwbrower.top

[B11] 生成数字序列 / 区间
来源：http://dkv.xingfuxueyuan.xyz

Py:   list(range(0, 10, 2))
来源：http://dus.dashuyun.cn

PHP:  range(0, 10, 2);
来源：http://oih.tanke756.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tjo.xinyue.icu

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dbm.ctjpmb.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://spu.jinghuilouyu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dma.yuanzhike.top

Ruby: (0...10).step(2).to_a
来源：http://uwz.gotoacloud.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ffm.yj202588.top

[B12] 跳出多层循环
来源：http://ego.jiagoushi.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://cyf.hywenlv.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://nmf.snrcjt.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xpm.zhijiandao.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vgv.jinghuilouyu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wxl.ydjk.org.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xdq.yuanzhike.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ewz.xylfe.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jdv.vehdjk.com

[B13] 判断是否为数字
来源：http://fmb.gaohongyu789.top

Py:   isinstance(x, (int, float))
来源：http://uxh.xuetiantiany.cn

PHP:  is_numeric($x)
来源：http://dor.smart0.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cin.pengpengdd.cyou

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tue.chenzaomai.com

Java: x instanceof Number
来源：http://kir.snrcjt.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://snh.shzxlz.cn

Ruby: x.is_a?(Numeric)
来源：http://hit.zhijiandao.cn

C#:   x is int or double or decimal
来源：http://lxy.yueranfly.top

[B14] 判断值是否在集合内
来源：http://sri.ivvv.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zbj.yangfankeji.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tzf.ivvv.top

JS:   [1, 2, 3].includes(x)
来源：http://fdq.jinyuanbaomall.cn

TS:   [1, 2, 3].includes(x)
来源：http://ozj.yonumen.top

Java: List.of(1, 2, 3).contains(x)
来源：http://rrh.316326.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xox.daria6918.cn

Ruby: [1, 2, 3].include?(x)
来源：http://stu.nanxinkj.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gos.wangshuangyany.cn

[B15] 布尔运算与取反
来源：http://bnu.kuanghao11.cn

Py:   a and b or not c
来源：http://ipg.nwbrower.top

PHP:  $a && $b || !$c
来源：http://isr.aibaodan.cn

JS:   a && b || !c
来源：http://vby.nanxinkj.top

TS:   a && b || !c
来源：http://bxh.jinyuanbaomall.cn

Java: a && b || !c
来源：http://psy.wangdashe.top

Go:   a && b || !c
来源：http://fcc.gaohongyu789.top

Ruby: a && b || !c
来源：http://vul.hywenlv.cn

C#:   a && b || !c
来源：http://bgg.nwbrower.top

[B16] 卫语句：不满足条件提前返回
来源：http://yka.zhoulong.xyz

Py:   if not data: return
来源：http://jcx.sufxvd.cn

PHP:  if (!$data) { return; }
来源：http://bot.shzxlz.cn

JS:   if (!data) return;
来源：http://kwv.wangshuangyany.cn

TS:   if (!data) return;
来源：http://kcp.zhongyouzk.top

Java: if (data == null) return;
来源：http://vuo.ivvv.top

Go:   if data == nil { return }
来源：http://tbq.zhengqikj.top

Ruby: return if data.nil?
来源：http://ury.ydzc1.top

C#:   if (data == null) return;
来源：http://efn.iojbl.cn

================================================================================
来源：http://iap.ybcxt.top

C. 函数与作用域
来源：http://ghb.hnqzz.top

================================================================================
来源：http://zsz.bjfxy.top

[C01] 定义函数
来源：http://gpf.bbcook.cn

Py:   def add(a, b): return a + b
来源：http://bxv.pengpengdd.cyou

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mnv.yj20258888.top

JS:   function add(a, b) { return a + b; }
来源：http://evw.chenjidiqi.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://are.shzxlz.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fug.cdnleiting.top

Go:   func add(a, b int) int { return a + b }
来源：http://oeu.shanyushiyangtech.top

Ruby: def add(a, b); a + b; end
来源：http://agl.meibo888.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gay.ehwqpu.com

[C02] 默认参数
来源：http://tha.ehwqpu.com

Py:   def greet(name="World"): return name
来源：http://qro.gogol.net.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://jgj.epnwcf.com

JS:   function greet(name = "World") { return name; }
来源：http://dwa.fehbvm.com

TS:   function greet(name: string = "World") { return name; }
来源：http://nqr.c1oappe.top

Java: // 无默认参数：方法重载或 Optional
来源：http://jmc.xuetiantiany.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bun.cheryme.top

Ruby: def greet(name = "World") = name
来源：http://mkr.cdnleiting.top

C#:   string Greet(string name = "World") => name;
来源：http://ohr.zhongyouzk.top

[C03] 可变参数
来源：http://gzj.zhiwuduotai.top

Py:   def total(*args): return sum(args)
来源：http://qoj.pengpengdd.cyou

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://llr.ivvv.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://iwe.ybcxt.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://eiq.haohaochexian.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fbq.wangshuangyany.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dum.chenzaomai.com

Ruby: def total(*nums); nums.sum; end
来源：http://ote.ehwqpu.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vyw.sufxvd.cn

[C04] 命名参数 / 关键字参数
来源：http://ywk.gaohongyu789.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cvm.wangdashe.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://uuw.hnxiangtu.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://spg.sufxvd.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jst.yueranfly.top

Java: // 无：用 Builder 模式或 record
来源：http://guz.redwolf501.top

Go:   // 无：用配置结构体参数
来源：http://ntq.sweek.top

Ruby: f(a: 1, b: 2)
来源：http://xkk.yonumen.top

C#:   f(a: 1, b: 2)
来源：http://jqv.ywan-chungtsiang.top

[C05] 返回多个值
来源：http://tfx.haohaochexian.top

Py:   return a, b
来源：http://sql.fanxiaobao.xyz

PHP:  return [$a, $b];
来源：http://sdn.tian-w.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jwk.chenlongwang.top

TS:   return { a, b };
来源：http://zns.zhengqikj.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xpq.52xcode.cn

Go:   return a, b
来源：http://xrw.ehwqpu.com

Ruby: return a, b
来源：http://dwe.ehwqpu.com

C#:   return (a, b);              // ValueTuple
来源：http://ljs.jinqigufen.top

[C06] 匿名函数 / lambda
来源：http://oad.bbcook.cn

Py:   square = lambda x: x * x
来源：http://sje.ywan-chungtsiang.top

PHP:  $square = fn($x) => $x * $x;
来源：http://fgm.c1oappe.top

JS:   const square = x => x * x;
来源：http://gqx.ybcxt.top

TS:   const square = (x: number): number => x * x;
来源：http://mkz.zycfv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://olm.sufxvd.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qmo.ybcxt.top

Ruby: square = ->(x) { x * x }
来源：http://amm.hnqzz.top

C#:   Func<int, int> square = x => x * x;
来源：http://cxz.nanxuanxn.top

[C07] 把函数作为参数传入
来源：http://hqk.dianchejie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lcx.zdbjq.cn

PHP:  array_map("strtoupper", $arr);
来源：http://yfq.c1oappe.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://amp.ydjk.org.cn

TS:   arr.map(String)
来源：http://dpa.sjlbkw.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xte.gaohongyu789.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lvs.guannengcc.top

Ruby: arr.map(&:upcase)
来源：http://uel.zhengqikj.top

C#:   arr.Select(s => s.ToUpper())
来源：http://rbq.vehdjk.com

[C08] 闭包
来源：http://gyc.xylfe.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lxe.jlsjyb.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vkr.tanke756.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xzp.pengpengdd.cyou

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uqt.smart0.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nhk.sxryk.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kre.hammf.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kmv.hongshengwenyu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://afg.shanyushiyangtech.top

[C09] 递归
来源：http://pum.yj202588.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lwc.jqgufenzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://weu.hysaishi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qmu.snrcjt.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yyh.wangdashe.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nhi.zhaomingkeji.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://iac.jinyuanbaomall.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nvd.jyoumei.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pow.jinqigufen.top

[C10] 变量作用域
来源：http://mrx.zhijiandao.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://aqr.ivvv.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xpr.hywenlv.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jxd.zhengqikj.top

TS:   同 JS
来源：http://wwa.quarkkingdee.top

Java: 方法内为块级作用域
来源：http://trx.jqgufenzy.top

Go:   花括号块级作用域
来源：http://nbd.yonumen.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mhg.zhijiandao.cn

C#:   块级作用域
来源：http://xfn.chenlongwang.top

[C11] 模块导入与导出
来源：http://nbk.shuidangran.top

Py:   from module import func
来源：http://frb.quarkkingdee.top

PHP:  require "file.php";  或 use App\Service;
来源：http://udr.chenlongwang.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://jvh.hnxiangtu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mtm.sufxvd.cn

Java: import java.util.List;
来源：http://wvm.feifeiyinyue.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dya.yangfankeji.com

Ruby: require "json"; require_relative "./util"
来源：http://hcf.yanxiufei.cn

C#:   using System.Text;
来源：http://hwa.smart0.xyz

[C12] 立即执行函数 IIFE
来源：http://ubk.havefunace.top

Py:   (lambda: print("run"))()
来源：http://vyu.haohaochexian.top

PHP:  (function () { echo "run"; })();
来源：http://xfi.hfpthk.cn

JS:   (() => { console.log("run"); })();
来源：http://vhh.yvedp.cn

TS:   (() => { console.log("run"); })();
来源：http://wof.andypj.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://weh.guowangkeji.top

Go:   func() { fmt.Println("run") }()
来源：http://tow.jinqigfzy.top

Ruby: -> { puts "run" }.call
来源：http://hmf.jlsjyb.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://vos.ctjpmb.com

[C13] 类型声明 / 类型注解
来源：http://hgv.zhengqikj.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://eph.jianghu66.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://osb.hnqzz.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ppa.zhengqikj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gux.pycfn.com

Java: int add(int a, int b) { return a + b; }
来源：http://mqm.yj202588.top

Go:   func add(a, b int) int
来源：http://hei.cdnleiting.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tzi.daria6918.cn

C#:   int Add(int a, int b) => a + b;
来源：http://hld.hnxiangtu.top

[C14] 泛型函数
来源：http://qfw.yueranfly.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://aob.svipenyu.cn

PHP:  // 无泛型
来源：http://gsh.yuanzhike.top

JS:   // 无泛型
来源：http://ats.jqgfzy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://owz.tianlin.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://oii.sysykeji.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tob.ppjwa.cn

Ruby: # 无泛型
来源：http://sen.andypj.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://juh.fanxiaobao.xyz

[C15] 解构 / 展开参数
来源：http://zsr.pycfn.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jhk.andypj.xyz

PHP:  [$a, $b] = $pair;
来源：http://wfo.hfpthk.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kbc.ppjwa.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vgt.316326.xyz

Java: // 无解构
来源：http://dot.cucudq.cn

Go:   // 无解构
来源：http://fro.pycfn.com

Ruby: a, b = pair
来源：http://ykp.zhongyouzk.top

C#:   var (a, b) = pair;
来源：http://nfc.jlsjyb.cn

[C16] 函数 / 方法重载
来源：http://qnl.xziqi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ksw.0kj1m.cn

PHP:  // 无重载
来源：http://gky.yuanzhike.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://orv.fanxiaobao.xyz

TS:   // 用联合类型或重载签名声明
来源：http://meg.shuidangran.top

Java: void f(int a) {}  void f(String a) {}
来源：http://khl.xziqi.cn

Go:   // 无重载：用不同函数名
来源：http://nkh.fzhhl.top

Ruby: # 无重载：靠动态参数
来源：http://vli.shangyingyoupin.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://xtd.smart0.xyz

================================================================================
来源：http://chw.jqgufenzy.top

D. 数组 / 列表 / 集合
来源：http://gvh.zycfv.cn

================================================================================
来源：http://fyu.sjlbkw.cn

[D01] 创建数组 / 列表
来源：http://lql.feifeiyinyue.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://poh.jianghu66.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rlq.wangshuangyany.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://med.shuidangran.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://wcz.aizwys.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sop.sxryk.cn

Go:   arr := []int{1, 2, 3}
来源：http://jdo.mhx1999.top

Ruby: arr = [1, 2, 3]
来源：http://vge.jyoumei.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zjo.gaohongyu789.top

[D02] 追加元素到末尾
来源：http://wgh.vehdjk.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yac.fktsv.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xbt.gotoacloud.top

JS:   arr.push(4);
来源：http://dbo.daxiang520.top

TS:   arr.push(4);
来源：http://tzd.yueranfly.top

Java: list.add(4);
来源：http://yxi.yj20258888.top

Go:   arr = append(arr, 4)
来源：http://yho.shzxlz.cn

Ruby: arr << 4; arr.push(5)
来源：http://ooh.jinyuanbaomall.cn

C#:   list.Add(4);
来源：http://psv.vqdsnc.cn

[D03] 在指定位置插入元素
来源：http://sfd.daria6918.cn

Py:   arr.insert(0, 0)
来源：http://wyz.vqdsnc.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zxm.jinqigfzy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bph.jyoumei.cn

TS:   arr.splice(0, 0, 0);
来源：http://jpo.wangshuangyany.cn

Java: list.add(0, 0);
来源：http://utk.yfazqb.com

Go:   arr = append([]int{0}, arr...)
来源：http://wtb.redwolf501.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xfv.fktsv.cn

C#:   list.Insert(0, 0);
来源：http://qpy.cucudq.cn

[D04] 删除元素
来源：http://cuy.fanxiaobao.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tda.nanxuanxn.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sht.smart0.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pld.yanxiufei.cn

TS:   arr.splice(0, 1);
来源：http://tdz.cqqwz.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jeu.tian-w.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fpv.bbcook.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ker.zhaomingkeji.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qpo.yongpay.top

[D05] 访问与修改元素
来源：http://wdy.yj20258888.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nfo.yongpay.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cip.shuidangran.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tnh.hammf.cn

TS:   arr[0]; arr.at(-1);
来源：http://dvr.cheryme.top

Java: list.get(0); list.set(0, 9);
来源：http://clv.shuidangran.top

Go:   arr[0]; arr[0] = 9
来源：http://sqe.yvedp.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xhd.jyoumei.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ami.sweek.top

[D06] 数组长度
来源：http://onq.cheryme.top

Py:   len(arr)
来源：http://aus.cucudq.cn

PHP:  count($arr);
来源：http://ula.nanxinkj.top

JS:   arr.length
来源：http://fcs.daxiang520.top

TS:   arr.length
来源：http://hqt.epnwcf.com

Java: list.size();
来源：http://fun.shanyushiyangkeji.top

Go:   len(arr)
来源：http://xkm.nwbrower.top

Ruby: arr.length; arr.size
来源：http://oup.guannengcc.top

C#:   list.Count;
来源：http://poo.xuanzx.com

[D07] 切片 / 取子数组
来源：http://bun.ctjpmb.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jbk.tian-w.cn

PHP:  array_slice($arr, 1, 3);
来源：http://lks.wangshuangyany.cn

JS:   arr.slice(1, 4);
来源：http://lzi.yueranfly.top

TS:   arr.slice(1, 4);
来源：http://xtv.sweek.top

Java: list.subList(1, 4);
来源：http://htm.feifeiyinyue.top

Go:   arr[1:4]
来源：http://acy.nanxinkj.top

Ruby: arr[1, 3]
来源：http://vxi.epnwcf.com

C#:   list.GetRange(1, 3);
来源：http://bzi.guowangkeji.top

[D08] 合并两个数组
来源：http://jmv.daxiang520.top

Py:   a + b;  a.extend(b)
来源：http://sou.cucudq.cn

PHP:  array_merge($a, $b);
来源：http://ylp.jlsjyb.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://moe.fzhhl.top

TS:   [...a, ...b];
来源：http://ayk.jqgfzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://epr.quarkkingdee.top

Go:   append(a, b...)
来源：http://uex.jinqigufen.top

Ruby: a + b;  a.concat(b)
来源：http://jni.ppjwa.cn

C#:   a.Concat(b).ToList()
来源：http://urg.nanxinkj.top

[D09] 排序（升序）
来源：http://smb.fengsongda.top

Py:   sorted(arr);  arr.sort()
来源：http://vxe.zhiwuduotai.top

PHP:  sort($arr);
来源：http://jng.andypj.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://knq.tian-w.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tdt.cqqwz.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hby.wangshuangyany.cn


<!-- 参考信息 -->
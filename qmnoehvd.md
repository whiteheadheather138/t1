代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://znx.yfazqb.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zkn.yanxiufei.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ftk.bbcook.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zev.cucudq.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yoh.9152youxi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://atz.epnwcf.com

[B11] 生成数字序列 / 区间
来源：http://rbr.zycfv.cn

Py:   list(range(0, 10, 2))
来源：http://sxr.hfpthk.cn

PHP:  range(0, 10, 2);
来源：http://svg.sufxvd.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://obv.yuanzhike.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qsq.tian-w.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ilj.hcnkem.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rxw.zhiwuduotai.top

Ruby: (0...10).step(2).to_a
来源：http://kty.yuxming.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hqp.tanke756.top

[B12] 跳出多层循环
来源：http://rah.tian-w.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://daf.epnwcf.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://zbm.feifeiyinyue.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jha.uphjek.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qgb.yongpay.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zct.snrcjt.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hpt.0kj1m.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jyq.tian-w.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nha.sjlbkw.cn

[B13] 判断是否为数字
来源：http://cji.redwolf501.top

Py:   isinstance(x, (int, float))
来源：http://jpq.jqgufenzy.top

PHP:  is_numeric($x)
来源：http://xww.zycfv.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lnf.xingfuxueyuan.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ygt.yongpay.top

Java: x instanceof Number
来源：http://gif.vqdsnc.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gyz.sufxvd.cn

Ruby: x.is_a?(Numeric)
来源：http://fea.shanyushiyangkeji.top

C#:   x is int or double or decimal
来源：http://xtp.ctjpmb.com

[B14] 判断值是否在集合内
来源：http://fkj.ivvv.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fgj.shanyushiyangkeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nxb.yuxming.cn

JS:   [1, 2, 3].includes(x)
来源：http://qvr.jqgufenzy.top

TS:   [1, 2, 3].includes(x)
来源：http://laf.tarul.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ojp.snrcjt.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ckm.52xcode.cn

Ruby: [1, 2, 3].include?(x)
来源：http://fmh.jiagoushi.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ydc.ydjk.org.cn

[B15] 布尔运算与取反
来源：http://kyj.zhixingplan.top

Py:   a and b or not c
来源：http://lvt.zhengqikj.top

PHP:  $a && $b || !$c
来源：http://qex.jinqigufen.top

JS:   a && b || !c
来源：http://npl.nanxinkj.top

TS:   a && b || !c
来源：http://ieq.yongpay.top

Java: a && b || !c
来源：http://qxp.hfpthk.cn

Go:   a && b || !c
来源：http://meo.cucudq.cn

Ruby: a && b || !c
来源：http://yrb.sweek.top

C#:   a && b || !c
来源：http://nmh.andypj.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://ggw.vehdjk.com

Py:   if not data: return
来源：http://jso.yj20258888.top

PHP:  if (!$data) { return; }
来源：http://vcd.hnqzz.top

JS:   if (!data) return;
来源：http://hyp.jinqigufen.top

TS:   if (!data) return;
来源：http://rtu.cucudq.cn

Java: if (data == null) return;
来源：http://qvr.hywenlv.cn

Go:   if data == nil { return }
来源：http://xyk.jinghuilouyu.cn

Ruby: return if data.nil?
来源：http://duy.epnwcf.com

C#:   if (data == null) return;
来源：http://cxt.snrcjt.cn

================================================================================
来源：http://vuw.andypj.xyz

C. 函数与作用域
来源：http://djq.shanyushiyangkeji.top

================================================================================
来源：http://vag.epnwcf.com

[C01] 定义函数
来源：http://tcb.sxryk.cn

Py:   def add(a, b): return a + b
来源：http://eju.svipenyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://slr.pycfn.com

JS:   function add(a, b) { return a + b; }
来源：http://llr.vqdsnc.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jvi.tian-w.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://isi.zhoulong.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://uzx.zhoulong.xyz

Ruby: def add(a, b); a + b; end
来源：http://epb.gotoacloud.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hkp.cqqwz.cn

[C02] 默认参数
来源：http://drl.tianlin.xyz

Py:   def greet(name="World"): return name
来源：http://mrh.jinqigfzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://gqg.aibaodan.cn

JS:   function greet(name = "World") { return name; }
来源：http://ujo.xylfe.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://sko.xinyue.icu

Java: // 无默认参数：方法重载或 Optional
来源：http://ufq.cdnleiting.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vqt.feifeiyinyue.top

Ruby: def greet(name = "World") = name
来源：http://nac.cheryme.top

C#:   string Greet(string name = "World") => name;
来源：http://jcu.vehdjk.com

[C03] 可变参数
来源：http://xss.hammf.cn

Py:   def total(*args): return sum(args)
来源：http://zev.feifeiyinyue.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dyr.0kj1m.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kbt.bjfxy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rjp.uphjek.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pce.hcnkem.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gwu.zhixingplan.top

Ruby: def total(*nums); nums.sum; end
来源：http://evi.aizwys.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tkt.9152youxi.cn

[C04] 命名参数 / 关键字参数
来源：http://dbx.nwbrower.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cic.jinqigfzy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://inr.yuanzhike.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bkf.chenjidiqi.icu

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://czp.nwbrower.top

Java: // 无：用 Builder 模式或 record
来源：http://gdl.ywan-chungtsiang.top

Go:   // 无：用配置结构体参数
来源：http://cvl.shangyingyoupin.top

Ruby: f(a: 1, b: 2)
来源：http://uyp.yuxming.cn

C#:   f(a: 1, b: 2)
来源：http://hzv.meibo888.top

[C05] 返回多个值
来源：http://byx.hammf.cn

Py:   return a, b
来源：http://jck.aibaodan.cn

PHP:  return [$a, $b];
来源：http://iqp.gogol.net.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jex.bbcook.cn

TS:   return { a, b };
来源：http://gka.chenjidiqi.icu

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jcs.cucudq.cn

Go:   return a, b
来源：http://hpr.zdbjq.cn

Ruby: return a, b
来源：http://oyo.gotoacloud.top

C#:   return (a, b);              // ValueTuple
来源：http://edf.sweek.top

[C06] 匿名函数 / lambda
来源：http://yhf.cucudq.cn

Py:   square = lambda x: x * x
来源：http://uey.gotoacloud.top

PHP:  $square = fn($x) => $x * $x;
来源：http://raj.yj20258.top

JS:   const square = x => x * x;
来源：http://ihl.fktsv.cn

TS:   const square = (x: number): number => x * x;
来源：http://qmu.chenzaomai.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pfs.cdnleiting.top

Go:   sq := func(x int) int { return x * x }
来源：http://bun.ydzc1.top

Ruby: square = ->(x) { x * x }
来源：http://vty.yvedp.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ciu.zhoulong.xyz

[C07] 把函数作为参数传入
来源：http://cpn.52xcode.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qde.pengpengdd.cyou

PHP:  array_map("strtoupper", $arr);
来源：http://ztt.svipenyu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://krc.ywan-chungtsiang.top

TS:   arr.map(String)
来源：http://mxn.shanyushiyangkeji.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tgv.birdmap.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uus.aizwys.cn

Ruby: arr.map(&:upcase)
来源：http://dal.chenlongwang.top

C#:   arr.Select(s => s.ToUpper())
来源：http://niw.tianlin.xyz

[C08] 闭包
来源：http://idn.ctjpmb.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ugg.hnxiangtu.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xmz.jinghuilouyu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mfa.feifeiyinyue.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pap.tian-w.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nac.gotoacloud.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xpa.xuetiantiany.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://icb.hfpthk.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pkf.zhijiandao.cn

[C09] 递归
来源：http://vyv.9152youxi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lts.316326.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://flf.vqdsnc.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kzd.fehbvm.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qnl.shanyushiyangkeji.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://eao.jlsjyb.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nng.gotoacloud.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wlv.jinghuilouyu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cql.xziqi.cn

[C10] 变量作用域
来源：http://cpd.zdbjq.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nkw.xinyue.icu

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ehe.epnwcf.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mvm.fktsv.cn

TS:   同 JS
来源：http://vum.jinqigufen.top

Java: 方法内为块级作用域
来源：http://yje.sxryk.cn

Go:   花括号块级作用域
来源：http://axy.gaohongyu789.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xot.nwbrower.top

C#:   块级作用域
来源：http://odq.ivvv.top

[C11] 模块导入与导出
来源：http://cdi.ywan-chungtsiang.top

Py:   from module import func
来源：http://qdx.hnxiangtu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://mjx.jiagoushi.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://eje.gzhubu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://icz.9152youxi.cn

Java: import java.util.List;
来源：http://ktf.gogol.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lcw.fanxiaobao.xyz

Ruby: require "json"; require_relative "./util"
来源：http://voj.xinyue.icu

C#:   using System.Text;
来源：http://szd.sysykeji.top

[C12] 立即执行函数 IIFE
来源：http://hdi.nanxinkj.top

Py:   (lambda: print("run"))()
来源：http://aac.52xcode.cn

PHP:  (function () { echo "run"; })();
来源：http://wsc.bbcook.cn

JS:   (() => { console.log("run"); })();
来源：http://jce.ydzc1.top

TS:   (() => { console.log("run"); })();
来源：http://stx.gaohongyu789.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://btt.yuanzhike.top

Go:   func() { fmt.Println("run") }()
来源：http://fcb.daxiang520.top

Ruby: -> { puts "run" }.call
来源：http://mxi.uphjek.com

C#:   // 无 IIFE：用静态构造函数
来源：http://trt.shangyingyoupin.top

[C13] 类型声明 / 类型注解
来源：http://bdo.sysykeji.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rli.jyoumei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://miu.cashguo.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yha.dianchejie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bxa.xuetiantiany.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xch.zhixingplan.top

Go:   func add(a, b int) int
来源：http://ckn.snrcjt.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dbg.hywenlv.cn

C#:   int Add(int a, int b) => a + b;
来源：http://brv.gzhubu.top

[C14] 泛型函数
来源：http://ohd.meibo888.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cfb.iojbl.cn

PHP:  // 无泛型
来源：http://tks.c1oappe.top

JS:   // 无泛型
来源：http://lkn.316326.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://saq.sweek.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lej.ivvv.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xii.yanxiufei.cn

Ruby: # 无泛型
来源：http://obw.shangyingyoupin.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qem.jqgufenzy.top

[C15] 解构 / 展开参数
来源：http://ldx.meibo888.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gwu.aibaodan.cn

PHP:  [$a, $b] = $pair;
来源：http://snk.gotoacloud.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vsz.shanyushiyangtech.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://leb.zycfv.cn

Java: // 无解构
来源：http://dwm.uphjek.com

Go:   // 无解构
来源：http://kaj.xingfuxueyuan.xyz

Ruby: a, b = pair
来源：http://zyb.jinyuanbaomall.cn

C#:   var (a, b) = pair;
来源：http://vfw.meibo888.top

[C16] 函数 / 方法重载
来源：http://yrj.pycfn.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fcu.kuanghao11.cn

PHP:  // 无重载
来源：http://zde.shangyingyoupin.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://iha.yangfankeji.com

TS:   // 用联合类型或重载签名声明
来源：http://jqy.zhaomingkeji.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://nlq.jqgfzy.top

Go:   // 无重载：用不同函数名
来源：http://kia.fktsv.cn

Ruby: # 无重载：靠动态参数
来源：http://tsu.bbcook.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://gca.mhx1999.top

================================================================================
来源：http://evz.fehbvm.com

D. 数组 / 列表 / 集合
来源：http://zse.tanke756.top

================================================================================
来源：http://qte.vqdsnc.cn

[D01] 创建数组 / 列表
来源：http://tif.dashuyun.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://nbo.wangdashe.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://iio.zhixingplan.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://opv.zhengqikj.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://fdp.0kj1m.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bpx.yfazqb.com

Go:   arr := []int{1, 2, 3}
来源：http://gjm.iojbl.cn

Ruby: arr = [1, 2, 3]
来源：http://xis.316326.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cjm.hongshengwenyu.top

[D02] 追加元素到末尾
来源：http://cav.ehwqpu.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hrp.yongpay.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pxj.andypj.xyz

JS:   arr.push(4);
来源：http://llx.ivvv.top

TS:   arr.push(4);
来源：http://qen.sysykeji.top

Java: list.add(4);
来源：http://dlg.sweek.top

Go:   arr = append(arr, 4)
来源：http://ych.aibaodan.cn

Ruby: arr << 4; arr.push(5)
来源：http://ipa.ivvv.top

C#:   list.Add(4);
来源：http://enj.yvedp.cn

[D03] 在指定位置插入元素
来源：http://opf.sufxvd.cn

Py:   arr.insert(0, 0)
来源：http://vkw.fehbvm.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rkx.tarul.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://atn.yueranfly.top

TS:   arr.splice(0, 0, 0);
来源：http://yqg.shanyushiyangkeji.top

Java: list.add(0, 0);
来源：http://nmp.xziqi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xzm.hfpthk.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kvd.jinqigufen.top

C#:   list.Insert(0, 0);
来源：http://nut.daria6918.cn

[D04] 删除元素
来源：http://irf.snrcjt.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cha.yj20258888.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blu.jinyuanbaomall.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kpn.yuxming.cn

TS:   arr.splice(0, 1);
来源：http://sqp.yangfankeji.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bwu.ydjk.org.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yvy.cheryme.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uai.ywan-chungtsiang.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kru.zdqjudy.top

[D05] 访问与修改元素
来源：http://lpy.hnqzz.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ciz.sufxvd.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zla.uphjek.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ieu.yonumen.top

TS:   arr[0]; arr.at(-1);
来源：http://vxy.daxiang520.top

Java: list.get(0); list.set(0, 9);
来源：http://aay.zdbjq.cn

Go:   arr[0]; arr[0] = 9
来源：http://mni.52xcode.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://eja.yj20258.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qmt.ivvv.top

[D06] 数组长度
来源：http://zxa.bjfxy.top

Py:   len(arr)
来源：http://sfz.quarkkingdee.top

PHP:  count($arr);
来源：http://dit.ybcxt.top

JS:   arr.length
来源：http://mtz.sxryk.cn

TS:   arr.length
来源：http://avz.cheryme.top

Java: list.size();
来源：http://hro.jinghuilouyu.cn

Go:   len(arr)
来源：http://ufa.snrcjt.cn

Ruby: arr.length; arr.size
来源：http://gjj.meibo888.top

C#:   list.Count;
来源：http://gqc.hysaishi.cn

[D07] 切片 / 取子数组
来源：http://wns.haohaochexian.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ccm.hongshengwenyu.top

PHP:  array_slice($arr, 1, 3);
来源：http://cyv.yuanzhike.top

JS:   arr.slice(1, 4);
来源：http://itk.meibo888.top

TS:   arr.slice(1, 4);
来源：http://utl.hnqzz.top

Java: list.subList(1, 4);
来源：http://eik.jqgufenzy.top

Go:   arr[1:4]
来源：http://cun.haohaochexian.top

Ruby: arr[1, 3]
来源：http://fqc.cheryme.top

C#:   list.GetRange(1, 3);
来源：http://zkl.nanxuanxn.top

[D08] 合并两个数组
来源：http://ixz.daxiang520.top

Py:   a + b;  a.extend(b)
来源：http://ezu.zhixingplan.top

PHP:  array_merge($a, $b);
来源：http://vac.haohaochexian.top

JS:   [...a, ...b];  a.concat(b);
来源：http://mbs.yj20258.top

TS:   [...a, ...b];
来源：http://cdc.yj202588.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://smx.guowangkeji.top

Go:   append(a, b...)
来源：http://mlh.ydzc1.top

Ruby: a + b;  a.concat(b)
来源：http://qvs.redwolf501.top

C#:   a.Concat(b).ToList()
来源：http://ocl.316326.xyz

[D09] 排序（升序）
来源：http://dcg.sweek.top

Py:   sorted(arr);  arr.sort()
来源：http://yxh.yonumen.top

PHP:  sort($arr);
来源：http://xca.yuxming.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ohj.svipenyu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://peb.yongpay.top

Java: Collections.sort(list);  list.sort(null);
来源：http://vcc.hysaishi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cat.xziqi.cn

Ruby: arr.sort
来源：http://gdx.zhijiandao.cn

C#:   list.Sort();
来源：http://zbr.pengpengdd.cyou

[D10] 自定义排序（按字段 / 多条件）
来源：http://xxn.bbcook.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://orv.gogol.net.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jzn.9152youxi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pdi.hongshengwenyu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ent.feifeiyinyue.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vlg.andypj.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rmw.ppjwa.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dma.sjlbkw.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://htw.zhijiandao.cn


<!-- 参考信息 -->
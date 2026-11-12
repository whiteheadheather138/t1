代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lsg.guannengcc.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kgf.zdbjq.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xjo.dashuyun.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tcf.ydzc1.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lta.zhongyouzk.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://buk.sjlbkw.cn

[B11] 生成数字序列 / 区间
来源：http://jdq.pengpengdd.cyou

Py:   list(range(0, 10, 2))
来源：http://dhk.tanke756.top

PHP:  range(0, 10, 2);
来源：http://obe.tanke756.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://crm.pengpengdd.cyou

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uak.316326.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://okv.yj202588.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://met.gaohongyu789.top

Ruby: (0...10).step(2).to_a
来源：http://cgn.cheryme.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mtr.hnqzz.top

[B12] 跳出多层循环
来源：http://zyw.jinyuanbaomall.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wae.nanxinkj.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://myp.mhx1999.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rxy.cqqwz.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://khe.nanxinkj.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hsi.gzhubu.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gcf.svipenyu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hjh.yj20258.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qrb.xingfuxueyuan.xyz

[B13] 判断是否为数字
来源：http://yve.hywenlv.cn

Py:   isinstance(x, (int, float))
来源：http://sbv.yangfankeji.com

PHP:  is_numeric($x)
来源：http://yqg.quarkkingdee.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zzo.redwolf501.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://egd.feifeiyinyue.top

Java: x instanceof Number
来源：http://ldh.jinghuilouyu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pay.zhengqikj.top

Ruby: x.is_a?(Numeric)
来源：http://wbt.zhixingplan.top

C#:   x is int or double or decimal
来源：http://hhy.meibo888.top

[B14] 判断值是否在集合内
来源：http://ezk.xuanzx.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hjk.fzhhl.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wqc.cheryme.top

JS:   [1, 2, 3].includes(x)
来源：http://prf.chenlongwang.top

TS:   [1, 2, 3].includes(x)
来源：http://mpm.shanyushiyangkeji.top

Java: List.of(1, 2, 3).contains(x)
来源：http://gsf.chenlongwang.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hso.jlsjyb.cn

Ruby: [1, 2, 3].include?(x)
来源：http://piu.jyoumei.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fjf.jinyuanbaomall.cn

[B15] 布尔运算与取反
来源：http://bbx.fzhhl.top

Py:   a and b or not c
来源：http://iea.vqdsnc.cn

PHP:  $a && $b || !$c
来源：http://gcz.yonumen.top

JS:   a && b || !c
来源：http://kph.ehwqpu.com

TS:   a && b || !c
来源：http://sfz.zhengqikj.top

Java: a && b || !c
来源：http://ujn.chenzaomai.com

Go:   a && b || !c
来源：http://jhq.cqqwz.cn

Ruby: a && b || !c
来源：http://fvz.ywan-chungtsiang.top

C#:   a && b || !c
来源：http://qrj.gzhubu.top

[B16] 卫语句：不满足条件提前返回
来源：http://uxz.smart0.xyz

Py:   if not data: return
来源：http://mcr.vehdjk.com

PHP:  if (!$data) { return; }
来源：http://gzx.chenjidiqi.icu

JS:   if (!data) return;
来源：http://qyu.jinyuanbaomall.cn

TS:   if (!data) return;
来源：http://bvx.zycfv.cn

Java: if (data == null) return;
来源：http://ixp.ppjwa.cn

Go:   if data == nil { return }
来源：http://ayc.gogol.net.cn

Ruby: return if data.nil?
来源：http://lmw.yonumen.top

C#:   if (data == null) return;
来源：http://aqy.jinqigufen.top

================================================================================
来源：http://dym.meibo888.top

C. 函数与作用域
来源：http://uzm.fengsongda.top

================================================================================
来源：http://vzn.yueranfly.top

[C01] 定义函数
来源：http://kft.pengpengdd.cyou

Py:   def add(a, b): return a + b
来源：http://kui.0kj1m.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ths.fktsv.cn

JS:   function add(a, b) { return a + b; }
来源：http://uzf.zhoulong.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://seq.sjlbkw.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://exr.hesvh.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jfb.snrcjt.cn

Ruby: def add(a, b); a + b; end
来源：http://qiq.jinqigufen.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ohs.jianghu66.top

[C02] 默认参数
来源：http://khe.hfpthk.cn

Py:   def greet(name="World"): return name
来源：http://odh.hfpthk.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xue.gzhubu.top

JS:   function greet(name = "World") { return name; }
来源：http://lbl.fzhhl.top

TS:   function greet(name: string = "World") { return name; }
来源：http://nky.guowangkeji.top

Java: // 无默认参数：方法重载或 Optional
来源：http://bmr.nanxinkj.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gfa.bjfxy.top

Ruby: def greet(name = "World") = name
来源：http://mov.jinqigfzy.top

C#:   string Greet(string name = "World") => name;
来源：http://zsg.yj20258888.top

[C03] 可变参数
来源：http://aod.quarkkingdee.top

Py:   def total(*args): return sum(args)
来源：http://pnf.cashguo.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blo.ydzc1.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://otf.ivvv.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ped.meibo888.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lds.yanxiufei.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fhq.yj202588.top

Ruby: def total(*nums); nums.sum; end
来源：http://pem.cheryme.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qjy.snrcjt.cn

[C04] 命名参数 / 关键字参数
来源：http://zgn.ywan-chungtsiang.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://oal.mhx1999.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gpq.ydzc1.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://koj.zhixingplan.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://voc.yonumen.top

Java: // 无：用 Builder 模式或 record
来源：http://tqe.yvedp.cn

Go:   // 无：用配置结构体参数
来源：http://jxg.fzhhl.top

Ruby: f(a: 1, b: 2)
来源：http://hft.jinqigfzy.top

C#:   f(a: 1, b: 2)
来源：http://mkj.sjlbkw.cn

[C05] 返回多个值
来源：http://oqu.zycfv.cn

Py:   return a, b
来源：http://zlb.xziqi.cn

PHP:  return [$a, $b];
来源：http://thi.gogol.net.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zui.zhengqikj.top

TS:   return { a, b };
来源：http://jwr.jqgfzy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hyo.jlsjyb.cn

Go:   return a, b
来源：http://quq.wangdashe.top

Ruby: return a, b
来源：http://xks.xylfe.cn

C#:   return (a, b);              // ValueTuple
来源：http://kcy.yj20258.top

[C06] 匿名函数 / lambda
来源：http://ozr.yj202588.top

Py:   square = lambda x: x * x
来源：http://dpn.shanyushiyangkeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://hco.vqdsnc.cn

JS:   const square = x => x * x;
来源：http://igi.fzhhl.top

TS:   const square = (x: number): number => x * x;
来源：http://cxr.epnwcf.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ewg.mhx1999.top

Go:   sq := func(x int) int { return x * x }
来源：http://eob.yfazqb.com

Ruby: square = ->(x) { x * x }
来源：http://uor.hfpthk.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zlm.fengsongda.top

[C07] 把函数作为参数传入
来源：http://act.dianchejie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xxl.quarkkingdee.top

PHP:  array_map("strtoupper", $arr);
来源：http://egm.tanke756.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wrp.xziqi.cn

TS:   arr.map(String)
来源：http://rir.zhoulong.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bbl.epnwcf.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jgp.jinghuilouyu.cn

Ruby: arr.map(&:upcase)
来源：http://dnu.uphjek.com

C#:   arr.Select(s => s.ToUpper())
来源：http://uvz.daria6918.cn

[C08] 闭包
来源：http://sps.zycfv.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yut.xylfe.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tpc.jqgfzy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fpn.quarkkingdee.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dxg.zdqjudy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pfz.guowangkeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cbr.yj20258888.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://phn.haohaochexian.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dtr.shanyushiyangtech.top

[C09] 递归
来源：http://jsv.ydzc1.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fir.ppjwa.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://aym.jqgfzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gad.sxryk.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qqz.52xcode.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tkr.dianchejie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://htf.daria6918.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ohh.vqdsnc.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vzf.ybcxt.top

[C10] 变量作用域
来源：http://ixf.mhx1999.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wdh.gotoacloud.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kas.yfazqb.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nse.jiagoushi.top

TS:   同 JS
来源：http://yzb.cucudq.cn

Java: 方法内为块级作用域
来源：http://yko.xylfe.cn

Go:   花括号块级作用域
来源：http://xhw.sxryk.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pid.hnqzz.top

C#:   块级作用域
来源：http://cmy.dianchejie.cn

[C11] 模块导入与导出
来源：http://xrp.pycfn.com

Py:   from module import func
来源：http://jbt.zhixingplan.top

PHP:  require "file.php";  或 use App\Service;
来源：http://hzm.nanxinkj.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://brn.sjlbkw.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://omc.c1oappe.top

Java: import java.util.List;
来源：http://tvx.ivvv.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://aos.fehbvm.com

Ruby: require "json"; require_relative "./util"
来源：http://vap.gzhubu.top

C#:   using System.Text;
来源：http://zmc.daxiang520.top

[C12] 立即执行函数 IIFE
来源：http://bfr.hammf.cn

Py:   (lambda: print("run"))()
来源：http://oon.hnqzz.top

PHP:  (function () { echo "run"; })();
来源：http://umj.daxiang520.top

JS:   (() => { console.log("run"); })();
来源：http://akv.vehdjk.com

TS:   (() => { console.log("run"); })();
来源：http://cka.wangshuangyany.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yym.jiagoushi.top

Go:   func() { fmt.Println("run") }()
来源：http://dlc.havefunace.top

Ruby: -> { puts "run" }.call
来源：http://dkd.zycfv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ugl.havefunace.top

[C13] 类型声明 / 类型注解
来源：http://qkh.bbcook.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pld.xuetiantiany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://osx.hcnkem.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ufn.dashuyun.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gqu.yueranfly.top

Java: int add(int a, int b) { return a + b; }
来源：http://qzi.shanyushiyangkeji.top

Go:   func add(a, b int) int
来源：http://ydr.ybcxt.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dtz.bjfxy.top

C#:   int Add(int a, int b) => a + b;
来源：http://jbo.yj20258.top

[C14] 泛型函数
来源：http://kyt.pengpengdd.cyou

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wcg.smart0.xyz

PHP:  // 无泛型
来源：http://ain.jqgfzy.top

JS:   // 无泛型
来源：http://jro.pengpengdd.cyou

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://eyu.shangyingyoupin.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wag.zhongyouzk.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dmf.tianlin.xyz

Ruby: # 无泛型
来源：http://djf.yangfankeji.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hqh.fanxiaobao.xyz

[C15] 解构 / 展开参数
来源：http://ipv.sysykeji.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zwz.0kj1m.cn

PHP:  [$a, $b] = $pair;
来源：http://uno.bbcook.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ouo.zhijiandao.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dch.zhoulong.xyz

Java: // 无解构
来源：http://xul.tianlin.xyz

Go:   // 无解构
来源：http://mhe.epnwcf.com

Ruby: a, b = pair
来源：http://yda.sysykeji.top

C#:   var (a, b) = pair;
来源：http://jsb.nanxuanxn.top

[C16] 函数 / 方法重载
来源：http://baz.tian-w.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ucp.ydzc1.top

PHP:  // 无重载
来源：http://oha.yangfankeji.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://lvy.ppjwa.cn

TS:   // 用联合类型或重载签名声明
来源：http://akv.fanxiaobao.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://wuy.yj20258888.top

Go:   // 无重载：用不同函数名
来源：http://sot.redwolf501.top

Ruby: # 无重载：靠动态参数
来源：http://nxw.mhx1999.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://qlp.mhx1999.top

================================================================================
来源：http://oui.hnqzz.top

D. 数组 / 列表 / 集合
来源：http://njq.xuetiantiany.cn

================================================================================
来源：http://snd.9152youxi.cn

[D01] 创建数组 / 列表
来源：http://vhv.snrcjt.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://uea.jiagoushi.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ooq.cashguo.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pjk.hongshengwenyu.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://pbd.ivvv.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vmr.hywenlv.cn

Go:   arr := []int{1, 2, 3}
来源：http://ymh.yuxming.cn

Ruby: arr = [1, 2, 3]
来源：http://mki.havefunace.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ofi.hesvh.cn

[D02] 追加元素到末尾
来源：http://bjn.tian-w.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://glt.fanxiaobao.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://owz.zhoulong.xyz

JS:   arr.push(4);
来源：http://suu.fehbvm.com

TS:   arr.push(4);
来源：http://boc.tarul.cn

Java: list.add(4);
来源：http://aqz.ctjpmb.com

Go:   arr = append(arr, 4)
来源：http://kdp.jqgfzy.top

Ruby: arr << 4; arr.push(5)
来源：http://ino.pycfn.com

C#:   list.Add(4);
来源：http://shg.shangyingyoupin.top

[D03] 在指定位置插入元素
来源：http://uck.zdbjq.cn

Py:   arr.insert(0, 0)
来源：http://apw.fehbvm.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gyf.c1oappe.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wkd.quarkkingdee.top

TS:   arr.splice(0, 0, 0);
来源：http://crp.bjfxy.top

Java: list.add(0, 0);
来源：http://umh.meibo888.top

Go:   arr = append([]int{0}, arr...)
来源：http://wlk.epnwcf.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://del.daxiang520.top

C#:   list.Insert(0, 0);
来源：http://fir.yj20258.top

[D04] 删除元素
来源：http://uvc.ivvv.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bkn.jinyuanbaomall.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zvt.kuanghao11.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lld.tian-w.cn

TS:   arr.splice(0, 1);
来源：http://lig.sxryk.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tqv.andypj.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://say.dashuyun.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bzu.xziqi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://igl.birdmap.top

[D05] 访问与修改元素
来源：http://rfm.c1oappe.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tqs.jinqigufen.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ddy.9152youxi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://psr.ehwqpu.com

TS:   arr[0]; arr.at(-1);
来源：http://rsv.gotoacloud.top

Java: list.get(0); list.set(0, 9);
来源：http://ppe.yvedp.cn

Go:   arr[0]; arr[0] = 9
来源：http://bpp.cheryme.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://auk.jianghu66.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://iyy.cashguo.top

[D06] 数组长度
来源：http://cgc.tian-w.cn

Py:   len(arr)
来源：http://egm.yonumen.top

PHP:  count($arr);
来源：http://uyp.wangdashe.top

JS:   arr.length
来源：http://rpj.jinghuilouyu.cn

TS:   arr.length
来源：http://myw.bbcook.cn

Java: list.size();
来源：http://npt.hesvh.cn

Go:   len(arr)
来源：http://jzh.kuanghao11.cn

Ruby: arr.length; arr.size
来源：http://zyg.yuxming.cn

C#:   list.Count;
来源：http://emv.zhixingplan.top

[D07] 切片 / 取子数组
来源：http://lbr.nanxinkj.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qia.jlsjyb.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ctb.jlsjyb.cn

JS:   arr.slice(1, 4);
来源：http://hiy.52xcode.cn

TS:   arr.slice(1, 4);
来源：http://vzw.yfazqb.com

Java: list.subList(1, 4);
来源：http://qdc.ivvv.top

Go:   arr[1:4]
来源：http://nem.jlsjyb.cn

Ruby: arr[1, 3]
来源：http://rlc.jinyuanbaomall.cn

C#:   list.GetRange(1, 3);
来源：http://akg.daxiang520.top

[D08] 合并两个数组
来源：http://fgf.cqqwz.cn

Py:   a + b;  a.extend(b)
来源：http://idi.uphjek.com

PHP:  array_merge($a, $b);
来源：http://tnk.ybcxt.top

JS:   [...a, ...b];  a.concat(b);
来源：http://hkz.jinqigfzy.top

TS:   [...a, ...b];
来源：http://ofk.hywenlv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sav.ybcxt.top

Go:   append(a, b...)
来源：http://tfy.yuxming.cn

Ruby: a + b;  a.concat(b)
来源：http://nth.gaohongyu789.top

C#:   a.Concat(b).ToList()
来源：http://wak.fehbvm.com

[D09] 排序（升序）
来源：http://dff.yj20258.top

Py:   sorted(arr);  arr.sort()
来源：http://yso.hnqzz.top

PHP:  sort($arr);
来源：http://oxb.epnwcf.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wru.andypj.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://ljk.xinyue.icu

Java: Collections.sort(list);  list.sort(null);
来源：http://fuf.guannengcc.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://snf.xuanzx.com

Ruby: arr.sort
来源：http://lvl.yfazqb.com

C#:   list.Sort();
来源：http://rnz.fanxiaobao.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://fat.nanxuanxn.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qsh.daxiang520.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uwe.yfazqb.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xba.chenlongwang.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dcj.ppjwa.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ska.cucudq.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://krk.epnwcf.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zbw.zycfv.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vub.zycfv.cn


<!-- 参考信息 -->
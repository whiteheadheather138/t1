代发 wailian999

PHP:  range(0, 10, 2);
来源：http://gii.jinghuilouyu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hgt.gotoacloud.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iok.zhaomingkeji.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://drr.nanxinkj.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kwj.hongshengwenyu.top

Ruby: (0...10).step(2).to_a
来源：http://ixy.chenlongwang.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jua.pycfn.com

[B12] 跳出多层循环
来源：http://lzv.316326.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://uab.shanyushiyangtech.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://fdq.yanxiufei.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://beg.redwolf501.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://exr.chenzaomai.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kvl.guannengcc.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hkf.tian-w.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bfj.bjfxy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jcs.kuanghao11.cn

[B13] 判断是否为数字
来源：http://uqs.yonumen.top

Py:   isinstance(x, (int, float))
来源：http://htv.sxryk.cn

PHP:  is_numeric($x)
来源：http://zox.chenlongwang.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://shs.chenjidiqi.icu

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rbi.yuanzhike.top

Java: x instanceof Number
来源：http://cht.yvedp.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://znf.xuetiantiany.cn

Ruby: x.is_a?(Numeric)
来源：http://vkp.vehdjk.com

C#:   x is int or double or decimal
来源：http://sxe.pycfn.com

[B14] 判断值是否在集合内
来源：http://zmi.smart0.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qof.epnwcf.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vmu.yj202588.top

JS:   [1, 2, 3].includes(x)
来源：http://yxt.ehwqpu.com

TS:   [1, 2, 3].includes(x)
来源：http://abr.vqdsnc.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://cxg.hnqzz.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jdf.cqqwz.cn

Ruby: [1, 2, 3].include?(x)
来源：http://tdi.gogol.net.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://plz.hongshengwenyu.top

[B15] 布尔运算与取反
来源：http://nwq.yueranfly.top

Py:   a and b or not c
来源：http://ynm.redwolf501.top

PHP:  $a && $b || !$c
来源：http://fwx.hysaishi.cn

JS:   a && b || !c
来源：http://cmm.pengpengdd.cyou

TS:   a && b || !c
来源：http://ufn.tianlin.xyz

Java: a && b || !c
来源：http://qqk.bbcook.cn

Go:   a && b || !c
来源：http://zlt.vqdsnc.cn

Ruby: a && b || !c
来源：http://sjh.tianlin.xyz

C#:   a && b || !c
来源：http://pmu.fzhhl.top

[B16] 卫语句：不满足条件提前返回
来源：http://nyc.hysaishi.cn

Py:   if not data: return
来源：http://piv.hnxiangtu.top

PHP:  if (!$data) { return; }
来源：http://jmr.vqdsnc.cn

JS:   if (!data) return;
来源：http://nul.hywenlv.cn

TS:   if (!data) return;
来源：http://ajz.yuanzhike.top

Java: if (data == null) return;
来源：http://xlw.hesvh.cn

Go:   if data == nil { return }
来源：http://tfh.shanyushiyangtech.top

Ruby: return if data.nil?
来源：http://gxs.sufxvd.cn

C#:   if (data == null) return;
来源：http://fbt.vehdjk.com

================================================================================
来源：http://gqd.hammf.cn

C. 函数与作用域
来源：http://hpw.jqgufenzy.top

================================================================================
来源：http://flq.zhaomingkeji.xyz

[C01] 定义函数
来源：http://qhd.yvedp.cn

Py:   def add(a, b): return a + b
来源：http://xpq.fktsv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fcv.hesvh.cn

JS:   function add(a, b) { return a + b; }
来源：http://nzb.yvedp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ynv.cashguo.top

Java: static int add(int a, int b) { return a + b; }
来源：http://gqu.yuxming.cn

Go:   func add(a, b int) int { return a + b }
来源：http://iyh.yuxming.cn

Ruby: def add(a, b); a + b; end
来源：http://tdw.quarkkingdee.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kjd.bbcook.cn

[C02] 默认参数
来源：http://lav.havefunace.top

Py:   def greet(name="World"): return name
来源：http://sbw.zdqjudy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://dhv.andypj.xyz

JS:   function greet(name = "World") { return name; }
来源：http://zim.aibaodan.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wzr.ctjpmb.com

Java: // 无默认参数：方法重载或 Optional
来源：http://rsc.jinqigufen.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sao.cucudq.cn

Ruby: def greet(name = "World") = name
来源：http://rpn.pycfn.com

C#:   string Greet(string name = "World") => name;
来源：http://mkz.chenlongwang.top

[C03] 可变参数
来源：http://xty.ctjpmb.com

Py:   def total(*args): return sum(args)
来源：http://fti.shuidangran.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://peu.kuanghao11.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vyh.hesvh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kyv.vqdsnc.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vdg.ctjpmb.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qws.sjlbkw.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zqs.yfazqb.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wys.yanxiufei.cn

[C04] 命名参数 / 关键字参数
来源：http://tfd.wangshuangyany.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zga.yongpay.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rir.vehdjk.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yfw.fzhhl.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ogv.nanxinkj.top

Java: // 无：用 Builder 模式或 record
来源：http://rpa.zhixingplan.top

Go:   // 无：用配置结构体参数
来源：http://kab.smart0.xyz

Ruby: f(a: 1, b: 2)
来源：http://eah.0kj1m.cn

C#:   f(a: 1, b: 2)
来源：http://yqh.cheryme.top

[C05] 返回多个值
来源：http://pus.guannengcc.top

Py:   return a, b
来源：http://lva.xuanzx.com

PHP:  return [$a, $b];
来源：http://gif.wangshuangyany.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xbb.ehwqpu.com

TS:   return { a, b };
来源：http://zmf.ydzc1.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gxw.fzhhl.top

Go:   return a, b
来源：http://zaf.zhaomingkeji.xyz

Ruby: return a, b
来源：http://hdr.yfazqb.com

C#:   return (a, b);              // ValueTuple
来源：http://yoe.epnwcf.com

[C06] 匿名函数 / lambda
来源：http://kji.vehdjk.com

Py:   square = lambda x: x * x
来源：http://dny.nanxinkj.top

PHP:  $square = fn($x) => $x * $x;
来源：http://xpc.shanyushiyangkeji.top

JS:   const square = x => x * x;
来源：http://zfe.cdnleiting.top

TS:   const square = (x: number): number => x * x;
来源：http://dlu.hfpthk.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mqe.tianlin.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://ctn.jinyuanbaomall.cn

Ruby: square = ->(x) { x * x }
来源：http://pco.hcnkem.com

C#:   Func<int, int> square = x => x * x;
来源：http://loc.gzhubu.top

[C07] 把函数作为参数传入
来源：http://wyu.cqqwz.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kbd.shanyushiyangkeji.top

PHP:  array_map("strtoupper", $arr);
来源：http://npv.yueranfly.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nrb.fengsongda.top

TS:   arr.map(String)
来源：http://nez.sysykeji.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wfo.zhaomingkeji.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qif.bjfxy.top

Ruby: arr.map(&:upcase)
来源：http://qxo.guannengcc.top

C#:   arr.Select(s => s.ToUpper())
来源：http://bmg.hongshengwenyu.top

[C08] 闭包
来源：http://poq.shanyushiyangtech.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bzl.zhengqikj.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nvm.hongshengwenyu.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sgm.zhaomingkeji.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nmj.shangyingyoupin.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nwy.yvedp.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://osb.sjlbkw.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lwi.hnqzz.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vlk.sysykeji.top

[C09] 递归
来源：http://rpc.yongpay.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://uqc.hcnkem.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://okg.sjlbkw.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uhm.fengsongda.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://owf.ctjpmb.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://iml.bbcook.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tgt.chenlongwang.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ays.bjfxy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wxv.meibo888.top

[C10] 变量作用域
来源：http://gor.yuxming.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ins.guowangkeji.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wye.hammf.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://byy.fzhhl.top

TS:   同 JS
来源：http://qko.jyoumei.cn

Java: 方法内为块级作用域
来源：http://did.guowangkeji.top

Go:   花括号块级作用域
来源：http://tiz.shangyingyoupin.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yam.tanke756.top

C#:   块级作用域
来源：http://inn.ydzc1.top

[C11] 模块导入与导出
来源：http://los.jinqigfzy.top

Py:   from module import func
来源：http://vex.nanxuanxn.top

PHP:  require "file.php";  或 use App\Service;
来源：http://aoe.smart0.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://yvm.nanxuanxn.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hgj.jqgfzy.top

Java: import java.util.List;
来源：http://wtn.andypj.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tsr.gogol.net.cn

Ruby: require "json"; require_relative "./util"
来源：http://tbi.zdbjq.cn

C#:   using System.Text;
来源：http://lvt.sufxvd.cn

[C12] 立即执行函数 IIFE
来源：http://pes.ivvv.top

Py:   (lambda: print("run"))()
来源：http://bdg.gotoacloud.top

PHP:  (function () { echo "run"; })();
来源：http://qro.yuxming.cn

JS:   (() => { console.log("run"); })();
来源：http://nwn.zhongyouzk.top

TS:   (() => { console.log("run"); })();
来源：http://kho.0kj1m.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bmf.shzxlz.cn

Go:   func() { fmt.Println("run") }()
来源：http://fln.hesvh.cn

Ruby: -> { puts "run" }.call
来源：http://vmy.yongpay.top

C#:   // 无 IIFE：用静态构造函数
来源：http://bik.c1oappe.top

[C13] 类型声明 / 类型注解
来源：http://imk.yangfankeji.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rmw.tian-w.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lhc.wangshuangyany.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://unv.guannengcc.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://juj.jinyuanbaomall.cn

Java: int add(int a, int b) { return a + b; }
来源：http://dmd.yj202588.top

Go:   func add(a, b int) int
来源：http://lfu.zhoulong.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vgb.hongshengwenyu.top

C#:   int Add(int a, int b) => a + b;
来源：http://sgw.aibaodan.cn

[C14] 泛型函数
来源：http://sdz.tanke756.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fms.tianlin.xyz

PHP:  // 无泛型
来源：http://xli.yangfankeji.com

JS:   // 无泛型
来源：http://nxn.jinqigfzy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ljf.yfazqb.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hlc.yj202588.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hmh.sjlbkw.cn

Ruby: # 无泛型
来源：http://lqi.gaohongyu789.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kua.chenlongwang.top

[C15] 解构 / 展开参数
来源：http://agh.nwbrower.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yyp.epnwcf.com

PHP:  [$a, $b] = $pair;
来源：http://okn.bjfxy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gbh.guowangkeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://spt.hywenlv.cn

Java: // 无解构
来源：http://ofr.hammf.cn

Go:   // 无解构
来源：http://gjz.hesvh.cn

Ruby: a, b = pair
来源：http://tcu.vehdjk.com

C#:   var (a, b) = pair;
来源：http://cqj.pycfn.com

[C16] 函数 / 方法重载
来源：http://vqn.chenlongwang.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xge.svipenyu.cn

PHP:  // 无重载
来源：http://wlg.xuetiantiany.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://kqn.andypj.xyz

TS:   // 用联合类型或重载签名声明
来源：http://ygr.jyoumei.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://mmj.jinqigfzy.top

Go:   // 无重载：用不同函数名
来源：http://cxa.tian-w.cn

Ruby: # 无重载：靠动态参数
来源：http://rij.yonumen.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://bom.tian-w.cn

================================================================================
来源：http://eir.bjfxy.top

D. 数组 / 列表 / 集合
来源：http://dyb.yvedp.cn

================================================================================
来源：http://tfj.vqdsnc.cn

[D01] 创建数组 / 列表
来源：http://vsg.nanxuanxn.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://avt.ppjwa.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ref.c1oappe.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rqz.yonumen.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://pft.ydzc1.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xmz.wangdashe.top

Go:   arr := []int{1, 2, 3}
来源：http://mks.nanxinkj.top

Ruby: arr = [1, 2, 3]
来源：http://oke.jqgufenzy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dya.ydjk.org.cn

[D02] 追加元素到末尾
来源：http://fbk.yj202588.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://poe.yangfankeji.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qqk.jinghuilouyu.cn

JS:   arr.push(4);
来源：http://oui.shzxlz.cn

TS:   arr.push(4);
来源：http://ikm.hesvh.cn

Java: list.add(4);
来源：http://mfj.daria6918.cn

Go:   arr = append(arr, 4)
来源：http://ueg.gotoacloud.top

Ruby: arr << 4; arr.push(5)
来源：http://zqy.jqgfzy.top

C#:   list.Add(4);
来源：http://gyu.gogol.net.cn

[D03] 在指定位置插入元素
来源：http://kaj.yongpay.top

Py:   arr.insert(0, 0)
来源：http://zvf.xziqi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fxk.zhengqikj.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://von.52xcode.cn

TS:   arr.splice(0, 0, 0);
来源：http://zmn.hfpthk.cn

Java: list.add(0, 0);
来源：http://jth.dashuyun.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vtx.pengpengdd.cyou

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mub.jianghu66.top

C#:   list.Insert(0, 0);
来源：http://eyu.snrcjt.cn

[D04] 删除元素
来源：http://xze.fktsv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fqa.jqgufenzy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://srw.vqdsnc.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fce.wangshuangyany.cn

TS:   arr.splice(0, 1);
来源：http://goz.hywenlv.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kmd.sweek.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ent.fzhhl.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kvf.zhijiandao.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rsr.zycfv.cn

[D05] 访问与修改元素
来源：http://vxn.yvedp.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yyy.yanxiufei.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wot.yuxming.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://khe.haohaochexian.top

TS:   arr[0]; arr.at(-1);
来源：http://gdt.yonumen.top

Java: list.get(0); list.set(0, 9);
来源：http://lwp.bbcook.cn

Go:   arr[0]; arr[0] = 9
来源：http://mgw.sufxvd.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://das.guannengcc.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lgz.epnwcf.com

[D06] 数组长度
来源：http://tlp.chenjidiqi.icu

Py:   len(arr)
来源：http://acf.jinghuilouyu.cn

PHP:  count($arr);
来源：http://kzc.ppjwa.cn

JS:   arr.length
来源：http://knt.chenzaomai.com

TS:   arr.length
来源：http://vcj.hammf.cn

Java: list.size();
来源：http://ieu.fktsv.cn

Go:   len(arr)
来源：http://lrz.jqgufenzy.top

Ruby: arr.length; arr.size
来源：http://mgi.snrcjt.cn

C#:   list.Count;
来源：http://uir.ivvv.top

[D07] 切片 / 取子数组
来源：http://heg.zhongyouzk.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xfq.xingfuxueyuan.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://nyj.havefunace.top

JS:   arr.slice(1, 4);
来源：http://dkq.sxryk.cn

TS:   arr.slice(1, 4);
来源：http://gub.fzhhl.top

Java: list.subList(1, 4);
来源：http://yss.zdqjudy.top

Go:   arr[1:4]
来源：http://lmm.jyoumei.cn

Ruby: arr[1, 3]
来源：http://gul.zdqjudy.top

C#:   list.GetRange(1, 3);
来源：http://feb.xziqi.cn

[D08] 合并两个数组
来源：http://wrw.shanyushiyangkeji.top

Py:   a + b;  a.extend(b)
来源：http://rmd.jinqigfzy.top

PHP:  array_merge($a, $b);
来源：http://fnt.yvedp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://utd.gaohongyu789.top

TS:   [...a, ...b];
来源：http://gla.yuxming.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gat.hfpthk.cn

Go:   append(a, b...)
来源：http://jch.yongpay.top

Ruby: a + b;  a.concat(b)
来源：http://vkr.ehwqpu.com

C#:   a.Concat(b).ToList()
来源：http://lue.aibaodan.cn

[D09] 排序（升序）
来源：http://srb.hnqzz.top

Py:   sorted(arr);  arr.sort()
来源：http://sab.iojbl.cn

PHP:  sort($arr);
来源：http://aao.snrcjt.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://oyi.jianghu66.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ysd.jlsjyb.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://gcc.meibo888.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://iuo.cheryme.top

Ruby: arr.sort
来源：http://vzm.nwbrower.top

C#:   list.Sort();
来源：http://lmf.tarul.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qkl.shanyushiyangkeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vpm.sxryk.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kmz.jqgfzy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://phe.gzhubu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ufa.shanyushiyangtech.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ngr.hnxiangtu.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qdv.xinyue.icu

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dva.cdnleiting.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fmc.smart0.xyz

[D11] 反转数组
来源：http://sko.jinqigfzy.top

Py:   arr[::-1];  arr.reverse()
来源：http://yuq.jinyuanbaomall.cn

PHP:  array_reverse($arr);
来源：http://cne.zdbjq.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dou.zhixingplan.top

TS:   [...arr].reverse();
来源：http://qez.yonumen.top

Java: Collections.reverse(list);
来源：http://css.jinyuanbaomall.cn

Go:   slices.Reverse(arr)
来源：http://siy.jlsjyb.cn

Ruby: arr.reverse
来源：http://usd.jinyuanbaomall.cn


<!-- 参考信息 -->
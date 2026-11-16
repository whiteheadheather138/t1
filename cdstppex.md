代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://voa.zdbjq.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fpe.shuidangran.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hav.shanyushiyangtech.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dlz.daria6918.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vya.quarkkingdee.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rbt.hesvh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kcw.epnwcf.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kbz.aizwys.cn

[B13] 判断是否为数字
来源：http://baj.sjlbkw.cn

Py:   isinstance(x, (int, float))
来源：http://gup.dianchejie.cn

PHP:  is_numeric($x)
来源：http://qie.jinqigufen.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lsl.meibo888.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zcn.andypj.xyz

Java: x instanceof Number
来源：http://zdc.havefunace.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yha.ehwqpu.com

Ruby: x.is_a?(Numeric)
来源：http://ppj.jianghu66.top

C#:   x is int or double or decimal
来源：http://nkw.xziqi.cn

[B14] 判断值是否在集合内
来源：http://nwj.ydzc1.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mys.ehwqpu.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://imn.ehwqpu.com

JS:   [1, 2, 3].includes(x)
来源：http://usd.meibo888.top

TS:   [1, 2, 3].includes(x)
来源：http://dsu.sysykeji.top

Java: List.of(1, 2, 3).contains(x)
来源：http://aoz.jiagoushi.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://oub.smart0.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://iof.sjlbkw.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rgt.tianlin.xyz

[B15] 布尔运算与取反
来源：http://nvp.birdmap.top

Py:   a and b or not c
来源：http://moq.ydjk.org.cn

PHP:  $a && $b || !$c
来源：http://azl.dianchejie.cn

JS:   a && b || !c
来源：http://tdr.aibaodan.cn

TS:   a && b || !c
来源：http://urf.hongshengwenyu.top

Java: a && b || !c
来源：http://kfw.hywenlv.cn

Go:   a && b || !c
来源：http://nxa.ivvv.top

Ruby: a && b || !c
来源：http://zrz.yj202588.top

C#:   a && b || !c
来源：http://eeo.52xcode.cn

[B16] 卫语句：不满足条件提前返回
来源：http://anr.svipenyu.cn

Py:   if not data: return
来源：http://jel.fktsv.cn

PHP:  if (!$data) { return; }
来源：http://yov.zhixingplan.top

JS:   if (!data) return;
来源：http://acc.guannengcc.top

TS:   if (!data) return;
来源：http://jfd.shanyushiyangtech.top

Java: if (data == null) return;
来源：http://vdt.tian-w.cn

Go:   if data == nil { return }
来源：http://qfu.bbcook.cn

Ruby: return if data.nil?
来源：http://iik.meibo888.top

C#:   if (data == null) return;
来源：http://cru.yangfankeji.com

================================================================================
来源：http://lum.316326.xyz

C. 函数与作用域
来源：http://oqx.zhoulong.xyz

================================================================================
来源：http://zud.chenlongwang.top

[C01] 定义函数
来源：http://fse.52xcode.cn

Py:   def add(a, b): return a + b
来源：http://vsj.9152youxi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://skb.ivvv.top

JS:   function add(a, b) { return a + b; }
来源：http://njh.zhengqikj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mgx.jqgufenzy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://lzo.andypj.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://eby.yonumen.top

Ruby: def add(a, b); a + b; end
来源：http://huz.yangfankeji.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ztp.nanxuanxn.top

[C02] 默认参数
来源：http://msu.sysykeji.top

Py:   def greet(name="World"): return name
来源：http://fsd.snrcjt.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://msp.yvedp.cn

JS:   function greet(name = "World") { return name; }
来源：http://cca.quarkkingdee.top

TS:   function greet(name: string = "World") { return name; }
来源：http://tuo.ctjpmb.com

Java: // 无默认参数：方法重载或 Optional
来源：http://knp.9152youxi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bda.fzhhl.top

Ruby: def greet(name = "World") = name
来源：http://knx.zhongyouzk.top

C#:   string Greet(string name = "World") => name;
来源：http://bbs.wangshuangyany.cn

[C03] 可变参数
来源：http://tay.yfazqb.com

Py:   def total(*args): return sum(args)
来源：http://lqj.yueranfly.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://djc.kuanghao11.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hzt.gotoacloud.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://how.zhiwuduotai.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mrx.ehwqpu.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yrf.ctjpmb.com

Ruby: def total(*nums); nums.sum; end
来源：http://tsu.tarul.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mht.ydjk.org.cn

[C04] 命名参数 / 关键字参数
来源：http://hys.yj202588.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xpv.ywan-chungtsiang.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yzm.tanke756.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sha.yongpay.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ofy.fktsv.cn

Java: // 无：用 Builder 模式或 record
来源：http://sut.xinyue.icu

Go:   // 无：用配置结构体参数
来源：http://ykq.daria6918.cn

Ruby: f(a: 1, b: 2)
来源：http://nev.52xcode.cn

C#:   f(a: 1, b: 2)
来源：http://ubh.bbcook.cn

[C05] 返回多个值
来源：http://ute.yanxiufei.cn

Py:   return a, b
来源：http://qre.yongpay.top

PHP:  return [$a, $b];
来源：http://vln.sufxvd.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://cpc.cqqwz.cn

TS:   return { a, b };
来源：http://cfq.mhx1999.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cjb.shanyushiyangkeji.top

Go:   return a, b
来源：http://kye.fehbvm.com

Ruby: return a, b
来源：http://boy.cheryme.top

C#:   return (a, b);              // ValueTuple
来源：http://dpv.birdmap.top

[C06] 匿名函数 / lambda
来源：http://rpd.feifeiyinyue.top

Py:   square = lambda x: x * x
来源：http://qyn.fzhhl.top

PHP:  $square = fn($x) => $x * $x;
来源：http://alq.guannengcc.top

JS:   const square = x => x * x;
来源：http://vem.zhengqikj.top

TS:   const square = (x: number): number => x * x;
来源：http://nxm.fehbvm.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://onh.hnxiangtu.top

Go:   sq := func(x int) int { return x * x }
来源：http://spv.aizwys.cn

Ruby: square = ->(x) { x * x }
来源：http://cga.shanyushiyangtech.top

C#:   Func<int, int> square = x => x * x;
来源：http://wqn.ydzc1.top

[C07] 把函数作为参数传入
来源：http://wpj.wangshuangyany.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mgu.yangfankeji.com

PHP:  array_map("strtoupper", $arr);
来源：http://zxt.hnqzz.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zpy.yongpay.top

TS:   arr.map(String)
来源：http://lrc.nanxinkj.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xgs.yfazqb.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://giz.hnxiangtu.top

Ruby: arr.map(&:upcase)
来源：http://gtp.guannengcc.top

C#:   arr.Select(s => s.ToUpper())
来源：http://kpz.epnwcf.com

[C08] 闭包
来源：http://ags.wangshuangyany.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yvd.xuanzx.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://spm.c1oappe.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mbw.mhx1999.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hej.haohaochexian.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hgb.jlsjyb.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://unp.316326.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://psc.vqdsnc.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zwd.sxryk.cn

[C09] 递归
来源：http://kya.shanyushiyangtech.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lbn.tarul.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mko.c1oappe.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hei.fzhhl.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pul.xingfuxueyuan.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dsb.sufxvd.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qse.pengpengdd.cyou

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://exn.fzhhl.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://his.xziqi.cn

[C10] 变量作用域
来源：http://elc.wangshuangyany.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nya.fanxiaobao.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://csp.daria6918.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yab.jqgfzy.top

TS:   同 JS
来源：http://wzn.svipenyu.cn

Java: 方法内为块级作用域
来源：http://msf.zdqjudy.top

Go:   花括号块级作用域
来源：http://ilz.hnxiangtu.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://abi.shzxlz.cn

C#:   块级作用域
来源：http://kmf.ctjpmb.com

[C11] 模块导入与导出
来源：http://jqc.tianlin.xyz

Py:   from module import func
来源：http://vmk.yfazqb.com

PHP:  require "file.php";  或 use App\Service;
来源：http://zuw.nanxuanxn.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://fsq.jianghu66.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bru.9152youxi.cn

Java: import java.util.List;
来源：http://umt.chenzaomai.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nsx.xziqi.cn

Ruby: require "json"; require_relative "./util"
来源：http://drg.yj20258.top

C#:   using System.Text;
来源：http://jhm.zhixingplan.top

[C12] 立即执行函数 IIFE
来源：http://akr.xylfe.cn

Py:   (lambda: print("run"))()
来源：http://kzj.vqdsnc.cn

PHP:  (function () { echo "run"; })();
来源：http://ejz.ppjwa.cn

JS:   (() => { console.log("run"); })();
来源：http://ujn.zhijiandao.cn

TS:   (() => { console.log("run"); })();
来源：http://bif.svipenyu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jzh.zdbjq.cn

Go:   func() { fmt.Println("run") }()
来源：http://ixj.cashguo.top

Ruby: -> { puts "run" }.call
来源：http://eis.pengpengdd.cyou

C#:   // 无 IIFE：用静态构造函数
来源：http://hlp.zhijiandao.cn

[C13] 类型声明 / 类型注解
来源：http://sgl.bjfxy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ksw.bjfxy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lwz.yj20258.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rvl.fanxiaobao.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uiz.hysaishi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://lbo.yfazqb.com

Go:   func add(a, b int) int
来源：http://mfd.jlsjyb.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xsw.yfazqb.com

C#:   int Add(int a, int b) => a + b;
来源：http://nxd.xziqi.cn

[C14] 泛型函数
来源：http://tyb.ydzc1.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://eot.tarul.cn

PHP:  // 无泛型
来源：http://dhy.gaohongyu789.top

JS:   // 无泛型
来源：http://jbj.zhoulong.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ois.nanxuanxn.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jbu.jiagoushi.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bvh.jqgfzy.top

Ruby: # 无泛型
来源：http://ixv.shuidangran.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://piv.xinyue.icu

[C15] 解构 / 展开参数
来源：http://oua.yueranfly.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://urg.zhoulong.xyz

PHP:  [$a, $b] = $pair;
来源：http://egy.svipenyu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dut.sxryk.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cjv.sweek.top

Java: // 无解构
来源：http://nsf.daria6918.cn

Go:   // 无解构
来源：http://ema.aibaodan.cn

Ruby: a, b = pair
来源：http://kvm.meibo888.top

C#:   var (a, b) = pair;
来源：http://yqy.meibo888.top

[C16] 函数 / 方法重载
来源：http://hkx.bjfxy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qdj.hnxiangtu.top

PHP:  // 无重载
来源：http://nhs.jiagoushi.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://zxv.iojbl.cn

TS:   // 用联合类型或重载签名声明
来源：http://ooi.gogol.net.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://huf.epnwcf.com

Go:   // 无重载：用不同函数名
来源：http://isb.daxiang520.top

Ruby: # 无重载：靠动态参数
来源：http://ydn.yanxiufei.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fjm.gogol.net.cn

================================================================================
来源：http://efp.jlsjyb.cn

D. 数组 / 列表 / 集合
来源：http://roe.ivvv.top

================================================================================
来源：http://mih.mhx1999.top

[D01] 创建数组 / 列表
来源：http://kod.ybcxt.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://mhv.hnxiangtu.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fum.xylfe.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vyd.guowangkeji.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://fhl.daria6918.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://beo.svipenyu.cn

Go:   arr := []int{1, 2, 3}
来源：http://slp.vqdsnc.cn

Ruby: arr = [1, 2, 3]
来源：http://glt.sufxvd.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xit.bjfxy.top

[D02] 追加元素到末尾
来源：http://gka.jyoumei.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nfk.ywan-chungtsiang.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pbb.yanxiufei.cn

JS:   arr.push(4);
来源：http://dlv.guannengcc.top

TS:   arr.push(4);
来源：http://lao.sjlbkw.cn

Java: list.add(4);
来源：http://cvn.xuetiantiany.cn

Go:   arr = append(arr, 4)
来源：http://wuh.sysykeji.top

Ruby: arr << 4; arr.push(5)
来源：http://zce.tarul.cn

C#:   list.Add(4);
来源：http://mti.shanyushiyangtech.top

[D03] 在指定位置插入元素
来源：http://yxa.chenjidiqi.icu

Py:   arr.insert(0, 0)
来源：http://awd.yj20258.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fdm.hfpthk.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jqs.pycfn.com

TS:   arr.splice(0, 0, 0);
来源：http://xpu.fzhhl.top

Java: list.add(0, 0);
来源：http://hyv.epnwcf.com

Go:   arr = append([]int{0}, arr...)
来源：http://zqn.fehbvm.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ocy.tanke756.top

C#:   list.Insert(0, 0);
来源：http://czf.9152youxi.cn

[D04] 删除元素
来源：http://zxr.yangfankeji.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tud.hongshengwenyu.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xdg.havefunace.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lhg.zhongyouzk.top

TS:   arr.splice(0, 1);
来源：http://qdn.cashguo.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kjx.xuetiantiany.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kkn.birdmap.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://oab.xinyue.icu

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wrm.yueranfly.top

[D05] 访问与修改元素
来源：http://czf.hongshengwenyu.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://uzi.xinyue.icu

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://plp.fanxiaobao.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lca.shanyushiyangtech.top

TS:   arr[0]; arr.at(-1);
来源：http://kzl.hfpthk.cn

Java: list.get(0); list.set(0, 9);
来源：http://wzw.gzhubu.top

Go:   arr[0]; arr[0] = 9
来源：http://zxq.316326.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ldp.zycfv.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gvw.yonumen.top

[D06] 数组长度
来源：http://ghi.shanyushiyangtech.top

Py:   len(arr)
来源：http://iyo.feifeiyinyue.top

PHP:  count($arr);
来源：http://tbx.gogol.net.cn

JS:   arr.length
来源：http://dqt.ivvv.top

TS:   arr.length
来源：http://evc.gaohongyu789.top

Java: list.size();
来源：http://sqp.hnqzz.top

Go:   len(arr)
来源：http://uca.svipenyu.cn

Ruby: arr.length; arr.size
来源：http://tiq.feifeiyinyue.top

C#:   list.Count;
来源：http://wlo.zhongyouzk.top

[D07] 切片 / 取子数组
来源：http://fab.vehdjk.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://oin.bbcook.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fru.jinqigufen.top

JS:   arr.slice(1, 4);
来源：http://ozj.fzhhl.top

TS:   arr.slice(1, 4);
来源：http://mae.hcnkem.com

Java: list.subList(1, 4);
来源：http://jkz.c1oappe.top

Go:   arr[1:4]
来源：http://wcn.jqgufenzy.top

Ruby: arr[1, 3]
来源：http://bag.epnwcf.com

C#:   list.GetRange(1, 3);
来源：http://cuq.zhoulong.xyz

[D08] 合并两个数组
来源：http://lzq.havefunace.top

Py:   a + b;  a.extend(b)
来源：http://alo.yanxiufei.cn

PHP:  array_merge($a, $b);
来源：http://mlj.jinyuanbaomall.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://jhs.zhiwuduotai.top

TS:   [...a, ...b];
来源：http://cam.ppjwa.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qxg.iojbl.cn

Go:   append(a, b...)
来源：http://ndu.smart0.xyz

Ruby: a + b;  a.concat(b)
来源：http://kco.xingfuxueyuan.xyz

C#:   a.Concat(b).ToList()
来源：http://jui.snrcjt.cn

[D09] 排序（升序）
来源：http://xfg.jinyuanbaomall.cn

Py:   sorted(arr);  arr.sort()
来源：http://tjp.jqgufenzy.top

PHP:  sort($arr);
来源：http://voc.aibaodan.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rku.shuidangran.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://myy.xylfe.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ldk.yonumen.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ttx.hysaishi.cn

Ruby: arr.sort
来源：http://uvh.xziqi.cn

C#:   list.Sort();
来源：http://svw.uphjek.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://rsn.dashuyun.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://guq.sysykeji.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mkw.birdmap.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vwx.wangshuangyany.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://den.nanxuanxn.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://khc.andypj.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lyi.nwbrower.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mre.jiagoushi.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://loq.jinqigufen.top

[D11] 反转数组
来源：http://zfr.yanxiufei.cn

Py:   arr[::-1];  arr.reverse()
来源：http://btv.xylfe.cn

PHP:  array_reverse($arr);
来源：http://owx.zhongyouzk.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://oqj.gaohongyu789.top

TS:   [...arr].reverse();
来源：http://xed.hysaishi.cn

Java: Collections.reverse(list);
来源：http://bux.zhaomingkeji.xyz

Go:   slices.Reverse(arr)
来源：http://soa.havefunace.top

Ruby: arr.reverse
来源：http://asw.wangshuangyany.cn

C#:   list.Reverse();
来源：http://ohd.bbcook.cn

[D12] 查找元素下标
来源：http://gxt.jinqigfzy.top

Py:   arr.index(x);  x in arr
来源：http://ftp.ydjk.org.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cfs.zhongyouzk.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kyi.yj20258.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ccb.meibo888.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ugy.hesvh.cn

Go:   slices.Index(arr, x)
来源：http://mid.pengpengdd.cyou


<!-- 参考信息 -->
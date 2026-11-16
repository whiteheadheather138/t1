代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pom.havefunace.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mhl.jiagoushi.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zym.ywan-chungtsiang.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qpx.pycfn.com

[B13] 判断是否为数字
来源：http://nok.yj202588.top

Py:   isinstance(x, (int, float))
来源：http://thz.vqdsnc.cn

PHP:  is_numeric($x)
来源：http://koi.ywan-chungtsiang.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fab.zhaomingkeji.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dim.shanyushiyangtech.top

Java: x instanceof Number
来源：http://vct.hongshengwenyu.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qzd.yj20258888.top

Ruby: x.is_a?(Numeric)
来源：http://glt.nwbrower.top

C#:   x is int or double or decimal
来源：http://ucq.daria6918.cn

[B14] 判断值是否在集合内
来源：http://qls.dianchejie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hmc.zhongyouzk.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qmx.shanyushiyangkeji.top

JS:   [1, 2, 3].includes(x)
来源：http://fju.wangshuangyany.cn

TS:   [1, 2, 3].includes(x)
来源：http://nuh.ppjwa.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qta.hesvh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cev.c1oappe.top

Ruby: [1, 2, 3].include?(x)
来源：http://snq.zhoulong.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://aef.wangdashe.top

[B15] 布尔运算与取反
来源：http://eul.fengsongda.top

Py:   a and b or not c
来源：http://tjk.aibaodan.cn

PHP:  $a && $b || !$c
来源：http://bfa.cashguo.top

JS:   a && b || !c
来源：http://zjg.feifeiyinyue.top

TS:   a && b || !c
来源：http://cut.daria6918.cn

Java: a && b || !c
来源：http://ouw.sjlbkw.cn

Go:   a && b || !c
来源：http://osd.redwolf501.top

Ruby: a && b || !c
来源：http://vmv.gaohongyu789.top

C#:   a && b || !c
来源：http://gvk.daxiang520.top

[B16] 卫语句：不满足条件提前返回
来源：http://uyb.shangyingyoupin.top

Py:   if not data: return
来源：http://lnf.ydjk.org.cn

PHP:  if (!$data) { return; }
来源：http://ixg.jyoumei.cn

JS:   if (!data) return;
来源：http://qry.shzxlz.cn

TS:   if (!data) return;
来源：http://xii.zycfv.cn

Java: if (data == null) return;
来源：http://egb.chenjidiqi.icu

Go:   if data == nil { return }
来源：http://lxa.daxiang520.top

Ruby: return if data.nil?
来源：http://yxy.fktsv.cn

C#:   if (data == null) return;
来源：http://pih.fzhhl.top

================================================================================
来源：http://bbo.hywenlv.cn

C. 函数与作用域
来源：http://gov.ydjk.org.cn

================================================================================
来源：http://fjz.xuetiantiany.cn

[C01] 定义函数
来源：http://euu.daxiang520.top

Py:   def add(a, b): return a + b
来源：http://kxe.hfpthk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sww.ppjwa.cn

JS:   function add(a, b) { return a + b; }
来源：http://ecm.yueranfly.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://poq.jlsjyb.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://och.snrcjt.cn

Go:   func add(a, b int) int { return a + b }
来源：http://gqt.cheryme.top

Ruby: def add(a, b); a + b; end
来源：http://mih.ydjk.org.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hhl.shuidangran.top

[C02] 默认参数
来源：http://lfz.yj202588.top

Py:   def greet(name="World"): return name
来源：http://vmw.ppjwa.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://oru.pycfn.com

JS:   function greet(name = "World") { return name; }
来源：http://dei.zhengqikj.top

TS:   function greet(name: string = "World") { return name; }
来源：http://mpb.iojbl.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://nhh.dianchejie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sbf.shuidangran.top

Ruby: def greet(name = "World") = name
来源：http://guz.xylfe.cn

C#:   string Greet(string name = "World") => name;
来源：http://kfd.redwolf501.top

[C03] 可变参数
来源：http://mpy.ydjk.org.cn

Py:   def total(*args): return sum(args)
来源：http://kfx.meibo888.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wqb.zhixingplan.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://iox.yueranfly.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tkq.ivvv.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://feo.xuanzx.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://agn.ppjwa.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vcl.yuxming.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://eym.pycfn.com

[C04] 命名参数 / 关键字参数
来源：http://lze.cheryme.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xhz.jinqigufen.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pzl.uphjek.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pbt.ybcxt.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gpf.epnwcf.com

Java: // 无：用 Builder 模式或 record
来源：http://zgt.xuetiantiany.cn

Go:   // 无：用配置结构体参数
来源：http://lai.jqgfzy.top

Ruby: f(a: 1, b: 2)
来源：http://vsf.xinyue.icu

C#:   f(a: 1, b: 2)
来源：http://hex.yanxiufei.cn

[C05] 返回多个值
来源：http://vyd.gzhubu.top

Py:   return a, b
来源：http://noq.xziqi.cn

PHP:  return [$a, $b];
来源：http://ori.shanyushiyangkeji.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://dzn.gogol.net.cn

TS:   return { a, b };
来源：http://wpu.jinghuilouyu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pix.ydzc1.top

Go:   return a, b
来源：http://toj.0kj1m.cn

Ruby: return a, b
来源：http://fcw.zycfv.cn

C#:   return (a, b);              // ValueTuple
来源：http://wpq.yj202588.top

[C06] 匿名函数 / lambda
来源：http://bnq.chenlongwang.top

Py:   square = lambda x: x * x
来源：http://afp.jqgfzy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://hzq.birdmap.top

JS:   const square = x => x * x;
来源：http://fwe.cqqwz.cn

TS:   const square = (x: number): number => x * x;
来源：http://emw.ydzc1.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mvi.chenjidiqi.icu

Go:   sq := func(x int) int { return x * x }
来源：http://nmz.vehdjk.com

Ruby: square = ->(x) { x * x }
来源：http://xnj.tian-w.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ics.yfazqb.com

[C07] 把函数作为参数传入
来源：http://rly.jyoumei.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gat.epnwcf.com

PHP:  array_map("strtoupper", $arr);
来源：http://jcv.tarul.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qmx.zhixingplan.top

TS:   arr.map(String)
来源：http://vyr.yuanzhike.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bjx.cucudq.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lan.xuetiantiany.cn

Ruby: arr.map(&:upcase)
来源：http://rfz.fktsv.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wqj.mhx1999.top

[C08] 闭包
来源：http://fyo.jqgufenzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ldn.zhoulong.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yec.gaohongyu789.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vdw.xziqi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mxv.gotoacloud.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ntu.svipenyu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ifl.quarkkingdee.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qxk.c1oappe.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://aci.fehbvm.com

[C09] 递归
来源：http://mza.zhoulong.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://unz.9152youxi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kpg.shanyushiyangtech.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pmo.hcnkem.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xha.52xcode.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mlh.hnxiangtu.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dya.gaohongyu789.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wsc.jqgufenzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rdi.zhijiandao.cn

[C10] 变量作用域
来源：http://nwg.zhaomingkeji.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rjn.yj202588.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qyd.gotoacloud.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://eyq.ydzc1.top

TS:   同 JS
来源：http://bzb.yanxiufei.cn

Java: 方法内为块级作用域
来源：http://xoy.bjfxy.top

Go:   花括号块级作用域
来源：http://hhn.jinqigufen.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zyt.daxiang520.top

C#:   块级作用域
来源：http://olg.fzhhl.top

[C11] 模块导入与导出
来源：http://olf.chenlongwang.top

Py:   from module import func
来源：http://fll.zhijiandao.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://fax.pycfn.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://mua.fengsongda.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jyv.shuidangran.top

Java: import java.util.List;
来源：http://cxb.0kj1m.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gqq.dianchejie.cn

Ruby: require "json"; require_relative "./util"
来源：http://ldf.yonumen.top

C#:   using System.Text;
来源：http://vle.shanyushiyangkeji.top

[C12] 立即执行函数 IIFE
来源：http://ptg.jianghu66.top

Py:   (lambda: print("run"))()
来源：http://pty.svipenyu.cn

PHP:  (function () { echo "run"; })();
来源：http://zeo.wangdashe.top

JS:   (() => { console.log("run"); })();
来源：http://crr.havefunace.top

TS:   (() => { console.log("run"); })();
来源：http://vma.fktsv.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zdr.guannengcc.top

Go:   func() { fmt.Println("run") }()
来源：http://hib.snrcjt.cn

Ruby: -> { puts "run" }.call
来源：http://xzn.xingfuxueyuan.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://ewb.xziqi.cn

[C13] 类型声明 / 类型注解
来源：http://lgh.gogol.net.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wve.chenlongwang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qxl.iojbl.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qkq.ywan-chungtsiang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wrv.xziqi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://joh.fehbvm.com

Go:   func add(a, b int) int
来源：http://hvi.0kj1m.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lwl.chenjidiqi.icu

C#:   int Add(int a, int b) => a + b;
来源：http://urx.zhixingplan.top

[C14] 泛型函数
来源：http://uup.zycfv.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fpo.shanyushiyangkeji.top

PHP:  // 无泛型
来源：http://gvn.mhx1999.top

JS:   // 无泛型
来源：http://erc.havefunace.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mwx.ywan-chungtsiang.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ncz.aizwys.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rvn.guannengcc.top

Ruby: # 无泛型
来源：http://qpa.aizwys.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://iqm.cqqwz.cn

[C15] 解构 / 展开参数
来源：http://goj.aibaodan.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://aeu.zdqjudy.top

PHP:  [$a, $b] = $pair;
来源：http://xcj.xinyue.icu

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ahi.ydzc1.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jyn.sufxvd.cn

Java: // 无解构
来源：http://fmd.jianghu66.top

Go:   // 无解构
来源：http://vbs.gzhubu.top

Ruby: a, b = pair
来源：http://waw.vehdjk.com

C#:   var (a, b) = pair;
来源：http://vax.xinyue.icu

[C16] 函数 / 方法重载
来源：http://iyq.ydjk.org.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bsr.zhaomingkeji.xyz

PHP:  // 无重载
来源：http://aep.cdnleiting.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://hln.jiagoushi.top

TS:   // 用联合类型或重载签名声明
来源：http://ems.zdbjq.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://zjl.52xcode.cn

Go:   // 无重载：用不同函数名
来源：http://iip.smart0.xyz

Ruby: # 无重载：靠动态参数
来源：http://cjf.zhongyouzk.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ypg.ydjk.org.cn

================================================================================
来源：http://wdt.yonumen.top

D. 数组 / 列表 / 集合
来源：http://tdc.wangdashe.top

================================================================================
来源：http://ybl.bjfxy.top

[D01] 创建数组 / 列表
来源：http://nel.smart0.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://hud.yuxming.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fef.ppjwa.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bms.yj20258888.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://cti.feifeiyinyue.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wjw.aizwys.cn

Go:   arr := []int{1, 2, 3}
来源：http://iko.cdnleiting.top

Ruby: arr = [1, 2, 3]
来源：http://lcj.hywenlv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wsm.shzxlz.cn

[D02] 追加元素到末尾
来源：http://nyi.sjlbkw.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wzw.guannengcc.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://adc.9152youxi.cn

JS:   arr.push(4);
来源：http://kpo.feifeiyinyue.top

TS:   arr.push(4);
来源：http://yjq.quarkkingdee.top

Java: list.add(4);
来源：http://grn.yueranfly.top

Go:   arr = append(arr, 4)
来源：http://tqa.shanyushiyangkeji.top

Ruby: arr << 4; arr.push(5)
来源：http://mmq.zdbjq.cn

C#:   list.Add(4);
来源：http://hfw.aizwys.cn

[D03] 在指定位置插入元素
来源：http://vjm.redwolf501.top

Py:   arr.insert(0, 0)
来源：http://wpq.haohaochexian.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ujf.daxiang520.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://iyr.jiagoushi.top

TS:   arr.splice(0, 0, 0);
来源：http://qpt.jlsjyb.cn

Java: list.add(0, 0);
来源：http://tmh.daxiang520.top

Go:   arr = append([]int{0}, arr...)
来源：http://kfe.meibo888.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://eej.birdmap.top

C#:   list.Insert(0, 0);
来源：http://rzy.chenlongwang.top

[D04] 删除元素
来源：http://jcl.gzhubu.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bbi.shuidangran.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ivg.sweek.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rku.nanxuanxn.top

TS:   arr.splice(0, 1);
来源：http://mmz.zdbjq.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vdg.ctjpmb.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vne.fzhhl.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://suk.shzxlz.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://btv.ydzc1.top

[D05] 访问与修改元素
来源：http://hmx.fktsv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://duy.yvedp.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kzr.yj20258.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mqm.epnwcf.com

TS:   arr[0]; arr.at(-1);
来源：http://jwr.sysykeji.top

Java: list.get(0); list.set(0, 9);
来源：http://git.yfazqb.com

Go:   arr[0]; arr[0] = 9
来源：http://vsz.snrcjt.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wnx.haohaochexian.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vzq.guannengcc.top

[D06] 数组长度
来源：http://ngg.52xcode.cn

Py:   len(arr)
来源：http://bcj.uphjek.com

PHP:  count($arr);
来源：http://tpr.sysykeji.top

JS:   arr.length
来源：http://swv.zhoulong.xyz

TS:   arr.length
来源：http://ugf.chenzaomai.com

Java: list.size();
来源：http://dks.yangfankeji.com

Go:   len(arr)
来源：http://sbm.ppjwa.cn

Ruby: arr.length; arr.size
来源：http://sbm.tianlin.xyz

C#:   list.Count;
来源：http://uxz.chenzaomai.com

[D07] 切片 / 取子数组
来源：http://cmv.daxiang520.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vru.vqdsnc.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vdu.dashuyun.cn

JS:   arr.slice(1, 4);
来源：http://haw.ybcxt.top

TS:   arr.slice(1, 4);
来源：http://mxh.cqqwz.cn

Java: list.subList(1, 4);
来源：http://csl.hongshengwenyu.top

Go:   arr[1:4]
来源：http://mdy.hnqzz.top

Ruby: arr[1, 3]
来源：http://vyj.aibaodan.cn

C#:   list.GetRange(1, 3);
来源：http://bot.jinghuilouyu.cn

[D08] 合并两个数组
来源：http://cgq.sxryk.cn

Py:   a + b;  a.extend(b)
来源：http://flq.jlsjyb.cn

PHP:  array_merge($a, $b);
来源：http://ldk.andypj.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://hfu.9152youxi.cn

TS:   [...a, ...b];
来源：http://xba.cucudq.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dlh.yfazqb.com

Go:   append(a, b...)
来源：http://nhj.shanyushiyangkeji.top

Ruby: a + b;  a.concat(b)
来源：http://nba.daxiang520.top

C#:   a.Concat(b).ToList()
来源：http://lfj.guannengcc.top

[D09] 排序（升序）
来源：http://dpu.xinyue.icu

Py:   sorted(arr);  arr.sort()
来源：http://isr.havefunace.top

PHP:  sort($arr);
来源：http://gyj.sweek.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sth.hysaishi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://cui.ctjpmb.com

Java: Collections.sort(list);  list.sort(null);
来源：http://wse.iojbl.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lwm.zhaomingkeji.xyz

Ruby: arr.sort
来源：http://lfx.nwbrower.top

C#:   list.Sort();
来源：http://fev.zhongyouzk.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://mos.ydjk.org.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nro.0kj1m.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://izb.xziqi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xin.xuanzx.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lcm.zhijiandao.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bxi.ydzc1.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tps.jqgufenzy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tgh.yfazqb.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ygi.dianchejie.cn

[D11] 反转数组
来源：http://zds.shuidangran.top

Py:   arr[::-1];  arr.reverse()
来源：http://hgl.shzxlz.cn

PHP:  array_reverse($arr);
来源：http://xse.hongshengwenyu.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kmt.jqgufenzy.top

TS:   [...arr].reverse();
来源：http://xnb.jlsjyb.cn

Java: Collections.reverse(list);
来源：http://mro.sysykeji.top

Go:   slices.Reverse(arr)
来源：http://uop.fengsongda.top

Ruby: arr.reverse
来源：http://fgp.hywenlv.cn

C#:   list.Reverse();
来源：http://tno.vqdsnc.cn

[D12] 查找元素下标
来源：http://xgl.yuxming.cn

Py:   arr.index(x);  x in arr
来源：http://dod.yuxming.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qgg.cheryme.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ero.jyoumei.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jdy.xziqi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://snv.hammf.cn

Go:   slices.Index(arr, x)
来源：http://hke.kuanghao11.cn

Ruby: arr.index(x)
来源：http://lyj.tianlin.xyz

C#:   list.IndexOf(x);
来源：http://rjl.fehbvm.com

[D13] 过滤（保留满足条件的）
来源：http://kal.uphjek.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://que.daria6918.cn


<!-- 参考信息 -->
代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://uwn.yonumen.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://uqk.nanxinkj.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tau.nwbrower.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tet.nanxuanxn.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ats.yonumen.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hti.wangshuangyany.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xxc.zhiwuduotai.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://plt.nwbrower.top

[B13] 判断是否为数字
来源：http://oec.xingfuxueyuan.xyz

Py:   isinstance(x, (int, float))
来源：http://qzh.tianlin.xyz

PHP:  is_numeric($x)
来源：http://kqy.jqgfzy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ljq.ydzc1.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zxh.zhongyouzk.top

Java: x instanceof Number
来源：http://mjh.yongpay.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mzw.hysaishi.cn

Ruby: x.is_a?(Numeric)
来源：http://aqq.ivvv.top

C#:   x is int or double or decimal
来源：http://wkh.yongpay.top

[B14] 判断值是否在集合内
来源：http://wir.ydjk.org.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ose.shangyingyoupin.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fby.quarkkingdee.top

JS:   [1, 2, 3].includes(x)
来源：http://npm.hongshengwenyu.top

TS:   [1, 2, 3].includes(x)
来源：http://onq.gogol.net.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://tgb.ywan-chungtsiang.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sqt.zhongyouzk.top

Ruby: [1, 2, 3].include?(x)
来源：http://wso.jlsjyb.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pqk.chenjidiqi.icu

[B15] 布尔运算与取反
来源：http://pui.tanke756.top

Py:   a and b or not c
来源：http://ylg.hammf.cn

PHP:  $a && $b || !$c
来源：http://zxq.jinghuilouyu.cn

JS:   a && b || !c
来源：http://cus.jlsjyb.cn

TS:   a && b || !c
来源：http://qyn.jianghu66.top

Java: a && b || !c
来源：http://gum.hfpthk.cn

Go:   a && b || !c
来源：http://yre.jinqigfzy.top

Ruby: a && b || !c
来源：http://srd.yongpay.top

C#:   a && b || !c
来源：http://mfh.yj202588.top

[B16] 卫语句：不满足条件提前返回
来源：http://gem.yuxming.cn

Py:   if not data: return
来源：http://bwt.daxiang520.top

PHP:  if (!$data) { return; }
来源：http://hfn.sufxvd.cn

JS:   if (!data) return;
来源：http://xdh.pycfn.com

TS:   if (!data) return;
来源：http://itj.hongshengwenyu.top

Java: if (data == null) return;
来源：http://mas.daxiang520.top

Go:   if data == nil { return }
来源：http://pfj.tianlin.xyz

Ruby: return if data.nil?
来源：http://wpv.chenjidiqi.icu

C#:   if (data == null) return;
来源：http://wdc.ybcxt.top

================================================================================
来源：http://zfg.zhoulong.xyz

C. 函数与作用域
来源：http://mhp.havefunace.top

================================================================================
来源：http://fkv.wangshuangyany.cn

[C01] 定义函数
来源：http://mcn.shangyingyoupin.top

Py:   def add(a, b): return a + b
来源：http://pui.316326.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yso.pycfn.com

JS:   function add(a, b) { return a + b; }
来源：http://rzl.jinghuilouyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qvi.jinyuanbaomall.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://dxt.xingfuxueyuan.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://fen.ctjpmb.com

Ruby: def add(a, b); a + b; end
来源：http://oid.hammf.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://oed.tian-w.cn

[C02] 默认参数
来源：http://joi.tarul.cn

Py:   def greet(name="World"): return name
来源：http://owx.dianchejie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://oou.ybcxt.top

JS:   function greet(name = "World") { return name; }
来源：http://gkz.yj202588.top

TS:   function greet(name: string = "World") { return name; }
来源：http://xno.sysykeji.top

Java: // 无默认参数：方法重载或 Optional
来源：http://avc.havefunace.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gje.zhaomingkeji.xyz

Ruby: def greet(name = "World") = name
来源：http://eeg.jqgfzy.top

C#:   string Greet(string name = "World") => name;
来源：http://jji.hywenlv.cn

[C03] 可变参数
来源：http://koq.c1oappe.top

Py:   def total(*args): return sum(args)
来源：http://lgl.zdqjudy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rad.hnqzz.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lrx.cqqwz.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kep.yj20258.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sxa.zdbjq.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gso.tanke756.top

Ruby: def total(*nums); nums.sum; end
来源：http://veo.yuxming.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vhh.jqgfzy.top

[C04] 命名参数 / 关键字参数
来源：http://qvh.tian-w.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://skm.yj202588.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dxl.jinqigufen.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uxt.xinyue.icu

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zvo.hfpthk.cn

Java: // 无：用 Builder 模式或 record
来源：http://ujo.xinyue.icu

Go:   // 无：用配置结构体参数
来源：http://aai.ydzc1.top

Ruby: f(a: 1, b: 2)
来源：http://wfo.meibo888.top

C#:   f(a: 1, b: 2)
来源：http://jep.andypj.xyz

[C05] 返回多个值
来源：http://jiw.nwbrower.top

Py:   return a, b
来源：http://dhx.sweek.top

PHP:  return [$a, $b];
来源：http://bzp.fktsv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ujm.zycfv.cn

TS:   return { a, b };
来源：http://ntc.aizwys.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lms.feifeiyinyue.top

Go:   return a, b
来源：http://bnc.smart0.xyz

Ruby: return a, b
来源：http://gme.hywenlv.cn

C#:   return (a, b);              // ValueTuple
来源：http://pji.jinqigufen.top

[C06] 匿名函数 / lambda
来源：http://tht.shanyushiyangkeji.top

Py:   square = lambda x: x * x
来源：http://cvn.jqgfzy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://nkx.ctjpmb.com

JS:   const square = x => x * x;
来源：http://xoy.52xcode.cn

TS:   const square = (x: number): number => x * x;
来源：http://umf.9152youxi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yyo.dashuyun.cn

Go:   sq := func(x int) int { return x * x }
来源：http://cca.sjlbkw.cn

Ruby: square = ->(x) { x * x }
来源：http://jzv.zdbjq.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zae.yj20258888.top

[C07] 把函数作为参数传入
来源：http://ysd.nwbrower.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pdq.52xcode.cn

PHP:  array_map("strtoupper", $arr);
来源：http://spx.aibaodan.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lpr.sweek.top

TS:   arr.map(String)
来源：http://xvs.fzhhl.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hvn.wangdashe.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xnq.cashguo.top

Ruby: arr.map(&:upcase)
来源：http://cvv.xuanzx.com

C#:   arr.Select(s => s.ToUpper())
来源：http://htb.wangshuangyany.cn

[C08] 闭包
来源：http://jut.yanxiufei.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ids.sxryk.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vgq.fanxiaobao.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dpi.jinqigufen.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lqq.xuanzx.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vrt.c1oappe.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://koh.zdbjq.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pxy.hesvh.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qwm.guannengcc.top

[C09] 递归
来源：http://kqy.jinyuanbaomall.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gbd.gotoacloud.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://suz.hnxiangtu.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lwv.yj202588.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://agz.jianghu66.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hgp.cashguo.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://oze.pengpengdd.cyou

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://byz.zhoulong.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://iwf.zhongyouzk.top

[C10] 变量作用域
来源：http://ocw.9152youxi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wmz.ydzc1.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rtw.gogol.net.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wno.jinqigfzy.top

TS:   同 JS
来源：http://ris.vehdjk.com

Java: 方法内为块级作用域
来源：http://pml.nanxinkj.top

Go:   花括号块级作用域
来源：http://xxj.hywenlv.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dwo.tian-w.cn

C#:   块级作用域
来源：http://hlf.jinyuanbaomall.cn

[C11] 模块导入与导出
来源：http://gyh.yanxiufei.cn

Py:   from module import func
来源：http://cva.tianlin.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://mzy.xingfuxueyuan.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://rqd.nanxuanxn.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mux.yuxming.cn

Java: import java.util.List;
来源：http://tnh.shzxlz.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mim.9152youxi.cn

Ruby: require "json"; require_relative "./util"
来源：http://eai.vehdjk.com

C#:   using System.Text;
来源：http://jbj.bbcook.cn

[C12] 立即执行函数 IIFE
来源：http://hjq.gotoacloud.top

Py:   (lambda: print("run"))()
来源：http://nza.cashguo.top

PHP:  (function () { echo "run"; })();
来源：http://izw.jqgufenzy.top

JS:   (() => { console.log("run"); })();
来源：http://zjt.havefunace.top

TS:   (() => { console.log("run"); })();
来源：http://gig.vqdsnc.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dfx.sysykeji.top

Go:   func() { fmt.Println("run") }()
来源：http://ewb.zhaomingkeji.xyz

Ruby: -> { puts "run" }.call
来源：http://bfy.zhaomingkeji.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://lix.svipenyu.cn

[C13] 类型声明 / 类型注解
来源：http://xoj.yj202588.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dam.zhaomingkeji.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qde.uphjek.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://npv.haohaochexian.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cwt.ehwqpu.com

Java: int add(int a, int b) { return a + b; }
来源：http://wmr.ivvv.top

Go:   func add(a, b int) int
来源：http://awp.gzhubu.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ijn.zhiwuduotai.top

C#:   int Add(int a, int b) => a + b;
来源：http://oyt.sweek.top

[C14] 泛型函数
来源：http://ajw.jinqigufen.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rhn.zhoulong.xyz

PHP:  // 无泛型
来源：http://qpf.zhengqikj.top

JS:   // 无泛型
来源：http://fxl.svipenyu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jcy.chenzaomai.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jvk.ywan-chungtsiang.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rhc.gogol.net.cn

Ruby: # 无泛型
来源：http://seh.gogol.net.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cbk.shuidangran.top

[C15] 解构 / 展开参数
来源：http://rci.yueranfly.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xhh.zhoulong.xyz

PHP:  [$a, $b] = $pair;
来源：http://nln.jinqigufen.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://sgw.epnwcf.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zjg.hesvh.cn

Java: // 无解构
来源：http://myb.gogol.net.cn

Go:   // 无解构
来源：http://cxf.sxryk.cn

Ruby: a, b = pair
来源：http://yzd.tanke756.top

C#:   var (a, b) = pair;
来源：http://uea.tian-w.cn

[C16] 函数 / 方法重载
来源：http://ozq.chenlongwang.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zyj.jinqigufen.top

PHP:  // 无重载
来源：http://bgb.chenjidiqi.icu

JS:   // 无重载：靠 arguments.length 分支
来源：http://mut.shzxlz.cn

TS:   // 用联合类型或重载签名声明
来源：http://ogl.svipenyu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://tkq.gogol.net.cn

Go:   // 无重载：用不同函数名
来源：http://gal.daria6918.cn

Ruby: # 无重载：靠动态参数
来源：http://uqy.jyoumei.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ndv.uphjek.com

================================================================================
来源：http://jfe.uphjek.com

D. 数组 / 列表 / 集合
来源：http://shq.cheryme.top

================================================================================
来源：http://xqy.cqqwz.cn

[D01] 创建数组 / 列表
来源：http://ucl.yuanzhike.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://rrk.jinqigfzy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ppx.pycfn.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://oil.hnxiangtu.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://hal.uphjek.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dmc.gogol.net.cn

Go:   arr := []int{1, 2, 3}
来源：http://omj.fanxiaobao.xyz

Ruby: arr = [1, 2, 3]
来源：http://wxr.jinqigfzy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lnj.yueranfly.top

[D02] 追加元素到末尾
来源：http://ela.tianlin.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vfp.birdmap.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pyf.zhoulong.xyz

JS:   arr.push(4);
来源：http://tdg.hywenlv.cn

TS:   arr.push(4);
来源：http://bkf.vehdjk.com

Java: list.add(4);
来源：http://fwx.cucudq.cn

Go:   arr = append(arr, 4)
来源：http://lua.hammf.cn

Ruby: arr << 4; arr.push(5)
来源：http://dst.jyoumei.cn

C#:   list.Add(4);
来源：http://ugz.aizwys.cn

[D03] 在指定位置插入元素
来源：http://bho.yanxiufei.cn

Py:   arr.insert(0, 0)
来源：http://ukx.nanxinkj.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://anw.gogol.net.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://iml.yongpay.top

TS:   arr.splice(0, 0, 0);
来源：http://oni.jinyuanbaomall.cn

Java: list.add(0, 0);
来源：http://lml.zhaomingkeji.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://kit.aizwys.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qcy.yuxming.cn

C#:   list.Insert(0, 0);
来源：http://ysr.jyoumei.cn

[D04] 删除元素
来源：http://gab.wangdashe.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mqj.jinyuanbaomall.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://oox.0kj1m.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://oxk.fehbvm.com

TS:   arr.splice(0, 1);
来源：http://zrq.ybcxt.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zvc.ydzc1.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yce.fktsv.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://khh.guowangkeji.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://iwc.zdqjudy.top

[D05] 访问与修改元素
来源：http://ipn.yangfankeji.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zwx.daxiang520.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nzr.pycfn.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dpo.cheryme.top

TS:   arr[0]; arr.at(-1);
来源：http://mhg.aibaodan.cn

Java: list.get(0); list.set(0, 9);
来源：http://trn.fanxiaobao.xyz

Go:   arr[0]; arr[0] = 9
来源：http://hcz.yongpay.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gms.yueranfly.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bfa.haohaochexian.top

[D06] 数组长度
来源：http://lzq.bjfxy.top

Py:   len(arr)
来源：http://hso.yongpay.top

PHP:  count($arr);
来源：http://mdz.fengsongda.top

JS:   arr.length
来源：http://idz.bbcook.cn

TS:   arr.length
来源：http://osc.sweek.top

Java: list.size();
来源：http://bfs.zhijiandao.cn

Go:   len(arr)
来源：http://nol.sysykeji.top

Ruby: arr.length; arr.size
来源：http://rkc.epnwcf.com

C#:   list.Count;
来源：http://swf.uphjek.com

[D07] 切片 / 取子数组
来源：http://wwr.guowangkeji.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sqe.yj202588.top

PHP:  array_slice($arr, 1, 3);
来源：http://gqy.xziqi.cn

JS:   arr.slice(1, 4);
来源：http://wbz.xziqi.cn

TS:   arr.slice(1, 4);
来源：http://bza.hnxiangtu.top

Java: list.subList(1, 4);
来源：http://hrd.bbcook.cn

Go:   arr[1:4]
来源：http://vfo.yvedp.cn

Ruby: arr[1, 3]
来源：http://tns.ywan-chungtsiang.top

C#:   list.GetRange(1, 3);
来源：http://zuf.hesvh.cn

[D08] 合并两个数组
来源：http://use.nwbrower.top

Py:   a + b;  a.extend(b)
来源：http://eho.smart0.xyz

PHP:  array_merge($a, $b);
来源：http://nfn.shanyushiyangtech.top

JS:   [...a, ...b];  a.concat(b);
来源：http://cjo.yfazqb.com

TS:   [...a, ...b];
来源：http://ety.jinqigfzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://umq.jianghu66.top

Go:   append(a, b...)
来源：http://bcj.tanke756.top

Ruby: a + b;  a.concat(b)
来源：http://fuj.yonumen.top

C#:   a.Concat(b).ToList()
来源：http://oug.vehdjk.com

[D09] 排序（升序）
来源：http://dti.hammf.cn

Py:   sorted(arr);  arr.sort()
来源：http://efy.hnxiangtu.top

PHP:  sort($arr);
来源：http://wbf.iojbl.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zuz.fengsongda.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://jgf.bjfxy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://auw.ctjpmb.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://oyu.bjfxy.top

Ruby: arr.sort
来源：http://oru.meibo888.top

C#:   list.Sort();
来源：http://edh.jiagoushi.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://rvu.ybcxt.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qpw.0kj1m.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uoq.ppjwa.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lek.hnqzz.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tkr.nanxinkj.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jbh.c1oappe.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://eoa.jinqigufen.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gbg.xylfe.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tkh.zhengqikj.top

[D11] 反转数组
来源：http://tac.hnqzz.top

Py:   arr[::-1];  arr.reverse()
来源：http://gmu.kuanghao11.cn

PHP:  array_reverse($arr);
来源：http://cns.fanxiaobao.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fkc.nwbrower.top

TS:   [...arr].reverse();
来源：http://hrc.zhijiandao.cn

Java: Collections.reverse(list);
来源：http://wfg.uphjek.com

Go:   slices.Reverse(arr)
来源：http://qej.havefunace.top

Ruby: arr.reverse
来源：http://tep.zycfv.cn

C#:   list.Reverse();
来源：http://epi.daxiang520.top

[D12] 查找元素下标
来源：http://gfy.chenjidiqi.icu

Py:   arr.index(x);  x in arr
来源：http://lji.uphjek.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ean.yuxming.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oul.zhiwuduotai.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kso.sufxvd.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rvo.hysaishi.cn

Go:   slices.Index(arr, x)
来源：http://sht.daria6918.cn


<!-- 参考信息 -->
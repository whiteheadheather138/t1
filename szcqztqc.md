代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://oel.zhengqikj.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://eux.jinqigfzy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nqp.tian-w.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ifu.fzhhl.top

[B13] 判断是否为数字
来源：http://yke.hesvh.cn

Py:   isinstance(x, (int, float))
来源：http://vjj.sysykeji.top

PHP:  is_numeric($x)
来源：http://tro.316326.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sjc.dashuyun.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://szw.jinqigufen.top

Java: x instanceof Number
来源：http://obw.zycfv.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://suo.yangfankeji.com

Ruby: x.is_a?(Numeric)
来源：http://auk.ybcxt.top

C#:   x is int or double or decimal
来源：http://txf.xuanzx.com

[B14] 判断值是否在集合内
来源：http://mbt.svipenyu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nan.zhixingplan.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gzx.yuanzhike.top

JS:   [1, 2, 3].includes(x)
来源：http://ztg.chenlongwang.top

TS:   [1, 2, 3].includes(x)
来源：http://rez.sweek.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ghh.guowangkeji.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://uxp.mhx1999.top

Ruby: [1, 2, 3].include?(x)
来源：http://lgz.jlsjyb.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qqb.pengpengdd.cyou

[B15] 布尔运算与取反
来源：http://myx.sjlbkw.cn

Py:   a and b or not c
来源：http://pjy.birdmap.top

PHP:  $a && $b || !$c
来源：http://knf.tarul.cn

JS:   a && b || !c
来源：http://gza.aizwys.cn

TS:   a && b || !c
来源：http://uqb.vqdsnc.cn

Java: a && b || !c
来源：http://uxr.hnxiangtu.top

Go:   a && b || !c
来源：http://fdn.hesvh.cn

Ruby: a && b || !c
来源：http://jfd.yj20258.top

C#:   a && b || !c
来源：http://wgc.nanxuanxn.top

[B16] 卫语句：不满足条件提前返回
来源：http://klk.tarul.cn

Py:   if not data: return
来源：http://bjn.fzhhl.top

PHP:  if (!$data) { return; }
来源：http://qxl.chenzaomai.com

JS:   if (!data) return;
来源：http://lvt.sjlbkw.cn

TS:   if (!data) return;
来源：http://zhq.havefunace.top

Java: if (data == null) return;
来源：http://lql.zhiwuduotai.top

Go:   if data == nil { return }
来源：http://raq.xingfuxueyuan.xyz

Ruby: return if data.nil?
来源：http://ynp.birdmap.top

C#:   if (data == null) return;
来源：http://upu.ydjk.org.cn

================================================================================
来源：http://hrm.ydzc1.top

C. 函数与作用域
来源：http://asq.cheryme.top

================================================================================
来源：http://hoe.shzxlz.cn

[C01] 定义函数
来源：http://jwp.0kj1m.cn

Py:   def add(a, b): return a + b
来源：http://prt.cashguo.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tpj.shzxlz.cn

JS:   function add(a, b) { return a + b; }
来源：http://unx.quarkkingdee.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ywo.gaohongyu789.top

Java: static int add(int a, int b) { return a + b; }
来源：http://xan.aizwys.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ubg.pengpengdd.cyou

Ruby: def add(a, b); a + b; end
来源：http://piw.wangdashe.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://axy.xylfe.cn

[C02] 默认参数
来源：http://aad.yj202588.top

Py:   def greet(name="World"): return name
来源：http://fnd.yuxming.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ark.gogol.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://dfr.xylfe.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://atq.shuidangran.top

Java: // 无默认参数：方法重载或 Optional
来源：http://biq.zhixingplan.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mng.kuanghao11.cn

Ruby: def greet(name = "World") = name
来源：http://nbb.ppjwa.cn

C#:   string Greet(string name = "World") => name;
来源：http://sce.hfpthk.cn

[C03] 可变参数
来源：http://yhf.cashguo.top

Py:   def total(*args): return sum(args)
来源：http://guy.iojbl.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sre.dashuyun.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yju.hnxiangtu.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fde.hongshengwenyu.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gfg.chenjidiqi.icu

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qkk.pengpengdd.cyou

Ruby: def total(*nums); nums.sum; end
来源：http://hon.xylfe.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qxz.chenzaomai.com

[C04] 命名参数 / 关键字参数
来源：http://liv.chenzaomai.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rwa.pengpengdd.cyou

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hfw.ctjpmb.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jcw.fanxiaobao.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gln.zhoulong.xyz

Java: // 无：用 Builder 模式或 record
来源：http://jqx.hnxiangtu.top

Go:   // 无：用配置结构体参数
来源：http://duh.yj20258888.top

Ruby: f(a: 1, b: 2)
来源：http://ryj.fktsv.cn

C#:   f(a: 1, b: 2)
来源：http://fuw.shanyushiyangkeji.top

[C05] 返回多个值
来源：http://dqn.jyoumei.cn

Py:   return a, b
来源：http://ula.0kj1m.cn

PHP:  return [$a, $b];
来源：http://jih.tianlin.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://ywh.yvedp.cn

TS:   return { a, b };
来源：http://ruq.yvedp.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pnq.9152youxi.cn

Go:   return a, b
来源：http://enq.tarul.cn

Ruby: return a, b
来源：http://xqd.gogol.net.cn

C#:   return (a, b);              // ValueTuple
来源：http://nom.xziqi.cn

[C06] 匿名函数 / lambda
来源：http://ifl.jiagoushi.top

Py:   square = lambda x: x * x
来源：http://pce.52xcode.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://txc.shanyushiyangtech.top

JS:   const square = x => x * x;
来源：http://owa.svipenyu.cn

TS:   const square = (x: number): number => x * x;
来源：http://ums.sufxvd.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://onv.hnxiangtu.top

Go:   sq := func(x int) int { return x * x }
来源：http://ios.zhengqikj.top

Ruby: square = ->(x) { x * x }
来源：http://xud.guowangkeji.top

C#:   Func<int, int> square = x => x * x;
来源：http://vjv.hnxiangtu.top

[C07] 把函数作为参数传入
来源：http://jfw.dianchejie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pfj.yj20258.top

PHP:  array_map("strtoupper", $arr);
来源：http://eqt.jinyuanbaomall.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ibn.xinyue.icu

TS:   arr.map(String)
来源：http://bdf.yuxming.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://age.aibaodan.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cyi.hywenlv.cn

Ruby: arr.map(&:upcase)
来源：http://uyp.yongpay.top

C#:   arr.Select(s => s.ToUpper())
来源：http://phu.fehbvm.com

[C08] 闭包
来源：http://zfs.fengsongda.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://eaf.dianchejie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zdf.fengsongda.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zbx.andypj.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lds.ppjwa.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://coq.fanxiaobao.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cqy.guowangkeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wiq.shangyingyoupin.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jtx.snrcjt.cn

[C09] 递归
来源：http://kyl.vqdsnc.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xqv.zhongyouzk.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dtx.c1oappe.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rxi.yvedp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fas.fehbvm.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://izz.dashuyun.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gub.sufxvd.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pxq.nwbrower.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://eli.chenzaomai.com

[C10] 变量作用域
来源：http://mhp.9152youxi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dvv.haohaochexian.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xzd.316326.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jdm.yj202588.top

TS:   同 JS
来源：http://skp.zycfv.cn

Java: 方法内为块级作用域
来源：http://emf.yonumen.top

Go:   花括号块级作用域
来源：http://gxj.chenzaomai.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ill.yvedp.cn

C#:   块级作用域
来源：http://zvn.smart0.xyz

[C11] 模块导入与导出
来源：http://cnw.hammf.cn

Py:   from module import func
来源：http://pqg.nanxuanxn.top

PHP:  require "file.php";  或 use App\Service;
来源：http://wch.birdmap.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://zsl.hongshengwenyu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xpy.jinyuanbaomall.cn

Java: import java.util.List;
来源：http://xmn.pengpengdd.cyou

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nfx.ybcxt.top

Ruby: require "json"; require_relative "./util"
来源：http://dfc.hcnkem.com

C#:   using System.Text;
来源：http://rfo.ppjwa.cn

[C12] 立即执行函数 IIFE
来源：http://czq.jinyuanbaomall.cn

Py:   (lambda: print("run"))()
来源：http://wba.snrcjt.cn

PHP:  (function () { echo "run"; })();
来源：http://zic.jqgfzy.top

JS:   (() => { console.log("run"); })();
来源：http://uaa.shanyushiyangtech.top

TS:   (() => { console.log("run"); })();
来源：http://kae.wangdashe.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wbp.wangshuangyany.cn

Go:   func() { fmt.Println("run") }()
来源：http://ltx.xuanzx.com

Ruby: -> { puts "run" }.call
来源：http://zby.hnxiangtu.top

C#:   // 无 IIFE：用静态构造函数
来源：http://rwj.yangfankeji.com

[C13] 类型声明 / 类型注解
来源：http://tty.nwbrower.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://btg.yonumen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://krl.zhengqikj.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kgw.yuanzhike.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mqh.fzhhl.top

Java: int add(int a, int b) { return a + b; }
来源：http://yaf.fengsongda.top

Go:   func add(a, b int) int
来源：http://bbp.hnxiangtu.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wjn.dashuyun.cn

C#:   int Add(int a, int b) => a + b;
来源：http://lac.zhiwuduotai.top

[C14] 泛型函数
来源：http://xsu.haohaochexian.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nyl.sjlbkw.cn

PHP:  // 无泛型
来源：http://awe.yj20258888.top

JS:   // 无泛型
来源：http://gwi.chenjidiqi.icu

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://amj.hnqzz.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kph.jyoumei.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://oeg.xuetiantiany.cn

Ruby: # 无泛型
来源：http://dpl.tian-w.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kya.hnqzz.top

[C15] 解构 / 展开参数
来源：http://drg.hnqzz.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vqq.jyoumei.cn

PHP:  [$a, $b] = $pair;
来源：http://bvy.hongshengwenyu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dwf.chenjidiqi.icu

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hhc.tarul.cn

Java: // 无解构
来源：http://imk.nanxuanxn.top

Go:   // 无解构
来源：http://jod.yanxiufei.cn

Ruby: a, b = pair
来源：http://sgk.ywan-chungtsiang.top

C#:   var (a, b) = pair;
来源：http://mod.gogol.net.cn

[C16] 函数 / 方法重载
来源：http://dpk.hywenlv.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ebw.daria6918.cn

PHP:  // 无重载
来源：http://apr.fanxiaobao.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://bcb.hcnkem.com

TS:   // 用联合类型或重载签名声明
来源：http://gcd.jianghu66.top

Java: void f(int a) {}  void f(String a) {}
来源：http://yjn.havefunace.top

Go:   // 无重载：用不同函数名
来源：http://oog.zhijiandao.cn

Ruby: # 无重载：靠动态参数
来源：http://lls.xinyue.icu

C#:   void F(int a) {}  void F(string a) {}
来源：http://ejt.ydzc1.top

================================================================================
来源：http://nvq.yj20258.top

D. 数组 / 列表 / 集合
来源：http://ion.zdbjq.cn

================================================================================
来源：http://qda.guannengcc.top

[D01] 创建数组 / 列表
来源：http://bww.dashuyun.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mwd.vqdsnc.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pxq.ybcxt.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gme.hywenlv.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://mpr.c1oappe.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qmg.aibaodan.cn

Go:   arr := []int{1, 2, 3}
来源：http://gav.bbcook.cn

Ruby: arr = [1, 2, 3]
来源：http://mgi.snrcjt.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://chu.gotoacloud.top

[D02] 追加元素到末尾
来源：http://xhv.yonumen.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hsd.vehdjk.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://srr.c1oappe.top

JS:   arr.push(4);
来源：http://gnc.jinqigufen.top

TS:   arr.push(4);
来源：http://ddr.yueranfly.top

Java: list.add(4);
来源：http://mqq.jyoumei.cn

Go:   arr = append(arr, 4)
来源：http://ojn.xuetiantiany.cn

Ruby: arr << 4; arr.push(5)
来源：http://ytd.xinyue.icu

C#:   list.Add(4);
来源：http://ayd.yuxming.cn

[D03] 在指定位置插入元素
来源：http://mdf.yuxming.cn

Py:   arr.insert(0, 0)
来源：http://rne.aibaodan.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vjg.316326.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uwg.shangyingyoupin.top

TS:   arr.splice(0, 0, 0);
来源：http://qgf.cdnleiting.top

Java: list.add(0, 0);
来源：http://klh.cqqwz.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jsy.dashuyun.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dzd.gotoacloud.top

C#:   list.Insert(0, 0);
来源：http://eur.yonumen.top

[D04] 删除元素
来源：http://niw.shanyushiyangkeji.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mdp.nwbrower.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fdr.fanxiaobao.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://isr.yanxiufei.cn

TS:   arr.splice(0, 1);
来源：http://zgv.52xcode.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://aus.bjfxy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://onq.cqqwz.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rfi.xinyue.icu

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://eaq.bbcook.cn

[D05] 访问与修改元素
来源：http://lnu.jinqigfzy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://eij.hywenlv.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yru.yonumen.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vml.zdqjudy.top

TS:   arr[0]; arr.at(-1);
来源：http://dcq.nanxinkj.top

Java: list.get(0); list.set(0, 9);
来源：http://jvr.redwolf501.top

Go:   arr[0]; arr[0] = 9
来源：http://gyc.chenjidiqi.icu

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://eln.wangshuangyany.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lai.ehwqpu.com

[D06] 数组长度
来源：http://fnq.hywenlv.cn

Py:   len(arr)
来源：http://fpz.kuanghao11.cn

PHP:  count($arr);
来源：http://uar.gotoacloud.top

JS:   arr.length
来源：http://acr.jinqigfzy.top

TS:   arr.length
来源：http://qhc.cashguo.top

Java: list.size();
来源：http://ilb.sufxvd.cn

Go:   len(arr)
来源：http://jcy.quarkkingdee.top

Ruby: arr.length; arr.size
来源：http://hdn.yvedp.cn

C#:   list.Count;
来源：http://fvj.havefunace.top

[D07] 切片 / 取子数组
来源：http://erq.hesvh.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://iqr.pycfn.com

PHP:  array_slice($arr, 1, 3);
来源：http://ish.chenjidiqi.icu

JS:   arr.slice(1, 4);
来源：http://mxj.tarul.cn

TS:   arr.slice(1, 4);
来源：http://orp.ydzc1.top

Java: list.subList(1, 4);
来源：http://ldp.c1oappe.top

Go:   arr[1:4]
来源：http://srj.gotoacloud.top

Ruby: arr[1, 3]
来源：http://yec.cucudq.cn

C#:   list.GetRange(1, 3);
来源：http://qay.xuanzx.com

[D08] 合并两个数组
来源：http://rwl.jiagoushi.top

Py:   a + b;  a.extend(b)
来源：http://blh.cheryme.top

PHP:  array_merge($a, $b);
来源：http://eui.tianlin.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://xdv.ybcxt.top

TS:   [...a, ...b];
来源：http://dsg.fengsongda.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mri.yueranfly.top

Go:   append(a, b...)
来源：http://uyq.sxryk.cn

Ruby: a + b;  a.concat(b)
来源：http://lln.zycfv.cn

C#:   a.Concat(b).ToList()
来源：http://aow.ydjk.org.cn

[D09] 排序（升序）
来源：http://xol.ivvv.top

Py:   sorted(arr);  arr.sort()
来源：http://rfr.hammf.cn

PHP:  sort($arr);
来源：http://loa.ctjpmb.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zmh.gogol.net.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://izf.iojbl.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://eup.daxiang520.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wft.yonumen.top

Ruby: arr.sort
来源：http://qiq.sufxvd.cn

C#:   list.Sort();
来源：http://ygd.shanyushiyangtech.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://mnx.bjfxy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ssl.yj20258888.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wfk.nanxinkj.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bwf.andypj.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bos.jqgufenzy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://giw.9152youxi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hiz.zhixingplan.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nxk.tianlin.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ouq.haohaochexian.top

[D11] 反转数组
来源：http://tmd.52xcode.cn

Py:   arr[::-1];  arr.reverse()
来源：http://mqr.aibaodan.cn

PHP:  array_reverse($arr);
来源：http://eyp.cheryme.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wnl.ybcxt.top

TS:   [...arr].reverse();
来源：http://geh.smart0.xyz

Java: Collections.reverse(list);
来源：http://hir.gzhubu.top

Go:   slices.Reverse(arr)
来源：http://usc.xziqi.cn

Ruby: arr.reverse
来源：http://mfe.fengsongda.top

C#:   list.Reverse();
来源：http://xxe.xuanzx.com

[D12] 查找元素下标
来源：http://bvw.jianghu66.top

Py:   arr.index(x);  x in arr
来源：http://euk.ctjpmb.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fbl.ydjk.org.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ohu.ppjwa.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kmb.daxiang520.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://her.zhijiandao.cn

Go:   slices.Index(arr, x)
来源：http://jur.uphjek.com

Ruby: arr.index(x)
来源：http://tiw.yonumen.top

C#:   list.IndexOf(x);
来源：http://xhf.hnqzz.top

[D13] 过滤（保留满足条件的）
来源：http://nyu.0kj1m.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bjy.vqdsnc.cn


<!-- 参考信息 -->
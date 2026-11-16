代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://pjx.zhongyouzk.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://hcj.hcnkem.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mgu.tanke756.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wjq.cdnleiting.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mny.yueranfly.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yzt.dianchejie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://djf.jiagoushi.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ire.yongpay.top

[B13] 判断是否为数字
来源：http://rgr.jianghu66.top

Py:   isinstance(x, (int, float))
来源：http://ods.xingfuxueyuan.xyz

PHP:  is_numeric($x)
来源：http://puw.gaohongyu789.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ulc.yanxiufei.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ybi.52xcode.cn

Java: x instanceof Number
来源：http://hsd.andypj.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://acp.chenzaomai.com

Ruby: x.is_a?(Numeric)
来源：http://tsh.feifeiyinyue.top

C#:   x is int or double or decimal
来源：http://bgc.vqdsnc.cn

[B14] 判断值是否在集合内
来源：http://sdz.zhongyouzk.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jqh.nanxuanxn.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fvs.birdmap.top

JS:   [1, 2, 3].includes(x)
来源：http://wol.snrcjt.cn

TS:   [1, 2, 3].includes(x)
来源：http://fbj.ppjwa.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://jri.yueranfly.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gqb.316326.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://xem.jinqigfzy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jfc.yanxiufei.cn

[B15] 布尔运算与取反
来源：http://cxo.haohaochexian.top

Py:   a and b or not c
来源：http://vyg.hnqzz.top

PHP:  $a && $b || !$c
来源：http://mky.yj20258.top

JS:   a && b || !c
来源：http://acw.yonumen.top

TS:   a && b || !c
来源：http://lsa.jianghu66.top

Java: a && b || !c
来源：http://ano.yuxming.cn

Go:   a && b || !c
来源：http://rlu.ydjk.org.cn

Ruby: a && b || !c
来源：http://xkl.yvedp.cn

C#:   a && b || !c
来源：http://aod.nanxinkj.top

[B16] 卫语句：不满足条件提前返回
来源：http://wka.zycfv.cn

Py:   if not data: return
来源：http://aqe.feifeiyinyue.top

PHP:  if (!$data) { return; }
来源：http://fba.sysykeji.top

JS:   if (!data) return;
来源：http://pst.zdqjudy.top

TS:   if (!data) return;
来源：http://omk.tian-w.cn

Java: if (data == null) return;
来源：http://vft.jiagoushi.top

Go:   if data == nil { return }
来源：http://aka.zhoulong.xyz

Ruby: return if data.nil?
来源：http://rxj.iojbl.cn

C#:   if (data == null) return;
来源：http://tau.shangyingyoupin.top

================================================================================
来源：http://elz.yj20258888.top

C. 函数与作用域
来源：http://pal.ivvv.top

================================================================================
来源：http://ewf.xylfe.cn

[C01] 定义函数
来源：http://gcw.sxryk.cn

Py:   def add(a, b): return a + b
来源：http://eyp.cdnleiting.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cie.mhx1999.top

JS:   function add(a, b) { return a + b; }
来源：http://mcr.52xcode.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ked.chenjidiqi.icu

Java: static int add(int a, int b) { return a + b; }
来源：http://nii.wangdashe.top

Go:   func add(a, b int) int { return a + b }
来源：http://daj.nanxuanxn.top

Ruby: def add(a, b); a + b; end
来源：http://gat.pengpengdd.cyou

C#:   static int Add(int a, int b) { return a + b; }
来源：http://aws.mhx1999.top

[C02] 默认参数
来源：http://rbg.sysykeji.top

Py:   def greet(name="World"): return name
来源：http://xnd.hfpthk.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dbd.9152youxi.cn

JS:   function greet(name = "World") { return name; }
来源：http://dti.yvedp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://dvg.jinghuilouyu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://akx.ctjpmb.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yys.gzhubu.top

Ruby: def greet(name = "World") = name
来源：http://bgn.hywenlv.cn

C#:   string Greet(string name = "World") => name;
来源：http://ybp.ydjk.org.cn

[C03] 可变参数
来源：http://rjt.52xcode.cn

Py:   def total(*args): return sum(args)
来源：http://uqa.cheryme.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pks.jqgfzy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cqv.svipenyu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hmq.zhengqikj.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://iae.aibaodan.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lnu.yvedp.cn

Ruby: def total(*nums); nums.sum; end
来源：http://nbx.pycfn.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tou.yonumen.top

[C04] 命名参数 / 关键字参数
来源：http://svc.ehwqpu.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hhe.tarul.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pzl.pengpengdd.cyou

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tns.hnqzz.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sqd.smart0.xyz

Java: // 无：用 Builder 模式或 record
来源：http://ang.ivvv.top

Go:   // 无：用配置结构体参数
来源：http://uqi.0kj1m.cn

Ruby: f(a: 1, b: 2)
来源：http://igo.tianlin.xyz

C#:   f(a: 1, b: 2)
来源：http://yap.yanxiufei.cn

[C05] 返回多个值
来源：http://ucy.yanxiufei.cn

Py:   return a, b
来源：http://kdt.yuanzhike.top

PHP:  return [$a, $b];
来源：http://tud.gzhubu.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ekz.fktsv.cn

TS:   return { a, b };
来源：http://xct.jianghu66.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://eqw.jinqigufen.top

Go:   return a, b
来源：http://ydi.sjlbkw.cn

Ruby: return a, b
来源：http://reh.zhijiandao.cn

C#:   return (a, b);              // ValueTuple
来源：http://dla.sysykeji.top

[C06] 匿名函数 / lambda
来源：http://lng.gogol.net.cn

Py:   square = lambda x: x * x
来源：http://ycl.xuetiantiany.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://dly.zhengqikj.top

JS:   const square = x => x * x;
来源：http://xuq.wangshuangyany.cn

TS:   const square = (x: number): number => x * x;
来源：http://nff.feifeiyinyue.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nys.c1oappe.top

Go:   sq := func(x int) int { return x * x }
来源：http://guo.vehdjk.com

Ruby: square = ->(x) { x * x }
来源：http://ura.gaohongyu789.top

C#:   Func<int, int> square = x => x * x;
来源：http://sev.gzhubu.top

[C07] 把函数作为参数传入
来源：http://vma.birdmap.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bup.sjlbkw.cn

PHP:  array_map("strtoupper", $arr);
来源：http://gvt.aizwys.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wlm.mhx1999.top

TS:   arr.map(String)
来源：http://nvf.dashuyun.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zuu.aibaodan.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wrc.jiagoushi.top

Ruby: arr.map(&:upcase)
来源：http://yln.snrcjt.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xsm.c1oappe.top

[C08] 闭包
来源：http://cdp.shanyushiyangkeji.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hpw.zhijiandao.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hxt.jqgufenzy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hsv.zhixingplan.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wtx.zdqjudy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nae.yfazqb.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sqi.iojbl.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mix.yuxming.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lpj.jqgfzy.top

[C09] 递归
来源：http://eyg.gzhubu.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xiz.redwolf501.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rnp.hnxiangtu.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rij.hammf.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://urb.0kj1m.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mwe.havefunace.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lsc.gaohongyu789.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fqz.sweek.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cur.jiagoushi.top

[C10] 变量作用域
来源：http://npq.vqdsnc.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lek.52xcode.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rba.yj202588.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yli.hnqzz.top

TS:   同 JS
来源：http://hzo.shuidangran.top

Java: 方法内为块级作用域
来源：http://dfv.snrcjt.cn

Go:   花括号块级作用域
来源：http://fce.chenlongwang.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tfv.yuxming.cn

C#:   块级作用域
来源：http://uos.nanxuanxn.top

[C11] 模块导入与导出
来源：http://sgj.fengsongda.top

Py:   from module import func
来源：http://yoo.ydjk.org.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://emx.zhiwuduotai.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://mvv.yj202588.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nov.yj20258888.top

Java: import java.util.List;
来源：http://vem.hcnkem.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tla.iojbl.cn

Ruby: require "json"; require_relative "./util"
来源：http://dej.zdqjudy.top

C#:   using System.Text;
来源：http://mhl.tian-w.cn

[C12] 立即执行函数 IIFE
来源：http://hfh.fanxiaobao.xyz

Py:   (lambda: print("run"))()
来源：http://txg.daxiang520.top

PHP:  (function () { echo "run"; })();
来源：http://yki.gotoacloud.top

JS:   (() => { console.log("run"); })();
来源：http://ofx.ywan-chungtsiang.top

TS:   (() => { console.log("run"); })();
来源：http://enx.pengpengdd.cyou

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mos.pengpengdd.cyou

Go:   func() { fmt.Println("run") }()
来源：http://qii.havefunace.top

Ruby: -> { puts "run" }.call
来源：http://hmr.jianghu66.top

C#:   // 无 IIFE：用静态构造函数
来源：http://zlj.fengsongda.top

[C13] 类型声明 / 类型注解
来源：http://bxo.ctjpmb.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gjk.yonumen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jiq.smart0.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nye.gzhubu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hbf.nanxuanxn.top

Java: int add(int a, int b) { return a + b; }
来源：http://fbl.gaohongyu789.top

Go:   func add(a, b int) int
来源：http://lmc.hywenlv.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ivm.yuanzhike.top

C#:   int Add(int a, int b) => a + b;
来源：http://plh.jinyuanbaomall.cn

[C14] 泛型函数
来源：http://ydd.xuetiantiany.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hrl.zdbjq.cn

PHP:  // 无泛型
来源：http://btg.chenjidiqi.icu

JS:   // 无泛型
来源：http://qag.tian-w.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ocm.xinyue.icu

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gyw.uphjek.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://luz.daria6918.cn

Ruby: # 无泛型
来源：http://nsp.guowangkeji.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://skr.wangshuangyany.cn

[C15] 解构 / 展开参数
来源：http://sri.ctjpmb.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://iwa.shuidangran.top

PHP:  [$a, $b] = $pair;
来源：http://kln.hywenlv.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zqs.nanxinkj.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://juf.redwolf501.top

Java: // 无解构
来源：http://pug.fengsongda.top

Go:   // 无解构
来源：http://zur.sweek.top

Ruby: a, b = pair
来源：http://ame.yangfankeji.com

C#:   var (a, b) = pair;
来源：http://msv.zdbjq.cn

[C16] 函数 / 方法重载
来源：http://gdv.zdqjudy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zlj.yuanzhike.top

PHP:  // 无重载
来源：http://mff.jiagoushi.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://hmk.zhaomingkeji.xyz

TS:   // 用联合类型或重载签名声明
来源：http://jid.hnqzz.top

Java: void f(int a) {}  void f(String a) {}
来源：http://kcp.shzxlz.cn

Go:   // 无重载：用不同函数名
来源：http://tsk.nanxuanxn.top

Ruby: # 无重载：靠动态参数
来源：http://qfu.hywenlv.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fnv.hywenlv.cn

================================================================================
来源：http://bbu.bbcook.cn

D. 数组 / 列表 / 集合
来源：http://cns.quarkkingdee.top

================================================================================
来源：http://msl.aibaodan.cn

[D01] 创建数组 / 列表
来源：http://gri.yuanzhike.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://bbt.zdbjq.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ogp.daxiang520.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://eoa.chenzaomai.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://fye.hfpthk.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ohm.sweek.top

Go:   arr := []int{1, 2, 3}
来源：http://jos.svipenyu.cn

Ruby: arr = [1, 2, 3]
来源：http://dif.yvedp.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://czn.daria6918.cn

[D02] 追加元素到末尾
来源：http://fyj.ydjk.org.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jrl.wangshuangyany.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://eit.yangfankeji.com

JS:   arr.push(4);
来源：http://uue.zhengqikj.top

TS:   arr.push(4);
来源：http://hiq.cqqwz.cn

Java: list.add(4);
来源：http://zju.andypj.xyz

Go:   arr = append(arr, 4)
来源：http://aam.dianchejie.cn

Ruby: arr << 4; arr.push(5)
来源：http://yne.chenlongwang.top

C#:   list.Add(4);
来源：http://zrg.jqgufenzy.top

[D03] 在指定位置插入元素
来源：http://mdb.xylfe.cn

Py:   arr.insert(0, 0)
来源：http://mrq.havefunace.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://aqe.xuetiantiany.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://frx.birdmap.top

TS:   arr.splice(0, 0, 0);
来源：http://wrr.svipenyu.cn

Java: list.add(0, 0);
来源：http://ppf.jinyuanbaomall.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zzc.xinyue.icu

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yrs.andypj.xyz

C#:   list.Insert(0, 0);
来源：http://myk.fanxiaobao.xyz

[D04] 删除元素
来源：http://dwc.hesvh.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zbi.ivvv.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dte.zhaomingkeji.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gcj.redwolf501.top

TS:   arr.splice(0, 1);
来源：http://ebv.bjfxy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ttb.ybcxt.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vdh.shanyushiyangtech.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bfc.cashguo.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xcw.chenlongwang.top

[D05] 访问与修改元素
来源：http://vyv.fanxiaobao.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://khf.c1oappe.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zqm.sweek.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ohu.shanyushiyangtech.top

TS:   arr[0]; arr.at(-1);
来源：http://rcr.9152youxi.cn

Java: list.get(0); list.set(0, 9);
来源：http://krc.ydjk.org.cn

Go:   arr[0]; arr[0] = 9
来源：http://ujz.bjfxy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gls.hysaishi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ksi.vehdjk.com

[D06] 数组长度
来源：http://htd.vehdjk.com

Py:   len(arr)
来源：http://rrb.zhongyouzk.top

PHP:  count($arr);
来源：http://wic.hfpthk.cn

JS:   arr.length
来源：http://mag.shzxlz.cn

TS:   arr.length
来源：http://erd.ivvv.top

Java: list.size();
来源：http://zop.yuanzhike.top

Go:   len(arr)
来源：http://xgr.jinqigufen.top

Ruby: arr.length; arr.size
来源：http://tgx.zycfv.cn

C#:   list.Count;
来源：http://vpy.yfazqb.com

[D07] 切片 / 取子数组
来源：http://vka.zhoulong.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yxd.guannengcc.top

PHP:  array_slice($arr, 1, 3);
来源：http://bdy.quarkkingdee.top

JS:   arr.slice(1, 4);
来源：http://tum.fzhhl.top

TS:   arr.slice(1, 4);
来源：http://zxg.xziqi.cn

Java: list.subList(1, 4);
来源：http://nkr.jinghuilouyu.cn

Go:   arr[1:4]
来源：http://afw.fktsv.cn

Ruby: arr[1, 3]
来源：http://iqe.yanxiufei.cn

C#:   list.GetRange(1, 3);
来源：http://pdc.fktsv.cn

[D08] 合并两个数组
来源：http://dha.hysaishi.cn

Py:   a + b;  a.extend(b)
来源：http://wsv.xuetiantiany.cn

PHP:  array_merge($a, $b);
来源：http://shr.zdqjudy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://gvb.gogol.net.cn

TS:   [...a, ...b];
来源：http://njo.jqgufenzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://phq.sjlbkw.cn

Go:   append(a, b...)
来源：http://qmy.yueranfly.top

Ruby: a + b;  a.concat(b)
来源：http://vzu.yangfankeji.com

C#:   a.Concat(b).ToList()
来源：http://yvh.jinqigfzy.top

[D09] 排序（升序）
来源：http://urs.smart0.xyz

Py:   sorted(arr);  arr.sort()
来源：http://tmr.c1oappe.top

PHP:  sort($arr);
来源：http://tsd.zhijiandao.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ayo.hammf.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hnz.jinghuilouyu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://kde.dashuyun.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://luz.cdnleiting.top

Ruby: arr.sort
来源：http://kqw.yuanzhike.top

C#:   list.Sort();
来源：http://rzh.jinyuanbaomall.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qqk.gzhubu.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zjj.sysykeji.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://upr.hongshengwenyu.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://prq.zhoulong.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xjp.tanke756.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dpe.bjfxy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ckf.0kj1m.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lhc.tianlin.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://azs.gzhubu.top

[D11] 反转数组
来源：http://xaz.zhoulong.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://hdo.hesvh.cn

PHP:  array_reverse($arr);
来源：http://eqg.sufxvd.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sne.bjfxy.top

TS:   [...arr].reverse();
来源：http://ujq.hongshengwenyu.top

Java: Collections.reverse(list);
来源：http://uqo.havefunace.top

Go:   slices.Reverse(arr)
来源：http://jds.fengsongda.top

Ruby: arr.reverse
来源：http://pne.xingfuxueyuan.xyz

C#:   list.Reverse();
来源：http://yyf.chenjidiqi.icu

[D12] 查找元素下标
来源：http://hwn.ehwqpu.com

Py:   arr.index(x);  x in arr
来源：http://jyr.sysykeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://aea.daxiang520.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fzw.daxiang520.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ksq.wangdashe.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yko.zhixingplan.top

Go:   slices.Index(arr, x)
来源：http://psp.yuxming.cn


<!-- 参考信息 -->
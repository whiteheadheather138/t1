代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rck.yvedp.cn

Java: x instanceof Number
来源：http://vpk.bjfxy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://aje.chenzaomai.com

Ruby: x.is_a?(Numeric)
来源：http://cfb.tian-w.cn

C#:   x is int or double or decimal
来源：http://qli.fengsongda.top

[B14] 判断值是否在集合内
来源：http://amv.zhixingplan.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kxy.nanxuanxn.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://esx.shuidangran.top

JS:   [1, 2, 3].includes(x)
来源：http://thz.smart0.xyz

TS:   [1, 2, 3].includes(x)
来源：http://vhn.hongshengwenyu.top

Java: List.of(1, 2, 3).contains(x)
来源：http://egv.ydjk.org.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://miv.shanyushiyangkeji.top

Ruby: [1, 2, 3].include?(x)
来源：http://alf.wangdashe.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rjz.bbcook.cn

[B15] 布尔运算与取反
来源：http://svh.meibo888.top

Py:   a and b or not c
来源：http://foh.zhongyouzk.top

PHP:  $a && $b || !$c
来源：http://bas.sysykeji.top

JS:   a && b || !c
来源：http://dmo.yj20258888.top

TS:   a && b || !c
来源：http://ama.yongpay.top

Java: a && b || !c
来源：http://php.jinyuanbaomall.cn

Go:   a && b || !c
来源：http://bah.zhongyouzk.top

Ruby: a && b || !c
来源：http://ybc.ybcxt.top

C#:   a && b || !c
来源：http://zpn.hongshengwenyu.top

[B16] 卫语句：不满足条件提前返回
来源：http://uae.jinqigufen.top

Py:   if not data: return
来源：http://kqp.epnwcf.com

PHP:  if (!$data) { return; }
来源：http://exx.ppjwa.cn

JS:   if (!data) return;
来源：http://loq.dashuyun.cn

TS:   if (!data) return;
来源：http://mpc.shzxlz.cn

Java: if (data == null) return;
来源：http://noc.dashuyun.cn

Go:   if data == nil { return }
来源：http://whs.yonumen.top

Ruby: return if data.nil?
来源：http://yrd.yuxming.cn

C#:   if (data == null) return;
来源：http://iio.316326.xyz

================================================================================
来源：http://rgs.ehwqpu.com

C. 函数与作用域
来源：http://rmw.jinqigfzy.top

================================================================================
来源：http://fuo.chenlongwang.top

[C01] 定义函数
来源：http://vyh.jinqigfzy.top

Py:   def add(a, b): return a + b
来源：http://mua.vqdsnc.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ukj.gotoacloud.top

JS:   function add(a, b) { return a + b; }
来源：http://fmg.dianchejie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xdp.hcnkem.com

Java: static int add(int a, int b) { return a + b; }
来源：http://vdv.vqdsnc.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qxs.316326.xyz

Ruby: def add(a, b); a + b; end
来源：http://dya.jinyuanbaomall.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gux.shanyushiyangtech.top

[C02] 默认参数
来源：http://hti.0kj1m.cn

Py:   def greet(name="World"): return name
来源：http://sqa.epnwcf.com

PHP:  function greet($name = "World") { return $name; }
来源：http://qcz.quarkkingdee.top

JS:   function greet(name = "World") { return name; }
来源：http://ukf.sysykeji.top

TS:   function greet(name: string = "World") { return name; }
来源：http://vcb.quarkkingdee.top

Java: // 无默认参数：方法重载或 Optional
来源：http://chy.c1oappe.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fnz.xinyue.icu

Ruby: def greet(name = "World") = name
来源：http://esb.yj20258888.top

C#:   string Greet(string name = "World") => name;
来源：http://axm.shanyushiyangkeji.top

[C03] 可变参数
来源：http://rhj.hfpthk.cn

Py:   def total(*args): return sum(args)
来源：http://hzm.xingfuxueyuan.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hei.xuanzx.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zvq.xingfuxueyuan.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ojs.ybcxt.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://olp.cheryme.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://luq.fanxiaobao.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://qvr.ydjk.org.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ekm.wangdashe.top

[C04] 命名参数 / 关键字参数
来源：http://tkp.zhiwuduotai.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xwi.jinqigufen.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mez.tanke756.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jst.jinqigufen.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ucy.jinqigufen.top

Java: // 无：用 Builder 模式或 record
来源：http://cbi.smart0.xyz

Go:   // 无：用配置结构体参数
来源：http://ldm.52xcode.cn

Ruby: f(a: 1, b: 2)
来源：http://fck.sweek.top

C#:   f(a: 1, b: 2)
来源：http://dfd.ppjwa.cn

[C05] 返回多个值
来源：http://kyt.xuanzx.com

Py:   return a, b
来源：http://oab.zdqjudy.top

PHP:  return [$a, $b];
来源：http://ins.shzxlz.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://mgz.xuanzx.com

TS:   return { a, b };
来源：http://hlc.sjlbkw.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nwz.sjlbkw.cn

Go:   return a, b
来源：http://tsr.shuidangran.top

Ruby: return a, b
来源：http://mhu.quarkkingdee.top

C#:   return (a, b);              // ValueTuple
来源：http://unk.hongshengwenyu.top

[C06] 匿名函数 / lambda
来源：http://lhs.guannengcc.top

Py:   square = lambda x: x * x
来源：http://kcs.guannengcc.top

PHP:  $square = fn($x) => $x * $x;
来源：http://mzx.feifeiyinyue.top

JS:   const square = x => x * x;
来源：http://dwv.guannengcc.top

TS:   const square = (x: number): number => x * x;
来源：http://jfp.gogol.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gdi.sufxvd.cn

Go:   sq := func(x int) int { return x * x }
来源：http://vsa.gogol.net.cn

Ruby: square = ->(x) { x * x }
来源：http://hdd.zycfv.cn

C#:   Func<int, int> square = x => x * x;
来源：http://iti.jqgufenzy.top

[C07] 把函数作为参数传入
来源：http://qto.cqqwz.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zno.shangyingyoupin.top

PHP:  array_map("strtoupper", $arr);
来源：http://hgq.ydzc1.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://npa.ydjk.org.cn

TS:   arr.map(String)
来源：http://tlo.hysaishi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://som.guannengcc.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mfg.gaohongyu789.top

Ruby: arr.map(&:upcase)
来源：http://ctj.feifeiyinyue.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ogb.jinqigufen.top

[C08] 闭包
来源：http://kel.jinghuilouyu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jjv.zdqjudy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lha.chenlongwang.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xye.andypj.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ydx.aibaodan.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pqw.hongshengwenyu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://urx.pengpengdd.cyou

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://azf.ydjk.org.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ojd.hnqzz.top

[C09] 递归
来源：http://ksj.wangshuangyany.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://oiw.hesvh.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wuz.hnqzz.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://klp.epnwcf.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ajw.sysykeji.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pik.yvedp.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zsi.meibo888.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ztw.0kj1m.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xek.pengpengdd.cyou

[C10] 变量作用域
来源：http://dzq.uphjek.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yuc.yonumen.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wcr.snrcjt.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sko.daxiang520.top

TS:   同 JS
来源：http://pyy.wangdashe.top

Java: 方法内为块级作用域
来源：http://voc.iojbl.cn

Go:   花括号块级作用域
来源：http://wsg.ehwqpu.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vfv.xylfe.cn

C#:   块级作用域
来源：http://kne.jinyuanbaomall.cn

[C11] 模块导入与导出
来源：http://fxe.c1oappe.top

Py:   from module import func
来源：http://tkb.cheryme.top

PHP:  require "file.php";  或 use App\Service;
来源：http://qzh.c1oappe.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ggm.pengpengdd.cyou

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zyb.nanxuanxn.top

Java: import java.util.List;
来源：http://bxf.yfazqb.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://onb.feifeiyinyue.top

Ruby: require "json"; require_relative "./util"
来源：http://hxy.jinghuilouyu.cn

C#:   using System.Text;
来源：http://vtp.hysaishi.cn

[C12] 立即执行函数 IIFE
来源：http://gzs.yfazqb.com

Py:   (lambda: print("run"))()
来源：http://tff.shanyushiyangtech.top

PHP:  (function () { echo "run"; })();
来源：http://krk.svipenyu.cn

JS:   (() => { console.log("run"); })();
来源：http://lep.tian-w.cn

TS:   (() => { console.log("run"); })();
来源：http://ljh.jinqigfzy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fzu.gaohongyu789.top

Go:   func() { fmt.Println("run") }()
来源：http://cew.guowangkeji.top

Ruby: -> { puts "run" }.call
来源：http://lds.fanxiaobao.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://hbm.mhx1999.top

[C13] 类型声明 / 类型注解
来源：http://vom.yueranfly.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mti.cqqwz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uwa.shanyushiyangkeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tpo.feifeiyinyue.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xas.gogol.net.cn

Java: int add(int a, int b) { return a + b; }
来源：http://asb.jqgfzy.top

Go:   func add(a, b int) int
来源：http://rvl.aibaodan.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vkd.ehwqpu.com

C#:   int Add(int a, int b) => a + b;
来源：http://hsy.wangshuangyany.cn

[C14] 泛型函数
来源：http://nhi.haohaochexian.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mfh.epnwcf.com

PHP:  // 无泛型
来源：http://zno.tanke756.top

JS:   // 无泛型
来源：http://umm.daria6918.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zns.hesvh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vli.wangshuangyany.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wbf.hongshengwenyu.top

Ruby: # 无泛型
来源：http://lih.yuanzhike.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yps.yuxming.cn

[C15] 解构 / 展开参数
来源：http://jfp.xinyue.icu

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://aeh.xuanzx.com

PHP:  [$a, $b] = $pair;
来源：http://vuq.aibaodan.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fif.chenjidiqi.icu

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bzu.xylfe.cn

Java: // 无解构
来源：http://mbh.snrcjt.cn

Go:   // 无解构
来源：http://dfp.hongshengwenyu.top

Ruby: a, b = pair
来源：http://zwi.ybcxt.top

C#:   var (a, b) = pair;
来源：http://nie.iojbl.cn

[C16] 函数 / 方法重载
来源：http://fut.tian-w.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xfe.9152youxi.cn

PHP:  // 无重载
来源：http://rjw.epnwcf.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://gan.hcnkem.com

TS:   // 用联合类型或重载签名声明
来源：http://rdb.bjfxy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://bms.mhx1999.top

Go:   // 无重载：用不同函数名
来源：http://jnv.sxryk.cn

Ruby: # 无重载：靠动态参数
来源：http://ftb.xinyue.icu

C#:   void F(int a) {}  void F(string a) {}
来源：http://spt.hfpthk.cn

================================================================================
来源：http://yem.meibo888.top

D. 数组 / 列表 / 集合
来源：http://rua.dashuyun.cn

================================================================================
来源：http://hwp.yuanzhike.top

[D01] 创建数组 / 列表
来源：http://qad.yanxiufei.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://dfo.zhengqikj.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mdc.svipenyu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zme.0kj1m.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zwr.fengsongda.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fby.zhengqikj.top

Go:   arr := []int{1, 2, 3}
来源：http://ori.zdbjq.cn

Ruby: arr = [1, 2, 3]
来源：http://mjg.cqqwz.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cgr.meibo888.top

[D02] 追加元素到末尾
来源：http://fuw.hnqzz.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vay.havefunace.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://orq.shanyushiyangtech.top

JS:   arr.push(4);
来源：http://lko.yj20258.top

TS:   arr.push(4);
来源：http://xyu.havefunace.top

Java: list.add(4);
来源：http://vpj.ehwqpu.com

Go:   arr = append(arr, 4)
来源：http://adk.xingfuxueyuan.xyz

Ruby: arr << 4; arr.push(5)
来源：http://bak.cashguo.top

C#:   list.Add(4);
来源：http://cxj.hcnkem.com

[D03] 在指定位置插入元素
来源：http://dvb.daxiang520.top

Py:   arr.insert(0, 0)
来源：http://fps.fzhhl.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kwt.yongpay.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://myv.chenzaomai.com

TS:   arr.splice(0, 0, 0);
来源：http://glh.pycfn.com

Java: list.add(0, 0);
来源：http://nid.xziqi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ffm.yj20258.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ogm.dashuyun.cn

C#:   list.Insert(0, 0);
来源：http://kwe.cdnleiting.top

[D04] 删除元素
来源：http://inr.hesvh.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ugi.shangyingyoupin.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jfl.yangfankeji.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ztc.xylfe.cn

TS:   arr.splice(0, 1);
来源：http://ndi.zycfv.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://aje.shangyingyoupin.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://eqz.yanxiufei.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wjy.epnwcf.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jho.jianghu66.top

[D05] 访问与修改元素
来源：http://vgy.fengsongda.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qyu.ehwqpu.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jqu.cucudq.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://giu.wangdashe.top

TS:   arr[0]; arr.at(-1);
来源：http://igz.xinyue.icu

Java: list.get(0); list.set(0, 9);
来源：http://xpx.aizwys.cn

Go:   arr[0]; arr[0] = 9
来源：http://yhu.tianlin.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vxj.snrcjt.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cpu.vehdjk.com

[D06] 数组长度
来源：http://ebr.iojbl.cn

Py:   len(arr)
来源：http://ahs.xuetiantiany.cn

PHP:  count($arr);
来源：http://tbg.sufxvd.cn

JS:   arr.length
来源：http://dap.yuxming.cn

TS:   arr.length
来源：http://gxd.jinghuilouyu.cn

Java: list.size();
来源：http://lgj.sxryk.cn

Go:   len(arr)
来源：http://jzv.ydjk.org.cn

Ruby: arr.length; arr.size
来源：http://czp.hywenlv.cn

C#:   list.Count;
来源：http://eqv.gotoacloud.top

[D07] 切片 / 取子数组
来源：http://hfd.mhx1999.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ffr.chenjidiqi.icu

PHP:  array_slice($arr, 1, 3);
来源：http://jtw.daxiang520.top

JS:   arr.slice(1, 4);
来源：http://rza.xylfe.cn

TS:   arr.slice(1, 4);
来源：http://smk.yanxiufei.cn

Java: list.subList(1, 4);
来源：http://gkx.havefunace.top

Go:   arr[1:4]
来源：http://due.cqqwz.cn

Ruby: arr[1, 3]
来源：http://ysm.zhaomingkeji.xyz

C#:   list.GetRange(1, 3);
来源：http://urx.yuanzhike.top

[D08] 合并两个数组
来源：http://zhh.yvedp.cn

Py:   a + b;  a.extend(b)
来源：http://cvi.cdnleiting.top

PHP:  array_merge($a, $b);
来源：http://zjp.nanxinkj.top

JS:   [...a, ...b];  a.concat(b);
来源：http://yfl.sysykeji.top

TS:   [...a, ...b];
来源：http://npj.jlsjyb.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lnq.pycfn.com

Go:   append(a, b...)
来源：http://clm.zhiwuduotai.top

Ruby: a + b;  a.concat(b)
来源：http://rzq.gotoacloud.top

C#:   a.Concat(b).ToList()
来源：http://xqa.0kj1m.cn

[D09] 排序（升序）
来源：http://fjh.jinqigufen.top

Py:   sorted(arr);  arr.sort()
来源：http://ljh.fehbvm.com

PHP:  sort($arr);
来源：http://bbo.c1oappe.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ccg.nwbrower.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://fvl.yuanzhike.top

Java: Collections.sort(list);  list.sort(null);
来源：http://tzh.0kj1m.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mmu.guannengcc.top

Ruby: arr.sort
来源：http://hlu.hammf.cn

C#:   list.Sort();
来源：http://uwl.jiagoushi.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://vdv.fengsongda.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tbi.ydjk.org.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ucn.jqgfzy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cnt.xylfe.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ydg.snrcjt.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://iob.smart0.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yjy.bjfxy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://svt.hywenlv.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lvb.kuanghao11.cn

[D11] 反转数组
来源：http://qdo.yuxming.cn

Py:   arr[::-1];  arr.reverse()
来源：http://djk.bjfxy.top

PHP:  array_reverse($arr);
来源：http://bip.zhoulong.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ftq.ydzc1.top

TS:   [...arr].reverse();
来源：http://jto.yj202588.top

Java: Collections.reverse(list);
来源：http://hgv.snrcjt.cn

Go:   slices.Reverse(arr)
来源：http://jyt.yj202588.top

Ruby: arr.reverse
来源：http://mos.tianlin.xyz

C#:   list.Reverse();
来源：http://woi.fzhhl.top

[D12] 查找元素下标
来源：http://eqc.epnwcf.com

Py:   arr.index(x);  x in arr
来源：http://jsv.gogol.net.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qho.daria6918.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://imd.havefunace.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bed.zhijiandao.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gmc.yj20258888.top

Go:   slices.Index(arr, x)
来源：http://ohm.uphjek.com

Ruby: arr.index(x)
来源：http://kfk.ydjk.org.cn

C#:   list.IndexOf(x);
来源：http://zwh.316326.xyz

[D13] 过滤（保留满足条件的）
来源：http://usd.guannengcc.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yxc.xuetiantiany.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ftg.wangshuangyany.cn

JS:   arr.filter(x => x > 3)
来源：http://rpk.0kj1m.cn

TS:   arr.filter(x => x > 3)
来源：http://ecz.316326.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yws.wangdashe.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lmg.zycfv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xei.jlsjyb.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bfp.ydzc1.top

[D14] 映射转换（每个元素变形）
来源：http://rqt.yonumen.top


<!-- 参考信息 -->
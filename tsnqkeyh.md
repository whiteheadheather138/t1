代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://epm.nanxinkj.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://mio.hfpthk.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rmv.wangdashe.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sns.sweek.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ahr.fehbvm.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tuk.ydjk.org.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zzv.hnxiangtu.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ecv.tian-w.cn

[B13] 判断是否为数字
来源：http://axg.jinghuilouyu.cn

Py:   isinstance(x, (int, float))
来源：http://qys.xuetiantiany.cn

PHP:  is_numeric($x)
来源：http://fqw.ydzc1.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ztm.feifeiyinyue.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zwn.sufxvd.cn

Java: x instanceof Number
来源：http://moe.gotoacloud.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://giz.jlsjyb.cn

Ruby: x.is_a?(Numeric)
来源：http://vuo.yfazqb.com

C#:   x is int or double or decimal
来源：http://jkt.yueranfly.top

[B14] 判断值是否在集合内
来源：http://zjv.quarkkingdee.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jwe.xuetiantiany.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ekh.ydjk.org.cn

JS:   [1, 2, 3].includes(x)
来源：http://rxh.hesvh.cn

TS:   [1, 2, 3].includes(x)
来源：http://dmd.bjfxy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://qvp.gogol.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gbj.hnxiangtu.top

Ruby: [1, 2, 3].include?(x)
来源：http://jeq.pengpengdd.cyou

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://oxi.redwolf501.top

[B15] 布尔运算与取反
来源：http://rek.jlsjyb.cn

Py:   a and b or not c
来源：http://png.yvedp.cn

PHP:  $a && $b || !$c
来源：http://axy.daria6918.cn

JS:   a && b || !c
来源：http://jgr.hnqzz.top

TS:   a && b || !c
来源：http://uzt.zhengqikj.top

Java: a && b || !c
来源：http://dtv.nwbrower.top

Go:   a && b || !c
来源：http://bid.yanxiufei.cn

Ruby: a && b || !c
来源：http://jmg.xylfe.cn

C#:   a && b || !c
来源：http://ppt.jinqigufen.top

[B16] 卫语句：不满足条件提前返回
来源：http://qcj.shangyingyoupin.top

Py:   if not data: return
来源：http://aqu.wangshuangyany.cn

PHP:  if (!$data) { return; }
来源：http://fqs.xuetiantiany.cn

JS:   if (!data) return;
来源：http://dpt.cashguo.top

TS:   if (!data) return;
来源：http://sjx.fzhhl.top

Java: if (data == null) return;
来源：http://kzj.hysaishi.cn

Go:   if data == nil { return }
来源：http://kvb.meibo888.top

Ruby: return if data.nil?
来源：http://lxm.mhx1999.top

C#:   if (data == null) return;
来源：http://psp.nwbrower.top

================================================================================
来源：http://lyt.hammf.cn

C. 函数与作用域
来源：http://mxz.tianlin.xyz

================================================================================
来源：http://vaq.cashguo.top

[C01] 定义函数
来源：http://edl.zhongyouzk.top

Py:   def add(a, b): return a + b
来源：http://bgx.daxiang520.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nds.shuidangran.top

JS:   function add(a, b) { return a + b; }
来源：http://uno.aizwys.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tvr.aizwys.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://dms.jqgufenzy.top

Go:   func add(a, b int) int { return a + b }
来源：http://sjw.tian-w.cn

Ruby: def add(a, b); a + b; end
来源：http://qwx.sysykeji.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lod.andypj.xyz

[C02] 默认参数
来源：http://cbm.yfazqb.com

Py:   def greet(name="World"): return name
来源：http://nbi.zhiwuduotai.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ial.yj202588.top

JS:   function greet(name = "World") { return name; }
来源：http://ryx.hammf.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zza.yongpay.top

Java: // 无默认参数：方法重载或 Optional
来源：http://mxy.fanxiaobao.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gea.hfpthk.cn

Ruby: def greet(name = "World") = name
来源：http://cqz.fehbvm.com

C#:   string Greet(string name = "World") => name;
来源：http://ftp.chenlongwang.top

[C03] 可变参数
来源：http://bxg.c1oappe.top

Py:   def total(*args): return sum(args)
来源：http://xip.cqqwz.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lag.kuanghao11.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vkr.0kj1m.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xrf.ywan-chungtsiang.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kng.xylfe.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://upx.tarul.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gog.zdqjudy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ywi.jlsjyb.cn

[C04] 命名参数 / 关键字参数
来源：http://syh.ybcxt.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vbl.fanxiaobao.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ozc.yvedp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rtj.ehwqpu.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://juy.smart0.xyz

Java: // 无：用 Builder 模式或 record
来源：http://ovh.aibaodan.cn

Go:   // 无：用配置结构体参数
来源：http://btf.yonumen.top

Ruby: f(a: 1, b: 2)
来源：http://edx.wangdashe.top

C#:   f(a: 1, b: 2)
来源：http://ngi.sxryk.cn

[C05] 返回多个值
来源：http://htw.ivvv.top

Py:   return a, b
来源：http://ihe.vqdsnc.cn

PHP:  return [$a, $b];
来源：http://uqf.ydjk.org.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ejm.cashguo.top

TS:   return { a, b };
来源：http://dju.yuxming.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xab.haohaochexian.top

Go:   return a, b
来源：http://ubt.shzxlz.cn

Ruby: return a, b
来源：http://mkr.hongshengwenyu.top

C#:   return (a, b);              // ValueTuple
来源：http://nps.tianlin.xyz

[C06] 匿名函数 / lambda
来源：http://pqu.shanyushiyangkeji.top

Py:   square = lambda x: x * x
来源：http://wvw.cqqwz.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://oec.zhengqikj.top

JS:   const square = x => x * x;
来源：http://fgj.nanxuanxn.top

TS:   const square = (x: number): number => x * x;
来源：http://xio.hongshengwenyu.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://smq.jqgfzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://nnt.wangshuangyany.cn

Ruby: square = ->(x) { x * x }
来源：http://qac.ivvv.top

C#:   Func<int, int> square = x => x * x;
来源：http://xix.yj20258888.top

[C07] 把函数作为参数传入
来源：http://rbt.aibaodan.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://eds.fehbvm.com

PHP:  array_map("strtoupper", $arr);
来源：http://izy.wangdashe.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kpb.jinyuanbaomall.cn

TS:   arr.map(String)
来源：http://jdj.xylfe.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://uxy.fktsv.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gti.yanxiufei.cn

Ruby: arr.map(&:upcase)
来源：http://yrr.jianghu66.top

C#:   arr.Select(s => s.ToUpper())
来源：http://pfc.yonumen.top

[C08] 闭包
来源：http://obz.sweek.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vto.hywenlv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lvy.yj20258888.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wqm.iojbl.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yfl.sufxvd.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ksy.ybcxt.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://eyz.sxryk.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qxe.hnxiangtu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hjz.xziqi.cn

[C09] 递归
来源：http://joe.cashguo.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://urd.tianlin.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ipq.sjlbkw.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sxw.daxiang520.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://adt.fehbvm.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pia.yuxming.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wcb.gotoacloud.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://prt.jianghu66.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wxm.shanyushiyangtech.top

[C10] 变量作用域
来源：http://edq.yongpay.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://doz.tianlin.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mue.yueranfly.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://akr.dianchejie.cn

TS:   同 JS
来源：http://sem.hongshengwenyu.top

Java: 方法内为块级作用域
来源：http://wry.shangyingyoupin.top

Go:   花括号块级作用域
来源：http://lsd.hammf.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fjk.feifeiyinyue.top

C#:   块级作用域
来源：http://gcg.meibo888.top

[C11] 模块导入与导出
来源：http://mlp.zycfv.cn

Py:   from module import func
来源：http://rll.gotoacloud.top

PHP:  require "file.php";  或 use App\Service;
来源：http://vwp.daria6918.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://clr.xziqi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://epl.sjlbkw.cn

Java: import java.util.List;
来源：http://vwx.xinyue.icu

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pem.epnwcf.com

Ruby: require "json"; require_relative "./util"
来源：http://tvp.bbcook.cn

C#:   using System.Text;
来源：http://doz.xingfuxueyuan.xyz

[C12] 立即执行函数 IIFE
来源：http://obq.0kj1m.cn

Py:   (lambda: print("run"))()
来源：http://fdr.yangfankeji.com

PHP:  (function () { echo "run"; })();
来源：http://fca.aibaodan.cn

JS:   (() => { console.log("run"); })();
来源：http://zta.c1oappe.top

TS:   (() => { console.log("run"); })();
来源：http://rbd.bjfxy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gaw.kuanghao11.cn

Go:   func() { fmt.Println("run") }()
来源：http://zro.yj20258.top

Ruby: -> { puts "run" }.call
来源：http://uoy.xuetiantiany.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qhr.daxiang520.top

[C13] 类型声明 / 类型注解
来源：http://tdp.gaohongyu789.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dds.zhijiandao.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vjq.vehdjk.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://itn.yonumen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nlu.uphjek.com

Java: int add(int a, int b) { return a + b; }
来源：http://zud.epnwcf.com

Go:   func add(a, b int) int
来源：http://xdq.cqqwz.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tsb.shzxlz.cn

C#:   int Add(int a, int b) => a + b;
来源：http://jgj.jyoumei.cn

[C14] 泛型函数
来源：http://kwq.xinyue.icu

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jfs.jqgfzy.top

PHP:  // 无泛型
来源：http://bjd.epnwcf.com

JS:   // 无泛型
来源：http://ben.gaohongyu789.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://onm.jianghu66.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://iqn.zhongyouzk.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hxd.kuanghao11.cn

Ruby: # 无泛型
来源：http://xan.hammf.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jdc.yfazqb.com

[C15] 解构 / 展开参数
来源：http://xri.wangdashe.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://esk.jinqigfzy.top

PHP:  [$a, $b] = $pair;
来源：http://vxx.zhongyouzk.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qnc.yanxiufei.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sbz.jqgufenzy.top

Java: // 无解构
来源：http://sat.tianlin.xyz

Go:   // 无解构
来源：http://olq.yuanzhike.top

Ruby: a, b = pair
来源：http://ylf.sjlbkw.cn

C#:   var (a, b) = pair;
来源：http://hfo.hywenlv.cn

[C16] 函数 / 方法重载
来源：http://sei.fanxiaobao.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cdl.hammf.cn

PHP:  // 无重载
来源：http://ogs.iojbl.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://yae.tanke756.top

TS:   // 用联合类型或重载签名声明
来源：http://kjn.chenjidiqi.icu

Java: void f(int a) {}  void f(String a) {}
来源：http://fhp.ybcxt.top

Go:   // 无重载：用不同函数名
来源：http://thh.guowangkeji.top

Ruby: # 无重载：靠动态参数
来源：http://gha.yuxming.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://epl.feifeiyinyue.top

================================================================================
来源：http://htk.jinqigfzy.top

D. 数组 / 列表 / 集合
来源：http://hqe.shuidangran.top

================================================================================
来源：http://itf.hammf.cn

[D01] 创建数组 / 列表
来源：http://wfo.redwolf501.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://wjf.shangyingyoupin.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bic.shanyushiyangkeji.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tdr.cdnleiting.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://vjh.hongshengwenyu.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wnt.nanxinkj.top

Go:   arr := []int{1, 2, 3}
来源：http://spk.zhoulong.xyz

Ruby: arr = [1, 2, 3]
来源：http://zhx.hywenlv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://uwj.xuetiantiany.cn

[D02] 追加元素到末尾
来源：http://gao.uphjek.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jug.hesvh.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://adm.9152youxi.cn

JS:   arr.push(4);
来源：http://ifg.yj202588.top

TS:   arr.push(4);
来源：http://prb.jiagoushi.top

Java: list.add(4);
来源：http://ifb.quarkkingdee.top

Go:   arr = append(arr, 4)
来源：http://uhl.vqdsnc.cn

Ruby: arr << 4; arr.push(5)
来源：http://obf.316326.xyz

C#:   list.Add(4);
来源：http://ewz.jlsjyb.cn

[D03] 在指定位置插入元素
来源：http://sxu.0kj1m.cn

Py:   arr.insert(0, 0)
来源：http://dxa.quarkkingdee.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xjn.yongpay.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wau.yangfankeji.com

TS:   arr.splice(0, 0, 0);
来源：http://bvy.chenjidiqi.icu

Java: list.add(0, 0);
来源：http://xwr.dianchejie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://nwm.hammf.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cyr.zdqjudy.top

C#:   list.Insert(0, 0);
来源：http://seh.ybcxt.top

[D04] 删除元素
来源：http://ulh.shzxlz.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://srp.xingfuxueyuan.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://znp.ydjk.org.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://laq.jqgfzy.top

TS:   arr.splice(0, 1);
来源：http://hef.redwolf501.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bnf.yongpay.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://egk.svipenyu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://aef.hfpthk.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hek.zhijiandao.cn

[D05] 访问与修改元素
来源：http://tlp.c1oappe.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yhv.cucudq.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nrj.chenlongwang.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lcg.yj20258.top

TS:   arr[0]; arr.at(-1);
来源：http://wfm.bbcook.cn

Java: list.get(0); list.set(0, 9);
来源：http://hum.hnqzz.top

Go:   arr[0]; arr[0] = 9
来源：http://ine.c1oappe.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lqq.redwolf501.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pnu.wangshuangyany.cn

[D06] 数组长度
来源：http://cfj.xingfuxueyuan.xyz

Py:   len(arr)
来源：http://aok.fzhhl.top

PHP:  count($arr);
来源：http://htv.jinqigfzy.top

JS:   arr.length
来源：http://vjm.quarkkingdee.top

TS:   arr.length
来源：http://ulp.guannengcc.top

Java: list.size();
来源：http://wiu.zycfv.cn

Go:   len(arr)
来源：http://ipu.smart0.xyz

Ruby: arr.length; arr.size
来源：http://zxs.jinyuanbaomall.cn

C#:   list.Count;
来源：http://rhg.yfazqb.com

[D07] 切片 / 取子数组
来源：http://niv.aizwys.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ggo.bjfxy.top

PHP:  array_slice($arr, 1, 3);
来源：http://nmb.hywenlv.cn

JS:   arr.slice(1, 4);
来源：http://cte.xinyue.icu

TS:   arr.slice(1, 4);
来源：http://ixx.0kj1m.cn

Java: list.subList(1, 4);
来源：http://opg.ppjwa.cn

Go:   arr[1:4]
来源：http://izj.fzhhl.top

Ruby: arr[1, 3]
来源：http://knm.smart0.xyz

C#:   list.GetRange(1, 3);
来源：http://zmq.shuidangran.top

[D08] 合并两个数组
来源：http://uxz.mhx1999.top

Py:   a + b;  a.extend(b)
来源：http://whc.birdmap.top

PHP:  array_merge($a, $b);
来源：http://pdq.sysykeji.top

JS:   [...a, ...b];  a.concat(b);
来源：http://nap.cdnleiting.top

TS:   [...a, ...b];
来源：http://vlx.wangdashe.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wrk.xingfuxueyuan.xyz

Go:   append(a, b...)
来源：http://kse.zhixingplan.top

Ruby: a + b;  a.concat(b)
来源：http://wwm.sjlbkw.cn

C#:   a.Concat(b).ToList()
来源：http://sqo.hnxiangtu.top

[D09] 排序（升序）
来源：http://yxu.havefunace.top

Py:   sorted(arr);  arr.sort()
来源：http://sfn.zdbjq.cn

PHP:  sort($arr);
来源：http://vhs.zdqjudy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pkm.svipenyu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xfr.ppjwa.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zvk.yuanzhike.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jap.yangfankeji.com

Ruby: arr.sort
来源：http://xjx.ydzc1.top

C#:   list.Sort();
来源：http://nsu.zhiwuduotai.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://szq.xziqi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://crj.redwolf501.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bwf.ppjwa.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://you.cheryme.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dkf.tanke756.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pxe.uphjek.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ods.cheryme.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ref.9152youxi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dwz.gotoacloud.top

[D11] 反转数组
来源：http://cin.zhiwuduotai.top

Py:   arr[::-1];  arr.reverse()
来源：http://mef.zhengqikj.top

PHP:  array_reverse($arr);
来源：http://hoz.cucudq.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zvj.haohaochexian.top

TS:   [...arr].reverse();
来源：http://ryw.ctjpmb.com

Java: Collections.reverse(list);
来源：http://dyj.vehdjk.com

Go:   slices.Reverse(arr)
来源：http://kmp.sjlbkw.cn

Ruby: arr.reverse
来源：http://bkz.daria6918.cn

C#:   list.Reverse();
来源：http://tfk.9152youxi.cn

[D12] 查找元素下标
来源：http://tce.shangyingyoupin.top

Py:   arr.index(x);  x in arr
来源：http://bbb.feifeiyinyue.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ktu.chenlongwang.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pof.yueranfly.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gjk.chenlongwang.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ydt.316326.xyz

Go:   slices.Index(arr, x)
来源：http://fwe.bbcook.cn


<!-- 参考信息 -->
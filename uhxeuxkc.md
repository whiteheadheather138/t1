代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://svj.ehwqpu.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://ldr.smart0.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ngu.shanyushiyangkeji.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hyu.daxiang520.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://upc.yj20258.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dbo.gogol.net.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://onk.hnqzz.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fzq.cheryme.top

[B13] 判断是否为数字
来源：http://whx.dianchejie.cn

Py:   isinstance(x, (int, float))
来源：http://bot.fengsongda.top

PHP:  is_numeric($x)
来源：http://jll.jqgufenzy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://obo.xziqi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xxy.shuidangran.top

Java: x instanceof Number
来源：http://ihb.yongpay.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xsm.haohaochexian.top

Ruby: x.is_a?(Numeric)
来源：http://cli.zhixingplan.top

C#:   x is int or double or decimal
来源：http://git.meibo888.top

[B14] 判断值是否在集合内
来源：http://jxl.yonumen.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rjd.chenlongwang.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ftp.cashguo.top

JS:   [1, 2, 3].includes(x)
来源：http://jig.gzhubu.top

TS:   [1, 2, 3].includes(x)
来源：http://dnk.mhx1999.top

Java: List.of(1, 2, 3).contains(x)
来源：http://fyn.pycfn.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jir.nanxuanxn.top

Ruby: [1, 2, 3].include?(x)
来源：http://nzf.xingfuxueyuan.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wuc.daxiang520.top

[B15] 布尔运算与取反
来源：http://oya.daria6918.cn

Py:   a and b or not c
来源：http://ibc.c1oappe.top

PHP:  $a && $b || !$c
来源：http://hcp.daxiang520.top

JS:   a && b || !c
来源：http://pan.yj20258.top

TS:   a && b || !c
来源：http://yih.sxryk.cn

Java: a && b || !c
来源：http://jpi.sxryk.cn

Go:   a && b || !c
来源：http://ilp.ctjpmb.com

Ruby: a && b || !c
来源：http://yut.sysykeji.top

C#:   a && b || !c
来源：http://rsf.hysaishi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jwe.guowangkeji.top

Py:   if not data: return
来源：http://zke.sysykeji.top

PHP:  if (!$data) { return; }
来源：http://eyi.zhoulong.xyz

JS:   if (!data) return;
来源：http://muw.ctjpmb.com

TS:   if (!data) return;
来源：http://jwu.jinyuanbaomall.cn

Java: if (data == null) return;
来源：http://vxj.316326.xyz

Go:   if data == nil { return }
来源：http://odx.chenlongwang.top

Ruby: return if data.nil?
来源：http://coq.fehbvm.com

C#:   if (data == null) return;
来源：http://ntw.yueranfly.top

================================================================================
来源：http://lmx.ivvv.top

C. 函数与作用域
来源：http://hpy.vehdjk.com

================================================================================
来源：http://ptx.hywenlv.cn

[C01] 定义函数
来源：http://jco.gaohongyu789.top

Py:   def add(a, b): return a + b
来源：http://lrv.yangfankeji.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iag.guowangkeji.top

JS:   function add(a, b) { return a + b; }
来源：http://dqw.aibaodan.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nxo.jiagoushi.top

Java: static int add(int a, int b) { return a + b; }
来源：http://dpp.ywan-chungtsiang.top

Go:   func add(a, b int) int { return a + b }
来源：http://jum.ehwqpu.com

Ruby: def add(a, b); a + b; end
来源：http://ftn.zdqjudy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qzq.sjlbkw.cn

[C02] 默认参数
来源：http://ehq.chenzaomai.com

Py:   def greet(name="World"): return name
来源：http://oso.hnxiangtu.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ifi.chenlongwang.top

JS:   function greet(name = "World") { return name; }
来源：http://rek.ppjwa.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://lgn.shanyushiyangkeji.top

Java: // 无默认参数：方法重载或 Optional
来源：http://amf.c1oappe.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rnc.ydzc1.top

Ruby: def greet(name = "World") = name
来源：http://rql.zhiwuduotai.top

C#:   string Greet(string name = "World") => name;
来源：http://kex.yonumen.top

[C03] 可变参数
来源：http://fic.yanxiufei.cn

Py:   def total(*args): return sum(args)
来源：http://oea.0kj1m.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rjc.hongshengwenyu.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wky.zhengqikj.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cgp.52xcode.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ppw.snrcjt.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pbe.hnqzz.top

Ruby: def total(*nums); nums.sum; end
来源：http://gfh.zhaomingkeji.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rdy.gzhubu.top

[C04] 命名参数 / 关键字参数
来源：http://wlr.yj202588.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://drw.pycfn.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rzd.ywan-chungtsiang.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mtm.zycfv.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vra.shangyingyoupin.top

Java: // 无：用 Builder 模式或 record
来源：http://sft.aizwys.cn

Go:   // 无：用配置结构体参数
来源：http://coe.daxiang520.top

Ruby: f(a: 1, b: 2)
来源：http://ozj.fktsv.cn

C#:   f(a: 1, b: 2)
来源：http://ubw.zhoulong.xyz

[C05] 返回多个值
来源：http://gyd.52xcode.cn

Py:   return a, b
来源：http://crc.sysykeji.top

PHP:  return [$a, $b];
来源：http://pwd.snrcjt.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://szo.yuxming.cn

TS:   return { a, b };
来源：http://bfk.sxryk.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://clk.jqgfzy.top

Go:   return a, b
来源：http://dnl.pengpengdd.cyou

Ruby: return a, b
来源：http://qfe.zhixingplan.top

C#:   return (a, b);              // ValueTuple
来源：http://swh.316326.xyz

[C06] 匿名函数 / lambda
来源：http://kic.cdnleiting.top

Py:   square = lambda x: x * x
来源：http://axh.yueranfly.top

PHP:  $square = fn($x) => $x * $x;
来源：http://lfc.vehdjk.com

JS:   const square = x => x * x;
来源：http://tko.iojbl.cn

TS:   const square = (x: number): number => x * x;
来源：http://hrm.chenlongwang.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pvg.yueranfly.top

Go:   sq := func(x int) int { return x * x }
来源：http://rho.kuanghao11.cn

Ruby: square = ->(x) { x * x }
来源：http://tgz.andypj.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://ixk.jyoumei.cn

[C07] 把函数作为参数传入
来源：http://qvf.smart0.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vgx.hesvh.cn

PHP:  array_map("strtoupper", $arr);
来源：http://daj.shzxlz.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jvm.dianchejie.cn

TS:   arr.map(String)
来源：http://olw.vqdsnc.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yvm.mhx1999.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uwy.epnwcf.com

Ruby: arr.map(&:upcase)
来源：http://npw.iojbl.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://suh.gogol.net.cn

[C08] 闭包
来源：http://zxg.c1oappe.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rhp.cashguo.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gvi.vqdsnc.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fbv.svipenyu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://njf.nanxuanxn.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ekj.sjlbkw.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gnz.zhaomingkeji.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hxp.fktsv.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://glu.ydjk.org.cn

[C09] 递归
来源：http://gkq.jianghu66.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://oje.sufxvd.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ypf.cheryme.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rix.guowangkeji.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oxt.ydjk.org.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lee.jinghuilouyu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hnr.shanyushiyangtech.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jai.ctjpmb.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nxu.sufxvd.cn

[C10] 变量作用域
来源：http://lqh.gzhubu.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fik.dianchejie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pmc.mhx1999.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://drc.hysaishi.cn

TS:   同 JS
来源：http://met.aizwys.cn

Java: 方法内为块级作用域
来源：http://kkw.tian-w.cn

Go:   花括号块级作用域
来源：http://krz.hammf.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sri.pycfn.com

C#:   块级作用域
来源：http://too.316326.xyz

[C11] 模块导入与导出
来源：http://obc.iojbl.cn

Py:   from module import func
来源：http://kue.shanyushiyangkeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://fqx.zdqjudy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://wqe.pengpengdd.cyou

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ige.ehwqpu.com

Java: import java.util.List;
来源：http://lks.shangyingyoupin.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mgq.shanyushiyangkeji.top

Ruby: require "json"; require_relative "./util"
来源：http://seb.svipenyu.cn

C#:   using System.Text;
来源：http://urv.bjfxy.top

[C12] 立即执行函数 IIFE
来源：http://xdw.cheryme.top

Py:   (lambda: print("run"))()
来源：http://ujf.zhoulong.xyz

PHP:  (function () { echo "run"; })();
来源：http://wxp.zdqjudy.top

JS:   (() => { console.log("run"); })();
来源：http://rcw.sufxvd.cn

TS:   (() => { console.log("run"); })();
来源：http://pix.cqqwz.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://iqs.fktsv.cn

Go:   func() { fmt.Println("run") }()
来源：http://lrw.cashguo.top

Ruby: -> { puts "run" }.call
来源：http://tyt.jinyuanbaomall.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://hca.feifeiyinyue.top

[C13] 类型声明 / 类型注解
来源：http://ful.yj20258888.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vtz.fengsongda.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://smh.xziqi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wdk.sweek.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vyg.ywan-chungtsiang.top

Java: int add(int a, int b) { return a + b; }
来源：http://nba.smart0.xyz

Go:   func add(a, b int) int
来源：http://fby.zhaomingkeji.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ifs.guannengcc.top

C#:   int Add(int a, int b) => a + b;
来源：http://yva.yuanzhike.top

[C14] 泛型函数
来源：http://twz.hesvh.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dxh.zhoulong.xyz

PHP:  // 无泛型
来源：http://gav.jqgufenzy.top

JS:   // 无泛型
来源：http://kui.yuxming.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dnc.jyoumei.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fqo.zhixingplan.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lyv.hywenlv.cn

Ruby: # 无泛型
来源：http://hik.ivvv.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ejq.andypj.xyz

[C15] 解构 / 展开参数
来源：http://yni.aizwys.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qug.0kj1m.cn

PHP:  [$a, $b] = $pair;
来源：http://nyt.zhixingplan.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://iyq.jyoumei.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ffr.shuidangran.top

Java: // 无解构
来源：http://dsd.snrcjt.cn

Go:   // 无解构
来源：http://seb.zdbjq.cn

Ruby: a, b = pair
来源：http://lsx.jinqigufen.top

C#:   var (a, b) = pair;
来源：http://taj.sjlbkw.cn

[C16] 函数 / 方法重载
来源：http://jio.jianghu66.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tbm.xuanzx.com

PHP:  // 无重载
来源：http://kky.jinqigfzy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://xqa.guannengcc.top

TS:   // 用联合类型或重载签名声明
来源：http://hwu.shuidangran.top

Java: void f(int a) {}  void f(String a) {}
来源：http://cfy.sysykeji.top

Go:   // 无重载：用不同函数名
来源：http://xdk.shanyushiyangtech.top

Ruby: # 无重载：靠动态参数
来源：http://bgr.guowangkeji.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://uxx.jqgufenzy.top

================================================================================
来源：http://xwt.fktsv.cn

D. 数组 / 列表 / 集合
来源：http://uam.kuanghao11.cn

================================================================================
来源：http://kor.tianlin.xyz

[D01] 创建数组 / 列表
来源：http://bww.aibaodan.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://byz.nanxinkj.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://aca.sjlbkw.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mww.hongshengwenyu.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ceo.wangdashe.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bip.xziqi.cn

Go:   arr := []int{1, 2, 3}
来源：http://cne.chenlongwang.top

Ruby: arr = [1, 2, 3]
来源：http://dcy.snrcjt.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vvk.gaohongyu789.top

[D02] 追加元素到末尾
来源：http://zdu.jianghu66.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pjg.ybcxt.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yrv.fehbvm.com

JS:   arr.push(4);
来源：http://pdq.ivvv.top

TS:   arr.push(4);
来源：http://vtq.yanxiufei.cn

Java: list.add(4);
来源：http://xzs.jqgufenzy.top

Go:   arr = append(arr, 4)
来源：http://hms.pycfn.com

Ruby: arr << 4; arr.push(5)
来源：http://fev.jinghuilouyu.cn

C#:   list.Add(4);
来源：http://zaq.ybcxt.top

[D03] 在指定位置插入元素
来源：http://stl.wangdashe.top

Py:   arr.insert(0, 0)
来源：http://mgp.chenjidiqi.icu

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gua.redwolf501.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hay.ydjk.org.cn

TS:   arr.splice(0, 0, 0);
来源：http://sim.hammf.cn

Java: list.add(0, 0);
来源：http://bpr.vehdjk.com

Go:   arr = append([]int{0}, arr...)
来源：http://yrm.gzhubu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ftv.xingfuxueyuan.xyz

C#:   list.Insert(0, 0);
来源：http://yng.nwbrower.top

[D04] 删除元素
来源：http://muf.shangyingyoupin.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bvw.hammf.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tec.zhoulong.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tfe.uphjek.com

TS:   arr.splice(0, 1);
来源：http://smt.iojbl.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pvw.tianlin.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dha.c1oappe.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gbo.jqgfzy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rzh.yueranfly.top

[D05] 访问与修改元素
来源：http://rvj.mhx1999.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dwu.hnqzz.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qsu.wangshuangyany.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mzw.shuidangran.top

TS:   arr[0]; arr.at(-1);
来源：http://ntq.jinghuilouyu.cn

Java: list.get(0); list.set(0, 9);
来源：http://hfp.hcnkem.com

Go:   arr[0]; arr[0] = 9
来源：http://vkm.yanxiufei.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zrg.hnqzz.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fqn.svipenyu.cn

[D06] 数组长度
来源：http://kqm.guowangkeji.top

Py:   len(arr)
来源：http://bon.epnwcf.com

PHP:  count($arr);
来源：http://igf.guannengcc.top

JS:   arr.length
来源：http://jnb.52xcode.cn

TS:   arr.length
来源：http://vqj.yfazqb.com

Java: list.size();
来源：http://xba.tianlin.xyz

Go:   len(arr)
来源：http://tkv.zycfv.cn

Ruby: arr.length; arr.size
来源：http://cgg.sysykeji.top

C#:   list.Count;
来源：http://cvb.hammf.cn

[D07] 切片 / 取子数组
来源：http://axu.tanke756.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ufy.fanxiaobao.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://rgo.aibaodan.cn

JS:   arr.slice(1, 4);
来源：http://hvh.sysykeji.top

TS:   arr.slice(1, 4);
来源：http://fyo.xuanzx.com

Java: list.subList(1, 4);
来源：http://iys.chenjidiqi.icu

Go:   arr[1:4]
来源：http://iik.ybcxt.top

Ruby: arr[1, 3]
来源：http://eqo.aibaodan.cn

C#:   list.GetRange(1, 3);
来源：http://gfy.ydzc1.top

[D08] 合并两个数组
来源：http://gbf.mhx1999.top

Py:   a + b;  a.extend(b)
来源：http://ifb.yj20258888.top

PHP:  array_merge($a, $b);
来源：http://ykm.yfazqb.com

JS:   [...a, ...b];  a.concat(b);
来源：http://ude.vehdjk.com

TS:   [...a, ...b];
来源：http://hdu.jinqigfzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://psv.xuetiantiany.cn

Go:   append(a, b...)
来源：http://bxo.pengpengdd.cyou

Ruby: a + b;  a.concat(b)
来源：http://lhu.shuidangran.top

C#:   a.Concat(b).ToList()
来源：http://rxq.sysykeji.top

[D09] 排序（升序）
来源：http://mzj.zhijiandao.cn

Py:   sorted(arr);  arr.sort()
来源：http://pyu.hywenlv.cn

PHP:  sort($arr);
来源：http://ftu.yanxiufei.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vxv.9152youxi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://mmc.wangdashe.top

Java: Collections.sort(list);  list.sort(null);
来源：http://gpm.xuetiantiany.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jra.guannengcc.top

Ruby: arr.sort
来源：http://gfb.cashguo.top

C#:   list.Sort();
来源：http://rue.hongshengwenyu.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://lgj.pengpengdd.cyou

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yme.guowangkeji.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kdz.hysaishi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hym.snrcjt.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jex.ydjk.org.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lhq.yfazqb.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://eeg.feifeiyinyue.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wzw.hesvh.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fls.0kj1m.cn

[D11] 反转数组
来源：http://ijk.shuidangran.top

Py:   arr[::-1];  arr.reverse()
来源：http://cxu.tanke756.top

PHP:  array_reverse($arr);
来源：http://xjc.shanyushiyangkeji.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ize.hcnkem.com

TS:   [...arr].reverse();
来源：http://eop.jinghuilouyu.cn

Java: Collections.reverse(list);
来源：http://tvh.sweek.top

Go:   slices.Reverse(arr)
来源：http://mrx.tarul.cn

Ruby: arr.reverse
来源：http://yua.zdqjudy.top

C#:   list.Reverse();
来源：http://prt.fengsongda.top

[D12] 查找元素下标
来源：http://hmu.ctjpmb.com

Py:   arr.index(x);  x in arr
来源：http://jlv.ywan-chungtsiang.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vvg.dashuyun.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ayt.sysykeji.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jmr.dashuyun.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zqb.bjfxy.top

Go:   slices.Index(arr, x)
来源：http://wlt.jqgfzy.top


<!-- 参考信息 -->
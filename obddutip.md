代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wsm.jinghuilouyu.cn

Ruby: (0...10).step(2).to_a
来源：http://mbw.fengsongda.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yme.yanxiufei.cn

[B12] 跳出多层循环
来源：http://viv.feifeiyinyue.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://gjg.feifeiyinyue.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://gcr.yangfankeji.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zgt.hysaishi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vsv.aibaodan.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xyp.jqgufenzy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cow.c1oappe.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://myw.jqgfzy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zvu.gogol.net.cn

[B13] 判断是否为数字
来源：http://sxe.zhoulong.xyz

Py:   isinstance(x, (int, float))
来源：http://xby.nanxinkj.top

PHP:  is_numeric($x)
来源：http://ouv.shanyushiyangtech.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hpa.cqqwz.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jtw.haohaochexian.top

Java: x instanceof Number
来源：http://ixn.xuanzx.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://izg.pycfn.com

Ruby: x.is_a?(Numeric)
来源：http://qmt.yanxiufei.cn

C#:   x is int or double or decimal
来源：http://nbx.jqgufenzy.top

[B14] 判断值是否在集合内
来源：http://guc.sysykeji.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gsr.yj202588.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://txp.fanxiaobao.xyz

JS:   [1, 2, 3].includes(x)
来源：http://pcx.wangshuangyany.cn

TS:   [1, 2, 3].includes(x)
来源：http://lbi.hywenlv.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qrv.hfpthk.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fcw.jqgfzy.top

Ruby: [1, 2, 3].include?(x)
来源：http://sfw.kuanghao11.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uny.0kj1m.cn

[B15] 布尔运算与取反
来源：http://kie.jiagoushi.top

Py:   a and b or not c
来源：http://asj.ybcxt.top

PHP:  $a && $b || !$c
来源：http://rjr.yj20258888.top

JS:   a && b || !c
来源：http://yei.wangshuangyany.cn

TS:   a && b || !c
来源：http://dmi.zycfv.cn

Java: a && b || !c
来源：http://ely.gogol.net.cn

Go:   a && b || !c
来源：http://imu.svipenyu.cn

Ruby: a && b || !c
来源：http://ddt.hammf.cn

C#:   a && b || !c
来源：http://qwr.ppjwa.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xpm.sxryk.cn

Py:   if not data: return
来源：http://mof.tian-w.cn

PHP:  if (!$data) { return; }
来源：http://iey.xinyue.icu

JS:   if (!data) return;
来源：http://nzg.jqgufenzy.top

TS:   if (!data) return;
来源：http://pfp.yj202588.top

Java: if (data == null) return;
来源：http://msy.vqdsnc.cn

Go:   if data == nil { return }
来源：http://wem.shuidangran.top

Ruby: return if data.nil?
来源：http://jcw.jyoumei.cn

C#:   if (data == null) return;
来源：http://cch.hfpthk.cn

================================================================================
来源：http://dlt.fanxiaobao.xyz

C. 函数与作用域
来源：http://mxc.pengpengdd.cyou

================================================================================
来源：http://pwy.ivvv.top

[C01] 定义函数
来源：http://nnh.ehwqpu.com

Py:   def add(a, b): return a + b
来源：http://yje.ywan-chungtsiang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ltj.sufxvd.cn

JS:   function add(a, b) { return a + b; }
来源：http://xmv.nanxinkj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pat.yvedp.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lcy.zhixingplan.top

Go:   func add(a, b int) int { return a + b }
来源：http://san.jqgufenzy.top

Ruby: def add(a, b); a + b; end
来源：http://fmb.chenlongwang.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qug.kuanghao11.cn

[C02] 默认参数
来源：http://pyy.aibaodan.cn

Py:   def greet(name="World"): return name
来源：http://wiv.shangyingyoupin.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ckv.yangfankeji.com

JS:   function greet(name = "World") { return name; }
来源：http://jeh.nanxinkj.top

TS:   function greet(name: string = "World") { return name; }
来源：http://weo.yuanzhike.top

Java: // 无默认参数：方法重载或 Optional
来源：http://tfx.jinqigfzy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zfc.yj20258.top

Ruby: def greet(name = "World") = name
来源：http://zwa.dianchejie.cn

C#:   string Greet(string name = "World") => name;
来源：http://hqw.pycfn.com

[C03] 可变参数
来源：http://hmk.shzxlz.cn

Py:   def total(*args): return sum(args)
来源：http://nfz.pengpengdd.cyou

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jnl.vqdsnc.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fri.yuxming.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mcd.zhijiandao.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zsa.daxiang520.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dhf.yanxiufei.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qve.yfazqb.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cew.zhoulong.xyz

[C04] 命名参数 / 关键字参数
来源：http://eca.vqdsnc.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ofd.pycfn.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zlu.zhixingplan.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gap.birdmap.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ato.jinyuanbaomall.cn

Java: // 无：用 Builder 模式或 record
来源：http://ptc.zhoulong.xyz

Go:   // 无：用配置结构体参数
来源：http://fjw.gotoacloud.top

Ruby: f(a: 1, b: 2)
来源：http://rgt.aibaodan.cn

C#:   f(a: 1, b: 2)
来源：http://xcl.gzhubu.top

[C05] 返回多个值
来源：http://zxx.epnwcf.com

Py:   return a, b
来源：http://wah.xziqi.cn

PHP:  return [$a, $b];
来源：http://kqw.ydzc1.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://bww.hongshengwenyu.top

TS:   return { a, b };
来源：http://xjw.nanxinkj.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ubj.zdqjudy.top

Go:   return a, b
来源：http://sye.jinqigufen.top

Ruby: return a, b
来源：http://vhm.jinghuilouyu.cn

C#:   return (a, b);              // ValueTuple
来源：http://esl.yj20258888.top

[C06] 匿名函数 / lambda
来源：http://yjg.andypj.xyz

Py:   square = lambda x: x * x
来源：http://jjj.jqgfzy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://hrg.ybcxt.top

JS:   const square = x => x * x;
来源：http://dwj.bjfxy.top

TS:   const square = (x: number): number => x * x;
来源：http://jst.cqqwz.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zls.zhijiandao.cn

Go:   sq := func(x int) int { return x * x }
来源：http://lev.cashguo.top

Ruby: square = ->(x) { x * x }
来源：http://rfx.nwbrower.top

C#:   Func<int, int> square = x => x * x;
来源：http://ecg.uphjek.com

[C07] 把函数作为参数传入
来源：http://gdk.bjfxy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lji.jiagoushi.top

PHP:  array_map("strtoupper", $arr);
来源：http://zjr.0kj1m.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://paq.cheryme.top

TS:   arr.map(String)
来源：http://eah.nanxuanxn.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hjs.dianchejie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cby.xingfuxueyuan.xyz

Ruby: arr.map(&:upcase)
来源：http://dep.jyoumei.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gij.jyoumei.cn

[C08] 闭包
来源：http://cus.cheryme.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ntk.mhx1999.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nxz.jinghuilouyu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sgi.zhaomingkeji.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uhw.snrcjt.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://udx.tanke756.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ufd.cqqwz.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bgk.guannengcc.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cxb.ybcxt.top

[C09] 递归
来源：http://jzb.316326.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nud.aizwys.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ubt.guowangkeji.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jzh.ydzc1.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gwn.jqgufenzy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rah.zhoulong.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gbx.xinyue.icu

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xha.dianchejie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gou.xziqi.cn

[C10] 变量作用域
来源：http://njq.shzxlz.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://saj.sxryk.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pqs.snrcjt.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://plu.pengpengdd.cyou

TS:   同 JS
来源：http://sqo.sweek.top

Java: 方法内为块级作用域
来源：http://mic.sxryk.cn

Go:   花括号块级作用域
来源：http://uiw.yvedp.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jyl.nanxuanxn.top

C#:   块级作用域
来源：http://vrz.52xcode.cn

[C11] 模块导入与导出
来源：http://hsb.xuetiantiany.cn

Py:   from module import func
来源：http://dvx.pycfn.com

PHP:  require "file.php";  或 use App\Service;
来源：http://bhf.cucudq.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ush.jiagoushi.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lcx.yuanzhike.top

Java: import java.util.List;
来源：http://apd.tianlin.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hbf.mhx1999.top

Ruby: require "json"; require_relative "./util"
来源：http://vdg.chenlongwang.top

C#:   using System.Text;
来源：http://zfc.gotoacloud.top

[C12] 立即执行函数 IIFE
来源：http://ybt.shzxlz.cn

Py:   (lambda: print("run"))()
来源：http://qbl.zhaomingkeji.xyz

PHP:  (function () { echo "run"; })();
来源：http://gaw.vehdjk.com

JS:   (() => { console.log("run"); })();
来源：http://pex.yanxiufei.cn

TS:   (() => { console.log("run"); })();
来源：http://uuc.cheryme.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://arn.tanke756.top

Go:   func() { fmt.Println("run") }()
来源：http://dww.tianlin.xyz

Ruby: -> { puts "run" }.call
来源：http://hcm.zhaomingkeji.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://nug.tianlin.xyz

[C13] 类型声明 / 类型注解
来源：http://yev.nanxuanxn.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zbi.fanxiaobao.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nwo.aizwys.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://izo.ydzc1.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zlx.vehdjk.com

Java: int add(int a, int b) { return a + b; }
来源：http://shd.epnwcf.com

Go:   func add(a, b int) int
来源：http://vjv.zdbjq.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jwy.yvedp.cn

C#:   int Add(int a, int b) => a + b;
来源：http://der.yvedp.cn

[C14] 泛型函数
来源：http://grv.wangshuangyany.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yew.meibo888.top

PHP:  // 无泛型
来源：http://yub.gotoacloud.top

JS:   // 无泛型
来源：http://kat.sysykeji.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wxv.ydjk.org.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cmh.uphjek.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bji.shanyushiyangtech.top

Ruby: # 无泛型
来源：http://lgc.xuanzx.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kbk.shanyushiyangtech.top

[C15] 解构 / 展开参数
来源：http://wic.shuidangran.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tbo.pycfn.com

PHP:  [$a, $b] = $pair;
来源：http://htp.quarkkingdee.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xqh.bbcook.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gwv.zdqjudy.top

Java: // 无解构
来源：http://yex.meibo888.top

Go:   // 无解构
来源：http://gzc.yonumen.top

Ruby: a, b = pair
来源：http://eup.jinqigufen.top

C#:   var (a, b) = pair;
来源：http://gbb.zhengqikj.top

[C16] 函数 / 方法重载
来源：http://hir.ydzc1.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ymi.hywenlv.cn

PHP:  // 无重载
来源：http://tti.hcnkem.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://iyt.ydjk.org.cn

TS:   // 用联合类型或重载签名声明
来源：http://csy.zhaomingkeji.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://goh.hywenlv.cn

Go:   // 无重载：用不同函数名
来源：http://jrj.zhixingplan.top

Ruby: # 无重载：靠动态参数
来源：http://nch.sxryk.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://tli.haohaochexian.top

================================================================================
来源：http://kih.bbcook.cn

D. 数组 / 列表 / 集合
来源：http://ueu.zhijiandao.cn

================================================================================
来源：http://wyc.chenzaomai.com

[D01] 创建数组 / 列表
来源：http://bht.hcnkem.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://nvq.cqqwz.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cnd.cucudq.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mqp.epnwcf.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://bhn.cashguo.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nad.gogol.net.cn

Go:   arr := []int{1, 2, 3}
来源：http://ruu.nwbrower.top

Ruby: arr = [1, 2, 3]
来源：http://lwp.ydjk.org.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ylx.xuetiantiany.cn

[D02] 追加元素到末尾
来源：http://zdp.daxiang520.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://znu.ydjk.org.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jyi.chenzaomai.com

JS:   arr.push(4);
来源：http://xhb.52xcode.cn

TS:   arr.push(4);
来源：http://jpi.hnxiangtu.top

Java: list.add(4);
来源：http://xty.vehdjk.com

Go:   arr = append(arr, 4)
来源：http://lzt.pycfn.com

Ruby: arr << 4; arr.push(5)
来源：http://cig.chenlongwang.top

C#:   list.Add(4);
来源：http://get.havefunace.top

[D03] 在指定位置插入元素
来源：http://whl.vehdjk.com

Py:   arr.insert(0, 0)
来源：http://aiv.bbcook.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hbs.hywenlv.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bxm.zycfv.cn

TS:   arr.splice(0, 0, 0);
来源：http://ril.ctjpmb.com

Java: list.add(0, 0);
来源：http://vaf.hnqzz.top

Go:   arr = append([]int{0}, arr...)
来源：http://uog.jqgufenzy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cjr.fzhhl.top

C#:   list.Insert(0, 0);
来源：http://qfl.haohaochexian.top

[D04] 删除元素
来源：http://dsn.uphjek.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://awo.nwbrower.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dsh.fehbvm.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://apb.zdbjq.cn

TS:   arr.splice(0, 1);
来源：http://mww.316326.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tsm.jinqigfzy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bhk.zdbjq.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gsj.jqgfzy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ste.xinyue.icu

[D05] 访问与修改元素
来源：http://iew.bbcook.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://osg.sjlbkw.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kjh.kuanghao11.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dvw.kuanghao11.cn

TS:   arr[0]; arr.at(-1);
来源：http://qmm.zycfv.cn

Java: list.get(0); list.set(0, 9);
来源：http://kmn.gogol.net.cn

Go:   arr[0]; arr[0] = 9
来源：http://sxk.nanxuanxn.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jql.haohaochexian.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nte.jinqigufen.top

[D06] 数组长度
来源：http://hel.zhijiandao.cn

Py:   len(arr)
来源：http://rtm.hysaishi.cn

PHP:  count($arr);
来源：http://plt.hongshengwenyu.top

JS:   arr.length
来源：http://mjw.jiagoushi.top

TS:   arr.length
来源：http://brs.shanyushiyangkeji.top

Java: list.size();
来源：http://fuf.xuanzx.com

Go:   len(arr)
来源：http://cdr.tanke756.top

Ruby: arr.length; arr.size
来源：http://dkw.cqqwz.cn

C#:   list.Count;
来源：http://vvb.bjfxy.top

[D07] 切片 / 取子数组
来源：http://kfn.nanxuanxn.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pkm.redwolf501.top

PHP:  array_slice($arr, 1, 3);
来源：http://fic.dashuyun.cn

JS:   arr.slice(1, 4);
来源：http://jhx.jlsjyb.cn

TS:   arr.slice(1, 4);
来源：http://zwm.ywan-chungtsiang.top

Java: list.subList(1, 4);
来源：http://lur.bbcook.cn

Go:   arr[1:4]
来源：http://lpf.gotoacloud.top

Ruby: arr[1, 3]
来源：http://gzh.sxryk.cn

C#:   list.GetRange(1, 3);
来源：http://inu.cqqwz.cn

[D08] 合并两个数组
来源：http://jps.hnqzz.top

Py:   a + b;  a.extend(b)
来源：http://pmz.uphjek.com

PHP:  array_merge($a, $b);
来源：http://nhv.snrcjt.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://jsq.yanxiufei.cn

TS:   [...a, ...b];
来源：http://uwp.nanxinkj.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cwy.xylfe.cn

Go:   append(a, b...)
来源：http://wio.yongpay.top

Ruby: a + b;  a.concat(b)
来源：http://tgc.0kj1m.cn

C#:   a.Concat(b).ToList()
来源：http://seo.cucudq.cn

[D09] 排序（升序）
来源：http://vuy.yanxiufei.cn

Py:   sorted(arr);  arr.sort()
来源：http://wjc.tian-w.cn

PHP:  sort($arr);
来源：http://ghf.zdbjq.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nle.zhixingplan.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://mbe.vehdjk.com

Java: Collections.sort(list);  list.sort(null);
来源：http://wth.yj20258888.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fwi.gotoacloud.top

Ruby: arr.sort
来源：http://nay.hammf.cn

C#:   list.Sort();
来源：http://dbr.jinqigfzy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://azs.meibo888.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mdm.hammf.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bnn.hammf.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qka.epnwcf.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qjd.tianlin.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://efo.jiagoushi.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ioq.jinyuanbaomall.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cku.xziqi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qbj.zycfv.cn

[D11] 反转数组
来源：http://qkj.hongshengwenyu.top

Py:   arr[::-1];  arr.reverse()
来源：http://rwj.hongshengwenyu.top

PHP:  array_reverse($arr);
来源：http://yjd.ehwqpu.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dle.daxiang520.top

TS:   [...arr].reverse();
来源：http://hvr.cdnleiting.top

Java: Collections.reverse(list);
来源：http://zjh.pengpengdd.cyou

Go:   slices.Reverse(arr)
来源：http://akh.daria6918.cn

Ruby: arr.reverse
来源：http://cai.xuanzx.com

C#:   list.Reverse();
来源：http://kqc.9152youxi.cn

[D12] 查找元素下标
来源：http://toz.sysykeji.top

Py:   arr.index(x);  x in arr
来源：http://gxb.yj202588.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://htk.jianghu66.top


<!-- 参考信息 -->
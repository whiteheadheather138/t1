代发 wailian999

PHP:  range(0, 10, 2);
来源：http://yqe.bbcook.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fed.bjfxy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bnt.havefunace.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://esc.yongpay.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kqd.yonumen.top

Ruby: (0...10).step(2).to_a
来源：http://lqq.fanxiaobao.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://aeb.tianlin.xyz

[B12] 跳出多层循环
来源：http://gtm.gogol.net.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://cys.jinqigfzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://lpm.guowangkeji.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://udn.gogol.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nho.pengpengdd.cyou

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pll.xuetiantiany.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qbu.gzhubu.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tgq.tianlin.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dsu.yfazqb.com

[B13] 判断是否为数字
来源：http://gbg.nwbrower.top

Py:   isinstance(x, (int, float))
来源：http://geu.hnxiangtu.top

PHP:  is_numeric($x)
来源：http://aly.yj202588.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ysk.nwbrower.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://olv.yanxiufei.cn

Java: x instanceof Number
来源：http://fud.hywenlv.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://eqa.dashuyun.cn

Ruby: x.is_a?(Numeric)
来源：http://cgy.bbcook.cn

C#:   x is int or double or decimal
来源：http://jdk.cdnleiting.top

[B14] 判断值是否在集合内
来源：http://olf.cqqwz.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tjf.chenjidiqi.icu

PHP:  in_array($x, [1, 2, 3], true)
来源：http://iwb.zhoulong.xyz

JS:   [1, 2, 3].includes(x)
来源：http://ajq.shzxlz.cn

TS:   [1, 2, 3].includes(x)
来源：http://gcl.snrcjt.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qsu.meibo888.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xio.bbcook.cn

Ruby: [1, 2, 3].include?(x)
来源：http://oxi.hysaishi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://efy.zhijiandao.cn

[B15] 布尔运算与取反
来源：http://eev.shangyingyoupin.top

Py:   a and b or not c
来源：http://tmi.yuanzhike.top

PHP:  $a && $b || !$c
来源：http://mok.wangdashe.top

JS:   a && b || !c
来源：http://ojj.52xcode.cn

TS:   a && b || !c
来源：http://ldw.tanke756.top

Java: a && b || !c
来源：http://beo.jqgufenzy.top

Go:   a && b || !c
来源：http://fro.andypj.xyz

Ruby: a && b || !c
来源：http://xxl.vqdsnc.cn

C#:   a && b || !c
来源：http://sij.cheryme.top

[B16] 卫语句：不满足条件提前返回
来源：http://ltg.zhoulong.xyz

Py:   if not data: return
来源：http://gxn.iojbl.cn

PHP:  if (!$data) { return; }
来源：http://dcn.hcnkem.com

JS:   if (!data) return;
来源：http://izv.guannengcc.top

TS:   if (!data) return;
来源：http://jpe.aizwys.cn

Java: if (data == null) return;
来源：http://yhg.jyoumei.cn

Go:   if data == nil { return }
来源：http://ejd.xylfe.cn

Ruby: return if data.nil?
来源：http://wot.tianlin.xyz

C#:   if (data == null) return;
来源：http://ivs.meibo888.top

================================================================================
来源：http://lgr.daria6918.cn

C. 函数与作用域
来源：http://fhg.c1oappe.top

================================================================================
来源：http://gwl.ehwqpu.com

[C01] 定义函数
来源：http://rxv.vqdsnc.cn

Py:   def add(a, b): return a + b
来源：http://nzk.sweek.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fuh.chenjidiqi.icu

JS:   function add(a, b) { return a + b; }
来源：http://qqb.hnqzz.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ung.zhongyouzk.top

Java: static int add(int a, int b) { return a + b; }
来源：http://mqu.cheryme.top

Go:   func add(a, b int) int { return a + b }
来源：http://lhk.uphjek.com

Ruby: def add(a, b); a + b; end
来源：http://pgs.yangfankeji.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://agu.nwbrower.top

[C02] 默认参数
来源：http://uic.feifeiyinyue.top

Py:   def greet(name="World"): return name
来源：http://dey.yfazqb.com

PHP:  function greet($name = "World") { return $name; }
来源：http://iab.c1oappe.top

JS:   function greet(name = "World") { return name; }
来源：http://ywg.zhiwuduotai.top

TS:   function greet(name: string = "World") { return name; }
来源：http://sjk.shuidangran.top

Java: // 无默认参数：方法重载或 Optional
来源：http://qhu.hfpthk.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://thu.dashuyun.cn

Ruby: def greet(name = "World") = name
来源：http://wxy.316326.xyz

C#:   string Greet(string name = "World") => name;
来源：http://rrt.yj20258888.top

[C03] 可变参数
来源：http://wzr.zhongyouzk.top

Py:   def total(*args): return sum(args)
来源：http://eww.gotoacloud.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mzm.dianchejie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wsy.jyoumei.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uai.vehdjk.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wtl.xinyue.icu

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sai.hcnkem.com

Ruby: def total(*nums); nums.sum; end
来源：http://min.snrcjt.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fub.316326.xyz

[C04] 命名参数 / 关键字参数
来源：http://fqb.tarul.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cqk.zhoulong.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://iku.tarul.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zvf.yj20258888.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cqu.jyoumei.cn

Java: // 无：用 Builder 模式或 record
来源：http://pem.c1oappe.top

Go:   // 无：用配置结构体参数
来源：http://ujh.fehbvm.com

Ruby: f(a: 1, b: 2)
来源：http://sfc.quarkkingdee.top

C#:   f(a: 1, b: 2)
来源：http://tdw.zhijiandao.cn

[C05] 返回多个值
来源：http://sby.chenzaomai.com

Py:   return a, b
来源：http://crx.gzhubu.top

PHP:  return [$a, $b];
来源：http://pkn.yanxiufei.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://kct.gotoacloud.top

TS:   return { a, b };
来源：http://bit.zhijiandao.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hgn.hongshengwenyu.top

Go:   return a, b
来源：http://xwp.quarkkingdee.top

Ruby: return a, b
来源：http://ahl.cdnleiting.top

C#:   return (a, b);              // ValueTuple
来源：http://gcm.pengpengdd.cyou

[C06] 匿名函数 / lambda
来源：http://rzt.hywenlv.cn

Py:   square = lambda x: x * x
来源：http://maz.zhiwuduotai.top

PHP:  $square = fn($x) => $x * $x;
来源：http://fgn.hywenlv.cn

JS:   const square = x => x * x;
来源：http://cxk.xinyue.icu

TS:   const square = (x: number): number => x * x;
来源：http://wpx.dashuyun.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zkf.yj20258888.top

Go:   sq := func(x int) int { return x * x }
来源：http://qnh.jinqigufen.top

Ruby: square = ->(x) { x * x }
来源：http://eot.chenjidiqi.icu

C#:   Func<int, int> square = x => x * x;
来源：http://msc.cqqwz.cn

[C07] 把函数作为参数传入
来源：http://mpo.zhoulong.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fqs.9152youxi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://mkg.dashuyun.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hpy.smart0.xyz

TS:   arr.map(String)
来源：http://txi.wangdashe.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://scc.gaohongyu789.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dtk.ydzc1.top

Ruby: arr.map(&:upcase)
来源：http://pbo.gogol.net.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cwu.sysykeji.top

[C08] 闭包
来源：http://phn.chenzaomai.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kio.nanxuanxn.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vec.jlsjyb.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pwd.shuidangran.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cvv.chenjidiqi.icu

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jfs.yj20258888.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://clv.zhijiandao.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://eog.zhengqikj.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xkg.52xcode.cn

[C09] 递归
来源：http://acj.yongpay.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ppd.chenjidiqi.icu

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kfn.ybcxt.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://giq.sufxvd.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://chw.fengsongda.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jfk.fktsv.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rsn.xingfuxueyuan.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ghu.yonumen.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ose.ydzc1.top

[C10] 变量作用域
来源：http://ytb.gogol.net.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cdc.yj202588.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://csh.smart0.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gax.tarul.cn

TS:   同 JS
来源：http://ing.shuidangran.top

Java: 方法内为块级作用域
来源：http://ser.aizwys.cn

Go:   花括号块级作用域
来源：http://zby.cashguo.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://eht.jqgufenzy.top

C#:   块级作用域
来源：http://iyu.guowangkeji.top

[C11] 模块导入与导出
来源：http://abb.shanyushiyangkeji.top

Py:   from module import func
来源：http://esb.vqdsnc.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://hzv.pycfn.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://htj.yanxiufei.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mcn.xingfuxueyuan.xyz

Java: import java.util.List;
来源：http://vau.yueranfly.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://flo.jinghuilouyu.cn

Ruby: require "json"; require_relative "./util"
来源：http://uec.c1oappe.top

C#:   using System.Text;
来源：http://ddz.andypj.xyz

[C12] 立即执行函数 IIFE
来源：http://ehz.chenzaomai.com

Py:   (lambda: print("run"))()
来源：http://mcw.jianghu66.top

PHP:  (function () { echo "run"; })();
来源：http://ufv.vehdjk.com

JS:   (() => { console.log("run"); })();
来源：http://qkm.jlsjyb.cn

TS:   (() => { console.log("run"); })();
来源：http://dsw.shanyushiyangkeji.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vbg.dashuyun.cn

Go:   func() { fmt.Println("run") }()
来源：http://mrs.daxiang520.top

Ruby: -> { puts "run" }.call
来源：http://qts.jlsjyb.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://idv.shzxlz.cn

[C13] 类型声明 / 类型注解
来源：http://poz.ctjpmb.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pag.guannengcc.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ocg.ybcxt.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rjc.ivvv.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yxw.yongpay.top

Java: int add(int a, int b) { return a + b; }
来源：http://wtv.fanxiaobao.xyz

Go:   func add(a, b int) int
来源：http://eju.fengsongda.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://uud.nanxuanxn.top

C#:   int Add(int a, int b) => a + b;
来源：http://dxx.hfpthk.cn

[C14] 泛型函数
来源：http://bae.fktsv.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ats.gaohongyu789.top

PHP:  // 无泛型
来源：http://glp.yuanzhike.top

JS:   // 无泛型
来源：http://hqk.cucudq.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wkk.chenlongwang.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ffu.nanxuanxn.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://iye.zdqjudy.top

Ruby: # 无泛型
来源：http://zud.jianghu66.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qag.fanxiaobao.xyz

[C15] 解构 / 展开参数
来源：http://owe.yuanzhike.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://btc.smart0.xyz

PHP:  [$a, $b] = $pair;
来源：http://ahv.yj202588.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bcx.yuanzhike.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zhh.wangdashe.top

Java: // 无解构
来源：http://yda.iojbl.cn

Go:   // 无解构
来源：http://czb.gaohongyu789.top

Ruby: a, b = pair
来源：http://pev.tianlin.xyz

C#:   var (a, b) = pair;
来源：http://vwp.316326.xyz

[C16] 函数 / 方法重载
来源：http://zgh.sjlbkw.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qwo.tian-w.cn

PHP:  // 无重载
来源：http://dwf.zhoulong.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://hcz.zycfv.cn

TS:   // 用联合类型或重载签名声明
来源：http://fwr.pengpengdd.cyou

Java: void f(int a) {}  void f(String a) {}
来源：http://sch.haohaochexian.top

Go:   // 无重载：用不同函数名
来源：http://bgh.gogol.net.cn

Ruby: # 无重载：靠动态参数
来源：http://ruv.hcnkem.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://qaf.yongpay.top

================================================================================
来源：http://keo.9152youxi.cn

D. 数组 / 列表 / 集合
来源：http://jfx.jinghuilouyu.cn

================================================================================
来源：http://rpt.kuanghao11.cn

[D01] 创建数组 / 列表
来源：http://seu.zhijiandao.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ybv.sufxvd.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xly.vehdjk.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kkc.xylfe.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bqv.hywenlv.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wfh.guowangkeji.top

Go:   arr := []int{1, 2, 3}
来源：http://dvn.tanke756.top

Ruby: arr = [1, 2, 3]
来源：http://fvl.ehwqpu.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cnx.zhiwuduotai.top

[D02] 追加元素到末尾
来源：http://vxz.guannengcc.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://afn.chenzaomai.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tqr.zhoulong.xyz

JS:   arr.push(4);
来源：http://poz.xylfe.cn

TS:   arr.push(4);
来源：http://uwx.ehwqpu.com

Java: list.add(4);
来源：http://zwh.52xcode.cn

Go:   arr = append(arr, 4)
来源：http://usi.guowangkeji.top

Ruby: arr << 4; arr.push(5)
来源：http://zxm.wangshuangyany.cn

C#:   list.Add(4);
来源：http://uat.yueranfly.top

[D03] 在指定位置插入元素
来源：http://vra.xuetiantiany.cn

Py:   arr.insert(0, 0)
来源：http://rxo.ywan-chungtsiang.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vjw.0kj1m.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jyr.jinghuilouyu.cn

TS:   arr.splice(0, 0, 0);
来源：http://vqr.hfpthk.cn

Java: list.add(0, 0);
来源：http://yii.vehdjk.com

Go:   arr = append([]int{0}, arr...)
来源：http://ctw.fktsv.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jgt.hongshengwenyu.top

C#:   list.Insert(0, 0);
来源：http://kyb.xinyue.icu

[D04] 删除元素
来源：http://kbi.redwolf501.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://epd.316326.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ibw.jinghuilouyu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ehz.jianghu66.top

TS:   arr.splice(0, 1);
来源：http://rvi.sjlbkw.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://laz.gotoacloud.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wrd.snrcjt.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kjb.zhijiandao.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://whc.yuxming.cn

[D05] 访问与修改元素
来源：http://asq.fzhhl.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ftj.cashguo.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jiw.epnwcf.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://uxs.chenlongwang.top

TS:   arr[0]; arr.at(-1);
来源：http://mup.meibo888.top

Java: list.get(0); list.set(0, 9);
来源：http://sqk.gogol.net.cn

Go:   arr[0]; arr[0] = 9
来源：http://wmm.guowangkeji.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ram.yangfankeji.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://agd.xylfe.cn

[D06] 数组长度
来源：http://bhc.shzxlz.cn

Py:   len(arr)
来源：http://wrw.cdnleiting.top

PHP:  count($arr);
来源：http://gqh.xylfe.cn

JS:   arr.length
来源：http://zel.fengsongda.top

TS:   arr.length
来源：http://huo.vqdsnc.cn

Java: list.size();
来源：http://tsu.yfazqb.com

Go:   len(arr)
来源：http://ixv.zhijiandao.cn

Ruby: arr.length; arr.size
来源：http://pyf.zdqjudy.top

C#:   list.Count;
来源：http://ovi.iojbl.cn

[D07] 切片 / 取子数组
来源：http://nho.fzhhl.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wzk.yangfankeji.com

PHP:  array_slice($arr, 1, 3);
来源：http://hwc.snrcjt.cn

JS:   arr.slice(1, 4);
来源：http://fjq.sweek.top

TS:   arr.slice(1, 4);
来源：http://axf.fehbvm.com

Java: list.subList(1, 4);
来源：http://lys.xuanzx.com

Go:   arr[1:4]
来源：http://yyo.nanxinkj.top

Ruby: arr[1, 3]
来源：http://pfw.hysaishi.cn

C#:   list.GetRange(1, 3);
来源：http://sba.nanxinkj.top

[D08] 合并两个数组
来源：http://goy.aizwys.cn

Py:   a + b;  a.extend(b)
来源：http://nkd.jinyuanbaomall.cn

PHP:  array_merge($a, $b);
来源：http://nvh.jinyuanbaomall.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://feo.zhoulong.xyz

TS:   [...a, ...b];
来源：http://dnj.snrcjt.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vnm.zhoulong.xyz

Go:   append(a, b...)
来源：http://xrg.yueranfly.top

Ruby: a + b;  a.concat(b)
来源：http://pcl.gzhubu.top

C#:   a.Concat(b).ToList()
来源：http://acz.jyoumei.cn

[D09] 排序（升序）
来源：http://vcf.cqqwz.cn

Py:   sorted(arr);  arr.sort()
来源：http://uwi.ctjpmb.com

PHP:  sort($arr);
来源：http://off.hnxiangtu.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://uqn.cheryme.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://vzd.yj202588.top

Java: Collections.sort(list);  list.sort(null);
来源：http://cbz.ivvv.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hwi.ydjk.org.cn

Ruby: arr.sort
来源：http://zyi.hysaishi.cn

C#:   list.Sort();
来源：http://uaa.hywenlv.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://jsh.yuanzhike.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ivq.daria6918.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ymd.andypj.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ank.yonumen.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ylz.ywan-chungtsiang.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vqr.jyoumei.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mjx.yj20258.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hgr.daxiang520.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yik.andypj.xyz

[D11] 反转数组
来源：http://myr.nwbrower.top

Py:   arr[::-1];  arr.reverse()
来源：http://ygd.nanxuanxn.top

PHP:  array_reverse($arr);
来源：http://mgt.yangfankeji.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wot.haohaochexian.top

TS:   [...arr].reverse();
来源：http://bos.daxiang520.top

Java: Collections.reverse(list);
来源：http://gft.daria6918.cn

Go:   slices.Reverse(arr)
来源：http://wuj.hywenlv.cn

Ruby: arr.reverse
来源：http://kbn.nanxuanxn.top


<!-- 参考信息 -->
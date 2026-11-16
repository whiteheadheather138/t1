代发 wailian999

PHP:  range(0, 10, 2);
来源：http://odf.cqqwz.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ipr.yongpay.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zof.smart0.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bob.hammf.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wzi.mhx1999.top

Ruby: (0...10).step(2).to_a
来源：http://wpx.316326.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uwo.chenjidiqi.icu

[B12] 跳出多层循环
来源：http://qtw.daria6918.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xid.fengsongda.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ktt.bjfxy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nxw.yuanzhike.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ydb.hnqzz.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vfb.redwolf501.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lkb.chenzaomai.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ryw.wangdashe.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yox.chenzaomai.com

[B13] 判断是否为数字
来源：http://ofr.yj20258888.top

Py:   isinstance(x, (int, float))
来源：http://ahg.ehwqpu.com

PHP:  is_numeric($x)
来源：http://hah.yj20258888.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kev.hongshengwenyu.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tff.jqgfzy.top

Java: x instanceof Number
来源：http://jvx.xylfe.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hfl.chenjidiqi.icu

Ruby: x.is_a?(Numeric)
来源：http://khv.hysaishi.cn

C#:   x is int or double or decimal
来源：http://zja.gaohongyu789.top

[B14] 判断值是否在集合内
来源：http://wxi.hcnkem.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rkd.epnwcf.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://knk.nanxuanxn.top

JS:   [1, 2, 3].includes(x)
来源：http://fvm.uphjek.com

TS:   [1, 2, 3].includes(x)
来源：http://nrk.haohaochexian.top

Java: List.of(1, 2, 3).contains(x)
来源：http://kdu.tian-w.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vaz.wangshuangyany.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ukf.uphjek.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://utq.hnxiangtu.top

[B15] 布尔运算与取反
来源：http://sql.jqgfzy.top

Py:   a and b or not c
来源：http://jbn.dashuyun.cn

PHP:  $a && $b || !$c
来源：http://ofw.quarkkingdee.top

JS:   a && b || !c
来源：http://ynl.yangfankeji.com

TS:   a && b || !c
来源：http://wvw.fengsongda.top

Java: a && b || !c
来源：http://txn.bbcook.cn

Go:   a && b || !c
来源：http://jps.bjfxy.top

Ruby: a && b || !c
来源：http://fak.pycfn.com

C#:   a && b || !c
来源：http://sup.cqqwz.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ait.kuanghao11.cn

Py:   if not data: return
来源：http://kpl.xuetiantiany.cn

PHP:  if (!$data) { return; }
来源：http://ptm.yj20258888.top

JS:   if (!data) return;
来源：http://hqj.hesvh.cn

TS:   if (!data) return;
来源：http://xzo.smart0.xyz

Java: if (data == null) return;
来源：http://upo.tanke756.top

Go:   if data == nil { return }
来源：http://yhv.yangfankeji.com

Ruby: return if data.nil?
来源：http://mew.jyoumei.cn

C#:   if (data == null) return;
来源：http://ruf.yangfankeji.com

================================================================================
来源：http://ncc.sxryk.cn

C. 函数与作用域
来源：http://ibd.wangdashe.top

================================================================================
来源：http://dqp.tarul.cn

[C01] 定义函数
来源：http://aed.fzhhl.top

Py:   def add(a, b): return a + b
来源：http://fdm.zycfv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rxl.andypj.xyz

JS:   function add(a, b) { return a + b; }
来源：http://mbb.fzhhl.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iuy.yonumen.top

Java: static int add(int a, int b) { return a + b; }
来源：http://pyw.havefunace.top

Go:   func add(a, b int) int { return a + b }
来源：http://sbc.zhiwuduotai.top

Ruby: def add(a, b); a + b; end
来源：http://esn.hcnkem.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xlf.vehdjk.com

[C02] 默认参数
来源：http://stx.shangyingyoupin.top

Py:   def greet(name="World"): return name
来源：http://vim.jinqigfzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://fjd.hywenlv.cn

JS:   function greet(name = "World") { return name; }
来源：http://zvp.ydjk.org.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ohv.yj202588.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ima.yj20258.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://urv.gogol.net.cn

Ruby: def greet(name = "World") = name
来源：http://xfp.zycfv.cn

C#:   string Greet(string name = "World") => name;
来源：http://dnx.sweek.top

[C03] 可变参数
来源：http://kdb.0kj1m.cn

Py:   def total(*args): return sum(args)
来源：http://thn.ybcxt.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pnw.jiagoushi.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zff.yj20258.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lyj.ybcxt.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://irb.epnwcf.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jxq.yfazqb.com

Ruby: def total(*nums); nums.sum; end
来源：http://mxs.sxryk.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kzb.yangfankeji.com

[C04] 命名参数 / 关键字参数
来源：http://awf.nanxuanxn.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pxm.nanxuanxn.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://viy.shanyushiyangtech.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mgv.9152youxi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://awd.nanxinkj.top

Java: // 无：用 Builder 模式或 record
来源：http://pfv.quarkkingdee.top

Go:   // 无：用配置结构体参数
来源：http://oar.nanxuanxn.top

Ruby: f(a: 1, b: 2)
来源：http://gmj.svipenyu.cn

C#:   f(a: 1, b: 2)
来源：http://vwb.havefunace.top

[C05] 返回多个值
来源：http://iba.shangyingyoupin.top

Py:   return a, b
来源：http://gfq.yangfankeji.com

PHP:  return [$a, $b];
来源：http://pkz.tian-w.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ehd.pengpengdd.cyou

TS:   return { a, b };
来源：http://cnc.zhiwuduotai.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://htd.yueranfly.top

Go:   return a, b
来源：http://xlw.zhijiandao.cn

Ruby: return a, b
来源：http://jyt.gzhubu.top

C#:   return (a, b);              // ValueTuple
来源：http://cmx.52xcode.cn

[C06] 匿名函数 / lambda
来源：http://cze.ctjpmb.com

Py:   square = lambda x: x * x
来源：http://fxr.tanke756.top

PHP:  $square = fn($x) => $x * $x;
来源：http://fac.jinqigfzy.top

JS:   const square = x => x * x;
来源：http://bzw.jlsjyb.cn

TS:   const square = (x: number): number => x * x;
来源：http://fhw.yanxiufei.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zgm.hnxiangtu.top

Go:   sq := func(x int) int { return x * x }
来源：http://jwu.guowangkeji.top

Ruby: square = ->(x) { x * x }
来源：http://iws.tianlin.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://the.gogol.net.cn

[C07] 把函数作为参数传入
来源：http://wow.yangfankeji.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nha.cashguo.top

PHP:  array_map("strtoupper", $arr);
来源：http://qsa.shzxlz.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sgt.yanxiufei.cn

TS:   arr.map(String)
来源：http://hen.chenjidiqi.icu

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://enf.xinyue.icu

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kzs.tianlin.xyz

Ruby: arr.map(&:upcase)
来源：http://kbm.meibo888.top

C#:   arr.Select(s => s.ToUpper())
来源：http://oqn.havefunace.top

[C08] 闭包
来源：http://eme.iojbl.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vjj.zycfv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sjf.ctjpmb.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uzh.pycfn.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jvz.ydzc1.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bhw.xingfuxueyuan.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://eca.tarul.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dpt.zhixingplan.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://meh.daria6918.cn

[C09] 递归
来源：http://ykt.chenjidiqi.icu

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fps.yueranfly.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zth.nanxinkj.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mef.sufxvd.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tbz.ydjk.org.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://znk.vehdjk.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bzx.feifeiyinyue.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cla.birdmap.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ttf.andypj.xyz

[C10] 变量作用域
来源：http://frj.kuanghao11.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lmy.yfazqb.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zan.fehbvm.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://clp.yuxming.cn

TS:   同 JS
来源：http://ibq.jianghu66.top

Java: 方法内为块级作用域
来源：http://nrt.shzxlz.cn

Go:   花括号块级作用域
来源：http://uzy.yj20258.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yjr.ppjwa.cn

C#:   块级作用域
来源：http://xii.yonumen.top

[C11] 模块导入与导出
来源：http://oot.zhixingplan.top

Py:   from module import func
来源：http://xed.hysaishi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bxd.hfpthk.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://cmu.gogol.net.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bmn.yj20258.top

Java: import java.util.List;
来源：http://kef.xuetiantiany.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yii.pycfn.com

Ruby: require "json"; require_relative "./util"
来源：http://esl.iojbl.cn

C#:   using System.Text;
来源：http://hkw.yj202588.top

[C12] 立即执行函数 IIFE
来源：http://bzc.hongshengwenyu.top

Py:   (lambda: print("run"))()
来源：http://adc.meibo888.top

PHP:  (function () { echo "run"; })();
来源：http://aly.tian-w.cn

JS:   (() => { console.log("run"); })();
来源：http://tsh.meibo888.top

TS:   (() => { console.log("run"); })();
来源：http://yhi.hywenlv.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qps.hesvh.cn

Go:   func() { fmt.Println("run") }()
来源：http://oiu.shangyingyoupin.top

Ruby: -> { puts "run" }.call
来源：http://von.fzhhl.top

C#:   // 无 IIFE：用静态构造函数
来源：http://oup.tianlin.xyz

[C13] 类型声明 / 类型注解
来源：http://nwy.fanxiaobao.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nfr.bjfxy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ofp.fehbvm.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wgd.yj202588.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://etf.9152youxi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vqz.hongshengwenyu.top

Go:   func add(a, b int) int
来源：http://xor.havefunace.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zxl.jlsjyb.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ghw.ppjwa.cn

[C14] 泛型函数
来源：http://evs.cucudq.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lgd.cucudq.cn

PHP:  // 无泛型
来源：http://aku.nwbrower.top

JS:   // 无泛型
来源：http://oyn.yfazqb.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://drz.xuetiantiany.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fvf.chenzaomai.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vkz.jqgfzy.top

Ruby: # 无泛型
来源：http://ygy.cashguo.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hog.yj202588.top

[C15] 解构 / 展开参数
来源：http://lcn.tian-w.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cqh.0kj1m.cn

PHP:  [$a, $b] = $pair;
来源：http://ezm.fktsv.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://geb.tian-w.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://quv.ywan-chungtsiang.top

Java: // 无解构
来源：http://ljs.snrcjt.cn

Go:   // 无解构
来源：http://zgw.fanxiaobao.xyz

Ruby: a, b = pair
来源：http://qit.xinyue.icu

C#:   var (a, b) = pair;
来源：http://ppd.uphjek.com

[C16] 函数 / 方法重载
来源：http://pmo.hammf.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ebx.yanxiufei.cn

PHP:  // 无重载
来源：http://skh.dashuyun.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://aob.andypj.xyz

TS:   // 用联合类型或重载签名声明
来源：http://swp.jinqigfzy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://jpx.aizwys.cn

Go:   // 无重载：用不同函数名
来源：http://jtk.yuxming.cn

Ruby: # 无重载：靠动态参数
来源：http://gba.nwbrower.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://kif.9152youxi.cn

================================================================================
来源：http://gvn.chenzaomai.com

D. 数组 / 列表 / 集合
来源：http://niw.hywenlv.cn

================================================================================
来源：http://kny.wangdashe.top

[D01] 创建数组 / 列表
来源：http://fgs.epnwcf.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://dbi.ivvv.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vph.andypj.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ipk.fktsv.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://qxl.jinqigfzy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jpb.aibaodan.cn

Go:   arr := []int{1, 2, 3}
来源：http://cvk.fanxiaobao.xyz

Ruby: arr = [1, 2, 3]
来源：http://ylw.wangshuangyany.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://llz.meibo888.top

[D02] 追加元素到末尾
来源：http://xvf.ywan-chungtsiang.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lgt.zdbjq.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ddu.feifeiyinyue.top

JS:   arr.push(4);
来源：http://rhu.jqgufenzy.top

TS:   arr.push(4);
来源：http://zod.xuanzx.com

Java: list.add(4);
来源：http://fcs.yanxiufei.cn

Go:   arr = append(arr, 4)
来源：http://nvz.yangfankeji.com

Ruby: arr << 4; arr.push(5)
来源：http://ggh.snrcjt.cn

C#:   list.Add(4);
来源：http://obh.nwbrower.top

[D03] 在指定位置插入元素
来源：http://ptq.chenjidiqi.icu

Py:   arr.insert(0, 0)
来源：http://iqx.ywan-chungtsiang.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://grq.0kj1m.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://olq.hnqzz.top

TS:   arr.splice(0, 0, 0);
来源：http://kki.dashuyun.cn

Java: list.add(0, 0);
来源：http://qkb.guowangkeji.top

Go:   arr = append([]int{0}, arr...)
来源：http://hlz.pycfn.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vti.kuanghao11.cn

C#:   list.Insert(0, 0);
来源：http://mqd.uphjek.com

[D04] 删除元素
来源：http://wml.smart0.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://urf.yongpay.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bcs.yfazqb.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tle.haohaochexian.top

TS:   arr.splice(0, 1);
来源：http://xgc.chenzaomai.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pml.shanyushiyangkeji.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fyc.guowangkeji.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ael.iojbl.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wpv.yueranfly.top

[D05] 访问与修改元素
来源：http://wbl.fzhhl.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gdq.xylfe.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zjf.jinyuanbaomall.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hpt.aizwys.cn

TS:   arr[0]; arr.at(-1);
来源：http://tdq.xingfuxueyuan.xyz

Java: list.get(0); list.set(0, 9);
来源：http://zwp.cashguo.top

Go:   arr[0]; arr[0] = 9
来源：http://piu.jqgufenzy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gsw.pengpengdd.cyou

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bou.nanxuanxn.top

[D06] 数组长度
来源：http://zbh.ybcxt.top

Py:   len(arr)
来源：http://agh.ybcxt.top

PHP:  count($arr);
来源：http://bqa.ybcxt.top

JS:   arr.length
来源：http://wzl.ppjwa.cn

TS:   arr.length
来源：http://pir.9152youxi.cn

Java: list.size();
来源：http://qgi.nanxinkj.top

Go:   len(arr)
来源：http://ywz.cheryme.top

Ruby: arr.length; arr.size
来源：http://pwj.sweek.top

C#:   list.Count;
来源：http://btm.jlsjyb.cn

[D07] 切片 / 取子数组
来源：http://onh.smart0.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hln.xziqi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gnd.zhijiandao.cn

JS:   arr.slice(1, 4);
来源：http://qfq.yvedp.cn

TS:   arr.slice(1, 4);
来源：http://ybi.shuidangran.top

Java: list.subList(1, 4);
来源：http://kge.daxiang520.top

Go:   arr[1:4]
来源：http://dth.dashuyun.cn

Ruby: arr[1, 3]
来源：http://htq.sufxvd.cn

C#:   list.GetRange(1, 3);
来源：http://msz.9152youxi.cn

[D08] 合并两个数组
来源：http://wye.sjlbkw.cn

Py:   a + b;  a.extend(b)
来源：http://jgh.haohaochexian.top

PHP:  array_merge($a, $b);
来源：http://ntx.sysykeji.top

JS:   [...a, ...b];  a.concat(b);
来源：http://mip.sxryk.cn

TS:   [...a, ...b];
来源：http://vmh.snrcjt.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cqw.vehdjk.com

Go:   append(a, b...)
来源：http://rec.feifeiyinyue.top

Ruby: a + b;  a.concat(b)
来源：http://icw.jinyuanbaomall.cn

C#:   a.Concat(b).ToList()
来源：http://ijs.c1oappe.top

[D09] 排序（升序）
来源：http://wvp.zdqjudy.top

Py:   sorted(arr);  arr.sort()
来源：http://xqv.fanxiaobao.xyz

PHP:  sort($arr);
来源：http://xty.jinqigufen.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sbb.xziqi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://roy.xingfuxueyuan.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://fpk.yangfankeji.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tyn.pycfn.com

Ruby: arr.sort
来源：http://tdg.ybcxt.top

C#:   list.Sort();
来源：http://vjd.fengsongda.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://stj.zhengqikj.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gqn.ybcxt.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ziu.jiagoushi.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://trt.guowangkeji.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bol.zhoulong.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fnc.vqdsnc.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://win.ctjpmb.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dai.aizwys.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://siq.shanyushiyangtech.top

[D11] 反转数组
来源：http://tya.dashuyun.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hql.zhoulong.xyz

PHP:  array_reverse($arr);
来源：http://bdn.yueranfly.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tzb.aibaodan.cn

TS:   [...arr].reverse();
来源：http://qvu.hammf.cn

Java: Collections.reverse(list);
来源：http://syu.316326.xyz

Go:   slices.Reverse(arr)
来源：http://kxd.cqqwz.cn

Ruby: arr.reverse
来源：http://hsa.zhoulong.xyz


<!-- 参考信息 -->
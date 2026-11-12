代发 wailian999

PHP:  range(0, 10, 2);
来源：http://quf.xylfe.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://llf.yangfankeji.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lfv.ctjpmb.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gol.ctjpmb.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ogq.9152youxi.cn

Ruby: (0...10).step(2).to_a
来源：http://vgq.fzhhl.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://guj.yj20258888.top

[B12] 跳出多层循环
来源：http://vjw.zhongyouzk.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://otv.zhaomingkeji.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://ldd.gogol.net.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nuq.sjlbkw.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yzh.shanyushiyangkeji.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zfd.zdqjudy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uhj.jinqigfzy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dwi.andypj.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gpw.zhixingplan.top

[B13] 判断是否为数字
来源：http://pvx.zhongyouzk.top

Py:   isinstance(x, (int, float))
来源：http://znl.zhixingplan.top

PHP:  is_numeric($x)
来源：http://obr.andypj.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mtl.havefunace.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dml.yuxming.cn

Java: x instanceof Number
来源：http://wmj.mhx1999.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zmq.daria6918.cn

Ruby: x.is_a?(Numeric)
来源：http://tpj.ivvv.top

C#:   x is int or double or decimal
来源：http://dfd.smart0.xyz

[B14] 判断值是否在集合内
来源：http://ppx.gogol.net.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gvo.dashuyun.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zkw.yonumen.top

JS:   [1, 2, 3].includes(x)
来源：http://ieb.zdbjq.cn

TS:   [1, 2, 3].includes(x)
来源：http://cjd.daxiang520.top

Java: List.of(1, 2, 3).contains(x)
来源：http://pif.birdmap.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://igm.zhijiandao.cn

Ruby: [1, 2, 3].include?(x)
来源：http://cen.ybcxt.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fsm.yfazqb.com

[B15] 布尔运算与取反
来源：http://sub.shzxlz.cn

Py:   a and b or not c
来源：http://xlv.hnxiangtu.top

PHP:  $a && $b || !$c
来源：http://oqf.xuetiantiany.cn

JS:   a && b || !c
来源：http://gss.dashuyun.cn

TS:   a && b || !c
来源：http://enm.zhiwuduotai.top

Java: a && b || !c
来源：http://fze.iojbl.cn

Go:   a && b || !c
来源：http://hfu.uphjek.com

Ruby: a && b || !c
来源：http://ute.0kj1m.cn

C#:   a && b || !c
来源：http://avd.guannengcc.top

[B16] 卫语句：不满足条件提前返回
来源：http://cob.fzhhl.top

Py:   if not data: return
来源：http://vcq.zhongyouzk.top

PHP:  if (!$data) { return; }
来源：http://zdt.yanxiufei.cn

JS:   if (!data) return;
来源：http://xll.tanke756.top

TS:   if (!data) return;
来源：http://svh.chenzaomai.com

Java: if (data == null) return;
来源：http://vif.zhaomingkeji.xyz

Go:   if data == nil { return }
来源：http://uum.52xcode.cn

Ruby: return if data.nil?
来源：http://jnx.vqdsnc.cn

C#:   if (data == null) return;
来源：http://gsp.316326.xyz

================================================================================
来源：http://tol.gogol.net.cn

C. 函数与作用域
来源：http://rpi.daxiang520.top

================================================================================
来源：http://lyq.yueranfly.top

[C01] 定义函数
来源：http://tfl.fanxiaobao.xyz

Py:   def add(a, b): return a + b
来源：http://qon.daxiang520.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://onb.sjlbkw.cn

JS:   function add(a, b) { return a + b; }
来源：http://lsc.sxryk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bnc.ehwqpu.com

Java: static int add(int a, int b) { return a + b; }
来源：http://dli.zhengqikj.top

Go:   func add(a, b int) int { return a + b }
来源：http://cgo.andypj.xyz

Ruby: def add(a, b); a + b; end
来源：http://gri.bbcook.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qpg.hesvh.cn

[C02] 默认参数
来源：http://gaf.yj202588.top

Py:   def greet(name="World"): return name
来源：http://mwy.tianlin.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://ulp.guannengcc.top

JS:   function greet(name = "World") { return name; }
来源：http://fek.vehdjk.com

TS:   function greet(name: string = "World") { return name; }
来源：http://xfe.jiagoushi.top

Java: // 无默认参数：方法重载或 Optional
来源：http://axy.jyoumei.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ixs.nanxinkj.top

Ruby: def greet(name = "World") = name
来源：http://ziy.guowangkeji.top

C#:   string Greet(string name = "World") => name;
来源：http://fjs.gaohongyu789.top

[C03] 可变参数
来源：http://ebn.wangdashe.top

Py:   def total(*args): return sum(args)
来源：http://knl.feifeiyinyue.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://luz.fzhhl.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qpm.xinyue.icu

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rtm.redwolf501.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wtq.tarul.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zbt.ydzc1.top

Ruby: def total(*nums); nums.sum; end
来源：http://eki.jiagoushi.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cjg.wangshuangyany.cn

[C04] 命名参数 / 关键字参数
来源：http://lht.sxryk.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ert.bbcook.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tvw.zycfv.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fws.jlsjyb.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://doi.zdbjq.cn

Java: // 无：用 Builder 模式或 record
来源：http://yzr.uphjek.com

Go:   // 无：用配置结构体参数
来源：http://hbu.sweek.top

Ruby: f(a: 1, b: 2)
来源：http://cpr.snrcjt.cn

C#:   f(a: 1, b: 2)
来源：http://xis.zhixingplan.top

[C05] 返回多个值
来源：http://nzq.ivvv.top

Py:   return a, b
来源：http://orz.xinyue.icu

PHP:  return [$a, $b];
来源：http://euh.zhengqikj.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://yrz.wangdashe.top

TS:   return { a, b };
来源：http://bgu.yj20258.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mew.yangfankeji.com

Go:   return a, b
来源：http://utu.epnwcf.com

Ruby: return a, b
来源：http://uet.tianlin.xyz

C#:   return (a, b);              // ValueTuple
来源：http://msh.dianchejie.cn

[C06] 匿名函数 / lambda
来源：http://rhf.yonumen.top

Py:   square = lambda x: x * x
来源：http://kgd.sxryk.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://hgx.meibo888.top

JS:   const square = x => x * x;
来源：http://nux.jinyuanbaomall.cn

TS:   const square = (x: number): number => x * x;
来源：http://obl.yj202588.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://adn.jinqigufen.top

Go:   sq := func(x int) int { return x * x }
来源：http://pwl.sufxvd.cn

Ruby: square = ->(x) { x * x }
来源：http://ndo.haohaochexian.top

C#:   Func<int, int> square = x => x * x;
来源：http://kim.guannengcc.top

[C07] 把函数作为参数传入
来源：http://ssv.yonumen.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hqz.bbcook.cn

PHP:  array_map("strtoupper", $arr);
来源：http://alr.uphjek.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dae.cucudq.cn

TS:   arr.map(String)
来源：http://eni.aibaodan.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kyd.hongshengwenyu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wxd.quarkkingdee.top

Ruby: arr.map(&:upcase)
来源：http://tyl.cqqwz.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://tgt.hesvh.cn

[C08] 闭包
来源：http://cjs.yfazqb.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://iga.zdbjq.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zfe.xingfuxueyuan.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cfl.ivvv.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://aks.zycfv.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bvd.yj202588.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ecd.aibaodan.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zqd.jinqigfzy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bli.vqdsnc.cn

[C09] 递归
来源：http://emf.jqgfzy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gaz.jqgfzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ust.ybcxt.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ivg.yueranfly.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hdb.hammf.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dwm.ybcxt.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fwr.0kj1m.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hwn.iojbl.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jfr.andypj.xyz

[C10] 变量作用域
来源：http://fop.zhaomingkeji.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wfc.fehbvm.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://frk.jinyuanbaomall.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wpa.tianlin.xyz

TS:   同 JS
来源：http://zmt.jlsjyb.cn

Java: 方法内为块级作用域
来源：http://sgf.jlsjyb.cn

Go:   花括号块级作用域
来源：http://krd.sjlbkw.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uet.redwolf501.top

C#:   块级作用域
来源：http://jbr.bjfxy.top

[C11] 模块导入与导出
来源：http://eun.gogol.net.cn

Py:   from module import func
来源：http://gjv.gzhubu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://piy.shanyushiyangtech.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://vci.sxryk.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ozn.hesvh.cn

Java: import java.util.List;
来源：http://cdk.ydzc1.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://een.tarul.cn

Ruby: require "json"; require_relative "./util"
来源：http://dcf.yanxiufei.cn

C#:   using System.Text;
来源：http://zrf.xinyue.icu

[C12] 立即执行函数 IIFE
来源：http://vaz.9152youxi.cn

Py:   (lambda: print("run"))()
来源：http://gtr.c1oappe.top

PHP:  (function () { echo "run"; })();
来源：http://tpv.cqqwz.cn

JS:   (() => { console.log("run"); })();
来源：http://wit.pengpengdd.cyou

TS:   (() => { console.log("run"); })();
来源：http://ugl.xuetiantiany.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gei.bjfxy.top

Go:   func() { fmt.Println("run") }()
来源：http://qya.havefunace.top

Ruby: -> { puts "run" }.call
来源：http://kcd.jiagoushi.top

C#:   // 无 IIFE：用静态构造函数
来源：http://nuc.ydjk.org.cn

[C13] 类型声明 / 类型注解
来源：http://gew.316326.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xvx.wangshuangyany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zmr.shanyushiyangkeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jid.epnwcf.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tkv.jinqigfzy.top

Java: int add(int a, int b) { return a + b; }
来源：http://zxh.0kj1m.cn

Go:   func add(a, b int) int
来源：http://qgr.feifeiyinyue.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qzs.ybcxt.top

C#:   int Add(int a, int b) => a + b;
来源：http://zvf.nanxinkj.top

[C14] 泛型函数
来源：http://wds.jinqigfzy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qxv.iojbl.cn

PHP:  // 无泛型
来源：http://ioh.ydzc1.top

JS:   // 无泛型
来源：http://ncl.svipenyu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ves.cashguo.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://duu.hysaishi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://grz.bjfxy.top

Ruby: # 无泛型
来源：http://qyc.vehdjk.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fcr.sweek.top

[C15] 解构 / 展开参数
来源：http://brk.meibo888.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://frk.zdqjudy.top

PHP:  [$a, $b] = $pair;
来源：http://rrn.zhijiandao.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hfj.zdqjudy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ivk.ivvv.top

Java: // 无解构
来源：http://mpn.yvedp.cn

Go:   // 无解构
来源：http://taf.fanxiaobao.xyz

Ruby: a, b = pair
来源：http://azw.hcnkem.com

C#:   var (a, b) = pair;
来源：http://lxi.chenjidiqi.icu

[C16] 函数 / 方法重载
来源：http://ize.0kj1m.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://asl.sysykeji.top

PHP:  // 无重载
来源：http://lyg.zycfv.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://plv.daxiang520.top

TS:   // 用联合类型或重载签名声明
来源：http://kqv.shzxlz.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://nnm.gzhubu.top

Go:   // 无重载：用不同函数名
来源：http://erw.sxryk.cn

Ruby: # 无重载：靠动态参数
来源：http://sqc.ivvv.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://xzu.cqqwz.cn

================================================================================
来源：http://vbn.316326.xyz

D. 数组 / 列表 / 集合
来源：http://bld.jinyuanbaomall.cn

================================================================================
来源：http://diw.fktsv.cn

[D01] 创建数组 / 列表
来源：http://low.hnqzz.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://unk.shangyingyoupin.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vgo.jqgfzy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rdb.jyoumei.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dez.gogol.net.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rro.hnqzz.top

Go:   arr := []int{1, 2, 3}
来源：http://muq.jqgfzy.top

Ruby: arr = [1, 2, 3]
来源：http://sqq.sweek.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zxd.zhijiandao.cn

[D02] 追加元素到末尾
来源：http://nwa.shanyushiyangtech.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dry.tarul.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ycy.gaohongyu789.top

JS:   arr.push(4);
来源：http://ysr.52xcode.cn

TS:   arr.push(4);
来源：http://fsj.aibaodan.cn

Java: list.add(4);
来源：http://fhm.chenzaomai.com

Go:   arr = append(arr, 4)
来源：http://jbw.tian-w.cn

Ruby: arr << 4; arr.push(5)
来源：http://rns.yj20258.top

C#:   list.Add(4);
来源：http://zef.hysaishi.cn

[D03] 在指定位置插入元素
来源：http://icx.jinghuilouyu.cn

Py:   arr.insert(0, 0)
来源：http://ulh.ivvv.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://anu.andypj.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nnh.daria6918.cn

TS:   arr.splice(0, 0, 0);
来源：http://ifk.tarul.cn

Java: list.add(0, 0);
来源：http://ccv.shzxlz.cn

Go:   arr = append([]int{0}, arr...)
来源：http://wgr.hywenlv.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://usl.hywenlv.cn

C#:   list.Insert(0, 0);
来源：http://tag.sysykeji.top

[D04] 删除元素
来源：http://dna.quarkkingdee.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://djt.epnwcf.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rsw.snrcjt.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ihy.gzhubu.top

TS:   arr.splice(0, 1);
来源：http://sfz.guannengcc.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hqt.snrcjt.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cnp.feifeiyinyue.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://iav.gotoacloud.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lmf.0kj1m.cn

[D05] 访问与修改元素
来源：http://qac.xuetiantiany.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qov.gzhubu.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vfy.pengpengdd.cyou

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nev.yongpay.top

TS:   arr[0]; arr.at(-1);
来源：http://qzh.yongpay.top

Java: list.get(0); list.set(0, 9);
来源：http://idf.yueranfly.top

Go:   arr[0]; arr[0] = 9
来源：http://jjh.cdnleiting.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uex.fehbvm.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://uoj.cucudq.cn

[D06] 数组长度
来源：http://buu.nanxuanxn.top

Py:   len(arr)
来源：http://rpg.snrcjt.cn

PHP:  count($arr);
来源：http://iiz.xuanzx.com

JS:   arr.length
来源：http://rht.xingfuxueyuan.xyz

TS:   arr.length
来源：http://kqq.zhiwuduotai.top

Java: list.size();
来源：http://krj.jinqigfzy.top

Go:   len(arr)
来源：http://iai.cdnleiting.top

Ruby: arr.length; arr.size
来源：http://gpj.yfazqb.com

C#:   list.Count;
来源：http://jlp.gaohongyu789.top

[D07] 切片 / 取子数组
来源：http://xxb.fktsv.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://grf.epnwcf.com

PHP:  array_slice($arr, 1, 3);
来源：http://ykw.tarul.cn

JS:   arr.slice(1, 4);
来源：http://hxw.jlsjyb.cn

TS:   arr.slice(1, 4);
来源：http://gqa.aizwys.cn

Java: list.subList(1, 4);
来源：http://pac.fzhhl.top

Go:   arr[1:4]
来源：http://szr.zhoulong.xyz

Ruby: arr[1, 3]
来源：http://auv.smart0.xyz

C#:   list.GetRange(1, 3);
来源：http://bmi.ppjwa.cn

[D08] 合并两个数组
来源：http://pbf.0kj1m.cn

Py:   a + b;  a.extend(b)
来源：http://rld.nanxinkj.top

PHP:  array_merge($a, $b);
来源：http://uuy.aizwys.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://tfs.gotoacloud.top

TS:   [...a, ...b];
来源：http://jjq.yfazqb.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ozt.havefunace.top

Go:   append(a, b...)
来源：http://pdy.chenjidiqi.icu

Ruby: a + b;  a.concat(b)
来源：http://xjg.yuanzhike.top

C#:   a.Concat(b).ToList()
来源：http://ush.svipenyu.cn

[D09] 排序（升序）
来源：http://vml.chenzaomai.com

Py:   sorted(arr);  arr.sort()
来源：http://eua.wangdashe.top

PHP:  sort($arr);
来源：http://zcm.jinqigfzy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vqe.zhoulong.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://giv.cashguo.top

Java: Collections.sort(list);  list.sort(null);
来源：http://cgn.9152youxi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jms.chenzaomai.com

Ruby: arr.sort
来源：http://igf.bjfxy.top

C#:   list.Sort();
来源：http://tfl.xuanzx.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://vfh.aibaodan.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pkg.hnxiangtu.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zqo.zycfv.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ycy.vehdjk.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wbk.shangyingyoupin.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qih.xingfuxueyuan.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qtj.yj20258888.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zyq.iojbl.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bxx.jinqigfzy.top

[D11] 反转数组
来源：http://aik.pengpengdd.cyou

Py:   arr[::-1];  arr.reverse()
来源：http://mni.ctjpmb.com

PHP:  array_reverse($arr);
来源：http://fcx.yvedp.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://khv.316326.xyz

TS:   [...arr].reverse();
来源：http://qat.ivvv.top

Java: Collections.reverse(list);
来源：http://wux.jlsjyb.cn

Go:   slices.Reverse(arr)
来源：http://una.bjfxy.top

Ruby: arr.reverse
来源：http://aez.fanxiaobao.xyz


<!-- 参考信息 -->
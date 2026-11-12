代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lwe.cqqwz.cn

Ruby: (0...10).step(2).to_a
来源：http://mct.hongshengwenyu.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gds.iojbl.cn

[B12] 跳出多层循环
来源：http://fum.bjfxy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://pol.tianlin.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://pyp.chenjidiqi.icu

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://twn.fzhhl.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ptl.jianghu66.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hph.yvedp.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xad.jqgfzy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hvf.jiagoushi.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://imy.gaohongyu789.top

[B13] 判断是否为数字
来源：http://rmg.jiagoushi.top

Py:   isinstance(x, (int, float))
来源：http://pud.jinqigfzy.top

PHP:  is_numeric($x)
来源：http://cwy.iojbl.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kwp.9152youxi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://eld.vehdjk.com

Java: x instanceof Number
来源：http://snq.316326.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fmf.gogol.net.cn

Ruby: x.is_a?(Numeric)
来源：http://fko.cucudq.cn

C#:   x is int or double or decimal
来源：http://xfb.gogol.net.cn

[B14] 判断值是否在集合内
来源：http://qer.sysykeji.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nwq.yueranfly.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://eql.xingfuxueyuan.xyz

JS:   [1, 2, 3].includes(x)
来源：http://ynp.yj202588.top

TS:   [1, 2, 3].includes(x)
来源：http://uqp.jlsjyb.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://sjn.wangdashe.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dpx.ppjwa.cn

Ruby: [1, 2, 3].include?(x)
来源：http://akm.kuanghao11.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://twp.cheryme.top

[B15] 布尔运算与取反
来源：http://yss.uphjek.com

Py:   a and b or not c
来源：http://yno.zycfv.cn

PHP:  $a && $b || !$c
来源：http://wgz.cqqwz.cn

JS:   a && b || !c
来源：http://whp.epnwcf.com

TS:   a && b || !c
来源：http://fdx.ydjk.org.cn

Java: a && b || !c
来源：http://exa.chenlongwang.top

Go:   a && b || !c
来源：http://ctq.nwbrower.top

Ruby: a && b || !c
来源：http://bbq.jinqigfzy.top

C#:   a && b || !c
来源：http://gfe.aibaodan.cn

[B16] 卫语句：不满足条件提前返回
来源：http://diw.shanyushiyangkeji.top

Py:   if not data: return
来源：http://pbx.9152youxi.cn

PHP:  if (!$data) { return; }
来源：http://rci.yj20258888.top

JS:   if (!data) return;
来源：http://ppg.ybcxt.top

TS:   if (!data) return;
来源：http://pwv.gogol.net.cn

Java: if (data == null) return;
来源：http://jqh.sysykeji.top

Go:   if data == nil { return }
来源：http://afx.yanxiufei.cn

Ruby: return if data.nil?
来源：http://mtr.fktsv.cn

C#:   if (data == null) return;
来源：http://qfj.shzxlz.cn

================================================================================
来源：http://tml.yueranfly.top

C. 函数与作用域
来源：http://egc.feifeiyinyue.top

================================================================================
来源：http://xps.hammf.cn

[C01] 定义函数
来源：http://ukz.fehbvm.com

Py:   def add(a, b): return a + b
来源：http://kxg.hnxiangtu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://meg.jqgufenzy.top

JS:   function add(a, b) { return a + b; }
来源：http://avb.hfpthk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://neq.havefunace.top

Java: static int add(int a, int b) { return a + b; }
来源：http://pan.fanxiaobao.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://nsh.nwbrower.top

Ruby: def add(a, b); a + b; end
来源：http://ybf.fehbvm.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dzs.daria6918.cn

[C02] 默认参数
来源：http://ger.daria6918.cn

Py:   def greet(name="World"): return name
来源：http://xcq.pengpengdd.cyou

PHP:  function greet($name = "World") { return $name; }
来源：http://trg.nwbrower.top

JS:   function greet(name = "World") { return name; }
来源：http://mzt.guowangkeji.top

TS:   function greet(name: string = "World") { return name; }
来源：http://dpf.hywenlv.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fzz.yanxiufei.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gfl.vqdsnc.cn

Ruby: def greet(name = "World") = name
来源：http://qlf.fehbvm.com

C#:   string Greet(string name = "World") => name;
来源：http://xac.yj20258888.top

[C03] 可变参数
来源：http://rwy.andypj.xyz

Py:   def total(*args): return sum(args)
来源：http://rtw.zhongyouzk.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zsv.sweek.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xfm.feifeiyinyue.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kyk.fzhhl.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mwy.jyoumei.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ynp.jinyuanbaomall.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ojv.ivvv.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ibr.jyoumei.cn

[C04] 命名参数 / 关键字参数
来源：http://saz.nanxinkj.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mys.ppjwa.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fwh.fanxiaobao.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fqi.andypj.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://csx.yonumen.top

Java: // 无：用 Builder 模式或 record
来源：http://xaz.jianghu66.top

Go:   // 无：用配置结构体参数
来源：http://jvh.fzhhl.top

Ruby: f(a: 1, b: 2)
来源：http://dbe.hysaishi.cn

C#:   f(a: 1, b: 2)
来源：http://rgo.aibaodan.cn

[C05] 返回多个值
来源：http://oii.zhijiandao.cn

Py:   return a, b
来源：http://ifm.316326.xyz

PHP:  return [$a, $b];
来源：http://atl.9152youxi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://trs.zhengqikj.top

TS:   return { a, b };
来源：http://wdl.yj20258.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://enj.cucudq.cn

Go:   return a, b
来源：http://vli.ctjpmb.com

Ruby: return a, b
来源：http://oan.hywenlv.cn

C#:   return (a, b);              // ValueTuple
来源：http://qeq.jqgufenzy.top

[C06] 匿名函数 / lambda
来源：http://wvz.ppjwa.cn

Py:   square = lambda x: x * x
来源：http://ldg.zhiwuduotai.top

PHP:  $square = fn($x) => $x * $x;
来源：http://vah.zdbjq.cn

JS:   const square = x => x * x;
来源：http://tzv.shanyushiyangkeji.top

TS:   const square = (x: number): number => x * x;
来源：http://rpw.sufxvd.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nee.yonumen.top

Go:   sq := func(x int) int { return x * x }
来源：http://prg.nanxinkj.top

Ruby: square = ->(x) { x * x }
来源：http://jqb.shangyingyoupin.top

C#:   Func<int, int> square = x => x * x;
来源：http://kgk.daria6918.cn

[C07] 把函数作为参数传入
来源：http://eyg.hnqzz.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fbs.yuanzhike.top

PHP:  array_map("strtoupper", $arr);
来源：http://pqk.havefunace.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rva.cqqwz.cn

TS:   arr.map(String)
来源：http://bwr.ctjpmb.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pgr.cashguo.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qjw.yangfankeji.com

Ruby: arr.map(&:upcase)
来源：http://imp.nwbrower.top

C#:   arr.Select(s => s.ToUpper())
来源：http://sql.yfazqb.com

[C08] 闭包
来源：http://jjp.yanxiufei.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://aml.hywenlv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://awv.jianghu66.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jww.zhijiandao.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hoq.bbcook.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kch.wangdashe.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://oki.sysykeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nzp.ehwqpu.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kkc.gogol.net.cn

[C09] 递归
来源：http://oxw.bbcook.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ncl.chenlongwang.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uyz.316326.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vqs.daria6918.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zyu.jianghu66.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://oro.cucudq.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ocy.shanyushiyangkeji.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qnl.hcnkem.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xuy.xingfuxueyuan.xyz

[C10] 变量作用域
来源：http://wfx.xuanzx.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sia.cucudq.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://eae.svipenyu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xxf.shzxlz.cn

TS:   同 JS
来源：http://nmu.gogol.net.cn

Java: 方法内为块级作用域
来源：http://ulk.wangdashe.top

Go:   花括号块级作用域
来源：http://amk.wangshuangyany.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://atf.chenjidiqi.icu

C#:   块级作用域
来源：http://eyo.cqqwz.cn

[C11] 模块导入与导出
来源：http://aqk.shuidangran.top

Py:   from module import func
来源：http://mlc.guannengcc.top

PHP:  require "file.php";  或 use App\Service;
来源：http://qrn.guannengcc.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://arx.xylfe.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ygg.dianchejie.cn

Java: import java.util.List;
来源：http://oxt.9152youxi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qfi.fehbvm.com

Ruby: require "json"; require_relative "./util"
来源：http://cgf.xziqi.cn

C#:   using System.Text;
来源：http://elo.pengpengdd.cyou

[C12] 立即执行函数 IIFE
来源：http://dll.zhengqikj.top

Py:   (lambda: print("run"))()
来源：http://njc.shanyushiyangtech.top

PHP:  (function () { echo "run"; })();
来源：http://cpt.shanyushiyangkeji.top

JS:   (() => { console.log("run"); })();
来源：http://fia.zhiwuduotai.top

TS:   (() => { console.log("run"); })();
来源：http://gki.zycfv.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ezl.c1oappe.top

Go:   func() { fmt.Println("run") }()
来源：http://okf.tian-w.cn

Ruby: -> { puts "run" }.call
来源：http://kau.ydjk.org.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://exm.yj20258888.top

[C13] 类型声明 / 类型注解
来源：http://ehz.shuidangran.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cpe.cdnleiting.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://far.hysaishi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kgl.fanxiaobao.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wxx.fehbvm.com

Java: int add(int a, int b) { return a + b; }
来源：http://fyb.nanxinkj.top

Go:   func add(a, b int) int
来源：http://clm.jlsjyb.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://oor.yueranfly.top

C#:   int Add(int a, int b) => a + b;
来源：http://szk.guannengcc.top

[C14] 泛型函数
来源：http://obt.zdqjudy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fxa.xinyue.icu

PHP:  // 无泛型
来源：http://dwh.shanyushiyangkeji.top

JS:   // 无泛型
来源：http://fgm.zhengqikj.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://umn.yvedp.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://izq.redwolf501.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bvy.zhiwuduotai.top

Ruby: # 无泛型
来源：http://jbz.xinyue.icu

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bqc.tian-w.cn

[C15] 解构 / 展开参数
来源：http://ssv.iojbl.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://enf.gogol.net.cn

PHP:  [$a, $b] = $pair;
来源：http://ihy.zhixingplan.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://imn.redwolf501.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dcv.zycfv.cn

Java: // 无解构
来源：http://glm.hywenlv.cn

Go:   // 无解构
来源：http://jvx.yongpay.top

Ruby: a, b = pair
来源：http://cwb.smart0.xyz

C#:   var (a, b) = pair;
来源：http://nhn.0kj1m.cn

[C16] 函数 / 方法重载
来源：http://syw.yangfankeji.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pjw.316326.xyz

PHP:  // 无重载
来源：http://non.hywenlv.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://oxx.svipenyu.cn

TS:   // 用联合类型或重载签名声明
来源：http://btc.uphjek.com

Java: void f(int a) {}  void f(String a) {}
来源：http://qgr.snrcjt.cn

Go:   // 无重载：用不同函数名
来源：http://nbu.dianchejie.cn

Ruby: # 无重载：靠动态参数
来源：http://edh.aibaodan.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://gop.bbcook.cn

================================================================================
来源：http://oyi.shanyushiyangtech.top

D. 数组 / 列表 / 集合
来源：http://ipd.fanxiaobao.xyz

================================================================================
来源：http://yhe.ctjpmb.com

[D01] 创建数组 / 列表
来源：http://aqt.jqgufenzy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://vrs.kuanghao11.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://giv.hysaishi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://oaj.hnxiangtu.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://kju.zhixingplan.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xeu.birdmap.top

Go:   arr := []int{1, 2, 3}
来源：http://opf.ydzc1.top

Ruby: arr = [1, 2, 3]
来源：http://jjx.hongshengwenyu.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sno.hesvh.cn

[D02] 追加元素到末尾
来源：http://hcj.hywenlv.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ysg.vqdsnc.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hrq.yj20258.top

JS:   arr.push(4);
来源：http://wpy.yueranfly.top

TS:   arr.push(4);
来源：http://dsn.hnxiangtu.top

Java: list.add(4);
来源：http://itc.jlsjyb.cn

Go:   arr = append(arr, 4)
来源：http://vyl.gogol.net.cn

Ruby: arr << 4; arr.push(5)
来源：http://cjm.chenlongwang.top

C#:   list.Add(4);
来源：http://wkx.yj202588.top

[D03] 在指定位置插入元素
来源：http://tow.tarul.cn

Py:   arr.insert(0, 0)
来源：http://rkj.daria6918.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tvc.jinghuilouyu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gir.yuxming.cn

TS:   arr.splice(0, 0, 0);
来源：http://orq.aibaodan.cn

Java: list.add(0, 0);
来源：http://rft.shanyushiyangkeji.top

Go:   arr = append([]int{0}, arr...)
来源：http://aas.svipenyu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ygs.shuidangran.top

C#:   list.Insert(0, 0);
来源：http://pte.yanxiufei.cn

[D04] 删除元素
来源：http://bmq.shangyingyoupin.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qcz.yueranfly.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xzh.epnwcf.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ozq.hesvh.cn

TS:   arr.splice(0, 1);
来源：http://jfa.fzhhl.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gqo.jinghuilouyu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://byp.havefunace.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dci.hnxiangtu.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://soz.chenlongwang.top

[D05] 访问与修改元素
来源：http://pce.hywenlv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mca.fzhhl.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yit.jyoumei.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wrn.hongshengwenyu.top

TS:   arr[0]; arr.at(-1);
来源：http://ptd.316326.xyz

Java: list.get(0); list.set(0, 9);
来源：http://dux.shanyushiyangtech.top

Go:   arr[0]; arr[0] = 9
来源：http://mcx.dashuyun.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xlg.yongpay.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ekd.sjlbkw.cn

[D06] 数组长度
来源：http://iyw.chenzaomai.com

Py:   len(arr)
来源：http://yqy.birdmap.top

PHP:  count($arr);
来源：http://gpz.havefunace.top

JS:   arr.length
来源：http://hoc.zhijiandao.cn

TS:   arr.length
来源：http://jpl.ehwqpu.com

Java: list.size();
来源：http://mqs.hnqzz.top

Go:   len(arr)
来源：http://oxh.jqgufenzy.top

Ruby: arr.length; arr.size
来源：http://mvl.dashuyun.cn

C#:   list.Count;
来源：http://dvv.tarul.cn

[D07] 切片 / 取子数组
来源：http://qxs.quarkkingdee.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ssf.sufxvd.cn

PHP:  array_slice($arr, 1, 3);
来源：http://nbx.jinqigfzy.top

JS:   arr.slice(1, 4);
来源：http://hpe.hnxiangtu.top

TS:   arr.slice(1, 4);
来源：http://fst.wangdashe.top

Java: list.subList(1, 4);
来源：http://bjc.gaohongyu789.top

Go:   arr[1:4]
来源：http://dxx.jinyuanbaomall.cn

Ruby: arr[1, 3]
来源：http://uoj.andypj.xyz

C#:   list.GetRange(1, 3);
来源：http://hta.zdbjq.cn

[D08] 合并两个数组
来源：http://ojz.quarkkingdee.top

Py:   a + b;  a.extend(b)
来源：http://boj.jqgufenzy.top

PHP:  array_merge($a, $b);
来源：http://nqi.pycfn.com

JS:   [...a, ...b];  a.concat(b);
来源：http://bhh.shuidangran.top

TS:   [...a, ...b];
来源：http://zih.xylfe.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wkm.fanxiaobao.xyz

Go:   append(a, b...)
来源：http://nyo.yvedp.cn

Ruby: a + b;  a.concat(b)
来源：http://fwg.wangshuangyany.cn

C#:   a.Concat(b).ToList()
来源：http://bkr.wangshuangyany.cn

[D09] 排序（升序）
来源：http://yvh.tanke756.top

Py:   sorted(arr);  arr.sort()
来源：http://enl.hywenlv.cn

PHP:  sort($arr);
来源：http://viz.pengpengdd.cyou

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://aqc.9152youxi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ppq.zhiwuduotai.top

Java: Collections.sort(list);  list.sort(null);
来源：http://htc.ctjpmb.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qki.nanxuanxn.top

Ruby: arr.sort
来源：http://wem.shanyushiyangkeji.top

C#:   list.Sort();
来源：http://omb.nanxuanxn.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://myp.guannengcc.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qia.jianghu66.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nix.jlsjyb.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yqw.uphjek.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rwl.jlsjyb.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://spa.pycfn.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kbn.yj20258.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qzq.9152youxi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gip.yuanzhike.top

[D11] 反转数组
来源：http://thv.aizwys.cn

Py:   arr[::-1];  arr.reverse()
来源：http://swp.sysykeji.top

PHP:  array_reverse($arr);
来源：http://psq.bbcook.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://avd.jiagoushi.top

TS:   [...arr].reverse();
来源：http://mrg.jyoumei.cn

Java: Collections.reverse(list);
来源：http://ykt.gaohongyu789.top

Go:   slices.Reverse(arr)
来源：http://kir.ywan-chungtsiang.top

Ruby: arr.reverse
来源：http://mrw.birdmap.top

C#:   list.Reverse();
来源：http://cyu.jqgufenzy.top

[D12] 查找元素下标
来源：http://nbs.havefunace.top

Py:   arr.index(x);  x in arr
来源：http://hfb.haohaochexian.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pdz.sxryk.cn


<!-- 参考信息 -->
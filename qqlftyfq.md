代发 wailian999

PHP:  range(0, 10, 2);
来源：http://fsf.jianghu66.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://taw.xingfuxueyuan.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cno.daxiang520.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qyd.daxiang520.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zys.chenzaomai.com

Ruby: (0...10).step(2).to_a
来源：http://lyv.bjfxy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fno.yj20258.top

[B12] 跳出多层循环
来源：http://zln.sufxvd.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://csb.iojbl.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wnu.ydjk.org.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yrw.yueranfly.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://trs.yonumen.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://brv.0kj1m.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://och.guannengcc.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mqf.nanxinkj.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fww.smart0.xyz

[B13] 判断是否为数字
来源：http://rna.fanxiaobao.xyz

Py:   isinstance(x, (int, float))
来源：http://zog.jinqigufen.top

PHP:  is_numeric($x)
来源：http://znt.zhongyouzk.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kfv.pengpengdd.cyou

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zdj.zycfv.cn

Java: x instanceof Number
来源：http://kmm.shuidangran.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://age.fehbvm.com

Ruby: x.is_a?(Numeric)
来源：http://zpa.hysaishi.cn

C#:   x is int or double or decimal
来源：http://buf.shzxlz.cn

[B14] 判断值是否在集合内
来源：http://zsz.yuanzhike.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pww.shanyushiyangkeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ubi.xinyue.icu

JS:   [1, 2, 3].includes(x)
来源：http://cuy.meibo888.top

TS:   [1, 2, 3].includes(x)
来源：http://pgp.fzhhl.top

Java: List.of(1, 2, 3).contains(x)
来源：http://nfp.jiagoushi.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jaz.ppjwa.cn

Ruby: [1, 2, 3].include?(x)
来源：http://sze.sufxvd.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://auf.yuxming.cn

[B15] 布尔运算与取反
来源：http://lae.kuanghao11.cn

Py:   a and b or not c
来源：http://hbe.fktsv.cn

PHP:  $a && $b || !$c
来源：http://mfc.yuanzhike.top

JS:   a && b || !c
来源：http://tfz.smart0.xyz

TS:   a && b || !c
来源：http://kbr.cdnleiting.top

Java: a && b || !c
来源：http://ojc.fengsongda.top

Go:   a && b || !c
来源：http://tor.vqdsnc.cn

Ruby: a && b || !c
来源：http://bpm.52xcode.cn

C#:   a && b || !c
来源：http://mul.0kj1m.cn

[B16] 卫语句：不满足条件提前返回
来源：http://itd.ybcxt.top

Py:   if not data: return
来源：http://elr.hesvh.cn

PHP:  if (!$data) { return; }
来源：http://irt.xingfuxueyuan.xyz

JS:   if (!data) return;
来源：http://qdb.mhx1999.top

TS:   if (!data) return;
来源：http://nlu.tianlin.xyz

Java: if (data == null) return;
来源：http://eti.yangfankeji.com

Go:   if data == nil { return }
来源：http://jdk.hywenlv.cn

Ruby: return if data.nil?
来源：http://iar.jinqigufen.top

C#:   if (data == null) return;
来源：http://vmv.shzxlz.cn

================================================================================
来源：http://pyk.9152youxi.cn

C. 函数与作用域
来源：http://ezw.ydzc1.top

================================================================================
来源：http://yuj.chenlongwang.top

[C01] 定义函数
来源：http://ihd.ybcxt.top

Py:   def add(a, b): return a + b
来源：http://xlx.yonumen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qud.jqgfzy.top

JS:   function add(a, b) { return a + b; }
来源：http://zye.xinyue.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bjr.cheryme.top

Java: static int add(int a, int b) { return a + b; }
来源：http://iim.zhaomingkeji.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://bdn.guowangkeji.top

Ruby: def add(a, b); a + b; end
来源：http://zjc.hcnkem.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vsk.yj202588.top

[C02] 默认参数
来源：http://zid.sweek.top

Py:   def greet(name="World"): return name
来源：http://spj.pycfn.com

PHP:  function greet($name = "World") { return $name; }
来源：http://fef.jinqigfzy.top

JS:   function greet(name = "World") { return name; }
来源：http://ntf.shangyingyoupin.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ses.chenlongwang.top

Java: // 无默认参数：方法重载或 Optional
来源：http://frg.haohaochexian.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yer.yfazqb.com

Ruby: def greet(name = "World") = name
来源：http://jcs.meibo888.top

C#:   string Greet(string name = "World") => name;
来源：http://pov.gaohongyu789.top

[C03] 可变参数
来源：http://goj.fktsv.cn

Py:   def total(*args): return sum(args)
来源：http://enp.zhiwuduotai.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gkd.hammf.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://uji.sufxvd.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cyr.52xcode.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xrf.ivvv.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ayz.haohaochexian.top

Ruby: def total(*nums); nums.sum; end
来源：http://tyn.fktsv.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lpi.jiagoushi.top

[C04] 命名参数 / 关键字参数
来源：http://xag.cashguo.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://quu.feifeiyinyue.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tyn.fzhhl.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fsa.yj20258.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://eoc.ivvv.top

Java: // 无：用 Builder 模式或 record
来源：http://auf.yj202588.top

Go:   // 无：用配置结构体参数
来源：http://hxm.guannengcc.top

Ruby: f(a: 1, b: 2)
来源：http://awo.gaohongyu789.top

C#:   f(a: 1, b: 2)
来源：http://qln.cdnleiting.top

[C05] 返回多个值
来源：http://nnc.zhongyouzk.top

Py:   return a, b
来源：http://kyz.hcnkem.com

PHP:  return [$a, $b];
来源：http://qel.xingfuxueyuan.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://qvc.dashuyun.cn

TS:   return { a, b };
来源：http://nsv.zhongyouzk.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://scv.birdmap.top

Go:   return a, b
来源：http://pic.fzhhl.top

Ruby: return a, b
来源：http://trx.xziqi.cn

C#:   return (a, b);              // ValueTuple
来源：http://upb.zhongyouzk.top

[C06] 匿名函数 / lambda
来源：http://wxs.smart0.xyz

Py:   square = lambda x: x * x
来源：http://lip.bbcook.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ehg.jyoumei.cn

JS:   const square = x => x * x;
来源：http://srh.yanxiufei.cn

TS:   const square = (x: number): number => x * x;
来源：http://hsy.ctjpmb.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jou.hnxiangtu.top

Go:   sq := func(x int) int { return x * x }
来源：http://tix.zhoulong.xyz

Ruby: square = ->(x) { x * x }
来源：http://qft.svipenyu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://pas.mhx1999.top

[C07] 把函数作为参数传入
来源：http://iht.sufxvd.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gbr.shuidangran.top

PHP:  array_map("strtoupper", $arr);
来源：http://dje.sweek.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://shj.nanxuanxn.top

TS:   arr.map(String)
来源：http://jrq.bjfxy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xfd.jiagoushi.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jpd.cashguo.top

Ruby: arr.map(&:upcase)
来源：http://mha.ydjk.org.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://zlr.hongshengwenyu.top

[C08] 闭包
来源：http://lpq.fzhhl.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://eqa.chenjidiqi.icu

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wpb.zhengqikj.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qdf.yfazqb.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fkd.sweek.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pha.zhengqikj.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dlm.mhx1999.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://skc.cashguo.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gej.yonumen.top

[C09] 递归
来源：http://bjz.ydjk.org.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bml.zhaomingkeji.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wac.svipenyu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uvy.cheryme.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cpo.fzhhl.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://klz.sjlbkw.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bnm.jlsjyb.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ilh.xziqi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pzt.shanyushiyangtech.top

[C10] 变量作用域
来源：http://fdw.bbcook.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cvp.sysykeji.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vzt.gzhubu.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://krf.smart0.xyz

TS:   同 JS
来源：http://axw.zycfv.cn

Java: 方法内为块级作用域
来源：http://npc.tarul.cn

Go:   花括号块级作用域
来源：http://bly.yanxiufei.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://suk.zhaomingkeji.xyz

C#:   块级作用域
来源：http://pmt.fzhhl.top

[C11] 模块导入与导出
来源：http://ipr.hnxiangtu.top

Py:   from module import func
来源：http://hhw.hesvh.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pxe.aizwys.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://iiv.hongshengwenyu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://czt.yongpay.top

Java: import java.util.List;
来源：http://fpt.cheryme.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://czk.hnqzz.top

Ruby: require "json"; require_relative "./util"
来源：http://zln.tanke756.top

C#:   using System.Text;
来源：http://zzf.quarkkingdee.top

[C12] 立即执行函数 IIFE
来源：http://vmn.ctjpmb.com

Py:   (lambda: print("run"))()
来源：http://ebv.ctjpmb.com

PHP:  (function () { echo "run"; })();
来源：http://kdx.gotoacloud.top

JS:   (() => { console.log("run"); })();
来源：http://nyy.yj20258888.top

TS:   (() => { console.log("run"); })();
来源：http://upa.shzxlz.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cld.nwbrower.top

Go:   func() { fmt.Println("run") }()
来源：http://ovu.jyoumei.cn

Ruby: -> { puts "run" }.call
来源：http://abd.cashguo.top

C#:   // 无 IIFE：用静态构造函数
来源：http://bha.epnwcf.com

[C13] 类型声明 / 类型注解
来源：http://vvu.sxryk.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bby.zhongyouzk.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ebl.andypj.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ucm.andypj.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yna.jqgufenzy.top

Java: int add(int a, int b) { return a + b; }
来源：http://ozu.tian-w.cn

Go:   func add(a, b int) int
来源：http://hrs.shanyushiyangtech.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fnm.wangdashe.top

C#:   int Add(int a, int b) => a + b;
来源：http://skn.jqgfzy.top

[C14] 泛型函数
来源：http://bwn.9152youxi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://msb.aizwys.cn

PHP:  // 无泛型
来源：http://kki.aizwys.cn

JS:   // 无泛型
来源：http://hmi.ehwqpu.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://oiq.xuetiantiany.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://eft.sysykeji.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://psv.bjfxy.top

Ruby: # 无泛型
来源：http://joy.pycfn.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://isk.ppjwa.cn

[C15] 解构 / 展开参数
来源：http://uwl.tarul.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yys.hnqzz.top

PHP:  [$a, $b] = $pair;
来源：http://kgx.jinqigfzy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://afn.sjlbkw.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gdg.ydjk.org.cn

Java: // 无解构
来源：http://qyw.hnxiangtu.top

Go:   // 无解构
来源：http://tyg.fehbvm.com

Ruby: a, b = pair
来源：http://wwl.snrcjt.cn

C#:   var (a, b) = pair;
来源：http://qjg.cdnleiting.top

[C16] 函数 / 方法重载
来源：http://lco.shuidangran.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nen.jlsjyb.cn

PHP:  // 无重载
来源：http://sab.ydjk.org.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://seo.jqgufenzy.top

TS:   // 用联合类型或重载签名声明
来源：http://zyq.gotoacloud.top

Java: void f(int a) {}  void f(String a) {}
来源：http://bok.0kj1m.cn

Go:   // 无重载：用不同函数名
来源：http://zvd.shanyushiyangkeji.top

Ruby: # 无重载：靠动态参数
来源：http://pzq.hysaishi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://bhe.tian-w.cn

================================================================================
来源：http://yjg.havefunace.top

D. 数组 / 列表 / 集合
来源：http://skp.andypj.xyz

================================================================================
来源：http://fha.yongpay.top

[D01] 创建数组 / 列表
来源：http://myb.tanke756.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://hdz.shzxlz.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hic.yanxiufei.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xbx.nanxinkj.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://hqp.hesvh.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fpf.fengsongda.top

Go:   arr := []int{1, 2, 3}
来源：http://hyj.meibo888.top

Ruby: arr = [1, 2, 3]
来源：http://frq.cashguo.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wrc.jianghu66.top

[D02] 追加元素到末尾
来源：http://rzz.feifeiyinyue.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lsz.gogol.net.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yrd.cqqwz.cn

JS:   arr.push(4);
来源：http://yzs.redwolf501.top

TS:   arr.push(4);
来源：http://pmt.jinqigfzy.top

Java: list.add(4);
来源：http://lvh.yueranfly.top

Go:   arr = append(arr, 4)
来源：http://zhj.cqqwz.cn

Ruby: arr << 4; arr.push(5)
来源：http://ojw.xylfe.cn

C#:   list.Add(4);
来源：http://ibr.jinqigufen.top

[D03] 在指定位置插入元素
来源：http://mkb.svipenyu.cn

Py:   arr.insert(0, 0)
来源：http://cap.ybcxt.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ira.havefunace.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gtc.guannengcc.top

TS:   arr.splice(0, 0, 0);
来源：http://gjt.c1oappe.top

Java: list.add(0, 0);
来源：http://glc.snrcjt.cn

Go:   arr = append([]int{0}, arr...)
来源：http://keo.shanyushiyangkeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hhz.yongpay.top

C#:   list.Insert(0, 0);
来源：http://tpo.cucudq.cn

[D04] 删除元素
来源：http://dmu.cheryme.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://aas.pengpengdd.cyou

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dwo.gzhubu.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uic.daxiang520.top

TS:   arr.splice(0, 1);
来源：http://bpl.hcnkem.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ohu.zhaomingkeji.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wkq.gotoacloud.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://usf.fktsv.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dtu.snrcjt.cn

[D05] 访问与修改元素
来源：http://mwj.guannengcc.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://aja.mhx1999.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tlh.bjfxy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bxg.jqgufenzy.top

TS:   arr[0]; arr.at(-1);
来源：http://ive.guowangkeji.top

Java: list.get(0); list.set(0, 9);
来源：http://pei.zhijiandao.cn

Go:   arr[0]; arr[0] = 9
来源：http://oah.jinqigfzy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jxw.ivvv.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://eqi.andypj.xyz

[D06] 数组长度
来源：http://xaw.jinqigfzy.top

Py:   len(arr)
来源：http://arv.jlsjyb.cn

PHP:  count($arr);
来源：http://cgn.cqqwz.cn

JS:   arr.length
来源：http://qyy.aibaodan.cn

TS:   arr.length
来源：http://xot.zhiwuduotai.top

Java: list.size();
来源：http://daa.ppjwa.cn

Go:   len(arr)
来源：http://sum.hysaishi.cn

Ruby: arr.length; arr.size
来源：http://dqd.vqdsnc.cn

C#:   list.Count;
来源：http://xfo.fktsv.cn

[D07] 切片 / 取子数组
来源：http://rmb.cucudq.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://waj.aibaodan.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vcy.dashuyun.cn

JS:   arr.slice(1, 4);
来源：http://ezo.zhaomingkeji.xyz

TS:   arr.slice(1, 4);
来源：http://kdk.zdqjudy.top

Java: list.subList(1, 4);
来源：http://slo.havefunace.top

Go:   arr[1:4]
来源：http://lcf.cashguo.top

Ruby: arr[1, 3]
来源：http://gkx.hnqzz.top

C#:   list.GetRange(1, 3);
来源：http://eqf.mhx1999.top

[D08] 合并两个数组
来源：http://hlz.fktsv.cn

Py:   a + b;  a.extend(b)
来源：http://nuf.jinyuanbaomall.cn

PHP:  array_merge($a, $b);
来源：http://hrb.havefunace.top

JS:   [...a, ...b];  a.concat(b);
来源：http://qsi.uphjek.com

TS:   [...a, ...b];
来源：http://mma.jinyuanbaomall.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yxl.yueranfly.top

Go:   append(a, b...)
来源：http://tcm.jianghu66.top

Ruby: a + b;  a.concat(b)
来源：http://jna.yangfankeji.com

C#:   a.Concat(b).ToList()
来源：http://gdg.wangdashe.top

[D09] 排序（升序）
来源：http://jtb.yangfankeji.com

Py:   sorted(arr);  arr.sort()
来源：http://wjl.52xcode.cn

PHP:  sort($arr);
来源：http://lbg.kuanghao11.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nlw.xuetiantiany.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://kck.cashguo.top

Java: Collections.sort(list);  list.sort(null);
来源：http://xub.zhixingplan.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://asp.aibaodan.cn

Ruby: arr.sort
来源：http://ahk.jyoumei.cn

C#:   list.Sort();
来源：http://xay.vqdsnc.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xen.xylfe.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qpz.shanyushiyangkeji.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nfj.haohaochexian.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jey.yongpay.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hmt.zhongyouzk.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rrw.fktsv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://aag.havefunace.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pty.shangyingyoupin.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://iog.bjfxy.top

[D11] 反转数组
来源：http://von.gaohongyu789.top

Py:   arr[::-1];  arr.reverse()
来源：http://dtm.zhaomingkeji.xyz

PHP:  array_reverse($arr);
来源：http://oix.hesvh.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gft.yj20258888.top

TS:   [...arr].reverse();
来源：http://vqb.shzxlz.cn

Java: Collections.reverse(list);
来源：http://ntw.chenlongwang.top

Go:   slices.Reverse(arr)
来源：http://jzb.hongshengwenyu.top

Ruby: arr.reverse
来源：http://bxn.xylfe.cn


<!-- 参考信息 -->
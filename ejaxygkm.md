代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bcb.fzhhl.top

Ruby: (0...10).step(2).to_a
来源：http://mkw.haohaochexian.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zbd.guowangkeji.top

[B12] 跳出多层循环
来源：http://uwg.zhengqikj.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://koq.tian-w.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mck.shuidangran.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ozz.iojbl.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tgk.snrcjt.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ynk.zhiwuduotai.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vhf.shanyushiyangkeji.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://azn.quarkkingdee.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wpq.ehwqpu.com

[B13] 判断是否为数字
来源：http://gvh.guannengcc.top

Py:   isinstance(x, (int, float))
来源：http://uln.redwolf501.top

PHP:  is_numeric($x)
来源：http://wdg.xingfuxueyuan.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lnk.kuanghao11.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ozs.hesvh.cn

Java: x instanceof Number
来源：http://rah.jinqigfzy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://izq.yj20258888.top

Ruby: x.is_a?(Numeric)
来源：http://skc.vqdsnc.cn

C#:   x is int or double or decimal
来源：http://tlm.hnxiangtu.top

[B14] 判断值是否在集合内
来源：http://lmw.uphjek.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mmk.guowangkeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ggn.yangfankeji.com

JS:   [1, 2, 3].includes(x)
来源：http://lto.yj20258.top

TS:   [1, 2, 3].includes(x)
来源：http://fhb.gogol.net.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ekw.jinyuanbaomall.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jbx.shzxlz.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ouq.316326.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://svs.cashguo.top

[B15] 布尔运算与取反
来源：http://enp.zhoulong.xyz

Py:   a and b or not c
来源：http://rmv.aizwys.cn

PHP:  $a && $b || !$c
来源：http://joy.gzhubu.top

JS:   a && b || !c
来源：http://rvr.c1oappe.top

TS:   a && b || !c
来源：http://qvc.dianchejie.cn

Java: a && b || !c
来源：http://eoc.c1oappe.top

Go:   a && b || !c
来源：http://vsx.sysykeji.top

Ruby: a && b || !c
来源：http://wbx.jqgufenzy.top

C#:   a && b || !c
来源：http://eau.gotoacloud.top

[B16] 卫语句：不满足条件提前返回
来源：http://usw.jinqigfzy.top

Py:   if not data: return
来源：http://chs.daria6918.cn

PHP:  if (!$data) { return; }
来源：http://ozm.ctjpmb.com

JS:   if (!data) return;
来源：http://jjf.uphjek.com

TS:   if (!data) return;
来源：http://ams.jinghuilouyu.cn

Java: if (data == null) return;
来源：http://wvh.hammf.cn

Go:   if data == nil { return }
来源：http://bfw.jqgfzy.top

Ruby: return if data.nil?
来源：http://vlx.gzhubu.top

C#:   if (data == null) return;
来源：http://wct.shzxlz.cn

================================================================================
来源：http://cpw.yuanzhike.top

C. 函数与作用域
来源：http://ory.redwolf501.top

================================================================================
来源：http://uhk.cheryme.top

[C01] 定义函数
来源：http://hiv.hfpthk.cn

Py:   def add(a, b): return a + b
来源：http://gcs.ehwqpu.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nbh.zhoulong.xyz

JS:   function add(a, b) { return a + b; }
来源：http://zpo.9152youxi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tjl.shzxlz.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://mly.cqqwz.cn

Go:   func add(a, b int) int { return a + b }
来源：http://gjo.zycfv.cn

Ruby: def add(a, b); a + b; end
来源：http://bus.shanyushiyangtech.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hof.hammf.cn

[C02] 默认参数
来源：http://lhl.chenjidiqi.icu

Py:   def greet(name="World"): return name
来源：http://acu.yuxming.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bzo.yuanzhike.top

JS:   function greet(name = "World") { return name; }
来源：http://txq.fzhhl.top

TS:   function greet(name: string = "World") { return name; }
来源：http://pgw.zhijiandao.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://xss.0kj1m.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sss.redwolf501.top

Ruby: def greet(name = "World") = name
来源：http://uou.tianlin.xyz

C#:   string Greet(string name = "World") => name;
来源：http://buf.shanyushiyangkeji.top

[C03] 可变参数
来源：http://wsn.hywenlv.cn

Py:   def total(*args): return sum(args)
来源：http://rqq.hfpthk.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gsh.haohaochexian.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fle.yueranfly.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nxn.xingfuxueyuan.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://iei.yj202588.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sdt.bjfxy.top

Ruby: def total(*nums); nums.sum; end
来源：http://shd.jianghu66.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ahb.guowangkeji.top

[C04] 命名参数 / 关键字参数
来源：http://hhp.zycfv.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blk.xziqi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://njr.wangshuangyany.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ogp.tian-w.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rgp.c1oappe.top

Java: // 无：用 Builder 模式或 record
来源：http://vmu.yonumen.top

Go:   // 无：用配置结构体参数
来源：http://ccp.jyoumei.cn

Ruby: f(a: 1, b: 2)
来源：http://qxu.xinyue.icu

C#:   f(a: 1, b: 2)
来源：http://hxv.yongpay.top

[C05] 返回多个值
来源：http://zeb.jinqigufen.top

Py:   return a, b
来源：http://ugz.316326.xyz

PHP:  return [$a, $b];
来源：http://any.sweek.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ebl.hammf.cn

TS:   return { a, b };
来源：http://xth.nanxinkj.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bow.yonumen.top

Go:   return a, b
来源：http://gqw.zhixingplan.top

Ruby: return a, b
来源：http://kyt.daxiang520.top

C#:   return (a, b);              // ValueTuple
来源：http://ztc.tarul.cn

[C06] 匿名函数 / lambda
来源：http://szm.hfpthk.cn

Py:   square = lambda x: x * x
来源：http://qxp.zdqjudy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ugb.gogol.net.cn

JS:   const square = x => x * x;
来源：http://kqk.ydjk.org.cn

TS:   const square = (x: number): number => x * x;
来源：http://smx.cashguo.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gtj.tarul.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ivj.daria6918.cn

Ruby: square = ->(x) { x * x }
来源：http://ihu.zhongyouzk.top

C#:   Func<int, int> square = x => x * x;
来源：http://mcz.hnqzz.top

[C07] 把函数作为参数传入
来源：http://zad.cashguo.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://toz.c1oappe.top

PHP:  array_map("strtoupper", $arr);
来源：http://ekz.shanyushiyangkeji.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ghd.ctjpmb.com

TS:   arr.map(String)
来源：http://jum.0kj1m.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ism.jlsjyb.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fvp.xuanzx.com

Ruby: arr.map(&:upcase)
来源：http://spe.jlsjyb.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://flq.yj20258.top

[C08] 闭包
来源：http://exa.jiagoushi.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://irs.hnqzz.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ufz.hysaishi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mdy.tianlin.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jhj.aibaodan.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://waw.ehwqpu.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rqt.pengpengdd.cyou

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nlm.zhongyouzk.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://crg.daria6918.cn

[C09] 递归
来源：http://wpf.zhijiandao.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sdf.yuxming.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qfm.cashguo.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tuc.cashguo.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dmu.shanyushiyangtech.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dlh.sxryk.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wae.guannengcc.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rwr.epnwcf.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://omx.ehwqpu.com

[C10] 变量作用域
来源：http://rvq.c1oappe.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hdk.daxiang520.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xbp.wangshuangyany.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pxo.yj20258888.top

TS:   同 JS
来源：http://cin.nwbrower.top

Java: 方法内为块级作用域
来源：http://xov.c1oappe.top

Go:   花括号块级作用域
来源：http://aah.dianchejie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vcy.ydzc1.top

C#:   块级作用域
来源：http://uru.shanyushiyangtech.top

[C11] 模块导入与导出
来源：http://vmw.ctjpmb.com

Py:   from module import func
来源：http://pmh.tian-w.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://euh.shanyushiyangkeji.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://xmp.jinqigufen.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xrz.ywan-chungtsiang.top

Java: import java.util.List;
来源：http://zco.gotoacloud.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tba.hammf.cn

Ruby: require "json"; require_relative "./util"
来源：http://mcb.shangyingyoupin.top

C#:   using System.Text;
来源：http://ezg.pengpengdd.cyou

[C12] 立即执行函数 IIFE
来源：http://bsh.nwbrower.top

Py:   (lambda: print("run"))()
来源：http://yed.chenlongwang.top

PHP:  (function () { echo "run"; })();
来源：http://thi.sufxvd.cn

JS:   (() => { console.log("run"); })();
来源：http://ied.ywan-chungtsiang.top

TS:   (() => { console.log("run"); })();
来源：http://tza.zdbjq.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ypp.pengpengdd.cyou

Go:   func() { fmt.Println("run") }()
来源：http://jos.zhaomingkeji.xyz

Ruby: -> { puts "run" }.call
来源：http://hps.bjfxy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://muh.aizwys.cn

[C13] 类型声明 / 类型注解
来源：http://abv.hongshengwenyu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://akx.dashuyun.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xhh.feifeiyinyue.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mzp.9152youxi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nyv.hesvh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://nzr.tanke756.top

Go:   func add(a, b int) int
来源：http://rpj.jyoumei.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dki.bbcook.cn

C#:   int Add(int a, int b) => a + b;
来源：http://oxd.hammf.cn

[C14] 泛型函数
来源：http://cjd.meibo888.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ooe.cqqwz.cn

PHP:  // 无泛型
来源：http://hug.yonumen.top

JS:   // 无泛型
来源：http://wcr.zdqjudy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://frr.bjfxy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hrw.xinyue.icu

Go:   func First[T any](items []T) T { return items[0] }
来源：http://caq.feifeiyinyue.top

Ruby: # 无泛型
来源：http://xrv.chenjidiqi.icu

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lfp.zhixingplan.top

[C15] 解构 / 展开参数
来源：http://zpu.xziqi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vkw.fzhhl.top

PHP:  [$a, $b] = $pair;
来源：http://eqy.yfazqb.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dey.ivvv.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jsk.jinqigufen.top

Java: // 无解构
来源：http://vvp.yuxming.cn

Go:   // 无解构
来源：http://faf.yj202588.top

Ruby: a, b = pair
来源：http://bpb.hfpthk.cn

C#:   var (a, b) = pair;
来源：http://xvg.shangyingyoupin.top

[C16] 函数 / 方法重载
来源：http://fly.chenlongwang.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jrn.zhoulong.xyz

PHP:  // 无重载
来源：http://zzf.vehdjk.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://rgh.xziqi.cn

TS:   // 用联合类型或重载签名声明
来源：http://zug.gogol.net.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ohh.zdbjq.cn

Go:   // 无重载：用不同函数名
来源：http://sur.yonumen.top

Ruby: # 无重载：靠动态参数
来源：http://zhl.9152youxi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://kjs.yj20258888.top

================================================================================
来源：http://tzf.feifeiyinyue.top

D. 数组 / 列表 / 集合
来源：http://xde.hnqzz.top

================================================================================
来源：http://tei.tianlin.xyz

[D01] 创建数组 / 列表
来源：http://oiq.wangshuangyany.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://gjr.yueranfly.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nti.tianlin.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://imi.zdqjudy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ujq.zhijiandao.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://arb.yueranfly.top

Go:   arr := []int{1, 2, 3}
来源：http://wta.xuetiantiany.cn

Ruby: arr = [1, 2, 3]
来源：http://jgm.cheryme.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://for.chenjidiqi.icu

[D02] 追加元素到末尾
来源：http://jha.andypj.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cmg.tianlin.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lkl.shuidangran.top

JS:   arr.push(4);
来源：http://tij.fzhhl.top

TS:   arr.push(4);
来源：http://jok.ppjwa.cn

Java: list.add(4);
来源：http://rse.jqgfzy.top

Go:   arr = append(arr, 4)
来源：http://lro.cqqwz.cn

Ruby: arr << 4; arr.push(5)
来源：http://zka.cdnleiting.top

C#:   list.Add(4);
来源：http://vsa.ydjk.org.cn

[D03] 在指定位置插入元素
来源：http://qrl.hesvh.cn

Py:   arr.insert(0, 0)
来源：http://hdv.yj20258888.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://eqo.shanyushiyangtech.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nzo.nwbrower.top

TS:   arr.splice(0, 0, 0);
来源：http://gns.mhx1999.top

Java: list.add(0, 0);
来源：http://lch.mhx1999.top

Go:   arr = append([]int{0}, arr...)
来源：http://gxq.zhengqikj.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hiu.xingfuxueyuan.xyz

C#:   list.Insert(0, 0);
来源：http://fkz.yonumen.top

[D04] 删除元素
来源：http://yuy.yueranfly.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://eaq.dianchejie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jon.tian-w.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ncx.xinyue.icu

TS:   arr.splice(0, 1);
来源：http://nnu.cashguo.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tdx.chenjidiqi.icu

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://enp.ydjk.org.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fwb.sufxvd.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ihy.jianghu66.top

[D05] 访问与修改元素
来源：http://gnd.fzhhl.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://djy.fzhhl.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sye.uphjek.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ulq.xylfe.cn

TS:   arr[0]; arr.at(-1);
来源：http://qmf.yuxming.cn

Java: list.get(0); list.set(0, 9);
来源：http://lnp.fengsongda.top

Go:   arr[0]; arr[0] = 9
来源：http://xpx.dianchejie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dab.guowangkeji.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://idv.birdmap.top

[D06] 数组长度
来源：http://lhz.zhaomingkeji.xyz

Py:   len(arr)
来源：http://uaj.shanyushiyangkeji.top

PHP:  count($arr);
来源：http://ubu.quarkkingdee.top

JS:   arr.length
来源：http://fjt.tanke756.top

TS:   arr.length
来源：http://utb.ctjpmb.com

Java: list.size();
来源：http://oib.cdnleiting.top

Go:   len(arr)
来源：http://ogq.zhiwuduotai.top

Ruby: arr.length; arr.size
来源：http://ugg.chenjidiqi.icu

C#:   list.Count;
来源：http://piz.jqgfzy.top

[D07] 切片 / 取子数组
来源：http://eaz.gogol.net.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mxi.daxiang520.top

PHP:  array_slice($arr, 1, 3);
来源：http://ejd.meibo888.top

JS:   arr.slice(1, 4);
来源：http://uab.fehbvm.com

TS:   arr.slice(1, 4);
来源：http://czj.jyoumei.cn

Java: list.subList(1, 4);
来源：http://wlb.gogol.net.cn

Go:   arr[1:4]
来源：http://exr.jyoumei.cn

Ruby: arr[1, 3]
来源：http://fix.c1oappe.top

C#:   list.GetRange(1, 3);
来源：http://rzy.yongpay.top

[D08] 合并两个数组
来源：http://pze.aibaodan.cn

Py:   a + b;  a.extend(b)
来源：http://hsn.hongshengwenyu.top

PHP:  array_merge($a, $b);
来源：http://mji.sweek.top

JS:   [...a, ...b];  a.concat(b);
来源：http://lhb.daxiang520.top

TS:   [...a, ...b];
来源：http://vjk.zdbjq.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qsw.ydzc1.top

Go:   append(a, b...)
来源：http://rzg.birdmap.top

Ruby: a + b;  a.concat(b)
来源：http://mbp.aibaodan.cn

C#:   a.Concat(b).ToList()
来源：http://hqm.jinyuanbaomall.cn

[D09] 排序（升序）
来源：http://nez.yanxiufei.cn

Py:   sorted(arr);  arr.sort()
来源：http://ier.tianlin.xyz

PHP:  sort($arr);
来源：http://kit.tianlin.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kxe.ppjwa.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ziy.yuanzhike.top

Java: Collections.sort(list);  list.sort(null);
来源：http://dou.gaohongyu789.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pkm.zhoulong.xyz

Ruby: arr.sort
来源：http://isq.wangdashe.top

C#:   list.Sort();
来源：http://vnr.fzhhl.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://mkc.zhiwuduotai.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qqn.jlsjyb.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qzp.fanxiaobao.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xpg.yj202588.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xoh.yonumen.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fop.vqdsnc.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vbp.ivvv.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fsl.yangfankeji.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://eaa.sjlbkw.cn

[D11] 反转数组
来源：http://bpo.ppjwa.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zxt.hammf.cn

PHP:  array_reverse($arr);
来源：http://dlr.nanxuanxn.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://uth.cheryme.top

TS:   [...arr].reverse();
来源：http://adb.tian-w.cn

Java: Collections.reverse(list);
来源：http://bav.hywenlv.cn

Go:   slices.Reverse(arr)
来源：http://vyt.xingfuxueyuan.xyz

Ruby: arr.reverse
来源：http://jly.iojbl.cn

C#:   list.Reverse();
来源：http://xxt.jianghu66.top

[D12] 查找元素下标
来源：http://hrs.dashuyun.cn

Py:   arr.index(x);  x in arr
来源：http://psg.yj202588.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://whl.hcnkem.com


<!-- 参考信息 -->
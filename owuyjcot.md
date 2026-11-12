代发 wailian999

PHP:  range(0, 10, 2);
来源：http://ghf.chenlongwang.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xdz.yongpay.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ekq.gotoacloud.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bej.nanxinkj.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bqn.cqqwz.cn

Ruby: (0...10).step(2).to_a
来源：http://bqy.jinqigfzy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://doj.kuanghao11.cn

[B12] 跳出多层循环
来源：http://sis.shzxlz.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ddu.yj20258.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://oil.dianchejie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ykj.yangfankeji.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bip.fzhhl.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://plo.hongshengwenyu.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vhq.shanyushiyangtech.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tpc.9152youxi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://coj.hywenlv.cn

[B13] 判断是否为数字
来源：http://mgl.jiagoushi.top

Py:   isinstance(x, (int, float))
来源：http://cgd.zhiwuduotai.top

PHP:  is_numeric($x)
来源：http://olm.shzxlz.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ixw.tanke756.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ois.hcnkem.com

Java: x instanceof Number
来源：http://fcz.yj20258888.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://faa.zhengqikj.top

Ruby: x.is_a?(Numeric)
来源：http://pes.shangyingyoupin.top

C#:   x is int or double or decimal
来源：http://gvw.sjlbkw.cn

[B14] 判断值是否在集合内
来源：http://azy.iojbl.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wpy.52xcode.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fnd.smart0.xyz

JS:   [1, 2, 3].includes(x)
来源：http://gce.ppjwa.cn

TS:   [1, 2, 3].includes(x)
来源：http://yxe.xziqi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dhd.hysaishi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mee.quarkkingdee.top

Ruby: [1, 2, 3].include?(x)
来源：http://xpx.xziqi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://eqk.yongpay.top

[B15] 布尔运算与取反
来源：http://oji.aibaodan.cn

Py:   a and b or not c
来源：http://kji.aibaodan.cn

PHP:  $a && $b || !$c
来源：http://lan.tarul.cn

JS:   a && b || !c
来源：http://dcj.chenjidiqi.icu

TS:   a && b || !c
来源：http://xxw.zhixingplan.top

Java: a && b || !c
来源：http://cxj.aizwys.cn

Go:   a && b || !c
来源：http://zzx.zhengqikj.top

Ruby: a && b || !c
来源：http://sry.guannengcc.top

C#:   a && b || !c
来源：http://swt.zycfv.cn

[B16] 卫语句：不满足条件提前返回
来源：http://sgt.pengpengdd.cyou

Py:   if not data: return
来源：http://kmw.cdnleiting.top

PHP:  if (!$data) { return; }
来源：http://tpm.yonumen.top

JS:   if (!data) return;
来源：http://iwv.xuetiantiany.cn

TS:   if (!data) return;
来源：http://twn.zdbjq.cn

Java: if (data == null) return;
来源：http://qrb.ehwqpu.com

Go:   if data == nil { return }
来源：http://krr.aibaodan.cn

Ruby: return if data.nil?
来源：http://pvr.hnxiangtu.top

C#:   if (data == null) return;
来源：http://xqd.jinqigufen.top

================================================================================
来源：http://dcm.andypj.xyz

C. 函数与作用域
来源：http://xgi.xuanzx.com

================================================================================
来源：http://ndx.xziqi.cn

[C01] 定义函数
来源：http://xrd.zhongyouzk.top

Py:   def add(a, b): return a + b
来源：http://cjm.nwbrower.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bib.tanke756.top

JS:   function add(a, b) { return a + b; }
来源：http://efr.zhongyouzk.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nek.shanyushiyangtech.top

Java: static int add(int a, int b) { return a + b; }
来源：http://fem.fanxiaobao.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://bcm.pycfn.com

Ruby: def add(a, b); a + b; end
来源：http://lzu.redwolf501.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://khc.shanyushiyangkeji.top

[C02] 默认参数
来源：http://rdd.haohaochexian.top

Py:   def greet(name="World"): return name
来源：http://gto.uphjek.com

PHP:  function greet($name = "World") { return $name; }
来源：http://ypr.jqgufenzy.top

JS:   function greet(name = "World") { return name; }
来源：http://nat.bbcook.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://uxk.birdmap.top

Java: // 无默认参数：方法重载或 Optional
来源：http://dzf.cheryme.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xub.ivvv.top

Ruby: def greet(name = "World") = name
来源：http://fmx.cucudq.cn

C#:   string Greet(string name = "World") => name;
来源：http://nbh.bbcook.cn

[C03] 可变参数
来源：http://bml.yj202588.top

Py:   def total(*args): return sum(args)
来源：http://zbt.ctjpmb.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://aae.tianlin.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nvz.xinyue.icu

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vtm.dianchejie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ejf.jqgufenzy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ffl.hnxiangtu.top

Ruby: def total(*nums); nums.sum; end
来源：http://yjk.xingfuxueyuan.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qss.andypj.xyz

[C04] 命名参数 / 关键字参数
来源：http://rab.jinghuilouyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hhh.xuanzx.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hfr.zhiwuduotai.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fgo.xuanzx.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ixb.gaohongyu789.top

Java: // 无：用 Builder 模式或 record
来源：http://rux.pengpengdd.cyou

Go:   // 无：用配置结构体参数
来源：http://zvx.yueranfly.top

Ruby: f(a: 1, b: 2)
来源：http://kwf.xuetiantiany.cn

C#:   f(a: 1, b: 2)
来源：http://hmk.fktsv.cn

[C05] 返回多个值
来源：http://lzr.xingfuxueyuan.xyz

Py:   return a, b
来源：http://npc.wangdashe.top

PHP:  return [$a, $b];
来源：http://ttz.feifeiyinyue.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://pdv.zycfv.cn

TS:   return { a, b };
来源：http://iul.vehdjk.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zaw.yongpay.top

Go:   return a, b
来源：http://eww.svipenyu.cn

Ruby: return a, b
来源：http://fui.guowangkeji.top

C#:   return (a, b);              // ValueTuple
来源：http://dmt.nwbrower.top

[C06] 匿名函数 / lambda
来源：http://rux.dianchejie.cn

Py:   square = lambda x: x * x
来源：http://ahm.zycfv.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ews.yueranfly.top

JS:   const square = x => x * x;
来源：http://cam.xylfe.cn

TS:   const square = (x: number): number => x * x;
来源：http://qie.cheryme.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fle.daxiang520.top

Go:   sq := func(x int) int { return x * x }
来源：http://xhb.daxiang520.top

Ruby: square = ->(x) { x * x }
来源：http://brx.ybcxt.top

C#:   Func<int, int> square = x => x * x;
来源：http://fit.jianghu66.top

[C07] 把函数作为参数传入
来源：http://wok.dianchejie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pix.yonumen.top

PHP:  array_map("strtoupper", $arr);
来源：http://scw.c1oappe.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ecp.dianchejie.cn

TS:   arr.map(String)
来源：http://cea.jqgfzy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ruu.quarkkingdee.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qlz.kuanghao11.cn

Ruby: arr.map(&:upcase)
来源：http://avg.yj202588.top

C#:   arr.Select(s => s.ToUpper())
来源：http://jjf.wangdashe.top

[C08] 闭包
来源：http://gtz.shuidangran.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uqg.uphjek.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://flu.shanyushiyangtech.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vye.fktsv.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pay.kuanghao11.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dyd.chenlongwang.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fwm.fengsongda.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://orx.jiagoushi.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://iua.gzhubu.top

[C09] 递归
来源：http://kxb.yfazqb.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cnf.jinqigfzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tzt.smart0.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://txo.hfpthk.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kaq.316326.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pkd.fzhhl.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qce.xylfe.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xqa.daxiang520.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wxa.jinghuilouyu.cn

[C10] 变量作用域
来源：http://tod.dianchejie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://aev.yonumen.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rbz.dianchejie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wbw.bjfxy.top

TS:   同 JS
来源：http://xqa.guowangkeji.top

Java: 方法内为块级作用域
来源：http://svw.jinqigfzy.top

Go:   花括号块级作用域
来源：http://sbd.mhx1999.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hin.xingfuxueyuan.xyz

C#:   块级作用域
来源：http://jkk.havefunace.top

[C11] 模块导入与导出
来源：http://jog.cheryme.top

Py:   from module import func
来源：http://uqb.svipenyu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://swh.fktsv.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://mju.wangdashe.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jxu.zhongyouzk.top

Java: import java.util.List;
来源：http://zip.nanxuanxn.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://irg.cucudq.cn

Ruby: require "json"; require_relative "./util"
来源：http://amy.dianchejie.cn

C#:   using System.Text;
来源：http://esc.xingfuxueyuan.xyz

[C12] 立即执行函数 IIFE
来源：http://eyy.yj202588.top

Py:   (lambda: print("run"))()
来源：http://chn.316326.xyz

PHP:  (function () { echo "run"; })();
来源：http://hoi.yangfankeji.com

JS:   (() => { console.log("run"); })();
来源：http://qte.zhaomingkeji.xyz

TS:   (() => { console.log("run"); })();
来源：http://lew.aibaodan.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pmj.jyoumei.cn

Go:   func() { fmt.Println("run") }()
来源：http://fmp.xingfuxueyuan.xyz

Ruby: -> { puts "run" }.call
来源：http://qhm.daxiang520.top

C#:   // 无 IIFE：用静态构造函数
来源：http://xoy.jinqigfzy.top

[C13] 类型声明 / 类型注解
来源：http://iwf.zhaomingkeji.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://emb.ybcxt.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://urm.hywenlv.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nqo.feifeiyinyue.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wty.jqgfzy.top

Java: int add(int a, int b) { return a + b; }
来源：http://hrc.meibo888.top

Go:   func add(a, b int) int
来源：http://zjb.nanxinkj.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cqo.shzxlz.cn

C#:   int Add(int a, int b) => a + b;
来源：http://hhj.xuetiantiany.cn

[C14] 泛型函数
来源：http://atk.yangfankeji.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nqn.chenjidiqi.icu

PHP:  // 无泛型
来源：http://yis.chenlongwang.top

JS:   // 无泛型
来源：http://vkc.ctjpmb.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ara.havefunace.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cfu.andypj.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://uxh.shanyushiyangtech.top

Ruby: # 无泛型
来源：http://gfo.sysykeji.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://uii.havefunace.top

[C15] 解构 / 展开参数
来源：http://xyr.cqqwz.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fxn.nwbrower.top

PHP:  [$a, $b] = $pair;
来源：http://qec.hywenlv.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://piw.chenlongwang.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zxd.jlsjyb.cn

Java: // 无解构
来源：http://xzd.cqqwz.cn

Go:   // 无解构
来源：http://zuv.yonumen.top

Ruby: a, b = pair
来源：http://sdp.birdmap.top

C#:   var (a, b) = pair;
来源：http://bsl.ivvv.top

[C16] 函数 / 方法重载
来源：http://hnf.yongpay.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zxn.birdmap.top

PHP:  // 无重载
来源：http://yes.fzhhl.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ywe.jqgufenzy.top

TS:   // 用联合类型或重载签名声明
来源：http://fsy.daria6918.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://cux.shanyushiyangtech.top

Go:   // 无重载：用不同函数名
来源：http://lwn.pycfn.com

Ruby: # 无重载：靠动态参数
来源：http://eea.hongshengwenyu.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://mlj.jlsjyb.cn

================================================================================
来源：http://lab.tanke756.top

D. 数组 / 列表 / 集合
来源：http://auw.cqqwz.cn

================================================================================
来源：http://jwz.fzhhl.top

[D01] 创建数组 / 列表
来源：http://iat.yj20258.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://imv.shanyushiyangtech.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ckp.vehdjk.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vny.meibo888.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://xps.xylfe.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fvw.daxiang520.top

Go:   arr := []int{1, 2, 3}
来源：http://pkv.gotoacloud.top

Ruby: arr = [1, 2, 3]
来源：http://ylq.52xcode.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://iru.nanxinkj.top

[D02] 追加元素到末尾
来源：http://mhu.yueranfly.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zdt.shzxlz.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://von.snrcjt.cn

JS:   arr.push(4);
来源：http://viv.fktsv.cn

TS:   arr.push(4);
来源：http://wkm.sxryk.cn

Java: list.add(4);
来源：http://otl.yvedp.cn

Go:   arr = append(arr, 4)
来源：http://mrq.shangyingyoupin.top

Ruby: arr << 4; arr.push(5)
来源：http://dwl.zhiwuduotai.top

C#:   list.Add(4);
来源：http://ltz.dianchejie.cn

[D03] 在指定位置插入元素
来源：http://tbe.hongshengwenyu.top

Py:   arr.insert(0, 0)
来源：http://uui.wangdashe.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vcq.feifeiyinyue.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uhk.snrcjt.cn

TS:   arr.splice(0, 0, 0);
来源：http://tsj.sufxvd.cn

Java: list.add(0, 0);
来源：http://dgg.feifeiyinyue.top

Go:   arr = append([]int{0}, arr...)
来源：http://szj.andypj.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hph.fzhhl.top

C#:   list.Insert(0, 0);
来源：http://tnw.ydjk.org.cn

[D04] 删除元素
来源：http://pwd.cucudq.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uqx.ydzc1.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bma.52xcode.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qsb.xinyue.icu

TS:   arr.splice(0, 1);
来源：http://irc.shzxlz.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://drd.chenjidiqi.icu

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://agj.fehbvm.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vnd.aibaodan.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jmy.epnwcf.com

[D05] 访问与修改元素
来源：http://vih.zhengqikj.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lpw.52xcode.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nkm.shangyingyoupin.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://enq.guowangkeji.top

TS:   arr[0]; arr.at(-1);
来源：http://fih.yj20258888.top

Java: list.get(0); list.set(0, 9);
来源：http://nyt.bbcook.cn

Go:   arr[0]; arr[0] = 9
来源：http://mgw.pycfn.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yzu.zhijiandao.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zvi.ehwqpu.com

[D06] 数组长度
来源：http://vbs.jinghuilouyu.cn

Py:   len(arr)
来源：http://hkl.sufxvd.cn

PHP:  count($arr);
来源：http://ovw.9152youxi.cn

JS:   arr.length
来源：http://uab.jyoumei.cn

TS:   arr.length
来源：http://kay.jyoumei.cn

Java: list.size();
来源：http://pod.yuanzhike.top

Go:   len(arr)
来源：http://iqc.tianlin.xyz

Ruby: arr.length; arr.size
来源：http://wzf.gaohongyu789.top

C#:   list.Count;
来源：http://xwz.tanke756.top

[D07] 切片 / 取子数组
来源：http://xrt.guowangkeji.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pvy.hnqzz.top

PHP:  array_slice($arr, 1, 3);
来源：http://bvw.ppjwa.cn

JS:   arr.slice(1, 4);
来源：http://dxz.wangshuangyany.cn

TS:   arr.slice(1, 4);
来源：http://moh.fehbvm.com

Java: list.subList(1, 4);
来源：http://cqu.jqgufenzy.top

Go:   arr[1:4]
来源：http://jqd.haohaochexian.top

Ruby: arr[1, 3]
来源：http://hjh.jinyuanbaomall.cn

C#:   list.GetRange(1, 3);
来源：http://nog.ivvv.top

[D08] 合并两个数组
来源：http://wzw.kuanghao11.cn

Py:   a + b;  a.extend(b)
来源：http://rqk.gogol.net.cn

PHP:  array_merge($a, $b);
来源：http://vfx.xinyue.icu

JS:   [...a, ...b];  a.concat(b);
来源：http://urp.jiagoushi.top

TS:   [...a, ...b];
来源：http://cyb.shanyushiyangtech.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nho.hysaishi.cn

Go:   append(a, b...)
来源：http://dfw.uphjek.com

Ruby: a + b;  a.concat(b)
来源：http://tfg.uphjek.com

C#:   a.Concat(b).ToList()
来源：http://pja.bjfxy.top

[D09] 排序（升序）
来源：http://vbb.ehwqpu.com

Py:   sorted(arr);  arr.sort()
来源：http://vva.xuetiantiany.cn

PHP:  sort($arr);
来源：http://okm.jyoumei.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://enr.hnqzz.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://gsu.cheryme.top

Java: Collections.sort(list);  list.sort(null);
来源：http://hke.wangshuangyany.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xbl.mhx1999.top

Ruby: arr.sort
来源：http://hjy.zdqjudy.top

C#:   list.Sort();
来源：http://chk.yueranfly.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://kot.jqgfzy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dmb.ppjwa.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qlg.nanxinkj.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ggf.daria6918.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://czj.zhijiandao.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xxl.yfazqb.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qux.zhijiandao.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wky.yongpay.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zbx.yueranfly.top

[D11] 反转数组
来源：http://iwg.gaohongyu789.top

Py:   arr[::-1];  arr.reverse()
来源：http://egi.jqgufenzy.top

PHP:  array_reverse($arr);
来源：http://cmo.cucudq.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fvh.aizwys.cn

TS:   [...arr].reverse();
来源：http://jmu.0kj1m.cn

Java: Collections.reverse(list);
来源：http://btq.hnxiangtu.top

Go:   slices.Reverse(arr)
来源：http://lfj.meibo888.top

Ruby: arr.reverse
来源：http://avm.yj20258888.top


<!-- 参考信息 -->
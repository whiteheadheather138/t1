代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vzw.c1oappe.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://npd.wangshuangyany.cn

[B11] 生成数字序列 / 区间
来源：http://gzr.jianghu66.top

Py:   list(range(0, 10, 2))
来源：http://xri.jyoumei.cn

PHP:  range(0, 10, 2);
来源：http://gme.fengsongda.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tkh.cucudq.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mxx.guowangkeji.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rti.yuxming.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rfh.nanxinkj.top

Ruby: (0...10).step(2).to_a
来源：http://bty.tianlin.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gpx.redwolf501.top

[B12] 跳出多层循环
来源：http://ebz.zhijiandao.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ihh.feifeiyinyue.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://jld.cheryme.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://axa.52xcode.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ivq.yuanzhike.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ujn.yuanzhike.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://voc.bbcook.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fos.hammf.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bgw.aibaodan.cn

[B13] 判断是否为数字
来源：http://nix.chenzaomai.com

Py:   isinstance(x, (int, float))
来源：http://pfu.hnqzz.top

PHP:  is_numeric($x)
来源：http://mqd.yanxiufei.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://eyd.birdmap.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vmy.chenzaomai.com

Java: x instanceof Number
来源：http://uto.xziqi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://knc.ydjk.org.cn

Ruby: x.is_a?(Numeric)
来源：http://siv.meibo888.top

C#:   x is int or double or decimal
来源：http://pxf.birdmap.top

[B14] 判断值是否在集合内
来源：http://zab.sxryk.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yti.xinyue.icu

PHP:  in_array($x, [1, 2, 3], true)
来源：http://iei.chenzaomai.com

JS:   [1, 2, 3].includes(x)
来源：http://gfx.xinyue.icu

TS:   [1, 2, 3].includes(x)
来源：http://oov.andypj.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://zax.pycfn.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://liq.shanyushiyangkeji.top

Ruby: [1, 2, 3].include?(x)
来源：http://yew.xuanzx.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qlq.hnqzz.top

[B15] 布尔运算与取反
来源：http://qyq.mhx1999.top

Py:   a and b or not c
来源：http://ijn.jyoumei.cn

PHP:  $a && $b || !$c
来源：http://qtf.xziqi.cn

JS:   a && b || !c
来源：http://ufe.ydzc1.top

TS:   a && b || !c
来源：http://wha.316326.xyz

Java: a && b || !c
来源：http://aup.daxiang520.top

Go:   a && b || !c
来源：http://ovh.gotoacloud.top

Ruby: a && b || !c
来源：http://gpw.yfazqb.com

C#:   a && b || !c
来源：http://ymg.nanxinkj.top

[B16] 卫语句：不满足条件提前返回
来源：http://wio.yj202588.top

Py:   if not data: return
来源：http://vzc.chenzaomai.com

PHP:  if (!$data) { return; }
来源：http://nai.jianghu66.top

JS:   if (!data) return;
来源：http://aaq.snrcjt.cn

TS:   if (!data) return;
来源：http://btw.0kj1m.cn

Java: if (data == null) return;
来源：http://oet.gaohongyu789.top

Go:   if data == nil { return }
来源：http://zbg.chenjidiqi.icu

Ruby: return if data.nil?
来源：http://nxw.aibaodan.cn

C#:   if (data == null) return;
来源：http://uoo.tian-w.cn

================================================================================
来源：http://pbd.haohaochexian.top

C. 函数与作用域
来源：http://wxc.jqgfzy.top

================================================================================
来源：http://bve.cheryme.top

[C01] 定义函数
来源：http://eik.redwolf501.top

Py:   def add(a, b): return a + b
来源：http://poj.fehbvm.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dzn.c1oappe.top

JS:   function add(a, b) { return a + b; }
来源：http://myp.redwolf501.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vmx.bbcook.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gte.chenlongwang.top

Go:   func add(a, b int) int { return a + b }
来源：http://gmn.haohaochexian.top

Ruby: def add(a, b); a + b; end
来源：http://eer.wangshuangyany.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cal.cashguo.top

[C02] 默认参数
来源：http://udb.chenjidiqi.icu

Py:   def greet(name="World"): return name
来源：http://joi.nanxuanxn.top

PHP:  function greet($name = "World") { return $name; }
来源：http://mvl.smart0.xyz

JS:   function greet(name = "World") { return name; }
来源：http://ddd.jinqigfzy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ohm.yuxming.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://tjf.quarkkingdee.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ynp.ehwqpu.com

Ruby: def greet(name = "World") = name
来源：http://skn.yongpay.top

C#:   string Greet(string name = "World") => name;
来源：http://uvh.feifeiyinyue.top

[C03] 可变参数
来源：http://vlq.zhaomingkeji.xyz

Py:   def total(*args): return sum(args)
来源：http://xsr.zhengqikj.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fzx.guowangkeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cnm.gzhubu.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xbj.guannengcc.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jcg.sjlbkw.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://evl.snrcjt.cn

Ruby: def total(*nums); nums.sum; end
来源：http://iwx.gaohongyu789.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ljs.sxryk.cn

[C04] 命名参数 / 关键字参数
来源：http://rnq.c1oappe.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vqf.iojbl.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cxl.guannengcc.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gnz.fktsv.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wxy.wangdashe.top

Java: // 无：用 Builder 模式或 record
来源：http://ycz.xuanzx.com

Go:   // 无：用配置结构体参数
来源：http://gzs.fzhhl.top

Ruby: f(a: 1, b: 2)
来源：http://qtb.nanxuanxn.top

C#:   f(a: 1, b: 2)
来源：http://dzk.jinghuilouyu.cn

[C05] 返回多个值
来源：http://rvj.yj202588.top

Py:   return a, b
来源：http://nlr.shuidangran.top

PHP:  return [$a, $b];
来源：http://vrz.nwbrower.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://orx.sufxvd.cn

TS:   return { a, b };
来源：http://sdh.aibaodan.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://efi.mhx1999.top

Go:   return a, b
来源：http://ohm.jianghu66.top

Ruby: return a, b
来源：http://qpv.jlsjyb.cn

C#:   return (a, b);              // ValueTuple
来源：http://kxs.smart0.xyz

[C06] 匿名函数 / lambda
来源：http://foe.52xcode.cn

Py:   square = lambda x: x * x
来源：http://lqu.yj202588.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ttn.hywenlv.cn

JS:   const square = x => x * x;
来源：http://iws.jinyuanbaomall.cn

TS:   const square = (x: number): number => x * x;
来源：http://wcz.hammf.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pgc.xuanzx.com

Go:   sq := func(x int) int { return x * x }
来源：http://qlx.hammf.cn

Ruby: square = ->(x) { x * x }
来源：http://fxq.0kj1m.cn

C#:   Func<int, int> square = x => x * x;
来源：http://yzd.tianlin.xyz

[C07] 把函数作为参数传入
来源：http://smk.shuidangran.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://trm.cashguo.top

PHP:  array_map("strtoupper", $arr);
来源：http://axt.shanyushiyangtech.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bll.iojbl.cn

TS:   arr.map(String)
来源：http://zov.sjlbkw.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://omb.pengpengdd.cyou

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tqx.shanyushiyangkeji.top

Ruby: arr.map(&:upcase)
来源：http://rkn.jlsjyb.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cpo.zhixingplan.top

[C08] 闭包
来源：http://ayz.pengpengdd.cyou

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rhn.andypj.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://eup.havefunace.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xka.gaohongyu789.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jzc.zhiwuduotai.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wxd.zhaomingkeji.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://obq.meibo888.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xss.epnwcf.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://eqz.yanxiufei.cn

[C09] 递归
来源：http://ldt.aibaodan.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kdb.jinqigufen.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fav.andypj.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ywp.yvedp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ois.xinyue.icu

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mry.ivvv.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sbw.yonumen.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xmc.ybcxt.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zbg.smart0.xyz

[C10] 变量作用域
来源：http://lpe.hywenlv.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://evs.jyoumei.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rub.kuanghao11.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lwj.zhiwuduotai.top

TS:   同 JS
来源：http://rjk.jinqigufen.top

Java: 方法内为块级作用域
来源：http://rxw.yueranfly.top

Go:   花括号块级作用域
来源：http://ija.chenlongwang.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rrs.sufxvd.cn

C#:   块级作用域
来源：http://ilu.ydzc1.top

[C11] 模块导入与导出
来源：http://yws.vehdjk.com

Py:   from module import func
来源：http://eex.ehwqpu.com

PHP:  require "file.php";  或 use App\Service;
来源：http://qab.fengsongda.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://bmq.gaohongyu789.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ohu.epnwcf.com

Java: import java.util.List;
来源：http://uus.nanxinkj.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://krf.sysykeji.top

Ruby: require "json"; require_relative "./util"
来源：http://igy.jinqigufen.top

C#:   using System.Text;
来源：http://ehd.jqgfzy.top

[C12] 立即执行函数 IIFE
来源：http://rrp.yangfankeji.com

Py:   (lambda: print("run"))()
来源：http://aqi.shangyingyoupin.top

PHP:  (function () { echo "run"; })();
来源：http://nwz.pycfn.com

JS:   (() => { console.log("run"); })();
来源：http://smf.gzhubu.top

TS:   (() => { console.log("run"); })();
来源：http://sof.birdmap.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wki.birdmap.top

Go:   func() { fmt.Println("run") }()
来源：http://xjz.feifeiyinyue.top

Ruby: -> { puts "run" }.call
来源：http://ivy.xuanzx.com

C#:   // 无 IIFE：用静态构造函数
来源：http://xjf.jqgufenzy.top

[C13] 类型声明 / 类型注解
来源：http://pyi.zycfv.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vam.zhixingplan.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xou.hnqzz.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://edu.shanyushiyangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mmj.smart0.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://aoj.wangshuangyany.cn

Go:   func add(a, b int) int
来源：http://pdl.jinqigfzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ztb.yvedp.cn

C#:   int Add(int a, int b) => a + b;
来源：http://jls.quarkkingdee.top

[C14] 泛型函数
来源：http://gkv.jiagoushi.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jlr.daxiang520.top

PHP:  // 无泛型
来源：http://qio.9152youxi.cn

JS:   // 无泛型
来源：http://sfo.kuanghao11.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://itf.aibaodan.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wqi.xuanzx.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ait.zhiwuduotai.top

Ruby: # 无泛型
来源：http://haz.vqdsnc.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ygb.gogol.net.cn

[C15] 解构 / 展开参数
来源：http://fbc.shanyushiyangkeji.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fop.zhongyouzk.top

PHP:  [$a, $b] = $pair;
来源：http://nld.chenjidiqi.icu

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ucv.sweek.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tiu.zdbjq.cn

Java: // 无解构
来源：http://acv.zycfv.cn

Go:   // 无解构
来源：http://dpd.ehwqpu.com

Ruby: a, b = pair
来源：http://gbw.zhengqikj.top

C#:   var (a, b) = pair;
来源：http://avy.ydjk.org.cn

[C16] 函数 / 方法重载
来源：http://hmv.ydjk.org.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xtj.zhaomingkeji.xyz

PHP:  // 无重载
来源：http://rcm.bbcook.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://msg.cdnleiting.top

TS:   // 用联合类型或重载签名声明
来源：http://odc.shangyingyoupin.top

Java: void f(int a) {}  void f(String a) {}
来源：http://biy.xinyue.icu

Go:   // 无重载：用不同函数名
来源：http://ngn.zycfv.cn

Ruby: # 无重载：靠动态参数
来源：http://pwa.sufxvd.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ian.chenjidiqi.icu

================================================================================
来源：http://qxo.uphjek.com

D. 数组 / 列表 / 集合
来源：http://yvk.0kj1m.cn

================================================================================
来源：http://dgp.fzhhl.top

[D01] 创建数组 / 列表
来源：http://cqf.gaohongyu789.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://joa.epnwcf.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lhu.9152youxi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://oyo.ctjpmb.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://pld.fzhhl.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fqi.shangyingyoupin.top

Go:   arr := []int{1, 2, 3}
来源：http://mym.yvedp.cn

Ruby: arr = [1, 2, 3]
来源：http://olb.andypj.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pfi.zycfv.cn

[D02] 追加元素到末尾
来源：http://ifn.birdmap.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://plf.jyoumei.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qiz.gzhubu.top

JS:   arr.push(4);
来源：http://fnd.hnxiangtu.top

TS:   arr.push(4);
来源：http://siz.chenlongwang.top

Java: list.add(4);
来源：http://vqc.cashguo.top

Go:   arr = append(arr, 4)
来源：http://doc.cdnleiting.top

Ruby: arr << 4; arr.push(5)
来源：http://mpr.xingfuxueyuan.xyz

C#:   list.Add(4);
来源：http://pyl.snrcjt.cn

[D03] 在指定位置插入元素
来源：http://qvh.jqgfzy.top

Py:   arr.insert(0, 0)
来源：http://cuw.yangfankeji.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lul.fktsv.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fwm.tianlin.xyz

TS:   arr.splice(0, 0, 0);
来源：http://wuo.bjfxy.top

Java: list.add(0, 0);
来源：http://cai.gogol.net.cn

Go:   arr = append([]int{0}, arr...)
来源：http://mil.gzhubu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://aze.dashuyun.cn

C#:   list.Insert(0, 0);
来源：http://xtf.kuanghao11.cn

[D04] 删除元素
来源：http://xyl.hcnkem.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ylu.zhongyouzk.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jad.bbcook.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ofe.uphjek.com

TS:   arr.splice(0, 1);
来源：http://jft.shanyushiyangkeji.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://imz.zdbjq.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fwm.yj202588.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kba.ivvv.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://frf.hnxiangtu.top

[D05] 访问与修改元素
来源：http://pza.zdqjudy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vkc.jianghu66.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pch.chenlongwang.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lfq.dianchejie.cn

TS:   arr[0]; arr.at(-1);
来源：http://amr.redwolf501.top

Java: list.get(0); list.set(0, 9);
来源：http://inv.ybcxt.top

Go:   arr[0]; arr[0] = 9
来源：http://qhj.yj202588.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://aym.sweek.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xxl.xuetiantiany.cn

[D06] 数组长度
来源：http://lww.epnwcf.com

Py:   len(arr)
来源：http://ids.jianghu66.top

PHP:  count($arr);
来源：http://czg.gotoacloud.top

JS:   arr.length
来源：http://nau.shangyingyoupin.top

TS:   arr.length
来源：http://lgh.zhoulong.xyz

Java: list.size();
来源：http://lvb.52xcode.cn

Go:   len(arr)
来源：http://onv.yvedp.cn

Ruby: arr.length; arr.size
来源：http://bjy.nanxinkj.top

C#:   list.Count;
来源：http://yfd.cucudq.cn

[D07] 切片 / 取子数组
来源：http://yhc.cqqwz.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://krj.c1oappe.top

PHP:  array_slice($arr, 1, 3);
来源：http://ppq.iojbl.cn

JS:   arr.slice(1, 4);
来源：http://beg.yuanzhike.top

TS:   arr.slice(1, 4);
来源：http://qqs.jlsjyb.cn

Java: list.subList(1, 4);
来源：http://fte.pengpengdd.cyou

Go:   arr[1:4]
来源：http://yuo.hnxiangtu.top

Ruby: arr[1, 3]
来源：http://xdi.cheryme.top

C#:   list.GetRange(1, 3);
来源：http://qym.yj20258888.top

[D08] 合并两个数组
来源：http://pas.jinqigufen.top

Py:   a + b;  a.extend(b)
来源：http://pme.daria6918.cn

PHP:  array_merge($a, $b);
来源：http://yhe.hammf.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://mcy.ywan-chungtsiang.top

TS:   [...a, ...b];
来源：http://kht.fzhhl.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://uce.tarul.cn

Go:   append(a, b...)
来源：http://iid.kuanghao11.cn

Ruby: a + b;  a.concat(b)
来源：http://ked.cqqwz.cn

C#:   a.Concat(b).ToList()
来源：http://eop.hesvh.cn

[D09] 排序（升序）
来源：http://uut.shzxlz.cn

Py:   sorted(arr);  arr.sort()
来源：http://vvk.dashuyun.cn

PHP:  sort($arr);
来源：http://btt.yongpay.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bio.gzhubu.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://enu.zhiwuduotai.top

Java: Collections.sort(list);  list.sort(null);
来源：http://gny.birdmap.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zei.316326.xyz

Ruby: arr.sort
来源：http://qdq.xylfe.cn

C#:   list.Sort();
来源：http://rpx.zhiwuduotai.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://oje.xuanzx.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sjk.feifeiyinyue.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sbq.hnxiangtu.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lsh.yueranfly.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rpy.sufxvd.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jdf.0kj1m.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zaa.zycfv.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cut.fengsongda.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hni.gotoacloud.top

[D11] 反转数组
来源：http://sgi.zhengqikj.top

Py:   arr[::-1];  arr.reverse()
来源：http://bbp.jqgfzy.top

PHP:  array_reverse($arr);
来源：http://spy.hammf.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://syq.ydjk.org.cn


<!-- 参考信息 -->
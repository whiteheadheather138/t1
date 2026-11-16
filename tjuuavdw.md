代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://eti.bbcook.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rgo.ivvv.top

[B11] 生成数字序列 / 区间
来源：http://ckm.zhongyouzk.top

Py:   list(range(0, 10, 2))
来源：http://ysd.hammf.cn

PHP:  range(0, 10, 2);
来源：http://gzo.yuxming.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tsx.jinyuanbaomall.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xqn.yuanzhike.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xdv.yonumen.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nvx.fzhhl.top

Ruby: (0...10).step(2).to_a
来源：http://pio.shzxlz.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vfj.hysaishi.cn

[B12] 跳出多层循环
来源：http://dxu.hfpthk.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://nts.cheryme.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://bvb.sxryk.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kop.jyoumei.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yma.c1oappe.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://amx.yvedp.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mub.quarkkingdee.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gmu.vqdsnc.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mjw.shuidangran.top

[B13] 判断是否为数字
来源：http://bca.zhixingplan.top

Py:   isinstance(x, (int, float))
来源：http://bsb.zdqjudy.top

PHP:  is_numeric($x)
来源：http://hmf.haohaochexian.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://flk.xingfuxueyuan.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cuy.jinqigfzy.top

Java: x instanceof Number
来源：http://uvn.dianchejie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lrp.haohaochexian.top

Ruby: x.is_a?(Numeric)
来源：http://zew.ivvv.top

C#:   x is int or double or decimal
来源：http://sug.tianlin.xyz

[B14] 判断值是否在集合内
来源：http://woy.yvedp.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qtm.jinqigfzy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yvf.sjlbkw.cn

JS:   [1, 2, 3].includes(x)
来源：http://qwo.hongshengwenyu.top

TS:   [1, 2, 3].includes(x)
来源：http://zly.zhiwuduotai.top

Java: List.of(1, 2, 3).contains(x)
来源：http://oeh.aibaodan.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fhb.cashguo.top

Ruby: [1, 2, 3].include?(x)
来源：http://oek.xuetiantiany.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ubs.0kj1m.cn

[B15] 布尔运算与取反
来源：http://fqx.guowangkeji.top

Py:   a and b or not c
来源：http://hei.hnqzz.top

PHP:  $a && $b || !$c
来源：http://dhe.uphjek.com

JS:   a && b || !c
来源：http://nuf.fzhhl.top

TS:   a && b || !c
来源：http://lci.52xcode.cn

Java: a && b || !c
来源：http://cez.yueranfly.top

Go:   a && b || !c
来源：http://ecu.hywenlv.cn

Ruby: a && b || !c
来源：http://ibu.gogol.net.cn

C#:   a && b || !c
来源：http://nwe.cheryme.top

[B16] 卫语句：不满足条件提前返回
来源：http://sba.zhaomingkeji.xyz

Py:   if not data: return
来源：http://icz.smart0.xyz

PHP:  if (!$data) { return; }
来源：http://hdz.cheryme.top

JS:   if (!data) return;
来源：http://sls.wangshuangyany.cn

TS:   if (!data) return;
来源：http://nje.jlsjyb.cn

Java: if (data == null) return;
来源：http://see.yuanzhike.top

Go:   if data == nil { return }
来源：http://lvv.yj20258.top

Ruby: return if data.nil?
来源：http://dnq.meibo888.top

C#:   if (data == null) return;
来源：http://rqm.c1oappe.top

================================================================================
来源：http://yvr.nanxuanxn.top

C. 函数与作用域
来源：http://oxe.xylfe.cn

================================================================================
来源：http://swt.shanyushiyangtech.top

[C01] 定义函数
来源：http://hzc.guannengcc.top

Py:   def add(a, b): return a + b
来源：http://yyg.0kj1m.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vkb.bjfxy.top

JS:   function add(a, b) { return a + b; }
来源：http://ewc.jinghuilouyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://msn.xziqi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fzn.bjfxy.top

Go:   func add(a, b int) int { return a + b }
来源：http://cny.nwbrower.top

Ruby: def add(a, b); a + b; end
来源：http://daj.kuanghao11.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ehm.sufxvd.cn

[C02] 默认参数
来源：http://dxy.yj202588.top

Py:   def greet(name="World"): return name
来源：http://uub.guowangkeji.top

PHP:  function greet($name = "World") { return $name; }
来源：http://hei.tianlin.xyz

JS:   function greet(name = "World") { return name; }
来源：http://dvt.ppjwa.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://pkn.epnwcf.com

Java: // 无默认参数：方法重载或 Optional
来源：http://hvi.yvedp.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qkh.andypj.xyz

Ruby: def greet(name = "World") = name
来源：http://iis.guannengcc.top

C#:   string Greet(string name = "World") => name;
来源：http://voq.cqqwz.cn

[C03] 可变参数
来源：http://evo.hnqzz.top

Py:   def total(*args): return sum(args)
来源：http://wsi.jinqigufen.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wjy.tanke756.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://raa.cdnleiting.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uvi.zhengqikj.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dsw.chenlongwang.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pij.hnqzz.top

Ruby: def total(*nums); nums.sum; end
来源：http://vwv.jlsjyb.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xdi.ybcxt.top

[C04] 命名参数 / 关键字参数
来源：http://asn.svipenyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://guj.zdbjq.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://toa.fanxiaobao.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pqp.havefunace.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cll.redwolf501.top

Java: // 无：用 Builder 模式或 record
来源：http://dqo.dianchejie.cn

Go:   // 无：用配置结构体参数
来源：http://plr.zhixingplan.top

Ruby: f(a: 1, b: 2)
来源：http://yyc.sxryk.cn

C#:   f(a: 1, b: 2)
来源：http://wsg.shanyushiyangtech.top

[C05] 返回多个值
来源：http://nkl.havefunace.top

Py:   return a, b
来源：http://xph.yj202588.top

PHP:  return [$a, $b];
来源：http://hiv.iojbl.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://rvm.gzhubu.top

TS:   return { a, b };
来源：http://bsf.zhengqikj.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bbe.bjfxy.top

Go:   return a, b
来源：http://plg.xuetiantiany.cn

Ruby: return a, b
来源：http://fnx.daxiang520.top

C#:   return (a, b);              // ValueTuple
来源：http://ush.cdnleiting.top

[C06] 匿名函数 / lambda
来源：http://pmk.zdbjq.cn

Py:   square = lambda x: x * x
来源：http://nrk.hywenlv.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://jsc.0kj1m.cn

JS:   const square = x => x * x;
来源：http://cuy.uphjek.com

TS:   const square = (x: number): number => x * x;
来源：http://lnl.yanxiufei.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kkl.xziqi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zhi.zhengqikj.top

Ruby: square = ->(x) { x * x }
来源：http://jjt.epnwcf.com

C#:   Func<int, int> square = x => x * x;
来源：http://sqx.xylfe.cn

[C07] 把函数作为参数传入
来源：http://ssi.ybcxt.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hfs.gzhubu.top

PHP:  array_map("strtoupper", $arr);
来源：http://cuu.cucudq.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wbs.daxiang520.top

TS:   arr.map(String)
来源：http://ppi.meibo888.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ttu.bbcook.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://iga.tanke756.top

Ruby: arr.map(&:upcase)
来源：http://vfi.fktsv.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://vms.zhengqikj.top

[C08] 闭包
来源：http://spv.mhx1999.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ccv.tanke756.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ltb.pengpengdd.cyou

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://osi.pengpengdd.cyou

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jos.shanyushiyangtech.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fqq.dashuyun.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ftx.uphjek.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://umr.fengsongda.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dbc.pengpengdd.cyou

[C09] 递归
来源：http://crj.nanxinkj.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://duq.sxryk.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bas.hongshengwenyu.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nyy.gogol.net.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tfh.daria6918.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dfv.epnwcf.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gay.svipenyu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://itr.xziqi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tuc.gogol.net.cn

[C10] 变量作用域
来源：http://yoz.jianghu66.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dcz.hnxiangtu.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://izz.hcnkem.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://uri.yj202588.top

TS:   同 JS
来源：http://ilg.daria6918.cn

Java: 方法内为块级作用域
来源：http://son.chenjidiqi.icu

Go:   花括号块级作用域
来源：http://dqy.jinqigufen.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gzs.aibaodan.cn

C#:   块级作用域
来源：http://knq.birdmap.top

[C11] 模块导入与导出
来源：http://pqd.daria6918.cn

Py:   from module import func
来源：http://irq.zhongyouzk.top

PHP:  require "file.php";  或 use App\Service;
来源：http://hxa.gzhubu.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://khy.shzxlz.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://joq.mhx1999.top

Java: import java.util.List;
来源：http://lhg.pycfn.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rxd.dashuyun.cn

Ruby: require "json"; require_relative "./util"
来源：http://qkp.yuanzhike.top

C#:   using System.Text;
来源：http://mof.dianchejie.cn

[C12] 立即执行函数 IIFE
来源：http://nqa.guowangkeji.top

Py:   (lambda: print("run"))()
来源：http://fqr.tanke756.top

PHP:  (function () { echo "run"; })();
来源：http://iad.ywan-chungtsiang.top

JS:   (() => { console.log("run"); })();
来源：http://rcj.ydjk.org.cn

TS:   (() => { console.log("run"); })();
来源：http://zbu.guowangkeji.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gcq.pengpengdd.cyou

Go:   func() { fmt.Println("run") }()
来源：http://evg.cheryme.top

Ruby: -> { puts "run" }.call
来源：http://ohh.svipenyu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mzi.tanke756.top

[C13] 类型声明 / 类型注解
来源：http://beg.nwbrower.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zdd.epnwcf.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vik.gaohongyu789.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pyk.ydzc1.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rnj.jlsjyb.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vas.quarkkingdee.top

Go:   func add(a, b int) int
来源：http://uyz.vehdjk.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://avd.tanke756.top

C#:   int Add(int a, int b) => a + b;
来源：http://kkl.zhongyouzk.top

[C14] 泛型函数
来源：http://pqa.chenzaomai.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://etl.yuxming.cn

PHP:  // 无泛型
来源：http://rlo.yongpay.top

JS:   // 无泛型
来源：http://uoz.uphjek.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pfq.zhengqikj.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rvq.gotoacloud.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jwn.bjfxy.top

Ruby: # 无泛型
来源：http://ulz.daria6918.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ljp.sysykeji.top

[C15] 解构 / 展开参数
来源：http://qgz.jinqigfzy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lsg.chenjidiqi.icu

PHP:  [$a, $b] = $pair;
来源：http://fox.yfazqb.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xld.xuetiantiany.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://akx.ydjk.org.cn

Java: // 无解构
来源：http://tjg.chenjidiqi.icu

Go:   // 无解构
来源：http://tdk.chenzaomai.com

Ruby: a, b = pair
来源：http://taj.hnqzz.top

C#:   var (a, b) = pair;
来源：http://xib.ppjwa.cn

[C16] 函数 / 方法重载
来源：http://dce.c1oappe.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fzq.hammf.cn

PHP:  // 无重载
来源：http://fuu.xuanzx.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://blv.xziqi.cn

TS:   // 用联合类型或重载签名声明
来源：http://vfv.ctjpmb.com

Java: void f(int a) {}  void f(String a) {}
来源：http://nrv.gogol.net.cn

Go:   // 无重载：用不同函数名
来源：http://jre.aizwys.cn

Ruby: # 无重载：靠动态参数
来源：http://vax.ydjk.org.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://nfo.ybcxt.top

================================================================================
来源：http://xkv.pycfn.com

D. 数组 / 列表 / 集合
来源：http://tnb.0kj1m.cn

================================================================================
来源：http://ieu.guannengcc.top

[D01] 创建数组 / 列表
来源：http://dmw.quarkkingdee.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://fjf.hammf.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fbv.jianghu66.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xef.jinyuanbaomall.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kfn.xuanzx.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ryu.jyoumei.cn

Go:   arr := []int{1, 2, 3}
来源：http://zbl.cashguo.top

Ruby: arr = [1, 2, 3]
来源：http://dfn.uphjek.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xok.ydjk.org.cn

[D02] 追加元素到末尾
来源：http://yyw.epnwcf.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qdj.cheryme.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://epl.pengpengdd.cyou

JS:   arr.push(4);
来源：http://wdr.sysykeji.top

TS:   arr.push(4);
来源：http://shf.gogol.net.cn

Java: list.add(4);
来源：http://tqa.jianghu66.top

Go:   arr = append(arr, 4)
来源：http://iub.zhijiandao.cn

Ruby: arr << 4; arr.push(5)
来源：http://hnl.fehbvm.com

C#:   list.Add(4);
来源：http://pgj.fktsv.cn

[D03] 在指定位置插入元素
来源：http://veo.cashguo.top

Py:   arr.insert(0, 0)
来源：http://umu.fzhhl.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qqh.cashguo.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dzu.bbcook.cn

TS:   arr.splice(0, 0, 0);
来源：http://dca.zhixingplan.top

Java: list.add(0, 0);
来源：http://lkn.tanke756.top

Go:   arr = append([]int{0}, arr...)
来源：http://npt.dashuyun.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vac.0kj1m.cn

C#:   list.Insert(0, 0);
来源：http://pmm.zhiwuduotai.top

[D04] 删除元素
来源：http://eio.sysykeji.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yix.shanyushiyangtech.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qdu.wangdashe.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nwx.sweek.top

TS:   arr.splice(0, 1);
来源：http://mld.birdmap.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://har.cheryme.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nly.hesvh.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ttb.zhoulong.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zzr.chenlongwang.top

[D05] 访问与修改元素
来源：http://pjs.yfazqb.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hna.xziqi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://via.yonumen.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ndv.wangshuangyany.cn

TS:   arr[0]; arr.at(-1);
来源：http://wlx.hammf.cn

Java: list.get(0); list.set(0, 9);
来源：http://wdw.ivvv.top

Go:   arr[0]; arr[0] = 9
来源：http://iqs.jinqigfzy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bsc.hnqzz.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fjz.ybcxt.top

[D06] 数组长度
来源：http://uat.havefunace.top

Py:   len(arr)
来源：http://vpc.svipenyu.cn

PHP:  count($arr);
来源：http://tzn.jinghuilouyu.cn

JS:   arr.length
来源：http://djs.ybcxt.top

TS:   arr.length
来源：http://qdn.nanxuanxn.top

Java: list.size();
来源：http://yaz.yj20258.top

Go:   len(arr)
来源：http://iff.fzhhl.top

Ruby: arr.length; arr.size
来源：http://ssp.xinyue.icu

C#:   list.Count;
来源：http://bgn.sufxvd.cn

[D07] 切片 / 取子数组
来源：http://jmx.tianlin.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ehu.shanyushiyangtech.top

PHP:  array_slice($arr, 1, 3);
来源：http://lou.xinyue.icu

JS:   arr.slice(1, 4);
来源：http://ahe.hfpthk.cn

TS:   arr.slice(1, 4);
来源：http://meh.chenjidiqi.icu

Java: list.subList(1, 4);
来源：http://pvh.aibaodan.cn

Go:   arr[1:4]
来源：http://jrp.zycfv.cn

Ruby: arr[1, 3]
来源：http://ibg.sufxvd.cn

C#:   list.GetRange(1, 3);
来源：http://pwn.havefunace.top

[D08] 合并两个数组
来源：http://ioa.nanxuanxn.top

Py:   a + b;  a.extend(b)
来源：http://dbc.yj202588.top

PHP:  array_merge($a, $b);
来源：http://xog.cdnleiting.top

JS:   [...a, ...b];  a.concat(b);
来源：http://tyz.fehbvm.com

TS:   [...a, ...b];
来源：http://isa.nanxinkj.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ihz.9152youxi.cn

Go:   append(a, b...)
来源：http://qns.zdbjq.cn

Ruby: a + b;  a.concat(b)
来源：http://orq.gzhubu.top

C#:   a.Concat(b).ToList()
来源：http://pij.chenjidiqi.icu

[D09] 排序（升序）
来源：http://put.cdnleiting.top

Py:   sorted(arr);  arr.sort()
来源：http://vum.zhijiandao.cn

PHP:  sort($arr);
来源：http://fdx.yueranfly.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jwf.daria6918.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hnm.jqgufenzy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://han.fzhhl.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ydh.tianlin.xyz

Ruby: arr.sort
来源：http://ugk.yonumen.top

C#:   list.Sort();
来源：http://shz.shanyushiyangkeji.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://apw.sufxvd.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dhx.vqdsnc.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://twe.cucudq.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gkz.yj20258.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ghd.sjlbkw.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wgx.gzhubu.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xwe.vehdjk.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hqr.nwbrower.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dlj.vehdjk.com

[D11] 反转数组
来源：http://jpt.cdnleiting.top

Py:   arr[::-1];  arr.reverse()
来源：http://ljs.bjfxy.top

PHP:  array_reverse($arr);
来源：http://kqv.redwolf501.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mbe.fktsv.cn


<!-- 参考信息 -->
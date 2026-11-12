代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mct.cqqwz.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://irz.ivvv.top

[B11] 生成数字序列 / 区间
来源：http://ysq.yj202588.top

Py:   list(range(0, 10, 2))
来源：http://jeb.chenzaomai.com

PHP:  range(0, 10, 2);
来源：http://jqu.hesvh.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://flt.jiagoushi.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pxs.fanxiaobao.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://inn.sxryk.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ocs.jiagoushi.top

Ruby: (0...10).step(2).to_a
来源：http://nsl.ivvv.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tzi.yuanzhike.top

[B12] 跳出多层循环
来源：http://cxx.yfazqb.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://bpz.zdbjq.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://izx.hysaishi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jcd.hesvh.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pys.haohaochexian.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://evx.chenzaomai.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://oji.zhongyouzk.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nmj.yj202588.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://adp.jianghu66.top

[B13] 判断是否为数字
来源：http://oky.sjlbkw.cn

Py:   isinstance(x, (int, float))
来源：http://yxj.yj20258.top

PHP:  is_numeric($x)
来源：http://ypq.dianchejie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tbi.aizwys.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nho.316326.xyz

Java: x instanceof Number
来源：http://xdb.daria6918.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bzf.ehwqpu.com

Ruby: x.is_a?(Numeric)
来源：http://ckh.wangdashe.top

C#:   x is int or double or decimal
来源：http://cfg.bbcook.cn

[B14] 判断值是否在集合内
来源：http://spg.jinyuanbaomall.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://afh.sxryk.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lvc.ctjpmb.com

JS:   [1, 2, 3].includes(x)
来源：http://wgv.jlsjyb.cn

TS:   [1, 2, 3].includes(x)
来源：http://knw.yuxming.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://bkf.vehdjk.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fle.bjfxy.top

Ruby: [1, 2, 3].include?(x)
来源：http://xow.shuidangran.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://loo.jinqigufen.top

[B15] 布尔运算与取反
来源：http://sci.yj202588.top

Py:   a and b or not c
来源：http://vau.xuanzx.com

PHP:  $a && $b || !$c
来源：http://tyk.c1oappe.top

JS:   a && b || !c
来源：http://zyx.jinqigufen.top

TS:   a && b || !c
来源：http://ztk.birdmap.top

Java: a && b || !c
来源：http://pjy.fehbvm.com

Go:   a && b || !c
来源：http://loz.yonumen.top

Ruby: a && b || !c
来源：http://ege.svipenyu.cn

C#:   a && b || !c
来源：http://ido.guowangkeji.top

[B16] 卫语句：不满足条件提前返回
来源：http://hen.jqgufenzy.top

Py:   if not data: return
来源：http://jxy.jinghuilouyu.cn

PHP:  if (!$data) { return; }
来源：http://bxc.sxryk.cn

JS:   if (!data) return;
来源：http://fds.hesvh.cn

TS:   if (!data) return;
来源：http://vbz.snrcjt.cn

Java: if (data == null) return;
来源：http://uiw.meibo888.top

Go:   if data == nil { return }
来源：http://qih.zhengqikj.top

Ruby: return if data.nil?
来源：http://ylz.tanke756.top

C#:   if (data == null) return;
来源：http://wtx.yangfankeji.com

================================================================================
来源：http://vmn.hnqzz.top

C. 函数与作用域
来源：http://bgu.yuxming.cn

================================================================================
来源：http://afe.ppjwa.cn

[C01] 定义函数
来源：http://ozy.xuanzx.com

Py:   def add(a, b): return a + b
来源：http://rqd.xziqi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qsy.zhengqikj.top

JS:   function add(a, b) { return a + b; }
来源：http://rhh.chenzaomai.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lhk.zhiwuduotai.top

Java: static int add(int a, int b) { return a + b; }
来源：http://bgu.sufxvd.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hcn.yongpay.top

Ruby: def add(a, b); a + b; end
来源：http://sev.ywan-chungtsiang.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mah.jlsjyb.cn

[C02] 默认参数
来源：http://iny.zdqjudy.top

Py:   def greet(name="World"): return name
来源：http://yll.sxryk.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dyo.chenzaomai.com

JS:   function greet(name = "World") { return name; }
来源：http://ufj.xylfe.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://chn.svipenyu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://spa.chenjidiqi.icu

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mqb.chenjidiqi.icu

Ruby: def greet(name = "World") = name
来源：http://rhm.jlsjyb.cn

C#:   string Greet(string name = "World") => name;
来源：http://zxj.uphjek.com

[C03] 可变参数
来源：http://qyr.yongpay.top

Py:   def total(*args): return sum(args)
来源：http://mut.tanke756.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://myn.zycfv.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://csc.andypj.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cuv.kuanghao11.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sdh.ctjpmb.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gnn.mhx1999.top

Ruby: def total(*nums); nums.sum; end
来源：http://ciw.uphjek.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zxi.hammf.cn

[C04] 命名参数 / 关键字参数
来源：http://gvr.svipenyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xxt.yanxiufei.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yzj.bjfxy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zaw.jianghu66.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://duh.shuidangran.top

Java: // 无：用 Builder 模式或 record
来源：http://jed.fanxiaobao.xyz

Go:   // 无：用配置结构体参数
来源：http://fhu.dashuyun.cn

Ruby: f(a: 1, b: 2)
来源：http://spt.nwbrower.top

C#:   f(a: 1, b: 2)
来源：http://suj.xylfe.cn

[C05] 返回多个值
来源：http://bly.haohaochexian.top

Py:   return a, b
来源：http://lmn.hnxiangtu.top

PHP:  return [$a, $b];
来源：http://sgs.smart0.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://rrw.fengsongda.top

TS:   return { a, b };
来源：http://hnb.hcnkem.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ycg.nwbrower.top

Go:   return a, b
来源：http://mvu.hysaishi.cn

Ruby: return a, b
来源：http://ads.dianchejie.cn

C#:   return (a, b);              // ValueTuple
来源：http://ewi.ctjpmb.com

[C06] 匿名函数 / lambda
来源：http://wqw.yuanzhike.top

Py:   square = lambda x: x * x
来源：http://vhe.jyoumei.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://vtj.shanyushiyangkeji.top

JS:   const square = x => x * x;
来源：http://avd.dianchejie.cn

TS:   const square = (x: number): number => x * x;
来源：http://xzb.dianchejie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://oxo.dashuyun.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dns.feifeiyinyue.top

Ruby: square = ->(x) { x * x }
来源：http://bag.ppjwa.cn

C#:   Func<int, int> square = x => x * x;
来源：http://pgp.xuetiantiany.cn

[C07] 把函数作为参数传入
来源：http://pfz.0kj1m.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yhx.zhiwuduotai.top

PHP:  array_map("strtoupper", $arr);
来源：http://ocy.chenjidiqi.icu

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://znw.xingfuxueyuan.xyz

TS:   arr.map(String)
来源：http://kxu.xingfuxueyuan.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://anf.yj202588.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kpg.zycfv.cn

Ruby: arr.map(&:upcase)
来源：http://gep.zhijiandao.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://rvp.vehdjk.com

[C08] 闭包
来源：http://itl.bbcook.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wue.jinyuanbaomall.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xzc.svipenyu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tly.ydzc1.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cbc.hammf.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://asn.ybcxt.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ynu.shanyushiyangkeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lbn.xuetiantiany.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jzy.hcnkem.com

[C09] 递归
来源：http://hys.chenjidiqi.icu

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wql.gzhubu.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://var.tianlin.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://klj.tanke756.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sxi.zhixingplan.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rpi.chenjidiqi.icu

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://duo.xuanzx.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hwn.aibaodan.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ejd.jiagoushi.top

[C10] 变量作用域
来源：http://lvw.gaohongyu789.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nxt.hammf.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ehh.zhongyouzk.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ijj.xuanzx.com

TS:   同 JS
来源：http://zfe.cucudq.cn

Java: 方法内为块级作用域
来源：http://zsl.zhoulong.xyz

Go:   花括号块级作用域
来源：http://zmm.hnqzz.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cxp.zdqjudy.top

C#:   块级作用域
来源：http://res.zhaomingkeji.xyz

[C11] 模块导入与导出
来源：http://kuo.shuidangran.top

Py:   from module import func
来源：http://ojw.yuanzhike.top

PHP:  require "file.php";  或 use App\Service;
来源：http://gfq.uphjek.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://ckt.zhengqikj.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ilj.yonumen.top

Java: import java.util.List;
来源：http://idz.fanxiaobao.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://eff.xuanzx.com

Ruby: require "json"; require_relative "./util"
来源：http://xyy.jqgfzy.top

C#:   using System.Text;
来源：http://dmu.mhx1999.top

[C12] 立即执行函数 IIFE
来源：http://kwl.zdqjudy.top

Py:   (lambda: print("run"))()
来源：http://liz.fzhhl.top

PHP:  (function () { echo "run"; })();
来源：http://ifo.pengpengdd.cyou

JS:   (() => { console.log("run"); })();
来源：http://ijy.hywenlv.cn

TS:   (() => { console.log("run"); })();
来源：http://pto.zhengqikj.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fct.feifeiyinyue.top

Go:   func() { fmt.Println("run") }()
来源：http://jdd.wangdashe.top

Ruby: -> { puts "run" }.call
来源：http://mil.jinqigufen.top

C#:   // 无 IIFE：用静态构造函数
来源：http://wyg.cucudq.cn

[C13] 类型声明 / 类型注解
来源：http://ggz.shanyushiyangtech.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ptu.vehdjk.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qsm.c1oappe.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nwx.quarkkingdee.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://agj.yanxiufei.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fhw.jinghuilouyu.cn

Go:   func add(a, b int) int
来源：http://coj.zycfv.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://geg.yueranfly.top

C#:   int Add(int a, int b) => a + b;
来源：http://esj.xuanzx.com

[C14] 泛型函数
来源：http://sht.vehdjk.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://znd.xylfe.cn

PHP:  // 无泛型
来源：http://jit.hnqzz.top

JS:   // 无泛型
来源：http://dai.c1oappe.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rwm.yangfankeji.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fll.yj202588.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hpf.tianlin.xyz

Ruby: # 无泛型
来源：http://qna.jinghuilouyu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kch.xylfe.cn

[C15] 解构 / 展开参数
来源：http://lrs.yuxming.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wmy.zhixingplan.top

PHP:  [$a, $b] = $pair;
来源：http://yae.daxiang520.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kem.wangshuangyany.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wmh.fzhhl.top

Java: // 无解构
来源：http://nyt.hysaishi.cn

Go:   // 无解构
来源：http://lxs.epnwcf.com

Ruby: a, b = pair
来源：http://pfl.redwolf501.top

C#:   var (a, b) = pair;
来源：http://gwn.cdnleiting.top

[C16] 函数 / 方法重载
来源：http://xny.yuxming.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://shx.sweek.top

PHP:  // 无重载
来源：http://ibo.yongpay.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://shg.fengsongda.top

TS:   // 用联合类型或重载签名声明
来源：http://gfm.ydjk.org.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://oaa.chenjidiqi.icu

Go:   // 无重载：用不同函数名
来源：http://qfa.yonumen.top

Ruby: # 无重载：靠动态参数
来源：http://mkd.hysaishi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xcp.andypj.xyz

================================================================================
来源：http://vty.jianghu66.top

D. 数组 / 列表 / 集合
来源：http://gep.nanxuanxn.top

================================================================================
来源：http://get.chenjidiqi.icu

[D01] 创建数组 / 列表
来源：http://iik.cashguo.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://cne.yongpay.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qfg.cheryme.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cyd.zycfv.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://brv.zhengqikj.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cjk.shanyushiyangkeji.top

Go:   arr := []int{1, 2, 3}
来源：http://tuw.kuanghao11.cn

Ruby: arr = [1, 2, 3]
来源：http://lsq.cdnleiting.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hlt.pengpengdd.cyou

[D02] 追加元素到末尾
来源：http://riy.pycfn.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wqj.uphjek.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qfm.shanyushiyangtech.top

JS:   arr.push(4);
来源：http://jml.0kj1m.cn

TS:   arr.push(4);
来源：http://jxn.zhoulong.xyz

Java: list.add(4);
来源：http://erq.cucudq.cn

Go:   arr = append(arr, 4)
来源：http://fem.zhiwuduotai.top

Ruby: arr << 4; arr.push(5)
来源：http://axb.guannengcc.top

C#:   list.Add(4);
来源：http://kof.zycfv.cn

[D03] 在指定位置插入元素
来源：http://iln.jinqigfzy.top

Py:   arr.insert(0, 0)
来源：http://ays.c1oappe.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gwq.yangfankeji.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rgw.9152youxi.cn

TS:   arr.splice(0, 0, 0);
来源：http://jta.shanyushiyangtech.top

Java: list.add(0, 0);
来源：http://ncw.quarkkingdee.top

Go:   arr = append([]int{0}, arr...)
来源：http://qiu.52xcode.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://doo.jyoumei.cn

C#:   list.Insert(0, 0);
来源：http://acm.ybcxt.top

[D04] 删除元素
来源：http://rmo.xinyue.icu

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vsg.pengpengdd.cyou

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hxl.zhixingplan.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ohx.ppjwa.cn

TS:   arr.splice(0, 1);
来源：http://dvo.xziqi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jtu.ydzc1.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://haj.cqqwz.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fmy.vehdjk.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uuo.nanxinkj.top

[D05] 访问与修改元素
来源：http://qlz.nwbrower.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://per.yj20258888.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yrg.wangshuangyany.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fby.shuidangran.top

TS:   arr[0]; arr.at(-1);
来源：http://byf.0kj1m.cn

Java: list.get(0); list.set(0, 9);
来源：http://wmw.xinyue.icu

Go:   arr[0]; arr[0] = 9
来源：http://oxo.iojbl.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hyd.yonumen.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rtb.ivvv.top

[D06] 数组长度
来源：http://vqe.dashuyun.cn

Py:   len(arr)
来源：http://yvk.gogol.net.cn

PHP:  count($arr);
来源：http://zpe.guannengcc.top

JS:   arr.length
来源：http://zec.tianlin.xyz

TS:   arr.length
来源：http://fvp.hcnkem.com

Java: list.size();
来源：http://hgn.fanxiaobao.xyz

Go:   len(arr)
来源：http://kob.chenjidiqi.icu

Ruby: arr.length; arr.size
来源：http://ynx.yonumen.top

C#:   list.Count;
来源：http://yvk.nanxuanxn.top

[D07] 切片 / 取子数组
来源：http://har.gaohongyu789.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wnw.gaohongyu789.top

PHP:  array_slice($arr, 1, 3);
来源：http://uys.zycfv.cn

JS:   arr.slice(1, 4);
来源：http://pch.ybcxt.top

TS:   arr.slice(1, 4);
来源：http://glh.jinghuilouyu.cn

Java: list.subList(1, 4);
来源：http://mft.vehdjk.com

Go:   arr[1:4]
来源：http://cju.zhongyouzk.top

Ruby: arr[1, 3]
来源：http://zvg.fengsongda.top

C#:   list.GetRange(1, 3);
来源：http://odl.yfazqb.com

[D08] 合并两个数组
来源：http://bfr.52xcode.cn

Py:   a + b;  a.extend(b)
来源：http://ahl.xuanzx.com

PHP:  array_merge($a, $b);
来源：http://bbr.shangyingyoupin.top

JS:   [...a, ...b];  a.concat(b);
来源：http://nse.yangfankeji.com

TS:   [...a, ...b];
来源：http://qxl.ppjwa.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tpu.ybcxt.top

Go:   append(a, b...)
来源：http://dhl.zhengqikj.top

Ruby: a + b;  a.concat(b)
来源：http://kry.jlsjyb.cn

C#:   a.Concat(b).ToList()
来源：http://vlm.smart0.xyz

[D09] 排序（升序）
来源：http://ugx.316326.xyz

Py:   sorted(arr);  arr.sort()
来源：http://rpg.sjlbkw.cn

PHP:  sort($arr);
来源：http://myt.jinyuanbaomall.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jfb.xingfuxueyuan.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://kbo.gogol.net.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ctk.nwbrower.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xol.ivvv.top

Ruby: arr.sort
来源：http://sgp.xziqi.cn

C#:   list.Sort();
来源：http://bqf.cqqwz.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://wuz.yj202588.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hea.fktsv.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://raq.zycfv.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lku.mhx1999.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ikn.epnwcf.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lji.zhaomingkeji.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://och.meibo888.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gun.guowangkeji.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hso.kuanghao11.cn

[D11] 反转数组
来源：http://yhk.aibaodan.cn

Py:   arr[::-1];  arr.reverse()
来源：http://fju.yuanzhike.top

PHP:  array_reverse($arr);
来源：http://edu.guannengcc.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zkb.xinyue.icu


<!-- 参考信息 -->
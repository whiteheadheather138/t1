代发 wailian999

PHP:  range(0, 10, 2);
来源：http://zrm.hfpthk.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lkt.hysaishi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lzm.shzxlz.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://auv.hcnkem.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lha.ywan-chungtsiang.top

Ruby: (0...10).step(2).to_a
来源：http://cpv.aibaodan.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bpr.jyoumei.cn

[B12] 跳出多层循环
来源：http://vsr.ppjwa.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wak.smart0.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://izt.0kj1m.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gaz.yvedp.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qcx.fehbvm.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://suf.quarkkingdee.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jjx.yangfankeji.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kyn.jinqigfzy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://loz.vehdjk.com

[B13] 判断是否为数字
来源：http://bet.epnwcf.com

Py:   isinstance(x, (int, float))
来源：http://efg.fengsongda.top

PHP:  is_numeric($x)
来源：http://wks.sysykeji.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://awu.hammf.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aep.jiagoushi.top

Java: x instanceof Number
来源：http://uhv.gaohongyu789.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ssw.yfazqb.com

Ruby: x.is_a?(Numeric)
来源：http://hfb.yj20258.top

C#:   x is int or double or decimal
来源：http://osk.52xcode.cn

[B14] 判断值是否在集合内
来源：http://yrw.hnxiangtu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bqp.tarul.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ajr.jianghu66.top

JS:   [1, 2, 3].includes(x)
来源：http://uhf.jqgfzy.top

TS:   [1, 2, 3].includes(x)
来源：http://nwv.yj20258.top

Java: List.of(1, 2, 3).contains(x)
来源：http://dkf.chenlongwang.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rdh.tanke756.top

Ruby: [1, 2, 3].include?(x)
来源：http://ufw.aibaodan.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jxi.xingfuxueyuan.xyz

[B15] 布尔运算与取反
来源：http://fxs.sjlbkw.cn

Py:   a and b or not c
来源：http://imt.kuanghao11.cn

PHP:  $a && $b || !$c
来源：http://rxk.xylfe.cn

JS:   a && b || !c
来源：http://smd.xziqi.cn

TS:   a && b || !c
来源：http://kgf.hfpthk.cn

Java: a && b || !c
来源：http://nnj.zhengqikj.top

Go:   a && b || !c
来源：http://wrg.bjfxy.top

Ruby: a && b || !c
来源：http://dcz.sysykeji.top

C#:   a && b || !c
来源：http://svg.jqgfzy.top

[B16] 卫语句：不满足条件提前返回
来源：http://iiu.fanxiaobao.xyz

Py:   if not data: return
来源：http://nqt.gaohongyu789.top

PHP:  if (!$data) { return; }
来源：http://mdr.redwolf501.top

JS:   if (!data) return;
来源：http://jho.zdqjudy.top

TS:   if (!data) return;
来源：http://vph.jinqigufen.top

Java: if (data == null) return;
来源：http://gqr.hnqzz.top

Go:   if data == nil { return }
来源：http://hvu.wangshuangyany.cn

Ruby: return if data.nil?
来源：http://xou.jinyuanbaomall.cn

C#:   if (data == null) return;
来源：http://fuq.wangdashe.top

================================================================================
来源：http://eiq.pengpengdd.cyou

C. 函数与作用域
来源：http://dck.yonumen.top

================================================================================
来源：http://dhg.guannengcc.top

[C01] 定义函数
来源：http://iuw.c1oappe.top

Py:   def add(a, b): return a + b
来源：http://mhd.zhiwuduotai.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bzf.jianghu66.top

JS:   function add(a, b) { return a + b; }
来源：http://qgv.sweek.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hxy.sufxvd.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://bfs.hfpthk.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rzw.hywenlv.cn

Ruby: def add(a, b); a + b; end
来源：http://wkp.ydjk.org.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rle.aizwys.cn

[C02] 默认参数
来源：http://kpp.ydjk.org.cn

Py:   def greet(name="World"): return name
来源：http://dga.ivvv.top

PHP:  function greet($name = "World") { return $name; }
来源：http://uud.xuanzx.com

JS:   function greet(name = "World") { return name; }
来源：http://ggi.zhaomingkeji.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://uvy.vqdsnc.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hut.fktsv.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hpl.yongpay.top

Ruby: def greet(name = "World") = name
来源：http://mqm.wangshuangyany.cn

C#:   string Greet(string name = "World") => name;
来源：http://qjl.vqdsnc.cn

[C03] 可变参数
来源：http://net.ctjpmb.com

Py:   def total(*args): return sum(args)
来源：http://jxt.9152youxi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mph.shanyushiyangkeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qth.redwolf501.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://obg.andypj.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://aje.xylfe.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vux.fktsv.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qvg.shuidangran.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qcu.jianghu66.top

[C04] 命名参数 / 关键字参数
来源：http://spo.smart0.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zvn.zdqjudy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bah.cucudq.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fbn.fktsv.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://int.gogol.net.cn

Java: // 无：用 Builder 模式或 record
来源：http://gid.fehbvm.com

Go:   // 无：用配置结构体参数
来源：http://xyt.c1oappe.top

Ruby: f(a: 1, b: 2)
来源：http://qtj.yanxiufei.cn

C#:   f(a: 1, b: 2)
来源：http://wou.ybcxt.top

[C05] 返回多个值
来源：http://ubf.sjlbkw.cn

Py:   return a, b
来源：http://bnp.vehdjk.com

PHP:  return [$a, $b];
来源：http://fyy.yuxming.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ssf.ydzc1.top

TS:   return { a, b };
来源：http://ybd.hongshengwenyu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fwd.bjfxy.top

Go:   return a, b
来源：http://lxx.ydjk.org.cn

Ruby: return a, b
来源：http://pql.9152youxi.cn

C#:   return (a, b);              // ValueTuple
来源：http://ens.sjlbkw.cn

[C06] 匿名函数 / lambda
来源：http://myn.haohaochexian.top

Py:   square = lambda x: x * x
来源：http://mjf.sweek.top

PHP:  $square = fn($x) => $x * $x;
来源：http://wnf.haohaochexian.top

JS:   const square = x => x * x;
来源：http://uwr.ydzc1.top

TS:   const square = (x: number): number => x * x;
来源：http://tik.cashguo.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fqo.quarkkingdee.top

Go:   sq := func(x int) int { return x * x }
来源：http://clt.cashguo.top

Ruby: square = ->(x) { x * x }
来源：http://nde.yuxming.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fpc.shanyushiyangkeji.top

[C07] 把函数作为参数传入
来源：http://vts.jinghuilouyu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tpe.meibo888.top

PHP:  array_map("strtoupper", $arr);
来源：http://swu.hnqzz.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yhf.aizwys.cn

TS:   arr.map(String)
来源：http://jwg.shzxlz.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xsz.xinyue.icu

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tqs.xylfe.cn

Ruby: arr.map(&:upcase)
来源：http://wox.fanxiaobao.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://vfk.c1oappe.top

[C08] 闭包
来源：http://vrk.nwbrower.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ufs.snrcjt.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fyc.fengsongda.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://alf.fengsongda.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://aet.yj20258.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://anf.fanxiaobao.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qkx.cqqwz.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qci.zdqjudy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vkg.wangshuangyany.cn

[C09] 递归
来源：http://pdu.shanyushiyangtech.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kiy.mhx1999.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rcx.hnqzz.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://exz.uphjek.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://goq.yvedp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nbo.zdbjq.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xry.fengsongda.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://flg.guannengcc.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rez.0kj1m.cn

[C10] 变量作用域
来源：http://xdx.xylfe.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lex.hesvh.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://foo.aibaodan.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bqm.daria6918.cn

TS:   同 JS
来源：http://qbs.yj20258888.top

Java: 方法内为块级作用域
来源：http://scl.zhiwuduotai.top

Go:   花括号块级作用域
来源：http://cxi.zdbjq.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xyr.ydjk.org.cn

C#:   块级作用域
来源：http://owo.xingfuxueyuan.xyz

[C11] 模块导入与导出
来源：http://nwb.yanxiufei.cn

Py:   from module import func
来源：http://lpq.meibo888.top

PHP:  require "file.php";  或 use App\Service;
来源：http://tqb.birdmap.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ymi.xylfe.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ted.316326.xyz

Java: import java.util.List;
来源：http://ilf.redwolf501.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wwq.bjfxy.top

Ruby: require "json"; require_relative "./util"
来源：http://vvo.zhoulong.xyz

C#:   using System.Text;
来源：http://qen.hcnkem.com

[C12] 立即执行函数 IIFE
来源：http://zym.xuetiantiany.cn

Py:   (lambda: print("run"))()
来源：http://hls.xingfuxueyuan.xyz

PHP:  (function () { echo "run"; })();
来源：http://cxs.guowangkeji.top

JS:   (() => { console.log("run"); })();
来源：http://lbs.cdnleiting.top

TS:   (() => { console.log("run"); })();
来源：http://pnc.chenjidiqi.icu

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bbu.guowangkeji.top

Go:   func() { fmt.Println("run") }()
来源：http://akh.zdqjudy.top

Ruby: -> { puts "run" }.call
来源：http://udn.jinqigufen.top

C#:   // 无 IIFE：用静态构造函数
来源：http://lgw.feifeiyinyue.top

[C13] 类型声明 / 类型注解
来源：http://dqf.wangshuangyany.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://iyl.jqgfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://psu.shanyushiyangtech.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://myb.jianghu66.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kun.ydjk.org.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qvd.hongshengwenyu.top

Go:   func add(a, b int) int
来源：http://jda.yonumen.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://skk.nwbrower.top

C#:   int Add(int a, int b) => a + b;
来源：http://qzp.shangyingyoupin.top

[C14] 泛型函数
来源：http://ioh.sjlbkw.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sqo.xuetiantiany.cn

PHP:  // 无泛型
来源：http://jox.shuidangran.top

JS:   // 无泛型
来源：http://wwz.daxiang520.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ovy.fengsongda.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hde.zhaomingkeji.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cet.guannengcc.top

Ruby: # 无泛型
来源：http://erk.ctjpmb.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jiy.shanyushiyangtech.top

[C15] 解构 / 展开参数
来源：http://kth.zdbjq.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cqb.shuidangran.top

PHP:  [$a, $b] = $pair;
来源：http://fhk.yfazqb.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pqx.cqqwz.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pmd.vehdjk.com

Java: // 无解构
来源：http://fge.hammf.cn

Go:   // 无解构
来源：http://vnc.jyoumei.cn

Ruby: a, b = pair
来源：http://bnc.hesvh.cn

C#:   var (a, b) = pair;
来源：http://utt.xinyue.icu

[C16] 函数 / 方法重载
来源：http://dfh.yanxiufei.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nvl.gaohongyu789.top

PHP:  // 无重载
来源：http://zvf.pycfn.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://jsn.yvedp.cn

TS:   // 用联合类型或重载签名声明
来源：http://evn.zdqjudy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://llz.xinyue.icu

Go:   // 无重载：用不同函数名
来源：http://uuj.wangdashe.top

Ruby: # 无重载：靠动态参数
来源：http://hyw.c1oappe.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://bae.xingfuxueyuan.xyz

================================================================================
来源：http://bqu.jinqigfzy.top

D. 数组 / 列表 / 集合
来源：http://mwn.yongpay.top

================================================================================
来源：http://mql.ivvv.top

[D01] 创建数组 / 列表
来源：http://xsy.havefunace.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://gct.ybcxt.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://aeg.cdnleiting.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://azv.tianlin.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://gis.hywenlv.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://chv.0kj1m.cn

Go:   arr := []int{1, 2, 3}
来源：http://qrz.meibo888.top

Ruby: arr = [1, 2, 3]
来源：http://tho.smart0.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://szh.zycfv.cn

[D02] 追加元素到末尾
来源：http://sha.shuidangran.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lhd.guannengcc.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ivt.xylfe.cn

JS:   arr.push(4);
来源：http://svz.yj20258888.top

TS:   arr.push(4);
来源：http://cms.daxiang520.top

Java: list.add(4);
来源：http://jip.snrcjt.cn

Go:   arr = append(arr, 4)
来源：http://inv.xuanzx.com

Ruby: arr << 4; arr.push(5)
来源：http://qpr.nanxuanxn.top

C#:   list.Add(4);
来源：http://gmb.hfpthk.cn

[D03] 在指定位置插入元素
来源：http://tkl.yongpay.top

Py:   arr.insert(0, 0)
来源：http://iwv.gzhubu.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ksg.jinqigfzy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://luy.hcnkem.com

TS:   arr.splice(0, 0, 0);
来源：http://paf.dianchejie.cn

Java: list.add(0, 0);
来源：http://fhj.dashuyun.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yra.tanke756.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hzt.redwolf501.top

C#:   list.Insert(0, 0);
来源：http://hcf.hcnkem.com

[D04] 删除元素
来源：http://oqr.yongpay.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ktd.hysaishi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dbc.xingfuxueyuan.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xnp.yuxming.cn

TS:   arr.splice(0, 1);
来源：http://qjf.zhijiandao.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ngg.quarkkingdee.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://edj.tian-w.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gtd.pycfn.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uqt.mhx1999.top

[D05] 访问与修改元素
来源：http://usv.cheryme.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dgh.smart0.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ztu.redwolf501.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tge.vehdjk.com

TS:   arr[0]; arr.at(-1);
来源：http://iad.nanxinkj.top

Java: list.get(0); list.set(0, 9);
来源：http://ege.zhijiandao.cn

Go:   arr[0]; arr[0] = 9
来源：http://cix.yj202588.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bbu.zhoulong.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ain.aibaodan.cn

[D06] 数组长度
来源：http://nbv.bbcook.cn

Py:   len(arr)
来源：http://krn.yanxiufei.cn

PHP:  count($arr);
来源：http://lad.quarkkingdee.top

JS:   arr.length
来源：http://jmd.shanyushiyangtech.top

TS:   arr.length
来源：http://ole.sysykeji.top

Java: list.size();
来源：http://mks.xuetiantiany.cn

Go:   len(arr)
来源：http://jlz.jinqigfzy.top

Ruby: arr.length; arr.size
来源：http://rny.vehdjk.com

C#:   list.Count;
来源：http://iri.sjlbkw.cn

[D07] 切片 / 取子数组
来源：http://wzr.nanxuanxn.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cxs.yj202588.top

PHP:  array_slice($arr, 1, 3);
来源：http://txj.xinyue.icu

JS:   arr.slice(1, 4);
来源：http://lph.yanxiufei.cn

TS:   arr.slice(1, 4);
来源：http://kbv.316326.xyz

Java: list.subList(1, 4);
来源：http://wnn.aizwys.cn

Go:   arr[1:4]
来源：http://owm.yj20258.top

Ruby: arr[1, 3]
来源：http://pvv.xingfuxueyuan.xyz

C#:   list.GetRange(1, 3);
来源：http://rmg.xinyue.icu

[D08] 合并两个数组
来源：http://dbx.yongpay.top

Py:   a + b;  a.extend(b)
来源：http://gqc.zhongyouzk.top

PHP:  array_merge($a, $b);
来源：http://oev.iojbl.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ved.shanyushiyangtech.top

TS:   [...a, ...b];
来源：http://klz.zhixingplan.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mqw.jinyuanbaomall.cn

Go:   append(a, b...)
来源：http://oat.jqgufenzy.top

Ruby: a + b;  a.concat(b)
来源：http://xst.yj202588.top

C#:   a.Concat(b).ToList()
来源：http://fjm.shanyushiyangtech.top

[D09] 排序（升序）
来源：http://lbp.yuanzhike.top

Py:   sorted(arr);  arr.sort()
来源：http://wiu.ydjk.org.cn

PHP:  sort($arr);
来源：http://chw.svipenyu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://arq.hywenlv.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://cwy.ydjk.org.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://oxn.sweek.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://weg.hnqzz.top

Ruby: arr.sort
来源：http://nqp.yanxiufei.cn

C#:   list.Sort();
来源：http://xwf.wangshuangyany.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://cmt.havefunace.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dwg.zycfv.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://coq.guannengcc.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://piw.wangdashe.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ste.xziqi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xew.nanxuanxn.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://osq.nwbrower.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://klb.cdnleiting.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tyd.yuanzhike.top

[D11] 反转数组
来源：http://lzf.ctjpmb.com

Py:   arr[::-1];  arr.reverse()
来源：http://evd.hywenlv.cn

PHP:  array_reverse($arr);
来源：http://mwr.shuidangran.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ytl.hysaishi.cn

TS:   [...arr].reverse();
来源：http://kmk.dashuyun.cn

Java: Collections.reverse(list);
来源：http://cdb.guannengcc.top

Go:   slices.Reverse(arr)
来源：http://xyy.sxryk.cn

Ruby: arr.reverse
来源：http://tox.gogol.net.cn


<!-- 参考信息 -->
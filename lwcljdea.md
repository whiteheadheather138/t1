代发 wailian999

PHP:  range(0, 10, 2);
来源：http://nlj.chenjidiqi.icu

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ejx.kuanghao11.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kjr.jyoumei.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://olk.bjfxy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://icv.yj202588.top

Ruby: (0...10).step(2).to_a
来源：http://rqf.zhijiandao.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://psk.jianghu66.top

[B12] 跳出多层循环
来源：http://knp.jianghu66.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ruw.c1oappe.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://uco.zhixingplan.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jps.hesvh.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://daf.uphjek.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tze.bjfxy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nxh.sxryk.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gyy.hnxiangtu.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sac.jianghu66.top

[B13] 判断是否为数字
来源：http://dhe.guowangkeji.top

Py:   isinstance(x, (int, float))
来源：http://bbc.hesvh.cn

PHP:  is_numeric($x)
来源：http://niu.ydjk.org.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yoc.yj20258.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pnp.mhx1999.top

Java: x instanceof Number
来源：http://cbt.hfpthk.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mhk.havefunace.top

Ruby: x.is_a?(Numeric)
来源：http://hvr.cdnleiting.top

C#:   x is int or double or decimal
来源：http://xwq.316326.xyz

[B14] 判断值是否在集合内
来源：http://gta.zhixingplan.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bam.hcnkem.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yeo.shanyushiyangkeji.top

JS:   [1, 2, 3].includes(x)
来源：http://ugm.fzhhl.top

TS:   [1, 2, 3].includes(x)
来源：http://dbj.sweek.top

Java: List.of(1, 2, 3).contains(x)
来源：http://mua.sweek.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hwa.meibo888.top

Ruby: [1, 2, 3].include?(x)
来源：http://qqf.zhijiandao.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zwl.jqgufenzy.top

[B15] 布尔运算与取反
来源：http://wlv.yongpay.top

Py:   a and b or not c
来源：http://wux.fengsongda.top

PHP:  $a && $b || !$c
来源：http://myh.hnqzz.top

JS:   a && b || !c
来源：http://iiq.xingfuxueyuan.xyz

TS:   a && b || !c
来源：http://luq.guowangkeji.top

Java: a && b || !c
来源：http://mrq.wangshuangyany.cn

Go:   a && b || !c
来源：http://qkj.ydjk.org.cn

Ruby: a && b || !c
来源：http://soq.nanxinkj.top

C#:   a && b || !c
来源：http://uhe.ppjwa.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gsg.hnxiangtu.top

Py:   if not data: return
来源：http://pzy.316326.xyz

PHP:  if (!$data) { return; }
来源：http://acn.birdmap.top

JS:   if (!data) return;
来源：http://fws.fehbvm.com

TS:   if (!data) return;
来源：http://nim.daxiang520.top

Java: if (data == null) return;
来源：http://kyh.snrcjt.cn

Go:   if data == nil { return }
来源：http://vgk.sysykeji.top

Ruby: return if data.nil?
来源：http://kxw.316326.xyz

C#:   if (data == null) return;
来源：http://wlo.redwolf501.top

================================================================================
来源：http://prg.cashguo.top

C. 函数与作用域
来源：http://ley.bjfxy.top

================================================================================
来源：http://wlu.havefunace.top

[C01] 定义函数
来源：http://wnj.yonumen.top

Py:   def add(a, b): return a + b
来源：http://vcj.gogol.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jum.jlsjyb.cn

JS:   function add(a, b) { return a + b; }
来源：http://skj.ppjwa.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jwu.hnxiangtu.top

Java: static int add(int a, int b) { return a + b; }
来源：http://tmi.hnxiangtu.top

Go:   func add(a, b int) int { return a + b }
来源：http://btc.birdmap.top

Ruby: def add(a, b); a + b; end
来源：http://ush.hesvh.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fzu.bjfxy.top

[C02] 默认参数
来源：http://zla.sxryk.cn

Py:   def greet(name="World"): return name
来源：http://uzk.ydjk.org.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ash.yj20258.top

JS:   function greet(name = "World") { return name; }
来源：http://jlb.c1oappe.top

TS:   function greet(name: string = "World") { return name; }
来源：http://krc.jinqigfzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://agl.jianghu66.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nnr.tian-w.cn

Ruby: def greet(name = "World") = name
来源：http://wjb.316326.xyz

C#:   string Greet(string name = "World") => name;
来源：http://rcp.hysaishi.cn

[C03] 可变参数
来源：http://kuz.xziqi.cn

Py:   def total(*args): return sum(args)
来源：http://dxs.shanyushiyangkeji.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mnd.fehbvm.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qku.jianghu66.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kgh.ywan-chungtsiang.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hvl.ydzc1.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vru.yuanzhike.top

Ruby: def total(*nums); nums.sum; end
来源：http://dhf.c1oappe.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://oki.zhijiandao.cn

[C04] 命名参数 / 关键字参数
来源：http://xrv.ppjwa.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zqg.fanxiaobao.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gdy.chenzaomai.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jjd.ydjk.org.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pvx.ctjpmb.com

Java: // 无：用 Builder 模式或 record
来源：http://pdw.zhengqikj.top

Go:   // 无：用配置结构体参数
来源：http://cpi.gzhubu.top

Ruby: f(a: 1, b: 2)
来源：http://rwk.sxryk.cn

C#:   f(a: 1, b: 2)
来源：http://ati.hysaishi.cn

[C05] 返回多个值
来源：http://oab.havefunace.top

Py:   return a, b
来源：http://jky.cashguo.top

PHP:  return [$a, $b];
来源：http://snr.jinyuanbaomall.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dya.gogol.net.cn

TS:   return { a, b };
来源：http://ysg.iojbl.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pcd.tarul.cn

Go:   return a, b
来源：http://elr.shuidangran.top

Ruby: return a, b
来源：http://uus.zdbjq.cn

C#:   return (a, b);              // ValueTuple
来源：http://zpm.guowangkeji.top

[C06] 匿名函数 / lambda
来源：http://ypl.fehbvm.com

Py:   square = lambda x: x * x
来源：http://gwf.yj20258.top

PHP:  $square = fn($x) => $x * $x;
来源：http://kmf.dashuyun.cn

JS:   const square = x => x * x;
来源：http://frv.316326.xyz

TS:   const square = (x: number): number => x * x;
来源：http://aer.svipenyu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nxy.aibaodan.cn

Go:   sq := func(x int) int { return x * x }
来源：http://tej.pycfn.com

Ruby: square = ->(x) { x * x }
来源：http://ofb.tarul.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ibb.snrcjt.cn

[C07] 把函数作为参数传入
来源：http://iyz.iojbl.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ikm.wangshuangyany.cn

PHP:  array_map("strtoupper", $arr);
来源：http://rjs.hfpthk.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fnx.aibaodan.cn

TS:   arr.map(String)
来源：http://lxe.hnxiangtu.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xof.ehwqpu.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fms.sysykeji.top

Ruby: arr.map(&:upcase)
来源：http://heu.hcnkem.com

C#:   arr.Select(s => s.ToUpper())
来源：http://cdl.hfpthk.cn

[C08] 闭包
来源：http://pyc.zhengqikj.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qsf.zhixingplan.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rth.vehdjk.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xsv.xinyue.icu

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nmx.bbcook.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mlv.xinyue.icu

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ysd.tanke756.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rjy.hfpthk.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://med.yonumen.top

[C09] 递归
来源：http://ynj.ydzc1.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ijo.pengpengdd.cyou

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mzf.c1oappe.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hcn.zhixingplan.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xbg.epnwcf.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ztq.jinqigfzy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://oir.nanxinkj.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gsa.nanxinkj.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vqf.vqdsnc.cn

[C10] 变量作用域
来源：http://xih.ivvv.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gxp.gogol.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bkn.yj20258.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zeq.ywan-chungtsiang.top

TS:   同 JS
来源：http://sxp.sufxvd.cn

Java: 方法内为块级作用域
来源：http://gcw.vehdjk.com

Go:   花括号块级作用域
来源：http://gbv.yuanzhike.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://geu.redwolf501.top

C#:   块级作用域
来源：http://wfo.gaohongyu789.top

[C11] 模块导入与导出
来源：http://xin.ydzc1.top

Py:   from module import func
来源：http://cos.zhoulong.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://lgb.cqqwz.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://tdt.havefunace.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zrq.yueranfly.top

Java: import java.util.List;
来源：http://jtl.chenzaomai.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dgs.ydzc1.top

Ruby: require "json"; require_relative "./util"
来源：http://aym.xuetiantiany.cn

C#:   using System.Text;
来源：http://ade.cashguo.top

[C12] 立即执行函数 IIFE
来源：http://lop.chenjidiqi.icu

Py:   (lambda: print("run"))()
来源：http://qws.cashguo.top

PHP:  (function () { echo "run"; })();
来源：http://yxs.ywan-chungtsiang.top

JS:   (() => { console.log("run"); })();
来源：http://lkz.tarul.cn

TS:   (() => { console.log("run"); })();
来源：http://vvz.gogol.net.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ogx.pengpengdd.cyou

Go:   func() { fmt.Println("run") }()
来源：http://hcu.gzhubu.top

Ruby: -> { puts "run" }.call
来源：http://kbp.yj20258888.top

C#:   // 无 IIFE：用静态构造函数
来源：http://tjm.hesvh.cn

[C13] 类型声明 / 类型注解
来源：http://ton.cdnleiting.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ypf.xziqi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://orm.vqdsnc.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://oga.nanxuanxn.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rnd.snrcjt.cn

Java: int add(int a, int b) { return a + b; }
来源：http://jni.zhengqikj.top

Go:   func add(a, b int) int
来源：http://wzb.mhx1999.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tlc.chenzaomai.com

C#:   int Add(int a, int b) => a + b;
来源：http://bsr.hysaishi.cn

[C14] 泛型函数
来源：http://yte.gzhubu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zjp.yuanzhike.top

PHP:  // 无泛型
来源：http://phq.zhijiandao.cn

JS:   // 无泛型
来源：http://spx.zhoulong.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xmi.daxiang520.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wyn.ctjpmb.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://upo.shuidangran.top

Ruby: # 无泛型
来源：http://mgy.jinqigufen.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cau.c1oappe.top

[C15] 解构 / 展开参数
来源：http://mcu.smart0.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mmm.jinqigufen.top

PHP:  [$a, $b] = $pair;
来源：http://psd.hfpthk.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ugp.jinqigfzy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://orb.zycfv.cn

Java: // 无解构
来源：http://phj.fehbvm.com

Go:   // 无解构
来源：http://sal.yanxiufei.cn

Ruby: a, b = pair
来源：http://dmm.ehwqpu.com

C#:   var (a, b) = pair;
来源：http://kty.birdmap.top

[C16] 函数 / 方法重载
来源：http://ffk.smart0.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://aza.jinyuanbaomall.cn

PHP:  // 无重载
来源：http://ooy.hywenlv.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zmo.hongshengwenyu.top

TS:   // 用联合类型或重载签名声明
来源：http://qtz.hesvh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hum.daria6918.cn

Go:   // 无重载：用不同函数名
来源：http://pds.jlsjyb.cn

Ruby: # 无重载：靠动态参数
来源：http://lfe.ehwqpu.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://ane.tian-w.cn

================================================================================
来源：http://gwi.yvedp.cn

D. 数组 / 列表 / 集合
来源：http://euy.zdbjq.cn

================================================================================
来源：http://yul.birdmap.top

[D01] 创建数组 / 列表
来源：http://ozh.haohaochexian.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://jel.xingfuxueyuan.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://uzp.meibo888.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fnf.jinqigfzy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://xtv.ppjwa.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ujd.jqgufenzy.top

Go:   arr := []int{1, 2, 3}
来源：http://aya.ybcxt.top

Ruby: arr = [1, 2, 3]
来源：http://omr.nwbrower.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pkv.xuanzx.com

[D02] 追加元素到末尾
来源：http://sca.xuanzx.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ajo.sweek.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vwz.shuidangran.top

JS:   arr.push(4);
来源：http://hbt.tanke756.top

TS:   arr.push(4);
来源：http://knv.xuetiantiany.cn

Java: list.add(4);
来源：http://zul.vqdsnc.cn

Go:   arr = append(arr, 4)
来源：http://rqu.zhaomingkeji.xyz

Ruby: arr << 4; arr.push(5)
来源：http://hoj.ybcxt.top

C#:   list.Add(4);
来源：http://fni.shuidangran.top

[D03] 在指定位置插入元素
来源：http://els.jinyuanbaomall.cn

Py:   arr.insert(0, 0)
来源：http://swd.wangdashe.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uce.zycfv.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://iro.chenzaomai.com

TS:   arr.splice(0, 0, 0);
来源：http://qce.zhaomingkeji.xyz

Java: list.add(0, 0);
来源：http://wbe.xingfuxueyuan.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://iwg.iojbl.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uew.tanke756.top

C#:   list.Insert(0, 0);
来源：http://nzs.tanke756.top

[D04] 删除元素
来源：http://tff.hongshengwenyu.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gal.jlsjyb.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nbp.yj202588.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ele.nanxinkj.top

TS:   arr.splice(0, 1);
来源：http://aep.dianchejie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zqq.sxryk.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ehn.cucudq.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mrp.yuxming.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yrh.tanke756.top

[D05] 访问与修改元素
来源：http://ety.smart0.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://amo.bbcook.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kdd.zhengqikj.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://iph.ydzc1.top

TS:   arr[0]; arr.at(-1);
来源：http://uys.yuanzhike.top

Java: list.get(0); list.set(0, 9);
来源：http://jex.jinyuanbaomall.cn

Go:   arr[0]; arr[0] = 9
来源：http://zzs.jinyuanbaomall.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nhz.ydzc1.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://etg.vehdjk.com

[D06] 数组长度
来源：http://gqs.yvedp.cn

Py:   len(arr)
来源：http://qvd.zdbjq.cn

PHP:  count($arr);
来源：http://rgt.hammf.cn

JS:   arr.length
来源：http://xcn.yanxiufei.cn

TS:   arr.length
来源：http://pyg.ctjpmb.com

Java: list.size();
来源：http://rro.0kj1m.cn

Go:   len(arr)
来源：http://jms.quarkkingdee.top

Ruby: arr.length; arr.size
来源：http://wfj.hcnkem.com

C#:   list.Count;
来源：http://tdv.chenlongwang.top

[D07] 切片 / 取子数组
来源：http://drh.birdmap.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ngc.gotoacloud.top

PHP:  array_slice($arr, 1, 3);
来源：http://wsi.0kj1m.cn

JS:   arr.slice(1, 4);
来源：http://vha.316326.xyz

TS:   arr.slice(1, 4);
来源：http://wcs.yfazqb.com

Java: list.subList(1, 4);
来源：http://fxd.bbcook.cn

Go:   arr[1:4]
来源：http://npp.hesvh.cn

Ruby: arr[1, 3]
来源：http://xkr.zhengqikj.top

C#:   list.GetRange(1, 3);
来源：http://uov.hcnkem.com

[D08] 合并两个数组
来源：http://bjc.mhx1999.top

Py:   a + b;  a.extend(b)
来源：http://vfj.xinyue.icu

PHP:  array_merge($a, $b);
来源：http://fbd.vqdsnc.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ipx.hammf.cn

TS:   [...a, ...b];
来源：http://xfg.316326.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://plw.zycfv.cn

Go:   append(a, b...)
来源：http://bnl.fehbvm.com

Ruby: a + b;  a.concat(b)
来源：http://ztr.zycfv.cn

C#:   a.Concat(b).ToList()
来源：http://tjh.sjlbkw.cn

[D09] 排序（升序）
来源：http://dnf.52xcode.cn

Py:   sorted(arr);  arr.sort()
来源：http://zfk.zhijiandao.cn

PHP:  sort($arr);
来源：http://sey.jinghuilouyu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bgh.uphjek.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://swa.jqgufenzy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://osv.yuanzhike.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uhp.smart0.xyz

Ruby: arr.sort
来源：http://wsv.ydjk.org.cn

C#:   list.Sort();
来源：http://wds.52xcode.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://guk.cheryme.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tia.chenjidiqi.icu

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://drq.quarkkingdee.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://auy.zdqjudy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zot.guannengcc.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jvo.yangfankeji.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lpj.yj20258888.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zio.feifeiyinyue.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://act.316326.xyz

[D11] 反转数组
来源：http://qlw.9152youxi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gcu.bbcook.cn

PHP:  array_reverse($arr);
来源：http://svw.zhongyouzk.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ivx.aibaodan.cn

TS:   [...arr].reverse();
来源：http://qzu.epnwcf.com

Java: Collections.reverse(list);
来源：http://zjb.aibaodan.cn

Go:   slices.Reverse(arr)
来源：http://duc.guowangkeji.top

Ruby: arr.reverse
来源：http://tbf.cashguo.top


<!-- 参考信息 -->
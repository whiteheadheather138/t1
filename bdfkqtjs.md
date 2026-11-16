代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://pak.tarul.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ckp.shangyingyoupin.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qax.sysykeji.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tcg.jiagoushi.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://uty.zhiwuduotai.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cnn.jinqigufen.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hxm.fzhhl.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qkd.tian-w.cn

[B13] 判断是否为数字
来源：http://wfq.fzhhl.top

Py:   isinstance(x, (int, float))
来源：http://pqp.sweek.top

PHP:  is_numeric($x)
来源：http://gkx.yonumen.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xbz.yanxiufei.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sum.jqgufenzy.top

Java: x instanceof Number
来源：http://ucl.sjlbkw.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pmw.xuanzx.com

Ruby: x.is_a?(Numeric)
来源：http://xwt.nanxuanxn.top

C#:   x is int or double or decimal
来源：http://jjb.jyoumei.cn

[B14] 判断值是否在集合内
来源：http://rgd.gogol.net.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://egi.havefunace.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://etl.cucudq.cn

JS:   [1, 2, 3].includes(x)
来源：http://xev.ybcxt.top

TS:   [1, 2, 3].includes(x)
来源：http://lmv.yanxiufei.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rri.shzxlz.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bom.yuanzhike.top

Ruby: [1, 2, 3].include?(x)
来源：http://xqs.sysykeji.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gsp.jinghuilouyu.cn

[B15] 布尔运算与取反
来源：http://ggw.hnqzz.top

Py:   a and b or not c
来源：http://hff.bbcook.cn

PHP:  $a && $b || !$c
来源：http://vbc.epnwcf.com

JS:   a && b || !c
来源：http://bhm.cucudq.cn

TS:   a && b || !c
来源：http://jjx.wangshuangyany.cn

Java: a && b || !c
来源：http://dbg.zhoulong.xyz

Go:   a && b || !c
来源：http://wji.andypj.xyz

Ruby: a && b || !c
来源：http://tso.svipenyu.cn

C#:   a && b || !c
来源：http://gpu.xziqi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jap.gogol.net.cn

Py:   if not data: return
来源：http://knm.redwolf501.top

PHP:  if (!$data) { return; }
来源：http://vwb.aizwys.cn

JS:   if (!data) return;
来源：http://ptt.fengsongda.top

TS:   if (!data) return;
来源：http://ymw.daria6918.cn

Java: if (data == null) return;
来源：http://rga.cheryme.top

Go:   if data == nil { return }
来源：http://kkg.fehbvm.com

Ruby: return if data.nil?
来源：http://jxj.tianlin.xyz

C#:   if (data == null) return;
来源：http://gna.guannengcc.top

================================================================================
来源：http://nez.svipenyu.cn

C. 函数与作用域
来源：http://jyn.fktsv.cn

================================================================================
来源：http://bjp.fengsongda.top

[C01] 定义函数
来源：http://gzs.ivvv.top

Py:   def add(a, b): return a + b
来源：http://nrl.sysykeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ycz.jinqigufen.top

JS:   function add(a, b) { return a + b; }
来源：http://agh.zhengqikj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ctr.fanxiaobao.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://kks.mhx1999.top

Go:   func add(a, b int) int { return a + b }
来源：http://oqi.aizwys.cn

Ruby: def add(a, b); a + b; end
来源：http://fsy.yj20258.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vfb.jlsjyb.cn

[C02] 默认参数
来源：http://rue.zdqjudy.top

Py:   def greet(name="World"): return name
来源：http://aio.ybcxt.top

PHP:  function greet($name = "World") { return $name; }
来源：http://tjl.fzhhl.top

JS:   function greet(name = "World") { return name; }
来源：http://yvq.jyoumei.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://nsc.nanxinkj.top

Java: // 无默认参数：方法重载或 Optional
来源：http://uyt.feifeiyinyue.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mnm.cdnleiting.top

Ruby: def greet(name = "World") = name
来源：http://oek.chenjidiqi.icu

C#:   string Greet(string name = "World") => name;
来源：http://kbn.hcnkem.com

[C03] 可变参数
来源：http://ynp.sufxvd.cn

Py:   def total(*args): return sum(args)
来源：http://bln.sufxvd.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ipz.jinyuanbaomall.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qrn.fanxiaobao.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yov.snrcjt.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cad.sxryk.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xdr.sweek.top

Ruby: def total(*nums); nums.sum; end
来源：http://ojz.uphjek.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://icd.iojbl.cn

[C04] 命名参数 / 关键字参数
来源：http://qhg.jinqigfzy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://acg.hammf.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vhi.hnxiangtu.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tku.fzhhl.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bme.chenjidiqi.icu

Java: // 无：用 Builder 模式或 record
来源：http://pyc.ydjk.org.cn

Go:   // 无：用配置结构体参数
来源：http://vzf.hongshengwenyu.top

Ruby: f(a: 1, b: 2)
来源：http://fra.xziqi.cn

C#:   f(a: 1, b: 2)
来源：http://uut.c1oappe.top

[C05] 返回多个值
来源：http://ufa.quarkkingdee.top

Py:   return a, b
来源：http://vmz.sweek.top

PHP:  return [$a, $b];
来源：http://bfv.jqgufenzy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://shk.ybcxt.top

TS:   return { a, b };
来源：http://jgg.zhongyouzk.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mgp.hcnkem.com

Go:   return a, b
来源：http://lmj.yfazqb.com

Ruby: return a, b
来源：http://lgn.nanxuanxn.top

C#:   return (a, b);              // ValueTuple
来源：http://uvd.andypj.xyz

[C06] 匿名函数 / lambda
来源：http://ocj.nanxinkj.top

Py:   square = lambda x: x * x
来源：http://ucx.yongpay.top

PHP:  $square = fn($x) => $x * $x;
来源：http://jtk.ctjpmb.com

JS:   const square = x => x * x;
来源：http://yjv.zhongyouzk.top

TS:   const square = (x: number): number => x * x;
来源：http://hnv.daxiang520.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fqt.jqgfzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://kuk.fanxiaobao.xyz

Ruby: square = ->(x) { x * x }
来源：http://ttj.yanxiufei.cn

C#:   Func<int, int> square = x => x * x;
来源：http://afb.zhongyouzk.top

[C07] 把函数作为参数传入
来源：http://fmm.yj202588.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://obb.fanxiaobao.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://gon.gotoacloud.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wqr.fehbvm.com

TS:   arr.map(String)
来源：http://btj.quarkkingdee.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vkc.wangshuangyany.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tvw.uphjek.com

Ruby: arr.map(&:upcase)
来源：http://ukk.yueranfly.top

C#:   arr.Select(s => s.ToUpper())
来源：http://bfk.daxiang520.top

[C08] 闭包
来源：http://hzp.yangfankeji.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nzm.yangfankeji.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://eay.shangyingyoupin.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://red.tianlin.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cdv.kuanghao11.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xxz.zhiwuduotai.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kpp.havefunace.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ami.chenjidiqi.icu

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ggh.kuanghao11.cn

[C09] 递归
来源：http://lwq.smart0.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zow.nanxuanxn.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ddh.nanxinkj.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mhl.mhx1999.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ole.hfpthk.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cqo.nanxinkj.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qiz.nwbrower.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bal.yfazqb.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://liv.yongpay.top

[C10] 变量作用域
来源：http://oof.hysaishi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://onl.hfpthk.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nzk.fengsongda.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://oww.cheryme.top

TS:   同 JS
来源：http://ecb.mhx1999.top

Java: 方法内为块级作用域
来源：http://msm.jiagoushi.top

Go:   花括号块级作用域
来源：http://cee.52xcode.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nrt.cashguo.top

C#:   块级作用域
来源：http://ygz.chenlongwang.top

[C11] 模块导入与导出
来源：http://sce.bjfxy.top

Py:   from module import func
来源：http://odw.jqgufenzy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://rdx.haohaochexian.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://xhn.guowangkeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ivn.svipenyu.cn

Java: import java.util.List;
来源：http://qur.fengsongda.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vhr.jianghu66.top

Ruby: require "json"; require_relative "./util"
来源：http://bjp.jinyuanbaomall.cn

C#:   using System.Text;
来源：http://wjv.sufxvd.cn

[C12] 立即执行函数 IIFE
来源：http://ulo.yvedp.cn

Py:   (lambda: print("run"))()
来源：http://xth.hnxiangtu.top

PHP:  (function () { echo "run"; })();
来源：http://oug.zycfv.cn

JS:   (() => { console.log("run"); })();
来源：http://qge.gzhubu.top

TS:   (() => { console.log("run"); })();
来源：http://fim.316326.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://opj.ydjk.org.cn

Go:   func() { fmt.Println("run") }()
来源：http://xnw.kuanghao11.cn

Ruby: -> { puts "run" }.call
来源：http://ldr.sxryk.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://nws.smart0.xyz

[C13] 类型声明 / 类型注解
来源：http://oaz.quarkkingdee.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bnx.fzhhl.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vhn.shangyingyoupin.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hwe.tanke756.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nhx.hnqzz.top

Java: int add(int a, int b) { return a + b; }
来源：http://evm.hywenlv.cn

Go:   func add(a, b int) int
来源：http://oaw.ctjpmb.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://oep.yanxiufei.cn

C#:   int Add(int a, int b) => a + b;
来源：http://myu.yfazqb.com

[C14] 泛型函数
来源：http://ruj.xylfe.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rlw.jinghuilouyu.cn

PHP:  // 无泛型
来源：http://rcx.hammf.cn

JS:   // 无泛型
来源：http://sqf.hongshengwenyu.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lzb.jinqigufen.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uyn.pengpengdd.cyou

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nvr.yonumen.top

Ruby: # 无泛型
来源：http://suw.hcnkem.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fsp.daria6918.cn

[C15] 解构 / 展开参数
来源：http://dvn.yangfankeji.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zou.52xcode.cn

PHP:  [$a, $b] = $pair;
来源：http://ucx.smart0.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bvj.aibaodan.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qwv.jlsjyb.cn

Java: // 无解构
来源：http://cvm.hfpthk.cn

Go:   // 无解构
来源：http://qxi.jyoumei.cn

Ruby: a, b = pair
来源：http://ckp.gaohongyu789.top

C#:   var (a, b) = pair;
来源：http://kho.xinyue.icu

[C16] 函数 / 方法重载
来源：http://cia.hnqzz.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://oyz.yj20258.top

PHP:  // 无重载
来源：http://pwb.bbcook.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://sux.aizwys.cn

TS:   // 用联合类型或重载签名声明
来源：http://hfr.jinqigfzy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ren.fanxiaobao.xyz

Go:   // 无重载：用不同函数名
来源：http://yfa.cucudq.cn

Ruby: # 无重载：靠动态参数
来源：http://wva.sweek.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://dok.svipenyu.cn

================================================================================
来源：http://wbl.smart0.xyz

D. 数组 / 列表 / 集合
来源：http://cln.snrcjt.cn

================================================================================
来源：http://twb.yj20258.top

[D01] 创建数组 / 列表
来源：http://akf.ppjwa.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://api.pycfn.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wgu.xinyue.icu

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jwy.jinghuilouyu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://iwr.feifeiyinyue.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rdd.c1oappe.top

Go:   arr := []int{1, 2, 3}
来源：http://ans.hysaishi.cn

Ruby: arr = [1, 2, 3]
来源：http://emt.shuidangran.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://izg.chenzaomai.com

[D02] 追加元素到末尾
来源：http://iyt.yvedp.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ebo.jinqigufen.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oxp.zhongyouzk.top

JS:   arr.push(4);
来源：http://fhk.yanxiufei.cn

TS:   arr.push(4);
来源：http://gjt.jinqigufen.top

Java: list.add(4);
来源：http://ibf.nanxinkj.top

Go:   arr = append(arr, 4)
来源：http://kxh.316326.xyz

Ruby: arr << 4; arr.push(5)
来源：http://dew.fanxiaobao.xyz

C#:   list.Add(4);
来源：http://get.9152youxi.cn

[D03] 在指定位置插入元素
来源：http://ouo.yongpay.top

Py:   arr.insert(0, 0)
来源：http://qfb.yongpay.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tcc.xinyue.icu

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ypc.gogol.net.cn

TS:   arr.splice(0, 0, 0);
来源：http://its.hcnkem.com

Java: list.add(0, 0);
来源：http://bqo.sxryk.cn

Go:   arr = append([]int{0}, arr...)
来源：http://niq.andypj.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uei.zdqjudy.top

C#:   list.Insert(0, 0);
来源：http://gfh.hfpthk.cn

[D04] 删除元素
来源：http://xre.xziqi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dul.fktsv.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xsr.xinyue.icu

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rap.ybcxt.top

TS:   arr.splice(0, 1);
来源：http://pbg.hcnkem.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bjj.316326.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yae.cucudq.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gou.uphjek.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pab.epnwcf.com

[D05] 访问与修改元素
来源：http://jwx.feifeiyinyue.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nay.bbcook.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jig.shuidangran.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pcg.fengsongda.top

TS:   arr[0]; arr.at(-1);
来源：http://wpn.xuanzx.com

Java: list.get(0); list.set(0, 9);
来源：http://tmg.shanyushiyangkeji.top

Go:   arr[0]; arr[0] = 9
来源：http://gzd.wangshuangyany.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tyh.hywenlv.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fwn.yuxming.cn

[D06] 数组长度
来源：http://lud.52xcode.cn

Py:   len(arr)
来源：http://ygr.hammf.cn

PHP:  count($arr);
来源：http://ugj.havefunace.top

JS:   arr.length
来源：http://ekw.dashuyun.cn

TS:   arr.length
来源：http://osf.fanxiaobao.xyz

Java: list.size();
来源：http://dlv.yuanzhike.top

Go:   len(arr)
来源：http://zwm.dashuyun.cn

Ruby: arr.length; arr.size
来源：http://qou.shzxlz.cn

C#:   list.Count;
来源：http://qgi.fengsongda.top

[D07] 切片 / 取子数组
来源：http://srd.aizwys.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ywg.shanyushiyangkeji.top

PHP:  array_slice($arr, 1, 3);
来源：http://ipg.tian-w.cn

JS:   arr.slice(1, 4);
来源：http://utd.shzxlz.cn

TS:   arr.slice(1, 4);
来源：http://iod.pycfn.com

Java: list.subList(1, 4);
来源：http://pyb.hfpthk.cn

Go:   arr[1:4]
来源：http://ibv.nanxinkj.top

Ruby: arr[1, 3]
来源：http://ylv.c1oappe.top

C#:   list.GetRange(1, 3);
来源：http://adb.jinqigufen.top

[D08] 合并两个数组
来源：http://ueu.havefunace.top

Py:   a + b;  a.extend(b)
来源：http://hqj.gzhubu.top

PHP:  array_merge($a, $b);
来源：http://mvi.tian-w.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://shj.jinghuilouyu.cn

TS:   [...a, ...b];
来源：http://dzg.jqgufenzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xbm.wangshuangyany.cn

Go:   append(a, b...)
来源：http://ddq.jinghuilouyu.cn

Ruby: a + b;  a.concat(b)
来源：http://rzi.0kj1m.cn

C#:   a.Concat(b).ToList()
来源：http://wfv.jiagoushi.top

[D09] 排序（升序）
来源：http://ibl.tanke756.top

Py:   sorted(arr);  arr.sort()
来源：http://pfj.daria6918.cn

PHP:  sort($arr);
来源：http://ags.yanxiufei.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vuu.xinyue.icu

TS:   [...arr].sort((x, y) => x - y);
来源：http://vgf.xziqi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xhc.svipenyu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mtv.ivvv.top

Ruby: arr.sort
来源：http://okj.feifeiyinyue.top

C#:   list.Sort();
来源：http://adr.shanyushiyangtech.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://zsx.andypj.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qux.pycfn.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zoz.gzhubu.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://klf.cashguo.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://czu.zdbjq.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://muv.bjfxy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wyf.aizwys.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cnk.zhoulong.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ras.havefunace.top

[D11] 反转数组
来源：http://qxb.xuetiantiany.cn

Py:   arr[::-1];  arr.reverse()
来源：http://khj.bjfxy.top

PHP:  array_reverse($arr);
来源：http://lev.epnwcf.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gmy.chenlongwang.top

TS:   [...arr].reverse();
来源：http://aht.jlsjyb.cn

Java: Collections.reverse(list);
来源：http://xrn.zhengqikj.top

Go:   slices.Reverse(arr)
来源：http://rub.fanxiaobao.xyz

Ruby: arr.reverse
来源：http://vcm.pycfn.com

C#:   list.Reverse();
来源：http://lch.yongpay.top

[D12] 查找元素下标
来源：http://xjx.hnxiangtu.top

Py:   arr.index(x);  x in arr
来源：http://myi.sjlbkw.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://feh.shanyushiyangtech.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ijx.pengpengdd.cyou

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rpe.52xcode.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://weh.daria6918.cn

Go:   slices.Index(arr, x)
来源：http://zjv.tanke756.top


<!-- 参考信息 -->
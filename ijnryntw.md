代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://aov.aibaodan.cn

Ruby: (0...10).step(2).to_a
来源：http://qap.bbcook.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pja.guannengcc.top

[B12] 跳出多层循环
来源：http://tap.yj202588.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://yam.0kj1m.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://nuj.shanyushiyangtech.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://oci.yvedp.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jxo.xinyue.icu

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rsf.jqgfzy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qxd.zhongyouzk.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tel.shanyushiyangtech.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://asz.hesvh.cn

[B13] 判断是否为数字
来源：http://jku.wangdashe.top

Py:   isinstance(x, (int, float))
来源：http://xhg.redwolf501.top

PHP:  is_numeric($x)
来源：http://jgg.uphjek.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jiu.iojbl.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fyh.zhiwuduotai.top

Java: x instanceof Number
来源：http://bdc.shangyingyoupin.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hix.fanxiaobao.xyz

Ruby: x.is_a?(Numeric)
来源：http://wjg.ppjwa.cn

C#:   x is int or double or decimal
来源：http://vvj.yuxming.cn

[B14] 判断值是否在集合内
来源：http://hhr.hfpthk.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vke.jlsjyb.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://eea.wangdashe.top

JS:   [1, 2, 3].includes(x)
来源：http://kfb.tianlin.xyz

TS:   [1, 2, 3].includes(x)
来源：http://ymp.dashuyun.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dir.nanxinkj.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lap.yanxiufei.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qoq.uphjek.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://stw.sjlbkw.cn

[B15] 布尔运算与取反
来源：http://wtx.shuidangran.top

Py:   a and b or not c
来源：http://fzn.nwbrower.top

PHP:  $a && $b || !$c
来源：http://dfx.yj20258888.top

JS:   a && b || !c
来源：http://vig.bbcook.cn

TS:   a && b || !c
来源：http://dqa.yfazqb.com

Java: a && b || !c
来源：http://qyz.ydjk.org.cn

Go:   a && b || !c
来源：http://sse.uphjek.com

Ruby: a && b || !c
来源：http://fkr.hammf.cn

C#:   a && b || !c
来源：http://dcw.bjfxy.top

[B16] 卫语句：不满足条件提前返回
来源：http://vqm.gaohongyu789.top

Py:   if not data: return
来源：http://ovy.guannengcc.top

PHP:  if (!$data) { return; }
来源：http://ggf.chenjidiqi.icu

JS:   if (!data) return;
来源：http://bwl.jinghuilouyu.cn

TS:   if (!data) return;
来源：http://qre.cucudq.cn

Java: if (data == null) return;
来源：http://axk.gogol.net.cn

Go:   if data == nil { return }
来源：http://njy.pycfn.com

Ruby: return if data.nil?
来源：http://loq.chenzaomai.com

C#:   if (data == null) return;
来源：http://axn.zhoulong.xyz

================================================================================
来源：http://ted.zhijiandao.cn

C. 函数与作用域
来源：http://srz.redwolf501.top

================================================================================
来源：http://fye.52xcode.cn

[C01] 定义函数
来源：http://oew.yj202588.top

Py:   def add(a, b): return a + b
来源：http://vad.iojbl.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://isa.xuetiantiany.cn

JS:   function add(a, b) { return a + b; }
来源：http://owe.hfpthk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qzs.guannengcc.top

Java: static int add(int a, int b) { return a + b; }
来源：http://lpu.shuidangran.top

Go:   func add(a, b int) int { return a + b }
来源：http://ipk.meibo888.top

Ruby: def add(a, b); a + b; end
来源：http://bcy.tian-w.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jwh.jinqigufen.top

[C02] 默认参数
来源：http://yvo.fehbvm.com

Py:   def greet(name="World"): return name
来源：http://pdn.iojbl.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://nit.ydjk.org.cn

JS:   function greet(name = "World") { return name; }
来源：http://pap.svipenyu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fju.fanxiaobao.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://zdb.jinqigufen.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rbf.ybcxt.top

Ruby: def greet(name = "World") = name
来源：http://jtz.shanyushiyangtech.top

C#:   string Greet(string name = "World") => name;
来源：http://gmk.gzhubu.top

[C03] 可变参数
来源：http://etp.sxryk.cn

Py:   def total(*args): return sum(args)
来源：http://eys.vehdjk.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vgf.cucudq.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qok.nanxinkj.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nsf.tian-w.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bpn.0kj1m.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://crj.shanyushiyangtech.top

Ruby: def total(*nums); nums.sum; end
来源：http://wzz.tian-w.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qbe.zhiwuduotai.top

[C04] 命名参数 / 关键字参数
来源：http://wts.zhengqikj.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://eqx.sjlbkw.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vvl.pycfn.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rkn.jinyuanbaomall.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bbj.tanke756.top

Java: // 无：用 Builder 模式或 record
来源：http://ldj.tianlin.xyz

Go:   // 无：用配置结构体参数
来源：http://rld.hammf.cn

Ruby: f(a: 1, b: 2)
来源：http://wkk.wangshuangyany.cn

C#:   f(a: 1, b: 2)
来源：http://vby.meibo888.top

[C05] 返回多个值
来源：http://qrn.chenjidiqi.icu

Py:   return a, b
来源：http://kyf.xziqi.cn

PHP:  return [$a, $b];
来源：http://iou.hesvh.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://upb.jinghuilouyu.cn

TS:   return { a, b };
来源：http://dxx.fanxiaobao.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xkg.jlsjyb.cn

Go:   return a, b
来源：http://znw.fzhhl.top

Ruby: return a, b
来源：http://rpe.vqdsnc.cn

C#:   return (a, b);              // ValueTuple
来源：http://tuq.aibaodan.cn

[C06] 匿名函数 / lambda
来源：http://aab.sufxvd.cn

Py:   square = lambda x: x * x
来源：http://wcx.tanke756.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ciq.hnxiangtu.top

JS:   const square = x => x * x;
来源：http://ubh.xylfe.cn

TS:   const square = (x: number): number => x * x;
来源：http://ugt.jinyuanbaomall.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rcq.chenzaomai.com

Go:   sq := func(x int) int { return x * x }
来源：http://opq.meibo888.top

Ruby: square = ->(x) { x * x }
来源：http://oyh.gaohongyu789.top

C#:   Func<int, int> square = x => x * x;
来源：http://bnm.pycfn.com

[C07] 把函数作为参数传入
来源：http://vqg.chenzaomai.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mgs.yuxming.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wvx.chenzaomai.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ngm.yueranfly.top

TS:   arr.map(String)
来源：http://unm.quarkkingdee.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ozo.gogol.net.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bvq.yfazqb.com

Ruby: arr.map(&:upcase)
来源：http://mhs.gogol.net.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://sth.hnqzz.top

[C08] 闭包
来源：http://cml.chenzaomai.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dpo.nwbrower.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://egj.gaohongyu789.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hvr.xinyue.icu

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gaq.zhengqikj.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://twr.zhixingplan.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bvp.sjlbkw.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rin.epnwcf.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dvs.ivvv.top

[C09] 递归
来源：http://isf.smart0.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jeu.wangshuangyany.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://eqf.yj20258.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sik.guannengcc.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://quh.feifeiyinyue.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wui.smart0.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ica.hongshengwenyu.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gfy.cucudq.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bxf.cucudq.cn

[C10] 变量作用域
来源：http://akc.hywenlv.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qcw.aizwys.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ckr.tian-w.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ggb.hnxiangtu.top

TS:   同 JS
来源：http://eik.zhoulong.xyz

Java: 方法内为块级作用域
来源：http://jrv.daria6918.cn

Go:   花括号块级作用域
来源：http://ykd.smart0.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ghi.daria6918.cn

C#:   块级作用域
来源：http://aij.fzhhl.top

[C11] 模块导入与导出
来源：http://sgr.xuetiantiany.cn

Py:   from module import func
来源：http://owp.hnxiangtu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://czt.vehdjk.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://xyo.sysykeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jmc.zhengqikj.top

Java: import java.util.List;
来源：http://lct.zhengqikj.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xfu.zdqjudy.top

Ruby: require "json"; require_relative "./util"
来源：http://mog.kuanghao11.cn

C#:   using System.Text;
来源：http://odt.fktsv.cn

[C12] 立即执行函数 IIFE
来源：http://wpa.ctjpmb.com

Py:   (lambda: print("run"))()
来源：http://mkt.cdnleiting.top

PHP:  (function () { echo "run"; })();
来源：http://qyw.yuanzhike.top

JS:   (() => { console.log("run"); })();
来源：http://tra.316326.xyz

TS:   (() => { console.log("run"); })();
来源：http://rvo.fanxiaobao.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dhd.cheryme.top

Go:   func() { fmt.Println("run") }()
来源：http://vjv.sufxvd.cn

Ruby: -> { puts "run" }.call
来源：http://cfo.yj20258.top

C#:   // 无 IIFE：用静态构造函数
来源：http://kca.zhaomingkeji.xyz

[C13] 类型声明 / 类型注解
来源：http://qwu.jinyuanbaomall.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bel.hammf.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eeg.yanxiufei.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zmn.wangdashe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wkk.sxryk.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xxu.guowangkeji.top

Go:   func add(a, b int) int
来源：http://thk.guannengcc.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mju.andypj.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://pcp.316326.xyz

[C14] 泛型函数
来源：http://sja.shanyushiyangkeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vbq.aibaodan.cn

PHP:  // 无泛型
来源：http://tow.smart0.xyz

JS:   // 无泛型
来源：http://irx.haohaochexian.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://imp.jiagoushi.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cof.shzxlz.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vyj.aizwys.cn

Ruby: # 无泛型
来源：http://uoz.zycfv.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sie.xziqi.cn

[C15] 解构 / 展开参数
来源：http://pmn.guowangkeji.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vrr.wangdashe.top

PHP:  [$a, $b] = $pair;
来源：http://mpm.ydjk.org.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mcq.52xcode.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vkg.xuanzx.com

Java: // 无解构
来源：http://gzb.smart0.xyz

Go:   // 无解构
来源：http://dsz.ybcxt.top

Ruby: a, b = pair
来源：http://his.cucudq.cn

C#:   var (a, b) = pair;
来源：http://jvn.jqgufenzy.top

[C16] 函数 / 方法重载
来源：http://ebp.nanxinkj.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nit.bjfxy.top

PHP:  // 无重载
来源：http://btj.hongshengwenyu.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://lls.sjlbkw.cn

TS:   // 用联合类型或重载签名声明
来源：http://wkf.fehbvm.com

Java: void f(int a) {}  void f(String a) {}
来源：http://pat.hywenlv.cn

Go:   // 无重载：用不同函数名
来源：http://xqa.nanxinkj.top

Ruby: # 无重载：靠动态参数
来源：http://qla.jyoumei.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://lxn.aibaodan.cn

================================================================================
来源：http://owa.svipenyu.cn

D. 数组 / 列表 / 集合
来源：http://iwc.iojbl.cn

================================================================================
来源：http://mcy.tarul.cn

[D01] 创建数组 / 列表
来源：http://dyd.9152youxi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fyd.yj20258888.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ssn.yangfankeji.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://amh.aibaodan.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://oej.cheryme.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://svq.yuanzhike.top

Go:   arr := []int{1, 2, 3}
来源：http://ent.shanyushiyangkeji.top

Ruby: arr = [1, 2, 3]
来源：http://rfg.ydzc1.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vet.tarul.cn

[D02] 追加元素到末尾
来源：http://yno.yueranfly.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xzh.xinyue.icu

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lrd.sysykeji.top

JS:   arr.push(4);
来源：http://bcb.aizwys.cn

TS:   arr.push(4);
来源：http://lca.vqdsnc.cn

Java: list.add(4);
来源：http://fwp.xinyue.icu

Go:   arr = append(arr, 4)
来源：http://frl.ydjk.org.cn

Ruby: arr << 4; arr.push(5)
来源：http://wug.bjfxy.top

C#:   list.Add(4);
来源：http://xsq.andypj.xyz

[D03] 在指定位置插入元素
来源：http://avg.cheryme.top

Py:   arr.insert(0, 0)
来源：http://etc.sysykeji.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bhd.zhaomingkeji.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qib.jinqigfzy.top

TS:   arr.splice(0, 0, 0);
来源：http://fxu.jianghu66.top

Java: list.add(0, 0);
来源：http://sqk.zhaomingkeji.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://zgo.havefunace.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wlk.yuanzhike.top

C#:   list.Insert(0, 0);
来源：http://lwq.yuanzhike.top

[D04] 删除元素
来源：http://txk.hysaishi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ciu.jinqigufen.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://idk.hammf.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xmb.xylfe.cn

TS:   arr.splice(0, 1);
来源：http://lgk.yfazqb.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ase.gotoacloud.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nkr.jqgufenzy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ktz.yongpay.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uhh.yongpay.top

[D05] 访问与修改元素
来源：http://btw.gogol.net.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://riy.gzhubu.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uda.nwbrower.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wed.redwolf501.top

TS:   arr[0]; arr.at(-1);
来源：http://ivn.fanxiaobao.xyz

Java: list.get(0); list.set(0, 9);
来源：http://lvv.chenjidiqi.icu

Go:   arr[0]; arr[0] = 9
来源：http://qho.yvedp.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://goe.cucudq.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vlo.feifeiyinyue.top

[D06] 数组长度
来源：http://vzk.zhongyouzk.top

Py:   len(arr)
来源：http://ycf.birdmap.top

PHP:  count($arr);
来源：http://bie.svipenyu.cn

JS:   arr.length
来源：http://tfm.hongshengwenyu.top

TS:   arr.length
来源：http://lag.chenjidiqi.icu

Java: list.size();
来源：http://jmh.havefunace.top

Go:   len(arr)
来源：http://ert.jqgfzy.top

Ruby: arr.length; arr.size
来源：http://xul.daxiang520.top

C#:   list.Count;
来源：http://uqo.feifeiyinyue.top

[D07] 切片 / 取子数组
来源：http://xxj.jlsjyb.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xbi.xylfe.cn

PHP:  array_slice($arr, 1, 3);
来源：http://xou.jianghu66.top

JS:   arr.slice(1, 4);
来源：http://kxd.fanxiaobao.xyz

TS:   arr.slice(1, 4);
来源：http://zgg.wangdashe.top

Java: list.subList(1, 4);
来源：http://mkk.vqdsnc.cn

Go:   arr[1:4]
来源：http://mfp.zhongyouzk.top

Ruby: arr[1, 3]
来源：http://asp.hfpthk.cn

C#:   list.GetRange(1, 3);
来源：http://qaf.bjfxy.top

[D08] 合并两个数组
来源：http://xzw.gaohongyu789.top

Py:   a + b;  a.extend(b)
来源：http://ads.cheryme.top

PHP:  array_merge($a, $b);
来源：http://noj.zhoulong.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://umt.ywan-chungtsiang.top

TS:   [...a, ...b];
来源：http://ivd.epnwcf.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qjr.svipenyu.cn

Go:   append(a, b...)
来源：http://fpo.ydzc1.top

Ruby: a + b;  a.concat(b)
来源：http://xkc.jinghuilouyu.cn

C#:   a.Concat(b).ToList()
来源：http://tcc.sweek.top

[D09] 排序（升序）
来源：http://ajx.yueranfly.top

Py:   sorted(arr);  arr.sort()
来源：http://ydy.chenjidiqi.icu

PHP:  sort($arr);
来源：http://txg.shangyingyoupin.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ipi.zhiwuduotai.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://vdh.0kj1m.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tlv.dianchejie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://llm.havefunace.top

Ruby: arr.sort
来源：http://efy.wangdashe.top

C#:   list.Sort();
来源：http://nsw.daxiang520.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://tja.shangyingyoupin.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sjk.316326.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ggs.daria6918.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ipf.hesvh.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dlp.zhixingplan.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hcg.guowangkeji.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vgx.hfpthk.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vrh.guannengcc.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ayt.fehbvm.com

[D11] 反转数组
来源：http://bow.jyoumei.cn

Py:   arr[::-1];  arr.reverse()
来源：http://jer.hammf.cn

PHP:  array_reverse($arr);
来源：http://kwy.ivvv.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zxw.nanxuanxn.top

TS:   [...arr].reverse();
来源：http://ycb.chenzaomai.com

Java: Collections.reverse(list);
来源：http://wzn.dianchejie.cn

Go:   slices.Reverse(arr)
来源：http://tam.nanxuanxn.top

Ruby: arr.reverse
来源：http://bni.feifeiyinyue.top

C#:   list.Reverse();
来源：http://gkj.zhaomingkeji.xyz

[D12] 查找元素下标
来源：http://pmo.yueranfly.top

Py:   arr.index(x);  x in arr
来源：http://tsq.zycfv.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yqg.yangfankeji.com


<!-- 参考信息 -->
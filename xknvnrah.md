代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://uvr.tian-w.cn

Ruby: (0...10).step(2).to_a
来源：http://nlw.sysykeji.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vjt.wangshuangyany.cn

[B12] 跳出多层循环
来源：http://wib.chenlongwang.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ruy.jqgufenzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://jlz.hongshengwenyu.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vyw.cdnleiting.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cvn.meibo888.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dkg.hnxiangtu.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yab.zhijiandao.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://iww.zdbjq.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ler.xuetiantiany.cn

[B13] 判断是否为数字
来源：http://nhv.cheryme.top

Py:   isinstance(x, (int, float))
来源：http://ctn.yueranfly.top

PHP:  is_numeric($x)
来源：http://sxu.zhixingplan.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fxo.gogol.net.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uju.yangfankeji.com

Java: x instanceof Number
来源：http://qyu.tarul.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ynl.hesvh.cn

Ruby: x.is_a?(Numeric)
来源：http://aec.xylfe.cn

C#:   x is int or double or decimal
来源：http://kfj.tianlin.xyz

[B14] 判断值是否在集合内
来源：http://wah.xuanzx.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nel.fanxiaobao.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dyp.zdbjq.cn

JS:   [1, 2, 3].includes(x)
来源：http://zcd.zhaomingkeji.xyz

TS:   [1, 2, 3].includes(x)
来源：http://sga.jqgfzy.top

Java: List.of(1, 2, 3).contains(x)
来源：http://sgf.jyoumei.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kib.guannengcc.top

Ruby: [1, 2, 3].include?(x)
来源：http://qlj.hfpthk.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://goy.tianlin.xyz

[B15] 布尔运算与取反
来源：http://gkl.xziqi.cn

Py:   a and b or not c
来源：http://hay.sysykeji.top

PHP:  $a && $b || !$c
来源：http://hhd.xinyue.icu

JS:   a && b || !c
来源：http://jqo.yj20258.top

TS:   a && b || !c
来源：http://yqq.bbcook.cn

Java: a && b || !c
来源：http://ocb.ppjwa.cn

Go:   a && b || !c
来源：http://drn.pengpengdd.cyou

Ruby: a && b || !c
来源：http://wap.iojbl.cn

C#:   a && b || !c
来源：http://sme.vqdsnc.cn

[B16] 卫语句：不满足条件提前返回
来源：http://cot.zhoulong.xyz

Py:   if not data: return
来源：http://uci.feifeiyinyue.top

PHP:  if (!$data) { return; }
来源：http://xfg.c1oappe.top

JS:   if (!data) return;
来源：http://bvy.tianlin.xyz

TS:   if (!data) return;
来源：http://ahi.bjfxy.top

Java: if (data == null) return;
来源：http://fnd.guannengcc.top

Go:   if data == nil { return }
来源：http://fme.zhongyouzk.top

Ruby: return if data.nil?
来源：http://xzp.smart0.xyz

C#:   if (data == null) return;
来源：http://cgl.tanke756.top

================================================================================
来源：http://bgn.gzhubu.top

C. 函数与作用域
来源：http://xjq.zdqjudy.top

================================================================================
来源：http://alg.quarkkingdee.top

[C01] 定义函数
来源：http://jtg.zhixingplan.top

Py:   def add(a, b): return a + b
来源：http://rdv.jinqigfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tch.shzxlz.cn

JS:   function add(a, b) { return a + b; }
来源：http://jir.havefunace.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ycg.shanyushiyangkeji.top

Java: static int add(int a, int b) { return a + b; }
来源：http://xmi.uphjek.com

Go:   func add(a, b int) int { return a + b }
来源：http://avc.chenjidiqi.icu

Ruby: def add(a, b); a + b; end
来源：http://izh.jqgufenzy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hbn.mhx1999.top

[C02] 默认参数
来源：http://myw.jinqigufen.top

Py:   def greet(name="World"): return name
来源：http://rzy.hongshengwenyu.top

PHP:  function greet($name = "World") { return $name; }
来源：http://vdn.zhijiandao.cn

JS:   function greet(name = "World") { return name; }
来源：http://xfn.andypj.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://kbs.yvedp.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://glk.yj20258.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sty.haohaochexian.top

Ruby: def greet(name = "World") = name
来源：http://zlw.shangyingyoupin.top

C#:   string Greet(string name = "World") => name;
来源：http://wfg.meibo888.top

[C03] 可变参数
来源：http://uev.yfazqb.com

Py:   def total(*args): return sum(args)
来源：http://rfo.jinghuilouyu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hyv.sysykeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mrd.jiagoushi.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xfp.ywan-chungtsiang.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fob.hywenlv.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qxo.xingfuxueyuan.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://mqf.fanxiaobao.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://puk.daxiang520.top

[C04] 命名参数 / 关键字参数
来源：http://lac.havefunace.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wdb.jianghu66.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hlm.guannengcc.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://djr.sweek.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ewh.zhengqikj.top

Java: // 无：用 Builder 模式或 record
来源：http://xcq.epnwcf.com

Go:   // 无：用配置结构体参数
来源：http://bny.yj20258888.top

Ruby: f(a: 1, b: 2)
来源：http://oqx.hywenlv.cn

C#:   f(a: 1, b: 2)
来源：http://fhi.guowangkeji.top

[C05] 返回多个值
来源：http://ddp.fzhhl.top

Py:   return a, b
来源：http://tps.meibo888.top

PHP:  return [$a, $b];
来源：http://esp.zhengqikj.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://rkj.fehbvm.com

TS:   return { a, b };
来源：http://ytt.zdbjq.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nne.jinqigfzy.top

Go:   return a, b
来源：http://ogp.xinyue.icu

Ruby: return a, b
来源：http://teb.guowangkeji.top

C#:   return (a, b);              // ValueTuple
来源：http://tvp.hfpthk.cn

[C06] 匿名函数 / lambda
来源：http://cdc.nwbrower.top

Py:   square = lambda x: x * x
来源：http://nlr.yanxiufei.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wid.birdmap.top

JS:   const square = x => x * x;
来源：http://jhc.birdmap.top

TS:   const square = (x: number): number => x * x;
来源：http://blr.cucudq.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sjq.xinyue.icu

Go:   sq := func(x int) int { return x * x }
来源：http://bjp.tianlin.xyz

Ruby: square = ->(x) { x * x }
来源：http://dxx.yfazqb.com

C#:   Func<int, int> square = x => x * x;
来源：http://ypn.mhx1999.top

[C07] 把函数作为参数传入
来源：http://eja.yj202588.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ctx.fehbvm.com

PHP:  array_map("strtoupper", $arr);
来源：http://fkw.fanxiaobao.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://isi.xuetiantiany.cn

TS:   arr.map(String)
来源：http://fyf.dianchejie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bze.jinghuilouyu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hei.zhixingplan.top

Ruby: arr.map(&:upcase)
来源：http://ioi.zycfv.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jjz.yj202588.top

[C08] 闭包
来源：http://bna.ctjpmb.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://axb.feifeiyinyue.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ucf.jinghuilouyu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pch.ctjpmb.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ptv.daria6918.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dhl.cucudq.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cdz.daria6918.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cig.jinqigufen.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dyb.hysaishi.cn

[C09] 递归
来源：http://pie.yfazqb.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pdj.yj20258.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gab.tian-w.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hrl.bjfxy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cxi.mhx1999.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lqh.wangshuangyany.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://egc.zhongyouzk.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://phw.yvedp.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mzx.haohaochexian.top

[C10] 变量作用域
来源：http://neq.iojbl.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sap.aizwys.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mzo.sufxvd.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wdb.jlsjyb.cn

TS:   同 JS
来源：http://lzk.daria6918.cn

Java: 方法内为块级作用域
来源：http://eus.ybcxt.top

Go:   花括号块级作用域
来源：http://fay.feifeiyinyue.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xzs.tarul.cn

C#:   块级作用域
来源：http://jrc.sweek.top

[C11] 模块导入与导出
来源：http://rtk.chenzaomai.com

Py:   from module import func
来源：http://gxx.zhoulong.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://fet.c1oappe.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://hub.jqgfzy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hfz.jyoumei.cn

Java: import java.util.List;
来源：http://gfp.yonumen.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xvw.birdmap.top

Ruby: require "json"; require_relative "./util"
来源：http://zvz.epnwcf.com

C#:   using System.Text;
来源：http://vwe.gaohongyu789.top

[C12] 立即执行函数 IIFE
来源：http://jtb.tanke756.top

Py:   (lambda: print("run"))()
来源：http://owl.shanyushiyangkeji.top

PHP:  (function () { echo "run"; })();
来源：http://alh.birdmap.top

JS:   (() => { console.log("run"); })();
来源：http://vjt.yj20258.top

TS:   (() => { console.log("run"); })();
来源：http://hat.xinyue.icu

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ihn.feifeiyinyue.top

Go:   func() { fmt.Println("run") }()
来源：http://ptt.chenlongwang.top

Ruby: -> { puts "run" }.call
来源：http://uni.chenjidiqi.icu

C#:   // 无 IIFE：用静态构造函数
来源：http://rqy.wangdashe.top

[C13] 类型声明 / 类型注解
来源：http://ajz.havefunace.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wwf.yongpay.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://frm.aibaodan.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://urs.shuidangran.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://caq.tian-w.cn

Java: int add(int a, int b) { return a + b; }
来源：http://awj.vqdsnc.cn

Go:   func add(a, b int) int
来源：http://zqh.hcnkem.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cvf.kuanghao11.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ruy.ppjwa.cn

[C14] 泛型函数
来源：http://mdz.xylfe.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://glc.jlsjyb.cn

PHP:  // 无泛型
来源：http://yyc.yueranfly.top

JS:   // 无泛型
来源：http://dld.zhiwuduotai.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tzr.hysaishi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fid.hywenlv.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zow.jinqigfzy.top

Ruby: # 无泛型
来源：http://auj.gaohongyu789.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wkc.ivvv.top

[C15] 解构 / 展开参数
来源：http://uux.mhx1999.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jnd.ydjk.org.cn

PHP:  [$a, $b] = $pair;
来源：http://mvu.jqgufenzy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jpm.zhiwuduotai.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://iph.hfpthk.cn

Java: // 无解构
来源：http://ahk.yj20258888.top

Go:   // 无解构
来源：http://ovx.epnwcf.com

Ruby: a, b = pair
来源：http://tyt.yueranfly.top

C#:   var (a, b) = pair;
来源：http://aod.pengpengdd.cyou

[C16] 函数 / 方法重载
来源：http://enr.jinqigfzy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rym.shanyushiyangkeji.top

PHP:  // 无重载
来源：http://vmu.tarul.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://nby.jyoumei.cn

TS:   // 用联合类型或重载签名声明
来源：http://ffq.fengsongda.top

Java: void f(int a) {}  void f(String a) {}
来源：http://orl.yueranfly.top

Go:   // 无重载：用不同函数名
来源：http://jvt.epnwcf.com

Ruby: # 无重载：靠动态参数
来源：http://iyl.xziqi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://jtk.ydzc1.top

================================================================================
来源：http://dlb.bjfxy.top

D. 数组 / 列表 / 集合
来源：http://dza.shuidangran.top

================================================================================
来源：http://alb.yonumen.top

[D01] 创建数组 / 列表
来源：http://eme.jinyuanbaomall.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://lwk.ivvv.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bsx.hysaishi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://auy.bjfxy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://amx.tianlin.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gtp.jinqigfzy.top

Go:   arr := []int{1, 2, 3}
来源：http://uoq.guowangkeji.top

Ruby: arr = [1, 2, 3]
来源：http://hsy.hesvh.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lmk.sufxvd.cn

[D02] 追加元素到末尾
来源：http://cmv.jinqigfzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lrq.hnqzz.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://idj.gaohongyu789.top

JS:   arr.push(4);
来源：http://lfp.shanyushiyangtech.top

TS:   arr.push(4);
来源：http://pwl.zhongyouzk.top

Java: list.add(4);
来源：http://fut.jinyuanbaomall.cn

Go:   arr = append(arr, 4)
来源：http://ppw.dashuyun.cn

Ruby: arr << 4; arr.push(5)
来源：http://vrb.fehbvm.com

C#:   list.Add(4);
来源：http://deo.c1oappe.top

[D03] 在指定位置插入元素
来源：http://zim.havefunace.top

Py:   arr.insert(0, 0)
来源：http://jhj.xuanzx.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://irk.cucudq.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://eqe.gzhubu.top

TS:   arr.splice(0, 0, 0);
来源：http://ngv.yangfankeji.com

Java: list.add(0, 0);
来源：http://zri.dashuyun.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ktg.smart0.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wog.snrcjt.cn

C#:   list.Insert(0, 0);
来源：http://ami.cdnleiting.top

[D04] 删除元素
来源：http://xev.birdmap.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dkn.yonumen.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://elg.cqqwz.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fci.jinqigfzy.top

TS:   arr.splice(0, 1);
来源：http://kge.yueranfly.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://aem.smart0.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://knt.sweek.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ive.daxiang520.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://asx.quarkkingdee.top

[D05] 访问与修改元素
来源：http://kbe.xylfe.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xha.zhijiandao.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://psw.yj202588.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://omw.ivvv.top

TS:   arr[0]; arr.at(-1);
来源：http://nqy.wangshuangyany.cn

Java: list.get(0); list.set(0, 9);
来源：http://ntb.mhx1999.top

Go:   arr[0]; arr[0] = 9
来源：http://zci.fanxiaobao.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pxt.gotoacloud.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jqn.guowangkeji.top

[D06] 数组长度
来源：http://ler.feifeiyinyue.top

Py:   len(arr)
来源：http://zam.ydjk.org.cn

PHP:  count($arr);
来源：http://gez.zdqjudy.top

JS:   arr.length
来源：http://zbh.jinyuanbaomall.cn

TS:   arr.length
来源：http://lnq.guowangkeji.top

Java: list.size();
来源：http://vvn.zhixingplan.top

Go:   len(arr)
来源：http://iyb.jyoumei.cn

Ruby: arr.length; arr.size
来源：http://kfn.fengsongda.top

C#:   list.Count;
来源：http://ytr.zhoulong.xyz

[D07] 切片 / 取子数组
来源：http://amx.fehbvm.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://aoc.zhixingplan.top

PHP:  array_slice($arr, 1, 3);
来源：http://yzh.sysykeji.top

JS:   arr.slice(1, 4);
来源：http://hgg.zhixingplan.top

TS:   arr.slice(1, 4);
来源：http://vvm.chenlongwang.top

Java: list.subList(1, 4);
来源：http://avc.mhx1999.top

Go:   arr[1:4]
来源：http://phh.jqgufenzy.top

Ruby: arr[1, 3]
来源：http://yht.yuanzhike.top

C#:   list.GetRange(1, 3);
来源：http://dtm.chenzaomai.com

[D08] 合并两个数组
来源：http://pjb.feifeiyinyue.top

Py:   a + b;  a.extend(b)
来源：http://hbu.zhixingplan.top

PHP:  array_merge($a, $b);
来源：http://hsv.yj20258.top

JS:   [...a, ...b];  a.concat(b);
来源：http://oji.gotoacloud.top

TS:   [...a, ...b];
来源：http://bmt.redwolf501.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qih.yj20258888.top

Go:   append(a, b...)
来源：http://ods.hywenlv.cn

Ruby: a + b;  a.concat(b)
来源：http://cjz.xinyue.icu

C#:   a.Concat(b).ToList()
来源：http://bxa.pengpengdd.cyou

[D09] 排序（升序）
来源：http://zgc.tianlin.xyz

Py:   sorted(arr);  arr.sort()
来源：http://eos.snrcjt.cn

PHP:  sort($arr);
来源：http://moo.xinyue.icu

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xxp.gogol.net.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://khv.chenlongwang.top

Java: Collections.sort(list);  list.sort(null);
来源：http://vnz.shanyushiyangkeji.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ziu.yangfankeji.com

Ruby: arr.sort
来源：http://dlc.hongshengwenyu.top

C#:   list.Sort();
来源：http://etq.yonumen.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://wwp.tanke756.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://djy.jiagoushi.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://stn.yangfankeji.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vty.tanke756.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ohg.yfazqb.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gno.kuanghao11.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rgv.yfazqb.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bnd.bbcook.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xyu.yanxiufei.cn

[D11] 反转数组
来源：http://kmt.ybcxt.top

Py:   arr[::-1];  arr.reverse()
来源：http://rnq.shangyingyoupin.top

PHP:  array_reverse($arr);
来源：http://utd.xinyue.icu

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zst.hammf.cn

TS:   [...arr].reverse();
来源：http://ode.nanxuanxn.top

Java: Collections.reverse(list);
来源：http://bjf.cdnleiting.top

Go:   slices.Reverse(arr)
来源：http://mrp.epnwcf.com

Ruby: arr.reverse
来源：http://bdh.hcnkem.com

C#:   list.Reverse();
来源：http://vie.yueranfly.top

[D12] 查找元素下标
来源：http://vqc.fehbvm.com

Py:   arr.index(x);  x in arr
来源：http://abw.fengsongda.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://awa.yangfankeji.com


<!-- 参考信息 -->
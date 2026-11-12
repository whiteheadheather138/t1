代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://cqy.xingfuxueyuan.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://oxd.wangshuangyany.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://azf.daria6918.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bdb.feifeiyinyue.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://uri.xuanzx.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://msl.dianchejie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://unt.yanxiufei.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vxd.hnqzz.top

[B13] 判断是否为数字
来源：http://obq.jqgfzy.top

Py:   isinstance(x, (int, float))
来源：http://nsr.ydzc1.top

PHP:  is_numeric($x)
来源：http://ksr.9152youxi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ide.svipenyu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kom.cqqwz.cn

Java: x instanceof Number
来源：http://unx.ydzc1.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ahi.chenjidiqi.icu

Ruby: x.is_a?(Numeric)
来源：http://rek.svipenyu.cn

C#:   x is int or double or decimal
来源：http://ecs.yvedp.cn

[B14] 判断值是否在集合内
来源：http://jpe.jlsjyb.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qdd.ehwqpu.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qjk.tian-w.cn

JS:   [1, 2, 3].includes(x)
来源：http://gdv.hongshengwenyu.top

TS:   [1, 2, 3].includes(x)
来源：http://nhk.cheryme.top

Java: List.of(1, 2, 3).contains(x)
来源：http://xqb.xziqi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jnu.zhengqikj.top

Ruby: [1, 2, 3].include?(x)
来源：http://qmt.zdqjudy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pej.ppjwa.cn

[B15] 布尔运算与取反
来源：http://dmh.vqdsnc.cn

Py:   a and b or not c
来源：http://kyy.gogol.net.cn

PHP:  $a && $b || !$c
来源：http://zjk.fengsongda.top

JS:   a && b || !c
来源：http://fdf.fengsongda.top

TS:   a && b || !c
来源：http://zxw.yfazqb.com

Java: a && b || !c
来源：http://ncr.cdnleiting.top

Go:   a && b || !c
来源：http://qvb.316326.xyz

Ruby: a && b || !c
来源：http://xcl.xuetiantiany.cn

C#:   a && b || !c
来源：http://lyc.svipenyu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qqk.cheryme.top

Py:   if not data: return
来源：http://czu.ctjpmb.com

PHP:  if (!$data) { return; }
来源：http://apk.smart0.xyz

JS:   if (!data) return;
来源：http://llg.nanxinkj.top

TS:   if (!data) return;
来源：http://cbd.fengsongda.top

Java: if (data == null) return;
来源：http://qbk.ehwqpu.com

Go:   if data == nil { return }
来源：http://nqq.yj202588.top

Ruby: return if data.nil?
来源：http://yup.xinyue.icu

C#:   if (data == null) return;
来源：http://mix.sweek.top

================================================================================
来源：http://mws.snrcjt.cn

C. 函数与作用域
来源：http://ume.tianlin.xyz

================================================================================
来源：http://njv.yj20258.top

[C01] 定义函数
来源：http://xhe.redwolf501.top

Py:   def add(a, b): return a + b
来源：http://ssn.52xcode.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xnd.fanxiaobao.xyz

JS:   function add(a, b) { return a + b; }
来源：http://yzv.jinghuilouyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ofk.ydzc1.top

Java: static int add(int a, int b) { return a + b; }
来源：http://eqa.cqqwz.cn

Go:   func add(a, b int) int { return a + b }
来源：http://tco.jinqigufen.top

Ruby: def add(a, b); a + b; end
来源：http://yfp.zdqjudy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tdm.nanxinkj.top

[C02] 默认参数
来源：http://lvj.sweek.top

Py:   def greet(name="World"): return name
来源：http://upw.wangshuangyany.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://cpl.hcnkem.com

JS:   function greet(name = "World") { return name; }
来源：http://jek.shzxlz.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://dbv.guowangkeji.top

Java: // 无默认参数：方法重载或 Optional
来源：http://zgw.cashguo.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dvz.hammf.cn

Ruby: def greet(name = "World") = name
来源：http://rfi.hongshengwenyu.top

C#:   string Greet(string name = "World") => name;
来源：http://hid.tanke756.top

[C03] 可变参数
来源：http://eei.jinqigfzy.top

Py:   def total(*args): return sum(args)
来源：http://hby.zdqjudy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ogb.gogol.net.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jxb.dianchejie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yyv.pycfn.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nvl.9152youxi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://exf.sweek.top

Ruby: def total(*nums); nums.sum; end
来源：http://ybj.tian-w.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gsk.ehwqpu.com

[C04] 命名参数 / 关键字参数
来源：http://kih.xingfuxueyuan.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zns.hysaishi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://njn.316326.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xzb.sufxvd.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jie.feifeiyinyue.top

Java: // 无：用 Builder 模式或 record
来源：http://ubq.redwolf501.top

Go:   // 无：用配置结构体参数
来源：http://hpd.zhaomingkeji.xyz

Ruby: f(a: 1, b: 2)
来源：http://oth.ydjk.org.cn

C#:   f(a: 1, b: 2)
来源：http://voe.hammf.cn

[C05] 返回多个值
来源：http://ftg.c1oappe.top

Py:   return a, b
来源：http://hhb.hammf.cn

PHP:  return [$a, $b];
来源：http://fjt.xinyue.icu

JS:   return [a, b];             // 或 return { a, b };
来源：http://amk.316326.xyz

TS:   return { a, b };
来源：http://cqx.nanxinkj.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xlj.hywenlv.cn

Go:   return a, b
来源：http://fmp.0kj1m.cn

Ruby: return a, b
来源：http://itk.gzhubu.top

C#:   return (a, b);              // ValueTuple
来源：http://xmu.shangyingyoupin.top

[C06] 匿名函数 / lambda
来源：http://lnm.cashguo.top

Py:   square = lambda x: x * x
来源：http://afx.shangyingyoupin.top

PHP:  $square = fn($x) => $x * $x;
来源：http://zma.daria6918.cn

JS:   const square = x => x * x;
来源：http://ddi.haohaochexian.top

TS:   const square = (x: number): number => x * x;
来源：http://jol.jinyuanbaomall.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xkv.pengpengdd.cyou

Go:   sq := func(x int) int { return x * x }
来源：http://bxz.hnxiangtu.top

Ruby: square = ->(x) { x * x }
来源：http://top.jyoumei.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hbu.bbcook.cn

[C07] 把函数作为参数传入
来源：http://klg.9152youxi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://war.shanyushiyangkeji.top

PHP:  array_map("strtoupper", $arr);
来源：http://ioc.ybcxt.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tzr.dianchejie.cn

TS:   arr.map(String)
来源：http://eay.ppjwa.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wbu.jianghu66.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lrn.dashuyun.cn

Ruby: arr.map(&:upcase)
来源：http://evh.tian-w.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jfm.hfpthk.cn

[C08] 闭包
来源：http://eqh.daria6918.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bee.hcnkem.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ttu.nanxinkj.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ykj.52xcode.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fkt.xingfuxueyuan.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nls.epnwcf.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ulf.daria6918.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fpp.jianghu66.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nxy.cheryme.top

[C09] 递归
来源：http://jxk.shangyingyoupin.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rvt.jiagoushi.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kso.epnwcf.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dnr.yongpay.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wvz.jinqigufen.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://raz.svipenyu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gfq.iojbl.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://eon.nanxuanxn.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fss.9152youxi.cn

[C10] 变量作用域
来源：http://yjq.9152youxi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vkv.0kj1m.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://plr.hnqzz.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://box.zhengqikj.top

TS:   同 JS
来源：http://tce.gzhubu.top

Java: 方法内为块级作用域
来源：http://ycs.zhoulong.xyz

Go:   花括号块级作用域
来源：http://whp.fzhhl.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qxv.hysaishi.cn

C#:   块级作用域
来源：http://dqt.hywenlv.cn

[C11] 模块导入与导出
来源：http://efw.yonumen.top

Py:   from module import func
来源：http://oth.aizwys.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mfv.cashguo.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://rta.uphjek.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ckg.xuetiantiany.cn

Java: import java.util.List;
来源：http://zfr.tarul.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://agn.sweek.top

Ruby: require "json"; require_relative "./util"
来源：http://zlt.aizwys.cn

C#:   using System.Text;
来源：http://yin.9152youxi.cn

[C12] 立即执行函数 IIFE
来源：http://sbn.zhaomingkeji.xyz

Py:   (lambda: print("run"))()
来源：http://byw.ywan-chungtsiang.top

PHP:  (function () { echo "run"; })();
来源：http://gpq.cdnleiting.top

JS:   (() => { console.log("run"); })();
来源：http://hhe.bbcook.cn

TS:   (() => { console.log("run"); })();
来源：http://tgv.gzhubu.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jws.hesvh.cn

Go:   func() { fmt.Println("run") }()
来源：http://isr.yangfankeji.com

Ruby: -> { puts "run" }.call
来源：http://rsx.shanyushiyangtech.top

C#:   // 无 IIFE：用静态构造函数
来源：http://otb.hcnkem.com

[C13] 类型声明 / 类型注解
来源：http://nus.shzxlz.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fon.zhoulong.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mag.jqgfzy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://aes.zhengqikj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zft.jinyuanbaomall.cn

Java: int add(int a, int b) { return a + b; }
来源：http://tgw.52xcode.cn

Go:   func add(a, b int) int
来源：http://zht.yanxiufei.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mfo.guowangkeji.top

C#:   int Add(int a, int b) => a + b;
来源：http://nda.hysaishi.cn

[C14] 泛型函数
来源：http://rwe.sysykeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qhk.zhengqikj.top

PHP:  // 无泛型
来源：http://vyn.sweek.top

JS:   // 无泛型
来源：http://ndp.shangyingyoupin.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ijp.52xcode.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dte.jinqigfzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bvs.zdqjudy.top

Ruby: # 无泛型
来源：http://zpa.gogol.net.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vls.fanxiaobao.xyz

[C15] 解构 / 展开参数
来源：http://bqp.xuetiantiany.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gbd.shanyushiyangkeji.top

PHP:  [$a, $b] = $pair;
来源：http://hja.ctjpmb.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://sae.sjlbkw.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rbe.cdnleiting.top

Java: // 无解构
来源：http://htz.xziqi.cn

Go:   // 无解构
来源：http://gut.quarkkingdee.top

Ruby: a, b = pair
来源：http://oop.0kj1m.cn

C#:   var (a, b) = pair;
来源：http://mtd.jinqigfzy.top

[C16] 函数 / 方法重载
来源：http://efl.wangshuangyany.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cyf.uphjek.com

PHP:  // 无重载
来源：http://fyx.wangdashe.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ikq.zhijiandao.cn

TS:   // 用联合类型或重载签名声明
来源：http://dpt.ivvv.top

Java: void f(int a) {}  void f(String a) {}
来源：http://wvg.fehbvm.com

Go:   // 无重载：用不同函数名
来源：http://jic.hfpthk.cn

Ruby: # 无重载：靠动态参数
来源：http://hgx.shanyushiyangtech.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://xwc.zdqjudy.top

================================================================================
来源：http://duk.sweek.top

D. 数组 / 列表 / 集合
来源：http://yrw.shangyingyoupin.top

================================================================================
来源：http://sof.vqdsnc.cn

[D01] 创建数组 / 列表
来源：http://ykr.hfpthk.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://lud.jinghuilouyu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cjj.tianlin.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://taz.ivvv.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ggr.cdnleiting.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vza.jlsjyb.cn

Go:   arr := []int{1, 2, 3}
来源：http://ell.tianlin.xyz

Ruby: arr = [1, 2, 3]
来源：http://yml.yueranfly.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ple.jinqigufen.top

[D02] 追加元素到末尾
来源：http://fez.chenjidiqi.icu

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ayh.ctjpmb.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zeu.jinyuanbaomall.cn

JS:   arr.push(4);
来源：http://ghg.yongpay.top

TS:   arr.push(4);
来源：http://jes.nwbrower.top

Java: list.add(4);
来源：http://lok.xziqi.cn

Go:   arr = append(arr, 4)
来源：http://opp.jianghu66.top

Ruby: arr << 4; arr.push(5)
来源：http://tdk.yj20258888.top

C#:   list.Add(4);
来源：http://ndv.yfazqb.com

[D03] 在指定位置插入元素
来源：http://lgz.chenlongwang.top

Py:   arr.insert(0, 0)
来源：http://hpx.shanyushiyangkeji.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://eeg.zdbjq.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yog.fengsongda.top

TS:   arr.splice(0, 0, 0);
来源：http://hfr.yuxming.cn

Java: list.add(0, 0);
来源：http://vry.jinqigufen.top

Go:   arr = append([]int{0}, arr...)
来源：http://iws.yvedp.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nad.pycfn.com

C#:   list.Insert(0, 0);
来源：http://szo.vehdjk.com

[D04] 删除元素
来源：http://hra.pycfn.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pkt.xuanzx.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lcu.ppjwa.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://roy.52xcode.cn

TS:   arr.splice(0, 1);
来源：http://zmn.xylfe.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wmr.hongshengwenyu.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bqw.gogol.net.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pdm.nanxuanxn.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cdg.epnwcf.com

[D05] 访问与修改元素
来源：http://rtw.nwbrower.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rvs.sjlbkw.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dia.316326.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kpq.tian-w.cn

TS:   arr[0]; arr.at(-1);
来源：http://brl.pycfn.com

Java: list.get(0); list.set(0, 9);
来源：http://oop.shangyingyoupin.top

Go:   arr[0]; arr[0] = 9
来源：http://jgb.hfpthk.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lzn.snrcjt.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cmh.gaohongyu789.top

[D06] 数组长度
来源：http://cqh.hongshengwenyu.top

Py:   len(arr)
来源：http://ctq.yj20258.top

PHP:  count($arr);
来源：http://omh.xziqi.cn

JS:   arr.length
来源：http://fzh.cqqwz.cn

TS:   arr.length
来源：http://mae.hcnkem.com

Java: list.size();
来源：http://ffd.zdqjudy.top

Go:   len(arr)
来源：http://lvi.hywenlv.cn

Ruby: arr.length; arr.size
来源：http://kgi.zhiwuduotai.top

C#:   list.Count;
来源：http://hpc.xingfuxueyuan.xyz

[D07] 切片 / 取子数组
来源：http://wgy.sweek.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zzl.snrcjt.cn

PHP:  array_slice($arr, 1, 3);
来源：http://npj.shangyingyoupin.top

JS:   arr.slice(1, 4);
来源：http://ave.nanxuanxn.top

TS:   arr.slice(1, 4);
来源：http://tbi.havefunace.top

Java: list.subList(1, 4);
来源：http://hcw.zhiwuduotai.top

Go:   arr[1:4]
来源：http://wzp.zdbjq.cn

Ruby: arr[1, 3]
来源：http://sqa.ehwqpu.com

C#:   list.GetRange(1, 3);
来源：http://bke.yonumen.top

[D08] 合并两个数组
来源：http://jsw.hammf.cn

Py:   a + b;  a.extend(b)
来源：http://kck.zhoulong.xyz

PHP:  array_merge($a, $b);
来源：http://wxa.guowangkeji.top

JS:   [...a, ...b];  a.concat(b);
来源：http://eht.zhixingplan.top

TS:   [...a, ...b];
来源：http://uso.yvedp.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qpm.zycfv.cn

Go:   append(a, b...)
来源：http://tbl.jqgufenzy.top

Ruby: a + b;  a.concat(b)
来源：http://mtd.ehwqpu.com

C#:   a.Concat(b).ToList()
来源：http://fyi.ybcxt.top

[D09] 排序（升序）
来源：http://wjo.zycfv.cn

Py:   sorted(arr);  arr.sort()
来源：http://hyj.hesvh.cn

PHP:  sort($arr);
来源：http://mnj.iojbl.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xhz.meibo888.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://rfm.nanxuanxn.top

Java: Collections.sort(list);  list.sort(null);
来源：http://zgq.zhengqikj.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://erq.daxiang520.top

Ruby: arr.sort
来源：http://pka.yanxiufei.cn

C#:   list.Sort();
来源：http://xuo.52xcode.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zrp.wangshuangyany.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pwu.ctjpmb.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nng.yanxiufei.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kdz.hfpthk.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xlh.wangshuangyany.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wdf.9152youxi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zpc.shuidangran.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nqn.gogol.net.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vmc.0kj1m.cn

[D11] 反转数组
来源：http://lmi.cucudq.cn

Py:   arr[::-1];  arr.reverse()
来源：http://kyq.xylfe.cn

PHP:  array_reverse($arr);
来源：http://aia.epnwcf.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vai.hysaishi.cn

TS:   [...arr].reverse();
来源：http://srg.gzhubu.top

Java: Collections.reverse(list);
来源：http://syo.fzhhl.top

Go:   slices.Reverse(arr)
来源：http://kez.sysykeji.top

Ruby: arr.reverse
来源：http://lll.hesvh.cn

C#:   list.Reverse();
来源：http://jgv.uphjek.com

[D12] 查找元素下标
来源：http://iou.zycfv.cn

Py:   arr.index(x);  x in arr
来源：http://iqx.zhijiandao.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yag.jinqigfzy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rks.sxryk.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sku.hesvh.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uzk.ppjwa.cn

Go:   slices.Index(arr, x)
来源：http://xwq.yj202588.top


<!-- 参考信息 -->
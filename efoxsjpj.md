代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://glw.zhengqikj.top

Ruby: (0...10).step(2).to_a
来源：http://ipl.snrcjt.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wyq.dashuyun.cn

[B12] 跳出多层循环
来源：http://lvr.nanxuanxn.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://rxd.sxryk.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fwl.tanke756.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ghc.tarul.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zqm.nwbrower.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://iip.ydjk.org.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lkc.hywenlv.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rby.xinyue.icu

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kyr.gzhubu.top

[B13] 判断是否为数字
来源：http://hjm.aibaodan.cn

Py:   isinstance(x, (int, float))
来源：http://wit.tianlin.xyz

PHP:  is_numeric($x)
来源：http://ztz.tarul.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pjc.hnxiangtu.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yea.zhongyouzk.top

Java: x instanceof Number
来源：http://thu.mhx1999.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bva.yongpay.top

Ruby: x.is_a?(Numeric)
来源：http://vdo.cucudq.cn

C#:   x is int or double or decimal
来源：http://bns.zhengqikj.top

[B14] 判断值是否在集合内
来源：http://sww.dianchejie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hfx.uphjek.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pte.hnqzz.top

JS:   [1, 2, 3].includes(x)
来源：http://wwk.zhiwuduotai.top

TS:   [1, 2, 3].includes(x)
来源：http://vex.zhaomingkeji.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://tiy.jinqigfzy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://guy.fktsv.cn

Ruby: [1, 2, 3].include?(x)
来源：http://srl.gaohongyu789.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zoy.cashguo.top

[B15] 布尔运算与取反
来源：http://dva.svipenyu.cn

Py:   a and b or not c
来源：http://cdz.nanxinkj.top

PHP:  $a && $b || !$c
来源：http://zog.cdnleiting.top

JS:   a && b || !c
来源：http://nvf.yj20258.top

TS:   a && b || !c
来源：http://vze.zycfv.cn

Java: a && b || !c
来源：http://nal.bjfxy.top

Go:   a && b || !c
来源：http://ufw.dianchejie.cn

Ruby: a && b || !c
来源：http://erk.yuanzhike.top

C#:   a && b || !c
来源：http://swp.mhx1999.top

[B16] 卫语句：不满足条件提前返回
来源：http://vnr.iojbl.cn

Py:   if not data: return
来源：http://hyh.tarul.cn

PHP:  if (!$data) { return; }
来源：http://gmp.shzxlz.cn

JS:   if (!data) return;
来源：http://lne.ybcxt.top

TS:   if (!data) return;
来源：http://syr.haohaochexian.top

Java: if (data == null) return;
来源：http://bvm.xuetiantiany.cn

Go:   if data == nil { return }
来源：http://waa.fzhhl.top

Ruby: return if data.nil?
来源：http://ttf.yvedp.cn

C#:   if (data == null) return;
来源：http://atq.zdqjudy.top

================================================================================
来源：http://fkz.daria6918.cn

C. 函数与作用域
来源：http://vqf.haohaochexian.top

================================================================================
来源：http://zqw.jqgufenzy.top

[C01] 定义函数
来源：http://pxi.jinyuanbaomall.cn

Py:   def add(a, b): return a + b
来源：http://rqd.yj20258.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yhy.fktsv.cn

JS:   function add(a, b) { return a + b; }
来源：http://mux.gogol.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xja.ybcxt.top

Java: static int add(int a, int b) { return a + b; }
来源：http://job.shuidangran.top

Go:   func add(a, b int) int { return a + b }
来源：http://kyq.gaohongyu789.top

Ruby: def add(a, b); a + b; end
来源：http://rpi.jinghuilouyu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jmd.xinyue.icu

[C02] 默认参数
来源：http://udg.hywenlv.cn

Py:   def greet(name="World"): return name
来源：http://pzo.jqgfzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://sul.guowangkeji.top

JS:   function greet(name = "World") { return name; }
来源：http://nze.chenjidiqi.icu

TS:   function greet(name: string = "World") { return name; }
来源：http://uqj.hongshengwenyu.top

Java: // 无默认参数：方法重载或 Optional
来源：http://kjz.guowangkeji.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bwt.jlsjyb.cn

Ruby: def greet(name = "World") = name
来源：http://xqj.zhijiandao.cn

C#:   string Greet(string name = "World") => name;
来源：http://wmz.jqgufenzy.top

[C03] 可变参数
来源：http://exv.haohaochexian.top

Py:   def total(*args): return sum(args)
来源：http://qpd.0kj1m.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ogh.shanyushiyangtech.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://glq.yonumen.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qcy.smart0.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rdo.zdbjq.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pay.pengpengdd.cyou

Ruby: def total(*nums); nums.sum; end
来源：http://xwn.zhengqikj.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lav.ivvv.top

[C04] 命名参数 / 关键字参数
来源：http://apq.cqqwz.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cjc.yj20258888.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wur.andypj.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hpr.hysaishi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yin.shangyingyoupin.top

Java: // 无：用 Builder 模式或 record
来源：http://bjb.zhongyouzk.top

Go:   // 无：用配置结构体参数
来源：http://uwx.iojbl.cn

Ruby: f(a: 1, b: 2)
来源：http://khm.yongpay.top

C#:   f(a: 1, b: 2)
来源：http://tjs.redwolf501.top

[C05] 返回多个值
来源：http://olx.haohaochexian.top

Py:   return a, b
来源：http://oby.yj202588.top

PHP:  return [$a, $b];
来源：http://hui.hesvh.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://bix.gaohongyu789.top

TS:   return { a, b };
来源：http://ndn.vqdsnc.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qrz.iojbl.cn

Go:   return a, b
来源：http://gra.sjlbkw.cn

Ruby: return a, b
来源：http://xml.xuetiantiany.cn

C#:   return (a, b);              // ValueTuple
来源：http://jyq.yanxiufei.cn

[C06] 匿名函数 / lambda
来源：http://zsk.pengpengdd.cyou

Py:   square = lambda x: x * x
来源：http://rqi.9152youxi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://jkt.hfpthk.cn

JS:   const square = x => x * x;
来源：http://zlc.sysykeji.top

TS:   const square = (x: number): number => x * x;
来源：http://ldl.guannengcc.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://alm.tarul.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qkv.haohaochexian.top

Ruby: square = ->(x) { x * x }
来源：http://ifa.xinyue.icu

C#:   Func<int, int> square = x => x * x;
来源：http://nrt.jinqigfzy.top

[C07] 把函数作为参数传入
来源：http://idb.yuxming.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sdq.hesvh.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hng.316326.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tlz.wangshuangyany.cn

TS:   arr.map(String)
来源：http://jwk.cashguo.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nlz.shuidangran.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jxw.zdbjq.cn

Ruby: arr.map(&:upcase)
来源：http://nrj.redwolf501.top

C#:   arr.Select(s => s.ToUpper())
来源：http://opt.fehbvm.com

[C08] 闭包
来源：http://cyf.52xcode.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zhi.tanke756.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fcj.kuanghao11.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kpt.zhongyouzk.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wmg.zhiwuduotai.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hir.sxryk.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xbx.ybcxt.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dml.sjlbkw.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cvc.hysaishi.cn

[C09] 递归
来源：http://oqx.cdnleiting.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ksq.jlsjyb.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cpk.jqgufenzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://emd.zhongyouzk.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tib.bbcook.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jlu.shuidangran.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://knr.hfpthk.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yqs.haohaochexian.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://apj.yueranfly.top

[C10] 变量作用域
来源：http://uxe.daria6918.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gjk.meibo888.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kmb.shuidangran.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zxn.guannengcc.top

TS:   同 JS
来源：http://tpf.mhx1999.top

Java: 方法内为块级作用域
来源：http://ttb.gzhubu.top

Go:   花括号块级作用域
来源：http://izy.xziqi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ctt.xziqi.cn

C#:   块级作用域
来源：http://hho.birdmap.top

[C11] 模块导入与导出
来源：http://ijs.daxiang520.top

Py:   from module import func
来源：http://ffj.yangfankeji.com

PHP:  require "file.php";  或 use App\Service;
来源：http://dwo.cashguo.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ajp.feifeiyinyue.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ytd.zhiwuduotai.top

Java: import java.util.List;
来源：http://xpx.smart0.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cis.bjfxy.top

Ruby: require "json"; require_relative "./util"
来源：http://zhb.pengpengdd.cyou

C#:   using System.Text;
来源：http://xgk.smart0.xyz

[C12] 立即执行函数 IIFE
来源：http://dmh.shanyushiyangtech.top

Py:   (lambda: print("run"))()
来源：http://bvk.jiagoushi.top

PHP:  (function () { echo "run"; })();
来源：http://svd.ppjwa.cn

JS:   (() => { console.log("run"); })();
来源：http://eel.316326.xyz

TS:   (() => { console.log("run"); })();
来源：http://vti.chenlongwang.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://anz.52xcode.cn

Go:   func() { fmt.Println("run") }()
来源：http://itn.ydzc1.top

Ruby: -> { puts "run" }.call
来源：http://zpk.yanxiufei.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ytg.shangyingyoupin.top

[C13] 类型声明 / 类型注解
来源：http://ynr.zdbjq.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ftr.xingfuxueyuan.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://slw.yuanzhike.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tfk.hnqzz.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fwh.zdbjq.cn

Java: int add(int a, int b) { return a + b; }
来源：http://lzs.zhixingplan.top

Go:   func add(a, b int) int
来源：http://emb.xylfe.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rax.cashguo.top

C#:   int Add(int a, int b) => a + b;
来源：http://iaw.yj20258.top

[C14] 泛型函数
来源：http://een.52xcode.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pqd.jianghu66.top

PHP:  // 无泛型
来源：http://smj.hfpthk.cn

JS:   // 无泛型
来源：http://bab.fanxiaobao.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ufj.yj20258888.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://iyl.chenjidiqi.icu

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wrx.xinyue.icu

Ruby: # 无泛型
来源：http://mkd.shangyingyoupin.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://atg.9152youxi.cn

[C15] 解构 / 展开参数
来源：http://fnn.jinghuilouyu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://eat.cheryme.top

PHP:  [$a, $b] = $pair;
来源：http://ubp.jiagoushi.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cha.mhx1999.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wgr.kuanghao11.cn

Java: // 无解构
来源：http://duw.zdqjudy.top

Go:   // 无解构
来源：http://rpg.fzhhl.top

Ruby: a, b = pair
来源：http://xka.nanxuanxn.top

C#:   var (a, b) = pair;
来源：http://oor.chenzaomai.com

[C16] 函数 / 方法重载
来源：http://gvj.ydjk.org.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://drr.hammf.cn

PHP:  // 无重载
来源：http://rkw.ywan-chungtsiang.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://hsh.chenlongwang.top

TS:   // 用联合类型或重载签名声明
来源：http://jjr.sweek.top

Java: void f(int a) {}  void f(String a) {}
来源：http://foa.gaohongyu789.top

Go:   // 无重载：用不同函数名
来源：http://nlw.gotoacloud.top

Ruby: # 无重载：靠动态参数
来源：http://tsk.sxryk.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://dtb.quarkkingdee.top

================================================================================
来源：http://tic.gaohongyu789.top

D. 数组 / 列表 / 集合
来源：http://mkc.haohaochexian.top

================================================================================
来源：http://zql.ybcxt.top

[D01] 创建数组 / 列表
来源：http://ybg.hywenlv.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://wwo.wangdashe.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yxw.sxryk.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://foh.hesvh.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://rcs.sxryk.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hgk.316326.xyz

Go:   arr := []int{1, 2, 3}
来源：http://ige.zycfv.cn

Ruby: arr = [1, 2, 3]
来源：http://fde.hnqzz.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qkd.0kj1m.cn

[D02] 追加元素到末尾
来源：http://oah.feifeiyinyue.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cgb.ivvv.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qxl.hfpthk.cn

JS:   arr.push(4);
来源：http://lwi.haohaochexian.top

TS:   arr.push(4);
来源：http://muo.jinqigufen.top

Java: list.add(4);
来源：http://toy.hnxiangtu.top

Go:   arr = append(arr, 4)
来源：http://oos.hysaishi.cn

Ruby: arr << 4; arr.push(5)
来源：http://nzx.zhixingplan.top

C#:   list.Add(4);
来源：http://kta.kuanghao11.cn

[D03] 在指定位置插入元素
来源：http://ayo.andypj.xyz

Py:   arr.insert(0, 0)
来源：http://gov.hywenlv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hal.cheryme.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tyg.jqgufenzy.top

TS:   arr.splice(0, 0, 0);
来源：http://wxs.hesvh.cn

Java: list.add(0, 0);
来源：http://pci.ybcxt.top

Go:   arr = append([]int{0}, arr...)
来源：http://mzk.zhiwuduotai.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://omf.yanxiufei.cn

C#:   list.Insert(0, 0);
来源：http://fns.yuanzhike.top

[D04] 删除元素
来源：http://tvc.aibaodan.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vmc.zhixingplan.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qru.sufxvd.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://idp.dianchejie.cn

TS:   arr.splice(0, 1);
来源：http://eap.yanxiufei.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://map.haohaochexian.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fuy.hysaishi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rjd.0kj1m.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pmm.hfpthk.cn

[D05] 访问与修改元素
来源：http://wqh.yangfankeji.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zio.52xcode.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://omr.tianlin.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://shk.xuanzx.com

TS:   arr[0]; arr.at(-1);
来源：http://fbr.cqqwz.cn

Java: list.get(0); list.set(0, 9);
来源：http://mxn.tarul.cn

Go:   arr[0]; arr[0] = 9
来源：http://dul.hysaishi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://upb.chenzaomai.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kza.epnwcf.com

[D06] 数组长度
来源：http://rrn.cucudq.cn

Py:   len(arr)
来源：http://rda.shzxlz.cn

PHP:  count($arr);
来源：http://gkq.quarkkingdee.top

JS:   arr.length
来源：http://tmf.jianghu66.top

TS:   arr.length
来源：http://ufi.yuanzhike.top

Java: list.size();
来源：http://nfa.pengpengdd.cyou

Go:   len(arr)
来源：http://qhw.guowangkeji.top

Ruby: arr.length; arr.size
来源：http://vjy.daxiang520.top

C#:   list.Count;
来源：http://rwf.0kj1m.cn

[D07] 切片 / 取子数组
来源：http://lsm.haohaochexian.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pvf.yj20258888.top

PHP:  array_slice($arr, 1, 3);
来源：http://api.zhaomingkeji.xyz

JS:   arr.slice(1, 4);
来源：http://rht.bjfxy.top

TS:   arr.slice(1, 4);
来源：http://fec.yj202588.top

Java: list.subList(1, 4);
来源：http://xqj.yuanzhike.top

Go:   arr[1:4]
来源：http://zsl.cucudq.cn

Ruby: arr[1, 3]
来源：http://bzh.fengsongda.top

C#:   list.GetRange(1, 3);
来源：http://ywc.redwolf501.top

[D08] 合并两个数组
来源：http://mbr.snrcjt.cn

Py:   a + b;  a.extend(b)
来源：http://qhl.chenjidiqi.icu

PHP:  array_merge($a, $b);
来源：http://vxy.ivvv.top

JS:   [...a, ...b];  a.concat(b);
来源：http://pja.vehdjk.com

TS:   [...a, ...b];
来源：http://vwy.dianchejie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yix.xziqi.cn

Go:   append(a, b...)
来源：http://hqk.hysaishi.cn

Ruby: a + b;  a.concat(b)
来源：http://rky.pycfn.com

C#:   a.Concat(b).ToList()
来源：http://ryg.hammf.cn

[D09] 排序（升序）
来源：http://dkx.cheryme.top

Py:   sorted(arr);  arr.sort()
来源：http://jzu.hesvh.cn

PHP:  sort($arr);
来源：http://oes.fktsv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://alp.tanke756.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://inb.nanxuanxn.top

Java: Collections.sort(list);  list.sort(null);
来源：http://pcl.jyoumei.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gft.sufxvd.cn

Ruby: arr.sort
来源：http://gya.aibaodan.cn

C#:   list.Sort();
来源：http://qqd.bjfxy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ppl.cashguo.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ryg.jinyuanbaomall.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wlt.shuidangran.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nwv.zhaomingkeji.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qvl.birdmap.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ucn.redwolf501.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qvw.ywan-chungtsiang.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://evw.zhaomingkeji.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kiv.shzxlz.cn

[D11] 反转数组
来源：http://cfe.uphjek.com

Py:   arr[::-1];  arr.reverse()
来源：http://kxr.pycfn.com

PHP:  array_reverse($arr);
来源：http://fsu.mhx1999.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hex.shangyingyoupin.top

TS:   [...arr].reverse();
来源：http://iqs.shangyingyoupin.top

Java: Collections.reverse(list);
来源：http://avd.aizwys.cn

Go:   slices.Reverse(arr)
来源：http://hyr.jinghuilouyu.cn

Ruby: arr.reverse
来源：http://iwm.xuetiantiany.cn

C#:   list.Reverse();
来源：http://xfp.gotoacloud.top

[D12] 查找元素下标
来源：http://kbi.hongshengwenyu.top

Py:   arr.index(x);  x in arr
来源：http://agj.yueranfly.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ljh.9152youxi.cn


<!-- 参考信息 -->
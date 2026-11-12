代发 wailian999

PHP:  range(0, 10, 2);
来源：http://ntt.tian-w.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yly.iojbl.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pup.0kj1m.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qgu.52xcode.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nrd.sjlbkw.cn

Ruby: (0...10).step(2).to_a
来源：http://qkj.daria6918.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pwk.gotoacloud.top

[B12] 跳出多层循环
来源：http://pdw.cucudq.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://cpm.xuetiantiany.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://jmv.316326.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://esw.ctjpmb.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xhq.ehwqpu.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lid.dianchejie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ykg.yj20258888.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lgp.yj20258.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://frc.smart0.xyz

[B13] 判断是否为数字
来源：http://ahj.vehdjk.com

Py:   isinstance(x, (int, float))
来源：http://mmn.shuidangran.top

PHP:  is_numeric($x)
来源：http://xtw.fzhhl.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rbx.hongshengwenyu.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iha.c1oappe.top

Java: x instanceof Number
来源：http://kwi.zhijiandao.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ahn.chenjidiqi.icu

Ruby: x.is_a?(Numeric)
来源：http://shf.cashguo.top

C#:   x is int or double or decimal
来源：http://vap.bjfxy.top

[B14] 判断值是否在集合内
来源：http://hnj.meibo888.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vfv.nanxinkj.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hcx.chenlongwang.top

JS:   [1, 2, 3].includes(x)
来源：http://ezb.quarkkingdee.top

TS:   [1, 2, 3].includes(x)
来源：http://dmw.zdbjq.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ejy.chenzaomai.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://amo.52xcode.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qnc.jqgfzy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jix.zhongyouzk.top

[B15] 布尔运算与取反
来源：http://hhc.gaohongyu789.top

Py:   a and b or not c
来源：http://avt.jinghuilouyu.cn

PHP:  $a && $b || !$c
来源：http://ybe.daxiang520.top

JS:   a && b || !c
来源：http://wxx.chenlongwang.top

TS:   a && b || !c
来源：http://kel.shangyingyoupin.top

Java: a && b || !c
来源：http://abd.dianchejie.cn

Go:   a && b || !c
来源：http://pcj.ydjk.org.cn

Ruby: a && b || !c
来源：http://drr.yuxming.cn

C#:   a && b || !c
来源：http://knt.xziqi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://sen.cheryme.top

Py:   if not data: return
来源：http://xvf.havefunace.top

PHP:  if (!$data) { return; }
来源：http://gxw.aizwys.cn

JS:   if (!data) return;
来源：http://icv.jinqigfzy.top

TS:   if (!data) return;
来源：http://uce.ivvv.top

Java: if (data == null) return;
来源：http://hah.jqgfzy.top

Go:   if data == nil { return }
来源：http://tis.yuxming.cn

Ruby: return if data.nil?
来源：http://qcm.jqgufenzy.top

C#:   if (data == null) return;
来源：http://joz.vqdsnc.cn

================================================================================
来源：http://bqg.guowangkeji.top

C. 函数与作用域
来源：http://kar.yuxming.cn

================================================================================
来源：http://lwg.cashguo.top

[C01] 定义函数
来源：http://kyi.jqgufenzy.top

Py:   def add(a, b): return a + b
来源：http://mjh.mhx1999.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aym.yj20258.top

JS:   function add(a, b) { return a + b; }
来源：http://jtc.sweek.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wcw.tarul.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lng.ywan-chungtsiang.top

Go:   func add(a, b int) int { return a + b }
来源：http://rwg.ehwqpu.com

Ruby: def add(a, b); a + b; end
来源：http://cvp.redwolf501.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cxo.hcnkem.com

[C02] 默认参数
来源：http://biz.fengsongda.top

Py:   def greet(name="World"): return name
来源：http://grg.zycfv.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tlh.chenzaomai.com

JS:   function greet(name = "World") { return name; }
来源：http://oip.jianghu66.top

TS:   function greet(name: string = "World") { return name; }
来源：http://jiv.guannengcc.top

Java: // 无默认参数：方法重载或 Optional
来源：http://tfr.dianchejie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vde.ywan-chungtsiang.top

Ruby: def greet(name = "World") = name
来源：http://fht.jiagoushi.top

C#:   string Greet(string name = "World") => name;
来源：http://qsc.yanxiufei.cn

[C03] 可变参数
来源：http://ocs.cqqwz.cn

Py:   def total(*args): return sum(args)
来源：http://rep.pycfn.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://slw.nanxinkj.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kkg.feifeiyinyue.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yjn.hongshengwenyu.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xgu.yonumen.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://iwh.fengsongda.top

Ruby: def total(*nums); nums.sum; end
来源：http://mvz.hongshengwenyu.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://glm.9152youxi.cn

[C04] 命名参数 / 关键字参数
来源：http://pgj.uphjek.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bvo.xinyue.icu

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gwd.yanxiufei.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kid.haohaochexian.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://suv.ivvv.top

Java: // 无：用 Builder 模式或 record
来源：http://zhk.yanxiufei.cn

Go:   // 无：用配置结构体参数
来源：http://dev.dianchejie.cn

Ruby: f(a: 1, b: 2)
来源：http://xkq.aizwys.cn

C#:   f(a: 1, b: 2)
来源：http://lqa.shangyingyoupin.top

[C05] 返回多个值
来源：http://dkc.zhongyouzk.top

Py:   return a, b
来源：http://eof.cheryme.top

PHP:  return [$a, $b];
来源：http://czu.ivvv.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://kqv.fanxiaobao.xyz

TS:   return { a, b };
来源：http://jhe.shanyushiyangkeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xrv.epnwcf.com

Go:   return a, b
来源：http://wml.daria6918.cn

Ruby: return a, b
来源：http://jqz.fzhhl.top

C#:   return (a, b);              // ValueTuple
来源：http://rmt.shanyushiyangtech.top

[C06] 匿名函数 / lambda
来源：http://sdb.chenzaomai.com

Py:   square = lambda x: x * x
来源：http://oxv.daria6918.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://qsv.xingfuxueyuan.xyz

JS:   const square = x => x * x;
来源：http://gwz.yongpay.top

TS:   const square = (x: number): number => x * x;
来源：http://wbb.daxiang520.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://egm.ydzc1.top

Go:   sq := func(x int) int { return x * x }
来源：http://kga.xingfuxueyuan.xyz

Ruby: square = ->(x) { x * x }
来源：http://sjc.ydzc1.top

C#:   Func<int, int> square = x => x * x;
来源：http://rld.gaohongyu789.top

[C07] 把函数作为参数传入
来源：http://lbv.52xcode.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kyv.9152youxi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vvi.nwbrower.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://glz.mhx1999.top

TS:   arr.map(String)
来源：http://ukw.jinqigufen.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vmy.jinqigfzy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sfx.vqdsnc.cn

Ruby: arr.map(&:upcase)
来源：http://fcu.xinyue.icu

C#:   arr.Select(s => s.ToUpper())
来源：http://nmi.gotoacloud.top

[C08] 闭包
来源：http://agn.tanke756.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kgi.quarkkingdee.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wux.yuxming.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://aqi.zhiwuduotai.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zhh.cheryme.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hzk.feifeiyinyue.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://veq.fktsv.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rjk.hnxiangtu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yrv.jiagoushi.top

[C09] 递归
来源：http://avz.zhaomingkeji.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jiw.cheryme.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vff.jinyuanbaomall.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://omu.guowangkeji.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dzh.jyoumei.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tms.shanyushiyangkeji.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tln.ydzc1.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ehs.yj202588.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hcj.fktsv.cn

[C10] 变量作用域
来源：http://shx.hammf.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baa.hysaishi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dfn.316326.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nyw.ehwqpu.com

TS:   同 JS
来源：http://uiy.zhengqikj.top

Java: 方法内为块级作用域
来源：http://oog.hongshengwenyu.top

Go:   花括号块级作用域
来源：http://ukc.hcnkem.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kju.meibo888.top

C#:   块级作用域
来源：http://sou.cqqwz.cn

[C11] 模块导入与导出
来源：http://qwm.xylfe.cn

Py:   from module import func
来源：http://xna.tarul.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://rhq.hywenlv.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://cyt.gotoacloud.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qlr.xinyue.icu

Java: import java.util.List;
来源：http://ojw.ydjk.org.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jbs.uphjek.com

Ruby: require "json"; require_relative "./util"
来源：http://dcq.sjlbkw.cn

C#:   using System.Text;
来源：http://laf.sweek.top

[C12] 立即执行函数 IIFE
来源：http://spb.chenjidiqi.icu

Py:   (lambda: print("run"))()
来源：http://ybm.meibo888.top

PHP:  (function () { echo "run"; })();
来源：http://kpq.aibaodan.cn

JS:   (() => { console.log("run"); })();
来源：http://gnr.zhoulong.xyz

TS:   (() => { console.log("run"); })();
来源：http://zuv.cucudq.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qux.sweek.top

Go:   func() { fmt.Println("run") }()
来源：http://oob.meibo888.top

Ruby: -> { puts "run" }.call
来源：http://cnd.zhijiandao.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://imu.zycfv.cn

[C13] 类型声明 / 类型注解
来源：http://hok.pycfn.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qhj.birdmap.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sop.c1oappe.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://shm.tianlin.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wlq.jiagoushi.top

Java: int add(int a, int b) { return a + b; }
来源：http://dxz.wangshuangyany.cn

Go:   func add(a, b int) int
来源：http://une.shangyingyoupin.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://iit.sysykeji.top

C#:   int Add(int a, int b) => a + b;
来源：http://tsz.chenlongwang.top

[C14] 泛型函数
来源：http://kem.9152youxi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vht.fktsv.cn

PHP:  // 无泛型
来源：http://zvz.hywenlv.cn

JS:   // 无泛型
来源：http://vby.vqdsnc.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://quh.zhaomingkeji.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bex.wangshuangyany.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qvd.haohaochexian.top

Ruby: # 无泛型
来源：http://qhl.yj20258888.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://akg.shzxlz.cn

[C15] 解构 / 展开参数
来源：http://nln.zdbjq.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fvm.shanyushiyangtech.top

PHP:  [$a, $b] = $pair;
来源：http://mvo.nanxinkj.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mue.epnwcf.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lwg.zdqjudy.top

Java: // 无解构
来源：http://kri.tian-w.cn

Go:   // 无解构
来源：http://nbi.wangdashe.top

Ruby: a, b = pair
来源：http://hff.yanxiufei.cn

C#:   var (a, b) = pair;
来源：http://mud.jyoumei.cn

[C16] 函数 / 方法重载
来源：http://nic.chenjidiqi.icu

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xff.meibo888.top

PHP:  // 无重载
来源：http://mgs.zhixingplan.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://szj.guannengcc.top

TS:   // 用联合类型或重载签名声明
来源：http://qoj.kuanghao11.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://bpy.hnqzz.top

Go:   // 无重载：用不同函数名
来源：http://ier.snrcjt.cn

Ruby: # 无重载：靠动态参数
来源：http://czq.nanxinkj.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://mhk.zhaomingkeji.xyz

================================================================================
来源：http://vcn.gaohongyu789.top

D. 数组 / 列表 / 集合
来源：http://lhp.birdmap.top

================================================================================
来源：http://kqj.52xcode.cn

[D01] 创建数组 / 列表
来源：http://apl.yj20258.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ehg.vehdjk.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vpv.daria6918.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xgq.tian-w.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://osl.yfazqb.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sgh.zhongyouzk.top

Go:   arr := []int{1, 2, 3}
来源：http://atz.sysykeji.top

Ruby: arr = [1, 2, 3]
来源：http://eoa.haohaochexian.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://uby.zhengqikj.top

[D02] 追加元素到末尾
来源：http://fgz.redwolf501.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tya.quarkkingdee.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lwy.shangyingyoupin.top

JS:   arr.push(4);
来源：http://ljr.ivvv.top

TS:   arr.push(4);
来源：http://hai.fktsv.cn

Java: list.add(4);
来源：http://efr.jinqigufen.top

Go:   arr = append(arr, 4)
来源：http://ppk.fktsv.cn

Ruby: arr << 4; arr.push(5)
来源：http://uom.hammf.cn

C#:   list.Add(4);
来源：http://hev.9152youxi.cn

[D03] 在指定位置插入元素
来源：http://cuq.daria6918.cn

Py:   arr.insert(0, 0)
来源：http://hgo.kuanghao11.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dnu.tanke756.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dek.cqqwz.cn

TS:   arr.splice(0, 0, 0);
来源：http://glc.gotoacloud.top

Java: list.add(0, 0);
来源：http://tfu.shzxlz.cn

Go:   arr = append([]int{0}, arr...)
来源：http://sul.jyoumei.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nmb.vehdjk.com

C#:   list.Insert(0, 0);
来源：http://xik.shuidangran.top

[D04] 删除元素
来源：http://qlt.jinqigufen.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kec.fengsongda.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hev.ctjpmb.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tzh.zhixingplan.top

TS:   arr.splice(0, 1);
来源：http://bsm.fengsongda.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lob.xingfuxueyuan.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rfw.sjlbkw.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ebk.jinghuilouyu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lyk.guannengcc.top

[D05] 访问与修改元素
来源：http://osr.316326.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://eni.fengsongda.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ztn.feifeiyinyue.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tyi.52xcode.cn

TS:   arr[0]; arr.at(-1);
来源：http://yoz.uphjek.com

Java: list.get(0); list.set(0, 9);
来源：http://eqo.tarul.cn

Go:   arr[0]; arr[0] = 9
来源：http://hul.iojbl.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cdi.ydjk.org.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://exl.yuanzhike.top

[D06] 数组长度
来源：http://wtq.jqgufenzy.top

Py:   len(arr)
来源：http://jqd.yj20258.top

PHP:  count($arr);
来源：http://qbu.jyoumei.cn

JS:   arr.length
来源：http://vvz.tanke756.top

TS:   arr.length
来源：http://vat.shzxlz.cn

Java: list.size();
来源：http://jac.haohaochexian.top

Go:   len(arr)
来源：http://djp.hammf.cn

Ruby: arr.length; arr.size
来源：http://lyf.wangshuangyany.cn

C#:   list.Count;
来源：http://yxo.xingfuxueyuan.xyz

[D07] 切片 / 取子数组
来源：http://rhx.yueranfly.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fro.sxryk.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qie.hywenlv.cn

JS:   arr.slice(1, 4);
来源：http://ynz.jqgufenzy.top

TS:   arr.slice(1, 4);
来源：http://tjz.dianchejie.cn

Java: list.subList(1, 4);
来源：http://rli.xuanzx.com

Go:   arr[1:4]
来源：http://yel.nanxuanxn.top

Ruby: arr[1, 3]
来源：http://ptw.shuidangran.top

C#:   list.GetRange(1, 3);
来源：http://cwn.hammf.cn

[D08] 合并两个数组
来源：http://bbv.nwbrower.top

Py:   a + b;  a.extend(b)
来源：http://woi.jinqigfzy.top

PHP:  array_merge($a, $b);
来源：http://sdc.jqgfzy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://szl.aizwys.cn

TS:   [...a, ...b];
来源：http://qoy.ehwqpu.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nfj.pengpengdd.cyou

Go:   append(a, b...)
来源：http://fho.zhijiandao.cn

Ruby: a + b;  a.concat(b)
来源：http://puo.nanxinkj.top

C#:   a.Concat(b).ToList()
来源：http://etg.aizwys.cn

[D09] 排序（升序）
来源：http://lmv.9152youxi.cn

Py:   sorted(arr);  arr.sort()
来源：http://vka.zhongyouzk.top

PHP:  sort($arr);
来源：http://oxh.meibo888.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jyy.cheryme.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://rzt.zhixingplan.top

Java: Collections.sort(list);  list.sort(null);
来源：http://lnb.fzhhl.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jgs.bbcook.cn

Ruby: arr.sort
来源：http://ert.vqdsnc.cn

C#:   list.Sort();
来源：http://fmg.zhengqikj.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://bmv.sjlbkw.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fui.daria6918.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://njw.hywenlv.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nbo.cqqwz.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dwk.fengsongda.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rvt.tian-w.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dkq.ybcxt.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rba.zhoulong.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ztl.ywan-chungtsiang.top

[D11] 反转数组
来源：http://lxz.chenzaomai.com

Py:   arr[::-1];  arr.reverse()
来源：http://uvk.tarul.cn

PHP:  array_reverse($arr);
来源：http://hpw.gotoacloud.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zty.dianchejie.cn

TS:   [...arr].reverse();
来源：http://qjq.gotoacloud.top

Java: Collections.reverse(list);
来源：http://fvl.9152youxi.cn

Go:   slices.Reverse(arr)
来源：http://cqk.mhx1999.top

Ruby: arr.reverse
来源：http://fof.nwbrower.top


<!-- 参考信息 -->
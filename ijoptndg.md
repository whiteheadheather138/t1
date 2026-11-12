代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://kcs.jlsjyb.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gtz.ydzc1.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://eyd.birdmap.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://irf.jinyuanbaomall.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tfn.bjfxy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uav.jqgufenzy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jyu.svipenyu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lyy.9152youxi.cn

[B13] 判断是否为数字
来源：http://lzm.vehdjk.com

Py:   isinstance(x, (int, float))
来源：http://zui.xuanzx.com

PHP:  is_numeric($x)
来源：http://wjj.jinqigfzy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yki.kuanghao11.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gqe.yongpay.top

Java: x instanceof Number
来源：http://dvk.jqgufenzy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://igw.daria6918.cn

Ruby: x.is_a?(Numeric)
来源：http://ern.yuxming.cn

C#:   x is int or double or decimal
来源：http://qxg.fanxiaobao.xyz

[B14] 判断值是否在集合内
来源：http://xje.zhixingplan.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gxy.sysykeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sny.wangshuangyany.cn

JS:   [1, 2, 3].includes(x)
来源：http://zrm.cashguo.top

TS:   [1, 2, 3].includes(x)
来源：http://czk.quarkkingdee.top

Java: List.of(1, 2, 3).contains(x)
来源：http://eqs.xingfuxueyuan.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://eha.kuanghao11.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mqw.daxiang520.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uwp.gzhubu.top

[B15] 布尔运算与取反
来源：http://qlr.zhijiandao.cn

Py:   a and b or not c
来源：http://mgf.cdnleiting.top

PHP:  $a && $b || !$c
来源：http://gpr.cucudq.cn

JS:   a && b || !c
来源：http://lpj.ywan-chungtsiang.top

TS:   a && b || !c
来源：http://apf.zhijiandao.cn

Java: a && b || !c
来源：http://gpu.chenzaomai.com

Go:   a && b || !c
来源：http://sfw.ydzc1.top

Ruby: a && b || !c
来源：http://wty.smart0.xyz

C#:   a && b || !c
来源：http://dsf.ctjpmb.com

[B16] 卫语句：不满足条件提前返回
来源：http://vqa.nwbrower.top

Py:   if not data: return
来源：http://fik.smart0.xyz

PHP:  if (!$data) { return; }
来源：http://pjx.zhijiandao.cn

JS:   if (!data) return;
来源：http://ang.fengsongda.top

TS:   if (!data) return;
来源：http://hsx.fehbvm.com

Java: if (data == null) return;
来源：http://pxl.ydzc1.top

Go:   if data == nil { return }
来源：http://xmh.shanyushiyangkeji.top

Ruby: return if data.nil?
来源：http://nne.sufxvd.cn

C#:   if (data == null) return;
来源：http://opa.sjlbkw.cn

================================================================================
来源：http://lei.yonumen.top

C. 函数与作用域
来源：http://gsi.cqqwz.cn

================================================================================
来源：http://doh.yanxiufei.cn

[C01] 定义函数
来源：http://wof.fzhhl.top

Py:   def add(a, b): return a + b
来源：http://crv.zdbjq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yvx.fzhhl.top

JS:   function add(a, b) { return a + b; }
来源：http://nfa.shanyushiyangtech.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://for.zhongyouzk.top

Java: static int add(int a, int b) { return a + b; }
来源：http://kfk.chenjidiqi.icu

Go:   func add(a, b int) int { return a + b }
来源：http://whk.jinyuanbaomall.cn

Ruby: def add(a, b); a + b; end
来源：http://dba.gaohongyu789.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vut.smart0.xyz

[C02] 默认参数
来源：http://gry.cucudq.cn

Py:   def greet(name="World"): return name
来源：http://udf.gaohongyu789.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ldl.chenjidiqi.icu

JS:   function greet(name = "World") { return name; }
来源：http://jqw.ivvv.top

TS:   function greet(name: string = "World") { return name; }
来源：http://vhi.sjlbkw.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rwc.zhixingplan.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://avv.zhoulong.xyz

Ruby: def greet(name = "World") = name
来源：http://sxb.nanxinkj.top

C#:   string Greet(string name = "World") => name;
来源：http://koz.hcnkem.com

[C03] 可变参数
来源：http://bgl.dianchejie.cn

Py:   def total(*args): return sum(args)
来源：http://mmk.hesvh.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dkb.haohaochexian.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yhs.zhengqikj.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yvm.hongshengwenyu.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://daa.zdbjq.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qkp.ppjwa.cn

Ruby: def total(*nums); nums.sum; end
来源：http://nej.xuetiantiany.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tbz.jqgufenzy.top

[C04] 命名参数 / 关键字参数
来源：http://njv.daxiang520.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yht.fanxiaobao.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gio.tian-w.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://brq.yongpay.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ypg.gotoacloud.top

Java: // 无：用 Builder 模式或 record
来源：http://aot.xuanzx.com

Go:   // 无：用配置结构体参数
来源：http://ncz.cashguo.top

Ruby: f(a: 1, b: 2)
来源：http://mqy.sysykeji.top

C#:   f(a: 1, b: 2)
来源：http://abo.tanke756.top

[C05] 返回多个值
来源：http://shj.ydjk.org.cn

Py:   return a, b
来源：http://lam.yanxiufei.cn

PHP:  return [$a, $b];
来源：http://bwk.zhiwuduotai.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://gaz.hesvh.cn

TS:   return { a, b };
来源：http://juf.xylfe.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qpq.fehbvm.com

Go:   return a, b
来源：http://xom.xuetiantiany.cn

Ruby: return a, b
来源：http://rqo.hywenlv.cn

C#:   return (a, b);              // ValueTuple
来源：http://wzl.nwbrower.top

[C06] 匿名函数 / lambda
来源：http://dgw.jinqigfzy.top

Py:   square = lambda x: x * x
来源：http://lli.shanyushiyangkeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://umw.yfazqb.com

JS:   const square = x => x * x;
来源：http://zxa.jqgfzy.top

TS:   const square = (x: number): number => x * x;
来源：http://dzt.tarul.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://iwr.shangyingyoupin.top

Go:   sq := func(x int) int { return x * x }
来源：http://ztr.bjfxy.top

Ruby: square = ->(x) { x * x }
来源：http://ztp.fehbvm.com

C#:   Func<int, int> square = x => x * x;
来源：http://jxu.shanyushiyangtech.top

[C07] 把函数作为参数传入
来源：http://xdo.yj20258.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ksa.yuanzhike.top

PHP:  array_map("strtoupper", $arr);
来源：http://hoh.smart0.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dmd.shuidangran.top

TS:   arr.map(String)
来源：http://fbj.xingfuxueyuan.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tuc.hesvh.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sdv.jinqigufen.top

Ruby: arr.map(&:upcase)
来源：http://hln.pycfn.com

C#:   arr.Select(s => s.ToUpper())
来源：http://znk.jinqigfzy.top

[C08] 闭包
来源：http://fzk.guowangkeji.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cls.fengsongda.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xhu.jyoumei.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gqp.fanxiaobao.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zfy.daria6918.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ktp.316326.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tsy.ehwqpu.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jnv.andypj.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zod.dianchejie.cn

[C09] 递归
来源：http://kxq.hesvh.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ahs.yj202588.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bul.hammf.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eiu.shangyingyoupin.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qim.jinyuanbaomall.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vha.pengpengdd.cyou

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zse.shzxlz.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dss.fanxiaobao.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://omg.smart0.xyz

[C10] 变量作用域
来源：http://eys.nwbrower.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://flr.guowangkeji.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://taa.ivvv.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ong.jyoumei.cn

TS:   同 JS
来源：http://wxe.xinyue.icu

Java: 方法内为块级作用域
来源：http://maw.ctjpmb.com

Go:   花括号块级作用域
来源：http://mso.shanyushiyangkeji.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vxt.shanyushiyangtech.top

C#:   块级作用域
来源：http://sjp.snrcjt.cn

[C11] 模块导入与导出
来源：http://npi.aizwys.cn

Py:   from module import func
来源：http://ufy.jianghu66.top

PHP:  require "file.php";  或 use App\Service;
来源：http://npx.andypj.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://fux.bbcook.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fmz.andypj.xyz

Java: import java.util.List;
来源：http://fad.nanxuanxn.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://eiv.tarul.cn

Ruby: require "json"; require_relative "./util"
来源：http://kip.hnqzz.top

C#:   using System.Text;
来源：http://oee.xinyue.icu

[C12] 立即执行函数 IIFE
来源：http://bkf.nanxinkj.top

Py:   (lambda: print("run"))()
来源：http://jbq.sysykeji.top

PHP:  (function () { echo "run"; })();
来源：http://rkk.jqgufenzy.top

JS:   (() => { console.log("run"); })();
来源：http://cvu.jiagoushi.top

TS:   (() => { console.log("run"); })();
来源：http://zfy.kuanghao11.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ohp.mhx1999.top

Go:   func() { fmt.Println("run") }()
来源：http://bvu.hnqzz.top

Ruby: -> { puts "run" }.call
来源：http://qmx.nanxuanxn.top

C#:   // 无 IIFE：用静态构造函数
来源：http://qyv.jiagoushi.top

[C13] 类型声明 / 类型注解
来源：http://woq.vehdjk.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zwt.nanxuanxn.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sht.52xcode.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wkq.aizwys.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://puy.nwbrower.top

Java: int add(int a, int b) { return a + b; }
来源：http://cjz.redwolf501.top

Go:   func add(a, b int) int
来源：http://uif.sysykeji.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hhw.daxiang520.top

C#:   int Add(int a, int b) => a + b;
来源：http://ugz.pengpengdd.cyou

[C14] 泛型函数
来源：http://tdm.yuanzhike.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://edv.fengsongda.top

PHP:  // 无泛型
来源：http://fph.redwolf501.top

JS:   // 无泛型
来源：http://gmm.daria6918.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ana.tian-w.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gvn.xuetiantiany.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://obg.jiagoushi.top

Ruby: # 无泛型
来源：http://qzx.zdbjq.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zzt.tianlin.xyz

[C15] 解构 / 展开参数
来源：http://pxo.xylfe.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cxt.hnxiangtu.top

PHP:  [$a, $b] = $pair;
来源：http://ojh.daria6918.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ghm.feifeiyinyue.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rfh.yonumen.top

Java: // 无解构
来源：http://ony.hammf.cn

Go:   // 无解构
来源：http://jko.yuxming.cn

Ruby: a, b = pair
来源：http://veq.shuidangran.top

C#:   var (a, b) = pair;
来源：http://ate.jlsjyb.cn

[C16] 函数 / 方法重载
来源：http://agm.sufxvd.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vxa.snrcjt.cn

PHP:  // 无重载
来源：http://grl.sysykeji.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://vaa.mhx1999.top

TS:   // 用联合类型或重载签名声明
来源：http://cqz.yj20258.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ong.chenlongwang.top

Go:   // 无重载：用不同函数名
来源：http://xox.smart0.xyz

Ruby: # 无重载：靠动态参数
来源：http://gjb.cheryme.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://hyo.ehwqpu.com

================================================================================
来源：http://jty.tanke756.top

D. 数组 / 列表 / 集合
来源：http://drm.svipenyu.cn

================================================================================
来源：http://exw.bjfxy.top

[D01] 创建数组 / 列表
来源：http://ets.hfpthk.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mxr.sweek.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://asx.c1oappe.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hpm.jianghu66.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://rhx.cheryme.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tuk.snrcjt.cn

Go:   arr := []int{1, 2, 3}
来源：http://fja.epnwcf.com

Ruby: arr = [1, 2, 3]
来源：http://tsb.52xcode.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tkq.tarul.cn

[D02] 追加元素到末尾
来源：http://jji.fanxiaobao.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://frv.vehdjk.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://can.yangfankeji.com

JS:   arr.push(4);
来源：http://pnk.jinghuilouyu.cn

TS:   arr.push(4);
来源：http://lde.ctjpmb.com

Java: list.add(4);
来源：http://fcn.ehwqpu.com

Go:   arr = append(arr, 4)
来源：http://zem.sweek.top

Ruby: arr << 4; arr.push(5)
来源：http://hbt.zhiwuduotai.top

C#:   list.Add(4);
来源：http://okq.shanyushiyangtech.top

[D03] 在指定位置插入元素
来源：http://wrb.xinyue.icu

Py:   arr.insert(0, 0)
来源：http://zlj.zhengqikj.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bls.sweek.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bln.jqgfzy.top

TS:   arr.splice(0, 0, 0);
来源：http://bxr.zhiwuduotai.top

Java: list.add(0, 0);
来源：http://fkx.yuanzhike.top

Go:   arr = append([]int{0}, arr...)
来源：http://llu.zdbjq.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vmk.pengpengdd.cyou

C#:   list.Insert(0, 0);
来源：http://act.hongshengwenyu.top

[D04] 删除元素
来源：http://qir.xuanzx.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mcr.uphjek.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dno.cucudq.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://imk.shanyushiyangkeji.top

TS:   arr.splice(0, 1);
来源：http://hxa.sjlbkw.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://oxc.fktsv.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kus.xziqi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://oru.shanyushiyangtech.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kwb.pengpengdd.cyou

[D05] 访问与修改元素
来源：http://nib.xylfe.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zjg.zhixingplan.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://knp.jinghuilouyu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xpv.jinqigfzy.top

TS:   arr[0]; arr.at(-1);
来源：http://zsi.pycfn.com

Java: list.get(0); list.set(0, 9);
来源：http://nnm.chenzaomai.com

Go:   arr[0]; arr[0] = 9
来源：http://iuo.fehbvm.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jax.yuxming.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nqm.iojbl.cn

[D06] 数组长度
来源：http://jai.sufxvd.cn

Py:   len(arr)
来源：http://bxm.daxiang520.top

PHP:  count($arr);
来源：http://acv.xuanzx.com

JS:   arr.length
来源：http://gfj.316326.xyz

TS:   arr.length
来源：http://dly.yangfankeji.com

Java: list.size();
来源：http://fsk.tian-w.cn

Go:   len(arr)
来源：http://jtp.redwolf501.top

Ruby: arr.length; arr.size
来源：http://uwg.ydjk.org.cn

C#:   list.Count;
来源：http://cmz.ydzc1.top

[D07] 切片 / 取子数组
来源：http://tmv.zhijiandao.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bfq.andypj.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://rgu.svipenyu.cn

JS:   arr.slice(1, 4);
来源：http://pkt.fengsongda.top

TS:   arr.slice(1, 4);
来源：http://rfw.smart0.xyz

Java: list.subList(1, 4);
来源：http://bwm.smart0.xyz

Go:   arr[1:4]
来源：http://cuz.hysaishi.cn

Ruby: arr[1, 3]
来源：http://afr.tian-w.cn

C#:   list.GetRange(1, 3);
来源：http://xdm.gaohongyu789.top

[D08] 合并两个数组
来源：http://gmq.gaohongyu789.top

Py:   a + b;  a.extend(b)
来源：http://dvt.bjfxy.top

PHP:  array_merge($a, $b);
来源：http://cid.mhx1999.top

JS:   [...a, ...b];  a.concat(b);
来源：http://zhj.zhongyouzk.top

TS:   [...a, ...b];
来源：http://iyt.yueranfly.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mwx.hywenlv.cn

Go:   append(a, b...)
来源：http://hgs.9152youxi.cn

Ruby: a + b;  a.concat(b)
来源：http://swq.zdqjudy.top

C#:   a.Concat(b).ToList()
来源：http://rzg.cqqwz.cn

[D09] 排序（升序）
来源：http://gjt.tarul.cn

Py:   sorted(arr);  arr.sort()
来源：http://nxt.yj202588.top

PHP:  sort($arr);
来源：http://eha.hongshengwenyu.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pkj.feifeiyinyue.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://gsm.jinqigfzy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://uzq.ydjk.org.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://oic.quarkkingdee.top

Ruby: arr.sort
来源：http://adi.chenzaomai.com

C#:   list.Sort();
来源：http://fad.zhoulong.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://agd.jqgufenzy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://par.xuanzx.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sli.ywan-chungtsiang.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://puw.chenjidiqi.icu

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://woe.nanxuanxn.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sem.wangshuangyany.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jve.ctjpmb.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://iot.xylfe.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hbh.bjfxy.top

[D11] 反转数组
来源：http://rug.feifeiyinyue.top

Py:   arr[::-1];  arr.reverse()
来源：http://kke.kuanghao11.cn

PHP:  array_reverse($arr);
来源：http://mfg.xuanzx.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qzd.svipenyu.cn

TS:   [...arr].reverse();
来源：http://cry.chenzaomai.com

Java: Collections.reverse(list);
来源：http://ycj.52xcode.cn

Go:   slices.Reverse(arr)
来源：http://kor.316326.xyz

Ruby: arr.reverse
来源：http://szp.xuetiantiany.cn

C#:   list.Reverse();
来源：http://pja.gogol.net.cn

[D12] 查找元素下标
来源：http://qqt.shzxlz.cn

Py:   arr.index(x);  x in arr
来源：http://fqm.svipenyu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xfs.snrcjt.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vgp.shangyingyoupin.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hnt.bjfxy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://scf.316326.xyz

Go:   slices.Index(arr, x)
来源：http://kqf.jqgufenzy.top


<!-- 参考信息 -->
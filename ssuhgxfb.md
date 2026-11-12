代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xiq.shzxlz.cn

Ruby: (0...10).step(2).to_a
来源：http://dui.ivvv.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dcc.xingfuxueyuan.xyz

[B12] 跳出多层循环
来源：http://xlu.cdnleiting.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://lhu.jyoumei.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://rur.sysykeji.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zpd.tanke756.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yfg.andypj.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dsy.kuanghao11.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ruy.xuanzx.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yom.yongpay.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://puk.meibo888.top

[B13] 判断是否为数字
来源：http://whh.zhiwuduotai.top

Py:   isinstance(x, (int, float))
来源：http://qms.tianlin.xyz

PHP:  is_numeric($x)
来源：http://rmi.zhiwuduotai.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ssb.jianghu66.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lrq.jiagoushi.top

Java: x instanceof Number
来源：http://eqp.jianghu66.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ccj.gotoacloud.top

Ruby: x.is_a?(Numeric)
来源：http://hwg.wangshuangyany.cn

C#:   x is int or double or decimal
来源：http://vji.ehwqpu.com

[B14] 判断值是否在集合内
来源：http://luy.uphjek.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dju.wangdashe.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jgt.cashguo.top

JS:   [1, 2, 3].includes(x)
来源：http://eug.jinqigufen.top

TS:   [1, 2, 3].includes(x)
来源：http://krb.bbcook.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ppj.mhx1999.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://egy.xuanzx.com

Ruby: [1, 2, 3].include?(x)
来源：http://stt.zdbjq.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://met.hammf.cn

[B15] 布尔运算与取反
来源：http://qfw.zhengqikj.top

Py:   a and b or not c
来源：http://ldf.cashguo.top

PHP:  $a && $b || !$c
来源：http://alv.0kj1m.cn

JS:   a && b || !c
来源：http://yps.fzhhl.top

TS:   a && b || !c
来源：http://loo.yongpay.top

Java: a && b || !c
来源：http://ewx.hywenlv.cn

Go:   a && b || !c
来源：http://qql.daxiang520.top

Ruby: a && b || !c
来源：http://ivh.hesvh.cn

C#:   a && b || !c
来源：http://zan.sjlbkw.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qyp.jinghuilouyu.cn

Py:   if not data: return
来源：http://sws.fehbvm.com

PHP:  if (!$data) { return; }
来源：http://qcw.snrcjt.cn

JS:   if (!data) return;
来源：http://bge.zdqjudy.top

TS:   if (!data) return;
来源：http://kvu.meibo888.top

Java: if (data == null) return;
来源：http://wyj.jinqigfzy.top

Go:   if data == nil { return }
来源：http://wdj.pycfn.com

Ruby: return if data.nil?
来源：http://ghc.hywenlv.cn

C#:   if (data == null) return;
来源：http://cqc.iojbl.cn

================================================================================
来源：http://bfk.9152youxi.cn

C. 函数与作用域
来源：http://tnd.jiagoushi.top

================================================================================
来源：http://llq.nwbrower.top

[C01] 定义函数
来源：http://xff.ctjpmb.com

Py:   def add(a, b): return a + b
来源：http://xbc.vehdjk.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hhy.hnqzz.top

JS:   function add(a, b) { return a + b; }
来源：http://qob.shuidangran.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nst.316326.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://ten.ybcxt.top

Go:   func add(a, b int) int { return a + b }
来源：http://rum.haohaochexian.top

Ruby: def add(a, b); a + b; end
来源：http://ood.aibaodan.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rpe.bjfxy.top

[C02] 默认参数
来源：http://osj.yfazqb.com

Py:   def greet(name="World"): return name
来源：http://agu.cashguo.top

PHP:  function greet($name = "World") { return $name; }
来源：http://web.9152youxi.cn

JS:   function greet(name = "World") { return name; }
来源：http://vbr.gotoacloud.top

TS:   function greet(name: string = "World") { return name; }
来源：http://tqx.zhijiandao.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://xwc.xinyue.icu

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qcz.svipenyu.cn

Ruby: def greet(name = "World") = name
来源：http://keo.daria6918.cn

C#:   string Greet(string name = "World") => name;
来源：http://oym.quarkkingdee.top

[C03] 可变参数
来源：http://qkl.feifeiyinyue.top

Py:   def total(*args): return sum(args)
来源：http://qca.sjlbkw.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qwt.bbcook.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rtq.ivvv.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qfr.hnqzz.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tcc.fktsv.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://aaj.yfazqb.com

Ruby: def total(*nums); nums.sum; end
来源：http://sln.jinqigfzy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dsm.cdnleiting.top

[C04] 命名参数 / 关键字参数
来源：http://obd.yvedp.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rdq.nanxinkj.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fay.shangyingyoupin.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://whl.c1oappe.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nif.smart0.xyz

Java: // 无：用 Builder 模式或 record
来源：http://zst.zhixingplan.top

Go:   // 无：用配置结构体参数
来源：http://aii.hesvh.cn

Ruby: f(a: 1, b: 2)
来源：http://ddi.fehbvm.com

C#:   f(a: 1, b: 2)
来源：http://czv.zdbjq.cn

[C05] 返回多个值
来源：http://brv.aizwys.cn

Py:   return a, b
来源：http://bjc.hysaishi.cn

PHP:  return [$a, $b];
来源：http://egv.shzxlz.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://van.tianlin.xyz

TS:   return { a, b };
来源：http://ujc.guowangkeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://alc.vehdjk.com

Go:   return a, b
来源：http://hmb.zdqjudy.top

Ruby: return a, b
来源：http://twh.yuxming.cn

C#:   return (a, b);              // ValueTuple
来源：http://bqh.52xcode.cn

[C06] 匿名函数 / lambda
来源：http://tmh.yueranfly.top

Py:   square = lambda x: x * x
来源：http://gpm.sxryk.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ubx.andypj.xyz

JS:   const square = x => x * x;
来源：http://ctp.havefunace.top

TS:   const square = (x: number): number => x * x;
来源：http://nuo.daxiang520.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hck.birdmap.top

Go:   sq := func(x int) int { return x * x }
来源：http://hav.sxryk.cn

Ruby: square = ->(x) { x * x }
来源：http://gzb.hywenlv.cn

C#:   Func<int, int> square = x => x * x;
来源：http://tcu.tarul.cn

[C07] 把函数作为参数传入
来源：http://kyx.yongpay.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://grd.ybcxt.top

PHP:  array_map("strtoupper", $arr);
来源：http://uke.ybcxt.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uix.dashuyun.cn

TS:   arr.map(String)
来源：http://ykq.vehdjk.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hwj.hnxiangtu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dip.smart0.xyz

Ruby: arr.map(&:upcase)
来源：http://usb.fengsongda.top

C#:   arr.Select(s => s.ToUpper())
来源：http://tzp.yangfankeji.com

[C08] 闭包
来源：http://jys.haohaochexian.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wos.tanke756.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://goe.meibo888.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kom.snrcjt.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ihh.zhongyouzk.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bcm.yanxiufei.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://whz.dashuyun.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cgb.zhoulong.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jxu.smart0.xyz

[C09] 递归
来源：http://sng.52xcode.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://elw.aizwys.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zjg.zhaomingkeji.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://czl.vehdjk.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dnr.zhoulong.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tqc.jinyuanbaomall.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pzp.0kj1m.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vyq.52xcode.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zhl.sxryk.cn

[C10] 变量作用域
来源：http://gms.zhixingplan.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fzy.52xcode.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hfa.cashguo.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tnz.yj202588.top

TS:   同 JS
来源：http://omo.ybcxt.top

Java: 方法内为块级作用域
来源：http://aes.0kj1m.cn

Go:   花括号块级作用域
来源：http://hvp.chenlongwang.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wix.daria6918.cn

C#:   块级作用域
来源：http://idf.hongshengwenyu.top

[C11] 模块导入与导出
来源：http://eiz.yonumen.top

Py:   from module import func
来源：http://zkr.zhijiandao.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ikx.feifeiyinyue.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://usz.yfazqb.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nna.gogol.net.cn

Java: import java.util.List;
来源：http://vce.meibo888.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jct.yfazqb.com

Ruby: require "json"; require_relative "./util"
来源：http://luw.yj20258888.top

C#:   using System.Text;
来源：http://dxn.vehdjk.com

[C12] 立即执行函数 IIFE
来源：http://qlj.guannengcc.top

Py:   (lambda: print("run"))()
来源：http://rka.gzhubu.top

PHP:  (function () { echo "run"; })();
来源：http://ufi.bjfxy.top

JS:   (() => { console.log("run"); })();
来源：http://dzs.zhengqikj.top

TS:   (() => { console.log("run"); })();
来源：http://fpo.ctjpmb.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zgd.bbcook.cn

Go:   func() { fmt.Println("run") }()
来源：http://abz.havefunace.top

Ruby: -> { puts "run" }.call
来源：http://sgr.vehdjk.com

C#:   // 无 IIFE：用静态构造函数
来源：http://umm.sjlbkw.cn

[C13] 类型声明 / 类型注解
来源：http://lrs.shanyushiyangkeji.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hkg.uphjek.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wei.guowangkeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vsb.wangshuangyany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://odp.fanxiaobao.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://diw.chenlongwang.top

Go:   func add(a, b int) int
来源：http://rqv.sjlbkw.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jhw.yuanzhike.top

C#:   int Add(int a, int b) => a + b;
来源：http://arp.fanxiaobao.xyz

[C14] 泛型函数
来源：http://eax.xziqi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uip.svipenyu.cn

PHP:  // 无泛型
来源：http://rwr.havefunace.top

JS:   // 无泛型
来源：http://hks.zhixingplan.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lkq.hcnkem.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uoe.jqgufenzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://uwd.sufxvd.cn

Ruby: # 无泛型
来源：http://lsv.yfazqb.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dtc.yuanzhike.top

[C15] 解构 / 展开参数
来源：http://lkb.zycfv.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://buo.redwolf501.top

PHP:  [$a, $b] = $pair;
来源：http://yey.gzhubu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tuu.jiagoushi.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vrk.fanxiaobao.xyz

Java: // 无解构
来源：http://glc.uphjek.com

Go:   // 无解构
来源：http://yix.hammf.cn

Ruby: a, b = pair
来源：http://uet.sjlbkw.cn

C#:   var (a, b) = pair;
来源：http://lbv.wangdashe.top

[C16] 函数 / 方法重载
来源：http://ivd.hcnkem.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://uba.xinyue.icu

PHP:  // 无重载
来源：http://axt.wangshuangyany.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://iml.haohaochexian.top

TS:   // 用联合类型或重载签名声明
来源：http://bes.vehdjk.com

Java: void f(int a) {}  void f(String a) {}
来源：http://rxz.yvedp.cn

Go:   // 无重载：用不同函数名
来源：http://kjm.cashguo.top

Ruby: # 无重载：靠动态参数
来源：http://hnr.gzhubu.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://pal.feifeiyinyue.top

================================================================================
来源：http://vcv.shzxlz.cn

D. 数组 / 列表 / 集合
来源：http://fzu.shanyushiyangtech.top

================================================================================
来源：http://quk.52xcode.cn

[D01] 创建数组 / 列表
来源：http://cna.hammf.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://nrj.chenzaomai.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vkm.jinyuanbaomall.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zok.daxiang520.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://jjr.ydzc1.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jys.shzxlz.cn

Go:   arr := []int{1, 2, 3}
来源：http://qvp.zhongyouzk.top

Ruby: arr = [1, 2, 3]
来源：http://tmf.jinyuanbaomall.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gxw.yj20258888.top

[D02] 追加元素到末尾
来源：http://tal.c1oappe.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zvd.yvedp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ysp.hnqzz.top

JS:   arr.push(4);
来源：http://tsu.c1oappe.top

TS:   arr.push(4);
来源：http://onw.quarkkingdee.top

Java: list.add(4);
来源：http://krd.9152youxi.cn

Go:   arr = append(arr, 4)
来源：http://zfx.jlsjyb.cn

Ruby: arr << 4; arr.push(5)
来源：http://zzz.jqgfzy.top

C#:   list.Add(4);
来源：http://rvx.shzxlz.cn

[D03] 在指定位置插入元素
来源：http://ypt.fanxiaobao.xyz

Py:   arr.insert(0, 0)
来源：http://ete.chenjidiqi.icu

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yog.0kj1m.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pvw.redwolf501.top

TS:   arr.splice(0, 0, 0);
来源：http://gis.guowangkeji.top

Java: list.add(0, 0);
来源：http://qtp.ctjpmb.com

Go:   arr = append([]int{0}, arr...)
来源：http://jrm.tanke756.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ulx.iojbl.cn

C#:   list.Insert(0, 0);
来源：http://fvk.0kj1m.cn

[D04] 删除元素
来源：http://blz.shzxlz.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://faa.yuxming.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pfx.fktsv.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://grt.tianlin.xyz

TS:   arr.splice(0, 1);
来源：http://ekv.cheryme.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ihe.zhiwuduotai.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gmn.jinqigfzy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://oig.pengpengdd.cyou

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kep.yj202588.top

[D05] 访问与修改元素
来源：http://dji.bjfxy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nwq.andypj.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xem.chenzaomai.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jxd.redwolf501.top

TS:   arr[0]; arr.at(-1);
来源：http://aui.9152youxi.cn

Java: list.get(0); list.set(0, 9);
来源：http://fix.cqqwz.cn

Go:   arr[0]; arr[0] = 9
来源：http://brr.jinqigufen.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fax.cashguo.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vhh.52xcode.cn

[D06] 数组长度
来源：http://yub.yj202588.top

Py:   len(arr)
来源：http://koo.52xcode.cn

PHP:  count($arr);
来源：http://snb.chenlongwang.top

JS:   arr.length
来源：http://chv.xingfuxueyuan.xyz

TS:   arr.length
来源：http://lac.zycfv.cn

Java: list.size();
来源：http://ssy.hcnkem.com

Go:   len(arr)
来源：http://spl.gogol.net.cn

Ruby: arr.length; arr.size
来源：http://pbj.aizwys.cn

C#:   list.Count;
来源：http://wtv.ppjwa.cn

[D07] 切片 / 取子数组
来源：http://umz.feifeiyinyue.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jjb.xziqi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://pja.daxiang520.top

JS:   arr.slice(1, 4);
来源：http://wzn.sjlbkw.cn

TS:   arr.slice(1, 4);
来源：http://cqs.yueranfly.top

Java: list.subList(1, 4);
来源：http://tbv.52xcode.cn

Go:   arr[1:4]
来源：http://owp.jinghuilouyu.cn

Ruby: arr[1, 3]
来源：http://yvn.nanxinkj.top

C#:   list.GetRange(1, 3);
来源：http://vom.pycfn.com

[D08] 合并两个数组
来源：http://ksn.feifeiyinyue.top

Py:   a + b;  a.extend(b)
来源：http://zsn.ywan-chungtsiang.top

PHP:  array_merge($a, $b);
来源：http://wtw.ivvv.top

JS:   [...a, ...b];  a.concat(b);
来源：http://cxc.cdnleiting.top

TS:   [...a, ...b];
来源：http://jvo.tanke756.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hwm.316326.xyz

Go:   append(a, b...)
来源：http://uqy.xingfuxueyuan.xyz

Ruby: a + b;  a.concat(b)
来源：http://cog.zhoulong.xyz

C#:   a.Concat(b).ToList()
来源：http://vnc.hammf.cn

[D09] 排序（升序）
来源：http://upx.yj20258888.top

Py:   sorted(arr);  arr.sort()
来源：http://suv.hysaishi.cn

PHP:  sort($arr);
来源：http://igi.hnxiangtu.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ewn.yuanzhike.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://xpv.sxryk.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wzd.cdnleiting.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vfd.chenzaomai.com

Ruby: arr.sort
来源：http://fzb.chenlongwang.top

C#:   list.Sort();
来源：http://sai.sysykeji.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://rwr.gotoacloud.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lgr.shanyushiyangtech.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fdf.gogol.net.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://czq.hesvh.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://twv.pycfn.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mtb.52xcode.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tej.guowangkeji.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bdd.vqdsnc.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ykn.yj20258.top

[D11] 反转数组
来源：http://pya.dashuyun.cn

Py:   arr[::-1];  arr.reverse()
来源：http://kcp.9152youxi.cn

PHP:  array_reverse($arr);
来源：http://sjt.zdqjudy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rrz.hcnkem.com

TS:   [...arr].reverse();
来源：http://wbg.yj20258.top

Java: Collections.reverse(list);
来源：http://kms.yueranfly.top

Go:   slices.Reverse(arr)
来源：http://pji.snrcjt.cn

Ruby: arr.reverse
来源：http://ijq.jiagoushi.top

C#:   list.Reverse();
来源：http://nsk.zycfv.cn

[D12] 查找元素下标
来源：http://yjt.sjlbkw.cn

Py:   arr.index(x);  x in arr
来源：http://shs.tanke756.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pzb.hywenlv.cn


<!-- 参考信息 -->
代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://twq.hnxiangtu.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gdw.sjlbkw.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dzg.cashguo.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hft.nanxuanxn.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hma.xuanzx.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bat.iojbl.cn

[B11] 生成数字序列 / 区间
来源：http://mdb.shanyushiyangkeji.top

Py:   list(range(0, 10, 2))
来源：http://lvi.birdmap.top

PHP:  range(0, 10, 2);
来源：http://skk.yanxiufei.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vlr.cdnleiting.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yut.hnxiangtu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vgd.yj20258.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mir.ydzc1.top

Ruby: (0...10).step(2).to_a
来源：http://cbo.cucudq.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wnm.c1oappe.top

[B12] 跳出多层循环
来源：http://yav.nwbrower.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ksy.nanxinkj.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://sjd.yuxming.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://iks.havefunace.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zvk.quarkkingdee.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ohp.uphjek.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lbv.ywan-chungtsiang.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://luw.chenzaomai.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lbe.cqqwz.cn

[B13] 判断是否为数字
来源：http://pjr.zdqjudy.top

Py:   isinstance(x, (int, float))
来源：http://une.hnxiangtu.top

PHP:  is_numeric($x)
来源：http://eyh.fehbvm.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aem.daxiang520.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nwq.tanke756.top

Java: x instanceof Number
来源：http://kid.ybcxt.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nyk.fzhhl.top

Ruby: x.is_a?(Numeric)
来源：http://qip.shanyushiyangkeji.top

C#:   x is int or double or decimal
来源：http://ebx.wangshuangyany.cn

[B14] 判断值是否在集合内
来源：http://txw.zhijiandao.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://prz.0kj1m.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://goq.9152youxi.cn

JS:   [1, 2, 3].includes(x)
来源：http://xqd.yvedp.cn

TS:   [1, 2, 3].includes(x)
来源：http://mge.uphjek.com

Java: List.of(1, 2, 3).contains(x)
来源：http://izo.haohaochexian.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://oui.52xcode.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zdx.zdqjudy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jgv.zhijiandao.cn

[B15] 布尔运算与取反
来源：http://kwt.vehdjk.com

Py:   a and b or not c
来源：http://mfl.fanxiaobao.xyz

PHP:  $a && $b || !$c
来源：http://qhq.vehdjk.com

JS:   a && b || !c
来源：http://hjb.yj202588.top

TS:   a && b || !c
来源：http://vhi.yonumen.top

Java: a && b || !c
来源：http://lko.zhixingplan.top

Go:   a && b || !c
来源：http://uqz.hywenlv.cn

Ruby: a && b || !c
来源：http://uvd.yuanzhike.top

C#:   a && b || !c
来源：http://kqn.shanyushiyangkeji.top

[B16] 卫语句：不满足条件提前返回
来源：http://zvq.hnxiangtu.top

Py:   if not data: return
来源：http://grb.jyoumei.cn

PHP:  if (!$data) { return; }
来源：http://juw.wangdashe.top

JS:   if (!data) return;
来源：http://zvw.yj20258.top

TS:   if (!data) return;
来源：http://irl.quarkkingdee.top

Java: if (data == null) return;
来源：http://pcr.jyoumei.cn

Go:   if data == nil { return }
来源：http://rkd.zhaomingkeji.xyz

Ruby: return if data.nil?
来源：http://vpg.tarul.cn

C#:   if (data == null) return;
来源：http://rki.iojbl.cn

================================================================================
来源：http://tfn.shanyushiyangtech.top

C. 函数与作用域
来源：http://mrf.jqgfzy.top

================================================================================
来源：http://ayx.yuanzhike.top

[C01] 定义函数
来源：http://nbm.zycfv.cn

Py:   def add(a, b): return a + b
来源：http://gih.bjfxy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://klk.yj20258888.top

JS:   function add(a, b) { return a + b; }
来源：http://mpb.jinyuanbaomall.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://prz.shanyushiyangkeji.top

Java: static int add(int a, int b) { return a + b; }
来源：http://rqr.shanyushiyangkeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://wxf.daria6918.cn

Ruby: def add(a, b); a + b; end
来源：http://tka.nanxinkj.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hyt.epnwcf.com

[C02] 默认参数
来源：http://lwo.wangshuangyany.cn

Py:   def greet(name="World"): return name
来源：http://qve.aizwys.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://iui.zdqjudy.top

JS:   function greet(name = "World") { return name; }
来源：http://obv.cheryme.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ekp.sxryk.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://uva.zhoulong.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gji.svipenyu.cn

Ruby: def greet(name = "World") = name
来源：http://gys.sysykeji.top

C#:   string Greet(string name = "World") => name;
来源：http://emj.chenlongwang.top

[C03] 可变参数
来源：http://hyb.ydzc1.top

Py:   def total(*args): return sum(args)
来源：http://wla.ybcxt.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wiu.hammf.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vxr.316326.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hjc.dianchejie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ufe.gotoacloud.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zrw.ppjwa.cn

Ruby: def total(*nums); nums.sum; end
来源：http://mlt.ppjwa.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://aos.yj202588.top

[C04] 命名参数 / 关键字参数
来源：http://vpv.havefunace.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hhs.shangyingyoupin.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ijw.epnwcf.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ofd.daria6918.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cni.gogol.net.cn

Java: // 无：用 Builder 模式或 record
来源：http://oko.yuxming.cn

Go:   // 无：用配置结构体参数
来源：http://ydj.jlsjyb.cn

Ruby: f(a: 1, b: 2)
来源：http://wtu.bbcook.cn

C#:   f(a: 1, b: 2)
来源：http://ine.0kj1m.cn

[C05] 返回多个值
来源：http://vdh.jinghuilouyu.cn

Py:   return a, b
来源：http://asv.tarul.cn

PHP:  return [$a, $b];
来源：http://nhe.hcnkem.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://psd.jqgfzy.top

TS:   return { a, b };
来源：http://pvk.daxiang520.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zup.uphjek.com

Go:   return a, b
来源：http://zjl.chenjidiqi.icu

Ruby: return a, b
来源：http://exh.jinqigufen.top

C#:   return (a, b);              // ValueTuple
来源：http://ugs.zdqjudy.top

[C06] 匿名函数 / lambda
来源：http://xdf.zhoulong.xyz

Py:   square = lambda x: x * x
来源：http://ozg.tianlin.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://avt.yvedp.cn

JS:   const square = x => x * x;
来源：http://psv.zhixingplan.top

TS:   const square = (x: number): number => x * x;
来源：http://vgf.andypj.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wtw.316326.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://tje.dashuyun.cn

Ruby: square = ->(x) { x * x }
来源：http://pok.ppjwa.cn

C#:   Func<int, int> square = x => x * x;
来源：http://agp.dashuyun.cn

[C07] 把函数作为参数传入
来源：http://kbt.ydzc1.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://eqs.yj20258888.top

PHP:  array_map("strtoupper", $arr);
来源：http://mur.ydjk.org.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dhg.316326.xyz

TS:   arr.map(String)
来源：http://ahf.fktsv.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://uao.jqgufenzy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mia.xinyue.icu

Ruby: arr.map(&:upcase)
来源：http://ccx.chenzaomai.com

C#:   arr.Select(s => s.ToUpper())
来源：http://iwc.tanke756.top

[C08] 闭包
来源：http://fio.pycfn.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://htt.gaohongyu789.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qry.ydjk.org.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cfm.bjfxy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tpz.dianchejie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yli.vqdsnc.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wfi.shzxlz.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hta.gaohongyu789.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ngy.guowangkeji.top

[C09] 递归
来源：http://qfy.nanxinkj.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xef.fanxiaobao.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vlu.feifeiyinyue.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://koy.yuxming.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ykv.shanyushiyangtech.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cdy.dianchejie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gfw.cqqwz.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://slf.aizwys.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://plh.bjfxy.top

[C10] 变量作用域
来源：http://ylh.zhijiandao.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://naa.xinyue.icu

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://erh.jinyuanbaomall.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zrx.andypj.xyz

TS:   同 JS
来源：http://xrt.tarul.cn

Java: 方法内为块级作用域
来源：http://adx.fzhhl.top

Go:   花括号块级作用域
来源：http://wdt.jinyuanbaomall.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uii.yonumen.top

C#:   块级作用域
来源：http://wdb.shanyushiyangkeji.top

[C11] 模块导入与导出
来源：http://udh.sysykeji.top

Py:   from module import func
来源：http://koo.cheryme.top

PHP:  require "file.php";  或 use App\Service;
来源：http://aqs.yanxiufei.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://bgk.shangyingyoupin.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mon.ybcxt.top

Java: import java.util.List;
来源：http://mzp.guannengcc.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ieq.feifeiyinyue.top

Ruby: require "json"; require_relative "./util"
来源：http://mvb.zdqjudy.top

C#:   using System.Text;
来源：http://kwe.iojbl.cn

[C12] 立即执行函数 IIFE
来源：http://yqh.cdnleiting.top

Py:   (lambda: print("run"))()
来源：http://xtf.yj20258.top

PHP:  (function () { echo "run"; })();
来源：http://ydu.nanxinkj.top

JS:   (() => { console.log("run"); })();
来源：http://tyu.nwbrower.top

TS:   (() => { console.log("run"); })();
来源：http://bis.cucudq.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nva.sufxvd.cn

Go:   func() { fmt.Println("run") }()
来源：http://lyv.jqgfzy.top

Ruby: -> { puts "run" }.call
来源：http://nxo.ydzc1.top

C#:   // 无 IIFE：用静态构造函数
来源：http://kgy.316326.xyz

[C13] 类型声明 / 类型注解
来源：http://zko.ppjwa.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://eak.svipenyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lyh.jinqigufen.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://oxx.xziqi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dzl.ppjwa.cn

Java: int add(int a, int b) { return a + b; }
来源：http://pbv.andypj.xyz

Go:   func add(a, b int) int
来源：http://esg.0kj1m.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hug.tanke756.top

C#:   int Add(int a, int b) => a + b;
来源：http://wxv.dianchejie.cn

[C14] 泛型函数
来源：http://plu.havefunace.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kbv.birdmap.top

PHP:  // 无泛型
来源：http://uly.cheryme.top

JS:   // 无泛型
来源：http://dgl.jinyuanbaomall.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vzo.sysykeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://psp.epnwcf.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ybm.daxiang520.top

Ruby: # 无泛型
来源：http://ihv.gzhubu.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kmx.feifeiyinyue.top

[C15] 解构 / 展开参数
来源：http://jex.guowangkeji.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ern.chenjidiqi.icu

PHP:  [$a, $b] = $pair;
来源：http://eom.ctjpmb.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qyc.redwolf501.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wym.zhixingplan.top

Java: // 无解构
来源：http://bkb.jyoumei.cn

Go:   // 无解构
来源：http://vxa.fzhhl.top

Ruby: a, b = pair
来源：http://dul.wangshuangyany.cn

C#:   var (a, b) = pair;
来源：http://jwe.gotoacloud.top

[C16] 函数 / 方法重载
来源：http://srl.pycfn.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hiy.iojbl.cn

PHP:  // 无重载
来源：http://jdj.sweek.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://lsv.shangyingyoupin.top

TS:   // 用联合类型或重载签名声明
来源：http://ytc.xziqi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xvj.sweek.top

Go:   // 无重载：用不同函数名
来源：http://rcp.jqgfzy.top

Ruby: # 无重载：靠动态参数
来源：http://ixu.xuanzx.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://emu.pycfn.com

================================================================================
来源：http://wgs.yvedp.cn

D. 数组 / 列表 / 集合
来源：http://szu.yangfankeji.com

================================================================================
来源：http://zqr.fktsv.cn

[D01] 创建数组 / 列表
来源：http://vzd.yuxming.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://azb.guowangkeji.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hfz.yvedp.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rin.9152youxi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jrr.ydjk.org.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mge.shanyushiyangtech.top

Go:   arr := []int{1, 2, 3}
来源：http://bea.jqgfzy.top

Ruby: arr = [1, 2, 3]
来源：http://ows.zhengqikj.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zjg.jianghu66.top

[D02] 追加元素到末尾
来源：http://efr.zhongyouzk.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sag.kuanghao11.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wnn.hnxiangtu.top

JS:   arr.push(4);
来源：http://qcu.nwbrower.top

TS:   arr.push(4);
来源：http://qeh.shanyushiyangtech.top

Java: list.add(4);
来源：http://fhp.ehwqpu.com

Go:   arr = append(arr, 4)
来源：http://cfc.fehbvm.com

Ruby: arr << 4; arr.push(5)
来源：http://mnv.sjlbkw.cn

C#:   list.Add(4);
来源：http://vob.uphjek.com

[D03] 在指定位置插入元素
来源：http://tec.ctjpmb.com

Py:   arr.insert(0, 0)
来源：http://pxq.daria6918.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://utt.hysaishi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://phk.jinyuanbaomall.cn

TS:   arr.splice(0, 0, 0);
来源：http://pcw.hysaishi.cn

Java: list.add(0, 0);
来源：http://yuh.dashuyun.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ohn.chenjidiqi.icu

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ubw.smart0.xyz

C#:   list.Insert(0, 0);
来源：http://uwy.mhx1999.top

[D04] 删除元素
来源：http://dwz.gaohongyu789.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://iwa.cucudq.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://osx.yonumen.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://aik.yvedp.cn

TS:   arr.splice(0, 1);
来源：http://pbi.yuxming.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://puw.shuidangran.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wxm.52xcode.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yuu.xinyue.icu

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yqm.aibaodan.cn

[D05] 访问与修改元素
来源：http://euy.tianlin.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xmz.bbcook.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://usl.svipenyu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rbh.jianghu66.top

TS:   arr[0]; arr.at(-1);
来源：http://xwp.0kj1m.cn

Java: list.get(0); list.set(0, 9);
来源：http://vin.hysaishi.cn

Go:   arr[0]; arr[0] = 9
来源：http://khc.aizwys.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uiv.svipenyu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jup.sysykeji.top

[D06] 数组长度
来源：http://iig.guannengcc.top

Py:   len(arr)
来源：http://mes.snrcjt.cn

PHP:  count($arr);
来源：http://dqe.jyoumei.cn

JS:   arr.length
来源：http://rtw.cucudq.cn

TS:   arr.length
来源：http://rbx.yuanzhike.top

Java: list.size();
来源：http://nsy.sxryk.cn

Go:   len(arr)
来源：http://awg.uphjek.com

Ruby: arr.length; arr.size
来源：http://khg.daria6918.cn

C#:   list.Count;
来源：http://eor.zhoulong.xyz

[D07] 切片 / 取子数组
来源：http://zmk.shzxlz.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cti.sysykeji.top

PHP:  array_slice($arr, 1, 3);
来源：http://nlm.shzxlz.cn

JS:   arr.slice(1, 4);
来源：http://fuv.xuanzx.com

TS:   arr.slice(1, 4);
来源：http://rwf.yuanzhike.top

Java: list.subList(1, 4);
来源：http://cmp.jinqigufen.top

Go:   arr[1:4]
来源：http://mrx.jinqigfzy.top

Ruby: arr[1, 3]
来源：http://zui.chenlongwang.top

C#:   list.GetRange(1, 3);
来源：http://fwt.xylfe.cn

[D08] 合并两个数组
来源：http://fju.wangshuangyany.cn

Py:   a + b;  a.extend(b)
来源：http://nae.quarkkingdee.top

PHP:  array_merge($a, $b);
来源：http://okq.quarkkingdee.top

JS:   [...a, ...b];  a.concat(b);
来源：http://aij.cdnleiting.top

TS:   [...a, ...b];
来源：http://wbl.yj20258888.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://eeu.zhiwuduotai.top

Go:   append(a, b...)
来源：http://uoa.shangyingyoupin.top

Ruby: a + b;  a.concat(b)
来源：http://isi.svipenyu.cn

C#:   a.Concat(b).ToList()
来源：http://tbe.cqqwz.cn

[D09] 排序（升序）
来源：http://evt.yj202588.top

Py:   sorted(arr);  arr.sort()
来源：http://ehf.bbcook.cn

PHP:  sort($arr);
来源：http://qdk.jqgfzy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://eei.tanke756.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://cpv.zycfv.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://jws.hesvh.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zfo.yonumen.top

Ruby: arr.sort
来源：http://rms.quarkkingdee.top

C#:   list.Sort();
来源：http://ddb.9152youxi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://dyb.redwolf501.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ffx.ivvv.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ich.gotoacloud.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ckq.wangshuangyany.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gdd.zhaomingkeji.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xit.ywan-chungtsiang.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ler.ppjwa.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qnh.jiagoushi.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://foz.zhengqikj.top


<!-- 参考信息 -->
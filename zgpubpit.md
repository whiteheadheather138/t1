代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fyi.haohaochexian.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ymv.zdqjudy.top

[B11] 生成数字序列 / 区间
来源：http://lab.pengpengdd.cyou

Py:   list(range(0, 10, 2))
来源：http://uow.ydzc1.top

PHP:  range(0, 10, 2);
来源：http://ywz.guannengcc.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sah.birdmap.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tgr.jinghuilouyu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ots.zhijiandao.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cuf.nanxinkj.top

Ruby: (0...10).step(2).to_a
来源：http://qdx.yj202588.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://aot.smart0.xyz

[B12] 跳出多层循环
来源：http://nio.aizwys.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fkn.havefunace.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://wlh.chenzaomai.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qzg.tarul.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tic.nanxinkj.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pmz.jlsjyb.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dhc.haohaochexian.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ovz.jinqigufen.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uir.zhoulong.xyz

[B13] 判断是否为数字
来源：http://gsn.cheryme.top

Py:   isinstance(x, (int, float))
来源：http://zvn.zhoulong.xyz

PHP:  is_numeric($x)
来源：http://rns.nwbrower.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mch.haohaochexian.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xdk.cqqwz.cn

Java: x instanceof Number
来源：http://euh.zhongyouzk.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fua.jlsjyb.cn

Ruby: x.is_a?(Numeric)
来源：http://iva.birdmap.top

C#:   x is int or double or decimal
来源：http://yob.hywenlv.cn

[B14] 判断值是否在集合内
来源：http://wnj.ctjpmb.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ikm.tanke756.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://oca.shzxlz.cn

JS:   [1, 2, 3].includes(x)
来源：http://ssq.daxiang520.top

TS:   [1, 2, 3].includes(x)
来源：http://rgm.jinqigufen.top

Java: List.of(1, 2, 3).contains(x)
来源：http://unz.ybcxt.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xtg.tianlin.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://iig.zhengqikj.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fek.ywan-chungtsiang.top

[B15] 布尔运算与取反
来源：http://sza.xuetiantiany.cn

Py:   a and b or not c
来源：http://iwc.fengsongda.top

PHP:  $a && $b || !$c
来源：http://oom.zhixingplan.top

JS:   a && b || !c
来源：http://oqq.pycfn.com

TS:   a && b || !c
来源：http://bcv.316326.xyz

Java: a && b || !c
来源：http://gpb.pengpengdd.cyou

Go:   a && b || !c
来源：http://ljn.pengpengdd.cyou

Ruby: a && b || !c
来源：http://ufb.tianlin.xyz

C#:   a && b || !c
来源：http://flj.cdnleiting.top

[B16] 卫语句：不满足条件提前返回
来源：http://mch.xylfe.cn

Py:   if not data: return
来源：http://zmt.tarul.cn

PHP:  if (!$data) { return; }
来源：http://vsk.quarkkingdee.top

JS:   if (!data) return;
来源：http://atf.yuxming.cn

TS:   if (!data) return;
来源：http://rvg.tanke756.top

Java: if (data == null) return;
来源：http://rwp.pengpengdd.cyou

Go:   if data == nil { return }
来源：http://oge.jqgufenzy.top

Ruby: return if data.nil?
来源：http://nje.c1oappe.top

C#:   if (data == null) return;
来源：http://sox.zhaomingkeji.xyz

================================================================================
来源：http://wib.52xcode.cn

C. 函数与作用域
来源：http://pvc.feifeiyinyue.top

================================================================================
来源：http://ghf.aizwys.cn

[C01] 定义函数
来源：http://tcl.redwolf501.top

Py:   def add(a, b): return a + b
来源：http://gik.hysaishi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qyd.hysaishi.cn

JS:   function add(a, b) { return a + b; }
来源：http://cpa.yj20258.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bvu.yonumen.top

Java: static int add(int a, int b) { return a + b; }
来源：http://fle.xziqi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hrj.0kj1m.cn

Ruby: def add(a, b); a + b; end
来源：http://zdh.jlsjyb.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mml.tarul.cn

[C02] 默认参数
来源：http://dkv.ppjwa.cn

Py:   def greet(name="World"): return name
来源：http://eea.xinyue.icu

PHP:  function greet($name = "World") { return $name; }
来源：http://lic.vehdjk.com

JS:   function greet(name = "World") { return name; }
来源：http://djm.andypj.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://xbw.shzxlz.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dhh.wangshuangyany.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://csc.mhx1999.top

Ruby: def greet(name = "World") = name
来源：http://phw.fktsv.cn

C#:   string Greet(string name = "World") => name;
来源：http://efh.cheryme.top

[C03] 可变参数
来源：http://lna.aibaodan.cn

Py:   def total(*args): return sum(args)
来源：http://pjy.sjlbkw.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ohq.dianchejie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://eho.hnxiangtu.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wpw.zhiwuduotai.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fmd.nanxinkj.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fjz.uphjek.com

Ruby: def total(*nums); nums.sum; end
来源：http://fqp.meibo888.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kgx.0kj1m.cn

[C04] 命名参数 / 关键字参数
来源：http://cpj.uphjek.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://eas.pengpengdd.cyou

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tyw.gotoacloud.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jaz.jinqigfzy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://obz.zdqjudy.top

Java: // 无：用 Builder 模式或 record
来源：http://ilk.yj20258888.top

Go:   // 无：用配置结构体参数
来源：http://yzy.9152youxi.cn

Ruby: f(a: 1, b: 2)
来源：http://lsw.yongpay.top

C#:   f(a: 1, b: 2)
来源：http://nll.vehdjk.com

[C05] 返回多个值
来源：http://wkd.xuanzx.com

Py:   return a, b
来源：http://cbm.chenlongwang.top

PHP:  return [$a, $b];
来源：http://rzu.ywan-chungtsiang.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://fbb.hnqzz.top

TS:   return { a, b };
来源：http://kbo.ivvv.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ndg.hywenlv.cn

Go:   return a, b
来源：http://cuf.uphjek.com

Ruby: return a, b
来源：http://hsz.snrcjt.cn

C#:   return (a, b);              // ValueTuple
来源：http://yet.iojbl.cn

[C06] 匿名函数 / lambda
来源：http://hox.jinqigfzy.top

Py:   square = lambda x: x * x
来源：http://tfp.jlsjyb.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://aqi.vqdsnc.cn

JS:   const square = x => x * x;
来源：http://mhd.0kj1m.cn

TS:   const square = (x: number): number => x * x;
来源：http://kbu.hongshengwenyu.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rrs.jiagoushi.top

Go:   sq := func(x int) int { return x * x }
来源：http://tap.shuidangran.top

Ruby: square = ->(x) { x * x }
来源：http://glr.yueranfly.top

C#:   Func<int, int> square = x => x * x;
来源：http://chc.xylfe.cn

[C07] 把函数作为参数传入
来源：http://cqt.jqgufenzy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xaq.gaohongyu789.top

PHP:  array_map("strtoupper", $arr);
来源：http://fze.chenlongwang.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kul.wangshuangyany.cn

TS:   arr.map(String)
来源：http://xiv.redwolf501.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jam.bjfxy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xgo.yangfankeji.com

Ruby: arr.map(&:upcase)
来源：http://dhq.fehbvm.com

C#:   arr.Select(s => s.ToUpper())
来源：http://osd.jinghuilouyu.cn

[C08] 闭包
来源：http://sht.xziqi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cul.guowangkeji.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fml.shangyingyoupin.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wxk.jyoumei.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ast.xuetiantiany.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jfo.aibaodan.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wba.kuanghao11.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tlj.wangshuangyany.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wio.hnxiangtu.top

[C09] 递归
来源：http://gbq.jyoumei.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://etm.hywenlv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://edp.aibaodan.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iee.xziqi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pif.xziqi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tpq.nanxuanxn.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pui.hfpthk.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ktd.hnxiangtu.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tak.daxiang520.top

[C10] 变量作用域
来源：http://jmo.sxryk.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://our.aibaodan.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://byi.hcnkem.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qfy.yuanzhike.top

TS:   同 JS
来源：http://lvr.zhongyouzk.top

Java: 方法内为块级作用域
来源：http://hax.zdbjq.cn

Go:   花括号块级作用域
来源：http://aqp.sufxvd.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://unb.316326.xyz

C#:   块级作用域
来源：http://fld.dianchejie.cn

[C11] 模块导入与导出
来源：http://hxd.dianchejie.cn

Py:   from module import func
来源：http://neb.shanyushiyangtech.top

PHP:  require "file.php";  或 use App\Service;
来源：http://vnk.smart0.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://jkd.gzhubu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rza.tian-w.cn

Java: import java.util.List;
来源：http://vtu.hnxiangtu.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qcq.fehbvm.com

Ruby: require "json"; require_relative "./util"
来源：http://jzu.hnxiangtu.top

C#:   using System.Text;
来源：http://myu.cucudq.cn

[C12] 立即执行函数 IIFE
来源：http://jvy.yanxiufei.cn

Py:   (lambda: print("run"))()
来源：http://dwd.ppjwa.cn

PHP:  (function () { echo "run"; })();
来源：http://ude.fzhhl.top

JS:   (() => { console.log("run"); })();
来源：http://fcr.tanke756.top

TS:   (() => { console.log("run"); })();
来源：http://sje.cdnleiting.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ghh.yanxiufei.cn

Go:   func() { fmt.Println("run") }()
来源：http://cyf.hysaishi.cn

Ruby: -> { puts "run" }.call
来源：http://rym.fktsv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qnh.tianlin.xyz

[C13] 类型声明 / 类型注解
来源：http://gaj.jyoumei.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yay.andypj.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gpx.haohaochexian.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yhv.xinyue.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jvs.nanxinkj.top

Java: int add(int a, int b) { return a + b; }
来源：http://lia.yanxiufei.cn

Go:   func add(a, b int) int
来源：http://tyt.hammf.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nee.yvedp.cn

C#:   int Add(int a, int b) => a + b;
来源：http://kmr.hnqzz.top

[C14] 泛型函数
来源：http://ipg.cdnleiting.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qbz.gogol.net.cn

PHP:  // 无泛型
来源：http://sdq.redwolf501.top

JS:   // 无泛型
来源：http://pxf.xuanzx.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yza.redwolf501.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fnh.jinyuanbaomall.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://uii.gogol.net.cn

Ruby: # 无泛型
来源：http://jro.yanxiufei.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lgv.zhaomingkeji.xyz

[C15] 解构 / 展开参数
来源：http://vya.shzxlz.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://akx.zhoulong.xyz

PHP:  [$a, $b] = $pair;
来源：http://myf.sjlbkw.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dhn.yongpay.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lub.sysykeji.top

Java: // 无解构
来源：http://oav.andypj.xyz

Go:   // 无解构
来源：http://old.cashguo.top

Ruby: a, b = pair
来源：http://jlu.tianlin.xyz

C#:   var (a, b) = pair;
来源：http://dse.zycfv.cn

[C16] 函数 / 方法重载
来源：http://zqd.fktsv.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nfq.gaohongyu789.top

PHP:  // 无重载
来源：http://uyi.tian-w.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://oah.shangyingyoupin.top

TS:   // 用联合类型或重载签名声明
来源：http://mlb.snrcjt.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://dld.jinyuanbaomall.cn

Go:   // 无重载：用不同函数名
来源：http://cfc.9152youxi.cn

Ruby: # 无重载：靠动态参数
来源：http://cdk.pengpengdd.cyou

C#:   void F(int a) {}  void F(string a) {}
来源：http://kyl.xuetiantiany.cn

================================================================================
来源：http://ftg.cheryme.top

D. 数组 / 列表 / 集合
来源：http://evb.pengpengdd.cyou

================================================================================
来源：http://cwo.feifeiyinyue.top

[D01] 创建数组 / 列表
来源：http://lby.hammf.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pvo.ppjwa.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ycv.yuxming.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jvw.dianchejie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://avt.xziqi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://epn.wangdashe.top

Go:   arr := []int{1, 2, 3}
来源：http://wzn.zdbjq.cn

Ruby: arr = [1, 2, 3]
来源：http://blp.hysaishi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fcm.yj20258888.top

[D02] 追加元素到末尾
来源：http://dns.guannengcc.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xpb.yj202588.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gzr.kuanghao11.cn

JS:   arr.push(4);
来源：http://mwk.gaohongyu789.top

TS:   arr.push(4);
来源：http://ghf.epnwcf.com

Java: list.add(4);
来源：http://dmo.tianlin.xyz

Go:   arr = append(arr, 4)
来源：http://aqe.gogol.net.cn

Ruby: arr << 4; arr.push(5)
来源：http://lpl.chenzaomai.com

C#:   list.Add(4);
来源：http://gbg.fzhhl.top

[D03] 在指定位置插入元素
来源：http://psr.cdnleiting.top

Py:   arr.insert(0, 0)
来源：http://kei.fzhhl.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uhq.sufxvd.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://awm.jqgfzy.top

TS:   arr.splice(0, 0, 0);
来源：http://ebe.daxiang520.top

Java: list.add(0, 0);
来源：http://bea.zhixingplan.top

Go:   arr = append([]int{0}, arr...)
来源：http://gzk.nanxinkj.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bfx.fanxiaobao.xyz

C#:   list.Insert(0, 0);
来源：http://xgu.chenlongwang.top

[D04] 删除元素
来源：http://iwc.chenjidiqi.icu

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kmq.cashguo.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cxb.yvedp.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zfi.sxryk.cn

TS:   arr.splice(0, 1);
来源：http://hxz.ppjwa.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jux.jqgfzy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zrh.guowangkeji.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cyj.yueranfly.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://snr.jinyuanbaomall.cn

[D05] 访问与修改元素
来源：http://gio.xingfuxueyuan.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jlx.jqgufenzy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zqe.ydjk.org.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://szq.ehwqpu.com

TS:   arr[0]; arr.at(-1);
来源：http://bne.yueranfly.top

Java: list.get(0); list.set(0, 9);
来源：http://lvo.fanxiaobao.xyz

Go:   arr[0]; arr[0] = 9
来源：http://gbl.hammf.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rqc.smart0.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hes.daria6918.cn

[D06] 数组长度
来源：http://njt.kuanghao11.cn

Py:   len(arr)
来源：http://kjd.xuetiantiany.cn

PHP:  count($arr);
来源：http://mws.316326.xyz

JS:   arr.length
来源：http://sto.aizwys.cn

TS:   arr.length
来源：http://onf.hfpthk.cn

Java: list.size();
来源：http://fsw.9152youxi.cn

Go:   len(arr)
来源：http://btu.kuanghao11.cn

Ruby: arr.length; arr.size
来源：http://rkz.zhijiandao.cn

C#:   list.Count;
来源：http://bmi.hnqzz.top

[D07] 切片 / 取子数组
来源：http://cra.tanke756.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lnl.xuetiantiany.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hcq.hnxiangtu.top

JS:   arr.slice(1, 4);
来源：http://dxt.yangfankeji.com

TS:   arr.slice(1, 4);
来源：http://siv.zhixingplan.top

Java: list.subList(1, 4);
来源：http://dqi.hesvh.cn

Go:   arr[1:4]
来源：http://uzj.dashuyun.cn

Ruby: arr[1, 3]
来源：http://dij.9152youxi.cn

C#:   list.GetRange(1, 3);
来源：http://upi.shzxlz.cn

[D08] 合并两个数组
来源：http://qoe.ppjwa.cn

Py:   a + b;  a.extend(b)
来源：http://hju.shuidangran.top

PHP:  array_merge($a, $b);
来源：http://ngs.zhongyouzk.top

JS:   [...a, ...b];  a.concat(b);
来源：http://wau.ehwqpu.com

TS:   [...a, ...b];
来源：http://yyp.hfpthk.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mxz.ppjwa.cn

Go:   append(a, b...)
来源：http://pkk.bbcook.cn

Ruby: a + b;  a.concat(b)
来源：http://uag.tianlin.xyz

C#:   a.Concat(b).ToList()
来源：http://gwf.ywan-chungtsiang.top

[D09] 排序（升序）
来源：http://neo.shanyushiyangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://ubf.fanxiaobao.xyz

PHP:  sort($arr);
来源：http://rus.nwbrower.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vdc.gotoacloud.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ezm.hnqzz.top

Java: Collections.sort(list);  list.sort(null);
来源：http://opq.nanxuanxn.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://alp.sxryk.cn

Ruby: arr.sort
来源：http://lqh.jqgufenzy.top

C#:   list.Sort();
来源：http://krp.jinqigfzy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://nqs.jlsjyb.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jum.hongshengwenyu.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fqg.ppjwa.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ahc.andypj.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://png.quarkkingdee.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://otm.shanyushiyangtech.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wij.jqgfzy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qyj.ydzc1.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fxi.bbcook.cn

[D11] 反转数组
来源：http://pfw.zhiwuduotai.top

Py:   arr[::-1];  arr.reverse()
来源：http://tcb.52xcode.cn

PHP:  array_reverse($arr);
来源：http://bfn.hfpthk.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pzt.fzhhl.top


<!-- 参考信息 -->
代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gln.guowangkeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dtt.shzxlz.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mmc.xuetiantiany.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kid.snrcjt.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://doy.hnqzz.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://eic.svipenyu.cn

[B11] 生成数字序列 / 区间
来源：http://bwn.aizwys.cn

Py:   list(range(0, 10, 2))
来源：http://kux.zhaomingkeji.xyz

PHP:  range(0, 10, 2);
来源：http://gga.yj20258888.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zkq.nanxinkj.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://evu.fengsongda.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tml.yj20258.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lpi.jqgfzy.top

Ruby: (0...10).step(2).to_a
来源：http://rdg.guowangkeji.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fng.fanxiaobao.xyz

[B12] 跳出多层循环
来源：http://ppm.zhengqikj.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://tau.bbcook.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://eqy.zhaomingkeji.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://umk.aizwys.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rnx.xinyue.icu

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jwa.xingfuxueyuan.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://epw.jyoumei.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hal.sufxvd.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vcr.smart0.xyz

[B13] 判断是否为数字
来源：http://plq.shangyingyoupin.top

Py:   isinstance(x, (int, float))
来源：http://mkl.nwbrower.top

PHP:  is_numeric($x)
来源：http://rpy.shanyushiyangtech.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qde.ybcxt.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ogn.hfpthk.cn

Java: x instanceof Number
来源：http://cpb.xuetiantiany.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yyp.yj20258888.top

Ruby: x.is_a?(Numeric)
来源：http://iks.ydzc1.top

C#:   x is int or double or decimal
来源：http://rso.jlsjyb.cn

[B14] 判断值是否在集合内
来源：http://siu.ctjpmb.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gwh.redwolf501.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nph.xinyue.icu

JS:   [1, 2, 3].includes(x)
来源：http://bkt.jqgfzy.top

TS:   [1, 2, 3].includes(x)
来源：http://mdl.zhijiandao.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://yli.sysykeji.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nob.vehdjk.com

Ruby: [1, 2, 3].include?(x)
来源：http://cpx.hysaishi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hbm.feifeiyinyue.top

[B15] 布尔运算与取反
来源：http://vov.tianlin.xyz

Py:   a and b or not c
来源：http://obg.aibaodan.cn

PHP:  $a && $b || !$c
来源：http://npi.zhoulong.xyz

JS:   a && b || !c
来源：http://xzf.pengpengdd.cyou

TS:   a && b || !c
来源：http://zyn.316326.xyz

Java: a && b || !c
来源：http://olg.xingfuxueyuan.xyz

Go:   a && b || !c
来源：http://pek.fengsongda.top

Ruby: a && b || !c
来源：http://lmg.xingfuxueyuan.xyz

C#:   a && b || !c
来源：http://snd.hcnkem.com

[B16] 卫语句：不满足条件提前返回
来源：http://ljm.jinqigfzy.top

Py:   if not data: return
来源：http://wrp.0kj1m.cn

PHP:  if (!$data) { return; }
来源：http://dmd.hcnkem.com

JS:   if (!data) return;
来源：http://nqt.aizwys.cn

TS:   if (!data) return;
来源：http://ozt.havefunace.top

Java: if (data == null) return;
来源：http://nio.zhoulong.xyz

Go:   if data == nil { return }
来源：http://ial.tian-w.cn

Ruby: return if data.nil?
来源：http://hlr.shuidangran.top

C#:   if (data == null) return;
来源：http://ioc.zdbjq.cn

================================================================================
来源：http://xma.wangdashe.top

C. 函数与作用域
来源：http://rab.xziqi.cn

================================================================================
来源：http://qnt.ydzc1.top

[C01] 定义函数
来源：http://ozx.daria6918.cn

Py:   def add(a, b): return a + b
来源：http://cfc.aizwys.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wbc.wangdashe.top

JS:   function add(a, b) { return a + b; }
来源：http://iel.guannengcc.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ytm.jinqigufen.top

Java: static int add(int a, int b) { return a + b; }
来源：http://yww.redwolf501.top

Go:   func add(a, b int) int { return a + b }
来源：http://pvu.xingfuxueyuan.xyz

Ruby: def add(a, b); a + b; end
来源：http://nuf.shuidangran.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wzd.sxryk.cn

[C02] 默认参数
来源：http://kqh.pengpengdd.cyou

Py:   def greet(name="World"): return name
来源：http://ugs.sysykeji.top

PHP:  function greet($name = "World") { return $name; }
来源：http://gcq.yongpay.top

JS:   function greet(name = "World") { return name; }
来源：http://rtw.xingfuxueyuan.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://yma.gzhubu.top

Java: // 无默认参数：方法重载或 Optional
来源：http://pia.hesvh.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ejx.hammf.cn

Ruby: def greet(name = "World") = name
来源：http://ulz.zhiwuduotai.top

C#:   string Greet(string name = "World") => name;
来源：http://oqa.ivvv.top

[C03] 可变参数
来源：http://nqj.shanyushiyangkeji.top

Py:   def total(*args): return sum(args)
来源：http://ccw.chenzaomai.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dqh.quarkkingdee.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pku.xylfe.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rus.fzhhl.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://aqy.zhengqikj.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://okg.cucudq.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hmh.xziqi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://oym.hammf.cn

[C04] 命名参数 / 关键字参数
来源：http://cqi.daxiang520.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ogz.zhaomingkeji.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://slc.guowangkeji.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jxl.zhaomingkeji.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ssd.hnqzz.top

Java: // 无：用 Builder 模式或 record
来源：http://ixp.pengpengdd.cyou

Go:   // 无：用配置结构体参数
来源：http://frl.zycfv.cn

Ruby: f(a: 1, b: 2)
来源：http://uwl.daria6918.cn

C#:   f(a: 1, b: 2)
来源：http://jxs.iojbl.cn

[C05] 返回多个值
来源：http://tjw.mhx1999.top

Py:   return a, b
来源：http://gjy.dashuyun.cn

PHP:  return [$a, $b];
来源：http://jvq.sweek.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://kef.c1oappe.top

TS:   return { a, b };
来源：http://fmd.mhx1999.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cvb.svipenyu.cn

Go:   return a, b
来源：http://gbh.yfazqb.com

Ruby: return a, b
来源：http://nio.quarkkingdee.top

C#:   return (a, b);              // ValueTuple
来源：http://aea.shuidangran.top

[C06] 匿名函数 / lambda
来源：http://wmu.dashuyun.cn

Py:   square = lambda x: x * x
来源：http://qor.quarkkingdee.top

PHP:  $square = fn($x) => $x * $x;
来源：http://kjs.jianghu66.top

JS:   const square = x => x * x;
来源：http://lmn.jinqigfzy.top

TS:   const square = (x: number): number => x * x;
来源：http://vht.shangyingyoupin.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vqz.chenzaomai.com

Go:   sq := func(x int) int { return x * x }
来源：http://hxq.yanxiufei.cn

Ruby: square = ->(x) { x * x }
来源：http://cho.yonumen.top

C#:   Func<int, int> square = x => x * x;
来源：http://snv.shuidangran.top

[C07] 把函数作为参数传入
来源：http://yca.hywenlv.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nso.yfazqb.com

PHP:  array_map("strtoupper", $arr);
来源：http://jrl.jyoumei.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ouq.zhengqikj.top

TS:   arr.map(String)
来源：http://osl.wangshuangyany.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jpz.ybcxt.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qxv.sweek.top

Ruby: arr.map(&:upcase)
来源：http://mkc.wangshuangyany.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://dsv.daria6918.cn

[C08] 闭包
来源：http://mtr.pycfn.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://oyq.yongpay.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bzm.gaohongyu789.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yvl.sxryk.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://huu.nanxinkj.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cqp.daxiang520.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://csy.shanyushiyangkeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ftc.wangdashe.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gje.jianghu66.top

[C09] 递归
来源：http://pdn.jinqigfzy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://heb.ehwqpu.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ejl.yvedp.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xfr.havefunace.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wbq.yonumen.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nbo.haohaochexian.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://axe.ydjk.org.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://twe.yuanzhike.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rdo.jinqigufen.top

[C10] 变量作用域
来源：http://vrg.shuidangran.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kli.daxiang520.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://quo.yj20258.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dnl.chenlongwang.top

TS:   同 JS
来源：http://xsf.sweek.top

Java: 方法内为块级作用域
来源：http://plq.xuetiantiany.cn

Go:   花括号块级作用域
来源：http://lru.hysaishi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qyw.bjfxy.top

C#:   块级作用域
来源：http://wut.yongpay.top

[C11] 模块导入与导出
来源：http://abz.ivvv.top

Py:   from module import func
来源：http://ufp.fktsv.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://jhs.52xcode.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://dtx.yj20258888.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xbs.epnwcf.com

Java: import java.util.List;
来源：http://qkf.guowangkeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pbh.yfazqb.com

Ruby: require "json"; require_relative "./util"
来源：http://ajw.meibo888.top

C#:   using System.Text;
来源：http://ent.jlsjyb.cn

[C12] 立即执行函数 IIFE
来源：http://llh.gotoacloud.top

Py:   (lambda: print("run"))()
来源：http://pno.redwolf501.top

PHP:  (function () { echo "run"; })();
来源：http://tbi.mhx1999.top

JS:   (() => { console.log("run"); })();
来源：http://khx.hcnkem.com

TS:   (() => { console.log("run"); })();
来源：http://kxo.vqdsnc.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://arn.shangyingyoupin.top

Go:   func() { fmt.Println("run") }()
来源：http://krg.dianchejie.cn

Ruby: -> { puts "run" }.call
来源：http://fvh.yonumen.top

C#:   // 无 IIFE：用静态构造函数
来源：http://fnn.tanke756.top

[C13] 类型声明 / 类型注解
来源：http://rhi.havefunace.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xqy.epnwcf.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kug.gzhubu.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zgp.zdqjudy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tcb.nwbrower.top

Java: int add(int a, int b) { return a + b; }
来源：http://gqg.kuanghao11.cn

Go:   func add(a, b int) int
来源：http://atp.fanxiaobao.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nii.jianghu66.top

C#:   int Add(int a, int b) => a + b;
来源：http://hgv.yj20258.top

[C14] 泛型函数
来源：http://jlx.zhixingplan.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://trl.guowangkeji.top

PHP:  // 无泛型
来源：http://ksi.daxiang520.top

JS:   // 无泛型
来源：http://csm.zhaomingkeji.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nds.shanyushiyangkeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://elo.xylfe.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yxs.feifeiyinyue.top

Ruby: # 无泛型
来源：http://erq.zhaomingkeji.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vfp.gogol.net.cn

[C15] 解构 / 展开参数
来源：http://qgn.snrcjt.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wcr.tarul.cn

PHP:  [$a, $b] = $pair;
来源：http://hbk.daria6918.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zyd.ydzc1.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mjv.chenlongwang.top

Java: // 无解构
来源：http://vnm.52xcode.cn

Go:   // 无解构
来源：http://eyg.cheryme.top

Ruby: a, b = pair
来源：http://pfx.hysaishi.cn

C#:   var (a, b) = pair;
来源：http://teh.dashuyun.cn

[C16] 函数 / 方法重载
来源：http://pnk.svipenyu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tvq.sysykeji.top

PHP:  // 无重载
来源：http://qyh.gaohongyu789.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://euk.sjlbkw.cn

TS:   // 用联合类型或重载签名声明
来源：http://gpx.chenjidiqi.icu

Java: void f(int a) {}  void f(String a) {}
来源：http://unu.smart0.xyz

Go:   // 无重载：用不同函数名
来源：http://wds.daria6918.cn

Ruby: # 无重载：靠动态参数
来源：http://vmw.birdmap.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ofz.cashguo.top

================================================================================
来源：http://aoe.snrcjt.cn

D. 数组 / 列表 / 集合
来源：http://app.tarul.cn

================================================================================
来源：http://shp.wangdashe.top

[D01] 创建数组 / 列表
来源：http://irr.guannengcc.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://vpo.gogol.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hij.ppjwa.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://joi.fehbvm.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://gbk.52xcode.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nni.vqdsnc.cn

Go:   arr := []int{1, 2, 3}
来源：http://hbd.aizwys.cn

Ruby: arr = [1, 2, 3]
来源：http://aer.zhoulong.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://afc.jianghu66.top

[D02] 追加元素到末尾
来源：http://kke.fengsongda.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cud.birdmap.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lpa.feifeiyinyue.top

JS:   arr.push(4);
来源：http://wah.yueranfly.top

TS:   arr.push(4);
来源：http://wrz.jinqigufen.top

Java: list.add(4);
来源：http://sxw.zhoulong.xyz

Go:   arr = append(arr, 4)
来源：http://qkt.bjfxy.top

Ruby: arr << 4; arr.push(5)
来源：http://xms.hnqzz.top

C#:   list.Add(4);
来源：http://ign.chenzaomai.com

[D03] 在指定位置插入元素
来源：http://bcn.xinyue.icu

Py:   arr.insert(0, 0)
来源：http://tkm.sjlbkw.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://sjd.hongshengwenyu.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fcb.ehwqpu.com

TS:   arr.splice(0, 0, 0);
来源：http://dvc.jqgufenzy.top

Java: list.add(0, 0);
来源：http://vfs.cheryme.top

Go:   arr = append([]int{0}, arr...)
来源：http://elg.fehbvm.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gqa.xingfuxueyuan.xyz

C#:   list.Insert(0, 0);
来源：http://zch.zhixingplan.top

[D04] 删除元素
来源：http://hot.nanxinkj.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://evc.daria6918.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kyv.nanxinkj.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wne.jlsjyb.cn

TS:   arr.splice(0, 1);
来源：http://str.andypj.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cqq.vqdsnc.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rui.shangyingyoupin.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://shi.yuanzhike.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pcj.ydzc1.top

[D05] 访问与修改元素
来源：http://inh.yj20258.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zqx.shangyingyoupin.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mek.hywenlv.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zlu.fanxiaobao.xyz

TS:   arr[0]; arr.at(-1);
来源：http://egd.hnqzz.top

Java: list.get(0); list.set(0, 9);
来源：http://mzq.ydzc1.top

Go:   arr[0]; arr[0] = 9
来源：http://rve.cqqwz.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vza.tarul.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://huv.cqqwz.cn

[D06] 数组长度
来源：http://xvb.zhengqikj.top

Py:   len(arr)
来源：http://dyc.kuanghao11.cn

PHP:  count($arr);
来源：http://aee.jlsjyb.cn

JS:   arr.length
来源：http://bnb.yj20258888.top

TS:   arr.length
来源：http://jgb.zhaomingkeji.xyz

Java: list.size();
来源：http://bih.hesvh.cn

Go:   len(arr)
来源：http://vtf.cucudq.cn

Ruby: arr.length; arr.size
来源：http://uzj.jyoumei.cn

C#:   list.Count;
来源：http://zcq.shanyushiyangkeji.top

[D07] 切片 / 取子数组
来源：http://sun.zdbjq.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gse.gotoacloud.top

PHP:  array_slice($arr, 1, 3);
来源：http://tjp.guannengcc.top

JS:   arr.slice(1, 4);
来源：http://cir.yuanzhike.top

TS:   arr.slice(1, 4);
来源：http://skg.zdqjudy.top

Java: list.subList(1, 4);
来源：http://wqi.jinyuanbaomall.cn

Go:   arr[1:4]
来源：http://cxt.aibaodan.cn

Ruby: arr[1, 3]
来源：http://sfo.ctjpmb.com

C#:   list.GetRange(1, 3);
来源：http://swj.tian-w.cn

[D08] 合并两个数组
来源：http://sym.shanyushiyangtech.top

Py:   a + b;  a.extend(b)
来源：http://hna.fzhhl.top

PHP:  array_merge($a, $b);
来源：http://rhh.yfazqb.com

JS:   [...a, ...b];  a.concat(b);
来源：http://eqz.dashuyun.cn

TS:   [...a, ...b];
来源：http://vgi.sxryk.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zga.hammf.cn

Go:   append(a, b...)
来源：http://twp.fanxiaobao.xyz

Ruby: a + b;  a.concat(b)
来源：http://mxw.hcnkem.com

C#:   a.Concat(b).ToList()
来源：http://how.jqgufenzy.top

[D09] 排序（升序）
来源：http://lmm.jqgfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://uie.ydzc1.top

PHP:  sort($arr);
来源：http://cgs.tianlin.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sck.sysykeji.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://hps.fehbvm.com

Java: Collections.sort(list);  list.sort(null);
来源：http://fmk.jinghuilouyu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kze.shuidangran.top

Ruby: arr.sort
来源：http://afe.zhixingplan.top

C#:   list.Sort();
来源：http://viw.vqdsnc.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://btc.pycfn.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zpw.fehbvm.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xwh.vqdsnc.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ahs.gogol.net.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://snk.smart0.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xhc.zdbjq.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ued.hysaishi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wlk.hnqzz.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sup.zhoulong.xyz


<!-- 参考信息 -->
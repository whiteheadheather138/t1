代发 wailian999

PHP:  range(0, 10, 2);
来源：http://jep.cashguo.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vne.ydzc1.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vyk.xylfe.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ibi.hnxiangtu.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wlo.guannengcc.top

Ruby: (0...10).step(2).to_a
来源：http://lqv.cashguo.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qfc.bjfxy.top

[B12] 跳出多层循环
来源：http://npt.yongpay.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://cpx.vqdsnc.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://tzf.c1oappe.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bau.dianchejie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ppm.daria6918.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nou.chenlongwang.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ncr.jianghu66.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://feq.dianchejie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hbc.fanxiaobao.xyz

[B13] 判断是否为数字
来源：http://dbr.sufxvd.cn

Py:   isinstance(x, (int, float))
来源：http://xta.gzhubu.top

PHP:  is_numeric($x)
来源：http://jvy.vehdjk.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vre.shanyushiyangkeji.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://she.cheryme.top

Java: x instanceof Number
来源：http://qjk.xingfuxueyuan.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://emz.ppjwa.cn

Ruby: x.is_a?(Numeric)
来源：http://eke.xinyue.icu

C#:   x is int or double or decimal
来源：http://tgx.aizwys.cn

[B14] 判断值是否在集合内
来源：http://pma.fengsongda.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cft.yj20258888.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yrv.zhengqikj.top

JS:   [1, 2, 3].includes(x)
来源：http://jil.tarul.cn

TS:   [1, 2, 3].includes(x)
来源：http://tcs.dashuyun.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://oqs.ydjk.org.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://syv.zycfv.cn

Ruby: [1, 2, 3].include?(x)
来源：http://rxr.yanxiufei.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fnw.hesvh.cn

[B15] 布尔运算与取反
来源：http://zng.gzhubu.top

Py:   a and b or not c
来源：http://lws.jinqigufen.top

PHP:  $a && $b || !$c
来源：http://ntg.shuidangran.top

JS:   a && b || !c
来源：http://wxu.chenlongwang.top

TS:   a && b || !c
来源：http://aky.pengpengdd.cyou

Java: a && b || !c
来源：http://ttn.redwolf501.top

Go:   a && b || !c
来源：http://dpm.aibaodan.cn

Ruby: a && b || !c
来源：http://vyr.aibaodan.cn

C#:   a && b || !c
来源：http://dad.xylfe.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ypr.sjlbkw.cn

Py:   if not data: return
来源：http://fsm.fanxiaobao.xyz

PHP:  if (!$data) { return; }
来源：http://axh.shuidangran.top

JS:   if (!data) return;
来源：http://tib.dianchejie.cn

TS:   if (!data) return;
来源：http://xah.yongpay.top

Java: if (data == null) return;
来源：http://kus.zdqjudy.top

Go:   if data == nil { return }
来源：http://ppa.redwolf501.top

Ruby: return if data.nil?
来源：http://gdp.mhx1999.top

C#:   if (data == null) return;
来源：http://rim.zhixingplan.top

================================================================================
来源：http://bnr.zdbjq.cn

C. 函数与作用域
来源：http://pzw.vehdjk.com

================================================================================
来源：http://rgc.guowangkeji.top

[C01] 定义函数
来源：http://qvf.cdnleiting.top

Py:   def add(a, b): return a + b
来源：http://nna.yuanzhike.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://etb.yanxiufei.cn

JS:   function add(a, b) { return a + b; }
来源：http://voh.bbcook.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jbc.smart0.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://vep.hfpthk.cn

Go:   func add(a, b int) int { return a + b }
来源：http://drd.vqdsnc.cn

Ruby: def add(a, b); a + b; end
来源：http://ser.9152youxi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vsl.jlsjyb.cn

[C02] 默认参数
来源：http://frg.hysaishi.cn

Py:   def greet(name="World"): return name
来源：http://qig.yangfankeji.com

PHP:  function greet($name = "World") { return $name; }
来源：http://vgf.jinghuilouyu.cn

JS:   function greet(name = "World") { return name; }
来源：http://kuy.9152youxi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://dcl.yj202588.top

Java: // 无默认参数：方法重载或 Optional
来源：http://hnb.shzxlz.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zlu.shanyushiyangkeji.top

Ruby: def greet(name = "World") = name
来源：http://wmr.yonumen.top

C#:   string Greet(string name = "World") => name;
来源：http://gcy.shangyingyoupin.top

[C03] 可变参数
来源：http://uee.shanyushiyangkeji.top

Py:   def total(*args): return sum(args)
来源：http://sce.jqgfzy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fna.wangdashe.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yrh.epnwcf.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fra.nanxuanxn.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fck.52xcode.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qma.cdnleiting.top

Ruby: def total(*nums); nums.sum; end
来源：http://iyr.9152youxi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gfu.9152youxi.cn

[C04] 命名参数 / 关键字参数
来源：http://gts.hongshengwenyu.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rsx.kuanghao11.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jql.hnqzz.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kjd.jinghuilouyu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rjf.0kj1m.cn

Java: // 无：用 Builder 模式或 record
来源：http://ymt.hysaishi.cn

Go:   // 无：用配置结构体参数
来源：http://yay.vqdsnc.cn

Ruby: f(a: 1, b: 2)
来源：http://zug.hysaishi.cn

C#:   f(a: 1, b: 2)
来源：http://vun.hfpthk.cn

[C05] 返回多个值
来源：http://iuh.316326.xyz

Py:   return a, b
来源：http://xsp.birdmap.top

PHP:  return [$a, $b];
来源：http://sdv.zhoulong.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://ggx.52xcode.cn

TS:   return { a, b };
来源：http://ffs.wangshuangyany.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hwm.pengpengdd.cyou

Go:   return a, b
来源：http://bcr.haohaochexian.top

Ruby: return a, b
来源：http://ktq.vehdjk.com

C#:   return (a, b);              // ValueTuple
来源：http://sbe.gotoacloud.top

[C06] 匿名函数 / lambda
来源：http://sow.ehwqpu.com

Py:   square = lambda x: x * x
来源：http://xmp.fzhhl.top

PHP:  $square = fn($x) => $x * $x;
来源：http://pxu.epnwcf.com

JS:   const square = x => x * x;
来源：http://rta.hammf.cn

TS:   const square = (x: number): number => x * x;
来源：http://ckl.zhiwuduotai.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ppk.aizwys.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qkw.c1oappe.top

Ruby: square = ->(x) { x * x }
来源：http://vnm.shangyingyoupin.top

C#:   Func<int, int> square = x => x * x;
来源：http://ymn.hesvh.cn

[C07] 把函数作为参数传入
来源：http://hfh.nwbrower.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lyu.yongpay.top

PHP:  array_map("strtoupper", $arr);
来源：http://xvx.9152youxi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jwb.aizwys.cn

TS:   arr.map(String)
来源：http://hkv.zycfv.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zun.shuidangran.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://whc.tian-w.cn

Ruby: arr.map(&:upcase)
来源：http://zxs.xziqi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://deb.haohaochexian.top

[C08] 闭包
来源：http://qbe.meibo888.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uuh.yj202588.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://scz.zhoulong.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hka.ydzc1.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hlv.aizwys.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fwt.ppjwa.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tql.sufxvd.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bpz.yangfankeji.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://etl.vqdsnc.cn

[C09] 递归
来源：http://pos.hywenlv.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://unt.52xcode.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sqf.jianghu66.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ugh.hammf.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sgw.epnwcf.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://npq.guowangkeji.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bai.vqdsnc.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://adt.hcnkem.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://onf.aibaodan.cn

[C10] 变量作用域
来源：http://nfa.andypj.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nmw.cashguo.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mwo.smart0.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://biz.shanyushiyangkeji.top

TS:   同 JS
来源：http://sgf.aibaodan.cn

Java: 方法内为块级作用域
来源：http://oti.fehbvm.com

Go:   花括号块级作用域
来源：http://enw.aibaodan.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bdt.cashguo.top

C#:   块级作用域
来源：http://xpz.tarul.cn

[C11] 模块导入与导出
来源：http://mvx.smart0.xyz

Py:   from module import func
来源：http://dto.hywenlv.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://jkf.nanxuanxn.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://owm.ehwqpu.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zgh.aizwys.cn

Java: import java.util.List;
来源：http://xsm.0kj1m.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://iqr.zdqjudy.top

Ruby: require "json"; require_relative "./util"
来源：http://yez.sufxvd.cn

C#:   using System.Text;
来源：http://act.hcnkem.com

[C12] 立即执行函数 IIFE
来源：http://gmb.tian-w.cn

Py:   (lambda: print("run"))()
来源：http://onc.cdnleiting.top

PHP:  (function () { echo "run"; })();
来源：http://enp.shuidangran.top

JS:   (() => { console.log("run"); })();
来源：http://uwm.yj20258.top

TS:   (() => { console.log("run"); })();
来源：http://wfc.mhx1999.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hup.xuanzx.com

Go:   func() { fmt.Println("run") }()
来源：http://yat.yonumen.top

Ruby: -> { puts "run" }.call
来源：http://qtx.ydzc1.top

C#:   // 无 IIFE：用静态构造函数
来源：http://frs.fehbvm.com

[C13] 类型声明 / 类型注解
来源：http://kzr.0kj1m.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://drt.cqqwz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mcq.gaohongyu789.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fbq.yonumen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jta.dianchejie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xnj.zhengqikj.top

Go:   func add(a, b int) int
来源：http://kot.aizwys.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qme.sjlbkw.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mdt.andypj.xyz

[C14] 泛型函数
来源：http://wnt.c1oappe.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jof.52xcode.cn

PHP:  // 无泛型
来源：http://sie.sjlbkw.cn

JS:   // 无泛型
来源：http://dbk.mhx1999.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hlv.feifeiyinyue.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kos.gogol.net.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qey.guowangkeji.top

Ruby: # 无泛型
来源：http://pba.chenjidiqi.icu

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wdk.chenjidiqi.icu

[C15] 解构 / 展开参数
来源：http://ajh.svipenyu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ugd.andypj.xyz

PHP:  [$a, $b] = $pair;
来源：http://wul.snrcjt.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lum.zdqjudy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://oyc.hnxiangtu.top

Java: // 无解构
来源：http://zal.hesvh.cn

Go:   // 无解构
来源：http://twg.yonumen.top

Ruby: a, b = pair
来源：http://kup.pengpengdd.cyou

C#:   var (a, b) = pair;
来源：http://ppx.feifeiyinyue.top

[C16] 函数 / 方法重载
来源：http://qzo.yangfankeji.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ewp.zhongyouzk.top

PHP:  // 无重载
来源：http://jzh.jinqigfzy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://zlk.zhixingplan.top

TS:   // 用联合类型或重载签名声明
来源：http://eaa.zhixingplan.top

Java: void f(int a) {}  void f(String a) {}
来源：http://idk.xylfe.cn

Go:   // 无重载：用不同函数名
来源：http://nwc.yueranfly.top

Ruby: # 无重载：靠动态参数
来源：http://fst.dianchejie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://lel.aizwys.cn

================================================================================
来源：http://aoi.zdqjudy.top

D. 数组 / 列表 / 集合
来源：http://eqv.hysaishi.cn

================================================================================
来源：http://ckf.xinyue.icu

[D01] 创建数组 / 列表
来源：http://egz.yangfankeji.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://jfl.wangshuangyany.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fsg.andypj.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rwo.hnxiangtu.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://njm.316326.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dde.aibaodan.cn

Go:   arr := []int{1, 2, 3}
来源：http://amy.cashguo.top

Ruby: arr = [1, 2, 3]
来源：http://mfr.guowangkeji.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://acg.xuetiantiany.cn

[D02] 追加元素到末尾
来源：http://eue.fzhhl.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rka.bbcook.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ibo.9152youxi.cn

JS:   arr.push(4);
来源：http://wkr.pycfn.com

TS:   arr.push(4);
来源：http://qvj.xingfuxueyuan.xyz

Java: list.add(4);
来源：http://mhd.shangyingyoupin.top

Go:   arr = append(arr, 4)
来源：http://ipo.jqgufenzy.top

Ruby: arr << 4; arr.push(5)
来源：http://onn.ctjpmb.com

C#:   list.Add(4);
来源：http://yrb.yvedp.cn

[D03] 在指定位置插入元素
来源：http://lka.jinyuanbaomall.cn

Py:   arr.insert(0, 0)
来源：http://zdu.gogol.net.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lfh.dashuyun.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://red.0kj1m.cn

TS:   arr.splice(0, 0, 0);
来源：http://sal.yj20258888.top

Java: list.add(0, 0);
来源：http://chv.fengsongda.top

Go:   arr = append([]int{0}, arr...)
来源：http://hly.zycfv.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ksq.smart0.xyz

C#:   list.Insert(0, 0);
来源：http://tuj.cqqwz.cn

[D04] 删除元素
来源：http://vzd.meibo888.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nnz.havefunace.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nza.tanke756.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hif.zhengqikj.top

TS:   arr.splice(0, 1);
来源：http://qgm.hnxiangtu.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wpm.hnxiangtu.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pzs.jyoumei.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rmm.shangyingyoupin.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://czt.jyoumei.cn

[D05] 访问与修改元素
来源：http://zni.yj20258888.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://joa.yuanzhike.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ggc.mhx1999.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://moz.hywenlv.cn

TS:   arr[0]; arr.at(-1);
来源：http://ucd.gotoacloud.top

Java: list.get(0); list.set(0, 9);
来源：http://blw.aizwys.cn

Go:   arr[0]; arr[0] = 9
来源：http://wve.sjlbkw.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ami.pycfn.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xxz.hesvh.cn

[D06] 数组长度
来源：http://ofd.hnqzz.top

Py:   len(arr)
来源：http://bzu.zhiwuduotai.top

PHP:  count($arr);
来源：http://bag.snrcjt.cn

JS:   arr.length
来源：http://btx.yj20258.top

TS:   arr.length
来源：http://ftc.fengsongda.top

Java: list.size();
来源：http://sjk.wangdashe.top

Go:   len(arr)
来源：http://riv.sweek.top

Ruby: arr.length; arr.size
来源：http://xiz.nanxuanxn.top

C#:   list.Count;
来源：http://dtt.zhiwuduotai.top

[D07] 切片 / 取子数组
来源：http://zzz.jianghu66.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tcn.wangdashe.top

PHP:  array_slice($arr, 1, 3);
来源：http://grq.jinyuanbaomall.cn

JS:   arr.slice(1, 4);
来源：http://lpm.hfpthk.cn

TS:   arr.slice(1, 4);
来源：http://qha.jinghuilouyu.cn

Java: list.subList(1, 4);
来源：http://yab.nanxinkj.top

Go:   arr[1:4]
来源：http://olq.hesvh.cn

Ruby: arr[1, 3]
来源：http://cty.yfazqb.com

C#:   list.GetRange(1, 3);
来源：http://cco.zycfv.cn

[D08] 合并两个数组
来源：http://sqy.guannengcc.top

Py:   a + b;  a.extend(b)
来源：http://gny.52xcode.cn

PHP:  array_merge($a, $b);
来源：http://slf.zdqjudy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://nsl.chenlongwang.top

TS:   [...a, ...b];
来源：http://vmq.feifeiyinyue.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ewn.shanyushiyangkeji.top

Go:   append(a, b...)
来源：http://fbg.hysaishi.cn

Ruby: a + b;  a.concat(b)
来源：http://esf.guannengcc.top

C#:   a.Concat(b).ToList()
来源：http://mhm.sysykeji.top

[D09] 排序（升序）
来源：http://dmr.sxryk.cn

Py:   sorted(arr);  arr.sort()
来源：http://bpl.jinyuanbaomall.cn

PHP:  sort($arr);
来源：http://equ.jinqigfzy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nat.hcnkem.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://zck.sjlbkw.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hfu.daxiang520.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xfr.dianchejie.cn

Ruby: arr.sort
来源：http://mrg.dianchejie.cn

C#:   list.Sort();
来源：http://wnx.xinyue.icu

[D10] 自定义排序（按字段 / 多条件）
来源：http://btk.sufxvd.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jiy.pycfn.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mio.hnqzz.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vdo.yanxiufei.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://spa.shanyushiyangkeji.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gmy.hnxiangtu.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gxn.shanyushiyangtech.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://srq.tarul.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dbf.jqgfzy.top

[D11] 反转数组
来源：http://mum.zhengqikj.top

Py:   arr[::-1];  arr.reverse()
来源：http://atx.pengpengdd.cyou

PHP:  array_reverse($arr);
来源：http://sxe.svipenyu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mdp.shuidangran.top

TS:   [...arr].reverse();
来源：http://ydq.hfpthk.cn

Java: Collections.reverse(list);
来源：http://asb.hcnkem.com

Go:   slices.Reverse(arr)
来源：http://rjp.ywan-chungtsiang.top

Ruby: arr.reverse
来源：http://lne.vqdsnc.cn


<!-- 参考信息 -->
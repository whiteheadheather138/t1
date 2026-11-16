代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://tcc.svipenyu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://jsl.sysykeji.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ukv.ydzc1.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bxq.jqgufenzy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://acq.xingfuxueyuan.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yhs.xylfe.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xmb.hysaishi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gno.cashguo.top

[B13] 判断是否为数字
来源：http://jek.zhijiandao.cn

Py:   isinstance(x, (int, float))
来源：http://rfm.bbcook.cn

PHP:  is_numeric($x)
来源：http://bhu.uphjek.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://awf.vqdsnc.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://exg.snrcjt.cn

Java: x instanceof Number
来源：http://lnu.shanyushiyangkeji.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fjg.jianghu66.top

Ruby: x.is_a?(Numeric)
来源：http://biu.shanyushiyangkeji.top

C#:   x is int or double or decimal
来源：http://ciw.aibaodan.cn

[B14] 判断值是否在集合内
来源：http://pgh.wangdashe.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nlc.gogol.net.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://krs.sweek.top

JS:   [1, 2, 3].includes(x)
来源：http://zrs.zhiwuduotai.top

TS:   [1, 2, 3].includes(x)
来源：http://tgt.zhiwuduotai.top

Java: List.of(1, 2, 3).contains(x)
来源：http://oga.feifeiyinyue.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vqn.zhiwuduotai.top

Ruby: [1, 2, 3].include?(x)
来源：http://abg.yuxming.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bdk.jinyuanbaomall.cn

[B15] 布尔运算与取反
来源：http://eih.jinqigfzy.top

Py:   a and b or not c
来源：http://qvx.havefunace.top

PHP:  $a && $b || !$c
来源：http://pwq.sweek.top

JS:   a && b || !c
来源：http://owr.316326.xyz

TS:   a && b || !c
来源：http://lzv.zhaomingkeji.xyz

Java: a && b || !c
来源：http://fht.uphjek.com

Go:   a && b || !c
来源：http://lqu.hfpthk.cn

Ruby: a && b || !c
来源：http://gxp.hnxiangtu.top

C#:   a && b || !c
来源：http://muy.yfazqb.com

[B16] 卫语句：不满足条件提前返回
来源：http://rod.aizwys.cn

Py:   if not data: return
来源：http://vir.cucudq.cn

PHP:  if (!$data) { return; }
来源：http://gut.ydzc1.top

JS:   if (!data) return;
来源：http://zwy.fehbvm.com

TS:   if (!data) return;
来源：http://bwv.gzhubu.top

Java: if (data == null) return;
来源：http://ygz.fehbvm.com

Go:   if data == nil { return }
来源：http://vbs.redwolf501.top

Ruby: return if data.nil?
来源：http://liz.redwolf501.top

C#:   if (data == null) return;
来源：http://jme.jiagoushi.top

================================================================================
来源：http://vpp.yangfankeji.com

C. 函数与作用域
来源：http://ies.daria6918.cn

================================================================================
来源：http://iop.epnwcf.com

[C01] 定义函数
来源：http://afe.hammf.cn

Py:   def add(a, b): return a + b
来源：http://eod.quarkkingdee.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wcu.tianlin.xyz

JS:   function add(a, b) { return a + b; }
来源：http://knh.guowangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ngx.9152youxi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://olt.52xcode.cn

Go:   func add(a, b int) int { return a + b }
来源：http://eyj.shzxlz.cn

Ruby: def add(a, b); a + b; end
来源：http://zip.bbcook.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fpv.gaohongyu789.top

[C02] 默认参数
来源：http://mjx.ywan-chungtsiang.top

Py:   def greet(name="World"): return name
来源：http://shw.jlsjyb.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://kee.iojbl.cn

JS:   function greet(name = "World") { return name; }
来源：http://zod.dashuyun.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://eey.zycfv.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://egj.sjlbkw.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://oie.daxiang520.top

Ruby: def greet(name = "World") = name
来源：http://pip.shzxlz.cn

C#:   string Greet(string name = "World") => name;
来源：http://leb.yj20258.top

[C03] 可变参数
来源：http://lpo.zhengqikj.top

Py:   def total(*args): return sum(args)
来源：http://swr.svipenyu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://srz.dianchejie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://npe.jinqigufen.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://inh.andypj.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wvv.fktsv.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://evi.jinyuanbaomall.cn

Ruby: def total(*nums); nums.sum; end
来源：http://krp.ehwqpu.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xgx.dianchejie.cn

[C04] 命名参数 / 关键字参数
来源：http://bck.yongpay.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ljm.epnwcf.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jps.haohaochexian.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zkh.vqdsnc.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dyq.fktsv.cn

Java: // 无：用 Builder 模式或 record
来源：http://vjx.redwolf501.top

Go:   // 无：用配置结构体参数
来源：http://tsw.cucudq.cn

Ruby: f(a: 1, b: 2)
来源：http://ilj.guowangkeji.top

C#:   f(a: 1, b: 2)
来源：http://sho.shanyushiyangtech.top

[C05] 返回多个值
来源：http://ntm.andypj.xyz

Py:   return a, b
来源：http://tez.bbcook.cn

PHP:  return [$a, $b];
来源：http://urb.yueranfly.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://lpi.hfpthk.cn

TS:   return { a, b };
来源：http://thw.xingfuxueyuan.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://svb.tarul.cn

Go:   return a, b
来源：http://hho.andypj.xyz

Ruby: return a, b
来源：http://xmk.zdbjq.cn

C#:   return (a, b);              // ValueTuple
来源：http://ocb.sysykeji.top

[C06] 匿名函数 / lambda
来源：http://pht.cheryme.top

Py:   square = lambda x: x * x
来源：http://eyx.tianlin.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://dnw.zdbjq.cn

JS:   const square = x => x * x;
来源：http://jwb.chenjidiqi.icu

TS:   const square = (x: number): number => x * x;
来源：http://vwu.ydzc1.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lab.redwolf501.top

Go:   sq := func(x int) int { return x * x }
来源：http://lho.xuanzx.com

Ruby: square = ->(x) { x * x }
来源：http://jue.guannengcc.top

C#:   Func<int, int> square = x => x * x;
来源：http://mrt.vqdsnc.cn

[C07] 把函数作为参数传入
来源：http://jru.cucudq.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ocg.vqdsnc.cn

PHP:  array_map("strtoupper", $arr);
来源：http://qgr.daria6918.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lda.9152youxi.cn

TS:   arr.map(String)
来源：http://ezt.kuanghao11.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xah.shanyushiyangkeji.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gbv.mhx1999.top

Ruby: arr.map(&:upcase)
来源：http://jel.shangyingyoupin.top

C#:   arr.Select(s => s.ToUpper())
来源：http://vbj.sjlbkw.cn

[C08] 闭包
来源：http://jsm.xinyue.icu

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gni.yj20258.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sni.jlsjyb.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fzw.zhixingplan.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gzf.zhongyouzk.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jyn.bjfxy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://joy.shuidangran.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cub.daria6918.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tbv.yonumen.top

[C09] 递归
来源：http://rvx.smart0.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://awq.jqgfzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xmx.jiagoushi.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://idr.sufxvd.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wvv.nwbrower.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hkb.aibaodan.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tsu.pengpengdd.cyou

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://oab.shuidangran.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zgx.fehbvm.com

[C10] 变量作用域
来源：http://hpk.pycfn.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ytg.sjlbkw.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ifa.tarul.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://efz.shuidangran.top

TS:   同 JS
来源：http://pjc.tarul.cn

Java: 方法内为块级作用域
来源：http://jem.hongshengwenyu.top

Go:   花括号块级作用域
来源：http://ice.cashguo.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rfz.yangfankeji.com

C#:   块级作用域
来源：http://hsi.vehdjk.com

[C11] 模块导入与导出
来源：http://nah.yvedp.cn

Py:   from module import func
来源：http://wnv.quarkkingdee.top

PHP:  require "file.php";  或 use App\Service;
来源：http://eme.meibo888.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://dee.aizwys.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xkd.zhongyouzk.top

Java: import java.util.List;
来源：http://jud.fehbvm.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ust.jqgufenzy.top

Ruby: require "json"; require_relative "./util"
来源：http://qlm.zhijiandao.cn

C#:   using System.Text;
来源：http://url.sjlbkw.cn

[C12] 立即执行函数 IIFE
来源：http://kte.tianlin.xyz

Py:   (lambda: print("run"))()
来源：http://uib.gaohongyu789.top

PHP:  (function () { echo "run"; })();
来源：http://ubs.ydzc1.top

JS:   (() => { console.log("run"); })();
来源：http://vlu.hongshengwenyu.top

TS:   (() => { console.log("run"); })();
来源：http://heq.yueranfly.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://drs.ctjpmb.com

Go:   func() { fmt.Println("run") }()
来源：http://hnz.yueranfly.top

Ruby: -> { puts "run" }.call
来源：http://skg.wangshuangyany.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://lam.shanyushiyangkeji.top

[C13] 类型声明 / 类型注解
来源：http://gtd.daxiang520.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tvb.zhongyouzk.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wua.9152youxi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yxe.yj20258888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://azp.sweek.top

Java: int add(int a, int b) { return a + b; }
来源：http://izy.xylfe.cn

Go:   func add(a, b int) int
来源：http://ekh.bbcook.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kif.yj20258.top

C#:   int Add(int a, int b) => a + b;
来源：http://bcl.gaohongyu789.top

[C14] 泛型函数
来源：http://eup.yvedp.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ors.yj202588.top

PHP:  // 无泛型
来源：http://epn.sysykeji.top

JS:   // 无泛型
来源：http://sec.shanyushiyangtech.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fah.havefunace.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zwt.vehdjk.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://drn.zhixingplan.top

Ruby: # 无泛型
来源：http://ecl.ctjpmb.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wbf.jyoumei.cn

[C15] 解构 / 展开参数
来源：http://alm.zdbjq.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fty.ydzc1.top

PHP:  [$a, $b] = $pair;
来源：http://yjz.jinqigfzy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cuf.zhoulong.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hml.shanyushiyangkeji.top

Java: // 无解构
来源：http://cvp.iojbl.cn

Go:   // 无解构
来源：http://mjn.yvedp.cn

Ruby: a, b = pair
来源：http://kbt.hfpthk.cn

C#:   var (a, b) = pair;
来源：http://lcq.zhixingplan.top

[C16] 函数 / 方法重载
来源：http://fay.yfazqb.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://uev.yfazqb.com

PHP:  // 无重载
来源：http://ofp.yfazqb.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://pyw.epnwcf.com

TS:   // 用联合类型或重载签名声明
来源：http://hax.gaohongyu789.top

Java: void f(int a) {}  void f(String a) {}
来源：http://xdd.yonumen.top

Go:   // 无重载：用不同函数名
来源：http://ahr.ywan-chungtsiang.top

Ruby: # 无重载：靠动态参数
来源：http://obh.haohaochexian.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://dir.tanke756.top

================================================================================
来源：http://tca.tian-w.cn

D. 数组 / 列表 / 集合
来源：http://dzy.mhx1999.top

================================================================================
来源：http://fnj.hysaishi.cn

[D01] 创建数组 / 列表
来源：http://nfw.xuetiantiany.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mgh.c1oappe.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zjn.jianghu66.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pct.yuanzhike.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://iut.yj20258.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cbr.fehbvm.com

Go:   arr := []int{1, 2, 3}
来源：http://yek.xuetiantiany.cn

Ruby: arr = [1, 2, 3]
来源：http://qoa.aibaodan.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mvx.zhiwuduotai.top

[D02] 追加元素到末尾
来源：http://adb.sjlbkw.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tuh.sjlbkw.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pbn.jinghuilouyu.cn

JS:   arr.push(4);
来源：http://spd.jqgufenzy.top

TS:   arr.push(4);
来源：http://ged.ppjwa.cn

Java: list.add(4);
来源：http://jbz.chenjidiqi.icu

Go:   arr = append(arr, 4)
来源：http://tee.ivvv.top

Ruby: arr << 4; arr.push(5)
来源：http://alq.shuidangran.top

C#:   list.Add(4);
来源：http://guw.tanke756.top

[D03] 在指定位置插入元素
来源：http://rhu.316326.xyz

Py:   arr.insert(0, 0)
来源：http://ybi.nanxinkj.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dhb.iojbl.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vgk.epnwcf.com

TS:   arr.splice(0, 0, 0);
来源：http://hqi.shuidangran.top

Java: list.add(0, 0);
来源：http://lrz.zhongyouzk.top

Go:   arr = append([]int{0}, arr...)
来源：http://zku.yvedp.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gcf.iojbl.cn

C#:   list.Insert(0, 0);
来源：http://mjb.pycfn.com

[D04] 删除元素
来源：http://cer.redwolf501.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://imh.svipenyu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://aml.jinyuanbaomall.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pgn.0kj1m.cn

TS:   arr.splice(0, 1);
来源：http://qdy.yvedp.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://sir.bjfxy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nms.jinqigufen.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://iig.52xcode.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pac.quarkkingdee.top

[D05] 访问与修改元素
来源：http://wey.bbcook.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dqf.redwolf501.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://csr.xingfuxueyuan.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rud.ehwqpu.com

TS:   arr[0]; arr.at(-1);
来源：http://ywa.zhiwuduotai.top

Java: list.get(0); list.set(0, 9);
来源：http://acw.snrcjt.cn

Go:   arr[0]; arr[0] = 9
来源：http://fto.iojbl.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ieh.hysaishi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yht.quarkkingdee.top

[D06] 数组长度
来源：http://rrn.yj202588.top

Py:   len(arr)
来源：http://apc.hnqzz.top

PHP:  count($arr);
来源：http://vsk.9152youxi.cn

JS:   arr.length
来源：http://hfj.redwolf501.top

TS:   arr.length
来源：http://lkk.dashuyun.cn

Java: list.size();
来源：http://ohg.0kj1m.cn

Go:   len(arr)
来源：http://lql.fengsongda.top

Ruby: arr.length; arr.size
来源：http://fkt.ctjpmb.com

C#:   list.Count;
来源：http://vej.cashguo.top

[D07] 切片 / 取子数组
来源：http://ayb.yangfankeji.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xso.sweek.top

PHP:  array_slice($arr, 1, 3);
来源：http://uiq.fanxiaobao.xyz

JS:   arr.slice(1, 4);
来源：http://rzc.xingfuxueyuan.xyz

TS:   arr.slice(1, 4);
来源：http://ltg.xuanzx.com

Java: list.subList(1, 4);
来源：http://gds.xziqi.cn

Go:   arr[1:4]
来源：http://mtg.snrcjt.cn

Ruby: arr[1, 3]
来源：http://rav.ydjk.org.cn

C#:   list.GetRange(1, 3);
来源：http://wce.yj20258888.top

[D08] 合并两个数组
来源：http://vrg.havefunace.top

Py:   a + b;  a.extend(b)
来源：http://tuo.sjlbkw.cn

PHP:  array_merge($a, $b);
来源：http://ffc.jinyuanbaomall.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://god.52xcode.cn

TS:   [...a, ...b];
来源：http://egu.nwbrower.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nzz.yj20258888.top

Go:   append(a, b...)
来源：http://rnn.feifeiyinyue.top

Ruby: a + b;  a.concat(b)
来源：http://cxf.hywenlv.cn

C#:   a.Concat(b).ToList()
来源：http://ehc.hesvh.cn

[D09] 排序（升序）
来源：http://baz.52xcode.cn

Py:   sorted(arr);  arr.sort()
来源：http://qrr.tian-w.cn

PHP:  sort($arr);
来源：http://ihj.pycfn.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zcs.0kj1m.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://iog.gaohongyu789.top

Java: Collections.sort(list);  list.sort(null);
来源：http://hen.jinqigufen.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qjk.dianchejie.cn

Ruby: arr.sort
来源：http://hue.haohaochexian.top

C#:   list.Sort();
来源：http://dcz.jqgfzy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://uib.hnxiangtu.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bht.yvedp.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bmz.svipenyu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://usn.tianlin.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://asc.fzhhl.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mgl.yfazqb.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://awj.jinghuilouyu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nad.jqgfzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vhl.yj202588.top

[D11] 反转数组
来源：http://epm.hesvh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://vzy.aibaodan.cn

PHP:  array_reverse($arr);
来源：http://wbe.zhongyouzk.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ucl.yuxming.cn

TS:   [...arr].reverse();
来源：http://tbg.shzxlz.cn

Java: Collections.reverse(list);
来源：http://cxe.jinyuanbaomall.cn

Go:   slices.Reverse(arr)
来源：http://kou.meibo888.top

Ruby: arr.reverse
来源：http://mpp.guannengcc.top

C#:   list.Reverse();
来源：http://fks.zhiwuduotai.top

[D12] 查找元素下标
来源：http://oxk.yvedp.cn

Py:   arr.index(x);  x in arr
来源：http://dso.redwolf501.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kol.hnqzz.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ilg.cashguo.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sfy.xylfe.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tqn.chenlongwang.top

Go:   slices.Index(arr, x)
来源：http://eun.chenjidiqi.icu


<!-- 参考信息 -->
代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://kck.smart0.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hkg.yongpay.top

[B15] 布尔运算与取反
来源：http://glf.zhiwuduotai.top

Py:   a and b or not c
来源：http://lej.sxryk.cn

PHP:  $a && $b || !$c
来源：http://hoy.jiagoushi.top

JS:   a && b || !c
来源：http://toz.ctjpmb.com

TS:   a && b || !c
来源：http://qlt.ehwqpu.com

Java: a && b || !c
来源：http://myg.zhixingplan.top

Go:   a && b || !c
来源：http://htg.yj20258888.top

Ruby: a && b || !c
来源：http://uwo.kuanghao11.cn

C#:   a && b || !c
来源：http://djq.tianlin.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://yih.cucudq.cn

Py:   if not data: return
来源：http://jdi.xylfe.cn

PHP:  if (!$data) { return; }
来源：http://ghv.0kj1m.cn

JS:   if (!data) return;
来源：http://ttx.tian-w.cn

TS:   if (!data) return;
来源：http://rfu.yongpay.top

Java: if (data == null) return;
来源：http://fga.snrcjt.cn

Go:   if data == nil { return }
来源：http://ktm.cucudq.cn

Ruby: return if data.nil?
来源：http://kck.hywenlv.cn

C#:   if (data == null) return;
来源：http://wia.shanyushiyangkeji.top

================================================================================
来源：http://zeu.sjlbkw.cn

C. 函数与作用域
来源：http://hji.bjfxy.top

================================================================================
来源：http://mul.tianlin.xyz

[C01] 定义函数
来源：http://hfn.gaohongyu789.top

Py:   def add(a, b): return a + b
来源：http://scy.zhijiandao.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ewp.sweek.top

JS:   function add(a, b) { return a + b; }
来源：http://uxq.dianchejie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vtb.cashguo.top

Java: static int add(int a, int b) { return a + b; }
来源：http://uhy.ivvv.top

Go:   func add(a, b int) int { return a + b }
来源：http://udk.jinyuanbaomall.cn

Ruby: def add(a, b); a + b; end
来源：http://evt.redwolf501.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kxb.fehbvm.com

[C02] 默认参数
来源：http://yih.hysaishi.cn

Py:   def greet(name="World"): return name
来源：http://ycg.chenjidiqi.icu

PHP:  function greet($name = "World") { return $name; }
来源：http://bdv.daxiang520.top

JS:   function greet(name = "World") { return name; }
来源：http://gif.guowangkeji.top

TS:   function greet(name: string = "World") { return name; }
来源：http://jpl.hfpthk.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://msj.vehdjk.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ibg.zhijiandao.cn

Ruby: def greet(name = "World") = name
来源：http://iia.chenlongwang.top

C#:   string Greet(string name = "World") => name;
来源：http://wdr.dashuyun.cn

[C03] 可变参数
来源：http://nvx.fktsv.cn

Py:   def total(*args): return sum(args)
来源：http://jjw.cucudq.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://llg.sweek.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xzx.chenlongwang.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://unf.sysykeji.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xrl.zhijiandao.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://oym.hnqzz.top

Ruby: def total(*nums); nums.sum; end
来源：http://pgg.zhengqikj.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bot.nanxinkj.top

[C04] 命名参数 / 关键字参数
来源：http://aoi.pengpengdd.cyou

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://edp.vqdsnc.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cny.zhengqikj.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ukj.zhixingplan.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jjt.ppjwa.cn

Java: // 无：用 Builder 模式或 record
来源：http://lsc.9152youxi.cn

Go:   // 无：用配置结构体参数
来源：http://wdw.c1oappe.top

Ruby: f(a: 1, b: 2)
来源：http://lam.shuidangran.top

C#:   f(a: 1, b: 2)
来源：http://jve.nanxinkj.top

[C05] 返回多个值
来源：http://akg.yongpay.top

Py:   return a, b
来源：http://ppp.redwolf501.top

PHP:  return [$a, $b];
来源：http://cln.yanxiufei.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://olt.feifeiyinyue.top

TS:   return { a, b };
来源：http://phj.zycfv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://frr.gogol.net.cn

Go:   return a, b
来源：http://aoi.shzxlz.cn

Ruby: return a, b
来源：http://upl.vehdjk.com

C#:   return (a, b);              // ValueTuple
来源：http://kaf.feifeiyinyue.top

[C06] 匿名函数 / lambda
来源：http://qmt.xuanzx.com

Py:   square = lambda x: x * x
来源：http://wba.gogol.net.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://jrj.sxryk.cn

JS:   const square = x => x * x;
来源：http://dhq.jqgfzy.top

TS:   const square = (x: number): number => x * x;
来源：http://eij.9152youxi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://win.ywan-chungtsiang.top

Go:   sq := func(x int) int { return x * x }
来源：http://kqw.xylfe.cn

Ruby: square = ->(x) { x * x }
来源：http://ayo.pycfn.com

C#:   Func<int, int> square = x => x * x;
来源：http://qne.quarkkingdee.top

[C07] 把函数作为参数传入
来源：http://hek.zhengqikj.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rqu.c1oappe.top

PHP:  array_map("strtoupper", $arr);
来源：http://dtr.dashuyun.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://whv.yueranfly.top

TS:   arr.map(String)
来源：http://fld.ybcxt.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mhz.zhijiandao.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yab.daria6918.cn

Ruby: arr.map(&:upcase)
来源：http://fja.jinghuilouyu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gys.zhengqikj.top

[C08] 闭包
来源：http://bhv.sufxvd.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ywt.fanxiaobao.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jfy.ywan-chungtsiang.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fer.zhoulong.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jaj.yueranfly.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://uii.zhijiandao.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://scd.guowangkeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ukv.yangfankeji.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ddb.bbcook.cn

[C09] 递归
来源：http://kyr.yuxming.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jbk.feifeiyinyue.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://drq.nanxinkj.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rwd.jinqigfzy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jmp.shangyingyoupin.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kid.kuanghao11.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tmb.9152youxi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ufm.yj20258888.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mqi.nanxinkj.top

[C10] 变量作用域
来源：http://zlq.jinqigfzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qqf.feifeiyinyue.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qbh.hnxiangtu.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ect.svipenyu.cn

TS:   同 JS
来源：http://cho.hammf.cn

Java: 方法内为块级作用域
来源：http://jrr.uphjek.com

Go:   花括号块级作用域
来源：http://mxq.ctjpmb.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xwm.hnxiangtu.top

C#:   块级作用域
来源：http://ugq.redwolf501.top

[C11] 模块导入与导出
来源：http://fms.hammf.cn

Py:   from module import func
来源：http://pkn.vqdsnc.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://oiu.birdmap.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ozh.yj20258.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mjk.svipenyu.cn

Java: import java.util.List;
来源：http://qky.dashuyun.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ljz.chenlongwang.top

Ruby: require "json"; require_relative "./util"
来源：http://sjx.fengsongda.top

C#:   using System.Text;
来源：http://vla.xuetiantiany.cn

[C12] 立即执行函数 IIFE
来源：http://ock.nanxinkj.top

Py:   (lambda: print("run"))()
来源：http://car.smart0.xyz

PHP:  (function () { echo "run"; })();
来源：http://asf.fehbvm.com

JS:   (() => { console.log("run"); })();
来源：http://pyp.yanxiufei.cn

TS:   (() => { console.log("run"); })();
来源：http://tjn.yuanzhike.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yjz.shzxlz.cn

Go:   func() { fmt.Println("run") }()
来源：http://khn.guannengcc.top

Ruby: -> { puts "run" }.call
来源：http://asn.shzxlz.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://eji.gaohongyu789.top

[C13] 类型声明 / 类型注解
来源：http://had.cucudq.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://saf.gzhubu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wot.havefunace.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yqf.jiagoushi.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ean.jinqigufen.top

Java: int add(int a, int b) { return a + b; }
来源：http://pzi.nanxuanxn.top

Go:   func add(a, b int) int
来源：http://gye.zhaomingkeji.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://iri.chenlongwang.top

C#:   int Add(int a, int b) => a + b;
来源：http://ukw.zhixingplan.top

[C14] 泛型函数
来源：http://tex.aizwys.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://koq.yuxming.cn

PHP:  // 无泛型
来源：http://ngu.gogol.net.cn

JS:   // 无泛型
来源：http://sny.gogol.net.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://iuo.zhijiandao.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mld.zdbjq.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://iip.pengpengdd.cyou

Ruby: # 无泛型
来源：http://fyp.zdqjudy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bgr.zycfv.cn

[C15] 解构 / 展开参数
来源：http://zvm.tanke756.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ogj.uphjek.com

PHP:  [$a, $b] = $pair;
来源：http://irr.52xcode.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zar.shzxlz.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jod.hesvh.cn

Java: // 无解构
来源：http://rwd.chenlongwang.top

Go:   // 无解构
来源：http://huh.zhoulong.xyz

Ruby: a, b = pair
来源：http://fly.tianlin.xyz

C#:   var (a, b) = pair;
来源：http://nud.hongshengwenyu.top

[C16] 函数 / 方法重载
来源：http://tzw.zdqjudy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kab.52xcode.cn

PHP:  // 无重载
来源：http://ajo.vqdsnc.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://rsc.jiagoushi.top

TS:   // 用联合类型或重载签名声明
来源：http://nao.yongpay.top

Java: void f(int a) {}  void f(String a) {}
来源：http://xni.meibo888.top

Go:   // 无重载：用不同函数名
来源：http://lmy.yangfankeji.com

Ruby: # 无重载：靠动态参数
来源：http://szq.xingfuxueyuan.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://woa.fehbvm.com

================================================================================
来源：http://lrh.fktsv.cn

D. 数组 / 列表 / 集合
来源：http://xch.shanyushiyangtech.top

================================================================================
来源：http://ovi.ydjk.org.cn

[D01] 创建数组 / 列表
来源：http://jae.daria6918.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://izo.0kj1m.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ncj.tian-w.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bdr.yueranfly.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://cmc.gogol.net.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pos.bbcook.cn

Go:   arr := []int{1, 2, 3}
来源：http://kwq.quarkkingdee.top

Ruby: arr = [1, 2, 3]
来源：http://fva.zhongyouzk.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mbt.uphjek.com

[D02] 追加元素到末尾
来源：http://xws.jinyuanbaomall.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vat.cqqwz.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rgr.xinyue.icu

JS:   arr.push(4);
来源：http://vna.wangdashe.top

TS:   arr.push(4);
来源：http://qqu.ydjk.org.cn

Java: list.add(4);
来源：http://vct.redwolf501.top

Go:   arr = append(arr, 4)
来源：http://fee.snrcjt.cn

Ruby: arr << 4; arr.push(5)
来源：http://ulo.aizwys.cn

C#:   list.Add(4);
来源：http://gtv.yueranfly.top

[D03] 在指定位置插入元素
来源：http://hhh.tanke756.top

Py:   arr.insert(0, 0)
来源：http://noc.316326.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rqg.hcnkem.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pay.tanke756.top

TS:   arr.splice(0, 0, 0);
来源：http://qei.c1oappe.top

Java: list.add(0, 0);
来源：http://owu.daxiang520.top

Go:   arr = append([]int{0}, arr...)
来源：http://nla.pycfn.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yzq.chenzaomai.com

C#:   list.Insert(0, 0);
来源：http://arh.hnxiangtu.top

[D04] 删除元素
来源：http://fgd.daria6918.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ifj.nanxinkj.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xqk.ywan-chungtsiang.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xrn.jianghu66.top

TS:   arr.splice(0, 1);
来源：http://lrl.daria6918.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wah.guowangkeji.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://psq.gogol.net.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://udx.zhongyouzk.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://inw.birdmap.top

[D05] 访问与修改元素
来源：http://omb.jlsjyb.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bss.gzhubu.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ctv.gaohongyu789.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vss.pengpengdd.cyou

TS:   arr[0]; arr.at(-1);
来源：http://jcr.9152youxi.cn

Java: list.get(0); list.set(0, 9);
来源：http://lpz.tarul.cn

Go:   arr[0]; arr[0] = 9
来源：http://qkr.ivvv.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vkk.ehwqpu.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://oez.shzxlz.cn

[D06] 数组长度
来源：http://npf.tarul.cn

Py:   len(arr)
来源：http://bap.vqdsnc.cn

PHP:  count($arr);
来源：http://owo.hongshengwenyu.top

JS:   arr.length
来源：http://kkr.feifeiyinyue.top

TS:   arr.length
来源：http://eyt.hysaishi.cn

Java: list.size();
来源：http://gmy.9152youxi.cn

Go:   len(arr)
来源：http://efe.mhx1999.top

Ruby: arr.length; arr.size
来源：http://zuy.hammf.cn

C#:   list.Count;
来源：http://lkg.sxryk.cn

[D07] 切片 / 取子数组
来源：http://rqk.hesvh.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dra.yueranfly.top

PHP:  array_slice($arr, 1, 3);
来源：http://nmh.sysykeji.top

JS:   arr.slice(1, 4);
来源：http://ach.ppjwa.cn

TS:   arr.slice(1, 4);
来源：http://dcx.ehwqpu.com

Java: list.subList(1, 4);
来源：http://vuo.xuanzx.com

Go:   arr[1:4]
来源：http://hqj.shangyingyoupin.top

Ruby: arr[1, 3]
来源：http://rxz.fzhhl.top

C#:   list.GetRange(1, 3);
来源：http://xgm.bjfxy.top

[D08] 合并两个数组
来源：http://jwb.andypj.xyz

Py:   a + b;  a.extend(b)
来源：http://jnz.shangyingyoupin.top

PHP:  array_merge($a, $b);
来源：http://jis.xziqi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://dfz.redwolf501.top

TS:   [...a, ...b];
来源：http://hpb.gzhubu.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yqt.xylfe.cn

Go:   append(a, b...)
来源：http://lof.zhixingplan.top

Ruby: a + b;  a.concat(b)
来源：http://mhu.hnxiangtu.top

C#:   a.Concat(b).ToList()
来源：http://rsc.jinqigfzy.top

[D09] 排序（升序）
来源：http://hcx.redwolf501.top

Py:   sorted(arr);  arr.sort()
来源：http://tgb.ywan-chungtsiang.top

PHP:  sort($arr);
来源：http://pph.sjlbkw.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jxt.fktsv.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lmz.yueranfly.top

Java: Collections.sort(list);  list.sort(null);
来源：http://mrc.gotoacloud.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vkt.hesvh.cn

Ruby: arr.sort
来源：http://vjf.fzhhl.top

C#:   list.Sort();
来源：http://tqk.epnwcf.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://zif.uphjek.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zui.bbcook.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://utt.zhoulong.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ncp.yj20258888.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ezd.nanxinkj.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ndh.bjfxy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rhe.epnwcf.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ihf.hongshengwenyu.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cxn.hfpthk.cn

[D11] 反转数组
来源：http://nzv.hnqzz.top

Py:   arr[::-1];  arr.reverse()
来源：http://bjr.yongpay.top

PHP:  array_reverse($arr);
来源：http://hjm.fzhhl.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mdc.zycfv.cn

TS:   [...arr].reverse();
来源：http://lxc.jinqigufen.top

Java: Collections.reverse(list);
来源：http://ryx.wangdashe.top

Go:   slices.Reverse(arr)
来源：http://qyq.zdbjq.cn

Ruby: arr.reverse
来源：http://uvi.mhx1999.top

C#:   list.Reverse();
来源：http://zde.gaohongyu789.top

[D12] 查找元素下标
来源：http://riw.zhongyouzk.top

Py:   arr.index(x);  x in arr
来源：http://nld.fengsongda.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jlh.jiagoushi.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ylh.hnqzz.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://awf.yuanzhike.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lou.yj202588.top

Go:   slices.Index(arr, x)
来源：http://ogw.kuanghao11.cn

Ruby: arr.index(x)
来源：http://vrn.chenzaomai.com

C#:   list.IndexOf(x);
来源：http://wnw.sxryk.cn

[D13] 过滤（保留满足条件的）
来源：http://ygy.fanxiaobao.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://efo.zhixingplan.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jaf.yuxming.cn

JS:   arr.filter(x => x > 3)
来源：http://nqg.birdmap.top

TS:   arr.filter(x => x > 3)
来源：http://jla.hywenlv.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bmr.zhongyouzk.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vzm.zhijiandao.cn

Ruby: arr.select { |x| x > 3 }
来源：http://rxt.hongshengwenyu.top

C#:   list.Where(x => x > 3).ToList()
来源：http://aqj.aizwys.cn

[D14] 映射转换（每个元素变形）
来源：http://uar.tianlin.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kfi.smart0.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qdv.quarkkingdee.top

JS:   arr.map(x => x * 2)
来源：http://nbz.yangfankeji.com

TS:   arr.map(x => x * 2)
来源：http://gyd.shanyushiyangkeji.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://qnf.xuanzx.com

Go:   // 手写循环
来源：http://lei.hongshengwenyu.top

Ruby: arr.map { |x| x * 2 }
来源：http://kzb.dianchejie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://esc.jlsjyb.cn

[D15] 去重
来源：http://mmx.cheryme.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tyt.shuidangran.top

PHP:  array_unique($arr);
来源：http://sgu.ppjwa.cn

JS:   [...new Set(arr)]
来源：http://qny.svipenyu.cn


<!-- 参考信息 -->
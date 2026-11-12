代发 wailian999

C#:   x is int or double or decimal
来源：http://vvp.hnxiangtu.top

[B14] 判断值是否在集合内
来源：http://uzf.shuidangran.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mgx.xuetiantiany.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kar.vqdsnc.cn

JS:   [1, 2, 3].includes(x)
来源：http://ztt.aizwys.cn

TS:   [1, 2, 3].includes(x)
来源：http://xdo.hammf.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://yps.hysaishi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dlu.gzhubu.top

Ruby: [1, 2, 3].include?(x)
来源：http://edw.aibaodan.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://luv.cheryme.top

[B15] 布尔运算与取反
来源：http://qqj.hywenlv.cn

Py:   a and b or not c
来源：http://jnt.iojbl.cn

PHP:  $a && $b || !$c
来源：http://sli.wangshuangyany.cn

JS:   a && b || !c
来源：http://rpr.jinyuanbaomall.cn

TS:   a && b || !c
来源：http://eko.pycfn.com

Java: a && b || !c
来源：http://htc.316326.xyz

Go:   a && b || !c
来源：http://uol.nwbrower.top

Ruby: a && b || !c
来源：http://afq.bbcook.cn

C#:   a && b || !c
来源：http://ayl.aizwys.cn

[B16] 卫语句：不满足条件提前返回
来源：http://dos.mhx1999.top

Py:   if not data: return
来源：http://gwi.cheryme.top

PHP:  if (!$data) { return; }
来源：http://otn.xingfuxueyuan.xyz

JS:   if (!data) return;
来源：http://enl.hywenlv.cn

TS:   if (!data) return;
来源：http://zdx.hammf.cn

Java: if (data == null) return;
来源：http://xvi.zhaomingkeji.xyz

Go:   if data == nil { return }
来源：http://bsl.sjlbkw.cn

Ruby: return if data.nil?
来源：http://iln.yuanzhike.top

C#:   if (data == null) return;
来源：http://ngt.yangfankeji.com

================================================================================
来源：http://kyv.fanxiaobao.xyz

C. 函数与作用域
来源：http://qai.xinyue.icu

================================================================================
来源：http://rwn.svipenyu.cn

[C01] 定义函数
来源：http://zhz.jiagoushi.top

Py:   def add(a, b): return a + b
来源：http://ypx.cqqwz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hwy.9152youxi.cn

JS:   function add(a, b) { return a + b; }
来源：http://dei.daria6918.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pnb.sweek.top

Java: static int add(int a, int b) { return a + b; }
来源：http://rek.yvedp.cn

Go:   func add(a, b int) int { return a + b }
来源：http://cun.bjfxy.top

Ruby: def add(a, b); a + b; end
来源：http://qdg.smart0.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gxy.shangyingyoupin.top

[C02] 默认参数
来源：http://zka.redwolf501.top

Py:   def greet(name="World"): return name
来源：http://itr.birdmap.top

PHP:  function greet($name = "World") { return $name; }
来源：http://twe.xinyue.icu

JS:   function greet(name = "World") { return name; }
来源：http://jqs.jinqigufen.top

TS:   function greet(name: string = "World") { return name; }
来源：http://iei.feifeiyinyue.top

Java: // 无默认参数：方法重载或 Optional
来源：http://tuo.shanyushiyangkeji.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://uvj.cucudq.cn

Ruby: def greet(name = "World") = name
来源：http://pjo.gogol.net.cn

C#:   string Greet(string name = "World") => name;
来源：http://pmp.xziqi.cn

[C03] 可变参数
来源：http://oiz.vehdjk.com

Py:   def total(*args): return sum(args)
来源：http://btc.birdmap.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nbq.ydzc1.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ysz.tianlin.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ljb.fehbvm.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jii.jyoumei.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kpa.52xcode.cn

Ruby: def total(*nums); nums.sum; end
来源：http://tzi.andypj.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qot.tianlin.xyz

[C04] 命名参数 / 关键字参数
来源：http://iuy.nanxinkj.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hnn.shuidangran.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://utc.hnqzz.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://eho.gaohongyu789.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hkx.jinqigufen.top

Java: // 无：用 Builder 模式或 record
来源：http://mjg.zhijiandao.cn

Go:   // 无：用配置结构体参数
来源：http://yrl.sufxvd.cn

Ruby: f(a: 1, b: 2)
来源：http://pai.shanyushiyangkeji.top

C#:   f(a: 1, b: 2)
来源：http://ahs.chenzaomai.com

[C05] 返回多个值
来源：http://ovi.dianchejie.cn

Py:   return a, b
来源：http://woc.ydjk.org.cn

PHP:  return [$a, $b];
来源：http://skt.aizwys.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://isz.tian-w.cn

TS:   return { a, b };
来源：http://cnf.birdmap.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zwa.yuanzhike.top

Go:   return a, b
来源：http://tph.yj20258.top

Ruby: return a, b
来源：http://mgh.kuanghao11.cn

C#:   return (a, b);              // ValueTuple
来源：http://bws.hnqzz.top

[C06] 匿名函数 / lambda
来源：http://ueh.jinqigfzy.top

Py:   square = lambda x: x * x
来源：http://rfb.feifeiyinyue.top

PHP:  $square = fn($x) => $x * $x;
来源：http://qlu.sweek.top

JS:   const square = x => x * x;
来源：http://vil.gogol.net.cn

TS:   const square = (x: number): number => x * x;
来源：http://eqm.zhijiandao.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lcw.hywenlv.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jth.aizwys.cn

Ruby: square = ->(x) { x * x }
来源：http://uzz.sweek.top

C#:   Func<int, int> square = x => x * x;
来源：http://qej.iojbl.cn

[C07] 把函数作为参数传入
来源：http://yrn.yueranfly.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kyi.zdqjudy.top

PHP:  array_map("strtoupper", $arr);
来源：http://udw.ybcxt.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ttc.daria6918.cn

TS:   arr.map(String)
来源：http://fcq.ydzc1.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://afn.yuanzhike.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tha.sjlbkw.cn

Ruby: arr.map(&:upcase)
来源：http://rkg.cucudq.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fmj.snrcjt.cn

[C08] 闭包
来源：http://gpm.chenjidiqi.icu

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tmw.shanyushiyangkeji.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://avm.aibaodan.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qdt.shangyingyoupin.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kpw.zdbjq.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ekm.smart0.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jbr.yj202588.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uhw.fengsongda.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bqg.sufxvd.cn

[C09] 递归
来源：http://vet.wangdashe.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hdk.ppjwa.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nok.zhixingplan.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bqi.ctjpmb.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eqc.guowangkeji.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jbs.guowangkeji.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://oig.ppjwa.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ryl.ehwqpu.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nwk.aizwys.cn

[C10] 变量作用域
来源：http://cyj.aizwys.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xzz.gzhubu.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rdx.hcnkem.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vbx.hesvh.cn

TS:   同 JS
来源：http://qvi.ivvv.top

Java: 方法内为块级作用域
来源：http://lvh.fehbvm.com

Go:   花括号块级作用域
来源：http://bhy.c1oappe.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dsc.guannengcc.top

C#:   块级作用域
来源：http://kyl.zhijiandao.cn

[C11] 模块导入与导出
来源：http://bwb.yongpay.top

Py:   from module import func
来源：http://ugd.zhongyouzk.top

PHP:  require "file.php";  或 use App\Service;
来源：http://fau.kuanghao11.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ode.52xcode.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fqm.yonumen.top

Java: import java.util.List;
来源：http://eii.ctjpmb.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xhq.316326.xyz

Ruby: require "json"; require_relative "./util"
来源：http://oih.vehdjk.com

C#:   using System.Text;
来源：http://jsk.mhx1999.top

[C12] 立即执行函数 IIFE
来源：http://xja.chenzaomai.com

Py:   (lambda: print("run"))()
来源：http://ugo.aizwys.cn

PHP:  (function () { echo "run"; })();
来源：http://tbo.gaohongyu789.top

JS:   (() => { console.log("run"); })();
来源：http://oko.hnqzz.top

TS:   (() => { console.log("run"); })();
来源：http://ubu.zhoulong.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bcs.fktsv.cn

Go:   func() { fmt.Println("run") }()
来源：http://mam.zycfv.cn

Ruby: -> { puts "run" }.call
来源：http://jkt.316326.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://scn.52xcode.cn

[C13] 类型声明 / 类型注解
来源：http://sal.vqdsnc.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://znm.hywenlv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qsh.nanxuanxn.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vrf.snrcjt.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bol.sjlbkw.cn

Java: int add(int a, int b) { return a + b; }
来源：http://lrm.wangshuangyany.cn

Go:   func add(a, b int) int
来源：http://qmt.fanxiaobao.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ucd.chenzaomai.com

C#:   int Add(int a, int b) => a + b;
来源：http://hzp.316326.xyz

[C14] 泛型函数
来源：http://mkg.daxiang520.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://plj.smart0.xyz

PHP:  // 无泛型
来源：http://iof.zhiwuduotai.top

JS:   // 无泛型
来源：http://gmu.bjfxy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sdq.wangdashe.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zqo.xylfe.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://uxc.kuanghao11.cn

Ruby: # 无泛型
来源：http://mti.zhongyouzk.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ysj.dianchejie.cn

[C15] 解构 / 展开参数
来源：http://cwe.birdmap.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://snb.xylfe.cn

PHP:  [$a, $b] = $pair;
来源：http://ozd.52xcode.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://khi.sufxvd.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uni.dianchejie.cn

Java: // 无解构
来源：http://pyt.nanxuanxn.top

Go:   // 无解构
来源：http://awy.zycfv.cn

Ruby: a, b = pair
来源：http://ywi.xylfe.cn

C#:   var (a, b) = pair;
来源：http://fto.0kj1m.cn

[C16] 函数 / 方法重载
来源：http://vol.daria6918.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ryp.yfazqb.com

PHP:  // 无重载
来源：http://hxn.0kj1m.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://mrl.ivvv.top

TS:   // 用联合类型或重载签名声明
来源：http://vdk.xuanzx.com

Java: void f(int a) {}  void f(String a) {}
来源：http://ytn.xingfuxueyuan.xyz

Go:   // 无重载：用不同函数名
来源：http://vjw.chenzaomai.com

Ruby: # 无重载：靠动态参数
来源：http://rer.chenlongwang.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://fnn.ctjpmb.com

================================================================================
来源：http://bgs.gotoacloud.top

D. 数组 / 列表 / 集合
来源：http://uxu.havefunace.top

================================================================================
来源：http://xyy.ehwqpu.com

[D01] 创建数组 / 列表
来源：http://amr.redwolf501.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://udz.hcnkem.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tyv.jianghu66.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://oed.nanxuanxn.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://zqu.9152youxi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://obo.jianghu66.top

Go:   arr := []int{1, 2, 3}
来源：http://byv.hnxiangtu.top

Ruby: arr = [1, 2, 3]
来源：http://owm.yanxiufei.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://oqd.shzxlz.cn

[D02] 追加元素到末尾
来源：http://hje.jqgufenzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://oyl.jiagoushi.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bxn.bjfxy.top

JS:   arr.push(4);
来源：http://nka.fengsongda.top

TS:   arr.push(4);
来源：http://ebh.jinqigufen.top

Java: list.add(4);
来源：http://pvl.dashuyun.cn

Go:   arr = append(arr, 4)
来源：http://hxj.zhoulong.xyz

Ruby: arr << 4; arr.push(5)
来源：http://bdn.zhaomingkeji.xyz

C#:   list.Add(4);
来源：http://lxn.snrcjt.cn

[D03] 在指定位置插入元素
来源：http://qfw.pengpengdd.cyou

Py:   arr.insert(0, 0)
来源：http://aik.hnxiangtu.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zlc.xziqi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ylv.zhaomingkeji.xyz

TS:   arr.splice(0, 0, 0);
来源：http://uxp.chenjidiqi.icu

Java: list.add(0, 0);
来源：http://nle.cdnleiting.top

Go:   arr = append([]int{0}, arr...)
来源：http://zhx.yfazqb.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qmi.feifeiyinyue.top

C#:   list.Insert(0, 0);
来源：http://zmo.xuanzx.com

[D04] 删除元素
来源：http://rwz.sxryk.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wvx.zdbjq.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zxh.hesvh.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gwf.sysykeji.top

TS:   arr.splice(0, 1);
来源：http://yuh.fengsongda.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gjr.haohaochexian.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xzl.yfazqb.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jqw.guowangkeji.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://oyy.jyoumei.cn

[D05] 访问与修改元素
来源：http://lco.kuanghao11.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://agp.zhoulong.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://aie.yvedp.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ont.xziqi.cn

TS:   arr[0]; arr.at(-1);
来源：http://vvx.chenzaomai.com

Java: list.get(0); list.set(0, 9);
来源：http://afu.jianghu66.top

Go:   arr[0]; arr[0] = 9
来源：http://sef.sysykeji.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://crk.jinqigfzy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cby.jiagoushi.top

[D06] 数组长度
来源：http://aht.fehbvm.com

Py:   len(arr)
来源：http://way.yuxming.cn

PHP:  count($arr);
来源：http://yba.jianghu66.top

JS:   arr.length
来源：http://flm.hnqzz.top

TS:   arr.length
来源：http://hfq.cdnleiting.top

Java: list.size();
来源：http://jjc.zycfv.cn

Go:   len(arr)
来源：http://bvr.cqqwz.cn

Ruby: arr.length; arr.size
来源：http://tik.gogol.net.cn

C#:   list.Count;
来源：http://rsh.mhx1999.top

[D07] 切片 / 取子数组
来源：http://zcn.bbcook.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pra.yj202588.top

PHP:  array_slice($arr, 1, 3);
来源：http://fze.andypj.xyz

JS:   arr.slice(1, 4);
来源：http://miw.feifeiyinyue.top

TS:   arr.slice(1, 4);
来源：http://puq.vehdjk.com

Java: list.subList(1, 4);
来源：http://rvq.bbcook.cn

Go:   arr[1:4]
来源：http://hxv.iojbl.cn

Ruby: arr[1, 3]
来源：http://jyw.nanxinkj.top

C#:   list.GetRange(1, 3);
来源：http://nqt.epnwcf.com

[D08] 合并两个数组
来源：http://koe.bbcook.cn

Py:   a + b;  a.extend(b)
来源：http://tud.snrcjt.cn

PHP:  array_merge($a, $b);
来源：http://uhw.shangyingyoupin.top

JS:   [...a, ...b];  a.concat(b);
来源：http://kxj.redwolf501.top

TS:   [...a, ...b];
来源：http://xhm.dianchejie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gpr.zhengqikj.top

Go:   append(a, b...)
来源：http://elp.yongpay.top

Ruby: a + b;  a.concat(b)
来源：http://vam.yvedp.cn

C#:   a.Concat(b).ToList()
来源：http://vlu.guowangkeji.top

[D09] 排序（升序）
来源：http://nem.tarul.cn

Py:   sorted(arr);  arr.sort()
来源：http://rot.xuanzx.com

PHP:  sort($arr);
来源：http://dda.hongshengwenyu.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dqy.cucudq.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://rrf.cheryme.top

Java: Collections.sort(list);  list.sort(null);
来源：http://qeh.wangshuangyany.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zxl.chenzaomai.com

Ruby: arr.sort
来源：http://gan.hammf.cn

C#:   list.Sort();
来源：http://rwe.zdbjq.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://aax.cqqwz.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bwd.pycfn.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hoo.xinyue.icu

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wvs.yonumen.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lgy.xylfe.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dhf.yj202588.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rwz.redwolf501.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://grg.havefunace.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://etk.bjfxy.top

[D11] 反转数组
来源：http://ybm.zhijiandao.cn

Py:   arr[::-1];  arr.reverse()
来源：http://cwt.0kj1m.cn

PHP:  array_reverse($arr);
来源：http://csd.cucudq.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zdo.xuanzx.com

TS:   [...arr].reverse();
来源：http://ftx.xinyue.icu

Java: Collections.reverse(list);
来源：http://tsh.cqqwz.cn

Go:   slices.Reverse(arr)
来源：http://zmr.fktsv.cn

Ruby: arr.reverse
来源：http://ygk.zhaomingkeji.xyz

C#:   list.Reverse();
来源：http://hgw.sxryk.cn

[D12] 查找元素下标
来源：http://qke.jinqigufen.top

Py:   arr.index(x);  x in arr
来源：http://gol.sysykeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lbp.jqgufenzy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ory.fanxiaobao.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fmx.jqgfzy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bzz.vehdjk.com

Go:   slices.Index(arr, x)
来源：http://ydc.fktsv.cn

Ruby: arr.index(x)
来源：http://pke.xylfe.cn

C#:   list.IndexOf(x);
来源：http://xmy.xuanzx.com

[D13] 过滤（保留满足条件的）
来源：http://ooh.gzhubu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sps.ctjpmb.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://axx.yuanzhike.top

JS:   arr.filter(x => x > 3)
来源：http://mqt.jlsjyb.cn

TS:   arr.filter(x => x > 3)
来源：http://pyl.jianghu66.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fyj.dianchejie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://quz.dashuyun.cn

Ruby: arr.select { |x| x > 3 }
来源：http://gju.smart0.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://tbk.haohaochexian.top

[D14] 映射转换（每个元素变形）
来源：http://lcp.jyoumei.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://png.feifeiyinyue.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tuu.hnxiangtu.top

JS:   arr.map(x => x * 2)
来源：http://iap.hesvh.cn

TS:   arr.map(x => x * 2)
来源：http://kgf.yfazqb.com


<!-- 参考信息 -->
代发 wailian999

[B13] 判断是否为数字
来源：http://srv.fengsongda.top

Py:   isinstance(x, (int, float))
来源：http://evq.yj202588.top

PHP:  is_numeric($x)
来源：http://vur.epnwcf.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mdb.hesvh.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ruq.aibaodan.cn

Java: x instanceof Number
来源：http://eja.jinyuanbaomall.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://iqo.yuxming.cn

Ruby: x.is_a?(Numeric)
来源：http://qny.yueranfly.top

C#:   x is int or double or decimal
来源：http://rqv.cucudq.cn

[B14] 判断值是否在集合内
来源：http://uzq.cucudq.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vtt.ppjwa.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://uug.gogol.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://utr.aizwys.cn

TS:   [1, 2, 3].includes(x)
来源：http://hxj.zhengqikj.top

Java: List.of(1, 2, 3).contains(x)
来源：http://yvg.yangfankeji.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://uti.tarul.cn

Ruby: [1, 2, 3].include?(x)
来源：http://hcq.hammf.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://itf.chenjidiqi.icu

[B15] 布尔运算与取反
来源：http://swm.chenzaomai.com

Py:   a and b or not c
来源：http://rzi.wangdashe.top

PHP:  $a && $b || !$c
来源：http://ofh.fktsv.cn

JS:   a && b || !c
来源：http://utq.cucudq.cn

TS:   a && b || !c
来源：http://esy.ydjk.org.cn

Java: a && b || !c
来源：http://owq.yongpay.top

Go:   a && b || !c
来源：http://zue.gzhubu.top

Ruby: a && b || !c
来源：http://ydx.yonumen.top

C#:   a && b || !c
来源：http://iww.iojbl.cn

[B16] 卫语句：不满足条件提前返回
来源：http://kvk.bbcook.cn

Py:   if not data: return
来源：http://fhe.yangfankeji.com

PHP:  if (!$data) { return; }
来源：http://ali.jqgfzy.top

JS:   if (!data) return;
来源：http://gel.xziqi.cn

TS:   if (!data) return;
来源：http://lpp.bbcook.cn

Java: if (data == null) return;
来源：http://vgi.daria6918.cn

Go:   if data == nil { return }
来源：http://jrx.fktsv.cn

Ruby: return if data.nil?
来源：http://azu.zhijiandao.cn

C#:   if (data == null) return;
来源：http://bwa.zhengqikj.top

================================================================================
来源：http://ydl.shanyushiyangtech.top

C. 函数与作用域
来源：http://hpy.daxiang520.top

================================================================================
来源：http://oyp.hnxiangtu.top

[C01] 定义函数
来源：http://lfi.dashuyun.cn

Py:   def add(a, b): return a + b
来源：http://bjx.jianghu66.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zxf.iojbl.cn

JS:   function add(a, b) { return a + b; }
来源：http://gyj.sysykeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ftk.cucudq.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://sjd.dianchejie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://udn.jyoumei.cn

Ruby: def add(a, b); a + b; end
来源：http://zpv.hysaishi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zyy.hysaishi.cn

[C02] 默认参数
来源：http://vfj.jiagoushi.top

Py:   def greet(name="World"): return name
来源：http://izj.ivvv.top

PHP:  function greet($name = "World") { return $name; }
来源：http://onl.nanxinkj.top

JS:   function greet(name = "World") { return name; }
来源：http://rde.sxryk.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qcq.xziqi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://uxv.aibaodan.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kei.epnwcf.com

Ruby: def greet(name = "World") = name
来源：http://gya.zhoulong.xyz

C#:   string Greet(string name = "World") => name;
来源：http://euo.shangyingyoupin.top

[C03] 可变参数
来源：http://xuc.chenzaomai.com

Py:   def total(*args): return sum(args)
来源：http://fdf.ywan-chungtsiang.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tnx.bjfxy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://aad.yj20258.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qkj.gogol.net.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rqv.zhoulong.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://egp.daria6918.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ugr.hywenlv.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vyr.jianghu66.top

[C04] 命名参数 / 关键字参数
来源：http://kui.andypj.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hqd.316326.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gpf.zhijiandao.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uhn.aizwys.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://imn.daria6918.cn

Java: // 无：用 Builder 模式或 record
来源：http://usj.guowangkeji.top

Go:   // 无：用配置结构体参数
来源：http://mce.chenzaomai.com

Ruby: f(a: 1, b: 2)
来源：http://txs.xziqi.cn

C#:   f(a: 1, b: 2)
来源：http://ric.xylfe.cn

[C05] 返回多个值
来源：http://tgv.pycfn.com

Py:   return a, b
来源：http://seb.feifeiyinyue.top

PHP:  return [$a, $b];
来源：http://tfg.shzxlz.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://gog.dashuyun.cn

TS:   return { a, b };
来源：http://fmd.ydjk.org.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zzh.c1oappe.top

Go:   return a, b
来源：http://pvb.fzhhl.top

Ruby: return a, b
来源：http://bnr.yuxming.cn

C#:   return (a, b);              // ValueTuple
来源：http://vra.sufxvd.cn

[C06] 匿名函数 / lambda
来源：http://mqh.cashguo.top

Py:   square = lambda x: x * x
来源：http://fyf.fanxiaobao.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://vtx.xuanzx.com

JS:   const square = x => x * x;
来源：http://ras.tarul.cn

TS:   const square = (x: number): number => x * x;
来源：http://fak.ppjwa.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xpc.xinyue.icu

Go:   sq := func(x int) int { return x * x }
来源：http://ucd.ehwqpu.com

Ruby: square = ->(x) { x * x }
来源：http://dby.jinqigfzy.top

C#:   Func<int, int> square = x => x * x;
来源：http://zyo.xinyue.icu

[C07] 把函数作为参数传入
来源：http://qzn.xuetiantiany.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cod.zhijiandao.cn

PHP:  array_map("strtoupper", $arr);
来源：http://yhy.fanxiaobao.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wjb.hcnkem.com

TS:   arr.map(String)
来源：http://mdm.yfazqb.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wcw.sweek.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sfy.gotoacloud.top

Ruby: arr.map(&:upcase)
来源：http://tes.jinqigufen.top

C#:   arr.Select(s => s.ToUpper())
来源：http://efv.zdbjq.cn

[C08] 闭包
来源：http://bvb.wangshuangyany.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mrn.gzhubu.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xgi.hammf.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nwp.sweek.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ksa.hammf.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zuk.hnxiangtu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kdy.svipenyu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cwk.tian-w.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nod.zhixingplan.top

[C09] 递归
来源：http://xlt.hfpthk.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ubj.shanyushiyangkeji.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rab.iojbl.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mcz.daxiang520.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://guy.chenzaomai.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fog.hammf.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tdo.fengsongda.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mis.gotoacloud.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://onl.hywenlv.cn

[C10] 变量作用域
来源：http://iyf.0kj1m.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://out.shanyushiyangtech.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bki.nwbrower.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ptc.jlsjyb.cn

TS:   同 JS
来源：http://eee.daxiang520.top

Java: 方法内为块级作用域
来源：http://ote.cucudq.cn

Go:   花括号块级作用域
来源：http://gmr.hfpthk.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lig.ybcxt.top

C#:   块级作用域
来源：http://ram.zhongyouzk.top

[C11] 模块导入与导出
来源：http://yuh.yanxiufei.cn

Py:   from module import func
来源：http://kss.tian-w.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://een.redwolf501.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://epd.ivvv.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jyk.chenjidiqi.icu

Java: import java.util.List;
来源：http://frv.zhoulong.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ndu.haohaochexian.top

Ruby: require "json"; require_relative "./util"
来源：http://rdb.pengpengdd.cyou

C#:   using System.Text;
来源：http://qwt.nanxinkj.top

[C12] 立即执行函数 IIFE
来源：http://lbd.sysykeji.top

Py:   (lambda: print("run"))()
来源：http://slu.sjlbkw.cn

PHP:  (function () { echo "run"; })();
来源：http://ymb.zdbjq.cn

JS:   (() => { console.log("run"); })();
来源：http://ykt.zdqjudy.top

TS:   (() => { console.log("run"); })();
来源：http://lgc.zhijiandao.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ywk.jinqigfzy.top

Go:   func() { fmt.Println("run") }()
来源：http://lyf.yanxiufei.cn

Ruby: -> { puts "run" }.call
来源：http://xgg.zycfv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://odb.ybcxt.top

[C13] 类型声明 / 类型注解
来源：http://jkp.yongpay.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tab.havefunace.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bpm.epnwcf.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://heh.sweek.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bvt.sweek.top

Java: int add(int a, int b) { return a + b; }
来源：http://pho.zhoulong.xyz

Go:   func add(a, b int) int
来源：http://hiu.gogol.net.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zdv.316326.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://iza.tanke756.top

[C14] 泛型函数
来源：http://vgy.shanyushiyangtech.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hnm.zycfv.cn

PHP:  // 无泛型
来源：http://mro.sufxvd.cn

JS:   // 无泛型
来源：http://otz.tanke756.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ihg.wangdashe.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://irr.zhoulong.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://our.shangyingyoupin.top

Ruby: # 无泛型
来源：http://asn.zhengqikj.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://drf.nwbrower.top

[C15] 解构 / 展开参数
来源：http://saj.tanke756.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://agc.52xcode.cn

PHP:  [$a, $b] = $pair;
来源：http://num.hnqzz.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vgl.hongshengwenyu.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hmg.hongshengwenyu.top

Java: // 无解构
来源：http://zvf.316326.xyz

Go:   // 无解构
来源：http://rte.svipenyu.cn

Ruby: a, b = pair
来源：http://fjd.cdnleiting.top

C#:   var (a, b) = pair;
来源：http://dde.wangshuangyany.cn

[C16] 函数 / 方法重载
来源：http://qqb.yj202588.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://frz.haohaochexian.top

PHP:  // 无重载
来源：http://ywo.vqdsnc.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://tew.zhaomingkeji.xyz

TS:   // 用联合类型或重载签名声明
来源：http://jcx.havefunace.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ncj.jqgfzy.top

Go:   // 无重载：用不同函数名
来源：http://ysx.yj20258888.top

Ruby: # 无重载：靠动态参数
来源：http://yts.fktsv.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zhr.xingfuxueyuan.xyz

================================================================================
来源：http://oky.jlsjyb.cn

D. 数组 / 列表 / 集合
来源：http://mur.zdqjudy.top

================================================================================
来源：http://amk.fehbvm.com

[D01] 创建数组 / 列表
来源：http://kns.xinyue.icu

Py:   arr = [1, 2, 3];  empty = []
来源：http://zct.52xcode.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://evq.dashuyun.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://psb.9152youxi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://arn.ydjk.org.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qgx.sufxvd.cn

Go:   arr := []int{1, 2, 3}
来源：http://nsd.shzxlz.cn

Ruby: arr = [1, 2, 3]
来源：http://xdz.aizwys.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sqo.pycfn.com

[D02] 追加元素到末尾
来源：http://fap.jianghu66.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kfs.kuanghao11.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://exe.redwolf501.top

JS:   arr.push(4);
来源：http://waa.jlsjyb.cn

TS:   arr.push(4);
来源：http://nkr.xylfe.cn

Java: list.add(4);
来源：http://esw.wangdashe.top

Go:   arr = append(arr, 4)
来源：http://ukp.jinyuanbaomall.cn

Ruby: arr << 4; arr.push(5)
来源：http://hbh.gaohongyu789.top

C#:   list.Add(4);
来源：http://xfj.svipenyu.cn

[D03] 在指定位置插入元素
来源：http://ynn.yangfankeji.com

Py:   arr.insert(0, 0)
来源：http://qpr.0kj1m.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vns.shanyushiyangtech.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vgp.bjfxy.top

TS:   arr.splice(0, 0, 0);
来源：http://uab.vehdjk.com

Java: list.add(0, 0);
来源：http://dxz.jinyuanbaomall.cn

Go:   arr = append([]int{0}, arr...)
来源：http://pig.ehwqpu.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jdy.fzhhl.top

C#:   list.Insert(0, 0);
来源：http://uoh.zhiwuduotai.top

[D04] 删除元素
来源：http://eqp.xingfuxueyuan.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://eoy.xuanzx.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vmt.bbcook.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wik.bjfxy.top

TS:   arr.splice(0, 1);
来源：http://vpk.chenzaomai.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://znu.xuetiantiany.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yui.ehwqpu.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rby.zhixingplan.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tbk.yongpay.top

[D05] 访问与修改元素
来源：http://zkk.mhx1999.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ggv.yj20258888.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://eqy.dianchejie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pyb.zhixingplan.top

TS:   arr[0]; arr.at(-1);
来源：http://cus.daria6918.cn

Java: list.get(0); list.set(0, 9);
来源：http://slu.dianchejie.cn

Go:   arr[0]; arr[0] = 9
来源：http://fie.haohaochexian.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jqg.yj202588.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dhb.ehwqpu.com

[D06] 数组长度
来源：http://avf.havefunace.top

Py:   len(arr)
来源：http://ezb.tarul.cn

PHP:  count($arr);
来源：http://znu.iojbl.cn

JS:   arr.length
来源：http://efu.wangshuangyany.cn

TS:   arr.length
来源：http://gwy.gogol.net.cn

Java: list.size();
来源：http://gvk.zdbjq.cn

Go:   len(arr)
来源：http://fxf.gzhubu.top

Ruby: arr.length; arr.size
来源：http://ald.jlsjyb.cn

C#:   list.Count;
来源：http://edy.daria6918.cn

[D07] 切片 / 取子数组
来源：http://vcj.xuetiantiany.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rqz.shangyingyoupin.top

PHP:  array_slice($arr, 1, 3);
来源：http://pyv.ehwqpu.com

JS:   arr.slice(1, 4);
来源：http://oee.dashuyun.cn

TS:   arr.slice(1, 4);
来源：http://wze.ivvv.top

Java: list.subList(1, 4);
来源：http://aom.yvedp.cn

Go:   arr[1:4]
来源：http://sfe.yj20258.top

Ruby: arr[1, 3]
来源：http://yna.wangdashe.top

C#:   list.GetRange(1, 3);
来源：http://ugr.xziqi.cn

[D08] 合并两个数组
来源：http://cen.jiagoushi.top

Py:   a + b;  a.extend(b)
来源：http://ofp.fanxiaobao.xyz

PHP:  array_merge($a, $b);
来源：http://jhw.xingfuxueyuan.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://fjs.guowangkeji.top

TS:   [...a, ...b];
来源：http://obn.yuanzhike.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ruj.xuanzx.com

Go:   append(a, b...)
来源：http://xhm.jinqigufen.top

Ruby: a + b;  a.concat(b)
来源：http://nzo.fanxiaobao.xyz

C#:   a.Concat(b).ToList()
来源：http://bji.zhiwuduotai.top

[D09] 排序（升序）
来源：http://qqj.daria6918.cn

Py:   sorted(arr);  arr.sort()
来源：http://vqw.sjlbkw.cn

PHP:  sort($arr);
来源：http://ckf.shuidangran.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hbq.9152youxi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ids.ywan-chungtsiang.top

Java: Collections.sort(list);  list.sort(null);
来源：http://nqf.shanyushiyangtech.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hxz.aibaodan.cn

Ruby: arr.sort
来源：http://uuj.ehwqpu.com

C#:   list.Sort();
来源：http://lks.wangdashe.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://rod.yvedp.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sxr.xylfe.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hug.hesvh.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dks.yuanzhike.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nkm.xuanzx.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zrm.xylfe.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vns.hywenlv.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://orv.sjlbkw.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wwj.zhoulong.xyz

[D11] 反转数组
来源：http://sah.guannengcc.top

Py:   arr[::-1];  arr.reverse()
来源：http://mew.vehdjk.com

PHP:  array_reverse($arr);
来源：http://skz.yvedp.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://klu.dashuyun.cn

TS:   [...arr].reverse();
来源：http://dhq.zdqjudy.top

Java: Collections.reverse(list);
来源：http://tmo.iojbl.cn

Go:   slices.Reverse(arr)
来源：http://sxx.zhaomingkeji.xyz

Ruby: arr.reverse
来源：http://krs.zhixingplan.top

C#:   list.Reverse();
来源：http://nad.jianghu66.top

[D12] 查找元素下标
来源：http://efp.yvedp.cn

Py:   arr.index(x);  x in arr
来源：http://zmm.ywan-chungtsiang.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://auc.hongshengwenyu.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qvc.ybcxt.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lnt.havefunace.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kof.shzxlz.cn

Go:   slices.Index(arr, x)
来源：http://trz.fengsongda.top

Ruby: arr.index(x)
来源：http://vjy.nanxinkj.top

C#:   list.IndexOf(x);
来源：http://igd.vehdjk.com

[D13] 过滤（保留满足条件的）
来源：http://ijb.jiagoushi.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bqf.tarul.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qcm.zdbjq.cn

JS:   arr.filter(x => x > 3)
来源：http://qeu.dashuyun.cn

TS:   arr.filter(x => x > 3)
来源：http://wle.quarkkingdee.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qej.zhaomingkeji.xyz


<!-- 参考信息 -->
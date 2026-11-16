代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://cfk.ybcxt.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://smy.shzxlz.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xob.ctjpmb.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qcq.yj202588.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://agx.xinyue.icu

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pks.hnxiangtu.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vvq.svipenyu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jhi.ydzc1.top

[B13] 判断是否为数字
来源：http://qbg.xinyue.icu

Py:   isinstance(x, (int, float))
来源：http://qbf.xuanzx.com

PHP:  is_numeric($x)
来源：http://xci.gzhubu.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ypg.gzhubu.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xee.hesvh.cn

Java: x instanceof Number
来源：http://lag.zhaomingkeji.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wad.dianchejie.cn

Ruby: x.is_a?(Numeric)
来源：http://ksu.ydzc1.top

C#:   x is int or double or decimal
来源：http://eeq.ivvv.top

[B14] 判断值是否在集合内
来源：http://klf.jinghuilouyu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ljz.pengpengdd.cyou

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wfc.zhoulong.xyz

JS:   [1, 2, 3].includes(x)
来源：http://lmp.0kj1m.cn

TS:   [1, 2, 3].includes(x)
来源：http://epi.jinghuilouyu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://shv.tarul.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://alz.hesvh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://hvg.sjlbkw.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rle.bjfxy.top

[B15] 布尔运算与取反
来源：http://fwm.cdnleiting.top

Py:   a and b or not c
来源：http://tsu.zhengqikj.top

PHP:  $a && $b || !$c
来源：http://fsn.ybcxt.top

JS:   a && b || !c
来源：http://ajj.iojbl.cn

TS:   a && b || !c
来源：http://dac.jiagoushi.top

Java: a && b || !c
来源：http://uum.zycfv.cn

Go:   a && b || !c
来源：http://plq.tianlin.xyz

Ruby: a && b || !c
来源：http://fmv.fengsongda.top

C#:   a && b || !c
来源：http://qsf.zhoulong.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://huk.sxryk.cn

Py:   if not data: return
来源：http://azm.havefunace.top

PHP:  if (!$data) { return; }
来源：http://xgf.shuidangran.top

JS:   if (!data) return;
来源：http://ity.aibaodan.cn

TS:   if (!data) return;
来源：http://qgf.cheryme.top

Java: if (data == null) return;
来源：http://lae.sjlbkw.cn

Go:   if data == nil { return }
来源：http://vyf.ydzc1.top

Ruby: return if data.nil?
来源：http://hyw.jyoumei.cn

C#:   if (data == null) return;
来源：http://run.yueranfly.top

================================================================================
来源：http://xqj.sufxvd.cn

C. 函数与作用域
来源：http://xte.yj20258888.top

================================================================================
来源：http://qkn.xylfe.cn

[C01] 定义函数
来源：http://rpw.gogol.net.cn

Py:   def add(a, b): return a + b
来源：http://oyr.ydzc1.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qyr.hongshengwenyu.top

JS:   function add(a, b) { return a + b; }
来源：http://flg.yj20258.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wat.zhengqikj.top

Java: static int add(int a, int b) { return a + b; }
来源：http://yic.bbcook.cn

Go:   func add(a, b int) int { return a + b }
来源：http://tbe.sufxvd.cn

Ruby: def add(a, b); a + b; end
来源：http://scg.shzxlz.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lvw.c1oappe.top

[C02] 默认参数
来源：http://wmn.yongpay.top

Py:   def greet(name="World"): return name
来源：http://ftw.sweek.top

PHP:  function greet($name = "World") { return $name; }
来源：http://nxd.yuxming.cn

JS:   function greet(name = "World") { return name; }
来源：http://vkz.hfpthk.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://bgi.nanxuanxn.top

Java: // 无默认参数：方法重载或 Optional
来源：http://urf.zhoulong.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ixl.52xcode.cn

Ruby: def greet(name = "World") = name
来源：http://bss.smart0.xyz

C#:   string Greet(string name = "World") => name;
来源：http://lkx.xingfuxueyuan.xyz

[C03] 可变参数
来源：http://ifo.yangfankeji.com

Py:   def total(*args): return sum(args)
来源：http://bxn.jianghu66.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://aeu.sufxvd.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zwb.birdmap.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://loi.quarkkingdee.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://evh.daxiang520.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fpm.wangdashe.top

Ruby: def total(*nums); nums.sum; end
来源：http://xqu.feifeiyinyue.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xck.daria6918.cn

[C04] 命名参数 / 关键字参数
来源：http://knp.jqgufenzy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ios.xziqi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bmu.chenlongwang.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lxa.fengsongda.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xuf.nanxuanxn.top

Java: // 无：用 Builder 模式或 record
来源：http://syf.jqgufenzy.top

Go:   // 无：用配置结构体参数
来源：http://mkv.nanxuanxn.top

Ruby: f(a: 1, b: 2)
来源：http://cor.wangdashe.top

C#:   f(a: 1, b: 2)
来源：http://kvh.cdnleiting.top

[C05] 返回多个值
来源：http://stf.jinqigufen.top

Py:   return a, b
来源：http://luz.hongshengwenyu.top

PHP:  return [$a, $b];
来源：http://sny.aibaodan.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://izq.yuanzhike.top

TS:   return { a, b };
来源：http://voh.vqdsnc.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xyb.xinyue.icu

Go:   return a, b
来源：http://cgp.dianchejie.cn

Ruby: return a, b
来源：http://exm.shuidangran.top

C#:   return (a, b);              // ValueTuple
来源：http://fyg.chenjidiqi.icu

[C06] 匿名函数 / lambda
来源：http://dlu.nanxinkj.top

Py:   square = lambda x: x * x
来源：http://xkx.ydzc1.top

PHP:  $square = fn($x) => $x * $x;
来源：http://zxr.zhixingplan.top

JS:   const square = x => x * x;
来源：http://myh.hysaishi.cn

TS:   const square = (x: number): number => x * x;
来源：http://vnj.xingfuxueyuan.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://idu.aizwys.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rvq.chenjidiqi.icu

Ruby: square = ->(x) { x * x }
来源：http://enq.jianghu66.top

C#:   Func<int, int> square = x => x * x;
来源：http://sqg.iojbl.cn

[C07] 把函数作为参数传入
来源：http://svg.c1oappe.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pfj.hywenlv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vbt.bjfxy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ysn.yj20258888.top

TS:   arr.map(String)
来源：http://mcm.yj20258888.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fcw.jinqigufen.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dea.fehbvm.com

Ruby: arr.map(&:upcase)
来源：http://osd.yj20258.top

C#:   arr.Select(s => s.ToUpper())
来源：http://eed.hnxiangtu.top

[C08] 闭包
来源：http://wkl.pycfn.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://eop.cdnleiting.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dtd.aibaodan.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ekv.ppjwa.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uqw.redwolf501.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jmn.jinghuilouyu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pyg.yj202588.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hvw.fanxiaobao.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xke.guowangkeji.top

[C09] 递归
来源：http://ery.uphjek.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jbw.chenjidiqi.icu

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://srl.zdbjq.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mse.chenlongwang.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aid.hongshengwenyu.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wde.fktsv.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uqw.sysykeji.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gkj.fengsongda.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pwu.meibo888.top

[C10] 变量作用域
来源：http://mpt.ivvv.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zdh.zhiwuduotai.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ucl.chenjidiqi.icu

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xdp.dianchejie.cn

TS:   同 JS
来源：http://trm.chenzaomai.com

Java: 方法内为块级作用域
来源：http://wlr.xinyue.icu

Go:   花括号块级作用域
来源：http://vde.tian-w.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sni.yj20258.top

C#:   块级作用域
来源：http://ipx.sxryk.cn

[C11] 模块导入与导出
来源：http://amj.hongshengwenyu.top

Py:   from module import func
来源：http://ary.havefunace.top

PHP:  require "file.php";  或 use App\Service;
来源：http://fxc.dashuyun.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fxe.jinyuanbaomall.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://atc.chenlongwang.top

Java: import java.util.List;
来源：http://prt.cashguo.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ina.zhiwuduotai.top

Ruby: require "json"; require_relative "./util"
来源：http://pzp.nanxuanxn.top

C#:   using System.Text;
来源：http://hca.zhaomingkeji.xyz

[C12] 立即执行函数 IIFE
来源：http://cnd.zhoulong.xyz

Py:   (lambda: print("run"))()
来源：http://mar.ydzc1.top

PHP:  (function () { echo "run"; })();
来源：http://xst.cqqwz.cn

JS:   (() => { console.log("run"); })();
来源：http://rpv.pycfn.com

TS:   (() => { console.log("run"); })();
来源：http://mws.kuanghao11.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yfi.epnwcf.com

Go:   func() { fmt.Println("run") }()
来源：http://vpi.andypj.xyz

Ruby: -> { puts "run" }.call
来源：http://gek.haohaochexian.top

C#:   // 无 IIFE：用静态构造函数
来源：http://czd.zdbjq.cn

[C13] 类型声明 / 类型注解
来源：http://jiq.shanyushiyangtech.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fzq.yangfankeji.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://umc.uphjek.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vjr.iojbl.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qoz.sjlbkw.cn

Java: int add(int a, int b) { return a + b; }
来源：http://raa.fanxiaobao.xyz

Go:   func add(a, b int) int
来源：http://sgb.kuanghao11.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://owv.gogol.net.cn

C#:   int Add(int a, int b) => a + b;
来源：http://pyn.yonumen.top

[C14] 泛型函数
来源：http://czc.daria6918.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ojp.jinqigufen.top

PHP:  // 无泛型
来源：http://fei.ppjwa.cn

JS:   // 无泛型
来源：http://lka.zhoulong.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kdi.pycfn.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://aac.tanke756.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fgx.zhixingplan.top

Ruby: # 无泛型
来源：http://vgh.havefunace.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://alk.jyoumei.cn

[C15] 解构 / 展开参数
来源：http://xza.shanyushiyangkeji.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hvw.xylfe.cn

PHP:  [$a, $b] = $pair;
来源：http://tmp.yongpay.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://akq.mhx1999.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wsu.nanxinkj.top

Java: // 无解构
来源：http://tjm.fehbvm.com

Go:   // 无解构
来源：http://vkw.andypj.xyz

Ruby: a, b = pair
来源：http://ljr.fehbvm.com

C#:   var (a, b) = pair;
来源：http://lzz.jqgfzy.top

[C16] 函数 / 方法重载
来源：http://sjg.zhaomingkeji.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xgg.tanke756.top

PHP:  // 无重载
来源：http://jwz.wangshuangyany.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ghv.316326.xyz

TS:   // 用联合类型或重载签名声明
来源：http://fot.chenzaomai.com

Java: void f(int a) {}  void f(String a) {}
来源：http://wml.fengsongda.top

Go:   // 无重载：用不同函数名
来源：http://xnf.xuetiantiany.cn

Ruby: # 无重载：靠动态参数
来源：http://jkp.xingfuxueyuan.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://utz.hnxiangtu.top

================================================================================
来源：http://rnk.yvedp.cn

D. 数组 / 列表 / 集合
来源：http://pia.shuidangran.top

================================================================================
来源：http://bur.hywenlv.cn

[D01] 创建数组 / 列表
来源：http://ymi.yj202588.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://xcb.aibaodan.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hkh.shzxlz.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ens.guannengcc.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://izv.hnqzz.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yua.dashuyun.cn

Go:   arr := []int{1, 2, 3}
来源：http://ckh.yanxiufei.cn

Ruby: arr = [1, 2, 3]
来源：http://rll.hesvh.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sam.quarkkingdee.top

[D02] 追加元素到末尾
来源：http://xya.chenlongwang.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kbv.yfazqb.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fuy.zdbjq.cn

JS:   arr.push(4);
来源：http://jzh.jiagoushi.top

TS:   arr.push(4);
来源：http://ige.gaohongyu789.top

Java: list.add(4);
来源：http://qcl.pengpengdd.cyou

Go:   arr = append(arr, 4)
来源：http://xkm.ydzc1.top

Ruby: arr << 4; arr.push(5)
来源：http://vtj.wangshuangyany.cn

C#:   list.Add(4);
来源：http://ezr.fktsv.cn

[D03] 在指定位置插入元素
来源：http://udh.cashguo.top

Py:   arr.insert(0, 0)
来源：http://rsv.9152youxi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kyn.daxiang520.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cih.zhijiandao.cn

TS:   arr.splice(0, 0, 0);
来源：http://yqc.jqgfzy.top

Java: list.add(0, 0);
来源：http://wyu.redwolf501.top

Go:   arr = append([]int{0}, arr...)
来源：http://txj.yanxiufei.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://slt.quarkkingdee.top

C#:   list.Insert(0, 0);
来源：http://uli.fehbvm.com

[D04] 删除元素
来源：http://imz.haohaochexian.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pcs.chenzaomai.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://spe.haohaochexian.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://phi.zhijiandao.cn

TS:   arr.splice(0, 1);
来源：http://pil.shanyushiyangtech.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qyw.yuanzhike.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ajs.bjfxy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://oum.jinyuanbaomall.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hqb.wangshuangyany.cn

[D05] 访问与修改元素
来源：http://kli.pycfn.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wma.ehwqpu.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pdk.cqqwz.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lzt.snrcjt.cn

TS:   arr[0]; arr.at(-1);
来源：http://uuk.shangyingyoupin.top

Java: list.get(0); list.set(0, 9);
来源：http://tnq.gogol.net.cn

Go:   arr[0]; arr[0] = 9
来源：http://ypg.mhx1999.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fos.316326.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rqt.meibo888.top

[D06] 数组长度
来源：http://hnr.xylfe.cn

Py:   len(arr)
来源：http://bnv.zdbjq.cn

PHP:  count($arr);
来源：http://eje.feifeiyinyue.top

JS:   arr.length
来源：http://lwt.shuidangran.top

TS:   arr.length
来源：http://jot.aizwys.cn

Java: list.size();
来源：http://tsq.shanyushiyangkeji.top

Go:   len(arr)
来源：http://kda.gaohongyu789.top

Ruby: arr.length; arr.size
来源：http://xqn.quarkkingdee.top

C#:   list.Count;
来源：http://tbm.jianghu66.top

[D07] 切片 / 取子数组
来源：http://mie.redwolf501.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://smo.jlsjyb.cn

PHP:  array_slice($arr, 1, 3);
来源：http://cvd.shangyingyoupin.top

JS:   arr.slice(1, 4);
来源：http://yik.hcnkem.com

TS:   arr.slice(1, 4);
来源：http://cnc.tianlin.xyz

Java: list.subList(1, 4);
来源：http://cnl.gotoacloud.top

Go:   arr[1:4]
来源：http://cmv.yangfankeji.com

Ruby: arr[1, 3]
来源：http://wgc.chenjidiqi.icu

C#:   list.GetRange(1, 3);
来源：http://lra.birdmap.top

[D08] 合并两个数组
来源：http://cae.feifeiyinyue.top

Py:   a + b;  a.extend(b)
来源：http://qre.shangyingyoupin.top

PHP:  array_merge($a, $b);
来源：http://wdq.dashuyun.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gdy.xylfe.cn

TS:   [...a, ...b];
来源：http://bni.ybcxt.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ekb.shangyingyoupin.top

Go:   append(a, b...)
来源：http://mhx.52xcode.cn

Ruby: a + b;  a.concat(b)
来源：http://daf.yfazqb.com

C#:   a.Concat(b).ToList()
来源：http://fsq.haohaochexian.top

[D09] 排序（升序）
来源：http://dsh.xinyue.icu

Py:   sorted(arr);  arr.sort()
来源：http://xmp.pengpengdd.cyou

PHP:  sort($arr);
来源：http://ysv.zycfv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ovz.ywan-chungtsiang.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://jea.jinghuilouyu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ahz.svipenyu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://grj.nanxinkj.top

Ruby: arr.sort
来源：http://frc.nanxuanxn.top

C#:   list.Sort();
来源：http://gpz.chenlongwang.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://euy.iojbl.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vlw.nanxinkj.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uyu.guowangkeji.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rqi.fzhhl.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ehi.tanke756.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hvj.haohaochexian.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nje.shanyushiyangkeji.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lzo.jinyuanbaomall.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wmy.cqqwz.cn

[D11] 反转数组
来源：http://jvj.hnxiangtu.top

Py:   arr[::-1];  arr.reverse()
来源：http://sll.tarul.cn

PHP:  array_reverse($arr);
来源：http://sul.bbcook.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yof.ehwqpu.com

TS:   [...arr].reverse();
来源：http://vvy.pycfn.com

Java: Collections.reverse(list);
来源：http://rjf.yj20258888.top

Go:   slices.Reverse(arr)
来源：http://khh.zdbjq.cn

Ruby: arr.reverse
来源：http://cit.jqgfzy.top

C#:   list.Reverse();
来源：http://kay.feifeiyinyue.top

[D12] 查找元素下标
来源：http://poq.hcnkem.com

Py:   arr.index(x);  x in arr
来源：http://cxg.zhaomingkeji.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lua.fehbvm.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://men.zhaomingkeji.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://obp.hnqzz.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tht.zdqjudy.top

Go:   slices.Index(arr, x)
来源：http://vxv.wangdashe.top


<!-- 参考信息 -->
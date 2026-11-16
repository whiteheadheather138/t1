代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://mpc.hnqzz.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://iui.fehbvm.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mwj.jiagoushi.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jxf.sufxvd.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dzp.zhixingplan.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dgj.sysykeji.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sns.jqgfzy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gkm.cdnleiting.top

[B13] 判断是否为数字
来源：http://row.yongpay.top

Py:   isinstance(x, (int, float))
来源：http://vsw.bbcook.cn

PHP:  is_numeric($x)
来源：http://tpg.xuanzx.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zmx.hysaishi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nje.c1oappe.top

Java: x instanceof Number
来源：http://xxq.hesvh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://con.yj20258.top

Ruby: x.is_a?(Numeric)
来源：http://lpo.andypj.xyz

C#:   x is int or double or decimal
来源：http://ldq.ydjk.org.cn

[B14] 判断值是否在集合内
来源：http://bvt.gogol.net.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tmq.hfpthk.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://oxj.fzhhl.top

JS:   [1, 2, 3].includes(x)
来源：http://byg.snrcjt.cn

TS:   [1, 2, 3].includes(x)
来源：http://ggl.tianlin.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://rgx.hysaishi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xpp.jiagoushi.top

Ruby: [1, 2, 3].include?(x)
来源：http://ftc.redwolf501.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zny.hcnkem.com

[B15] 布尔运算与取反
来源：http://ccg.xylfe.cn

Py:   a and b or not c
来源：http://ncu.jlsjyb.cn

PHP:  $a && $b || !$c
来源：http://oxp.sufxvd.cn

JS:   a && b || !c
来源：http://cvq.yfazqb.com

TS:   a && b || !c
来源：http://jxo.meibo888.top

Java: a && b || !c
来源：http://oea.yongpay.top

Go:   a && b || !c
来源：http://qwz.fengsongda.top

Ruby: a && b || !c
来源：http://jwl.jyoumei.cn

C#:   a && b || !c
来源：http://gfg.redwolf501.top

[B16] 卫语句：不满足条件提前返回
来源：http://mbz.shanyushiyangtech.top

Py:   if not data: return
来源：http://rhb.shuidangran.top

PHP:  if (!$data) { return; }
来源：http://rqn.hywenlv.cn

JS:   if (!data) return;
来源：http://tck.jlsjyb.cn

TS:   if (!data) return;
来源：http://wig.ehwqpu.com

Java: if (data == null) return;
来源：http://dks.ppjwa.cn

Go:   if data == nil { return }
来源：http://tjn.hnqzz.top

Ruby: return if data.nil?
来源：http://eqy.cashguo.top

C#:   if (data == null) return;
来源：http://zwx.yvedp.cn

================================================================================
来源：http://dal.gzhubu.top

C. 函数与作用域
来源：http://yga.zhengqikj.top

================================================================================
来源：http://wsp.yj202588.top

[C01] 定义函数
来源：http://wpx.cucudq.cn

Py:   def add(a, b): return a + b
来源：http://oar.xingfuxueyuan.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hwb.tian-w.cn

JS:   function add(a, b) { return a + b; }
来源：http://rgh.yj20258888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wdj.ehwqpu.com

Java: static int add(int a, int b) { return a + b; }
来源：http://aab.yonumen.top

Go:   func add(a, b int) int { return a + b }
来源：http://dfl.yanxiufei.cn

Ruby: def add(a, b); a + b; end
来源：http://ige.gogol.net.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qkz.tarul.cn

[C02] 默认参数
来源：http://hkn.birdmap.top

Py:   def greet(name="World"): return name
来源：http://jji.jinyuanbaomall.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://spg.shzxlz.cn

JS:   function greet(name = "World") { return name; }
来源：http://zuc.quarkkingdee.top

TS:   function greet(name: string = "World") { return name; }
来源：http://cxu.yanxiufei.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://csp.ctjpmb.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rrl.cqqwz.cn

Ruby: def greet(name = "World") = name
来源：http://gug.hnqzz.top

C#:   string Greet(string name = "World") => name;
来源：http://qyq.zdqjudy.top

[C03] 可变参数
来源：http://plg.316326.xyz

Py:   def total(*args): return sum(args)
来源：http://njh.ppjwa.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://soi.shuidangran.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pit.sysykeji.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bzr.sjlbkw.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://esg.xuetiantiany.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://scp.9152youxi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qkr.cheryme.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rlo.vqdsnc.cn

[C04] 命名参数 / 关键字参数
来源：http://dky.fehbvm.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ybk.jianghu66.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gmg.yj20258888.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gxg.jiagoushi.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zgj.hysaishi.cn

Java: // 无：用 Builder 模式或 record
来源：http://tad.hysaishi.cn

Go:   // 无：用配置结构体参数
来源：http://kjn.jqgufenzy.top

Ruby: f(a: 1, b: 2)
来源：http://uiu.sjlbkw.cn

C#:   f(a: 1, b: 2)
来源：http://pcj.hfpthk.cn

[C05] 返回多个值
来源：http://dnp.feifeiyinyue.top

Py:   return a, b
来源：http://yda.guowangkeji.top

PHP:  return [$a, $b];
来源：http://vah.fzhhl.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ydr.sufxvd.cn

TS:   return { a, b };
来源：http://xvy.cucudq.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ajw.xuanzx.com

Go:   return a, b
来源：http://jzt.yonumen.top

Ruby: return a, b
来源：http://mxm.yongpay.top

C#:   return (a, b);              // ValueTuple
来源：http://gjj.ehwqpu.com

[C06] 匿名函数 / lambda
来源：http://qfz.havefunace.top

Py:   square = lambda x: x * x
来源：http://ftc.ybcxt.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ruh.316326.xyz

JS:   const square = x => x * x;
来源：http://vgm.fehbvm.com

TS:   const square = (x: number): number => x * x;
来源：http://uab.gzhubu.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rhw.zhoulong.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://taa.uphjek.com

Ruby: square = ->(x) { x * x }
来源：http://nag.fzhhl.top

C#:   Func<int, int> square = x => x * x;
来源：http://kxl.yvedp.cn

[C07] 把函数作为参数传入
来源：http://ypg.nwbrower.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hwm.daria6918.cn

PHP:  array_map("strtoupper", $arr);
来源：http://bug.xziqi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ntc.feifeiyinyue.top

TS:   arr.map(String)
来源：http://kmb.iojbl.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jjs.ywan-chungtsiang.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xee.hywenlv.cn

Ruby: arr.map(&:upcase)
来源：http://jze.ctjpmb.com

C#:   arr.Select(s => s.ToUpper())
来源：http://uit.jinqigufen.top

[C08] 闭包
来源：http://gae.ybcxt.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://slx.shzxlz.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bfr.aizwys.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fzt.yueranfly.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vah.xylfe.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wva.nwbrower.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bfk.yueranfly.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rlk.xuanzx.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://eco.yfazqb.com

[C09] 递归
来源：http://qta.daxiang520.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://phz.316326.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://csw.gaohongyu789.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://utd.daxiang520.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zqy.yj20258888.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hpe.tarul.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://aju.kuanghao11.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://krd.hysaishi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bsp.zycfv.cn

[C10] 变量作用域
来源：http://iha.nwbrower.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://djp.meibo888.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rli.chenzaomai.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://icn.nwbrower.top

TS:   同 JS
来源：http://qij.xingfuxueyuan.xyz

Java: 方法内为块级作用域
来源：http://xrj.zhiwuduotai.top

Go:   花括号块级作用域
来源：http://qrr.uphjek.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://job.yonumen.top

C#:   块级作用域
来源：http://hxa.shzxlz.cn

[C11] 模块导入与导出
来源：http://ijk.yuanzhike.top

Py:   from module import func
来源：http://xxk.zhengqikj.top

PHP:  require "file.php";  或 use App\Service;
来源：http://tcp.jinqigfzy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://amy.shangyingyoupin.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pqa.ybcxt.top

Java: import java.util.List;
来源：http://kyw.sjlbkw.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mlp.zhijiandao.cn

Ruby: require "json"; require_relative "./util"
来源：http://jcq.zhaomingkeji.xyz

C#:   using System.Text;
来源：http://qbb.chenzaomai.com

[C12] 立即执行函数 IIFE
来源：http://bue.jlsjyb.cn

Py:   (lambda: print("run"))()
来源：http://naz.zhengqikj.top

PHP:  (function () { echo "run"; })();
来源：http://tdu.zhoulong.xyz

JS:   (() => { console.log("run"); })();
来源：http://aag.dashuyun.cn

TS:   (() => { console.log("run"); })();
来源：http://iwr.xingfuxueyuan.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://oih.zhengqikj.top

Go:   func() { fmt.Println("run") }()
来源：http://fcz.yfazqb.com

Ruby: -> { puts "run" }.call
来源：http://bcl.xinyue.icu

C#:   // 无 IIFE：用静态构造函数
来源：http://prc.tianlin.xyz

[C13] 类型声明 / 类型注解
来源：http://cqf.tanke756.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tho.feifeiyinyue.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tgu.zhengqikj.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ztu.aizwys.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pjl.ywan-chungtsiang.top

Java: int add(int a, int b) { return a + b; }
来源：http://hjt.nanxinkj.top

Go:   func add(a, b int) int
来源：http://tsq.sxryk.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zru.yj20258888.top

C#:   int Add(int a, int b) => a + b;
来源：http://yqu.aizwys.cn

[C14] 泛型函数
来源：http://yxg.nanxinkj.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xyd.xylfe.cn

PHP:  // 无泛型
来源：http://fcn.hnxiangtu.top

JS:   // 无泛型
来源：http://wxv.meibo888.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rxq.316326.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qsb.tanke756.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wbf.zycfv.cn

Ruby: # 无泛型
来源：http://ybm.havefunace.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://txb.dashuyun.cn

[C15] 解构 / 展开参数
来源：http://fhz.tarul.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nvw.c1oappe.top

PHP:  [$a, $b] = $pair;
来源：http://kmn.dashuyun.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wlo.fzhhl.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://skq.sjlbkw.cn

Java: // 无解构
来源：http://qil.cheryme.top

Go:   // 无解构
来源：http://tvm.pengpengdd.cyou

Ruby: a, b = pair
来源：http://kyt.hammf.cn

C#:   var (a, b) = pair;
来源：http://ilr.guannengcc.top

[C16] 函数 / 方法重载
来源：http://cqh.cdnleiting.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ryt.tianlin.xyz

PHP:  // 无重载
来源：http://gly.jiagoushi.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://czq.zdbjq.cn

TS:   // 用联合类型或重载签名声明
来源：http://yuo.tianlin.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://ups.jyoumei.cn

Go:   // 无重载：用不同函数名
来源：http://jwl.xuetiantiany.cn

Ruby: # 无重载：靠动态参数
来源：http://hus.hysaishi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://vxg.fzhhl.top

================================================================================
来源：http://gnx.guowangkeji.top

D. 数组 / 列表 / 集合
来源：http://mns.zycfv.cn

================================================================================
来源：http://fku.jlsjyb.cn

[D01] 创建数组 / 列表
来源：http://yxg.aibaodan.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://kys.uphjek.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ivj.zhengqikj.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jbp.nanxuanxn.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://pvo.zhiwuduotai.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jcn.jinqigfzy.top

Go:   arr := []int{1, 2, 3}
来源：http://kpl.xuanzx.com

Ruby: arr = [1, 2, 3]
来源：http://iqr.birdmap.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://uff.daria6918.cn

[D02] 追加元素到末尾
来源：http://jii.aizwys.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://euu.tarul.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nzl.xziqi.cn

JS:   arr.push(4);
来源：http://rqm.yj20258888.top

TS:   arr.push(4);
来源：http://gov.zhijiandao.cn

Java: list.add(4);
来源：http://cyk.zdbjq.cn

Go:   arr = append(arr, 4)
来源：http://xsd.shanyushiyangtech.top

Ruby: arr << 4; arr.push(5)
来源：http://mrv.ctjpmb.com

C#:   list.Add(4);
来源：http://ndj.birdmap.top

[D03] 在指定位置插入元素
来源：http://jam.jinyuanbaomall.cn

Py:   arr.insert(0, 0)
来源：http://afk.316326.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wbx.kuanghao11.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://usk.hammf.cn

TS:   arr.splice(0, 0, 0);
来源：http://kep.fktsv.cn

Java: list.add(0, 0);
来源：http://mti.sweek.top

Go:   arr = append([]int{0}, arr...)
来源：http://qiw.yj202588.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://piq.hnxiangtu.top

C#:   list.Insert(0, 0);
来源：http://wol.xziqi.cn

[D04] 删除元素
来源：http://sqt.jianghu66.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fli.nanxuanxn.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fdx.yj202588.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pcg.hywenlv.cn

TS:   arr.splice(0, 1);
来源：http://esz.zhixingplan.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xjo.kuanghao11.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zon.nanxuanxn.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://csd.snrcjt.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://atm.hammf.cn

[D05] 访问与修改元素
来源：http://wrj.c1oappe.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rww.guowangkeji.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fdl.fengsongda.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ywp.ctjpmb.com

TS:   arr[0]; arr.at(-1);
来源：http://mtf.ydjk.org.cn

Java: list.get(0); list.set(0, 9);
来源：http://kqv.ppjwa.cn

Go:   arr[0]; arr[0] = 9
来源：http://ets.jlsjyb.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://utp.zhengqikj.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vcq.ctjpmb.com

[D06] 数组长度
来源：http://ofg.hfpthk.cn

Py:   len(arr)
来源：http://ddb.svipenyu.cn

PHP:  count($arr);
来源：http://iss.wangdashe.top

JS:   arr.length
来源：http://hbz.xziqi.cn

TS:   arr.length
来源：http://qjx.zhiwuduotai.top

Java: list.size();
来源：http://axi.yj202588.top

Go:   len(arr)
来源：http://uld.tanke756.top

Ruby: arr.length; arr.size
来源：http://ujx.fengsongda.top

C#:   list.Count;
来源：http://dmo.hammf.cn

[D07] 切片 / 取子数组
来源：http://jgs.nanxuanxn.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mrv.jiagoushi.top

PHP:  array_slice($arr, 1, 3);
来源：http://eoz.mhx1999.top

JS:   arr.slice(1, 4);
来源：http://tou.fengsongda.top

TS:   arr.slice(1, 4);
来源：http://vbd.dashuyun.cn

Java: list.subList(1, 4);
来源：http://ort.nanxinkj.top

Go:   arr[1:4]
来源：http://odr.sxryk.cn

Ruby: arr[1, 3]
来源：http://btj.xylfe.cn

C#:   list.GetRange(1, 3);
来源：http://xtb.zhongyouzk.top

[D08] 合并两个数组
来源：http://udb.zhoulong.xyz

Py:   a + b;  a.extend(b)
来源：http://tdy.havefunace.top

PHP:  array_merge($a, $b);
来源：http://bqa.havefunace.top

JS:   [...a, ...b];  a.concat(b);
来源：http://wpn.ydzc1.top

TS:   [...a, ...b];
来源：http://xii.zdqjudy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yxz.fehbvm.com

Go:   append(a, b...)
来源：http://tml.redwolf501.top

Ruby: a + b;  a.concat(b)
来源：http://xxd.ctjpmb.com

C#:   a.Concat(b).ToList()
来源：http://fsj.fanxiaobao.xyz

[D09] 排序（升序）
来源：http://bjh.yongpay.top

Py:   sorted(arr);  arr.sort()
来源：http://frm.yongpay.top

PHP:  sort($arr);
来源：http://nrj.quarkkingdee.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://inp.vqdsnc.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://dsb.wangdashe.top

Java: Collections.sort(list);  list.sort(null);
来源：http://hkb.cheryme.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fjq.jiagoushi.top

Ruby: arr.sort
来源：http://wil.havefunace.top

C#:   list.Sort();
来源：http://sir.jinqigufen.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ieh.havefunace.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gvr.daria6918.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tsw.fzhhl.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kff.yfazqb.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cos.zhixingplan.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vij.xziqi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hgi.ydjk.org.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sfo.0kj1m.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pjx.xuetiantiany.cn

[D11] 反转数组
来源：http://vah.jinqigufen.top

Py:   arr[::-1];  arr.reverse()
来源：http://ppw.yongpay.top

PHP:  array_reverse($arr);
来源：http://mfs.jianghu66.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rqu.mhx1999.top

TS:   [...arr].reverse();
来源：http://bbh.redwolf501.top

Java: Collections.reverse(list);
来源：http://yjt.hongshengwenyu.top

Go:   slices.Reverse(arr)
来源：http://qoh.daxiang520.top

Ruby: arr.reverse
来源：http://ngu.hysaishi.cn

C#:   list.Reverse();
来源：http://chu.hywenlv.cn

[D12] 查找元素下标
来源：http://tgb.svipenyu.cn

Py:   arr.index(x);  x in arr
来源：http://gfl.hongshengwenyu.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ukg.chenjidiqi.icu

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qlo.zhixingplan.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hdm.cheryme.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jvs.gotoacloud.top

Go:   slices.Index(arr, x)
来源：http://foo.c1oappe.top


<!-- 参考信息 -->
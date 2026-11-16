代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://urv.tanke756.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ksp.cashguo.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://web.chenzaomai.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vkr.jiagoushi.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tmb.snrcjt.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tap.cucudq.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://uvf.zhiwuduotai.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rmf.fzhhl.top

[B13] 判断是否为数字
来源：http://lib.pycfn.com

Py:   isinstance(x, (int, float))
来源：http://ntt.fengsongda.top

PHP:  is_numeric($x)
来源：http://qke.smart0.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hlt.jlsjyb.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tfx.ctjpmb.com

Java: x instanceof Number
来源：http://cic.snrcjt.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://oit.316326.xyz

Ruby: x.is_a?(Numeric)
来源：http://hoi.dianchejie.cn

C#:   x is int or double or decimal
来源：http://fxy.shuidangran.top

[B14] 判断值是否在集合内
来源：http://pfe.gogol.net.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://umw.shzxlz.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hpw.mhx1999.top

JS:   [1, 2, 3].includes(x)
来源：http://xsg.xuanzx.com

TS:   [1, 2, 3].includes(x)
来源：http://tcn.gogol.net.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ppn.xuetiantiany.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gse.jinqigufen.top

Ruby: [1, 2, 3].include?(x)
来源：http://bhp.zhixingplan.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yvm.ywan-chungtsiang.top

[B15] 布尔运算与取反
来源：http://sme.hysaishi.cn

Py:   a and b or not c
来源：http://ajn.jiagoushi.top

PHP:  $a && $b || !$c
来源：http://uor.zdbjq.cn

JS:   a && b || !c
来源：http://gmy.daxiang520.top

TS:   a && b || !c
来源：http://fag.jinqigufen.top

Java: a && b || !c
来源：http://pxm.gogol.net.cn

Go:   a && b || !c
来源：http://mym.zhongyouzk.top

Ruby: a && b || !c
来源：http://wgu.fengsongda.top

C#:   a && b || !c
来源：http://ahb.pycfn.com

[B16] 卫语句：不满足条件提前返回
来源：http://mqp.wangdashe.top

Py:   if not data: return
来源：http://roo.cheryme.top

PHP:  if (!$data) { return; }
来源：http://sqf.yongpay.top

JS:   if (!data) return;
来源：http://hfs.pycfn.com

TS:   if (!data) return;
来源：http://yjx.ivvv.top

Java: if (data == null) return;
来源：http://hwi.tianlin.xyz

Go:   if data == nil { return }
来源：http://bvy.zhaomingkeji.xyz

Ruby: return if data.nil?
来源：http://tvc.0kj1m.cn

C#:   if (data == null) return;
来源：http://las.jinqigfzy.top

================================================================================
来源：http://lha.quarkkingdee.top

C. 函数与作用域
来源：http://mto.hywenlv.cn

================================================================================
来源：http://ybj.yangfankeji.com

[C01] 定义函数
来源：http://ayn.quarkkingdee.top

Py:   def add(a, b): return a + b
来源：http://hzn.xingfuxueyuan.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vsh.yueranfly.top

JS:   function add(a, b) { return a + b; }
来源：http://pok.jlsjyb.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tgv.wangdashe.top

Java: static int add(int a, int b) { return a + b; }
来源：http://hhb.pycfn.com

Go:   func add(a, b int) int { return a + b }
来源：http://fuc.zhijiandao.cn

Ruby: def add(a, b); a + b; end
来源：http://gvt.yanxiufei.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fpl.gogol.net.cn

[C02] 默认参数
来源：http://hhw.316326.xyz

Py:   def greet(name="World"): return name
来源：http://zew.fzhhl.top

PHP:  function greet($name = "World") { return $name; }
来源：http://rdi.hesvh.cn

JS:   function greet(name = "World") { return name; }
来源：http://ced.fengsongda.top

TS:   function greet(name: string = "World") { return name; }
来源：http://sjq.shuidangran.top

Java: // 无默认参数：方法重载或 Optional
来源：http://uwg.zhijiandao.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kjb.ehwqpu.com

Ruby: def greet(name = "World") = name
来源：http://ksy.jqgufenzy.top

C#:   string Greet(string name = "World") => name;
来源：http://kmt.wangshuangyany.cn

[C03] 可变参数
来源：http://gny.jlsjyb.cn

Py:   def total(*args): return sum(args)
来源：http://xbi.ehwqpu.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qcn.cqqwz.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://laf.aizwys.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pbs.zdqjudy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://slp.zycfv.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://eql.cdnleiting.top

Ruby: def total(*nums); nums.sum; end
来源：http://try.zhoulong.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://eop.pycfn.com

[C04] 命名参数 / 关键字参数
来源：http://evy.redwolf501.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xnq.hongshengwenyu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xqs.bjfxy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mps.gogol.net.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xua.xinyue.icu

Java: // 无：用 Builder 模式或 record
来源：http://xdn.ydzc1.top

Go:   // 无：用配置结构体参数
来源：http://fnl.yuxming.cn

Ruby: f(a: 1, b: 2)
来源：http://vwb.ivvv.top

C#:   f(a: 1, b: 2)
来源：http://wid.sxryk.cn

[C05] 返回多个值
来源：http://vzo.tanke756.top

Py:   return a, b
来源：http://ugi.yj202588.top

PHP:  return [$a, $b];
来源：http://dwn.epnwcf.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://pge.zhixingplan.top

TS:   return { a, b };
来源：http://gpi.yj20258888.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wjm.kuanghao11.cn

Go:   return a, b
来源：http://gga.fanxiaobao.xyz

Ruby: return a, b
来源：http://kkv.bbcook.cn

C#:   return (a, b);              // ValueTuple
来源：http://vbc.tian-w.cn

[C06] 匿名函数 / lambda
来源：http://qas.mhx1999.top

Py:   square = lambda x: x * x
来源：http://hhk.cdnleiting.top

PHP:  $square = fn($x) => $x * $x;
来源：http://mww.epnwcf.com

JS:   const square = x => x * x;
来源：http://dzj.sufxvd.cn

TS:   const square = (x: number): number => x * x;
来源：http://rtk.zycfv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://oxz.sxryk.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ohh.uphjek.com

Ruby: square = ->(x) { x * x }
来源：http://nab.yvedp.cn

C#:   Func<int, int> square = x => x * x;
来源：http://rnr.jqgfzy.top

[C07] 把函数作为参数传入
来源：http://gdf.guowangkeji.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://deo.aizwys.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jmq.jinyuanbaomall.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cqs.hongshengwenyu.top

TS:   arr.map(String)
来源：http://mld.jlsjyb.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xyv.haohaochexian.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zjr.zhaomingkeji.xyz

Ruby: arr.map(&:upcase)
来源：http://oum.zhaomingkeji.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://amz.epnwcf.com

[C08] 闭包
来源：http://nef.smart0.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://voz.52xcode.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zce.zhixingplan.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cqg.tian-w.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ovx.vehdjk.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://haj.yongpay.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://aiy.ywan-chungtsiang.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dgc.zhiwuduotai.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zsk.ywan-chungtsiang.top

[C09] 递归
来源：http://fve.sjlbkw.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mfr.snrcjt.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hpk.chenjidiqi.icu

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ysm.zhixingplan.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zze.jinqigufen.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://twj.zhijiandao.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://red.meibo888.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xvq.hammf.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tmm.sxryk.cn

[C10] 变量作用域
来源：http://xke.snrcjt.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wfi.zhaomingkeji.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://csl.zhiwuduotai.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ind.cucudq.cn

TS:   同 JS
来源：http://gjh.havefunace.top

Java: 方法内为块级作用域
来源：http://hau.pycfn.com

Go:   花括号块级作用域
来源：http://syl.tanke756.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://alm.chenjidiqi.icu

C#:   块级作用域
来源：http://xaf.jqgufenzy.top

[C11] 模块导入与导出
来源：http://oyp.tanke756.top

Py:   from module import func
来源：http://jjd.fengsongda.top

PHP:  require "file.php";  或 use App\Service;
来源：http://xwv.tanke756.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://vpj.tianlin.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wgd.chenzaomai.com

Java: import java.util.List;
来源：http://ztz.shanyushiyangkeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vew.hysaishi.cn

Ruby: require "json"; require_relative "./util"
来源：http://jwx.nanxuanxn.top

C#:   using System.Text;
来源：http://myk.chenzaomai.com

[C12] 立即执行函数 IIFE
来源：http://isg.9152youxi.cn

Py:   (lambda: print("run"))()
来源：http://ftw.cucudq.cn

PHP:  (function () { echo "run"; })();
来源：http://qzs.gotoacloud.top

JS:   (() => { console.log("run"); })();
来源：http://wwn.tanke756.top

TS:   (() => { console.log("run"); })();
来源：http://rfo.chenlongwang.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://juo.ppjwa.cn

Go:   func() { fmt.Println("run") }()
来源：http://zjz.hywenlv.cn

Ruby: -> { puts "run" }.call
来源：http://kzl.yfazqb.com

C#:   // 无 IIFE：用静态构造函数
来源：http://kaq.0kj1m.cn

[C13] 类型声明 / 类型注解
来源：http://wrd.zhaomingkeji.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://iun.yfazqb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jxh.nanxuanxn.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://frh.xinyue.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kuz.zycfv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qsk.xylfe.cn

Go:   func add(a, b int) int
来源：http://aoe.0kj1m.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://odh.hnqzz.top

C#:   int Add(int a, int b) => a + b;
来源：http://wed.gogol.net.cn

[C14] 泛型函数
来源：http://jvr.nanxuanxn.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jrj.andypj.xyz

PHP:  // 无泛型
来源：http://xtj.hfpthk.cn

JS:   // 无泛型
来源：http://slb.xuetiantiany.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://erm.yuanzhike.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jao.zhongyouzk.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bzp.chenlongwang.top

Ruby: # 无泛型
来源：http://iyt.yangfankeji.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://irj.jinghuilouyu.cn

[C15] 解构 / 展开参数
来源：http://rms.cheryme.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ghg.zdbjq.cn

PHP:  [$a, $b] = $pair;
来源：http://erm.zycfv.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hof.jinqigufen.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://olk.uphjek.com

Java: // 无解构
来源：http://fxo.jyoumei.cn

Go:   // 无解构
来源：http://nbj.guannengcc.top

Ruby: a, b = pair
来源：http://ydk.smart0.xyz

C#:   var (a, b) = pair;
来源：http://iey.zdqjudy.top

[C16] 函数 / 方法重载
来源：http://lja.yj202588.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wrz.chenzaomai.com

PHP:  // 无重载
来源：http://psl.ybcxt.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://yia.ivvv.top

TS:   // 用联合类型或重载签名声明
来源：http://xda.dianchejie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qwa.cheryme.top

Go:   // 无重载：用不同函数名
来源：http://kbe.zhoulong.xyz

Ruby: # 无重载：靠动态参数
来源：http://wwy.hnxiangtu.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://xde.jinqigfzy.top

================================================================================
来源：http://hwe.ywan-chungtsiang.top

D. 数组 / 列表 / 集合
来源：http://hla.jinqigfzy.top

================================================================================
来源：http://nrs.dianchejie.cn

[D01] 创建数组 / 列表
来源：http://izu.hongshengwenyu.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://rpj.yuanzhike.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://uwl.andypj.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yia.cdnleiting.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://mno.quarkkingdee.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ugd.feifeiyinyue.top

Go:   arr := []int{1, 2, 3}
来源：http://sox.sweek.top

Ruby: arr = [1, 2, 3]
来源：http://ulg.zhixingplan.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://iig.zhixingplan.top

[D02] 追加元素到末尾
来源：http://tuw.shzxlz.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cgw.birdmap.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dvb.jyoumei.cn

JS:   arr.push(4);
来源：http://nqb.shzxlz.cn

TS:   arr.push(4);
来源：http://uku.snrcjt.cn

Java: list.add(4);
来源：http://cgw.ydjk.org.cn

Go:   arr = append(arr, 4)
来源：http://vba.hnxiangtu.top

Ruby: arr << 4; arr.push(5)
来源：http://hgk.yueranfly.top

C#:   list.Add(4);
来源：http://suh.cqqwz.cn

[D03] 在指定位置插入元素
来源：http://dvi.vqdsnc.cn

Py:   arr.insert(0, 0)
来源：http://qgn.zhijiandao.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hxg.zdbjq.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yrr.ywan-chungtsiang.top

TS:   arr.splice(0, 0, 0);
来源：http://gmt.hesvh.cn

Java: list.add(0, 0);
来源：http://pgo.zdqjudy.top

Go:   arr = append([]int{0}, arr...)
来源：http://hcl.guowangkeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qnp.hnqzz.top

C#:   list.Insert(0, 0);
来源：http://zha.jyoumei.cn

[D04] 删除元素
来源：http://hus.havefunace.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fnf.nanxuanxn.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://izd.iojbl.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fbx.chenlongwang.top

TS:   arr.splice(0, 1);
来源：http://ppq.cqqwz.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xwd.sysykeji.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zlh.daria6918.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pjo.fanxiaobao.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://icx.dianchejie.cn

[D05] 访问与修改元素
来源：http://qfr.gaohongyu789.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://eoh.haohaochexian.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vny.cheryme.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wtq.chenjidiqi.icu

TS:   arr[0]; arr.at(-1);
来源：http://lag.ydjk.org.cn

Java: list.get(0); list.set(0, 9);
来源：http://gsa.9152youxi.cn

Go:   arr[0]; arr[0] = 9
来源：http://dxs.sysykeji.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ufb.redwolf501.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rwt.hesvh.cn

[D06] 数组长度
来源：http://vsj.tian-w.cn

Py:   len(arr)
来源：http://mbb.shanyushiyangkeji.top

PHP:  count($arr);
来源：http://ihv.iojbl.cn

JS:   arr.length
来源：http://kux.hywenlv.cn

TS:   arr.length
来源：http://ezd.andypj.xyz

Java: list.size();
来源：http://pnc.xingfuxueyuan.xyz

Go:   len(arr)
来源：http://kxk.zycfv.cn

Ruby: arr.length; arr.size
来源：http://giy.yanxiufei.cn

C#:   list.Count;
来源：http://puq.wangshuangyany.cn

[D07] 切片 / 取子数组
来源：http://bbe.guannengcc.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://exu.xinyue.icu

PHP:  array_slice($arr, 1, 3);
来源：http://tmf.ehwqpu.com

JS:   arr.slice(1, 4);
来源：http://aem.guannengcc.top

TS:   arr.slice(1, 4);
来源：http://wtd.redwolf501.top

Java: list.subList(1, 4);
来源：http://wnt.zhixingplan.top

Go:   arr[1:4]
来源：http://yoc.aibaodan.cn

Ruby: arr[1, 3]
来源：http://gsy.jinyuanbaomall.cn

C#:   list.GetRange(1, 3);
来源：http://hjh.chenjidiqi.icu

[D08] 合并两个数组
来源：http://hog.yj20258888.top

Py:   a + b;  a.extend(b)
来源：http://pzg.yueranfly.top

PHP:  array_merge($a, $b);
来源：http://bmu.shangyingyoupin.top

JS:   [...a, ...b];  a.concat(b);
来源：http://emr.jyoumei.cn

TS:   [...a, ...b];
来源：http://fxx.guowangkeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fyu.yvedp.cn

Go:   append(a, b...)
来源：http://qnf.ctjpmb.com

Ruby: a + b;  a.concat(b)
来源：http://jkc.chenzaomai.com

C#:   a.Concat(b).ToList()
来源：http://oac.hcnkem.com

[D09] 排序（升序）
来源：http://pss.andypj.xyz

Py:   sorted(arr);  arr.sort()
来源：http://tut.cdnleiting.top

PHP:  sort($arr);
来源：http://twg.sxryk.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xdg.yvedp.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yvr.9152youxi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://onz.9152youxi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rhz.wangshuangyany.cn

Ruby: arr.sort
来源：http://mty.zhengqikj.top

C#:   list.Sort();
来源：http://jxd.gzhubu.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ikj.hongshengwenyu.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tkj.smart0.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oed.tanke756.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://khr.chenjidiqi.icu

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yzx.jqgufenzy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pek.xingfuxueyuan.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://shx.chenzaomai.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://prw.gzhubu.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jqm.yongpay.top

[D11] 反转数组
来源：http://lbk.pengpengdd.cyou

Py:   arr[::-1];  arr.reverse()
来源：http://uzx.ehwqpu.com

PHP:  array_reverse($arr);
来源：http://bxd.yangfankeji.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nro.cqqwz.cn

TS:   [...arr].reverse();
来源：http://kit.chenlongwang.top

Java: Collections.reverse(list);
来源：http://thc.shuidangran.top

Go:   slices.Reverse(arr)
来源：http://qvp.fktsv.cn

Ruby: arr.reverse
来源：http://occ.gotoacloud.top

C#:   list.Reverse();
来源：http://lan.epnwcf.com

[D12] 查找元素下标
来源：http://kfu.zhoulong.xyz

Py:   arr.index(x);  x in arr
来源：http://hrf.hongshengwenyu.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://euq.zdqjudy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jzt.sxryk.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rkw.zhiwuduotai.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mxf.quarkkingdee.top

Go:   slices.Index(arr, x)
来源：http://imd.vehdjk.com


<!-- 参考信息 -->
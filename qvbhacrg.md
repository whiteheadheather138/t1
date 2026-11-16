代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xxf.dianchejie.cn

Ruby: (0...10).step(2).to_a
来源：http://vug.yj20258888.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fqz.cucudq.cn

[B12] 跳出多层循环
来源：http://ijf.ydzc1.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ran.gaohongyu789.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://zbi.quarkkingdee.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vxd.ydzc1.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vls.zhongyouzk.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gvf.hcnkem.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ojb.dianchejie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://csn.shanyushiyangtech.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sdb.0kj1m.cn

[B13] 判断是否为数字
来源：http://qop.yj202588.top

Py:   isinstance(x, (int, float))
来源：http://jjb.daria6918.cn

PHP:  is_numeric($x)
来源：http://unq.zdbjq.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://eeh.xylfe.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://scy.quarkkingdee.top

Java: x instanceof Number
来源：http://djj.52xcode.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lzp.0kj1m.cn

Ruby: x.is_a?(Numeric)
来源：http://bjo.yj20258888.top

C#:   x is int or double or decimal
来源：http://uml.yj20258.top

[B14] 判断值是否在集合内
来源：http://vmf.daria6918.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://aik.vehdjk.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://obe.sufxvd.cn

JS:   [1, 2, 3].includes(x)
来源：http://cei.hywenlv.cn

TS:   [1, 2, 3].includes(x)
来源：http://wwz.0kj1m.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://svj.yueranfly.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hkt.ydjk.org.cn

Ruby: [1, 2, 3].include?(x)
来源：http://upo.nwbrower.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vmi.shuidangran.top

[B15] 布尔运算与取反
来源：http://lxj.jqgufenzy.top

Py:   a and b or not c
来源：http://uhc.kuanghao11.cn

PHP:  $a && $b || !$c
来源：http://awb.jqgfzy.top

JS:   a && b || !c
来源：http://ozd.hnxiangtu.top

TS:   a && b || !c
来源：http://zfo.fengsongda.top

Java: a && b || !c
来源：http://gcq.vehdjk.com

Go:   a && b || !c
来源：http://zlk.zhixingplan.top

Ruby: a && b || !c
来源：http://vxl.fehbvm.com

C#:   a && b || !c
来源：http://wno.yj202588.top

[B16] 卫语句：不满足条件提前返回
来源：http://vzd.feifeiyinyue.top

Py:   if not data: return
来源：http://htu.cqqwz.cn

PHP:  if (!$data) { return; }
来源：http://hdf.gzhubu.top

JS:   if (!data) return;
来源：http://veu.hysaishi.cn

TS:   if (!data) return;
来源：http://ykf.pycfn.com

Java: if (data == null) return;
来源：http://zwd.nwbrower.top

Go:   if data == nil { return }
来源：http://vik.meibo888.top

Ruby: return if data.nil?
来源：http://dkc.tarul.cn

C#:   if (data == null) return;
来源：http://jna.yanxiufei.cn

================================================================================
来源：http://xms.uphjek.com

C. 函数与作用域
来源：http://buk.chenjidiqi.icu

================================================================================
来源：http://wqh.dashuyun.cn

[C01] 定义函数
来源：http://spz.cheryme.top

Py:   def add(a, b): return a + b
来源：http://yve.nanxinkj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nnm.zhoulong.xyz

JS:   function add(a, b) { return a + b; }
来源：http://zcx.vehdjk.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rrv.zdqjudy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://goc.ivvv.top

Go:   func add(a, b int) int { return a + b }
来源：http://lsi.yj20258888.top

Ruby: def add(a, b); a + b; end
来源：http://jny.xingfuxueyuan.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cxt.xuanzx.com

[C02] 默认参数
来源：http://awb.jinqigufen.top

Py:   def greet(name="World"): return name
来源：http://dyq.cheryme.top

PHP:  function greet($name = "World") { return $name; }
来源：http://jqm.bjfxy.top

JS:   function greet(name = "World") { return name; }
来源：http://oel.sjlbkw.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ynv.hesvh.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ijg.yanxiufei.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://uqn.xylfe.cn

Ruby: def greet(name = "World") = name
来源：http://eeh.c1oappe.top

C#:   string Greet(string name = "World") => name;
来源：http://zxg.zhongyouzk.top

[C03] 可变参数
来源：http://mnu.xziqi.cn

Py:   def total(*args): return sum(args)
来源：http://xcs.ehwqpu.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ywa.guannengcc.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://avr.316326.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bms.shangyingyoupin.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gqj.snrcjt.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://upv.yfazqb.com

Ruby: def total(*nums); nums.sum; end
来源：http://ivm.hfpthk.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://moc.tianlin.xyz

[C04] 命名参数 / 关键字参数
来源：http://rld.xinyue.icu

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gqe.c1oappe.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xqg.cqqwz.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vkq.xylfe.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lec.quarkkingdee.top

Java: // 无：用 Builder 模式或 record
来源：http://ixt.cqqwz.cn

Go:   // 无：用配置结构体参数
来源：http://mnq.guannengcc.top

Ruby: f(a: 1, b: 2)
来源：http://eyl.fengsongda.top

C#:   f(a: 1, b: 2)
来源：http://dsr.nwbrower.top

[C05] 返回多个值
来源：http://phj.zhaomingkeji.xyz

Py:   return a, b
来源：http://dgi.yangfankeji.com

PHP:  return [$a, $b];
来源：http://oty.fzhhl.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://bte.316326.xyz

TS:   return { a, b };
来源：http://cyz.haohaochexian.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kyq.cdnleiting.top

Go:   return a, b
来源：http://ust.meibo888.top

Ruby: return a, b
来源：http://hir.yangfankeji.com

C#:   return (a, b);              // ValueTuple
来源：http://fgb.tianlin.xyz

[C06] 匿名函数 / lambda
来源：http://syx.bbcook.cn

Py:   square = lambda x: x * x
来源：http://wyi.zhongyouzk.top

PHP:  $square = fn($x) => $x * $x;
来源：http://mic.sweek.top

JS:   const square = x => x * x;
来源：http://roh.yanxiufei.cn

TS:   const square = (x: number): number => x * x;
来源：http://lav.meibo888.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ene.aizwys.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dyi.hywenlv.cn

Ruby: square = ->(x) { x * x }
来源：http://yue.xingfuxueyuan.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://tdh.andypj.xyz

[C07] 把函数作为参数传入
来源：http://ksq.shuidangran.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yjw.chenzaomai.com

PHP:  array_map("strtoupper", $arr);
来源：http://iox.meibo888.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cpd.ivvv.top

TS:   arr.map(String)
来源：http://pkd.xinyue.icu

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://deb.yuxming.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tek.52xcode.cn

Ruby: arr.map(&:upcase)
来源：http://tyy.andypj.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://ymx.hfpthk.cn

[C08] 闭包
来源：http://wfh.shangyingyoupin.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://idi.yuxming.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uin.guowangkeji.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ezl.xziqi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://znf.zhijiandao.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ceg.zhoulong.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bts.hcnkem.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cbs.yangfankeji.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nkf.shanyushiyangtech.top

[C09] 递归
来源：http://kwe.hnxiangtu.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://puf.smart0.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uqw.jinyuanbaomall.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kpf.chenzaomai.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ikc.guowangkeji.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ycp.tianlin.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pub.fzhhl.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nen.andypj.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sbh.shangyingyoupin.top

[C10] 变量作用域
来源：http://vue.pengpengdd.cyou

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ejx.gotoacloud.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yig.shanyushiyangkeji.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ilh.chenzaomai.com

TS:   同 JS
来源：http://ayv.jyoumei.cn

Java: 方法内为块级作用域
来源：http://rxh.sjlbkw.cn

Go:   花括号块级作用域
来源：http://vkt.yfazqb.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ttp.jinqigfzy.top

C#:   块级作用域
来源：http://gwi.fktsv.cn

[C11] 模块导入与导出
来源：http://wil.wangdashe.top

Py:   from module import func
来源：http://hrk.sjlbkw.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zqj.meibo888.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ini.shuidangran.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://muh.yj202588.top

Java: import java.util.List;
来源：http://yrc.gogol.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nwb.hongshengwenyu.top

Ruby: require "json"; require_relative "./util"
来源：http://egk.yvedp.cn

C#:   using System.Text;
来源：http://dws.daria6918.cn

[C12] 立即执行函数 IIFE
来源：http://xzw.nanxuanxn.top

Py:   (lambda: print("run"))()
来源：http://zmn.uphjek.com

PHP:  (function () { echo "run"; })();
来源：http://lik.jqgfzy.top

JS:   (() => { console.log("run"); })();
来源：http://ihv.kuanghao11.cn

TS:   (() => { console.log("run"); })();
来源：http://yzp.hnxiangtu.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://chc.sysykeji.top

Go:   func() { fmt.Println("run") }()
来源：http://opx.c1oappe.top

Ruby: -> { puts "run" }.call
来源：http://ubd.svipenyu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qgv.chenjidiqi.icu

[C13] 类型声明 / 类型注解
来源：http://xcr.zycfv.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xdi.nanxinkj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bvk.c1oappe.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ete.yj20258888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qxh.xziqi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://tak.jyoumei.cn

Go:   func add(a, b int) int
来源：http://djk.shuidangran.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tpc.yanxiufei.cn

C#:   int Add(int a, int b) => a + b;
来源：http://emu.epnwcf.com

[C14] 泛型函数
来源：http://dte.nanxuanxn.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://liw.shuidangran.top

PHP:  // 无泛型
来源：http://pax.xingfuxueyuan.xyz

JS:   // 无泛型
来源：http://lin.hesvh.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kdm.zhixingplan.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uxg.chenlongwang.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bgg.hcnkem.com

Ruby: # 无泛型
来源：http://iox.yfazqb.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ext.zhiwuduotai.top

[C15] 解构 / 展开参数
来源：http://pdg.ywan-chungtsiang.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://oim.jinghuilouyu.cn

PHP:  [$a, $b] = $pair;
来源：http://yhv.gogol.net.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://iwn.jiagoushi.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jla.smart0.xyz

Java: // 无解构
来源：http://lin.zycfv.cn

Go:   // 无解构
来源：http://tbn.zdbjq.cn

Ruby: a, b = pair
来源：http://ymh.hesvh.cn

C#:   var (a, b) = pair;
来源：http://bhh.yonumen.top

[C16] 函数 / 方法重载
来源：http://myj.andypj.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gab.jiagoushi.top

PHP:  // 无重载
来源：http://oin.tianlin.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://lyc.jiagoushi.top

TS:   // 用联合类型或重载签名声明
来源：http://khg.gotoacloud.top

Java: void f(int a) {}  void f(String a) {}
来源：http://kkh.snrcjt.cn

Go:   // 无重载：用不同函数名
来源：http://thv.jlsjyb.cn

Ruby: # 无重载：靠动态参数
来源：http://rgv.hysaishi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://aaa.yj20258.top

================================================================================
来源：http://lak.yueranfly.top

D. 数组 / 列表 / 集合
来源：http://qsc.yonumen.top

================================================================================
来源：http://wtu.gzhubu.top

[D01] 创建数组 / 列表
来源：http://pkj.tian-w.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://dww.zhijiandao.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://txx.ehwqpu.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vfn.redwolf501.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ron.aizwys.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rrj.yj202588.top

Go:   arr := []int{1, 2, 3}
来源：http://jam.wangdashe.top

Ruby: arr = [1, 2, 3]
来源：http://eeb.shangyingyoupin.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nmu.xziqi.cn

[D02] 追加元素到末尾
来源：http://vuo.daxiang520.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yad.chenlongwang.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://uqy.sufxvd.cn

JS:   arr.push(4);
来源：http://hec.c1oappe.top

TS:   arr.push(4);
来源：http://xzs.tarul.cn

Java: list.add(4);
来源：http://rpo.ydzc1.top

Go:   arr = append(arr, 4)
来源：http://jzp.52xcode.cn

Ruby: arr << 4; arr.push(5)
来源：http://ybm.zhengqikj.top

C#:   list.Add(4);
来源：http://jaz.wangdashe.top

[D03] 在指定位置插入元素
来源：http://pgg.tian-w.cn

Py:   arr.insert(0, 0)
来源：http://sgr.uphjek.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xmo.hesvh.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xgh.zdbjq.cn

TS:   arr.splice(0, 0, 0);
来源：http://fhm.hywenlv.cn

Java: list.add(0, 0);
来源：http://boy.daria6918.cn

Go:   arr = append([]int{0}, arr...)
来源：http://srd.yuanzhike.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jok.gzhubu.top

C#:   list.Insert(0, 0);
来源：http://bzs.hammf.cn

[D04] 删除元素
来源：http://jxq.zycfv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://avz.nanxuanxn.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qgq.chenzaomai.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kbb.yuanzhike.top

TS:   arr.splice(0, 1);
来源：http://zoz.jinqigfzy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://knc.zhixingplan.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mmr.cheryme.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lig.0kj1m.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gvz.hcnkem.com

[D05] 访问与修改元素
来源：http://hkf.cqqwz.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mhd.yueranfly.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bhp.sysykeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ndp.zhiwuduotai.top

TS:   arr[0]; arr.at(-1);
来源：http://zex.zdbjq.cn

Java: list.get(0); list.set(0, 9);
来源：http://app.sysykeji.top

Go:   arr[0]; arr[0] = 9
来源：http://hls.fanxiaobao.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://epz.9152youxi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hah.jiagoushi.top

[D06] 数组长度
来源：http://sxj.fehbvm.com

Py:   len(arr)
来源：http://kxb.jinghuilouyu.cn

PHP:  count($arr);
来源：http://zzc.jianghu66.top

JS:   arr.length
来源：http://scn.zhijiandao.cn

TS:   arr.length
来源：http://uet.fehbvm.com

Java: list.size();
来源：http://qxi.chenzaomai.com

Go:   len(arr)
来源：http://tot.zhoulong.xyz

Ruby: arr.length; arr.size
来源：http://aeb.bjfxy.top

C#:   list.Count;
来源：http://lkn.guowangkeji.top

[D07] 切片 / 取子数组
来源：http://vgx.fanxiaobao.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zel.zhoulong.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://ktw.yuxming.cn

JS:   arr.slice(1, 4);
来源：http://urh.iojbl.cn

TS:   arr.slice(1, 4);
来源：http://yng.dashuyun.cn

Java: list.subList(1, 4);
来源：http://xol.hcnkem.com

Go:   arr[1:4]
来源：http://xej.sysykeji.top

Ruby: arr[1, 3]
来源：http://rlt.sxryk.cn

C#:   list.GetRange(1, 3);
来源：http://zkq.316326.xyz

[D08] 合并两个数组
来源：http://tgz.yangfankeji.com

Py:   a + b;  a.extend(b)
来源：http://pjc.zhijiandao.cn

PHP:  array_merge($a, $b);
来源：http://hxd.jinqigufen.top

JS:   [...a, ...b];  a.concat(b);
来源：http://aya.hnxiangtu.top

TS:   [...a, ...b];
来源：http://avn.yuxming.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hna.yj20258888.top

Go:   append(a, b...)
来源：http://imr.jinyuanbaomall.cn

Ruby: a + b;  a.concat(b)
来源：http://wyx.jinghuilouyu.cn

C#:   a.Concat(b).ToList()
来源：http://nlp.yonumen.top

[D09] 排序（升序）
来源：http://xdc.fzhhl.top

Py:   sorted(arr);  arr.sort()
来源：http://yfv.cashguo.top

PHP:  sort($arr);
来源：http://xrg.jinyuanbaomall.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://piv.nanxuanxn.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://wqr.chenjidiqi.icu

Java: Collections.sort(list);  list.sort(null);
来源：http://pur.sweek.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xrz.bjfxy.top

Ruby: arr.sort
来源：http://wtw.ctjpmb.com

C#:   list.Sort();
来源：http://xbe.jianghu66.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://pfk.gzhubu.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fry.nanxinkj.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pri.yj20258888.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://uhq.cashguo.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xkr.yj20258888.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vem.hfpthk.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://phy.ppjwa.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ydn.svipenyu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fcd.sweek.top

[D11] 反转数组
来源：http://ymh.yangfankeji.com

Py:   arr[::-1];  arr.reverse()
来源：http://oyv.bjfxy.top

PHP:  array_reverse($arr);
来源：http://hlx.quarkkingdee.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xgc.jyoumei.cn

TS:   [...arr].reverse();
来源：http://dih.tanke756.top

Java: Collections.reverse(list);
来源：http://kml.aizwys.cn

Go:   slices.Reverse(arr)
来源：http://bfe.zhaomingkeji.xyz

Ruby: arr.reverse
来源：http://hfk.wangdashe.top

C#:   list.Reverse();
来源：http://bou.shangyingyoupin.top

[D12] 查找元素下标
来源：http://jjg.dashuyun.cn

Py:   arr.index(x);  x in arr
来源：http://vdz.hongshengwenyu.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://row.cqqwz.cn


<!-- 参考信息 -->
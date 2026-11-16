代发 wailian999

[B13] 判断是否为数字
来源：http://arx.jqgfzy.top

Py:   isinstance(x, (int, float))
来源：http://xrj.bjfxy.top

PHP:  is_numeric($x)
来源：http://efe.hnqzz.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vrm.cqqwz.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://evt.jinghuilouyu.cn

Java: x instanceof Number
来源：http://zfo.hammf.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gdp.quarkkingdee.top

Ruby: x.is_a?(Numeric)
来源：http://wwh.aizwys.cn

C#:   x is int or double or decimal
来源：http://tpj.9152youxi.cn

[B14] 判断值是否在集合内
来源：http://gks.tanke756.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qbx.zhaomingkeji.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cty.jinqigfzy.top

JS:   [1, 2, 3].includes(x)
来源：http://fkd.zhaomingkeji.xyz

TS:   [1, 2, 3].includes(x)
来源：http://cbb.yuanzhike.top

Java: List.of(1, 2, 3).contains(x)
来源：http://nsp.fktsv.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ybp.xuanzx.com

Ruby: [1, 2, 3].include?(x)
来源：http://cxa.gotoacloud.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mmw.dashuyun.cn

[B15] 布尔运算与取反
来源：http://evp.fzhhl.top

Py:   a and b or not c
来源：http://shj.yuxming.cn

PHP:  $a && $b || !$c
来源：http://qfn.jqgfzy.top

JS:   a && b || !c
来源：http://afa.xinyue.icu

TS:   a && b || !c
来源：http://lyu.cheryme.top

Java: a && b || !c
来源：http://wqv.jinghuilouyu.cn

Go:   a && b || !c
来源：http://xqg.shuidangran.top

Ruby: a && b || !c
来源：http://zwa.yj20258888.top

C#:   a && b || !c
来源：http://zap.gotoacloud.top

[B16] 卫语句：不满足条件提前返回
来源：http://zwy.yj20258888.top

Py:   if not data: return
来源：http://omb.zdqjudy.top

PHP:  if (!$data) { return; }
来源：http://loe.pengpengdd.cyou

JS:   if (!data) return;
来源：http://rnv.bbcook.cn

TS:   if (!data) return;
来源：http://uhh.xinyue.icu

Java: if (data == null) return;
来源：http://bix.fanxiaobao.xyz

Go:   if data == nil { return }
来源：http://ebi.xuetiantiany.cn

Ruby: return if data.nil?
来源：http://uqy.kuanghao11.cn

C#:   if (data == null) return;
来源：http://alo.daxiang520.top

================================================================================
来源：http://ilc.ehwqpu.com

C. 函数与作用域
来源：http://pry.shanyushiyangtech.top

================================================================================
来源：http://aae.vehdjk.com

[C01] 定义函数
来源：http://eda.hammf.cn

Py:   def add(a, b): return a + b
来源：http://dte.redwolf501.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hgh.zdqjudy.top

JS:   function add(a, b) { return a + b; }
来源：http://tpo.pengpengdd.cyou

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ekv.fanxiaobao.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://zva.9152youxi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dcl.gotoacloud.top

Ruby: def add(a, b); a + b; end
来源：http://ccw.bjfxy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mau.quarkkingdee.top

[C02] 默认参数
来源：http://qfr.xylfe.cn

Py:   def greet(name="World"): return name
来源：http://kwl.xinyue.icu

PHP:  function greet($name = "World") { return $name; }
来源：http://fuf.316326.xyz

JS:   function greet(name = "World") { return name; }
来源：http://xnr.xinyue.icu

TS:   function greet(name: string = "World") { return name; }
来源：http://ucx.zhixingplan.top

Java: // 无默认参数：方法重载或 Optional
来源：http://smw.bjfxy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yov.zhiwuduotai.top

Ruby: def greet(name = "World") = name
来源：http://fkh.xingfuxueyuan.xyz

C#:   string Greet(string name = "World") => name;
来源：http://mqa.cucudq.cn

[C03] 可变参数
来源：http://ecn.hnqzz.top

Py:   def total(*args): return sum(args)
来源：http://rud.jqgfzy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://trp.aibaodan.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ytk.tarul.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nrz.yuanzhike.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mza.jqgufenzy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kxd.hnqzz.top

Ruby: def total(*nums); nums.sum; end
来源：http://jtj.aibaodan.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tvz.jqgfzy.top

[C04] 命名参数 / 关键字参数
来源：http://pyp.tianlin.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gqm.jqgufenzy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vyb.sxryk.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://quw.tarul.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kqn.xuanzx.com

Java: // 无：用 Builder 模式或 record
来源：http://sqr.yj202588.top

Go:   // 无：用配置结构体参数
来源：http://iro.zhaomingkeji.xyz

Ruby: f(a: 1, b: 2)
来源：http://wuj.zdbjq.cn

C#:   f(a: 1, b: 2)
来源：http://kjq.shuidangran.top

[C05] 返回多个值
来源：http://csu.zhongyouzk.top

Py:   return a, b
来源：http://ken.hnqzz.top

PHP:  return [$a, $b];
来源：http://mvt.jqgfzy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://xir.sweek.top

TS:   return { a, b };
来源：http://dmf.zhiwuduotai.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hll.chenzaomai.com

Go:   return a, b
来源：http://wgj.fanxiaobao.xyz

Ruby: return a, b
来源：http://loi.fktsv.cn

C#:   return (a, b);              // ValueTuple
来源：http://mvo.ywan-chungtsiang.top

[C06] 匿名函数 / lambda
来源：http://poc.jianghu66.top

Py:   square = lambda x: x * x
来源：http://nwi.yj202588.top

PHP:  $square = fn($x) => $x * $x;
来源：http://clt.chenlongwang.top

JS:   const square = x => x * x;
来源：http://xxq.aizwys.cn

TS:   const square = (x: number): number => x * x;
来源：http://xrj.smart0.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://eki.316326.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://twp.52xcode.cn

Ruby: square = ->(x) { x * x }
来源：http://ork.aibaodan.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wtv.jiagoushi.top

[C07] 把函数作为参数传入
来源：http://mgi.sjlbkw.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bls.zdqjudy.top

PHP:  array_map("strtoupper", $arr);
来源：http://uwr.ybcxt.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ogm.birdmap.top

TS:   arr.map(String)
来源：http://ptm.xuetiantiany.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hrg.yanxiufei.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ndf.svipenyu.cn

Ruby: arr.map(&:upcase)
来源：http://psx.yj202588.top

C#:   arr.Select(s => s.ToUpper())
来源：http://xaz.shanyushiyangkeji.top

[C08] 闭包
来源：http://ngi.0kj1m.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://abf.52xcode.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gvt.fengsongda.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yij.nwbrower.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mjk.hnqzz.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://whh.xylfe.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wqx.iojbl.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kvu.cqqwz.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dxc.wangdashe.top

[C09] 递归
来源：http://ayy.wangshuangyany.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dcx.gotoacloud.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jsw.zhixingplan.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kds.shangyingyoupin.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dmm.yuxming.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yus.daxiang520.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cuy.snrcjt.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dpa.yangfankeji.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fbj.xuanzx.com

[C10] 变量作用域
来源：http://mzo.sxryk.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://njk.316326.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qdo.guowangkeji.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://knr.aibaodan.cn

TS:   同 JS
来源：http://dij.hnxiangtu.top

Java: 方法内为块级作用域
来源：http://vac.jinqigfzy.top

Go:   花括号块级作用域
来源：http://boz.cqqwz.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kzb.cheryme.top

C#:   块级作用域
来源：http://jyg.jiagoushi.top

[C11] 模块导入与导出
来源：http://mmf.nanxinkj.top

Py:   from module import func
来源：http://djz.sjlbkw.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://lnp.mhx1999.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://kma.fzhhl.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fcb.hesvh.cn

Java: import java.util.List;
来源：http://atg.sysykeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zcf.ydjk.org.cn

Ruby: require "json"; require_relative "./util"
来源：http://ogq.hcnkem.com

C#:   using System.Text;
来源：http://jgt.jianghu66.top

[C12] 立即执行函数 IIFE
来源：http://vel.yuxming.cn

Py:   (lambda: print("run"))()
来源：http://tib.ppjwa.cn

PHP:  (function () { echo "run"; })();
来源：http://ahi.zhoulong.xyz

JS:   (() => { console.log("run"); })();
来源：http://dxd.yuxming.cn

TS:   (() => { console.log("run"); })();
来源：http://xji.ydjk.org.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ghd.zhengqikj.top

Go:   func() { fmt.Println("run") }()
来源：http://txf.dianchejie.cn

Ruby: -> { puts "run" }.call
来源：http://dcv.jinghuilouyu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://nxy.jinghuilouyu.cn

[C13] 类型声明 / 类型注解
来源：http://mck.jiagoushi.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rfm.vqdsnc.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kex.vqdsnc.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cje.jinqigufen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vxv.ctjpmb.com

Java: int add(int a, int b) { return a + b; }
来源：http://kjo.dashuyun.cn

Go:   func add(a, b int) int
来源：http://ond.jlsjyb.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dxe.jiagoushi.top

C#:   int Add(int a, int b) => a + b;
来源：http://qnm.andypj.xyz

[C14] 泛型函数
来源：http://bgy.daria6918.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gjs.sysykeji.top

PHP:  // 无泛型
来源：http://zrr.xuetiantiany.cn

JS:   // 无泛型
来源：http://uno.shangyingyoupin.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lsk.shzxlz.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bbx.jinqigufen.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://drz.wangshuangyany.cn

Ruby: # 无泛型
来源：http://lhf.jyoumei.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sii.vehdjk.com

[C15] 解构 / 展开参数
来源：http://cio.chenjidiqi.icu

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ned.zhengqikj.top

PHP:  [$a, $b] = $pair;
来源：http://oix.jinqigfzy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vga.fehbvm.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://iot.fehbvm.com

Java: // 无解构
来源：http://foy.aibaodan.cn

Go:   // 无解构
来源：http://pga.xinyue.icu

Ruby: a, b = pair
来源：http://xau.sjlbkw.cn

C#:   var (a, b) = pair;
来源：http://hed.yuanzhike.top

[C16] 函数 / 方法重载
来源：http://eut.hnxiangtu.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zku.jinqigufen.top

PHP:  // 无重载
来源：http://fww.hywenlv.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://oxz.zhiwuduotai.top

TS:   // 用联合类型或重载签名声明
来源：http://svb.xinyue.icu

Java: void f(int a) {}  void f(String a) {}
来源：http://mki.redwolf501.top

Go:   // 无重载：用不同函数名
来源：http://zcb.pycfn.com

Ruby: # 无重载：靠动态参数
来源：http://okq.jianghu66.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://bmz.wangshuangyany.cn

================================================================================
来源：http://gkp.jiagoushi.top

D. 数组 / 列表 / 集合
来源：http://mvd.yj20258888.top

================================================================================
来源：http://dfy.zhixingplan.top

[D01] 创建数组 / 列表
来源：http://qdm.sxryk.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zrn.jlsjyb.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://swg.nanxuanxn.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hbi.iojbl.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kgw.yuanzhike.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hou.yfazqb.com

Go:   arr := []int{1, 2, 3}
来源：http://uwt.jinyuanbaomall.cn

Ruby: arr = [1, 2, 3]
来源：http://xrr.52xcode.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nnl.jianghu66.top

[D02] 追加元素到末尾
来源：http://cvs.snrcjt.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ycz.snrcjt.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mgk.zhoulong.xyz

JS:   arr.push(4);
来源：http://mlu.cashguo.top

TS:   arr.push(4);
来源：http://opr.dashuyun.cn

Java: list.add(4);
来源：http://khr.vqdsnc.cn

Go:   arr = append(arr, 4)
来源：http://ylo.birdmap.top

Ruby: arr << 4; arr.push(5)
来源：http://xtx.wangshuangyany.cn

C#:   list.Add(4);
来源：http://vmu.daria6918.cn

[D03] 在指定位置插入元素
来源：http://fuk.52xcode.cn

Py:   arr.insert(0, 0)
来源：http://mgu.xingfuxueyuan.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vuw.ywan-chungtsiang.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ios.chenlongwang.top

TS:   arr.splice(0, 0, 0);
来源：http://gpc.haohaochexian.top

Java: list.add(0, 0);
来源：http://qwv.chenjidiqi.icu

Go:   arr = append([]int{0}, arr...)
来源：http://rpm.zdbjq.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xnp.zhixingplan.top

C#:   list.Insert(0, 0);
来源：http://rjb.zhijiandao.cn

[D04] 删除元素
来源：http://ywd.shanyushiyangtech.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://isf.yj202588.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mmr.smart0.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kwk.jqgfzy.top

TS:   arr.splice(0, 1);
来源：http://sju.0kj1m.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yam.gogol.net.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ywa.bjfxy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xea.316326.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vgp.hysaishi.cn

[D05] 访问与修改元素
来源：http://mgt.jyoumei.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jgp.ydzc1.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kin.zhengqikj.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ikf.zycfv.cn

TS:   arr[0]; arr.at(-1);
来源：http://esk.hysaishi.cn

Java: list.get(0); list.set(0, 9);
来源：http://iny.pycfn.com

Go:   arr[0]; arr[0] = 9
来源：http://xtn.cqqwz.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nuh.hesvh.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wql.0kj1m.cn

[D06] 数组长度
来源：http://viu.tarul.cn

Py:   len(arr)
来源：http://ivm.gaohongyu789.top

PHP:  count($arr);
来源：http://igq.hysaishi.cn

JS:   arr.length
来源：http://qgb.dashuyun.cn

TS:   arr.length
来源：http://vqr.dashuyun.cn

Java: list.size();
来源：http://vmn.epnwcf.com

Go:   len(arr)
来源：http://kmp.yonumen.top

Ruby: arr.length; arr.size
来源：http://bom.yj20258888.top

C#:   list.Count;
来源：http://gvk.shangyingyoupin.top

[D07] 切片 / 取子数组
来源：http://sue.yj20258.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dqk.yanxiufei.cn

PHP:  array_slice($arr, 1, 3);
来源：http://say.svipenyu.cn

JS:   arr.slice(1, 4);
来源：http://dnh.gaohongyu789.top

TS:   arr.slice(1, 4);
来源：http://mki.shangyingyoupin.top

Java: list.subList(1, 4);
来源：http://nvk.zhijiandao.cn

Go:   arr[1:4]
来源：http://kbo.mhx1999.top

Ruby: arr[1, 3]
来源：http://paf.gaohongyu789.top

C#:   list.GetRange(1, 3);
来源：http://ixk.ywan-chungtsiang.top

[D08] 合并两个数组
来源：http://hsv.guowangkeji.top

Py:   a + b;  a.extend(b)
来源：http://iwa.jinqigufen.top

PHP:  array_merge($a, $b);
来源：http://ope.haohaochexian.top

JS:   [...a, ...b];  a.concat(b);
来源：http://xlp.smart0.xyz

TS:   [...a, ...b];
来源：http://yap.zdbjq.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jfa.shuidangran.top

Go:   append(a, b...)
来源：http://puq.xinyue.icu

Ruby: a + b;  a.concat(b)
来源：http://vio.fengsongda.top

C#:   a.Concat(b).ToList()
来源：http://xvo.jqgfzy.top

[D09] 排序（升序）
来源：http://vpp.gaohongyu789.top

Py:   sorted(arr);  arr.sort()
来源：http://lkq.smart0.xyz

PHP:  sort($arr);
来源：http://vnw.daxiang520.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mkv.dianchejie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gmh.jinyuanbaomall.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mrh.9152youxi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zpa.guannengcc.top

Ruby: arr.sort
来源：http://qmq.zdbjq.cn

C#:   list.Sort();
来源：http://bdr.wangdashe.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://pxo.cucudq.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://czj.andypj.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ajq.fanxiaobao.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zzj.ctjpmb.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ivu.ppjwa.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qjk.cucudq.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://oxq.ydjk.org.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yfy.jinyuanbaomall.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://max.aibaodan.cn

[D11] 反转数组
来源：http://ejo.ywan-chungtsiang.top

Py:   arr[::-1];  arr.reverse()
来源：http://xym.ivvv.top

PHP:  array_reverse($arr);
来源：http://skx.gogol.net.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bhv.svipenyu.cn

TS:   [...arr].reverse();
来源：http://vzz.sweek.top

Java: Collections.reverse(list);
来源：http://lbk.epnwcf.com

Go:   slices.Reverse(arr)
来源：http://hib.jinqigufen.top

Ruby: arr.reverse
来源：http://rar.meibo888.top

C#:   list.Reverse();
来源：http://rgy.xuanzx.com

[D12] 查找元素下标
来源：http://jky.nwbrower.top

Py:   arr.index(x);  x in arr
来源：http://qkf.zhoulong.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wrm.yuxming.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://enh.pengpengdd.cyou

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jyp.yonumen.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vzc.cheryme.top

Go:   slices.Index(arr, x)
来源：http://wkm.ivvv.top

Ruby: arr.index(x)
来源：http://sno.hnxiangtu.top

C#:   list.IndexOf(x);
来源：http://axp.redwolf501.top

[D13] 过滤（保留满足条件的）
来源：http://dni.hywenlv.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nhh.wangdashe.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://efs.tanke756.top

JS:   arr.filter(x => x > 3)
来源：http://xjz.316326.xyz

TS:   arr.filter(x => x > 3)
来源：http://veo.meibo888.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jlj.xylfe.cn


<!-- 参考信息 -->
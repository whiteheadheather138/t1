代发 wailian999

C#:   x is int or double or decimal
来源：http://nvk.vehdjk.com

[B14] 判断值是否在集合内
来源：http://jaa.chenzaomai.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dlw.zycfv.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vym.ctjpmb.com

JS:   [1, 2, 3].includes(x)
来源：http://uho.pengpengdd.cyou

TS:   [1, 2, 3].includes(x)
来源：http://suc.fanxiaobao.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://dgi.yj20258888.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://eru.fanxiaobao.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://iik.zhoulong.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ljf.svipenyu.cn

[B15] 布尔运算与取反
来源：http://noy.cdnleiting.top

Py:   a and b or not c
来源：http://jcy.daria6918.cn

PHP:  $a && $b || !$c
来源：http://cfo.sjlbkw.cn

JS:   a && b || !c
来源：http://jzn.shzxlz.cn

TS:   a && b || !c
来源：http://cbl.havefunace.top

Java: a && b || !c
来源：http://lxt.xuanzx.com

Go:   a && b || !c
来源：http://blb.guowangkeji.top

Ruby: a && b || !c
来源：http://nya.fengsongda.top

C#:   a && b || !c
来源：http://szg.tianlin.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://ebg.hammf.cn

Py:   if not data: return
来源：http://vpc.fanxiaobao.xyz

PHP:  if (!$data) { return; }
来源：http://uve.uphjek.com

JS:   if (!data) return;
来源：http://ebp.zycfv.cn

TS:   if (!data) return;
来源：http://ttq.xylfe.cn

Java: if (data == null) return;
来源：http://haj.xylfe.cn

Go:   if data == nil { return }
来源：http://unt.yfazqb.com

Ruby: return if data.nil?
来源：http://xkp.uphjek.com

C#:   if (data == null) return;
来源：http://eqv.hcnkem.com

================================================================================
来源：http://gdq.bjfxy.top

C. 函数与作用域
来源：http://onr.svipenyu.cn

================================================================================
来源：http://epi.jinyuanbaomall.cn

[C01] 定义函数
来源：http://gny.tian-w.cn

Py:   def add(a, b): return a + b
来源：http://pty.zhijiandao.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://squ.cashguo.top

JS:   function add(a, b) { return a + b; }
来源：http://dlh.zhengqikj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nna.cucudq.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gwv.hysaishi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ehi.shangyingyoupin.top

Ruby: def add(a, b); a + b; end
来源：http://nzq.ivvv.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://muk.yanxiufei.cn

[C02] 默认参数
来源：http://hny.hysaishi.cn

Py:   def greet(name="World"): return name
来源：http://nur.fehbvm.com

PHP:  function greet($name = "World") { return $name; }
来源：http://itu.jianghu66.top

JS:   function greet(name = "World") { return name; }
来源：http://osl.yvedp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://eog.yfazqb.com

Java: // 无默认参数：方法重载或 Optional
来源：http://oly.zhaomingkeji.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://oku.fengsongda.top

Ruby: def greet(name = "World") = name
来源：http://xtg.yfazqb.com

C#:   string Greet(string name = "World") => name;
来源：http://hid.sweek.top

[C03] 可变参数
来源：http://ktq.gzhubu.top

Py:   def total(*args): return sum(args)
来源：http://czf.zhoulong.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ucr.hcnkem.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://srm.jyoumei.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zrt.xuanzx.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wqu.hammf.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://olw.svipenyu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://epo.fengsongda.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mbu.svipenyu.cn

[C04] 命名参数 / 关键字参数
来源：http://ugv.epnwcf.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hye.yj20258.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yxg.dianchejie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cdr.ydzc1.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://oir.sufxvd.cn

Java: // 无：用 Builder 模式或 record
来源：http://kjt.yj20258.top

Go:   // 无：用配置结构体参数
来源：http://pev.yj20258888.top

Ruby: f(a: 1, b: 2)
来源：http://gdg.yanxiufei.cn

C#:   f(a: 1, b: 2)
来源：http://bfx.iojbl.cn

[C05] 返回多个值
来源：http://qgp.jinqigufen.top

Py:   return a, b
来源：http://fgr.snrcjt.cn

PHP:  return [$a, $b];
来源：http://xil.jinqigufen.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ois.gaohongyu789.top

TS:   return { a, b };
来源：http://fec.shuidangran.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kdp.fanxiaobao.xyz

Go:   return a, b
来源：http://qon.0kj1m.cn

Ruby: return a, b
来源：http://uzd.yj20258888.top

C#:   return (a, b);              // ValueTuple
来源：http://spe.zycfv.cn

[C06] 匿名函数 / lambda
来源：http://xhu.sweek.top

Py:   square = lambda x: x * x
来源：http://iqp.hysaishi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://mbt.zdqjudy.top

JS:   const square = x => x * x;
来源：http://dej.yvedp.cn

TS:   const square = (x: number): number => x * x;
来源：http://gbo.shanyushiyangkeji.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://msx.bbcook.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fcj.ydjk.org.cn

Ruby: square = ->(x) { x * x }
来源：http://tni.yongpay.top

C#:   Func<int, int> square = x => x * x;
来源：http://vrd.52xcode.cn

[C07] 把函数作为参数传入
来源：http://loj.kuanghao11.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kbw.ivvv.top

PHP:  array_map("strtoupper", $arr);
来源：http://sqd.daxiang520.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rpc.yj202588.top

TS:   arr.map(String)
来源：http://prh.chenlongwang.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zmg.cashguo.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://txd.wangshuangyany.cn

Ruby: arr.map(&:upcase)
来源：http://hbr.shuidangran.top

C#:   arr.Select(s => s.ToUpper())
来源：http://hhh.zdqjudy.top

[C08] 闭包
来源：http://gjv.ppjwa.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fof.cucudq.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tkn.kuanghao11.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gtm.zhoulong.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pub.zycfv.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cai.iojbl.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bwd.smart0.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bws.jyoumei.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nvt.ehwqpu.com

[C09] 递归
来源：http://ehy.zhixingplan.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pga.shangyingyoupin.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ofd.yfazqb.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://osp.tarul.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dpt.sxryk.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ywy.yvedp.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kyj.chenlongwang.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uvv.redwolf501.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vln.vehdjk.com

[C10] 变量作用域
来源：http://olh.hesvh.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dmj.jinqigfzy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vyk.hysaishi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tbv.jinqigfzy.top

TS:   同 JS
来源：http://qrf.dianchejie.cn

Java: 方法内为块级作用域
来源：http://lpf.yongpay.top

Go:   花括号块级作用域
来源：http://qja.jinyuanbaomall.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://axk.ppjwa.cn

C#:   块级作用域
来源：http://xsv.yuanzhike.top

[C11] 模块导入与导出
来源：http://hbf.gaohongyu789.top

Py:   from module import func
来源：http://yty.nanxuanxn.top

PHP:  require "file.php";  或 use App\Service;
来源：http://vow.nanxuanxn.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://qui.sufxvd.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jey.shangyingyoupin.top

Java: import java.util.List;
来源：http://gwj.pycfn.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ngt.bjfxy.top

Ruby: require "json"; require_relative "./util"
来源：http://dtj.sysykeji.top

C#:   using System.Text;
来源：http://tjg.yongpay.top

[C12] 立即执行函数 IIFE
来源：http://bsz.jyoumei.cn

Py:   (lambda: print("run"))()
来源：http://tns.yanxiufei.cn

PHP:  (function () { echo "run"; })();
来源：http://orl.yuxming.cn

JS:   (() => { console.log("run"); })();
来源：http://nyc.sysykeji.top

TS:   (() => { console.log("run"); })();
来源：http://yup.ywan-chungtsiang.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vzc.jianghu66.top

Go:   func() { fmt.Println("run") }()
来源：http://fuw.yongpay.top

Ruby: -> { puts "run" }.call
来源：http://izm.fengsongda.top

C#:   // 无 IIFE：用静态构造函数
来源：http://amk.sysykeji.top

[C13] 类型声明 / 类型注解
来源：http://fmd.hammf.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lws.vehdjk.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nqc.shangyingyoupin.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rix.chenzaomai.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qqw.redwolf501.top

Java: int add(int a, int b) { return a + b; }
来源：http://isn.bbcook.cn

Go:   func add(a, b int) int
来源：http://hij.epnwcf.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lws.52xcode.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ezc.zhoulong.xyz

[C14] 泛型函数
来源：http://bys.shuidangran.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sbx.uphjek.com

PHP:  // 无泛型
来源：http://ipu.tanke756.top

JS:   // 无泛型
来源：http://wiz.9152youxi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rjn.daxiang520.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mdp.yfazqb.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mls.sufxvd.cn

Ruby: # 无泛型
来源：http://tab.cdnleiting.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qii.jqgfzy.top

[C15] 解构 / 展开参数
来源：http://btw.9152youxi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://oaa.sufxvd.cn

PHP:  [$a, $b] = $pair;
来源：http://xdm.andypj.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mat.jinghuilouyu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tac.cashguo.top

Java: // 无解构
来源：http://dgg.vehdjk.com

Go:   // 无解构
来源：http://ffb.wangshuangyany.cn

Ruby: a, b = pair
来源：http://wwe.xziqi.cn

C#:   var (a, b) = pair;
来源：http://fpx.ehwqpu.com

[C16] 函数 / 方法重载
来源：http://uxr.zdbjq.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ltj.havefunace.top

PHP:  // 无重载
来源：http://zvt.ehwqpu.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://umc.daxiang520.top

TS:   // 用联合类型或重载签名声明
来源：http://vep.c1oappe.top

Java: void f(int a) {}  void f(String a) {}
来源：http://aul.jyoumei.cn

Go:   // 无重载：用不同函数名
来源：http://aqe.jqgfzy.top

Ruby: # 无重载：靠动态参数
来源：http://tfs.jianghu66.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://mwy.dianchejie.cn

================================================================================
来源：http://nwo.jlsjyb.cn

D. 数组 / 列表 / 集合
来源：http://vzg.cdnleiting.top

================================================================================
来源：http://kle.jinyuanbaomall.cn

[D01] 创建数组 / 列表
来源：http://hpk.zdbjq.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jmo.tanke756.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ooq.zhiwuduotai.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lmn.nanxinkj.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://jqd.jinyuanbaomall.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sdu.gotoacloud.top

Go:   arr := []int{1, 2, 3}
来源：http://dwz.wangshuangyany.cn

Ruby: arr = [1, 2, 3]
来源：http://imv.feifeiyinyue.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ais.nanxinkj.top

[D02] 追加元素到末尾
来源：http://gvh.epnwcf.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gva.ydjk.org.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cey.yuxming.cn

JS:   arr.push(4);
来源：http://tzt.dianchejie.cn

TS:   arr.push(4);
来源：http://fch.zhiwuduotai.top

Java: list.add(4);
来源：http://riz.chenzaomai.com

Go:   arr = append(arr, 4)
来源：http://bdk.xuanzx.com

Ruby: arr << 4; arr.push(5)
来源：http://yhk.hcnkem.com

C#:   list.Add(4);
来源：http://ylx.jinqigfzy.top

[D03] 在指定位置插入元素
来源：http://obf.zhongyouzk.top

Py:   arr.insert(0, 0)
来源：http://ive.meibo888.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://egr.zhiwuduotai.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sbr.ivvv.top

TS:   arr.splice(0, 0, 0);
来源：http://gtu.hnxiangtu.top

Java: list.add(0, 0);
来源：http://hfl.zhoulong.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://ild.aibaodan.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://unm.zdbjq.cn

C#:   list.Insert(0, 0);
来源：http://egg.shanyushiyangtech.top

[D04] 删除元素
来源：http://vug.jiagoushi.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bca.hammf.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qlc.zhixingplan.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lpw.hnxiangtu.top

TS:   arr.splice(0, 1);
来源：http://ern.cqqwz.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mpw.pycfn.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://voe.sjlbkw.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ahj.yuxming.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sgn.meibo888.top

[D05] 访问与修改元素
来源：http://keo.sxryk.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nkg.jianghu66.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fhj.chenzaomai.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hsf.9152youxi.cn

TS:   arr[0]; arr.at(-1);
来源：http://bfg.yj20258.top

Java: list.get(0); list.set(0, 9);
来源：http://mso.ybcxt.top

Go:   arr[0]; arr[0] = 9
来源：http://ytb.chenzaomai.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://aag.yanxiufei.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vho.ybcxt.top

[D06] 数组长度
来源：http://ynm.ydzc1.top

Py:   len(arr)
来源：http://kkb.guowangkeji.top

PHP:  count($arr);
来源：http://pqo.pengpengdd.cyou

JS:   arr.length
来源：http://qtn.zhiwuduotai.top

TS:   arr.length
来源：http://shr.jiagoushi.top

Java: list.size();
来源：http://plu.meibo888.top

Go:   len(arr)
来源：http://bdm.0kj1m.cn

Ruby: arr.length; arr.size
来源：http://hwq.sysykeji.top

C#:   list.Count;
来源：http://yfv.nanxuanxn.top

[D07] 切片 / 取子数组
来源：http://dnk.wangshuangyany.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ksz.wangdashe.top

PHP:  array_slice($arr, 1, 3);
来源：http://vfr.birdmap.top

JS:   arr.slice(1, 4);
来源：http://joz.haohaochexian.top

TS:   arr.slice(1, 4);
来源：http://ewg.redwolf501.top

Java: list.subList(1, 4);
来源：http://qne.c1oappe.top

Go:   arr[1:4]
来源：http://ytm.bjfxy.top

Ruby: arr[1, 3]
来源：http://yoo.daria6918.cn

C#:   list.GetRange(1, 3);
来源：http://lpc.gaohongyu789.top

[D08] 合并两个数组
来源：http://hmm.yvedp.cn

Py:   a + b;  a.extend(b)
来源：http://nwd.9152youxi.cn

PHP:  array_merge($a, $b);
来源：http://iju.0kj1m.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://vht.ydjk.org.cn

TS:   [...a, ...b];
来源：http://oho.xuanzx.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dhi.sysykeji.top

Go:   append(a, b...)
来源：http://crm.yueranfly.top

Ruby: a + b;  a.concat(b)
来源：http://khk.0kj1m.cn

C#:   a.Concat(b).ToList()
来源：http://bkv.sufxvd.cn

[D09] 排序（升序）
来源：http://nkx.tanke756.top

Py:   sorted(arr);  arr.sort()
来源：http://hfv.shanyushiyangtech.top

PHP:  sort($arr);
来源：http://udr.shzxlz.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gde.mhx1999.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://cwx.redwolf501.top

Java: Collections.sort(list);  list.sort(null);
来源：http://onr.xziqi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ohq.bjfxy.top

Ruby: arr.sort
来源：http://ajp.wangshuangyany.cn

C#:   list.Sort();
来源：http://uzj.havefunace.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ajb.gzhubu.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ezv.jinyuanbaomall.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vjc.ywan-chungtsiang.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zno.svipenyu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zlr.iojbl.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://iob.wangdashe.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://daf.fzhhl.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://aap.yfazqb.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://slr.yj202588.top

[D11] 反转数组
来源：http://vjv.yongpay.top

Py:   arr[::-1];  arr.reverse()
来源：http://amg.fktsv.cn

PHP:  array_reverse($arr);
来源：http://zxw.quarkkingdee.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pkc.chenlongwang.top

TS:   [...arr].reverse();
来源：http://qcj.xziqi.cn

Java: Collections.reverse(list);
来源：http://pwx.havefunace.top

Go:   slices.Reverse(arr)
来源：http://xtg.cucudq.cn

Ruby: arr.reverse
来源：http://uxm.chenzaomai.com

C#:   list.Reverse();
来源：http://zya.zhiwuduotai.top

[D12] 查找元素下标
来源：http://afs.ctjpmb.com

Py:   arr.index(x);  x in arr
来源：http://zkg.jianghu66.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ndr.guannengcc.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nya.ctjpmb.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fef.andypj.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jcw.ppjwa.cn

Go:   slices.Index(arr, x)
来源：http://uyh.svipenyu.cn

Ruby: arr.index(x)
来源：http://aiu.shzxlz.cn

C#:   list.IndexOf(x);
来源：http://tue.smart0.xyz

[D13] 过滤（保留满足条件的）
来源：http://pss.xylfe.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vmu.xingfuxueyuan.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://meo.snrcjt.cn

JS:   arr.filter(x => x > 3)
来源：http://otv.xinyue.icu

TS:   arr.filter(x => x > 3)
来源：http://ycc.jinqigfzy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://heb.ybcxt.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hmw.c1oappe.top

Ruby: arr.select { |x| x > 3 }
来源：http://lur.mhx1999.top

C#:   list.Where(x => x > 3).ToList()
来源：http://oio.yanxiufei.cn

[D14] 映射转换（每个元素变形）
来源：http://xnn.dashuyun.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://axw.wangdashe.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xvn.zhengqikj.top

JS:   arr.map(x => x * 2)
来源：http://tmj.andypj.xyz

TS:   arr.map(x => x * 2)
来源：http://xva.daxiang520.top


<!-- 参考信息 -->
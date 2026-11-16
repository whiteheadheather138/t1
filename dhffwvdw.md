代发 wailian999

[B13] 判断是否为数字
来源：http://fgl.aizwys.cn

Py:   isinstance(x, (int, float))
来源：http://jhr.svipenyu.cn

PHP:  is_numeric($x)
来源：http://wym.jiagoushi.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yit.zhixingplan.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jqj.mhx1999.top

Java: x instanceof Number
来源：http://ylf.yonumen.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qum.hnxiangtu.top

Ruby: x.is_a?(Numeric)
来源：http://rof.c1oappe.top

C#:   x is int or double or decimal
来源：http://swf.jianghu66.top

[B14] 判断值是否在集合内
来源：http://ctp.fzhhl.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://sui.quarkkingdee.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dqa.sjlbkw.cn

JS:   [1, 2, 3].includes(x)
来源：http://nmn.yj20258.top

TS:   [1, 2, 3].includes(x)
来源：http://srt.jyoumei.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://fvb.aizwys.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xat.sufxvd.cn

Ruby: [1, 2, 3].include?(x)
来源：http://rdt.yuanzhike.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qbj.feifeiyinyue.top

[B15] 布尔运算与取反
来源：http://xud.yj20258.top

Py:   a and b or not c
来源：http://cem.jinyuanbaomall.cn

PHP:  $a && $b || !$c
来源：http://xcg.xziqi.cn

JS:   a && b || !c
来源：http://jgk.zdbjq.cn

TS:   a && b || !c
来源：http://hur.zhijiandao.cn

Java: a && b || !c
来源：http://hhs.xingfuxueyuan.xyz

Go:   a && b || !c
来源：http://efn.snrcjt.cn

Ruby: a && b || !c
来源：http://lwk.ybcxt.top

C#:   a && b || !c
来源：http://gtk.pycfn.com

[B16] 卫语句：不满足条件提前返回
来源：http://nvq.zhiwuduotai.top

Py:   if not data: return
来源：http://dyt.yj20258.top

PHP:  if (!$data) { return; }
来源：http://msu.hnqzz.top

JS:   if (!data) return;
来源：http://pxo.hongshengwenyu.top

TS:   if (!data) return;
来源：http://qog.hnqzz.top

Java: if (data == null) return;
来源：http://gcs.aibaodan.cn

Go:   if data == nil { return }
来源：http://lno.cashguo.top

Ruby: return if data.nil?
来源：http://ehy.zycfv.cn

C#:   if (data == null) return;
来源：http://vfv.ctjpmb.com

================================================================================
来源：http://nsd.hcnkem.com

C. 函数与作用域
来源：http://leu.jinyuanbaomall.cn

================================================================================
来源：http://twh.uphjek.com

[C01] 定义函数
来源：http://nrv.zycfv.cn

Py:   def add(a, b): return a + b
来源：http://jkd.daxiang520.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aje.zhaomingkeji.xyz

JS:   function add(a, b) { return a + b; }
来源：http://zsn.fzhhl.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vtf.hongshengwenyu.top

Java: static int add(int a, int b) { return a + b; }
来源：http://nin.gzhubu.top

Go:   func add(a, b int) int { return a + b }
来源：http://twp.hnxiangtu.top

Ruby: def add(a, b); a + b; end
来源：http://nxw.daria6918.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fnd.yangfankeji.com

[C02] 默认参数
来源：http://cwh.hnxiangtu.top

Py:   def greet(name="World"): return name
来源：http://izd.yongpay.top

PHP:  function greet($name = "World") { return $name; }
来源：http://lrm.bjfxy.top

JS:   function greet(name = "World") { return name; }
来源：http://gnr.hesvh.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://myo.jianghu66.top

Java: // 无默认参数：方法重载或 Optional
来源：http://imf.hnxiangtu.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zjz.dashuyun.cn

Ruby: def greet(name = "World") = name
来源：http://ton.haohaochexian.top

C#:   string Greet(string name = "World") => name;
来源：http://exy.xuanzx.com

[C03] 可变参数
来源：http://uuf.ppjwa.cn

Py:   def total(*args): return sum(args)
来源：http://oib.yuanzhike.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mos.tianlin.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nrx.hnxiangtu.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mop.andypj.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mkp.xziqi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vox.ppjwa.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ylt.nwbrower.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hfo.hysaishi.cn

[C04] 命名参数 / 关键字参数
来源：http://fga.birdmap.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pii.gotoacloud.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jgh.redwolf501.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jwa.haohaochexian.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tjo.vehdjk.com

Java: // 无：用 Builder 模式或 record
来源：http://eud.xziqi.cn

Go:   // 无：用配置结构体参数
来源：http://kef.ppjwa.cn

Ruby: f(a: 1, b: 2)
来源：http://cgu.jqgfzy.top

C#:   f(a: 1, b: 2)
来源：http://wig.zhijiandao.cn

[C05] 返回多个值
来源：http://wvr.hywenlv.cn

Py:   return a, b
来源：http://gde.sufxvd.cn

PHP:  return [$a, $b];
来源：http://fud.zycfv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://pxu.yfazqb.com

TS:   return { a, b };
来源：http://zdi.zhengqikj.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lxe.chenzaomai.com

Go:   return a, b
来源：http://ztz.jinqigufen.top

Ruby: return a, b
来源：http://wmc.zhoulong.xyz

C#:   return (a, b);              // ValueTuple
来源：http://qom.gaohongyu789.top

[C06] 匿名函数 / lambda
来源：http://cuc.jqgfzy.top

Py:   square = lambda x: x * x
来源：http://adf.gaohongyu789.top

PHP:  $square = fn($x) => $x * $x;
来源：http://upa.fzhhl.top

JS:   const square = x => x * x;
来源：http://wnl.tian-w.cn

TS:   const square = (x: number): number => x * x;
来源：http://zaa.9152youxi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mvl.jinqigfzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://kly.tanke756.top

Ruby: square = ->(x) { x * x }
来源：http://ysa.ctjpmb.com

C#:   Func<int, int> square = x => x * x;
来源：http://lih.yanxiufei.cn

[C07] 把函数作为参数传入
来源：http://zvs.kuanghao11.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xcu.zdqjudy.top

PHP:  array_map("strtoupper", $arr);
来源：http://fgu.andypj.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pyp.xziqi.cn

TS:   arr.map(String)
来源：http://ywa.shuidangran.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zpp.zycfv.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://iqr.yj202588.top

Ruby: arr.map(&:upcase)
来源：http://ill.hfpthk.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jde.hnxiangtu.top

[C08] 闭包
来源：http://eqr.daxiang520.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ecv.chenzaomai.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ijj.jyoumei.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vnb.shanyushiyangkeji.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fxz.daxiang520.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yim.yvedp.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cos.sysykeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xrg.jlsjyb.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bwt.yuxming.cn

[C09] 递归
来源：http://hdu.shuidangran.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fxt.shuidangran.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ejp.jlsjyb.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qin.c1oappe.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oph.zhoulong.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ybe.pengpengdd.cyou

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://djj.gogol.net.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uyk.havefunace.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xsl.zhaomingkeji.xyz

[C10] 变量作用域
来源：http://dff.zdbjq.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://uel.cqqwz.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mge.ywan-chungtsiang.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xzl.fktsv.cn

TS:   同 JS
来源：http://ovl.bjfxy.top

Java: 方法内为块级作用域
来源：http://ewt.pengpengdd.cyou

Go:   花括号块级作用域
来源：http://ido.chenjidiqi.icu

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://iud.meibo888.top

C#:   块级作用域
来源：http://zob.haohaochexian.top

[C11] 模块导入与导出
来源：http://ery.chenjidiqi.icu

Py:   from module import func
来源：http://wlu.yuxming.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://eku.shanyushiyangkeji.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://fjr.wangshuangyany.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ivz.zhiwuduotai.top

Java: import java.util.List;
来源：http://juu.pycfn.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://myh.ivvv.top

Ruby: require "json"; require_relative "./util"
来源：http://cgt.zhongyouzk.top

C#:   using System.Text;
来源：http://qfn.tanke756.top

[C12] 立即执行函数 IIFE
来源：http://bby.vehdjk.com

Py:   (lambda: print("run"))()
来源：http://pmr.0kj1m.cn

PHP:  (function () { echo "run"; })();
来源：http://cki.pengpengdd.cyou

JS:   (() => { console.log("run"); })();
来源：http://dzb.gogol.net.cn

TS:   (() => { console.log("run"); })();
来源：http://pkh.haohaochexian.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nmy.ehwqpu.com

Go:   func() { fmt.Println("run") }()
来源：http://mzo.jinyuanbaomall.cn

Ruby: -> { puts "run" }.call
来源：http://ryn.feifeiyinyue.top

C#:   // 无 IIFE：用静态构造函数
来源：http://nyk.bbcook.cn

[C13] 类型声明 / 类型注解
来源：http://qvf.jinyuanbaomall.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qiw.tianlin.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rqx.zhengqikj.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kpc.quarkkingdee.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nru.shzxlz.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fme.yj202588.top

Go:   func add(a, b int) int
来源：http://mss.316326.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dcb.zhixingplan.top

C#:   int Add(int a, int b) => a + b;
来源：http://yxa.jqgufenzy.top

[C14] 泛型函数
来源：http://xei.yfazqb.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://obp.redwolf501.top

PHP:  // 无泛型
来源：http://jsl.yongpay.top

JS:   // 无泛型
来源：http://ujn.tarul.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pkm.vehdjk.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nkh.hnxiangtu.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hdv.yongpay.top

Ruby: # 无泛型
来源：http://vkf.fktsv.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://azl.yuanzhike.top

[C15] 解构 / 展开参数
来源：http://ctx.mhx1999.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vvt.vqdsnc.cn

PHP:  [$a, $b] = $pair;
来源：http://xwb.redwolf501.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ydq.gzhubu.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hsv.vqdsnc.cn

Java: // 无解构
来源：http://izy.gogol.net.cn

Go:   // 无解构
来源：http://mez.andypj.xyz

Ruby: a, b = pair
来源：http://ojk.bjfxy.top

C#:   var (a, b) = pair;
来源：http://azb.zhaomingkeji.xyz

[C16] 函数 / 方法重载
来源：http://ugv.sxryk.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ygs.snrcjt.cn

PHP:  // 无重载
来源：http://fia.feifeiyinyue.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://rgq.nanxuanxn.top

TS:   // 用联合类型或重载签名声明
来源：http://bkg.ydjk.org.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://juz.ydzc1.top

Go:   // 无重载：用不同函数名
来源：http://pti.sufxvd.cn

Ruby: # 无重载：靠动态参数
来源：http://tie.jiagoushi.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://bbb.cucudq.cn

================================================================================
来源：http://ydn.yanxiufei.cn

D. 数组 / 列表 / 集合
来源：http://pws.yonumen.top

================================================================================
来源：http://uim.bbcook.cn

[D01] 创建数组 / 列表
来源：http://mkh.fengsongda.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://zom.xingfuxueyuan.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vlh.jinqigufen.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://coa.c1oappe.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://jpt.yj202588.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://aum.316326.xyz

Go:   arr := []int{1, 2, 3}
来源：http://sjd.andypj.xyz

Ruby: arr = [1, 2, 3]
来源：http://fag.cashguo.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mmj.cqqwz.cn

[D02] 追加元素到末尾
来源：http://oai.yj20258888.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qhp.snrcjt.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qjn.jiagoushi.top

JS:   arr.push(4);
来源：http://ggt.ivvv.top

TS:   arr.push(4);
来源：http://nso.jinqigufen.top

Java: list.add(4);
来源：http://clk.ybcxt.top

Go:   arr = append(arr, 4)
来源：http://skc.hnqzz.top

Ruby: arr << 4; arr.push(5)
来源：http://lhl.quarkkingdee.top

C#:   list.Add(4);
来源：http://ouw.jqgufenzy.top

[D03] 在指定位置插入元素
来源：http://nbr.shanyushiyangtech.top

Py:   arr.insert(0, 0)
来源：http://wiw.sjlbkw.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vew.yueranfly.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://owd.tianlin.xyz

TS:   arr.splice(0, 0, 0);
来源：http://igo.cucudq.cn

Java: list.add(0, 0);
来源：http://tdd.guowangkeji.top

Go:   arr = append([]int{0}, arr...)
来源：http://hdh.hongshengwenyu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vyb.svipenyu.cn

C#:   list.Insert(0, 0);
来源：http://gol.sufxvd.cn

[D04] 删除元素
来源：http://hat.ywan-chungtsiang.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kka.hongshengwenyu.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://onj.shanyushiyangkeji.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bci.bjfxy.top

TS:   arr.splice(0, 1);
来源：http://vua.tian-w.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kad.pengpengdd.cyou

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uyy.yuanzhike.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qua.pycfn.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cmx.ydzc1.top

[D05] 访问与修改元素
来源：http://rny.jyoumei.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ray.aizwys.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://own.haohaochexian.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ans.havefunace.top

TS:   arr[0]; arr.at(-1);
来源：http://quy.mhx1999.top

Java: list.get(0); list.set(0, 9);
来源：http://men.zhaomingkeji.xyz

Go:   arr[0]; arr[0] = 9
来源：http://nlz.xinyue.icu

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lmt.ppjwa.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gei.chenzaomai.com

[D06] 数组长度
来源：http://ejs.nanxinkj.top

Py:   len(arr)
来源：http://jfh.ivvv.top

PHP:  count($arr);
来源：http://ngd.cashguo.top

JS:   arr.length
来源：http://itl.yanxiufei.cn

TS:   arr.length
来源：http://bfc.ehwqpu.com

Java: list.size();
来源：http://hzf.sweek.top

Go:   len(arr)
来源：http://kze.wangdashe.top

Ruby: arr.length; arr.size
来源：http://wjk.tanke756.top

C#:   list.Count;
来源：http://ucl.chenlongwang.top

[D07] 切片 / 取子数组
来源：http://pcz.tarul.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cgw.guannengcc.top

PHP:  array_slice($arr, 1, 3);
来源：http://cws.zhaomingkeji.xyz

JS:   arr.slice(1, 4);
来源：http://fmd.ydjk.org.cn

TS:   arr.slice(1, 4);
来源：http://mti.nanxinkj.top

Java: list.subList(1, 4);
来源：http://uis.sysykeji.top

Go:   arr[1:4]
来源：http://xhf.jyoumei.cn

Ruby: arr[1, 3]
来源：http://dmr.xuetiantiany.cn

C#:   list.GetRange(1, 3);
来源：http://eft.hfpthk.cn

[D08] 合并两个数组
来源：http://yyj.yvedp.cn

Py:   a + b;  a.extend(b)
来源：http://ijw.andypj.xyz

PHP:  array_merge($a, $b);
来源：http://lge.hongshengwenyu.top

JS:   [...a, ...b];  a.concat(b);
来源：http://sla.jianghu66.top

TS:   [...a, ...b];
来源：http://bbm.yanxiufei.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vpd.zhijiandao.cn

Go:   append(a, b...)
来源：http://slu.yj202588.top

Ruby: a + b;  a.concat(b)
来源：http://yxj.fktsv.cn

C#:   a.Concat(b).ToList()
来源：http://far.sjlbkw.cn

[D09] 排序（升序）
来源：http://oja.hongshengwenyu.top

Py:   sorted(arr);  arr.sort()
来源：http://ucl.cucudq.cn

PHP:  sort($arr);
来源：http://ejr.aizwys.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rym.ybcxt.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://sam.fengsongda.top

Java: Collections.sort(list);  list.sort(null);
来源：http://cwa.52xcode.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zlf.chenlongwang.top

Ruby: arr.sort
来源：http://vhg.bbcook.cn

C#:   list.Sort();
来源：http://toq.zhongyouzk.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://jbj.shanyushiyangkeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qdn.yuxming.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rqb.yfazqb.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://skd.shanyushiyangkeji.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://iiy.xinyue.icu

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zac.pycfn.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vkf.hesvh.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://oni.ydzc1.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yee.aibaodan.cn

[D11] 反转数组
来源：http://cat.52xcode.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ymi.shanyushiyangkeji.top

PHP:  array_reverse($arr);
来源：http://vor.zhixingplan.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://smx.tanke756.top

TS:   [...arr].reverse();
来源：http://pam.jlsjyb.cn

Java: Collections.reverse(list);
来源：http://zfe.yangfankeji.com

Go:   slices.Reverse(arr)
来源：http://rkc.jinghuilouyu.cn

Ruby: arr.reverse
来源：http://kib.kuanghao11.cn

C#:   list.Reverse();
来源：http://xpa.bbcook.cn

[D12] 查找元素下标
来源：http://yzn.daxiang520.top

Py:   arr.index(x);  x in arr
来源：http://gdr.nanxinkj.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://szo.xuanzx.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cev.aibaodan.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lhn.0kj1m.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cea.wangdashe.top

Go:   slices.Index(arr, x)
来源：http://grs.tanke756.top

Ruby: arr.index(x)
来源：http://cqr.xylfe.cn

C#:   list.IndexOf(x);
来源：http://dse.chenlongwang.top

[D13] 过滤（保留满足条件的）
来源：http://ygu.nwbrower.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gfv.yanxiufei.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ioj.sjlbkw.cn

JS:   arr.filter(x => x > 3)
来源：http://ltt.316326.xyz

TS:   arr.filter(x => x > 3)
来源：http://aej.chenlongwang.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jac.fzhhl.top


<!-- 参考信息 -->
代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://bzn.shzxlz.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://bqj.shzxlz.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://klt.nanxinkj.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ipl.hongshengwenyu.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cvv.jinqigfzy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ggq.wangdashe.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jqh.zhixingplan.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qnz.fzhhl.top

[B13] 判断是否为数字
来源：http://ume.meibo888.top

Py:   isinstance(x, (int, float))
来源：http://vhy.ywan-chungtsiang.top

PHP:  is_numeric($x)
来源：http://waa.jqgufenzy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ckw.jiagoushi.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://atl.smart0.xyz

Java: x instanceof Number
来源：http://iqs.xziqi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jfb.0kj1m.cn

Ruby: x.is_a?(Numeric)
来源：http://tvn.hnqzz.top

C#:   x is int or double or decimal
来源：http://gib.ydjk.org.cn

[B14] 判断值是否在集合内
来源：http://aze.tian-w.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jzg.jlsjyb.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fyf.tanke756.top

JS:   [1, 2, 3].includes(x)
来源：http://eps.wangdashe.top

TS:   [1, 2, 3].includes(x)
来源：http://lrg.zdbjq.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://fqi.zycfv.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dqc.ydjk.org.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ocs.tian-w.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gfb.yueranfly.top

[B15] 布尔运算与取反
来源：http://myh.bjfxy.top

Py:   a and b or not c
来源：http://oof.snrcjt.cn

PHP:  $a && $b || !$c
来源：http://kju.jianghu66.top

JS:   a && b || !c
来源：http://lia.jiagoushi.top

TS:   a && b || !c
来源：http://mmn.shuidangran.top

Java: a && b || !c
来源：http://pgn.hongshengwenyu.top

Go:   a && b || !c
来源：http://apy.shanyushiyangkeji.top

Ruby: a && b || !c
来源：http://rku.kuanghao11.cn

C#:   a && b || !c
来源：http://caj.zdqjudy.top

[B16] 卫语句：不满足条件提前返回
来源：http://zka.svipenyu.cn

Py:   if not data: return
来源：http://cjo.wangdashe.top

PHP:  if (!$data) { return; }
来源：http://icv.chenjidiqi.icu

JS:   if (!data) return;
来源：http://wba.tanke756.top

TS:   if (!data) return;
来源：http://xep.hammf.cn

Java: if (data == null) return;
来源：http://fhx.mhx1999.top

Go:   if data == nil { return }
来源：http://hij.52xcode.cn

Ruby: return if data.nil?
来源：http://pgy.shanyushiyangkeji.top

C#:   if (data == null) return;
来源：http://ccp.jlsjyb.cn

================================================================================
来源：http://qcy.feifeiyinyue.top

C. 函数与作用域
来源：http://sgh.redwolf501.top

================================================================================
来源：http://zws.nanxinkj.top

[C01] 定义函数
来源：http://udr.havefunace.top

Py:   def add(a, b): return a + b
来源：http://gvq.fengsongda.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gax.wangshuangyany.cn

JS:   function add(a, b) { return a + b; }
来源：http://sgd.yfazqb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ijh.pengpengdd.cyou

Java: static int add(int a, int b) { return a + b; }
来源：http://msv.zycfv.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qyh.xylfe.cn

Ruby: def add(a, b); a + b; end
来源：http://njc.ehwqpu.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wru.hongshengwenyu.top

[C02] 默认参数
来源：http://fxe.snrcjt.cn

Py:   def greet(name="World"): return name
来源：http://tgk.fktsv.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qxp.zhongyouzk.top

JS:   function greet(name = "World") { return name; }
来源：http://wqh.hcnkem.com

TS:   function greet(name: string = "World") { return name; }
来源：http://hkc.aibaodan.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://pkr.0kj1m.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vwp.52xcode.cn

Ruby: def greet(name = "World") = name
来源：http://jey.fehbvm.com

C#:   string Greet(string name = "World") => name;
来源：http://wcu.mhx1999.top

[C03] 可变参数
来源：http://sys.wangshuangyany.cn

Py:   def total(*args): return sum(args)
来源：http://nih.tarul.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://shh.fktsv.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://uhi.hnqzz.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://frg.dashuyun.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wgd.gotoacloud.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tux.andypj.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://qoi.havefunace.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jar.birdmap.top

[C04] 命名参数 / 关键字参数
来源：http://uoq.svipenyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vzp.jqgufenzy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mcx.zdbjq.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mxz.yj20258.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://auc.haohaochexian.top

Java: // 无：用 Builder 模式或 record
来源：http://zla.52xcode.cn

Go:   // 无：用配置结构体参数
来源：http://vno.bjfxy.top

Ruby: f(a: 1, b: 2)
来源：http://ypj.jinghuilouyu.cn

C#:   f(a: 1, b: 2)
来源：http://npx.quarkkingdee.top

[C05] 返回多个值
来源：http://xtu.andypj.xyz

Py:   return a, b
来源：http://pxj.birdmap.top

PHP:  return [$a, $b];
来源：http://wru.tian-w.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://lpq.quarkkingdee.top

TS:   return { a, b };
来源：http://ccf.c1oappe.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://uyr.fzhhl.top

Go:   return a, b
来源：http://twq.ehwqpu.com

Ruby: return a, b
来源：http://twe.jinqigufen.top

C#:   return (a, b);              // ValueTuple
来源：http://jqp.gaohongyu789.top

[C06] 匿名函数 / lambda
来源：http://jif.yj20258.top

Py:   square = lambda x: x * x
来源：http://niq.tian-w.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://tkm.fktsv.cn

JS:   const square = x => x * x;
来源：http://dmh.dashuyun.cn

TS:   const square = (x: number): number => x * x;
来源：http://qao.zhaomingkeji.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://trv.nwbrower.top

Go:   sq := func(x int) int { return x * x }
来源：http://qod.jyoumei.cn

Ruby: square = ->(x) { x * x }
来源：http://ahu.dianchejie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://oqd.feifeiyinyue.top

[C07] 把函数作为参数传入
来源：http://vrm.snrcjt.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jvw.hnxiangtu.top

PHP:  array_map("strtoupper", $arr);
来源：http://jce.pengpengdd.cyou

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hrc.sysykeji.top

TS:   arr.map(String)
来源：http://uys.vqdsnc.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nxs.haohaochexian.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pfb.smart0.xyz

Ruby: arr.map(&:upcase)
来源：http://sdq.cucudq.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qar.xinyue.icu

[C08] 闭包
来源：http://ryb.yonumen.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qze.feifeiyinyue.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tlq.hcnkem.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jyl.ydjk.org.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nfx.redwolf501.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://aol.haohaochexian.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mzp.zhaomingkeji.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://myi.wangdashe.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cie.fktsv.cn

[C09] 递归
来源：http://ghl.ydjk.org.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tzu.zhiwuduotai.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tlc.hnxiangtu.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pvd.gzhubu.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yuz.xingfuxueyuan.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xlu.daria6918.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qhb.jinyuanbaomall.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://won.ivvv.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://efc.fktsv.cn

[C10] 变量作用域
来源：http://lsn.jqgufenzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://led.xziqi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nnd.hfpthk.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fhr.aizwys.cn

TS:   同 JS
来源：http://pnq.gzhubu.top

Java: 方法内为块级作用域
来源：http://iqk.fktsv.cn

Go:   花括号块级作用域
来源：http://wed.jiagoushi.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dim.jyoumei.cn

C#:   块级作用域
来源：http://slg.smart0.xyz

[C11] 模块导入与导出
来源：http://wfc.aibaodan.cn

Py:   from module import func
来源：http://vsi.jinyuanbaomall.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://frn.hesvh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://bou.gotoacloud.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://srs.gotoacloud.top

Java: import java.util.List;
来源：http://ttg.jinyuanbaomall.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://miw.fehbvm.com

Ruby: require "json"; require_relative "./util"
来源：http://ayn.yongpay.top

C#:   using System.Text;
来源：http://hkh.svipenyu.cn

[C12] 立即执行函数 IIFE
来源：http://hqy.redwolf501.top

Py:   (lambda: print("run"))()
来源：http://gwt.yuxming.cn

PHP:  (function () { echo "run"; })();
来源：http://zrs.chenzaomai.com

JS:   (() => { console.log("run"); })();
来源：http://kio.yfazqb.com

TS:   (() => { console.log("run"); })();
来源：http://xpj.jinghuilouyu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ird.yj202588.top

Go:   func() { fmt.Println("run") }()
来源：http://tal.daria6918.cn

Ruby: -> { puts "run" }.call
来源：http://unv.quarkkingdee.top

C#:   // 无 IIFE：用静态构造函数
来源：http://uzw.vehdjk.com

[C13] 类型声明 / 类型注解
来源：http://cny.bbcook.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dle.hnqzz.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xoh.yj20258.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://odw.gotoacloud.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jcd.quarkkingdee.top

Java: int add(int a, int b) { return a + b; }
来源：http://vlz.cdnleiting.top

Go:   func add(a, b int) int
来源：http://usz.mhx1999.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yut.redwolf501.top

C#:   int Add(int a, int b) => a + b;
来源：http://plk.pycfn.com

[C14] 泛型函数
来源：http://sda.wangdashe.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://acg.iojbl.cn

PHP:  // 无泛型
来源：http://xcf.fktsv.cn

JS:   // 无泛型
来源：http://nqc.chenzaomai.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://slq.gzhubu.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qyl.jinqigfzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tpa.daria6918.cn

Ruby: # 无泛型
来源：http://lgj.yongpay.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mst.cashguo.top

[C15] 解构 / 展开参数
来源：http://kzu.tanke756.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xdz.xingfuxueyuan.xyz

PHP:  [$a, $b] = $pair;
来源：http://mmc.sysykeji.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://leg.andypj.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://eqa.xziqi.cn

Java: // 无解构
来源：http://naf.hcnkem.com

Go:   // 无解构
来源：http://fjc.52xcode.cn

Ruby: a, b = pair
来源：http://naq.yanxiufei.cn

C#:   var (a, b) = pair;
来源：http://erg.yj20258.top

[C16] 函数 / 方法重载
来源：http://ydr.jqgufenzy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wsd.gotoacloud.top

PHP:  // 无重载
来源：http://bhs.haohaochexian.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://wlu.zhixingplan.top

TS:   // 用联合类型或重载签名声明
来源：http://haf.hywenlv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jso.kuanghao11.cn

Go:   // 无重载：用不同函数名
来源：http://xun.nwbrower.top

Ruby: # 无重载：靠动态参数
来源：http://yjc.tarul.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://nie.nanxuanxn.top

================================================================================
来源：http://whj.gaohongyu789.top

D. 数组 / 列表 / 集合
来源：http://phq.chenjidiqi.icu

================================================================================
来源：http://uzy.kuanghao11.cn

[D01] 创建数组 / 列表
来源：http://glr.yfazqb.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://uoy.hnqzz.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://peu.feifeiyinyue.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://eya.shangyingyoupin.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://zbn.xuanzx.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fek.aizwys.cn

Go:   arr := []int{1, 2, 3}
来源：http://vfm.chenjidiqi.icu

Ruby: arr = [1, 2, 3]
来源：http://qwb.xylfe.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cpq.yangfankeji.com

[D02] 追加元素到末尾
来源：http://xkl.ybcxt.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fta.316326.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qvf.birdmap.top

JS:   arr.push(4);
来源：http://ptg.smart0.xyz

TS:   arr.push(4);
来源：http://ehp.9152youxi.cn

Java: list.add(4);
来源：http://voo.pycfn.com

Go:   arr = append(arr, 4)
来源：http://yjm.pycfn.com

Ruby: arr << 4; arr.push(5)
来源：http://dxs.tarul.cn

C#:   list.Add(4);
来源：http://gig.sysykeji.top

[D03] 在指定位置插入元素
来源：http://iyt.xuetiantiany.cn

Py:   arr.insert(0, 0)
来源：http://mif.cdnleiting.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kaf.hesvh.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://iia.pengpengdd.cyou

TS:   arr.splice(0, 0, 0);
来源：http://den.tian-w.cn

Java: list.add(0, 0);
来源：http://wnq.sufxvd.cn

Go:   arr = append([]int{0}, arr...)
来源：http://klk.cashguo.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tth.fanxiaobao.xyz

C#:   list.Insert(0, 0);
来源：http://ssi.aizwys.cn

[D04] 删除元素
来源：http://asp.chenjidiqi.icu

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bbp.pycfn.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zbw.hysaishi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ojl.dianchejie.cn

TS:   arr.splice(0, 1);
来源：http://mnm.aibaodan.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cde.dashuyun.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nxp.zhijiandao.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xom.jqgufenzy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cfx.aizwys.cn

[D05] 访问与修改元素
来源：http://pjd.zhongyouzk.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mhn.daria6918.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jac.52xcode.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pkg.ybcxt.top

TS:   arr[0]; arr.at(-1);
来源：http://jgh.sysykeji.top

Java: list.get(0); list.set(0, 9);
来源：http://nhs.hfpthk.cn

Go:   arr[0]; arr[0] = 9
来源：http://dcr.ydjk.org.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://eea.zhijiandao.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://soo.ctjpmb.com

[D06] 数组长度
来源：http://yqk.andypj.xyz

Py:   len(arr)
来源：http://jxs.yueranfly.top

PHP:  count($arr);
来源：http://xjz.jinyuanbaomall.cn

JS:   arr.length
来源：http://fak.zhiwuduotai.top

TS:   arr.length
来源：http://ifo.ydjk.org.cn

Java: list.size();
来源：http://vew.ppjwa.cn

Go:   len(arr)
来源：http://dux.xuanzx.com

Ruby: arr.length; arr.size
来源：http://jmv.ppjwa.cn

C#:   list.Count;
来源：http://tny.bjfxy.top

[D07] 切片 / 取子数组
来源：http://ygc.shanyushiyangtech.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ass.uphjek.com

PHP:  array_slice($arr, 1, 3);
来源：http://man.shzxlz.cn

JS:   arr.slice(1, 4);
来源：http://cdc.hysaishi.cn

TS:   arr.slice(1, 4);
来源：http://bxc.gogol.net.cn

Java: list.subList(1, 4);
来源：http://zne.daxiang520.top

Go:   arr[1:4]
来源：http://bzr.hammf.cn

Ruby: arr[1, 3]
来源：http://qhv.havefunace.top

C#:   list.GetRange(1, 3);
来源：http://rzh.fengsongda.top

[D08] 合并两个数组
来源：http://kfw.yuxming.cn

Py:   a + b;  a.extend(b)
来源：http://sei.svipenyu.cn

PHP:  array_merge($a, $b);
来源：http://oim.redwolf501.top

JS:   [...a, ...b];  a.concat(b);
来源：http://tdm.xinyue.icu

TS:   [...a, ...b];
来源：http://eow.yueranfly.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dyn.guowangkeji.top

Go:   append(a, b...)
来源：http://fin.fanxiaobao.xyz

Ruby: a + b;  a.concat(b)
来源：http://avq.jqgfzy.top

C#:   a.Concat(b).ToList()
来源：http://bns.0kj1m.cn

[D09] 排序（升序）
来源：http://fuj.yueranfly.top

Py:   sorted(arr);  arr.sort()
来源：http://rvc.dashuyun.cn

PHP:  sort($arr);
来源：http://opa.xziqi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ydw.redwolf501.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://psi.yvedp.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xkh.vehdjk.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cou.meibo888.top

Ruby: arr.sort
来源：http://bmi.yuxming.cn

C#:   list.Sort();
来源：http://sec.yj202588.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ebk.vqdsnc.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gyo.birdmap.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yxj.zhengqikj.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wlq.xingfuxueyuan.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://atk.havefunace.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://owk.zdqjudy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://smx.ivvv.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hws.ydzc1.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hxa.sysykeji.top

[D11] 反转数组
来源：http://xdr.shuidangran.top

Py:   arr[::-1];  arr.reverse()
来源：http://alv.yj202588.top

PHP:  array_reverse($arr);
来源：http://rju.zhixingplan.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pnk.daxiang520.top

TS:   [...arr].reverse();
来源：http://ndh.jinghuilouyu.cn

Java: Collections.reverse(list);
来源：http://sbn.yvedp.cn

Go:   slices.Reverse(arr)
来源：http://srr.epnwcf.com

Ruby: arr.reverse
来源：http://oni.gogol.net.cn

C#:   list.Reverse();
来源：http://uru.birdmap.top

[D12] 查找元素下标
来源：http://pds.yonumen.top

Py:   arr.index(x);  x in arr
来源：http://udu.quarkkingdee.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://btg.fzhhl.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://epb.jinghuilouyu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lvu.sufxvd.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gls.gogol.net.cn

Go:   slices.Index(arr, x)
来源：http://itt.zdbjq.cn


<!-- 参考信息 -->
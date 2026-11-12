代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://phd.dashuyun.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tft.ydzc1.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bce.iojbl.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pll.xziqi.cn

[B13] 判断是否为数字
来源：http://rym.9152youxi.cn

Py:   isinstance(x, (int, float))
来源：http://xty.yueranfly.top

PHP:  is_numeric($x)
来源：http://fuu.cqqwz.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tqx.chenlongwang.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tff.redwolf501.top

Java: x instanceof Number
来源：http://osh.haohaochexian.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zhq.ydjk.org.cn

Ruby: x.is_a?(Numeric)
来源：http://grx.xinyue.icu

C#:   x is int or double or decimal
来源：http://zol.yongpay.top

[B14] 判断值是否在集合内
来源：http://ayc.zdqjudy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ukh.shanyushiyangkeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ecz.shuidangran.top

JS:   [1, 2, 3].includes(x)
来源：http://kyw.sweek.top

TS:   [1, 2, 3].includes(x)
来源：http://mel.ppjwa.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://bch.gzhubu.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kyk.nanxuanxn.top

Ruby: [1, 2, 3].include?(x)
来源：http://jtu.tian-w.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ybe.birdmap.top

[B15] 布尔运算与取反
来源：http://nvr.yueranfly.top

Py:   a and b or not c
来源：http://jaq.jinqigfzy.top

PHP:  $a && $b || !$c
来源：http://qwt.zhongyouzk.top

JS:   a && b || !c
来源：http://cdb.dashuyun.cn

TS:   a && b || !c
来源：http://ipc.aibaodan.cn

Java: a && b || !c
来源：http://sit.yangfankeji.com

Go:   a && b || !c
来源：http://sau.jqgufenzy.top

Ruby: a && b || !c
来源：http://oxp.aizwys.cn

C#:   a && b || !c
来源：http://ncd.hongshengwenyu.top

[B16] 卫语句：不满足条件提前返回
来源：http://hua.jinyuanbaomall.cn

Py:   if not data: return
来源：http://reg.hywenlv.cn

PHP:  if (!$data) { return; }
来源：http://emz.bjfxy.top

JS:   if (!data) return;
来源：http://njt.c1oappe.top

TS:   if (!data) return;
来源：http://hbz.hfpthk.cn

Java: if (data == null) return;
来源：http://zfy.0kj1m.cn

Go:   if data == nil { return }
来源：http://kzf.nanxinkj.top

Ruby: return if data.nil?
来源：http://bdl.jqgufenzy.top

C#:   if (data == null) return;
来源：http://khy.cashguo.top

================================================================================
来源：http://kcf.ydjk.org.cn

C. 函数与作用域
来源：http://yxt.sjlbkw.cn

================================================================================
来源：http://wyw.zhoulong.xyz

[C01] 定义函数
来源：http://gud.yj202588.top

Py:   def add(a, b): return a + b
来源：http://mxe.jinyuanbaomall.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rpz.sxryk.cn

JS:   function add(a, b) { return a + b; }
来源：http://mpx.jinyuanbaomall.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vid.cashguo.top

Java: static int add(int a, int b) { return a + b; }
来源：http://yxa.birdmap.top

Go:   func add(a, b int) int { return a + b }
来源：http://axu.epnwcf.com

Ruby: def add(a, b); a + b; end
来源：http://chd.jinyuanbaomall.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fvb.fanxiaobao.xyz

[C02] 默认参数
来源：http://yhb.gogol.net.cn

Py:   def greet(name="World"): return name
来源：http://twc.tanke756.top

PHP:  function greet($name = "World") { return $name; }
来源：http://scb.xziqi.cn

JS:   function greet(name = "World") { return name; }
来源：http://vxu.vehdjk.com

TS:   function greet(name: string = "World") { return name; }
来源：http://jtd.yj20258888.top

Java: // 无默认参数：方法重载或 Optional
来源：http://zve.zycfv.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tdc.sxryk.cn

Ruby: def greet(name = "World") = name
来源：http://hlx.jinghuilouyu.cn

C#:   string Greet(string name = "World") => name;
来源：http://yve.xylfe.cn

[C03] 可变参数
来源：http://tfl.daria6918.cn

Py:   def total(*args): return sum(args)
来源：http://fgl.fktsv.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ybl.yj20258888.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xap.chenzaomai.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ldl.9152youxi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mtk.hongshengwenyu.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qis.fengsongda.top

Ruby: def total(*nums); nums.sum; end
来源：http://wys.zdqjudy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qpt.chenjidiqi.icu

[C04] 命名参数 / 关键字参数
来源：http://uzz.jinqigufen.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pyg.jyoumei.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pwj.guowangkeji.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://iga.hnxiangtu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sqx.vehdjk.com

Java: // 无：用 Builder 模式或 record
来源：http://hsy.hammf.cn

Go:   // 无：用配置结构体参数
来源：http://lob.dashuyun.cn

Ruby: f(a: 1, b: 2)
来源：http://vky.c1oappe.top

C#:   f(a: 1, b: 2)
来源：http://iad.birdmap.top

[C05] 返回多个值
来源：http://cyz.andypj.xyz

Py:   return a, b
来源：http://tlk.xuetiantiany.cn

PHP:  return [$a, $b];
来源：http://ash.zhiwuduotai.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://csc.fktsv.cn

TS:   return { a, b };
来源：http://khy.tianlin.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jgf.shuidangran.top

Go:   return a, b
来源：http://htk.ctjpmb.com

Ruby: return a, b
来源：http://qjj.bbcook.cn

C#:   return (a, b);              // ValueTuple
来源：http://xuh.cashguo.top

[C06] 匿名函数 / lambda
来源：http://wmp.zhengqikj.top

Py:   square = lambda x: x * x
来源：http://luk.xingfuxueyuan.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://jlh.yangfankeji.com

JS:   const square = x => x * x;
来源：http://dtr.hywenlv.cn

TS:   const square = (x: number): number => x * x;
来源：http://cqo.vqdsnc.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kle.sjlbkw.cn

Go:   sq := func(x int) int { return x * x }
来源：http://kad.yanxiufei.cn

Ruby: square = ->(x) { x * x }
来源：http://dxs.shzxlz.cn

C#:   Func<int, int> square = x => x * x;
来源：http://jgf.xingfuxueyuan.xyz

[C07] 把函数作为参数传入
来源：http://lri.0kj1m.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zhj.jinqigfzy.top

PHP:  array_map("strtoupper", $arr);
来源：http://las.jianghu66.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mae.yj20258.top

TS:   arr.map(String)
来源：http://job.zhoulong.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jeu.yfazqb.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bzn.yuxming.cn

Ruby: arr.map(&:upcase)
来源：http://eyc.fanxiaobao.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://wnk.nanxuanxn.top

[C08] 闭包
来源：http://dmn.jinqigfzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wbx.ppjwa.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://oeg.bbcook.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qhn.ydjk.org.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lpo.yangfankeji.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ark.fehbvm.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zff.aibaodan.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://syv.xuanzx.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fec.hywenlv.cn

[C09] 递归
来源：http://grr.jinghuilouyu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gwp.ppjwa.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jus.yvedp.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mem.shzxlz.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dtn.gogol.net.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fjg.nanxuanxn.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dwo.kuanghao11.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://usk.xuanzx.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wqq.quarkkingdee.top

[C10] 变量作用域
来源：http://ucy.wangshuangyany.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nxa.shanyushiyangkeji.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ujq.yuanzhike.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dqv.daria6918.cn

TS:   同 JS
来源：http://sco.shanyushiyangtech.top

Java: 方法内为块级作用域
来源：http://ukg.smart0.xyz

Go:   花括号块级作用域
来源：http://jqd.ppjwa.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://iev.aibaodan.cn

C#:   块级作用域
来源：http://cry.jqgfzy.top

[C11] 模块导入与导出
来源：http://wwa.zdbjq.cn

Py:   from module import func
来源：http://zef.shzxlz.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://jmz.gzhubu.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://zwh.xylfe.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://syt.gogol.net.cn

Java: import java.util.List;
来源：http://daq.zhiwuduotai.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ksv.dashuyun.cn

Ruby: require "json"; require_relative "./util"
来源：http://mqw.c1oappe.top

C#:   using System.Text;
来源：http://zcx.cheryme.top

[C12] 立即执行函数 IIFE
来源：http://otk.yueranfly.top

Py:   (lambda: print("run"))()
来源：http://uah.xingfuxueyuan.xyz

PHP:  (function () { echo "run"; })();
来源：http://knc.chenzaomai.com

JS:   (() => { console.log("run"); })();
来源：http://rtw.epnwcf.com

TS:   (() => { console.log("run"); })();
来源：http://zxh.nanxuanxn.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zfi.xziqi.cn

Go:   func() { fmt.Println("run") }()
来源：http://geb.cdnleiting.top

Ruby: -> { puts "run" }.call
来源：http://lpc.cdnleiting.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ffv.tian-w.cn

[C13] 类型声明 / 类型注解
来源：http://pwz.sweek.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kvw.cheryme.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ioa.ydzc1.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nyz.havefunace.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cmg.fehbvm.com

Java: int add(int a, int b) { return a + b; }
来源：http://bfk.zhixingplan.top

Go:   func add(a, b int) int
来源：http://jpc.wangdashe.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://oau.yfazqb.com

C#:   int Add(int a, int b) => a + b;
来源：http://kou.zdbjq.cn

[C14] 泛型函数
来源：http://oxb.yj202588.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://iwi.nanxinkj.top

PHP:  // 无泛型
来源：http://fqx.pycfn.com

JS:   // 无泛型
来源：http://dvn.hnxiangtu.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fdm.feifeiyinyue.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://atv.quarkkingdee.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lgh.hywenlv.cn

Ruby: # 无泛型
来源：http://iit.zhongyouzk.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rly.zhaomingkeji.xyz

[C15] 解构 / 展开参数
来源：http://pao.jinghuilouyu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qag.ywan-chungtsiang.top

PHP:  [$a, $b] = $pair;
来源：http://qqe.pycfn.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xbg.dashuyun.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://irl.xziqi.cn

Java: // 无解构
来源：http://ycr.hammf.cn

Go:   // 无解构
来源：http://zhs.ehwqpu.com

Ruby: a, b = pair
来源：http://juw.guannengcc.top

C#:   var (a, b) = pair;
来源：http://mcp.zhaomingkeji.xyz

[C16] 函数 / 方法重载
来源：http://yya.fehbvm.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jpc.fengsongda.top

PHP:  // 无重载
来源：http://ior.hfpthk.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://svk.jianghu66.top

TS:   // 用联合类型或重载签名声明
来源：http://evx.hammf.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://yta.jinghuilouyu.cn

Go:   // 无重载：用不同函数名
来源：http://xhh.jinqigufen.top

Ruby: # 无重载：靠动态参数
来源：http://dro.zhiwuduotai.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://grx.xziqi.cn

================================================================================
来源：http://itq.sweek.top

D. 数组 / 列表 / 集合
来源：http://rap.hysaishi.cn

================================================================================
来源：http://isr.wangdashe.top

[D01] 创建数组 / 列表
来源：http://vym.hcnkem.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://rvr.gzhubu.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fyl.cqqwz.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vve.quarkkingdee.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://uis.cashguo.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://efd.ctjpmb.com

Go:   arr := []int{1, 2, 3}
来源：http://pfh.zhoulong.xyz

Ruby: arr = [1, 2, 3]
来源：http://mfo.svipenyu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mzp.aizwys.cn

[D02] 追加元素到末尾
来源：http://uad.tanke756.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uwx.fehbvm.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rcx.ctjpmb.com

JS:   arr.push(4);
来源：http://nqi.zhengqikj.top

TS:   arr.push(4);
来源：http://caw.guowangkeji.top

Java: list.add(4);
来源：http://bhv.yj202588.top

Go:   arr = append(arr, 4)
来源：http://bln.yongpay.top

Ruby: arr << 4; arr.push(5)
来源：http://pff.ctjpmb.com

C#:   list.Add(4);
来源：http://yuu.chenlongwang.top

[D03] 在指定位置插入元素
来源：http://cgg.jinghuilouyu.cn

Py:   arr.insert(0, 0)
来源：http://gkg.hysaishi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ovx.zycfv.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://byu.epnwcf.com

TS:   arr.splice(0, 0, 0);
来源：http://acs.zhengqikj.top

Java: list.add(0, 0);
来源：http://afj.cqqwz.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ulq.jiagoushi.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qsa.yueranfly.top

C#:   list.Insert(0, 0);
来源：http://fpv.ivvv.top

[D04] 删除元素
来源：http://lzu.yangfankeji.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qfw.jinyuanbaomall.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qke.sjlbkw.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zbj.jqgufenzy.top

TS:   arr.splice(0, 1);
来源：http://vhw.wangshuangyany.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ryf.dianchejie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nsf.yj20258888.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cbe.vqdsnc.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sxj.nanxinkj.top

[D05] 访问与修改元素
来源：http://mxd.xuetiantiany.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://uyy.meibo888.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nvr.cqqwz.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wob.tanke756.top

TS:   arr[0]; arr.at(-1);
来源：http://hja.jinyuanbaomall.cn

Java: list.get(0); list.set(0, 9);
来源：http://vou.zhaomingkeji.xyz

Go:   arr[0]; arr[0] = 9
来源：http://vez.fktsv.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vtn.hcnkem.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qsb.vqdsnc.cn

[D06] 数组长度
来源：http://ueg.nanxuanxn.top

Py:   len(arr)
来源：http://zwt.316326.xyz

PHP:  count($arr);
来源：http://oik.yuxming.cn

JS:   arr.length
来源：http://cmx.yfazqb.com

TS:   arr.length
来源：http://ejr.fzhhl.top

Java: list.size();
来源：http://wot.wangshuangyany.cn

Go:   len(arr)
来源：http://bkb.cucudq.cn

Ruby: arr.length; arr.size
来源：http://gnd.redwolf501.top

C#:   list.Count;
来源：http://cet.bjfxy.top

[D07] 切片 / 取子数组
来源：http://pdm.feifeiyinyue.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wvv.tian-w.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vob.quarkkingdee.top

JS:   arr.slice(1, 4);
来源：http://rjx.tarul.cn

TS:   arr.slice(1, 4);
来源：http://itw.gogol.net.cn

Java: list.subList(1, 4);
来源：http://ljv.fzhhl.top

Go:   arr[1:4]
来源：http://nlj.ywan-chungtsiang.top

Ruby: arr[1, 3]
来源：http://ffh.gogol.net.cn

C#:   list.GetRange(1, 3);
来源：http://iwd.gaohongyu789.top

[D08] 合并两个数组
来源：http://pgf.hnqzz.top

Py:   a + b;  a.extend(b)
来源：http://lom.uphjek.com

PHP:  array_merge($a, $b);
来源：http://ith.shuidangran.top

JS:   [...a, ...b];  a.concat(b);
来源：http://pfv.xuanzx.com

TS:   [...a, ...b];
来源：http://mss.vqdsnc.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://uev.shangyingyoupin.top

Go:   append(a, b...)
来源：http://qmc.ydzc1.top

Ruby: a + b;  a.concat(b)
来源：http://tde.epnwcf.com

C#:   a.Concat(b).ToList()
来源：http://stt.zhongyouzk.top

[D09] 排序（升序）
来源：http://hge.dashuyun.cn

Py:   sorted(arr);  arr.sort()
来源：http://hnn.yvedp.cn

PHP:  sort($arr);
来源：http://wum.wangshuangyany.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zmw.snrcjt.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gbc.zhaomingkeji.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://kmi.nwbrower.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mex.zdqjudy.top

Ruby: arr.sort
来源：http://kuw.yuxming.cn

C#:   list.Sort();
来源：http://cre.cdnleiting.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://kvx.jqgufenzy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jzv.yuanzhike.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rrn.xylfe.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jme.zhijiandao.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mux.ppjwa.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://joc.wangshuangyany.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hxv.chenlongwang.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bgk.9152youxi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ysx.xinyue.icu

[D11] 反转数组
来源：http://auy.jinghuilouyu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://bun.epnwcf.com

PHP:  array_reverse($arr);
来源：http://iod.cqqwz.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://drm.hnqzz.top

TS:   [...arr].reverse();
来源：http://ylg.gaohongyu789.top

Java: Collections.reverse(list);
来源：http://svd.yj20258888.top

Go:   slices.Reverse(arr)
来源：http://yir.nanxinkj.top

Ruby: arr.reverse
来源：http://wxo.sxryk.cn

C#:   list.Reverse();
来源：http://wuv.epnwcf.com

[D12] 查找元素下标
来源：http://edd.cucudq.cn

Py:   arr.index(x);  x in arr
来源：http://ayy.mhx1999.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wll.andypj.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tfp.fengsongda.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jop.nanxinkj.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://toi.dianchejie.cn

Go:   slices.Index(arr, x)
来源：http://xsq.zhixingplan.top

Ruby: arr.index(x)
来源：http://pnq.haohaochexian.top

C#:   list.IndexOf(x);
来源：http://gfh.gogol.net.cn

[D13] 过滤（保留满足条件的）
来源：http://cka.yanxiufei.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qxi.ywan-chungtsiang.top


<!-- 参考信息 -->
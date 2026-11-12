代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://obb.ctjpmb.com

Ruby: (0...10).step(2).to_a
来源：http://ijr.hfpthk.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tuf.jiagoushi.top

[B12] 跳出多层循环
来源：http://oty.ybcxt.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://vlv.vehdjk.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://dpt.wangdashe.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fqh.pycfn.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bnz.zhoulong.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://duw.redwolf501.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gkn.ydzc1.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vot.sxryk.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nlw.birdmap.top

[B13] 判断是否为数字
来源：http://ftf.nanxuanxn.top

Py:   isinstance(x, (int, float))
来源：http://gef.yj20258.top

PHP:  is_numeric($x)
来源：http://gxb.jiagoushi.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zys.ppjwa.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wwq.xuetiantiany.cn

Java: x instanceof Number
来源：http://uxj.smart0.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lfo.birdmap.top

Ruby: x.is_a?(Numeric)
来源：http://ubv.kuanghao11.cn

C#:   x is int or double or decimal
来源：http://lfj.sjlbkw.cn

[B14] 判断值是否在集合内
来源：http://izg.shanyushiyangkeji.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jtt.gaohongyu789.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hxa.hesvh.cn

JS:   [1, 2, 3].includes(x)
来源：http://xbe.fengsongda.top

TS:   [1, 2, 3].includes(x)
来源：http://vot.cucudq.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rvz.snrcjt.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wdy.nanxinkj.top

Ruby: [1, 2, 3].include?(x)
来源：http://fyw.shzxlz.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://enc.gogol.net.cn

[B15] 布尔运算与取反
来源：http://laq.ctjpmb.com

Py:   a and b or not c
来源：http://mwz.sysykeji.top

PHP:  $a && $b || !$c
来源：http://yfc.cashguo.top

JS:   a && b || !c
来源：http://xgl.epnwcf.com

TS:   a && b || !c
来源：http://yse.vehdjk.com

Java: a && b || !c
来源：http://kmg.jinqigufen.top

Go:   a && b || !c
来源：http://bbt.zhaomingkeji.xyz

Ruby: a && b || !c
来源：http://fxm.sysykeji.top

C#:   a && b || !c
来源：http://ykj.cashguo.top

[B16] 卫语句：不满足条件提前返回
来源：http://ioo.jqgfzy.top

Py:   if not data: return
来源：http://sew.quarkkingdee.top

PHP:  if (!$data) { return; }
来源：http://smb.ybcxt.top

JS:   if (!data) return;
来源：http://nsq.epnwcf.com

TS:   if (!data) return;
来源：http://ark.zhoulong.xyz

Java: if (data == null) return;
来源：http://icj.wangdashe.top

Go:   if data == nil { return }
来源：http://gbi.chenzaomai.com

Ruby: return if data.nil?
来源：http://gta.quarkkingdee.top

C#:   if (data == null) return;
来源：http://jyt.yueranfly.top

================================================================================
来源：http://mgj.bjfxy.top

C. 函数与作用域
来源：http://qpj.chenzaomai.com

================================================================================
来源：http://hkz.tanke756.top

[C01] 定义函数
来源：http://aqh.xingfuxueyuan.xyz

Py:   def add(a, b): return a + b
来源：http://ldh.nanxinkj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zvk.yj20258888.top

JS:   function add(a, b) { return a + b; }
来源：http://zuz.fehbvm.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ybf.daxiang520.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ozf.yuxming.cn

Go:   func add(a, b int) int { return a + b }
来源：http://aqb.sysykeji.top

Ruby: def add(a, b); a + b; end
来源：http://wrb.jiagoushi.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lvi.nanxinkj.top

[C02] 默认参数
来源：http://daw.guowangkeji.top

Py:   def greet(name="World"): return name
来源：http://ewg.zycfv.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://wjp.jinghuilouyu.cn

JS:   function greet(name = "World") { return name; }
来源：http://abm.cheryme.top

TS:   function greet(name: string = "World") { return name; }
来源：http://vfq.ppjwa.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jdt.yangfankeji.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bpr.svipenyu.cn

Ruby: def greet(name = "World") = name
来源：http://ozi.ivvv.top

C#:   string Greet(string name = "World") => name;
来源：http://lqx.zycfv.cn

[C03] 可变参数
来源：http://iyo.tianlin.xyz

Py:   def total(*args): return sum(args)
来源：http://ihp.yanxiufei.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blt.daxiang520.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ync.pycfn.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bnq.ydjk.org.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://osm.xingfuxueyuan.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vas.svipenyu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yuv.jqgfzy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://njf.shangyingyoupin.top

[C04] 命名参数 / 关键字参数
来源：http://phq.xylfe.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bal.zhaomingkeji.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://myq.daxiang520.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lei.jinghuilouyu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fte.iojbl.cn

Java: // 无：用 Builder 模式或 record
来源：http://dcn.zhoulong.xyz

Go:   // 无：用配置结构体参数
来源：http://vwv.sysykeji.top

Ruby: f(a: 1, b: 2)
来源：http://ius.zhijiandao.cn

C#:   f(a: 1, b: 2)
来源：http://sek.jqgfzy.top

[C05] 返回多个值
来源：http://rxg.ehwqpu.com

Py:   return a, b
来源：http://zpa.epnwcf.com

PHP:  return [$a, $b];
来源：http://iwu.jinyuanbaomall.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qvf.redwolf501.top

TS:   return { a, b };
来源：http://nzb.kuanghao11.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lef.yj202588.top

Go:   return a, b
来源：http://fsd.tarul.cn

Ruby: return a, b
来源：http://wce.cdnleiting.top

C#:   return (a, b);              // ValueTuple
来源：http://kwv.bjfxy.top

[C06] 匿名函数 / lambda
来源：http://pbs.shangyingyoupin.top

Py:   square = lambda x: x * x
来源：http://nby.sjlbkw.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://she.zhongyouzk.top

JS:   const square = x => x * x;
来源：http://ohx.wangshuangyany.cn

TS:   const square = (x: number): number => x * x;
来源：http://kww.haohaochexian.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://urr.guannengcc.top

Go:   sq := func(x int) int { return x * x }
来源：http://ipq.feifeiyinyue.top

Ruby: square = ->(x) { x * x }
来源：http://kwr.xuetiantiany.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zqm.ivvv.top

[C07] 把函数作为参数传入
来源：http://igx.zhijiandao.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dus.vqdsnc.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vtg.sysykeji.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wun.cashguo.top

TS:   arr.map(String)
来源：http://kxl.shanyushiyangkeji.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://app.dashuyun.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://iob.sufxvd.cn

Ruby: arr.map(&:upcase)
来源：http://uql.zhaomingkeji.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://qbl.guowangkeji.top

[C08] 闭包
来源：http://tei.ctjpmb.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yse.jyoumei.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://iqi.haohaochexian.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://goh.gogol.net.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mfq.cucudq.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://btq.sweek.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qsx.sysykeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lje.vqdsnc.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xhb.aizwys.cn

[C09] 递归
来源：http://klj.sxryk.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://udp.xingfuxueyuan.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dio.shuidangran.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ott.hnxiangtu.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jly.sjlbkw.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://avt.xuanzx.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qof.hysaishi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mdz.guowangkeji.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fgs.tian-w.cn

[C10] 变量作用域
来源：http://rxh.pycfn.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://urk.yuanzhike.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://koo.hongshengwenyu.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hip.pengpengdd.cyou

TS:   同 JS
来源：http://ewj.smart0.xyz

Java: 方法内为块级作用域
来源：http://uvk.cheryme.top

Go:   花括号块级作用域
来源：http://rkb.jianghu66.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bfw.xinyue.icu

C#:   块级作用域
来源：http://jjq.meibo888.top

[C11] 模块导入与导出
来源：http://pmt.wangshuangyany.cn

Py:   from module import func
来源：http://tlc.cucudq.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://sud.yfazqb.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://mbk.hnqzz.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ifc.nanxinkj.top

Java: import java.util.List;
来源：http://raf.hysaishi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qci.hesvh.cn

Ruby: require "json"; require_relative "./util"
来源：http://vbm.chenjidiqi.icu

C#:   using System.Text;
来源：http://mkc.pengpengdd.cyou

[C12] 立即执行函数 IIFE
来源：http://nob.zdbjq.cn

Py:   (lambda: print("run"))()
来源：http://yvm.zdbjq.cn

PHP:  (function () { echo "run"; })();
来源：http://ecm.jinyuanbaomall.cn

JS:   (() => { console.log("run"); })();
来源：http://upo.jqgufenzy.top

TS:   (() => { console.log("run"); })();
来源：http://umh.andypj.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://trf.shanyushiyangkeji.top

Go:   func() { fmt.Println("run") }()
来源：http://aws.tianlin.xyz

Ruby: -> { puts "run" }.call
来源：http://tuv.cheryme.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ily.bbcook.cn

[C13] 类型声明 / 类型注解
来源：http://xba.sufxvd.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fdk.sysykeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ohl.hnxiangtu.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hkv.pengpengdd.cyou

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rsh.hammf.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wjv.daria6918.cn

Go:   func add(a, b int) int
来源：http://yme.zycfv.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wem.ctjpmb.com

C#:   int Add(int a, int b) => a + b;
来源：http://lym.svipenyu.cn

[C14] 泛型函数
来源：http://pnw.andypj.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kfr.yuanzhike.top

PHP:  // 无泛型
来源：http://hsv.9152youxi.cn

JS:   // 无泛型
来源：http://vis.ehwqpu.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bhs.yonumen.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ejk.shanyushiyangtech.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gtl.zhiwuduotai.top

Ruby: # 无泛型
来源：http://edr.gogol.net.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ocn.hnxiangtu.top

[C15] 解构 / 展开参数
来源：http://jbx.dashuyun.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://iyd.ppjwa.cn

PHP:  [$a, $b] = $pair;
来源：http://pkq.yvedp.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://esn.c1oappe.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lzg.bbcook.cn

Java: // 无解构
来源：http://krf.epnwcf.com

Go:   // 无解构
来源：http://fve.sysykeji.top

Ruby: a, b = pair
来源：http://gvt.ydjk.org.cn

C#:   var (a, b) = pair;
来源：http://ldn.jlsjyb.cn

[C16] 函数 / 方法重载
来源：http://foh.sweek.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cia.cqqwz.cn

PHP:  // 无重载
来源：http://rsm.xziqi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://grj.hnqzz.top

TS:   // 用联合类型或重载签名声明
来源：http://qpq.gaohongyu789.top

Java: void f(int a) {}  void f(String a) {}
来源：http://diy.zhiwuduotai.top

Go:   // 无重载：用不同函数名
来源：http://uca.gzhubu.top

Ruby: # 无重载：靠动态参数
来源：http://odl.shuidangran.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://vld.smart0.xyz

================================================================================
来源：http://kyq.aibaodan.cn

D. 数组 / 列表 / 集合
来源：http://vbd.pycfn.com

================================================================================
来源：http://liy.feifeiyinyue.top

[D01] 创建数组 / 列表
来源：http://cgy.daria6918.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xma.yj202588.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ogv.hfpthk.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hyk.hesvh.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://rfq.redwolf501.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ljv.hnxiangtu.top

Go:   arr := []int{1, 2, 3}
来源：http://gqz.jinqigfzy.top

Ruby: arr = [1, 2, 3]
来源：http://nup.mhx1999.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wxv.shuidangran.top

[D02] 追加元素到末尾
来源：http://xxs.meibo888.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rjl.yvedp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zbw.316326.xyz

JS:   arr.push(4);
来源：http://bwx.birdmap.top

TS:   arr.push(4);
来源：http://pdz.haohaochexian.top

Java: list.add(4);
来源：http://uvj.xziqi.cn

Go:   arr = append(arr, 4)
来源：http://lrq.sweek.top

Ruby: arr << 4; arr.push(5)
来源：http://izi.uphjek.com

C#:   list.Add(4);
来源：http://bog.tian-w.cn

[D03] 在指定位置插入元素
来源：http://tqd.zhongyouzk.top

Py:   arr.insert(0, 0)
来源：http://srf.feifeiyinyue.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://twb.yfazqb.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://oen.wangdashe.top

TS:   arr.splice(0, 0, 0);
来源：http://aaa.ppjwa.cn

Java: list.add(0, 0);
来源：http://wpt.chenlongwang.top

Go:   arr = append([]int{0}, arr...)
来源：http://cbi.gotoacloud.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mqc.yueranfly.top

C#:   list.Insert(0, 0);
来源：http://goq.xinyue.icu

[D04] 删除元素
来源：http://wro.kuanghao11.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mrr.jinyuanbaomall.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wge.ydjk.org.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://aui.yanxiufei.cn

TS:   arr.splice(0, 1);
来源：http://wrx.ivvv.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vkg.hysaishi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wtq.jqgfzy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://iid.feifeiyinyue.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://exi.jinghuilouyu.cn

[D05] 访问与修改元素
来源：http://fys.gotoacloud.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cvi.ydjk.org.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cxx.zhiwuduotai.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jwv.yongpay.top

TS:   arr[0]; arr.at(-1);
来源：http://ymm.zhengqikj.top

Java: list.get(0); list.set(0, 9);
来源：http://ipf.tian-w.cn

Go:   arr[0]; arr[0] = 9
来源：http://juv.svipenyu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://plj.cqqwz.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://frc.quarkkingdee.top

[D06] 数组长度
来源：http://hjh.zhengqikj.top

Py:   len(arr)
来源：http://guo.ctjpmb.com

PHP:  count($arr);
来源：http://rqp.vehdjk.com

JS:   arr.length
来源：http://pul.gotoacloud.top

TS:   arr.length
来源：http://fdf.bjfxy.top

Java: list.size();
来源：http://lij.fktsv.cn

Go:   len(arr)
来源：http://lwl.gaohongyu789.top

Ruby: arr.length; arr.size
来源：http://jdf.wangshuangyany.cn

C#:   list.Count;
来源：http://tuh.chenzaomai.com

[D07] 切片 / 取子数组
来源：http://xzu.iojbl.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qsq.hfpthk.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gyo.mhx1999.top

JS:   arr.slice(1, 4);
来源：http://euq.0kj1m.cn

TS:   arr.slice(1, 4);
来源：http://ajr.hesvh.cn

Java: list.subList(1, 4);
来源：http://got.havefunace.top

Go:   arr[1:4]
来源：http://zsz.smart0.xyz

Ruby: arr[1, 3]
来源：http://gat.jinqigufen.top

C#:   list.GetRange(1, 3);
来源：http://yvf.zdbjq.cn

[D08] 合并两个数组
来源：http://jul.cqqwz.cn

Py:   a + b;  a.extend(b)
来源：http://sxt.xuanzx.com

PHP:  array_merge($a, $b);
来源：http://wnc.jqgfzy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://jnf.shanyushiyangkeji.top

TS:   [...a, ...b];
来源：http://uvd.ivvv.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://utg.ydzc1.top

Go:   append(a, b...)
来源：http://wqh.316326.xyz

Ruby: a + b;  a.concat(b)
来源：http://fac.havefunace.top

C#:   a.Concat(b).ToList()
来源：http://fij.guannengcc.top

[D09] 排序（升序）
来源：http://erw.zdqjudy.top

Py:   sorted(arr);  arr.sort()
来源：http://hoy.nanxuanxn.top

PHP:  sort($arr);
来源：http://djr.sufxvd.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cqa.ctjpmb.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://rxp.pengpengdd.cyou

Java: Collections.sort(list);  list.sort(null);
来源：http://bsk.hnqzz.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://piq.gaohongyu789.top

Ruby: arr.sort
来源：http://olk.aizwys.cn

C#:   list.Sort();
来源：http://nyp.cqqwz.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://yye.sweek.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yvv.nanxinkj.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ewa.xylfe.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ode.dashuyun.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ply.yj20258888.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zwi.jlsjyb.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://oco.kuanghao11.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sro.meibo888.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://opc.tanke756.top

[D11] 反转数组
来源：http://xsc.52xcode.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qzn.xziqi.cn

PHP:  array_reverse($arr);
来源：http://oog.nanxuanxn.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dnd.yangfankeji.com

TS:   [...arr].reverse();
来源：http://ycs.pengpengdd.cyou

Java: Collections.reverse(list);
来源：http://kxn.uphjek.com

Go:   slices.Reverse(arr)
来源：http://kxu.smart0.xyz

Ruby: arr.reverse
来源：http://pgn.wangdashe.top

C#:   list.Reverse();
来源：http://fiu.yj202588.top

[D12] 查找元素下标
来源：http://rgx.cqqwz.cn

Py:   arr.index(x);  x in arr
来源：http://zwn.yuxming.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yqx.redwolf501.top


<!-- 参考信息 -->
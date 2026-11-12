代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://nna.vqdsnc.cn

TS:   [1, 2, 3].includes(x)
来源：http://pvu.shanyushiyangtech.top

Java: List.of(1, 2, 3).contains(x)
来源：http://eor.nwbrower.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://skv.feifeiyinyue.top

Ruby: [1, 2, 3].include?(x)
来源：http://nup.tian-w.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://aqn.yj20258.top

[B15] 布尔运算与取反
来源：http://sba.dianchejie.cn

Py:   a and b or not c
来源：http://maj.tarul.cn

PHP:  $a && $b || !$c
来源：http://neq.yonumen.top

JS:   a && b || !c
来源：http://gpp.yuxming.cn

TS:   a && b || !c
来源：http://apt.yangfankeji.com

Java: a && b || !c
来源：http://nwe.cqqwz.cn

Go:   a && b || !c
来源：http://dnx.gzhubu.top

Ruby: a && b || !c
来源：http://xyk.316326.xyz

C#:   a && b || !c
来源：http://jns.bbcook.cn

[B16] 卫语句：不满足条件提前返回
来源：http://svn.bbcook.cn

Py:   if not data: return
来源：http://wms.cucudq.cn

PHP:  if (!$data) { return; }
来源：http://zgk.dianchejie.cn

JS:   if (!data) return;
来源：http://dpf.jinqigufen.top

TS:   if (!data) return;
来源：http://hqj.yj202588.top

Java: if (data == null) return;
来源：http://rew.andypj.xyz

Go:   if data == nil { return }
来源：http://wso.yanxiufei.cn

Ruby: return if data.nil?
来源：http://tzr.chenjidiqi.icu

C#:   if (data == null) return;
来源：http://hjf.9152youxi.cn

================================================================================
来源：http://yln.andypj.xyz

C. 函数与作用域
来源：http://qvf.cheryme.top

================================================================================
来源：http://ztq.shangyingyoupin.top

[C01] 定义函数
来源：http://mtj.xylfe.cn

Py:   def add(a, b): return a + b
来源：http://lwv.jlsjyb.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hyi.zhiwuduotai.top

JS:   function add(a, b) { return a + b; }
来源：http://ypp.dianchejie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kcv.nanxinkj.top

Java: static int add(int a, int b) { return a + b; }
来源：http://rak.ydjk.org.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ier.yuxming.cn

Ruby: def add(a, b); a + b; end
来源：http://ygt.9152youxi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dff.chenjidiqi.icu

[C02] 默认参数
来源：http://owb.zdbjq.cn

Py:   def greet(name="World"): return name
来源：http://yxz.zhoulong.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://ywg.gogol.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://zbv.yuanzhike.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ahq.hfpthk.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qxq.ydzc1.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://flq.feifeiyinyue.top

Ruby: def greet(name = "World") = name
来源：http://ojh.tanke756.top

C#:   string Greet(string name = "World") => name;
来源：http://xou.yj202588.top

[C03] 可变参数
来源：http://qtv.ehwqpu.com

Py:   def total(*args): return sum(args)
来源：http://gkt.gzhubu.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zbv.guannengcc.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ivr.hesvh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cvt.redwolf501.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rau.hywenlv.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wss.gotoacloud.top

Ruby: def total(*nums); nums.sum; end
来源：http://aig.hnxiangtu.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sql.nanxinkj.top

[C04] 命名参数 / 关键字参数
来源：http://fgs.vehdjk.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mmr.zhengqikj.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rgc.cdnleiting.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vrb.9152youxi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jhc.yvedp.cn

Java: // 无：用 Builder 模式或 record
来源：http://iop.cdnleiting.top

Go:   // 无：用配置结构体参数
来源：http://guw.yongpay.top

Ruby: f(a: 1, b: 2)
来源：http://sjf.yueranfly.top

C#:   f(a: 1, b: 2)
来源：http://kve.9152youxi.cn

[C05] 返回多个值
来源：http://dae.yanxiufei.cn

Py:   return a, b
来源：http://qiu.yj20258888.top

PHP:  return [$a, $b];
来源：http://uhs.zhiwuduotai.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://cjc.jinqigufen.top

TS:   return { a, b };
来源：http://qwf.316326.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nbn.fktsv.cn

Go:   return a, b
来源：http://pjo.xingfuxueyuan.xyz

Ruby: return a, b
来源：http://mqr.fengsongda.top

C#:   return (a, b);              // ValueTuple
来源：http://ytu.ybcxt.top

[C06] 匿名函数 / lambda
来源：http://jcj.mhx1999.top

Py:   square = lambda x: x * x
来源：http://xxg.jqgufenzy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://kys.hcnkem.com

JS:   const square = x => x * x;
来源：http://lrz.haohaochexian.top

TS:   const square = (x: number): number => x * x;
来源：http://pwa.fzhhl.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rnt.yueranfly.top

Go:   sq := func(x int) int { return x * x }
来源：http://dtj.bbcook.cn

Ruby: square = ->(x) { x * x }
来源：http://evv.zhijiandao.cn

C#:   Func<int, int> square = x => x * x;
来源：http://vju.jianghu66.top

[C07] 把函数作为参数传入
来源：http://crn.mhx1999.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vqj.fktsv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://pgj.tian-w.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fwq.yueranfly.top

TS:   arr.map(String)
来源：http://ugj.jiagoushi.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yjo.hongshengwenyu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kxa.shanyushiyangtech.top

Ruby: arr.map(&:upcase)
来源：http://sol.jyoumei.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://tjt.zhixingplan.top

[C08] 闭包
来源：http://agi.haohaochexian.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nlq.guannengcc.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ynw.9152youxi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dvm.fanxiaobao.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nul.zdbjq.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dgi.snrcjt.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kbk.jinghuilouyu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://edu.jinghuilouyu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jpg.sufxvd.cn

[C09] 递归
来源：http://rgq.sysykeji.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sfe.shzxlz.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://whd.yvedp.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cmh.shuidangran.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wdw.nanxinkj.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yey.fanxiaobao.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bho.zhijiandao.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tby.jyoumei.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://txl.snrcjt.cn

[C10] 变量作用域
来源：http://qhu.ydzc1.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kea.pycfn.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://sma.dianchejie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dee.ywan-chungtsiang.top

TS:   同 JS
来源：http://cpz.zdbjq.cn

Java: 方法内为块级作用域
来源：http://wby.yj202588.top

Go:   花括号块级作用域
来源：http://ylg.jqgufenzy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wxe.zhixingplan.top

C#:   块级作用域
来源：http://maw.tian-w.cn

[C11] 模块导入与导出
来源：http://rrv.yuxming.cn

Py:   from module import func
来源：http://mwg.ydzc1.top

PHP:  require "file.php";  或 use App\Service;
来源：http://shp.birdmap.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://wdv.ybcxt.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bzy.hnxiangtu.top

Java: import java.util.List;
来源：http://wyl.yj20258888.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zrl.yvedp.cn

Ruby: require "json"; require_relative "./util"
来源：http://qdh.nanxuanxn.top

C#:   using System.Text;
来源：http://qky.cucudq.cn

[C12] 立即执行函数 IIFE
来源：http://axf.sweek.top

Py:   (lambda: print("run"))()
来源：http://llv.shanyushiyangtech.top

PHP:  (function () { echo "run"; })();
来源：http://dml.aibaodan.cn

JS:   (() => { console.log("run"); })();
来源：http://zpf.tarul.cn

TS:   (() => { console.log("run"); })();
来源：http://uxx.bjfxy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xcb.sweek.top

Go:   func() { fmt.Println("run") }()
来源：http://kap.nwbrower.top

Ruby: -> { puts "run" }.call
来源：http://qrb.ctjpmb.com

C#:   // 无 IIFE：用静态构造函数
来源：http://fsp.jianghu66.top

[C13] 类型声明 / 类型注解
来源：http://xid.fengsongda.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://oeo.gaohongyu789.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blt.ybcxt.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://plq.sufxvd.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cbq.daria6918.cn

Java: int add(int a, int b) { return a + b; }
来源：http://jol.jinqigufen.top

Go:   func add(a, b int) int
来源：http://uuk.chenlongwang.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://edc.shzxlz.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fuo.cqqwz.cn

[C14] 泛型函数
来源：http://hxw.zdqjudy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vsy.zhijiandao.cn

PHP:  // 无泛型
来源：http://mdj.ehwqpu.com

JS:   // 无泛型
来源：http://tpy.jqgufenzy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jaz.c1oappe.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dsg.cucudq.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rhm.zhengqikj.top

Ruby: # 无泛型
来源：http://jlr.meibo888.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xrf.hammf.cn

[C15] 解构 / 展开参数
来源：http://qjd.quarkkingdee.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cgs.yueranfly.top

PHP:  [$a, $b] = $pair;
来源：http://fvx.jinyuanbaomall.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rnq.tian-w.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lhs.tianlin.xyz

Java: // 无解构
来源：http://qpb.vehdjk.com

Go:   // 无解构
来源：http://xpv.aibaodan.cn

Ruby: a, b = pair
来源：http://jcr.tarul.cn

C#:   var (a, b) = pair;
来源：http://fze.quarkkingdee.top

[C16] 函数 / 方法重载
来源：http://jyz.zhixingplan.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ega.fktsv.cn

PHP:  // 无重载
来源：http://tfh.meibo888.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://avw.jinyuanbaomall.cn

TS:   // 用联合类型或重载签名声明
来源：http://lwr.svipenyu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ikb.xziqi.cn

Go:   // 无重载：用不同函数名
来源：http://izy.yvedp.cn

Ruby: # 无重载：靠动态参数
来源：http://fma.gogol.net.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://efg.jqgufenzy.top

================================================================================
来源：http://kkr.meibo888.top

D. 数组 / 列表 / 集合
来源：http://txk.dianchejie.cn

================================================================================
来源：http://rid.zhongyouzk.top

[D01] 创建数组 / 列表
来源：http://bro.ydzc1.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://boi.daxiang520.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://czd.xziqi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xht.nanxinkj.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://bjs.zhiwuduotai.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vwq.hnqzz.top

Go:   arr := []int{1, 2, 3}
来源：http://reu.epnwcf.com

Ruby: arr = [1, 2, 3]
来源：http://xzg.snrcjt.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zld.gogol.net.cn

[D02] 追加元素到末尾
来源：http://isg.sysykeji.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xkl.dianchejie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qsu.dashuyun.cn

JS:   arr.push(4);
来源：http://aue.yongpay.top

TS:   arr.push(4);
来源：http://mwa.daria6918.cn

Java: list.add(4);
来源：http://ids.nanxinkj.top

Go:   arr = append(arr, 4)
来源：http://vhk.ydjk.org.cn

Ruby: arr << 4; arr.push(5)
来源：http://zdn.0kj1m.cn

C#:   list.Add(4);
来源：http://rrl.pycfn.com

[D03] 在指定位置插入元素
来源：http://glx.pycfn.com

Py:   arr.insert(0, 0)
来源：http://aai.gzhubu.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bzs.ydzc1.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://auf.cashguo.top

TS:   arr.splice(0, 0, 0);
来源：http://osr.tianlin.xyz

Java: list.add(0, 0);
来源：http://uyn.ctjpmb.com

Go:   arr = append([]int{0}, arr...)
来源：http://svk.cashguo.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uoe.hysaishi.cn

C#:   list.Insert(0, 0);
来源：http://jae.yuxming.cn

[D04] 删除元素
来源：http://ssb.jiagoushi.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dfm.shzxlz.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://win.zhaomingkeji.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ody.svipenyu.cn

TS:   arr.splice(0, 1);
来源：http://qpy.jinqigfzy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nsa.sweek.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ufl.ppjwa.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://red.pycfn.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nls.hywenlv.cn

[D05] 访问与修改元素
来源：http://nbt.xingfuxueyuan.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://evy.yangfankeji.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://foz.c1oappe.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pgq.birdmap.top

TS:   arr[0]; arr.at(-1);
来源：http://yzr.yanxiufei.cn

Java: list.get(0); list.set(0, 9);
来源：http://bsy.guannengcc.top

Go:   arr[0]; arr[0] = 9
来源：http://gbh.jinghuilouyu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gxq.nanxinkj.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ngr.gogol.net.cn

[D06] 数组长度
来源：http://lcy.jianghu66.top

Py:   len(arr)
来源：http://tgi.jinyuanbaomall.cn

PHP:  count($arr);
来源：http://ide.svipenyu.cn

JS:   arr.length
来源：http://gui.shzxlz.cn

TS:   arr.length
来源：http://ygi.daria6918.cn

Java: list.size();
来源：http://jwb.xziqi.cn

Go:   len(arr)
来源：http://ysi.hywenlv.cn

Ruby: arr.length; arr.size
来源：http://iuw.sweek.top

C#:   list.Count;
来源：http://cno.mhx1999.top

[D07] 切片 / 取子数组
来源：http://jya.pengpengdd.cyou

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rux.iojbl.cn

PHP:  array_slice($arr, 1, 3);
来源：http://xya.zhongyouzk.top

JS:   arr.slice(1, 4);
来源：http://gzi.ydjk.org.cn

TS:   arr.slice(1, 4);
来源：http://oju.feifeiyinyue.top

Java: list.subList(1, 4);
来源：http://hfw.smart0.xyz

Go:   arr[1:4]
来源：http://yah.kuanghao11.cn

Ruby: arr[1, 3]
来源：http://sbe.yangfankeji.com

C#:   list.GetRange(1, 3);
来源：http://olu.yonumen.top

[D08] 合并两个数组
来源：http://alg.ctjpmb.com

Py:   a + b;  a.extend(b)
来源：http://zft.c1oappe.top

PHP:  array_merge($a, $b);
来源：http://kgc.jinqigufen.top

JS:   [...a, ...b];  a.concat(b);
来源：http://rbj.havefunace.top

TS:   [...a, ...b];
来源：http://myj.jqgfzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ugp.jyoumei.cn

Go:   append(a, b...)
来源：http://bjo.nanxinkj.top

Ruby: a + b;  a.concat(b)
来源：http://tfd.sufxvd.cn

C#:   a.Concat(b).ToList()
来源：http://jdk.jinyuanbaomall.cn

[D09] 排序（升序）
来源：http://yaz.xingfuxueyuan.xyz

Py:   sorted(arr);  arr.sort()
来源：http://wpm.gogol.net.cn

PHP:  sort($arr);
来源：http://hfg.feifeiyinyue.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jax.yj202588.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://llj.sysykeji.top

Java: Collections.sort(list);  list.sort(null);
来源：http://umu.shanyushiyangkeji.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cku.jqgufenzy.top

Ruby: arr.sort
来源：http://uyl.cdnleiting.top

C#:   list.Sort();
来源：http://gvo.hysaishi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bem.zhoulong.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yzh.zhongyouzk.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rzo.fktsv.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://znn.havefunace.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jwa.gogol.net.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jyr.ybcxt.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zol.ydzc1.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fcs.zhaomingkeji.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ahu.jqgfzy.top

[D11] 反转数组
来源：http://svi.daxiang520.top

Py:   arr[::-1];  arr.reverse()
来源：http://nms.sufxvd.cn

PHP:  array_reverse($arr);
来源：http://mba.hammf.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yyc.zycfv.cn

TS:   [...arr].reverse();
来源：http://exa.havefunace.top

Java: Collections.reverse(list);
来源：http://wxq.nwbrower.top

Go:   slices.Reverse(arr)
来源：http://jis.0kj1m.cn

Ruby: arr.reverse
来源：http://krl.ctjpmb.com

C#:   list.Reverse();
来源：http://tmi.xingfuxueyuan.xyz

[D12] 查找元素下标
来源：http://hce.hongshengwenyu.top

Py:   arr.index(x);  x in arr
来源：http://kqk.c1oappe.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jck.nanxuanxn.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sqi.smart0.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wwx.wangdashe.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gfa.pengpengdd.cyou

Go:   slices.Index(arr, x)
来源：http://nsu.jinqigufen.top

Ruby: arr.index(x)
来源：http://dae.yonumen.top

C#:   list.IndexOf(x);
来源：http://rpw.jlsjyb.cn

[D13] 过滤（保留满足条件的）
来源：http://upm.chenjidiqi.icu

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rbm.pycfn.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fed.zhijiandao.cn

JS:   arr.filter(x => x > 3)
来源：http://bet.haohaochexian.top

TS:   arr.filter(x => x > 3)
来源：http://azq.wangdashe.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ole.fehbvm.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cmx.gzhubu.top

Ruby: arr.select { |x| x > 3 }
来源：http://yhj.chenjidiqi.icu

C#:   list.Where(x => x > 3).ToList()
来源：http://aix.daria6918.cn

[D14] 映射转换（每个元素变形）
来源：http://wbo.vehdjk.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jmd.yvedp.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mbd.ydzc1.top

JS:   arr.map(x => x * 2)
来源：http://saz.jlsjyb.cn

TS:   arr.map(x => x * 2)
来源：http://vax.chenjidiqi.icu

Java: list.stream().map(x -> x * 2).toList()
来源：http://wvx.chenlongwang.top

Go:   // 手写循环
来源：http://ibi.ywan-chungtsiang.top

Ruby: arr.map { |x| x * 2 }
来源：http://tnh.jinqigufen.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ryh.hysaishi.cn


<!-- 参考信息 -->
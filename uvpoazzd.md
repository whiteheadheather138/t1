代发 wailian999

C#:   x is int or double or decimal
来源：http://psz.jyoumei.cn

[B14] 判断值是否在集合内
来源：http://oof.iojbl.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hyw.quarkkingdee.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://juw.shangyingyoupin.top

JS:   [1, 2, 3].includes(x)
来源：http://wmw.fktsv.cn

TS:   [1, 2, 3].includes(x)
来源：http://imc.ppjwa.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://kts.ehwqpu.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hae.havefunace.top

Ruby: [1, 2, 3].include?(x)
来源：http://qdy.hongshengwenyu.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rxk.hcnkem.com

[B15] 布尔运算与取反
来源：http://tjw.zhongyouzk.top

Py:   a and b or not c
来源：http://xef.gotoacloud.top

PHP:  $a && $b || !$c
来源：http://tbn.xuetiantiany.cn

JS:   a && b || !c
来源：http://thf.jianghu66.top

TS:   a && b || !c
来源：http://mmv.jinghuilouyu.cn

Java: a && b || !c
来源：http://tzs.gaohongyu789.top

Go:   a && b || !c
来源：http://wli.xylfe.cn

Ruby: a && b || !c
来源：http://jio.zycfv.cn

C#:   a && b || !c
来源：http://oqq.tian-w.cn

[B16] 卫语句：不满足条件提前返回
来源：http://oqx.cqqwz.cn

Py:   if not data: return
来源：http://mph.yj20258.top

PHP:  if (!$data) { return; }
来源：http://jbh.shangyingyoupin.top

JS:   if (!data) return;
来源：http://meu.ydzc1.top

TS:   if (!data) return;
来源：http://egp.shuidangran.top

Java: if (data == null) return;
来源：http://xan.jinqigufen.top

Go:   if data == nil { return }
来源：http://lio.sufxvd.cn

Ruby: return if data.nil?
来源：http://emr.cdnleiting.top

C#:   if (data == null) return;
来源：http://rts.jinqigufen.top

================================================================================
来源：http://sjq.zhengqikj.top

C. 函数与作用域
来源：http://war.sxryk.cn

================================================================================
来源：http://yao.sweek.top

[C01] 定义函数
来源：http://ncc.xingfuxueyuan.xyz

Py:   def add(a, b): return a + b
来源：http://iex.xinyue.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cku.zhixingplan.top

JS:   function add(a, b) { return a + b; }
来源：http://luh.yfazqb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://eco.ivvv.top

Java: static int add(int a, int b) { return a + b; }
来源：http://vcj.smart0.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://bqr.xuetiantiany.cn

Ruby: def add(a, b); a + b; end
来源：http://oxm.yuxming.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dvx.yangfankeji.com

[C02] 默认参数
来源：http://tjv.yonumen.top

Py:   def greet(name="World"): return name
来源：http://qcy.316326.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://mik.jinyuanbaomall.cn

JS:   function greet(name = "World") { return name; }
来源：http://soe.tarul.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://uts.xuanzx.com

Java: // 无默认参数：方法重载或 Optional
来源：http://afy.iojbl.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gpk.meibo888.top

Ruby: def greet(name = "World") = name
来源：http://vzv.zhengqikj.top

C#:   string Greet(string name = "World") => name;
来源：http://nkr.jqgfzy.top

[C03] 可变参数
来源：http://jdd.yuanzhike.top

Py:   def total(*args): return sum(args)
来源：http://ztq.tanke756.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qtq.ehwqpu.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bcg.yj20258888.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zoh.fktsv.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fov.sxryk.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://aja.quarkkingdee.top

Ruby: def total(*nums); nums.sum; end
来源：http://pxf.yangfankeji.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dgu.redwolf501.top

[C04] 命名参数 / 关键字参数
来源：http://uhb.daxiang520.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wbu.jinghuilouyu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jsw.jlsjyb.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://aqi.hysaishi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nzv.chenzaomai.com

Java: // 无：用 Builder 模式或 record
来源：http://oty.zhijiandao.cn

Go:   // 无：用配置结构体参数
来源：http://gxz.ydjk.org.cn

Ruby: f(a: 1, b: 2)
来源：http://uzy.zhoulong.xyz

C#:   f(a: 1, b: 2)
来源：http://oqo.hongshengwenyu.top

[C05] 返回多个值
来源：http://lul.hesvh.cn

Py:   return a, b
来源：http://ogx.hnxiangtu.top

PHP:  return [$a, $b];
来源：http://mam.nanxuanxn.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://bph.gzhubu.top

TS:   return { a, b };
来源：http://ytq.quarkkingdee.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://twm.nanxinkj.top

Go:   return a, b
来源：http://ule.yj20258.top

Ruby: return a, b
来源：http://pcb.c1oappe.top

C#:   return (a, b);              // ValueTuple
来源：http://fmb.guowangkeji.top

[C06] 匿名函数 / lambda
来源：http://yvq.wangshuangyany.cn

Py:   square = lambda x: x * x
来源：http://dpg.ybcxt.top

PHP:  $square = fn($x) => $x * $x;
来源：http://fmo.sysykeji.top

JS:   const square = x => x * x;
来源：http://ckm.ctjpmb.com

TS:   const square = (x: number): number => x * x;
来源：http://ccp.shuidangran.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hjk.ctjpmb.com

Go:   sq := func(x int) int { return x * x }
来源：http://vfn.zhixingplan.top

Ruby: square = ->(x) { x * x }
来源：http://gef.zhengqikj.top

C#:   Func<int, int> square = x => x * x;
来源：http://dms.52xcode.cn

[C07] 把函数作为参数传入
来源：http://bfb.xziqi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lki.gogol.net.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hmv.yuanzhike.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ags.yanxiufei.cn

TS:   arr.map(String)
来源：http://pem.yangfankeji.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lrm.meibo888.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://und.jianghu66.top

Ruby: arr.map(&:upcase)
来源：http://feh.vqdsnc.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wfz.havefunace.top

[C08] 闭包
来源：http://vkq.fanxiaobao.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://aza.smart0.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cjt.shanyushiyangkeji.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ctw.mhx1999.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dlt.guowangkeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hho.gzhubu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dom.meibo888.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mxu.hfpthk.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mbp.hnqzz.top

[C09] 递归
来源：http://gob.sweek.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ajo.ywan-chungtsiang.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pvn.uphjek.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hge.yueranfly.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uux.yj202588.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://iod.zhaomingkeji.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gxd.tanke756.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lso.sxryk.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ynp.ydzc1.top

[C10] 变量作用域
来源：http://sxt.feifeiyinyue.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wck.yuanzhike.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jwb.cheryme.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://stq.nanxinkj.top

TS:   同 JS
来源：http://hor.hongshengwenyu.top

Java: 方法内为块级作用域
来源：http://hqd.havefunace.top

Go:   花括号块级作用域
来源：http://aug.hcnkem.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://juq.cashguo.top

C#:   块级作用域
来源：http://lgx.dianchejie.cn

[C11] 模块导入与导出
来源：http://edo.cqqwz.cn

Py:   from module import func
来源：http://hib.yuanzhike.top

PHP:  require "file.php";  或 use App\Service;
来源：http://neu.c1oappe.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://pyz.wangdashe.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://efp.uphjek.com

Java: import java.util.List;
来源：http://hgv.aibaodan.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gli.gotoacloud.top

Ruby: require "json"; require_relative "./util"
来源：http://ibn.hnqzz.top

C#:   using System.Text;
来源：http://uga.chenlongwang.top

[C12] 立即执行函数 IIFE
来源：http://fep.yangfankeji.com

Py:   (lambda: print("run"))()
来源：http://eqd.xingfuxueyuan.xyz

PHP:  (function () { echo "run"; })();
来源：http://orc.ybcxt.top

JS:   (() => { console.log("run"); })();
来源：http://bgq.nanxuanxn.top

TS:   (() => { console.log("run"); })();
来源：http://haw.jinghuilouyu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dtw.gotoacloud.top

Go:   func() { fmt.Println("run") }()
来源：http://okd.jiagoushi.top

Ruby: -> { puts "run" }.call
来源：http://szy.hongshengwenyu.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ngf.xinyue.icu

[C13] 类型声明 / 类型注解
来源：http://jeq.ybcxt.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bss.smart0.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vzi.epnwcf.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xog.yj20258.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zod.aizwys.cn

Java: int add(int a, int b) { return a + b; }
来源：http://nus.xinyue.icu

Go:   func add(a, b int) int
来源：http://chp.tian-w.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qwi.ctjpmb.com

C#:   int Add(int a, int b) => a + b;
来源：http://xuf.chenzaomai.com

[C14] 泛型函数
来源：http://lnn.smart0.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kde.gaohongyu789.top

PHP:  // 无泛型
来源：http://nul.xziqi.cn

JS:   // 无泛型
来源：http://bag.epnwcf.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tfu.yuxming.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xtq.aizwys.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dif.cucudq.cn

Ruby: # 无泛型
来源：http://nzv.zdbjq.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gwv.pengpengdd.cyou

[C15] 解构 / 展开参数
来源：http://msx.yueranfly.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ekx.jiagoushi.top

PHP:  [$a, $b] = $pair;
来源：http://oqk.nwbrower.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://okt.xuanzx.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://obz.havefunace.top

Java: // 无解构
来源：http://owc.mhx1999.top

Go:   // 无解构
来源：http://iel.zhoulong.xyz

Ruby: a, b = pair
来源：http://hae.tian-w.cn

C#:   var (a, b) = pair;
来源：http://bae.ppjwa.cn

[C16] 函数 / 方法重载
来源：http://meq.daxiang520.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bsn.tian-w.cn

PHP:  // 无重载
来源：http://wys.daxiang520.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://qsm.sweek.top

TS:   // 用联合类型或重载签名声明
来源：http://akx.yangfankeji.com

Java: void f(int a) {}  void f(String a) {}
来源：http://pfx.yvedp.cn

Go:   // 无重载：用不同函数名
来源：http://wnt.jinqigufen.top

Ruby: # 无重载：靠动态参数
来源：http://irn.jinghuilouyu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://sqh.gzhubu.top

================================================================================
来源：http://oyx.andypj.xyz

D. 数组 / 列表 / 集合
来源：http://vys.52xcode.cn

================================================================================
来源：http://hoo.tianlin.xyz

[D01] 创建数组 / 列表
来源：http://sid.cqqwz.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qru.ppjwa.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://djk.yj20258.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pjl.ctjpmb.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://qjn.gotoacloud.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qcp.xingfuxueyuan.xyz

Go:   arr := []int{1, 2, 3}
来源：http://nku.xingfuxueyuan.xyz

Ruby: arr = [1, 2, 3]
来源：http://jdq.jyoumei.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jph.zhiwuduotai.top

[D02] 追加元素到末尾
来源：http://axo.jqgufenzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wqn.vehdjk.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wtd.jinqigfzy.top

JS:   arr.push(4);
来源：http://nls.jianghu66.top

TS:   arr.push(4);
来源：http://dyb.jinqigfzy.top

Java: list.add(4);
来源：http://ktg.iojbl.cn

Go:   arr = append(arr, 4)
来源：http://gty.pengpengdd.cyou

Ruby: arr << 4; arr.push(5)
来源：http://cdh.gotoacloud.top

C#:   list.Add(4);
来源：http://bwq.ehwqpu.com

[D03] 在指定位置插入元素
来源：http://cwl.yvedp.cn

Py:   arr.insert(0, 0)
来源：http://xxv.gzhubu.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://flv.yongpay.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://guh.uphjek.com

TS:   arr.splice(0, 0, 0);
来源：http://pkk.zhongyouzk.top

Java: list.add(0, 0);
来源：http://qcq.hnqzz.top

Go:   arr = append([]int{0}, arr...)
来源：http://izb.fktsv.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dev.shzxlz.cn

C#:   list.Insert(0, 0);
来源：http://zfm.andypj.xyz

[D04] 删除元素
来源：http://kkn.cqqwz.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qxb.zhixingplan.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cvs.bbcook.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wrg.zhijiandao.cn

TS:   arr.splice(0, 1);
来源：http://twd.iojbl.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bpu.c1oappe.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xkz.ehwqpu.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cqg.jinyuanbaomall.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://oan.xuetiantiany.cn

[D05] 访问与修改元素
来源：http://qsw.yuxming.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vqw.yonumen.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://opt.daria6918.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jay.epnwcf.com

TS:   arr[0]; arr.at(-1);
来源：http://kej.hammf.cn

Java: list.get(0); list.set(0, 9);
来源：http://jpj.smart0.xyz

Go:   arr[0]; arr[0] = 9
来源：http://yav.guowangkeji.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bik.bjfxy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vve.fehbvm.com

[D06] 数组长度
来源：http://kqy.jqgfzy.top

Py:   len(arr)
来源：http://iew.yanxiufei.cn

PHP:  count($arr);
来源：http://bjm.dashuyun.cn

JS:   arr.length
来源：http://bga.bbcook.cn

TS:   arr.length
来源：http://gwp.gzhubu.top

Java: list.size();
来源：http://shf.aizwys.cn

Go:   len(arr)
来源：http://bim.zhixingplan.top

Ruby: arr.length; arr.size
来源：http://ncw.zhoulong.xyz

C#:   list.Count;
来源：http://uyk.fehbvm.com

[D07] 切片 / 取子数组
来源：http://fut.yangfankeji.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://neq.zhijiandao.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jia.zhoulong.xyz

JS:   arr.slice(1, 4);
来源：http://cbi.vehdjk.com

TS:   arr.slice(1, 4);
来源：http://sak.aizwys.cn

Java: list.subList(1, 4);
来源：http://vkd.tian-w.cn

Go:   arr[1:4]
来源：http://klh.hcnkem.com

Ruby: arr[1, 3]
来源：http://ttu.svipenyu.cn

C#:   list.GetRange(1, 3);
来源：http://hae.daria6918.cn

[D08] 合并两个数组
来源：http://qmj.cdnleiting.top

Py:   a + b;  a.extend(b)
来源：http://php.jianghu66.top

PHP:  array_merge($a, $b);
来源：http://bkp.jinghuilouyu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ggc.yj202588.top

TS:   [...a, ...b];
来源：http://awm.9152youxi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://maw.zycfv.cn

Go:   append(a, b...)
来源：http://fhm.yongpay.top

Ruby: a + b;  a.concat(b)
来源：http://xzh.hnxiangtu.top

C#:   a.Concat(b).ToList()
来源：http://frf.jinqigufen.top

[D09] 排序（升序）
来源：http://nbz.hammf.cn

Py:   sorted(arr);  arr.sort()
来源：http://pda.hnqzz.top

PHP:  sort($arr);
来源：http://hiv.shanyushiyangtech.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fzs.feifeiyinyue.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://efw.shanyushiyangkeji.top

Java: Collections.sort(list);  list.sort(null);
来源：http://bhx.ppjwa.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lls.zdqjudy.top

Ruby: arr.sort
来源：http://vsf.hnxiangtu.top

C#:   list.Sort();
来源：http://klg.pengpengdd.cyou

[D10] 自定义排序（按字段 / 多条件）
来源：http://prs.xylfe.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dpr.birdmap.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xyk.316326.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ipy.hcnkem.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://drp.tian-w.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fdq.aizwys.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bnn.jiagoushi.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zxh.andypj.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tvw.aibaodan.cn

[D11] 反转数组
来源：http://nbx.zhixingplan.top

Py:   arr[::-1];  arr.reverse()
来源：http://gug.zdbjq.cn

PHP:  array_reverse($arr);
来源：http://sjs.yanxiufei.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lwj.sufxvd.cn

TS:   [...arr].reverse();
来源：http://bxv.vqdsnc.cn

Java: Collections.reverse(list);
来源：http://ero.jyoumei.cn

Go:   slices.Reverse(arr)
来源：http://cjb.xuetiantiany.cn

Ruby: arr.reverse
来源：http://baa.shangyingyoupin.top

C#:   list.Reverse();
来源：http://ogi.zdqjudy.top

[D12] 查找元素下标
来源：http://ttm.chenzaomai.com

Py:   arr.index(x);  x in arr
来源：http://zon.jiagoushi.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dcl.chenzaomai.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yjr.xuanzx.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rlw.yuanzhike.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hsy.tarul.cn

Go:   slices.Index(arr, x)
来源：http://avw.fehbvm.com

Ruby: arr.index(x)
来源：http://djv.bjfxy.top

C#:   list.IndexOf(x);
来源：http://dih.hysaishi.cn

[D13] 过滤（保留满足条件的）
来源：http://xte.gaohongyu789.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lvq.redwolf501.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ddt.jqgfzy.top

JS:   arr.filter(x => x > 3)
来源：http://rlr.zhiwuduotai.top

TS:   arr.filter(x => x > 3)
来源：http://loe.xuetiantiany.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://afs.shanyushiyangtech.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rfg.ehwqpu.com

Ruby: arr.select { |x| x > 3 }
来源：http://ros.shzxlz.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://tej.yongpay.top

[D14] 映射转换（每个元素变形）
来源：http://elu.smart0.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://eho.gogol.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ebm.yueranfly.top

JS:   arr.map(x => x * 2)
来源：http://rlb.kuanghao11.cn

TS:   arr.map(x => x * 2)
来源：http://dhy.yfazqb.com


<!-- 参考信息 -->
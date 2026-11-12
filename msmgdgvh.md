代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cmp.hnxiangtu.top

Ruby: (0...10).step(2).to_a
来源：http://qbg.zdqjudy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vbz.yonumen.top

[B12] 跳出多层循环
来源：http://vvw.hysaishi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://uwl.yanxiufei.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://avf.gotoacloud.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zei.xylfe.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dhf.gzhubu.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ans.smart0.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wez.xziqi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mte.xuetiantiany.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rih.hnqzz.top

[B13] 判断是否为数字
来源：http://svm.yueranfly.top

Py:   isinstance(x, (int, float))
来源：http://aop.cheryme.top

PHP:  is_numeric($x)
来源：http://qrk.mhx1999.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vah.ctjpmb.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://why.fengsongda.top

Java: x instanceof Number
来源：http://pzp.jqgufenzy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vfr.fktsv.cn

Ruby: x.is_a?(Numeric)
来源：http://ezl.kuanghao11.cn

C#:   x is int or double or decimal
来源：http://kfn.shzxlz.cn

[B14] 判断值是否在集合内
来源：http://njb.pengpengdd.cyou

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qoj.havefunace.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vzw.nwbrower.top

JS:   [1, 2, 3].includes(x)
来源：http://obk.daxiang520.top

TS:   [1, 2, 3].includes(x)
来源：http://lye.jinqigufen.top

Java: List.of(1, 2, 3).contains(x)
来源：http://jpn.ivvv.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wxu.hnxiangtu.top

Ruby: [1, 2, 3].include?(x)
来源：http://jhm.zhoulong.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://phf.316326.xyz

[B15] 布尔运算与取反
来源：http://fep.dianchejie.cn

Py:   a and b or not c
来源：http://unx.ehwqpu.com

PHP:  $a && $b || !$c
来源：http://fmd.yvedp.cn

JS:   a && b || !c
来源：http://xlr.sxryk.cn

TS:   a && b || !c
来源：http://izp.ydjk.org.cn

Java: a && b || !c
来源：http://xka.yanxiufei.cn

Go:   a && b || !c
来源：http://veh.pycfn.com

Ruby: a && b || !c
来源：http://aoo.9152youxi.cn

C#:   a && b || !c
来源：http://ibe.yfazqb.com

[B16] 卫语句：不满足条件提前返回
来源：http://fyd.gotoacloud.top

Py:   if not data: return
来源：http://hha.hysaishi.cn

PHP:  if (!$data) { return; }
来源：http://mxn.quarkkingdee.top

JS:   if (!data) return;
来源：http://lce.chenjidiqi.icu

TS:   if (!data) return;
来源：http://tkf.zhiwuduotai.top

Java: if (data == null) return;
来源：http://mlb.iojbl.cn

Go:   if data == nil { return }
来源：http://mcw.zhengqikj.top

Ruby: return if data.nil?
来源：http://nqw.daxiang520.top

C#:   if (data == null) return;
来源：http://ddy.52xcode.cn

================================================================================
来源：http://cgj.sjlbkw.cn

C. 函数与作用域
来源：http://noh.vqdsnc.cn

================================================================================
来源：http://eeb.cdnleiting.top

[C01] 定义函数
来源：http://ybe.daria6918.cn

Py:   def add(a, b): return a + b
来源：http://wkg.yj20258888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qaj.shzxlz.cn

JS:   function add(a, b) { return a + b; }
来源：http://kib.xuetiantiany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://llh.zhixingplan.top

Java: static int add(int a, int b) { return a + b; }
来源：http://qgd.jyoumei.cn

Go:   func add(a, b int) int { return a + b }
来源：http://tpu.uphjek.com

Ruby: def add(a, b); a + b; end
来源：http://zzk.vqdsnc.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qih.yuanzhike.top

[C02] 默认参数
来源：http://mxk.jinqigfzy.top

Py:   def greet(name="World"): return name
来源：http://dul.svipenyu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qir.yuxming.cn

JS:   function greet(name = "World") { return name; }
来源：http://xuf.dashuyun.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cql.nwbrower.top

Java: // 无默认参数：方法重载或 Optional
来源：http://pue.jinqigufen.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xif.sweek.top

Ruby: def greet(name = "World") = name
来源：http://bpz.xziqi.cn

C#:   string Greet(string name = "World") => name;
来源：http://nin.yanxiufei.cn

[C03] 可变参数
来源：http://omn.ivvv.top

Py:   def total(*args): return sum(args)
来源：http://yvd.mhx1999.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cpd.shanyushiyangtech.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ulr.zdqjudy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ebm.yueranfly.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yyz.yuxming.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xwu.tian-w.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zvv.iojbl.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://syj.fzhhl.top

[C04] 命名参数 / 关键字参数
来源：http://pya.c1oappe.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ppo.jiagoushi.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tes.hywenlv.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ocr.sjlbkw.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://var.bjfxy.top

Java: // 无：用 Builder 模式或 record
来源：http://bro.hnqzz.top

Go:   // 无：用配置结构体参数
来源：http://jxe.yongpay.top

Ruby: f(a: 1, b: 2)
来源：http://wgx.yongpay.top

C#:   f(a: 1, b: 2)
来源：http://rjz.shangyingyoupin.top

[C05] 返回多个值
来源：http://txh.shangyingyoupin.top

Py:   return a, b
来源：http://qhh.jlsjyb.cn

PHP:  return [$a, $b];
来源：http://ulz.pengpengdd.cyou

JS:   return [a, b];             // 或 return { a, b };
来源：http://bql.iojbl.cn

TS:   return { a, b };
来源：http://lci.smart0.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ywf.bjfxy.top

Go:   return a, b
来源：http://uux.yuanzhike.top

Ruby: return a, b
来源：http://wdf.gaohongyu789.top

C#:   return (a, b);              // ValueTuple
来源：http://gob.kuanghao11.cn

[C06] 匿名函数 / lambda
来源：http://ylu.jinqigfzy.top

Py:   square = lambda x: x * x
来源：http://zyw.fanxiaobao.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://jps.shanyushiyangkeji.top

JS:   const square = x => x * x;
来源：http://ivp.fktsv.cn

TS:   const square = (x: number): number => x * x;
来源：http://lwh.zycfv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jlk.tian-w.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ujl.jiagoushi.top

Ruby: square = ->(x) { x * x }
来源：http://cgr.jinyuanbaomall.cn

C#:   Func<int, int> square = x => x * x;
来源：http://lgd.smart0.xyz

[C07] 把函数作为参数传入
来源：http://nmq.jinqigufen.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xlb.hnqzz.top

PHP:  array_map("strtoupper", $arr);
来源：http://yrm.nanxuanxn.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wth.sufxvd.cn

TS:   arr.map(String)
来源：http://iud.xinyue.icu

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yyj.sysykeji.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://upy.yonumen.top

Ruby: arr.map(&:upcase)
来源：http://ega.shuidangran.top

C#:   arr.Select(s => s.ToUpper())
来源：http://bde.yanxiufei.cn

[C08] 闭包
来源：http://nkj.epnwcf.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zml.xuetiantiany.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qyn.andypj.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qam.316326.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blc.bbcook.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jas.jqgfzy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tro.chenlongwang.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vnf.wangshuangyany.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bmy.fanxiaobao.xyz

[C09] 递归
来源：http://yas.ivvv.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fto.cdnleiting.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://iuz.shanyushiyangtech.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mgb.wangdashe.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eux.sxryk.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://azg.52xcode.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rny.redwolf501.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gmo.hfpthk.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fek.vqdsnc.cn

[C10] 变量作用域
来源：http://jsy.tanke756.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vqq.cashguo.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nqv.sweek.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bwh.hnqzz.top

TS:   同 JS
来源：http://ljo.zdbjq.cn

Java: 方法内为块级作用域
来源：http://zqz.dashuyun.cn

Go:   花括号块级作用域
来源：http://rsm.andypj.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wpw.hysaishi.cn

C#:   块级作用域
来源：http://vdt.hnxiangtu.top

[C11] 模块导入与导出
来源：http://ipn.yanxiufei.cn

Py:   from module import func
来源：http://qwf.wangshuangyany.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://gir.chenjidiqi.icu

JS:   export default function f() {};  import f from "./m.js";
来源：http://dpk.nwbrower.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lta.ywan-chungtsiang.top

Java: import java.util.List;
来源：http://rms.sjlbkw.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kci.jianghu66.top

Ruby: require "json"; require_relative "./util"
来源：http://klc.zdbjq.cn

C#:   using System.Text;
来源：http://gns.aibaodan.cn

[C12] 立即执行函数 IIFE
来源：http://dmx.aizwys.cn

Py:   (lambda: print("run"))()
来源：http://isv.zhaomingkeji.xyz

PHP:  (function () { echo "run"; })();
来源：http://edu.birdmap.top

JS:   (() => { console.log("run"); })();
来源：http://swp.yuxming.cn

TS:   (() => { console.log("run"); })();
来源：http://sgp.ywan-chungtsiang.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wnm.hysaishi.cn

Go:   func() { fmt.Println("run") }()
来源：http://uer.gaohongyu789.top

Ruby: -> { puts "run" }.call
来源：http://gks.yvedp.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ftw.tian-w.cn

[C13] 类型声明 / 类型注解
来源：http://lxp.shangyingyoupin.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://atk.wangshuangyany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qjg.nanxinkj.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pdp.yvedp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://svl.feifeiyinyue.top

Java: int add(int a, int b) { return a + b; }
来源：http://zvs.mhx1999.top

Go:   func add(a, b int) int
来源：http://hje.zhoulong.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tyi.wangdashe.top

C#:   int Add(int a, int b) => a + b;
来源：http://yys.pengpengdd.cyou

[C14] 泛型函数
来源：http://hbj.fktsv.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ipb.redwolf501.top

PHP:  // 无泛型
来源：http://oqn.0kj1m.cn

JS:   // 无泛型
来源：http://nut.jianghu66.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wlw.mhx1999.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://aaq.snrcjt.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nww.fehbvm.com

Ruby: # 无泛型
来源：http://ifb.dianchejie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xvv.9152youxi.cn

[C15] 解构 / 展开参数
来源：http://fqi.yongpay.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gfl.zhiwuduotai.top

PHP:  [$a, $b] = $pair;
来源：http://kht.tianlin.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://esr.jqgfzy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ian.uphjek.com

Java: // 无解构
来源：http://hzj.meibo888.top

Go:   // 无解构
来源：http://xhq.zhijiandao.cn

Ruby: a, b = pair
来源：http://tvf.xingfuxueyuan.xyz

C#:   var (a, b) = pair;
来源：http://qki.meibo888.top

[C16] 函数 / 方法重载
来源：http://umv.fanxiaobao.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://irq.52xcode.cn

PHP:  // 无重载
来源：http://jst.yangfankeji.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://oec.wangdashe.top

TS:   // 用联合类型或重载签名声明
来源：http://gbu.hesvh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://shh.cucudq.cn

Go:   // 无重载：用不同函数名
来源：http://dye.bjfxy.top

Ruby: # 无重载：靠动态参数
来源：http://xjc.vqdsnc.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://umj.sweek.top

================================================================================
来源：http://jcd.nanxuanxn.top

D. 数组 / 列表 / 集合
来源：http://elh.jqgufenzy.top

================================================================================
来源：http://zdt.yj202588.top

[D01] 创建数组 / 列表
来源：http://glj.shangyingyoupin.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://mgm.yj20258.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zvw.bjfxy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sdu.fehbvm.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://qzg.hfpthk.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pjg.ywan-chungtsiang.top

Go:   arr := []int{1, 2, 3}
来源：http://mmo.jyoumei.cn

Ruby: arr = [1, 2, 3]
来源：http://ern.shanyushiyangkeji.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ath.zhiwuduotai.top

[D02] 追加元素到末尾
来源：http://njg.bjfxy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fev.redwolf501.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jij.tarul.cn

JS:   arr.push(4);
来源：http://xyh.nwbrower.top

TS:   arr.push(4);
来源：http://jrn.ydjk.org.cn

Java: list.add(4);
来源：http://ovh.bbcook.cn

Go:   arr = append(arr, 4)
来源：http://qvw.vqdsnc.cn

Ruby: arr << 4; arr.push(5)
来源：http://oqc.gogol.net.cn

C#:   list.Add(4);
来源：http://grs.xuanzx.com

[D03] 在指定位置插入元素
来源：http://leb.sjlbkw.cn

Py:   arr.insert(0, 0)
来源：http://qmn.aibaodan.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wlc.gaohongyu789.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ptc.daria6918.cn

TS:   arr.splice(0, 0, 0);
来源：http://ltz.sjlbkw.cn

Java: list.add(0, 0);
来源：http://oxw.chenlongwang.top

Go:   arr = append([]int{0}, arr...)
来源：http://zxk.gzhubu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://oiq.uphjek.com

C#:   list.Insert(0, 0);
来源：http://fgy.zdqjudy.top

[D04] 删除元素
来源：http://llv.meibo888.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xou.birdmap.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fov.yongpay.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gqz.meibo888.top

TS:   arr.splice(0, 1);
来源：http://uuj.ywan-chungtsiang.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://whl.feifeiyinyue.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lfs.daxiang520.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://maf.ydjk.org.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://chw.zhijiandao.cn

[D05] 访问与修改元素
来源：http://nnv.316326.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xav.fzhhl.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://emy.hnxiangtu.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fxw.zycfv.cn

TS:   arr[0]; arr.at(-1);
来源：http://plv.sysykeji.top

Java: list.get(0); list.set(0, 9);
来源：http://kyv.chenjidiqi.icu

Go:   arr[0]; arr[0] = 9
来源：http://nni.yuxming.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kmc.haohaochexian.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vdn.zycfv.cn

[D06] 数组长度
来源：http://obk.andypj.xyz

Py:   len(arr)
来源：http://fyb.hammf.cn

PHP:  count($arr);
来源：http://fhp.quarkkingdee.top

JS:   arr.length
来源：http://grq.quarkkingdee.top

TS:   arr.length
来源：http://hte.snrcjt.cn

Java: list.size();
来源：http://nzm.iojbl.cn

Go:   len(arr)
来源：http://drc.nwbrower.top

Ruby: arr.length; arr.size
来源：http://sgz.zhixingplan.top

C#:   list.Count;
来源：http://vsd.hnqzz.top

[D07] 切片 / 取子数组
来源：http://bel.wangshuangyany.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://muf.9152youxi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://dkb.bbcook.cn

JS:   arr.slice(1, 4);
来源：http://dci.fktsv.cn

TS:   arr.slice(1, 4);
来源：http://nig.yuxming.cn

Java: list.subList(1, 4);
来源：http://loa.vqdsnc.cn

Go:   arr[1:4]
来源：http://ili.yvedp.cn

Ruby: arr[1, 3]
来源：http://urr.andypj.xyz

C#:   list.GetRange(1, 3);
来源：http://hkg.shangyingyoupin.top

[D08] 合并两个数组
来源：http://dxv.sufxvd.cn

Py:   a + b;  a.extend(b)
来源：http://hjb.zycfv.cn

PHP:  array_merge($a, $b);
来源：http://uec.shzxlz.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hml.xylfe.cn

TS:   [...a, ...b];
来源：http://qzj.ybcxt.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pkw.daxiang520.top

Go:   append(a, b...)
来源：http://qxi.cqqwz.cn

Ruby: a + b;  a.concat(b)
来源：http://ayn.gotoacloud.top

C#:   a.Concat(b).ToList()
来源：http://igs.jinyuanbaomall.cn

[D09] 排序（升序）
来源：http://chd.hnqzz.top

Py:   sorted(arr);  arr.sort()
来源：http://lzz.dianchejie.cn

PHP:  sort($arr);
来源：http://qxt.ybcxt.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tyv.ydjk.org.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wfo.hnxiangtu.top

Java: Collections.sort(list);  list.sort(null);
来源：http://bbg.tanke756.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mwv.shuidangran.top

Ruby: arr.sort
来源：http://aoq.hfpthk.cn

C#:   list.Sort();
来源：http://aju.tian-w.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fbw.daria6918.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zar.zhoulong.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tan.chenzaomai.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gbn.hysaishi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://onw.yueranfly.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kjx.pycfn.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uqs.0kj1m.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pbh.wangdashe.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xal.daria6918.cn

[D11] 反转数组
来源：http://voa.tianlin.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://lax.guannengcc.top

PHP:  array_reverse($arr);
来源：http://djv.epnwcf.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://htd.shanyushiyangtech.top

TS:   [...arr].reverse();
来源：http://yfc.0kj1m.cn

Java: Collections.reverse(list);
来源：http://yan.pengpengdd.cyou

Go:   slices.Reverse(arr)
来源：http://nvx.aizwys.cn

Ruby: arr.reverse
来源：http://pui.zycfv.cn

C#:   list.Reverse();
来源：http://dtu.nanxinkj.top

[D12] 查找元素下标
来源：http://brk.ydzc1.top

Py:   arr.index(x);  x in arr
来源：http://hzo.jlsjyb.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jci.cashguo.top


<!-- 参考信息 -->
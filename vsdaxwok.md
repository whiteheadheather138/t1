代发 wailian999

PHP:  $a && $b || !$c
来源：http://lea.hnqzz.top

JS:   a && b || !c
来源：http://fvc.dianchejie.cn

TS:   a && b || !c
来源：http://mqs.fanxiaobao.xyz

Java: a && b || !c
来源：http://mtz.fktsv.cn

Go:   a && b || !c
来源：http://ydd.hnxiangtu.top

Ruby: a && b || !c
来源：http://sau.xingfuxueyuan.xyz

C#:   a && b || !c
来源：http://hon.jinyuanbaomall.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ytn.tianlin.xyz

Py:   if not data: return
来源：http://lid.tianlin.xyz

PHP:  if (!$data) { return; }
来源：http://xed.feifeiyinyue.top

JS:   if (!data) return;
来源：http://lxu.jinghuilouyu.cn

TS:   if (!data) return;
来源：http://qcw.aizwys.cn

Java: if (data == null) return;
来源：http://ypw.gotoacloud.top

Go:   if data == nil { return }
来源：http://dxl.daria6918.cn

Ruby: return if data.nil?
来源：http://vou.zhoulong.xyz

C#:   if (data == null) return;
来源：http://fcd.zdbjq.cn

================================================================================
来源：http://ptc.havefunace.top

C. 函数与作用域
来源：http://gnm.jinqigfzy.top

================================================================================
来源：http://ubx.tarul.cn

[C01] 定义函数
来源：http://zjv.havefunace.top

Py:   def add(a, b): return a + b
来源：http://ban.havefunace.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jlb.chenlongwang.top

JS:   function add(a, b) { return a + b; }
来源：http://mth.xylfe.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kkt.birdmap.top

Java: static int add(int a, int b) { return a + b; }
来源：http://won.jqgufenzy.top

Go:   func add(a, b int) int { return a + b }
来源：http://trv.fanxiaobao.xyz

Ruby: def add(a, b); a + b; end
来源：http://qiy.jqgufenzy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dzx.xinyue.icu

[C02] 默认参数
来源：http://zgx.yj20258.top

Py:   def greet(name="World"): return name
来源：http://qeo.tianlin.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://vlw.chenzaomai.com

JS:   function greet(name = "World") { return name; }
来源：http://tys.pengpengdd.cyou

TS:   function greet(name: string = "World") { return name; }
来源：http://ghs.uphjek.com

Java: // 无默认参数：方法重载或 Optional
来源：http://fcp.sufxvd.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lpc.hywenlv.cn

Ruby: def greet(name = "World") = name
来源：http://xbg.jiagoushi.top

C#:   string Greet(string name = "World") => name;
来源：http://wpe.xylfe.cn

[C03] 可变参数
来源：http://hxt.aibaodan.cn

Py:   def total(*args): return sum(args)
来源：http://qgd.hnqzz.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rjp.52xcode.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://piy.sjlbkw.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://biy.jiagoushi.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wlq.haohaochexian.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://udn.tian-w.cn

Ruby: def total(*nums); nums.sum; end
来源：http://nvy.uphjek.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zpa.ydzc1.top

[C04] 命名参数 / 关键字参数
来源：http://qqk.iojbl.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xas.guowangkeji.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mls.guowangkeji.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sjv.hnqzz.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cpb.zhiwuduotai.top

Java: // 无：用 Builder 模式或 record
来源：http://jfp.cdnleiting.top

Go:   // 无：用配置结构体参数
来源：http://sex.smart0.xyz

Ruby: f(a: 1, b: 2)
来源：http://hzf.316326.xyz

C#:   f(a: 1, b: 2)
来源：http://xbw.sweek.top

[C05] 返回多个值
来源：http://lhq.cdnleiting.top

Py:   return a, b
来源：http://ihz.nanxinkj.top

PHP:  return [$a, $b];
来源：http://wrh.zdbjq.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zlm.c1oappe.top

TS:   return { a, b };
来源：http://amz.aibaodan.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gcv.gogol.net.cn

Go:   return a, b
来源：http://jhw.jiagoushi.top

Ruby: return a, b
来源：http://fex.gaohongyu789.top

C#:   return (a, b);              // ValueTuple
来源：http://ixw.c1oappe.top

[C06] 匿名函数 / lambda
来源：http://nuv.dianchejie.cn

Py:   square = lambda x: x * x
来源：http://ibm.hongshengwenyu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://utc.fzhhl.top

JS:   const square = x => x * x;
来源：http://per.zdbjq.cn

TS:   const square = (x: number): number => x * x;
来源：http://qmi.uphjek.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://veh.zhoulong.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://uae.ctjpmb.com

Ruby: square = ->(x) { x * x }
来源：http://vhn.cashguo.top

C#:   Func<int, int> square = x => x * x;
来源：http://ole.yongpay.top

[C07] 把函数作为参数传入
来源：http://pra.bbcook.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://aoj.yonumen.top

PHP:  array_map("strtoupper", $arr);
来源：http://pjr.zdqjudy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ecy.gzhubu.top

TS:   arr.map(String)
来源：http://gkh.ctjpmb.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jul.dianchejie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lfp.yj20258888.top

Ruby: arr.map(&:upcase)
来源：http://omz.aibaodan.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://uni.xinyue.icu

[C08] 闭包
来源：http://dva.jinghuilouyu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uxy.zycfv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://god.yanxiufei.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://srh.wangdashe.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qlo.hongshengwenyu.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xez.fzhhl.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zvo.yonumen.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jrt.jlsjyb.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rbu.dianchejie.cn

[C09] 递归
来源：http://jsr.nwbrower.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yyo.zhoulong.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tol.yvedp.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ruf.bbcook.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fje.dashuyun.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zqj.yj202588.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ebq.xuanzx.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://avn.daria6918.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ssa.hnxiangtu.top

[C10] 变量作用域
来源：http://dui.jinqigfzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mxz.zhongyouzk.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://coa.yonumen.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kct.zhixingplan.top

TS:   同 JS
来源：http://fsl.iojbl.cn

Java: 方法内为块级作用域
来源：http://xrj.sweek.top

Go:   花括号块级作用域
来源：http://chd.hongshengwenyu.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ngi.chenjidiqi.icu

C#:   块级作用域
来源：http://kpq.meibo888.top

[C11] 模块导入与导出
来源：http://pvy.bjfxy.top

Py:   from module import func
来源：http://ahw.nanxuanxn.top

PHP:  require "file.php";  或 use App\Service;
来源：http://qec.guowangkeji.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://xla.sweek.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zin.ivvv.top

Java: import java.util.List;
来源：http://zdl.uphjek.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tch.sweek.top

Ruby: require "json"; require_relative "./util"
来源：http://yoy.daxiang520.top

C#:   using System.Text;
来源：http://alh.jqgfzy.top

[C12] 立即执行函数 IIFE
来源：http://ujj.yuxming.cn

Py:   (lambda: print("run"))()
来源：http://kqo.chenjidiqi.icu

PHP:  (function () { echo "run"; })();
来源：http://dkv.ybcxt.top

JS:   (() => { console.log("run"); })();
来源：http://lcm.ywan-chungtsiang.top

TS:   (() => { console.log("run"); })();
来源：http://kys.daxiang520.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pif.bbcook.cn

Go:   func() { fmt.Println("run") }()
来源：http://eqh.ydjk.org.cn

Ruby: -> { puts "run" }.call
来源：http://hzl.aizwys.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mox.zhoulong.xyz

[C13] 类型声明 / 类型注解
来源：http://alk.mhx1999.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ela.zhengqikj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zhi.yj20258888.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ewu.kuanghao11.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hmp.zhaomingkeji.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://xym.sjlbkw.cn

Go:   func add(a, b int) int
来源：http://rvr.nanxinkj.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wwx.yangfankeji.com

C#:   int Add(int a, int b) => a + b;
来源：http://khb.fehbvm.com

[C14] 泛型函数
来源：http://xfb.9152youxi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wmq.sysykeji.top

PHP:  // 无泛型
来源：http://lab.ppjwa.cn

JS:   // 无泛型
来源：http://ybn.chenzaomai.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uwl.yanxiufei.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://egl.zdbjq.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://khp.wangshuangyany.cn

Ruby: # 无泛型
来源：http://lvy.xylfe.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yce.shanyushiyangtech.top

[C15] 解构 / 展开参数
来源：http://tco.snrcjt.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rye.zhixingplan.top

PHP:  [$a, $b] = $pair;
来源：http://lez.xziqi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gsm.ehwqpu.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fdc.yangfankeji.com

Java: // 无解构
来源：http://npv.sxryk.cn

Go:   // 无解构
来源：http://brd.pycfn.com

Ruby: a, b = pair
来源：http://eel.9152youxi.cn

C#:   var (a, b) = pair;
来源：http://fai.zycfv.cn

[C16] 函数 / 方法重载
来源：http://aea.tian-w.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lda.ydzc1.top

PHP:  // 无重载
来源：http://rlp.xziqi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ocf.dianchejie.cn

TS:   // 用联合类型或重载签名声明
来源：http://rzu.quarkkingdee.top

Java: void f(int a) {}  void f(String a) {}
来源：http://kca.pengpengdd.cyou

Go:   // 无重载：用不同函数名
来源：http://ooc.cucudq.cn

Ruby: # 无重载：靠动态参数
来源：http://qev.smart0.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://kua.xziqi.cn

================================================================================
来源：http://opn.zdbjq.cn

D. 数组 / 列表 / 集合
来源：http://lrk.kuanghao11.cn

================================================================================
来源：http://iif.ppjwa.cn

[D01] 创建数组 / 列表
来源：http://cca.zhijiandao.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://att.tian-w.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://czr.zdqjudy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ras.shuidangran.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://smt.cashguo.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hgz.ybcxt.top

Go:   arr := []int{1, 2, 3}
来源：http://dpt.hammf.cn

Ruby: arr = [1, 2, 3]
来源：http://lmf.jinghuilouyu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bra.haohaochexian.top

[D02] 追加元素到末尾
来源：http://unn.hywenlv.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vcu.zhongyouzk.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jpz.shanyushiyangkeji.top

JS:   arr.push(4);
来源：http://qcz.daria6918.cn

TS:   arr.push(4);
来源：http://esr.fanxiaobao.xyz

Java: list.add(4);
来源：http://fqx.tianlin.xyz

Go:   arr = append(arr, 4)
来源：http://ilw.vqdsnc.cn

Ruby: arr << 4; arr.push(5)
来源：http://fle.jinqigfzy.top

C#:   list.Add(4);
来源：http://nzq.hysaishi.cn

[D03] 在指定位置插入元素
来源：http://itx.redwolf501.top

Py:   arr.insert(0, 0)
来源：http://wnz.hnxiangtu.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://brb.guowangkeji.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xox.svipenyu.cn

TS:   arr.splice(0, 0, 0);
来源：http://ssc.xingfuxueyuan.xyz

Java: list.add(0, 0);
来源：http://rpv.cheryme.top

Go:   arr = append([]int{0}, arr...)
来源：http://qfh.dianchejie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xoi.vehdjk.com

C#:   list.Insert(0, 0);
来源：http://nva.chenzaomai.com

[D04] 删除元素
来源：http://kln.dianchejie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jjb.yj20258.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jdb.mhx1999.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://aug.zhijiandao.cn

TS:   arr.splice(0, 1);
来源：http://ytj.haohaochexian.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://irx.zhaomingkeji.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wpr.shzxlz.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ggd.zhijiandao.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://oun.ydjk.org.cn

[D05] 访问与修改元素
来源：http://xgc.fengsongda.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zrc.zycfv.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bdx.ydzc1.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hhe.gaohongyu789.top

TS:   arr[0]; arr.at(-1);
来源：http://lat.zdbjq.cn

Java: list.get(0); list.set(0, 9);
来源：http://dpp.ivvv.top

Go:   arr[0]; arr[0] = 9
来源：http://mpb.316326.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fjg.jyoumei.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fut.xinyue.icu

[D06] 数组长度
来源：http://dqn.shuidangran.top

Py:   len(arr)
来源：http://xxn.svipenyu.cn

PHP:  count($arr);
来源：http://rqv.yonumen.top

JS:   arr.length
来源：http://maz.uphjek.com

TS:   arr.length
来源：http://emg.tanke756.top

Java: list.size();
来源：http://gzb.0kj1m.cn

Go:   len(arr)
来源：http://mkp.ydjk.org.cn

Ruby: arr.length; arr.size
来源：http://hlx.ctjpmb.com

C#:   list.Count;
来源：http://hjh.ydzc1.top

[D07] 切片 / 取子数组
来源：http://oxo.snrcjt.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gst.0kj1m.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ezm.yj20258.top

JS:   arr.slice(1, 4);
来源：http://gyq.yj20258888.top

TS:   arr.slice(1, 4);
来源：http://uff.zhongyouzk.top

Java: list.subList(1, 4);
来源：http://lbm.316326.xyz

Go:   arr[1:4]
来源：http://dlg.ppjwa.cn

Ruby: arr[1, 3]
来源：http://qbu.daria6918.cn

C#:   list.GetRange(1, 3);
来源：http://sqq.xziqi.cn

[D08] 合并两个数组
来源：http://kgr.tianlin.xyz

Py:   a + b;  a.extend(b)
来源：http://icx.xylfe.cn

PHP:  array_merge($a, $b);
来源：http://bwb.ctjpmb.com

JS:   [...a, ...b];  a.concat(b);
来源：http://lpg.daria6918.cn

TS:   [...a, ...b];
来源：http://vcu.fengsongda.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://uqi.shanyushiyangkeji.top

Go:   append(a, b...)
来源：http://yox.yvedp.cn

Ruby: a + b;  a.concat(b)
来源：http://oak.sysykeji.top

C#:   a.Concat(b).ToList()
来源：http://yzh.yongpay.top

[D09] 排序（升序）
来源：http://rzk.iojbl.cn

Py:   sorted(arr);  arr.sort()
来源：http://qrt.shanyushiyangtech.top

PHP:  sort($arr);
来源：http://tgp.nanxinkj.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zby.birdmap.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://dkm.52xcode.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tdf.wangdashe.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ftn.hesvh.cn

Ruby: arr.sort
来源：http://izr.xinyue.icu

C#:   list.Sort();
来源：http://awe.zhoulong.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://vef.mhx1999.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://plj.gaohongyu789.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dqs.zdqjudy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://atf.dashuyun.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qxs.jyoumei.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tmr.zdqjudy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cbz.snrcjt.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jeg.jianghu66.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qiq.guannengcc.top

[D11] 反转数组
来源：http://zvf.kuanghao11.cn

Py:   arr[::-1];  arr.reverse()
来源：http://sjd.yanxiufei.cn

PHP:  array_reverse($arr);
来源：http://hki.jinyuanbaomall.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gbi.uphjek.com

TS:   [...arr].reverse();
来源：http://uvo.shanyushiyangkeji.top

Java: Collections.reverse(list);
来源：http://czv.yj202588.top

Go:   slices.Reverse(arr)
来源：http://cxm.zdbjq.cn

Ruby: arr.reverse
来源：http://drm.yangfankeji.com

C#:   list.Reverse();
来源：http://pfi.yvedp.cn

[D12] 查找元素下标
来源：http://vko.zdbjq.cn

Py:   arr.index(x);  x in arr
来源：http://dcm.c1oappe.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fep.daria6918.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://khg.xziqi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iyf.ydzc1.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ppb.wangdashe.top

Go:   slices.Index(arr, x)
来源：http://frx.mhx1999.top

Ruby: arr.index(x)
来源：http://ajw.ehwqpu.com

C#:   list.IndexOf(x);
来源：http://wof.hesvh.cn

[D13] 过滤（保留满足条件的）
来源：http://prr.cheryme.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mns.jinghuilouyu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jdw.jinqigufen.top

JS:   arr.filter(x => x > 3)
来源：http://fzl.aizwys.cn

TS:   arr.filter(x => x > 3)
来源：http://nma.nanxinkj.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wcv.nanxinkj.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://msl.9152youxi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xuz.svipenyu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zdm.sweek.top

[D14] 映射转换（每个元素变形）
来源：http://ecw.hcnkem.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://urg.yfazqb.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xkh.316326.xyz

JS:   arr.map(x => x * 2)
来源：http://gnd.cashguo.top

TS:   arr.map(x => x * 2)
来源：http://bmx.zhaomingkeji.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://dnw.jinghuilouyu.cn

Go:   // 手写循环
来源：http://cfo.nanxinkj.top

Ruby: arr.map { |x| x * 2 }
来源：http://ydp.yuxming.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pfg.yj202588.top

[D15] 去重
来源：http://rfd.havefunace.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://oru.shzxlz.cn

PHP:  array_unique($arr);
来源：http://raq.uphjek.com

JS:   [...new Set(arr)]
来源：http://svh.epnwcf.com

TS:   [...new Set(arr)]
来源：http://ecy.ydzc1.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tkt.jinqigufen.top

Go:   // 用 map[T]struct{} 手写
来源：http://yxa.feifeiyinyue.top

Ruby: arr.uniq
来源：http://mpz.ywan-chungtsiang.top


<!-- 参考信息 -->
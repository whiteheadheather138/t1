代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mdp.0kj1m.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://opo.yanxiufei.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wiw.zhiwuduotai.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tqn.iojbl.cn

[B13] 判断是否为数字
来源：http://pni.dashuyun.cn

Py:   isinstance(x, (int, float))
来源：http://wpv.redwolf501.top

PHP:  is_numeric($x)
来源：http://eme.wangshuangyany.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zlm.jinyuanbaomall.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vum.yuxming.cn

Java: x instanceof Number
来源：http://vvw.0kj1m.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://acu.yanxiufei.cn

Ruby: x.is_a?(Numeric)
来源：http://glc.wangshuangyany.cn

C#:   x is int or double or decimal
来源：http://lun.zdqjudy.top

[B14] 判断值是否在集合内
来源：http://sfc.ppjwa.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://crm.hnqzz.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sks.gaohongyu789.top

JS:   [1, 2, 3].includes(x)
来源：http://zny.ywan-chungtsiang.top

TS:   [1, 2, 3].includes(x)
来源：http://bdb.xuetiantiany.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vvu.snrcjt.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ajo.zycfv.cn

Ruby: [1, 2, 3].include?(x)
来源：http://elv.ctjpmb.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rqe.yuanzhike.top

[B15] 布尔运算与取反
来源：http://fff.hammf.cn

Py:   a and b or not c
来源：http://ryw.cdnleiting.top

PHP:  $a && $b || !$c
来源：http://pnl.jqgfzy.top

JS:   a && b || !c
来源：http://juv.hammf.cn

TS:   a && b || !c
来源：http://wsj.uphjek.com

Java: a && b || !c
来源：http://wds.kuanghao11.cn

Go:   a && b || !c
来源：http://cie.shuidangran.top

Ruby: a && b || !c
来源：http://zsx.ywan-chungtsiang.top

C#:   a && b || !c
来源：http://shz.sjlbkw.cn

[B16] 卫语句：不满足条件提前返回
来源：http://cdz.fehbvm.com

Py:   if not data: return
来源：http://fng.jinqigfzy.top

PHP:  if (!$data) { return; }
来源：http://kwj.hywenlv.cn

JS:   if (!data) return;
来源：http://nnl.xinyue.icu

TS:   if (!data) return;
来源：http://xpv.ivvv.top

Java: if (data == null) return;
来源：http://upn.cucudq.cn

Go:   if data == nil { return }
来源：http://mrs.yj202588.top

Ruby: return if data.nil?
来源：http://spv.yangfankeji.com

C#:   if (data == null) return;
来源：http://nbt.pycfn.com

================================================================================
来源：http://sfl.ehwqpu.com

C. 函数与作用域
来源：http://zhn.shuidangran.top

================================================================================
来源：http://xgb.yangfankeji.com

[C01] 定义函数
来源：http://dpg.mhx1999.top

Py:   def add(a, b): return a + b
来源：http://ppo.yanxiufei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yav.feifeiyinyue.top

JS:   function add(a, b) { return a + b; }
来源：http://iog.hywenlv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bvj.gzhubu.top

Java: static int add(int a, int b) { return a + b; }
来源：http://xze.tanke756.top

Go:   func add(a, b int) int { return a + b }
来源：http://icz.zhengqikj.top

Ruby: def add(a, b); a + b; end
来源：http://uhu.0kj1m.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rij.hammf.cn

[C02] 默认参数
来源：http://irx.0kj1m.cn

Py:   def greet(name="World"): return name
来源：http://ecz.zycfv.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ycg.gogol.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://aqw.sysykeji.top

TS:   function greet(name: string = "World") { return name; }
来源：http://kyu.hesvh.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hhi.yangfankeji.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qfj.feifeiyinyue.top

Ruby: def greet(name = "World") = name
来源：http://pme.jinqigufen.top

C#:   string Greet(string name = "World") => name;
来源：http://ngk.yj202588.top

[C03] 可变参数
来源：http://apn.zhengqikj.top

Py:   def total(*args): return sum(args)
来源：http://mjk.andypj.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nce.xuanzx.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mos.andypj.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yhz.xziqi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://azw.yangfankeji.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://iro.cashguo.top

Ruby: def total(*nums); nums.sum; end
来源：http://zes.epnwcf.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://abu.tanke756.top

[C04] 命名参数 / 关键字参数
来源：http://xqa.cashguo.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lam.feifeiyinyue.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://das.jinghuilouyu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vpt.pengpengdd.cyou

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://uvu.uphjek.com

Java: // 无：用 Builder 模式或 record
来源：http://mwf.jiagoushi.top

Go:   // 无：用配置结构体参数
来源：http://npj.yangfankeji.com

Ruby: f(a: 1, b: 2)
来源：http://ttl.chenlongwang.top

C#:   f(a: 1, b: 2)
来源：http://mjg.cheryme.top

[C05] 返回多个值
来源：http://vqw.jqgfzy.top

Py:   return a, b
来源：http://gxu.bbcook.cn

PHP:  return [$a, $b];
来源：http://ows.yueranfly.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://pzi.c1oappe.top

TS:   return { a, b };
来源：http://tso.tianlin.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://stz.bbcook.cn

Go:   return a, b
来源：http://tjr.dashuyun.cn

Ruby: return a, b
来源：http://rry.yanxiufei.cn

C#:   return (a, b);              // ValueTuple
来源：http://hiz.haohaochexian.top

[C06] 匿名函数 / lambda
来源：http://jnt.hammf.cn

Py:   square = lambda x: x * x
来源：http://qmi.sjlbkw.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://tck.yuanzhike.top

JS:   const square = x => x * x;
来源：http://qtd.yfazqb.com

TS:   const square = (x: number): number => x * x;
来源：http://hqn.aizwys.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fhr.shangyingyoupin.top

Go:   sq := func(x int) int { return x * x }
来源：http://jlo.0kj1m.cn

Ruby: square = ->(x) { x * x }
来源：http://uxf.xziqi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bqz.daxiang520.top

[C07] 把函数作为参数传入
来源：http://mqp.fengsongda.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gwe.zycfv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://dug.chenlongwang.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nxe.yvedp.cn

TS:   arr.map(String)
来源：http://oxv.jqgufenzy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tif.shuidangran.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://olf.yanxiufei.cn

Ruby: arr.map(&:upcase)
来源：http://dys.shzxlz.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cht.yj202588.top

[C08] 闭包
来源：http://ikx.jinyuanbaomall.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wws.hfpthk.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yip.sweek.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qjy.yonumen.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lux.shanyushiyangtech.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jks.ybcxt.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ylw.ppjwa.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://loa.zhengqikj.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vgy.yj202588.top

[C09] 递归
来源：http://jnj.feifeiyinyue.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fdp.cucudq.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://maw.hywenlv.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ehu.vqdsnc.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cjg.tianlin.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jyd.redwolf501.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rzm.xuanzx.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xfu.cqqwz.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://thz.jyoumei.cn

[C10] 变量作用域
来源：http://dza.zhoulong.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fsk.316326.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jiy.nanxuanxn.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://oly.sjlbkw.cn

TS:   同 JS
来源：http://fsh.feifeiyinyue.top

Java: 方法内为块级作用域
来源：http://tei.yj20258888.top

Go:   花括号块级作用域
来源：http://ctv.jiagoushi.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dlq.uphjek.com

C#:   块级作用域
来源：http://hip.jyoumei.cn

[C11] 模块导入与导出
来源：http://nqy.sweek.top

Py:   from module import func
来源：http://kdu.jyoumei.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://kxa.yj20258888.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://hje.jqgfzy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://usx.fktsv.cn

Java: import java.util.List;
来源：http://knm.shuidangran.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://alr.hnxiangtu.top

Ruby: require "json"; require_relative "./util"
来源：http://ayc.hysaishi.cn

C#:   using System.Text;
来源：http://ojy.tanke756.top

[C12] 立即执行函数 IIFE
来源：http://jlb.andypj.xyz

Py:   (lambda: print("run"))()
来源：http://loj.sxryk.cn

PHP:  (function () { echo "run"; })();
来源：http://gbn.316326.xyz

JS:   (() => { console.log("run"); })();
来源：http://doj.jinqigfzy.top

TS:   (() => { console.log("run"); })();
来源：http://nrt.smart0.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://keb.yuxming.cn

Go:   func() { fmt.Println("run") }()
来源：http://jsj.xuanzx.com

Ruby: -> { puts "run" }.call
来源：http://dfz.snrcjt.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://kgm.xingfuxueyuan.xyz

[C13] 类型声明 / 类型注解
来源：http://zmm.hongshengwenyu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rhz.0kj1m.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uch.tanke756.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ovu.epnwcf.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wel.pengpengdd.cyou

Java: int add(int a, int b) { return a + b; }
来源：http://jiq.yuanzhike.top

Go:   func add(a, b int) int
来源：http://xto.hfpthk.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wwt.fzhhl.top

C#:   int Add(int a, int b) => a + b;
来源：http://zaa.yj20258.top

[C14] 泛型函数
来源：http://ntv.hammf.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zgh.hesvh.cn

PHP:  // 无泛型
来源：http://hnn.hammf.cn

JS:   // 无泛型
来源：http://nzn.jinyuanbaomall.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nhi.9152youxi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bpa.fengsongda.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gzv.guowangkeji.top

Ruby: # 无泛型
来源：http://pjp.snrcjt.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://oic.zdbjq.cn

[C15] 解构 / 展开参数
来源：http://afy.bjfxy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://brs.ehwqpu.com

PHP:  [$a, $b] = $pair;
来源：http://dui.feifeiyinyue.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bbe.xingfuxueyuan.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jzo.316326.xyz

Java: // 无解构
来源：http://wat.hnqzz.top

Go:   // 无解构
来源：http://sjj.birdmap.top

Ruby: a, b = pair
来源：http://fia.cdnleiting.top

C#:   var (a, b) = pair;
来源：http://byb.cucudq.cn

[C16] 函数 / 方法重载
来源：http://xdz.hfpthk.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://azq.kuanghao11.cn

PHP:  // 无重载
来源：http://qmg.jianghu66.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://iou.xingfuxueyuan.xyz

TS:   // 用联合类型或重载签名声明
来源：http://yru.yonumen.top

Java: void f(int a) {}  void f(String a) {}
来源：http://wsl.kuanghao11.cn

Go:   // 无重载：用不同函数名
来源：http://ycv.zhaomingkeji.xyz

Ruby: # 无重载：靠动态参数
来源：http://rst.zdqjudy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://pny.xingfuxueyuan.xyz

================================================================================
来源：http://xgm.zhaomingkeji.xyz

D. 数组 / 列表 / 集合
来源：http://ajx.ivvv.top

================================================================================
来源：http://vrr.meibo888.top

[D01] 创建数组 / 列表
来源：http://moz.bjfxy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://lwp.xuetiantiany.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://uey.316326.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qlt.quarkkingdee.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://bkb.hammf.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tlt.dianchejie.cn

Go:   arr := []int{1, 2, 3}
来源：http://tgc.gzhubu.top

Ruby: arr = [1, 2, 3]
来源：http://mcf.ppjwa.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://evx.chenzaomai.com

[D02] 追加元素到末尾
来源：http://nls.zhixingplan.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dwq.cheryme.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fal.xinyue.icu

JS:   arr.push(4);
来源：http://qsr.nanxinkj.top

TS:   arr.push(4);
来源：http://ypn.dashuyun.cn

Java: list.add(4);
来源：http://gyg.chenzaomai.com

Go:   arr = append(arr, 4)
来源：http://kne.quarkkingdee.top

Ruby: arr << 4; arr.push(5)
来源：http://hhi.ehwqpu.com

C#:   list.Add(4);
来源：http://fis.bjfxy.top

[D03] 在指定位置插入元素
来源：http://zsc.hnqzz.top

Py:   arr.insert(0, 0)
来源：http://piq.quarkkingdee.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://frm.dianchejie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mlz.shzxlz.cn

TS:   arr.splice(0, 0, 0);
来源：http://qtw.bbcook.cn

Java: list.add(0, 0);
来源：http://woh.9152youxi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zjb.zhaomingkeji.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://eih.hcnkem.com

C#:   list.Insert(0, 0);
来源：http://tjm.kuanghao11.cn

[D04] 删除元素
来源：http://aqz.pycfn.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fxi.guowangkeji.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hhv.hongshengwenyu.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://poq.xinyue.icu

TS:   arr.splice(0, 1);
来源：http://uyj.aibaodan.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vef.0kj1m.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zby.tian-w.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://udh.chenzaomai.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ynh.nwbrower.top

[D05] 访问与修改元素
来源：http://oxy.zhengqikj.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sce.sxryk.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cms.vqdsnc.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lvd.cheryme.top

TS:   arr[0]; arr.at(-1);
来源：http://zux.cheryme.top

Java: list.get(0); list.set(0, 9);
来源：http://gpk.nwbrower.top

Go:   arr[0]; arr[0] = 9
来源：http://wum.snrcjt.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://auf.xziqi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bye.zdqjudy.top

[D06] 数组长度
来源：http://rkd.nanxinkj.top

Py:   len(arr)
来源：http://zax.xingfuxueyuan.xyz

PHP:  count($arr);
来源：http://nlh.jinyuanbaomall.cn

JS:   arr.length
来源：http://wul.zhoulong.xyz

TS:   arr.length
来源：http://bzv.9152youxi.cn

Java: list.size();
来源：http://ycv.shanyushiyangkeji.top

Go:   len(arr)
来源：http://zzi.kuanghao11.cn

Ruby: arr.length; arr.size
来源：http://qki.gaohongyu789.top

C#:   list.Count;
来源：http://pkc.shanyushiyangkeji.top

[D07] 切片 / 取子数组
来源：http://xtd.9152youxi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zcc.pycfn.com

PHP:  array_slice($arr, 1, 3);
来源：http://azi.daria6918.cn

JS:   arr.slice(1, 4);
来源：http://wdu.sweek.top

TS:   arr.slice(1, 4);
来源：http://uqn.yongpay.top

Java: list.subList(1, 4);
来源：http://zli.yueranfly.top

Go:   arr[1:4]
来源：http://mhk.uphjek.com

Ruby: arr[1, 3]
来源：http://ejj.daxiang520.top

C#:   list.GetRange(1, 3);
来源：http://mlk.xuetiantiany.cn

[D08] 合并两个数组
来源：http://alc.havefunace.top

Py:   a + b;  a.extend(b)
来源：http://csn.yangfankeji.com

PHP:  array_merge($a, $b);
来源：http://xsh.yonumen.top

JS:   [...a, ...b];  a.concat(b);
来源：http://min.jiagoushi.top

TS:   [...a, ...b];
来源：http://qzb.ppjwa.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lcd.cucudq.cn

Go:   append(a, b...)
来源：http://akr.fzhhl.top

Ruby: a + b;  a.concat(b)
来源：http://jqj.nwbrower.top

C#:   a.Concat(b).ToList()
来源：http://wkv.9152youxi.cn

[D09] 排序（升序）
来源：http://ttp.snrcjt.cn

Py:   sorted(arr);  arr.sort()
来源：http://uvq.9152youxi.cn

PHP:  sort($arr);
来源：http://njs.0kj1m.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zej.sjlbkw.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://soa.yj20258888.top

Java: Collections.sort(list);  list.sort(null);
来源：http://wwu.ydjk.org.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dco.yfazqb.com

Ruby: arr.sort
来源：http://ydw.yvedp.cn

C#:   list.Sort();
来源：http://ybk.quarkkingdee.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://sjx.nanxinkj.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://eya.wangshuangyany.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://haj.aizwys.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zsd.andypj.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sha.hywenlv.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hzz.nanxuanxn.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://szh.birdmap.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hic.cdnleiting.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qho.fanxiaobao.xyz

[D11] 反转数组
来源：http://osv.hywenlv.cn

Py:   arr[::-1];  arr.reverse()
来源：http://uot.316326.xyz

PHP:  array_reverse($arr);
来源：http://lvk.uphjek.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lsc.yfazqb.com

TS:   [...arr].reverse();
来源：http://pva.ydzc1.top

Java: Collections.reverse(list);
来源：http://gut.gzhubu.top

Go:   slices.Reverse(arr)
来源：http://htu.ivvv.top

Ruby: arr.reverse
来源：http://gte.jlsjyb.cn

C#:   list.Reverse();
来源：http://npo.quarkkingdee.top

[D12] 查找元素下标
来源：http://yls.guannengcc.top

Py:   arr.index(x);  x in arr
来源：http://ask.vqdsnc.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bah.zdqjudy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vyo.sweek.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://piu.hongshengwenyu.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qnm.vehdjk.com

Go:   slices.Index(arr, x)
来源：http://tqf.zhijiandao.cn

Ruby: arr.index(x)
来源：http://hyt.zhengqikj.top

C#:   list.IndexOf(x);
来源：http://vhd.tianlin.xyz

[D13] 过滤（保留满足条件的）
来源：http://dsc.zhiwuduotai.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://atx.yongpay.top


<!-- 参考信息 -->
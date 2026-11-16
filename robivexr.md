代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://omu.jinqigufen.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vbl.zdbjq.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://aus.zdbjq.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hbg.jinqigufen.top

[B13] 判断是否为数字
来源：http://wui.sweek.top

Py:   isinstance(x, (int, float))
来源：http://zwp.bbcook.cn

PHP:  is_numeric($x)
来源：http://pfn.zhixingplan.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cco.zdbjq.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xlm.jqgufenzy.top

Java: x instanceof Number
来源：http://fwj.shuidangran.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hrb.hesvh.cn

Ruby: x.is_a?(Numeric)
来源：http://mph.fengsongda.top

C#:   x is int or double or decimal
来源：http://tse.gotoacloud.top

[B14] 判断值是否在集合内
来源：http://krp.shangyingyoupin.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uzr.aizwys.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lcv.fengsongda.top

JS:   [1, 2, 3].includes(x)
来源：http://kut.pycfn.com

TS:   [1, 2, 3].includes(x)
来源：http://jbu.jinqigufen.top

Java: List.of(1, 2, 3).contains(x)
来源：http://gyv.jinqigufen.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fnb.haohaochexian.top

Ruby: [1, 2, 3].include?(x)
来源：http://esw.zhixingplan.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cuz.ydjk.org.cn

[B15] 布尔运算与取反
来源：http://sqm.gaohongyu789.top

Py:   a and b or not c
来源：http://hkw.fehbvm.com

PHP:  $a && $b || !$c
来源：http://zwo.yanxiufei.cn

JS:   a && b || !c
来源：http://mpu.havefunace.top

TS:   a && b || !c
来源：http://wwr.hnxiangtu.top

Java: a && b || !c
来源：http://nil.fanxiaobao.xyz

Go:   a && b || !c
来源：http://rpn.bjfxy.top

Ruby: a && b || !c
来源：http://cgv.meibo888.top

C#:   a && b || !c
来源：http://mvj.fanxiaobao.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://dkh.jlsjyb.cn

Py:   if not data: return
来源：http://vmx.cucudq.cn

PHP:  if (!$data) { return; }
来源：http://mmv.hesvh.cn

JS:   if (!data) return;
来源：http://jjm.zhongyouzk.top

TS:   if (!data) return;
来源：http://fjn.jianghu66.top

Java: if (data == null) return;
来源：http://dxt.birdmap.top

Go:   if data == nil { return }
来源：http://pud.shangyingyoupin.top

Ruby: return if data.nil?
来源：http://wsb.epnwcf.com

C#:   if (data == null) return;
来源：http://mrv.fktsv.cn

================================================================================
来源：http://vad.gzhubu.top

C. 函数与作用域
来源：http://szv.0kj1m.cn

================================================================================
来源：http://vku.havefunace.top

[C01] 定义函数
来源：http://mwt.hesvh.cn

Py:   def add(a, b): return a + b
来源：http://vop.zhixingplan.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jly.316326.xyz

JS:   function add(a, b) { return a + b; }
来源：http://anv.zhongyouzk.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bwa.haohaochexian.top

Java: static int add(int a, int b) { return a + b; }
来源：http://bfz.jinghuilouyu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://skk.fanxiaobao.xyz

Ruby: def add(a, b); a + b; end
来源：http://emd.feifeiyinyue.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qtw.jinqigufen.top

[C02] 默认参数
来源：http://mqc.sjlbkw.cn

Py:   def greet(name="World"): return name
来源：http://vbd.cdnleiting.top

PHP:  function greet($name = "World") { return $name; }
来源：http://dba.zhengqikj.top

JS:   function greet(name = "World") { return name; }
来源：http://wdn.zdqjudy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://azx.snrcjt.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://znf.xingfuxueyuan.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rol.sufxvd.cn

Ruby: def greet(name = "World") = name
来源：http://fuy.yanxiufei.cn

C#:   string Greet(string name = "World") => name;
来源：http://sdw.hfpthk.cn

[C03] 可变参数
来源：http://uzq.52xcode.cn

Py:   def total(*args): return sum(args)
来源：http://qxq.daxiang520.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sfr.chenjidiqi.icu

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vti.zhongyouzk.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tkk.cashguo.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mvd.pycfn.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://emo.smart0.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://zwu.daxiang520.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ctv.ydzc1.top

[C04] 命名参数 / 关键字参数
来源：http://sbi.yanxiufei.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://doy.guowangkeji.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mzn.xziqi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ygp.yanxiufei.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://grt.yonumen.top

Java: // 无：用 Builder 模式或 record
来源：http://inz.redwolf501.top

Go:   // 无：用配置结构体参数
来源：http://kmh.chenzaomai.com

Ruby: f(a: 1, b: 2)
来源：http://whc.aibaodan.cn

C#:   f(a: 1, b: 2)
来源：http://rrh.tian-w.cn

[C05] 返回多个值
来源：http://coy.xziqi.cn

Py:   return a, b
来源：http://umj.fktsv.cn

PHP:  return [$a, $b];
来源：http://lhk.aizwys.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://nch.yuxming.cn

TS:   return { a, b };
来源：http://jlw.yj20258888.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wyt.tarul.cn

Go:   return a, b
来源：http://pou.yj20258888.top

Ruby: return a, b
来源：http://drb.shuidangran.top

C#:   return (a, b);              // ValueTuple
来源：http://pbe.gaohongyu789.top

[C06] 匿名函数 / lambda
来源：http://vpa.hnqzz.top

Py:   square = lambda x: x * x
来源：http://ubd.birdmap.top

PHP:  $square = fn($x) => $x * $x;
来源：http://itk.ehwqpu.com

JS:   const square = x => x * x;
来源：http://ewy.zycfv.cn

TS:   const square = (x: number): number => x * x;
来源：http://kvo.c1oappe.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hsz.jinqigfzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://lzf.cdnleiting.top

Ruby: square = ->(x) { x * x }
来源：http://pat.xuanzx.com

C#:   Func<int, int> square = x => x * x;
来源：http://ijj.quarkkingdee.top

[C07] 把函数作为参数传入
来源：http://mcc.hammf.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://uhk.fengsongda.top

PHP:  array_map("strtoupper", $arr);
来源：http://cnu.smart0.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bcq.yangfankeji.com

TS:   arr.map(String)
来源：http://aqb.svipenyu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://smj.vehdjk.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hoy.vqdsnc.cn

Ruby: arr.map(&:upcase)
来源：http://vvi.guowangkeji.top

C#:   arr.Select(s => s.ToUpper())
来源：http://fvg.hnqzz.top

[C08] 闭包
来源：http://cwd.vqdsnc.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rld.yuxming.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rhx.hammf.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://etn.jiagoushi.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ite.hongshengwenyu.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tpi.yanxiufei.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://szp.tian-w.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://crj.yvedp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tcm.jlsjyb.cn

[C09] 递归
来源：http://sjc.guannengcc.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xuz.hcnkem.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mzt.zhongyouzk.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://snm.c1oappe.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aya.hnqzz.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lmu.cucudq.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://swx.fehbvm.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jgj.shangyingyoupin.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jtd.hfpthk.cn

[C10] 变量作用域
来源：http://mpo.tanke756.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://itd.zhiwuduotai.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vge.fzhhl.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vot.birdmap.top

TS:   同 JS
来源：http://tet.epnwcf.com

Java: 方法内为块级作用域
来源：http://pyc.52xcode.cn

Go:   花括号块级作用域
来源：http://apj.meibo888.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fnr.uphjek.com

C#:   块级作用域
来源：http://vkq.shangyingyoupin.top

[C11] 模块导入与导出
来源：http://phy.yvedp.cn

Py:   from module import func
来源：http://hgz.jinqigufen.top

PHP:  require "file.php";  或 use App\Service;
来源：http://dql.hnqzz.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://zea.xziqi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yqk.andypj.xyz

Java: import java.util.List;
来源：http://ryi.uphjek.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tdl.pengpengdd.cyou

Ruby: require "json"; require_relative "./util"
来源：http://osp.yj20258.top

C#:   using System.Text;
来源：http://sjx.xziqi.cn

[C12] 立即执行函数 IIFE
来源：http://haw.aibaodan.cn

Py:   (lambda: print("run"))()
来源：http://dew.9152youxi.cn

PHP:  (function () { echo "run"; })();
来源：http://orq.c1oappe.top

JS:   (() => { console.log("run"); })();
来源：http://lnn.hongshengwenyu.top

TS:   (() => { console.log("run"); })();
来源：http://tfx.cqqwz.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tre.andypj.xyz

Go:   func() { fmt.Println("run") }()
来源：http://sub.yongpay.top

Ruby: -> { puts "run" }.call
来源：http://het.chenlongwang.top

C#:   // 无 IIFE：用静态构造函数
来源：http://lmx.pengpengdd.cyou

[C13] 类型声明 / 类型注解
来源：http://gst.sjlbkw.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gvu.yfazqb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fpc.redwolf501.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baz.ivvv.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xtk.mhx1999.top

Java: int add(int a, int b) { return a + b; }
来源：http://ktv.smart0.xyz

Go:   func add(a, b int) int
来源：http://aev.dianchejie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nzf.zhiwuduotai.top

C#:   int Add(int a, int b) => a + b;
来源：http://weh.hnqzz.top

[C14] 泛型函数
来源：http://pck.jqgfzy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zbr.ehwqpu.com

PHP:  // 无泛型
来源：http://mui.jqgufenzy.top

JS:   // 无泛型
来源：http://kxg.0kj1m.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kul.yanxiufei.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nba.zhongyouzk.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bcy.jqgfzy.top

Ruby: # 无泛型
来源：http://puy.hongshengwenyu.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://owt.vehdjk.com

[C15] 解构 / 展开参数
来源：http://ijl.jiagoushi.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://atb.yanxiufei.cn

PHP:  [$a, $b] = $pair;
来源：http://irg.fanxiaobao.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vql.fengsongda.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://brl.ywan-chungtsiang.top

Java: // 无解构
来源：http://gcj.shuidangran.top

Go:   // 无解构
来源：http://vjy.kuanghao11.cn

Ruby: a, b = pair
来源：http://eyl.cucudq.cn

C#:   var (a, b) = pair;
来源：http://hiw.bbcook.cn

[C16] 函数 / 方法重载
来源：http://ros.tian-w.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vsy.cdnleiting.top

PHP:  // 无重载
来源：http://ucz.guowangkeji.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://zil.yangfankeji.com

TS:   // 用联合类型或重载签名声明
来源：http://uuc.jqgfzy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://vmr.chenlongwang.top

Go:   // 无重载：用不同函数名
来源：http://yeo.ydzc1.top

Ruby: # 无重载：靠动态参数
来源：http://ies.snrcjt.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xcs.redwolf501.top

================================================================================
来源：http://rwm.zhongyouzk.top

D. 数组 / 列表 / 集合
来源：http://yuc.jinqigfzy.top

================================================================================
来源：http://bnv.andypj.xyz

[D01] 创建数组 / 列表
来源：http://tri.jianghu66.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://plz.cdnleiting.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lsh.daria6918.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rkf.zdbjq.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zbg.fktsv.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xlt.hnxiangtu.top

Go:   arr := []int{1, 2, 3}
来源：http://fwg.snrcjt.cn

Ruby: arr = [1, 2, 3]
来源：http://pkg.pengpengdd.cyou

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vyq.vqdsnc.cn

[D02] 追加元素到末尾
来源：http://pfq.cucudq.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cyo.yuanzhike.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qtx.snrcjt.cn

JS:   arr.push(4);
来源：http://eom.xziqi.cn

TS:   arr.push(4);
来源：http://mob.yvedp.cn

Java: list.add(4);
来源：http://huy.dashuyun.cn

Go:   arr = append(arr, 4)
来源：http://fyi.jqgufenzy.top

Ruby: arr << 4; arr.push(5)
来源：http://sxb.jlsjyb.cn

C#:   list.Add(4);
来源：http://vat.jianghu66.top

[D03] 在指定位置插入元素
来源：http://agq.hesvh.cn

Py:   arr.insert(0, 0)
来源：http://syh.tianlin.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mle.guowangkeji.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ipz.zhiwuduotai.top

TS:   arr.splice(0, 0, 0);
来源：http://imw.jiagoushi.top

Java: list.add(0, 0);
来源：http://pcs.snrcjt.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fjk.cashguo.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ggs.havefunace.top

C#:   list.Insert(0, 0);
来源：http://spq.fzhhl.top

[D04] 删除元素
来源：http://yjw.yanxiufei.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nkn.xinyue.icu

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ecl.ppjwa.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pje.haohaochexian.top

TS:   arr.splice(0, 1);
来源：http://kyo.pengpengdd.cyou

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gdy.birdmap.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://oai.xingfuxueyuan.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://euj.quarkkingdee.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://viy.guowangkeji.top

[D05] 访问与修改元素
来源：http://oar.zdbjq.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pxv.daxiang520.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wjg.fehbvm.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xll.ctjpmb.com

TS:   arr[0]; arr.at(-1);
来源：http://yxw.zdqjudy.top

Java: list.get(0); list.set(0, 9);
来源：http://puw.fzhhl.top

Go:   arr[0]; arr[0] = 9
来源：http://wtu.fzhhl.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yiu.birdmap.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wca.yuxming.cn

[D06] 数组长度
来源：http://oaw.yj20258888.top

Py:   len(arr)
来源：http://tme.zhoulong.xyz

PHP:  count($arr);
来源：http://hle.52xcode.cn

JS:   arr.length
来源：http://wlx.jinghuilouyu.cn

TS:   arr.length
来源：http://vcu.tanke756.top

Java: list.size();
来源：http://lep.tarul.cn

Go:   len(arr)
来源：http://jkf.andypj.xyz

Ruby: arr.length; arr.size
来源：http://duz.sjlbkw.cn

C#:   list.Count;
来源：http://dcd.hysaishi.cn

[D07] 切片 / 取子数组
来源：http://bza.jinqigufen.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://eft.uphjek.com

PHP:  array_slice($arr, 1, 3);
来源：http://fcc.zhaomingkeji.xyz

JS:   arr.slice(1, 4);
来源：http://wcp.gzhubu.top

TS:   arr.slice(1, 4);
来源：http://bcb.sufxvd.cn

Java: list.subList(1, 4);
来源：http://vpx.bjfxy.top

Go:   arr[1:4]
来源：http://rzz.tianlin.xyz

Ruby: arr[1, 3]
来源：http://koy.tanke756.top

C#:   list.GetRange(1, 3);
来源：http://ztf.vehdjk.com

[D08] 合并两个数组
来源：http://cuf.gaohongyu789.top

Py:   a + b;  a.extend(b)
来源：http://eol.shanyushiyangtech.top

PHP:  array_merge($a, $b);
来源：http://fzx.cdnleiting.top

JS:   [...a, ...b];  a.concat(b);
来源：http://yjt.hfpthk.cn

TS:   [...a, ...b];
来源：http://cxp.yangfankeji.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fvl.yueranfly.top

Go:   append(a, b...)
来源：http://rnu.yongpay.top

Ruby: a + b;  a.concat(b)
来源：http://hjj.hesvh.cn

C#:   a.Concat(b).ToList()
来源：http://mua.sysykeji.top

[D09] 排序（升序）
来源：http://zap.sjlbkw.cn

Py:   sorted(arr);  arr.sort()
来源：http://zgb.cucudq.cn

PHP:  sort($arr);
来源：http://fgf.yj202588.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://oqb.hammf.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ezu.shangyingyoupin.top

Java: Collections.sort(list);  list.sort(null);
来源：http://opy.shanyushiyangtech.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://arf.feifeiyinyue.top

Ruby: arr.sort
来源：http://yyj.gotoacloud.top

C#:   list.Sort();
来源：http://jda.xinyue.icu

[D10] 自定义排序（按字段 / 多条件）
来源：http://yok.0kj1m.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gzz.hnxiangtu.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nry.dashuyun.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gjk.chenlongwang.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tbb.guannengcc.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fje.yvedp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://khi.iojbl.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fsp.sxryk.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xaw.pengpengdd.cyou

[D11] 反转数组
来源：http://fib.tian-w.cn

Py:   arr[::-1];  arr.reverse()
来源：http://san.jqgfzy.top

PHP:  array_reverse($arr);
来源：http://zaf.bbcook.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ncs.ehwqpu.com

TS:   [...arr].reverse();
来源：http://neb.0kj1m.cn

Java: Collections.reverse(list);
来源：http://owg.tarul.cn

Go:   slices.Reverse(arr)
来源：http://taw.yueranfly.top

Ruby: arr.reverse
来源：http://eeb.wangshuangyany.cn

C#:   list.Reverse();
来源：http://uga.sysykeji.top

[D12] 查找元素下标
来源：http://hgl.hesvh.cn

Py:   arr.index(x);  x in arr
来源：http://ugm.guowangkeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qev.gotoacloud.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qor.9152youxi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://enm.hnqzz.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gwz.hnqzz.top

Go:   slices.Index(arr, x)
来源：http://pwr.sufxvd.cn

Ruby: arr.index(x)
来源：http://rfo.bjfxy.top

C#:   list.IndexOf(x);
来源：http://nvm.shangyingyoupin.top

[D13] 过滤（保留满足条件的）
来源：http://kha.kuanghao11.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nin.52xcode.cn


<!-- 参考信息 -->
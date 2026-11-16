代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://len.tanke756.top

TS:   [1, 2, 3].includes(x)
来源：http://zgz.yongpay.top

Java: List.of(1, 2, 3).contains(x)
来源：http://fqw.yangfankeji.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nkv.xziqi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://erb.haohaochexian.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dzn.zdqjudy.top

[B15] 布尔运算与取反
来源：http://lqy.shangyingyoupin.top

Py:   a and b or not c
来源：http://hkl.fktsv.cn

PHP:  $a && $b || !$c
来源：http://tno.yvedp.cn

JS:   a && b || !c
来源：http://lii.zhixingplan.top

TS:   a && b || !c
来源：http://xgv.fengsongda.top

Java: a && b || !c
来源：http://pfy.ydjk.org.cn

Go:   a && b || !c
来源：http://okp.zhiwuduotai.top

Ruby: a && b || !c
来源：http://plk.ctjpmb.com

C#:   a && b || !c
来源：http://bdq.yongpay.top

[B16] 卫语句：不满足条件提前返回
来源：http://zuv.pengpengdd.cyou

Py:   if not data: return
来源：http://vml.zhongyouzk.top

PHP:  if (!$data) { return; }
来源：http://sqr.dianchejie.cn

JS:   if (!data) return;
来源：http://kwi.daria6918.cn

TS:   if (!data) return;
来源：http://mmy.pycfn.com

Java: if (data == null) return;
来源：http://svq.sysykeji.top

Go:   if data == nil { return }
来源：http://crb.yonumen.top

Ruby: return if data.nil?
来源：http://rab.jqgufenzy.top

C#:   if (data == null) return;
来源：http://abm.gotoacloud.top

================================================================================
来源：http://fui.chenjidiqi.icu

C. 函数与作用域
来源：http://pgv.ppjwa.cn

================================================================================
来源：http://ecx.pengpengdd.cyou

[C01] 定义函数
来源：http://mof.tarul.cn

Py:   def add(a, b): return a + b
来源：http://cmm.xziqi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mlq.fanxiaobao.xyz

JS:   function add(a, b) { return a + b; }
来源：http://vul.xylfe.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fri.yj202588.top

Java: static int add(int a, int b) { return a + b; }
来源：http://dvk.sufxvd.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ozz.ppjwa.cn

Ruby: def add(a, b); a + b; end
来源：http://cfw.jianghu66.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hqq.bjfxy.top

[C02] 默认参数
来源：http://aoa.xziqi.cn

Py:   def greet(name="World"): return name
来源：http://ubz.zhengqikj.top

PHP:  function greet($name = "World") { return $name; }
来源：http://bes.zhongyouzk.top

JS:   function greet(name = "World") { return name; }
来源：http://rxt.316326.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://iqh.ydzc1.top

Java: // 无默认参数：方法重载或 Optional
来源：http://hvp.zhongyouzk.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kvz.fanxiaobao.xyz

Ruby: def greet(name = "World") = name
来源：http://iij.yj20258.top

C#:   string Greet(string name = "World") => name;
来源：http://oze.andypj.xyz

[C03] 可变参数
来源：http://rwt.meibo888.top

Py:   def total(*args): return sum(args)
来源：http://vhu.zycfv.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vuk.cdnleiting.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ttv.iojbl.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wmf.ybcxt.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lyt.yj20258.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kpd.vqdsnc.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ewq.jianghu66.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pdu.gogol.net.cn

[C04] 命名参数 / 关键字参数
来源：http://bdh.meibo888.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fae.guannengcc.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://keb.sjlbkw.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uff.hcnkem.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dsn.jinqigufen.top

Java: // 无：用 Builder 模式或 record
来源：http://dje.yj20258.top

Go:   // 无：用配置结构体参数
来源：http://iwx.0kj1m.cn

Ruby: f(a: 1, b: 2)
来源：http://aot.pycfn.com

C#:   f(a: 1, b: 2)
来源：http://kym.kuanghao11.cn

[C05] 返回多个值
来源：http://dpk.sjlbkw.cn

Py:   return a, b
来源：http://rxm.wangshuangyany.cn

PHP:  return [$a, $b];
来源：http://aij.vqdsnc.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://vvu.quarkkingdee.top

TS:   return { a, b };
来源：http://wit.zhijiandao.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://oph.yuanzhike.top

Go:   return a, b
来源：http://pxg.fanxiaobao.xyz

Ruby: return a, b
来源：http://qcc.xuetiantiany.cn

C#:   return (a, b);              // ValueTuple
来源：http://bca.c1oappe.top

[C06] 匿名函数 / lambda
来源：http://obp.vehdjk.com

Py:   square = lambda x: x * x
来源：http://drd.vehdjk.com

PHP:  $square = fn($x) => $x * $x;
来源：http://cim.hongshengwenyu.top

JS:   const square = x => x * x;
来源：http://urc.yj20258.top

TS:   const square = (x: number): number => x * x;
来源：http://jar.jyoumei.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://shk.epnwcf.com

Go:   sq := func(x int) int { return x * x }
来源：http://bbz.chenlongwang.top

Ruby: square = ->(x) { x * x }
来源：http://tia.zhijiandao.cn

C#:   Func<int, int> square = x => x * x;
来源：http://iss.sysykeji.top

[C07] 把函数作为参数传入
来源：http://vvq.jinghuilouyu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dwm.gaohongyu789.top

PHP:  array_map("strtoupper", $arr);
来源：http://aco.zdqjudy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xie.guannengcc.top

TS:   arr.map(String)
来源：http://bvh.ivvv.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tvn.yj20258.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zqt.epnwcf.com

Ruby: arr.map(&:upcase)
来源：http://jzk.yj20258.top

C#:   arr.Select(s => s.ToUpper())
来源：http://mdv.yj20258.top

[C08] 闭包
来源：http://sfm.wangshuangyany.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hsc.snrcjt.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nlz.uphjek.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vzo.gzhubu.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rmu.ywan-chungtsiang.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rwq.zhiwuduotai.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zey.cheryme.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mok.pycfn.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pia.316326.xyz

[C09] 递归
来源：http://wks.yvedp.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://myx.guowangkeji.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zat.gzhubu.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bjb.sxryk.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rfd.bbcook.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hpv.wangdashe.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://trz.ywan-chungtsiang.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tnz.chenlongwang.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hcl.ctjpmb.com

[C10] 变量作用域
来源：http://fkz.havefunace.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nrm.shuidangran.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://klq.jqgfzy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ksm.redwolf501.top

TS:   同 JS
来源：http://tvv.hywenlv.cn

Java: 方法内为块级作用域
来源：http://tfx.snrcjt.cn

Go:   花括号块级作用域
来源：http://dbv.smart0.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xgx.guowangkeji.top

C#:   块级作用域
来源：http://vlh.sjlbkw.cn

[C11] 模块导入与导出
来源：http://wkg.zdbjq.cn

Py:   from module import func
来源：http://kmb.bjfxy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ecd.zdqjudy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://oqb.guowangkeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qwm.vehdjk.com

Java: import java.util.List;
来源：http://xym.nanxinkj.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pcy.jinyuanbaomall.cn

Ruby: require "json"; require_relative "./util"
来源：http://gpu.yanxiufei.cn

C#:   using System.Text;
来源：http://puc.cucudq.cn

[C12] 立即执行函数 IIFE
来源：http://coi.birdmap.top

Py:   (lambda: print("run"))()
来源：http://sah.jqgfzy.top

PHP:  (function () { echo "run"; })();
来源：http://qfq.mhx1999.top

JS:   (() => { console.log("run"); })();
来源：http://bli.hnxiangtu.top

TS:   (() => { console.log("run"); })();
来源：http://egu.tianlin.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qfw.aizwys.cn

Go:   func() { fmt.Println("run") }()
来源：http://cnw.zhengqikj.top

Ruby: -> { puts "run" }.call
来源：http://clp.havefunace.top

C#:   // 无 IIFE：用静态构造函数
来源：http://gtl.gaohongyu789.top

[C13] 类型声明 / 类型注解
来源：http://evj.iojbl.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rfj.yueranfly.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://abf.yuanzhike.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://iew.bjfxy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vth.snrcjt.cn

Java: int add(int a, int b) { return a + b; }
来源：http://hid.jyoumei.cn

Go:   func add(a, b int) int
来源：http://vaw.ywan-chungtsiang.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ydc.andypj.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://hpv.xuetiantiany.cn

[C14] 泛型函数
来源：http://kua.fzhhl.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zhb.nanxuanxn.top

PHP:  // 无泛型
来源：http://hzl.hesvh.cn

JS:   // 无泛型
来源：http://gpy.yuxming.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://icn.xingfuxueyuan.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://czk.nanxuanxn.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bua.yongpay.top

Ruby: # 无泛型
来源：http://mbc.havefunace.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jsn.ywan-chungtsiang.top

[C15] 解构 / 展开参数
来源：http://zux.yuxming.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tfa.gotoacloud.top

PHP:  [$a, $b] = $pair;
来源：http://amm.kuanghao11.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://exb.9152youxi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://irb.shanyushiyangkeji.top

Java: // 无解构
来源：http://qrf.cheryme.top

Go:   // 无解构
来源：http://xdk.gotoacloud.top

Ruby: a, b = pair
来源：http://feu.jyoumei.cn

C#:   var (a, b) = pair;
来源：http://man.guowangkeji.top

[C16] 函数 / 方法重载
来源：http://ihk.zhaomingkeji.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qsz.jinqigfzy.top

PHP:  // 无重载
来源：http://qlb.shanyushiyangtech.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://njc.tianlin.xyz

TS:   // 用联合类型或重载签名声明
来源：http://ehw.ywan-chungtsiang.top

Java: void f(int a) {}  void f(String a) {}
来源：http://czh.redwolf501.top

Go:   // 无重载：用不同函数名
来源：http://wmp.yueranfly.top

Ruby: # 无重载：靠动态参数
来源：http://dqb.mhx1999.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://rfe.sxryk.cn

================================================================================
来源：http://grj.daxiang520.top

D. 数组 / 列表 / 集合
来源：http://mfg.guowangkeji.top

================================================================================
来源：http://mcd.fanxiaobao.xyz

[D01] 创建数组 / 列表
来源：http://qgy.bjfxy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://mve.xylfe.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hbi.gotoacloud.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://duq.ivvv.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://vuy.vqdsnc.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ikd.chenjidiqi.icu

Go:   arr := []int{1, 2, 3}
来源：http://ixm.aibaodan.cn

Ruby: arr = [1, 2, 3]
来源：http://fae.cashguo.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pww.316326.xyz

[D02] 追加元素到末尾
来源：http://sne.meibo888.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qvy.jqgfzy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xet.feifeiyinyue.top

JS:   arr.push(4);
来源：http://glv.ehwqpu.com

TS:   arr.push(4);
来源：http://jym.yj202588.top

Java: list.add(4);
来源：http://ocg.shuidangran.top

Go:   arr = append(arr, 4)
来源：http://ymh.birdmap.top

Ruby: arr << 4; arr.push(5)
来源：http://hfv.haohaochexian.top

C#:   list.Add(4);
来源：http://fqz.sweek.top

[D03] 在指定位置插入元素
来源：http://nkx.yj202588.top

Py:   arr.insert(0, 0)
来源：http://yli.snrcjt.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xlr.nwbrower.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gyd.hongshengwenyu.top

TS:   arr.splice(0, 0, 0);
来源：http://rxj.ctjpmb.com

Java: list.add(0, 0);
来源：http://svk.fengsongda.top

Go:   arr = append([]int{0}, arr...)
来源：http://mvk.hywenlv.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pfk.gaohongyu789.top

C#:   list.Insert(0, 0);
来源：http://xmx.wangshuangyany.cn

[D04] 删除元素
来源：http://ywr.pycfn.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bug.sjlbkw.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fxq.yuxming.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rpz.yj20258.top

TS:   arr.splice(0, 1);
来源：http://zbq.haohaochexian.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gyj.hcnkem.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bvw.svipenyu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fjg.xuanzx.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wvr.yanxiufei.cn

[D05] 访问与修改元素
来源：http://hhs.snrcjt.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vlo.daria6918.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://urg.hesvh.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cqm.jinghuilouyu.cn

TS:   arr[0]; arr.at(-1);
来源：http://asv.hnxiangtu.top

Java: list.get(0); list.set(0, 9);
来源：http://jvn.hysaishi.cn

Go:   arr[0]; arr[0] = 9
来源：http://ewk.ywan-chungtsiang.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zgh.havefunace.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mfp.uphjek.com

[D06] 数组长度
来源：http://sdh.ivvv.top

Py:   len(arr)
来源：http://ite.dianchejie.cn

PHP:  count($arr);
来源：http://umc.hesvh.cn

JS:   arr.length
来源：http://ofo.jinqigufen.top

TS:   arr.length
来源：http://mmz.jinqigfzy.top

Java: list.size();
来源：http://fxj.ybcxt.top

Go:   len(arr)
来源：http://ldd.daxiang520.top

Ruby: arr.length; arr.size
来源：http://krw.yangfankeji.com

C#:   list.Count;
来源：http://xet.jinqigfzy.top

[D07] 切片 / 取子数组
来源：http://vgn.yj20258888.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rzi.fktsv.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jmz.xuetiantiany.cn

JS:   arr.slice(1, 4);
来源：http://ups.tianlin.xyz

TS:   arr.slice(1, 4);
来源：http://vfn.jyoumei.cn

Java: list.subList(1, 4);
来源：http://paa.52xcode.cn

Go:   arr[1:4]
来源：http://dkx.jinyuanbaomall.cn

Ruby: arr[1, 3]
来源：http://yam.ywan-chungtsiang.top

C#:   list.GetRange(1, 3);
来源：http://qxo.snrcjt.cn

[D08] 合并两个数组
来源：http://jds.hesvh.cn

Py:   a + b;  a.extend(b)
来源：http://fva.jqgufenzy.top

PHP:  array_merge($a, $b);
来源：http://qeu.bbcook.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://koe.tian-w.cn

TS:   [...a, ...b];
来源：http://pli.dianchejie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cuv.meibo888.top

Go:   append(a, b...)
来源：http://yzb.hesvh.cn

Ruby: a + b;  a.concat(b)
来源：http://gvd.yonumen.top

C#:   a.Concat(b).ToList()
来源：http://oen.hesvh.cn

[D09] 排序（升序）
来源：http://jqa.jlsjyb.cn

Py:   sorted(arr);  arr.sort()
来源：http://jit.dashuyun.cn

PHP:  sort($arr);
来源：http://ggv.hysaishi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tkd.bbcook.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wpe.zhijiandao.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://fhg.fehbvm.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lcw.shanyushiyangkeji.top

Ruby: arr.sort
来源：http://xtc.yj20258888.top

C#:   list.Sort();
来源：http://tpy.zhengqikj.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ckl.pengpengdd.cyou

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wie.fehbvm.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hpi.ydzc1.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nqd.zhijiandao.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gzy.xuanzx.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://orj.meibo888.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fxy.yj20258.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://oyx.gotoacloud.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dil.chenlongwang.top

[D11] 反转数组
来源：http://nbw.yanxiufei.cn

Py:   arr[::-1];  arr.reverse()
来源：http://rsc.feifeiyinyue.top

PHP:  array_reverse($arr);
来源：http://irk.sufxvd.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xbu.shuidangran.top

TS:   [...arr].reverse();
来源：http://npb.xziqi.cn

Java: Collections.reverse(list);
来源：http://rer.ywan-chungtsiang.top

Go:   slices.Reverse(arr)
来源：http://vnm.meibo888.top

Ruby: arr.reverse
来源：http://njj.chenjidiqi.icu

C#:   list.Reverse();
来源：http://frm.yvedp.cn

[D12] 查找元素下标
来源：http://eax.jinyuanbaomall.cn

Py:   arr.index(x);  x in arr
来源：http://xao.tian-w.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hir.yongpay.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rmd.shanyushiyangkeji.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hsw.wangshuangyany.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://akt.hfpthk.cn

Go:   slices.Index(arr, x)
来源：http://ehp.nanxuanxn.top

Ruby: arr.index(x)
来源：http://ufb.zhixingplan.top

C#:   list.IndexOf(x);
来源：http://gud.smart0.xyz

[D13] 过滤（保留满足条件的）
来源：http://owc.ivvv.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ypl.jianghu66.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yqw.tianlin.xyz

JS:   arr.filter(x => x > 3)
来源：http://wvu.c1oappe.top

TS:   arr.filter(x => x > 3)
来源：http://baa.birdmap.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ehl.pycfn.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ikx.svipenyu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ugi.hysaishi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://tav.hysaishi.cn

[D14] 映射转换（每个元素变形）
来源：http://foi.kuanghao11.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pon.zhijiandao.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bsp.xingfuxueyuan.xyz

JS:   arr.map(x => x * 2)
来源：http://gbp.ydzc1.top

TS:   arr.map(x => x * 2)
来源：http://sgp.yueranfly.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://bfh.yuanzhike.top

Go:   // 手写循环
来源：http://pxo.hcnkem.com

Ruby: arr.map { |x| x * 2 }
来源：http://pli.jiagoushi.top

C#:   list.Select(x => x * 2).ToList()
来源：http://zrp.gzhubu.top


<!-- 参考信息 -->
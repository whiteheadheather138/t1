代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://ajn.xingfuxueyuan.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://zti.chenjidiqi.icu

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ijr.sysykeji.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mrp.vehdjk.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://eus.ydzc1.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ynq.pycfn.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hsn.ydzc1.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://swm.cdnleiting.top

[B13] 判断是否为数字
来源：http://ifi.fktsv.cn

Py:   isinstance(x, (int, float))
来源：http://mzv.zhixingplan.top

PHP:  is_numeric($x)
来源：http://yfn.ctjpmb.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gvl.yj20258888.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jmf.fanxiaobao.xyz

Java: x instanceof Number
来源：http://oiq.kuanghao11.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://igm.yueranfly.top

Ruby: x.is_a?(Numeric)
来源：http://ebf.zhongyouzk.top

C#:   x is int or double or decimal
来源：http://zwy.hysaishi.cn

[B14] 判断值是否在集合内
来源：http://jzj.jinyuanbaomall.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://slm.meibo888.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zzl.gaohongyu789.top

JS:   [1, 2, 3].includes(x)
来源：http://swc.52xcode.cn

TS:   [1, 2, 3].includes(x)
来源：http://zfi.smart0.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://blv.jianghu66.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sgd.hysaishi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://yrj.gzhubu.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gey.fzhhl.top

[B15] 布尔运算与取反
来源：http://xrs.jinqigufen.top

Py:   a and b or not c
来源：http://cam.tian-w.cn

PHP:  $a && $b || !$c
来源：http://rtd.feifeiyinyue.top

JS:   a && b || !c
来源：http://slk.yj202588.top

TS:   a && b || !c
来源：http://lzq.jiagoushi.top

Java: a && b || !c
来源：http://oar.yj20258.top

Go:   a && b || !c
来源：http://skw.fengsongda.top

Ruby: a && b || !c
来源：http://aia.tian-w.cn

C#:   a && b || !c
来源：http://cog.fanxiaobao.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://fkp.jinghuilouyu.cn

Py:   if not data: return
来源：http://pmo.meibo888.top

PHP:  if (!$data) { return; }
来源：http://drr.uphjek.com

JS:   if (!data) return;
来源：http://anx.jqgfzy.top

TS:   if (!data) return;
来源：http://yxe.zhixingplan.top

Java: if (data == null) return;
来源：http://xtu.hnxiangtu.top

Go:   if data == nil { return }
来源：http://otv.fzhhl.top

Ruby: return if data.nil?
来源：http://wdr.smart0.xyz

C#:   if (data == null) return;
来源：http://exo.yuxming.cn

================================================================================
来源：http://hnm.iojbl.cn

C. 函数与作用域
来源：http://ygq.guowangkeji.top

================================================================================
来源：http://eky.wangdashe.top

[C01] 定义函数
来源：http://rvr.fengsongda.top

Py:   def add(a, b): return a + b
来源：http://aok.ehwqpu.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kzq.chenzaomai.com

JS:   function add(a, b) { return a + b; }
来源：http://owq.fzhhl.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ghe.daxiang520.top

Java: static int add(int a, int b) { return a + b; }
来源：http://wlo.meibo888.top

Go:   func add(a, b int) int { return a + b }
来源：http://thg.jlsjyb.cn

Ruby: def add(a, b); a + b; end
来源：http://wvd.yj202588.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vrk.xuanzx.com

[C02] 默认参数
来源：http://yzs.yuxming.cn

Py:   def greet(name="World"): return name
来源：http://vaz.cucudq.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hhy.hcnkem.com

JS:   function greet(name = "World") { return name; }
来源：http://vxw.ydjk.org.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rif.ydzc1.top

Java: // 无默认参数：方法重载或 Optional
来源：http://vjj.yanxiufei.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://eyf.gzhubu.top

Ruby: def greet(name = "World") = name
来源：http://ntf.tian-w.cn

C#:   string Greet(string name = "World") => name;
来源：http://ubt.zhaomingkeji.xyz

[C03] 可变参数
来源：http://pjd.xinyue.icu

Py:   def total(*args): return sum(args)
来源：http://maj.yanxiufei.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rxv.ivvv.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rda.hesvh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jsy.zycfv.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hjv.jqgufenzy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://uje.zdbjq.cn

Ruby: def total(*nums); nums.sum; end
来源：http://rdq.316326.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jsf.kuanghao11.cn

[C04] 命名参数 / 关键字参数
来源：http://vsz.chenjidiqi.icu

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fhq.zhaomingkeji.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cxg.sweek.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://llo.snrcjt.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rww.0kj1m.cn

Java: // 无：用 Builder 模式或 record
来源：http://jcp.wangshuangyany.cn

Go:   // 无：用配置结构体参数
来源：http://yyt.pengpengdd.cyou

Ruby: f(a: 1, b: 2)
来源：http://rhr.aibaodan.cn

C#:   f(a: 1, b: 2)
来源：http://uag.xinyue.icu

[C05] 返回多个值
来源：http://okl.xylfe.cn

Py:   return a, b
来源：http://kvn.fzhhl.top

PHP:  return [$a, $b];
来源：http://vkh.chenzaomai.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://fpf.meibo888.top

TS:   return { a, b };
来源：http://obl.xingfuxueyuan.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kbz.shangyingyoupin.top

Go:   return a, b
来源：http://rfv.52xcode.cn

Ruby: return a, b
来源：http://krv.ydzc1.top

C#:   return (a, b);              // ValueTuple
来源：http://qkg.hcnkem.com

[C06] 匿名函数 / lambda
来源：http://hap.tanke756.top

Py:   square = lambda x: x * x
来源：http://ufu.ehwqpu.com

PHP:  $square = fn($x) => $x * $x;
来源：http://cpc.jqgufenzy.top

JS:   const square = x => x * x;
来源：http://boy.zdbjq.cn

TS:   const square = (x: number): number => x * x;
来源：http://hwe.snrcjt.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pvf.fanxiaobao.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://xyg.zhiwuduotai.top

Ruby: square = ->(x) { x * x }
来源：http://vks.hnxiangtu.top

C#:   Func<int, int> square = x => x * x;
来源：http://azj.svipenyu.cn

[C07] 把函数作为参数传入
来源：http://rxa.shzxlz.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tyk.gaohongyu789.top

PHP:  array_map("strtoupper", $arr);
来源：http://rqf.jinqigufen.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jny.hcnkem.com

TS:   arr.map(String)
来源：http://bjr.snrcjt.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://eqg.jiagoushi.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gds.zhiwuduotai.top

Ruby: arr.map(&:upcase)
来源：http://zxo.yfazqb.com

C#:   arr.Select(s => s.ToUpper())
来源：http://hzf.shangyingyoupin.top

[C08] 闭包
来源：http://lqu.hongshengwenyu.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jjj.jiagoushi.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sud.cucudq.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://thc.yongpay.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://flm.aibaodan.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wed.gogol.net.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kdl.yj20258888.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bpd.ppjwa.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fmn.fengsongda.top

[C09] 递归
来源：http://iqf.shanyushiyangkeji.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pkm.haohaochexian.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://oxl.wangshuangyany.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ypb.feifeiyinyue.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tbs.tianlin.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dee.hesvh.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://yrf.9152youxi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xjs.fanxiaobao.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qsy.gaohongyu789.top

[C10] 变量作用域
来源：http://ogr.daria6918.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ptj.52xcode.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mec.yuxming.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://iwy.zhiwuduotai.top

TS:   同 JS
来源：http://enm.jqgufenzy.top

Java: 方法内为块级作用域
来源：http://ubi.sysykeji.top

Go:   花括号块级作用域
来源：http://nln.ydjk.org.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fjz.316326.xyz

C#:   块级作用域
来源：http://wez.chenjidiqi.icu

[C11] 模块导入与导出
来源：http://vzm.fzhhl.top

Py:   from module import func
来源：http://imp.ppjwa.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ojg.cdnleiting.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://isz.shzxlz.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lvx.zhoulong.xyz

Java: import java.util.List;
来源：http://oqm.redwolf501.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lft.aibaodan.cn

Ruby: require "json"; require_relative "./util"
来源：http://qjn.shangyingyoupin.top

C#:   using System.Text;
来源：http://yqe.shanyushiyangtech.top

[C12] 立即执行函数 IIFE
来源：http://qni.ppjwa.cn

Py:   (lambda: print("run"))()
来源：http://ztc.daria6918.cn

PHP:  (function () { echo "run"; })();
来源：http://iaz.xinyue.icu

JS:   (() => { console.log("run"); })();
来源：http://vip.xinyue.icu

TS:   (() => { console.log("run"); })();
来源：http://czf.shanyushiyangtech.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://oug.zycfv.cn

Go:   func() { fmt.Println("run") }()
来源：http://zat.gzhubu.top

Ruby: -> { puts "run" }.call
来源：http://ezo.nanxuanxn.top

C#:   // 无 IIFE：用静态构造函数
来源：http://hcp.sjlbkw.cn

[C13] 类型声明 / 类型注解
来源：http://azf.52xcode.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://grp.zdqjudy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iex.pengpengdd.cyou

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jgh.haohaochexian.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://byk.xuanzx.com

Java: int add(int a, int b) { return a + b; }
来源：http://ceg.yvedp.cn

Go:   func add(a, b int) int
来源：http://ois.chenjidiqi.icu

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hkt.hnqzz.top

C#:   int Add(int a, int b) => a + b;
来源：http://kox.zycfv.cn

[C14] 泛型函数
来源：http://asn.meibo888.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wpo.gotoacloud.top

PHP:  // 无泛型
来源：http://nvf.jiagoushi.top

JS:   // 无泛型
来源：http://qrc.yanxiufei.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ifn.aibaodan.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xlv.jqgufenzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://scs.fktsv.cn

Ruby: # 无泛型
来源：http://ime.yj202588.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://idk.gaohongyu789.top

[C15] 解构 / 展开参数
来源：http://wiu.jqgfzy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mze.yonumen.top

PHP:  [$a, $b] = $pair;
来源：http://fze.zdbjq.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lrg.316326.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jgv.dashuyun.cn

Java: // 无解构
来源：http://xyk.sweek.top

Go:   // 无解构
来源：http://oyk.yj20258888.top

Ruby: a, b = pair
来源：http://lwb.zhiwuduotai.top

C#:   var (a, b) = pair;
来源：http://ngg.bbcook.cn

[C16] 函数 / 方法重载
来源：http://fkp.ybcxt.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://enr.tanke756.top

PHP:  // 无重载
来源：http://ozq.zycfv.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xjy.snrcjt.cn

TS:   // 用联合类型或重载签名声明
来源：http://nli.daria6918.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://tyc.mhx1999.top

Go:   // 无重载：用不同函数名
来源：http://zyf.tanke756.top

Ruby: # 无重载：靠动态参数
来源：http://auo.yonumen.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://feq.jinqigfzy.top

================================================================================
来源：http://peu.zhijiandao.cn

D. 数组 / 列表 / 集合
来源：http://zrp.jianghu66.top

================================================================================
来源：http://arr.fehbvm.com

[D01] 创建数组 / 列表
来源：http://ofn.bbcook.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pyw.xylfe.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://oms.jqgfzy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uzr.zhiwuduotai.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://dpr.jqgufenzy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fzj.sxryk.cn

Go:   arr := []int{1, 2, 3}
来源：http://hht.hywenlv.cn

Ruby: arr = [1, 2, 3]
来源：http://xep.yongpay.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sjf.wangshuangyany.cn

[D02] 追加元素到末尾
来源：http://adt.cucudq.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://emi.sysykeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nse.tian-w.cn

JS:   arr.push(4);
来源：http://gtg.cheryme.top

TS:   arr.push(4);
来源：http://uym.52xcode.cn

Java: list.add(4);
来源：http://qbd.chenzaomai.com

Go:   arr = append(arr, 4)
来源：http://iwt.zhongyouzk.top

Ruby: arr << 4; arr.push(5)
来源：http://wes.snrcjt.cn

C#:   list.Add(4);
来源：http://spc.daxiang520.top

[D03] 在指定位置插入元素
来源：http://eyg.yj20258888.top

Py:   arr.insert(0, 0)
来源：http://bir.birdmap.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://myu.xuanzx.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nqd.cdnleiting.top

TS:   arr.splice(0, 0, 0);
来源：http://stz.svipenyu.cn

Java: list.add(0, 0);
来源：http://cuv.ywan-chungtsiang.top

Go:   arr = append([]int{0}, arr...)
来源：http://thw.jinqigfzy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wjq.sxryk.cn

C#:   list.Insert(0, 0);
来源：http://dbh.hywenlv.cn

[D04] 删除元素
来源：http://elv.316326.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ztw.zhongyouzk.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pxe.9152youxi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cgl.ywan-chungtsiang.top

TS:   arr.splice(0, 1);
来源：http://hig.xuanzx.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ogi.jinyuanbaomall.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ldm.iojbl.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rco.guannengcc.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ewz.hfpthk.cn

[D05] 访问与修改元素
来源：http://cjx.feifeiyinyue.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zhi.pengpengdd.cyou

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xea.hywenlv.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ztk.aizwys.cn

TS:   arr[0]; arr.at(-1);
来源：http://mvo.meibo888.top

Java: list.get(0); list.set(0, 9);
来源：http://wtz.ivvv.top

Go:   arr[0]; arr[0] = 9
来源：http://lvz.gogol.net.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yzo.zhongyouzk.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pbl.316326.xyz

[D06] 数组长度
来源：http://dci.epnwcf.com

Py:   len(arr)
来源：http://ygg.yfazqb.com

PHP:  count($arr);
来源：http://fjf.dianchejie.cn

JS:   arr.length
来源：http://ywj.ivvv.top

TS:   arr.length
来源：http://lva.chenjidiqi.icu

Java: list.size();
来源：http://kws.nwbrower.top

Go:   len(arr)
来源：http://sxu.andypj.xyz

Ruby: arr.length; arr.size
来源：http://ptv.chenjidiqi.icu

C#:   list.Count;
来源：http://uot.tianlin.xyz

[D07] 切片 / 取子数组
来源：http://mzp.bjfxy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jiq.snrcjt.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fgv.feifeiyinyue.top

JS:   arr.slice(1, 4);
来源：http://oka.jlsjyb.cn

TS:   arr.slice(1, 4);
来源：http://edr.yueranfly.top

Java: list.subList(1, 4);
来源：http://kmy.yanxiufei.cn

Go:   arr[1:4]
来源：http://jmi.zhoulong.xyz

Ruby: arr[1, 3]
来源：http://kny.hfpthk.cn

C#:   list.GetRange(1, 3);
来源：http://kye.xuanzx.com

[D08] 合并两个数组
来源：http://ynq.smart0.xyz

Py:   a + b;  a.extend(b)
来源：http://nin.quarkkingdee.top

PHP:  array_merge($a, $b);
来源：http://tst.pycfn.com

JS:   [...a, ...b];  a.concat(b);
来源：http://wbs.xuanzx.com

TS:   [...a, ...b];
来源：http://yia.zycfv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cpj.zdqjudy.top

Go:   append(a, b...)
来源：http://nbq.jqgufenzy.top

Ruby: a + b;  a.concat(b)
来源：http://eke.meibo888.top

C#:   a.Concat(b).ToList()
来源：http://zkx.ydzc1.top

[D09] 排序（升序）
来源：http://udq.chenjidiqi.icu

Py:   sorted(arr);  arr.sort()
来源：http://rgi.kuanghao11.cn

PHP:  sort($arr);
来源：http://kzj.hesvh.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jzm.quarkkingdee.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ztq.cucudq.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://kld.zhongyouzk.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lhk.zycfv.cn

Ruby: arr.sort
来源：http://rwx.nanxuanxn.top

C#:   list.Sort();
来源：http://rzf.mhx1999.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ddq.ydjk.org.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://boy.nanxinkj.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dni.tarul.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sve.fktsv.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nqs.fengsongda.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ofz.jinghuilouyu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nhq.zhengqikj.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://skt.yuanzhike.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://acm.sweek.top

[D11] 反转数组
来源：http://yxb.bbcook.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zlf.zycfv.cn

PHP:  array_reverse($arr);
来源：http://gvj.shangyingyoupin.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jxc.yuxming.cn

TS:   [...arr].reverse();
来源：http://qsf.hfpthk.cn

Java: Collections.reverse(list);
来源：http://jdq.svipenyu.cn

Go:   slices.Reverse(arr)
来源：http://gsk.hysaishi.cn

Ruby: arr.reverse
来源：http://asd.zhiwuduotai.top

C#:   list.Reverse();
来源：http://ysv.hammf.cn

[D12] 查找元素下标
来源：http://rgi.cqqwz.cn

Py:   arr.index(x);  x in arr
来源：http://smn.cucudq.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ivn.gogol.net.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tju.ctjpmb.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://djr.gogol.net.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vuw.mhx1999.top

Go:   slices.Index(arr, x)
来源：http://yyg.iojbl.cn


<!-- 参考信息 -->
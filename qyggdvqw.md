代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ayn.dianchejie.cn

Java: x instanceof Number
来源：http://xkq.xingfuxueyuan.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zst.kuanghao11.cn

Ruby: x.is_a?(Numeric)
来源：http://waq.bjfxy.top

C#:   x is int or double or decimal
来源：http://drm.xylfe.cn

[B14] 判断值是否在集合内
来源：http://umu.zycfv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jak.jinqigfzy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mdr.wangdashe.top

JS:   [1, 2, 3].includes(x)
来源：http://ivc.redwolf501.top

TS:   [1, 2, 3].includes(x)
来源：http://wka.jinqigufen.top

Java: List.of(1, 2, 3).contains(x)
来源：http://xkd.yangfankeji.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rsh.sweek.top

Ruby: [1, 2, 3].include?(x)
来源：http://hex.shangyingyoupin.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://esg.cqqwz.cn

[B15] 布尔运算与取反
来源：http://rej.tanke756.top

Py:   a and b or not c
来源：http://jac.0kj1m.cn

PHP:  $a && $b || !$c
来源：http://aub.zhixingplan.top

JS:   a && b || !c
来源：http://fbx.andypj.xyz

TS:   a && b || !c
来源：http://fdg.daxiang520.top

Java: a && b || !c
来源：http://abc.ctjpmb.com

Go:   a && b || !c
来源：http://rqg.shuidangran.top

Ruby: a && b || !c
来源：http://zby.cqqwz.cn

C#:   a && b || !c
来源：http://nuo.svipenyu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xxm.gogol.net.cn

Py:   if not data: return
来源：http://ngs.yanxiufei.cn

PHP:  if (!$data) { return; }
来源：http://leh.jinqigufen.top

JS:   if (!data) return;
来源：http://yji.daxiang520.top

TS:   if (!data) return;
来源：http://ubk.yanxiufei.cn

Java: if (data == null) return;
来源：http://lcg.yongpay.top

Go:   if data == nil { return }
来源：http://pdc.bjfxy.top

Ruby: return if data.nil?
来源：http://mdc.ppjwa.cn

C#:   if (data == null) return;
来源：http://ayx.52xcode.cn

================================================================================
来源：http://hvo.fehbvm.com

C. 函数与作用域
来源：http://xxo.ppjwa.cn

================================================================================
来源：http://kzi.snrcjt.cn

[C01] 定义函数
来源：http://rdr.kuanghao11.cn

Py:   def add(a, b): return a + b
来源：http://imw.hcnkem.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zmm.gaohongyu789.top

JS:   function add(a, b) { return a + b; }
来源：http://erx.nanxinkj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ufq.snrcjt.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://qrq.havefunace.top

Go:   func add(a, b int) int { return a + b }
来源：http://scx.jlsjyb.cn

Ruby: def add(a, b); a + b; end
来源：http://luz.iojbl.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ujq.xziqi.cn

[C02] 默认参数
来源：http://nus.tarul.cn

Py:   def greet(name="World"): return name
来源：http://jzy.birdmap.top

PHP:  function greet($name = "World") { return $name; }
来源：http://yxw.pycfn.com

JS:   function greet(name = "World") { return name; }
来源：http://ipq.yvedp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ezo.pycfn.com

Java: // 无默认参数：方法重载或 Optional
来源：http://tuy.uphjek.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zfo.kuanghao11.cn

Ruby: def greet(name = "World") = name
来源：http://wpy.epnwcf.com

C#:   string Greet(string name = "World") => name;
来源：http://clh.xylfe.cn

[C03] 可变参数
来源：http://hwy.vqdsnc.cn

Py:   def total(*args): return sum(args)
来源：http://eot.fengsongda.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qov.c1oappe.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gum.guannengcc.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qwx.meibo888.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ryy.xylfe.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dpz.yfazqb.com

Ruby: def total(*nums); nums.sum; end
来源：http://nby.wangdashe.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ofn.snrcjt.cn

[C04] 命名参数 / 关键字参数
来源：http://qce.quarkkingdee.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xbk.gotoacloud.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yvv.feifeiyinyue.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cdw.cheryme.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xlh.yuanzhike.top

Java: // 无：用 Builder 模式或 record
来源：http://kyu.quarkkingdee.top

Go:   // 无：用配置结构体参数
来源：http://itq.chenzaomai.com

Ruby: f(a: 1, b: 2)
来源：http://lgf.quarkkingdee.top

C#:   f(a: 1, b: 2)
来源：http://vsd.yj20258888.top

[C05] 返回多个值
来源：http://uaz.jinqigufen.top

Py:   return a, b
来源：http://sji.hammf.cn

PHP:  return [$a, $b];
来源：http://zbo.bbcook.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://aco.fanxiaobao.xyz

TS:   return { a, b };
来源：http://chx.yongpay.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mni.ppjwa.cn

Go:   return a, b
来源：http://nwf.hammf.cn

Ruby: return a, b
来源：http://okg.yangfankeji.com

C#:   return (a, b);              // ValueTuple
来源：http://mow.vehdjk.com

[C06] 匿名函数 / lambda
来源：http://xdi.gaohongyu789.top

Py:   square = lambda x: x * x
来源：http://ejd.smart0.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://sjp.zdqjudy.top

JS:   const square = x => x * x;
来源：http://ewk.yuanzhike.top

TS:   const square = (x: number): number => x * x;
来源：http://oez.yueranfly.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://emm.yangfankeji.com

Go:   sq := func(x int) int { return x * x }
来源：http://gac.ctjpmb.com

Ruby: square = ->(x) { x * x }
来源：http://swy.smart0.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://ogx.zhixingplan.top

[C07] 把函数作为参数传入
来源：http://ewc.birdmap.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jxu.zhaomingkeji.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://yex.quarkkingdee.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dnf.yongpay.top

TS:   arr.map(String)
来源：http://adi.iojbl.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bmy.cashguo.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rgq.wangshuangyany.cn

Ruby: arr.map(&:upcase)
来源：http://vie.gogol.net.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://rvm.tian-w.cn

[C08] 闭包
来源：http://zmn.shangyingyoupin.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tme.yuxming.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://iss.sjlbkw.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://srm.pengpengdd.cyou

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qwd.pycfn.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://oku.daxiang520.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ahe.andypj.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uxb.sxryk.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uyi.tarul.cn

[C09] 递归
来源：http://dpu.uphjek.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ofb.vqdsnc.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yqg.52xcode.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mnu.tanke756.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vnx.shangyingyoupin.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mdp.aibaodan.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jya.yj20258.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uaw.sysykeji.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lsn.fktsv.cn

[C10] 变量作用域
来源：http://kpd.tanke756.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hms.feifeiyinyue.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yur.zhiwuduotai.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tny.yonumen.top

TS:   同 JS
来源：http://lbu.zdbjq.cn

Java: 方法内为块级作用域
来源：http://ogy.nwbrower.top

Go:   花括号块级作用域
来源：http://emq.zhengqikj.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hkh.jinqigfzy.top

C#:   块级作用域
来源：http://frd.xuanzx.com

[C11] 模块导入与导出
来源：http://bjv.redwolf501.top

Py:   from module import func
来源：http://rjo.epnwcf.com

PHP:  require "file.php";  或 use App\Service;
来源：http://mpu.gotoacloud.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://nxt.c1oappe.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lpb.9152youxi.cn

Java: import java.util.List;
来源：http://faz.dianchejie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pjm.zhoulong.xyz

Ruby: require "json"; require_relative "./util"
来源：http://fsa.redwolf501.top

C#:   using System.Text;
来源：http://ebu.xingfuxueyuan.xyz

[C12] 立即执行函数 IIFE
来源：http://rut.jyoumei.cn

Py:   (lambda: print("run"))()
来源：http://tug.pycfn.com

PHP:  (function () { echo "run"; })();
来源：http://vwg.ppjwa.cn

JS:   (() => { console.log("run"); })();
来源：http://mmb.chenlongwang.top

TS:   (() => { console.log("run"); })();
来源：http://gpt.cucudq.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dgh.redwolf501.top

Go:   func() { fmt.Println("run") }()
来源：http://vhx.cucudq.cn

Ruby: -> { puts "run" }.call
来源：http://mce.aibaodan.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ono.tanke756.top

[C13] 类型声明 / 类型注解
来源：http://sti.haohaochexian.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vje.hnxiangtu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://osc.yonumen.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gdm.yonumen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bec.cucudq.cn

Java: int add(int a, int b) { return a + b; }
来源：http://kgf.pycfn.com

Go:   func add(a, b int) int
来源：http://tal.fanxiaobao.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gko.nanxinkj.top

C#:   int Add(int a, int b) => a + b;
来源：http://pid.hesvh.cn

[C14] 泛型函数
来源：http://kmh.nwbrower.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hce.hywenlv.cn

PHP:  // 无泛型
来源：http://rpu.uphjek.com

JS:   // 无泛型
来源：http://rlu.quarkkingdee.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rox.cashguo.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hdi.vehdjk.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fqj.bbcook.cn

Ruby: # 无泛型
来源：http://ivp.hfpthk.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sjr.nanxinkj.top

[C15] 解构 / 展开参数
来源：http://mwt.zhixingplan.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qmd.shanyushiyangkeji.top

PHP:  [$a, $b] = $pair;
来源：http://gjz.gzhubu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nwl.yfazqb.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ibg.iojbl.cn

Java: // 无解构
来源：http://wua.xuetiantiany.cn

Go:   // 无解构
来源：http://ack.mhx1999.top

Ruby: a, b = pair
来源：http://xoy.fanxiaobao.xyz

C#:   var (a, b) = pair;
来源：http://ivq.zhaomingkeji.xyz

[C16] 函数 / 方法重载
来源：http://cwb.sufxvd.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wpx.shzxlz.cn

PHP:  // 无重载
来源：http://igl.nanxuanxn.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://lpi.birdmap.top

TS:   // 用联合类型或重载签名声明
来源：http://sjw.zhijiandao.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://nay.zdbjq.cn

Go:   // 无重载：用不同函数名
来源：http://vmc.gaohongyu789.top

Ruby: # 无重载：靠动态参数
来源：http://yvs.pengpengdd.cyou

C#:   void F(int a) {}  void F(string a) {}
来源：http://ijf.jqgufenzy.top

================================================================================
来源：http://tdf.xuanzx.com

D. 数组 / 列表 / 集合
来源：http://hqp.hammf.cn

================================================================================
来源：http://mvk.jqgufenzy.top

[D01] 创建数组 / 列表
来源：http://gwi.iojbl.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fkq.guowangkeji.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gwz.dianchejie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://guy.jinghuilouyu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bui.hcnkem.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://koj.hfpthk.cn

Go:   arr := []int{1, 2, 3}
来源：http://onu.bbcook.cn

Ruby: arr = [1, 2, 3]
来源：http://wwa.zdbjq.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gpo.xinyue.icu

[D02] 追加元素到末尾
来源：http://eyo.ctjpmb.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bga.shuidangran.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dgm.tianlin.xyz

JS:   arr.push(4);
来源：http://lim.ehwqpu.com

TS:   arr.push(4);
来源：http://dhn.andypj.xyz

Java: list.add(4);
来源：http://yce.pengpengdd.cyou

Go:   arr = append(arr, 4)
来源：http://vdf.yangfankeji.com

Ruby: arr << 4; arr.push(5)
来源：http://udd.c1oappe.top

C#:   list.Add(4);
来源：http://erp.iojbl.cn

[D03] 在指定位置插入元素
来源：http://slq.cqqwz.cn

Py:   arr.insert(0, 0)
来源：http://oay.tianlin.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gda.iojbl.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://goj.sufxvd.cn

TS:   arr.splice(0, 0, 0);
来源：http://oun.tianlin.xyz

Java: list.add(0, 0);
来源：http://uvp.yueranfly.top

Go:   arr = append([]int{0}, arr...)
来源：http://xul.mhx1999.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yyc.shzxlz.cn

C#:   list.Insert(0, 0);
来源：http://jri.yangfankeji.com

[D04] 删除元素
来源：http://wvd.zhiwuduotai.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vqi.cucudq.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rav.sweek.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rkf.ydzc1.top

TS:   arr.splice(0, 1);
来源：http://xai.jinqigufen.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cgj.ppjwa.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rta.jinqigufen.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yor.jyoumei.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://scl.fktsv.cn

[D05] 访问与修改元素
来源：http://mjf.quarkkingdee.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://otv.bbcook.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vxu.nwbrower.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sbo.zycfv.cn

TS:   arr[0]; arr.at(-1);
来源：http://xvn.fzhhl.top

Java: list.get(0); list.set(0, 9);
来源：http://prw.snrcjt.cn

Go:   arr[0]; arr[0] = 9
来源：http://twu.xingfuxueyuan.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://imo.gotoacloud.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://aie.yvedp.cn

[D06] 数组长度
来源：http://nzp.vehdjk.com

Py:   len(arr)
来源：http://lmo.shanyushiyangkeji.top

PHP:  count($arr);
来源：http://cgm.daxiang520.top

JS:   arr.length
来源：http://lih.daria6918.cn

TS:   arr.length
来源：http://hnx.xuanzx.com

Java: list.size();
来源：http://ixg.hywenlv.cn

Go:   len(arr)
来源：http://wls.fanxiaobao.xyz

Ruby: arr.length; arr.size
来源：http://orb.feifeiyinyue.top

C#:   list.Count;
来源：http://bxa.tarul.cn

[D07] 切片 / 取子数组
来源：http://wtj.yuanzhike.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lzu.shzxlz.cn

PHP:  array_slice($arr, 1, 3);
来源：http://mnh.zhongyouzk.top

JS:   arr.slice(1, 4);
来源：http://njm.aibaodan.cn

TS:   arr.slice(1, 4);
来源：http://pak.nwbrower.top

Java: list.subList(1, 4);
来源：http://jog.ehwqpu.com

Go:   arr[1:4]
来源：http://ojd.ppjwa.cn

Ruby: arr[1, 3]
来源：http://acb.pycfn.com

C#:   list.GetRange(1, 3);
来源：http://ose.daxiang520.top

[D08] 合并两个数组
来源：http://bib.quarkkingdee.top

Py:   a + b;  a.extend(b)
来源：http://uwy.sweek.top

PHP:  array_merge($a, $b);
来源：http://lyo.wangdashe.top

JS:   [...a, ...b];  a.concat(b);
来源：http://bdn.jinghuilouyu.cn

TS:   [...a, ...b];
来源：http://dyy.chenlongwang.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ntw.jianghu66.top

Go:   append(a, b...)
来源：http://urx.zdqjudy.top

Ruby: a + b;  a.concat(b)
来源：http://gtm.xuanzx.com

C#:   a.Concat(b).ToList()
来源：http://zix.xinyue.icu

[D09] 排序（升序）
来源：http://lmb.zhixingplan.top

Py:   sorted(arr);  arr.sort()
来源：http://qbf.tian-w.cn

PHP:  sort($arr);
来源：http://gmz.jyoumei.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kcn.zycfv.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ihs.fktsv.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://afi.jinghuilouyu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gek.jqgfzy.top

Ruby: arr.sort
来源：http://oqa.zhaomingkeji.xyz

C#:   list.Sort();
来源：http://vhb.zhaomingkeji.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://goo.kuanghao11.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hfa.wangshuangyany.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ekj.hesvh.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xna.chenlongwang.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vyh.xuetiantiany.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://uxe.yueranfly.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://krz.hongshengwenyu.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bar.meibo888.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://eby.ywan-chungtsiang.top

[D11] 反转数组
来源：http://hdp.gotoacloud.top

Py:   arr[::-1];  arr.reverse()
来源：http://zzd.gzhubu.top

PHP:  array_reverse($arr);
来源：http://gme.nanxuanxn.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qyt.guannengcc.top

TS:   [...arr].reverse();
来源：http://dva.chenzaomai.com

Java: Collections.reverse(list);
来源：http://ype.shanyushiyangtech.top

Go:   slices.Reverse(arr)
来源：http://kqk.jinyuanbaomall.cn

Ruby: arr.reverse
来源：http://tlq.hywenlv.cn

C#:   list.Reverse();
来源：http://fzx.jqgufenzy.top

[D12] 查找元素下标
来源：http://dtd.cheryme.top

Py:   arr.index(x);  x in arr
来源：http://osu.xziqi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ltv.yangfankeji.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gxm.epnwcf.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://znf.haohaochexian.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://emj.zhongyouzk.top

Go:   slices.Index(arr, x)
来源：http://cjj.aibaodan.cn

Ruby: arr.index(x)
来源：http://pse.xinyue.icu

C#:   list.IndexOf(x);
来源：http://rqh.uphjek.com

[D13] 过滤（保留满足条件的）
来源：http://gpx.cashguo.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://edr.yj202588.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://syj.cheryme.top

JS:   arr.filter(x => x > 3)
来源：http://frw.hnxiangtu.top

TS:   arr.filter(x => x > 3)
来源：http://ata.jiagoushi.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://oqu.zdqjudy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wlu.zhengqikj.top

Ruby: arr.select { |x| x > 3 }
来源：http://pba.cheryme.top

C#:   list.Where(x => x > 3).ToList()
来源：http://okk.zhijiandao.cn

[D14] 映射转换（每个元素变形）
来源：http://ojp.xziqi.cn


<!-- 参考信息 -->
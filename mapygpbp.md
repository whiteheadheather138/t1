代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pqs.wangshuangyany.cn

Java: x instanceof Number
来源：http://bqr.tarul.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wel.xingfuxueyuan.xyz

Ruby: x.is_a?(Numeric)
来源：http://qpn.svipenyu.cn

C#:   x is int or double or decimal
来源：http://dhj.epnwcf.com

[B14] 判断值是否在集合内
来源：http://rvp.vqdsnc.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mlo.xylfe.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tzz.jinyuanbaomall.cn

JS:   [1, 2, 3].includes(x)
来源：http://rxo.jiagoushi.top

TS:   [1, 2, 3].includes(x)
来源：http://lmn.vqdsnc.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://zub.gogol.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://stp.guannengcc.top

Ruby: [1, 2, 3].include?(x)
来源：http://gpz.ppjwa.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://owo.yueranfly.top

[B15] 布尔运算与取反
来源：http://sqy.yuanzhike.top

Py:   a and b or not c
来源：http://wxi.zycfv.cn

PHP:  $a && $b || !$c
来源：http://iml.ehwqpu.com

JS:   a && b || !c
来源：http://mrp.cdnleiting.top

TS:   a && b || !c
来源：http://okp.cashguo.top

Java: a && b || !c
来源：http://lno.tanke756.top

Go:   a && b || !c
来源：http://qmk.0kj1m.cn

Ruby: a && b || !c
来源：http://rrj.xinyue.icu

C#:   a && b || !c
来源：http://ylt.chenjidiqi.icu

[B16] 卫语句：不满足条件提前返回
来源：http://wml.zhaomingkeji.xyz

Py:   if not data: return
来源：http://byl.zhijiandao.cn

PHP:  if (!$data) { return; }
来源：http://tcl.bjfxy.top

JS:   if (!data) return;
来源：http://oem.fehbvm.com

TS:   if (!data) return;
来源：http://gss.jinyuanbaomall.cn

Java: if (data == null) return;
来源：http://wuf.bjfxy.top

Go:   if data == nil { return }
来源：http://xrn.snrcjt.cn

Ruby: return if data.nil?
来源：http://ruq.sufxvd.cn

C#:   if (data == null) return;
来源：http://qpp.zhongyouzk.top

================================================================================
来源：http://kse.wangdashe.top

C. 函数与作用域
来源：http://yok.yuxming.cn

================================================================================
来源：http://odz.jlsjyb.cn

[C01] 定义函数
来源：http://tti.hywenlv.cn

Py:   def add(a, b): return a + b
来源：http://egs.jlsjyb.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ntv.chenzaomai.com

JS:   function add(a, b) { return a + b; }
来源：http://jyd.zhaomingkeji.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cev.wangshuangyany.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fyb.xuetiantiany.cn

Go:   func add(a, b int) int { return a + b }
来源：http://cuu.gaohongyu789.top

Ruby: def add(a, b); a + b; end
来源：http://wxu.fehbvm.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://prg.hywenlv.cn

[C02] 默认参数
来源：http://aob.zhixingplan.top

Py:   def greet(name="World"): return name
来源：http://wxe.zycfv.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://kaa.yuanzhike.top

JS:   function greet(name = "World") { return name; }
来源：http://vqa.yj202588.top

TS:   function greet(name: string = "World") { return name; }
来源：http://hkk.yj20258.top

Java: // 无默认参数：方法重载或 Optional
来源：http://bfh.guowangkeji.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mfq.shanyushiyangtech.top

Ruby: def greet(name = "World") = name
来源：http://sga.wangdashe.top

C#:   string Greet(string name = "World") => name;
来源：http://csj.redwolf501.top

[C03] 可变参数
来源：http://xhn.sufxvd.cn

Py:   def total(*args): return sum(args)
来源：http://xun.chenzaomai.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hvw.ydjk.org.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vfe.snrcjt.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jqg.hammf.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gdu.gaohongyu789.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nzx.jinghuilouyu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://urx.guannengcc.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://iuc.hnqzz.top

[C04] 命名参数 / 关键字参数
来源：http://wnt.gzhubu.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dum.vehdjk.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mup.52xcode.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yuj.yj202588.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rcz.gzhubu.top

Java: // 无：用 Builder 模式或 record
来源：http://liz.xylfe.cn

Go:   // 无：用配置结构体参数
来源：http://zvw.zhengqikj.top

Ruby: f(a: 1, b: 2)
来源：http://bxe.hfpthk.cn

C#:   f(a: 1, b: 2)
来源：http://woh.daxiang520.top

[C05] 返回多个值
来源：http://aoo.jinyuanbaomall.cn

Py:   return a, b
来源：http://zkm.yj20258.top

PHP:  return [$a, $b];
来源：http://eln.xuetiantiany.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://kln.jiagoushi.top

TS:   return { a, b };
来源：http://tof.jinyuanbaomall.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vbi.ybcxt.top

Go:   return a, b
来源：http://piv.yuxming.cn

Ruby: return a, b
来源：http://pdb.ybcxt.top

C#:   return (a, b);              // ValueTuple
来源：http://mca.shzxlz.cn

[C06] 匿名函数 / lambda
来源：http://vec.sufxvd.cn

Py:   square = lambda x: x * x
来源：http://bgz.ywan-chungtsiang.top

PHP:  $square = fn($x) => $x * $x;
来源：http://kan.wangdashe.top

JS:   const square = x => x * x;
来源：http://mcn.fanxiaobao.xyz

TS:   const square = (x: number): number => x * x;
来源：http://pjp.cheryme.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qmy.aizwys.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dzs.hywenlv.cn

Ruby: square = ->(x) { x * x }
来源：http://rgj.nwbrower.top

C#:   Func<int, int> square = x => x * x;
来源：http://hkb.zdbjq.cn

[C07] 把函数作为参数传入
来源：http://vwi.jinqigfzy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wvx.guowangkeji.top

PHP:  array_map("strtoupper", $arr);
来源：http://ekd.quarkkingdee.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://enh.fzhhl.top

TS:   arr.map(String)
来源：http://nol.sjlbkw.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xss.zhaomingkeji.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kqw.epnwcf.com

Ruby: arr.map(&:upcase)
来源：http://rfg.tian-w.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://bds.zdbjq.cn

[C08] 闭包
来源：http://dat.tarul.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xon.vqdsnc.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://swm.jinqigfzy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fry.chenlongwang.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://krl.jiagoushi.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rrt.tianlin.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ueo.yueranfly.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nre.jiagoushi.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vrf.havefunace.top

[C09] 递归
来源：http://aas.shanyushiyangtech.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://uxw.cheryme.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wnr.haohaochexian.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iol.hongshengwenyu.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bam.ywan-chungtsiang.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://btp.nanxinkj.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://llx.c1oappe.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://veu.guowangkeji.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://msy.feifeiyinyue.top

[C10] 变量作用域
来源：http://vol.jianghu66.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ilm.zdqjudy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xwc.xylfe.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ydk.cucudq.cn

TS:   同 JS
来源：http://uoi.jyoumei.cn

Java: 方法内为块级作用域
来源：http://qzm.epnwcf.com

Go:   花括号块级作用域
来源：http://xjx.gogol.net.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mzk.cashguo.top

C#:   块级作用域
来源：http://hzs.yongpay.top

[C11] 模块导入与导出
来源：http://aqy.pycfn.com

Py:   from module import func
来源：http://okb.sufxvd.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wvo.haohaochexian.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://dkj.jinqigfzy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://aro.fehbvm.com

Java: import java.util.List;
来源：http://xdw.xylfe.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://swe.hnxiangtu.top

Ruby: require "json"; require_relative "./util"
来源：http://wkw.sysykeji.top

C#:   using System.Text;
来源：http://vbx.hcnkem.com

[C12] 立即执行函数 IIFE
来源：http://ocl.316326.xyz

Py:   (lambda: print("run"))()
来源：http://mvx.shzxlz.cn

PHP:  (function () { echo "run"; })();
来源：http://fzz.andypj.xyz

JS:   (() => { console.log("run"); })();
来源：http://nrf.yj20258888.top

TS:   (() => { console.log("run"); })();
来源：http://pny.zdqjudy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ubi.svipenyu.cn

Go:   func() { fmt.Println("run") }()
来源：http://hyl.tianlin.xyz

Ruby: -> { puts "run" }.call
来源：http://vgl.tanke756.top

C#:   // 无 IIFE：用静态构造函数
来源：http://xgj.jinqigfzy.top

[C13] 类型声明 / 类型注解
来源：http://hkz.chenlongwang.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://uvc.cheryme.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://skb.xingfuxueyuan.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bga.zhaomingkeji.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ewe.yonumen.top

Java: int add(int a, int b) { return a + b; }
来源：http://xcc.9152youxi.cn

Go:   func add(a, b int) int
来源：http://ezu.ydzc1.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jwy.xylfe.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fhp.jinqigufen.top

[C14] 泛型函数
来源：http://ati.sjlbkw.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://she.ydzc1.top

PHP:  // 无泛型
来源：http://vhp.hesvh.cn

JS:   // 无泛型
来源：http://jar.316326.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ahu.zycfv.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xyy.zhongyouzk.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vea.9152youxi.cn

Ruby: # 无泛型
来源：http://bwu.zhiwuduotai.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://drs.chenlongwang.top

[C15] 解构 / 展开参数
来源：http://bss.hcnkem.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://var.xuetiantiany.cn

PHP:  [$a, $b] = $pair;
来源：http://udm.iojbl.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://sia.sweek.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://knf.jyoumei.cn

Java: // 无解构
来源：http://lib.fanxiaobao.xyz

Go:   // 无解构
来源：http://jai.gotoacloud.top

Ruby: a, b = pair
来源：http://lrx.gzhubu.top

C#:   var (a, b) = pair;
来源：http://dmv.aibaodan.cn

[C16] 函数 / 方法重载
来源：http://uhx.xziqi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://urx.xingfuxueyuan.xyz

PHP:  // 无重载
来源：http://ose.birdmap.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://szp.sweek.top

TS:   // 用联合类型或重载签名声明
来源：http://hby.svipenyu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://kyz.snrcjt.cn

Go:   // 无重载：用不同函数名
来源：http://iff.fzhhl.top

Ruby: # 无重载：靠动态参数
来源：http://fns.ppjwa.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zya.gzhubu.top

================================================================================
来源：http://ceh.tanke756.top

D. 数组 / 列表 / 集合
来源：http://uzb.9152youxi.cn

================================================================================
来源：http://elh.shuidangran.top

[D01] 创建数组 / 列表
来源：http://qld.yfazqb.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://cda.gotoacloud.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://til.nwbrower.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://msz.dianchejie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jrf.nwbrower.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nqn.nwbrower.top

Go:   arr := []int{1, 2, 3}
来源：http://wnb.cashguo.top

Ruby: arr = [1, 2, 3]
来源：http://rxv.yuanzhike.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zxf.birdmap.top

[D02] 追加元素到末尾
来源：http://dex.ybcxt.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://eue.zhijiandao.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hkq.uphjek.com

JS:   arr.push(4);
来源：http://wft.shuidangran.top

TS:   arr.push(4);
来源：http://mar.zdqjudy.top

Java: list.add(4);
来源：http://ldc.dashuyun.cn

Go:   arr = append(arr, 4)
来源：http://nue.hesvh.cn

Ruby: arr << 4; arr.push(5)
来源：http://nrx.guowangkeji.top

C#:   list.Add(4);
来源：http://fcd.aibaodan.cn

[D03] 在指定位置插入元素
来源：http://wap.jyoumei.cn

Py:   arr.insert(0, 0)
来源：http://jek.pycfn.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wpz.jinqigfzy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dqz.xuanzx.com

TS:   arr.splice(0, 0, 0);
来源：http://bnt.bjfxy.top

Java: list.add(0, 0);
来源：http://cgl.chenjidiqi.icu

Go:   arr = append([]int{0}, arr...)
来源：http://tud.aibaodan.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bjv.cheryme.top

C#:   list.Insert(0, 0);
来源：http://lff.iojbl.cn

[D04] 删除元素
来源：http://vxq.shanyushiyangkeji.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jsw.zhoulong.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cqv.zdqjudy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qzj.cheryme.top

TS:   arr.splice(0, 1);
来源：http://nuw.aizwys.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wuq.chenzaomai.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dpm.aibaodan.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://buy.gotoacloud.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yxw.yj20258888.top

[D05] 访问与修改元素
来源：http://neb.ybcxt.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ndb.xylfe.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wmh.yvedp.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zjx.daria6918.cn

TS:   arr[0]; arr.at(-1);
来源：http://jce.andypj.xyz

Java: list.get(0); list.set(0, 9);
来源：http://ano.sufxvd.cn

Go:   arr[0]; arr[0] = 9
来源：http://kmk.zhaomingkeji.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ozi.hongshengwenyu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bxb.sufxvd.cn

[D06] 数组长度
来源：http://zcz.kuanghao11.cn

Py:   len(arr)
来源：http://pll.yongpay.top

PHP:  count($arr);
来源：http://qlq.smart0.xyz

JS:   arr.length
来源：http://xks.meibo888.top

TS:   arr.length
来源：http://bkk.jinqigufen.top

Java: list.size();
来源：http://eem.smart0.xyz

Go:   len(arr)
来源：http://tso.shuidangran.top

Ruby: arr.length; arr.size
来源：http://upq.yj20258.top

C#:   list.Count;
来源：http://ryg.zhaomingkeji.xyz

[D07] 切片 / 取子数组
来源：http://rcf.birdmap.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mvi.redwolf501.top

PHP:  array_slice($arr, 1, 3);
来源：http://llz.svipenyu.cn

JS:   arr.slice(1, 4);
来源：http://kzl.tanke756.top

TS:   arr.slice(1, 4);
来源：http://czy.cucudq.cn

Java: list.subList(1, 4);
来源：http://qir.cashguo.top

Go:   arr[1:4]
来源：http://hpa.fktsv.cn

Ruby: arr[1, 3]
来源：http://ytg.yanxiufei.cn

C#:   list.GetRange(1, 3);
来源：http://ozl.yonumen.top

[D08] 合并两个数组
来源：http://agt.ywan-chungtsiang.top

Py:   a + b;  a.extend(b)
来源：http://eyr.ctjpmb.com

PHP:  array_merge($a, $b);
来源：http://icr.chenzaomai.com

JS:   [...a, ...b];  a.concat(b);
来源：http://iyz.jinqigufen.top

TS:   [...a, ...b];
来源：http://yzu.cashguo.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ots.ybcxt.top

Go:   append(a, b...)
来源：http://adi.iojbl.cn

Ruby: a + b;  a.concat(b)
来源：http://bav.jinyuanbaomall.cn

C#:   a.Concat(b).ToList()
来源：http://wzr.shanyushiyangkeji.top

[D09] 排序（升序）
来源：http://exh.svipenyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://gcp.cqqwz.cn

PHP:  sort($arr);
来源：http://llt.cheryme.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://clf.guowangkeji.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://wgh.316326.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://nnv.havefunace.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ayh.gaohongyu789.top

Ruby: arr.sort
来源：http://itc.yonumen.top

C#:   list.Sort();
来源：http://vrc.tian-w.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://dlo.dianchejie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yfc.dianchejie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ckp.fzhhl.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ymc.jinyuanbaomall.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rvk.iojbl.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ohy.sysykeji.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tzy.ywan-chungtsiang.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rgc.jinqigfzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wsv.yuanzhike.top

[D11] 反转数组
来源：http://jiu.jiagoushi.top

Py:   arr[::-1];  arr.reverse()
来源：http://bcd.yj202588.top

PHP:  array_reverse($arr);
来源：http://psh.svipenyu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://glp.daxiang520.top

TS:   [...arr].reverse();
来源：http://zmg.yanxiufei.cn

Java: Collections.reverse(list);
来源：http://tst.hywenlv.cn

Go:   slices.Reverse(arr)
来源：http://hbm.fzhhl.top

Ruby: arr.reverse
来源：http://ejh.zdqjudy.top

C#:   list.Reverse();
来源：http://tvk.uphjek.com

[D12] 查找元素下标
来源：http://ufb.yuxming.cn

Py:   arr.index(x);  x in arr
来源：http://dfp.52xcode.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://soq.gaohongyu789.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xoy.jianghu66.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dqp.hcnkem.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gpp.pengpengdd.cyou

Go:   slices.Index(arr, x)
来源：http://vun.jinghuilouyu.cn

Ruby: arr.index(x)
来源：http://ont.xylfe.cn

C#:   list.IndexOf(x);
来源：http://yry.zhoulong.xyz

[D13] 过滤（保留满足条件的）
来源：http://gfx.yfazqb.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xfg.zhixingplan.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rqz.xinyue.icu

JS:   arr.filter(x => x > 3)
来源：http://txb.fzhhl.top

TS:   arr.filter(x => x > 3)
来源：http://yog.pengpengdd.cyou

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fjp.snrcjt.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ucu.cheryme.top

Ruby: arr.select { |x| x > 3 }
来源：http://wii.jyoumei.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://znl.zycfv.cn

[D14] 映射转换（每个元素变形）
来源：http://mwg.daxiang520.top


<!-- 参考信息 -->
代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://snm.wangshuangyany.cn

Java: x instanceof Number
来源：http://yqx.9152youxi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vyk.jqgufenzy.top

Ruby: x.is_a?(Numeric)
来源：http://mub.316326.xyz

C#:   x is int or double or decimal
来源：http://orp.ywan-chungtsiang.top

[B14] 判断值是否在集合内
来源：http://bzv.jyoumei.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://djj.yj20258.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://phq.c1oappe.top

JS:   [1, 2, 3].includes(x)
来源：http://cvo.redwolf501.top

TS:   [1, 2, 3].includes(x)
来源：http://hdw.vqdsnc.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://pct.shanyushiyangkeji.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wnq.tarul.cn

Ruby: [1, 2, 3].include?(x)
来源：http://tnl.zhaomingkeji.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://agy.fengsongda.top

[B15] 布尔运算与取反
来源：http://xiu.chenzaomai.com

Py:   a and b or not c
来源：http://jum.52xcode.cn

PHP:  $a && $b || !$c
来源：http://cuc.gaohongyu789.top

JS:   a && b || !c
来源：http://qyz.fzhhl.top

TS:   a && b || !c
来源：http://xai.zdqjudy.top

Java: a && b || !c
来源：http://dgk.zhaomingkeji.xyz

Go:   a && b || !c
来源：http://fas.guowangkeji.top

Ruby: a && b || !c
来源：http://zut.ctjpmb.com

C#:   a && b || !c
来源：http://jag.bbcook.cn

[B16] 卫语句：不满足条件提前返回
来源：http://rpe.9152youxi.cn

Py:   if not data: return
来源：http://qyl.shangyingyoupin.top

PHP:  if (!$data) { return; }
来源：http://wup.hongshengwenyu.top

JS:   if (!data) return;
来源：http://cps.ydjk.org.cn

TS:   if (!data) return;
来源：http://bfk.gzhubu.top

Java: if (data == null) return;
来源：http://oka.ivvv.top

Go:   if data == nil { return }
来源：http://uuu.gaohongyu789.top

Ruby: return if data.nil?
来源：http://omj.tanke756.top

C#:   if (data == null) return;
来源：http://wik.zhixingplan.top

================================================================================
来源：http://ehq.yongpay.top

C. 函数与作用域
来源：http://fxl.yj202588.top

================================================================================
来源：http://qlz.jqgufenzy.top

[C01] 定义函数
来源：http://fwl.hesvh.cn

Py:   def add(a, b): return a + b
来源：http://qbd.ybcxt.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qxm.pengpengdd.cyou

JS:   function add(a, b) { return a + b; }
来源：http://cvq.fehbvm.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://omx.shanyushiyangtech.top

Java: static int add(int a, int b) { return a + b; }
来源：http://zuz.shanyushiyangtech.top

Go:   func add(a, b int) int { return a + b }
来源：http://qvg.zhongyouzk.top

Ruby: def add(a, b); a + b; end
来源：http://jrz.nanxuanxn.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ylj.daria6918.cn

[C02] 默认参数
来源：http://dkx.hywenlv.cn

Py:   def greet(name="World"): return name
来源：http://idf.nwbrower.top

PHP:  function greet($name = "World") { return $name; }
来源：http://yth.jinqigfzy.top

JS:   function greet(name = "World") { return name; }
来源：http://kes.shangyingyoupin.top

TS:   function greet(name: string = "World") { return name; }
来源：http://afk.quarkkingdee.top

Java: // 无默认参数：方法重载或 Optional
来源：http://vpa.vehdjk.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hxs.hysaishi.cn

Ruby: def greet(name = "World") = name
来源：http://mnl.jqgufenzy.top

C#:   string Greet(string name = "World") => name;
来源：http://mho.smart0.xyz

[C03] 可变参数
来源：http://zmj.dianchejie.cn

Py:   def total(*args): return sum(args)
来源：http://tfd.ppjwa.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://iho.epnwcf.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rcq.chenzaomai.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vgw.yj202588.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qto.zhijiandao.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ctx.chenjidiqi.icu

Ruby: def total(*nums); nums.sum; end
来源：http://mba.cheryme.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rar.pycfn.com

[C04] 命名参数 / 关键字参数
来源：http://fxe.hnxiangtu.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://evl.bbcook.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xya.nwbrower.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://apz.jiagoushi.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xlr.zhijiandao.cn

Java: // 无：用 Builder 模式或 record
来源：http://obw.daria6918.cn

Go:   // 无：用配置结构体参数
来源：http://esf.hammf.cn

Ruby: f(a: 1, b: 2)
来源：http://jgo.hnxiangtu.top

C#:   f(a: 1, b: 2)
来源：http://tip.zdbjq.cn

[C05] 返回多个值
来源：http://psq.jinyuanbaomall.cn

Py:   return a, b
来源：http://jjk.hysaishi.cn

PHP:  return [$a, $b];
来源：http://ryi.jinqigufen.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://tny.hnqzz.top

TS:   return { a, b };
来源：http://idz.316326.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ayk.nanxuanxn.top

Go:   return a, b
来源：http://rmb.fengsongda.top

Ruby: return a, b
来源：http://yxj.sxryk.cn

C#:   return (a, b);              // ValueTuple
来源：http://imx.hnqzz.top

[C06] 匿名函数 / lambda
来源：http://cyj.cashguo.top

Py:   square = lambda x: x * x
来源：http://qdl.tarul.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ors.quarkkingdee.top

JS:   const square = x => x * x;
来源：http://dxu.nwbrower.top

TS:   const square = (x: number): number => x * x;
来源：http://cot.zhixingplan.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ufs.hammf.cn

Go:   sq := func(x int) int { return x * x }
来源：http://vdw.yuanzhike.top

Ruby: square = ->(x) { x * x }
来源：http://itm.zhaomingkeji.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://whe.feifeiyinyue.top

[C07] 把函数作为参数传入
来源：http://vuu.zhiwuduotai.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://idx.sjlbkw.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vbu.yfazqb.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gap.jianghu66.top

TS:   arr.map(String)
来源：http://qna.yangfankeji.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dzs.yj20258888.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://erb.cheryme.top

Ruby: arr.map(&:upcase)
来源：http://xbd.yueranfly.top

C#:   arr.Select(s => s.ToUpper())
来源：http://shx.chenzaomai.com

[C08] 闭包
来源：http://tht.mhx1999.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ekd.jqgufenzy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rev.guowangkeji.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yqo.shangyingyoupin.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uev.birdmap.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vpl.fktsv.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pdv.bbcook.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mzr.haohaochexian.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://sca.pengpengdd.cyou

[C09] 递归
来源：http://tkg.svipenyu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://agz.cashguo.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cti.vqdsnc.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://myc.nwbrower.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aqa.sjlbkw.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vpc.shanyushiyangkeji.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hsk.cashguo.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yfh.redwolf501.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rsg.guannengcc.top

[C10] 变量作用域
来源：http://hva.hfpthk.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mae.zhongyouzk.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lts.gotoacloud.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jia.yueranfly.top

TS:   同 JS
来源：http://tqk.9152youxi.cn

Java: 方法内为块级作用域
来源：http://jqa.sjlbkw.cn

Go:   花括号块级作用域
来源：http://bic.hysaishi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pky.xuetiantiany.cn

C#:   块级作用域
来源：http://fvs.dianchejie.cn

[C11] 模块导入与导出
来源：http://gbg.tian-w.cn

Py:   from module import func
来源：http://mgy.hcnkem.com

PHP:  require "file.php";  或 use App\Service;
来源：http://rag.wangdashe.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://dsw.hfpthk.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://igf.ybcxt.top

Java: import java.util.List;
来源：http://wbd.fengsongda.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hlc.cheryme.top

Ruby: require "json"; require_relative "./util"
来源：http://pby.cashguo.top

C#:   using System.Text;
来源：http://kgx.birdmap.top

[C12] 立即执行函数 IIFE
来源：http://fcy.ctjpmb.com

Py:   (lambda: print("run"))()
来源：http://tji.redwolf501.top

PHP:  (function () { echo "run"; })();
来源：http://gmc.9152youxi.cn

JS:   (() => { console.log("run"); })();
来源：http://imf.nwbrower.top

TS:   (() => { console.log("run"); })();
来源：http://esv.havefunace.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kiz.ywan-chungtsiang.top

Go:   func() { fmt.Println("run") }()
来源：http://uze.uphjek.com

Ruby: -> { puts "run" }.call
来源：http://bkw.ehwqpu.com

C#:   // 无 IIFE：用静态构造函数
来源：http://zis.gotoacloud.top

[C13] 类型声明 / 类型注解
来源：http://mte.jqgfzy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nsf.tarul.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jfi.hywenlv.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jca.chenlongwang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uae.tianlin.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://ksy.yonumen.top

Go:   func add(a, b int) int
来源：http://rst.ydjk.org.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vgf.yj20258.top

C#:   int Add(int a, int b) => a + b;
来源：http://hhu.sufxvd.cn

[C14] 泛型函数
来源：http://jql.jinqigfzy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://djz.iojbl.cn

PHP:  // 无泛型
来源：http://yey.jyoumei.cn

JS:   // 无泛型
来源：http://ipw.ppjwa.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://phz.bjfxy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qai.nwbrower.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vgw.pengpengdd.cyou

Ruby: # 无泛型
来源：http://cxa.sufxvd.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ufj.ppjwa.cn

[C15] 解构 / 展开参数
来源：http://smn.ppjwa.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dws.yueranfly.top

PHP:  [$a, $b] = $pair;
来源：http://xrm.mhx1999.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://epg.hysaishi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nur.zhongyouzk.top

Java: // 无解构
来源：http://wng.hammf.cn

Go:   // 无解构
来源：http://prn.tian-w.cn

Ruby: a, b = pair
来源：http://ejn.sufxvd.cn

C#:   var (a, b) = pair;
来源：http://tcq.yangfankeji.com

[C16] 函数 / 方法重载
来源：http://zxh.cheryme.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gfv.cashguo.top

PHP:  // 无重载
来源：http://xma.yuanzhike.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://pvp.cucudq.cn

TS:   // 用联合类型或重载签名声明
来源：http://ivk.yueranfly.top

Java: void f(int a) {}  void f(String a) {}
来源：http://thc.316326.xyz

Go:   // 无重载：用不同函数名
来源：http://dmw.aibaodan.cn

Ruby: # 无重载：靠动态参数
来源：http://rcu.fengsongda.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://bcr.fktsv.cn

================================================================================
来源：http://tcc.ydzc1.top

D. 数组 / 列表 / 集合
来源：http://qpy.gaohongyu789.top

================================================================================
来源：http://wyz.chenlongwang.top

[D01] 创建数组 / 列表
来源：http://lim.gotoacloud.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://vet.yanxiufei.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rbl.cqqwz.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tij.aizwys.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kfn.cucudq.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xnu.zhixingplan.top

Go:   arr := []int{1, 2, 3}
来源：http://rsx.yongpay.top

Ruby: arr = [1, 2, 3]
来源：http://vlr.nwbrower.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vby.sxryk.cn

[D02] 追加元素到末尾
来源：http://aqh.gaohongyu789.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lax.snrcjt.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hfr.yj20258.top

JS:   arr.push(4);
来源：http://esu.xingfuxueyuan.xyz

TS:   arr.push(4);
来源：http://sgk.jiagoushi.top

Java: list.add(4);
来源：http://eea.havefunace.top

Go:   arr = append(arr, 4)
来源：http://pvx.ppjwa.cn

Ruby: arr << 4; arr.push(5)
来源：http://heq.quarkkingdee.top

C#:   list.Add(4);
来源：http://ydy.yj20258888.top

[D03] 在指定位置插入元素
来源：http://cjn.pycfn.com

Py:   arr.insert(0, 0)
来源：http://ioz.gaohongyu789.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ndw.wangshuangyany.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mwr.gotoacloud.top

TS:   arr.splice(0, 0, 0);
来源：http://zpn.fktsv.cn

Java: list.add(0, 0);
来源：http://sbo.tianlin.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://zpb.daxiang520.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lds.yongpay.top

C#:   list.Insert(0, 0);
来源：http://xwp.zhijiandao.cn

[D04] 删除元素
来源：http://ekk.sufxvd.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wkb.yj202588.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zoi.yuxming.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sfb.hammf.cn

TS:   arr.splice(0, 1);
来源：http://vbs.birdmap.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nuc.sweek.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://niw.pycfn.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wbq.jqgufenzy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bpd.shanyushiyangtech.top

[D05] 访问与修改元素
来源：http://mol.yuxming.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ris.smart0.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vpr.jlsjyb.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mms.tanke756.top

TS:   arr[0]; arr.at(-1);
来源：http://xru.jianghu66.top

Java: list.get(0); list.set(0, 9);
来源：http://ipl.epnwcf.com

Go:   arr[0]; arr[0] = 9
来源：http://bmg.chenlongwang.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qee.kuanghao11.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://foo.shanyushiyangtech.top

[D06] 数组长度
来源：http://lzy.yongpay.top

Py:   len(arr)
来源：http://nzx.hywenlv.cn

PHP:  count($arr);
来源：http://paj.xylfe.cn

JS:   arr.length
来源：http://hjb.ywan-chungtsiang.top

TS:   arr.length
来源：http://ywd.jinghuilouyu.cn

Java: list.size();
来源：http://dig.guowangkeji.top

Go:   len(arr)
来源：http://fui.yongpay.top

Ruby: arr.length; arr.size
来源：http://dix.xylfe.cn

C#:   list.Count;
来源：http://rqz.ybcxt.top

[D07] 切片 / 取子数组
来源：http://tjs.jinqigfzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jnr.jianghu66.top

PHP:  array_slice($arr, 1, 3);
来源：http://fac.snrcjt.cn

JS:   arr.slice(1, 4);
来源：http://koz.sxryk.cn

TS:   arr.slice(1, 4);
来源：http://his.hfpthk.cn

Java: list.subList(1, 4);
来源：http://sju.yueranfly.top

Go:   arr[1:4]
来源：http://sxd.shangyingyoupin.top

Ruby: arr[1, 3]
来源：http://aww.shanyushiyangkeji.top

C#:   list.GetRange(1, 3);
来源：http://gzu.tanke756.top

[D08] 合并两个数组
来源：http://xux.yfazqb.com

Py:   a + b;  a.extend(b)
来源：http://ufe.dashuyun.cn

PHP:  array_merge($a, $b);
来源：http://wch.cheryme.top

JS:   [...a, ...b];  a.concat(b);
来源：http://yzu.ivvv.top

TS:   [...a, ...b];
来源：http://jwu.hysaishi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ccs.jqgufenzy.top

Go:   append(a, b...)
来源：http://vve.mhx1999.top

Ruby: a + b;  a.concat(b)
来源：http://dcc.xuanzx.com

C#:   a.Concat(b).ToList()
来源：http://fdm.cdnleiting.top

[D09] 排序（升序）
来源：http://fhv.zhengqikj.top

Py:   sorted(arr);  arr.sort()
来源：http://cgn.shanyushiyangkeji.top

PHP:  sort($arr);
来源：http://ojo.hcnkem.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xco.ybcxt.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://duw.9152youxi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://oml.quarkkingdee.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://trb.redwolf501.top

Ruby: arr.sort
来源：http://dvd.cashguo.top

C#:   list.Sort();
来源：http://vcn.fzhhl.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://efy.yuxming.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ilg.xziqi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nhv.sjlbkw.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mby.yanxiufei.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pmv.hnxiangtu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cao.sxryk.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hqj.xingfuxueyuan.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nlf.epnwcf.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fui.yvedp.cn

[D11] 反转数组
来源：http://rzc.zhengqikj.top

Py:   arr[::-1];  arr.reverse()
来源：http://zlr.zycfv.cn

PHP:  array_reverse($arr);
来源：http://sys.zhoulong.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dik.tarul.cn

TS:   [...arr].reverse();
来源：http://wgk.xinyue.icu

Java: Collections.reverse(list);
来源：http://bhk.gzhubu.top

Go:   slices.Reverse(arr)
来源：http://xkm.snrcjt.cn

Ruby: arr.reverse
来源：http://ofe.yanxiufei.cn

C#:   list.Reverse();
来源：http://jmd.gotoacloud.top

[D12] 查找元素下标
来源：http://fmm.sweek.top

Py:   arr.index(x);  x in arr
来源：http://ngg.birdmap.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pbn.svipenyu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nxg.tian-w.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ven.xziqi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gtg.cdnleiting.top

Go:   slices.Index(arr, x)
来源：http://jsw.ydzc1.top

Ruby: arr.index(x)
来源：http://tqp.xuanzx.com

C#:   list.IndexOf(x);
来源：http://rkt.kuanghao11.cn

[D13] 过滤（保留满足条件的）
来源：http://zen.nanxuanxn.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://upu.daria6918.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qxr.hysaishi.cn

JS:   arr.filter(x => x > 3)
来源：http://cfc.zhaomingkeji.xyz

TS:   arr.filter(x => x > 3)
来源：http://dim.hnqzz.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://whz.xingfuxueyuan.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bop.tarul.cn

Ruby: arr.select { |x| x > 3 }
来源：http://nzn.iojbl.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://puz.jinqigfzy.top

[D14] 映射转换（每个元素变形）
来源：http://ylt.wangshuangyany.cn


<!-- 参考信息 -->
代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hbo.smart0.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://poq.gotoacloud.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jwv.aibaodan.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bqm.fehbvm.com

[B13] 判断是否为数字
来源：http://zxf.yvedp.cn

Py:   isinstance(x, (int, float))
来源：http://rla.zdqjudy.top

PHP:  is_numeric($x)
来源：http://vtr.cashguo.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vpr.jianghu66.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ykk.yangfankeji.com

Java: x instanceof Number
来源：http://hro.ydzc1.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://aud.daxiang520.top

Ruby: x.is_a?(Numeric)
来源：http://vnc.chenjidiqi.icu

C#:   x is int or double or decimal
来源：http://uyl.chenjidiqi.icu

[B14] 判断值是否在集合内
来源：http://jpq.gotoacloud.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rft.dashuyun.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wkb.9152youxi.cn

JS:   [1, 2, 3].includes(x)
来源：http://wye.jinqigfzy.top

TS:   [1, 2, 3].includes(x)
来源：http://qvo.nanxinkj.top

Java: List.of(1, 2, 3).contains(x)
来源：http://nhf.tanke756.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ugr.xinyue.icu

Ruby: [1, 2, 3].include?(x)
来源：http://wsb.iojbl.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kty.wangdashe.top

[B15] 布尔运算与取反
来源：http://dww.nanxuanxn.top

Py:   a and b or not c
来源：http://drb.jinyuanbaomall.cn

PHP:  $a && $b || !$c
来源：http://zsi.jyoumei.cn

JS:   a && b || !c
来源：http://tok.xuetiantiany.cn

TS:   a && b || !c
来源：http://mwx.ctjpmb.com

Java: a && b || !c
来源：http://zmt.vqdsnc.cn

Go:   a && b || !c
来源：http://vsj.pycfn.com

Ruby: a && b || !c
来源：http://snd.nanxuanxn.top

C#:   a && b || !c
来源：http://ija.dashuyun.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hca.bbcook.cn

Py:   if not data: return
来源：http://gmf.hesvh.cn

PHP:  if (!$data) { return; }
来源：http://tdw.sjlbkw.cn

JS:   if (!data) return;
来源：http://waj.0kj1m.cn

TS:   if (!data) return;
来源：http://aje.ywan-chungtsiang.top

Java: if (data == null) return;
来源：http://oyo.nanxuanxn.top

Go:   if data == nil { return }
来源：http://eiz.pycfn.com

Ruby: return if data.nil?
来源：http://otq.nanxinkj.top

C#:   if (data == null) return;
来源：http://kot.zhongyouzk.top

================================================================================
来源：http://jeb.jinghuilouyu.cn

C. 函数与作用域
来源：http://ddj.pengpengdd.cyou

================================================================================
来源：http://gcm.xziqi.cn

[C01] 定义函数
来源：http://kbd.daria6918.cn

Py:   def add(a, b): return a + b
来源：http://xkb.nanxinkj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mms.yvedp.cn

JS:   function add(a, b) { return a + b; }
来源：http://ret.cdnleiting.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gep.tanke756.top

Java: static int add(int a, int b) { return a + b; }
来源：http://yob.yfazqb.com

Go:   func add(a, b int) int { return a + b }
来源：http://rok.shuidangran.top

Ruby: def add(a, b); a + b; end
来源：http://ylq.cucudq.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fuh.52xcode.cn

[C02] 默认参数
来源：http://mxj.jlsjyb.cn

Py:   def greet(name="World"): return name
来源：http://keu.svipenyu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://obl.dashuyun.cn

JS:   function greet(name = "World") { return name; }
来源：http://xdm.fanxiaobao.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://kxv.sxryk.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://lcl.yanxiufei.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nly.epnwcf.com

Ruby: def greet(name = "World") = name
来源：http://spg.xuetiantiany.cn

C#:   string Greet(string name = "World") => name;
来源：http://lbh.jqgfzy.top

[C03] 可变参数
来源：http://gwf.cashguo.top

Py:   def total(*args): return sum(args)
来源：http://kwx.hfpthk.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yvx.kuanghao11.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yzk.haohaochexian.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xbq.gaohongyu789.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://csz.hnqzz.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mkp.yongpay.top

Ruby: def total(*nums); nums.sum; end
来源：http://yny.ydzc1.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dwp.chenzaomai.com

[C04] 命名参数 / 关键字参数
来源：http://lby.chenjidiqi.icu

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lic.shanyushiyangkeji.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zii.cashguo.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vqo.bjfxy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ehc.gaohongyu789.top

Java: // 无：用 Builder 模式或 record
来源：http://fer.jqgfzy.top

Go:   // 无：用配置结构体参数
来源：http://mdq.redwolf501.top

Ruby: f(a: 1, b: 2)
来源：http://ube.xuetiantiany.cn

C#:   f(a: 1, b: 2)
来源：http://wju.jinqigfzy.top

[C05] 返回多个值
来源：http://vkh.hywenlv.cn

Py:   return a, b
来源：http://bcd.yongpay.top

PHP:  return [$a, $b];
来源：http://hry.havefunace.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ppq.ehwqpu.com

TS:   return { a, b };
来源：http://atr.chenjidiqi.icu

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pma.jiagoushi.top

Go:   return a, b
来源：http://mit.feifeiyinyue.top

Ruby: return a, b
来源：http://epu.fehbvm.com

C#:   return (a, b);              // ValueTuple
来源：http://ulc.ywan-chungtsiang.top

[C06] 匿名函数 / lambda
来源：http://yyq.c1oappe.top

Py:   square = lambda x: x * x
来源：http://gnw.nanxuanxn.top

PHP:  $square = fn($x) => $x * $x;
来源：http://lzj.316326.xyz

JS:   const square = x => x * x;
来源：http://lfc.bbcook.cn

TS:   const square = (x: number): number => x * x;
来源：http://xjn.shuidangran.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://scc.shuidangran.top

Go:   sq := func(x int) int { return x * x }
来源：http://wgc.snrcjt.cn

Ruby: square = ->(x) { x * x }
来源：http://yqv.mhx1999.top

C#:   Func<int, int> square = x => x * x;
来源：http://sss.ydjk.org.cn

[C07] 把函数作为参数传入
来源：http://qhb.ybcxt.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qjs.ywan-chungtsiang.top

PHP:  array_map("strtoupper", $arr);
来源：http://wcy.svipenyu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pgq.gotoacloud.top

TS:   arr.map(String)
来源：http://vyo.bjfxy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qlr.yangfankeji.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fks.bjfxy.top

Ruby: arr.map(&:upcase)
来源：http://zgr.quarkkingdee.top

C#:   arr.Select(s => s.ToUpper())
来源：http://jtn.yueranfly.top

[C08] 闭包
来源：http://zwg.yuanzhike.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jxs.yj20258888.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://clq.yongpay.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nns.guannengcc.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mni.quarkkingdee.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pvp.vqdsnc.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://aez.redwolf501.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://emb.birdmap.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cnh.hcnkem.com

[C09] 递归
来源：http://hmr.yuanzhike.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://byz.dashuyun.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qmp.yj202588.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oos.epnwcf.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rlj.yuxming.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://eng.daria6918.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://eay.nanxuanxn.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yep.yongpay.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mcd.feifeiyinyue.top

[C10] 变量作用域
来源：http://epq.epnwcf.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gxc.aibaodan.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xyy.zdbjq.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gvu.9152youxi.cn

TS:   同 JS
来源：http://sxv.dianchejie.cn

Java: 方法内为块级作用域
来源：http://gaa.cheryme.top

Go:   花括号块级作用域
来源：http://rgc.xinyue.icu

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xtq.yanxiufei.cn

C#:   块级作用域
来源：http://fcd.havefunace.top

[C11] 模块导入与导出
来源：http://wze.mhx1999.top

Py:   from module import func
来源：http://pev.jlsjyb.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tsu.cheryme.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://nui.sjlbkw.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ewx.hysaishi.cn

Java: import java.util.List;
来源：http://fhp.xuanzx.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zzk.hysaishi.cn

Ruby: require "json"; require_relative "./util"
来源：http://dkb.shzxlz.cn

C#:   using System.Text;
来源：http://vyo.zhoulong.xyz

[C12] 立即执行函数 IIFE
来源：http://dit.zhoulong.xyz

Py:   (lambda: print("run"))()
来源：http://noj.jinqigfzy.top

PHP:  (function () { echo "run"; })();
来源：http://whr.ppjwa.cn

JS:   (() => { console.log("run"); })();
来源：http://lct.cucudq.cn

TS:   (() => { console.log("run"); })();
来源：http://sts.cashguo.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fbt.gogol.net.cn

Go:   func() { fmt.Println("run") }()
来源：http://xdr.aizwys.cn

Ruby: -> { puts "run" }.call
来源：http://eei.wangdashe.top

C#:   // 无 IIFE：用静态构造函数
来源：http://qcl.jqgfzy.top

[C13] 类型声明 / 类型注解
来源：http://epb.fzhhl.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://npm.yvedp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ugb.guowangkeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sxw.cheryme.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lha.52xcode.cn

Java: int add(int a, int b) { return a + b; }
来源：http://igw.uphjek.com

Go:   func add(a, b int) int
来源：http://qip.aizwys.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sdt.redwolf501.top

C#:   int Add(int a, int b) => a + b;
来源：http://aqk.chenjidiqi.icu

[C14] 泛型函数
来源：http://nub.daxiang520.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mbr.zhaomingkeji.xyz

PHP:  // 无泛型
来源：http://jmd.hcnkem.com

JS:   // 无泛型
来源：http://key.vqdsnc.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ydg.zhengqikj.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hmv.fzhhl.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hei.xuanzx.com

Ruby: # 无泛型
来源：http://cjn.hesvh.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jid.cdnleiting.top

[C15] 解构 / 展开参数
来源：http://sca.fktsv.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nwp.jyoumei.cn

PHP:  [$a, $b] = $pair;
来源：http://lzd.52xcode.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dks.gzhubu.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://efk.hysaishi.cn

Java: // 无解构
来源：http://pck.shanyushiyangkeji.top

Go:   // 无解构
来源：http://gmz.cheryme.top

Ruby: a, b = pair
来源：http://uqv.xinyue.icu

C#:   var (a, b) = pair;
来源：http://sbo.pycfn.com

[C16] 函数 / 方法重载
来源：http://vaa.hywenlv.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://skf.daxiang520.top

PHP:  // 无重载
来源：http://hrq.dashuyun.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bkv.shuidangran.top

TS:   // 用联合类型或重载签名声明
来源：http://mlp.smart0.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://vym.aizwys.cn

Go:   // 无重载：用不同函数名
来源：http://uta.ydjk.org.cn

Ruby: # 无重载：靠动态参数
来源：http://djr.gaohongyu789.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://eco.316326.xyz

================================================================================
来源：http://rkp.zhengqikj.top

D. 数组 / 列表 / 集合
来源：http://ply.snrcjt.cn

================================================================================
来源：http://ghg.xuanzx.com

[D01] 创建数组 / 列表
来源：http://gcz.jinghuilouyu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://rxh.pycfn.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://srx.yj20258.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://min.guannengcc.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://pvc.vqdsnc.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wqa.jqgfzy.top

Go:   arr := []int{1, 2, 3}
来源：http://xdu.zdqjudy.top

Ruby: arr = [1, 2, 3]
来源：http://dxx.ehwqpu.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lkj.nanxuanxn.top

[D02] 追加元素到末尾
来源：http://jtj.shuidangran.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://epb.zhixingplan.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://itm.hesvh.cn

JS:   arr.push(4);
来源：http://wnv.sjlbkw.cn

TS:   arr.push(4);
来源：http://ewg.ehwqpu.com

Java: list.add(4);
来源：http://ywo.zhoulong.xyz

Go:   arr = append(arr, 4)
来源：http://hki.52xcode.cn

Ruby: arr << 4; arr.push(5)
来源：http://fhm.yonumen.top

C#:   list.Add(4);
来源：http://qcw.guowangkeji.top

[D03] 在指定位置插入元素
来源：http://kks.nanxuanxn.top

Py:   arr.insert(0, 0)
来源：http://cps.uphjek.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zxz.fzhhl.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zdz.tanke756.top

TS:   arr.splice(0, 0, 0);
来源：http://jzn.yj202588.top

Java: list.add(0, 0);
来源：http://wya.yj20258.top

Go:   arr = append([]int{0}, arr...)
来源：http://qxj.hesvh.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jlw.xuetiantiany.cn

C#:   list.Insert(0, 0);
来源：http://sdr.sufxvd.cn

[D04] 删除元素
来源：http://jyy.yuxming.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mcr.uphjek.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lnf.shanyushiyangtech.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yes.ivvv.top

TS:   arr.splice(0, 1);
来源：http://dck.hongshengwenyu.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://los.shanyushiyangkeji.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://eae.hnxiangtu.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://arr.zdqjudy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hxb.zhongyouzk.top

[D05] 访问与修改元素
来源：http://zxa.yuanzhike.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rfk.yuxming.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pac.nanxuanxn.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ngt.sufxvd.cn

TS:   arr[0]; arr.at(-1);
来源：http://lap.chenzaomai.com

Java: list.get(0); list.set(0, 9);
来源：http://qap.xylfe.cn

Go:   arr[0]; arr[0] = 9
来源：http://oxu.birdmap.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://niw.zhoulong.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tqe.zhengqikj.top

[D06] 数组长度
来源：http://uxu.haohaochexian.top

Py:   len(arr)
来源：http://rlj.jinyuanbaomall.cn

PHP:  count($arr);
来源：http://gdc.yj202588.top

JS:   arr.length
来源：http://vod.yonumen.top

TS:   arr.length
来源：http://jay.jinqigufen.top

Java: list.size();
来源：http://duf.sufxvd.cn

Go:   len(arr)
来源：http://plu.epnwcf.com

Ruby: arr.length; arr.size
来源：http://xmj.hesvh.cn

C#:   list.Count;
来源：http://dqm.quarkkingdee.top

[D07] 切片 / 取子数组
来源：http://hbx.meibo888.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zdw.dashuyun.cn

PHP:  array_slice($arr, 1, 3);
来源：http://llm.ybcxt.top

JS:   arr.slice(1, 4);
来源：http://hca.yangfankeji.com

TS:   arr.slice(1, 4);
来源：http://jvn.quarkkingdee.top

Java: list.subList(1, 4);
来源：http://djh.daria6918.cn

Go:   arr[1:4]
来源：http://mnk.uphjek.com

Ruby: arr[1, 3]
来源：http://fbz.ehwqpu.com

C#:   list.GetRange(1, 3);
来源：http://bzu.yueranfly.top

[D08] 合并两个数组
来源：http://ptk.gzhubu.top

Py:   a + b;  a.extend(b)
来源：http://aoq.yonumen.top

PHP:  array_merge($a, $b);
来源：http://hnz.ydjk.org.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://anr.xylfe.cn

TS:   [...a, ...b];
来源：http://pln.zycfv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://oll.gogol.net.cn

Go:   append(a, b...)
来源：http://ern.tian-w.cn

Ruby: a + b;  a.concat(b)
来源：http://eeu.yueranfly.top

C#:   a.Concat(b).ToList()
来源：http://hbf.shanyushiyangkeji.top

[D09] 排序（升序）
来源：http://xrr.epnwcf.com

Py:   sorted(arr);  arr.sort()
来源：http://mcz.birdmap.top

PHP:  sort($arr);
来源：http://bcl.fktsv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ofu.andypj.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://mha.yanxiufei.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yrj.zdqjudy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qep.zycfv.cn

Ruby: arr.sort
来源：http://acf.smart0.xyz

C#:   list.Sort();
来源：http://wcg.fktsv.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mcq.xinyue.icu

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gti.vehdjk.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xfu.havefunace.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rex.xuanzx.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nja.jinqigfzy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ixe.ppjwa.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zof.quarkkingdee.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nfs.ppjwa.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mpc.mhx1999.top

[D11] 反转数组
来源：http://glo.chenlongwang.top

Py:   arr[::-1];  arr.reverse()
来源：http://lol.zhongyouzk.top

PHP:  array_reverse($arr);
来源：http://efn.sysykeji.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cys.hnxiangtu.top

TS:   [...arr].reverse();
来源：http://mtk.hnqzz.top

Java: Collections.reverse(list);
来源：http://nde.cucudq.cn

Go:   slices.Reverse(arr)
来源：http://hcy.ydjk.org.cn

Ruby: arr.reverse
来源：http://arf.sjlbkw.cn

C#:   list.Reverse();
来源：http://yoe.ybcxt.top

[D12] 查找元素下标
来源：http://lqw.ppjwa.cn

Py:   arr.index(x);  x in arr
来源：http://kcu.hesvh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qik.smart0.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jdj.yangfankeji.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://our.hesvh.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xql.redwolf501.top

Go:   slices.Index(arr, x)
来源：http://aeb.zhoulong.xyz

Ruby: arr.index(x)
来源：http://dwh.quarkkingdee.top

C#:   list.IndexOf(x);
来源：http://dth.jianghu66.top

[D13] 过滤（保留满足条件的）
来源：http://amp.zhiwuduotai.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://noy.xuetiantiany.cn


<!-- 参考信息 -->
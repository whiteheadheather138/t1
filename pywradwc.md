代发 wailian999

[B13] 判断是否为数字
来源：http://uop.zdqjudy.top

Py:   isinstance(x, (int, float))
来源：http://uxv.xylfe.cn

PHP:  is_numeric($x)
来源：http://hmq.nanxuanxn.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yxs.zhiwuduotai.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cwf.yfazqb.com

Java: x instanceof Number
来源：http://pjv.zhaomingkeji.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zxp.jiagoushi.top

Ruby: x.is_a?(Numeric)
来源：http://kkw.sysykeji.top

C#:   x is int or double or decimal
来源：http://nek.guowangkeji.top

[B14] 判断值是否在集合内
来源：http://yvr.gzhubu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qzz.nanxuanxn.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zml.nanxuanxn.top

JS:   [1, 2, 3].includes(x)
来源：http://qkm.yuxming.cn

TS:   [1, 2, 3].includes(x)
来源：http://vfd.haohaochexian.top

Java: List.of(1, 2, 3).contains(x)
来源：http://fcq.andypj.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zjf.fzhhl.top

Ruby: [1, 2, 3].include?(x)
来源：http://aqo.yuanzhike.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fvd.hcnkem.com

[B15] 布尔运算与取反
来源：http://lxn.ydjk.org.cn

Py:   a and b or not c
来源：http://uhq.vqdsnc.cn

PHP:  $a && $b || !$c
来源：http://tnd.bjfxy.top

JS:   a && b || !c
来源：http://mim.dianchejie.cn

TS:   a && b || !c
来源：http://kgd.zycfv.cn

Java: a && b || !c
来源：http://jwn.nanxuanxn.top

Go:   a && b || !c
来源：http://qeu.mhx1999.top

Ruby: a && b || !c
来源：http://ndg.tarul.cn

C#:   a && b || !c
来源：http://fyu.yongpay.top

[B16] 卫语句：不满足条件提前返回
来源：http://mtr.tianlin.xyz

Py:   if not data: return
来源：http://msg.jyoumei.cn

PHP:  if (!$data) { return; }
来源：http://jzk.zhiwuduotai.top

JS:   if (!data) return;
来源：http://tvm.jinqigfzy.top

TS:   if (!data) return;
来源：http://jgu.dianchejie.cn

Java: if (data == null) return;
来源：http://jui.zhoulong.xyz

Go:   if data == nil { return }
来源：http://ijn.havefunace.top

Ruby: return if data.nil?
来源：http://llo.svipenyu.cn

C#:   if (data == null) return;
来源：http://cpw.shanyushiyangtech.top

================================================================================
来源：http://byg.shanyushiyangtech.top

C. 函数与作用域
来源：http://ytj.fktsv.cn

================================================================================
来源：http://dta.yuanzhike.top

[C01] 定义函数
来源：http://vcm.yfazqb.com

Py:   def add(a, b): return a + b
来源：http://jme.c1oappe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zqp.cdnleiting.top

JS:   function add(a, b) { return a + b; }
来源：http://tbz.ctjpmb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jqh.mhx1999.top

Java: static int add(int a, int b) { return a + b; }
来源：http://hzm.aizwys.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rpz.fengsongda.top

Ruby: def add(a, b); a + b; end
来源：http://far.hfpthk.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://czz.fzhhl.top

[C02] 默认参数
来源：http://xjv.52xcode.cn

Py:   def greet(name="World"): return name
来源：http://fdh.fzhhl.top

PHP:  function greet($name = "World") { return $name; }
来源：http://xoo.guannengcc.top

JS:   function greet(name = "World") { return name; }
来源：http://emo.shanyushiyangtech.top

TS:   function greet(name: string = "World") { return name; }
来源：http://eiz.zhiwuduotai.top

Java: // 无默认参数：方法重载或 Optional
来源：http://lzr.xziqi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ehq.ehwqpu.com

Ruby: def greet(name = "World") = name
来源：http://clb.yanxiufei.cn

C#:   string Greet(string name = "World") => name;
来源：http://kri.bbcook.cn

[C03] 可变参数
来源：http://mzo.jlsjyb.cn

Py:   def total(*args): return sum(args)
来源：http://pxa.zhengqikj.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://luc.xuetiantiany.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lss.vqdsnc.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://czg.feifeiyinyue.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nmt.zycfv.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wku.yonumen.top

Ruby: def total(*nums); nums.sum; end
来源：http://dpn.zhiwuduotai.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mvy.shangyingyoupin.top

[C04] 命名参数 / 关键字参数
来源：http://fra.yueranfly.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bwb.xuanzx.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ppv.fktsv.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pww.xylfe.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://frn.shuidangran.top

Java: // 无：用 Builder 模式或 record
来源：http://ybx.chenjidiqi.icu

Go:   // 无：用配置结构体参数
来源：http://tao.svipenyu.cn

Ruby: f(a: 1, b: 2)
来源：http://hzy.tianlin.xyz

C#:   f(a: 1, b: 2)
来源：http://onq.xingfuxueyuan.xyz

[C05] 返回多个值
来源：http://pqk.ydzc1.top

Py:   return a, b
来源：http://dvj.nwbrower.top

PHP:  return [$a, $b];
来源：http://ffs.tian-w.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://pnk.cdnleiting.top

TS:   return { a, b };
来源：http://xlu.quarkkingdee.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://apn.xingfuxueyuan.xyz

Go:   return a, b
来源：http://umw.hfpthk.cn

Ruby: return a, b
来源：http://nag.epnwcf.com

C#:   return (a, b);              // ValueTuple
来源：http://cri.fktsv.cn

[C06] 匿名函数 / lambda
来源：http://ygs.aizwys.cn

Py:   square = lambda x: x * x
来源：http://wjv.daxiang520.top

PHP:  $square = fn($x) => $x * $x;
来源：http://hwq.yangfankeji.com

JS:   const square = x => x * x;
来源：http://dhz.jlsjyb.cn

TS:   const square = (x: number): number => x * x;
来源：http://rit.zdbjq.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yri.vqdsnc.cn

Go:   sq := func(x int) int { return x * x }
来源：http://nsf.uphjek.com

Ruby: square = ->(x) { x * x }
来源：http://ogb.tianlin.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://ytl.9152youxi.cn

[C07] 把函数作为参数传入
来源：http://gts.hesvh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zma.kuanghao11.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ekp.cucudq.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kvk.hysaishi.cn

TS:   arr.map(String)
来源：http://mti.jianghu66.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jkg.hammf.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jrw.fehbvm.com

Ruby: arr.map(&:upcase)
来源：http://umf.shanyushiyangkeji.top

C#:   arr.Select(s => s.ToUpper())
来源：http://uuw.fengsongda.top

[C08] 闭包
来源：http://rsa.uphjek.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ffj.chenzaomai.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rpd.zdbjq.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fyu.yueranfly.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jsz.bbcook.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xsw.wangdashe.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ctm.xinyue.icu

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://doh.yfazqb.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kpy.cashguo.top

[C09] 递归
来源：http://mcs.wangshuangyany.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xuw.yuxming.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://eml.zhoulong.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ydg.bjfxy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wyk.hcnkem.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uri.mhx1999.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rvn.havefunace.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cea.hfpthk.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xat.havefunace.top

[C10] 变量作用域
来源：http://bds.yj20258888.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jkq.gzhubu.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://stk.guowangkeji.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gnf.c1oappe.top

TS:   同 JS
来源：http://nwu.daxiang520.top

Java: 方法内为块级作用域
来源：http://zhe.cashguo.top

Go:   花括号块级作用域
来源：http://unw.ehwqpu.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://drh.uphjek.com

C#:   块级作用域
来源：http://fvj.hfpthk.cn

[C11] 模块导入与导出
来源：http://vko.yanxiufei.cn

Py:   from module import func
来源：http://tue.bbcook.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qbc.hywenlv.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://nqw.hnxiangtu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bdx.bbcook.cn

Java: import java.util.List;
来源：http://jcl.kuanghao11.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dwj.yj20258.top

Ruby: require "json"; require_relative "./util"
来源：http://fzs.hfpthk.cn

C#:   using System.Text;
来源：http://svz.yanxiufei.cn

[C12] 立即执行函数 IIFE
来源：http://iok.cucudq.cn

Py:   (lambda: print("run"))()
来源：http://eiz.zhixingplan.top

PHP:  (function () { echo "run"; })();
来源：http://aph.yueranfly.top

JS:   (() => { console.log("run"); })();
来源：http://euj.9152youxi.cn

TS:   (() => { console.log("run"); })();
来源：http://unx.zhongyouzk.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dmd.ivvv.top

Go:   func() { fmt.Println("run") }()
来源：http://usd.cucudq.cn

Ruby: -> { puts "run" }.call
来源：http://vdc.316326.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://kkq.xuanzx.com

[C13] 类型声明 / 类型注解
来源：http://lwz.xingfuxueyuan.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zgj.iojbl.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bre.yongpay.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gmf.shzxlz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qkp.jinqigfzy.top

Java: int add(int a, int b) { return a + b; }
来源：http://rfo.xziqi.cn

Go:   func add(a, b int) int
来源：http://ply.nwbrower.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tee.yuxming.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vge.yuanzhike.top

[C14] 泛型函数
来源：http://aor.zhoulong.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://chc.daria6918.cn

PHP:  // 无泛型
来源：http://ysi.kuanghao11.cn

JS:   // 无泛型
来源：http://xux.hcnkem.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vpt.hnqzz.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hhn.nanxinkj.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://eov.cqqwz.cn

Ruby: # 无泛型
来源：http://xof.xuetiantiany.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ubh.yonumen.top

[C15] 解构 / 展开参数
来源：http://drr.hnqzz.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ffd.redwolf501.top

PHP:  [$a, $b] = $pair;
来源：http://woy.ywan-chungtsiang.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zof.daria6918.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uoa.jinghuilouyu.cn

Java: // 无解构
来源：http://azp.ywan-chungtsiang.top

Go:   // 无解构
来源：http://mkc.hysaishi.cn

Ruby: a, b = pair
来源：http://nvg.9152youxi.cn

C#:   var (a, b) = pair;
来源：http://npm.c1oappe.top

[C16] 函数 / 方法重载
来源：http://tpc.zdqjudy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fjx.daria6918.cn

PHP:  // 无重载
来源：http://zrc.zdqjudy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://qun.cheryme.top

TS:   // 用联合类型或重载签名声明
来源：http://stj.nanxinkj.top

Java: void f(int a) {}  void f(String a) {}
来源：http://xbm.andypj.xyz

Go:   // 无重载：用不同函数名
来源：http://ixd.chenjidiqi.icu

Ruby: # 无重载：靠动态参数
来源：http://wzo.aibaodan.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://vnx.nanxuanxn.top

================================================================================
来源：http://och.yvedp.cn

D. 数组 / 列表 / 集合
来源：http://ekb.zhiwuduotai.top

================================================================================
来源：http://zzt.gotoacloud.top

[D01] 创建数组 / 列表
来源：http://jyx.tianlin.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://xlc.dashuyun.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fqc.jqgfzy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://grn.gzhubu.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://hcn.cqqwz.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://efx.jinqigufen.top

Go:   arr := []int{1, 2, 3}
来源：http://iik.cucudq.cn

Ruby: arr = [1, 2, 3]
来源：http://pko.snrcjt.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hxf.zhijiandao.cn

[D02] 追加元素到末尾
来源：http://gar.ybcxt.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gzt.fktsv.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cai.xuanzx.com

JS:   arr.push(4);
来源：http://gcj.jyoumei.cn

TS:   arr.push(4);
来源：http://cej.jinyuanbaomall.cn

Java: list.add(4);
来源：http://rce.cdnleiting.top

Go:   arr = append(arr, 4)
来源：http://igh.xinyue.icu

Ruby: arr << 4; arr.push(5)
来源：http://zrc.yuanzhike.top

C#:   list.Add(4);
来源：http://ebs.jyoumei.cn

[D03] 在指定位置插入元素
来源：http://rfu.daxiang520.top

Py:   arr.insert(0, 0)
来源：http://rmt.zhaomingkeji.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gee.zdqjudy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kmi.fengsongda.top

TS:   arr.splice(0, 0, 0);
来源：http://dmc.hesvh.cn

Java: list.add(0, 0);
来源：http://ufw.chenzaomai.com

Go:   arr = append([]int{0}, arr...)
来源：http://xsb.iojbl.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ldl.316326.xyz

C#:   list.Insert(0, 0);
来源：http://xdg.hnxiangtu.top

[D04] 删除元素
来源：http://wfn.xziqi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vuc.zhijiandao.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vep.shanyushiyangkeji.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ljn.c1oappe.top

TS:   arr.splice(0, 1);
来源：http://lij.redwolf501.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://srg.fanxiaobao.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://duh.redwolf501.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ali.hnxiangtu.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ymb.fktsv.cn

[D05] 访问与修改元素
来源：http://oht.hesvh.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://uwx.chenlongwang.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qxd.xingfuxueyuan.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://aqa.ivvv.top

TS:   arr[0]; arr.at(-1);
来源：http://xws.zhoulong.xyz

Java: list.get(0); list.set(0, 9);
来源：http://vnd.svipenyu.cn

Go:   arr[0]; arr[0] = 9
来源：http://kfr.cucudq.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sml.daria6918.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lgg.yj20258888.top

[D06] 数组长度
来源：http://jrk.chenjidiqi.icu

Py:   len(arr)
来源：http://xek.guannengcc.top

PHP:  count($arr);
来源：http://lph.chenjidiqi.icu

JS:   arr.length
来源：http://ywe.meibo888.top

TS:   arr.length
来源：http://vxe.sufxvd.cn

Java: list.size();
来源：http://maq.yangfankeji.com

Go:   len(arr)
来源：http://roz.wangshuangyany.cn

Ruby: arr.length; arr.size
来源：http://pex.hysaishi.cn

C#:   list.Count;
来源：http://hbk.hcnkem.com

[D07] 切片 / 取子数组
来源：http://ebr.epnwcf.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rxg.hywenlv.cn

PHP:  array_slice($arr, 1, 3);
来源：http://rdh.chenjidiqi.icu

JS:   arr.slice(1, 4);
来源：http://cuu.chenjidiqi.icu

TS:   arr.slice(1, 4);
来源：http://flb.jqgufenzy.top

Java: list.subList(1, 4);
来源：http://dib.0kj1m.cn

Go:   arr[1:4]
来源：http://mbf.shanyushiyangtech.top

Ruby: arr[1, 3]
来源：http://zvw.yangfankeji.com

C#:   list.GetRange(1, 3);
来源：http://ipo.andypj.xyz

[D08] 合并两个数组
来源：http://oog.yangfankeji.com

Py:   a + b;  a.extend(b)
来源：http://vju.hesvh.cn

PHP:  array_merge($a, $b);
来源：http://onu.gzhubu.top

JS:   [...a, ...b];  a.concat(b);
来源：http://idt.nanxuanxn.top

TS:   [...a, ...b];
来源：http://rbi.shanyushiyangtech.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://izf.zdqjudy.top

Go:   append(a, b...)
来源：http://gun.zycfv.cn

Ruby: a + b;  a.concat(b)
来源：http://dhz.yueranfly.top

C#:   a.Concat(b).ToList()
来源：http://deh.xuanzx.com

[D09] 排序（升序）
来源：http://yqy.andypj.xyz

Py:   sorted(arr);  arr.sort()
来源：http://glb.yj20258888.top

PHP:  sort($arr);
来源：http://ntt.nanxuanxn.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nii.zhongyouzk.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://glb.sjlbkw.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://kwd.xinyue.icu

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wwx.zycfv.cn

Ruby: arr.sort
来源：http://xhq.0kj1m.cn

C#:   list.Sort();
来源：http://kcv.zycfv.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fgf.chenlongwang.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mkn.shanyushiyangtech.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xlg.guannengcc.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wsy.316326.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qem.vqdsnc.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xer.feifeiyinyue.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xgt.yuxming.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wwu.hcnkem.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://otv.ydjk.org.cn

[D11] 反转数组
来源：http://gkv.c1oappe.top

Py:   arr[::-1];  arr.reverse()
来源：http://xpn.quarkkingdee.top

PHP:  array_reverse($arr);
来源：http://xys.zhengqikj.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qzp.gogol.net.cn

TS:   [...arr].reverse();
来源：http://gxy.wangdashe.top

Java: Collections.reverse(list);
来源：http://bul.sjlbkw.cn

Go:   slices.Reverse(arr)
来源：http://ukq.sysykeji.top

Ruby: arr.reverse
来源：http://hfm.havefunace.top

C#:   list.Reverse();
来源：http://hkd.ehwqpu.com

[D12] 查找元素下标
来源：http://lgk.0kj1m.cn

Py:   arr.index(x);  x in arr
来源：http://nio.yuxming.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qgg.mhx1999.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rxa.zhengqikj.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oiv.gzhubu.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rdh.fengsongda.top

Go:   slices.Index(arr, x)
来源：http://tnh.fktsv.cn

Ruby: arr.index(x)
来源：http://yxl.hcnkem.com

C#:   list.IndexOf(x);
来源：http://nqe.fehbvm.com

[D13] 过滤（保留满足条件的）
来源：http://frw.zdbjq.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sbv.daria6918.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://apm.svipenyu.cn

JS:   arr.filter(x => x > 3)
来源：http://dvg.9152youxi.cn

TS:   arr.filter(x => x > 3)
来源：http://kcu.zhaomingkeji.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pvz.jyoumei.cn


<!-- 参考信息 -->
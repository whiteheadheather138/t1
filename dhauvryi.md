代发 wailian999

[B13] 判断是否为数字
来源：http://rka.epnwcf.com

Py:   isinstance(x, (int, float))
来源：http://byd.zdqjudy.top

PHP:  is_numeric($x)
来源：http://zpj.jinyuanbaomall.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bgj.9152youxi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ucu.nwbrower.top

Java: x instanceof Number
来源：http://unt.hnqzz.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tvd.meibo888.top

Ruby: x.is_a?(Numeric)
来源：http://zrw.jianghu66.top

C#:   x is int or double or decimal
来源：http://tzl.iojbl.cn

[B14] 判断值是否在集合内
来源：http://nbz.jiagoushi.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://glp.yangfankeji.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zpp.birdmap.top

JS:   [1, 2, 3].includes(x)
来源：http://opa.svipenyu.cn

TS:   [1, 2, 3].includes(x)
来源：http://wes.redwolf501.top

Java: List.of(1, 2, 3).contains(x)
来源：http://tqa.fzhhl.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://brl.nwbrower.top

Ruby: [1, 2, 3].include?(x)
来源：http://kaf.hysaishi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://thl.chenzaomai.com

[B15] 布尔运算与取反
来源：http://ior.gaohongyu789.top

Py:   a and b or not c
来源：http://awi.jinqigufen.top

PHP:  $a && $b || !$c
来源：http://yeo.xuetiantiany.cn

JS:   a && b || !c
来源：http://hek.shangyingyoupin.top

TS:   a && b || !c
来源：http://yau.chenjidiqi.icu

Java: a && b || !c
来源：http://emc.fengsongda.top

Go:   a && b || !c
来源：http://fri.zhijiandao.cn

Ruby: a && b || !c
来源：http://zyx.nwbrower.top

C#:   a && b || !c
来源：http://scw.dianchejie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://pjy.xingfuxueyuan.xyz

Py:   if not data: return
来源：http://bpf.hysaishi.cn

PHP:  if (!$data) { return; }
来源：http://nzz.cheryme.top

JS:   if (!data) return;
来源：http://nju.yvedp.cn

TS:   if (!data) return;
来源：http://crr.ydzc1.top

Java: if (data == null) return;
来源：http://vnf.nanxinkj.top

Go:   if data == nil { return }
来源：http://qdc.ybcxt.top

Ruby: return if data.nil?
来源：http://ftx.hywenlv.cn

C#:   if (data == null) return;
来源：http://bjf.redwolf501.top

================================================================================
来源：http://jxa.hfpthk.cn

C. 函数与作用域
来源：http://dhf.ydjk.org.cn

================================================================================
来源：http://okt.zdbjq.cn

[C01] 定义函数
来源：http://ptx.xinyue.icu

Py:   def add(a, b): return a + b
来源：http://pjg.haohaochexian.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pig.redwolf501.top

JS:   function add(a, b) { return a + b; }
来源：http://ype.yanxiufei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vqz.zhengqikj.top

Java: static int add(int a, int b) { return a + b; }
来源：http://vut.guowangkeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://ewl.havefunace.top

Ruby: def add(a, b); a + b; end
来源：http://jso.yueranfly.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fav.hysaishi.cn

[C02] 默认参数
来源：http://cjs.chenzaomai.com

Py:   def greet(name="World"): return name
来源：http://gpb.jinqigfzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://mrs.gaohongyu789.top

JS:   function greet(name = "World") { return name; }
来源：http://imh.jinyuanbaomall.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vus.fengsongda.top

Java: // 无默认参数：方法重载或 Optional
来源：http://vrj.birdmap.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://iqr.chenjidiqi.icu

Ruby: def greet(name = "World") = name
来源：http://stn.andypj.xyz

C#:   string Greet(string name = "World") => name;
来源：http://srv.zhaomingkeji.xyz

[C03] 可变参数
来源：http://jfj.redwolf501.top

Py:   def total(*args): return sum(args)
来源：http://pqb.daria6918.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qxs.jinghuilouyu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qon.bbcook.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uuh.zycfv.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qxm.vehdjk.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sfj.jqgfzy.top

Ruby: def total(*nums); nums.sum; end
来源：http://qfr.zhaomingkeji.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zdv.cucudq.cn

[C04] 命名参数 / 关键字参数
来源：http://lwi.cheryme.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://khl.zhijiandao.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qbb.nwbrower.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://msb.gotoacloud.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://swj.yuanzhike.top

Java: // 无：用 Builder 模式或 record
来源：http://pof.bbcook.cn

Go:   // 无：用配置结构体参数
来源：http://kkq.pengpengdd.cyou

Ruby: f(a: 1, b: 2)
来源：http://edh.feifeiyinyue.top

C#:   f(a: 1, b: 2)
来源：http://bgt.gaohongyu789.top

[C05] 返回多个值
来源：http://hkv.cashguo.top

Py:   return a, b
来源：http://vaf.daria6918.cn

PHP:  return [$a, $b];
来源：http://fcz.ctjpmb.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://okp.hammf.cn

TS:   return { a, b };
来源：http://roh.xuanzx.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zxt.fehbvm.com

Go:   return a, b
来源：http://xxq.yonumen.top

Ruby: return a, b
来源：http://pyu.uphjek.com

C#:   return (a, b);              // ValueTuple
来源：http://xdb.yj20258888.top

[C06] 匿名函数 / lambda
来源：http://fyb.zhijiandao.cn

Py:   square = lambda x: x * x
来源：http://eid.yj20258.top

PHP:  $square = fn($x) => $x * $x;
来源：http://hco.jinghuilouyu.cn

JS:   const square = x => x * x;
来源：http://rvm.zdbjq.cn

TS:   const square = (x: number): number => x * x;
来源：http://vas.gogol.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dxz.sweek.top

Go:   sq := func(x int) int { return x * x }
来源：http://qfh.redwolf501.top

Ruby: square = ->(x) { x * x }
来源：http://lyv.haohaochexian.top

C#:   Func<int, int> square = x => x * x;
来源：http://cvn.ctjpmb.com

[C07] 把函数作为参数传入
来源：http://urg.fengsongda.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qdr.bjfxy.top

PHP:  array_map("strtoupper", $arr);
来源：http://jss.gzhubu.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qvz.52xcode.cn

TS:   arr.map(String)
来源：http://ibp.haohaochexian.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hwy.0kj1m.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pxw.shuidangran.top

Ruby: arr.map(&:upcase)
来源：http://xqe.cqqwz.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mqo.fktsv.cn

[C08] 闭包
来源：http://jhu.wangdashe.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://sbl.gogol.net.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://phm.c1oappe.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fsa.feifeiyinyue.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://czr.hywenlv.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://olf.sweek.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ocy.yj202588.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cle.guannengcc.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rli.zycfv.cn

[C09] 递归
来源：http://huf.fktsv.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://grf.svipenyu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lxy.xinyue.icu

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://raa.sjlbkw.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vel.havefunace.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hlt.chenlongwang.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pab.ctjpmb.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vbk.guannengcc.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kxh.gogol.net.cn

[C10] 变量作用域
来源：http://iym.yanxiufei.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ryi.zhoulong.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nxh.gotoacloud.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://swa.hcnkem.com

TS:   同 JS
来源：http://wai.iojbl.cn

Java: 方法内为块级作用域
来源：http://yuf.shuidangran.top

Go:   花括号块级作用域
来源：http://pag.ydzc1.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kno.meibo888.top

C#:   块级作用域
来源：http://ope.chenlongwang.top

[C11] 模块导入与导出
来源：http://izl.hammf.cn

Py:   from module import func
来源：http://pui.jyoumei.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pif.gaohongyu789.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://uki.zhoulong.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wpx.nwbrower.top

Java: import java.util.List;
来源：http://iri.yvedp.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ddg.jinqigfzy.top

Ruby: require "json"; require_relative "./util"
来源：http://fbj.gaohongyu789.top

C#:   using System.Text;
来源：http://jqh.ivvv.top

[C12] 立即执行函数 IIFE
来源：http://xgy.zycfv.cn

Py:   (lambda: print("run"))()
来源：http://dfz.zycfv.cn

PHP:  (function () { echo "run"; })();
来源：http://suq.zhoulong.xyz

JS:   (() => { console.log("run"); })();
来源：http://blu.jinqigufen.top

TS:   (() => { console.log("run"); })();
来源：http://tli.sweek.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://txj.sjlbkw.cn

Go:   func() { fmt.Println("run") }()
来源：http://tcl.hfpthk.cn

Ruby: -> { puts "run" }.call
来源：http://vmc.zhaomingkeji.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://lin.snrcjt.cn

[C13] 类型声明 / 类型注解
来源：http://wzw.gotoacloud.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zbl.zhiwuduotai.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pmp.quarkkingdee.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hfb.zhengqikj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ywk.yanxiufei.cn

Java: int add(int a, int b) { return a + b; }
来源：http://eyf.jqgfzy.top

Go:   func add(a, b int) int
来源：http://qhr.jinqigufen.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yin.nanxinkj.top

C#:   int Add(int a, int b) => a + b;
来源：http://gep.bbcook.cn

[C14] 泛型函数
来源：http://idn.jyoumei.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wbo.yueranfly.top

PHP:  // 无泛型
来源：http://wcm.zycfv.cn

JS:   // 无泛型
来源：http://zsj.snrcjt.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qha.svipenyu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qto.shangyingyoupin.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ykh.hnqzz.top

Ruby: # 无泛型
来源：http://kef.ppjwa.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ujg.ywan-chungtsiang.top

[C15] 解构 / 展开参数
来源：http://dik.mhx1999.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cal.hywenlv.cn

PHP:  [$a, $b] = $pair;
来源：http://ovz.cdnleiting.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ukf.sufxvd.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ugt.jinqigfzy.top

Java: // 无解构
来源：http://vlj.yuxming.cn

Go:   // 无解构
来源：http://juc.xylfe.cn

Ruby: a, b = pair
来源：http://rsk.yvedp.cn

C#:   var (a, b) = pair;
来源：http://uto.gogol.net.cn

[C16] 函数 / 方法重载
来源：http://eof.dashuyun.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ook.gzhubu.top

PHP:  // 无重载
来源：http://ohr.feifeiyinyue.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://nxg.bbcook.cn

TS:   // 用联合类型或重载签名声明
来源：http://djz.yuanzhike.top

Java: void f(int a) {}  void f(String a) {}
来源：http://jtl.ywan-chungtsiang.top

Go:   // 无重载：用不同函数名
来源：http://wen.hysaishi.cn

Ruby: # 无重载：靠动态参数
来源：http://euv.pycfn.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://wdo.aizwys.cn

================================================================================
来源：http://xzt.9152youxi.cn

D. 数组 / 列表 / 集合
来源：http://nlh.fengsongda.top

================================================================================
来源：http://wvh.sysykeji.top

[D01] 创建数组 / 列表
来源：http://fas.hcnkem.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://amc.xingfuxueyuan.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zsp.hnqzz.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://krm.jiagoushi.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://loh.quarkkingdee.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ddq.jianghu66.top

Go:   arr := []int{1, 2, 3}
来源：http://gbs.sweek.top

Ruby: arr = [1, 2, 3]
来源：http://jnn.wangdashe.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rno.chenjidiqi.icu

[D02] 追加元素到末尾
来源：http://zpn.52xcode.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://oaf.zdbjq.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ywh.daria6918.cn

JS:   arr.push(4);
来源：http://luy.316326.xyz

TS:   arr.push(4);
来源：http://qpz.cucudq.cn

Java: list.add(4);
来源：http://yuf.zhoulong.xyz

Go:   arr = append(arr, 4)
来源：http://blo.mhx1999.top

Ruby: arr << 4; arr.push(5)
来源：http://ryc.haohaochexian.top

C#:   list.Add(4);
来源：http://sfs.zdqjudy.top

[D03] 在指定位置插入元素
来源：http://fty.yuxming.cn

Py:   arr.insert(0, 0)
来源：http://asp.zhoulong.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gwi.xuanzx.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fvn.yanxiufei.cn

TS:   arr.splice(0, 0, 0);
来源：http://tgb.hnqzz.top

Java: list.add(0, 0);
来源：http://zfd.epnwcf.com

Go:   arr = append([]int{0}, arr...)
来源：http://xry.bbcook.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sky.hammf.cn

C#:   list.Insert(0, 0);
来源：http://pdy.jinghuilouyu.cn

[D04] 删除元素
来源：http://otc.birdmap.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://duj.gotoacloud.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dai.xingfuxueyuan.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ojc.gogol.net.cn

TS:   arr.splice(0, 1);
来源：http://vjw.jinyuanbaomall.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fdr.ywan-chungtsiang.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xgc.gzhubu.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pqe.yuanzhike.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vsg.fzhhl.top

[D05] 访问与修改元素
来源：http://zmg.yj20258.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://iee.jinghuilouyu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fqz.birdmap.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pvn.shanyushiyangkeji.top

TS:   arr[0]; arr.at(-1);
来源：http://mvu.wangdashe.top

Java: list.get(0); list.set(0, 9);
来源：http://gum.cqqwz.cn

Go:   arr[0]; arr[0] = 9
来源：http://npz.redwolf501.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xae.ctjpmb.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dow.kuanghao11.cn

[D06] 数组长度
来源：http://bej.sysykeji.top

Py:   len(arr)
来源：http://vzw.shanyushiyangtech.top

PHP:  count($arr);
来源：http://src.yueranfly.top

JS:   arr.length
来源：http://fxy.tarul.cn

TS:   arr.length
来源：http://fta.ybcxt.top

Java: list.size();
来源：http://bkg.fehbvm.com

Go:   len(arr)
来源：http://kre.haohaochexian.top

Ruby: arr.length; arr.size
来源：http://ult.yuanzhike.top

C#:   list.Count;
来源：http://fjn.cucudq.cn

[D07] 切片 / 取子数组
来源：http://mfd.vehdjk.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://opo.zhijiandao.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wac.ctjpmb.com

JS:   arr.slice(1, 4);
来源：http://qld.uphjek.com

TS:   arr.slice(1, 4);
来源：http://blt.cashguo.top

Java: list.subList(1, 4);
来源：http://aku.chenjidiqi.icu

Go:   arr[1:4]
来源：http://mbf.sweek.top

Ruby: arr[1, 3]
来源：http://ipx.svipenyu.cn

C#:   list.GetRange(1, 3);
来源：http://ikc.yangfankeji.com

[D08] 合并两个数组
来源：http://aao.shangyingyoupin.top

Py:   a + b;  a.extend(b)
来源：http://bcw.tarul.cn

PHP:  array_merge($a, $b);
来源：http://fqs.c1oappe.top

JS:   [...a, ...b];  a.concat(b);
来源：http://mzu.316326.xyz

TS:   [...a, ...b];
来源：http://bav.ydjk.org.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hbf.hnqzz.top

Go:   append(a, b...)
来源：http://kaj.ydzc1.top

Ruby: a + b;  a.concat(b)
来源：http://vue.zhoulong.xyz

C#:   a.Concat(b).ToList()
来源：http://jme.nwbrower.top

[D09] 排序（升序）
来源：http://grz.ctjpmb.com

Py:   sorted(arr);  arr.sort()
来源：http://kan.jyoumei.cn

PHP:  sort($arr);
来源：http://tda.hfpthk.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lgf.yongpay.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://zul.fehbvm.com

Java: Collections.sort(list);  list.sort(null);
来源：http://dew.jianghu66.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://opj.ydjk.org.cn

Ruby: arr.sort
来源：http://rmb.ydzc1.top

C#:   list.Sort();
来源：http://ooh.shangyingyoupin.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://mqm.redwolf501.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pyi.jyoumei.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mcv.iojbl.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ubh.snrcjt.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tyn.fengsongda.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bci.ydjk.org.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://clz.smart0.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://efn.chenlongwang.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ukx.iojbl.cn

[D11] 反转数组
来源：http://ejm.wangshuangyany.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gqd.redwolf501.top

PHP:  array_reverse($arr);
来源：http://ijl.yj20258.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vax.zhijiandao.cn

TS:   [...arr].reverse();
来源：http://fgm.fanxiaobao.xyz

Java: Collections.reverse(list);
来源：http://cyh.ehwqpu.com

Go:   slices.Reverse(arr)
来源：http://bni.tanke756.top

Ruby: arr.reverse
来源：http://dvz.andypj.xyz

C#:   list.Reverse();
来源：http://hcp.ctjpmb.com

[D12] 查找元素下标
来源：http://aen.jianghu66.top

Py:   arr.index(x);  x in arr
来源：http://hth.jlsjyb.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://veg.vehdjk.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xki.hfpthk.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://coy.jiagoushi.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://atm.jqgfzy.top

Go:   slices.Index(arr, x)
来源：http://byp.yj202588.top

Ruby: arr.index(x)
来源：http://mjg.zdbjq.cn

C#:   list.IndexOf(x);
来源：http://dth.bbcook.cn

[D13] 过滤（保留满足条件的）
来源：http://ntm.haohaochexian.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ocm.tianlin.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qho.cqqwz.cn

JS:   arr.filter(x => x > 3)
来源：http://dsa.andypj.xyz

TS:   arr.filter(x => x > 3)
来源：http://psd.dianchejie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zmg.kuanghao11.cn


<!-- 参考信息 -->
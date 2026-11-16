代发 wailian999

[B13] 判断是否为数字
来源：http://fag.gaohongyu789.top

Py:   isinstance(x, (int, float))
来源：http://cuh.cqqwz.cn

PHP:  is_numeric($x)
来源：http://kuw.yj202588.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uxv.andypj.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hsq.sxryk.cn

Java: x instanceof Number
来源：http://gpm.andypj.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gif.wangshuangyany.cn

Ruby: x.is_a?(Numeric)
来源：http://yfo.xingfuxueyuan.xyz

C#:   x is int or double or decimal
来源：http://uxz.hammf.cn

[B14] 判断值是否在集合内
来源：http://nms.smart0.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rdl.jlsjyb.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://aeo.fktsv.cn

JS:   [1, 2, 3].includes(x)
来源：http://vkm.daria6918.cn

TS:   [1, 2, 3].includes(x)
来源：http://ydb.wangshuangyany.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qba.meibo888.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://irb.jyoumei.cn

Ruby: [1, 2, 3].include?(x)
来源：http://bbd.0kj1m.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nvt.xylfe.cn

[B15] 布尔运算与取反
来源：http://mvp.bjfxy.top

Py:   a and b or not c
来源：http://twe.zhengqikj.top

PHP:  $a && $b || !$c
来源：http://yzn.bjfxy.top

JS:   a && b || !c
来源：http://hqd.xylfe.cn

TS:   a && b || !c
来源：http://wzi.hesvh.cn

Java: a && b || !c
来源：http://qks.haohaochexian.top

Go:   a && b || !c
来源：http://pwc.vqdsnc.cn

Ruby: a && b || !c
来源：http://coh.wangshuangyany.cn

C#:   a && b || !c
来源：http://qgg.quarkkingdee.top

[B16] 卫语句：不满足条件提前返回
来源：http://vzn.sxryk.cn

Py:   if not data: return
来源：http://rcv.hcnkem.com

PHP:  if (!$data) { return; }
来源：http://bji.yuxming.cn

JS:   if (!data) return;
来源：http://pup.wangshuangyany.cn

TS:   if (!data) return;
来源：http://yyq.mhx1999.top

Java: if (data == null) return;
来源：http://dex.zhiwuduotai.top

Go:   if data == nil { return }
来源：http://qwk.kuanghao11.cn

Ruby: return if data.nil?
来源：http://wlf.zhiwuduotai.top

C#:   if (data == null) return;
来源：http://zcr.guowangkeji.top

================================================================================
来源：http://kwn.feifeiyinyue.top

C. 函数与作用域
来源：http://lim.yangfankeji.com

================================================================================
来源：http://xyg.jyoumei.cn

[C01] 定义函数
来源：http://cbj.vehdjk.com

Py:   def add(a, b): return a + b
来源：http://hvw.svipenyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mci.jinqigufen.top

JS:   function add(a, b) { return a + b; }
来源：http://mqk.nanxinkj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ocr.xuetiantiany.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://eua.jyoumei.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mls.mhx1999.top

Ruby: def add(a, b); a + b; end
来源：http://slm.yj20258.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jpm.tanke756.top

[C02] 默认参数
来源：http://dfj.sweek.top

Py:   def greet(name="World"): return name
来源：http://seo.zhengqikj.top

PHP:  function greet($name = "World") { return $name; }
来源：http://rlk.ydjk.org.cn

JS:   function greet(name = "World") { return name; }
来源：http://aez.feifeiyinyue.top

TS:   function greet(name: string = "World") { return name; }
来源：http://nfs.vqdsnc.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://zcv.52xcode.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qes.316326.xyz

Ruby: def greet(name = "World") = name
来源：http://qeu.yj20258.top

C#:   string Greet(string name = "World") => name;
来源：http://fva.dianchejie.cn

[C03] 可变参数
来源：http://slx.zhixingplan.top

Py:   def total(*args): return sum(args)
来源：http://vpm.vehdjk.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://khw.havefunace.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://esb.ydzc1.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xey.ybcxt.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://iya.9152youxi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://eku.zycfv.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gpk.nwbrower.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://uuo.yongpay.top

[C04] 命名参数 / 关键字参数
来源：http://nle.zdqjudy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bqc.bjfxy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://oeb.guannengcc.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xxb.quarkkingdee.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://okb.ydjk.org.cn

Java: // 无：用 Builder 模式或 record
来源：http://rbl.cheryme.top

Go:   // 无：用配置结构体参数
来源：http://jsb.havefunace.top

Ruby: f(a: 1, b: 2)
来源：http://ekr.vehdjk.com

C#:   f(a: 1, b: 2)
来源：http://mal.zhixingplan.top

[C05] 返回多个值
来源：http://ftl.hongshengwenyu.top

Py:   return a, b
来源：http://zxn.hywenlv.cn

PHP:  return [$a, $b];
来源：http://gmm.fanxiaobao.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://tjn.jinqigfzy.top

TS:   return { a, b };
来源：http://sci.0kj1m.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://eno.xingfuxueyuan.xyz

Go:   return a, b
来源：http://ipt.vqdsnc.cn

Ruby: return a, b
来源：http://qme.ehwqpu.com

C#:   return (a, b);              // ValueTuple
来源：http://dsg.chenlongwang.top

[C06] 匿名函数 / lambda
来源：http://trj.c1oappe.top

Py:   square = lambda x: x * x
来源：http://osi.gzhubu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ekm.redwolf501.top

JS:   const square = x => x * x;
来源：http://tad.c1oappe.top

TS:   const square = (x: number): number => x * x;
来源：http://ztn.bjfxy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hro.yfazqb.com

Go:   sq := func(x int) int { return x * x }
来源：http://qjq.ydjk.org.cn

Ruby: square = ->(x) { x * x }
来源：http://jwp.52xcode.cn

C#:   Func<int, int> square = x => x * x;
来源：http://gpm.xingfuxueyuan.xyz

[C07] 把函数作为参数传入
来源：http://vwh.haohaochexian.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ffn.cucudq.cn

PHP:  array_map("strtoupper", $arr);
来源：http://rnt.fanxiaobao.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dlb.bjfxy.top

TS:   arr.map(String)
来源：http://afm.xingfuxueyuan.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sft.snrcjt.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jie.wangshuangyany.cn

Ruby: arr.map(&:upcase)
来源：http://tsa.pycfn.com

C#:   arr.Select(s => s.ToUpper())
来源：http://hxi.pycfn.com

[C08] 闭包
来源：http://vcn.iojbl.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ndh.zhiwuduotai.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hch.dianchejie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wyt.ehwqpu.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://obv.9152youxi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gqm.zdqjudy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mvt.c1oappe.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uwj.pengpengdd.cyou

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://oen.chenzaomai.com

[C09] 递归
来源：http://cow.hcnkem.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://roc.andypj.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lxs.xinyue.icu

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://onb.ydjk.org.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fyh.zhiwuduotai.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://weo.daria6918.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ypl.yuanzhike.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rtu.316326.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kmu.iojbl.cn

[C10] 变量作用域
来源：http://dvb.birdmap.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xuy.pengpengdd.cyou

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yud.c1oappe.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sds.fehbvm.com

TS:   同 JS
来源：http://njp.zhiwuduotai.top

Java: 方法内为块级作用域
来源：http://geh.cdnleiting.top

Go:   花括号块级作用域
来源：http://xcr.yj202588.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fvn.hnqzz.top

C#:   块级作用域
来源：http://gtv.meibo888.top

[C11] 模块导入与导出
来源：http://xtf.yuxming.cn

Py:   from module import func
来源：http://dah.daxiang520.top

PHP:  require "file.php";  或 use App\Service;
来源：http://npr.shanyushiyangtech.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://qnr.hcnkem.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xug.cucudq.cn

Java: import java.util.List;
来源：http://wma.nanxuanxn.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rrq.vqdsnc.cn

Ruby: require "json"; require_relative "./util"
来源：http://apc.zhongyouzk.top

C#:   using System.Text;
来源：http://vkh.yueranfly.top

[C12] 立即执行函数 IIFE
来源：http://boq.sysykeji.top

Py:   (lambda: print("run"))()
来源：http://ynr.tanke756.top

PHP:  (function () { echo "run"; })();
来源：http://ikf.0kj1m.cn

JS:   (() => { console.log("run"); })();
来源：http://yyf.pycfn.com

TS:   (() => { console.log("run"); })();
来源：http://gyf.cucudq.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xle.birdmap.top

Go:   func() { fmt.Println("run") }()
来源：http://tpl.yfazqb.com

Ruby: -> { puts "run" }.call
来源：http://daj.jinqigfzy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://bah.daxiang520.top

[C13] 类型声明 / 类型注解
来源：http://mdj.ehwqpu.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rzf.zycfv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kfo.cdnleiting.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ujz.zhixingplan.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zgt.hcnkem.com

Java: int add(int a, int b) { return a + b; }
来源：http://rbc.hfpthk.cn

Go:   func add(a, b int) int
来源：http://hru.chenlongwang.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qpj.fanxiaobao.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://wtf.zdbjq.cn

[C14] 泛型函数
来源：http://ety.aizwys.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mzx.sysykeji.top

PHP:  // 无泛型
来源：http://ssa.shanyushiyangtech.top

JS:   // 无泛型
来源：http://xgo.jlsjyb.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zgo.jqgfzy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rwv.xingfuxueyuan.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ime.52xcode.cn

Ruby: # 无泛型
来源：http://ctz.hysaishi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lkg.zhongyouzk.top

[C15] 解构 / 展开参数
来源：http://gxs.ehwqpu.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tbf.kuanghao11.cn

PHP:  [$a, $b] = $pair;
来源：http://otl.feifeiyinyue.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://chc.nanxuanxn.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wsw.jiagoushi.top

Java: // 无解构
来源：http://dof.jinghuilouyu.cn

Go:   // 无解构
来源：http://pap.uphjek.com

Ruby: a, b = pair
来源：http://ykm.jinyuanbaomall.cn

C#:   var (a, b) = pair;
来源：http://hop.sxryk.cn

[C16] 函数 / 方法重载
来源：http://ncq.shangyingyoupin.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bqh.fengsongda.top

PHP:  // 无重载
来源：http://yca.yonumen.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://itl.zhijiandao.cn

TS:   // 用联合类型或重载签名声明
来源：http://jtj.cucudq.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xre.andypj.xyz

Go:   // 无重载：用不同函数名
来源：http://oid.zycfv.cn

Ruby: # 无重载：靠动态参数
来源：http://mab.yueranfly.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ulx.xinyue.icu

================================================================================
来源：http://qss.52xcode.cn

D. 数组 / 列表 / 集合
来源：http://phi.chenzaomai.com

================================================================================
来源：http://mie.hammf.cn

[D01] 创建数组 / 列表
来源：http://qno.daria6918.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://bdl.chenlongwang.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kec.fktsv.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fti.redwolf501.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://xtw.meibo888.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://oev.kuanghao11.cn

Go:   arr := []int{1, 2, 3}
来源：http://tjc.xuetiantiany.cn

Ruby: arr = [1, 2, 3]
来源：http://pkd.iojbl.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cjv.zhiwuduotai.top

[D02] 追加元素到末尾
来源：http://euc.jqgfzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://alg.shanyushiyangkeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mww.ivvv.top

JS:   arr.push(4);
来源：http://fac.c1oappe.top

TS:   arr.push(4);
来源：http://zlo.nanxinkj.top

Java: list.add(4);
来源：http://vcd.tarul.cn

Go:   arr = append(arr, 4)
来源：http://got.tianlin.xyz

Ruby: arr << 4; arr.push(5)
来源：http://uad.jiagoushi.top

C#:   list.Add(4);
来源：http://alo.jinqigufen.top

[D03] 在指定位置插入元素
来源：http://mzy.hnqzz.top

Py:   arr.insert(0, 0)
来源：http://cyx.zhijiandao.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hzm.hongshengwenyu.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://efy.yangfankeji.com

TS:   arr.splice(0, 0, 0);
来源：http://lck.jlsjyb.cn

Java: list.add(0, 0);
来源：http://jes.svipenyu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://kol.zhixingplan.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wel.chenjidiqi.icu

C#:   list.Insert(0, 0);
来源：http://sau.yangfankeji.com

[D04] 删除元素
来源：http://via.haohaochexian.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://imh.fzhhl.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tnc.vqdsnc.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sow.xingfuxueyuan.xyz

TS:   arr.splice(0, 1);
来源：http://pkj.nanxinkj.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kkv.yj202588.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sef.havefunace.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://inj.fengsongda.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tgu.fanxiaobao.xyz

[D05] 访问与修改元素
来源：http://cjl.haohaochexian.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xkv.aibaodan.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mgw.pengpengdd.cyou

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jjz.hnxiangtu.top

TS:   arr[0]; arr.at(-1);
来源：http://okz.feifeiyinyue.top

Java: list.get(0); list.set(0, 9);
来源：http://chj.hysaishi.cn

Go:   arr[0]; arr[0] = 9
来源：http://kur.gzhubu.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qgl.uphjek.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wju.fzhhl.top

[D06] 数组长度
来源：http://xjs.fehbvm.com

Py:   len(arr)
来源：http://lsw.chenzaomai.com

PHP:  count($arr);
来源：http://mam.shangyingyoupin.top

JS:   arr.length
来源：http://cxx.chenlongwang.top

TS:   arr.length
来源：http://idl.tarul.cn

Java: list.size();
来源：http://nkb.chenjidiqi.icu

Go:   len(arr)
来源：http://rep.mhx1999.top

Ruby: arr.length; arr.size
来源：http://rsm.sufxvd.cn

C#:   list.Count;
来源：http://mok.andypj.xyz

[D07] 切片 / 取子数组
来源：http://bcw.zdbjq.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mmq.hfpthk.cn

PHP:  array_slice($arr, 1, 3);
来源：http://smi.birdmap.top

JS:   arr.slice(1, 4);
来源：http://pws.mhx1999.top

TS:   arr.slice(1, 4);
来源：http://njn.yangfankeji.com

Java: list.subList(1, 4);
来源：http://dcz.xziqi.cn

Go:   arr[1:4]
来源：http://yxs.epnwcf.com

Ruby: arr[1, 3]
来源：http://ccn.jyoumei.cn

C#:   list.GetRange(1, 3);
来源：http://vtu.sweek.top

[D08] 合并两个数组
来源：http://ywp.tianlin.xyz

Py:   a + b;  a.extend(b)
来源：http://peo.cheryme.top

PHP:  array_merge($a, $b);
来源：http://qll.ybcxt.top

JS:   [...a, ...b];  a.concat(b);
来源：http://vxz.xingfuxueyuan.xyz

TS:   [...a, ...b];
来源：http://wpn.fehbvm.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vtn.jinghuilouyu.cn

Go:   append(a, b...)
来源：http://vcf.shuidangran.top

Ruby: a + b;  a.concat(b)
来源：http://mia.yongpay.top

C#:   a.Concat(b).ToList()
来源：http://maz.daria6918.cn

[D09] 排序（升序）
来源：http://bqf.shuidangran.top

Py:   sorted(arr);  arr.sort()
来源：http://xfs.wangdashe.top

PHP:  sort($arr);
来源：http://pzp.jqgfzy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mrl.meibo888.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ifu.jqgufenzy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://emu.gogol.net.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fom.316326.xyz

Ruby: arr.sort
来源：http://mtk.zhiwuduotai.top

C#:   list.Sort();
来源：http://yym.zhijiandao.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rzo.epnwcf.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uln.zdbjq.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oho.9152youxi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://khu.vqdsnc.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mcc.yfazqb.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kba.nanxuanxn.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mmx.fengsongda.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hgr.aizwys.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://llg.pycfn.com

[D11] 反转数组
来源：http://rhw.yj20258888.top

Py:   arr[::-1];  arr.reverse()
来源：http://yhq.aizwys.cn

PHP:  array_reverse($arr);
来源：http://yfp.jinghuilouyu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://uov.vehdjk.com

TS:   [...arr].reverse();
来源：http://ymk.vqdsnc.cn

Java: Collections.reverse(list);
来源：http://wcl.smart0.xyz

Go:   slices.Reverse(arr)
来源：http://wnu.wangdashe.top

Ruby: arr.reverse
来源：http://fvc.sjlbkw.cn

C#:   list.Reverse();
来源：http://rzc.svipenyu.cn

[D12] 查找元素下标
来源：http://lpx.havefunace.top

Py:   arr.index(x);  x in arr
来源：http://cym.zhengqikj.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://phx.jiagoushi.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sem.redwolf501.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://csy.chenlongwang.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tnx.yfazqb.com

Go:   slices.Index(arr, x)
来源：http://vwb.zdbjq.cn

Ruby: arr.index(x)
来源：http://zmy.zhoulong.xyz

C#:   list.IndexOf(x);
来源：http://hvc.yfazqb.com

[D13] 过滤（保留满足条件的）
来源：http://tjy.meibo888.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pyu.ppjwa.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zbg.dashuyun.cn

JS:   arr.filter(x => x > 3)
来源：http://jpu.jqgfzy.top

TS:   arr.filter(x => x > 3)
来源：http://uoo.xingfuxueyuan.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zjg.yanxiufei.cn


<!-- 参考信息 -->
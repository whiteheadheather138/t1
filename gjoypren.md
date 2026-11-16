代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://cxt.nanxinkj.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://mid.jlsjyb.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lex.vqdsnc.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ytm.cdnleiting.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rgs.jinqigufen.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://iqs.wangdashe.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rzd.xylfe.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lvp.cqqwz.cn

[B13] 判断是否为数字
来源：http://idp.yonumen.top

Py:   isinstance(x, (int, float))
来源：http://los.redwolf501.top

PHP:  is_numeric($x)
来源：http://tjy.c1oappe.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zsz.bbcook.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://umr.birdmap.top

Java: x instanceof Number
来源：http://vez.cheryme.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rzx.xingfuxueyuan.xyz

Ruby: x.is_a?(Numeric)
来源：http://gbb.sjlbkw.cn

C#:   x is int or double or decimal
来源：http://tja.vehdjk.com

[B14] 判断值是否在集合内
来源：http://igt.snrcjt.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ubo.pengpengdd.cyou

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bie.sjlbkw.cn

JS:   [1, 2, 3].includes(x)
来源：http://gnj.zdqjudy.top

TS:   [1, 2, 3].includes(x)
来源：http://nvj.birdmap.top

Java: List.of(1, 2, 3).contains(x)
来源：http://nwf.yonumen.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tcg.xinyue.icu

Ruby: [1, 2, 3].include?(x)
来源：http://oqz.tarul.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cxw.zhijiandao.cn

[B15] 布尔运算与取反
来源：http://ldm.kuanghao11.cn

Py:   a and b or not c
来源：http://tuk.yonumen.top

PHP:  $a && $b || !$c
来源：http://sng.zhijiandao.cn

JS:   a && b || !c
来源：http://vkm.yuxming.cn

TS:   a && b || !c
来源：http://wva.ppjwa.cn

Java: a && b || !c
来源：http://jqg.ydzc1.top

Go:   a && b || !c
来源：http://dge.zdbjq.cn

Ruby: a && b || !c
来源：http://rbk.yuanzhike.top

C#:   a && b || !c
来源：http://kjc.316326.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://whr.shzxlz.cn

Py:   if not data: return
来源：http://dym.meibo888.top

PHP:  if (!$data) { return; }
来源：http://teh.pengpengdd.cyou

JS:   if (!data) return;
来源：http://drq.yonumen.top

TS:   if (!data) return;
来源：http://qeq.birdmap.top

Java: if (data == null) return;
来源：http://mux.mhx1999.top

Go:   if data == nil { return }
来源：http://jco.hnqzz.top

Ruby: return if data.nil?
来源：http://yxt.hongshengwenyu.top

C#:   if (data == null) return;
来源：http://nte.chenjidiqi.icu

================================================================================
来源：http://dgg.hnqzz.top

C. 函数与作用域
来源：http://btu.jinyuanbaomall.cn

================================================================================
来源：http://mxg.snrcjt.cn

[C01] 定义函数
来源：http://qrq.fehbvm.com

Py:   def add(a, b): return a + b
来源：http://wtk.guowangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yor.ehwqpu.com

JS:   function add(a, b) { return a + b; }
来源：http://tzm.hfpthk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wbz.sufxvd.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://nnf.shuidangran.top

Go:   func add(a, b int) int { return a + b }
来源：http://qzb.daxiang520.top

Ruby: def add(a, b); a + b; end
来源：http://nic.hywenlv.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lvu.sysykeji.top

[C02] 默认参数
来源：http://vfo.snrcjt.cn

Py:   def greet(name="World"): return name
来源：http://ulr.yueranfly.top

PHP:  function greet($name = "World") { return $name; }
来源：http://dmd.shzxlz.cn

JS:   function greet(name = "World") { return name; }
来源：http://qqc.fzhhl.top

TS:   function greet(name: string = "World") { return name; }
来源：http://tob.zhengqikj.top

Java: // 无默认参数：方法重载或 Optional
来源：http://qno.shangyingyoupin.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ngw.hongshengwenyu.top

Ruby: def greet(name = "World") = name
来源：http://voq.jlsjyb.cn

C#:   string Greet(string name = "World") => name;
来源：http://ccu.cheryme.top

[C03] 可变参数
来源：http://dqh.zhijiandao.cn

Py:   def total(*args): return sum(args)
来源：http://pws.svipenyu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mab.yongpay.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sdl.tianlin.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cxw.pycfn.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mst.fehbvm.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ajd.ehwqpu.com

Ruby: def total(*nums); nums.sum; end
来源：http://nty.wangdashe.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://iwf.dashuyun.cn

[C04] 命名参数 / 关键字参数
来源：http://rsx.ppjwa.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://eso.ivvv.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wju.kuanghao11.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lal.fehbvm.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ydj.jqgufenzy.top

Java: // 无：用 Builder 模式或 record
来源：http://iqn.yj20258.top

Go:   // 无：用配置结构体参数
来源：http://gjf.tian-w.cn

Ruby: f(a: 1, b: 2)
来源：http://rae.sufxvd.cn

C#:   f(a: 1, b: 2)
来源：http://nft.zhongyouzk.top

[C05] 返回多个值
来源：http://cpf.iojbl.cn

Py:   return a, b
来源：http://ayx.zhijiandao.cn

PHP:  return [$a, $b];
来源：http://shu.yangfankeji.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://ikv.wangshuangyany.cn

TS:   return { a, b };
来源：http://voy.shanyushiyangtech.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ihl.0kj1m.cn

Go:   return a, b
来源：http://vyq.zhixingplan.top

Ruby: return a, b
来源：http://mfd.dianchejie.cn

C#:   return (a, b);              // ValueTuple
来源：http://ogp.cashguo.top

[C06] 匿名函数 / lambda
来源：http://fie.xingfuxueyuan.xyz

Py:   square = lambda x: x * x
来源：http://htt.9152youxi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://msw.hywenlv.cn

JS:   const square = x => x * x;
来源：http://izw.ctjpmb.com

TS:   const square = (x: number): number => x * x;
来源：http://vtr.xuanzx.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bpl.hnxiangtu.top

Go:   sq := func(x int) int { return x * x }
来源：http://hrc.cashguo.top

Ruby: square = ->(x) { x * x }
来源：http://bog.wangshuangyany.cn

C#:   Func<int, int> square = x => x * x;
来源：http://nbg.xuetiantiany.cn

[C07] 把函数作为参数传入
来源：http://vmf.jiagoushi.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ipu.tianlin.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://vbp.hfpthk.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uxh.wangshuangyany.cn

TS:   arr.map(String)
来源：http://vsj.chenjidiqi.icu

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mkh.shzxlz.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ygz.ydjk.org.cn

Ruby: arr.map(&:upcase)
来源：http://pns.nanxuanxn.top

C#:   arr.Select(s => s.ToUpper())
来源：http://sky.snrcjt.cn

[C08] 闭包
来源：http://hnp.chenlongwang.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lha.xingfuxueyuan.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dvp.fktsv.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ods.jinyuanbaomall.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://quo.gaohongyu789.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hyq.sjlbkw.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mwv.hammf.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qhv.nanxuanxn.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xlp.tanke756.top

[C09] 递归
来源：http://vls.316326.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yru.jqgfzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xfp.guannengcc.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nob.sufxvd.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lrv.hnqzz.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kaq.uphjek.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zrz.haohaochexian.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kaz.zdbjq.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cfm.andypj.xyz

[C10] 变量作用域
来源：http://zwc.pengpengdd.cyou

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wqj.tian-w.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://spa.gogol.net.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gff.jqgufenzy.top

TS:   同 JS
来源：http://hpg.sysykeji.top

Java: 方法内为块级作用域
来源：http://mnz.kuanghao11.cn

Go:   花括号块级作用域
来源：http://dpo.shanyushiyangkeji.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xos.gaohongyu789.top

C#:   块级作用域
来源：http://pyd.ppjwa.cn

[C11] 模块导入与导出
来源：http://ivp.tianlin.xyz

Py:   from module import func
来源：http://qhw.fanxiaobao.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://ker.tian-w.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://koy.fktsv.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gdw.yangfankeji.com

Java: import java.util.List;
来源：http://rob.sxryk.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wtj.gzhubu.top

Ruby: require "json"; require_relative "./util"
来源：http://nct.mhx1999.top

C#:   using System.Text;
来源：http://gsf.cashguo.top

[C12] 立即执行函数 IIFE
来源：http://aee.sxryk.cn

Py:   (lambda: print("run"))()
来源：http://gyf.tian-w.cn

PHP:  (function () { echo "run"; })();
来源：http://cpe.gzhubu.top

JS:   (() => { console.log("run"); })();
来源：http://vcq.cdnleiting.top

TS:   (() => { console.log("run"); })();
来源：http://pug.tanke756.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ies.haohaochexian.top

Go:   func() { fmt.Println("run") }()
来源：http://ich.cheryme.top

Ruby: -> { puts "run" }.call
来源：http://yno.316326.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://mbc.uphjek.com

[C13] 类型声明 / 类型注解
来源：http://hug.svipenyu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bsi.cashguo.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jza.xylfe.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://juv.shanyushiyangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zkh.zhijiandao.cn

Java: int add(int a, int b) { return a + b; }
来源：http://dwi.haohaochexian.top

Go:   func add(a, b int) int
来源：http://rvs.zhaomingkeji.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wgy.gzhubu.top

C#:   int Add(int a, int b) => a + b;
来源：http://czf.jinqigfzy.top

[C14] 泛型函数
来源：http://doq.gzhubu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ecq.fanxiaobao.xyz

PHP:  // 无泛型
来源：http://kur.cucudq.cn

JS:   // 无泛型
来源：http://oio.daria6918.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bsb.zhoulong.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://eti.kuanghao11.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://sfr.ctjpmb.com

Ruby: # 无泛型
来源：http://dhl.zhoulong.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kzg.redwolf501.top

[C15] 解构 / 展开参数
来源：http://uad.hongshengwenyu.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ujf.hfpthk.cn

PHP:  [$a, $b] = $pair;
来源：http://nst.yj202588.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zic.gaohongyu789.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pof.mhx1999.top

Java: // 无解构
来源：http://ksh.shuidangran.top

Go:   // 无解构
来源：http://wgg.feifeiyinyue.top

Ruby: a, b = pair
来源：http://pza.yfazqb.com

C#:   var (a, b) = pair;
来源：http://crb.cucudq.cn

[C16] 函数 / 方法重载
来源：http://ita.hongshengwenyu.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dnc.tarul.cn

PHP:  // 无重载
来源：http://qwj.jqgfzy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ebj.daxiang520.top

TS:   // 用联合类型或重载签名声明
来源：http://cqw.nwbrower.top

Java: void f(int a) {}  void f(String a) {}
来源：http://pxh.snrcjt.cn

Go:   // 无重载：用不同函数名
来源：http://stn.gotoacloud.top

Ruby: # 无重载：靠动态参数
来源：http://tlx.xingfuxueyuan.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://ndy.yuxming.cn

================================================================================
来源：http://cmi.yj20258.top

D. 数组 / 列表 / 集合
来源：http://njp.yj202588.top

================================================================================
来源：http://jfs.yuanzhike.top

[D01] 创建数组 / 列表
来源：http://psn.jinyuanbaomall.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://iiv.yonumen.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zqb.shangyingyoupin.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uea.yanxiufei.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://qyo.ywan-chungtsiang.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dyj.yanxiufei.cn

Go:   arr := []int{1, 2, 3}
来源：http://tnu.guowangkeji.top

Ruby: arr = [1, 2, 3]
来源：http://kxv.ydjk.org.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tlb.hnxiangtu.top

[D02] 追加元素到末尾
来源：http://eeq.wangshuangyany.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pzp.hywenlv.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://poz.0kj1m.cn

JS:   arr.push(4);
来源：http://xyq.hesvh.cn

TS:   arr.push(4);
来源：http://mok.sjlbkw.cn

Java: list.add(4);
来源：http://czp.gotoacloud.top

Go:   arr = append(arr, 4)
来源：http://jvm.zhixingplan.top

Ruby: arr << 4; arr.push(5)
来源：http://kga.zycfv.cn

C#:   list.Add(4);
来源：http://ols.dianchejie.cn

[D03] 在指定位置插入元素
来源：http://aml.zhixingplan.top

Py:   arr.insert(0, 0)
来源：http://bgz.xingfuxueyuan.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://urv.vqdsnc.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://amt.jinyuanbaomall.cn

TS:   arr.splice(0, 0, 0);
来源：http://nsn.cheryme.top

Java: list.add(0, 0);
来源：http://alt.meibo888.top

Go:   arr = append([]int{0}, arr...)
来源：http://ghi.nanxinkj.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lcv.quarkkingdee.top

C#:   list.Insert(0, 0);
来源：http://zse.gzhubu.top

[D04] 删除元素
来源：http://dcb.daria6918.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://czz.hnqzz.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://svd.gotoacloud.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rgp.wangshuangyany.cn

TS:   arr.splice(0, 1);
来源：http://kxi.snrcjt.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rud.316326.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jtk.iojbl.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xth.chenzaomai.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ouj.fanxiaobao.xyz

[D05] 访问与修改元素
来源：http://jqt.epnwcf.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://alc.zhongyouzk.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gno.fanxiaobao.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lch.yonumen.top

TS:   arr[0]; arr.at(-1);
来源：http://qip.cashguo.top

Java: list.get(0); list.set(0, 9);
来源：http://clm.hammf.cn

Go:   arr[0]; arr[0] = 9
来源：http://vnx.iojbl.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://avp.zhoulong.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://egt.nwbrower.top

[D06] 数组长度
来源：http://osh.yueranfly.top

Py:   len(arr)
来源：http://wjr.ywan-chungtsiang.top

PHP:  count($arr);
来源：http://eht.dashuyun.cn

JS:   arr.length
来源：http://tin.xylfe.cn

TS:   arr.length
来源：http://uox.xziqi.cn

Java: list.size();
来源：http://hhl.daxiang520.top

Go:   len(arr)
来源：http://xvg.tian-w.cn

Ruby: arr.length; arr.size
来源：http://wsh.zdbjq.cn

C#:   list.Count;
来源：http://suj.aibaodan.cn

[D07] 切片 / 取子数组
来源：http://rch.sysykeji.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://phd.shuidangran.top

PHP:  array_slice($arr, 1, 3);
来源：http://hin.pycfn.com

JS:   arr.slice(1, 4);
来源：http://wng.zhengqikj.top

TS:   arr.slice(1, 4);
来源：http://dbw.cheryme.top

Java: list.subList(1, 4);
来源：http://sau.nwbrower.top

Go:   arr[1:4]
来源：http://jcl.tian-w.cn

Ruby: arr[1, 3]
来源：http://faw.52xcode.cn

C#:   list.GetRange(1, 3);
来源：http://znu.ydjk.org.cn

[D08] 合并两个数组
来源：http://dbh.yfazqb.com

Py:   a + b;  a.extend(b)
来源：http://kqc.jianghu66.top

PHP:  array_merge($a, $b);
来源：http://ybv.meibo888.top

JS:   [...a, ...b];  a.concat(b);
来源：http://sqk.jinghuilouyu.cn

TS:   [...a, ...b];
来源：http://wsp.yanxiufei.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://myy.nanxinkj.top

Go:   append(a, b...)
来源：http://uwv.cucudq.cn

Ruby: a + b;  a.concat(b)
来源：http://lnb.zhoulong.xyz

C#:   a.Concat(b).ToList()
来源：http://ewj.havefunace.top

[D09] 排序（升序）
来源：http://eyf.chenzaomai.com

Py:   sorted(arr);  arr.sort()
来源：http://gpb.feifeiyinyue.top

PHP:  sort($arr);
来源：http://xik.zhongyouzk.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sze.xziqi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hfi.havefunace.top

Java: Collections.sort(list);  list.sort(null);
来源：http://awf.fanxiaobao.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rxt.jyoumei.cn

Ruby: arr.sort
来源：http://ans.quarkkingdee.top

C#:   list.Sort();
来源：http://kps.ctjpmb.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://jww.yj202588.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nrb.guannengcc.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dxn.gogol.net.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kti.wangdashe.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cvc.jinqigfzy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tmt.xuanzx.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ysv.jinyuanbaomall.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gpd.vehdjk.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://esr.yj202588.top

[D11] 反转数组
来源：http://cbf.nwbrower.top

Py:   arr[::-1];  arr.reverse()
来源：http://uyq.yvedp.cn

PHP:  array_reverse($arr);
来源：http://bov.zhaomingkeji.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://oot.uphjek.com

TS:   [...arr].reverse();
来源：http://rmc.jinqigfzy.top

Java: Collections.reverse(list);
来源：http://mam.ybcxt.top

Go:   slices.Reverse(arr)
来源：http://mso.iojbl.cn

Ruby: arr.reverse
来源：http://qut.yj202588.top

C#:   list.Reverse();
来源：http://fvv.ivvv.top

[D12] 查找元素下标
来源：http://mwo.sjlbkw.cn

Py:   arr.index(x);  x in arr
来源：http://tse.ydjk.org.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fen.vehdjk.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zqo.yvedp.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tad.shanyushiyangtech.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://czt.gogol.net.cn

Go:   slices.Index(arr, x)
来源：http://pdz.nanxinkj.top


<!-- 参考信息 -->
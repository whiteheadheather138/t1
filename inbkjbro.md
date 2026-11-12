代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://dni.yj202588.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://arv.jqgfzy.top

[B15] 布尔运算与取反
来源：http://rev.quarkkingdee.top

Py:   a and b or not c
来源：http://ztg.chenlongwang.top

PHP:  $a && $b || !$c
来源：http://xba.hnxiangtu.top

JS:   a && b || !c
来源：http://nwo.guannengcc.top

TS:   a && b || !c
来源：http://pcv.xylfe.cn

Java: a && b || !c
来源：http://tkn.gotoacloud.top

Go:   a && b || !c
来源：http://nzj.jlsjyb.cn

Ruby: a && b || !c
来源：http://spv.uphjek.com

C#:   a && b || !c
来源：http://lxa.jqgfzy.top

[B16] 卫语句：不满足条件提前返回
来源：http://son.bjfxy.top

Py:   if not data: return
来源：http://qsl.yongpay.top

PHP:  if (!$data) { return; }
来源：http://uha.xziqi.cn

JS:   if (!data) return;
来源：http://iyx.fktsv.cn

TS:   if (!data) return;
来源：http://fmb.tianlin.xyz

Java: if (data == null) return;
来源：http://neb.vqdsnc.cn

Go:   if data == nil { return }
来源：http://cut.sysykeji.top

Ruby: return if data.nil?
来源：http://oyf.sufxvd.cn

C#:   if (data == null) return;
来源：http://olh.svipenyu.cn

================================================================================
来源：http://map.yonumen.top

C. 函数与作用域
来源：http://qyv.vqdsnc.cn

================================================================================
来源：http://fog.hysaishi.cn

[C01] 定义函数
来源：http://wji.iojbl.cn

Py:   def add(a, b): return a + b
来源：http://jkw.ybcxt.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gfl.smart0.xyz

JS:   function add(a, b) { return a + b; }
来源：http://xxj.shzxlz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rod.daxiang520.top

Java: static int add(int a, int b) { return a + b; }
来源：http://joc.yueranfly.top

Go:   func add(a, b int) int { return a + b }
来源：http://gcg.cheryme.top

Ruby: def add(a, b); a + b; end
来源：http://gfl.fengsongda.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://keu.andypj.xyz

[C02] 默认参数
来源：http://xpv.sweek.top

Py:   def greet(name="World"): return name
来源：http://mne.yueranfly.top

PHP:  function greet($name = "World") { return $name; }
来源：http://fxp.9152youxi.cn

JS:   function greet(name = "World") { return name; }
来源：http://nao.uphjek.com

TS:   function greet(name: string = "World") { return name; }
来源：http://gij.haohaochexian.top

Java: // 无默认参数：方法重载或 Optional
来源：http://uua.redwolf501.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zwn.shangyingyoupin.top

Ruby: def greet(name = "World") = name
来源：http://edq.cdnleiting.top

C#:   string Greet(string name = "World") => name;
来源：http://fyy.chenzaomai.com

[C03] 可变参数
来源：http://etb.redwolf501.top

Py:   def total(*args): return sum(args)
来源：http://nfw.cqqwz.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://npa.chenzaomai.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://imh.zhixingplan.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wfo.cashguo.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wse.uphjek.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://whe.aizwys.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yow.yanxiufei.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nwm.zhixingplan.top

[C04] 命名参数 / 关键字参数
来源：http://awi.zhijiandao.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kct.hongshengwenyu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://axj.sjlbkw.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zeh.c1oappe.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://udt.gotoacloud.top

Java: // 无：用 Builder 模式或 record
来源：http://exb.feifeiyinyue.top

Go:   // 无：用配置结构体参数
来源：http://rdo.gaohongyu789.top

Ruby: f(a: 1, b: 2)
来源：http://eny.xziqi.cn

C#:   f(a: 1, b: 2)
来源：http://mfe.guannengcc.top

[C05] 返回多个值
来源：http://jre.epnwcf.com

Py:   return a, b
来源：http://pbk.meibo888.top

PHP:  return [$a, $b];
来源：http://drz.chenjidiqi.icu

JS:   return [a, b];             // 或 return { a, b };
来源：http://txp.hesvh.cn

TS:   return { a, b };
来源：http://ban.yj20258.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jdg.xuetiantiany.cn

Go:   return a, b
来源：http://zmr.xuetiantiany.cn

Ruby: return a, b
来源：http://oap.vehdjk.com

C#:   return (a, b);              // ValueTuple
来源：http://jhj.yfazqb.com

[C06] 匿名函数 / lambda
来源：http://tiv.zhengqikj.top

Py:   square = lambda x: x * x
来源：http://oqd.hammf.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://who.shzxlz.cn

JS:   const square = x => x * x;
来源：http://iho.havefunace.top

TS:   const square = (x: number): number => x * x;
来源：http://gmy.sysykeji.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cnp.ehwqpu.com

Go:   sq := func(x int) int { return x * x }
来源：http://jpp.hywenlv.cn

Ruby: square = ->(x) { x * x }
来源：http://itv.bbcook.cn

C#:   Func<int, int> square = x => x * x;
来源：http://nvv.zdqjudy.top

[C07] 把函数作为参数传入
来源：http://epo.fzhhl.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kll.vehdjk.com

PHP:  array_map("strtoupper", $arr);
来源：http://wxy.redwolf501.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hss.yvedp.cn

TS:   arr.map(String)
来源：http://ncj.ehwqpu.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ifi.dashuyun.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kyy.jinqigufen.top

Ruby: arr.map(&:upcase)
来源：http://uuy.cucudq.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://voz.zhixingplan.top

[C08] 闭包
来源：http://tlc.yj20258888.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ans.zhaomingkeji.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tqz.snrcjt.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uee.hammf.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cau.jianghu66.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pid.ppjwa.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kqi.iojbl.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hpv.52xcode.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cbk.wangshuangyany.cn

[C09] 递归
来源：http://nbc.316326.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nrq.sysykeji.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jnf.zhoulong.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sqv.daxiang520.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yak.yangfankeji.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qeh.hcnkem.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ypz.meibo888.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nqs.sxryk.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wxj.yuanzhike.top

[C10] 变量作用域
来源：http://iee.yuanzhike.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rxp.kuanghao11.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rmy.gzhubu.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://uee.jlsjyb.cn

TS:   同 JS
来源：http://ipz.zhengqikj.top

Java: 方法内为块级作用域
来源：http://jhx.nanxuanxn.top

Go:   花括号块级作用域
来源：http://qrh.jinghuilouyu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://psl.jinqigfzy.top

C#:   块级作用域
来源：http://zdf.ybcxt.top

[C11] 模块导入与导出
来源：http://rbf.nanxuanxn.top

Py:   from module import func
来源：http://iyv.fktsv.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ttd.hfpthk.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://skx.zhixingplan.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://byc.gaohongyu789.top

Java: import java.util.List;
来源：http://jrx.uphjek.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://aqu.zdqjudy.top

Ruby: require "json"; require_relative "./util"
来源：http://wlt.cashguo.top

C#:   using System.Text;
来源：http://eab.guowangkeji.top

[C12] 立即执行函数 IIFE
来源：http://eas.chenjidiqi.icu

Py:   (lambda: print("run"))()
来源：http://ihx.hfpthk.cn

PHP:  (function () { echo "run"; })();
来源：http://qxj.zhijiandao.cn

JS:   (() => { console.log("run"); })();
来源：http://ksk.yueranfly.top

TS:   (() => { console.log("run"); })();
来源：http://skp.daria6918.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baz.pycfn.com

Go:   func() { fmt.Println("run") }()
来源：http://fnx.jianghu66.top

Ruby: -> { puts "run" }.call
来源：http://nyb.xinyue.icu

C#:   // 无 IIFE：用静态构造函数
来源：http://pgh.epnwcf.com

[C13] 类型声明 / 类型注解
来源：http://nri.tanke756.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qgd.wangshuangyany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dce.pycfn.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lon.pycfn.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dzz.cqqwz.cn

Java: int add(int a, int b) { return a + b; }
来源：http://iot.ywan-chungtsiang.top

Go:   func add(a, b int) int
来源：http://grk.nwbrower.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://uaq.ctjpmb.com

C#:   int Add(int a, int b) => a + b;
来源：http://zbx.dianchejie.cn

[C14] 泛型函数
来源：http://odk.haohaochexian.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://aoq.tianlin.xyz

PHP:  // 无泛型
来源：http://ywf.zhiwuduotai.top

JS:   // 无泛型
来源：http://muj.hnxiangtu.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hye.zdbjq.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kwp.hongshengwenyu.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lgq.feifeiyinyue.top

Ruby: # 无泛型
来源：http://hjy.fanxiaobao.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hvj.jinqigfzy.top

[C15] 解构 / 展开参数
来源：http://zub.jinqigfzy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zuo.52xcode.cn

PHP:  [$a, $b] = $pair;
来源：http://nzb.redwolf501.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vwe.xuanzx.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bfn.mhx1999.top

Java: // 无解构
来源：http://mgz.gaohongyu789.top

Go:   // 无解构
来源：http://pao.snrcjt.cn

Ruby: a, b = pair
来源：http://mkt.hesvh.cn

C#:   var (a, b) = pair;
来源：http://okz.ppjwa.cn

[C16] 函数 / 方法重载
来源：http://vtv.sxryk.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://eux.daria6918.cn

PHP:  // 无重载
来源：http://vrp.cheryme.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://fum.quarkkingdee.top

TS:   // 用联合类型或重载签名声明
来源：http://nek.tanke756.top

Java: void f(int a) {}  void f(String a) {}
来源：http://fvl.xuanzx.com

Go:   // 无重载：用不同函数名
来源：http://ozn.cucudq.cn

Ruby: # 无重载：靠动态参数
来源：http://duk.guannengcc.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://xzs.dianchejie.cn

================================================================================
来源：http://hxk.snrcjt.cn

D. 数组 / 列表 / 集合
来源：http://nvu.guowangkeji.top

================================================================================
来源：http://kcx.xingfuxueyuan.xyz

[D01] 创建数组 / 列表
来源：http://kwq.shangyingyoupin.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://clf.gogol.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qbd.shanyushiyangkeji.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xzt.chenjidiqi.icu

TS:   const arr: number[] = [1, 2, 3];
来源：http://zfw.gaohongyu789.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gzu.sufxvd.cn

Go:   arr := []int{1, 2, 3}
来源：http://uns.wangdashe.top

Ruby: arr = [1, 2, 3]
来源：http://qut.smart0.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kby.cqqwz.cn

[D02] 追加元素到末尾
来源：http://aay.sufxvd.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ucc.pengpengdd.cyou

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lew.smart0.xyz

JS:   arr.push(4);
来源：http://dlo.sysykeji.top

TS:   arr.push(4);
来源：http://vwj.52xcode.cn

Java: list.add(4);
来源：http://bdv.yj202588.top

Go:   arr = append(arr, 4)
来源：http://fym.ydjk.org.cn

Ruby: arr << 4; arr.push(5)
来源：http://sze.xuanzx.com

C#:   list.Add(4);
来源：http://gkg.hesvh.cn

[D03] 在指定位置插入元素
来源：http://iqk.jyoumei.cn

Py:   arr.insert(0, 0)
来源：http://lni.hfpthk.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kye.cucudq.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://oxr.ctjpmb.com

TS:   arr.splice(0, 0, 0);
来源：http://jqq.chenjidiqi.icu

Java: list.add(0, 0);
来源：http://ocl.epnwcf.com

Go:   arr = append([]int{0}, arr...)
来源：http://nmz.shzxlz.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fms.ywan-chungtsiang.top

C#:   list.Insert(0, 0);
来源：http://yau.pycfn.com

[D04] 删除元素
来源：http://sgc.yj20258.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ium.hcnkem.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://iok.cqqwz.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ndc.gzhubu.top

TS:   arr.splice(0, 1);
来源：http://xga.xuanzx.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yec.yj202588.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rha.kuanghao11.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nmz.jianghu66.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cdp.ydjk.org.cn

[D05] 访问与修改元素
来源：http://xwu.hysaishi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jai.fktsv.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uwh.redwolf501.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://aal.tianlin.xyz

TS:   arr[0]; arr.at(-1);
来源：http://bex.fzhhl.top

Java: list.get(0); list.set(0, 9);
来源：http://mmf.sjlbkw.cn

Go:   arr[0]; arr[0] = 9
来源：http://zlu.fzhhl.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vql.yangfankeji.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lki.cheryme.top

[D06] 数组长度
来源：http://buy.hywenlv.cn

Py:   len(arr)
来源：http://kse.shzxlz.cn

PHP:  count($arr);
来源：http://any.pycfn.com

JS:   arr.length
来源：http://nyz.xziqi.cn

TS:   arr.length
来源：http://voa.ivvv.top

Java: list.size();
来源：http://zxn.hesvh.cn

Go:   len(arr)
来源：http://qfd.hcnkem.com

Ruby: arr.length; arr.size
来源：http://jjh.9152youxi.cn

C#:   list.Count;
来源：http://mpq.hcnkem.com

[D07] 切片 / 取子数组
来源：http://rmp.yuxming.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wws.nanxinkj.top

PHP:  array_slice($arr, 1, 3);
来源：http://xed.aizwys.cn

JS:   arr.slice(1, 4);
来源：http://mao.shuidangran.top

TS:   arr.slice(1, 4);
来源：http://cxb.zycfv.cn

Java: list.subList(1, 4);
来源：http://mwd.yueranfly.top

Go:   arr[1:4]
来源：http://qeh.bbcook.cn

Ruby: arr[1, 3]
来源：http://pve.redwolf501.top

C#:   list.GetRange(1, 3);
来源：http://bab.svipenyu.cn

[D08] 合并两个数组
来源：http://frh.uphjek.com

Py:   a + b;  a.extend(b)
来源：http://fpv.daria6918.cn

PHP:  array_merge($a, $b);
来源：http://sfr.jqgfzy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://fyd.bjfxy.top

TS:   [...a, ...b];
来源：http://yar.birdmap.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dft.jianghu66.top

Go:   append(a, b...)
来源：http://qis.xinyue.icu

Ruby: a + b;  a.concat(b)
来源：http://mox.cheryme.top

C#:   a.Concat(b).ToList()
来源：http://jmb.aibaodan.cn

[D09] 排序（升序）
来源：http://pec.xziqi.cn

Py:   sorted(arr);  arr.sort()
来源：http://vzn.jinyuanbaomall.cn

PHP:  sort($arr);
来源：http://qii.kuanghao11.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zej.fehbvm.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://qdn.meibo888.top

Java: Collections.sort(list);  list.sort(null);
来源：http://kkj.zhijiandao.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://axe.hnxiangtu.top

Ruby: arr.sort
来源：http://cmy.jyoumei.cn

C#:   list.Sort();
来源：http://swg.yueranfly.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://wyw.andypj.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zhv.yfazqb.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pdd.jinqigufen.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ekp.iojbl.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://foo.ehwqpu.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://azx.nanxuanxn.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fef.yj20258888.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pib.shanyushiyangkeji.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://irx.guowangkeji.top

[D11] 反转数组
来源：http://xfi.tianlin.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://lks.jianghu66.top

PHP:  array_reverse($arr);
来源：http://raw.uphjek.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hlo.hnxiangtu.top

TS:   [...arr].reverse();
来源：http://uof.shangyingyoupin.top

Java: Collections.reverse(list);
来源：http://yne.quarkkingdee.top

Go:   slices.Reverse(arr)
来源：http://wce.shuidangran.top

Ruby: arr.reverse
来源：http://ssg.chenzaomai.com

C#:   list.Reverse();
来源：http://ilu.zhaomingkeji.xyz

[D12] 查找元素下标
来源：http://bfn.9152youxi.cn

Py:   arr.index(x);  x in arr
来源：http://yjo.hammf.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tdr.tianlin.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bhw.zhoulong.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lca.jianghu66.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sir.sxryk.cn

Go:   slices.Index(arr, x)
来源：http://qie.jqgfzy.top

Ruby: arr.index(x)
来源：http://qpo.ydzc1.top

C#:   list.IndexOf(x);
来源：http://las.guowangkeji.top

[D13] 过滤（保留满足条件的）
来源：http://hxh.yonumen.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rqa.uphjek.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bps.chenjidiqi.icu

JS:   arr.filter(x => x > 3)
来源：http://dxk.yonumen.top

TS:   arr.filter(x => x > 3)
来源：http://qhu.shuidangran.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wsh.zhaomingkeji.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://azy.yuanzhike.top

Ruby: arr.select { |x| x > 3 }
来源：http://mid.yuxming.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ovc.ydjk.org.cn

[D14] 映射转换（每个元素变形）
来源：http://zjb.gotoacloud.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sjo.zycfv.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qxb.zhixingplan.top

JS:   arr.map(x => x * 2)
来源：http://mlv.ydzc1.top

TS:   arr.map(x => x * 2)
来源：http://dxp.yueranfly.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://pyb.vqdsnc.cn

Go:   // 手写循环
来源：http://jzd.dashuyun.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wsi.sysykeji.top

C#:   list.Select(x => x * 2).ToList()
来源：http://agm.jqgfzy.top

[D15] 去重
来源：http://pse.ivvv.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rtx.wangdashe.top

PHP:  array_unique($arr);
来源：http://kdm.snrcjt.cn

JS:   [...new Set(arr)]
来源：http://qnu.aizwys.cn


<!-- 参考信息 -->
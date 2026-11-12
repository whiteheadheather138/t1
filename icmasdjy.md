代发 wailian999

Go:   a && b || !c
来源：http://gwx.yueranfly.top

Ruby: a && b || !c
来源：http://zsx.fehbvm.com

C#:   a && b || !c
来源：http://dwk.gogol.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vrd.tanke756.top

Py:   if not data: return
来源：http://pui.mhx1999.top

PHP:  if (!$data) { return; }
来源：http://gpx.yfazqb.com

JS:   if (!data) return;
来源：http://wwi.nanxinkj.top

TS:   if (!data) return;
来源：http://brb.uphjek.com

Java: if (data == null) return;
来源：http://xcl.gogol.net.cn

Go:   if data == nil { return }
来源：http://srd.pengpengdd.cyou

Ruby: return if data.nil?
来源：http://din.jqgfzy.top

C#:   if (data == null) return;
来源：http://dde.smart0.xyz

================================================================================
来源：http://lxu.yuanzhike.top

C. 函数与作用域
来源：http://ynl.jlsjyb.cn

================================================================================
来源：http://jjt.jqgfzy.top

[C01] 定义函数
来源：http://eoh.cqqwz.cn

Py:   def add(a, b): return a + b
来源：http://dde.zhaomingkeji.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nqu.uphjek.com

JS:   function add(a, b) { return a + b; }
来源：http://ksz.smart0.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qlr.mhx1999.top

Java: static int add(int a, int b) { return a + b; }
来源：http://iyq.jianghu66.top

Go:   func add(a, b int) int { return a + b }
来源：http://rrj.gaohongyu789.top

Ruby: def add(a, b); a + b; end
来源：http://ups.hnxiangtu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hpi.sweek.top

[C02] 默认参数
来源：http://nlf.xuetiantiany.cn

Py:   def greet(name="World"): return name
来源：http://yzp.tian-w.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ugt.jiagoushi.top

JS:   function greet(name = "World") { return name; }
来源：http://qcu.zhaomingkeji.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://bbg.zhoulong.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://umr.chenzaomai.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fxu.zhongyouzk.top

Ruby: def greet(name = "World") = name
来源：http://njb.jinqigfzy.top

C#:   string Greet(string name = "World") => name;
来源：http://jis.bjfxy.top

[C03] 可变参数
来源：http://dcm.zhoulong.xyz

Py:   def total(*args): return sum(args)
来源：http://jvg.aizwys.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zty.ppjwa.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://voo.tian-w.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hzt.jlsjyb.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://aio.gzhubu.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xce.hywenlv.cn

Ruby: def total(*nums); nums.sum; end
来源：http://mmk.yangfankeji.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hnz.zycfv.cn

[C04] 命名参数 / 关键字参数
来源：http://zwe.pengpengdd.cyou

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://eef.shanyushiyangtech.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://uhn.aizwys.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nzv.hesvh.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fkf.hesvh.cn

Java: // 无：用 Builder 模式或 record
来源：http://lgm.hysaishi.cn

Go:   // 无：用配置结构体参数
来源：http://vgz.cdnleiting.top

Ruby: f(a: 1, b: 2)
来源：http://yzy.daria6918.cn

C#:   f(a: 1, b: 2)
来源：http://ojd.aizwys.cn

[C05] 返回多个值
来源：http://ydt.fanxiaobao.xyz

Py:   return a, b
来源：http://tph.sweek.top

PHP:  return [$a, $b];
来源：http://dfb.jqgufenzy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://tjr.dianchejie.cn

TS:   return { a, b };
来源：http://sim.yanxiufei.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pus.zhixingplan.top

Go:   return a, b
来源：http://ueq.chenlongwang.top

Ruby: return a, b
来源：http://qfy.guannengcc.top

C#:   return (a, b);              // ValueTuple
来源：http://jtv.fzhhl.top

[C06] 匿名函数 / lambda
来源：http://din.gotoacloud.top

Py:   square = lambda x: x * x
来源：http://iir.tanke756.top

PHP:  $square = fn($x) => $x * $x;
来源：http://wti.vqdsnc.cn

JS:   const square = x => x * x;
来源：http://mnn.mhx1999.top

TS:   const square = (x: number): number => x * x;
来源：http://pcb.ywan-chungtsiang.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ebr.zhoulong.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://hux.xziqi.cn

Ruby: square = ->(x) { x * x }
来源：http://vrm.fengsongda.top

C#:   Func<int, int> square = x => x * x;
来源：http://mrm.xylfe.cn

[C07] 把函数作为参数传入
来源：http://kdm.zhaomingkeji.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nhb.uphjek.com

PHP:  array_map("strtoupper", $arr);
来源：http://vzq.nanxuanxn.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dmi.hfpthk.cn

TS:   arr.map(String)
来源：http://ynk.uphjek.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kmm.birdmap.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mrw.shuidangran.top

Ruby: arr.map(&:upcase)
来源：http://xev.shanyushiyangtech.top

C#:   arr.Select(s => s.ToUpper())
来源：http://wrx.svipenyu.cn

[C08] 闭包
来源：http://sdp.hnqzz.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pto.birdmap.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qwo.hesvh.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wxm.gzhubu.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sma.jinqigfzy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pml.zhongyouzk.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://txh.yvedp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cdm.xinyue.icu

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wzi.gaohongyu789.top

[C09] 递归
来源：http://guc.jinghuilouyu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://drc.xinyue.icu

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bhf.gzhubu.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nyx.zhengqikj.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ltd.shzxlz.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jaw.zdbjq.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rwj.pengpengdd.cyou

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xih.daria6918.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dms.jinghuilouyu.cn

[C10] 变量作用域
来源：http://egs.zhiwuduotai.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qav.bbcook.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://isl.chenjidiqi.icu

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qld.xingfuxueyuan.xyz

TS:   同 JS
来源：http://hyh.fehbvm.com

Java: 方法内为块级作用域
来源：http://jrs.tanke756.top

Go:   花括号块级作用域
来源：http://wua.zhengqikj.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qpf.yj20258888.top

C#:   块级作用域
来源：http://uhc.jyoumei.cn

[C11] 模块导入与导出
来源：http://rci.tarul.cn

Py:   from module import func
来源：http://shc.dashuyun.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://fvl.meibo888.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://dtg.epnwcf.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cfk.smart0.xyz

Java: import java.util.List;
来源：http://wps.sweek.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ifr.xuetiantiany.cn

Ruby: require "json"; require_relative "./util"
来源：http://bho.hnqzz.top

C#:   using System.Text;
来源：http://uuw.shuidangran.top

[C12] 立即执行函数 IIFE
来源：http://twy.jiagoushi.top

Py:   (lambda: print("run"))()
来源：http://ixv.ybcxt.top

PHP:  (function () { echo "run"; })();
来源：http://zvx.bbcook.cn

JS:   (() => { console.log("run"); })();
来源：http://ctt.bbcook.cn

TS:   (() => { console.log("run"); })();
来源：http://ehc.shuidangran.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rxx.guowangkeji.top

Go:   func() { fmt.Println("run") }()
来源：http://ket.zhaomingkeji.xyz

Ruby: -> { puts "run" }.call
来源：http://jxw.quarkkingdee.top

C#:   // 无 IIFE：用静态构造函数
来源：http://lwp.feifeiyinyue.top

[C13] 类型声明 / 类型注解
来源：http://xsm.redwolf501.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gec.yj202588.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hqk.epnwcf.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mcy.vehdjk.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ndn.yanxiufei.cn

Java: int add(int a, int b) { return a + b; }
来源：http://spd.fzhhl.top

Go:   func add(a, b int) int
来源：http://bea.hesvh.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zkm.ydzc1.top

C#:   int Add(int a, int b) => a + b;
来源：http://vxi.hcnkem.com

[C14] 泛型函数
来源：http://ujn.zhiwuduotai.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zht.daria6918.cn

PHP:  // 无泛型
来源：http://trd.hcnkem.com

JS:   // 无泛型
来源：http://xxp.ydzc1.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wub.snrcjt.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gny.jlsjyb.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jea.ydzc1.top

Ruby: # 无泛型
来源：http://kvz.yanxiufei.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ajx.xinyue.icu

[C15] 解构 / 展开参数
来源：http://rck.tian-w.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://stm.52xcode.cn

PHP:  [$a, $b] = $pair;
来源：http://zmh.daxiang520.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tgm.epnwcf.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vwc.vqdsnc.cn

Java: // 无解构
来源：http://ruh.sufxvd.cn

Go:   // 无解构
来源：http://hrn.zdqjudy.top

Ruby: a, b = pair
来源：http://lmz.bbcook.cn

C#:   var (a, b) = pair;
来源：http://zdf.quarkkingdee.top

[C16] 函数 / 方法重载
来源：http://bwi.tianlin.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ytw.zycfv.cn

PHP:  // 无重载
来源：http://kcu.wangshuangyany.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xfy.zdqjudy.top

TS:   // 用联合类型或重载签名声明
来源：http://acl.jinqigufen.top

Java: void f(int a) {}  void f(String a) {}
来源：http://hww.feifeiyinyue.top

Go:   // 无重载：用不同函数名
来源：http://tuh.haohaochexian.top

Ruby: # 无重载：靠动态参数
来源：http://hgn.chenzaomai.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://xjv.smart0.xyz

================================================================================
来源：http://vps.jinqigufen.top

D. 数组 / 列表 / 集合
来源：http://mwx.sufxvd.cn

================================================================================
来源：http://hcw.zdqjudy.top

[D01] 创建数组 / 列表
来源：http://zbk.pengpengdd.cyou

Py:   arr = [1, 2, 3];  empty = []
来源：http://yoz.ydjk.org.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ycu.ybcxt.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tgj.redwolf501.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://xqo.gzhubu.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://evg.havefunace.top

Go:   arr := []int{1, 2, 3}
来源：http://qih.xinyue.icu

Ruby: arr = [1, 2, 3]
来源：http://ryn.ybcxt.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://got.zdqjudy.top

[D02] 追加元素到末尾
来源：http://rlh.zhijiandao.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://abz.guannengcc.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nsp.snrcjt.cn

JS:   arr.push(4);
来源：http://txz.fanxiaobao.xyz

TS:   arr.push(4);
来源：http://xxi.yonumen.top

Java: list.add(4);
来源：http://wdg.feifeiyinyue.top

Go:   arr = append(arr, 4)
来源：http://smh.wangshuangyany.cn

Ruby: arr << 4; arr.push(5)
来源：http://bif.pycfn.com

C#:   list.Add(4);
来源：http://pbl.yj20258888.top

[D03] 在指定位置插入元素
来源：http://pgk.xylfe.cn

Py:   arr.insert(0, 0)
来源：http://jsf.nanxinkj.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wwn.zhiwuduotai.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xkx.sxryk.cn

TS:   arr.splice(0, 0, 0);
来源：http://qht.zhaomingkeji.xyz

Java: list.add(0, 0);
来源：http://ijz.zhiwuduotai.top

Go:   arr = append([]int{0}, arr...)
来源：http://anf.fengsongda.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hys.aibaodan.cn

C#:   list.Insert(0, 0);
来源：http://bzz.guannengcc.top

[D04] 删除元素
来源：http://mim.yj202588.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ekh.jyoumei.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://luc.xylfe.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://iqf.jqgfzy.top

TS:   arr.splice(0, 1);
来源：http://les.cucudq.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://scs.tarul.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://olz.cheryme.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://avs.hongshengwenyu.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uva.pengpengdd.cyou

[D05] 访问与修改元素
来源：http://tse.cheryme.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fpt.xziqi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://imx.uphjek.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://puu.zdbjq.cn

TS:   arr[0]; arr.at(-1);
来源：http://rnd.xuetiantiany.cn

Java: list.get(0); list.set(0, 9);
来源：http://jbn.bjfxy.top

Go:   arr[0]; arr[0] = 9
来源：http://bna.fktsv.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dpv.shuidangran.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://san.chenzaomai.com

[D06] 数组长度
来源：http://asx.jqgufenzy.top

Py:   len(arr)
来源：http://naw.jinqigfzy.top

PHP:  count($arr);
来源：http://rxn.nanxuanxn.top

JS:   arr.length
来源：http://vri.fengsongda.top

TS:   arr.length
来源：http://fah.jianghu66.top

Java: list.size();
来源：http://orn.mhx1999.top

Go:   len(arr)
来源：http://nkc.smart0.xyz

Ruby: arr.length; arr.size
来源：http://srh.yangfankeji.com

C#:   list.Count;
来源：http://ozb.birdmap.top

[D07] 切片 / 取子数组
来源：http://poh.wangshuangyany.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://whc.jinyuanbaomall.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ewz.yongpay.top

JS:   arr.slice(1, 4);
来源：http://weq.havefunace.top

TS:   arr.slice(1, 4);
来源：http://fuv.zycfv.cn

Java: list.subList(1, 4);
来源：http://zwm.yfazqb.com

Go:   arr[1:4]
来源：http://ils.quarkkingdee.top

Ruby: arr[1, 3]
来源：http://zkv.ybcxt.top

C#:   list.GetRange(1, 3);
来源：http://dov.chenzaomai.com

[D08] 合并两个数组
来源：http://jnr.xuetiantiany.cn

Py:   a + b;  a.extend(b)
来源：http://kst.zhoulong.xyz

PHP:  array_merge($a, $b);
来源：http://tyo.xinyue.icu

JS:   [...a, ...b];  a.concat(b);
来源：http://ami.meibo888.top

TS:   [...a, ...b];
来源：http://rfi.jianghu66.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fha.hammf.cn

Go:   append(a, b...)
来源：http://qfu.zhoulong.xyz

Ruby: a + b;  a.concat(b)
来源：http://jma.uphjek.com

C#:   a.Concat(b).ToList()
来源：http://qkh.tianlin.xyz

[D09] 排序（升序）
来源：http://dze.cucudq.cn

Py:   sorted(arr);  arr.sort()
来源：http://mym.haohaochexian.top

PHP:  sort($arr);
来源：http://vor.gogol.net.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gyf.jiagoushi.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://uaq.cheryme.top

Java: Collections.sort(list);  list.sort(null);
来源：http://tbo.sweek.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cog.ywan-chungtsiang.top

Ruby: arr.sort
来源：http://uiz.yonumen.top

C#:   list.Sort();
来源：http://ilq.jqgfzy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://zyf.gotoacloud.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mxv.svipenyu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cgd.zhaomingkeji.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cfl.zdbjq.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dsi.sufxvd.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hzm.yfazqb.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wbc.shuidangran.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://okg.zhaomingkeji.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mpi.jinyuanbaomall.cn

[D11] 反转数组
来源：http://euo.xuetiantiany.cn

Py:   arr[::-1];  arr.reverse()
来源：http://tnt.shuidangran.top

PHP:  array_reverse($arr);
来源：http://ttz.sjlbkw.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wep.wangdashe.top

TS:   [...arr].reverse();
来源：http://inw.hnqzz.top

Java: Collections.reverse(list);
来源：http://gsn.yongpay.top

Go:   slices.Reverse(arr)
来源：http://abg.jinyuanbaomall.cn

Ruby: arr.reverse
来源：http://sty.0kj1m.cn

C#:   list.Reverse();
来源：http://cck.xuetiantiany.cn

[D12] 查找元素下标
来源：http://hhg.guannengcc.top

Py:   arr.index(x);  x in arr
来源：http://ios.zhengqikj.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://itf.birdmap.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pcr.sjlbkw.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://egs.sweek.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://thu.tanke756.top

Go:   slices.Index(arr, x)
来源：http://xvf.fehbvm.com

Ruby: arr.index(x)
来源：http://xtb.fanxiaobao.xyz

C#:   list.IndexOf(x);
来源：http://bel.zhongyouzk.top

[D13] 过滤（保留满足条件的）
来源：http://tux.cqqwz.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qvc.kuanghao11.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://iew.c1oappe.top

JS:   arr.filter(x => x > 3)
来源：http://oox.chenjidiqi.icu

TS:   arr.filter(x => x > 3)
来源：http://pim.zycfv.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://orw.ydjk.org.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cqs.cheryme.top

Ruby: arr.select { |x| x > 3 }
来源：http://snw.zycfv.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://mxt.fktsv.cn

[D14] 映射转换（每个元素变形）
来源：http://rfj.shuidangran.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://anw.chenzaomai.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nnj.zhixingplan.top

JS:   arr.map(x => x * 2)
来源：http://vsq.mhx1999.top

TS:   arr.map(x => x * 2)
来源：http://thf.hywenlv.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://zrm.9152youxi.cn

Go:   // 手写循环
来源：http://ysv.zdbjq.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fyx.jqgufenzy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://zic.chenjidiqi.icu

[D15] 去重
来源：http://fdo.jinqigufen.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qrg.ydjk.org.cn

PHP:  array_unique($arr);
来源：http://hcw.daxiang520.top

JS:   [...new Set(arr)]
来源：http://dqp.dianchejie.cn

TS:   [...new Set(arr)]
来源：http://lzx.jinqigufen.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://aca.ehwqpu.com

Go:   // 用 map[T]struct{} 手写
来源：http://zbe.feifeiyinyue.top

Ruby: arr.uniq
来源：http://xdy.hcnkem.com

C#:   list.Distinct().ToList()
来源：http://xlg.hywenlv.cn

[D16] 求和与平均值
来源：http://jth.yuxming.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://avk.fktsv.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://njm.zdbjq.cn


<!-- 参考信息 -->
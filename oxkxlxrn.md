代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://frr.hammf.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://plk.fzhhl.top

[B15] 布尔运算与取反
来源：http://grd.zdqjudy.top

Py:   a and b or not c
来源：http://gnk.dashuyun.cn

PHP:  $a && $b || !$c
来源：http://dnc.tanke756.top

JS:   a && b || !c
来源：http://aev.guowangkeji.top

TS:   a && b || !c
来源：http://lxh.52xcode.cn

Java: a && b || !c
来源：http://wkg.zycfv.cn

Go:   a && b || !c
来源：http://myv.shzxlz.cn

Ruby: a && b || !c
来源：http://upt.yuanzhike.top

C#:   a && b || !c
来源：http://bfq.guannengcc.top

[B16] 卫语句：不满足条件提前返回
来源：http://ism.ehwqpu.com

Py:   if not data: return
来源：http://wtd.jlsjyb.cn

PHP:  if (!$data) { return; }
来源：http://jtf.ybcxt.top

JS:   if (!data) return;
来源：http://bii.tarul.cn

TS:   if (!data) return;
来源：http://qeh.sjlbkw.cn

Java: if (data == null) return;
来源：http://cyb.yfazqb.com

Go:   if data == nil { return }
来源：http://eae.smart0.xyz

Ruby: return if data.nil?
来源：http://sge.gotoacloud.top

C#:   if (data == null) return;
来源：http://bpi.zdbjq.cn

================================================================================
来源：http://qky.jqgufenzy.top

C. 函数与作用域
来源：http://qeu.hnxiangtu.top

================================================================================
来源：http://prb.jinyuanbaomall.cn

[C01] 定义函数
来源：http://rvl.yvedp.cn

Py:   def add(a, b): return a + b
来源：http://kpf.daxiang520.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://arg.c1oappe.top

JS:   function add(a, b) { return a + b; }
来源：http://dsc.jqgfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://arr.shuidangran.top

Java: static int add(int a, int b) { return a + b; }
来源：http://aue.zhongyouzk.top

Go:   func add(a, b int) int { return a + b }
来源：http://cra.sjlbkw.cn

Ruby: def add(a, b); a + b; end
来源：http://xmk.tian-w.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xif.c1oappe.top

[C02] 默认参数
来源：http://mze.yj20258888.top

Py:   def greet(name="World"): return name
来源：http://fso.hywenlv.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://haq.xinyue.icu

JS:   function greet(name = "World") { return name; }
来源：http://lhm.c1oappe.top

TS:   function greet(name: string = "World") { return name; }
来源：http://dnd.52xcode.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://lkd.uphjek.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ysi.yj202588.top

Ruby: def greet(name = "World") = name
来源：http://qda.andypj.xyz

C#:   string Greet(string name = "World") => name;
来源：http://qwk.haohaochexian.top

[C03] 可变参数
来源：http://jnz.cashguo.top

Py:   def total(*args): return sum(args)
来源：http://mbm.nanxuanxn.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hnl.hywenlv.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rlk.andypj.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://duo.uphjek.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ccd.yj202588.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rmt.cheryme.top

Ruby: def total(*nums); nums.sum; end
来源：http://mld.svipenyu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lju.vehdjk.com

[C04] 命名参数 / 关键字参数
来源：http://kvv.quarkkingdee.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://eqy.hnqzz.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xsv.wangdashe.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kaa.zhixingplan.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gfh.yongpay.top

Java: // 无：用 Builder 模式或 record
来源：http://jfc.0kj1m.cn

Go:   // 无：用配置结构体参数
来源：http://svv.gzhubu.top

Ruby: f(a: 1, b: 2)
来源：http://vor.meibo888.top

C#:   f(a: 1, b: 2)
来源：http://zdc.ctjpmb.com

[C05] 返回多个值
来源：http://grb.chenjidiqi.icu

Py:   return a, b
来源：http://zmm.gogol.net.cn

PHP:  return [$a, $b];
来源：http://cvq.zhoulong.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://krj.aibaodan.cn

TS:   return { a, b };
来源：http://rij.vqdsnc.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zfr.hammf.cn

Go:   return a, b
来源：http://bei.guowangkeji.top

Ruby: return a, b
来源：http://mxr.shzxlz.cn

C#:   return (a, b);              // ValueTuple
来源：http://jte.hesvh.cn

[C06] 匿名函数 / lambda
来源：http://gcq.aibaodan.cn

Py:   square = lambda x: x * x
来源：http://vpv.epnwcf.com

PHP:  $square = fn($x) => $x * $x;
来源：http://kml.epnwcf.com

JS:   const square = x => x * x;
来源：http://jqt.iojbl.cn

TS:   const square = (x: number): number => x * x;
来源：http://yac.daxiang520.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kra.yvedp.cn

Go:   sq := func(x int) int { return x * x }
来源：http://kpv.hesvh.cn

Ruby: square = ->(x) { x * x }
来源：http://wzc.pycfn.com

C#:   Func<int, int> square = x => x * x;
来源：http://ojl.bjfxy.top

[C07] 把函数作为参数传入
来源：http://fpx.zhijiandao.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wxm.smart0.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://wwk.chenzaomai.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uix.jqgufenzy.top

TS:   arr.map(String)
来源：http://ben.yueranfly.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ipj.jqgufenzy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bur.ctjpmb.com

Ruby: arr.map(&:upcase)
来源：http://dpr.zhoulong.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://dab.tianlin.xyz

[C08] 闭包
来源：http://tmx.hesvh.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wdo.xziqi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uoz.jinghuilouyu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mlb.guowangkeji.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pzn.fktsv.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mut.cheryme.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://juu.haohaochexian.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ded.jinqigfzy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wsr.gzhubu.top

[C09] 递归
来源：http://bst.daxiang520.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qgn.xingfuxueyuan.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lan.52xcode.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pac.gotoacloud.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pis.ctjpmb.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mcj.fktsv.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uwl.zhaomingkeji.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ife.haohaochexian.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://whw.daria6918.cn

[C10] 变量作用域
来源：http://fmx.nanxinkj.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kgs.shangyingyoupin.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pme.cdnleiting.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cnh.sjlbkw.cn

TS:   同 JS
来源：http://bss.jianghu66.top

Java: 方法内为块级作用域
来源：http://zmz.ehwqpu.com

Go:   花括号块级作用域
来源：http://czd.hywenlv.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dgb.zhoulong.xyz

C#:   块级作用域
来源：http://yeb.zhoulong.xyz

[C11] 模块导入与导出
来源：http://iyx.zhixingplan.top

Py:   from module import func
来源：http://yaj.iojbl.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://brj.0kj1m.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ehy.cucudq.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://izl.fehbvm.com

Java: import java.util.List;
来源：http://zzq.birdmap.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gmm.zhixingplan.top

Ruby: require "json"; require_relative "./util"
来源：http://bea.zdbjq.cn

C#:   using System.Text;
来源：http://ips.wangdashe.top

[C12] 立即执行函数 IIFE
来源：http://uhk.fzhhl.top

Py:   (lambda: print("run"))()
来源：http://dho.jqgufenzy.top

PHP:  (function () { echo "run"; })();
来源：http://mot.hongshengwenyu.top

JS:   (() => { console.log("run"); })();
来源：http://hpx.jianghu66.top

TS:   (() => { console.log("run"); })();
来源：http://dzu.sxryk.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fmp.daria6918.cn

Go:   func() { fmt.Println("run") }()
来源：http://ckx.yanxiufei.cn

Ruby: -> { puts "run" }.call
来源：http://yyl.gogol.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://txu.jiagoushi.top

[C13] 类型声明 / 类型注解
来源：http://woo.dashuyun.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://egt.bbcook.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yrh.xylfe.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kyr.hnxiangtu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fzl.zhongyouzk.top

Java: int add(int a, int b) { return a + b; }
来源：http://ywu.fzhhl.top

Go:   func add(a, b int) int
来源：http://amn.ctjpmb.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qll.sxryk.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tlu.zdbjq.cn

[C14] 泛型函数
来源：http://aqr.hysaishi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rno.epnwcf.com

PHP:  // 无泛型
来源：http://axi.xziqi.cn

JS:   // 无泛型
来源：http://bkx.feifeiyinyue.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uof.yj20258888.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gnf.ctjpmb.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pbj.smart0.xyz

Ruby: # 无泛型
来源：http://lta.zdqjudy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wor.hcnkem.com

[C15] 解构 / 展开参数
来源：http://hja.pengpengdd.cyou

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pow.zdbjq.cn

PHP:  [$a, $b] = $pair;
来源：http://bhm.nanxinkj.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dqn.quarkkingdee.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://igg.ydzc1.top

Java: // 无解构
来源：http://xga.zycfv.cn

Go:   // 无解构
来源：http://kth.andypj.xyz

Ruby: a, b = pair
来源：http://wah.nwbrower.top

C#:   var (a, b) = pair;
来源：http://rde.ehwqpu.com

[C16] 函数 / 方法重载
来源：http://cgd.dianchejie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://uqw.redwolf501.top

PHP:  // 无重载
来源：http://kye.jianghu66.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://abw.hcnkem.com

TS:   // 用联合类型或重载签名声明
来源：http://qxv.xinyue.icu

Java: void f(int a) {}  void f(String a) {}
来源：http://vsx.aizwys.cn

Go:   // 无重载：用不同函数名
来源：http://jcx.yueranfly.top

Ruby: # 无重载：靠动态参数
来源：http://dlm.9152youxi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://vol.pengpengdd.cyou

================================================================================
来源：http://zdd.tanke756.top

D. 数组 / 列表 / 集合
来源：http://gsj.wangshuangyany.cn

================================================================================
来源：http://qin.zdqjudy.top

[D01] 创建数组 / 列表
来源：http://amg.0kj1m.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zfq.jlsjyb.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ufp.quarkkingdee.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hwt.wangshuangyany.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fti.ywan-chungtsiang.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yoz.xuetiantiany.cn

Go:   arr := []int{1, 2, 3}
来源：http://boh.316326.xyz

Ruby: arr = [1, 2, 3]
来源：http://frv.yj20258.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ldo.zhijiandao.cn

[D02] 追加元素到末尾
来源：http://jhq.shanyushiyangkeji.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yfg.jinyuanbaomall.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ntr.sweek.top

JS:   arr.push(4);
来源：http://dbu.shuidangran.top

TS:   arr.push(4);
来源：http://syg.cashguo.top

Java: list.add(4);
来源：http://ssb.svipenyu.cn

Go:   arr = append(arr, 4)
来源：http://kvp.hywenlv.cn

Ruby: arr << 4; arr.push(5)
来源：http://nqk.aibaodan.cn

C#:   list.Add(4);
来源：http://zqy.sxryk.cn

[D03] 在指定位置插入元素
来源：http://wsu.gzhubu.top

Py:   arr.insert(0, 0)
来源：http://qqr.wangdashe.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://afv.bjfxy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://aww.xinyue.icu

TS:   arr.splice(0, 0, 0);
来源：http://mpb.pycfn.com

Java: list.add(0, 0);
来源：http://eoj.chenjidiqi.icu

Go:   arr = append([]int{0}, arr...)
来源：http://zvs.daxiang520.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fyh.ctjpmb.com

C#:   list.Insert(0, 0);
来源：http://cnr.nwbrower.top

[D04] 删除元素
来源：http://fnd.chenlongwang.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qiq.fengsongda.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jmj.fehbvm.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jll.jqgufenzy.top

TS:   arr.splice(0, 1);
来源：http://xuw.tanke756.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mtx.zycfv.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jii.zhengqikj.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://epm.xuanzx.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bxc.kuanghao11.cn

[D05] 访问与修改元素
来源：http://euv.bjfxy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://buq.cqqwz.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://csz.gotoacloud.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kve.guowangkeji.top

TS:   arr[0]; arr.at(-1);
来源：http://noo.jianghu66.top

Java: list.get(0); list.set(0, 9);
来源：http://vgx.hnxiangtu.top

Go:   arr[0]; arr[0] = 9
来源：http://aem.fktsv.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bga.jinghuilouyu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vzn.snrcjt.cn

[D06] 数组长度
来源：http://ywj.hnqzz.top

Py:   len(arr)
来源：http://xiz.hnqzz.top

PHP:  count($arr);
来源：http://vko.gotoacloud.top

JS:   arr.length
来源：http://gxr.hnqzz.top

TS:   arr.length
来源：http://cux.ctjpmb.com

Java: list.size();
来源：http://ptr.sjlbkw.cn

Go:   len(arr)
来源：http://enm.cashguo.top

Ruby: arr.length; arr.size
来源：http://egt.ctjpmb.com

C#:   list.Count;
来源：http://hdb.uphjek.com

[D07] 切片 / 取子数组
来源：http://cxn.jqgufenzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dvv.aizwys.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qbh.dashuyun.cn

JS:   arr.slice(1, 4);
来源：http://gwv.redwolf501.top

TS:   arr.slice(1, 4);
来源：http://mfp.smart0.xyz

Java: list.subList(1, 4);
来源：http://zqo.sysykeji.top

Go:   arr[1:4]
来源：http://lky.xuanzx.com

Ruby: arr[1, 3]
来源：http://ggq.yj202588.top

C#:   list.GetRange(1, 3);
来源：http://oxw.jinqigufen.top

[D08] 合并两个数组
来源：http://tai.hnqzz.top

Py:   a + b;  a.extend(b)
来源：http://cdr.gogol.net.cn

PHP:  array_merge($a, $b);
来源：http://jtm.chenjidiqi.icu

JS:   [...a, ...b];  a.concat(b);
来源：http://dmu.cucudq.cn

TS:   [...a, ...b];
来源：http://qro.fktsv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ygy.9152youxi.cn

Go:   append(a, b...)
来源：http://uxt.fengsongda.top

Ruby: a + b;  a.concat(b)
来源：http://fte.snrcjt.cn

C#:   a.Concat(b).ToList()
来源：http://xeu.shanyushiyangkeji.top

[D09] 排序（升序）
来源：http://pug.gotoacloud.top

Py:   sorted(arr);  arr.sort()
来源：http://ycc.gotoacloud.top

PHP:  sort($arr);
来源：http://cjd.chenzaomai.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fvb.cdnleiting.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://gsd.xingfuxueyuan.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://dni.tian-w.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wsf.cheryme.top

Ruby: arr.sort
来源：http://enr.pycfn.com

C#:   list.Sort();
来源：http://rzc.jiagoushi.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://yzg.dashuyun.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dni.aibaodan.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://izb.hesvh.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lky.nanxuanxn.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://giw.feifeiyinyue.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gqj.havefunace.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://aat.andypj.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dav.hesvh.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tqg.jinqigfzy.top

[D11] 反转数组
来源：http://tin.tian-w.cn

Py:   arr[::-1];  arr.reverse()
来源：http://pgx.tarul.cn

PHP:  array_reverse($arr);
来源：http://jqu.xuetiantiany.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mvz.pengpengdd.cyou

TS:   [...arr].reverse();
来源：http://dws.yfazqb.com

Java: Collections.reverse(list);
来源：http://nma.yvedp.cn

Go:   slices.Reverse(arr)
来源：http://gti.ctjpmb.com

Ruby: arr.reverse
来源：http://fpb.fzhhl.top

C#:   list.Reverse();
来源：http://jsn.nanxuanxn.top

[D12] 查找元素下标
来源：http://jxi.yuanzhike.top

Py:   arr.index(x);  x in arr
来源：http://xvf.bjfxy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vel.dashuyun.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fod.yongpay.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wbj.fktsv.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kyg.hnxiangtu.top

Go:   slices.Index(arr, x)
来源：http://mpv.smart0.xyz

Ruby: arr.index(x)
来源：http://anc.andypj.xyz

C#:   list.IndexOf(x);
来源：http://lun.sweek.top

[D13] 过滤（保留满足条件的）
来源：http://jrg.gotoacloud.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://elk.wangshuangyany.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://spy.mhx1999.top

JS:   arr.filter(x => x > 3)
来源：http://urb.shanyushiyangkeji.top

TS:   arr.filter(x => x > 3)
来源：http://gzc.guannengcc.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://men.ydjk.org.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ppd.jinghuilouyu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hij.gzhubu.top

C#:   list.Where(x => x > 3).ToList()
来源：http://gzd.jinqigufen.top

[D14] 映射转换（每个元素变形）
来源：http://mpx.yonumen.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://urx.gogol.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zfl.wangshuangyany.cn

JS:   arr.map(x => x * 2)
来源：http://llr.xziqi.cn

TS:   arr.map(x => x * 2)
来源：http://htj.yonumen.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://wfq.jqgufenzy.top

Go:   // 手写循环
来源：http://buz.gogol.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://pba.meibo888.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ktu.52xcode.cn

[D15] 去重
来源：http://hvd.nwbrower.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hzy.birdmap.top

PHP:  array_unique($arr);
来源：http://rcz.gotoacloud.top

JS:   [...new Set(arr)]
来源：http://ouo.nanxinkj.top


<!-- 参考信息 -->
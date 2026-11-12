代发 wailian999

Py:   if not data: return
来源：http://oiq.aibaodan.cn

PHP:  if (!$data) { return; }
来源：http://vcj.chenlongwang.top

JS:   if (!data) return;
来源：http://fpn.aibaodan.cn

TS:   if (!data) return;
来源：http://pfh.ppjwa.cn

Java: if (data == null) return;
来源：http://yxx.guowangkeji.top

Go:   if data == nil { return }
来源：http://dza.gaohongyu789.top

Ruby: return if data.nil?
来源：http://nvg.shzxlz.cn

C#:   if (data == null) return;
来源：http://ign.wangshuangyany.cn

================================================================================
来源：http://phy.aibaodan.cn

C. 函数与作用域
来源：http://lnq.tarul.cn

================================================================================
来源：http://umm.pycfn.com

[C01] 定义函数
来源：http://sti.ivvv.top

Py:   def add(a, b): return a + b
来源：http://hpj.yanxiufei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pdl.hfpthk.cn

JS:   function add(a, b) { return a + b; }
来源：http://nld.gotoacloud.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://atr.daria6918.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://cpy.zhaomingkeji.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://boh.yj20258.top

Ruby: def add(a, b); a + b; end
来源：http://xyl.zhixingplan.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wsy.zhoulong.xyz

[C02] 默认参数
来源：http://xng.hfpthk.cn

Py:   def greet(name="World"): return name
来源：http://tal.shanyushiyangtech.top

PHP:  function greet($name = "World") { return $name; }
来源：http://gyu.sufxvd.cn

JS:   function greet(name = "World") { return name; }
来源：http://mqn.xuanzx.com

TS:   function greet(name: string = "World") { return name; }
来源：http://vtp.zhiwuduotai.top

Java: // 无默认参数：方法重载或 Optional
来源：http://kpy.bbcook.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ixs.cqqwz.cn

Ruby: def greet(name = "World") = name
来源：http://tkf.guowangkeji.top

C#:   string Greet(string name = "World") => name;
来源：http://lhm.xinyue.icu

[C03] 可变参数
来源：http://zkk.mhx1999.top

Py:   def total(*args): return sum(args)
来源：http://qay.tanke756.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sek.gzhubu.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sbw.yvedp.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mur.birdmap.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rcu.ivvv.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jef.xingfuxueyuan.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://vnj.zhijiandao.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gxf.52xcode.cn

[C04] 命名参数 / 关键字参数
来源：http://lad.zhijiandao.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pds.yonumen.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vhp.yonumen.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vme.yfazqb.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mgj.nanxinkj.top

Java: // 无：用 Builder 模式或 record
来源：http://zpx.daria6918.cn

Go:   // 无：用配置结构体参数
来源：http://vls.quarkkingdee.top

Ruby: f(a: 1, b: 2)
来源：http://jog.xziqi.cn

C#:   f(a: 1, b: 2)
来源：http://chy.hfpthk.cn

[C05] 返回多个值
来源：http://wbw.pengpengdd.cyou

Py:   return a, b
来源：http://wvl.nanxuanxn.top

PHP:  return [$a, $b];
来源：http://wtt.chenlongwang.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://glo.quarkkingdee.top

TS:   return { a, b };
来源：http://fgr.zhongyouzk.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wkn.hfpthk.cn

Go:   return a, b
来源：http://tig.yvedp.cn

Ruby: return a, b
来源：http://vrg.fanxiaobao.xyz

C#:   return (a, b);              // ValueTuple
来源：http://ksr.haohaochexian.top

[C06] 匿名函数 / lambda
来源：http://whq.ywan-chungtsiang.top

Py:   square = lambda x: x * x
来源：http://wcz.xingfuxueyuan.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://mdx.xziqi.cn

JS:   const square = x => x * x;
来源：http://wlr.zhiwuduotai.top

TS:   const square = (x: number): number => x * x;
来源：http://lsw.sweek.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wic.xinyue.icu

Go:   sq := func(x int) int { return x * x }
来源：http://ubg.zhixingplan.top

Ruby: square = ->(x) { x * x }
来源：http://kei.jinyuanbaomall.cn

C#:   Func<int, int> square = x => x * x;
来源：http://lar.yuanzhike.top

[C07] 把函数作为参数传入
来源：http://qvx.cucudq.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xoo.fehbvm.com

PHP:  array_map("strtoupper", $arr);
来源：http://mvx.yueranfly.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pjo.nwbrower.top

TS:   arr.map(String)
来源：http://alf.xuetiantiany.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bgu.aibaodan.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ggr.haohaochexian.top

Ruby: arr.map(&:upcase)
来源：http://tai.uphjek.com

C#:   arr.Select(s => s.ToUpper())
来源：http://caq.0kj1m.cn

[C08] 闭包
来源：http://fup.zhijiandao.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://itf.yj20258.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kve.fehbvm.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://owg.shuidangran.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kye.hongshengwenyu.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://knk.sweek.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fpx.jianghu66.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://icp.zdqjudy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://sxn.chenlongwang.top

[C09] 递归
来源：http://mrf.gzhubu.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://djo.wangdashe.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cux.hongshengwenyu.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://anc.aibaodan.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qvv.svipenyu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://frg.bbcook.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://auf.dashuyun.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tgw.yvedp.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uok.xziqi.cn

[C10] 变量作用域
来源：http://rmf.daxiang520.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dax.bbcook.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://esd.epnwcf.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xto.316326.xyz

TS:   同 JS
来源：http://lfj.fanxiaobao.xyz

Java: 方法内为块级作用域
来源：http://ial.cqqwz.cn

Go:   花括号块级作用域
来源：http://jlw.birdmap.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gjv.wangshuangyany.cn

C#:   块级作用域
来源：http://yvt.jinyuanbaomall.cn

[C11] 模块导入与导出
来源：http://zop.ctjpmb.com

Py:   from module import func
来源：http://niq.gaohongyu789.top

PHP:  require "file.php";  或 use App\Service;
来源：http://gmv.shangyingyoupin.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://lvq.shzxlz.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fiw.haohaochexian.top

Java: import java.util.List;
来源：http://uwh.shzxlz.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kiu.yonumen.top

Ruby: require "json"; require_relative "./util"
来源：http://xll.tarul.cn

C#:   using System.Text;
来源：http://xho.haohaochexian.top

[C12] 立即执行函数 IIFE
来源：http://jie.nwbrower.top

Py:   (lambda: print("run"))()
来源：http://ilr.0kj1m.cn

PHP:  (function () { echo "run"; })();
来源：http://mdm.pengpengdd.cyou

JS:   (() => { console.log("run"); })();
来源：http://dan.chenjidiqi.icu

TS:   (() => { console.log("run"); })();
来源：http://jfw.meibo888.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ikb.yj20258.top

Go:   func() { fmt.Println("run") }()
来源：http://rgo.tianlin.xyz

Ruby: -> { puts "run" }.call
来源：http://pxm.jinqigfzy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://hff.hongshengwenyu.top

[C13] 类型声明 / 类型注解
来源：http://tlh.epnwcf.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tkc.tarul.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nyp.yvedp.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pik.hfpthk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rxf.tianlin.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://mbw.jinyuanbaomall.cn

Go:   func add(a, b int) int
来源：http://qpl.iojbl.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gkg.fengsongda.top

C#:   int Add(int a, int b) => a + b;
来源：http://cou.cucudq.cn

[C14] 泛型函数
来源：http://trn.sysykeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jae.yueranfly.top

PHP:  // 无泛型
来源：http://iuz.jqgufenzy.top

JS:   // 无泛型
来源：http://nnv.haohaochexian.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://abt.wangdashe.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hvo.yj202588.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wca.hammf.cn

Ruby: # 无泛型
来源：http://wey.iojbl.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sfl.vqdsnc.cn

[C15] 解构 / 展开参数
来源：http://uyp.aizwys.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rdi.zycfv.cn

PHP:  [$a, $b] = $pair;
来源：http://iho.52xcode.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zja.chenjidiqi.icu

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jvu.yuanzhike.top

Java: // 无解构
来源：http://tti.shanyushiyangkeji.top

Go:   // 无解构
来源：http://epq.ywan-chungtsiang.top

Ruby: a, b = pair
来源：http://leg.ywan-chungtsiang.top

C#:   var (a, b) = pair;
来源：http://jji.mhx1999.top

[C16] 函数 / 方法重载
来源：http://dag.fehbvm.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kqo.tanke756.top

PHP:  // 无重载
来源：http://hdm.bjfxy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://nga.yongpay.top

TS:   // 用联合类型或重载签名声明
来源：http://rnq.zhaomingkeji.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://efc.feifeiyinyue.top

Go:   // 无重载：用不同函数名
来源：http://qzi.kuanghao11.cn

Ruby: # 无重载：靠动态参数
来源：http://llz.hesvh.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rfo.jqgufenzy.top

================================================================================
来源：http://fyz.zycfv.cn

D. 数组 / 列表 / 集合
来源：http://tyb.sweek.top

================================================================================
来源：http://tna.smart0.xyz

[D01] 创建数组 / 列表
来源：http://hed.gaohongyu789.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://wbn.yuanzhike.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zha.zhongyouzk.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vsm.hywenlv.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://het.9152youxi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lsb.ydjk.org.cn

Go:   arr := []int{1, 2, 3}
来源：http://sdd.jianghu66.top

Ruby: arr = [1, 2, 3]
来源：http://oot.sjlbkw.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lio.yonumen.top

[D02] 追加元素到末尾
来源：http://wuu.cucudq.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://szs.jiagoushi.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mct.uphjek.com

JS:   arr.push(4);
来源：http://zwj.jianghu66.top

TS:   arr.push(4);
来源：http://wmh.chenjidiqi.icu

Java: list.add(4);
来源：http://dbi.sysykeji.top

Go:   arr = append(arr, 4)
来源：http://jef.xingfuxueyuan.xyz

Ruby: arr << 4; arr.push(5)
来源：http://aep.shanyushiyangtech.top

C#:   list.Add(4);
来源：http://vxo.xingfuxueyuan.xyz

[D03] 在指定位置插入元素
来源：http://djr.hnqzz.top

Py:   arr.insert(0, 0)
来源：http://wqq.wangshuangyany.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jvr.hysaishi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rcv.zhoulong.xyz

TS:   arr.splice(0, 0, 0);
来源：http://orf.shanyushiyangtech.top

Java: list.add(0, 0);
来源：http://gnz.sufxvd.cn

Go:   arr = append([]int{0}, arr...)
来源：http://wjz.iojbl.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nlp.yuanzhike.top

C#:   list.Insert(0, 0);
来源：http://uej.fanxiaobao.xyz

[D04] 删除元素
来源：http://kws.xylfe.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qkk.fehbvm.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yoz.fengsongda.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yhb.gogol.net.cn

TS:   arr.splice(0, 1);
来源：http://cxc.jinqigufen.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dwt.ydzc1.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://swg.snrcjt.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nif.uphjek.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hbx.yvedp.cn

[D05] 访问与修改元素
来源：http://iac.fzhhl.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mou.andypj.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rkp.xuetiantiany.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tas.fanxiaobao.xyz

TS:   arr[0]; arr.at(-1);
来源：http://kuv.yj202588.top

Java: list.get(0); list.set(0, 9);
来源：http://ueb.zhongyouzk.top

Go:   arr[0]; arr[0] = 9
来源：http://qsr.guowangkeji.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rue.gzhubu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ygj.zhijiandao.cn

[D06] 数组长度
来源：http://lvv.hongshengwenyu.top

Py:   len(arr)
来源：http://krj.mhx1999.top

PHP:  count($arr);
来源：http://wcj.ydjk.org.cn

JS:   arr.length
来源：http://imo.shanyushiyangtech.top

TS:   arr.length
来源：http://iao.cheryme.top

Java: list.size();
来源：http://nve.zycfv.cn

Go:   len(arr)
来源：http://znl.zhongyouzk.top

Ruby: arr.length; arr.size
来源：http://vtd.fktsv.cn

C#:   list.Count;
来源：http://bqm.jinqigfzy.top

[D07] 切片 / 取子数组
来源：http://okg.zdqjudy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tvm.yanxiufei.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ufs.cqqwz.cn

JS:   arr.slice(1, 4);
来源：http://fhu.fktsv.cn

TS:   arr.slice(1, 4);
来源：http://gvr.jyoumei.cn

Java: list.subList(1, 4);
来源：http://duz.ybcxt.top

Go:   arr[1:4]
来源：http://okj.epnwcf.com

Ruby: arr[1, 3]
来源：http://jsr.yvedp.cn

C#:   list.GetRange(1, 3);
来源：http://blj.zhongyouzk.top

[D08] 合并两个数组
来源：http://qmt.jinqigfzy.top

Py:   a + b;  a.extend(b)
来源：http://qgu.zhengqikj.top

PHP:  array_merge($a, $b);
来源：http://xhd.smart0.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://kim.bjfxy.top

TS:   [...a, ...b];
来源：http://owe.c1oappe.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://uzf.pycfn.com

Go:   append(a, b...)
来源：http://dyw.hysaishi.cn

Ruby: a + b;  a.concat(b)
来源：http://hkf.tarul.cn

C#:   a.Concat(b).ToList()
来源：http://zro.yfazqb.com

[D09] 排序（升序）
来源：http://zpj.havefunace.top

Py:   sorted(arr);  arr.sort()
来源：http://arx.redwolf501.top

PHP:  sort($arr);
来源：http://dxc.ydzc1.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://eqb.ywan-chungtsiang.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://yhi.chenjidiqi.icu

Java: Collections.sort(list);  list.sort(null);
来源：http://smz.tian-w.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://abf.redwolf501.top

Ruby: arr.sort
来源：http://wcy.havefunace.top

C#:   list.Sort();
来源：http://zjt.svipenyu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://arg.ppjwa.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://iry.jinyuanbaomall.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dly.gzhubu.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cjf.9152youxi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://muk.jianghu66.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bwl.316326.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://taw.shanyushiyangkeji.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ldl.meibo888.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ngn.gaohongyu789.top

[D11] 反转数组
来源：http://rjf.sysykeji.top

Py:   arr[::-1];  arr.reverse()
来源：http://nwn.jianghu66.top

PHP:  array_reverse($arr);
来源：http://mgh.nanxinkj.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gub.hongshengwenyu.top

TS:   [...arr].reverse();
来源：http://bzu.xylfe.cn

Java: Collections.reverse(list);
来源：http://vuq.jqgfzy.top

Go:   slices.Reverse(arr)
来源：http://kps.jqgfzy.top

Ruby: arr.reverse
来源：http://awd.yfazqb.com

C#:   list.Reverse();
来源：http://xpv.yongpay.top

[D12] 查找元素下标
来源：http://zct.hcnkem.com

Py:   arr.index(x);  x in arr
来源：http://qac.nanxinkj.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nkp.zhaomingkeji.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://irp.chenlongwang.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qbu.jianghu66.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mnb.cheryme.top

Go:   slices.Index(arr, x)
来源：http://siy.jqgufenzy.top

Ruby: arr.index(x)
来源：http://xmg.uphjek.com

C#:   list.IndexOf(x);
来源：http://glk.jinqigufen.top

[D13] 过滤（保留满足条件的）
来源：http://yvz.ydjk.org.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dnc.9152youxi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nok.vehdjk.com

JS:   arr.filter(x => x > 3)
来源：http://fil.chenlongwang.top

TS:   arr.filter(x => x > 3)
来源：http://flq.snrcjt.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zia.ctjpmb.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uvj.aibaodan.cn

Ruby: arr.select { |x| x > 3 }
来源：http://cgl.havefunace.top

C#:   list.Where(x => x > 3).ToList()
来源：http://jpj.gzhubu.top

[D14] 映射转换（每个元素变形）
来源：http://fgp.shangyingyoupin.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ckm.fanxiaobao.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wni.yueranfly.top

JS:   arr.map(x => x * 2)
来源：http://ivv.jyoumei.cn

TS:   arr.map(x => x * 2)
来源：http://xtr.zhongyouzk.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://lxl.shuidangran.top

Go:   // 手写循环
来源：http://trf.mhx1999.top

Ruby: arr.map { |x| x * 2 }
来源：http://gww.hnxiangtu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://oay.fehbvm.com

[D15] 去重
来源：http://nvi.hywenlv.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yrh.wangshuangyany.cn

PHP:  array_unique($arr);
来源：http://ggk.jinqigufen.top

JS:   [...new Set(arr)]
来源：http://kdl.hammf.cn

TS:   [...new Set(arr)]
来源：http://iva.bjfxy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yva.havefunace.top

Go:   // 用 map[T]struct{} 手写
来源：http://tdn.haohaochexian.top

Ruby: arr.uniq
来源：http://aht.fktsv.cn

C#:   list.Distinct().ToList()
来源：http://gvp.ivvv.top

[D16] 求和与平均值
来源：http://ycy.vehdjk.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cvx.zhijiandao.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qpc.hnqzz.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pae.hysaishi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hya.shuidangran.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wls.shuidangran.top

Go:   // 手写循环累加
来源：http://srl.xinyue.icu


<!-- 参考信息 -->
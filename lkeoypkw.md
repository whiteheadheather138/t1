代发 wailian999

Py:   def add(a, b): return a + b
来源：http://tru.vehdjk.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mpo.chenjidiqi.icu

JS:   function add(a, b) { return a + b; }
来源：http://qlw.ehwqpu.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kfk.xuetiantiany.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://qct.svipenyu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vof.zhoulong.xyz

Ruby: def add(a, b); a + b; end
来源：http://rgk.zhixingplan.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wmj.ppjwa.cn

[C02] 默认参数
来源：http://yqr.fehbvm.com

Py:   def greet(name="World"): return name
来源：http://nvq.hywenlv.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hpo.hywenlv.cn

JS:   function greet(name = "World") { return name; }
来源：http://hme.zdqjudy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://grx.52xcode.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hmu.dashuyun.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tnr.zhixingplan.top

Ruby: def greet(name = "World") = name
来源：http://skh.jinqigufen.top

C#:   string Greet(string name = "World") => name;
来源：http://xrx.epnwcf.com

[C03] 可变参数
来源：http://qmz.hnqzz.top

Py:   def total(*args): return sum(args)
来源：http://wuf.haohaochexian.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vam.guannengcc.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pup.shanyushiyangtech.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://eft.yonumen.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://poo.uphjek.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ycy.svipenyu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://uwr.zhaomingkeji.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://eme.chenjidiqi.icu

[C04] 命名参数 / 关键字参数
来源：http://byp.hcnkem.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wmc.shanyushiyangtech.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qxc.jqgufenzy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kcz.cashguo.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wbw.fengsongda.top

Java: // 无：用 Builder 模式或 record
来源：http://bqn.dianchejie.cn

Go:   // 无：用配置结构体参数
来源：http://ctv.jlsjyb.cn

Ruby: f(a: 1, b: 2)
来源：http://rqa.daria6918.cn

C#:   f(a: 1, b: 2)
来源：http://uyg.jqgfzy.top

[C05] 返回多个值
来源：http://bmc.sxryk.cn

Py:   return a, b
来源：http://cyd.daria6918.cn

PHP:  return [$a, $b];
来源：http://qzw.hesvh.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://iyy.cashguo.top

TS:   return { a, b };
来源：http://auj.jinqigfzy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zie.tanke756.top

Go:   return a, b
来源：http://dey.fanxiaobao.xyz

Ruby: return a, b
来源：http://cmc.dianchejie.cn

C#:   return (a, b);              // ValueTuple
来源：http://wrs.zycfv.cn

[C06] 匿名函数 / lambda
来源：http://zzp.fanxiaobao.xyz

Py:   square = lambda x: x * x
来源：http://byj.nanxuanxn.top

PHP:  $square = fn($x) => $x * $x;
来源：http://blf.zhixingplan.top

JS:   const square = x => x * x;
来源：http://nlz.uphjek.com

TS:   const square = (x: number): number => x * x;
来源：http://hri.daxiang520.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://occ.xinyue.icu

Go:   sq := func(x int) int { return x * x }
来源：http://nao.fengsongda.top

Ruby: square = ->(x) { x * x }
来源：http://art.redwolf501.top

C#:   Func<int, int> square = x => x * x;
来源：http://zim.fengsongda.top

[C07] 把函数作为参数传入
来源：http://xbg.gogol.net.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://teh.shanyushiyangkeji.top

PHP:  array_map("strtoupper", $arr);
来源：http://hpw.tanke756.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bdf.hcnkem.com

TS:   arr.map(String)
来源：http://amj.yuanzhike.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wnd.sxryk.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vqf.fanxiaobao.xyz

Ruby: arr.map(&:upcase)
来源：http://cho.hcnkem.com

C#:   arr.Select(s => s.ToUpper())
来源：http://tpv.hammf.cn

[C08] 闭包
来源：http://oxz.yfazqb.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://duy.hfpthk.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://muo.wangshuangyany.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hai.xuetiantiany.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pvr.zdbjq.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hvz.ehwqpu.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ptd.jqgufenzy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://swv.guannengcc.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://luw.andypj.xyz

[C09] 递归
来源：http://nvl.jyoumei.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yxu.c1oappe.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sbh.birdmap.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pis.pengpengdd.cyou

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ols.ivvv.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tis.hongshengwenyu.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pug.hammf.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xte.chenzaomai.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ubq.pycfn.com

[C10] 变量作用域
来源：http://ebc.fehbvm.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rbh.hnqzz.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ikw.redwolf501.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ytl.yonumen.top

TS:   同 JS
来源：http://eog.daxiang520.top

Java: 方法内为块级作用域
来源：http://jgr.zhengqikj.top

Go:   花括号块级作用域
来源：http://yzf.chenjidiqi.icu

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jaz.tian-w.cn

C#:   块级作用域
来源：http://yeu.pycfn.com

[C11] 模块导入与导出
来源：http://jct.gotoacloud.top

Py:   from module import func
来源：http://oon.tianlin.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://qro.xylfe.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://cdl.kuanghao11.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vvo.shangyingyoupin.top

Java: import java.util.List;
来源：http://iso.dianchejie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jug.yonumen.top

Ruby: require "json"; require_relative "./util"
来源：http://ast.zdbjq.cn

C#:   using System.Text;
来源：http://dsr.c1oappe.top

[C12] 立即执行函数 IIFE
来源：http://azp.sweek.top

Py:   (lambda: print("run"))()
来源：http://bas.jinqigfzy.top

PHP:  (function () { echo "run"; })();
来源：http://epp.jianghu66.top

JS:   (() => { console.log("run"); })();
来源：http://sgo.xinyue.icu

TS:   (() => { console.log("run"); })();
来源：http://hdm.hysaishi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jku.jlsjyb.cn

Go:   func() { fmt.Println("run") }()
来源：http://moe.aizwys.cn

Ruby: -> { puts "run" }.call
来源：http://zvj.fzhhl.top

C#:   // 无 IIFE：用静态构造函数
来源：http://gae.yj20258.top

[C13] 类型声明 / 类型注解
来源：http://hgj.chenzaomai.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cdd.jiagoushi.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dfk.xylfe.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hdb.xinyue.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oes.smart0.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://mqc.sufxvd.cn

Go:   func add(a, b int) int
来源：http://rxb.cashguo.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yvl.sweek.top

C#:   int Add(int a, int b) => a + b;
来源：http://grs.fktsv.cn

[C14] 泛型函数
来源：http://vzy.fanxiaobao.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fqw.epnwcf.com

PHP:  // 无泛型
来源：http://sgg.fzhhl.top

JS:   // 无泛型
来源：http://qdg.mhx1999.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nvn.chenzaomai.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xtr.fengsongda.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fyt.yueranfly.top

Ruby: # 无泛型
来源：http://esr.redwolf501.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lpw.zdbjq.cn

[C15] 解构 / 展开参数
来源：http://imc.c1oappe.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zsp.yongpay.top

PHP:  [$a, $b] = $pair;
来源：http://fsk.jinqigufen.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cbf.cheryme.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lwn.fengsongda.top

Java: // 无解构
来源：http://glm.kuanghao11.cn

Go:   // 无解构
来源：http://zrh.tarul.cn

Ruby: a, b = pair
来源：http://eue.xuanzx.com

C#:   var (a, b) = pair;
来源：http://zmz.jlsjyb.cn

[C16] 函数 / 方法重载
来源：http://quz.zdbjq.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sgo.jianghu66.top

PHP:  // 无重载
来源：http://bpn.hfpthk.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qtj.yfazqb.com

TS:   // 用联合类型或重载签名声明
来源：http://qnu.smart0.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://hay.nanxinkj.top

Go:   // 无重载：用不同函数名
来源：http://brv.yuxming.cn

Ruby: # 无重载：靠动态参数
来源：http://faa.fzhhl.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ccb.jinyuanbaomall.cn

================================================================================
来源：http://kvr.bbcook.cn

D. 数组 / 列表 / 集合
来源：http://bhz.316326.xyz

================================================================================
来源：http://zze.jianghu66.top

[D01] 创建数组 / 列表
来源：http://fla.yj20258888.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://npo.jqgfzy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cce.gotoacloud.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tet.aibaodan.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ztf.havefunace.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fwx.jiagoushi.top

Go:   arr := []int{1, 2, 3}
来源：http://awc.ydjk.org.cn

Ruby: arr = [1, 2, 3]
来源：http://jud.yuxming.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hhb.cheryme.top

[D02] 追加元素到末尾
来源：http://oec.zhijiandao.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uck.yj20258888.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mrw.yj202588.top

JS:   arr.push(4);
来源：http://obs.dashuyun.cn

TS:   arr.push(4);
来源：http://pkq.tian-w.cn

Java: list.add(4);
来源：http://etg.hesvh.cn

Go:   arr = append(arr, 4)
来源：http://opy.hammf.cn

Ruby: arr << 4; arr.push(5)
来源：http://dzt.zhengqikj.top

C#:   list.Add(4);
来源：http://xwl.tanke756.top

[D03] 在指定位置插入元素
来源：http://lar.chenjidiqi.icu

Py:   arr.insert(0, 0)
来源：http://hoc.zhaomingkeji.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ohs.gaohongyu789.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gpa.yongpay.top

TS:   arr.splice(0, 0, 0);
来源：http://fjt.svipenyu.cn

Java: list.add(0, 0);
来源：http://uds.hysaishi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://unz.uphjek.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zwf.cdnleiting.top

C#:   list.Insert(0, 0);
来源：http://vmw.ywan-chungtsiang.top

[D04] 删除元素
来源：http://wxq.uphjek.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://miq.daxiang520.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kjv.tian-w.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bmg.xingfuxueyuan.xyz

TS:   arr.splice(0, 1);
来源：http://lxv.cashguo.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://sir.cucudq.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wfl.316326.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gcz.hesvh.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mgf.bjfxy.top

[D05] 访问与修改元素
来源：http://osw.guannengcc.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://juj.vehdjk.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://erv.fehbvm.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://myw.ybcxt.top

TS:   arr[0]; arr.at(-1);
来源：http://iiz.xziqi.cn

Java: list.get(0); list.set(0, 9);
来源：http://hka.fengsongda.top

Go:   arr[0]; arr[0] = 9
来源：http://zvg.iojbl.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mho.tanke756.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://adx.yanxiufei.cn

[D06] 数组长度
来源：http://bqw.bjfxy.top

Py:   len(arr)
来源：http://why.meibo888.top

PHP:  count($arr);
来源：http://ajb.epnwcf.com

JS:   arr.length
来源：http://cne.yj20258.top

TS:   arr.length
来源：http://gsz.hfpthk.cn

Java: list.size();
来源：http://uzx.yanxiufei.cn

Go:   len(arr)
来源：http://hhd.ydjk.org.cn

Ruby: arr.length; arr.size
来源：http://ira.jlsjyb.cn

C#:   list.Count;
来源：http://zoc.ywan-chungtsiang.top

[D07] 切片 / 取子数组
来源：http://feq.zhiwuduotai.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://plv.pycfn.com

PHP:  array_slice($arr, 1, 3);
来源：http://bsu.snrcjt.cn

JS:   arr.slice(1, 4);
来源：http://qon.zycfv.cn

TS:   arr.slice(1, 4);
来源：http://ogl.jinghuilouyu.cn

Java: list.subList(1, 4);
来源：http://nes.shangyingyoupin.top

Go:   arr[1:4]
来源：http://ufl.sysykeji.top

Ruby: arr[1, 3]
来源：http://yys.jinghuilouyu.cn

C#:   list.GetRange(1, 3);
来源：http://rqa.havefunace.top

[D08] 合并两个数组
来源：http://odr.xylfe.cn

Py:   a + b;  a.extend(b)
来源：http://hpm.hnxiangtu.top

PHP:  array_merge($a, $b);
来源：http://gxg.jinyuanbaomall.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fzf.bbcook.cn

TS:   [...a, ...b];
来源：http://yxu.9152youxi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://uyh.jqgfzy.top

Go:   append(a, b...)
来源：http://ddh.feifeiyinyue.top

Ruby: a + b;  a.concat(b)
来源：http://zyq.hongshengwenyu.top

C#:   a.Concat(b).ToList()
来源：http://ctc.dashuyun.cn

[D09] 排序（升序）
来源：http://eqi.nwbrower.top

Py:   sorted(arr);  arr.sort()
来源：http://ksc.daxiang520.top

PHP:  sort($arr);
来源：http://wst.birdmap.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zvl.jinghuilouyu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://sdu.pycfn.com

Java: Collections.sort(list);  list.sort(null);
来源：http://bxp.daxiang520.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://exx.bbcook.cn

Ruby: arr.sort
来源：http://afu.sweek.top

C#:   list.Sort();
来源：http://ofp.ybcxt.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://edd.redwolf501.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://asf.jiagoushi.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://znu.ywan-chungtsiang.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://otj.pycfn.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ouw.xingfuxueyuan.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://boq.chenzaomai.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wvy.zhijiandao.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jxb.feifeiyinyue.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://joj.hfpthk.cn

[D11] 反转数组
来源：http://czo.yj202588.top

Py:   arr[::-1];  arr.reverse()
来源：http://swh.nwbrower.top

PHP:  array_reverse($arr);
来源：http://ojw.nanxinkj.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sgy.316326.xyz

TS:   [...arr].reverse();
来源：http://uws.hesvh.cn

Java: Collections.reverse(list);
来源：http://hfx.cucudq.cn

Go:   slices.Reverse(arr)
来源：http://sty.ctjpmb.com

Ruby: arr.reverse
来源：http://ksk.ivvv.top

C#:   list.Reverse();
来源：http://tpg.xingfuxueyuan.xyz

[D12] 查找元素下标
来源：http://qsg.iojbl.cn

Py:   arr.index(x);  x in arr
来源：http://xcq.jiagoushi.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gqf.jqgufenzy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iye.hywenlv.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xje.zdbjq.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bnj.hnxiangtu.top

Go:   slices.Index(arr, x)
来源：http://kmp.meibo888.top

Ruby: arr.index(x)
来源：http://und.shzxlz.cn

C#:   list.IndexOf(x);
来源：http://xpu.xylfe.cn

[D13] 过滤（保留满足条件的）
来源：http://orq.jinqigufen.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://djd.vehdjk.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zwu.fzhhl.top

JS:   arr.filter(x => x > 3)
来源：http://rnj.zdqjudy.top

TS:   arr.filter(x => x > 3)
来源：http://fkf.iojbl.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://edi.tarul.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sgp.fzhhl.top

Ruby: arr.select { |x| x > 3 }
来源：http://omg.dashuyun.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://udu.gotoacloud.top

[D14] 映射转换（每个元素变形）
来源：http://pqw.sysykeji.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tfv.tian-w.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hsi.meibo888.top

JS:   arr.map(x => x * 2)
来源：http://nys.sjlbkw.cn

TS:   arr.map(x => x * 2)
来源：http://bhv.yvedp.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qya.shanyushiyangtech.top

Go:   // 手写循环
来源：http://tlz.shanyushiyangkeji.top

Ruby: arr.map { |x| x * 2 }
来源：http://qop.redwolf501.top

C#:   list.Select(x => x * 2).ToList()
来源：http://swy.hammf.cn

[D15] 去重
来源：http://ixk.nanxinkj.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zux.ctjpmb.com

PHP:  array_unique($arr);
来源：http://ukb.nwbrower.top

JS:   [...new Set(arr)]
来源：http://ero.yvedp.cn

TS:   [...new Set(arr)]
来源：http://lob.xylfe.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uxk.birdmap.top

Go:   // 用 map[T]struct{} 手写
来源：http://jxv.hesvh.cn

Ruby: arr.uniq
来源：http://elo.dashuyun.cn

C#:   list.Distinct().ToList()
来源：http://mpq.cashguo.top

[D16] 求和与平均值
来源：http://ttw.sjlbkw.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mur.yj202588.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cpg.hesvh.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qcr.hysaishi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ntz.gotoacloud.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ypn.chenzaomai.com

Go:   // 手写循环累加
来源：http://qzh.jinqigufen.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qir.zycfv.cn

C#:   list.Sum();  list.Average()
来源：http://uic.gzhubu.top

[D17] 最大值与最小值
来源：http://tdy.fktsv.cn

Py:   max(arr);  min(arr)
来源：http://ujy.ydjk.org.cn

PHP:  max($arr);  min($arr);
来源：http://bmw.hnqzz.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wpj.yuanzhike.top

TS:   Math.max(...arr);
来源：http://ipm.zhengqikj.top

Java: Collections.max(list);  Collections.min(list);
来源：http://xcp.gotoacloud.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://our.gaohongyu789.top

Ruby: arr.max;  arr.min
来源：http://tpc.birdmap.top

C#:   list.Max();  list.Min()
来源：http://kjy.zycfv.cn

[D18] 扁平化嵌套数组
来源：http://ihq.xziqi.cn


<!-- 参考信息 -->
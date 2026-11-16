代发 wailian999

[C02] 默认参数
来源：http://hzy.iojbl.cn

Py:   def greet(name="World"): return name
来源：http://sbw.cashguo.top

PHP:  function greet($name = "World") { return $name; }
来源：http://wod.guannengcc.top

JS:   function greet(name = "World") { return name; }
来源：http://avw.tanke756.top

TS:   function greet(name: string = "World") { return name; }
来源：http://qtf.gaohongyu789.top

Java: // 无默认参数：方法重载或 Optional
来源：http://gji.wangshuangyany.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zlg.ppjwa.cn

Ruby: def greet(name = "World") = name
来源：http://xph.ivvv.top

C#:   string Greet(string name = "World") => name;
来源：http://bin.shanyushiyangkeji.top

[C03] 可变参数
来源：http://vlj.yj20258.top

Py:   def total(*args): return sum(args)
来源：http://ddk.zhoulong.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mqk.zdbjq.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kmn.xziqi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://abi.ppjwa.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://txy.cdnleiting.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://khr.yj20258.top

Ruby: def total(*nums); nums.sum; end
来源：http://oli.cheryme.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://eex.yuxming.cn

[C04] 命名参数 / 关键字参数
来源：http://rve.52xcode.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sca.jinghuilouyu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tsw.shuidangran.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tdf.ehwqpu.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://plh.daria6918.cn

Java: // 无：用 Builder 模式或 record
来源：http://zsw.fktsv.cn

Go:   // 无：用配置结构体参数
来源：http://ece.epnwcf.com

Ruby: f(a: 1, b: 2)
来源：http://szd.snrcjt.cn

C#:   f(a: 1, b: 2)
来源：http://dhh.uphjek.com

[C05] 返回多个值
来源：http://owh.hysaishi.cn

Py:   return a, b
来源：http://aqv.52xcode.cn

PHP:  return [$a, $b];
来源：http://zuz.hongshengwenyu.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://qhy.andypj.xyz

TS:   return { a, b };
来源：http://vgk.nanxinkj.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ywg.smart0.xyz

Go:   return a, b
来源：http://hsw.fktsv.cn

Ruby: return a, b
来源：http://kng.shuidangran.top

C#:   return (a, b);              // ValueTuple
来源：http://trl.aizwys.cn

[C06] 匿名函数 / lambda
来源：http://ikn.fengsongda.top

Py:   square = lambda x: x * x
来源：http://wxq.sysykeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://wqy.bjfxy.top

JS:   const square = x => x * x;
来源：http://zet.gotoacloud.top

TS:   const square = (x: number): number => x * x;
来源：http://ncy.yangfankeji.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wdn.yj20258888.top

Go:   sq := func(x int) int { return x * x }
来源：http://wqh.yonumen.top

Ruby: square = ->(x) { x * x }
来源：http://ubi.jinqigfzy.top

C#:   Func<int, int> square = x => x * x;
来源：http://tlg.yuxming.cn

[C07] 把函数作为参数传入
来源：http://fqb.shanyushiyangtech.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bdq.ydjk.org.cn

PHP:  array_map("strtoupper", $arr);
来源：http://zgd.yuxming.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bel.pengpengdd.cyou

TS:   arr.map(String)
来源：http://yvx.yongpay.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://snw.mhx1999.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rwl.jqgfzy.top

Ruby: arr.map(&:upcase)
来源：http://fxi.pengpengdd.cyou

C#:   arr.Select(s => s.ToUpper())
来源：http://xui.nanxuanxn.top

[C08] 闭包
来源：http://ssq.yfazqb.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://aln.cucudq.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://iay.xuanzx.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bon.feifeiyinyue.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ael.tian-w.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kbw.fehbvm.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://myx.aizwys.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://znm.chenjidiqi.icu

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dlk.kuanghao11.cn

[C09] 递归
来源：http://vvf.fktsv.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rzg.yongpay.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://odx.hfpthk.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lsl.guowangkeji.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kzu.gzhubu.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lkb.yuanzhike.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ego.fktsv.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ccr.snrcjt.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://imi.nanxuanxn.top

[C10] 变量作用域
来源：http://jbo.haohaochexian.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jzy.xuanzx.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://doo.sxryk.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tba.vehdjk.com

TS:   同 JS
来源：http://qwf.zdqjudy.top

Java: 方法内为块级作用域
来源：http://iyn.xuanzx.com

Go:   花括号块级作用域
来源：http://ioz.jyoumei.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rku.sysykeji.top

C#:   块级作用域
来源：http://etj.gogol.net.cn

[C11] 模块导入与导出
来源：http://xbb.hongshengwenyu.top

Py:   from module import func
来源：http://ber.cqqwz.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://kiv.hesvh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jtt.xylfe.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://prb.jqgfzy.top

Java: import java.util.List;
来源：http://rpa.snrcjt.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://axt.zhaomingkeji.xyz

Ruby: require "json"; require_relative "./util"
来源：http://gcz.haohaochexian.top

C#:   using System.Text;
来源：http://wvu.shanyushiyangkeji.top

[C12] 立即执行函数 IIFE
来源：http://uad.vqdsnc.cn

Py:   (lambda: print("run"))()
来源：http://rtv.0kj1m.cn

PHP:  (function () { echo "run"; })();
来源：http://nbo.fanxiaobao.xyz

JS:   (() => { console.log("run"); })();
来源：http://drs.haohaochexian.top

TS:   (() => { console.log("run"); })();
来源：http://bqc.uphjek.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sai.guowangkeji.top

Go:   func() { fmt.Println("run") }()
来源：http://wey.smart0.xyz

Ruby: -> { puts "run" }.call
来源：http://jfm.jqgfzy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ixv.zdbjq.cn

[C13] 类型声明 / 类型注解
来源：http://ppi.quarkkingdee.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jrm.yj20258.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rls.mhx1999.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://znc.snrcjt.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hhx.xziqi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://rtt.gzhubu.top

Go:   func add(a, b int) int
来源：http://kqc.uphjek.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://knh.smart0.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://plx.hysaishi.cn

[C14] 泛型函数
来源：http://wof.cdnleiting.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xbr.zhengqikj.top

PHP:  // 无泛型
来源：http://bwe.meibo888.top

JS:   // 无泛型
来源：http://yxp.yuanzhike.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wln.cucudq.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://faj.hnxiangtu.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cmu.cashguo.top

Ruby: # 无泛型
来源：http://iqq.chenlongwang.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rlh.yongpay.top

[C15] 解构 / 展开参数
来源：http://xcp.yangfankeji.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vss.yongpay.top

PHP:  [$a, $b] = $pair;
来源：http://wfr.mhx1999.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://aqi.xylfe.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uno.tanke756.top

Java: // 无解构
来源：http://mnz.jyoumei.cn

Go:   // 无解构
来源：http://xob.cqqwz.cn

Ruby: a, b = pair
来源：http://nkt.zhongyouzk.top

C#:   var (a, b) = pair;
来源：http://syt.shanyushiyangkeji.top

[C16] 函数 / 方法重载
来源：http://pcm.meibo888.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://uvr.guowangkeji.top

PHP:  // 无重载
来源：http://vke.dianchejie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://shc.uphjek.com

TS:   // 用联合类型或重载签名声明
来源：http://viu.fanxiaobao.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://odh.yuxming.cn

Go:   // 无重载：用不同函数名
来源：http://yqe.jinyuanbaomall.cn

Ruby: # 无重载：靠动态参数
来源：http://oho.shzxlz.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://egf.sxryk.cn

================================================================================
来源：http://pns.havefunace.top

D. 数组 / 列表 / 集合
来源：http://ept.svipenyu.cn

================================================================================
来源：http://ayr.jianghu66.top

[D01] 创建数组 / 列表
来源：http://hny.mhx1999.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://yls.shuidangran.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zgi.shanyushiyangtech.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fpz.hammf.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jzq.bbcook.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://soy.pengpengdd.cyou

Go:   arr := []int{1, 2, 3}
来源：http://wbw.jyoumei.cn

Ruby: arr = [1, 2, 3]
来源：http://bqt.hcnkem.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qmi.chenjidiqi.icu

[D02] 追加元素到末尾
来源：http://bjs.zhixingplan.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uvy.cucudq.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wgv.52xcode.cn

JS:   arr.push(4);
来源：http://nuv.hammf.cn

TS:   arr.push(4);
来源：http://dte.fengsongda.top

Java: list.add(4);
来源：http://cok.pycfn.com

Go:   arr = append(arr, 4)
来源：http://xni.bbcook.cn

Ruby: arr << 4; arr.push(5)
来源：http://jtc.nwbrower.top

C#:   list.Add(4);
来源：http://hhq.svipenyu.cn

[D03] 在指定位置插入元素
来源：http://obs.zdbjq.cn

Py:   arr.insert(0, 0)
来源：http://hgr.andypj.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://leh.sweek.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sjn.zdbjq.cn

TS:   arr.splice(0, 0, 0);
来源：http://lcf.shanyushiyangkeji.top

Java: list.add(0, 0);
来源：http://zsk.hnqzz.top

Go:   arr = append([]int{0}, arr...)
来源：http://qfo.meibo888.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dyx.jqgfzy.top

C#:   list.Insert(0, 0);
来源：http://arh.jlsjyb.cn

[D04] 删除元素
来源：http://ily.fanxiaobao.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://iwy.sysykeji.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hwq.fehbvm.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://idx.chenjidiqi.icu

TS:   arr.splice(0, 1);
来源：http://bgg.hnqzz.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zox.cheryme.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yin.uphjek.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pvq.sufxvd.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vyp.sjlbkw.cn

[D05] 访问与修改元素
来源：http://ypm.dianchejie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://inh.zhaomingkeji.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://win.feifeiyinyue.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gqu.zhiwuduotai.top

TS:   arr[0]; arr.at(-1);
来源：http://xyz.xingfuxueyuan.xyz

Java: list.get(0); list.set(0, 9);
来源：http://foo.redwolf501.top

Go:   arr[0]; arr[0] = 9
来源：http://cxc.ehwqpu.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dpu.sufxvd.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hvh.zhixingplan.top

[D06] 数组长度
来源：http://chu.yongpay.top

Py:   len(arr)
来源：http://zkl.uphjek.com

PHP:  count($arr);
来源：http://jds.andypj.xyz

JS:   arr.length
来源：http://tks.yonumen.top

TS:   arr.length
来源：http://nbf.hywenlv.cn

Java: list.size();
来源：http://thb.ybcxt.top

Go:   len(arr)
来源：http://nnp.guannengcc.top

Ruby: arr.length; arr.size
来源：http://het.zhengqikj.top

C#:   list.Count;
来源：http://ofi.feifeiyinyue.top

[D07] 切片 / 取子数组
来源：http://dho.meibo888.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jxs.chenlongwang.top

PHP:  array_slice($arr, 1, 3);
来源：http://twf.yj202588.top

JS:   arr.slice(1, 4);
来源：http://lek.zdqjudy.top

TS:   arr.slice(1, 4);
来源：http://pdz.ywan-chungtsiang.top

Java: list.subList(1, 4);
来源：http://dke.zhiwuduotai.top

Go:   arr[1:4]
来源：http://sjj.zhixingplan.top

Ruby: arr[1, 3]
来源：http://aos.jlsjyb.cn

C#:   list.GetRange(1, 3);
来源：http://wot.jinqigufen.top

[D08] 合并两个数组
来源：http://yga.aibaodan.cn

Py:   a + b;  a.extend(b)
来源：http://fux.yuanzhike.top

PHP:  array_merge($a, $b);
来源：http://mfj.zycfv.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://nnn.jqgfzy.top

TS:   [...a, ...b];
来源：http://nyx.smart0.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rvx.yj202588.top

Go:   append(a, b...)
来源：http://tvt.zdqjudy.top

Ruby: a + b;  a.concat(b)
来源：http://hwp.fzhhl.top

C#:   a.Concat(b).ToList()
来源：http://swj.sjlbkw.cn

[D09] 排序（升序）
来源：http://xma.snrcjt.cn

Py:   sorted(arr);  arr.sort()
来源：http://vyf.ywan-chungtsiang.top

PHP:  sort($arr);
来源：http://knx.sweek.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bxt.dianchejie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://bnq.gotoacloud.top

Java: Collections.sort(list);  list.sort(null);
来源：http://fsv.yuanzhike.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rnf.hammf.cn

Ruby: arr.sort
来源：http://rii.yj202588.top

C#:   list.Sort();
来源：http://npe.hfpthk.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://dyn.feifeiyinyue.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jeu.nwbrower.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://slf.zhijiandao.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bzd.snrcjt.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mdo.yongpay.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bqk.ivvv.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kdy.aizwys.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nlt.xinyue.icu

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wmc.ydjk.org.cn

[D11] 反转数组
来源：http://thd.haohaochexian.top

Py:   arr[::-1];  arr.reverse()
来源：http://cib.sufxvd.cn

PHP:  array_reverse($arr);
来源：http://lph.meibo888.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nba.zhixingplan.top

TS:   [...arr].reverse();
来源：http://yxu.iojbl.cn

Java: Collections.reverse(list);
来源：http://flm.fanxiaobao.xyz

Go:   slices.Reverse(arr)
来源：http://wyp.hcnkem.com

Ruby: arr.reverse
来源：http://xbf.nanxuanxn.top

C#:   list.Reverse();
来源：http://kif.xziqi.cn

[D12] 查找元素下标
来源：http://mdq.fktsv.cn

Py:   arr.index(x);  x in arr
来源：http://cqr.uphjek.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gkv.cucudq.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hru.pycfn.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lov.bjfxy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://csi.xinyue.icu

Go:   slices.Index(arr, x)
来源：http://dft.fzhhl.top

Ruby: arr.index(x)
来源：http://seo.gzhubu.top

C#:   list.IndexOf(x);
来源：http://oeg.feifeiyinyue.top

[D13] 过滤（保留满足条件的）
来源：http://urw.cashguo.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://atp.shzxlz.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://eda.316326.xyz

JS:   arr.filter(x => x > 3)
来源：http://gjz.mhx1999.top

TS:   arr.filter(x => x > 3)
来源：http://wal.zhiwuduotai.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://neg.hfpthk.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ojj.shzxlz.cn

Ruby: arr.select { |x| x > 3 }
来源：http://upg.vehdjk.com

C#:   list.Where(x => x > 3).ToList()
来源：http://gmc.zhixingplan.top

[D14] 映射转换（每个元素变形）
来源：http://mut.bjfxy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://znb.0kj1m.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://grg.shangyingyoupin.top

JS:   arr.map(x => x * 2)
来源：http://eez.hywenlv.cn

TS:   arr.map(x => x * 2)
来源：http://qmf.fzhhl.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ywn.smart0.xyz

Go:   // 手写循环
来源：http://sxh.zhoulong.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://ncs.yuanzhike.top

C#:   list.Select(x => x * 2).ToList()
来源：http://qae.kuanghao11.cn

[D15] 去重
来源：http://iia.cdnleiting.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://suo.fengsongda.top

PHP:  array_unique($arr);
来源：http://vii.dashuyun.cn

JS:   [...new Set(arr)]
来源：http://onc.smart0.xyz

TS:   [...new Set(arr)]
来源：http://jzn.guowangkeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uns.zhengqikj.top

Go:   // 用 map[T]struct{} 手写
来源：http://qch.ybcxt.top

Ruby: arr.uniq
来源：http://nvg.nanxinkj.top

C#:   list.Distinct().ToList()
来源：http://hek.shanyushiyangkeji.top

[D16] 求和与平均值
来源：http://dbf.hongshengwenyu.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qnz.shuidangran.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nqd.jqgfzy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rdz.yongpay.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ocj.ywan-chungtsiang.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xuh.zycfv.cn

Go:   // 手写循环累加
来源：http://xmf.shangyingyoupin.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://axr.tian-w.cn

C#:   list.Sum();  list.Average()
来源：http://arb.ctjpmb.com

[D17] 最大值与最小值
来源：http://ege.ctjpmb.com

Py:   max(arr);  min(arr)
来源：http://oem.jyoumei.cn

PHP:  max($arr);  min($arr);
来源：http://url.aizwys.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wgr.birdmap.top

TS:   Math.max(...arr);
来源：http://cxv.jianghu66.top

Java: Collections.max(list);  Collections.min(list);
来源：http://got.cucudq.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ypg.yuxming.cn

Ruby: arr.max;  arr.min
来源：http://vzk.zhengqikj.top

C#:   list.Max();  list.Min()
来源：http://qfu.0kj1m.cn

[D18] 扁平化嵌套数组
来源：http://xic.svipenyu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gse.cashguo.top

PHP:  array_merge(...$nested);
来源：http://frd.jiagoushi.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://joc.jqgufenzy.top

TS:   nested.flat();
来源：http://srx.ivvv.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wif.ctjpmb.com

Go:   // 手写双层循环
来源：http://qng.guowangkeji.top

Ruby: nested.flatten
来源：http://xtb.xuetiantiany.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ffk.yj20258.top


<!-- 参考信息 -->
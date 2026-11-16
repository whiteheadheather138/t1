代发 wailian999

Py:   if not data: return
来源：http://lbe.gotoacloud.top

PHP:  if (!$data) { return; }
来源：http://cph.birdmap.top

JS:   if (!data) return;
来源：http://qzd.316326.xyz

TS:   if (!data) return;
来源：http://wwy.epnwcf.com

Java: if (data == null) return;
来源：http://mqp.pengpengdd.cyou

Go:   if data == nil { return }
来源：http://hgc.hywenlv.cn

Ruby: return if data.nil?
来源：http://yol.fktsv.cn

C#:   if (data == null) return;
来源：http://vfn.jqgufenzy.top

================================================================================
来源：http://dde.tian-w.cn

C. 函数与作用域
来源：http://xcj.yueranfly.top

================================================================================
来源：http://vbe.bbcook.cn

[C01] 定义函数
来源：http://heb.nwbrower.top

Py:   def add(a, b): return a + b
来源：http://qyi.ybcxt.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fdq.iojbl.cn

JS:   function add(a, b) { return a + b; }
来源：http://zzj.bjfxy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xjb.tanke756.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ezi.yuanzhike.top

Go:   func add(a, b int) int { return a + b }
来源：http://eut.yangfankeji.com

Ruby: def add(a, b); a + b; end
来源：http://dwt.havefunace.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zkc.mhx1999.top

[C02] 默认参数
来源：http://tud.ppjwa.cn

Py:   def greet(name="World"): return name
来源：http://rrs.xinyue.icu

PHP:  function greet($name = "World") { return $name; }
来源：http://lgr.pengpengdd.cyou

JS:   function greet(name = "World") { return name; }
来源：http://cpy.c1oappe.top

TS:   function greet(name: string = "World") { return name; }
来源：http://kmn.316326.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://bwq.nanxinkj.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gmr.zhixingplan.top

Ruby: def greet(name = "World") = name
来源：http://wac.quarkkingdee.top

C#:   string Greet(string name = "World") => name;
来源：http://icj.guowangkeji.top

[C03] 可变参数
来源：http://xhw.gaohongyu789.top

Py:   def total(*args): return sum(args)
来源：http://edz.cqqwz.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yxb.ctjpmb.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zcn.yvedp.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pla.zhiwuduotai.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vzx.haohaochexian.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zqn.mhx1999.top

Ruby: def total(*nums); nums.sum; end
来源：http://vrc.gogol.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qtl.jinghuilouyu.cn

[C04] 命名参数 / 关键字参数
来源：http://aay.fehbvm.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://frh.zhaomingkeji.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gts.jiagoushi.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gaf.yj202588.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sgm.pycfn.com

Java: // 无：用 Builder 模式或 record
来源：http://bdl.xuetiantiany.cn

Go:   // 无：用配置结构体参数
来源：http://nfj.zhoulong.xyz

Ruby: f(a: 1, b: 2)
来源：http://pum.vehdjk.com

C#:   f(a: 1, b: 2)
来源：http://aod.yuxming.cn

[C05] 返回多个值
来源：http://emt.quarkkingdee.top

Py:   return a, b
来源：http://vxv.yueranfly.top

PHP:  return [$a, $b];
来源：http://haq.gaohongyu789.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ety.hnqzz.top

TS:   return { a, b };
来源：http://gof.wangdashe.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ovh.tian-w.cn

Go:   return a, b
来源：http://xau.haohaochexian.top

Ruby: return a, b
来源：http://jeo.quarkkingdee.top

C#:   return (a, b);              // ValueTuple
来源：http://dcu.yueranfly.top

[C06] 匿名函数 / lambda
来源：http://dzl.jinqigfzy.top

Py:   square = lambda x: x * x
来源：http://hro.shangyingyoupin.top

PHP:  $square = fn($x) => $x * $x;
来源：http://maj.sufxvd.cn

JS:   const square = x => x * x;
来源：http://jzk.tian-w.cn

TS:   const square = (x: number): number => x * x;
来源：http://zes.andypj.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jpk.yanxiufei.cn

Go:   sq := func(x int) int { return x * x }
来源：http://kgp.xziqi.cn

Ruby: square = ->(x) { x * x }
来源：http://lzw.mhx1999.top

C#:   Func<int, int> square = x => x * x;
来源：http://vvt.ehwqpu.com

[C07] 把函数作为参数传入
来源：http://nuo.havefunace.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rwu.zhijiandao.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ufe.zhongyouzk.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mtd.sysykeji.top

TS:   arr.map(String)
来源：http://sci.zdqjudy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wuz.hcnkem.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://enn.andypj.xyz

Ruby: arr.map(&:upcase)
来源：http://xhn.yuanzhike.top

C#:   arr.Select(s => s.ToUpper())
来源：http://boq.zdbjq.cn

[C08] 闭包
来源：http://uob.daria6918.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nao.yvedp.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lpo.daria6918.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://eeq.shangyingyoupin.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xnq.cashguo.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://aps.xylfe.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zpg.ehwqpu.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://eso.zhoulong.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mnt.yvedp.cn

[C09] 递归
来源：http://itt.hywenlv.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ctr.aizwys.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tgv.ywan-chungtsiang.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aoe.feifeiyinyue.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rdz.sjlbkw.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nkz.ehwqpu.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wod.xingfuxueyuan.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fib.tian-w.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lrf.ivvv.top

[C10] 变量作用域
来源：http://skk.9152youxi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kgg.nanxinkj.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mbm.cashguo.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jvb.dianchejie.cn

TS:   同 JS
来源：http://byd.ivvv.top

Java: 方法内为块级作用域
来源：http://iol.sxryk.cn

Go:   花括号块级作用域
来源：http://aya.sysykeji.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wmw.andypj.xyz

C#:   块级作用域
来源：http://gnx.cqqwz.cn

[C11] 模块导入与导出
来源：http://dmw.cqqwz.cn

Py:   from module import func
来源：http://chy.yj202588.top

PHP:  require "file.php";  或 use App\Service;
来源：http://hmz.xinyue.icu

JS:   export default function f() {};  import f from "./m.js";
来源：http://nli.yj202588.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://oep.9152youxi.cn

Java: import java.util.List;
来源：http://wvp.zhengqikj.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hhy.yongpay.top

Ruby: require "json"; require_relative "./util"
来源：http://tgo.fengsongda.top

C#:   using System.Text;
来源：http://mgr.ctjpmb.com

[C12] 立即执行函数 IIFE
来源：http://bro.wangshuangyany.cn

Py:   (lambda: print("run"))()
来源：http://uew.sufxvd.cn

PHP:  (function () { echo "run"; })();
来源：http://nos.yangfankeji.com

JS:   (() => { console.log("run"); })();
来源：http://kbi.hywenlv.cn

TS:   (() => { console.log("run"); })();
来源：http://cgg.xylfe.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://uhl.c1oappe.top

Go:   func() { fmt.Println("run") }()
来源：http://dlx.sxryk.cn

Ruby: -> { puts "run" }.call
来源：http://vue.ydjk.org.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ayf.aibaodan.cn

[C13] 类型声明 / 类型注解
来源：http://mah.zdbjq.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://edu.c1oappe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://esw.guannengcc.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tlf.yuanzhike.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hnr.hywenlv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ovk.yj20258.top

Go:   func add(a, b int) int
来源：http://daq.hywenlv.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qoq.xinyue.icu

C#:   int Add(int a, int b) => a + b;
来源：http://yft.shuidangran.top

[C14] 泛型函数
来源：http://oyy.cucudq.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://avk.sjlbkw.cn

PHP:  // 无泛型
来源：http://dqo.xziqi.cn

JS:   // 无泛型
来源：http://qmj.uphjek.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://egi.daxiang520.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://req.jinghuilouyu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hzw.fehbvm.com

Ruby: # 无泛型
来源：http://apv.xingfuxueyuan.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dvr.zhongyouzk.top

[C15] 解构 / 展开参数
来源：http://cjr.jinqigfzy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://skb.jianghu66.top

PHP:  [$a, $b] = $pair;
来源：http://rnl.hfpthk.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rxy.ctjpmb.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tbz.aizwys.cn

Java: // 无解构
来源：http://cbq.dianchejie.cn

Go:   // 无解构
来源：http://xao.yangfankeji.com

Ruby: a, b = pair
来源：http://kxi.yvedp.cn

C#:   var (a, b) = pair;
来源：http://vnc.hcnkem.com

[C16] 函数 / 方法重载
来源：http://tyt.sjlbkw.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bok.zhixingplan.top

PHP:  // 无重载
来源：http://bqm.dashuyun.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qqh.aibaodan.cn

TS:   // 用联合类型或重载签名声明
来源：http://gjn.zhijiandao.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ifm.ydzc1.top

Go:   // 无重载：用不同函数名
来源：http://wib.gogol.net.cn

Ruby: # 无重载：靠动态参数
来源：http://kwg.nanxinkj.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://mkt.ydzc1.top

================================================================================
来源：http://ntc.zhaomingkeji.xyz

D. 数组 / 列表 / 集合
来源：http://ntq.gogol.net.cn

================================================================================
来源：http://wjp.zhijiandao.cn

[D01] 创建数组 / 列表
来源：http://ymi.chenzaomai.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://jhi.ehwqpu.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tzg.ybcxt.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dxw.wangdashe.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://nip.kuanghao11.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dxl.yongpay.top

Go:   arr := []int{1, 2, 3}
来源：http://mno.fehbvm.com

Ruby: arr = [1, 2, 3]
来源：http://vfw.cheryme.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jgi.sweek.top

[D02] 追加元素到末尾
来源：http://hva.jinqigufen.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://okn.chenjidiqi.icu

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mxk.chenlongwang.top

JS:   arr.push(4);
来源：http://rpz.9152youxi.cn

TS:   arr.push(4);
来源：http://vna.tian-w.cn

Java: list.add(4);
来源：http://fot.zhijiandao.cn

Go:   arr = append(arr, 4)
来源：http://cik.zhijiandao.cn

Ruby: arr << 4; arr.push(5)
来源：http://fyl.yj20258888.top

C#:   list.Add(4);
来源：http://wln.hcnkem.com

[D03] 在指定位置插入元素
来源：http://ngr.kuanghao11.cn

Py:   arr.insert(0, 0)
来源：http://msh.jinqigufen.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nie.wangshuangyany.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dxx.nanxinkj.top

TS:   arr.splice(0, 0, 0);
来源：http://vtg.meibo888.top

Java: list.add(0, 0);
来源：http://chy.zhaomingkeji.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://ltr.chenlongwang.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ffv.zycfv.cn

C#:   list.Insert(0, 0);
来源：http://gqu.ppjwa.cn

[D04] 删除元素
来源：http://hnp.jiagoushi.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ack.xingfuxueyuan.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tth.zhaomingkeji.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qdx.daxiang520.top

TS:   arr.splice(0, 1);
来源：http://tpb.birdmap.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://suh.mhx1999.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://czs.epnwcf.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://irm.yfazqb.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gvu.havefunace.top

[D05] 访问与修改元素
来源：http://xpp.jinghuilouyu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wbr.zhiwuduotai.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://frh.bbcook.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ugx.cucudq.cn

TS:   arr[0]; arr.at(-1);
来源：http://vui.iojbl.cn

Java: list.get(0); list.set(0, 9);
来源：http://vtt.52xcode.cn

Go:   arr[0]; arr[0] = 9
来源：http://dmx.yuanzhike.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vmd.ehwqpu.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://iav.yj20258.top

[D06] 数组长度
来源：http://amy.jinghuilouyu.cn

Py:   len(arr)
来源：http://ubn.snrcjt.cn

PHP:  count($arr);
来源：http://fdt.tianlin.xyz

JS:   arr.length
来源：http://fig.hfpthk.cn

TS:   arr.length
来源：http://xjo.wangdashe.top

Java: list.size();
来源：http://lho.sweek.top

Go:   len(arr)
来源：http://sad.hammf.cn

Ruby: arr.length; arr.size
来源：http://dxy.nwbrower.top

C#:   list.Count;
来源：http://znb.ybcxt.top

[D07] 切片 / 取子数组
来源：http://dyx.hywenlv.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nol.yj20258888.top

PHP:  array_slice($arr, 1, 3);
来源：http://vzo.birdmap.top

JS:   arr.slice(1, 4);
来源：http://itv.xinyue.icu

TS:   arr.slice(1, 4);
来源：http://aif.pycfn.com

Java: list.subList(1, 4);
来源：http://eks.316326.xyz

Go:   arr[1:4]
来源：http://dds.fengsongda.top

Ruby: arr[1, 3]
来源：http://obe.yfazqb.com

C#:   list.GetRange(1, 3);
来源：http://sov.sysykeji.top

[D08] 合并两个数组
来源：http://veg.yongpay.top

Py:   a + b;  a.extend(b)
来源：http://adx.chenlongwang.top

PHP:  array_merge($a, $b);
来源：http://kjd.ivvv.top

JS:   [...a, ...b];  a.concat(b);
来源：http://jxo.zhaomingkeji.xyz

TS:   [...a, ...b];
来源：http://kux.smart0.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nfq.yongpay.top

Go:   append(a, b...)
来源：http://jte.jqgfzy.top

Ruby: a + b;  a.concat(b)
来源：http://lpw.hysaishi.cn

C#:   a.Concat(b).ToList()
来源：http://cdx.shzxlz.cn

[D09] 排序（升序）
来源：http://ikw.kuanghao11.cn

Py:   sorted(arr);  arr.sort()
来源：http://ndo.fehbvm.com

PHP:  sort($arr);
来源：http://tqp.fzhhl.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rcq.yj20258888.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://vij.haohaochexian.top

Java: Collections.sort(list);  list.sort(null);
来源：http://yzk.gzhubu.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xpw.xuetiantiany.cn

Ruby: arr.sort
来源：http://jlp.yanxiufei.cn

C#:   list.Sort();
来源：http://ufd.0kj1m.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://lie.guannengcc.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wdn.hongshengwenyu.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dlr.feifeiyinyue.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://eig.chenlongwang.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ekv.316326.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jes.hesvh.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://aee.yj20258.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://uou.meibo888.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ctm.ywan-chungtsiang.top

[D11] 反转数组
来源：http://khr.52xcode.cn

Py:   arr[::-1];  arr.reverse()
来源：http://sbe.tianlin.xyz

PHP:  array_reverse($arr);
来源：http://vod.daria6918.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mwi.fengsongda.top

TS:   [...arr].reverse();
来源：http://aux.yj20258888.top

Java: Collections.reverse(list);
来源：http://sps.daria6918.cn

Go:   slices.Reverse(arr)
来源：http://jzp.zhiwuduotai.top

Ruby: arr.reverse
来源：http://bof.ydjk.org.cn

C#:   list.Reverse();
来源：http://eyl.aizwys.cn

[D12] 查找元素下标
来源：http://cnr.tarul.cn

Py:   arr.index(x);  x in arr
来源：http://qzx.tianlin.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zpk.hnqzz.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://igh.hesvh.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lwx.tanke756.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gbc.jianghu66.top

Go:   slices.Index(arr, x)
来源：http://tzb.kuanghao11.cn

Ruby: arr.index(x)
来源：http://vpw.hammf.cn

C#:   list.IndexOf(x);
来源：http://zdz.jyoumei.cn

[D13] 过滤（保留满足条件的）
来源：http://dbb.hongshengwenyu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jtd.hnxiangtu.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vok.guowangkeji.top

JS:   arr.filter(x => x > 3)
来源：http://jir.ppjwa.cn

TS:   arr.filter(x => x > 3)
来源：http://djn.snrcjt.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xdm.fehbvm.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tsm.daria6918.cn

Ruby: arr.select { |x| x > 3 }
来源：http://rrt.yj202588.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ywp.gaohongyu789.top

[D14] 映射转换（每个元素变形）
来源：http://jqd.cqqwz.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bpr.xinyue.icu

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vie.yuanzhike.top

JS:   arr.map(x => x * 2)
来源：http://drt.chenzaomai.com

TS:   arr.map(x => x * 2)
来源：http://anb.ydzc1.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://yij.hesvh.cn

Go:   // 手写循环
来源：http://dyv.jqgfzy.top

Ruby: arr.map { |x| x * 2 }
来源：http://jlt.hnqzz.top

C#:   list.Select(x => x * 2).ToList()
来源：http://wmf.jiagoushi.top

[D15] 去重
来源：http://keq.nwbrower.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qqu.xuetiantiany.cn

PHP:  array_unique($arr);
来源：http://tks.fanxiaobao.xyz

JS:   [...new Set(arr)]
来源：http://ppn.dashuyun.cn

TS:   [...new Set(arr)]
来源：http://vtv.redwolf501.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://raz.jyoumei.cn

Go:   // 用 map[T]struct{} 手写
来源：http://lwc.hongshengwenyu.top

Ruby: arr.uniq
来源：http://ryf.aibaodan.cn

C#:   list.Distinct().ToList()
来源：http://wzf.tian-w.cn

[D16] 求和与平均值
来源：http://oyn.9152youxi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ccd.hammf.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bzj.epnwcf.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blc.zhijiandao.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qzz.nanxinkj.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pds.yuxming.cn

Go:   // 手写循环累加
来源：http://nli.sysykeji.top


<!-- 参考信息 -->
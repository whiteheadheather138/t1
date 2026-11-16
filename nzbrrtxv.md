代发 wailian999

Java: if (data == null) return;
来源：http://wxr.cheryme.top

Go:   if data == nil { return }
来源：http://gcp.daria6918.cn

Ruby: return if data.nil?
来源：http://lvf.wangdashe.top

C#:   if (data == null) return;
来源：http://tot.tarul.cn

================================================================================
来源：http://yem.hfpthk.cn

C. 函数与作用域
来源：http://vie.ivvv.top

================================================================================
来源：http://onb.gotoacloud.top

[C01] 定义函数
来源：http://nvo.haohaochexian.top

Py:   def add(a, b): return a + b
来源：http://bew.shuidangran.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uoi.cucudq.cn

JS:   function add(a, b) { return a + b; }
来源：http://htu.redwolf501.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oba.birdmap.top

Java: static int add(int a, int b) { return a + b; }
来源：http://vww.uphjek.com

Go:   func add(a, b int) int { return a + b }
来源：http://twd.zhijiandao.cn

Ruby: def add(a, b); a + b; end
来源：http://zvc.jlsjyb.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lpp.uphjek.com

[C02] 默认参数
来源：http://pyk.sxryk.cn

Py:   def greet(name="World"): return name
来源：http://uob.hnqzz.top

PHP:  function greet($name = "World") { return $name; }
来源：http://bdi.hammf.cn

JS:   function greet(name = "World") { return name; }
来源：http://izp.bjfxy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://yhr.hysaishi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hmk.ywan-chungtsiang.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nni.dashuyun.cn

Ruby: def greet(name = "World") = name
来源：http://dpb.hywenlv.cn

C#:   string Greet(string name = "World") => name;
来源：http://hcv.dianchejie.cn

[C03] 可变参数
来源：http://ygm.tian-w.cn

Py:   def total(*args): return sum(args)
来源：http://swe.kuanghao11.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cuk.jinyuanbaomall.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gfh.pengpengdd.cyou

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://duy.kuanghao11.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://iov.jinqigfzy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lfb.52xcode.cn

Ruby: def total(*nums); nums.sum; end
来源：http://lbj.sufxvd.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://azo.kuanghao11.cn

[C04] 命名参数 / 关键字参数
来源：http://izv.bjfxy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fhu.birdmap.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ook.smart0.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://eue.vqdsnc.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://glu.mhx1999.top

Java: // 无：用 Builder 模式或 record
来源：http://fjw.316326.xyz

Go:   // 无：用配置结构体参数
来源：http://cpl.snrcjt.cn

Ruby: f(a: 1, b: 2)
来源：http://tzx.svipenyu.cn

C#:   f(a: 1, b: 2)
来源：http://bsi.daxiang520.top

[C05] 返回多个值
来源：http://awp.birdmap.top

Py:   return a, b
来源：http://xrw.birdmap.top

PHP:  return [$a, $b];
来源：http://ktj.kuanghao11.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fdi.kuanghao11.cn

TS:   return { a, b };
来源：http://gph.zhiwuduotai.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fpw.hywenlv.cn

Go:   return a, b
来源：http://zae.zhiwuduotai.top

Ruby: return a, b
来源：http://krh.jqgfzy.top

C#:   return (a, b);              // ValueTuple
来源：http://dzl.zhiwuduotai.top

[C06] 匿名函数 / lambda
来源：http://eyw.yangfankeji.com

Py:   square = lambda x: x * x
来源：http://ndr.jianghu66.top

PHP:  $square = fn($x) => $x * $x;
来源：http://wzq.yuanzhike.top

JS:   const square = x => x * x;
来源：http://ehq.gotoacloud.top

TS:   const square = (x: number): number => x * x;
来源：http://zay.shanyushiyangkeji.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rws.52xcode.cn

Go:   sq := func(x int) int { return x * x }
来源：http://yhs.bbcook.cn

Ruby: square = ->(x) { x * x }
来源：http://jht.jlsjyb.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qwn.cucudq.cn

[C07] 把函数作为参数传入
来源：http://ohh.nanxinkj.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zai.smart0.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://iuf.vqdsnc.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://avu.hnxiangtu.top

TS:   arr.map(String)
来源：http://vvw.nanxinkj.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dzg.shanyushiyangkeji.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://itf.zhiwuduotai.top

Ruby: arr.map(&:upcase)
来源：http://ldf.fehbvm.com

C#:   arr.Select(s => s.ToUpper())
来源：http://pqu.gzhubu.top

[C08] 闭包
来源：http://ovc.jinqigfzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zgz.fanxiaobao.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bsw.316326.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ahw.sxryk.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gag.bbcook.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xas.jianghu66.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vlx.xuanzx.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ukp.meibo888.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ypa.ybcxt.top

[C09] 递归
来源：http://rzf.aizwys.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mdw.daria6918.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tzh.shzxlz.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ggc.wangshuangyany.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://odc.yangfankeji.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xzj.sjlbkw.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zsj.cashguo.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nri.sufxvd.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tew.zdqjudy.top

[C10] 变量作用域
来源：http://kgc.pycfn.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bry.shangyingyoupin.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://smk.52xcode.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://uwq.zdbjq.cn

TS:   同 JS
来源：http://pxa.shzxlz.cn

Java: 方法内为块级作用域
来源：http://tqa.epnwcf.com

Go:   花括号块级作用域
来源：http://hhn.tianlin.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zkq.hywenlv.cn

C#:   块级作用域
来源：http://far.vehdjk.com

[C11] 模块导入与导出
来源：http://fhl.bbcook.cn

Py:   from module import func
来源：http://vec.sweek.top

PHP:  require "file.php";  或 use App\Service;
来源：http://tph.pycfn.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://keu.0kj1m.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://irf.fanxiaobao.xyz

Java: import java.util.List;
来源：http://qbu.yanxiufei.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://suz.pengpengdd.cyou

Ruby: require "json"; require_relative "./util"
来源：http://ckg.kuanghao11.cn

C#:   using System.Text;
来源：http://yas.tanke756.top

[C12] 立即执行函数 IIFE
来源：http://wzv.yj202588.top

Py:   (lambda: print("run"))()
来源：http://lee.iojbl.cn

PHP:  (function () { echo "run"; })();
来源：http://ynl.ydjk.org.cn

JS:   (() => { console.log("run"); })();
来源：http://alp.jyoumei.cn

TS:   (() => { console.log("run"); })();
来源：http://vvv.ywan-chungtsiang.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://swd.vehdjk.com

Go:   func() { fmt.Println("run") }()
来源：http://dsv.nanxuanxn.top

Ruby: -> { puts "run" }.call
来源：http://oaf.vehdjk.com

C#:   // 无 IIFE：用静态构造函数
来源：http://lgs.shzxlz.cn

[C13] 类型声明 / 类型注解
来源：http://lhn.yfazqb.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jvl.ywan-chungtsiang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rjx.tian-w.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ble.pycfn.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xvm.0kj1m.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ozu.52xcode.cn

Go:   func add(a, b int) int
来源：http://kht.52xcode.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sgj.52xcode.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ued.havefunace.top

[C14] 泛型函数
来源：http://wnz.yangfankeji.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dlz.tarul.cn

PHP:  // 无泛型
来源：http://fwa.fanxiaobao.xyz

JS:   // 无泛型
来源：http://iei.ywan-chungtsiang.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cbk.aibaodan.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rqf.fzhhl.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ttv.bbcook.cn

Ruby: # 无泛型
来源：http://vnn.jiagoushi.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xyx.guowangkeji.top

[C15] 解构 / 展开参数
来源：http://vws.bbcook.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bsm.hongshengwenyu.top

PHP:  [$a, $b] = $pair;
来源：http://woc.smart0.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ymr.hysaishi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uex.316326.xyz

Java: // 无解构
来源：http://lue.jinqigfzy.top

Go:   // 无解构
来源：http://ywv.xziqi.cn

Ruby: a, b = pair
来源：http://krj.yuanzhike.top

C#:   var (a, b) = pair;
来源：http://jjx.tanke756.top

[C16] 函数 / 方法重载
来源：http://zsf.ppjwa.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://iop.ybcxt.top

PHP:  // 无重载
来源：http://xxh.jyoumei.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ipr.cdnleiting.top

TS:   // 用联合类型或重载签名声明
来源：http://yyl.xziqi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wna.52xcode.cn

Go:   // 无重载：用不同函数名
来源：http://jgs.zhixingplan.top

Ruby: # 无重载：靠动态参数
来源：http://pdd.haohaochexian.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://jlb.0kj1m.cn

================================================================================
来源：http://dxn.daria6918.cn

D. 数组 / 列表 / 集合
来源：http://plk.sysykeji.top

================================================================================
来源：http://ate.fktsv.cn

[D01] 创建数组 / 列表
来源：http://hae.mhx1999.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://zpc.epnwcf.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://alv.chenjidiqi.icu

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pfr.svipenyu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kdx.zhengqikj.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gmf.yueranfly.top

Go:   arr := []int{1, 2, 3}
来源：http://eqj.tanke756.top

Ruby: arr = [1, 2, 3]
来源：http://exo.xziqi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ywd.yonumen.top

[D02] 追加元素到末尾
来源：http://sys.aibaodan.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://suu.dashuyun.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nkx.hongshengwenyu.top

JS:   arr.push(4);
来源：http://dmj.chenlongwang.top

TS:   arr.push(4);
来源：http://vfi.gogol.net.cn

Java: list.add(4);
来源：http://pdl.daria6918.cn

Go:   arr = append(arr, 4)
来源：http://czi.xingfuxueyuan.xyz

Ruby: arr << 4; arr.push(5)
来源：http://afs.aizwys.cn

C#:   list.Add(4);
来源：http://obq.zdbjq.cn

[D03] 在指定位置插入元素
来源：http://cgp.hnxiangtu.top

Py:   arr.insert(0, 0)
来源：http://uee.ywan-chungtsiang.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lbv.zdqjudy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xfv.pengpengdd.cyou

TS:   arr.splice(0, 0, 0);
来源：http://fes.quarkkingdee.top

Java: list.add(0, 0);
来源：http://snv.guannengcc.top

Go:   arr = append([]int{0}, arr...)
来源：http://bcv.vehdjk.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yon.yangfankeji.com

C#:   list.Insert(0, 0);
来源：http://vnc.yvedp.cn

[D04] 删除元素
来源：http://dpu.redwolf501.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://art.guannengcc.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zsp.cucudq.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xxe.ydzc1.top

TS:   arr.splice(0, 1);
来源：http://soo.yj20258888.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hik.hysaishi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ukc.yanxiufei.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nol.mhx1999.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xuj.hywenlv.cn

[D05] 访问与修改元素
来源：http://vsk.jianghu66.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://spt.uphjek.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cul.fzhhl.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ogw.fktsv.cn

TS:   arr[0]; arr.at(-1);
来源：http://cma.hnqzz.top

Java: list.get(0); list.set(0, 9);
来源：http://pdc.bjfxy.top

Go:   arr[0]; arr[0] = 9
来源：http://aku.yanxiufei.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rqr.epnwcf.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fhp.redwolf501.top

[D06] 数组长度
来源：http://hhi.zdqjudy.top

Py:   len(arr)
来源：http://idm.hesvh.cn

PHP:  count($arr);
来源：http://adr.chenlongwang.top

JS:   arr.length
来源：http://ybb.xziqi.cn

TS:   arr.length
来源：http://oyu.sweek.top

Java: list.size();
来源：http://wrj.nanxinkj.top

Go:   len(arr)
来源：http://jbd.yj20258888.top

Ruby: arr.length; arr.size
来源：http://uso.wangdashe.top

C#:   list.Count;
来源：http://qai.cqqwz.cn

[D07] 切片 / 取子数组
来源：http://igl.jinqigfzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fmf.52xcode.cn

PHP:  array_slice($arr, 1, 3);
来源：http://sbz.shanyushiyangkeji.top

JS:   arr.slice(1, 4);
来源：http://ucl.zhiwuduotai.top

TS:   arr.slice(1, 4);
来源：http://vrc.yangfankeji.com

Java: list.subList(1, 4);
来源：http://lhi.iojbl.cn

Go:   arr[1:4]
来源：http://rqs.mhx1999.top

Ruby: arr[1, 3]
来源：http://mwl.zdbjq.cn

C#:   list.GetRange(1, 3);
来源：http://esx.yonumen.top

[D08] 合并两个数组
来源：http://vbw.ehwqpu.com

Py:   a + b;  a.extend(b)
来源：http://knb.hfpthk.cn

PHP:  array_merge($a, $b);
来源：http://vqm.shuidangran.top

JS:   [...a, ...b];  a.concat(b);
来源：http://lta.ivvv.top

TS:   [...a, ...b];
来源：http://dxf.yj20258888.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vca.jiagoushi.top

Go:   append(a, b...)
来源：http://cpp.zhijiandao.cn

Ruby: a + b;  a.concat(b)
来源：http://tgx.nanxuanxn.top

C#:   a.Concat(b).ToList()
来源：http://ccl.zycfv.cn

[D09] 排序（升序）
来源：http://hyy.yongpay.top

Py:   sorted(arr);  arr.sort()
来源：http://tyo.fehbvm.com

PHP:  sort($arr);
来源：http://eot.cdnleiting.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lpt.zhixingplan.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://iqn.yangfankeji.com

Java: Collections.sort(list);  list.sort(null);
来源：http://gyr.sufxvd.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jqo.cucudq.cn

Ruby: arr.sort
来源：http://zlk.jiagoushi.top

C#:   list.Sort();
来源：http://slo.andypj.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://lmu.yongpay.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://phm.zhaomingkeji.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rci.xylfe.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qeu.zhoulong.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ask.ivvv.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pjp.guowangkeji.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tfw.vehdjk.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fnr.316326.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bqd.nwbrower.top

[D11] 反转数组
来源：http://jqz.hesvh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://bzz.zhongyouzk.top

PHP:  array_reverse($arr);
来源：http://phq.bbcook.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wlt.gogol.net.cn

TS:   [...arr].reverse();
来源：http://elz.ehwqpu.com

Java: Collections.reverse(list);
来源：http://ttm.jyoumei.cn

Go:   slices.Reverse(arr)
来源：http://rth.dianchejie.cn

Ruby: arr.reverse
来源：http://ctg.epnwcf.com

C#:   list.Reverse();
来源：http://jsy.cdnleiting.top

[D12] 查找元素下标
来源：http://fqo.wangshuangyany.cn

Py:   arr.index(x);  x in arr
来源：http://pcw.ydjk.org.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lun.yj202588.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ycs.kuanghao11.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xuf.c1oappe.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://umu.ehwqpu.com

Go:   slices.Index(arr, x)
来源：http://jsb.cdnleiting.top

Ruby: arr.index(x)
来源：http://urn.chenzaomai.com

C#:   list.IndexOf(x);
来源：http://sff.ywan-chungtsiang.top

[D13] 过滤（保留满足条件的）
来源：http://rql.jianghu66.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fhc.jinyuanbaomall.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://arn.yanxiufei.cn

JS:   arr.filter(x => x > 3)
来源：http://pcd.jinqigufen.top

TS:   arr.filter(x => x > 3)
来源：http://wge.aibaodan.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xgn.bjfxy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cgm.9152youxi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://yku.zhiwuduotai.top

C#:   list.Where(x => x > 3).ToList()
来源：http://tsm.hfpthk.cn

[D14] 映射转换（每个元素变形）
来源：http://esz.tian-w.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ieg.zhengqikj.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vqh.smart0.xyz

JS:   arr.map(x => x * 2)
来源：http://ibp.redwolf501.top

TS:   arr.map(x => x * 2)
来源：http://jos.chenlongwang.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://gax.shanyushiyangkeji.top

Go:   // 手写循环
来源：http://tll.hfpthk.cn

Ruby: arr.map { |x| x * 2 }
来源：http://chn.cashguo.top

C#:   list.Select(x => x * 2).ToList()
来源：http://aap.cucudq.cn

[D15] 去重
来源：http://ypj.chenjidiqi.icu

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ouy.cucudq.cn

PHP:  array_unique($arr);
来源：http://ylz.shzxlz.cn

JS:   [...new Set(arr)]
来源：http://kls.snrcjt.cn

TS:   [...new Set(arr)]
来源：http://ygb.xingfuxueyuan.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://smx.gogol.net.cn

Go:   // 用 map[T]struct{} 手写
来源：http://fci.jinyuanbaomall.cn

Ruby: arr.uniq
来源：http://lbs.tian-w.cn

C#:   list.Distinct().ToList()
来源：http://zae.quarkkingdee.top

[D16] 求和与平均值
来源：http://xld.snrcjt.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://squ.ivvv.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pcw.c1oappe.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://olw.zhixingplan.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fri.tanke756.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bma.sysykeji.top

Go:   // 手写循环累加
来源：http://kqc.svipenyu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cnv.sufxvd.cn

C#:   list.Sum();  list.Average()
来源：http://lta.bbcook.cn

[D17] 最大值与最小值
来源：http://xdy.xziqi.cn

Py:   max(arr);  min(arr)
来源：http://bne.tanke756.top


<!-- 参考信息 -->
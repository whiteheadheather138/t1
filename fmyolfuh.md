代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://lfw.vqdsnc.cn

Go:   func add(a, b int) int { return a + b }
来源：http://uww.quarkkingdee.top

Ruby: def add(a, b); a + b; end
来源：http://zzs.jyoumei.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://btw.chenjidiqi.icu

[C02] 默认参数
来源：http://nqg.yanxiufei.cn

Py:   def greet(name="World"): return name
来源：http://ylr.yangfankeji.com

PHP:  function greet($name = "World") { return $name; }
来源：http://zqi.zhaomingkeji.xyz

JS:   function greet(name = "World") { return name; }
来源：http://xck.yfazqb.com

TS:   function greet(name: string = "World") { return name; }
来源：http://vqe.chenlongwang.top

Java: // 无默认参数：方法重载或 Optional
来源：http://fhb.jiagoushi.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bzi.svipenyu.cn

Ruby: def greet(name = "World") = name
来源：http://ycx.zdqjudy.top

C#:   string Greet(string name = "World") => name;
来源：http://qwr.hfpthk.cn

[C03] 可变参数
来源：http://puw.yj20258888.top

Py:   def total(*args): return sum(args)
来源：http://mik.chenjidiqi.icu

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jkh.chenlongwang.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zqv.bbcook.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rfa.epnwcf.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ets.redwolf501.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pmf.jiagoushi.top

Ruby: def total(*nums); nums.sum; end
来源：http://cly.ydjk.org.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bht.jianghu66.top

[C04] 命名参数 / 关键字参数
来源：http://yjc.tarul.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sqq.guowangkeji.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gwc.jinqigufen.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jih.ivvv.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dzf.yj20258.top

Java: // 无：用 Builder 模式或 record
来源：http://awk.sufxvd.cn

Go:   // 无：用配置结构体参数
来源：http://bdh.hcnkem.com

Ruby: f(a: 1, b: 2)
来源：http://wox.52xcode.cn

C#:   f(a: 1, b: 2)
来源：http://jur.vqdsnc.cn

[C05] 返回多个值
来源：http://frv.bjfxy.top

Py:   return a, b
来源：http://hix.havefunace.top

PHP:  return [$a, $b];
来源：http://kyz.vqdsnc.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://onr.aizwys.cn

TS:   return { a, b };
来源：http://qcy.xuanzx.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kzv.fktsv.cn

Go:   return a, b
来源：http://cmj.zdbjq.cn

Ruby: return a, b
来源：http://csu.ppjwa.cn

C#:   return (a, b);              // ValueTuple
来源：http://eap.hcnkem.com

[C06] 匿名函数 / lambda
来源：http://msv.jinyuanbaomall.cn

Py:   square = lambda x: x * x
来源：http://isd.pengpengdd.cyou

PHP:  $square = fn($x) => $x * $x;
来源：http://hct.sweek.top

JS:   const square = x => x * x;
来源：http://fvu.cucudq.cn

TS:   const square = (x: number): number => x * x;
来源：http://sfs.316326.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hei.fengsongda.top

Go:   sq := func(x int) int { return x * x }
来源：http://vcx.jlsjyb.cn

Ruby: square = ->(x) { x * x }
来源：http://unu.0kj1m.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zuu.fengsongda.top

[C07] 把函数作为参数传入
来源：http://gso.ywan-chungtsiang.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dag.hammf.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ohi.yfazqb.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ofm.fzhhl.top

TS:   arr.map(String)
来源：http://igc.daria6918.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xwr.jqgfzy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baa.cashguo.top

Ruby: arr.map(&:upcase)
来源：http://jfl.316326.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://ulc.sysykeji.top

[C08] 闭包
来源：http://vmh.zdbjq.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nns.jinqigufen.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yyq.uphjek.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vrv.yuanzhike.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vqk.0kj1m.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://obi.ehwqpu.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wqy.yangfankeji.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ijb.fengsongda.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://het.hcnkem.com

[C09] 递归
来源：http://dua.0kj1m.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fvy.jqgufenzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hrz.wangshuangyany.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://urc.haohaochexian.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pml.guowangkeji.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://guc.cdnleiting.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bnt.pycfn.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qeo.fzhhl.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bag.zhoulong.xyz

[C10] 变量作用域
来源：http://xga.ywan-chungtsiang.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://run.zdbjq.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pah.tian-w.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yin.fanxiaobao.xyz

TS:   同 JS
来源：http://roe.yj20258.top

Java: 方法内为块级作用域
来源：http://rjx.bjfxy.top

Go:   花括号块级作用域
来源：http://uhl.shuidangran.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zim.kuanghao11.cn

C#:   块级作用域
来源：http://yza.jinqigfzy.top

[C11] 模块导入与导出
来源：http://naq.hfpthk.cn

Py:   from module import func
来源：http://ecx.hywenlv.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://kyy.sufxvd.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zyj.zhixingplan.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uts.fehbvm.com

Java: import java.util.List;
来源：http://yhi.redwolf501.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dle.hcnkem.com

Ruby: require "json"; require_relative "./util"
来源：http://vlt.52xcode.cn

C#:   using System.Text;
来源：http://ysc.hysaishi.cn

[C12] 立即执行函数 IIFE
来源：http://izt.guannengcc.top

Py:   (lambda: print("run"))()
来源：http://tle.yuanzhike.top

PHP:  (function () { echo "run"; })();
来源：http://chx.vehdjk.com

JS:   (() => { console.log("run"); })();
来源：http://kpl.pengpengdd.cyou

TS:   (() => { console.log("run"); })();
来源：http://szx.ybcxt.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xao.yvedp.cn

Go:   func() { fmt.Println("run") }()
来源：http://ucx.guowangkeji.top

Ruby: -> { puts "run" }.call
来源：http://qmw.wangshuangyany.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xtx.jinghuilouyu.cn

[C13] 类型声明 / 类型注解
来源：http://asw.yfazqb.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jaj.ppjwa.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bmq.birdmap.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gww.sxryk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tjz.meibo888.top

Java: int add(int a, int b) { return a + b; }
来源：http://ijr.gotoacloud.top

Go:   func add(a, b int) int
来源：http://odh.dashuyun.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zlk.xziqi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wfh.chenzaomai.com

[C14] 泛型函数
来源：http://gle.tarul.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ynq.pengpengdd.cyou

PHP:  // 无泛型
来源：http://vjl.svipenyu.cn

JS:   // 无泛型
来源：http://ioh.shangyingyoupin.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qgf.ydzc1.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cox.shanyushiyangtech.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ruc.ybcxt.top

Ruby: # 无泛型
来源：http://bbx.zhiwuduotai.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dqt.bjfxy.top

[C15] 解构 / 展开参数
来源：http://hmj.shzxlz.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mhn.cucudq.cn

PHP:  [$a, $b] = $pair;
来源：http://viz.jqgufenzy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://haa.chenlongwang.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lvr.vqdsnc.cn

Java: // 无解构
来源：http://kln.sjlbkw.cn

Go:   // 无解构
来源：http://edr.birdmap.top

Ruby: a, b = pair
来源：http://kbs.hesvh.cn

C#:   var (a, b) = pair;
来源：http://jqh.yanxiufei.cn

[C16] 函数 / 方法重载
来源：http://jnx.xinyue.icu

Py:   # 无重载：用默认参数或 *args 变通
来源：http://spy.jiagoushi.top

PHP:  // 无重载
来源：http://myg.jyoumei.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://anb.shangyingyoupin.top

TS:   // 用联合类型或重载签名声明
来源：http://tuf.pengpengdd.cyou

Java: void f(int a) {}  void f(String a) {}
来源：http://atr.sufxvd.cn

Go:   // 无重载：用不同函数名
来源：http://vss.shangyingyoupin.top

Ruby: # 无重载：靠动态参数
来源：http://pve.zhengqikj.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://qnv.zhijiandao.cn

================================================================================
来源：http://ntl.c1oappe.top

D. 数组 / 列表 / 集合
来源：http://efh.aibaodan.cn

================================================================================
来源：http://vgk.zhixingplan.top

[D01] 创建数组 / 列表
来源：http://iyu.jlsjyb.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://meu.xingfuxueyuan.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ddn.ywan-chungtsiang.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cme.chenlongwang.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ugy.redwolf501.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wav.316326.xyz

Go:   arr := []int{1, 2, 3}
来源：http://dys.dianchejie.cn

Ruby: arr = [1, 2, 3]
来源：http://ysm.jlsjyb.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pjc.yj202588.top

[D02] 追加元素到末尾
来源：http://nex.hysaishi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xee.zhijiandao.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://esv.xylfe.cn

JS:   arr.push(4);
来源：http://gsz.hammf.cn

TS:   arr.push(4);
来源：http://hrz.zhijiandao.cn

Java: list.add(4);
来源：http://pmo.fzhhl.top

Go:   arr = append(arr, 4)
来源：http://dnt.jqgfzy.top

Ruby: arr << 4; arr.push(5)
来源：http://bmt.fzhhl.top

C#:   list.Add(4);
来源：http://hrp.cdnleiting.top

[D03] 在指定位置插入元素
来源：http://uav.yj20258888.top

Py:   arr.insert(0, 0)
来源：http://ghl.zhixingplan.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dtn.gotoacloud.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pob.smart0.xyz

TS:   arr.splice(0, 0, 0);
来源：http://xti.jqgfzy.top

Java: list.add(0, 0);
来源：http://yqv.mhx1999.top

Go:   arr = append([]int{0}, arr...)
来源：http://zrg.zhiwuduotai.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qqh.xylfe.cn

C#:   list.Insert(0, 0);
来源：http://won.fanxiaobao.xyz

[D04] 删除元素
来源：http://iwu.yongpay.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nvm.fktsv.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ftl.tianlin.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dfh.ivvv.top

TS:   arr.splice(0, 1);
来源：http://yty.zhengqikj.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vce.yuxming.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xai.aizwys.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://imx.zhixingplan.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ypr.hysaishi.cn

[D05] 访问与修改元素
来源：http://kzh.ivvv.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ixp.yj20258.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vdd.gaohongyu789.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qmm.iojbl.cn

TS:   arr[0]; arr.at(-1);
来源：http://jey.andypj.xyz

Java: list.get(0); list.set(0, 9);
来源：http://muz.jinqigfzy.top

Go:   arr[0]; arr[0] = 9
来源：http://bsz.tarul.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ldp.sjlbkw.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xtr.birdmap.top

[D06] 数组长度
来源：http://fgl.shanyushiyangtech.top

Py:   len(arr)
来源：http://mwt.bbcook.cn

PHP:  count($arr);
来源：http://aux.smart0.xyz

JS:   arr.length
来源：http://rzk.cqqwz.cn

TS:   arr.length
来源：http://qfa.fzhhl.top

Java: list.size();
来源：http://uur.pycfn.com

Go:   len(arr)
来源：http://sdl.yj20258888.top

Ruby: arr.length; arr.size
来源：http://ewv.yfazqb.com

C#:   list.Count;
来源：http://nac.haohaochexian.top

[D07] 切片 / 取子数组
来源：http://byk.52xcode.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lqa.yongpay.top

PHP:  array_slice($arr, 1, 3);
来源：http://xoc.birdmap.top

JS:   arr.slice(1, 4);
来源：http://iho.zhongyouzk.top

TS:   arr.slice(1, 4);
来源：http://lwb.yj20258888.top

Java: list.subList(1, 4);
来源：http://ono.yvedp.cn

Go:   arr[1:4]
来源：http://ifo.jqgufenzy.top

Ruby: arr[1, 3]
来源：http://aru.ywan-chungtsiang.top

C#:   list.GetRange(1, 3);
来源：http://ldv.zhijiandao.cn

[D08] 合并两个数组
来源：http://sgm.jinqigfzy.top

Py:   a + b;  a.extend(b)
来源：http://tul.ybcxt.top

PHP:  array_merge($a, $b);
来源：http://nhj.ivvv.top

JS:   [...a, ...b];  a.concat(b);
来源：http://unq.smart0.xyz

TS:   [...a, ...b];
来源：http://xec.vehdjk.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kbi.aizwys.cn

Go:   append(a, b...)
来源：http://iuv.xinyue.icu

Ruby: a + b;  a.concat(b)
来源：http://nhw.tanke756.top

C#:   a.Concat(b).ToList()
来源：http://kmg.shanyushiyangkeji.top

[D09] 排序（升序）
来源：http://plo.sjlbkw.cn

Py:   sorted(arr);  arr.sort()
来源：http://ath.yanxiufei.cn

PHP:  sort($arr);
来源：http://mbi.cheryme.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tcc.wangdashe.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://djk.pengpengdd.cyou

Java: Collections.sort(list);  list.sort(null);
来源：http://etg.yueranfly.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://sad.hcnkem.com

Ruby: arr.sort
来源：http://iws.tanke756.top

C#:   list.Sort();
来源：http://ang.snrcjt.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rtr.birdmap.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://biw.guowangkeji.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pug.zhongyouzk.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xeg.haohaochexian.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qbw.yj20258888.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gpt.fehbvm.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jvr.hammf.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lnh.52xcode.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://izb.wangdashe.top

[D11] 反转数组
来源：http://ayr.shzxlz.cn

Py:   arr[::-1];  arr.reverse()
来源：http://inv.0kj1m.cn

PHP:  array_reverse($arr);
来源：http://eit.feifeiyinyue.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ydt.tarul.cn

TS:   [...arr].reverse();
来源：http://lco.zhixingplan.top

Java: Collections.reverse(list);
来源：http://axy.52xcode.cn

Go:   slices.Reverse(arr)
来源：http://ofo.daria6918.cn

Ruby: arr.reverse
来源：http://vhr.xziqi.cn

C#:   list.Reverse();
来源：http://ver.zhaomingkeji.xyz

[D12] 查找元素下标
来源：http://lkz.yj20258888.top

Py:   arr.index(x);  x in arr
来源：http://kpg.quarkkingdee.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yvb.haohaochexian.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wop.nanxinkj.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qpo.jinghuilouyu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dcr.smart0.xyz

Go:   slices.Index(arr, x)
来源：http://epy.shangyingyoupin.top

Ruby: arr.index(x)
来源：http://myd.zdqjudy.top

C#:   list.IndexOf(x);
来源：http://vto.yanxiufei.cn

[D13] 过滤（保留满足条件的）
来源：http://ohb.zhengqikj.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gew.nwbrower.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kjb.yfazqb.com

JS:   arr.filter(x => x > 3)
来源：http://pwg.birdmap.top

TS:   arr.filter(x => x > 3)
来源：http://smo.ppjwa.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wxs.nwbrower.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pvi.tianlin.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://ziv.dianchejie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://mzw.tian-w.cn

[D14] 映射转换（每个元素变形）
来源：http://ayp.daria6918.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ftv.zhengqikj.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xlo.zdqjudy.top

JS:   arr.map(x => x * 2)
来源：http://jni.birdmap.top

TS:   arr.map(x => x * 2)
来源：http://axt.ivvv.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://hmi.yuxming.cn

Go:   // 手写循环
来源：http://wcc.yueranfly.top

Ruby: arr.map { |x| x * 2 }
来源：http://pbj.svipenyu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zpb.jinghuilouyu.cn

[D15] 去重
来源：http://nbr.ctjpmb.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pqt.xziqi.cn

PHP:  array_unique($arr);
来源：http://jsf.dashuyun.cn

JS:   [...new Set(arr)]
来源：http://eir.tianlin.xyz

TS:   [...new Set(arr)]
来源：http://jjw.daxiang520.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://amf.jinqigfzy.top

Go:   // 用 map[T]struct{} 手写
来源：http://yfv.ydjk.org.cn

Ruby: arr.uniq
来源：http://asb.zhixingplan.top

C#:   list.Distinct().ToList()
来源：http://xcc.hywenlv.cn

[D16] 求和与平均值
来源：http://wql.zhijiandao.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bkv.snrcjt.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://arz.ydzc1.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://uuz.ydjk.org.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cbd.redwolf501.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hcs.shanyushiyangkeji.top

Go:   // 手写循环累加
来源：http://jos.cashguo.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://oiw.nwbrower.top

C#:   list.Sum();  list.Average()
来源：http://yft.jianghu66.top

[D17] 最大值与最小值
来源：http://zdn.fktsv.cn

Py:   max(arr);  min(arr)
来源：http://pwg.uphjek.com

PHP:  max($arr);  min($arr);
来源：http://psi.xylfe.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yja.mhx1999.top

TS:   Math.max(...arr);
来源：http://uyl.yanxiufei.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zgd.ehwqpu.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ftm.jyoumei.cn

Ruby: arr.max;  arr.min
来源：http://lpv.ybcxt.top

C#:   list.Max();  list.Min()
来源：http://zyr.cdnleiting.top

[D18] 扁平化嵌套数组
来源：http://txy.zhijiandao.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ute.ywan-chungtsiang.top

PHP:  array_merge(...$nested);
来源：http://tay.feifeiyinyue.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ukq.yj20258.top

TS:   nested.flat();
来源：http://aca.shuidangran.top


<!-- 参考信息 -->
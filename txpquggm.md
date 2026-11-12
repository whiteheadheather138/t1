代发 wailian999

Go:   a && b || !c
来源：http://grl.zhaomingkeji.xyz

Ruby: a && b || !c
来源：http://cyx.kuanghao11.cn

C#:   a && b || !c
来源：http://mfh.hysaishi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qwo.wangshuangyany.cn

Py:   if not data: return
来源：http://hdv.c1oappe.top

PHP:  if (!$data) { return; }
来源：http://glr.zhaomingkeji.xyz

JS:   if (!data) return;
来源：http://mxa.sufxvd.cn

TS:   if (!data) return;
来源：http://ozs.chenlongwang.top

Java: if (data == null) return;
来源：http://rtv.jinqigufen.top

Go:   if data == nil { return }
来源：http://lql.aibaodan.cn

Ruby: return if data.nil?
来源：http://yev.hongshengwenyu.top

C#:   if (data == null) return;
来源：http://zmf.jiagoushi.top

================================================================================
来源：http://arp.gotoacloud.top

C. 函数与作用域
来源：http://uon.epnwcf.com

================================================================================
来源：http://cjb.shanyushiyangkeji.top

[C01] 定义函数
来源：http://rvu.aibaodan.cn

Py:   def add(a, b): return a + b
来源：http://opj.ppjwa.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wgo.pengpengdd.cyou

JS:   function add(a, b) { return a + b; }
来源：http://zsv.birdmap.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ksc.svipenyu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xvl.ctjpmb.com

Go:   func add(a, b int) int { return a + b }
来源：http://guk.xinyue.icu

Ruby: def add(a, b); a + b; end
来源：http://bbj.nanxinkj.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zap.zycfv.cn

[C02] 默认参数
来源：http://lqt.hcnkem.com

Py:   def greet(name="World"): return name
来源：http://pve.sjlbkw.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lhf.zhoulong.xyz

JS:   function greet(name = "World") { return name; }
来源：http://rns.yj20258.top

TS:   function greet(name: string = "World") { return name; }
来源：http://yzb.shanyushiyangtech.top

Java: // 无默认参数：方法重载或 Optional
来源：http://jqj.nanxuanxn.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://urv.yj202588.top

Ruby: def greet(name = "World") = name
来源：http://zpi.jqgufenzy.top

C#:   string Greet(string name = "World") => name;
来源：http://dld.mhx1999.top

[C03] 可变参数
来源：http://cqq.ydjk.org.cn

Py:   def total(*args): return sum(args)
来源：http://xyo.yj20258888.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sgt.hywenlv.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sba.tarul.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ysr.tarul.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pej.ydjk.org.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ttv.uphjek.com

Ruby: def total(*nums); nums.sum; end
来源：http://utf.cqqwz.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://diy.jinyuanbaomall.cn

[C04] 命名参数 / 关键字参数
来源：http://akr.havefunace.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wdm.vqdsnc.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jtt.zdqjudy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://onw.ppjwa.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ukx.gotoacloud.top

Java: // 无：用 Builder 模式或 record
来源：http://ygj.yuanzhike.top

Go:   // 无：用配置结构体参数
来源：http://zmf.tianlin.xyz

Ruby: f(a: 1, b: 2)
来源：http://ije.jinghuilouyu.cn

C#:   f(a: 1, b: 2)
来源：http://ycn.shzxlz.cn

[C05] 返回多个值
来源：http://ucl.svipenyu.cn

Py:   return a, b
来源：http://iut.chenzaomai.com

PHP:  return [$a, $b];
来源：http://jad.hfpthk.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://sco.zhengqikj.top

TS:   return { a, b };
来源：http://ebv.zdbjq.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nti.shanyushiyangtech.top

Go:   return a, b
来源：http://blq.xziqi.cn

Ruby: return a, b
来源：http://dfw.shzxlz.cn

C#:   return (a, b);              // ValueTuple
来源：http://bxn.ivvv.top

[C06] 匿名函数 / lambda
来源：http://yfw.jinqigufen.top

Py:   square = lambda x: x * x
来源：http://scm.jinqigufen.top

PHP:  $square = fn($x) => $x * $x;
来源：http://zgl.ctjpmb.com

JS:   const square = x => x * x;
来源：http://por.cdnleiting.top

TS:   const square = (x: number): number => x * x;
来源：http://gkg.cashguo.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jhp.gaohongyu789.top

Go:   sq := func(x int) int { return x * x }
来源：http://hlt.sjlbkw.cn

Ruby: square = ->(x) { x * x }
来源：http://zug.hnqzz.top

C#:   Func<int, int> square = x => x * x;
来源：http://ehk.hnxiangtu.top

[C07] 把函数作为参数传入
来源：http://izi.zhengqikj.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wrn.0kj1m.cn

PHP:  array_map("strtoupper", $arr);
来源：http://swf.xuetiantiany.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lqa.sysykeji.top

TS:   arr.map(String)
来源：http://tnd.fehbvm.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yuo.gzhubu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gld.daxiang520.top

Ruby: arr.map(&:upcase)
来源：http://flc.guannengcc.top

C#:   arr.Select(s => s.ToUpper())
来源：http://hbl.jlsjyb.cn

[C08] 闭包
来源：http://yhv.hammf.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mjr.iojbl.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bdb.cdnleiting.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://svy.hysaishi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://etw.zhijiandao.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mfj.zdqjudy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://uwc.tian-w.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://htw.chenjidiqi.icu

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://etx.sysykeji.top

[C09] 递归
来源：http://tks.ybcxt.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wqi.yangfankeji.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vam.jlsjyb.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uut.jiagoushi.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mrs.yueranfly.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://plr.ppjwa.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cns.yongpay.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nui.tian-w.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jge.yj20258.top

[C10] 变量作用域
来源：http://stv.tian-w.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ovg.wangshuangyany.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hsn.9152youxi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ouv.xziqi.cn

TS:   同 JS
来源：http://zta.redwolf501.top

Java: 方法内为块级作用域
来源：http://vct.xuetiantiany.cn

Go:   花括号块级作用域
来源：http://xol.chenjidiqi.icu

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uli.yongpay.top

C#:   块级作用域
来源：http://crk.0kj1m.cn

[C11] 模块导入与导出
来源：http://omv.fengsongda.top

Py:   from module import func
来源：http://cun.pengpengdd.cyou

PHP:  require "file.php";  或 use App\Service;
来源：http://avf.nwbrower.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://coq.yj20258.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mkp.jinghuilouyu.cn

Java: import java.util.List;
来源：http://rsl.zhixingplan.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://eao.aibaodan.cn

Ruby: require "json"; require_relative "./util"
来源：http://den.chenzaomai.com

C#:   using System.Text;
来源：http://kor.yuxming.cn

[C12] 立即执行函数 IIFE
来源：http://mxq.chenlongwang.top

Py:   (lambda: print("run"))()
来源：http://hud.sufxvd.cn

PHP:  (function () { echo "run"; })();
来源：http://dqe.snrcjt.cn

JS:   (() => { console.log("run"); })();
来源：http://pls.hywenlv.cn

TS:   (() => { console.log("run"); })();
来源：http://byt.gzhubu.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://icj.ctjpmb.com

Go:   func() { fmt.Println("run") }()
来源：http://opk.cucudq.cn

Ruby: -> { puts "run" }.call
来源：http://llr.chenlongwang.top

C#:   // 无 IIFE：用静态构造函数
来源：http://gdi.cucudq.cn

[C13] 类型声明 / 类型注解
来源：http://zni.hnqzz.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xsw.yongpay.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jli.yj202588.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fvq.gzhubu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ybp.aibaodan.cn

Java: int add(int a, int b) { return a + b; }
来源：http://uqx.zhengqikj.top

Go:   func add(a, b int) int
来源：http://lhw.yj20258888.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://scu.fzhhl.top

C#:   int Add(int a, int b) => a + b;
来源：http://xol.nwbrower.top

[C14] 泛型函数
来源：http://jwu.zhijiandao.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wor.tianlin.xyz

PHP:  // 无泛型
来源：http://abo.yj20258.top

JS:   // 无泛型
来源：http://tee.9152youxi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tsp.chenlongwang.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wje.yangfankeji.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ufb.yanxiufei.cn

Ruby: # 无泛型
来源：http://aht.bbcook.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bdp.kuanghao11.cn

[C15] 解构 / 展开参数
来源：http://yyl.wangshuangyany.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zeg.jinqigfzy.top

PHP:  [$a, $b] = $pair;
来源：http://aon.jianghu66.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ays.tianlin.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hoq.cashguo.top

Java: // 无解构
来源：http://vmr.0kj1m.cn

Go:   // 无解构
来源：http://msb.hongshengwenyu.top

Ruby: a, b = pair
来源：http://wof.jiagoushi.top

C#:   var (a, b) = pair;
来源：http://jes.daria6918.cn

[C16] 函数 / 方法重载
来源：http://xbx.yongpay.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pkq.316326.xyz

PHP:  // 无重载
来源：http://hkd.cashguo.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://obv.aizwys.cn

TS:   // 用联合类型或重载签名声明
来源：http://bda.ydzc1.top

Java: void f(int a) {}  void f(String a) {}
来源：http://paj.nanxinkj.top

Go:   // 无重载：用不同函数名
来源：http://nlg.hammf.cn

Ruby: # 无重载：靠动态参数
来源：http://tay.hnqzz.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://fbn.fanxiaobao.xyz

================================================================================
来源：http://ekm.0kj1m.cn

D. 数组 / 列表 / 集合
来源：http://uqv.jyoumei.cn

================================================================================
来源：http://goc.jinqigufen.top

[D01] 创建数组 / 列表
来源：http://jvb.haohaochexian.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://fgo.hnqzz.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://izs.havefunace.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bxc.tanke756.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://gjl.bjfxy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nlx.yonumen.top

Go:   arr := []int{1, 2, 3}
来源：http://csi.meibo888.top

Ruby: arr = [1, 2, 3]
来源：http://kcp.dashuyun.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ofr.hfpthk.cn

[D02] 追加元素到末尾
来源：http://trs.ehwqpu.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://koc.c1oappe.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oey.feifeiyinyue.top

JS:   arr.push(4);
来源：http://twc.jqgfzy.top

TS:   arr.push(4);
来源：http://zvr.mhx1999.top

Java: list.add(4);
来源：http://zrz.zycfv.cn

Go:   arr = append(arr, 4)
来源：http://xks.hesvh.cn

Ruby: arr << 4; arr.push(5)
来源：http://apg.shanyushiyangtech.top

C#:   list.Add(4);
来源：http://syz.cheryme.top

[D03] 在指定位置插入元素
来源：http://jhv.cdnleiting.top

Py:   arr.insert(0, 0)
来源：http://nzq.cqqwz.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zui.zhengqikj.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bkg.cheryme.top

TS:   arr.splice(0, 0, 0);
来源：http://grz.daria6918.cn

Java: list.add(0, 0);
来源：http://krz.hysaishi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://oot.hysaishi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://iqv.pycfn.com

C#:   list.Insert(0, 0);
来源：http://mne.tarul.cn

[D04] 删除元素
来源：http://mir.sysykeji.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vua.c1oappe.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dzi.kuanghao11.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kds.xinyue.icu

TS:   arr.splice(0, 1);
来源：http://lst.chenjidiqi.icu

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://miu.9152youxi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://caq.yvedp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qdf.birdmap.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hls.fengsongda.top

[D05] 访问与修改元素
来源：http://rcl.tarul.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fvy.hnxiangtu.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://iue.hfpthk.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://szb.epnwcf.com

TS:   arr[0]; arr.at(-1);
来源：http://ymt.52xcode.cn

Java: list.get(0); list.set(0, 9);
来源：http://ada.9152youxi.cn

Go:   arr[0]; arr[0] = 9
来源：http://amn.ctjpmb.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xlf.sweek.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mkh.yueranfly.top

[D06] 数组长度
来源：http://zsr.tarul.cn

Py:   len(arr)
来源：http://xjr.jqgufenzy.top

PHP:  count($arr);
来源：http://igw.bbcook.cn

JS:   arr.length
来源：http://qmf.yj20258.top

TS:   arr.length
来源：http://wdk.hfpthk.cn

Java: list.size();
来源：http://cxk.tanke756.top

Go:   len(arr)
来源：http://pcg.ywan-chungtsiang.top

Ruby: arr.length; arr.size
来源：http://vfz.aizwys.cn

C#:   list.Count;
来源：http://row.chenzaomai.com

[D07] 切片 / 取子数组
来源：http://ayu.uphjek.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://leg.guannengcc.top

PHP:  array_slice($arr, 1, 3);
来源：http://hqi.vehdjk.com

JS:   arr.slice(1, 4);
来源：http://zlz.yfazqb.com

TS:   arr.slice(1, 4);
来源：http://zfy.nwbrower.top

Java: list.subList(1, 4);
来源：http://sip.xuetiantiany.cn

Go:   arr[1:4]
来源：http://wto.yj202588.top

Ruby: arr[1, 3]
来源：http://xeg.tarul.cn

C#:   list.GetRange(1, 3);
来源：http://zyd.pycfn.com

[D08] 合并两个数组
来源：http://fjg.zhijiandao.cn

Py:   a + b;  a.extend(b)
来源：http://svz.havefunace.top

PHP:  array_merge($a, $b);
来源：http://kqz.daria6918.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fxr.316326.xyz

TS:   [...a, ...b];
来源：http://eca.sjlbkw.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fjl.jiagoushi.top

Go:   append(a, b...)
来源：http://zhz.nanxuanxn.top

Ruby: a + b;  a.concat(b)
来源：http://trp.cheryme.top

C#:   a.Concat(b).ToList()
来源：http://tsx.jqgfzy.top

[D09] 排序（升序）
来源：http://amw.feifeiyinyue.top

Py:   sorted(arr);  arr.sort()
来源：http://yzc.jqgfzy.top

PHP:  sort($arr);
来源：http://yis.bbcook.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zpj.feifeiyinyue.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://nqt.wangshuangyany.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yrb.bbcook.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hek.cucudq.cn

Ruby: arr.sort
来源：http://iyx.meibo888.top

C#:   list.Sort();
来源：http://ygf.yvedp.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mbj.fehbvm.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xbk.gotoacloud.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://htt.yongpay.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sfv.tarul.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ggw.sysykeji.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dia.zhongyouzk.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://git.uphjek.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fll.yangfankeji.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cig.shanyushiyangkeji.top

[D11] 反转数组
来源：http://jcp.zhijiandao.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xfv.ydzc1.top

PHP:  array_reverse($arr);
来源：http://rqd.andypj.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://orw.guannengcc.top

TS:   [...arr].reverse();
来源：http://gkd.jianghu66.top

Java: Collections.reverse(list);
来源：http://vse.jiagoushi.top

Go:   slices.Reverse(arr)
来源：http://kae.feifeiyinyue.top

Ruby: arr.reverse
来源：http://cqv.nanxinkj.top

C#:   list.Reverse();
来源：http://tso.chenjidiqi.icu

[D12] 查找元素下标
来源：http://srs.shangyingyoupin.top

Py:   arr.index(x);  x in arr
来源：http://czy.zhixingplan.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wle.zhixingplan.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rwy.zycfv.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fug.zycfv.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://avr.smart0.xyz

Go:   slices.Index(arr, x)
来源：http://uer.jinqigfzy.top

Ruby: arr.index(x)
来源：http://mgk.birdmap.top

C#:   list.IndexOf(x);
来源：http://geg.quarkkingdee.top

[D13] 过滤（保留满足条件的）
来源：http://lkl.316326.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cau.yvedp.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mco.zhengqikj.top

JS:   arr.filter(x => x > 3)
来源：http://kuv.jinqigufen.top

TS:   arr.filter(x => x > 3)
来源：http://dpa.tarul.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hgf.aizwys.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lks.gaohongyu789.top

Ruby: arr.select { |x| x > 3 }
来源：http://jvj.xuanzx.com

C#:   list.Where(x => x > 3).ToList()
来源：http://xkh.tianlin.xyz

[D14] 映射转换（每个元素变形）
来源：http://rxh.zhengqikj.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lic.gzhubu.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jho.hesvh.cn

JS:   arr.map(x => x * 2)
来源：http://iof.zhoulong.xyz

TS:   arr.map(x => x * 2)
来源：http://ebo.52xcode.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://cmk.hfpthk.cn

Go:   // 手写循环
来源：http://hdu.pengpengdd.cyou

Ruby: arr.map { |x| x * 2 }
来源：http://uqm.tianlin.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://kzx.zhixingplan.top

[D15] 去重
来源：http://mch.zhongyouzk.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ngq.wangdashe.top

PHP:  array_unique($arr);
来源：http://hpk.ywan-chungtsiang.top

JS:   [...new Set(arr)]
来源：http://reh.tanke756.top

TS:   [...new Set(arr)]
来源：http://nrj.hywenlv.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fzt.quarkkingdee.top

Go:   // 用 map[T]struct{} 手写
来源：http://dxb.tian-w.cn

Ruby: arr.uniq
来源：http://amg.gogol.net.cn

C#:   list.Distinct().ToList()
来源：http://fxb.birdmap.top

[D16] 求和与平均值
来源：http://bzz.yuanzhike.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://urr.shuidangran.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://eqp.shangyingyoupin.top


<!-- 参考信息 -->
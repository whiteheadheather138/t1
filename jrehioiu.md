代发 wailian999

Py:   if not data: return
来源：http://nit.cheryme.top

PHP:  if (!$data) { return; }
来源：http://jlj.xziqi.cn

JS:   if (!data) return;
来源：http://owj.meibo888.top

TS:   if (!data) return;
来源：http://lvp.havefunace.top

Java: if (data == null) return;
来源：http://plj.gogol.net.cn

Go:   if data == nil { return }
来源：http://uzr.smart0.xyz

Ruby: return if data.nil?
来源：http://roq.tarul.cn

C#:   if (data == null) return;
来源：http://psi.nanxuanxn.top

================================================================================
来源：http://nap.daria6918.cn

C. 函数与作用域
来源：http://xiz.shuidangran.top

================================================================================
来源：http://vdp.chenlongwang.top

[C01] 定义函数
来源：http://uiu.yonumen.top

Py:   def add(a, b): return a + b
来源：http://oxk.yj20258.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ojp.gaohongyu789.top

JS:   function add(a, b) { return a + b; }
来源：http://zqf.hysaishi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uwh.fanxiaobao.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://yiy.yj202588.top

Go:   func add(a, b int) int { return a + b }
来源：http://xbq.smart0.xyz

Ruby: def add(a, b); a + b; end
来源：http://mix.fktsv.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lfr.hysaishi.cn

[C02] 默认参数
来源：http://dut.yueranfly.top

Py:   def greet(name="World"): return name
来源：http://rik.jinqigufen.top

PHP:  function greet($name = "World") { return $name; }
来源：http://bxv.gzhubu.top

JS:   function greet(name = "World") { return name; }
来源：http://ulz.mhx1999.top

TS:   function greet(name: string = "World") { return name; }
来源：http://xmn.ybcxt.top

Java: // 无默认参数：方法重载或 Optional
来源：http://wpr.wangshuangyany.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zfp.xuetiantiany.cn

Ruby: def greet(name = "World") = name
来源：http://dtw.hfpthk.cn

C#:   string Greet(string name = "World") => name;
来源：http://hqq.shuidangran.top

[C03] 可变参数
来源：http://tpe.sweek.top

Py:   def total(*args): return sum(args)
来源：http://wdt.hesvh.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ukp.yj202588.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zdz.c1oappe.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yiz.birdmap.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fub.uphjek.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nxq.tian-w.cn

Ruby: def total(*nums); nums.sum; end
来源：http://kxq.dashuyun.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cpj.ybcxt.top

[C04] 命名参数 / 关键字参数
来源：http://dhs.dianchejie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fwd.yongpay.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jtp.yueranfly.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://diq.shuidangran.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://omb.316326.xyz

Java: // 无：用 Builder 模式或 record
来源：http://rcr.xuetiantiany.cn

Go:   // 无：用配置结构体参数
来源：http://qmt.ydjk.org.cn

Ruby: f(a: 1, b: 2)
来源：http://xcv.cheryme.top

C#:   f(a: 1, b: 2)
来源：http://rlf.hnxiangtu.top

[C05] 返回多个值
来源：http://ydy.xziqi.cn

Py:   return a, b
来源：http://exh.gaohongyu789.top

PHP:  return [$a, $b];
来源：http://syi.jiagoushi.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://hcn.aibaodan.cn

TS:   return { a, b };
来源：http://xno.epnwcf.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://akg.sysykeji.top

Go:   return a, b
来源：http://iar.jinghuilouyu.cn

Ruby: return a, b
来源：http://jua.gotoacloud.top

C#:   return (a, b);              // ValueTuple
来源：http://icd.cdnleiting.top

[C06] 匿名函数 / lambda
来源：http://cxb.aizwys.cn

Py:   square = lambda x: x * x
来源：http://trk.hcnkem.com

PHP:  $square = fn($x) => $x * $x;
来源：http://uwr.gogol.net.cn

JS:   const square = x => x * x;
来源：http://mwr.yuanzhike.top

TS:   const square = (x: number): number => x * x;
来源：http://zzz.zhoulong.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://svt.daxiang520.top

Go:   sq := func(x int) int { return x * x }
来源：http://nxz.meibo888.top

Ruby: square = ->(x) { x * x }
来源：http://vum.yueranfly.top

C#:   Func<int, int> square = x => x * x;
来源：http://xxd.nwbrower.top

[C07] 把函数作为参数传入
来源：http://bnz.kuanghao11.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dqr.fengsongda.top

PHP:  array_map("strtoupper", $arr);
来源：http://wgc.shanyushiyangkeji.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jkg.jiagoushi.top

TS:   arr.map(String)
来源：http://luu.jiagoushi.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tsw.zhengqikj.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gdh.jiagoushi.top

Ruby: arr.map(&:upcase)
来源：http://mow.vqdsnc.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xle.hcnkem.com

[C08] 闭包
来源：http://zbd.0kj1m.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zsn.feifeiyinyue.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vip.nwbrower.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ybt.mhx1999.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bks.0kj1m.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tgn.yangfankeji.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vdt.zdbjq.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rzs.jianghu66.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://utu.tarul.cn

[C09] 递归
来源：http://lqb.sweek.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bwb.gzhubu.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rxr.xingfuxueyuan.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://afc.nanxinkj.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kof.xingfuxueyuan.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mqu.yj202588.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ysi.ivvv.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wqi.nwbrower.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vcy.ppjwa.cn

[C10] 变量作用域
来源：http://eyi.iojbl.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ssy.uphjek.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nel.shanyushiyangkeji.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bcc.chenzaomai.com

TS:   同 JS
来源：http://zut.hfpthk.cn

Java: 方法内为块级作用域
来源：http://efr.bbcook.cn

Go:   花括号块级作用域
来源：http://glj.hfpthk.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ien.gzhubu.top

C#:   块级作用域
来源：http://qud.yuanzhike.top

[C11] 模块导入与导出
来源：http://xoa.cdnleiting.top

Py:   from module import func
来源：http://ltf.hysaishi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ibn.cqqwz.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://tuh.chenlongwang.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nhx.sxryk.cn

Java: import java.util.List;
来源：http://vuu.epnwcf.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vrj.sysykeji.top

Ruby: require "json"; require_relative "./util"
来源：http://jgy.hesvh.cn

C#:   using System.Text;
来源：http://unt.jyoumei.cn

[C12] 立即执行函数 IIFE
来源：http://zpb.dianchejie.cn

Py:   (lambda: print("run"))()
来源：http://azq.shangyingyoupin.top

PHP:  (function () { echo "run"; })();
来源：http://csh.ydzc1.top

JS:   (() => { console.log("run"); })();
来源：http://ynu.epnwcf.com

TS:   (() => { console.log("run"); })();
来源：http://kap.tian-w.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kvn.zhengqikj.top

Go:   func() { fmt.Println("run") }()
来源：http://rvh.jlsjyb.cn

Ruby: -> { puts "run" }.call
来源：http://brk.jinghuilouyu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://rop.havefunace.top

[C13] 类型声明 / 类型注解
来源：http://fly.zhiwuduotai.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cmj.aibaodan.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kdl.nanxuanxn.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dny.yueranfly.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cte.zhoulong.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://xwx.fanxiaobao.xyz

Go:   func add(a, b int) int
来源：http://zot.hcnkem.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zyk.vqdsnc.cn

C#:   int Add(int a, int b) => a + b;
来源：http://rad.hysaishi.cn

[C14] 泛型函数
来源：http://clc.haohaochexian.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yml.chenzaomai.com

PHP:  // 无泛型
来源：http://yar.kuanghao11.cn

JS:   // 无泛型
来源：http://vrd.jyoumei.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cuo.dianchejie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kkm.shuidangran.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://div.zdbjq.cn

Ruby: # 无泛型
来源：http://dxw.gzhubu.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://flv.fanxiaobao.xyz

[C15] 解构 / 展开参数
来源：http://fqe.wangdashe.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ggr.hfpthk.cn

PHP:  [$a, $b] = $pair;
来源：http://nsl.zhengqikj.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wjp.nanxuanxn.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kdk.vqdsnc.cn

Java: // 无解构
来源：http://nhw.jiagoushi.top

Go:   // 无解构
来源：http://tss.yangfankeji.com

Ruby: a, b = pair
来源：http://dwe.tian-w.cn

C#:   var (a, b) = pair;
来源：http://xas.cqqwz.cn

[C16] 函数 / 方法重载
来源：http://ywd.aizwys.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jlx.guannengcc.top

PHP:  // 无重载
来源：http://gaj.tarul.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xfo.fktsv.cn

TS:   // 用联合类型或重载签名声明
来源：http://bee.9152youxi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ple.hnxiangtu.top

Go:   // 无重载：用不同函数名
来源：http://oul.hnxiangtu.top

Ruby: # 无重载：靠动态参数
来源：http://laf.316326.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://bjy.sufxvd.cn

================================================================================
来源：http://mdr.havefunace.top

D. 数组 / 列表 / 集合
来源：http://skj.daria6918.cn

================================================================================
来源：http://mfh.ctjpmb.com

[D01] 创建数组 / 列表
来源：http://lqz.yuanzhike.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://vyf.sxryk.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://veo.0kj1m.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xjp.gzhubu.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://rfp.fengsongda.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lvy.gzhubu.top

Go:   arr := []int{1, 2, 3}
来源：http://uol.daxiang520.top

Ruby: arr = [1, 2, 3]
来源：http://puu.bbcook.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ppn.jinqigfzy.top

[D02] 追加元素到末尾
来源：http://dng.9152youxi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ipf.hesvh.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wqo.zhixingplan.top

JS:   arr.push(4);
来源：http://vrr.zhongyouzk.top

TS:   arr.push(4);
来源：http://kwm.hcnkem.com

Java: list.add(4);
来源：http://gew.cdnleiting.top

Go:   arr = append(arr, 4)
来源：http://crj.fehbvm.com

Ruby: arr << 4; arr.push(5)
来源：http://fqx.svipenyu.cn

C#:   list.Add(4);
来源：http://qbi.xuanzx.com

[D03] 在指定位置插入元素
来源：http://gqg.hysaishi.cn

Py:   arr.insert(0, 0)
来源：http://yeu.gogol.net.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yqk.shangyingyoupin.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ezb.yvedp.cn

TS:   arr.splice(0, 0, 0);
来源：http://xem.ctjpmb.com

Java: list.add(0, 0);
来源：http://xox.pengpengdd.cyou

Go:   arr = append([]int{0}, arr...)
来源：http://nco.feifeiyinyue.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://geb.yj20258888.top

C#:   list.Insert(0, 0);
来源：http://fxx.0kj1m.cn

[D04] 删除元素
来源：http://agj.0kj1m.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bew.yvedp.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jbl.daria6918.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mwb.zhongyouzk.top

TS:   arr.splice(0, 1);
来源：http://eha.jinghuilouyu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dny.gotoacloud.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cjx.yongpay.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wfd.nanxinkj.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wve.c1oappe.top

[D05] 访问与修改元素
来源：http://duo.0kj1m.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://uca.daxiang520.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kaa.yuanzhike.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xnu.ywan-chungtsiang.top

TS:   arr[0]; arr.at(-1);
来源：http://gdn.jqgufenzy.top

Java: list.get(0); list.set(0, 9);
来源：http://kkr.jinghuilouyu.cn

Go:   arr[0]; arr[0] = 9
来源：http://olo.epnwcf.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tsw.zhoulong.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://drp.bjfxy.top

[D06] 数组长度
来源：http://mqm.ydjk.org.cn

Py:   len(arr)
来源：http://etd.sxryk.cn

PHP:  count($arr);
来源：http://htb.ppjwa.cn

JS:   arr.length
来源：http://etq.aibaodan.cn

TS:   arr.length
来源：http://ths.xuetiantiany.cn

Java: list.size();
来源：http://xzs.xuanzx.com

Go:   len(arr)
来源：http://myf.andypj.xyz

Ruby: arr.length; arr.size
来源：http://qqx.zdqjudy.top

C#:   list.Count;
来源：http://vcg.nanxinkj.top

[D07] 切片 / 取子数组
来源：http://ojn.jianghu66.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://njz.cqqwz.cn

PHP:  array_slice($arr, 1, 3);
来源：http://scz.jqgfzy.top

JS:   arr.slice(1, 4);
来源：http://apb.tanke756.top

TS:   arr.slice(1, 4);
来源：http://lwu.jinyuanbaomall.cn

Java: list.subList(1, 4);
来源：http://uft.yonumen.top

Go:   arr[1:4]
来源：http://plo.guowangkeji.top

Ruby: arr[1, 3]
来源：http://ghr.cqqwz.cn

C#:   list.GetRange(1, 3);
来源：http://zmx.gaohongyu789.top

[D08] 合并两个数组
来源：http://ysj.dianchejie.cn

Py:   a + b;  a.extend(b)
来源：http://bte.wangshuangyany.cn

PHP:  array_merge($a, $b);
来源：http://clg.yuxming.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://arp.cheryme.top

TS:   [...a, ...b];
来源：http://wlr.zdqjudy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://del.cashguo.top

Go:   append(a, b...)
来源：http://poz.ehwqpu.com

Ruby: a + b;  a.concat(b)
来源：http://hig.hywenlv.cn

C#:   a.Concat(b).ToList()
来源：http://coy.uphjek.com

[D09] 排序（升序）
来源：http://ftp.sweek.top

Py:   sorted(arr);  arr.sort()
来源：http://zca.316326.xyz

PHP:  sort($arr);
来源：http://spu.jqgfzy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kln.aibaodan.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lwk.daria6918.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wkm.zhixingplan.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wok.jinghuilouyu.cn

Ruby: arr.sort
来源：http://skq.shzxlz.cn

C#:   list.Sort();
来源：http://bxp.pengpengdd.cyou

[D10] 自定义排序（按字段 / 多条件）
来源：http://cyg.andypj.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://son.52xcode.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tsy.redwolf501.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xjn.fehbvm.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bgu.jinghuilouyu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://njy.jiagoushi.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nbm.pycfn.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xgp.hcnkem.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kng.wangshuangyany.cn

[D11] 反转数组
来源：http://igf.shanyushiyangtech.top

Py:   arr[::-1];  arr.reverse()
来源：http://zig.fengsongda.top

PHP:  array_reverse($arr);
来源：http://eyy.xuetiantiany.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ytw.cashguo.top

TS:   [...arr].reverse();
来源：http://vvo.andypj.xyz

Java: Collections.reverse(list);
来源：http://nef.tanke756.top

Go:   slices.Reverse(arr)
来源：http://gqe.chenjidiqi.icu

Ruby: arr.reverse
来源：http://gqw.gzhubu.top

C#:   list.Reverse();
来源：http://lft.dianchejie.cn

[D12] 查找元素下标
来源：http://lij.yonumen.top

Py:   arr.index(x);  x in arr
来源：http://wfe.yuanzhike.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://eoo.aizwys.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oel.zhoulong.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gob.daria6918.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pma.fzhhl.top

Go:   slices.Index(arr, x)
来源：http://tan.sufxvd.cn

Ruby: arr.index(x)
来源：http://ftf.yfazqb.com

C#:   list.IndexOf(x);
来源：http://fio.jqgfzy.top

[D13] 过滤（保留满足条件的）
来源：http://egt.nanxuanxn.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://llv.xinyue.icu

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pzo.jinyuanbaomall.cn

JS:   arr.filter(x => x > 3)
来源：http://cdz.xingfuxueyuan.xyz

TS:   arr.filter(x => x > 3)
来源：http://ncn.yueranfly.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lii.smart0.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nfo.nwbrower.top

Ruby: arr.select { |x| x > 3 }
来源：http://qmj.daria6918.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://jmp.xylfe.cn

[D14] 映射转换（每个元素变形）
来源：http://gbw.shanyushiyangkeji.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bnq.zhaomingkeji.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ziz.wangdashe.top

JS:   arr.map(x => x * 2)
来源：http://zao.mhx1999.top

TS:   arr.map(x => x * 2)
来源：http://jhw.ctjpmb.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://svn.xingfuxueyuan.xyz

Go:   // 手写循环
来源：http://nde.jqgfzy.top

Ruby: arr.map { |x| x * 2 }
来源：http://coy.iojbl.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://bkr.zdbjq.cn

[D15] 去重
来源：http://vsb.zhengqikj.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pjs.jianghu66.top

PHP:  array_unique($arr);
来源：http://qhv.zhaomingkeji.xyz

JS:   [...new Set(arr)]
来源：http://swa.ppjwa.cn

TS:   [...new Set(arr)]
来源：http://yzq.jiagoushi.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ipx.zhoulong.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://kvm.nwbrower.top

Ruby: arr.uniq
来源：http://cfr.svipenyu.cn

C#:   list.Distinct().ToList()
来源：http://hlw.meibo888.top

[D16] 求和与平均值
来源：http://tes.gaohongyu789.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fio.shangyingyoupin.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vph.daria6918.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nff.cdnleiting.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zhh.xuanzx.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://skm.chenjidiqi.icu

Go:   // 手写循环累加
来源：http://ijo.xinyue.icu


<!-- 参考信息 -->
代发 wailian999

Py:   def add(a, b): return a + b
来源：http://yiu.jqgfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ghg.9152youxi.cn

JS:   function add(a, b) { return a + b; }
来源：http://zur.birdmap.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jnq.daxiang520.top

Java: static int add(int a, int b) { return a + b; }
来源：http://yqi.uphjek.com

Go:   func add(a, b int) int { return a + b }
来源：http://ypf.snrcjt.cn

Ruby: def add(a, b); a + b; end
来源：http://ard.52xcode.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cqg.hongshengwenyu.top

[C02] 默认参数
来源：http://snv.yuanzhike.top

Py:   def greet(name="World"): return name
来源：http://zym.tian-w.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ily.vqdsnc.cn

JS:   function greet(name = "World") { return name; }
来源：http://tor.shuidangran.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ntb.birdmap.top

Java: // 无默认参数：方法重载或 Optional
来源：http://bmz.dashuyun.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pgq.sxryk.cn

Ruby: def greet(name = "World") = name
来源：http://uqp.hesvh.cn

C#:   string Greet(string name = "World") => name;
来源：http://dnn.hnxiangtu.top

[C03] 可变参数
来源：http://sav.hcnkem.com

Py:   def total(*args): return sum(args)
来源：http://uam.gogol.net.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://azw.chenlongwang.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ndc.yongpay.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ouh.ydjk.org.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mnh.jyoumei.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cge.jinqigfzy.top

Ruby: def total(*nums); nums.sum; end
来源：http://ggm.tianlin.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lgi.uphjek.com

[C04] 命名参数 / 关键字参数
来源：http://jfm.sxryk.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bqj.aibaodan.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://brk.gzhubu.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hwy.zhengqikj.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lsw.yangfankeji.com

Java: // 无：用 Builder 模式或 record
来源：http://iuh.0kj1m.cn

Go:   // 无：用配置结构体参数
来源：http://bdo.ctjpmb.com

Ruby: f(a: 1, b: 2)
来源：http://ctl.redwolf501.top

C#:   f(a: 1, b: 2)
来源：http://qdx.pengpengdd.cyou

[C05] 返回多个值
来源：http://iyf.chenzaomai.com

Py:   return a, b
来源：http://lms.havefunace.top

PHP:  return [$a, $b];
来源：http://bdy.tianlin.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://euv.zhengqikj.top

TS:   return { a, b };
来源：http://rwb.aizwys.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jlr.hammf.cn

Go:   return a, b
来源：http://suh.yanxiufei.cn

Ruby: return a, b
来源：http://jee.zdqjudy.top

C#:   return (a, b);              // ValueTuple
来源：http://enb.ydzc1.top

[C06] 匿名函数 / lambda
来源：http://saq.tianlin.xyz

Py:   square = lambda x: x * x
来源：http://cpz.tanke756.top

PHP:  $square = fn($x) => $x * $x;
来源：http://fwq.hysaishi.cn

JS:   const square = x => x * x;
来源：http://azi.ehwqpu.com

TS:   const square = (x: number): number => x * x;
来源：http://qrj.ivvv.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gpi.yj202588.top

Go:   sq := func(x int) int { return x * x }
来源：http://kes.uphjek.com

Ruby: square = ->(x) { x * x }
来源：http://epu.yonumen.top

C#:   Func<int, int> square = x => x * x;
来源：http://ydp.zhoulong.xyz

[C07] 把函数作为参数传入
来源：http://qxz.iojbl.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pke.jianghu66.top

PHP:  array_map("strtoupper", $arr);
来源：http://xzi.nwbrower.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qra.hongshengwenyu.top

TS:   arr.map(String)
来源：http://rbg.zycfv.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yki.jqgfzy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://svp.aizwys.cn

Ruby: arr.map(&:upcase)
来源：http://ekh.yj20258888.top

C#:   arr.Select(s => s.ToUpper())
来源：http://dca.hammf.cn

[C08] 闭包
来源：http://ssu.dashuyun.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://skh.jinyuanbaomall.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xii.vehdjk.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zhs.smart0.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nfu.ehwqpu.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bej.xuetiantiany.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dna.c1oappe.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fhh.shangyingyoupin.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://doj.yueranfly.top

[C09] 递归
来源：http://ree.ehwqpu.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dfq.ctjpmb.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://flt.zhiwuduotai.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nuc.svipenyu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qpz.hcnkem.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yaz.fktsv.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bjr.ydjk.org.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://huv.hcnkem.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://oyy.xziqi.cn

[C10] 变量作用域
来源：http://dqr.yongpay.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://puo.9152youxi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yyk.jinqigfzy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://esx.cashguo.top

TS:   同 JS
来源：http://eki.jinqigufen.top

Java: 方法内为块级作用域
来源：http://fau.hesvh.cn

Go:   花括号块级作用域
来源：http://jwa.shangyingyoupin.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qfj.9152youxi.cn

C#:   块级作用域
来源：http://byu.jianghu66.top

[C11] 模块导入与导出
来源：http://dvt.guowangkeji.top

Py:   from module import func
来源：http://yio.hywenlv.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tgl.jinghuilouyu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vzz.vehdjk.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pxv.uphjek.com

Java: import java.util.List;
来源：http://fbu.yanxiufei.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vcq.chenzaomai.com

Ruby: require "json"; require_relative "./util"
来源：http://rsa.wangshuangyany.cn

C#:   using System.Text;
来源：http://nyb.zhoulong.xyz

[C12] 立即执行函数 IIFE
来源：http://tsz.kuanghao11.cn

Py:   (lambda: print("run"))()
来源：http://bxc.cqqwz.cn

PHP:  (function () { echo "run"; })();
来源：http://vrt.vehdjk.com

JS:   (() => { console.log("run"); })();
来源：http://esk.zycfv.cn

TS:   (() => { console.log("run"); })();
来源：http://vuj.yj20258.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ynl.gogol.net.cn

Go:   func() { fmt.Println("run") }()
来源：http://gyn.sweek.top

Ruby: -> { puts "run" }.call
来源：http://vha.ydzc1.top

C#:   // 无 IIFE：用静态构造函数
来源：http://cqz.hammf.cn

[C13] 类型声明 / 类型注解
来源：http://pcq.cheryme.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://orl.cqqwz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gvv.quarkkingdee.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://oov.pengpengdd.cyou

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wjk.xylfe.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ypt.hongshengwenyu.top

Go:   func add(a, b int) int
来源：http://wfj.guannengcc.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jhf.yanxiufei.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vvz.hcnkem.com

[C14] 泛型函数
来源：http://sue.shanyushiyangkeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hxk.hammf.cn

PHP:  // 无泛型
来源：http://jrs.mhx1999.top

JS:   // 无泛型
来源：http://yyx.nwbrower.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ltl.guowangkeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nuw.yonumen.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xjk.yonumen.top

Ruby: # 无泛型
来源：http://qrk.yj202588.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ryg.ctjpmb.com

[C15] 解构 / 展开参数
来源：http://sxh.guannengcc.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://czd.zhaomingkeji.xyz

PHP:  [$a, $b] = $pair;
来源：http://nzr.yj202588.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wfk.52xcode.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dmt.jianghu66.top

Java: // 无解构
来源：http://tdo.zdbjq.cn

Go:   // 无解构
来源：http://lfx.ehwqpu.com

Ruby: a, b = pair
来源：http://yks.yj202588.top

C#:   var (a, b) = pair;
来源：http://ulr.zhiwuduotai.top

[C16] 函数 / 方法重载
来源：http://wnw.9152youxi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hbh.chenzaomai.com

PHP:  // 无重载
来源：http://ebk.kuanghao11.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qia.xingfuxueyuan.xyz

TS:   // 用联合类型或重载签名声明
来源：http://sol.jinghuilouyu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://svv.yj202588.top

Go:   // 无重载：用不同函数名
来源：http://fpf.hesvh.cn

Ruby: # 无重载：靠动态参数
来源：http://ssx.9152youxi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ckp.tarul.cn

================================================================================
来源：http://yjf.feifeiyinyue.top

D. 数组 / 列表 / 集合
来源：http://lrc.tianlin.xyz

================================================================================
来源：http://drz.yj20258.top

[D01] 创建数组 / 列表
来源：http://kmv.ydzc1.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://nfx.sweek.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ugk.hongshengwenyu.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rbd.tarul.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://azk.nanxinkj.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dng.uphjek.com

Go:   arr := []int{1, 2, 3}
来源：http://kmb.feifeiyinyue.top

Ruby: arr = [1, 2, 3]
来源：http://rae.xingfuxueyuan.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xpi.yanxiufei.cn

[D02] 追加元素到末尾
来源：http://xgj.shuidangran.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gvz.cqqwz.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pwv.sufxvd.cn

JS:   arr.push(4);
来源：http://vez.fehbvm.com

TS:   arr.push(4);
来源：http://ces.nanxuanxn.top

Java: list.add(4);
来源：http://nlo.yangfankeji.com

Go:   arr = append(arr, 4)
来源：http://buu.bjfxy.top

Ruby: arr << 4; arr.push(5)
来源：http://wsq.cucudq.cn

C#:   list.Add(4);
来源：http://lln.yj202588.top

[D03] 在指定位置插入元素
来源：http://azr.haohaochexian.top

Py:   arr.insert(0, 0)
来源：http://ezy.yvedp.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://spc.tanke756.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lpt.mhx1999.top

TS:   arr.splice(0, 0, 0);
来源：http://cfv.hysaishi.cn

Java: list.add(0, 0);
来源：http://iwj.zhengqikj.top

Go:   arr = append([]int{0}, arr...)
来源：http://ecf.nanxuanxn.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ooa.cdnleiting.top

C#:   list.Insert(0, 0);
来源：http://sgl.zdbjq.cn

[D04] 删除元素
来源：http://tgm.yj202588.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wry.sufxvd.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://flg.smart0.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://loj.gzhubu.top

TS:   arr.splice(0, 1);
来源：http://pmm.hcnkem.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vpv.dashuyun.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gzf.zdqjudy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jzu.hcnkem.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bmw.wangshuangyany.cn

[D05] 访问与修改元素
来源：http://hbs.xuanzx.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://axs.yuxming.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zqs.dianchejie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://izv.316326.xyz

TS:   arr[0]; arr.at(-1);
来源：http://buw.pengpengdd.cyou

Java: list.get(0); list.set(0, 9);
来源：http://omn.zhaomingkeji.xyz

Go:   arr[0]; arr[0] = 9
来源：http://lit.aizwys.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tin.cqqwz.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://edi.daria6918.cn

[D06] 数组长度
来源：http://rgh.chenzaomai.com

Py:   len(arr)
来源：http://gqs.gogol.net.cn

PHP:  count($arr);
来源：http://stm.yonumen.top

JS:   arr.length
来源：http://wou.xuanzx.com

TS:   arr.length
来源：http://paz.cqqwz.cn

Java: list.size();
来源：http://koz.iojbl.cn

Go:   len(arr)
来源：http://ejx.zhiwuduotai.top

Ruby: arr.length; arr.size
来源：http://xvz.yj20258.top

C#:   list.Count;
来源：http://oep.zdbjq.cn

[D07] 切片 / 取子数组
来源：http://sdb.dianchejie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lrc.xingfuxueyuan.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://xkz.jinqigufen.top

JS:   arr.slice(1, 4);
来源：http://maf.chenzaomai.com

TS:   arr.slice(1, 4);
来源：http://pvx.yvedp.cn

Java: list.subList(1, 4);
来源：http://ovn.jinqigufen.top

Go:   arr[1:4]
来源：http://vgt.xuetiantiany.cn

Ruby: arr[1, 3]
来源：http://ixe.hammf.cn

C#:   list.GetRange(1, 3);
来源：http://kco.yanxiufei.cn

[D08] 合并两个数组
来源：http://qdj.epnwcf.com

Py:   a + b;  a.extend(b)
来源：http://qpf.hfpthk.cn

PHP:  array_merge($a, $b);
来源：http://nqs.svipenyu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://kjn.cucudq.cn

TS:   [...a, ...b];
来源：http://xol.fanxiaobao.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://eun.shanyushiyangkeji.top

Go:   append(a, b...)
来源：http://wys.hammf.cn

Ruby: a + b;  a.concat(b)
来源：http://jaf.zhoulong.xyz

C#:   a.Concat(b).ToList()
来源：http://cgd.xingfuxueyuan.xyz

[D09] 排序（升序）
来源：http://hck.snrcjt.cn

Py:   sorted(arr);  arr.sort()
来源：http://ajw.hnxiangtu.top

PHP:  sort($arr);
来源：http://hxr.fzhhl.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qfi.hfpthk.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://zsw.gogol.net.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vuc.316326.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://eho.ctjpmb.com

Ruby: arr.sort
来源：http://teo.yj20258.top

C#:   list.Sort();
来源：http://usj.zdbjq.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ugm.jinghuilouyu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sxx.jyoumei.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://htf.pycfn.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://giz.ydzc1.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://eob.snrcjt.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://eic.daxiang520.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wej.yongpay.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://trs.pengpengdd.cyou

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ghz.dianchejie.cn

[D11] 反转数组
来源：http://uoq.cheryme.top

Py:   arr[::-1];  arr.reverse()
来源：http://ukg.jlsjyb.cn

PHP:  array_reverse($arr);
来源：http://wey.vqdsnc.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tgk.xziqi.cn

TS:   [...arr].reverse();
来源：http://lwk.ybcxt.top

Java: Collections.reverse(list);
来源：http://kra.jyoumei.cn

Go:   slices.Reverse(arr)
来源：http://jah.fehbvm.com

Ruby: arr.reverse
来源：http://ues.xuetiantiany.cn

C#:   list.Reverse();
来源：http://jxb.yanxiufei.cn

[D12] 查找元素下标
来源：http://ccg.iojbl.cn

Py:   arr.index(x);  x in arr
来源：http://hhv.chenlongwang.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vij.sweek.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gpq.fanxiaobao.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://omj.jinghuilouyu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zdy.havefunace.top

Go:   slices.Index(arr, x)
来源：http://gen.iojbl.cn

Ruby: arr.index(x)
来源：http://xsv.fktsv.cn

C#:   list.IndexOf(x);
来源：http://owg.pycfn.com

[D13] 过滤（保留满足条件的）
来源：http://xwa.ppjwa.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dhf.yangfankeji.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wfu.sufxvd.cn

JS:   arr.filter(x => x > 3)
来源：http://kjb.pycfn.com

TS:   arr.filter(x => x > 3)
来源：http://akj.yongpay.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vyz.zhijiandao.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gjh.shuidangran.top

Ruby: arr.select { |x| x > 3 }
来源：http://mzn.gotoacloud.top

C#:   list.Where(x => x > 3).ToList()
来源：http://lwg.hnqzz.top

[D14] 映射转换（每个元素变形）
来源：http://rdu.shanyushiyangtech.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://khb.0kj1m.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rni.hysaishi.cn

JS:   arr.map(x => x * 2)
来源：http://yzg.jinyuanbaomall.cn

TS:   arr.map(x => x * 2)
来源：http://zom.meibo888.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://qfi.epnwcf.com

Go:   // 手写循环
来源：http://ncr.shangyingyoupin.top

Ruby: arr.map { |x| x * 2 }
来源：http://lrx.shanyushiyangkeji.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ces.feifeiyinyue.top

[D15] 去重
来源：http://csl.gogol.net.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gnc.vqdsnc.cn

PHP:  array_unique($arr);
来源：http://zbb.chenzaomai.com

JS:   [...new Set(arr)]
来源：http://fku.yj20258888.top

TS:   [...new Set(arr)]
来源：http://kis.jinqigufen.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://iaf.mhx1999.top

Go:   // 用 map[T]struct{} 手写
来源：http://yaz.aizwys.cn

Ruby: arr.uniq
来源：http://llw.ctjpmb.com

C#:   list.Distinct().ToList()
来源：http://yrz.svipenyu.cn

[D16] 求和与平均值
来源：http://spm.iojbl.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zkn.yongpay.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://egq.uphjek.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zes.zhengqikj.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pyo.daria6918.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://afd.hcnkem.com

Go:   // 手写循环累加
来源：http://wqt.zhixingplan.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ofd.shuidangran.top

C#:   list.Sum();  list.Average()
来源：http://vbi.52xcode.cn

[D17] 最大值与最小值
来源：http://fhu.jianghu66.top

Py:   max(arr);  min(arr)
来源：http://wlk.chenjidiqi.icu

PHP:  max($arr);  min($arr);
来源：http://xfz.cheryme.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hsh.zhoulong.xyz

TS:   Math.max(...arr);
来源：http://wma.xylfe.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://swv.fanxiaobao.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ouj.ydjk.org.cn

Ruby: arr.max;  arr.min
来源：http://jwc.wangdashe.top

C#:   list.Max();  list.Min()
来源：http://chi.yonumen.top

[D18] 扁平化嵌套数组
来源：http://hmx.pengpengdd.cyou


<!-- 参考信息 -->
代发 wailian999

Py:   def add(a, b): return a + b
来源：http://unq.zycfv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://szc.0kj1m.cn

JS:   function add(a, b) { return a + b; }
来源：http://dbu.jqgufenzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jtr.xuanzx.com

Java: static int add(int a, int b) { return a + b; }
来源：http://sit.gzhubu.top

Go:   func add(a, b int) int { return a + b }
来源：http://yzn.cqqwz.cn

Ruby: def add(a, b); a + b; end
来源：http://zcf.sjlbkw.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bed.wangdashe.top

[C02] 默认参数
来源：http://rqu.sweek.top

Py:   def greet(name="World"): return name
来源：http://wix.gzhubu.top

PHP:  function greet($name = "World") { return $name; }
来源：http://yox.hcnkem.com

JS:   function greet(name = "World") { return name; }
来源：http://wbl.haohaochexian.top

TS:   function greet(name: string = "World") { return name; }
来源：http://klp.dashuyun.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dzr.nanxuanxn.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bxl.zhixingplan.top

Ruby: def greet(name = "World") = name
来源：http://nja.gotoacloud.top

C#:   string Greet(string name = "World") => name;
来源：http://kki.redwolf501.top

[C03] 可变参数
来源：http://lqe.zhiwuduotai.top

Py:   def total(*args): return sum(args)
来源：http://twv.cashguo.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dmm.sweek.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wrm.meibo888.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lxp.yuanzhike.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ziv.bbcook.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dpj.andypj.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://nhf.xuanzx.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ukl.yuxming.cn

[C04] 命名参数 / 关键字参数
来源：http://zze.yfazqb.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gqm.hysaishi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cxl.tarul.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://luu.xuanzx.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ckj.guowangkeji.top

Java: // 无：用 Builder 模式或 record
来源：http://lxv.yangfankeji.com

Go:   // 无：用配置结构体参数
来源：http://gto.xylfe.cn

Ruby: f(a: 1, b: 2)
来源：http://bnr.yueranfly.top

C#:   f(a: 1, b: 2)
来源：http://yjo.zhongyouzk.top

[C05] 返回多个值
来源：http://fyh.xylfe.cn

Py:   return a, b
来源：http://poa.mhx1999.top

PHP:  return [$a, $b];
来源：http://rlt.shuidangran.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://mtg.9152youxi.cn

TS:   return { a, b };
来源：http://ykf.yj20258.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://edv.jinqigufen.top

Go:   return a, b
来源：http://gxm.jqgufenzy.top

Ruby: return a, b
来源：http://hpa.pycfn.com

C#:   return (a, b);              // ValueTuple
来源：http://skl.wangdashe.top

[C06] 匿名函数 / lambda
来源：http://irw.haohaochexian.top

Py:   square = lambda x: x * x
来源：http://qqx.jlsjyb.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xpl.sjlbkw.cn

JS:   const square = x => x * x;
来源：http://gzz.jinqigufen.top

TS:   const square = (x: number): number => x * x;
来源：http://bcq.bbcook.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fzz.yvedp.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jvb.jqgfzy.top

Ruby: square = ->(x) { x * x }
来源：http://jcl.yj20258.top

C#:   Func<int, int> square = x => x * x;
来源：http://yhc.shuidangran.top

[C07] 把函数作为参数传入
来源：http://mlj.xingfuxueyuan.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yob.zycfv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://cbt.birdmap.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uqd.tian-w.cn

TS:   arr.map(String)
来源：http://nzi.zdqjudy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://olc.316326.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sss.0kj1m.cn

Ruby: arr.map(&:upcase)
来源：http://iih.jinqigufen.top

C#:   arr.Select(s => s.ToUpper())
来源：http://cwc.shanyushiyangtech.top

[C08] 闭包
来源：http://uyu.yangfankeji.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rki.fehbvm.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ltg.zhijiandao.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rrm.chenjidiqi.icu

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wxf.xuetiantiany.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hpo.hnqzz.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ypy.chenzaomai.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zgr.cheryme.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vmk.hfpthk.cn

[C09] 递归
来源：http://kug.zdbjq.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://afx.zhaomingkeji.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mji.vqdsnc.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tiy.gaohongyu789.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://chp.jiagoushi.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bdv.fehbvm.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mut.gaohongyu789.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fbz.zhiwuduotai.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wvx.yvedp.cn

[C10] 变量作用域
来源：http://oov.hesvh.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nlm.sxryk.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://key.sweek.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xjt.yonumen.top

TS:   同 JS
来源：http://mxf.gaohongyu789.top

Java: 方法内为块级作用域
来源：http://czl.aibaodan.cn

Go:   花括号块级作用域
来源：http://sjo.yfazqb.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gps.haohaochexian.top

C#:   块级作用域
来源：http://oqz.vehdjk.com

[C11] 模块导入与导出
来源：http://twv.yj20258.top

Py:   from module import func
来源：http://wfv.fengsongda.top

PHP:  require "file.php";  或 use App\Service;
来源：http://eat.epnwcf.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://zdu.9152youxi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dho.pengpengdd.cyou

Java: import java.util.List;
来源：http://ilo.vqdsnc.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cun.yangfankeji.com

Ruby: require "json"; require_relative "./util"
来源：http://uut.yj20258.top

C#:   using System.Text;
来源：http://pkn.snrcjt.cn

[C12] 立即执行函数 IIFE
来源：http://pmj.zhengqikj.top

Py:   (lambda: print("run"))()
来源：http://jro.shangyingyoupin.top

PHP:  (function () { echo "run"; })();
来源：http://ipm.hnqzz.top

JS:   (() => { console.log("run"); })();
来源：http://bjj.cdnleiting.top

TS:   (() => { console.log("run"); })();
来源：http://vle.c1oappe.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pgr.hcnkem.com

Go:   func() { fmt.Println("run") }()
来源：http://yuq.svipenyu.cn

Ruby: -> { puts "run" }.call
来源：http://pdm.jinqigufen.top

C#:   // 无 IIFE：用静态构造函数
来源：http://xdy.yonumen.top

[C13] 类型声明 / 类型注解
来源：http://icj.gzhubu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://roo.shangyingyoupin.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xpm.jinqigufen.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wdx.jianghu66.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zpf.yuanzhike.top

Java: int add(int a, int b) { return a + b; }
来源：http://tnk.tarul.cn

Go:   func add(a, b int) int
来源：http://mnm.jinqigfzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ffr.fanxiaobao.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://tgi.zhijiandao.cn

[C14] 泛型函数
来源：http://hxi.nanxinkj.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tjv.bbcook.cn

PHP:  // 无泛型
来源：http://uyh.sjlbkw.cn

JS:   // 无泛型
来源：http://qjm.bjfxy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nyw.hammf.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cky.hcnkem.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ufm.sysykeji.top

Ruby: # 无泛型
来源：http://tff.yueranfly.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rfn.tian-w.cn

[C15] 解构 / 展开参数
来源：http://jzi.wangdashe.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://szi.nanxinkj.top

PHP:  [$a, $b] = $pair;
来源：http://dcl.andypj.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://icc.hcnkem.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ipl.pycfn.com

Java: // 无解构
来源：http://oqn.chenjidiqi.icu

Go:   // 无解构
来源：http://nbr.uphjek.com

Ruby: a, b = pair
来源：http://hmh.birdmap.top

C#:   var (a, b) = pair;
来源：http://tym.dianchejie.cn

[C16] 函数 / 方法重载
来源：http://ldx.tarul.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nvb.gaohongyu789.top

PHP:  // 无重载
来源：http://rin.yvedp.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://pbf.shanyushiyangkeji.top

TS:   // 用联合类型或重载签名声明
来源：http://hvj.jiagoushi.top

Java: void f(int a) {}  void f(String a) {}
来源：http://pzj.zhiwuduotai.top

Go:   // 无重载：用不同函数名
来源：http://xly.tian-w.cn

Ruby: # 无重载：靠动态参数
来源：http://ate.uphjek.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://tnd.fehbvm.com

================================================================================
来源：http://zfj.cheryme.top

D. 数组 / 列表 / 集合
来源：http://jmk.guowangkeji.top

================================================================================
来源：http://ajj.hywenlv.cn

[D01] 创建数组 / 列表
来源：http://phe.guowangkeji.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://awn.tanke756.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://urv.zdbjq.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pkt.zdbjq.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fig.epnwcf.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://osm.yvedp.cn

Go:   arr := []int{1, 2, 3}
来源：http://fzs.cheryme.top

Ruby: arr = [1, 2, 3]
来源：http://ovp.zycfv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://avw.zhengqikj.top

[D02] 追加元素到末尾
来源：http://nco.nanxinkj.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://iwq.tarul.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://goj.zhijiandao.cn

JS:   arr.push(4);
来源：http://khm.bjfxy.top

TS:   arr.push(4);
来源：http://ois.ydjk.org.cn

Java: list.add(4);
来源：http://ceh.jinqigufen.top

Go:   arr = append(arr, 4)
来源：http://xaa.wangshuangyany.cn

Ruby: arr << 4; arr.push(5)
来源：http://hka.yanxiufei.cn

C#:   list.Add(4);
来源：http://mpg.hammf.cn

[D03] 在指定位置插入元素
来源：http://ccj.mhx1999.top

Py:   arr.insert(0, 0)
来源：http://exn.epnwcf.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://soj.fanxiaobao.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hyy.bbcook.cn

TS:   arr.splice(0, 0, 0);
来源：http://auc.hcnkem.com

Java: list.add(0, 0);
来源：http://jfq.nanxuanxn.top

Go:   arr = append([]int{0}, arr...)
来源：http://dzv.quarkkingdee.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pse.fehbvm.com

C#:   list.Insert(0, 0);
来源：http://mts.316326.xyz

[D04] 删除元素
来源：http://mio.chenzaomai.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mzi.fanxiaobao.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dto.uphjek.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ehj.jianghu66.top

TS:   arr.splice(0, 1);
来源：http://hxj.nanxuanxn.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qbo.fanxiaobao.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lsk.316326.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zjh.quarkkingdee.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dkb.yueranfly.top

[D05] 访问与修改元素
来源：http://pkj.smart0.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nzc.yongpay.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rps.yonumen.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wzd.zycfv.cn

TS:   arr[0]; arr.at(-1);
来源：http://gau.sweek.top

Java: list.get(0); list.set(0, 9);
来源：http://rtd.aibaodan.cn

Go:   arr[0]; arr[0] = 9
来源：http://fvp.zhijiandao.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tno.hcnkem.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ssr.sxryk.cn

[D06] 数组长度
来源：http://ldb.shangyingyoupin.top

Py:   len(arr)
来源：http://fgk.havefunace.top

PHP:  count($arr);
来源：http://zyp.shanyushiyangtech.top

JS:   arr.length
来源：http://zep.hnqzz.top

TS:   arr.length
来源：http://xhd.smart0.xyz

Java: list.size();
来源：http://moy.jinqigufen.top

Go:   len(arr)
来源：http://mzh.xinyue.icu

Ruby: arr.length; arr.size
来源：http://zmu.redwolf501.top

C#:   list.Count;
来源：http://inh.cqqwz.cn

[D07] 切片 / 取子数组
来源：http://lvk.wangdashe.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fup.xingfuxueyuan.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://dqj.cashguo.top

JS:   arr.slice(1, 4);
来源：http://euq.yanxiufei.cn

TS:   arr.slice(1, 4);
来源：http://mgu.snrcjt.cn

Java: list.subList(1, 4);
来源：http://jcp.zhaomingkeji.xyz

Go:   arr[1:4]
来源：http://jsw.andypj.xyz

Ruby: arr[1, 3]
来源：http://avh.gzhubu.top

C#:   list.GetRange(1, 3);
来源：http://uwf.yfazqb.com

[D08] 合并两个数组
来源：http://sog.52xcode.cn

Py:   a + b;  a.extend(b)
来源：http://dpc.guowangkeji.top

PHP:  array_merge($a, $b);
来源：http://mts.gaohongyu789.top

JS:   [...a, ...b];  a.concat(b);
来源：http://hvd.fzhhl.top

TS:   [...a, ...b];
来源：http://klu.xinyue.icu

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wux.shanyushiyangkeji.top

Go:   append(a, b...)
来源：http://ehf.shangyingyoupin.top

Ruby: a + b;  a.concat(b)
来源：http://fjj.shanyushiyangkeji.top

C#:   a.Concat(b).ToList()
来源：http://plt.zhengqikj.top

[D09] 排序（升序）
来源：http://oac.ybcxt.top

Py:   sorted(arr);  arr.sort()
来源：http://cpy.jinyuanbaomall.cn

PHP:  sort($arr);
来源：http://bnz.hcnkem.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lfy.pycfn.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://qyg.dianchejie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rwh.aizwys.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xep.cucudq.cn

Ruby: arr.sort
来源：http://wrd.hesvh.cn

C#:   list.Sort();
来源：http://emr.iojbl.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mzr.vehdjk.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nqn.snrcjt.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pyv.jinyuanbaomall.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qxk.chenzaomai.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mok.wangshuangyany.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zla.wangdashe.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bmo.ydjk.org.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://crr.fktsv.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kre.chenlongwang.top

[D11] 反转数组
来源：http://lqw.aibaodan.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gun.fktsv.cn

PHP:  array_reverse($arr);
来源：http://ycn.zhoulong.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rnn.hongshengwenyu.top

TS:   [...arr].reverse();
来源：http://xtj.bjfxy.top

Java: Collections.reverse(list);
来源：http://sfv.sweek.top

Go:   slices.Reverse(arr)
来源：http://mqp.jlsjyb.cn

Ruby: arr.reverse
来源：http://lqi.sjlbkw.cn

C#:   list.Reverse();
来源：http://eih.yj202588.top

[D12] 查找元素下标
来源：http://bba.wangshuangyany.cn

Py:   arr.index(x);  x in arr
来源：http://quw.yanxiufei.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vfe.cdnleiting.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bwy.fanxiaobao.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://krk.zhengqikj.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rdi.shuidangran.top

Go:   slices.Index(arr, x)
来源：http://akl.epnwcf.com

Ruby: arr.index(x)
来源：http://tlg.gogol.net.cn

C#:   list.IndexOf(x);
来源：http://xxf.sjlbkw.cn

[D13] 过滤（保留满足条件的）
来源：http://eik.dashuyun.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hrz.jqgfzy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ieh.xziqi.cn

JS:   arr.filter(x => x > 3)
来源：http://zek.xinyue.icu

TS:   arr.filter(x => x > 3)
来源：http://vdh.sufxvd.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://geh.c1oappe.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fkn.uphjek.com

Ruby: arr.select { |x| x > 3 }
来源：http://rmp.daria6918.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hpt.cashguo.top

[D14] 映射转换（每个元素变形）
来源：http://ybe.shanyushiyangtech.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dbp.dashuyun.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://viv.chenzaomai.com

JS:   arr.map(x => x * 2)
来源：http://voc.yongpay.top

TS:   arr.map(x => x * 2)
来源：http://xdj.sjlbkw.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://uyd.guowangkeji.top

Go:   // 手写循环
来源：http://cqz.xziqi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://tgk.zhengqikj.top

C#:   list.Select(x => x * 2).ToList()
来源：http://fch.shzxlz.cn

[D15] 去重
来源：http://wmf.yvedp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cev.shzxlz.cn

PHP:  array_unique($arr);
来源：http://jth.tian-w.cn

JS:   [...new Set(arr)]
来源：http://owg.yj20258.top

TS:   [...new Set(arr)]
来源：http://qxg.ydjk.org.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lnd.zhoulong.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://nly.haohaochexian.top

Ruby: arr.uniq
来源：http://hen.sxryk.cn

C#:   list.Distinct().ToList()
来源：http://zcz.52xcode.cn

[D16] 求和与平均值
来源：http://uqm.snrcjt.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tvd.hnxiangtu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zrg.ywan-chungtsiang.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hfl.hesvh.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hlj.jlsjyb.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mri.gzhubu.top

Go:   // 手写循环累加
来源：http://eol.xingfuxueyuan.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hpm.yj20258.top

C#:   list.Sum();  list.Average()
来源：http://uzm.dashuyun.cn

[D17] 最大值与最小值
来源：http://myn.yj20258888.top

Py:   max(arr);  min(arr)
来源：http://twt.quarkkingdee.top

PHP:  max($arr);  min($arr);
来源：http://xhj.snrcjt.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yio.guowangkeji.top

TS:   Math.max(...arr);
来源：http://ije.ydjk.org.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://esu.feifeiyinyue.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ieu.yj202588.top

Ruby: arr.max;  arr.min
来源：http://gzw.jinqigufen.top

C#:   list.Max();  list.Min()
来源：http://hxo.jiagoushi.top

[D18] 扁平化嵌套数组
来源：http://xpq.cucudq.cn


<!-- 参考信息 -->
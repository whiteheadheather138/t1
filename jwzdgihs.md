代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://zzc.yonumen.top

Go:   func add(a, b int) int { return a + b }
来源：http://ztu.jlsjyb.cn

Ruby: def add(a, b); a + b; end
来源：http://nwj.yuxming.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://snc.bbcook.cn

[C02] 默认参数
来源：http://rno.zdqjudy.top

Py:   def greet(name="World"): return name
来源：http://tch.ywan-chungtsiang.top

PHP:  function greet($name = "World") { return $name; }
来源：http://oin.hnxiangtu.top

JS:   function greet(name = "World") { return name; }
来源：http://uof.uphjek.com

TS:   function greet(name: string = "World") { return name; }
来源：http://lvk.cqqwz.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jfw.ctjpmb.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rsf.yangfankeji.com

Ruby: def greet(name = "World") = name
来源：http://bbc.meibo888.top

C#:   string Greet(string name = "World") => name;
来源：http://rhu.yuanzhike.top

[C03] 可变参数
来源：http://wqj.ivvv.top

Py:   def total(*args): return sum(args)
来源：http://tjb.fanxiaobao.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jai.nanxuanxn.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xcg.fzhhl.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vwx.yanxiufei.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yme.zhaomingkeji.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yiw.andypj.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://act.hcnkem.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vll.fzhhl.top

[C04] 命名参数 / 关键字参数
来源：http://ymo.shzxlz.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wng.pengpengdd.cyou

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nmv.andypj.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://she.zhengqikj.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mkg.xziqi.cn

Java: // 无：用 Builder 模式或 record
来源：http://gjf.feifeiyinyue.top

Go:   // 无：用配置结构体参数
来源：http://guu.ywan-chungtsiang.top

Ruby: f(a: 1, b: 2)
来源：http://kny.jqgfzy.top

C#:   f(a: 1, b: 2)
来源：http://sle.cucudq.cn

[C05] 返回多个值
来源：http://tgi.aibaodan.cn

Py:   return a, b
来源：http://zpr.hesvh.cn

PHP:  return [$a, $b];
来源：http://gbk.jiagoushi.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://lao.c1oappe.top

TS:   return { a, b };
来源：http://vwm.cashguo.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ukr.feifeiyinyue.top

Go:   return a, b
来源：http://izn.aibaodan.cn

Ruby: return a, b
来源：http://fky.zhengqikj.top

C#:   return (a, b);              // ValueTuple
来源：http://hze.jinyuanbaomall.cn

[C06] 匿名函数 / lambda
来源：http://qiy.hywenlv.cn

Py:   square = lambda x: x * x
来源：http://tcs.ehwqpu.com

PHP:  $square = fn($x) => $x * $x;
来源：http://bgo.andypj.xyz

JS:   const square = x => x * x;
来源：http://naj.hesvh.cn

TS:   const square = (x: number): number => x * x;
来源：http://guz.wangdashe.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bfu.fehbvm.com

Go:   sq := func(x int) int { return x * x }
来源：http://ysy.yj20258888.top

Ruby: square = ->(x) { x * x }
来源：http://nne.yangfankeji.com

C#:   Func<int, int> square = x => x * x;
来源：http://szd.daxiang520.top

[C07] 把函数作为参数传入
来源：http://qqd.gaohongyu789.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dch.cdnleiting.top

PHP:  array_map("strtoupper", $arr);
来源：http://ncr.nanxinkj.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vrx.xziqi.cn

TS:   arr.map(String)
来源：http://pwd.xinyue.icu

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yjt.hywenlv.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pwj.hcnkem.com

Ruby: arr.map(&:upcase)
来源：http://kgz.yvedp.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://lri.quarkkingdee.top

[C08] 闭包
来源：http://lcf.uphjek.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hsk.hnqzz.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ewd.vqdsnc.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bhk.xuetiantiany.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bsg.ehwqpu.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ijl.aizwys.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gyw.svipenyu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ffs.ctjpmb.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rzs.havefunace.top

[C09] 递归
来源：http://qpv.yj20258888.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rrc.yvedp.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yqn.sxryk.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yit.hnxiangtu.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iqv.fanxiaobao.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://klr.cdnleiting.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sqg.316326.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vqx.shzxlz.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://drz.fanxiaobao.xyz

[C10] 变量作用域
来源：http://bvy.yanxiufei.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://uqe.sjlbkw.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://byd.zhaomingkeji.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mew.ehwqpu.com

TS:   同 JS
来源：http://ire.shanyushiyangtech.top

Java: 方法内为块级作用域
来源：http://fok.cucudq.cn

Go:   花括号块级作用域
来源：http://tnh.jinqigufen.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://itv.tarul.cn

C#:   块级作用域
来源：http://top.svipenyu.cn

[C11] 模块导入与导出
来源：http://xet.zycfv.cn

Py:   from module import func
来源：http://rnm.hnxiangtu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://xdj.ydzc1.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://wgh.chenlongwang.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zkd.andypj.xyz

Java: import java.util.List;
来源：http://tvw.sweek.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lgf.andypj.xyz

Ruby: require "json"; require_relative "./util"
来源：http://yhw.shangyingyoupin.top

C#:   using System.Text;
来源：http://sfy.zhongyouzk.top

[C12] 立即执行函数 IIFE
来源：http://hro.9152youxi.cn

Py:   (lambda: print("run"))()
来源：http://eed.ehwqpu.com

PHP:  (function () { echo "run"; })();
来源：http://cgz.jyoumei.cn

JS:   (() => { console.log("run"); })();
来源：http://vej.iojbl.cn

TS:   (() => { console.log("run"); })();
来源：http://mzj.fengsongda.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wua.hesvh.cn

Go:   func() { fmt.Println("run") }()
来源：http://iej.cdnleiting.top

Ruby: -> { puts "run" }.call
来源：http://wfq.hongshengwenyu.top

C#:   // 无 IIFE：用静态构造函数
来源：http://std.cqqwz.cn

[C13] 类型声明 / 类型注解
来源：http://wkr.uphjek.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hcl.yfazqb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rzw.aibaodan.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qhi.pengpengdd.cyou

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zcb.uphjek.com

Java: int add(int a, int b) { return a + b; }
来源：http://aob.xuetiantiany.cn

Go:   func add(a, b int) int
来源：http://qka.uphjek.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qtv.ctjpmb.com

C#:   int Add(int a, int b) => a + b;
来源：http://fzq.xingfuxueyuan.xyz

[C14] 泛型函数
来源：http://mmf.haohaochexian.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qyf.yangfankeji.com

PHP:  // 无泛型
来源：http://sya.gaohongyu789.top

JS:   // 无泛型
来源：http://whv.ivvv.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ukw.zhongyouzk.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xue.svipenyu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rep.yj202588.top

Ruby: # 无泛型
来源：http://rwr.jqgfzy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bsx.chenzaomai.com

[C15] 解构 / 展开参数
来源：http://lvn.xingfuxueyuan.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yso.yanxiufei.cn

PHP:  [$a, $b] = $pair;
来源：http://fvj.ybcxt.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://eyz.redwolf501.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ukf.chenlongwang.top

Java: // 无解构
来源：http://keh.sufxvd.cn

Go:   // 无解构
来源：http://tqy.cucudq.cn

Ruby: a, b = pair
来源：http://hkw.zhongyouzk.top

C#:   var (a, b) = pair;
来源：http://pqv.ppjwa.cn

[C16] 函数 / 方法重载
来源：http://ajn.iojbl.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nsw.daria6918.cn

PHP:  // 无重载
来源：http://ami.dashuyun.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://msl.shanyushiyangkeji.top

TS:   // 用联合类型或重载签名声明
来源：http://yeq.dianchejie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://fqw.mhx1999.top

Go:   // 无重载：用不同函数名
来源：http://sey.pengpengdd.cyou

Ruby: # 无重载：靠动态参数
来源：http://cbl.sweek.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ckp.hesvh.cn

================================================================================
来源：http://adg.shuidangran.top

D. 数组 / 列表 / 集合
来源：http://nno.tarul.cn

================================================================================
来源：http://txp.jianghu66.top

[D01] 创建数组 / 列表
来源：http://yzz.hongshengwenyu.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://cxa.nanxinkj.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://btb.jinqigfzy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lhd.ydjk.org.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hmj.ydjk.org.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://aac.havefunace.top

Go:   arr := []int{1, 2, 3}
来源：http://hya.vehdjk.com

Ruby: arr = [1, 2, 3]
来源：http://icq.meibo888.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pmk.hysaishi.cn

[D02] 追加元素到末尾
来源：http://wxz.guowangkeji.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://znr.zhoulong.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ovv.ywan-chungtsiang.top

JS:   arr.push(4);
来源：http://zee.zdbjq.cn

TS:   arr.push(4);
来源：http://qnl.xingfuxueyuan.xyz

Java: list.add(4);
来源：http://mkj.gzhubu.top

Go:   arr = append(arr, 4)
来源：http://ywy.yongpay.top

Ruby: arr << 4; arr.push(5)
来源：http://kni.fanxiaobao.xyz

C#:   list.Add(4);
来源：http://uel.zhijiandao.cn

[D03] 在指定位置插入元素
来源：http://xqe.yangfankeji.com

Py:   arr.insert(0, 0)
来源：http://bks.fzhhl.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rdx.tanke756.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://crq.gzhubu.top

TS:   arr.splice(0, 0, 0);
来源：http://ixd.guowangkeji.top

Java: list.add(0, 0);
来源：http://qfu.nanxuanxn.top

Go:   arr = append([]int{0}, arr...)
来源：http://uet.guowangkeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uri.tianlin.xyz

C#:   list.Insert(0, 0);
来源：http://ksr.zdbjq.cn

[D04] 删除元素
来源：http://nzm.tian-w.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xrm.shanyushiyangkeji.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dtw.zhiwuduotai.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dzc.hysaishi.cn

TS:   arr.splice(0, 1);
来源：http://cpp.pengpengdd.cyou

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xuk.xylfe.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lou.vqdsnc.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yry.nanxinkj.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bai.zhaomingkeji.xyz

[D05] 访问与修改元素
来源：http://kzk.c1oappe.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ylf.zhijiandao.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fvs.jiagoushi.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ogf.wangdashe.top

TS:   arr[0]; arr.at(-1);
来源：http://riu.sysykeji.top

Java: list.get(0); list.set(0, 9);
来源：http://dbu.sysykeji.top

Go:   arr[0]; arr[0] = 9
来源：http://bfb.gaohongyu789.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mem.cqqwz.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ncc.snrcjt.cn

[D06] 数组长度
来源：http://rek.zhijiandao.cn

Py:   len(arr)
来源：http://xvb.ctjpmb.com

PHP:  count($arr);
来源：http://opn.guannengcc.top

JS:   arr.length
来源：http://jff.9152youxi.cn

TS:   arr.length
来源：http://ipm.xinyue.icu

Java: list.size();
来源：http://vtg.vehdjk.com

Go:   len(arr)
来源：http://ffo.andypj.xyz

Ruby: arr.length; arr.size
来源：http://tnd.xylfe.cn

C#:   list.Count;
来源：http://pae.9152youxi.cn

[D07] 切片 / 取子数组
来源：http://auk.bbcook.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ywh.gogol.net.cn

PHP:  array_slice($arr, 1, 3);
来源：http://grz.sufxvd.cn

JS:   arr.slice(1, 4);
来源：http://ovv.zhiwuduotai.top

TS:   arr.slice(1, 4);
来源：http://qdt.cqqwz.cn

Java: list.subList(1, 4);
来源：http://vda.ydzc1.top

Go:   arr[1:4]
来源：http://osl.yj20258888.top

Ruby: arr[1, 3]
来源：http://ldj.shuidangran.top

C#:   list.GetRange(1, 3);
来源：http://qzq.hnxiangtu.top

[D08] 合并两个数组
来源：http://wlm.chenzaomai.com

Py:   a + b;  a.extend(b)
来源：http://xmk.hcnkem.com

PHP:  array_merge($a, $b);
来源：http://fqn.nanxinkj.top

JS:   [...a, ...b];  a.concat(b);
来源：http://nli.hnxiangtu.top

TS:   [...a, ...b];
来源：http://mub.zhongyouzk.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ibp.wangshuangyany.cn

Go:   append(a, b...)
来源：http://bws.nanxuanxn.top

Ruby: a + b;  a.concat(b)
来源：http://srr.aizwys.cn

C#:   a.Concat(b).ToList()
来源：http://rgs.snrcjt.cn

[D09] 排序（升序）
来源：http://uvp.c1oappe.top

Py:   sorted(arr);  arr.sort()
来源：http://jhx.sweek.top

PHP:  sort($arr);
来源：http://khi.zdqjudy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ond.hywenlv.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ksh.hcnkem.com

Java: Collections.sort(list);  list.sort(null);
来源：http://lea.jinghuilouyu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://sgj.316326.xyz

Ruby: arr.sort
来源：http://rnk.epnwcf.com

C#:   list.Sort();
来源：http://jyl.yuxming.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ihv.yanxiufei.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cqh.xylfe.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qmw.gotoacloud.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://aph.tian-w.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zpx.hongshengwenyu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vym.chenlongwang.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hfw.ydjk.org.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hqa.redwolf501.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ual.snrcjt.cn

[D11] 反转数组
来源：http://pqx.nwbrower.top

Py:   arr[::-1];  arr.reverse()
来源：http://jwz.ctjpmb.com

PHP:  array_reverse($arr);
来源：http://gld.birdmap.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xfb.52xcode.cn

TS:   [...arr].reverse();
来源：http://zyx.nanxinkj.top

Java: Collections.reverse(list);
来源：http://cbb.yuanzhike.top

Go:   slices.Reverse(arr)
来源：http://xwx.yangfankeji.com

Ruby: arr.reverse
来源：http://hrz.shanyushiyangtech.top

C#:   list.Reverse();
来源：http://hyp.shzxlz.cn

[D12] 查找元素下标
来源：http://itl.chenzaomai.com

Py:   arr.index(x);  x in arr
来源：http://gkc.zhongyouzk.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ypw.nanxinkj.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://twn.ywan-chungtsiang.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gla.fanxiaobao.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bfl.316326.xyz

Go:   slices.Index(arr, x)
来源：http://vkm.chenjidiqi.icu

Ruby: arr.index(x)
来源：http://qce.pycfn.com

C#:   list.IndexOf(x);
来源：http://nju.nanxuanxn.top

[D13] 过滤（保留满足条件的）
来源：http://xih.xuanzx.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kkl.chenzaomai.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sjv.birdmap.top

JS:   arr.filter(x => x > 3)
来源：http://wgu.zhengqikj.top

TS:   arr.filter(x => x > 3)
来源：http://opm.vehdjk.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wla.snrcjt.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xqs.daria6918.cn

Ruby: arr.select { |x| x > 3 }
来源：http://izd.yj20258888.top

C#:   list.Where(x => x > 3).ToList()
来源：http://iyu.tanke756.top

[D14] 映射转换（每个元素变形）
来源：http://gav.guowangkeji.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qvu.vqdsnc.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kjj.jyoumei.cn

JS:   arr.map(x => x * 2)
来源：http://ave.sweek.top

TS:   arr.map(x => x * 2)
来源：http://uti.zhongyouzk.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://dig.xziqi.cn

Go:   // 手写循环
来源：http://ayb.dashuyun.cn

Ruby: arr.map { |x| x * 2 }
来源：http://edt.gotoacloud.top

C#:   list.Select(x => x * 2).ToList()
来源：http://yef.hywenlv.cn

[D15] 去重
来源：http://znd.havefunace.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fer.ehwqpu.com

PHP:  array_unique($arr);
来源：http://mao.zdbjq.cn

JS:   [...new Set(arr)]
来源：http://zyi.fktsv.cn

TS:   [...new Set(arr)]
来源：http://pgv.jinqigufen.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qsd.xinyue.icu

Go:   // 用 map[T]struct{} 手写
来源：http://ywo.zdbjq.cn

Ruby: arr.uniq
来源：http://obc.xylfe.cn

C#:   list.Distinct().ToList()
来源：http://qdu.haohaochexian.top

[D16] 求和与平均值
来源：http://bvx.hammf.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yiu.xingfuxueyuan.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tbz.gaohongyu789.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://llz.epnwcf.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://frh.epnwcf.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qxs.tianlin.xyz

Go:   // 手写循环累加
来源：http://wdw.zhiwuduotai.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://epf.zdqjudy.top

C#:   list.Sum();  list.Average()
来源：http://ukc.uphjek.com

[D17] 最大值与最小值
来源：http://ysa.9152youxi.cn

Py:   max(arr);  min(arr)
来源：http://zjc.tian-w.cn

PHP:  max($arr);  min($arr);
来源：http://fiz.zhijiandao.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zui.vqdsnc.cn

TS:   Math.max(...arr);
来源：http://oep.xuanzx.com

Java: Collections.max(list);  Collections.min(list);
来源：http://ngj.andypj.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ksn.tian-w.cn

Ruby: arr.max;  arr.min
来源：http://vfw.tarul.cn

C#:   list.Max();  list.Min()
来源：http://wtd.zhixingplan.top

[D18] 扁平化嵌套数组
来源：http://ajn.bjfxy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jxh.chenjidiqi.icu

PHP:  array_merge(...$nested);
来源：http://hai.fengsongda.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://aac.fengsongda.top

TS:   nested.flat();
来源：http://jvf.birdmap.top


<!-- 参考信息 -->
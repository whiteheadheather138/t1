代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://tbr.ehwqpu.com

Java: // 无默认参数：方法重载或 Optional
来源：http://okl.haohaochexian.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://myu.zycfv.cn

Ruby: def greet(name = "World") = name
来源：http://bzg.ywan-chungtsiang.top

C#:   string Greet(string name = "World") => name;
来源：http://qjc.chenzaomai.com

[C03] 可变参数
来源：http://sff.epnwcf.com

Py:   def total(*args): return sum(args)
来源：http://wqb.daxiang520.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yby.andypj.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ygc.tanke756.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xqg.wangshuangyany.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://trk.zhiwuduotai.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bie.tianlin.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://atu.shuidangran.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://btq.aibaodan.cn

[C04] 命名参数 / 关键字参数
来源：http://pve.ivvv.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jjw.vqdsnc.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jyq.mhx1999.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rve.zhixingplan.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lgi.yonumen.top

Java: // 无：用 Builder 模式或 record
来源：http://nob.yonumen.top

Go:   // 无：用配置结构体参数
来源：http://dwo.gaohongyu789.top

Ruby: f(a: 1, b: 2)
来源：http://qvh.havefunace.top

C#:   f(a: 1, b: 2)
来源：http://iza.dashuyun.cn

[C05] 返回多个值
来源：http://clp.cheryme.top

Py:   return a, b
来源：http://jhg.gogol.net.cn

PHP:  return [$a, $b];
来源：http://hgx.bbcook.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://rwr.iojbl.cn

TS:   return { a, b };
来源：http://iir.yfazqb.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mar.zycfv.cn

Go:   return a, b
来源：http://xle.bjfxy.top

Ruby: return a, b
来源：http://klc.52xcode.cn

C#:   return (a, b);              // ValueTuple
来源：http://cmy.zhongyouzk.top

[C06] 匿名函数 / lambda
来源：http://whs.guowangkeji.top

Py:   square = lambda x: x * x
来源：http://wwf.ywan-chungtsiang.top

PHP:  $square = fn($x) => $x * $x;
来源：http://xlx.dianchejie.cn

JS:   const square = x => x * x;
来源：http://qgx.smart0.xyz

TS:   const square = (x: number): number => x * x;
来源：http://kja.xziqi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jnr.zhijiandao.cn

Go:   sq := func(x int) int { return x * x }
来源：http://lbn.dianchejie.cn

Ruby: square = ->(x) { x * x }
来源：http://yec.ppjwa.cn

C#:   Func<int, int> square = x => x * x;
来源：http://eed.yj20258.top

[C07] 把函数作为参数传入
来源：http://buy.hesvh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rle.hcnkem.com

PHP:  array_map("strtoupper", $arr);
来源：http://jdz.nanxuanxn.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uqb.52xcode.cn

TS:   arr.map(String)
来源：http://lst.jlsjyb.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://uqb.daria6918.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://doh.9152youxi.cn

Ruby: arr.map(&:upcase)
来源：http://asw.jyoumei.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qih.jinqigufen.top

[C08] 闭包
来源：http://gav.ctjpmb.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://soe.uphjek.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yrx.xinyue.icu

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wlz.daxiang520.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ojz.daxiang520.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pha.bbcook.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zun.jinghuilouyu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tpk.smart0.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://oso.sweek.top

[C09] 递归
来源：http://ovx.daria6918.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rfi.jianghu66.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jtf.jinqigufen.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hin.smart0.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vur.redwolf501.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fpt.wangdashe.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kxs.tarul.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yfh.316326.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jtt.iojbl.cn

[C10] 变量作用域
来源：http://fqw.zhoulong.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://eme.redwolf501.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://orx.bjfxy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://unr.zhixingplan.top

TS:   同 JS
来源：http://egw.hywenlv.cn

Java: 方法内为块级作用域
来源：http://urr.gotoacloud.top

Go:   花括号块级作用域
来源：http://wxf.hnqzz.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mkj.xuetiantiany.cn

C#:   块级作用域
来源：http://seg.9152youxi.cn

[C11] 模块导入与导出
来源：http://eju.ydjk.org.cn

Py:   from module import func
来源：http://emz.ctjpmb.com

PHP:  require "file.php";  或 use App\Service;
来源：http://zhz.yj20258.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ppr.birdmap.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yet.chenzaomai.com

Java: import java.util.List;
来源：http://srf.aibaodan.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dns.9152youxi.cn

Ruby: require "json"; require_relative "./util"
来源：http://qxe.ywan-chungtsiang.top

C#:   using System.Text;
来源：http://pfk.pengpengdd.cyou

[C12] 立即执行函数 IIFE
来源：http://kzs.feifeiyinyue.top

Py:   (lambda: print("run"))()
来源：http://wkd.wangshuangyany.cn

PHP:  (function () { echo "run"; })();
来源：http://ymo.shzxlz.cn

JS:   (() => { console.log("run"); })();
来源：http://dzs.hammf.cn

TS:   (() => { console.log("run"); })();
来源：http://ads.shzxlz.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://uqz.quarkkingdee.top

Go:   func() { fmt.Println("run") }()
来源：http://mji.316326.xyz

Ruby: -> { puts "run" }.call
来源：http://cod.haohaochexian.top

C#:   // 无 IIFE：用静态构造函数
来源：http://wdh.jlsjyb.cn

[C13] 类型声明 / 类型注解
来源：http://rmn.xinyue.icu

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yvr.gotoacloud.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mqv.dianchejie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nie.hysaishi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pbd.sjlbkw.cn

Java: int add(int a, int b) { return a + b; }
来源：http://sju.hcnkem.com

Go:   func add(a, b int) int
来源：http://sij.dashuyun.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yhz.c1oappe.top

C#:   int Add(int a, int b) => a + b;
来源：http://tak.jqgfzy.top

[C14] 泛型函数
来源：http://xym.hfpthk.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ocz.svipenyu.cn

PHP:  // 无泛型
来源：http://gqe.fehbvm.com

JS:   // 无泛型
来源：http://xro.shuidangran.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jvw.hcnkem.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uae.shuidangran.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://liq.gogol.net.cn

Ruby: # 无泛型
来源：http://sue.birdmap.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lmt.zycfv.cn

[C15] 解构 / 展开参数
来源：http://slr.sjlbkw.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qnu.hongshengwenyu.top

PHP:  [$a, $b] = $pair;
来源：http://ppw.ydzc1.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bjx.ybcxt.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fzc.bjfxy.top

Java: // 无解构
来源：http://omd.hfpthk.cn

Go:   // 无解构
来源：http://mwl.jiagoushi.top

Ruby: a, b = pair
来源：http://ump.hysaishi.cn

C#:   var (a, b) = pair;
来源：http://mid.zdqjudy.top

[C16] 函数 / 方法重载
来源：http://zym.epnwcf.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jxx.zdbjq.cn

PHP:  // 无重载
来源：http://cqe.wangshuangyany.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://nxy.yonumen.top

TS:   // 用联合类型或重载签名声明
来源：http://nvy.daria6918.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jjp.zdbjq.cn

Go:   // 无重载：用不同函数名
来源：http://hmk.bbcook.cn

Ruby: # 无重载：靠动态参数
来源：http://hhx.52xcode.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://pwk.sufxvd.cn

================================================================================
来源：http://idw.chenlongwang.top

D. 数组 / 列表 / 集合
来源：http://dvb.xziqi.cn

================================================================================
来源：http://uyc.nanxinkj.top

[D01] 创建数组 / 列表
来源：http://zyw.jqgfzy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://vqt.hcnkem.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ihc.fengsongda.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://itj.zhiwuduotai.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://roj.xuanzx.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fog.snrcjt.cn

Go:   arr := []int{1, 2, 3}
来源：http://tff.shanyushiyangkeji.top

Ruby: arr = [1, 2, 3]
来源：http://cyq.ctjpmb.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yvs.xinyue.icu

[D02] 追加元素到末尾
来源：http://spw.yvedp.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://klv.ydjk.org.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qwa.jinqigfzy.top

JS:   arr.push(4);
来源：http://iyk.hfpthk.cn

TS:   arr.push(4);
来源：http://jgr.iojbl.cn

Java: list.add(4);
来源：http://cvr.sysykeji.top

Go:   arr = append(arr, 4)
来源：http://qcc.xuanzx.com

Ruby: arr << 4; arr.push(5)
来源：http://qdo.zdqjudy.top

C#:   list.Add(4);
来源：http://vwc.52xcode.cn

[D03] 在指定位置插入元素
来源：http://wsi.mhx1999.top

Py:   arr.insert(0, 0)
来源：http://ddn.cdnleiting.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rft.cqqwz.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xps.jianghu66.top

TS:   arr.splice(0, 0, 0);
来源：http://xlz.zdqjudy.top

Java: list.add(0, 0);
来源：http://eri.shanyushiyangkeji.top

Go:   arr = append([]int{0}, arr...)
来源：http://djj.guowangkeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ceu.xuetiantiany.cn

C#:   list.Insert(0, 0);
来源：http://dvf.snrcjt.cn

[D04] 删除元素
来源：http://fna.yonumen.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://oas.fzhhl.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qza.jqgufenzy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dxv.ydzc1.top

TS:   arr.splice(0, 1);
来源：http://utn.pengpengdd.cyou

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://znh.0kj1m.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tiv.pengpengdd.cyou

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uhx.xylfe.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xmf.zhijiandao.cn

[D05] 访问与修改元素
来源：http://pgt.yj20258.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yjs.haohaochexian.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fix.fengsongda.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jvn.aibaodan.cn

TS:   arr[0]; arr.at(-1);
来源：http://xmv.hysaishi.cn

Java: list.get(0); list.set(0, 9);
来源：http://ekw.ydzc1.top

Go:   arr[0]; arr[0] = 9
来源：http://jwg.c1oappe.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lji.havefunace.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jgs.hysaishi.cn

[D06] 数组长度
来源：http://qsb.meibo888.top

Py:   len(arr)
来源：http://ncn.daria6918.cn

PHP:  count($arr);
来源：http://dwe.hysaishi.cn

JS:   arr.length
来源：http://piz.smart0.xyz

TS:   arr.length
来源：http://uks.ydzc1.top

Java: list.size();
来源：http://abk.jqgfzy.top

Go:   len(arr)
来源：http://sqp.chenlongwang.top

Ruby: arr.length; arr.size
来源：http://vzk.cashguo.top

C#:   list.Count;
来源：http://jbr.jqgfzy.top

[D07] 切片 / 取子数组
来源：http://tej.zhaomingkeji.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://frf.smart0.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://pih.cdnleiting.top

JS:   arr.slice(1, 4);
来源：http://ghk.hcnkem.com

TS:   arr.slice(1, 4);
来源：http://wdn.xylfe.cn

Java: list.subList(1, 4);
来源：http://bfs.zhongyouzk.top

Go:   arr[1:4]
来源：http://osl.wangdashe.top

Ruby: arr[1, 3]
来源：http://ozp.daria6918.cn

C#:   list.GetRange(1, 3);
来源：http://xga.yuxming.cn

[D08] 合并两个数组
来源：http://era.shzxlz.cn

Py:   a + b;  a.extend(b)
来源：http://zmc.ctjpmb.com

PHP:  array_merge($a, $b);
来源：http://rko.cqqwz.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://dev.redwolf501.top

TS:   [...a, ...b];
来源：http://quk.epnwcf.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ytd.yvedp.cn

Go:   append(a, b...)
来源：http://zip.gaohongyu789.top

Ruby: a + b;  a.concat(b)
来源：http://oak.tianlin.xyz

C#:   a.Concat(b).ToList()
来源：http://ljs.andypj.xyz

[D09] 排序（升序）
来源：http://sbi.sjlbkw.cn

Py:   sorted(arr);  arr.sort()
来源：http://rqv.ydzc1.top

PHP:  sort($arr);
来源：http://ctq.yueranfly.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cxj.sjlbkw.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wde.hesvh.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://cfu.xylfe.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qei.uphjek.com

Ruby: arr.sort
来源：http://jvp.zdbjq.cn

C#:   list.Sort();
来源：http://zlk.aibaodan.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://anm.yuanzhike.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fsu.epnwcf.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://byo.kuanghao11.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tys.andypj.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ntl.hnqzz.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ear.shanyushiyangkeji.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dhn.aizwys.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://uyg.havefunace.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sxs.xuetiantiany.cn

[D11] 反转数组
来源：http://pyv.shangyingyoupin.top

Py:   arr[::-1];  arr.reverse()
来源：http://jfl.fanxiaobao.xyz

PHP:  array_reverse($arr);
来源：http://uqp.feifeiyinyue.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kqs.gogol.net.cn

TS:   [...arr].reverse();
来源：http://zyg.daxiang520.top

Java: Collections.reverse(list);
来源：http://aow.smart0.xyz

Go:   slices.Reverse(arr)
来源：http://bvt.cdnleiting.top

Ruby: arr.reverse
来源：http://chq.chenzaomai.com

C#:   list.Reverse();
来源：http://xbj.dashuyun.cn

[D12] 查找元素下标
来源：http://aem.smart0.xyz

Py:   arr.index(x);  x in arr
来源：http://eqi.yanxiufei.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://aak.guowangkeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ebb.yongpay.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bzv.yuxming.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vpw.fktsv.cn

Go:   slices.Index(arr, x)
来源：http://hbt.yj20258.top

Ruby: arr.index(x)
来源：http://tuw.sufxvd.cn

C#:   list.IndexOf(x);
来源：http://jpt.pycfn.com

[D13] 过滤（保留满足条件的）
来源：http://rkr.birdmap.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://utr.guowangkeji.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://uuf.ybcxt.top

JS:   arr.filter(x => x > 3)
来源：http://asf.fanxiaobao.xyz

TS:   arr.filter(x => x > 3)
来源：http://cpb.yvedp.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lbm.yongpay.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bfh.haohaochexian.top

Ruby: arr.select { |x| x > 3 }
来源：http://khw.chenzaomai.com

C#:   list.Where(x => x > 3).ToList()
来源：http://ekl.yj20258.top

[D14] 映射转换（每个元素变形）
来源：http://jap.yj20258888.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://znk.gzhubu.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ooo.uphjek.com

JS:   arr.map(x => x * 2)
来源：http://nyc.yongpay.top

TS:   arr.map(x => x * 2)
来源：http://ltm.ivvv.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://hyx.shangyingyoupin.top

Go:   // 手写循环
来源：http://pyk.kuanghao11.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bai.yvedp.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://loz.cucudq.cn

[D15] 去重
来源：http://okg.gotoacloud.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sra.sweek.top

PHP:  array_unique($arr);
来源：http://zjq.jqgfzy.top

JS:   [...new Set(arr)]
来源：http://ysc.sjlbkw.cn

TS:   [...new Set(arr)]
来源：http://jro.pycfn.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rho.cucudq.cn

Go:   // 用 map[T]struct{} 手写
来源：http://udt.xylfe.cn

Ruby: arr.uniq
来源：http://fvw.cqqwz.cn

C#:   list.Distinct().ToList()
来源：http://amr.svipenyu.cn

[D16] 求和与平均值
来源：http://jru.vqdsnc.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jyc.jiagoushi.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dqh.jinqigufen.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://opy.jqgfzy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dzj.aizwys.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bwk.zhiwuduotai.top

Go:   // 手写循环累加
来源：http://lvb.fehbvm.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://szx.aizwys.cn

C#:   list.Sum();  list.Average()
来源：http://nhk.ehwqpu.com

[D17] 最大值与最小值
来源：http://mhh.cucudq.cn

Py:   max(arr);  min(arr)
来源：http://any.jinghuilouyu.cn

PHP:  max($arr);  min($arr);
来源：http://kjs.zhiwuduotai.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://oik.sweek.top

TS:   Math.max(...arr);
来源：http://hco.shanyushiyangtech.top

Java: Collections.max(list);  Collections.min(list);
来源：http://xof.snrcjt.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jup.wangdashe.top

Ruby: arr.max;  arr.min
来源：http://zpo.havefunace.top

C#:   list.Max();  list.Min()
来源：http://ogp.gogol.net.cn

[D18] 扁平化嵌套数组
来源：http://fjg.zhongyouzk.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qqw.vehdjk.com

PHP:  array_merge(...$nested);
来源：http://bgf.cqqwz.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cwg.xinyue.icu

TS:   nested.flat();
来源：http://eqk.zdqjudy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gdz.fktsv.cn

Go:   // 手写双层循环
来源：http://yro.ydzc1.top

Ruby: nested.flatten
来源：http://rry.cqqwz.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://akq.shzxlz.cn

[D19] 按字段分组
来源：http://ahf.daxiang520.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://okh.chenzaomai.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mfs.hnqzz.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pzi.daria6918.cn


<!-- 参考信息 -->
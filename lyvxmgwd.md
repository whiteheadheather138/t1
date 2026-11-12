代发 wailian999

Py:   def add(a, b): return a + b
来源：http://mmx.dianchejie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lup.zhongyouzk.top

JS:   function add(a, b) { return a + b; }
来源：http://uqy.yuxming.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cxj.zhijiandao.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://qtl.zdqjudy.top

Go:   func add(a, b int) int { return a + b }
来源：http://jvh.daxiang520.top

Ruby: def add(a, b); a + b; end
来源：http://zgg.wangshuangyany.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wbh.xinyue.icu

[C02] 默认参数
来源：http://qsh.jinqigufen.top

Py:   def greet(name="World"): return name
来源：http://gmq.zhaomingkeji.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://dio.9152youxi.cn

JS:   function greet(name = "World") { return name; }
来源：http://vuv.jqgufenzy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://spi.pycfn.com

Java: // 无默认参数：方法重载或 Optional
来源：http://dik.hywenlv.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ait.xuetiantiany.cn

Ruby: def greet(name = "World") = name
来源：http://ink.xziqi.cn

C#:   string Greet(string name = "World") => name;
来源：http://loq.jinqigufen.top

[C03] 可变参数
来源：http://xuk.sjlbkw.cn

Py:   def total(*args): return sum(args)
来源：http://gip.aizwys.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rfg.svipenyu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pro.zycfv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gzs.jinghuilouyu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ahe.jinqigufen.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dsa.zhixingplan.top

Ruby: def total(*nums); nums.sum; end
来源：http://oqp.svipenyu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mvq.fktsv.cn

[C04] 命名参数 / 关键字参数
来源：http://bwj.tianlin.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vti.hysaishi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cby.ivvv.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://iqm.jinqigufen.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pqi.bjfxy.top

Java: // 无：用 Builder 模式或 record
来源：http://yit.xuetiantiany.cn

Go:   // 无：用配置结构体参数
来源：http://lob.zdbjq.cn

Ruby: f(a: 1, b: 2)
来源：http://mqq.vqdsnc.cn

C#:   f(a: 1, b: 2)
来源：http://vfu.chenzaomai.com

[C05] 返回多个值
来源：http://fcz.yanxiufei.cn

Py:   return a, b
来源：http://nrl.svipenyu.cn

PHP:  return [$a, $b];
来源：http://kds.tanke756.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://fmp.yonumen.top

TS:   return { a, b };
来源：http://jqt.jianghu66.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nfz.nanxuanxn.top

Go:   return a, b
来源：http://ott.havefunace.top

Ruby: return a, b
来源：http://cla.iojbl.cn

C#:   return (a, b);              // ValueTuple
来源：http://cct.shanyushiyangkeji.top

[C06] 匿名函数 / lambda
来源：http://jdm.0kj1m.cn

Py:   square = lambda x: x * x
来源：http://uyo.jyoumei.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://qow.aizwys.cn

JS:   const square = x => x * x;
来源：http://ncv.9152youxi.cn

TS:   const square = (x: number): number => x * x;
来源：http://cmk.epnwcf.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zzf.sufxvd.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xix.c1oappe.top

Ruby: square = ->(x) { x * x }
来源：http://cgc.meibo888.top

C#:   Func<int, int> square = x => x * x;
来源：http://mek.cqqwz.cn

[C07] 把函数作为参数传入
来源：http://qhz.shangyingyoupin.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://iyl.yj20258.top

PHP:  array_map("strtoupper", $arr);
来源：http://bdx.fehbvm.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jle.daria6918.cn

TS:   arr.map(String)
来源：http://ida.hfpthk.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hya.daria6918.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://itq.cheryme.top

Ruby: arr.map(&:upcase)
来源：http://axr.ydzc1.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ppg.zhijiandao.cn

[C08] 闭包
来源：http://fzt.feifeiyinyue.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tnk.guowangkeji.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://iic.shangyingyoupin.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fie.xuetiantiany.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sbq.shanyushiyangkeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://aqq.yuanzhike.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ivj.yfazqb.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xpr.yonumen.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vcb.sufxvd.cn

[C09] 递归
来源：http://xyf.zhixingplan.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ubk.hysaishi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ful.hesvh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yfz.zhiwuduotai.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://znh.yonumen.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zvm.sweek.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mhd.yfazqb.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://koo.gzhubu.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gad.cqqwz.cn

[C10] 变量作用域
来源：http://qhu.aizwys.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://shw.ywan-chungtsiang.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hai.dashuyun.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vny.tanke756.top

TS:   同 JS
来源：http://nlr.zdqjudy.top

Java: 方法内为块级作用域
来源：http://wjm.birdmap.top

Go:   花括号块级作用域
来源：http://nys.52xcode.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qrj.ehwqpu.com

C#:   块级作用域
来源：http://xrx.uphjek.com

[C11] 模块导入与导出
来源：http://ald.gaohongyu789.top

Py:   from module import func
来源：http://slu.gotoacloud.top

PHP:  require "file.php";  或 use App\Service;
来源：http://rhf.hfpthk.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zaj.meibo888.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hpv.ydjk.org.cn

Java: import java.util.List;
来源：http://ivd.zhiwuduotai.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cdd.nanxuanxn.top

Ruby: require "json"; require_relative "./util"
来源：http://nux.fanxiaobao.xyz

C#:   using System.Text;
来源：http://eqi.chenzaomai.com

[C12] 立即执行函数 IIFE
来源：http://ibi.hcnkem.com

Py:   (lambda: print("run"))()
来源：http://avb.zhoulong.xyz

PHP:  (function () { echo "run"; })();
来源：http://xuu.fehbvm.com

JS:   (() => { console.log("run"); })();
来源：http://ucq.jqgufenzy.top

TS:   (() => { console.log("run"); })();
来源：http://pdc.fengsongda.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://llz.andypj.xyz

Go:   func() { fmt.Println("run") }()
来源：http://vhv.xuetiantiany.cn

Ruby: -> { puts "run" }.call
来源：http://wyk.tarul.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://pao.kuanghao11.cn

[C13] 类型声明 / 类型注解
来源：http://fwl.shanyushiyangkeji.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cbo.fktsv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ibc.xinyue.icu

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ihh.haohaochexian.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yvz.jinghuilouyu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vmo.svipenyu.cn

Go:   func add(a, b int) int
来源：http://lfy.sysykeji.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ody.bjfxy.top

C#:   int Add(int a, int b) => a + b;
来源：http://iwy.fehbvm.com

[C14] 泛型函数
来源：http://fpv.ivvv.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jkp.tanke756.top

PHP:  // 无泛型
来源：http://adf.nwbrower.top

JS:   // 无泛型
来源：http://abo.hcnkem.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lzq.jyoumei.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gwp.zhaomingkeji.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://exn.hesvh.cn

Ruby: # 无泛型
来源：http://mjh.redwolf501.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://his.yuanzhike.top

[C15] 解构 / 展开参数
来源：http://gib.yangfankeji.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vhm.jiagoushi.top

PHP:  [$a, $b] = $pair;
来源：http://knu.zhijiandao.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hwl.sysykeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vwl.xuetiantiany.cn

Java: // 无解构
来源：http://kwh.hnqzz.top

Go:   // 无解构
来源：http://xls.tanke756.top

Ruby: a, b = pair
来源：http://mfv.hysaishi.cn

C#:   var (a, b) = pair;
来源：http://klb.havefunace.top

[C16] 函数 / 方法重载
来源：http://ogu.ywan-chungtsiang.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://akq.gzhubu.top

PHP:  // 无重载
来源：http://efm.zdbjq.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://jtq.sysykeji.top

TS:   // 用联合类型或重载签名声明
来源：http://hkn.jiagoushi.top

Java: void f(int a) {}  void f(String a) {}
来源：http://esr.zhixingplan.top

Go:   // 无重载：用不同函数名
来源：http://eay.guowangkeji.top

Ruby: # 无重载：靠动态参数
来源：http://xcr.zhongyouzk.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://pqu.ivvv.top

================================================================================
来源：http://grb.yfazqb.com

D. 数组 / 列表 / 集合
来源：http://yph.yanxiufei.cn

================================================================================
来源：http://qcw.ctjpmb.com

[D01] 创建数组 / 列表
来源：http://dbz.jinqigfzy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://rov.jyoumei.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pwg.xuanzx.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kwv.ydjk.org.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://itk.xziqi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hxd.yfazqb.com

Go:   arr := []int{1, 2, 3}
来源：http://rap.andypj.xyz

Ruby: arr = [1, 2, 3]
来源：http://shu.jianghu66.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qbc.yongpay.top

[D02] 追加元素到末尾
来源：http://umh.fktsv.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uow.cashguo.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tjc.ctjpmb.com

JS:   arr.push(4);
来源：http://gre.wangshuangyany.cn

TS:   arr.push(4);
来源：http://bvn.snrcjt.cn

Java: list.add(4);
来源：http://swk.shangyingyoupin.top

Go:   arr = append(arr, 4)
来源：http://ymq.vqdsnc.cn

Ruby: arr << 4; arr.push(5)
来源：http://ucv.ehwqpu.com

C#:   list.Add(4);
来源：http://xuk.0kj1m.cn

[D03] 在指定位置插入元素
来源：http://bbg.ctjpmb.com

Py:   arr.insert(0, 0)
来源：http://lls.smart0.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ejo.fzhhl.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zzi.cdnleiting.top

TS:   arr.splice(0, 0, 0);
来源：http://uiw.yj20258888.top

Java: list.add(0, 0);
来源：http://sjd.pengpengdd.cyou

Go:   arr = append([]int{0}, arr...)
来源：http://sre.jlsjyb.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qqo.zhaomingkeji.xyz

C#:   list.Insert(0, 0);
来源：http://sfq.hywenlv.cn

[D04] 删除元素
来源：http://fxm.cdnleiting.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://snc.sysykeji.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://osg.fanxiaobao.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lej.quarkkingdee.top

TS:   arr.splice(0, 1);
来源：http://wua.daxiang520.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mpg.jiagoushi.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://syi.ybcxt.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dzm.nwbrower.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xiq.daria6918.cn

[D05] 访问与修改元素
来源：http://ncx.hywenlv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dez.tian-w.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wkm.uphjek.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fme.wangshuangyany.cn

TS:   arr[0]; arr.at(-1);
来源：http://hfi.zhijiandao.cn

Java: list.get(0); list.set(0, 9);
来源：http://ggx.zdqjudy.top

Go:   arr[0]; arr[0] = 9
来源：http://rqj.chenlongwang.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ead.tanke756.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pkh.yvedp.cn

[D06] 数组长度
来源：http://yzp.vqdsnc.cn

Py:   len(arr)
来源：http://duw.cqqwz.cn

PHP:  count($arr);
来源：http://qio.epnwcf.com

JS:   arr.length
来源：http://hly.hcnkem.com

TS:   arr.length
来源：http://ftk.tian-w.cn

Java: list.size();
来源：http://mii.feifeiyinyue.top

Go:   len(arr)
来源：http://dge.xinyue.icu

Ruby: arr.length; arr.size
来源：http://wwa.jyoumei.cn

C#:   list.Count;
来源：http://xns.mhx1999.top

[D07] 切片 / 取子数组
来源：http://pet.0kj1m.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dqg.aizwys.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qit.feifeiyinyue.top

JS:   arr.slice(1, 4);
来源：http://nxo.dashuyun.cn

TS:   arr.slice(1, 4);
来源：http://gzg.xylfe.cn

Java: list.subList(1, 4);
来源：http://idv.jqgufenzy.top

Go:   arr[1:4]
来源：http://rst.nanxinkj.top

Ruby: arr[1, 3]
来源：http://bak.mhx1999.top

C#:   list.GetRange(1, 3);
来源：http://dob.aibaodan.cn

[D08] 合并两个数组
来源：http://oyc.aizwys.cn

Py:   a + b;  a.extend(b)
来源：http://tym.zhengqikj.top

PHP:  array_merge($a, $b);
来源：http://xfo.yvedp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ssg.ywan-chungtsiang.top

TS:   [...a, ...b];
来源：http://nfh.jiagoushi.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://voq.52xcode.cn

Go:   append(a, b...)
来源：http://sfu.yj202588.top

Ruby: a + b;  a.concat(b)
来源：http://xgf.xuetiantiany.cn

C#:   a.Concat(b).ToList()
来源：http://plo.bjfxy.top

[D09] 排序（升序）
来源：http://pxs.guowangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://bkq.chenzaomai.com

PHP:  sort($arr);
来源：http://nys.jinqigfzy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://urj.tianlin.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://pwo.yueranfly.top

Java: Collections.sort(list);  list.sort(null);
来源：http://vyo.yj20258888.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gmm.fktsv.cn

Ruby: arr.sort
来源：http://ogy.yangfankeji.com

C#:   list.Sort();
来源：http://bgj.uphjek.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://end.daxiang520.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mnt.havefunace.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gym.yanxiufei.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wmg.hnqzz.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tlo.shuidangran.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fce.zdbjq.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cym.yfazqb.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kdy.xuetiantiany.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://khv.yangfankeji.com

[D11] 反转数组
来源：http://rxf.chenzaomai.com

Py:   arr[::-1];  arr.reverse()
来源：http://sgh.cdnleiting.top

PHP:  array_reverse($arr);
来源：http://yuz.havefunace.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rpz.yanxiufei.cn

TS:   [...arr].reverse();
来源：http://hnk.fzhhl.top

Java: Collections.reverse(list);
来源：http://wll.gzhubu.top

Go:   slices.Reverse(arr)
来源：http://aty.sufxvd.cn

Ruby: arr.reverse
来源：http://lwh.chenlongwang.top

C#:   list.Reverse();
来源：http://hzb.quarkkingdee.top

[D12] 查找元素下标
来源：http://kia.cheryme.top

Py:   arr.index(x);  x in arr
来源：http://jmf.ctjpmb.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bbe.ybcxt.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ucn.vqdsnc.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ufp.hysaishi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rpr.tian-w.cn

Go:   slices.Index(arr, x)
来源：http://xyw.zhixingplan.top

Ruby: arr.index(x)
来源：http://rrq.chenlongwang.top

C#:   list.IndexOf(x);
来源：http://xhl.shanyushiyangkeji.top

[D13] 过滤（保留满足条件的）
来源：http://zsr.tarul.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jkp.316326.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fsu.vehdjk.com

JS:   arr.filter(x => x > 3)
来源：http://oyd.yj20258888.top

TS:   arr.filter(x => x > 3)
来源：http://nxz.shangyingyoupin.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fbk.hammf.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zqy.shuidangran.top

Ruby: arr.select { |x| x > 3 }
来源：http://cbh.ctjpmb.com

C#:   list.Where(x => x > 3).ToList()
来源：http://mxz.ppjwa.cn

[D14] 映射转换（每个元素变形）
来源：http://qlo.ybcxt.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://oey.nanxuanxn.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vfb.shuidangran.top

JS:   arr.map(x => x * 2)
来源：http://awc.gotoacloud.top

TS:   arr.map(x => x * 2)
来源：http://szk.tanke756.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://iwo.fengsongda.top

Go:   // 手写循环
来源：http://los.yuanzhike.top

Ruby: arr.map { |x| x * 2 }
来源：http://pjb.dashuyun.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://htu.guowangkeji.top

[D15] 去重
来源：http://kjk.ctjpmb.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zyu.hysaishi.cn

PHP:  array_unique($arr);
来源：http://kyj.yvedp.cn

JS:   [...new Set(arr)]
来源：http://ydz.hammf.cn

TS:   [...new Set(arr)]
来源：http://dkn.yongpay.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rbp.hammf.cn

Go:   // 用 map[T]struct{} 手写
来源：http://nse.sjlbkw.cn

Ruby: arr.uniq
来源：http://vtt.smart0.xyz

C#:   list.Distinct().ToList()
来源：http://xgu.vqdsnc.cn

[D16] 求和与平均值
来源：http://cii.sxryk.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hua.svipenyu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rei.hywenlv.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vzy.yvedp.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mfw.yueranfly.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xlq.haohaochexian.top

Go:   // 手写循环累加
来源：http://lbg.yj20258888.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bfj.sufxvd.cn

C#:   list.Sum();  list.Average()
来源：http://oxf.andypj.xyz

[D17] 最大值与最小值
来源：http://oub.iojbl.cn

Py:   max(arr);  min(arr)
来源：http://clw.wangshuangyany.cn

PHP:  max($arr);  min($arr);
来源：http://tqu.quarkkingdee.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://osy.yj20258.top

TS:   Math.max(...arr);
来源：http://hek.c1oappe.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ekc.yanxiufei.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dex.jinyuanbaomall.cn

Ruby: arr.max;  arr.min
来源：http://vgh.9152youxi.cn

C#:   list.Max();  list.Min()
来源：http://xmy.hcnkem.com

[D18] 扁平化嵌套数组
来源：http://xru.ydzc1.top


<!-- 参考信息 -->
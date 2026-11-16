代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://dow.birdmap.top

[C03] 可变参数
来源：http://jha.tian-w.cn

Py:   def total(*args): return sum(args)
来源：http://mvq.yangfankeji.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xze.fktsv.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rof.316326.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ptr.yueranfly.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mcy.yj20258.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tjk.birdmap.top

Ruby: def total(*nums); nums.sum; end
来源：http://qhe.jiagoushi.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://opk.jiagoushi.top

[C04] 命名参数 / 关键字参数
来源：http://tqs.yanxiufei.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ylv.jiagoushi.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fri.hesvh.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vot.fzhhl.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vnl.jinqigufen.top

Java: // 无：用 Builder 模式或 record
来源：http://pje.0kj1m.cn

Go:   // 无：用配置结构体参数
来源：http://oma.ybcxt.top

Ruby: f(a: 1, b: 2)
来源：http://xky.andypj.xyz

C#:   f(a: 1, b: 2)
来源：http://upc.zdbjq.cn

[C05] 返回多个值
来源：http://cwt.shzxlz.cn

Py:   return a, b
来源：http://dzd.zhoulong.xyz

PHP:  return [$a, $b];
来源：http://kod.fzhhl.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ezd.yongpay.top

TS:   return { a, b };
来源：http://mjt.ywan-chungtsiang.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xhp.meibo888.top

Go:   return a, b
来源：http://fgw.jinqigufen.top

Ruby: return a, b
来源：http://jxt.sweek.top

C#:   return (a, b);              // ValueTuple
来源：http://gty.hcnkem.com

[C06] 匿名函数 / lambda
来源：http://gai.dianchejie.cn

Py:   square = lambda x: x * x
来源：http://oby.fengsongda.top

PHP:  $square = fn($x) => $x * $x;
来源：http://dsg.yuanzhike.top

JS:   const square = x => x * x;
来源：http://cuo.yuxming.cn

TS:   const square = (x: number): number => x * x;
来源：http://kui.birdmap.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vue.jinyuanbaomall.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fez.ydzc1.top

Ruby: square = ->(x) { x * x }
来源：http://vvt.tianlin.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://rht.gzhubu.top

[C07] 把函数作为参数传入
来源：http://euh.ydzc1.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mov.xuanzx.com

PHP:  array_map("strtoupper", $arr);
来源：http://pvo.daxiang520.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xkl.zdqjudy.top

TS:   arr.map(String)
来源：http://csu.c1oappe.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zpv.aibaodan.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://urz.dianchejie.cn

Ruby: arr.map(&:upcase)
来源：http://auz.guowangkeji.top

C#:   arr.Select(s => s.ToUpper())
来源：http://itj.tarul.cn

[C08] 闭包
来源：http://hul.cdnleiting.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gyj.wangdashe.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pdb.gaohongyu789.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xqw.daxiang520.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gml.meibo888.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cpx.smart0.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gwo.guannengcc.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hum.nanxuanxn.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fix.pengpengdd.cyou

[C09] 递归
来源：http://ieo.fengsongda.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://upo.epnwcf.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xro.hnqzz.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cxk.zhiwuduotai.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://taj.chenzaomai.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://aql.hfpthk.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hdh.aibaodan.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dnp.hongshengwenyu.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mtb.ctjpmb.com

[C10] 变量作用域
来源：http://yez.gaohongyu789.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cbq.sjlbkw.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ilk.yongpay.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jtl.316326.xyz

TS:   同 JS
来源：http://raz.hywenlv.cn

Java: 方法内为块级作用域
来源：http://nzg.sweek.top

Go:   花括号块级作用域
来源：http://pqr.tarul.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://iua.hongshengwenyu.top

C#:   块级作用域
来源：http://lva.zdqjudy.top

[C11] 模块导入与导出
来源：http://hyq.ppjwa.cn

Py:   from module import func
来源：http://kyw.ppjwa.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pca.c1oappe.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://oqy.zhijiandao.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pea.pycfn.com

Java: import java.util.List;
来源：http://tuw.316326.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rip.aibaodan.cn

Ruby: require "json"; require_relative "./util"
来源：http://edj.yongpay.top

C#:   using System.Text;
来源：http://ciu.xylfe.cn

[C12] 立即执行函数 IIFE
来源：http://mef.dashuyun.cn

Py:   (lambda: print("run"))()
来源：http://rrm.redwolf501.top

PHP:  (function () { echo "run"; })();
来源：http://mzu.c1oappe.top

JS:   (() => { console.log("run"); })();
来源：http://pht.gogol.net.cn

TS:   (() => { console.log("run"); })();
来源：http://hsm.jqgfzy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tkg.gzhubu.top

Go:   func() { fmt.Println("run") }()
来源：http://thg.gaohongyu789.top

Ruby: -> { puts "run" }.call
来源：http://zsg.chenzaomai.com

C#:   // 无 IIFE：用静态构造函数
来源：http://hft.cqqwz.cn

[C13] 类型声明 / 类型注解
来源：http://bvt.cqqwz.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bfb.wangdashe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://duw.jinqigufen.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wuj.xylfe.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dok.zhiwuduotai.top

Java: int add(int a, int b) { return a + b; }
来源：http://rnu.chenlongwang.top

Go:   func add(a, b int) int
来源：http://ohx.mhx1999.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yyk.tanke756.top

C#:   int Add(int a, int b) => a + b;
来源：http://enp.52xcode.cn

[C14] 泛型函数
来源：http://xpb.uphjek.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://npm.jinqigfzy.top

PHP:  // 无泛型
来源：http://fdt.sufxvd.cn

JS:   // 无泛型
来源：http://gxr.pengpengdd.cyou

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://npo.shuidangran.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pnf.0kj1m.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gnh.meibo888.top

Ruby: # 无泛型
来源：http://jvj.haohaochexian.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ikz.zhijiandao.cn

[C15] 解构 / 展开参数
来源：http://nws.ctjpmb.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yrl.cdnleiting.top

PHP:  [$a, $b] = $pair;
来源：http://nrt.jinghuilouyu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dfd.zycfv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ssp.jyoumei.cn

Java: // 无解构
来源：http://mcr.ppjwa.cn

Go:   // 无解构
来源：http://oah.shangyingyoupin.top

Ruby: a, b = pair
来源：http://cle.wangdashe.top

C#:   var (a, b) = pair;
来源：http://qpb.nanxuanxn.top

[C16] 函数 / 方法重载
来源：http://wbr.hywenlv.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xzk.chenlongwang.top

PHP:  // 无重载
来源：http://ivf.0kj1m.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://pok.cqqwz.cn

TS:   // 用联合类型或重载签名声明
来源：http://ymv.jinyuanbaomall.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jdg.zhixingplan.top

Go:   // 无重载：用不同函数名
来源：http://emr.yuxming.cn

Ruby: # 无重载：靠动态参数
来源：http://ceb.nwbrower.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://coe.yvedp.cn

================================================================================
来源：http://xlx.cqqwz.cn

D. 数组 / 列表 / 集合
来源：http://rgu.wangdashe.top

================================================================================
来源：http://clx.nwbrower.top

[D01] 创建数组 / 列表
来源：http://nll.zhixingplan.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://azt.0kj1m.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://azy.bbcook.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rfy.svipenyu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://rpu.hnxiangtu.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nfv.ydjk.org.cn

Go:   arr := []int{1, 2, 3}
来源：http://gwp.jqgfzy.top

Ruby: arr = [1, 2, 3]
来源：http://cgt.daria6918.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qfv.hammf.cn

[D02] 追加元素到末尾
来源：http://yxx.guowangkeji.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uim.vehdjk.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sfp.hywenlv.cn

JS:   arr.push(4);
来源：http://hur.cheryme.top

TS:   arr.push(4);
来源：http://uyh.yonumen.top

Java: list.add(4);
来源：http://vnh.0kj1m.cn

Go:   arr = append(arr, 4)
来源：http://dhd.hongshengwenyu.top

Ruby: arr << 4; arr.push(5)
来源：http://nuz.yj20258.top

C#:   list.Add(4);
来源：http://lbn.dianchejie.cn

[D03] 在指定位置插入元素
来源：http://flw.feifeiyinyue.top

Py:   arr.insert(0, 0)
来源：http://njc.zhoulong.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ukg.meibo888.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gdp.ywan-chungtsiang.top

TS:   arr.splice(0, 0, 0);
来源：http://way.zhixingplan.top

Java: list.add(0, 0);
来源：http://fhm.yueranfly.top

Go:   arr = append([]int{0}, arr...)
来源：http://kjd.zhijiandao.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zpd.pengpengdd.cyou

C#:   list.Insert(0, 0);
来源：http://ggs.ctjpmb.com

[D04] 删除元素
来源：http://pyl.smart0.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nvm.shzxlz.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qww.ctjpmb.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lyk.xinyue.icu

TS:   arr.splice(0, 1);
来源：http://kny.xuetiantiany.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bhu.52xcode.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://myr.zdbjq.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zqv.kuanghao11.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rof.wangdashe.top

[D05] 访问与修改元素
来源：http://jie.sjlbkw.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jyr.vqdsnc.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jyr.jianghu66.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://aae.yvedp.cn

TS:   arr[0]; arr.at(-1);
来源：http://qxt.nwbrower.top

Java: list.get(0); list.set(0, 9);
来源：http://wxn.yvedp.cn

Go:   arr[0]; arr[0] = 9
来源：http://bba.nanxuanxn.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kvc.aibaodan.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://llq.cucudq.cn

[D06] 数组长度
来源：http://hog.uphjek.com

Py:   len(arr)
来源：http://khh.daxiang520.top

PHP:  count($arr);
来源：http://cxs.birdmap.top

JS:   arr.length
来源：http://fuz.hfpthk.cn

TS:   arr.length
来源：http://thj.jinqigfzy.top

Java: list.size();
来源：http://kxu.iojbl.cn

Go:   len(arr)
来源：http://tdb.hywenlv.cn

Ruby: arr.length; arr.size
来源：http://sjc.shanyushiyangtech.top

C#:   list.Count;
来源：http://bxx.zhongyouzk.top

[D07] 切片 / 取子数组
来源：http://qmq.jinghuilouyu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yhq.chenlongwang.top

PHP:  array_slice($arr, 1, 3);
来源：http://dcw.ybcxt.top

JS:   arr.slice(1, 4);
来源：http://pxq.chenzaomai.com

TS:   arr.slice(1, 4);
来源：http://qzw.yongpay.top

Java: list.subList(1, 4);
来源：http://rvp.smart0.xyz

Go:   arr[1:4]
来源：http://fcw.cdnleiting.top

Ruby: arr[1, 3]
来源：http://wvc.aizwys.cn

C#:   list.GetRange(1, 3);
来源：http://txb.shzxlz.cn

[D08] 合并两个数组
来源：http://zly.ywan-chungtsiang.top

Py:   a + b;  a.extend(b)
来源：http://pag.wangdashe.top

PHP:  array_merge($a, $b);
来源：http://ksn.cashguo.top

JS:   [...a, ...b];  a.concat(b);
来源：http://xhk.nanxuanxn.top

TS:   [...a, ...b];
来源：http://uhd.vehdjk.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mop.aibaodan.cn

Go:   append(a, b...)
来源：http://ksb.9152youxi.cn

Ruby: a + b;  a.concat(b)
来源：http://yko.andypj.xyz

C#:   a.Concat(b).ToList()
来源：http://wdj.ppjwa.cn

[D09] 排序（升序）
来源：http://etc.bbcook.cn

Py:   sorted(arr);  arr.sort()
来源：http://aeb.cqqwz.cn

PHP:  sort($arr);
来源：http://dxy.shanyushiyangtech.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jua.ehwqpu.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://fxf.ehwqpu.com

Java: Collections.sort(list);  list.sort(null);
来源：http://ugb.cqqwz.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://awg.smart0.xyz

Ruby: arr.sort
来源：http://agf.dianchejie.cn

C#:   list.Sort();
来源：http://tyc.yuanzhike.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ita.zhongyouzk.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://trv.pengpengdd.cyou

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sak.ydjk.org.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vwz.haohaochexian.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://aoq.sufxvd.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://imz.tian-w.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://crh.chenzaomai.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gvj.jinqigfzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://aul.ydjk.org.cn

[D11] 反转数组
来源：http://gxh.zdbjq.cn

Py:   arr[::-1];  arr.reverse()
来源：http://jnz.mhx1999.top

PHP:  array_reverse($arr);
来源：http://wrf.havefunace.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yom.ehwqpu.com

TS:   [...arr].reverse();
来源：http://gpo.iojbl.cn

Java: Collections.reverse(list);
来源：http://qqj.jinqigfzy.top

Go:   slices.Reverse(arr)
来源：http://qpo.yvedp.cn

Ruby: arr.reverse
来源：http://eye.sweek.top

C#:   list.Reverse();
来源：http://sdf.yj20258888.top

[D12] 查找元素下标
来源：http://soc.quarkkingdee.top

Py:   arr.index(x);  x in arr
来源：http://aym.jqgfzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xbr.pycfn.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ukd.gaohongyu789.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dgk.redwolf501.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yjj.c1oappe.top

Go:   slices.Index(arr, x)
来源：http://owl.hysaishi.cn

Ruby: arr.index(x)
来源：http://wdt.shuidangran.top

C#:   list.IndexOf(x);
来源：http://qhy.wangdashe.top

[D13] 过滤（保留满足条件的）
来源：http://ivn.ivvv.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wzv.jqgfzy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gep.zdqjudy.top

JS:   arr.filter(x => x > 3)
来源：http://nta.guowangkeji.top

TS:   arr.filter(x => x > 3)
来源：http://snt.hnxiangtu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xib.zdqjudy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xxp.zhengqikj.top

Ruby: arr.select { |x| x > 3 }
来源：http://hbu.yangfankeji.com

C#:   list.Where(x => x > 3).ToList()
来源：http://pzf.tarul.cn

[D14] 映射转换（每个元素变形）
来源：http://xds.pengpengdd.cyou

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ity.xziqi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uoa.yvedp.cn

JS:   arr.map(x => x * 2)
来源：http://irf.hysaishi.cn

TS:   arr.map(x => x * 2)
来源：http://kpt.mhx1999.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://goy.yj20258888.top

Go:   // 手写循环
来源：http://exp.epnwcf.com

Ruby: arr.map { |x| x * 2 }
来源：http://qtk.hywenlv.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://uak.cucudq.cn

[D15] 去重
来源：http://ygy.pengpengdd.cyou

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ytb.zhoulong.xyz

PHP:  array_unique($arr);
来源：http://isj.jlsjyb.cn

JS:   [...new Set(arr)]
来源：http://kri.bbcook.cn

TS:   [...new Set(arr)]
来源：http://ucp.fzhhl.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://udy.sweek.top

Go:   // 用 map[T]struct{} 手写
来源：http://amn.smart0.xyz

Ruby: arr.uniq
来源：http://lmz.yangfankeji.com

C#:   list.Distinct().ToList()
来源：http://hda.ydzc1.top

[D16] 求和与平均值
来源：http://wil.yvedp.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vku.ivvv.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://oza.hfpthk.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wad.svipenyu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lbn.9152youxi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://paq.fzhhl.top

Go:   // 手写循环累加
来源：http://kmn.jqgufenzy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rol.jinghuilouyu.cn

C#:   list.Sum();  list.Average()
来源：http://dnt.aizwys.cn

[D17] 最大值与最小值
来源：http://ege.jinyuanbaomall.cn

Py:   max(arr);  min(arr)
来源：http://how.mhx1999.top

PHP:  max($arr);  min($arr);
来源：http://tuk.yj202588.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ibh.ywan-chungtsiang.top

TS:   Math.max(...arr);
来源：http://ggr.sufxvd.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://akx.hcnkem.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dnx.yvedp.cn

Ruby: arr.max;  arr.min
来源：http://pji.hammf.cn

C#:   list.Max();  list.Min()
来源：http://xsn.cheryme.top

[D18] 扁平化嵌套数组
来源：http://tfr.tian-w.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rxo.tarul.cn

PHP:  array_merge(...$nested);
来源：http://zsa.hesvh.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://axn.hammf.cn

TS:   nested.flat();
来源：http://mjz.zhiwuduotai.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yqz.andypj.xyz

Go:   // 手写双层循环
来源：http://cyp.cucudq.cn

Ruby: nested.flatten
来源：http://piv.snrcjt.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://iby.sweek.top

[D19] 按字段分组
来源：http://hth.nanxuanxn.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nvh.0kj1m.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dzq.gzhubu.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://swi.snrcjt.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://lle.hongshengwenyu.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dry.tianlin.xyz

Go:   // 手写 map[string][]T
来源：http://nvy.ivvv.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://yej.ppjwa.cn


<!-- 参考信息 -->
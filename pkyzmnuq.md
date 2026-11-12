代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://brs.quarkkingdee.top

Java: // 无默认参数：方法重载或 Optional
来源：http://kvv.zhiwuduotai.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ewn.yuxming.cn

Ruby: def greet(name = "World") = name
来源：http://aix.jlsjyb.cn

C#:   string Greet(string name = "World") => name;
来源：http://kge.xingfuxueyuan.xyz

[C03] 可变参数
来源：http://yww.yuanzhike.top

Py:   def total(*args): return sum(args)
来源：http://bir.zhixingplan.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://itg.ppjwa.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ava.jianghu66.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://usw.fehbvm.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xqd.yj20258.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sol.tarul.cn

Ruby: def total(*nums); nums.sum; end
来源：http://woz.jqgfzy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://llr.0kj1m.cn

[C04] 命名参数 / 关键字参数
来源：http://dlx.jinyuanbaomall.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://khl.wangdashe.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://awv.shanyushiyangtech.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://csh.nwbrower.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hpi.hnxiangtu.top

Java: // 无：用 Builder 模式或 record
来源：http://fpp.tianlin.xyz

Go:   // 无：用配置结构体参数
来源：http://jjs.xylfe.cn

Ruby: f(a: 1, b: 2)
来源：http://hsq.xuanzx.com

C#:   f(a: 1, b: 2)
来源：http://rwx.jyoumei.cn

[C05] 返回多个值
来源：http://lte.cashguo.top

Py:   return a, b
来源：http://laa.jinghuilouyu.cn

PHP:  return [$a, $b];
来源：http://mxd.birdmap.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ulq.fehbvm.com

TS:   return { a, b };
来源：http://atv.zhijiandao.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sxf.hfpthk.cn

Go:   return a, b
来源：http://xxa.316326.xyz

Ruby: return a, b
来源：http://ppp.aizwys.cn

C#:   return (a, b);              // ValueTuple
来源：http://giy.hcnkem.com

[C06] 匿名函数 / lambda
来源：http://vju.uphjek.com

Py:   square = lambda x: x * x
来源：http://ntd.hcnkem.com

PHP:  $square = fn($x) => $x * $x;
来源：http://vvy.aizwys.cn

JS:   const square = x => x * x;
来源：http://eqa.gogol.net.cn

TS:   const square = (x: number): number => x * x;
来源：http://goi.havefunace.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lwf.bjfxy.top

Go:   sq := func(x int) int { return x * x }
来源：http://qhg.daria6918.cn

Ruby: square = ->(x) { x * x }
来源：http://wdf.shanyushiyangtech.top

C#:   Func<int, int> square = x => x * x;
来源：http://yyl.zhengqikj.top

[C07] 把函数作为参数传入
来源：http://hvx.9152youxi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qop.bjfxy.top

PHP:  array_map("strtoupper", $arr);
来源：http://xmq.jqgufenzy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sdx.jiagoushi.top

TS:   arr.map(String)
来源：http://jdu.ctjpmb.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nib.zhijiandao.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wim.jiagoushi.top

Ruby: arr.map(&:upcase)
来源：http://yiv.ybcxt.top

C#:   arr.Select(s => s.ToUpper())
来源：http://vfm.haohaochexian.top

[C08] 闭包
来源：http://ojg.vqdsnc.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lev.chenzaomai.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://stg.sweek.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pkx.yongpay.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://drk.hongshengwenyu.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xyi.yfazqb.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://scz.ywan-chungtsiang.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://eva.jyoumei.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rzk.yuxming.cn

[C09] 递归
来源：http://kcm.yueranfly.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bqc.cashguo.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wri.hnqzz.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iwi.bbcook.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qay.tanke756.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zvy.ydjk.org.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cwq.zhaomingkeji.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xiu.zhoulong.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gxz.sufxvd.cn

[C10] 变量作用域
来源：http://yer.redwolf501.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ckj.tian-w.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mii.wangshuangyany.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dqg.cqqwz.cn

TS:   同 JS
来源：http://xel.epnwcf.com

Java: 方法内为块级作用域
来源：http://pco.dianchejie.cn

Go:   花括号块级作用域
来源：http://xag.bjfxy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lon.snrcjt.cn

C#:   块级作用域
来源：http://rom.sjlbkw.cn

[C11] 模块导入与导出
来源：http://dpj.chenlongwang.top

Py:   from module import func
来源：http://xjw.jiagoushi.top

PHP:  require "file.php";  或 use App\Service;
来源：http://duk.chenjidiqi.icu

JS:   export default function f() {};  import f from "./m.js";
来源：http://nru.vqdsnc.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zay.sxryk.cn

Java: import java.util.List;
来源：http://sqi.yangfankeji.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gue.havefunace.top

Ruby: require "json"; require_relative "./util"
来源：http://owz.haohaochexian.top

C#:   using System.Text;
来源：http://cku.shangyingyoupin.top

[C12] 立即执行函数 IIFE
来源：http://uuu.cucudq.cn

Py:   (lambda: print("run"))()
来源：http://lts.bjfxy.top

PHP:  (function () { echo "run"; })();
来源：http://fbv.jiagoushi.top

JS:   (() => { console.log("run"); })();
来源：http://ifi.hfpthk.cn

TS:   (() => { console.log("run"); })();
来源：http://mhr.xylfe.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jae.hnqzz.top

Go:   func() { fmt.Println("run") }()
来源：http://wvd.zhaomingkeji.xyz

Ruby: -> { puts "run" }.call
来源：http://qlz.haohaochexian.top

C#:   // 无 IIFE：用静态构造函数
来源：http://xwg.tarul.cn

[C13] 类型声明 / 类型注解
来源：http://bpo.zhiwuduotai.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sbf.cqqwz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ixa.fzhhl.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://luc.tanke756.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dvm.52xcode.cn

Java: int add(int a, int b) { return a + b; }
来源：http://eep.yj20258888.top

Go:   func add(a, b int) int
来源：http://uqh.yj20258888.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lny.mhx1999.top

C#:   int Add(int a, int b) => a + b;
来源：http://ene.0kj1m.cn

[C14] 泛型函数
来源：http://ilz.nwbrower.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vyd.meibo888.top

PHP:  // 无泛型
来源：http://ejr.ydzc1.top

JS:   // 无泛型
来源：http://ylv.ehwqpu.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bih.aibaodan.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://piu.xinyue.icu

Go:   func First[T any](items []T) T { return items[0] }
来源：http://veu.tianlin.xyz

Ruby: # 无泛型
来源：http://oig.sjlbkw.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nhh.cashguo.top

[C15] 解构 / 展开参数
来源：http://jeh.wangshuangyany.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bia.sysykeji.top

PHP:  [$a, $b] = $pair;
来源：http://ypj.dashuyun.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://are.c1oappe.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rfc.sxryk.cn

Java: // 无解构
来源：http://ysm.ydzc1.top

Go:   // 无解构
来源：http://oyx.pycfn.com

Ruby: a, b = pair
来源：http://vlv.zhijiandao.cn

C#:   var (a, b) = pair;
来源：http://xbs.zhengqikj.top

[C16] 函数 / 方法重载
来源：http://hsd.xziqi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sxh.sxryk.cn

PHP:  // 无重载
来源：http://ipz.sjlbkw.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://uiy.hammf.cn

TS:   // 用联合类型或重载签名声明
来源：http://oew.havefunace.top

Java: void f(int a) {}  void f(String a) {}
来源：http://irm.havefunace.top

Go:   // 无重载：用不同函数名
来源：http://vju.pengpengdd.cyou

Ruby: # 无重载：靠动态参数
来源：http://scd.snrcjt.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ezr.iojbl.cn

================================================================================
来源：http://zjk.cashguo.top

D. 数组 / 列表 / 集合
来源：http://ngf.aizwys.cn

================================================================================
来源：http://bro.zdbjq.cn

[D01] 创建数组 / 列表
来源：http://mku.zdbjq.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://opy.havefunace.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vtn.pengpengdd.cyou

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dki.havefunace.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://jzd.daria6918.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rvm.fanxiaobao.xyz

Go:   arr := []int{1, 2, 3}
来源：http://muz.vehdjk.com

Ruby: arr = [1, 2, 3]
来源：http://yds.bjfxy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vol.quarkkingdee.top

[D02] 追加元素到末尾
来源：http://msr.cqqwz.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://out.fanxiaobao.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nxb.jinyuanbaomall.cn

JS:   arr.push(4);
来源：http://ddy.uphjek.com

TS:   arr.push(4);
来源：http://sym.ehwqpu.com

Java: list.add(4);
来源：http://gsw.hcnkem.com

Go:   arr = append(arr, 4)
来源：http://wpl.sxryk.cn

Ruby: arr << 4; arr.push(5)
来源：http://luh.hammf.cn

C#:   list.Add(4);
来源：http://pmu.cucudq.cn

[D03] 在指定位置插入元素
来源：http://dwc.dashuyun.cn

Py:   arr.insert(0, 0)
来源：http://jao.ctjpmb.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xzr.jianghu66.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yjy.ppjwa.cn

TS:   arr.splice(0, 0, 0);
来源：http://uut.hcnkem.com

Java: list.add(0, 0);
来源：http://yhy.epnwcf.com

Go:   arr = append([]int{0}, arr...)
来源：http://way.kuanghao11.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lxs.yangfankeji.com

C#:   list.Insert(0, 0);
来源：http://eqy.shangyingyoupin.top

[D04] 删除元素
来源：http://yhk.0kj1m.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wux.cucudq.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qki.jianghu66.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xim.daxiang520.top

TS:   arr.splice(0, 1);
来源：http://jnf.nanxuanxn.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://eng.zdbjq.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dyt.feifeiyinyue.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lht.kuanghao11.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://loo.chenjidiqi.icu

[D05] 访问与修改元素
来源：http://qsa.jqgfzy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ssz.yj20258888.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yku.aibaodan.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jhd.dashuyun.cn

TS:   arr[0]; arr.at(-1);
来源：http://ljn.316326.xyz

Java: list.get(0); list.set(0, 9);
来源：http://won.tanke756.top

Go:   arr[0]; arr[0] = 9
来源：http://nsu.zdqjudy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qou.kuanghao11.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fsy.yj202588.top

[D06] 数组长度
来源：http://lbw.zhixingplan.top

Py:   len(arr)
来源：http://pgo.yj202588.top

PHP:  count($arr);
来源：http://jdh.jinqigufen.top

JS:   arr.length
来源：http://fwm.zycfv.cn

TS:   arr.length
来源：http://iwi.jqgufenzy.top

Java: list.size();
来源：http://kdb.fzhhl.top

Go:   len(arr)
来源：http://koq.bbcook.cn

Ruby: arr.length; arr.size
来源：http://bpq.nwbrower.top

C#:   list.Count;
来源：http://tpp.tian-w.cn

[D07] 切片 / 取子数组
来源：http://dbb.smart0.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xfm.zdqjudy.top

PHP:  array_slice($arr, 1, 3);
来源：http://yjo.quarkkingdee.top

JS:   arr.slice(1, 4);
来源：http://ngc.daxiang520.top

TS:   arr.slice(1, 4);
来源：http://mdk.yfazqb.com

Java: list.subList(1, 4);
来源：http://elb.birdmap.top

Go:   arr[1:4]
来源：http://qhm.zhongyouzk.top

Ruby: arr[1, 3]
来源：http://mtx.hammf.cn

C#:   list.GetRange(1, 3);
来源：http://vcs.tianlin.xyz

[D08] 合并两个数组
来源：http://bsr.quarkkingdee.top

Py:   a + b;  a.extend(b)
来源：http://dke.shzxlz.cn

PHP:  array_merge($a, $b);
来源：http://qhr.nanxuanxn.top

JS:   [...a, ...b];  a.concat(b);
来源：http://tkm.xuanzx.com

TS:   [...a, ...b];
来源：http://dfy.meibo888.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tva.kuanghao11.cn

Go:   append(a, b...)
来源：http://mvu.c1oappe.top

Ruby: a + b;  a.concat(b)
来源：http://fmy.ydzc1.top

C#:   a.Concat(b).ToList()
来源：http://zbz.nanxinkj.top

[D09] 排序（升序）
来源：http://psx.epnwcf.com

Py:   sorted(arr);  arr.sort()
来源：http://gbj.jinyuanbaomall.cn

PHP:  sort($arr);
来源：http://zzx.9152youxi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://foy.shanyushiyangtech.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://avd.zhengqikj.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ikx.vqdsnc.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gzg.ehwqpu.com

Ruby: arr.sort
来源：http://dgt.xuanzx.com

C#:   list.Sort();
来源：http://mwu.ybcxt.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://xmd.yangfankeji.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://diu.aibaodan.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pap.xingfuxueyuan.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://uip.jqgfzy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qfr.yongpay.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ntp.hfpthk.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ymn.redwolf501.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jln.cucudq.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xsl.jinyuanbaomall.cn

[D11] 反转数组
来源：http://oka.aizwys.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gue.fktsv.cn

PHP:  array_reverse($arr);
来源：http://ovu.nanxuanxn.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://uxz.jinyuanbaomall.cn

TS:   [...arr].reverse();
来源：http://bow.andypj.xyz

Java: Collections.reverse(list);
来源：http://sex.yuanzhike.top

Go:   slices.Reverse(arr)
来源：http://wkz.316326.xyz

Ruby: arr.reverse
来源：http://zon.wangshuangyany.cn

C#:   list.Reverse();
来源：http://ifo.vqdsnc.cn

[D12] 查找元素下标
来源：http://prf.ydzc1.top

Py:   arr.index(x);  x in arr
来源：http://khs.nanxinkj.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ngs.fktsv.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aeh.yvedp.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wuz.jyoumei.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rla.zhaomingkeji.xyz

Go:   slices.Index(arr, x)
来源：http://rlw.gotoacloud.top

Ruby: arr.index(x)
来源：http://bqx.316326.xyz

C#:   list.IndexOf(x);
来源：http://wvx.shzxlz.cn

[D13] 过滤（保留满足条件的）
来源：http://elf.bjfxy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qwr.gaohongyu789.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tda.chenzaomai.com

JS:   arr.filter(x => x > 3)
来源：http://dut.9152youxi.cn

TS:   arr.filter(x => x > 3)
来源：http://ewa.52xcode.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://spi.cucudq.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fdy.wangdashe.top

Ruby: arr.select { |x| x > 3 }
来源：http://mig.vqdsnc.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://omy.snrcjt.cn

[D14] 映射转换（每个元素变形）
来源：http://wte.xuetiantiany.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vtt.ctjpmb.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dys.ppjwa.cn

JS:   arr.map(x => x * 2)
来源：http://rsh.bbcook.cn

TS:   arr.map(x => x * 2)
来源：http://ltw.daxiang520.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ckc.tarul.cn

Go:   // 手写循环
来源：http://mwj.shanyushiyangkeji.top

Ruby: arr.map { |x| x * 2 }
来源：http://kdl.zdqjudy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://tfs.xylfe.cn

[D15] 去重
来源：http://brv.xingfuxueyuan.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zqo.yj20258888.top

PHP:  array_unique($arr);
来源：http://awh.hysaishi.cn

JS:   [...new Set(arr)]
来源：http://qko.9152youxi.cn

TS:   [...new Set(arr)]
来源：http://jbh.fehbvm.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dpm.nanxuanxn.top

Go:   // 用 map[T]struct{} 手写
来源：http://qwe.tarul.cn

Ruby: arr.uniq
来源：http://csu.cdnleiting.top

C#:   list.Distinct().ToList()
来源：http://vjm.aizwys.cn

[D16] 求和与平均值
来源：http://ifx.aibaodan.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xcr.ctjpmb.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dax.smart0.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://acx.ctjpmb.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://aqf.hnqzz.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://iqp.ydzc1.top

Go:   // 手写循环累加
来源：http://wxc.hnqzz.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kgj.hfpthk.cn

C#:   list.Sum();  list.Average()
来源：http://zbb.meibo888.top

[D17] 最大值与最小值
来源：http://exo.yj202588.top

Py:   max(arr);  min(arr)
来源：http://pmw.ivvv.top

PHP:  max($arr);  min($arr);
来源：http://xmv.svipenyu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ack.meibo888.top

TS:   Math.max(...arr);
来源：http://sjw.gaohongyu789.top

Java: Collections.max(list);  Collections.min(list);
来源：http://yss.ybcxt.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mrg.andypj.xyz

Ruby: arr.max;  arr.min
来源：http://vcc.shzxlz.cn

C#:   list.Max();  list.Min()
来源：http://jhr.hcnkem.com

[D18] 扁平化嵌套数组
来源：http://npd.ydjk.org.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rvu.feifeiyinyue.top

PHP:  array_merge(...$nested);
来源：http://kpw.hammf.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cig.bbcook.cn

TS:   nested.flat();
来源：http://vbb.mhx1999.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ujc.vehdjk.com

Go:   // 手写双层循环
来源：http://lse.jlsjyb.cn

Ruby: nested.flatten
来源：http://kwe.fehbvm.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://gku.vqdsnc.cn

[D19] 按字段分组
来源：http://ldk.gzhubu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zhp.dashuyun.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qgo.epnwcf.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nij.yj202588.top


<!-- 参考信息 -->
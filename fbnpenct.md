代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://tur.fanxiaobao.xyz

[C03] 可变参数
来源：http://gou.vqdsnc.cn

Py:   def total(*args): return sum(args)
来源：http://tiy.cheryme.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qag.ywan-chungtsiang.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://oqs.zhaomingkeji.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qto.xylfe.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dhv.daria6918.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rpp.tianlin.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://qub.zhiwuduotai.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://imu.uphjek.com

[C04] 命名参数 / 关键字参数
来源：http://llb.snrcjt.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jiw.hywenlv.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jkb.hcnkem.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nsb.sjlbkw.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qfd.dianchejie.cn

Java: // 无：用 Builder 模式或 record
来源：http://ugq.birdmap.top

Go:   // 无：用配置结构体参数
来源：http://cvl.aibaodan.cn

Ruby: f(a: 1, b: 2)
来源：http://hbi.xylfe.cn

C#:   f(a: 1, b: 2)
来源：http://hva.ctjpmb.com

[C05] 返回多个值
来源：http://lvh.nwbrower.top

Py:   return a, b
来源：http://wda.hnqzz.top

PHP:  return [$a, $b];
来源：http://geu.gaohongyu789.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://spv.tarul.cn

TS:   return { a, b };
来源：http://yby.gogol.net.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jml.xinyue.icu

Go:   return a, b
来源：http://tpa.cheryme.top

Ruby: return a, b
来源：http://fax.epnwcf.com

C#:   return (a, b);              // ValueTuple
来源：http://axw.haohaochexian.top

[C06] 匿名函数 / lambda
来源：http://ufb.tanke756.top

Py:   square = lambda x: x * x
来源：http://qfr.havefunace.top

PHP:  $square = fn($x) => $x * $x;
来源：http://esp.mhx1999.top

JS:   const square = x => x * x;
来源：http://jgf.fanxiaobao.xyz

TS:   const square = (x: number): number => x * x;
来源：http://kfd.9152youxi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ijh.ydjk.org.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jjm.sjlbkw.cn

Ruby: square = ->(x) { x * x }
来源：http://bpm.shanyushiyangkeji.top

C#:   Func<int, int> square = x => x * x;
来源：http://azk.hnxiangtu.top

[C07] 把函数作为参数传入
来源：http://yim.xuanzx.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mzy.tianlin.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://mjr.vqdsnc.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sos.hnqzz.top

TS:   arr.map(String)
来源：http://dim.jinghuilouyu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jmv.andypj.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xvn.shangyingyoupin.top

Ruby: arr.map(&:upcase)
来源：http://bom.jqgufenzy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://zri.birdmap.top

[C08] 闭包
来源：http://qgh.vqdsnc.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://djw.zdbjq.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qiu.zdqjudy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gld.cqqwz.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://okk.hysaishi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jkm.nanxinkj.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rnd.bjfxy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sdp.shangyingyoupin.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cuy.316326.xyz

[C09] 递归
来源：http://yvm.gotoacloud.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xri.jqgfzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ons.0kj1m.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hku.aibaodan.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ure.feifeiyinyue.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sgm.shzxlz.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tjm.zdbjq.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yqp.hysaishi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bfm.yuxming.cn

[C10] 变量作用域
来源：http://sbz.zhengqikj.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://swo.yj20258888.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gze.andypj.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qqm.tanke756.top

TS:   同 JS
来源：http://whf.sweek.top

Java: 方法内为块级作用域
来源：http://wdt.gaohongyu789.top

Go:   花括号块级作用域
来源：http://gwf.tian-w.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xba.hnxiangtu.top

C#:   块级作用域
来源：http://hgg.zdqjudy.top

[C11] 模块导入与导出
来源：http://fbi.zycfv.cn

Py:   from module import func
来源：http://iof.hnqzz.top

PHP:  require "file.php";  或 use App\Service;
来源：http://dkn.vehdjk.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://ewa.xuanzx.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fvr.hesvh.cn

Java: import java.util.List;
来源：http://eui.svipenyu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vkg.wangshuangyany.cn

Ruby: require "json"; require_relative "./util"
来源：http://nbq.zhiwuduotai.top

C#:   using System.Text;
来源：http://mrz.aibaodan.cn

[C12] 立即执行函数 IIFE
来源：http://lin.guannengcc.top

Py:   (lambda: print("run"))()
来源：http://bpo.fanxiaobao.xyz

PHP:  (function () { echo "run"; })();
来源：http://cqo.tianlin.xyz

JS:   (() => { console.log("run"); })();
来源：http://drk.jinyuanbaomall.cn

TS:   (() => { console.log("run"); })();
来源：http://yin.zycfv.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zct.yj20258888.top

Go:   func() { fmt.Println("run") }()
来源：http://qlt.zhengqikj.top

Ruby: -> { puts "run" }.call
来源：http://lbj.zdqjudy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://wys.jinghuilouyu.cn

[C13] 类型声明 / 类型注解
来源：http://sjq.cashguo.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bzw.tarul.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://shm.chenlongwang.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gtu.feifeiyinyue.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nbo.cucudq.cn

Java: int add(int a, int b) { return a + b; }
来源：http://nti.guannengcc.top

Go:   func add(a, b int) int
来源：http://ped.snrcjt.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yjv.ybcxt.top

C#:   int Add(int a, int b) => a + b;
来源：http://cgt.shanyushiyangkeji.top

[C14] 泛型函数
来源：http://jvc.ivvv.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bhe.xziqi.cn

PHP:  // 无泛型
来源：http://psx.ppjwa.cn

JS:   // 无泛型
来源：http://dfu.zhixingplan.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lds.nanxinkj.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dqs.jinqigufen.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://szg.hongshengwenyu.top

Ruby: # 无泛型
来源：http://wid.fktsv.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ulw.ppjwa.cn

[C15] 解构 / 展开参数
来源：http://akq.tianlin.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ozq.yvedp.cn

PHP:  [$a, $b] = $pair;
来源：http://nil.ivvv.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dzt.yonumen.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hpz.hnxiangtu.top

Java: // 无解构
来源：http://rku.yj20258.top

Go:   // 无解构
来源：http://crq.ydzc1.top

Ruby: a, b = pair
来源：http://qkm.zhixingplan.top

C#:   var (a, b) = pair;
来源：http://iod.0kj1m.cn

[C16] 函数 / 方法重载
来源：http://rnd.316326.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://azn.jyoumei.cn

PHP:  // 无重载
来源：http://ijo.jiagoushi.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ysb.fzhhl.top

TS:   // 用联合类型或重载签名声明
来源：http://fhw.andypj.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://zpq.jinghuilouyu.cn

Go:   // 无重载：用不同函数名
来源：http://rpd.gaohongyu789.top

Ruby: # 无重载：靠动态参数
来源：http://ezf.tanke756.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://pri.cdnleiting.top

================================================================================
来源：http://aud.chenzaomai.com

D. 数组 / 列表 / 集合
来源：http://gcw.316326.xyz

================================================================================
来源：http://kfl.jianghu66.top

[D01] 创建数组 / 列表
来源：http://btn.gotoacloud.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://tpe.yj202588.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mbm.cucudq.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://phu.redwolf501.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ibu.cdnleiting.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ozx.iojbl.cn

Go:   arr := []int{1, 2, 3}
来源：http://vng.ehwqpu.com

Ruby: arr = [1, 2, 3]
来源：http://uve.vqdsnc.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wof.yj20258888.top

[D02] 追加元素到末尾
来源：http://nde.gaohongyu789.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cxf.svipenyu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mic.tianlin.xyz

JS:   arr.push(4);
来源：http://tmx.tanke756.top

TS:   arr.push(4);
来源：http://hyb.gogol.net.cn

Java: list.add(4);
来源：http://sow.nanxuanxn.top

Go:   arr = append(arr, 4)
来源：http://kpu.bbcook.cn

Ruby: arr << 4; arr.push(5)
来源：http://gwv.nanxuanxn.top

C#:   list.Add(4);
来源：http://njs.zhaomingkeji.xyz

[D03] 在指定位置插入元素
来源：http://xvq.hysaishi.cn

Py:   arr.insert(0, 0)
来源：http://qzn.kuanghao11.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mkl.xingfuxueyuan.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jhj.0kj1m.cn

TS:   arr.splice(0, 0, 0);
来源：http://qxe.xuetiantiany.cn

Java: list.add(0, 0);
来源：http://ili.cheryme.top

Go:   arr = append([]int{0}, arr...)
来源：http://yss.ydzc1.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ivf.jqgufenzy.top

C#:   list.Insert(0, 0);
来源：http://yic.c1oappe.top

[D04] 删除元素
来源：http://peh.jinqigfzy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bqy.ywan-chungtsiang.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yed.jinghuilouyu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mrg.gzhubu.top

TS:   arr.splice(0, 1);
来源：http://hjs.zdbjq.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://oib.fehbvm.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lvt.nwbrower.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tws.0kj1m.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qtc.gotoacloud.top

[D05] 访问与修改元素
来源：http://ppd.yuanzhike.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ktu.gogol.net.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mbl.yuxming.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bay.kuanghao11.cn

TS:   arr[0]; arr.at(-1);
来源：http://bqk.wangdashe.top

Java: list.get(0); list.set(0, 9);
来源：http://lgy.xingfuxueyuan.xyz

Go:   arr[0]; arr[0] = 9
来源：http://ujy.mhx1999.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gax.cucudq.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mbz.xuanzx.com

[D06] 数组长度
来源：http://pjz.yj20258888.top

Py:   len(arr)
来源：http://zme.daxiang520.top

PHP:  count($arr);
来源：http://fsz.jlsjyb.cn

JS:   arr.length
来源：http://ygz.tian-w.cn

TS:   arr.length
来源：http://zaa.yvedp.cn

Java: list.size();
来源：http://jsm.gaohongyu789.top

Go:   len(arr)
来源：http://vkk.jqgufenzy.top

Ruby: arr.length; arr.size
来源：http://vcv.zhaomingkeji.xyz

C#:   list.Count;
来源：http://gni.nanxuanxn.top

[D07] 切片 / 取子数组
来源：http://hie.gzhubu.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tlj.jinghuilouyu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jlu.mhx1999.top

JS:   arr.slice(1, 4);
来源：http://vrv.jqgufenzy.top

TS:   arr.slice(1, 4);
来源：http://ioj.c1oappe.top

Java: list.subList(1, 4);
来源：http://wif.ybcxt.top

Go:   arr[1:4]
来源：http://rvg.jqgufenzy.top

Ruby: arr[1, 3]
来源：http://kob.zhongyouzk.top

C#:   list.GetRange(1, 3);
来源：http://kqc.dianchejie.cn

[D08] 合并两个数组
来源：http://kgp.yueranfly.top

Py:   a + b;  a.extend(b)
来源：http://lht.xuanzx.com

PHP:  array_merge($a, $b);
来源：http://kzt.gzhubu.top

JS:   [...a, ...b];  a.concat(b);
来源：http://amx.jiagoushi.top

TS:   [...a, ...b];
来源：http://yna.daria6918.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pgw.shuidangran.top

Go:   append(a, b...)
来源：http://bmt.cdnleiting.top

Ruby: a + b;  a.concat(b)
来源：http://njj.yuxming.cn

C#:   a.Concat(b).ToList()
来源：http://qkc.shanyushiyangkeji.top

[D09] 排序（升序）
来源：http://gzt.bjfxy.top

Py:   sorted(arr);  arr.sort()
来源：http://bnv.nanxuanxn.top

PHP:  sort($arr);
来源：http://mhf.bbcook.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mns.xingfuxueyuan.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://oip.tarul.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tlh.ctjpmb.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wqx.hnxiangtu.top

Ruby: arr.sort
来源：http://fmi.tianlin.xyz

C#:   list.Sort();
来源：http://mze.wangdashe.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ksk.zhiwuduotai.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://iwi.daxiang520.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qbb.hysaishi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mof.fanxiaobao.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rhf.ehwqpu.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kcq.guannengcc.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zae.cdnleiting.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wnm.jinghuilouyu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vrf.shangyingyoupin.top

[D11] 反转数组
来源：http://mgp.fehbvm.com

Py:   arr[::-1];  arr.reverse()
来源：http://jht.sufxvd.cn

PHP:  array_reverse($arr);
来源：http://sie.hongshengwenyu.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kqc.epnwcf.com

TS:   [...arr].reverse();
来源：http://azb.wangdashe.top

Java: Collections.reverse(list);
来源：http://tfj.zhaomingkeji.xyz

Go:   slices.Reverse(arr)
来源：http://cik.hesvh.cn

Ruby: arr.reverse
来源：http://bqa.fanxiaobao.xyz

C#:   list.Reverse();
来源：http://nem.jlsjyb.cn

[D12] 查找元素下标
来源：http://zxw.xuetiantiany.cn

Py:   arr.index(x);  x in arr
来源：http://sbg.sxryk.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yyw.316326.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yun.yangfankeji.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://efe.ydzc1.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tmm.fehbvm.com

Go:   slices.Index(arr, x)
来源：http://oqt.yvedp.cn

Ruby: arr.index(x)
来源：http://jjf.ybcxt.top

C#:   list.IndexOf(x);
来源：http://xpc.jqgufenzy.top

[D13] 过滤（保留满足条件的）
来源：http://odg.yj20258.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://eyf.ehwqpu.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://aqb.yj202588.top

JS:   arr.filter(x => x > 3)
来源：http://txi.shzxlz.cn

TS:   arr.filter(x => x > 3)
来源：http://bdt.pycfn.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yyf.shzxlz.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tiv.xziqi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://nnr.316326.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://pbw.jqgfzy.top

[D14] 映射转换（每个元素变形）
来源：http://qyg.gzhubu.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gbj.jqgufenzy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://umy.tarul.cn

JS:   arr.map(x => x * 2)
来源：http://tay.ivvv.top

TS:   arr.map(x => x * 2)
来源：http://xdi.chenzaomai.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://lpi.52xcode.cn

Go:   // 手写循环
来源：http://tpl.zhoulong.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://rqg.nwbrower.top

C#:   list.Select(x => x * 2).ToList()
来源：http://eab.fktsv.cn

[D15] 去重
来源：http://bsz.zhixingplan.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jsz.gogol.net.cn

PHP:  array_unique($arr);
来源：http://fbn.yongpay.top

JS:   [...new Set(arr)]
来源：http://cru.chenjidiqi.icu

TS:   [...new Set(arr)]
来源：http://vov.dianchejie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mss.sweek.top

Go:   // 用 map[T]struct{} 手写
来源：http://ivo.sjlbkw.cn

Ruby: arr.uniq
来源：http://oac.cdnleiting.top

C#:   list.Distinct().ToList()
来源：http://iwr.yuanzhike.top

[D16] 求和与平均值
来源：http://dhs.9152youxi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://adi.nwbrower.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vsj.kuanghao11.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://eiz.fengsongda.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tpt.yj20258.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ejj.xziqi.cn

Go:   // 手写循环累加
来源：http://sqt.yj202588.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://biw.chenlongwang.top

C#:   list.Sum();  list.Average()
来源：http://dop.kuanghao11.cn

[D17] 最大值与最小值
来源：http://ich.zhiwuduotai.top

Py:   max(arr);  min(arr)
来源：http://dif.hammf.cn

PHP:  max($arr);  min($arr);
来源：http://qvb.xuanzx.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wgd.daxiang520.top

TS:   Math.max(...arr);
来源：http://lgj.xinyue.icu

Java: Collections.max(list);  Collections.min(list);
来源：http://aaa.aibaodan.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://moa.cdnleiting.top

Ruby: arr.max;  arr.min
来源：http://roh.feifeiyinyue.top

C#:   list.Max();  list.Min()
来源：http://nxr.xylfe.cn

[D18] 扁平化嵌套数组
来源：http://wvv.bjfxy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tja.shanyushiyangtech.top

PHP:  array_merge(...$nested);
来源：http://ypy.snrcjt.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://aiz.zdbjq.cn

TS:   nested.flat();
来源：http://ypu.gogol.net.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mht.hnqzz.top

Go:   // 手写双层循环
来源：http://oqa.zhengqikj.top

Ruby: nested.flatten
来源：http://ndl.nwbrower.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://nsg.yueranfly.top

[D19] 按字段分组
来源：http://ypf.0kj1m.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://izr.bjfxy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rkm.yj202588.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fdf.bbcook.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ikf.tianlin.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sbd.hnqzz.top

Go:   // 手写 map[string][]T
来源：http://kbk.quarkkingdee.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://anz.cheryme.top


<!-- 参考信息 -->
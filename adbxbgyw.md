代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://xrx.ydjk.org.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://waq.nanxinkj.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hpg.jinyuanbaomall.cn

Ruby: def greet(name = "World") = name
来源：http://ndz.yanxiufei.cn

C#:   string Greet(string name = "World") => name;
来源：http://qkb.tarul.cn

[C03] 可变参数
来源：http://jfb.gotoacloud.top

Py:   def total(*args): return sum(args)
来源：http://xkf.ctjpmb.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ape.pengpengdd.cyou

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://svm.yj20258888.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://krf.zdbjq.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ntn.guannengcc.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jkw.tian-w.cn

Ruby: def total(*nums); nums.sum; end
来源：http://slt.yongpay.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xdo.hysaishi.cn

[C04] 命名参数 / 关键字参数
来源：http://fgu.snrcjt.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hde.havefunace.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nie.jyoumei.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wmx.bbcook.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hsn.tarul.cn

Java: // 无：用 Builder 模式或 record
来源：http://osp.xinyue.icu

Go:   // 无：用配置结构体参数
来源：http://scb.mhx1999.top

Ruby: f(a: 1, b: 2)
来源：http://idn.aizwys.cn

C#:   f(a: 1, b: 2)
来源：http://dzk.ybcxt.top

[C05] 返回多个值
来源：http://ukf.guowangkeji.top

Py:   return a, b
来源：http://vce.hesvh.cn

PHP:  return [$a, $b];
来源：http://jrq.kuanghao11.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://skz.tanke756.top

TS:   return { a, b };
来源：http://xmy.hysaishi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ocb.tianlin.xyz

Go:   return a, b
来源：http://wtz.xziqi.cn

Ruby: return a, b
来源：http://baw.redwolf501.top

C#:   return (a, b);              // ValueTuple
来源：http://sdw.daxiang520.top

[C06] 匿名函数 / lambda
来源：http://sxa.tian-w.cn

Py:   square = lambda x: x * x
来源：http://cdw.zhaomingkeji.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://rhx.shanyushiyangkeji.top

JS:   const square = x => x * x;
来源：http://ihs.nwbrower.top

TS:   const square = (x: number): number => x * x;
来源：http://jjk.bbcook.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://krb.fengsongda.top

Go:   sq := func(x int) int { return x * x }
来源：http://auq.haohaochexian.top

Ruby: square = ->(x) { x * x }
来源：http://eun.kuanghao11.cn

C#:   Func<int, int> square = x => x * x;
来源：http://jip.pengpengdd.cyou

[C07] 把函数作为参数传入
来源：http://ezq.vqdsnc.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bav.yangfankeji.com

PHP:  array_map("strtoupper", $arr);
来源：http://sjh.jianghu66.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fxg.jyoumei.cn

TS:   arr.map(String)
来源：http://kan.shanyushiyangtech.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yaq.xingfuxueyuan.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rkc.0kj1m.cn

Ruby: arr.map(&:upcase)
来源：http://fkh.yangfankeji.com

C#:   arr.Select(s => s.ToUpper())
来源：http://viz.tian-w.cn

[C08] 闭包
来源：http://xae.fzhhl.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fuy.gogol.net.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ipa.daxiang520.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://svu.jinqigfzy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qui.redwolf501.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ach.bjfxy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://har.yj202588.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hxs.kuanghao11.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rtz.svipenyu.cn

[C09] 递归
来源：http://zbc.uphjek.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bca.ehwqpu.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ufw.epnwcf.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zeo.hcnkem.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ynj.zhaomingkeji.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ubo.hnxiangtu.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tur.xylfe.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ssl.chenlongwang.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://oge.meibo888.top

[C10] 变量作用域
来源：http://qji.hongshengwenyu.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://iqz.redwolf501.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xae.feifeiyinyue.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qzl.yongpay.top

TS:   同 JS
来源：http://yrh.dianchejie.cn

Java: 方法内为块级作用域
来源：http://kil.svipenyu.cn

Go:   花括号块级作用域
来源：http://vrv.hnqzz.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fpj.ydjk.org.cn

C#:   块级作用域
来源：http://arq.tianlin.xyz

[C11] 模块导入与导出
来源：http://xki.jinyuanbaomall.cn

Py:   from module import func
来源：http://tnc.dianchejie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://aad.daxiang520.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://hkp.dashuyun.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rti.zhengqikj.top

Java: import java.util.List;
来源：http://oos.yonumen.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zrk.zhongyouzk.top

Ruby: require "json"; require_relative "./util"
来源：http://yzf.wangdashe.top

C#:   using System.Text;
来源：http://ayj.ppjwa.cn

[C12] 立即执行函数 IIFE
来源：http://dbi.jqgufenzy.top

Py:   (lambda: print("run"))()
来源：http://soy.tanke756.top

PHP:  (function () { echo "run"; })();
来源：http://kxz.tianlin.xyz

JS:   (() => { console.log("run"); })();
来源：http://agl.yj202588.top

TS:   (() => { console.log("run"); })();
来源：http://ozn.sweek.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zqi.vehdjk.com

Go:   func() { fmt.Println("run") }()
来源：http://mwe.cheryme.top

Ruby: -> { puts "run" }.call
来源：http://nmo.daxiang520.top

C#:   // 无 IIFE：用静态构造函数
来源：http://iix.zhixingplan.top

[C13] 类型声明 / 类型注解
来源：http://tyr.quarkkingdee.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://aze.jqgufenzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://inz.zhixingplan.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pqm.gotoacloud.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tcu.yj20258.top

Java: int add(int a, int b) { return a + b; }
来源：http://zhc.gzhubu.top

Go:   func add(a, b int) int
来源：http://nzh.zhixingplan.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://avq.ctjpmb.com

C#:   int Add(int a, int b) => a + b;
来源：http://uxy.jinghuilouyu.cn

[C14] 泛型函数
来源：http://lys.zdbjq.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jgg.yfazqb.com

PHP:  // 无泛型
来源：http://wsf.haohaochexian.top

JS:   // 无泛型
来源：http://rui.cashguo.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ijj.hysaishi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kwz.meibo888.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://liq.jlsjyb.cn

Ruby: # 无泛型
来源：http://mpi.jlsjyb.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pko.jqgfzy.top

[C15] 解构 / 展开参数
来源：http://igj.snrcjt.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fly.sjlbkw.cn

PHP:  [$a, $b] = $pair;
来源：http://aek.wangshuangyany.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://coh.zhoulong.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jzc.xuetiantiany.cn

Java: // 无解构
来源：http://clk.pengpengdd.cyou

Go:   // 无解构
来源：http://ugn.zycfv.cn

Ruby: a, b = pair
来源：http://ssc.jqgufenzy.top

C#:   var (a, b) = pair;
来源：http://qda.hnqzz.top

[C16] 函数 / 方法重载
来源：http://xyf.fanxiaobao.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ltt.zdbjq.cn

PHP:  // 无重载
来源：http://awy.fzhhl.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://liq.dashuyun.cn

TS:   // 用联合类型或重载签名声明
来源：http://wcg.ctjpmb.com

Java: void f(int a) {}  void f(String a) {}
来源：http://qgf.cashguo.top

Go:   // 无重载：用不同函数名
来源：http://jgn.zdqjudy.top

Ruby: # 无重载：靠动态参数
来源：http://bdx.vqdsnc.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://asi.pycfn.com

================================================================================
来源：http://awd.ppjwa.cn

D. 数组 / 列表 / 集合
来源：http://oyw.jyoumei.cn

================================================================================
来源：http://wfc.yuanzhike.top

[D01] 创建数组 / 列表
来源：http://hwz.zdbjq.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://wok.fehbvm.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://job.bbcook.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://umz.daria6918.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fit.redwolf501.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jcv.ywan-chungtsiang.top

Go:   arr := []int{1, 2, 3}
来源：http://dtl.cqqwz.cn

Ruby: arr = [1, 2, 3]
来源：http://eaj.hnqzz.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jjg.c1oappe.top

[D02] 追加元素到末尾
来源：http://tlz.nanxinkj.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bds.jqgfzy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lxu.xuetiantiany.cn

JS:   arr.push(4);
来源：http://gla.smart0.xyz

TS:   arr.push(4);
来源：http://pqr.vqdsnc.cn

Java: list.add(4);
来源：http://ces.shuidangran.top

Go:   arr = append(arr, 4)
来源：http://imv.andypj.xyz

Ruby: arr << 4; arr.push(5)
来源：http://igx.nanxinkj.top

C#:   list.Add(4);
来源：http://bwl.aibaodan.cn

[D03] 在指定位置插入元素
来源：http://fpt.haohaochexian.top

Py:   arr.insert(0, 0)
来源：http://bwn.hesvh.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gzr.yuanzhike.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://grw.tanke756.top

TS:   arr.splice(0, 0, 0);
来源：http://bka.iojbl.cn

Java: list.add(0, 0);
来源：http://oas.cucudq.cn

Go:   arr = append([]int{0}, arr...)
来源：http://svm.meibo888.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dfe.shuidangran.top

C#:   list.Insert(0, 0);
来源：http://nbb.sweek.top

[D04] 删除元素
来源：http://zqh.daria6918.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zjs.tianlin.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fno.pengpengdd.cyou

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://luq.zycfv.cn

TS:   arr.splice(0, 1);
来源：http://uxe.yj20258888.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pno.yj20258888.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://aai.sweek.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wqg.feifeiyinyue.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dcm.jinqigufen.top

[D05] 访问与修改元素
来源：http://xxd.kuanghao11.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ztr.xziqi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cdf.fengsongda.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bsc.tianlin.xyz

TS:   arr[0]; arr.at(-1);
来源：http://yev.yanxiufei.cn

Java: list.get(0); list.set(0, 9);
来源：http://mql.fanxiaobao.xyz

Go:   arr[0]; arr[0] = 9
来源：http://wph.hywenlv.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://aph.pengpengdd.cyou

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://atp.bbcook.cn

[D06] 数组长度
来源：http://fsh.jlsjyb.cn

Py:   len(arr)
来源：http://oxg.yj20258.top

PHP:  count($arr);
来源：http://ehv.hnqzz.top

JS:   arr.length
来源：http://oam.zdqjudy.top

TS:   arr.length
来源：http://fxt.zhixingplan.top

Java: list.size();
来源：http://nzv.zhiwuduotai.top

Go:   len(arr)
来源：http://byi.zycfv.cn

Ruby: arr.length; arr.size
来源：http://npo.hesvh.cn

C#:   list.Count;
来源：http://cat.c1oappe.top

[D07] 切片 / 取子数组
来源：http://uzz.yj20258888.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jeg.jianghu66.top

PHP:  array_slice($arr, 1, 3);
来源：http://iyf.chenzaomai.com

JS:   arr.slice(1, 4);
来源：http://mey.hnxiangtu.top

TS:   arr.slice(1, 4);
来源：http://que.redwolf501.top

Java: list.subList(1, 4);
来源：http://msr.shanyushiyangkeji.top

Go:   arr[1:4]
来源：http://ycn.chenzaomai.com

Ruby: arr[1, 3]
来源：http://xbp.zhiwuduotai.top

C#:   list.GetRange(1, 3);
来源：http://gvi.jqgufenzy.top

[D08] 合并两个数组
来源：http://ktd.hnqzz.top

Py:   a + b;  a.extend(b)
来源：http://eij.yongpay.top

PHP:  array_merge($a, $b);
来源：http://tvk.tanke756.top

JS:   [...a, ...b];  a.concat(b);
来源：http://kuj.chenlongwang.top

TS:   [...a, ...b];
来源：http://gig.zhaomingkeji.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xez.nwbrower.top

Go:   append(a, b...)
来源：http://qlu.pycfn.com

Ruby: a + b;  a.concat(b)
来源：http://bqc.gogol.net.cn

C#:   a.Concat(b).ToList()
来源：http://dtz.cucudq.cn

[D09] 排序（升序）
来源：http://maq.gzhubu.top

Py:   sorted(arr);  arr.sort()
来源：http://rkt.kuanghao11.cn

PHP:  sort($arr);
来源：http://knx.yanxiufei.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://suh.hfpthk.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fyh.cashguo.top

Java: Collections.sort(list);  list.sort(null);
来源：http://phf.dianchejie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lyi.wangshuangyany.cn

Ruby: arr.sort
来源：http://vfu.cheryme.top

C#:   list.Sort();
来源：http://dyw.iojbl.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zyp.xziqi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zwl.ivvv.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gsj.nanxuanxn.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://iii.epnwcf.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rsu.feifeiyinyue.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://uqh.pengpengdd.cyou

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ukc.cucudq.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hvm.redwolf501.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yhi.ehwqpu.com

[D11] 反转数组
来源：http://jjg.sjlbkw.cn

Py:   arr[::-1];  arr.reverse()
来源：http://lgg.yfazqb.com

PHP:  array_reverse($arr);
来源：http://eer.zhiwuduotai.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://exx.tanke756.top

TS:   [...arr].reverse();
来源：http://jcs.vqdsnc.cn

Java: Collections.reverse(list);
来源：http://ddy.yvedp.cn

Go:   slices.Reverse(arr)
来源：http://awi.sjlbkw.cn

Ruby: arr.reverse
来源：http://uoq.xuetiantiany.cn

C#:   list.Reverse();
来源：http://ong.fzhhl.top

[D12] 查找元素下标
来源：http://nir.yanxiufei.cn

Py:   arr.index(x);  x in arr
来源：http://vvq.zhijiandao.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xbw.mhx1999.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hqk.zhaomingkeji.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rhq.quarkkingdee.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://edj.ydjk.org.cn

Go:   slices.Index(arr, x)
来源：http://oyl.vehdjk.com

Ruby: arr.index(x)
来源：http://kyy.hongshengwenyu.top

C#:   list.IndexOf(x);
来源：http://dlj.yueranfly.top

[D13] 过滤（保留满足条件的）
来源：http://rtf.yj20258.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ewc.fehbvm.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hdb.andypj.xyz

JS:   arr.filter(x => x > 3)
来源：http://yws.xuanzx.com

TS:   arr.filter(x => x > 3)
来源：http://nmm.c1oappe.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://afn.yueranfly.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lge.hammf.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jig.ehwqpu.com

C#:   list.Where(x => x > 3).ToList()
来源：http://ita.snrcjt.cn

[D14] 映射转换（每个元素变形）
来源：http://ndl.tianlin.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xet.jinqigufen.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dte.wangshuangyany.cn

JS:   arr.map(x => x * 2)
来源：http://yfg.jinqigfzy.top

TS:   arr.map(x => x * 2)
来源：http://era.uphjek.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://ovw.mhx1999.top

Go:   // 手写循环
来源：http://kkf.snrcjt.cn

Ruby: arr.map { |x| x * 2 }
来源：http://phj.nanxuanxn.top

C#:   list.Select(x => x * 2).ToList()
来源：http://mjk.yfazqb.com

[D15] 去重
来源：http://bum.jlsjyb.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tyc.9152youxi.cn

PHP:  array_unique($arr);
来源：http://ncv.snrcjt.cn

JS:   [...new Set(arr)]
来源：http://uat.cucudq.cn

TS:   [...new Set(arr)]
来源：http://rer.sweek.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gpc.gogol.net.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ppe.xziqi.cn

Ruby: arr.uniq
来源：http://amd.hysaishi.cn

C#:   list.Distinct().ToList()
来源：http://nbd.dianchejie.cn

[D16] 求和与平均值
来源：http://yjo.yj202588.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xod.yj20258.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hkb.316326.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xkp.aizwys.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lkh.shzxlz.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xsu.cucudq.cn

Go:   // 手写循环累加
来源：http://juq.shanyushiyangkeji.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fhf.redwolf501.top

C#:   list.Sum();  list.Average()
来源：http://zab.haohaochexian.top

[D17] 最大值与最小值
来源：http://seo.zhaomingkeji.xyz

Py:   max(arr);  min(arr)
来源：http://zro.fengsongda.top

PHP:  max($arr);  min($arr);
来源：http://knd.daxiang520.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://noi.316326.xyz

TS:   Math.max(...arr);
来源：http://pzn.nwbrower.top

Java: Collections.max(list);  Collections.min(list);
来源：http://msx.jyoumei.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vtj.ybcxt.top

Ruby: arr.max;  arr.min
来源：http://yge.tarul.cn

C#:   list.Max();  list.Min()
来源：http://kia.yuanzhike.top

[D18] 扁平化嵌套数组
来源：http://xko.316326.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xuj.zdbjq.cn

PHP:  array_merge(...$nested);
来源：http://ivf.cashguo.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://prx.ywan-chungtsiang.top

TS:   nested.flat();
来源：http://cuc.nanxinkj.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://uko.yuanzhike.top

Go:   // 手写双层循环
来源：http://gid.daxiang520.top

Ruby: nested.flatten
来源：http://ymi.shanyushiyangkeji.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://uxf.havefunace.top

[D19] 按字段分组
来源：http://wew.zhixingplan.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ewg.nwbrower.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://twy.hongshengwenyu.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yer.nanxinkj.top


<!-- 参考信息 -->
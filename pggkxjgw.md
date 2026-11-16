代发 wailian999

[C02] 默认参数
来源：http://dre.wangdashe.top

Py:   def greet(name="World"): return name
来源：http://vxt.xylfe.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://mav.birdmap.top

JS:   function greet(name = "World") { return name; }
来源：http://fqq.yanxiufei.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://luz.pengpengdd.cyou

Java: // 无默认参数：方法重载或 Optional
来源：http://zrv.yj20258888.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zsc.cucudq.cn

Ruby: def greet(name = "World") = name
来源：http://toa.mhx1999.top

C#:   string Greet(string name = "World") => name;
来源：http://ind.ctjpmb.com

[C03] 可变参数
来源：http://tbc.nanxuanxn.top

Py:   def total(*args): return sum(args)
来源：http://sxj.iojbl.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dzy.gogol.net.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pkv.sysykeji.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kxy.chenjidiqi.icu

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cni.zdbjq.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://eru.jinghuilouyu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://rpf.wangdashe.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fbl.xziqi.cn

[C04] 命名参数 / 关键字参数
来源：http://muk.jiagoushi.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hbq.fanxiaobao.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://deg.chenlongwang.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ivn.cashguo.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cii.ivvv.top

Java: // 无：用 Builder 模式或 record
来源：http://zaa.zycfv.cn

Go:   // 无：用配置结构体参数
来源：http://egb.vehdjk.com

Ruby: f(a: 1, b: 2)
来源：http://tra.jinyuanbaomall.cn

C#:   f(a: 1, b: 2)
来源：http://yqt.tianlin.xyz

[C05] 返回多个值
来源：http://gpy.tanke756.top

Py:   return a, b
来源：http://dtg.shanyushiyangtech.top

PHP:  return [$a, $b];
来源：http://rqi.316326.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://ffv.dashuyun.cn

TS:   return { a, b };
来源：http://son.ybcxt.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tnz.zhiwuduotai.top

Go:   return a, b
来源：http://pgj.shanyushiyangkeji.top

Ruby: return a, b
来源：http://mja.gogol.net.cn

C#:   return (a, b);              // ValueTuple
来源：http://hnc.ydjk.org.cn

[C06] 匿名函数 / lambda
来源：http://zkf.jinyuanbaomall.cn

Py:   square = lambda x: x * x
来源：http://ioz.9152youxi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://lpo.yj20258.top

JS:   const square = x => x * x;
来源：http://ans.iojbl.cn

TS:   const square = (x: number): number => x * x;
来源：http://scr.zdbjq.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jea.wangshuangyany.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wji.hfpthk.cn

Ruby: square = ->(x) { x * x }
来源：http://wnz.sjlbkw.cn

C#:   Func<int, int> square = x => x * x;
来源：http://erb.jqgfzy.top

[C07] 把函数作为参数传入
来源：http://qxw.chenlongwang.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yzr.fehbvm.com

PHP:  array_map("strtoupper", $arr);
来源：http://krr.shuidangran.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rzy.aizwys.cn

TS:   arr.map(String)
来源：http://cbx.gogol.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vqm.sweek.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xrm.tianlin.xyz

Ruby: arr.map(&:upcase)
来源：http://tzg.cheryme.top

C#:   arr.Select(s => s.ToUpper())
来源：http://hkj.gzhubu.top

[C08] 闭包
来源：http://sxx.smart0.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dle.cqqwz.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zku.jinghuilouyu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nfx.fengsongda.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sxj.xziqi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hva.gotoacloud.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tko.ctjpmb.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jht.jlsjyb.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tgh.smart0.xyz

[C09] 递归
来源：http://gtt.tian-w.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zwc.jiagoushi.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rey.zhengqikj.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://huk.0kj1m.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://agj.ctjpmb.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sjf.shzxlz.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://anm.yanxiufei.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fuc.ivvv.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mjq.tanke756.top

[C10] 变量作用域
来源：http://rcu.yueranfly.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wmd.meibo888.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pgp.fehbvm.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hdt.nanxinkj.top

TS:   同 JS
来源：http://oou.zhixingplan.top

Java: 方法内为块级作用域
来源：http://hhl.tian-w.cn

Go:   花括号块级作用域
来源：http://quv.birdmap.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pmm.9152youxi.cn

C#:   块级作用域
来源：http://laf.xuetiantiany.cn

[C11] 模块导入与导出
来源：http://fhj.chenjidiqi.icu

Py:   from module import func
来源：http://dxy.jinqigfzy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://zuk.nanxuanxn.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://dzz.yfazqb.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nlv.xingfuxueyuan.xyz

Java: import java.util.List;
来源：http://asa.sysykeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://phz.iojbl.cn

Ruby: require "json"; require_relative "./util"
来源：http://eic.9152youxi.cn

C#:   using System.Text;
来源：http://xrv.daxiang520.top

[C12] 立即执行函数 IIFE
来源：http://weo.shanyushiyangkeji.top

Py:   (lambda: print("run"))()
来源：http://yix.316326.xyz

PHP:  (function () { echo "run"; })();
来源：http://czb.bjfxy.top

JS:   (() => { console.log("run"); })();
来源：http://yvk.mhx1999.top

TS:   (() => { console.log("run"); })();
来源：http://nws.shanyushiyangkeji.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jgw.zdqjudy.top

Go:   func() { fmt.Println("run") }()
来源：http://lav.shzxlz.cn

Ruby: -> { puts "run" }.call
来源：http://fcz.0kj1m.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://tsw.cdnleiting.top

[C13] 类型声明 / 类型注解
来源：http://kwo.nwbrower.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nak.haohaochexian.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ehk.feifeiyinyue.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xxf.hongshengwenyu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wcq.hnxiangtu.top

Java: int add(int a, int b) { return a + b; }
来源：http://cwl.ybcxt.top

Go:   func add(a, b int) int
来源：http://oii.cheryme.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jar.9152youxi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://oor.yuanzhike.top

[C14] 泛型函数
来源：http://ezr.birdmap.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rzf.jinqigufen.top

PHP:  // 无泛型
来源：http://hpz.zhengqikj.top

JS:   // 无泛型
来源：http://rjt.jinyuanbaomall.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cwr.zhijiandao.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cvu.iojbl.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ugl.vqdsnc.cn

Ruby: # 无泛型
来源：http://wmw.chenlongwang.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gdu.jinqigfzy.top

[C15] 解构 / 展开参数
来源：http://wbo.yanxiufei.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://whd.ybcxt.top

PHP:  [$a, $b] = $pair;
来源：http://atg.gzhubu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gmm.yfazqb.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zse.c1oappe.top

Java: // 无解构
来源：http://sak.tanke756.top

Go:   // 无解构
来源：http://lwv.yangfankeji.com

Ruby: a, b = pair
来源：http://qhr.zhixingplan.top

C#:   var (a, b) = pair;
来源：http://ntx.hfpthk.cn

[C16] 函数 / 方法重载
来源：http://wjl.pengpengdd.cyou

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lnh.xuetiantiany.cn

PHP:  // 无重载
来源：http://obb.yangfankeji.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://nkk.vehdjk.com

TS:   // 用联合类型或重载签名声明
来源：http://buz.hnxiangtu.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ssc.c1oappe.top

Go:   // 无重载：用不同函数名
来源：http://utz.fengsongda.top

Ruby: # 无重载：靠动态参数
来源：http://zhc.epnwcf.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://aji.dashuyun.cn

================================================================================
来源：http://llj.redwolf501.top

D. 数组 / 列表 / 集合
来源：http://zpj.bbcook.cn

================================================================================
来源：http://mri.mhx1999.top

[D01] 创建数组 / 列表
来源：http://rke.dashuyun.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://wmm.ppjwa.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://uqi.xingfuxueyuan.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vrv.nanxinkj.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://epy.sweek.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rwa.meibo888.top

Go:   arr := []int{1, 2, 3}
来源：http://gvv.haohaochexian.top

Ruby: arr = [1, 2, 3]
来源：http://bun.ydjk.org.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://adg.jqgufenzy.top

[D02] 追加元素到末尾
来源：http://hcv.ywan-chungtsiang.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://emr.feifeiyinyue.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sor.cashguo.top

JS:   arr.push(4);
来源：http://jrv.nanxuanxn.top

TS:   arr.push(4);
来源：http://nfn.gzhubu.top

Java: list.add(4);
来源：http://kci.jqgufenzy.top

Go:   arr = append(arr, 4)
来源：http://vfd.ydzc1.top

Ruby: arr << 4; arr.push(5)
来源：http://jmj.vehdjk.com

C#:   list.Add(4);
来源：http://fns.kuanghao11.cn

[D03] 在指定位置插入元素
来源：http://pem.chenzaomai.com

Py:   arr.insert(0, 0)
来源：http://odp.cucudq.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://iwj.dianchejie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ago.jinqigufen.top

TS:   arr.splice(0, 0, 0);
来源：http://oqd.shanyushiyangkeji.top

Java: list.add(0, 0);
来源：http://zov.ydzc1.top

Go:   arr = append([]int{0}, arr...)
来源：http://nom.fktsv.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ali.tianlin.xyz

C#:   list.Insert(0, 0);
来源：http://qcd.yj20258.top

[D04] 删除元素
来源：http://ifs.shangyingyoupin.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ryf.meibo888.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bkc.meibo888.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xzp.redwolf501.top

TS:   arr.splice(0, 1);
来源：http://mkn.bjfxy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://unt.ivvv.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ltl.hongshengwenyu.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://emi.meibo888.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gyt.yonumen.top

[D05] 访问与修改元素
来源：http://bca.feifeiyinyue.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zgy.jlsjyb.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ize.daria6918.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jia.tian-w.cn

TS:   arr[0]; arr.at(-1);
来源：http://tpn.smart0.xyz

Java: list.get(0); list.set(0, 9);
来源：http://quh.ppjwa.cn

Go:   arr[0]; arr[0] = 9
来源：http://uiv.zhiwuduotai.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dnu.iojbl.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kkw.zhoulong.xyz

[D06] 数组长度
来源：http://lgk.yj20258888.top

Py:   len(arr)
来源：http://bpx.52xcode.cn

PHP:  count($arr);
来源：http://sps.xuetiantiany.cn

JS:   arr.length
来源：http://zey.shzxlz.cn

TS:   arr.length
来源：http://ela.316326.xyz

Java: list.size();
来源：http://aaq.zhongyouzk.top

Go:   len(arr)
来源：http://tqi.jlsjyb.cn

Ruby: arr.length; arr.size
来源：http://crv.dashuyun.cn

C#:   list.Count;
来源：http://rhc.fanxiaobao.xyz

[D07] 切片 / 取子数组
来源：http://uzm.fktsv.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zmf.daxiang520.top

PHP:  array_slice($arr, 1, 3);
来源：http://szd.jianghu66.top

JS:   arr.slice(1, 4);
来源：http://wus.0kj1m.cn

TS:   arr.slice(1, 4);
来源：http://pro.jinqigfzy.top

Java: list.subList(1, 4);
来源：http://ybl.mhx1999.top

Go:   arr[1:4]
来源：http://qha.cucudq.cn

Ruby: arr[1, 3]
来源：http://gor.zdqjudy.top

C#:   list.GetRange(1, 3);
来源：http://gxq.daria6918.cn

[D08] 合并两个数组
来源：http://tnb.fengsongda.top

Py:   a + b;  a.extend(b)
来源：http://atx.hnxiangtu.top

PHP:  array_merge($a, $b);
来源：http://zah.shuidangran.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ggk.zhiwuduotai.top

TS:   [...a, ...b];
来源：http://lyh.chenzaomai.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ykl.iojbl.cn

Go:   append(a, b...)
来源：http://cck.daxiang520.top

Ruby: a + b;  a.concat(b)
来源：http://dml.zhijiandao.cn

C#:   a.Concat(b).ToList()
来源：http://rtc.cashguo.top

[D09] 排序（升序）
来源：http://mqb.shanyushiyangtech.top

Py:   sorted(arr);  arr.sort()
来源：http://bln.zhixingplan.top

PHP:  sort($arr);
来源：http://vfm.jyoumei.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nxp.fehbvm.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://fjf.zhaomingkeji.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://btt.zhijiandao.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qxz.aizwys.cn

Ruby: arr.sort
来源：http://hwv.nanxinkj.top

C#:   list.Sort();
来源：http://xul.pycfn.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://yfy.fktsv.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zpn.yuanzhike.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kpl.jiagoushi.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hpn.yj20258888.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ijh.ywan-chungtsiang.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ucv.hesvh.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vzn.shangyingyoupin.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://oci.aibaodan.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rwq.gzhubu.top

[D11] 反转数组
来源：http://iug.zhixingplan.top

Py:   arr[::-1];  arr.reverse()
来源：http://lfg.aizwys.cn

PHP:  array_reverse($arr);
来源：http://dox.yuanzhike.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sgl.9152youxi.cn

TS:   [...arr].reverse();
来源：http://fum.ywan-chungtsiang.top

Java: Collections.reverse(list);
来源：http://euv.yongpay.top

Go:   slices.Reverse(arr)
来源：http://dlg.xuanzx.com

Ruby: arr.reverse
来源：http://vsa.daxiang520.top

C#:   list.Reverse();
来源：http://rqm.xuanzx.com

[D12] 查找元素下标
来源：http://yzg.jinqigufen.top

Py:   arr.index(x);  x in arr
来源：http://stb.yueranfly.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wtj.jinyuanbaomall.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ozj.sufxvd.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xej.sysykeji.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xyl.xinyue.icu

Go:   slices.Index(arr, x)
来源：http://bps.shanyushiyangkeji.top

Ruby: arr.index(x)
来源：http://uio.9152youxi.cn

C#:   list.IndexOf(x);
来源：http://ggl.vehdjk.com

[D13] 过滤（保留满足条件的）
来源：http://aak.fktsv.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://drv.feifeiyinyue.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bpa.havefunace.top

JS:   arr.filter(x => x > 3)
来源：http://nyj.aizwys.cn

TS:   arr.filter(x => x > 3)
来源：http://ogi.chenlongwang.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pel.ivvv.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rbk.hywenlv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ser.xylfe.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://nmm.hammf.cn

[D14] 映射转换（每个元素变形）
来源：http://kgo.shangyingyoupin.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://etb.ppjwa.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hed.zhongyouzk.top

JS:   arr.map(x => x * 2)
来源：http://iws.yj202588.top

TS:   arr.map(x => x * 2)
来源：http://opg.fanxiaobao.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://vsb.sysykeji.top

Go:   // 手写循环
来源：http://wpy.cashguo.top

Ruby: arr.map { |x| x * 2 }
来源：http://dit.yanxiufei.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ruc.andypj.xyz

[D15] 去重
来源：http://peq.redwolf501.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wlh.chenzaomai.com

PHP:  array_unique($arr);
来源：http://pbl.sweek.top

JS:   [...new Set(arr)]
来源：http://jdg.ywan-chungtsiang.top

TS:   [...new Set(arr)]
来源：http://hcw.hywenlv.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yij.zhengqikj.top

Go:   // 用 map[T]struct{} 手写
来源：http://vye.cashguo.top

Ruby: arr.uniq
来源：http://lvu.dashuyun.cn

C#:   list.Distinct().ToList()
来源：http://qre.tianlin.xyz

[D16] 求和与平均值
来源：http://nal.gotoacloud.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qcj.uphjek.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xcq.zdqjudy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xyi.haohaochexian.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mqg.cqqwz.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wti.hcnkem.com

Go:   // 手写循环累加
来源：http://dzg.sxryk.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lfu.zhongyouzk.top

C#:   list.Sum();  list.Average()
来源：http://ddl.guannengcc.top

[D17] 最大值与最小值
来源：http://rpy.wangshuangyany.cn

Py:   max(arr);  min(arr)
来源：http://yer.meibo888.top

PHP:  max($arr);  min($arr);
来源：http://yhm.yfazqb.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gqc.hnqzz.top

TS:   Math.max(...arr);
来源：http://aht.guannengcc.top

Java: Collections.max(list);  Collections.min(list);
来源：http://nav.fengsongda.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jya.hesvh.cn

Ruby: arr.max;  arr.min
来源：http://sxj.shzxlz.cn

C#:   list.Max();  list.Min()
来源：http://uca.sufxvd.cn

[D18] 扁平化嵌套数组
来源：http://vis.jinghuilouyu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qfi.daxiang520.top

PHP:  array_merge(...$nested);
来源：http://ljc.nwbrower.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vfj.xylfe.cn

TS:   nested.flat();
来源：http://zln.sysykeji.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ozn.yangfankeji.com

Go:   // 手写双层循环
来源：http://tus.jinghuilouyu.cn

Ruby: nested.flatten
来源：http://xyx.iojbl.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://svf.nanxuanxn.top


<!-- 参考信息 -->
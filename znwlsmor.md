代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://bzb.fzhhl.top

[C03] 可变参数
来源：http://osm.pycfn.com

Py:   def total(*args): return sum(args)
来源：http://soe.zhaomingkeji.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wwh.uphjek.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pjh.sxryk.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://klh.xinyue.icu

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zix.hfpthk.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jdp.aizwys.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pcy.xinyue.icu

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rqn.redwolf501.top

[C04] 命名参数 / 关键字参数
来源：http://ucs.hesvh.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wvh.havefunace.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fbe.vqdsnc.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wvl.cqqwz.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rqr.shuidangran.top

Java: // 无：用 Builder 模式或 record
来源：http://zyc.havefunace.top

Go:   // 无：用配置结构体参数
来源：http://gjb.xuanzx.com

Ruby: f(a: 1, b: 2)
来源：http://dpx.jqgufenzy.top

C#:   f(a: 1, b: 2)
来源：http://pcd.jinqigfzy.top

[C05] 返回多个值
来源：http://rbf.shuidangran.top

Py:   return a, b
来源：http://liu.ybcxt.top

PHP:  return [$a, $b];
来源：http://fgs.xingfuxueyuan.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://cwj.havefunace.top

TS:   return { a, b };
来源：http://trz.jqgfzy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://aye.wangshuangyany.cn

Go:   return a, b
来源：http://jbb.cashguo.top

Ruby: return a, b
来源：http://vgh.vehdjk.com

C#:   return (a, b);              // ValueTuple
来源：http://bhy.yueranfly.top

[C06] 匿名函数 / lambda
来源：http://adu.zhoulong.xyz

Py:   square = lambda x: x * x
来源：http://joo.jianghu66.top

PHP:  $square = fn($x) => $x * $x;
来源：http://cuw.cashguo.top

JS:   const square = x => x * x;
来源：http://lrv.quarkkingdee.top

TS:   const square = (x: number): number => x * x;
来源：http://wtc.zhixingplan.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://oin.nanxuanxn.top

Go:   sq := func(x int) int { return x * x }
来源：http://tkm.tarul.cn

Ruby: square = ->(x) { x * x }
来源：http://tph.hnqzz.top

C#:   Func<int, int> square = x => x * x;
来源：http://etp.yvedp.cn

[C07] 把函数作为参数传入
来源：http://wdr.sjlbkw.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://suu.hammf.cn

PHP:  array_map("strtoupper", $arr);
来源：http://cbh.hysaishi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wyk.epnwcf.com

TS:   arr.map(String)
来源：http://zlc.yangfankeji.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fid.havefunace.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hny.snrcjt.cn

Ruby: arr.map(&:upcase)
来源：http://elm.aizwys.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://rdw.ctjpmb.com

[C08] 闭包
来源：http://yhh.chenlongwang.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://viq.yonumen.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nbu.zhaomingkeji.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gfm.hongshengwenyu.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://iqq.jqgufenzy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://aaj.fehbvm.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://njo.xuetiantiany.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ott.fehbvm.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kkk.meibo888.top

[C09] 递归
来源：http://aca.hesvh.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pbm.fehbvm.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://krp.hongshengwenyu.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fad.fktsv.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://guh.shanyushiyangtech.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zkv.pengpengdd.cyou

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://oqr.sxryk.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bpk.hesvh.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cgv.daxiang520.top

[C10] 变量作用域
来源：http://pyg.yongpay.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fwe.xinyue.icu

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rgt.hywenlv.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://csq.fzhhl.top

TS:   同 JS
来源：http://wji.yj202588.top

Java: 方法内为块级作用域
来源：http://kme.svipenyu.cn

Go:   花括号块级作用域
来源：http://qsp.jinqigfzy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wnf.jqgfzy.top

C#:   块级作用域
来源：http://ias.jianghu66.top

[C11] 模块导入与导出
来源：http://eus.hywenlv.cn

Py:   from module import func
来源：http://nym.zdqjudy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://qdf.hysaishi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://qot.hysaishi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kur.hammf.cn

Java: import java.util.List;
来源：http://ydp.shangyingyoupin.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wsc.guowangkeji.top

Ruby: require "json"; require_relative "./util"
来源：http://gdz.fehbvm.com

C#:   using System.Text;
来源：http://yeo.cdnleiting.top

[C12] 立即执行函数 IIFE
来源：http://kht.jiagoushi.top

Py:   (lambda: print("run"))()
来源：http://kkv.fehbvm.com

PHP:  (function () { echo "run"; })();
来源：http://med.zhengqikj.top

JS:   (() => { console.log("run"); })();
来源：http://wrg.havefunace.top

TS:   (() => { console.log("run"); })();
来源：http://ubi.wangshuangyany.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lwh.xingfuxueyuan.xyz

Go:   func() { fmt.Println("run") }()
来源：http://ayj.jyoumei.cn

Ruby: -> { puts "run" }.call
来源：http://jqf.jyoumei.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://tdz.316326.xyz

[C13] 类型声明 / 类型注解
来源：http://xpe.zhoulong.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zpm.jqgfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uco.aibaodan.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://omx.hfpthk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oix.shanyushiyangkeji.top

Java: int add(int a, int b) { return a + b; }
来源：http://dxq.shzxlz.cn

Go:   func add(a, b int) int
来源：http://gfx.sysykeji.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://saj.snrcjt.cn

C#:   int Add(int a, int b) => a + b;
来源：http://lrv.hcnkem.com

[C14] 泛型函数
来源：http://wwb.hcnkem.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wos.sxryk.cn

PHP:  // 无泛型
来源：http://knd.sufxvd.cn

JS:   // 无泛型
来源：http://bbq.cdnleiting.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hlz.andypj.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://goo.hfpthk.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zbo.zhaomingkeji.xyz

Ruby: # 无泛型
来源：http://mug.yuanzhike.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://knr.shuidangran.top

[C15] 解构 / 展开参数
来源：http://jlb.jinghuilouyu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://aha.gogol.net.cn

PHP:  [$a, $b] = $pair;
来源：http://xjp.hywenlv.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hij.chenlongwang.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dhw.zhixingplan.top

Java: // 无解构
来源：http://qzw.c1oappe.top

Go:   // 无解构
来源：http://tcz.redwolf501.top

Ruby: a, b = pair
来源：http://esi.fktsv.cn

C#:   var (a, b) = pair;
来源：http://zxk.wangdashe.top

[C16] 函数 / 方法重载
来源：http://xsq.xuetiantiany.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mui.jinghuilouyu.cn

PHP:  // 无重载
来源：http://oor.0kj1m.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ydq.tianlin.xyz

TS:   // 用联合类型或重载签名声明
来源：http://mku.aizwys.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://mtj.zhoulong.xyz

Go:   // 无重载：用不同函数名
来源：http://wgn.zhixingplan.top

Ruby: # 无重载：靠动态参数
来源：http://ine.yanxiufei.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://cfx.0kj1m.cn

================================================================================
来源：http://qyw.ivvv.top

D. 数组 / 列表 / 集合
来源：http://cog.tanke756.top

================================================================================
来源：http://kwr.gzhubu.top

[D01] 创建数组 / 列表
来源：http://eqz.c1oappe.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ikk.shuidangran.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rck.fktsv.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sru.ppjwa.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://izp.hysaishi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lzj.tarul.cn

Go:   arr := []int{1, 2, 3}
来源：http://scx.nanxinkj.top

Ruby: arr = [1, 2, 3]
来源：http://kfh.haohaochexian.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ikc.meibo888.top

[D02] 追加元素到末尾
来源：http://ebc.yfazqb.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://oih.nwbrower.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rny.yanxiufei.cn

JS:   arr.push(4);
来源：http://cmo.shuidangran.top

TS:   arr.push(4);
来源：http://bnt.chenlongwang.top

Java: list.add(4);
来源：http://chk.shangyingyoupin.top

Go:   arr = append(arr, 4)
来源：http://iyf.feifeiyinyue.top

Ruby: arr << 4; arr.push(5)
来源：http://ukv.zycfv.cn

C#:   list.Add(4);
来源：http://arr.daxiang520.top

[D03] 在指定位置插入元素
来源：http://vno.guowangkeji.top

Py:   arr.insert(0, 0)
来源：http://ppm.vqdsnc.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kmn.cucudq.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://snh.chenjidiqi.icu

TS:   arr.splice(0, 0, 0);
来源：http://fzs.shzxlz.cn

Java: list.add(0, 0);
来源：http://kbl.shanyushiyangtech.top

Go:   arr = append([]int{0}, arr...)
来源：http://tyb.yj20258.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nab.yonumen.top

C#:   list.Insert(0, 0);
来源：http://aze.wangshuangyany.cn

[D04] 删除元素
来源：http://ely.bbcook.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jab.ybcxt.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ldf.jianghu66.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gis.hammf.cn

TS:   arr.splice(0, 1);
来源：http://jpx.yvedp.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://soq.wangdashe.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nev.jinqigfzy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wrp.dashuyun.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hbr.birdmap.top

[D05] 访问与修改元素
来源：http://puy.fanxiaobao.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://waq.hongshengwenyu.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fid.ydjk.org.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ija.shanyushiyangkeji.top

TS:   arr[0]; arr.at(-1);
来源：http://jro.mhx1999.top

Java: list.get(0); list.set(0, 9);
来源：http://lcm.xinyue.icu

Go:   arr[0]; arr[0] = 9
来源：http://add.9152youxi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://aml.yfazqb.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://huc.hcnkem.com

[D06] 数组长度
来源：http://hcl.ybcxt.top

Py:   len(arr)
来源：http://ppq.sweek.top

PHP:  count($arr);
来源：http://scc.yj20258888.top

JS:   arr.length
来源：http://lse.hcnkem.com

TS:   arr.length
来源：http://lke.jlsjyb.cn

Java: list.size();
来源：http://gvx.yangfankeji.com

Go:   len(arr)
来源：http://upl.fzhhl.top

Ruby: arr.length; arr.size
来源：http://eus.smart0.xyz

C#:   list.Count;
来源：http://cim.ydzc1.top

[D07] 切片 / 取子数组
来源：http://ctt.yongpay.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fcv.guowangkeji.top

PHP:  array_slice($arr, 1, 3);
来源：http://iqa.jlsjyb.cn

JS:   arr.slice(1, 4);
来源：http://czf.svipenyu.cn

TS:   arr.slice(1, 4);
来源：http://zhr.yueranfly.top

Java: list.subList(1, 4);
来源：http://aez.smart0.xyz

Go:   arr[1:4]
来源：http://snb.jinyuanbaomall.cn

Ruby: arr[1, 3]
来源：http://pks.hnqzz.top

C#:   list.GetRange(1, 3);
来源：http://pru.hongshengwenyu.top

[D08] 合并两个数组
来源：http://erm.xingfuxueyuan.xyz

Py:   a + b;  a.extend(b)
来源：http://cjv.yanxiufei.cn

PHP:  array_merge($a, $b);
来源：http://gue.yuxming.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gce.yueranfly.top

TS:   [...a, ...b];
来源：http://evo.dashuyun.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ngt.xinyue.icu

Go:   append(a, b...)
来源：http://ima.jqgufenzy.top

Ruby: a + b;  a.concat(b)
来源：http://bqq.dashuyun.cn

C#:   a.Concat(b).ToList()
来源：http://xeo.daxiang520.top

[D09] 排序（升序）
来源：http://zos.aizwys.cn

Py:   sorted(arr);  arr.sort()
来源：http://wwe.shzxlz.cn

PHP:  sort($arr);
来源：http://dbz.fktsv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://oje.9152youxi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://kjc.xylfe.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vtg.nanxuanxn.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ekr.jinqigfzy.top

Ruby: arr.sort
来源：http://ufq.shzxlz.cn

C#:   list.Sort();
来源：http://fzf.ywan-chungtsiang.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://utk.52xcode.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ffk.ehwqpu.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jic.pycfn.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xkc.jinyuanbaomall.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mnl.epnwcf.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://thj.yj20258.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fjb.mhx1999.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://olm.nanxinkj.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rto.hysaishi.cn

[D11] 反转数组
来源：http://qxp.tian-w.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wiu.yvedp.cn

PHP:  array_reverse($arr);
来源：http://lrs.zhaomingkeji.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nvf.iojbl.cn

TS:   [...arr].reverse();
来源：http://zre.svipenyu.cn

Java: Collections.reverse(list);
来源：http://thh.hywenlv.cn

Go:   slices.Reverse(arr)
来源：http://bvz.zhijiandao.cn

Ruby: arr.reverse
来源：http://clz.nanxinkj.top

C#:   list.Reverse();
来源：http://dss.hfpthk.cn

[D12] 查找元素下标
来源：http://lin.zhiwuduotai.top

Py:   arr.index(x);  x in arr
来源：http://xgs.zhoulong.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nkl.hnxiangtu.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rov.9152youxi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mzx.ivvv.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://njp.zhoulong.xyz

Go:   slices.Index(arr, x)
来源：http://bmp.ydjk.org.cn

Ruby: arr.index(x)
来源：http://kdn.hesvh.cn

C#:   list.IndexOf(x);
来源：http://ihl.aibaodan.cn

[D13] 过滤（保留满足条件的）
来源：http://jzl.jlsjyb.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hts.dashuyun.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kqt.fengsongda.top

JS:   arr.filter(x => x > 3)
来源：http://qdw.guannengcc.top

TS:   arr.filter(x => x > 3)
来源：http://pbb.ydzc1.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rkw.ivvv.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sar.quarkkingdee.top

Ruby: arr.select { |x| x > 3 }
来源：http://xnq.jinqigufen.top

C#:   list.Where(x => x > 3).ToList()
来源：http://pap.uphjek.com

[D14] 映射转换（每个元素变形）
来源：http://pzd.xinyue.icu

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mxc.yangfankeji.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://job.jianghu66.top

JS:   arr.map(x => x * 2)
来源：http://vtz.ydzc1.top

TS:   arr.map(x => x * 2)
来源：http://txy.zhiwuduotai.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://bax.aibaodan.cn

Go:   // 手写循环
来源：http://erv.gaohongyu789.top

Ruby: arr.map { |x| x * 2 }
来源：http://iqd.xinyue.icu

C#:   list.Select(x => x * 2).ToList()
来源：http://svf.smart0.xyz

[D15] 去重
来源：http://qsw.xuetiantiany.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://oor.cheryme.top

PHP:  array_unique($arr);
来源：http://ecw.jqgfzy.top

JS:   [...new Set(arr)]
来源：http://lja.hammf.cn

TS:   [...new Set(arr)]
来源：http://tuk.daria6918.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://oju.gzhubu.top

Go:   // 用 map[T]struct{} 手写
来源：http://ozs.quarkkingdee.top

Ruby: arr.uniq
来源：http://vms.zhiwuduotai.top

C#:   list.Distinct().ToList()
来源：http://sqy.snrcjt.cn

[D16] 求和与平均值
来源：http://iqq.shanyushiyangtech.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lkz.316326.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gxb.mhx1999.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tfi.cdnleiting.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lem.bjfxy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kth.svipenyu.cn

Go:   // 手写循环累加
来源：http://wso.gotoacloud.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://inp.tian-w.cn

C#:   list.Sum();  list.Average()
来源：http://fip.wangdashe.top

[D17] 最大值与最小值
来源：http://llt.ydjk.org.cn

Py:   max(arr);  min(arr)
来源：http://crz.xingfuxueyuan.xyz

PHP:  max($arr);  min($arr);
来源：http://urc.zhengqikj.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://een.chenjidiqi.icu

TS:   Math.max(...arr);
来源：http://htl.hywenlv.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gau.gaohongyu789.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zuo.iojbl.cn

Ruby: arr.max;  arr.min
来源：http://mas.tianlin.xyz

C#:   list.Max();  list.Min()
来源：http://bpm.jinghuilouyu.cn

[D18] 扁平化嵌套数组
来源：http://epi.hongshengwenyu.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xsj.cdnleiting.top

PHP:  array_merge(...$nested);
来源：http://jih.gzhubu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zbd.sufxvd.cn

TS:   nested.flat();
来源：http://hdg.tanke756.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ooc.hnxiangtu.top

Go:   // 手写双层循环
来源：http://jga.ydzc1.top

Ruby: nested.flatten
来源：http://jpy.zycfv.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://glr.meibo888.top

[D19] 按字段分组
来源：http://shx.aibaodan.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ezg.sxryk.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yff.zhoulong.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lbf.fengsongda.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://uuq.vehdjk.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://inl.birdmap.top

Go:   // 手写 map[string][]T
来源：http://onf.sweek.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://loc.jqgufenzy.top


<!-- 参考信息 -->
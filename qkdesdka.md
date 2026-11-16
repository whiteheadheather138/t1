代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://gsm.yuanzhike.top

Java: // 无默认参数：方法重载或 Optional
来源：http://jqu.aizwys.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wmu.fanxiaobao.xyz

Ruby: def greet(name = "World") = name
来源：http://peb.316326.xyz

C#:   string Greet(string name = "World") => name;
来源：http://sfi.hongshengwenyu.top

[C03] 可变参数
来源：http://yzl.ivvv.top

Py:   def total(*args): return sum(args)
来源：http://yfl.nanxinkj.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vdx.hysaishi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://iez.sysykeji.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gqf.hysaishi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zsx.52xcode.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nfv.yj20258.top

Ruby: def total(*nums); nums.sum; end
来源：http://vgs.nanxuanxn.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zng.cucudq.cn

[C04] 命名参数 / 关键字参数
来源：http://gdf.xziqi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ebq.zhengqikj.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nxd.sysykeji.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nnk.daxiang520.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jyk.shanyushiyangkeji.top

Java: // 无：用 Builder 模式或 record
来源：http://fzj.0kj1m.cn

Go:   // 无：用配置结构体参数
来源：http://pjc.wangshuangyany.cn

Ruby: f(a: 1, b: 2)
来源：http://dzv.yanxiufei.cn

C#:   f(a: 1, b: 2)
来源：http://fbv.zhijiandao.cn

[C05] 返回多个值
来源：http://gbj.sysykeji.top

Py:   return a, b
来源：http://ejq.shuidangran.top

PHP:  return [$a, $b];
来源：http://jjx.daria6918.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xjv.ivvv.top

TS:   return { a, b };
来源：http://ygf.gzhubu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yzu.yj20258888.top

Go:   return a, b
来源：http://bbr.jqgufenzy.top

Ruby: return a, b
来源：http://ncw.mhx1999.top

C#:   return (a, b);              // ValueTuple
来源：http://xgt.zhongyouzk.top

[C06] 匿名函数 / lambda
来源：http://vwf.xingfuxueyuan.xyz

Py:   square = lambda x: x * x
来源：http://cec.haohaochexian.top

PHP:  $square = fn($x) => $x * $x;
来源：http://oxn.jyoumei.cn

JS:   const square = x => x * x;
来源：http://lsn.shzxlz.cn

TS:   const square = (x: number): number => x * x;
来源：http://xbx.mhx1999.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cvt.cheryme.top

Go:   sq := func(x int) int { return x * x }
来源：http://wyo.hywenlv.cn

Ruby: square = ->(x) { x * x }
来源：http://jar.hywenlv.cn

C#:   Func<int, int> square = x => x * x;
来源：http://nyq.xuetiantiany.cn

[C07] 把函数作为参数传入
来源：http://oxn.yuanzhike.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rqq.tianlin.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://zwb.epnwcf.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bbz.yvedp.cn

TS:   arr.map(String)
来源：http://wrl.vqdsnc.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ell.52xcode.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pag.cheryme.top

Ruby: arr.map(&:upcase)
来源：http://fsv.yuanzhike.top

C#:   arr.Select(s => s.ToUpper())
来源：http://uwn.hongshengwenyu.top

[C08] 闭包
来源：http://yfg.yj20258888.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vct.hammf.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rja.ehwqpu.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mbc.guannengcc.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ofy.nwbrower.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://snp.nanxuanxn.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zjj.sxryk.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bhd.jqgufenzy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://oyw.jinqigufen.top

[C09] 递归
来源：http://bhz.zhijiandao.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sxq.yj20258.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nyj.fehbvm.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://krj.jlsjyb.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kbp.zdqjudy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://imk.xingfuxueyuan.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nsu.gogol.net.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bxa.feifeiyinyue.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xac.sweek.top

[C10] 变量作用域
来源：http://toa.shuidangran.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://maw.fengsongda.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://otd.shangyingyoupin.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ecv.aibaodan.cn

TS:   同 JS
来源：http://mbx.redwolf501.top

Java: 方法内为块级作用域
来源：http://gww.birdmap.top

Go:   花括号块级作用域
来源：http://zti.fktsv.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hid.c1oappe.top

C#:   块级作用域
来源：http://iqz.gaohongyu789.top

[C11] 模块导入与导出
来源：http://jcv.ctjpmb.com

Py:   from module import func
来源：http://kjw.chenjidiqi.icu

PHP:  require "file.php";  或 use App\Service;
来源：http://vby.yj20258888.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://gfj.cucudq.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://obg.hesvh.cn

Java: import java.util.List;
来源：http://tkt.yongpay.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://djv.ppjwa.cn

Ruby: require "json"; require_relative "./util"
来源：http://baf.hfpthk.cn

C#:   using System.Text;
来源：http://qyf.fktsv.cn

[C12] 立即执行函数 IIFE
来源：http://vvn.dianchejie.cn

Py:   (lambda: print("run"))()
来源：http://rlo.zhaomingkeji.xyz

PHP:  (function () { echo "run"; })();
来源：http://epj.vehdjk.com

JS:   (() => { console.log("run"); })();
来源：http://nam.jianghu66.top

TS:   (() => { console.log("run"); })();
来源：http://dzl.hysaishi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xky.bbcook.cn

Go:   func() { fmt.Println("run") }()
来源：http://iqz.ctjpmb.com

Ruby: -> { puts "run" }.call
来源：http://pma.zhijiandao.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://bzc.gogol.net.cn

[C13] 类型声明 / 类型注解
来源：http://gcn.mhx1999.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://uux.hnxiangtu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://quc.nwbrower.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://own.sjlbkw.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xqv.fktsv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vse.mhx1999.top

Go:   func add(a, b int) int
来源：http://mvq.nanxinkj.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sef.gzhubu.top

C#:   int Add(int a, int b) => a + b;
来源：http://xgj.cheryme.top

[C14] 泛型函数
来源：http://gmr.jqgufenzy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hkd.sjlbkw.cn

PHP:  // 无泛型
来源：http://pgh.c1oappe.top

JS:   // 无泛型
来源：http://zyi.hcnkem.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://oaf.xuanzx.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xcs.nanxuanxn.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ntb.yonumen.top

Ruby: # 无泛型
来源：http://rxu.jinqigfzy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zbu.hysaishi.cn

[C15] 解构 / 展开参数
来源：http://tgv.yueranfly.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://erf.jlsjyb.cn

PHP:  [$a, $b] = $pair;
来源：http://nxw.zhiwuduotai.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fga.hammf.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wtz.redwolf501.top

Java: // 无解构
来源：http://abn.jlsjyb.cn

Go:   // 无解构
来源：http://vbd.ehwqpu.com

Ruby: a, b = pair
来源：http://ufw.9152youxi.cn

C#:   var (a, b) = pair;
来源：http://ign.xuanzx.com

[C16] 函数 / 方法重载
来源：http://omf.tianlin.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://aeg.uphjek.com

PHP:  // 无重载
来源：http://iaf.aibaodan.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://tbv.tian-w.cn

TS:   // 用联合类型或重载签名声明
来源：http://ulw.ydzc1.top

Java: void f(int a) {}  void f(String a) {}
来源：http://khk.yueranfly.top

Go:   // 无重载：用不同函数名
来源：http://azd.meibo888.top

Ruby: # 无重载：靠动态参数
来源：http://adl.ehwqpu.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://trm.hammf.cn

================================================================================
来源：http://mer.epnwcf.com

D. 数组 / 列表 / 集合
来源：http://uvb.epnwcf.com

================================================================================
来源：http://tew.aibaodan.cn

[D01] 创建数组 / 列表
来源：http://zgs.meibo888.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://zzm.yj20258888.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://swu.zhongyouzk.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vlw.gogol.net.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zzf.0kj1m.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mzd.feifeiyinyue.top

Go:   arr := []int{1, 2, 3}
来源：http://ymr.chenlongwang.top

Ruby: arr = [1, 2, 3]
来源：http://azr.hesvh.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vka.xingfuxueyuan.xyz

[D02] 追加元素到末尾
来源：http://gpj.aibaodan.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qnv.shanyushiyangkeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hmi.vqdsnc.cn

JS:   arr.push(4);
来源：http://gtr.dashuyun.cn

TS:   arr.push(4);
来源：http://trz.vqdsnc.cn

Java: list.add(4);
来源：http://vvq.pengpengdd.cyou

Go:   arr = append(arr, 4)
来源：http://wir.iojbl.cn

Ruby: arr << 4; arr.push(5)
来源：http://bmk.bbcook.cn

C#:   list.Add(4);
来源：http://sis.jiagoushi.top

[D03] 在指定位置插入元素
来源：http://pxp.jiagoushi.top

Py:   arr.insert(0, 0)
来源：http://sjd.aizwys.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://usj.dashuyun.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://afs.jinghuilouyu.cn

TS:   arr.splice(0, 0, 0);
来源：http://ndd.fktsv.cn

Java: list.add(0, 0);
来源：http://eya.birdmap.top

Go:   arr = append([]int{0}, arr...)
来源：http://wod.gotoacloud.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://oau.guowangkeji.top

C#:   list.Insert(0, 0);
来源：http://kkd.zdqjudy.top

[D04] 删除元素
来源：http://wrx.ydjk.org.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ddy.aizwys.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://eqn.316326.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bgs.chenzaomai.com

TS:   arr.splice(0, 1);
来源：http://svw.jyoumei.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nia.jqgfzy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wrz.uphjek.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zho.fktsv.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hui.gotoacloud.top

[D05] 访问与修改元素
来源：http://zrx.ivvv.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mqn.yfazqb.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nww.cucudq.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://swo.ehwqpu.com

TS:   arr[0]; arr.at(-1);
来源：http://sdq.jinghuilouyu.cn

Java: list.get(0); list.set(0, 9);
来源：http://qcg.wangshuangyany.cn

Go:   arr[0]; arr[0] = 9
来源：http://dmp.wangshuangyany.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uyb.xylfe.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hqr.xylfe.cn

[D06] 数组长度
来源：http://mfk.ivvv.top

Py:   len(arr)
来源：http://vac.jlsjyb.cn

PHP:  count($arr);
来源：http://pjf.meibo888.top

JS:   arr.length
来源：http://vfh.tarul.cn

TS:   arr.length
来源：http://unk.jinghuilouyu.cn

Java: list.size();
来源：http://tjr.zdbjq.cn

Go:   len(arr)
来源：http://lrd.tarul.cn

Ruby: arr.length; arr.size
来源：http://gib.gzhubu.top

C#:   list.Count;
来源：http://etg.cdnleiting.top

[D07] 切片 / 取子数组
来源：http://fkc.hammf.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tel.wangshuangyany.cn

PHP:  array_slice($arr, 1, 3);
来源：http://snm.c1oappe.top

JS:   arr.slice(1, 4);
来源：http://dhj.316326.xyz

TS:   arr.slice(1, 4);
来源：http://bsa.zhengqikj.top

Java: list.subList(1, 4);
来源：http://dpn.yongpay.top

Go:   arr[1:4]
来源：http://qlr.dianchejie.cn

Ruby: arr[1, 3]
来源：http://kll.pengpengdd.cyou

C#:   list.GetRange(1, 3);
来源：http://zeb.uphjek.com

[D08] 合并两个数组
来源：http://hxv.cucudq.cn

Py:   a + b;  a.extend(b)
来源：http://gas.jinqigfzy.top

PHP:  array_merge($a, $b);
来源：http://str.epnwcf.com

JS:   [...a, ...b];  a.concat(b);
来源：http://dfe.fengsongda.top

TS:   [...a, ...b];
来源：http://dbs.smart0.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rir.xingfuxueyuan.xyz

Go:   append(a, b...)
来源：http://tfn.ehwqpu.com

Ruby: a + b;  a.concat(b)
来源：http://zyv.sufxvd.cn

C#:   a.Concat(b).ToList()
来源：http://zpd.yvedp.cn

[D09] 排序（升序）
来源：http://bic.yongpay.top

Py:   sorted(arr);  arr.sort()
来源：http://agl.snrcjt.cn

PHP:  sort($arr);
来源：http://uuw.hcnkem.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://obc.cucudq.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://uge.yangfankeji.com

Java: Collections.sort(list);  list.sort(null);
来源：http://itq.jinqigufen.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fna.chenlongwang.top

Ruby: arr.sort
来源：http://usc.vehdjk.com

C#:   list.Sort();
来源：http://pup.andypj.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://nta.bjfxy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zzi.gaohongyu789.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rcq.nanxinkj.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dhy.nwbrower.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ngk.yanxiufei.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://olg.9152youxi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://iya.xingfuxueyuan.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ame.cashguo.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gid.hammf.cn

[D11] 反转数组
来源：http://hdc.jqgfzy.top

Py:   arr[::-1];  arr.reverse()
来源：http://ofu.316326.xyz

PHP:  array_reverse($arr);
来源：http://eie.zycfv.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rnf.aizwys.cn

TS:   [...arr].reverse();
来源：http://wot.dianchejie.cn

Java: Collections.reverse(list);
来源：http://zye.yueranfly.top

Go:   slices.Reverse(arr)
来源：http://fur.jlsjyb.cn

Ruby: arr.reverse
来源：http://cxi.gogol.net.cn

C#:   list.Reverse();
来源：http://eoc.ybcxt.top

[D12] 查找元素下标
来源：http://enk.shuidangran.top

Py:   arr.index(x);  x in arr
来源：http://csr.feifeiyinyue.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hpq.shzxlz.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://alc.gaohongyu789.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wyo.nanxuanxn.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://urj.gogol.net.cn

Go:   slices.Index(arr, x)
来源：http://syx.snrcjt.cn

Ruby: arr.index(x)
来源：http://vtx.xylfe.cn

C#:   list.IndexOf(x);
来源：http://qfx.vqdsnc.cn

[D13] 过滤（保留满足条件的）
来源：http://nkn.uphjek.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hws.yj202588.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cqa.zdqjudy.top

JS:   arr.filter(x => x > 3)
来源：http://nqk.shangyingyoupin.top

TS:   arr.filter(x => x > 3)
来源：http://xpc.kuanghao11.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uwp.feifeiyinyue.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cfr.hcnkem.com

Ruby: arr.select { |x| x > 3 }
来源：http://iax.svipenyu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bhz.dianchejie.cn

[D14] 映射转换（每个元素变形）
来源：http://kcm.shuidangran.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cdm.fktsv.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bmx.jqgufenzy.top

JS:   arr.map(x => x * 2)
来源：http://erk.dianchejie.cn

TS:   arr.map(x => x * 2)
来源：http://jvh.gogol.net.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://bwp.shanyushiyangtech.top

Go:   // 手写循环
来源：http://tks.hywenlv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://prn.quarkkingdee.top

C#:   list.Select(x => x * 2).ToList()
来源：http://wgl.mhx1999.top

[D15] 去重
来源：http://uqc.birdmap.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nun.iojbl.cn

PHP:  array_unique($arr);
来源：http://cgf.guowangkeji.top

JS:   [...new Set(arr)]
来源：http://zuv.chenjidiqi.icu

TS:   [...new Set(arr)]
来源：http://yxm.pengpengdd.cyou

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ghc.cucudq.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hvr.yangfankeji.com

Ruby: arr.uniq
来源：http://dut.xuetiantiany.cn

C#:   list.Distinct().ToList()
来源：http://iak.andypj.xyz

[D16] 求和与平均值
来源：http://fby.cheryme.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://psa.xziqi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xal.wangshuangyany.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://uqb.tarul.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dzk.chenlongwang.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tzi.svipenyu.cn

Go:   // 手写循环累加
来源：http://yoi.meibo888.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://szn.feifeiyinyue.top

C#:   list.Sum();  list.Average()
来源：http://pnb.hfpthk.cn

[D17] 最大值与最小值
来源：http://scr.feifeiyinyue.top

Py:   max(arr);  min(arr)
来源：http://qho.fehbvm.com

PHP:  max($arr);  min($arr);
来源：http://scc.yj20258.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xkv.zhoulong.xyz

TS:   Math.max(...arr);
来源：http://zdp.fehbvm.com

Java: Collections.max(list);  Collections.min(list);
来源：http://imz.zhongyouzk.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wls.c1oappe.top

Ruby: arr.max;  arr.min
来源：http://yvh.jinqigfzy.top

C#:   list.Max();  list.Min()
来源：http://owk.pycfn.com

[D18] 扁平化嵌套数组
来源：http://rol.hongshengwenyu.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jvw.chenjidiqi.icu

PHP:  array_merge(...$nested);
来源：http://ygz.yfazqb.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hxk.sysykeji.top

TS:   nested.flat();
来源：http://tpp.nwbrower.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qhn.vqdsnc.cn

Go:   // 手写双层循环
来源：http://tkb.ywan-chungtsiang.top

Ruby: nested.flatten
来源：http://zil.cqqwz.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://tiy.ydjk.org.cn

[D19] 按字段分组
来源：http://teq.tanke756.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kdr.hcnkem.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jjl.aizwys.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xxz.dashuyun.cn


<!-- 参考信息 -->
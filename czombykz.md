代发 wailian999

Py:   if not data: return
来源：http://wiq.aizwys.cn

PHP:  if (!$data) { return; }
来源：http://jjh.cheryme.top

JS:   if (!data) return;
来源：http://jto.cashguo.top

TS:   if (!data) return;
来源：http://mrd.dashuyun.cn

Java: if (data == null) return;
来源：http://yki.shzxlz.cn

Go:   if data == nil { return }
来源：http://fxb.zhijiandao.cn

Ruby: return if data.nil?
来源：http://ipf.gotoacloud.top

C#:   if (data == null) return;
来源：http://nkp.yongpay.top

================================================================================
来源：http://xoh.uphjek.com

C. 函数与作用域
来源：http://shl.jiagoushi.top

================================================================================
来源：http://gli.bbcook.cn

[C01] 定义函数
来源：http://zts.kuanghao11.cn

Py:   def add(a, b): return a + b
来源：http://ace.xziqi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qnx.chenlongwang.top

JS:   function add(a, b) { return a + b; }
来源：http://aqm.xingfuxueyuan.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dzr.fktsv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://bzw.feifeiyinyue.top

Go:   func add(a, b int) int { return a + b }
来源：http://pbs.gotoacloud.top

Ruby: def add(a, b); a + b; end
来源：http://ckb.cucudq.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://odx.nanxinkj.top

[C02] 默认参数
来源：http://spf.yonumen.top

Py:   def greet(name="World"): return name
来源：http://gsy.zhaomingkeji.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://flf.cqqwz.cn

JS:   function greet(name = "World") { return name; }
来源：http://nsq.shangyingyoupin.top

TS:   function greet(name: string = "World") { return name; }
来源：http://rme.zdqjudy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://mba.yuxming.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gmt.havefunace.top

Ruby: def greet(name = "World") = name
来源：http://bjb.zhiwuduotai.top

C#:   string Greet(string name = "World") => name;
来源：http://rze.pengpengdd.cyou

[C03] 可变参数
来源：http://bei.xuetiantiany.cn

Py:   def total(*args): return sum(args)
来源：http://kkm.hongshengwenyu.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://duw.nanxuanxn.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://aat.sufxvd.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fxx.pengpengdd.cyou

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ilt.tanke756.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fvn.tarul.cn

Ruby: def total(*nums); nums.sum; end
来源：http://cng.xingfuxueyuan.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wci.chenlongwang.top

[C04] 命名参数 / 关键字参数
来源：http://fvu.gogol.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yue.fengsongda.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hwa.316326.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kie.shangyingyoupin.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tqb.yuxming.cn

Java: // 无：用 Builder 模式或 record
来源：http://soe.yonumen.top

Go:   // 无：用配置结构体参数
来源：http://zki.jyoumei.cn

Ruby: f(a: 1, b: 2)
来源：http://aga.zhixingplan.top

C#:   f(a: 1, b: 2)
来源：http://pib.yuxming.cn

[C05] 返回多个值
来源：http://wcb.sjlbkw.cn

Py:   return a, b
来源：http://pvv.jlsjyb.cn

PHP:  return [$a, $b];
来源：http://msv.mhx1999.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://pio.yueranfly.top

TS:   return { a, b };
来源：http://wlk.birdmap.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bum.daxiang520.top

Go:   return a, b
来源：http://wtc.haohaochexian.top

Ruby: return a, b
来源：http://tmi.mhx1999.top

C#:   return (a, b);              // ValueTuple
来源：http://ohv.nanxuanxn.top

[C06] 匿名函数 / lambda
来源：http://iey.havefunace.top

Py:   square = lambda x: x * x
来源：http://ord.epnwcf.com

PHP:  $square = fn($x) => $x * $x;
来源：http://xwh.fzhhl.top

JS:   const square = x => x * x;
来源：http://owq.pengpengdd.cyou

TS:   const square = (x: number): number => x * x;
来源：http://kyw.tanke756.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rlm.yj20258888.top

Go:   sq := func(x int) int { return x * x }
来源：http://lno.jinqigufen.top

Ruby: square = ->(x) { x * x }
来源：http://apg.aibaodan.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hfn.tarul.cn

[C07] 把函数作为参数传入
来源：http://vfp.ivvv.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bey.sysykeji.top

PHP:  array_map("strtoupper", $arr);
来源：http://ddd.jinqigufen.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qyx.xuetiantiany.cn

TS:   arr.map(String)
来源：http://hjw.shuidangran.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tbb.zhengqikj.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tca.zycfv.cn

Ruby: arr.map(&:upcase)
来源：http://djc.yvedp.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://rmm.tanke756.top

[C08] 闭包
来源：http://vhc.snrcjt.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dge.zhengqikj.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bsc.dianchejie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://smd.hysaishi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://trj.sufxvd.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://exj.bjfxy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vev.haohaochexian.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jxh.shuidangran.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://inl.jinghuilouyu.cn

[C09] 递归
来源：http://iym.hcnkem.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://trl.jinyuanbaomall.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://epq.316326.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oie.chenjidiqi.icu

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cpt.yj202588.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://guv.feifeiyinyue.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qfi.tianlin.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lsu.guannengcc.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://eim.yfazqb.com

[C10] 变量作用域
来源：http://cff.hfpthk.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ipu.xuetiantiany.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vcq.yuxming.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ftg.mhx1999.top

TS:   同 JS
来源：http://eyl.52xcode.cn

Java: 方法内为块级作用域
来源：http://bja.andypj.xyz

Go:   花括号块级作用域
来源：http://tni.wangshuangyany.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bbv.uphjek.com

C#:   块级作用域
来源：http://qel.feifeiyinyue.top

[C11] 模块导入与导出
来源：http://xfs.shanyushiyangtech.top

Py:   from module import func
来源：http://oqm.aizwys.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://eee.cdnleiting.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://pca.zdqjudy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jvr.cqqwz.cn

Java: import java.util.List;
来源：http://tgo.jqgufenzy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://czp.xinyue.icu

Ruby: require "json"; require_relative "./util"
来源：http://myk.guannengcc.top

C#:   using System.Text;
来源：http://cwi.shangyingyoupin.top

[C12] 立即执行函数 IIFE
来源：http://mww.hammf.cn

Py:   (lambda: print("run"))()
来源：http://cam.aibaodan.cn

PHP:  (function () { echo "run"; })();
来源：http://wav.yj202588.top

JS:   (() => { console.log("run"); })();
来源：http://nir.hysaishi.cn

TS:   (() => { console.log("run"); })();
来源：http://dgi.tianlin.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://avj.9152youxi.cn

Go:   func() { fmt.Println("run") }()
来源：http://fxa.hfpthk.cn

Ruby: -> { puts "run" }.call
来源：http://amk.hywenlv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://nnj.nanxuanxn.top

[C13] 类型声明 / 类型注解
来源：http://yrl.mhx1999.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://afr.zhaomingkeji.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jsp.andypj.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fuf.cdnleiting.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://osz.zhaomingkeji.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://sfu.zdbjq.cn

Go:   func add(a, b int) int
来源：http://fyc.fehbvm.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://biy.yuanzhike.top

C#:   int Add(int a, int b) => a + b;
来源：http://syi.xylfe.cn

[C14] 泛型函数
来源：http://seo.birdmap.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qvb.gzhubu.top

PHP:  // 无泛型
来源：http://zow.uphjek.com

JS:   // 无泛型
来源：http://bqk.hesvh.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vse.guannengcc.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hmd.yj20258.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lgy.yvedp.cn

Ruby: # 无泛型
来源：http://tla.jiagoushi.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://klo.dashuyun.cn

[C15] 解构 / 展开参数
来源：http://ken.gaohongyu789.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hlh.bbcook.cn

PHP:  [$a, $b] = $pair;
来源：http://cym.cdnleiting.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://sdb.jinqigfzy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zmm.feifeiyinyue.top

Java: // 无解构
来源：http://nnb.xinyue.icu

Go:   // 无解构
来源：http://wcp.yfazqb.com

Ruby: a, b = pair
来源：http://fju.jinqigfzy.top

C#:   var (a, b) = pair;
来源：http://gos.birdmap.top

[C16] 函数 / 方法重载
来源：http://mcp.chenlongwang.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bos.pengpengdd.cyou

PHP:  // 无重载
来源：http://vjz.yangfankeji.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://dgo.cqqwz.cn

TS:   // 用联合类型或重载签名声明
来源：http://osl.jlsjyb.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://cat.jianghu66.top

Go:   // 无重载：用不同函数名
来源：http://sxu.havefunace.top

Ruby: # 无重载：靠动态参数
来源：http://qek.smart0.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://dty.haohaochexian.top

================================================================================
来源：http://zab.hcnkem.com

D. 数组 / 列表 / 集合
来源：http://xip.aizwys.cn

================================================================================
来源：http://vbv.aizwys.cn

[D01] 创建数组 / 列表
来源：http://syj.snrcjt.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://lhq.zhoulong.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ztv.aizwys.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uoq.xuetiantiany.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wgx.cqqwz.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fgc.daria6918.cn

Go:   arr := []int{1, 2, 3}
来源：http://mpq.ctjpmb.com

Ruby: arr = [1, 2, 3]
来源：http://axc.chenjidiqi.icu

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://khc.nanxinkj.top

[D02] 追加元素到末尾
来源：http://chl.andypj.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dqm.feifeiyinyue.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bsf.zhiwuduotai.top

JS:   arr.push(4);
来源：http://hvf.zhongyouzk.top

TS:   arr.push(4);
来源：http://bcc.mhx1999.top

Java: list.add(4);
来源：http://zpb.shanyushiyangkeji.top

Go:   arr = append(arr, 4)
来源：http://fie.c1oappe.top

Ruby: arr << 4; arr.push(5)
来源：http://ree.zhiwuduotai.top

C#:   list.Add(4);
来源：http://fjt.xziqi.cn

[D03] 在指定位置插入元素
来源：http://dhu.guannengcc.top

Py:   arr.insert(0, 0)
来源：http://qfr.cucudq.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tdc.hnxiangtu.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nos.daria6918.cn

TS:   arr.splice(0, 0, 0);
来源：http://ugf.meibo888.top

Java: list.add(0, 0);
来源：http://mnw.ydzc1.top

Go:   arr = append([]int{0}, arr...)
来源：http://wdj.nanxinkj.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pmb.ivvv.top

C#:   list.Insert(0, 0);
来源：http://uaq.svipenyu.cn

[D04] 删除元素
来源：http://nqc.chenlongwang.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wrm.tarul.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://eqy.jqgufenzy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://aqg.yonumen.top

TS:   arr.splice(0, 1);
来源：http://pus.iojbl.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xxv.zhoulong.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nzb.316326.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://izp.c1oappe.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vwg.shangyingyoupin.top

[D05] 访问与修改元素
来源：http://iky.gogol.net.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kld.nanxinkj.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://umj.guannengcc.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qgs.tarul.cn

TS:   arr[0]; arr.at(-1);
来源：http://btg.meibo888.top

Java: list.get(0); list.set(0, 9);
来源：http://hbc.gaohongyu789.top

Go:   arr[0]; arr[0] = 9
来源：http://tpc.yj202588.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ocs.hfpthk.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lya.haohaochexian.top

[D06] 数组长度
来源：http://itm.zhixingplan.top

Py:   len(arr)
来源：http://hyg.gzhubu.top

PHP:  count($arr);
来源：http://uek.yj202588.top

JS:   arr.length
来源：http://dzm.cheryme.top

TS:   arr.length
来源：http://ouo.hammf.cn

Java: list.size();
来源：http://hjg.xylfe.cn

Go:   len(arr)
来源：http://zvb.mhx1999.top

Ruby: arr.length; arr.size
来源：http://jwf.hcnkem.com

C#:   list.Count;
来源：http://kqa.snrcjt.cn

[D07] 切片 / 取子数组
来源：http://eqa.cucudq.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://iwp.sjlbkw.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zpo.xuanzx.com

JS:   arr.slice(1, 4);
来源：http://eku.hnqzz.top

TS:   arr.slice(1, 4);
来源：http://qqa.zhiwuduotai.top

Java: list.subList(1, 4);
来源：http://ecl.epnwcf.com

Go:   arr[1:4]
来源：http://jad.zdqjudy.top

Ruby: arr[1, 3]
来源：http://oib.xziqi.cn

C#:   list.GetRange(1, 3);
来源：http://cwd.xylfe.cn

[D08] 合并两个数组
来源：http://vge.iojbl.cn

Py:   a + b;  a.extend(b)
来源：http://nzc.sjlbkw.cn

PHP:  array_merge($a, $b);
来源：http://mdy.hongshengwenyu.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ljd.yongpay.top

TS:   [...a, ...b];
来源：http://phi.andypj.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xgq.jianghu66.top

Go:   append(a, b...)
来源：http://icb.zdbjq.cn

Ruby: a + b;  a.concat(b)
来源：http://zpv.yj202588.top

C#:   a.Concat(b).ToList()
来源：http://pej.cucudq.cn

[D09] 排序（升序）
来源：http://jmg.daxiang520.top

Py:   sorted(arr);  arr.sort()
来源：http://zus.chenzaomai.com

PHP:  sort($arr);
来源：http://toa.jinyuanbaomall.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vez.ppjwa.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gvt.daxiang520.top

Java: Collections.sort(list);  list.sort(null);
来源：http://zxh.iojbl.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vbj.zhengqikj.top

Ruby: arr.sort
来源：http://gir.redwolf501.top

C#:   list.Sort();
来源：http://rah.cucudq.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://szu.fehbvm.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://goy.xinyue.icu

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://scc.xziqi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gni.jianghu66.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://equ.meibo888.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bnr.sxryk.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vil.yvedp.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ghd.cucudq.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tek.jinghuilouyu.cn

[D11] 反转数组
来源：http://ddx.svipenyu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://sct.guowangkeji.top

PHP:  array_reverse($arr);
来源：http://fkx.hfpthk.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mpj.tarul.cn

TS:   [...arr].reverse();
来源：http://ohp.tianlin.xyz

Java: Collections.reverse(list);
来源：http://lkb.ppjwa.cn

Go:   slices.Reverse(arr)
来源：http://atl.hcnkem.com

Ruby: arr.reverse
来源：http://stq.vqdsnc.cn

C#:   list.Reverse();
来源：http://snp.yuxming.cn

[D12] 查找元素下标
来源：http://eco.redwolf501.top

Py:   arr.index(x);  x in arr
来源：http://imq.sysykeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qto.ivvv.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gys.meibo888.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dqn.jyoumei.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tof.hcnkem.com

Go:   slices.Index(arr, x)
来源：http://zjo.zhiwuduotai.top

Ruby: arr.index(x)
来源：http://khp.shuidangran.top

C#:   list.IndexOf(x);
来源：http://mis.xinyue.icu

[D13] 过滤（保留满足条件的）
来源：http://sgy.chenlongwang.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wxx.shuidangran.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bid.xinyue.icu

JS:   arr.filter(x => x > 3)
来源：http://arb.yuxming.cn

TS:   arr.filter(x => x > 3)
来源：http://pci.jyoumei.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://evt.jiagoushi.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wqi.meibo888.top

Ruby: arr.select { |x| x > 3 }
来源：http://hkf.tian-w.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://avp.yj202588.top

[D14] 映射转换（每个元素变形）
来源：http://yok.xinyue.icu

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://olv.sxryk.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zma.gogol.net.cn

JS:   arr.map(x => x * 2)
来源：http://uhu.hnqzz.top

TS:   arr.map(x => x * 2)
来源：http://hjx.chenlongwang.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://rve.shzxlz.cn

Go:   // 手写循环
来源：http://yiq.0kj1m.cn

Ruby: arr.map { |x| x * 2 }
来源：http://tly.ydjk.org.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hiu.hongshengwenyu.top

[D15] 去重
来源：http://uas.hongshengwenyu.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mty.fengsongda.top

PHP:  array_unique($arr);
来源：http://efs.sjlbkw.cn

JS:   [...new Set(arr)]
来源：http://oso.yonumen.top

TS:   [...new Set(arr)]
来源：http://ida.fktsv.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://abs.smart0.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://vvl.vqdsnc.cn

Ruby: arr.uniq
来源：http://gva.jinghuilouyu.cn

C#:   list.Distinct().ToList()
来源：http://ouz.zhijiandao.cn

[D16] 求和与平均值
来源：http://plm.svipenyu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xwc.hcnkem.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xdd.9152youxi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rqa.yongpay.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wdc.snrcjt.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://msh.jinghuilouyu.cn

Go:   // 手写循环累加
来源：http://jas.zhoulong.xyz


<!-- 参考信息 -->
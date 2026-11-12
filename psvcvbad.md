代发 wailian999

================================================================================
来源：http://orp.smart0.xyz

C. 函数与作用域
来源：http://pwp.sjlbkw.cn

================================================================================
来源：http://rui.cashguo.top

[C01] 定义函数
来源：http://yxb.dashuyun.cn

Py:   def add(a, b): return a + b
来源：http://mwv.ctjpmb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jui.zdbjq.cn

JS:   function add(a, b) { return a + b; }
来源：http://ueu.hesvh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fle.zhijiandao.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xxi.bbcook.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ywp.bjfxy.top

Ruby: def add(a, b); a + b; end
来源：http://hrs.hesvh.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ywz.xuetiantiany.cn

[C02] 默认参数
来源：http://tcc.wangdashe.top

Py:   def greet(name="World"): return name
来源：http://gyh.dianchejie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://orc.cqqwz.cn

JS:   function greet(name = "World") { return name; }
来源：http://lck.shzxlz.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://aky.haohaochexian.top

Java: // 无默认参数：方法重载或 Optional
来源：http://rqg.xingfuxueyuan.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hgy.haohaochexian.top

Ruby: def greet(name = "World") = name
来源：http://fph.sufxvd.cn

C#:   string Greet(string name = "World") => name;
来源：http://wfj.gaohongyu789.top

[C03] 可变参数
来源：http://twr.zdqjudy.top

Py:   def total(*args): return sum(args)
来源：http://ifi.dianchejie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vop.hnqzz.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xpa.zhaomingkeji.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sdd.hysaishi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ljt.pycfn.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lal.cashguo.top

Ruby: def total(*nums); nums.sum; end
来源：http://ybd.andypj.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qdl.cdnleiting.top

[C04] 命名参数 / 关键字参数
来源：http://kmf.zycfv.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qhe.quarkkingdee.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hmu.jiagoushi.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dnr.xingfuxueyuan.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xlp.yanxiufei.cn

Java: // 无：用 Builder 模式或 record
来源：http://idz.yueranfly.top

Go:   // 无：用配置结构体参数
来源：http://cib.shanyushiyangtech.top

Ruby: f(a: 1, b: 2)
来源：http://zwy.316326.xyz

C#:   f(a: 1, b: 2)
来源：http://lfg.bbcook.cn

[C05] 返回多个值
来源：http://gdu.fanxiaobao.xyz

Py:   return a, b
来源：http://cmo.zhengqikj.top

PHP:  return [$a, $b];
来源：http://zyq.redwolf501.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://syd.jinyuanbaomall.cn

TS:   return { a, b };
来源：http://htn.aibaodan.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gne.hongshengwenyu.top

Go:   return a, b
来源：http://lqw.gaohongyu789.top

Ruby: return a, b
来源：http://gcs.tian-w.cn

C#:   return (a, b);              // ValueTuple
来源：http://sci.shzxlz.cn

[C06] 匿名函数 / lambda
来源：http://bho.andypj.xyz

Py:   square = lambda x: x * x
来源：http://miy.haohaochexian.top

PHP:  $square = fn($x) => $x * $x;
来源：http://aag.hammf.cn

JS:   const square = x => x * x;
来源：http://vpk.haohaochexian.top

TS:   const square = (x: number): number => x * x;
来源：http://bca.daria6918.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mxx.zhongyouzk.top

Go:   sq := func(x int) int { return x * x }
来源：http://oaw.svipenyu.cn

Ruby: square = ->(x) { x * x }
来源：http://zhw.yuxming.cn

C#:   Func<int, int> square = x => x * x;
来源：http://dgi.ydzc1.top

[C07] 把函数作为参数传入
来源：http://kzv.guowangkeji.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gmt.nanxuanxn.top

PHP:  array_map("strtoupper", $arr);
来源：http://wec.zhoulong.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rae.yuxming.cn

TS:   arr.map(String)
来源：http://dyj.vqdsnc.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lsa.xuetiantiany.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jtu.yj202588.top

Ruby: arr.map(&:upcase)
来源：http://toq.nwbrower.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ulq.shanyushiyangtech.top

[C08] 闭包
来源：http://byy.jqgufenzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uzb.0kj1m.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tks.vehdjk.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://poh.wangshuangyany.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rtp.ivvv.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ycx.guowangkeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qoo.jinqigufen.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ocj.haohaochexian.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ubv.tarul.cn

[C09] 递归
来源：http://xww.tianlin.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ryv.vqdsnc.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jss.xingfuxueyuan.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kyp.hcnkem.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ebw.sxryk.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mon.nwbrower.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wef.iojbl.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://sjd.jqgfzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vym.zhongyouzk.top

[C10] 变量作用域
来源：http://uym.cucudq.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qer.xinyue.icu

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ved.cashguo.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cri.xylfe.cn

TS:   同 JS
来源：http://cei.jinghuilouyu.cn

Java: 方法内为块级作用域
来源：http://mlb.yj20258888.top

Go:   花括号块级作用域
来源：http://cnc.nwbrower.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qci.chenjidiqi.icu

C#:   块级作用域
来源：http://bno.gzhubu.top

[C11] 模块导入与导出
来源：http://bjr.jiagoushi.top

Py:   from module import func
来源：http://edh.jinqigufen.top

PHP:  require "file.php";  或 use App\Service;
来源：http://lwe.vehdjk.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://tyy.dashuyun.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://atu.316326.xyz

Java: import java.util.List;
来源：http://buq.bjfxy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kle.tarul.cn

Ruby: require "json"; require_relative "./util"
来源：http://kfs.ydzc1.top

C#:   using System.Text;
来源：http://wxt.redwolf501.top

[C12] 立即执行函数 IIFE
来源：http://kue.yj20258888.top

Py:   (lambda: print("run"))()
来源：http://jfd.chenjidiqi.icu

PHP:  (function () { echo "run"; })();
来源：http://vef.jiagoushi.top

JS:   (() => { console.log("run"); })();
来源：http://nhv.9152youxi.cn

TS:   (() => { console.log("run"); })();
来源：http://ubs.yj202588.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ljv.guowangkeji.top

Go:   func() { fmt.Println("run") }()
来源：http://ekk.fzhhl.top

Ruby: -> { puts "run" }.call
来源：http://zos.gogol.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://uzq.hfpthk.cn

[C13] 类型声明 / 类型注解
来源：http://xff.c1oappe.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kar.kuanghao11.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fnf.snrcjt.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gpd.birdmap.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bbg.xinyue.icu

Java: int add(int a, int b) { return a + b; }
来源：http://kjp.iojbl.cn

Go:   func add(a, b int) int
来源：http://dyw.birdmap.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.hnxiangtu.top

C#:   int Add(int a, int b) => a + b;
来源：http://rpq.zhongyouzk.top

[C14] 泛型函数
来源：http://frf.cdnleiting.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xsh.sysykeji.top

PHP:  // 无泛型
来源：http://nfx.feifeiyinyue.top

JS:   // 无泛型
来源：http://okd.shzxlz.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kxd.epnwcf.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://slk.meibo888.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://krk.andypj.xyz

Ruby: # 无泛型
来源：http://wkx.yonumen.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yez.jlsjyb.cn

[C15] 解构 / 展开参数
来源：http://qpc.chenlongwang.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jze.fktsv.cn

PHP:  [$a, $b] = $pair;
来源：http://mbk.haohaochexian.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yjg.wangshuangyany.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xcr.aizwys.cn

Java: // 无解构
来源：http://gbs.jyoumei.cn

Go:   // 无解构
来源：http://ehi.aibaodan.cn

Ruby: a, b = pair
来源：http://xvb.jinyuanbaomall.cn

C#:   var (a, b) = pair;
来源：http://szv.zhaomingkeji.xyz

[C16] 函数 / 方法重载
来源：http://mmw.316326.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fjx.ivvv.top

PHP:  // 无重载
来源：http://yff.ctjpmb.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://cms.bjfxy.top

TS:   // 用联合类型或重载签名声明
来源：http://xyg.wangshuangyany.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hzg.nanxuanxn.top

Go:   // 无重载：用不同函数名
来源：http://zyz.redwolf501.top

Ruby: # 无重载：靠动态参数
来源：http://mxb.sufxvd.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://iff.iojbl.cn

================================================================================
来源：http://rst.yanxiufei.cn

D. 数组 / 列表 / 集合
来源：http://fxw.hammf.cn

================================================================================
来源：http://uxf.hesvh.cn

[D01] 创建数组 / 列表
来源：http://rof.ywan-chungtsiang.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://xpc.jyoumei.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://huh.zhengqikj.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://szc.zycfv.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://tnc.cdnleiting.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nma.sxryk.cn

Go:   arr := []int{1, 2, 3}
来源：http://lox.gaohongyu789.top

Ruby: arr = [1, 2, 3]
来源：http://may.zdbjq.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xrt.yonumen.top

[D02] 追加元素到末尾
来源：http://ikd.jyoumei.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dcx.yvedp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oub.bbcook.cn

JS:   arr.push(4);
来源：http://tee.zdqjudy.top

TS:   arr.push(4);
来源：http://kiy.wangdashe.top

Java: list.add(4);
来源：http://beg.tanke756.top

Go:   arr = append(arr, 4)
来源：http://bmm.dianchejie.cn

Ruby: arr << 4; arr.push(5)
来源：http://scd.xuetiantiany.cn

C#:   list.Add(4);
来源：http://crl.meibo888.top

[D03] 在指定位置插入元素
来源：http://mae.cucudq.cn

Py:   arr.insert(0, 0)
来源：http://jzp.chenzaomai.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://aph.0kj1m.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xvi.havefunace.top

TS:   arr.splice(0, 0, 0);
来源：http://acq.hnqzz.top

Java: list.add(0, 0);
来源：http://ufj.yvedp.cn

Go:   arr = append([]int{0}, arr...)
来源：http://stn.havefunace.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qti.xingfuxueyuan.xyz

C#:   list.Insert(0, 0);
来源：http://jxx.jinghuilouyu.cn

[D04] 删除元素
来源：http://ylk.pycfn.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://oba.yanxiufei.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fgp.cdnleiting.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dyq.cqqwz.cn

TS:   arr.splice(0, 1);
来源：http://zxr.shanyushiyangkeji.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xrp.sysykeji.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fsf.hammf.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hdw.daxiang520.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ehx.tian-w.cn

[D05] 访问与修改元素
来源：http://gqc.shanyushiyangkeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://swp.bbcook.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rxk.ywan-chungtsiang.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mmq.xingfuxueyuan.xyz

TS:   arr[0]; arr.at(-1);
来源：http://meu.chenlongwang.top

Java: list.get(0); list.set(0, 9);
来源：http://mdv.zhiwuduotai.top

Go:   arr[0]; arr[0] = 9
来源：http://myb.fktsv.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vcs.daria6918.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rqm.jqgfzy.top

[D06] 数组长度
来源：http://mcu.chenjidiqi.icu

Py:   len(arr)
来源：http://nah.cqqwz.cn

PHP:  count($arr);
来源：http://ytj.fanxiaobao.xyz

JS:   arr.length
来源：http://nnt.gaohongyu789.top

TS:   arr.length
来源：http://fdx.52xcode.cn

Java: list.size();
来源：http://bfn.jinqigufen.top

Go:   len(arr)
来源：http://zrn.mhx1999.top

Ruby: arr.length; arr.size
来源：http://ocn.c1oappe.top

C#:   list.Count;
来源：http://yba.jlsjyb.cn

[D07] 切片 / 取子数组
来源：http://pwk.andypj.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://epv.zhengqikj.top

PHP:  array_slice($arr, 1, 3);
来源：http://pbo.316326.xyz

JS:   arr.slice(1, 4);
来源：http://cys.guannengcc.top

TS:   arr.slice(1, 4);
来源：http://tfk.guannengcc.top

Java: list.subList(1, 4);
来源：http://hem.jqgfzy.top

Go:   arr[1:4]
来源：http://uev.ivvv.top

Ruby: arr[1, 3]
来源：http://gsr.xuetiantiany.cn

C#:   list.GetRange(1, 3);
来源：http://oxl.svipenyu.cn

[D08] 合并两个数组
来源：http://ipx.aizwys.cn

Py:   a + b;  a.extend(b)
来源：http://bsn.zhongyouzk.top

PHP:  array_merge($a, $b);
来源：http://tho.ywan-chungtsiang.top

JS:   [...a, ...b];  a.concat(b);
来源：http://wpy.jqgfzy.top

TS:   [...a, ...b];
来源：http://hcv.yangfankeji.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qjh.aizwys.cn

Go:   append(a, b...)
来源：http://mrz.316326.xyz

Ruby: a + b;  a.concat(b)
来源：http://nej.yonumen.top

C#:   a.Concat(b).ToList()
来源：http://fwi.jlsjyb.cn

[D09] 排序（升序）
来源：http://epn.zhiwuduotai.top

Py:   sorted(arr);  arr.sort()
来源：http://bdb.ydjk.org.cn

PHP:  sort($arr);
来源：http://zxg.pycfn.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pic.fehbvm.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://hqe.haohaochexian.top

Java: Collections.sort(list);  list.sort(null);
来源：http://eaw.jinyuanbaomall.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://eky.nanxuanxn.top

Ruby: arr.sort
来源：http://yxz.hammf.cn

C#:   list.Sort();
来源：http://tfy.cdnleiting.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://hpt.wangshuangyany.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uvu.ivvv.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ozm.yanxiufei.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://stq.chenzaomai.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jnh.sweek.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hkn.316326.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://isg.tian-w.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ann.sxryk.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ycr.jinqigufen.top

[D11] 反转数组
来源：http://giz.yonumen.top

Py:   arr[::-1];  arr.reverse()
来源：http://xrl.shzxlz.cn

PHP:  array_reverse($arr);
来源：http://jmo.xingfuxueyuan.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qqh.hnqzz.top

TS:   [...arr].reverse();
来源：http://zjh.meibo888.top

Java: Collections.reverse(list);
来源：http://bdt.zhoulong.xyz

Go:   slices.Reverse(arr)
来源：http://ycq.aizwys.cn

Ruby: arr.reverse
来源：http://cin.dianchejie.cn

C#:   list.Reverse();
来源：http://gvz.ybcxt.top

[D12] 查找元素下标
来源：http://sbp.vqdsnc.cn

Py:   arr.index(x);  x in arr
来源：http://scd.shzxlz.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rbz.ehwqpu.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rpb.chenjidiqi.icu

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mcz.mhx1999.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://scq.svipenyu.cn

Go:   slices.Index(arr, x)
来源：http://mgq.c1oappe.top

Ruby: arr.index(x)
来源：http://ers.dianchejie.cn

C#:   list.IndexOf(x);
来源：http://lki.dianchejie.cn

[D13] 过滤（保留满足条件的）
来源：http://uwr.guannengcc.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mvm.ybcxt.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mbl.zhaomingkeji.xyz

JS:   arr.filter(x => x > 3)
来源：http://xpn.zhiwuduotai.top

TS:   arr.filter(x => x > 3)
来源：http://lbl.cashguo.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ghb.ydjk.org.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tup.ctjpmb.com

Ruby: arr.select { |x| x > 3 }
来源：http://jth.gaohongyu789.top

C#:   list.Where(x => x > 3).ToList()
来源：http://xcf.xylfe.cn

[D14] 映射转换（每个元素变形）
来源：http://mpl.snrcjt.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gmt.gogol.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fgw.xziqi.cn

JS:   arr.map(x => x * 2)
来源：http://dqh.jinqigufen.top

TS:   arr.map(x => x * 2)
来源：http://rjf.yj202588.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://chq.gaohongyu789.top

Go:   // 手写循环
来源：http://mnt.shanyushiyangtech.top

Ruby: arr.map { |x| x * 2 }
来源：http://qfw.ctjpmb.com

C#:   list.Select(x => x * 2).ToList()
来源：http://gry.quarkkingdee.top

[D15] 去重
来源：http://ibb.xylfe.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ynj.jlsjyb.cn

PHP:  array_unique($arr);
来源：http://lnl.jqgufenzy.top

JS:   [...new Set(arr)]
来源：http://xpb.xziqi.cn

TS:   [...new Set(arr)]
来源：http://udn.jinqigufen.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bgi.smart0.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://wvd.sxryk.cn

Ruby: arr.uniq
来源：http://aej.aibaodan.cn

C#:   list.Distinct().ToList()
来源：http://nqf.yuanzhike.top

[D16] 求和与平均值
来源：http://xyg.vehdjk.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ztt.snrcjt.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hio.yuxming.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vzi.pycfn.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://njw.feifeiyinyue.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://iym.havefunace.top

Go:   // 手写循环累加
来源：http://ovf.wangshuangyany.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fjh.ivvv.top

C#:   list.Sum();  list.Average()
来源：http://ybd.jianghu66.top

[D17] 最大值与最小值
来源：http://ikc.tianlin.xyz

Py:   max(arr);  min(arr)
来源：http://bor.fengsongda.top

PHP:  max($arr);  min($arr);
来源：http://aan.yonumen.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dlm.quarkkingdee.top

TS:   Math.max(...arr);
来源：http://dle.gotoacloud.top

Java: Collections.max(list);  Collections.min(list);
来源：http://tuz.zdqjudy.top


<!-- 参考信息 -->
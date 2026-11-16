代发 wailian999

PHP:  $a && $b || !$c
来源：http://oag.jyoumei.cn

JS:   a && b || !c
来源：http://pwh.guowangkeji.top

TS:   a && b || !c
来源：http://qch.aibaodan.cn

Java: a && b || !c
来源：http://ety.xuetiantiany.cn

Go:   a && b || !c
来源：http://wuh.dianchejie.cn

Ruby: a && b || !c
来源：http://yyj.meibo888.top

C#:   a && b || !c
来源：http://wop.c1oappe.top

[B16] 卫语句：不满足条件提前返回
来源：http://nfk.nanxinkj.top

Py:   if not data: return
来源：http://rit.hammf.cn

PHP:  if (!$data) { return; }
来源：http://akk.hysaishi.cn

JS:   if (!data) return;
来源：http://xnu.haohaochexian.top

TS:   if (!data) return;
来源：http://rlm.nanxuanxn.top

Java: if (data == null) return;
来源：http://cut.fehbvm.com

Go:   if data == nil { return }
来源：http://hhy.ehwqpu.com

Ruby: return if data.nil?
来源：http://qzm.iojbl.cn

C#:   if (data == null) return;
来源：http://sec.nwbrower.top

================================================================================
来源：http://dxy.yanxiufei.cn

C. 函数与作用域
来源：http://cgh.jlsjyb.cn

================================================================================
来源：http://jhm.cheryme.top

[C01] 定义函数
来源：http://uqx.fehbvm.com

Py:   def add(a, b): return a + b
来源：http://pjz.yj20258888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fbe.fktsv.cn

JS:   function add(a, b) { return a + b; }
来源：http://vwu.tianlin.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nrq.ydzc1.top

Java: static int add(int a, int b) { return a + b; }
来源：http://jdo.fengsongda.top

Go:   func add(a, b int) int { return a + b }
来源：http://prv.ywan-chungtsiang.top

Ruby: def add(a, b); a + b; end
来源：http://rxx.kuanghao11.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zlh.fzhhl.top

[C02] 默认参数
来源：http://dmx.cheryme.top

Py:   def greet(name="World"): return name
来源：http://izp.fehbvm.com

PHP:  function greet($name = "World") { return $name; }
来源：http://pdl.9152youxi.cn

JS:   function greet(name = "World") { return name; }
来源：http://jhd.shanyushiyangkeji.top

TS:   function greet(name: string = "World") { return name; }
来源：http://oue.jinqigfzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://lst.jlsjyb.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ahj.hysaishi.cn

Ruby: def greet(name = "World") = name
来源：http://ddz.gzhubu.top

C#:   string Greet(string name = "World") => name;
来源：http://gln.9152youxi.cn

[C03] 可变参数
来源：http://yrg.ywan-chungtsiang.top

Py:   def total(*args): return sum(args)
来源：http://eoq.xuetiantiany.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://whc.gaohongyu789.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lqy.jyoumei.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://iau.zhengqikj.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ahf.mhx1999.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lkv.birdmap.top

Ruby: def total(*nums); nums.sum; end
来源：http://epn.vqdsnc.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://opw.meibo888.top

[C04] 命名参数 / 关键字参数
来源：http://thm.sufxvd.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vug.quarkkingdee.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ldp.yongpay.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://spi.316326.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cbk.ivvv.top

Java: // 无：用 Builder 模式或 record
来源：http://bwb.gogol.net.cn

Go:   // 无：用配置结构体参数
来源：http://gjb.gotoacloud.top

Ruby: f(a: 1, b: 2)
来源：http://gvx.sjlbkw.cn

C#:   f(a: 1, b: 2)
来源：http://fxx.zhijiandao.cn

[C05] 返回多个值
来源：http://sse.fanxiaobao.xyz

Py:   return a, b
来源：http://jmy.sweek.top

PHP:  return [$a, $b];
来源：http://xcc.vehdjk.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://wuz.cashguo.top

TS:   return { a, b };
来源：http://nql.shuidangran.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tvb.fanxiaobao.xyz

Go:   return a, b
来源：http://vsr.hnqzz.top

Ruby: return a, b
来源：http://kho.tarul.cn

C#:   return (a, b);              // ValueTuple
来源：http://dls.xinyue.icu

[C06] 匿名函数 / lambda
来源：http://hdu.sjlbkw.cn

Py:   square = lambda x: x * x
来源：http://lxr.hammf.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://nid.zdqjudy.top

JS:   const square = x => x * x;
来源：http://wcs.fengsongda.top

TS:   const square = (x: number): number => x * x;
来源：http://jyc.hesvh.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sue.shzxlz.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rtp.hysaishi.cn

Ruby: square = ->(x) { x * x }
来源：http://myz.dashuyun.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xbl.daxiang520.top

[C07] 把函数作为参数传入
来源：http://xfo.52xcode.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ifl.yueranfly.top

PHP:  array_map("strtoupper", $arr);
来源：http://dqm.cheryme.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://eqc.jianghu66.top

TS:   arr.map(String)
来源：http://ftl.hcnkem.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qqz.yuxming.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vgw.yvedp.cn

Ruby: arr.map(&:upcase)
来源：http://xjy.fehbvm.com

C#:   arr.Select(s => s.ToUpper())
来源：http://lun.hcnkem.com

[C08] 闭包
来源：http://jwo.xinyue.icu

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kgz.guannengcc.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pql.shanyushiyangtech.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baa.xinyue.icu

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://htu.hfpthk.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ezw.jianghu66.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bpk.cashguo.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mna.gogol.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wkf.shangyingyoupin.top

[C09] 递归
来源：http://hcp.zdqjudy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zmx.ivvv.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xvu.sysykeji.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ody.zhixingplan.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wbp.quarkkingdee.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lzk.andypj.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cod.xziqi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bzb.jianghu66.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rqb.9152youxi.cn

[C10] 变量作用域
来源：http://kze.sjlbkw.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fyj.shuidangran.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bis.meibo888.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kfc.nanxinkj.top

TS:   同 JS
来源：http://lmj.feifeiyinyue.top

Java: 方法内为块级作用域
来源：http://smz.hcnkem.com

Go:   花括号块级作用域
来源：http://ohe.jlsjyb.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jfe.haohaochexian.top

C#:   块级作用域
来源：http://vlu.sxryk.cn

[C11] 模块导入与导出
来源：http://fgn.bjfxy.top

Py:   from module import func
来源：http://szx.bjfxy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://bjg.smart0.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://oaj.chenzaomai.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qlg.jinqigufen.top

Java: import java.util.List;
来源：http://vei.meibo888.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yqx.meibo888.top

Ruby: require "json"; require_relative "./util"
来源：http://rqy.jlsjyb.cn

C#:   using System.Text;
来源：http://rir.svipenyu.cn

[C12] 立即执行函数 IIFE
来源：http://gut.gzhubu.top

Py:   (lambda: print("run"))()
来源：http://bgx.nanxinkj.top

PHP:  (function () { echo "run"; })();
来源：http://nwp.hcnkem.com

JS:   (() => { console.log("run"); })();
来源：http://fmy.yueranfly.top

TS:   (() => { console.log("run"); })();
来源：http://wpk.zhiwuduotai.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ntc.yuxming.cn

Go:   func() { fmt.Println("run") }()
来源：http://zcl.shuidangran.top

Ruby: -> { puts "run" }.call
来源：http://kyg.gzhubu.top

C#:   // 无 IIFE：用静态构造函数
来源：http://twe.shanyushiyangtech.top

[C13] 类型声明 / 类型注解
来源：http://urn.ybcxt.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hji.jinqigfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nqx.chenlongwang.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://toz.xuetiantiany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rex.ybcxt.top

Java: int add(int a, int b) { return a + b; }
来源：http://bba.chenzaomai.com

Go:   func add(a, b int) int
来源：http://lad.nanxuanxn.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://efl.cheryme.top

C#:   int Add(int a, int b) => a + b;
来源：http://lhe.meibo888.top

[C14] 泛型函数
来源：http://ezt.snrcjt.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pxl.daxiang520.top

PHP:  // 无泛型
来源：http://lli.shzxlz.cn

JS:   // 无泛型
来源：http://edv.sysykeji.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xgk.jlsjyb.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vwn.xingfuxueyuan.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xwj.chenjidiqi.icu

Ruby: # 无泛型
来源：http://yiq.sjlbkw.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ssk.zhoulong.xyz

[C15] 解构 / 展开参数
来源：http://ddl.pycfn.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hrh.epnwcf.com

PHP:  [$a, $b] = $pair;
来源：http://akb.dashuyun.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ukq.cheryme.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ugh.zhaomingkeji.xyz

Java: // 无解构
来源：http://quc.iojbl.cn

Go:   // 无解构
来源：http://ykz.xinyue.icu

Ruby: a, b = pair
来源：http://xpj.dianchejie.cn

C#:   var (a, b) = pair;
来源：http://hvq.zhoulong.xyz

[C16] 函数 / 方法重载
来源：http://smv.hcnkem.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bzz.feifeiyinyue.top

PHP:  // 无重载
来源：http://iwz.xingfuxueyuan.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://ndy.9152youxi.cn

TS:   // 用联合类型或重载签名声明
来源：http://evc.feifeiyinyue.top

Java: void f(int a) {}  void f(String a) {}
来源：http://brf.ppjwa.cn

Go:   // 无重载：用不同函数名
来源：http://bfd.zhijiandao.cn

Ruby: # 无重载：靠动态参数
来源：http://fhx.ydjk.org.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://cku.jinghuilouyu.cn

================================================================================
来源：http://xfl.havefunace.top

D. 数组 / 列表 / 集合
来源：http://ggw.guowangkeji.top

================================================================================
来源：http://lfn.jinyuanbaomall.cn

[D01] 创建数组 / 列表
来源：http://vvx.hongshengwenyu.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://bnn.guowangkeji.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kbs.xuanzx.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hye.havefunace.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://snx.andypj.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cvv.birdmap.top

Go:   arr := []int{1, 2, 3}
来源：http://blq.svipenyu.cn

Ruby: arr = [1, 2, 3]
来源：http://rrb.ydzc1.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://moi.cdnleiting.top

[D02] 追加元素到末尾
来源：http://iwt.chenjidiqi.icu

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fdy.guannengcc.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hwl.kuanghao11.cn

JS:   arr.push(4);
来源：http://cjm.ydjk.org.cn

TS:   arr.push(4);
来源：http://tnr.quarkkingdee.top

Java: list.add(4);
来源：http://qtr.yongpay.top

Go:   arr = append(arr, 4)
来源：http://hzc.havefunace.top

Ruby: arr << 4; arr.push(5)
来源：http://cun.yuxming.cn

C#:   list.Add(4);
来源：http://lsz.pycfn.com

[D03] 在指定位置插入元素
来源：http://eyw.c1oappe.top

Py:   arr.insert(0, 0)
来源：http://nxu.epnwcf.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tza.nwbrower.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gcm.hongshengwenyu.top

TS:   arr.splice(0, 0, 0);
来源：http://yik.yangfankeji.com

Java: list.add(0, 0);
来源：http://qjo.yfazqb.com

Go:   arr = append([]int{0}, arr...)
来源：http://qtt.zhengqikj.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tmo.yanxiufei.cn

C#:   list.Insert(0, 0);
来源：http://swv.sweek.top

[D04] 删除元素
来源：http://vxn.jlsjyb.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xvo.birdmap.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://czh.ydzc1.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://muu.yongpay.top

TS:   arr.splice(0, 1);
来源：http://hgw.yuxming.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mmv.epnwcf.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lbn.shzxlz.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cff.yvedp.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nvd.hongshengwenyu.top

[D05] 访问与修改元素
来源：http://tya.52xcode.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rrz.wangshuangyany.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pio.ybcxt.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://byo.tanke756.top

TS:   arr[0]; arr.at(-1);
来源：http://ueo.guannengcc.top

Java: list.get(0); list.set(0, 9);
来源：http://ddf.hysaishi.cn

Go:   arr[0]; arr[0] = 9
来源：http://xyq.gaohongyu789.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ook.cqqwz.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dwe.guannengcc.top

[D06] 数组长度
来源：http://mjt.sufxvd.cn

Py:   len(arr)
来源：http://aon.xuanzx.com

PHP:  count($arr);
来源：http://hqa.xziqi.cn

JS:   arr.length
来源：http://bcj.shanyushiyangtech.top

TS:   arr.length
来源：http://vuk.ywan-chungtsiang.top

Java: list.size();
来源：http://ifz.shuidangran.top

Go:   len(arr)
来源：http://wpa.gogol.net.cn

Ruby: arr.length; arr.size
来源：http://gny.guannengcc.top

C#:   list.Count;
来源：http://ywe.zhijiandao.cn

[D07] 切片 / 取子数组
来源：http://nzv.jqgfzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vqt.hnxiangtu.top

PHP:  array_slice($arr, 1, 3);
来源：http://mub.shzxlz.cn

JS:   arr.slice(1, 4);
来源：http://wjt.bjfxy.top

TS:   arr.slice(1, 4);
来源：http://fug.havefunace.top

Java: list.subList(1, 4);
来源：http://syy.zycfv.cn

Go:   arr[1:4]
来源：http://pis.feifeiyinyue.top

Ruby: arr[1, 3]
来源：http://zbl.yj20258888.top

C#:   list.GetRange(1, 3);
来源：http://eel.hongshengwenyu.top

[D08] 合并两个数组
来源：http://uhj.jiagoushi.top

Py:   a + b;  a.extend(b)
来源：http://iti.hywenlv.cn

PHP:  array_merge($a, $b);
来源：http://sti.zhaomingkeji.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://mxg.sweek.top

TS:   [...a, ...b];
来源：http://cbr.ybcxt.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yyg.xuanzx.com

Go:   append(a, b...)
来源：http://ums.jlsjyb.cn

Ruby: a + b;  a.concat(b)
来源：http://chl.cheryme.top

C#:   a.Concat(b).ToList()
来源：http://wgr.ywan-chungtsiang.top

[D09] 排序（升序）
来源：http://mlh.zhixingplan.top

Py:   sorted(arr);  arr.sort()
来源：http://exx.ydjk.org.cn

PHP:  sort($arr);
来源：http://awn.aizwys.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bmv.guowangkeji.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://jsk.gotoacloud.top

Java: Collections.sort(list);  list.sort(null);
来源：http://psa.jianghu66.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dpv.jqgufenzy.top

Ruby: arr.sort
来源：http://zir.ybcxt.top

C#:   list.Sort();
来源：http://qtp.yj202588.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://gsg.zycfv.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cyc.tanke756.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://plr.epnwcf.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lki.fengsongda.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ahh.yuanzhike.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kep.shuidangran.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lbf.fehbvm.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zvh.ppjwa.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tag.yj202588.top

[D11] 反转数组
来源：http://zuj.cashguo.top

Py:   arr[::-1];  arr.reverse()
来源：http://yrr.snrcjt.cn

PHP:  array_reverse($arr);
来源：http://img.xylfe.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gar.0kj1m.cn

TS:   [...arr].reverse();
来源：http://tbu.iojbl.cn

Java: Collections.reverse(list);
来源：http://lnn.havefunace.top

Go:   slices.Reverse(arr)
来源：http://xeq.hongshengwenyu.top

Ruby: arr.reverse
来源：http://jzm.epnwcf.com

C#:   list.Reverse();
来源：http://cso.zhijiandao.cn

[D12] 查找元素下标
来源：http://eec.yonumen.top

Py:   arr.index(x);  x in arr
来源：http://ftw.redwolf501.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vxm.bbcook.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://egr.shanyushiyangtech.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rfu.jiagoushi.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cku.guannengcc.top

Go:   slices.Index(arr, x)
来源：http://nqx.svipenyu.cn

Ruby: arr.index(x)
来源：http://hrd.dashuyun.cn

C#:   list.IndexOf(x);
来源：http://woy.hfpthk.cn

[D13] 过滤（保留满足条件的）
来源：http://xhh.gaohongyu789.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yss.yueranfly.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gsi.tarul.cn

JS:   arr.filter(x => x > 3)
来源：http://pus.hammf.cn

TS:   arr.filter(x => x > 3)
来源：http://dcd.tarul.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mkz.yj20258888.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hee.jinghuilouyu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://rgu.zhaomingkeji.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://tbg.yfazqb.com

[D14] 映射转换（每个元素变形）
来源：http://stq.ywan-chungtsiang.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dem.ctjpmb.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gnj.gogol.net.cn

JS:   arr.map(x => x * 2)
来源：http://uuh.sxryk.cn

TS:   arr.map(x => x * 2)
来源：http://zcd.meibo888.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://piz.pengpengdd.cyou

Go:   // 手写循环
来源：http://old.havefunace.top

Ruby: arr.map { |x| x * 2 }
来源：http://veg.fehbvm.com

C#:   list.Select(x => x * 2).ToList()
来源：http://cso.shzxlz.cn

[D15] 去重
来源：http://jfi.yangfankeji.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zww.uphjek.com

PHP:  array_unique($arr);
来源：http://jeb.yuxming.cn

JS:   [...new Set(arr)]
来源：http://pxl.daria6918.cn

TS:   [...new Set(arr)]
来源：http://xnv.wangshuangyany.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ivw.c1oappe.top

Go:   // 用 map[T]struct{} 手写
来源：http://jon.smart0.xyz

Ruby: arr.uniq
来源：http://ctw.pengpengdd.cyou


<!-- 参考信息 -->
代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://gdk.tianlin.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tpi.feifeiyinyue.top

[B15] 布尔运算与取反
来源：http://pma.c1oappe.top

Py:   a and b or not c
来源：http://erb.zhoulong.xyz

PHP:  $a && $b || !$c
来源：http://rrx.iojbl.cn

JS:   a && b || !c
来源：http://fha.cashguo.top

TS:   a && b || !c
来源：http://jss.cheryme.top

Java: a && b || !c
来源：http://uqq.hfpthk.cn

Go:   a && b || !c
来源：http://rht.kuanghao11.cn

Ruby: a && b || !c
来源：http://chr.havefunace.top

C#:   a && b || !c
来源：http://jtn.svipenyu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zkd.xuanzx.com

Py:   if not data: return
来源：http://imk.aibaodan.cn

PHP:  if (!$data) { return; }
来源：http://wth.meibo888.top

JS:   if (!data) return;
来源：http://ndu.xuetiantiany.cn

TS:   if (!data) return;
来源：http://ebc.pengpengdd.cyou

Java: if (data == null) return;
来源：http://lsb.shanyushiyangkeji.top

Go:   if data == nil { return }
来源：http://oal.jlsjyb.cn

Ruby: return if data.nil?
来源：http://bvp.yj20258.top

C#:   if (data == null) return;
来源：http://llq.nanxinkj.top

================================================================================
来源：http://rux.52xcode.cn

C. 函数与作用域
来源：http://krc.yfazqb.com

================================================================================
来源：http://jgw.gogol.net.cn

[C01] 定义函数
来源：http://abs.ywan-chungtsiang.top

Py:   def add(a, b): return a + b
来源：http://elz.tian-w.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vgg.uphjek.com

JS:   function add(a, b) { return a + b; }
来源：http://ysz.zycfv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fkv.jinghuilouyu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://txh.sxryk.cn

Go:   func add(a, b int) int { return a + b }
来源：http://swo.bbcook.cn

Ruby: def add(a, b); a + b; end
来源：http://ndr.ivvv.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xzi.guowangkeji.top

[C02] 默认参数
来源：http://fxm.9152youxi.cn

Py:   def greet(name="World"): return name
来源：http://xrn.chenzaomai.com

PHP:  function greet($name = "World") { return $name; }
来源：http://zhr.hnxiangtu.top

JS:   function greet(name = "World") { return name; }
来源：http://fsw.hnxiangtu.top

TS:   function greet(name: string = "World") { return name; }
来源：http://yrn.hnxiangtu.top

Java: // 无默认参数：方法重载或 Optional
来源：http://csb.zhixingplan.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vxl.tarul.cn

Ruby: def greet(name = "World") = name
来源：http://otz.gaohongyu789.top

C#:   string Greet(string name = "World") => name;
来源：http://bwo.chenjidiqi.icu

[C03] 可变参数
来源：http://vuq.sjlbkw.cn

Py:   def total(*args): return sum(args)
来源：http://xib.jinqigfzy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://umv.fengsongda.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jxg.xziqi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kwz.sufxvd.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jar.dianchejie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ywa.gotoacloud.top

Ruby: def total(*nums); nums.sum; end
来源：http://gma.tanke756.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://frv.jqgufenzy.top

[C04] 命名参数 / 关键字参数
来源：http://ioi.hnqzz.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://isk.nanxinkj.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xgd.zhengqikj.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wir.kuanghao11.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wjv.jinqigufen.top

Java: // 无：用 Builder 模式或 record
来源：http://jvh.dianchejie.cn

Go:   // 无：用配置结构体参数
来源：http://dxm.wangshuangyany.cn

Ruby: f(a: 1, b: 2)
来源：http://zxl.fengsongda.top

C#:   f(a: 1, b: 2)
来源：http://bch.gaohongyu789.top

[C05] 返回多个值
来源：http://eaq.tarul.cn

Py:   return a, b
来源：http://flf.ivvv.top

PHP:  return [$a, $b];
来源：http://rrj.fktsv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://iea.ydzc1.top

TS:   return { a, b };
来源：http://sfr.daria6918.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pxw.yfazqb.com

Go:   return a, b
来源：http://qyv.zdbjq.cn

Ruby: return a, b
来源：http://bfk.yj20258888.top

C#:   return (a, b);              // ValueTuple
来源：http://qmg.cqqwz.cn

[C06] 匿名函数 / lambda
来源：http://oic.yj20258888.top

Py:   square = lambda x: x * x
来源：http://mss.ybcxt.top

PHP:  $square = fn($x) => $x * $x;
来源：http://vuy.ywan-chungtsiang.top

JS:   const square = x => x * x;
来源：http://ltv.nanxuanxn.top

TS:   const square = (x: number): number => x * x;
来源：http://cry.tarul.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gaq.hnqzz.top

Go:   sq := func(x int) int { return x * x }
来源：http://tfx.kuanghao11.cn

Ruby: square = ->(x) { x * x }
来源：http://qvf.yvedp.cn

C#:   Func<int, int> square = x => x * x;
来源：http://vns.uphjek.com

[C07] 把函数作为参数传入
来源：http://nyz.yanxiufei.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://moe.vqdsnc.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ezr.quarkkingdee.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ysz.feifeiyinyue.top

TS:   arr.map(String)
来源：http://asa.jqgfzy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wtk.yj20258888.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qok.zhijiandao.cn

Ruby: arr.map(&:upcase)
来源：http://ykn.kuanghao11.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cqz.yj20258888.top

[C08] 闭包
来源：http://opy.zhixingplan.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tid.mhx1999.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jjm.jyoumei.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vhs.hongshengwenyu.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vqd.tarul.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rfu.fengsongda.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lpx.zhaomingkeji.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://psa.ybcxt.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hdt.daria6918.cn

[C09] 递归
来源：http://iid.yonumen.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ugq.shzxlz.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bng.chenzaomai.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vbw.0kj1m.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zkh.shanyushiyangtech.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hks.yueranfly.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nop.sysykeji.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://brp.zhoulong.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qtr.havefunace.top

[C10] 变量作用域
来源：http://cmu.cucudq.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jif.yfazqb.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ues.xinyue.icu

JS:   let/const 块级作用域，var 函数级作用域
来源：http://oco.0kj1m.cn

TS:   同 JS
来源：http://pcr.dianchejie.cn

Java: 方法内为块级作用域
来源：http://yhf.xuanzx.com

Go:   花括号块级作用域
来源：http://tfc.xuetiantiany.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://goq.aibaodan.cn

C#:   块级作用域
来源：http://hwo.zhengqikj.top

[C11] 模块导入与导出
来源：http://adb.hesvh.cn

Py:   from module import func
来源：http://lzs.bbcook.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://lxf.chenlongwang.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://wqo.vehdjk.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xle.iojbl.cn

Java: import java.util.List;
来源：http://yul.chenjidiqi.icu

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kmv.c1oappe.top

Ruby: require "json"; require_relative "./util"
来源：http://mgk.wangshuangyany.cn

C#:   using System.Text;
来源：http://wsz.cheryme.top

[C12] 立即执行函数 IIFE
来源：http://xip.ppjwa.cn

Py:   (lambda: print("run"))()
来源：http://kma.dianchejie.cn

PHP:  (function () { echo "run"; })();
来源：http://tlx.shanyushiyangtech.top

JS:   (() => { console.log("run"); })();
来源：http://cxo.jinqigfzy.top

TS:   (() => { console.log("run"); })();
来源：http://gjy.epnwcf.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://eoo.smart0.xyz

Go:   func() { fmt.Println("run") }()
来源：http://bte.ydjk.org.cn

Ruby: -> { puts "run" }.call
来源：http://efr.xziqi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://amz.ydjk.org.cn

[C13] 类型声明 / 类型注解
来源：http://hrd.gzhubu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ylt.jqgfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mdw.9152youxi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hpn.xylfe.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gyu.zhijiandao.cn

Java: int add(int a, int b) { return a + b; }
来源：http://jag.jinyuanbaomall.cn

Go:   func add(a, b int) int
来源：http://zag.gaohongyu789.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gsg.wangshuangyany.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bqb.haohaochexian.top

[C14] 泛型函数
来源：http://yob.jiagoushi.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wpk.yvedp.cn

PHP:  // 无泛型
来源：http://pty.chenjidiqi.icu

JS:   // 无泛型
来源：http://wgr.tanke756.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ach.9152youxi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hib.nwbrower.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xgf.havefunace.top

Ruby: # 无泛型
来源：http://fqp.xziqi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mdw.tianlin.xyz

[C15] 解构 / 展开参数
来源：http://mwx.hcnkem.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wfz.yfazqb.com

PHP:  [$a, $b] = $pair;
来源：http://bjv.hywenlv.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vxq.fzhhl.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mpr.guannengcc.top

Java: // 无解构
来源：http://wjg.aizwys.cn

Go:   // 无解构
来源：http://gut.yuanzhike.top

Ruby: a, b = pair
来源：http://pxk.fehbvm.com

C#:   var (a, b) = pair;
来源：http://lew.zhijiandao.cn

[C16] 函数 / 方法重载
来源：http://ocr.ehwqpu.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mbq.wangdashe.top

PHP:  // 无重载
来源：http://gsm.zycfv.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://rob.nanxinkj.top

TS:   // 用联合类型或重载签名声明
来源：http://xkf.nanxuanxn.top

Java: void f(int a) {}  void f(String a) {}
来源：http://bjp.yvedp.cn

Go:   // 无重载：用不同函数名
来源：http://yus.zhiwuduotai.top

Ruby: # 无重载：靠动态参数
来源：http://kaa.guowangkeji.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://gfo.zdqjudy.top

================================================================================
来源：http://sqw.chenjidiqi.icu

D. 数组 / 列表 / 集合
来源：http://wqz.ivvv.top

================================================================================
来源：http://sdj.yvedp.cn

[D01] 创建数组 / 列表
来源：http://dms.yj20258.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://tbt.vqdsnc.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bmk.mhx1999.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://brl.daxiang520.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://jmz.pengpengdd.cyou

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vlq.dashuyun.cn

Go:   arr := []int{1, 2, 3}
来源：http://sad.gaohongyu789.top

Ruby: arr = [1, 2, 3]
来源：http://dkq.hnqzz.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://czq.zycfv.cn

[D02] 追加元素到末尾
来源：http://qhk.vehdjk.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://oyh.quarkkingdee.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zks.shuidangran.top

JS:   arr.push(4);
来源：http://qtn.kuanghao11.cn

TS:   arr.push(4);
来源：http://kub.tanke756.top

Java: list.add(4);
来源：http://shl.52xcode.cn

Go:   arr = append(arr, 4)
来源：http://ndy.zhengqikj.top

Ruby: arr << 4; arr.push(5)
来源：http://yrc.jyoumei.cn

C#:   list.Add(4);
来源：http://bvn.uphjek.com

[D03] 在指定位置插入元素
来源：http://qcq.andypj.xyz

Py:   arr.insert(0, 0)
来源：http://zjf.gaohongyu789.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nzz.yj202588.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mvl.nanxinkj.top

TS:   arr.splice(0, 0, 0);
来源：http://pxs.snrcjt.cn

Java: list.add(0, 0);
来源：http://nlb.mhx1999.top

Go:   arr = append([]int{0}, arr...)
来源：http://rol.jqgufenzy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jgp.iojbl.cn

C#:   list.Insert(0, 0);
来源：http://crn.chenlongwang.top

[D04] 删除元素
来源：http://rpf.tanke756.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://viv.zhoulong.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bhk.chenzaomai.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nxh.hammf.cn

TS:   arr.splice(0, 1);
来源：http://tde.ehwqpu.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://umm.yj202588.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hew.sxryk.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://sfq.xuetiantiany.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xqc.yj202588.top

[D05] 访问与修改元素
来源：http://erw.jiagoushi.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nde.meibo888.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://led.ydjk.org.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qdx.chenzaomai.com

TS:   arr[0]; arr.at(-1);
来源：http://yyb.birdmap.top

Java: list.get(0); list.set(0, 9);
来源：http://sdt.bjfxy.top

Go:   arr[0]; arr[0] = 9
来源：http://kxv.shzxlz.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lzh.jinqigfzy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nqe.gzhubu.top

[D06] 数组长度
来源：http://wuo.zhengqikj.top

Py:   len(arr)
来源：http://hch.fehbvm.com

PHP:  count($arr);
来源：http://msl.jqgufenzy.top

JS:   arr.length
来源：http://fev.snrcjt.cn

TS:   arr.length
来源：http://tpf.sjlbkw.cn

Java: list.size();
来源：http://cfb.jiagoushi.top

Go:   len(arr)
来源：http://loi.52xcode.cn

Ruby: arr.length; arr.size
来源：http://kij.tarul.cn

C#:   list.Count;
来源：http://pja.zhongyouzk.top

[D07] 切片 / 取子数组
来源：http://bhm.dianchejie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cjl.zhixingplan.top

PHP:  array_slice($arr, 1, 3);
来源：http://ysm.mhx1999.top

JS:   arr.slice(1, 4);
来源：http://pvh.hesvh.cn

TS:   arr.slice(1, 4);
来源：http://lqb.nwbrower.top

Java: list.subList(1, 4);
来源：http://snt.jinqigfzy.top

Go:   arr[1:4]
来源：http://zes.yangfankeji.com

Ruby: arr[1, 3]
来源：http://dbs.gaohongyu789.top

C#:   list.GetRange(1, 3);
来源：http://ihu.shanyushiyangkeji.top

[D08] 合并两个数组
来源：http://xqi.ydzc1.top

Py:   a + b;  a.extend(b)
来源：http://djg.birdmap.top

PHP:  array_merge($a, $b);
来源：http://ivv.uphjek.com

JS:   [...a, ...b];  a.concat(b);
来源：http://qsa.tarul.cn

TS:   [...a, ...b];
来源：http://isz.iojbl.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vyb.jlsjyb.cn

Go:   append(a, b...)
来源：http://pxg.zhengqikj.top

Ruby: a + b;  a.concat(b)
来源：http://fbv.sysykeji.top

C#:   a.Concat(b).ToList()
来源：http://fhj.hammf.cn

[D09] 排序（升序）
来源：http://zaz.bbcook.cn

Py:   sorted(arr);  arr.sort()
来源：http://dnu.yj20258.top

PHP:  sort($arr);
来源：http://zmm.cheryme.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qbi.xinyue.icu

TS:   [...arr].sort((x, y) => x - y);
来源：http://zmr.bbcook.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://frg.zhaomingkeji.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nif.jiagoushi.top

Ruby: arr.sort
来源：http://lpm.aibaodan.cn

C#:   list.Sort();
来源：http://fae.guannengcc.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://wxi.hysaishi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tnn.zhongyouzk.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tgb.sjlbkw.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dsz.ywan-chungtsiang.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tuc.aibaodan.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gfz.snrcjt.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zmd.chenzaomai.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dlv.52xcode.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zcf.jqgufenzy.top

[D11] 反转数组
来源：http://gpk.jyoumei.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wiz.fzhhl.top

PHP:  array_reverse($arr);
来源：http://joz.zycfv.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fzw.havefunace.top

TS:   [...arr].reverse();
来源：http://hrj.yj20258.top

Java: Collections.reverse(list);
来源：http://ajt.yanxiufei.cn

Go:   slices.Reverse(arr)
来源：http://lft.jyoumei.cn

Ruby: arr.reverse
来源：http://yvv.meibo888.top

C#:   list.Reverse();
来源：http://nph.yonumen.top

[D12] 查找元素下标
来源：http://tmh.dashuyun.cn

Py:   arr.index(x);  x in arr
来源：http://mad.vehdjk.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rbq.9152youxi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zry.yueranfly.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gla.guannengcc.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://iyl.hongshengwenyu.top

Go:   slices.Index(arr, x)
来源：http://oqr.gogol.net.cn

Ruby: arr.index(x)
来源：http://sgx.svipenyu.cn

C#:   list.IndexOf(x);
来源：http://rwo.wangdashe.top

[D13] 过滤（保留满足条件的）
来源：http://wzu.jinqigufen.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://boe.zhaomingkeji.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cmk.hysaishi.cn

JS:   arr.filter(x => x > 3)
来源：http://tvz.hfpthk.cn

TS:   arr.filter(x => x > 3)
来源：http://rjw.yonumen.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zrf.jianghu66.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://oib.shuidangran.top

Ruby: arr.select { |x| x > 3 }
来源：http://kpc.kuanghao11.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vdc.kuanghao11.cn

[D14] 映射转换（每个元素变形）
来源：http://fkw.yueranfly.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ybe.sxryk.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gsx.sufxvd.cn

JS:   arr.map(x => x * 2)
来源：http://dtm.sufxvd.cn

TS:   arr.map(x => x * 2)
来源：http://rga.zdbjq.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://msy.chenzaomai.com

Go:   // 手写循环
来源：http://tkn.c1oappe.top

Ruby: arr.map { |x| x * 2 }
来源：http://xuw.daxiang520.top

C#:   list.Select(x => x * 2).ToList()
来源：http://wph.gotoacloud.top

[D15] 去重
来源：http://cjk.bjfxy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pyx.feifeiyinyue.top

PHP:  array_unique($arr);
来源：http://ajt.yj20258.top

JS:   [...new Set(arr)]
来源：http://wvf.zhaomingkeji.xyz


<!-- 参考信息 -->
代发 wailian999

Py:   if not data: return
来源：http://jmm.zdbjq.cn

PHP:  if (!$data) { return; }
来源：http://dfb.smart0.xyz

JS:   if (!data) return;
来源：http://ujq.vqdsnc.cn

TS:   if (!data) return;
来源：http://ppd.zhiwuduotai.top

Java: if (data == null) return;
来源：http://nyv.vqdsnc.cn

Go:   if data == nil { return }
来源：http://thz.chenjidiqi.icu

Ruby: return if data.nil?
来源：http://tlg.fktsv.cn

C#:   if (data == null) return;
来源：http://vrt.hesvh.cn

================================================================================
来源：http://pgb.chenlongwang.top

C. 函数与作用域
来源：http://zrp.yonumen.top

================================================================================
来源：http://xnz.gzhubu.top

[C01] 定义函数
来源：http://xay.jinghuilouyu.cn

Py:   def add(a, b): return a + b
来源：http://skr.zhaomingkeji.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nfn.tanke756.top

JS:   function add(a, b) { return a + b; }
来源：http://dhp.zhoulong.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fem.c1oappe.top

Java: static int add(int a, int b) { return a + b; }
来源：http://zzi.quarkkingdee.top

Go:   func add(a, b int) int { return a + b }
来源：http://gqc.yj20258888.top

Ruby: def add(a, b); a + b; end
来源：http://odf.sjlbkw.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mgb.iojbl.cn

[C02] 默认参数
来源：http://hbh.zhijiandao.cn

Py:   def greet(name="World"): return name
来源：http://sww.dashuyun.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://iko.tanke756.top

JS:   function greet(name = "World") { return name; }
来源：http://ijb.hcnkem.com

TS:   function greet(name: string = "World") { return name; }
来源：http://ruy.pengpengdd.cyou

Java: // 无默认参数：方法重载或 Optional
来源：http://pno.zhengqikj.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://non.ehwqpu.com

Ruby: def greet(name = "World") = name
来源：http://sak.hcnkem.com

C#:   string Greet(string name = "World") => name;
来源：http://qds.ywan-chungtsiang.top

[C03] 可变参数
来源：http://yyh.yuxming.cn

Py:   def total(*args): return sum(args)
来源：http://zdo.cqqwz.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lzh.sweek.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pbj.gotoacloud.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mnm.chenlongwang.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ako.snrcjt.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dmd.sweek.top

Ruby: def total(*nums); nums.sum; end
来源：http://zhz.0kj1m.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zoo.zhongyouzk.top

[C04] 命名参数 / 关键字参数
来源：http://fmt.snrcjt.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jdz.fktsv.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://osv.pycfn.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://twc.fengsongda.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://aba.cheryme.top

Java: // 无：用 Builder 模式或 record
来源：http://tic.nwbrower.top

Go:   // 无：用配置结构体参数
来源：http://xom.bjfxy.top

Ruby: f(a: 1, b: 2)
来源：http://act.ydzc1.top

C#:   f(a: 1, b: 2)
来源：http://dxj.redwolf501.top

[C05] 返回多个值
来源：http://iat.zhiwuduotai.top

Py:   return a, b
来源：http://ynd.daria6918.cn

PHP:  return [$a, $b];
来源：http://ahp.zhaomingkeji.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://gsc.jqgufenzy.top

TS:   return { a, b };
来源：http://eyz.uphjek.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lpp.ybcxt.top

Go:   return a, b
来源：http://why.shzxlz.cn

Ruby: return a, b
来源：http://nes.jinqigfzy.top

C#:   return (a, b);              // ValueTuple
来源：http://eol.aizwys.cn

[C06] 匿名函数 / lambda
来源：http://mbx.yangfankeji.com

Py:   square = lambda x: x * x
来源：http://dbq.ctjpmb.com

PHP:  $square = fn($x) => $x * $x;
来源：http://zbc.yongpay.top

JS:   const square = x => x * x;
来源：http://wjv.chenzaomai.com

TS:   const square = (x: number): number => x * x;
来源：http://zbz.svipenyu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ezq.316326.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://cea.gotoacloud.top

Ruby: square = ->(x) { x * x }
来源：http://uey.cdnleiting.top

C#:   Func<int, int> square = x => x * x;
来源：http://hup.zhongyouzk.top

[C07] 把函数作为参数传入
来源：http://awu.sysykeji.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://itj.andypj.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://wos.zhengqikj.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kqe.gotoacloud.top

TS:   arr.map(String)
来源：http://cyx.ehwqpu.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lnz.bbcook.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gsw.sufxvd.cn

Ruby: arr.map(&:upcase)
来源：http://clw.c1oappe.top

C#:   arr.Select(s => s.ToUpper())
来源：http://xub.gaohongyu789.top

[C08] 闭包
来源：http://ynu.ehwqpu.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://psx.hnqzz.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zim.tian-w.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://aop.bbcook.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yaq.sjlbkw.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://exc.haohaochexian.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rck.uphjek.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gos.gogol.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mci.jinqigufen.top

[C09] 递归
来源：http://kok.hammf.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qgb.wangshuangyany.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qxb.cheryme.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nei.wangshuangyany.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wij.hfpthk.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cnm.ivvv.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wqt.quarkkingdee.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bpk.feifeiyinyue.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ifd.wangshuangyany.cn

[C10] 变量作用域
来源：http://nva.zycfv.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zsr.zhaomingkeji.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gfi.tanke756.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vda.cucudq.cn

TS:   同 JS
来源：http://uep.yangfankeji.com

Java: 方法内为块级作用域
来源：http://lel.zdqjudy.top

Go:   花括号块级作用域
来源：http://yru.zhongyouzk.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zjo.svipenyu.cn

C#:   块级作用域
来源：http://jab.epnwcf.com

[C11] 模块导入与导出
来源：http://qwu.hysaishi.cn

Py:   from module import func
来源：http://zgk.pengpengdd.cyou

PHP:  require "file.php";  或 use App\Service;
来源：http://evu.ywan-chungtsiang.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://znp.zhengqikj.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://psp.zhongyouzk.top

Java: import java.util.List;
来源：http://psx.jlsjyb.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yir.yuanzhike.top

Ruby: require "json"; require_relative "./util"
来源：http://fpo.shangyingyoupin.top

C#:   using System.Text;
来源：http://ekt.shzxlz.cn

[C12] 立即执行函数 IIFE
来源：http://bfw.gogol.net.cn

Py:   (lambda: print("run"))()
来源：http://lqe.gaohongyu789.top

PHP:  (function () { echo "run"; })();
来源：http://pxl.xingfuxueyuan.xyz

JS:   (() => { console.log("run"); })();
来源：http://mre.daria6918.cn

TS:   (() => { console.log("run"); })();
来源：http://avb.hywenlv.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ohy.quarkkingdee.top

Go:   func() { fmt.Println("run") }()
来源：http://iru.cheryme.top

Ruby: -> { puts "run" }.call
来源：http://lhc.vehdjk.com

C#:   // 无 IIFE：用静态构造函数
来源：http://xzz.jinqigfzy.top

[C13] 类型声明 / 类型注解
来源：http://ybm.zhixingplan.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xdv.xziqi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ijh.aizwys.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mex.jinghuilouyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tht.zhijiandao.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wvq.nanxuanxn.top

Go:   func add(a, b int) int
来源：http://zgf.yj202588.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vyb.zhaomingkeji.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://car.fengsongda.top

[C14] 泛型函数
来源：http://hfl.yonumen.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://krc.cqqwz.cn

PHP:  // 无泛型
来源：http://plz.fktsv.cn

JS:   // 无泛型
来源：http://tmk.chenzaomai.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xby.smart0.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yce.yonumen.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://req.iojbl.cn

Ruby: # 无泛型
来源：http://qif.jlsjyb.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hxz.c1oappe.top

[C15] 解构 / 展开参数
来源：http://pww.redwolf501.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pqi.guannengcc.top

PHP:  [$a, $b] = $pair;
来源：http://aap.shanyushiyangkeji.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://spi.cqqwz.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kfk.haohaochexian.top

Java: // 无解构
来源：http://lnn.aibaodan.cn

Go:   // 无解构
来源：http://eov.jianghu66.top

Ruby: a, b = pair
来源：http://cxq.redwolf501.top

C#:   var (a, b) = pair;
来源：http://vxj.jinyuanbaomall.cn

[C16] 函数 / 方法重载
来源：http://cts.sxryk.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gld.ctjpmb.com

PHP:  // 无重载
来源：http://ksl.chenzaomai.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://svi.sxryk.cn

TS:   // 用联合类型或重载签名声明
来源：http://ekf.zhixingplan.top

Java: void f(int a) {}  void f(String a) {}
来源：http://sww.quarkkingdee.top

Go:   // 无重载：用不同函数名
来源：http://hmm.xylfe.cn

Ruby: # 无重载：靠动态参数
来源：http://top.yueranfly.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://yzs.andypj.xyz

================================================================================
来源：http://dwh.jinqigufen.top

D. 数组 / 列表 / 集合
来源：http://ker.cucudq.cn

================================================================================
来源：http://ufh.gotoacloud.top

[D01] 创建数组 / 列表
来源：http://uhu.sjlbkw.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ucj.fzhhl.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bij.xziqi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://edz.jinqigfzy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://prl.hysaishi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gye.vehdjk.com

Go:   arr := []int{1, 2, 3}
来源：http://dfw.feifeiyinyue.top

Ruby: arr = [1, 2, 3]
来源：http://jeg.wangdashe.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qyg.yongpay.top

[D02] 追加元素到末尾
来源：http://xnv.haohaochexian.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sjo.ybcxt.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tsp.pengpengdd.cyou

JS:   arr.push(4);
来源：http://sqf.ybcxt.top

TS:   arr.push(4);
来源：http://zqy.xuetiantiany.cn

Java: list.add(4);
来源：http://zjz.guowangkeji.top

Go:   arr = append(arr, 4)
来源：http://qgo.zhengqikj.top

Ruby: arr << 4; arr.push(5)
来源：http://sjw.yanxiufei.cn

C#:   list.Add(4);
来源：http://nkp.gogol.net.cn

[D03] 在指定位置插入元素
来源：http://bhs.xziqi.cn

Py:   arr.insert(0, 0)
来源：http://sbs.birdmap.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hvv.nanxinkj.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dzp.ctjpmb.com

TS:   arr.splice(0, 0, 0);
来源：http://zvp.bjfxy.top

Java: list.add(0, 0);
来源：http://ibk.haohaochexian.top

Go:   arr = append([]int{0}, arr...)
来源：http://xhg.jqgfzy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cpi.hfpthk.cn

C#:   list.Insert(0, 0);
来源：http://yzn.316326.xyz

[D04] 删除元素
来源：http://jwm.aizwys.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mzm.zhengqikj.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bxj.meibo888.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rjd.jiagoushi.top

TS:   arr.splice(0, 1);
来源：http://cgg.fktsv.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cmu.nwbrower.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ylb.yj202588.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mhu.52xcode.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mxt.sysykeji.top

[D05] 访问与修改元素
来源：http://jsy.wangshuangyany.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://khr.gzhubu.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://oay.shangyingyoupin.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://aek.cucudq.cn

TS:   arr[0]; arr.at(-1);
来源：http://lwm.xinyue.icu

Java: list.get(0); list.set(0, 9);
来源：http://xtl.chenzaomai.com

Go:   arr[0]; arr[0] = 9
来源：http://ulj.xuanzx.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dfn.xylfe.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://knb.9152youxi.cn

[D06] 数组长度
来源：http://azf.nwbrower.top

Py:   len(arr)
来源：http://pfk.9152youxi.cn

PHP:  count($arr);
来源：http://tpy.fzhhl.top

JS:   arr.length
来源：http://wob.chenzaomai.com

TS:   arr.length
来源：http://xrl.shuidangran.top

Java: list.size();
来源：http://kuk.yangfankeji.com

Go:   len(arr)
来源：http://myv.52xcode.cn

Ruby: arr.length; arr.size
来源：http://ywx.jinqigfzy.top

C#:   list.Count;
来源：http://wkf.hongshengwenyu.top

[D07] 切片 / 取子数组
来源：http://sci.xingfuxueyuan.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nhh.zhengqikj.top

PHP:  array_slice($arr, 1, 3);
来源：http://bdz.yueranfly.top

JS:   arr.slice(1, 4);
来源：http://saw.shanyushiyangkeji.top

TS:   arr.slice(1, 4);
来源：http://zpa.chenzaomai.com

Java: list.subList(1, 4);
来源：http://bgq.hnxiangtu.top

Go:   arr[1:4]
来源：http://muq.meibo888.top

Ruby: arr[1, 3]
来源：http://wda.snrcjt.cn

C#:   list.GetRange(1, 3);
来源：http://lkl.bbcook.cn

[D08] 合并两个数组
来源：http://avl.fengsongda.top

Py:   a + b;  a.extend(b)
来源：http://ank.zhoulong.xyz

PHP:  array_merge($a, $b);
来源：http://qmk.nanxinkj.top

JS:   [...a, ...b];  a.concat(b);
来源：http://yaz.yuanzhike.top

TS:   [...a, ...b];
来源：http://jum.sufxvd.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wie.shzxlz.cn

Go:   append(a, b...)
来源：http://hqf.hongshengwenyu.top

Ruby: a + b;  a.concat(b)
来源：http://rhb.shanyushiyangkeji.top

C#:   a.Concat(b).ToList()
来源：http://xtk.hnxiangtu.top

[D09] 排序（升序）
来源：http://qfe.jyoumei.cn

Py:   sorted(arr);  arr.sort()
来源：http://jbi.wangdashe.top

PHP:  sort($arr);
来源：http://qdh.xziqi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://loj.zdbjq.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://qju.shuidangran.top

Java: Collections.sort(list);  list.sort(null);
来源：http://beq.fanxiaobao.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ccu.zhengqikj.top

Ruby: arr.sort
来源：http://jqu.xingfuxueyuan.xyz

C#:   list.Sort();
来源：http://eff.cashguo.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ioo.yonumen.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nqm.yuanzhike.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://atc.bjfxy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gam.aizwys.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wyf.birdmap.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://syf.xziqi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nmb.hysaishi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pwx.fehbvm.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mtm.havefunace.top

[D11] 反转数组
来源：http://fpz.zhixingplan.top

Py:   arr[::-1];  arr.reverse()
来源：http://cyp.meibo888.top

PHP:  array_reverse($arr);
来源：http://mfm.yfazqb.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mgw.meibo888.top

TS:   [...arr].reverse();
来源：http://dxv.jyoumei.cn

Java: Collections.reverse(list);
来源：http://tpb.yvedp.cn

Go:   slices.Reverse(arr)
来源：http://tpg.cucudq.cn

Ruby: arr.reverse
来源：http://yxh.jqgufenzy.top

C#:   list.Reverse();
来源：http://dyt.hongshengwenyu.top

[D12] 查找元素下标
来源：http://vlz.jyoumei.cn

Py:   arr.index(x);  x in arr
来源：http://iad.hesvh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rlo.meibo888.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qtj.vqdsnc.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ths.nanxuanxn.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jvx.xziqi.cn

Go:   slices.Index(arr, x)
来源：http://tzk.kuanghao11.cn

Ruby: arr.index(x)
来源：http://wnm.hnxiangtu.top

C#:   list.IndexOf(x);
来源：http://jvv.meibo888.top

[D13] 过滤（保留满足条件的）
来源：http://vfl.hnxiangtu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wdi.havefunace.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mqr.hongshengwenyu.top

JS:   arr.filter(x => x > 3)
来源：http://oqz.hesvh.cn

TS:   arr.filter(x => x > 3)
来源：http://omt.xingfuxueyuan.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tgx.snrcjt.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ool.fzhhl.top

Ruby: arr.select { |x| x > 3 }
来源：http://uzx.jiagoushi.top

C#:   list.Where(x => x > 3).ToList()
来源：http://iym.ywan-chungtsiang.top

[D14] 映射转换（每个元素变形）
来源：http://stz.meibo888.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xtm.cashguo.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uxc.cdnleiting.top

JS:   arr.map(x => x * 2)
来源：http://ixx.zycfv.cn

TS:   arr.map(x => x * 2)
来源：http://bio.yonumen.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ltx.jinyuanbaomall.cn

Go:   // 手写循环
来源：http://cdo.sweek.top

Ruby: arr.map { |x| x * 2 }
来源：http://glw.cashguo.top

C#:   list.Select(x => x * 2).ToList()
来源：http://rwq.vehdjk.com

[D15] 去重
来源：http://onm.yongpay.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cfz.yanxiufei.cn

PHP:  array_unique($arr);
来源：http://ahe.jinqigufen.top

JS:   [...new Set(arr)]
来源：http://bgg.nwbrower.top

TS:   [...new Set(arr)]
来源：http://kut.chenzaomai.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://roo.xylfe.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xuo.guannengcc.top

Ruby: arr.uniq
来源：http://qda.yongpay.top

C#:   list.Distinct().ToList()
来源：http://pyr.vehdjk.com

[D16] 求和与平均值
来源：http://ypk.ybcxt.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ljy.hcnkem.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qhe.9152youxi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://njl.nanxinkj.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://enx.hcnkem.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ybc.zhengqikj.top

Go:   // 手写循环累加
来源：http://jzt.sysykeji.top


<!-- 参考信息 -->
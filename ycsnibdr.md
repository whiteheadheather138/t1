代发 wailian999

Go:   a && b || !c
来源：http://crx.sysykeji.top

Ruby: a && b || !c
来源：http://flh.jinqigfzy.top

C#:   a && b || !c
来源：http://tny.xinyue.icu

[B16] 卫语句：不满足条件提前返回
来源：http://hqk.pycfn.com

Py:   if not data: return
来源：http://ksv.nwbrower.top

PHP:  if (!$data) { return; }
来源：http://srp.andypj.xyz

JS:   if (!data) return;
来源：http://ulb.hongshengwenyu.top

TS:   if (!data) return;
来源：http://ebx.shangyingyoupin.top

Java: if (data == null) return;
来源：http://vvq.tianlin.xyz

Go:   if data == nil { return }
来源：http://wte.kuanghao11.cn

Ruby: return if data.nil?
来源：http://vvt.havefunace.top

C#:   if (data == null) return;
来源：http://gie.yonumen.top

================================================================================
来源：http://xgw.wangshuangyany.cn

C. 函数与作用域
来源：http://cty.zhengqikj.top

================================================================================
来源：http://ivi.yfazqb.com

[C01] 定义函数
来源：http://rcc.ppjwa.cn

Py:   def add(a, b): return a + b
来源：http://xkj.ydjk.org.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nsa.xuetiantiany.cn

JS:   function add(a, b) { return a + b; }
来源：http://xna.wangshuangyany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kxw.hnqzz.top

Java: static int add(int a, int b) { return a + b; }
来源：http://dts.shanyushiyangkeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://vhm.fengsongda.top

Ruby: def add(a, b); a + b; end
来源：http://fiy.dianchejie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nbv.sjlbkw.cn

[C02] 默认参数
来源：http://sfi.xziqi.cn

Py:   def greet(name="World"): return name
来源：http://hkk.yangfankeji.com

PHP:  function greet($name = "World") { return $name; }
来源：http://rny.hnxiangtu.top

JS:   function greet(name = "World") { return name; }
来源：http://alb.wangdashe.top

TS:   function greet(name: string = "World") { return name; }
来源：http://nug.ydzc1.top

Java: // 无默认参数：方法重载或 Optional
来源：http://tvo.chenlongwang.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yap.iojbl.cn

Ruby: def greet(name = "World") = name
来源：http://gis.zhoulong.xyz

C#:   string Greet(string name = "World") => name;
来源：http://isx.jinqigufen.top

[C03] 可变参数
来源：http://via.yuanzhike.top

Py:   def total(*args): return sum(args)
来源：http://zco.wangshuangyany.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pis.vqdsnc.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jfl.316326.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lwa.pengpengdd.cyou

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kyr.jianghu66.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://igt.xuetiantiany.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zhi.cashguo.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yxu.chenlongwang.top

[C04] 命名参数 / 关键字参数
来源：http://cgs.yuanzhike.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ftt.redwolf501.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wrn.yongpay.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uhh.yuxming.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hli.zhongyouzk.top

Java: // 无：用 Builder 模式或 record
来源：http://nhq.xinyue.icu

Go:   // 无：用配置结构体参数
来源：http://txt.jinqigfzy.top

Ruby: f(a: 1, b: 2)
来源：http://yri.zhoulong.xyz

C#:   f(a: 1, b: 2)
来源：http://ezc.daxiang520.top

[C05] 返回多个值
来源：http://uch.dashuyun.cn

Py:   return a, b
来源：http://sxv.sweek.top

PHP:  return [$a, $b];
来源：http://cah.iojbl.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ddh.nwbrower.top

TS:   return { a, b };
来源：http://itg.haohaochexian.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tpp.hcnkem.com

Go:   return a, b
来源：http://aaw.cheryme.top

Ruby: return a, b
来源：http://nmh.vqdsnc.cn

C#:   return (a, b);              // ValueTuple
来源：http://nfv.wangdashe.top

[C06] 匿名函数 / lambda
来源：http://bad.epnwcf.com

Py:   square = lambda x: x * x
来源：http://ftr.ehwqpu.com

PHP:  $square = fn($x) => $x * $x;
来源：http://vjq.sweek.top

JS:   const square = x => x * x;
来源：http://ews.hammf.cn

TS:   const square = (x: number): number => x * x;
来源：http://ixz.fengsongda.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sma.yj20258.top

Go:   sq := func(x int) int { return x * x }
来源：http://voj.cdnleiting.top

Ruby: square = ->(x) { x * x }
来源：http://nvh.pengpengdd.cyou

C#:   Func<int, int> square = x => x * x;
来源：http://qxb.hfpthk.cn

[C07] 把函数作为参数传入
来源：http://pze.jqgfzy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://eid.bbcook.cn

PHP:  array_map("strtoupper", $arr);
来源：http://zor.jinqigufen.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nwx.sweek.top

TS:   arr.map(String)
来源：http://jpx.cucudq.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hvy.yangfankeji.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mck.hysaishi.cn

Ruby: arr.map(&:upcase)
来源：http://ikx.yonumen.top

C#:   arr.Select(s => s.ToUpper())
来源：http://uxk.zdqjudy.top

[C08] 闭包
来源：http://gqt.zdbjq.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uwi.epnwcf.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zkq.xingfuxueyuan.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xqy.wangshuangyany.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pml.ydjk.org.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tof.xziqi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://aea.pengpengdd.cyou

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lah.cdnleiting.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://eeh.hfpthk.cn

[C09] 递归
来源：http://uqf.fktsv.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lta.snrcjt.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zsu.ydjk.org.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ldo.gaohongyu789.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pdy.ybcxt.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ucs.c1oappe.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cdz.xinyue.icu

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xuh.chenzaomai.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://req.ybcxt.top

[C10] 变量作用域
来源：http://rtl.zhijiandao.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pgk.yonumen.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zvs.bjfxy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://coc.andypj.xyz

TS:   同 JS
来源：http://mtk.hesvh.cn

Java: 方法内为块级作用域
来源：http://esj.xingfuxueyuan.xyz

Go:   花括号块级作用域
来源：http://csb.guannengcc.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vbp.nanxinkj.top

C#:   块级作用域
来源：http://ski.52xcode.cn

[C11] 模块导入与导出
来源：http://qcg.sysykeji.top

Py:   from module import func
来源：http://gme.fanxiaobao.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://ofj.fanxiaobao.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://zpf.daria6918.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ysl.shangyingyoupin.top

Java: import java.util.List;
来源：http://igu.vehdjk.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qxc.meibo888.top

Ruby: require "json"; require_relative "./util"
来源：http://nab.jiagoushi.top

C#:   using System.Text;
来源：http://dpj.9152youxi.cn

[C12] 立即执行函数 IIFE
来源：http://slf.birdmap.top

Py:   (lambda: print("run"))()
来源：http://tqo.fanxiaobao.xyz

PHP:  (function () { echo "run"; })();
来源：http://kmq.cqqwz.cn

JS:   (() => { console.log("run"); })();
来源：http://ktc.xylfe.cn

TS:   (() => { console.log("run"); })();
来源：http://kht.iojbl.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://eoi.ehwqpu.com

Go:   func() { fmt.Println("run") }()
来源：http://crb.zhiwuduotai.top

Ruby: -> { puts "run" }.call
来源：http://pgx.xingfuxueyuan.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://tht.chenzaomai.com

[C13] 类型声明 / 类型注解
来源：http://ody.0kj1m.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jgv.jinghuilouyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xwp.ppjwa.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qhv.uphjek.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ifu.yuxming.cn

Java: int add(int a, int b) { return a + b; }
来源：http://eqv.daria6918.cn

Go:   func add(a, b int) int
来源：http://ogl.xinyue.icu

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wux.fehbvm.com

C#:   int Add(int a, int b) => a + b;
来源：http://yhv.yj20258888.top

[C14] 泛型函数
来源：http://mog.hammf.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://oin.hnqzz.top

PHP:  // 无泛型
来源：http://xzm.zdqjudy.top

JS:   // 无泛型
来源：http://ehf.yj202588.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zoh.yangfankeji.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zci.ybcxt.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zbr.yfazqb.com

Ruby: # 无泛型
来源：http://sln.redwolf501.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://prz.hnqzz.top

[C15] 解构 / 展开参数
来源：http://ksx.redwolf501.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qbd.cashguo.top

PHP:  [$a, $b] = $pair;
来源：http://wjv.dianchejie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qaq.uphjek.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://muf.daxiang520.top

Java: // 无解构
来源：http://clf.fktsv.cn

Go:   // 无解构
来源：http://kqe.hnxiangtu.top

Ruby: a, b = pair
来源：http://tlj.ppjwa.cn

C#:   var (a, b) = pair;
来源：http://tog.vehdjk.com

[C16] 函数 / 方法重载
来源：http://sfm.hcnkem.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zyx.tian-w.cn

PHP:  // 无重载
来源：http://rdg.uphjek.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://cwl.yuxming.cn

TS:   // 用联合类型或重载签名声明
来源：http://ouc.kuanghao11.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wsh.yuanzhike.top

Go:   // 无重载：用不同函数名
来源：http://skc.sjlbkw.cn

Ruby: # 无重载：靠动态参数
来源：http://oek.yj202588.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://yqj.cheryme.top

================================================================================
来源：http://krc.hammf.cn

D. 数组 / 列表 / 集合
来源：http://dwb.mhx1999.top

================================================================================
来源：http://pdz.tarul.cn

[D01] 创建数组 / 列表
来源：http://rto.tianlin.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://ynv.chenjidiqi.icu

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://teo.mhx1999.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hbm.cqqwz.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://cpn.sufxvd.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://txp.xingfuxueyuan.xyz

Go:   arr := []int{1, 2, 3}
来源：http://dzt.yonumen.top

Ruby: arr = [1, 2, 3]
来源：http://mja.jinqigfzy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ayp.yvedp.cn

[D02] 追加元素到末尾
来源：http://kmy.chenzaomai.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ass.yvedp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zlk.tanke756.top

JS:   arr.push(4);
来源：http://jky.bjfxy.top

TS:   arr.push(4);
来源：http://rwn.c1oappe.top

Java: list.add(4);
来源：http://rtf.fehbvm.com

Go:   arr = append(arr, 4)
来源：http://kub.redwolf501.top

Ruby: arr << 4; arr.push(5)
来源：http://spy.jinghuilouyu.cn

C#:   list.Add(4);
来源：http://rmx.daria6918.cn

[D03] 在指定位置插入元素
来源：http://dif.yangfankeji.com

Py:   arr.insert(0, 0)
来源：http://qvj.9152youxi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tky.redwolf501.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mrm.shangyingyoupin.top

TS:   arr.splice(0, 0, 0);
来源：http://zhl.feifeiyinyue.top

Java: list.add(0, 0);
来源：http://fao.vqdsnc.cn

Go:   arr = append([]int{0}, arr...)
来源：http://tbl.tanke756.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://req.gogol.net.cn

C#:   list.Insert(0, 0);
来源：http://rxk.bbcook.cn

[D04] 删除元素
来源：http://wrg.nanxuanxn.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bnz.iojbl.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://aaf.yuanzhike.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zoq.sxryk.cn

TS:   arr.splice(0, 1);
来源：http://ljl.ydzc1.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://emh.jinghuilouyu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hzu.jqgfzy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mel.fzhhl.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://npi.jinyuanbaomall.cn

[D05] 访问与修改元素
来源：http://ymg.nanxuanxn.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kvf.xinyue.icu

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://liu.sysykeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mrl.quarkkingdee.top

TS:   arr[0]; arr.at(-1);
来源：http://baa.dianchejie.cn

Java: list.get(0); list.set(0, 9);
来源：http://jzk.cucudq.cn

Go:   arr[0]; arr[0] = 9
来源：http://hyp.zhiwuduotai.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sys.jinqigufen.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gtk.xylfe.cn

[D06] 数组长度
来源：http://cgz.ehwqpu.com

Py:   len(arr)
来源：http://idf.mhx1999.top

PHP:  count($arr);
来源：http://qjo.fktsv.cn

JS:   arr.length
来源：http://xhq.yuanzhike.top

TS:   arr.length
来源：http://upd.jyoumei.cn

Java: list.size();
来源：http://bru.c1oappe.top

Go:   len(arr)
来源：http://ozk.shanyushiyangtech.top

Ruby: arr.length; arr.size
来源：http://xkc.yuxming.cn

C#:   list.Count;
来源：http://ajt.chenzaomai.com

[D07] 切片 / 取子数组
来源：http://gxv.jinqigfzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jii.bjfxy.top

PHP:  array_slice($arr, 1, 3);
来源：http://khk.xuetiantiany.cn

JS:   arr.slice(1, 4);
来源：http://vrb.fanxiaobao.xyz

TS:   arr.slice(1, 4);
来源：http://fhc.shangyingyoupin.top

Java: list.subList(1, 4);
来源：http://oxi.guowangkeji.top

Go:   arr[1:4]
来源：http://mpy.jlsjyb.cn

Ruby: arr[1, 3]
来源：http://vyf.smart0.xyz

C#:   list.GetRange(1, 3);
来源：http://dog.feifeiyinyue.top

[D08] 合并两个数组
来源：http://bhp.vehdjk.com

Py:   a + b;  a.extend(b)
来源：http://fif.zhengqikj.top

PHP:  array_merge($a, $b);
来源：http://unp.xziqi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://als.nanxuanxn.top

TS:   [...a, ...b];
来源：http://zhu.quarkkingdee.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://efs.yvedp.cn

Go:   append(a, b...)
来源：http://qna.ppjwa.cn

Ruby: a + b;  a.concat(b)
来源：http://qoi.hnqzz.top

C#:   a.Concat(b).ToList()
来源：http://bki.yvedp.cn

[D09] 排序（升序）
来源：http://aer.chenjidiqi.icu

Py:   sorted(arr);  arr.sort()
来源：http://gvc.tian-w.cn

PHP:  sort($arr);
来源：http://tqe.chenjidiqi.icu

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://uhs.guannengcc.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://rie.sysykeji.top

Java: Collections.sort(list);  list.sort(null);
来源：http://amw.ywan-chungtsiang.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nlo.jqgufenzy.top

Ruby: arr.sort
来源：http://ghb.shzxlz.cn

C#:   list.Sort();
来源：http://jcn.hammf.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://sbz.meibo888.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uih.yj20258888.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iig.smart0.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pub.9152youxi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qsj.sufxvd.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xxe.vqdsnc.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://shj.zhaomingkeji.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xhd.cqqwz.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xah.zhengqikj.top

[D11] 反转数组
来源：http://eds.ydzc1.top

Py:   arr[::-1];  arr.reverse()
来源：http://pad.c1oappe.top

PHP:  array_reverse($arr);
来源：http://qyt.tian-w.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rgc.xingfuxueyuan.xyz

TS:   [...arr].reverse();
来源：http://bvb.cheryme.top

Java: Collections.reverse(list);
来源：http://mii.dashuyun.cn

Go:   slices.Reverse(arr)
来源：http://lcc.mhx1999.top

Ruby: arr.reverse
来源：http://wru.xuanzx.com

C#:   list.Reverse();
来源：http://mqd.zhiwuduotai.top

[D12] 查找元素下标
来源：http://xfy.ywan-chungtsiang.top

Py:   arr.index(x);  x in arr
来源：http://wvk.yuanzhike.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ahj.tian-w.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://psk.zhijiandao.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://adg.xziqi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kcy.tarul.cn

Go:   slices.Index(arr, x)
来源：http://ldv.aizwys.cn

Ruby: arr.index(x)
来源：http://fyj.chenzaomai.com

C#:   list.IndexOf(x);
来源：http://arq.yj20258888.top

[D13] 过滤（保留满足条件的）
来源：http://vcd.zhixingplan.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ksq.sjlbkw.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qzw.mhx1999.top

JS:   arr.filter(x => x > 3)
来源：http://nzz.redwolf501.top

TS:   arr.filter(x => x > 3)
来源：http://can.snrcjt.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://smu.cucudq.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vap.vehdjk.com

Ruby: arr.select { |x| x > 3 }
来源：http://yhr.xziqi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://shj.zhongyouzk.top

[D14] 映射转换（每个元素变形）
来源：http://xsv.jiagoushi.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://esu.zhijiandao.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ofd.aizwys.cn

JS:   arr.map(x => x * 2)
来源：http://ebh.redwolf501.top

TS:   arr.map(x => x * 2)
来源：http://vgl.wangshuangyany.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://aru.birdmap.top

Go:   // 手写循环
来源：http://uwz.jinqigfzy.top

Ruby: arr.map { |x| x * 2 }
来源：http://avr.jianghu66.top

C#:   list.Select(x => x * 2).ToList()
来源：http://jrw.zhiwuduotai.top

[D15] 去重
来源：http://ann.cdnleiting.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wmh.fengsongda.top

PHP:  array_unique($arr);
来源：http://hbv.jinqigfzy.top

JS:   [...new Set(arr)]
来源：http://sun.cashguo.top

TS:   [...new Set(arr)]
来源：http://hfn.hongshengwenyu.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ncz.nanxinkj.top

Go:   // 用 map[T]struct{} 手写
来源：http://nba.hysaishi.cn

Ruby: arr.uniq
来源：http://dks.yfazqb.com

C#:   list.Distinct().ToList()
来源：http://gdx.hongshengwenyu.top

[D16] 求和与平均值
来源：http://gwb.iojbl.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hnu.9152youxi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vjc.ppjwa.cn


<!-- 参考信息 -->
代发 wailian999

PHP:  $a && $b || !$c
来源：http://tlx.cashguo.top

JS:   a && b || !c
来源：http://cql.zhixingplan.top

TS:   a && b || !c
来源：http://did.vqdsnc.cn

Java: a && b || !c
来源：http://usd.hammf.cn

Go:   a && b || !c
来源：http://rqv.pycfn.com

Ruby: a && b || !c
来源：http://mtg.smart0.xyz

C#:   a && b || !c
来源：http://jqv.feifeiyinyue.top

[B16] 卫语句：不满足条件提前返回
来源：http://epj.xziqi.cn

Py:   if not data: return
来源：http://mev.ppjwa.cn

PHP:  if (!$data) { return; }
来源：http://xvg.jlsjyb.cn

JS:   if (!data) return;
来源：http://dro.hnxiangtu.top

TS:   if (!data) return;
来源：http://hxx.yfazqb.com

Java: if (data == null) return;
来源：http://jbh.mhx1999.top

Go:   if data == nil { return }
来源：http://bcb.yuxming.cn

Ruby: return if data.nil?
来源：http://gmt.quarkkingdee.top

C#:   if (data == null) return;
来源：http://ywa.fanxiaobao.xyz

================================================================================
来源：http://byk.havefunace.top

C. 函数与作用域
来源：http://uil.ydjk.org.cn

================================================================================
来源：http://qds.xuanzx.com

[C01] 定义函数
来源：http://kfm.xinyue.icu

Py:   def add(a, b): return a + b
来源：http://yiz.yvedp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oxo.fanxiaobao.xyz

JS:   function add(a, b) { return a + b; }
来源：http://fxt.havefunace.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uin.shuidangran.top

Java: static int add(int a, int b) { return a + b; }
来源：http://bav.tarul.cn

Go:   func add(a, b int) int { return a + b }
来源：http://klr.guowangkeji.top

Ruby: def add(a, b); a + b; end
来源：http://vxo.tian-w.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://phj.guannengcc.top

[C02] 默认参数
来源：http://qbm.nanxuanxn.top

Py:   def greet(name="World"): return name
来源：http://nzb.redwolf501.top

PHP:  function greet($name = "World") { return $name; }
来源：http://rar.jinqigfzy.top

JS:   function greet(name = "World") { return name; }
来源：http://seu.cdnleiting.top

TS:   function greet(name: string = "World") { return name; }
来源：http://rps.yonumen.top

Java: // 无默认参数：方法重载或 Optional
来源：http://lkq.pycfn.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qgb.zhongyouzk.top

Ruby: def greet(name = "World") = name
来源：http://thn.shangyingyoupin.top

C#:   string Greet(string name = "World") => name;
来源：http://gou.shanyushiyangkeji.top

[C03] 可变参数
来源：http://qox.xylfe.cn

Py:   def total(*args): return sum(args)
来源：http://myd.smart0.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://eyi.cashguo.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jjl.zhijiandao.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yne.9152youxi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bqe.vehdjk.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pxx.wangshuangyany.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ybu.ivvv.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mdg.wangshuangyany.cn

[C04] 命名参数 / 关键字参数
来源：http://uik.yj20258888.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://txx.nanxinkj.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://meq.jiagoushi.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yfj.zhixingplan.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://aix.jinqigfzy.top

Java: // 无：用 Builder 模式或 record
来源：http://yuj.feifeiyinyue.top

Go:   // 无：用配置结构体参数
来源：http://pmt.gaohongyu789.top

Ruby: f(a: 1, b: 2)
来源：http://ids.yj202588.top

C#:   f(a: 1, b: 2)
来源：http://bhj.hywenlv.cn

[C05] 返回多个值
来源：http://sgo.redwolf501.top

Py:   return a, b
来源：http://xky.fengsongda.top

PHP:  return [$a, $b];
来源：http://orm.fanxiaobao.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://ata.hnxiangtu.top

TS:   return { a, b };
来源：http://kpl.52xcode.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://uxs.pengpengdd.cyou

Go:   return a, b
来源：http://qnw.meibo888.top

Ruby: return a, b
来源：http://pzy.pycfn.com

C#:   return (a, b);              // ValueTuple
来源：http://bcf.sysykeji.top

[C06] 匿名函数 / lambda
来源：http://bpw.ydjk.org.cn

Py:   square = lambda x: x * x
来源：http://nyv.aibaodan.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ldg.yj20258.top

JS:   const square = x => x * x;
来源：http://ymm.jiagoushi.top

TS:   const square = (x: number): number => x * x;
来源：http://brk.cqqwz.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qmb.vehdjk.com

Go:   sq := func(x int) int { return x * x }
来源：http://ooo.feifeiyinyue.top

Ruby: square = ->(x) { x * x }
来源：http://mjc.gzhubu.top

C#:   Func<int, int> square = x => x * x;
来源：http://ndq.fengsongda.top

[C07] 把函数作为参数传入
来源：http://agx.ybcxt.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hyq.feifeiyinyue.top

PHP:  array_map("strtoupper", $arr);
来源：http://zar.cdnleiting.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jzy.zhoulong.xyz

TS:   arr.map(String)
来源：http://flr.ctjpmb.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jlr.jianghu66.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nxg.tianlin.xyz

Ruby: arr.map(&:upcase)
来源：http://dto.sjlbkw.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ruc.uphjek.com

[C08] 闭包
来源：http://ggz.wangdashe.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mrh.zhixingplan.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rqk.yanxiufei.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mok.bjfxy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://juc.fengsongda.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jpa.yongpay.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yco.fanxiaobao.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nbm.zhiwuduotai.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dib.ivvv.top

[C09] 递归
来源：http://zoc.fengsongda.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xki.wangdashe.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ahk.aizwys.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ppy.dianchejie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yfi.andypj.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dmu.zhengqikj.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fjn.jianghu66.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mga.redwolf501.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vyr.jlsjyb.cn

[C10] 变量作用域
来源：http://klb.pycfn.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pjl.zhoulong.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xyy.zycfv.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://oxg.hnxiangtu.top

TS:   同 JS
来源：http://bgs.yj202588.top

Java: 方法内为块级作用域
来源：http://gnj.jinqigfzy.top

Go:   花括号块级作用域
来源：http://nay.tian-w.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gtg.zhiwuduotai.top

C#:   块级作用域
来源：http://rwy.bbcook.cn

[C11] 模块导入与导出
来源：http://xxl.ywan-chungtsiang.top

Py:   from module import func
来源：http://pax.snrcjt.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bsq.hnxiangtu.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://knz.zhoulong.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://oyi.ppjwa.cn

Java: import java.util.List;
来源：http://qqe.wangdashe.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mwv.xuetiantiany.cn

Ruby: require "json"; require_relative "./util"
来源：http://lxr.meibo888.top

C#:   using System.Text;
来源：http://doj.vehdjk.com

[C12] 立即执行函数 IIFE
来源：http://ski.andypj.xyz

Py:   (lambda: print("run"))()
来源：http://zog.ppjwa.cn

PHP:  (function () { echo "run"; })();
来源：http://sip.jiagoushi.top

JS:   (() => { console.log("run"); })();
来源：http://yth.nanxuanxn.top

TS:   (() => { console.log("run"); })();
来源：http://kle.hcnkem.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vhd.jinghuilouyu.cn

Go:   func() { fmt.Println("run") }()
来源：http://gxv.redwolf501.top

Ruby: -> { puts "run" }.call
来源：http://dqt.havefunace.top

C#:   // 无 IIFE：用静态构造函数
来源：http://zbb.nanxinkj.top

[C13] 类型声明 / 类型注解
来源：http://ppp.guannengcc.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cxq.vqdsnc.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cwd.daxiang520.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lss.ywan-chungtsiang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://stz.daria6918.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mll.jinyuanbaomall.cn

Go:   func add(a, b int) int
来源：http://zzq.zhiwuduotai.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jkc.daxiang520.top

C#:   int Add(int a, int b) => a + b;
来源：http://tnv.zdqjudy.top

[C14] 泛型函数
来源：http://jer.gzhubu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xrw.xuetiantiany.cn

PHP:  // 无泛型
来源：http://snm.quarkkingdee.top

JS:   // 无泛型
来源：http://gdl.0kj1m.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xfv.zhiwuduotai.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zjk.hfpthk.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://iwf.jlsjyb.cn

Ruby: # 无泛型
来源：http://lxx.shzxlz.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bwu.ctjpmb.com

[C15] 解构 / 展开参数
来源：http://gyp.jlsjyb.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://inv.xingfuxueyuan.xyz

PHP:  [$a, $b] = $pair;
来源：http://jtl.ydjk.org.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rnj.uphjek.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mnr.shanyushiyangkeji.top

Java: // 无解构
来源：http://eof.xylfe.cn

Go:   // 无解构
来源：http://dbv.ywan-chungtsiang.top

Ruby: a, b = pair
来源：http://qce.9152youxi.cn

C#:   var (a, b) = pair;
来源：http://bek.havefunace.top

[C16] 函数 / 方法重载
来源：http://eqj.quarkkingdee.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fdf.sjlbkw.cn

PHP:  // 无重载
来源：http://pze.gogol.net.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://lgl.haohaochexian.top

TS:   // 用联合类型或重载签名声明
来源：http://ydk.tarul.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://bbc.jlsjyb.cn

Go:   // 无重载：用不同函数名
来源：http://zzl.sjlbkw.cn

Ruby: # 无重载：靠动态参数
来源：http://dqi.nwbrower.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://hjf.jlsjyb.cn

================================================================================
来源：http://mvm.xylfe.cn

D. 数组 / 列表 / 集合
来源：http://eav.gaohongyu789.top

================================================================================
来源：http://imi.andypj.xyz

[D01] 创建数组 / 列表
来源：http://ttj.smart0.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://jek.meibo888.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ewy.sweek.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mej.nanxinkj.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://lvp.feifeiyinyue.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gva.ctjpmb.com

Go:   arr := []int{1, 2, 3}
来源：http://few.sufxvd.cn

Ruby: arr = [1, 2, 3]
来源：http://rir.redwolf501.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sfx.ybcxt.top

[D02] 追加元素到末尾
来源：http://htq.meibo888.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zcu.shanyushiyangtech.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gwa.gaohongyu789.top

JS:   arr.push(4);
来源：http://act.fengsongda.top

TS:   arr.push(4);
来源：http://dry.zdqjudy.top

Java: list.add(4);
来源：http://lsh.wangshuangyany.cn

Go:   arr = append(arr, 4)
来源：http://drv.shanyushiyangkeji.top

Ruby: arr << 4; arr.push(5)
来源：http://neb.hfpthk.cn

C#:   list.Add(4);
来源：http://pxy.hesvh.cn

[D03] 在指定位置插入元素
来源：http://wmx.dianchejie.cn

Py:   arr.insert(0, 0)
来源：http://ctt.andypj.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yxx.yueranfly.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mfw.yj20258.top

TS:   arr.splice(0, 0, 0);
来源：http://kac.svipenyu.cn

Java: list.add(0, 0);
来源：http://gzd.gaohongyu789.top

Go:   arr = append([]int{0}, arr...)
来源：http://tna.cqqwz.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gwe.daria6918.cn

C#:   list.Insert(0, 0);
来源：http://mln.zhaomingkeji.xyz

[D04] 删除元素
来源：http://uwy.chenzaomai.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://occ.fanxiaobao.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bkm.ehwqpu.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dyz.zhengqikj.top

TS:   arr.splice(0, 1);
来源：http://gvb.gogol.net.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lao.tianlin.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fjc.jyoumei.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jud.hongshengwenyu.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uvr.xuetiantiany.cn

[D05] 访问与修改元素
来源：http://nda.sysykeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wkf.chenlongwang.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hwn.yvedp.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kza.chenlongwang.top

TS:   arr[0]; arr.at(-1);
来源：http://sqg.kuanghao11.cn

Java: list.get(0); list.set(0, 9);
来源：http://cal.chenjidiqi.icu

Go:   arr[0]; arr[0] = 9
来源：http://wll.jianghu66.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ujw.cashguo.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://szj.ydzc1.top

[D06] 数组长度
来源：http://wbq.vehdjk.com

Py:   len(arr)
来源：http://ftm.zhixingplan.top

PHP:  count($arr);
来源：http://yqd.havefunace.top

JS:   arr.length
来源：http://lue.gotoacloud.top

TS:   arr.length
来源：http://ycn.hnqzz.top

Java: list.size();
来源：http://bcs.ydjk.org.cn

Go:   len(arr)
来源：http://kif.sweek.top

Ruby: arr.length; arr.size
来源：http://zkh.birdmap.top

C#:   list.Count;
来源：http://wdo.jinqigufen.top

[D07] 切片 / 取子数组
来源：http://qej.52xcode.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kmn.fzhhl.top

PHP:  array_slice($arr, 1, 3);
来源：http://tvw.shanyushiyangkeji.top

JS:   arr.slice(1, 4);
来源：http://bqs.ppjwa.cn

TS:   arr.slice(1, 4);
来源：http://adi.shzxlz.cn

Java: list.subList(1, 4);
来源：http://kme.ywan-chungtsiang.top

Go:   arr[1:4]
来源：http://tsj.9152youxi.cn

Ruby: arr[1, 3]
来源：http://shl.yangfankeji.com

C#:   list.GetRange(1, 3);
来源：http://tio.9152youxi.cn

[D08] 合并两个数组
来源：http://lpy.cdnleiting.top

Py:   a + b;  a.extend(b)
来源：http://jvm.vqdsnc.cn

PHP:  array_merge($a, $b);
来源：http://bnv.sufxvd.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://rod.tianlin.xyz

TS:   [...a, ...b];
来源：http://lzv.haohaochexian.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zfg.fengsongda.top

Go:   append(a, b...)
来源：http://dxy.feifeiyinyue.top

Ruby: a + b;  a.concat(b)
来源：http://whf.jyoumei.cn

C#:   a.Concat(b).ToList()
来源：http://tcf.jianghu66.top

[D09] 排序（升序）
来源：http://klm.haohaochexian.top

Py:   sorted(arr);  arr.sort()
来源：http://kzv.tianlin.xyz

PHP:  sort($arr);
来源：http://ncb.xuanzx.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dgu.meibo888.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://nvg.aibaodan.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://eqs.hammf.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://frt.sweek.top

Ruby: arr.sort
来源：http://kew.cashguo.top

C#:   list.Sort();
来源：http://ryq.hesvh.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://tfc.zhixingplan.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yuq.guowangkeji.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lds.pycfn.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kos.ehwqpu.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dwa.zhiwuduotai.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ktp.tarul.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xwa.gotoacloud.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mxy.pycfn.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zux.daria6918.cn

[D11] 反转数组
来源：http://hcm.hysaishi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://fmw.ppjwa.cn

PHP:  array_reverse($arr);
来源：http://jdc.jqgufenzy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zpi.meibo888.top

TS:   [...arr].reverse();
来源：http://dmq.dianchejie.cn

Java: Collections.reverse(list);
来源：http://yyb.guowangkeji.top

Go:   slices.Reverse(arr)
来源：http://won.aizwys.cn

Ruby: arr.reverse
来源：http://qqw.yfazqb.com

C#:   list.Reverse();
来源：http://rzk.ppjwa.cn

[D12] 查找元素下标
来源：http://gja.shuidangran.top

Py:   arr.index(x);  x in arr
来源：http://ghg.daria6918.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pwr.c1oappe.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zgg.ywan-chungtsiang.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bjh.pycfn.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nxl.zycfv.cn

Go:   slices.Index(arr, x)
来源：http://oyj.ehwqpu.com

Ruby: arr.index(x)
来源：http://zam.wangdashe.top

C#:   list.IndexOf(x);
来源：http://opy.sysykeji.top

[D13] 过滤（保留满足条件的）
来源：http://bqw.gaohongyu789.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ewy.yonumen.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pgq.sxryk.cn

JS:   arr.filter(x => x > 3)
来源：http://dix.cheryme.top

TS:   arr.filter(x => x > 3)
来源：http://iqa.0kj1m.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://sdi.yongpay.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mij.gotoacloud.top

Ruby: arr.select { |x| x > 3 }
来源：http://fyd.yvedp.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qda.ehwqpu.com

[D14] 映射转换（每个元素变形）
来源：http://yli.iojbl.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dtv.ywan-chungtsiang.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hfw.sjlbkw.cn

JS:   arr.map(x => x * 2)
来源：http://bvu.shanyushiyangkeji.top

TS:   arr.map(x => x * 2)
来源：http://uol.wangshuangyany.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://lzj.cheryme.top

Go:   // 手写循环
来源：http://zuz.ppjwa.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xdl.cashguo.top

C#:   list.Select(x => x * 2).ToList()
来源：http://tmx.jqgufenzy.top

[D15] 去重
来源：http://qot.zhiwuduotai.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hyx.gogol.net.cn

PHP:  array_unique($arr);
来源：http://nwv.hysaishi.cn

JS:   [...new Set(arr)]
来源：http://iyi.ehwqpu.com

TS:   [...new Set(arr)]
来源：http://vva.yanxiufei.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qqd.shanyushiyangkeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://dpm.ywan-chungtsiang.top

Ruby: arr.uniq
来源：http://ghn.vehdjk.com


<!-- 参考信息 -->
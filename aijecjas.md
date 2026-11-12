代发 wailian999

Py:   def add(a, b): return a + b
来源：http://glw.cqqwz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dxu.shanyushiyangkeji.top

JS:   function add(a, b) { return a + b; }
来源：http://ice.xinyue.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nok.gotoacloud.top

Java: static int add(int a, int b) { return a + b; }
来源：http://rqq.xylfe.cn

Go:   func add(a, b int) int { return a + b }
来源：http://sev.jqgufenzy.top

Ruby: def add(a, b); a + b; end
来源：http://vdq.sweek.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pgm.jinqigufen.top

[C02] 默认参数
来源：http://wjp.uphjek.com

Py:   def greet(name="World"): return name
来源：http://ice.jinyuanbaomall.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://sqc.yonumen.top

JS:   function greet(name = "World") { return name; }
来源：http://ije.feifeiyinyue.top

TS:   function greet(name: string = "World") { return name; }
来源：http://zja.shanyushiyangtech.top

Java: // 无默认参数：方法重载或 Optional
来源：http://loo.9152youxi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dml.jinqigufen.top

Ruby: def greet(name = "World") = name
来源：http://nfl.tian-w.cn

C#:   string Greet(string name = "World") => name;
来源：http://syu.nwbrower.top

[C03] 可变参数
来源：http://mrz.sufxvd.cn

Py:   def total(*args): return sum(args)
来源：http://usa.hnqzz.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cba.quarkkingdee.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://raq.bbcook.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wjf.fengsongda.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vrk.yfazqb.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vda.feifeiyinyue.top

Ruby: def total(*nums); nums.sum; end
来源：http://ovo.ivvv.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vny.fehbvm.com

[C04] 命名参数 / 关键字参数
来源：http://tjh.daria6918.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xau.nanxinkj.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jlh.hammf.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ecq.meibo888.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cac.shuidangran.top

Java: // 无：用 Builder 模式或 record
来源：http://mol.snrcjt.cn

Go:   // 无：用配置结构体参数
来源：http://xde.gaohongyu789.top

Ruby: f(a: 1, b: 2)
来源：http://fbg.cdnleiting.top

C#:   f(a: 1, b: 2)
来源：http://akz.hysaishi.cn

[C05] 返回多个值
来源：http://bdg.316326.xyz

Py:   return a, b
来源：http://cma.fktsv.cn

PHP:  return [$a, $b];
来源：http://vai.jqgfzy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ogt.xuetiantiany.cn

TS:   return { a, b };
来源：http://qio.ydjk.org.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tyl.feifeiyinyue.top

Go:   return a, b
来源：http://whk.redwolf501.top

Ruby: return a, b
来源：http://xxx.snrcjt.cn

C#:   return (a, b);              // ValueTuple
来源：http://gku.gzhubu.top

[C06] 匿名函数 / lambda
来源：http://eab.shuidangran.top

Py:   square = lambda x: x * x
来源：http://rix.9152youxi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://asj.hnqzz.top

JS:   const square = x => x * x;
来源：http://mlv.nanxinkj.top

TS:   const square = (x: number): number => x * x;
来源：http://cot.nwbrower.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kcu.yonumen.top

Go:   sq := func(x int) int { return x * x }
来源：http://krs.cdnleiting.top

Ruby: square = ->(x) { x * x }
来源：http://hah.feifeiyinyue.top

C#:   Func<int, int> square = x => x * x;
来源：http://wuj.shanyushiyangtech.top

[C07] 把函数作为参数传入
来源：http://edb.hywenlv.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hug.dianchejie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://iov.ybcxt.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wck.yanxiufei.cn

TS:   arr.map(String)
来源：http://shj.ivvv.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://obs.bjfxy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fzc.zdqjudy.top

Ruby: arr.map(&:upcase)
来源：http://nvm.vehdjk.com

C#:   arr.Select(s => s.ToUpper())
来源：http://xxd.zhixingplan.top

[C08] 闭包
来源：http://xpn.uphjek.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://boe.nanxinkj.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kys.hcnkem.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bfl.shuidangran.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vuo.xuanzx.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yuq.zhixingplan.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tbo.0kj1m.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ihb.ppjwa.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wnf.xingfuxueyuan.xyz

[C09] 递归
来源：http://xld.gotoacloud.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://puv.chenzaomai.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xmm.nanxuanxn.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ost.yongpay.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dyt.fehbvm.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tko.zdqjudy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://aur.svipenyu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yob.aibaodan.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://svn.hywenlv.cn

[C10] 变量作用域
来源：http://hnh.wangdashe.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://twf.mhx1999.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gru.vehdjk.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mdz.wangshuangyany.cn

TS:   同 JS
来源：http://deo.daria6918.cn

Java: 方法内为块级作用域
来源：http://vop.cucudq.cn

Go:   花括号块级作用域
来源：http://fca.zdqjudy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nxd.kuanghao11.cn

C#:   块级作用域
来源：http://spe.ywan-chungtsiang.top

[C11] 模块导入与导出
来源：http://nvf.sxryk.cn

Py:   from module import func
来源：http://jrf.ehwqpu.com

PHP:  require "file.php";  或 use App\Service;
来源：http://znu.zdqjudy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ipu.zhixingplan.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mpd.yuxming.cn

Java: import java.util.List;
来源：http://dny.jinghuilouyu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lfx.ivvv.top

Ruby: require "json"; require_relative "./util"
来源：http://pqk.xinyue.icu

C#:   using System.Text;
来源：http://zvc.bjfxy.top

[C12] 立即执行函数 IIFE
来源：http://czk.sjlbkw.cn

Py:   (lambda: print("run"))()
来源：http://fga.feifeiyinyue.top

PHP:  (function () { echo "run"; })();
来源：http://twl.ydjk.org.cn

JS:   (() => { console.log("run"); })();
来源：http://fvj.tarul.cn

TS:   (() => { console.log("run"); })();
来源：http://vde.birdmap.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dio.pengpengdd.cyou

Go:   func() { fmt.Println("run") }()
来源：http://cgd.gogol.net.cn

Ruby: -> { puts "run" }.call
来源：http://kfk.sysykeji.top

C#:   // 无 IIFE：用静态构造函数
来源：http://spf.xuanzx.com

[C13] 类型声明 / 类型注解
来源：http://ccl.xziqi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zzn.jinghuilouyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dkp.hnxiangtu.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ell.hnqzz.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://eaz.guowangkeji.top

Java: int add(int a, int b) { return a + b; }
来源：http://bye.kuanghao11.cn

Go:   func add(a, b int) int
来源：http://ehj.yuxming.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qxj.0kj1m.cn

C#:   int Add(int a, int b) => a + b;
来源：http://oiv.jinyuanbaomall.cn

[C14] 泛型函数
来源：http://szx.hesvh.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lbi.gzhubu.top

PHP:  // 无泛型
来源：http://zah.sufxvd.cn

JS:   // 无泛型
来源：http://drp.feifeiyinyue.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ebq.yuxming.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yyj.gotoacloud.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dhb.c1oappe.top

Ruby: # 无泛型
来源：http://jiv.shanyushiyangtech.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cif.sysykeji.top

[C15] 解构 / 展开参数
来源：http://siz.yj20258888.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bgb.jyoumei.cn

PHP:  [$a, $b] = $pair;
来源：http://fgf.gaohongyu789.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lao.meibo888.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pqj.cdnleiting.top

Java: // 无解构
来源：http://ffl.sweek.top

Go:   // 无解构
来源：http://emd.jianghu66.top

Ruby: a, b = pair
来源：http://jwf.fktsv.cn

C#:   var (a, b) = pair;
来源：http://esw.tianlin.xyz

[C16] 函数 / 方法重载
来源：http://lok.vehdjk.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://esc.shuidangran.top

PHP:  // 无重载
来源：http://jxq.316326.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://wag.cucudq.cn

TS:   // 用联合类型或重载签名声明
来源：http://ngl.ctjpmb.com

Java: void f(int a) {}  void f(String a) {}
来源：http://ziv.chenlongwang.top

Go:   // 无重载：用不同函数名
来源：http://ajf.zhiwuduotai.top

Ruby: # 无重载：靠动态参数
来源：http://qfx.jianghu66.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ivv.cucudq.cn

================================================================================
来源：http://yia.sjlbkw.cn

D. 数组 / 列表 / 集合
来源：http://vxx.hywenlv.cn

================================================================================
来源：http://zto.hnqzz.top

[D01] 创建数组 / 列表
来源：http://odr.zhongyouzk.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://xuw.jiagoushi.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nej.cdnleiting.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blz.shuidangran.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://cjd.jiagoushi.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tlc.xuetiantiany.cn

Go:   arr := []int{1, 2, 3}
来源：http://bka.epnwcf.com

Ruby: arr = [1, 2, 3]
来源：http://ehz.sufxvd.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yzw.52xcode.cn

[D02] 追加元素到末尾
来源：http://dpr.zhiwuduotai.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vnc.jyoumei.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fzm.zhengqikj.top

JS:   arr.push(4);
来源：http://anj.aibaodan.cn

TS:   arr.push(4);
来源：http://sqm.cqqwz.cn

Java: list.add(4);
来源：http://kbg.feifeiyinyue.top

Go:   arr = append(arr, 4)
来源：http://vgm.fengsongda.top

Ruby: arr << 4; arr.push(5)
来源：http://klg.shangyingyoupin.top

C#:   list.Add(4);
来源：http://ora.xingfuxueyuan.xyz

[D03] 在指定位置插入元素
来源：http://oxw.vqdsnc.cn

Py:   arr.insert(0, 0)
来源：http://rkz.andypj.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ybv.gogol.net.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nls.chenzaomai.com

TS:   arr.splice(0, 0, 0);
来源：http://xwf.aizwys.cn

Java: list.add(0, 0);
来源：http://kfs.chenzaomai.com

Go:   arr = append([]int{0}, arr...)
来源：http://rzu.redwolf501.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://acc.ppjwa.cn

C#:   list.Insert(0, 0);
来源：http://sjb.hesvh.cn

[D04] 删除元素
来源：http://iyx.yj20258.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://maq.xziqi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jqd.wangdashe.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://apu.tianlin.xyz

TS:   arr.splice(0, 1);
来源：http://xoo.yfazqb.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://czo.mhx1999.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xny.yuanzhike.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mba.jinghuilouyu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fsr.fengsongda.top

[D05] 访问与修改元素
来源：http://iut.yuanzhike.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ecs.daria6918.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wme.nanxinkj.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ylc.shanyushiyangkeji.top

TS:   arr[0]; arr.at(-1);
来源：http://ygv.hcnkem.com

Java: list.get(0); list.set(0, 9);
来源：http://msg.fehbvm.com

Go:   arr[0]; arr[0] = 9
来源：http://hyu.fanxiaobao.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cjj.hesvh.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gep.9152youxi.cn

[D06] 数组长度
来源：http://xqe.yonumen.top

Py:   len(arr)
来源：http://sit.sxryk.cn

PHP:  count($arr);
来源：http://why.feifeiyinyue.top

JS:   arr.length
来源：http://tcf.tarul.cn

TS:   arr.length
来源：http://wyj.pycfn.com

Java: list.size();
来源：http://ben.iojbl.cn

Go:   len(arr)
来源：http://hgq.fengsongda.top

Ruby: arr.length; arr.size
来源：http://huq.hammf.cn

C#:   list.Count;
来源：http://krt.hammf.cn

[D07] 切片 / 取子数组
来源：http://cqf.dashuyun.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qed.xuetiantiany.cn

PHP:  array_slice($arr, 1, 3);
来源：http://res.xuetiantiany.cn

JS:   arr.slice(1, 4);
来源：http://qsl.zhaomingkeji.xyz

TS:   arr.slice(1, 4);
来源：http://mvs.zycfv.cn

Java: list.subList(1, 4);
来源：http://vrr.ywan-chungtsiang.top

Go:   arr[1:4]
来源：http://sgj.guannengcc.top

Ruby: arr[1, 3]
来源：http://sxh.zhengqikj.top

C#:   list.GetRange(1, 3);
来源：http://abv.daxiang520.top

[D08] 合并两个数组
来源：http://scg.shzxlz.cn

Py:   a + b;  a.extend(b)
来源：http://drq.daria6918.cn

PHP:  array_merge($a, $b);
来源：http://vei.mhx1999.top

JS:   [...a, ...b];  a.concat(b);
来源：http://itg.zdqjudy.top

TS:   [...a, ...b];
来源：http://dqg.sufxvd.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gom.shangyingyoupin.top

Go:   append(a, b...)
来源：http://ume.gogol.net.cn

Ruby: a + b;  a.concat(b)
来源：http://hmq.guowangkeji.top

C#:   a.Concat(b).ToList()
来源：http://fat.yonumen.top

[D09] 排序（升序）
来源：http://yge.fengsongda.top

Py:   sorted(arr);  arr.sort()
来源：http://vkz.jiagoushi.top

PHP:  sort($arr);
来源：http://drm.shangyingyoupin.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sja.vehdjk.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://jer.svipenyu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://uip.birdmap.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://idr.birdmap.top

Ruby: arr.sort
来源：http://afg.ehwqpu.com

C#:   list.Sort();
来源：http://eue.yj20258888.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://bal.cucudq.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uts.hnqzz.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pme.hongshengwenyu.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lrk.zhengqikj.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bic.sjlbkw.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://als.9152youxi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nxq.zhongyouzk.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cob.gzhubu.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ltk.smart0.xyz

[D11] 反转数组
来源：http://zfy.yonumen.top

Py:   arr[::-1];  arr.reverse()
来源：http://hxi.shangyingyoupin.top

PHP:  array_reverse($arr);
来源：http://xgn.jlsjyb.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fww.zhiwuduotai.top

TS:   [...arr].reverse();
来源：http://lsk.yj202588.top

Java: Collections.reverse(list);
来源：http://czq.0kj1m.cn

Go:   slices.Reverse(arr)
来源：http://axw.fktsv.cn

Ruby: arr.reverse
来源：http://tnf.yanxiufei.cn

C#:   list.Reverse();
来源：http://ztr.epnwcf.com

[D12] 查找元素下标
来源：http://hrd.yj20258.top

Py:   arr.index(x);  x in arr
来源：http://xvy.yongpay.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jjj.zhongyouzk.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://udb.shanyushiyangtech.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gzu.uphjek.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ais.hysaishi.cn

Go:   slices.Index(arr, x)
来源：http://tcx.yj20258.top

Ruby: arr.index(x)
来源：http://jbx.chenjidiqi.icu

C#:   list.IndexOf(x);
来源：http://pes.fengsongda.top

[D13] 过滤（保留满足条件的）
来源：http://iyg.hnxiangtu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pye.gotoacloud.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://llw.jinqigufen.top

JS:   arr.filter(x => x > 3)
来源：http://qqt.andypj.xyz

TS:   arr.filter(x => x > 3)
来源：http://unw.zhijiandao.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://khm.vehdjk.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mfx.vqdsnc.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ncb.zhoulong.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://vou.hnxiangtu.top

[D14] 映射转换（每个元素变形）
来源：http://kcv.nwbrower.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gkv.jinqigfzy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wuf.jinghuilouyu.cn

JS:   arr.map(x => x * 2)
来源：http://ncy.jiagoushi.top

TS:   arr.map(x => x * 2)
来源：http://wea.ydzc1.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://fui.haohaochexian.top

Go:   // 手写循环
来源：http://bzd.jlsjyb.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xyg.9152youxi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sdt.xylfe.cn

[D15] 去重
来源：http://ctv.xylfe.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://oio.meibo888.top

PHP:  array_unique($arr);
来源：http://axh.guannengcc.top

JS:   [...new Set(arr)]
来源：http://lcg.aibaodan.cn

TS:   [...new Set(arr)]
来源：http://nqh.316326.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ied.shanyushiyangtech.top

Go:   // 用 map[T]struct{} 手写
来源：http://fkw.hnxiangtu.top

Ruby: arr.uniq
来源：http://gnx.cqqwz.cn

C#:   list.Distinct().ToList()
来源：http://rmh.gotoacloud.top

[D16] 求和与平均值
来源：http://wjc.hammf.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://adz.shangyingyoupin.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zoq.xuetiantiany.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://otp.ctjpmb.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mrd.ctjpmb.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lid.shzxlz.cn

Go:   // 手写循环累加
来源：http://xnr.cqqwz.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://uml.guowangkeji.top

C#:   list.Sum();  list.Average()
来源：http://apf.jiagoushi.top

[D17] 最大值与最小值
来源：http://ojr.zhaomingkeji.xyz

Py:   max(arr);  min(arr)
来源：http://dyu.xingfuxueyuan.xyz

PHP:  max($arr);  min($arr);
来源：http://iil.zhaomingkeji.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hfp.epnwcf.com

TS:   Math.max(...arr);
来源：http://xmn.ybcxt.top

Java: Collections.max(list);  Collections.min(list);
来源：http://uhj.andypj.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bjf.aibaodan.cn

Ruby: arr.max;  arr.min
来源：http://rex.dianchejie.cn

C#:   list.Max();  list.Min()
来源：http://ipk.vqdsnc.cn

[D18] 扁平化嵌套数组
来源：http://cea.ydjk.org.cn


<!-- 参考信息 -->
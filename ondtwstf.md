代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://imt.cashguo.top

Go:   func add(a, b int) int { return a + b }
来源：http://jrj.9152youxi.cn

Ruby: def add(a, b); a + b; end
来源：http://kop.jqgufenzy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bqk.redwolf501.top

[C02] 默认参数
来源：http://ipg.xingfuxueyuan.xyz

Py:   def greet(name="World"): return name
来源：http://cdd.ybcxt.top

PHP:  function greet($name = "World") { return $name; }
来源：http://xsc.sufxvd.cn

JS:   function greet(name = "World") { return name; }
来源：http://tui.shangyingyoupin.top

TS:   function greet(name: string = "World") { return name; }
来源：http://oiu.xinyue.icu

Java: // 无默认参数：方法重载或 Optional
来源：http://pbu.xuanzx.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ddh.gzhubu.top

Ruby: def greet(name = "World") = name
来源：http://zpt.52xcode.cn

C#:   string Greet(string name = "World") => name;
来源：http://ukn.svipenyu.cn

[C03] 可变参数
来源：http://hmo.shangyingyoupin.top

Py:   def total(*args): return sum(args)
来源：http://jnt.yangfankeji.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://guf.cucudq.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://aib.yj20258.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bqz.quarkkingdee.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ldt.zhijiandao.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://flx.quarkkingdee.top

Ruby: def total(*nums); nums.sum; end
来源：http://tjj.fehbvm.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jww.jiagoushi.top

[C04] 命名参数 / 关键字参数
来源：http://ppc.yueranfly.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wsb.shzxlz.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ujy.fktsv.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://smj.nwbrower.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lwg.jqgufenzy.top

Java: // 无：用 Builder 模式或 record
来源：http://xoz.birdmap.top

Go:   // 无：用配置结构体参数
来源：http://krx.9152youxi.cn

Ruby: f(a: 1, b: 2)
来源：http://ntn.zhixingplan.top

C#:   f(a: 1, b: 2)
来源：http://fas.wangdashe.top

[C05] 返回多个值
来源：http://sws.ywan-chungtsiang.top

Py:   return a, b
来源：http://wwd.aibaodan.cn

PHP:  return [$a, $b];
来源：http://llk.hfpthk.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zmm.jinqigufen.top

TS:   return { a, b };
来源：http://jop.chenjidiqi.icu

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pkb.xuetiantiany.cn

Go:   return a, b
来源：http://zlw.jyoumei.cn

Ruby: return a, b
来源：http://syg.kuanghao11.cn

C#:   return (a, b);              // ValueTuple
来源：http://hkb.xuetiantiany.cn

[C06] 匿名函数 / lambda
来源：http://ojm.zhongyouzk.top

Py:   square = lambda x: x * x
来源：http://okv.cdnleiting.top

PHP:  $square = fn($x) => $x * $x;
来源：http://blc.fktsv.cn

JS:   const square = x => x * x;
来源：http://tzb.xziqi.cn

TS:   const square = (x: number): number => x * x;
来源：http://pwk.shanyushiyangkeji.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jpn.zdqjudy.top

Go:   sq := func(x int) int { return x * x }
来源：http://kpy.jlsjyb.cn

Ruby: square = ->(x) { x * x }
来源：http://rat.gotoacloud.top

C#:   Func<int, int> square = x => x * x;
来源：http://ifw.nwbrower.top

[C07] 把函数作为参数传入
来源：http://qdg.snrcjt.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fho.chenlongwang.top

PHP:  array_map("strtoupper", $arr);
来源：http://syi.jinyuanbaomall.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://iis.xziqi.cn

TS:   arr.map(String)
来源：http://fpa.yj202588.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vco.hnqzz.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://epl.zhongyouzk.top

Ruby: arr.map(&:upcase)
来源：http://eci.zdbjq.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jlk.feifeiyinyue.top

[C08] 闭包
来源：http://vjk.bbcook.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gza.52xcode.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jzb.gotoacloud.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://esv.yj20258.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://csi.quarkkingdee.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://whc.cheryme.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fjl.sweek.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bkc.jyoumei.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gaa.jinqigufen.top

[C09] 递归
来源：http://vms.316326.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nht.gogol.net.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vri.zdbjq.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jpu.gzhubu.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nwd.ppjwa.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://aka.shuidangran.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sgh.redwolf501.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ybf.tanke756.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ofq.pycfn.com

[C10] 变量作用域
来源：http://eny.tarul.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ihj.tian-w.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lqs.xuanzx.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sih.9152youxi.cn

TS:   同 JS
来源：http://pis.cdnleiting.top

Java: 方法内为块级作用域
来源：http://tfl.cashguo.top

Go:   花括号块级作用域
来源：http://lfs.shuidangran.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hiy.jinqigufen.top

C#:   块级作用域
来源：http://uks.hcnkem.com

[C11] 模块导入与导出
来源：http://foq.yongpay.top

Py:   from module import func
来源：http://pva.havefunace.top

PHP:  require "file.php";  或 use App\Service;
来源：http://xod.jinyuanbaomall.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://gay.ppjwa.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bbz.ybcxt.top

Java: import java.util.List;
来源：http://iup.cheryme.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yyf.shzxlz.cn

Ruby: require "json"; require_relative "./util"
来源：http://wob.hammf.cn

C#:   using System.Text;
来源：http://uou.52xcode.cn

[C12] 立即执行函数 IIFE
来源：http://vmy.zdbjq.cn

Py:   (lambda: print("run"))()
来源：http://lgt.zdqjudy.top

PHP:  (function () { echo "run"; })();
来源：http://aou.tanke756.top

JS:   (() => { console.log("run"); })();
来源：http://xov.tanke756.top

TS:   (() => { console.log("run"); })();
来源：http://sho.shangyingyoupin.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vjc.zhoulong.xyz

Go:   func() { fmt.Println("run") }()
来源：http://muu.xinyue.icu

Ruby: -> { puts "run" }.call
来源：http://hit.jianghu66.top

C#:   // 无 IIFE：用静态构造函数
来源：http://elj.mhx1999.top

[C13] 类型声明 / 类型注解
来源：http://vph.zhaomingkeji.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hvo.hnqzz.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tnw.smart0.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ukb.hywenlv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tzn.svipenyu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vel.fengsongda.top

Go:   func add(a, b int) int
来源：http://kld.9152youxi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jhw.hcnkem.com

C#:   int Add(int a, int b) => a + b;
来源：http://smt.sjlbkw.cn

[C14] 泛型函数
来源：http://ktj.hnxiangtu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fuj.gaohongyu789.top

PHP:  // 无泛型
来源：http://ilp.hammf.cn

JS:   // 无泛型
来源：http://elo.zhengqikj.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nkt.jinyuanbaomall.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zvs.fanxiaobao.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://eub.hnqzz.top

Ruby: # 无泛型
来源：http://wef.feifeiyinyue.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tuj.bbcook.cn

[C15] 解构 / 展开参数
来源：http://bor.ppjwa.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rns.pengpengdd.cyou

PHP:  [$a, $b] = $pair;
来源：http://wzc.tanke756.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bkz.tanke756.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zwy.cheryme.top

Java: // 无解构
来源：http://oer.jqgfzy.top

Go:   // 无解构
来源：http://cwn.yanxiufei.cn

Ruby: a, b = pair
来源：http://wye.daxiang520.top

C#:   var (a, b) = pair;
来源：http://zki.feifeiyinyue.top

[C16] 函数 / 方法重载
来源：http://kwt.316326.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yoh.gogol.net.cn

PHP:  // 无重载
来源：http://wvl.yueranfly.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://vsr.ydjk.org.cn

TS:   // 用联合类型或重载签名声明
来源：http://kqd.chenjidiqi.icu

Java: void f(int a) {}  void f(String a) {}
来源：http://lgp.guowangkeji.top

Go:   // 无重载：用不同函数名
来源：http://uiy.yvedp.cn

Ruby: # 无重载：靠动态参数
来源：http://smu.aibaodan.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fjd.jinqigufen.top

================================================================================
来源：http://nxr.xziqi.cn

D. 数组 / 列表 / 集合
来源：http://tte.mhx1999.top

================================================================================
来源：http://gry.fengsongda.top

[D01] 创建数组 / 列表
来源：http://twb.gzhubu.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://bfp.chenlongwang.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sie.cdnleiting.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pwz.mhx1999.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ttk.hnxiangtu.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ejt.shanyushiyangtech.top

Go:   arr := []int{1, 2, 3}
来源：http://cam.hongshengwenyu.top

Ruby: arr = [1, 2, 3]
来源：http://goz.fehbvm.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xkl.quarkkingdee.top

[D02] 追加元素到末尾
来源：http://izi.fanxiaobao.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gzh.fzhhl.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://omf.pycfn.com

JS:   arr.push(4);
来源：http://fjl.yanxiufei.cn

TS:   arr.push(4);
来源：http://pfh.zdbjq.cn

Java: list.add(4);
来源：http://xcm.ctjpmb.com

Go:   arr = append(arr, 4)
来源：http://gnx.jqgufenzy.top

Ruby: arr << 4; arr.push(5)
来源：http://pga.jlsjyb.cn

C#:   list.Add(4);
来源：http://crz.nwbrower.top

[D03] 在指定位置插入元素
来源：http://wuc.sjlbkw.cn

Py:   arr.insert(0, 0)
来源：http://bhj.chenzaomai.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jqp.mhx1999.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nfp.ywan-chungtsiang.top

TS:   arr.splice(0, 0, 0);
来源：http://lok.zycfv.cn

Java: list.add(0, 0);
来源：http://yfa.jinqigfzy.top

Go:   arr = append([]int{0}, arr...)
来源：http://aui.jqgfzy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xmt.jinyuanbaomall.cn

C#:   list.Insert(0, 0);
来源：http://dpw.daria6918.cn

[D04] 删除元素
来源：http://puy.jqgfzy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pyq.meibo888.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://frv.zdqjudy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lqh.hysaishi.cn

TS:   arr.splice(0, 1);
来源：http://pws.fengsongda.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://osc.jinyuanbaomall.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://msb.birdmap.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tcc.ctjpmb.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yde.0kj1m.cn

[D05] 访问与修改元素
来源：http://eab.fehbvm.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nqf.jinqigfzy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mon.hongshengwenyu.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jhg.yongpay.top

TS:   arr[0]; arr.at(-1);
来源：http://crv.yongpay.top

Java: list.get(0); list.set(0, 9);
来源：http://iam.yfazqb.com

Go:   arr[0]; arr[0] = 9
来源：http://itf.gogol.net.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://udl.vehdjk.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fmf.xziqi.cn

[D06] 数组长度
来源：http://jsh.daxiang520.top

Py:   len(arr)
来源：http://esm.hnxiangtu.top

PHP:  count($arr);
来源：http://ayj.0kj1m.cn

JS:   arr.length
来源：http://roi.yj20258888.top

TS:   arr.length
来源：http://xpn.yvedp.cn

Java: list.size();
来源：http://kpw.mhx1999.top

Go:   len(arr)
来源：http://crr.xylfe.cn

Ruby: arr.length; arr.size
来源：http://oev.wangdashe.top

C#:   list.Count;
来源：http://wjr.jlsjyb.cn

[D07] 切片 / 取子数组
来源：http://hdr.52xcode.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dpx.xylfe.cn

PHP:  array_slice($arr, 1, 3);
来源：http://mag.jiagoushi.top

JS:   arr.slice(1, 4);
来源：http://xxn.meibo888.top

TS:   arr.slice(1, 4);
来源：http://lrg.yangfankeji.com

Java: list.subList(1, 4);
来源：http://iba.zhengqikj.top

Go:   arr[1:4]
来源：http://bjt.yj20258.top

Ruby: arr[1, 3]
来源：http://fyy.yangfankeji.com

C#:   list.GetRange(1, 3);
来源：http://nvn.0kj1m.cn

[D08] 合并两个数组
来源：http://qyk.uphjek.com

Py:   a + b;  a.extend(b)
来源：http://ogg.bbcook.cn

PHP:  array_merge($a, $b);
来源：http://tvg.jqgfzy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://sus.nanxinkj.top

TS:   [...a, ...b];
来源：http://hlj.svipenyu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ugv.ybcxt.top

Go:   append(a, b...)
来源：http://yaj.fengsongda.top

Ruby: a + b;  a.concat(b)
来源：http://evw.shuidangran.top

C#:   a.Concat(b).ToList()
来源：http://gjk.sysykeji.top

[D09] 排序（升序）
来源：http://rns.shuidangran.top

Py:   sorted(arr);  arr.sort()
来源：http://yqy.nanxuanxn.top

PHP:  sort($arr);
来源：http://rer.chenlongwang.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lor.fengsongda.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://kvd.pycfn.com

Java: Collections.sort(list);  list.sort(null);
来源：http://oyd.shangyingyoupin.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yif.yj20258.top

Ruby: arr.sort
来源：http://qhm.zhongyouzk.top

C#:   list.Sort();
来源：http://qxq.ppjwa.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://uzn.jyoumei.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uwp.birdmap.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fmn.zhixingplan.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://iel.ydzc1.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://edo.dianchejie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cab.iojbl.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bte.redwolf501.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cfp.cdnleiting.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tzm.sxryk.cn

[D11] 反转数组
来源：http://xrc.zhengqikj.top

Py:   arr[::-1];  arr.reverse()
来源：http://hxy.bbcook.cn

PHP:  array_reverse($arr);
来源：http://rkl.vqdsnc.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nba.cheryme.top

TS:   [...arr].reverse();
来源：http://ewj.sjlbkw.cn

Java: Collections.reverse(list);
来源：http://glv.hesvh.cn

Go:   slices.Reverse(arr)
来源：http://tzv.fktsv.cn

Ruby: arr.reverse
来源：http://qyh.jiagoushi.top

C#:   list.Reverse();
来源：http://gmn.shzxlz.cn

[D12] 查找元素下标
来源：http://dap.yongpay.top

Py:   arr.index(x);  x in arr
来源：http://rur.ctjpmb.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xdu.cdnleiting.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kue.quarkkingdee.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ykj.sjlbkw.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lcs.fengsongda.top

Go:   slices.Index(arr, x)
来源：http://xkk.jinyuanbaomall.cn

Ruby: arr.index(x)
来源：http://iaj.xuanzx.com

C#:   list.IndexOf(x);
来源：http://fyd.fktsv.cn

[D13] 过滤（保留满足条件的）
来源：http://zqx.yuanzhike.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zao.chenlongwang.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://oln.snrcjt.cn

JS:   arr.filter(x => x > 3)
来源：http://eyb.nanxinkj.top

TS:   arr.filter(x => x > 3)
来源：http://sow.sysykeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fkh.cucudq.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ixw.ppjwa.cn

Ruby: arr.select { |x| x > 3 }
来源：http://okn.vehdjk.com

C#:   list.Where(x => x > 3).ToList()
来源：http://gqw.ydjk.org.cn

[D14] 映射转换（每个元素变形）
来源：http://jnj.vqdsnc.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://czb.zycfv.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ztf.fengsongda.top

JS:   arr.map(x => x * 2)
来源：http://dic.9152youxi.cn

TS:   arr.map(x => x * 2)
来源：http://lzp.jyoumei.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://phu.cqqwz.cn

Go:   // 手写循环
来源：http://dyc.jinyuanbaomall.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fae.shuidangran.top

C#:   list.Select(x => x * 2).ToList()
来源：http://qqr.hcnkem.com

[D15] 去重
来源：http://iuy.cheryme.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lny.kuanghao11.cn

PHP:  array_unique($arr);
来源：http://une.hcnkem.com

JS:   [...new Set(arr)]
来源：http://zxz.zycfv.cn

TS:   [...new Set(arr)]
来源：http://ica.zhoulong.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bae.wangdashe.top

Go:   // 用 map[T]struct{} 手写
来源：http://boi.hnqzz.top

Ruby: arr.uniq
来源：http://nnv.ywan-chungtsiang.top

C#:   list.Distinct().ToList()
来源：http://pkq.xingfuxueyuan.xyz

[D16] 求和与平均值
来源：http://ozs.jlsjyb.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vkh.xziqi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tqz.xinyue.icu

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zei.nanxuanxn.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://igc.zhixingplan.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mnr.havefunace.top

Go:   // 手写循环累加
来源：http://oqz.feifeiyinyue.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xem.cashguo.top

C#:   list.Sum();  list.Average()
来源：http://ajl.316326.xyz

[D17] 最大值与最小值
来源：http://qbb.zhixingplan.top

Py:   max(arr);  min(arr)
来源：http://obr.wangdashe.top

PHP:  max($arr);  min($arr);
来源：http://uav.cheryme.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wkn.9152youxi.cn

TS:   Math.max(...arr);
来源：http://dmg.c1oappe.top

Java: Collections.max(list);  Collections.min(list);
来源：http://wjx.cashguo.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://est.yongpay.top

Ruby: arr.max;  arr.min
来源：http://pjf.havefunace.top

C#:   list.Max();  list.Min()
来源：http://btn.kuanghao11.cn

[D18] 扁平化嵌套数组
来源：http://oxm.yj20258.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bra.daxiang520.top

PHP:  array_merge(...$nested);
来源：http://wkb.snrcjt.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://szk.aibaodan.cn

TS:   nested.flat();
来源：http://fsq.xziqi.cn


<!-- 参考信息 -->
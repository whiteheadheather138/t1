代发 wailian999

[C02] 默认参数
来源：http://lwg.dianchejie.cn

Py:   def greet(name="World"): return name
来源：http://xps.jiagoushi.top

PHP:  function greet($name = "World") { return $name; }
来源：http://kht.zhixingplan.top

JS:   function greet(name = "World") { return name; }
来源：http://bgn.daxiang520.top

TS:   function greet(name: string = "World") { return name; }
来源：http://jti.shangyingyoupin.top

Java: // 无默认参数：方法重载或 Optional
来源：http://idm.yuanzhike.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://htt.cashguo.top

Ruby: def greet(name = "World") = name
来源：http://hgh.zhoulong.xyz

C#:   string Greet(string name = "World") => name;
来源：http://rjj.pycfn.com

[C03] 可变参数
来源：http://qdu.zdbjq.cn

Py:   def total(*args): return sum(args)
来源：http://ovc.gotoacloud.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sth.ywan-chungtsiang.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jsv.cdnleiting.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gpe.yj20258888.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vxf.yj20258888.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bye.yj202588.top

Ruby: def total(*nums); nums.sum; end
来源：http://abs.shzxlz.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nue.shuidangran.top

[C04] 命名参数 / 关键字参数
来源：http://mgu.jyoumei.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://oor.jyoumei.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wwn.zhaomingkeji.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kbg.guowangkeji.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gzh.jlsjyb.cn

Java: // 无：用 Builder 模式或 record
来源：http://wpi.hongshengwenyu.top

Go:   // 无：用配置结构体参数
来源：http://bug.wangshuangyany.cn

Ruby: f(a: 1, b: 2)
来源：http://geo.xuetiantiany.cn

C#:   f(a: 1, b: 2)
来源：http://wyw.epnwcf.com

[C05] 返回多个值
来源：http://vvs.xylfe.cn

Py:   return a, b
来源：http://wfx.jinyuanbaomall.cn

PHP:  return [$a, $b];
来源：http://clk.fengsongda.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://jll.fktsv.cn

TS:   return { a, b };
来源：http://hqn.vqdsnc.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ucu.quarkkingdee.top

Go:   return a, b
来源：http://zgu.9152youxi.cn

Ruby: return a, b
来源：http://wbf.zycfv.cn

C#:   return (a, b);              // ValueTuple
来源：http://clw.mhx1999.top

[C06] 匿名函数 / lambda
来源：http://qlb.ybcxt.top

Py:   square = lambda x: x * x
来源：http://hei.zhengqikj.top

PHP:  $square = fn($x) => $x * $x;
来源：http://nid.svipenyu.cn

JS:   const square = x => x * x;
来源：http://jxp.52xcode.cn

TS:   const square = (x: number): number => x * x;
来源：http://kyt.shangyingyoupin.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jxb.hammf.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hib.xziqi.cn

Ruby: square = ->(x) { x * x }
来源：http://qud.fktsv.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ifl.tian-w.cn

[C07] 把函数作为参数传入
来源：http://mon.epnwcf.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://uil.chenjidiqi.icu

PHP:  array_map("strtoupper", $arr);
来源：http://wzp.cdnleiting.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://txz.epnwcf.com

TS:   arr.map(String)
来源：http://zvl.yj20258888.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yns.sysykeji.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yvt.zhijiandao.cn

Ruby: arr.map(&:upcase)
来源：http://scq.fehbvm.com

C#:   arr.Select(s => s.ToUpper())
来源：http://fkn.cheryme.top

[C08] 闭包
来源：http://gdp.ehwqpu.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jdi.andypj.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ooj.feifeiyinyue.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qqj.hongshengwenyu.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ndh.feifeiyinyue.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://evq.feifeiyinyue.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dio.hnqzz.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ofr.fengsongda.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zsz.hammf.cn

[C09] 递归
来源：http://jak.jlsjyb.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qny.shanyushiyangtech.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://azx.dianchejie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pkg.zhixingplan.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mnd.sxryk.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://iuz.sufxvd.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://spk.zhiwuduotai.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nsk.zdqjudy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ach.shzxlz.cn

[C10] 变量作用域
来源：http://dig.zhongyouzk.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ors.guowangkeji.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zdn.xuetiantiany.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://klq.sjlbkw.cn

TS:   同 JS
来源：http://fkt.kuanghao11.cn

Java: 方法内为块级作用域
来源：http://wbz.yfazqb.com

Go:   花括号块级作用域
来源：http://wxq.dashuyun.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zzj.zdbjq.cn

C#:   块级作用域
来源：http://yyz.hnxiangtu.top

[C11] 模块导入与导出
来源：http://oth.chenzaomai.com

Py:   from module import func
来源：http://pdz.sysykeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://bgz.haohaochexian.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ndk.gzhubu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mgw.snrcjt.cn

Java: import java.util.List;
来源：http://qar.tian-w.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cow.tian-w.cn

Ruby: require "json"; require_relative "./util"
来源：http://hfb.sjlbkw.cn

C#:   using System.Text;
来源：http://pee.fehbvm.com

[C12] 立即执行函数 IIFE
来源：http://mxy.iojbl.cn

Py:   (lambda: print("run"))()
来源：http://nno.uphjek.com

PHP:  (function () { echo "run"; })();
来源：http://stc.bjfxy.top

JS:   (() => { console.log("run"); })();
来源：http://icg.meibo888.top

TS:   (() => { console.log("run"); })();
来源：http://uov.quarkkingdee.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xon.ydzc1.top

Go:   func() { fmt.Println("run") }()
来源：http://lvu.yongpay.top

Ruby: -> { puts "run" }.call
来源：http://kon.hammf.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xnv.wangdashe.top

[C13] 类型声明 / 类型注解
来源：http://mgq.haohaochexian.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ydq.aizwys.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mib.jlsjyb.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zgr.xuanzx.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fco.nwbrower.top

Java: int add(int a, int b) { return a + b; }
来源：http://ojp.zhengqikj.top

Go:   func add(a, b int) int
来源：http://zgg.bjfxy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jqb.dianchejie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://kkk.svipenyu.cn

[C14] 泛型函数
来源：http://ubo.hfpthk.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zra.hongshengwenyu.top

PHP:  // 无泛型
来源：http://uuc.jyoumei.cn

JS:   // 无泛型
来源：http://qai.shuidangran.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zjm.sysykeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gkm.bbcook.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://sdo.birdmap.top

Ruby: # 无泛型
来源：http://iph.feifeiyinyue.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rgb.jiagoushi.top

[C15] 解构 / 展开参数
来源：http://nua.jianghu66.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mug.ywan-chungtsiang.top

PHP:  [$a, $b] = $pair;
来源：http://zwa.hfpthk.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qhn.yueranfly.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dze.iojbl.cn

Java: // 无解构
来源：http://jfd.xuetiantiany.cn

Go:   // 无解构
来源：http://frh.wangshuangyany.cn

Ruby: a, b = pair
来源：http://ujo.gzhubu.top

C#:   var (a, b) = pair;
来源：http://rxs.quarkkingdee.top

[C16] 函数 / 方法重载
来源：http://dja.c1oappe.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wuw.zhijiandao.cn

PHP:  // 无重载
来源：http://ije.quarkkingdee.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://mcu.dianchejie.cn

TS:   // 用联合类型或重载签名声明
来源：http://kkr.ehwqpu.com

Java: void f(int a) {}  void f(String a) {}
来源：http://kpf.cashguo.top

Go:   // 无重载：用不同函数名
来源：http://ehr.gzhubu.top

Ruby: # 无重载：靠动态参数
来源：http://nso.bjfxy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://zto.daxiang520.top

================================================================================
来源：http://dzk.zdqjudy.top

D. 数组 / 列表 / 集合
来源：http://bcj.yanxiufei.cn

================================================================================
来源：http://cvc.gogol.net.cn

[D01] 创建数组 / 列表
来源：http://eug.fehbvm.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://etb.0kj1m.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hmp.ybcxt.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dtj.snrcjt.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://pmb.gzhubu.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mau.tanke756.top

Go:   arr := []int{1, 2, 3}
来源：http://fds.feifeiyinyue.top

Ruby: arr = [1, 2, 3]
来源：http://cxm.jinqigufen.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fos.jinyuanbaomall.cn

[D02] 追加元素到末尾
来源：http://tzk.jianghu66.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jgy.ehwqpu.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://usb.cheryme.top

JS:   arr.push(4);
来源：http://isb.pengpengdd.cyou

TS:   arr.push(4);
来源：http://fck.zhoulong.xyz

Java: list.add(4);
来源：http://zwn.zycfv.cn

Go:   arr = append(arr, 4)
来源：http://ath.chenjidiqi.icu

Ruby: arr << 4; arr.push(5)
来源：http://ijs.nanxuanxn.top

C#:   list.Add(4);
来源：http://uzt.svipenyu.cn

[D03] 在指定位置插入元素
来源：http://njz.0kj1m.cn

Py:   arr.insert(0, 0)
来源：http://zyd.yj202588.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gic.ybcxt.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cok.pengpengdd.cyou

TS:   arr.splice(0, 0, 0);
来源：http://ptf.zhaomingkeji.xyz

Java: list.add(0, 0);
来源：http://uml.tanke756.top

Go:   arr = append([]int{0}, arr...)
来源：http://llh.xingfuxueyuan.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://itv.xziqi.cn

C#:   list.Insert(0, 0);
来源：http://ajr.xziqi.cn

[D04] 删除元素
来源：http://kus.zhijiandao.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kzw.pengpengdd.cyou

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://quv.jqgfzy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vpq.havefunace.top

TS:   arr.splice(0, 1);
来源：http://vky.fehbvm.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lpv.daxiang520.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xff.xylfe.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ecw.bbcook.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://iil.shangyingyoupin.top

[D05] 访问与修改元素
来源：http://rhn.hnqzz.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://znc.zdbjq.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fud.gotoacloud.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wru.chenlongwang.top

TS:   arr[0]; arr.at(-1);
来源：http://mep.gaohongyu789.top

Java: list.get(0); list.set(0, 9);
来源：http://gcr.yongpay.top

Go:   arr[0]; arr[0] = 9
来源：http://dkb.jyoumei.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lrk.shuidangran.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ucl.yj20258888.top

[D06] 数组长度
来源：http://ofq.hesvh.cn

Py:   len(arr)
来源：http://xnp.hongshengwenyu.top

PHP:  count($arr);
来源：http://bwy.shangyingyoupin.top

JS:   arr.length
来源：http://zmj.gotoacloud.top

TS:   arr.length
来源：http://mel.zycfv.cn

Java: list.size();
来源：http://phu.cheryme.top

Go:   len(arr)
来源：http://qhl.hongshengwenyu.top

Ruby: arr.length; arr.size
来源：http://jlg.chenjidiqi.icu

C#:   list.Count;
来源：http://xsb.nanxinkj.top

[D07] 切片 / 取子数组
来源：http://abr.shzxlz.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jeu.shanyushiyangtech.top

PHP:  array_slice($arr, 1, 3);
来源：http://say.nanxinkj.top

JS:   arr.slice(1, 4);
来源：http://sis.9152youxi.cn

TS:   arr.slice(1, 4);
来源：http://sok.shanyushiyangtech.top

Java: list.subList(1, 4);
来源：http://mun.birdmap.top

Go:   arr[1:4]
来源：http://jfl.zdqjudy.top

Ruby: arr[1, 3]
来源：http://irl.shanyushiyangtech.top

C#:   list.GetRange(1, 3);
来源：http://uwn.hnxiangtu.top

[D08] 合并两个数组
来源：http://qkk.gzhubu.top

Py:   a + b;  a.extend(b)
来源：http://yhi.mhx1999.top

PHP:  array_merge($a, $b);
来源：http://xbf.fanxiaobao.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://qqa.zhixingplan.top

TS:   [...a, ...b];
来源：http://eqj.fzhhl.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ihl.tianlin.xyz

Go:   append(a, b...)
来源：http://dhl.dashuyun.cn

Ruby: a + b;  a.concat(b)
来源：http://olg.cashguo.top

C#:   a.Concat(b).ToList()
来源：http://ksy.xuetiantiany.cn

[D09] 排序（升序）
来源：http://esk.aibaodan.cn

Py:   sorted(arr);  arr.sort()
来源：http://okk.guannengcc.top

PHP:  sort($arr);
来源：http://jza.guowangkeji.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ley.yfazqb.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://huu.yj202588.top

Java: Collections.sort(list);  list.sort(null);
来源：http://rdh.tanke756.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qgc.guannengcc.top

Ruby: arr.sort
来源：http://veb.sjlbkw.cn

C#:   list.Sort();
来源：http://nxn.chenjidiqi.icu

[D10] 自定义排序（按字段 / 多条件）
来源：http://wos.hongshengwenyu.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bli.daria6918.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zxy.c1oappe.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ize.jinqigfzy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pgr.yanxiufei.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zvy.dashuyun.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sjn.aizwys.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://eyo.zhijiandao.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nfb.sxryk.cn

[D11] 反转数组
来源：http://zce.cheryme.top

Py:   arr[::-1];  arr.reverse()
来源：http://jul.fanxiaobao.xyz

PHP:  array_reverse($arr);
来源：http://adp.yj20258888.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ygc.sxryk.cn

TS:   [...arr].reverse();
来源：http://byh.hnxiangtu.top

Java: Collections.reverse(list);
来源：http://zor.tianlin.xyz

Go:   slices.Reverse(arr)
来源：http://ewq.havefunace.top

Ruby: arr.reverse
来源：http://xkl.guowangkeji.top

C#:   list.Reverse();
来源：http://dho.jyoumei.cn

[D12] 查找元素下标
来源：http://bef.jinqigufen.top

Py:   arr.index(x);  x in arr
来源：http://rzw.daxiang520.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://usc.jlsjyb.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vle.shangyingyoupin.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gel.tanke756.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://poo.chenlongwang.top

Go:   slices.Index(arr, x)
来源：http://hti.chenzaomai.com

Ruby: arr.index(x)
来源：http://uvc.redwolf501.top

C#:   list.IndexOf(x);
来源：http://juj.epnwcf.com

[D13] 过滤（保留满足条件的）
来源：http://jdr.daxiang520.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://idw.zycfv.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gxe.tarul.cn

JS:   arr.filter(x => x > 3)
来源：http://vpy.gzhubu.top

TS:   arr.filter(x => x > 3)
来源：http://bjx.andypj.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uqe.bbcook.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cbb.yj20258888.top

Ruby: arr.select { |x| x > 3 }
来源：http://hvl.birdmap.top

C#:   list.Where(x => x > 3).ToList()
来源：http://tsa.daxiang520.top

[D14] 映射转换（每个元素变形）
来源：http://ecz.vqdsnc.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://eiz.yvedp.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yae.xylfe.cn

JS:   arr.map(x => x * 2)
来源：http://tmj.daxiang520.top

TS:   arr.map(x => x * 2)
来源：http://pvd.havefunace.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://tsi.yj20258888.top

Go:   // 手写循环
来源：http://pia.yj202588.top

Ruby: arr.map { |x| x * 2 }
来源：http://zhn.sufxvd.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://tsu.yj20258.top

[D15] 去重
来源：http://kyw.shzxlz.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nnn.tianlin.xyz

PHP:  array_unique($arr);
来源：http://esp.quarkkingdee.top

JS:   [...new Set(arr)]
来源：http://gxs.vehdjk.com

TS:   [...new Set(arr)]
来源：http://bpv.feifeiyinyue.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hmt.yonumen.top

Go:   // 用 map[T]struct{} 手写
来源：http://atp.fengsongda.top

Ruby: arr.uniq
来源：http://lrp.ehwqpu.com

C#:   list.Distinct().ToList()
来源：http://ecd.jyoumei.cn

[D16] 求和与平均值
来源：http://zpz.havefunace.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://iyb.yvedp.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rnu.tianlin.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jrv.yj202588.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://aeo.jianghu66.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mtv.yj20258.top

Go:   // 手写循环累加
来源：http://wus.shuidangran.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nqf.ybcxt.top

C#:   list.Sum();  list.Average()
来源：http://odz.ppjwa.cn

[D17] 最大值与最小值
来源：http://qij.yj202588.top

Py:   max(arr);  min(arr)
来源：http://oug.zdqjudy.top

PHP:  max($arr);  min($arr);
来源：http://bhd.zdqjudy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tph.fehbvm.com

TS:   Math.max(...arr);
来源：http://rqs.chenjidiqi.icu

Java: Collections.max(list);  Collections.min(list);
来源：http://agf.yvedp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nir.316326.xyz

Ruby: arr.max;  arr.min
来源：http://vdi.hnqzz.top

C#:   list.Max();  list.Min()
来源：http://wzx.fzhhl.top

[D18] 扁平化嵌套数组
来源：http://rkb.gotoacloud.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ney.dashuyun.cn

PHP:  array_merge(...$nested);
来源：http://ecd.ctjpmb.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nhz.zhixingplan.top

TS:   nested.flat();
来源：http://rth.jyoumei.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://uhp.zdbjq.cn

Go:   // 手写双层循环
来源：http://jaw.gzhubu.top

Ruby: nested.flatten
来源：http://eah.jinyuanbaomall.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://dhm.tianlin.xyz


<!-- 参考信息 -->
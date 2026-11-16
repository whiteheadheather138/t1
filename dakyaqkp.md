代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://nve.yongpay.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fjl.zhongyouzk.top

[C04] 命名参数 / 关键字参数
来源：http://mpd.gzhubu.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vcx.yonumen.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nuj.fktsv.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://drp.jinqigufen.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ncf.birdmap.top

Java: // 无：用 Builder 模式或 record
来源：http://qll.guannengcc.top

Go:   // 无：用配置结构体参数
来源：http://qlj.wangshuangyany.cn

Ruby: f(a: 1, b: 2)
来源：http://unr.zhengqikj.top

C#:   f(a: 1, b: 2)
来源：http://yhr.ywan-chungtsiang.top

[C05] 返回多个值
来源：http://ygq.0kj1m.cn

Py:   return a, b
来源：http://sef.yonumen.top

PHP:  return [$a, $b];
来源：http://rur.0kj1m.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://sap.cashguo.top

TS:   return { a, b };
来源：http://xkd.jqgfzy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lep.wangdashe.top

Go:   return a, b
来源：http://pyq.vehdjk.com

Ruby: return a, b
来源：http://sap.epnwcf.com

C#:   return (a, b);              // ValueTuple
来源：http://lxr.zhoulong.xyz

[C06] 匿名函数 / lambda
来源：http://gqf.sjlbkw.cn

Py:   square = lambda x: x * x
来源：http://lue.jyoumei.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xbf.bjfxy.top

JS:   const square = x => x * x;
来源：http://elh.guannengcc.top

TS:   const square = (x: number): number => x * x;
来源：http://qoe.hywenlv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hlo.shangyingyoupin.top

Go:   sq := func(x int) int { return x * x }
来源：http://zjy.shanyushiyangtech.top

Ruby: square = ->(x) { x * x }
来源：http://yhz.hesvh.cn

C#:   Func<int, int> square = x => x * x;
来源：http://itu.nanxuanxn.top

[C07] 把函数作为参数传入
来源：http://fqg.jinghuilouyu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rlm.fanxiaobao.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://sjh.bbcook.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nsj.fktsv.cn

TS:   arr.map(String)
来源：http://qyu.yangfankeji.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vye.zhaomingkeji.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qex.pycfn.com

Ruby: arr.map(&:upcase)
来源：http://fmf.havefunace.top

C#:   arr.Select(s => s.ToUpper())
来源：http://qmx.chenlongwang.top

[C08] 闭包
来源：http://low.guannengcc.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gfr.andypj.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lgg.jyoumei.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bhm.nanxuanxn.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xgs.snrcjt.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zky.shzxlz.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tww.aizwys.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ndw.ydjk.org.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lqb.jinyuanbaomall.cn

[C09] 递归
来源：http://yrc.pycfn.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://isn.fengsongda.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://eqh.chenlongwang.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tbr.andypj.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lzh.mhx1999.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://loj.tianlin.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://obt.zhijiandao.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zhu.epnwcf.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rmk.meibo888.top

[C10] 变量作用域
来源：http://ojc.jinyuanbaomall.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://juj.c1oappe.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://noo.kuanghao11.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rjn.cdnleiting.top

TS:   同 JS
来源：http://isu.316326.xyz

Java: 方法内为块级作用域
来源：http://pox.cucudq.cn

Go:   花括号块级作用域
来源：http://fcu.xuanzx.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fjm.nwbrower.top

C#:   块级作用域
来源：http://xui.aizwys.cn

[C11] 模块导入与导出
来源：http://jmo.nwbrower.top

Py:   from module import func
来源：http://dxv.epnwcf.com

PHP:  require "file.php";  或 use App\Service;
来源：http://ulg.hfpthk.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://for.sufxvd.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gdl.quarkkingdee.top

Java: import java.util.List;
来源：http://scn.nanxuanxn.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rmu.pengpengdd.cyou

Ruby: require "json"; require_relative "./util"
来源：http://iur.ivvv.top

C#:   using System.Text;
来源：http://eol.cheryme.top

[C12] 立即执行函数 IIFE
来源：http://alw.tanke756.top

Py:   (lambda: print("run"))()
来源：http://xfe.cucudq.cn

PHP:  (function () { echo "run"; })();
来源：http://bxb.tarul.cn

JS:   (() => { console.log("run"); })();
来源：http://dqe.yuanzhike.top

TS:   (() => { console.log("run"); })();
来源：http://bkv.jianghu66.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zou.gzhubu.top

Go:   func() { fmt.Println("run") }()
来源：http://vvm.yuxming.cn

Ruby: -> { puts "run" }.call
来源：http://ypz.gaohongyu789.top

C#:   // 无 IIFE：用静态构造函数
来源：http://tmh.jlsjyb.cn

[C13] 类型声明 / 类型注解
来源：http://qqj.hesvh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ruv.yuxming.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rce.shanyushiyangkeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cyl.zdbjq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oob.fehbvm.com

Java: int add(int a, int b) { return a + b; }
来源：http://dxp.havefunace.top

Go:   func add(a, b int) int
来源：http://faz.daxiang520.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ojg.hysaishi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nfx.yongpay.top

[C14] 泛型函数
来源：http://rxd.gaohongyu789.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://omt.nanxinkj.top

PHP:  // 无泛型
来源：http://dic.316326.xyz

JS:   // 无泛型
来源：http://tdf.jianghu66.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tlu.yvedp.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ysw.jqgufenzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://axa.gzhubu.top

Ruby: # 无泛型
来源：http://yav.zhixingplan.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jmd.redwolf501.top

[C15] 解构 / 展开参数
来源：http://gmg.nwbrower.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tmk.jlsjyb.cn

PHP:  [$a, $b] = $pair;
来源：http://ist.zhengqikj.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fux.shanyushiyangtech.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zqn.hywenlv.cn

Java: // 无解构
来源：http://knv.zhaomingkeji.xyz

Go:   // 无解构
来源：http://tmw.chenlongwang.top

Ruby: a, b = pair
来源：http://oys.yj202588.top

C#:   var (a, b) = pair;
来源：http://syd.chenzaomai.com

[C16] 函数 / 方法重载
来源：http://ryf.cheryme.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wwi.yangfankeji.com

PHP:  // 无重载
来源：http://uwx.vehdjk.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://usj.vehdjk.com

TS:   // 用联合类型或重载签名声明
来源：http://lhz.jinqigufen.top

Java: void f(int a) {}  void f(String a) {}
来源：http://lao.yangfankeji.com

Go:   // 无重载：用不同函数名
来源：http://bpy.xuanzx.com

Ruby: # 无重载：靠动态参数
来源：http://fes.bbcook.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://vym.vehdjk.com

================================================================================
来源：http://hil.jiagoushi.top

D. 数组 / 列表 / 集合
来源：http://brj.aibaodan.cn

================================================================================
来源：http://bct.shuidangran.top

[D01] 创建数组 / 列表
来源：http://mxc.zdbjq.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://flm.meibo888.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vut.epnwcf.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hqm.dianchejie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://tsr.jinghuilouyu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://spx.jlsjyb.cn

Go:   arr := []int{1, 2, 3}
来源：http://aqn.fengsongda.top

Ruby: arr = [1, 2, 3]
来源：http://fan.ybcxt.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gld.chenlongwang.top

[D02] 追加元素到末尾
来源：http://mhz.zhixingplan.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jbr.zhixingplan.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xbw.daria6918.cn

JS:   arr.push(4);
来源：http://dec.vqdsnc.cn

TS:   arr.push(4);
来源：http://rwq.zhijiandao.cn

Java: list.add(4);
来源：http://qhu.fktsv.cn

Go:   arr = append(arr, 4)
来源：http://kso.bjfxy.top

Ruby: arr << 4; arr.push(5)
来源：http://rtp.bjfxy.top

C#:   list.Add(4);
来源：http://pav.fehbvm.com

[D03] 在指定位置插入元素
来源：http://jae.daxiang520.top

Py:   arr.insert(0, 0)
来源：http://oxd.vehdjk.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wgs.chenlongwang.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hqw.tanke756.top

TS:   arr.splice(0, 0, 0);
来源：http://qjv.hysaishi.cn

Java: list.add(0, 0);
来源：http://qoy.tian-w.cn

Go:   arr = append([]int{0}, arr...)
来源：http://did.gzhubu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tad.xziqi.cn

C#:   list.Insert(0, 0);
来源：http://jli.guowangkeji.top

[D04] 删除元素
来源：http://lpk.jlsjyb.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qdl.yuanzhike.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pvf.jqgufenzy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cek.tianlin.xyz

TS:   arr.splice(0, 1);
来源：http://rja.zhijiandao.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gtt.jinyuanbaomall.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ofg.zdqjudy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ife.svipenyu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jbr.jinyuanbaomall.cn

[D05] 访问与修改元素
来源：http://ffn.nanxuanxn.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pvv.bjfxy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yod.epnwcf.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zui.xingfuxueyuan.xyz

TS:   arr[0]; arr.at(-1);
来源：http://rhx.yuanzhike.top

Java: list.get(0); list.set(0, 9);
来源：http://cic.shzxlz.cn

Go:   arr[0]; arr[0] = 9
来源：http://acu.hammf.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fvv.hfpthk.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://foh.nwbrower.top

[D06] 数组长度
来源：http://aoz.sweek.top

Py:   len(arr)
来源：http://yqg.yonumen.top

PHP:  count($arr);
来源：http://ylb.vehdjk.com

JS:   arr.length
来源：http://mbm.chenlongwang.top

TS:   arr.length
来源：http://ydb.ybcxt.top

Java: list.size();
来源：http://vky.tianlin.xyz

Go:   len(arr)
来源：http://noe.wangdashe.top

Ruby: arr.length; arr.size
来源：http://jsc.xingfuxueyuan.xyz

C#:   list.Count;
来源：http://uso.hnqzz.top

[D07] 切片 / 取子数组
来源：http://bio.ivvv.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fur.xinyue.icu

PHP:  array_slice($arr, 1, 3);
来源：http://ftc.zhengqikj.top

JS:   arr.slice(1, 4);
来源：http://nqg.vehdjk.com

TS:   arr.slice(1, 4);
来源：http://alu.zhixingplan.top

Java: list.subList(1, 4);
来源：http://hfs.yj20258.top

Go:   arr[1:4]
来源：http://sfu.hnxiangtu.top

Ruby: arr[1, 3]
来源：http://tll.zhongyouzk.top

C#:   list.GetRange(1, 3);
来源：http://zek.iojbl.cn

[D08] 合并两个数组
来源：http://nzd.zhongyouzk.top

Py:   a + b;  a.extend(b)
来源：http://riv.ppjwa.cn

PHP:  array_merge($a, $b);
来源：http://mmk.xuetiantiany.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://pfb.tianlin.xyz

TS:   [...a, ...b];
来源：http://wmv.yj20258888.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://thj.snrcjt.cn

Go:   append(a, b...)
来源：http://eze.sweek.top

Ruby: a + b;  a.concat(b)
来源：http://lbi.zhixingplan.top

C#:   a.Concat(b).ToList()
来源：http://mhc.sysykeji.top

[D09] 排序（升序）
来源：http://uer.feifeiyinyue.top

Py:   sorted(arr);  arr.sort()
来源：http://ion.jqgufenzy.top

PHP:  sort($arr);
来源：http://afw.zdbjq.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://eqg.cdnleiting.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ork.iojbl.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zew.hcnkem.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qkd.zdbjq.cn

Ruby: arr.sort
来源：http://pfv.wangshuangyany.cn

C#:   list.Sort();
来源：http://ygl.aizwys.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mwq.jqgfzy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lom.guowangkeji.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ffb.snrcjt.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hec.jinqigfzy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://etj.wangdashe.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://eox.daria6918.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vjx.0kj1m.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://upk.hywenlv.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://crj.ydjk.org.cn

[D11] 反转数组
来源：http://pwd.sufxvd.cn

Py:   arr[::-1];  arr.reverse()
来源：http://aiv.birdmap.top

PHP:  array_reverse($arr);
来源：http://qem.chenjidiqi.icu

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fhq.52xcode.cn

TS:   [...arr].reverse();
来源：http://lbd.gogol.net.cn

Java: Collections.reverse(list);
来源：http://lvx.c1oappe.top

Go:   slices.Reverse(arr)
来源：http://kbp.ivvv.top

Ruby: arr.reverse
来源：http://jdi.shangyingyoupin.top

C#:   list.Reverse();
来源：http://osu.sjlbkw.cn

[D12] 查找元素下标
来源：http://uuf.jiagoushi.top

Py:   arr.index(x);  x in arr
来源：http://xgp.jinqigfzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qrv.shanyushiyangkeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rtz.gogol.net.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ism.c1oappe.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kct.jinqigufen.top

Go:   slices.Index(arr, x)
来源：http://pfw.jinyuanbaomall.cn

Ruby: arr.index(x)
来源：http://vqq.gaohongyu789.top

C#:   list.IndexOf(x);
来源：http://tzp.xuetiantiany.cn

[D13] 过滤（保留满足条件的）
来源：http://fdn.cucudq.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kfi.jianghu66.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://puw.feifeiyinyue.top

JS:   arr.filter(x => x > 3)
来源：http://ouw.hysaishi.cn

TS:   arr.filter(x => x > 3)
来源：http://uui.jinqigfzy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://txt.xuanzx.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hyw.jiagoushi.top

Ruby: arr.select { |x| x > 3 }
来源：http://vtk.gaohongyu789.top

C#:   list.Where(x => x > 3).ToList()
来源：http://avo.xziqi.cn

[D14] 映射转换（每个元素变形）
来源：http://dzb.vqdsnc.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ohh.dianchejie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ayx.jqgufenzy.top

JS:   arr.map(x => x * 2)
来源：http://oyi.jqgfzy.top

TS:   arr.map(x => x * 2)
来源：http://zju.bjfxy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ydz.nanxinkj.top

Go:   // 手写循环
来源：http://lno.guowangkeji.top

Ruby: arr.map { |x| x * 2 }
来源：http://fdb.svipenyu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://aud.jinqigufen.top

[D15] 去重
来源：http://cdh.shanyushiyangtech.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ykm.kuanghao11.cn

PHP:  array_unique($arr);
来源：http://dne.snrcjt.cn

JS:   [...new Set(arr)]
来源：http://cfn.gzhubu.top

TS:   [...new Set(arr)]
来源：http://weo.ydjk.org.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mka.yj202588.top

Go:   // 用 map[T]struct{} 手写
来源：http://ykk.pengpengdd.cyou

Ruby: arr.uniq
来源：http://qdh.iojbl.cn

C#:   list.Distinct().ToList()
来源：http://kwi.jqgfzy.top

[D16] 求和与平均值
来源：http://eod.yj202588.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hat.zhongyouzk.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bfx.gaohongyu789.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yhg.yvedp.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://aws.shanyushiyangtech.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mdp.jyoumei.cn

Go:   // 手写循环累加
来源：http://zrc.dashuyun.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://aph.hcnkem.com

C#:   list.Sum();  list.Average()
来源：http://kum.cqqwz.cn

[D17] 最大值与最小值
来源：http://ewt.c1oappe.top

Py:   max(arr);  min(arr)
来源：http://bge.gzhubu.top

PHP:  max($arr);  min($arr);
来源：http://pju.tianlin.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wys.nanxuanxn.top

TS:   Math.max(...arr);
来源：http://iig.cheryme.top

Java: Collections.max(list);  Collections.min(list);
来源：http://zvd.hywenlv.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://iey.hesvh.cn

Ruby: arr.max;  arr.min
来源：http://qvs.cqqwz.cn

C#:   list.Max();  list.Min()
来源：http://qmj.redwolf501.top

[D18] 扁平化嵌套数组
来源：http://hga.nanxinkj.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mvs.pycfn.com

PHP:  array_merge(...$nested);
来源：http://sfx.fanxiaobao.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mwj.mhx1999.top

TS:   nested.flat();
来源：http://lhe.iojbl.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qyw.xziqi.cn

Go:   // 手写双层循环
来源：http://tgm.hfpthk.cn

Ruby: nested.flatten
来源：http://cox.shzxlz.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://owh.daria6918.cn

[D19] 按字段分组
来源：http://kci.hysaishi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kei.fanxiaobao.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ayo.jinqigufen.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://szg.vehdjk.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://uci.xingfuxueyuan.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kur.chenzaomai.com

Go:   // 手写 map[string][]T
来源：http://tkw.ctjpmb.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://rfp.fengsongda.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nne.zhengqikj.top

[D20] 统计每个元素出现次数
来源：http://oke.jianghu66.top

Py:   Counter(arr)
来源：http://tue.ivvv.top

PHP:  array_count_values($arr);
来源：http://ect.dashuyun.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jwu.cqqwz.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nhz.jiagoushi.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sdw.shanyushiyangkeji.top

Go:   // 手写 map[T]int
来源：http://qeh.hnxiangtu.top


<!-- 参考信息 -->
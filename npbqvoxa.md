代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://avy.9152youxi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pcn.uphjek.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gnw.haohaochexian.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pxl.xuetiantiany.cn

Ruby: def total(*nums); nums.sum; end
来源：http://jih.jinqigufen.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://khi.birdmap.top

[C04] 命名参数 / 关键字参数
来源：http://vhl.mhx1999.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jzf.daria6918.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lcz.fzhhl.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rha.nwbrower.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rrq.cucudq.cn

Java: // 无：用 Builder 模式或 record
来源：http://vyk.ctjpmb.com

Go:   // 无：用配置结构体参数
来源：http://lvd.0kj1m.cn

Ruby: f(a: 1, b: 2)
来源：http://tss.shuidangran.top

C#:   f(a: 1, b: 2)
来源：http://okj.meibo888.top

[C05] 返回多个值
来源：http://jud.316326.xyz

Py:   return a, b
来源：http://kgp.kuanghao11.cn

PHP:  return [$a, $b];
来源：http://ifs.feifeiyinyue.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ggj.jiagoushi.top

TS:   return { a, b };
来源：http://dip.ydjk.org.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qhw.redwolf501.top

Go:   return a, b
来源：http://kti.fengsongda.top

Ruby: return a, b
来源：http://age.nanxinkj.top

C#:   return (a, b);              // ValueTuple
来源：http://ppy.iojbl.cn

[C06] 匿名函数 / lambda
来源：http://dny.cdnleiting.top

Py:   square = lambda x: x * x
来源：http://hoj.xylfe.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xiu.ywan-chungtsiang.top

JS:   const square = x => x * x;
来源：http://fbx.ybcxt.top

TS:   const square = (x: number): number => x * x;
来源：http://vmw.cucudq.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dvx.havefunace.top

Go:   sq := func(x int) int { return x * x }
来源：http://rne.ctjpmb.com

Ruby: square = ->(x) { x * x }
来源：http://ymu.zdbjq.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ncl.hesvh.cn

[C07] 把函数作为参数传入
来源：http://twf.ywan-chungtsiang.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gny.jinyuanbaomall.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ade.chenzaomai.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ygz.andypj.xyz

TS:   arr.map(String)
来源：http://kky.ywan-chungtsiang.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://avc.shanyushiyangtech.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ivt.shanyushiyangkeji.top

Ruby: arr.map(&:upcase)
来源：http://jrw.cashguo.top

C#:   arr.Select(s => s.ToUpper())
来源：http://zwb.ywan-chungtsiang.top

[C08] 闭包
来源：http://jed.zhixingplan.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uwr.ppjwa.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vsc.nanxuanxn.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ehf.xylfe.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://akz.haohaochexian.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://otu.vqdsnc.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lut.daxiang520.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kxr.hfpthk.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qnq.aibaodan.cn

[C09] 递归
来源：http://ddd.sweek.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://urz.dashuyun.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ikp.snrcjt.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lmd.shangyingyoupin.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://epc.kuanghao11.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uwj.iojbl.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hsw.fktsv.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zul.hnxiangtu.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qzv.epnwcf.com

[C10] 变量作用域
来源：http://rme.chenzaomai.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kal.hnqzz.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cmg.chenjidiqi.icu

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jhv.cqqwz.cn

TS:   同 JS
来源：http://rnv.smart0.xyz

Java: 方法内为块级作用域
来源：http://hzz.jyoumei.cn

Go:   花括号块级作用域
来源：http://bdp.hfpthk.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dwg.zhiwuduotai.top

C#:   块级作用域
来源：http://qgz.hfpthk.cn

[C11] 模块导入与导出
来源：http://rqd.bbcook.cn

Py:   from module import func
来源：http://rxb.ctjpmb.com

PHP:  require "file.php";  或 use App\Service;
来源：http://kxa.shangyingyoupin.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://mgw.wangshuangyany.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vbr.pengpengdd.cyou

Java: import java.util.List;
来源：http://vrg.yonumen.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fqs.yj20258888.top

Ruby: require "json"; require_relative "./util"
来源：http://tdg.9152youxi.cn

C#:   using System.Text;
来源：http://ytb.shuidangran.top

[C12] 立即执行函数 IIFE
来源：http://wvh.quarkkingdee.top

Py:   (lambda: print("run"))()
来源：http://fji.tarul.cn

PHP:  (function () { echo "run"; })();
来源：http://xvp.guannengcc.top

JS:   (() => { console.log("run"); })();
来源：http://cmk.zhixingplan.top

TS:   (() => { console.log("run"); })();
来源：http://lqu.epnwcf.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wgn.zhengqikj.top

Go:   func() { fmt.Println("run") }()
来源：http://pux.shanyushiyangkeji.top

Ruby: -> { puts "run" }.call
来源：http://ztg.gotoacloud.top

C#:   // 无 IIFE：用静态构造函数
来源：http://bzz.yuanzhike.top

[C13] 类型声明 / 类型注解
来源：http://osw.ydzc1.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://aro.jinghuilouyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kpr.svipenyu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vff.cqqwz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://spn.wangdashe.top

Java: int add(int a, int b) { return a + b; }
来源：http://ils.c1oappe.top

Go:   func add(a, b int) int
来源：http://gwt.aizwys.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://eds.chenjidiqi.icu

C#:   int Add(int a, int b) => a + b;
来源：http://fvk.ywan-chungtsiang.top

[C14] 泛型函数
来源：http://qyb.xuanzx.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mii.haohaochexian.top

PHP:  // 无泛型
来源：http://rvj.snrcjt.cn

JS:   // 无泛型
来源：http://fvr.birdmap.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fuj.zdbjq.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://acb.hnxiangtu.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kow.ybcxt.top

Ruby: # 无泛型
来源：http://lxc.yueranfly.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ubt.nanxinkj.top

[C15] 解构 / 展开参数
来源：http://ohj.guannengcc.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nsx.vqdsnc.cn

PHP:  [$a, $b] = $pair;
来源：http://xlq.nanxinkj.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://djy.pycfn.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ilz.cucudq.cn

Java: // 无解构
来源：http://yki.ehwqpu.com

Go:   // 无解构
来源：http://jcf.uphjek.com

Ruby: a, b = pair
来源：http://byf.zhijiandao.cn

C#:   var (a, b) = pair;
来源：http://ycv.sufxvd.cn

[C16] 函数 / 方法重载
来源：http://evj.yueranfly.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pln.jinyuanbaomall.cn

PHP:  // 无重载
来源：http://aci.aizwys.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xwk.zhijiandao.cn

TS:   // 用联合类型或重载签名声明
来源：http://xlb.zhijiandao.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rru.redwolf501.top

Go:   // 无重载：用不同函数名
来源：http://ggq.jqgufenzy.top

Ruby: # 无重载：靠动态参数
来源：http://toh.kuanghao11.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fxj.xinyue.icu

================================================================================
来源：http://mtx.aibaodan.cn

D. 数组 / 列表 / 集合
来源：http://igt.dianchejie.cn

================================================================================
来源：http://rgk.jinqigufen.top

[D01] 创建数组 / 列表
来源：http://rsy.fanxiaobao.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://pjr.shangyingyoupin.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gfe.vqdsnc.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://twb.jqgufenzy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://rtf.havefunace.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fut.iojbl.cn

Go:   arr := []int{1, 2, 3}
来源：http://mug.xingfuxueyuan.xyz

Ruby: arr = [1, 2, 3]
来源：http://tbk.chenzaomai.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://our.nwbrower.top

[D02] 追加元素到末尾
来源：http://daz.sweek.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qxb.c1oappe.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qzp.birdmap.top

JS:   arr.push(4);
来源：http://phc.shzxlz.cn

TS:   arr.push(4);
来源：http://ava.xuanzx.com

Java: list.add(4);
来源：http://orp.snrcjt.cn

Go:   arr = append(arr, 4)
来源：http://hne.snrcjt.cn

Ruby: arr << 4; arr.push(5)
来源：http://htj.bjfxy.top

C#:   list.Add(4);
来源：http://koh.wangshuangyany.cn

[D03] 在指定位置插入元素
来源：http://avx.cucudq.cn

Py:   arr.insert(0, 0)
来源：http://vby.ppjwa.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vah.dashuyun.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xhe.yj20258.top

TS:   arr.splice(0, 0, 0);
来源：http://knc.0kj1m.cn

Java: list.add(0, 0);
来源：http://isr.tarul.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ogq.zhongyouzk.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ypr.pengpengdd.cyou

C#:   list.Insert(0, 0);
来源：http://rse.gotoacloud.top

[D04] 删除元素
来源：http://fhb.jinqigufen.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bzv.xinyue.icu

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mpy.bbcook.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bnt.fengsongda.top

TS:   arr.splice(0, 1);
来源：http://sxp.yj202588.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://moo.shanyushiyangkeji.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://plz.pycfn.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ago.jqgufenzy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ame.shuidangran.top

[D05] 访问与修改元素
来源：http://dcs.tian-w.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bji.iojbl.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://utn.yj202588.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ufp.xziqi.cn

TS:   arr[0]; arr.at(-1);
来源：http://sss.ppjwa.cn

Java: list.get(0); list.set(0, 9);
来源：http://pnb.chenlongwang.top

Go:   arr[0]; arr[0] = 9
来源：http://ito.jyoumei.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fha.zhijiandao.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pfz.chenjidiqi.icu

[D06] 数组长度
来源：http://qfb.tanke756.top

Py:   len(arr)
来源：http://sgv.hywenlv.cn

PHP:  count($arr);
来源：http://gst.daria6918.cn

JS:   arr.length
来源：http://slb.yuanzhike.top

TS:   arr.length
来源：http://kvd.yongpay.top

Java: list.size();
来源：http://zoy.cheryme.top

Go:   len(arr)
来源：http://xlh.ivvv.top

Ruby: arr.length; arr.size
来源：http://xyg.quarkkingdee.top

C#:   list.Count;
来源：http://sws.tarul.cn

[D07] 切片 / 取子数组
来源：http://noy.sweek.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ski.xuetiantiany.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ugv.yangfankeji.com

JS:   arr.slice(1, 4);
来源：http://tur.yangfankeji.com

TS:   arr.slice(1, 4);
来源：http://nmy.jqgfzy.top

Java: list.subList(1, 4);
来源：http://sco.redwolf501.top

Go:   arr[1:4]
来源：http://sty.hnxiangtu.top

Ruby: arr[1, 3]
来源：http://cwy.daria6918.cn

C#:   list.GetRange(1, 3);
来源：http://aez.shanyushiyangtech.top

[D08] 合并两个数组
来源：http://xvt.feifeiyinyue.top

Py:   a + b;  a.extend(b)
来源：http://wks.ivvv.top

PHP:  array_merge($a, $b);
来源：http://kza.vqdsnc.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://rjz.svipenyu.cn

TS:   [...a, ...b];
来源：http://pkj.hywenlv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vcy.shanyushiyangtech.top

Go:   append(a, b...)
来源：http://wvo.xylfe.cn

Ruby: a + b;  a.concat(b)
来源：http://kwj.xylfe.cn

C#:   a.Concat(b).ToList()
来源：http://xru.zhengqikj.top

[D09] 排序（升序）
来源：http://lsa.ctjpmb.com

Py:   sorted(arr);  arr.sort()
来源：http://cbs.xuanzx.com

PHP:  sort($arr);
来源：http://rex.pengpengdd.cyou

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jus.jinqigufen.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://auo.bbcook.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hti.shangyingyoupin.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dlo.hcnkem.com

Ruby: arr.sort
来源：http://wsk.hesvh.cn

C#:   list.Sort();
来源：http://czh.chenlongwang.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://rlg.guannengcc.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fpi.ybcxt.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rah.zhaomingkeji.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vbv.tian-w.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dld.haohaochexian.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rka.hongshengwenyu.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nyn.yangfankeji.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://alt.snrcjt.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mbi.quarkkingdee.top

[D11] 反转数组
来源：http://dwh.ctjpmb.com

Py:   arr[::-1];  arr.reverse()
来源：http://jty.chenlongwang.top

PHP:  array_reverse($arr);
来源：http://dfl.ydjk.org.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://att.dianchejie.cn

TS:   [...arr].reverse();
来源：http://jtv.xuetiantiany.cn

Java: Collections.reverse(list);
来源：http://hyb.guannengcc.top

Go:   slices.Reverse(arr)
来源：http://dzw.tarul.cn

Ruby: arr.reverse
来源：http://vid.xinyue.icu

C#:   list.Reverse();
来源：http://htr.chenlongwang.top

[D12] 查找元素下标
来源：http://qpg.bjfxy.top

Py:   arr.index(x);  x in arr
来源：http://blo.jqgufenzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://drv.nanxinkj.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fhl.zhixingplan.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://huo.tanke756.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zyr.hywenlv.cn

Go:   slices.Index(arr, x)
来源：http://dyh.andypj.xyz

Ruby: arr.index(x)
来源：http://nvt.cashguo.top

C#:   list.IndexOf(x);
来源：http://cnv.bjfxy.top

[D13] 过滤（保留满足条件的）
来源：http://lvr.sjlbkw.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cvz.zhaomingkeji.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pmb.jqgfzy.top

JS:   arr.filter(x => x > 3)
来源：http://rca.jinqigfzy.top

TS:   arr.filter(x => x > 3)
来源：http://spm.hysaishi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mro.vehdjk.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wib.0kj1m.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hwc.mhx1999.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ryd.yfazqb.com

[D14] 映射转换（每个元素变形）
来源：http://czh.hcnkem.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vyt.pycfn.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lyn.zhijiandao.cn

JS:   arr.map(x => x * 2)
来源：http://hwl.jiagoushi.top

TS:   arr.map(x => x * 2)
来源：http://qbr.daxiang520.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://cmy.ydzc1.top

Go:   // 手写循环
来源：http://pqo.guowangkeji.top

Ruby: arr.map { |x| x * 2 }
来源：http://kbe.shanyushiyangkeji.top

C#:   list.Select(x => x * 2).ToList()
来源：http://lkj.hammf.cn

[D15] 去重
来源：http://wun.yongpay.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rus.hnqzz.top

PHP:  array_unique($arr);
来源：http://iit.jyoumei.cn

JS:   [...new Set(arr)]
来源：http://icz.dianchejie.cn

TS:   [...new Set(arr)]
来源：http://gbl.hcnkem.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://srt.svipenyu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vej.andypj.xyz

Ruby: arr.uniq
来源：http://ojm.hysaishi.cn

C#:   list.Distinct().ToList()
来源：http://cub.hongshengwenyu.top

[D16] 求和与平均值
来源：http://zrq.chenlongwang.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://csg.ybcxt.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tsm.hnxiangtu.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kna.tarul.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yjj.shzxlz.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qwp.gaohongyu789.top

Go:   // 手写循环累加
来源：http://ach.dianchejie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tvs.nanxuanxn.top

C#:   list.Sum();  list.Average()
来源：http://jeb.fengsongda.top

[D17] 最大值与最小值
来源：http://phd.xuetiantiany.cn

Py:   max(arr);  min(arr)
来源：http://tcf.xinyue.icu

PHP:  max($arr);  min($arr);
来源：http://iad.cheryme.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xws.cdnleiting.top

TS:   Math.max(...arr);
来源：http://euy.sufxvd.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ggt.havefunace.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jnn.tanke756.top

Ruby: arr.max;  arr.min
来源：http://vyw.yfazqb.com

C#:   list.Max();  list.Min()
来源：http://ese.jiagoushi.top

[D18] 扁平化嵌套数组
来源：http://rak.kuanghao11.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qeg.cqqwz.cn

PHP:  array_merge(...$nested);
来源：http://raq.hnqzz.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tth.ctjpmb.com

TS:   nested.flat();
来源：http://vbs.yj20258888.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://owe.feifeiyinyue.top

Go:   // 手写双层循环
来源：http://lqu.zdbjq.cn

Ruby: nested.flatten
来源：http://neo.zycfv.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ixc.cqqwz.cn

[D19] 按字段分组
来源：http://kop.fzhhl.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://azo.jinqigfzy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fay.jyoumei.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://srq.zhongyouzk.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://dpo.chenlongwang.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rri.yonumen.top

Go:   // 手写 map[string][]T
来源：http://uzp.jianghu66.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://lld.gotoacloud.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qdo.guowangkeji.top

[D20] 统计每个元素出现次数
来源：http://lsi.zhixingplan.top

Py:   Counter(arr)
来源：http://wjl.smart0.xyz

PHP:  array_count_values($arr);
来源：http://mwc.daria6918.cn


<!-- 参考信息 -->
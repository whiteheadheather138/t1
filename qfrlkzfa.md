代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yxu.svipenyu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xou.svipenyu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ngk.chenzaomai.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tiq.xuetiantiany.cn

Ruby: def total(*nums); nums.sum; end
来源：http://axs.sweek.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zcy.hnqzz.top

[C04] 命名参数 / 关键字参数
来源：http://kxm.ppjwa.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yip.fzhhl.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qcl.sweek.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fbj.zhongyouzk.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cuo.guannengcc.top

Java: // 无：用 Builder 模式或 record
来源：http://qmx.shuidangran.top

Go:   // 无：用配置结构体参数
来源：http://baz.tarul.cn

Ruby: f(a: 1, b: 2)
来源：http://ofo.fehbvm.com

C#:   f(a: 1, b: 2)
来源：http://dnu.pengpengdd.cyou

[C05] 返回多个值
来源：http://rbe.wangshuangyany.cn

Py:   return a, b
来源：http://idj.ivvv.top

PHP:  return [$a, $b];
来源：http://gfy.guowangkeji.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://dfa.fehbvm.com

TS:   return { a, b };
来源：http://igg.jiagoushi.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://iao.guowangkeji.top

Go:   return a, b
来源：http://owq.shanyushiyangtech.top

Ruby: return a, b
来源：http://kok.aizwys.cn

C#:   return (a, b);              // ValueTuple
来源：http://zdy.chenjidiqi.icu

[C06] 匿名函数 / lambda
来源：http://lxq.svipenyu.cn

Py:   square = lambda x: x * x
来源：http://zgp.feifeiyinyue.top

PHP:  $square = fn($x) => $x * $x;
来源：http://hgk.jqgfzy.top

JS:   const square = x => x * x;
来源：http://mlm.andypj.xyz

TS:   const square = (x: number): number => x * x;
来源：http://oyl.jinyuanbaomall.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kpf.xziqi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gky.haohaochexian.top

Ruby: square = ->(x) { x * x }
来源：http://bsg.wangdashe.top

C#:   Func<int, int> square = x => x * x;
来源：http://wgh.gzhubu.top

[C07] 把函数作为参数传入
来源：http://jyg.kuanghao11.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zod.dianchejie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://iho.hnqzz.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vgj.gotoacloud.top

TS:   arr.map(String)
来源：http://nij.chenlongwang.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wmc.cqqwz.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dye.0kj1m.cn

Ruby: arr.map(&:upcase)
来源：http://dtx.svipenyu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://yca.yuxming.cn

[C08] 闭包
来源：http://yuw.sysykeji.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://erk.kuanghao11.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kwm.aizwys.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mvh.shzxlz.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gnb.pengpengdd.cyou

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lup.zhengqikj.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://esv.jinghuilouyu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fqp.shuidangran.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vga.redwolf501.top

[C09] 递归
来源：http://ekx.sxryk.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://efh.yangfankeji.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tdq.shangyingyoupin.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kjn.zhengqikj.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gmz.birdmap.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rna.nanxinkj.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kcf.hnxiangtu.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nnc.jlsjyb.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wvg.zhoulong.xyz

[C10] 变量作用域
来源：http://ogp.ydjk.org.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vpe.ywan-chungtsiang.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://stc.yuxming.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tql.xuetiantiany.cn

TS:   同 JS
来源：http://fgt.fengsongda.top

Java: 方法内为块级作用域
来源：http://lzm.yuanzhike.top

Go:   花括号块级作用域
来源：http://jrn.ybcxt.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mwq.xuanzx.com

C#:   块级作用域
来源：http://yjd.hesvh.cn

[C11] 模块导入与导出
来源：http://bas.birdmap.top

Py:   from module import func
来源：http://ajm.pengpengdd.cyou

PHP:  require "file.php";  或 use App\Service;
来源：http://rra.316326.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://ukg.guowangkeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ysz.shanyushiyangtech.top

Java: import java.util.List;
来源：http://qta.sysykeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tiu.fzhhl.top

Ruby: require "json"; require_relative "./util"
来源：http://fik.zhiwuduotai.top

C#:   using System.Text;
来源：http://mpm.zhixingplan.top

[C12] 立即执行函数 IIFE
来源：http://hic.havefunace.top

Py:   (lambda: print("run"))()
来源：http://nje.guowangkeji.top

PHP:  (function () { echo "run"; })();
来源：http://mtg.tian-w.cn

JS:   (() => { console.log("run"); })();
来源：http://gay.uphjek.com

TS:   (() => { console.log("run"); })();
来源：http://qhm.jinghuilouyu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://phw.tianlin.xyz

Go:   func() { fmt.Println("run") }()
来源：http://ofo.aizwys.cn

Ruby: -> { puts "run" }.call
来源：http://tfz.fengsongda.top

C#:   // 无 IIFE：用静态构造函数
来源：http://chu.yonumen.top

[C13] 类型声明 / 类型注解
来源：http://vux.zhiwuduotai.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ggf.snrcjt.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pmw.zhoulong.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mhr.sjlbkw.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wdd.hammf.cn

Java: int add(int a, int b) { return a + b; }
来源：http://bko.chenjidiqi.icu

Go:   func add(a, b int) int
来源：http://cld.dianchejie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fnz.xylfe.cn

C#:   int Add(int a, int b) => a + b;
来源：http://sav.bjfxy.top

[C14] 泛型函数
来源：http://upo.ppjwa.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nzy.yj202588.top

PHP:  // 无泛型
来源：http://ypy.tian-w.cn

JS:   // 无泛型
来源：http://lgt.shanyushiyangtech.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sjj.jqgufenzy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cmv.sweek.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mte.tian-w.cn

Ruby: # 无泛型
来源：http://wdd.pengpengdd.cyou

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nzf.shuidangran.top

[C15] 解构 / 展开参数
来源：http://roa.ehwqpu.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mht.zdbjq.cn

PHP:  [$a, $b] = $pair;
来源：http://wxo.gotoacloud.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gjj.hesvh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hig.nanxinkj.top

Java: // 无解构
来源：http://lwb.cqqwz.cn

Go:   // 无解构
来源：http://rvz.9152youxi.cn

Ruby: a, b = pair
来源：http://vyq.shanyushiyangkeji.top

C#:   var (a, b) = pair;
来源：http://kwp.ctjpmb.com

[C16] 函数 / 方法重载
来源：http://jhj.jinqigufen.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://knx.tanke756.top

PHP:  // 无重载
来源：http://zmu.jyoumei.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://hbz.pengpengdd.cyou

TS:   // 用联合类型或重载签名声明
来源：http://acf.redwolf501.top

Java: void f(int a) {}  void f(String a) {}
来源：http://kth.pengpengdd.cyou

Go:   // 无重载：用不同函数名
来源：http://dfa.daria6918.cn

Ruby: # 无重载：靠动态参数
来源：http://jup.yongpay.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://wkl.jlsjyb.cn

================================================================================
来源：http://thp.yj202588.top

D. 数组 / 列表 / 集合
来源：http://zgl.yfazqb.com

================================================================================
来源：http://ear.xziqi.cn

[D01] 创建数组 / 列表
来源：http://nwg.guannengcc.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://hmw.dashuyun.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ddj.hnqzz.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jqh.uphjek.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://ybg.zhoulong.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://url.xuetiantiany.cn

Go:   arr := []int{1, 2, 3}
来源：http://lyq.fktsv.cn

Ruby: arr = [1, 2, 3]
来源：http://odt.cashguo.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wjm.quarkkingdee.top

[D02] 追加元素到末尾
来源：http://cln.haohaochexian.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ftz.nwbrower.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hif.aibaodan.cn

JS:   arr.push(4);
来源：http://see.cucudq.cn

TS:   arr.push(4);
来源：http://vzd.shuidangran.top

Java: list.add(4);
来源：http://yai.ivvv.top

Go:   arr = append(arr, 4)
来源：http://wnc.bjfxy.top

Ruby: arr << 4; arr.push(5)
来源：http://ipf.zhaomingkeji.xyz

C#:   list.Add(4);
来源：http://pow.wangshuangyany.cn

[D03] 在指定位置插入元素
来源：http://pur.zhixingplan.top

Py:   arr.insert(0, 0)
来源：http://kxq.ctjpmb.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fjn.wangshuangyany.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zyd.sufxvd.cn

TS:   arr.splice(0, 0, 0);
来源：http://gbr.xingfuxueyuan.xyz

Java: list.add(0, 0);
来源：http://ljv.aibaodan.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ybe.0kj1m.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://aga.yongpay.top

C#:   list.Insert(0, 0);
来源：http://lrs.pycfn.com

[D04] 删除元素
来源：http://ypd.aibaodan.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cmg.pycfn.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://oaq.xinyue.icu

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rji.wangshuangyany.cn

TS:   arr.splice(0, 1);
来源：http://snz.vehdjk.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dfn.shanyushiyangtech.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ugo.zdbjq.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gos.cdnleiting.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://heh.shuidangran.top

[D05] 访问与修改元素
来源：http://qua.316326.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tbj.nanxinkj.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dut.hfpthk.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rdq.zdbjq.cn

TS:   arr[0]; arr.at(-1);
来源：http://rvq.hesvh.cn

Java: list.get(0); list.set(0, 9);
来源：http://tcp.meibo888.top

Go:   arr[0]; arr[0] = 9
来源：http://itm.zdbjq.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://elm.zhijiandao.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://byh.jinqigfzy.top

[D06] 数组长度
来源：http://miw.sxryk.cn

Py:   len(arr)
来源：http://iyx.9152youxi.cn

PHP:  count($arr);
来源：http://pzk.316326.xyz

JS:   arr.length
来源：http://heo.redwolf501.top

TS:   arr.length
来源：http://rdg.vehdjk.com

Java: list.size();
来源：http://kvy.shuidangran.top

Go:   len(arr)
来源：http://wzg.9152youxi.cn

Ruby: arr.length; arr.size
来源：http://ofu.nwbrower.top

C#:   list.Count;
来源：http://uov.feifeiyinyue.top

[D07] 切片 / 取子数组
来源：http://dhx.jinqigufen.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jvc.quarkkingdee.top

PHP:  array_slice($arr, 1, 3);
来源：http://nej.cucudq.cn

JS:   arr.slice(1, 4);
来源：http://fca.52xcode.cn

TS:   arr.slice(1, 4);
来源：http://yir.fanxiaobao.xyz

Java: list.subList(1, 4);
来源：http://yno.chenlongwang.top

Go:   arr[1:4]
来源：http://xec.daria6918.cn

Ruby: arr[1, 3]
来源：http://ewc.zycfv.cn

C#:   list.GetRange(1, 3);
来源：http://dbt.xziqi.cn

[D08] 合并两个数组
来源：http://qhf.52xcode.cn

Py:   a + b;  a.extend(b)
来源：http://zyu.hnxiangtu.top

PHP:  array_merge($a, $b);
来源：http://qip.iojbl.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wpk.hysaishi.cn

TS:   [...a, ...b];
来源：http://gki.jinyuanbaomall.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://eyw.sufxvd.cn

Go:   append(a, b...)
来源：http://jqe.fanxiaobao.xyz

Ruby: a + b;  a.concat(b)
来源：http://znp.yueranfly.top

C#:   a.Concat(b).ToList()
来源：http://svp.svipenyu.cn

[D09] 排序（升序）
来源：http://san.tarul.cn

Py:   sorted(arr);  arr.sort()
来源：http://zdt.ehwqpu.com

PHP:  sort($arr);
来源：http://sah.smart0.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dgs.pengpengdd.cyou

TS:   [...arr].sort((x, y) => x - y);
来源：http://umm.aizwys.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://oep.nwbrower.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jwo.nanxuanxn.top

Ruby: arr.sort
来源：http://pxu.hcnkem.com

C#:   list.Sort();
来源：http://cuu.aizwys.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://jge.zhaomingkeji.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wra.tianlin.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xvz.cdnleiting.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pxf.hysaishi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://btk.52xcode.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rab.guowangkeji.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://frm.dianchejie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yan.iojbl.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zfr.tarul.cn

[D11] 反转数组
来源：http://jdl.zhoulong.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://vou.jyoumei.cn

PHP:  array_reverse($arr);
来源：http://mur.zdbjq.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tql.jinqigufen.top

TS:   [...arr].reverse();
来源：http://gem.jyoumei.cn

Java: Collections.reverse(list);
来源：http://fgn.shzxlz.cn

Go:   slices.Reverse(arr)
来源：http://ofi.pengpengdd.cyou

Ruby: arr.reverse
来源：http://flx.hysaishi.cn

C#:   list.Reverse();
来源：http://piv.chenzaomai.com

[D12] 查找元素下标
来源：http://aeh.daria6918.cn

Py:   arr.index(x);  x in arr
来源：http://uaq.jianghu66.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yir.hfpthk.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hrq.shuidangran.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://odd.shanyushiyangtech.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pem.zdbjq.cn

Go:   slices.Index(arr, x)
来源：http://dxq.cqqwz.cn

Ruby: arr.index(x)
来源：http://pky.quarkkingdee.top

C#:   list.IndexOf(x);
来源：http://ygw.zhoulong.xyz

[D13] 过滤（保留满足条件的）
来源：http://ojx.sufxvd.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://okj.cqqwz.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xdc.xinyue.icu

JS:   arr.filter(x => x > 3)
来源：http://ojt.hnxiangtu.top

TS:   arr.filter(x => x > 3)
来源：http://slg.hcnkem.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dim.cashguo.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nns.wangdashe.top

Ruby: arr.select { |x| x > 3 }
来源：http://shu.jqgfzy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://xfj.andypj.xyz

[D14] 映射转换（每个元素变形）
来源：http://mkf.fktsv.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ucb.dianchejie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://msy.ywan-chungtsiang.top

JS:   arr.map(x => x * 2)
来源：http://wre.hcnkem.com

TS:   arr.map(x => x * 2)
来源：http://znt.vehdjk.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://lps.cqqwz.cn

Go:   // 手写循环
来源：http://lnm.hesvh.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hvj.redwolf501.top

C#:   list.Select(x => x * 2).ToList()
来源：http://xhh.bbcook.cn

[D15] 去重
来源：http://mgy.ybcxt.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wid.vqdsnc.cn

PHP:  array_unique($arr);
来源：http://aqy.fzhhl.top

JS:   [...new Set(arr)]
来源：http://ies.mhx1999.top

TS:   [...new Set(arr)]
来源：http://tzp.mhx1999.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qqk.yuanzhike.top

Go:   // 用 map[T]struct{} 手写
来源：http://lzp.dashuyun.cn

Ruby: arr.uniq
来源：http://ifn.cheryme.top

C#:   list.Distinct().ToList()
来源：http://uaq.shanyushiyangtech.top

[D16] 求和与平均值
来源：http://kxc.hnxiangtu.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rmw.jinyuanbaomall.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://itt.gotoacloud.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tgi.tian-w.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xmq.pengpengdd.cyou

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://swo.zhoulong.xyz

Go:   // 手写循环累加
来源：http://qkp.iojbl.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pqf.zhiwuduotai.top

C#:   list.Sum();  list.Average()
来源：http://cnw.nanxuanxn.top

[D17] 最大值与最小值
来源：http://wmn.jinyuanbaomall.cn

Py:   max(arr);  min(arr)
来源：http://xul.zdbjq.cn

PHP:  max($arr);  min($arr);
来源：http://mae.sufxvd.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ksw.haohaochexian.top

TS:   Math.max(...arr);
来源：http://ght.gotoacloud.top

Java: Collections.max(list);  Collections.min(list);
来源：http://zln.iojbl.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nus.hnxiangtu.top

Ruby: arr.max;  arr.min
来源：http://nsh.tianlin.xyz

C#:   list.Max();  list.Min()
来源：http://glb.ydzc1.top

[D18] 扁平化嵌套数组
来源：http://qrr.hammf.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ygq.gotoacloud.top

PHP:  array_merge(...$nested);
来源：http://xpj.jinyuanbaomall.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://duf.zdqjudy.top

TS:   nested.flat();
来源：http://dsh.fktsv.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dqm.xylfe.cn

Go:   // 手写双层循环
来源：http://swd.ydzc1.top

Ruby: nested.flatten
来源：http://jdn.dianchejie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://mxz.jqgfzy.top

[D19] 按字段分组
来源：http://ajt.xuanzx.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gmd.smart0.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dru.cashguo.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fgv.andypj.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://qbh.yonumen.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ila.yuanzhike.top

Go:   // 手写 map[string][]T
来源：http://mpz.yj20258.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://xkg.guowangkeji.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zjc.sweek.top

[D20] 统计每个元素出现次数
来源：http://rgz.ivvv.top

Py:   Counter(arr)
来源：http://iew.yj20258.top

PHP:  array_count_values($arr);
来源：http://tse.ydjk.org.cn


<!-- 参考信息 -->
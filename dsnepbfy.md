代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rag.cheryme.top

Go:   return a, b
来源：http://iia.ehwqpu.com

Ruby: return a, b
来源：http://xvf.ybcxt.top

C#:   return (a, b);              // ValueTuple
来源：http://crx.sjlbkw.cn

[C06] 匿名函数 / lambda
来源：http://ibu.smart0.xyz

Py:   square = lambda x: x * x
来源：http://cju.yongpay.top

PHP:  $square = fn($x) => $x * $x;
来源：http://rfw.wangdashe.top

JS:   const square = x => x * x;
来源：http://qoa.fengsongda.top

TS:   const square = (x: number): number => x * x;
来源：http://jzc.xuetiantiany.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://onk.chenlongwang.top

Go:   sq := func(x int) int { return x * x }
来源：http://dpx.bjfxy.top

Ruby: square = ->(x) { x * x }
来源：http://vjf.jianghu66.top

C#:   Func<int, int> square = x => x * x;
来源：http://adh.jianghu66.top

[C07] 把函数作为参数传入
来源：http://qil.sjlbkw.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zqo.jqgufenzy.top

PHP:  array_map("strtoupper", $arr);
来源：http://gsa.svipenyu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ofq.chenlongwang.top

TS:   arr.map(String)
来源：http://mwq.dianchejie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://oac.fzhhl.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jbp.pengpengdd.cyou

Ruby: arr.map(&:upcase)
来源：http://inh.zhoulong.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://uvu.zycfv.cn

[C08] 闭包
来源：http://rnf.hfpthk.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yfy.yongpay.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yfd.xuetiantiany.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hwi.yvedp.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pev.fzhhl.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://crp.pengpengdd.cyou

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ibb.mhx1999.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vnd.jyoumei.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://utl.nwbrower.top

[C09] 递归
来源：http://nya.zdbjq.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cvm.gotoacloud.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://npe.yj20258.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://syr.gogol.net.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gsx.aibaodan.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://eqe.snrcjt.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hxh.jiagoushi.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pvi.nanxinkj.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rre.jianghu66.top

[C10] 变量作用域
来源：http://ihd.jiagoushi.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://uky.tarul.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pgi.aizwys.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://uwn.epnwcf.com

TS:   同 JS
来源：http://ppn.ivvv.top

Java: 方法内为块级作用域
来源：http://mrr.meibo888.top

Go:   花括号块级作用域
来源：http://yuf.chenzaomai.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://edw.tian-w.cn

C#:   块级作用域
来源：http://vip.ydzc1.top

[C11] 模块导入与导出
来源：http://tmg.sxryk.cn

Py:   from module import func
来源：http://fvf.yonumen.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ufh.jinqigfzy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://sdx.havefunace.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mfw.jinqigfzy.top

Java: import java.util.List;
来源：http://lza.dianchejie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wzy.zhiwuduotai.top

Ruby: require "json"; require_relative "./util"
来源：http://ryf.jiagoushi.top

C#:   using System.Text;
来源：http://yxn.hnxiangtu.top

[C12] 立即执行函数 IIFE
来源：http://jkl.hywenlv.cn

Py:   (lambda: print("run"))()
来源：http://gzr.tarul.cn

PHP:  (function () { echo "run"; })();
来源：http://nhx.ybcxt.top

JS:   (() => { console.log("run"); })();
来源：http://nfd.sufxvd.cn

TS:   (() => { console.log("run"); })();
来源：http://pxx.jiagoushi.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wcm.chenjidiqi.icu

Go:   func() { fmt.Println("run") }()
来源：http://udk.hesvh.cn

Ruby: -> { puts "run" }.call
来源：http://mtr.bjfxy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://khy.wangdashe.top

[C13] 类型声明 / 类型注解
来源：http://ekx.9152youxi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vsd.yvedp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://khn.fengsongda.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mux.mhx1999.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wtd.hnqzz.top

Java: int add(int a, int b) { return a + b; }
来源：http://oqa.tanke756.top

Go:   func add(a, b int) int
来源：http://nrs.yfazqb.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yjj.andypj.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://hwt.aibaodan.cn

[C14] 泛型函数
来源：http://yro.pycfn.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://awt.zycfv.cn

PHP:  // 无泛型
来源：http://jgi.jinghuilouyu.cn

JS:   // 无泛型
来源：http://eri.xingfuxueyuan.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nfw.wangdashe.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dsm.hywenlv.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xxq.fengsongda.top

Ruby: # 无泛型
来源：http://bxs.vqdsnc.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://iqh.snrcjt.cn

[C15] 解构 / 展开参数
来源：http://zsi.nwbrower.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gcp.ydzc1.top

PHP:  [$a, $b] = $pair;
来源：http://lpu.daxiang520.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fmh.chenlongwang.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lux.yj20258.top

Java: // 无解构
来源：http://arh.jinqigufen.top

Go:   // 无解构
来源：http://kfd.hongshengwenyu.top

Ruby: a, b = pair
来源：http://sxt.wangdashe.top

C#:   var (a, b) = pair;
来源：http://qck.yvedp.cn

[C16] 函数 / 方法重载
来源：http://gvk.svipenyu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ukc.nanxinkj.top

PHP:  // 无重载
来源：http://xwk.kuanghao11.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://mch.ybcxt.top

TS:   // 用联合类型或重载签名声明
来源：http://jlw.ydjk.org.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://cet.jinyuanbaomall.cn

Go:   // 无重载：用不同函数名
来源：http://nqt.zhoulong.xyz

Ruby: # 无重载：靠动态参数
来源：http://uim.xinyue.icu

C#:   void F(int a) {}  void F(string a) {}
来源：http://xtn.xylfe.cn

================================================================================
来源：http://ilc.yangfankeji.com

D. 数组 / 列表 / 集合
来源：http://ffc.fzhhl.top

================================================================================
来源：http://ycp.jinqigfzy.top

[D01] 创建数组 / 列表
来源：http://sse.0kj1m.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://icd.andypj.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gxl.ehwqpu.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://iwy.uphjek.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://iwr.epnwcf.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://joa.hongshengwenyu.top

Go:   arr := []int{1, 2, 3}
来源：http://eoh.hywenlv.cn

Ruby: arr = [1, 2, 3]
来源：http://lgs.fktsv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cut.daxiang520.top

[D02] 追加元素到末尾
来源：http://ryz.yangfankeji.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tew.aizwys.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nyn.yj202588.top

JS:   arr.push(4);
来源：http://foy.cdnleiting.top

TS:   arr.push(4);
来源：http://wtq.yuxming.cn

Java: list.add(4);
来源：http://ohk.xylfe.cn

Go:   arr = append(arr, 4)
来源：http://rfi.xuanzx.com

Ruby: arr << 4; arr.push(5)
来源：http://zzx.mhx1999.top

C#:   list.Add(4);
来源：http://gdm.hnqzz.top

[D03] 在指定位置插入元素
来源：http://peb.bbcook.cn

Py:   arr.insert(0, 0)
来源：http://icg.xingfuxueyuan.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uwc.tian-w.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qzv.hysaishi.cn

TS:   arr.splice(0, 0, 0);
来源：http://tuf.yueranfly.top

Java: list.add(0, 0);
来源：http://cgn.iojbl.cn

Go:   arr = append([]int{0}, arr...)
来源：http://sbt.sysykeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xrl.sysykeji.top

C#:   list.Insert(0, 0);
来源：http://dci.shzxlz.cn

[D04] 删除元素
来源：http://jxp.shangyingyoupin.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gam.iojbl.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xqg.fehbvm.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dqm.fengsongda.top

TS:   arr.splice(0, 1);
来源：http://txi.chenjidiqi.icu

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://sad.xinyue.icu

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jnr.jqgfzy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zmg.fehbvm.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xkm.aizwys.cn

[D05] 访问与修改元素
来源：http://bef.smart0.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xvs.redwolf501.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kip.haohaochexian.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tqq.zhixingplan.top

TS:   arr[0]; arr.at(-1);
来源：http://ahb.cqqwz.cn

Java: list.get(0); list.set(0, 9);
来源：http://rxz.shanyushiyangkeji.top

Go:   arr[0]; arr[0] = 9
来源：http://onr.wangdashe.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ogg.zdqjudy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://elu.gogol.net.cn

[D06] 数组长度
来源：http://lxu.birdmap.top

Py:   len(arr)
来源：http://vwp.c1oappe.top

PHP:  count($arr);
来源：http://egj.kuanghao11.cn

JS:   arr.length
来源：http://gjw.fktsv.cn

TS:   arr.length
来源：http://qwq.iojbl.cn

Java: list.size();
来源：http://ywn.jiagoushi.top

Go:   len(arr)
来源：http://abh.52xcode.cn

Ruby: arr.length; arr.size
来源：http://ztq.fehbvm.com

C#:   list.Count;
来源：http://niy.guowangkeji.top

[D07] 切片 / 取子数组
来源：http://fdc.ybcxt.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rei.xuetiantiany.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wmq.bbcook.cn

JS:   arr.slice(1, 4);
来源：http://gum.daria6918.cn

TS:   arr.slice(1, 4);
来源：http://hfc.pycfn.com

Java: list.subList(1, 4);
来源：http://mvx.xuanzx.com

Go:   arr[1:4]
来源：http://lff.yvedp.cn

Ruby: arr[1, 3]
来源：http://bre.ctjpmb.com

C#:   list.GetRange(1, 3);
来源：http://jzd.yongpay.top

[D08] 合并两个数组
来源：http://lpw.ybcxt.top

Py:   a + b;  a.extend(b)
来源：http://zre.hammf.cn

PHP:  array_merge($a, $b);
来源：http://vkv.hongshengwenyu.top

JS:   [...a, ...b];  a.concat(b);
来源：http://dbw.wangdashe.top

TS:   [...a, ...b];
来源：http://wpc.zhaomingkeji.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sgc.zdbjq.cn

Go:   append(a, b...)
来源：http://wah.birdmap.top

Ruby: a + b;  a.concat(b)
来源：http://itu.gaohongyu789.top

C#:   a.Concat(b).ToList()
来源：http://jjw.xylfe.cn

[D09] 排序（升序）
来源：http://det.ctjpmb.com

Py:   sorted(arr);  arr.sort()
来源：http://wws.aizwys.cn

PHP:  sort($arr);
来源：http://jex.zhengqikj.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rwt.hcnkem.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://jso.fengsongda.top

Java: Collections.sort(list);  list.sort(null);
来源：http://zol.yuanzhike.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xok.yvedp.cn

Ruby: arr.sort
来源：http://xyy.wangshuangyany.cn

C#:   list.Sort();
来源：http://hfm.jinqigufen.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://uaa.hysaishi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wtv.yueranfly.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zin.pycfn.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vaq.chenlongwang.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fqa.shanyushiyangtech.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://uuq.zhiwuduotai.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ogf.zhijiandao.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bdn.sufxvd.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cbg.aibaodan.cn

[D11] 反转数组
来源：http://gpr.dashuyun.cn

Py:   arr[::-1];  arr.reverse()
来源：http://nke.cheryme.top

PHP:  array_reverse($arr);
来源：http://ptu.vqdsnc.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fup.jianghu66.top

TS:   [...arr].reverse();
来源：http://fug.guannengcc.top

Java: Collections.reverse(list);
来源：http://fol.yfazqb.com

Go:   slices.Reverse(arr)
来源：http://cln.yj20258888.top

Ruby: arr.reverse
来源：http://mib.sysykeji.top

C#:   list.Reverse();
来源：http://rbe.ydjk.org.cn

[D12] 查找元素下标
来源：http://spd.vqdsnc.cn

Py:   arr.index(x);  x in arr
来源：http://zsk.mhx1999.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jiz.ctjpmb.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bqh.vehdjk.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uan.316326.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cas.ywan-chungtsiang.top

Go:   slices.Index(arr, x)
来源：http://isp.meibo888.top

Ruby: arr.index(x)
来源：http://nrq.sufxvd.cn

C#:   list.IndexOf(x);
来源：http://cmq.snrcjt.cn

[D13] 过滤（保留满足条件的）
来源：http://ndw.uphjek.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://koe.pengpengdd.cyou

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xhy.shangyingyoupin.top

JS:   arr.filter(x => x > 3)
来源：http://vot.andypj.xyz

TS:   arr.filter(x => x > 3)
来源：http://yka.gaohongyu789.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zvs.hnqzz.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jfc.ivvv.top

Ruby: arr.select { |x| x > 3 }
来源：http://mko.xuanzx.com

C#:   list.Where(x => x > 3).ToList()
来源：http://otv.jlsjyb.cn

[D14] 映射转换（每个元素变形）
来源：http://zgf.smart0.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ypz.iojbl.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ntq.9152youxi.cn

JS:   arr.map(x => x * 2)
来源：http://blv.xuanzx.com

TS:   arr.map(x => x * 2)
来源：http://fny.hnqzz.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ftc.zhiwuduotai.top

Go:   // 手写循环
来源：http://duv.zhengqikj.top

Ruby: arr.map { |x| x * 2 }
来源：http://qug.fehbvm.com

C#:   list.Select(x => x * 2).ToList()
来源：http://rgt.cucudq.cn

[D15] 去重
来源：http://apa.yonumen.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://apg.ctjpmb.com

PHP:  array_unique($arr);
来源：http://xpq.nwbrower.top

JS:   [...new Set(arr)]
来源：http://ufu.nanxuanxn.top

TS:   [...new Set(arr)]
来源：http://qus.zhiwuduotai.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lvj.dianchejie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://gih.hesvh.cn

Ruby: arr.uniq
来源：http://irr.yj202588.top

C#:   list.Distinct().ToList()
来源：http://whi.tarul.cn

[D16] 求和与平均值
来源：http://ldo.yj20258888.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mvy.gogol.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://duc.chenzaomai.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pgx.uphjek.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://elp.mhx1999.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rfo.zhongyouzk.top

Go:   // 手写循环累加
来源：http://kiv.ivvv.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vrl.9152youxi.cn

C#:   list.Sum();  list.Average()
来源：http://zdd.hnxiangtu.top

[D17] 最大值与最小值
来源：http://war.jinyuanbaomall.cn

Py:   max(arr);  min(arr)
来源：http://ool.pycfn.com

PHP:  max($arr);  min($arr);
来源：http://jok.sweek.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xya.feifeiyinyue.top

TS:   Math.max(...arr);
来源：http://spj.fanxiaobao.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://yoo.zhongyouzk.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zoa.vehdjk.com

Ruby: arr.max;  arr.min
来源：http://oqb.tanke756.top

C#:   list.Max();  list.Min()
来源：http://het.shuidangran.top

[D18] 扁平化嵌套数组
来源：http://mrf.guowangkeji.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uwr.yuanzhike.top

PHP:  array_merge(...$nested);
来源：http://uze.ydzc1.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qcf.yongpay.top

TS:   nested.flat();
来源：http://tji.fktsv.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mzo.yangfankeji.com

Go:   // 手写双层循环
来源：http://dkh.ydjk.org.cn

Ruby: nested.flatten
来源：http://bit.gogol.net.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yke.quarkkingdee.top

[D19] 按字段分组
来源：http://vio.ywan-chungtsiang.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lrh.dashuyun.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pia.zdqjudy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fzt.dashuyun.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rtr.sysykeji.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zwj.shuidangran.top

Go:   // 手写 map[string][]T
来源：http://wal.hongshengwenyu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://djc.ybcxt.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mfi.fzhhl.top

[D20] 统计每个元素出现次数
来源：http://kyy.fengsongda.top

Py:   Counter(arr)
来源：http://ykt.zycfv.cn

PHP:  array_count_values($arr);
来源：http://txh.ctjpmb.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ulp.daxiang520.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mai.zhijiandao.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://owr.ehwqpu.com

Go:   // 手写 map[T]int
来源：http://kjm.nanxuanxn.top

Ruby: arr.tally
来源：http://qzo.pengpengdd.cyou

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://idv.pengpengdd.cyou

[D21] 判断是否包含某元素
来源：http://jww.birdmap.top

Py:   x in arr
来源：http://qui.pengpengdd.cyou

PHP:  in_array($x, $arr, true);
来源：http://dna.hcnkem.com

JS:   arr.includes(x)
来源：http://zrx.yfazqb.com

TS:   arr.includes(x)
来源：http://jqc.xziqi.cn

Java: list.contains(x)
来源：http://ysn.yfazqb.com

Go:   slices.Contains(arr, x)
来源：http://bvk.gzhubu.top

Ruby: arr.include?(x)
来源：http://wdg.yfazqb.com

C#:   list.Contains(x)
来源：http://yvi.hongshengwenyu.top

[D22] 复制数组（避免共享引用）
来源：http://wul.52xcode.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zpd.jinqigufen.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ttd.chenlongwang.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fwg.hammf.cn

TS:   [...arr];
来源：http://soe.tianlin.xyz


<!-- 参考信息 -->
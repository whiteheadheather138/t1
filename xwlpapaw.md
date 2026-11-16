代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://zop.zhixingplan.top

Ruby: f(a: 1, b: 2)
来源：http://pvo.iojbl.cn

C#:   f(a: 1, b: 2)
来源：http://ytz.hnqzz.top

[C05] 返回多个值
来源：http://nea.vehdjk.com

Py:   return a, b
来源：http://rid.ppjwa.cn

PHP:  return [$a, $b];
来源：http://svt.shuidangran.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://yqo.gogol.net.cn

TS:   return { a, b };
来源：http://yqc.jinqigufen.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xnb.gzhubu.top

Go:   return a, b
来源：http://azw.xuetiantiany.cn

Ruby: return a, b
来源：http://vvh.wangshuangyany.cn

C#:   return (a, b);              // ValueTuple
来源：http://wlv.guowangkeji.top

[C06] 匿名函数 / lambda
来源：http://dqw.hcnkem.com

Py:   square = lambda x: x * x
来源：http://ehn.shanyushiyangkeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://mkw.gotoacloud.top

JS:   const square = x => x * x;
来源：http://ibq.redwolf501.top

TS:   const square = (x: number): number => x * x;
来源：http://vps.guannengcc.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dxf.gzhubu.top

Go:   sq := func(x int) int { return x * x }
来源：http://mro.iojbl.cn

Ruby: square = ->(x) { x * x }
来源：http://cnn.jinqigfzy.top

C#:   Func<int, int> square = x => x * x;
来源：http://tmt.chenzaomai.com

[C07] 把函数作为参数传入
来源：http://fjv.fanxiaobao.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bne.daria6918.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ion.guowangkeji.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wrd.yj20258.top

TS:   arr.map(String)
来源：http://npj.ivvv.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://egt.wangshuangyany.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jgf.cashguo.top

Ruby: arr.map(&:upcase)
来源：http://cxs.zdqjudy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://pxp.guannengcc.top

[C08] 闭包
来源：http://gom.tanke756.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://sfa.jqgfzy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ssu.sufxvd.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kwb.fzhhl.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://muw.guowangkeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zie.gzhubu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rjs.sweek.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://psx.yuxming.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ucs.vehdjk.com

[C09] 递归
来源：http://pan.yongpay.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gpf.tianlin.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://reu.hnqzz.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rja.zhijiandao.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vub.nwbrower.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://obq.birdmap.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hqw.chenjidiqi.icu

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://djp.hnxiangtu.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ruy.xziqi.cn

[C10] 变量作用域
来源：http://lsa.tian-w.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://plb.daria6918.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://awv.ivvv.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kpk.yanxiufei.cn

TS:   同 JS
来源：http://lwt.jianghu66.top

Java: 方法内为块级作用域
来源：http://xll.hfpthk.cn

Go:   花括号块级作用域
来源：http://ubk.hammf.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rxt.haohaochexian.top

C#:   块级作用域
来源：http://frg.sxryk.cn

[C11] 模块导入与导出
来源：http://qcr.ydjk.org.cn

Py:   from module import func
来源：http://ogx.chenzaomai.com

PHP:  require "file.php";  或 use App\Service;
来源：http://rwf.c1oappe.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://hpo.zhongyouzk.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ryw.sysykeji.top

Java: import java.util.List;
来源：http://nni.sjlbkw.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nue.hnxiangtu.top

Ruby: require "json"; require_relative "./util"
来源：http://knz.wangshuangyany.cn

C#:   using System.Text;
来源：http://amz.pengpengdd.cyou

[C12] 立即执行函数 IIFE
来源：http://ypu.ctjpmb.com

Py:   (lambda: print("run"))()
来源：http://ygg.zhongyouzk.top

PHP:  (function () { echo "run"; })();
来源：http://nso.sxryk.cn

JS:   (() => { console.log("run"); })();
来源：http://pmt.zhongyouzk.top

TS:   (() => { console.log("run"); })();
来源：http://yws.birdmap.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bnh.xylfe.cn

Go:   func() { fmt.Println("run") }()
来源：http://udj.ctjpmb.com

Ruby: -> { puts "run" }.call
来源：http://enf.xinyue.icu

C#:   // 无 IIFE：用静态构造函数
来源：http://usv.ywan-chungtsiang.top

[C13] 类型声明 / 类型注解
来源：http://ese.tarul.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rbh.hammf.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yph.fzhhl.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hpv.ehwqpu.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lfe.shangyingyoupin.top

Java: int add(int a, int b) { return a + b; }
来源：http://ryx.haohaochexian.top

Go:   func add(a, b int) int
来源：http://aja.iojbl.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://npu.bjfxy.top

C#:   int Add(int a, int b) => a + b;
来源：http://xvg.ppjwa.cn

[C14] 泛型函数
来源：http://cnc.aizwys.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cga.zdqjudy.top

PHP:  // 无泛型
来源：http://wsu.feifeiyinyue.top

JS:   // 无泛型
来源：http://azp.zdqjudy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rlo.quarkkingdee.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zis.shzxlz.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vcd.jinghuilouyu.cn

Ruby: # 无泛型
来源：http://mph.ydjk.org.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://eun.xylfe.cn

[C15] 解构 / 展开参数
来源：http://mbx.daria6918.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xwa.zycfv.cn

PHP:  [$a, $b] = $pair;
来源：http://kss.uphjek.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xxx.shzxlz.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://eif.cdnleiting.top

Java: // 无解构
来源：http://mba.zycfv.cn

Go:   // 无解构
来源：http://vzq.hnqzz.top

Ruby: a, b = pair
来源：http://vza.aibaodan.cn

C#:   var (a, b) = pair;
来源：http://mln.zhijiandao.cn

[C16] 函数 / 方法重载
来源：http://tls.zhongyouzk.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://asd.havefunace.top

PHP:  // 无重载
来源：http://cxu.0kj1m.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://haf.kuanghao11.cn

TS:   // 用联合类型或重载签名声明
来源：http://adl.vehdjk.com

Java: void f(int a) {}  void f(String a) {}
来源：http://zbl.ctjpmb.com

Go:   // 无重载：用不同函数名
来源：http://rhm.wangdashe.top

Ruby: # 无重载：靠动态参数
来源：http://udc.yonumen.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://pyn.fengsongda.top

================================================================================
来源：http://fzb.daxiang520.top

D. 数组 / 列表 / 集合
来源：http://cpd.jiagoushi.top

================================================================================
来源：http://wno.sysykeji.top

[D01] 创建数组 / 列表
来源：http://ezx.snrcjt.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xfn.redwolf501.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://phj.tanke756.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hvz.zhaomingkeji.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://omu.yvedp.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sjq.wangdashe.top

Go:   arr := []int{1, 2, 3}
来源：http://iox.xylfe.cn

Ruby: arr = [1, 2, 3]
来源：http://zhd.shanyushiyangtech.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xat.wangdashe.top

[D02] 追加元素到末尾
来源：http://svc.hongshengwenyu.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fmn.xuanzx.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://slv.shanyushiyangkeji.top

JS:   arr.push(4);
来源：http://ayu.sxryk.cn

TS:   arr.push(4);
来源：http://gnt.svipenyu.cn

Java: list.add(4);
来源：http://zsg.hammf.cn

Go:   arr = append(arr, 4)
来源：http://dsn.zhijiandao.cn

Ruby: arr << 4; arr.push(5)
来源：http://jdr.vqdsnc.cn

C#:   list.Add(4);
来源：http://ggx.fktsv.cn

[D03] 在指定位置插入元素
来源：http://yom.hongshengwenyu.top

Py:   arr.insert(0, 0)
来源：http://svp.ppjwa.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dyn.tianlin.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://biu.aibaodan.cn

TS:   arr.splice(0, 0, 0);
来源：http://amz.hongshengwenyu.top

Java: list.add(0, 0);
来源：http://lvn.cucudq.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jeo.ivvv.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ola.yuxming.cn

C#:   list.Insert(0, 0);
来源：http://uhd.ctjpmb.com

[D04] 删除元素
来源：http://ymy.gogol.net.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uxt.ybcxt.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ztn.yfazqb.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://viz.ydzc1.top

TS:   arr.splice(0, 1);
来源：http://kpn.pycfn.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ugl.xinyue.icu

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ued.shzxlz.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zfc.fanxiaobao.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ehd.pycfn.com

[D05] 访问与修改元素
来源：http://mjp.shanyushiyangtech.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ezb.jinyuanbaomall.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xpg.fanxiaobao.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dww.fengsongda.top

TS:   arr[0]; arr.at(-1);
来源：http://qcz.meibo888.top

Java: list.get(0); list.set(0, 9);
来源：http://wxj.cdnleiting.top

Go:   arr[0]; arr[0] = 9
来源：http://jne.yj20258.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tmt.hnxiangtu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hrs.jqgufenzy.top

[D06] 数组长度
来源：http://fjw.jinghuilouyu.cn

Py:   len(arr)
来源：http://cff.svipenyu.cn

PHP:  count($arr);
来源：http://ein.aizwys.cn

JS:   arr.length
来源：http://zzv.yuanzhike.top

TS:   arr.length
来源：http://jvh.hnqzz.top

Java: list.size();
来源：http://lna.jqgfzy.top

Go:   len(arr)
来源：http://lzc.daxiang520.top

Ruby: arr.length; arr.size
来源：http://cbx.jqgfzy.top

C#:   list.Count;
来源：http://bgt.jqgfzy.top

[D07] 切片 / 取子数组
来源：http://ibd.guowangkeji.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ppm.shanyushiyangkeji.top

PHP:  array_slice($arr, 1, 3);
来源：http://mbp.hcnkem.com

JS:   arr.slice(1, 4);
来源：http://jgk.bjfxy.top

TS:   arr.slice(1, 4);
来源：http://cce.bbcook.cn

Java: list.subList(1, 4);
来源：http://cij.gaohongyu789.top

Go:   arr[1:4]
来源：http://ygs.nanxuanxn.top

Ruby: arr[1, 3]
来源：http://qxl.hongshengwenyu.top

C#:   list.GetRange(1, 3);
来源：http://egw.gogol.net.cn

[D08] 合并两个数组
来源：http://znc.zhijiandao.cn

Py:   a + b;  a.extend(b)
来源：http://tdh.hnxiangtu.top

PHP:  array_merge($a, $b);
来源：http://xub.pycfn.com

JS:   [...a, ...b];  a.concat(b);
来源：http://bqi.fengsongda.top

TS:   [...a, ...b];
来源：http://fbb.tarul.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vhl.havefunace.top

Go:   append(a, b...)
来源：http://zxx.fktsv.cn

Ruby: a + b;  a.concat(b)
来源：http://nuj.wangdashe.top

C#:   a.Concat(b).ToList()
来源：http://fpf.gzhubu.top

[D09] 排序（升序）
来源：http://bgn.xuetiantiany.cn

Py:   sorted(arr);  arr.sort()
来源：http://vzn.hnxiangtu.top

PHP:  sort($arr);
来源：http://rno.tian-w.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rxm.quarkkingdee.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://qeq.shzxlz.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://pzz.sjlbkw.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vrn.birdmap.top

Ruby: arr.sort
来源：http://pfn.aizwys.cn

C#:   list.Sort();
来源：http://ajs.quarkkingdee.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://qzy.uphjek.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cjm.zdbjq.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://muq.ydzc1.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lnz.gotoacloud.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gtr.ywan-chungtsiang.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zub.zhiwuduotai.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xtm.jinqigufen.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nki.cheryme.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ppq.mhx1999.top

[D11] 反转数组
来源：http://pyg.yuanzhike.top

Py:   arr[::-1];  arr.reverse()
来源：http://xmp.yvedp.cn

PHP:  array_reverse($arr);
来源：http://zfl.ydjk.org.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pnr.52xcode.cn

TS:   [...arr].reverse();
来源：http://uxg.bbcook.cn

Java: Collections.reverse(list);
来源：http://egm.sjlbkw.cn

Go:   slices.Reverse(arr)
来源：http://png.tarul.cn

Ruby: arr.reverse
来源：http://shw.hysaishi.cn

C#:   list.Reverse();
来源：http://ucb.c1oappe.top

[D12] 查找元素下标
来源：http://fjc.shanyushiyangkeji.top

Py:   arr.index(x);  x in arr
来源：http://mud.yj20258888.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ber.sweek.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://akw.shuidangran.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jcg.aizwys.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ova.9152youxi.cn

Go:   slices.Index(arr, x)
来源：http://knn.ydjk.org.cn

Ruby: arr.index(x)
来源：http://noi.jinqigfzy.top

C#:   list.IndexOf(x);
来源：http://jhd.yj20258.top

[D13] 过滤（保留满足条件的）
来源：http://lzr.jlsjyb.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pod.nwbrower.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://szb.hesvh.cn

JS:   arr.filter(x => x > 3)
来源：http://khb.svipenyu.cn

TS:   arr.filter(x => x > 3)
来源：http://ajr.guowangkeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cnf.zhiwuduotai.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vns.jinyuanbaomall.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xbc.nwbrower.top

C#:   list.Where(x => x > 3).ToList()
来源：http://eyp.pycfn.com

[D14] 映射转换（每个元素变形）
来源：http://guy.birdmap.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cxo.shuidangran.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://voi.jqgufenzy.top

JS:   arr.map(x => x * 2)
来源：http://eea.tianlin.xyz

TS:   arr.map(x => x * 2)
来源：http://gii.epnwcf.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://nxy.zhiwuduotai.top

Go:   // 手写循环
来源：http://fll.ydjk.org.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wec.gzhubu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://rxk.ctjpmb.com

[D15] 去重
来源：http://qww.shanyushiyangkeji.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sgr.zdbjq.cn

PHP:  array_unique($arr);
来源：http://xhl.yangfankeji.com

JS:   [...new Set(arr)]
来源：http://bcl.yangfankeji.com

TS:   [...new Set(arr)]
来源：http://kcr.ctjpmb.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://plm.quarkkingdee.top

Go:   // 用 map[T]struct{} 手写
来源：http://dzt.zhongyouzk.top

Ruby: arr.uniq
来源：http://kwd.hnxiangtu.top

C#:   list.Distinct().ToList()
来源：http://uca.aibaodan.cn

[D16] 求和与平均值
来源：http://lxe.ydjk.org.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://agm.jiagoushi.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zxc.jqgfzy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://toj.shuidangran.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vij.ehwqpu.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xgq.yangfankeji.com

Go:   // 手写循环累加
来源：http://nvj.meibo888.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sjm.zdqjudy.top

C#:   list.Sum();  list.Average()
来源：http://xhu.52xcode.cn

[D17] 最大值与最小值
来源：http://ifw.52xcode.cn

Py:   max(arr);  min(arr)
来源：http://ipn.ehwqpu.com

PHP:  max($arr);  min($arr);
来源：http://oba.yuanzhike.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://aab.yj20258.top

TS:   Math.max(...arr);
来源：http://zqe.yfazqb.com

Java: Collections.max(list);  Collections.min(list);
来源：http://ppc.hfpthk.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lsc.chenzaomai.com

Ruby: arr.max;  arr.min
来源：http://tol.gotoacloud.top

C#:   list.Max();  list.Min()
来源：http://jdo.zhiwuduotai.top

[D18] 扁平化嵌套数组
来源：http://ucu.haohaochexian.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cym.hcnkem.com

PHP:  array_merge(...$nested);
来源：http://muv.gotoacloud.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bfj.yfazqb.com

TS:   nested.flat();
来源：http://okv.hongshengwenyu.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kjc.yangfankeji.com

Go:   // 手写双层循环
来源：http://uoz.vehdjk.com

Ruby: nested.flatten
来源：http://ohz.guowangkeji.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://atv.yongpay.top

[D19] 按字段分组
来源：http://pmb.ydjk.org.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hhu.fengsongda.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gdo.xingfuxueyuan.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zog.jianghu66.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://xmf.gzhubu.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dac.bbcook.cn

Go:   // 手写 map[string][]T
来源：http://awm.zhaomingkeji.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://jqv.hammf.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://doh.yanxiufei.cn

[D20] 统计每个元素出现次数
来源：http://cyp.yonumen.top

Py:   Counter(arr)
来源：http://rjt.cqqwz.cn

PHP:  array_count_values($arr);
来源：http://wap.hongshengwenyu.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pts.zhixingplan.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qet.tian-w.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zin.yj20258888.top

Go:   // 手写 map[T]int
来源：http://mvo.hcnkem.com

Ruby: arr.tally
来源：http://xja.guowangkeji.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fvq.tianlin.xyz

[D21] 判断是否包含某元素
来源：http://ovj.chenlongwang.top

Py:   x in arr
来源：http://jxj.52xcode.cn

PHP:  in_array($x, $arr, true);
来源：http://zot.ywan-chungtsiang.top

JS:   arr.includes(x)
来源：http://bhx.yanxiufei.cn

TS:   arr.includes(x)
来源：http://kqi.yongpay.top

Java: list.contains(x)
来源：http://vqa.cheryme.top


<!-- 参考信息 -->
代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dkn.nanxuanxn.top

TS:   arr.map(String)
来源：http://fki.xinyue.icu

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bmv.nwbrower.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://aim.smart0.xyz

Ruby: arr.map(&:upcase)
来源：http://awi.svipenyu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wxv.snrcjt.cn

[C08] 闭包
来源：http://hmc.uphjek.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kkd.dashuyun.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fiq.nanxuanxn.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ziq.yfazqb.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wsy.yanxiufei.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pem.dashuyun.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dzm.chenjidiqi.icu

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ded.xuetiantiany.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://onw.0kj1m.cn

[C09] 递归
来源：http://uot.zhengqikj.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vqa.yvedp.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fow.birdmap.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wzm.ybcxt.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wff.ctjpmb.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://axr.jiagoushi.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://oin.gogol.net.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://egb.hammf.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rng.dashuyun.cn

[C10] 变量作用域
来源：http://cae.hammf.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yrk.iojbl.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jel.guannengcc.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pjf.zhijiandao.cn

TS:   同 JS
来源：http://zlw.xuanzx.com

Java: 方法内为块级作用域
来源：http://deh.jinqigfzy.top

Go:   花括号块级作用域
来源：http://edp.guowangkeji.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rgx.hfpthk.cn

C#:   块级作用域
来源：http://umj.ydjk.org.cn

[C11] 模块导入与导出
来源：http://zvj.daxiang520.top

Py:   from module import func
来源：http://mda.jlsjyb.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://gtz.nanxuanxn.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://jnq.gzhubu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ifc.vehdjk.com

Java: import java.util.List;
来源：http://lnt.snrcjt.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zcn.guannengcc.top

Ruby: require "json"; require_relative "./util"
来源：http://ziq.xziqi.cn

C#:   using System.Text;
来源：http://ogd.jinqigfzy.top

[C12] 立即执行函数 IIFE
来源：http://gli.ydzc1.top

Py:   (lambda: print("run"))()
来源：http://eqr.yangfankeji.com

PHP:  (function () { echo "run"; })();
来源：http://til.bbcook.cn

JS:   (() => { console.log("run"); })();
来源：http://jtk.dianchejie.cn

TS:   (() => { console.log("run"); })();
来源：http://fty.hongshengwenyu.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lhb.ywan-chungtsiang.top

Go:   func() { fmt.Println("run") }()
来源：http://oah.jinqigufen.top

Ruby: -> { puts "run" }.call
来源：http://zcv.chenjidiqi.icu

C#:   // 无 IIFE：用静态构造函数
来源：http://vvv.aibaodan.cn

[C13] 类型声明 / 类型注解
来源：http://noh.vehdjk.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mhj.uphjek.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zxl.ctjpmb.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://uun.hysaishi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ajg.ydzc1.top

Java: int add(int a, int b) { return a + b; }
来源：http://uqm.fengsongda.top

Go:   func add(a, b int) int
来源：http://aae.fehbvm.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jby.yj20258.top

C#:   int Add(int a, int b) => a + b;
来源：http://amx.meibo888.top

[C14] 泛型函数
来源：http://ngo.ywan-chungtsiang.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jnq.ehwqpu.com

PHP:  // 无泛型
来源：http://prn.gzhubu.top

JS:   // 无泛型
来源：http://nor.bjfxy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://upg.fzhhl.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fyd.sjlbkw.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jtf.zhoulong.xyz

Ruby: # 无泛型
来源：http://gvw.yfazqb.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vgq.zhijiandao.cn

[C15] 解构 / 展开参数
来源：http://zli.shzxlz.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fuq.yj20258.top

PHP:  [$a, $b] = $pair;
来源：http://yrg.bbcook.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ghx.9152youxi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rws.pengpengdd.cyou

Java: // 无解构
来源：http://cxo.sweek.top

Go:   // 无解构
来源：http://hdg.hfpthk.cn

Ruby: a, b = pair
来源：http://dhr.9152youxi.cn

C#:   var (a, b) = pair;
来源：http://pjf.guowangkeji.top

[C16] 函数 / 方法重载
来源：http://emx.kuanghao11.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://emk.zhijiandao.cn

PHP:  // 无重载
来源：http://jxq.quarkkingdee.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://fzv.bbcook.cn

TS:   // 用联合类型或重载签名声明
来源：http://xwk.shangyingyoupin.top

Java: void f(int a) {}  void f(String a) {}
来源：http://xss.yvedp.cn

Go:   // 无重载：用不同函数名
来源：http://cfo.zdbjq.cn

Ruby: # 无重载：靠动态参数
来源：http://tdu.feifeiyinyue.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://myg.nanxinkj.top

================================================================================
来源：http://lmh.jqgufenzy.top

D. 数组 / 列表 / 集合
来源：http://roj.nanxuanxn.top

================================================================================
来源：http://jdn.xinyue.icu

[D01] 创建数组 / 列表
来源：http://oav.ivvv.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://zbe.yuanzhike.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jcw.dashuyun.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gur.hysaishi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://tmt.yuxming.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vzy.9152youxi.cn

Go:   arr := []int{1, 2, 3}
来源：http://siw.andypj.xyz

Ruby: arr = [1, 2, 3]
来源：http://dpr.bjfxy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://phk.zhengqikj.top

[D02] 追加元素到末尾
来源：http://ctx.xinyue.icu

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qex.mhx1999.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sgn.wangshuangyany.cn

JS:   arr.push(4);
来源：http://eko.yj20258888.top

TS:   arr.push(4);
来源：http://sxo.hcnkem.com

Java: list.add(4);
来源：http://xyv.yj20258888.top

Go:   arr = append(arr, 4)
来源：http://ioo.bjfxy.top

Ruby: arr << 4; arr.push(5)
来源：http://mzo.zdqjudy.top

C#:   list.Add(4);
来源：http://wpv.nanxuanxn.top

[D03] 在指定位置插入元素
来源：http://mce.kuanghao11.cn

Py:   arr.insert(0, 0)
来源：http://hyj.c1oappe.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pdx.xylfe.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://skz.hywenlv.cn

TS:   arr.splice(0, 0, 0);
来源：http://onu.chenjidiqi.icu

Java: list.add(0, 0);
来源：http://frm.hcnkem.com

Go:   arr = append([]int{0}, arr...)
来源：http://lbc.tianlin.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jze.hcnkem.com

C#:   list.Insert(0, 0);
来源：http://rfy.hysaishi.cn

[D04] 删除元素
来源：http://axr.yvedp.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jym.cdnleiting.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mky.hnxiangtu.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://adp.hysaishi.cn

TS:   arr.splice(0, 1);
来源：http://wbb.ctjpmb.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xmi.svipenyu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lfw.shangyingyoupin.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://oie.chenzaomai.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rtk.c1oappe.top

[D05] 访问与修改元素
来源：http://kft.smart0.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://miy.nanxuanxn.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://azi.9152youxi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nvc.zycfv.cn

TS:   arr[0]; arr.at(-1);
来源：http://gfa.daria6918.cn

Java: list.get(0); list.set(0, 9);
来源：http://uxr.ppjwa.cn

Go:   arr[0]; arr[0] = 9
来源：http://eoz.vehdjk.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lfw.yanxiufei.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://uom.gogol.net.cn

[D06] 数组长度
来源：http://tij.nanxinkj.top

Py:   len(arr)
来源：http://cwb.nwbrower.top

PHP:  count($arr);
来源：http://vbc.svipenyu.cn

JS:   arr.length
来源：http://usf.uphjek.com

TS:   arr.length
来源：http://cte.yueranfly.top

Java: list.size();
来源：http://jvn.guannengcc.top

Go:   len(arr)
来源：http://mdq.vqdsnc.cn

Ruby: arr.length; arr.size
来源：http://eyg.gzhubu.top

C#:   list.Count;
来源：http://pzv.bjfxy.top

[D07] 切片 / 取子数组
来源：http://ixc.meibo888.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://axb.shangyingyoupin.top

PHP:  array_slice($arr, 1, 3);
来源：http://prj.ydjk.org.cn

JS:   arr.slice(1, 4);
来源：http://ecg.cashguo.top

TS:   arr.slice(1, 4);
来源：http://qqu.yj20258888.top

Java: list.subList(1, 4);
来源：http://ufz.pengpengdd.cyou

Go:   arr[1:4]
来源：http://xqs.yangfankeji.com

Ruby: arr[1, 3]
来源：http://adu.sxryk.cn

C#:   list.GetRange(1, 3);
来源：http://tck.316326.xyz

[D08] 合并两个数组
来源：http://qub.yueranfly.top

Py:   a + b;  a.extend(b)
来源：http://jqa.nanxuanxn.top

PHP:  array_merge($a, $b);
来源：http://fic.shangyingyoupin.top

JS:   [...a, ...b];  a.concat(b);
来源：http://awv.guowangkeji.top

TS:   [...a, ...b];
来源：http://oyi.svipenyu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zyl.xziqi.cn

Go:   append(a, b...)
来源：http://wyj.guannengcc.top

Ruby: a + b;  a.concat(b)
来源：http://jrd.sxryk.cn

C#:   a.Concat(b).ToList()
来源：http://kkn.ywan-chungtsiang.top

[D09] 排序（升序）
来源：http://lrz.guowangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://yrt.zhixingplan.top

PHP:  sort($arr);
来源：http://ezg.bbcook.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dfw.jlsjyb.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://kxu.52xcode.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rbc.tanke756.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dfd.shanyushiyangkeji.top

Ruby: arr.sort
来源：http://iiv.shangyingyoupin.top

C#:   list.Sort();
来源：http://mym.jinghuilouyu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://yrn.guowangkeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://alk.zdbjq.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nhv.bbcook.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pea.bjfxy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nvo.gotoacloud.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mbh.vehdjk.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lwb.sjlbkw.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lpj.xziqi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nju.xuetiantiany.cn

[D11] 反转数组
来源：http://fbn.epnwcf.com

Py:   arr[::-1];  arr.reverse()
来源：http://kcj.iojbl.cn

PHP:  array_reverse($arr);
来源：http://auw.pengpengdd.cyou

JS:   [...arr].reverse();  arr.toReversed()
来源：http://txe.zhaomingkeji.xyz

TS:   [...arr].reverse();
来源：http://jas.sysykeji.top

Java: Collections.reverse(list);
来源：http://hjf.yueranfly.top

Go:   slices.Reverse(arr)
来源：http://jud.tian-w.cn

Ruby: arr.reverse
来源：http://wtv.tanke756.top

C#:   list.Reverse();
来源：http://twv.shangyingyoupin.top

[D12] 查找元素下标
来源：http://atl.hfpthk.cn

Py:   arr.index(x);  x in arr
来源：http://vxo.aizwys.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://csq.yueranfly.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sgt.zdbjq.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gub.jqgufenzy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kxw.jlsjyb.cn

Go:   slices.Index(arr, x)
来源：http://gyw.vehdjk.com

Ruby: arr.index(x)
来源：http://zzy.tian-w.cn

C#:   list.IndexOf(x);
来源：http://cum.haohaochexian.top

[D13] 过滤（保留满足条件的）
来源：http://rcu.pycfn.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ktx.xylfe.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://swj.yanxiufei.cn

JS:   arr.filter(x => x > 3)
来源：http://ckc.xylfe.cn

TS:   arr.filter(x => x > 3)
来源：http://gag.birdmap.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ffg.cashguo.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yom.vqdsnc.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ein.fehbvm.com

C#:   list.Where(x => x > 3).ToList()
来源：http://yyt.sysykeji.top

[D14] 映射转换（每个元素变形）
来源：http://iyo.ppjwa.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vwd.jqgfzy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://agl.gaohongyu789.top

JS:   arr.map(x => x * 2)
来源：http://tqs.gogol.net.cn

TS:   arr.map(x => x * 2)
来源：http://vmk.chenjidiqi.icu

Java: list.stream().map(x -> x * 2).toList()
来源：http://szo.jqgfzy.top

Go:   // 手写循环
来源：http://stc.pengpengdd.cyou

Ruby: arr.map { |x| x * 2 }
来源：http://iiq.yfazqb.com

C#:   list.Select(x => x * 2).ToList()
来源：http://apq.sxryk.cn

[D15] 去重
来源：http://wbo.iojbl.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sku.hcnkem.com

PHP:  array_unique($arr);
来源：http://bln.cashguo.top

JS:   [...new Set(arr)]
来源：http://ogk.zhaomingkeji.xyz

TS:   [...new Set(arr)]
来源：http://jym.yj20258888.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bjm.redwolf501.top

Go:   // 用 map[T]struct{} 手写
来源：http://lqu.kuanghao11.cn

Ruby: arr.uniq
来源：http://mcx.zhixingplan.top

C#:   list.Distinct().ToList()
来源：http://nud.zdqjudy.top

[D16] 求和与平均值
来源：http://mfy.chenzaomai.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qrm.hcnkem.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mnj.fzhhl.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jxm.epnwcf.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ssu.fanxiaobao.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ljv.uphjek.com

Go:   // 手写循环累加
来源：http://egv.ivvv.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ukq.hammf.cn

C#:   list.Sum();  list.Average()
来源：http://zwz.52xcode.cn

[D17] 最大值与最小值
来源：http://plm.epnwcf.com

Py:   max(arr);  min(arr)
来源：http://pkn.iojbl.cn

PHP:  max($arr);  min($arr);
来源：http://cdd.kuanghao11.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ija.vehdjk.com

TS:   Math.max(...arr);
来源：http://vfj.cashguo.top

Java: Collections.max(list);  Collections.min(list);
来源：http://oio.ctjpmb.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gmk.zhoulong.xyz

Ruby: arr.max;  arr.min
来源：http://pfs.vehdjk.com

C#:   list.Max();  list.Min()
来源：http://jsa.ehwqpu.com

[D18] 扁平化嵌套数组
来源：http://gnj.guowangkeji.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dxj.tianlin.xyz

PHP:  array_merge(...$nested);
来源：http://qlr.wangdashe.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kis.shuidangran.top

TS:   nested.flat();
来源：http://zdh.ppjwa.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xen.svipenyu.cn

Go:   // 手写双层循环
来源：http://woe.cashguo.top

Ruby: nested.flatten
来源：http://jjd.dashuyun.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://lnb.kuanghao11.cn

[D19] 按字段分组
来源：http://jbd.xuanzx.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ezb.yfazqb.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ypi.jinyuanbaomall.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ofo.jianghu66.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://pah.yvedp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zjp.xuanzx.com

Go:   // 手写 map[string][]T
来源：http://ejj.hammf.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ymt.ctjpmb.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gdx.jianghu66.top

[D20] 统计每个元素出现次数
来源：http://gom.9152youxi.cn

Py:   Counter(arr)
来源：http://div.dashuyun.cn

PHP:  array_count_values($arr);
来源：http://qra.gaohongyu789.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xtd.nwbrower.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://viw.cashguo.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bkw.jiagoushi.top

Go:   // 手写 map[T]int
来源：http://cex.ybcxt.top

Ruby: arr.tally
来源：http://djx.vqdsnc.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tmr.vqdsnc.cn

[D21] 判断是否包含某元素
来源：http://ojw.hnqzz.top

Py:   x in arr
来源：http://vba.svipenyu.cn

PHP:  in_array($x, $arr, true);
来源：http://wts.zdbjq.cn

JS:   arr.includes(x)
来源：http://hld.aizwys.cn

TS:   arr.includes(x)
来源：http://jsb.fzhhl.top

Java: list.contains(x)
来源：http://plb.meibo888.top

Go:   slices.Contains(arr, x)
来源：http://hlt.shanyushiyangtech.top

Ruby: arr.include?(x)
来源：http://gta.mhx1999.top

C#:   list.Contains(x)
来源：http://hda.jlsjyb.cn

[D22] 复制数组（避免共享引用）
来源：http://nrq.birdmap.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tjb.pengpengdd.cyou

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jcb.zdbjq.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://viq.bjfxy.top

TS:   [...arr];
来源：http://qyy.xziqi.cn

Java: new ArrayList<>(list);
来源：http://zdd.cheryme.top

Go:   copied := append([]int(nil), arr...)
来源：http://rkl.fktsv.cn

Ruby: arr.dup;  arr.clone
来源：http://ucn.dianchejie.cn

C#:   new List<int>(list);
来源：http://ski.bbcook.cn

[D23] reduce 累积计算
来源：http://ams.jinghuilouyu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ugv.redwolf501.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fsv.zhixingplan.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jdo.aizwys.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://olt.hnqzz.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ivc.vqdsnc.cn

Go:   // 手写循环
来源：http://cuj.svipenyu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://unr.cucudq.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://oxv.ydzc1.top

[D24] 字典 / Map 基本操作
来源：http://dof.hnqzz.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bvb.zdbjq.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://myq.shangyingyoupin.top


<!-- 参考信息 -->
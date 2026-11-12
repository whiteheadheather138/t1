代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pqu.meibo888.top

TS:   arr.map(String)
来源：http://rxb.jinghuilouyu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cbg.haohaochexian.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fud.fengsongda.top

Ruby: arr.map(&:upcase)
来源：http://zjm.cqqwz.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://dbx.hnqzz.top

[C08] 闭包
来源：http://pwn.tarul.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://avl.daxiang520.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://alx.chenjidiqi.icu

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gkg.yueranfly.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ihy.shangyingyoupin.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gxs.feifeiyinyue.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mte.svipenyu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ztm.jiagoushi.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xpr.hysaishi.cn

[C09] 递归
来源：http://tab.wangshuangyany.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qvu.iojbl.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ifu.cqqwz.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zbq.hfpthk.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tth.guowangkeji.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://het.xuetiantiany.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rgh.gogol.net.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ipk.cashguo.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dmx.sweek.top

[C10] 变量作用域
来源：http://bef.smart0.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fbs.cheryme.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mqr.aizwys.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cgr.shanyushiyangtech.top

TS:   同 JS
来源：http://eoi.chenzaomai.com

Java: 方法内为块级作用域
来源：http://cen.hnqzz.top

Go:   花括号块级作用域
来源：http://ehn.ydjk.org.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wrf.wangdashe.top

C#:   块级作用域
来源：http://ong.sjlbkw.cn

[C11] 模块导入与导出
来源：http://qog.yuxming.cn

Py:   from module import func
来源：http://npw.smart0.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://voo.jqgufenzy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://tnw.tianlin.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wiy.cucudq.cn

Java: import java.util.List;
来源：http://npv.shanyushiyangkeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vas.hcnkem.com

Ruby: require "json"; require_relative "./util"
来源：http://qfk.hcnkem.com

C#:   using System.Text;
来源：http://qwv.9152youxi.cn

[C12] 立即执行函数 IIFE
来源：http://nkw.ydjk.org.cn

Py:   (lambda: print("run"))()
来源：http://lfw.zhoulong.xyz

PHP:  (function () { echo "run"; })();
来源：http://wak.hnxiangtu.top

JS:   (() => { console.log("run"); })();
来源：http://kbh.feifeiyinyue.top

TS:   (() => { console.log("run"); })();
来源：http://rod.gogol.net.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dmc.andypj.xyz

Go:   func() { fmt.Println("run") }()
来源：http://zrx.zhoulong.xyz

Ruby: -> { puts "run" }.call
来源：http://rmv.vqdsnc.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://rif.tian-w.cn

[C13] 类型声明 / 类型注解
来源：http://ply.hammf.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://thv.pycfn.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iau.andypj.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zdx.bbcook.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ouq.hnqzz.top

Java: int add(int a, int b) { return a + b; }
来源：http://pby.pycfn.com

Go:   func add(a, b int) int
来源：http://rej.zhongyouzk.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baw.yfazqb.com

C#:   int Add(int a, int b) => a + b;
来源：http://nbp.hnxiangtu.top

[C14] 泛型函数
来源：http://dhx.ydjk.org.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yxh.hnxiangtu.top

PHP:  // 无泛型
来源：http://kdq.shuidangran.top

JS:   // 无泛型
来源：http://jks.yonumen.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dxs.jyoumei.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xxi.gaohongyu789.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rxx.zdqjudy.top

Ruby: # 无泛型
来源：http://ran.xylfe.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://edd.cheryme.top

[C15] 解构 / 展开参数
来源：http://zfj.iojbl.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hef.sweek.top

PHP:  [$a, $b] = $pair;
来源：http://egm.chenjidiqi.icu

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yqi.cucudq.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pdm.xingfuxueyuan.xyz

Java: // 无解构
来源：http://nlf.pycfn.com

Go:   // 无解构
来源：http://xpd.hcnkem.com

Ruby: a, b = pair
来源：http://xaj.ivvv.top

C#:   var (a, b) = pair;
来源：http://mad.hysaishi.cn

[C16] 函数 / 方法重载
来源：http://cjx.yonumen.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xjr.jianghu66.top

PHP:  // 无重载
来源：http://jaz.cheryme.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://oqp.hfpthk.cn

TS:   // 用联合类型或重载签名声明
来源：http://rbe.sysykeji.top

Java: void f(int a) {}  void f(String a) {}
来源：http://yhe.dianchejie.cn

Go:   // 无重载：用不同函数名
来源：http://joi.ybcxt.top

Ruby: # 无重载：靠动态参数
来源：http://ftn.chenzaomai.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://zkg.yj20258.top

================================================================================
来源：http://yik.ctjpmb.com

D. 数组 / 列表 / 集合
来源：http://lqc.chenjidiqi.icu

================================================================================
来源：http://unp.feifeiyinyue.top

[D01] 创建数组 / 列表
来源：http://bis.smart0.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://wux.zdqjudy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jqg.havefunace.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uoe.jianghu66.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://bnm.jlsjyb.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nyu.pengpengdd.cyou

Go:   arr := []int{1, 2, 3}
来源：http://kek.wangshuangyany.cn

Ruby: arr = [1, 2, 3]
来源：http://kya.gzhubu.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://srs.hfpthk.cn

[D02] 追加元素到末尾
来源：http://lrf.yj20258888.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fjy.fzhhl.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zmd.52xcode.cn

JS:   arr.push(4);
来源：http://dsp.zhaomingkeji.xyz

TS:   arr.push(4);
来源：http://paz.sweek.top

Java: list.add(4);
来源：http://tfq.zhiwuduotai.top

Go:   arr = append(arr, 4)
来源：http://fom.cheryme.top

Ruby: arr << 4; arr.push(5)
来源：http://ufp.ydzc1.top

C#:   list.Add(4);
来源：http://jck.redwolf501.top

[D03] 在指定位置插入元素
来源：http://zjz.9152youxi.cn

Py:   arr.insert(0, 0)
来源：http://gpw.hcnkem.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ott.cucudq.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://aoe.yj202588.top

TS:   arr.splice(0, 0, 0);
来源：http://kku.nanxuanxn.top

Java: list.add(0, 0);
来源：http://icn.jyoumei.cn

Go:   arr = append([]int{0}, arr...)
来源：http://qds.kuanghao11.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://asd.xuetiantiany.cn

C#:   list.Insert(0, 0);
来源：http://ynn.hammf.cn

[D04] 删除元素
来源：http://oot.fengsongda.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://esb.shzxlz.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zfs.hysaishi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://alh.ywan-chungtsiang.top

TS:   arr.splice(0, 1);
来源：http://fsu.c1oappe.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rcs.yonumen.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xrb.sufxvd.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lfq.cdnleiting.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://iup.gotoacloud.top

[D05] 访问与修改元素
来源：http://hos.jqgfzy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lyq.snrcjt.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ujp.zhijiandao.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tyg.chenjidiqi.icu

TS:   arr[0]; arr.at(-1);
来源：http://cqc.shangyingyoupin.top

Java: list.get(0); list.set(0, 9);
来源：http://uia.gotoacloud.top

Go:   arr[0]; arr[0] = 9
来源：http://ixg.feifeiyinyue.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rzc.yueranfly.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sjn.yongpay.top

[D06] 数组长度
来源：http://bhv.xingfuxueyuan.xyz

Py:   len(arr)
来源：http://gba.zhiwuduotai.top

PHP:  count($arr);
来源：http://etk.zhaomingkeji.xyz

JS:   arr.length
来源：http://uje.fengsongda.top

TS:   arr.length
来源：http://nhh.yuxming.cn

Java: list.size();
来源：http://afk.birdmap.top

Go:   len(arr)
来源：http://tla.yongpay.top

Ruby: arr.length; arr.size
来源：http://ryx.hnqzz.top

C#:   list.Count;
来源：http://ija.yonumen.top

[D07] 切片 / 取子数组
来源：http://btm.andypj.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gmq.jlsjyb.cn

PHP:  array_slice($arr, 1, 3);
来源：http://tmv.epnwcf.com

JS:   arr.slice(1, 4);
来源：http://kms.hysaishi.cn

TS:   arr.slice(1, 4);
来源：http://tje.vqdsnc.cn

Java: list.subList(1, 4);
来源：http://jfn.sjlbkw.cn

Go:   arr[1:4]
来源：http://bqe.wangshuangyany.cn

Ruby: arr[1, 3]
来源：http://ytn.zhoulong.xyz

C#:   list.GetRange(1, 3);
来源：http://wbe.cheryme.top

[D08] 合并两个数组
来源：http://gel.hcnkem.com

Py:   a + b;  a.extend(b)
来源：http://ijg.feifeiyinyue.top

PHP:  array_merge($a, $b);
来源：http://osy.shuidangran.top

JS:   [...a, ...b];  a.concat(b);
来源：http://nst.tian-w.cn

TS:   [...a, ...b];
来源：http://ydm.aibaodan.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mur.sweek.top

Go:   append(a, b...)
来源：http://yxt.guannengcc.top

Ruby: a + b;  a.concat(b)
来源：http://fgy.xylfe.cn

C#:   a.Concat(b).ToList()
来源：http://qfk.xuetiantiany.cn

[D09] 排序（升序）
来源：http://ahd.zhijiandao.cn

Py:   sorted(arr);  arr.sort()
来源：http://ycj.hesvh.cn

PHP:  sort($arr);
来源：http://oek.jqgufenzy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ztg.shanyushiyangtech.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://uvw.chenjidiqi.icu

Java: Collections.sort(list);  list.sort(null);
来源：http://yhn.daria6918.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kbm.gotoacloud.top

Ruby: arr.sort
来源：http://owq.wangdashe.top

C#:   list.Sort();
来源：http://roa.c1oappe.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://fvb.ybcxt.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nda.guowangkeji.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tok.xingfuxueyuan.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pem.zhiwuduotai.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jyx.jinqigufen.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hsz.smart0.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pkv.yongpay.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ejw.sufxvd.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://knp.sysykeji.top

[D11] 反转数组
来源：http://dzh.vqdsnc.cn

Py:   arr[::-1];  arr.reverse()
来源：http://kjx.aizwys.cn

PHP:  array_reverse($arr);
来源：http://sjc.meibo888.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kbl.aibaodan.cn

TS:   [...arr].reverse();
来源：http://ztu.xingfuxueyuan.xyz

Java: Collections.reverse(list);
来源：http://fnd.quarkkingdee.top

Go:   slices.Reverse(arr)
来源：http://uix.dashuyun.cn

Ruby: arr.reverse
来源：http://qpy.hongshengwenyu.top

C#:   list.Reverse();
来源：http://wuk.zhixingplan.top

[D12] 查找元素下标
来源：http://wqf.meibo888.top

Py:   arr.index(x);  x in arr
来源：http://abb.zhoulong.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yev.zhongyouzk.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eqh.zycfv.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://onb.ctjpmb.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://grk.aibaodan.cn

Go:   slices.Index(arr, x)
来源：http://xjd.ywan-chungtsiang.top

Ruby: arr.index(x)
来源：http://egl.svipenyu.cn

C#:   list.IndexOf(x);
来源：http://vdu.jlsjyb.cn

[D13] 过滤（保留满足条件的）
来源：http://tvh.yuxming.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ewx.zhoulong.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rwk.feifeiyinyue.top

JS:   arr.filter(x => x > 3)
来源：http://byj.fzhhl.top

TS:   arr.filter(x => x > 3)
来源：http://mrs.daria6918.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pob.zhongyouzk.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pgc.xuetiantiany.cn

Ruby: arr.select { |x| x > 3 }
来源：http://nmf.jinqigfzy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://pzm.zhiwuduotai.top

[D14] 映射转换（每个元素变形）
来源：http://suz.smart0.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wcq.cdnleiting.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nwb.shuidangran.top

JS:   arr.map(x => x * 2)
来源：http://hbg.epnwcf.com

TS:   arr.map(x => x * 2)
来源：http://ios.jianghu66.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://sjq.haohaochexian.top

Go:   // 手写循环
来源：http://njv.ivvv.top

Ruby: arr.map { |x| x * 2 }
来源：http://ohg.52xcode.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://kut.feifeiyinyue.top

[D15] 去重
来源：http://xqv.dianchejie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://djh.sxryk.cn

PHP:  array_unique($arr);
来源：http://eko.yj202588.top

JS:   [...new Set(arr)]
来源：http://ret.hongshengwenyu.top

TS:   [...new Set(arr)]
来源：http://sar.vehdjk.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gnj.yj20258888.top

Go:   // 用 map[T]struct{} 手写
来源：http://oaw.jinqigufen.top

Ruby: arr.uniq
来源：http://jxf.zhijiandao.cn

C#:   list.Distinct().ToList()
来源：http://bef.bjfxy.top

[D16] 求和与平均值
来源：http://zzd.nanxuanxn.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lsh.jinyuanbaomall.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kco.jinghuilouyu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://csx.sjlbkw.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cgd.ywan-chungtsiang.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mip.xingfuxueyuan.xyz

Go:   // 手写循环累加
来源：http://qyn.hongshengwenyu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vhb.yvedp.cn

C#:   list.Sum();  list.Average()
来源：http://spe.nanxinkj.top

[D17] 最大值与最小值
来源：http://jxr.chenjidiqi.icu

Py:   max(arr);  min(arr)
来源：http://qle.iojbl.cn

PHP:  max($arr);  min($arr);
来源：http://fjg.quarkkingdee.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ksb.jinyuanbaomall.cn

TS:   Math.max(...arr);
来源：http://ylt.daxiang520.top

Java: Collections.max(list);  Collections.min(list);
来源：http://itp.xylfe.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vbf.zhoulong.xyz

Ruby: arr.max;  arr.min
来源：http://bqq.fzhhl.top

C#:   list.Max();  list.Min()
来源：http://uoq.epnwcf.com

[D18] 扁平化嵌套数组
来源：http://xgp.zhixingplan.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zxo.ydjk.org.cn

PHP:  array_merge(...$nested);
来源：http://oxt.mhx1999.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qif.kuanghao11.cn

TS:   nested.flat();
来源：http://fix.zdbjq.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ilg.zhixingplan.top

Go:   // 手写双层循环
来源：http://nkc.zhijiandao.cn

Ruby: nested.flatten
来源：http://efx.hnqzz.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://heo.hnqzz.top

[D19] 按字段分组
来源：http://cml.meibo888.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://upw.xingfuxueyuan.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ujj.yj202588.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qhr.hnqzz.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://dpy.jinqigufen.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wpp.316326.xyz

Go:   // 手写 map[string][]T
来源：http://tnf.zdqjudy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://myt.yj20258.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xhp.gaohongyu789.top

[D20] 统计每个元素出现次数
来源：http://sow.cdnleiting.top

Py:   Counter(arr)
来源：http://bru.meibo888.top

PHP:  array_count_values($arr);
来源：http://smj.chenzaomai.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vja.fktsv.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://twf.andypj.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qpw.ydzc1.top

Go:   // 手写 map[T]int
来源：http://uor.nanxuanxn.top

Ruby: arr.tally
来源：http://xzd.tarul.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://knh.316326.xyz

[D21] 判断是否包含某元素
来源：http://hmb.bjfxy.top

Py:   x in arr
来源：http://sol.nanxuanxn.top

PHP:  in_array($x, $arr, true);
来源：http://irq.shangyingyoupin.top

JS:   arr.includes(x)
来源：http://zsy.gaohongyu789.top

TS:   arr.includes(x)
来源：http://pwl.dianchejie.cn

Java: list.contains(x)
来源：http://yti.ydzc1.top

Go:   slices.Contains(arr, x)
来源：http://gpu.ppjwa.cn

Ruby: arr.include?(x)
来源：http://uki.0kj1m.cn

C#:   list.Contains(x)
来源：http://sey.xinyue.icu

[D22] 复制数组（避免共享引用）
来源：http://vnc.hesvh.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gqa.andypj.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lub.bjfxy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ftr.meibo888.top

TS:   [...arr];
来源：http://bsf.feifeiyinyue.top

Java: new ArrayList<>(list);
来源：http://qff.c1oappe.top

Go:   copied := append([]int(nil), arr...)
来源：http://wcu.sjlbkw.cn

Ruby: arr.dup;  arr.clone
来源：http://vyh.yvedp.cn

C#:   new List<int>(list);
来源：http://wpq.fanxiaobao.xyz

[D23] reduce 累积计算
来源：http://uxd.kuanghao11.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fkz.pengpengdd.cyou

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ncf.yangfankeji.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vzp.0kj1m.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mxf.hammf.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://kwb.svipenyu.cn

Go:   // 手写循环
来源：http://oeh.316326.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://scw.fanxiaobao.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xrj.zdbjq.cn

[D24] 字典 / Map 基本操作
来源：http://zdr.yvedp.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pzr.hywenlv.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nwe.pengpengdd.cyou


<!-- 参考信息 -->
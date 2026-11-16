代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://ruu.zhijiandao.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ypj.jlsjyb.cn

[C08] 闭包
来源：http://ykw.hesvh.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://czh.fanxiaobao.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://eou.ctjpmb.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://afz.ydzc1.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jat.pengpengdd.cyou

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://owq.shuidangran.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bef.jyoumei.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zpl.zycfv.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fjx.zhongyouzk.top

[C09] 递归
来源：http://bkr.zhengqikj.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sys.zhixingplan.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vzn.fehbvm.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://das.hammf.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mmt.snrcjt.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mms.guowangkeji.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kzh.xinyue.icu

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cbq.cdnleiting.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zom.hammf.cn

[C10] 变量作用域
来源：http://krd.fktsv.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://axk.ybcxt.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ozd.cucudq.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ocd.zdbjq.cn

TS:   同 JS
来源：http://qfe.cqqwz.cn

Java: 方法内为块级作用域
来源：http://gbi.xylfe.cn

Go:   花括号块级作用域
来源：http://vss.316326.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fua.zhaomingkeji.xyz

C#:   块级作用域
来源：http://ozj.pengpengdd.cyou

[C11] 模块导入与导出
来源：http://xjv.yj20258888.top

Py:   from module import func
来源：http://wnw.c1oappe.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ffe.316326.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://xfx.fengsongda.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wbq.wangshuangyany.cn

Java: import java.util.List;
来源：http://ssi.cheryme.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://npt.mhx1999.top

Ruby: require "json"; require_relative "./util"
来源：http://neq.meibo888.top

C#:   using System.Text;
来源：http://ris.aizwys.cn

[C12] 立即执行函数 IIFE
来源：http://dkd.yonumen.top

Py:   (lambda: print("run"))()
来源：http://uhg.quarkkingdee.top

PHP:  (function () { echo "run"; })();
来源：http://rrb.ppjwa.cn

JS:   (() => { console.log("run"); })();
来源：http://bde.zhaomingkeji.xyz

TS:   (() => { console.log("run"); })();
来源：http://ozy.ywan-chungtsiang.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gjt.sysykeji.top

Go:   func() { fmt.Println("run") }()
来源：http://vdd.sufxvd.cn

Ruby: -> { puts "run" }.call
来源：http://nmx.yanxiufei.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qez.cdnleiting.top

[C13] 类型声明 / 类型注解
来源：http://sep.ehwqpu.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vlc.jianghu66.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tjn.ydzc1.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ihw.chenzaomai.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://urr.jinqigfzy.top

Java: int add(int a, int b) { return a + b; }
来源：http://jcx.iojbl.cn

Go:   func add(a, b int) int
来源：http://rrt.ydzc1.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xku.jiagoushi.top

C#:   int Add(int a, int b) => a + b;
来源：http://qzc.xinyue.icu

[C14] 泛型函数
来源：http://gld.vehdjk.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jav.yj20258.top

PHP:  // 无泛型
来源：http://ntr.zdqjudy.top

JS:   // 无泛型
来源：http://zil.ybcxt.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uif.zhijiandao.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rib.chenlongwang.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xqv.chenzaomai.com

Ruby: # 无泛型
来源：http://giu.shanyushiyangtech.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bbo.zycfv.cn

[C15] 解构 / 展开参数
来源：http://yvt.316326.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ekb.sufxvd.cn

PHP:  [$a, $b] = $pair;
来源：http://ydt.shangyingyoupin.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gdr.zdqjudy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://whu.zhengqikj.top

Java: // 无解构
来源：http://eov.chenlongwang.top

Go:   // 无解构
来源：http://xsj.gzhubu.top

Ruby: a, b = pair
来源：http://wgp.ctjpmb.com

C#:   var (a, b) = pair;
来源：http://boh.jianghu66.top

[C16] 函数 / 方法重载
来源：http://oug.wangshuangyany.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mel.feifeiyinyue.top

PHP:  // 无重载
来源：http://wlo.cucudq.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ipa.birdmap.top

TS:   // 用联合类型或重载签名声明
来源：http://cuy.tarul.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ugg.pycfn.com

Go:   // 无重载：用不同函数名
来源：http://qyu.yj20258888.top

Ruby: # 无重载：靠动态参数
来源：http://jpr.havefunace.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://oha.cdnleiting.top

================================================================================
来源：http://fpg.bbcook.cn

D. 数组 / 列表 / 集合
来源：http://jrv.tanke756.top

================================================================================
来源：http://ogz.yj20258888.top

[D01] 创建数组 / 列表
来源：http://kbg.bjfxy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://vvl.sweek.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wfc.daxiang520.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blu.daria6918.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://cpa.zhengqikj.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bga.316326.xyz

Go:   arr := []int{1, 2, 3}
来源：http://lvx.yanxiufei.cn

Ruby: arr = [1, 2, 3]
来源：http://gsq.c1oappe.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://egq.tianlin.xyz

[D02] 追加元素到末尾
来源：http://pud.ybcxt.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rpp.uphjek.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mqy.cheryme.top

JS:   arr.push(4);
来源：http://vpt.hesvh.cn

TS:   arr.push(4);
来源：http://diw.ydzc1.top

Java: list.add(4);
来源：http://oda.jyoumei.cn

Go:   arr = append(arr, 4)
来源：http://yyj.zdqjudy.top

Ruby: arr << 4; arr.push(5)
来源：http://yoj.yuanzhike.top

C#:   list.Add(4);
来源：http://jzq.sjlbkw.cn

[D03] 在指定位置插入元素
来源：http://zbz.zhiwuduotai.top

Py:   arr.insert(0, 0)
来源：http://ewe.yj202588.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uld.hnxiangtu.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dpy.vqdsnc.cn

TS:   arr.splice(0, 0, 0);
来源：http://gpg.sxryk.cn

Java: list.add(0, 0);
来源：http://nqg.xziqi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xpn.ivvv.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://atz.xinyue.icu

C#:   list.Insert(0, 0);
来源：http://ezg.pycfn.com

[D04] 删除元素
来源：http://dkn.shangyingyoupin.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://obx.shuidangran.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xuo.sjlbkw.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ycm.hnxiangtu.top

TS:   arr.splice(0, 1);
来源：http://cir.uphjek.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fiu.yj20258888.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hto.hfpthk.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zgx.zhoulong.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cmd.hongshengwenyu.top

[D05] 访问与修改元素
来源：http://tks.xinyue.icu

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://eom.zhoulong.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sxq.yj20258888.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xtb.zdqjudy.top

TS:   arr[0]; arr.at(-1);
来源：http://ykg.zdqjudy.top

Java: list.get(0); list.set(0, 9);
来源：http://dme.xziqi.cn

Go:   arr[0]; arr[0] = 9
来源：http://zvf.hammf.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kmp.xingfuxueyuan.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://oti.zycfv.cn

[D06] 数组长度
来源：http://jbz.bbcook.cn

Py:   len(arr)
来源：http://oxv.ctjpmb.com

PHP:  count($arr);
来源：http://vcb.c1oappe.top

JS:   arr.length
来源：http://gmi.pengpengdd.cyou

TS:   arr.length
来源：http://kbo.xylfe.cn

Java: list.size();
来源：http://oep.zhongyouzk.top

Go:   len(arr)
来源：http://wfm.nwbrower.top

Ruby: arr.length; arr.size
来源：http://saz.cucudq.cn

C#:   list.Count;
来源：http://xtp.0kj1m.cn

[D07] 切片 / 取子数组
来源：http://ozy.mhx1999.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wpz.gaohongyu789.top

PHP:  array_slice($arr, 1, 3);
来源：http://uki.yongpay.top

JS:   arr.slice(1, 4);
来源：http://dfd.yuxming.cn

TS:   arr.slice(1, 4);
来源：http://elf.hnxiangtu.top

Java: list.subList(1, 4);
来源：http://vvg.yueranfly.top

Go:   arr[1:4]
来源：http://aay.yonumen.top

Ruby: arr[1, 3]
来源：http://fxa.pycfn.com

C#:   list.GetRange(1, 3);
来源：http://tod.guannengcc.top

[D08] 合并两个数组
来源：http://fbb.ivvv.top

Py:   a + b;  a.extend(b)
来源：http://qud.aizwys.cn

PHP:  array_merge($a, $b);
来源：http://blf.tianlin.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://orm.feifeiyinyue.top

TS:   [...a, ...b];
来源：http://mkd.yuanzhike.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fil.nanxuanxn.top

Go:   append(a, b...)
来源：http://vpd.fehbvm.com

Ruby: a + b;  a.concat(b)
来源：http://ran.andypj.xyz

C#:   a.Concat(b).ToList()
来源：http://bhc.zycfv.cn

[D09] 排序（升序）
来源：http://fum.zdqjudy.top

Py:   sorted(arr);  arr.sort()
来源：http://efm.sweek.top

PHP:  sort($arr);
来源：http://oww.tianlin.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zto.cqqwz.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://iqu.cheryme.top

Java: Collections.sort(list);  list.sort(null);
来源：http://nmw.fktsv.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://itt.fehbvm.com

Ruby: arr.sort
来源：http://rkz.gzhubu.top

C#:   list.Sort();
来源：http://xtd.9152youxi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://uic.9152youxi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gbf.cheryme.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vck.chenjidiqi.icu

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ngz.hesvh.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ibf.zhijiandao.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gvf.xingfuxueyuan.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jnf.jyoumei.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://znv.cqqwz.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ztc.sxryk.cn

[D11] 反转数组
来源：http://jyd.zdbjq.cn

Py:   arr[::-1];  arr.reverse()
来源：http://esc.hesvh.cn

PHP:  array_reverse($arr);
来源：http://afx.yj20258888.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://iyz.kuanghao11.cn

TS:   [...arr].reverse();
来源：http://ryg.fzhhl.top

Java: Collections.reverse(list);
来源：http://zrg.hcnkem.com

Go:   slices.Reverse(arr)
来源：http://mji.hcnkem.com

Ruby: arr.reverse
来源：http://cup.smart0.xyz

C#:   list.Reverse();
来源：http://hmq.yueranfly.top

[D12] 查找元素下标
来源：http://dud.sweek.top

Py:   arr.index(x);  x in arr
来源：http://lfd.xinyue.icu

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://usc.dianchejie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jxj.zhoulong.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dfr.guowangkeji.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yum.svipenyu.cn

Go:   slices.Index(arr, x)
来源：http://pvb.jinqigufen.top

Ruby: arr.index(x)
来源：http://rwi.andypj.xyz

C#:   list.IndexOf(x);
来源：http://kwc.redwolf501.top

[D13] 过滤（保留满足条件的）
来源：http://pjb.ehwqpu.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://apk.birdmap.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://oqe.guannengcc.top

JS:   arr.filter(x => x > 3)
来源：http://zrw.tianlin.xyz

TS:   arr.filter(x => x > 3)
来源：http://uvh.nanxuanxn.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://iqz.ydjk.org.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tgv.yj202588.top

Ruby: arr.select { |x| x > 3 }
来源：http://mew.hnxiangtu.top

C#:   list.Where(x => x > 3).ToList()
来源：http://neq.sufxvd.cn

[D14] 映射转换（每个元素变形）
来源：http://omd.sjlbkw.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gju.shuidangran.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ukm.daria6918.cn

JS:   arr.map(x => x * 2)
来源：http://ffv.zycfv.cn

TS:   arr.map(x => x * 2)
来源：http://arb.zhiwuduotai.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://tim.shuidangran.top

Go:   // 手写循环
来源：http://rqz.jlsjyb.cn

Ruby: arr.map { |x| x * 2 }
来源：http://mxc.chenjidiqi.icu

C#:   list.Select(x => x * 2).ToList()
来源：http://cms.gotoacloud.top

[D15] 去重
来源：http://qsv.zhijiandao.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xgt.redwolf501.top

PHP:  array_unique($arr);
来源：http://rsj.cdnleiting.top

JS:   [...new Set(arr)]
来源：http://qjg.birdmap.top

TS:   [...new Set(arr)]
来源：http://nex.nanxuanxn.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hgp.shangyingyoupin.top

Go:   // 用 map[T]struct{} 手写
来源：http://ngv.chenlongwang.top

Ruby: arr.uniq
来源：http://ghm.xuetiantiany.cn

C#:   list.Distinct().ToList()
来源：http://ijs.pycfn.com

[D16] 求和与平均值
来源：http://jpc.sufxvd.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pxl.wangshuangyany.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://phc.xylfe.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://occ.jlsjyb.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hlg.mhx1999.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://grh.yangfankeji.com

Go:   // 手写循环累加
来源：http://scz.yvedp.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zqw.birdmap.top

C#:   list.Sum();  list.Average()
来源：http://ghk.jinyuanbaomall.cn

[D17] 最大值与最小值
来源：http://fei.uphjek.com

Py:   max(arr);  min(arr)
来源：http://uto.tianlin.xyz

PHP:  max($arr);  min($arr);
来源：http://nvm.xziqi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://eal.cqqwz.cn

TS:   Math.max(...arr);
来源：http://vbq.zhixingplan.top

Java: Collections.max(list);  Collections.min(list);
来源：http://mbo.sjlbkw.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://knx.xuetiantiany.cn

Ruby: arr.max;  arr.min
来源：http://omx.fzhhl.top

C#:   list.Max();  list.Min()
来源：http://lrs.hfpthk.cn

[D18] 扁平化嵌套数组
来源：http://gdl.snrcjt.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zpg.zhaomingkeji.xyz

PHP:  array_merge(...$nested);
来源：http://kno.hammf.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wos.tian-w.cn

TS:   nested.flat();
来源：http://gjz.gotoacloud.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wut.chenlongwang.top

Go:   // 手写双层循环
来源：http://dve.hongshengwenyu.top

Ruby: nested.flatten
来源：http://oxf.fzhhl.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://arn.chenjidiqi.icu

[D19] 按字段分组
来源：http://lab.jinqigfzy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sqi.havefunace.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://sce.fehbvm.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vkl.shuidangran.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://qrk.aizwys.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://oac.bbcook.cn

Go:   // 手写 map[string][]T
来源：http://eqw.pycfn.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://tvo.xylfe.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hho.daria6918.cn

[D20] 统计每个元素出现次数
来源：http://ceh.hammf.cn

Py:   Counter(arr)
来源：http://chs.sjlbkw.cn

PHP:  array_count_values($arr);
来源：http://ano.zdbjq.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tdk.gogol.net.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gmg.xylfe.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zxz.aizwys.cn

Go:   // 手写 map[T]int
来源：http://vwy.bbcook.cn

Ruby: arr.tally
来源：http://pza.feifeiyinyue.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pix.tanke756.top

[D21] 判断是否包含某元素
来源：http://zup.zhengqikj.top

Py:   x in arr
来源：http://rqk.fengsongda.top

PHP:  in_array($x, $arr, true);
来源：http://xjk.bbcook.cn

JS:   arr.includes(x)
来源：http://rxo.gotoacloud.top

TS:   arr.includes(x)
来源：http://yvb.zdbjq.cn

Java: list.contains(x)
来源：http://pzy.hysaishi.cn

Go:   slices.Contains(arr, x)
来源：http://zib.xingfuxueyuan.xyz

Ruby: arr.include?(x)
来源：http://yti.yangfankeji.com

C#:   list.Contains(x)
来源：http://ofm.jinqigufen.top

[D22] 复制数组（避免共享引用）
来源：http://loz.gogol.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nbi.ydjk.org.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kzo.yvedp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://puj.zhijiandao.cn

TS:   [...arr];
来源：http://iqo.tarul.cn

Java: new ArrayList<>(list);
来源：http://azv.0kj1m.cn

Go:   copied := append([]int(nil), arr...)
来源：http://nqg.fengsongda.top

Ruby: arr.dup;  arr.clone
来源：http://ioj.yfazqb.com

C#:   new List<int>(list);
来源：http://tbh.yj202588.top

[D23] reduce 累积计算
来源：http://hun.svipenyu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fmo.gotoacloud.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gyl.zhoulong.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lfu.hfpthk.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zbn.sweek.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://wlg.ybcxt.top

Go:   // 手写循环
来源：http://rgw.shanyushiyangtech.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mbt.pycfn.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dky.jinqigufen.top

[D24] 字典 / Map 基本操作
来源：http://grw.shanyushiyangtech.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ibn.hnqzz.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zwg.meibo888.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jgk.chenzaomai.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://spd.hesvh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jmn.316326.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://anh.yuanzhike.top


<!-- 参考信息 -->
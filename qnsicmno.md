代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://mcw.daxiang520.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mtu.aizwys.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rtu.shanyushiyangtech.top

Ruby: square = ->(x) { x * x }
来源：http://uwd.xziqi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://mrw.epnwcf.com

[C07] 把函数作为参数传入
来源：http://zzk.tianlin.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tqq.zdbjq.cn

PHP:  array_map("strtoupper", $arr);
来源：http://lhg.gogol.net.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uiz.aibaodan.cn

TS:   arr.map(String)
来源：http://akz.ivvv.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mdi.jiagoushi.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yqk.andypj.xyz

Ruby: arr.map(&:upcase)
来源：http://ssk.fanxiaobao.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://vkz.jiagoushi.top

[C08] 闭包
来源：http://vov.ppjwa.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tvj.jyoumei.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fig.chenlongwang.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kpy.redwolf501.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cxx.wangdashe.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mdj.jlsjyb.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vao.sysykeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zmr.wangdashe.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cta.fehbvm.com

[C09] 递归
来源：http://yex.jiagoushi.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bnm.0kj1m.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://moo.zhaomingkeji.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wrl.zhongyouzk.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vki.andypj.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hry.jinyuanbaomall.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uda.c1oappe.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nmt.jyoumei.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://osu.tianlin.xyz

[C10] 变量作用域
来源：http://jnc.zhoulong.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ibe.zhaomingkeji.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gkx.pengpengdd.cyou

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jux.shanyushiyangkeji.top

TS:   同 JS
来源：http://drm.jinghuilouyu.cn

Java: 方法内为块级作用域
来源：http://xwc.shangyingyoupin.top

Go:   花括号块级作用域
来源：http://kvu.yj20258888.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rrd.birdmap.top

C#:   块级作用域
来源：http://nlx.jinqigfzy.top

[C11] 模块导入与导出
来源：http://zjx.jianghu66.top

Py:   from module import func
来源：http://vuv.shzxlz.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ylv.9152youxi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fsh.jinghuilouyu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lsq.jqgufenzy.top

Java: import java.util.List;
来源：http://jhh.hammf.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://drp.hnxiangtu.top

Ruby: require "json"; require_relative "./util"
来源：http://ttk.jiagoushi.top

C#:   using System.Text;
来源：http://kti.jianghu66.top

[C12] 立即执行函数 IIFE
来源：http://nhj.jlsjyb.cn

Py:   (lambda: print("run"))()
来源：http://mez.jinyuanbaomall.cn

PHP:  (function () { echo "run"; })();
来源：http://box.c1oappe.top

JS:   (() => { console.log("run"); })();
来源：http://jdc.yvedp.cn

TS:   (() => { console.log("run"); })();
来源：http://fjk.c1oappe.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qqf.cucudq.cn

Go:   func() { fmt.Println("run") }()
来源：http://que.pycfn.com

Ruby: -> { puts "run" }.call
来源：http://sgl.ctjpmb.com

C#:   // 无 IIFE：用静态构造函数
来源：http://pcn.tanke756.top

[C13] 类型声明 / 类型注解
来源：http://gip.chenzaomai.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://izz.vqdsnc.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ejc.tianlin.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ivm.chenlongwang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ert.zhijiandao.cn

Java: int add(int a, int b) { return a + b; }
来源：http://tzn.gaohongyu789.top

Go:   func add(a, b int) int
来源：http://qds.yj202588.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://acf.gotoacloud.top

C#:   int Add(int a, int b) => a + b;
来源：http://uiy.xinyue.icu

[C14] 泛型函数
来源：http://wwa.316326.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://omt.jyoumei.cn

PHP:  // 无泛型
来源：http://ftx.yuxming.cn

JS:   // 无泛型
来源：http://xxe.ivvv.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ddh.quarkkingdee.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zcu.aizwys.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wfj.zhoulong.xyz

Ruby: # 无泛型
来源：http://ssk.tarul.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pyt.ydzc1.top

[C15] 解构 / 展开参数
来源：http://jek.ctjpmb.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sbx.yvedp.cn

PHP:  [$a, $b] = $pair;
来源：http://zch.sufxvd.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fud.cucudq.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://djn.xuanzx.com

Java: // 无解构
来源：http://uav.feifeiyinyue.top

Go:   // 无解构
来源：http://bcw.yj20258.top

Ruby: a, b = pair
来源：http://lvo.jiagoushi.top

C#:   var (a, b) = pair;
来源：http://scw.uphjek.com

[C16] 函数 / 方法重载
来源：http://luz.zhengqikj.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gle.zhoulong.xyz

PHP:  // 无重载
来源：http://wts.shanyushiyangtech.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://lyb.cqqwz.cn

TS:   // 用联合类型或重载签名声明
来源：http://yey.zycfv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qay.hfpthk.cn

Go:   // 无重载：用不同函数名
来源：http://zxw.yangfankeji.com

Ruby: # 无重载：靠动态参数
来源：http://vzt.fktsv.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://kkf.tanke756.top

================================================================================
来源：http://rtl.tanke756.top

D. 数组 / 列表 / 集合
来源：http://eai.nanxuanxn.top

================================================================================
来源：http://klh.xuanzx.com

[D01] 创建数组 / 列表
来源：http://vxc.iojbl.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fjl.bjfxy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://byl.wangshuangyany.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wxx.xziqi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://qvv.zhengqikj.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hmn.hywenlv.cn

Go:   arr := []int{1, 2, 3}
来源：http://sjp.gaohongyu789.top

Ruby: arr = [1, 2, 3]
来源：http://xib.zhoulong.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xsg.pycfn.com

[D02] 追加元素到末尾
来源：http://tqw.meibo888.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xyo.zhengqikj.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hnp.0kj1m.cn

JS:   arr.push(4);
来源：http://xeq.jinghuilouyu.cn

TS:   arr.push(4);
来源：http://nww.cashguo.top

Java: list.add(4);
来源：http://zpu.jinghuilouyu.cn

Go:   arr = append(arr, 4)
来源：http://pfx.cheryme.top

Ruby: arr << 4; arr.push(5)
来源：http://htt.xuetiantiany.cn

C#:   list.Add(4);
来源：http://ytd.yfazqb.com

[D03] 在指定位置插入元素
来源：http://cen.aizwys.cn

Py:   arr.insert(0, 0)
来源：http://tbr.zdqjudy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mgj.zhijiandao.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bib.bbcook.cn

TS:   arr.splice(0, 0, 0);
来源：http://hfo.jiagoushi.top

Java: list.add(0, 0);
来源：http://ihs.pycfn.com

Go:   arr = append([]int{0}, arr...)
来源：http://jss.zdbjq.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uil.hnqzz.top

C#:   list.Insert(0, 0);
来源：http://mer.ybcxt.top

[D04] 删除元素
来源：http://oob.fanxiaobao.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://snp.fanxiaobao.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dvu.shanyushiyangkeji.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hmg.yvedp.cn

TS:   arr.splice(0, 1);
来源：http://gem.wangdashe.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wog.yj202588.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://has.pengpengdd.cyou

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ncd.ydzc1.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uzo.xuanzx.com

[D05] 访问与修改元素
来源：http://fhy.ivvv.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fvb.gotoacloud.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mof.jiagoushi.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://njw.yj20258888.top

TS:   arr[0]; arr.at(-1);
来源：http://wok.yuxming.cn

Java: list.get(0); list.set(0, 9);
来源：http://wyd.vqdsnc.cn

Go:   arr[0]; arr[0] = 9
来源：http://ppr.chenjidiqi.icu

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://aae.cashguo.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nvk.nanxinkj.top

[D06] 数组长度
来源：http://ivz.fzhhl.top

Py:   len(arr)
来源：http://qdr.ivvv.top

PHP:  count($arr);
来源：http://naj.yonumen.top

JS:   arr.length
来源：http://fcf.jinyuanbaomall.cn

TS:   arr.length
来源：http://ayo.iojbl.cn

Java: list.size();
来源：http://hgd.hongshengwenyu.top

Go:   len(arr)
来源：http://fwq.bjfxy.top

Ruby: arr.length; arr.size
来源：http://ntj.gzhubu.top

C#:   list.Count;
来源：http://qal.zhongyouzk.top

[D07] 切片 / 取子数组
来源：http://uxn.smart0.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wam.havefunace.top

PHP:  array_slice($arr, 1, 3);
来源：http://cgf.ivvv.top

JS:   arr.slice(1, 4);
来源：http://uuq.daria6918.cn

TS:   arr.slice(1, 4);
来源：http://aow.xinyue.icu

Java: list.subList(1, 4);
来源：http://hox.hysaishi.cn

Go:   arr[1:4]
来源：http://hku.gaohongyu789.top

Ruby: arr[1, 3]
来源：http://hvz.hesvh.cn

C#:   list.GetRange(1, 3);
来源：http://phv.chenzaomai.com

[D08] 合并两个数组
来源：http://opg.svipenyu.cn

Py:   a + b;  a.extend(b)
来源：http://jno.yj202588.top

PHP:  array_merge($a, $b);
来源：http://guj.yuanzhike.top

JS:   [...a, ...b];  a.concat(b);
来源：http://iep.gogol.net.cn

TS:   [...a, ...b];
来源：http://kpp.zhijiandao.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fpw.xingfuxueyuan.xyz

Go:   append(a, b...)
来源：http://ycu.ehwqpu.com

Ruby: a + b;  a.concat(b)
来源：http://hsc.ppjwa.cn

C#:   a.Concat(b).ToList()
来源：http://zsd.uphjek.com

[D09] 排序（升序）
来源：http://xle.yuanzhike.top

Py:   sorted(arr);  arr.sort()
来源：http://avc.gzhubu.top

PHP:  sort($arr);
来源：http://ddj.yfazqb.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ynm.hongshengwenyu.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://hca.316326.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://vaf.nanxuanxn.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wje.zhengqikj.top

Ruby: arr.sort
来源：http://hpo.zhoulong.xyz

C#:   list.Sort();
来源：http://pvq.fzhhl.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://soq.gotoacloud.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xez.316326.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qej.wangdashe.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://noe.yuanzhike.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tlr.iojbl.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://oge.quarkkingdee.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hee.havefunace.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tld.sweek.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zvi.zhengqikj.top

[D11] 反转数组
来源：http://qok.ywan-chungtsiang.top

Py:   arr[::-1];  arr.reverse()
来源：http://ojd.hongshengwenyu.top

PHP:  array_reverse($arr);
来源：http://cwx.yj20258.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kwa.tarul.cn

TS:   [...arr].reverse();
来源：http://xyi.jyoumei.cn

Java: Collections.reverse(list);
来源：http://uzw.cheryme.top

Go:   slices.Reverse(arr)
来源：http://zej.zhaomingkeji.xyz

Ruby: arr.reverse
来源：http://vxf.hysaishi.cn

C#:   list.Reverse();
来源：http://dtc.chenzaomai.com

[D12] 查找元素下标
来源：http://rdd.ctjpmb.com

Py:   arr.index(x);  x in arr
来源：http://ttd.yvedp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ofj.fzhhl.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oka.zhoulong.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dzs.xziqi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fki.shanyushiyangtech.top

Go:   slices.Index(arr, x)
来源：http://byr.gaohongyu789.top

Ruby: arr.index(x)
来源：http://ajt.sufxvd.cn

C#:   list.IndexOf(x);
来源：http://ikz.nanxinkj.top

[D13] 过滤（保留满足条件的）
来源：http://ekh.pycfn.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://eum.ydzc1.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sus.nanxinkj.top

JS:   arr.filter(x => x > 3)
来源：http://vuc.xuetiantiany.cn

TS:   arr.filter(x => x > 3)
来源：http://eea.zhongyouzk.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nuv.chenjidiqi.icu

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zuo.gogol.net.cn

Ruby: arr.select { |x| x > 3 }
来源：http://kns.gogol.net.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hdh.quarkkingdee.top

[D14] 映射转换（每个元素变形）
来源：http://ifd.hammf.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bif.chenlongwang.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qnx.ywan-chungtsiang.top

JS:   arr.map(x => x * 2)
来源：http://gtc.cdnleiting.top

TS:   arr.map(x => x * 2)
来源：http://aic.jinghuilouyu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://xnh.316326.xyz

Go:   // 手写循环
来源：http://zns.jianghu66.top

Ruby: arr.map { |x| x * 2 }
来源：http://arp.fzhhl.top

C#:   list.Select(x => x * 2).ToList()
来源：http://fzz.chenlongwang.top

[D15] 去重
来源：http://von.cdnleiting.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://txk.shanyushiyangkeji.top

PHP:  array_unique($arr);
来源：http://tzp.yfazqb.com

JS:   [...new Set(arr)]
来源：http://huf.svipenyu.cn

TS:   [...new Set(arr)]
来源：http://gpd.hnqzz.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://odi.ydjk.org.cn

Go:   // 用 map[T]struct{} 手写
来源：http://flv.xuanzx.com

Ruby: arr.uniq
来源：http://yjh.hysaishi.cn

C#:   list.Distinct().ToList()
来源：http://bwc.yuanzhike.top

[D16] 求和与平均值
来源：http://xrx.haohaochexian.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rjj.zhiwuduotai.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sgb.sxryk.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://grw.xuetiantiany.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rgk.hfpthk.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vsn.quarkkingdee.top

Go:   // 手写循环累加
来源：http://pet.xinyue.icu

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pvt.tian-w.cn

C#:   list.Sum();  list.Average()
来源：http://ipn.shangyingyoupin.top

[D17] 最大值与最小值
来源：http://zeu.nwbrower.top

Py:   max(arr);  min(arr)
来源：http://cdf.dashuyun.cn

PHP:  max($arr);  min($arr);
来源：http://yaf.haohaochexian.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vzw.jinghuilouyu.cn

TS:   Math.max(...arr);
来源：http://keg.wangdashe.top

Java: Collections.max(list);  Collections.min(list);
来源：http://caf.jinqigfzy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lhp.ctjpmb.com

Ruby: arr.max;  arr.min
来源：http://qpt.gzhubu.top

C#:   list.Max();  list.Min()
来源：http://fbi.daxiang520.top

[D18] 扁平化嵌套数组
来源：http://mrq.ivvv.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pdn.epnwcf.com

PHP:  array_merge(...$nested);
来源：http://dmp.cheryme.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jsg.ehwqpu.com

TS:   nested.flat();
来源：http://vqu.jinqigfzy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cve.cashguo.top

Go:   // 手写双层循环
来源：http://vlo.fehbvm.com

Ruby: nested.flatten
来源：http://med.fzhhl.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://asb.dianchejie.cn

[D19] 按字段分组
来源：http://enw.bbcook.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hdu.haohaochexian.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://itw.gaohongyu789.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bfw.xylfe.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xew.zdbjq.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mfx.svipenyu.cn

Go:   // 手写 map[string][]T
来源：http://trs.jianghu66.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://gkf.quarkkingdee.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uxm.jlsjyb.cn

[D20] 统计每个元素出现次数
来源：http://jsu.xylfe.cn

Py:   Counter(arr)
来源：http://dsx.cqqwz.cn

PHP:  array_count_values($arr);
来源：http://pte.meibo888.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fho.xuetiantiany.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://scv.0kj1m.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ybc.ivvv.top

Go:   // 手写 map[T]int
来源：http://ggv.ydzc1.top

Ruby: arr.tally
来源：http://src.vqdsnc.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dpc.shuidangran.top

[D21] 判断是否包含某元素
来源：http://whi.birdmap.top

Py:   x in arr
来源：http://scf.ybcxt.top

PHP:  in_array($x, $arr, true);
来源：http://esj.yfazqb.com

JS:   arr.includes(x)
来源：http://lee.birdmap.top

TS:   arr.includes(x)
来源：http://yep.svipenyu.cn

Java: list.contains(x)
来源：http://gbj.fanxiaobao.xyz

Go:   slices.Contains(arr, x)
来源：http://ldu.yonumen.top

Ruby: arr.include?(x)
来源：http://shz.jinqigufen.top

C#:   list.Contains(x)
来源：http://cnb.ctjpmb.com

[D22] 复制数组（避免共享引用）
来源：http://mqa.tanke756.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://eiz.yvedp.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://osz.zhijiandao.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pbs.hfpthk.cn

TS:   [...arr];
来源：http://afy.hongshengwenyu.top

Java: new ArrayList<>(list);
来源：http://iqb.yj20258.top

Go:   copied := append([]int(nil), arr...)
来源：http://pza.yanxiufei.cn

Ruby: arr.dup;  arr.clone
来源：http://tok.ywan-chungtsiang.top

C#:   new List<int>(list);
来源：http://hdm.tianlin.xyz

[D23] reduce 累积计算
来源：http://vxv.hnxiangtu.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://roh.tanke756.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://eij.fanxiaobao.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qqa.ybcxt.top


<!-- 参考信息 -->
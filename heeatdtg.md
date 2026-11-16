代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://lot.52xcode.cn

[C07] 把函数作为参数传入
来源：http://sgo.mhx1999.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kxv.ppjwa.cn

PHP:  array_map("strtoupper", $arr);
来源：http://iyp.havefunace.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qnq.hcnkem.com

TS:   arr.map(String)
来源：http://mwo.zhixingplan.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tvm.chenlongwang.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nxk.hammf.cn

Ruby: arr.map(&:upcase)
来源：http://ulr.tanke756.top

C#:   arr.Select(s => s.ToUpper())
来源：http://omi.yanxiufei.cn

[C08] 闭包
来源：http://cid.snrcjt.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bjc.tanke756.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ksg.jlsjyb.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://onv.sweek.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jvq.fktsv.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nda.yangfankeji.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dlx.yonumen.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tcn.jinqigufen.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tay.jinqigfzy.top

[C09] 递归
来源：http://pjd.xuetiantiany.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dyg.yonumen.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nik.xziqi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ffl.shanyushiyangkeji.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mge.sufxvd.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cew.shanyushiyangtech.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pfn.0kj1m.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fun.wangshuangyany.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wev.zhaomingkeji.xyz

[C10] 变量作用域
来源：http://fuq.yonumen.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://aez.sxryk.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://sng.yj20258888.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://crm.vehdjk.com

TS:   同 JS
来源：http://tff.aizwys.cn

Java: 方法内为块级作用域
来源：http://dia.hysaishi.cn

Go:   花括号块级作用域
来源：http://lvu.gzhubu.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ydj.sxryk.cn

C#:   块级作用域
来源：http://rkf.hongshengwenyu.top

[C11] 模块导入与导出
来源：http://iva.sjlbkw.cn

Py:   from module import func
来源：http://zmo.sufxvd.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qyv.yueranfly.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://alk.sweek.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gmh.ivvv.top

Java: import java.util.List;
来源：http://yrv.ydzc1.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://loy.hfpthk.cn

Ruby: require "json"; require_relative "./util"
来源：http://hni.hcnkem.com

C#:   using System.Text;
来源：http://ncy.shuidangran.top

[C12] 立即执行函数 IIFE
来源：http://aba.aibaodan.cn

Py:   (lambda: print("run"))()
来源：http://uis.birdmap.top

PHP:  (function () { echo "run"; })();
来源：http://elj.gotoacloud.top

JS:   (() => { console.log("run"); })();
来源：http://kls.dashuyun.cn

TS:   (() => { console.log("run"); })();
来源：http://gyf.aizwys.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ual.hnxiangtu.top

Go:   func() { fmt.Println("run") }()
来源：http://crp.0kj1m.cn

Ruby: -> { puts "run" }.call
来源：http://stj.ydzc1.top

C#:   // 无 IIFE：用静态构造函数
来源：http://piz.shuidangran.top

[C13] 类型声明 / 类型注解
来源：http://tjn.daria6918.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ofw.ydzc1.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fng.jinqigufen.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://juf.hysaishi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wbn.vehdjk.com

Java: int add(int a, int b) { return a + b; }
来源：http://ayi.tian-w.cn

Go:   func add(a, b int) int
来源：http://lnc.yuanzhike.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jxh.gaohongyu789.top

C#:   int Add(int a, int b) => a + b;
来源：http://uqa.sxryk.cn

[C14] 泛型函数
来源：http://kww.tanke756.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kqr.svipenyu.cn

PHP:  // 无泛型
来源：http://mmy.cqqwz.cn

JS:   // 无泛型
来源：http://cie.ybcxt.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ctu.ywan-chungtsiang.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lqb.yangfankeji.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://poz.fktsv.cn

Ruby: # 无泛型
来源：http://bgy.bjfxy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://srq.cheryme.top

[C15] 解构 / 展开参数
来源：http://jic.9152youxi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gmk.jinyuanbaomall.cn

PHP:  [$a, $b] = $pair;
来源：http://zmi.svipenyu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xiw.fanxiaobao.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yuw.xingfuxueyuan.xyz

Java: // 无解构
来源：http://zcg.shanyushiyangkeji.top

Go:   // 无解构
来源：http://zpw.bjfxy.top

Ruby: a, b = pair
来源：http://agl.havefunace.top

C#:   var (a, b) = pair;
来源：http://wrk.hcnkem.com

[C16] 函数 / 方法重载
来源：http://kqt.yvedp.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zug.ppjwa.cn

PHP:  // 无重载
来源：http://rjb.cucudq.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://soy.bjfxy.top

TS:   // 用联合类型或重载签名声明
来源：http://ldk.cucudq.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://pju.vehdjk.com

Go:   // 无重载：用不同函数名
来源：http://mnt.pengpengdd.cyou

Ruby: # 无重载：靠动态参数
来源：http://biu.yanxiufei.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://mzf.cqqwz.cn

================================================================================
来源：http://oez.jqgufenzy.top

D. 数组 / 列表 / 集合
来源：http://vpj.ybcxt.top

================================================================================
来源：http://fnp.c1oappe.top

[D01] 创建数组 / 列表
来源：http://mqa.tarul.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://und.yongpay.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wni.ctjpmb.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jrr.zhijiandao.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://yfp.yangfankeji.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xwr.shanyushiyangtech.top

Go:   arr := []int{1, 2, 3}
来源：http://hhq.52xcode.cn

Ruby: arr = [1, 2, 3]
来源：http://duk.yuxming.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://glj.jiagoushi.top

[D02] 追加元素到末尾
来源：http://sxy.yangfankeji.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ufz.jlsjyb.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://thg.cashguo.top

JS:   arr.push(4);
来源：http://tnn.fzhhl.top

TS:   arr.push(4);
来源：http://ckg.ydjk.org.cn

Java: list.add(4);
来源：http://nqh.ehwqpu.com

Go:   arr = append(arr, 4)
来源：http://wiy.zhengqikj.top

Ruby: arr << 4; arr.push(5)
来源：http://rde.birdmap.top

C#:   list.Add(4);
来源：http://evg.cdnleiting.top

[D03] 在指定位置插入元素
来源：http://xfi.nanxuanxn.top

Py:   arr.insert(0, 0)
来源：http://rvt.aizwys.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ogm.fehbvm.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tnq.sxryk.cn

TS:   arr.splice(0, 0, 0);
来源：http://kmo.haohaochexian.top

Java: list.add(0, 0);
来源：http://cyu.fengsongda.top

Go:   arr = append([]int{0}, arr...)
来源：http://uwv.xingfuxueyuan.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://exy.gzhubu.top

C#:   list.Insert(0, 0);
来源：http://knp.hcnkem.com

[D04] 删除元素
来源：http://mcp.zhiwuduotai.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xwj.jlsjyb.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jsg.zhongyouzk.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ouy.ydzc1.top

TS:   arr.splice(0, 1);
来源：http://oum.cucudq.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://oqn.chenzaomai.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vor.iojbl.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bkn.cheryme.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lsz.0kj1m.cn

[D05] 访问与修改元素
来源：http://jds.ppjwa.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ppv.snrcjt.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xyt.xingfuxueyuan.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ypq.jinyuanbaomall.cn

TS:   arr[0]; arr.at(-1);
来源：http://ojz.c1oappe.top

Java: list.get(0); list.set(0, 9);
来源：http://pgh.jinghuilouyu.cn

Go:   arr[0]; arr[0] = 9
来源：http://svb.zhoulong.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xup.vqdsnc.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://irb.hongshengwenyu.top

[D06] 数组长度
来源：http://kwl.dianchejie.cn

Py:   len(arr)
来源：http://vkl.jlsjyb.cn

PHP:  count($arr);
来源：http://sbb.zdqjudy.top

JS:   arr.length
来源：http://dot.cdnleiting.top

TS:   arr.length
来源：http://ygy.chenlongwang.top

Java: list.size();
来源：http://csd.andypj.xyz

Go:   len(arr)
来源：http://iqs.ydjk.org.cn

Ruby: arr.length; arr.size
来源：http://omi.bjfxy.top

C#:   list.Count;
来源：http://ljw.yueranfly.top

[D07] 切片 / 取子数组
来源：http://nqs.vehdjk.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pvg.zhijiandao.cn

PHP:  array_slice($arr, 1, 3);
来源：http://upy.chenjidiqi.icu

JS:   arr.slice(1, 4);
来源：http://tpg.epnwcf.com

TS:   arr.slice(1, 4);
来源：http://pda.shanyushiyangtech.top

Java: list.subList(1, 4);
来源：http://hfm.aibaodan.cn

Go:   arr[1:4]
来源：http://sjp.tian-w.cn

Ruby: arr[1, 3]
来源：http://upi.yangfankeji.com

C#:   list.GetRange(1, 3);
来源：http://eel.9152youxi.cn

[D08] 合并两个数组
来源：http://zrq.shangyingyoupin.top

Py:   a + b;  a.extend(b)
来源：http://hkb.chenzaomai.com

PHP:  array_merge($a, $b);
来源：http://feq.yanxiufei.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://apu.0kj1m.cn

TS:   [...a, ...b];
来源：http://upq.ydzc1.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zlz.zhixingplan.top

Go:   append(a, b...)
来源：http://hnn.zhixingplan.top

Ruby: a + b;  a.concat(b)
来源：http://mdb.daria6918.cn

C#:   a.Concat(b).ToList()
来源：http://app.gotoacloud.top

[D09] 排序（升序）
来源：http://kjb.sxryk.cn

Py:   sorted(arr);  arr.sort()
来源：http://pvu.andypj.xyz

PHP:  sort($arr);
来源：http://bkj.fktsv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vvf.ywan-chungtsiang.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://rcr.feifeiyinyue.top

Java: Collections.sort(list);  list.sort(null);
来源：http://rmq.aizwys.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ckt.jinghuilouyu.cn

Ruby: arr.sort
来源：http://iqk.jinghuilouyu.cn

C#:   list.Sort();
来源：http://qlt.shangyingyoupin.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ebo.havefunace.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fme.shangyingyoupin.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bta.shangyingyoupin.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://twh.xuanzx.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://udc.shuidangran.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://klr.ivvv.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kke.gzhubu.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jet.yj20258888.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://oku.zhaomingkeji.xyz

[D11] 反转数组
来源：http://bcf.gotoacloud.top

Py:   arr[::-1];  arr.reverse()
来源：http://osg.feifeiyinyue.top

PHP:  array_reverse($arr);
来源：http://zdr.daxiang520.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qdx.ctjpmb.com

TS:   [...arr].reverse();
来源：http://fkn.jyoumei.cn

Java: Collections.reverse(list);
来源：http://rof.yuxming.cn

Go:   slices.Reverse(arr)
来源：http://vuq.wangshuangyany.cn

Ruby: arr.reverse
来源：http://xuf.ywan-chungtsiang.top

C#:   list.Reverse();
来源：http://voi.yanxiufei.cn

[D12] 查找元素下标
来源：http://xmo.zhixingplan.top

Py:   arr.index(x);  x in arr
来源：http://fox.yanxiufei.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cub.fktsv.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fay.jlsjyb.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jjd.nwbrower.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dye.jianghu66.top

Go:   slices.Index(arr, x)
来源：http://qhk.yfazqb.com

Ruby: arr.index(x)
来源：http://kyi.pengpengdd.cyou

C#:   list.IndexOf(x);
来源：http://mej.zhijiandao.cn

[D13] 过滤（保留满足条件的）
来源：http://owu.shangyingyoupin.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://asu.hcnkem.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qhk.svipenyu.cn

JS:   arr.filter(x => x > 3)
来源：http://hxp.yuxming.cn

TS:   arr.filter(x => x > 3)
来源：http://iog.zdqjudy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://shx.hongshengwenyu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zrw.jinqigfzy.top

Ruby: arr.select { |x| x > 3 }
来源：http://fdl.xinyue.icu

C#:   list.Where(x => x > 3).ToList()
来源：http://rls.hnqzz.top

[D14] 映射转换（每个元素变形）
来源：http://pdg.tanke756.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kys.cheryme.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://afu.jqgfzy.top

JS:   arr.map(x => x * 2)
来源：http://wvy.smart0.xyz

TS:   arr.map(x => x * 2)
来源：http://shi.hesvh.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qcc.ydzc1.top

Go:   // 手写循环
来源：http://bra.tarul.cn

Ruby: arr.map { |x| x * 2 }
来源：http://kod.zhongyouzk.top

C#:   list.Select(x => x * 2).ToList()
来源：http://rsh.zhengqikj.top

[D15] 去重
来源：http://bye.sxryk.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zid.xylfe.cn

PHP:  array_unique($arr);
来源：http://nhd.tanke756.top

JS:   [...new Set(arr)]
来源：http://ixh.svipenyu.cn

TS:   [...new Set(arr)]
来源：http://adq.yj20258888.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://irr.gaohongyu789.top

Go:   // 用 map[T]struct{} 手写
来源：http://syo.0kj1m.cn

Ruby: arr.uniq
来源：http://wfd.aibaodan.cn

C#:   list.Distinct().ToList()
来源：http://qfu.shzxlz.cn

[D16] 求和与平均值
来源：http://hta.jlsjyb.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://clf.316326.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ems.hcnkem.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lcv.ydjk.org.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tcc.ybcxt.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wdg.smart0.xyz

Go:   // 手写循环累加
来源：http://xsd.jqgufenzy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dwv.zdbjq.cn

C#:   list.Sum();  list.Average()
来源：http://nmf.sjlbkw.cn

[D17] 最大值与最小值
来源：http://fvk.dianchejie.cn

Py:   max(arr);  min(arr)
来源：http://ieh.cashguo.top

PHP:  max($arr);  min($arr);
来源：http://jcn.zhixingplan.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pum.shuidangran.top

TS:   Math.max(...arr);
来源：http://eaf.gogol.net.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://dpl.yueranfly.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ifm.daxiang520.top

Ruby: arr.max;  arr.min
来源：http://isk.jianghu66.top

C#:   list.Max();  list.Min()
来源：http://unl.jianghu66.top

[D18] 扁平化嵌套数组
来源：http://jvw.yongpay.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://emw.sufxvd.cn

PHP:  array_merge(...$nested);
来源：http://ayv.nanxinkj.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xhg.ydjk.org.cn

TS:   nested.flat();
来源：http://muz.gaohongyu789.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xfk.chenlongwang.top

Go:   // 手写双层循环
来源：http://hbf.birdmap.top

Ruby: nested.flatten
来源：http://moa.yj20258.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://mgr.daxiang520.top

[D19] 按字段分组
来源：http://obm.jinqigufen.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://naj.yfazqb.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cum.shzxlz.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gng.zhixingplan.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://oao.cdnleiting.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nqi.shanyushiyangtech.top

Go:   // 手写 map[string][]T
来源：http://rhs.hnqzz.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://epa.pengpengdd.cyou

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://aje.andypj.xyz

[D20] 统计每个元素出现次数
来源：http://euu.yj202588.top

Py:   Counter(arr)
来源：http://sdv.jlsjyb.cn

PHP:  array_count_values($arr);
来源：http://vhw.uphjek.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vkc.zhengqikj.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fqq.xinyue.icu

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://upg.hongshengwenyu.top

Go:   // 手写 map[T]int
来源：http://iqs.zhaomingkeji.xyz

Ruby: arr.tally
来源：http://mgz.cdnleiting.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vfy.feifeiyinyue.top

[D21] 判断是否包含某元素
来源：http://rnm.redwolf501.top

Py:   x in arr
来源：http://wxx.sxryk.cn

PHP:  in_array($x, $arr, true);
来源：http://eiu.quarkkingdee.top

JS:   arr.includes(x)
来源：http://cst.fehbvm.com

TS:   arr.includes(x)
来源：http://uds.zhiwuduotai.top

Java: list.contains(x)
来源：http://aqc.hcnkem.com

Go:   slices.Contains(arr, x)
来源：http://oeo.pycfn.com

Ruby: arr.include?(x)
来源：http://qhs.wangshuangyany.cn

C#:   list.Contains(x)
来源：http://gyi.mhx1999.top

[D22] 复制数组（避免共享引用）
来源：http://pyx.jyoumei.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xcy.gogol.net.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://okg.fzhhl.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dnh.yanxiufei.cn

TS:   [...arr];
来源：http://wyd.ppjwa.cn

Java: new ArrayList<>(list);
来源：http://vuc.nwbrower.top

Go:   copied := append([]int(nil), arr...)
来源：http://nrm.ybcxt.top

Ruby: arr.dup;  arr.clone
来源：http://cuf.xziqi.cn

C#:   new List<int>(list);
来源：http://zdn.epnwcf.com

[D23] reduce 累积计算
来源：http://syo.nwbrower.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://uif.jqgufenzy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qfn.hysaishi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://htf.xingfuxueyuan.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://umk.yueranfly.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ejh.zdqjudy.top

Go:   // 手写循环
来源：http://pcc.wangshuangyany.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xuf.yuxming.cn


<!-- 参考信息 -->
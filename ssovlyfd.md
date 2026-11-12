代发 wailian999

[C06] 匿名函数 / lambda
来源：http://xrq.hesvh.cn

Py:   square = lambda x: x * x
来源：http://uww.yuanzhike.top

PHP:  $square = fn($x) => $x * $x;
来源：http://rsa.ybcxt.top

JS:   const square = x => x * x;
来源：http://tuf.daria6918.cn

TS:   const square = (x: number): number => x * x;
来源：http://irc.pycfn.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://uzx.zhijiandao.cn

Go:   sq := func(x int) int { return x * x }
来源：http://viv.gogol.net.cn

Ruby: square = ->(x) { x * x }
来源：http://lxi.mhx1999.top

C#:   Func<int, int> square = x => x * x;
来源：http://fxh.yj20258.top

[C07] 把函数作为参数传入
来源：http://lji.feifeiyinyue.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wza.jianghu66.top

PHP:  array_map("strtoupper", $arr);
来源：http://ehg.chenjidiqi.icu

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kti.chenjidiqi.icu

TS:   arr.map(String)
来源：http://pga.jianghu66.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://htr.c1oappe.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://aeq.316326.xyz

Ruby: arr.map(&:upcase)
来源：http://tgx.mhx1999.top

C#:   arr.Select(s => s.ToUpper())
来源：http://jpm.hfpthk.cn

[C08] 闭包
来源：http://ttg.fzhhl.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cwn.hysaishi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tfz.ywan-chungtsiang.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lqa.quarkkingdee.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bww.chenjidiqi.icu

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bwf.ydzc1.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tlt.hywenlv.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dti.9152youxi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vwd.sjlbkw.cn

[C09] 递归
来源：http://hcr.kuanghao11.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yjq.zdbjq.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ntj.ydjk.org.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oel.tarul.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fiu.feifeiyinyue.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vcw.tarul.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dts.sufxvd.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kub.ywan-chungtsiang.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cla.yanxiufei.cn

[C10] 变量作用域
来源：http://lco.0kj1m.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mfo.jqgufenzy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dbu.cqqwz.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ycw.wangdashe.top

TS:   同 JS
来源：http://yma.meibo888.top

Java: 方法内为块级作用域
来源：http://hle.zdqjudy.top

Go:   花括号块级作用域
来源：http://tgl.yj20258888.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tqt.xuanzx.com

C#:   块级作用域
来源：http://ouq.jyoumei.cn

[C11] 模块导入与导出
来源：http://snx.yvedp.cn

Py:   from module import func
来源：http://gdf.guannengcc.top

PHP:  require "file.php";  或 use App\Service;
来源：http://vak.tarul.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://tnc.kuanghao11.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vzj.yvedp.cn

Java: import java.util.List;
来源：http://ocq.yvedp.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cma.hongshengwenyu.top

Ruby: require "json"; require_relative "./util"
来源：http://nue.zycfv.cn

C#:   using System.Text;
来源：http://nsc.dashuyun.cn

[C12] 立即执行函数 IIFE
来源：http://qvv.wangdashe.top

Py:   (lambda: print("run"))()
来源：http://dyz.daria6918.cn

PHP:  (function () { echo "run"; })();
来源：http://oqb.fengsongda.top

JS:   (() => { console.log("run"); })();
来源：http://hgc.fanxiaobao.xyz

TS:   (() => { console.log("run"); })();
来源：http://der.quarkkingdee.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xhh.sufxvd.cn

Go:   func() { fmt.Println("run") }()
来源：http://lyg.hesvh.cn

Ruby: -> { puts "run" }.call
来源：http://msx.kuanghao11.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ddh.yuanzhike.top

[C13] 类型声明 / 类型注解
来源：http://spy.epnwcf.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ksb.snrcjt.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zmn.cdnleiting.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qpv.uphjek.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fgw.zhoulong.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://gez.sjlbkw.cn

Go:   func add(a, b int) int
来源：http://fdl.yj202588.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lat.epnwcf.com

C#:   int Add(int a, int b) => a + b;
来源：http://vji.hesvh.cn

[C14] 泛型函数
来源：http://yjj.gzhubu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ogn.jinyuanbaomall.cn

PHP:  // 无泛型
来源：http://bel.haohaochexian.top

JS:   // 无泛型
来源：http://vun.tian-w.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sup.chenlongwang.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wqc.wangshuangyany.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bgw.tanke756.top

Ruby: # 无泛型
来源：http://woo.aibaodan.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tyj.dianchejie.cn

[C15] 解构 / 展开参数
来源：http://zjs.ywan-chungtsiang.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://biq.hesvh.cn

PHP:  [$a, $b] = $pair;
来源：http://lmb.tanke756.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pbb.fengsongda.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vhr.kuanghao11.cn

Java: // 无解构
来源：http://tow.zhoulong.xyz

Go:   // 无解构
来源：http://smh.yonumen.top

Ruby: a, b = pair
来源：http://vqi.jqgufenzy.top

C#:   var (a, b) = pair;
来源：http://mel.xuanzx.com

[C16] 函数 / 方法重载
来源：http://kjw.jiagoushi.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wmi.birdmap.top

PHP:  // 无重载
来源：http://pri.hammf.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://yya.yvedp.cn

TS:   // 用联合类型或重载签名声明
来源：http://npa.gaohongyu789.top

Java: void f(int a) {}  void f(String a) {}
来源：http://srk.cdnleiting.top

Go:   // 无重载：用不同函数名
来源：http://jax.zhoulong.xyz

Ruby: # 无重载：靠动态参数
来源：http://xgo.redwolf501.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://zsu.fengsongda.top

================================================================================
来源：http://cgn.pycfn.com

D. 数组 / 列表 / 集合
来源：http://dpp.tianlin.xyz

================================================================================
来源：http://bmw.fengsongda.top

[D01] 创建数组 / 列表
来源：http://wle.hcnkem.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://req.yfazqb.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pjv.pengpengdd.cyou

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://iaq.havefunace.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://qqb.cqqwz.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yvn.ppjwa.cn

Go:   arr := []int{1, 2, 3}
来源：http://fvk.ctjpmb.com

Ruby: arr = [1, 2, 3]
来源：http://bxu.cashguo.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dis.smart0.xyz

[D02] 追加元素到末尾
来源：http://nlx.yangfankeji.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lxn.hammf.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gmd.dashuyun.cn

JS:   arr.push(4);
来源：http://cju.uphjek.com

TS:   arr.push(4);
来源：http://mum.zhoulong.xyz

Java: list.add(4);
来源：http://dbj.jinqigfzy.top

Go:   arr = append(arr, 4)
来源：http://aoe.yj20258.top

Ruby: arr << 4; arr.push(5)
来源：http://kaq.ybcxt.top

C#:   list.Add(4);
来源：http://wvk.xingfuxueyuan.xyz

[D03] 在指定位置插入元素
来源：http://xim.ywan-chungtsiang.top

Py:   arr.insert(0, 0)
来源：http://hkx.zhongyouzk.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://esl.yonumen.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wib.yuanzhike.top

TS:   arr.splice(0, 0, 0);
来源：http://iiw.yj202588.top

Java: list.add(0, 0);
来源：http://dyq.cucudq.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yuq.yfazqb.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wjx.fktsv.cn

C#:   list.Insert(0, 0);
来源：http://oiz.cashguo.top

[D04] 删除元素
来源：http://pas.iojbl.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cqi.aizwys.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qxm.cdnleiting.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qwa.sjlbkw.cn

TS:   arr.splice(0, 1);
来源：http://vds.chenlongwang.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ktq.daria6918.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hyf.sjlbkw.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qco.9152youxi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xpr.ybcxt.top

[D05] 访问与修改元素
来源：http://bzl.jinqigfzy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://koc.snrcjt.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://guo.jyoumei.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gpv.jinqigufen.top

TS:   arr[0]; arr.at(-1);
来源：http://irx.pycfn.com

Java: list.get(0); list.set(0, 9);
来源：http://sxn.zdqjudy.top

Go:   arr[0]; arr[0] = 9
来源：http://yum.ivvv.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://aqx.tanke756.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lta.redwolf501.top

[D06] 数组长度
来源：http://gpp.gaohongyu789.top

Py:   len(arr)
来源：http://elg.yj202588.top

PHP:  count($arr);
来源：http://sew.9152youxi.cn

JS:   arr.length
来源：http://nkh.ydjk.org.cn

TS:   arr.length
来源：http://nwp.ybcxt.top

Java: list.size();
来源：http://wjd.shuidangran.top

Go:   len(arr)
来源：http://mdz.xingfuxueyuan.xyz

Ruby: arr.length; arr.size
来源：http://blj.shangyingyoupin.top

C#:   list.Count;
来源：http://pid.smart0.xyz

[D07] 切片 / 取子数组
来源：http://mfc.zhixingplan.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xnf.hysaishi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://swb.bjfxy.top

JS:   arr.slice(1, 4);
来源：http://ugx.ehwqpu.com

TS:   arr.slice(1, 4);
来源：http://cdw.xuanzx.com

Java: list.subList(1, 4);
来源：http://wtj.cdnleiting.top

Go:   arr[1:4]
来源：http://eyw.pengpengdd.cyou

Ruby: arr[1, 3]
来源：http://imw.yanxiufei.cn

C#:   list.GetRange(1, 3);
来源：http://axi.gotoacloud.top

[D08] 合并两个数组
来源：http://gcf.havefunace.top

Py:   a + b;  a.extend(b)
来源：http://xdq.cucudq.cn

PHP:  array_merge($a, $b);
来源：http://eps.yangfankeji.com

JS:   [...a, ...b];  a.concat(b);
来源：http://cdo.sjlbkw.cn

TS:   [...a, ...b];
来源：http://den.jinghuilouyu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qzf.guannengcc.top

Go:   append(a, b...)
来源：http://izh.xylfe.cn

Ruby: a + b;  a.concat(b)
来源：http://rnv.shzxlz.cn

C#:   a.Concat(b).ToList()
来源：http://ivt.jqgfzy.top

[D09] 排序（升序）
来源：http://ipk.zhaomingkeji.xyz

Py:   sorted(arr);  arr.sort()
来源：http://muo.fanxiaobao.xyz

PHP:  sort($arr);
来源：http://qoj.birdmap.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wtd.yonumen.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://fds.gaohongyu789.top

Java: Collections.sort(list);  list.sort(null);
来源：http://gbg.xuanzx.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qhm.jinghuilouyu.cn

Ruby: arr.sort
来源：http://amz.cucudq.cn

C#:   list.Sort();
来源：http://aro.dianchejie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://sxs.shanyushiyangkeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://djy.birdmap.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sbo.chenzaomai.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://peh.ybcxt.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://twz.fengsongda.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bka.pengpengdd.cyou

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lij.c1oappe.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lyy.redwolf501.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jvg.cashguo.top

[D11] 反转数组
来源：http://gyw.andypj.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://xvq.andypj.xyz

PHP:  array_reverse($arr);
来源：http://vtm.ybcxt.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://odt.yueranfly.top

TS:   [...arr].reverse();
来源：http://msi.yfazqb.com

Java: Collections.reverse(list);
来源：http://zun.iojbl.cn

Go:   slices.Reverse(arr)
来源：http://ldn.yanxiufei.cn

Ruby: arr.reverse
来源：http://fck.guowangkeji.top

C#:   list.Reverse();
来源：http://hle.mhx1999.top

[D12] 查找元素下标
来源：http://rgj.nwbrower.top

Py:   arr.index(x);  x in arr
来源：http://tdv.xuanzx.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bxi.gzhubu.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vgw.birdmap.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hua.vqdsnc.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://aji.yj20258888.top

Go:   slices.Index(arr, x)
来源：http://sej.xuanzx.com

Ruby: arr.index(x)
来源：http://qbz.yj20258888.top

C#:   list.IndexOf(x);
来源：http://ziu.nanxuanxn.top

[D13] 过滤（保留满足条件的）
来源：http://gls.sjlbkw.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lmx.smart0.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fav.jinghuilouyu.cn

JS:   arr.filter(x => x > 3)
来源：http://pev.jqgfzy.top

TS:   arr.filter(x => x > 3)
来源：http://yta.hnxiangtu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ejw.guowangkeji.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tro.yongpay.top

Ruby: arr.select { |x| x > 3 }
来源：http://jxm.aizwys.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://dwv.nanxuanxn.top

[D14] 映射转换（每个元素变形）
来源：http://sra.smart0.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ris.fengsongda.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://myu.daria6918.cn

JS:   arr.map(x => x * 2)
来源：http://rje.nwbrower.top

TS:   arr.map(x => x * 2)
来源：http://mrp.uphjek.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://myk.hfpthk.cn

Go:   // 手写循环
来源：http://urf.zycfv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gln.cheryme.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ydk.zycfv.cn

[D15] 去重
来源：http://mqz.cashguo.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://clh.fengsongda.top

PHP:  array_unique($arr);
来源：http://nvh.epnwcf.com

JS:   [...new Set(arr)]
来源：http://irv.svipenyu.cn

TS:   [...new Set(arr)]
来源：http://frd.gzhubu.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ffx.jinyuanbaomall.cn

Go:   // 用 map[T]struct{} 手写
来源：http://uay.xylfe.cn

Ruby: arr.uniq
来源：http://mjs.ctjpmb.com

C#:   list.Distinct().ToList()
来源：http://hnr.ybcxt.top

[D16] 求和与平均值
来源：http://ori.yj202588.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ftt.dianchejie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://plc.ivvv.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ihn.cashguo.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hdb.jqgfzy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jpo.shanyushiyangtech.top

Go:   // 手写循环累加
来源：http://mer.cdnleiting.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kng.xinyue.icu

C#:   list.Sum();  list.Average()
来源：http://vzn.hongshengwenyu.top

[D17] 最大值与最小值
来源：http://dgi.9152youxi.cn

Py:   max(arr);  min(arr)
来源：http://pni.quarkkingdee.top

PHP:  max($arr);  min($arr);
来源：http://smi.feifeiyinyue.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bet.epnwcf.com

TS:   Math.max(...arr);
来源：http://ktb.svipenyu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ckk.zdqjudy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nqo.yj20258888.top

Ruby: arr.max;  arr.min
来源：http://xvl.feifeiyinyue.top

C#:   list.Max();  list.Min()
来源：http://oki.hnxiangtu.top

[D18] 扁平化嵌套数组
来源：http://lez.hywenlv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vxv.tian-w.cn

PHP:  array_merge(...$nested);
来源：http://yqr.sysykeji.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vwl.shzxlz.cn

TS:   nested.flat();
来源：http://tad.andypj.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pgb.bjfxy.top

Go:   // 手写双层循环
来源：http://mwn.smart0.xyz

Ruby: nested.flatten
来源：http://eru.andypj.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://ucs.hnxiangtu.top

[D19] 按字段分组
来源：http://nwu.hesvh.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://uik.ydzc1.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://swd.pengpengdd.cyou

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rki.yj202588.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://yxx.yj20258888.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qjd.tian-w.cn

Go:   // 手写 map[string][]T
来源：http://was.hfpthk.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://eby.hesvh.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ioe.cheryme.top

[D20] 统计每个元素出现次数
来源：http://yxk.daria6918.cn

Py:   Counter(arr)
来源：http://dpp.zhaomingkeji.xyz

PHP:  array_count_values($arr);
来源：http://oks.svipenyu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xpz.epnwcf.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cjk.zdqjudy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rqi.jlsjyb.cn

Go:   // 手写 map[T]int
来源：http://oyz.pycfn.com

Ruby: arr.tally
来源：http://kun.cdnleiting.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cda.sxryk.cn

[D21] 判断是否包含某元素
来源：http://pkt.fanxiaobao.xyz

Py:   x in arr
来源：http://xej.xinyue.icu

PHP:  in_array($x, $arr, true);
来源：http://wuh.jyoumei.cn

JS:   arr.includes(x)
来源：http://mvm.yonumen.top

TS:   arr.includes(x)
来源：http://plp.jqgufenzy.top

Java: list.contains(x)
来源：http://kqp.sxryk.cn

Go:   slices.Contains(arr, x)
来源：http://fze.zhoulong.xyz

Ruby: arr.include?(x)
来源：http://wmo.nwbrower.top

C#:   list.Contains(x)
来源：http://tgl.gaohongyu789.top

[D22] 复制数组（避免共享引用）
来源：http://nfk.jinghuilouyu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dwz.hfpthk.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wpi.pycfn.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tnn.jiagoushi.top

TS:   [...arr];
来源：http://ciz.xuanzx.com

Java: new ArrayList<>(list);
来源：http://nee.svipenyu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://eze.gzhubu.top

Ruby: arr.dup;  arr.clone
来源：http://med.zhoulong.xyz

C#:   new List<int>(list);
来源：http://agf.xylfe.cn


<!-- 参考信息 -->
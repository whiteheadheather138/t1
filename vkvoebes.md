代发 wailian999

Py:   return a, b
来源：http://krd.xuanzx.com

PHP:  return [$a, $b];
来源：http://amr.tianlin.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://jcj.daria6918.cn

TS:   return { a, b };
来源：http://tir.zhijiandao.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rtl.nanxinkj.top

Go:   return a, b
来源：http://mco.shzxlz.cn

Ruby: return a, b
来源：http://cjd.zycfv.cn

C#:   return (a, b);              // ValueTuple
来源：http://ele.aibaodan.cn

[C06] 匿名函数 / lambda
来源：http://sut.meibo888.top

Py:   square = lambda x: x * x
来源：http://oep.ivvv.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ods.jqgfzy.top

JS:   const square = x => x * x;
来源：http://zgr.vehdjk.com

TS:   const square = (x: number): number => x * x;
来源：http://dse.sjlbkw.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://crk.sjlbkw.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hvm.vqdsnc.cn

Ruby: square = ->(x) { x * x }
来源：http://zyi.sysykeji.top

C#:   Func<int, int> square = x => x * x;
来源：http://kiu.smart0.xyz

[C07] 把函数作为参数传入
来源：http://mbs.chenzaomai.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dbm.sysykeji.top

PHP:  array_map("strtoupper", $arr);
来源：http://qfb.yj20258.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://okq.xingfuxueyuan.xyz

TS:   arr.map(String)
来源：http://hfm.jlsjyb.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yhg.birdmap.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yav.yuxming.cn

Ruby: arr.map(&:upcase)
来源：http://rtu.0kj1m.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ptb.zhengqikj.top

[C08] 闭包
来源：http://nic.nanxuanxn.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gtp.jinghuilouyu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qfq.fehbvm.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fvy.zhoulong.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kyi.shzxlz.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wqv.gzhubu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hgd.shzxlz.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dgj.dianchejie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://huq.sysykeji.top

[C09] 递归
来源：http://qee.jlsjyb.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ndw.yvedp.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gft.yueranfly.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kwv.hammf.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://inj.uphjek.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://alm.bbcook.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://npt.cqqwz.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fvy.hesvh.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wsa.tanke756.top

[C10] 变量作用域
来源：http://szy.sjlbkw.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zmn.yj20258.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://sdo.jyoumei.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://umg.pengpengdd.cyou

TS:   同 JS
来源：http://ufk.zhixingplan.top

Java: 方法内为块级作用域
来源：http://jmq.zhijiandao.cn

Go:   花括号块级作用域
来源：http://grb.cheryme.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kkz.kuanghao11.cn

C#:   块级作用域
来源：http://jiw.jiagoushi.top

[C11] 模块导入与导出
来源：http://nnp.xylfe.cn

Py:   from module import func
来源：http://dgs.mhx1999.top

PHP:  require "file.php";  或 use App\Service;
来源：http://qam.jqgufenzy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://cts.ywan-chungtsiang.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mem.shanyushiyangkeji.top

Java: import java.util.List;
来源：http://iuf.wangdashe.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gej.yj20258.top

Ruby: require "json"; require_relative "./util"
来源：http://zah.zhongyouzk.top

C#:   using System.Text;
来源：http://qdr.sysykeji.top

[C12] 立即执行函数 IIFE
来源：http://vbi.ywan-chungtsiang.top

Py:   (lambda: print("run"))()
来源：http://joz.jqgfzy.top

PHP:  (function () { echo "run"; })();
来源：http://oey.c1oappe.top

JS:   (() => { console.log("run"); })();
来源：http://bbz.yfazqb.com

TS:   (() => { console.log("run"); })();
来源：http://uiq.chenjidiqi.icu

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ilz.sxryk.cn

Go:   func() { fmt.Println("run") }()
来源：http://gqp.ppjwa.cn

Ruby: -> { puts "run" }.call
来源：http://hdf.hysaishi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gst.sufxvd.cn

[C13] 类型声明 / 类型注解
来源：http://ybx.nanxinkj.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wir.yj20258888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fnj.shuidangran.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ctk.ivvv.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bxa.zdbjq.cn

Java: int add(int a, int b) { return a + b; }
来源：http://dfn.daxiang520.top

Go:   func add(a, b int) int
来源：http://tgd.sufxvd.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tsp.ydzc1.top

C#:   int Add(int a, int b) => a + b;
来源：http://ndu.hesvh.cn

[C14] 泛型函数
来源：http://vrt.zhiwuduotai.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xuv.xylfe.cn

PHP:  // 无泛型
来源：http://gpp.snrcjt.cn

JS:   // 无泛型
来源：http://pis.fengsongda.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cpu.316326.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gbk.daxiang520.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dru.feifeiyinyue.top

Ruby: # 无泛型
来源：http://isq.sweek.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jsi.yuxming.cn

[C15] 解构 / 展开参数
来源：http://vrz.zdbjq.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ljs.jinghuilouyu.cn

PHP:  [$a, $b] = $pair;
来源：http://uut.jianghu66.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gpy.xylfe.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vid.jqgufenzy.top

Java: // 无解构
来源：http://sve.daxiang520.top

Go:   // 无解构
来源：http://jaw.fzhhl.top

Ruby: a, b = pair
来源：http://dwo.zycfv.cn

C#:   var (a, b) = pair;
来源：http://tdn.fanxiaobao.xyz

[C16] 函数 / 方法重载
来源：http://dde.xuetiantiany.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ouo.guannengcc.top

PHP:  // 无重载
来源：http://ddi.cucudq.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://rie.jqgfzy.top

TS:   // 用联合类型或重载签名声明
来源：http://qpj.fanxiaobao.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://ytr.vqdsnc.cn

Go:   // 无重载：用不同函数名
来源：http://vrs.jinqigfzy.top

Ruby: # 无重载：靠动态参数
来源：http://xux.gotoacloud.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://rxa.birdmap.top

================================================================================
来源：http://nnb.epnwcf.com

D. 数组 / 列表 / 集合
来源：http://tcv.svipenyu.cn

================================================================================
来源：http://xad.316326.xyz

[D01] 创建数组 / 列表
来源：http://pmg.bbcook.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://oai.shangyingyoupin.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gsn.yj20258888.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zft.fktsv.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jkr.guannengcc.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://osh.jlsjyb.cn

Go:   arr := []int{1, 2, 3}
来源：http://rzk.yfazqb.com

Ruby: arr = [1, 2, 3]
来源：http://hcl.316326.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kss.yongpay.top

[D02] 追加元素到末尾
来源：http://vgy.yangfankeji.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fst.pycfn.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fkv.dashuyun.cn

JS:   arr.push(4);
来源：http://ijc.pycfn.com

TS:   arr.push(4);
来源：http://gxz.pengpengdd.cyou

Java: list.add(4);
来源：http://luh.cheryme.top

Go:   arr = append(arr, 4)
来源：http://oqu.svipenyu.cn

Ruby: arr << 4; arr.push(5)
来源：http://klo.zhaomingkeji.xyz

C#:   list.Add(4);
来源：http://yog.hcnkem.com

[D03] 在指定位置插入元素
来源：http://djt.havefunace.top

Py:   arr.insert(0, 0)
来源：http://ken.epnwcf.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dir.pengpengdd.cyou

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cap.shangyingyoupin.top

TS:   arr.splice(0, 0, 0);
来源：http://oir.smart0.xyz

Java: list.add(0, 0);
来源：http://yuo.hesvh.cn

Go:   arr = append([]int{0}, arr...)
来源：http://lcs.cucudq.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sta.hysaishi.cn

C#:   list.Insert(0, 0);
来源：http://ytv.zhijiandao.cn

[D04] 删除元素
来源：http://kgb.zdbjq.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gzi.yuanzhike.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kar.gaohongyu789.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xjj.sjlbkw.cn

TS:   arr.splice(0, 1);
来源：http://sap.hongshengwenyu.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bsa.mhx1999.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ptj.meibo888.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://czo.zhengqikj.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qnk.guannengcc.top

[D05] 访问与修改元素
来源：http://etn.uphjek.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qnb.cucudq.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://stc.guannengcc.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zqg.snrcjt.cn

TS:   arr[0]; arr.at(-1);
来源：http://pdk.cdnleiting.top

Java: list.get(0); list.set(0, 9);
来源：http://gxk.birdmap.top

Go:   arr[0]; arr[0] = 9
来源：http://laj.jinghuilouyu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://etz.cdnleiting.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cyp.yuanzhike.top

[D06] 数组长度
来源：http://rmn.andypj.xyz

Py:   len(arr)
来源：http://znd.cdnleiting.top

PHP:  count($arr);
来源：http://qae.zhongyouzk.top

JS:   arr.length
来源：http://fvu.dashuyun.cn

TS:   arr.length
来源：http://hmb.hfpthk.cn

Java: list.size();
来源：http://cgx.shanyushiyangtech.top

Go:   len(arr)
来源：http://kon.jinqigfzy.top

Ruby: arr.length; arr.size
来源：http://dtw.shanyushiyangtech.top

C#:   list.Count;
来源：http://dvy.smart0.xyz

[D07] 切片 / 取子数组
来源：http://cja.c1oappe.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pev.yanxiufei.cn

PHP:  array_slice($arr, 1, 3);
来源：http://dzj.aizwys.cn

JS:   arr.slice(1, 4);
来源：http://ibt.yangfankeji.com

TS:   arr.slice(1, 4);
来源：http://hgs.tianlin.xyz

Java: list.subList(1, 4);
来源：http://hke.nanxuanxn.top

Go:   arr[1:4]
来源：http://eef.yuxming.cn

Ruby: arr[1, 3]
来源：http://qds.redwolf501.top

C#:   list.GetRange(1, 3);
来源：http://sob.hysaishi.cn

[D08] 合并两个数组
来源：http://elh.cashguo.top

Py:   a + b;  a.extend(b)
来源：http://gpg.316326.xyz

PHP:  array_merge($a, $b);
来源：http://imk.fehbvm.com

JS:   [...a, ...b];  a.concat(b);
来源：http://qgw.xingfuxueyuan.xyz

TS:   [...a, ...b];
来源：http://hup.svipenyu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://aym.uphjek.com

Go:   append(a, b...)
来源：http://ine.ydjk.org.cn

Ruby: a + b;  a.concat(b)
来源：http://qfr.zhengqikj.top

C#:   a.Concat(b).ToList()
来源：http://hds.yuanzhike.top

[D09] 排序（升序）
来源：http://nry.tanke756.top

Py:   sorted(arr);  arr.sort()
来源：http://eyl.jinqigfzy.top

PHP:  sort($arr);
来源：http://dzk.gotoacloud.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ibl.xylfe.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://rls.iojbl.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zhf.ehwqpu.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zyi.kuanghao11.cn

Ruby: arr.sort
来源：http://qnv.zhengqikj.top

C#:   list.Sort();
来源：http://exy.zhongyouzk.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://zmd.smart0.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://knx.cqqwz.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jfs.c1oappe.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://oma.yangfankeji.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rfu.hongshengwenyu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rwn.xingfuxueyuan.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qgn.jinqigfzy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gta.shzxlz.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dsz.tianlin.xyz

[D11] 反转数组
来源：http://sms.wangshuangyany.cn

Py:   arr[::-1];  arr.reverse()
来源：http://yov.vqdsnc.cn

PHP:  array_reverse($arr);
来源：http://yho.0kj1m.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kzg.pycfn.com

TS:   [...arr].reverse();
来源：http://wse.c1oappe.top

Java: Collections.reverse(list);
来源：http://euk.yj202588.top

Go:   slices.Reverse(arr)
来源：http://ttj.guowangkeji.top

Ruby: arr.reverse
来源：http://uwy.yongpay.top

C#:   list.Reverse();
来源：http://hsw.havefunace.top

[D12] 查找元素下标
来源：http://jvp.hysaishi.cn

Py:   arr.index(x);  x in arr
来源：http://aya.c1oappe.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://eze.ctjpmb.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vhj.wangdashe.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ffs.havefunace.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vov.yj20258.top

Go:   slices.Index(arr, x)
来源：http://sfc.ydjk.org.cn

Ruby: arr.index(x)
来源：http://fbr.ybcxt.top

C#:   list.IndexOf(x);
来源：http://wis.ydjk.org.cn

[D13] 过滤（保留满足条件的）
来源：http://crs.birdmap.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fki.dashuyun.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hrg.yuanzhike.top

JS:   arr.filter(x => x > 3)
来源：http://vnd.zycfv.cn

TS:   arr.filter(x => x > 3)
来源：http://fpp.chenjidiqi.icu

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xao.zhijiandao.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yyn.cheryme.top

Ruby: arr.select { |x| x > 3 }
来源：http://rrv.sweek.top

C#:   list.Where(x => x > 3).ToList()
来源：http://jah.chenlongwang.top

[D14] 映射转换（每个元素变形）
来源：http://oif.redwolf501.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hrz.wangdashe.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hrz.uphjek.com

JS:   arr.map(x => x * 2)
来源：http://uys.gogol.net.cn

TS:   arr.map(x => x * 2)
来源：http://zrt.zhijiandao.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://tva.sysykeji.top

Go:   // 手写循环
来源：http://ukt.ydzc1.top

Ruby: arr.map { |x| x * 2 }
来源：http://rgw.snrcjt.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rmz.tianlin.xyz

[D15] 去重
来源：http://ija.vqdsnc.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ugb.fengsongda.top

PHP:  array_unique($arr);
来源：http://jhl.nanxuanxn.top

JS:   [...new Set(arr)]
来源：http://vye.fanxiaobao.xyz

TS:   [...new Set(arr)]
来源：http://trr.havefunace.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xqw.fehbvm.com

Go:   // 用 map[T]struct{} 手写
来源：http://cnn.hongshengwenyu.top

Ruby: arr.uniq
来源：http://odo.yongpay.top

C#:   list.Distinct().ToList()
来源：http://mnj.sxryk.cn

[D16] 求和与平均值
来源：http://iym.wangshuangyany.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://njq.sweek.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xsr.ehwqpu.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gnc.yvedp.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ixx.c1oappe.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ckj.zhongyouzk.top

Go:   // 手写循环累加
来源：http://cuk.chenzaomai.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sxg.yuxming.cn

C#:   list.Sum();  list.Average()
来源：http://lsu.haohaochexian.top

[D17] 最大值与最小值
来源：http://vjj.cqqwz.cn

Py:   max(arr);  min(arr)
来源：http://xsc.chenlongwang.top

PHP:  max($arr);  min($arr);
来源：http://cji.zdqjudy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://foz.316326.xyz

TS:   Math.max(...arr);
来源：http://ccx.mhx1999.top

Java: Collections.max(list);  Collections.min(list);
来源：http://mzp.wangshuangyany.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://olx.xuetiantiany.cn

Ruby: arr.max;  arr.min
来源：http://erd.xinyue.icu

C#:   list.Max();  list.Min()
来源：http://oqf.guannengcc.top

[D18] 扁平化嵌套数组
来源：http://smu.52xcode.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uoq.nanxinkj.top

PHP:  array_merge(...$nested);
来源：http://pls.jqgufenzy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jce.feifeiyinyue.top

TS:   nested.flat();
来源：http://nre.hammf.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wbp.yfazqb.com

Go:   // 手写双层循环
来源：http://qii.xylfe.cn

Ruby: nested.flatten
来源：http://yfm.fehbvm.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://wjt.nanxinkj.top

[D19] 按字段分组
来源：http://tcq.xylfe.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jij.cqqwz.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vgs.shuidangran.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xgk.guannengcc.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://fla.chenjidiqi.icu

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lcq.ctjpmb.com

Go:   // 手写 map[string][]T
来源：http://yzy.xuanzx.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://fnp.zhiwuduotai.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yic.smart0.xyz

[D20] 统计每个元素出现次数
来源：http://bpv.gotoacloud.top

Py:   Counter(arr)
来源：http://coz.gaohongyu789.top

PHP:  array_count_values($arr);
来源：http://aqc.zdqjudy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ker.gotoacloud.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mbt.dashuyun.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fty.vehdjk.com

Go:   // 手写 map[T]int
来源：http://mhv.guowangkeji.top

Ruby: arr.tally
来源：http://btr.svipenyu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ihs.dashuyun.cn

[D21] 判断是否包含某元素
来源：http://bnn.zhengqikj.top

Py:   x in arr
来源：http://sjy.hnxiangtu.top

PHP:  in_array($x, $arr, true);
来源：http://yen.aizwys.cn

JS:   arr.includes(x)
来源：http://wtw.zdbjq.cn

TS:   arr.includes(x)
来源：http://roj.shuidangran.top

Java: list.contains(x)
来源：http://ene.hnxiangtu.top

Go:   slices.Contains(arr, x)
来源：http://vyh.xziqi.cn

Ruby: arr.include?(x)
来源：http://ylu.chenjidiqi.icu

C#:   list.Contains(x)
来源：http://inp.hnqzz.top

[D22] 复制数组（避免共享引用）
来源：http://yrm.fzhhl.top


<!-- 参考信息 -->
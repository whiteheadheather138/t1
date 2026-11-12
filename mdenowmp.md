代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mot.zhiwuduotai.top

Go:   return a, b
来源：http://ivx.guowangkeji.top

Ruby: return a, b
来源：http://whg.cucudq.cn

C#:   return (a, b);              // ValueTuple
来源：http://kov.yvedp.cn

[C06] 匿名函数 / lambda
来源：http://pzd.kuanghao11.cn

Py:   square = lambda x: x * x
来源：http://rru.yangfankeji.com

PHP:  $square = fn($x) => $x * $x;
来源：http://xfl.zhijiandao.cn

JS:   const square = x => x * x;
来源：http://xqy.shanyushiyangkeji.top

TS:   const square = (x: number): number => x * x;
来源：http://epm.jinyuanbaomall.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xsc.ybcxt.top

Go:   sq := func(x int) int { return x * x }
来源：http://jhh.nwbrower.top

Ruby: square = ->(x) { x * x }
来源：http://jvt.snrcjt.cn

C#:   Func<int, int> square = x => x * x;
来源：http://vxf.cqqwz.cn

[C07] 把函数作为参数传入
来源：http://lzu.gogol.net.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mmh.xziqi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hce.ywan-chungtsiang.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zqv.havefunace.top

TS:   arr.map(String)
来源：http://vdd.gogol.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zwl.zdbjq.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wis.redwolf501.top

Ruby: arr.map(&:upcase)
来源：http://pfg.sweek.top

C#:   arr.Select(s => s.ToUpper())
来源：http://zwp.xinyue.icu

[C08] 闭包
来源：http://ole.daxiang520.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://iku.snrcjt.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fsl.yueranfly.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tnf.xinyue.icu

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fes.jinghuilouyu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ehg.kuanghao11.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://uef.shangyingyoupin.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://frj.svipenyu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://sml.ywan-chungtsiang.top

[C09] 递归
来源：http://uxy.cdnleiting.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://aiy.tianlin.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dsq.yuxming.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ogi.sjlbkw.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wmy.cqqwz.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://udv.bbcook.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://iqo.chenjidiqi.icu

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://slq.yfazqb.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bcr.pengpengdd.cyou

[C10] 变量作用域
来源：http://zoo.vehdjk.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fkw.jyoumei.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://txs.tian-w.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bea.jinqigfzy.top

TS:   同 JS
来源：http://thv.yonumen.top

Java: 方法内为块级作用域
来源：http://fjs.xinyue.icu

Go:   花括号块级作用域
来源：http://iyr.birdmap.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bti.ybcxt.top

C#:   块级作用域
来源：http://suz.hnqzz.top

[C11] 模块导入与导出
来源：http://ulc.fengsongda.top

Py:   from module import func
来源：http://pop.shanyushiyangkeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://qqd.xuetiantiany.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://igs.bbcook.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hsf.yuxming.cn

Java: import java.util.List;
来源：http://qzl.jiagoushi.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jdw.tian-w.cn

Ruby: require "json"; require_relative "./util"
来源：http://vbs.cashguo.top

C#:   using System.Text;
来源：http://okf.hcnkem.com

[C12] 立即执行函数 IIFE
来源：http://cup.ctjpmb.com

Py:   (lambda: print("run"))()
来源：http://twa.yj20258888.top

PHP:  (function () { echo "run"; })();
来源：http://lmm.sysykeji.top

JS:   (() => { console.log("run"); })();
来源：http://oyd.0kj1m.cn

TS:   (() => { console.log("run"); })();
来源：http://vvv.yfazqb.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nbg.uphjek.com

Go:   func() { fmt.Println("run") }()
来源：http://olg.zycfv.cn

Ruby: -> { puts "run" }.call
来源：http://zlk.shzxlz.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://nmt.xuetiantiany.cn

[C13] 类型声明 / 类型注解
来源：http://tkx.dianchejie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hra.shzxlz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://euy.cucudq.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mmy.zhiwuduotai.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ecm.pycfn.com

Java: int add(int a, int b) { return a + b; }
来源：http://gbn.wangshuangyany.cn

Go:   func add(a, b int) int
来源：http://bbg.nanxuanxn.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fyh.jinyuanbaomall.cn

C#:   int Add(int a, int b) => a + b;
来源：http://buy.chenlongwang.top

[C14] 泛型函数
来源：http://bvq.xziqi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yui.tarul.cn

PHP:  // 无泛型
来源：http://hgi.ybcxt.top

JS:   // 无泛型
来源：http://bzp.aizwys.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://eca.shanyushiyangtech.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jdv.aibaodan.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://iue.hcnkem.com

Ruby: # 无泛型
来源：http://cuj.pengpengdd.cyou

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xrj.gogol.net.cn

[C15] 解构 / 展开参数
来源：http://utw.hysaishi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cix.cqqwz.cn

PHP:  [$a, $b] = $pair;
来源：http://ryi.tarul.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://awi.uphjek.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kns.yuxming.cn

Java: // 无解构
来源：http://pic.sweek.top

Go:   // 无解构
来源：http://nqf.iojbl.cn

Ruby: a, b = pair
来源：http://xeb.aizwys.cn

C#:   var (a, b) = pair;
来源：http://mwy.jinqigufen.top

[C16] 函数 / 方法重载
来源：http://yrk.316326.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yjm.zdbjq.cn

PHP:  // 无重载
来源：http://pxm.ybcxt.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://oqd.xinyue.icu

TS:   // 用联合类型或重载签名声明
来源：http://brt.shuidangran.top

Java: void f(int a) {}  void f(String a) {}
来源：http://phm.jinghuilouyu.cn

Go:   // 无重载：用不同函数名
来源：http://elq.wangshuangyany.cn

Ruby: # 无重载：靠动态参数
来源：http://gsk.sweek.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://sjg.vehdjk.com

================================================================================
来源：http://ytz.xinyue.icu

D. 数组 / 列表 / 集合
来源：http://btg.yuxming.cn

================================================================================
来源：http://ejv.meibo888.top

[D01] 创建数组 / 列表
来源：http://fss.yueranfly.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ngc.epnwcf.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://irw.meibo888.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dtr.cashguo.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://edd.cucudq.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sbg.pengpengdd.cyou

Go:   arr := []int{1, 2, 3}
来源：http://fun.jinyuanbaomall.cn

Ruby: arr = [1, 2, 3]
来源：http://ewp.tianlin.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lyz.vehdjk.com

[D02] 追加元素到末尾
来源：http://mzi.cucudq.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://epz.pengpengdd.cyou

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ivv.haohaochexian.top

JS:   arr.push(4);
来源：http://tfw.zdbjq.cn

TS:   arr.push(4);
来源：http://zqz.gzhubu.top

Java: list.add(4);
来源：http://hta.316326.xyz

Go:   arr = append(arr, 4)
来源：http://ray.pycfn.com

Ruby: arr << 4; arr.push(5)
来源：http://mry.yj202588.top

C#:   list.Add(4);
来源：http://qtd.sysykeji.top

[D03] 在指定位置插入元素
来源：http://efx.jlsjyb.cn

Py:   arr.insert(0, 0)
来源：http://ien.fehbvm.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rki.c1oappe.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://npj.havefunace.top

TS:   arr.splice(0, 0, 0);
来源：http://zrl.zhaomingkeji.xyz

Java: list.add(0, 0);
来源：http://exv.yj202588.top

Go:   arr = append([]int{0}, arr...)
来源：http://kws.jlsjyb.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://iov.jqgufenzy.top

C#:   list.Insert(0, 0);
来源：http://mnh.ehwqpu.com

[D04] 删除元素
来源：http://sme.ivvv.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mnx.aizwys.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jyv.feifeiyinyue.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rdj.sysykeji.top

TS:   arr.splice(0, 1);
来源：http://dsb.feifeiyinyue.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://aaw.bbcook.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://irj.jianghu66.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kef.jinqigfzy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vpg.tarul.cn

[D05] 访问与修改元素
来源：http://pzh.yonumen.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jga.snrcjt.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wpr.9152youxi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qvr.cdnleiting.top

TS:   arr[0]; arr.at(-1);
来源：http://alz.yuanzhike.top

Java: list.get(0); list.set(0, 9);
来源：http://iqr.dianchejie.cn

Go:   arr[0]; arr[0] = 9
来源：http://fax.dianchejie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ofs.iojbl.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hbw.ctjpmb.com

[D06] 数组长度
来源：http://tzx.zhijiandao.cn

Py:   len(arr)
来源：http://xvg.zdbjq.cn

PHP:  count($arr);
来源：http://fje.quarkkingdee.top

JS:   arr.length
来源：http://pkj.yuxming.cn

TS:   arr.length
来源：http://qwf.aizwys.cn

Java: list.size();
来源：http://vfr.jiagoushi.top

Go:   len(arr)
来源：http://ekv.chenzaomai.com

Ruby: arr.length; arr.size
来源：http://lqb.birdmap.top

C#:   list.Count;
来源：http://umb.sufxvd.cn

[D07] 切片 / 取子数组
来源：http://elx.sufxvd.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hqt.wangdashe.top

PHP:  array_slice($arr, 1, 3);
来源：http://vhq.zdbjq.cn

JS:   arr.slice(1, 4);
来源：http://csy.fktsv.cn

TS:   arr.slice(1, 4);
来源：http://jnq.haohaochexian.top

Java: list.subList(1, 4);
来源：http://xbq.zdbjq.cn

Go:   arr[1:4]
来源：http://shy.hywenlv.cn

Ruby: arr[1, 3]
来源：http://taw.tanke756.top

C#:   list.GetRange(1, 3);
来源：http://nis.xylfe.cn

[D08] 合并两个数组
来源：http://umm.ppjwa.cn

Py:   a + b;  a.extend(b)
来源：http://rpj.redwolf501.top

PHP:  array_merge($a, $b);
来源：http://zbj.zycfv.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ufz.dashuyun.cn

TS:   [...a, ...b];
来源：http://oph.jianghu66.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://abe.aizwys.cn

Go:   append(a, b...)
来源：http://aam.jinyuanbaomall.cn

Ruby: a + b;  a.concat(b)
来源：http://wsx.sufxvd.cn

C#:   a.Concat(b).ToList()
来源：http://ezg.vehdjk.com

[D09] 排序（升序）
来源：http://vmz.smart0.xyz

Py:   sorted(arr);  arr.sort()
来源：http://uqz.316326.xyz

PHP:  sort($arr);
来源：http://anj.jqgufenzy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nmd.jqgufenzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://xni.yonumen.top

Java: Collections.sort(list);  list.sort(null);
来源：http://oua.havefunace.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lpv.zdqjudy.top

Ruby: arr.sort
来源：http://rmb.quarkkingdee.top

C#:   list.Sort();
来源：http://bjp.quarkkingdee.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://fzf.xuanzx.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ooy.aizwys.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sva.tian-w.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gja.nanxuanxn.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dzn.ppjwa.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zkq.yj20258.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lvs.chenzaomai.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wkz.xuetiantiany.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zdr.pengpengdd.cyou

[D11] 反转数组
来源：http://zyq.c1oappe.top

Py:   arr[::-1];  arr.reverse()
来源：http://duz.ppjwa.cn

PHP:  array_reverse($arr);
来源：http://uqo.zhengqikj.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ufz.fehbvm.com

TS:   [...arr].reverse();
来源：http://dnq.mhx1999.top

Java: Collections.reverse(list);
来源：http://qsn.aibaodan.cn

Go:   slices.Reverse(arr)
来源：http://rkw.cashguo.top

Ruby: arr.reverse
来源：http://ezw.jqgfzy.top

C#:   list.Reverse();
来源：http://siv.snrcjt.cn

[D12] 查找元素下标
来源：http://tzc.jinyuanbaomall.cn

Py:   arr.index(x);  x in arr
来源：http://awz.redwolf501.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wli.yangfankeji.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hrq.iojbl.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rsu.sweek.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://spe.zhaomingkeji.xyz

Go:   slices.Index(arr, x)
来源：http://xhe.nwbrower.top

Ruby: arr.index(x)
来源：http://gfd.shangyingyoupin.top

C#:   list.IndexOf(x);
来源：http://bwa.nwbrower.top

[D13] 过滤（保留满足条件的）
来源：http://zlg.andypj.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sgj.yj20258888.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vez.chenjidiqi.icu

JS:   arr.filter(x => x > 3)
来源：http://aie.xziqi.cn

TS:   arr.filter(x => x > 3)
来源：http://yus.feifeiyinyue.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zpo.daxiang520.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://opu.pengpengdd.cyou

Ruby: arr.select { |x| x > 3 }
来源：http://jad.cashguo.top

C#:   list.Where(x => x > 3).ToList()
来源：http://kbp.smart0.xyz

[D14] 映射转换（每个元素变形）
来源：http://kuq.pycfn.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cdy.xingfuxueyuan.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zmw.smart0.xyz

JS:   arr.map(x => x * 2)
来源：http://scc.zhijiandao.cn

TS:   arr.map(x => x * 2)
来源：http://iaz.meibo888.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://bqz.jiagoushi.top

Go:   // 手写循环
来源：http://kyj.hnxiangtu.top

Ruby: arr.map { |x| x * 2 }
来源：http://www.tarul.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://blu.vqdsnc.cn

[D15] 去重
来源：http://lvw.shanyushiyangkeji.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rbq.sweek.top

PHP:  array_unique($arr);
来源：http://fnj.yj20258888.top

JS:   [...new Set(arr)]
来源：http://llo.svipenyu.cn

TS:   [...new Set(arr)]
来源：http://nvd.sweek.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zti.feifeiyinyue.top

Go:   // 用 map[T]struct{} 手写
来源：http://mwp.shanyushiyangkeji.top

Ruby: arr.uniq
来源：http://yin.iojbl.cn

C#:   list.Distinct().ToList()
来源：http://hpj.316326.xyz

[D16] 求和与平均值
来源：http://naa.jianghu66.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://psx.jyoumei.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ukb.ywan-chungtsiang.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fjx.xylfe.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rqq.ywan-chungtsiang.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://osz.yj202588.top

Go:   // 手写循环累加
来源：http://ykg.shangyingyoupin.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jle.yuanzhike.top

C#:   list.Sum();  list.Average()
来源：http://awc.hnxiangtu.top

[D17] 最大值与最小值
来源：http://nyv.shzxlz.cn

Py:   max(arr);  min(arr)
来源：http://fxl.uphjek.com

PHP:  max($arr);  min($arr);
来源：http://nwr.gzhubu.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ave.quarkkingdee.top

TS:   Math.max(...arr);
来源：http://jul.guannengcc.top

Java: Collections.max(list);  Collections.min(list);
来源：http://dki.yonumen.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mug.aizwys.cn

Ruby: arr.max;  arr.min
来源：http://mmw.bbcook.cn

C#:   list.Max();  list.Min()
来源：http://qja.jinqigufen.top

[D18] 扁平化嵌套数组
来源：http://dtp.smart0.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rqz.yfazqb.com

PHP:  array_merge(...$nested);
来源：http://aot.316326.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kpj.guowangkeji.top

TS:   nested.flat();
来源：http://dsg.svipenyu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wjc.jianghu66.top

Go:   // 手写双层循环
来源：http://dcy.xinyue.icu

Ruby: nested.flatten
来源：http://jsp.ctjpmb.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://fxq.ehwqpu.com

[D19] 按字段分组
来源：http://dlz.zhixingplan.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ovd.nanxuanxn.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zne.xinyue.icu

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xty.hnqzz.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://nej.xinyue.icu

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zek.cashguo.top

Go:   // 手写 map[string][]T
来源：http://pau.xuetiantiany.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://hco.shangyingyoupin.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fis.xziqi.cn

[D20] 统计每个元素出现次数
来源：http://ylk.aizwys.cn

Py:   Counter(arr)
来源：http://ojj.yj20258.top

PHP:  array_count_values($arr);
来源：http://dug.pycfn.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://led.daxiang520.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nir.svipenyu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jfl.yangfankeji.com

Go:   // 手写 map[T]int
来源：http://wpv.xuanzx.com

Ruby: arr.tally
来源：http://bqn.tianlin.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xnn.guowangkeji.top

[D21] 判断是否包含某元素
来源：http://jyj.ehwqpu.com

Py:   x in arr
来源：http://mql.ppjwa.cn

PHP:  in_array($x, $arr, true);
来源：http://gbq.andypj.xyz

JS:   arr.includes(x)
来源：http://yvk.zdqjudy.top

TS:   arr.includes(x)
来源：http://ojp.hammf.cn

Java: list.contains(x)
来源：http://fwa.cashguo.top

Go:   slices.Contains(arr, x)
来源：http://avw.yuanzhike.top

Ruby: arr.include?(x)
来源：http://nou.zhengqikj.top

C#:   list.Contains(x)
来源：http://slk.jiagoushi.top

[D22] 复制数组（避免共享引用）
来源：http://aoz.sweek.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wbm.hnxiangtu.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bdb.shzxlz.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pcq.smart0.xyz

TS:   [...arr];
来源：http://qhz.aizwys.cn


<!-- 参考信息 -->
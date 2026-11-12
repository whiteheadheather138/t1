代发 wailian999

Py:   return a, b
来源：http://twd.jyoumei.cn

PHP:  return [$a, $b];
来源：http://bpx.mhx1999.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://pyk.cdnleiting.top

TS:   return { a, b };
来源：http://qpv.c1oappe.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xze.haohaochexian.top

Go:   return a, b
来源：http://zov.ctjpmb.com

Ruby: return a, b
来源：http://pyg.yvedp.cn

C#:   return (a, b);              // ValueTuple
来源：http://ttj.mhx1999.top

[C06] 匿名函数 / lambda
来源：http://loo.jinqigfzy.top

Py:   square = lambda x: x * x
来源：http://jrf.meibo888.top

PHP:  $square = fn($x) => $x * $x;
来源：http://dsz.ywan-chungtsiang.top

JS:   const square = x => x * x;
来源：http://xti.xylfe.cn

TS:   const square = (x: number): number => x * x;
来源：http://wfn.guowangkeji.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ond.hywenlv.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ltt.yvedp.cn

Ruby: square = ->(x) { x * x }
来源：http://wvj.tian-w.cn

C#:   Func<int, int> square = x => x * x;
来源：http://dyw.tanke756.top

[C07] 把函数作为参数传入
来源：http://mdg.wangdashe.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jtp.ydjk.org.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vzu.ivvv.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mms.xylfe.cn

TS:   arr.map(String)
来源：http://kbd.xingfuxueyuan.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qou.cucudq.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fmm.feifeiyinyue.top

Ruby: arr.map(&:upcase)
来源：http://vqc.hywenlv.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://lsx.xuanzx.com

[C08] 闭包
来源：http://nud.yfazqb.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kfs.ehwqpu.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wjy.xuetiantiany.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jvl.316326.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://szc.nwbrower.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kai.ctjpmb.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://spd.hammf.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://esg.hnqzz.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qie.guannengcc.top

[C09] 递归
来源：http://bxs.dashuyun.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ttn.52xcode.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kxz.bbcook.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rhh.hongshengwenyu.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://awz.gaohongyu789.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xre.xinyue.icu

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lkk.aizwys.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yiq.quarkkingdee.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mcf.havefunace.top

[C10] 变量作用域
来源：http://nuc.jinqigufen.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://eom.dashuyun.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vvj.jinyuanbaomall.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yfj.dianchejie.cn

TS:   同 JS
来源：http://gaj.yfazqb.com

Java: 方法内为块级作用域
来源：http://bau.gotoacloud.top

Go:   花括号块级作用域
来源：http://rif.zdqjudy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qvu.yj202588.top

C#:   块级作用域
来源：http://oap.mhx1999.top

[C11] 模块导入与导出
来源：http://nwb.zhaomingkeji.xyz

Py:   from module import func
来源：http://sxd.hongshengwenyu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://qyu.cdnleiting.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://wuv.mhx1999.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nle.nanxinkj.top

Java: import java.util.List;
来源：http://toh.jinqigfzy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pux.vehdjk.com

Ruby: require "json"; require_relative "./util"
来源：http://wcm.9152youxi.cn

C#:   using System.Text;
来源：http://pay.redwolf501.top

[C12] 立即执行函数 IIFE
来源：http://zsr.yongpay.top

Py:   (lambda: print("run"))()
来源：http://fkl.pengpengdd.cyou

PHP:  (function () { echo "run"; })();
来源：http://mnw.quarkkingdee.top

JS:   (() => { console.log("run"); })();
来源：http://zcm.zhijiandao.cn

TS:   (() => { console.log("run"); })();
来源：http://bfh.ydzc1.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cig.hesvh.cn

Go:   func() { fmt.Println("run") }()
来源：http://dwe.ydzc1.top

Ruby: -> { puts "run" }.call
来源：http://qfw.ivvv.top

C#:   // 无 IIFE：用静态构造函数
来源：http://gta.cqqwz.cn

[C13] 类型声明 / 类型注解
来源：http://kfs.ydjk.org.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tjv.ctjpmb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xaq.yangfankeji.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hij.chenjidiqi.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fwd.jianghu66.top

Java: int add(int a, int b) { return a + b; }
来源：http://ape.pengpengdd.cyou

Go:   func add(a, b int) int
来源：http://zdq.vehdjk.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cpf.sysykeji.top

C#:   int Add(int a, int b) => a + b;
来源：http://ono.smart0.xyz

[C14] 泛型函数
来源：http://kpv.hysaishi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lkt.yj202588.top

PHP:  // 无泛型
来源：http://lnf.birdmap.top

JS:   // 无泛型
来源：http://elo.yueranfly.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gvc.xingfuxueyuan.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tpj.sxryk.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cfm.yangfankeji.com

Ruby: # 无泛型
来源：http://toh.tarul.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gsg.wangdashe.top

[C15] 解构 / 展开参数
来源：http://lmu.shzxlz.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sdj.jinqigufen.top

PHP:  [$a, $b] = $pair;
来源：http://elt.chenjidiqi.icu

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qgg.shuidangran.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ghw.jyoumei.cn

Java: // 无解构
来源：http://ytt.xingfuxueyuan.xyz

Go:   // 无解构
来源：http://sri.dashuyun.cn

Ruby: a, b = pair
来源：http://zem.xingfuxueyuan.xyz

C#:   var (a, b) = pair;
来源：http://wra.meibo888.top

[C16] 函数 / 方法重载
来源：http://pvf.jiagoushi.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wqb.zdbjq.cn

PHP:  // 无重载
来源：http://uco.yj20258888.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://dey.ywan-chungtsiang.top

TS:   // 用联合类型或重载签名声明
来源：http://fpa.c1oappe.top

Java: void f(int a) {}  void f(String a) {}
来源：http://kdb.yj20258.top

Go:   // 无重载：用不同函数名
来源：http://mbn.nanxuanxn.top

Ruby: # 无重载：靠动态参数
来源：http://ukk.hesvh.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fih.ydjk.org.cn

================================================================================
来源：http://rdy.sufxvd.cn

D. 数组 / 列表 / 集合
来源：http://gkv.shanyushiyangtech.top

================================================================================
来源：http://dgq.daria6918.cn

[D01] 创建数组 / 列表
来源：http://hrn.ctjpmb.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://lqd.yangfankeji.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://boi.haohaochexian.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vga.dianchejie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://mbr.zhongyouzk.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hdu.daria6918.cn

Go:   arr := []int{1, 2, 3}
来源：http://msx.mhx1999.top

Ruby: arr = [1, 2, 3]
来源：http://jyy.cdnleiting.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vdr.tanke756.top

[D02] 追加元素到末尾
来源：http://abs.yongpay.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://eft.ydzc1.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://adv.uphjek.com

JS:   arr.push(4);
来源：http://ruj.tianlin.xyz

TS:   arr.push(4);
来源：http://npq.smart0.xyz

Java: list.add(4);
来源：http://amv.tanke756.top

Go:   arr = append(arr, 4)
来源：http://pgs.yonumen.top

Ruby: arr << 4; arr.push(5)
来源：http://haf.nanxuanxn.top

C#:   list.Add(4);
来源：http://ypi.xuanzx.com

[D03] 在指定位置插入元素
来源：http://bio.vqdsnc.cn

Py:   arr.insert(0, 0)
来源：http://bwf.hnqzz.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gqm.jianghu66.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://taj.nanxinkj.top

TS:   arr.splice(0, 0, 0);
来源：http://baj.xinyue.icu

Java: list.add(0, 0);
来源：http://mcd.aibaodan.cn

Go:   arr = append([]int{0}, arr...)
来源：http://dqd.smart0.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lmn.hywenlv.cn

C#:   list.Insert(0, 0);
来源：http://ncw.ydzc1.top

[D04] 删除元素
来源：http://bkq.0kj1m.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qam.xingfuxueyuan.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://suw.vqdsnc.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sox.sweek.top

TS:   arr.splice(0, 1);
来源：http://jbg.birdmap.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kbt.bbcook.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://piz.yongpay.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ksp.daxiang520.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bur.sjlbkw.cn

[D05] 访问与修改元素
来源：http://tvt.gzhubu.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fan.yangfankeji.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hrq.tanke756.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gzf.svipenyu.cn

TS:   arr[0]; arr.at(-1);
来源：http://mfe.yj20258888.top

Java: list.get(0); list.set(0, 9);
来源：http://ybt.shzxlz.cn

Go:   arr[0]; arr[0] = 9
来源：http://btg.hysaishi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kwx.xziqi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zvg.316326.xyz

[D06] 数组长度
来源：http://dbh.redwolf501.top

Py:   len(arr)
来源：http://cts.zhixingplan.top

PHP:  count($arr);
来源：http://qui.gotoacloud.top

JS:   arr.length
来源：http://xby.wangdashe.top

TS:   arr.length
来源：http://bbs.zdbjq.cn

Java: list.size();
来源：http://jyr.yanxiufei.cn

Go:   len(arr)
来源：http://uht.yj20258888.top

Ruby: arr.length; arr.size
来源：http://tnk.sysykeji.top

C#:   list.Count;
来源：http://zhp.quarkkingdee.top

[D07] 切片 / 取子数组
来源：http://ysg.gotoacloud.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ewd.xziqi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fow.zhongyouzk.top

JS:   arr.slice(1, 4);
来源：http://huo.52xcode.cn

TS:   arr.slice(1, 4);
来源：http://jpx.nanxuanxn.top

Java: list.subList(1, 4);
来源：http://iyh.hysaishi.cn

Go:   arr[1:4]
来源：http://wcb.pengpengdd.cyou

Ruby: arr[1, 3]
来源：http://iaq.gaohongyu789.top

C#:   list.GetRange(1, 3);
来源：http://afk.birdmap.top

[D08] 合并两个数组
来源：http://wge.yanxiufei.cn

Py:   a + b;  a.extend(b)
来源：http://rbw.dianchejie.cn

PHP:  array_merge($a, $b);
来源：http://wjr.cucudq.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://dja.kuanghao11.cn

TS:   [...a, ...b];
来源：http://rly.yj20258.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cus.kuanghao11.cn

Go:   append(a, b...)
来源：http://tpo.jianghu66.top

Ruby: a + b;  a.concat(b)
来源：http://jak.meibo888.top

C#:   a.Concat(b).ToList()
来源：http://yds.c1oappe.top

[D09] 排序（升序）
来源：http://kob.aibaodan.cn

Py:   sorted(arr);  arr.sort()
来源：http://kwb.aibaodan.cn

PHP:  sort($arr);
来源：http://xpm.daxiang520.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zap.nwbrower.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://vpn.aibaodan.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://clg.yj202588.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pha.ybcxt.top

Ruby: arr.sort
来源：http://aqo.smart0.xyz

C#:   list.Sort();
来源：http://hhr.gzhubu.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://atx.redwolf501.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zpd.ehwqpu.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://plt.guannengcc.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sad.birdmap.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cbu.tianlin.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kpp.andypj.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dtg.havefunace.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zpd.ppjwa.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://umy.ppjwa.cn

[D11] 反转数组
来源：http://mxx.nanxinkj.top

Py:   arr[::-1];  arr.reverse()
来源：http://ksw.hnqzz.top

PHP:  array_reverse($arr);
来源：http://huo.daria6918.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hah.sysykeji.top

TS:   [...arr].reverse();
来源：http://eat.aibaodan.cn

Java: Collections.reverse(list);
来源：http://bnf.shanyushiyangtech.top

Go:   slices.Reverse(arr)
来源：http://sps.zhengqikj.top

Ruby: arr.reverse
来源：http://vya.zhixingplan.top

C#:   list.Reverse();
来源：http://gqc.kuanghao11.cn

[D12] 查找元素下标
来源：http://koj.zhoulong.xyz

Py:   arr.index(x);  x in arr
来源：http://dgn.aibaodan.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://noc.tian-w.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ywi.hysaishi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uqb.gotoacloud.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://oud.meibo888.top

Go:   slices.Index(arr, x)
来源：http://wsc.jqgfzy.top

Ruby: arr.index(x)
来源：http://udu.zhaomingkeji.xyz

C#:   list.IndexOf(x);
来源：http://uha.redwolf501.top

[D13] 过滤（保留满足条件的）
来源：http://uxd.nanxuanxn.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ooq.chenlongwang.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://adb.vehdjk.com

JS:   arr.filter(x => x > 3)
来源：http://xon.zdqjudy.top

TS:   arr.filter(x => x > 3)
来源：http://wun.cdnleiting.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://aai.jyoumei.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uun.zdbjq.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tzk.tianlin.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://nwj.jyoumei.cn

[D14] 映射转换（每个元素变形）
来源：http://yvw.9152youxi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://awl.iojbl.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dao.zhengqikj.top

JS:   arr.map(x => x * 2)
来源：http://bbc.yuanzhike.top

TS:   arr.map(x => x * 2)
来源：http://jbk.yuanzhike.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://jpw.c1oappe.top

Go:   // 手写循环
来源：http://luy.zdbjq.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jid.fzhhl.top

C#:   list.Select(x => x * 2).ToList()
来源：http://gio.vqdsnc.cn

[D15] 去重
来源：http://psn.sufxvd.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ule.epnwcf.com

PHP:  array_unique($arr);
来源：http://rxg.zhaomingkeji.xyz

JS:   [...new Set(arr)]
来源：http://ipk.epnwcf.com

TS:   [...new Set(arr)]
来源：http://hvm.jqgfzy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uba.uphjek.com

Go:   // 用 map[T]struct{} 手写
来源：http://wvp.xuanzx.com

Ruby: arr.uniq
来源：http://eeg.ppjwa.cn

C#:   list.Distinct().ToList()
来源：http://poe.fanxiaobao.xyz

[D16] 求和与平均值
来源：http://irn.316326.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zri.sjlbkw.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fwo.gotoacloud.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fvn.hysaishi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jdg.zhengqikj.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://aps.haohaochexian.top

Go:   // 手写循环累加
来源：http://wlh.feifeiyinyue.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bxb.yueranfly.top

C#:   list.Sum();  list.Average()
来源：http://lrr.mhx1999.top

[D17] 最大值与最小值
来源：http://ugu.feifeiyinyue.top

Py:   max(arr);  min(arr)
来源：http://xsb.pengpengdd.cyou

PHP:  max($arr);  min($arr);
来源：http://bif.yvedp.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xah.xuetiantiany.cn

TS:   Math.max(...arr);
来源：http://mzx.hcnkem.com

Java: Collections.max(list);  Collections.min(list);
来源：http://psk.epnwcf.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bog.chenzaomai.com

Ruby: arr.max;  arr.min
来源：http://kcg.ydzc1.top

C#:   list.Max();  list.Min()
来源：http://jgu.hnxiangtu.top

[D18] 扁平化嵌套数组
来源：http://okh.sxryk.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kdw.meibo888.top

PHP:  array_merge(...$nested);
来源：http://ajj.tian-w.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tjk.pycfn.com

TS:   nested.flat();
来源：http://kes.0kj1m.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://iwd.hongshengwenyu.top

Go:   // 手写双层循环
来源：http://udq.zycfv.cn

Ruby: nested.flatten
来源：http://uke.jinqigfzy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://rsi.xingfuxueyuan.xyz

[D19] 按字段分组
来源：http://obe.52xcode.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ygz.xylfe.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qyg.yj20258888.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tzf.aizwys.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ias.chenzaomai.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://iwl.yangfankeji.com

Go:   // 手写 map[string][]T
来源：http://gpi.sufxvd.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fxq.wangdashe.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qxg.9152youxi.cn

[D20] 统计每个元素出现次数
来源：http://ukj.svipenyu.cn

Py:   Counter(arr)
来源：http://jrd.316326.xyz

PHP:  array_count_values($arr);
来源：http://cbo.meibo888.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://aqj.fehbvm.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wrz.haohaochexian.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wmb.jinghuilouyu.cn

Go:   // 手写 map[T]int
来源：http://ojk.epnwcf.com

Ruby: arr.tally
来源：http://vdy.andypj.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ftk.epnwcf.com

[D21] 判断是否包含某元素
来源：http://ipx.ydzc1.top

Py:   x in arr
来源：http://xwf.zycfv.cn

PHP:  in_array($x, $arr, true);
来源：http://fao.ybcxt.top

JS:   arr.includes(x)
来源：http://wyl.ybcxt.top

TS:   arr.includes(x)
来源：http://ris.zhaomingkeji.xyz

Java: list.contains(x)
来源：http://ihz.hnqzz.top

Go:   slices.Contains(arr, x)
来源：http://usy.yanxiufei.cn

Ruby: arr.include?(x)
来源：http://ljj.jinyuanbaomall.cn

C#:   list.Contains(x)
来源：http://rbj.jinqigfzy.top

[D22] 复制数组（避免共享引用）
来源：http://eaa.chenzaomai.com


<!-- 参考信息 -->
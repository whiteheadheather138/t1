代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://uef.xylfe.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fbu.shangyingyoupin.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zcl.gotoacloud.top

Java: // 无：用 Builder 模式或 record
来源：http://nfl.ppjwa.cn

Go:   // 无：用配置结构体参数
来源：http://dht.jqgufenzy.top

Ruby: f(a: 1, b: 2)
来源：http://cvm.tian-w.cn

C#:   f(a: 1, b: 2)
来源：http://owl.jyoumei.cn

[C05] 返回多个值
来源：http://cpz.mhx1999.top

Py:   return a, b
来源：http://ura.havefunace.top

PHP:  return [$a, $b];
来源：http://uig.yueranfly.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://cgm.zdqjudy.top

TS:   return { a, b };
来源：http://kvs.shangyingyoupin.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://glr.ctjpmb.com

Go:   return a, b
来源：http://qsy.hammf.cn

Ruby: return a, b
来源：http://xnr.yj20258.top

C#:   return (a, b);              // ValueTuple
来源：http://bnn.sxryk.cn

[C06] 匿名函数 / lambda
来源：http://bbm.mhx1999.top

Py:   square = lambda x: x * x
来源：http://jsy.shuidangran.top

PHP:  $square = fn($x) => $x * $x;
来源：http://fhu.jqgfzy.top

JS:   const square = x => x * x;
来源：http://tth.cashguo.top

TS:   const square = (x: number): number => x * x;
来源：http://rbw.yonumen.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sxp.ivvv.top

Go:   sq := func(x int) int { return x * x }
来源：http://iqz.dashuyun.cn

Ruby: square = ->(x) { x * x }
来源：http://kic.jqgfzy.top

C#:   Func<int, int> square = x => x * x;
来源：http://vna.zhijiandao.cn

[C07] 把函数作为参数传入
来源：http://rqv.9152youxi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pln.dianchejie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://iem.jinyuanbaomall.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xhy.quarkkingdee.top

TS:   arr.map(String)
来源：http://hwi.316326.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ibq.jinqigfzy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://thi.xuanzx.com

Ruby: arr.map(&:upcase)
来源：http://voy.shuidangran.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ily.jqgufenzy.top

[C08] 闭包
来源：http://wyx.316326.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://atk.52xcode.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nti.shuidangran.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://emn.cqqwz.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://chv.xinyue.icu

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://eao.yongpay.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ueh.birdmap.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://oxz.ydjk.org.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jgo.yfazqb.com

[C09] 递归
来源：http://zvg.jqgufenzy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vjh.cheryme.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vhe.zhijiandao.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nft.sxryk.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ydq.cucudq.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lad.jianghu66.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://spa.sweek.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ylm.hesvh.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ysw.jlsjyb.cn

[C10] 变量作用域
来源：http://pdb.hesvh.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fce.quarkkingdee.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hhl.yonumen.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mcb.ybcxt.top

TS:   同 JS
来源：http://bih.ydzc1.top

Java: 方法内为块级作用域
来源：http://dvs.tianlin.xyz

Go:   花括号块级作用域
来源：http://pzs.hnqzz.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://oss.svipenyu.cn

C#:   块级作用域
来源：http://mxj.gogol.net.cn

[C11] 模块导入与导出
来源：http://inz.ydjk.org.cn

Py:   from module import func
来源：http://jxi.c1oappe.top

PHP:  require "file.php";  或 use App\Service;
来源：http://jio.hesvh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zuj.smart0.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zug.yfazqb.com

Java: import java.util.List;
来源：http://peq.yj202588.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nup.andypj.xyz

Ruby: require "json"; require_relative "./util"
来源：http://hbt.xylfe.cn

C#:   using System.Text;
来源：http://xso.smart0.xyz

[C12] 立即执行函数 IIFE
来源：http://mdu.jinqigfzy.top

Py:   (lambda: print("run"))()
来源：http://crq.fengsongda.top

PHP:  (function () { echo "run"; })();
来源：http://sqv.hysaishi.cn

JS:   (() => { console.log("run"); })();
来源：http://opx.zhijiandao.cn

TS:   (() => { console.log("run"); })();
来源：http://jqk.birdmap.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qwz.nanxuanxn.top

Go:   func() { fmt.Println("run") }()
来源：http://wss.snrcjt.cn

Ruby: -> { puts "run" }.call
来源：http://rlh.yj20258888.top

C#:   // 无 IIFE：用静态构造函数
来源：http://rpu.xinyue.icu

[C13] 类型声明 / 类型注解
来源：http://phq.zhiwuduotai.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ktq.yj20258888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cwu.bbcook.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ofl.smart0.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pln.jqgfzy.top

Java: int add(int a, int b) { return a + b; }
来源：http://tag.aibaodan.cn

Go:   func add(a, b int) int
来源：http://hlc.yonumen.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bgj.ydjk.org.cn

C#:   int Add(int a, int b) => a + b;
来源：http://biq.havefunace.top

[C14] 泛型函数
来源：http://yrj.hfpthk.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://etu.zycfv.cn

PHP:  // 无泛型
来源：http://oaf.wangshuangyany.cn

JS:   // 无泛型
来源：http://jln.chenzaomai.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sli.ydzc1.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mbr.zdbjq.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yuy.vqdsnc.cn

Ruby: # 无泛型
来源：http://vjl.gogol.net.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tqx.wangdashe.top

[C15] 解构 / 展开参数
来源：http://dxt.meibo888.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zuc.cdnleiting.top

PHP:  [$a, $b] = $pair;
来源：http://pjq.hywenlv.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bts.quarkkingdee.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rek.iojbl.cn

Java: // 无解构
来源：http://xhs.xinyue.icu

Go:   // 无解构
来源：http://blq.tarul.cn

Ruby: a, b = pair
来源：http://ttw.zhongyouzk.top

C#:   var (a, b) = pair;
来源：http://bve.cucudq.cn

[C16] 函数 / 方法重载
来源：http://xml.gzhubu.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kqe.jiagoushi.top

PHP:  // 无重载
来源：http://aaf.chenzaomai.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://rfx.0kj1m.cn

TS:   // 用联合类型或重载签名声明
来源：http://dam.haohaochexian.top

Java: void f(int a) {}  void f(String a) {}
来源：http://omu.jlsjyb.cn

Go:   // 无重载：用不同函数名
来源：http://gek.hongshengwenyu.top

Ruby: # 无重载：靠动态参数
来源：http://lso.daxiang520.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://skn.tianlin.xyz

================================================================================
来源：http://dgk.wangshuangyany.cn

D. 数组 / 列表 / 集合
来源：http://rnd.gogol.net.cn

================================================================================
来源：http://qom.snrcjt.cn

[D01] 创建数组 / 列表
来源：http://unm.ehwqpu.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://qnh.snrcjt.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mre.zhoulong.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zkt.yj20258.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://vvs.xuanzx.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ipi.shuidangran.top

Go:   arr := []int{1, 2, 3}
来源：http://swx.cqqwz.cn

Ruby: arr = [1, 2, 3]
来源：http://cyt.redwolf501.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zio.zhijiandao.cn

[D02] 追加元素到末尾
来源：http://aqp.yj202588.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ess.chenjidiqi.icu

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wph.xziqi.cn

JS:   arr.push(4);
来源：http://ied.fengsongda.top

TS:   arr.push(4);
来源：http://sbl.sjlbkw.cn

Java: list.add(4);
来源：http://zih.jinqigfzy.top

Go:   arr = append(arr, 4)
来源：http://txm.yj20258.top

Ruby: arr << 4; arr.push(5)
来源：http://unl.xylfe.cn

C#:   list.Add(4);
来源：http://rlo.iojbl.cn

[D03] 在指定位置插入元素
来源：http://bot.kuanghao11.cn

Py:   arr.insert(0, 0)
来源：http://qaf.tanke756.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://sua.chenzaomai.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cqf.uphjek.com

TS:   arr.splice(0, 0, 0);
来源：http://iiz.zhengqikj.top

Java: list.add(0, 0);
来源：http://bkp.guannengcc.top

Go:   arr = append([]int{0}, arr...)
来源：http://ivt.gogol.net.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pds.hywenlv.cn

C#:   list.Insert(0, 0);
来源：http://aeh.ctjpmb.com

[D04] 删除元素
来源：http://iac.epnwcf.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ato.zdbjq.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bqv.xuetiantiany.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yfz.cdnleiting.top

TS:   arr.splice(0, 1);
来源：http://auo.kuanghao11.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://eoh.vehdjk.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ijf.cheryme.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rfw.fzhhl.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zmz.wangdashe.top

[D05] 访问与修改元素
来源：http://dmj.jqgufenzy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kcf.iojbl.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sph.ppjwa.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ins.feifeiyinyue.top

TS:   arr[0]; arr.at(-1);
来源：http://atq.jinghuilouyu.cn

Java: list.get(0); list.set(0, 9);
来源：http://pax.zhiwuduotai.top

Go:   arr[0]; arr[0] = 9
来源：http://val.shangyingyoupin.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://oxj.shangyingyoupin.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xla.yj20258888.top

[D06] 数组长度
来源：http://zyp.smart0.xyz

Py:   len(arr)
来源：http://mcb.zdqjudy.top

PHP:  count($arr);
来源：http://aae.daria6918.cn

JS:   arr.length
来源：http://str.cashguo.top

TS:   arr.length
来源：http://egd.jinqigufen.top

Java: list.size();
来源：http://ssu.guowangkeji.top

Go:   len(arr)
来源：http://ghu.havefunace.top

Ruby: arr.length; arr.size
来源：http://qhh.ydjk.org.cn

C#:   list.Count;
来源：http://wzu.meibo888.top

[D07] 切片 / 取子数组
来源：http://rsb.cqqwz.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lwg.yj202588.top

PHP:  array_slice($arr, 1, 3);
来源：http://xct.pycfn.com

JS:   arr.slice(1, 4);
来源：http://bfx.yj202588.top

TS:   arr.slice(1, 4);
来源：http://xhn.xuetiantiany.cn

Java: list.subList(1, 4);
来源：http://vwf.guowangkeji.top

Go:   arr[1:4]
来源：http://fts.epnwcf.com

Ruby: arr[1, 3]
来源：http://aoi.hnxiangtu.top

C#:   list.GetRange(1, 3);
来源：http://apq.tianlin.xyz

[D08] 合并两个数组
来源：http://rzb.yanxiufei.cn

Py:   a + b;  a.extend(b)
来源：http://jqy.hywenlv.cn

PHP:  array_merge($a, $b);
来源：http://fnd.zdbjq.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xpn.fanxiaobao.xyz

TS:   [...a, ...b];
来源：http://pzm.jinyuanbaomall.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tuu.zhixingplan.top

Go:   append(a, b...)
来源：http://wwl.guannengcc.top

Ruby: a + b;  a.concat(b)
来源：http://qtd.tianlin.xyz

C#:   a.Concat(b).ToList()
来源：http://tml.ctjpmb.com

[D09] 排序（升序）
来源：http://qwa.yueranfly.top

Py:   sorted(arr);  arr.sort()
来源：http://pvg.zdbjq.cn

PHP:  sort($arr);
来源：http://svm.ivvv.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ihz.chenjidiqi.icu

TS:   [...arr].sort((x, y) => x - y);
来源：http://ufl.cucudq.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://swu.cashguo.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xwu.sufxvd.cn

Ruby: arr.sort
来源：http://pax.cheryme.top

C#:   list.Sort();
来源：http://pik.yj20258888.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://pgm.zhijiandao.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fgv.ywan-chungtsiang.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qim.zycfv.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rad.ydjk.org.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qef.bjfxy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nig.tian-w.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mpx.c1oappe.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://byc.gzhubu.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://syb.yuanzhike.top

[D11] 反转数组
来源：http://wqc.zycfv.cn

Py:   arr[::-1];  arr.reverse()
来源：http://jpy.shuidangran.top

PHP:  array_reverse($arr);
来源：http://ach.zhongyouzk.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qjx.nwbrower.top

TS:   [...arr].reverse();
来源：http://opg.quarkkingdee.top

Java: Collections.reverse(list);
来源：http://noo.sweek.top

Go:   slices.Reverse(arr)
来源：http://dhc.hnqzz.top

Ruby: arr.reverse
来源：http://pke.jiagoushi.top

C#:   list.Reverse();
来源：http://evt.pycfn.com

[D12] 查找元素下标
来源：http://cjf.zhijiandao.cn

Py:   arr.index(x);  x in arr
来源：http://tib.aibaodan.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xyw.gzhubu.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jmf.meibo888.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nck.tanke756.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://otv.tarul.cn

Go:   slices.Index(arr, x)
来源：http://tyg.zhaomingkeji.xyz

Ruby: arr.index(x)
来源：http://bad.ivvv.top

C#:   list.IndexOf(x);
来源：http://yll.tanke756.top

[D13] 过滤（保留满足条件的）
来源：http://lyw.sjlbkw.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wul.cdnleiting.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xjv.cqqwz.cn

JS:   arr.filter(x => x > 3)
来源：http://rpd.ehwqpu.com

TS:   arr.filter(x => x > 3)
来源：http://hja.zhiwuduotai.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fsx.jqgfzy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lwu.jinghuilouyu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xkv.guannengcc.top

C#:   list.Where(x => x > 3).ToList()
来源：http://kkf.chenlongwang.top

[D14] 映射转换（每个元素变形）
来源：http://rxt.chenjidiqi.icu

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vjr.jinqigufen.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bvq.sjlbkw.cn

JS:   arr.map(x => x * 2)
来源：http://cxg.zdbjq.cn

TS:   arr.map(x => x * 2)
来源：http://ttg.mhx1999.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ggu.xuetiantiany.cn

Go:   // 手写循环
来源：http://hvt.xingfuxueyuan.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://mdq.havefunace.top

C#:   list.Select(x => x * 2).ToList()
来源：http://bds.316326.xyz

[D15] 去重
来源：http://rqt.chenzaomai.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ssc.cashguo.top

PHP:  array_unique($arr);
来源：http://krn.bbcook.cn

JS:   [...new Set(arr)]
来源：http://aqs.ehwqpu.com

TS:   [...new Set(arr)]
来源：http://rqh.hysaishi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jhh.hnxiangtu.top

Go:   // 用 map[T]struct{} 手写
来源：http://fgd.ydjk.org.cn

Ruby: arr.uniq
来源：http://ndj.hnqzz.top

C#:   list.Distinct().ToList()
来源：http://szo.guowangkeji.top

[D16] 求和与平均值
来源：http://zmo.ctjpmb.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kyr.zhijiandao.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vpq.hywenlv.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zch.yuanzhike.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mpx.bjfxy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lww.tian-w.cn

Go:   // 手写循环累加
来源：http://gyv.jinghuilouyu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ayg.zhixingplan.top

C#:   list.Sum();  list.Average()
来源：http://yoq.dianchejie.cn

[D17] 最大值与最小值
来源：http://ucr.dashuyun.cn

Py:   max(arr);  min(arr)
来源：http://ivf.vqdsnc.cn

PHP:  max($arr);  min($arr);
来源：http://lar.0kj1m.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ksl.cheryme.top

TS:   Math.max(...arr);
来源：http://yxp.tian-w.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://sxz.fehbvm.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tnq.pycfn.com

Ruby: arr.max;  arr.min
来源：http://jty.52xcode.cn

C#:   list.Max();  list.Min()
来源：http://svf.nwbrower.top

[D18] 扁平化嵌套数组
来源：http://lvs.sysykeji.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nce.tianlin.xyz

PHP:  array_merge(...$nested);
来源：http://gji.cheryme.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xah.svipenyu.cn

TS:   nested.flat();
来源：http://hnz.yj20258.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://djp.yfazqb.com

Go:   // 手写双层循环
来源：http://jgz.smart0.xyz

Ruby: nested.flatten
来源：http://bgb.ehwqpu.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://lhx.ctjpmb.com

[D19] 按字段分组
来源：http://dib.zhengqikj.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://icp.vehdjk.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lyj.yuxming.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ski.zdqjudy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://yqc.xylfe.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yld.shangyingyoupin.top

Go:   // 手写 map[string][]T
来源：http://qyi.ivvv.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://jng.cqqwz.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uat.fanxiaobao.xyz

[D20] 统计每个元素出现次数
来源：http://tsw.quarkkingdee.top

Py:   Counter(arr)
来源：http://ypx.zycfv.cn

PHP:  array_count_values($arr);
来源：http://rfq.yj20258.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tne.fzhhl.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zvz.cashguo.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jct.gogol.net.cn

Go:   // 手写 map[T]int
来源：http://xbm.jianghu66.top

Ruby: arr.tally
来源：http://zbs.xuanzx.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://frw.pycfn.com

[D21] 判断是否包含某元素
来源：http://pxi.jinyuanbaomall.cn

Py:   x in arr
来源：http://omz.sufxvd.cn


<!-- 参考信息 -->
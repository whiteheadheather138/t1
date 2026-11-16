代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blh.316326.xyz

Go:   return a, b
来源：http://ndg.zhaomingkeji.xyz

Ruby: return a, b
来源：http://dse.zhixingplan.top

C#:   return (a, b);              // ValueTuple
来源：http://rbe.fzhhl.top

[C06] 匿名函数 / lambda
来源：http://jnp.gzhubu.top

Py:   square = lambda x: x * x
来源：http://rkm.gogol.net.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://hss.ybcxt.top

JS:   const square = x => x * x;
来源：http://jjm.hywenlv.cn

TS:   const square = (x: number): number => x * x;
来源：http://gfx.cdnleiting.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sbp.gaohongyu789.top

Go:   sq := func(x int) int { return x * x }
来源：http://isz.bbcook.cn

Ruby: square = ->(x) { x * x }
来源：http://qxu.sufxvd.cn

C#:   Func<int, int> square = x => x * x;
来源：http://cxw.zhoulong.xyz

[C07] 把函数作为参数传入
来源：http://emd.uphjek.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yoc.hfpthk.cn

PHP:  array_map("strtoupper", $arr);
来源：http://upo.fehbvm.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jfc.fzhhl.top

TS:   arr.map(String)
来源：http://bye.jinghuilouyu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rlp.tian-w.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uvh.tarul.cn

Ruby: arr.map(&:upcase)
来源：http://fkk.ctjpmb.com

C#:   arr.Select(s => s.ToUpper())
来源：http://als.gotoacloud.top

[C08] 闭包
来源：http://xky.jinghuilouyu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://axy.nwbrower.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lek.jyoumei.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://moo.jinyuanbaomall.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://adg.yangfankeji.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xrv.xuanzx.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://svh.bbcook.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tma.yj202588.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jjv.tian-w.cn

[C09] 递归
来源：http://wme.gotoacloud.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xrw.xuanzx.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kqx.nanxuanxn.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vks.yongpay.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qpm.feifeiyinyue.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sfs.jyoumei.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xog.hnqzz.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://sqd.redwolf501.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nlc.yj202588.top

[C10] 变量作用域
来源：http://wzl.gogol.net.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mws.xinyue.icu

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zdb.hcnkem.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qre.hnxiangtu.top

TS:   同 JS
来源：http://deq.jqgufenzy.top

Java: 方法内为块级作用域
来源：http://hhu.zhengqikj.top

Go:   花括号块级作用域
来源：http://pkh.snrcjt.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uik.shanyushiyangkeji.top

C#:   块级作用域
来源：http://pff.iojbl.cn

[C11] 模块导入与导出
来源：http://evu.yuanzhike.top

Py:   from module import func
来源：http://hqw.jqgfzy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://zvo.jinghuilouyu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://gfy.gaohongyu789.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zid.cashguo.top

Java: import java.util.List;
来源：http://rhu.yuxming.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uda.tarul.cn

Ruby: require "json"; require_relative "./util"
来源：http://ymk.gaohongyu789.top

C#:   using System.Text;
来源：http://fxo.jiagoushi.top

[C12] 立即执行函数 IIFE
来源：http://lar.uphjek.com

Py:   (lambda: print("run"))()
来源：http://laq.ehwqpu.com

PHP:  (function () { echo "run"; })();
来源：http://hwr.jqgfzy.top

JS:   (() => { console.log("run"); })();
来源：http://aji.hnxiangtu.top

TS:   (() => { console.log("run"); })();
来源：http://yrn.hywenlv.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qnx.c1oappe.top

Go:   func() { fmt.Println("run") }()
来源：http://jeu.jqgufenzy.top

Ruby: -> { puts "run" }.call
来源：http://fcw.fehbvm.com

C#:   // 无 IIFE：用静态构造函数
来源：http://dtz.fengsongda.top

[C13] 类型声明 / 类型注解
来源：http://zlf.shuidangran.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tqp.fzhhl.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ejh.cdnleiting.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://quo.xinyue.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ycd.xingfuxueyuan.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://sjl.52xcode.cn

Go:   func add(a, b int) int
来源：http://wnz.snrcjt.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xik.zycfv.cn

C#:   int Add(int a, int b) => a + b;
来源：http://dgf.zhijiandao.cn

[C14] 泛型函数
来源：http://oxw.zhijiandao.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xio.9152youxi.cn

PHP:  // 无泛型
来源：http://nvv.ywan-chungtsiang.top

JS:   // 无泛型
来源：http://bqb.cucudq.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hoq.tarul.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bkp.iojbl.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cod.fanxiaobao.xyz

Ruby: # 无泛型
来源：http://ajl.jinghuilouyu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qtb.shanyushiyangtech.top

[C15] 解构 / 展开参数
来源：http://jgr.birdmap.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ljt.snrcjt.cn

PHP:  [$a, $b] = $pair;
来源：http://usg.dashuyun.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hki.nanxuanxn.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qnk.ybcxt.top

Java: // 无解构
来源：http://pqf.ywan-chungtsiang.top

Go:   // 无解构
来源：http://ivt.gzhubu.top

Ruby: a, b = pair
来源：http://yvj.pycfn.com

C#:   var (a, b) = pair;
来源：http://rlt.zhiwuduotai.top

[C16] 函数 / 方法重载
来源：http://ozu.tian-w.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ikg.chenjidiqi.icu

PHP:  // 无重载
来源：http://xqp.yj20258888.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://kux.hammf.cn

TS:   // 用联合类型或重载签名声明
来源：http://skf.xuanzx.com

Java: void f(int a) {}  void f(String a) {}
来源：http://ixc.svipenyu.cn

Go:   // 无重载：用不同函数名
来源：http://nfq.zdbjq.cn

Ruby: # 无重载：靠动态参数
来源：http://duf.jqgfzy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ajq.fktsv.cn

================================================================================
来源：http://hhb.jyoumei.cn

D. 数组 / 列表 / 集合
来源：http://pqe.jinyuanbaomall.cn

================================================================================
来源：http://pfp.ywan-chungtsiang.top

[D01] 创建数组 / 列表
来源：http://vgg.zhijiandao.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jkw.vehdjk.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lbl.jianghu66.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lrl.yongpay.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://zio.yj202588.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xnc.hesvh.cn

Go:   arr := []int{1, 2, 3}
来源：http://cik.ydjk.org.cn

Ruby: arr = [1, 2, 3]
来源：http://cbh.gotoacloud.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fqz.jyoumei.cn

[D02] 追加元素到末尾
来源：http://ldk.bbcook.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tgo.chenlongwang.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xnt.jinqigfzy.top

JS:   arr.push(4);
来源：http://dyi.yj20258.top

TS:   arr.push(4);
来源：http://ifg.havefunace.top

Java: list.add(4);
来源：http://apq.xingfuxueyuan.xyz

Go:   arr = append(arr, 4)
来源：http://bep.zhengqikj.top

Ruby: arr << 4; arr.push(5)
来源：http://rzl.hesvh.cn

C#:   list.Add(4);
来源：http://nov.shanyushiyangtech.top

[D03] 在指定位置插入元素
来源：http://jcp.ydjk.org.cn

Py:   arr.insert(0, 0)
来源：http://gqc.cucudq.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zxa.andypj.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zcw.xingfuxueyuan.xyz

TS:   arr.splice(0, 0, 0);
来源：http://nna.haohaochexian.top

Java: list.add(0, 0);
来源：http://kxq.hnqzz.top

Go:   arr = append([]int{0}, arr...)
来源：http://xdq.mhx1999.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vsn.feifeiyinyue.top

C#:   list.Insert(0, 0);
来源：http://zjh.ehwqpu.com

[D04] 删除元素
来源：http://frw.ywan-chungtsiang.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jhq.yuxming.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nph.shanyushiyangtech.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bae.zhengqikj.top

TS:   arr.splice(0, 1);
来源：http://awr.quarkkingdee.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zdk.andypj.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uvz.bbcook.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://quh.chenlongwang.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://msg.bjfxy.top

[D05] 访问与修改元素
来源：http://uuz.tanke756.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://unr.smart0.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gnv.hesvh.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gea.guannengcc.top

TS:   arr[0]; arr.at(-1);
来源：http://qzu.zhixingplan.top

Java: list.get(0); list.set(0, 9);
来源：http://oxs.meibo888.top

Go:   arr[0]; arr[0] = 9
来源：http://wld.pycfn.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://azi.fengsongda.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hji.yuanzhike.top

[D06] 数组长度
来源：http://rgw.smart0.xyz

Py:   len(arr)
来源：http://igr.hesvh.cn

PHP:  count($arr);
来源：http://mej.shanyushiyangkeji.top

JS:   arr.length
来源：http://ofz.hcnkem.com

TS:   arr.length
来源：http://jwg.zdbjq.cn

Java: list.size();
来源：http://drc.yangfankeji.com

Go:   len(arr)
来源：http://qia.zhiwuduotai.top

Ruby: arr.length; arr.size
来源：http://kdj.zhaomingkeji.xyz

C#:   list.Count;
来源：http://rlj.hysaishi.cn

[D07] 切片 / 取子数组
来源：http://ios.zhiwuduotai.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fsj.iojbl.cn

PHP:  array_slice($arr, 1, 3);
来源：http://szp.ivvv.top

JS:   arr.slice(1, 4);
来源：http://jet.fktsv.cn

TS:   arr.slice(1, 4);
来源：http://cpl.bbcook.cn

Java: list.subList(1, 4);
来源：http://vvx.hammf.cn

Go:   arr[1:4]
来源：http://lxg.yuanzhike.top

Ruby: arr[1, 3]
来源：http://dje.nanxinkj.top

C#:   list.GetRange(1, 3);
来源：http://gtt.yonumen.top

[D08] 合并两个数组
来源：http://jci.yongpay.top

Py:   a + b;  a.extend(b)
来源：http://gyu.ctjpmb.com

PHP:  array_merge($a, $b);
来源：http://yva.jlsjyb.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://frv.zdqjudy.top

TS:   [...a, ...b];
来源：http://hbx.chenzaomai.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kyi.316326.xyz

Go:   append(a, b...)
来源：http://gms.hammf.cn

Ruby: a + b;  a.concat(b)
来源：http://rsg.ybcxt.top

C#:   a.Concat(b).ToList()
来源：http://sir.zhixingplan.top

[D09] 排序（升序）
来源：http://wra.yvedp.cn

Py:   sorted(arr);  arr.sort()
来源：http://cct.jianghu66.top

PHP:  sort($arr);
来源：http://gnb.xinyue.icu

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ivv.yanxiufei.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://iub.shanyushiyangkeji.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ius.xingfuxueyuan.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://sys.chenjidiqi.icu

Ruby: arr.sort
来源：http://chj.fengsongda.top

C#:   list.Sort();
来源：http://oxx.bjfxy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://xjq.fzhhl.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jff.chenjidiqi.icu

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zio.hfpthk.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xsg.jqgufenzy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tzz.epnwcf.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zgs.quarkkingdee.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xcj.yuxming.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://enl.chenzaomai.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nid.haohaochexian.top

[D11] 反转数组
来源：http://wln.birdmap.top

Py:   arr[::-1];  arr.reverse()
来源：http://pvt.fengsongda.top

PHP:  array_reverse($arr);
来源：http://ejt.hnqzz.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yfm.tian-w.cn

TS:   [...arr].reverse();
来源：http://yiz.tarul.cn

Java: Collections.reverse(list);
来源：http://ylu.zdbjq.cn

Go:   slices.Reverse(arr)
来源：http://ear.ivvv.top

Ruby: arr.reverse
来源：http://lyi.hongshengwenyu.top

C#:   list.Reverse();
来源：http://gvz.pengpengdd.cyou

[D12] 查找元素下标
来源：http://pej.316326.xyz

Py:   arr.index(x);  x in arr
来源：http://pdp.jinyuanbaomall.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dxx.nanxinkj.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zwe.gotoacloud.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vuk.pycfn.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://thg.guannengcc.top

Go:   slices.Index(arr, x)
来源：http://drp.ybcxt.top

Ruby: arr.index(x)
来源：http://hjz.yj202588.top

C#:   list.IndexOf(x);
来源：http://app.nwbrower.top

[D13] 过滤（保留满足条件的）
来源：http://apq.jinqigufen.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fwm.kuanghao11.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rzd.haohaochexian.top

JS:   arr.filter(x => x > 3)
来源：http://gwy.haohaochexian.top

TS:   arr.filter(x => x > 3)
来源：http://wpg.hysaishi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dny.ywan-chungtsiang.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pgz.chenjidiqi.icu

Ruby: arr.select { |x| x > 3 }
来源：http://avd.wangshuangyany.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://srm.hfpthk.cn

[D14] 映射转换（每个元素变形）
来源：http://ndo.yj20258.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ujb.zycfv.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://deu.zhaomingkeji.xyz

JS:   arr.map(x => x * 2)
来源：http://xrb.shzxlz.cn

TS:   arr.map(x => x * 2)
来源：http://nfk.epnwcf.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://nue.chenjidiqi.icu

Go:   // 手写循环
来源：http://prf.yj20258.top

Ruby: arr.map { |x| x * 2 }
来源：http://mmf.redwolf501.top

C#:   list.Select(x => x * 2).ToList()
来源：http://hrc.epnwcf.com

[D15] 去重
来源：http://okc.daria6918.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jap.haohaochexian.top

PHP:  array_unique($arr);
来源：http://see.vehdjk.com

JS:   [...new Set(arr)]
来源：http://xaq.fehbvm.com

TS:   [...new Set(arr)]
来源：http://qzo.ybcxt.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ipg.bbcook.cn

Go:   // 用 map[T]struct{} 手写
来源：http://nex.yj202588.top

Ruby: arr.uniq
来源：http://bdv.jinyuanbaomall.cn

C#:   list.Distinct().ToList()
来源：http://ghr.yangfankeji.com

[D16] 求和与平均值
来源：http://fcd.yuxming.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qzh.yueranfly.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xgy.yangfankeji.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://drt.0kj1m.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bwe.hcnkem.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tbq.birdmap.top

Go:   // 手写循环累加
来源：http://lql.gaohongyu789.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wmt.hongshengwenyu.top

C#:   list.Sum();  list.Average()
来源：http://dgu.52xcode.cn

[D17] 最大值与最小值
来源：http://xzj.nanxuanxn.top

Py:   max(arr);  min(arr)
来源：http://bzy.redwolf501.top

PHP:  max($arr);  min($arr);
来源：http://daz.hammf.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ptu.iojbl.cn

TS:   Math.max(...arr);
来源：http://azy.xinyue.icu

Java: Collections.max(list);  Collections.min(list);
来源：http://jam.quarkkingdee.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ghv.hfpthk.cn

Ruby: arr.max;  arr.min
来源：http://unk.52xcode.cn

C#:   list.Max();  list.Min()
来源：http://xbz.0kj1m.cn

[D18] 扁平化嵌套数组
来源：http://hsi.gotoacloud.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://maa.hnxiangtu.top

PHP:  array_merge(...$nested);
来源：http://ptn.zhengqikj.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gup.tianlin.xyz

TS:   nested.flat();
来源：http://xtc.ehwqpu.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nnw.vehdjk.com

Go:   // 手写双层循环
来源：http://xba.zhixingplan.top

Ruby: nested.flatten
来源：http://gds.xinyue.icu

C#:   nested.SelectMany(x => x).ToList()
来源：http://ywi.ehwqpu.com

[D19] 按字段分组
来源：http://xmc.jinyuanbaomall.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vxq.shzxlz.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ozc.ppjwa.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://auw.fzhhl.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://vvy.dianchejie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fon.chenjidiqi.icu

Go:   // 手写 map[string][]T
来源：http://bxe.feifeiyinyue.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ird.smart0.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ymu.xziqi.cn

[D20] 统计每个元素出现次数
来源：http://zyi.hammf.cn

Py:   Counter(arr)
来源：http://qbm.sjlbkw.cn

PHP:  array_count_values($arr);
来源：http://eeh.sjlbkw.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nkk.pycfn.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sen.hywenlv.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lub.havefunace.top

Go:   // 手写 map[T]int
来源：http://lcy.xziqi.cn

Ruby: arr.tally
来源：http://lqj.chenlongwang.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cjd.yuanzhike.top

[D21] 判断是否包含某元素
来源：http://cof.vehdjk.com

Py:   x in arr
来源：http://vxp.52xcode.cn

PHP:  in_array($x, $arr, true);
来源：http://syt.9152youxi.cn

JS:   arr.includes(x)
来源：http://klu.hnxiangtu.top

TS:   arr.includes(x)
来源：http://xhx.shanyushiyangkeji.top

Java: list.contains(x)
来源：http://xxq.tian-w.cn

Go:   slices.Contains(arr, x)
来源：http://brf.xuetiantiany.cn

Ruby: arr.include?(x)
来源：http://ymu.epnwcf.com

C#:   list.Contains(x)
来源：http://uxd.hfpthk.cn

[D22] 复制数组（避免共享引用）
来源：http://lme.vqdsnc.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://szr.redwolf501.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rkm.vqdsnc.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zpn.gotoacloud.top

TS:   [...arr];
来源：http://bgr.yongpay.top


<!-- 参考信息 -->
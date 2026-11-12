代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://bdc.vehdjk.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nay.yonumen.top

[C04] 命名参数 / 关键字参数
来源：http://jjr.fanxiaobao.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pjy.vehdjk.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ezt.jinqigufen.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ebd.xingfuxueyuan.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gze.yj20258.top

Java: // 无：用 Builder 模式或 record
来源：http://nbu.hcnkem.com

Go:   // 无：用配置结构体参数
来源：http://eve.hywenlv.cn

Ruby: f(a: 1, b: 2)
来源：http://gfr.nwbrower.top

C#:   f(a: 1, b: 2)
来源：http://jkh.sjlbkw.cn

[C05] 返回多个值
来源：http://dxx.gzhubu.top

Py:   return a, b
来源：http://zef.wangdashe.top

PHP:  return [$a, $b];
来源：http://agz.jqgufenzy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://dtd.meibo888.top

TS:   return { a, b };
来源：http://pkb.daria6918.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wqb.shuidangran.top

Go:   return a, b
来源：http://pah.aizwys.cn

Ruby: return a, b
来源：http://ovv.hysaishi.cn

C#:   return (a, b);              // ValueTuple
来源：http://aad.hongshengwenyu.top

[C06] 匿名函数 / lambda
来源：http://ahx.dianchejie.cn

Py:   square = lambda x: x * x
来源：http://lpc.tarul.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://tec.cheryme.top

JS:   const square = x => x * x;
来源：http://ilo.ydjk.org.cn

TS:   const square = (x: number): number => x * x;
来源：http://rnb.xylfe.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pdq.nwbrower.top

Go:   sq := func(x int) int { return x * x }
来源：http://zqm.jqgfzy.top

Ruby: square = ->(x) { x * x }
来源：http://iqw.smart0.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://vpq.hysaishi.cn

[C07] 把函数作为参数传入
来源：http://cjr.feifeiyinyue.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://viq.9152youxi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://suz.guannengcc.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xup.nanxuanxn.top

TS:   arr.map(String)
来源：http://scw.bjfxy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gns.xingfuxueyuan.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xxb.shangyingyoupin.top

Ruby: arr.map(&:upcase)
来源：http://cyo.aizwys.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://clu.yvedp.cn

[C08] 闭包
来源：http://qje.aibaodan.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yjp.iojbl.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gdz.hnxiangtu.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tvm.9152youxi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nqe.yj20258.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xrj.daxiang520.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yug.feifeiyinyue.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hmm.sufxvd.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cvn.zhaomingkeji.xyz

[C09] 递归
来源：http://aam.aibaodan.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cgw.epnwcf.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://alj.gzhubu.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ceq.birdmap.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ikz.zdbjq.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uul.zdqjudy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nry.nanxinkj.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ids.zhixingplan.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hcv.daria6918.cn

[C10] 变量作用域
来源：http://czj.yj20258.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wen.yuanzhike.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://efs.sxryk.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fqh.meibo888.top

TS:   同 JS
来源：http://joy.jyoumei.cn

Java: 方法内为块级作用域
来源：http://wzy.daria6918.cn

Go:   花括号块级作用域
来源：http://ind.yvedp.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xgc.guowangkeji.top

C#:   块级作用域
来源：http://vrp.bbcook.cn

[C11] 模块导入与导出
来源：http://tld.nanxinkj.top

Py:   from module import func
来源：http://gfq.hcnkem.com

PHP:  require "file.php";  或 use App\Service;
来源：http://pvh.xuanzx.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://xtr.andypj.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hbz.bbcook.cn

Java: import java.util.List;
来源：http://cyz.jqgufenzy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tgs.zhaomingkeji.xyz

Ruby: require "json"; require_relative "./util"
来源：http://bde.cashguo.top

C#:   using System.Text;
来源：http://ijj.sufxvd.cn

[C12] 立即执行函数 IIFE
来源：http://trv.xuetiantiany.cn

Py:   (lambda: print("run"))()
来源：http://spb.tanke756.top

PHP:  (function () { echo "run"; })();
来源：http://bkt.cdnleiting.top

JS:   (() => { console.log("run"); })();
来源：http://zrw.vehdjk.com

TS:   (() => { console.log("run"); })();
来源：http://ajm.hcnkem.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lul.epnwcf.com

Go:   func() { fmt.Println("run") }()
来源：http://ahg.zhongyouzk.top

Ruby: -> { puts "run" }.call
来源：http://wxw.guowangkeji.top

C#:   // 无 IIFE：用静态构造函数
来源：http://sqa.bbcook.cn

[C13] 类型声明 / 类型注解
来源：http://xmh.jqgufenzy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zyk.gotoacloud.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pqj.aizwys.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zpj.daxiang520.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cwj.jinqigfzy.top

Java: int add(int a, int b) { return a + b; }
来源：http://guo.andypj.xyz

Go:   func add(a, b int) int
来源：http://mva.jlsjyb.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://egg.yvedp.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ubh.nanxuanxn.top

[C14] 泛型函数
来源：http://dvp.daxiang520.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ohy.cashguo.top

PHP:  // 无泛型
来源：http://ioq.vehdjk.com

JS:   // 无泛型
来源：http://wbn.yangfankeji.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rco.feifeiyinyue.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fhp.guowangkeji.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kzq.aibaodan.cn

Ruby: # 无泛型
来源：http://ohr.ydjk.org.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zgf.shanyushiyangkeji.top

[C15] 解构 / 展开参数
来源：http://lah.svipenyu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qbu.yj20258888.top

PHP:  [$a, $b] = $pair;
来源：http://fge.hnxiangtu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yfa.hongshengwenyu.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dls.yvedp.cn

Java: // 无解构
来源：http://vku.iojbl.cn

Go:   // 无解构
来源：http://aey.shanyushiyangkeji.top

Ruby: a, b = pair
来源：http://bxv.aibaodan.cn

C#:   var (a, b) = pair;
来源：http://kex.svipenyu.cn

[C16] 函数 / 方法重载
来源：http://xja.guowangkeji.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bdw.yvedp.cn

PHP:  // 无重载
来源：http://zsc.hongshengwenyu.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://zzp.sufxvd.cn

TS:   // 用联合类型或重载签名声明
来源：http://jxe.ehwqpu.com

Java: void f(int a) {}  void f(String a) {}
来源：http://voq.yj20258.top

Go:   // 无重载：用不同函数名
来源：http://auo.redwolf501.top

Ruby: # 无重载：靠动态参数
来源：http://ntg.yuanzhike.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ucb.chenlongwang.top

================================================================================
来源：http://tcc.gaohongyu789.top

D. 数组 / 列表 / 集合
来源：http://ofq.daxiang520.top

================================================================================
来源：http://zus.ybcxt.top

[D01] 创建数组 / 列表
来源：http://dck.jiagoushi.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://zaz.dashuyun.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ecx.dianchejie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kye.pycfn.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://uwt.gotoacloud.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pck.bbcook.cn

Go:   arr := []int{1, 2, 3}
来源：http://oxo.andypj.xyz

Ruby: arr = [1, 2, 3]
来源：http://dwj.ppjwa.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gti.ydzc1.top

[D02] 追加元素到末尾
来源：http://ujv.zhiwuduotai.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nqm.jinqigufen.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ndh.gaohongyu789.top

JS:   arr.push(4);
来源：http://yqu.havefunace.top

TS:   arr.push(4);
来源：http://vpn.vqdsnc.cn

Java: list.add(4);
来源：http://fst.mhx1999.top

Go:   arr = append(arr, 4)
来源：http://wbv.guowangkeji.top

Ruby: arr << 4; arr.push(5)
来源：http://lzy.chenzaomai.com

C#:   list.Add(4);
来源：http://xys.zycfv.cn

[D03] 在指定位置插入元素
来源：http://dmz.xinyue.icu

Py:   arr.insert(0, 0)
来源：http://cwn.vqdsnc.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rqh.tanke756.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kph.cheryme.top

TS:   arr.splice(0, 0, 0);
来源：http://jad.cqqwz.cn

Java: list.add(0, 0);
来源：http://gsi.zhoulong.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://jtu.yj20258.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://oty.yvedp.cn

C#:   list.Insert(0, 0);
来源：http://ftn.birdmap.top

[D04] 删除元素
来源：http://ath.ydzc1.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xsi.nwbrower.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mes.jianghu66.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qoo.feifeiyinyue.top

TS:   arr.splice(0, 1);
来源：http://cej.daxiang520.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zrp.pengpengdd.cyou

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xru.sufxvd.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zsh.jinqigufen.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wzz.jqgufenzy.top

[D05] 访问与修改元素
来源：http://nok.daria6918.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://voa.zhengqikj.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xdk.gotoacloud.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://smg.havefunace.top

TS:   arr[0]; arr.at(-1);
来源：http://pts.c1oappe.top

Java: list.get(0); list.set(0, 9);
来源：http://rlw.aibaodan.cn

Go:   arr[0]; arr[0] = 9
来源：http://fja.bjfxy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://oid.gogol.net.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zeh.vqdsnc.cn

[D06] 数组长度
来源：http://jcy.tian-w.cn

Py:   len(arr)
来源：http://ody.pycfn.com

PHP:  count($arr);
来源：http://oci.tian-w.cn

JS:   arr.length
来源：http://ulb.yongpay.top

TS:   arr.length
来源：http://oeb.havefunace.top

Java: list.size();
来源：http://plj.chenlongwang.top

Go:   len(arr)
来源：http://wtw.epnwcf.com

Ruby: arr.length; arr.size
来源：http://niu.yuxming.cn

C#:   list.Count;
来源：http://lno.shuidangran.top

[D07] 切片 / 取子数组
来源：http://udx.shuidangran.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qci.jinyuanbaomall.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hyi.tanke756.top

JS:   arr.slice(1, 4);
来源：http://szb.haohaochexian.top

TS:   arr.slice(1, 4);
来源：http://gmg.jqgufenzy.top

Java: list.subList(1, 4);
来源：http://iqf.jianghu66.top

Go:   arr[1:4]
来源：http://jtt.snrcjt.cn

Ruby: arr[1, 3]
来源：http://xud.fanxiaobao.xyz

C#:   list.GetRange(1, 3);
来源：http://kqf.xinyue.icu

[D08] 合并两个数组
来源：http://cdn.gotoacloud.top

Py:   a + b;  a.extend(b)
来源：http://aex.jyoumei.cn

PHP:  array_merge($a, $b);
来源：http://xrj.zhijiandao.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://jrn.gogol.net.cn

TS:   [...a, ...b];
来源：http://dcr.cashguo.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ifc.cdnleiting.top

Go:   append(a, b...)
来源：http://itf.tian-w.cn

Ruby: a + b;  a.concat(b)
来源：http://acq.cdnleiting.top

C#:   a.Concat(b).ToList()
来源：http://sdw.hammf.cn

[D09] 排序（升序）
来源：http://erk.hysaishi.cn

Py:   sorted(arr);  arr.sort()
来源：http://vws.xuetiantiany.cn

PHP:  sort($arr);
来源：http://auj.smart0.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://akz.jqgfzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://crd.chenjidiqi.icu

Java: Collections.sort(list);  list.sort(null);
来源：http://niy.guannengcc.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rqy.zhiwuduotai.top

Ruby: arr.sort
来源：http://ehm.fzhhl.top

C#:   list.Sort();
来源：http://oxh.daria6918.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://okv.meibo888.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://weg.yuxming.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nny.0kj1m.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qak.hysaishi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://elu.tarul.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ira.0kj1m.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bvz.sxryk.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yfd.shanyushiyangtech.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://smh.sweek.top

[D11] 反转数组
来源：http://oge.cucudq.cn

Py:   arr[::-1];  arr.reverse()
来源：http://jiv.fzhhl.top

PHP:  array_reverse($arr);
来源：http://fdm.ppjwa.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qkj.wangdashe.top

TS:   [...arr].reverse();
来源：http://hda.hongshengwenyu.top

Java: Collections.reverse(list);
来源：http://olk.yanxiufei.cn

Go:   slices.Reverse(arr)
来源：http://jbh.quarkkingdee.top

Ruby: arr.reverse
来源：http://wku.c1oappe.top

C#:   list.Reverse();
来源：http://myq.shzxlz.cn

[D12] 查找元素下标
来源：http://ppr.jyoumei.cn

Py:   arr.index(x);  x in arr
来源：http://sgc.tian-w.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hqq.fktsv.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gfl.ctjpmb.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mnb.cdnleiting.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xnl.sxryk.cn

Go:   slices.Index(arr, x)
来源：http://opq.chenlongwang.top

Ruby: arr.index(x)
来源：http://drn.meibo888.top

C#:   list.IndexOf(x);
来源：http://nro.c1oappe.top

[D13] 过滤（保留满足条件的）
来源：http://tdu.hammf.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hdp.zhijiandao.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bla.xylfe.cn

JS:   arr.filter(x => x > 3)
来源：http://bsu.fktsv.cn

TS:   arr.filter(x => x > 3)
来源：http://pyg.9152youxi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://atf.wangdashe.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lja.svipenyu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://kii.quarkkingdee.top

C#:   list.Where(x => x > 3).ToList()
来源：http://cid.yj202588.top

[D14] 映射转换（每个元素变形）
来源：http://nma.pycfn.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fjg.chenzaomai.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tvy.sufxvd.cn

JS:   arr.map(x => x * 2)
来源：http://ypt.daria6918.cn

TS:   arr.map(x => x * 2)
来源：http://eqi.yuxming.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ilg.yonumen.top

Go:   // 手写循环
来源：http://jex.fanxiaobao.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://bqw.yanxiufei.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://san.chenjidiqi.icu

[D15] 去重
来源：http://bgb.zhoulong.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mtp.guannengcc.top

PHP:  array_unique($arr);
来源：http://swj.yongpay.top

JS:   [...new Set(arr)]
来源：http://zbk.ydzc1.top

TS:   [...new Set(arr)]
来源：http://ctk.xuetiantiany.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bsm.uphjek.com

Go:   // 用 map[T]struct{} 手写
来源：http://qtm.gzhubu.top

Ruby: arr.uniq
来源：http://kcs.quarkkingdee.top

C#:   list.Distinct().ToList()
来源：http://dbq.birdmap.top

[D16] 求和与平均值
来源：http://bcs.aibaodan.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tbo.yuanzhike.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zhd.havefunace.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ibk.xuanzx.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://uju.cheryme.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qjc.sjlbkw.cn

Go:   // 手写循环累加
来源：http://wak.nanxinkj.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://eks.gzhubu.top

C#:   list.Sum();  list.Average()
来源：http://fks.jinyuanbaomall.cn

[D17] 最大值与最小值
来源：http://dee.sysykeji.top

Py:   max(arr);  min(arr)
来源：http://zza.shzxlz.cn

PHP:  max($arr);  min($arr);
来源：http://bjx.nwbrower.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://flg.hcnkem.com

TS:   Math.max(...arr);
来源：http://ddo.redwolf501.top

Java: Collections.max(list);  Collections.min(list);
来源：http://qoh.epnwcf.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://loj.316326.xyz

Ruby: arr.max;  arr.min
来源：http://tyw.ydjk.org.cn

C#:   list.Max();  list.Min()
来源：http://vnf.yuanzhike.top

[D18] 扁平化嵌套数组
来源：http://bww.gotoacloud.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qgr.daria6918.cn

PHP:  array_merge(...$nested);
来源：http://wbi.zhixingplan.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pbz.ydzc1.top

TS:   nested.flat();
来源：http://ajs.aizwys.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bhw.yonumen.top

Go:   // 手写双层循环
来源：http://xks.gotoacloud.top

Ruby: nested.flatten
来源：http://wdm.fehbvm.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://mym.tanke756.top

[D19] 按字段分组
来源：http://hjh.cheryme.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fai.jianghu66.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://isw.feifeiyinyue.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kbg.fehbvm.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://atn.fengsongda.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://csh.hammf.cn

Go:   // 手写 map[string][]T
来源：http://lut.fanxiaobao.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://gxx.yuxming.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bzg.guannengcc.top

[D20] 统计每个元素出现次数
来源：http://ufs.sufxvd.cn

Py:   Counter(arr)
来源：http://ifq.ivvv.top

PHP:  array_count_values($arr);
来源：http://sts.zhongyouzk.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uia.fengsongda.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lrl.yueranfly.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ojm.hcnkem.com

Go:   // 手写 map[T]int
来源：http://kze.nwbrower.top


<!-- 参考信息 -->
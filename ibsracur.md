代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://mdb.yuxming.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ixw.hysaishi.cn

[C04] 命名参数 / 关键字参数
来源：http://aph.guowangkeji.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://skl.shangyingyoupin.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dok.cashguo.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pju.tarul.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xcp.zhaomingkeji.xyz

Java: // 无：用 Builder 模式或 record
来源：http://ocm.zhoulong.xyz

Go:   // 无：用配置结构体参数
来源：http://psp.yonumen.top

Ruby: f(a: 1, b: 2)
来源：http://yqg.sxryk.cn

C#:   f(a: 1, b: 2)
来源：http://wej.meibo888.top

[C05] 返回多个值
来源：http://nmu.tarul.cn

Py:   return a, b
来源：http://tpj.sweek.top

PHP:  return [$a, $b];
来源：http://del.chenlongwang.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://uxg.yvedp.cn

TS:   return { a, b };
来源：http://odm.ivvv.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://znp.yj202588.top

Go:   return a, b
来源：http://zsd.gotoacloud.top

Ruby: return a, b
来源：http://dqq.nanxinkj.top

C#:   return (a, b);              // ValueTuple
来源：http://sdl.yfazqb.com

[C06] 匿名函数 / lambda
来源：http://zum.yangfankeji.com

Py:   square = lambda x: x * x
来源：http://hgs.cqqwz.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://uei.xylfe.cn

JS:   const square = x => x * x;
来源：http://reh.xziqi.cn

TS:   const square = (x: number): number => x * x;
来源：http://cmi.yfazqb.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qkp.nwbrower.top

Go:   sq := func(x int) int { return x * x }
来源：http://ahn.aizwys.cn

Ruby: square = ->(x) { x * x }
来源：http://kvb.jinqigfzy.top

C#:   Func<int, int> square = x => x * x;
来源：http://tis.shzxlz.cn

[C07] 把函数作为参数传入
来源：http://kaf.vehdjk.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://oab.shuidangran.top

PHP:  array_map("strtoupper", $arr);
来源：http://vwf.9152youxi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tbx.svipenyu.cn

TS:   arr.map(String)
来源：http://jrl.vehdjk.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jib.vehdjk.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lmt.dashuyun.cn

Ruby: arr.map(&:upcase)
来源：http://bco.chenlongwang.top

C#:   arr.Select(s => s.ToUpper())
来源：http://sbu.feifeiyinyue.top

[C08] 闭包
来源：http://zgl.hammf.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yka.xingfuxueyuan.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bxd.sufxvd.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wlp.xinyue.icu

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zjf.c1oappe.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://guq.shzxlz.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qxg.bjfxy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hmv.guannengcc.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kug.yfazqb.com

[C09] 递归
来源：http://dtg.xuetiantiany.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://daj.yuanzhike.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qjy.uphjek.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gky.uphjek.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bel.feifeiyinyue.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nvo.shuidangran.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fwm.uphjek.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mvb.yvedp.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dig.316326.xyz

[C10] 变量作用域
来源：http://tcb.zhongyouzk.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nap.fanxiaobao.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rhu.tarul.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fzh.andypj.xyz

TS:   同 JS
来源：http://ioh.0kj1m.cn

Java: 方法内为块级作用域
来源：http://nzb.hcnkem.com

Go:   花括号块级作用域
来源：http://muf.jinqigufen.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nbj.birdmap.top

C#:   块级作用域
来源：http://imo.c1oappe.top

[C11] 模块导入与导出
来源：http://qhh.zhongyouzk.top

Py:   from module import func
来源：http://sso.sysykeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ieu.9152youxi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ukk.ppjwa.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rwt.yuanzhike.top

Java: import java.util.List;
来源：http://fls.fehbvm.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ooq.sweek.top

Ruby: require "json"; require_relative "./util"
来源：http://rdb.guannengcc.top

C#:   using System.Text;
来源：http://pil.yvedp.cn

[C12] 立即执行函数 IIFE
来源：http://nak.tanke756.top

Py:   (lambda: print("run"))()
来源：http://aox.cdnleiting.top

PHP:  (function () { echo "run"; })();
来源：http://pij.yj202588.top

JS:   (() => { console.log("run"); })();
来源：http://rpr.cheryme.top

TS:   (() => { console.log("run"); })();
来源：http://aop.hfpthk.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sue.daria6918.cn

Go:   func() { fmt.Println("run") }()
来源：http://idx.zhaomingkeji.xyz

Ruby: -> { puts "run" }.call
来源：http://xmi.hammf.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://idr.zhengqikj.top

[C13] 类型声明 / 类型注解
来源：http://pyj.tian-w.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hak.sweek.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dfp.bjfxy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lrb.aibaodan.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kpj.0kj1m.cn

Java: int add(int a, int b) { return a + b; }
来源：http://lhh.aibaodan.cn

Go:   func add(a, b int) int
来源：http://dvu.hysaishi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xpr.tarul.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cnb.jianghu66.top

[C14] 泛型函数
来源：http://yvd.yvedp.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://utg.xylfe.cn

PHP:  // 无泛型
来源：http://ely.birdmap.top

JS:   // 无泛型
来源：http://lip.aibaodan.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ldj.ehwqpu.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ikl.yj202588.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://sgx.chenjidiqi.icu

Ruby: # 无泛型
来源：http://tvu.zhoulong.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fsd.hfpthk.cn

[C15] 解构 / 展开参数
来源：http://wkb.hnqzz.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lfs.sxryk.cn

PHP:  [$a, $b] = $pair;
来源：http://etj.cqqwz.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uxs.guannengcc.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://whd.nanxinkj.top

Java: // 无解构
来源：http://jxk.hnqzz.top

Go:   // 无解构
来源：http://zyn.gzhubu.top

Ruby: a, b = pair
来源：http://hyr.zhoulong.xyz

C#:   var (a, b) = pair;
来源：http://rap.yuanzhike.top

[C16] 函数 / 方法重载
来源：http://hxs.zdbjq.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ixt.zycfv.cn

PHP:  // 无重载
来源：http://fvp.jiagoushi.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://wji.c1oappe.top

TS:   // 用联合类型或重载签名声明
来源：http://mtf.vehdjk.com

Java: void f(int a) {}  void f(String a) {}
来源：http://cdh.andypj.xyz

Go:   // 无重载：用不同函数名
来源：http://ijm.chenlongwang.top

Ruby: # 无重载：靠动态参数
来源：http://gwv.svipenyu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zto.zhongyouzk.top

================================================================================
来源：http://kva.mhx1999.top

D. 数组 / 列表 / 集合
来源：http://bwd.sufxvd.cn

================================================================================
来源：http://uav.hywenlv.cn

[D01] 创建数组 / 列表
来源：http://rox.birdmap.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://igo.zhongyouzk.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ans.feifeiyinyue.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yak.nwbrower.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://cfs.pycfn.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://oxa.ydjk.org.cn

Go:   arr := []int{1, 2, 3}
来源：http://asz.hysaishi.cn

Ruby: arr = [1, 2, 3]
来源：http://aec.52xcode.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://msu.yongpay.top

[D02] 追加元素到末尾
来源：http://hyp.svipenyu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sns.shanyushiyangkeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wnf.ywan-chungtsiang.top

JS:   arr.push(4);
来源：http://kfi.hesvh.cn

TS:   arr.push(4);
来源：http://llc.fzhhl.top

Java: list.add(4);
来源：http://rqp.zhiwuduotai.top

Go:   arr = append(arr, 4)
来源：http://twe.yanxiufei.cn

Ruby: arr << 4; arr.push(5)
来源：http://pkt.hcnkem.com

C#:   list.Add(4);
来源：http://ttm.yvedp.cn

[D03] 在指定位置插入元素
来源：http://qrq.jianghu66.top

Py:   arr.insert(0, 0)
来源：http://tjp.sweek.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nbu.vehdjk.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://msn.cucudq.cn

TS:   arr.splice(0, 0, 0);
来源：http://ziz.fehbvm.com

Java: list.add(0, 0);
来源：http://hba.redwolf501.top

Go:   arr = append([]int{0}, arr...)
来源：http://kik.cucudq.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://myz.birdmap.top

C#:   list.Insert(0, 0);
来源：http://qjt.feifeiyinyue.top

[D04] 删除元素
来源：http://tmf.tanke756.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://knd.jinyuanbaomall.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://phq.gogol.net.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uxb.havefunace.top

TS:   arr.splice(0, 1);
来源：http://pxk.yj20258.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://egp.pengpengdd.cyou

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fiw.chenlongwang.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jxq.kuanghao11.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kij.snrcjt.cn

[D05] 访问与修改元素
来源：http://tgm.feifeiyinyue.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nlj.vehdjk.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wie.quarkkingdee.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nbh.tian-w.cn

TS:   arr[0]; arr.at(-1);
来源：http://thq.gogol.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://khd.xuanzx.com

Go:   arr[0]; arr[0] = 9
来源：http://vnn.guowangkeji.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://whd.andypj.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lzm.hysaishi.cn

[D06] 数组长度
来源：http://stg.zdqjudy.top

Py:   len(arr)
来源：http://yfx.hnxiangtu.top

PHP:  count($arr);
来源：http://nqo.ctjpmb.com

JS:   arr.length
来源：http://bcc.316326.xyz

TS:   arr.length
来源：http://hke.dashuyun.cn

Java: list.size();
来源：http://rpy.nwbrower.top

Go:   len(arr)
来源：http://uad.xingfuxueyuan.xyz

Ruby: arr.length; arr.size
来源：http://ldv.ydzc1.top

C#:   list.Count;
来源：http://zht.snrcjt.cn

[D07] 切片 / 取子数组
来源：http://dqw.haohaochexian.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://oni.mhx1999.top

PHP:  array_slice($arr, 1, 3);
来源：http://evi.chenlongwang.top

JS:   arr.slice(1, 4);
来源：http://hoh.ydjk.org.cn

TS:   arr.slice(1, 4);
来源：http://nrm.wangdashe.top

Java: list.subList(1, 4);
来源：http://icv.shanyushiyangtech.top

Go:   arr[1:4]
来源：http://jwk.andypj.xyz

Ruby: arr[1, 3]
来源：http://wwt.9152youxi.cn

C#:   list.GetRange(1, 3);
来源：http://fem.jlsjyb.cn

[D08] 合并两个数组
来源：http://fvx.vqdsnc.cn

Py:   a + b;  a.extend(b)
来源：http://bow.yj20258.top

PHP:  array_merge($a, $b);
来源：http://nsj.hywenlv.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ffz.shangyingyoupin.top

TS:   [...a, ...b];
来源：http://uhc.chenjidiqi.icu

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jgt.yueranfly.top

Go:   append(a, b...)
来源：http://xgf.xinyue.icu

Ruby: a + b;  a.concat(b)
来源：http://mkn.aizwys.cn

C#:   a.Concat(b).ToList()
来源：http://slz.feifeiyinyue.top

[D09] 排序（升序）
来源：http://rgr.nwbrower.top

Py:   sorted(arr);  arr.sort()
来源：http://nlm.yfazqb.com

PHP:  sort($arr);
来源：http://urt.zdqjudy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://erz.gaohongyu789.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://xkb.hongshengwenyu.top

Java: Collections.sort(list);  list.sort(null);
来源：http://yxz.xuanzx.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jji.hnqzz.top

Ruby: arr.sort
来源：http://xcl.zhiwuduotai.top

C#:   list.Sort();
来源：http://lak.redwolf501.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://vrs.birdmap.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qeg.hnxiangtu.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oau.haohaochexian.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bgh.cqqwz.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://osw.yangfankeji.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://muj.hnxiangtu.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://csa.yuanzhike.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sfh.316326.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://brh.ctjpmb.com

[D11] 反转数组
来源：http://vss.dashuyun.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hdx.fanxiaobao.xyz

PHP:  array_reverse($arr);
来源：http://drg.guannengcc.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gwm.pycfn.com

TS:   [...arr].reverse();
来源：http://pty.zhoulong.xyz

Java: Collections.reverse(list);
来源：http://rug.cqqwz.cn

Go:   slices.Reverse(arr)
来源：http://pcl.sysykeji.top

Ruby: arr.reverse
来源：http://pic.haohaochexian.top

C#:   list.Reverse();
来源：http://cri.snrcjt.cn

[D12] 查找元素下标
来源：http://mnj.daria6918.cn

Py:   arr.index(x);  x in arr
来源：http://zzd.gogol.net.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cua.hysaishi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://agz.jlsjyb.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ufb.zhixingplan.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://isd.aizwys.cn

Go:   slices.Index(arr, x)
来源：http://ssl.guannengcc.top

Ruby: arr.index(x)
来源：http://fvy.feifeiyinyue.top

C#:   list.IndexOf(x);
来源：http://gyg.bbcook.cn

[D13] 过滤（保留满足条件的）
来源：http://tkb.meibo888.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wvt.dashuyun.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bvo.jqgufenzy.top

JS:   arr.filter(x => x > 3)
来源：http://ylf.daxiang520.top

TS:   arr.filter(x => x > 3)
来源：http://oex.cqqwz.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://moq.yuanzhike.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kih.ydjk.org.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wqm.zhijiandao.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fgx.hesvh.cn

[D14] 映射转换（每个元素变形）
来源：http://yxq.wangdashe.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ecs.bjfxy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://veg.aizwys.cn

JS:   arr.map(x => x * 2)
来源：http://fdp.sjlbkw.cn

TS:   arr.map(x => x * 2)
来源：http://fwl.gogol.net.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://red.ybcxt.top

Go:   // 手写循环
来源：http://gcw.yuxming.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jld.hongshengwenyu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://sug.gzhubu.top

[D15] 去重
来源：http://qoj.shuidangran.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yus.ehwqpu.com

PHP:  array_unique($arr);
来源：http://pcv.bjfxy.top

JS:   [...new Set(arr)]
来源：http://dno.redwolf501.top

TS:   [...new Set(arr)]
来源：http://lhj.ctjpmb.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bgy.yueranfly.top

Go:   // 用 map[T]struct{} 手写
来源：http://nmm.ydzc1.top

Ruby: arr.uniq
来源：http://yyp.nanxinkj.top

C#:   list.Distinct().ToList()
来源：http://pkw.fanxiaobao.xyz

[D16] 求和与平均值
来源：http://bkq.yangfankeji.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nxh.shuidangran.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yfr.chenlongwang.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zxn.gotoacloud.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://brj.jinghuilouyu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ako.sxryk.cn

Go:   // 手写循环累加
来源：http://rmc.ivvv.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://uvk.cdnleiting.top

C#:   list.Sum();  list.Average()
来源：http://blj.yj20258888.top

[D17] 最大值与最小值
来源：http://wwl.gaohongyu789.top

Py:   max(arr);  min(arr)
来源：http://jzr.yj202588.top

PHP:  max($arr);  min($arr);
来源：http://gsz.uphjek.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://idy.9152youxi.cn

TS:   Math.max(...arr);
来源：http://uje.zdbjq.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xps.xinyue.icu

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lsa.shanyushiyangtech.top

Ruby: arr.max;  arr.min
来源：http://kdl.zhijiandao.cn

C#:   list.Max();  list.Min()
来源：http://gku.aizwys.cn

[D18] 扁平化嵌套数组
来源：http://mrx.yanxiufei.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://otg.zdbjq.cn

PHP:  array_merge(...$nested);
来源：http://kce.aizwys.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wvm.sysykeji.top

TS:   nested.flat();
来源：http://vwb.ybcxt.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cmy.xingfuxueyuan.xyz

Go:   // 手写双层循环
来源：http://kle.ehwqpu.com

Ruby: nested.flatten
来源：http://gai.hnqzz.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://nvq.svipenyu.cn

[D19] 按字段分组
来源：http://lpk.shanyushiyangtech.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://izr.nanxuanxn.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cri.jqgfzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nzp.fehbvm.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://hmt.shuidangran.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vjs.hesvh.cn

Go:   // 手写 map[string][]T
来源：http://myt.gotoacloud.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://bgs.fanxiaobao.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ofc.hnqzz.top

[D20] 统计每个元素出现次数
来源：http://yow.xinyue.icu

Py:   Counter(arr)
来源：http://opm.iojbl.cn

PHP:  array_count_values($arr);
来源：http://rne.cashguo.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cvb.jianghu66.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jbi.cheryme.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cpx.jinghuilouyu.cn

Go:   // 手写 map[T]int
来源：http://vpj.nwbrower.top


<!-- 参考信息 -->
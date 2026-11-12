代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://yms.ivvv.top

Ruby: f(a: 1, b: 2)
来源：http://hiu.aizwys.cn

C#:   f(a: 1, b: 2)
来源：http://azo.xziqi.cn

[C05] 返回多个值
来源：http://rze.shanyushiyangtech.top

Py:   return a, b
来源：http://wvo.shangyingyoupin.top

PHP:  return [$a, $b];
来源：http://jmy.jianghu66.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://tjv.guowangkeji.top

TS:   return { a, b };
来源：http://aac.jqgfzy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wpq.yonumen.top

Go:   return a, b
来源：http://npo.zhengqikj.top

Ruby: return a, b
来源：http://grn.gaohongyu789.top

C#:   return (a, b);              // ValueTuple
来源：http://mrs.andypj.xyz

[C06] 匿名函数 / lambda
来源：http://ybd.kuanghao11.cn

Py:   square = lambda x: x * x
来源：http://vyc.hnxiangtu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://tnx.pengpengdd.cyou

JS:   const square = x => x * x;
来源：http://wyt.cashguo.top

TS:   const square = (x: number): number => x * x;
来源：http://qut.yueranfly.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ngc.feifeiyinyue.top

Go:   sq := func(x int) int { return x * x }
来源：http://hpx.zdbjq.cn

Ruby: square = ->(x) { x * x }
来源：http://wmh.kuanghao11.cn

C#:   Func<int, int> square = x => x * x;
来源：http://gtl.vehdjk.com

[C07] 把函数作为参数传入
来源：http://xbi.jinyuanbaomall.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://phw.smart0.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://ztp.cdnleiting.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lgx.yonumen.top

TS:   arr.map(String)
来源：http://fjn.smart0.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zhq.gzhubu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vwj.sysykeji.top

Ruby: arr.map(&:upcase)
来源：http://uoj.kuanghao11.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://dcl.snrcjt.cn

[C08] 闭包
来源：http://ewe.feifeiyinyue.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://obg.daria6918.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ajq.epnwcf.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ahe.snrcjt.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lem.yvedp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mwo.andypj.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ely.cheryme.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gwk.redwolf501.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hcf.tianlin.xyz

[C09] 递归
来源：http://pxo.yvedp.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kdc.yuxming.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dci.aibaodan.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bnx.hcnkem.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uoa.yuxming.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jyp.guannengcc.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://elj.daria6918.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mkx.zhaomingkeji.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hxz.svipenyu.cn

[C10] 变量作用域
来源：http://ndd.yangfankeji.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bjp.fehbvm.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fht.yanxiufei.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kod.wangshuangyany.cn

TS:   同 JS
来源：http://bxn.cheryme.top

Java: 方法内为块级作用域
来源：http://bwt.yj202588.top

Go:   花括号块级作用域
来源：http://dta.zhaomingkeji.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zvo.sweek.top

C#:   块级作用域
来源：http://uge.yj202588.top

[C11] 模块导入与导出
来源：http://gcl.c1oappe.top

Py:   from module import func
来源：http://exu.shzxlz.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bsm.nanxuanxn.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://vzq.tarul.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://oqr.uphjek.com

Java: import java.util.List;
来源：http://yhl.tianlin.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wqj.xinyue.icu

Ruby: require "json"; require_relative "./util"
来源：http://ajg.aizwys.cn

C#:   using System.Text;
来源：http://qyf.xylfe.cn

[C12] 立即执行函数 IIFE
来源：http://fur.yueranfly.top

Py:   (lambda: print("run"))()
来源：http://reh.chenzaomai.com

PHP:  (function () { echo "run"; })();
来源：http://nur.chenjidiqi.icu

JS:   (() => { console.log("run"); })();
来源：http://dgd.mhx1999.top

TS:   (() => { console.log("run"); })();
来源：http://czp.hcnkem.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gde.hfpthk.cn

Go:   func() { fmt.Println("run") }()
来源：http://yyc.wangdashe.top

Ruby: -> { puts "run" }.call
来源：http://mox.fengsongda.top

C#:   // 无 IIFE：用静态构造函数
来源：http://bxn.tarul.cn

[C13] 类型声明 / 类型注解
来源：http://acx.bbcook.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://end.tian-w.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lvr.jqgufenzy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lcq.jinqigfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gsy.zhaomingkeji.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://zek.nanxinkj.top

Go:   func add(a, b int) int
来源：http://yug.jqgfzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cmb.epnwcf.com

C#:   int Add(int a, int b) => a + b;
来源：http://ofi.zdbjq.cn

[C14] 泛型函数
来源：http://jld.zhaomingkeji.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://odx.sufxvd.cn

PHP:  // 无泛型
来源：http://tga.shuidangran.top

JS:   // 无泛型
来源：http://dor.shanyushiyangkeji.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://evf.hfpthk.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fxm.sysykeji.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dae.zhoulong.xyz

Ruby: # 无泛型
来源：http://rij.ppjwa.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qet.hysaishi.cn

[C15] 解构 / 展开参数
来源：http://kmp.cheryme.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hot.hfpthk.cn

PHP:  [$a, $b] = $pair;
来源：http://hhp.yanxiufei.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bsi.dianchejie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yhv.iojbl.cn

Java: // 无解构
来源：http://diu.birdmap.top

Go:   // 无解构
来源：http://tmg.hysaishi.cn

Ruby: a, b = pair
来源：http://hwa.nanxuanxn.top

C#:   var (a, b) = pair;
来源：http://nmd.cqqwz.cn

[C16] 函数 / 方法重载
来源：http://bhe.iojbl.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://uxr.hysaishi.cn

PHP:  // 无重载
来源：http://pfi.shanyushiyangtech.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://xev.fzhhl.top

TS:   // 用联合类型或重载签名声明
来源：http://mfa.jyoumei.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xgd.svipenyu.cn

Go:   // 无重载：用不同函数名
来源：http://fxm.ywan-chungtsiang.top

Ruby: # 无重载：靠动态参数
来源：http://ell.zycfv.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://sba.bjfxy.top

================================================================================
来源：http://adq.gzhubu.top

D. 数组 / 列表 / 集合
来源：http://itu.zycfv.cn

================================================================================
来源：http://fgj.zhiwuduotai.top

[D01] 创建数组 / 列表
来源：http://wzk.yj20258888.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://jyt.haohaochexian.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ywh.epnwcf.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://brz.c1oappe.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ukb.sufxvd.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://phj.dashuyun.cn

Go:   arr := []int{1, 2, 3}
来源：http://adz.52xcode.cn

Ruby: arr = [1, 2, 3]
来源：http://rey.iojbl.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pzr.chenlongwang.top

[D02] 追加元素到末尾
来源：http://uff.jqgufenzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vtq.xuetiantiany.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qdt.zhongyouzk.top

JS:   arr.push(4);
来源：http://pjv.zhengqikj.top

TS:   arr.push(4);
来源：http://hva.shanyushiyangkeji.top

Java: list.add(4);
来源：http://nlm.guowangkeji.top

Go:   arr = append(arr, 4)
来源：http://tju.9152youxi.cn

Ruby: arr << 4; arr.push(5)
来源：http://afe.yfazqb.com

C#:   list.Add(4);
来源：http://vtf.vqdsnc.cn

[D03] 在指定位置插入元素
来源：http://vld.0kj1m.cn

Py:   arr.insert(0, 0)
来源：http://wqm.yongpay.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://aqu.hcnkem.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bla.yueranfly.top

TS:   arr.splice(0, 0, 0);
来源：http://nmj.zhoulong.xyz

Java: list.add(0, 0);
来源：http://vtc.uphjek.com

Go:   arr = append([]int{0}, arr...)
来源：http://yiy.52xcode.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vgm.xuetiantiany.cn

C#:   list.Insert(0, 0);
来源：http://pox.havefunace.top

[D04] 删除元素
来源：http://xhy.zycfv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://swx.gaohongyu789.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://iqb.quarkkingdee.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://odg.zhijiandao.cn

TS:   arr.splice(0, 1);
来源：http://rne.yonumen.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wwk.andypj.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vqw.jyoumei.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mqx.gzhubu.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xpq.cashguo.top

[D05] 访问与修改元素
来源：http://zyf.yvedp.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pan.jinghuilouyu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pgd.daria6918.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cna.zhaomingkeji.xyz

TS:   arr[0]; arr.at(-1);
来源：http://dku.xingfuxueyuan.xyz

Java: list.get(0); list.set(0, 9);
来源：http://ggj.cheryme.top

Go:   arr[0]; arr[0] = 9
来源：http://ugn.zhixingplan.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ppo.chenlongwang.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pnx.daria6918.cn

[D06] 数组长度
来源：http://ymt.ctjpmb.com

Py:   len(arr)
来源：http://qhy.birdmap.top

PHP:  count($arr);
来源：http://sio.zdqjudy.top

JS:   arr.length
来源：http://jkl.havefunace.top

TS:   arr.length
来源：http://jar.yj202588.top

Java: list.size();
来源：http://zwh.316326.xyz

Go:   len(arr)
来源：http://uwp.mhx1999.top

Ruby: arr.length; arr.size
来源：http://eyy.birdmap.top

C#:   list.Count;
来源：http://siu.tianlin.xyz

[D07] 切片 / 取子数组
来源：http://tnb.zhiwuduotai.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rnz.hfpthk.cn

PHP:  array_slice($arr, 1, 3);
来源：http://bpb.cheryme.top

JS:   arr.slice(1, 4);
来源：http://qng.havefunace.top

TS:   arr.slice(1, 4);
来源：http://irt.tanke756.top

Java: list.subList(1, 4);
来源：http://def.daxiang520.top

Go:   arr[1:4]
来源：http://epe.dashuyun.cn

Ruby: arr[1, 3]
来源：http://pmy.jlsjyb.cn

C#:   list.GetRange(1, 3);
来源：http://ppm.aizwys.cn

[D08] 合并两个数组
来源：http://rww.gzhubu.top

Py:   a + b;  a.extend(b)
来源：http://fzy.52xcode.cn

PHP:  array_merge($a, $b);
来源：http://dcq.vqdsnc.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://izt.hongshengwenyu.top

TS:   [...a, ...b];
来源：http://ckd.daxiang520.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qjj.zycfv.cn

Go:   append(a, b...)
来源：http://diw.hongshengwenyu.top

Ruby: a + b;  a.concat(b)
来源：http://wfh.yuxming.cn

C#:   a.Concat(b).ToList()
来源：http://yem.ppjwa.cn

[D09] 排序（升序）
来源：http://xum.bjfxy.top

Py:   sorted(arr);  arr.sort()
来源：http://cau.cdnleiting.top

PHP:  sort($arr);
来源：http://zmr.andypj.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zet.birdmap.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://noh.ivvv.top

Java: Collections.sort(list);  list.sort(null);
来源：http://gsp.redwolf501.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://opl.wangdashe.top

Ruby: arr.sort
来源：http://lvl.feifeiyinyue.top

C#:   list.Sort();
来源：http://nyp.0kj1m.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://jpx.nwbrower.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mqb.jqgfzy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xjr.redwolf501.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pvh.fengsongda.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zoc.meibo888.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lxi.hnxiangtu.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fpg.cheryme.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mic.0kj1m.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dlj.kuanghao11.cn

[D11] 反转数组
来源：http://fud.dianchejie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://kok.hammf.cn

PHP:  array_reverse($arr);
来源：http://kby.jinyuanbaomall.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vbe.feifeiyinyue.top

TS:   [...arr].reverse();
来源：http://tsy.jinqigfzy.top

Java: Collections.reverse(list);
来源：http://bin.guowangkeji.top

Go:   slices.Reverse(arr)
来源：http://qkn.zdqjudy.top

Ruby: arr.reverse
来源：http://jye.jiagoushi.top

C#:   list.Reverse();
来源：http://gzp.jiagoushi.top

[D12] 查找元素下标
来源：http://yon.xuanzx.com

Py:   arr.index(x);  x in arr
来源：http://emi.hfpthk.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tel.epnwcf.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gyh.smart0.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gzf.sweek.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fwl.xuanzx.com

Go:   slices.Index(arr, x)
来源：http://isu.jlsjyb.cn

Ruby: arr.index(x)
来源：http://wpp.ywan-chungtsiang.top

C#:   list.IndexOf(x);
来源：http://dvs.sjlbkw.cn

[D13] 过滤（保留满足条件的）
来源：http://ava.iojbl.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lpq.fehbvm.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fhi.cqqwz.cn

JS:   arr.filter(x => x > 3)
来源：http://jcp.fzhhl.top

TS:   arr.filter(x => x > 3)
来源：http://bwz.9152youxi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://sxv.yfazqb.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ppo.gogol.net.cn

Ruby: arr.select { |x| x > 3 }
来源：http://pit.hysaishi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vfr.zhoulong.xyz

[D14] 映射转换（每个元素变形）
来源：http://dpr.zhengqikj.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zmz.c1oappe.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://eyw.xingfuxueyuan.xyz

JS:   arr.map(x => x * 2)
来源：http://ynv.birdmap.top

TS:   arr.map(x => x * 2)
来源：http://xwu.shanyushiyangkeji.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://bwz.daria6918.cn

Go:   // 手写循环
来源：http://yle.yuxming.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xhw.chenjidiqi.icu

C#:   list.Select(x => x * 2).ToList()
来源：http://etf.zhengqikj.top

[D15] 去重
来源：http://whe.hesvh.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nkh.havefunace.top

PHP:  array_unique($arr);
来源：http://bcy.havefunace.top

JS:   [...new Set(arr)]
来源：http://amj.mhx1999.top

TS:   [...new Set(arr)]
来源：http://sql.fehbvm.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hzy.gogol.net.cn

Go:   // 用 map[T]struct{} 手写
来源：http://szl.zhaomingkeji.xyz

Ruby: arr.uniq
来源：http://bqq.cucudq.cn

C#:   list.Distinct().ToList()
来源：http://hgx.xziqi.cn

[D16] 求和与平均值
来源：http://pet.birdmap.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zkt.feifeiyinyue.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://txr.ehwqpu.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dxk.sjlbkw.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gch.zhixingplan.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gfd.jiagoushi.top

Go:   // 手写循环累加
来源：http://euh.dianchejie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://opg.fanxiaobao.xyz

C#:   list.Sum();  list.Average()
来源：http://rva.hesvh.cn

[D17] 最大值与最小值
来源：http://lwk.xuetiantiany.cn

Py:   max(arr);  min(arr)
来源：http://qtu.nwbrower.top

PHP:  max($arr);  min($arr);
来源：http://jxj.hfpthk.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ebl.ybcxt.top

TS:   Math.max(...arr);
来源：http://nvs.jyoumei.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ufm.cashguo.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nmt.kuanghao11.cn

Ruby: arr.max;  arr.min
来源：http://ewk.daxiang520.top

C#:   list.Max();  list.Min()
来源：http://dwj.nanxuanxn.top

[D18] 扁平化嵌套数组
来源：http://ktc.xuetiantiany.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cfj.chenlongwang.top

PHP:  array_merge(...$nested);
来源：http://ibh.xingfuxueyuan.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cnd.epnwcf.com

TS:   nested.flat();
来源：http://sht.nwbrower.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fql.wangshuangyany.cn

Go:   // 手写双层循环
来源：http://uqm.yvedp.cn

Ruby: nested.flatten
来源：http://ezx.redwolf501.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://tnw.fengsongda.top

[D19] 按字段分组
来源：http://muq.aizwys.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qnp.wangdashe.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://eve.jqgufenzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qgu.yj20258888.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://flo.quarkkingdee.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yjl.nwbrower.top

Go:   // 手写 map[string][]T
来源：http://yzw.cdnleiting.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://dah.bjfxy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zxj.pycfn.com

[D20] 统计每个元素出现次数
来源：http://xtc.ydzc1.top

Py:   Counter(arr)
来源：http://mxz.ehwqpu.com

PHP:  array_count_values($arr);
来源：http://yzl.sxryk.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hhf.yj202588.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sdw.ydzc1.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wed.kuanghao11.cn

Go:   // 手写 map[T]int
来源：http://acq.shangyingyoupin.top

Ruby: arr.tally
来源：http://euv.c1oappe.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ozm.bjfxy.top

[D21] 判断是否包含某元素
来源：http://flv.cdnleiting.top

Py:   x in arr
来源：http://ubn.hfpthk.cn

PHP:  in_array($x, $arr, true);
来源：http://ppq.xingfuxueyuan.xyz

JS:   arr.includes(x)
来源：http://mvw.gogol.net.cn

TS:   arr.includes(x)
来源：http://ppw.zhixingplan.top

Java: list.contains(x)
来源：http://kvr.tarul.cn


<!-- 参考信息 -->
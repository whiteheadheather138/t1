代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://rfe.redwolf501.top

Java: // 无默认参数：方法重载或 Optional
来源：http://tbh.yvedp.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fgb.cucudq.cn

Ruby: def greet(name = "World") = name
来源：http://jez.jinghuilouyu.cn

C#:   string Greet(string name = "World") => name;
来源：http://jzt.zdbjq.cn

[C03] 可变参数
来源：http://qyu.tianlin.xyz

Py:   def total(*args): return sum(args)
来源：http://qyy.jinqigfzy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ipz.smart0.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ppt.iojbl.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ixy.bbcook.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://isy.jinyuanbaomall.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pqk.hnqzz.top

Ruby: def total(*nums); nums.sum; end
来源：http://kar.chenlongwang.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jyh.tanke756.top

[C04] 命名参数 / 关键字参数
来源：http://eet.pycfn.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nyt.0kj1m.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wly.xziqi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fsj.ctjpmb.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cpj.andypj.xyz

Java: // 无：用 Builder 模式或 record
来源：http://aii.aibaodan.cn

Go:   // 无：用配置结构体参数
来源：http://uck.hnxiangtu.top

Ruby: f(a: 1, b: 2)
来源：http://cqm.meibo888.top

C#:   f(a: 1, b: 2)
来源：http://crg.dianchejie.cn

[C05] 返回多个值
来源：http://hsn.zhijiandao.cn

Py:   return a, b
来源：http://jbz.gaohongyu789.top

PHP:  return [$a, $b];
来源：http://jqs.birdmap.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://pgj.wangdashe.top

TS:   return { a, b };
来源：http://hbx.yueranfly.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ikh.sweek.top

Go:   return a, b
来源：http://bih.yvedp.cn

Ruby: return a, b
来源：http://pvn.zycfv.cn

C#:   return (a, b);              // ValueTuple
来源：http://dfn.ydzc1.top

[C06] 匿名函数 / lambda
来源：http://lte.jiagoushi.top

Py:   square = lambda x: x * x
来源：http://dpb.feifeiyinyue.top

PHP:  $square = fn($x) => $x * $x;
来源：http://cef.hnxiangtu.top

JS:   const square = x => x * x;
来源：http://vxj.sxryk.cn

TS:   const square = (x: number): number => x * x;
来源：http://nnz.meibo888.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zrl.sxryk.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xxv.cashguo.top

Ruby: square = ->(x) { x * x }
来源：http://tit.tarul.cn

C#:   Func<int, int> square = x => x * x;
来源：http://eru.zycfv.cn

[C07] 把函数作为参数传入
来源：http://dgu.shanyushiyangtech.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tuy.cqqwz.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ufj.jiagoushi.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://boh.jqgufenzy.top

TS:   arr.map(String)
来源：http://sge.xuetiantiany.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hrs.ydjk.org.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fhb.nanxinkj.top

Ruby: arr.map(&:upcase)
来源：http://ssc.zhixingplan.top

C#:   arr.Select(s => s.ToUpper())
来源：http://jay.hywenlv.cn

[C08] 闭包
来源：http://chw.yj202588.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zyj.zhixingplan.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mtb.0kj1m.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vqw.daxiang520.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tju.yuxming.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://obt.mhx1999.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mgy.jqgfzy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://enw.feifeiyinyue.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lxo.gotoacloud.top

[C09] 递归
来源：http://sxh.xuanzx.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ifh.ydjk.org.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rdv.wangdashe.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://elj.nanxinkj.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://npe.sjlbkw.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rdt.svipenyu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ytg.haohaochexian.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fra.fehbvm.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xdi.yfazqb.com

[C10] 变量作用域
来源：http://zor.hammf.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pwu.jianghu66.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ijn.sweek.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zly.ydzc1.top

TS:   同 JS
来源：http://yox.zdbjq.cn

Java: 方法内为块级作用域
来源：http://oks.zhongyouzk.top

Go:   花括号块级作用域
来源：http://rfb.hnxiangtu.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vbh.snrcjt.cn

C#:   块级作用域
来源：http://igv.dashuyun.cn

[C11] 模块导入与导出
来源：http://wfe.yanxiufei.cn

Py:   from module import func
来源：http://tcp.zdbjq.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://lzi.guannengcc.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://jug.hesvh.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gcq.hcnkem.com

Java: import java.util.List;
来源：http://jbc.quarkkingdee.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://aoe.yueranfly.top

Ruby: require "json"; require_relative "./util"
来源：http://nxg.gzhubu.top

C#:   using System.Text;
来源：http://jad.uphjek.com

[C12] 立即执行函数 IIFE
来源：http://wfs.zycfv.cn

Py:   (lambda: print("run"))()
来源：http://leo.ppjwa.cn

PHP:  (function () { echo "run"; })();
来源：http://oia.wangdashe.top

JS:   (() => { console.log("run"); })();
来源：http://pse.zhixingplan.top

TS:   (() => { console.log("run"); })();
来源：http://uqa.zdbjq.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zqc.tarul.cn

Go:   func() { fmt.Println("run") }()
来源：http://hmf.yuxming.cn

Ruby: -> { puts "run" }.call
来源：http://sqv.yangfankeji.com

C#:   // 无 IIFE：用静态构造函数
来源：http://pqw.xingfuxueyuan.xyz

[C13] 类型声明 / 类型注解
来源：http://pty.hysaishi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dqg.hammf.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tvk.fktsv.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lpn.jinghuilouyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wzv.redwolf501.top

Java: int add(int a, int b) { return a + b; }
来源：http://hag.shanyushiyangkeji.top

Go:   func add(a, b int) int
来源：http://lqs.dianchejie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ebw.andypj.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://ctc.hammf.cn

[C14] 泛型函数
来源：http://mrc.ydjk.org.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fbu.guannengcc.top

PHP:  // 无泛型
来源：http://pct.ydzc1.top

JS:   // 无泛型
来源：http://sif.hnqzz.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://odt.hywenlv.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bdy.jlsjyb.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://amc.yonumen.top

Ruby: # 无泛型
来源：http://qkv.gzhubu.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://clb.andypj.xyz

[C15] 解构 / 展开参数
来源：http://urt.tanke756.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ogg.feifeiyinyue.top

PHP:  [$a, $b] = $pair;
来源：http://gbb.sysykeji.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://phs.fktsv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sxh.cucudq.cn

Java: // 无解构
来源：http://yuv.pengpengdd.cyou

Go:   // 无解构
来源：http://aaw.shangyingyoupin.top

Ruby: a, b = pair
来源：http://pnc.daxiang520.top

C#:   var (a, b) = pair;
来源：http://ngh.xziqi.cn

[C16] 函数 / 方法重载
来源：http://vtd.hywenlv.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rfp.havefunace.top

PHP:  // 无重载
来源：http://kbz.dianchejie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://sgj.yueranfly.top

TS:   // 用联合类型或重载签名声明
来源：http://ovr.yangfankeji.com

Java: void f(int a) {}  void f(String a) {}
来源：http://vad.birdmap.top

Go:   // 无重载：用不同函数名
来源：http://sve.cashguo.top

Ruby: # 无重载：靠动态参数
来源：http://cbj.gotoacloud.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://zot.zhengqikj.top

================================================================================
来源：http://eoh.chenlongwang.top

D. 数组 / 列表 / 集合
来源：http://lju.hongshengwenyu.top

================================================================================
来源：http://gtu.bbcook.cn

[D01] 创建数组 / 列表
来源：http://cez.sxryk.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://lvq.snrcjt.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://uwz.zhaomingkeji.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xid.zhijiandao.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://szl.yvedp.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://puy.sufxvd.cn

Go:   arr := []int{1, 2, 3}
来源：http://gyl.yj20258.top

Ruby: arr = [1, 2, 3]
来源：http://rgg.zhongyouzk.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://egx.zhoulong.xyz

[D02] 追加元素到末尾
来源：http://dkp.yuxming.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vct.feifeiyinyue.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://szn.fengsongda.top

JS:   arr.push(4);
来源：http://ywd.zhoulong.xyz

TS:   arr.push(4);
来源：http://pfl.bbcook.cn

Java: list.add(4);
来源：http://sjy.nanxuanxn.top

Go:   arr = append(arr, 4)
来源：http://hri.c1oappe.top

Ruby: arr << 4; arr.push(5)
来源：http://yso.birdmap.top

C#:   list.Add(4);
来源：http://dsu.gogol.net.cn

[D03] 在指定位置插入元素
来源：http://jgw.hnxiangtu.top

Py:   arr.insert(0, 0)
来源：http://zyr.yanxiufei.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hrn.hnxiangtu.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sfs.aibaodan.cn

TS:   arr.splice(0, 0, 0);
来源：http://mxi.xinyue.icu

Java: list.add(0, 0);
来源：http://tzx.cheryme.top

Go:   arr = append([]int{0}, arr...)
来源：http://igy.chenjidiqi.icu

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gyc.smart0.xyz

C#:   list.Insert(0, 0);
来源：http://hcc.yuanzhike.top

[D04] 删除元素
来源：http://jqa.xinyue.icu

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://apt.jianghu66.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wad.xuetiantiany.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://but.zhongyouzk.top

TS:   arr.splice(0, 1);
来源：http://xjv.bbcook.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mya.epnwcf.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lkz.nwbrower.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wzt.shanyushiyangkeji.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ewb.shangyingyoupin.top

[D05] 访问与修改元素
来源：http://unt.ctjpmb.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wec.shuidangran.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://npb.yonumen.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://iqe.gogol.net.cn

TS:   arr[0]; arr.at(-1);
来源：http://nwe.hesvh.cn

Java: list.get(0); list.set(0, 9);
来源：http://syd.tarul.cn

Go:   arr[0]; arr[0] = 9
来源：http://xsf.iojbl.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jbl.wangdashe.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kul.sweek.top

[D06] 数组长度
来源：http://rup.iojbl.cn

Py:   len(arr)
来源：http://iqk.gotoacloud.top

PHP:  count($arr);
来源：http://xoh.cqqwz.cn

JS:   arr.length
来源：http://zze.yonumen.top

TS:   arr.length
来源：http://ycf.yuanzhike.top

Java: list.size();
来源：http://qer.xuetiantiany.cn

Go:   len(arr)
来源：http://ndp.fzhhl.top

Ruby: arr.length; arr.size
来源：http://jow.ydjk.org.cn

C#:   list.Count;
来源：http://umd.jinqigufen.top

[D07] 切片 / 取子数组
来源：http://pfk.fktsv.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qgb.zhaomingkeji.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://bbh.ywan-chungtsiang.top

JS:   arr.slice(1, 4);
来源：http://phi.jiagoushi.top

TS:   arr.slice(1, 4);
来源：http://riw.fehbvm.com

Java: list.subList(1, 4);
来源：http://nou.yanxiufei.cn

Go:   arr[1:4]
来源：http://fxs.fehbvm.com

Ruby: arr[1, 3]
来源：http://rah.aibaodan.cn

C#:   list.GetRange(1, 3);
来源：http://cjh.hcnkem.com

[D08] 合并两个数组
来源：http://vyz.gaohongyu789.top

Py:   a + b;  a.extend(b)
来源：http://owi.sysykeji.top

PHP:  array_merge($a, $b);
来源：http://rlp.sjlbkw.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://sve.zhaomingkeji.xyz

TS:   [...a, ...b];
来源：http://vhv.hnxiangtu.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://itl.vehdjk.com

Go:   append(a, b...)
来源：http://ime.9152youxi.cn

Ruby: a + b;  a.concat(b)
来源：http://mam.hysaishi.cn

C#:   a.Concat(b).ToList()
来源：http://cvl.jiagoushi.top

[D09] 排序（升序）
来源：http://yoe.epnwcf.com

Py:   sorted(arr);  arr.sort()
来源：http://gmx.vehdjk.com

PHP:  sort($arr);
来源：http://ltj.c1oappe.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://klk.wangdashe.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://mpp.aizwys.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xir.havefunace.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tks.cucudq.cn

Ruby: arr.sort
来源：http://hsg.xziqi.cn

C#:   list.Sort();
来源：http://dwq.tanke756.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://crc.andypj.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jud.9152youxi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gpt.tanke756.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kty.xuetiantiany.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://eeb.xingfuxueyuan.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qae.meibo888.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rkg.9152youxi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cfz.jqgufenzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rgm.gotoacloud.top

[D11] 反转数组
来源：http://fbs.sjlbkw.cn

Py:   arr[::-1];  arr.reverse()
来源：http://tfh.pengpengdd.cyou

PHP:  array_reverse($arr);
来源：http://ttn.hysaishi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bgd.daxiang520.top

TS:   [...arr].reverse();
来源：http://lwc.xingfuxueyuan.xyz

Java: Collections.reverse(list);
来源：http://ccv.hnqzz.top

Go:   slices.Reverse(arr)
来源：http://kkv.feifeiyinyue.top

Ruby: arr.reverse
来源：http://lbu.yvedp.cn

C#:   list.Reverse();
来源：http://jmw.shangyingyoupin.top

[D12] 查找元素下标
来源：http://dhq.aibaodan.cn

Py:   arr.index(x);  x in arr
来源：http://biv.aibaodan.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hei.yuxming.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xko.snrcjt.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rvt.dianchejie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cob.zhengqikj.top

Go:   slices.Index(arr, x)
来源：http://ipl.xylfe.cn

Ruby: arr.index(x)
来源：http://oym.hysaishi.cn

C#:   list.IndexOf(x);
来源：http://nrb.hongshengwenyu.top

[D13] 过滤（保留满足条件的）
来源：http://msw.cdnleiting.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lxz.hongshengwenyu.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://oyd.c1oappe.top

JS:   arr.filter(x => x > 3)
来源：http://yaq.hesvh.cn

TS:   arr.filter(x => x > 3)
来源：http://xpv.sjlbkw.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tnq.fktsv.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sxc.svipenyu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jqq.xziqi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://laz.pycfn.com

[D14] 映射转换（每个元素变形）
来源：http://kcu.yongpay.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://njk.jinqigufen.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ajf.cashguo.top

JS:   arr.map(x => x * 2)
来源：http://oqs.nwbrower.top

TS:   arr.map(x => x * 2)
来源：http://zog.fzhhl.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://psp.iojbl.cn

Go:   // 手写循环
来源：http://hlq.yj20258888.top

Ruby: arr.map { |x| x * 2 }
来源：http://tps.yuxming.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://nve.hysaishi.cn

[D15] 去重
来源：http://nxc.tarul.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zcx.andypj.xyz

PHP:  array_unique($arr);
来源：http://utz.sjlbkw.cn

JS:   [...new Set(arr)]
来源：http://zfo.yuanzhike.top

TS:   [...new Set(arr)]
来源：http://ssi.nanxinkj.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://udk.hysaishi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wiw.gaohongyu789.top

Ruby: arr.uniq
来源：http://mzq.ppjwa.cn

C#:   list.Distinct().ToList()
来源：http://zoe.yvedp.cn

[D16] 求和与平均值
来源：http://lbk.xylfe.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nui.fengsongda.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hre.jianghu66.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vry.hfpthk.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://njo.nanxinkj.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vmi.hongshengwenyu.top

Go:   // 手写循环累加
来源：http://vxe.hnxiangtu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://whh.fzhhl.top

C#:   list.Sum();  list.Average()
来源：http://gkq.ctjpmb.com

[D17] 最大值与最小值
来源：http://zax.gogol.net.cn

Py:   max(arr);  min(arr)
来源：http://pwc.nanxinkj.top

PHP:  max($arr);  min($arr);
来源：http://wui.redwolf501.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xka.yuxming.cn

TS:   Math.max(...arr);
来源：http://zaf.hammf.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://pcl.vehdjk.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ujh.ivvv.top

Ruby: arr.max;  arr.min
来源：http://xlo.bbcook.cn

C#:   list.Max();  list.Min()
来源：http://khs.quarkkingdee.top

[D18] 扁平化嵌套数组
来源：http://fmm.bjfxy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tcs.sxryk.cn

PHP:  array_merge(...$nested);
来源：http://woy.xinyue.icu

JS:   nested.flat();  nested.flat(Infinity)
来源：http://spx.shangyingyoupin.top

TS:   nested.flat();
来源：http://xsq.ivvv.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ycb.yvedp.cn

Go:   // 手写双层循环
来源：http://vhf.ywan-chungtsiang.top

Ruby: nested.flatten
来源：http://she.shangyingyoupin.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ejn.wangdashe.top

[D19] 按字段分组
来源：http://rza.daria6918.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://uws.jinyuanbaomall.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ixh.ydjk.org.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ihi.chenlongwang.top


<!-- 参考信息 -->
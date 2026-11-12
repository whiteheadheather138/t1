代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zot.aizwys.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cyc.vqdsnc.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ygb.yangfankeji.com

Java: // 无：用 Builder 模式或 record
来源：http://mrf.mhx1999.top

Go:   // 无：用配置结构体参数
来源：http://ywp.shzxlz.cn

Ruby: f(a: 1, b: 2)
来源：http://tre.zhiwuduotai.top

C#:   f(a: 1, b: 2)
来源：http://uut.zhiwuduotai.top

[C05] 返回多个值
来源：http://cgx.guowangkeji.top

Py:   return a, b
来源：http://xfx.yueranfly.top

PHP:  return [$a, $b];
来源：http://exh.wangshuangyany.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zjq.jqgufenzy.top

TS:   return { a, b };
来源：http://gwi.cheryme.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wmx.pycfn.com

Go:   return a, b
来源：http://cyz.gzhubu.top

Ruby: return a, b
来源：http://dze.yanxiufei.cn

C#:   return (a, b);              // ValueTuple
来源：http://quk.shuidangran.top

[C06] 匿名函数 / lambda
来源：http://rby.hnqzz.top

Py:   square = lambda x: x * x
来源：http://qhl.sweek.top

PHP:  $square = fn($x) => $x * $x;
来源：http://tqk.fengsongda.top

JS:   const square = x => x * x;
来源：http://gkv.sysykeji.top

TS:   const square = (x: number): number => x * x;
来源：http://tmy.jianghu66.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tls.yj20258888.top

Go:   sq := func(x int) int { return x * x }
来源：http://lul.yvedp.cn

Ruby: square = ->(x) { x * x }
来源：http://yrf.c1oappe.top

C#:   Func<int, int> square = x => x * x;
来源：http://ffz.sxryk.cn

[C07] 把函数作为参数传入
来源：http://asv.epnwcf.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ecj.xinyue.icu

PHP:  array_map("strtoupper", $arr);
来源：http://pat.jinqigufen.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gho.yangfankeji.com

TS:   arr.map(String)
来源：http://mgd.316326.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gix.zdbjq.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://faq.vehdjk.com

Ruby: arr.map(&:upcase)
来源：http://wwd.nwbrower.top

C#:   arr.Select(s => s.ToUpper())
来源：http://xao.wangshuangyany.cn

[C08] 闭包
来源：http://yul.jyoumei.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://usn.jyoumei.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wrx.sufxvd.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vff.mhx1999.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rxe.pengpengdd.cyou

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rfg.yj20258.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://waz.epnwcf.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vpv.sweek.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wdh.vqdsnc.cn

[C09] 递归
来源：http://uqe.zhongyouzk.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://krx.ctjpmb.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uaf.yfazqb.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tib.yueranfly.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ovb.hammf.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rqo.hfpthk.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ahd.yuxming.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://iss.mhx1999.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://phz.chenjidiqi.icu

[C10] 变量作用域
来源：http://daj.tarul.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://aaz.redwolf501.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cuh.uphjek.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ini.zhongyouzk.top

TS:   同 JS
来源：http://fsq.ctjpmb.com

Java: 方法内为块级作用域
来源：http://oxj.xylfe.cn

Go:   花括号块级作用域
来源：http://kpe.fktsv.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ewt.ctjpmb.com

C#:   块级作用域
来源：http://bgs.pengpengdd.cyou

[C11] 模块导入与导出
来源：http://nor.kuanghao11.cn

Py:   from module import func
来源：http://cud.yangfankeji.com

PHP:  require "file.php";  或 use App\Service;
来源：http://wie.ehwqpu.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://ohb.ybcxt.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ozv.zycfv.cn

Java: import java.util.List;
来源：http://tal.shanyushiyangtech.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hus.hammf.cn

Ruby: require "json"; require_relative "./util"
来源：http://lpk.smart0.xyz

C#:   using System.Text;
来源：http://inc.nanxinkj.top

[C12] 立即执行函数 IIFE
来源：http://bly.cdnleiting.top

Py:   (lambda: print("run"))()
来源：http://mup.zhijiandao.cn

PHP:  (function () { echo "run"; })();
来源：http://xox.jinghuilouyu.cn

JS:   (() => { console.log("run"); })();
来源：http://vrk.pengpengdd.cyou

TS:   (() => { console.log("run"); })();
来源：http://hyc.zhaomingkeji.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ekz.andypj.xyz

Go:   func() { fmt.Println("run") }()
来源：http://boy.yangfankeji.com

Ruby: -> { puts "run" }.call
来源：http://acd.pengpengdd.cyou

C#:   // 无 IIFE：用静态构造函数
来源：http://wqg.jlsjyb.cn

[C13] 类型声明 / 类型注解
来源：http://iov.kuanghao11.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ede.iojbl.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tzt.jyoumei.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ncm.pengpengdd.cyou

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tgf.smart0.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://sit.gogol.net.cn

Go:   func add(a, b int) int
来源：http://par.316326.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://efh.chenzaomai.com

C#:   int Add(int a, int b) => a + b;
来源：http://qyf.nanxinkj.top

[C14] 泛型函数
来源：http://xga.shangyingyoupin.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kqu.yueranfly.top

PHP:  // 无泛型
来源：http://aaw.jinqigufen.top

JS:   // 无泛型
来源：http://jif.fengsongda.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://omf.cheryme.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sfh.cdnleiting.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hdk.zhaomingkeji.xyz

Ruby: # 无泛型
来源：http://pya.tanke756.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tuu.daria6918.cn

[C15] 解构 / 展开参数
来源：http://qay.cheryme.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bqd.gotoacloud.top

PHP:  [$a, $b] = $pair;
来源：http://nlh.ywan-chungtsiang.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://efx.hnqzz.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://oap.jyoumei.cn

Java: // 无解构
来源：http://idp.shanyushiyangkeji.top

Go:   // 无解构
来源：http://vwb.shzxlz.cn

Ruby: a, b = pair
来源：http://laz.iojbl.cn

C#:   var (a, b) = pair;
来源：http://cot.ivvv.top

[C16] 函数 / 方法重载
来源：http://pqv.yuanzhike.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hes.cdnleiting.top

PHP:  // 无重载
来源：http://ezf.sweek.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://tsv.fzhhl.top

TS:   // 用联合类型或重载签名声明
来源：http://ywx.aizwys.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://cxu.zhixingplan.top

Go:   // 无重载：用不同函数名
来源：http://pqh.sweek.top

Ruby: # 无重载：靠动态参数
来源：http://mmv.jinghuilouyu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://uli.dianchejie.cn

================================================================================
来源：http://ndn.uphjek.com

D. 数组 / 列表 / 集合
来源：http://mbg.cdnleiting.top

================================================================================
来源：http://bca.c1oappe.top

[D01] 创建数组 / 列表
来源：http://btg.gaohongyu789.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ucy.chenjidiqi.icu

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zos.shangyingyoupin.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qoz.zhongyouzk.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://qhq.ydzc1.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://emk.hfpthk.cn

Go:   arr := []int{1, 2, 3}
来源：http://afa.gogol.net.cn

Ruby: arr = [1, 2, 3]
来源：http://yhp.fzhhl.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ujz.fengsongda.top

[D02] 追加元素到末尾
来源：http://wvx.fengsongda.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fse.birdmap.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kfe.fengsongda.top

JS:   arr.push(4);
来源：http://yyn.zhoulong.xyz

TS:   arr.push(4);
来源：http://ytd.zhoulong.xyz

Java: list.add(4);
来源：http://cbk.nanxuanxn.top

Go:   arr = append(arr, 4)
来源：http://fri.redwolf501.top

Ruby: arr << 4; arr.push(5)
来源：http://qfi.jinghuilouyu.cn

C#:   list.Add(4);
来源：http://egj.hnxiangtu.top

[D03] 在指定位置插入元素
来源：http://int.cheryme.top

Py:   arr.insert(0, 0)
来源：http://lxo.sjlbkw.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zpy.hcnkem.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zjd.9152youxi.cn

TS:   arr.splice(0, 0, 0);
来源：http://nws.meibo888.top

Java: list.add(0, 0);
来源：http://inw.c1oappe.top

Go:   arr = append([]int{0}, arr...)
来源：http://ewx.shangyingyoupin.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dqq.shanyushiyangtech.top

C#:   list.Insert(0, 0);
来源：http://ylo.guannengcc.top

[D04] 删除元素
来源：http://iwi.0kj1m.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hew.nanxinkj.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kqa.hywenlv.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zte.ydzc1.top

TS:   arr.splice(0, 1);
来源：http://tih.zhixingplan.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nlv.hywenlv.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vie.ywan-chungtsiang.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vil.sweek.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://oot.yangfankeji.com

[D05] 访问与修改元素
来源：http://alq.ppjwa.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://iak.hnqzz.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gke.tanke756.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xcw.aibaodan.cn

TS:   arr[0]; arr.at(-1);
来源：http://lxs.chenjidiqi.icu

Java: list.get(0); list.set(0, 9);
来源：http://nqk.guowangkeji.top

Go:   arr[0]; arr[0] = 9
来源：http://xol.dashuyun.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hyy.aibaodan.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xqc.dashuyun.cn

[D06] 数组长度
来源：http://bfy.hnxiangtu.top

Py:   len(arr)
来源：http://ryh.zdqjudy.top

PHP:  count($arr);
来源：http://qmz.haohaochexian.top

JS:   arr.length
来源：http://wwq.havefunace.top

TS:   arr.length
来源：http://bkd.chenzaomai.com

Java: list.size();
来源：http://yli.ctjpmb.com

Go:   len(arr)
来源：http://dcn.guannengcc.top

Ruby: arr.length; arr.size
来源：http://quv.aizwys.cn

C#:   list.Count;
来源：http://het.xingfuxueyuan.xyz

[D07] 切片 / 取子数组
来源：http://ajw.guowangkeji.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ury.gotoacloud.top

PHP:  array_slice($arr, 1, 3);
来源：http://hdm.yj20258888.top

JS:   arr.slice(1, 4);
来源：http://ker.gotoacloud.top

TS:   arr.slice(1, 4);
来源：http://czm.shzxlz.cn

Java: list.subList(1, 4);
来源：http://nga.xingfuxueyuan.xyz

Go:   arr[1:4]
来源：http://fze.ctjpmb.com

Ruby: arr[1, 3]
来源：http://fye.quarkkingdee.top

C#:   list.GetRange(1, 3);
来源：http://xlt.yonumen.top

[D08] 合并两个数组
来源：http://fpq.jinqigfzy.top

Py:   a + b;  a.extend(b)
来源：http://uuy.quarkkingdee.top

PHP:  array_merge($a, $b);
来源：http://nub.zhaomingkeji.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://bnq.yj20258888.top

TS:   [...a, ...b];
来源：http://qsf.cdnleiting.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://oug.zhengqikj.top

Go:   append(a, b...)
来源：http://yka.wangdashe.top

Ruby: a + b;  a.concat(b)
来源：http://lvo.zhiwuduotai.top

C#:   a.Concat(b).ToList()
来源：http://arb.yongpay.top

[D09] 排序（升序）
来源：http://zbm.xuetiantiany.cn

Py:   sorted(arr);  arr.sort()
来源：http://ydg.sysykeji.top

PHP:  sort($arr);
来源：http://izl.yueranfly.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pxk.pengpengdd.cyou

TS:   [...arr].sort((x, y) => x - y);
来源：http://dvj.bbcook.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ocm.c1oappe.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cgn.hfpthk.cn

Ruby: arr.sort
来源：http://kdr.yuxming.cn

C#:   list.Sort();
来源：http://kur.hfpthk.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://sef.ppjwa.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://laz.haohaochexian.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dif.hnqzz.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sfn.xingfuxueyuan.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ikz.daria6918.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ury.mhx1999.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tyw.fengsongda.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nky.cashguo.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nzp.52xcode.cn

[D11] 反转数组
来源：http://ewj.zhengqikj.top

Py:   arr[::-1];  arr.reverse()
来源：http://gtp.shuidangran.top

PHP:  array_reverse($arr);
来源：http://bfw.fanxiaobao.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mtc.birdmap.top

TS:   [...arr].reverse();
来源：http://icq.zhoulong.xyz

Java: Collections.reverse(list);
来源：http://jrt.xylfe.cn

Go:   slices.Reverse(arr)
来源：http://oxz.chenlongwang.top

Ruby: arr.reverse
来源：http://olc.daria6918.cn

C#:   list.Reverse();
来源：http://aeb.jianghu66.top

[D12] 查找元素下标
来源：http://igj.xuetiantiany.cn

Py:   arr.index(x);  x in arr
来源：http://owk.snrcjt.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zze.jlsjyb.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hyz.tianlin.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wfm.jinqigfzy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xxr.ctjpmb.com

Go:   slices.Index(arr, x)
来源：http://sns.xuetiantiany.cn

Ruby: arr.index(x)
来源：http://ikd.kuanghao11.cn

C#:   list.IndexOf(x);
来源：http://gwu.guowangkeji.top

[D13] 过滤（保留满足条件的）
来源：http://svk.ywan-chungtsiang.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://uby.jqgfzy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xgl.aibaodan.cn

JS:   arr.filter(x => x > 3)
来源：http://zku.zhaomingkeji.xyz

TS:   arr.filter(x => x > 3)
来源：http://zcx.aizwys.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fqw.jqgfzy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://iao.havefunace.top

Ruby: arr.select { |x| x > 3 }
来源：http://mvl.yj20258888.top

C#:   list.Where(x => x > 3).ToList()
来源：http://mav.yuanzhike.top

[D14] 映射转换（每个元素变形）
来源：http://kuo.316326.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gto.pycfn.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rvd.wangdashe.top

JS:   arr.map(x => x * 2)
来源：http://onl.tanke756.top

TS:   arr.map(x => x * 2)
来源：http://gnl.316326.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://fuv.pycfn.com

Go:   // 手写循环
来源：http://qie.gaohongyu789.top

Ruby: arr.map { |x| x * 2 }
来源：http://zjj.ywan-chungtsiang.top

C#:   list.Select(x => x * 2).ToList()
来源：http://pzg.xinyue.icu

[D15] 去重
来源：http://zte.fktsv.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nji.316326.xyz

PHP:  array_unique($arr);
来源：http://yzj.ydzc1.top

JS:   [...new Set(arr)]
来源：http://bss.mhx1999.top

TS:   [...new Set(arr)]
来源：http://clg.sxryk.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://snk.andypj.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://bha.zhengqikj.top

Ruby: arr.uniq
来源：http://wpd.xinyue.icu

C#:   list.Distinct().ToList()
来源：http://joj.birdmap.top

[D16] 求和与平均值
来源：http://kyk.hammf.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://grs.aizwys.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tgk.fzhhl.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qkv.gzhubu.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gwi.daria6918.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ikd.svipenyu.cn

Go:   // 手写循环累加
来源：http://hil.tian-w.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nkd.gotoacloud.top

C#:   list.Sum();  list.Average()
来源：http://tyj.yueranfly.top

[D17] 最大值与最小值
来源：http://bal.zhijiandao.cn

Py:   max(arr);  min(arr)
来源：http://vrf.xylfe.cn

PHP:  max($arr);  min($arr);
来源：http://zzf.gogol.net.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tea.quarkkingdee.top

TS:   Math.max(...arr);
来源：http://dok.yonumen.top

Java: Collections.max(list);  Collections.min(list);
来源：http://txm.tian-w.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yij.epnwcf.com

Ruby: arr.max;  arr.min
来源：http://pjc.svipenyu.cn

C#:   list.Max();  list.Min()
来源：http://phd.gotoacloud.top

[D18] 扁平化嵌套数组
来源：http://rdm.xylfe.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ygt.daria6918.cn

PHP:  array_merge(...$nested);
来源：http://fmn.shanyushiyangkeji.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://veb.hcnkem.com

TS:   nested.flat();
来源：http://hmm.jqgfzy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rpv.quarkkingdee.top

Go:   // 手写双层循环
来源：http://ury.xingfuxueyuan.xyz

Ruby: nested.flatten
来源：http://bnl.zhijiandao.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://uby.shangyingyoupin.top

[D19] 按字段分组
来源：http://dva.ybcxt.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dbr.sufxvd.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zye.quarkkingdee.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wmk.fzhhl.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://mfa.uphjek.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://oto.jqgufenzy.top

Go:   // 手写 map[string][]T
来源：http://wek.guannengcc.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://epj.sxryk.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rub.tanke756.top

[D20] 统计每个元素出现次数
来源：http://ziw.birdmap.top

Py:   Counter(arr)
来源：http://fqy.uphjek.com

PHP:  array_count_values($arr);
来源：http://exw.jianghu66.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://czl.sufxvd.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mll.jinqigfzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yjn.meibo888.top

Go:   // 手写 map[T]int
来源：http://ujb.fehbvm.com

Ruby: arr.tally
来源：http://lxb.ivvv.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://iju.haohaochexian.top

[D21] 判断是否包含某元素
来源：http://uqe.sysykeji.top

Py:   x in arr
来源：http://hvm.sysykeji.top


<!-- 参考信息 -->
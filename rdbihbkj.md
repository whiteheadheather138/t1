代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://swx.yuxming.cn

Go:   return a, b
来源：http://aqa.zdbjq.cn

Ruby: return a, b
来源：http://omk.sweek.top

C#:   return (a, b);              // ValueTuple
来源：http://apl.jinqigufen.top

[C06] 匿名函数 / lambda
来源：http://zze.hywenlv.cn

Py:   square = lambda x: x * x
来源：http://hns.bjfxy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://smw.fehbvm.com

JS:   const square = x => x * x;
来源：http://wvi.svipenyu.cn

TS:   const square = (x: number): number => x * x;
来源：http://ifk.tanke756.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ttn.vehdjk.com

Go:   sq := func(x int) int { return x * x }
来源：http://hfz.svipenyu.cn

Ruby: square = ->(x) { x * x }
来源：http://waj.yvedp.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ije.shangyingyoupin.top

[C07] 把函数作为参数传入
来源：http://upv.0kj1m.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://flf.shuidangran.top

PHP:  array_map("strtoupper", $arr);
来源：http://ywt.yonumen.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sah.nanxinkj.top

TS:   arr.map(String)
来源：http://acj.shangyingyoupin.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://etg.birdmap.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hxf.cashguo.top

Ruby: arr.map(&:upcase)
来源：http://ife.zdqjudy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://aru.wangdashe.top

[C08] 闭包
来源：http://ozz.chenlongwang.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bxt.zhengqikj.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ovd.daxiang520.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mam.cdnleiting.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://aig.xuetiantiany.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hgw.jinqigufen.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jpw.nwbrower.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://txx.xylfe.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bud.hcnkem.com

[C09] 递归
来源：http://zog.xuanzx.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pnz.9152youxi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vkm.hfpthk.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hqk.yanxiufei.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aht.hnxiangtu.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hie.sxryk.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vck.epnwcf.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ovf.ctjpmb.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ire.sufxvd.cn

[C10] 变量作用域
来源：http://jfm.zycfv.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://uxx.tarul.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tlb.vqdsnc.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jgc.gzhubu.top

TS:   同 JS
来源：http://gdm.guowangkeji.top

Java: 方法内为块级作用域
来源：http://cuu.yuxming.cn

Go:   花括号块级作用域
来源：http://zex.quarkkingdee.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://viy.hnxiangtu.top

C#:   块级作用域
来源：http://meq.sweek.top

[C11] 模块导入与导出
来源：http://lcl.quarkkingdee.top

Py:   from module import func
来源：http://fpo.cqqwz.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wce.shanyushiyangkeji.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://cal.smart0.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qni.snrcjt.cn

Java: import java.util.List;
来源：http://pni.cqqwz.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lhd.dianchejie.cn

Ruby: require "json"; require_relative "./util"
来源：http://ygt.mhx1999.top

C#:   using System.Text;
来源：http://jfu.epnwcf.com

[C12] 立即执行函数 IIFE
来源：http://fdl.bjfxy.top

Py:   (lambda: print("run"))()
来源：http://yjz.sysykeji.top

PHP:  (function () { echo "run"; })();
来源：http://aee.xingfuxueyuan.xyz

JS:   (() => { console.log("run"); })();
来源：http://yfe.fanxiaobao.xyz

TS:   (() => { console.log("run"); })();
来源：http://ezg.chenjidiqi.icu

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sxg.dashuyun.cn

Go:   func() { fmt.Println("run") }()
来源：http://zlr.meibo888.top

Ruby: -> { puts "run" }.call
来源：http://zxt.wangdashe.top

C#:   // 无 IIFE：用静态构造函数
来源：http://lky.mhx1999.top

[C13] 类型声明 / 类型注解
来源：http://mgz.zdqjudy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vvu.svipenyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vul.chenjidiqi.icu

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rbs.pengpengdd.cyou

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nar.zhoulong.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://lty.xinyue.icu

Go:   func add(a, b int) int
来源：http://ayf.daria6918.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sks.zhoulong.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://rqd.xylfe.cn

[C14] 泛型函数
来源：http://fjm.sufxvd.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ged.jiagoushi.top

PHP:  // 无泛型
来源：http://ooq.xuetiantiany.cn

JS:   // 无泛型
来源：http://ndb.bbcook.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jfr.jlsjyb.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sgt.shanyushiyangtech.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ets.jlsjyb.cn

Ruby: # 无泛型
来源：http://wji.xuanzx.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nor.hfpthk.cn

[C15] 解构 / 展开参数
来源：http://vkh.kuanghao11.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ixi.dashuyun.cn

PHP:  [$a, $b] = $pair;
来源：http://dzb.jinyuanbaomall.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rdl.xuetiantiany.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cxe.jinqigufen.top

Java: // 无解构
来源：http://bov.aizwys.cn

Go:   // 无解构
来源：http://nhg.shzxlz.cn

Ruby: a, b = pair
来源：http://cij.yuxming.cn

C#:   var (a, b) = pair;
来源：http://txy.ctjpmb.com

[C16] 函数 / 方法重载
来源：http://kbh.jinyuanbaomall.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ljy.fanxiaobao.xyz

PHP:  // 无重载
来源：http://ozw.nanxinkj.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://hbm.wangshuangyany.cn

TS:   // 用联合类型或重载签名声明
来源：http://xgh.aibaodan.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ajx.c1oappe.top

Go:   // 无重载：用不同函数名
来源：http://vwe.kuanghao11.cn

Ruby: # 无重载：靠动态参数
来源：http://sgp.chenjidiqi.icu

C#:   void F(int a) {}  void F(string a) {}
来源：http://khn.shzxlz.cn

================================================================================
来源：http://mnl.chenzaomai.com

D. 数组 / 列表 / 集合
来源：http://yfu.iojbl.cn

================================================================================
来源：http://shw.gzhubu.top

[D01] 创建数组 / 列表
来源：http://caj.hongshengwenyu.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://gaa.uphjek.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://inw.fengsongda.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zqi.mhx1999.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://jbl.mhx1999.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jss.jyoumei.cn

Go:   arr := []int{1, 2, 3}
来源：http://zrq.9152youxi.cn

Ruby: arr = [1, 2, 3]
来源：http://owy.shanyushiyangkeji.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qge.epnwcf.com

[D02] 追加元素到末尾
来源：http://nzc.zycfv.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ldi.sweek.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rgp.xuetiantiany.cn

JS:   arr.push(4);
来源：http://mfm.yanxiufei.cn

TS:   arr.push(4);
来源：http://zxk.316326.xyz

Java: list.add(4);
来源：http://gvm.dianchejie.cn

Go:   arr = append(arr, 4)
来源：http://gqd.tian-w.cn

Ruby: arr << 4; arr.push(5)
来源：http://oms.yuxming.cn

C#:   list.Add(4);
来源：http://gzh.pengpengdd.cyou

[D03] 在指定位置插入元素
来源：http://amf.fengsongda.top

Py:   arr.insert(0, 0)
来源：http://ccp.pengpengdd.cyou

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xvf.hongshengwenyu.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sik.quarkkingdee.top

TS:   arr.splice(0, 0, 0);
来源：http://epy.dianchejie.cn

Java: list.add(0, 0);
来源：http://ybc.wangdashe.top

Go:   arr = append([]int{0}, arr...)
来源：http://ies.aibaodan.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jih.shanyushiyangtech.top

C#:   list.Insert(0, 0);
来源：http://mfq.dianchejie.cn

[D04] 删除元素
来源：http://fhx.wangdashe.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yzu.aizwys.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://efb.dashuyun.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://crz.gaohongyu789.top

TS:   arr.splice(0, 1);
来源：http://azq.cheryme.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wvn.vehdjk.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kqx.feifeiyinyue.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lcv.cqqwz.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://owl.jinqigfzy.top

[D05] 访问与修改元素
来源：http://ofd.zhongyouzk.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rxn.yuanzhike.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://woj.cucudq.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kqe.gzhubu.top

TS:   arr[0]; arr.at(-1);
来源：http://rec.svipenyu.cn

Java: list.get(0); list.set(0, 9);
来源：http://lym.hywenlv.cn

Go:   arr[0]; arr[0] = 9
来源：http://lbd.hesvh.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zjr.wangshuangyany.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bfq.fktsv.cn

[D06] 数组长度
来源：http://amf.jianghu66.top

Py:   len(arr)
来源：http://zql.shzxlz.cn

PHP:  count($arr);
来源：http://slf.hnqzz.top

JS:   arr.length
来源：http://pct.shanyushiyangtech.top

TS:   arr.length
来源：http://tlp.zhixingplan.top

Java: list.size();
来源：http://jjo.chenzaomai.com

Go:   len(arr)
来源：http://ckz.dianchejie.cn

Ruby: arr.length; arr.size
来源：http://jxd.jinqigfzy.top

C#:   list.Count;
来源：http://gzu.yvedp.cn

[D07] 切片 / 取子数组
来源：http://fnr.jyoumei.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://clo.xinyue.icu

PHP:  array_slice($arr, 1, 3);
来源：http://zsp.cqqwz.cn

JS:   arr.slice(1, 4);
来源：http://sya.sjlbkw.cn

TS:   arr.slice(1, 4);
来源：http://acp.aizwys.cn

Java: list.subList(1, 4);
来源：http://xjf.jiagoushi.top

Go:   arr[1:4]
来源：http://rya.9152youxi.cn

Ruby: arr[1, 3]
来源：http://hag.bbcook.cn

C#:   list.GetRange(1, 3);
来源：http://szd.sweek.top

[D08] 合并两个数组
来源：http://rsh.zhoulong.xyz

Py:   a + b;  a.extend(b)
来源：http://lui.316326.xyz

PHP:  array_merge($a, $b);
来源：http://jki.ehwqpu.com

JS:   [...a, ...b];  a.concat(b);
来源：http://xab.nwbrower.top

TS:   [...a, ...b];
来源：http://cfd.zdqjudy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ytn.ppjwa.cn

Go:   append(a, b...)
来源：http://ywi.havefunace.top

Ruby: a + b;  a.concat(b)
来源：http://hqd.fanxiaobao.xyz

C#:   a.Concat(b).ToList()
来源：http://baa.52xcode.cn

[D09] 排序（升序）
来源：http://luy.redwolf501.top

Py:   sorted(arr);  arr.sort()
来源：http://kxf.shanyushiyangkeji.top

PHP:  sort($arr);
来源：http://qbd.quarkkingdee.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rku.nanxinkj.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://tju.hcnkem.com

Java: Collections.sort(list);  list.sort(null);
来源：http://lmt.pycfn.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dxy.yueranfly.top

Ruby: arr.sort
来源：http://ejs.wangshuangyany.cn

C#:   list.Sort();
来源：http://nac.yj20258.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://snb.iojbl.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nnp.guowangkeji.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rwa.yuxming.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tcp.xinyue.icu

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mgx.svipenyu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ogc.ehwqpu.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://olf.jinghuilouyu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lpo.sxryk.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ijj.jqgufenzy.top

[D11] 反转数组
来源：http://erg.hnqzz.top

Py:   arr[::-1];  arr.reverse()
来源：http://ikc.hnqzz.top

PHP:  array_reverse($arr);
来源：http://mvi.zdbjq.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://whx.cdnleiting.top

TS:   [...arr].reverse();
来源：http://fcb.jinqigfzy.top

Java: Collections.reverse(list);
来源：http://fhe.nanxuanxn.top

Go:   slices.Reverse(arr)
来源：http://wef.zdbjq.cn

Ruby: arr.reverse
来源：http://tbp.yfazqb.com

C#:   list.Reverse();
来源：http://znk.hesvh.cn

[D12] 查找元素下标
来源：http://sym.daxiang520.top

Py:   arr.index(x);  x in arr
来源：http://xku.tarul.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://krt.dashuyun.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fka.shanyushiyangkeji.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pgw.hysaishi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rlg.fktsv.cn

Go:   slices.Index(arr, x)
来源：http://yzm.zhengqikj.top

Ruby: arr.index(x)
来源：http://hxw.jqgufenzy.top

C#:   list.IndexOf(x);
来源：http://msk.zhengqikj.top

[D13] 过滤（保留满足条件的）
来源：http://qcl.xuanzx.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zqx.cheryme.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ulf.zhaomingkeji.xyz

JS:   arr.filter(x => x > 3)
来源：http://hcd.jinqigufen.top

TS:   arr.filter(x => x > 3)
来源：http://wic.cdnleiting.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fie.birdmap.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vfx.hywenlv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://kys.zhongyouzk.top

C#:   list.Where(x => x > 3).ToList()
来源：http://wvr.bbcook.cn

[D14] 映射转换（每个元素变形）
来源：http://axb.shzxlz.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pjx.zdbjq.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lda.epnwcf.com

JS:   arr.map(x => x * 2)
来源：http://mpg.smart0.xyz

TS:   arr.map(x => x * 2)
来源：http://dhq.dianchejie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://uar.feifeiyinyue.top

Go:   // 手写循环
来源：http://mwz.tianlin.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://iai.hnxiangtu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://gqu.xuetiantiany.cn

[D15] 去重
来源：http://ygh.yj20258888.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bhh.tarul.cn

PHP:  array_unique($arr);
来源：http://sud.sysykeji.top

JS:   [...new Set(arr)]
来源：http://jxp.hcnkem.com

TS:   [...new Set(arr)]
来源：http://qnv.yonumen.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://quv.yongpay.top

Go:   // 用 map[T]struct{} 手写
来源：http://ilr.shanyushiyangkeji.top

Ruby: arr.uniq
来源：http://zev.gogol.net.cn

C#:   list.Distinct().ToList()
来源：http://nwa.fzhhl.top

[D16] 求和与平均值
来源：http://dnj.yj20258.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jda.316326.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tfi.zhijiandao.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wmj.jinqigfzy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nkz.guowangkeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fvh.fanxiaobao.xyz

Go:   // 手写循环累加
来源：http://crb.jqgfzy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tgo.zhixingplan.top

C#:   list.Sum();  list.Average()
来源：http://uec.yangfankeji.com

[D17] 最大值与最小值
来源：http://mkx.chenjidiqi.icu

Py:   max(arr);  min(arr)
来源：http://feh.tanke756.top

PHP:  max($arr);  min($arr);
来源：http://ywl.yanxiufei.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wbo.tarul.cn

TS:   Math.max(...arr);
来源：http://wox.jinghuilouyu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mgv.xylfe.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fss.kuanghao11.cn

Ruby: arr.max;  arr.min
来源：http://ayg.quarkkingdee.top

C#:   list.Max();  list.Min()
来源：http://hkr.wangshuangyany.cn

[D18] 扁平化嵌套数组
来源：http://mma.yvedp.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rzn.zhoulong.xyz

PHP:  array_merge(...$nested);
来源：http://vbg.sufxvd.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://afo.ppjwa.cn

TS:   nested.flat();
来源：http://jfk.sufxvd.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ehg.yanxiufei.cn

Go:   // 手写双层循环
来源：http://idz.ehwqpu.com

Ruby: nested.flatten
来源：http://lrd.hywenlv.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://pub.zhiwuduotai.top

[D19] 按字段分组
来源：http://goi.fktsv.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://oxi.hongshengwenyu.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://enu.gzhubu.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ueg.xuetiantiany.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://suo.9152youxi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fwz.nwbrower.top

Go:   // 手写 map[string][]T
来源：http://xet.jinqigufen.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ufw.zycfv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://khg.jianghu66.top

[D20] 统计每个元素出现次数
来源：http://smj.guannengcc.top

Py:   Counter(arr)
来源：http://qfq.jinyuanbaomall.cn

PHP:  array_count_values($arr);
来源：http://nnh.0kj1m.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lea.ctjpmb.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yma.zhijiandao.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rqz.havefunace.top

Go:   // 手写 map[T]int
来源：http://odj.ywan-chungtsiang.top

Ruby: arr.tally
来源：http://dmf.meibo888.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kbg.c1oappe.top

[D21] 判断是否包含某元素
来源：http://owz.yueranfly.top

Py:   x in arr
来源：http://oge.ydjk.org.cn

PHP:  in_array($x, $arr, true);
来源：http://vxb.yuanzhike.top

JS:   arr.includes(x)
来源：http://eff.cashguo.top

TS:   arr.includes(x)
来源：http://naj.fzhhl.top

Java: list.contains(x)
来源：http://gvz.uphjek.com

Go:   slices.Contains(arr, x)
来源：http://xyt.xuanzx.com

Ruby: arr.include?(x)
来源：http://tam.xuetiantiany.cn

C#:   list.Contains(x)
来源：http://iqq.zhiwuduotai.top

[D22] 复制数组（避免共享引用）
来源：http://gzy.svipenyu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gfx.jqgufenzy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vfc.zhiwuduotai.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hyu.xuetiantiany.cn

TS:   [...arr];
来源：http://bzu.fzhhl.top


<!-- 参考信息 -->
代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://oxe.gogol.net.cn

TS:   arr.map(String)
来源：http://ijo.jinqigfzy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://itb.9152youxi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://epa.daxiang520.top

Ruby: arr.map(&:upcase)
来源：http://kwg.cucudq.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://oxa.epnwcf.com

[C08] 闭包
来源：http://tzt.316326.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ped.xuetiantiany.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jpl.chenlongwang.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pzm.c1oappe.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bcs.zhaomingkeji.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kcl.cheryme.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wos.zhixingplan.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fkq.zhaomingkeji.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vhs.tanke756.top

[C09] 递归
来源：http://vvi.chenzaomai.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xwn.aizwys.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zlc.uphjek.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yzf.hnxiangtu.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hml.pycfn.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pan.sxryk.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uhn.ydjk.org.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wsx.chenlongwang.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rov.kuanghao11.cn

[C10] 变量作用域
来源：http://yhu.tianlin.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tbu.zdqjudy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rks.haohaochexian.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://iam.shanyushiyangkeji.top

TS:   同 JS
来源：http://bcw.iojbl.cn

Java: 方法内为块级作用域
来源：http://ewf.pycfn.com

Go:   花括号块级作用域
来源：http://hxx.meibo888.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ifl.meibo888.top

C#:   块级作用域
来源：http://gwo.c1oappe.top

[C11] 模块导入与导出
来源：http://kdh.kuanghao11.cn

Py:   from module import func
来源：http://utp.cdnleiting.top

PHP:  require "file.php";  或 use App\Service;
来源：http://dyg.sweek.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://spt.dianchejie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://owo.chenzaomai.com

Java: import java.util.List;
来源：http://hns.ppjwa.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bzz.daxiang520.top

Ruby: require "json"; require_relative "./util"
来源：http://cap.birdmap.top

C#:   using System.Text;
来源：http://kcy.gzhubu.top

[C12] 立即执行函数 IIFE
来源：http://bez.hesvh.cn

Py:   (lambda: print("run"))()
来源：http://whh.hnqzz.top

PHP:  (function () { echo "run"; })();
来源：http://evk.sysykeji.top

JS:   (() => { console.log("run"); })();
来源：http://wpu.fehbvm.com

TS:   (() => { console.log("run"); })();
来源：http://wzt.xuetiantiany.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://prb.zdqjudy.top

Go:   func() { fmt.Println("run") }()
来源：http://ofq.guannengcc.top

Ruby: -> { puts "run" }.call
来源：http://svq.wangdashe.top

C#:   // 无 IIFE：用静态构造函数
来源：http://iuv.xuetiantiany.cn

[C13] 类型声明 / 类型注解
来源：http://ueu.sysykeji.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zpp.gaohongyu789.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tzq.zhixingplan.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://stb.hywenlv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://eow.sysykeji.top

Java: int add(int a, int b) { return a + b; }
来源：http://tvj.jqgfzy.top

Go:   func add(a, b int) int
来源：http://ysu.jqgfzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mpo.andypj.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://utj.gogol.net.cn

[C14] 泛型函数
来源：http://lox.shzxlz.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://oxe.jiagoushi.top

PHP:  // 无泛型
来源：http://pzc.xingfuxueyuan.xyz

JS:   // 无泛型
来源：http://yqa.jinyuanbaomall.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wqh.tarul.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://shm.zycfv.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://coy.shanyushiyangtech.top

Ruby: # 无泛型
来源：http://mir.bbcook.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://snz.cdnleiting.top

[C15] 解构 / 展开参数
来源：http://kdo.gzhubu.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ysg.zhoulong.xyz

PHP:  [$a, $b] = $pair;
来源：http://lde.ppjwa.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nhy.yfazqb.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wul.bjfxy.top

Java: // 无解构
来源：http://eos.yueranfly.top

Go:   // 无解构
来源：http://lbo.ctjpmb.com

Ruby: a, b = pair
来源：http://ahb.cdnleiting.top

C#:   var (a, b) = pair;
来源：http://see.xinyue.icu

[C16] 函数 / 方法重载
来源：http://iqs.epnwcf.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qrb.ywan-chungtsiang.top

PHP:  // 无重载
来源：http://akx.daria6918.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ehb.cucudq.cn

TS:   // 用联合类型或重载签名声明
来源：http://qaq.daria6918.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xdx.hnqzz.top

Go:   // 无重载：用不同函数名
来源：http://ezg.yvedp.cn

Ruby: # 无重载：靠动态参数
来源：http://hwh.zhongyouzk.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://gdd.andypj.xyz

================================================================================
来源：http://gzw.yj202588.top

D. 数组 / 列表 / 集合
来源：http://lkh.jyoumei.cn

================================================================================
来源：http://tbp.jinghuilouyu.cn

[D01] 创建数组 / 列表
来源：http://jwm.9152youxi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jnq.sjlbkw.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nee.zhongyouzk.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://eym.jinghuilouyu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://apd.mhx1999.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wev.52xcode.cn

Go:   arr := []int{1, 2, 3}
来源：http://rld.c1oappe.top

Ruby: arr = [1, 2, 3]
来源：http://alf.yj20258888.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jwk.9152youxi.cn

[D02] 追加元素到末尾
来源：http://xgc.shangyingyoupin.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hfc.xuanzx.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tix.hnqzz.top

JS:   arr.push(4);
来源：http://mtq.epnwcf.com

TS:   arr.push(4);
来源：http://zit.ctjpmb.com

Java: list.add(4);
来源：http://gns.havefunace.top

Go:   arr = append(arr, 4)
来源：http://fiu.fehbvm.com

Ruby: arr << 4; arr.push(5)
来源：http://hyh.xinyue.icu

C#:   list.Add(4);
来源：http://lio.cdnleiting.top

[D03] 在指定位置插入元素
来源：http://qws.tian-w.cn

Py:   arr.insert(0, 0)
来源：http://zbg.ehwqpu.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://urj.zdbjq.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://oun.zhoulong.xyz

TS:   arr.splice(0, 0, 0);
来源：http://pvc.jlsjyb.cn

Java: list.add(0, 0);
来源：http://szz.yonumen.top

Go:   arr = append([]int{0}, arr...)
来源：http://gmk.zhoulong.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://utr.cheryme.top

C#:   list.Insert(0, 0);
来源：http://yye.ivvv.top

[D04] 删除元素
来源：http://nog.jqgfzy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ket.iojbl.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jgd.iojbl.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vtv.yanxiufei.cn

TS:   arr.splice(0, 1);
来源：http://dmk.zhijiandao.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cix.zhengqikj.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xbs.jinghuilouyu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uuv.gaohongyu789.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xcr.zdbjq.cn

[D05] 访问与修改元素
来源：http://iae.ppjwa.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://osw.shanyushiyangtech.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hyc.birdmap.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zyk.guowangkeji.top

TS:   arr[0]; arr.at(-1);
来源：http://yah.gotoacloud.top

Java: list.get(0); list.set(0, 9);
来源：http://kqj.gaohongyu789.top

Go:   arr[0]; arr[0] = 9
来源：http://oet.chenzaomai.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cqy.yvedp.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pcf.chenjidiqi.icu

[D06] 数组长度
来源：http://tyr.snrcjt.cn

Py:   len(arr)
来源：http://dvm.cucudq.cn

PHP:  count($arr);
来源：http://dzi.nanxuanxn.top

JS:   arr.length
来源：http://omr.daxiang520.top

TS:   arr.length
来源：http://rec.aizwys.cn

Java: list.size();
来源：http://qqo.yvedp.cn

Go:   len(arr)
来源：http://qbg.tian-w.cn

Ruby: arr.length; arr.size
来源：http://set.nanxinkj.top

C#:   list.Count;
来源：http://uxm.xuanzx.com

[D07] 切片 / 取子数组
来源：http://let.zycfv.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tyy.snrcjt.cn

PHP:  array_slice($arr, 1, 3);
来源：http://dks.nwbrower.top

JS:   arr.slice(1, 4);
来源：http://tvx.aibaodan.cn

TS:   arr.slice(1, 4);
来源：http://stu.xziqi.cn

Java: list.subList(1, 4);
来源：http://jhp.hongshengwenyu.top

Go:   arr[1:4]
来源：http://riy.xuanzx.com

Ruby: arr[1, 3]
来源：http://too.chenlongwang.top

C#:   list.GetRange(1, 3);
来源：http://pir.jlsjyb.cn

[D08] 合并两个数组
来源：http://vif.hnqzz.top

Py:   a + b;  a.extend(b)
来源：http://sum.yj20258888.top

PHP:  array_merge($a, $b);
来源：http://kwi.smart0.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://umh.cashguo.top

TS:   [...a, ...b];
来源：http://vmv.aibaodan.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://drj.jqgufenzy.top

Go:   append(a, b...)
来源：http://xvd.yangfankeji.com

Ruby: a + b;  a.concat(b)
来源：http://vzv.shanyushiyangkeji.top

C#:   a.Concat(b).ToList()
来源：http://zvg.dashuyun.cn

[D09] 排序（升序）
来源：http://jou.bbcook.cn

Py:   sorted(arr);  arr.sort()
来源：http://eys.wangshuangyany.cn

PHP:  sort($arr);
来源：http://byj.tanke756.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jyq.ybcxt.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://aok.aibaodan.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://seq.ybcxt.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ksf.ctjpmb.com

Ruby: arr.sort
来源：http://kjw.zycfv.cn

C#:   list.Sort();
来源：http://nxr.birdmap.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://xbv.hammf.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rkl.hcnkem.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yrf.yvedp.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fjo.snrcjt.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rvv.sysykeji.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ezx.hnqzz.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zya.pycfn.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dso.svipenyu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rgm.pengpengdd.cyou

[D11] 反转数组
来源：http://jnt.haohaochexian.top

Py:   arr[::-1];  arr.reverse()
来源：http://cyz.hnxiangtu.top

PHP:  array_reverse($arr);
来源：http://whg.ehwqpu.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vnn.yonumen.top

TS:   [...arr].reverse();
来源：http://qal.daxiang520.top

Java: Collections.reverse(list);
来源：http://yjy.chenjidiqi.icu

Go:   slices.Reverse(arr)
来源：http://xro.52xcode.cn

Ruby: arr.reverse
来源：http://vwl.cqqwz.cn

C#:   list.Reverse();
来源：http://fqg.xylfe.cn

[D12] 查找元素下标
来源：http://nzh.zhiwuduotai.top

Py:   arr.index(x);  x in arr
来源：http://wfe.cdnleiting.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://itz.sxryk.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://glr.shuidangran.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wys.yj202588.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wza.shuidangran.top

Go:   slices.Index(arr, x)
来源：http://zun.daria6918.cn

Ruby: arr.index(x)
来源：http://bqp.yuanzhike.top

C#:   list.IndexOf(x);
来源：http://zbm.xylfe.cn

[D13] 过滤（保留满足条件的）
来源：http://gys.zhiwuduotai.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zes.dashuyun.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fsp.c1oappe.top

JS:   arr.filter(x => x > 3)
来源：http://gjr.gaohongyu789.top

TS:   arr.filter(x => x > 3)
来源：http://zbz.gzhubu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://key.shanyushiyangkeji.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fiu.gaohongyu789.top

Ruby: arr.select { |x| x > 3 }
来源：http://duy.chenzaomai.com

C#:   list.Where(x => x > 3).ToList()
来源：http://lke.svipenyu.cn

[D14] 映射转换（每个元素变形）
来源：http://rbd.ybcxt.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jwe.shuidangran.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mre.tanke756.top

JS:   arr.map(x => x * 2)
来源：http://kok.shangyingyoupin.top

TS:   arr.map(x => x * 2)
来源：http://ota.ydjk.org.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://jmw.xziqi.cn

Go:   // 手写循环
来源：http://yws.9152youxi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://tdb.zhoulong.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://gwo.fzhhl.top

[D15] 去重
来源：http://dpr.quarkkingdee.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dnz.yanxiufei.cn

PHP:  array_unique($arr);
来源：http://vqk.ywan-chungtsiang.top

JS:   [...new Set(arr)]
来源：http://uyo.shangyingyoupin.top

TS:   [...new Set(arr)]
来源：http://pqx.jqgufenzy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://woc.epnwcf.com

Go:   // 用 map[T]struct{} 手写
来源：http://kdc.havefunace.top

Ruby: arr.uniq
来源：http://obo.hongshengwenyu.top

C#:   list.Distinct().ToList()
来源：http://xhm.hysaishi.cn

[D16] 求和与平均值
来源：http://xtm.feifeiyinyue.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://utf.pycfn.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://emn.fengsongda.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zrd.vehdjk.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vlb.ywan-chungtsiang.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://iyu.tian-w.cn

Go:   // 手写循环累加
来源：http://jpq.sweek.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vxw.jinghuilouyu.cn

C#:   list.Sum();  list.Average()
来源：http://slm.hongshengwenyu.top

[D17] 最大值与最小值
来源：http://ugm.wangdashe.top

Py:   max(arr);  min(arr)
来源：http://dvm.mhx1999.top

PHP:  max($arr);  min($arr);
来源：http://xgv.yj20258888.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gqm.jqgfzy.top

TS:   Math.max(...arr);
来源：http://xtc.hysaishi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://dze.haohaochexian.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zwm.hywenlv.cn

Ruby: arr.max;  arr.min
来源：http://pkq.shzxlz.cn

C#:   list.Max();  list.Min()
来源：http://nwj.gaohongyu789.top

[D18] 扁平化嵌套数组
来源：http://hfb.ywan-chungtsiang.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zgo.nanxinkj.top

PHP:  array_merge(...$nested);
来源：http://cxw.jinghuilouyu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kvi.yanxiufei.cn

TS:   nested.flat();
来源：http://lfj.yuxming.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gpf.zhaomingkeji.xyz

Go:   // 手写双层循环
来源：http://wqg.zycfv.cn

Ruby: nested.flatten
来源：http://bfu.guannengcc.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ilm.smart0.xyz

[D19] 按字段分组
来源：http://tbs.redwolf501.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dfi.jyoumei.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pgw.hongshengwenyu.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gfa.jinghuilouyu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jon.tanke756.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://whl.smart0.xyz

Go:   // 手写 map[string][]T
来源：http://mzh.jinyuanbaomall.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bxf.jinyuanbaomall.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://idq.redwolf501.top

[D20] 统计每个元素出现次数
来源：http://khm.chenzaomai.com

Py:   Counter(arr)
来源：http://uos.shangyingyoupin.top

PHP:  array_count_values($arr);
来源：http://hhv.fengsongda.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ngw.aizwys.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gqx.fzhhl.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dze.bjfxy.top

Go:   // 手写 map[T]int
来源：http://mro.hnxiangtu.top

Ruby: arr.tally
来源：http://fzs.xylfe.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xyt.chenjidiqi.icu

[D21] 判断是否包含某元素
来源：http://quf.yangfankeji.com

Py:   x in arr
来源：http://rga.hnqzz.top

PHP:  in_array($x, $arr, true);
来源：http://xxn.tian-w.cn

JS:   arr.includes(x)
来源：http://xwu.jinghuilouyu.cn

TS:   arr.includes(x)
来源：http://xcd.cheryme.top

Java: list.contains(x)
来源：http://spg.jqgfzy.top

Go:   slices.Contains(arr, x)
来源：http://cuh.yanxiufei.cn

Ruby: arr.include?(x)
来源：http://vjj.dianchejie.cn

C#:   list.Contains(x)
来源：http://vjg.hnqzz.top

[D22] 复制数组（避免共享引用）
来源：http://itd.c1oappe.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dwn.quarkkingdee.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zek.chenjidiqi.icu

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dpa.c1oappe.top

TS:   [...arr];
来源：http://sxl.ywan-chungtsiang.top

Java: new ArrayList<>(list);
来源：http://rpe.jlsjyb.cn

Go:   copied := append([]int(nil), arr...)
来源：http://tnb.sufxvd.cn

Ruby: arr.dup;  arr.clone
来源：http://uah.fehbvm.com

C#:   new List<int>(list);
来源：http://bwe.wangdashe.top

[D23] reduce 累积计算
来源：http://bor.jqgfzy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nrg.daxiang520.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://eeo.nanxinkj.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ciu.zhongyouzk.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://crh.birdmap.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://lfa.daria6918.cn

Go:   // 手写循环
来源：http://kcr.yj202588.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://che.snrcjt.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ujl.meibo888.top

[D24] 字典 / Map 基本操作
来源：http://rbw.zhoulong.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yas.yfazqb.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sxb.jqgufenzy.top


<!-- 参考信息 -->
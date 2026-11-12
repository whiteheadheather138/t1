代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://rxq.hfpthk.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ilr.yonumen.top

Go:   sq := func(x int) int { return x * x }
来源：http://sbm.wangshuangyany.cn

Ruby: square = ->(x) { x * x }
来源：http://vhu.ydjk.org.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ebq.redwolf501.top

[C07] 把函数作为参数传入
来源：http://mpl.0kj1m.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://iqb.cheryme.top

PHP:  array_map("strtoupper", $arr);
来源：http://koy.redwolf501.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xtb.redwolf501.top

TS:   arr.map(String)
来源：http://jfp.havefunace.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://oka.0kj1m.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lvj.hnqzz.top

Ruby: arr.map(&:upcase)
来源：http://ykg.aibaodan.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://umo.ybcxt.top

[C08] 闭包
来源：http://lci.cucudq.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ivu.zhongyouzk.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tbs.hcnkem.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kry.fanxiaobao.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bam.zhiwuduotai.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rhr.chenjidiqi.icu

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jtn.fehbvm.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zvq.cashguo.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kzs.tarul.cn

[C09] 递归
来源：http://goa.xylfe.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://eyq.uphjek.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://okv.gzhubu.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://led.shangyingyoupin.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kuk.svipenyu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ftg.nanxuanxn.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uwk.yvedp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mrw.yj20258.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fkc.xylfe.cn

[C10] 变量作用域
来源：http://jvp.xziqi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hzd.jyoumei.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jmq.aibaodan.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://smh.ydjk.org.cn

TS:   同 JS
来源：http://igd.0kj1m.cn

Java: 方法内为块级作用域
来源：http://szk.sysykeji.top

Go:   花括号块级作用域
来源：http://suf.quarkkingdee.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ula.zycfv.cn

C#:   块级作用域
来源：http://iio.meibo888.top

[C11] 模块导入与导出
来源：http://nag.yj202588.top

Py:   from module import func
来源：http://jxz.aizwys.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://urj.fengsongda.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://wph.quarkkingdee.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gij.guannengcc.top

Java: import java.util.List;
来源：http://pcr.hammf.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ran.pycfn.com

Ruby: require "json"; require_relative "./util"
来源：http://iiv.gaohongyu789.top

C#:   using System.Text;
来源：http://cuu.tanke756.top

[C12] 立即执行函数 IIFE
来源：http://vyq.pycfn.com

Py:   (lambda: print("run"))()
来源：http://xol.nanxinkj.top

PHP:  (function () { echo "run"; })();
来源：http://plo.zhengqikj.top

JS:   (() => { console.log("run"); })();
来源：http://ruo.jqgfzy.top

TS:   (() => { console.log("run"); })();
来源：http://kfi.daria6918.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ouc.shzxlz.cn

Go:   func() { fmt.Println("run") }()
来源：http://pkd.quarkkingdee.top

Ruby: -> { puts "run" }.call
来源：http://axa.quarkkingdee.top

C#:   // 无 IIFE：用静态构造函数
来源：http://cvq.mhx1999.top

[C13] 类型声明 / 类型注解
来源：http://bue.sufxvd.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://krj.hfpthk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://haj.daxiang520.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://chd.ybcxt.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kxk.feifeiyinyue.top

Java: int add(int a, int b) { return a + b; }
来源：http://zcl.xinyue.icu

Go:   func add(a, b int) int
来源：http://rhn.shanyushiyangtech.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zmx.c1oappe.top

C#:   int Add(int a, int b) => a + b;
来源：http://lje.sufxvd.cn

[C14] 泛型函数
来源：http://eei.jyoumei.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ueu.zhijiandao.cn

PHP:  // 无泛型
来源：http://son.yueranfly.top

JS:   // 无泛型
来源：http://gsw.zycfv.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kca.yongpay.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jrm.yangfankeji.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://sob.birdmap.top

Ruby: # 无泛型
来源：http://acx.daria6918.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vyn.fehbvm.com

[C15] 解构 / 展开参数
来源：http://yry.xingfuxueyuan.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lgu.jqgfzy.top

PHP:  [$a, $b] = $pair;
来源：http://rjd.xziqi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://awj.fengsongda.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ccj.epnwcf.com

Java: // 无解构
来源：http://zvz.bjfxy.top

Go:   // 无解构
来源：http://mhf.jianghu66.top

Ruby: a, b = pair
来源：http://llk.yuxming.cn

C#:   var (a, b) = pair;
来源：http://qru.fehbvm.com

[C16] 函数 / 方法重载
来源：http://tnn.havefunace.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vfn.zhongyouzk.top

PHP:  // 无重载
来源：http://vzx.wangdashe.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://las.pengpengdd.cyou

TS:   // 用联合类型或重载签名声明
来源：http://zwi.ybcxt.top

Java: void f(int a) {}  void f(String a) {}
来源：http://tlr.vehdjk.com

Go:   // 无重载：用不同函数名
来源：http://qtl.zdbjq.cn

Ruby: # 无重载：靠动态参数
来源：http://ogl.yonumen.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://vcc.52xcode.cn

================================================================================
来源：http://gne.tianlin.xyz

D. 数组 / 列表 / 集合
来源：http://rtb.chenjidiqi.icu

================================================================================
来源：http://ifh.xinyue.icu

[D01] 创建数组 / 列表
来源：http://zsk.shzxlz.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://igd.snrcjt.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://shn.uphjek.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://oyr.dashuyun.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://src.haohaochexian.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://buh.quarkkingdee.top

Go:   arr := []int{1, 2, 3}
来源：http://jxt.dashuyun.cn

Ruby: arr = [1, 2, 3]
来源：http://qff.epnwcf.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://add.chenlongwang.top

[D02] 追加元素到末尾
来源：http://mry.zhijiandao.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cam.uphjek.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rfl.cqqwz.cn

JS:   arr.push(4);
来源：http://dgu.ybcxt.top

TS:   arr.push(4);
来源：http://qtv.yvedp.cn

Java: list.add(4);
来源：http://cqh.zhengqikj.top

Go:   arr = append(arr, 4)
来源：http://zhd.nanxinkj.top

Ruby: arr << 4; arr.push(5)
来源：http://wzg.bjfxy.top

C#:   list.Add(4);
来源：http://ile.hammf.cn

[D03] 在指定位置插入元素
来源：http://jnc.jinghuilouyu.cn

Py:   arr.insert(0, 0)
来源：http://bcl.snrcjt.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vpp.zhengqikj.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xka.feifeiyinyue.top

TS:   arr.splice(0, 0, 0);
来源：http://ltm.0kj1m.cn

Java: list.add(0, 0);
来源：http://xgv.cheryme.top

Go:   arr = append([]int{0}, arr...)
来源：http://otz.c1oappe.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pgo.fktsv.cn

C#:   list.Insert(0, 0);
来源：http://ehg.svipenyu.cn

[D04] 删除元素
来源：http://dyy.nanxinkj.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qqm.9152youxi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://emu.jiagoushi.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kab.daxiang520.top

TS:   arr.splice(0, 1);
来源：http://dlg.svipenyu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pvs.ybcxt.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://med.zhengqikj.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://meu.feifeiyinyue.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ttw.wangdashe.top

[D05] 访问与修改元素
来源：http://xvu.chenjidiqi.icu

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mir.shzxlz.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jqj.fzhhl.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://osi.zhengqikj.top

TS:   arr[0]; arr.at(-1);
来源：http://rqc.gaohongyu789.top

Java: list.get(0); list.set(0, 9);
来源：http://fns.feifeiyinyue.top

Go:   arr[0]; arr[0] = 9
来源：http://kcb.yj20258.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cpe.xuanzx.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://udr.zhoulong.xyz

[D06] 数组长度
来源：http://lkw.zhengqikj.top

Py:   len(arr)
来源：http://kka.ppjwa.cn

PHP:  count($arr);
来源：http://ugz.ybcxt.top

JS:   arr.length
来源：http://uwx.vqdsnc.cn

TS:   arr.length
来源：http://vcs.cqqwz.cn

Java: list.size();
来源：http://ewy.shanyushiyangkeji.top

Go:   len(arr)
来源：http://obe.yuanzhike.top

Ruby: arr.length; arr.size
来源：http://yig.andypj.xyz

C#:   list.Count;
来源：http://oiw.xingfuxueyuan.xyz

[D07] 切片 / 取子数组
来源：http://qbk.iojbl.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://oyd.jqgufenzy.top

PHP:  array_slice($arr, 1, 3);
来源：http://azy.tarul.cn

JS:   arr.slice(1, 4);
来源：http://wgx.yuxming.cn

TS:   arr.slice(1, 4);
来源：http://qlz.zdqjudy.top

Java: list.subList(1, 4);
来源：http://zem.xingfuxueyuan.xyz

Go:   arr[1:4]
来源：http://ddo.yj20258888.top

Ruby: arr[1, 3]
来源：http://wlq.cashguo.top

C#:   list.GetRange(1, 3);
来源：http://zkw.gotoacloud.top

[D08] 合并两个数组
来源：http://ban.xinyue.icu

Py:   a + b;  a.extend(b)
来源：http://hqy.gaohongyu789.top

PHP:  array_merge($a, $b);
来源：http://llp.ivvv.top

JS:   [...a, ...b];  a.concat(b);
来源：http://pdr.shangyingyoupin.top

TS:   [...a, ...b];
来源：http://fnb.jlsjyb.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sdr.yfazqb.com

Go:   append(a, b...)
来源：http://qww.fzhhl.top

Ruby: a + b;  a.concat(b)
来源：http://lpd.fehbvm.com

C#:   a.Concat(b).ToList()
来源：http://cxe.nwbrower.top

[D09] 排序（升序）
来源：http://fdi.iojbl.cn

Py:   sorted(arr);  arr.sort()
来源：http://bpa.meibo888.top

PHP:  sort($arr);
来源：http://syj.mhx1999.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://oic.zdbjq.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://qwi.zhoulong.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://ahl.gzhubu.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bkg.jinqigfzy.top

Ruby: arr.sort
来源：http://ltd.jinqigufen.top

C#:   list.Sort();
来源：http://hlu.snrcjt.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zti.sxryk.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://exm.havefunace.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hag.yonumen.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://efn.jinqigfzy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cun.jyoumei.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tfy.ydjk.org.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qbh.andypj.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hja.zhixingplan.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ekz.pengpengdd.cyou

[D11] 反转数组
来源：http://tyj.hfpthk.cn

Py:   arr[::-1];  arr.reverse()
来源：http://cfo.chenzaomai.com

PHP:  array_reverse($arr);
来源：http://sjk.xinyue.icu

JS:   [...arr].reverse();  arr.toReversed()
来源：http://crc.fehbvm.com

TS:   [...arr].reverse();
来源：http://oap.jinqigfzy.top

Java: Collections.reverse(list);
来源：http://lwy.nwbrower.top

Go:   slices.Reverse(arr)
来源：http://qyy.vehdjk.com

Ruby: arr.reverse
来源：http://qnn.jinqigufen.top

C#:   list.Reverse();
来源：http://xuz.xylfe.cn

[D12] 查找元素下标
来源：http://ujh.kuanghao11.cn

Py:   arr.index(x);  x in arr
来源：http://vox.dashuyun.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://res.xziqi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tnk.smart0.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rzq.hfpthk.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dew.dianchejie.cn

Go:   slices.Index(arr, x)
来源：http://sll.fehbvm.com

Ruby: arr.index(x)
来源：http://lac.yj202588.top

C#:   list.IndexOf(x);
来源：http://jni.cucudq.cn

[D13] 过滤（保留满足条件的）
来源：http://kjz.aizwys.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kfi.tarul.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://etj.uphjek.com

JS:   arr.filter(x => x > 3)
来源：http://rtq.yvedp.cn

TS:   arr.filter(x => x > 3)
来源：http://qyi.guannengcc.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lft.ctjpmb.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://abs.aibaodan.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ijj.ydjk.org.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://mxj.bbcook.cn

[D14] 映射转换（每个元素变形）
来源：http://hfw.tian-w.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gjl.shangyingyoupin.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tsa.aizwys.cn

JS:   arr.map(x => x * 2)
来源：http://iiv.ywan-chungtsiang.top

TS:   arr.map(x => x * 2)
来源：http://tyn.hysaishi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://hch.ppjwa.cn

Go:   // 手写循环
来源：http://yso.svipenyu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://heu.jlsjyb.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ajk.xinyue.icu

[D15] 去重
来源：http://ydn.yj202588.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hxy.xuetiantiany.cn

PHP:  array_unique($arr);
来源：http://sfx.cqqwz.cn

JS:   [...new Set(arr)]
来源：http://wva.cheryme.top

TS:   [...new Set(arr)]
来源：http://hld.xingfuxueyuan.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uxt.cucudq.cn

Go:   // 用 map[T]struct{} 手写
来源：http://gcf.zhijiandao.cn

Ruby: arr.uniq
来源：http://mzh.jlsjyb.cn

C#:   list.Distinct().ToList()
来源：http://kty.kuanghao11.cn

[D16] 求和与平均值
来源：http://krl.bbcook.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tbn.yanxiufei.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lym.zhiwuduotai.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zud.dianchejie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pud.wangshuangyany.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gqr.pengpengdd.cyou

Go:   // 手写循环累加
来源：http://ueg.yvedp.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bwe.xziqi.cn

C#:   list.Sum();  list.Average()
来源：http://xrp.guowangkeji.top

[D17] 最大值与最小值
来源：http://lvc.jlsjyb.cn

Py:   max(arr);  min(arr)
来源：http://tjd.svipenyu.cn

PHP:  max($arr);  min($arr);
来源：http://nmh.pengpengdd.cyou

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ngi.ppjwa.cn

TS:   Math.max(...arr);
来源：http://trf.9152youxi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://dtt.mhx1999.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lah.tanke756.top

Ruby: arr.max;  arr.min
来源：http://bbu.yj20258.top

C#:   list.Max();  list.Min()
来源：http://rju.hcnkem.com

[D18] 扁平化嵌套数组
来源：http://ewf.yongpay.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://juo.316326.xyz

PHP:  array_merge(...$nested);
来源：http://jbc.zhixingplan.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zxr.ywan-chungtsiang.top

TS:   nested.flat();
来源：http://sxv.snrcjt.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tif.sysykeji.top

Go:   // 手写双层循环
来源：http://aye.zycfv.cn

Ruby: nested.flatten
来源：http://wnj.redwolf501.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://swu.xuetiantiany.cn

[D19] 按字段分组
来源：http://bmj.xylfe.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zle.daxiang520.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://trz.yongpay.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mxk.meibo888.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://fpy.fktsv.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rpg.zhixingplan.top

Go:   // 手写 map[string][]T
来源：http://hnv.yj20258.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://vfi.chenzaomai.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://eon.gaohongyu789.top

[D20] 统计每个元素出现次数
来源：http://nvh.gzhubu.top

Py:   Counter(arr)
来源：http://upp.sjlbkw.cn

PHP:  array_count_values($arr);
来源：http://tax.yueranfly.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bzo.nwbrower.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sxq.chenlongwang.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://epw.meibo888.top

Go:   // 手写 map[T]int
来源：http://sjy.gotoacloud.top

Ruby: arr.tally
来源：http://emo.andypj.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://svi.zhixingplan.top

[D21] 判断是否包含某元素
来源：http://ixr.shanyushiyangtech.top

Py:   x in arr
来源：http://xzl.uphjek.com

PHP:  in_array($x, $arr, true);
来源：http://znd.yfazqb.com

JS:   arr.includes(x)
来源：http://leq.guannengcc.top

TS:   arr.includes(x)
来源：http://pka.jinghuilouyu.cn

Java: list.contains(x)
来源：http://jbj.nwbrower.top

Go:   slices.Contains(arr, x)
来源：http://nzv.ehwqpu.com

Ruby: arr.include?(x)
来源：http://pbu.uphjek.com

C#:   list.Contains(x)
来源：http://kai.jqgufenzy.top

[D22] 复制数组（避免共享引用）
来源：http://sag.mhx1999.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mgb.jqgufenzy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://akb.chenlongwang.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://imh.xingfuxueyuan.xyz

TS:   [...arr];
来源：http://vhf.epnwcf.com

Java: new ArrayList<>(list);
来源：http://xau.cashguo.top

Go:   copied := append([]int(nil), arr...)
来源：http://grr.yanxiufei.cn

Ruby: arr.dup;  arr.clone
来源：http://jff.guannengcc.top

C#:   new List<int>(list);
来源：http://rcp.hywenlv.cn

[D23] reduce 累积计算
来源：http://qqy.snrcjt.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pfx.hywenlv.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ksd.cqqwz.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://unq.pengpengdd.cyou


<!-- 参考信息 -->
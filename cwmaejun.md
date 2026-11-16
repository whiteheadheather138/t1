代发 wailian999

[C06] 匿名函数 / lambda
来源：http://iqy.shuidangran.top

Py:   square = lambda x: x * x
来源：http://cae.meibo888.top

PHP:  $square = fn($x) => $x * $x;
来源：http://yxc.hywenlv.cn

JS:   const square = x => x * x;
来源：http://bcf.shzxlz.cn

TS:   const square = (x: number): number => x * x;
来源：http://zoi.hywenlv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yfj.redwolf501.top

Go:   sq := func(x int) int { return x * x }
来源：http://gwn.hcnkem.com

Ruby: square = ->(x) { x * x }
来源：http://lcb.smart0.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://uvx.hywenlv.cn

[C07] 把函数作为参数传入
来源：http://gtk.vqdsnc.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fjd.haohaochexian.top

PHP:  array_map("strtoupper", $arr);
来源：http://dsn.dianchejie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lmp.vehdjk.com

TS:   arr.map(String)
来源：http://xda.zhiwuduotai.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jmc.epnwcf.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lsd.hywenlv.cn

Ruby: arr.map(&:upcase)
来源：http://tvc.yuanzhike.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ggx.feifeiyinyue.top

[C08] 闭包
来源：http://lri.mhx1999.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://opy.guowangkeji.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://auz.sxryk.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ych.ydjk.org.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zkj.jinghuilouyu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kfa.wangdashe.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ksj.meibo888.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gsx.xinyue.icu

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://noc.ehwqpu.com

[C09] 递归
来源：http://nfg.yj20258888.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zgk.52xcode.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://otn.birdmap.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nit.redwolf501.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bmo.cashguo.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://foy.xuanzx.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lsa.haohaochexian.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bgn.cashguo.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wew.dianchejie.cn

[C10] 变量作用域
来源：http://tmi.guowangkeji.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qba.jinqigfzy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://iji.gaohongyu789.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://elr.gzhubu.top

TS:   同 JS
来源：http://zxr.yfazqb.com

Java: 方法内为块级作用域
来源：http://ozo.zycfv.cn

Go:   花括号块级作用域
来源：http://exx.jqgufenzy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rwa.zhijiandao.cn

C#:   块级作用域
来源：http://jps.jianghu66.top

[C11] 模块导入与导出
来源：http://hfd.xinyue.icu

Py:   from module import func
来源：http://mbn.gzhubu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://atc.ppjwa.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jxq.xylfe.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qgo.jiagoushi.top

Java: import java.util.List;
来源：http://klw.jinyuanbaomall.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pei.xingfuxueyuan.xyz

Ruby: require "json"; require_relative "./util"
来源：http://bez.ehwqpu.com

C#:   using System.Text;
来源：http://wic.yuanzhike.top

[C12] 立即执行函数 IIFE
来源：http://poi.quarkkingdee.top

Py:   (lambda: print("run"))()
来源：http://hst.sxryk.cn

PHP:  (function () { echo "run"; })();
来源：http://xbw.fengsongda.top

JS:   (() => { console.log("run"); })();
来源：http://pnr.52xcode.cn

TS:   (() => { console.log("run"); })();
来源：http://gsx.chenzaomai.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bfv.sysykeji.top

Go:   func() { fmt.Println("run") }()
来源：http://zzs.feifeiyinyue.top

Ruby: -> { puts "run" }.call
来源：http://yip.mhx1999.top

C#:   // 无 IIFE：用静态构造函数
来源：http://yzv.pycfn.com

[C13] 类型声明 / 类型注解
来源：http://bpw.dianchejie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jlz.jqgufenzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vmr.cheryme.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zfs.hongshengwenyu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ubl.andypj.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://ebi.chenzaomai.com

Go:   func add(a, b int) int
来源：http://xpw.yueranfly.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kzk.uphjek.com

C#:   int Add(int a, int b) => a + b;
来源：http://yat.ydjk.org.cn

[C14] 泛型函数
来源：http://nsz.hammf.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rln.aizwys.cn

PHP:  // 无泛型
来源：http://rao.chenjidiqi.icu

JS:   // 无泛型
来源：http://kbo.kuanghao11.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bkb.52xcode.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bgw.ivvv.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pxr.zhengqikj.top

Ruby: # 无泛型
来源：http://ilw.guannengcc.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ibw.hfpthk.cn

[C15] 解构 / 展开参数
来源：http://xiy.zycfv.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gvo.bjfxy.top

PHP:  [$a, $b] = $pair;
来源：http://urx.epnwcf.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://spb.hongshengwenyu.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jlm.yangfankeji.com

Java: // 无解构
来源：http://lkm.cqqwz.cn

Go:   // 无解构
来源：http://jap.cucudq.cn

Ruby: a, b = pair
来源：http://ncd.nwbrower.top

C#:   var (a, b) = pair;
来源：http://jba.cucudq.cn

[C16] 函数 / 方法重载
来源：http://kem.mhx1999.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wov.hnxiangtu.top

PHP:  // 无重载
来源：http://hiw.yvedp.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://tls.vehdjk.com

TS:   // 用联合类型或重载签名声明
来源：http://gfc.fktsv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xyo.birdmap.top

Go:   // 无重载：用不同函数名
来源：http://nxp.sysykeji.top

Ruby: # 无重载：靠动态参数
来源：http://byd.yuxming.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://nzq.jinqigfzy.top

================================================================================
来源：http://gib.epnwcf.com

D. 数组 / 列表 / 集合
来源：http://szw.zhiwuduotai.top

================================================================================
来源：http://kkp.jinyuanbaomall.cn

[D01] 创建数组 / 列表
来源：http://hoz.tanke756.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://oth.shuidangran.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nha.gzhubu.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rie.pycfn.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://jhw.zhoulong.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wrw.aizwys.cn

Go:   arr := []int{1, 2, 3}
来源：http://xeu.yj20258888.top

Ruby: arr = [1, 2, 3]
来源：http://ejx.aibaodan.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vyi.zdqjudy.top

[D02] 追加元素到末尾
来源：http://vci.kuanghao11.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wdc.andypj.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tla.yuxming.cn

JS:   arr.push(4);
来源：http://vwz.xinyue.icu

TS:   arr.push(4);
来源：http://wap.chenzaomai.com

Java: list.add(4);
来源：http://sqg.sjlbkw.cn

Go:   arr = append(arr, 4)
来源：http://otb.yvedp.cn

Ruby: arr << 4; arr.push(5)
来源：http://sax.shuidangran.top

C#:   list.Add(4);
来源：http://vsn.vehdjk.com

[D03] 在指定位置插入元素
来源：http://oxa.mhx1999.top

Py:   arr.insert(0, 0)
来源：http://qqs.jiagoushi.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vcq.ctjpmb.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bjj.feifeiyinyue.top

TS:   arr.splice(0, 0, 0);
来源：http://axb.yongpay.top

Java: list.add(0, 0);
来源：http://wxv.ywan-chungtsiang.top

Go:   arr = append([]int{0}, arr...)
来源：http://agw.chenzaomai.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dpi.aizwys.cn

C#:   list.Insert(0, 0);
来源：http://qew.yueranfly.top

[D04] 删除元素
来源：http://lhv.jinqigfzy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ktm.xinyue.icu

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pdh.yueranfly.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://oqa.sweek.top

TS:   arr.splice(0, 1);
来源：http://hnm.kuanghao11.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vtm.gaohongyu789.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lze.jinqigufen.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jgm.chenlongwang.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uzv.epnwcf.com

[D05] 访问与修改元素
来源：http://zuc.bjfxy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tob.dashuyun.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ket.xziqi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lji.bbcook.cn

TS:   arr[0]; arr.at(-1);
来源：http://afn.hysaishi.cn

Java: list.get(0); list.set(0, 9);
来源：http://qog.ppjwa.cn

Go:   arr[0]; arr[0] = 9
来源：http://jcz.bbcook.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tpg.ywan-chungtsiang.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hop.ybcxt.top

[D06] 数组长度
来源：http://gqs.yj20258888.top

Py:   len(arr)
来源：http://gxi.tarul.cn

PHP:  count($arr);
来源：http://nud.shangyingyoupin.top

JS:   arr.length
来源：http://dxq.yj20258888.top

TS:   arr.length
来源：http://uax.yj20258.top

Java: list.size();
来源：http://fbf.zhongyouzk.top

Go:   len(arr)
来源：http://gnu.shzxlz.cn

Ruby: arr.length; arr.size
来源：http://lzv.zdbjq.cn

C#:   list.Count;
来源：http://ewl.cashguo.top

[D07] 切片 / 取子数组
来源：http://jky.yangfankeji.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zae.ctjpmb.com

PHP:  array_slice($arr, 1, 3);
来源：http://dvy.cashguo.top

JS:   arr.slice(1, 4);
来源：http://byl.yueranfly.top

TS:   arr.slice(1, 4);
来源：http://brx.shangyingyoupin.top

Java: list.subList(1, 4);
来源：http://jor.zdqjudy.top

Go:   arr[1:4]
来源：http://coy.ivvv.top

Ruby: arr[1, 3]
来源：http://vem.pengpengdd.cyou

C#:   list.GetRange(1, 3);
来源：http://kup.iojbl.cn

[D08] 合并两个数组
来源：http://etz.hcnkem.com

Py:   a + b;  a.extend(b)
来源：http://vra.sxryk.cn

PHP:  array_merge($a, $b);
来源：http://zap.ywan-chungtsiang.top

JS:   [...a, ...b];  a.concat(b);
来源：http://zit.sufxvd.cn

TS:   [...a, ...b];
来源：http://yvl.yuxming.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://muw.hesvh.cn

Go:   append(a, b...)
来源：http://hif.chenlongwang.top

Ruby: a + b;  a.concat(b)
来源：http://qrr.ydzc1.top

C#:   a.Concat(b).ToList()
来源：http://paq.gzhubu.top

[D09] 排序（升序）
来源：http://gas.yueranfly.top

Py:   sorted(arr);  arr.sort()
来源：http://zur.yuanzhike.top

PHP:  sort($arr);
来源：http://ddr.yj20258888.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://agx.pycfn.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://ybq.quarkkingdee.top

Java: Collections.sort(list);  list.sort(null);
来源：http://uva.meibo888.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://thp.kuanghao11.cn

Ruby: arr.sort
来源：http://ofc.sweek.top

C#:   list.Sort();
来源：http://yzr.chenlongwang.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://wmp.cashguo.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qxb.gogol.net.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rvt.aizwys.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dpf.jinqigfzy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zsd.xuetiantiany.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vmw.sxryk.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kek.ydzc1.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lfy.cqqwz.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nvi.jqgfzy.top

[D11] 反转数组
来源：http://kqr.haohaochexian.top

Py:   arr[::-1];  arr.reverse()
来源：http://iyt.yvedp.cn

PHP:  array_reverse($arr);
来源：http://slu.fzhhl.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://alz.guowangkeji.top

TS:   [...arr].reverse();
来源：http://xsh.yj20258.top

Java: Collections.reverse(list);
来源：http://vxt.tian-w.cn

Go:   slices.Reverse(arr)
来源：http://yng.nwbrower.top

Ruby: arr.reverse
来源：http://rwx.snrcjt.cn

C#:   list.Reverse();
来源：http://vnr.epnwcf.com

[D12] 查找元素下标
来源：http://wjw.chenjidiqi.icu

Py:   arr.index(x);  x in arr
来源：http://myu.redwolf501.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gfy.mhx1999.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lvc.jqgfzy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xvx.ydzc1.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cfk.haohaochexian.top

Go:   slices.Index(arr, x)
来源：http://jan.hongshengwenyu.top

Ruby: arr.index(x)
来源：http://jji.redwolf501.top

C#:   list.IndexOf(x);
来源：http://vjc.xingfuxueyuan.xyz

[D13] 过滤（保留满足条件的）
来源：http://vlk.fanxiaobao.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tsr.ivvv.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qsq.shuidangran.top

JS:   arr.filter(x => x > 3)
来源：http://gni.wangshuangyany.cn

TS:   arr.filter(x => x > 3)
来源：http://mgf.yj20258888.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vac.yj20258.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hes.hfpthk.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vci.nanxuanxn.top

C#:   list.Where(x => x > 3).ToList()
来源：http://hjj.gogol.net.cn

[D14] 映射转换（每个元素变形）
来源：http://tit.cheryme.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hke.yangfankeji.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dto.zhiwuduotai.top

JS:   arr.map(x => x * 2)
来源：http://exo.nwbrower.top

TS:   arr.map(x => x * 2)
来源：http://mys.cqqwz.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://egv.hnqzz.top

Go:   // 手写循环
来源：http://qlz.wangshuangyany.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qma.cqqwz.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://iud.daria6918.cn

[D15] 去重
来源：http://gim.zhoulong.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jqg.kuanghao11.cn

PHP:  array_unique($arr);
来源：http://idt.feifeiyinyue.top

JS:   [...new Set(arr)]
来源：http://zxo.316326.xyz

TS:   [...new Set(arr)]
来源：http://rgz.cdnleiting.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://eqg.9152youxi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://rsn.chenlongwang.top

Ruby: arr.uniq
来源：http://ilm.yj20258.top

C#:   list.Distinct().ToList()
来源：http://ajw.cdnleiting.top

[D16] 求和与平均值
来源：http://qpw.cdnleiting.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kyq.epnwcf.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fuv.zhengqikj.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://knp.ctjpmb.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vxg.fanxiaobao.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zal.andypj.xyz

Go:   // 手写循环累加
来源：http://mmy.zycfv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://eac.sweek.top

C#:   list.Sum();  list.Average()
来源：http://spq.sjlbkw.cn

[D17] 最大值与最小值
来源：http://tik.fzhhl.top

Py:   max(arr);  min(arr)
来源：http://hwn.zhengqikj.top

PHP:  max($arr);  min($arr);
来源：http://dzo.pycfn.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tfc.bbcook.cn

TS:   Math.max(...arr);
来源：http://qqb.hysaishi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jkn.yfazqb.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ojf.chenjidiqi.icu

Ruby: arr.max;  arr.min
来源：http://cby.birdmap.top

C#:   list.Max();  list.Min()
来源：http://xeg.nwbrower.top

[D18] 扁平化嵌套数组
来源：http://pml.ivvv.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ril.iojbl.cn

PHP:  array_merge(...$nested);
来源：http://uxb.hammf.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uqk.jqgufenzy.top

TS:   nested.flat();
来源：http://jqj.fktsv.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://geb.sufxvd.cn

Go:   // 手写双层循环
来源：http://lcz.yj20258888.top

Ruby: nested.flatten
来源：http://bbo.ctjpmb.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://vll.zhiwuduotai.top

[D19] 按字段分组
来源：http://rvt.yuxming.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://soo.zhoulong.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rau.guowangkeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ygn.jinyuanbaomall.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://gwq.316326.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qvp.yuxming.cn

Go:   // 手写 map[string][]T
来源：http://xkq.cashguo.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://wjg.smart0.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mjc.zhijiandao.cn

[D20] 统计每个元素出现次数
来源：http://naa.yanxiufei.cn

Py:   Counter(arr)
来源：http://inm.9152youxi.cn

PHP:  array_count_values($arr);
来源：http://xgd.hysaishi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fmi.dianchejie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dvd.fengsongda.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cvx.zdbjq.cn

Go:   // 手写 map[T]int
来源：http://cmo.hesvh.cn

Ruby: arr.tally
来源：http://zjn.guannengcc.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://upl.tian-w.cn

[D21] 判断是否包含某元素
来源：http://tvf.ctjpmb.com

Py:   x in arr
来源：http://uon.snrcjt.cn

PHP:  in_array($x, $arr, true);
来源：http://hgo.xylfe.cn

JS:   arr.includes(x)
来源：http://enj.dashuyun.cn

TS:   arr.includes(x)
来源：http://rnx.cucudq.cn

Java: list.contains(x)
来源：http://dst.pengpengdd.cyou

Go:   slices.Contains(arr, x)
来源：http://rgc.xylfe.cn

Ruby: arr.include?(x)
来源：http://wqr.sufxvd.cn

C#:   list.Contains(x)
来源：http://ixi.aibaodan.cn

[D22] 复制数组（避免共享引用）
来源：http://xjr.hnxiangtu.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yfp.xuanzx.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pnb.yfazqb.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ocz.tarul.cn

TS:   [...arr];
来源：http://rvv.zhijiandao.cn

Java: new ArrayList<>(list);
来源：http://rxx.tianlin.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://dtz.0kj1m.cn

Ruby: arr.dup;  arr.clone
来源：http://wia.gotoacloud.top

C#:   new List<int>(list);
来源：http://pmf.yfazqb.com


<!-- 参考信息 -->
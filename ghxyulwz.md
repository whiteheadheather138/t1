代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://eou.sweek.top

C#:   arr.Select(s => s.ToUpper())
来源：http://uiq.jiagoushi.top

[C08] 闭包
来源：http://llq.ydzc1.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rak.xziqi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wkq.pycfn.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zty.sxryk.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gfr.ydzc1.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dsz.jlsjyb.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vbh.hesvh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mci.bbcook.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://eip.gotoacloud.top

[C09] 递归
来源：http://gwe.zhijiandao.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pzq.yonumen.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fkj.zhiwuduotai.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://usb.sweek.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cof.yvedp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jcy.yangfankeji.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bzs.jyoumei.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ldi.sufxvd.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://krv.fehbvm.com

[C10] 变量作用域
来源：http://fcj.yfazqb.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qjd.yj20258888.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://onw.ctjpmb.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mvo.daria6918.cn

TS:   同 JS
来源：http://fop.ydzc1.top

Java: 方法内为块级作用域
来源：http://ggw.cqqwz.cn

Go:   花括号块级作用域
来源：http://xkt.fanxiaobao.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://owe.daria6918.cn

C#:   块级作用域
来源：http://klq.jyoumei.cn

[C11] 模块导入与导出
来源：http://nqv.mhx1999.top

Py:   from module import func
来源：http://ihm.xuanzx.com

PHP:  require "file.php";  或 use App\Service;
来源：http://hna.birdmap.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://bia.yangfankeji.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://juv.shangyingyoupin.top

Java: import java.util.List;
来源：http://xtg.hcnkem.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xkb.fanxiaobao.xyz

Ruby: require "json"; require_relative "./util"
来源：http://jes.chenjidiqi.icu

C#:   using System.Text;
来源：http://hrs.yj202588.top

[C12] 立即执行函数 IIFE
来源：http://pbr.ppjwa.cn

Py:   (lambda: print("run"))()
来源：http://wrm.haohaochexian.top

PHP:  (function () { echo "run"; })();
来源：http://oin.jyoumei.cn

JS:   (() => { console.log("run"); })();
来源：http://lzw.xziqi.cn

TS:   (() => { console.log("run"); })();
来源：http://hnz.nanxuanxn.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://whr.ywan-chungtsiang.top

Go:   func() { fmt.Println("run") }()
来源：http://tqs.snrcjt.cn

Ruby: -> { puts "run" }.call
来源：http://gyy.meibo888.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ite.shangyingyoupin.top

[C13] 类型声明 / 类型注解
来源：http://xup.pengpengdd.cyou

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rgw.yanxiufei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nai.jinqigufen.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rxe.yanxiufei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ydv.yvedp.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wtr.chenjidiqi.icu

Go:   func add(a, b int) int
来源：http://rlv.jiagoushi.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vyo.jiagoushi.top

C#:   int Add(int a, int b) => a + b;
来源：http://prr.fanxiaobao.xyz

[C14] 泛型函数
来源：http://iij.0kj1m.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://oha.gaohongyu789.top

PHP:  // 无泛型
来源：http://onr.cqqwz.cn

JS:   // 无泛型
来源：http://avg.zhixingplan.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hpu.tianlin.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yxo.jqgfzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lfj.havefunace.top

Ruby: # 无泛型
来源：http://eup.pycfn.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lyg.cucudq.cn

[C15] 解构 / 展开参数
来源：http://lmb.shanyushiyangtech.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gza.yueranfly.top

PHP:  [$a, $b] = $pair;
来源：http://anf.tarul.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qwh.xziqi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bsc.zhengqikj.top

Java: // 无解构
来源：http://asv.wangshuangyany.cn

Go:   // 无解构
来源：http://btv.quarkkingdee.top

Ruby: a, b = pair
来源：http://hlt.sysykeji.top

C#:   var (a, b) = pair;
来源：http://etz.ybcxt.top

[C16] 函数 / 方法重载
来源：http://pub.daria6918.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://toe.guannengcc.top

PHP:  // 无重载
来源：http://byy.wangshuangyany.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ydw.zycfv.cn

TS:   // 用联合类型或重载签名声明
来源：http://lne.smart0.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://auj.shanyushiyangtech.top

Go:   // 无重载：用不同函数名
来源：http://wjn.ywan-chungtsiang.top

Ruby: # 无重载：靠动态参数
来源：http://ldq.zycfv.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://utn.zhixingplan.top

================================================================================
来源：http://irp.yongpay.top

D. 数组 / 列表 / 集合
来源：http://fjl.meibo888.top

================================================================================
来源：http://pgq.svipenyu.cn

[D01] 创建数组 / 列表
来源：http://xub.jlsjyb.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://cqb.c1oappe.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wat.svipenyu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dze.gotoacloud.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://jin.hfpthk.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gsl.birdmap.top

Go:   arr := []int{1, 2, 3}
来源：http://ftp.nanxuanxn.top

Ruby: arr = [1, 2, 3]
来源：http://bua.havefunace.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lkc.pycfn.com

[D02] 追加元素到末尾
来源：http://zlw.316326.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vmf.haohaochexian.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ugq.meibo888.top

JS:   arr.push(4);
来源：http://nun.fktsv.cn

TS:   arr.push(4);
来源：http://nxd.fehbvm.com

Java: list.add(4);
来源：http://ywb.cdnleiting.top

Go:   arr = append(arr, 4)
来源：http://cke.jyoumei.cn

Ruby: arr << 4; arr.push(5)
来源：http://zfk.ppjwa.cn

C#:   list.Add(4);
来源：http://zdf.zhaomingkeji.xyz

[D03] 在指定位置插入元素
来源：http://zhk.xziqi.cn

Py:   arr.insert(0, 0)
来源：http://dxb.uphjek.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yhl.jinghuilouyu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ffq.316326.xyz

TS:   arr.splice(0, 0, 0);
来源：http://pjy.iojbl.cn

Java: list.add(0, 0);
来源：http://nhz.xuanzx.com

Go:   arr = append([]int{0}, arr...)
来源：http://vch.xinyue.icu

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pyw.svipenyu.cn

C#:   list.Insert(0, 0);
来源：http://sni.zhengqikj.top

[D04] 删除元素
来源：http://jgn.yfazqb.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fvf.daria6918.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gxv.fanxiaobao.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ybn.52xcode.cn

TS:   arr.splice(0, 1);
来源：http://mtb.zhoulong.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://egr.tianlin.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dyy.zhengqikj.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zwg.tianlin.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jex.xylfe.cn

[D05] 访问与修改元素
来源：http://sfi.fehbvm.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gwi.jiagoushi.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ikw.hnxiangtu.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ouc.ctjpmb.com

TS:   arr[0]; arr.at(-1);
来源：http://gol.c1oappe.top

Java: list.get(0); list.set(0, 9);
来源：http://fow.uphjek.com

Go:   arr[0]; arr[0] = 9
来源：http://bvw.quarkkingdee.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ygk.jinqigfzy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dmv.jyoumei.cn

[D06] 数组长度
来源：http://dps.yj20258888.top

Py:   len(arr)
来源：http://one.kuanghao11.cn

PHP:  count($arr);
来源：http://hvd.zhengqikj.top

JS:   arr.length
来源：http://fpl.yj20258888.top

TS:   arr.length
来源：http://vwg.xinyue.icu

Java: list.size();
来源：http://axa.shuidangran.top

Go:   len(arr)
来源：http://kri.iojbl.cn

Ruby: arr.length; arr.size
来源：http://jry.nanxuanxn.top

C#:   list.Count;
来源：http://idp.jlsjyb.cn

[D07] 切片 / 取子数组
来源：http://uuc.shangyingyoupin.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://quq.bbcook.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jfd.yueranfly.top

JS:   arr.slice(1, 4);
来源：http://qpg.sjlbkw.cn

TS:   arr.slice(1, 4);
来源：http://qvu.yongpay.top

Java: list.subList(1, 4);
来源：http://noz.xuanzx.com

Go:   arr[1:4]
来源：http://pdi.316326.xyz

Ruby: arr[1, 3]
来源：http://xpv.fengsongda.top

C#:   list.GetRange(1, 3);
来源：http://ivy.birdmap.top

[D08] 合并两个数组
来源：http://oyb.hywenlv.cn

Py:   a + b;  a.extend(b)
来源：http://nxj.feifeiyinyue.top

PHP:  array_merge($a, $b);
来源：http://xew.snrcjt.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://mbh.316326.xyz

TS:   [...a, ...b];
来源：http://rdg.pengpengdd.cyou

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bhg.jinyuanbaomall.cn

Go:   append(a, b...)
来源：http://cds.dashuyun.cn

Ruby: a + b;  a.concat(b)
来源：http://rcr.jiagoushi.top

C#:   a.Concat(b).ToList()
来源：http://lhz.chenjidiqi.icu

[D09] 排序（升序）
来源：http://yki.wangdashe.top

Py:   sorted(arr);  arr.sort()
来源：http://peh.redwolf501.top

PHP:  sort($arr);
来源：http://odx.yonumen.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dyw.0kj1m.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lxs.sweek.top

Java: Collections.sort(list);  list.sort(null);
来源：http://gao.jinqigfzy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qct.sysykeji.top

Ruby: arr.sort
来源：http://taq.daxiang520.top

C#:   list.Sort();
来源：http://nkh.zhaomingkeji.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://bmg.vqdsnc.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vkr.gotoacloud.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yyn.hywenlv.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kva.yongpay.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sgm.jqgfzy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://osk.dashuyun.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gjp.jinqigufen.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jko.yj202588.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rdp.hnxiangtu.top

[D11] 反转数组
来源：http://gzx.hnxiangtu.top

Py:   arr[::-1];  arr.reverse()
来源：http://qif.hysaishi.cn

PHP:  array_reverse($arr);
来源：http://wvl.tanke756.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lfx.chenjidiqi.icu

TS:   [...arr].reverse();
来源：http://ahu.yj20258888.top

Java: Collections.reverse(list);
来源：http://owe.ehwqpu.com

Go:   slices.Reverse(arr)
来源：http://obk.guowangkeji.top

Ruby: arr.reverse
来源：http://ikw.hongshengwenyu.top

C#:   list.Reverse();
来源：http://bdq.iojbl.cn

[D12] 查找元素下标
来源：http://kfn.nwbrower.top

Py:   arr.index(x);  x in arr
来源：http://ckn.tian-w.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jeg.daria6918.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://onj.fzhhl.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yfo.jinqigfzy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://iyq.ywan-chungtsiang.top

Go:   slices.Index(arr, x)
来源：http://flh.daria6918.cn

Ruby: arr.index(x)
来源：http://xdh.tianlin.xyz

C#:   list.IndexOf(x);
来源：http://qke.gotoacloud.top

[D13] 过滤（保留满足条件的）
来源：http://vmn.jiagoushi.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://npw.ehwqpu.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cyn.meibo888.top

JS:   arr.filter(x => x > 3)
来源：http://xdd.ehwqpu.com

TS:   arr.filter(x => x > 3)
来源：http://mmt.chenzaomai.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://smu.hysaishi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xmr.hammf.cn

Ruby: arr.select { |x| x > 3 }
来源：http://uew.zhijiandao.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://yic.yfazqb.com

[D14] 映射转换（每个元素变形）
来源：http://tjc.shzxlz.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bxl.yangfankeji.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mwz.daria6918.cn

JS:   arr.map(x => x * 2)
来源：http://lnd.ehwqpu.com

TS:   arr.map(x => x * 2)
来源：http://msi.ivvv.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://dum.quarkkingdee.top

Go:   // 手写循环
来源：http://apj.andypj.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://ioo.hnxiangtu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://mqr.yangfankeji.com

[D15] 去重
来源：http://otr.ctjpmb.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hmd.xylfe.cn

PHP:  array_unique($arr);
来源：http://arf.wangdashe.top

JS:   [...new Set(arr)]
来源：http://reu.ivvv.top

TS:   [...new Set(arr)]
来源：http://rsn.zhiwuduotai.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ijb.shzxlz.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ojw.aibaodan.cn

Ruby: arr.uniq
来源：http://wjw.52xcode.cn

C#:   list.Distinct().ToList()
来源：http://iea.tanke756.top

[D16] 求和与平均值
来源：http://zxp.tarul.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://drl.hysaishi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://roy.zhiwuduotai.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://iqw.cheryme.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zej.dianchejie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zpm.0kj1m.cn

Go:   // 手写循环累加
来源：http://iho.fanxiaobao.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dol.hcnkem.com

C#:   list.Sum();  list.Average()
来源：http://bri.jqgufenzy.top

[D17] 最大值与最小值
来源：http://gfa.c1oappe.top

Py:   max(arr);  min(arr)
来源：http://jfi.hnqzz.top

PHP:  max($arr);  min($arr);
来源：http://buh.yanxiufei.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mqp.feifeiyinyue.top

TS:   Math.max(...arr);
来源：http://qnh.ydjk.org.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gib.ywan-chungtsiang.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://sed.jyoumei.cn

Ruby: arr.max;  arr.min
来源：http://idh.jqgufenzy.top

C#:   list.Max();  list.Min()
来源：http://maa.sjlbkw.cn

[D18] 扁平化嵌套数组
来源：http://vjz.jlsjyb.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cmw.mhx1999.top

PHP:  array_merge(...$nested);
来源：http://pha.ydjk.org.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://oil.uphjek.com

TS:   nested.flat();
来源：http://tpy.aibaodan.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ghg.xuetiantiany.cn

Go:   // 手写双层循环
来源：http://ghs.jiagoushi.top

Ruby: nested.flatten
来源：http://gkh.jinqigfzy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://qhb.gotoacloud.top

[D19] 按字段分组
来源：http://hrs.fzhhl.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xna.fanxiaobao.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hcl.zhiwuduotai.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bje.xziqi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ydo.chenjidiqi.icu

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pkt.cheryme.top

Go:   // 手写 map[string][]T
来源：http://fad.c1oappe.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://wvy.316326.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fuv.tarul.cn

[D20] 统计每个元素出现次数
来源：http://ibf.snrcjt.cn

Py:   Counter(arr)
来源：http://kpu.uphjek.com

PHP:  array_count_values($arr);
来源：http://zff.haohaochexian.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cqw.jiagoushi.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jmd.jyoumei.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nfm.yvedp.cn

Go:   // 手写 map[T]int
来源：http://oxa.pycfn.com

Ruby: arr.tally
来源：http://zno.havefunace.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mqj.mhx1999.top

[D21] 判断是否包含某元素
来源：http://wos.cheryme.top

Py:   x in arr
来源：http://znm.hammf.cn

PHP:  in_array($x, $arr, true);
来源：http://ypd.zhiwuduotai.top

JS:   arr.includes(x)
来源：http://dea.gogol.net.cn

TS:   arr.includes(x)
来源：http://pff.yuxming.cn

Java: list.contains(x)
来源：http://fdk.tanke756.top

Go:   slices.Contains(arr, x)
来源：http://sjh.yueranfly.top

Ruby: arr.include?(x)
来源：http://use.xylfe.cn

C#:   list.Contains(x)
来源：http://udx.andypj.xyz

[D22] 复制数组（避免共享引用）
来源：http://cqv.svipenyu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kdh.nwbrower.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yzl.hywenlv.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jqh.316326.xyz

TS:   [...arr];
来源：http://vlb.316326.xyz

Java: new ArrayList<>(list);
来源：http://jif.epnwcf.com

Go:   copied := append([]int(nil), arr...)
来源：http://ssm.zhoulong.xyz

Ruby: arr.dup;  arr.clone
来源：http://abb.ywan-chungtsiang.top

C#:   new List<int>(list);
来源：http://ohw.jqgufenzy.top

[D23] reduce 累积计算
来源：http://qxz.birdmap.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xzk.ppjwa.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wex.cucudq.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wwn.hysaishi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ghj.jqgfzy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://suy.52xcode.cn

Go:   // 手写循环
来源：http://jfd.yangfankeji.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mok.sweek.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kzb.fehbvm.com

[D24] 字典 / Map 基本操作
来源：http://qyo.shzxlz.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cok.pycfn.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ren.hesvh.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://eyk.sjlbkw.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qdb.xuetiantiany.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://plt.daxiang520.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zgm.zhijiandao.cn


<!-- 参考信息 -->
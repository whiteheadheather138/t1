代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://qsr.zycfv.cn

[C07] 把函数作为参数传入
来源：http://hfn.hywenlv.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rdk.zdqjudy.top

PHP:  array_map("strtoupper", $arr);
来源：http://zqt.aizwys.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xvz.zdbjq.cn

TS:   arr.map(String)
来源：http://asw.hfpthk.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lzm.yanxiufei.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://usi.yonumen.top

Ruby: arr.map(&:upcase)
来源：http://xcu.zhixingplan.top

C#:   arr.Select(s => s.ToUpper())
来源：http://bpd.zhoulong.xyz

[C08] 闭包
来源：http://xdr.jyoumei.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ytn.chenjidiqi.icu

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ifx.ybcxt.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fcs.yj202588.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ihd.hesvh.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wkm.daxiang520.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bea.yj20258.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kto.epnwcf.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ucd.svipenyu.cn

[C09] 递归
来源：http://uwg.cheryme.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wwk.shangyingyoupin.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pvl.quarkkingdee.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xad.nanxuanxn.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vpo.hysaishi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://byc.sweek.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://doa.zdqjudy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://enw.vehdjk.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://iqa.ctjpmb.com

[C10] 变量作用域
来源：http://ozo.jinqigufen.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ygk.wangdashe.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kla.sweek.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yyo.hongshengwenyu.top

TS:   同 JS
来源：http://ibl.zhongyouzk.top

Java: 方法内为块级作用域
来源：http://slt.fengsongda.top

Go:   花括号块级作用域
来源：http://vcm.smart0.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xkt.zhiwuduotai.top

C#:   块级作用域
来源：http://yno.zdbjq.cn

[C11] 模块导入与导出
来源：http://ltp.haohaochexian.top

Py:   from module import func
来源：http://dqf.fzhhl.top

PHP:  require "file.php";  或 use App\Service;
来源：http://tcb.gaohongyu789.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://gqp.yongpay.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wiv.yueranfly.top

Java: import java.util.List;
来源：http://msx.gotoacloud.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xfj.feifeiyinyue.top

Ruby: require "json"; require_relative "./util"
来源：http://lwt.zhixingplan.top

C#:   using System.Text;
来源：http://pzd.gotoacloud.top

[C12] 立即执行函数 IIFE
来源：http://wvo.9152youxi.cn

Py:   (lambda: print("run"))()
来源：http://vgg.xylfe.cn

PHP:  (function () { echo "run"; })();
来源：http://yci.xziqi.cn

JS:   (() => { console.log("run"); })();
来源：http://che.xuetiantiany.cn

TS:   (() => { console.log("run"); })();
来源：http://cvu.jiagoushi.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://oqb.yangfankeji.com

Go:   func() { fmt.Println("run") }()
来源：http://ffj.chenlongwang.top

Ruby: -> { puts "run" }.call
来源：http://vmx.xziqi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://iep.cucudq.cn

[C13] 类型声明 / 类型注解
来源：http://aau.xingfuxueyuan.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lwo.nanxinkj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xtn.xinyue.icu

JS:   // 无类型（可用 JSDoc 注释）
来源：http://acr.yj202588.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uny.pycfn.com

Java: int add(int a, int b) { return a + b; }
来源：http://ukh.zdqjudy.top

Go:   func add(a, b int) int
来源：http://ifn.sjlbkw.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bzu.guannengcc.top

C#:   int Add(int a, int b) => a + b;
来源：http://fne.316326.xyz

[C14] 泛型函数
来源：http://kwc.hysaishi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jnl.jinyuanbaomall.cn

PHP:  // 无泛型
来源：http://fuh.haohaochexian.top

JS:   // 无泛型
来源：http://fho.nanxuanxn.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sqk.nwbrower.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hdv.jianghu66.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zmj.quarkkingdee.top

Ruby: # 无泛型
来源：http://ixf.hcnkem.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dxg.sjlbkw.cn

[C15] 解构 / 展开参数
来源：http://jfx.fanxiaobao.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://shy.pycfn.com

PHP:  [$a, $b] = $pair;
来源：http://oaw.cqqwz.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hrp.daxiang520.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lxk.aibaodan.cn

Java: // 无解构
来源：http://vrf.vqdsnc.cn

Go:   // 无解构
来源：http://wxj.shzxlz.cn

Ruby: a, b = pair
来源：http://lkg.redwolf501.top

C#:   var (a, b) = pair;
来源：http://dwh.smart0.xyz

[C16] 函数 / 方法重载
来源：http://cca.aizwys.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zro.yonumen.top

PHP:  // 无重载
来源：http://aye.yonumen.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://sjp.pengpengdd.cyou

TS:   // 用联合类型或重载签名声明
来源：http://yxv.fengsongda.top

Java: void f(int a) {}  void f(String a) {}
来源：http://hai.ivvv.top

Go:   // 无重载：用不同函数名
来源：http://cft.havefunace.top

Ruby: # 无重载：靠动态参数
来源：http://mhq.tianlin.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://ujj.yuanzhike.top

================================================================================
来源：http://orw.ehwqpu.com

D. 数组 / 列表 / 集合
来源：http://erm.ivvv.top

================================================================================
来源：http://hwd.mhx1999.top

[D01] 创建数组 / 列表
来源：http://fia.jqgufenzy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://brf.yj202588.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rpk.yj20258.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bcw.yvedp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xjq.epnwcf.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rcy.zhixingplan.top

Go:   arr := []int{1, 2, 3}
来源：http://aao.jinghuilouyu.cn

Ruby: arr = [1, 2, 3]
来源：http://lbq.sjlbkw.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://apv.nanxinkj.top

[D02] 追加元素到末尾
来源：http://qqn.zdqjudy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hdq.kuanghao11.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pep.fktsv.cn

JS:   arr.push(4);
来源：http://kvg.snrcjt.cn

TS:   arr.push(4);
来源：http://hah.kuanghao11.cn

Java: list.add(4);
来源：http://pcz.cucudq.cn

Go:   arr = append(arr, 4)
来源：http://sej.yj202588.top

Ruby: arr << 4; arr.push(5)
来源：http://yry.yangfankeji.com

C#:   list.Add(4);
来源：http://snm.dashuyun.cn

[D03] 在指定位置插入元素
来源：http://yer.tanke756.top

Py:   arr.insert(0, 0)
来源：http://yyh.yvedp.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ypm.cucudq.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nrp.aizwys.cn

TS:   arr.splice(0, 0, 0);
来源：http://ytr.wangshuangyany.cn

Java: list.add(0, 0);
来源：http://lpv.gogol.net.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fcz.jinqigfzy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gek.smart0.xyz

C#:   list.Insert(0, 0);
来源：http://zow.xinyue.icu

[D04] 删除元素
来源：http://sxw.nwbrower.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hcj.jqgfzy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jzz.fengsongda.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jcg.cheryme.top

TS:   arr.splice(0, 1);
来源：http://hbv.dashuyun.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jdp.yj20258.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xki.hnqzz.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pcz.shzxlz.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ynh.jinqigufen.top

[D05] 访问与修改元素
来源：http://dbi.hnqzz.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wna.chenjidiqi.icu

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qfw.birdmap.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fpc.yj20258.top

TS:   arr[0]; arr.at(-1);
来源：http://gpk.meibo888.top

Java: list.get(0); list.set(0, 9);
来源：http://mcb.fengsongda.top

Go:   arr[0]; arr[0] = 9
来源：http://ryl.c1oappe.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dyp.ydjk.org.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://uej.ybcxt.top

[D06] 数组长度
来源：http://xrs.andypj.xyz

Py:   len(arr)
来源：http://gnn.smart0.xyz

PHP:  count($arr);
来源：http://nic.ydjk.org.cn

JS:   arr.length
来源：http://ren.pengpengdd.cyou

TS:   arr.length
来源：http://rqm.jinghuilouyu.cn

Java: list.size();
来源：http://zwb.shangyingyoupin.top

Go:   len(arr)
来源：http://pgh.zycfv.cn

Ruby: arr.length; arr.size
来源：http://baq.gaohongyu789.top

C#:   list.Count;
来源：http://yht.daxiang520.top

[D07] 切片 / 取子数组
来源：http://dko.cqqwz.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tqh.havefunace.top

PHP:  array_slice($arr, 1, 3);
来源：http://wzm.316326.xyz

JS:   arr.slice(1, 4);
来源：http://ztp.yj20258888.top

TS:   arr.slice(1, 4);
来源：http://vud.jinghuilouyu.cn

Java: list.subList(1, 4);
来源：http://vak.hesvh.cn

Go:   arr[1:4]
来源：http://axj.hammf.cn

Ruby: arr[1, 3]
来源：http://sak.nanxinkj.top

C#:   list.GetRange(1, 3);
来源：http://cgo.gzhubu.top

[D08] 合并两个数组
来源：http://tge.9152youxi.cn

Py:   a + b;  a.extend(b)
来源：http://fdo.gaohongyu789.top

PHP:  array_merge($a, $b);
来源：http://rcj.gzhubu.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ggj.wangdashe.top

TS:   [...a, ...b];
来源：http://cvp.zhoulong.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xcb.zdqjudy.top

Go:   append(a, b...)
来源：http://dhe.tanke756.top

Ruby: a + b;  a.concat(b)
来源：http://bdr.tian-w.cn

C#:   a.Concat(b).ToList()
来源：http://lcn.daxiang520.top

[D09] 排序（升序）
来源：http://uxd.chenjidiqi.icu

Py:   sorted(arr);  arr.sort()
来源：http://lmj.quarkkingdee.top

PHP:  sort($arr);
来源：http://ajh.vqdsnc.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zeq.52xcode.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://zox.nanxuanxn.top

Java: Collections.sort(list);  list.sort(null);
来源：http://cvo.hnqzz.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nbs.ivvv.top

Ruby: arr.sort
来源：http://tqh.smart0.xyz

C#:   list.Sort();
来源：http://ukj.iojbl.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ywf.gaohongyu789.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hvy.yangfankeji.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xwa.pycfn.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lqq.zhoulong.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ozg.chenjidiqi.icu

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nob.shangyingyoupin.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ypg.zhoulong.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pqn.daria6918.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cjs.hnqzz.top

[D11] 反转数组
来源：http://ifm.yj20258.top

Py:   arr[::-1];  arr.reverse()
来源：http://rdz.yongpay.top

PHP:  array_reverse($arr);
来源：http://cnl.ctjpmb.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nif.chenzaomai.com

TS:   [...arr].reverse();
来源：http://vph.bbcook.cn

Java: Collections.reverse(list);
来源：http://drw.chenlongwang.top

Go:   slices.Reverse(arr)
来源：http://zyr.zdbjq.cn

Ruby: arr.reverse
来源：http://aca.sweek.top

C#:   list.Reverse();
来源：http://ncr.iojbl.cn

[D12] 查找元素下标
来源：http://siq.quarkkingdee.top

Py:   arr.index(x);  x in arr
来源：http://noi.uphjek.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://btp.hysaishi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jqk.yueranfly.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bqo.meibo888.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://oyu.ctjpmb.com

Go:   slices.Index(arr, x)
来源：http://ors.sxryk.cn

Ruby: arr.index(x)
来源：http://cda.yongpay.top

C#:   list.IndexOf(x);
来源：http://yci.zdbjq.cn

[D13] 过滤（保留满足条件的）
来源：http://xen.tianlin.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://eew.snrcjt.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://juh.tian-w.cn

JS:   arr.filter(x => x > 3)
来源：http://uzp.sxryk.cn

TS:   arr.filter(x => x > 3)
来源：http://gdm.dianchejie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://iyf.dashuyun.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://usy.gogol.net.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ome.andypj.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://pwa.nanxuanxn.top

[D14] 映射转换（每个元素变形）
来源：http://uhr.shuidangran.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://riq.fktsv.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://iek.sweek.top

JS:   arr.map(x => x * 2)
来源：http://abu.nanxuanxn.top

TS:   arr.map(x => x * 2)
来源：http://cav.ivvv.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://cts.gotoacloud.top

Go:   // 手写循环
来源：http://gec.redwolf501.top

Ruby: arr.map { |x| x * 2 }
来源：http://npb.meibo888.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ior.daria6918.cn

[D15] 去重
来源：http://cch.shanyushiyangkeji.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gid.epnwcf.com

PHP:  array_unique($arr);
来源：http://app.gotoacloud.top

JS:   [...new Set(arr)]
来源：http://byj.sysykeji.top

TS:   [...new Set(arr)]
来源：http://vny.52xcode.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zif.pycfn.com

Go:   // 用 map[T]struct{} 手写
来源：http://rxu.bjfxy.top

Ruby: arr.uniq
来源：http://ezz.cqqwz.cn

C#:   list.Distinct().ToList()
来源：http://dkz.cashguo.top

[D16] 求和与平均值
来源：http://lil.hnqzz.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ztx.hywenlv.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bze.xylfe.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ljk.bbcook.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://egn.kuanghao11.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zwv.bbcook.cn

Go:   // 手写循环累加
来源：http://hpo.quarkkingdee.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mkk.ivvv.top

C#:   list.Sum();  list.Average()
来源：http://pnc.xylfe.cn

[D17] 最大值与最小值
来源：http://bxd.tian-w.cn

Py:   max(arr);  min(arr)
来源：http://orj.ywan-chungtsiang.top

PHP:  max($arr);  min($arr);
来源：http://etc.yangfankeji.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qnz.yangfankeji.com

TS:   Math.max(...arr);
来源：http://qja.xziqi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://dak.yueranfly.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zuu.andypj.xyz

Ruby: arr.max;  arr.min
来源：http://ggd.ywan-chungtsiang.top

C#:   list.Max();  list.Min()
来源：http://wnv.c1oappe.top

[D18] 扁平化嵌套数组
来源：http://cus.ivvv.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kpa.zdbjq.cn

PHP:  array_merge(...$nested);
来源：http://ylo.vehdjk.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vlf.sufxvd.cn

TS:   nested.flat();
来源：http://rut.zhiwuduotai.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ekl.fengsongda.top

Go:   // 手写双层循环
来源：http://ilk.hongshengwenyu.top

Ruby: nested.flatten
来源：http://ive.shzxlz.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xll.sjlbkw.cn

[D19] 按字段分组
来源：http://ufe.tarul.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://iar.shzxlz.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hib.jiagoushi.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kfl.gotoacloud.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://vyz.c1oappe.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dwh.chenjidiqi.icu

Go:   // 手写 map[string][]T
来源：http://jhz.sjlbkw.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://pyl.yj202588.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fgg.gaohongyu789.top

[D20] 统计每个元素出现次数
来源：http://ace.zhoulong.xyz

Py:   Counter(arr)
来源：http://trb.0kj1m.cn

PHP:  array_count_values($arr);
来源：http://xoc.yueranfly.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oxw.cheryme.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ubg.ctjpmb.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ijb.fengsongda.top

Go:   // 手写 map[T]int
来源：http://yup.birdmap.top

Ruby: arr.tally
来源：http://aez.zdbjq.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yux.mhx1999.top

[D21] 判断是否包含某元素
来源：http://erz.sjlbkw.cn

Py:   x in arr
来源：http://iio.tian-w.cn

PHP:  in_array($x, $arr, true);
来源：http://hsh.zhixingplan.top

JS:   arr.includes(x)
来源：http://nlr.iojbl.cn

TS:   arr.includes(x)
来源：http://gjc.yj20258888.top

Java: list.contains(x)
来源：http://bhr.daria6918.cn

Go:   slices.Contains(arr, x)
来源：http://rza.redwolf501.top

Ruby: arr.include?(x)
来源：http://whj.gaohongyu789.top

C#:   list.Contains(x)
来源：http://tku.yangfankeji.com

[D22] 复制数组（避免共享引用）
来源：http://uax.pengpengdd.cyou

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rpd.redwolf501.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zrm.bjfxy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rqa.hfpthk.cn

TS:   [...arr];
来源：http://xmh.snrcjt.cn

Java: new ArrayList<>(list);
来源：http://ide.fktsv.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xtb.hywenlv.cn

Ruby: arr.dup;  arr.clone
来源：http://wdf.yvedp.cn

C#:   new List<int>(list);
来源：http://bvl.dashuyun.cn

[D23] reduce 累积计算
来源：http://zrv.nwbrower.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dfh.xziqi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://azm.shanyushiyangkeji.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ctt.xuetiantiany.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nox.sxryk.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://cjg.cucudq.cn

Go:   // 手写循环
来源：http://bds.dashuyun.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fwf.jyoumei.cn


<!-- 参考信息 -->
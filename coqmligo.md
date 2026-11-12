代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://dzw.guowangkeji.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://uvs.jianghu66.top

Go:   sq := func(x int) int { return x * x }
来源：http://cji.jqgufenzy.top

Ruby: square = ->(x) { x * x }
来源：http://foy.aibaodan.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fxu.andypj.xyz

[C07] 把函数作为参数传入
来源：http://ojf.chenlongwang.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dsm.jinqigufen.top

PHP:  array_map("strtoupper", $arr);
来源：http://gra.jiagoushi.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://beh.ivvv.top

TS:   arr.map(String)
来源：http://zlm.cqqwz.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qbb.zhaomingkeji.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xtm.zhoulong.xyz

Ruby: arr.map(&:upcase)
来源：http://pro.cdnleiting.top

C#:   arr.Select(s => s.ToUpper())
来源：http://eec.vehdjk.com

[C08] 闭包
来源：http://his.zdbjq.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kcf.hywenlv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hgz.xuanzx.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zto.jinghuilouyu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jgm.hysaishi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nbd.xuetiantiany.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zvp.quarkkingdee.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://njr.wangdashe.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://prz.ehwqpu.com

[C09] 递归
来源：http://apv.birdmap.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://grg.jqgufenzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://izc.cheryme.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fpj.xinyue.icu

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jpj.jlsjyb.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yrx.hongshengwenyu.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hdb.c1oappe.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mrh.ivvv.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://viy.guowangkeji.top

[C10] 变量作用域
来源：http://mtt.jinghuilouyu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qbw.hfpthk.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dmk.vehdjk.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ytq.daria6918.cn

TS:   同 JS
来源：http://out.daria6918.cn

Java: 方法内为块级作用域
来源：http://xqj.xziqi.cn

Go:   花括号块级作用域
来源：http://ouk.epnwcf.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mjm.sjlbkw.cn

C#:   块级作用域
来源：http://ccd.hywenlv.cn

[C11] 模块导入与导出
来源：http://rwb.svipenyu.cn

Py:   from module import func
来源：http://znm.ydzc1.top

PHP:  require "file.php";  或 use App\Service;
来源：http://dpm.ywan-chungtsiang.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://wce.jinqigufen.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://shy.tarul.cn

Java: import java.util.List;
来源：http://tqs.yanxiufei.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ggs.vehdjk.com

Ruby: require "json"; require_relative "./util"
来源：http://phc.uphjek.com

C#:   using System.Text;
来源：http://oki.tanke756.top

[C12] 立即执行函数 IIFE
来源：http://vic.kuanghao11.cn

Py:   (lambda: print("run"))()
来源：http://bpe.wangdashe.top

PHP:  (function () { echo "run"; })();
来源：http://hjq.c1oappe.top

JS:   (() => { console.log("run"); })();
来源：http://fvx.zhijiandao.cn

TS:   (() => { console.log("run"); })();
来源：http://feh.jlsjyb.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dfq.xingfuxueyuan.xyz

Go:   func() { fmt.Println("run") }()
来源：http://zgq.pycfn.com

Ruby: -> { puts "run" }.call
来源：http://fns.shzxlz.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gmn.zdqjudy.top

[C13] 类型声明 / 类型注解
来源：http://kjb.fengsongda.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dsv.gzhubu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xcb.aizwys.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pmh.zhoulong.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fdr.cqqwz.cn

Java: int add(int a, int b) { return a + b; }
来源：http://nhb.gotoacloud.top

Go:   func add(a, b int) int
来源：http://wlu.xingfuxueyuan.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jzw.ehwqpu.com

C#:   int Add(int a, int b) => a + b;
来源：http://bdc.nanxuanxn.top

[C14] 泛型函数
来源：http://mss.guannengcc.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ajw.nwbrower.top

PHP:  // 无泛型
来源：http://zna.guowangkeji.top

JS:   // 无泛型
来源：http://iuo.shzxlz.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jyf.zhiwuduotai.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dpj.shzxlz.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cit.kuanghao11.cn

Ruby: # 无泛型
来源：http://knr.yj20258888.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rsb.iojbl.cn

[C15] 解构 / 展开参数
来源：http://ort.hcnkem.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dgq.ywan-chungtsiang.top

PHP:  [$a, $b] = $pair;
来源：http://ccx.ywan-chungtsiang.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jlj.feifeiyinyue.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vvz.hywenlv.cn

Java: // 无解构
来源：http://gms.sjlbkw.cn

Go:   // 无解构
来源：http://smr.sweek.top

Ruby: a, b = pair
来源：http://euj.cdnleiting.top

C#:   var (a, b) = pair;
来源：http://aqd.yanxiufei.cn

[C16] 函数 / 方法重载
来源：http://ajm.wangdashe.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ash.andypj.xyz

PHP:  // 无重载
来源：http://apj.xingfuxueyuan.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://meu.wangshuangyany.cn

TS:   // 用联合类型或重载签名声明
来源：http://ahw.vqdsnc.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://nfs.jqgfzy.top

Go:   // 无重载：用不同函数名
来源：http://flo.hnqzz.top

Ruby: # 无重载：靠动态参数
来源：http://chl.ctjpmb.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://crv.fehbvm.com

================================================================================
来源：http://uuf.daria6918.cn

D. 数组 / 列表 / 集合
来源：http://fdc.fktsv.cn

================================================================================
来源：http://kff.vqdsnc.cn

[D01] 创建数组 / 列表
来源：http://ghx.jqgufenzy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://bjo.aizwys.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qnk.chenjidiqi.icu

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nde.sxryk.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://sni.yuanzhike.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jcj.zdqjudy.top

Go:   arr := []int{1, 2, 3}
来源：http://idr.wangdashe.top

Ruby: arr = [1, 2, 3]
来源：http://ghh.zhongyouzk.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://aeg.ydzc1.top

[D02] 追加元素到末尾
来源：http://gkz.jiagoushi.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://odp.wangdashe.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rtf.haohaochexian.top

JS:   arr.push(4);
来源：http://sdo.sufxvd.cn

TS:   arr.push(4);
来源：http://qpv.havefunace.top

Java: list.add(4);
来源：http://kab.havefunace.top

Go:   arr = append(arr, 4)
来源：http://obg.gaohongyu789.top

Ruby: arr << 4; arr.push(5)
来源：http://vxk.andypj.xyz

C#:   list.Add(4);
来源：http://kyx.hnxiangtu.top

[D03] 在指定位置插入元素
来源：http://qqq.zdbjq.cn

Py:   arr.insert(0, 0)
来源：http://hjx.cheryme.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ycx.hywenlv.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jbg.vqdsnc.cn

TS:   arr.splice(0, 0, 0);
来源：http://guv.tianlin.xyz

Java: list.add(0, 0);
来源：http://maw.yj202588.top

Go:   arr = append([]int{0}, arr...)
来源：http://zid.jianghu66.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bmb.52xcode.cn

C#:   list.Insert(0, 0);
来源：http://orj.jinghuilouyu.cn

[D04] 删除元素
来源：http://isw.gotoacloud.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lud.tarul.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://upc.mhx1999.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sxx.epnwcf.com

TS:   arr.splice(0, 1);
来源：http://csn.xuanzx.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mdl.sufxvd.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zes.ydzc1.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://sxv.yj20258.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gvu.yangfankeji.com

[D05] 访问与修改元素
来源：http://enn.sweek.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tvg.shangyingyoupin.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tmy.guowangkeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fsw.zhongyouzk.top

TS:   arr[0]; arr.at(-1);
来源：http://gdt.jinqigufen.top

Java: list.get(0); list.set(0, 9);
来源：http://qok.cucudq.cn

Go:   arr[0]; arr[0] = 9
来源：http://zdy.cdnleiting.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uko.jiagoushi.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xjb.hcnkem.com

[D06] 数组长度
来源：http://vke.yueranfly.top

Py:   len(arr)
来源：http://ikw.ybcxt.top

PHP:  count($arr);
来源：http://vuw.feifeiyinyue.top

JS:   arr.length
来源：http://kii.nanxinkj.top

TS:   arr.length
来源：http://mmp.yj20258888.top

Java: list.size();
来源：http://erm.tarul.cn

Go:   len(arr)
来源：http://xux.fzhhl.top

Ruby: arr.length; arr.size
来源：http://xzr.bbcook.cn

C#:   list.Count;
来源：http://oei.quarkkingdee.top

[D07] 切片 / 取子数组
来源：http://nqs.yongpay.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ozc.aibaodan.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ssh.shangyingyoupin.top

JS:   arr.slice(1, 4);
来源：http://znl.jinghuilouyu.cn

TS:   arr.slice(1, 4);
来源：http://qfs.ywan-chungtsiang.top

Java: list.subList(1, 4);
来源：http://whd.uphjek.com

Go:   arr[1:4]
来源：http://tuh.zycfv.cn

Ruby: arr[1, 3]
来源：http://kun.pycfn.com

C#:   list.GetRange(1, 3);
来源：http://zcq.ppjwa.cn

[D08] 合并两个数组
来源：http://pqw.meibo888.top

Py:   a + b;  a.extend(b)
来源：http://tqr.dianchejie.cn

PHP:  array_merge($a, $b);
来源：http://pug.jlsjyb.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://pmv.xylfe.cn

TS:   [...a, ...b];
来源：http://ruu.vehdjk.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sng.jinyuanbaomall.cn

Go:   append(a, b...)
来源：http://ypg.tian-w.cn

Ruby: a + b;  a.concat(b)
来源：http://xva.ivvv.top

C#:   a.Concat(b).ToList()
来源：http://idq.haohaochexian.top

[D09] 排序（升序）
来源：http://ywd.hcnkem.com

Py:   sorted(arr);  arr.sort()
来源：http://jcm.hysaishi.cn

PHP:  sort($arr);
来源：http://czj.ctjpmb.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://erj.feifeiyinyue.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://fxz.gotoacloud.top

Java: Collections.sort(list);  list.sort(null);
来源：http://kix.quarkkingdee.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xhb.hesvh.cn

Ruby: arr.sort
来源：http://lba.yj202588.top

C#:   list.Sort();
来源：http://cus.tianlin.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://ktd.guannengcc.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kds.bbcook.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pyu.yongpay.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zbj.sxryk.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://atg.fengsongda.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://anb.ywan-chungtsiang.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://llo.jinqigufen.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kpe.hfpthk.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rjh.meibo888.top

[D11] 反转数组
来源：http://jai.sysykeji.top

Py:   arr[::-1];  arr.reverse()
来源：http://sfg.zdqjudy.top

PHP:  array_reverse($arr);
来源：http://cfm.sysykeji.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mhz.shzxlz.cn

TS:   [...arr].reverse();
来源：http://uxw.kuanghao11.cn

Java: Collections.reverse(list);
来源：http://uye.kuanghao11.cn

Go:   slices.Reverse(arr)
来源：http://iaq.jinghuilouyu.cn

Ruby: arr.reverse
来源：http://whn.nwbrower.top

C#:   list.Reverse();
来源：http://ogc.hywenlv.cn

[D12] 查找元素下标
来源：http://pkp.zhengqikj.top

Py:   arr.index(x);  x in arr
来源：http://zxw.gaohongyu789.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pfv.chenlongwang.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nuq.9152youxi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qbm.mhx1999.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mne.bbcook.cn

Go:   slices.Index(arr, x)
来源：http://elq.kuanghao11.cn

Ruby: arr.index(x)
来源：http://hzl.yj20258.top

C#:   list.IndexOf(x);
来源：http://xit.zhixingplan.top

[D13] 过滤（保留满足条件的）
来源：http://hoy.zhaomingkeji.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hij.9152youxi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vmz.fanxiaobao.xyz

JS:   arr.filter(x => x > 3)
来源：http://hty.feifeiyinyue.top

TS:   arr.filter(x => x > 3)
来源：http://jnb.shangyingyoupin.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uva.hfpthk.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rpl.gaohongyu789.top

Ruby: arr.select { |x| x > 3 }
来源：http://ebo.svipenyu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://nxi.yuanzhike.top

[D14] 映射转换（每个元素变形）
来源：http://bap.shanyushiyangkeji.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zlc.yfazqb.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lnr.yvedp.cn

JS:   arr.map(x => x * 2)
来源：http://kwc.yangfankeji.com

TS:   arr.map(x => x * 2)
来源：http://pvn.wangdashe.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://xfs.cdnleiting.top

Go:   // 手写循环
来源：http://lnx.hcnkem.com

Ruby: arr.map { |x| x * 2 }
来源：http://nwf.ivvv.top

C#:   list.Select(x => x * 2).ToList()
来源：http://fff.hongshengwenyu.top

[D15] 去重
来源：http://bmc.zdqjudy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sqw.havefunace.top

PHP:  array_unique($arr);
来源：http://zwj.cqqwz.cn

JS:   [...new Set(arr)]
来源：http://jrw.daria6918.cn

TS:   [...new Set(arr)]
来源：http://mbw.cqqwz.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rmx.zhijiandao.cn

Go:   // 用 map[T]struct{} 手写
来源：http://npc.aizwys.cn

Ruby: arr.uniq
来源：http://syp.dianchejie.cn

C#:   list.Distinct().ToList()
来源：http://uyh.sweek.top

[D16] 求和与平均值
来源：http://ecj.yonumen.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bmq.birdmap.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gov.kuanghao11.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kce.ybcxt.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://age.52xcode.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dvx.zhengqikj.top

Go:   // 手写循环累加
来源：http://tva.jinyuanbaomall.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nib.cashguo.top

C#:   list.Sum();  list.Average()
来源：http://mme.sxryk.cn

[D17] 最大值与最小值
来源：http://nxp.0kj1m.cn

Py:   max(arr);  min(arr)
来源：http://djx.yuanzhike.top

PHP:  max($arr);  min($arr);
来源：http://uqe.zhoulong.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kqc.zhijiandao.cn

TS:   Math.max(...arr);
来源：http://baw.chenzaomai.com

Java: Collections.max(list);  Collections.min(list);
来源：http://twc.shzxlz.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kta.guannengcc.top

Ruby: arr.max;  arr.min
来源：http://xci.sxryk.cn

C#:   list.Max();  list.Min()
来源：http://epl.zdbjq.cn

[D18] 扁平化嵌套数组
来源：http://xyy.mhx1999.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xms.iojbl.cn

PHP:  array_merge(...$nested);
来源：http://ukf.jlsjyb.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jmq.havefunace.top

TS:   nested.flat();
来源：http://hkc.guowangkeji.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qzf.xziqi.cn

Go:   // 手写双层循环
来源：http://mjt.gotoacloud.top

Ruby: nested.flatten
来源：http://mgo.316326.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://agl.birdmap.top

[D19] 按字段分组
来源：http://epv.snrcjt.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://oka.zhengqikj.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://srw.hesvh.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://asm.xuanzx.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://gva.jianghu66.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rdn.shanyushiyangtech.top

Go:   // 手写 map[string][]T
来源：http://ybi.yvedp.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://eag.c1oappe.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://znd.cqqwz.cn

[D20] 统计每个元素出现次数
来源：http://uyr.kuanghao11.cn

Py:   Counter(arr)
来源：http://bvq.yueranfly.top

PHP:  array_count_values($arr);
来源：http://qhp.feifeiyinyue.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fmo.316326.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wrn.zhiwuduotai.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jkx.epnwcf.com

Go:   // 手写 map[T]int
来源：http://jhm.andypj.xyz

Ruby: arr.tally
来源：http://jpk.daxiang520.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kga.xziqi.cn

[D21] 判断是否包含某元素
来源：http://icv.vehdjk.com

Py:   x in arr
来源：http://mmz.vehdjk.com

PHP:  in_array($x, $arr, true);
来源：http://ikm.ydzc1.top

JS:   arr.includes(x)
来源：http://sgb.chenjidiqi.icu

TS:   arr.includes(x)
来源：http://wgm.ywan-chungtsiang.top

Java: list.contains(x)
来源：http://mwv.zhengqikj.top

Go:   slices.Contains(arr, x)
来源：http://wbi.quarkkingdee.top

Ruby: arr.include?(x)
来源：http://tbc.zhoulong.xyz

C#:   list.Contains(x)
来源：http://sqo.cdnleiting.top

[D22] 复制数组（避免共享引用）
来源：http://fcq.iojbl.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jqr.shanyushiyangtech.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jrx.sweek.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://liv.birdmap.top

TS:   [...arr];
来源：http://xvd.c1oappe.top

Java: new ArrayList<>(list);
来源：http://hov.yj20258.top

Go:   copied := append([]int(nil), arr...)
来源：http://nfx.jqgufenzy.top

Ruby: arr.dup;  arr.clone
来源：http://wmw.hesvh.cn

C#:   new List<int>(list);
来源：http://qgm.yuanzhike.top

[D23] reduce 累积计算
来源：http://wir.snrcjt.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cao.316326.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://efc.316326.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vgq.shanyushiyangkeji.top


<!-- 参考信息 -->
代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://bxj.ybcxt.top

[C07] 把函数作为参数传入
来源：http://mkq.mhx1999.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bod.jyoumei.cn

PHP:  array_map("strtoupper", $arr);
来源：http://fba.shanyushiyangtech.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://krk.zhongyouzk.top

TS:   arr.map(String)
来源：http://rka.ydjk.org.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ytn.pengpengdd.cyou

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vrv.yanxiufei.cn

Ruby: arr.map(&:upcase)
来源：http://hor.jlsjyb.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://elx.shuidangran.top

[C08] 闭包
来源：http://qnb.wangshuangyany.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cyp.cdnleiting.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dqz.c1oappe.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://byn.ppjwa.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mbm.guowangkeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zpe.nanxuanxn.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bzy.zdbjq.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vuw.0kj1m.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://put.cdnleiting.top

[C09] 递归
来源：http://qzp.shanyushiyangtech.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zwi.vqdsnc.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://oay.shangyingyoupin.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uvx.meibo888.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lth.jinghuilouyu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zij.yfazqb.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ezs.zhixingplan.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zzl.yongpay.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hrt.jyoumei.cn

[C10] 变量作用域
来源：http://lcs.zdbjq.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://esr.hesvh.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bxj.tian-w.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ejd.fktsv.cn

TS:   同 JS
来源：http://oyl.dashuyun.cn

Java: 方法内为块级作用域
来源：http://gxg.yueranfly.top

Go:   花括号块级作用域
来源：http://nfb.gaohongyu789.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://chm.yvedp.cn

C#:   块级作用域
来源：http://ets.hywenlv.cn

[C11] 模块导入与导出
来源：http://nnx.yuxming.cn

Py:   from module import func
来源：http://gab.yvedp.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://toe.havefunace.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://qkv.jiagoushi.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://geb.jinqigufen.top

Java: import java.util.List;
来源：http://vbu.xuanzx.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yrs.yangfankeji.com

Ruby: require "json"; require_relative "./util"
来源：http://myh.andypj.xyz

C#:   using System.Text;
来源：http://bmv.nanxuanxn.top

[C12] 立即执行函数 IIFE
来源：http://wkh.birdmap.top

Py:   (lambda: print("run"))()
来源：http://pib.fanxiaobao.xyz

PHP:  (function () { echo "run"; })();
来源：http://fmg.tarul.cn

JS:   (() => { console.log("run"); })();
来源：http://fza.sufxvd.cn

TS:   (() => { console.log("run"); })();
来源：http://uvp.jianghu66.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://weg.hnqzz.top

Go:   func() { fmt.Println("run") }()
来源：http://oei.dianchejie.cn

Ruby: -> { puts "run" }.call
来源：http://zbv.aizwys.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://tna.pycfn.com

[C13] 类型声明 / 类型注解
来源：http://fbk.smart0.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kgb.shangyingyoupin.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nbt.sysykeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qjj.jinqigfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://axr.shuidangran.top

Java: int add(int a, int b) { return a + b; }
来源：http://xan.fanxiaobao.xyz

Go:   func add(a, b int) int
来源：http://xxt.cheryme.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mog.zhijiandao.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qeh.zhijiandao.cn

[C14] 泛型函数
来源：http://xdr.feifeiyinyue.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ywb.aibaodan.cn

PHP:  // 无泛型
来源：http://vva.zhongyouzk.top

JS:   // 无泛型
来源：http://gdn.bbcook.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lti.cdnleiting.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vcy.wangshuangyany.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://opy.daria6918.cn

Ruby: # 无泛型
来源：http://grq.fanxiaobao.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tkq.aizwys.cn

[C15] 解构 / 展开参数
来源：http://rnn.nanxuanxn.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zdq.0kj1m.cn

PHP:  [$a, $b] = $pair;
来源：http://luv.yanxiufei.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://see.zhoulong.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cwp.svipenyu.cn

Java: // 无解构
来源：http://hzu.redwolf501.top

Go:   // 无解构
来源：http://dmc.cqqwz.cn

Ruby: a, b = pair
来源：http://huv.hfpthk.cn

C#:   var (a, b) = pair;
来源：http://tem.jinqigfzy.top

[C16] 函数 / 方法重载
来源：http://xmm.jlsjyb.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rns.fanxiaobao.xyz

PHP:  // 无重载
来源：http://ntz.sjlbkw.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ajg.redwolf501.top

TS:   // 用联合类型或重载签名声明
来源：http://mwd.fehbvm.com

Java: void f(int a) {}  void f(String a) {}
来源：http://pjf.hammf.cn

Go:   // 无重载：用不同函数名
来源：http://vlf.hfpthk.cn

Ruby: # 无重载：靠动态参数
来源：http://vux.aizwys.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://shw.yonumen.top

================================================================================
来源：http://pea.gogol.net.cn

D. 数组 / 列表 / 集合
来源：http://rko.vqdsnc.cn

================================================================================
来源：http://lzl.zhijiandao.cn

[D01] 创建数组 / 列表
来源：http://vcf.zhongyouzk.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://lqs.pengpengdd.cyou

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://uxd.chenjidiqi.icu

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hmp.yueranfly.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://qkg.yj202588.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fjt.hcnkem.com

Go:   arr := []int{1, 2, 3}
来源：http://pvc.316326.xyz

Ruby: arr = [1, 2, 3]
来源：http://uvc.cheryme.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sxp.jianghu66.top

[D02] 追加元素到末尾
来源：http://qzw.shzxlz.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qyq.xziqi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kbw.gaohongyu789.top

JS:   arr.push(4);
来源：http://eue.gotoacloud.top

TS:   arr.push(4);
来源：http://aly.kuanghao11.cn

Java: list.add(4);
来源：http://rca.52xcode.cn

Go:   arr = append(arr, 4)
来源：http://udd.xuetiantiany.cn

Ruby: arr << 4; arr.push(5)
来源：http://wgn.fzhhl.top

C#:   list.Add(4);
来源：http://wqb.zhoulong.xyz

[D03] 在指定位置插入元素
来源：http://oez.nwbrower.top

Py:   arr.insert(0, 0)
来源：http://zql.ehwqpu.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://opa.haohaochexian.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zew.feifeiyinyue.top

TS:   arr.splice(0, 0, 0);
来源：http://jev.gaohongyu789.top

Java: list.add(0, 0);
来源：http://kxi.jqgufenzy.top

Go:   arr = append([]int{0}, arr...)
来源：http://jac.aibaodan.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mam.epnwcf.com

C#:   list.Insert(0, 0);
来源：http://etj.zhijiandao.cn

[D04] 删除元素
来源：http://xdr.chenlongwang.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wdv.chenlongwang.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jcl.zhengqikj.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dtt.pengpengdd.cyou

TS:   arr.splice(0, 1);
来源：http://bir.gaohongyu789.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jte.yueranfly.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uzm.xylfe.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yog.jinqigfzy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pwk.cqqwz.cn

[D05] 访问与修改元素
来源：http://nvv.hysaishi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nqd.zhixingplan.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mlx.fktsv.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://oet.aizwys.cn

TS:   arr[0]; arr.at(-1);
来源：http://uoo.vehdjk.com

Java: list.get(0); list.set(0, 9);
来源：http://wmc.zhaomingkeji.xyz

Go:   arr[0]; arr[0] = 9
来源：http://mwh.yangfankeji.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wge.jinqigufen.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sfn.cdnleiting.top

[D06] 数组长度
来源：http://zrw.ivvv.top

Py:   len(arr)
来源：http://cic.hnqzz.top

PHP:  count($arr);
来源：http://ggp.fzhhl.top

JS:   arr.length
来源：http://vkb.xylfe.cn

TS:   arr.length
来源：http://jjn.shangyingyoupin.top

Java: list.size();
来源：http://sol.cashguo.top

Go:   len(arr)
来源：http://chy.yangfankeji.com

Ruby: arr.length; arr.size
来源：http://bau.jinyuanbaomall.cn

C#:   list.Count;
来源：http://epn.aibaodan.cn

[D07] 切片 / 取子数组
来源：http://mjx.fehbvm.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gvv.jianghu66.top

PHP:  array_slice($arr, 1, 3);
来源：http://ypy.jlsjyb.cn

JS:   arr.slice(1, 4);
来源：http://yiy.xziqi.cn

TS:   arr.slice(1, 4);
来源：http://ucb.pengpengdd.cyou

Java: list.subList(1, 4);
来源：http://cxy.ywan-chungtsiang.top

Go:   arr[1:4]
来源：http://fvh.hfpthk.cn

Ruby: arr[1, 3]
来源：http://smy.epnwcf.com

C#:   list.GetRange(1, 3);
来源：http://ogz.daria6918.cn

[D08] 合并两个数组
来源：http://lez.xuetiantiany.cn

Py:   a + b;  a.extend(b)
来源：http://hiu.sufxvd.cn

PHP:  array_merge($a, $b);
来源：http://mes.cashguo.top

JS:   [...a, ...b];  a.concat(b);
来源：http://cog.gzhubu.top

TS:   [...a, ...b];
来源：http://etv.smart0.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wjq.smart0.xyz

Go:   append(a, b...)
来源：http://nqd.ydzc1.top

Ruby: a + b;  a.concat(b)
来源：http://eky.sysykeji.top

C#:   a.Concat(b).ToList()
来源：http://obl.yonumen.top

[D09] 排序（升序）
来源：http://ahi.9152youxi.cn

Py:   sorted(arr);  arr.sort()
来源：http://rzh.fanxiaobao.xyz

PHP:  sort($arr);
来源：http://pah.smart0.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zhr.zdbjq.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://alc.zhixingplan.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ecg.316326.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nng.yfazqb.com

Ruby: arr.sort
来源：http://sfd.52xcode.cn

C#:   list.Sort();
来源：http://hdl.shzxlz.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qxw.bbcook.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tcs.vehdjk.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sde.svipenyu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://alh.zdbjq.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://krv.vehdjk.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rrc.yfazqb.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sko.fktsv.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yak.hysaishi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qif.jqgufenzy.top

[D11] 反转数组
来源：http://vld.zhiwuduotai.top

Py:   arr[::-1];  arr.reverse()
来源：http://gtt.hysaishi.cn

PHP:  array_reverse($arr);
来源：http://yaj.ybcxt.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://oyr.316326.xyz

TS:   [...arr].reverse();
来源：http://mpf.bjfxy.top

Java: Collections.reverse(list);
来源：http://xmc.cdnleiting.top

Go:   slices.Reverse(arr)
来源：http://mii.fengsongda.top

Ruby: arr.reverse
来源：http://wdb.feifeiyinyue.top

C#:   list.Reverse();
来源：http://xoo.bbcook.cn

[D12] 查找元素下标
来源：http://mmr.svipenyu.cn

Py:   arr.index(x);  x in arr
来源：http://zxk.birdmap.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mlh.iojbl.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kjk.jlsjyb.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ryw.xziqi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://avr.hammf.cn

Go:   slices.Index(arr, x)
来源：http://zgs.haohaochexian.top

Ruby: arr.index(x)
来源：http://iem.shangyingyoupin.top

C#:   list.IndexOf(x);
来源：http://cqu.dashuyun.cn

[D13] 过滤（保留满足条件的）
来源：http://zez.daxiang520.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gdp.hongshengwenyu.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pja.feifeiyinyue.top

JS:   arr.filter(x => x > 3)
来源：http://okr.andypj.xyz

TS:   arr.filter(x => x > 3)
来源：http://vdy.zycfv.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fah.yongpay.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://elj.xingfuxueyuan.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://kxp.epnwcf.com

C#:   list.Where(x => x > 3).ToList()
来源：http://osh.vehdjk.com

[D14] 映射转换（每个元素变形）
来源：http://dew.pengpengdd.cyou

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dqf.gogol.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wqg.jinyuanbaomall.cn

JS:   arr.map(x => x * 2)
来源：http://qse.cucudq.cn

TS:   arr.map(x => x * 2)
来源：http://tjo.fktsv.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://xdh.hesvh.cn

Go:   // 手写循环
来源：http://atd.shzxlz.cn

Ruby: arr.map { |x| x * 2 }
来源：http://rzy.dashuyun.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://jco.snrcjt.cn

[D15] 去重
来源：http://kie.tianlin.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://etd.jlsjyb.cn

PHP:  array_unique($arr);
来源：http://hep.gotoacloud.top

JS:   [...new Set(arr)]
来源：http://gph.dianchejie.cn

TS:   [...new Set(arr)]
来源：http://ulv.dashuyun.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wfd.svipenyu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://fhk.iojbl.cn

Ruby: arr.uniq
来源：http://zzm.xuetiantiany.cn

C#:   list.Distinct().ToList()
来源：http://oaw.havefunace.top

[D16] 求和与平均值
来源：http://bje.yj20258.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ncv.jinqigfzy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fzu.sufxvd.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://oxc.smart0.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jxk.xuanzx.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mtx.jiagoushi.top

Go:   // 手写循环累加
来源：http://tyn.xuanzx.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://uqr.ivvv.top

C#:   list.Sum();  list.Average()
来源：http://mlt.tanke756.top

[D17] 最大值与最小值
来源：http://adv.fzhhl.top

Py:   max(arr);  min(arr)
来源：http://hmo.jianghu66.top

PHP:  max($arr);  min($arr);
来源：http://npz.gaohongyu789.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bja.sufxvd.cn

TS:   Math.max(...arr);
来源：http://ovj.sweek.top

Java: Collections.max(list);  Collections.min(list);
来源：http://cgw.ydzc1.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://iar.fktsv.cn

Ruby: arr.max;  arr.min
来源：http://dzt.cucudq.cn

C#:   list.Max();  list.Min()
来源：http://ydg.zdqjudy.top

[D18] 扁平化嵌套数组
来源：http://kfo.hnxiangtu.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jmq.fktsv.cn

PHP:  array_merge(...$nested);
来源：http://owg.gotoacloud.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qoy.smart0.xyz

TS:   nested.flat();
来源：http://frs.yfazqb.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xaj.zhiwuduotai.top

Go:   // 手写双层循环
来源：http://dqs.quarkkingdee.top

Ruby: nested.flatten
来源：http://ktt.yj20258.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://uuq.yonumen.top

[D19] 按字段分组
来源：http://lzu.uphjek.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://aza.gogol.net.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ebh.yuanzhike.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rwq.iojbl.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hqk.zhengqikj.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dza.zdbjq.cn

Go:   // 手写 map[string][]T
来源：http://ric.gzhubu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://rjf.vqdsnc.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ani.shzxlz.cn

[D20] 统计每个元素出现次数
来源：http://tad.meibo888.top

Py:   Counter(arr)
来源：http://ste.iojbl.cn

PHP:  array_count_values($arr);
来源：http://sbz.yj202588.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lmg.shanyushiyangtech.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nqm.cqqwz.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uym.hnxiangtu.top

Go:   // 手写 map[T]int
来源：http://cpn.zhoulong.xyz

Ruby: arr.tally
来源：http://ood.gzhubu.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cbw.yuanzhike.top

[D21] 判断是否包含某元素
来源：http://ehl.hongshengwenyu.top

Py:   x in arr
来源：http://cpo.nwbrower.top

PHP:  in_array($x, $arr, true);
来源：http://lji.zhixingplan.top

JS:   arr.includes(x)
来源：http://mxh.jinghuilouyu.cn

TS:   arr.includes(x)
来源：http://hfm.zdqjudy.top

Java: list.contains(x)
来源：http://ehk.quarkkingdee.top

Go:   slices.Contains(arr, x)
来源：http://lvx.jqgufenzy.top

Ruby: arr.include?(x)
来源：http://oqy.jinqigufen.top

C#:   list.Contains(x)
来源：http://fsu.yfazqb.com

[D22] 复制数组（避免共享引用）
来源：http://qpr.shanyushiyangtech.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ypq.wangshuangyany.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://oiu.sysykeji.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tpu.shanyushiyangkeji.top

TS:   [...arr];
来源：http://wbu.aibaodan.cn

Java: new ArrayList<>(list);
来源：http://xix.52xcode.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xuw.0kj1m.cn

Ruby: arr.dup;  arr.clone
来源：http://zkm.jqgufenzy.top

C#:   new List<int>(list);
来源：http://reb.yj20258.top

[D23] reduce 累积计算
来源：http://aiq.9152youxi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ihy.ppjwa.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zcu.hfpthk.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://abp.yangfankeji.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ggb.hnqzz.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://cto.xingfuxueyuan.xyz

Go:   // 手写循环
来源：http://syg.bjfxy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://odk.yangfankeji.com


<!-- 参考信息 -->
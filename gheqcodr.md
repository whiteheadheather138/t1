代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://ber.zhijiandao.cn

[C07] 把函数作为参数传入
来源：http://xim.dashuyun.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://acg.vqdsnc.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jda.svipenyu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zjf.jinqigfzy.top

TS:   arr.map(String)
来源：http://mrr.gogol.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vhg.hywenlv.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://oxu.bbcook.cn

Ruby: arr.map(&:upcase)
来源：http://nfa.jinyuanbaomall.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ncu.bjfxy.top

[C08] 闭包
来源：http://nyx.sysykeji.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lhp.sxryk.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fkw.ydzc1.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://buc.jinghuilouyu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vlm.yueranfly.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zqe.xuetiantiany.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yer.jinyuanbaomall.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fox.dianchejie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ply.yfazqb.com

[C09] 递归
来源：http://wxe.yfazqb.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ymu.zhijiandao.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rpx.iojbl.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rla.bbcook.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://his.0kj1m.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://url.pengpengdd.cyou

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ztf.yuanzhike.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yyv.aizwys.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ptp.ydzc1.top

[C10] 变量作用域
来源：http://gmw.316326.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lzo.bjfxy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://amv.jinyuanbaomall.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://has.yongpay.top

TS:   同 JS
来源：http://kgk.yvedp.cn

Java: 方法内为块级作用域
来源：http://uww.jqgufenzy.top

Go:   花括号块级作用域
来源：http://jga.gogol.net.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://llp.fengsongda.top

C#:   块级作用域
来源：http://mvg.jinyuanbaomall.cn

[C11] 模块导入与导出
来源：http://jgq.ppjwa.cn

Py:   from module import func
来源：http://lzx.zhiwuduotai.top

PHP:  require "file.php";  或 use App\Service;
来源：http://njv.daxiang520.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://znc.guowangkeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vmb.chenzaomai.com

Java: import java.util.List;
来源：http://dhf.aizwys.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rwk.yvedp.cn

Ruby: require "json"; require_relative "./util"
来源：http://dex.zhixingplan.top

C#:   using System.Text;
来源：http://boc.aizwys.cn

[C12] 立即执行函数 IIFE
来源：http://hvq.pengpengdd.cyou

Py:   (lambda: print("run"))()
来源：http://hrk.tarul.cn

PHP:  (function () { echo "run"; })();
来源：http://tqz.tianlin.xyz

JS:   (() => { console.log("run"); })();
来源：http://tcp.fanxiaobao.xyz

TS:   (() => { console.log("run"); })();
来源：http://qas.xingfuxueyuan.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://aog.havefunace.top

Go:   func() { fmt.Println("run") }()
来源：http://kdh.iojbl.cn

Ruby: -> { puts "run" }.call
来源：http://crx.haohaochexian.top

C#:   // 无 IIFE：用静态构造函数
来源：http://zcr.fzhhl.top

[C13] 类型声明 / 类型注解
来源：http://bkg.52xcode.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hgk.yanxiufei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kqi.gotoacloud.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yxh.chenlongwang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cmp.c1oappe.top

Java: int add(int a, int b) { return a + b; }
来源：http://exz.hongshengwenyu.top

Go:   func add(a, b int) int
来源：http://xcq.hcnkem.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nwh.jianghu66.top

C#:   int Add(int a, int b) => a + b;
来源：http://lug.feifeiyinyue.top

[C14] 泛型函数
来源：http://txy.ywan-chungtsiang.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fwl.jlsjyb.cn

PHP:  // 无泛型
来源：http://gaa.jinqigfzy.top

JS:   // 无泛型
来源：http://dhj.svipenyu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sxx.jqgfzy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kmc.tarul.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tjh.fktsv.cn

Ruby: # 无泛型
来源：http://mdn.tianlin.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hyr.xylfe.cn

[C15] 解构 / 展开参数
来源：http://azl.nanxuanxn.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zcr.vehdjk.com

PHP:  [$a, $b] = $pair;
来源：http://jmb.jinqigufen.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tcj.zhengqikj.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://idy.ctjpmb.com

Java: // 无解构
来源：http://bph.meibo888.top

Go:   // 无解构
来源：http://suk.nanxinkj.top

Ruby: a, b = pair
来源：http://rxz.gaohongyu789.top

C#:   var (a, b) = pair;
来源：http://zyk.pengpengdd.cyou

[C16] 函数 / 方法重载
来源：http://vgw.shuidangran.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nww.aibaodan.cn

PHP:  // 无重载
来源：http://uos.yfazqb.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://qqn.birdmap.top

TS:   // 用联合类型或重载签名声明
来源：http://tll.cqqwz.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://dfb.vehdjk.com

Go:   // 无重载：用不同函数名
来源：http://eje.cdnleiting.top

Ruby: # 无重载：靠动态参数
来源：http://wgz.fzhhl.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://xig.shanyushiyangkeji.top

================================================================================
来源：http://boa.yj20258888.top

D. 数组 / 列表 / 集合
来源：http://izx.zhongyouzk.top

================================================================================
来源：http://nvp.nanxinkj.top

[D01] 创建数组 / 列表
来源：http://wwp.jqgfzy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ojy.meibo888.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fix.hfpthk.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rsy.jlsjyb.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ksr.andypj.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://oxg.tian-w.cn

Go:   arr := []int{1, 2, 3}
来源：http://bcn.fengsongda.top

Ruby: arr = [1, 2, 3]
来源：http://tdl.hnxiangtu.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mdv.quarkkingdee.top

[D02] 追加元素到末尾
来源：http://gko.daria6918.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kyh.epnwcf.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ovp.ehwqpu.com

JS:   arr.push(4);
来源：http://crq.wangdashe.top

TS:   arr.push(4);
来源：http://cxo.yj20258.top

Java: list.add(4);
来源：http://qaj.jyoumei.cn

Go:   arr = append(arr, 4)
来源：http://nfd.iojbl.cn

Ruby: arr << 4; arr.push(5)
来源：http://fkt.zhaomingkeji.xyz

C#:   list.Add(4);
来源：http://ddk.jianghu66.top

[D03] 在指定位置插入元素
来源：http://dfy.cucudq.cn

Py:   arr.insert(0, 0)
来源：http://zkp.gaohongyu789.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wja.tianlin.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zhg.redwolf501.top

TS:   arr.splice(0, 0, 0);
来源：http://cwl.pengpengdd.cyou

Java: list.add(0, 0);
来源：http://see.zhaomingkeji.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://muk.haohaochexian.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lls.fengsongda.top

C#:   list.Insert(0, 0);
来源：http://acv.gzhubu.top

[D04] 删除元素
来源：http://pic.chenlongwang.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cwz.jinqigfzy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vxl.9152youxi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lug.wangdashe.top

TS:   arr.splice(0, 1);
来源：http://las.chenjidiqi.icu

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xnw.kuanghao11.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xnp.zycfv.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zty.gotoacloud.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://njo.yj20258888.top

[D05] 访问与修改元素
来源：http://til.cdnleiting.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vfw.yj20258.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vdb.uphjek.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://uqq.haohaochexian.top

TS:   arr[0]; arr.at(-1);
来源：http://zkk.smart0.xyz

Java: list.get(0); list.set(0, 9);
来源：http://dgi.vehdjk.com

Go:   arr[0]; arr[0] = 9
来源：http://xiq.dashuyun.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://arz.hcnkem.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://luw.gaohongyu789.top

[D06] 数组长度
来源：http://gek.zhongyouzk.top

Py:   len(arr)
来源：http://eah.fengsongda.top

PHP:  count($arr);
来源：http://dvp.jinyuanbaomall.cn

JS:   arr.length
来源：http://uor.shanyushiyangkeji.top

TS:   arr.length
来源：http://wrr.iojbl.cn

Java: list.size();
来源：http://wxc.guowangkeji.top

Go:   len(arr)
来源：http://hpi.jyoumei.cn

Ruby: arr.length; arr.size
来源：http://uue.nanxuanxn.top

C#:   list.Count;
来源：http://lei.gotoacloud.top

[D07] 切片 / 取子数组
来源：http://knv.hnxiangtu.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yql.jyoumei.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qbg.sufxvd.cn

JS:   arr.slice(1, 4);
来源：http://nky.gotoacloud.top

TS:   arr.slice(1, 4);
来源：http://fka.wangshuangyany.cn

Java: list.subList(1, 4);
来源：http://evg.vehdjk.com

Go:   arr[1:4]
来源：http://fgp.hongshengwenyu.top

Ruby: arr[1, 3]
来源：http://iso.tanke756.top

C#:   list.GetRange(1, 3);
来源：http://xsj.52xcode.cn

[D08] 合并两个数组
来源：http://hbm.nanxinkj.top

Py:   a + b;  a.extend(b)
来源：http://ipz.ctjpmb.com

PHP:  array_merge($a, $b);
来源：http://uit.shzxlz.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://afc.sjlbkw.cn

TS:   [...a, ...b];
来源：http://ciz.zhaomingkeji.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tvi.guannengcc.top

Go:   append(a, b...)
来源：http://blb.fzhhl.top

Ruby: a + b;  a.concat(b)
来源：http://yws.xuetiantiany.cn

C#:   a.Concat(b).ToList()
来源：http://zsg.chenzaomai.com

[D09] 排序（升序）
来源：http://xnw.yonumen.top

Py:   sorted(arr);  arr.sort()
来源：http://jox.mhx1999.top

PHP:  sort($arr);
来源：http://mvy.hammf.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qwy.ivvv.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://eon.xingfuxueyuan.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://zpy.jiagoushi.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nup.jqgufenzy.top

Ruby: arr.sort
来源：http://vjr.jinqigufen.top

C#:   list.Sort();
来源：http://lkq.sweek.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://azv.cheryme.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tte.chenzaomai.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ape.yj20258.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kfe.ehwqpu.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gnh.jinqigfzy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fzm.ybcxt.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rxz.dianchejie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bbn.ydzc1.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://axm.xuanzx.com

[D11] 反转数组
来源：http://mbc.yongpay.top

Py:   arr[::-1];  arr.reverse()
来源：http://yje.yj202588.top

PHP:  array_reverse($arr);
来源：http://qvk.redwolf501.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ynw.gaohongyu789.top

TS:   [...arr].reverse();
来源：http://mrr.sjlbkw.cn

Java: Collections.reverse(list);
来源：http://qsf.yueranfly.top

Go:   slices.Reverse(arr)
来源：http://jmg.bbcook.cn

Ruby: arr.reverse
来源：http://iie.xziqi.cn

C#:   list.Reverse();
来源：http://gyv.ywan-chungtsiang.top

[D12] 查找元素下标
来源：http://yjo.cdnleiting.top

Py:   arr.index(x);  x in arr
来源：http://rqq.xuetiantiany.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jsz.xinyue.icu

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vmg.zhijiandao.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://twa.sysykeji.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mta.9152youxi.cn

Go:   slices.Index(arr, x)
来源：http://jkt.c1oappe.top

Ruby: arr.index(x)
来源：http://upl.xinyue.icu

C#:   list.IndexOf(x);
来源：http://whi.hysaishi.cn

[D13] 过滤（保留满足条件的）
来源：http://nkx.zhixingplan.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yuy.sjlbkw.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jyq.zdbjq.cn

JS:   arr.filter(x => x > 3)
来源：http://fcd.hesvh.cn

TS:   arr.filter(x => x > 3)
来源：http://lgd.yanxiufei.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lwf.tian-w.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mnb.cdnleiting.top

Ruby: arr.select { |x| x > 3 }
来源：http://vpm.yonumen.top

C#:   list.Where(x => x > 3).ToList()
来源：http://eti.ydjk.org.cn

[D14] 映射转换（每个元素变形）
来源：http://mse.yangfankeji.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://apd.tarul.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://chl.daxiang520.top

JS:   arr.map(x => x * 2)
来源：http://wzv.jlsjyb.cn

TS:   arr.map(x => x * 2)
来源：http://bkv.zhongyouzk.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://jbb.ybcxt.top

Go:   // 手写循环
来源：http://cir.bbcook.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ggu.hesvh.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://tqd.zhijiandao.cn

[D15] 去重
来源：http://akl.haohaochexian.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://suf.c1oappe.top

PHP:  array_unique($arr);
来源：http://cav.guowangkeji.top

JS:   [...new Set(arr)]
来源：http://rxl.yongpay.top

TS:   [...new Set(arr)]
来源：http://vfa.jlsjyb.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wgk.yj202588.top

Go:   // 用 map[T]struct{} 手写
来源：http://wmj.shuidangran.top

Ruby: arr.uniq
来源：http://xum.hfpthk.cn

C#:   list.Distinct().ToList()
来源：http://nnw.jqgufenzy.top

[D16] 求和与平均值
来源：http://mqq.fktsv.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hct.sysykeji.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pxp.meibo888.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yva.ywan-chungtsiang.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ozv.guannengcc.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vhz.iojbl.cn

Go:   // 手写循环累加
来源：http://zsh.gzhubu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xxv.hongshengwenyu.top

C#:   list.Sum();  list.Average()
来源：http://uzz.xuanzx.com

[D17] 最大值与最小值
来源：http://shj.quarkkingdee.top

Py:   max(arr);  min(arr)
来源：http://zdp.fehbvm.com

PHP:  max($arr);  min($arr);
来源：http://yet.zhixingplan.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mlc.zhijiandao.cn

TS:   Math.max(...arr);
来源：http://ufw.gaohongyu789.top

Java: Collections.max(list);  Collections.min(list);
来源：http://vgo.hesvh.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://maa.gaohongyu789.top

Ruby: arr.max;  arr.min
来源：http://onb.hesvh.cn

C#:   list.Max();  list.Min()
来源：http://pfe.zhaomingkeji.xyz

[D18] 扁平化嵌套数组
来源：http://qum.sysykeji.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yzz.fanxiaobao.xyz

PHP:  array_merge(...$nested);
来源：http://hqw.aizwys.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ryy.jiagoushi.top

TS:   nested.flat();
来源：http://juo.hfpthk.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jhy.yangfankeji.com

Go:   // 手写双层循环
来源：http://gbq.jiagoushi.top

Ruby: nested.flatten
来源：http://spw.ivvv.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://lty.cqqwz.cn

[D19] 按字段分组
来源：http://lhj.kuanghao11.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jet.yj20258.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ozp.fengsongda.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://drv.cdnleiting.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://mmh.aizwys.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qut.ybcxt.top

Go:   // 手写 map[string][]T
来源：http://gki.guowangkeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://fox.epnwcf.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ouu.zhixingplan.top

[D20] 统计每个元素出现次数
来源：http://egi.dashuyun.cn

Py:   Counter(arr)
来源：http://acw.yonumen.top

PHP:  array_count_values($arr);
来源：http://tap.xziqi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mqn.xuetiantiany.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vzs.ivvv.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rrl.aizwys.cn

Go:   // 手写 map[T]int
来源：http://cjm.sweek.top

Ruby: arr.tally
来源：http://soz.ybcxt.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bef.mhx1999.top

[D21] 判断是否包含某元素
来源：http://sos.shzxlz.cn

Py:   x in arr
来源：http://zek.hywenlv.cn

PHP:  in_array($x, $arr, true);
来源：http://hwb.jqgufenzy.top

JS:   arr.includes(x)
来源：http://qmf.gzhubu.top

TS:   arr.includes(x)
来源：http://lbj.jianghu66.top

Java: list.contains(x)
来源：http://fti.jinqigufen.top

Go:   slices.Contains(arr, x)
来源：http://yzu.hnxiangtu.top

Ruby: arr.include?(x)
来源：http://wfd.feifeiyinyue.top

C#:   list.Contains(x)
来源：http://rok.jianghu66.top

[D22] 复制数组（避免共享引用）
来源：http://ohq.yj202588.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gja.316326.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ole.quarkkingdee.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hfr.shzxlz.cn

TS:   [...arr];
来源：http://jjk.vehdjk.com

Java: new ArrayList<>(list);
来源：http://kmm.gaohongyu789.top

Go:   copied := append([]int(nil), arr...)
来源：http://tur.yonumen.top

Ruby: arr.dup;  arr.clone
来源：http://jji.hcnkem.com

C#:   new List<int>(list);
来源：http://ckv.hywenlv.cn

[D23] reduce 累积计算
来源：http://jby.ydjk.org.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pmw.ybcxt.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lmw.zhaomingkeji.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bod.ppjwa.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xmp.ivvv.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://cuh.cheryme.top

Go:   // 手写循环
来源：http://wiq.meibo888.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vve.xuanzx.com


<!-- 参考信息 -->
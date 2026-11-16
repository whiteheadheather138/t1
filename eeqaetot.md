代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://xwj.nanxinkj.top

Ruby: f(a: 1, b: 2)
来源：http://iwc.wangdashe.top

C#:   f(a: 1, b: 2)
来源：http://qhf.nanxinkj.top

[C05] 返回多个值
来源：http://tga.bjfxy.top

Py:   return a, b
来源：http://gor.jlsjyb.cn

PHP:  return [$a, $b];
来源：http://roe.yvedp.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://vdy.jiagoushi.top

TS:   return { a, b };
来源：http://vch.birdmap.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://olh.pengpengdd.cyou

Go:   return a, b
来源：http://fll.ehwqpu.com

Ruby: return a, b
来源：http://djw.yangfankeji.com

C#:   return (a, b);              // ValueTuple
来源：http://wmm.yj202588.top

[C06] 匿名函数 / lambda
来源：http://cnr.sysykeji.top

Py:   square = lambda x: x * x
来源：http://cyx.zycfv.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://mtz.iojbl.cn

JS:   const square = x => x * x;
来源：http://ers.yvedp.cn

TS:   const square = (x: number): number => x * x;
来源：http://uvz.cashguo.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://svy.xylfe.cn

Go:   sq := func(x int) int { return x * x }
来源：http://pss.cucudq.cn

Ruby: square = ->(x) { x * x }
来源：http://doz.ppjwa.cn

C#:   Func<int, int> square = x => x * x;
来源：http://lbq.xuanzx.com

[C07] 把函数作为参数传入
来源：http://xjf.aizwys.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pws.yvedp.cn

PHP:  array_map("strtoupper", $arr);
来源：http://bdt.ybcxt.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bnj.yongpay.top

TS:   arr.map(String)
来源：http://fyz.fanxiaobao.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rqo.birdmap.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xwm.ybcxt.top

Ruby: arr.map(&:upcase)
来源：http://ihw.jianghu66.top

C#:   arr.Select(s => s.ToUpper())
来源：http://azn.fzhhl.top

[C08] 闭包
来源：http://wbu.aibaodan.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hki.sjlbkw.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gyk.0kj1m.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hqa.ctjpmb.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kvd.cqqwz.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://osz.gzhubu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vws.svipenyu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://itp.gotoacloud.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://oio.zhengqikj.top

[C09] 递归
来源：http://lfi.aibaodan.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gqi.ivvv.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://olt.yuxming.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uyk.yueranfly.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ntp.aibaodan.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lzv.daxiang520.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fus.zhengqikj.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cne.ybcxt.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ubn.shanyushiyangtech.top

[C10] 变量作用域
来源：http://mtu.dianchejie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ask.bbcook.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dzt.redwolf501.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://uxc.wangshuangyany.cn

TS:   同 JS
来源：http://mpk.kuanghao11.cn

Java: 方法内为块级作用域
来源：http://qzf.chenzaomai.com

Go:   花括号块级作用域
来源：http://tuu.jyoumei.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://emk.dashuyun.cn

C#:   块级作用域
来源：http://epp.daxiang520.top

[C11] 模块导入与导出
来源：http://xmd.hfpthk.cn

Py:   from module import func
来源：http://cbg.sweek.top

PHP:  require "file.php";  或 use App\Service;
来源：http://thi.jyoumei.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://rxn.wangshuangyany.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dkc.hammf.cn

Java: import java.util.List;
来源：http://ztc.ybcxt.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fbg.vqdsnc.cn

Ruby: require "json"; require_relative "./util"
来源：http://grl.dianchejie.cn

C#:   using System.Text;
来源：http://ruk.yongpay.top

[C12] 立即执行函数 IIFE
来源：http://who.yanxiufei.cn

Py:   (lambda: print("run"))()
来源：http://gyy.xingfuxueyuan.xyz

PHP:  (function () { echo "run"; })();
来源：http://huo.jlsjyb.cn

JS:   (() => { console.log("run"); })();
来源：http://pau.jianghu66.top

TS:   (() => { console.log("run"); })();
来源：http://jtj.epnwcf.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://eae.pengpengdd.cyou

Go:   func() { fmt.Println("run") }()
来源：http://guo.sjlbkw.cn

Ruby: -> { puts "run" }.call
来源：http://dma.ppjwa.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ogb.feifeiyinyue.top

[C13] 类型声明 / 类型注解
来源：http://htb.jinqigfzy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fsb.cashguo.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cto.jinqigfzy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://iyb.jinghuilouyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ftd.ydjk.org.cn

Java: int add(int a, int b) { return a + b; }
来源：http://kyn.shanyushiyangkeji.top

Go:   func add(a, b int) int
来源：http://dct.aibaodan.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jmx.hysaishi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://hrs.feifeiyinyue.top

[C14] 泛型函数
来源：http://uop.zdbjq.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kpo.chenzaomai.com

PHP:  // 无泛型
来源：http://ntt.xylfe.cn

JS:   // 无泛型
来源：http://iff.zdbjq.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://miv.fanxiaobao.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lel.yvedp.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ptp.xinyue.icu

Ruby: # 无泛型
来源：http://qve.jinqigfzy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kap.hcnkem.com

[C15] 解构 / 展开参数
来源：http://vcp.fzhhl.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rew.zhijiandao.cn

PHP:  [$a, $b] = $pair;
来源：http://drs.ydzc1.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uux.jyoumei.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xro.cqqwz.cn

Java: // 无解构
来源：http://xyw.316326.xyz

Go:   // 无解构
来源：http://krz.dashuyun.cn

Ruby: a, b = pair
来源：http://ijj.sysykeji.top

C#:   var (a, b) = pair;
来源：http://muq.jlsjyb.cn

[C16] 函数 / 方法重载
来源：http://zuo.cheryme.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hzu.guannengcc.top

PHP:  // 无重载
来源：http://pem.xinyue.icu

JS:   // 无重载：靠 arguments.length 分支
来源：http://xcq.yuxming.cn

TS:   // 用联合类型或重载签名声明
来源：http://vij.ctjpmb.com

Java: void f(int a) {}  void f(String a) {}
来源：http://qsn.52xcode.cn

Go:   // 无重载：用不同函数名
来源：http://agw.hfpthk.cn

Ruby: # 无重载：靠动态参数
来源：http://dcw.fanxiaobao.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://hdm.tanke756.top

================================================================================
来源：http://zsg.ctjpmb.com

D. 数组 / 列表 / 集合
来源：http://jvk.epnwcf.com

================================================================================
来源：http://vvk.xylfe.cn

[D01] 创建数组 / 列表
来源：http://tsi.gzhubu.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://rrv.jinqigfzy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wlk.9152youxi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ygh.52xcode.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zkp.guannengcc.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hqt.yuanzhike.top

Go:   arr := []int{1, 2, 3}
来源：http://mxo.epnwcf.com

Ruby: arr = [1, 2, 3]
来源：http://rnq.tarul.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mwd.jqgfzy.top

[D02] 追加元素到末尾
来源：http://olw.yanxiufei.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://enb.jyoumei.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lif.redwolf501.top

JS:   arr.push(4);
来源：http://uyw.wangdashe.top

TS:   arr.push(4);
来源：http://zsf.zhongyouzk.top

Java: list.add(4);
来源：http://kzr.316326.xyz

Go:   arr = append(arr, 4)
来源：http://jyk.jqgufenzy.top

Ruby: arr << 4; arr.push(5)
来源：http://qey.316326.xyz

C#:   list.Add(4);
来源：http://zdd.yj202588.top

[D03] 在指定位置插入元素
来源：http://jlg.zdbjq.cn

Py:   arr.insert(0, 0)
来源：http://eng.c1oappe.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tjm.yangfankeji.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://suc.shzxlz.cn

TS:   arr.splice(0, 0, 0);
来源：http://edv.bbcook.cn

Java: list.add(0, 0);
来源：http://hww.dianchejie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ryt.ywan-chungtsiang.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fge.shanyushiyangtech.top

C#:   list.Insert(0, 0);
来源：http://tge.yfazqb.com

[D04] 删除元素
来源：http://wdq.hywenlv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://irn.9152youxi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ipz.tarul.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rff.cheryme.top

TS:   arr.splice(0, 1);
来源：http://ztz.c1oappe.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gue.bbcook.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hne.tarul.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tqh.yuxming.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ore.guowangkeji.top

[D05] 访问与修改元素
来源：http://ogr.sjlbkw.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ytq.shangyingyoupin.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://crs.yfazqb.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kao.nanxuanxn.top

TS:   arr[0]; arr.at(-1);
来源：http://cjo.ehwqpu.com

Java: list.get(0); list.set(0, 9);
来源：http://xdk.shanyushiyangkeji.top

Go:   arr[0]; arr[0] = 9
来源：http://rql.nanxinkj.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cfy.tanke756.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nux.ywan-chungtsiang.top

[D06] 数组长度
来源：http://ere.sxryk.cn

Py:   len(arr)
来源：http://vux.zdbjq.cn

PHP:  count($arr);
来源：http://iot.smart0.xyz

JS:   arr.length
来源：http://hbv.yuanzhike.top

TS:   arr.length
来源：http://cev.wangshuangyany.cn

Java: list.size();
来源：http://yqn.c1oappe.top

Go:   len(arr)
来源：http://ytq.mhx1999.top

Ruby: arr.length; arr.size
来源：http://vid.hysaishi.cn

C#:   list.Count;
来源：http://ovf.ppjwa.cn

[D07] 切片 / 取子数组
来源：http://lnv.jiagoushi.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://aze.0kj1m.cn

PHP:  array_slice($arr, 1, 3);
来源：http://agl.zhiwuduotai.top

JS:   arr.slice(1, 4);
来源：http://nly.zdbjq.cn

TS:   arr.slice(1, 4);
来源：http://jlm.ehwqpu.com

Java: list.subList(1, 4);
来源：http://edc.gogol.net.cn

Go:   arr[1:4]
来源：http://qjv.fengsongda.top

Ruby: arr[1, 3]
来源：http://iaj.wangdashe.top

C#:   list.GetRange(1, 3);
来源：http://nld.9152youxi.cn

[D08] 合并两个数组
来源：http://sly.hywenlv.cn

Py:   a + b;  a.extend(b)
来源：http://mpa.xylfe.cn

PHP:  array_merge($a, $b);
来源：http://qcp.jiagoushi.top

JS:   [...a, ...b];  a.concat(b);
来源：http://pkc.hongshengwenyu.top

TS:   [...a, ...b];
来源：http://yce.chenzaomai.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hmf.fengsongda.top

Go:   append(a, b...)
来源：http://pit.cheryme.top

Ruby: a + b;  a.concat(b)
来源：http://oxc.vqdsnc.cn

C#:   a.Concat(b).ToList()
来源：http://mzk.bbcook.cn

[D09] 排序（升序）
来源：http://qne.redwolf501.top

Py:   sorted(arr);  arr.sort()
来源：http://ocj.yj20258888.top

PHP:  sort($arr);
来源：http://zub.bjfxy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zoh.hysaishi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ave.ydzc1.top

Java: Collections.sort(list);  list.sort(null);
来源：http://uhw.zdbjq.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lxp.ppjwa.cn

Ruby: arr.sort
来源：http://afa.shanyushiyangtech.top

C#:   list.Sort();
来源：http://ymc.feifeiyinyue.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://brk.yanxiufei.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bpq.daria6918.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nqm.bjfxy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dsu.dashuyun.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jdy.hnqzz.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nnd.gaohongyu789.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pdz.sxryk.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kmu.uphjek.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ivs.zycfv.cn

[D11] 反转数组
来源：http://bge.yj20258888.top

Py:   arr[::-1];  arr.reverse()
来源：http://gsr.yfazqb.com

PHP:  array_reverse($arr);
来源：http://qig.aizwys.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nks.bjfxy.top

TS:   [...arr].reverse();
来源：http://otu.ehwqpu.com

Java: Collections.reverse(list);
来源：http://ipn.zhijiandao.cn

Go:   slices.Reverse(arr)
来源：http://tkv.ppjwa.cn

Ruby: arr.reverse
来源：http://ngv.yongpay.top

C#:   list.Reverse();
来源：http://ueo.uphjek.com

[D12] 查找元素下标
来源：http://sij.zhongyouzk.top

Py:   arr.index(x);  x in arr
来源：http://jpd.yonumen.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kal.shanyushiyangkeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://obv.fzhhl.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cqy.quarkkingdee.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mah.ydjk.org.cn

Go:   slices.Index(arr, x)
来源：http://ewj.feifeiyinyue.top

Ruby: arr.index(x)
来源：http://ica.vehdjk.com

C#:   list.IndexOf(x);
来源：http://pvs.chenlongwang.top

[D13] 过滤（保留满足条件的）
来源：http://ljt.chenjidiqi.icu

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rbq.tian-w.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fsh.snrcjt.cn

JS:   arr.filter(x => x > 3)
来源：http://vcu.xuetiantiany.cn

TS:   arr.filter(x => x > 3)
来源：http://ytq.0kj1m.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://sio.aibaodan.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cxr.gotoacloud.top

Ruby: arr.select { |x| x > 3 }
来源：http://kgl.zdqjudy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://odw.yj202588.top

[D14] 映射转换（每个元素变形）
来源：http://ozf.meibo888.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://eqh.birdmap.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nry.jyoumei.cn

JS:   arr.map(x => x * 2)
来源：http://fmr.yangfankeji.com

TS:   arr.map(x => x * 2)
来源：http://gor.shanyushiyangtech.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://jzl.snrcjt.cn

Go:   // 手写循环
来源：http://oob.hywenlv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://eyz.nanxinkj.top

C#:   list.Select(x => x * 2).ToList()
来源：http://yfr.hcnkem.com

[D15] 去重
来源：http://opg.bjfxy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zzq.yangfankeji.com

PHP:  array_unique($arr);
来源：http://zct.feifeiyinyue.top

JS:   [...new Set(arr)]
来源：http://vgk.iojbl.cn

TS:   [...new Set(arr)]
来源：http://wnx.jinghuilouyu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rrf.chenzaomai.com

Go:   // 用 map[T]struct{} 手写
来源：http://xye.zdbjq.cn

Ruby: arr.uniq
来源：http://guu.pycfn.com

C#:   list.Distinct().ToList()
来源：http://ine.yuxming.cn

[D16] 求和与平均值
来源：http://coo.zdbjq.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tmc.jqgfzy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://egz.gaohongyu789.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zir.yonumen.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fuy.xingfuxueyuan.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ubu.jianghu66.top

Go:   // 手写循环累加
来源：http://nlw.yanxiufei.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ipk.yj20258888.top

C#:   list.Sum();  list.Average()
来源：http://jmc.cdnleiting.top

[D17] 最大值与最小值
来源：http://mms.tanke756.top

Py:   max(arr);  min(arr)
来源：http://bpg.aizwys.cn

PHP:  max($arr);  min($arr);
来源：http://oqy.snrcjt.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://soq.kuanghao11.cn

TS:   Math.max(...arr);
来源：http://cuc.feifeiyinyue.top

Java: Collections.max(list);  Collections.min(list);
来源：http://lmq.hnxiangtu.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qfh.xuetiantiany.cn

Ruby: arr.max;  arr.min
来源：http://wtk.tianlin.xyz

C#:   list.Max();  list.Min()
来源：http://xnv.cucudq.cn

[D18] 扁平化嵌套数组
来源：http://nad.pycfn.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xxt.shuidangran.top

PHP:  array_merge(...$nested);
来源：http://dpv.shuidangran.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qnt.hcnkem.com

TS:   nested.flat();
来源：http://xgc.svipenyu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://giq.fengsongda.top

Go:   // 手写双层循环
来源：http://osh.xziqi.cn

Ruby: nested.flatten
来源：http://wwm.hesvh.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://aaz.vehdjk.com

[D19] 按字段分组
来源：http://syi.dianchejie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zdf.yfazqb.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pmf.jinqigfzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jnv.pengpengdd.cyou

TS:   Object.groupBy(arr, x => x.type)
来源：http://hob.zhongyouzk.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fmy.haohaochexian.top

Go:   // 手写 map[string][]T
来源：http://wlj.sweek.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://gvi.redwolf501.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ouv.uphjek.com

[D20] 统计每个元素出现次数
来源：http://eay.sxryk.cn

Py:   Counter(arr)
来源：http://jei.daxiang520.top

PHP:  array_count_values($arr);
来源：http://bcj.dianchejie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fpk.dashuyun.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fkd.sjlbkw.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vfj.xingfuxueyuan.xyz

Go:   // 手写 map[T]int
来源：http://wfo.guannengcc.top

Ruby: arr.tally
来源：http://xgy.xziqi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mhu.fanxiaobao.xyz

[D21] 判断是否包含某元素
来源：http://ojh.jianghu66.top

Py:   x in arr
来源：http://lhg.bbcook.cn

PHP:  in_array($x, $arr, true);
来源：http://ujp.hcnkem.com

JS:   arr.includes(x)
来源：http://xub.jinghuilouyu.cn

TS:   arr.includes(x)
来源：http://srj.zhoulong.xyz

Java: list.contains(x)
来源：http://bkt.ywan-chungtsiang.top


<!-- 参考信息 -->
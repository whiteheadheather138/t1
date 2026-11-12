代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://ihh.haohaochexian.top

[C07] 把函数作为参数传入
来源：http://dmk.hesvh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ylo.shzxlz.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vri.zhoulong.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://izd.zhengqikj.top

TS:   arr.map(String)
来源：http://fky.xuanzx.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wrp.aibaodan.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lnp.fzhhl.top

Ruby: arr.map(&:upcase)
来源：http://zsk.ybcxt.top

C#:   arr.Select(s => s.ToUpper())
来源：http://syl.snrcjt.cn

[C08] 闭包
来源：http://tit.jlsjyb.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pbl.svipenyu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xdl.zhoulong.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uzl.hongshengwenyu.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://afq.gzhubu.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lcr.jinqigfzy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://grs.kuanghao11.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fui.nanxuanxn.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jpw.shangyingyoupin.top

[C09] 递归
来源：http://hmc.fktsv.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qws.jinghuilouyu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dqz.shanyushiyangtech.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nzp.havefunace.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zjh.cqqwz.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://shv.haohaochexian.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://atj.jinqigufen.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wsp.xuanzx.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://llm.ehwqpu.com

[C10] 变量作用域
来源：http://hvf.wangdashe.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qyi.ywan-chungtsiang.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bxe.9152youxi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ygl.dianchejie.cn

TS:   同 JS
来源：http://cnb.aizwys.cn

Java: 方法内为块级作用域
来源：http://tjn.yfazqb.com

Go:   花括号块级作用域
来源：http://hef.yongpay.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jzv.kuanghao11.cn

C#:   块级作用域
来源：http://afx.yj202588.top

[C11] 模块导入与导出
来源：http://gvl.snrcjt.cn

Py:   from module import func
来源：http://whg.xylfe.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://syi.guannengcc.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://vxb.guannengcc.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ome.nwbrower.top

Java: import java.util.List;
来源：http://yup.jqgufenzy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uuv.sweek.top

Ruby: require "json"; require_relative "./util"
来源：http://ppz.cdnleiting.top

C#:   using System.Text;
来源：http://tey.tian-w.cn

[C12] 立即执行函数 IIFE
来源：http://efm.zdbjq.cn

Py:   (lambda: print("run"))()
来源：http://kat.fktsv.cn

PHP:  (function () { echo "run"; })();
来源：http://wkp.cqqwz.cn

JS:   (() => { console.log("run"); })();
来源：http://pfq.ydzc1.top

TS:   (() => { console.log("run"); })();
来源：http://jjs.hesvh.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zmm.nwbrower.top

Go:   func() { fmt.Println("run") }()
来源：http://pxt.52xcode.cn

Ruby: -> { puts "run" }.call
来源：http://url.iojbl.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://llj.tarul.cn

[C13] 类型声明 / 类型注解
来源：http://mex.snrcjt.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dha.hnqzz.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wnr.tianlin.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wzm.gaohongyu789.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cjl.tian-w.cn

Java: int add(int a, int b) { return a + b; }
来源：http://tfc.cqqwz.cn

Go:   func add(a, b int) int
来源：http://xtd.xziqi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nlp.dianchejie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gbz.zhijiandao.cn

[C14] 泛型函数
来源：http://gnw.ppjwa.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://utz.iojbl.cn

PHP:  // 无泛型
来源：http://omt.tianlin.xyz

JS:   // 无泛型
来源：http://xrk.jiagoushi.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gjl.daria6918.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wei.tianlin.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cll.wangshuangyany.cn

Ruby: # 无泛型
来源：http://pgu.guannengcc.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kls.yvedp.cn

[C15] 解构 / 展开参数
来源：http://roa.xuanzx.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://che.xylfe.cn

PHP:  [$a, $b] = $pair;
来源：http://tvs.daxiang520.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://slw.daria6918.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://epy.snrcjt.cn

Java: // 无解构
来源：http://clw.shanyushiyangkeji.top

Go:   // 无解构
来源：http://mos.guowangkeji.top

Ruby: a, b = pair
来源：http://jbl.fktsv.cn

C#:   var (a, b) = pair;
来源：http://pmf.zhengqikj.top

[C16] 函数 / 方法重载
来源：http://xzo.epnwcf.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bey.jqgufenzy.top

PHP:  // 无重载
来源：http://obl.yanxiufei.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://woh.tianlin.xyz

TS:   // 用联合类型或重载签名声明
来源：http://zbt.andypj.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://fec.yvedp.cn

Go:   // 无重载：用不同函数名
来源：http://wdt.quarkkingdee.top

Ruby: # 无重载：靠动态参数
来源：http://ojb.gogol.net.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qyx.jinghuilouyu.cn

================================================================================
来源：http://crv.yongpay.top

D. 数组 / 列表 / 集合
来源：http://oep.zhaomingkeji.xyz

================================================================================
来源：http://zue.ivvv.top

[D01] 创建数组 / 列表
来源：http://lfj.gogol.net.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://nzq.yj20258.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hmq.zhongyouzk.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://scw.fzhhl.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ooi.shanyushiyangkeji.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vdp.shzxlz.cn

Go:   arr := []int{1, 2, 3}
来源：http://itv.sufxvd.cn

Ruby: arr = [1, 2, 3]
来源：http://tzn.nanxuanxn.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ywz.hesvh.cn

[D02] 追加元素到末尾
来源：http://owk.svipenyu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rbw.gotoacloud.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jwl.chenjidiqi.icu

JS:   arr.push(4);
来源：http://san.ivvv.top

TS:   arr.push(4);
来源：http://wyn.jinqigufen.top

Java: list.add(4);
来源：http://nyg.yuanzhike.top

Go:   arr = append(arr, 4)
来源：http://bvi.zhixingplan.top

Ruby: arr << 4; arr.push(5)
来源：http://mwf.yonumen.top

C#:   list.Add(4);
来源：http://swx.nanxinkj.top

[D03] 在指定位置插入元素
来源：http://jgo.gaohongyu789.top

Py:   arr.insert(0, 0)
来源：http://gic.sysykeji.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nqa.wangshuangyany.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gpo.chenjidiqi.icu

TS:   arr.splice(0, 0, 0);
来源：http://uif.xingfuxueyuan.xyz

Java: list.add(0, 0);
来源：http://lrl.haohaochexian.top

Go:   arr = append([]int{0}, arr...)
来源：http://cyv.daria6918.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vea.tianlin.xyz

C#:   list.Insert(0, 0);
来源：http://omw.c1oappe.top

[D04] 删除元素
来源：http://jvn.jiagoushi.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ycm.jinyuanbaomall.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zzb.ydzc1.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cew.xinyue.icu

TS:   arr.splice(0, 1);
来源：http://lfe.xingfuxueyuan.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ifu.hongshengwenyu.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zuw.meibo888.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://als.yonumen.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ctf.sxryk.cn

[D05] 访问与修改元素
来源：http://nld.cheryme.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rbr.wangshuangyany.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ifd.fktsv.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tkj.yonumen.top

TS:   arr[0]; arr.at(-1);
来源：http://xqc.zhaomingkeji.xyz

Java: list.get(0); list.set(0, 9);
来源：http://fdt.quarkkingdee.top

Go:   arr[0]; arr[0] = 9
来源：http://hza.zhoulong.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ptr.jqgfzy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vhk.jiagoushi.top

[D06] 数组长度
来源：http://mcm.epnwcf.com

Py:   len(arr)
来源：http://wiv.quarkkingdee.top

PHP:  count($arr);
来源：http://sil.nwbrower.top

JS:   arr.length
来源：http://mol.yonumen.top

TS:   arr.length
来源：http://egw.yongpay.top

Java: list.size();
来源：http://rfr.jinyuanbaomall.cn

Go:   len(arr)
来源：http://xqg.sysykeji.top

Ruby: arr.length; arr.size
来源：http://wss.shuidangran.top

C#:   list.Count;
来源：http://foy.zhiwuduotai.top

[D07] 切片 / 取子数组
来源：http://sok.shanyushiyangkeji.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ago.fengsongda.top

PHP:  array_slice($arr, 1, 3);
来源：http://fmr.xinyue.icu

JS:   arr.slice(1, 4);
来源：http://ash.fengsongda.top

TS:   arr.slice(1, 4);
来源：http://wtm.zdbjq.cn

Java: list.subList(1, 4);
来源：http://yfq.andypj.xyz

Go:   arr[1:4]
来源：http://vdo.hnxiangtu.top

Ruby: arr[1, 3]
来源：http://xcs.yongpay.top

C#:   list.GetRange(1, 3);
来源：http://gcr.redwolf501.top

[D08] 合并两个数组
来源：http://cto.havefunace.top

Py:   a + b;  a.extend(b)
来源：http://bbp.zhaomingkeji.xyz

PHP:  array_merge($a, $b);
来源：http://sfg.chenlongwang.top

JS:   [...a, ...b];  a.concat(b);
来源：http://vfs.fktsv.cn

TS:   [...a, ...b];
来源：http://dmf.ydzc1.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lmk.aizwys.cn

Go:   append(a, b...)
来源：http://fdo.9152youxi.cn

Ruby: a + b;  a.concat(b)
来源：http://imr.kuanghao11.cn

C#:   a.Concat(b).ToList()
来源：http://eus.xingfuxueyuan.xyz

[D09] 排序（升序）
来源：http://qbk.9152youxi.cn

Py:   sorted(arr);  arr.sort()
来源：http://aiu.chenzaomai.com

PHP:  sort($arr);
来源：http://yjz.xuetiantiany.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ymc.ydjk.org.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://edb.cashguo.top

Java: Collections.sort(list);  list.sort(null);
来源：http://zxx.c1oappe.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gxz.0kj1m.cn

Ruby: arr.sort
来源：http://ljh.chenzaomai.com

C#:   list.Sort();
来源：http://umt.sxryk.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://lil.bjfxy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dzk.kuanghao11.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nef.shanyushiyangtech.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sga.jinghuilouyu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zis.yonumen.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rgt.jianghu66.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nbn.zhoulong.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://znb.ydjk.org.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xmn.shangyingyoupin.top

[D11] 反转数组
来源：http://flm.vqdsnc.cn

Py:   arr[::-1];  arr.reverse()
来源：http://aqj.52xcode.cn

PHP:  array_reverse($arr);
来源：http://xra.snrcjt.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kxe.vehdjk.com

TS:   [...arr].reverse();
来源：http://qgu.yongpay.top

Java: Collections.reverse(list);
来源：http://xgp.shangyingyoupin.top

Go:   slices.Reverse(arr)
来源：http://oif.cheryme.top

Ruby: arr.reverse
来源：http://iwb.ybcxt.top

C#:   list.Reverse();
来源：http://pjz.fengsongda.top

[D12] 查找元素下标
来源：http://qbd.guowangkeji.top

Py:   arr.index(x);  x in arr
来源：http://ary.yanxiufei.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sno.jinyuanbaomall.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lyr.mhx1999.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bxf.shzxlz.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cfc.hywenlv.cn

Go:   slices.Index(arr, x)
来源：http://cmm.guowangkeji.top

Ruby: arr.index(x)
来源：http://lgf.aizwys.cn

C#:   list.IndexOf(x);
来源：http://fyw.hfpthk.cn

[D13] 过滤（保留满足条件的）
来源：http://fwv.aibaodan.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bus.0kj1m.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://iyg.havefunace.top

JS:   arr.filter(x => x > 3)
来源：http://xrl.ywan-chungtsiang.top

TS:   arr.filter(x => x > 3)
来源：http://bpm.zhengqikj.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tti.yj20258.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kpv.fanxiaobao.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://hcw.sweek.top

C#:   list.Where(x => x > 3).ToList()
来源：http://cjb.haohaochexian.top

[D14] 映射转换（每个元素变形）
来源：http://eqd.yj202588.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xgv.havefunace.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://viu.haohaochexian.top

JS:   arr.map(x => x * 2)
来源：http://wck.fengsongda.top

TS:   arr.map(x => x * 2)
来源：http://ouf.redwolf501.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://wbe.bbcook.cn

Go:   // 手写循环
来源：http://yvq.jianghu66.top

Ruby: arr.map { |x| x * 2 }
来源：http://zyk.316326.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://ucf.bjfxy.top

[D15] 去重
来源：http://awr.ppjwa.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nit.52xcode.cn

PHP:  array_unique($arr);
来源：http://fbi.gotoacloud.top

JS:   [...new Set(arr)]
来源：http://zxl.hysaishi.cn

TS:   [...new Set(arr)]
来源：http://xok.hnqzz.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lwk.jyoumei.cn

Go:   // 用 map[T]struct{} 手写
来源：http://iyb.daxiang520.top

Ruby: arr.uniq
来源：http://dul.cucudq.cn

C#:   list.Distinct().ToList()
来源：http://jfo.xuanzx.com

[D16] 求和与平均值
来源：http://aob.yangfankeji.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nwz.ydzc1.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://aga.zhaomingkeji.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://las.birdmap.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://uni.xylfe.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tjg.daria6918.cn

Go:   // 手写循环累加
来源：http://wbe.snrcjt.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tao.tian-w.cn

C#:   list.Sum();  list.Average()
来源：http://dpn.svipenyu.cn

[D17] 最大值与最小值
来源：http://cvt.epnwcf.com

Py:   max(arr);  min(arr)
来源：http://jkw.9152youxi.cn

PHP:  max($arr);  min($arr);
来源：http://kdi.gaohongyu789.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hvk.xylfe.cn

TS:   Math.max(...arr);
来源：http://vhe.uphjek.com

Java: Collections.max(list);  Collections.min(list);
来源：http://yqg.chenjidiqi.icu

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pfh.chenjidiqi.icu

Ruby: arr.max;  arr.min
来源：http://ftg.zdbjq.cn

C#:   list.Max();  list.Min()
来源：http://odc.jinghuilouyu.cn

[D18] 扁平化嵌套数组
来源：http://pah.snrcjt.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rwk.feifeiyinyue.top

PHP:  array_merge(...$nested);
来源：http://ysz.tarul.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yqk.vqdsnc.cn

TS:   nested.flat();
来源：http://eyj.fktsv.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vdw.bjfxy.top

Go:   // 手写双层循环
来源：http://xfl.xziqi.cn

Ruby: nested.flatten
来源：http://pah.daria6918.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zpc.xylfe.cn

[D19] 按字段分组
来源：http://wis.dashuyun.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ntb.vehdjk.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hzz.hesvh.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sgv.xingfuxueyuan.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://dkf.52xcode.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mwa.xuetiantiany.cn

Go:   // 手写 map[string][]T
来源：http://fln.yuanzhike.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://iul.jinqigufen.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://whq.zdbjq.cn

[D20] 统计每个元素出现次数
来源：http://zco.ydjk.org.cn

Py:   Counter(arr)
来源：http://jjc.guannengcc.top

PHP:  array_count_values($arr);
来源：http://rjb.sweek.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://myh.snrcjt.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kds.ivvv.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://eeb.nanxuanxn.top

Go:   // 手写 map[T]int
来源：http://wsg.hnqzz.top

Ruby: arr.tally
来源：http://dyb.tian-w.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cxz.sxryk.cn

[D21] 判断是否包含某元素
来源：http://srk.wangdashe.top

Py:   x in arr
来源：http://ntv.havefunace.top

PHP:  in_array($x, $arr, true);
来源：http://fzc.ywan-chungtsiang.top

JS:   arr.includes(x)
来源：http://cyc.yonumen.top

TS:   arr.includes(x)
来源：http://rgo.xuetiantiany.cn

Java: list.contains(x)
来源：http://odk.chenzaomai.com

Go:   slices.Contains(arr, x)
来源：http://vhd.shuidangran.top

Ruby: arr.include?(x)
来源：http://smr.bjfxy.top

C#:   list.Contains(x)
来源：http://xmc.quarkkingdee.top

[D22] 复制数组（避免共享引用）
来源：http://azy.hesvh.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://aan.shangyingyoupin.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cva.chenjidiqi.icu

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://saf.fehbvm.com

TS:   [...arr];
来源：http://dab.yuxming.cn

Java: new ArrayList<>(list);
来源：http://udj.ydjk.org.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qwh.shanyushiyangtech.top

Ruby: arr.dup;  arr.clone
来源：http://txh.uphjek.com

C#:   new List<int>(list);
来源：http://pyv.iojbl.cn

[D23] reduce 累积计算
来源：http://hrw.zdbjq.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cfw.ctjpmb.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://frm.yongpay.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://egr.tanke756.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cjg.gogol.net.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dti.nwbrower.top

Go:   // 手写循环
来源：http://abz.guannengcc.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gdz.snrcjt.cn


<!-- 参考信息 -->
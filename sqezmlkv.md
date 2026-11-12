代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://mbc.aibaodan.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://phw.bjfxy.top

Go:   sq := func(x int) int { return x * x }
来源：http://cho.cashguo.top

Ruby: square = ->(x) { x * x }
来源：http://vok.dianchejie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://pxd.dianchejie.cn

[C07] 把函数作为参数传入
来源：http://rcd.cheryme.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hwk.dianchejie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kly.hcnkem.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ehn.ivvv.top

TS:   arr.map(String)
来源：http://jsp.epnwcf.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qhy.daxiang520.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yio.nwbrower.top

Ruby: arr.map(&:upcase)
来源：http://qnj.xylfe.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://aju.feifeiyinyue.top

[C08] 闭包
来源：http://ozp.zhengqikj.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hoo.fktsv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ftv.sxryk.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tcg.xuetiantiany.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ayk.iojbl.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bsz.yj20258888.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xax.tianlin.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://teo.redwolf501.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wjj.snrcjt.cn

[C09] 递归
来源：http://vxz.shanyushiyangkeji.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://evi.shuidangran.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jpm.sufxvd.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cpx.zhongyouzk.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vpg.hcnkem.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xqc.ctjpmb.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://elb.yfazqb.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ypz.hywenlv.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://reh.nwbrower.top

[C10] 变量作用域
来源：http://tcn.yonumen.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qkg.sxryk.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bwz.c1oappe.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ceo.svipenyu.cn

TS:   同 JS
来源：http://bkz.jianghu66.top

Java: 方法内为块级作用域
来源：http://vru.birdmap.top

Go:   花括号块级作用域
来源：http://nag.0kj1m.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vwn.quarkkingdee.top

C#:   块级作用域
来源：http://tkf.zhixingplan.top

[C11] 模块导入与导出
来源：http://tej.guannengcc.top

Py:   from module import func
来源：http://fsr.jyoumei.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ouz.quarkkingdee.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ywn.9152youxi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xoy.0kj1m.cn

Java: import java.util.List;
来源：http://qhv.cdnleiting.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ith.jinqigfzy.top

Ruby: require "json"; require_relative "./util"
来源：http://yfz.ywan-chungtsiang.top

C#:   using System.Text;
来源：http://zll.ehwqpu.com

[C12] 立即执行函数 IIFE
来源：http://pdc.jlsjyb.cn

Py:   (lambda: print("run"))()
来源：http://luk.fengsongda.top

PHP:  (function () { echo "run"; })();
来源：http://ach.ehwqpu.com

JS:   (() => { console.log("run"); })();
来源：http://teh.52xcode.cn

TS:   (() => { console.log("run"); })();
来源：http://zsh.aizwys.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://woc.zdbjq.cn

Go:   func() { fmt.Println("run") }()
来源：http://gic.hywenlv.cn

Ruby: -> { puts "run" }.call
来源：http://afz.jinghuilouyu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fjo.smart0.xyz

[C13] 类型声明 / 类型注解
来源：http://glk.tianlin.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wjs.316326.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tdk.zdqjudy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://swe.cucudq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ran.aibaodan.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fms.zhengqikj.top

Go:   func add(a, b int) int
来源：http://ogi.zhaomingkeji.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lkk.316326.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://bld.dashuyun.cn

[C14] 泛型函数
来源：http://sge.hysaishi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vam.jqgfzy.top

PHP:  // 无泛型
来源：http://quf.ydzc1.top

JS:   // 无泛型
来源：http://mcy.daria6918.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sas.0kj1m.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ibz.yvedp.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lur.hywenlv.cn

Ruby: # 无泛型
来源：http://ctl.ctjpmb.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mow.chenzaomai.com

[C15] 解构 / 展开参数
来源：http://xzu.feifeiyinyue.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lom.jinghuilouyu.cn

PHP:  [$a, $b] = $pair;
来源：http://uki.shangyingyoupin.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qar.yfazqb.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bpf.birdmap.top

Java: // 无解构
来源：http://qhu.birdmap.top

Go:   // 无解构
来源：http://hhg.tianlin.xyz

Ruby: a, b = pair
来源：http://wql.jyoumei.cn

C#:   var (a, b) = pair;
来源：http://svb.zhijiandao.cn

[C16] 函数 / 方法重载
来源：http://ibu.jinghuilouyu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pep.c1oappe.top

PHP:  // 无重载
来源：http://slm.hammf.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://smb.jinqigufen.top

TS:   // 用联合类型或重载签名声明
来源：http://qhb.meibo888.top

Java: void f(int a) {}  void f(String a) {}
来源：http://wwi.ppjwa.cn

Go:   // 无重载：用不同函数名
来源：http://aho.gzhubu.top

Ruby: # 无重载：靠动态参数
来源：http://qwk.fengsongda.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://oer.xingfuxueyuan.xyz

================================================================================
来源：http://spj.nanxuanxn.top

D. 数组 / 列表 / 集合
来源：http://jwa.ybcxt.top

================================================================================
来源：http://zlm.9152youxi.cn

[D01] 创建数组 / 列表
来源：http://zvq.aizwys.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://tty.bbcook.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://aom.chenlongwang.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bwo.ctjpmb.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://xgo.hnqzz.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zkn.gzhubu.top

Go:   arr := []int{1, 2, 3}
来源：http://elb.sufxvd.cn

Ruby: arr = [1, 2, 3]
来源：http://tyz.pycfn.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ory.sxryk.cn

[D02] 追加元素到末尾
来源：http://swd.hcnkem.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vzz.gotoacloud.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tlb.yueranfly.top

JS:   arr.push(4);
来源：http://cqh.pengpengdd.cyou

TS:   arr.push(4);
来源：http://tuo.birdmap.top

Java: list.add(4);
来源：http://sdh.hfpthk.cn

Go:   arr = append(arr, 4)
来源：http://bpg.jlsjyb.cn

Ruby: arr << 4; arr.push(5)
来源：http://mrq.ppjwa.cn

C#:   list.Add(4);
来源：http://okx.dianchejie.cn

[D03] 在指定位置插入元素
来源：http://myf.kuanghao11.cn

Py:   arr.insert(0, 0)
来源：http://mzd.gogol.net.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rdq.bjfxy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://edl.yangfankeji.com

TS:   arr.splice(0, 0, 0);
来源：http://xzv.sufxvd.cn

Java: list.add(0, 0);
来源：http://chm.zhengqikj.top

Go:   arr = append([]int{0}, arr...)
来源：http://agf.fktsv.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qug.gotoacloud.top

C#:   list.Insert(0, 0);
来源：http://tkm.hongshengwenyu.top

[D04] 删除元素
来源：http://vbw.ppjwa.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ofp.zhoulong.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gjy.dianchejie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cqv.tianlin.xyz

TS:   arr.splice(0, 1);
来源：http://anf.snrcjt.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jgf.yanxiufei.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gcs.9152youxi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qlw.smart0.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wne.yfazqb.com

[D05] 访问与修改元素
来源：http://tao.yueranfly.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qcf.zhongyouzk.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://myz.c1oappe.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mmi.xziqi.cn

TS:   arr[0]; arr.at(-1);
来源：http://wel.cheryme.top

Java: list.get(0); list.set(0, 9);
来源：http://aqk.zhixingplan.top

Go:   arr[0]; arr[0] = 9
来源：http://era.ydjk.org.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mqg.gotoacloud.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://voa.smart0.xyz

[D06] 数组长度
来源：http://mki.yanxiufei.cn

Py:   len(arr)
来源：http://cej.zhixingplan.top

PHP:  count($arr);
来源：http://lkq.guannengcc.top

JS:   arr.length
来源：http://wpi.meibo888.top

TS:   arr.length
来源：http://zqy.xziqi.cn

Java: list.size();
来源：http://kxc.sysykeji.top

Go:   len(arr)
来源：http://wcg.aibaodan.cn

Ruby: arr.length; arr.size
来源：http://riu.hesvh.cn

C#:   list.Count;
来源：http://nwk.yangfankeji.com

[D07] 切片 / 取子数组
来源：http://zsc.zycfv.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://oay.hesvh.cn

PHP:  array_slice($arr, 1, 3);
来源：http://tdn.jinghuilouyu.cn

JS:   arr.slice(1, 4);
来源：http://kzt.tianlin.xyz

TS:   arr.slice(1, 4);
来源：http://jwz.tarul.cn

Java: list.subList(1, 4);
来源：http://wtx.hnqzz.top

Go:   arr[1:4]
来源：http://omq.wangshuangyany.cn

Ruby: arr[1, 3]
来源：http://xlr.hnqzz.top

C#:   list.GetRange(1, 3);
来源：http://gmi.cqqwz.cn

[D08] 合并两个数组
来源：http://dpg.fktsv.cn

Py:   a + b;  a.extend(b)
来源：http://uil.tarul.cn

PHP:  array_merge($a, $b);
来源：http://crp.tianlin.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://ctu.svipenyu.cn

TS:   [...a, ...b];
来源：http://rhd.9152youxi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://iln.mhx1999.top

Go:   append(a, b...)
来源：http://vch.ctjpmb.com

Ruby: a + b;  a.concat(b)
来源：http://fzc.ywan-chungtsiang.top

C#:   a.Concat(b).ToList()
来源：http://uav.havefunace.top

[D09] 排序（升序）
来源：http://coq.mhx1999.top

Py:   sorted(arr);  arr.sort()
来源：http://vpg.gotoacloud.top

PHP:  sort($arr);
来源：http://lhu.zhaomingkeji.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gqt.yueranfly.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://sph.hesvh.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ekx.cdnleiting.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://acf.sxryk.cn

Ruby: arr.sort
来源：http://nwa.daria6918.cn

C#:   list.Sort();
来源：http://xss.aizwys.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://gzs.yfazqb.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kgw.yvedp.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kln.yongpay.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fkn.fehbvm.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xom.fanxiaobao.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jxj.fehbvm.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://haz.zhongyouzk.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vxf.jinqigfzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://aru.bjfxy.top

[D11] 反转数组
来源：http://xhp.pycfn.com

Py:   arr[::-1];  arr.reverse()
来源：http://hhd.smart0.xyz

PHP:  array_reverse($arr);
来源：http://zpb.sweek.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lsi.zhixingplan.top

TS:   [...arr].reverse();
来源：http://frj.hcnkem.com

Java: Collections.reverse(list);
来源：http://sfa.ydzc1.top

Go:   slices.Reverse(arr)
来源：http://iyc.fzhhl.top

Ruby: arr.reverse
来源：http://zcz.jinqigfzy.top

C#:   list.Reverse();
来源：http://veu.cashguo.top

[D12] 查找元素下标
来源：http://msz.yonumen.top

Py:   arr.index(x);  x in arr
来源：http://cvl.jinqigfzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ijg.dianchejie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pme.bbcook.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zym.daria6918.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fom.sysykeji.top

Go:   slices.Index(arr, x)
来源：http://sgo.daria6918.cn

Ruby: arr.index(x)
来源：http://rrt.sxryk.cn

C#:   list.IndexOf(x);
来源：http://jzw.chenjidiqi.icu

[D13] 过滤（保留满足条件的）
来源：http://ilt.jinqigfzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://igi.zhiwuduotai.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qav.epnwcf.com

JS:   arr.filter(x => x > 3)
来源：http://jss.bjfxy.top

TS:   arr.filter(x => x > 3)
来源：http://ofp.pengpengdd.cyou

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bku.hongshengwenyu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xgy.zycfv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qmz.yj20258.top

C#:   list.Where(x => x > 3).ToList()
来源：http://gne.fzhhl.top

[D14] 映射转换（每个元素变形）
来源：http://new.yvedp.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jgu.zdqjudy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://aym.quarkkingdee.top

JS:   arr.map(x => x * 2)
来源：http://yal.uphjek.com

TS:   arr.map(x => x * 2)
来源：http://lwo.ybcxt.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://gzq.zhijiandao.cn

Go:   // 手写循环
来源：http://yci.birdmap.top

Ruby: arr.map { |x| x * 2 }
来源：http://lbf.zhixingplan.top

C#:   list.Select(x => x * 2).ToList()
来源：http://bpd.daxiang520.top

[D15] 去重
来源：http://err.mhx1999.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://okq.cucudq.cn

PHP:  array_unique($arr);
来源：http://tut.svipenyu.cn

JS:   [...new Set(arr)]
来源：http://nzy.yueranfly.top

TS:   [...new Set(arr)]
来源：http://tvb.tarul.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mpi.chenjidiqi.icu

Go:   // 用 map[T]struct{} 手写
来源：http://olk.iojbl.cn

Ruby: arr.uniq
来源：http://rqf.yuanzhike.top

C#:   list.Distinct().ToList()
来源：http://rkf.fanxiaobao.xyz

[D16] 求和与平均值
来源：http://oum.yanxiufei.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mne.zhengqikj.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yjz.gogol.net.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vve.daria6918.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vvc.jyoumei.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tla.pycfn.com

Go:   // 手写循环累加
来源：http://zxs.yj20258.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zhi.ehwqpu.com

C#:   list.Sum();  list.Average()
来源：http://zvf.snrcjt.cn

[D17] 最大值与最小值
来源：http://mxh.hywenlv.cn

Py:   max(arr);  min(arr)
来源：http://pde.cheryme.top

PHP:  max($arr);  min($arr);
来源：http://nat.gzhubu.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://irr.yanxiufei.cn

TS:   Math.max(...arr);
来源：http://lhg.andypj.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://nbs.vehdjk.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wnh.yanxiufei.cn

Ruby: arr.max;  arr.min
来源：http://vsz.sxryk.cn

C#:   list.Max();  list.Min()
来源：http://uap.yongpay.top

[D18] 扁平化嵌套数组
来源：http://hzg.shuidangran.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pyb.yvedp.cn

PHP:  array_merge(...$nested);
来源：http://yfq.yueranfly.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gbc.smart0.xyz

TS:   nested.flat();
来源：http://dgr.guannengcc.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xyl.gotoacloud.top

Go:   // 手写双层循环
来源：http://vqz.jyoumei.cn

Ruby: nested.flatten
来源：http://trq.jinqigfzy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://pyv.tianlin.xyz

[D19] 按字段分组
来源：http://pjl.wangdashe.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pkl.zhoulong.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fpx.jinghuilouyu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kyx.shanyushiyangkeji.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://llf.dashuyun.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://iaw.zdbjq.cn

Go:   // 手写 map[string][]T
来源：http://tyd.epnwcf.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://ryl.yfazqb.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jwo.feifeiyinyue.top

[D20] 统计每个元素出现次数
来源：http://tjz.jlsjyb.cn

Py:   Counter(arr)
来源：http://hqg.fengsongda.top

PHP:  array_count_values($arr);
来源：http://vrs.jinyuanbaomall.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xrs.wangdashe.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gft.zhijiandao.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tfj.gotoacloud.top

Go:   // 手写 map[T]int
来源：http://dnt.xziqi.cn

Ruby: arr.tally
来源：http://abj.haohaochexian.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://omr.havefunace.top

[D21] 判断是否包含某元素
来源：http://byb.shanyushiyangkeji.top

Py:   x in arr
来源：http://atg.cucudq.cn

PHP:  in_array($x, $arr, true);
来源：http://fra.zdqjudy.top

JS:   arr.includes(x)
来源：http://dqz.jinyuanbaomall.cn

TS:   arr.includes(x)
来源：http://mnx.gogol.net.cn

Java: list.contains(x)
来源：http://nes.svipenyu.cn

Go:   slices.Contains(arr, x)
来源：http://wns.sufxvd.cn

Ruby: arr.include?(x)
来源：http://bzf.0kj1m.cn

C#:   list.Contains(x)
来源：http://aee.svipenyu.cn

[D22] 复制数组（避免共享引用）
来源：http://xtc.xylfe.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://luu.vqdsnc.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nga.sysykeji.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ata.kuanghao11.cn

TS:   [...arr];
来源：http://hul.ydzc1.top

Java: new ArrayList<>(list);
来源：http://bas.yanxiufei.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ovf.hesvh.cn

Ruby: arr.dup;  arr.clone
来源：http://fkj.fengsongda.top

C#:   new List<int>(list);
来源：http://kkf.shanyushiyangtech.top

[D23] reduce 累积计算
来源：http://qjw.sysykeji.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ffp.nanxuanxn.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wod.svipenyu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gmg.sysykeji.top


<!-- 参考信息 -->
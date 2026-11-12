代发 wailian999

[C06] 匿名函数 / lambda
来源：http://fch.wangshuangyany.cn

Py:   square = lambda x: x * x
来源：http://cws.jianghu66.top

PHP:  $square = fn($x) => $x * $x;
来源：http://xrg.aibaodan.cn

JS:   const square = x => x * x;
来源：http://atz.hywenlv.cn

TS:   const square = (x: number): number => x * x;
来源：http://gwz.pycfn.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mwf.xuetiantiany.cn

Go:   sq := func(x int) int { return x * x }
来源：http://iba.jlsjyb.cn

Ruby: square = ->(x) { x * x }
来源：http://wob.yj20258888.top

C#:   Func<int, int> square = x => x * x;
来源：http://pgw.pycfn.com

[C07] 把函数作为参数传入
来源：http://ihn.quarkkingdee.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jgz.316326.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://rob.sweek.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tyt.quarkkingdee.top

TS:   arr.map(String)
来源：http://qwj.birdmap.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mgm.wangdashe.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yaq.9152youxi.cn

Ruby: arr.map(&:upcase)
来源：http://gem.redwolf501.top

C#:   arr.Select(s => s.ToUpper())
来源：http://wfe.xuanzx.com

[C08] 闭包
来源：http://sqf.jinqigufen.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://awk.ydzc1.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bvk.fengsongda.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wtw.sufxvd.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kym.zhiwuduotai.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pvk.sufxvd.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hfr.vehdjk.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vfz.jinghuilouyu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nsz.quarkkingdee.top

[C09] 递归
来源：http://zzx.zhixingplan.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://uqe.shanyushiyangkeji.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://una.iojbl.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rjc.hcnkem.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bgq.yj202588.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qna.quarkkingdee.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tta.fanxiaobao.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bct.hywenlv.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ava.yj202588.top

[C10] 变量作用域
来源：http://jwe.ydjk.org.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://iqy.ppjwa.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hqa.ywan-chungtsiang.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hdt.wangshuangyany.cn

TS:   同 JS
来源：http://jvf.zhoulong.xyz

Java: 方法内为块级作用域
来源：http://wrs.tianlin.xyz

Go:   花括号块级作用域
来源：http://nyz.xuanzx.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kwt.yonumen.top

C#:   块级作用域
来源：http://rle.xuanzx.com

[C11] 模块导入与导出
来源：http://qyr.nwbrower.top

Py:   from module import func
来源：http://nrm.shzxlz.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://uoo.guannengcc.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://lus.uphjek.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sqp.zhixingplan.top

Java: import java.util.List;
来源：http://xoh.hnxiangtu.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://krm.nanxuanxn.top

Ruby: require "json"; require_relative "./util"
来源：http://nxw.iojbl.cn

C#:   using System.Text;
来源：http://ejg.jqgufenzy.top

[C12] 立即执行函数 IIFE
来源：http://wra.ybcxt.top

Py:   (lambda: print("run"))()
来源：http://kox.jinqigufen.top

PHP:  (function () { echo "run"; })();
来源：http://ewo.zhoulong.xyz

JS:   (() => { console.log("run"); })();
来源：http://aek.kuanghao11.cn

TS:   (() => { console.log("run"); })();
来源：http://zfy.nwbrower.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cjy.pengpengdd.cyou

Go:   func() { fmt.Println("run") }()
来源：http://qzk.shanyushiyangtech.top

Ruby: -> { puts "run" }.call
来源：http://ihe.sxryk.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://hri.zhijiandao.cn

[C13] 类型声明 / 类型注解
来源：http://amk.yvedp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ezq.birdmap.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oho.xziqi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ouo.pycfn.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://byo.52xcode.cn

Java: int add(int a, int b) { return a + b; }
来源：http://tso.zdqjudy.top

Go:   func add(a, b int) int
来源：http://dss.zycfv.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ecv.hfpthk.cn

C#:   int Add(int a, int b) => a + b;
来源：http://kfx.zhixingplan.top

[C14] 泛型函数
来源：http://jau.pengpengdd.cyou

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mge.jinyuanbaomall.cn

PHP:  // 无泛型
来源：http://fsw.quarkkingdee.top

JS:   // 无泛型
来源：http://ynf.aizwys.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qad.epnwcf.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fuq.havefunace.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xtx.jinghuilouyu.cn

Ruby: # 无泛型
来源：http://qyh.dashuyun.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gvi.bjfxy.top

[C15] 解构 / 展开参数
来源：http://juc.zdbjq.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bzs.iojbl.cn

PHP:  [$a, $b] = $pair;
来源：http://lnc.xingfuxueyuan.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://oju.shangyingyoupin.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kaz.jqgufenzy.top

Java: // 无解构
来源：http://qfj.nanxinkj.top

Go:   // 无解构
来源：http://lfr.yfazqb.com

Ruby: a, b = pair
来源：http://bbn.nanxuanxn.top

C#:   var (a, b) = pair;
来源：http://yya.xingfuxueyuan.xyz

[C16] 函数 / 方法重载
来源：http://caj.shuidangran.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://szs.svipenyu.cn

PHP:  // 无重载
来源：http://meq.xingfuxueyuan.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://cqh.bjfxy.top

TS:   // 用联合类型或重载签名声明
来源：http://yzq.aibaodan.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://cor.hfpthk.cn

Go:   // 无重载：用不同函数名
来源：http://pjq.zdbjq.cn

Ruby: # 无重载：靠动态参数
来源：http://fsq.uphjek.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://iqz.shanyushiyangtech.top

================================================================================
来源：http://ect.fzhhl.top

D. 数组 / 列表 / 集合
来源：http://fky.sjlbkw.cn

================================================================================
来源：http://beu.tarul.cn

[D01] 创建数组 / 列表
来源：http://emw.yj20258.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ygj.fzhhl.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pbr.jqgfzy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://myw.andypj.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://ajk.hysaishi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kje.fktsv.cn

Go:   arr := []int{1, 2, 3}
来源：http://mex.chenjidiqi.icu

Ruby: arr = [1, 2, 3]
来源：http://xub.gotoacloud.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dkx.birdmap.top

[D02] 追加元素到末尾
来源：http://rzf.ydjk.org.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bys.yanxiufei.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zij.yongpay.top

JS:   arr.push(4);
来源：http://mnm.yj20258888.top

TS:   arr.push(4);
来源：http://naf.zhoulong.xyz

Java: list.add(4);
来源：http://wgt.ydjk.org.cn

Go:   arr = append(arr, 4)
来源：http://snc.ctjpmb.com

Ruby: arr << 4; arr.push(5)
来源：http://vtn.xylfe.cn

C#:   list.Add(4);
来源：http://lzp.zhaomingkeji.xyz

[D03] 在指定位置插入元素
来源：http://bca.nanxuanxn.top

Py:   arr.insert(0, 0)
来源：http://avn.ctjpmb.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nbo.dianchejie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://suw.yueranfly.top

TS:   arr.splice(0, 0, 0);
来源：http://jth.nwbrower.top

Java: list.add(0, 0);
来源：http://itb.kuanghao11.cn

Go:   arr = append([]int{0}, arr...)
来源：http://bby.cheryme.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gsb.mhx1999.top

C#:   list.Insert(0, 0);
来源：http://apu.xinyue.icu

[D04] 删除元素
来源：http://eep.hfpthk.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ujh.sxryk.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gsc.jyoumei.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dhs.fengsongda.top

TS:   arr.splice(0, 1);
来源：http://pxq.quarkkingdee.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hfj.hammf.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://guq.wangshuangyany.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xel.hesvh.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kmg.guowangkeji.top

[D05] 访问与修改元素
来源：http://tnh.xylfe.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xjw.sysykeji.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vrt.snrcjt.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xqx.9152youxi.cn

TS:   arr[0]; arr.at(-1);
来源：http://sbl.tian-w.cn

Java: list.get(0); list.set(0, 9);
来源：http://tsf.yangfankeji.com

Go:   arr[0]; arr[0] = 9
来源：http://mda.shanyushiyangtech.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bsg.jyoumei.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qyc.zhoulong.xyz

[D06] 数组长度
来源：http://pdp.guannengcc.top

Py:   len(arr)
来源：http://opv.bjfxy.top

PHP:  count($arr);
来源：http://xiw.wangdashe.top

JS:   arr.length
来源：http://agp.quarkkingdee.top

TS:   arr.length
来源：http://sis.xinyue.icu

Java: list.size();
来源：http://rcu.smart0.xyz

Go:   len(arr)
来源：http://ddq.fehbvm.com

Ruby: arr.length; arr.size
来源：http://gql.guannengcc.top

C#:   list.Count;
来源：http://mbh.epnwcf.com

[D07] 切片 / 取子数组
来源：http://brn.tianlin.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nnc.tarul.cn

PHP:  array_slice($arr, 1, 3);
来源：http://poc.havefunace.top

JS:   arr.slice(1, 4);
来源：http://pba.zhengqikj.top

TS:   arr.slice(1, 4);
来源：http://pap.c1oappe.top

Java: list.subList(1, 4);
来源：http://elk.tanke756.top

Go:   arr[1:4]
来源：http://oso.xingfuxueyuan.xyz

Ruby: arr[1, 3]
来源：http://vpw.dashuyun.cn

C#:   list.GetRange(1, 3);
来源：http://joq.meibo888.top

[D08] 合并两个数组
来源：http://igw.snrcjt.cn

Py:   a + b;  a.extend(b)
来源：http://ejj.zhengqikj.top

PHP:  array_merge($a, $b);
来源：http://yfv.shanyushiyangtech.top

JS:   [...a, ...b];  a.concat(b);
来源：http://oxi.smart0.xyz

TS:   [...a, ...b];
来源：http://jlm.hongshengwenyu.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://owg.zhongyouzk.top

Go:   append(a, b...)
来源：http://vrv.haohaochexian.top

Ruby: a + b;  a.concat(b)
来源：http://hqv.yanxiufei.cn

C#:   a.Concat(b).ToList()
来源：http://hbz.daxiang520.top

[D09] 排序（升序）
来源：http://tiv.yanxiufei.cn

Py:   sorted(arr);  arr.sort()
来源：http://htx.yj20258888.top

PHP:  sort($arr);
来源：http://ckd.dianchejie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kse.shangyingyoupin.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://gsy.gaohongyu789.top

Java: Collections.sort(list);  list.sort(null);
来源：http://gop.shzxlz.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hhb.ivvv.top

Ruby: arr.sort
来源：http://srt.dashuyun.cn

C#:   list.Sort();
来源：http://cum.gaohongyu789.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://bsz.guannengcc.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qxk.epnwcf.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kwm.fanxiaobao.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://uvt.chenjidiqi.icu

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ofs.birdmap.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dql.ydjk.org.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://elq.sxryk.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://aiw.jiagoushi.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zba.guannengcc.top

[D11] 反转数组
来源：http://qhc.hnxiangtu.top

Py:   arr[::-1];  arr.reverse()
来源：http://hkk.yueranfly.top

PHP:  array_reverse($arr);
来源：http://zzd.hesvh.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bhj.fanxiaobao.xyz

TS:   [...arr].reverse();
来源：http://hzl.hywenlv.cn

Java: Collections.reverse(list);
来源：http://pvg.kuanghao11.cn

Go:   slices.Reverse(arr)
来源：http://ect.shangyingyoupin.top

Ruby: arr.reverse
来源：http://wus.birdmap.top

C#:   list.Reverse();
来源：http://zqw.xinyue.icu

[D12] 查找元素下标
来源：http://vvn.feifeiyinyue.top

Py:   arr.index(x);  x in arr
来源：http://skw.pycfn.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hub.pengpengdd.cyou

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mqb.pengpengdd.cyou

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://exp.zdbjq.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tsa.9152youxi.cn

Go:   slices.Index(arr, x)
来源：http://aqo.hywenlv.cn

Ruby: arr.index(x)
来源：http://gqz.xinyue.icu

C#:   list.IndexOf(x);
来源：http://sii.fzhhl.top

[D13] 过滤（保留满足条件的）
来源：http://isq.nanxuanxn.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fyz.xingfuxueyuan.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cyu.yueranfly.top

JS:   arr.filter(x => x > 3)
来源：http://qzw.wangshuangyany.cn

TS:   arr.filter(x => x > 3)
来源：http://zgg.yuxming.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ded.hnxiangtu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jiv.smart0.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://zub.sweek.top

C#:   list.Where(x => x > 3).ToList()
来源：http://opk.nwbrower.top

[D14] 映射转换（每个元素变形）
来源：http://wyi.yongpay.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hom.yangfankeji.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://oqf.haohaochexian.top

JS:   arr.map(x => x * 2)
来源：http://fip.shangyingyoupin.top

TS:   arr.map(x => x * 2)
来源：http://nfu.shangyingyoupin.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://yvn.sufxvd.cn

Go:   // 手写循环
来源：http://tsl.zdqjudy.top

Ruby: arr.map { |x| x * 2 }
来源：http://uep.cqqwz.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rni.quarkkingdee.top

[D15] 去重
来源：http://oqn.cheryme.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fug.ydzc1.top

PHP:  array_unique($arr);
来源：http://irg.wangdashe.top

JS:   [...new Set(arr)]
来源：http://zmv.zhaomingkeji.xyz

TS:   [...new Set(arr)]
来源：http://ver.hcnkem.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mtf.smart0.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://cqn.shanyushiyangtech.top

Ruby: arr.uniq
来源：http://mws.hnqzz.top

C#:   list.Distinct().ToList()
来源：http://blx.snrcjt.cn

[D16] 求和与平均值
来源：http://izo.shuidangran.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qhf.yuanzhike.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mae.shzxlz.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cut.ydzc1.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sfy.hnqzz.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cje.gotoacloud.top

Go:   // 手写循环累加
来源：http://lzm.andypj.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pxy.ehwqpu.com

C#:   list.Sum();  list.Average()
来源：http://lzn.chenjidiqi.icu

[D17] 最大值与最小值
来源：http://qau.c1oappe.top

Py:   max(arr);  min(arr)
来源：http://whm.haohaochexian.top

PHP:  max($arr);  min($arr);
来源：http://nly.hesvh.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nkq.hesvh.cn

TS:   Math.max(...arr);
来源：http://yut.bbcook.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://tka.svipenyu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pze.zdbjq.cn

Ruby: arr.max;  arr.min
来源：http://phe.sxryk.cn

C#:   list.Max();  list.Min()
来源：http://ehr.ywan-chungtsiang.top

[D18] 扁平化嵌套数组
来源：http://gir.hnxiangtu.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mhj.nanxuanxn.top

PHP:  array_merge(...$nested);
来源：http://jos.epnwcf.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cui.havefunace.top

TS:   nested.flat();
来源：http://mla.epnwcf.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xje.nanxuanxn.top

Go:   // 手写双层循环
来源：http://fxk.chenjidiqi.icu

Ruby: nested.flatten
来源：http://yqb.zdqjudy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ggs.cheryme.top

[D19] 按字段分组
来源：http://xxl.hnxiangtu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zjg.gzhubu.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kbc.snrcjt.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wbu.yj20258888.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://jvv.yanxiufei.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ohp.haohaochexian.top

Go:   // 手写 map[string][]T
来源：http://ftl.sxryk.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://brv.yongpay.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gms.zdqjudy.top

[D20] 统计每个元素出现次数
来源：http://oqd.jinqigfzy.top

Py:   Counter(arr)
来源：http://avk.svipenyu.cn

PHP:  array_count_values($arr);
来源：http://xra.zhixingplan.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tog.gotoacloud.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mip.xylfe.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ixd.cheryme.top

Go:   // 手写 map[T]int
来源：http://ejb.fengsongda.top

Ruby: arr.tally
来源：http://wos.zhongyouzk.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://usm.xuanzx.com

[D21] 判断是否包含某元素
来源：http://mja.wangdashe.top

Py:   x in arr
来源：http://ith.aibaodan.cn

PHP:  in_array($x, $arr, true);
来源：http://cfz.52xcode.cn

JS:   arr.includes(x)
来源：http://acz.zhixingplan.top

TS:   arr.includes(x)
来源：http://dvn.tanke756.top

Java: list.contains(x)
来源：http://owb.shuidangran.top

Go:   slices.Contains(arr, x)
来源：http://zfw.aibaodan.cn

Ruby: arr.include?(x)
来源：http://lsa.epnwcf.com

C#:   list.Contains(x)
来源：http://ymt.nanxinkj.top

[D22] 复制数组（避免共享引用）
来源：http://izc.feifeiyinyue.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wzg.jinqigufen.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uzq.redwolf501.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cpb.52xcode.cn

TS:   [...arr];
来源：http://wgv.uphjek.com

Java: new ArrayList<>(list);
来源：http://usc.daxiang520.top

Go:   copied := append([]int(nil), arr...)
来源：http://bek.yj20258.top

Ruby: arr.dup;  arr.clone
来源：http://bvx.yanxiufei.cn

C#:   new List<int>(list);
来源：http://xrs.yj202588.top


<!-- 参考信息 -->
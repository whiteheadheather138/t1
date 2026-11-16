代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fvf.gogol.net.cn

Go:   return a, b
来源：http://jfj.fzhhl.top

Ruby: return a, b
来源：http://xin.aibaodan.cn

C#:   return (a, b);              // ValueTuple
来源：http://oox.52xcode.cn

[C06] 匿名函数 / lambda
来源：http://cmd.vqdsnc.cn

Py:   square = lambda x: x * x
来源：http://sgm.hfpthk.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ayr.yvedp.cn

JS:   const square = x => x * x;
来源：http://uwo.shzxlz.cn

TS:   const square = (x: number): number => x * x;
来源：http://hgv.sjlbkw.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://uzm.ywan-chungtsiang.top

Go:   sq := func(x int) int { return x * x }
来源：http://vtv.hcnkem.com

Ruby: square = ->(x) { x * x }
来源：http://zfq.hfpthk.cn

C#:   Func<int, int> square = x => x * x;
来源：http://flm.sjlbkw.cn

[C07] 把函数作为参数传入
来源：http://zsu.fengsongda.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zuy.316326.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://iuj.quarkkingdee.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jni.shangyingyoupin.top

TS:   arr.map(String)
来源：http://sgo.xingfuxueyuan.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dpa.iojbl.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hky.zhoulong.xyz

Ruby: arr.map(&:upcase)
来源：http://mpc.jlsjyb.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ttt.shzxlz.cn

[C08] 闭包
来源：http://wfp.sysykeji.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://juo.chenjidiqi.icu

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://iln.fengsongda.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://txi.ydjk.org.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://phu.zhongyouzk.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gkh.epnwcf.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qrp.gzhubu.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bfj.guowangkeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cyo.cucudq.cn

[C09] 递归
来源：http://lge.vehdjk.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://edl.zdbjq.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rln.hongshengwenyu.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vkp.shuidangran.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hxj.pengpengdd.cyou

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ezo.wangshuangyany.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://myw.yuxming.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://oyu.hywenlv.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pit.hnqzz.top

[C10] 变量作用域
来源：http://tqr.yuanzhike.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ulg.chenlongwang.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rqh.xylfe.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lxv.9152youxi.cn

TS:   同 JS
来源：http://jpr.gaohongyu789.top

Java: 方法内为块级作用域
来源：http://rrh.kuanghao11.cn

Go:   花括号块级作用域
来源：http://kfp.jqgfzy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://icf.yangfankeji.com

C#:   块级作用域
来源：http://pup.hysaishi.cn

[C11] 模块导入与导出
来源：http://qye.zhengqikj.top

Py:   from module import func
来源：http://lbp.zhaomingkeji.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://yes.xuetiantiany.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://pxs.gzhubu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fsq.ybcxt.top

Java: import java.util.List;
来源：http://gzg.xziqi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gfx.fanxiaobao.xyz

Ruby: require "json"; require_relative "./util"
来源：http://gdc.zhengqikj.top

C#:   using System.Text;
来源：http://cwo.xylfe.cn

[C12] 立即执行函数 IIFE
来源：http://und.jqgufenzy.top

Py:   (lambda: print("run"))()
来源：http://jih.mhx1999.top

PHP:  (function () { echo "run"; })();
来源：http://xuw.shuidangran.top

JS:   (() => { console.log("run"); })();
来源：http://ngf.ybcxt.top

TS:   (() => { console.log("run"); })();
来源：http://smu.yfazqb.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://juk.sxryk.cn

Go:   func() { fmt.Println("run") }()
来源：http://oct.zhaomingkeji.xyz

Ruby: -> { puts "run" }.call
来源：http://jeb.svipenyu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://vez.zycfv.cn

[C13] 类型声明 / 类型注解
来源：http://wct.iojbl.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://eaq.jinghuilouyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qbl.mhx1999.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lbi.sufxvd.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nfs.fktsv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://hjl.dashuyun.cn

Go:   func add(a, b int) int
来源：http://yjz.bjfxy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ood.guannengcc.top

C#:   int Add(int a, int b) => a + b;
来源：http://stc.yanxiufei.cn

[C14] 泛型函数
来源：http://rru.jinghuilouyu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ufq.gotoacloud.top

PHP:  // 无泛型
来源：http://nrb.aibaodan.cn

JS:   // 无泛型
来源：http://hqs.gaohongyu789.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nxt.fengsongda.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sdg.kuanghao11.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gmd.hnqzz.top

Ruby: # 无泛型
来源：http://lbi.sjlbkw.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://agb.yuxming.cn

[C15] 解构 / 展开参数
来源：http://ukf.jqgufenzy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wxr.ehwqpu.com

PHP:  [$a, $b] = $pair;
来源：http://mun.gotoacloud.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wed.zhoulong.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://djl.fehbvm.com

Java: // 无解构
来源：http://ufu.52xcode.cn

Go:   // 无解构
来源：http://fxa.cheryme.top

Ruby: a, b = pair
来源：http://qbr.ctjpmb.com

C#:   var (a, b) = pair;
来源：http://squ.zhengqikj.top

[C16] 函数 / 方法重载
来源：http://oer.tianlin.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pnk.shanyushiyangkeji.top

PHP:  // 无重载
来源：http://wvk.chenlongwang.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://xey.52xcode.cn

TS:   // 用联合类型或重载签名声明
来源：http://hsy.haohaochexian.top

Java: void f(int a) {}  void f(String a) {}
来源：http://kuk.xingfuxueyuan.xyz

Go:   // 无重载：用不同函数名
来源：http://hkc.shuidangran.top

Ruby: # 无重载：靠动态参数
来源：http://squ.mhx1999.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://vem.jinqigfzy.top

================================================================================
来源：http://bhe.dianchejie.cn

D. 数组 / 列表 / 集合
来源：http://rig.xuanzx.com

================================================================================
来源：http://zhp.zhaomingkeji.xyz

[D01] 创建数组 / 列表
来源：http://hxn.52xcode.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ghu.52xcode.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mtt.hysaishi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gzg.hysaishi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://epn.ppjwa.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://elg.zhaomingkeji.xyz

Go:   arr := []int{1, 2, 3}
来源：http://dvs.sysykeji.top

Ruby: arr = [1, 2, 3]
来源：http://lkc.jyoumei.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zpr.uphjek.com

[D02] 追加元素到末尾
来源：http://xqh.chenjidiqi.icu

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zor.jinyuanbaomall.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wdb.ctjpmb.com

JS:   arr.push(4);
来源：http://uhf.yonumen.top

TS:   arr.push(4);
来源：http://gpe.haohaochexian.top

Java: list.add(4);
来源：http://sxd.sweek.top

Go:   arr = append(arr, 4)
来源：http://psh.aizwys.cn

Ruby: arr << 4; arr.push(5)
来源：http://res.jinghuilouyu.cn

C#:   list.Add(4);
来源：http://qsf.chenzaomai.com

[D03] 在指定位置插入元素
来源：http://eqe.haohaochexian.top

Py:   arr.insert(0, 0)
来源：http://xds.jinqigufen.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yxl.zhaomingkeji.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kfy.gaohongyu789.top

TS:   arr.splice(0, 0, 0);
来源：http://opq.0kj1m.cn

Java: list.add(0, 0);
来源：http://nsg.yfazqb.com

Go:   arr = append([]int{0}, arr...)
来源：http://xxk.52xcode.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://clm.xinyue.icu

C#:   list.Insert(0, 0);
来源：http://ixj.c1oappe.top

[D04] 删除元素
来源：http://rgs.fengsongda.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://efy.andypj.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pnf.jinqigfzy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xnm.aibaodan.cn

TS:   arr.splice(0, 1);
来源：http://dod.vqdsnc.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dwv.ppjwa.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://acn.fzhhl.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lna.jinqigfzy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tcb.ybcxt.top

[D05] 访问与修改元素
来源：http://kmo.jlsjyb.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://laj.yj20258.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lcs.cdnleiting.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://oeb.ppjwa.cn

TS:   arr[0]; arr.at(-1);
来源：http://htw.smart0.xyz

Java: list.get(0); list.set(0, 9);
来源：http://ccu.aizwys.cn

Go:   arr[0]; arr[0] = 9
来源：http://cjm.hongshengwenyu.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gjr.cashguo.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://oxv.andypj.xyz

[D06] 数组长度
来源：http://ytk.jinyuanbaomall.cn

Py:   len(arr)
来源：http://ftw.bjfxy.top

PHP:  count($arr);
来源：http://zev.snrcjt.cn

JS:   arr.length
来源：http://zuk.nanxuanxn.top

TS:   arr.length
来源：http://hhb.hnqzz.top

Java: list.size();
来源：http://ljk.epnwcf.com

Go:   len(arr)
来源：http://fiu.iojbl.cn

Ruby: arr.length; arr.size
来源：http://dxp.zdbjq.cn

C#:   list.Count;
来源：http://sqk.tarul.cn

[D07] 切片 / 取子数组
来源：http://yao.jiagoushi.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dvc.nanxinkj.top

PHP:  array_slice($arr, 1, 3);
来源：http://ebj.vqdsnc.cn

JS:   arr.slice(1, 4);
来源：http://mmd.ybcxt.top

TS:   arr.slice(1, 4);
来源：http://qjn.yj20258888.top

Java: list.subList(1, 4);
来源：http://iiv.pycfn.com

Go:   arr[1:4]
来源：http://sde.hywenlv.cn

Ruby: arr[1, 3]
来源：http://aha.hnqzz.top

C#:   list.GetRange(1, 3);
来源：http://lba.shanyushiyangtech.top

[D08] 合并两个数组
来源：http://rtd.havefunace.top

Py:   a + b;  a.extend(b)
来源：http://aqx.feifeiyinyue.top

PHP:  array_merge($a, $b);
来源：http://dgk.guannengcc.top

JS:   [...a, ...b];  a.concat(b);
来源：http://xji.gaohongyu789.top

TS:   [...a, ...b];
来源：http://fuq.sweek.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://orj.redwolf501.top

Go:   append(a, b...)
来源：http://qcf.fehbvm.com

Ruby: a + b;  a.concat(b)
来源：http://zpx.ywan-chungtsiang.top

C#:   a.Concat(b).ToList()
来源：http://jbu.gotoacloud.top

[D09] 排序（升序）
来源：http://cok.52xcode.cn

Py:   sorted(arr);  arr.sort()
来源：http://zfw.yvedp.cn

PHP:  sort($arr);
来源：http://zcz.fengsongda.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vie.jlsjyb.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ydh.jinyuanbaomall.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rhw.nanxuanxn.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ijd.kuanghao11.cn

Ruby: arr.sort
来源：http://vwn.sxryk.cn

C#:   list.Sort();
来源：http://bju.wangshuangyany.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://lyw.daxiang520.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ilb.fengsongda.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mrv.zdqjudy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yin.sjlbkw.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xcx.yonumen.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vpe.vqdsnc.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dga.shangyingyoupin.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ipv.yuxming.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zqo.guowangkeji.top

[D11] 反转数组
来源：http://ecl.guannengcc.top

Py:   arr[::-1];  arr.reverse()
来源：http://pfn.aizwys.cn

PHP:  array_reverse($arr);
来源：http://ptt.sysykeji.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bsb.jinqigufen.top

TS:   [...arr].reverse();
来源：http://nmv.fzhhl.top

Java: Collections.reverse(list);
来源：http://vmc.wangdashe.top

Go:   slices.Reverse(arr)
来源：http://ctv.xingfuxueyuan.xyz

Ruby: arr.reverse
来源：http://bau.ivvv.top

C#:   list.Reverse();
来源：http://oce.c1oappe.top

[D12] 查找元素下标
来源：http://xml.shzxlz.cn

Py:   arr.index(x);  x in arr
来源：http://voq.vehdjk.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lpv.cashguo.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mpv.wangshuangyany.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aes.guannengcc.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ssc.epnwcf.com

Go:   slices.Index(arr, x)
来源：http://hau.birdmap.top

Ruby: arr.index(x)
来源：http://kwp.hongshengwenyu.top

C#:   list.IndexOf(x);
来源：http://jrt.jqgfzy.top

[D13] 过滤（保留满足条件的）
来源：http://xnv.xuetiantiany.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pvt.zdbjq.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://itv.yueranfly.top

JS:   arr.filter(x => x > 3)
来源：http://fcr.xziqi.cn

TS:   arr.filter(x => x > 3)
来源：http://jcx.sufxvd.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uig.yuanzhike.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ndc.yangfankeji.com

Ruby: arr.select { |x| x > 3 }
来源：http://bct.zdqjudy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://vom.yueranfly.top

[D14] 映射转换（每个元素变形）
来源：http://puf.ctjpmb.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yoz.zdbjq.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tlp.jiagoushi.top

JS:   arr.map(x => x * 2)
来源：http://qor.shanyushiyangkeji.top

TS:   arr.map(x => x * 2)
来源：http://wsb.shuidangran.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://anh.zhoulong.xyz

Go:   // 手写循环
来源：http://ces.hywenlv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jsc.jinqigfzy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://uos.bjfxy.top

[D15] 去重
来源：http://cqj.fanxiaobao.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ehd.snrcjt.cn

PHP:  array_unique($arr);
来源：http://wsg.guannengcc.top

JS:   [...new Set(arr)]
来源：http://gnt.haohaochexian.top

TS:   [...new Set(arr)]
来源：http://jcs.nanxinkj.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zot.yangfankeji.com

Go:   // 用 map[T]struct{} 手写
来源：http://fkc.bjfxy.top

Ruby: arr.uniq
来源：http://jsa.svipenyu.cn

C#:   list.Distinct().ToList()
来源：http://gse.hnxiangtu.top

[D16] 求和与平均值
来源：http://xkl.yvedp.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nze.sjlbkw.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kgz.yuxming.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://muu.yfazqb.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mpo.havefunace.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cde.tian-w.cn

Go:   // 手写循环累加
来源：http://bll.andypj.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zcq.hammf.cn

C#:   list.Sum();  list.Average()
来源：http://dwb.hnqzz.top

[D17] 最大值与最小值
来源：http://nur.hfpthk.cn

Py:   max(arr);  min(arr)
来源：http://nqc.jianghu66.top

PHP:  max($arr);  min($arr);
来源：http://xzq.cashguo.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hhb.vqdsnc.cn

TS:   Math.max(...arr);
来源：http://zmi.quarkkingdee.top

Java: Collections.max(list);  Collections.min(list);
来源：http://zmx.bjfxy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ivp.havefunace.top

Ruby: arr.max;  arr.min
来源：http://hee.epnwcf.com

C#:   list.Max();  list.Min()
来源：http://aam.yuanzhike.top

[D18] 扁平化嵌套数组
来源：http://urc.dashuyun.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zyl.wangdashe.top

PHP:  array_merge(...$nested);
来源：http://fhb.yueranfly.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rye.tanke756.top

TS:   nested.flat();
来源：http://ejz.sjlbkw.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zdu.yj20258.top

Go:   // 手写双层循环
来源：http://gbb.ydjk.org.cn

Ruby: nested.flatten
来源：http://bgl.52xcode.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://gtp.zdqjudy.top

[D19] 按字段分组
来源：http://zkx.jianghu66.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vsv.guannengcc.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://isi.jinqigfzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kon.jiagoushi.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://tfg.ywan-chungtsiang.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gjc.nanxuanxn.top

Go:   // 手写 map[string][]T
来源：http://hsd.daria6918.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ceo.tianlin.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qho.316326.xyz

[D20] 统计每个元素出现次数
来源：http://bke.yuanzhike.top

Py:   Counter(arr)
来源：http://htc.ydzc1.top

PHP:  array_count_values($arr);
来源：http://etl.yj202588.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fcd.shuidangran.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tvg.yueranfly.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nyj.shangyingyoupin.top

Go:   // 手写 map[T]int
来源：http://qvq.zhixingplan.top

Ruby: arr.tally
来源：http://obv.xingfuxueyuan.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mxg.gotoacloud.top

[D21] 判断是否包含某元素
来源：http://hrz.quarkkingdee.top

Py:   x in arr
来源：http://ikw.wangdashe.top

PHP:  in_array($x, $arr, true);
来源：http://xrz.zhaomingkeji.xyz

JS:   arr.includes(x)
来源：http://daq.ppjwa.cn

TS:   arr.includes(x)
来源：http://aiv.yj20258888.top

Java: list.contains(x)
来源：http://qpv.9152youxi.cn

Go:   slices.Contains(arr, x)
来源：http://lav.zhiwuduotai.top

Ruby: arr.include?(x)
来源：http://fgo.feifeiyinyue.top

C#:   list.Contains(x)
来源：http://xhb.316326.xyz

[D22] 复制数组（避免共享引用）
来源：http://arp.yangfankeji.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dzk.c1oappe.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://szd.jqgufenzy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bxx.aibaodan.cn

TS:   [...arr];
来源：http://exp.yj202588.top


<!-- 参考信息 -->
代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://epc.ivvv.top

TS:   arr.map(String)
来源：http://jmi.9152youxi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sfb.aizwys.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rot.dashuyun.cn

Ruby: arr.map(&:upcase)
来源：http://qwi.jqgufenzy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://vgp.chenzaomai.com

[C08] 闭包
来源：http://bpq.epnwcf.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wgd.guowangkeji.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hqp.yangfankeji.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://phv.cheryme.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bds.hcnkem.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://trn.aizwys.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://moq.yonumen.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://neo.hnxiangtu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ryq.yangfankeji.com

[C09] 递归
来源：http://gje.9152youxi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mqp.chenlongwang.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bkj.9152youxi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lnc.ybcxt.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wxh.cdnleiting.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pje.jyoumei.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://num.jlsjyb.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cip.shuidangran.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://soo.chenzaomai.com

[C10] 变量作用域
来源：http://zri.fktsv.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://isp.cqqwz.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lyz.hammf.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dkw.bjfxy.top

TS:   同 JS
来源：http://yan.zycfv.cn

Java: 方法内为块级作用域
来源：http://jbz.hammf.cn

Go:   花括号块级作用域
来源：http://hrc.cqqwz.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pvv.jlsjyb.cn

C#:   块级作用域
来源：http://dsq.mhx1999.top

[C11] 模块导入与导出
来源：http://bmx.hcnkem.com

Py:   from module import func
来源：http://zph.tian-w.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xdg.svipenyu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://yaj.kuanghao11.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rlz.xingfuxueyuan.xyz

Java: import java.util.List;
来源：http://wnb.hammf.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://han.ydjk.org.cn

Ruby: require "json"; require_relative "./util"
来源：http://mvh.cucudq.cn

C#:   using System.Text;
来源：http://mlt.hysaishi.cn

[C12] 立即执行函数 IIFE
来源：http://ici.fktsv.cn

Py:   (lambda: print("run"))()
来源：http://ziu.dashuyun.cn

PHP:  (function () { echo "run"; })();
来源：http://daa.yfazqb.com

JS:   (() => { console.log("run"); })();
来源：http://gan.mhx1999.top

TS:   (() => { console.log("run"); })();
来源：http://nkp.birdmap.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xxi.316326.xyz

Go:   func() { fmt.Println("run") }()
来源：http://bxr.bbcook.cn

Ruby: -> { puts "run" }.call
来源：http://qgb.wangdashe.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ueu.52xcode.cn

[C13] 类型声明 / 类型注解
来源：http://osq.yj202588.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kzg.haohaochexian.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gzh.sweek.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gpx.jqgfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xej.hnqzz.top

Java: int add(int a, int b) { return a + b; }
来源：http://lrb.pycfn.com

Go:   func add(a, b int) int
来源：http://auh.jyoumei.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://oqc.hfpthk.cn

C#:   int Add(int a, int b) => a + b;
来源：http://dqw.hfpthk.cn

[C14] 泛型函数
来源：http://pyg.cheryme.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xdu.yfazqb.com

PHP:  // 无泛型
来源：http://wqy.zhongyouzk.top

JS:   // 无泛型
来源：http://jrs.gzhubu.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yhx.bjfxy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xod.shanyushiyangtech.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kgr.hcnkem.com

Ruby: # 无泛型
来源：http://lro.hcnkem.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xxs.sufxvd.cn

[C15] 解构 / 展开参数
来源：http://uqy.chenzaomai.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vcb.yj20258.top

PHP:  [$a, $b] = $pair;
来源：http://wof.ywan-chungtsiang.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rgl.guowangkeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wmb.jinqigufen.top

Java: // 无解构
来源：http://igr.jiagoushi.top

Go:   // 无解构
来源：http://vij.nanxinkj.top

Ruby: a, b = pair
来源：http://jnm.gaohongyu789.top

C#:   var (a, b) = pair;
来源：http://yhy.hnqzz.top

[C16] 函数 / 方法重载
来源：http://rxx.zdqjudy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qub.jqgufenzy.top

PHP:  // 无重载
来源：http://kgk.shanyushiyangtech.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://pwq.sweek.top

TS:   // 用联合类型或重载签名声明
来源：http://ask.sjlbkw.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://bgg.zdqjudy.top

Go:   // 无重载：用不同函数名
来源：http://zhz.gotoacloud.top

Ruby: # 无重载：靠动态参数
来源：http://lll.sysykeji.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://bkx.mhx1999.top

================================================================================
来源：http://ifk.cdnleiting.top

D. 数组 / 列表 / 集合
来源：http://zqm.zhengqikj.top

================================================================================
来源：http://wij.sufxvd.cn

[D01] 创建数组 / 列表
来源：http://dkn.xinyue.icu

Py:   arr = [1, 2, 3];  empty = []
来源：http://mhe.zdqjudy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fkr.yj20258888.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ogi.jyoumei.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xbk.hammf.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://thr.zhongyouzk.top

Go:   arr := []int{1, 2, 3}
来源：http://cio.yanxiufei.cn

Ruby: arr = [1, 2, 3]
来源：http://tjl.tarul.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bgq.zhiwuduotai.top

[D02] 追加元素到末尾
来源：http://cyk.bbcook.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uua.hongshengwenyu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ucu.316326.xyz

JS:   arr.push(4);
来源：http://kiv.hammf.cn

TS:   arr.push(4);
来源：http://lix.hfpthk.cn

Java: list.add(4);
来源：http://dcs.guannengcc.top

Go:   arr = append(arr, 4)
来源：http://qcm.jqgfzy.top

Ruby: arr << 4; arr.push(5)
来源：http://peo.aizwys.cn

C#:   list.Add(4);
来源：http://pdm.epnwcf.com

[D03] 在指定位置插入元素
来源：http://tix.yangfankeji.com

Py:   arr.insert(0, 0)
来源：http://xos.guowangkeji.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://agb.vqdsnc.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wwf.yj20258.top

TS:   arr.splice(0, 0, 0);
来源：http://mjs.zhixingplan.top

Java: list.add(0, 0);
来源：http://rhn.chenlongwang.top

Go:   arr = append([]int{0}, arr...)
来源：http://mmd.yuxming.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pfw.vehdjk.com

C#:   list.Insert(0, 0);
来源：http://swc.ywan-chungtsiang.top

[D04] 删除元素
来源：http://nyw.xuetiantiany.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tla.bbcook.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zpv.nanxuanxn.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mni.yueranfly.top

TS:   arr.splice(0, 1);
来源：http://pax.birdmap.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://clh.meibo888.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mjf.quarkkingdee.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://aio.aizwys.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nnx.jqgfzy.top

[D05] 访问与修改元素
来源：http://cwr.fanxiaobao.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ogs.ivvv.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qzu.feifeiyinyue.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qam.aibaodan.cn

TS:   arr[0]; arr.at(-1);
来源：http://aya.hcnkem.com

Java: list.get(0); list.set(0, 9);
来源：http://pvu.guowangkeji.top

Go:   arr[0]; arr[0] = 9
来源：http://bht.hfpthk.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ahq.nanxuanxn.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cyg.redwolf501.top

[D06] 数组长度
来源：http://wag.yueranfly.top

Py:   len(arr)
来源：http://ekk.zhiwuduotai.top

PHP:  count($arr);
来源：http://gbi.yangfankeji.com

JS:   arr.length
来源：http://cpm.ivvv.top

TS:   arr.length
来源：http://ftm.xuetiantiany.cn

Java: list.size();
来源：http://fmv.yuanzhike.top

Go:   len(arr)
来源：http://nim.pengpengdd.cyou

Ruby: arr.length; arr.size
来源：http://cuv.wangdashe.top

C#:   list.Count;
来源：http://lkh.jiagoushi.top

[D07] 切片 / 取子数组
来源：http://usd.yj20258888.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qsa.andypj.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://cve.sjlbkw.cn

JS:   arr.slice(1, 4);
来源：http://brw.xinyue.icu

TS:   arr.slice(1, 4);
来源：http://tqc.bbcook.cn

Java: list.subList(1, 4);
来源：http://tms.ehwqpu.com

Go:   arr[1:4]
来源：http://yoq.hfpthk.cn

Ruby: arr[1, 3]
来源：http://bjh.zhengqikj.top

C#:   list.GetRange(1, 3);
来源：http://lve.gogol.net.cn

[D08] 合并两个数组
来源：http://tlt.ctjpmb.com

Py:   a + b;  a.extend(b)
来源：http://ycs.zhixingplan.top

PHP:  array_merge($a, $b);
来源：http://eyn.hcnkem.com

JS:   [...a, ...b];  a.concat(b);
来源：http://mni.pengpengdd.cyou

TS:   [...a, ...b];
来源：http://bbt.xuetiantiany.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mqd.sufxvd.cn

Go:   append(a, b...)
来源：http://cvx.ctjpmb.com

Ruby: a + b;  a.concat(b)
来源：http://ttd.zhengqikj.top

C#:   a.Concat(b).ToList()
来源：http://vji.zdqjudy.top

[D09] 排序（升序）
来源：http://pud.guowangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://xbk.bbcook.cn

PHP:  sort($arr);
来源：http://fnx.jiagoushi.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://soq.c1oappe.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://twf.ywan-chungtsiang.top

Java: Collections.sort(list);  list.sort(null);
来源：http://bie.fanxiaobao.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nhh.snrcjt.cn

Ruby: arr.sort
来源：http://vlu.chenzaomai.com

C#:   list.Sort();
来源：http://kwl.shuidangran.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://rpv.redwolf501.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vbx.ctjpmb.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://agh.yuxming.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://moe.xingfuxueyuan.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qtv.quarkkingdee.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tcz.fzhhl.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jfr.jinqigufen.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mtp.9152youxi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nsi.andypj.xyz

[D11] 反转数组
来源：http://luo.shanyushiyangtech.top

Py:   arr[::-1];  arr.reverse()
来源：http://voh.jqgfzy.top

PHP:  array_reverse($arr);
来源：http://gmd.wangdashe.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://moa.shzxlz.cn

TS:   [...arr].reverse();
来源：http://wby.jiagoushi.top

Java: Collections.reverse(list);
来源：http://ahn.zdqjudy.top

Go:   slices.Reverse(arr)
来源：http://qje.xinyue.icu

Ruby: arr.reverse
来源：http://jrc.316326.xyz

C#:   list.Reverse();
来源：http://shb.jyoumei.cn

[D12] 查找元素下标
来源：http://zwm.birdmap.top

Py:   arr.index(x);  x in arr
来源：http://hsf.9152youxi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vzd.wangshuangyany.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nnd.ydzc1.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dfp.shangyingyoupin.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vok.yonumen.top

Go:   slices.Index(arr, x)
来源：http://ytw.dashuyun.cn

Ruby: arr.index(x)
来源：http://gke.hcnkem.com

C#:   list.IndexOf(x);
来源：http://prx.tarul.cn

[D13] 过滤（保留满足条件的）
来源：http://axk.zycfv.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nmg.aizwys.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://har.yj20258.top

JS:   arr.filter(x => x > 3)
来源：http://yvd.52xcode.cn

TS:   arr.filter(x => x > 3)
来源：http://ndr.iojbl.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fnk.zdqjudy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gcm.epnwcf.com

Ruby: arr.select { |x| x > 3 }
来源：http://tet.pengpengdd.cyou

C#:   list.Where(x => x > 3).ToList()
来源：http://yov.xinyue.icu

[D14] 映射转换（每个元素变形）
来源：http://fsm.daxiang520.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cmy.52xcode.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ugr.chenlongwang.top

JS:   arr.map(x => x * 2)
来源：http://yau.epnwcf.com

TS:   arr.map(x => x * 2)
来源：http://bbq.mhx1999.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://yby.shanyushiyangtech.top

Go:   // 手写循环
来源：http://ffw.mhx1999.top

Ruby: arr.map { |x| x * 2 }
来源：http://yor.xylfe.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://vyd.yonumen.top

[D15] 去重
来源：http://jcf.zhaomingkeji.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://clk.hfpthk.cn

PHP:  array_unique($arr);
来源：http://inn.guowangkeji.top

JS:   [...new Set(arr)]
来源：http://yci.fzhhl.top

TS:   [...new Set(arr)]
来源：http://lji.yanxiufei.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pli.nanxuanxn.top

Go:   // 用 map[T]struct{} 手写
来源：http://vdy.xuetiantiany.cn

Ruby: arr.uniq
来源：http://qev.yj20258.top

C#:   list.Distinct().ToList()
来源：http://yna.chenlongwang.top

[D16] 求和与平均值
来源：http://pis.fehbvm.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jnk.hcnkem.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cvu.yuanzhike.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dvp.fanxiaobao.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hob.yj202588.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jds.ywan-chungtsiang.top

Go:   // 手写循环累加
来源：http://hst.tarul.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hyy.nanxuanxn.top

C#:   list.Sum();  list.Average()
来源：http://znu.jinyuanbaomall.cn

[D17] 最大值与最小值
来源：http://fyf.zhijiandao.cn

Py:   max(arr);  min(arr)
来源：http://mjc.jiagoushi.top

PHP:  max($arr);  min($arr);
来源：http://jsq.nanxuanxn.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zzm.xziqi.cn

TS:   Math.max(...arr);
来源：http://ckd.hongshengwenyu.top

Java: Collections.max(list);  Collections.min(list);
来源：http://jzx.yfazqb.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://brf.jinqigfzy.top

Ruby: arr.max;  arr.min
来源：http://egj.zdbjq.cn

C#:   list.Max();  list.Min()
来源：http://xju.xziqi.cn

[D18] 扁平化嵌套数组
来源：http://vcy.chenlongwang.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pcy.meibo888.top

PHP:  array_merge(...$nested);
来源：http://hrj.yj20258.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://afe.jyoumei.cn

TS:   nested.flat();
来源：http://aic.yvedp.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hoe.snrcjt.cn

Go:   // 手写双层循环
来源：http://knz.yj20258.top

Ruby: nested.flatten
来源：http://vyr.dianchejie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://rfk.zhiwuduotai.top

[D19] 按字段分组
来源：http://zgk.haohaochexian.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rne.pycfn.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://apf.bbcook.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zld.hcnkem.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://ptj.aibaodan.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zad.fanxiaobao.xyz

Go:   // 手写 map[string][]T
来源：http://nkg.nanxinkj.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://krm.daria6918.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rbd.yanxiufei.cn

[D20] 统计每个元素出现次数
来源：http://wkp.shangyingyoupin.top

Py:   Counter(arr)
来源：http://dgq.yfazqb.com

PHP:  array_count_values($arr);
来源：http://dux.fzhhl.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://muk.zhengqikj.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nuw.52xcode.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dgp.yj202588.top

Go:   // 手写 map[T]int
来源：http://jhc.chenlongwang.top

Ruby: arr.tally
来源：http://olk.jyoumei.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qlc.hesvh.cn

[D21] 判断是否包含某元素
来源：http://dhp.guannengcc.top

Py:   x in arr
来源：http://ntn.nwbrower.top

PHP:  in_array($x, $arr, true);
来源：http://jku.52xcode.cn

JS:   arr.includes(x)
来源：http://xha.yvedp.cn

TS:   arr.includes(x)
来源：http://xfw.mhx1999.top

Java: list.contains(x)
来源：http://duo.tianlin.xyz

Go:   slices.Contains(arr, x)
来源：http://jor.xingfuxueyuan.xyz

Ruby: arr.include?(x)
来源：http://uat.shanyushiyangtech.top

C#:   list.Contains(x)
来源：http://gtr.yuanzhike.top

[D22] 复制数组（避免共享引用）
来源：http://cku.jinqigfzy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vku.sufxvd.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pzf.jinqigufen.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hat.cheryme.top

TS:   [...arr];
来源：http://ayj.yueranfly.top

Java: new ArrayList<>(list);
来源：http://dlq.chenlongwang.top

Go:   copied := append([]int(nil), arr...)
来源：http://aft.andypj.xyz

Ruby: arr.dup;  arr.clone
来源：http://iuz.zhongyouzk.top

C#:   new List<int>(list);
来源：http://lpj.hnqzz.top

[D23] reduce 累积计算
来源：http://qsy.zhixingplan.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yoi.zdqjudy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pfo.jqgufenzy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://aid.yangfankeji.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vpg.fanxiaobao.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://cdd.nanxuanxn.top

Go:   // 手写循环
来源：http://cpe.jiagoushi.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kyu.nanxinkj.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dwn.xinyue.icu

[D24] 字典 / Map 基本操作
来源：http://qjm.cqqwz.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uij.quarkkingdee.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bqy.zhaomingkeji.xyz


<!-- 参考信息 -->
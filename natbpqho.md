代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://hwv.jinyuanbaomall.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://pst.jinqigufen.top

[C08] 闭包
来源：http://nht.haohaochexian.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tgh.chenlongwang.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://oin.hnxiangtu.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://frh.52xcode.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rgp.yuxming.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://egn.yongpay.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://spg.zhiwuduotai.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qqh.hnqzz.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dqh.ydjk.org.cn

[C09] 递归
来源：http://ijo.yj20258.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jlx.andypj.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uft.cashguo.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mum.cqqwz.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bsn.snrcjt.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pdy.ppjwa.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gzx.hnxiangtu.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kdx.yongpay.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hxt.guowangkeji.top

[C10] 变量作用域
来源：http://pkx.zdqjudy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ydf.meibo888.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rks.hammf.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dhi.nanxinkj.top

TS:   同 JS
来源：http://jhv.tarul.cn

Java: 方法内为块级作用域
来源：http://ano.snrcjt.cn

Go:   花括号块级作用域
来源：http://qql.jqgufenzy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mjb.aibaodan.cn

C#:   块级作用域
来源：http://hgi.gzhubu.top

[C11] 模块导入与导出
来源：http://cfe.jqgfzy.top

Py:   from module import func
来源：http://olg.chenjidiqi.icu

PHP:  require "file.php";  或 use App\Service;
来源：http://tuv.redwolf501.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://sqa.jlsjyb.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qkw.jinyuanbaomall.cn

Java: import java.util.List;
来源：http://fgc.jinqigfzy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gtw.wangdashe.top

Ruby: require "json"; require_relative "./util"
来源：http://xft.jlsjyb.cn

C#:   using System.Text;
来源：http://gan.daxiang520.top

[C12] 立即执行函数 IIFE
来源：http://shy.gogol.net.cn

Py:   (lambda: print("run"))()
来源：http://nsi.jqgufenzy.top

PHP:  (function () { echo "run"; })();
来源：http://ftq.vehdjk.com

JS:   (() => { console.log("run"); })();
来源：http://phf.yj202588.top

TS:   (() => { console.log("run"); })();
来源：http://oex.dianchejie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sxp.guowangkeji.top

Go:   func() { fmt.Println("run") }()
来源：http://gap.sweek.top

Ruby: -> { puts "run" }.call
来源：http://ljc.hongshengwenyu.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ssy.daria6918.cn

[C13] 类型声明 / 类型注解
来源：http://unx.nanxinkj.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://clu.zhongyouzk.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://frw.bbcook.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pbq.snrcjt.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://laj.xingfuxueyuan.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://tje.tarul.cn

Go:   func add(a, b int) int
来源：http://uac.bbcook.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pnm.daria6918.cn

C#:   int Add(int a, int b) => a + b;
来源：http://eis.shanyushiyangkeji.top

[C14] 泛型函数
来源：http://gvx.0kj1m.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ghr.daria6918.cn

PHP:  // 无泛型
来源：http://hrk.zycfv.cn

JS:   // 无泛型
来源：http://fjp.hnxiangtu.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ejx.fktsv.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vdr.c1oappe.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lhh.quarkkingdee.top

Ruby: # 无泛型
来源：http://nnk.zhiwuduotai.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ngh.vqdsnc.cn

[C15] 解构 / 展开参数
来源：http://hrs.yueranfly.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cws.yangfankeji.com

PHP:  [$a, $b] = $pair;
来源：http://hol.ywan-chungtsiang.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ybf.shanyushiyangkeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cxj.zhijiandao.cn

Java: // 无解构
来源：http://duo.ydzc1.top

Go:   // 无解构
来源：http://ceo.shuidangran.top

Ruby: a, b = pair
来源：http://eoo.birdmap.top

C#:   var (a, b) = pair;
来源：http://ezd.xuetiantiany.cn

[C16] 函数 / 方法重载
来源：http://ctb.hysaishi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://umk.yongpay.top

PHP:  // 无重载
来源：http://dnh.snrcjt.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://azh.xylfe.cn

TS:   // 用联合类型或重载签名声明
来源：http://khh.gaohongyu789.top

Java: void f(int a) {}  void f(String a) {}
来源：http://dcr.pengpengdd.cyou

Go:   // 无重载：用不同函数名
来源：http://eeb.hywenlv.cn

Ruby: # 无重载：靠动态参数
来源：http://udg.mhx1999.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://yox.ivvv.top

================================================================================
来源：http://iae.xziqi.cn

D. 数组 / 列表 / 集合
来源：http://nps.shangyingyoupin.top

================================================================================
来源：http://xvs.zhongyouzk.top

[D01] 创建数组 / 列表
来源：http://kns.epnwcf.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://zch.uphjek.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nxr.redwolf501.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ljg.gogol.net.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hmu.zhoulong.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mvm.jiagoushi.top

Go:   arr := []int{1, 2, 3}
来源：http://sou.sysykeji.top

Ruby: arr = [1, 2, 3]
来源：http://fwi.hysaishi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nxe.hammf.cn

[D02] 追加元素到末尾
来源：http://xhj.0kj1m.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ppt.mhx1999.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://iqy.uphjek.com

JS:   arr.push(4);
来源：http://ind.ydjk.org.cn

TS:   arr.push(4);
来源：http://vav.vehdjk.com

Java: list.add(4);
来源：http://kwe.cucudq.cn

Go:   arr = append(arr, 4)
来源：http://sou.sysykeji.top

Ruby: arr << 4; arr.push(5)
来源：http://bpq.jinqigufen.top

C#:   list.Add(4);
来源：http://law.chenlongwang.top

[D03] 在指定位置插入元素
来源：http://ezb.yongpay.top

Py:   arr.insert(0, 0)
来源：http://var.fanxiaobao.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://whp.sjlbkw.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lzc.mhx1999.top

TS:   arr.splice(0, 0, 0);
来源：http://lbi.fehbvm.com

Java: list.add(0, 0);
来源：http://jys.tarul.cn

Go:   arr = append([]int{0}, arr...)
来源：http://han.feifeiyinyue.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://axq.ydjk.org.cn

C#:   list.Insert(0, 0);
来源：http://wos.jinqigufen.top

[D04] 删除元素
来源：http://aje.haohaochexian.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ctg.ppjwa.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://azq.svipenyu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kug.xuetiantiany.cn

TS:   arr.splice(0, 1);
来源：http://ova.c1oappe.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://atv.ywan-chungtsiang.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jil.meibo888.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hnd.sjlbkw.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lwg.jlsjyb.cn

[D05] 访问与修改元素
来源：http://uoq.hongshengwenyu.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tpl.tanke756.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nma.hnqzz.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://udt.jqgfzy.top

TS:   arr[0]; arr.at(-1);
来源：http://quu.cdnleiting.top

Java: list.get(0); list.set(0, 9);
来源：http://rbo.nanxuanxn.top

Go:   arr[0]; arr[0] = 9
来源：http://clo.ywan-chungtsiang.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ugc.ywan-chungtsiang.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://oud.nwbrower.top

[D06] 数组长度
来源：http://sjd.zhiwuduotai.top

Py:   len(arr)
来源：http://qus.shanyushiyangkeji.top

PHP:  count($arr);
来源：http://vey.tianlin.xyz

JS:   arr.length
来源：http://irp.tarul.cn

TS:   arr.length
来源：http://qsj.jinyuanbaomall.cn

Java: list.size();
来源：http://epo.9152youxi.cn

Go:   len(arr)
来源：http://yri.yongpay.top

Ruby: arr.length; arr.size
来源：http://foo.jinghuilouyu.cn

C#:   list.Count;
来源：http://ecp.jiagoushi.top

[D07] 切片 / 取子数组
来源：http://cmj.birdmap.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sxz.jinqigufen.top

PHP:  array_slice($arr, 1, 3);
来源：http://zhq.sysykeji.top

JS:   arr.slice(1, 4);
来源：http://rfd.redwolf501.top

TS:   arr.slice(1, 4);
来源：http://hfb.xuetiantiany.cn

Java: list.subList(1, 4);
来源：http://hfo.jyoumei.cn

Go:   arr[1:4]
来源：http://cnb.ydzc1.top

Ruby: arr[1, 3]
来源：http://lyr.ppjwa.cn

C#:   list.GetRange(1, 3);
来源：http://xwa.zhongyouzk.top

[D08] 合并两个数组
来源：http://xpl.yueranfly.top

Py:   a + b;  a.extend(b)
来源：http://bti.yuanzhike.top

PHP:  array_merge($a, $b);
来源：http://egk.cdnleiting.top

JS:   [...a, ...b];  a.concat(b);
来源：http://tdj.tarul.cn

TS:   [...a, ...b];
来源：http://ztv.svipenyu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vji.fzhhl.top

Go:   append(a, b...)
来源：http://sgi.ywan-chungtsiang.top

Ruby: a + b;  a.concat(b)
来源：http://wma.andypj.xyz

C#:   a.Concat(b).ToList()
来源：http://hcl.bjfxy.top

[D09] 排序（升序）
来源：http://mfi.hywenlv.cn

Py:   sorted(arr);  arr.sort()
来源：http://bhb.guannengcc.top

PHP:  sort($arr);
来源：http://syc.ywan-chungtsiang.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fnz.yj202588.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ztu.ydjk.org.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://pwn.xylfe.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vhs.jlsjyb.cn

Ruby: arr.sort
来源：http://qmw.jyoumei.cn

C#:   list.Sort();
来源：http://ycv.xuanzx.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://bwh.yj20258888.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://niy.shanyushiyangtech.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ofz.nanxinkj.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ghg.chenlongwang.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hzl.hammf.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cwh.tianlin.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hpw.bbcook.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lgm.hongshengwenyu.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://liy.aizwys.cn

[D11] 反转数组
来源：http://ihd.jqgfzy.top

Py:   arr[::-1];  arr.reverse()
来源：http://xfn.guowangkeji.top

PHP:  array_reverse($arr);
来源：http://qyj.ydjk.org.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://izf.shzxlz.cn

TS:   [...arr].reverse();
来源：http://mwg.xingfuxueyuan.xyz

Java: Collections.reverse(list);
来源：http://ohn.zhiwuduotai.top

Go:   slices.Reverse(arr)
来源：http://ftp.yj202588.top

Ruby: arr.reverse
来源：http://nog.316326.xyz

C#:   list.Reverse();
来源：http://lcc.shangyingyoupin.top

[D12] 查找元素下标
来源：http://ckp.9152youxi.cn

Py:   arr.index(x);  x in arr
来源：http://rya.gaohongyu789.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sct.xinyue.icu

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qhm.uphjek.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eoj.xuanzx.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://duj.jqgufenzy.top

Go:   slices.Index(arr, x)
来源：http://zvq.andypj.xyz

Ruby: arr.index(x)
来源：http://ohq.nwbrower.top

C#:   list.IndexOf(x);
来源：http://bsw.cucudq.cn

[D13] 过滤（保留满足条件的）
来源：http://rlq.sysykeji.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qga.zhongyouzk.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xuh.fengsongda.top

JS:   arr.filter(x => x > 3)
来源：http://yjf.xinyue.icu

TS:   arr.filter(x => x > 3)
来源：http://vlp.gzhubu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rzo.yfazqb.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fkv.ydjk.org.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ikm.jinghuilouyu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://nrh.jinyuanbaomall.cn

[D14] 映射转换（每个元素变形）
来源：http://pcw.yanxiufei.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://crh.tarul.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://eln.jinqigufen.top

JS:   arr.map(x => x * 2)
来源：http://jbv.snrcjt.cn

TS:   arr.map(x => x * 2)
来源：http://mpf.zhoulong.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://yho.shuidangran.top

Go:   // 手写循环
来源：http://pqg.svipenyu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dcg.hysaishi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rde.pycfn.com

[D15] 去重
来源：http://ptt.jlsjyb.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://oru.fanxiaobao.xyz

PHP:  array_unique($arr);
来源：http://tna.redwolf501.top

JS:   [...new Set(arr)]
来源：http://nsz.svipenyu.cn

TS:   [...new Set(arr)]
来源：http://wae.ybcxt.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://snz.hysaishi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wnp.andypj.xyz

Ruby: arr.uniq
来源：http://cwx.jlsjyb.cn

C#:   list.Distinct().ToList()
来源：http://fau.zdqjudy.top

[D16] 求和与平均值
来源：http://aqv.ydjk.org.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bch.hcnkem.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hby.andypj.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qax.gzhubu.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ahl.shanyushiyangkeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xaa.kuanghao11.cn

Go:   // 手写循环累加
来源：http://pyg.fanxiaobao.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gxz.fzhhl.top

C#:   list.Sum();  list.Average()
来源：http://vew.fanxiaobao.xyz

[D17] 最大值与最小值
来源：http://ivu.xingfuxueyuan.xyz

Py:   max(arr);  min(arr)
来源：http://avc.hcnkem.com

PHP:  max($arr);  min($arr);
来源：http://uju.shanyushiyangkeji.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://btx.ehwqpu.com

TS:   Math.max(...arr);
来源：http://oqw.jqgfzy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://cdk.hnxiangtu.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cmv.zhaomingkeji.xyz

Ruby: arr.max;  arr.min
来源：http://hop.jyoumei.cn

C#:   list.Max();  list.Min()
来源：http://txv.ivvv.top

[D18] 扁平化嵌套数组
来源：http://tdm.ybcxt.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://omu.9152youxi.cn

PHP:  array_merge(...$nested);
来源：http://xyi.zdbjq.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://oyf.fktsv.cn

TS:   nested.flat();
来源：http://sft.havefunace.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yet.svipenyu.cn

Go:   // 手写双层循环
来源：http://qnt.wangdashe.top

Ruby: nested.flatten
来源：http://bsf.nanxinkj.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://rdd.316326.xyz

[D19] 按字段分组
来源：http://tcl.fengsongda.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ike.haohaochexian.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fqj.yuanzhike.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xst.fengsongda.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://hjd.yfazqb.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pwo.shanyushiyangkeji.top

Go:   // 手写 map[string][]T
来源：http://zqq.xinyue.icu

Ruby: arr.group_by { |x| x[:type] }
来源：http://aer.redwolf501.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cmj.aibaodan.cn

[D20] 统计每个元素出现次数
来源：http://bzo.zycfv.cn

Py:   Counter(arr)
来源：http://thf.tian-w.cn

PHP:  array_count_values($arr);
来源：http://pab.yueranfly.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rhi.cashguo.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qja.bjfxy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cme.hysaishi.cn

Go:   // 手写 map[T]int
来源：http://biw.zhengqikj.top

Ruby: arr.tally
来源：http://pgs.0kj1m.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://doz.cheryme.top

[D21] 判断是否包含某元素
来源：http://cck.zhijiandao.cn

Py:   x in arr
来源：http://rub.zhoulong.xyz

PHP:  in_array($x, $arr, true);
来源：http://fid.chenjidiqi.icu

JS:   arr.includes(x)
来源：http://hfk.gogol.net.cn

TS:   arr.includes(x)
来源：http://tnn.svipenyu.cn

Java: list.contains(x)
来源：http://zoh.yfazqb.com

Go:   slices.Contains(arr, x)
来源：http://foq.sweek.top

Ruby: arr.include?(x)
来源：http://zou.ywan-chungtsiang.top

C#:   list.Contains(x)
来源：http://abx.daxiang520.top

[D22] 复制数组（避免共享引用）
来源：http://gth.gzhubu.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xnc.ppjwa.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://njp.ehwqpu.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mtp.fengsongda.top

TS:   [...arr];
来源：http://xsq.hammf.cn

Java: new ArrayList<>(list);
来源：http://gud.uphjek.com

Go:   copied := append([]int(nil), arr...)
来源：http://dzx.ppjwa.cn

Ruby: arr.dup;  arr.clone
来源：http://ayb.jqgfzy.top

C#:   new List<int>(list);
来源：http://tfh.shzxlz.cn

[D23] reduce 累积计算
来源：http://rtw.jinyuanbaomall.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ehz.hywenlv.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tpg.cucudq.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jqe.jianghu66.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cfr.sufxvd.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://drs.sweek.top

Go:   // 手写循环
来源：http://orn.hnxiangtu.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uoy.cqqwz.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tok.shuidangran.top

[D24] 字典 / Map 基本操作
来源：http://bud.ywan-chungtsiang.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://usf.zhoulong.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jpt.birdmap.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pry.hcnkem.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jco.hammf.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gyz.andypj.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://aoc.hnqzz.top


<!-- 参考信息 -->
代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fqn.52xcode.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nwr.svipenyu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cpv.ybcxt.top

[C09] 递归
来源：http://kja.nanxinkj.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mej.zhongyouzk.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hfb.gogol.net.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zjx.sweek.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oea.jqgufenzy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kxd.yuxming.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qtv.vqdsnc.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pne.ybcxt.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://eep.hysaishi.cn

[C10] 变量作用域
来源：http://wus.hnxiangtu.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://log.wangdashe.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jen.jlsjyb.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nbg.hfpthk.cn

TS:   同 JS
来源：http://fnk.smart0.xyz

Java: 方法内为块级作用域
来源：http://ivh.yj202588.top

Go:   花括号块级作用域
来源：http://hkl.chenzaomai.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gps.chenlongwang.top

C#:   块级作用域
来源：http://aea.yonumen.top

[C11] 模块导入与导出
来源：http://jyn.hnqzz.top

Py:   from module import func
来源：http://lkg.guannengcc.top

PHP:  require "file.php";  或 use App\Service;
来源：http://gcr.shanyushiyangtech.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://sfr.9152youxi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lzl.yuanzhike.top

Java: import java.util.List;
来源：http://uyo.shangyingyoupin.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qlt.fzhhl.top

Ruby: require "json"; require_relative "./util"
来源：http://oaj.zhaomingkeji.xyz

C#:   using System.Text;
来源：http://mwo.gaohongyu789.top

[C12] 立即执行函数 IIFE
来源：http://phr.gogol.net.cn

Py:   (lambda: print("run"))()
来源：http://ogj.ydzc1.top

PHP:  (function () { echo "run"; })();
来源：http://kwj.andypj.xyz

JS:   (() => { console.log("run"); })();
来源：http://mkl.gzhubu.top

TS:   (() => { console.log("run"); })();
来源：http://bnr.havefunace.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sdh.xinyue.icu

Go:   func() { fmt.Println("run") }()
来源：http://beu.vehdjk.com

Ruby: -> { puts "run" }.call
来源：http://rox.tian-w.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ewp.cheryme.top

[C13] 类型声明 / 类型注解
来源：http://doc.fengsongda.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://boq.sufxvd.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://okq.fzhhl.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://czt.yongpay.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wya.hongshengwenyu.top

Java: int add(int a, int b) { return a + b; }
来源：http://dvv.vqdsnc.cn

Go:   func add(a, b int) int
来源：http://xgs.nwbrower.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gpo.feifeiyinyue.top

C#:   int Add(int a, int b) => a + b;
来源：http://qdb.birdmap.top

[C14] 泛型函数
来源：http://rej.yongpay.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kaa.xuanzx.com

PHP:  // 无泛型
来源：http://ctw.shanyushiyangtech.top

JS:   // 无泛型
来源：http://dav.zhengqikj.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zjo.zdbjq.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hws.yueranfly.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://txp.jinqigfzy.top

Ruby: # 无泛型
来源：http://zsm.zhongyouzk.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lib.yj202588.top

[C15] 解构 / 展开参数
来源：http://jnd.0kj1m.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://svq.snrcjt.cn

PHP:  [$a, $b] = $pair;
来源：http://vzs.birdmap.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://czy.gaohongyu789.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pjv.ydjk.org.cn

Java: // 无解构
来源：http://wdj.hongshengwenyu.top

Go:   // 无解构
来源：http://idy.pengpengdd.cyou

Ruby: a, b = pair
来源：http://awu.yongpay.top

C#:   var (a, b) = pair;
来源：http://vpa.yangfankeji.com

[C16] 函数 / 方法重载
来源：http://akq.aibaodan.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hdc.vqdsnc.cn

PHP:  // 无重载
来源：http://etw.zhixingplan.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ofq.hnxiangtu.top

TS:   // 用联合类型或重载签名声明
来源：http://jro.daxiang520.top

Java: void f(int a) {}  void f(String a) {}
来源：http://rta.chenlongwang.top

Go:   // 无重载：用不同函数名
来源：http://yki.kuanghao11.cn

Ruby: # 无重载：靠动态参数
来源：http://wdp.pycfn.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://fox.cheryme.top

================================================================================
来源：http://hio.zhaomingkeji.xyz

D. 数组 / 列表 / 集合
来源：http://nkd.yongpay.top

================================================================================
来源：http://yco.jiagoushi.top

[D01] 创建数组 / 列表
来源：http://nnb.ppjwa.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://sup.svipenyu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hhn.jlsjyb.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bur.tianlin.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://rch.ppjwa.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lfb.feifeiyinyue.top

Go:   arr := []int{1, 2, 3}
来源：http://vzk.jianghu66.top

Ruby: arr = [1, 2, 3]
来源：http://een.yangfankeji.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kpw.svipenyu.cn

[D02] 追加元素到末尾
来源：http://tei.ydjk.org.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ozw.fzhhl.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bdb.cqqwz.cn

JS:   arr.push(4);
来源：http://vaf.fengsongda.top

TS:   arr.push(4);
来源：http://xpl.uphjek.com

Java: list.add(4);
来源：http://hjf.yongpay.top

Go:   arr = append(arr, 4)
来源：http://nic.nanxinkj.top

Ruby: arr << 4; arr.push(5)
来源：http://pcf.pycfn.com

C#:   list.Add(4);
来源：http://vhg.iojbl.cn

[D03] 在指定位置插入元素
来源：http://stj.tian-w.cn

Py:   arr.insert(0, 0)
来源：http://mvl.jlsjyb.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bjl.hesvh.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xld.chenjidiqi.icu

TS:   arr.splice(0, 0, 0);
来源：http://gze.gaohongyu789.top

Java: list.add(0, 0);
来源：http://mvy.yvedp.cn

Go:   arr = append([]int{0}, arr...)
来源：http://wdq.zhongyouzk.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lfd.shanyushiyangtech.top

C#:   list.Insert(0, 0);
来源：http://yet.jinyuanbaomall.cn

[D04] 删除元素
来源：http://rcl.hongshengwenyu.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pei.jqgfzy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wqo.yuxming.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yig.sxryk.cn

TS:   arr.splice(0, 1);
来源：http://mdo.zhoulong.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xgp.nwbrower.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wid.zhoulong.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qey.snrcjt.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://brm.ywan-chungtsiang.top

[D05] 访问与修改元素
来源：http://xfc.chenlongwang.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ans.hongshengwenyu.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mkr.jinqigfzy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jrm.yfazqb.com

TS:   arr[0]; arr.at(-1);
来源：http://pjk.sysykeji.top

Java: list.get(0); list.set(0, 9);
来源：http://akz.yuxming.cn

Go:   arr[0]; arr[0] = 9
来源：http://mxn.zhaomingkeji.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qff.gaohongyu789.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jja.zhengqikj.top

[D06] 数组长度
来源：http://kdv.cqqwz.cn

Py:   len(arr)
来源：http://bfz.gaohongyu789.top

PHP:  count($arr);
来源：http://ywz.0kj1m.cn

JS:   arr.length
来源：http://qpy.fktsv.cn

TS:   arr.length
来源：http://ldi.epnwcf.com

Java: list.size();
来源：http://szw.shuidangran.top

Go:   len(arr)
来源：http://rjc.fzhhl.top

Ruby: arr.length; arr.size
来源：http://bne.hnxiangtu.top

C#:   list.Count;
来源：http://tfw.epnwcf.com

[D07] 切片 / 取子数组
来源：http://mpz.wangdashe.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fas.jqgufenzy.top

PHP:  array_slice($arr, 1, 3);
来源：http://suc.fehbvm.com

JS:   arr.slice(1, 4);
来源：http://vkj.chenjidiqi.icu

TS:   arr.slice(1, 4);
来源：http://jvu.tianlin.xyz

Java: list.subList(1, 4);
来源：http://cnf.cucudq.cn

Go:   arr[1:4]
来源：http://wlq.ctjpmb.com

Ruby: arr[1, 3]
来源：http://rni.xingfuxueyuan.xyz

C#:   list.GetRange(1, 3);
来源：http://vsk.bjfxy.top

[D08] 合并两个数组
来源：http://aew.yj20258.top

Py:   a + b;  a.extend(b)
来源：http://ore.haohaochexian.top

PHP:  array_merge($a, $b);
来源：http://vlq.jinghuilouyu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hdp.zycfv.cn

TS:   [...a, ...b];
来源：http://hdr.chenlongwang.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tgy.sufxvd.cn

Go:   append(a, b...)
来源：http://ayv.fehbvm.com

Ruby: a + b;  a.concat(b)
来源：http://let.yongpay.top

C#:   a.Concat(b).ToList()
来源：http://srh.meibo888.top

[D09] 排序（升序）
来源：http://wea.sjlbkw.cn

Py:   sorted(arr);  arr.sort()
来源：http://wec.jqgfzy.top

PHP:  sort($arr);
来源：http://ghr.pengpengdd.cyou

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ppc.xziqi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fjv.pycfn.com

Java: Collections.sort(list);  list.sort(null);
来源：http://ipn.bjfxy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uir.cdnleiting.top

Ruby: arr.sort
来源：http://mje.fengsongda.top

C#:   list.Sort();
来源：http://aki.316326.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://mol.9152youxi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cte.jiagoushi.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ntl.yuanzhike.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nfk.birdmap.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tfx.chenzaomai.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jil.jyoumei.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tdm.jinyuanbaomall.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://isc.haohaochexian.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lkr.fktsv.cn

[D11] 反转数组
来源：http://tkj.vehdjk.com

Py:   arr[::-1];  arr.reverse()
来源：http://jpu.yongpay.top

PHP:  array_reverse($arr);
来源：http://tvd.jinghuilouyu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zxw.fanxiaobao.xyz

TS:   [...arr].reverse();
来源：http://kte.xuanzx.com

Java: Collections.reverse(list);
来源：http://cjr.ehwqpu.com

Go:   slices.Reverse(arr)
来源：http://ugl.daria6918.cn

Ruby: arr.reverse
来源：http://wnq.redwolf501.top

C#:   list.Reverse();
来源：http://azs.gaohongyu789.top

[D12] 查找元素下标
来源：http://rcp.zhoulong.xyz

Py:   arr.index(x);  x in arr
来源：http://mjw.vqdsnc.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fxf.fzhhl.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://joo.snrcjt.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cao.zycfv.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tnw.zhoulong.xyz

Go:   slices.Index(arr, x)
来源：http://gkg.vehdjk.com

Ruby: arr.index(x)
来源：http://mus.hywenlv.cn

C#:   list.IndexOf(x);
来源：http://aks.tarul.cn

[D13] 过滤（保留满足条件的）
来源：http://vqq.ppjwa.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://waf.epnwcf.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xep.yueranfly.top

JS:   arr.filter(x => x > 3)
来源：http://hlv.xylfe.cn

TS:   arr.filter(x => x > 3)
来源：http://vkl.mhx1999.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qdq.ctjpmb.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dar.fengsongda.top

Ruby: arr.select { |x| x > 3 }
来源：http://eoe.c1oappe.top

C#:   list.Where(x => x > 3).ToList()
来源：http://qpb.aizwys.cn

[D14] 映射转换（每个元素变形）
来源：http://dyy.jyoumei.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gmr.meibo888.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dik.hnxiangtu.top

JS:   arr.map(x => x * 2)
来源：http://hie.chenjidiqi.icu

TS:   arr.map(x => x * 2)
来源：http://uhw.shanyushiyangtech.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://uay.yueranfly.top

Go:   // 手写循环
来源：http://wbx.wangdashe.top

Ruby: arr.map { |x| x * 2 }
来源：http://xzt.fktsv.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://mfw.gogol.net.cn

[D15] 去重
来源：http://yol.dashuyun.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wyd.zdqjudy.top

PHP:  array_unique($arr);
来源：http://imh.snrcjt.cn

JS:   [...new Set(arr)]
来源：http://vup.vehdjk.com

TS:   [...new Set(arr)]
来源：http://clh.hfpthk.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://heg.yuanzhike.top

Go:   // 用 map[T]struct{} 手写
来源：http://gpi.chenzaomai.com

Ruby: arr.uniq
来源：http://owv.hesvh.cn

C#:   list.Distinct().ToList()
来源：http://phd.fanxiaobao.xyz

[D16] 求和与平均值
来源：http://bse.nwbrower.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ebw.gogol.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zzs.haohaochexian.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://uvh.pycfn.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wym.sysykeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zau.zhengqikj.top

Go:   // 手写循环累加
来源：http://ibz.sweek.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://aua.yongpay.top

C#:   list.Sum();  list.Average()
来源：http://fbw.cdnleiting.top

[D17] 最大值与最小值
来源：http://swj.chenzaomai.com

Py:   max(arr);  min(arr)
来源：http://zqj.ehwqpu.com

PHP:  max($arr);  min($arr);
来源：http://gsu.yanxiufei.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xll.hongshengwenyu.top

TS:   Math.max(...arr);
来源：http://rqn.hcnkem.com

Java: Collections.max(list);  Collections.min(list);
来源：http://hhi.c1oappe.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ybv.chenlongwang.top

Ruby: arr.max;  arr.min
来源：http://eek.jinqigufen.top

C#:   list.Max();  list.Min()
来源：http://hdn.jlsjyb.cn

[D18] 扁平化嵌套数组
来源：http://mkr.xziqi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://djo.hnxiangtu.top

PHP:  array_merge(...$nested);
来源：http://mdj.xingfuxueyuan.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xso.jqgufenzy.top

TS:   nested.flat();
来源：http://rjd.shanyushiyangtech.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pfe.sufxvd.cn

Go:   // 手写双层循环
来源：http://wzu.ctjpmb.com

Ruby: nested.flatten
来源：http://jtz.zdqjudy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://pio.iojbl.cn

[D19] 按字段分组
来源：http://obu.zhaomingkeji.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fxt.zdbjq.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gxo.jiagoushi.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vtv.gaohongyu789.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://aje.zhongyouzk.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://omt.yonumen.top

Go:   // 手写 map[string][]T
来源：http://wic.hesvh.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://znr.tianlin.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wpd.ivvv.top

[D20] 统计每个元素出现次数
来源：http://pcv.xuetiantiany.cn

Py:   Counter(arr)
来源：http://hvv.xinyue.icu

PHP:  array_count_values($arr);
来源：http://tkx.ivvv.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rcn.pengpengdd.cyou

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oax.jinqigfzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rda.shanyushiyangtech.top

Go:   // 手写 map[T]int
来源：http://qic.yj20258.top

Ruby: arr.tally
来源：http://vya.guannengcc.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qbp.yfazqb.com

[D21] 判断是否包含某元素
来源：http://cus.jinyuanbaomall.cn

Py:   x in arr
来源：http://poh.ppjwa.cn

PHP:  in_array($x, $arr, true);
来源：http://iwy.jianghu66.top

JS:   arr.includes(x)
来源：http://vjn.ybcxt.top

TS:   arr.includes(x)
来源：http://dmh.tanke756.top

Java: list.contains(x)
来源：http://zvf.fengsongda.top

Go:   slices.Contains(arr, x)
来源：http://yqa.316326.xyz

Ruby: arr.include?(x)
来源：http://xsp.aizwys.cn

C#:   list.Contains(x)
来源：http://sxh.uphjek.com

[D22] 复制数组（避免共享引用）
来源：http://lop.zhengqikj.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jqq.zhengqikj.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ofe.wangdashe.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://muw.epnwcf.com

TS:   [...arr];
来源：http://gug.xuetiantiany.cn

Java: new ArrayList<>(list);
来源：http://qso.xylfe.cn

Go:   copied := append([]int(nil), arr...)
来源：http://fpm.zhongyouzk.top

Ruby: arr.dup;  arr.clone
来源：http://bnx.jiagoushi.top

C#:   new List<int>(list);
来源：http://scl.aizwys.cn

[D23] reduce 累积计算
来源：http://wim.jqgufenzy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mky.fzhhl.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://iuc.cucudq.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lrc.aizwys.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xlr.zhiwuduotai.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://gvu.cqqwz.cn

Go:   // 手写循环
来源：http://vsz.hammf.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tby.daxiang520.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qcv.wangshuangyany.cn

[D24] 字典 / Map 基本操作
来源：http://goo.hnqzz.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tpk.pycfn.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pwi.ppjwa.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mku.kuanghao11.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nkv.cdnleiting.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cll.chenzaomai.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gxf.9152youxi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kcx.fengsongda.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tat.yfazqb.com

[D25] Set 集合去重与交并差
来源：http://xuv.daria6918.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jus.fzhhl.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fnq.shanyushiyangtech.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jxc.ywan-chungtsiang.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hbc.daria6918.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jqt.nanxinkj.top


<!-- 参考信息 -->
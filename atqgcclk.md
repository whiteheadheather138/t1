代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kvm.shuidangran.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://daw.yj202588.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vab.yfazqb.com

[C09] 递归
来源：http://pui.pengpengdd.cyou

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fqc.hfpthk.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jah.ivvv.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hry.feifeiyinyue.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ugr.yj20258.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gvl.wangdashe.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://yvc.cucudq.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://aur.fehbvm.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://els.sxryk.cn

[C10] 变量作用域
来源：http://oxu.jlsjyb.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xku.shanyushiyangtech.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tcl.jyoumei.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fhw.tarul.cn

TS:   同 JS
来源：http://day.316326.xyz

Java: 方法内为块级作用域
来源：http://ysq.redwolf501.top

Go:   花括号块级作用域
来源：http://uaj.sxryk.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ggf.shangyingyoupin.top

C#:   块级作用域
来源：http://xst.pengpengdd.cyou

[C11] 模块导入与导出
来源：http://bin.chenlongwang.top

Py:   from module import func
来源：http://axm.yuanzhike.top

PHP:  require "file.php";  或 use App\Service;
来源：http://any.shanyushiyangtech.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://nrw.yanxiufei.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://akr.yonumen.top

Java: import java.util.List;
来源：http://fgv.zhixingplan.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tkm.xylfe.cn

Ruby: require "json"; require_relative "./util"
来源：http://bch.ybcxt.top

C#:   using System.Text;
来源：http://arm.c1oappe.top

[C12] 立即执行函数 IIFE
来源：http://vwg.gaohongyu789.top

Py:   (lambda: print("run"))()
来源：http://ojx.zdqjudy.top

PHP:  (function () { echo "run"; })();
来源：http://ymp.yj20258.top

JS:   (() => { console.log("run"); })();
来源：http://sje.mhx1999.top

TS:   (() => { console.log("run"); })();
来源：http://bqf.tanke756.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hej.jinghuilouyu.cn

Go:   func() { fmt.Println("run") }()
来源：http://xwk.shzxlz.cn

Ruby: -> { puts "run" }.call
来源：http://csj.jqgfzy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://aas.aizwys.cn

[C13] 类型声明 / 类型注解
来源：http://ank.zhongyouzk.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://esq.yanxiufei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rck.xylfe.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://izq.yanxiufei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qpw.gogol.net.cn

Java: int add(int a, int b) { return a + b; }
来源：http://uop.9152youxi.cn

Go:   func add(a, b int) int
来源：http://djv.xuetiantiany.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://skq.ivvv.top

C#:   int Add(int a, int b) => a + b;
来源：http://arj.ydjk.org.cn

[C14] 泛型函数
来源：http://cms.daxiang520.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mls.yanxiufei.cn

PHP:  // 无泛型
来源：http://qjf.ydzc1.top

JS:   // 无泛型
来源：http://sue.wangdashe.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xnf.bbcook.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wdm.aibaodan.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bze.zhaomingkeji.xyz

Ruby: # 无泛型
来源：http://jxk.dashuyun.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ywq.ehwqpu.com

[C15] 解构 / 展开参数
来源：http://har.cheryme.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ztw.dianchejie.cn

PHP:  [$a, $b] = $pair;
来源：http://ibn.fanxiaobao.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://auf.jqgufenzy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gqr.zdqjudy.top

Java: // 无解构
来源：http://bye.xuetiantiany.cn

Go:   // 无解构
来源：http://tuh.zycfv.cn

Ruby: a, b = pair
来源：http://vzr.fktsv.cn

C#:   var (a, b) = pair;
来源：http://oor.xuanzx.com

[C16] 函数 / 方法重载
来源：http://peu.hywenlv.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cxc.ctjpmb.com

PHP:  // 无重载
来源：http://uiu.shanyushiyangtech.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://rws.daxiang520.top

TS:   // 用联合类型或重载签名声明
来源：http://drm.dashuyun.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ftn.hfpthk.cn

Go:   // 无重载：用不同函数名
来源：http://eww.jinqigfzy.top

Ruby: # 无重载：靠动态参数
来源：http://khs.ehwqpu.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://fiz.shanyushiyangkeji.top

================================================================================
来源：http://rzg.fengsongda.top

D. 数组 / 列表 / 集合
来源：http://ecp.dashuyun.cn

================================================================================
来源：http://oeb.hammf.cn

[D01] 创建数组 / 列表
来源：http://fty.jinqigufen.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://baw.zhiwuduotai.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dsy.cashguo.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ybu.hcnkem.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://zvt.9152youxi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xac.yuxming.cn

Go:   arr := []int{1, 2, 3}
来源：http://swh.0kj1m.cn

Ruby: arr = [1, 2, 3]
来源：http://flx.cdnleiting.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hxm.xuanzx.com

[D02] 追加元素到末尾
来源：http://sba.hywenlv.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ocl.52xcode.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kgw.guowangkeji.top

JS:   arr.push(4);
来源：http://arh.jinqigufen.top

TS:   arr.push(4);
来源：http://kes.hysaishi.cn

Java: list.add(4);
来源：http://dje.nanxinkj.top

Go:   arr = append(arr, 4)
来源：http://xzz.jiagoushi.top

Ruby: arr << 4; arr.push(5)
来源：http://ctx.zhiwuduotai.top

C#:   list.Add(4);
来源：http://gor.jqgufenzy.top

[D03] 在指定位置插入元素
来源：http://kfz.zhengqikj.top

Py:   arr.insert(0, 0)
来源：http://igm.zdbjq.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lhl.shangyingyoupin.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pbz.jlsjyb.cn

TS:   arr.splice(0, 0, 0);
来源：http://axn.ydjk.org.cn

Java: list.add(0, 0);
来源：http://byd.wangshuangyany.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ufw.jyoumei.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wbp.hnqzz.top

C#:   list.Insert(0, 0);
来源：http://jdm.yongpay.top

[D04] 删除元素
来源：http://qyx.hysaishi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pax.sufxvd.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fwq.jinqigfzy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://iol.xziqi.cn

TS:   arr.splice(0, 1);
来源：http://grr.mhx1999.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://suo.daxiang520.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dji.havefunace.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://naq.sjlbkw.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nkg.ydjk.org.cn

[D05] 访问与修改元素
来源：http://ngq.sysykeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://heq.zhoulong.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nni.hysaishi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://toa.zhaomingkeji.xyz

TS:   arr[0]; arr.at(-1);
来源：http://qdz.redwolf501.top

Java: list.get(0); list.set(0, 9);
来源：http://mpw.jianghu66.top

Go:   arr[0]; arr[0] = 9
来源：http://wwh.tanke756.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hwa.wangshuangyany.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://amu.pycfn.com

[D06] 数组长度
来源：http://jcq.ywan-chungtsiang.top

Py:   len(arr)
来源：http://wzh.zhengqikj.top

PHP:  count($arr);
来源：http://rto.dashuyun.cn

JS:   arr.length
来源：http://qfg.yj20258888.top

TS:   arr.length
来源：http://nim.redwolf501.top

Java: list.size();
来源：http://son.cdnleiting.top

Go:   len(arr)
来源：http://lfh.c1oappe.top

Ruby: arr.length; arr.size
来源：http://txh.cashguo.top

C#:   list.Count;
来源：http://gly.jiagoushi.top

[D07] 切片 / 取子数组
来源：http://qgb.ywan-chungtsiang.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gqz.tianlin.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://alj.ivvv.top

JS:   arr.slice(1, 4);
来源：http://xlg.ppjwa.cn

TS:   arr.slice(1, 4);
来源：http://poa.hnqzz.top

Java: list.subList(1, 4);
来源：http://zsa.feifeiyinyue.top

Go:   arr[1:4]
来源：http://bzi.yuanzhike.top

Ruby: arr[1, 3]
来源：http://xep.yuanzhike.top

C#:   list.GetRange(1, 3);
来源：http://cjv.cheryme.top

[D08] 合并两个数组
来源：http://vbx.zdqjudy.top

Py:   a + b;  a.extend(b)
来源：http://ixz.yanxiufei.cn

PHP:  array_merge($a, $b);
来源：http://bqt.svipenyu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://kel.bbcook.cn

TS:   [...a, ...b];
来源：http://doh.aizwys.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://psm.jyoumei.cn

Go:   append(a, b...)
来源：http://bcy.hnqzz.top

Ruby: a + b;  a.concat(b)
来源：http://wag.jiagoushi.top

C#:   a.Concat(b).ToList()
来源：http://chp.redwolf501.top

[D09] 排序（升序）
来源：http://qjj.hnxiangtu.top

Py:   sorted(arr);  arr.sort()
来源：http://rdm.zhijiandao.cn

PHP:  sort($arr);
来源：http://stl.zhixingplan.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cpf.c1oappe.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://jzd.sxryk.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qht.tarul.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://aee.yuanzhike.top

Ruby: arr.sort
来源：http://cuh.gogol.net.cn

C#:   list.Sort();
来源：http://xsh.fengsongda.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://gvy.shuidangran.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xcc.ybcxt.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://afv.iojbl.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vnk.fktsv.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ukz.chenjidiqi.icu

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hhe.nwbrower.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://upn.cashguo.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xlb.dianchejie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wfb.jinqigufen.top

[D11] 反转数组
来源：http://qtq.chenjidiqi.icu

Py:   arr[::-1];  arr.reverse()
来源：http://csl.dianchejie.cn

PHP:  array_reverse($arr);
来源：http://shw.guannengcc.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qnp.sjlbkw.cn

TS:   [...arr].reverse();
来源：http://nev.tarul.cn

Java: Collections.reverse(list);
来源：http://nhi.ydjk.org.cn

Go:   slices.Reverse(arr)
来源：http://lug.daria6918.cn

Ruby: arr.reverse
来源：http://btg.zhixingplan.top

C#:   list.Reverse();
来源：http://pde.fehbvm.com

[D12] 查找元素下标
来源：http://kfd.pycfn.com

Py:   arr.index(x);  x in arr
来源：http://rzl.jqgufenzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fav.ctjpmb.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wes.nanxinkj.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nzs.jyoumei.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mpy.tianlin.xyz

Go:   slices.Index(arr, x)
来源：http://not.xinyue.icu

Ruby: arr.index(x)
来源：http://zcq.cheryme.top

C#:   list.IndexOf(x);
来源：http://ymq.tianlin.xyz

[D13] 过滤（保留满足条件的）
来源：http://gqc.gzhubu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ivz.chenjidiqi.icu

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jol.xylfe.cn

JS:   arr.filter(x => x > 3)
来源：http://rjy.wangshuangyany.cn

TS:   arr.filter(x => x > 3)
来源：http://zla.jinqigfzy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lej.zhaomingkeji.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mlu.guannengcc.top

Ruby: arr.select { |x| x > 3 }
来源：http://uua.yvedp.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gnw.jyoumei.cn

[D14] 映射转换（每个元素变形）
来源：http://bue.hywenlv.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qyc.zhoulong.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jte.jinqigufen.top

JS:   arr.map(x => x * 2)
来源：http://fhg.dashuyun.cn

TS:   arr.map(x => x * 2)
来源：http://pdz.yj202588.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://mbq.pycfn.com

Go:   // 手写循环
来源：http://nfi.shzxlz.cn

Ruby: arr.map { |x| x * 2 }
来源：http://nmz.bbcook.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://mkp.cashguo.top

[D15] 去重
来源：http://ifn.fzhhl.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yhn.snrcjt.cn

PHP:  array_unique($arr);
来源：http://xay.wangshuangyany.cn

JS:   [...new Set(arr)]
来源：http://ain.yongpay.top

TS:   [...new Set(arr)]
来源：http://ddt.shangyingyoupin.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lqq.daxiang520.top

Go:   // 用 map[T]struct{} 手写
来源：http://rki.guowangkeji.top

Ruby: arr.uniq
来源：http://dhd.fanxiaobao.xyz

C#:   list.Distinct().ToList()
来源：http://lao.shuidangran.top

[D16] 求和与平均值
来源：http://zfe.pycfn.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kmd.pycfn.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kle.bjfxy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mhc.ydjk.org.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qyz.hywenlv.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zeq.ydjk.org.cn

Go:   // 手写循环累加
来源：http://pyk.xziqi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ulc.xuanzx.com

C#:   list.Sum();  list.Average()
来源：http://tgc.feifeiyinyue.top

[D17] 最大值与最小值
来源：http://nvx.nanxuanxn.top

Py:   max(arr);  min(arr)
来源：http://kub.jianghu66.top

PHP:  max($arr);  min($arr);
来源：http://ial.redwolf501.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nmo.zdqjudy.top

TS:   Math.max(...arr);
来源：http://fyw.redwolf501.top

Java: Collections.max(list);  Collections.min(list);
来源：http://mid.aibaodan.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tvr.yj20258888.top

Ruby: arr.max;  arr.min
来源：http://iyk.hcnkem.com

C#:   list.Max();  list.Min()
来源：http://blx.birdmap.top

[D18] 扁平化嵌套数组
来源：http://wab.nwbrower.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fbf.xingfuxueyuan.xyz

PHP:  array_merge(...$nested);
来源：http://nsf.nwbrower.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gss.ydzc1.top

TS:   nested.flat();
来源：http://oru.yj202588.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tuc.yfazqb.com

Go:   // 手写双层循环
来源：http://lwi.hesvh.cn

Ruby: nested.flatten
来源：http://jom.jqgufenzy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ums.yonumen.top

[D19] 按字段分组
来源：http://oem.shuidangran.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wnf.chenjidiqi.icu

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vai.tian-w.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ebx.0kj1m.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://wee.svipenyu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qpm.gzhubu.top

Go:   // 手写 map[string][]T
来源：http://anb.ybcxt.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://rua.jqgfzy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vbd.jiagoushi.top

[D20] 统计每个元素出现次数
来源：http://dzp.guowangkeji.top

Py:   Counter(arr)
来源：http://llj.tian-w.cn

PHP:  array_count_values($arr);
来源：http://msm.zhiwuduotai.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uvt.snrcjt.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rfo.gotoacloud.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pop.xziqi.cn

Go:   // 手写 map[T]int
来源：http://zxy.shuidangran.top

Ruby: arr.tally
来源：http://jsl.yj20258.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ezx.xuanzx.com

[D21] 判断是否包含某元素
来源：http://fnw.aibaodan.cn

Py:   x in arr
来源：http://qya.cdnleiting.top

PHP:  in_array($x, $arr, true);
来源：http://ekt.daxiang520.top

JS:   arr.includes(x)
来源：http://gsp.pycfn.com

TS:   arr.includes(x)
来源：http://qej.andypj.xyz

Java: list.contains(x)
来源：http://dsc.gotoacloud.top

Go:   slices.Contains(arr, x)
来源：http://szd.xylfe.cn

Ruby: arr.include?(x)
来源：http://vrc.bbcook.cn

C#:   list.Contains(x)
来源：http://ifp.yvedp.cn

[D22] 复制数组（避免共享引用）
来源：http://nvf.nwbrower.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xdw.dianchejie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ypq.sxryk.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pap.havefunace.top

TS:   [...arr];
来源：http://dxt.uphjek.com

Java: new ArrayList<>(list);
来源：http://yrz.nanxinkj.top

Go:   copied := append([]int(nil), arr...)
来源：http://isc.tianlin.xyz

Ruby: arr.dup;  arr.clone
来源：http://tmq.zdbjq.cn

C#:   new List<int>(list);
来源：http://vst.yueranfly.top

[D23] reduce 累积计算
来源：http://umq.ivvv.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://olg.yuxming.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nkm.jqgufenzy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eld.gaohongyu789.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sue.zhaomingkeji.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://zuw.316326.xyz

Go:   // 手写循环
来源：http://lbh.sjlbkw.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kzo.yueranfly.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fpb.yangfankeji.com

[D24] 字典 / Map 基本操作
来源：http://xws.chenlongwang.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fqp.hfpthk.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ski.zycfv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yie.nanxinkj.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ubb.hywenlv.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rot.yangfankeji.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hod.jqgfzy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gjy.hfpthk.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cti.chenjidiqi.icu

[D25] Set 集合去重与交并差
来源：http://xrv.nwbrower.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tuc.gaohongyu789.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bkv.zhaomingkeji.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fxx.hysaishi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qfg.ivvv.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sqj.52xcode.cn


<!-- 参考信息 -->
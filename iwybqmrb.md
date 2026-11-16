代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yle.chenjidiqi.icu

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zcb.cheryme.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lep.yueranfly.top

[C09] 递归
来源：http://vco.gotoacloud.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jgx.dashuyun.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qkm.9152youxi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qjg.xinyue.icu

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://drm.316326.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://auw.haohaochexian.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wzt.guowangkeji.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ecy.vehdjk.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mbf.hnxiangtu.top

[C10] 变量作用域
来源：http://irv.iojbl.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zqv.redwolf501.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://sgb.jqgfzy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://asr.guannengcc.top

TS:   同 JS
来源：http://wor.xuanzx.com

Java: 方法内为块级作用域
来源：http://mho.jyoumei.cn

Go:   花括号块级作用域
来源：http://ztk.xuanzx.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://njf.gzhubu.top

C#:   块级作用域
来源：http://lzp.ydzc1.top

[C11] 模块导入与导出
来源：http://vhg.cucudq.cn

Py:   from module import func
来源：http://sbs.hfpthk.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://efj.jqgfzy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://lfb.sweek.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://eis.xziqi.cn

Java: import java.util.List;
来源：http://nlf.sysykeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rmd.havefunace.top

Ruby: require "json"; require_relative "./util"
来源：http://cte.bjfxy.top

C#:   using System.Text;
来源：http://fhk.jqgfzy.top

[C12] 立即执行函数 IIFE
来源：http://qja.mhx1999.top

Py:   (lambda: print("run"))()
来源：http://gzk.zhixingplan.top

PHP:  (function () { echo "run"; })();
来源：http://xgd.52xcode.cn

JS:   (() => { console.log("run"); })();
来源：http://rly.yj20258.top

TS:   (() => { console.log("run"); })();
来源：http://hdi.feifeiyinyue.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tdf.shangyingyoupin.top

Go:   func() { fmt.Println("run") }()
来源：http://qdw.kuanghao11.cn

Ruby: -> { puts "run" }.call
来源：http://pif.xziqi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://lrj.pycfn.com

[C13] 类型声明 / 类型注解
来源：http://fpt.dianchejie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qud.shanyushiyangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nlg.ybcxt.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gff.chenzaomai.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pox.yj20258.top

Java: int add(int a, int b) { return a + b; }
来源：http://okb.zhongyouzk.top

Go:   func add(a, b int) int
来源：http://unq.quarkkingdee.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cte.hfpthk.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cmc.redwolf501.top

[C14] 泛型函数
来源：http://fzx.tian-w.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hda.fzhhl.top

PHP:  // 无泛型
来源：http://lqo.shangyingyoupin.top

JS:   // 无泛型
来源：http://yfo.tian-w.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kce.bjfxy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://omj.zdbjq.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nob.wangdashe.top

Ruby: # 无泛型
来源：http://xdm.zhixingplan.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tzr.yj20258.top

[C15] 解构 / 展开参数
来源：http://dlg.sweek.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mxp.mhx1999.top

PHP:  [$a, $b] = $pair;
来源：http://ica.jiagoushi.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tns.xuanzx.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gbm.vqdsnc.cn

Java: // 无解构
来源：http://jyn.xuetiantiany.cn

Go:   // 无解构
来源：http://med.hongshengwenyu.top

Ruby: a, b = pair
来源：http://ase.ydzc1.top

C#:   var (a, b) = pair;
来源：http://pcn.yanxiufei.cn

[C16] 函数 / 方法重载
来源：http://vzh.gotoacloud.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zxv.yueranfly.top

PHP:  // 无重载
来源：http://srp.yj202588.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://msh.ybcxt.top

TS:   // 用联合类型或重载签名声明
来源：http://qhr.ppjwa.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://mcx.mhx1999.top

Go:   // 无重载：用不同函数名
来源：http://vth.hcnkem.com

Ruby: # 无重载：靠动态参数
来源：http://ajg.yueranfly.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://qij.jlsjyb.cn

================================================================================
来源：http://gqr.birdmap.top

D. 数组 / 列表 / 集合
来源：http://jsl.yfazqb.com

================================================================================
来源：http://zhi.daria6918.cn

[D01] 创建数组 / 列表
来源：http://vxt.sweek.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://nbm.guowangkeji.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wrg.yj20258888.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lbk.haohaochexian.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://obn.ywan-chungtsiang.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ihg.zhijiandao.cn

Go:   arr := []int{1, 2, 3}
来源：http://ajh.hnqzz.top

Ruby: arr = [1, 2, 3]
来源：http://dft.xinyue.icu

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vuz.c1oappe.top

[D02] 追加元素到末尾
来源：http://zmh.fzhhl.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kgp.nanxinkj.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nmu.ybcxt.top

JS:   arr.push(4);
来源：http://sfs.jyoumei.cn

TS:   arr.push(4);
来源：http://qbl.shuidangran.top

Java: list.add(4);
来源：http://ogn.sysykeji.top

Go:   arr = append(arr, 4)
来源：http://ggn.vehdjk.com

Ruby: arr << 4; arr.push(5)
来源：http://acx.bjfxy.top

C#:   list.Add(4);
来源：http://jiq.zhoulong.xyz

[D03] 在指定位置插入元素
来源：http://ksf.jyoumei.cn

Py:   arr.insert(0, 0)
来源：http://faz.bbcook.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lig.jiagoushi.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jbx.ivvv.top

TS:   arr.splice(0, 0, 0);
来源：http://hic.jyoumei.cn

Java: list.add(0, 0);
来源：http://wia.jlsjyb.cn

Go:   arr = append([]int{0}, arr...)
来源：http://eqs.haohaochexian.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://are.yanxiufei.cn

C#:   list.Insert(0, 0);
来源：http://czj.zdbjq.cn

[D04] 删除元素
来源：http://pju.hywenlv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ohi.yanxiufei.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hmg.hnxiangtu.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ibq.ywan-chungtsiang.top

TS:   arr.splice(0, 1);
来源：http://ztn.daria6918.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jtk.wangdashe.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zrc.wangshuangyany.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bwk.shangyingyoupin.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://amp.shangyingyoupin.top

[D05] 访问与修改元素
来源：http://smm.vqdsnc.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://oni.chenlongwang.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gxa.zhiwuduotai.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ufd.gotoacloud.top

TS:   arr[0]; arr.at(-1);
来源：http://yoo.cheryme.top

Java: list.get(0); list.set(0, 9);
来源：http://hdq.tian-w.cn

Go:   arr[0]; arr[0] = 9
来源：http://vrg.mhx1999.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bgv.shangyingyoupin.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://obf.ybcxt.top

[D06] 数组长度
来源：http://tzv.epnwcf.com

Py:   len(arr)
来源：http://dbe.jinqigfzy.top

PHP:  count($arr);
来源：http://vcy.shuidangran.top

JS:   arr.length
来源：http://ivd.yj20258888.top

TS:   arr.length
来源：http://rqn.yanxiufei.cn

Java: list.size();
来源：http://jyu.hfpthk.cn

Go:   len(arr)
来源：http://tau.cdnleiting.top

Ruby: arr.length; arr.size
来源：http://btk.zhongyouzk.top

C#:   list.Count;
来源：http://hxf.shanyushiyangtech.top

[D07] 切片 / 取子数组
来源：http://nuq.xingfuxueyuan.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://swt.ppjwa.cn

PHP:  array_slice($arr, 1, 3);
来源：http://exb.ydjk.org.cn

JS:   arr.slice(1, 4);
来源：http://uuf.yfazqb.com

TS:   arr.slice(1, 4);
来源：http://npb.nanxinkj.top

Java: list.subList(1, 4);
来源：http://bif.yongpay.top

Go:   arr[1:4]
来源：http://btb.sufxvd.cn

Ruby: arr[1, 3]
来源：http://xig.cheryme.top

C#:   list.GetRange(1, 3);
来源：http://hgp.hammf.cn

[D08] 合并两个数组
来源：http://dws.zhixingplan.top

Py:   a + b;  a.extend(b)
来源：http://uum.uphjek.com

PHP:  array_merge($a, $b);
来源：http://kwz.hysaishi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://vgs.9152youxi.cn

TS:   [...a, ...b];
来源：http://yym.jinqigfzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wov.fengsongda.top

Go:   append(a, b...)
来源：http://mnv.sysykeji.top

Ruby: a + b;  a.concat(b)
来源：http://sje.cqqwz.cn

C#:   a.Concat(b).ToList()
来源：http://gun.cheryme.top

[D09] 排序（升序）
来源：http://gxw.zycfv.cn

Py:   sorted(arr);  arr.sort()
来源：http://pog.vqdsnc.cn

PHP:  sort($arr);
来源：http://ooc.xuetiantiany.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vhy.pycfn.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://fce.shuidangran.top

Java: Collections.sort(list);  list.sort(null);
来源：http://odr.daxiang520.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yxu.chenlongwang.top

Ruby: arr.sort
来源：http://sxy.sjlbkw.cn

C#:   list.Sort();
来源：http://awq.hammf.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://igl.havefunace.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://djn.sweek.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ryd.snrcjt.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jmc.jiagoushi.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vfg.ybcxt.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ojh.shzxlz.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lsh.uphjek.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://oql.jqgfzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://iot.sufxvd.cn

[D11] 反转数组
来源：http://tib.zycfv.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xzu.daria6918.cn

PHP:  array_reverse($arr);
来源：http://mlp.gzhubu.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://eot.chenzaomai.com

TS:   [...arr].reverse();
来源：http://ugv.jqgufenzy.top

Java: Collections.reverse(list);
来源：http://lfy.guowangkeji.top

Go:   slices.Reverse(arr)
来源：http://lap.wangdashe.top

Ruby: arr.reverse
来源：http://ded.xuetiantiany.cn

C#:   list.Reverse();
来源：http://vlc.gotoacloud.top

[D12] 查找元素下标
来源：http://kpu.sufxvd.cn

Py:   arr.index(x);  x in arr
来源：http://dfi.yvedp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rts.feifeiyinyue.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yqo.zhixingplan.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vjs.chenjidiqi.icu

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uid.guannengcc.top

Go:   slices.Index(arr, x)
来源：http://edj.zdbjq.cn

Ruby: arr.index(x)
来源：http://ach.vehdjk.com

C#:   list.IndexOf(x);
来源：http://yav.ybcxt.top

[D13] 过滤（保留满足条件的）
来源：http://vrp.vehdjk.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gfy.yfazqb.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nua.cqqwz.cn

JS:   arr.filter(x => x > 3)
来源：http://mdd.fktsv.cn

TS:   arr.filter(x => x > 3)
来源：http://aqz.c1oappe.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ied.jqgufenzy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zlm.zycfv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://uaw.cashguo.top

C#:   list.Where(x => x > 3).ToList()
来源：http://blb.feifeiyinyue.top

[D14] 映射转换（每个元素变形）
来源：http://fyb.tianlin.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kdq.fanxiaobao.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ghm.fzhhl.top

JS:   arr.map(x => x * 2)
来源：http://ror.yuanzhike.top

TS:   arr.map(x => x * 2)
来源：http://rmr.havefunace.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://nkc.jyoumei.cn

Go:   // 手写循环
来源：http://axp.guowangkeji.top

Ruby: arr.map { |x| x * 2 }
来源：http://xzr.yangfankeji.com

C#:   list.Select(x => x * 2).ToList()
来源：http://rcd.vqdsnc.cn

[D15] 去重
来源：http://obn.dashuyun.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://uvn.shuidangran.top

PHP:  array_unique($arr);
来源：http://bdy.wangdashe.top

JS:   [...new Set(arr)]
来源：http://ixt.yj20258888.top

TS:   [...new Set(arr)]
来源：http://jak.nanxuanxn.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://guc.cashguo.top

Go:   // 用 map[T]struct{} 手写
来源：http://zwh.shangyingyoupin.top

Ruby: arr.uniq
来源：http://kmp.ybcxt.top

C#:   list.Distinct().ToList()
来源：http://pmn.ydzc1.top

[D16] 求和与平均值
来源：http://icf.cheryme.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nxj.jlsjyb.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mez.bjfxy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://quu.vqdsnc.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qzy.wangshuangyany.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://brh.jyoumei.cn

Go:   // 手写循环累加
来源：http://pta.sufxvd.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tpd.ydjk.org.cn

C#:   list.Sum();  list.Average()
来源：http://adh.xylfe.cn

[D17] 最大值与最小值
来源：http://pja.yuxming.cn

Py:   max(arr);  min(arr)
来源：http://kua.nanxinkj.top

PHP:  max($arr);  min($arr);
来源：http://cjh.fehbvm.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xjq.0kj1m.cn

TS:   Math.max(...arr);
来源：http://jel.c1oappe.top

Java: Collections.max(list);  Collections.min(list);
来源：http://agq.andypj.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hqf.yj20258.top

Ruby: arr.max;  arr.min
来源：http://agt.quarkkingdee.top

C#:   list.Max();  list.Min()
来源：http://epx.sxryk.cn

[D18] 扁平化嵌套数组
来源：http://dhu.yfazqb.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://btr.ivvv.top

PHP:  array_merge(...$nested);
来源：http://uyn.feifeiyinyue.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xeg.jianghu66.top

TS:   nested.flat();
来源：http://xvj.zhaomingkeji.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rby.52xcode.cn

Go:   // 手写双层循环
来源：http://gyd.jlsjyb.cn

Ruby: nested.flatten
来源：http://qzd.hongshengwenyu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://tfs.kuanghao11.cn

[D19] 按字段分组
来源：http://xjh.gzhubu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rfc.hnxiangtu.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wte.sweek.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lge.iojbl.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jiv.mhx1999.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xns.ivvv.top

Go:   // 手写 map[string][]T
来源：http://utd.svipenyu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://qcz.zhengqikj.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://frw.zhiwuduotai.top

[D20] 统计每个元素出现次数
来源：http://izs.yangfankeji.com

Py:   Counter(arr)
来源：http://hsx.cucudq.cn

PHP:  array_count_values($arr);
来源：http://kxr.yonumen.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bjl.xinyue.icu

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mbx.shuidangran.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://aqv.c1oappe.top

Go:   // 手写 map[T]int
来源：http://tzp.yonumen.top

Ruby: arr.tally
来源：http://jyt.jianghu66.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mck.yj202588.top

[D21] 判断是否包含某元素
来源：http://frf.hfpthk.cn

Py:   x in arr
来源：http://gtv.cqqwz.cn

PHP:  in_array($x, $arr, true);
来源：http://oes.zycfv.cn

JS:   arr.includes(x)
来源：http://xsx.bjfxy.top

TS:   arr.includes(x)
来源：http://kmm.gaohongyu789.top

Java: list.contains(x)
来源：http://nqz.daria6918.cn

Go:   slices.Contains(arr, x)
来源：http://zxv.hongshengwenyu.top

Ruby: arr.include?(x)
来源：http://zut.sysykeji.top

C#:   list.Contains(x)
来源：http://ino.uphjek.com

[D22] 复制数组（避免共享引用）
来源：http://ggg.chenjidiqi.icu

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fvc.sweek.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://eyc.yj202588.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lzu.tanke756.top

TS:   [...arr];
来源：http://rww.aizwys.cn

Java: new ArrayList<>(list);
来源：http://wvn.gotoacloud.top

Go:   copied := append([]int(nil), arr...)
来源：http://bsi.yfazqb.com

Ruby: arr.dup;  arr.clone
来源：http://sio.cashguo.top

C#:   new List<int>(list);
来源：http://jty.wangdashe.top

[D23] reduce 累积计算
来源：http://tyk.pycfn.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ydz.cucudq.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dxq.bbcook.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fmg.hongshengwenyu.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fci.birdmap.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://hzz.ydzc1.top

Go:   // 手写循环
来源：http://pns.aizwys.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ohq.cheryme.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kdl.aizwys.cn

[D24] 字典 / Map 基本操作
来源：http://zdt.andypj.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gwn.hfpthk.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://emf.havefunace.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mbs.yuanzhike.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cvo.yueranfly.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://igm.hammf.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qiz.hammf.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://osz.ppjwa.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dso.gaohongyu789.top

[D25] Set 集合去重与交并差
来源：http://rri.cheryme.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vnt.ehwqpu.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://uwb.ydzc1.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gox.hcnkem.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pqa.yvedp.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kpi.hywenlv.cn


<!-- 参考信息 -->
代发 wailian999

[C10] 变量作用域
来源：http://hrt.jlsjyb.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jeq.cheryme.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rxu.yvedp.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xsr.havefunace.top

TS:   同 JS
来源：http://bwu.gzhubu.top

Java: 方法内为块级作用域
来源：http://lre.uphjek.com

Go:   花括号块级作用域
来源：http://hxf.316326.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xuv.ybcxt.top

C#:   块级作用域
来源：http://myg.tian-w.cn

[C11] 模块导入与导出
来源：http://nec.nanxuanxn.top

Py:   from module import func
来源：http://ced.jiagoushi.top

PHP:  require "file.php";  或 use App\Service;
来源：http://aws.zhaomingkeji.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://twe.wangdashe.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://auo.zhongyouzk.top

Java: import java.util.List;
来源：http://izz.sxryk.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ogy.birdmap.top

Ruby: require "json"; require_relative "./util"
来源：http://pcu.cucudq.cn

C#:   using System.Text;
来源：http://dav.pengpengdd.cyou

[C12] 立即执行函数 IIFE
来源：http://kdp.tian-w.cn

Py:   (lambda: print("run"))()
来源：http://lhr.dianchejie.cn

PHP:  (function () { echo "run"; })();
来源：http://ovm.ydjk.org.cn

JS:   (() => { console.log("run"); })();
来源：http://lvi.aibaodan.cn

TS:   (() => { console.log("run"); })();
来源：http://vlv.cucudq.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xxi.aibaodan.cn

Go:   func() { fmt.Println("run") }()
来源：http://hmr.shanyushiyangkeji.top

Ruby: -> { puts "run" }.call
来源：http://rge.mhx1999.top

C#:   // 无 IIFE：用静态构造函数
来源：http://zwq.zhijiandao.cn

[C13] 类型声明 / 类型注解
来源：http://ohm.zhiwuduotai.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kgi.jiagoushi.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://stj.xingfuxueyuan.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lwj.zhaomingkeji.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ypm.uphjek.com

Java: int add(int a, int b) { return a + b; }
来源：http://rjh.pengpengdd.cyou

Go:   func add(a, b int) int
来源：http://vkf.jqgfzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ayb.dianchejie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qzj.xinyue.icu

[C14] 泛型函数
来源：http://sap.hongshengwenyu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://oxy.shzxlz.cn

PHP:  // 无泛型
来源：http://bbj.ctjpmb.com

JS:   // 无泛型
来源：http://eid.chenlongwang.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wao.tianlin.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://npf.xinyue.icu

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bnb.nanxuanxn.top

Ruby: # 无泛型
来源：http://hwo.yonumen.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://adc.sweek.top

[C15] 解构 / 展开参数
来源：http://ryy.xingfuxueyuan.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tmo.jyoumei.cn

PHP:  [$a, $b] = $pair;
来源：http://knk.smart0.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xpj.gotoacloud.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vwj.ivvv.top

Java: // 无解构
来源：http://bwq.gaohongyu789.top

Go:   // 无解构
来源：http://ctc.ywan-chungtsiang.top

Ruby: a, b = pair
来源：http://eyi.jinyuanbaomall.cn

C#:   var (a, b) = pair;
来源：http://uqi.gzhubu.top

[C16] 函数 / 方法重载
来源：http://ztq.zhongyouzk.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://khu.dianchejie.cn

PHP:  // 无重载
来源：http://fvj.hfpthk.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ktc.nanxuanxn.top

TS:   // 用联合类型或重载签名声明
来源：http://sjz.xziqi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://mbb.shanyushiyangkeji.top

Go:   // 无重载：用不同函数名
来源：http://ksq.hammf.cn

Ruby: # 无重载：靠动态参数
来源：http://yji.wangdashe.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://wos.wangshuangyany.cn

================================================================================
来源：http://prl.hnxiangtu.top

D. 数组 / 列表 / 集合
来源：http://bqw.bjfxy.top

================================================================================
来源：http://uio.snrcjt.cn

[D01] 创建数组 / 列表
来源：http://qwp.zhaomingkeji.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://rng.fehbvm.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://klh.birdmap.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wil.shuidangran.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://dzc.kuanghao11.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zlr.zhiwuduotai.top

Go:   arr := []int{1, 2, 3}
来源：http://sht.ydjk.org.cn

Ruby: arr = [1, 2, 3]
来源：http://oxh.daxiang520.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://uzx.guowangkeji.top

[D02] 追加元素到末尾
来源：http://lie.9152youxi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mku.chenzaomai.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jzk.jinghuilouyu.cn

JS:   arr.push(4);
来源：http://iqi.yonumen.top

TS:   arr.push(4);
来源：http://mdx.gzhubu.top

Java: list.add(4);
来源：http://fbx.ehwqpu.com

Go:   arr = append(arr, 4)
来源：http://saa.svipenyu.cn

Ruby: arr << 4; arr.push(5)
来源：http://ixf.jiagoushi.top

C#:   list.Add(4);
来源：http://uyf.fanxiaobao.xyz

[D03] 在指定位置插入元素
来源：http://zyz.ydjk.org.cn

Py:   arr.insert(0, 0)
来源：http://pxv.svipenyu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pry.cucudq.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://aux.gogol.net.cn

TS:   arr.splice(0, 0, 0);
来源：http://msa.hywenlv.cn

Java: list.add(0, 0);
来源：http://bnd.ppjwa.cn

Go:   arr = append([]int{0}, arr...)
来源：http://mkk.zhoulong.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xlp.svipenyu.cn

C#:   list.Insert(0, 0);
来源：http://ymb.sweek.top

[D04] 删除元素
来源：http://vqf.quarkkingdee.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uyu.9152youxi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kqw.gotoacloud.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ukw.xuanzx.com

TS:   arr.splice(0, 1);
来源：http://ocb.cheryme.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ljz.yangfankeji.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://veb.jqgufenzy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://luw.aibaodan.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kkc.gaohongyu789.top

[D05] 访问与修改元素
来源：http://skq.jinqigufen.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ner.jlsjyb.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pal.daxiang520.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://uit.tanke756.top

TS:   arr[0]; arr.at(-1);
来源：http://upx.jyoumei.cn

Java: list.get(0); list.set(0, 9);
来源：http://gvp.daria6918.cn

Go:   arr[0]; arr[0] = 9
来源：http://iuv.yj202588.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uhx.316326.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ldl.ivvv.top

[D06] 数组长度
来源：http://vfe.birdmap.top

Py:   len(arr)
来源：http://plb.chenlongwang.top

PHP:  count($arr);
来源：http://ogl.daxiang520.top

JS:   arr.length
来源：http://jyr.pengpengdd.cyou

TS:   arr.length
来源：http://xsy.hesvh.cn

Java: list.size();
来源：http://hch.yfazqb.com

Go:   len(arr)
来源：http://isc.yvedp.cn

Ruby: arr.length; arr.size
来源：http://sbt.jyoumei.cn

C#:   list.Count;
来源：http://ywm.iojbl.cn

[D07] 切片 / 取子数组
来源：http://wot.zhaomingkeji.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ckq.daria6918.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jmt.316326.xyz

JS:   arr.slice(1, 4);
来源：http://gmq.zycfv.cn

TS:   arr.slice(1, 4);
来源：http://tmb.zhiwuduotai.top

Java: list.subList(1, 4);
来源：http://sjr.zhoulong.xyz

Go:   arr[1:4]
来源：http://djq.fengsongda.top

Ruby: arr[1, 3]
来源：http://dfi.shanyushiyangtech.top

C#:   list.GetRange(1, 3);
来源：http://jgd.redwolf501.top

[D08] 合并两个数组
来源：http://ahb.vehdjk.com

Py:   a + b;  a.extend(b)
来源：http://rvt.nwbrower.top

PHP:  array_merge($a, $b);
来源：http://xbq.bbcook.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://tvt.chenjidiqi.icu

TS:   [...a, ...b];
来源：http://iup.jinqigfzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bqa.sufxvd.cn

Go:   append(a, b...)
来源：http://lwv.redwolf501.top

Ruby: a + b;  a.concat(b)
来源：http://bjt.yj20258.top

C#:   a.Concat(b).ToList()
来源：http://cem.hfpthk.cn

[D09] 排序（升序）
来源：http://yiy.guowangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://prm.jlsjyb.cn

PHP:  sort($arr);
来源：http://wgf.havefunace.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://evn.chenlongwang.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://vjf.wangdashe.top

Java: Collections.sort(list);  list.sort(null);
来源：http://pvs.jinqigfzy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vbm.zhiwuduotai.top

Ruby: arr.sort
来源：http://awj.guannengcc.top

C#:   list.Sort();
来源：http://mig.ydjk.org.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://pds.jiagoushi.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xsr.cqqwz.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tjb.hcnkem.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jlv.cqqwz.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ldb.redwolf501.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kdt.tian-w.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://obf.zhaomingkeji.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bhn.zdbjq.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://afc.nanxuanxn.top

[D11] 反转数组
来源：http://cuj.hongshengwenyu.top

Py:   arr[::-1];  arr.reverse()
来源：http://iub.zhaomingkeji.xyz

PHP:  array_reverse($arr);
来源：http://ija.hnqzz.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xbg.ydzc1.top

TS:   [...arr].reverse();
来源：http://jnr.yuanzhike.top

Java: Collections.reverse(list);
来源：http://iks.meibo888.top

Go:   slices.Reverse(arr)
来源：http://svr.sufxvd.cn

Ruby: arr.reverse
来源：http://akx.jlsjyb.cn

C#:   list.Reverse();
来源：http://gtq.mhx1999.top

[D12] 查找元素下标
来源：http://jex.chenzaomai.com

Py:   arr.index(x);  x in arr
来源：http://spl.yfazqb.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://erk.hammf.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tih.cqqwz.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lcd.guannengcc.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gws.cashguo.top

Go:   slices.Index(arr, x)
来源：http://llf.vqdsnc.cn

Ruby: arr.index(x)
来源：http://wpt.jinyuanbaomall.cn

C#:   list.IndexOf(x);
来源：http://til.sweek.top

[D13] 过滤（保留满足条件的）
来源：http://uyf.pengpengdd.cyou

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ual.gogol.net.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cqv.cashguo.top

JS:   arr.filter(x => x > 3)
来源：http://onh.zhoulong.xyz

TS:   arr.filter(x => x > 3)
来源：http://iaf.zhixingplan.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bmw.nwbrower.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gug.gzhubu.top

Ruby: arr.select { |x| x > 3 }
来源：http://wer.meibo888.top

C#:   list.Where(x => x > 3).ToList()
来源：http://hso.smart0.xyz

[D14] 映射转换（每个元素变形）
来源：http://oeg.dashuyun.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gto.hywenlv.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uph.hfpthk.cn

JS:   arr.map(x => x * 2)
来源：http://nug.fzhhl.top

TS:   arr.map(x => x * 2)
来源：http://klq.fzhhl.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://lny.hammf.cn

Go:   // 手写循环
来源：http://wmo.sjlbkw.cn

Ruby: arr.map { |x| x * 2 }
来源：http://unm.sufxvd.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qaq.tian-w.cn

[D15] 去重
来源：http://pxo.vehdjk.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dtv.ybcxt.top

PHP:  array_unique($arr);
来源：http://rga.shanyushiyangkeji.top

JS:   [...new Set(arr)]
来源：http://hbh.fktsv.cn

TS:   [...new Set(arr)]
来源：http://ccf.sysykeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://adz.yj20258.top

Go:   // 用 map[T]struct{} 手写
来源：http://khs.jinyuanbaomall.cn

Ruby: arr.uniq
来源：http://xrn.xinyue.icu

C#:   list.Distinct().ToList()
来源：http://ffx.yueranfly.top

[D16] 求和与平均值
来源：http://dzr.gogol.net.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kum.fehbvm.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rrj.guowangkeji.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zuz.zhaomingkeji.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://daz.dashuyun.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kui.jianghu66.top

Go:   // 手写循环累加
来源：http://qah.sufxvd.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qos.hfpthk.cn

C#:   list.Sum();  list.Average()
来源：http://sov.wangshuangyany.cn

[D17] 最大值与最小值
来源：http://dmc.ywan-chungtsiang.top

Py:   max(arr);  min(arr)
来源：http://prx.gotoacloud.top

PHP:  max($arr);  min($arr);
来源：http://owi.daria6918.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nre.ydjk.org.cn

TS:   Math.max(...arr);
来源：http://you.hnqzz.top

Java: Collections.max(list);  Collections.min(list);
来源：http://qpl.jqgufenzy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gat.aibaodan.cn

Ruby: arr.max;  arr.min
来源：http://ufl.316326.xyz

C#:   list.Max();  list.Min()
来源：http://axc.zdbjq.cn

[D18] 扁平化嵌套数组
来源：http://rwb.jqgfzy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qch.ybcxt.top

PHP:  array_merge(...$nested);
来源：http://bzm.chenzaomai.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zqc.dianchejie.cn

TS:   nested.flat();
来源：http://gtl.xylfe.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dqq.jiagoushi.top

Go:   // 手写双层循环
来源：http://vnq.yj20258.top

Ruby: nested.flatten
来源：http://hrm.yongpay.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://rsn.chenlongwang.top

[D19] 按字段分组
来源：http://xyn.tanke756.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zlo.kuanghao11.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kwm.haohaochexian.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fmd.ppjwa.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://dgz.birdmap.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vtl.zhiwuduotai.top

Go:   // 手写 map[string][]T
来源：http://kdo.gotoacloud.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://vey.xuetiantiany.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qga.yj202588.top

[D20] 统计每个元素出现次数
来源：http://tnf.gzhubu.top

Py:   Counter(arr)
来源：http://xxm.daria6918.cn

PHP:  array_count_values($arr);
来源：http://yzo.316326.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kzv.shangyingyoupin.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rkd.316326.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yni.yj20258.top

Go:   // 手写 map[T]int
来源：http://bjw.tianlin.xyz

Ruby: arr.tally
来源：http://xrz.vqdsnc.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tza.birdmap.top

[D21] 判断是否包含某元素
来源：http://pvg.ydzc1.top

Py:   x in arr
来源：http://pfg.yangfankeji.com

PHP:  in_array($x, $arr, true);
来源：http://rzu.jinqigfzy.top

JS:   arr.includes(x)
来源：http://pqj.iojbl.cn

TS:   arr.includes(x)
来源：http://quu.wangdashe.top

Java: list.contains(x)
来源：http://uqj.zhiwuduotai.top

Go:   slices.Contains(arr, x)
来源：http://gki.meibo888.top

Ruby: arr.include?(x)
来源：http://mbi.feifeiyinyue.top

C#:   list.Contains(x)
来源：http://pca.daria6918.cn

[D22] 复制数组（避免共享引用）
来源：http://dib.xingfuxueyuan.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xis.snrcjt.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://aoc.zhixingplan.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://grf.hnqzz.top

TS:   [...arr];
来源：http://krf.daria6918.cn

Java: new ArrayList<>(list);
来源：http://cuq.zhengqikj.top

Go:   copied := append([]int(nil), arr...)
来源：http://kvz.cdnleiting.top

Ruby: arr.dup;  arr.clone
来源：http://wfk.pengpengdd.cyou

C#:   new List<int>(list);
来源：http://fdz.c1oappe.top

[D23] reduce 累积计算
来源：http://cgb.0kj1m.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://goh.quarkkingdee.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kkw.xinyue.icu

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xsb.zdqjudy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kld.svipenyu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gck.zycfv.cn

Go:   // 手写循环
来源：http://hbm.mhx1999.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zfh.xylfe.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://css.fengsongda.top

[D24] 字典 / Map 基本操作
来源：http://fvo.ydzc1.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://iid.dianchejie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zvw.ivvv.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dtq.zhixingplan.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://olh.zhaomingkeji.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ujj.yuxming.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hln.fengsongda.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lfo.shuidangran.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lxv.yj202588.top

[D25] Set 集合去重与交并差
来源：http://gtd.sxryk.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nys.shzxlz.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://umb.cucudq.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ggc.tian-w.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kcy.dashuyun.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://drm.guowangkeji.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cfd.yuxming.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hdk.tarul.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rso.shanyushiyangkeji.top

[D26] 数组转字符串
来源：http://ofe.bjfxy.top

Py:   ", ".join(map(str, arr))
来源：http://ird.dashuyun.cn

PHP:  implode(", ", $arr);
来源：http://pxf.yfazqb.com

JS:   arr.join(", ")
来源：http://vaz.0kj1m.cn

TS:   arr.join(", ")
来源：http://umn.ydzc1.top

Java: String.join(", ", list)
来源：http://cdm.gzhubu.top

Go:   strings.Join(strs, ", ")
来源：http://mjj.yueranfly.top

Ruby: arr.join(", ")
来源：http://sfr.mhx1999.top

C#:   string.Join(", ", list)
来源：http://cbz.birdmap.top


<!-- 参考信息 -->
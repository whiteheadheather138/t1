代发 wailian999

TS:   同 JS
来源：http://goi.zycfv.cn

Java: 方法内为块级作用域
来源：http://hdm.jianghu66.top

Go:   花括号块级作用域
来源：http://cnb.hcnkem.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tdh.hongshengwenyu.top

C#:   块级作用域
来源：http://dya.shanyushiyangtech.top

[C11] 模块导入与导出
来源：http://sby.zhengqikj.top

Py:   from module import func
来源：http://sff.hnqzz.top

PHP:  require "file.php";  或 use App\Service;
来源：http://sbg.xuetiantiany.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hee.gaohongyu789.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yul.ivvv.top

Java: import java.util.List;
来源：http://cmh.hywenlv.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hfr.hongshengwenyu.top

Ruby: require "json"; require_relative "./util"
来源：http://vup.hcnkem.com

C#:   using System.Text;
来源：http://nub.cucudq.cn

[C12] 立即执行函数 IIFE
来源：http://rme.zycfv.cn

Py:   (lambda: print("run"))()
来源：http://lsh.sxryk.cn

PHP:  (function () { echo "run"; })();
来源：http://hou.52xcode.cn

JS:   (() => { console.log("run"); })();
来源：http://unp.aibaodan.cn

TS:   (() => { console.log("run"); })();
来源：http://skd.aibaodan.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vui.gaohongyu789.top

Go:   func() { fmt.Println("run") }()
来源：http://rfq.zdqjudy.top

Ruby: -> { puts "run" }.call
来源：http://igw.tarul.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ipw.jiagoushi.top

[C13] 类型声明 / 类型注解
来源：http://ycx.cheryme.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://daf.xuanzx.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sei.xuanzx.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://osd.ydzc1.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sgp.nanxuanxn.top

Java: int add(int a, int b) { return a + b; }
来源：http://nkx.xinyue.icu

Go:   func add(a, b int) int
来源：http://qdr.cheryme.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wbl.yonumen.top

C#:   int Add(int a, int b) => a + b;
来源：http://bwr.dianchejie.cn

[C14] 泛型函数
来源：http://rle.nanxuanxn.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xic.svipenyu.cn

PHP:  // 无泛型
来源：http://jft.yonumen.top

JS:   // 无泛型
来源：http://hxs.yj20258888.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fou.jinqigfzy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vqp.316326.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lyn.gaohongyu789.top

Ruby: # 无泛型
来源：http://pff.haohaochexian.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bcq.hcnkem.com

[C15] 解构 / 展开参数
来源：http://jdw.cqqwz.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dcx.cdnleiting.top

PHP:  [$a, $b] = $pair;
来源：http://jmi.yj202588.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dwn.tanke756.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ieq.chenzaomai.com

Java: // 无解构
来源：http://hre.nanxinkj.top

Go:   // 无解构
来源：http://iyr.yvedp.cn

Ruby: a, b = pair
来源：http://lui.tanke756.top

C#:   var (a, b) = pair;
来源：http://vjj.bjfxy.top

[C16] 函数 / 方法重载
来源：http://psn.shuidangran.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xqm.jlsjyb.cn

PHP:  // 无重载
来源：http://qbp.zhixingplan.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://cmx.havefunace.top

TS:   // 用联合类型或重载签名声明
来源：http://exk.ppjwa.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://buj.vqdsnc.cn

Go:   // 无重载：用不同函数名
来源：http://dsp.gzhubu.top

Ruby: # 无重载：靠动态参数
来源：http://gup.zdbjq.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://sdt.jinyuanbaomall.cn

================================================================================
来源：http://dan.hnxiangtu.top

D. 数组 / 列表 / 集合
来源：http://eam.svipenyu.cn

================================================================================
来源：http://tjo.snrcjt.cn

[D01] 创建数组 / 列表
来源：http://cpp.dianchejie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fzy.shzxlz.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qyn.ehwqpu.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vwc.cqqwz.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://crz.sjlbkw.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://doc.hywenlv.cn

Go:   arr := []int{1, 2, 3}
来源：http://lfv.mhx1999.top

Ruby: arr = [1, 2, 3]
来源：http://swb.tanke756.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ocf.jqgufenzy.top

[D02] 追加元素到末尾
来源：http://brn.shanyushiyangtech.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wag.redwolf501.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ckz.cheryme.top

JS:   arr.push(4);
来源：http://lyn.yongpay.top

TS:   arr.push(4);
来源：http://xov.jyoumei.cn

Java: list.add(4);
来源：http://cfb.tarul.cn

Go:   arr = append(arr, 4)
来源：http://rsw.tianlin.xyz

Ruby: arr << 4; arr.push(5)
来源：http://zcl.yangfankeji.com

C#:   list.Add(4);
来源：http://twp.tian-w.cn

[D03] 在指定位置插入元素
来源：http://tjd.vehdjk.com

Py:   arr.insert(0, 0)
来源：http://wfa.ppjwa.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://oef.yuxming.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wof.zycfv.cn

TS:   arr.splice(0, 0, 0);
来源：http://pxc.zhongyouzk.top

Java: list.add(0, 0);
来源：http://dvf.fktsv.cn

Go:   arr = append([]int{0}, arr...)
来源：http://gho.jlsjyb.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zqs.zhaomingkeji.xyz

C#:   list.Insert(0, 0);
来源：http://pta.vehdjk.com

[D04] 删除元素
来源：http://zhs.jinghuilouyu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tff.hywenlv.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vkx.xziqi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://phm.yfazqb.com

TS:   arr.splice(0, 1);
来源：http://jsv.yuanzhike.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://thp.jiagoushi.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ekr.ydzc1.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mnu.52xcode.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jdh.ywan-chungtsiang.top

[D05] 访问与修改元素
来源：http://fle.hnxiangtu.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bjy.shanyushiyangkeji.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gsb.yonumen.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://eqz.chenjidiqi.icu

TS:   arr[0]; arr.at(-1);
来源：http://jxl.uphjek.com

Java: list.get(0); list.set(0, 9);
来源：http://rsl.shanyushiyangtech.top

Go:   arr[0]; arr[0] = 9
来源：http://nmr.52xcode.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://avn.iojbl.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ryr.guannengcc.top

[D06] 数组长度
来源：http://gfd.tianlin.xyz

Py:   len(arr)
来源：http://kfw.yj20258.top

PHP:  count($arr);
来源：http://gvk.svipenyu.cn

JS:   arr.length
来源：http://rha.iojbl.cn

TS:   arr.length
来源：http://srf.shuidangran.top

Java: list.size();
来源：http://lyl.jyoumei.cn

Go:   len(arr)
来源：http://hpc.shangyingyoupin.top

Ruby: arr.length; arr.size
来源：http://zfx.tanke756.top

C#:   list.Count;
来源：http://imk.fengsongda.top

[D07] 切片 / 取子数组
来源：http://zgf.ppjwa.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fsf.guannengcc.top

PHP:  array_slice($arr, 1, 3);
来源：http://ont.ehwqpu.com

JS:   arr.slice(1, 4);
来源：http://xsw.quarkkingdee.top

TS:   arr.slice(1, 4);
来源：http://rgj.epnwcf.com

Java: list.subList(1, 4);
来源：http://jjm.xylfe.cn

Go:   arr[1:4]
来源：http://hqw.zdbjq.cn

Ruby: arr[1, 3]
来源：http://zgl.guannengcc.top

C#:   list.GetRange(1, 3);
来源：http://jnf.epnwcf.com

[D08] 合并两个数组
来源：http://uxt.chenjidiqi.icu

Py:   a + b;  a.extend(b)
来源：http://puk.daria6918.cn

PHP:  array_merge($a, $b);
来源：http://ltk.chenjidiqi.icu

JS:   [...a, ...b];  a.concat(b);
来源：http://dqk.haohaochexian.top

TS:   [...a, ...b];
来源：http://cra.iojbl.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kmk.cdnleiting.top

Go:   append(a, b...)
来源：http://vpp.hongshengwenyu.top

Ruby: a + b;  a.concat(b)
来源：http://vss.hfpthk.cn

C#:   a.Concat(b).ToList()
来源：http://nan.xylfe.cn

[D09] 排序（升序）
来源：http://ymi.shanyushiyangtech.top

Py:   sorted(arr);  arr.sort()
来源：http://nok.xylfe.cn

PHP:  sort($arr);
来源：http://oty.bbcook.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://csj.hywenlv.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://bvy.yanxiufei.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hvr.xuetiantiany.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://krk.vehdjk.com

Ruby: arr.sort
来源：http://ojg.xziqi.cn

C#:   list.Sort();
来源：http://gll.guannengcc.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://xpc.zycfv.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rya.zhaomingkeji.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jrh.hywenlv.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://aqa.daria6918.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://quw.kuanghao11.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://swt.sjlbkw.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ynh.jiagoushi.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zen.hfpthk.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zqu.feifeiyinyue.top

[D11] 反转数组
来源：http://jec.guowangkeji.top

Py:   arr[::-1];  arr.reverse()
来源：http://nbw.316326.xyz

PHP:  array_reverse($arr);
来源：http://stw.dashuyun.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mwk.yj20258888.top

TS:   [...arr].reverse();
来源：http://nrm.daxiang520.top

Java: Collections.reverse(list);
来源：http://trq.jinqigfzy.top

Go:   slices.Reverse(arr)
来源：http://ggu.daxiang520.top

Ruby: arr.reverse
来源：http://kwt.jianghu66.top

C#:   list.Reverse();
来源：http://iht.aibaodan.cn

[D12] 查找元素下标
来源：http://gde.xuanzx.com

Py:   arr.index(x);  x in arr
来源：http://fmr.yuxming.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fhe.chenlongwang.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oip.tanke756.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://euz.yj20258888.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dbf.jiagoushi.top

Go:   slices.Index(arr, x)
来源：http://kff.cqqwz.cn

Ruby: arr.index(x)
来源：http://lww.iojbl.cn

C#:   list.IndexOf(x);
来源：http://vhm.zhaomingkeji.xyz

[D13] 过滤（保留满足条件的）
来源：http://zcc.yuanzhike.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hwa.zhongyouzk.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wtq.52xcode.cn

JS:   arr.filter(x => x > 3)
来源：http://ghq.epnwcf.com

TS:   arr.filter(x => x > 3)
来源：http://kiq.mhx1999.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wuh.ybcxt.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kuf.xinyue.icu

Ruby: arr.select { |x| x > 3 }
来源：http://acr.ydjk.org.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zky.fengsongda.top

[D14] 映射转换（每个元素变形）
来源：http://ppi.yueranfly.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yde.hysaishi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://owd.ivvv.top

JS:   arr.map(x => x * 2)
来源：http://uzy.epnwcf.com

TS:   arr.map(x => x * 2)
来源：http://tze.pycfn.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://jou.nanxinkj.top

Go:   // 手写循环
来源：http://qrr.bbcook.cn

Ruby: arr.map { |x| x * 2 }
来源：http://toq.ehwqpu.com

C#:   list.Select(x => x * 2).ToList()
来源：http://kyr.meibo888.top

[D15] 去重
来源：http://dtn.shanyushiyangtech.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jbf.yuxming.cn

PHP:  array_unique($arr);
来源：http://tpm.sweek.top

JS:   [...new Set(arr)]
来源：http://aag.gotoacloud.top

TS:   [...new Set(arr)]
来源：http://led.hongshengwenyu.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pch.jinghuilouyu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://cqy.yj20258888.top

Ruby: arr.uniq
来源：http://mww.shzxlz.cn

C#:   list.Distinct().ToList()
来源：http://oiy.nwbrower.top

[D16] 求和与平均值
来源：http://dxu.gaohongyu789.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lhg.hongshengwenyu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lri.iojbl.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hgz.jinqigfzy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sdm.sjlbkw.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ldg.hnxiangtu.top

Go:   // 手写循环累加
来源：http://pnz.52xcode.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cge.haohaochexian.top

C#:   list.Sum();  list.Average()
来源：http://xtr.gogol.net.cn

[D17] 最大值与最小值
来源：http://ctu.xuanzx.com

Py:   max(arr);  min(arr)
来源：http://rnw.feifeiyinyue.top

PHP:  max($arr);  min($arr);
来源：http://wai.jinqigufen.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sml.svipenyu.cn

TS:   Math.max(...arr);
来源：http://jem.zdbjq.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://png.tarul.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wne.zhongyouzk.top

Ruby: arr.max;  arr.min
来源：http://xbm.aibaodan.cn

C#:   list.Max();  list.Min()
来源：http://tgm.guannengcc.top

[D18] 扁平化嵌套数组
来源：http://gfi.yanxiufei.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://emy.ivvv.top

PHP:  array_merge(...$nested);
来源：http://fva.yj20258.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://unm.zhijiandao.cn

TS:   nested.flat();
来源：http://sam.ehwqpu.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hrc.mhx1999.top

Go:   // 手写双层循环
来源：http://eas.xuetiantiany.cn

Ruby: nested.flatten
来源：http://iir.tarul.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://umv.guannengcc.top

[D19] 按字段分组
来源：http://qyg.xziqi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zsp.birdmap.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mvf.iojbl.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qot.meibo888.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://wcc.yj20258888.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qls.c1oappe.top

Go:   // 手写 map[string][]T
来源：http://hiu.sufxvd.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://amf.sxryk.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://abp.sysykeji.top

[D20] 统计每个元素出现次数
来源：http://cvs.ywan-chungtsiang.top

Py:   Counter(arr)
来源：http://eii.birdmap.top

PHP:  array_count_values($arr);
来源：http://dpn.yangfankeji.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fzl.yuanzhike.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ylb.chenzaomai.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xcq.jianghu66.top

Go:   // 手写 map[T]int
来源：http://pgz.havefunace.top

Ruby: arr.tally
来源：http://ldc.xingfuxueyuan.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ibv.epnwcf.com

[D21] 判断是否包含某元素
来源：http://wuj.tanke756.top

Py:   x in arr
来源：http://hfq.birdmap.top

PHP:  in_array($x, $arr, true);
来源：http://gsm.vehdjk.com

JS:   arr.includes(x)
来源：http://aae.yuanzhike.top

TS:   arr.includes(x)
来源：http://zpg.ivvv.top

Java: list.contains(x)
来源：http://bex.yanxiufei.cn

Go:   slices.Contains(arr, x)
来源：http://byq.havefunace.top

Ruby: arr.include?(x)
来源：http://gzn.jinqigfzy.top

C#:   list.Contains(x)
来源：http://yak.mhx1999.top

[D22] 复制数组（避免共享引用）
来源：http://hca.yj20258.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://unk.gaohongyu789.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ioy.wangshuangyany.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ocx.svipenyu.cn

TS:   [...arr];
来源：http://yrk.yanxiufei.cn

Java: new ArrayList<>(list);
来源：http://lpf.aizwys.cn

Go:   copied := append([]int(nil), arr...)
来源：http://myq.sjlbkw.cn

Ruby: arr.dup;  arr.clone
来源：http://hiu.sufxvd.cn

C#:   new List<int>(list);
来源：http://ruc.zycfv.cn

[D23] reduce 累积计算
来源：http://kdn.nanxuanxn.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://koe.birdmap.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ptj.mhx1999.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://flu.hfpthk.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gwz.zhaomingkeji.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://oix.cheryme.top

Go:   // 手写循环
来源：http://mgd.yj202588.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://urp.sysykeji.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gdv.gaohongyu789.top

[D24] 字典 / Map 基本操作
来源：http://mbc.sufxvd.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://unv.jqgfzy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ege.zhoulong.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xcz.316326.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fls.nanxinkj.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rhb.shuidangran.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nph.c1oappe.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://oze.xuanzx.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://udl.wangshuangyany.cn

[D25] Set 集合去重与交并差
来源：http://mew.xziqi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jke.tarul.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tjh.havefunace.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wua.ydjk.org.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vop.gogol.net.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://way.haohaochexian.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zgl.pycfn.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rrb.smart0.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xnu.aizwys.cn

[D26] 数组转字符串
来源：http://gcz.jiagoushi.top

Py:   ", ".join(map(str, arr))
来源：http://pdq.aibaodan.cn

PHP:  implode(", ", $arr);
来源：http://rrm.yuxming.cn

JS:   arr.join(", ")
来源：http://eqh.sxryk.cn

TS:   arr.join(", ")
来源：http://wau.nanxinkj.top

Java: String.join(", ", list)
来源：http://edd.jinyuanbaomall.cn

Go:   strings.Join(strs, ", ")
来源：http://chc.jinyuanbaomall.cn

Ruby: arr.join(", ")
来源：http://nnd.zhaomingkeji.xyz

C#:   string.Join(", ", list)
来源：http://xki.gaohongyu789.top

================================================================================
来源：http://igb.yj202588.top

E. 字符串处理
来源：http://zgl.jqgufenzy.top

================================================================================
来源：http://xxp.havefunace.top

[E01] 拼接字符串
来源：http://cig.kuanghao11.cn


<!-- 参考信息 -->
代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://chi.redwolf501.top

C#:   using System.Text;
来源：http://pyo.316326.xyz

[C12] 立即执行函数 IIFE
来源：http://fkt.c1oappe.top

Py:   (lambda: print("run"))()
来源：http://uux.gotoacloud.top

PHP:  (function () { echo "run"; })();
来源：http://wqy.fengsongda.top

JS:   (() => { console.log("run"); })();
来源：http://mza.xuanzx.com

TS:   (() => { console.log("run"); })();
来源：http://jde.haohaochexian.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dvs.hywenlv.cn

Go:   func() { fmt.Println("run") }()
来源：http://zje.mhx1999.top

Ruby: -> { puts "run" }.call
来源：http://pni.zhiwuduotai.top

C#:   // 无 IIFE：用静态构造函数
来源：http://vjb.316326.xyz

[C13] 类型声明 / 类型注解
来源：http://sqq.xuanzx.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ieo.sufxvd.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ovy.fehbvm.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xih.gzhubu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mgf.quarkkingdee.top

Java: int add(int a, int b) { return a + b; }
来源：http://kiz.yonumen.top

Go:   func add(a, b int) int
来源：http://qle.wangshuangyany.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vle.jiagoushi.top

C#:   int Add(int a, int b) => a + b;
来源：http://att.ppjwa.cn

[C14] 泛型函数
来源：http://whi.pengpengdd.cyou

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fes.ydzc1.top

PHP:  // 无泛型
来源：http://kve.tarul.cn

JS:   // 无泛型
来源：http://wmv.yj202588.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rzo.mhx1999.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kwv.ivvv.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bwj.bbcook.cn

Ruby: # 无泛型
来源：http://ntd.cdnleiting.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://stu.ydzc1.top

[C15] 解构 / 展开参数
来源：http://miq.yonumen.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nbj.mhx1999.top

PHP:  [$a, $b] = $pair;
来源：http://ize.haohaochexian.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fyb.hammf.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://taa.yuanzhike.top

Java: // 无解构
来源：http://ark.xuanzx.com

Go:   // 无解构
来源：http://kmw.0kj1m.cn

Ruby: a, b = pair
来源：http://vxh.xziqi.cn

C#:   var (a, b) = pair;
来源：http://pvo.guowangkeji.top

[C16] 函数 / 方法重载
来源：http://vbe.zhengqikj.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ceo.feifeiyinyue.top

PHP:  // 无重载
来源：http://vzh.bjfxy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://iyx.daxiang520.top

TS:   // 用联合类型或重载签名声明
来源：http://mnr.meibo888.top

Java: void f(int a) {}  void f(String a) {}
来源：http://kcr.pycfn.com

Go:   // 无重载：用不同函数名
来源：http://ega.jqgfzy.top

Ruby: # 无重载：靠动态参数
来源：http://zmt.uphjek.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://umu.snrcjt.cn

================================================================================
来源：http://vqx.guannengcc.top

D. 数组 / 列表 / 集合
来源：http://pma.dashuyun.cn

================================================================================
来源：http://uks.yfazqb.com

[D01] 创建数组 / 列表
来源：http://ycr.fktsv.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://otg.gogol.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hfn.tian-w.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vsa.feifeiyinyue.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ijw.xylfe.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gxf.cucudq.cn

Go:   arr := []int{1, 2, 3}
来源：http://gjs.aibaodan.cn

Ruby: arr = [1, 2, 3]
来源：http://pxf.feifeiyinyue.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://eto.hnxiangtu.top

[D02] 追加元素到末尾
来源：http://foq.hesvh.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://osv.vehdjk.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bsk.jqgufenzy.top

JS:   arr.push(4);
来源：http://sxz.nwbrower.top

TS:   arr.push(4);
来源：http://lvr.ctjpmb.com

Java: list.add(4);
来源：http://aeq.yueranfly.top

Go:   arr = append(arr, 4)
来源：http://ddz.chenzaomai.com

Ruby: arr << 4; arr.push(5)
来源：http://dbj.yueranfly.top

C#:   list.Add(4);
来源：http://uzc.hesvh.cn

[D03] 在指定位置插入元素
来源：http://oio.yj202588.top

Py:   arr.insert(0, 0)
来源：http://aqf.316326.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ula.hfpthk.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ibi.jlsjyb.cn

TS:   arr.splice(0, 0, 0);
来源：http://bmk.epnwcf.com

Java: list.add(0, 0);
来源：http://bjp.xuanzx.com

Go:   arr = append([]int{0}, arr...)
来源：http://ozj.jianghu66.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tyx.iojbl.cn

C#:   list.Insert(0, 0);
来源：http://joh.shzxlz.cn

[D04] 删除元素
来源：http://isj.hesvh.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cwl.chenlongwang.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gex.uphjek.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nbu.wangdashe.top

TS:   arr.splice(0, 1);
来源：http://hyt.zhixingplan.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rjs.ydjk.org.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://poe.sweek.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jsz.xuetiantiany.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nzy.feifeiyinyue.top

[D05] 访问与修改元素
来源：http://lje.ivvv.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://trz.svipenyu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://oje.sysykeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wnh.vehdjk.com

TS:   arr[0]; arr.at(-1);
来源：http://suq.jqgufenzy.top

Java: list.get(0); list.set(0, 9);
来源：http://kze.ydjk.org.cn

Go:   arr[0]; arr[0] = 9
来源：http://xiv.jinqigfzy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uzq.jianghu66.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mgs.sysykeji.top

[D06] 数组长度
来源：http://nao.zhijiandao.cn

Py:   len(arr)
来源：http://lji.epnwcf.com

PHP:  count($arr);
来源：http://svb.smart0.xyz

JS:   arr.length
来源：http://xhv.jiagoushi.top

TS:   arr.length
来源：http://dbw.gzhubu.top

Java: list.size();
来源：http://ufc.tian-w.cn

Go:   len(arr)
来源：http://gei.yanxiufei.cn

Ruby: arr.length; arr.size
来源：http://jin.jinqigfzy.top

C#:   list.Count;
来源：http://oyl.andypj.xyz

[D07] 切片 / 取子数组
来源：http://fes.cheryme.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mjd.shuidangran.top

PHP:  array_slice($arr, 1, 3);
来源：http://kjz.hfpthk.cn

JS:   arr.slice(1, 4);
来源：http://ffa.kuanghao11.cn

TS:   arr.slice(1, 4);
来源：http://rou.zhaomingkeji.xyz

Java: list.subList(1, 4);
来源：http://igm.wangdashe.top

Go:   arr[1:4]
来源：http://wmw.gaohongyu789.top

Ruby: arr[1, 3]
来源：http://gqb.yanxiufei.cn

C#:   list.GetRange(1, 3);
来源：http://mge.hfpthk.cn

[D08] 合并两个数组
来源：http://gbt.nanxuanxn.top

Py:   a + b;  a.extend(b)
来源：http://zfu.ctjpmb.com

PHP:  array_merge($a, $b);
来源：http://nbp.ydjk.org.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://uib.hcnkem.com

TS:   [...a, ...b];
来源：http://ccc.dashuyun.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://elw.zhoulong.xyz

Go:   append(a, b...)
来源：http://kkh.tian-w.cn

Ruby: a + b;  a.concat(b)
来源：http://kxp.dianchejie.cn

C#:   a.Concat(b).ToList()
来源：http://fft.yfazqb.com

[D09] 排序（升序）
来源：http://spu.gogol.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://djy.yvedp.cn

PHP:  sort($arr);
来源：http://gav.hcnkem.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://drw.iojbl.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xoa.gotoacloud.top

Java: Collections.sort(list);  list.sort(null);
来源：http://cas.smart0.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wau.ctjpmb.com

Ruby: arr.sort
来源：http://bhq.chenzaomai.com

C#:   list.Sort();
来源：http://ocl.yueranfly.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://fxn.sweek.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dwx.iojbl.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dbo.guowangkeji.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hmk.hnxiangtu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://uir.vqdsnc.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yxw.gaohongyu789.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wwy.epnwcf.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wgb.bjfxy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bzq.jqgufenzy.top

[D11] 反转数组
来源：http://qjh.bjfxy.top

Py:   arr[::-1];  arr.reverse()
来源：http://mze.bjfxy.top

PHP:  array_reverse($arr);
来源：http://nul.wangshuangyany.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qar.yonumen.top

TS:   [...arr].reverse();
来源：http://iud.hfpthk.cn

Java: Collections.reverse(list);
来源：http://spr.chenjidiqi.icu

Go:   slices.Reverse(arr)
来源：http://nyg.xuetiantiany.cn

Ruby: arr.reverse
来源：http://max.zhongyouzk.top

C#:   list.Reverse();
来源：http://ipv.yj20258888.top

[D12] 查找元素下标
来源：http://xqa.0kj1m.cn

Py:   arr.index(x);  x in arr
来源：http://iwp.epnwcf.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zfl.dashuyun.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qhr.xuetiantiany.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sko.fktsv.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zwm.fehbvm.com

Go:   slices.Index(arr, x)
来源：http://brh.nwbrower.top

Ruby: arr.index(x)
来源：http://ulj.cucudq.cn

C#:   list.IndexOf(x);
来源：http://cxk.zhoulong.xyz

[D13] 过滤（保留满足条件的）
来源：http://pzr.ivvv.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://two.snrcjt.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gwz.yvedp.cn

JS:   arr.filter(x => x > 3)
来源：http://xhb.shangyingyoupin.top

TS:   arr.filter(x => x > 3)
来源：http://rpg.uphjek.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zzo.hcnkem.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qbr.daria6918.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qgf.ywan-chungtsiang.top

C#:   list.Where(x => x > 3).ToList()
来源：http://wli.ppjwa.cn

[D14] 映射转换（每个元素变形）
来源：http://hbu.cqqwz.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fux.sxryk.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ksx.epnwcf.com

JS:   arr.map(x => x * 2)
来源：http://crm.ybcxt.top

TS:   arr.map(x => x * 2)
来源：http://wmz.aibaodan.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sra.yangfankeji.com

Go:   // 手写循环
来源：http://rhs.cucudq.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jkw.uphjek.com

C#:   list.Select(x => x * 2).ToList()
来源：http://zrm.pycfn.com

[D15] 去重
来源：http://mht.jlsjyb.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qog.hesvh.cn

PHP:  array_unique($arr);
来源：http://vbs.fzhhl.top

JS:   [...new Set(arr)]
来源：http://thd.dianchejie.cn

TS:   [...new Set(arr)]
来源：http://edk.yj20258.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://plm.yuxming.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hou.yvedp.cn

Ruby: arr.uniq
来源：http://sah.daxiang520.top

C#:   list.Distinct().ToList()
来源：http://fut.zhoulong.xyz

[D16] 求和与平均值
来源：http://fsv.zycfv.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://joy.aizwys.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://myo.yj20258.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://eeb.hammf.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ptv.ybcxt.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hkz.shanyushiyangtech.top

Go:   // 手写循环累加
来源：http://fhk.zhoulong.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rtd.jqgfzy.top

C#:   list.Sum();  list.Average()
来源：http://xay.fengsongda.top

[D17] 最大值与最小值
来源：http://gxg.pycfn.com

Py:   max(arr);  min(arr)
来源：http://aor.shanyushiyangtech.top

PHP:  max($arr);  min($arr);
来源：http://gen.jqgufenzy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ndh.hcnkem.com

TS:   Math.max(...arr);
来源：http://czw.yfazqb.com

Java: Collections.max(list);  Collections.min(list);
来源：http://ioi.aizwys.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hrz.yj202588.top

Ruby: arr.max;  arr.min
来源：http://dzl.jinqigfzy.top

C#:   list.Max();  list.Min()
来源：http://pii.ctjpmb.com

[D18] 扁平化嵌套数组
来源：http://tke.epnwcf.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cfq.xinyue.icu

PHP:  array_merge(...$nested);
来源：http://kml.yongpay.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hws.yanxiufei.cn

TS:   nested.flat();
来源：http://ujk.hongshengwenyu.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kcq.gzhubu.top

Go:   // 手写双层循环
来源：http://yrj.cqqwz.cn

Ruby: nested.flatten
来源：http://uvz.daxiang520.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://wao.shangyingyoupin.top

[D19] 按字段分组
来源：http://lha.vehdjk.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://uab.uphjek.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mpu.sufxvd.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uax.52xcode.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ozu.zhengqikj.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://trr.yongpay.top

Go:   // 手写 map[string][]T
来源：http://bof.jianghu66.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://tiz.vqdsnc.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kfx.hnxiangtu.top

[D20] 统计每个元素出现次数
来源：http://sia.aizwys.cn

Py:   Counter(arr)
来源：http://ifz.jinqigufen.top

PHP:  array_count_values($arr);
来源：http://rqz.shangyingyoupin.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mqa.zhijiandao.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hjs.yangfankeji.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mmw.zhixingplan.top

Go:   // 手写 map[T]int
来源：http://gkh.xylfe.cn

Ruby: arr.tally
来源：http://kgs.fengsongda.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://uii.zhixingplan.top

[D21] 判断是否包含某元素
来源：http://cdl.jianghu66.top

Py:   x in arr
来源：http://epe.yueranfly.top

PHP:  in_array($x, $arr, true);
来源：http://qhm.jinghuilouyu.cn

JS:   arr.includes(x)
来源：http://dbs.sxryk.cn

TS:   arr.includes(x)
来源：http://hdk.sjlbkw.cn

Java: list.contains(x)
来源：http://blx.vehdjk.com

Go:   slices.Contains(arr, x)
来源：http://adt.xylfe.cn

Ruby: arr.include?(x)
来源：http://fcj.yuxming.cn

C#:   list.Contains(x)
来源：http://mxc.ydzc1.top

[D22] 复制数组（避免共享引用）
来源：http://jbm.daxiang520.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ydg.chenlongwang.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bow.chenlongwang.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nuf.meibo888.top

TS:   [...arr];
来源：http://crp.yj202588.top

Java: new ArrayList<>(list);
来源：http://mrn.jqgfzy.top

Go:   copied := append([]int(nil), arr...)
来源：http://sga.fanxiaobao.xyz

Ruby: arr.dup;  arr.clone
来源：http://udq.shanyushiyangkeji.top

C#:   new List<int>(list);
来源：http://jpg.52xcode.cn

[D23] reduce 累积计算
来源：http://iqc.zhengqikj.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xsz.gaohongyu789.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ero.yuxming.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rsv.daria6918.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://agu.zhijiandao.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fyn.pycfn.com

Go:   // 手写循环
来源：http://xnz.sjlbkw.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ozi.xziqi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hhw.shangyingyoupin.top

[D24] 字典 / Map 基本操作
来源：http://hxi.zhaomingkeji.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uzx.ywan-chungtsiang.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fbv.pengpengdd.cyou

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://whe.aibaodan.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kme.316326.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://udx.jiagoushi.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://stj.vqdsnc.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pai.yangfankeji.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qnb.havefunace.top

[D25] Set 集合去重与交并差
来源：http://yox.zycfv.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mfr.bbcook.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rfd.sweek.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ytc.jianghu66.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ebj.zdqjudy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://juv.zhoulong.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nys.jinqigfzy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://deb.shuidangran.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fkw.sweek.top

[D26] 数组转字符串
来源：http://rii.shanyushiyangtech.top

Py:   ", ".join(map(str, arr))
来源：http://hri.xingfuxueyuan.xyz

PHP:  implode(", ", $arr);
来源：http://biq.ctjpmb.com

JS:   arr.join(", ")
来源：http://kqy.shanyushiyangkeji.top

TS:   arr.join(", ")
来源：http://ehx.cdnleiting.top

Java: String.join(", ", list)
来源：http://lml.zhaomingkeji.xyz

Go:   strings.Join(strs, ", ")
来源：http://pcz.zycfv.cn

Ruby: arr.join(", ")
来源：http://bna.guowangkeji.top

C#:   string.Join(", ", list)
来源：http://mip.vehdjk.com

================================================================================
来源：http://ndh.daxiang520.top

E. 字符串处理
来源：http://ahl.zdqjudy.top

================================================================================
来源：http://ptf.feifeiyinyue.top

[E01] 拼接字符串
来源：http://ahm.jqgfzy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://akz.shuidangran.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://unt.daria6918.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gyn.feifeiyinyue.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yew.0kj1m.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xhb.jiagoushi.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qpm.jqgfzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wbv.fengsongda.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://urt.fanxiaobao.xyz

[E02] 重复字符串
来源：http://tbu.yj202588.top

Py:   "ab" * 3
来源：http://cpq.yangfankeji.com

PHP:  str_repeat("ab", 3);
来源：http://zfw.svipenyu.cn

JS:   "ab".repeat(3)
来源：http://gpm.yangfankeji.com


<!-- 参考信息 -->
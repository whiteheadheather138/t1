代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://pgt.cheryme.top

Go:   func add(a, b int) int
来源：http://oew.316326.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jya.shangyingyoupin.top

C#:   int Add(int a, int b) => a + b;
来源：http://lac.hywenlv.cn

[C14] 泛型函数
来源：http://syp.cucudq.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jxn.xingfuxueyuan.xyz

PHP:  // 无泛型
来源：http://drc.xziqi.cn

JS:   // 无泛型
来源：http://fup.fengsongda.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://izg.yj202588.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rye.zycfv.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bow.chenlongwang.top

Ruby: # 无泛型
来源：http://etz.gogol.net.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hnk.hammf.cn

[C15] 解构 / 展开参数
来源：http://ypp.yj20258888.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wvo.hfpthk.cn

PHP:  [$a, $b] = $pair;
来源：http://qmv.quarkkingdee.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wpv.xuetiantiany.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hoo.xylfe.cn

Java: // 无解构
来源：http://bvs.zhongyouzk.top

Go:   // 无解构
来源：http://rcs.cdnleiting.top

Ruby: a, b = pair
来源：http://gwv.ivvv.top

C#:   var (a, b) = pair;
来源：http://htm.cheryme.top

[C16] 函数 / 方法重载
来源：http://qov.hammf.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jdg.xingfuxueyuan.xyz

PHP:  // 无重载
来源：http://zdd.chenjidiqi.icu

JS:   // 无重载：靠 arguments.length 分支
来源：http://juh.pengpengdd.cyou

TS:   // 用联合类型或重载签名声明
来源：http://eoz.zdbjq.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://bkw.yvedp.cn

Go:   // 无重载：用不同函数名
来源：http://dft.cucudq.cn

Ruby: # 无重载：靠动态参数
来源：http://cgq.yvedp.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://avs.dashuyun.cn

================================================================================
来源：http://cko.sweek.top

D. 数组 / 列表 / 集合
来源：http://yim.shzxlz.cn

================================================================================
来源：http://rog.sufxvd.cn

[D01] 创建数组 / 列表
来源：http://ctl.aibaodan.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mmu.sufxvd.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pck.shangyingyoupin.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://csa.ctjpmb.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://tkf.shangyingyoupin.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vyv.c1oappe.top

Go:   arr := []int{1, 2, 3}
来源：http://qzn.yonumen.top

Ruby: arr = [1, 2, 3]
来源：http://xdn.nanxinkj.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zsb.hcnkem.com

[D02] 追加元素到末尾
来源：http://tbe.hammf.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mle.c1oappe.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fxp.316326.xyz

JS:   arr.push(4);
来源：http://rmt.jinqigfzy.top

TS:   arr.push(4);
来源：http://ezy.smart0.xyz

Java: list.add(4);
来源：http://lww.hysaishi.cn

Go:   arr = append(arr, 4)
来源：http://lhe.jinghuilouyu.cn

Ruby: arr << 4; arr.push(5)
来源：http://uyt.c1oappe.top

C#:   list.Add(4);
来源：http://qhu.ybcxt.top

[D03] 在指定位置插入元素
来源：http://ukr.fktsv.cn

Py:   arr.insert(0, 0)
来源：http://mvs.jqgufenzy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ftf.aibaodan.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ofc.shuidangran.top

TS:   arr.splice(0, 0, 0);
来源：http://ifs.guowangkeji.top

Java: list.add(0, 0);
来源：http://spa.hnqzz.top

Go:   arr = append([]int{0}, arr...)
来源：http://gny.havefunace.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yey.gotoacloud.top

C#:   list.Insert(0, 0);
来源：http://mpi.vehdjk.com

[D04] 删除元素
来源：http://zrq.sjlbkw.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gtf.xuanzx.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ceb.316326.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fbd.hammf.cn

TS:   arr.splice(0, 1);
来源：http://beg.sysykeji.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yqj.nanxinkj.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://upq.yongpay.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ohk.wangshuangyany.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ufd.yvedp.cn

[D05] 访问与修改元素
来源：http://xlx.c1oappe.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pmy.mhx1999.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://oht.zhongyouzk.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zlq.cheryme.top

TS:   arr[0]; arr.at(-1);
来源：http://fch.jinghuilouyu.cn

Java: list.get(0); list.set(0, 9);
来源：http://bld.yj20258.top

Go:   arr[0]; arr[0] = 9
来源：http://yfk.cucudq.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cni.yj20258888.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bdw.smart0.xyz

[D06] 数组长度
来源：http://bbz.zdqjudy.top

Py:   len(arr)
来源：http://ajk.aibaodan.cn

PHP:  count($arr);
来源：http://xeq.ydjk.org.cn

JS:   arr.length
来源：http://mti.daria6918.cn

TS:   arr.length
来源：http://fdh.tanke756.top

Java: list.size();
来源：http://drp.dianchejie.cn

Go:   len(arr)
来源：http://exj.yvedp.cn

Ruby: arr.length; arr.size
来源：http://xfy.andypj.xyz

C#:   list.Count;
来源：http://bbb.ydjk.org.cn

[D07] 切片 / 取子数组
来源：http://gfo.zhengqikj.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fwq.ybcxt.top

PHP:  array_slice($arr, 1, 3);
来源：http://cqk.yj20258.top

JS:   arr.slice(1, 4);
来源：http://cqz.yangfankeji.com

TS:   arr.slice(1, 4);
来源：http://trc.yongpay.top

Java: list.subList(1, 4);
来源：http://gyk.pengpengdd.cyou

Go:   arr[1:4]
来源：http://swa.ivvv.top

Ruby: arr[1, 3]
来源：http://fkk.ydzc1.top

C#:   list.GetRange(1, 3);
来源：http://sfi.vqdsnc.cn

[D08] 合并两个数组
来源：http://zwh.svipenyu.cn

Py:   a + b;  a.extend(b)
来源：http://ozn.aizwys.cn

PHP:  array_merge($a, $b);
来源：http://kix.jyoumei.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://khk.ctjpmb.com

TS:   [...a, ...b];
来源：http://qon.uphjek.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://uaa.xuetiantiany.cn

Go:   append(a, b...)
来源：http://ieo.shuidangran.top

Ruby: a + b;  a.concat(b)
来源：http://xst.nanxuanxn.top

C#:   a.Concat(b).ToList()
来源：http://vyh.cqqwz.cn

[D09] 排序（升序）
来源：http://odn.sjlbkw.cn

Py:   sorted(arr);  arr.sort()
来源：http://ssx.haohaochexian.top

PHP:  sort($arr);
来源：http://mit.yvedp.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bgo.fzhhl.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://zpm.gaohongyu789.top

Java: Collections.sort(list);  list.sort(null);
来源：http://kya.guowangkeji.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qxe.jiagoushi.top

Ruby: arr.sort
来源：http://omo.kuanghao11.cn

C#:   list.Sort();
来源：http://fpk.xinyue.icu

[D10] 自定义排序（按字段 / 多条件）
来源：http://tia.hnqzz.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://iju.daxiang520.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ldy.jianghu66.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lag.shangyingyoupin.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wrd.zhoulong.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qjw.guowangkeji.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gpa.uphjek.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ujk.hfpthk.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zti.snrcjt.cn

[D11] 反转数组
来源：http://dok.zhengqikj.top

Py:   arr[::-1];  arr.reverse()
来源：http://tsx.zhengqikj.top

PHP:  array_reverse($arr);
来源：http://rbu.dianchejie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://uwe.yj202588.top

TS:   [...arr].reverse();
来源：http://vxh.gotoacloud.top

Java: Collections.reverse(list);
来源：http://nyb.shangyingyoupin.top

Go:   slices.Reverse(arr)
来源：http://exz.jianghu66.top

Ruby: arr.reverse
来源：http://jit.nanxinkj.top

C#:   list.Reverse();
来源：http://uki.yvedp.cn

[D12] 查找元素下标
来源：http://byg.epnwcf.com

Py:   arr.index(x);  x in arr
来源：http://eyl.0kj1m.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uzt.feifeiyinyue.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zoz.guannengcc.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ckc.yuanzhike.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://whg.hysaishi.cn

Go:   slices.Index(arr, x)
来源：http://lwe.jqgfzy.top

Ruby: arr.index(x)
来源：http://aov.xuanzx.com

C#:   list.IndexOf(x);
来源：http://bhv.cheryme.top

[D13] 过滤（保留满足条件的）
来源：http://csy.pycfn.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://box.epnwcf.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wet.hfpthk.cn

JS:   arr.filter(x => x > 3)
来源：http://sdw.svipenyu.cn

TS:   arr.filter(x => x > 3)
来源：http://tiu.gaohongyu789.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cea.mhx1999.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vlt.zhongyouzk.top

Ruby: arr.select { |x| x > 3 }
来源：http://fmp.guannengcc.top

C#:   list.Where(x => x > 3).ToList()
来源：http://wow.jinqigfzy.top

[D14] 映射转换（每个元素变形）
来源：http://uyx.xuetiantiany.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hso.fktsv.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nor.hysaishi.cn

JS:   arr.map(x => x * 2)
来源：http://rxg.kuanghao11.cn

TS:   arr.map(x => x * 2)
来源：http://jaa.havefunace.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://yhj.feifeiyinyue.top

Go:   // 手写循环
来源：http://wkk.zhaomingkeji.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://kaf.zhongyouzk.top

C#:   list.Select(x => x * 2).ToList()
来源：http://qoi.cqqwz.cn

[D15] 去重
来源：http://fye.xuanzx.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kth.ivvv.top

PHP:  array_unique($arr);
来源：http://kbp.gzhubu.top

JS:   [...new Set(arr)]
来源：http://hkg.pengpengdd.cyou

TS:   [...new Set(arr)]
来源：http://ohs.nanxuanxn.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://abn.shanyushiyangtech.top

Go:   // 用 map[T]struct{} 手写
来源：http://wsr.dashuyun.cn

Ruby: arr.uniq
来源：http://snx.cdnleiting.top

C#:   list.Distinct().ToList()
来源：http://tmc.smart0.xyz

[D16] 求和与平均值
来源：http://bby.vqdsnc.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://psu.shanyushiyangkeji.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://utv.guannengcc.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://agy.c1oappe.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ijc.ctjpmb.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dpt.hysaishi.cn

Go:   // 手写循环累加
来源：http://avt.yfazqb.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hqv.jinqigufen.top

C#:   list.Sum();  list.Average()
来源：http://ans.fengsongda.top

[D17] 最大值与最小值
来源：http://nbw.yfazqb.com

Py:   max(arr);  min(arr)
来源：http://amj.cheryme.top

PHP:  max($arr);  min($arr);
来源：http://kuq.cdnleiting.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tgq.hcnkem.com

TS:   Math.max(...arr);
来源：http://pvz.redwolf501.top

Java: Collections.max(list);  Collections.min(list);
来源：http://sly.fehbvm.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lkp.zdbjq.cn

Ruby: arr.max;  arr.min
来源：http://tts.chenlongwang.top

C#:   list.Max();  list.Min()
来源：http://nwd.sweek.top

[D18] 扁平化嵌套数组
来源：http://qto.fengsongda.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cpu.zhoulong.xyz

PHP:  array_merge(...$nested);
来源：http://lpm.nanxinkj.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://epx.pycfn.com

TS:   nested.flat();
来源：http://gse.gotoacloud.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://but.xziqi.cn

Go:   // 手写双层循环
来源：http://qxh.gotoacloud.top

Ruby: nested.flatten
来源：http://gac.hammf.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://jsz.dashuyun.cn

[D19] 按字段分组
来源：http://vlf.hongshengwenyu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hfw.yfazqb.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://beo.xingfuxueyuan.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tsi.sufxvd.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://kwq.hysaishi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xjj.yueranfly.top

Go:   // 手写 map[string][]T
来源：http://qen.jlsjyb.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://qqg.52xcode.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kbb.9152youxi.cn

[D20] 统计每个元素出现次数
来源：http://jac.xziqi.cn

Py:   Counter(arr)
来源：http://hvo.guowangkeji.top

PHP:  array_count_values($arr);
来源：http://rew.hnqzz.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://meg.52xcode.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vns.nanxinkj.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vww.hfpthk.cn

Go:   // 手写 map[T]int
来源：http://gxm.nwbrower.top

Ruby: arr.tally
来源：http://bnh.hnxiangtu.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://iyv.chenjidiqi.icu

[D21] 判断是否包含某元素
来源：http://smb.zycfv.cn

Py:   x in arr
来源：http://fek.hongshengwenyu.top

PHP:  in_array($x, $arr, true);
来源：http://xvr.jinyuanbaomall.cn

JS:   arr.includes(x)
来源：http://zwx.tanke756.top

TS:   arr.includes(x)
来源：http://fxq.ppjwa.cn

Java: list.contains(x)
来源：http://vzl.shzxlz.cn

Go:   slices.Contains(arr, x)
来源：http://ati.xylfe.cn

Ruby: arr.include?(x)
来源：http://sdv.ybcxt.top

C#:   list.Contains(x)
来源：http://lvh.jinghuilouyu.cn

[D22] 复制数组（避免共享引用）
来源：http://kzb.hammf.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nkf.tarul.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pgt.ydzc1.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bpf.zdqjudy.top

TS:   [...arr];
来源：http://lqn.zhixingplan.top

Java: new ArrayList<>(list);
来源：http://lmx.ctjpmb.com

Go:   copied := append([]int(nil), arr...)
来源：http://vrg.hesvh.cn

Ruby: arr.dup;  arr.clone
来源：http://ars.316326.xyz

C#:   new List<int>(list);
来源：http://jur.xuetiantiany.cn

[D23] reduce 累积计算
来源：http://czk.fktsv.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nju.zhijiandao.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cao.jinghuilouyu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pog.gzhubu.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tmj.haohaochexian.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ktz.zhoulong.xyz

Go:   // 手写循环
来源：http://jdx.zhixingplan.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://aef.xziqi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://iyf.sufxvd.cn

[D24] 字典 / Map 基本操作
来源：http://tsv.andypj.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mgv.guannengcc.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gsj.tanke756.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pwv.shzxlz.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ohv.shanyushiyangkeji.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bpb.xylfe.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://azw.shzxlz.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vej.feifeiyinyue.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lmi.hesvh.cn

[D25] Set 集合去重与交并差
来源：http://yor.jinqigufen.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vep.zhixingplan.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ckx.cqqwz.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gdh.wangshuangyany.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cbw.haohaochexian.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fdx.snrcjt.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jyu.zhengqikj.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://otl.jinqigfzy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xbm.tian-w.cn

[D26] 数组转字符串
来源：http://wsb.yangfankeji.com

Py:   ", ".join(map(str, arr))
来源：http://qec.meibo888.top

PHP:  implode(", ", $arr);
来源：http://dgw.ivvv.top

JS:   arr.join(", ")
来源：http://pig.ywan-chungtsiang.top

TS:   arr.join(", ")
来源：http://olg.jyoumei.cn

Java: String.join(", ", list)
来源：http://hsl.ehwqpu.com

Go:   strings.Join(strs, ", ")
来源：http://pmd.shuidangran.top

Ruby: arr.join(", ")
来源：http://toq.hcnkem.com

C#:   string.Join(", ", list)
来源：http://prl.sjlbkw.cn

================================================================================
来源：http://qvp.nanxinkj.top

E. 字符串处理
来源：http://iqm.nanxuanxn.top

================================================================================
来源：http://rij.pengpengdd.cyou

[E01] 拼接字符串
来源：http://vus.jinghuilouyu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ukz.dianchejie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wsa.shzxlz.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zzr.shangyingyoupin.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kta.cheryme.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ahc.jinghuilouyu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ikp.hfpthk.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vfw.hywenlv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rec.hywenlv.cn

[E02] 重复字符串
来源：http://znl.gotoacloud.top

Py:   "ab" * 3
来源：http://ech.vqdsnc.cn

PHP:  str_repeat("ab", 3);
来源：http://wwo.316326.xyz

JS:   "ab".repeat(3)
来源：http://zsx.ctjpmb.com

TS:   "ab".repeat(3)
来源：http://whj.nanxuanxn.top

Java: "ab".repeat(3)
来源：http://gdn.nwbrower.top

Go:   strings.Repeat("ab", 3)
来源：http://lzq.xingfuxueyuan.xyz

Ruby: "ab" * 3
来源：http://cug.yuxming.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pib.xingfuxueyuan.xyz

[E03] 截取子串
来源：http://yvv.pengpengdd.cyou

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ibr.shanyushiyangtech.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tcz.pengpengdd.cyou

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://amm.mhx1999.top

TS:   s.slice(1, 4)
来源：http://nwq.ydjk.org.cn

Java: s.substring(1, 4)
来源：http://fyk.zhiwuduotai.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sjt.ppjwa.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jgj.yonumen.top

C#:   s.Substring(1, 3)
来源：http://xne.epnwcf.com

[E04] 查找子串位置
来源：http://uzv.shanyushiyangtech.top

Py:   s.find("x");  s.index("x")
来源：http://tdu.shanyushiyangkeji.top


<!-- 参考信息 -->
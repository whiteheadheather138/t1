代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fgy.ppjwa.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gsi.xingfuxueyuan.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cul.feifeiyinyue.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jvo.fanxiaobao.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://eqe.ywan-chungtsiang.top

Go:   func add(a, b int) int
来源：http://nwo.jinghuilouyu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rgd.xuetiantiany.cn

C#:   int Add(int a, int b) => a + b;
来源：http://sgj.jqgfzy.top

[C14] 泛型函数
来源：http://imu.cqqwz.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tyj.tanke756.top

PHP:  // 无泛型
来源：http://pqa.kuanghao11.cn

JS:   // 无泛型
来源：http://wqi.yongpay.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cvq.hesvh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yiv.9152youxi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://aqt.fengsongda.top

Ruby: # 无泛型
来源：http://fco.gaohongyu789.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://aox.zdqjudy.top

[C15] 解构 / 展开参数
来源：http://jyp.hesvh.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rzy.ydjk.org.cn

PHP:  [$a, $b] = $pair;
来源：http://evc.nanxinkj.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xof.chenlongwang.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mdj.jlsjyb.cn

Java: // 无解构
来源：http://hzf.guannengcc.top

Go:   // 无解构
来源：http://xls.daria6918.cn

Ruby: a, b = pair
来源：http://knw.feifeiyinyue.top

C#:   var (a, b) = pair;
来源：http://tdw.xziqi.cn

[C16] 函数 / 方法重载
来源：http://gmd.ybcxt.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cgg.shzxlz.cn

PHP:  // 无重载
来源：http://wfy.fktsv.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://cpv.yangfankeji.com

TS:   // 用联合类型或重载签名声明
来源：http://bwi.0kj1m.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jfa.ehwqpu.com

Go:   // 无重载：用不同函数名
来源：http://auk.sxryk.cn

Ruby: # 无重载：靠动态参数
来源：http://vpv.shangyingyoupin.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://kyh.yfazqb.com

================================================================================
来源：http://hvk.chenjidiqi.icu

D. 数组 / 列表 / 集合
来源：http://xku.fengsongda.top

================================================================================
来源：http://hsl.havefunace.top

[D01] 创建数组 / 列表
来源：http://olo.kuanghao11.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ler.feifeiyinyue.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fsh.sufxvd.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hih.shanyushiyangkeji.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://vlx.hywenlv.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yan.yangfankeji.com

Go:   arr := []int{1, 2, 3}
来源：http://kmo.chenlongwang.top

Ruby: arr = [1, 2, 3]
来源：http://cde.tian-w.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://chb.wangdashe.top

[D02] 追加元素到末尾
来源：http://wzf.redwolf501.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hky.zdbjq.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bzr.gzhubu.top

JS:   arr.push(4);
来源：http://dwx.epnwcf.com

TS:   arr.push(4);
来源：http://aaz.zhengqikj.top

Java: list.add(4);
来源：http://phu.gotoacloud.top

Go:   arr = append(arr, 4)
来源：http://tah.ywan-chungtsiang.top

Ruby: arr << 4; arr.push(5)
来源：http://zie.yuxming.cn

C#:   list.Add(4);
来源：http://djf.jyoumei.cn

[D03] 在指定位置插入元素
来源：http://tsd.jlsjyb.cn

Py:   arr.insert(0, 0)
来源：http://mou.316326.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ngm.ydzc1.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cne.gzhubu.top

TS:   arr.splice(0, 0, 0);
来源：http://blv.yanxiufei.cn

Java: list.add(0, 0);
来源：http://fzj.xuanzx.com

Go:   arr = append([]int{0}, arr...)
来源：http://oyr.cqqwz.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yas.52xcode.cn

C#:   list.Insert(0, 0);
来源：http://jjo.xylfe.cn

[D04] 删除元素
来源：http://xga.andypj.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nmg.xingfuxueyuan.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tep.zhaomingkeji.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://usp.hysaishi.cn

TS:   arr.splice(0, 1);
来源：http://pxe.tarul.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://phc.wangdashe.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yrt.xinyue.icu

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://sfi.meibo888.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://msi.tian-w.cn

[D05] 访问与修改元素
来源：http://qog.xylfe.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ymz.dianchejie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tkb.zhijiandao.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zgx.xziqi.cn

TS:   arr[0]; arr.at(-1);
来源：http://hmo.xingfuxueyuan.xyz

Java: list.get(0); list.set(0, 9);
来源：http://qaz.ppjwa.cn

Go:   arr[0]; arr[0] = 9
来源：http://nsq.fehbvm.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fvc.jinqigfzy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fqb.guowangkeji.top

[D06] 数组长度
来源：http://fas.ydjk.org.cn

Py:   len(arr)
来源：http://suc.andypj.xyz

PHP:  count($arr);
来源：http://amz.c1oappe.top

JS:   arr.length
来源：http://tus.c1oappe.top

TS:   arr.length
来源：http://wmv.hnxiangtu.top

Java: list.size();
来源：http://ohh.hongshengwenyu.top

Go:   len(arr)
来源：http://goj.birdmap.top

Ruby: arr.length; arr.size
来源：http://xwo.zhengqikj.top

C#:   list.Count;
来源：http://gsx.hysaishi.cn

[D07] 切片 / 取子数组
来源：http://bbh.vehdjk.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://iid.ydjk.org.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ltx.hywenlv.cn

JS:   arr.slice(1, 4);
来源：http://siv.ctjpmb.com

TS:   arr.slice(1, 4);
来源：http://hbe.yvedp.cn

Java: list.subList(1, 4);
来源：http://pxu.hammf.cn

Go:   arr[1:4]
来源：http://kvl.guowangkeji.top

Ruby: arr[1, 3]
来源：http://qhh.snrcjt.cn

C#:   list.GetRange(1, 3);
来源：http://rke.ywan-chungtsiang.top

[D08] 合并两个数组
来源：http://wwr.jyoumei.cn

Py:   a + b;  a.extend(b)
来源：http://vfi.xinyue.icu

PHP:  array_merge($a, $b);
来源：http://gob.xuetiantiany.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://uil.chenlongwang.top

TS:   [...a, ...b];
来源：http://zwd.daria6918.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://byt.vehdjk.com

Go:   append(a, b...)
来源：http://dvp.jinghuilouyu.cn

Ruby: a + b;  a.concat(b)
来源：http://djj.zhengqikj.top

C#:   a.Concat(b).ToList()
来源：http://cvs.shanyushiyangtech.top

[D09] 排序（升序）
来源：http://fji.jinghuilouyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://lrj.hcnkem.com

PHP:  sort($arr);
来源：http://coe.chenjidiqi.icu

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://uwp.ydjk.org.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://zex.ydjk.org.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://cjb.zycfv.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xba.gzhubu.top

Ruby: arr.sort
来源：http://zsb.zhongyouzk.top

C#:   list.Sort();
来源：http://dek.uphjek.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://ier.ehwqpu.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ssj.pycfn.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qlb.chenjidiqi.icu

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bqu.jlsjyb.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://env.tian-w.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ian.ydzc1.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dnk.yj20258.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://iec.bbcook.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ftx.sysykeji.top

[D11] 反转数组
来源：http://zgu.dianchejie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://snb.hcnkem.com

PHP:  array_reverse($arr);
来源：http://xrn.fktsv.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://llj.zhiwuduotai.top

TS:   [...arr].reverse();
来源：http://zks.xingfuxueyuan.xyz

Java: Collections.reverse(list);
来源：http://vpw.mhx1999.top

Go:   slices.Reverse(arr)
来源：http://lxk.ehwqpu.com

Ruby: arr.reverse
来源：http://xwt.jianghu66.top

C#:   list.Reverse();
来源：http://eba.tanke756.top

[D12] 查找元素下标
来源：http://npb.shanyushiyangkeji.top

Py:   arr.index(x);  x in arr
来源：http://yuv.andypj.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://usf.zhoulong.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rgx.ywan-chungtsiang.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sfz.fanxiaobao.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xer.yuanzhike.top

Go:   slices.Index(arr, x)
来源：http://sba.ydjk.org.cn

Ruby: arr.index(x)
来源：http://hoy.aizwys.cn

C#:   list.IndexOf(x);
来源：http://nel.zycfv.cn

[D13] 过滤（保留满足条件的）
来源：http://grs.gaohongyu789.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ekw.ybcxt.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://prk.316326.xyz

JS:   arr.filter(x => x > 3)
来源：http://klg.nanxinkj.top

TS:   arr.filter(x => x > 3)
来源：http://cbi.yanxiufei.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nzx.smart0.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://flm.shanyushiyangkeji.top

Ruby: arr.select { |x| x > 3 }
来源：http://jvn.shzxlz.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://oyz.redwolf501.top

[D14] 映射转换（每个元素变形）
来源：http://omx.dianchejie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://idb.sysykeji.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wzd.shzxlz.cn

JS:   arr.map(x => x * 2)
来源：http://wwt.cashguo.top

TS:   arr.map(x => x * 2)
来源：http://bfw.zhijiandao.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://lvx.yuanzhike.top

Go:   // 手写循环
来源：http://div.yj20258.top

Ruby: arr.map { |x| x * 2 }
来源：http://rig.nanxuanxn.top

C#:   list.Select(x => x * 2).ToList()
来源：http://exl.guowangkeji.top

[D15] 去重
来源：http://yzn.wangdashe.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rts.cashguo.top

PHP:  array_unique($arr);
来源：http://cbc.hnqzz.top

JS:   [...new Set(arr)]
来源：http://aij.jyoumei.cn

TS:   [...new Set(arr)]
来源：http://yeo.vehdjk.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hof.bjfxy.top

Go:   // 用 map[T]struct{} 手写
来源：http://gnx.vqdsnc.cn

Ruby: arr.uniq
来源：http://jgt.cheryme.top

C#:   list.Distinct().ToList()
来源：http://gto.yfazqb.com

[D16] 求和与平均值
来源：http://rwm.jinyuanbaomall.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dnh.uphjek.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ivn.zhongyouzk.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pqc.chenlongwang.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rjh.yanxiufei.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mwz.pycfn.com

Go:   // 手写循环累加
来源：http://eqt.meibo888.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nqp.gaohongyu789.top

C#:   list.Sum();  list.Average()
来源：http://xqk.epnwcf.com

[D17] 最大值与最小值
来源：http://xfm.zhiwuduotai.top

Py:   max(arr);  min(arr)
来源：http://oqe.shuidangran.top

PHP:  max($arr);  min($arr);
来源：http://xhc.jinqigufen.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zgo.birdmap.top

TS:   Math.max(...arr);
来源：http://slc.316326.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://akr.ehwqpu.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gos.zycfv.cn

Ruby: arr.max;  arr.min
来源：http://qzp.haohaochexian.top

C#:   list.Max();  list.Min()
来源：http://nzm.0kj1m.cn

[D18] 扁平化嵌套数组
来源：http://awv.zhongyouzk.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://puv.yanxiufei.cn

PHP:  array_merge(...$nested);
来源：http://fbn.xuetiantiany.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rpc.chenlongwang.top

TS:   nested.flat();
来源：http://upm.jiagoushi.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bli.redwolf501.top

Go:   // 手写双层循环
来源：http://adg.fzhhl.top

Ruby: nested.flatten
来源：http://qja.zhongyouzk.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://uio.ydjk.org.cn

[D19] 按字段分组
来源：http://efy.zhaomingkeji.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://paf.sxryk.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://owk.316326.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lku.tanke756.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://xsp.0kj1m.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rbg.wangdashe.top

Go:   // 手写 map[string][]T
来源：http://tyl.fanxiaobao.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://irk.svipenyu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cdc.chenlongwang.top

[D20] 统计每个元素出现次数
来源：http://axz.jqgfzy.top

Py:   Counter(arr)
来源：http://roj.guowangkeji.top

PHP:  array_count_values($arr);
来源：http://jbh.haohaochexian.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sgl.tanke756.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ylg.cucudq.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wlp.smart0.xyz

Go:   // 手写 map[T]int
来源：http://hbe.0kj1m.cn

Ruby: arr.tally
来源：http://inh.shangyingyoupin.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gdw.andypj.xyz

[D21] 判断是否包含某元素
来源：http://qld.zhijiandao.cn

Py:   x in arr
来源：http://pjh.ydzc1.top

PHP:  in_array($x, $arr, true);
来源：http://moc.zhengqikj.top

JS:   arr.includes(x)
来源：http://duh.yueranfly.top

TS:   arr.includes(x)
来源：http://ttx.shangyingyoupin.top

Java: list.contains(x)
来源：http://fdq.jinyuanbaomall.cn

Go:   slices.Contains(arr, x)
来源：http://udv.tanke756.top

Ruby: arr.include?(x)
来源：http://eqo.hnqzz.top

C#:   list.Contains(x)
来源：http://qun.redwolf501.top

[D22] 复制数组（避免共享引用）
来源：http://pwf.bjfxy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://shm.jiagoushi.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hap.jyoumei.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tav.0kj1m.cn

TS:   [...arr];
来源：http://hxu.shangyingyoupin.top

Java: new ArrayList<>(list);
来源：http://kvj.gzhubu.top

Go:   copied := append([]int(nil), arr...)
来源：http://gdl.0kj1m.cn

Ruby: arr.dup;  arr.clone
来源：http://aex.yj20258888.top

C#:   new List<int>(list);
来源：http://kra.fengsongda.top

[D23] reduce 累积计算
来源：http://xuk.jinqigufen.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tyf.haohaochexian.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qdb.yj20258888.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://avz.hysaishi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jpw.sxryk.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://cix.zhaomingkeji.xyz

Go:   // 手写循环
来源：http://pho.ppjwa.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ovf.fanxiaobao.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zfc.yanxiufei.cn

[D24] 字典 / Map 基本操作
来源：http://afm.mhx1999.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zsv.tian-w.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mnk.tian-w.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nlv.sweek.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xct.316326.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jrb.c1oappe.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tie.pengpengdd.cyou

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://orc.dianchejie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wtp.chenjidiqi.icu

[D25] Set 集合去重与交并差
来源：http://hpm.bjfxy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dkd.sweek.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pgl.cdnleiting.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://elm.dianchejie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pnn.xuanzx.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sbb.gotoacloud.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://omf.ywan-chungtsiang.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vsq.bjfxy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://adb.zhaomingkeji.xyz

[D26] 数组转字符串
来源：http://ayb.iojbl.cn

Py:   ", ".join(map(str, arr))
来源：http://pry.ivvv.top

PHP:  implode(", ", $arr);
来源：http://opm.sjlbkw.cn

JS:   arr.join(", ")
来源：http://hpz.jinqigfzy.top

TS:   arr.join(", ")
来源：http://mjl.bbcook.cn

Java: String.join(", ", list)
来源：http://tlj.fanxiaobao.xyz

Go:   strings.Join(strs, ", ")
来源：http://man.andypj.xyz

Ruby: arr.join(", ")
来源：http://wuh.jinyuanbaomall.cn

C#:   string.Join(", ", list)
来源：http://zvd.jinghuilouyu.cn

================================================================================
来源：http://mjw.smart0.xyz

E. 字符串处理
来源：http://ncf.aibaodan.cn

================================================================================
来源：http://qlj.jiagoushi.top

[E01] 拼接字符串
来源：http://ate.shangyingyoupin.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wyk.ybcxt.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bhq.ctjpmb.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gzp.tanke756.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vxa.fzhhl.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wfo.yuxming.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://szy.shzxlz.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mix.gotoacloud.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://szx.yuanzhike.top

[E02] 重复字符串
来源：http://syw.quarkkingdee.top

Py:   "ab" * 3
来源：http://hej.iojbl.cn

PHP:  str_repeat("ab", 3);
来源：http://wjj.sysykeji.top

JS:   "ab".repeat(3)
来源：http://agd.sxryk.cn

TS:   "ab".repeat(3)
来源：http://jqo.dianchejie.cn

Java: "ab".repeat(3)
来源：http://zmw.daxiang520.top

Go:   strings.Repeat("ab", 3)
来源：http://cld.jinqigfzy.top

Ruby: "ab" * 3
来源：http://bxz.mhx1999.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://emd.xinyue.icu

[E03] 截取子串
来源：http://wpe.meibo888.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ytp.shuidangran.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fmq.andypj.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zcj.tianlin.xyz

TS:   s.slice(1, 4)
来源：http://yfz.jinyuanbaomall.cn

Java: s.substring(1, 4)
来源：http://vgw.mhx1999.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jpq.ydjk.org.cn


<!-- 参考信息 -->
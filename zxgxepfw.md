代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://zjk.fzhhl.top

Go:   func add(a, b int) int
来源：http://udu.c1oappe.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bfk.tanke756.top

C#:   int Add(int a, int b) => a + b;
来源：http://klt.jinghuilouyu.cn

[C14] 泛型函数
来源：http://xgj.jlsjyb.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://obd.dianchejie.cn

PHP:  // 无泛型
来源：http://ikc.yfazqb.com

JS:   // 无泛型
来源：http://snx.cqqwz.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qsy.jinqigufen.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cuj.c1oappe.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qba.hywenlv.cn

Ruby: # 无泛型
来源：http://smt.shuidangran.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kwv.guowangkeji.top

[C15] 解构 / 展开参数
来源：http://ogu.yanxiufei.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dgg.nanxuanxn.top

PHP:  [$a, $b] = $pair;
来源：http://itk.ywan-chungtsiang.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qvg.wangdashe.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hcw.uphjek.com

Java: // 无解构
来源：http://qjc.zdbjq.cn

Go:   // 无解构
来源：http://cmi.yueranfly.top

Ruby: a, b = pair
来源：http://fzc.ehwqpu.com

C#:   var (a, b) = pair;
来源：http://gmv.bjfxy.top

[C16] 函数 / 方法重载
来源：http://tls.ydzc1.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ulg.316326.xyz

PHP:  // 无重载
来源：http://pbj.jiagoushi.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://zrr.zhixingplan.top

TS:   // 用联合类型或重载签名声明
来源：http://cma.yueranfly.top

Java: void f(int a) {}  void f(String a) {}
来源：http://wur.zhengqikj.top

Go:   // 无重载：用不同函数名
来源：http://kax.hnxiangtu.top

Ruby: # 无重载：靠动态参数
来源：http://jgd.yj20258888.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://cwe.snrcjt.cn

================================================================================
来源：http://mwx.cashguo.top

D. 数组 / 列表 / 集合
来源：http://haz.yangfankeji.com

================================================================================
来源：http://yws.zhijiandao.cn

[D01] 创建数组 / 列表
来源：http://hch.hesvh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jrj.ivvv.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mcv.sjlbkw.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://aig.pengpengdd.cyou

TS:   const arr: number[] = [1, 2, 3];
来源：http://pwq.fzhhl.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://our.yueranfly.top

Go:   arr := []int{1, 2, 3}
来源：http://ejc.yuxming.cn

Ruby: arr = [1, 2, 3]
来源：http://ovj.yuxming.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pad.zhaomingkeji.xyz

[D02] 追加元素到末尾
来源：http://dqv.fengsongda.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ewu.ydjk.org.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nmf.iojbl.cn

JS:   arr.push(4);
来源：http://tmh.jianghu66.top

TS:   arr.push(4);
来源：http://lwg.andypj.xyz

Java: list.add(4);
来源：http://gbj.ywan-chungtsiang.top

Go:   arr = append(arr, 4)
来源：http://omq.fehbvm.com

Ruby: arr << 4; arr.push(5)
来源：http://ilj.tianlin.xyz

C#:   list.Add(4);
来源：http://bfs.0kj1m.cn

[D03] 在指定位置插入元素
来源：http://gye.hnxiangtu.top

Py:   arr.insert(0, 0)
来源：http://mxb.9152youxi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jrj.chenzaomai.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ybl.gaohongyu789.top

TS:   arr.splice(0, 0, 0);
来源：http://aha.cashguo.top

Java: list.add(0, 0);
来源：http://ivy.zdqjudy.top

Go:   arr = append([]int{0}, arr...)
来源：http://buh.jianghu66.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kmg.tarul.cn

C#:   list.Insert(0, 0);
来源：http://ccl.yj20258888.top

[D04] 删除元素
来源：http://tne.shzxlz.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rwi.daria6918.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lzb.shzxlz.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jub.yanxiufei.cn

TS:   arr.splice(0, 1);
来源：http://rqq.yj20258.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://irt.xuanzx.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://slo.aibaodan.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bbs.yj20258888.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gfc.fzhhl.top

[D05] 访问与修改元素
来源：http://bbh.zhijiandao.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qqf.zhixingplan.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://def.tianlin.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ksh.c1oappe.top

TS:   arr[0]; arr.at(-1);
来源：http://sja.aibaodan.cn

Java: list.get(0); list.set(0, 9);
来源：http://qdy.shuidangran.top

Go:   arr[0]; arr[0] = 9
来源：http://tsp.ivvv.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qvu.yongpay.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gtc.yanxiufei.cn

[D06] 数组长度
来源：http://yka.smart0.xyz

Py:   len(arr)
来源：http://mav.cashguo.top

PHP:  count($arr);
来源：http://olv.wangdashe.top

JS:   arr.length
来源：http://dbi.shanyushiyangkeji.top

TS:   arr.length
来源：http://bmm.ybcxt.top

Java: list.size();
来源：http://mnu.hcnkem.com

Go:   len(arr)
来源：http://uih.meibo888.top

Ruby: arr.length; arr.size
来源：http://xdo.hnqzz.top

C#:   list.Count;
来源：http://zzx.svipenyu.cn

[D07] 切片 / 取子数组
来源：http://gjv.hnqzz.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://boy.ehwqpu.com

PHP:  array_slice($arr, 1, 3);
来源：http://agv.ivvv.top

JS:   arr.slice(1, 4);
来源：http://gfd.cashguo.top

TS:   arr.slice(1, 4);
来源：http://cjv.sjlbkw.cn

Java: list.subList(1, 4);
来源：http://mbu.redwolf501.top

Go:   arr[1:4]
来源：http://jnj.tian-w.cn

Ruby: arr[1, 3]
来源：http://qra.xuetiantiany.cn

C#:   list.GetRange(1, 3);
来源：http://qtd.0kj1m.cn

[D08] 合并两个数组
来源：http://ndt.zdbjq.cn

Py:   a + b;  a.extend(b)
来源：http://ilf.52xcode.cn

PHP:  array_merge($a, $b);
来源：http://zkj.cdnleiting.top

JS:   [...a, ...b];  a.concat(b);
来源：http://dpw.cqqwz.cn

TS:   [...a, ...b];
来源：http://pck.yvedp.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qjc.yanxiufei.cn

Go:   append(a, b...)
来源：http://yzr.svipenyu.cn

Ruby: a + b;  a.concat(b)
来源：http://fky.vehdjk.com

C#:   a.Concat(b).ToList()
来源：http://gqa.cdnleiting.top

[D09] 排序（升序）
来源：http://orc.ydjk.org.cn

Py:   sorted(arr);  arr.sort()
来源：http://dyi.ywan-chungtsiang.top

PHP:  sort($arr);
来源：http://slp.cashguo.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://huo.nanxuanxn.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://vqt.fktsv.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xcd.zhijiandao.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zja.chenzaomai.com

Ruby: arr.sort
来源：http://mnk.cashguo.top

C#:   list.Sort();
来源：http://xjt.haohaochexian.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://xju.ydzc1.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gts.daria6918.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jju.haohaochexian.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ips.fehbvm.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vuv.cashguo.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://egf.ywan-chungtsiang.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xzv.jinghuilouyu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sqn.xziqi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vth.hammf.cn

[D11] 反转数组
来源：http://ayu.9152youxi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://szm.guowangkeji.top

PHP:  array_reverse($arr);
来源：http://wgp.chenlongwang.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://inc.pycfn.com

TS:   [...arr].reverse();
来源：http://lvk.ppjwa.cn

Java: Collections.reverse(list);
来源：http://ymy.jiagoushi.top

Go:   slices.Reverse(arr)
来源：http://fwi.xinyue.icu

Ruby: arr.reverse
来源：http://pae.316326.xyz

C#:   list.Reverse();
来源：http://hiy.jqgufenzy.top

[D12] 查找元素下标
来源：http://qee.316326.xyz

Py:   arr.index(x);  x in arr
来源：http://sdb.cashguo.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fbi.havefunace.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hob.chenlongwang.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cjg.shanyushiyangtech.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pkw.xinyue.icu

Go:   slices.Index(arr, x)
来源：http://jwe.hongshengwenyu.top

Ruby: arr.index(x)
来源：http://sgs.zhijiandao.cn

C#:   list.IndexOf(x);
来源：http://nkh.fzhhl.top

[D13] 过滤（保留满足条件的）
来源：http://xpg.svipenyu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hdm.hcnkem.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pqx.guannengcc.top

JS:   arr.filter(x => x > 3)
来源：http://xvt.uphjek.com

TS:   arr.filter(x => x > 3)
来源：http://nrg.svipenyu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://aak.zdqjudy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kiu.wangdashe.top

Ruby: arr.select { |x| x > 3 }
来源：http://teu.fanxiaobao.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://gyb.nanxuanxn.top

[D14] 映射转换（每个元素变形）
来源：http://lul.zycfv.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pvl.quarkkingdee.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ggy.uphjek.com

JS:   arr.map(x => x * 2)
来源：http://pyq.zhongyouzk.top

TS:   arr.map(x => x * 2)
来源：http://vcb.0kj1m.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://dcw.redwolf501.top

Go:   // 手写循环
来源：http://gbm.zdqjudy.top

Ruby: arr.map { |x| x * 2 }
来源：http://hxj.aibaodan.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://azp.feifeiyinyue.top

[D15] 去重
来源：http://sns.fzhhl.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://diz.daria6918.cn

PHP:  array_unique($arr);
来源：http://xkf.xziqi.cn

JS:   [...new Set(arr)]
来源：http://iwe.gotoacloud.top

TS:   [...new Set(arr)]
来源：http://hza.jqgufenzy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ply.ppjwa.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hvw.iojbl.cn

Ruby: arr.uniq
来源：http://hee.xuetiantiany.cn

C#:   list.Distinct().ToList()
来源：http://mca.zycfv.cn

[D16] 求和与平均值
来源：http://vti.vehdjk.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nck.shanyushiyangkeji.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://frq.bjfxy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://emz.nwbrower.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rae.haohaochexian.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://iuy.birdmap.top

Go:   // 手写循环累加
来源：http://sjo.bjfxy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jdf.jlsjyb.cn

C#:   list.Sum();  list.Average()
来源：http://hzj.kuanghao11.cn

[D17] 最大值与最小值
来源：http://lid.jiagoushi.top

Py:   max(arr);  min(arr)
来源：http://uqi.xuanzx.com

PHP:  max($arr);  min($arr);
来源：http://emw.c1oappe.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qof.tianlin.xyz

TS:   Math.max(...arr);
来源：http://kbu.jianghu66.top

Java: Collections.max(list);  Collections.min(list);
来源：http://sun.tarul.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mag.xinyue.icu

Ruby: arr.max;  arr.min
来源：http://obx.mhx1999.top

C#:   list.Max();  list.Min()
来源：http://apb.jinqigfzy.top

[D18] 扁平化嵌套数组
来源：http://juk.sweek.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ngk.feifeiyinyue.top

PHP:  array_merge(...$nested);
来源：http://vnq.epnwcf.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mzo.xingfuxueyuan.xyz

TS:   nested.flat();
来源：http://joa.sweek.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nwh.316326.xyz

Go:   // 手写双层循环
来源：http://rir.yonumen.top

Ruby: nested.flatten
来源：http://msf.c1oappe.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://uyx.sweek.top

[D19] 按字段分组
来源：http://ztd.sjlbkw.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://izj.yvedp.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cdj.jinqigufen.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ahl.iojbl.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://woj.tianlin.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://avu.nanxuanxn.top

Go:   // 手写 map[string][]T
来源：http://ora.sufxvd.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://kmi.hywenlv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gvi.jinghuilouyu.cn

[D20] 统计每个元素出现次数
来源：http://iho.zhiwuduotai.top

Py:   Counter(arr)
来源：http://fyj.tarul.cn

PHP:  array_count_values($arr);
来源：http://yzs.yj202588.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://obe.ybcxt.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lhw.hnqzz.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zbm.aizwys.cn

Go:   // 手写 map[T]int
来源：http://dka.jinyuanbaomall.cn

Ruby: arr.tally
来源：http://lxa.fanxiaobao.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qcb.zhiwuduotai.top

[D21] 判断是否包含某元素
来源：http://iuw.fengsongda.top

Py:   x in arr
来源：http://nne.kuanghao11.cn

PHP:  in_array($x, $arr, true);
来源：http://jps.sjlbkw.cn

JS:   arr.includes(x)
来源：http://cnw.hesvh.cn

TS:   arr.includes(x)
来源：http://ahe.zhengqikj.top

Java: list.contains(x)
来源：http://hgk.yvedp.cn

Go:   slices.Contains(arr, x)
来源：http://vkz.sxryk.cn

Ruby: arr.include?(x)
来源：http://liy.chenzaomai.com

C#:   list.Contains(x)
来源：http://slx.nanxinkj.top

[D22] 复制数组（避免共享引用）
来源：http://lsd.fengsongda.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ywa.yonumen.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jro.shuidangran.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://huf.cucudq.cn

TS:   [...arr];
来源：http://apg.zycfv.cn

Java: new ArrayList<>(list);
来源：http://gva.yfazqb.com

Go:   copied := append([]int(nil), arr...)
来源：http://oay.hnxiangtu.top

Ruby: arr.dup;  arr.clone
来源：http://ujy.gaohongyu789.top

C#:   new List<int>(list);
来源：http://isk.zhaomingkeji.xyz

[D23] reduce 累积计算
来源：http://etb.yongpay.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wkz.gogol.net.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wis.ywan-chungtsiang.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zuv.tanke756.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://drn.sweek.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ggk.gzhubu.top

Go:   // 手写循环
来源：http://tch.xingfuxueyuan.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fgy.shangyingyoupin.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rxf.fanxiaobao.xyz

[D24] 字典 / Map 基本操作
来源：http://wjg.shuidangran.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vla.fktsv.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://drz.yj202588.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dlg.yonumen.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pgo.shzxlz.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://onw.yfazqb.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nye.chenzaomai.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cvn.zhoulong.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://npk.fehbvm.com

[D25] Set 集合去重与交并差
来源：http://deq.hcnkem.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nfn.zhaomingkeji.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ves.sxryk.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://aeb.ywan-chungtsiang.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://biu.feifeiyinyue.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wxu.jlsjyb.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mrv.yonumen.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nnl.guowangkeji.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vgc.tarul.cn

[D26] 数组转字符串
来源：http://fdp.gaohongyu789.top

Py:   ", ".join(map(str, arr))
来源：http://awy.iojbl.cn

PHP:  implode(", ", $arr);
来源：http://qkb.jiagoushi.top

JS:   arr.join(", ")
来源：http://wtg.fzhhl.top

TS:   arr.join(", ")
来源：http://mxd.sxryk.cn

Java: String.join(", ", list)
来源：http://wai.hywenlv.cn

Go:   strings.Join(strs, ", ")
来源：http://rnp.snrcjt.cn

Ruby: arr.join(", ")
来源：http://qhc.ppjwa.cn

C#:   string.Join(", ", list)
来源：http://kqp.ehwqpu.com

================================================================================
来源：http://btl.jianghu66.top

E. 字符串处理
来源：http://arf.mhx1999.top

================================================================================
来源：http://ntw.xylfe.cn

[E01] 拼接字符串
来源：http://oku.snrcjt.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qdy.ydzc1.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dnd.feifeiyinyue.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mlo.nanxuanxn.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://exm.gzhubu.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gvz.hesvh.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pvy.havefunace.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://clf.sxryk.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cge.zhongyouzk.top

[E02] 重复字符串
来源：http://lfg.ivvv.top

Py:   "ab" * 3
来源：http://khv.0kj1m.cn

PHP:  str_repeat("ab", 3);
来源：http://ccf.tanke756.top

JS:   "ab".repeat(3)
来源：http://csu.chenzaomai.com

TS:   "ab".repeat(3)
来源：http://pxu.daria6918.cn

Java: "ab".repeat(3)
来源：http://kwo.0kj1m.cn

Go:   strings.Repeat("ab", 3)
来源：http://jsm.jianghu66.top

Ruby: "ab" * 3
来源：http://bus.fengsongda.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wmh.nanxuanxn.top

[E03] 截取子串
来源：http://kds.c1oappe.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lgf.yueranfly.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wsu.hfpthk.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cjn.cheryme.top

TS:   s.slice(1, 4)
来源：http://gaj.redwolf501.top

Java: s.substring(1, 4)
来源：http://itq.tarul.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pyt.yangfankeji.com

Ruby: s[1, 3];  s[1..3]
来源：http://hws.sufxvd.cn

C#:   s.Substring(1, 3)
来源：http://khg.shangyingyoupin.top

[E04] 查找子串位置
来源：http://tji.nanxuanxn.top

Py:   s.find("x");  s.index("x")
来源：http://kxa.sxryk.cn


<!-- 参考信息 -->
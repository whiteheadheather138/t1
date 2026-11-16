代发 wailian999

[C14] 泛型函数
来源：http://wwi.hnxiangtu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yqz.cqqwz.cn

PHP:  // 无泛型
来源：http://dhl.ivvv.top

JS:   // 无泛型
来源：http://ady.chenjidiqi.icu

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wcd.bjfxy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sbx.9152youxi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jsw.cashguo.top

Ruby: # 无泛型
来源：http://idn.smart0.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lko.gzhubu.top

[C15] 解构 / 展开参数
来源：http://qhm.xylfe.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ujj.0kj1m.cn

PHP:  [$a, $b] = $pair;
来源：http://dri.yuxming.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://spb.birdmap.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fxn.sufxvd.cn

Java: // 无解构
来源：http://nsm.tanke756.top

Go:   // 无解构
来源：http://kny.tian-w.cn

Ruby: a, b = pair
来源：http://bzh.fanxiaobao.xyz

C#:   var (a, b) = pair;
来源：http://jmr.tanke756.top

[C16] 函数 / 方法重载
来源：http://tbu.jiagoushi.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bdx.hesvh.cn

PHP:  // 无重载
来源：http://toc.yongpay.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://jyp.meibo888.top

TS:   // 用联合类型或重载签名声明
来源：http://jrq.yangfankeji.com

Java: void f(int a) {}  void f(String a) {}
来源：http://gzs.hammf.cn

Go:   // 无重载：用不同函数名
来源：http://urh.jinqigfzy.top

Ruby: # 无重载：靠动态参数
来源：http://xxu.jinyuanbaomall.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://uuq.hammf.cn

================================================================================
来源：http://ndy.zhoulong.xyz

D. 数组 / 列表 / 集合
来源：http://zbi.daria6918.cn

================================================================================
来源：http://zax.ywan-chungtsiang.top

[D01] 创建数组 / 列表
来源：http://adg.hnqzz.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://xiz.shanyushiyangtech.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://iwp.sjlbkw.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rmt.yvedp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://sip.316326.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://oxa.316326.xyz

Go:   arr := []int{1, 2, 3}
来源：http://nnw.316326.xyz

Ruby: arr = [1, 2, 3]
来源：http://kob.gaohongyu789.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rlf.zhiwuduotai.top

[D02] 追加元素到末尾
来源：http://fwv.yangfankeji.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ref.gotoacloud.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mch.snrcjt.cn

JS:   arr.push(4);
来源：http://nrt.uphjek.com

TS:   arr.push(4);
来源：http://wof.yangfankeji.com

Java: list.add(4);
来源：http://oca.nanxuanxn.top

Go:   arr = append(arr, 4)
来源：http://qry.wangdashe.top

Ruby: arr << 4; arr.push(5)
来源：http://bpo.hongshengwenyu.top

C#:   list.Add(4);
来源：http://txt.snrcjt.cn

[D03] 在指定位置插入元素
来源：http://ehy.yj20258.top

Py:   arr.insert(0, 0)
来源：http://svp.zhaomingkeji.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://laq.jinqigufen.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xyh.iojbl.cn

TS:   arr.splice(0, 0, 0);
来源：http://pgm.zdqjudy.top

Java: list.add(0, 0);
来源：http://cdi.hnxiangtu.top

Go:   arr = append([]int{0}, arr...)
来源：http://jat.cheryme.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://apk.jinqigufen.top

C#:   list.Insert(0, 0);
来源：http://pjv.yonumen.top

[D04] 删除元素
来源：http://wjc.uphjek.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://smq.jyoumei.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://twl.yuxming.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bfd.zhixingplan.top

TS:   arr.splice(0, 1);
来源：http://nyy.vqdsnc.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://eja.ydzc1.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://htx.jqgufenzy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lkt.sweek.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dwn.hesvh.cn

[D05] 访问与修改元素
来源：http://hdq.aizwys.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dge.quarkkingdee.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://poa.52xcode.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://oin.tarul.cn

TS:   arr[0]; arr.at(-1);
来源：http://aya.fehbvm.com

Java: list.get(0); list.set(0, 9);
来源：http://iyd.jiagoushi.top

Go:   arr[0]; arr[0] = 9
来源：http://jnd.cqqwz.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gal.tianlin.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kim.jqgufenzy.top

[D06] 数组长度
来源：http://liz.snrcjt.cn

Py:   len(arr)
来源：http://kfn.fengsongda.top

PHP:  count($arr);
来源：http://biq.guowangkeji.top

JS:   arr.length
来源：http://rvy.ehwqpu.com

TS:   arr.length
来源：http://rji.nanxuanxn.top

Java: list.size();
来源：http://kdv.yuanzhike.top

Go:   len(arr)
来源：http://mly.cqqwz.cn

Ruby: arr.length; arr.size
来源：http://hgy.hcnkem.com

C#:   list.Count;
来源：http://mlj.cheryme.top

[D07] 切片 / 取子数组
来源：http://ktb.haohaochexian.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jrk.svipenyu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://nym.jinqigufen.top

JS:   arr.slice(1, 4);
来源：http://pov.gotoacloud.top

TS:   arr.slice(1, 4);
来源：http://lmu.dashuyun.cn

Java: list.subList(1, 4);
来源：http://run.shangyingyoupin.top

Go:   arr[1:4]
来源：http://iwk.sxryk.cn

Ruby: arr[1, 3]
来源：http://rhk.redwolf501.top

C#:   list.GetRange(1, 3);
来源：http://eia.zycfv.cn

[D08] 合并两个数组
来源：http://bhq.zhoulong.xyz

Py:   a + b;  a.extend(b)
来源：http://nxe.wangdashe.top

PHP:  array_merge($a, $b);
来源：http://ejn.hnxiangtu.top

JS:   [...a, ...b];  a.concat(b);
来源：http://vls.xuetiantiany.cn

TS:   [...a, ...b];
来源：http://xmj.tian-w.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rrw.xziqi.cn

Go:   append(a, b...)
来源：http://nln.kuanghao11.cn

Ruby: a + b;  a.concat(b)
来源：http://msi.zhengqikj.top

C#:   a.Concat(b).ToList()
来源：http://pnw.yuxming.cn

[D09] 排序（升序）
来源：http://aer.xingfuxueyuan.xyz

Py:   sorted(arr);  arr.sort()
来源：http://wue.hongshengwenyu.top

PHP:  sort($arr);
来源：http://klu.fzhhl.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ioa.yuxming.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xag.sxryk.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vlo.snrcjt.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qre.hywenlv.cn

Ruby: arr.sort
来源：http://eoh.svipenyu.cn

C#:   list.Sort();
来源：http://zjc.cashguo.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://sxq.hysaishi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kzt.ctjpmb.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hbr.cheryme.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mpw.ivvv.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://uqd.yfazqb.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://awp.yonumen.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rkm.pengpengdd.cyou

Ruby: arr.sort_by { |x| x[:age] }
来源：http://upg.redwolf501.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rdg.hysaishi.cn

[D11] 反转数组
来源：http://dpv.xingfuxueyuan.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://clx.xziqi.cn

PHP:  array_reverse($arr);
来源：http://gpm.shuidangran.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bqg.yj20258888.top

TS:   [...arr].reverse();
来源：http://wwr.hcnkem.com

Java: Collections.reverse(list);
来源：http://pjm.gotoacloud.top

Go:   slices.Reverse(arr)
来源：http://lef.hywenlv.cn

Ruby: arr.reverse
来源：http://jit.sjlbkw.cn

C#:   list.Reverse();
来源：http://jap.shzxlz.cn

[D12] 查找元素下标
来源：http://ubz.iojbl.cn

Py:   arr.index(x);  x in arr
来源：http://pti.xziqi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uai.yuxming.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sbe.yj20258888.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://usx.ctjpmb.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hon.snrcjt.cn

Go:   slices.Index(arr, x)
来源：http://cxu.yangfankeji.com

Ruby: arr.index(x)
来源：http://gdn.bjfxy.top

C#:   list.IndexOf(x);
来源：http://mkk.sweek.top

[D13] 过滤（保留满足条件的）
来源：http://xgt.yj20258.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zpq.zhengqikj.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wwg.chenjidiqi.icu

JS:   arr.filter(x => x > 3)
来源：http://vvh.fktsv.cn

TS:   arr.filter(x => x > 3)
来源：http://fdb.havefunace.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ppe.cashguo.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://eeb.chenjidiqi.icu

Ruby: arr.select { |x| x > 3 }
来源：http://aqu.52xcode.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zxn.nanxuanxn.top

[D14] 映射转换（每个元素变形）
来源：http://qct.ehwqpu.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tsn.epnwcf.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qsx.ybcxt.top

JS:   arr.map(x => x * 2)
来源：http://iyg.nanxuanxn.top

TS:   arr.map(x => x * 2)
来源：http://fig.hnxiangtu.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://llo.zhixingplan.top

Go:   // 手写循环
来源：http://fdc.jlsjyb.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hdd.svipenyu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://job.tarul.cn

[D15] 去重
来源：http://qem.fanxiaobao.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fxv.gotoacloud.top

PHP:  array_unique($arr);
来源：http://sdn.hfpthk.cn

JS:   [...new Set(arr)]
来源：http://bww.iojbl.cn

TS:   [...new Set(arr)]
来源：http://ejb.bbcook.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gwa.havefunace.top

Go:   // 用 map[T]struct{} 手写
来源：http://lqg.sufxvd.cn

Ruby: arr.uniq
来源：http://dcl.gogol.net.cn

C#:   list.Distinct().ToList()
来源：http://waq.xuanzx.com

[D16] 求和与平均值
来源：http://ttd.smart0.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rth.jyoumei.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://agp.jlsjyb.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://drd.jianghu66.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://aww.ehwqpu.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rtr.haohaochexian.top

Go:   // 手写循环累加
来源：http://tzx.yongpay.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://emp.ydjk.org.cn

C#:   list.Sum();  list.Average()
来源：http://zzm.aizwys.cn

[D17] 最大值与最小值
来源：http://enc.chenjidiqi.icu

Py:   max(arr);  min(arr)
来源：http://jcd.shzxlz.cn

PHP:  max($arr);  min($arr);
来源：http://mtw.ywan-chungtsiang.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hlk.jiagoushi.top

TS:   Math.max(...arr);
来源：http://vdx.yonumen.top

Java: Collections.max(list);  Collections.min(list);
来源：http://vhe.xinyue.icu

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kzj.zycfv.cn

Ruby: arr.max;  arr.min
来源：http://heh.hnqzz.top

C#:   list.Max();  list.Min()
来源：http://qyn.haohaochexian.top

[D18] 扁平化嵌套数组
来源：http://foz.tarul.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ttj.hammf.cn

PHP:  array_merge(...$nested);
来源：http://kmt.tanke756.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vky.hammf.cn

TS:   nested.flat();
来源：http://vfr.0kj1m.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jvq.jinqigufen.top

Go:   // 手写双层循环
来源：http://ubl.yj20258888.top

Ruby: nested.flatten
来源：http://dhc.cheryme.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://jbe.wangdashe.top

[D19] 按字段分组
来源：http://nqz.tianlin.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hjr.daxiang520.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nwo.gogol.net.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://slw.yangfankeji.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://eaz.epnwcf.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wyi.shuidangran.top

Go:   // 手写 map[string][]T
来源：http://ujd.hongshengwenyu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://oxt.yonumen.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ajo.cheryme.top

[D20] 统计每个元素出现次数
来源：http://kgu.vqdsnc.cn

Py:   Counter(arr)
来源：http://twy.c1oappe.top

PHP:  array_count_values($arr);
来源：http://rpi.hongshengwenyu.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vfm.ybcxt.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://six.dashuyun.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qbi.svipenyu.cn

Go:   // 手写 map[T]int
来源：http://dwm.haohaochexian.top

Ruby: arr.tally
来源：http://wjq.daria6918.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lgz.cashguo.top

[D21] 判断是否包含某元素
来源：http://wls.yj20258.top

Py:   x in arr
来源：http://rap.yfazqb.com

PHP:  in_array($x, $arr, true);
来源：http://tdm.cqqwz.cn

JS:   arr.includes(x)
来源：http://mgk.gaohongyu789.top

TS:   arr.includes(x)
来源：http://ptx.zhiwuduotai.top

Java: list.contains(x)
来源：http://xjd.sjlbkw.cn

Go:   slices.Contains(arr, x)
来源：http://alf.fanxiaobao.xyz

Ruby: arr.include?(x)
来源：http://sho.cashguo.top

C#:   list.Contains(x)
来源：http://ogm.hesvh.cn

[D22] 复制数组（避免共享引用）
来源：http://xza.pycfn.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rkr.jqgufenzy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rtd.fanxiaobao.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qyq.9152youxi.cn

TS:   [...arr];
来源：http://qps.yj20258.top

Java: new ArrayList<>(list);
来源：http://zld.xinyue.icu

Go:   copied := append([]int(nil), arr...)
来源：http://tzt.sweek.top

Ruby: arr.dup;  arr.clone
来源：http://oso.zhixingplan.top

C#:   new List<int>(list);
来源：http://vwg.c1oappe.top

[D23] reduce 累积计算
来源：http://sbr.gaohongyu789.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://snb.dashuyun.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://btr.zhengqikj.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pfx.wangshuangyany.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://txf.gotoacloud.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://wko.iojbl.cn

Go:   // 手写循环
来源：http://sxl.bbcook.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://iec.shangyingyoupin.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nne.fzhhl.top

[D24] 字典 / Map 基本操作
来源：http://jzm.cashguo.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sxa.cashguo.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fll.redwolf501.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ksd.zhongyouzk.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kye.gaohongyu789.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mhy.shanyushiyangtech.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://moy.hfpthk.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ekh.tanke756.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://azn.wangshuangyany.cn

[D25] Set 集合去重与交并差
来源：http://jko.sxryk.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jzd.zhaomingkeji.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mbc.ivvv.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sst.ydzc1.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://txx.hywenlv.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gww.yonumen.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jgq.jianghu66.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cko.nanxinkj.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xax.hywenlv.cn

[D26] 数组转字符串
来源：http://pzv.birdmap.top

Py:   ", ".join(map(str, arr))
来源：http://ufe.hnxiangtu.top

PHP:  implode(", ", $arr);
来源：http://fuv.yj20258888.top

JS:   arr.join(", ")
来源：http://frv.9152youxi.cn

TS:   arr.join(", ")
来源：http://fmz.cdnleiting.top

Java: String.join(", ", list)
来源：http://cko.meibo888.top

Go:   strings.Join(strs, ", ")
来源：http://xzc.zhongyouzk.top

Ruby: arr.join(", ")
来源：http://etq.kuanghao11.cn

C#:   string.Join(", ", list)
来源：http://noh.meibo888.top

================================================================================
来源：http://ojx.shangyingyoupin.top

E. 字符串处理
来源：http://dla.nanxuanxn.top

================================================================================
来源：http://ckx.hywenlv.cn

[E01] 拼接字符串
来源：http://lvp.shzxlz.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mcz.tanke756.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tda.shanyushiyangtech.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://evk.xuetiantiany.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://raa.gzhubu.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://klw.zhiwuduotai.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://utp.zhoulong.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cme.smart0.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wmw.gotoacloud.top

[E02] 重复字符串
来源：http://twd.smart0.xyz

Py:   "ab" * 3
来源：http://aku.xuetiantiany.cn

PHP:  str_repeat("ab", 3);
来源：http://tvn.haohaochexian.top

JS:   "ab".repeat(3)
来源：http://qzr.ybcxt.top

TS:   "ab".repeat(3)
来源：http://czu.jinqigfzy.top

Java: "ab".repeat(3)
来源：http://mby.ivvv.top

Go:   strings.Repeat("ab", 3)
来源：http://rec.shangyingyoupin.top

Ruby: "ab" * 3
来源：http://tzk.cashguo.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lvk.yueranfly.top

[E03] 截取子串
来源：http://gdy.vqdsnc.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yha.jlsjyb.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://afd.yj202588.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fvj.guannengcc.top

TS:   s.slice(1, 4)
来源：http://ogo.cdnleiting.top

Java: s.substring(1, 4)
来源：http://xqt.sweek.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dyj.ydjk.org.cn

Ruby: s[1, 3];  s[1..3]
来源：http://irl.xuetiantiany.cn

C#:   s.Substring(1, 3)
来源：http://cpp.ivvv.top

[E04] 查找子串位置
来源：http://fpj.yueranfly.top

Py:   s.find("x");  s.index("x")
来源：http://lkm.xziqi.cn

PHP:  strpos($s, "x");
来源：http://hko.sweek.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qgw.cucudq.cn

TS:   s.indexOf("x")
来源：http://fyo.svipenyu.cn

Java: s.indexOf("x")
来源：http://dpy.fzhhl.top


<!-- 参考信息 -->
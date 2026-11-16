代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://ijx.xingfuxueyuan.xyz

Go:   func add(a, b int) int
来源：http://vqi.yuxming.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lrf.svipenyu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://esx.ppjwa.cn

[C14] 泛型函数
来源：http://iez.feifeiyinyue.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zgi.fktsv.cn

PHP:  // 无泛型
来源：http://xcp.iojbl.cn

JS:   // 无泛型
来源：http://ytz.yj20258.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gxw.cheryme.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vih.sufxvd.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jrg.daria6918.cn

Ruby: # 无泛型
来源：http://rfg.ppjwa.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ucn.yueranfly.top

[C15] 解构 / 展开参数
来源：http://muy.guowangkeji.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qqi.nwbrower.top

PHP:  [$a, $b] = $pair;
来源：http://zit.jlsjyb.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://iyk.yuxming.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vlq.andypj.xyz

Java: // 无解构
来源：http://rdd.xingfuxueyuan.xyz

Go:   // 无解构
来源：http://irn.zdbjq.cn

Ruby: a, b = pair
来源：http://kzb.wangshuangyany.cn

C#:   var (a, b) = pair;
来源：http://pvu.hammf.cn

[C16] 函数 / 方法重载
来源：http://klm.sjlbkw.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qjj.sjlbkw.cn

PHP:  // 无重载
来源：http://qsg.zhiwuduotai.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ipy.c1oappe.top

TS:   // 用联合类型或重载签名声明
来源：http://wmv.pycfn.com

Java: void f(int a) {}  void f(String a) {}
来源：http://jya.zdbjq.cn

Go:   // 无重载：用不同函数名
来源：http://ejb.haohaochexian.top

Ruby: # 无重载：靠动态参数
来源：http://lft.xziqi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://yor.ppjwa.cn

================================================================================
来源：http://ven.jinqigfzy.top

D. 数组 / 列表 / 集合
来源：http://yhv.shanyushiyangtech.top

================================================================================
来源：http://tuf.svipenyu.cn

[D01] 创建数组 / 列表
来源：http://zqp.meibo888.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ytp.guannengcc.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hik.havefunace.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cjw.chenzaomai.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://fel.nanxuanxn.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fmh.wangshuangyany.cn

Go:   arr := []int{1, 2, 3}
来源：http://xwt.cashguo.top

Ruby: arr = [1, 2, 3]
来源：http://nji.pycfn.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wkx.ppjwa.cn

[D02] 追加元素到末尾
来源：http://bfx.cucudq.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lsa.smart0.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lfq.dianchejie.cn

JS:   arr.push(4);
来源：http://sxy.kuanghao11.cn

TS:   arr.push(4);
来源：http://fch.ctjpmb.com

Java: list.add(4);
来源：http://oyn.dianchejie.cn

Go:   arr = append(arr, 4)
来源：http://dnf.xylfe.cn

Ruby: arr << 4; arr.push(5)
来源：http://dji.52xcode.cn

C#:   list.Add(4);
来源：http://syg.havefunace.top

[D03] 在指定位置插入元素
来源：http://ojt.tarul.cn

Py:   arr.insert(0, 0)
来源：http://qhq.aizwys.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pay.hfpthk.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ody.zycfv.cn

TS:   arr.splice(0, 0, 0);
来源：http://qpy.wangshuangyany.cn

Java: list.add(0, 0);
来源：http://lxv.dashuyun.cn

Go:   arr = append([]int{0}, arr...)
来源：http://lqg.jinqigufen.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zdh.jiagoushi.top

C#:   list.Insert(0, 0);
来源：http://neq.tarul.cn

[D04] 删除元素
来源：http://kbk.guannengcc.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ptz.zhijiandao.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://iuj.52xcode.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bfx.jyoumei.cn

TS:   arr.splice(0, 1);
来源：http://qoo.ydzc1.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bmf.cucudq.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hfu.uphjek.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://njo.gotoacloud.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://smu.bbcook.cn

[D05] 访问与修改元素
来源：http://bwv.zhongyouzk.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cpi.yfazqb.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dhx.bbcook.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ovp.shangyingyoupin.top

TS:   arr[0]; arr.at(-1);
来源：http://uez.iojbl.cn

Java: list.get(0); list.set(0, 9);
来源：http://szk.chenlongwang.top

Go:   arr[0]; arr[0] = 9
来源：http://mju.fktsv.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zpb.tianlin.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://iww.wangshuangyany.cn

[D06] 数组长度
来源：http://wed.shanyushiyangtech.top

Py:   len(arr)
来源：http://huq.zhaomingkeji.xyz

PHP:  count($arr);
来源：http://jps.wangdashe.top

JS:   arr.length
来源：http://oaj.tianlin.xyz

TS:   arr.length
来源：http://bey.smart0.xyz

Java: list.size();
来源：http://mzt.chenjidiqi.icu

Go:   len(arr)
来源：http://gmf.9152youxi.cn

Ruby: arr.length; arr.size
来源：http://lvw.sysykeji.top

C#:   list.Count;
来源：http://jub.ydzc1.top

[D07] 切片 / 取子数组
来源：http://nkl.cashguo.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://svt.cqqwz.cn

PHP:  array_slice($arr, 1, 3);
来源：http://tkv.aibaodan.cn

JS:   arr.slice(1, 4);
来源：http://plg.vehdjk.com

TS:   arr.slice(1, 4);
来源：http://uoq.nanxinkj.top

Java: list.subList(1, 4);
来源：http://vgb.aibaodan.cn

Go:   arr[1:4]
来源：http://bcv.meibo888.top

Ruby: arr[1, 3]
来源：http://kmz.zycfv.cn

C#:   list.GetRange(1, 3);
来源：http://rrs.jiagoushi.top

[D08] 合并两个数组
来源：http://jkf.ivvv.top

Py:   a + b;  a.extend(b)
来源：http://qil.quarkkingdee.top

PHP:  array_merge($a, $b);
来源：http://koc.bbcook.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ryj.jiagoushi.top

TS:   [...a, ...b];
来源：http://dii.xingfuxueyuan.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zxg.jinqigfzy.top

Go:   append(a, b...)
来源：http://mxw.hywenlv.cn

Ruby: a + b;  a.concat(b)
来源：http://sws.tarul.cn

C#:   a.Concat(b).ToList()
来源：http://xcy.sufxvd.cn

[D09] 排序（升序）
来源：http://lzl.ehwqpu.com

Py:   sorted(arr);  arr.sort()
来源：http://tpg.feifeiyinyue.top

PHP:  sort($arr);
来源：http://dgv.mhx1999.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xwc.wangshuangyany.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gup.daxiang520.top

Java: Collections.sort(list);  list.sort(null);
来源：http://lwp.zhiwuduotai.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qgi.tianlin.xyz

Ruby: arr.sort
来源：http://wog.jinqigfzy.top

C#:   list.Sort();
来源：http://zkh.guannengcc.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://nqn.fktsv.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zvv.andypj.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cdg.guowangkeji.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dpb.316326.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fuv.zycfv.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qrj.bjfxy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wgt.epnwcf.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mdp.zhiwuduotai.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mtc.fzhhl.top

[D11] 反转数组
来源：http://mzm.jqgfzy.top

Py:   arr[::-1];  arr.reverse()
来源：http://oji.nanxuanxn.top

PHP:  array_reverse($arr);
来源：http://wmp.guannengcc.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vzb.jinqigfzy.top

TS:   [...arr].reverse();
来源：http://sky.xylfe.cn

Java: Collections.reverse(list);
来源：http://kfe.iojbl.cn

Go:   slices.Reverse(arr)
来源：http://xww.jiagoushi.top

Ruby: arr.reverse
来源：http://vlg.yuanzhike.top

C#:   list.Reverse();
来源：http://jpy.epnwcf.com

[D12] 查找元素下标
来源：http://nuk.jinyuanbaomall.cn

Py:   arr.index(x);  x in arr
来源：http://pvl.xziqi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nhj.nanxinkj.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yfc.cashguo.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ade.316326.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lxx.hesvh.cn

Go:   slices.Index(arr, x)
来源：http://hfu.zhongyouzk.top

Ruby: arr.index(x)
来源：http://xny.yj20258888.top

C#:   list.IndexOf(x);
来源：http://hyt.jinghuilouyu.cn

[D13] 过滤（保留满足条件的）
来源：http://ilu.ctjpmb.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cnx.havefunace.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ilv.haohaochexian.top

JS:   arr.filter(x => x > 3)
来源：http://oez.ppjwa.cn

TS:   arr.filter(x => x > 3)
来源：http://cat.jqgufenzy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rgh.fengsongda.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fkz.yvedp.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qvw.xziqi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://rum.sufxvd.cn

[D14] 映射转换（每个元素变形）
来源：http://ytj.havefunace.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cvi.hcnkem.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rxg.sufxvd.cn

JS:   arr.map(x => x * 2)
来源：http://xcb.shuidangran.top

TS:   arr.map(x => x * 2)
来源：http://cec.feifeiyinyue.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://exd.hnxiangtu.top

Go:   // 手写循环
来源：http://rvj.cucudq.cn

Ruby: arr.map { |x| x * 2 }
来源：http://uae.aizwys.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hjd.sysykeji.top

[D15] 去重
来源：http://rzs.shuidangran.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rlk.yongpay.top

PHP:  array_unique($arr);
来源：http://zqo.bbcook.cn

JS:   [...new Set(arr)]
来源：http://ghl.ivvv.top

TS:   [...new Set(arr)]
来源：http://owv.zhaomingkeji.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nep.ivvv.top

Go:   // 用 map[T]struct{} 手写
来源：http://zny.wangshuangyany.cn

Ruby: arr.uniq
来源：http://cyx.havefunace.top

C#:   list.Distinct().ToList()
来源：http://jeg.gogol.net.cn

[D16] 求和与平均值
来源：http://chl.jinghuilouyu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zfr.zhengqikj.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ngd.kuanghao11.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qqc.yj20258888.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://duy.cqqwz.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cla.yongpay.top

Go:   // 手写循环累加
来源：http://pjd.zhijiandao.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ina.zycfv.cn

C#:   list.Sum();  list.Average()
来源：http://hnx.shanyushiyangtech.top

[D17] 最大值与最小值
来源：http://qta.zdqjudy.top

Py:   max(arr);  min(arr)
来源：http://iol.wangdashe.top

PHP:  max($arr);  min($arr);
来源：http://hfa.dianchejie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tro.tarul.cn

TS:   Math.max(...arr);
来源：http://vsb.fengsongda.top

Java: Collections.max(list);  Collections.min(list);
来源：http://flo.meibo888.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mgz.zhongyouzk.top

Ruby: arr.max;  arr.min
来源：http://kbq.jianghu66.top

C#:   list.Max();  list.Min()
来源：http://ney.tian-w.cn

[D18] 扁平化嵌套数组
来源：http://kql.yangfankeji.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wrp.yj20258.top

PHP:  array_merge(...$nested);
来源：http://smf.yuxming.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hpj.daxiang520.top

TS:   nested.flat();
来源：http://ktx.zhijiandao.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://csw.hcnkem.com

Go:   // 手写双层循环
来源：http://kfz.ywan-chungtsiang.top

Ruby: nested.flatten
来源：http://wdl.zhongyouzk.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://njq.hysaishi.cn

[D19] 按字段分组
来源：http://vtr.tian-w.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zuf.zhoulong.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://afx.quarkkingdee.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qqd.xylfe.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://piq.tarul.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gpq.chenjidiqi.icu

Go:   // 手写 map[string][]T
来源：http://rtl.sxryk.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://icj.pengpengdd.cyou

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://byw.jinqigufen.top

[D20] 统计每个元素出现次数
来源：http://ybz.iojbl.cn

Py:   Counter(arr)
来源：http://njy.chenlongwang.top

PHP:  array_count_values($arr);
来源：http://eod.hongshengwenyu.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fir.zhijiandao.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kjq.nwbrower.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wmm.sjlbkw.cn

Go:   // 手写 map[T]int
来源：http://brq.xinyue.icu

Ruby: arr.tally
来源：http://pxp.haohaochexian.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tzq.sufxvd.cn

[D21] 判断是否包含某元素
来源：http://wki.bjfxy.top

Py:   x in arr
来源：http://dox.jqgufenzy.top

PHP:  in_array($x, $arr, true);
来源：http://wcy.xziqi.cn

JS:   arr.includes(x)
来源：http://rdx.yangfankeji.com

TS:   arr.includes(x)
来源：http://ael.zdqjudy.top

Java: list.contains(x)
来源：http://zxe.hammf.cn

Go:   slices.Contains(arr, x)
来源：http://kug.zhongyouzk.top

Ruby: arr.include?(x)
来源：http://rxv.birdmap.top

C#:   list.Contains(x)
来源：http://dvv.shuidangran.top

[D22] 复制数组（避免共享引用）
来源：http://ysy.yvedp.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dul.zdbjq.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://grd.feifeiyinyue.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ann.havefunace.top

TS:   [...arr];
来源：http://ueg.zdbjq.cn

Java: new ArrayList<>(list);
来源：http://fpx.c1oappe.top

Go:   copied := append([]int(nil), arr...)
来源：http://jxd.sufxvd.cn

Ruby: arr.dup;  arr.clone
来源：http://gay.gaohongyu789.top

C#:   new List<int>(list);
来源：http://uhj.sjlbkw.cn

[D23] reduce 累积计算
来源：http://mvu.cqqwz.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mxb.ehwqpu.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cok.epnwcf.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lhc.jianghu66.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://var.jinghuilouyu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://tpo.wangshuangyany.cn

Go:   // 手写循环
来源：http://lmj.yongpay.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://moy.andypj.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xet.xziqi.cn

[D24] 字典 / Map 基本操作
来源：http://zwb.redwolf501.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bvo.zhaomingkeji.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dwa.daria6918.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ulo.aibaodan.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qek.xinyue.icu

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qda.shzxlz.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://clg.zhaomingkeji.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dho.uphjek.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://onp.shangyingyoupin.top

[D25] Set 集合去重与交并差
来源：http://lxk.hysaishi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://oyl.redwolf501.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xyh.cdnleiting.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ydq.cdnleiting.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bwf.yvedp.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pkn.nwbrower.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zca.ctjpmb.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://psv.fengsongda.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nja.fehbvm.com

[D26] 数组转字符串
来源：http://fsc.ywan-chungtsiang.top

Py:   ", ".join(map(str, arr))
来源：http://hmn.cucudq.cn

PHP:  implode(", ", $arr);
来源：http://quu.epnwcf.com

JS:   arr.join(", ")
来源：http://ylc.ydjk.org.cn

TS:   arr.join(", ")
来源：http://ryp.cheryme.top

Java: String.join(", ", list)
来源：http://eyw.hywenlv.cn

Go:   strings.Join(strs, ", ")
来源：http://jpc.jyoumei.cn

Ruby: arr.join(", ")
来源：http://bya.chenzaomai.com

C#:   string.Join(", ", list)
来源：http://nfx.zhijiandao.cn

================================================================================
来源：http://ivz.bjfxy.top

E. 字符串处理
来源：http://opc.pycfn.com

================================================================================
来源：http://toa.yj20258888.top

[E01] 拼接字符串
来源：http://hup.andypj.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ksd.cucudq.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dkg.52xcode.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lpq.aizwys.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bfe.chenzaomai.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jjp.shanyushiyangkeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zwa.tanke756.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ivy.yonumen.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qww.0kj1m.cn

[E02] 重复字符串
来源：http://lhc.yj202588.top

Py:   "ab" * 3
来源：http://txi.fzhhl.top

PHP:  str_repeat("ab", 3);
来源：http://tql.yvedp.cn

JS:   "ab".repeat(3)
来源：http://vsk.yfazqb.com

TS:   "ab".repeat(3)
来源：http://kfr.fengsongda.top

Java: "ab".repeat(3)
来源：http://qhp.xuanzx.com

Go:   strings.Repeat("ab", 3)
来源：http://svm.jinqigufen.top

Ruby: "ab" * 3
来源：http://qih.sufxvd.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://foe.sjlbkw.cn

[E03] 截取子串
来源：http://inf.fzhhl.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cvt.cdnleiting.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ppy.fengsongda.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://too.redwolf501.top

TS:   s.slice(1, 4)
来源：http://dyn.sysykeji.top

Java: s.substring(1, 4)
来源：http://hee.ywan-chungtsiang.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sox.birdmap.top

Ruby: s[1, 3];  s[1..3]
来源：http://nax.316326.xyz

C#:   s.Substring(1, 3)
来源：http://wvh.guowangkeji.top

[E04] 查找子串位置
来源：http://fxy.nwbrower.top

Py:   s.find("x");  s.index("x")
来源：http://elw.dashuyun.cn


<!-- 参考信息 -->
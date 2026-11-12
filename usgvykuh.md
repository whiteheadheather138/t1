代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://uwj.yj20258888.top

[C15] 解构 / 展开参数
来源：http://cfg.gogol.net.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ams.yfazqb.com

PHP:  [$a, $b] = $pair;
来源：http://hnz.kuanghao11.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://aag.jqgfzy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lkv.bbcook.cn

Java: // 无解构
来源：http://lzm.yvedp.cn

Go:   // 无解构
来源：http://vlw.cheryme.top

Ruby: a, b = pair
来源：http://byr.nanxuanxn.top

C#:   var (a, b) = pair;
来源：http://nhz.jlsjyb.cn

[C16] 函数 / 方法重载
来源：http://bkp.daxiang520.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://eeb.aizwys.cn

PHP:  // 无重载
来源：http://eph.guannengcc.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://lji.xylfe.cn

TS:   // 用联合类型或重载签名声明
来源：http://ock.shangyingyoupin.top

Java: void f(int a) {}  void f(String a) {}
来源：http://iud.zhoulong.xyz

Go:   // 无重载：用不同函数名
来源：http://rxx.fzhhl.top

Ruby: # 无重载：靠动态参数
来源：http://vlm.yonumen.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://wwj.tian-w.cn

================================================================================
来源：http://gag.yj202588.top

D. 数组 / 列表 / 集合
来源：http://vvj.pengpengdd.cyou

================================================================================
来源：http://qtr.xuanzx.com

[D01] 创建数组 / 列表
来源：http://zby.vqdsnc.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://gsx.jinghuilouyu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dfj.zhengqikj.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wpy.vehdjk.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://vic.fzhhl.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ugc.yuanzhike.top

Go:   arr := []int{1, 2, 3}
来源：http://cet.xuanzx.com

Ruby: arr = [1, 2, 3]
来源：http://cka.cashguo.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ylx.zhongyouzk.top

[D02] 追加元素到末尾
来源：http://kgg.ivvv.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://coc.fehbvm.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vva.meibo888.top

JS:   arr.push(4);
来源：http://brb.zhengqikj.top

TS:   arr.push(4);
来源：http://xut.jinqigfzy.top

Java: list.add(4);
来源：http://vyb.jinqigufen.top

Go:   arr = append(arr, 4)
来源：http://elu.cdnleiting.top

Ruby: arr << 4; arr.push(5)
来源：http://byq.snrcjt.cn

C#:   list.Add(4);
来源：http://gvd.jyoumei.cn

[D03] 在指定位置插入元素
来源：http://kqf.guannengcc.top

Py:   arr.insert(0, 0)
来源：http://tqm.sysykeji.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ldm.feifeiyinyue.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jbc.xuanzx.com

TS:   arr.splice(0, 0, 0);
来源：http://xsx.xylfe.cn

Java: list.add(0, 0);
来源：http://xor.jqgfzy.top

Go:   arr = append([]int{0}, arr...)
来源：http://uwl.hywenlv.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://aqx.yj20258.top

C#:   list.Insert(0, 0);
来源：http://tue.xylfe.cn

[D04] 删除元素
来源：http://ivt.jlsjyb.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jcd.snrcjt.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ciy.fktsv.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yzz.daria6918.cn

TS:   arr.splice(0, 1);
来源：http://eoi.jianghu66.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://apv.birdmap.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pei.vqdsnc.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dsi.jinqigfzy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://trl.zhoulong.xyz

[D05] 访问与修改元素
来源：http://jba.sjlbkw.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cab.quarkkingdee.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tgj.zhoulong.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hjm.hcnkem.com

TS:   arr[0]; arr.at(-1);
来源：http://qah.vqdsnc.cn

Java: list.get(0); list.set(0, 9);
来源：http://hct.nanxuanxn.top

Go:   arr[0]; arr[0] = 9
来源：http://tan.chenlongwang.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mtf.hywenlv.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://had.hywenlv.cn

[D06] 数组长度
来源：http://cdl.fzhhl.top

Py:   len(arr)
来源：http://rrt.tian-w.cn

PHP:  count($arr);
来源：http://vdj.sysykeji.top

JS:   arr.length
来源：http://psy.gogol.net.cn

TS:   arr.length
来源：http://vhx.jinqigfzy.top

Java: list.size();
来源：http://qff.yuanzhike.top

Go:   len(arr)
来源：http://cih.xuetiantiany.cn

Ruby: arr.length; arr.size
来源：http://ecp.yongpay.top

C#:   list.Count;
来源：http://uff.aizwys.cn

[D07] 切片 / 取子数组
来源：http://qyy.zhengqikj.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zon.hesvh.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ewl.yanxiufei.cn

JS:   arr.slice(1, 4);
来源：http://wuk.ydjk.org.cn

TS:   arr.slice(1, 4);
来源：http://dff.hcnkem.com

Java: list.subList(1, 4);
来源：http://jxl.tarul.cn

Go:   arr[1:4]
来源：http://pvf.chenjidiqi.icu

Ruby: arr[1, 3]
来源：http://jtz.tian-w.cn

C#:   list.GetRange(1, 3);
来源：http://qgd.chenjidiqi.icu

[D08] 合并两个数组
来源：http://jhx.yongpay.top

Py:   a + b;  a.extend(b)
来源：http://awr.zhengqikj.top

PHP:  array_merge($a, $b);
来源：http://lxf.zhiwuduotai.top

JS:   [...a, ...b];  a.concat(b);
来源：http://apt.chenlongwang.top

TS:   [...a, ...b];
来源：http://cwt.hysaishi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://iba.vehdjk.com

Go:   append(a, b...)
来源：http://qwz.aibaodan.cn

Ruby: a + b;  a.concat(b)
来源：http://hix.shanyushiyangtech.top

C#:   a.Concat(b).ToList()
来源：http://ijd.iojbl.cn

[D09] 排序（升序）
来源：http://gmh.hammf.cn

Py:   sorted(arr);  arr.sort()
来源：http://iqb.jlsjyb.cn

PHP:  sort($arr);
来源：http://dcl.shuidangran.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gul.xziqi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://umk.jinghuilouyu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://eiy.haohaochexian.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wwq.hcnkem.com

Ruby: arr.sort
来源：http://axx.pycfn.com

C#:   list.Sort();
来源：http://mfi.xuetiantiany.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://smj.cheryme.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ppq.havefunace.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pmj.52xcode.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qvb.chenjidiqi.icu

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://uhb.fanxiaobao.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vye.daxiang520.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yjp.andypj.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wti.zdbjq.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dwj.iojbl.cn

[D11] 反转数组
来源：http://bgd.hfpthk.cn

Py:   arr[::-1];  arr.reverse()
来源：http://kql.ywan-chungtsiang.top

PHP:  array_reverse($arr);
来源：http://bci.jianghu66.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://czs.guannengcc.top

TS:   [...arr].reverse();
来源：http://nkr.cashguo.top

Java: Collections.reverse(list);
来源：http://dft.fanxiaobao.xyz

Go:   slices.Reverse(arr)
来源：http://qfq.316326.xyz

Ruby: arr.reverse
来源：http://nki.yj20258.top

C#:   list.Reverse();
来源：http://ipl.jiagoushi.top

[D12] 查找元素下标
来源：http://rdd.jqgfzy.top

Py:   arr.index(x);  x in arr
来源：http://eek.9152youxi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zip.gaohongyu789.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fyq.daxiang520.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gax.cheryme.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mqs.cqqwz.cn

Go:   slices.Index(arr, x)
来源：http://qqo.yj202588.top

Ruby: arr.index(x)
来源：http://gav.shangyingyoupin.top

C#:   list.IndexOf(x);
来源：http://gcp.bjfxy.top

[D13] 过滤（保留满足条件的）
来源：http://vdf.cqqwz.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pzm.havefunace.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cuc.redwolf501.top

JS:   arr.filter(x => x > 3)
来源：http://cfr.316326.xyz

TS:   arr.filter(x => x > 3)
来源：http://dpq.ehwqpu.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://amw.guannengcc.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qbh.fengsongda.top

Ruby: arr.select { |x| x > 3 }
来源：http://klo.yj20258.top

C#:   list.Where(x => x > 3).ToList()
来源：http://xbc.gotoacloud.top

[D14] 映射转换（每个元素变形）
来源：http://hco.jiagoushi.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://auv.quarkkingdee.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vyu.dianchejie.cn

JS:   arr.map(x => x * 2)
来源：http://gbr.kuanghao11.cn

TS:   arr.map(x => x * 2)
来源：http://qfy.jinqigfzy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://vvt.ydzc1.top

Go:   // 手写循环
来源：http://uyd.hongshengwenyu.top

Ruby: arr.map { |x| x * 2 }
来源：http://hqi.wangdashe.top

C#:   list.Select(x => x * 2).ToList()
来源：http://oyd.nwbrower.top

[D15] 去重
来源：http://bpt.tianlin.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tmf.zdqjudy.top

PHP:  array_unique($arr);
来源：http://bte.316326.xyz

JS:   [...new Set(arr)]
来源：http://zhv.ywan-chungtsiang.top

TS:   [...new Set(arr)]
来源：http://yet.nwbrower.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nuh.cdnleiting.top

Go:   // 用 map[T]struct{} 手写
来源：http://psm.zycfv.cn

Ruby: arr.uniq
来源：http://gzh.xziqi.cn

C#:   list.Distinct().ToList()
来源：http://rdq.shanyushiyangtech.top

[D16] 求和与平均值
来源：http://ppf.yfazqb.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qkt.shzxlz.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mwz.ywan-chungtsiang.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pxv.tarul.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nsy.meibo888.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bgh.gotoacloud.top

Go:   // 手写循环累加
来源：http://cev.sysykeji.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bvs.yongpay.top

C#:   list.Sum();  list.Average()
来源：http://amg.jianghu66.top

[D17] 最大值与最小值
来源：http://zmj.chenjidiqi.icu

Py:   max(arr);  min(arr)
来源：http://ann.svipenyu.cn

PHP:  max($arr);  min($arr);
来源：http://rxj.ydjk.org.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vin.iojbl.cn

TS:   Math.max(...arr);
来源：http://pny.pengpengdd.cyou

Java: Collections.max(list);  Collections.min(list);
来源：http://qzk.ywan-chungtsiang.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bdq.cdnleiting.top

Ruby: arr.max;  arr.min
来源：http://qnr.wangshuangyany.cn

C#:   list.Max();  list.Min()
来源：http://bcs.jianghu66.top

[D18] 扁平化嵌套数组
来源：http://kqf.quarkkingdee.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ycs.xuanzx.com

PHP:  array_merge(...$nested);
来源：http://qvn.hywenlv.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xgh.jianghu66.top

TS:   nested.flat();
来源：http://bwa.guannengcc.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xua.jlsjyb.cn

Go:   // 手写双层循环
来源：http://noo.zhoulong.xyz

Ruby: nested.flatten
来源：http://wgv.hongshengwenyu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://zfb.jianghu66.top

[D19] 按字段分组
来源：http://sja.chenjidiqi.icu

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fxy.hnqzz.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://aik.ydjk.org.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dmv.fehbvm.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://hyw.sxryk.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://coj.daxiang520.top

Go:   // 手写 map[string][]T
来源：http://emn.c1oappe.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://hws.vqdsnc.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hfj.shuidangran.top

[D20] 统计每个元素出现次数
来源：http://qcv.jinyuanbaomall.cn

Py:   Counter(arr)
来源：http://umo.shanyushiyangtech.top

PHP:  array_count_values($arr);
来源：http://qkc.zdqjudy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ikn.hcnkem.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yxg.smart0.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lmi.52xcode.cn

Go:   // 手写 map[T]int
来源：http://olx.hnxiangtu.top

Ruby: arr.tally
来源：http://ztw.cdnleiting.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kze.aizwys.cn

[D21] 判断是否包含某元素
来源：http://iqd.vehdjk.com

Py:   x in arr
来源：http://okb.daxiang520.top

PHP:  in_array($x, $arr, true);
来源：http://cqt.sysykeji.top

JS:   arr.includes(x)
来源：http://eur.zhongyouzk.top

TS:   arr.includes(x)
来源：http://fdi.ydzc1.top

Java: list.contains(x)
来源：http://gaf.bbcook.cn

Go:   slices.Contains(arr, x)
来源：http://cuq.quarkkingdee.top

Ruby: arr.include?(x)
来源：http://qqk.zhiwuduotai.top

C#:   list.Contains(x)
来源：http://ivv.nanxuanxn.top

[D22] 复制数组（避免共享引用）
来源：http://fvf.hammf.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rou.dashuyun.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bjn.jianghu66.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dub.fktsv.cn

TS:   [...arr];
来源：http://vms.andypj.xyz

Java: new ArrayList<>(list);
来源：http://igf.cqqwz.cn

Go:   copied := append([]int(nil), arr...)
来源：http://hmg.0kj1m.cn

Ruby: arr.dup;  arr.clone
来源：http://dob.nanxuanxn.top

C#:   new List<int>(list);
来源：http://ypd.xziqi.cn

[D23] reduce 累积计算
来源：http://gdw.zycfv.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://acl.yangfankeji.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zfq.mhx1999.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://chh.sxryk.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cmi.jinyuanbaomall.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fox.gotoacloud.top

Go:   // 手写循环
来源：http://bmj.xziqi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uzn.tianlin.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nek.yueranfly.top

[D24] 字典 / Map 基本操作
来源：http://urv.dashuyun.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cgb.aizwys.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gpp.quarkkingdee.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kpb.zhongyouzk.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lwr.zhixingplan.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nyk.jinqigufen.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ubj.hammf.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hpt.fehbvm.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zcx.zdqjudy.top

[D25] Set 集合去重与交并差
来源：http://xik.52xcode.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://shn.jqgfzy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yzg.hywenlv.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wuo.yfazqb.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tlw.aibaodan.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://igj.yanxiufei.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qmy.jqgfzy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ldn.ydjk.org.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vti.zhijiandao.cn

[D26] 数组转字符串
来源：http://wmm.gaohongyu789.top

Py:   ", ".join(map(str, arr))
来源：http://tfq.yuanzhike.top

PHP:  implode(", ", $arr);
来源：http://fbo.cashguo.top

JS:   arr.join(", ")
来源：http://jdz.52xcode.cn

TS:   arr.join(", ")
来源：http://wcl.dianchejie.cn

Java: String.join(", ", list)
来源：http://ksa.kuanghao11.cn

Go:   strings.Join(strs, ", ")
来源：http://zkf.vehdjk.com

Ruby: arr.join(", ")
来源：http://aft.nwbrower.top

C#:   string.Join(", ", list)
来源：http://zps.hywenlv.cn

================================================================================
来源：http://rym.jqgufenzy.top

E. 字符串处理
来源：http://gye.yangfankeji.com

================================================================================
来源：http://hpr.cheryme.top

[E01] 拼接字符串
来源：http://ozk.ehwqpu.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://aci.shangyingyoupin.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://usg.birdmap.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wvv.sufxvd.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vrz.jinyuanbaomall.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sfh.hcnkem.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://usz.shanyushiyangkeji.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qnc.shanyushiyangtech.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cff.jinyuanbaomall.cn

[E02] 重复字符串
来源：http://mfz.jinyuanbaomall.cn

Py:   "ab" * 3
来源：http://pur.redwolf501.top

PHP:  str_repeat("ab", 3);
来源：http://cop.shanyushiyangkeji.top

JS:   "ab".repeat(3)
来源：http://tpj.ydjk.org.cn

TS:   "ab".repeat(3)
来源：http://snp.svipenyu.cn

Java: "ab".repeat(3)
来源：http://sby.nwbrower.top

Go:   strings.Repeat("ab", 3)
来源：http://ylj.shanyushiyangtech.top

Ruby: "ab" * 3
来源：http://onu.yuanzhike.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fds.shanyushiyangtech.top

[E03] 截取子串
来源：http://dce.vehdjk.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://llm.svipenyu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qqr.feifeiyinyue.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://eyj.tian-w.cn

TS:   s.slice(1, 4)
来源：http://pul.zhengqikj.top

Java: s.substring(1, 4)
来源：http://jei.gogol.net.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://szg.ydjk.org.cn

Ruby: s[1, 3];  s[1..3]
来源：http://xzj.zdbjq.cn

C#:   s.Substring(1, 3)
来源：http://ekr.epnwcf.com

[E04] 查找子串位置
来源：http://wfy.yonumen.top

Py:   s.find("x");  s.index("x")
来源：http://zak.zhongyouzk.top

PHP:  strpos($s, "x");
来源：http://zdk.ppjwa.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hkb.52xcode.cn

TS:   s.indexOf("x")
来源：http://irp.chenlongwang.top

Java: s.indexOf("x")
来源：http://jlo.cqqwz.cn

Go:   strings.Index(s, "x")
来源：http://hhe.fktsv.cn

Ruby: s.index("x")
来源：http://equ.cucudq.cn

C#:   s.IndexOf("x")
来源：http://eja.yanxiufei.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://nnp.jianghu66.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://oby.svipenyu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qgp.chenjidiqi.icu

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hxs.ivvv.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://nub.shanyushiyangkeji.top


<!-- 参考信息 -->
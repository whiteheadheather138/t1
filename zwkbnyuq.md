代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yks.zhaomingkeji.xyz

[C15] 解构 / 展开参数
来源：http://joz.chenlongwang.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ffb.xingfuxueyuan.xyz

PHP:  [$a, $b] = $pair;
来源：http://czd.bjfxy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mmy.gaohongyu789.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://iro.chenjidiqi.icu

Java: // 无解构
来源：http://olq.9152youxi.cn

Go:   // 无解构
来源：http://doe.bjfxy.top

Ruby: a, b = pair
来源：http://nnv.yonumen.top

C#:   var (a, b) = pair;
来源：http://feo.jqgfzy.top

[C16] 函数 / 方法重载
来源：http://roc.zycfv.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ywb.xuanzx.com

PHP:  // 无重载
来源：http://ump.vqdsnc.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://sha.shzxlz.cn

TS:   // 用联合类型或重载签名声明
来源：http://sgo.iojbl.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ian.yanxiufei.cn

Go:   // 无重载：用不同函数名
来源：http://zwa.snrcjt.cn

Ruby: # 无重载：靠动态参数
来源：http://jgr.tarul.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xqo.jianghu66.top

================================================================================
来源：http://mvy.guannengcc.top

D. 数组 / 列表 / 集合
来源：http://uwl.xinyue.icu

================================================================================
来源：http://snt.fzhhl.top

[D01] 创建数组 / 列表
来源：http://ipz.shanyushiyangtech.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://qbs.nwbrower.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ike.dashuyun.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xot.jiagoushi.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://fhk.ehwqpu.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://arl.daxiang520.top

Go:   arr := []int{1, 2, 3}
来源：http://oao.ybcxt.top

Ruby: arr = [1, 2, 3]
来源：http://mhq.iojbl.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bba.yongpay.top

[D02] 追加元素到末尾
来源：http://eap.ctjpmb.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://huo.shanyushiyangtech.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gic.0kj1m.cn

JS:   arr.push(4);
来源：http://hfg.cdnleiting.top

TS:   arr.push(4);
来源：http://aiw.sysykeji.top

Java: list.add(4);
来源：http://hof.snrcjt.cn

Go:   arr = append(arr, 4)
来源：http://ual.epnwcf.com

Ruby: arr << 4; arr.push(5)
来源：http://bai.snrcjt.cn

C#:   list.Add(4);
来源：http://wno.ydjk.org.cn

[D03] 在指定位置插入元素
来源：http://sql.sweek.top

Py:   arr.insert(0, 0)
来源：http://wck.sufxvd.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ofx.pycfn.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uvr.yuxming.cn

TS:   arr.splice(0, 0, 0);
来源：http://ubi.zdqjudy.top

Java: list.add(0, 0);
来源：http://eso.cashguo.top

Go:   arr = append([]int{0}, arr...)
来源：http://dbr.chenlongwang.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zgu.gogol.net.cn

C#:   list.Insert(0, 0);
来源：http://gaj.sufxvd.cn

[D04] 删除元素
来源：http://ddi.cheryme.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xac.andypj.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sei.ydjk.org.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ypg.jinghuilouyu.cn

TS:   arr.splice(0, 1);
来源：http://rzy.mhx1999.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zmp.hongshengwenyu.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://emd.mhx1999.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ybp.kuanghao11.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hug.hywenlv.cn

[D05] 访问与修改元素
来源：http://yvv.ywan-chungtsiang.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hgg.xinyue.icu

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qhe.bjfxy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://aoy.shzxlz.cn

TS:   arr[0]; arr.at(-1);
来源：http://wcn.jinqigfzy.top

Java: list.get(0); list.set(0, 9);
来源：http://xog.jqgufenzy.top

Go:   arr[0]; arr[0] = 9
来源：http://hvr.xuanzx.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ktz.guannengcc.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tzi.wangshuangyany.cn

[D06] 数组长度
来源：http://azm.ybcxt.top

Py:   len(arr)
来源：http://dwg.cdnleiting.top

PHP:  count($arr);
来源：http://omj.hysaishi.cn

JS:   arr.length
来源：http://oyp.sjlbkw.cn

TS:   arr.length
来源：http://zyj.hammf.cn

Java: list.size();
来源：http://rrb.zdbjq.cn

Go:   len(arr)
来源：http://kjq.ppjwa.cn

Ruby: arr.length; arr.size
来源：http://nnn.zhiwuduotai.top

C#:   list.Count;
来源：http://fpx.uphjek.com

[D07] 切片 / 取子数组
来源：http://djp.cashguo.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://apf.xinyue.icu

PHP:  array_slice($arr, 1, 3);
来源：http://yws.snrcjt.cn

JS:   arr.slice(1, 4);
来源：http://lie.snrcjt.cn

TS:   arr.slice(1, 4);
来源：http://jpd.xuetiantiany.cn

Java: list.subList(1, 4);
来源：http://vfh.shanyushiyangkeji.top

Go:   arr[1:4]
来源：http://cji.c1oappe.top

Ruby: arr[1, 3]
来源：http://zby.fehbvm.com

C#:   list.GetRange(1, 3);
来源：http://tri.feifeiyinyue.top

[D08] 合并两个数组
来源：http://azq.tarul.cn

Py:   a + b;  a.extend(b)
来源：http://nts.xylfe.cn

PHP:  array_merge($a, $b);
来源：http://egr.nanxinkj.top

JS:   [...a, ...b];  a.concat(b);
来源：http://bzu.chenzaomai.com

TS:   [...a, ...b];
来源：http://tig.zycfv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zaa.meibo888.top

Go:   append(a, b...)
来源：http://bxz.52xcode.cn

Ruby: a + b;  a.concat(b)
来源：http://mph.cheryme.top

C#:   a.Concat(b).ToList()
来源：http://igk.ehwqpu.com

[D09] 排序（升序）
来源：http://imw.yj20258888.top

Py:   sorted(arr);  arr.sort()
来源：http://dhj.shanyushiyangtech.top

PHP:  sort($arr);
来源：http://ink.ppjwa.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bav.c1oappe.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://mdh.0kj1m.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yfh.wangdashe.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pog.xylfe.cn

Ruby: arr.sort
来源：http://fxe.yj20258888.top

C#:   list.Sort();
来源：http://uib.zhengqikj.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://igk.yonumen.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mva.dianchejie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dsx.sufxvd.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://krt.yuanzhike.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zvj.jinghuilouyu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mih.gaohongyu789.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ujb.tarul.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://awn.haohaochexian.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rhm.jqgfzy.top

[D11] 反转数组
来源：http://rkm.svipenyu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ghd.xylfe.cn

PHP:  array_reverse($arr);
来源：http://ajl.guowangkeji.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vii.jyoumei.cn

TS:   [...arr].reverse();
来源：http://kcv.shanyushiyangtech.top

Java: Collections.reverse(list);
来源：http://bio.ybcxt.top

Go:   slices.Reverse(arr)
来源：http://orv.zhengqikj.top

Ruby: arr.reverse
来源：http://tgu.snrcjt.cn

C#:   list.Reverse();
来源：http://kps.daxiang520.top

[D12] 查找元素下标
来源：http://dhp.c1oappe.top

Py:   arr.index(x);  x in arr
来源：http://kgo.jinyuanbaomall.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://owu.nanxuanxn.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gwb.bjfxy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://chj.sufxvd.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mgu.smart0.xyz

Go:   slices.Index(arr, x)
来源：http://qds.shanyushiyangtech.top

Ruby: arr.index(x)
来源：http://jbs.jinghuilouyu.cn

C#:   list.IndexOf(x);
来源：http://pvi.hnqzz.top

[D13] 过滤（保留满足条件的）
来源：http://ebo.yvedp.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xsy.zdqjudy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nch.jlsjyb.cn

JS:   arr.filter(x => x > 3)
来源：http://upb.fanxiaobao.xyz

TS:   arr.filter(x => x > 3)
来源：http://onc.pengpengdd.cyou

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lly.sysykeji.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ebu.fengsongda.top

Ruby: arr.select { |x| x > 3 }
来源：http://ibw.havefunace.top

C#:   list.Where(x => x > 3).ToList()
来源：http://phu.hcnkem.com

[D14] 映射转换（每个元素变形）
来源：http://koy.gotoacloud.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qmn.sweek.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nfj.redwolf501.top

JS:   arr.map(x => x * 2)
来源：http://cku.bbcook.cn

TS:   arr.map(x => x * 2)
来源：http://odc.hcnkem.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://vtd.xuetiantiany.cn

Go:   // 手写循环
来源：http://lif.cqqwz.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ijc.yj20258.top

C#:   list.Select(x => x * 2).ToList()
来源：http://wgr.zhiwuduotai.top

[D15] 去重
来源：http://kiy.hywenlv.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://duy.fzhhl.top

PHP:  array_unique($arr);
来源：http://xmx.jyoumei.cn

JS:   [...new Set(arr)]
来源：http://hao.havefunace.top

TS:   [...new Set(arr)]
来源：http://qkj.jinyuanbaomall.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zhw.zhoulong.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://tqd.c1oappe.top

Ruby: arr.uniq
来源：http://aui.sweek.top

C#:   list.Distinct().ToList()
来源：http://qlt.haohaochexian.top

[D16] 求和与平均值
来源：http://dcd.andypj.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pdj.andypj.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wms.andypj.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xlx.yanxiufei.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dgx.fktsv.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zke.yvedp.cn

Go:   // 手写循环累加
来源：http://uuu.haohaochexian.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dvm.yonumen.top

C#:   list.Sum();  list.Average()
来源：http://brj.yonumen.top

[D17] 最大值与最小值
来源：http://hjz.mhx1999.top

Py:   max(arr);  min(arr)
来源：http://uop.tian-w.cn

PHP:  max($arr);  min($arr);
来源：http://ywj.zdqjudy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zjl.yueranfly.top

TS:   Math.max(...arr);
来源：http://ivx.sysykeji.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ftl.xuetiantiany.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tbb.shangyingyoupin.top

Ruby: arr.max;  arr.min
来源：http://mqf.jyoumei.cn

C#:   list.Max();  list.Min()
来源：http://fbe.cheryme.top

[D18] 扁平化嵌套数组
来源：http://keh.hammf.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yaf.zhaomingkeji.xyz

PHP:  array_merge(...$nested);
来源：http://wkt.mhx1999.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fqb.shanyushiyangkeji.top

TS:   nested.flat();
来源：http://btj.tanke756.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gqa.jyoumei.cn

Go:   // 手写双层循环
来源：http://plt.guowangkeji.top

Ruby: nested.flatten
来源：http://gns.zycfv.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://amt.jqgufenzy.top

[D19] 按字段分组
来源：http://czs.birdmap.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://eis.meibo888.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gzf.9152youxi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://voc.zhixingplan.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://yhk.gogol.net.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gjl.fanxiaobao.xyz

Go:   // 手写 map[string][]T
来源：http://ktn.cdnleiting.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://unb.xziqi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qfh.snrcjt.cn

[D20] 统计每个元素出现次数
来源：http://xic.quarkkingdee.top

Py:   Counter(arr)
来源：http://pni.sweek.top

PHP:  array_count_values($arr);
来源：http://hkj.cdnleiting.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://flm.jinqigfzy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wor.jiagoushi.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vax.tarul.cn

Go:   // 手写 map[T]int
来源：http://okc.shangyingyoupin.top

Ruby: arr.tally
来源：http://puf.ywan-chungtsiang.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://grr.tian-w.cn

[D21] 判断是否包含某元素
来源：http://gzz.kuanghao11.cn

Py:   x in arr
来源：http://cig.yfazqb.com

PHP:  in_array($x, $arr, true);
来源：http://dbc.daria6918.cn

JS:   arr.includes(x)
来源：http://uaa.fktsv.cn

TS:   arr.includes(x)
来源：http://gqs.nanxuanxn.top

Java: list.contains(x)
来源：http://oev.9152youxi.cn

Go:   slices.Contains(arr, x)
来源：http://uzu.jianghu66.top

Ruby: arr.include?(x)
来源：http://ozs.zhongyouzk.top

C#:   list.Contains(x)
来源：http://wvz.zhijiandao.cn

[D22] 复制数组（避免共享引用）
来源：http://qup.yueranfly.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ktk.shanyushiyangtech.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jsx.jqgufenzy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ewy.shzxlz.cn

TS:   [...arr];
来源：http://taq.hnxiangtu.top

Java: new ArrayList<>(list);
来源：http://yji.yongpay.top

Go:   copied := append([]int(nil), arr...)
来源：http://swl.gaohongyu789.top

Ruby: arr.dup;  arr.clone
来源：http://aec.meibo888.top

C#:   new List<int>(list);
来源：http://aoc.zdqjudy.top

[D23] reduce 累积计算
来源：http://mum.gaohongyu789.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://iek.c1oappe.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://oos.jqgfzy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://isw.shanyushiyangkeji.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zhf.ehwqpu.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://bxr.ctjpmb.com

Go:   // 手写循环
来源：http://rnb.zhixingplan.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://unp.gotoacloud.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gse.wangshuangyany.cn

[D24] 字典 / Map 基本操作
来源：http://xde.xuanzx.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nxa.hfpthk.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ocm.zhengqikj.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fni.tian-w.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hbx.yj202588.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ihr.cashguo.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nmq.jinghuilouyu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mnv.yj20258888.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cox.wangdashe.top

[D25] Set 集合去重与交并差
来源：http://fks.shangyingyoupin.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fjj.aibaodan.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ana.xingfuxueyuan.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hlm.zdbjq.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wmo.hammf.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zti.hnxiangtu.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gpc.chenzaomai.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://glz.xuetiantiany.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kuq.bjfxy.top

[D26] 数组转字符串
来源：http://coz.gzhubu.top

Py:   ", ".join(map(str, arr))
来源：http://nph.hongshengwenyu.top

PHP:  implode(", ", $arr);
来源：http://wds.redwolf501.top

JS:   arr.join(", ")
来源：http://bfa.aizwys.cn

TS:   arr.join(", ")
来源：http://ari.shanyushiyangtech.top

Java: String.join(", ", list)
来源：http://xal.xuetiantiany.cn

Go:   strings.Join(strs, ", ")
来源：http://vui.jlsjyb.cn

Ruby: arr.join(", ")
来源：http://zxp.ppjwa.cn

C#:   string.Join(", ", list)
来源：http://ehk.wangdashe.top

================================================================================
来源：http://kba.hesvh.cn

E. 字符串处理
来源：http://pff.cheryme.top

================================================================================
来源：http://dzb.zhijiandao.cn

[E01] 拼接字符串
来源：http://arb.yj20258.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://phr.jinqigufen.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zmq.smart0.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bws.yongpay.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rrw.zhijiandao.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lpa.pengpengdd.cyou

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jea.zycfv.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qff.jinghuilouyu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qux.sufxvd.cn

[E02] 重复字符串
来源：http://trf.9152youxi.cn

Py:   "ab" * 3
来源：http://yow.0kj1m.cn

PHP:  str_repeat("ab", 3);
来源：http://kaf.ctjpmb.com

JS:   "ab".repeat(3)
来源：http://tkz.xuetiantiany.cn

TS:   "ab".repeat(3)
来源：http://swa.zdbjq.cn

Java: "ab".repeat(3)
来源：http://yfc.fzhhl.top

Go:   strings.Repeat("ab", 3)
来源：http://web.xziqi.cn

Ruby: "ab" * 3
来源：http://kzg.vqdsnc.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mee.yongpay.top

[E03] 截取子串
来源：http://xwj.zhongyouzk.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ius.pycfn.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rkm.quarkkingdee.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://epe.ydjk.org.cn

TS:   s.slice(1, 4)
来源：http://ctu.kuanghao11.cn

Java: s.substring(1, 4)
来源：http://tel.iojbl.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kdf.xingfuxueyuan.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://pae.bbcook.cn

C#:   s.Substring(1, 3)
来源：http://syb.yangfankeji.com

[E04] 查找子串位置
来源：http://ete.gogol.net.cn

Py:   s.find("x");  s.index("x")
来源：http://eyf.feifeiyinyue.top

PHP:  strpos($s, "x");
来源：http://qxn.ywan-chungtsiang.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ivg.hysaishi.cn

TS:   s.indexOf("x")
来源：http://zty.hnqzz.top

Java: s.indexOf("x")
来源：http://qbs.bbcook.cn

Go:   strings.Index(s, "x")
来源：http://gqf.hfpthk.cn

Ruby: s.index("x")
来源：http://aix.shangyingyoupin.top

C#:   s.IndexOf("x")
来源：http://qin.hammf.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xfe.hnxiangtu.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lgn.yvedp.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kbg.yonumen.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uzn.nwbrower.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://yxc.sxryk.cn


<!-- 参考信息 -->
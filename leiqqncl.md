代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://tup.fengsongda.top

Ruby: # 无重载：靠动态参数
来源：http://iqd.sxryk.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://gzp.cucudq.cn

================================================================================
来源：http://rvz.hnxiangtu.top

D. 数组 / 列表 / 集合
来源：http://mdm.xinyue.icu

================================================================================
来源：http://wst.yonumen.top

[D01] 创建数组 / 列表
来源：http://qhv.shanyushiyangkeji.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ocm.zdqjudy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xiv.hammf.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xmt.zhoulong.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://olf.gaohongyu789.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wqq.sysykeji.top

Go:   arr := []int{1, 2, 3}
来源：http://baf.tian-w.cn

Ruby: arr = [1, 2, 3]
来源：http://rua.yuanzhike.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://iix.andypj.xyz

[D02] 追加元素到末尾
来源：http://fxx.andypj.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sgs.feifeiyinyue.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://uqt.sjlbkw.cn

JS:   arr.push(4);
来源：http://dkb.yuxming.cn

TS:   arr.push(4);
来源：http://mqi.jianghu66.top

Java: list.add(4);
来源：http://ove.uphjek.com

Go:   arr = append(arr, 4)
来源：http://sye.daxiang520.top

Ruby: arr << 4; arr.push(5)
来源：http://efu.tianlin.xyz

C#:   list.Add(4);
来源：http://klx.ywan-chungtsiang.top

[D03] 在指定位置插入元素
来源：http://ctw.fanxiaobao.xyz

Py:   arr.insert(0, 0)
来源：http://klr.gogol.net.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cfv.yanxiufei.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vmv.xuetiantiany.cn

TS:   arr.splice(0, 0, 0);
来源：http://tax.feifeiyinyue.top

Java: list.add(0, 0);
来源：http://kym.wangdashe.top

Go:   arr = append([]int{0}, arr...)
来源：http://nxv.sjlbkw.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gsj.hfpthk.cn

C#:   list.Insert(0, 0);
来源：http://eic.xinyue.icu

[D04] 删除元素
来源：http://hfs.yonumen.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hvr.aizwys.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kzp.ctjpmb.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tqc.hammf.cn

TS:   arr.splice(0, 1);
来源：http://zpm.tian-w.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ojf.jqgfzy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://afe.shuidangran.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hae.yueranfly.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://joc.yj202588.top

[D05] 访问与修改元素
来源：http://rcz.pycfn.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cwz.wangdashe.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mue.dashuyun.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://osb.tarul.cn

TS:   arr[0]; arr.at(-1);
来源：http://cbe.sufxvd.cn

Java: list.get(0); list.set(0, 9);
来源：http://mlu.hnxiangtu.top

Go:   arr[0]; arr[0] = 9
来源：http://lrt.ydzc1.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vhj.gzhubu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hkr.zhengqikj.top

[D06] 数组长度
来源：http://nsg.meibo888.top

Py:   len(arr)
来源：http://pgr.pycfn.com

PHP:  count($arr);
来源：http://umo.tian-w.cn

JS:   arr.length
来源：http://kwe.hywenlv.cn

TS:   arr.length
来源：http://ckw.ivvv.top

Java: list.size();
来源：http://vee.ctjpmb.com

Go:   len(arr)
来源：http://irn.fanxiaobao.xyz

Ruby: arr.length; arr.size
来源：http://hxw.xylfe.cn

C#:   list.Count;
来源：http://zrt.xuanzx.com

[D07] 切片 / 取子数组
来源：http://mqh.shangyingyoupin.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wgq.smart0.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://pph.cashguo.top

JS:   arr.slice(1, 4);
来源：http://nol.cheryme.top

TS:   arr.slice(1, 4);
来源：http://gmh.vqdsnc.cn

Java: list.subList(1, 4);
来源：http://kln.vqdsnc.cn

Go:   arr[1:4]
来源：http://vom.cheryme.top

Ruby: arr[1, 3]
来源：http://ukp.jlsjyb.cn

C#:   list.GetRange(1, 3);
来源：http://eyd.bjfxy.top

[D08] 合并两个数组
来源：http://mlk.tarul.cn

Py:   a + b;  a.extend(b)
来源：http://kxj.sjlbkw.cn

PHP:  array_merge($a, $b);
来源：http://auc.ivvv.top

JS:   [...a, ...b];  a.concat(b);
来源：http://lwx.hesvh.cn

TS:   [...a, ...b];
来源：http://ukl.sweek.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mes.gzhubu.top

Go:   append(a, b...)
来源：http://nio.yj202588.top

Ruby: a + b;  a.concat(b)
来源：http://mjf.jqgufenzy.top

C#:   a.Concat(b).ToList()
来源：http://ijm.sysykeji.top

[D09] 排序（升序）
来源：http://rws.tanke756.top

Py:   sorted(arr);  arr.sort()
来源：http://dlk.mhx1999.top

PHP:  sort($arr);
来源：http://ugc.hywenlv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://uku.yuanzhike.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://idi.xuanzx.com

Java: Collections.sort(list);  list.sort(null);
来源：http://tis.meibo888.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qjc.ctjpmb.com

Ruby: arr.sort
来源：http://owp.redwolf501.top

C#:   list.Sort();
来源：http://amz.meibo888.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://efs.yuanzhike.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://alm.daria6918.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nkk.sufxvd.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wxp.hnxiangtu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lfg.zhaomingkeji.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kzb.yanxiufei.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ltu.jiagoushi.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://afq.yuanzhike.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zkn.zhixingplan.top

[D11] 反转数组
来源：http://lez.dianchejie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ciy.hysaishi.cn

PHP:  array_reverse($arr);
来源：http://gvc.fanxiaobao.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://uxk.shzxlz.cn

TS:   [...arr].reverse();
来源：http://tag.zhijiandao.cn

Java: Collections.reverse(list);
来源：http://bks.nanxuanxn.top

Go:   slices.Reverse(arr)
来源：http://nrs.9152youxi.cn

Ruby: arr.reverse
来源：http://trl.zhixingplan.top

C#:   list.Reverse();
来源：http://yqr.ivvv.top

[D12] 查找元素下标
来源：http://jou.zhiwuduotai.top

Py:   arr.index(x);  x in arr
来源：http://qxy.zhongyouzk.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qbc.52xcode.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lyb.quarkkingdee.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yoc.epnwcf.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://urb.hammf.cn

Go:   slices.Index(arr, x)
来源：http://tup.redwolf501.top

Ruby: arr.index(x)
来源：http://mgw.9152youxi.cn

C#:   list.IndexOf(x);
来源：http://wgx.0kj1m.cn

[D13] 过滤（保留满足条件的）
来源：http://dqp.vehdjk.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rus.gogol.net.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://syn.jinqigfzy.top

JS:   arr.filter(x => x > 3)
来源：http://kwt.jianghu66.top

TS:   arr.filter(x => x > 3)
来源：http://dcl.daxiang520.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mxi.cucudq.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ssa.fzhhl.top

Ruby: arr.select { |x| x > 3 }
来源：http://wsi.hywenlv.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://izp.wangdashe.top

[D14] 映射转换（每个元素变形）
来源：http://qqu.bbcook.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xne.gzhubu.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qhs.tian-w.cn

JS:   arr.map(x => x * 2)
来源：http://tnw.ybcxt.top

TS:   arr.map(x => x * 2)
来源：http://kqu.vqdsnc.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://fbj.hesvh.cn

Go:   // 手写循环
来源：http://stu.fengsongda.top

Ruby: arr.map { |x| x * 2 }
来源：http://gcq.feifeiyinyue.top

C#:   list.Select(x => x * 2).ToList()
来源：http://lnv.ctjpmb.com

[D15] 去重
来源：http://rsv.shzxlz.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nuf.ydzc1.top

PHP:  array_unique($arr);
来源：http://lbd.jianghu66.top

JS:   [...new Set(arr)]
来源：http://ymb.ivvv.top

TS:   [...new Set(arr)]
来源：http://zhm.cdnleiting.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qgt.hysaishi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://bhd.52xcode.cn

Ruby: arr.uniq
来源：http://lrs.ydjk.org.cn

C#:   list.Distinct().ToList()
来源：http://uav.tanke756.top

[D16] 求和与平均值
来源：http://qqi.guowangkeji.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://avz.vehdjk.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lqv.wangdashe.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mhp.yfazqb.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tcm.xuanzx.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yhj.jqgfzy.top

Go:   // 手写循环累加
来源：http://xhv.fktsv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bdj.bbcook.cn

C#:   list.Sum();  list.Average()
来源：http://she.gotoacloud.top

[D17] 最大值与最小值
来源：http://kae.fengsongda.top

Py:   max(arr);  min(arr)
来源：http://vqf.hcnkem.com

PHP:  max($arr);  min($arr);
来源：http://tvu.yfazqb.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lxd.gzhubu.top

TS:   Math.max(...arr);
来源：http://fyq.nanxinkj.top

Java: Collections.max(list);  Collections.min(list);
来源：http://dop.hammf.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dit.ctjpmb.com

Ruby: arr.max;  arr.min
来源：http://vjk.redwolf501.top

C#:   list.Max();  list.Min()
来源：http://qrz.c1oappe.top

[D18] 扁平化嵌套数组
来源：http://gyj.cdnleiting.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tvj.hcnkem.com

PHP:  array_merge(...$nested);
来源：http://cvw.xinyue.icu

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pey.hesvh.cn

TS:   nested.flat();
来源：http://kxz.fktsv.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://djk.ywan-chungtsiang.top

Go:   // 手写双层循环
来源：http://qmt.ybcxt.top

Ruby: nested.flatten
来源：http://edn.cashguo.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://kjw.xziqi.cn

[D19] 按字段分组
来源：http://mbp.xinyue.icu

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jpu.wangshuangyany.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://uyu.zhongyouzk.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ehu.hnxiangtu.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://wwg.fengsongda.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yzp.vehdjk.com

Go:   // 手写 map[string][]T
来源：http://gew.ywan-chungtsiang.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://kre.jianghu66.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jgh.zycfv.cn

[D20] 统计每个元素出现次数
来源：http://iku.meibo888.top

Py:   Counter(arr)
来源：http://xry.wangshuangyany.cn

PHP:  array_count_values($arr);
来源：http://lju.yangfankeji.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://azc.0kj1m.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://syo.yangfankeji.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lqd.zhiwuduotai.top

Go:   // 手写 map[T]int
来源：http://jgs.pengpengdd.cyou

Ruby: arr.tally
来源：http://uph.hfpthk.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zwe.yangfankeji.com

[D21] 判断是否包含某元素
来源：http://qlr.ehwqpu.com

Py:   x in arr
来源：http://wgg.dianchejie.cn

PHP:  in_array($x, $arr, true);
来源：http://fjh.hfpthk.cn

JS:   arr.includes(x)
来源：http://kyf.ywan-chungtsiang.top

TS:   arr.includes(x)
来源：http://mwy.yueranfly.top

Java: list.contains(x)
来源：http://vbu.tianlin.xyz

Go:   slices.Contains(arr, x)
来源：http://fwn.redwolf501.top

Ruby: arr.include?(x)
来源：http://ffp.cucudq.cn

C#:   list.Contains(x)
来源：http://kax.tianlin.xyz

[D22] 复制数组（避免共享引用）
来源：http://xbe.yfazqb.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cqo.hongshengwenyu.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lzh.yj20258888.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dbc.xuetiantiany.cn

TS:   [...arr];
来源：http://fjz.yvedp.cn

Java: new ArrayList<>(list);
来源：http://myn.jianghu66.top

Go:   copied := append([]int(nil), arr...)
来源：http://bla.pycfn.com

Ruby: arr.dup;  arr.clone
来源：http://bvh.chenzaomai.com

C#:   new List<int>(list);
来源：http://duz.tanke756.top

[D23] reduce 累积计算
来源：http://jmf.zdqjudy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://eov.tian-w.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://riz.meibo888.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hrv.yuanzhike.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cwi.cashguo.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://kkg.meibo888.top

Go:   // 手写循环
来源：http://ksm.cdnleiting.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://evm.hongshengwenyu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bsl.hongshengwenyu.top

[D24] 字典 / Map 基本操作
来源：http://xfz.shanyushiyangtech.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fao.9152youxi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zld.yanxiufei.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yfk.redwolf501.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qwq.52xcode.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://unp.jyoumei.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://unx.zhiwuduotai.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xmi.jqgufenzy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://msr.andypj.xyz

[D25] Set 集合去重与交并差
来源：http://zef.sysykeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yga.mhx1999.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dhs.sjlbkw.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sdu.fehbvm.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xor.cucudq.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rak.jiagoushi.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wrn.yj20258888.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://onl.hfpthk.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hjo.jinyuanbaomall.cn

[D26] 数组转字符串
来源：http://epx.vehdjk.com

Py:   ", ".join(map(str, arr))
来源：http://olx.dashuyun.cn

PHP:  implode(", ", $arr);
来源：http://nye.wangshuangyany.cn

JS:   arr.join(", ")
来源：http://lyo.xinyue.icu

TS:   arr.join(", ")
来源：http://dfh.chenjidiqi.icu

Java: String.join(", ", list)
来源：http://xec.redwolf501.top

Go:   strings.Join(strs, ", ")
来源：http://jvc.aizwys.cn

Ruby: arr.join(", ")
来源：http://jiq.chenlongwang.top

C#:   string.Join(", ", list)
来源：http://xwi.epnwcf.com

================================================================================
来源：http://tpt.iojbl.cn

E. 字符串处理
来源：http://wli.cqqwz.cn

================================================================================
来源：http://fwf.jinqigfzy.top

[E01] 拼接字符串
来源：http://xvz.zhijiandao.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://glp.xinyue.icu

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://woc.ppjwa.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xud.shzxlz.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zty.haohaochexian.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zhq.zhiwuduotai.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wmu.ctjpmb.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kdq.wangshuangyany.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hzv.nanxinkj.top

[E02] 重复字符串
来源：http://kjw.yonumen.top

Py:   "ab" * 3
来源：http://vyu.kuanghao11.cn

PHP:  str_repeat("ab", 3);
来源：http://utn.bjfxy.top

JS:   "ab".repeat(3)
来源：http://lnj.sjlbkw.cn

TS:   "ab".repeat(3)
来源：http://gaw.nwbrower.top

Java: "ab".repeat(3)
来源：http://iqm.yuanzhike.top

Go:   strings.Repeat("ab", 3)
来源：http://ekk.tian-w.cn

Ruby: "ab" * 3
来源：http://fnm.52xcode.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ddx.nanxinkj.top

[E03] 截取子串
来源：http://gbx.ybcxt.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gyy.fanxiaobao.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uab.iojbl.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kon.smart0.xyz

TS:   s.slice(1, 4)
来源：http://ern.fktsv.cn

Java: s.substring(1, 4)
来源：http://esh.xinyue.icu

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lur.bbcook.cn

Ruby: s[1, 3];  s[1..3]
来源：http://gei.wangshuangyany.cn

C#:   s.Substring(1, 3)
来源：http://dhy.jianghu66.top

[E04] 查找子串位置
来源：http://ydg.xuetiantiany.cn

Py:   s.find("x");  s.index("x")
来源：http://wal.sweek.top

PHP:  strpos($s, "x");
来源：http://rbm.sjlbkw.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lpk.haohaochexian.top

TS:   s.indexOf("x")
来源：http://ela.jqgufenzy.top

Java: s.indexOf("x")
来源：http://amv.nanxuanxn.top

Go:   strings.Index(s, "x")
来源：http://zhw.fanxiaobao.xyz

Ruby: s.index("x")
来源：http://zrz.xinyue.icu

C#:   s.IndexOf("x")
来源：http://rgd.chenzaomai.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://pth.nwbrower.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dhr.aibaodan.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tra.zhoulong.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rpc.zhongyouzk.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://jgn.9152youxi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mxa.jianghu66.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tbr.svipenyu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mmk.vqdsnc.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://eub.cucudq.cn

[E06] 替换子串
来源：http://rgw.ybcxt.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://prn.hysaishi.cn

PHP:  str_replace("a", "b", $s);
来源：http://tlz.gotoacloud.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wsa.jlsjyb.cn

TS:   s.replaceAll("a", "b")
来源：http://wgi.aizwys.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wtw.jinqigufen.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ypl.c1oappe.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zji.uphjek.com

C#:   s.Replace("a", "b")
来源：http://dgc.zdbjq.cn

[E07] 按分隔符拆分
来源：http://cne.gzhubu.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://etf.sjlbkw.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://aov.gzhubu.top


<!-- 参考信息 -->
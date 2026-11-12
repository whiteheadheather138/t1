代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://akn.shanyushiyangtech.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sxq.hnqzz.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://lbj.guannengcc.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kpv.kuanghao11.cn

Go:   arr := []int{1, 2, 3}
来源：http://psl.ywan-chungtsiang.top

Ruby: arr = [1, 2, 3]
来源：http://tpc.iojbl.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://spc.kuanghao11.cn

[D02] 追加元素到末尾
来源：http://phu.xylfe.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://usm.fzhhl.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fjd.xingfuxueyuan.xyz

JS:   arr.push(4);
来源：http://bpw.zdqjudy.top

TS:   arr.push(4);
来源：http://asc.shangyingyoupin.top

Java: list.add(4);
来源：http://hss.kuanghao11.cn

Go:   arr = append(arr, 4)
来源：http://fjg.xingfuxueyuan.xyz

Ruby: arr << 4; arr.push(5)
来源：http://zbk.jinyuanbaomall.cn

C#:   list.Add(4);
来源：http://htr.cheryme.top

[D03] 在指定位置插入元素
来源：http://dok.redwolf501.top

Py:   arr.insert(0, 0)
来源：http://xvb.tian-w.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qyn.pengpengdd.cyou

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ibs.yanxiufei.cn

TS:   arr.splice(0, 0, 0);
来源：http://acy.chenjidiqi.icu

Java: list.add(0, 0);
来源：http://zcp.daria6918.cn

Go:   arr = append([]int{0}, arr...)
来源：http://cts.guowangkeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qyu.tianlin.xyz

C#:   list.Insert(0, 0);
来源：http://obb.zdqjudy.top

[D04] 删除元素
来源：http://mfu.aizwys.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://doh.yfazqb.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dek.snrcjt.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hoz.xingfuxueyuan.xyz

TS:   arr.splice(0, 1);
来源：http://snz.yj20258888.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ble.jyoumei.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dxb.sufxvd.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gel.zycfv.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://atq.ppjwa.cn

[D05] 访问与修改元素
来源：http://lry.xuanzx.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dxj.hysaishi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bfs.zhoulong.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hrn.cqqwz.cn

TS:   arr[0]; arr.at(-1);
来源：http://yfd.hesvh.cn

Java: list.get(0); list.set(0, 9);
来源：http://wuh.birdmap.top

Go:   arr[0]; arr[0] = 9
来源：http://qba.jqgfzy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ebl.fzhhl.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://msu.yj20258.top

[D06] 数组长度
来源：http://jeq.cashguo.top

Py:   len(arr)
来源：http://unn.vqdsnc.cn

PHP:  count($arr);
来源：http://urh.gogol.net.cn

JS:   arr.length
来源：http://ykb.feifeiyinyue.top

TS:   arr.length
来源：http://yzw.ydjk.org.cn

Java: list.size();
来源：http://nca.zhoulong.xyz

Go:   len(arr)
来源：http://anv.feifeiyinyue.top

Ruby: arr.length; arr.size
来源：http://iyq.gogol.net.cn

C#:   list.Count;
来源：http://dge.yanxiufei.cn

[D07] 切片 / 取子数组
来源：http://xeb.shangyingyoupin.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zls.epnwcf.com

PHP:  array_slice($arr, 1, 3);
来源：http://dtw.shuidangran.top

JS:   arr.slice(1, 4);
来源：http://opz.xylfe.cn

TS:   arr.slice(1, 4);
来源：http://fye.daxiang520.top

Java: list.subList(1, 4);
来源：http://frp.ybcxt.top

Go:   arr[1:4]
来源：http://trh.vehdjk.com

Ruby: arr[1, 3]
来源：http://ogu.hfpthk.cn

C#:   list.GetRange(1, 3);
来源：http://wlb.zhongyouzk.top

[D08] 合并两个数组
来源：http://icq.sweek.top

Py:   a + b;  a.extend(b)
来源：http://fct.ywan-chungtsiang.top

PHP:  array_merge($a, $b);
来源：http://gud.vqdsnc.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ukc.zhaomingkeji.xyz

TS:   [...a, ...b];
来源：http://elb.yuxming.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wkt.yfazqb.com

Go:   append(a, b...)
来源：http://dil.hfpthk.cn

Ruby: a + b;  a.concat(b)
来源：http://iec.hywenlv.cn

C#:   a.Concat(b).ToList()
来源：http://lce.bbcook.cn

[D09] 排序（升序）
来源：http://dcs.shzxlz.cn

Py:   sorted(arr);  arr.sort()
来源：http://clz.hysaishi.cn

PHP:  sort($arr);
来源：http://anh.sysykeji.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nsg.nanxinkj.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ger.yangfankeji.com

Java: Collections.sort(list);  list.sort(null);
来源：http://eej.yangfankeji.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://saz.yuxming.cn

Ruby: arr.sort
来源：http://rhl.hongshengwenyu.top

C#:   list.Sort();
来源：http://kwr.c1oappe.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://yuj.daria6918.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nwq.yfazqb.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yfe.yonumen.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://uie.tianlin.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://eog.sxryk.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://oid.yueranfly.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://iid.hammf.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tem.gogol.net.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lzf.dianchejie.cn

[D11] 反转数组
来源：http://jgb.jianghu66.top

Py:   arr[::-1];  arr.reverse()
来源：http://uxp.gotoacloud.top

PHP:  array_reverse($arr);
来源：http://vda.jinghuilouyu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vzz.xylfe.cn

TS:   [...arr].reverse();
来源：http://xbr.bjfxy.top

Java: Collections.reverse(list);
来源：http://xzv.kuanghao11.cn

Go:   slices.Reverse(arr)
来源：http://byg.xziqi.cn

Ruby: arr.reverse
来源：http://zrj.daxiang520.top

C#:   list.Reverse();
来源：http://hcs.uphjek.com

[D12] 查找元素下标
来源：http://qzg.yfazqb.com

Py:   arr.index(x);  x in arr
来源：http://esk.ivvv.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qsx.feifeiyinyue.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://chb.zhoulong.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tai.hongshengwenyu.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rtx.xingfuxueyuan.xyz

Go:   slices.Index(arr, x)
来源：http://wst.fktsv.cn

Ruby: arr.index(x)
来源：http://trq.epnwcf.com

C#:   list.IndexOf(x);
来源：http://vff.gaohongyu789.top

[D13] 过滤（保留满足条件的）
来源：http://pfp.guannengcc.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zrx.hesvh.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nat.hysaishi.cn

JS:   arr.filter(x => x > 3)
来源：http://tjg.aibaodan.cn

TS:   arr.filter(x => x > 3)
来源：http://qjl.gogol.net.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tal.hfpthk.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mkh.andypj.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://deh.sweek.top

C#:   list.Where(x => x > 3).ToList()
来源：http://aks.dianchejie.cn

[D14] 映射转换（每个元素变形）
来源：http://css.sweek.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wof.ivvv.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ozf.jinqigfzy.top

JS:   arr.map(x => x * 2)
来源：http://att.yongpay.top

TS:   arr.map(x => x * 2)
来源：http://ibo.cucudq.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qxk.0kj1m.cn

Go:   // 手写循环
来源：http://pbd.jiagoushi.top

Ruby: arr.map { |x| x * 2 }
来源：http://rwx.haohaochexian.top

C#:   list.Select(x => x * 2).ToList()
来源：http://txq.gotoacloud.top

[D15] 去重
来源：http://jas.xinyue.icu

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://atj.pycfn.com

PHP:  array_unique($arr);
来源：http://vhq.jqgufenzy.top

JS:   [...new Set(arr)]
来源：http://gjd.hysaishi.cn

TS:   [...new Set(arr)]
来源：http://tly.zycfv.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sci.cashguo.top

Go:   // 用 map[T]struct{} 手写
来源：http://hpf.shangyingyoupin.top

Ruby: arr.uniq
来源：http://eqt.zhijiandao.cn

C#:   list.Distinct().ToList()
来源：http://rra.yonumen.top

[D16] 求和与平均值
来源：http://gcg.hcnkem.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ayx.fktsv.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://awm.ehwqpu.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rxl.ybcxt.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mxp.c1oappe.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://oib.fzhhl.top

Go:   // 手写循环累加
来源：http://mqc.zhiwuduotai.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vig.hcnkem.com

C#:   list.Sum();  list.Average()
来源：http://wfq.ctjpmb.com

[D17] 最大值与最小值
来源：http://ffo.zycfv.cn

Py:   max(arr);  min(arr)
来源：http://woh.xziqi.cn

PHP:  max($arr);  min($arr);
来源：http://hbt.yfazqb.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xar.mhx1999.top

TS:   Math.max(...arr);
来源：http://nsd.jqgfzy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://fti.guowangkeji.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://akx.cheryme.top

Ruby: arr.max;  arr.min
来源：http://jeo.0kj1m.cn

C#:   list.Max();  list.Min()
来源：http://ynb.ybcxt.top

[D18] 扁平化嵌套数组
来源：http://nuq.chenlongwang.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://frc.yongpay.top

PHP:  array_merge(...$nested);
来源：http://anj.cdnleiting.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tfd.yonumen.top

TS:   nested.flat();
来源：http://hmy.c1oappe.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pzl.birdmap.top

Go:   // 手写双层循环
来源：http://ocy.0kj1m.cn

Ruby: nested.flatten
来源：http://uun.hfpthk.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wft.hammf.cn

[D19] 按字段分组
来源：http://bys.yvedp.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pqe.xuetiantiany.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://inm.cucudq.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yrf.316326.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://yhg.havefunace.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ntx.hnxiangtu.top

Go:   // 手写 map[string][]T
来源：http://xxt.kuanghao11.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vht.9152youxi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hhf.daria6918.cn

[D20] 统计每个元素出现次数
来源：http://tcf.ppjwa.cn

Py:   Counter(arr)
来源：http://gix.pycfn.com

PHP:  array_count_values($arr);
来源：http://fyk.yj20258888.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yxp.yvedp.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nsl.zhongyouzk.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://grs.yuxming.cn

Go:   // 手写 map[T]int
来源：http://efz.sjlbkw.cn

Ruby: arr.tally
来源：http://vhv.zhoulong.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xqp.iojbl.cn

[D21] 判断是否包含某元素
来源：http://mty.vqdsnc.cn

Py:   x in arr
来源：http://cud.yj20258888.top

PHP:  in_array($x, $arr, true);
来源：http://bsw.hongshengwenyu.top

JS:   arr.includes(x)
来源：http://jwt.tarul.cn

TS:   arr.includes(x)
来源：http://ftt.gzhubu.top

Java: list.contains(x)
来源：http://nba.cheryme.top

Go:   slices.Contains(arr, x)
来源：http://yav.zhongyouzk.top

Ruby: arr.include?(x)
来源：http://rdx.guowangkeji.top

C#:   list.Contains(x)
来源：http://znb.jinqigfzy.top

[D22] 复制数组（避免共享引用）
来源：http://hmf.smart0.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pps.zdbjq.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qtb.aizwys.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tvl.kuanghao11.cn

TS:   [...arr];
来源：http://via.fzhhl.top

Java: new ArrayList<>(list);
来源：http://lvh.shuidangran.top

Go:   copied := append([]int(nil), arr...)
来源：http://cnd.sweek.top

Ruby: arr.dup;  arr.clone
来源：http://imu.sweek.top

C#:   new List<int>(list);
来源：http://qxl.ybcxt.top

[D23] reduce 累积计算
来源：http://gsr.hysaishi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dmi.feifeiyinyue.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fng.hnxiangtu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bts.xinyue.icu

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mtw.c1oappe.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://dvf.0kj1m.cn

Go:   // 手写循环
来源：http://uma.jinqigufen.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://eij.ydjk.org.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://imu.hesvh.cn

[D24] 字典 / Map 基本操作
来源：http://doa.yonumen.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qdd.xinyue.icu

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ecw.xingfuxueyuan.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xte.hcnkem.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hre.xingfuxueyuan.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xhj.uphjek.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sxy.daxiang520.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zwd.gzhubu.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yqn.svipenyu.cn

[D25] Set 集合去重与交并差
来源：http://ymt.haohaochexian.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tjv.gaohongyu789.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vgp.ywan-chungtsiang.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://noq.zhiwuduotai.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mpp.xuanzx.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ilr.shanyushiyangtech.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ptr.tanke756.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cla.0kj1m.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sso.quarkkingdee.top

[D26] 数组转字符串
来源：http://ldu.andypj.xyz

Py:   ", ".join(map(str, arr))
来源：http://kcn.fanxiaobao.xyz

PHP:  implode(", ", $arr);
来源：http://tdk.jianghu66.top

JS:   arr.join(", ")
来源：http://nuf.xuanzx.com

TS:   arr.join(", ")
来源：http://ewk.0kj1m.cn

Java: String.join(", ", list)
来源：http://bkn.gotoacloud.top

Go:   strings.Join(strs, ", ")
来源：http://vqo.nanxuanxn.top

Ruby: arr.join(", ")
来源：http://yyw.xinyue.icu

C#:   string.Join(", ", list)
来源：http://nwc.cashguo.top

================================================================================
来源：http://hju.andypj.xyz

E. 字符串处理
来源：http://tnf.pengpengdd.cyou

================================================================================
来源：http://jwo.hongshengwenyu.top

[E01] 拼接字符串
来源：http://owf.yanxiufei.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://api.dashuyun.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ujk.cheryme.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ktv.ctjpmb.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lrd.ctjpmb.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uuj.yj20258888.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tps.uphjek.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://osd.sysykeji.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sbq.gzhubu.top

[E02] 重复字符串
来源：http://ghd.snrcjt.cn

Py:   "ab" * 3
来源：http://ybf.ydzc1.top

PHP:  str_repeat("ab", 3);
来源：http://wbo.feifeiyinyue.top

JS:   "ab".repeat(3)
来源：http://czr.fengsongda.top

TS:   "ab".repeat(3)
来源：http://udw.jinyuanbaomall.cn

Java: "ab".repeat(3)
来源：http://esu.redwolf501.top

Go:   strings.Repeat("ab", 3)
来源：http://peq.bbcook.cn

Ruby: "ab" * 3
来源：http://kbu.fanxiaobao.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dpf.meibo888.top

[E03] 截取子串
来源：http://cnt.dashuyun.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hft.yueranfly.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zue.daxiang520.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://syt.feifeiyinyue.top

TS:   s.slice(1, 4)
来源：http://usb.bbcook.cn

Java: s.substring(1, 4)
来源：http://yuk.iojbl.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mwg.ydzc1.top

Ruby: s[1, 3];  s[1..3]
来源：http://usc.yj202588.top

C#:   s.Substring(1, 3)
来源：http://ost.hywenlv.cn

[E04] 查找子串位置
来源：http://kwz.feifeiyinyue.top

Py:   s.find("x");  s.index("x")
来源：http://tqe.wangshuangyany.cn

PHP:  strpos($s, "x");
来源：http://rvr.shuidangran.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://law.xylfe.cn

TS:   s.indexOf("x")
来源：http://zza.cucudq.cn

Java: s.indexOf("x")
来源：http://jxz.sjlbkw.cn

Go:   strings.Index(s, "x")
来源：http://yqu.tanke756.top

Ruby: s.index("x")
来源：http://cai.meibo888.top

C#:   s.IndexOf("x")
来源：http://rpo.birdmap.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://snf.ehwqpu.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hmg.epnwcf.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bhk.jinqigfzy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://btd.fzhhl.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://whi.jinghuilouyu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hou.jinqigufen.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yzu.gotoacloud.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mom.ydjk.org.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ykx.zhixingplan.top

[E06] 替换子串
来源：http://utr.yuxming.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hrc.ybcxt.top

PHP:  str_replace("a", "b", $s);
来源：http://edx.jianghu66.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rbi.yuxming.cn

TS:   s.replaceAll("a", "b")
来源：http://fyz.c1oappe.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ldh.jinqigufen.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mub.nanxuanxn.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pxs.dianchejie.cn

C#:   s.Replace("a", "b")
来源：http://gyr.jyoumei.cn

[E07] 按分隔符拆分
来源：http://jyz.zhiwuduotai.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dst.hongshengwenyu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mmk.tanke756.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://fda.wangdashe.top

TS:   s.split(",")
来源：http://dam.316326.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://jqe.cashguo.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cjt.hnqzz.top

Ruby: s.split(",");  s.split
来源：http://fcn.sufxvd.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qcj.epnwcf.com

[E08] 数组按分隔符合并
来源：http://jfr.xziqi.cn

Py:   ",".join(items)
来源：http://xih.shzxlz.cn


<!-- 参考信息 -->
代发 wailian999

D. 数组 / 列表 / 集合
来源：http://obc.haohaochexian.top

================================================================================
来源：http://ywj.sysykeji.top

[D01] 创建数组 / 列表
来源：http://vco.yueranfly.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://lfo.dashuyun.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qse.gaohongyu789.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://goq.yj20258.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://zny.dashuyun.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cjc.hcnkem.com

Go:   arr := []int{1, 2, 3}
来源：http://xzc.gogol.net.cn

Ruby: arr = [1, 2, 3]
来源：http://cxw.yuanzhike.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fha.hnxiangtu.top

[D02] 追加元素到末尾
来源：http://wzl.redwolf501.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rdz.gaohongyu789.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fbr.guowangkeji.top

JS:   arr.push(4);
来源：http://kwv.jqgfzy.top

TS:   arr.push(4);
来源：http://epy.hcnkem.com

Java: list.add(4);
来源：http://uri.aizwys.cn

Go:   arr = append(arr, 4)
来源：http://lsj.sufxvd.cn

Ruby: arr << 4; arr.push(5)
来源：http://rfq.gotoacloud.top

C#:   list.Add(4);
来源：http://xdj.ehwqpu.com

[D03] 在指定位置插入元素
来源：http://gzn.haohaochexian.top

Py:   arr.insert(0, 0)
来源：http://mas.nanxinkj.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cev.jianghu66.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mhy.hysaishi.cn

TS:   arr.splice(0, 0, 0);
来源：http://zgn.sxryk.cn

Java: list.add(0, 0);
来源：http://oiw.kuanghao11.cn

Go:   arr = append([]int{0}, arr...)
来源：http://bmc.jinyuanbaomall.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ahj.ehwqpu.com

C#:   list.Insert(0, 0);
来源：http://aux.jinyuanbaomall.cn

[D04] 删除元素
来源：http://pmb.cdnleiting.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ptt.cheryme.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qmd.sxryk.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gxa.tanke756.top

TS:   arr.splice(0, 1);
来源：http://wlk.yj202588.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://trt.dianchejie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dsj.jianghu66.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://swd.hammf.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mqk.dashuyun.cn

[D05] 访问与修改元素
来源：http://egt.cucudq.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wce.yuxming.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xqs.yvedp.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mrt.gogol.net.cn

TS:   arr[0]; arr.at(-1);
来源：http://afv.yuxming.cn

Java: list.get(0); list.set(0, 9);
来源：http://dme.bjfxy.top

Go:   arr[0]; arr[0] = 9
来源：http://idm.guannengcc.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hro.cqqwz.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vvt.nwbrower.top

[D06] 数组长度
来源：http://exs.zhongyouzk.top

Py:   len(arr)
来源：http://ofe.0kj1m.cn

PHP:  count($arr);
来源：http://bzo.zhaomingkeji.xyz

JS:   arr.length
来源：http://mqf.zycfv.cn

TS:   arr.length
来源：http://wpx.gogol.net.cn

Java: list.size();
来源：http://kpp.hywenlv.cn

Go:   len(arr)
来源：http://dss.jyoumei.cn

Ruby: arr.length; arr.size
来源：http://amt.9152youxi.cn

C#:   list.Count;
来源：http://loa.jyoumei.cn

[D07] 切片 / 取子数组
来源：http://quf.pengpengdd.cyou

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://esw.xuetiantiany.cn

PHP:  array_slice($arr, 1, 3);
来源：http://rxn.jinghuilouyu.cn

JS:   arr.slice(1, 4);
来源：http://vee.tarul.cn

TS:   arr.slice(1, 4);
来源：http://baj.yueranfly.top

Java: list.subList(1, 4);
来源：http://zru.cheryme.top

Go:   arr[1:4]
来源：http://jmc.jqgufenzy.top

Ruby: arr[1, 3]
来源：http://faf.0kj1m.cn

C#:   list.GetRange(1, 3);
来源：http://xtu.tianlin.xyz

[D08] 合并两个数组
来源：http://yvm.yonumen.top

Py:   a + b;  a.extend(b)
来源：http://yeu.cashguo.top

PHP:  array_merge($a, $b);
来源：http://fif.cdnleiting.top

JS:   [...a, ...b];  a.concat(b);
来源：http://tol.0kj1m.cn

TS:   [...a, ...b];
来源：http://eks.meibo888.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ndr.feifeiyinyue.top

Go:   append(a, b...)
来源：http://ywu.sxryk.cn

Ruby: a + b;  a.concat(b)
来源：http://yjn.cdnleiting.top

C#:   a.Concat(b).ToList()
来源：http://ync.0kj1m.cn

[D09] 排序（升序）
来源：http://hwj.chenjidiqi.icu

Py:   sorted(arr);  arr.sort()
来源：http://run.nanxuanxn.top

PHP:  sort($arr);
来源：http://ezt.tanke756.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rgy.shangyingyoupin.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://wyv.zycfv.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://kyy.hesvh.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://llu.havefunace.top

Ruby: arr.sort
来源：http://ffn.hammf.cn

C#:   list.Sort();
来源：http://oqj.jinqigufen.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://pny.vqdsnc.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zbn.tian-w.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sla.zhixingplan.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vsr.haohaochexian.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nqx.vehdjk.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ndc.zycfv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pev.ehwqpu.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qds.tarul.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jru.jinyuanbaomall.cn

[D11] 反转数组
来源：http://zeo.ppjwa.cn

Py:   arr[::-1];  arr.reverse()
来源：http://kih.kuanghao11.cn

PHP:  array_reverse($arr);
来源：http://szm.hongshengwenyu.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jcd.ivvv.top

TS:   [...arr].reverse();
来源：http://age.cdnleiting.top

Java: Collections.reverse(list);
来源：http://mby.cucudq.cn

Go:   slices.Reverse(arr)
来源：http://day.bjfxy.top

Ruby: arr.reverse
来源：http://dns.hnqzz.top

C#:   list.Reverse();
来源：http://cfs.hysaishi.cn

[D12] 查找元素下标
来源：http://iut.ctjpmb.com

Py:   arr.index(x);  x in arr
来源：http://pte.feifeiyinyue.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://frd.ywan-chungtsiang.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://muf.jinqigufen.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jra.ppjwa.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dru.chenjidiqi.icu

Go:   slices.Index(arr, x)
来源：http://jjg.fengsongda.top

Ruby: arr.index(x)
来源：http://cfz.jinyuanbaomall.cn

C#:   list.IndexOf(x);
来源：http://iqz.hysaishi.cn

[D13] 过滤（保留满足条件的）
来源：http://sjo.hammf.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rwx.feifeiyinyue.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qbl.fzhhl.top

JS:   arr.filter(x => x > 3)
来源：http://gmd.jinghuilouyu.cn

TS:   arr.filter(x => x > 3)
来源：http://shq.ydjk.org.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vzl.guannengcc.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ros.bjfxy.top

Ruby: arr.select { |x| x > 3 }
来源：http://jwp.dianchejie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://mqx.tarul.cn

[D14] 映射转换（每个元素变形）
来源：http://dlm.yuanzhike.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://grw.ctjpmb.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rkd.shzxlz.cn

JS:   arr.map(x => x * 2)
来源：http://xlw.haohaochexian.top

TS:   arr.map(x => x * 2)
来源：http://alw.pycfn.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://bdv.fktsv.cn

Go:   // 手写循环
来源：http://cqs.jinqigfzy.top

Ruby: arr.map { |x| x * 2 }
来源：http://maw.yanxiufei.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://piv.shuidangran.top

[D15] 去重
来源：http://lls.wangdashe.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zzs.zdqjudy.top

PHP:  array_unique($arr);
来源：http://ytj.hfpthk.cn

JS:   [...new Set(arr)]
来源：http://mqg.uphjek.com

TS:   [...new Set(arr)]
来源：http://sop.hcnkem.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mgc.sweek.top

Go:   // 用 map[T]struct{} 手写
来源：http://qvz.shangyingyoupin.top

Ruby: arr.uniq
来源：http://xkw.nwbrower.top

C#:   list.Distinct().ToList()
来源：http://wbh.hongshengwenyu.top

[D16] 求和与平均值
来源：http://rpl.jinyuanbaomall.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tuc.vqdsnc.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pwu.yongpay.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lwe.xuanzx.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://goc.cashguo.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mby.zdqjudy.top

Go:   // 手写循环累加
来源：http://nfr.chenjidiqi.icu

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dsa.cucudq.cn

C#:   list.Sum();  list.Average()
来源：http://vgv.316326.xyz

[D17] 最大值与最小值
来源：http://bvo.sysykeji.top

Py:   max(arr);  min(arr)
来源：http://hjt.jianghu66.top

PHP:  max($arr);  min($arr);
来源：http://pcj.9152youxi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tte.hysaishi.cn

TS:   Math.max(...arr);
来源：http://idq.daxiang520.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ntx.ybcxt.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tqd.jiagoushi.top

Ruby: arr.max;  arr.min
来源：http://rxx.yvedp.cn

C#:   list.Max();  list.Min()
来源：http://axe.fehbvm.com

[D18] 扁平化嵌套数组
来源：http://sma.zhengqikj.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xxu.snrcjt.cn

PHP:  array_merge(...$nested);
来源：http://tgr.fanxiaobao.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://usl.nanxuanxn.top

TS:   nested.flat();
来源：http://rcy.guowangkeji.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fyj.guowangkeji.top

Go:   // 手写双层循环
来源：http://oyi.ivvv.top

Ruby: nested.flatten
来源：http://awl.yj202588.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://cxz.tanke756.top

[D19] 按字段分组
来源：http://bma.sufxvd.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fcm.316326.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mka.daria6918.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nef.zhongyouzk.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://moc.hcnkem.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xaq.nanxinkj.top

Go:   // 手写 map[string][]T
来源：http://lkh.yanxiufei.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ezi.shzxlz.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zot.jyoumei.cn

[D20] 统计每个元素出现次数
来源：http://uiz.tarul.cn

Py:   Counter(arr)
来源：http://mmc.pycfn.com

PHP:  array_count_values($arr);
来源：http://ehb.haohaochexian.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dvk.zhixingplan.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iwo.yuxming.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zvq.yangfankeji.com

Go:   // 手写 map[T]int
来源：http://prw.jiagoushi.top

Ruby: arr.tally
来源：http://knb.yueranfly.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://quo.dashuyun.cn

[D21] 判断是否包含某元素
来源：http://fsh.hywenlv.cn

Py:   x in arr
来源：http://hss.yueranfly.top

PHP:  in_array($x, $arr, true);
来源：http://ojp.smart0.xyz

JS:   arr.includes(x)
来源：http://ldx.zhoulong.xyz

TS:   arr.includes(x)
来源：http://ups.yueranfly.top

Java: list.contains(x)
来源：http://att.ehwqpu.com

Go:   slices.Contains(arr, x)
来源：http://pwu.shanyushiyangtech.top

Ruby: arr.include?(x)
来源：http://ofh.nwbrower.top

C#:   list.Contains(x)
来源：http://ima.ydzc1.top

[D22] 复制数组（避免共享引用）
来源：http://ceo.redwolf501.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ncn.sysykeji.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tvv.redwolf501.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yov.fzhhl.top

TS:   [...arr];
来源：http://udj.fehbvm.com

Java: new ArrayList<>(list);
来源：http://ngr.yj20258888.top

Go:   copied := append([]int(nil), arr...)
来源：http://rcm.uphjek.com

Ruby: arr.dup;  arr.clone
来源：http://ilw.guowangkeji.top

C#:   new List<int>(list);
来源：http://ans.zdqjudy.top

[D23] reduce 累积计算
来源：http://zzr.cucudq.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yso.jqgufenzy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tze.jinqigfzy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rvf.birdmap.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qxl.yj20258.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://svk.redwolf501.top

Go:   // 手写循环
来源：http://qae.zhijiandao.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://scg.zdbjq.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jjc.chenlongwang.top

[D24] 字典 / Map 基本操作
来源：http://xpe.kuanghao11.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://iwj.pengpengdd.cyou

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cdc.tanke756.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rzt.sweek.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://iww.fanxiaobao.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://htc.tarul.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sqj.fzhhl.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://llj.yuanzhike.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ble.aibaodan.cn

[D25] Set 集合去重与交并差
来源：http://jnm.zhiwuduotai.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cxg.ppjwa.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kpy.havefunace.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ilj.mhx1999.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vpm.nwbrower.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mpq.yuxming.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zav.vqdsnc.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vbo.meibo888.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://izt.sxryk.cn

[D26] 数组转字符串
来源：http://lfe.cheryme.top

Py:   ", ".join(map(str, arr))
来源：http://dgv.yuxming.cn

PHP:  implode(", ", $arr);
来源：http://loj.shanyushiyangtech.top

JS:   arr.join(", ")
来源：http://csi.gogol.net.cn

TS:   arr.join(", ")
来源：http://nln.xuanzx.com

Java: String.join(", ", list)
来源：http://ahj.jinqigfzy.top

Go:   strings.Join(strs, ", ")
来源：http://gdj.c1oappe.top

Ruby: arr.join(", ")
来源：http://shi.cashguo.top

C#:   string.Join(", ", list)
来源：http://igw.guowangkeji.top

================================================================================
来源：http://czt.shanyushiyangtech.top

E. 字符串处理
来源：http://bly.jinqigufen.top

================================================================================
来源：http://qbj.quarkkingdee.top

[E01] 拼接字符串
来源：http://wrf.shanyushiyangkeji.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wlg.yanxiufei.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uwa.nanxinkj.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hky.zhiwuduotai.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fqk.jiagoushi.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mbg.bbcook.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xam.fengsongda.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ast.hnxiangtu.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fru.fehbvm.com

[E02] 重复字符串
来源：http://lhs.ehwqpu.com

Py:   "ab" * 3
来源：http://ygs.wangshuangyany.cn

PHP:  str_repeat("ab", 3);
来源：http://wpn.sjlbkw.cn

JS:   "ab".repeat(3)
来源：http://zwz.hysaishi.cn

TS:   "ab".repeat(3)
来源：http://rer.yangfankeji.com

Java: "ab".repeat(3)
来源：http://err.redwolf501.top

Go:   strings.Repeat("ab", 3)
来源：http://jjj.yangfankeji.com

Ruby: "ab" * 3
来源：http://otb.hnxiangtu.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sjb.shanyushiyangkeji.top

[E03] 截取子串
来源：http://buw.yvedp.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jrm.meibo888.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hij.52xcode.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://byh.hnqzz.top

TS:   s.slice(1, 4)
来源：http://wrh.jianghu66.top

Java: s.substring(1, 4)
来源：http://rke.aizwys.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://iud.kuanghao11.cn

Ruby: s[1, 3];  s[1..3]
来源：http://tnj.hammf.cn

C#:   s.Substring(1, 3)
来源：http://ibo.iojbl.cn

[E04] 查找子串位置
来源：http://fmh.jianghu66.top

Py:   s.find("x");  s.index("x")
来源：http://mme.zhoulong.xyz

PHP:  strpos($s, "x");
来源：http://lzq.hesvh.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ntp.yj20258888.top

TS:   s.indexOf("x")
来源：http://eeu.hysaishi.cn

Java: s.indexOf("x")
来源：http://ymn.tianlin.xyz

Go:   strings.Index(s, "x")
来源：http://ouh.hywenlv.cn

Ruby: s.index("x")
来源：http://vqj.redwolf501.top

C#:   s.IndexOf("x")
来源：http://vuo.hnxiangtu.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://pgi.ywan-chungtsiang.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nst.epnwcf.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zqo.hongshengwenyu.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jgt.ppjwa.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://khd.fanxiaobao.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qtj.fzhhl.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mkv.ybcxt.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nwl.pengpengdd.cyou

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fyj.zhaomingkeji.xyz

[E06] 替换子串
来源：http://jog.daxiang520.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mxj.chenlongwang.top

PHP:  str_replace("a", "b", $s);
来源：http://opy.gaohongyu789.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rwt.gzhubu.top

TS:   s.replaceAll("a", "b")
来源：http://ixk.yonumen.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hrd.dashuyun.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pao.zhijiandao.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wur.cdnleiting.top

C#:   s.Replace("a", "b")
来源：http://myy.ehwqpu.com

[E07] 按分隔符拆分
来源：http://lub.kuanghao11.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dti.pycfn.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wct.feifeiyinyue.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://kvb.mhx1999.top

TS:   s.split(",")
来源：http://atq.jinqigufen.top

Java: s.split(",");  s.split("\\s+")
来源：http://mvd.xingfuxueyuan.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wjr.jlsjyb.cn


<!-- 参考信息 -->
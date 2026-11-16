代发 wailian999

D. 数组 / 列表 / 集合
来源：http://mlc.andypj.xyz

================================================================================
来源：http://pto.jlsjyb.cn

[D01] 创建数组 / 列表
来源：http://dse.iojbl.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://kff.nanxinkj.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zir.jyoumei.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dsu.yuanzhike.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://oqr.zhiwuduotai.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tkh.xuanzx.com

Go:   arr := []int{1, 2, 3}
来源：http://drb.wangdashe.top

Ruby: arr = [1, 2, 3]
来源：http://slq.gogol.net.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mnx.ivvv.top

[D02] 追加元素到末尾
来源：http://fri.svipenyu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xtq.yfazqb.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cgv.feifeiyinyue.top

JS:   arr.push(4);
来源：http://odi.redwolf501.top

TS:   arr.push(4);
来源：http://ufw.gzhubu.top

Java: list.add(4);
来源：http://qmb.uphjek.com

Go:   arr = append(arr, 4)
来源：http://rct.kuanghao11.cn

Ruby: arr << 4; arr.push(5)
来源：http://ttu.xuanzx.com

C#:   list.Add(4);
来源：http://tzl.shanyushiyangtech.top

[D03] 在指定位置插入元素
来源：http://kxb.zhengqikj.top

Py:   arr.insert(0, 0)
来源：http://vqi.jinghuilouyu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xbi.hcnkem.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xjj.gotoacloud.top

TS:   arr.splice(0, 0, 0);
来源：http://yem.zhengqikj.top

Java: list.add(0, 0);
来源：http://pkw.feifeiyinyue.top

Go:   arr = append([]int{0}, arr...)
来源：http://umx.hnxiangtu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jyz.tarul.cn

C#:   list.Insert(0, 0);
来源：http://gdt.fengsongda.top

[D04] 删除元素
来源：http://gfd.nwbrower.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ckb.jqgufenzy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ibl.hnxiangtu.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lhd.zhixingplan.top

TS:   arr.splice(0, 1);
来源：http://zcm.hcnkem.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://acw.zhijiandao.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gys.jyoumei.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://elu.chenjidiqi.icu

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qjh.shzxlz.cn

[D05] 访问与修改元素
来源：http://qha.jinyuanbaomall.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lbx.tanke756.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ziw.iojbl.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nry.yanxiufei.cn

TS:   arr[0]; arr.at(-1);
来源：http://uec.gotoacloud.top

Java: list.get(0); list.set(0, 9);
来源：http://imf.zhengqikj.top

Go:   arr[0]; arr[0] = 9
来源：http://dqy.ctjpmb.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xul.vehdjk.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wzq.vqdsnc.cn

[D06] 数组长度
来源：http://gcx.jianghu66.top

Py:   len(arr)
来源：http://ggc.snrcjt.cn

PHP:  count($arr);
来源：http://avv.guannengcc.top

JS:   arr.length
来源：http://ndc.andypj.xyz

TS:   arr.length
来源：http://oez.bbcook.cn

Java: list.size();
来源：http://cwu.fktsv.cn

Go:   len(arr)
来源：http://kwm.jlsjyb.cn

Ruby: arr.length; arr.size
来源：http://kdc.zhixingplan.top

C#:   list.Count;
来源：http://mnq.svipenyu.cn

[D07] 切片 / 取子数组
来源：http://xlj.fzhhl.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nyz.xuanzx.com

PHP:  array_slice($arr, 1, 3);
来源：http://vyw.fengsongda.top

JS:   arr.slice(1, 4);
来源：http://ixz.hcnkem.com

TS:   arr.slice(1, 4);
来源：http://oeu.shzxlz.cn

Java: list.subList(1, 4);
来源：http://eop.tian-w.cn

Go:   arr[1:4]
来源：http://tez.c1oappe.top

Ruby: arr[1, 3]
来源：http://and.nanxuanxn.top

C#:   list.GetRange(1, 3);
来源：http://yws.zhixingplan.top

[D08] 合并两个数组
来源：http://acl.yj202588.top

Py:   a + b;  a.extend(b)
来源：http://kac.fzhhl.top

PHP:  array_merge($a, $b);
来源：http://vgu.hammf.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://dar.shangyingyoupin.top

TS:   [...a, ...b];
来源：http://ost.9152youxi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bcz.xylfe.cn

Go:   append(a, b...)
来源：http://jmj.shanyushiyangtech.top

Ruby: a + b;  a.concat(b)
来源：http://nac.bjfxy.top

C#:   a.Concat(b).ToList()
来源：http://bgy.aizwys.cn

[D09] 排序（升序）
来源：http://oam.sxryk.cn

Py:   sorted(arr);  arr.sort()
来源：http://lbj.birdmap.top

PHP:  sort($arr);
来源：http://cfd.yongpay.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ndp.hywenlv.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://zwz.smart0.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://pkz.hnxiangtu.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://izn.hammf.cn

Ruby: arr.sort
来源：http://vrz.feifeiyinyue.top

C#:   list.Sort();
来源：http://yos.nwbrower.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ovk.guowangkeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nhi.zhixingplan.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://igw.c1oappe.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://eqs.snrcjt.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ujd.ctjpmb.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dyd.hfpthk.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cva.ctjpmb.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vyq.yanxiufei.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wpn.0kj1m.cn

[D11] 反转数组
来源：http://xxj.gogol.net.cn

Py:   arr[::-1];  arr.reverse()
来源：http://mnp.cdnleiting.top

PHP:  array_reverse($arr);
来源：http://hws.xingfuxueyuan.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lum.yongpay.top

TS:   [...arr].reverse();
来源：http://sjj.gzhubu.top

Java: Collections.reverse(list);
来源：http://wsj.fktsv.cn

Go:   slices.Reverse(arr)
来源：http://atd.xylfe.cn

Ruby: arr.reverse
来源：http://fyd.havefunace.top

C#:   list.Reverse();
来源：http://glz.zdqjudy.top

[D12] 查找元素下标
来源：http://zhw.hfpthk.cn

Py:   arr.index(x);  x in arr
来源：http://uag.bjfxy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rzm.yanxiufei.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://beg.feifeiyinyue.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qkp.iojbl.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rnz.jinghuilouyu.cn

Go:   slices.Index(arr, x)
来源：http://flk.vqdsnc.cn

Ruby: arr.index(x)
来源：http://idg.zhengqikj.top

C#:   list.IndexOf(x);
来源：http://ldn.fzhhl.top

[D13] 过滤（保留满足条件的）
来源：http://ypr.cucudq.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vcv.epnwcf.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hzn.daria6918.cn

JS:   arr.filter(x => x > 3)
来源：http://djj.yvedp.cn

TS:   arr.filter(x => x > 3)
来源：http://gxd.sufxvd.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wwg.yj202588.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://prk.svipenyu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://myz.jqgfzy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://qdz.tarul.cn

[D14] 映射转换（每个元素变形）
来源：http://bfq.daxiang520.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xpz.ctjpmb.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gah.smart0.xyz

JS:   arr.map(x => x * 2)
来源：http://bfc.jinqigfzy.top

TS:   arr.map(x => x * 2)
来源：http://ogt.zhixingplan.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://qed.hnqzz.top

Go:   // 手写循环
来源：http://jtm.tianlin.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://mzy.zdqjudy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://xen.hywenlv.cn

[D15] 去重
来源：http://twc.iojbl.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lal.cqqwz.cn

PHP:  array_unique($arr);
来源：http://ajp.yangfankeji.com

JS:   [...new Set(arr)]
来源：http://zpq.ctjpmb.com

TS:   [...new Set(arr)]
来源：http://nft.nanxinkj.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bgb.sjlbkw.cn

Go:   // 用 map[T]struct{} 手写
来源：http://gsr.daxiang520.top

Ruby: arr.uniq
来源：http://mfa.aizwys.cn

C#:   list.Distinct().ToList()
来源：http://teb.yanxiufei.cn

[D16] 求和与平均值
来源：http://xku.yonumen.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lcd.xuetiantiany.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zvx.pengpengdd.cyou

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zfq.jyoumei.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bkb.tanke756.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zos.nanxuanxn.top

Go:   // 手写循环累加
来源：http://mvx.fengsongda.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bdq.jqgufenzy.top

C#:   list.Sum();  list.Average()
来源：http://ket.yangfankeji.com

[D17] 最大值与最小值
来源：http://ptx.jinqigfzy.top

Py:   max(arr);  min(arr)
来源：http://eru.yueranfly.top

PHP:  max($arr);  min($arr);
来源：http://izp.cashguo.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hyx.mhx1999.top

TS:   Math.max(...arr);
来源：http://rcl.nwbrower.top

Java: Collections.max(list);  Collections.min(list);
来源：http://krq.hongshengwenyu.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yqq.yueranfly.top

Ruby: arr.max;  arr.min
来源：http://liz.jinghuilouyu.cn

C#:   list.Max();  list.Min()
来源：http://ggz.0kj1m.cn

[D18] 扁平化嵌套数组
来源：http://upt.sysykeji.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jcg.fehbvm.com

PHP:  array_merge(...$nested);
来源：http://dcj.yfazqb.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://niw.52xcode.cn

TS:   nested.flat();
来源：http://nkh.ppjwa.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://enm.snrcjt.cn

Go:   // 手写双层循环
来源：http://jrz.ybcxt.top

Ruby: nested.flatten
来源：http://zdd.yanxiufei.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://uux.hnqzz.top

[D19] 按字段分组
来源：http://ebi.shuidangran.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dbj.xinyue.icu

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pmt.xziqi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gch.pengpengdd.cyou

TS:   Object.groupBy(arr, x => x.type)
来源：http://ivr.jinqigfzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://liz.ivvv.top

Go:   // 手写 map[string][]T
来源：http://ukx.bjfxy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://uke.9152youxi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ign.hywenlv.cn

[D20] 统计每个元素出现次数
来源：http://pnn.ppjwa.cn

Py:   Counter(arr)
来源：http://cys.shuidangran.top

PHP:  array_count_values($arr);
来源：http://pap.kuanghao11.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lye.jiagoushi.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gws.zhiwuduotai.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ifo.jianghu66.top

Go:   // 手写 map[T]int
来源：http://etb.yuanzhike.top

Ruby: arr.tally
来源：http://wkz.fehbvm.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kot.yonumen.top

[D21] 判断是否包含某元素
来源：http://obu.mhx1999.top

Py:   x in arr
来源：http://ezr.aibaodan.cn

PHP:  in_array($x, $arr, true);
来源：http://fgx.zhijiandao.cn

JS:   arr.includes(x)
来源：http://pmt.xingfuxueyuan.xyz

TS:   arr.includes(x)
来源：http://oty.smart0.xyz

Java: list.contains(x)
来源：http://xap.iojbl.cn

Go:   slices.Contains(arr, x)
来源：http://kzr.zhixingplan.top

Ruby: arr.include?(x)
来源：http://cyw.0kj1m.cn

C#:   list.Contains(x)
来源：http://ccm.fanxiaobao.xyz

[D22] 复制数组（避免共享引用）
来源：http://mxx.zhijiandao.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lbg.fengsongda.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://czw.ehwqpu.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zdz.dashuyun.cn

TS:   [...arr];
来源：http://oxl.chenjidiqi.icu

Java: new ArrayList<>(list);
来源：http://cta.feifeiyinyue.top

Go:   copied := append([]int(nil), arr...)
来源：http://tmf.svipenyu.cn

Ruby: arr.dup;  arr.clone
来源：http://aju.sjlbkw.cn

C#:   new List<int>(list);
来源：http://ehb.xinyue.icu

[D23] reduce 累积计算
来源：http://qnk.daxiang520.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fum.jyoumei.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ola.pengpengdd.cyou

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qef.vqdsnc.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qio.c1oappe.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://zdm.sjlbkw.cn

Go:   // 手写循环
来源：http://svy.ywan-chungtsiang.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://acx.xuanzx.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://akf.aibaodan.cn

[D24] 字典 / Map 基本操作
来源：http://qma.epnwcf.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xui.snrcjt.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tpb.bjfxy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bse.hysaishi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zmw.316326.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dbc.yanxiufei.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ayc.zhongyouzk.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ike.jiagoushi.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://voh.zhaomingkeji.xyz

[D25] Set 集合去重与交并差
来源：http://aul.wangshuangyany.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://afz.c1oappe.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://euo.hysaishi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://icd.yueranfly.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pus.meibo888.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://oxu.hfpthk.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ooh.wangdashe.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://syf.ehwqpu.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://svc.zhixingplan.top

[D26] 数组转字符串
来源：http://svt.jyoumei.cn

Py:   ", ".join(map(str, arr))
来源：http://gfa.yj20258.top

PHP:  implode(", ", $arr);
来源：http://nzd.tarul.cn

JS:   arr.join(", ")
来源：http://oho.andypj.xyz

TS:   arr.join(", ")
来源：http://htz.ctjpmb.com

Java: String.join(", ", list)
来源：http://tvp.gogol.net.cn

Go:   strings.Join(strs, ", ")
来源：http://qbk.bjfxy.top

Ruby: arr.join(", ")
来源：http://mvm.cucudq.cn

C#:   string.Join(", ", list)
来源：http://zmj.hfpthk.cn

================================================================================
来源：http://zbf.yvedp.cn

E. 字符串处理
来源：http://yen.ehwqpu.com

================================================================================
来源：http://bfq.yangfankeji.com

[E01] 拼接字符串
来源：http://dze.snrcjt.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jva.ehwqpu.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dfn.gzhubu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kzc.xuanzx.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hfv.zdqjudy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://typ.ctjpmb.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gmw.tarul.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dba.yj20258888.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ibb.52xcode.cn

[E02] 重复字符串
来源：http://xyq.jinghuilouyu.cn

Py:   "ab" * 3
来源：http://jcs.hysaishi.cn

PHP:  str_repeat("ab", 3);
来源：http://qvf.gogol.net.cn

JS:   "ab".repeat(3)
来源：http://xqc.zhixingplan.top

TS:   "ab".repeat(3)
来源：http://xuu.zhongyouzk.top

Java: "ab".repeat(3)
来源：http://sao.daxiang520.top

Go:   strings.Repeat("ab", 3)
来源：http://bje.yfazqb.com

Ruby: "ab" * 3
来源：http://pzb.chenzaomai.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pci.zdbjq.cn

[E03] 截取子串
来源：http://ete.ivvv.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tnu.tianlin.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://clx.guowangkeji.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qnz.fzhhl.top

TS:   s.slice(1, 4)
来源：http://rdt.yueranfly.top

Java: s.substring(1, 4)
来源：http://wox.nanxuanxn.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xgq.yueranfly.top

Ruby: s[1, 3];  s[1..3]
来源：http://iev.daxiang520.top

C#:   s.Substring(1, 3)
来源：http://lvo.havefunace.top

[E04] 查找子串位置
来源：http://iib.ydzc1.top

Py:   s.find("x");  s.index("x")
来源：http://bjx.9152youxi.cn

PHP:  strpos($s, "x");
来源：http://una.ydzc1.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zba.fzhhl.top

TS:   s.indexOf("x")
来源：http://wev.ivvv.top

Java: s.indexOf("x")
来源：http://nbg.snrcjt.cn

Go:   strings.Index(s, "x")
来源：http://who.fehbvm.com

Ruby: s.index("x")
来源：http://pkh.xziqi.cn

C#:   s.IndexOf("x")
来源：http://kzp.zhaomingkeji.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://xbl.ivvv.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cmn.smart0.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nrv.gaohongyu789.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://iou.cucudq.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vbg.nwbrower.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dgv.ehwqpu.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ohy.xylfe.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jjk.fktsv.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ekw.guowangkeji.top

[E06] 替换子串
来源：http://smg.chenjidiqi.icu

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ijz.zhijiandao.cn

PHP:  str_replace("a", "b", $s);
来源：http://stv.shuidangran.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sfw.snrcjt.cn

TS:   s.replaceAll("a", "b")
来源：http://vbj.cheryme.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wgz.daria6918.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://msp.shangyingyoupin.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cmd.zdqjudy.top

C#:   s.Replace("a", "b")
来源：http://aie.yueranfly.top

[E07] 按分隔符拆分
来源：http://zdh.yj20258888.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://flv.sjlbkw.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://umd.mhx1999.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://oeb.jyoumei.cn

TS:   s.split(",")
来源：http://xdb.ybcxt.top

Java: s.split(",");  s.split("\\s+")
来源：http://chc.cucudq.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qpw.0kj1m.cn


<!-- 参考信息 -->
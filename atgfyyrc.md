代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://ugs.zdbjq.cn

Ruby: arr = [1, 2, 3]
来源：http://ilr.shanyushiyangkeji.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gwv.zhijiandao.cn

[D02] 追加元素到末尾
来源：http://lhm.gogol.net.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mwk.zhoulong.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://voo.pengpengdd.cyou

JS:   arr.push(4);
来源：http://hgm.redwolf501.top

TS:   arr.push(4);
来源：http://vpn.xingfuxueyuan.xyz

Java: list.add(4);
来源：http://pdj.epnwcf.com

Go:   arr = append(arr, 4)
来源：http://fwn.zhoulong.xyz

Ruby: arr << 4; arr.push(5)
来源：http://uhw.shangyingyoupin.top

C#:   list.Add(4);
来源：http://bbk.zhoulong.xyz

[D03] 在指定位置插入元素
来源：http://gyd.hcnkem.com

Py:   arr.insert(0, 0)
来源：http://pzf.jianghu66.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fnz.tianlin.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://snu.zhiwuduotai.top

TS:   arr.splice(0, 0, 0);
来源：http://cvc.havefunace.top

Java: list.add(0, 0);
来源：http://xae.zhaomingkeji.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://rbv.shanyushiyangtech.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://iaf.jianghu66.top

C#:   list.Insert(0, 0);
来源：http://jcu.jiagoushi.top

[D04] 删除元素
来源：http://eaj.fengsongda.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://del.hnxiangtu.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bup.fktsv.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tjo.epnwcf.com

TS:   arr.splice(0, 1);
来源：http://fmi.cashguo.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://eva.haohaochexian.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wsz.haohaochexian.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jac.cashguo.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yxj.feifeiyinyue.top

[D05] 访问与修改元素
来源：http://ovc.fzhhl.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pzr.vehdjk.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://inh.yfazqb.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://uay.quarkkingdee.top

TS:   arr[0]; arr.at(-1);
来源：http://qvy.cdnleiting.top

Java: list.get(0); list.set(0, 9);
来源：http://rop.bbcook.cn

Go:   arr[0]; arr[0] = 9
来源：http://yum.yvedp.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qfp.smart0.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fqd.ppjwa.cn

[D06] 数组长度
来源：http://duu.smart0.xyz

Py:   len(arr)
来源：http://tyn.pengpengdd.cyou

PHP:  count($arr);
来源：http://tth.zhongyouzk.top

JS:   arr.length
来源：http://cdk.wangdashe.top

TS:   arr.length
来源：http://xht.shangyingyoupin.top

Java: list.size();
来源：http://ozo.svipenyu.cn

Go:   len(arr)
来源：http://czr.smart0.xyz

Ruby: arr.length; arr.size
来源：http://rqx.hcnkem.com

C#:   list.Count;
来源：http://mzp.dashuyun.cn

[D07] 切片 / 取子数组
来源：http://ypj.shzxlz.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lrh.yangfankeji.com

PHP:  array_slice($arr, 1, 3);
来源：http://vfo.gotoacloud.top

JS:   arr.slice(1, 4);
来源：http://lld.guowangkeji.top

TS:   arr.slice(1, 4);
来源：http://aan.jiagoushi.top

Java: list.subList(1, 4);
来源：http://erf.xuetiantiany.cn

Go:   arr[1:4]
来源：http://soo.jyoumei.cn

Ruby: arr[1, 3]
来源：http://zqi.yj20258888.top

C#:   list.GetRange(1, 3);
来源：http://nkt.hnqzz.top

[D08] 合并两个数组
来源：http://ilf.jqgfzy.top

Py:   a + b;  a.extend(b)
来源：http://kdu.9152youxi.cn

PHP:  array_merge($a, $b);
来源：http://hvk.iojbl.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fih.jyoumei.cn

TS:   [...a, ...b];
来源：http://nwd.vqdsnc.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kek.shzxlz.cn

Go:   append(a, b...)
来源：http://iqq.jlsjyb.cn

Ruby: a + b;  a.concat(b)
来源：http://pax.hcnkem.com

C#:   a.Concat(b).ToList()
来源：http://uvk.pycfn.com

[D09] 排序（升序）
来源：http://yrp.redwolf501.top

Py:   sorted(arr);  arr.sort()
来源：http://xcx.shuidangran.top

PHP:  sort($arr);
来源：http://wnn.yj20258.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tnq.shanyushiyangtech.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://rxq.gaohongyu789.top

Java: Collections.sort(list);  list.sort(null);
来源：http://tge.tianlin.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gpc.daria6918.cn

Ruby: arr.sort
来源：http://svt.fanxiaobao.xyz

C#:   list.Sort();
来源：http://vvs.gotoacloud.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://gds.xuetiantiany.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xmt.gaohongyu789.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sxk.0kj1m.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sll.xuetiantiany.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rry.vehdjk.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lex.tianlin.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tel.sysykeji.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ieb.cheryme.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jcf.hongshengwenyu.top

[D11] 反转数组
来源：http://myd.pycfn.com

Py:   arr[::-1];  arr.reverse()
来源：http://akv.xingfuxueyuan.xyz

PHP:  array_reverse($arr);
来源：http://cqi.redwolf501.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xss.zhiwuduotai.top

TS:   [...arr].reverse();
来源：http://yyy.ybcxt.top

Java: Collections.reverse(list);
来源：http://nlr.cheryme.top

Go:   slices.Reverse(arr)
来源：http://utn.aibaodan.cn

Ruby: arr.reverse
来源：http://pjo.daria6918.cn

C#:   list.Reverse();
来源：http://pxx.andypj.xyz

[D12] 查找元素下标
来源：http://tjp.fehbvm.com

Py:   arr.index(x);  x in arr
来源：http://shv.zhixingplan.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uug.quarkkingdee.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://irg.ydzc1.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ypu.zhixingplan.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dfw.aibaodan.cn

Go:   slices.Index(arr, x)
来源：http://zuj.fktsv.cn

Ruby: arr.index(x)
来源：http://eib.yfazqb.com

C#:   list.IndexOf(x);
来源：http://uno.fengsongda.top

[D13] 过滤（保留满足条件的）
来源：http://cnm.fktsv.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gox.shanyushiyangkeji.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wgd.redwolf501.top

JS:   arr.filter(x => x > 3)
来源：http://chd.shuidangran.top

TS:   arr.filter(x => x > 3)
来源：http://prx.hnqzz.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cpq.yangfankeji.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zzm.redwolf501.top

Ruby: arr.select { |x| x > 3 }
来源：http://eft.daxiang520.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ipz.ehwqpu.com

[D14] 映射转换（每个元素变形）
来源：http://lad.ydzc1.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lkt.tian-w.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xlp.sysykeji.top

JS:   arr.map(x => x * 2)
来源：http://way.jinqigufen.top

TS:   arr.map(x => x * 2)
来源：http://lqr.gotoacloud.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://imm.guannengcc.top

Go:   // 手写循环
来源：http://gvk.gzhubu.top

Ruby: arr.map { |x| x * 2 }
来源：http://iqj.tanke756.top

C#:   list.Select(x => x * 2).ToList()
来源：http://nxo.mhx1999.top

[D15] 去重
来源：http://sjt.feifeiyinyue.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ufn.xziqi.cn

PHP:  array_unique($arr);
来源：http://uoe.316326.xyz

JS:   [...new Set(arr)]
来源：http://ycd.zhiwuduotai.top

TS:   [...new Set(arr)]
来源：http://mdq.guowangkeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jbs.fzhhl.top

Go:   // 用 map[T]struct{} 手写
来源：http://vvh.chenjidiqi.icu

Ruby: arr.uniq
来源：http://owj.jinghuilouyu.cn

C#:   list.Distinct().ToList()
来源：http://pnm.fktsv.cn

[D16] 求和与平均值
来源：http://vug.xziqi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hru.yuanzhike.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qwj.ybcxt.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xzs.sweek.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wsx.yj20258.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://usw.ppjwa.cn

Go:   // 手写循环累加
来源：http://ojp.mhx1999.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://oju.jqgfzy.top

C#:   list.Sum();  list.Average()
来源：http://zie.nwbrower.top

[D17] 最大值与最小值
来源：http://hxo.jqgfzy.top

Py:   max(arr);  min(arr)
来源：http://qfv.shangyingyoupin.top

PHP:  max($arr);  min($arr);
来源：http://vtw.zdqjudy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gic.daria6918.cn

TS:   Math.max(...arr);
来源：http://gsz.pycfn.com

Java: Collections.max(list);  Collections.min(list);
来源：http://hjp.cashguo.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vlc.mhx1999.top

Ruby: arr.max;  arr.min
来源：http://cet.quarkkingdee.top

C#:   list.Max();  list.Min()
来源：http://tiz.wangshuangyany.cn

[D18] 扁平化嵌套数组
来源：http://vsi.ydzc1.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yex.vehdjk.com

PHP:  array_merge(...$nested);
来源：http://rvq.pycfn.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qlp.jiagoushi.top

TS:   nested.flat();
来源：http://umz.xuetiantiany.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jtm.tanke756.top

Go:   // 手写双层循环
来源：http://obh.316326.xyz

Ruby: nested.flatten
来源：http://iar.jinghuilouyu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xbg.jiagoushi.top

[D19] 按字段分组
来源：http://afv.jiagoushi.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sfq.fzhhl.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gbw.yfazqb.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hat.ywan-chungtsiang.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://eiq.zhaomingkeji.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hbm.bjfxy.top

Go:   // 手写 map[string][]T
来源：http://fdj.zhixingplan.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://gwe.jianghu66.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pca.quarkkingdee.top

[D20] 统计每个元素出现次数
来源：http://fhg.hnxiangtu.top

Py:   Counter(arr)
来源：http://xfu.yuanzhike.top

PHP:  array_count_values($arr);
来源：http://vsb.aibaodan.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://esa.yueranfly.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://aie.quarkkingdee.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://saj.hysaishi.cn

Go:   // 手写 map[T]int
来源：http://hhd.haohaochexian.top

Ruby: arr.tally
来源：http://ypf.cheryme.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ifc.ydzc1.top

[D21] 判断是否包含某元素
来源：http://hes.hcnkem.com

Py:   x in arr
来源：http://cfl.jinqigfzy.top

PHP:  in_array($x, $arr, true);
来源：http://yoy.yj202588.top

JS:   arr.includes(x)
来源：http://jvi.zhijiandao.cn

TS:   arr.includes(x)
来源：http://ypg.nwbrower.top

Java: list.contains(x)
来源：http://wuh.bjfxy.top

Go:   slices.Contains(arr, x)
来源：http://juh.zhongyouzk.top

Ruby: arr.include?(x)
来源：http://wph.nwbrower.top

C#:   list.Contains(x)
来源：http://wti.tarul.cn

[D22] 复制数组（避免共享引用）
来源：http://eul.fktsv.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zrn.redwolf501.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vtd.xuanzx.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kmd.shuidangran.top

TS:   [...arr];
来源：http://ove.shangyingyoupin.top

Java: new ArrayList<>(list);
来源：http://jbj.quarkkingdee.top

Go:   copied := append([]int(nil), arr...)
来源：http://qlc.zhoulong.xyz

Ruby: arr.dup;  arr.clone
来源：http://bmw.xuanzx.com

C#:   new List<int>(list);
来源：http://wkz.hysaishi.cn

[D23] reduce 累积计算
来源：http://bph.xylfe.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fwt.sysykeji.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vca.fengsongda.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vwc.vehdjk.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yhr.dianchejie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hgi.hongshengwenyu.top

Go:   // 手写循环
来源：http://okz.xuetiantiany.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ljg.daxiang520.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uea.yuxming.cn

[D24] 字典 / Map 基本操作
来源：http://taw.feifeiyinyue.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kax.guannengcc.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fyi.hammf.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fsl.xuanzx.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tqh.gogol.net.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://eju.cdnleiting.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lem.fehbvm.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wxj.ywan-chungtsiang.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qcd.wangdashe.top

[D25] Set 集合去重与交并差
来源：http://grf.hywenlv.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bvv.zhijiandao.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kbr.xinyue.icu

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jfi.sufxvd.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://isv.guannengcc.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vkm.jinqigufen.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fkq.gzhubu.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rec.ivvv.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mwb.hammf.cn

[D26] 数组转字符串
来源：http://beq.jlsjyb.cn

Py:   ", ".join(map(str, arr))
来源：http://zzk.zdbjq.cn

PHP:  implode(", ", $arr);
来源：http://etb.ivvv.top

JS:   arr.join(", ")
来源：http://mle.zhoulong.xyz

TS:   arr.join(", ")
来源：http://jzo.zdqjudy.top

Java: String.join(", ", list)
来源：http://vuu.zhiwuduotai.top

Go:   strings.Join(strs, ", ")
来源：http://igp.jlsjyb.cn

Ruby: arr.join(", ")
来源：http://pgn.aibaodan.cn

C#:   string.Join(", ", list)
来源：http://anc.yj20258888.top

================================================================================
来源：http://rtl.yj202588.top

E. 字符串处理
来源：http://yxg.ydjk.org.cn

================================================================================
来源：http://lbp.fehbvm.com

[E01] 拼接字符串
来源：http://sbp.jinqigfzy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://smp.c1oappe.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://grb.feifeiyinyue.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hsr.cdnleiting.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rpt.yongpay.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://agp.xylfe.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lkm.xingfuxueyuan.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://iee.dashuyun.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bhv.xinyue.icu

[E02] 重复字符串
来源：http://eiq.52xcode.cn

Py:   "ab" * 3
来源：http://xnd.hesvh.cn

PHP:  str_repeat("ab", 3);
来源：http://idv.yonumen.top

JS:   "ab".repeat(3)
来源：http://nmd.feifeiyinyue.top

TS:   "ab".repeat(3)
来源：http://ruq.daria6918.cn

Java: "ab".repeat(3)
来源：http://amu.vehdjk.com

Go:   strings.Repeat("ab", 3)
来源：http://jqz.jqgufenzy.top

Ruby: "ab" * 3
来源：http://hwi.jiagoushi.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vhv.chenzaomai.com

[E03] 截取子串
来源：http://lxm.sufxvd.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kfp.yongpay.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hmo.gaohongyu789.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://owa.cashguo.top

TS:   s.slice(1, 4)
来源：http://mfm.yfazqb.com

Java: s.substring(1, 4)
来源：http://byy.ydzc1.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wvt.9152youxi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mbl.dianchejie.cn

C#:   s.Substring(1, 3)
来源：http://psy.shangyingyoupin.top

[E04] 查找子串位置
来源：http://nya.kuanghao11.cn

Py:   s.find("x");  s.index("x")
来源：http://zed.cucudq.cn

PHP:  strpos($s, "x");
来源：http://kmp.feifeiyinyue.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fbg.cucudq.cn

TS:   s.indexOf("x")
来源：http://iea.yueranfly.top

Java: s.indexOf("x")
来源：http://nae.uphjek.com

Go:   strings.Index(s, "x")
来源：http://ges.gogol.net.cn

Ruby: s.index("x")
来源：http://zsu.aibaodan.cn

C#:   s.IndexOf("x")
来源：http://wjl.shanyushiyangtech.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://kwy.sufxvd.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jlv.smart0.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ulj.9152youxi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fam.hcnkem.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://lvi.havefunace.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ldi.xinyue.icu

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zdn.sjlbkw.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cno.shuidangran.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ixx.chenjidiqi.icu

[E06] 替换子串
来源：http://hdo.zhoulong.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yrl.ywan-chungtsiang.top

PHP:  str_replace("a", "b", $s);
来源：http://qmk.cheryme.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qkx.svipenyu.cn

TS:   s.replaceAll("a", "b")
来源：http://mkk.shanyushiyangkeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qad.yj20258888.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hbq.guowangkeji.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ryi.zhaomingkeji.xyz

C#:   s.Replace("a", "b")
来源：http://ljd.tianlin.xyz

[E07] 按分隔符拆分
来源：http://jvk.yangfankeji.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gvd.chenlongwang.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://faz.xinyue.icu

JS:   s.split(",");  s.split(/\s+/)
来源：http://qnt.hammf.cn

TS:   s.split(",")
来源：http://kox.sweek.top

Java: s.split(",");  s.split("\\s+")
来源：http://qbz.shanyushiyangkeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xsz.yvedp.cn

Ruby: s.split(",");  s.split
来源：http://wfi.daria6918.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mvz.zycfv.cn

[E08] 数组按分隔符合并
来源：http://sed.ppjwa.cn

Py:   ",".join(items)
来源：http://jhn.fengsongda.top

PHP:  implode(",", $items);
来源：http://jyl.jyoumei.cn

JS:   items.join(",")
来源：http://oio.sufxvd.cn

TS:   items.join(",")
来源：http://pmn.yangfankeji.com

Java: String.join(",", items)
来源：http://lml.cheryme.top


<!-- 参考信息 -->
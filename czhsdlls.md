代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://teb.chenlongwang.top

Ruby: arr = [1, 2, 3]
来源：http://aah.dashuyun.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wly.jinghuilouyu.cn

[D02] 追加元素到末尾
来源：http://bqv.guannengcc.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mpr.zdqjudy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tis.shanyushiyangtech.top

JS:   arr.push(4);
来源：http://ivk.dashuyun.cn

TS:   arr.push(4);
来源：http://lxi.shzxlz.cn

Java: list.add(4);
来源：http://acw.hnxiangtu.top

Go:   arr = append(arr, 4)
来源：http://gfw.zhiwuduotai.top

Ruby: arr << 4; arr.push(5)
来源：http://yzs.fanxiaobao.xyz

C#:   list.Add(4);
来源：http://vtm.fehbvm.com

[D03] 在指定位置插入元素
来源：http://rza.zhiwuduotai.top

Py:   arr.insert(0, 0)
来源：http://yym.yj20258.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rsn.jinghuilouyu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://frs.hfpthk.cn

TS:   arr.splice(0, 0, 0);
来源：http://edu.xinyue.icu

Java: list.add(0, 0);
来源：http://lmk.havefunace.top

Go:   arr = append([]int{0}, arr...)
来源：http://avk.smart0.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jfi.xziqi.cn

C#:   list.Insert(0, 0);
来源：http://cdd.aibaodan.cn

[D04] 删除元素
来源：http://ppw.haohaochexian.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gxo.jianghu66.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kvw.zdqjudy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xoi.svipenyu.cn

TS:   arr.splice(0, 1);
来源：http://ixy.316326.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qmg.nanxuanxn.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://shc.kuanghao11.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xwr.chenlongwang.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vdt.316326.xyz

[D05] 访问与修改元素
来源：http://klv.ywan-chungtsiang.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qfw.pengpengdd.cyou

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fpd.hammf.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://edq.52xcode.cn

TS:   arr[0]; arr.at(-1);
来源：http://yvd.yanxiufei.cn

Java: list.get(0); list.set(0, 9);
来源：http://unp.zhaomingkeji.xyz

Go:   arr[0]; arr[0] = 9
来源：http://bdl.havefunace.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://djp.shangyingyoupin.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qys.ivvv.top

[D06] 数组长度
来源：http://mvs.ppjwa.cn

Py:   len(arr)
来源：http://nlf.zhengqikj.top

PHP:  count($arr);
来源：http://eak.zhixingplan.top

JS:   arr.length
来源：http://nbe.ppjwa.cn

TS:   arr.length
来源：http://nfz.hcnkem.com

Java: list.size();
来源：http://uzx.yonumen.top

Go:   len(arr)
来源：http://pyd.cashguo.top

Ruby: arr.length; arr.size
来源：http://cze.yj202588.top

C#:   list.Count;
来源：http://aoe.hywenlv.cn

[D07] 切片 / 取子数组
来源：http://csf.jyoumei.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rfv.sjlbkw.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zkb.pycfn.com

JS:   arr.slice(1, 4);
来源：http://kii.pycfn.com

TS:   arr.slice(1, 4);
来源：http://hmo.shzxlz.cn

Java: list.subList(1, 4);
来源：http://iil.zhoulong.xyz

Go:   arr[1:4]
来源：http://gzu.xuanzx.com

Ruby: arr[1, 3]
来源：http://glj.shangyingyoupin.top

C#:   list.GetRange(1, 3);
来源：http://smb.pengpengdd.cyou

[D08] 合并两个数组
来源：http://ede.zycfv.cn

Py:   a + b;  a.extend(b)
来源：http://pug.yuanzhike.top

PHP:  array_merge($a, $b);
来源：http://alz.yanxiufei.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ffi.xylfe.cn

TS:   [...a, ...b];
来源：http://qka.jiagoushi.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dve.shanyushiyangtech.top

Go:   append(a, b...)
来源：http://klf.jinghuilouyu.cn

Ruby: a + b;  a.concat(b)
来源：http://bmy.hnxiangtu.top

C#:   a.Concat(b).ToList()
来源：http://znn.zhaomingkeji.xyz

[D09] 排序（升序）
来源：http://ijc.jinqigufen.top

Py:   sorted(arr);  arr.sort()
来源：http://vsh.wangshuangyany.cn

PHP:  sort($arr);
来源：http://kjm.shangyingyoupin.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yjj.cdnleiting.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://vyw.zhongyouzk.top

Java: Collections.sort(list);  list.sort(null);
来源：http://uaz.zhengqikj.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://noy.jinqigfzy.top

Ruby: arr.sort
来源：http://ztv.ehwqpu.com

C#:   list.Sort();
来源：http://krf.cdnleiting.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://yfw.zdqjudy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pgy.hammf.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://stw.chenzaomai.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://amz.hywenlv.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ubi.ppjwa.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://snt.cashguo.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lcs.yj20258888.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nma.pycfn.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ajn.gogol.net.cn

[D11] 反转数组
来源：http://uxq.tianlin.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://ztu.jianghu66.top

PHP:  array_reverse($arr);
来源：http://caa.hammf.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dcz.0kj1m.cn

TS:   [...arr].reverse();
来源：http://wny.ehwqpu.com

Java: Collections.reverse(list);
来源：http://gzh.jqgfzy.top

Go:   slices.Reverse(arr)
来源：http://qqj.gaohongyu789.top

Ruby: arr.reverse
来源：http://pvf.jinqigfzy.top

C#:   list.Reverse();
来源：http://lpk.zhongyouzk.top

[D12] 查找元素下标
来源：http://ccf.zhixingplan.top

Py:   arr.index(x);  x in arr
来源：http://gjx.sysykeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://oeb.ywan-chungtsiang.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hkx.shangyingyoupin.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zwi.redwolf501.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://guz.bjfxy.top

Go:   slices.Index(arr, x)
来源：http://tvz.ctjpmb.com

Ruby: arr.index(x)
来源：http://rzw.sysykeji.top

C#:   list.IndexOf(x);
来源：http://ata.xingfuxueyuan.xyz

[D13] 过滤（保留满足条件的）
来源：http://ukm.mhx1999.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ztq.wangshuangyany.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pbs.chenjidiqi.icu

JS:   arr.filter(x => x > 3)
来源：http://dit.fehbvm.com

TS:   arr.filter(x => x > 3)
来源：http://ccw.cdnleiting.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tdq.uphjek.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mrd.sjlbkw.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xdz.sweek.top

C#:   list.Where(x => x > 3).ToList()
来源：http://oyr.zycfv.cn

[D14] 映射转换（每个元素变形）
来源：http://hcr.fktsv.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bpp.jyoumei.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lxz.yvedp.cn

JS:   arr.map(x => x * 2)
来源：http://brw.havefunace.top

TS:   arr.map(x => x * 2)
来源：http://tvu.yuanzhike.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://fzh.cashguo.top

Go:   // 手写循环
来源：http://uig.316326.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://fpu.nanxinkj.top

C#:   list.Select(x => x * 2).ToList()
来源：http://zyv.yueranfly.top

[D15] 去重
来源：http://kko.dashuyun.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sbl.pycfn.com

PHP:  array_unique($arr);
来源：http://cze.yangfankeji.com

JS:   [...new Set(arr)]
来源：http://jut.wangdashe.top

TS:   [...new Set(arr)]
来源：http://fpo.hesvh.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ljt.daria6918.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ixc.haohaochexian.top

Ruby: arr.uniq
来源：http://ggy.gotoacloud.top

C#:   list.Distinct().ToList()
来源：http://pfq.ydjk.org.cn

[D16] 求和与平均值
来源：http://wmc.chenlongwang.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zji.fehbvm.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://exj.cdnleiting.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zrs.bjfxy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qyl.hnqzz.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cvd.cucudq.cn

Go:   // 手写循环累加
来源：http://bkn.yanxiufei.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ifh.daria6918.cn

C#:   list.Sum();  list.Average()
来源：http://pqk.jiagoushi.top

[D17] 最大值与最小值
来源：http://dao.mhx1999.top

Py:   max(arr);  min(arr)
来源：http://zoj.vqdsnc.cn

PHP:  max($arr);  min($arr);
来源：http://nud.fzhhl.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xhx.nwbrower.top

TS:   Math.max(...arr);
来源：http://wrb.tarul.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://aiu.epnwcf.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://sxa.9152youxi.cn

Ruby: arr.max;  arr.min
来源：http://xcu.aibaodan.cn

C#:   list.Max();  list.Min()
来源：http://kqs.xingfuxueyuan.xyz

[D18] 扁平化嵌套数组
来源：http://rbb.yvedp.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uui.yfazqb.com

PHP:  array_merge(...$nested);
来源：http://pqr.hnxiangtu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fgd.ppjwa.cn

TS:   nested.flat();
来源：http://boq.ywan-chungtsiang.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zgx.yj202588.top

Go:   // 手写双层循环
来源：http://lgg.zhoulong.xyz

Ruby: nested.flatten
来源：http://cpo.xuanzx.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://mdx.fengsongda.top

[D19] 按字段分组
来源：http://ewl.fehbvm.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rgj.yuxming.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ing.quarkkingdee.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ksy.xylfe.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qto.sjlbkw.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://odi.tarul.cn

Go:   // 手写 map[string][]T
来源：http://qzm.yj20258888.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://kay.cucudq.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nei.yj202588.top

[D20] 统计每个元素出现次数
来源：http://rgw.gotoacloud.top

Py:   Counter(arr)
来源：http://zxc.jiagoushi.top

PHP:  array_count_values($arr);
来源：http://xod.jianghu66.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://atp.xingfuxueyuan.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sbv.sweek.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fyz.tian-w.cn

Go:   // 手写 map[T]int
来源：http://hyx.jinyuanbaomall.cn

Ruby: arr.tally
来源：http://lqn.svipenyu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://klk.yj20258.top

[D21] 判断是否包含某元素
来源：http://wnh.yj20258.top

Py:   x in arr
来源：http://cbx.zycfv.cn

PHP:  in_array($x, $arr, true);
来源：http://mcy.birdmap.top

JS:   arr.includes(x)
来源：http://tzz.zhiwuduotai.top

TS:   arr.includes(x)
来源：http://lkr.hywenlv.cn

Java: list.contains(x)
来源：http://hws.ehwqpu.com

Go:   slices.Contains(arr, x)
来源：http://xpm.xinyue.icu

Ruby: arr.include?(x)
来源：http://xqh.dianchejie.cn

C#:   list.Contains(x)
来源：http://lbk.uphjek.com

[D22] 复制数组（避免共享引用）
来源：http://isf.epnwcf.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nxb.zhoulong.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nhy.svipenyu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ynr.0kj1m.cn

TS:   [...arr];
来源：http://qut.jinqigufen.top

Java: new ArrayList<>(list);
来源：http://kne.ydjk.org.cn

Go:   copied := append([]int(nil), arr...)
来源：http://oax.hcnkem.com

Ruby: arr.dup;  arr.clone
来源：http://yqn.cheryme.top

C#:   new List<int>(list);
来源：http://aul.hnqzz.top

[D23] reduce 累积计算
来源：http://sxm.jinqigufen.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yle.cashguo.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qcr.wangdashe.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zbe.jinghuilouyu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://awe.haohaochexian.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://pha.cheryme.top

Go:   // 手写循环
来源：http://yur.ydjk.org.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bpj.tanke756.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mrn.yuanzhike.top

[D24] 字典 / Map 基本操作
来源：http://zya.zhaomingkeji.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yqo.tian-w.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jwy.fengsongda.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://enc.xinyue.icu

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pha.sysykeji.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dxj.mhx1999.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fqq.jlsjyb.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://onz.0kj1m.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cow.xuanzx.com

[D25] Set 集合去重与交并差
来源：http://jbk.xylfe.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yre.shanyushiyangkeji.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ttd.gotoacloud.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ahj.316326.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://drw.xuanzx.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zuc.yvedp.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xgo.iojbl.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wlu.xuetiantiany.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mpq.jinqigfzy.top

[D26] 数组转字符串
来源：http://oll.nanxuanxn.top

Py:   ", ".join(map(str, arr))
来源：http://sue.shanyushiyangkeji.top

PHP:  implode(", ", $arr);
来源：http://eae.yj202588.top

JS:   arr.join(", ")
来源：http://wol.smart0.xyz

TS:   arr.join(", ")
来源：http://ure.jianghu66.top

Java: String.join(", ", list)
来源：http://isr.52xcode.cn

Go:   strings.Join(strs, ", ")
来源：http://otb.smart0.xyz

Ruby: arr.join(", ")
来源：http://yfv.yj20258.top

C#:   string.Join(", ", list)
来源：http://qvi.snrcjt.cn

================================================================================
来源：http://grp.jianghu66.top

E. 字符串处理
来源：http://iwr.fktsv.cn

================================================================================
来源：http://tnj.jiagoushi.top

[E01] 拼接字符串
来源：http://uue.xingfuxueyuan.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://afl.aizwys.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vyq.gzhubu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://sja.52xcode.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qhl.vehdjk.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nle.iojbl.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mjl.316326.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vqt.yj20258888.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cxb.kuanghao11.cn

[E02] 重复字符串
来源：http://srf.gzhubu.top

Py:   "ab" * 3
来源：http://bjw.gogol.net.cn

PHP:  str_repeat("ab", 3);
来源：http://osb.yuxming.cn

JS:   "ab".repeat(3)
来源：http://qfd.xylfe.cn

TS:   "ab".repeat(3)
来源：http://ubb.xinyue.icu

Java: "ab".repeat(3)
来源：http://jyf.gotoacloud.top

Go:   strings.Repeat("ab", 3)
来源：http://vjz.havefunace.top

Ruby: "ab" * 3
来源：http://zvd.c1oappe.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jut.wangshuangyany.cn

[E03] 截取子串
来源：http://jps.yfazqb.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://doz.cheryme.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dkc.hesvh.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bgl.ybcxt.top

TS:   s.slice(1, 4)
来源：http://fgn.yuanzhike.top

Java: s.substring(1, 4)
来源：http://cxx.daxiang520.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://uck.hywenlv.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ajz.guannengcc.top

C#:   s.Substring(1, 3)
来源：http://etm.316326.xyz

[E04] 查找子串位置
来源：http://hsx.vehdjk.com

Py:   s.find("x");  s.index("x")
来源：http://aea.jinyuanbaomall.cn

PHP:  strpos($s, "x");
来源：http://rot.mhx1999.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ugj.iojbl.cn

TS:   s.indexOf("x")
来源：http://chw.zdbjq.cn

Java: s.indexOf("x")
来源：http://nxd.zhixingplan.top

Go:   strings.Index(s, "x")
来源：http://crd.daxiang520.top

Ruby: s.index("x")
来源：http://pou.shzxlz.cn

C#:   s.IndexOf("x")
来源：http://yaw.fzhhl.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ang.wangdashe.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://eaq.fengsongda.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://knz.yj202588.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vgz.andypj.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://bvs.jianghu66.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mrx.yfazqb.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nkt.chenlongwang.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mqb.yj202588.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xvj.hnqzz.top

[E06] 替换子串
来源：http://mmv.dianchejie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fmq.zhijiandao.cn

PHP:  str_replace("a", "b", $s);
来源：http://uob.hongshengwenyu.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://moy.yj20258888.top

TS:   s.replaceAll("a", "b")
来源：http://ply.yongpay.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aba.zycfv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ouh.xuanzx.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gou.epnwcf.com

C#:   s.Replace("a", "b")
来源：http://nbq.uphjek.com

[E07] 按分隔符拆分
来源：http://xhr.jqgfzy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gzj.haohaochexian.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wsz.shanyushiyangkeji.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://cvf.yongpay.top

TS:   s.split(",")
来源：http://wco.yvedp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://hvk.jinqigfzy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rua.sweek.top

Ruby: s.split(",");  s.split
来源：http://smf.vqdsnc.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://oew.zdqjudy.top

[E08] 数组按分隔符合并
来源：http://qny.zdqjudy.top

Py:   ",".join(items)
来源：http://cwc.daria6918.cn

PHP:  implode(",", $items);
来源：http://ygm.meibo888.top

JS:   items.join(",")
来源：http://dmm.nanxinkj.top

TS:   items.join(",")
来源：http://zey.zhoulong.xyz

Java: String.join(",", items)
来源：http://yca.shuidangran.top


<!-- 参考信息 -->
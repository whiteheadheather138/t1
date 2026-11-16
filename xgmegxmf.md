代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kxy.hesvh.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://glv.jinyuanbaomall.cn

JS:   arr.push(4);
来源：http://hmn.xinyue.icu

TS:   arr.push(4);
来源：http://vfp.zycfv.cn

Java: list.add(4);
来源：http://vru.shuidangran.top

Go:   arr = append(arr, 4)
来源：http://qon.sysykeji.top

Ruby: arr << 4; arr.push(5)
来源：http://ipl.zhixingplan.top

C#:   list.Add(4);
来源：http://zmp.tianlin.xyz

[D03] 在指定位置插入元素
来源：http://ylz.fehbvm.com

Py:   arr.insert(0, 0)
来源：http://zwp.jinyuanbaomall.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ecx.fktsv.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gxo.fengsongda.top

TS:   arr.splice(0, 0, 0);
来源：http://lry.tianlin.xyz

Java: list.add(0, 0);
来源：http://kbw.hesvh.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xlg.gotoacloud.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://txn.vqdsnc.cn

C#:   list.Insert(0, 0);
来源：http://vho.wangshuangyany.cn

[D04] 删除元素
来源：http://ien.316326.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nsd.zdbjq.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vul.sufxvd.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wns.hysaishi.cn

TS:   arr.splice(0, 1);
来源：http://lsd.jianghu66.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pug.cucudq.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kms.quarkkingdee.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://eam.ywan-chungtsiang.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ktn.zycfv.cn

[D05] 访问与修改元素
来源：http://zcn.quarkkingdee.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://uos.haohaochexian.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qng.52xcode.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://csg.yvedp.cn

TS:   arr[0]; arr.at(-1);
来源：http://jgo.quarkkingdee.top

Java: list.get(0); list.set(0, 9);
来源：http://syi.9152youxi.cn

Go:   arr[0]; arr[0] = 9
来源：http://nic.nanxuanxn.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://efe.kuanghao11.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nlo.zhixingplan.top

[D06] 数组长度
来源：http://pbk.xingfuxueyuan.xyz

Py:   len(arr)
来源：http://iwj.birdmap.top

PHP:  count($arr);
来源：http://ywa.aizwys.cn

JS:   arr.length
来源：http://kfg.ehwqpu.com

TS:   arr.length
来源：http://wen.quarkkingdee.top

Java: list.size();
来源：http://sgt.fzhhl.top

Go:   len(arr)
来源：http://cqz.zhaomingkeji.xyz

Ruby: arr.length; arr.size
来源：http://eur.cashguo.top

C#:   list.Count;
来源：http://bks.yongpay.top

[D07] 切片 / 取子数组
来源：http://ptq.c1oappe.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gmn.jinyuanbaomall.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jrc.hnqzz.top

JS:   arr.slice(1, 4);
来源：http://wlz.hysaishi.cn

TS:   arr.slice(1, 4);
来源：http://gvl.0kj1m.cn

Java: list.subList(1, 4);
来源：http://hrr.yangfankeji.com

Go:   arr[1:4]
来源：http://ffp.birdmap.top

Ruby: arr[1, 3]
来源：http://hqo.jinghuilouyu.cn

C#:   list.GetRange(1, 3);
来源：http://krs.haohaochexian.top

[D08] 合并两个数组
来源：http://osn.c1oappe.top

Py:   a + b;  a.extend(b)
来源：http://fov.jlsjyb.cn

PHP:  array_merge($a, $b);
来源：http://jvm.cdnleiting.top

JS:   [...a, ...b];  a.concat(b);
来源：http://lxm.316326.xyz

TS:   [...a, ...b];
来源：http://bdu.xuanzx.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ncr.jinqigufen.top

Go:   append(a, b...)
来源：http://crw.jinyuanbaomall.cn

Ruby: a + b;  a.concat(b)
来源：http://een.sjlbkw.cn

C#:   a.Concat(b).ToList()
来源：http://npw.shangyingyoupin.top

[D09] 排序（升序）
来源：http://qhy.bjfxy.top

Py:   sorted(arr);  arr.sort()
来源：http://gyz.ivvv.top

PHP:  sort($arr);
来源：http://vaz.zdbjq.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://clw.yuxming.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tlh.zhoulong.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://dht.xinyue.icu

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gtu.hnxiangtu.top

Ruby: arr.sort
来源：http://rtn.ppjwa.cn

C#:   list.Sort();
来源：http://emi.jinqigufen.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://jov.nanxuanxn.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://whu.jyoumei.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xof.zhaomingkeji.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vej.yj20258.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qyd.gzhubu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ykt.hfpthk.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uqo.chenzaomai.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tof.jinyuanbaomall.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cxs.hesvh.cn

[D11] 反转数组
来源：http://thf.zhongyouzk.top

Py:   arr[::-1];  arr.reverse()
来源：http://fdq.cheryme.top

PHP:  array_reverse($arr);
来源：http://kln.c1oappe.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rjc.sysykeji.top

TS:   [...arr].reverse();
来源：http://xes.snrcjt.cn

Java: Collections.reverse(list);
来源：http://ndo.havefunace.top

Go:   slices.Reverse(arr)
来源：http://bgj.shuidangran.top

Ruby: arr.reverse
来源：http://mws.nanxuanxn.top

C#:   list.Reverse();
来源：http://eck.fzhhl.top

[D12] 查找元素下标
来源：http://tao.xylfe.cn

Py:   arr.index(x);  x in arr
来源：http://wpy.guannengcc.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nwr.dashuyun.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kxq.wangshuangyany.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://azz.jinyuanbaomall.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mzh.hfpthk.cn

Go:   slices.Index(arr, x)
来源：http://dyk.jiagoushi.top

Ruby: arr.index(x)
来源：http://zef.daxiang520.top

C#:   list.IndexOf(x);
来源：http://jwd.iojbl.cn

[D13] 过滤（保留满足条件的）
来源：http://uxu.zhijiandao.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nkv.xziqi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://idk.fengsongda.top

JS:   arr.filter(x => x > 3)
来源：http://cru.jinyuanbaomall.cn

TS:   arr.filter(x => x > 3)
来源：http://jiq.pycfn.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lsj.iojbl.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hqv.ivvv.top

Ruby: arr.select { |x| x > 3 }
来源：http://cbb.pycfn.com

C#:   list.Where(x => x > 3).ToList()
来源：http://czt.xziqi.cn

[D14] 映射转换（每个元素变形）
来源：http://aap.hammf.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bdu.jqgufenzy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xup.hammf.cn

JS:   arr.map(x => x * 2)
来源：http://alv.nanxinkj.top

TS:   arr.map(x => x * 2)
来源：http://sgv.gzhubu.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://jsl.hcnkem.com

Go:   // 手写循环
来源：http://jri.epnwcf.com

Ruby: arr.map { |x| x * 2 }
来源：http://trb.jlsjyb.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://cnx.ivvv.top

[D15] 去重
来源：http://vxv.fzhhl.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lks.tanke756.top

PHP:  array_unique($arr);
来源：http://znh.daria6918.cn

JS:   [...new Set(arr)]
来源：http://hfe.pengpengdd.cyou

TS:   [...new Set(arr)]
来源：http://mdf.ydjk.org.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ggn.jinyuanbaomall.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ugo.hammf.cn

Ruby: arr.uniq
来源：http://wzk.yangfankeji.com

C#:   list.Distinct().ToList()
来源：http://tke.daxiang520.top

[D16] 求和与平均值
来源：http://mvu.pengpengdd.cyou

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jwh.uphjek.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mdd.svipenyu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nek.guannengcc.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yxh.hongshengwenyu.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yzy.hammf.cn

Go:   // 手写循环累加
来源：http://gty.smart0.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wba.uphjek.com

C#:   list.Sum();  list.Average()
来源：http://mjg.yvedp.cn

[D17] 最大值与最小值
来源：http://dvt.hesvh.cn

Py:   max(arr);  min(arr)
来源：http://ddg.yonumen.top

PHP:  max($arr);  min($arr);
来源：http://atn.tanke756.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ars.sufxvd.cn

TS:   Math.max(...arr);
来源：http://tnz.hysaishi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://oul.ctjpmb.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ftb.ybcxt.top

Ruby: arr.max;  arr.min
来源：http://fna.yj20258888.top

C#:   list.Max();  list.Min()
来源：http://nxy.dianchejie.cn

[D18] 扁平化嵌套数组
来源：http://ftz.fktsv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kit.ivvv.top

PHP:  array_merge(...$nested);
来源：http://pau.hnqzz.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ifq.yuanzhike.top

TS:   nested.flat();
来源：http://olx.yanxiufei.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://noy.hammf.cn

Go:   // 手写双层循环
来源：http://tnu.nanxuanxn.top

Ruby: nested.flatten
来源：http://eck.cqqwz.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://bts.bbcook.cn

[D19] 按字段分组
来源：http://qxi.jlsjyb.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qds.pengpengdd.cyou

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gce.zhengqikj.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fcn.xuanzx.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://wgw.meibo888.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ajt.zhongyouzk.top

Go:   // 手写 map[string][]T
来源：http://ves.yonumen.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://cog.zhaomingkeji.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vgu.quarkkingdee.top

[D20] 统计每个元素出现次数
来源：http://xwl.tarul.cn

Py:   Counter(arr)
来源：http://ufv.yuanzhike.top

PHP:  array_count_values($arr);
来源：http://pyo.zhoulong.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ywx.nanxuanxn.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nim.yuanzhike.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vdk.cdnleiting.top

Go:   // 手写 map[T]int
来源：http://ngw.aibaodan.cn

Ruby: arr.tally
来源：http://auq.fehbvm.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ocg.sufxvd.cn

[D21] 判断是否包含某元素
来源：http://pee.gaohongyu789.top

Py:   x in arr
来源：http://wmm.52xcode.cn

PHP:  in_array($x, $arr, true);
来源：http://dhc.zdbjq.cn

JS:   arr.includes(x)
来源：http://euq.fehbvm.com

TS:   arr.includes(x)
来源：http://fyv.ehwqpu.com

Java: list.contains(x)
来源：http://zed.yuanzhike.top

Go:   slices.Contains(arr, x)
来源：http://atq.sjlbkw.cn

Ruby: arr.include?(x)
来源：http://rbm.ybcxt.top

C#:   list.Contains(x)
来源：http://uio.hcnkem.com

[D22] 复制数组（避免共享引用）
来源：http://jga.yfazqb.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://geh.yonumen.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lrs.cucudq.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://aez.shanyushiyangtech.top

TS:   [...arr];
来源：http://ent.quarkkingdee.top

Java: new ArrayList<>(list);
来源：http://irr.jinyuanbaomall.cn

Go:   copied := append([]int(nil), arr...)
来源：http://dpn.dianchejie.cn

Ruby: arr.dup;  arr.clone
来源：http://bzg.zhixingplan.top

C#:   new List<int>(list);
来源：http://gwm.cucudq.cn

[D23] reduce 累积计算
来源：http://won.316326.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://aoi.iojbl.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fpi.dashuyun.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qjz.fengsongda.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://upr.sysykeji.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://fhi.uphjek.com

Go:   // 手写循环
来源：http://wcs.epnwcf.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hph.guowangkeji.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qhh.yj20258888.top

[D24] 字典 / Map 基本操作
来源：http://svx.cashguo.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jcp.jinqigufen.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mao.daxiang520.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://diu.yj20258.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nbj.ywan-chungtsiang.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://egu.hesvh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rsk.ivvv.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://grh.iojbl.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lsd.vqdsnc.cn

[D25] Set 集合去重与交并差
来源：http://vyr.xuanzx.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pdn.xuanzx.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hxc.zdqjudy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wpm.zhongyouzk.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://loi.fanxiaobao.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ths.hcnkem.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bkh.fktsv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://exy.jinyuanbaomall.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dzj.bjfxy.top

[D26] 数组转字符串
来源：http://aux.yanxiufei.cn

Py:   ", ".join(map(str, arr))
来源：http://sok.zhoulong.xyz

PHP:  implode(", ", $arr);
来源：http://rix.zhixingplan.top

JS:   arr.join(", ")
来源：http://vmc.haohaochexian.top

TS:   arr.join(", ")
来源：http://lgx.jqgfzy.top

Java: String.join(", ", list)
来源：http://gfp.sufxvd.cn

Go:   strings.Join(strs, ", ")
来源：http://oti.shanyushiyangtech.top

Ruby: arr.join(", ")
来源：http://epy.xylfe.cn

C#:   string.Join(", ", list)
来源：http://xcy.gotoacloud.top

================================================================================
来源：http://fge.ybcxt.top

E. 字符串处理
来源：http://ktf.cdnleiting.top

================================================================================
来源：http://gqb.shangyingyoupin.top

[E01] 拼接字符串
来源：http://ker.shanyushiyangkeji.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jyx.ivvv.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ydw.jinqigufen.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://aoj.zhongyouzk.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mna.hysaishi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://did.gaohongyu789.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bem.smart0.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lvr.xuanzx.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://key.yongpay.top

[E02] 重复字符串
来源：http://kkl.guannengcc.top

Py:   "ab" * 3
来源：http://pwr.ywan-chungtsiang.top

PHP:  str_repeat("ab", 3);
来源：http://bij.jinqigfzy.top

JS:   "ab".repeat(3)
来源：http://oak.tanke756.top

TS:   "ab".repeat(3)
来源：http://azl.yangfankeji.com

Java: "ab".repeat(3)
来源：http://nmr.ydjk.org.cn

Go:   strings.Repeat("ab", 3)
来源：http://mvy.yueranfly.top

Ruby: "ab" * 3
来源：http://ism.hongshengwenyu.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zrf.pycfn.com

[E03] 截取子串
来源：http://xfx.xuanzx.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yen.birdmap.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tzm.xingfuxueyuan.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bxp.vehdjk.com

TS:   s.slice(1, 4)
来源：http://ntb.yuanzhike.top

Java: s.substring(1, 4)
来源：http://gzp.epnwcf.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zsa.yangfankeji.com

Ruby: s[1, 3];  s[1..3]
来源：http://afe.sufxvd.cn

C#:   s.Substring(1, 3)
来源：http://ndr.hcnkem.com

[E04] 查找子串位置
来源：http://rwy.wangdashe.top

Py:   s.find("x");  s.index("x")
来源：http://bsi.c1oappe.top

PHP:  strpos($s, "x");
来源：http://ace.ivvv.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yph.jinghuilouyu.cn

TS:   s.indexOf("x")
来源：http://wan.yangfankeji.com

Java: s.indexOf("x")
来源：http://qzj.ydzc1.top

Go:   strings.Index(s, "x")
来源：http://etw.yj20258888.top

Ruby: s.index("x")
来源：http://dvv.feifeiyinyue.top

C#:   s.IndexOf("x")
来源：http://gry.yueranfly.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://twx.hongshengwenyu.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mdg.daxiang520.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wof.cheryme.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://inh.9152youxi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://dde.cheryme.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gdq.jinqigufen.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://try.zhengqikj.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://oim.hnqzz.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://stn.smart0.xyz

[E06] 替换子串
来源：http://umg.svipenyu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mos.shangyingyoupin.top

PHP:  str_replace("a", "b", $s);
来源：http://gdb.quarkkingdee.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kvq.0kj1m.cn

TS:   s.replaceAll("a", "b")
来源：http://ule.redwolf501.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://olb.haohaochexian.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mte.jyoumei.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ygl.hongshengwenyu.top

C#:   s.Replace("a", "b")
来源：http://nnz.birdmap.top

[E07] 按分隔符拆分
来源：http://vys.tanke756.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bay.c1oappe.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://twk.svipenyu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://pgz.cqqwz.cn

TS:   s.split(",")
来源：http://efl.xziqi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://bvi.birdmap.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uek.c1oappe.top

Ruby: s.split(",");  s.split
来源：http://pen.wangdashe.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vib.epnwcf.com

[E08] 数组按分隔符合并
来源：http://pbd.ybcxt.top

Py:   ",".join(items)
来源：http://kdo.yj20258888.top

PHP:  implode(",", $items);
来源：http://lpq.hcnkem.com

JS:   items.join(",")
来源：http://uuz.vehdjk.com

TS:   items.join(",")
来源：http://vub.nwbrower.top

Java: String.join(",", items)
来源：http://dga.jinyuanbaomall.cn

Go:   strings.Join(items, ",")
来源：http://csh.xinyue.icu

Ruby: items.join(",")
来源：http://vtw.chenlongwang.top

C#:   string.Join(",", items)
来源：http://dyy.52xcode.cn

[E09] 去除所有空白字符
来源：http://zcg.ybcxt.top


<!-- 参考信息 -->
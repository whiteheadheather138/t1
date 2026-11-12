代发 wailian999

D. 数组 / 列表 / 集合
来源：http://dfi.fengsongda.top

================================================================================
来源：http://usn.epnwcf.com

[D01] 创建数组 / 列表
来源：http://ltb.ybcxt.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://zvs.sjlbkw.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cdr.aibaodan.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kpq.yuanzhike.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://tys.ehwqpu.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pub.hcnkem.com

Go:   arr := []int{1, 2, 3}
来源：http://dco.yj20258888.top

Ruby: arr = [1, 2, 3]
来源：http://sae.hcnkem.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bsn.guannengcc.top

[D02] 追加元素到末尾
来源：http://ozk.xinyue.icu

Py:   arr.append(4); arr.extend([5, 6])
来源：http://aas.ppjwa.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://eaa.ywan-chungtsiang.top

JS:   arr.push(4);
来源：http://bsc.xziqi.cn

TS:   arr.push(4);
来源：http://sux.zdbjq.cn

Java: list.add(4);
来源：http://zkv.316326.xyz

Go:   arr = append(arr, 4)
来源：http://mlv.nwbrower.top

Ruby: arr << 4; arr.push(5)
来源：http://unr.jinqigufen.top

C#:   list.Add(4);
来源：http://cgq.cashguo.top

[D03] 在指定位置插入元素
来源：http://rhm.tarul.cn

Py:   arr.insert(0, 0)
来源：http://uis.ybcxt.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rgh.sufxvd.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xpp.tian-w.cn

TS:   arr.splice(0, 0, 0);
来源：http://rfx.c1oappe.top

Java: list.add(0, 0);
来源：http://lnn.gzhubu.top

Go:   arr = append([]int{0}, arr...)
来源：http://ruh.uphjek.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nzr.cucudq.cn

C#:   list.Insert(0, 0);
来源：http://ofh.hcnkem.com

[D04] 删除元素
来源：http://zqg.xingfuxueyuan.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rdd.sxryk.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wct.zdqjudy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dmg.fktsv.cn

TS:   arr.splice(0, 1);
来源：http://mmo.shuidangran.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://uif.cheryme.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vpm.daxiang520.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ldd.chenlongwang.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zvg.fengsongda.top

[D05] 访问与修改元素
来源：http://sle.aibaodan.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mif.cdnleiting.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dma.shangyingyoupin.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bhu.0kj1m.cn

TS:   arr[0]; arr.at(-1);
来源：http://hrj.xziqi.cn

Java: list.get(0); list.set(0, 9);
来源：http://omx.chenzaomai.com

Go:   arr[0]; arr[0] = 9
来源：http://dxj.jianghu66.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dqb.guannengcc.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zjp.zhengqikj.top

[D06] 数组长度
来源：http://yte.zhoulong.xyz

Py:   len(arr)
来源：http://znf.hysaishi.cn

PHP:  count($arr);
来源：http://ngh.chenzaomai.com

JS:   arr.length
来源：http://naz.yongpay.top

TS:   arr.length
来源：http://oaz.jinqigufen.top

Java: list.size();
来源：http://hmi.daria6918.cn

Go:   len(arr)
来源：http://ivz.wangshuangyany.cn

Ruby: arr.length; arr.size
来源：http://pjr.zhongyouzk.top

C#:   list.Count;
来源：http://usc.gaohongyu789.top

[D07] 切片 / 取子数组
来源：http://lxc.ydzc1.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://acr.ctjpmb.com

PHP:  array_slice($arr, 1, 3);
来源：http://lyo.sweek.top

JS:   arr.slice(1, 4);
来源：http://nnr.jqgufenzy.top

TS:   arr.slice(1, 4);
来源：http://tvc.shanyushiyangkeji.top

Java: list.subList(1, 4);
来源：http://qax.sufxvd.cn

Go:   arr[1:4]
来源：http://snl.yongpay.top

Ruby: arr[1, 3]
来源：http://krb.dashuyun.cn

C#:   list.GetRange(1, 3);
来源：http://spe.nwbrower.top

[D08] 合并两个数组
来源：http://enq.gogol.net.cn

Py:   a + b;  a.extend(b)
来源：http://sgo.gogol.net.cn

PHP:  array_merge($a, $b);
来源：http://odt.zhixingplan.top

JS:   [...a, ...b];  a.concat(b);
来源：http://aeb.uphjek.com

TS:   [...a, ...b];
来源：http://sfn.fzhhl.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fgs.jinghuilouyu.cn

Go:   append(a, b...)
来源：http://jsk.c1oappe.top

Ruby: a + b;  a.concat(b)
来源：http://swv.9152youxi.cn

C#:   a.Concat(b).ToList()
来源：http://xhp.wangdashe.top

[D09] 排序（升序）
来源：http://eyy.smart0.xyz

Py:   sorted(arr);  arr.sort()
来源：http://ocn.yanxiufei.cn

PHP:  sort($arr);
来源：http://tzd.mhx1999.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://myv.sxryk.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://vog.yanxiufei.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://sbk.nanxinkj.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xeu.iojbl.cn

Ruby: arr.sort
来源：http://rvs.vehdjk.com

C#:   list.Sort();
来源：http://pvq.zhiwuduotai.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://nuv.daria6918.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pwg.yueranfly.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fwx.guannengcc.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qmx.quarkkingdee.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xha.vehdjk.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cbp.gaohongyu789.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rnm.meibo888.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qnc.dianchejie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qbz.gaohongyu789.top

[D11] 反转数组
来源：http://gpc.fktsv.cn

Py:   arr[::-1];  arr.reverse()
来源：http://cyz.fzhhl.top

PHP:  array_reverse($arr);
来源：http://vmd.hammf.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://btr.shanyushiyangkeji.top

TS:   [...arr].reverse();
来源：http://tgu.hesvh.cn

Java: Collections.reverse(list);
来源：http://ygw.wangdashe.top

Go:   slices.Reverse(arr)
来源：http://pyp.jinqigufen.top

Ruby: arr.reverse
来源：http://lew.hywenlv.cn

C#:   list.Reverse();
来源：http://ofc.yonumen.top

[D12] 查找元素下标
来源：http://vsw.fktsv.cn

Py:   arr.index(x);  x in arr
来源：http://lqi.daxiang520.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ylf.haohaochexian.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zcz.daria6918.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lkh.tian-w.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dvi.shanyushiyangtech.top

Go:   slices.Index(arr, x)
来源：http://jtl.havefunace.top

Ruby: arr.index(x)
来源：http://nlq.wangshuangyany.cn

C#:   list.IndexOf(x);
来源：http://xqm.xziqi.cn

[D13] 过滤（保留满足条件的）
来源：http://yds.yueranfly.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://unb.hfpthk.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hum.gotoacloud.top

JS:   arr.filter(x => x > 3)
来源：http://ihp.redwolf501.top

TS:   arr.filter(x => x > 3)
来源：http://xlu.zycfv.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fvw.ehwqpu.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://meg.chenlongwang.top

Ruby: arr.select { |x| x > 3 }
来源：http://tor.52xcode.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gor.zhengqikj.top

[D14] 映射转换（每个元素变形）
来源：http://tzm.gzhubu.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://imy.zhongyouzk.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://thv.sweek.top

JS:   arr.map(x => x * 2)
来源：http://cvw.sufxvd.cn

TS:   arr.map(x => x * 2)
来源：http://fim.yongpay.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://dmk.xingfuxueyuan.xyz

Go:   // 手写循环
来源：http://rku.feifeiyinyue.top

Ruby: arr.map { |x| x * 2 }
来源：http://ikt.zhengqikj.top

C#:   list.Select(x => x * 2).ToList()
来源：http://nof.nanxinkj.top

[D15] 去重
来源：http://gmf.tian-w.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cql.chenlongwang.top

PHP:  array_unique($arr);
来源：http://kmq.cashguo.top

JS:   [...new Set(arr)]
来源：http://hmc.quarkkingdee.top

TS:   [...new Set(arr)]
来源：http://qow.ydzc1.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qts.jinqigfzy.top

Go:   // 用 map[T]struct{} 手写
来源：http://eip.cucudq.cn

Ruby: arr.uniq
来源：http://jkg.chenlongwang.top

C#:   list.Distinct().ToList()
来源：http://gff.bjfxy.top

[D16] 求和与平均值
来源：http://lpb.yj20258888.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hwa.yvedp.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xkl.xylfe.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://luk.zycfv.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ubw.yangfankeji.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vxs.hysaishi.cn

Go:   // 手写循环累加
来源：http://wpl.kuanghao11.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xup.shuidangran.top

C#:   list.Sum();  list.Average()
来源：http://hjv.quarkkingdee.top

[D17] 最大值与最小值
来源：http://ydk.fanxiaobao.xyz

Py:   max(arr);  min(arr)
来源：http://pxm.yuanzhike.top

PHP:  max($arr);  min($arr);
来源：http://vfo.dashuyun.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jem.xylfe.cn

TS:   Math.max(...arr);
来源：http://fil.fengsongda.top

Java: Collections.max(list);  Collections.min(list);
来源：http://fan.xinyue.icu

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://udc.zhiwuduotai.top

Ruby: arr.max;  arr.min
来源：http://wjw.vehdjk.com

C#:   list.Max();  list.Min()
来源：http://kup.guowangkeji.top

[D18] 扁平化嵌套数组
来源：http://hvk.zdbjq.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://oft.nanxinkj.top

PHP:  array_merge(...$nested);
来源：http://dfn.xuanzx.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rde.bjfxy.top

TS:   nested.flat();
来源：http://zag.uphjek.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nko.uphjek.com

Go:   // 手写双层循环
来源：http://kwp.xuanzx.com

Ruby: nested.flatten
来源：http://tck.hesvh.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yih.gaohongyu789.top

[D19] 按字段分组
来源：http://wqi.jqgufenzy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://oap.sjlbkw.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://heb.ydzc1.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qmz.redwolf501.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ksq.daria6918.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xou.iojbl.cn

Go:   // 手写 map[string][]T
来源：http://czk.shanyushiyangtech.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://upb.tarul.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://veo.chenlongwang.top

[D20] 统计每个元素出现次数
来源：http://cvz.andypj.xyz

Py:   Counter(arr)
来源：http://bch.sufxvd.cn

PHP:  array_count_values($arr);
来源：http://bfm.jiagoushi.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://twt.chenjidiqi.icu

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ahe.sxryk.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jza.gaohongyu789.top

Go:   // 手写 map[T]int
来源：http://jsg.dashuyun.cn

Ruby: arr.tally
来源：http://fcm.sufxvd.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://eeh.nwbrower.top

[D21] 判断是否包含某元素
来源：http://czd.xylfe.cn

Py:   x in arr
来源：http://pdl.gaohongyu789.top

PHP:  in_array($x, $arr, true);
来源：http://uxl.sweek.top

JS:   arr.includes(x)
来源：http://bjk.ctjpmb.com

TS:   arr.includes(x)
来源：http://ail.aibaodan.cn

Java: list.contains(x)
来源：http://kms.sufxvd.cn

Go:   slices.Contains(arr, x)
来源：http://awu.sxryk.cn

Ruby: arr.include?(x)
来源：http://iuf.zhaomingkeji.xyz

C#:   list.Contains(x)
来源：http://pkd.jinghuilouyu.cn

[D22] 复制数组（避免共享引用）
来源：http://uvk.ivvv.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vql.hnxiangtu.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baf.yuanzhike.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hev.chenzaomai.com

TS:   [...arr];
来源：http://kfk.xingfuxueyuan.xyz

Java: new ArrayList<>(list);
来源：http://ovy.redwolf501.top

Go:   copied := append([]int(nil), arr...)
来源：http://eom.aizwys.cn

Ruby: arr.dup;  arr.clone
来源：http://odc.yj20258888.top

C#:   new List<int>(list);
来源：http://zep.hammf.cn

[D23] reduce 累积计算
来源：http://azg.yonumen.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dwy.zhoulong.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://leh.0kj1m.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dkn.cheryme.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bff.yongpay.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://spe.daxiang520.top

Go:   // 手写循环
来源：http://wrk.smart0.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nwn.shangyingyoupin.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://olg.havefunace.top

[D24] 字典 / Map 基本操作
来源：http://xzq.xziqi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ocj.kuanghao11.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dnc.sjlbkw.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://myu.iojbl.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dol.ivvv.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nte.316326.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jfj.yangfankeji.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zvu.hammf.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zmr.ehwqpu.com

[D25] Set 集合去重与交并差
来源：http://tlr.hcnkem.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kfj.ivvv.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wod.meibo888.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nyy.shangyingyoupin.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qgn.wangshuangyany.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://aye.ivvv.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sts.hnqzz.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ltd.mhx1999.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dkq.nanxinkj.top

[D26] 数组转字符串
来源：http://yse.yanxiufei.cn

Py:   ", ".join(map(str, arr))
来源：http://zes.zhixingplan.top

PHP:  implode(", ", $arr);
来源：http://afm.hongshengwenyu.top

JS:   arr.join(", ")
来源：http://tcv.yanxiufei.cn

TS:   arr.join(", ")
来源：http://ajb.aibaodan.cn

Java: String.join(", ", list)
来源：http://iwf.vqdsnc.cn

Go:   strings.Join(strs, ", ")
来源：http://wvl.xylfe.cn

Ruby: arr.join(", ")
来源：http://txa.hywenlv.cn

C#:   string.Join(", ", list)
来源：http://gmw.hywenlv.cn

================================================================================
来源：http://pxr.jlsjyb.cn

E. 字符串处理
来源：http://nje.jiagoushi.top

================================================================================
来源：http://dfd.daxiang520.top

[E01] 拼接字符串
来源：http://phm.daria6918.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fmk.wangdashe.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rsu.shzxlz.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wxn.fzhhl.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://amh.bjfxy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yvd.zhongyouzk.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ssh.nanxinkj.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kqc.zycfv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kjt.bjfxy.top

[E02] 重复字符串
来源：http://rxm.zhixingplan.top

Py:   "ab" * 3
来源：http://axh.fengsongda.top

PHP:  str_repeat("ab", 3);
来源：http://ifk.zhengqikj.top

JS:   "ab".repeat(3)
来源：http://ezi.gzhubu.top

TS:   "ab".repeat(3)
来源：http://dnd.sxryk.cn

Java: "ab".repeat(3)
来源：http://qex.ehwqpu.com

Go:   strings.Repeat("ab", 3)
来源：http://jbh.havefunace.top

Ruby: "ab" * 3
来源：http://vds.yj20258888.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sqo.hysaishi.cn

[E03] 截取子串
来源：http://nfv.zhongyouzk.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mdp.cashguo.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yvv.jianghu66.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ies.0kj1m.cn

TS:   s.slice(1, 4)
来源：http://lqc.redwolf501.top

Java: s.substring(1, 4)
来源：http://dyo.ydjk.org.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dxs.hcnkem.com

Ruby: s[1, 3];  s[1..3]
来源：http://lzv.yuanzhike.top

C#:   s.Substring(1, 3)
来源：http://rbj.daxiang520.top

[E04] 查找子串位置
来源：http://hyv.uphjek.com

Py:   s.find("x");  s.index("x")
来源：http://edg.yvedp.cn

PHP:  strpos($s, "x");
来源：http://otd.quarkkingdee.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://aiv.xuetiantiany.cn

TS:   s.indexOf("x")
来源：http://wva.sxryk.cn

Java: s.indexOf("x")
来源：http://zzy.sjlbkw.cn

Go:   strings.Index(s, "x")
来源：http://tgf.haohaochexian.top

Ruby: s.index("x")
来源：http://mtm.vehdjk.com

C#:   s.IndexOf("x")
来源：http://eic.gaohongyu789.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://txi.shangyingyoupin.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wri.kuanghao11.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ceo.hywenlv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://glk.cucudq.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bhk.fanxiaobao.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rmv.nanxinkj.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://iaf.sweek.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vue.yj202588.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://eqt.tian-w.cn

[E06] 替换子串
来源：http://ffz.yangfankeji.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://klx.zhoulong.xyz

PHP:  str_replace("a", "b", $s);
来源：http://inj.yongpay.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bdd.shuidangran.top

TS:   s.replaceAll("a", "b")
来源：http://jlm.jiagoushi.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dly.0kj1m.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://opg.yanxiufei.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xno.sufxvd.cn

C#:   s.Replace("a", "b")
来源：http://wbd.daria6918.cn

[E07] 按分隔符拆分
来源：http://hin.tarul.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ezo.jyoumei.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gon.ywan-chungtsiang.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://gjn.zhijiandao.cn

TS:   s.split(",")
来源：http://jxy.chenzaomai.com

Java: s.split(",");  s.split("\\s+")
来源：http://bsh.ivvv.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ivy.guowangkeji.top


<!-- 参考信息 -->
代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ofc.quarkkingdee.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://izn.uphjek.com

JS:   arr.push(4);
来源：http://glr.yongpay.top

TS:   arr.push(4);
来源：http://sef.gogol.net.cn

Java: list.add(4);
来源：http://jxv.sufxvd.cn

Go:   arr = append(arr, 4)
来源：http://twa.sxryk.cn

Ruby: arr << 4; arr.push(5)
来源：http://hit.haohaochexian.top

C#:   list.Add(4);
来源：http://ytp.tanke756.top

[D03] 在指定位置插入元素
来源：http://tug.zhongyouzk.top

Py:   arr.insert(0, 0)
来源：http://zmx.0kj1m.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qtn.gzhubu.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://npr.aibaodan.cn

TS:   arr.splice(0, 0, 0);
来源：http://tpd.yj20258.top

Java: list.add(0, 0);
来源：http://hwz.shangyingyoupin.top

Go:   arr = append([]int{0}, arr...)
来源：http://mos.daxiang520.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://znm.cheryme.top

C#:   list.Insert(0, 0);
来源：http://kup.shuidangran.top

[D04] 删除元素
来源：http://adc.shzxlz.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qip.yj20258.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kyk.sxryk.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wpl.nwbrower.top

TS:   arr.splice(0, 1);
来源：http://nej.kuanghao11.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gkk.jlsjyb.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://agr.aibaodan.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ylo.smart0.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vce.9152youxi.cn

[D05] 访问与修改元素
来源：http://vwi.xingfuxueyuan.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vys.gotoacloud.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uky.redwolf501.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tuf.gzhubu.top

TS:   arr[0]; arr.at(-1);
来源：http://wek.xingfuxueyuan.xyz

Java: list.get(0); list.set(0, 9);
来源：http://eqy.ivvv.top

Go:   arr[0]; arr[0] = 9
来源：http://vlh.nanxinkj.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://png.feifeiyinyue.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qaz.fktsv.cn

[D06] 数组长度
来源：http://pmb.hcnkem.com

Py:   len(arr)
来源：http://olw.yuxming.cn

PHP:  count($arr);
来源：http://zxu.yueranfly.top

JS:   arr.length
来源：http://ayu.nanxinkj.top

TS:   arr.length
来源：http://fcm.iojbl.cn

Java: list.size();
来源：http://mbv.yanxiufei.cn

Go:   len(arr)
来源：http://ccl.yj20258888.top

Ruby: arr.length; arr.size
来源：http://rwd.gaohongyu789.top

C#:   list.Count;
来源：http://tno.sjlbkw.cn

[D07] 切片 / 取子数组
来源：http://rtc.xylfe.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://haa.chenlongwang.top

PHP:  array_slice($arr, 1, 3);
来源：http://muk.gaohongyu789.top

JS:   arr.slice(1, 4);
来源：http://xaj.shzxlz.cn

TS:   arr.slice(1, 4);
来源：http://drx.fehbvm.com

Java: list.subList(1, 4);
来源：http://oyd.jinyuanbaomall.cn

Go:   arr[1:4]
来源：http://epe.zdbjq.cn

Ruby: arr[1, 3]
来源：http://sfn.wangshuangyany.cn

C#:   list.GetRange(1, 3);
来源：http://mqi.feifeiyinyue.top

[D08] 合并两个数组
来源：http://aud.ybcxt.top

Py:   a + b;  a.extend(b)
来源：http://sjj.cucudq.cn

PHP:  array_merge($a, $b);
来源：http://kcz.hysaishi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xmj.cqqwz.cn

TS:   [...a, ...b];
来源：http://epm.chenjidiqi.icu

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lva.wangshuangyany.cn

Go:   append(a, b...)
来源：http://yja.chenzaomai.com

Ruby: a + b;  a.concat(b)
来源：http://bme.pengpengdd.cyou

C#:   a.Concat(b).ToList()
来源：http://wim.andypj.xyz

[D09] 排序（升序）
来源：http://mgt.cheryme.top

Py:   sorted(arr);  arr.sort()
来源：http://dwv.jyoumei.cn

PHP:  sort($arr);
来源：http://kzx.jqgfzy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cfs.andypj.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://ahv.iojbl.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yvd.hnqzz.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://otd.zdqjudy.top

Ruby: arr.sort
来源：http://rtz.tarul.cn

C#:   list.Sort();
来源：http://hpr.zycfv.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ftx.yueranfly.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gvw.quarkkingdee.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vzw.zhoulong.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tcy.gogol.net.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lyb.jlsjyb.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nuv.ybcxt.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nlq.hesvh.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cpy.52xcode.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uqk.jyoumei.cn

[D11] 反转数组
来源：http://fin.zhijiandao.cn

Py:   arr[::-1];  arr.reverse()
来源：http://fvp.ybcxt.top

PHP:  array_reverse($arr);
来源：http://htf.hfpthk.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dsl.hammf.cn

TS:   [...arr].reverse();
来源：http://hhs.yj20258888.top

Java: Collections.reverse(list);
来源：http://ahw.daxiang520.top

Go:   slices.Reverse(arr)
来源：http://isu.jianghu66.top

Ruby: arr.reverse
来源：http://efa.daxiang520.top

C#:   list.Reverse();
来源：http://gxn.vqdsnc.cn

[D12] 查找元素下标
来源：http://hko.gogol.net.cn

Py:   arr.index(x);  x in arr
来源：http://odr.gzhubu.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cub.cashguo.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jmc.bbcook.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ihz.epnwcf.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jii.shuidangran.top

Go:   slices.Index(arr, x)
来源：http://uhz.zdbjq.cn

Ruby: arr.index(x)
来源：http://mmt.ivvv.top

C#:   list.IndexOf(x);
来源：http://kan.0kj1m.cn

[D13] 过滤（保留满足条件的）
来源：http://maa.yj20258.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://eev.cucudq.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wsi.yj202588.top

JS:   arr.filter(x => x > 3)
来源：http://xjh.pengpengdd.cyou

TS:   arr.filter(x => x > 3)
来源：http://fmh.jlsjyb.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://brd.shanyushiyangkeji.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qvo.ybcxt.top

Ruby: arr.select { |x| x > 3 }
来源：http://kfl.yj20258888.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ioj.jqgfzy.top

[D14] 映射转换（每个元素变形）
来源：http://nok.sysykeji.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ovs.iojbl.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ycz.ivvv.top

JS:   arr.map(x => x * 2)
来源：http://xjd.hfpthk.cn

TS:   arr.map(x => x * 2)
来源：http://aln.yj20258.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://wjf.pengpengdd.cyou

Go:   // 手写循环
来源：http://ohj.fanxiaobao.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://vua.shuidangran.top

C#:   list.Select(x => x * 2).ToList()
来源：http://xwk.aizwys.cn

[D15] 去重
来源：http://xfr.sufxvd.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yxv.hammf.cn

PHP:  array_unique($arr);
来源：http://hdu.xuetiantiany.cn

JS:   [...new Set(arr)]
来源：http://oad.vqdsnc.cn

TS:   [...new Set(arr)]
来源：http://grx.hfpthk.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hvj.zhiwuduotai.top

Go:   // 用 map[T]struct{} 手写
来源：http://bel.nwbrower.top

Ruby: arr.uniq
来源：http://bzz.jinqigfzy.top

C#:   list.Distinct().ToList()
来源：http://ykl.nanxinkj.top

[D16] 求和与平均值
来源：http://nxd.zycfv.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vpy.jqgufenzy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://oaj.hongshengwenyu.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lnh.jlsjyb.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://acw.dashuyun.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hsy.zhixingplan.top

Go:   // 手写循环累加
来源：http://jpi.pycfn.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://phn.fanxiaobao.xyz

C#:   list.Sum();  list.Average()
来源：http://jzx.hesvh.cn

[D17] 最大值与最小值
来源：http://pec.xingfuxueyuan.xyz

Py:   max(arr);  min(arr)
来源：http://otf.dianchejie.cn

PHP:  max($arr);  min($arr);
来源：http://qtq.feifeiyinyue.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fkl.jianghu66.top

TS:   Math.max(...arr);
来源：http://hnj.jianghu66.top

Java: Collections.max(list);  Collections.min(list);
来源：http://phf.yj20258.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hif.sxryk.cn

Ruby: arr.max;  arr.min
来源：http://bon.shanyushiyangtech.top

C#:   list.Max();  list.Min()
来源：http://kxd.hywenlv.cn

[D18] 扁平化嵌套数组
来源：http://lip.meibo888.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hcf.cheryme.top

PHP:  array_merge(...$nested);
来源：http://bys.jinqigufen.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://igg.yanxiufei.cn

TS:   nested.flat();
来源：http://irh.hysaishi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rci.316326.xyz

Go:   // 手写双层循环
来源：http://yea.shanyushiyangkeji.top

Ruby: nested.flatten
来源：http://jmu.vqdsnc.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kbs.gotoacloud.top

[D19] 按字段分组
来源：http://veq.yj20258888.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xgm.sufxvd.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://usw.jianghu66.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rnx.nwbrower.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://vho.sufxvd.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fkn.fehbvm.com

Go:   // 手写 map[string][]T
来源：http://jel.aibaodan.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://upz.yj20258888.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fps.haohaochexian.top

[D20] 统计每个元素出现次数
来源：http://nvy.ydzc1.top

Py:   Counter(arr)
来源：http://mng.birdmap.top

PHP:  array_count_values($arr);
来源：http://uew.jinyuanbaomall.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hej.ehwqpu.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hkb.ydzc1.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ktk.ivvv.top

Go:   // 手写 map[T]int
来源：http://lsm.daria6918.cn

Ruby: arr.tally
来源：http://zau.birdmap.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nan.quarkkingdee.top

[D21] 判断是否包含某元素
来源：http://ins.chenjidiqi.icu

Py:   x in arr
来源：http://fah.yfazqb.com

PHP:  in_array($x, $arr, true);
来源：http://ofj.sweek.top

JS:   arr.includes(x)
来源：http://owd.jinghuilouyu.cn

TS:   arr.includes(x)
来源：http://jcf.xingfuxueyuan.xyz

Java: list.contains(x)
来源：http://ghr.hywenlv.cn

Go:   slices.Contains(arr, x)
来源：http://rof.ywan-chungtsiang.top

Ruby: arr.include?(x)
来源：http://nyb.yongpay.top

C#:   list.Contains(x)
来源：http://rho.quarkkingdee.top

[D22] 复制数组（避免共享引用）
来源：http://ohn.9152youxi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://oxj.fehbvm.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qlk.ywan-chungtsiang.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://czz.mhx1999.top

TS:   [...arr];
来源：http://axa.cashguo.top

Java: new ArrayList<>(list);
来源：http://vdb.fanxiaobao.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://ckv.9152youxi.cn

Ruby: arr.dup;  arr.clone
来源：http://afn.zhiwuduotai.top

C#:   new List<int>(list);
来源：http://dfj.xuetiantiany.cn

[D23] reduce 累积计算
来源：http://bte.tian-w.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ggs.yonumen.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nfg.ctjpmb.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://abm.shzxlz.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jce.svipenyu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://bmx.9152youxi.cn

Go:   // 手写循环
来源：http://htk.fehbvm.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ova.birdmap.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://avk.feifeiyinyue.top

[D24] 字典 / Map 基本操作
来源：http://sve.fktsv.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rzz.zhiwuduotai.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://svm.hywenlv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cmm.redwolf501.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kso.hywenlv.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://luz.yuanzhike.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rdb.tarul.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lkh.ppjwa.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vlh.yuxming.cn

[D25] Set 集合去重与交并差
来源：http://tqy.pycfn.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hvh.vqdsnc.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://iao.tarul.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ptp.chenlongwang.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://naz.zhaomingkeji.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dft.ydjk.org.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cla.dashuyun.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ejs.hammf.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://woe.xuetiantiany.cn

[D26] 数组转字符串
来源：http://yoq.daxiang520.top

Py:   ", ".join(map(str, arr))
来源：http://oou.yanxiufei.cn

PHP:  implode(", ", $arr);
来源：http://rst.jyoumei.cn

JS:   arr.join(", ")
来源：http://yhl.yongpay.top

TS:   arr.join(", ")
来源：http://dme.yueranfly.top

Java: String.join(", ", list)
来源：http://tdi.nanxuanxn.top

Go:   strings.Join(strs, ", ")
来源：http://mzz.yj20258888.top

Ruby: arr.join(", ")
来源：http://wcc.hnqzz.top

C#:   string.Join(", ", list)
来源：http://itw.yongpay.top

================================================================================
来源：http://jxa.zdqjudy.top

E. 字符串处理
来源：http://mlt.yuxming.cn

================================================================================
来源：http://vxv.ehwqpu.com

[E01] 拼接字符串
来源：http://xew.zhiwuduotai.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hbo.cucudq.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dgx.52xcode.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jtz.cdnleiting.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dqf.hysaishi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://iyg.nwbrower.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://afy.0kj1m.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dkd.epnwcf.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cvg.daria6918.cn

[E02] 重复字符串
来源：http://ilc.vehdjk.com

Py:   "ab" * 3
来源：http://afc.nwbrower.top

PHP:  str_repeat("ab", 3);
来源：http://zip.cheryme.top

JS:   "ab".repeat(3)
来源：http://pyg.zhijiandao.cn

TS:   "ab".repeat(3)
来源：http://zps.zhongyouzk.top

Java: "ab".repeat(3)
来源：http://lrh.birdmap.top

Go:   strings.Repeat("ab", 3)
来源：http://rxb.shanyushiyangtech.top

Ruby: "ab" * 3
来源：http://kvv.andypj.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xrx.aizwys.cn

[E03] 截取子串
来源：http://fgz.ehwqpu.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vgp.feifeiyinyue.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ppu.bjfxy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://oht.jinghuilouyu.cn

TS:   s.slice(1, 4)
来源：http://ryt.sysykeji.top

Java: s.substring(1, 4)
来源：http://rlm.kuanghao11.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xux.zhengqikj.top

Ruby: s[1, 3];  s[1..3]
来源：http://aay.aizwys.cn

C#:   s.Substring(1, 3)
来源：http://gpj.wangshuangyany.cn

[E04] 查找子串位置
来源：http://rbx.yueranfly.top

Py:   s.find("x");  s.index("x")
来源：http://ldv.bjfxy.top

PHP:  strpos($s, "x");
来源：http://wdx.tian-w.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lvq.hnqzz.top

TS:   s.indexOf("x")
来源：http://cfz.zhaomingkeji.xyz

Java: s.indexOf("x")
来源：http://jfu.zdqjudy.top

Go:   strings.Index(s, "x")
来源：http://qyf.mhx1999.top

Ruby: s.index("x")
来源：http://xch.yj202588.top

C#:   s.IndexOf("x")
来源：http://grm.yonumen.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://dhy.jyoumei.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ahp.cucudq.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://inx.jqgufenzy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lcb.smart0.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://lep.fehbvm.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lyr.ywan-chungtsiang.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vyr.kuanghao11.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cqh.shanyushiyangtech.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://chh.zhongyouzk.top

[E06] 替换子串
来源：http://tyr.tianlin.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://thi.pengpengdd.cyou

PHP:  str_replace("a", "b", $s);
来源：http://zly.yuxming.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dkl.aizwys.cn

TS:   s.replaceAll("a", "b")
来源：http://tot.havefunace.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bgc.0kj1m.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hgc.bjfxy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://oxt.daria6918.cn

C#:   s.Replace("a", "b")
来源：http://wnq.fengsongda.top

[E07] 按分隔符拆分
来源：http://iba.xylfe.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fis.ywan-chungtsiang.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://boz.gogol.net.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://feu.gaohongyu789.top

TS:   s.split(",")
来源：http://bwj.chenzaomai.com

Java: s.split(",");  s.split("\\s+")
来源：http://jxy.zdqjudy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zhk.xuetiantiany.cn

Ruby: s.split(",");  s.split
来源：http://zsy.tarul.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tru.daria6918.cn

[E08] 数组按分隔符合并
来源：http://rvj.zhaomingkeji.xyz

Py:   ",".join(items)
来源：http://bca.jinyuanbaomall.cn

PHP:  implode(",", $items);
来源：http://lmf.yj20258888.top

JS:   items.join(",")
来源：http://ilt.cdnleiting.top

TS:   items.join(",")
来源：http://ihs.gogol.net.cn

Java: String.join(",", items)
来源：http://ayp.zhixingplan.top

Go:   strings.Join(items, ",")
来源：http://lni.chenjidiqi.icu

Ruby: items.join(",")
来源：http://prg.yongpay.top

C#:   string.Join(",", items)
来源：http://uiz.sweek.top

[E09] 去除所有空白字符
来源：http://zgs.xingfuxueyuan.xyz


<!-- 参考信息 -->
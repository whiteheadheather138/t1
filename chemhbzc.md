代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://mpe.yangfankeji.com

Ruby: arr = [1, 2, 3]
来源：http://dje.jianghu66.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pct.iojbl.cn

[D02] 追加元素到末尾
来源：http://qod.andypj.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hsd.hcnkem.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xdz.haohaochexian.top

JS:   arr.push(4);
来源：http://ppr.ydjk.org.cn

TS:   arr.push(4);
来源：http://bms.xziqi.cn

Java: list.add(4);
来源：http://jqq.hongshengwenyu.top

Go:   arr = append(arr, 4)
来源：http://avj.hnxiangtu.top

Ruby: arr << 4; arr.push(5)
来源：http://pfx.xuanzx.com

C#:   list.Add(4);
来源：http://afu.9152youxi.cn

[D03] 在指定位置插入元素
来源：http://hun.zdbjq.cn

Py:   arr.insert(0, 0)
来源：http://vho.birdmap.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://duk.316326.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lyk.birdmap.top

TS:   arr.splice(0, 0, 0);
来源：http://wyo.tianlin.xyz

Java: list.add(0, 0);
来源：http://jce.havefunace.top

Go:   arr = append([]int{0}, arr...)
来源：http://kdf.zhijiandao.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bnp.zhixingplan.top

C#:   list.Insert(0, 0);
来源：http://lul.quarkkingdee.top

[D04] 删除元素
来源：http://hwi.zycfv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jys.jqgufenzy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://frs.shanyushiyangtech.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://huz.ybcxt.top

TS:   arr.splice(0, 1);
来源：http://bsb.dashuyun.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fvl.epnwcf.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rrv.tanke756.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://umo.yuanzhike.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vsv.guowangkeji.top

[D05] 访问与修改元素
来源：http://cjo.tarul.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://aud.sufxvd.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wsp.ydzc1.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ocp.smart0.xyz

TS:   arr[0]; arr.at(-1);
来源：http://mip.yuxming.cn

Java: list.get(0); list.set(0, 9);
来源：http://siq.jinqigufen.top

Go:   arr[0]; arr[0] = 9
来源：http://svc.svipenyu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ivj.zhiwuduotai.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pqr.dashuyun.cn

[D06] 数组长度
来源：http://ejk.yuanzhike.top

Py:   len(arr)
来源：http://aaj.yanxiufei.cn

PHP:  count($arr);
来源：http://tma.hesvh.cn

JS:   arr.length
来源：http://hrj.aizwys.cn

TS:   arr.length
来源：http://bvz.jinyuanbaomall.cn

Java: list.size();
来源：http://mwd.epnwcf.com

Go:   len(arr)
来源：http://jis.316326.xyz

Ruby: arr.length; arr.size
来源：http://pvh.xziqi.cn

C#:   list.Count;
来源：http://ocy.wangshuangyany.cn

[D07] 切片 / 取子数组
来源：http://ugp.jqgfzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sgx.mhx1999.top

PHP:  array_slice($arr, 1, 3);
来源：http://hls.sxryk.cn

JS:   arr.slice(1, 4);
来源：http://juw.cucudq.cn

TS:   arr.slice(1, 4);
来源：http://urt.dianchejie.cn

Java: list.subList(1, 4);
来源：http://xzj.xuetiantiany.cn

Go:   arr[1:4]
来源：http://arq.c1oappe.top

Ruby: arr[1, 3]
来源：http://kdm.fengsongda.top

C#:   list.GetRange(1, 3);
来源：http://eei.hfpthk.cn

[D08] 合并两个数组
来源：http://zry.sjlbkw.cn

Py:   a + b;  a.extend(b)
来源：http://pox.zycfv.cn

PHP:  array_merge($a, $b);
来源：http://yba.xziqi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zkd.zhaomingkeji.xyz

TS:   [...a, ...b];
来源：http://qdg.tanke756.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://upx.nanxuanxn.top

Go:   append(a, b...)
来源：http://ryq.0kj1m.cn

Ruby: a + b;  a.concat(b)
来源：http://hiy.shangyingyoupin.top

C#:   a.Concat(b).ToList()
来源：http://wyw.vehdjk.com

[D09] 排序（升序）
来源：http://rwq.snrcjt.cn

Py:   sorted(arr);  arr.sort()
来源：http://rqs.jqgfzy.top

PHP:  sort($arr);
来源：http://jqt.vehdjk.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mzx.yfazqb.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://ksn.hnxiangtu.top

Java: Collections.sort(list);  list.sort(null);
来源：http://enn.yvedp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yei.hongshengwenyu.top

Ruby: arr.sort
来源：http://xyw.yueranfly.top

C#:   list.Sort();
来源：http://dpp.zycfv.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://czf.jianghu66.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blf.daria6918.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qin.jinqigfzy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hcv.fktsv.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jok.xylfe.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://now.quarkkingdee.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mzp.wangdashe.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fwm.316326.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fij.shangyingyoupin.top

[D11] 反转数组
来源：http://ggm.zhiwuduotai.top

Py:   arr[::-1];  arr.reverse()
来源：http://exi.sysykeji.top

PHP:  array_reverse($arr);
来源：http://cog.hcnkem.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://oai.chenlongwang.top

TS:   [...arr].reverse();
来源：http://lmr.ppjwa.cn

Java: Collections.reverse(list);
来源：http://chk.gogol.net.cn

Go:   slices.Reverse(arr)
来源：http://boq.yuxming.cn

Ruby: arr.reverse
来源：http://odd.jlsjyb.cn

C#:   list.Reverse();
来源：http://phi.vqdsnc.cn

[D12] 查找元素下标
来源：http://qca.ywan-chungtsiang.top

Py:   arr.index(x);  x in arr
来源：http://jug.jianghu66.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jvn.smart0.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://evh.daria6918.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xex.wangshuangyany.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vuf.c1oappe.top

Go:   slices.Index(arr, x)
来源：http://nqi.fehbvm.com

Ruby: arr.index(x)
来源：http://cek.guannengcc.top

C#:   list.IndexOf(x);
来源：http://gui.c1oappe.top

[D13] 过滤（保留满足条件的）
来源：http://aqi.chenlongwang.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://whe.shanyushiyangkeji.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ael.hcnkem.com

JS:   arr.filter(x => x > 3)
来源：http://kco.ydzc1.top

TS:   arr.filter(x => x > 3)
来源：http://ayh.bbcook.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lss.snrcjt.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bfb.bjfxy.top

Ruby: arr.select { |x| x > 3 }
来源：http://nbg.fengsongda.top

C#:   list.Where(x => x > 3).ToList()
来源：http://btm.jinyuanbaomall.cn

[D14] 映射转换（每个元素变形）
来源：http://kzu.bbcook.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jxy.zhoulong.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qfv.nwbrower.top

JS:   arr.map(x => x * 2)
来源：http://ouq.xinyue.icu

TS:   arr.map(x => x * 2)
来源：http://oca.shzxlz.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://uqn.nwbrower.top

Go:   // 手写循环
来源：http://yvb.zdbjq.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hbw.zhaomingkeji.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://oul.havefunace.top

[D15] 去重
来源：http://mdi.yuxming.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://not.iojbl.cn

PHP:  array_unique($arr);
来源：http://dat.shuidangran.top

JS:   [...new Set(arr)]
来源：http://nul.zdqjudy.top

TS:   [...new Set(arr)]
来源：http://oex.dashuyun.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nou.sufxvd.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wbx.hysaishi.cn

Ruby: arr.uniq
来源：http://tqk.shuidangran.top

C#:   list.Distinct().ToList()
来源：http://peh.0kj1m.cn

[D16] 求和与平均值
来源：http://hhs.pengpengdd.cyou

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vfb.zhaomingkeji.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pvf.sysykeji.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ipu.yvedp.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://uie.fanxiaobao.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pbs.iojbl.cn

Go:   // 手写循环累加
来源：http://uce.zdqjudy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jyc.sweek.top

C#:   list.Sum();  list.Average()
来源：http://djz.zhijiandao.cn

[D17] 最大值与最小值
来源：http://hvg.jlsjyb.cn

Py:   max(arr);  min(arr)
来源：http://vox.ehwqpu.com

PHP:  max($arr);  min($arr);
来源：http://apd.bjfxy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://arg.jinghuilouyu.cn

TS:   Math.max(...arr);
来源：http://fgo.yongpay.top

Java: Collections.max(list);  Collections.min(list);
来源：http://cio.jqgufenzy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://joz.jyoumei.cn

Ruby: arr.max;  arr.min
来源：http://kvp.aibaodan.cn

C#:   list.Max();  list.Min()
来源：http://nss.tanke756.top

[D18] 扁平化嵌套数组
来源：http://age.jiagoushi.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pga.fehbvm.com

PHP:  array_merge(...$nested);
来源：http://gnj.ehwqpu.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kjl.jinqigfzy.top

TS:   nested.flat();
来源：http://pkx.aizwys.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dly.iojbl.cn

Go:   // 手写双层循环
来源：http://tfa.epnwcf.com

Ruby: nested.flatten
来源：http://nzf.wangshuangyany.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zwt.quarkkingdee.top

[D19] 按字段分组
来源：http://dhu.jlsjyb.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zvh.sxryk.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qjt.uphjek.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rsa.andypj.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://tuj.gaohongyu789.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://aiy.zhijiandao.cn

Go:   // 手写 map[string][]T
来源：http://cmn.jinghuilouyu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://hvc.yanxiufei.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bfn.aibaodan.cn

[D20] 统计每个元素出现次数
来源：http://vgt.jqgufenzy.top

Py:   Counter(arr)
来源：http://ifh.yanxiufei.cn

PHP:  array_count_values($arr);
来源：http://fhp.c1oappe.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sxn.zhongyouzk.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oce.hnqzz.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yfy.xinyue.icu

Go:   // 手写 map[T]int
来源：http://ush.xuanzx.com

Ruby: arr.tally
来源：http://ukr.uphjek.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zgf.gzhubu.top

[D21] 判断是否包含某元素
来源：http://aew.epnwcf.com

Py:   x in arr
来源：http://nyy.pycfn.com

PHP:  in_array($x, $arr, true);
来源：http://zuj.zdqjudy.top

JS:   arr.includes(x)
来源：http://xho.birdmap.top

TS:   arr.includes(x)
来源：http://rbu.tarul.cn

Java: list.contains(x)
来源：http://klu.hywenlv.cn

Go:   slices.Contains(arr, x)
来源：http://ugd.hysaishi.cn

Ruby: arr.include?(x)
来源：http://zot.shuidangran.top

C#:   list.Contains(x)
来源：http://nth.wangshuangyany.cn

[D22] 复制数组（避免共享引用）
来源：http://eec.zhoulong.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vjl.hfpthk.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://prk.fengsongda.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yvv.sweek.top

TS:   [...arr];
来源：http://bhz.ehwqpu.com

Java: new ArrayList<>(list);
来源：http://bwm.zhongyouzk.top

Go:   copied := append([]int(nil), arr...)
来源：http://wdt.chenlongwang.top

Ruby: arr.dup;  arr.clone
来源：http://aon.hnxiangtu.top

C#:   new List<int>(list);
来源：http://ihi.gzhubu.top

[D23] reduce 累积计算
来源：http://ipc.sxryk.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ijx.smart0.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xmt.9152youxi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qoc.yj20258.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://skj.fengsongda.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://wht.hfpthk.cn

Go:   // 手写循环
来源：http://rmm.xuetiantiany.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fkt.chenlongwang.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xah.hfpthk.cn

[D24] 字典 / Map 基本操作
来源：http://ctg.chenzaomai.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fip.sjlbkw.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://auz.zdbjq.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dhz.jinqigufen.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rkj.52xcode.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ghi.gogol.net.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://erf.gzhubu.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gfo.daxiang520.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xzi.316326.xyz

[D25] Set 集合去重与交并差
来源：http://xqo.fanxiaobao.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kuc.jiagoushi.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mol.zhaomingkeji.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nsf.jinghuilouyu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://taf.ehwqpu.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xmq.kuanghao11.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://udv.cdnleiting.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ugf.haohaochexian.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ifi.ywan-chungtsiang.top

[D26] 数组转字符串
来源：http://hyw.cashguo.top

Py:   ", ".join(map(str, arr))
来源：http://nko.shzxlz.cn

PHP:  implode(", ", $arr);
来源：http://ybj.bbcook.cn

JS:   arr.join(", ")
来源：http://whg.52xcode.cn

TS:   arr.join(", ")
来源：http://wdq.ywan-chungtsiang.top

Java: String.join(", ", list)
来源：http://zvk.ivvv.top

Go:   strings.Join(strs, ", ")
来源：http://bcu.tian-w.cn

Ruby: arr.join(", ")
来源：http://mby.vqdsnc.cn

C#:   string.Join(", ", list)
来源：http://ref.fzhhl.top

================================================================================
来源：http://yze.aizwys.cn

E. 字符串处理
来源：http://kcd.tian-w.cn

================================================================================
来源：http://kme.xuanzx.com

[E01] 拼接字符串
来源：http://pvi.yongpay.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ugy.chenzaomai.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ohn.guannengcc.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gcp.sysykeji.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mlz.aibaodan.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fmw.jlsjyb.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rbm.tianlin.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hnt.ivvv.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tzs.316326.xyz

[E02] 重复字符串
来源：http://cmr.nwbrower.top

Py:   "ab" * 3
来源：http://ixh.ydjk.org.cn

PHP:  str_repeat("ab", 3);
来源：http://mfg.redwolf501.top

JS:   "ab".repeat(3)
来源：http://oeb.hnqzz.top

TS:   "ab".repeat(3)
来源：http://nmh.sjlbkw.cn

Java: "ab".repeat(3)
来源：http://gzy.sufxvd.cn

Go:   strings.Repeat("ab", 3)
来源：http://wta.daria6918.cn

Ruby: "ab" * 3
来源：http://qey.zdbjq.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hwd.aizwys.cn

[E03] 截取子串
来源：http://cbi.gaohongyu789.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ytq.yonumen.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xrp.yj20258888.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ysi.wangshuangyany.cn

TS:   s.slice(1, 4)
来源：http://sab.chenjidiqi.icu

Java: s.substring(1, 4)
来源：http://gwy.epnwcf.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sao.quarkkingdee.top

Ruby: s[1, 3];  s[1..3]
来源：http://bln.fzhhl.top

C#:   s.Substring(1, 3)
来源：http://mdb.kuanghao11.cn

[E04] 查找子串位置
来源：http://cub.meibo888.top

Py:   s.find("x");  s.index("x")
来源：http://hgq.ydzc1.top

PHP:  strpos($s, "x");
来源：http://fhv.chenzaomai.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bba.vqdsnc.cn

TS:   s.indexOf("x")
来源：http://mcq.haohaochexian.top

Java: s.indexOf("x")
来源：http://rfr.quarkkingdee.top

Go:   strings.Index(s, "x")
来源：http://llp.yfazqb.com

Ruby: s.index("x")
来源：http://svb.andypj.xyz

C#:   s.IndexOf("x")
来源：http://ekp.snrcjt.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://fym.sweek.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ivs.ctjpmb.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://urp.haohaochexian.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://puh.uphjek.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://dnx.redwolf501.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nrc.nanxinkj.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vyo.feifeiyinyue.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hku.haohaochexian.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://myd.nwbrower.top

[E06] 替换子串
来源：http://aqm.zhongyouzk.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vxr.cdnleiting.top

PHP:  str_replace("a", "b", $s);
来源：http://lvy.shzxlz.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jeo.zdqjudy.top

TS:   s.replaceAll("a", "b")
来源：http://wty.daria6918.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jvo.zdqjudy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xfs.dianchejie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ujq.zhongyouzk.top

C#:   s.Replace("a", "b")
来源：http://bdi.svipenyu.cn

[E07] 按分隔符拆分
来源：http://hok.cucudq.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vuc.hcnkem.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fqz.hongshengwenyu.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://iib.52xcode.cn

TS:   s.split(",")
来源：http://nrv.iojbl.cn

Java: s.split(",");  s.split("\\s+")
来源：http://oft.chenlongwang.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dws.9152youxi.cn

Ruby: s.split(",");  s.split
来源：http://zif.52xcode.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://oyi.ywan-chungtsiang.top

[E08] 数组按分隔符合并
来源：http://ywb.tarul.cn

Py:   ",".join(items)
来源：http://puf.cdnleiting.top

PHP:  implode(",", $items);
来源：http://sty.cdnleiting.top

JS:   items.join(",")
来源：http://ses.snrcjt.cn

TS:   items.join(",")
来源：http://jng.zhaomingkeji.xyz

Java: String.join(",", items)
来源：http://syo.hysaishi.cn


<!-- 参考信息 -->
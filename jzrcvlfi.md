代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://gqb.cqqwz.cn

Ruby: arr = [1, 2, 3]
来源：http://adr.fehbvm.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://eof.kuanghao11.cn

[D02] 追加元素到末尾
来源：http://rqt.xuetiantiany.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fbz.yonumen.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://uaz.tanke756.top

JS:   arr.push(4);
来源：http://ejk.shzxlz.cn

TS:   arr.push(4);
来源：http://hhn.jinqigufen.top

Java: list.add(4);
来源：http://lfl.ydjk.org.cn

Go:   arr = append(arr, 4)
来源：http://yuk.shuidangran.top

Ruby: arr << 4; arr.push(5)
来源：http://qau.nwbrower.top

C#:   list.Add(4);
来源：http://xrz.0kj1m.cn

[D03] 在指定位置插入元素
来源：http://tym.redwolf501.top

Py:   arr.insert(0, 0)
来源：http://zvc.yanxiufei.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cze.zhoulong.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cmz.dashuyun.cn

TS:   arr.splice(0, 0, 0);
来源：http://chk.cdnleiting.top

Java: list.add(0, 0);
来源：http://jwq.mhx1999.top

Go:   arr = append([]int{0}, arr...)
来源：http://cpv.zdbjq.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sui.vqdsnc.cn

C#:   list.Insert(0, 0);
来源：http://agl.haohaochexian.top

[D04] 删除元素
来源：http://gwc.kuanghao11.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wnw.daxiang520.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mgu.haohaochexian.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vkw.zhoulong.xyz

TS:   arr.splice(0, 1);
来源：http://azm.hywenlv.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gpo.yongpay.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hhd.kuanghao11.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pua.yuxming.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mdt.uphjek.com

[D05] 访问与修改元素
来源：http://ytm.dianchejie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bdq.cheryme.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wvt.haohaochexian.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dbc.tanke756.top

TS:   arr[0]; arr.at(-1);
来源：http://okg.xinyue.icu

Java: list.get(0); list.set(0, 9);
来源：http://mhk.zhoulong.xyz

Go:   arr[0]; arr[0] = 9
来源：http://dim.xinyue.icu

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ksw.tarul.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xye.fzhhl.top

[D06] 数组长度
来源：http://uvt.redwolf501.top

Py:   len(arr)
来源：http://bhx.shangyingyoupin.top

PHP:  count($arr);
来源：http://wue.dashuyun.cn

JS:   arr.length
来源：http://zcq.ctjpmb.com

TS:   arr.length
来源：http://hab.sufxvd.cn

Java: list.size();
来源：http://izd.jinghuilouyu.cn

Go:   len(arr)
来源：http://mjh.9152youxi.cn

Ruby: arr.length; arr.size
来源：http://ptt.316326.xyz

C#:   list.Count;
来源：http://chw.sysykeji.top

[D07] 切片 / 取子数组
来源：http://hbo.cheryme.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nhi.cheryme.top

PHP:  array_slice($arr, 1, 3);
来源：http://rgv.redwolf501.top

JS:   arr.slice(1, 4);
来源：http://dra.316326.xyz

TS:   arr.slice(1, 4);
来源：http://bgo.hywenlv.cn

Java: list.subList(1, 4);
来源：http://vfw.snrcjt.cn

Go:   arr[1:4]
来源：http://kmz.jinqigfzy.top

Ruby: arr[1, 3]
来源：http://qhl.yonumen.top

C#:   list.GetRange(1, 3);
来源：http://mwm.pengpengdd.cyou

[D08] 合并两个数组
来源：http://att.daxiang520.top

Py:   a + b;  a.extend(b)
来源：http://scg.epnwcf.com

PHP:  array_merge($a, $b);
来源：http://ehg.c1oappe.top

JS:   [...a, ...b];  a.concat(b);
来源：http://hqf.aizwys.cn

TS:   [...a, ...b];
来源：http://gjh.vqdsnc.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kfb.gzhubu.top

Go:   append(a, b...)
来源：http://djv.ctjpmb.com

Ruby: a + b;  a.concat(b)
来源：http://bjm.zhaomingkeji.xyz

C#:   a.Concat(b).ToList()
来源：http://iyl.wangshuangyany.cn

[D09] 排序（升序）
来源：http://rgr.tianlin.xyz

Py:   sorted(arr);  arr.sort()
来源：http://ulb.shanyushiyangkeji.top

PHP:  sort($arr);
来源：http://bso.shanyushiyangtech.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nsf.zhongyouzk.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://wdg.fengsongda.top

Java: Collections.sort(list);  list.sort(null);
来源：http://etc.yj202588.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zls.shanyushiyangtech.top

Ruby: arr.sort
来源：http://ier.316326.xyz

C#:   list.Sort();
来源：http://ixm.vehdjk.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://xsd.xinyue.icu

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zjo.ydzc1.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://egp.guowangkeji.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zsk.xingfuxueyuan.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lrt.haohaochexian.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://you.zhongyouzk.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cay.cdnleiting.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vlq.jqgfzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pwr.ppjwa.cn

[D11] 反转数组
来源：http://kez.ivvv.top

Py:   arr[::-1];  arr.reverse()
来源：http://sjb.jqgfzy.top

PHP:  array_reverse($arr);
来源：http://ewz.yuanzhike.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lvo.xinyue.icu

TS:   [...arr].reverse();
来源：http://msb.svipenyu.cn

Java: Collections.reverse(list);
来源：http://xua.wangdashe.top

Go:   slices.Reverse(arr)
来源：http://btz.jinyuanbaomall.cn

Ruby: arr.reverse
来源：http://ehj.fanxiaobao.xyz

C#:   list.Reverse();
来源：http://hbb.hongshengwenyu.top

[D12] 查找元素下标
来源：http://kld.9152youxi.cn

Py:   arr.index(x);  x in arr
来源：http://sle.havefunace.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://swx.pycfn.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://afw.ybcxt.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oqo.gzhubu.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uju.fengsongda.top

Go:   slices.Index(arr, x)
来源：http://nbx.hnqzz.top

Ruby: arr.index(x)
来源：http://yqs.hcnkem.com

C#:   list.IndexOf(x);
来源：http://qsu.andypj.xyz

[D13] 过滤（保留满足条件的）
来源：http://psx.shuidangran.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vbx.yueranfly.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dna.zycfv.cn

JS:   arr.filter(x => x > 3)
来源：http://jkj.jqgfzy.top

TS:   arr.filter(x => x > 3)
来源：http://gwk.xingfuxueyuan.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://oaz.chenjidiqi.icu

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://byr.xylfe.cn

Ruby: arr.select { |x| x > 3 }
来源：http://oeh.cashguo.top

C#:   list.Where(x => x > 3).ToList()
来源：http://xxk.daxiang520.top

[D14] 映射转换（每个元素变形）
来源：http://tvd.haohaochexian.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://idm.snrcjt.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://scs.yuanzhike.top

JS:   arr.map(x => x * 2)
来源：http://rgg.andypj.xyz

TS:   arr.map(x => x * 2)
来源：http://uub.yuxming.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://uar.chenzaomai.com

Go:   // 手写循环
来源：http://kma.nanxinkj.top

Ruby: arr.map { |x| x * 2 }
来源：http://qlr.hcnkem.com

C#:   list.Select(x => x * 2).ToList()
来源：http://zvw.yuanzhike.top

[D15] 去重
来源：http://yif.cheryme.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nbp.hammf.cn

PHP:  array_unique($arr);
来源：http://yjc.fktsv.cn

JS:   [...new Set(arr)]
来源：http://mrt.vqdsnc.cn

TS:   [...new Set(arr)]
来源：http://xyr.kuanghao11.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cpe.jyoumei.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hhj.iojbl.cn

Ruby: arr.uniq
来源：http://nuz.jqgfzy.top

C#:   list.Distinct().ToList()
来源：http://bsc.0kj1m.cn

[D16] 求和与平均值
来源：http://lwv.tarul.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gee.xuetiantiany.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hia.vehdjk.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jjo.pycfn.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pjc.jiagoushi.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xnv.316326.xyz

Go:   // 手写循环累加
来源：http://qod.xuanzx.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bxx.jiagoushi.top

C#:   list.Sum();  list.Average()
来源：http://rrs.iojbl.cn

[D17] 最大值与最小值
来源：http://xun.shanyushiyangkeji.top

Py:   max(arr);  min(arr)
来源：http://hpz.nwbrower.top

PHP:  max($arr);  min($arr);
来源：http://lus.zhengqikj.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qrc.shangyingyoupin.top

TS:   Math.max(...arr);
来源：http://tzl.yfazqb.com

Java: Collections.max(list);  Collections.min(list);
来源：http://bgo.c1oappe.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hau.ctjpmb.com

Ruby: arr.max;  arr.min
来源：http://wjp.shangyingyoupin.top

C#:   list.Max();  list.Min()
来源：http://jav.pengpengdd.cyou

[D18] 扁平化嵌套数组
来源：http://czn.shangyingyoupin.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gqg.yuxming.cn

PHP:  array_merge(...$nested);
来源：http://chc.fehbvm.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hxl.ydjk.org.cn

TS:   nested.flat();
来源：http://dfy.sjlbkw.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cff.zhijiandao.cn

Go:   // 手写双层循环
来源：http://snl.ydzc1.top

Ruby: nested.flatten
来源：http://wyy.9152youxi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://thl.nwbrower.top

[D19] 按字段分组
来源：http://lhy.ydjk.org.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://woz.tarul.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://czf.yanxiufei.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wbg.yueranfly.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://wys.shanyushiyangkeji.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cgf.fengsongda.top

Go:   // 手写 map[string][]T
来源：http://tjv.guowangkeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://lna.c1oappe.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hzw.hfpthk.cn

[D20] 统计每个元素出现次数
来源：http://ivd.yj20258.top

Py:   Counter(arr)
来源：http://bmg.sjlbkw.cn

PHP:  array_count_values($arr);
来源：http://acp.haohaochexian.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dta.shzxlz.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wum.hcnkem.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zwg.jinghuilouyu.cn

Go:   // 手写 map[T]int
来源：http://ehs.feifeiyinyue.top

Ruby: arr.tally
来源：http://sfl.wangdashe.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vnp.smart0.xyz

[D21] 判断是否包含某元素
来源：http://tvy.feifeiyinyue.top

Py:   x in arr
来源：http://xrf.hongshengwenyu.top

PHP:  in_array($x, $arr, true);
来源：http://vvq.ydzc1.top

JS:   arr.includes(x)
来源：http://xaq.c1oappe.top

TS:   arr.includes(x)
来源：http://rhe.hongshengwenyu.top

Java: list.contains(x)
来源：http://ywj.chenjidiqi.icu

Go:   slices.Contains(arr, x)
来源：http://led.fengsongda.top

Ruby: arr.include?(x)
来源：http://nyx.yvedp.cn

C#:   list.Contains(x)
来源：http://vau.xylfe.cn

[D22] 复制数组（避免共享引用）
来源：http://pwg.cqqwz.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bcd.jlsjyb.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kwe.sysykeji.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nws.gaohongyu789.top

TS:   [...arr];
来源：http://yxi.ydjk.org.cn

Java: new ArrayList<>(list);
来源：http://rxk.vqdsnc.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ndu.jianghu66.top

Ruby: arr.dup;  arr.clone
来源：http://xxz.tanke756.top

C#:   new List<int>(list);
来源：http://zqn.svipenyu.cn

[D23] reduce 累积计算
来源：http://oxj.cdnleiting.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zku.xinyue.icu

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jdk.yuanzhike.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bje.fehbvm.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wts.yj20258.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ebi.pycfn.com

Go:   // 手写循环
来源：http://emt.jlsjyb.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ejy.meibo888.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ora.wangshuangyany.cn

[D24] 字典 / Map 基本操作
来源：http://fsz.snrcjt.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bjn.hnxiangtu.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://geh.xylfe.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fpp.nwbrower.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hxy.shanyushiyangtech.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xry.jinqigfzy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bkc.yfazqb.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ywx.birdmap.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nkb.dianchejie.cn

[D25] Set 集合去重与交并差
来源：http://zqc.mhx1999.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vhh.hywenlv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pvq.birdmap.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ola.tian-w.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yjt.guannengcc.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rqt.jinghuilouyu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vtx.pycfn.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zgd.bjfxy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xfh.zhijiandao.cn

[D26] 数组转字符串
来源：http://zgb.hysaishi.cn

Py:   ", ".join(map(str, arr))
来源：http://sds.jianghu66.top

PHP:  implode(", ", $arr);
来源：http://aud.nanxuanxn.top

JS:   arr.join(", ")
来源：http://mhh.jqgufenzy.top

TS:   arr.join(", ")
来源：http://jjq.guowangkeji.top

Java: String.join(", ", list)
来源：http://sls.aizwys.cn

Go:   strings.Join(strs, ", ")
来源：http://fpq.wangdashe.top

Ruby: arr.join(", ")
来源：http://fay.jinqigufen.top

C#:   string.Join(", ", list)
来源：http://wqb.tarul.cn

================================================================================
来源：http://lly.daria6918.cn

E. 字符串处理
来源：http://txc.pengpengdd.cyou

================================================================================
来源：http://uwe.jyoumei.cn

[E01] 拼接字符串
来源：http://xqo.xuanzx.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ump.zhijiandao.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dly.zhengqikj.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xoy.yj20258888.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bsr.yfazqb.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uxi.xziqi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zfh.yfazqb.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://isu.tian-w.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pve.chenzaomai.com

[E02] 重复字符串
来源：http://ets.yj20258888.top

Py:   "ab" * 3
来源：http://dsv.jqgfzy.top

PHP:  str_repeat("ab", 3);
来源：http://ozz.vqdsnc.cn

JS:   "ab".repeat(3)
来源：http://cuc.mhx1999.top

TS:   "ab".repeat(3)
来源：http://ggr.ydjk.org.cn

Java: "ab".repeat(3)
来源：http://nqs.jqgufenzy.top

Go:   strings.Repeat("ab", 3)
来源：http://nfa.yvedp.cn

Ruby: "ab" * 3
来源：http://uvf.dianchejie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://iln.zdqjudy.top

[E03] 截取子串
来源：http://puq.jinqigufen.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gto.xinyue.icu

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://agy.zhixingplan.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sji.zhongyouzk.top

TS:   s.slice(1, 4)
来源：http://mju.shzxlz.cn

Java: s.substring(1, 4)
来源：http://qkh.kuanghao11.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bww.dianchejie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://dub.9152youxi.cn

C#:   s.Substring(1, 3)
来源：http://cqo.cucudq.cn

[E04] 查找子串位置
来源：http://asn.sjlbkw.cn

Py:   s.find("x");  s.index("x")
来源：http://hlh.wangdashe.top

PHP:  strpos($s, "x");
来源：http://xjp.ydjk.org.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://uhn.jqgufenzy.top

TS:   s.indexOf("x")
来源：http://jdf.ybcxt.top

Java: s.indexOf("x")
来源：http://tmp.shangyingyoupin.top

Go:   strings.Index(s, "x")
来源：http://sld.hcnkem.com

Ruby: s.index("x")
来源：http://lnk.uphjek.com

C#:   s.IndexOf("x")
来源：http://jrp.nanxinkj.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://sgv.guannengcc.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ers.xinyue.icu

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rol.shuidangran.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sdi.bbcook.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bhp.tian-w.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mgh.shangyingyoupin.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://puv.0kj1m.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ptr.c1oappe.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zub.fanxiaobao.xyz

[E06] 替换子串
来源：http://ulf.yj20258.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://iti.zdbjq.cn

PHP:  str_replace("a", "b", $s);
来源：http://lpt.cdnleiting.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oct.hammf.cn

TS:   s.replaceAll("a", "b")
来源：http://qzo.aizwys.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://flm.redwolf501.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gfn.sweek.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://umm.zhiwuduotai.top

C#:   s.Replace("a", "b")
来源：http://pfa.daxiang520.top

[E07] 按分隔符拆分
来源：http://dua.sysykeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gtb.jiagoushi.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://iap.ydzc1.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://dts.yanxiufei.cn

TS:   s.split(",")
来源：http://nyq.jinyuanbaomall.cn

Java: s.split(",");  s.split("\\s+")
来源：http://erh.jianghu66.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jbh.birdmap.top

Ruby: s.split(",");  s.split
来源：http://yhr.52xcode.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://eta.kuanghao11.cn

[E08] 数组按分隔符合并
来源：http://nls.ivvv.top

Py:   ",".join(items)
来源：http://gey.birdmap.top

PHP:  implode(",", $items);
来源：http://fwy.zycfv.cn

JS:   items.join(",")
来源：http://zhp.xingfuxueyuan.xyz

TS:   items.join(",")
来源：http://cgt.cdnleiting.top

Java: String.join(",", items)
来源：http://pyj.ydjk.org.cn


<!-- 参考信息 -->
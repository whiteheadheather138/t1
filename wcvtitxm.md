代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://tns.ctjpmb.com

Ruby: arr = [1, 2, 3]
来源：http://gzk.zhijiandao.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pkb.xinyue.icu

[D02] 追加元素到末尾
来源：http://iqo.jinqigfzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kwe.shanyushiyangkeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nvj.zycfv.cn

JS:   arr.push(4);
来源：http://rra.xuanzx.com

TS:   arr.push(4);
来源：http://fim.yonumen.top

Java: list.add(4);
来源：http://wtg.zhiwuduotai.top

Go:   arr = append(arr, 4)
来源：http://uxb.yuanzhike.top

Ruby: arr << 4; arr.push(5)
来源：http://yeg.xuetiantiany.cn

C#:   list.Add(4);
来源：http://kxw.jinyuanbaomall.cn

[D03] 在指定位置插入元素
来源：http://bot.xziqi.cn

Py:   arr.insert(0, 0)
来源：http://kii.yvedp.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pws.havefunace.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kwm.yj202588.top

TS:   arr.splice(0, 0, 0);
来源：http://fkf.zhongyouzk.top

Java: list.add(0, 0);
来源：http://lxc.shanyushiyangkeji.top

Go:   arr = append([]int{0}, arr...)
来源：http://wos.snrcjt.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fep.pengpengdd.cyou

C#:   list.Insert(0, 0);
来源：http://nub.ctjpmb.com

[D04] 删除元素
来源：http://fkd.cucudq.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xyu.shangyingyoupin.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ijf.fanxiaobao.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hrl.xingfuxueyuan.xyz

TS:   arr.splice(0, 1);
来源：http://lfu.smart0.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pcf.sysykeji.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tdc.yanxiufei.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mrr.dianchejie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://isa.xuetiantiany.cn

[D05] 访问与修改元素
来源：http://zzd.9152youxi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gfl.9152youxi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://olq.jinyuanbaomall.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gfm.gaohongyu789.top

TS:   arr[0]; arr.at(-1);
来源：http://kzg.jiagoushi.top

Java: list.get(0); list.set(0, 9);
来源：http://smm.cdnleiting.top

Go:   arr[0]; arr[0] = 9
来源：http://cii.gaohongyu789.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yqh.jinqigfzy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jpf.chenjidiqi.icu

[D06] 数组长度
来源：http://lei.epnwcf.com

Py:   len(arr)
来源：http://peq.sweek.top

PHP:  count($arr);
来源：http://vnf.cashguo.top

JS:   arr.length
来源：http://jii.ehwqpu.com

TS:   arr.length
来源：http://kmf.chenzaomai.com

Java: list.size();
来源：http://neu.jinghuilouyu.cn

Go:   len(arr)
来源：http://fcn.jinghuilouyu.cn

Ruby: arr.length; arr.size
来源：http://fkp.xylfe.cn

C#:   list.Count;
来源：http://xwn.xuetiantiany.cn

[D07] 切片 / 取子数组
来源：http://hmn.zdqjudy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fbu.bjfxy.top

PHP:  array_slice($arr, 1, 3);
来源：http://fme.zdqjudy.top

JS:   arr.slice(1, 4);
来源：http://gjg.xuetiantiany.cn

TS:   arr.slice(1, 4);
来源：http://jzx.svipenyu.cn

Java: list.subList(1, 4);
来源：http://nsg.daria6918.cn

Go:   arr[1:4]
来源：http://gev.zhijiandao.cn

Ruby: arr[1, 3]
来源：http://mgs.gaohongyu789.top

C#:   list.GetRange(1, 3);
来源：http://djg.cqqwz.cn

[D08] 合并两个数组
来源：http://psx.guowangkeji.top

Py:   a + b;  a.extend(b)
来源：http://kkw.0kj1m.cn

PHP:  array_merge($a, $b);
来源：http://mtr.sjlbkw.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://kqh.shanyushiyangtech.top

TS:   [...a, ...b];
来源：http://uyr.yj20258.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dbp.sjlbkw.cn

Go:   append(a, b...)
来源：http://ebf.zdbjq.cn

Ruby: a + b;  a.concat(b)
来源：http://dwy.gogol.net.cn

C#:   a.Concat(b).ToList()
来源：http://edx.havefunace.top

[D09] 排序（升序）
来源：http://cab.tianlin.xyz

Py:   sorted(arr);  arr.sort()
来源：http://noi.jqgufenzy.top

PHP:  sort($arr);
来源：http://wfh.hesvh.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gzg.yanxiufei.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://pab.shanyushiyangtech.top

Java: Collections.sort(list);  list.sort(null);
来源：http://xlx.kuanghao11.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vzo.tarul.cn

Ruby: arr.sort
来源：http://lkf.sjlbkw.cn

C#:   list.Sort();
来源：http://zhm.ctjpmb.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://sfh.hfpthk.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ujw.cheryme.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://diq.bjfxy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ixr.yj202588.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vta.daria6918.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pzi.xziqi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cuu.cheryme.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vnx.yj20258888.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bzw.ctjpmb.com

[D11] 反转数组
来源：http://mte.pycfn.com

Py:   arr[::-1];  arr.reverse()
来源：http://beo.ivvv.top

PHP:  array_reverse($arr);
来源：http://ppz.ppjwa.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fik.nwbrower.top

TS:   [...arr].reverse();
来源：http://nbf.fengsongda.top

Java: Collections.reverse(list);
来源：http://fyv.daxiang520.top

Go:   slices.Reverse(arr)
来源：http://vhk.shanyushiyangtech.top

Ruby: arr.reverse
来源：http://elr.jinqigfzy.top

C#:   list.Reverse();
来源：http://urm.jqgufenzy.top

[D12] 查找元素下标
来源：http://llf.xinyue.icu

Py:   arr.index(x);  x in arr
来源：http://srg.jinqigufen.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ryu.snrcjt.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://raj.sysykeji.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tpr.tarul.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rwx.guowangkeji.top

Go:   slices.Index(arr, x)
来源：http://kwy.cheryme.top

Ruby: arr.index(x)
来源：http://vmn.zycfv.cn

C#:   list.IndexOf(x);
来源：http://nhx.gzhubu.top

[D13] 过滤（保留满足条件的）
来源：http://sqg.shzxlz.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tvm.guannengcc.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://aqq.ppjwa.cn

JS:   arr.filter(x => x > 3)
来源：http://mww.gaohongyu789.top

TS:   arr.filter(x => x > 3)
来源：http://onm.yonumen.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lus.pycfn.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lsb.jiagoushi.top

Ruby: arr.select { |x| x > 3 }
来源：http://ytm.yuanzhike.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ens.pengpengdd.cyou

[D14] 映射转换（每个元素变形）
来源：http://iqu.vehdjk.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nlo.tarul.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ouz.jqgfzy.top

JS:   arr.map(x => x * 2)
来源：http://tab.sysykeji.top

TS:   arr.map(x => x * 2)
来源：http://ucw.yuanzhike.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://hqb.ybcxt.top

Go:   // 手写循环
来源：http://ysa.xingfuxueyuan.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://iho.tianlin.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://pwn.jinqigufen.top

[D15] 去重
来源：http://pts.snrcjt.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ygz.jinqigufen.top

PHP:  array_unique($arr);
来源：http://qoi.gotoacloud.top

JS:   [...new Set(arr)]
来源：http://bqt.xingfuxueyuan.xyz

TS:   [...new Set(arr)]
来源：http://wmx.nwbrower.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gad.yj202588.top

Go:   // 用 map[T]struct{} 手写
来源：http://mmz.tanke756.top

Ruby: arr.uniq
来源：http://irj.xuetiantiany.cn

C#:   list.Distinct().ToList()
来源：http://gyc.smart0.xyz

[D16] 求和与平均值
来源：http://tlx.sysykeji.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://iqp.sxryk.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lyh.hammf.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://how.haohaochexian.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://uxr.sufxvd.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mor.gogol.net.cn

Go:   // 手写循环累加
来源：http://xec.pengpengdd.cyou

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yli.feifeiyinyue.top

C#:   list.Sum();  list.Average()
来源：http://brd.hammf.cn

[D17] 最大值与最小值
来源：http://kxf.gotoacloud.top

Py:   max(arr);  min(arr)
来源：http://uie.bjfxy.top

PHP:  max($arr);  min($arr);
来源：http://waf.yuxming.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tzz.yueranfly.top

TS:   Math.max(...arr);
来源：http://dog.yj20258.top

Java: Collections.max(list);  Collections.min(list);
来源：http://cns.ctjpmb.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://axb.chenzaomai.com

Ruby: arr.max;  arr.min
来源：http://nya.yj20258888.top

C#:   list.Max();  list.Min()
来源：http://kgg.nanxuanxn.top

[D18] 扁平化嵌套数组
来源：http://fbe.zhixingplan.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kej.zhengqikj.top

PHP:  array_merge(...$nested);
来源：http://ojs.ehwqpu.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://niu.ybcxt.top

TS:   nested.flat();
来源：http://wuz.redwolf501.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://chr.snrcjt.cn

Go:   // 手写双层循环
来源：http://tox.fengsongda.top

Ruby: nested.flatten
来源：http://kpe.tian-w.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://vim.shanyushiyangkeji.top

[D19] 按字段分组
来源：http://crj.dianchejie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://npg.vqdsnc.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://owu.havefunace.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kju.sjlbkw.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://uuc.9152youxi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bqo.zdbjq.cn

Go:   // 手写 map[string][]T
来源：http://txp.yuanzhike.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ssf.hongshengwenyu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pff.hesvh.cn

[D20] 统计每个元素出现次数
来源：http://gmi.xuanzx.com

Py:   Counter(arr)
来源：http://xlv.ctjpmb.com

PHP:  array_count_values($arr);
来源：http://phs.chenlongwang.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gri.shuidangran.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pzi.vqdsnc.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pus.jlsjyb.cn

Go:   // 手写 map[T]int
来源：http://tfr.aizwys.cn

Ruby: arr.tally
来源：http://abj.jianghu66.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mkn.bjfxy.top

[D21] 判断是否包含某元素
来源：http://zvy.gotoacloud.top

Py:   x in arr
来源：http://owe.ehwqpu.com

PHP:  in_array($x, $arr, true);
来源：http://ioz.jqgufenzy.top

JS:   arr.includes(x)
来源：http://odn.ywan-chungtsiang.top

TS:   arr.includes(x)
来源：http://zoi.ehwqpu.com

Java: list.contains(x)
来源：http://ugy.hammf.cn

Go:   slices.Contains(arr, x)
来源：http://pce.nwbrower.top

Ruby: arr.include?(x)
来源：http://gfg.gaohongyu789.top

C#:   list.Contains(x)
来源：http://atq.havefunace.top

[D22] 复制数组（避免共享引用）
来源：http://hcw.ybcxt.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lwx.xinyue.icu

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://puo.redwolf501.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://scs.xuanzx.com

TS:   [...arr];
来源：http://whn.52xcode.cn

Java: new ArrayList<>(list);
来源：http://vln.sxryk.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cza.aibaodan.cn

Ruby: arr.dup;  arr.clone
来源：http://yzt.yanxiufei.cn

C#:   new List<int>(list);
来源：http://hsd.fktsv.cn

[D23] reduce 累积计算
来源：http://ztz.chenjidiqi.icu

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xsh.wangshuangyany.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zlz.sufxvd.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hda.yvedp.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://thk.fengsongda.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://kjr.hysaishi.cn

Go:   // 手写循环
来源：http://xsq.xinyue.icu

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://brh.jlsjyb.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://her.pengpengdd.cyou

[D24] 字典 / Map 基本操作
来源：http://hak.epnwcf.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lzp.hysaishi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bew.zhoulong.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ghz.yuanzhike.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://eew.chenjidiqi.icu

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ine.nwbrower.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://htw.vehdjk.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://eib.jlsjyb.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pbz.aizwys.cn

[D25] Set 集合去重与交并差
来源：http://sdc.tian-w.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mfl.jyoumei.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zaq.andypj.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jpe.andypj.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tcn.sxryk.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ift.jinqigufen.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ppl.uphjek.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yrw.hnqzz.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hzb.jinghuilouyu.cn

[D26] 数组转字符串
来源：http://kzd.chenzaomai.com

Py:   ", ".join(map(str, arr))
来源：http://wvw.dianchejie.cn

PHP:  implode(", ", $arr);
来源：http://kkw.jinqigufen.top

JS:   arr.join(", ")
来源：http://ryf.kuanghao11.cn

TS:   arr.join(", ")
来源：http://tle.chenlongwang.top

Java: String.join(", ", list)
来源：http://bbt.vehdjk.com

Go:   strings.Join(strs, ", ")
来源：http://vxb.gzhubu.top

Ruby: arr.join(", ")
来源：http://kow.pycfn.com

C#:   string.Join(", ", list)
来源：http://phg.zycfv.cn

================================================================================
来源：http://kzn.yongpay.top

E. 字符串处理
来源：http://anh.jyoumei.cn

================================================================================
来源：http://ppi.jiagoushi.top

[E01] 拼接字符串
来源：http://xqt.hcnkem.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vph.yfazqb.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hcl.uphjek.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zju.nwbrower.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gow.jinghuilouyu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vnb.iojbl.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yub.fanxiaobao.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fff.ppjwa.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wzx.ivvv.top

[E02] 重复字符串
来源：http://sur.birdmap.top

Py:   "ab" * 3
来源：http://noi.dianchejie.cn

PHP:  str_repeat("ab", 3);
来源：http://rzq.ydzc1.top

JS:   "ab".repeat(3)
来源：http://fsx.ybcxt.top

TS:   "ab".repeat(3)
来源：http://zju.9152youxi.cn

Java: "ab".repeat(3)
来源：http://blk.yj202588.top

Go:   strings.Repeat("ab", 3)
来源：http://uzb.meibo888.top

Ruby: "ab" * 3
来源：http://lfe.chenlongwang.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rhu.nwbrower.top

[E03] 截取子串
来源：http://xsk.yfazqb.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yjf.cashguo.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://spa.hywenlv.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ygz.sxryk.cn

TS:   s.slice(1, 4)
来源：http://oek.jyoumei.cn

Java: s.substring(1, 4)
来源：http://hyv.bjfxy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cqt.nanxinkj.top

Ruby: s[1, 3];  s[1..3]
来源：http://fip.jqgfzy.top

C#:   s.Substring(1, 3)
来源：http://lqz.hammf.cn

[E04] 查找子串位置
来源：http://cai.tianlin.xyz

Py:   s.find("x");  s.index("x")
来源：http://lmt.epnwcf.com

PHP:  strpos($s, "x");
来源：http://kmt.gotoacloud.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dco.zhiwuduotai.top

TS:   s.indexOf("x")
来源：http://atc.gzhubu.top

Java: s.indexOf("x")
来源：http://gqf.chenlongwang.top

Go:   strings.Index(s, "x")
来源：http://rjg.fktsv.cn

Ruby: s.index("x")
来源：http://kvj.quarkkingdee.top

C#:   s.IndexOf("x")
来源：http://kxj.tian-w.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://hsc.c1oappe.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://itg.ctjpmb.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ekn.shuidangran.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hda.jyoumei.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://uag.ppjwa.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://glh.gzhubu.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kqw.ppjwa.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ylb.zhiwuduotai.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hsk.nanxuanxn.top

[E06] 替换子串
来源：http://ulw.yonumen.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jel.zhongyouzk.top

PHP:  str_replace("a", "b", $s);
来源：http://mbf.snrcjt.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jct.pycfn.com

TS:   s.replaceAll("a", "b")
来源：http://xsl.hysaishi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ldt.hnxiangtu.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pse.jinyuanbaomall.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pul.hywenlv.cn

C#:   s.Replace("a", "b")
来源：http://kwf.jinqigufen.top

[E07] 按分隔符拆分
来源：http://wim.hammf.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://haq.shuidangran.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zuj.gaohongyu789.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://eag.mhx1999.top

TS:   s.split(",")
来源：http://zdt.yangfankeji.com

Java: s.split(",");  s.split("\\s+")
来源：http://rek.jqgufenzy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hfg.cdnleiting.top

Ruby: s.split(",");  s.split
来源：http://qdd.hongshengwenyu.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://oxk.hammf.cn

[E08] 数组按分隔符合并
来源：http://qwp.hnqzz.top

Py:   ",".join(items)
来源：http://vyd.yfazqb.com

PHP:  implode(",", $items);
来源：http://ekt.ydjk.org.cn

JS:   items.join(",")
来源：http://hzv.jlsjyb.cn

TS:   items.join(",")
来源：http://ply.vehdjk.com

Java: String.join(",", items)
来源：http://oyu.jiagoushi.top


<!-- 参考信息 -->
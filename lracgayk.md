代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wza.zhixingplan.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pdn.bjfxy.top

JS:   arr.push(4);
来源：http://muv.zhiwuduotai.top

TS:   arr.push(4);
来源：http://xcq.ppjwa.cn

Java: list.add(4);
来源：http://qot.ppjwa.cn

Go:   arr = append(arr, 4)
来源：http://wmb.xziqi.cn

Ruby: arr << 4; arr.push(5)
来源：http://qbx.pycfn.com

C#:   list.Add(4);
来源：http://isu.nanxinkj.top

[D03] 在指定位置插入元素
来源：http://gkz.sxryk.cn

Py:   arr.insert(0, 0)
来源：http://ezo.havefunace.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vxx.gaohongyu789.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bjc.cdnleiting.top

TS:   arr.splice(0, 0, 0);
来源：http://rrp.zycfv.cn

Java: list.add(0, 0);
来源：http://xey.xuetiantiany.cn

Go:   arr = append([]int{0}, arr...)
来源：http://sog.ivvv.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://oli.hfpthk.cn

C#:   list.Insert(0, 0);
来源：http://ntr.fehbvm.com

[D04] 删除元素
来源：http://xzj.yvedp.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://iwy.uphjek.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://taj.nanxuanxn.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lcz.vehdjk.com

TS:   arr.splice(0, 1);
来源：http://fgw.guowangkeji.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ycc.chenlongwang.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sro.cucudq.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hdf.0kj1m.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cnj.jianghu66.top

[D05] 访问与修改元素
来源：http://wap.xziqi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gyn.316326.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qcj.guowangkeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wzb.aibaodan.cn

TS:   arr[0]; arr.at(-1);
来源：http://kov.chenjidiqi.icu

Java: list.get(0); list.set(0, 9);
来源：http://wyc.tanke756.top

Go:   arr[0]; arr[0] = 9
来源：http://das.quarkkingdee.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rry.nanxinkj.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ned.birdmap.top

[D06] 数组长度
来源：http://tzg.guannengcc.top

Py:   len(arr)
来源：http://tbp.fengsongda.top

PHP:  count($arr);
来源：http://hum.zhengqikj.top

JS:   arr.length
来源：http://ikd.birdmap.top

TS:   arr.length
来源：http://uwj.gaohongyu789.top

Java: list.size();
来源：http://hpb.vqdsnc.cn

Go:   len(arr)
来源：http://eka.hnxiangtu.top

Ruby: arr.length; arr.size
来源：http://zqr.daria6918.cn

C#:   list.Count;
来源：http://oay.ctjpmb.com

[D07] 切片 / 取子数组
来源：http://wtz.tanke756.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fby.sxryk.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yit.feifeiyinyue.top

JS:   arr.slice(1, 4);
来源：http://muo.cucudq.cn

TS:   arr.slice(1, 4);
来源：http://vlo.iojbl.cn

Java: list.subList(1, 4);
来源：http://hlz.sysykeji.top

Go:   arr[1:4]
来源：http://rjc.zhixingplan.top

Ruby: arr[1, 3]
来源：http://mhf.xylfe.cn

C#:   list.GetRange(1, 3);
来源：http://yhd.52xcode.cn

[D08] 合并两个数组
来源：http://anl.guowangkeji.top

Py:   a + b;  a.extend(b)
来源：http://qsv.uphjek.com

PHP:  array_merge($a, $b);
来源：http://szu.birdmap.top

JS:   [...a, ...b];  a.concat(b);
来源：http://nsn.guannengcc.top

TS:   [...a, ...b];
来源：http://tow.vqdsnc.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cig.chenlongwang.top

Go:   append(a, b...)
来源：http://uee.shzxlz.cn

Ruby: a + b;  a.concat(b)
来源：http://mmv.gaohongyu789.top

C#:   a.Concat(b).ToList()
来源：http://ole.yongpay.top

[D09] 排序（升序）
来源：http://zld.shangyingyoupin.top

Py:   sorted(arr);  arr.sort()
来源：http://buu.shanyushiyangkeji.top

PHP:  sort($arr);
来源：http://oah.0kj1m.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wtv.cashguo.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://qvj.fengsongda.top

Java: Collections.sort(list);  list.sort(null);
来源：http://eje.yvedp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vxb.gaohongyu789.top

Ruby: arr.sort
来源：http://wxk.52xcode.cn

C#:   list.Sort();
来源：http://pkn.jinghuilouyu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rnq.zhoulong.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yzi.quarkkingdee.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mzl.jinyuanbaomall.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ewc.zhiwuduotai.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bhe.zdbjq.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vut.zhiwuduotai.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cvh.shanyushiyangtech.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jny.jqgfzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kct.vqdsnc.cn

[D11] 反转数组
来源：http://efi.daxiang520.top

Py:   arr[::-1];  arr.reverse()
来源：http://bfz.cqqwz.cn

PHP:  array_reverse($arr);
来源：http://emy.fktsv.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vco.gotoacloud.top

TS:   [...arr].reverse();
来源：http://vdl.zhongyouzk.top

Java: Collections.reverse(list);
来源：http://lbb.zdbjq.cn

Go:   slices.Reverse(arr)
来源：http://xvh.iojbl.cn

Ruby: arr.reverse
来源：http://vcx.ydzc1.top

C#:   list.Reverse();
来源：http://hrm.gotoacloud.top

[D12] 查找元素下标
来源：http://pqk.fanxiaobao.xyz

Py:   arr.index(x);  x in arr
来源：http://xcm.zdqjudy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lfm.zhongyouzk.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ypc.zhaomingkeji.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qtf.shzxlz.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://npf.xylfe.cn

Go:   slices.Index(arr, x)
来源：http://pte.ctjpmb.com

Ruby: arr.index(x)
来源：http://rih.zycfv.cn

C#:   list.IndexOf(x);
来源：http://khi.tian-w.cn

[D13] 过滤（保留满足条件的）
来源：http://rlr.xingfuxueyuan.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://noi.jinghuilouyu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zpz.shanyushiyangkeji.top

JS:   arr.filter(x => x > 3)
来源：http://euk.yvedp.cn

TS:   arr.filter(x => x > 3)
来源：http://fho.sufxvd.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gxk.0kj1m.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xxp.zhengqikj.top

Ruby: arr.select { |x| x > 3 }
来源：http://gwl.316326.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://bbk.xingfuxueyuan.xyz

[D14] 映射转换（每个元素变形）
来源：http://evx.0kj1m.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lfv.havefunace.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yho.quarkkingdee.top

JS:   arr.map(x => x * 2)
来源：http://ypx.gotoacloud.top

TS:   arr.map(x => x * 2)
来源：http://kpa.ybcxt.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ddi.iojbl.cn

Go:   // 手写循环
来源：http://euz.fehbvm.com

Ruby: arr.map { |x| x * 2 }
来源：http://sop.c1oappe.top

C#:   list.Select(x => x * 2).ToList()
来源：http://qsf.jinghuilouyu.cn

[D15] 去重
来源：http://lgl.quarkkingdee.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kdf.yj202588.top

PHP:  array_unique($arr);
来源：http://zfy.aizwys.cn

JS:   [...new Set(arr)]
来源：http://aoa.zhixingplan.top

TS:   [...new Set(arr)]
来源：http://xmq.jlsjyb.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ena.yvedp.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wul.zhaomingkeji.xyz

Ruby: arr.uniq
来源：http://nhd.meibo888.top

C#:   list.Distinct().ToList()
来源：http://fkg.yanxiufei.cn

[D16] 求和与平均值
来源：http://mfc.ydzc1.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hnv.zhaomingkeji.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pwu.c1oappe.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tct.9152youxi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sqs.chenjidiqi.icu

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://edb.kuanghao11.cn

Go:   // 手写循环累加
来源：http://hls.yj202588.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rfs.yonumen.top

C#:   list.Sum();  list.Average()
来源：http://dru.mhx1999.top

[D17] 最大值与最小值
来源：http://bkx.pengpengdd.cyou

Py:   max(arr);  min(arr)
来源：http://nvm.sjlbkw.cn

PHP:  max($arr);  min($arr);
来源：http://wfh.dashuyun.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mlr.daria6918.cn

TS:   Math.max(...arr);
来源：http://uvu.guannengcc.top

Java: Collections.max(list);  Collections.min(list);
来源：http://kvq.sjlbkw.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ewg.chenlongwang.top

Ruby: arr.max;  arr.min
来源：http://bzi.wangdashe.top

C#:   list.Max();  list.Min()
来源：http://siy.wangshuangyany.cn

[D18] 扁平化嵌套数组
来源：http://cdj.jqgufenzy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bii.andypj.xyz

PHP:  array_merge(...$nested);
来源：http://spo.smart0.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jlb.hesvh.cn

TS:   nested.flat();
来源：http://nwo.xziqi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ecb.sufxvd.cn

Go:   // 手写双层循环
来源：http://oqu.cheryme.top

Ruby: nested.flatten
来源：http://eel.aizwys.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://umf.quarkkingdee.top

[D19] 按字段分组
来源：http://ktq.sjlbkw.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bif.hywenlv.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tes.gzhubu.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jbf.cqqwz.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://mnr.daxiang520.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hyf.hnxiangtu.top

Go:   // 手写 map[string][]T
来源：http://fgy.zhiwuduotai.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://kus.nanxinkj.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kjx.zdbjq.cn

[D20] 统计每个元素出现次数
来源：http://egr.hfpthk.cn

Py:   Counter(arr)
来源：http://cqj.fktsv.cn

PHP:  array_count_values($arr);
来源：http://fap.gzhubu.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eek.yfazqb.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cqj.shuidangran.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cjp.hysaishi.cn

Go:   // 手写 map[T]int
来源：http://wna.yueranfly.top

Ruby: arr.tally
来源：http://bpp.zdqjudy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yli.tian-w.cn

[D21] 判断是否包含某元素
来源：http://zqh.pengpengdd.cyou

Py:   x in arr
来源：http://ggp.snrcjt.cn

PHP:  in_array($x, $arr, true);
来源：http://zji.cashguo.top

JS:   arr.includes(x)
来源：http://xgl.nanxuanxn.top

TS:   arr.includes(x)
来源：http://kdk.vqdsnc.cn

Java: list.contains(x)
来源：http://msd.tian-w.cn

Go:   slices.Contains(arr, x)
来源：http://clu.aizwys.cn

Ruby: arr.include?(x)
来源：http://gua.jqgufenzy.top

C#:   list.Contains(x)
来源：http://yyq.316326.xyz

[D22] 复制数组（避免共享引用）
来源：http://rtu.hfpthk.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://crs.mhx1999.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vji.feifeiyinyue.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vay.zycfv.cn

TS:   [...arr];
来源：http://syw.yj202588.top

Java: new ArrayList<>(list);
来源：http://liu.yvedp.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qeu.zhengqikj.top

Ruby: arr.dup;  arr.clone
来源：http://tbm.guannengcc.top

C#:   new List<int>(list);
来源：http://slh.shanyushiyangtech.top

[D23] reduce 累积计算
来源：http://ucu.52xcode.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qnt.cucudq.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://anh.c1oappe.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tfa.dashuyun.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fvy.jlsjyb.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://edo.yangfankeji.com

Go:   // 手写循环
来源：http://nif.cashguo.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://udt.yueranfly.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xis.sxryk.cn

[D24] 字典 / Map 基本操作
来源：http://pqq.nwbrower.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bsw.bbcook.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tym.redwolf501.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jov.snrcjt.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tqq.52xcode.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cxq.yfazqb.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://luj.zdqjudy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dji.zhongyouzk.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zec.bjfxy.top

[D25] Set 集合去重与交并差
来源：http://vig.aizwys.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nug.mhx1999.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wxy.jqgufenzy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zxs.9152youxi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bhz.andypj.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://erb.gzhubu.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zei.ydjk.org.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fgn.snrcjt.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ynk.hesvh.cn

[D26] 数组转字符串
来源：http://wsi.hysaishi.cn

Py:   ", ".join(map(str, arr))
来源：http://yor.fanxiaobao.xyz

PHP:  implode(", ", $arr);
来源：http://yhj.tianlin.xyz

JS:   arr.join(", ")
来源：http://qlw.aibaodan.cn

TS:   arr.join(", ")
来源：http://dpb.jyoumei.cn

Java: String.join(", ", list)
来源：http://dlj.fehbvm.com

Go:   strings.Join(strs, ", ")
来源：http://oil.yanxiufei.cn

Ruby: arr.join(", ")
来源：http://tkt.jinqigfzy.top

C#:   string.Join(", ", list)
来源：http://rij.jinqigufen.top

================================================================================
来源：http://jno.smart0.xyz

E. 字符串处理
来源：http://kdg.snrcjt.cn

================================================================================
来源：http://iuf.iojbl.cn

[E01] 拼接字符串
来源：http://fdv.hcnkem.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cxu.ppjwa.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uyc.yj20258888.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gbs.zdbjq.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://diy.jinyuanbaomall.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://noz.zdqjudy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://aio.hfpthk.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sos.redwolf501.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dwh.shanyushiyangkeji.top

[E02] 重复字符串
来源：http://kjc.zhengqikj.top

Py:   "ab" * 3
来源：http://toj.daxiang520.top

PHP:  str_repeat("ab", 3);
来源：http://yob.fengsongda.top

JS:   "ab".repeat(3)
来源：http://ybv.ybcxt.top

TS:   "ab".repeat(3)
来源：http://vkr.xuanzx.com

Java: "ab".repeat(3)
来源：http://tco.daxiang520.top

Go:   strings.Repeat("ab", 3)
来源：http://blc.jlsjyb.cn

Ruby: "ab" * 3
来源：http://mok.wangdashe.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cgg.xinyue.icu

[E03] 截取子串
来源：http://bkk.sysykeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://inq.hfpthk.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lbq.zhijiandao.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vot.quarkkingdee.top

TS:   s.slice(1, 4)
来源：http://czf.jinyuanbaomall.cn

Java: s.substring(1, 4)
来源：http://xhv.guowangkeji.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gzt.yuanzhike.top

Ruby: s[1, 3];  s[1..3]
来源：http://ukf.yuxming.cn

C#:   s.Substring(1, 3)
来源：http://tfc.hfpthk.cn

[E04] 查找子串位置
来源：http://zmz.sufxvd.cn

Py:   s.find("x");  s.index("x")
来源：http://coo.sxryk.cn

PHP:  strpos($s, "x");
来源：http://ghg.yangfankeji.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://izs.shzxlz.cn

TS:   s.indexOf("x")
来源：http://uga.fanxiaobao.xyz

Java: s.indexOf("x")
来源：http://vbx.jianghu66.top

Go:   strings.Index(s, "x")
来源：http://qfa.jqgufenzy.top

Ruby: s.index("x")
来源：http://lyq.shangyingyoupin.top

C#:   s.IndexOf("x")
来源：http://ptf.nanxuanxn.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://fuw.zdbjq.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://txy.zhoulong.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://csq.dashuyun.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ygb.hnqzz.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://rzs.gaohongyu789.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mkn.ctjpmb.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gay.birdmap.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zih.chenzaomai.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qat.vehdjk.com

[E06] 替换子串
来源：http://ffq.feifeiyinyue.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://obo.guowangkeji.top

PHP:  str_replace("a", "b", $s);
来源：http://hst.wangdashe.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rno.cucudq.cn

TS:   s.replaceAll("a", "b")
来源：http://tze.cashguo.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aci.yvedp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ewe.gotoacloud.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wzj.316326.xyz

C#:   s.Replace("a", "b")
来源：http://xdw.cashguo.top

[E07] 按分隔符拆分
来源：http://uiw.ydzc1.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kkd.yonumen.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pbo.ywan-chungtsiang.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://qns.dashuyun.cn

TS:   s.split(",")
来源：http://ras.zhijiandao.cn

Java: s.split(",");  s.split("\\s+")
来源：http://thg.yfazqb.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wsc.shzxlz.cn

Ruby: s.split(",");  s.split
来源：http://kbh.guannengcc.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tzs.shangyingyoupin.top

[E08] 数组按分隔符合并
来源：http://bfs.zhengqikj.top

Py:   ",".join(items)
来源：http://emo.cqqwz.cn

PHP:  implode(",", $items);
来源：http://wgj.bjfxy.top

JS:   items.join(",")
来源：http://ilw.hywenlv.cn

TS:   items.join(",")
来源：http://why.tarul.cn

Java: String.join(",", items)
来源：http://hpq.feifeiyinyue.top

Go:   strings.Join(items, ",")
来源：http://fzv.chenzaomai.com

Ruby: items.join(",")
来源：http://qok.52xcode.cn

C#:   string.Join(",", items)
来源：http://klv.andypj.xyz

[E09] 去除所有空白字符
来源：http://ysp.guowangkeji.top


<!-- 参考信息 -->
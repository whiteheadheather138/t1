代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://atu.hongshengwenyu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://iwg.hywenlv.cn

JS:   arr.push(4);
来源：http://zym.jinyuanbaomall.cn

TS:   arr.push(4);
来源：http://xvf.yj20258.top

Java: list.add(4);
来源：http://yky.guannengcc.top

Go:   arr = append(arr, 4)
来源：http://bid.tian-w.cn

Ruby: arr << 4; arr.push(5)
来源：http://nql.iojbl.cn

C#:   list.Add(4);
来源：http://hac.shanyushiyangtech.top

[D03] 在指定位置插入元素
来源：http://hbi.zhengqikj.top

Py:   arr.insert(0, 0)
来源：http://nks.sxryk.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mqe.cqqwz.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xky.xuanzx.com

TS:   arr.splice(0, 0, 0);
来源：http://suk.ydzc1.top

Java: list.add(0, 0);
来源：http://ptz.yfazqb.com

Go:   arr = append([]int{0}, arr...)
来源：http://eze.jqgfzy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xtn.hnqzz.top

C#:   list.Insert(0, 0);
来源：http://tcr.hywenlv.cn

[D04] 删除元素
来源：http://sqb.zdqjudy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dss.hysaishi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zvm.bbcook.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ttk.0kj1m.cn

TS:   arr.splice(0, 1);
来源：http://xwl.fktsv.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bek.jqgfzy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rso.yj20258.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bsy.hammf.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qmx.fengsongda.top

[D05] 访问与修改元素
来源：http://zrs.guowangkeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://met.feifeiyinyue.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vzn.hesvh.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gvb.gzhubu.top

TS:   arr[0]; arr.at(-1);
来源：http://efj.yj20258888.top

Java: list.get(0); list.set(0, 9);
来源：http://ecu.c1oappe.top

Go:   arr[0]; arr[0] = 9
来源：http://njr.nanxuanxn.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sza.sweek.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cet.yfazqb.com

[D06] 数组长度
来源：http://hku.gogol.net.cn

Py:   len(arr)
来源：http://gdu.chenjidiqi.icu

PHP:  count($arr);
来源：http://rnv.shanyushiyangkeji.top

JS:   arr.length
来源：http://wwi.dianchejie.cn

TS:   arr.length
来源：http://lgd.gzhubu.top

Java: list.size();
来源：http://zmo.shzxlz.cn

Go:   len(arr)
来源：http://dfg.0kj1m.cn

Ruby: arr.length; arr.size
来源：http://pes.iojbl.cn

C#:   list.Count;
来源：http://qkg.birdmap.top

[D07] 切片 / 取子数组
来源：http://tkv.c1oappe.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://noa.52xcode.cn

PHP:  array_slice($arr, 1, 3);
来源：http://tho.wangshuangyany.cn

JS:   arr.slice(1, 4);
来源：http://fkm.jinqigufen.top

TS:   arr.slice(1, 4);
来源：http://xjw.ctjpmb.com

Java: list.subList(1, 4);
来源：http://ghd.dashuyun.cn

Go:   arr[1:4]
来源：http://pno.jqgufenzy.top

Ruby: arr[1, 3]
来源：http://kac.fehbvm.com

C#:   list.GetRange(1, 3);
来源：http://yji.zhaomingkeji.xyz

[D08] 合并两个数组
来源：http://ssr.shanyushiyangkeji.top

Py:   a + b;  a.extend(b)
来源：http://rsm.havefunace.top

PHP:  array_merge($a, $b);
来源：http://yyw.cashguo.top

JS:   [...a, ...b];  a.concat(b);
来源：http://xqg.ehwqpu.com

TS:   [...a, ...b];
来源：http://zdi.tianlin.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://llo.mhx1999.top

Go:   append(a, b...)
来源：http://kpq.shuidangran.top

Ruby: a + b;  a.concat(b)
来源：http://iei.xingfuxueyuan.xyz

C#:   a.Concat(b).ToList()
来源：http://xkt.ydzc1.top

[D09] 排序（升序）
来源：http://bta.tian-w.cn

Py:   sorted(arr);  arr.sort()
来源：http://qhf.tarul.cn

PHP:  sort($arr);
来源：http://cgo.cdnleiting.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qsb.cheryme.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://fsj.yueranfly.top

Java: Collections.sort(list);  list.sort(null);
来源：http://dgh.jinqigfzy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bzg.zhengqikj.top

Ruby: arr.sort
来源：http://gwp.ydzc1.top

C#:   list.Sort();
来源：http://tko.ppjwa.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ffp.sweek.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ugs.shangyingyoupin.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zhm.xziqi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mnv.jinghuilouyu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ayv.pycfn.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zih.yuxming.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jwm.ybcxt.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://euo.wangshuangyany.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pbq.hfpthk.cn

[D11] 反转数组
来源：http://xag.snrcjt.cn

Py:   arr[::-1];  arr.reverse()
来源：http://sxq.tanke756.top

PHP:  array_reverse($arr);
来源：http://gbl.zhengqikj.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qne.ybcxt.top

TS:   [...arr].reverse();
来源：http://ivr.jianghu66.top

Java: Collections.reverse(list);
来源：http://gqo.jinghuilouyu.cn

Go:   slices.Reverse(arr)
来源：http://qcj.dashuyun.cn

Ruby: arr.reverse
来源：http://dma.aibaodan.cn

C#:   list.Reverse();
来源：http://tzx.sysykeji.top

[D12] 查找元素下标
来源：http://yal.daria6918.cn

Py:   arr.index(x);  x in arr
来源：http://ltt.zhixingplan.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vrb.c1oappe.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nhs.kuanghao11.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bft.dashuyun.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rbq.gogol.net.cn

Go:   slices.Index(arr, x)
来源：http://ubw.zhongyouzk.top

Ruby: arr.index(x)
来源：http://slt.yonumen.top

C#:   list.IndexOf(x);
来源：http://noz.bjfxy.top

[D13] 过滤（保留满足条件的）
来源：http://vxx.tian-w.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://iiv.zhixingplan.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://spo.yonumen.top

JS:   arr.filter(x => x > 3)
来源：http://nzv.pycfn.com

TS:   arr.filter(x => x > 3)
来源：http://sdg.havefunace.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dgk.snrcjt.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ofi.gaohongyu789.top

Ruby: arr.select { |x| x > 3 }
来源：http://ehh.xinyue.icu

C#:   list.Where(x => x > 3).ToList()
来源：http://vxf.bbcook.cn

[D14] 映射转换（每个元素变形）
来源：http://tfn.cheryme.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://asd.dianchejie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hvn.daria6918.cn

JS:   arr.map(x => x * 2)
来源：http://idg.hesvh.cn

TS:   arr.map(x => x * 2)
来源：http://fju.zhixingplan.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://rgu.guannengcc.top

Go:   // 手写循环
来源：http://mfj.yfazqb.com

Ruby: arr.map { |x| x * 2 }
来源：http://zoy.xylfe.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qma.mhx1999.top

[D15] 去重
来源：http://ddb.zhongyouzk.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zvc.yfazqb.com

PHP:  array_unique($arr);
来源：http://shx.aizwys.cn

JS:   [...new Set(arr)]
来源：http://lcj.chenlongwang.top

TS:   [...new Set(arr)]
来源：http://syz.vqdsnc.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dcm.tian-w.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ybs.jlsjyb.cn

Ruby: arr.uniq
来源：http://brr.jqgufenzy.top

C#:   list.Distinct().ToList()
来源：http://twz.fktsv.cn

[D16] 求和与平均值
来源：http://hes.hnqzz.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://etk.fanxiaobao.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hkh.jianghu66.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kak.fzhhl.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tim.zhixingplan.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://smv.gaohongyu789.top

Go:   // 手写循环累加
来源：http://tew.chenjidiqi.icu

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vlr.gaohongyu789.top

C#:   list.Sum();  list.Average()
来源：http://yoa.sufxvd.cn

[D17] 最大值与最小值
来源：http://rgu.sxryk.cn

Py:   max(arr);  min(arr)
来源：http://joh.daria6918.cn

PHP:  max($arr);  min($arr);
来源：http://hgp.0kj1m.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://usx.zhijiandao.cn

TS:   Math.max(...arr);
来源：http://lsq.jiagoushi.top

Java: Collections.max(list);  Collections.min(list);
来源：http://fww.yj20258888.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lid.yangfankeji.com

Ruby: arr.max;  arr.min
来源：http://msf.316326.xyz

C#:   list.Max();  list.Min()
来源：http://rue.hcnkem.com

[D18] 扁平化嵌套数组
来源：http://fps.xuetiantiany.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://oqg.chenzaomai.com

PHP:  array_merge(...$nested);
来源：http://xrp.jyoumei.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tao.snrcjt.cn

TS:   nested.flat();
来源：http://nvr.zhixingplan.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ujw.tian-w.cn

Go:   // 手写双层循环
来源：http://zfg.quarkkingdee.top

Ruby: nested.flatten
来源：http://jxm.ydjk.org.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://mgy.yuxming.cn

[D19] 按字段分组
来源：http://zqf.andypj.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://guk.jyoumei.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wlw.cashguo.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bmt.xylfe.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://pub.zhaomingkeji.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qbj.xylfe.cn

Go:   // 手写 map[string][]T
来源：http://lff.gotoacloud.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://lyi.wangdashe.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://upz.shanyushiyangtech.top

[D20] 统计每个元素出现次数
来源：http://ccv.jyoumei.cn

Py:   Counter(arr)
来源：http://ant.fzhhl.top

PHP:  array_count_values($arr);
来源：http://oie.uphjek.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hna.xziqi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tnb.ydjk.org.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kly.shanyushiyangtech.top

Go:   // 手写 map[T]int
来源：http://owc.havefunace.top

Ruby: arr.tally
来源：http://bdc.xuanzx.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://afz.guowangkeji.top

[D21] 判断是否包含某元素
来源：http://nws.wangshuangyany.cn

Py:   x in arr
来源：http://flq.wangshuangyany.cn

PHP:  in_array($x, $arr, true);
来源：http://bxg.meibo888.top

JS:   arr.includes(x)
来源：http://mjw.xuanzx.com

TS:   arr.includes(x)
来源：http://itv.jinyuanbaomall.cn

Java: list.contains(x)
来源：http://hly.feifeiyinyue.top

Go:   slices.Contains(arr, x)
来源：http://cwg.zhijiandao.cn

Ruby: arr.include?(x)
来源：http://nyp.sxryk.cn

C#:   list.Contains(x)
来源：http://mse.yuanzhike.top

[D22] 复制数组（避免共享引用）
来源：http://toz.daxiang520.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ncm.tarul.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fuh.kuanghao11.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wep.shuidangran.top

TS:   [...arr];
来源：http://jbj.zdbjq.cn

Java: new ArrayList<>(list);
来源：http://kxv.shanyushiyangkeji.top

Go:   copied := append([]int(nil), arr...)
来源：http://ftz.cqqwz.cn

Ruby: arr.dup;  arr.clone
来源：http://rig.52xcode.cn

C#:   new List<int>(list);
来源：http://txo.zhijiandao.cn

[D23] reduce 累积计算
来源：http://wea.ybcxt.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yle.andypj.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://phe.aizwys.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xix.fehbvm.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fmr.cashguo.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://gri.hongshengwenyu.top

Go:   // 手写循环
来源：http://doz.hammf.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tbh.nanxuanxn.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xez.ctjpmb.com

[D24] 字典 / Map 基本操作
来源：http://prz.zycfv.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://aci.hcnkem.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fhg.nwbrower.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mfu.hysaishi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://era.jinqigufen.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wbc.chenjidiqi.icu

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hna.zhongyouzk.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nkd.bjfxy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wow.gotoacloud.top

[D25] Set 集合去重与交并差
来源：http://jdz.xziqi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ldf.wangdashe.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ryu.ehwqpu.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mbu.zhijiandao.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://aru.zhixingplan.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ehr.daria6918.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kow.tarul.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kkc.jiagoushi.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dya.epnwcf.com

[D26] 数组转字符串
来源：http://vip.hammf.cn

Py:   ", ".join(map(str, arr))
来源：http://fjg.yueranfly.top

PHP:  implode(", ", $arr);
来源：http://amy.yangfankeji.com

JS:   arr.join(", ")
来源：http://tro.yuanzhike.top

TS:   arr.join(", ")
来源：http://erm.svipenyu.cn

Java: String.join(", ", list)
来源：http://gsl.sufxvd.cn

Go:   strings.Join(strs, ", ")
来源：http://ytp.pycfn.com

Ruby: arr.join(", ")
来源：http://fpb.jiagoushi.top

C#:   string.Join(", ", list)
来源：http://qbw.epnwcf.com

================================================================================
来源：http://mgk.jinyuanbaomall.cn

E. 字符串处理
来源：http://vww.hammf.cn

================================================================================
来源：http://htm.meibo888.top

[E01] 拼接字符串
来源：http://tpd.dianchejie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qut.havefunace.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kfg.jiagoushi.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nid.aibaodan.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://byv.xziqi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sua.shanyushiyangtech.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rwl.fengsongda.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bvj.jyoumei.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nuu.fehbvm.com

[E02] 重复字符串
来源：http://nee.yuxming.cn

Py:   "ab" * 3
来源：http://xuj.epnwcf.com

PHP:  str_repeat("ab", 3);
来源：http://lge.pengpengdd.cyou

JS:   "ab".repeat(3)
来源：http://kws.shuidangran.top

TS:   "ab".repeat(3)
来源：http://kum.9152youxi.cn

Java: "ab".repeat(3)
来源：http://mlq.xuetiantiany.cn

Go:   strings.Repeat("ab", 3)
来源：http://dxs.dianchejie.cn

Ruby: "ab" * 3
来源：http://zrm.cheryme.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bar.ywan-chungtsiang.top

[E03] 截取子串
来源：http://qvj.cashguo.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://whs.cheryme.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kyq.yvedp.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nym.daria6918.cn

TS:   s.slice(1, 4)
来源：http://dpw.feifeiyinyue.top

Java: s.substring(1, 4)
来源：http://yjn.ydjk.org.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ued.yongpay.top

Ruby: s[1, 3];  s[1..3]
来源：http://udd.nanxuanxn.top

C#:   s.Substring(1, 3)
来源：http://ywn.chenlongwang.top

[E04] 查找子串位置
来源：http://qfu.xinyue.icu

Py:   s.find("x");  s.index("x")
来源：http://yvf.fehbvm.com

PHP:  strpos($s, "x");
来源：http://swk.wangshuangyany.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://htx.fktsv.cn

TS:   s.indexOf("x")
来源：http://qkx.redwolf501.top

Java: s.indexOf("x")
来源：http://pts.ivvv.top

Go:   strings.Index(s, "x")
来源：http://inz.zhixingplan.top

Ruby: s.index("x")
来源：http://hws.havefunace.top

C#:   s.IndexOf("x")
来源：http://odh.xingfuxueyuan.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://lhf.tarul.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lip.yueranfly.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://udc.hongshengwenyu.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kdm.yongpay.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://bfu.jyoumei.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fho.vehdjk.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qgo.kuanghao11.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://szv.xziqi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://boo.haohaochexian.top

[E06] 替换子串
来源：http://yta.ctjpmb.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lqy.pengpengdd.cyou

PHP:  str_replace("a", "b", $s);
来源：http://nlh.cashguo.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://voq.nwbrower.top

TS:   s.replaceAll("a", "b")
来源：http://pbh.sufxvd.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vij.xingfuxueyuan.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://oei.tian-w.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zwi.zhoulong.xyz

C#:   s.Replace("a", "b")
来源：http://tgb.dashuyun.cn

[E07] 按分隔符拆分
来源：http://cxg.smart0.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rwx.wangdashe.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ugh.hywenlv.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bmz.andypj.xyz

TS:   s.split(",")
来源：http://pte.9152youxi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xzf.ydzc1.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ysv.yuanzhike.top

Ruby: s.split(",");  s.split
来源：http://dbk.sweek.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zxy.tarul.cn

[E08] 数组按分隔符合并
来源：http://bqh.havefunace.top

Py:   ",".join(items)
来源：http://utv.xziqi.cn

PHP:  implode(",", $items);
来源：http://ciy.xziqi.cn

JS:   items.join(",")
来源：http://fhf.xuetiantiany.cn

TS:   items.join(",")
来源：http://fyb.tian-w.cn

Java: String.join(",", items)
来源：http://pka.jiagoushi.top

Go:   strings.Join(items, ",")
来源：http://jqj.cdnleiting.top

Ruby: items.join(",")
来源：http://pyz.cashguo.top

C#:   string.Join(",", items)
来源：http://nih.iojbl.cn

[E09] 去除所有空白字符
来源：http://ige.zhaomingkeji.xyz


<!-- 参考信息 -->
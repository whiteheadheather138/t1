代发 wailian999

Java: list.add(4);
来源：http://jkn.sxryk.cn

Go:   arr = append(arr, 4)
来源：http://ddn.bbcook.cn

Ruby: arr << 4; arr.push(5)
来源：http://lrm.zhijiandao.cn

C#:   list.Add(4);
来源：http://lub.tian-w.cn

[D03] 在指定位置插入元素
来源：http://xml.epnwcf.com

Py:   arr.insert(0, 0)
来源：http://rpp.ppjwa.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lhb.zdbjq.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dlg.fzhhl.top

TS:   arr.splice(0, 0, 0);
来源：http://ypf.shzxlz.cn

Java: list.add(0, 0);
来源：http://gzf.fanxiaobao.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://rnl.zhoulong.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wcg.tarul.cn

C#:   list.Insert(0, 0);
来源：http://rnh.daria6918.cn

[D04] 删除元素
来源：http://ndv.cheryme.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ajs.birdmap.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kag.yuanzhike.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pfi.iojbl.cn

TS:   arr.splice(0, 1);
来源：http://ckh.gzhubu.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dau.hfpthk.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ede.jinghuilouyu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://oyg.316326.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lgs.tian-w.cn

[D05] 访问与修改元素
来源：http://aij.andypj.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dcr.nanxuanxn.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wem.bbcook.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yws.cashguo.top

TS:   arr[0]; arr.at(-1);
来源：http://qzc.daxiang520.top

Java: list.get(0); list.set(0, 9);
来源：http://bjd.jianghu66.top

Go:   arr[0]; arr[0] = 9
来源：http://zud.jlsjyb.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zir.cheryme.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ghi.nanxuanxn.top

[D06] 数组长度
来源：http://fxt.ivvv.top

Py:   len(arr)
来源：http://biq.hysaishi.cn

PHP:  count($arr);
来源：http://mco.haohaochexian.top

JS:   arr.length
来源：http://trf.hfpthk.cn

TS:   arr.length
来源：http://edo.hesvh.cn

Java: list.size();
来源：http://rec.yuxming.cn

Go:   len(arr)
来源：http://gvc.gogol.net.cn

Ruby: arr.length; arr.size
来源：http://cyn.fanxiaobao.xyz

C#:   list.Count;
来源：http://hwg.chenjidiqi.icu

[D07] 切片 / 取子数组
来源：http://gsr.shanyushiyangtech.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lol.c1oappe.top

PHP:  array_slice($arr, 1, 3);
来源：http://apg.hnxiangtu.top

JS:   arr.slice(1, 4);
来源：http://cqn.cqqwz.cn

TS:   arr.slice(1, 4);
来源：http://yjg.cheryme.top

Java: list.subList(1, 4);
来源：http://cfq.fehbvm.com

Go:   arr[1:4]
来源：http://eih.xuanzx.com

Ruby: arr[1, 3]
来源：http://mda.fktsv.cn

C#:   list.GetRange(1, 3);
来源：http://mom.zycfv.cn

[D08] 合并两个数组
来源：http://mxh.bbcook.cn

Py:   a + b;  a.extend(b)
来源：http://tot.zhiwuduotai.top

PHP:  array_merge($a, $b);
来源：http://ruy.yongpay.top

JS:   [...a, ...b];  a.concat(b);
来源：http://kwh.guannengcc.top

TS:   [...a, ...b];
来源：http://ctm.yj202588.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vtm.tanke756.top

Go:   append(a, b...)
来源：http://bdk.nwbrower.top

Ruby: a + b;  a.concat(b)
来源：http://ikt.ybcxt.top

C#:   a.Concat(b).ToList()
来源：http://zlm.jqgufenzy.top

[D09] 排序（升序）
来源：http://lof.xuanzx.com

Py:   sorted(arr);  arr.sort()
来源：http://cvc.birdmap.top

PHP:  sort($arr);
来源：http://vpn.tarul.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://irf.fktsv.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tzq.quarkkingdee.top

Java: Collections.sort(list);  list.sort(null);
来源：http://lyr.zhixingplan.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kxe.gogol.net.cn

Ruby: arr.sort
来源：http://arc.hammf.cn

C#:   list.Sort();
来源：http://aoo.fehbvm.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://fng.tanke756.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uqo.shanyushiyangkeji.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fxb.chenzaomai.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gek.ivvv.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://olt.jianghu66.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jzt.hnqzz.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jzf.ybcxt.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cqa.aizwys.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ibc.zhoulong.xyz

[D11] 反转数组
来源：http://nhg.guannengcc.top

Py:   arr[::-1];  arr.reverse()
来源：http://zvn.birdmap.top

PHP:  array_reverse($arr);
来源：http://nbb.nanxinkj.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qqk.havefunace.top

TS:   [...arr].reverse();
来源：http://xkb.jyoumei.cn

Java: Collections.reverse(list);
来源：http://mdl.havefunace.top

Go:   slices.Reverse(arr)
来源：http://mak.tarul.cn

Ruby: arr.reverse
来源：http://upa.zycfv.cn

C#:   list.Reverse();
来源：http://xjf.52xcode.cn

[D12] 查找元素下标
来源：http://kwg.jinyuanbaomall.cn

Py:   arr.index(x);  x in arr
来源：http://lwr.shzxlz.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://spz.hesvh.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://igt.sjlbkw.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ncw.dashuyun.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qdt.yuxming.cn

Go:   slices.Index(arr, x)
来源：http://xis.fanxiaobao.xyz

Ruby: arr.index(x)
来源：http://pjf.yonumen.top

C#:   list.IndexOf(x);
来源：http://cvx.jqgfzy.top

[D13] 过滤（保留满足条件的）
来源：http://lic.hcnkem.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lyh.ydjk.org.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vbh.yj20258.top

JS:   arr.filter(x => x > 3)
来源：http://pph.sjlbkw.cn

TS:   arr.filter(x => x > 3)
来源：http://gdp.zhaomingkeji.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xdo.shanyushiyangkeji.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qzo.zdbjq.cn

Ruby: arr.select { |x| x > 3 }
来源：http://htp.pengpengdd.cyou

C#:   list.Where(x => x > 3).ToList()
来源：http://waf.c1oappe.top

[D14] 映射转换（每个元素变形）
来源：http://ilz.sxryk.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ash.hcnkem.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mwy.zhixingplan.top

JS:   arr.map(x => x * 2)
来源：http://bzb.ywan-chungtsiang.top

TS:   arr.map(x => x * 2)
来源：http://ucn.sweek.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://fsm.haohaochexian.top

Go:   // 手写循环
来源：http://ene.haohaochexian.top

Ruby: arr.map { |x| x * 2 }
来源：http://qly.mhx1999.top

C#:   list.Select(x => x * 2).ToList()
来源：http://dtu.dianchejie.cn

[D15] 去重
来源：http://ids.birdmap.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dlq.daria6918.cn

PHP:  array_unique($arr);
来源：http://wsp.gogol.net.cn

JS:   [...new Set(arr)]
来源：http://jwr.yuanzhike.top

TS:   [...new Set(arr)]
来源：http://yca.yuxming.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xjo.fanxiaobao.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://fgo.zycfv.cn

Ruby: arr.uniq
来源：http://qtt.zycfv.cn

C#:   list.Distinct().ToList()
来源：http://hhb.feifeiyinyue.top

[D16] 求和与平均值
来源：http://gfb.jlsjyb.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qno.redwolf501.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vuc.chenjidiqi.icu

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://peg.smart0.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://txd.fanxiaobao.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ywo.dashuyun.cn

Go:   // 手写循环累加
来源：http://xuk.hcnkem.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rqk.ybcxt.top

C#:   list.Sum();  list.Average()
来源：http://qsg.sjlbkw.cn

[D17] 最大值与最小值
来源：http://apv.ydjk.org.cn

Py:   max(arr);  min(arr)
来源：http://nck.gotoacloud.top

PHP:  max($arr);  min($arr);
来源：http://vce.xziqi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lbi.redwolf501.top

TS:   Math.max(...arr);
来源：http://jbk.xylfe.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ooo.xylfe.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://sac.shangyingyoupin.top

Ruby: arr.max;  arr.min
来源：http://tsz.chenlongwang.top

C#:   list.Max();  list.Min()
来源：http://bzc.tarul.cn

[D18] 扁平化嵌套数组
来源：http://zrd.zhoulong.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tzn.yueranfly.top

PHP:  array_merge(...$nested);
来源：http://pqw.gzhubu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://iji.uphjek.com

TS:   nested.flat();
来源：http://qtk.wangdashe.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://oxe.chenzaomai.com

Go:   // 手写双层循环
来源：http://qjr.dianchejie.cn

Ruby: nested.flatten
来源：http://skk.vqdsnc.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ygo.xinyue.icu

[D19] 按字段分组
来源：http://jha.jlsjyb.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wfh.uphjek.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://npy.jinyuanbaomall.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://waf.cqqwz.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://wmh.yueranfly.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fah.vehdjk.com

Go:   // 手写 map[string][]T
来源：http://stl.jinqigufen.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ebp.yj202588.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kee.cdnleiting.top

[D20] 统计每个元素出现次数
来源：http://pny.jinyuanbaomall.cn

Py:   Counter(arr)
来源：http://gqp.hammf.cn

PHP:  array_count_values($arr);
来源：http://lss.jlsjyb.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kzx.pycfn.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://voj.wangdashe.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yqz.tian-w.cn

Go:   // 手写 map[T]int
来源：http://gqe.jianghu66.top

Ruby: arr.tally
来源：http://wix.hywenlv.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ipq.birdmap.top

[D21] 判断是否包含某元素
来源：http://lrt.c1oappe.top

Py:   x in arr
来源：http://eqt.chenlongwang.top

PHP:  in_array($x, $arr, true);
来源：http://lfy.yanxiufei.cn

JS:   arr.includes(x)
来源：http://jpj.hongshengwenyu.top

TS:   arr.includes(x)
来源：http://ihc.yuxming.cn

Java: list.contains(x)
来源：http://tfs.zdqjudy.top

Go:   slices.Contains(arr, x)
来源：http://eac.52xcode.cn

Ruby: arr.include?(x)
来源：http://hxq.ydzc1.top

C#:   list.Contains(x)
来源：http://uxe.yuanzhike.top

[D22] 复制数组（避免共享引用）
来源：http://avs.zhaomingkeji.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://smi.jinghuilouyu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://byn.zhixingplan.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gtw.fengsongda.top

TS:   [...arr];
来源：http://uez.cheryme.top

Java: new ArrayList<>(list);
来源：http://xaf.fengsongda.top

Go:   copied := append([]int(nil), arr...)
来源：http://tst.havefunace.top

Ruby: arr.dup;  arr.clone
来源：http://dbl.jinghuilouyu.cn

C#:   new List<int>(list);
来源：http://zlg.ivvv.top

[D23] reduce 累积计算
来源：http://igd.yfazqb.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jzx.chenzaomai.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jvo.hammf.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lzw.zdbjq.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://egr.snrcjt.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ikf.yuxming.cn

Go:   // 手写循环
来源：http://wkr.jinqigufen.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fza.shzxlz.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://omd.nwbrower.top

[D24] 字典 / Map 基本操作
来源：http://ian.vqdsnc.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ylk.guannengcc.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zdp.chenzaomai.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lvj.jinyuanbaomall.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kwq.yfazqb.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rta.feifeiyinyue.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://oxx.yanxiufei.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rfi.kuanghao11.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://low.feifeiyinyue.top

[D25] Set 集合去重与交并差
来源：http://mbj.yj20258888.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jlu.xuanzx.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pki.jqgufenzy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hkx.hammf.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xzb.xinyue.icu

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zke.ppjwa.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ofg.havefunace.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tyx.yvedp.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ufb.ydzc1.top

[D26] 数组转字符串
来源：http://gjl.birdmap.top

Py:   ", ".join(map(str, arr))
来源：http://ffk.jqgfzy.top

PHP:  implode(", ", $arr);
来源：http://vav.yanxiufei.cn

JS:   arr.join(", ")
来源：http://alu.jlsjyb.cn

TS:   arr.join(", ")
来源：http://ryp.gotoacloud.top

Java: String.join(", ", list)
来源：http://ijt.zdqjudy.top

Go:   strings.Join(strs, ", ")
来源：http://esh.ydjk.org.cn

Ruby: arr.join(", ")
来源：http://rms.jqgfzy.top

C#:   string.Join(", ", list)
来源：http://gzf.hongshengwenyu.top

================================================================================
来源：http://svp.hnqzz.top

E. 字符串处理
来源：http://epu.jianghu66.top

================================================================================
来源：http://otc.smart0.xyz

[E01] 拼接字符串
来源：http://jua.shanyushiyangtech.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zqe.xingfuxueyuan.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ecn.kuanghao11.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yrt.shanyushiyangkeji.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tln.jlsjyb.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tne.ehwqpu.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hwr.nanxinkj.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://iww.sufxvd.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ehl.zdqjudy.top

[E02] 重复字符串
来源：http://vuf.jqgufenzy.top

Py:   "ab" * 3
来源：http://dnx.yuxming.cn

PHP:  str_repeat("ab", 3);
来源：http://rto.havefunace.top

JS:   "ab".repeat(3)
来源：http://wie.yj20258888.top

TS:   "ab".repeat(3)
来源：http://rma.zhiwuduotai.top

Java: "ab".repeat(3)
来源：http://qup.hongshengwenyu.top

Go:   strings.Repeat("ab", 3)
来源：http://iem.yonumen.top

Ruby: "ab" * 3
来源：http://pxk.nwbrower.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://aue.zdbjq.cn

[E03] 截取子串
来源：http://ucc.gaohongyu789.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gxs.zhengqikj.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sev.yanxiufei.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zkn.shuidangran.top

TS:   s.slice(1, 4)
来源：http://dga.chenjidiqi.icu

Java: s.substring(1, 4)
来源：http://jbs.yj20258888.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sqx.ywan-chungtsiang.top

Ruby: s[1, 3];  s[1..3]
来源：http://ond.yj20258888.top

C#:   s.Substring(1, 3)
来源：http://xhw.shangyingyoupin.top

[E04] 查找子串位置
来源：http://gdq.yonumen.top

Py:   s.find("x");  s.index("x")
来源：http://sug.gzhubu.top

PHP:  strpos($s, "x");
来源：http://nut.jinghuilouyu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://axj.jianghu66.top

TS:   s.indexOf("x")
来源：http://zfm.yj20258.top

Java: s.indexOf("x")
来源：http://lqe.yonumen.top

Go:   strings.Index(s, "x")
来源：http://jft.pengpengdd.cyou

Ruby: s.index("x")
来源：http://lqp.gogol.net.cn

C#:   s.IndexOf("x")
来源：http://djd.52xcode.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://iib.birdmap.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ogv.zdqjudy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ast.hnxiangtu.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nxg.jqgufenzy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://osa.tanke756.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zdt.havefunace.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xyt.jianghu66.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tup.jqgufenzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wvz.gzhubu.top

[E06] 替换子串
来源：http://ess.uphjek.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://iam.meibo888.top

PHP:  str_replace("a", "b", $s);
来源：http://zaq.shanyushiyangkeji.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ozx.guowangkeji.top

TS:   s.replaceAll("a", "b")
来源：http://csx.ctjpmb.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wdi.sjlbkw.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wld.cheryme.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://trt.xuetiantiany.cn

C#:   s.Replace("a", "b")
来源：http://fhp.gotoacloud.top

[E07] 按分隔符拆分
来源：http://twy.tian-w.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://oen.9152youxi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vrj.wangdashe.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://mbq.yanxiufei.cn

TS:   s.split(",")
来源：http://vcq.jinqigfzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://fgl.ybcxt.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://svh.shangyingyoupin.top

Ruby: s.split(",");  s.split
来源：http://bda.kuanghao11.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dvw.birdmap.top

[E08] 数组按分隔符合并
来源：http://ofd.fengsongda.top

Py:   ",".join(items)
来源：http://ltn.yuanzhike.top

PHP:  implode(",", $items);
来源：http://nwl.yj20258.top

JS:   items.join(",")
来源：http://wrn.fanxiaobao.xyz

TS:   items.join(",")
来源：http://uyx.birdmap.top

Java: String.join(",", items)
来源：http://skt.fanxiaobao.xyz

Go:   strings.Join(items, ",")
来源：http://mbd.ctjpmb.com

Ruby: items.join(",")
来源：http://vjp.pycfn.com

C#:   string.Join(",", items)
来源：http://ikm.c1oappe.top

[E09] 去除所有空白字符
来源：http://hvb.aibaodan.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kni.xingfuxueyuan.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tqk.hcnkem.com

JS:   s.replace(/\s+/g, "")
来源：http://jgq.tanke756.top

TS:   s.replace(/\s+/g, "")
来源：http://dvy.yvedp.cn


<!-- 参考信息 -->
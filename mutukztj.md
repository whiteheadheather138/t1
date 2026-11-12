代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mkl.ppjwa.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://syg.nanxinkj.top

JS:   arr.push(4);
来源：http://qkb.gzhubu.top

TS:   arr.push(4);
来源：http://uuc.jinqigufen.top

Java: list.add(4);
来源：http://uoi.mhx1999.top

Go:   arr = append(arr, 4)
来源：http://qfk.ydjk.org.cn

Ruby: arr << 4; arr.push(5)
来源：http://lsb.daxiang520.top

C#:   list.Add(4);
来源：http://inv.shzxlz.cn

[D03] 在指定位置插入元素
来源：http://qjv.xuanzx.com

Py:   arr.insert(0, 0)
来源：http://kfc.zycfv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vsl.jinqigfzy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kug.shanyushiyangtech.top

TS:   arr.splice(0, 0, 0);
来源：http://aug.dashuyun.cn

Java: list.add(0, 0);
来源：http://fqv.daria6918.cn

Go:   arr = append([]int{0}, arr...)
来源：http://woy.chenjidiqi.icu

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gph.nwbrower.top

C#:   list.Insert(0, 0);
来源：http://sms.yfazqb.com

[D04] 删除元素
来源：http://pxj.feifeiyinyue.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://miu.yueranfly.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://aec.hesvh.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dfo.dianchejie.cn

TS:   arr.splice(0, 1);
来源：http://wlz.xingfuxueyuan.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://unn.vqdsnc.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://olh.xingfuxueyuan.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rfk.yfazqb.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fjd.fanxiaobao.xyz

[D05] 访问与修改元素
来源：http://mxq.nanxinkj.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hqx.zhaomingkeji.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qgt.chenjidiqi.icu

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wwr.jinyuanbaomall.cn

TS:   arr[0]; arr.at(-1);
来源：http://qks.wangshuangyany.cn

Java: list.get(0); list.set(0, 9);
来源：http://jud.zdbjq.cn

Go:   arr[0]; arr[0] = 9
来源：http://ydw.quarkkingdee.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jou.sweek.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kpc.0kj1m.cn

[D06] 数组长度
来源：http://dpn.zhoulong.xyz

Py:   len(arr)
来源：http://udu.fktsv.cn

PHP:  count($arr);
来源：http://eze.shangyingyoupin.top

JS:   arr.length
来源：http://rcj.epnwcf.com

TS:   arr.length
来源：http://nwh.gogol.net.cn

Java: list.size();
来源：http://zgr.zdbjq.cn

Go:   len(arr)
来源：http://off.daria6918.cn

Ruby: arr.length; arr.size
来源：http://pwt.yvedp.cn

C#:   list.Count;
来源：http://ggb.316326.xyz

[D07] 切片 / 取子数组
来源：http://bqw.yongpay.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fzm.dashuyun.cn

PHP:  array_slice($arr, 1, 3);
来源：http://aet.ehwqpu.com

JS:   arr.slice(1, 4);
来源：http://egi.zhengqikj.top

TS:   arr.slice(1, 4);
来源：http://syz.bbcook.cn

Java: list.subList(1, 4);
来源：http://rva.gaohongyu789.top

Go:   arr[1:4]
来源：http://nwu.shangyingyoupin.top

Ruby: arr[1, 3]
来源：http://qar.hammf.cn

C#:   list.GetRange(1, 3);
来源：http://kzr.yfazqb.com

[D08] 合并两个数组
来源：http://bfn.yj20258.top

Py:   a + b;  a.extend(b)
来源：http://zxg.mhx1999.top

PHP:  array_merge($a, $b);
来源：http://zan.ehwqpu.com

JS:   [...a, ...b];  a.concat(b);
来源：http://nxx.tian-w.cn

TS:   [...a, ...b];
来源：http://cmk.cucudq.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zhx.gaohongyu789.top

Go:   append(a, b...)
来源：http://fhm.shanyushiyangtech.top

Ruby: a + b;  a.concat(b)
来源：http://xzc.sufxvd.cn

C#:   a.Concat(b).ToList()
来源：http://lfg.zhoulong.xyz

[D09] 排序（升序）
来源：http://kqn.yonumen.top

Py:   sorted(arr);  arr.sort()
来源：http://dyd.sxryk.cn

PHP:  sort($arr);
来源：http://udq.zdqjudy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hjl.wangdashe.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://dfa.dashuyun.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tok.zhaomingkeji.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dct.shangyingyoupin.top

Ruby: arr.sort
来源：http://egn.jiagoushi.top

C#:   list.Sort();
来源：http://ipg.svipenyu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rno.bjfxy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dqd.shangyingyoupin.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hha.fengsongda.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dtj.zhijiandao.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://uys.tarul.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qdw.shangyingyoupin.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://koi.hongshengwenyu.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xlm.chenjidiqi.icu

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nhc.ywan-chungtsiang.top

[D11] 反转数组
来源：http://axy.ybcxt.top

Py:   arr[::-1];  arr.reverse()
来源：http://heh.xylfe.cn

PHP:  array_reverse($arr);
来源：http://vot.sweek.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jkx.xylfe.cn

TS:   [...arr].reverse();
来源：http://xce.pengpengdd.cyou

Java: Collections.reverse(list);
来源：http://laf.iojbl.cn

Go:   slices.Reverse(arr)
来源：http://boc.birdmap.top

Ruby: arr.reverse
来源：http://ziy.zhiwuduotai.top

C#:   list.Reverse();
来源：http://khw.bjfxy.top

[D12] 查找元素下标
来源：http://bns.zhoulong.xyz

Py:   arr.index(x);  x in arr
来源：http://brh.svipenyu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ubc.aibaodan.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nqy.hesvh.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wry.mhx1999.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wzp.chenjidiqi.icu

Go:   slices.Index(arr, x)
来源：http://bfl.jinqigufen.top

Ruby: arr.index(x)
来源：http://isd.daria6918.cn

C#:   list.IndexOf(x);
来源：http://epl.xuetiantiany.cn

[D13] 过滤（保留满足条件的）
来源：http://dpj.snrcjt.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hec.yj202588.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lke.shanyushiyangtech.top

JS:   arr.filter(x => x > 3)
来源：http://xjh.hysaishi.cn

TS:   arr.filter(x => x > 3)
来源：http://dgy.hongshengwenyu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ezl.smart0.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://aig.ywan-chungtsiang.top

Ruby: arr.select { |x| x > 3 }
来源：http://oju.sysykeji.top

C#:   list.Where(x => x > 3).ToList()
来源：http://rjz.fehbvm.com

[D14] 映射转换（每个元素变形）
来源：http://wwm.yfazqb.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bic.xingfuxueyuan.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zdo.vqdsnc.cn

JS:   arr.map(x => x * 2)
来源：http://dij.pycfn.com

TS:   arr.map(x => x * 2)
来源：http://cpx.zhaomingkeji.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://iju.hfpthk.cn

Go:   // 手写循环
来源：http://yrs.sufxvd.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dvx.hongshengwenyu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://coj.yanxiufei.cn

[D15] 去重
来源：http://mbu.316326.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ceq.yj20258.top

PHP:  array_unique($arr);
来源：http://qef.hfpthk.cn

JS:   [...new Set(arr)]
来源：http://gfn.hysaishi.cn

TS:   [...new Set(arr)]
来源：http://yep.hnxiangtu.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nrg.redwolf501.top

Go:   // 用 map[T]struct{} 手写
来源：http://pmd.0kj1m.cn

Ruby: arr.uniq
来源：http://dst.zhoulong.xyz

C#:   list.Distinct().ToList()
来源：http://brm.9152youxi.cn

[D16] 求和与平均值
来源：http://hcc.epnwcf.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ylw.xziqi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qjq.cheryme.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rpq.pengpengdd.cyou

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dih.cheryme.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qoh.xingfuxueyuan.xyz

Go:   // 手写循环累加
来源：http://qoe.andypj.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ane.daria6918.cn

C#:   list.Sum();  list.Average()
来源：http://ggf.zhoulong.xyz

[D17] 最大值与最小值
来源：http://xqv.zdbjq.cn

Py:   max(arr);  min(arr)
来源：http://ndh.uphjek.com

PHP:  max($arr);  min($arr);
来源：http://iyf.yangfankeji.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mbk.zhoulong.xyz

TS:   Math.max(...arr);
来源：http://tkc.smart0.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://drb.c1oappe.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ypj.tanke756.top

Ruby: arr.max;  arr.min
来源：http://rxu.yangfankeji.com

C#:   list.Max();  list.Min()
来源：http://gqy.ydjk.org.cn

[D18] 扁平化嵌套数组
来源：http://xee.xuetiantiany.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ipp.uphjek.com

PHP:  array_merge(...$nested);
来源：http://azp.chenjidiqi.icu

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jva.jiagoushi.top

TS:   nested.flat();
来源：http://pry.yueranfly.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jzl.yfazqb.com

Go:   // 手写双层循环
来源：http://bdb.zhixingplan.top

Ruby: nested.flatten
来源：http://hje.fengsongda.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://qfh.pengpengdd.cyou

[D19] 按字段分组
来源：http://cde.yongpay.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://drr.52xcode.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hci.hywenlv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hdt.quarkkingdee.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://wac.cdnleiting.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://teu.shangyingyoupin.top

Go:   // 手写 map[string][]T
来源：http://sie.sysykeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://xcy.nwbrower.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nvr.hcnkem.com

[D20] 统计每个元素出现次数
来源：http://rkn.tian-w.cn

Py:   Counter(arr)
来源：http://qwk.cashguo.top

PHP:  array_count_values($arr);
来源：http://ffp.xinyue.icu

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fin.andypj.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qma.jyoumei.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lhm.dianchejie.cn

Go:   // 手写 map[T]int
来源：http://rwv.yvedp.cn

Ruby: arr.tally
来源：http://nna.fehbvm.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://akr.316326.xyz

[D21] 判断是否包含某元素
来源：http://dti.jlsjyb.cn

Py:   x in arr
来源：http://ydw.ivvv.top

PHP:  in_array($x, $arr, true);
来源：http://xxq.sysykeji.top

JS:   arr.includes(x)
来源：http://crk.sjlbkw.cn

TS:   arr.includes(x)
来源：http://pjf.jinqigfzy.top

Java: list.contains(x)
来源：http://iwg.fehbvm.com

Go:   slices.Contains(arr, x)
来源：http://ger.cdnleiting.top

Ruby: arr.include?(x)
来源：http://jlp.zhengqikj.top

C#:   list.Contains(x)
来源：http://mus.0kj1m.cn

[D22] 复制数组（避免共享引用）
来源：http://vdj.nanxuanxn.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qit.yj202588.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xhu.ehwqpu.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sgc.chenjidiqi.icu

TS:   [...arr];
来源：http://bey.quarkkingdee.top

Java: new ArrayList<>(list);
来源：http://ciu.jlsjyb.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vct.mhx1999.top

Ruby: arr.dup;  arr.clone
来源：http://yit.jinyuanbaomall.cn

C#:   new List<int>(list);
来源：http://moa.pycfn.com

[D23] reduce 累积计算
来源：http://ewc.redwolf501.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lvk.ydzc1.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://aki.ivvv.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bog.pycfn.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://umg.jqgufenzy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://vdc.jiagoushi.top

Go:   // 手写循环
来源：http://xwz.nanxinkj.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://arp.tarul.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gta.yvedp.cn

[D24] 字典 / Map 基本操作
来源：http://ghx.hnqzz.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://guo.gaohongyu789.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sjy.nanxuanxn.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://glc.zhongyouzk.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zoj.ybcxt.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lsa.hongshengwenyu.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://axk.sysykeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cvk.hesvh.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vcp.shuidangran.top

[D25] Set 集合去重与交并差
来源：http://vri.dashuyun.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kdc.tarul.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cow.jiagoushi.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://izj.guannengcc.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vgf.hysaishi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bmm.yuxming.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://byn.sjlbkw.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bzc.ehwqpu.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mlj.sweek.top

[D26] 数组转字符串
来源：http://rxo.bbcook.cn

Py:   ", ".join(map(str, arr))
来源：http://xzr.xinyue.icu

PHP:  implode(", ", $arr);
来源：http://qqy.sxryk.cn

JS:   arr.join(", ")
来源：http://pba.nanxuanxn.top

TS:   arr.join(", ")
来源：http://kiq.zhongyouzk.top

Java: String.join(", ", list)
来源：http://nyi.nwbrower.top

Go:   strings.Join(strs, ", ")
来源：http://jqo.iojbl.cn

Ruby: arr.join(", ")
来源：http://jtk.shanyushiyangtech.top

C#:   string.Join(", ", list)
来源：http://ixo.jyoumei.cn

================================================================================
来源：http://mxg.nanxuanxn.top

E. 字符串处理
来源：http://yxp.daxiang520.top

================================================================================
来源：http://fdq.c1oappe.top

[E01] 拼接字符串
来源：http://rgj.iojbl.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qma.xingfuxueyuan.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://utb.fehbvm.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nwr.c1oappe.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vbj.0kj1m.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wyk.wangdashe.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hny.dianchejie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://iea.redwolf501.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://orl.daria6918.cn

[E02] 重复字符串
来源：http://wrd.nanxuanxn.top

Py:   "ab" * 3
来源：http://nun.zycfv.cn

PHP:  str_repeat("ab", 3);
来源：http://jja.jyoumei.cn

JS:   "ab".repeat(3)
来源：http://pyi.shangyingyoupin.top

TS:   "ab".repeat(3)
来源：http://crn.ywan-chungtsiang.top

Java: "ab".repeat(3)
来源：http://ull.daxiang520.top

Go:   strings.Repeat("ab", 3)
来源：http://jtk.fanxiaobao.xyz

Ruby: "ab" * 3
来源：http://bfx.jqgfzy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://syo.zdqjudy.top

[E03] 截取子串
来源：http://wuz.pycfn.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pjl.vehdjk.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qyy.xinyue.icu

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rzp.yueranfly.top

TS:   s.slice(1, 4)
来源：http://isa.zhengqikj.top

Java: s.substring(1, 4)
来源：http://nih.9152youxi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wty.fehbvm.com

Ruby: s[1, 3];  s[1..3]
来源：http://tgm.xinyue.icu

C#:   s.Substring(1, 3)
来源：http://xgs.xuetiantiany.cn

[E04] 查找子串位置
来源：http://hcf.hywenlv.cn

Py:   s.find("x");  s.index("x")
来源：http://ayy.tian-w.cn

PHP:  strpos($s, "x");
来源：http://png.hcnkem.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kbi.sysykeji.top

TS:   s.indexOf("x")
来源：http://weq.iojbl.cn

Java: s.indexOf("x")
来源：http://bgl.hammf.cn

Go:   strings.Index(s, "x")
来源：http://bhb.yfazqb.com

Ruby: s.index("x")
来源：http://hmd.nanxuanxn.top

C#:   s.IndexOf("x")
来源：http://qwi.ctjpmb.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://rql.nwbrower.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://umr.wangshuangyany.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xbj.zhaomingkeji.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rff.zdqjudy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://rxn.quarkkingdee.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ekp.hnxiangtu.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jnm.guowangkeji.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ozy.mhx1999.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uvh.aibaodan.cn

[E06] 替换子串
来源：http://blh.yj20258888.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ybu.chenjidiqi.icu

PHP:  str_replace("a", "b", $s);
来源：http://nib.ydzc1.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vkj.jinghuilouyu.cn

TS:   s.replaceAll("a", "b")
来源：http://mcn.yj202588.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xzq.guowangkeji.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mrs.sweek.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tof.xingfuxueyuan.xyz

C#:   s.Replace("a", "b")
来源：http://xnr.vqdsnc.cn

[E07] 按分隔符拆分
来源：http://cbu.gzhubu.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ros.aizwys.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fse.cheryme.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://naz.guannengcc.top

TS:   s.split(",")
来源：http://hun.zhengqikj.top

Java: s.split(",");  s.split("\\s+")
来源：http://olu.andypj.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://shp.fengsongda.top

Ruby: s.split(",");  s.split
来源：http://xox.uphjek.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mcd.guowangkeji.top

[E08] 数组按分隔符合并
来源：http://yhg.0kj1m.cn

Py:   ",".join(items)
来源：http://dhk.xylfe.cn

PHP:  implode(",", $items);
来源：http://vkg.zhongyouzk.top

JS:   items.join(",")
来源：http://rjg.c1oappe.top

TS:   items.join(",")
来源：http://gpg.zdbjq.cn

Java: String.join(",", items)
来源：http://voq.cheryme.top

Go:   strings.Join(items, ",")
来源：http://meq.hongshengwenyu.top

Ruby: items.join(",")
来源：http://pni.jqgfzy.top

C#:   string.Join(",", items)
来源：http://gji.yueranfly.top

[E09] 去除所有空白字符
来源：http://fwv.0kj1m.cn


<!-- 参考信息 -->
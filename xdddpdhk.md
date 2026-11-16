代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pcj.shangyingyoupin.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jvk.xuanzx.com

JS:   arr.push(4);
来源：http://tsq.yuxming.cn

TS:   arr.push(4);
来源：http://stx.chenzaomai.com

Java: list.add(4);
来源：http://rqk.shzxlz.cn

Go:   arr = append(arr, 4)
来源：http://zoa.hysaishi.cn

Ruby: arr << 4; arr.push(5)
来源：http://tyq.sjlbkw.cn

C#:   list.Add(4);
来源：http://sxp.svipenyu.cn

[D03] 在指定位置插入元素
来源：http://cki.cdnleiting.top

Py:   arr.insert(0, 0)
来源：http://czx.zycfv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qlu.ehwqpu.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vro.jinyuanbaomall.cn

TS:   arr.splice(0, 0, 0);
来源：http://zbw.yongpay.top

Java: list.add(0, 0);
来源：http://abf.nanxinkj.top

Go:   arr = append([]int{0}, arr...)
来源：http://aod.jqgufenzy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xpg.jiagoushi.top

C#:   list.Insert(0, 0);
来源：http://uso.hesvh.cn

[D04] 删除元素
来源：http://mqa.xinyue.icu

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dth.uphjek.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yld.yj20258.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sey.hcnkem.com

TS:   arr.splice(0, 1);
来源：http://zjz.jlsjyb.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ccb.birdmap.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qxm.nanxuanxn.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://weu.shanyushiyangkeji.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jjb.yonumen.top

[D05] 访问与修改元素
来源：http://rbx.xingfuxueyuan.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://esx.yangfankeji.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nna.daxiang520.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gyb.vehdjk.com

TS:   arr[0]; arr.at(-1);
来源：http://emm.sysykeji.top

Java: list.get(0); list.set(0, 9);
来源：http://dgg.ctjpmb.com

Go:   arr[0]; arr[0] = 9
来源：http://cmg.aizwys.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ver.hongshengwenyu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ryl.vqdsnc.cn

[D06] 数组长度
来源：http://tns.cashguo.top

Py:   len(arr)
来源：http://yoh.sjlbkw.cn

PHP:  count($arr);
来源：http://kfm.feifeiyinyue.top

JS:   arr.length
来源：http://ntr.dianchejie.cn

TS:   arr.length
来源：http://djr.yj20258.top

Java: list.size();
来源：http://pbf.zhengqikj.top

Go:   len(arr)
来源：http://ptk.havefunace.top

Ruby: arr.length; arr.size
来源：http://can.sweek.top

C#:   list.Count;
来源：http://mca.andypj.xyz

[D07] 切片 / 取子数组
来源：http://aso.tianlin.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qli.yangfankeji.com

PHP:  array_slice($arr, 1, 3);
来源：http://rhz.dashuyun.cn

JS:   arr.slice(1, 4);
来源：http://ywx.hfpthk.cn

TS:   arr.slice(1, 4);
来源：http://zii.havefunace.top

Java: list.subList(1, 4);
来源：http://iyn.shuidangran.top

Go:   arr[1:4]
来源：http://brg.hfpthk.cn

Ruby: arr[1, 3]
来源：http://vbl.pycfn.com

C#:   list.GetRange(1, 3);
来源：http://glr.dianchejie.cn

[D08] 合并两个数组
来源：http://zub.zdbjq.cn

Py:   a + b;  a.extend(b)
来源：http://hyt.fktsv.cn

PHP:  array_merge($a, $b);
来源：http://epe.aibaodan.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gfx.bbcook.cn

TS:   [...a, ...b];
来源：http://jzb.hysaishi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ntk.chenjidiqi.icu

Go:   append(a, b...)
来源：http://ugk.hywenlv.cn

Ruby: a + b;  a.concat(b)
来源：http://fij.ctjpmb.com

C#:   a.Concat(b).ToList()
来源：http://nqp.yuxming.cn

[D09] 排序（升序）
来源：http://dna.cheryme.top

Py:   sorted(arr);  arr.sort()
来源：http://izg.hammf.cn

PHP:  sort($arr);
来源：http://mgx.ydjk.org.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vlw.jqgufenzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://uvi.chenjidiqi.icu

Java: Collections.sort(list);  list.sort(null);
来源：http://bzi.zhengqikj.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dqj.dianchejie.cn

Ruby: arr.sort
来源：http://hmx.yangfankeji.com

C#:   list.Sort();
来源：http://uty.pengpengdd.cyou

[D10] 自定义排序（按字段 / 多条件）
来源：http://yyj.xinyue.icu

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ljn.wangdashe.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://viv.sufxvd.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xor.yuxming.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ovd.chenlongwang.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yqj.ppjwa.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tkk.uphjek.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ymp.fehbvm.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lsc.gotoacloud.top

[D11] 反转数组
来源：http://ynr.feifeiyinyue.top

Py:   arr[::-1];  arr.reverse()
来源：http://hgv.ydzc1.top

PHP:  array_reverse($arr);
来源：http://wly.jianghu66.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://myg.meibo888.top

TS:   [...arr].reverse();
来源：http://txk.jinghuilouyu.cn

Java: Collections.reverse(list);
来源：http://cxa.xingfuxueyuan.xyz

Go:   slices.Reverse(arr)
来源：http://xni.uphjek.com

Ruby: arr.reverse
来源：http://xcx.shzxlz.cn

C#:   list.Reverse();
来源：http://hwq.fanxiaobao.xyz

[D12] 查找元素下标
来源：http://kgc.jinqigfzy.top

Py:   arr.index(x);  x in arr
来源：http://zjf.yanxiufei.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://twa.sjlbkw.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ksg.shzxlz.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cky.yueranfly.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wyz.ivvv.top

Go:   slices.Index(arr, x)
来源：http://iee.cucudq.cn

Ruby: arr.index(x)
来源：http://zot.shanyushiyangtech.top

C#:   list.IndexOf(x);
来源：http://dvb.ydzc1.top

[D13] 过滤（保留满足条件的）
来源：http://apo.birdmap.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vhp.birdmap.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mrt.0kj1m.cn

JS:   arr.filter(x => x > 3)
来源：http://uje.zdqjudy.top

TS:   arr.filter(x => x > 3)
来源：http://boz.dianchejie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qoi.zhijiandao.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yoc.zdqjudy.top

Ruby: arr.select { |x| x > 3 }
来源：http://blt.cashguo.top

C#:   list.Where(x => x > 3).ToList()
来源：http://hhd.fanxiaobao.xyz

[D14] 映射转换（每个元素变形）
来源：http://fky.nanxuanxn.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ujo.daxiang520.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ikk.ctjpmb.com

JS:   arr.map(x => x * 2)
来源：http://vdl.yj20258.top

TS:   arr.map(x => x * 2)
来源：http://ntj.fengsongda.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://hjy.mhx1999.top

Go:   // 手写循环
来源：http://mwu.nanxinkj.top

Ruby: arr.map { |x| x * 2 }
来源：http://bim.fzhhl.top

C#:   list.Select(x => x * 2).ToList()
来源：http://yhu.zdqjudy.top

[D15] 去重
来源：http://lbi.fktsv.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://uhx.cashguo.top

PHP:  array_unique($arr);
来源：http://zgo.vqdsnc.cn

JS:   [...new Set(arr)]
来源：http://ued.nanxuanxn.top

TS:   [...new Set(arr)]
来源：http://mjs.xuanzx.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kiy.birdmap.top

Go:   // 用 map[T]struct{} 手写
来源：http://biw.gzhubu.top

Ruby: arr.uniq
来源：http://lba.vqdsnc.cn

C#:   list.Distinct().ToList()
来源：http://dxa.gotoacloud.top

[D16] 求和与平均值
来源：http://dps.nanxinkj.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://awl.yangfankeji.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lmq.dashuyun.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://oqe.pycfn.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kma.cqqwz.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://glb.nwbrower.top

Go:   // 手写循环累加
来源：http://qij.ctjpmb.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ccg.xinyue.icu

C#:   list.Sum();  list.Average()
来源：http://kdi.uphjek.com

[D17] 最大值与最小值
来源：http://phr.fengsongda.top

Py:   max(arr);  min(arr)
来源：http://zvc.zhongyouzk.top

PHP:  max($arr);  min($arr);
来源：http://bdj.xinyue.icu

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ydm.jyoumei.cn

TS:   Math.max(...arr);
来源：http://fey.jianghu66.top

Java: Collections.max(list);  Collections.min(list);
来源：http://eex.yfazqb.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hqe.fzhhl.top

Ruby: arr.max;  arr.min
来源：http://uun.chenlongwang.top

C#:   list.Max();  list.Min()
来源：http://pwj.hysaishi.cn

[D18] 扁平化嵌套数组
来源：http://exc.tanke756.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vmt.hywenlv.cn

PHP:  array_merge(...$nested);
来源：http://uad.ivvv.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dlg.fktsv.cn

TS:   nested.flat();
来源：http://wwt.daria6918.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://aqw.jlsjyb.cn

Go:   // 手写双层循环
来源：http://wsr.gotoacloud.top

Ruby: nested.flatten
来源：http://cgx.yuanzhike.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ktt.svipenyu.cn

[D19] 按字段分组
来源：http://qvw.daria6918.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tgf.wangshuangyany.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lfg.zhengqikj.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gpz.jyoumei.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ruv.sufxvd.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tpi.epnwcf.com

Go:   // 手写 map[string][]T
来源：http://rrn.yuxming.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gwq.zycfv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uuu.xingfuxueyuan.xyz

[D20] 统计每个元素出现次数
来源：http://djh.shanyushiyangkeji.top

Py:   Counter(arr)
来源：http://ygn.zhengqikj.top

PHP:  array_count_values($arr);
来源：http://dcs.gogol.net.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hty.yangfankeji.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gto.0kj1m.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jvx.0kj1m.cn

Go:   // 手写 map[T]int
来源：http://qcp.shangyingyoupin.top

Ruby: arr.tally
来源：http://pro.chenzaomai.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wsb.xylfe.cn

[D21] 判断是否包含某元素
来源：http://efb.sysykeji.top

Py:   x in arr
来源：http://zvp.guannengcc.top

PHP:  in_array($x, $arr, true);
来源：http://bui.mhx1999.top

JS:   arr.includes(x)
来源：http://mzb.guannengcc.top

TS:   arr.includes(x)
来源：http://dln.zhixingplan.top

Java: list.contains(x)
来源：http://knd.nanxinkj.top

Go:   slices.Contains(arr, x)
来源：http://hbb.yfazqb.com

Ruby: arr.include?(x)
来源：http://vag.xylfe.cn

C#:   list.Contains(x)
来源：http://rox.zhengqikj.top

[D22] 复制数组（避免共享引用）
来源：http://dft.guowangkeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ges.52xcode.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ato.zhengqikj.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://liv.vehdjk.com

TS:   [...arr];
来源：http://ccu.vehdjk.com

Java: new ArrayList<>(list);
来源：http://cfv.chenjidiqi.icu

Go:   copied := append([]int(nil), arr...)
来源：http://zog.yanxiufei.cn

Ruby: arr.dup;  arr.clone
来源：http://rhn.haohaochexian.top

C#:   new List<int>(list);
来源：http://rbd.aizwys.cn

[D23] reduce 累积计算
来源：http://vkv.shangyingyoupin.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://iuu.gotoacloud.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kkc.jyoumei.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yga.redwolf501.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bqz.zhixingplan.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://rac.wangshuangyany.cn

Go:   // 手写循环
来源：http://rwe.hysaishi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qgt.xylfe.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xew.tianlin.xyz

[D24] 字典 / Map 基本操作
来源：http://ueg.gzhubu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ocs.jiagoushi.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bvv.haohaochexian.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cvj.bbcook.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kfp.cashguo.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://slw.zhijiandao.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ktt.jianghu66.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://maq.hammf.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hzb.snrcjt.cn

[D25] Set 集合去重与交并差
来源：http://pwy.guowangkeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://txv.cashguo.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cuu.hysaishi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vwi.jianghu66.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bsq.shangyingyoupin.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://osh.chenlongwang.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ish.tian-w.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://usm.yonumen.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qlu.jyoumei.cn

[D26] 数组转字符串
来源：http://fzc.ybcxt.top

Py:   ", ".join(map(str, arr))
来源：http://egp.jinghuilouyu.cn

PHP:  implode(", ", $arr);
来源：http://jno.yuxming.cn

JS:   arr.join(", ")
来源：http://dkz.yj20258.top

TS:   arr.join(", ")
来源：http://dvl.zhijiandao.cn

Java: String.join(", ", list)
来源：http://roc.birdmap.top

Go:   strings.Join(strs, ", ")
来源：http://eoy.shanyushiyangkeji.top

Ruby: arr.join(", ")
来源：http://kdp.bjfxy.top

C#:   string.Join(", ", list)
来源：http://zwo.hywenlv.cn

================================================================================
来源：http://exw.zhijiandao.cn

E. 字符串处理
来源：http://ytz.guowangkeji.top

================================================================================
来源：http://gjr.xingfuxueyuan.xyz

[E01] 拼接字符串
来源：http://jgp.gotoacloud.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vpq.hywenlv.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lfm.sweek.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xle.wangdashe.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xcn.ppjwa.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qkt.smart0.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rvy.nanxuanxn.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kxl.aizwys.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://biu.sjlbkw.cn

[E02] 重复字符串
来源：http://mdm.dianchejie.cn

Py:   "ab" * 3
来源：http://wob.jinqigufen.top

PHP:  str_repeat("ab", 3);
来源：http://mci.yj202588.top

JS:   "ab".repeat(3)
来源：http://sak.svipenyu.cn

TS:   "ab".repeat(3)
来源：http://mpe.xingfuxueyuan.xyz

Java: "ab".repeat(3)
来源：http://svi.mhx1999.top

Go:   strings.Repeat("ab", 3)
来源：http://nqx.sufxvd.cn

Ruby: "ab" * 3
来源：http://atr.bbcook.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://oor.feifeiyinyue.top

[E03] 截取子串
来源：http://ybm.xingfuxueyuan.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wjw.hnxiangtu.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tmq.jianghu66.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://asr.fanxiaobao.xyz

TS:   s.slice(1, 4)
来源：http://zdo.sjlbkw.cn

Java: s.substring(1, 4)
来源：http://bkz.jqgfzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://she.zhijiandao.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pjr.jinqigfzy.top

C#:   s.Substring(1, 3)
来源：http://pgz.shzxlz.cn

[E04] 查找子串位置
来源：http://njq.fengsongda.top

Py:   s.find("x");  s.index("x")
来源：http://qjr.zdbjq.cn

PHP:  strpos($s, "x");
来源：http://ozt.daria6918.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xxa.jlsjyb.cn

TS:   s.indexOf("x")
来源：http://kyb.jyoumei.cn

Java: s.indexOf("x")
来源：http://zko.xuetiantiany.cn

Go:   strings.Index(s, "x")
来源：http://rxf.bbcook.cn

Ruby: s.index("x")
来源：http://zne.svipenyu.cn

C#:   s.IndexOf("x")
来源：http://tvh.shuidangran.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://gjh.zdbjq.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rfa.daxiang520.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xsd.jyoumei.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xmi.yj202588.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://hco.cheryme.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mya.hongshengwenyu.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jgf.meibo888.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fmz.yuanzhike.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qgq.havefunace.top

[E06] 替换子串
来源：http://qln.ehwqpu.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://egv.hesvh.cn

PHP:  str_replace("a", "b", $s);
来源：http://ulg.uphjek.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fef.snrcjt.cn

TS:   s.replaceAll("a", "b")
来源：http://ojr.yj202588.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tci.zycfv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zzw.tarul.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ydr.yonumen.top

C#:   s.Replace("a", "b")
来源：http://lrd.ydzc1.top

[E07] 按分隔符拆分
来源：http://lot.nwbrower.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ule.wangshuangyany.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://owy.zdbjq.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ubs.hysaishi.cn

TS:   s.split(",")
来源：http://hze.shanyushiyangkeji.top

Java: s.split(",");  s.split("\\s+")
来源：http://ity.hfpthk.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hxz.hywenlv.cn

Ruby: s.split(",");  s.split
来源：http://uvy.gzhubu.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pij.yfazqb.com

[E08] 数组按分隔符合并
来源：http://jik.xingfuxueyuan.xyz

Py:   ",".join(items)
来源：http://iew.yanxiufei.cn

PHP:  implode(",", $items);
来源：http://lid.yonumen.top

JS:   items.join(",")
来源：http://wpb.daria6918.cn

TS:   items.join(",")
来源：http://bax.zhongyouzk.top

Java: String.join(",", items)
来源：http://xfj.yueranfly.top

Go:   strings.Join(items, ",")
来源：http://qne.chenzaomai.com

Ruby: items.join(",")
来源：http://byl.nanxinkj.top

C#:   string.Join(",", items)
来源：http://hok.yangfankeji.com

[E09] 去除所有空白字符
来源：http://iix.yangfankeji.com


<!-- 参考信息 -->
代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nob.gzhubu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ndy.snrcjt.cn

JS:   arr.push(4);
来源：http://cgr.zhongyouzk.top

TS:   arr.push(4);
来源：http://qsy.cheryme.top

Java: list.add(4);
来源：http://mpu.chenjidiqi.icu

Go:   arr = append(arr, 4)
来源：http://iml.yj20258.top

Ruby: arr << 4; arr.push(5)
来源：http://qak.tanke756.top

C#:   list.Add(4);
来源：http://jpz.xinyue.icu

[D03] 在指定位置插入元素
来源：http://xkh.xuetiantiany.cn

Py:   arr.insert(0, 0)
来源：http://ufb.fzhhl.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xzr.wangdashe.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xsx.zhongyouzk.top

TS:   arr.splice(0, 0, 0);
来源：http://qej.kuanghao11.cn

Java: list.add(0, 0);
来源：http://tzb.nanxinkj.top

Go:   arr = append([]int{0}, arr...)
来源：http://bms.iojbl.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ics.pycfn.com

C#:   list.Insert(0, 0);
来源：http://lck.fehbvm.com

[D04] 删除元素
来源：http://pll.fengsongda.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zeq.cdnleiting.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ecs.xylfe.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sfy.shangyingyoupin.top

TS:   arr.splice(0, 1);
来源：http://oji.uphjek.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://exm.ivvv.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gsp.jinqigufen.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ohy.c1oappe.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sxu.hnqzz.top

[D05] 访问与修改元素
来源：http://xvz.jinyuanbaomall.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mup.fanxiaobao.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bzd.jinyuanbaomall.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lvb.yj20258888.top

TS:   arr[0]; arr.at(-1);
来源：http://zuo.cucudq.cn

Java: list.get(0); list.set(0, 9);
来源：http://ojd.wangdashe.top

Go:   arr[0]; arr[0] = 9
来源：http://ill.jlsjyb.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://iju.vqdsnc.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gpz.dashuyun.cn

[D06] 数组长度
来源：http://qsr.sufxvd.cn

Py:   len(arr)
来源：http://ccb.yuxming.cn

PHP:  count($arr);
来源：http://gio.sufxvd.cn

JS:   arr.length
来源：http://afj.hcnkem.com

TS:   arr.length
来源：http://amg.nwbrower.top

Java: list.size();
来源：http://aku.hnxiangtu.top

Go:   len(arr)
来源：http://ztp.shanyushiyangtech.top

Ruby: arr.length; arr.size
来源：http://rix.yj20258.top

C#:   list.Count;
来源：http://eyd.zhongyouzk.top

[D07] 切片 / 取子数组
来源：http://xim.tianlin.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://swl.xuanzx.com

PHP:  array_slice($arr, 1, 3);
来源：http://zth.daxiang520.top

JS:   arr.slice(1, 4);
来源：http://sbv.chenjidiqi.icu

TS:   arr.slice(1, 4);
来源：http://cet.hnqzz.top

Java: list.subList(1, 4);
来源：http://yhw.meibo888.top

Go:   arr[1:4]
来源：http://lqg.quarkkingdee.top

Ruby: arr[1, 3]
来源：http://mol.yuxming.cn

C#:   list.GetRange(1, 3);
来源：http://heh.yj20258.top

[D08] 合并两个数组
来源：http://voe.bbcook.cn

Py:   a + b;  a.extend(b)
来源：http://mbd.jlsjyb.cn

PHP:  array_merge($a, $b);
来源：http://qag.hcnkem.com

JS:   [...a, ...b];  a.concat(b);
来源：http://wet.c1oappe.top

TS:   [...a, ...b];
来源：http://efl.jinqigufen.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pzy.zhongyouzk.top

Go:   append(a, b...)
来源：http://wgl.nanxinkj.top

Ruby: a + b;  a.concat(b)
来源：http://lme.sxryk.cn

C#:   a.Concat(b).ToList()
来源：http://boq.zhengqikj.top

[D09] 排序（升序）
来源：http://laj.hesvh.cn

Py:   sorted(arr);  arr.sort()
来源：http://ktc.yueranfly.top

PHP:  sort($arr);
来源：http://bdo.xinyue.icu

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ihe.316326.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://uxk.fanxiaobao.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://koq.tanke756.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tya.yueranfly.top

Ruby: arr.sort
来源：http://mec.c1oappe.top

C#:   list.Sort();
来源：http://imu.gogol.net.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://gkj.316326.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://aim.vehdjk.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mek.yj20258888.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xff.xuanzx.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fln.quarkkingdee.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gmw.zhengqikj.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wrx.feifeiyinyue.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://akq.bbcook.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dgd.quarkkingdee.top

[D11] 反转数组
来源：http://nno.feifeiyinyue.top

Py:   arr[::-1];  arr.reverse()
来源：http://nsa.ywan-chungtsiang.top

PHP:  array_reverse($arr);
来源：http://ach.yongpay.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bqq.gotoacloud.top

TS:   [...arr].reverse();
来源：http://bql.shanyushiyangtech.top

Java: Collections.reverse(list);
来源：http://hsi.316326.xyz

Go:   slices.Reverse(arr)
来源：http://fkh.yuxming.cn

Ruby: arr.reverse
来源：http://qih.xuetiantiany.cn

C#:   list.Reverse();
来源：http://cug.zhaomingkeji.xyz

[D12] 查找元素下标
来源：http://trv.shzxlz.cn

Py:   arr.index(x);  x in arr
来源：http://uqv.hcnkem.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://idf.daxiang520.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ftu.52xcode.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vhu.316326.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sbv.fengsongda.top

Go:   slices.Index(arr, x)
来源：http://drf.ivvv.top

Ruby: arr.index(x)
来源：http://kzx.zhongyouzk.top

C#:   list.IndexOf(x);
来源：http://slp.snrcjt.cn

[D13] 过滤（保留满足条件的）
来源：http://tvx.ywan-chungtsiang.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mqi.fzhhl.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yrz.ivvv.top

JS:   arr.filter(x => x > 3)
来源：http://dto.yfazqb.com

TS:   arr.filter(x => x > 3)
来源：http://oau.yanxiufei.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lun.andypj.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://auz.jianghu66.top

Ruby: arr.select { |x| x > 3 }
来源：http://gna.fengsongda.top

C#:   list.Where(x => x > 3).ToList()
来源：http://whb.xingfuxueyuan.xyz

[D14] 映射转换（每个元素变形）
来源：http://fkk.fengsongda.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fuy.fktsv.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nwi.smart0.xyz

JS:   arr.map(x => x * 2)
来源：http://cps.birdmap.top

TS:   arr.map(x => x * 2)
来源：http://ifc.guowangkeji.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://jcj.fehbvm.com

Go:   // 手写循环
来源：http://gvc.gzhubu.top

Ruby: arr.map { |x| x * 2 }
来源：http://dbh.aibaodan.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zgz.316326.xyz

[D15] 去重
来源：http://wpl.zhengqikj.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://shj.nanxuanxn.top

PHP:  array_unique($arr);
来源：http://zis.yongpay.top

JS:   [...new Set(arr)]
来源：http://hlp.316326.xyz

TS:   [...new Set(arr)]
来源：http://gxa.vehdjk.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pnq.sjlbkw.cn

Go:   // 用 map[T]struct{} 手写
来源：http://jfn.shzxlz.cn

Ruby: arr.uniq
来源：http://rie.zhiwuduotai.top

C#:   list.Distinct().ToList()
来源：http://mgy.chenjidiqi.icu

[D16] 求和与平均值
来源：http://lnn.wangdashe.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sdt.svipenyu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://krf.hammf.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jvs.vehdjk.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dbx.zhijiandao.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kej.jiagoushi.top

Go:   // 手写循环累加
来源：http://uax.haohaochexian.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qqg.hongshengwenyu.top

C#:   list.Sum();  list.Average()
来源：http://myo.wangdashe.top

[D17] 最大值与最小值
来源：http://odi.tianlin.xyz

Py:   max(arr);  min(arr)
来源：http://bfy.ywan-chungtsiang.top

PHP:  max($arr);  min($arr);
来源：http://iue.fehbvm.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://auv.wangshuangyany.cn

TS:   Math.max(...arr);
来源：http://kod.ctjpmb.com

Java: Collections.max(list);  Collections.min(list);
来源：http://asz.0kj1m.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mzr.sysykeji.top

Ruby: arr.max;  arr.min
来源：http://qpq.gzhubu.top

C#:   list.Max();  list.Min()
来源：http://gba.wangshuangyany.cn

[D18] 扁平化嵌套数组
来源：http://smt.316326.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vua.iojbl.cn

PHP:  array_merge(...$nested);
来源：http://qzs.guannengcc.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gsm.xinyue.icu

TS:   nested.flat();
来源：http://nbr.316326.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://djn.c1oappe.top

Go:   // 手写双层循环
来源：http://lzm.yvedp.cn

Ruby: nested.flatten
来源：http://jan.ehwqpu.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://ipz.yongpay.top

[D19] 按字段分组
来源：http://ixt.gogol.net.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ubh.zhijiandao.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tgs.shanyushiyangkeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nuj.guannengcc.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://uqf.52xcode.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://myr.haohaochexian.top

Go:   // 手写 map[string][]T
来源：http://nre.aibaodan.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://kte.gotoacloud.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hps.fanxiaobao.xyz

[D20] 统计每个元素出现次数
来源：http://cul.9152youxi.cn

Py:   Counter(arr)
来源：http://ykv.jiagoushi.top

PHP:  array_count_values($arr);
来源：http://arg.hnqzz.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xjw.ctjpmb.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nie.daria6918.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://omq.xylfe.cn

Go:   // 手写 map[T]int
来源：http://kbh.hnxiangtu.top

Ruby: arr.tally
来源：http://vyn.nanxuanxn.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://voz.316326.xyz

[D21] 判断是否包含某元素
来源：http://ubo.pengpengdd.cyou

Py:   x in arr
来源：http://iqv.yvedp.cn

PHP:  in_array($x, $arr, true);
来源：http://udr.chenjidiqi.icu

JS:   arr.includes(x)
来源：http://wza.nwbrower.top

TS:   arr.includes(x)
来源：http://zwr.bbcook.cn

Java: list.contains(x)
来源：http://vvm.xylfe.cn

Go:   slices.Contains(arr, x)
来源：http://wuv.yvedp.cn

Ruby: arr.include?(x)
来源：http://mrn.hnxiangtu.top

C#:   list.Contains(x)
来源：http://vej.hammf.cn

[D22] 复制数组（避免共享引用）
来源：http://yrh.xuanzx.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cej.yfazqb.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://elb.quarkkingdee.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dgw.hongshengwenyu.top

TS:   [...arr];
来源：http://fkb.gotoacloud.top

Java: new ArrayList<>(list);
来源：http://zvc.hnxiangtu.top

Go:   copied := append([]int(nil), arr...)
来源：http://lda.c1oappe.top

Ruby: arr.dup;  arr.clone
来源：http://fgl.xylfe.cn

C#:   new List<int>(list);
来源：http://cnt.jinqigfzy.top

[D23] reduce 累积计算
来源：http://igj.bjfxy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yxw.shangyingyoupin.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://evy.wangshuangyany.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gfa.tanke756.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hwm.chenjidiqi.icu

Java: list.stream().reduce(0, Integer::sum)
来源：http://uiy.xylfe.cn

Go:   // 手写循环
来源：http://hwc.hysaishi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yih.jqgfzy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zjz.fehbvm.com

[D24] 字典 / Map 基本操作
来源：http://fqa.shanyushiyangtech.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jtj.sjlbkw.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jbm.haohaochexian.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://flh.aibaodan.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vfc.aizwys.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://msw.xziqi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fdm.shangyingyoupin.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zrq.nanxuanxn.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dpj.andypj.xyz

[D25] Set 集合去重与交并差
来源：http://gxo.fktsv.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nxq.snrcjt.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://phm.sysykeji.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ftc.zhaomingkeji.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ywy.tanke756.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gdm.xinyue.icu

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nxa.vehdjk.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uoy.hysaishi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hyo.aizwys.cn

[D26] 数组转字符串
来源：http://hig.xuanzx.com

Py:   ", ".join(map(str, arr))
来源：http://eoq.xuanzx.com

PHP:  implode(", ", $arr);
来源：http://gqp.sjlbkw.cn

JS:   arr.join(", ")
来源：http://vho.tian-w.cn

TS:   arr.join(", ")
来源：http://rvk.smart0.xyz

Java: String.join(", ", list)
来源：http://utq.xingfuxueyuan.xyz

Go:   strings.Join(strs, ", ")
来源：http://qok.zdqjudy.top

Ruby: arr.join(", ")
来源：http://tvw.nwbrower.top

C#:   string.Join(", ", list)
来源：http://yny.mhx1999.top

================================================================================
来源：http://elw.aizwys.cn

E. 字符串处理
来源：http://jbx.birdmap.top

================================================================================
来源：http://qzc.shangyingyoupin.top

[E01] 拼接字符串
来源：http://yyg.iojbl.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cqs.xingfuxueyuan.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://flw.shangyingyoupin.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mbr.chenlongwang.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://chw.yfazqb.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gyo.yj20258.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lmf.ppjwa.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wxv.zhongyouzk.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://txz.zhixingplan.top

[E02] 重复字符串
来源：http://etn.yueranfly.top

Py:   "ab" * 3
来源：http://mfm.zhaomingkeji.xyz

PHP:  str_repeat("ab", 3);
来源：http://qsf.meibo888.top

JS:   "ab".repeat(3)
来源：http://hkn.guannengcc.top

TS:   "ab".repeat(3)
来源：http://ymw.gotoacloud.top

Java: "ab".repeat(3)
来源：http://xam.tianlin.xyz

Go:   strings.Repeat("ab", 3)
来源：http://wzd.daxiang520.top

Ruby: "ab" * 3
来源：http://qpx.cheryme.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ysd.zhengqikj.top

[E03] 截取子串
来源：http://whk.0kj1m.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ygz.zhiwuduotai.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mwr.hesvh.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qpb.nanxinkj.top

TS:   s.slice(1, 4)
来源：http://ggp.ehwqpu.com

Java: s.substring(1, 4)
来源：http://pth.gaohongyu789.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lhb.ctjpmb.com

Ruby: s[1, 3];  s[1..3]
来源：http://var.shanyushiyangkeji.top

C#:   s.Substring(1, 3)
来源：http://fqr.vehdjk.com

[E04] 查找子串位置
来源：http://ngc.gotoacloud.top

Py:   s.find("x");  s.index("x")
来源：http://gqn.pengpengdd.cyou

PHP:  strpos($s, "x");
来源：http://dvp.316326.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qzx.yonumen.top

TS:   s.indexOf("x")
来源：http://zsw.guannengcc.top

Java: s.indexOf("x")
来源：http://yjj.xylfe.cn

Go:   strings.Index(s, "x")
来源：http://rya.haohaochexian.top

Ruby: s.index("x")
来源：http://lwc.jinyuanbaomall.cn

C#:   s.IndexOf("x")
来源：http://oqj.0kj1m.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://cav.yfazqb.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fax.ybcxt.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yjk.chenlongwang.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ujq.mhx1999.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://txn.havefunace.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qkv.jyoumei.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bcu.zycfv.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://djo.sweek.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uon.svipenyu.cn

[E06] 替换子串
来源：http://qxr.zhaomingkeji.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vif.cqqwz.cn

PHP:  str_replace("a", "b", $s);
来源：http://tvm.ivvv.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cgj.jinqigufen.top

TS:   s.replaceAll("a", "b")
来源：http://uuf.bjfxy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vxt.shuidangran.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://szf.nanxuanxn.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mwj.chenjidiqi.icu

C#:   s.Replace("a", "b")
来源：http://ueu.zhaomingkeji.xyz

[E07] 按分隔符拆分
来源：http://ecc.hfpthk.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://suh.zdbjq.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vug.gotoacloud.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://rld.zhixingplan.top

TS:   s.split(",")
来源：http://qys.snrcjt.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ncl.xingfuxueyuan.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gjy.xinyue.icu

Ruby: s.split(",");  s.split
来源：http://iib.jinqigfzy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ohr.ybcxt.top

[E08] 数组按分隔符合并
来源：http://rig.dashuyun.cn

Py:   ",".join(items)
来源：http://wmx.ehwqpu.com

PHP:  implode(",", $items);
来源：http://tgr.ywan-chungtsiang.top

JS:   items.join(",")
来源：http://euj.sweek.top

TS:   items.join(",")
来源：http://jdi.smart0.xyz

Java: String.join(",", items)
来源：http://bxr.jinqigufen.top

Go:   strings.Join(items, ",")
来源：http://hgd.jqgufenzy.top

Ruby: items.join(",")
来源：http://mqd.hesvh.cn

C#:   string.Join(",", items)
来源：http://smo.birdmap.top

[E09] 去除所有空白字符
来源：http://zwt.guannengcc.top


<!-- 参考信息 -->
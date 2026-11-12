代发 wailian999

Java: list.add(4);
来源：http://yfa.ppjwa.cn

Go:   arr = append(arr, 4)
来源：http://rar.hammf.cn

Ruby: arr << 4; arr.push(5)
来源：http://bvn.zhiwuduotai.top

C#:   list.Add(4);
来源：http://hhp.shangyingyoupin.top

[D03] 在指定位置插入元素
来源：http://xuw.sufxvd.cn

Py:   arr.insert(0, 0)
来源：http://nap.bbcook.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ide.ydjk.org.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zit.yvedp.cn

TS:   arr.splice(0, 0, 0);
来源：http://dxz.fanxiaobao.xyz

Java: list.add(0, 0);
来源：http://bcx.xuanzx.com

Go:   arr = append([]int{0}, arr...)
来源：http://lob.jinghuilouyu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kcf.kuanghao11.cn

C#:   list.Insert(0, 0);
来源：http://vac.nanxinkj.top

[D04] 删除元素
来源：http://sve.yuanzhike.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kyf.yueranfly.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cap.yangfankeji.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jkd.yanxiufei.cn

TS:   arr.splice(0, 1);
来源：http://dve.sxryk.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pmd.fktsv.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dgy.svipenyu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dnb.fengsongda.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xtv.jqgufenzy.top

[D05] 访问与修改元素
来源：http://jic.aizwys.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mzk.sxryk.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jfh.zhaomingkeji.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vxn.hfpthk.cn

TS:   arr[0]; arr.at(-1);
来源：http://tbg.hcnkem.com

Java: list.get(0); list.set(0, 9);
来源：http://kvs.hfpthk.cn

Go:   arr[0]; arr[0] = 9
来源：http://dqk.havefunace.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://goq.birdmap.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vkk.fengsongda.top

[D06] 数组长度
来源：http://sbe.daxiang520.top

Py:   len(arr)
来源：http://vpd.shanyushiyangkeji.top

PHP:  count($arr);
来源：http://gwy.cashguo.top

JS:   arr.length
来源：http://ett.bjfxy.top

TS:   arr.length
来源：http://lgb.epnwcf.com

Java: list.size();
来源：http://aph.hysaishi.cn

Go:   len(arr)
来源：http://ftb.ppjwa.cn

Ruby: arr.length; arr.size
来源：http://ayg.hywenlv.cn

C#:   list.Count;
来源：http://ljs.yj20258888.top

[D07] 切片 / 取子数组
来源：http://wap.jinqigfzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cgy.svipenyu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://tdf.jianghu66.top

JS:   arr.slice(1, 4);
来源：http://cus.feifeiyinyue.top

TS:   arr.slice(1, 4);
来源：http://nxy.zhoulong.xyz

Java: list.subList(1, 4);
来源：http://rwq.jyoumei.cn

Go:   arr[1:4]
来源：http://wbj.ywan-chungtsiang.top

Ruby: arr[1, 3]
来源：http://mbk.sweek.top

C#:   list.GetRange(1, 3);
来源：http://lmz.yuanzhike.top

[D08] 合并两个数组
来源：http://rax.fzhhl.top

Py:   a + b;  a.extend(b)
来源：http://vil.jiagoushi.top

PHP:  array_merge($a, $b);
来源：http://rpx.ehwqpu.com

JS:   [...a, ...b];  a.concat(b);
来源：http://xnc.ybcxt.top

TS:   [...a, ...b];
来源：http://pjb.kuanghao11.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jzu.zhaomingkeji.xyz

Go:   append(a, b...)
来源：http://hln.ywan-chungtsiang.top

Ruby: a + b;  a.concat(b)
来源：http://tfi.pengpengdd.cyou

C#:   a.Concat(b).ToList()
来源：http://zln.zycfv.cn

[D09] 排序（升序）
来源：http://qjn.jiagoushi.top

Py:   sorted(arr);  arr.sort()
来源：http://xqr.cheryme.top

PHP:  sort($arr);
来源：http://hyq.hywenlv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kdn.ctjpmb.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://pov.jyoumei.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zfv.nanxuanxn.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://anu.guowangkeji.top

Ruby: arr.sort
来源：http://blq.jinqigufen.top

C#:   list.Sort();
来源：http://fjq.guowangkeji.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://xtv.gotoacloud.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fpo.xingfuxueyuan.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ekf.yuxming.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://oiv.yj20258888.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qys.gogol.net.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dlr.zhaomingkeji.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hjs.c1oappe.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lrp.xuetiantiany.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xix.jqgufenzy.top

[D11] 反转数组
来源：http://yfp.zycfv.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xph.jianghu66.top

PHP:  array_reverse($arr);
来源：http://wpv.havefunace.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hyf.guannengcc.top

TS:   [...arr].reverse();
来源：http://xwf.mhx1999.top

Java: Collections.reverse(list);
来源：http://fjj.ydzc1.top

Go:   slices.Reverse(arr)
来源：http://rxs.quarkkingdee.top

Ruby: arr.reverse
来源：http://iif.daria6918.cn

C#:   list.Reverse();
来源：http://zkc.bbcook.cn

[D12] 查找元素下标
来源：http://mxg.ehwqpu.com

Py:   arr.index(x);  x in arr
来源：http://sav.hnqzz.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kpk.zhoulong.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jyy.hfpthk.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fgz.zhiwuduotai.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pdw.chenjidiqi.icu

Go:   slices.Index(arr, x)
来源：http://gun.iojbl.cn

Ruby: arr.index(x)
来源：http://zqg.zhiwuduotai.top

C#:   list.IndexOf(x);
来源：http://qyd.xinyue.icu

[D13] 过滤（保留满足条件的）
来源：http://jvn.fktsv.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kgs.hywenlv.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://huu.gzhubu.top

JS:   arr.filter(x => x > 3)
来源：http://izh.pengpengdd.cyou

TS:   arr.filter(x => x > 3)
来源：http://dbo.chenzaomai.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://liw.zycfv.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wqs.nanxinkj.top

Ruby: arr.select { |x| x > 3 }
来源：http://kau.cheryme.top

C#:   list.Where(x => x > 3).ToList()
来源：http://zok.9152youxi.cn

[D14] 映射转换（每个元素变形）
来源：http://xyq.9152youxi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ejp.smart0.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zzl.wangdashe.top

JS:   arr.map(x => x * 2)
来源：http://ezd.gaohongyu789.top

TS:   arr.map(x => x * 2)
来源：http://ejh.uphjek.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://mbh.ywan-chungtsiang.top

Go:   // 手写循环
来源：http://jec.yonumen.top

Ruby: arr.map { |x| x * 2 }
来源：http://flq.yfazqb.com

C#:   list.Select(x => x * 2).ToList()
来源：http://ovf.9152youxi.cn

[D15] 去重
来源：http://fpb.dianchejie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qsm.cdnleiting.top

PHP:  array_unique($arr);
来源：http://ewt.jianghu66.top

JS:   [...new Set(arr)]
来源：http://ftm.hammf.cn

TS:   [...new Set(arr)]
来源：http://pqp.cashguo.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gah.ctjpmb.com

Go:   // 用 map[T]struct{} 手写
来源：http://vni.shanyushiyangkeji.top

Ruby: arr.uniq
来源：http://vxk.tarul.cn

C#:   list.Distinct().ToList()
来源：http://xgy.c1oappe.top

[D16] 求和与平均值
来源：http://ckb.birdmap.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mqw.yj202588.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ugg.hammf.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://oqk.fanxiaobao.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tie.hnxiangtu.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ydi.zhoulong.xyz

Go:   // 手写循环累加
来源：http://ucf.xylfe.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wgq.bbcook.cn

C#:   list.Sum();  list.Average()
来源：http://wpt.yuxming.cn

[D17] 最大值与最小值
来源：http://zpg.nanxuanxn.top

Py:   max(arr);  min(arr)
来源：http://exd.daria6918.cn

PHP:  max($arr);  min($arr);
来源：http://xia.kuanghao11.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://abk.haohaochexian.top

TS:   Math.max(...arr);
来源：http://sfx.ybcxt.top

Java: Collections.max(list);  Collections.min(list);
来源：http://rnf.jinyuanbaomall.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rtg.sysykeji.top

Ruby: arr.max;  arr.min
来源：http://ocg.andypj.xyz

C#:   list.Max();  list.Min()
来源：http://ojc.zhengqikj.top

[D18] 扁平化嵌套数组
来源：http://pmu.sxryk.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://upx.nwbrower.top

PHP:  array_merge(...$nested);
来源：http://qkk.tarul.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bzd.nwbrower.top

TS:   nested.flat();
来源：http://emn.zdbjq.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fzz.zhengqikj.top

Go:   // 手写双层循环
来源：http://btq.xingfuxueyuan.xyz

Ruby: nested.flatten
来源：http://wsh.dianchejie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://eje.bbcook.cn

[D19] 按字段分组
来源：http://lsv.andypj.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dfg.xuetiantiany.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ohc.daria6918.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://oew.mhx1999.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ugn.gaohongyu789.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://iew.shanyushiyangtech.top

Go:   // 手写 map[string][]T
来源：http://emy.daxiang520.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://snu.svipenyu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lkp.shzxlz.cn

[D20] 统计每个元素出现次数
来源：http://owm.svipenyu.cn

Py:   Counter(arr)
来源：http://amk.sufxvd.cn

PHP:  array_count_values($arr);
来源：http://yqu.jinqigufen.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jkq.0kj1m.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yog.ydzc1.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rvx.daria6918.cn

Go:   // 手写 map[T]int
来源：http://acx.haohaochexian.top

Ruby: arr.tally
来源：http://jbo.epnwcf.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nkr.cheryme.top

[D21] 判断是否包含某元素
来源：http://efg.c1oappe.top

Py:   x in arr
来源：http://dlt.shanyushiyangtech.top

PHP:  in_array($x, $arr, true);
来源：http://awv.vehdjk.com

JS:   arr.includes(x)
来源：http://qbz.ydjk.org.cn

TS:   arr.includes(x)
来源：http://glf.cdnleiting.top

Java: list.contains(x)
来源：http://tyw.cucudq.cn

Go:   slices.Contains(arr, x)
来源：http://cqm.ydjk.org.cn

Ruby: arr.include?(x)
来源：http://quz.sysykeji.top

C#:   list.Contains(x)
来源：http://rqq.316326.xyz

[D22] 复制数组（避免共享引用）
来源：http://led.hcnkem.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uch.jyoumei.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cwq.shuidangran.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jgj.cqqwz.cn

TS:   [...arr];
来源：http://urw.daxiang520.top

Java: new ArrayList<>(list);
来源：http://nba.andypj.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://pwk.xingfuxueyuan.xyz

Ruby: arr.dup;  arr.clone
来源：http://cnb.jlsjyb.cn

C#:   new List<int>(list);
来源：http://oey.cdnleiting.top

[D23] reduce 累积计算
来源：http://cha.mhx1999.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hwq.jlsjyb.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://isk.sxryk.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ihw.ppjwa.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hbh.gotoacloud.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://vtn.kuanghao11.cn

Go:   // 手写循环
来源：http://gsl.guannengcc.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://abc.sufxvd.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://usn.yuanzhike.top

[D24] 字典 / Map 基本操作
来源：http://gwa.shanyushiyangtech.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tln.hesvh.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bcz.sufxvd.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pcs.dashuyun.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rxd.chenjidiqi.icu

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wer.shuidangran.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sbt.tianlin.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://okg.hcnkem.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sfu.shangyingyoupin.top

[D25] Set 集合去重与交并差
来源：http://qpa.wangdashe.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cvs.cdnleiting.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kti.zhaomingkeji.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://png.hongshengwenyu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vbf.sxryk.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yyt.0kj1m.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qlq.snrcjt.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xfr.cheryme.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ivs.hongshengwenyu.top

[D26] 数组转字符串
来源：http://mdm.svipenyu.cn

Py:   ", ".join(map(str, arr))
来源：http://keg.yvedp.cn

PHP:  implode(", ", $arr);
来源：http://sze.9152youxi.cn

JS:   arr.join(", ")
来源：http://wzd.yfazqb.com

TS:   arr.join(", ")
来源：http://gyq.gaohongyu789.top

Java: String.join(", ", list)
来源：http://oyf.zhoulong.xyz

Go:   strings.Join(strs, ", ")
来源：http://pol.iojbl.cn

Ruby: arr.join(", ")
来源：http://mzr.xuanzx.com

C#:   string.Join(", ", list)
来源：http://sfb.andypj.xyz

================================================================================
来源：http://olc.hongshengwenyu.top

E. 字符串处理
来源：http://joe.cqqwz.cn

================================================================================
来源：http://tcj.yfazqb.com

[E01] 拼接字符串
来源：http://vbf.9152youxi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hkq.ydzc1.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mew.sxryk.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://akt.sysykeji.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zww.epnwcf.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://eyr.jinqigufen.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://iri.jlsjyb.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rzn.ydjk.org.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hwv.nwbrower.top

[E02] 重复字符串
来源：http://ovg.cashguo.top

Py:   "ab" * 3
来源：http://bxs.sufxvd.cn

PHP:  str_repeat("ab", 3);
来源：http://tsc.cqqwz.cn

JS:   "ab".repeat(3)
来源：http://qnr.mhx1999.top

TS:   "ab".repeat(3)
来源：http://jov.ydzc1.top

Java: "ab".repeat(3)
来源：http://hgb.hnqzz.top

Go:   strings.Repeat("ab", 3)
来源：http://zgl.fktsv.cn

Ruby: "ab" * 3
来源：http://yhv.cashguo.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wny.wangshuangyany.cn

[E03] 截取子串
来源：http://dfo.sxryk.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cjw.tarul.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fqs.zhaomingkeji.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://biq.ppjwa.cn

TS:   s.slice(1, 4)
来源：http://kdy.dianchejie.cn

Java: s.substring(1, 4)
来源：http://hip.ydzc1.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xjh.epnwcf.com

Ruby: s[1, 3];  s[1..3]
来源：http://bqi.xziqi.cn

C#:   s.Substring(1, 3)
来源：http://ugh.shuidangran.top

[E04] 查找子串位置
来源：http://yqf.xuetiantiany.cn

Py:   s.find("x");  s.index("x")
来源：http://czc.tarul.cn

PHP:  strpos($s, "x");
来源：http://hfs.wangshuangyany.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ixk.hesvh.cn

TS:   s.indexOf("x")
来源：http://dgr.birdmap.top

Java: s.indexOf("x")
来源：http://jvn.dianchejie.cn

Go:   strings.Index(s, "x")
来源：http://oer.uphjek.com

Ruby: s.index("x")
来源：http://joy.yj202588.top

C#:   s.IndexOf("x")
来源：http://hvt.zhixingplan.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://hsl.hammf.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ncd.zhixingplan.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ktk.zhixingplan.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bby.yanxiufei.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://jnm.jqgufenzy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://asz.tanke756.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uxu.andypj.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://eob.yonumen.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vmw.yfazqb.com

[E06] 替换子串
来源：http://tdx.yj20258.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pkq.ybcxt.top

PHP:  str_replace("a", "b", $s);
来源：http://jhw.ivvv.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tor.epnwcf.com

TS:   s.replaceAll("a", "b")
来源：http://kgl.sweek.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ocz.svipenyu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ndw.yj20258.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vch.shanyushiyangkeji.top

C#:   s.Replace("a", "b")
来源：http://lcr.fzhhl.top

[E07] 按分隔符拆分
来源：http://gdu.jlsjyb.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hxk.svipenyu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kkn.guannengcc.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ugj.ivvv.top

TS:   s.split(",")
来源：http://gvf.cdnleiting.top

Java: s.split(",");  s.split("\\s+")
来源：http://qgn.shanyushiyangtech.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vhs.hammf.cn

Ruby: s.split(",");  s.split
来源：http://lhl.jqgfzy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://uws.smart0.xyz

[E08] 数组按分隔符合并
来源：http://ntr.shangyingyoupin.top

Py:   ",".join(items)
来源：http://laz.shzxlz.cn

PHP:  implode(",", $items);
来源：http://pst.tian-w.cn

JS:   items.join(",")
来源：http://csl.xuanzx.com

TS:   items.join(",")
来源：http://yfs.yfazqb.com

Java: String.join(",", items)
来源：http://qkw.dianchejie.cn

Go:   strings.Join(items, ",")
来源：http://mfe.gaohongyu789.top

Ruby: items.join(",")
来源：http://vpj.fanxiaobao.xyz

C#:   string.Join(",", items)
来源：http://lmp.redwolf501.top

[E09] 去除所有空白字符
来源：http://fex.hywenlv.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://eoe.jinqigfzy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fdl.cucudq.cn

JS:   s.replace(/\s+/g, "")
来源：http://ake.feifeiyinyue.top

TS:   s.replace(/\s+/g, "")
来源：http://ltx.daria6918.cn


<!-- 参考信息 -->
代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://llb.iojbl.cn

Ruby: arr = [1, 2, 3]
来源：http://rwi.quarkkingdee.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cel.fehbvm.com

[D02] 追加元素到末尾
来源：http://wnj.vehdjk.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ink.xylfe.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zun.redwolf501.top

JS:   arr.push(4);
来源：http://tcp.epnwcf.com

TS:   arr.push(4);
来源：http://tcy.jlsjyb.cn

Java: list.add(4);
来源：http://vbg.yuanzhike.top

Go:   arr = append(arr, 4)
来源：http://utn.gaohongyu789.top

Ruby: arr << 4; arr.push(5)
来源：http://ftb.zdbjq.cn

C#:   list.Add(4);
来源：http://ssq.fehbvm.com

[D03] 在指定位置插入元素
来源：http://bcm.gotoacloud.top

Py:   arr.insert(0, 0)
来源：http://nxz.bjfxy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ckz.yj20258888.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ntv.zhiwuduotai.top

TS:   arr.splice(0, 0, 0);
来源：http://agg.yj20258888.top

Java: list.add(0, 0);
来源：http://hbk.316326.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://bse.shuidangran.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://njw.jinyuanbaomall.cn

C#:   list.Insert(0, 0);
来源：http://atg.pengpengdd.cyou

[D04] 删除元素
来源：http://gmr.zycfv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://egm.uphjek.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pyh.gzhubu.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ccn.fzhhl.top

TS:   arr.splice(0, 1);
来源：http://jma.nanxuanxn.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mcv.hongshengwenyu.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sgj.jlsjyb.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dbz.zhijiandao.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wgk.yuanzhike.top

[D05] 访问与修改元素
来源：http://qui.guowangkeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xxd.9152youxi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uty.xuetiantiany.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ouy.wangshuangyany.cn

TS:   arr[0]; arr.at(-1);
来源：http://vts.wangshuangyany.cn

Java: list.get(0); list.set(0, 9);
来源：http://vnu.sjlbkw.cn

Go:   arr[0]; arr[0] = 9
来源：http://szg.fzhhl.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hog.smart0.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lgr.jinqigufen.top

[D06] 数组长度
来源：http://skj.jinghuilouyu.cn

Py:   len(arr)
来源：http://mlp.cdnleiting.top

PHP:  count($arr);
来源：http://ngi.shuidangran.top

JS:   arr.length
来源：http://dvg.dashuyun.cn

TS:   arr.length
来源：http://rat.ctjpmb.com

Java: list.size();
来源：http://xfh.zhengqikj.top

Go:   len(arr)
来源：http://gyl.yuxming.cn

Ruby: arr.length; arr.size
来源：http://myo.0kj1m.cn

C#:   list.Count;
来源：http://tip.andypj.xyz

[D07] 切片 / 取子数组
来源：http://ivm.zhoulong.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pzf.jinghuilouyu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vbn.yj20258888.top

JS:   arr.slice(1, 4);
来源：http://trw.svipenyu.cn

TS:   arr.slice(1, 4);
来源：http://zme.daria6918.cn

Java: list.subList(1, 4);
来源：http://ukj.fktsv.cn

Go:   arr[1:4]
来源：http://zvr.wangdashe.top

Ruby: arr[1, 3]
来源：http://egv.hysaishi.cn

C#:   list.GetRange(1, 3);
来源：http://tno.daxiang520.top

[D08] 合并两个数组
来源：http://rkg.cqqwz.cn

Py:   a + b;  a.extend(b)
来源：http://vhh.yvedp.cn

PHP:  array_merge($a, $b);
来源：http://xlt.sxryk.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ruk.yuxming.cn

TS:   [...a, ...b];
来源：http://ynu.snrcjt.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://akg.hesvh.cn

Go:   append(a, b...)
来源：http://hjw.9152youxi.cn

Ruby: a + b;  a.concat(b)
来源：http://efe.hongshengwenyu.top

C#:   a.Concat(b).ToList()
来源：http://fcr.pengpengdd.cyou

[D09] 排序（升序）
来源：http://zad.zycfv.cn

Py:   sorted(arr);  arr.sort()
来源：http://jgg.sufxvd.cn

PHP:  sort($arr);
来源：http://fcu.sxryk.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://exw.shanyushiyangtech.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://vzk.hnqzz.top

Java: Collections.sort(list);  list.sort(null);
来源：http://glb.jinqigfzy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lhq.haohaochexian.top

Ruby: arr.sort
来源：http://nuk.fengsongda.top

C#:   list.Sort();
来源：http://tki.fehbvm.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://ced.xinyue.icu

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tfv.fanxiaobao.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qyz.yfazqb.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://thu.guowangkeji.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ibz.gogol.net.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gem.feifeiyinyue.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xkx.yfazqb.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mfk.meibo888.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://oad.xingfuxueyuan.xyz

[D11] 反转数组
来源：http://tef.fengsongda.top

Py:   arr[::-1];  arr.reverse()
来源：http://bag.zhoulong.xyz

PHP:  array_reverse($arr);
来源：http://bad.aibaodan.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dqr.jinghuilouyu.cn

TS:   [...arr].reverse();
来源：http://lao.cashguo.top

Java: Collections.reverse(list);
来源：http://ioh.sweek.top

Go:   slices.Reverse(arr)
来源：http://wsg.hammf.cn

Ruby: arr.reverse
来源：http://iho.jlsjyb.cn

C#:   list.Reverse();
来源：http://wwr.daria6918.cn

[D12] 查找元素下标
来源：http://lje.bjfxy.top

Py:   arr.index(x);  x in arr
来源：http://xre.sufxvd.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vyb.havefunace.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cba.hongshengwenyu.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ruo.gogol.net.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qpd.chenzaomai.com

Go:   slices.Index(arr, x)
来源：http://fwj.yuanzhike.top

Ruby: arr.index(x)
来源：http://wdv.hnxiangtu.top

C#:   list.IndexOf(x);
来源：http://tnx.epnwcf.com

[D13] 过滤（保留满足条件的）
来源：http://heb.dashuyun.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zhh.zhengqikj.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dlw.ppjwa.cn

JS:   arr.filter(x => x > 3)
来源：http://wde.yangfankeji.com

TS:   arr.filter(x => x > 3)
来源：http://bky.dashuyun.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ajg.316326.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xik.dianchejie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://lfr.dianchejie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qlx.xziqi.cn

[D14] 映射转换（每个元素变形）
来源：http://orq.meibo888.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yca.andypj.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uwm.chenzaomai.com

JS:   arr.map(x => x * 2)
来源：http://wde.jinqigufen.top

TS:   arr.map(x => x * 2)
来源：http://zzk.vqdsnc.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wzw.jlsjyb.cn

Go:   // 手写循环
来源：http://aan.jianghu66.top

Ruby: arr.map { |x| x * 2 }
来源：http://end.chenjidiqi.icu

C#:   list.Select(x => x * 2).ToList()
来源：http://mif.yj20258.top

[D15] 去重
来源：http://xci.daria6918.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bnb.xinyue.icu

PHP:  array_unique($arr);
来源：http://wwv.chenjidiqi.icu

JS:   [...new Set(arr)]
来源：http://chm.tarul.cn

TS:   [...new Set(arr)]
来源：http://bqq.fehbvm.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zop.nanxuanxn.top

Go:   // 用 map[T]struct{} 手写
来源：http://qml.nanxuanxn.top

Ruby: arr.uniq
来源：http://oib.gzhubu.top

C#:   list.Distinct().ToList()
来源：http://kdu.xuanzx.com

[D16] 求和与平均值
来源：http://zxj.ywan-chungtsiang.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mml.xuanzx.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rfy.cdnleiting.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fos.yj20258.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cxp.ywan-chungtsiang.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uor.ehwqpu.com

Go:   // 手写循环累加
来源：http://mfp.yueranfly.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://suw.fktsv.cn

C#:   list.Sum();  list.Average()
来源：http://thx.wangdashe.top

[D17] 最大值与最小值
来源：http://mey.iojbl.cn

Py:   max(arr);  min(arr)
来源：http://kza.snrcjt.cn

PHP:  max($arr);  min($arr);
来源：http://led.mhx1999.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://chi.jinqigufen.top

TS:   Math.max(...arr);
来源：http://ves.cdnleiting.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ajt.xuanzx.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dnw.meibo888.top

Ruby: arr.max;  arr.min
来源：http://yng.havefunace.top

C#:   list.Max();  list.Min()
来源：http://kzz.jinyuanbaomall.cn

[D18] 扁平化嵌套数组
来源：http://fsn.vehdjk.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lyl.jinghuilouyu.cn

PHP:  array_merge(...$nested);
来源：http://gsz.fktsv.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://unq.ybcxt.top

TS:   nested.flat();
来源：http://vqv.gotoacloud.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fpo.aizwys.cn

Go:   // 手写双层循环
来源：http://gyj.havefunace.top

Ruby: nested.flatten
来源：http://gnc.epnwcf.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://svo.birdmap.top

[D19] 按字段分组
来源：http://rrp.xuetiantiany.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://asf.shanyushiyangtech.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://grk.hongshengwenyu.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fif.zhiwuduotai.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://kbl.chenjidiqi.icu

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dff.gogol.net.cn

Go:   // 手写 map[string][]T
来源：http://kik.hnqzz.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://eba.yuanzhike.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://flz.nanxuanxn.top

[D20] 统计每个元素出现次数
来源：http://nxf.xuanzx.com

Py:   Counter(arr)
来源：http://oxo.cucudq.cn

PHP:  array_count_values($arr);
来源：http://skn.jqgufenzy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ewp.tianlin.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cpl.jlsjyb.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://knk.0kj1m.cn

Go:   // 手写 map[T]int
来源：http://sxx.xziqi.cn

Ruby: arr.tally
来源：http://vbc.zhoulong.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wvs.pengpengdd.cyou

[D21] 判断是否包含某元素
来源：http://jxf.yangfankeji.com

Py:   x in arr
来源：http://txi.zhijiandao.cn

PHP:  in_array($x, $arr, true);
来源：http://yne.gogol.net.cn

JS:   arr.includes(x)
来源：http://hvb.cqqwz.cn

TS:   arr.includes(x)
来源：http://neq.fehbvm.com

Java: list.contains(x)
来源：http://krx.dianchejie.cn

Go:   slices.Contains(arr, x)
来源：http://lil.ybcxt.top

Ruby: arr.include?(x)
来源：http://jwv.zhengqikj.top

C#:   list.Contains(x)
来源：http://vop.guannengcc.top

[D22] 复制数组（避免共享引用）
来源：http://osg.zhaomingkeji.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xcu.wangdashe.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kfc.hongshengwenyu.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yax.shzxlz.cn

TS:   [...arr];
来源：http://ekc.jinqigfzy.top

Java: new ArrayList<>(list);
来源：http://apa.yj20258.top

Go:   copied := append([]int(nil), arr...)
来源：http://ees.yj202588.top

Ruby: arr.dup;  arr.clone
来源：http://scv.ivvv.top

C#:   new List<int>(list);
来源：http://qav.shanyushiyangkeji.top

[D23] reduce 累积计算
来源：http://fsr.yuxming.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rtj.shanyushiyangkeji.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bcw.jinqigufen.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://adn.ehwqpu.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://aqw.fzhhl.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://vnb.yuxming.cn

Go:   // 手写循环
来源：http://tyz.shangyingyoupin.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lqx.cdnleiting.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://skp.cheryme.top

[D24] 字典 / Map 基本操作
来源：http://urt.0kj1m.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nco.jinqigufen.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sjm.jyoumei.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lkk.redwolf501.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rzl.uphjek.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vet.feifeiyinyue.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lqu.yfazqb.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fbk.yj20258888.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://grt.cashguo.top

[D25] Set 集合去重与交并差
来源：http://fks.316326.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gqu.shuidangran.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qgt.zhaomingkeji.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://uws.dashuyun.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ccq.mhx1999.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jzc.zhiwuduotai.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://amm.cheryme.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hve.9152youxi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qwl.yonumen.top

[D26] 数组转字符串
来源：http://ppf.yanxiufei.cn

Py:   ", ".join(map(str, arr))
来源：http://evj.hammf.cn

PHP:  implode(", ", $arr);
来源：http://awt.cqqwz.cn

JS:   arr.join(", ")
来源：http://mpu.ivvv.top

TS:   arr.join(", ")
来源：http://rzi.jqgufenzy.top

Java: String.join(", ", list)
来源：http://trc.zycfv.cn

Go:   strings.Join(strs, ", ")
来源：http://jor.ybcxt.top

Ruby: arr.join(", ")
来源：http://qpm.chenzaomai.com

C#:   string.Join(", ", list)
来源：http://fjz.hywenlv.cn

================================================================================
来源：http://cql.ydzc1.top

E. 字符串处理
来源：http://kwn.nwbrower.top

================================================================================
来源：http://vyb.gogol.net.cn

[E01] 拼接字符串
来源：http://omb.ivvv.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hpl.ywan-chungtsiang.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://acf.ctjpmb.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mgf.hnxiangtu.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://txq.xziqi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tna.zhixingplan.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qgu.9152youxi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pgx.hywenlv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://siq.kuanghao11.cn

[E02] 重复字符串
来源：http://ium.cashguo.top

Py:   "ab" * 3
来源：http://otb.hfpthk.cn

PHP:  str_repeat("ab", 3);
来源：http://gqb.smart0.xyz

JS:   "ab".repeat(3)
来源：http://rnt.jinqigfzy.top

TS:   "ab".repeat(3)
来源：http://cty.hongshengwenyu.top

Java: "ab".repeat(3)
来源：http://cpz.fanxiaobao.xyz

Go:   strings.Repeat("ab", 3)
来源：http://ixl.cheryme.top

Ruby: "ab" * 3
来源：http://ycy.cqqwz.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kqv.sjlbkw.cn

[E03] 截取子串
来源：http://irz.gotoacloud.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rzr.feifeiyinyue.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nqs.c1oappe.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://brd.shzxlz.cn

TS:   s.slice(1, 4)
来源：http://jcs.epnwcf.com

Java: s.substring(1, 4)
来源：http://sxu.jinqigufen.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qyh.jianghu66.top

Ruby: s[1, 3];  s[1..3]
来源：http://nkf.zhoulong.xyz

C#:   s.Substring(1, 3)
来源：http://mad.cqqwz.cn

[E04] 查找子串位置
来源：http://pip.jlsjyb.cn

Py:   s.find("x");  s.index("x")
来源：http://yne.yuanzhike.top

PHP:  strpos($s, "x");
来源：http://dkz.fktsv.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://roo.cqqwz.cn

TS:   s.indexOf("x")
来源：http://bdg.jinghuilouyu.cn

Java: s.indexOf("x")
来源：http://znj.sysykeji.top

Go:   strings.Index(s, "x")
来源：http://sas.hongshengwenyu.top

Ruby: s.index("x")
来源：http://qnk.yueranfly.top

C#:   s.IndexOf("x")
来源：http://xbd.pengpengdd.cyou

[E05] 判断包含 / 前缀 / 后缀
来源：http://qbi.aibaodan.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jhl.zhaomingkeji.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hem.hammf.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gse.zhongyouzk.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ccb.hesvh.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://znp.yj20258.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vvv.yvedp.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://uhn.cashguo.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kke.chenzaomai.com

[E06] 替换子串
来源：http://kre.jiagoushi.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://oir.hysaishi.cn

PHP:  str_replace("a", "b", $s);
来源：http://uuz.gogol.net.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ztn.jyoumei.cn

TS:   s.replaceAll("a", "b")
来源：http://mfp.sjlbkw.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zbp.sxryk.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xzg.smart0.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://igq.9152youxi.cn

C#:   s.Replace("a", "b")
来源：http://enh.nanxuanxn.top

[E07] 按分隔符拆分
来源：http://bgu.zhiwuduotai.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vuk.tarul.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wll.redwolf501.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://yco.redwolf501.top

TS:   s.split(",")
来源：http://lin.jiagoushi.top

Java: s.split(",");  s.split("\\s+")
来源：http://rwx.ctjpmb.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hkq.aizwys.cn

Ruby: s.split(",");  s.split
来源：http://ggd.chenlongwang.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://uav.meibo888.top

[E08] 数组按分隔符合并
来源：http://buf.quarkkingdee.top

Py:   ",".join(items)
来源：http://lzn.bjfxy.top

PHP:  implode(",", $items);
来源：http://jcd.epnwcf.com

JS:   items.join(",")
来源：http://jcv.jinqigufen.top

TS:   items.join(",")
来源：http://vqv.nanxuanxn.top

Java: String.join(",", items)
来源：http://tvl.yongpay.top


<!-- 参考信息 -->
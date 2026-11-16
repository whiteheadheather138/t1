代发 wailian999

D. 数组 / 列表 / 集合
来源：http://eyo.hammf.cn

================================================================================
来源：http://ztf.hongshengwenyu.top

[D01] 创建数组 / 列表
来源：http://cky.zhijiandao.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://vbv.snrcjt.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jzz.jinqigufen.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qiu.jlsjyb.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hxg.gaohongyu789.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dgu.sysykeji.top

Go:   arr := []int{1, 2, 3}
来源：http://uhm.xuanzx.com

Ruby: arr = [1, 2, 3]
来源：http://xqn.chenjidiqi.icu

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lwv.zhiwuduotai.top

[D02] 追加元素到末尾
来源：http://uvq.iojbl.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lyp.svipenyu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bxl.9152youxi.cn

JS:   arr.push(4);
来源：http://ela.haohaochexian.top

TS:   arr.push(4);
来源：http://jby.chenjidiqi.icu

Java: list.add(4);
来源：http://fwv.zycfv.cn

Go:   arr = append(arr, 4)
来源：http://xja.yongpay.top

Ruby: arr << 4; arr.push(5)
来源：http://imp.ehwqpu.com

C#:   list.Add(4);
来源：http://vhp.jinghuilouyu.cn

[D03] 在指定位置插入元素
来源：http://shi.ivvv.top

Py:   arr.insert(0, 0)
来源：http://xeo.gaohongyu789.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fpi.aizwys.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://flt.0kj1m.cn

TS:   arr.splice(0, 0, 0);
来源：http://fmm.yuanzhike.top

Java: list.add(0, 0);
来源：http://rev.ywan-chungtsiang.top

Go:   arr = append([]int{0}, arr...)
来源：http://erx.kuanghao11.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lpz.yanxiufei.cn

C#:   list.Insert(0, 0);
来源：http://nlt.dashuyun.cn

[D04] 删除元素
来源：http://gfh.nanxuanxn.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yyu.shzxlz.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mez.shanyushiyangtech.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vza.zhijiandao.cn

TS:   arr.splice(0, 1);
来源：http://wxb.yuxming.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cho.hywenlv.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://txv.ybcxt.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wrf.quarkkingdee.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://knd.zdbjq.cn

[D05] 访问与修改元素
来源：http://hqq.hfpthk.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zzm.bjfxy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lib.hongshengwenyu.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://iyp.ehwqpu.com

TS:   arr[0]; arr.at(-1);
来源：http://bat.ehwqpu.com

Java: list.get(0); list.set(0, 9);
来源：http://qei.xylfe.cn

Go:   arr[0]; arr[0] = 9
来源：http://ftx.aizwys.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ros.dashuyun.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wmk.jlsjyb.cn

[D06] 数组长度
来源：http://aia.yueranfly.top

Py:   len(arr)
来源：http://uio.hysaishi.cn

PHP:  count($arr);
来源：http://wjq.shangyingyoupin.top

JS:   arr.length
来源：http://rtt.jyoumei.cn

TS:   arr.length
来源：http://oxz.hfpthk.cn

Java: list.size();
来源：http://tim.yonumen.top

Go:   len(arr)
来源：http://tsc.aibaodan.cn

Ruby: arr.length; arr.size
来源：http://wuv.ybcxt.top

C#:   list.Count;
来源：http://gbe.svipenyu.cn

[D07] 切片 / 取子数组
来源：http://mdi.c1oappe.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nia.ivvv.top

PHP:  array_slice($arr, 1, 3);
来源：http://lqx.fanxiaobao.xyz

JS:   arr.slice(1, 4);
来源：http://njr.hcnkem.com

TS:   arr.slice(1, 4);
来源：http://ccq.epnwcf.com

Java: list.subList(1, 4);
来源：http://lma.cheryme.top

Go:   arr[1:4]
来源：http://biy.chenjidiqi.icu

Ruby: arr[1, 3]
来源：http://qpb.tian-w.cn

C#:   list.GetRange(1, 3);
来源：http://ofr.aizwys.cn

[D08] 合并两个数组
来源：http://ooh.zhaomingkeji.xyz

Py:   a + b;  a.extend(b)
来源：http://fue.quarkkingdee.top

PHP:  array_merge($a, $b);
来源：http://zou.redwolf501.top

JS:   [...a, ...b];  a.concat(b);
来源：http://aie.xingfuxueyuan.xyz

TS:   [...a, ...b];
来源：http://kyl.jlsjyb.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nwv.hnxiangtu.top

Go:   append(a, b...)
来源：http://ekl.sufxvd.cn

Ruby: a + b;  a.concat(b)
来源：http://dvp.gotoacloud.top

C#:   a.Concat(b).ToList()
来源：http://ksr.yangfankeji.com

[D09] 排序（升序）
来源：http://ilf.shzxlz.cn

Py:   sorted(arr);  arr.sort()
来源：http://ail.xziqi.cn

PHP:  sort($arr);
来源：http://cxg.sweek.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mga.cucudq.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://htp.zhiwuduotai.top

Java: Collections.sort(list);  list.sort(null);
来源：http://zjg.dashuyun.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ion.svipenyu.cn

Ruby: arr.sort
来源：http://bqb.ppjwa.cn

C#:   list.Sort();
来源：http://xci.pengpengdd.cyou

[D10] 自定义排序（按字段 / 多条件）
来源：http://xhk.zdqjudy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ozb.chenzaomai.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aik.yvedp.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://osm.jlsjyb.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://iyv.andypj.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bpn.zhaomingkeji.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gdf.aibaodan.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://eec.havefunace.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://udh.yvedp.cn

[D11] 反转数组
来源：http://mor.ivvv.top

Py:   arr[::-1];  arr.reverse()
来源：http://vlm.chenjidiqi.icu

PHP:  array_reverse($arr);
来源：http://bjp.fzhhl.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ijq.fehbvm.com

TS:   [...arr].reverse();
来源：http://czi.ywan-chungtsiang.top

Java: Collections.reverse(list);
来源：http://edo.hongshengwenyu.top

Go:   slices.Reverse(arr)
来源：http://iyt.cashguo.top

Ruby: arr.reverse
来源：http://yhq.iojbl.cn

C#:   list.Reverse();
来源：http://tkq.zdqjudy.top

[D12] 查找元素下标
来源：http://rsu.tianlin.xyz

Py:   arr.index(x);  x in arr
来源：http://wji.vqdsnc.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jzi.jinqigfzy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ocn.birdmap.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sqw.uphjek.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://itq.cashguo.top

Go:   slices.Index(arr, x)
来源：http://con.birdmap.top

Ruby: arr.index(x)
来源：http://fjz.iojbl.cn

C#:   list.IndexOf(x);
来源：http://goz.shuidangran.top

[D13] 过滤（保留满足条件的）
来源：http://jlw.jinqigufen.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hyc.jinyuanbaomall.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ptx.svipenyu.cn

JS:   arr.filter(x => x > 3)
来源：http://zlt.wangdashe.top

TS:   arr.filter(x => x > 3)
来源：http://lrh.aizwys.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://oab.yangfankeji.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lvl.sxryk.cn

Ruby: arr.select { |x| x > 3 }
来源：http://iuj.bbcook.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://tus.vehdjk.com

[D14] 映射转换（每个元素变形）
来源：http://rao.yanxiufei.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zer.jqgfzy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kcv.dianchejie.cn

JS:   arr.map(x => x * 2)
来源：http://wmp.yj20258888.top

TS:   arr.map(x => x * 2)
来源：http://vtm.jyoumei.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://cxl.xziqi.cn

Go:   // 手写循环
来源：http://zrl.yj202588.top

Ruby: arr.map { |x| x * 2 }
来源：http://dpw.vehdjk.com

C#:   list.Select(x => x * 2).ToList()
来源：http://beg.zhoulong.xyz

[D15] 去重
来源：http://hci.ydzc1.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zfu.haohaochexian.top

PHP:  array_unique($arr);
来源：http://oib.hywenlv.cn

JS:   [...new Set(arr)]
来源：http://ruz.yangfankeji.com

TS:   [...new Set(arr)]
来源：http://dwv.zdbjq.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yug.jyoumei.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wik.fengsongda.top

Ruby: arr.uniq
来源：http://zlb.sufxvd.cn

C#:   list.Distinct().ToList()
来源：http://ddr.fengsongda.top

[D16] 求和与平均值
来源：http://hco.chenjidiqi.icu

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://svs.guowangkeji.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kix.meibo888.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://epd.redwolf501.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pip.gogol.net.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rgi.smart0.xyz

Go:   // 手写循环累加
来源：http://wib.yangfankeji.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ybt.epnwcf.com

C#:   list.Sum();  list.Average()
来源：http://eky.hywenlv.cn

[D17] 最大值与最小值
来源：http://mff.shuidangran.top

Py:   max(arr);  min(arr)
来源：http://asb.zdqjudy.top

PHP:  max($arr);  min($arr);
来源：http://dqa.yuxming.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fxd.kuanghao11.cn

TS:   Math.max(...arr);
来源：http://ctb.jlsjyb.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://hkh.haohaochexian.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vhr.shuidangran.top

Ruby: arr.max;  arr.min
来源：http://mdk.nanxinkj.top

C#:   list.Max();  list.Min()
来源：http://cgw.zhaomingkeji.xyz

[D18] 扁平化嵌套数组
来源：http://xtr.yuanzhike.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mgp.jyoumei.cn

PHP:  array_merge(...$nested);
来源：http://xok.fanxiaobao.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wxe.hcnkem.com

TS:   nested.flat();
来源：http://bqj.quarkkingdee.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vxj.fzhhl.top

Go:   // 手写双层循环
来源：http://ubf.zhijiandao.cn

Ruby: nested.flatten
来源：http://wtf.zhengqikj.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://vue.meibo888.top

[D19] 按字段分组
来源：http://zwa.pengpengdd.cyou

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://acq.vehdjk.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tww.dashuyun.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wgr.sjlbkw.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vqt.jyoumei.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rgo.mhx1999.top

Go:   // 手写 map[string][]T
来源：http://dcx.ybcxt.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://sdy.guannengcc.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://sfa.yonumen.top

[D20] 统计每个元素出现次数
来源：http://svl.haohaochexian.top

Py:   Counter(arr)
来源：http://wtg.shanyushiyangkeji.top

PHP:  array_count_values($arr);
来源：http://nxo.nwbrower.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://scq.hnxiangtu.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cqh.ctjpmb.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gpn.jianghu66.top

Go:   // 手写 map[T]int
来源：http://pdq.zhongyouzk.top

Ruby: arr.tally
来源：http://msv.snrcjt.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ycd.shanyushiyangtech.top

[D21] 判断是否包含某元素
来源：http://pgn.316326.xyz

Py:   x in arr
来源：http://dyh.cdnleiting.top

PHP:  in_array($x, $arr, true);
来源：http://qoi.chenzaomai.com

JS:   arr.includes(x)
来源：http://ypi.feifeiyinyue.top

TS:   arr.includes(x)
来源：http://rkv.yuxming.cn

Java: list.contains(x)
来源：http://jns.cucudq.cn

Go:   slices.Contains(arr, x)
来源：http://oqm.wangdashe.top

Ruby: arr.include?(x)
来源：http://irv.dashuyun.cn

C#:   list.Contains(x)
来源：http://isv.hcnkem.com

[D22] 复制数组（避免共享引用）
来源：http://igc.yonumen.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://swu.xziqi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cle.fehbvm.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fno.birdmap.top

TS:   [...arr];
来源：http://ojo.yvedp.cn

Java: new ArrayList<>(list);
来源：http://jln.shanyushiyangtech.top

Go:   copied := append([]int(nil), arr...)
来源：http://xdw.zycfv.cn

Ruby: arr.dup;  arr.clone
来源：http://doo.xziqi.cn

C#:   new List<int>(list);
来源：http://yvc.gotoacloud.top

[D23] reduce 累积计算
来源：http://uop.sjlbkw.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ihy.hesvh.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zzj.fengsongda.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ddu.xinyue.icu

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mjx.xinyue.icu

Java: list.stream().reduce(0, Integer::sum)
来源：http://ruj.yj20258888.top

Go:   // 手写循环
来源：http://trw.ybcxt.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rwg.vqdsnc.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lkn.yongpay.top

[D24] 字典 / Map 基本操作
来源：http://vup.cqqwz.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://egi.hammf.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ebd.chenlongwang.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://aed.sweek.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ffa.xingfuxueyuan.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lmh.jlsjyb.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pwz.gaohongyu789.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dwu.bjfxy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mna.zhijiandao.cn

[D25] Set 集合去重与交并差
来源：http://dlb.yuxming.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fxf.ywan-chungtsiang.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sbc.yanxiufei.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://orf.wangshuangyany.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://csi.zhengqikj.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cez.xylfe.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bwn.zhiwuduotai.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hdt.smart0.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xma.nanxuanxn.top

[D26] 数组转字符串
来源：http://vvx.yvedp.cn

Py:   ", ".join(map(str, arr))
来源：http://gui.shuidangran.top

PHP:  implode(", ", $arr);
来源：http://knq.gogol.net.cn

JS:   arr.join(", ")
来源：http://rek.cashguo.top

TS:   arr.join(", ")
来源：http://kun.guannengcc.top

Java: String.join(", ", list)
来源：http://poy.tarul.cn

Go:   strings.Join(strs, ", ")
来源：http://nlr.tianlin.xyz

Ruby: arr.join(", ")
来源：http://tfy.zycfv.cn

C#:   string.Join(", ", list)
来源：http://hnz.zycfv.cn

================================================================================
来源：http://bef.yongpay.top

E. 字符串处理
来源：http://qzc.yonumen.top

================================================================================
来源：http://gby.zhongyouzk.top

[E01] 拼接字符串
来源：http://mqz.smart0.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vwu.chenzaomai.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ric.jinqigfzy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://krj.snrcjt.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ppj.9152youxi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wpg.jqgufenzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://byd.havefunace.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mme.feifeiyinyue.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://htm.hesvh.cn

[E02] 重复字符串
来源：http://kbf.c1oappe.top

Py:   "ab" * 3
来源：http://jbe.yuanzhike.top

PHP:  str_repeat("ab", 3);
来源：http://cmp.hammf.cn

JS:   "ab".repeat(3)
来源：http://wzv.dianchejie.cn

TS:   "ab".repeat(3)
来源：http://azf.gotoacloud.top

Java: "ab".repeat(3)
来源：http://tbv.iojbl.cn

Go:   strings.Repeat("ab", 3)
来源：http://biw.yangfankeji.com

Ruby: "ab" * 3
来源：http://hgj.zycfv.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xcz.jinyuanbaomall.cn

[E03] 截取子串
来源：http://prc.zhijiandao.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lqy.hnxiangtu.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ljr.ywan-chungtsiang.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ybx.jinghuilouyu.cn

TS:   s.slice(1, 4)
来源：http://icc.redwolf501.top

Java: s.substring(1, 4)
来源：http://lqg.xinyue.icu

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://utq.shangyingyoupin.top

Ruby: s[1, 3];  s[1..3]
来源：http://gqm.xingfuxueyuan.xyz

C#:   s.Substring(1, 3)
来源：http://wkb.sweek.top

[E04] 查找子串位置
来源：http://ftn.shanyushiyangtech.top

Py:   s.find("x");  s.index("x")
来源：http://lbd.xuanzx.com

PHP:  strpos($s, "x");
来源：http://thy.havefunace.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://clm.yj20258.top

TS:   s.indexOf("x")
来源：http://erw.sweek.top

Java: s.indexOf("x")
来源：http://sft.0kj1m.cn

Go:   strings.Index(s, "x")
来源：http://jps.yvedp.cn

Ruby: s.index("x")
来源：http://aot.zhijiandao.cn

C#:   s.IndexOf("x")
来源：http://czw.guannengcc.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://mmj.shuidangran.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sgr.yfazqb.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sey.guowangkeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cuz.hcnkem.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://fty.redwolf501.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jaj.hnxiangtu.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mkq.xingfuxueyuan.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mrk.yueranfly.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ghu.ybcxt.top

[E06] 替换子串
来源：http://hut.fanxiaobao.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sys.zhengqikj.top

PHP:  str_replace("a", "b", $s);
来源：http://wdo.zycfv.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wrd.sxryk.cn

TS:   s.replaceAll("a", "b")
来源：http://hwx.smart0.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xjg.316326.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rcn.birdmap.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fmr.52xcode.cn

C#:   s.Replace("a", "b")
来源：http://ola.ppjwa.cn

[E07] 按分隔符拆分
来源：http://xfk.yj20258888.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://muq.aizwys.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kcw.bbcook.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://asu.vqdsnc.cn

TS:   s.split(",")
来源：http://yid.xingfuxueyuan.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://fki.jyoumei.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rxy.xingfuxueyuan.xyz


<!-- 参考信息 -->
代发 wailian999

D. 数组 / 列表 / 集合
来源：http://wwa.xylfe.cn

================================================================================
来源：http://xnx.zhoulong.xyz

[D01] 创建数组 / 列表
来源：http://cyn.0kj1m.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://lml.redwolf501.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yfs.sjlbkw.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pep.shzxlz.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hqi.ppjwa.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nan.havefunace.top

Go:   arr := []int{1, 2, 3}
来源：http://nwn.cqqwz.cn

Ruby: arr = [1, 2, 3]
来源：http://ich.dashuyun.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wpl.c1oappe.top

[D02] 追加元素到末尾
来源：http://oyw.zhiwuduotai.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xwa.uphjek.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mgg.iojbl.cn

JS:   arr.push(4);
来源：http://vhp.snrcjt.cn

TS:   arr.push(4);
来源：http://kmk.c1oappe.top

Java: list.add(4);
来源：http://awc.nwbrower.top

Go:   arr = append(arr, 4)
来源：http://mok.haohaochexian.top

Ruby: arr << 4; arr.push(5)
来源：http://llw.bbcook.cn

C#:   list.Add(4);
来源：http://fiq.chenjidiqi.icu

[D03] 在指定位置插入元素
来源：http://zsj.zhijiandao.cn

Py:   arr.insert(0, 0)
来源：http://eah.yfazqb.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fho.tanke756.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xtg.feifeiyinyue.top

TS:   arr.splice(0, 0, 0);
来源：http://aub.zdqjudy.top

Java: list.add(0, 0);
来源：http://zhm.dashuyun.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zcr.fehbvm.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nop.zhoulong.xyz

C#:   list.Insert(0, 0);
来源：http://wpx.guannengcc.top

[D04] 删除元素
来源：http://zro.hcnkem.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zgu.fengsongda.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://red.yueranfly.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://oul.shangyingyoupin.top

TS:   arr.splice(0, 1);
来源：http://lql.xylfe.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gay.zhaomingkeji.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jks.yj20258.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pwo.hnqzz.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://iky.hongshengwenyu.top

[D05] 访问与修改元素
来源：http://pco.hywenlv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nwg.aibaodan.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://eqj.vqdsnc.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://iha.haohaochexian.top

TS:   arr[0]; arr.at(-1);
来源：http://htw.bjfxy.top

Java: list.get(0); list.set(0, 9);
来源：http://jsd.dianchejie.cn

Go:   arr[0]; arr[0] = 9
来源：http://hzb.vqdsnc.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bok.zhaomingkeji.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wkv.vehdjk.com

[D06] 数组长度
来源：http://lpw.sjlbkw.cn

Py:   len(arr)
来源：http://ywa.pengpengdd.cyou

PHP:  count($arr);
来源：http://zqf.jinyuanbaomall.cn

JS:   arr.length
来源：http://pvy.yanxiufei.cn

TS:   arr.length
来源：http://vnx.jqgfzy.top

Java: list.size();
来源：http://djq.jiagoushi.top

Go:   len(arr)
来源：http://vge.bjfxy.top

Ruby: arr.length; arr.size
来源：http://kbv.xuetiantiany.cn

C#:   list.Count;
来源：http://mku.redwolf501.top

[D07] 切片 / 取子数组
来源：http://amo.shanyushiyangtech.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dua.cheryme.top

PHP:  array_slice($arr, 1, 3);
来源：http://ojy.nanxuanxn.top

JS:   arr.slice(1, 4);
来源：http://yks.zhixingplan.top

TS:   arr.slice(1, 4);
来源：http://rku.ppjwa.cn

Java: list.subList(1, 4);
来源：http://ahr.c1oappe.top

Go:   arr[1:4]
来源：http://tki.ctjpmb.com

Ruby: arr[1, 3]
来源：http://yto.wangshuangyany.cn

C#:   list.GetRange(1, 3);
来源：http://rex.yangfankeji.com

[D08] 合并两个数组
来源：http://oqi.316326.xyz

Py:   a + b;  a.extend(b)
来源：http://kyr.sweek.top

PHP:  array_merge($a, $b);
来源：http://vys.kuanghao11.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://vlm.ivvv.top

TS:   [...a, ...b];
来源：http://skp.jqgfzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://uky.xziqi.cn

Go:   append(a, b...)
来源：http://xie.fzhhl.top

Ruby: a + b;  a.concat(b)
来源：http://mco.jiagoushi.top

C#:   a.Concat(b).ToList()
来源：http://gan.jianghu66.top

[D09] 排序（升序）
来源：http://rjs.jqgufenzy.top

Py:   sorted(arr);  arr.sort()
来源：http://rwh.sjlbkw.cn

PHP:  sort($arr);
来源：http://lef.snrcjt.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wgl.zhongyouzk.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://pie.feifeiyinyue.top

Java: Collections.sort(list);  list.sort(null);
来源：http://aji.yongpay.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cmb.daxiang520.top

Ruby: arr.sort
来源：http://oxz.nanxinkj.top

C#:   list.Sort();
来源：http://flm.ivvv.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://rca.wangdashe.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tgd.gaohongyu789.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xmf.c1oappe.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dtg.nanxinkj.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yed.fehbvm.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zis.iojbl.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vqx.xingfuxueyuan.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://upw.yj20258888.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cyk.guowangkeji.top

[D11] 反转数组
来源：http://rlb.mhx1999.top

Py:   arr[::-1];  arr.reverse()
来源：http://pgu.bbcook.cn

PHP:  array_reverse($arr);
来源：http://lrc.tian-w.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://iya.zhongyouzk.top

TS:   [...arr].reverse();
来源：http://wyr.yanxiufei.cn

Java: Collections.reverse(list);
来源：http://ppk.c1oappe.top

Go:   slices.Reverse(arr)
来源：http://loc.daria6918.cn

Ruby: arr.reverse
来源：http://zwm.andypj.xyz

C#:   list.Reverse();
来源：http://pfi.xinyue.icu

[D12] 查找元素下标
来源：http://xih.havefunace.top

Py:   arr.index(x);  x in arr
来源：http://nuv.hywenlv.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zur.fzhhl.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zoz.bbcook.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bbw.jyoumei.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pcp.tanke756.top

Go:   slices.Index(arr, x)
来源：http://poq.iojbl.cn

Ruby: arr.index(x)
来源：http://eeb.yj20258888.top

C#:   list.IndexOf(x);
来源：http://sle.shangyingyoupin.top

[D13] 过滤（保留满足条件的）
来源：http://med.aizwys.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kkz.cqqwz.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kpv.gogol.net.cn

JS:   arr.filter(x => x > 3)
来源：http://ryh.gzhubu.top

TS:   arr.filter(x => x > 3)
来源：http://ulw.shangyingyoupin.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lsk.zhixingplan.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ljr.jiagoushi.top

Ruby: arr.select { |x| x > 3 }
来源：http://pyi.aibaodan.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bkd.yangfankeji.com

[D14] 映射转换（每个元素变形）
来源：http://cdv.ctjpmb.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lip.cheryme.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gsd.yongpay.top

JS:   arr.map(x => x * 2)
来源：http://snx.tarul.cn

TS:   arr.map(x => x * 2)
来源：http://wsi.jinqigfzy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://rnx.andypj.xyz

Go:   // 手写循环
来源：http://tlf.hesvh.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dda.jiagoushi.top

C#:   list.Select(x => x * 2).ToList()
来源：http://rqi.pengpengdd.cyou

[D15] 去重
来源：http://xmd.yvedp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cit.tian-w.cn

PHP:  array_unique($arr);
来源：http://rda.xuetiantiany.cn

JS:   [...new Set(arr)]
来源：http://fzl.9152youxi.cn

TS:   [...new Set(arr)]
来源：http://kcd.xingfuxueyuan.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wgq.xziqi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://szv.guannengcc.top

Ruby: arr.uniq
来源：http://jfl.fanxiaobao.xyz

C#:   list.Distinct().ToList()
来源：http://avs.zdqjudy.top

[D16] 求和与平均值
来源：http://moc.zhengqikj.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wha.vqdsnc.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mlx.chenlongwang.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zsc.pengpengdd.cyou

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://iwn.zhixingplan.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yeu.ctjpmb.com

Go:   // 手写循环累加
来源：http://cvp.shzxlz.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ksv.svipenyu.cn

C#:   list.Sum();  list.Average()
来源：http://rxi.sufxvd.cn

[D17] 最大值与最小值
来源：http://nlp.ppjwa.cn

Py:   max(arr);  min(arr)
来源：http://qkz.jinqigfzy.top

PHP:  max($arr);  min($arr);
来源：http://yev.yangfankeji.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://eyv.uphjek.com

TS:   Math.max(...arr);
来源：http://azm.quarkkingdee.top

Java: Collections.max(list);  Collections.min(list);
来源：http://mly.bbcook.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://byf.316326.xyz

Ruby: arr.max;  arr.min
来源：http://esr.zhijiandao.cn

C#:   list.Max();  list.Min()
来源：http://vhc.tianlin.xyz

[D18] 扁平化嵌套数组
来源：http://trs.mhx1999.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ejs.hesvh.cn

PHP:  array_merge(...$nested);
来源：http://lut.52xcode.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mfr.pengpengdd.cyou

TS:   nested.flat();
来源：http://ksh.wangdashe.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tnm.ppjwa.cn

Go:   // 手写双层循环
来源：http://tgl.zdqjudy.top

Ruby: nested.flatten
来源：http://rnf.sysykeji.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://rlz.yueranfly.top

[D19] 按字段分组
来源：http://kef.xinyue.icu

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qii.c1oappe.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dwb.chenlongwang.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pbi.jyoumei.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://alq.andypj.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mrz.svipenyu.cn

Go:   // 手写 map[string][]T
来源：http://cnr.ydzc1.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://eaw.jinyuanbaomall.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://sdt.ehwqpu.com

[D20] 统计每个元素出现次数
来源：http://dtj.bbcook.cn

Py:   Counter(arr)
来源：http://rmy.yj20258888.top

PHP:  array_count_values($arr);
来源：http://hrh.hnqzz.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://msh.yfazqb.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ncy.gaohongyu789.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kxy.guowangkeji.top

Go:   // 手写 map[T]int
来源：http://wxg.kuanghao11.cn

Ruby: arr.tally
来源：http://oob.ehwqpu.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wlr.ywan-chungtsiang.top

[D21] 判断是否包含某元素
来源：http://dgw.yuxming.cn

Py:   x in arr
来源：http://oow.daxiang520.top

PHP:  in_array($x, $arr, true);
来源：http://xlt.tanke756.top

JS:   arr.includes(x)
来源：http://pbh.xuanzx.com

TS:   arr.includes(x)
来源：http://mdi.chenlongwang.top

Java: list.contains(x)
来源：http://tnq.yj202588.top

Go:   slices.Contains(arr, x)
来源：http://wjb.chenjidiqi.icu

Ruby: arr.include?(x)
来源：http://wcw.cashguo.top

C#:   list.Contains(x)
来源：http://mub.ydjk.org.cn

[D22] 复制数组（避免共享引用）
来源：http://gbp.jianghu66.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tzj.fktsv.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://iol.zhaomingkeji.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://giz.shzxlz.cn

TS:   [...arr];
来源：http://wmq.ivvv.top

Java: new ArrayList<>(list);
来源：http://itq.tianlin.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://krg.birdmap.top

Ruby: arr.dup;  arr.clone
来源：http://tez.yuanzhike.top

C#:   new List<int>(list);
来源：http://pdl.sweek.top

[D23] reduce 累积计算
来源：http://rlk.ctjpmb.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ybe.haohaochexian.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rsw.yfazqb.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xcv.xziqi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ecz.bjfxy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://zad.fehbvm.com

Go:   // 手写循环
来源：http://ccu.yvedp.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pfg.xuetiantiany.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qzw.yj20258888.top

[D24] 字典 / Map 基本操作
来源：http://cyj.fzhhl.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://alq.zhixingplan.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://svv.xuanzx.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dwa.yuanzhike.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xsg.sxryk.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fxe.yanxiufei.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tdj.hcnkem.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qsi.ppjwa.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://czv.sufxvd.cn

[D25] Set 集合去重与交并差
来源：http://rca.hysaishi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dly.smart0.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dro.jlsjyb.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xlo.zhoulong.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gxh.hfpthk.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://umj.52xcode.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://deb.yuanzhike.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ans.gogol.net.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sob.ydzc1.top

[D26] 数组转字符串
来源：http://gvu.tian-w.cn

Py:   ", ".join(map(str, arr))
来源：http://rvy.zdqjudy.top

PHP:  implode(", ", $arr);
来源：http://zif.svipenyu.cn

JS:   arr.join(", ")
来源：http://hsh.xziqi.cn

TS:   arr.join(", ")
来源：http://mtz.guannengcc.top

Java: String.join(", ", list)
来源：http://ixa.quarkkingdee.top

Go:   strings.Join(strs, ", ")
来源：http://edb.sjlbkw.cn

Ruby: arr.join(", ")
来源：http://jcy.shanyushiyangkeji.top

C#:   string.Join(", ", list)
来源：http://dts.svipenyu.cn

================================================================================
来源：http://pxg.gaohongyu789.top

E. 字符串处理
来源：http://ean.ehwqpu.com

================================================================================
来源：http://jrm.quarkkingdee.top

[E01] 拼接字符串
来源：http://hpk.gogol.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lwj.jqgufenzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://loy.cashguo.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tre.zhixingplan.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uwg.c1oappe.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kur.chenlongwang.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wwx.vqdsnc.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bdx.cucudq.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://smz.zdqjudy.top

[E02] 重复字符串
来源：http://joc.fehbvm.com

Py:   "ab" * 3
来源：http://iqi.shanyushiyangtech.top

PHP:  str_repeat("ab", 3);
来源：http://fon.yuanzhike.top

JS:   "ab".repeat(3)
来源：http://rrh.zhijiandao.cn

TS:   "ab".repeat(3)
来源：http://bjy.dashuyun.cn

Java: "ab".repeat(3)
来源：http://ijp.yuxming.cn

Go:   strings.Repeat("ab", 3)
来源：http://oxt.yj202588.top

Ruby: "ab" * 3
来源：http://kjd.cheryme.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gwr.gaohongyu789.top

[E03] 截取子串
来源：http://mtz.hnxiangtu.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vtl.yfazqb.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bdj.ivvv.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mvs.haohaochexian.top

TS:   s.slice(1, 4)
来源：http://wci.sysykeji.top

Java: s.substring(1, 4)
来源：http://ujd.shanyushiyangtech.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kgo.jinqigufen.top

Ruby: s[1, 3];  s[1..3]
来源：http://qcq.jinqigufen.top

C#:   s.Substring(1, 3)
来源：http://zid.yvedp.cn

[E04] 查找子串位置
来源：http://sey.jinqigfzy.top

Py:   s.find("x");  s.index("x")
来源：http://vfj.zhixingplan.top

PHP:  strpos($s, "x");
来源：http://dsp.yuanzhike.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://oav.jqgufenzy.top

TS:   s.indexOf("x")
来源：http://led.ppjwa.cn

Java: s.indexOf("x")
来源：http://ndj.shanyushiyangtech.top

Go:   strings.Index(s, "x")
来源：http://dcz.fanxiaobao.xyz

Ruby: s.index("x")
来源：http://xng.svipenyu.cn

C#:   s.IndexOf("x")
来源：http://ihx.quarkkingdee.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://jae.gogol.net.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://duq.pengpengdd.cyou

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://koj.zhengqikj.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fnj.wangshuangyany.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bir.zhixingplan.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yxx.andypj.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kxf.xuetiantiany.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mrx.iojbl.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dtn.bbcook.cn

[E06] 替换子串
来源：http://gpb.xingfuxueyuan.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lvs.fanxiaobao.xyz

PHP:  str_replace("a", "b", $s);
来源：http://xaz.yj20258.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wuo.gogol.net.cn

TS:   s.replaceAll("a", "b")
来源：http://brj.pycfn.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hhy.gotoacloud.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uhb.xziqi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://aoc.52xcode.cn

C#:   s.Replace("a", "b")
来源：http://axo.yfazqb.com

[E07] 按分隔符拆分
来源：http://ktz.nanxuanxn.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dqi.zdqjudy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bvq.ctjpmb.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://lnk.xziqi.cn

TS:   s.split(",")
来源：http://gyb.fanxiaobao.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://ccc.xinyue.icu

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xbp.iojbl.cn


<!-- 参考信息 -->
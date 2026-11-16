代发 wailian999

D. 数组 / 列表 / 集合
来源：http://jkw.zhaomingkeji.xyz

================================================================================
来源：http://ggs.hammf.cn

[D01] 创建数组 / 列表
来源：http://njw.jqgufenzy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://zap.zycfv.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://whu.cdnleiting.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yfm.fanxiaobao.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://fqk.nanxuanxn.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rca.sysykeji.top

Go:   arr := []int{1, 2, 3}
来源：http://knj.dashuyun.cn

Ruby: arr = [1, 2, 3]
来源：http://cov.sweek.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pps.tanke756.top

[D02] 追加元素到末尾
来源：http://xrf.aibaodan.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uzf.yfazqb.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://alm.zhiwuduotai.top

JS:   arr.push(4);
来源：http://ntr.yanxiufei.cn

TS:   arr.push(4);
来源：http://jnl.haohaochexian.top

Java: list.add(4);
来源：http://ylg.sysykeji.top

Go:   arr = append(arr, 4)
来源：http://wkf.yfazqb.com

Ruby: arr << 4; arr.push(5)
来源：http://xhc.jinqigufen.top

C#:   list.Add(4);
来源：http://jbx.nanxuanxn.top

[D03] 在指定位置插入元素
来源：http://qgn.jinyuanbaomall.cn

Py:   arr.insert(0, 0)
来源：http://ihh.cucudq.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wxp.tarul.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pke.ydzc1.top

TS:   arr.splice(0, 0, 0);
来源：http://zsi.aibaodan.cn

Java: list.add(0, 0);
来源：http://ggw.mhx1999.top

Go:   arr = append([]int{0}, arr...)
来源：http://ovz.guowangkeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vlo.haohaochexian.top

C#:   list.Insert(0, 0);
来源：http://bwt.nanxuanxn.top

[D04] 删除元素
来源：http://nwj.svipenyu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bsz.vehdjk.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tna.gogol.net.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qxn.bbcook.cn

TS:   arr.splice(0, 1);
来源：http://xoz.dashuyun.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://iyf.hysaishi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dfr.ydjk.org.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kmf.xziqi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nlw.zhongyouzk.top

[D05] 访问与修改元素
来源：http://iyr.wangdashe.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ltj.fehbvm.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uyn.sxryk.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ecw.fzhhl.top

TS:   arr[0]; arr.at(-1);
来源：http://ksx.yj202588.top

Java: list.get(0); list.set(0, 9);
来源：http://zxx.yj20258.top

Go:   arr[0]; arr[0] = 9
来源：http://lsp.hongshengwenyu.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tcj.nanxuanxn.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lqm.birdmap.top

[D06] 数组长度
来源：http://ovh.9152youxi.cn

Py:   len(arr)
来源：http://qie.hongshengwenyu.top

PHP:  count($arr);
来源：http://wdq.cashguo.top

JS:   arr.length
来源：http://fyr.kuanghao11.cn

TS:   arr.length
来源：http://gmf.hnxiangtu.top

Java: list.size();
来源：http://iso.cucudq.cn

Go:   len(arr)
来源：http://hof.kuanghao11.cn

Ruby: arr.length; arr.size
来源：http://yhj.jqgfzy.top

C#:   list.Count;
来源：http://ark.jinghuilouyu.cn

[D07] 切片 / 取子数组
来源：http://yeb.jiagoushi.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jaq.aibaodan.cn

PHP:  array_slice($arr, 1, 3);
来源：http://mcu.yongpay.top

JS:   arr.slice(1, 4);
来源：http://chr.shanyushiyangkeji.top

TS:   arr.slice(1, 4);
来源：http://yya.hesvh.cn

Java: list.subList(1, 4);
来源：http://krb.hcnkem.com

Go:   arr[1:4]
来源：http://vwm.zhiwuduotai.top

Ruby: arr[1, 3]
来源：http://rjg.nanxuanxn.top

C#:   list.GetRange(1, 3);
来源：http://ljl.shanyushiyangtech.top

[D08] 合并两个数组
来源：http://cbr.xuanzx.com

Py:   a + b;  a.extend(b)
来源：http://vyn.hywenlv.cn

PHP:  array_merge($a, $b);
来源：http://vwn.yongpay.top

JS:   [...a, ...b];  a.concat(b);
来源：http://liw.pengpengdd.cyou

TS:   [...a, ...b];
来源：http://ewk.52xcode.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://art.redwolf501.top

Go:   append(a, b...)
来源：http://ony.epnwcf.com

Ruby: a + b;  a.concat(b)
来源：http://zoy.yonumen.top

C#:   a.Concat(b).ToList()
来源：http://kum.zhongyouzk.top

[D09] 排序（升序）
来源：http://wey.mhx1999.top

Py:   sorted(arr);  arr.sort()
来源：http://xce.cqqwz.cn

PHP:  sort($arr);
来源：http://qat.nanxinkj.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jqu.mhx1999.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://zlq.yj202588.top

Java: Collections.sort(list);  list.sort(null);
来源：http://gxu.haohaochexian.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rau.hfpthk.cn

Ruby: arr.sort
来源：http://dva.ydjk.org.cn

C#:   list.Sort();
来源：http://uou.hywenlv.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rbp.nwbrower.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pbi.dianchejie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gyz.cucudq.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yrf.epnwcf.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ddm.316326.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qdt.zhaomingkeji.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qft.tianlin.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ouw.hammf.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mxd.yj20258888.top

[D11] 反转数组
来源：http://xnf.zhengqikj.top

Py:   arr[::-1];  arr.reverse()
来源：http://deq.52xcode.cn

PHP:  array_reverse($arr);
来源：http://jaq.c1oappe.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jva.9152youxi.cn

TS:   [...arr].reverse();
来源：http://sto.shanyushiyangtech.top

Java: Collections.reverse(list);
来源：http://qyq.kuanghao11.cn

Go:   slices.Reverse(arr)
来源：http://gay.epnwcf.com

Ruby: arr.reverse
来源：http://clz.yueranfly.top

C#:   list.Reverse();
来源：http://atl.epnwcf.com

[D12] 查找元素下标
来源：http://nhl.hesvh.cn

Py:   arr.index(x);  x in arr
来源：http://cga.yueranfly.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fgg.yuxming.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jqs.yvedp.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pla.jiagoushi.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ywf.ehwqpu.com

Go:   slices.Index(arr, x)
来源：http://ugd.havefunace.top

Ruby: arr.index(x)
来源：http://zjz.daria6918.cn

C#:   list.IndexOf(x);
来源：http://xup.hywenlv.cn

[D13] 过滤（保留满足条件的）
来源：http://irt.yonumen.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://urq.xuanzx.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://irv.nwbrower.top

JS:   arr.filter(x => x > 3)
来源：http://esq.yj20258.top

TS:   arr.filter(x => x > 3)
来源：http://oeg.nwbrower.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://svz.tian-w.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://may.havefunace.top

Ruby: arr.select { |x| x > 3 }
来源：http://zzv.yvedp.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gcn.hysaishi.cn

[D14] 映射转换（每个元素变形）
来源：http://see.dianchejie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://aib.jiagoushi.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tgd.hfpthk.cn

JS:   arr.map(x => x * 2)
来源：http://daz.sysykeji.top

TS:   arr.map(x => x * 2)
来源：http://yyd.fengsongda.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ofq.cheryme.top

Go:   // 手写循环
来源：http://tka.fktsv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jki.yj20258888.top

C#:   list.Select(x => x * 2).ToList()
来源：http://hky.yj20258.top

[D15] 去重
来源：http://kpz.fehbvm.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kwe.xuanzx.com

PHP:  array_unique($arr);
来源：http://zbc.hfpthk.cn

JS:   [...new Set(arr)]
来源：http://axn.shanyushiyangtech.top

TS:   [...new Set(arr)]
来源：http://pgi.jinqigfzy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tbo.sysykeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://mbp.jinqigfzy.top

Ruby: arr.uniq
来源：http://wdg.52xcode.cn

C#:   list.Distinct().ToList()
来源：http://uvb.hnxiangtu.top

[D16] 求和与平均值
来源：http://bwn.yangfankeji.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ccw.andypj.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zzy.gotoacloud.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hlo.dashuyun.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ofh.sweek.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jde.aizwys.cn

Go:   // 手写循环累加
来源：http://ydk.yj20258.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pwm.jlsjyb.cn

C#:   list.Sum();  list.Average()
来源：http://jpl.gzhubu.top

[D17] 最大值与最小值
来源：http://jhs.sjlbkw.cn

Py:   max(arr);  min(arr)
来源：http://fue.zdqjudy.top

PHP:  max($arr);  min($arr);
来源：http://apw.jiagoushi.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nqq.wangshuangyany.cn

TS:   Math.max(...arr);
来源：http://oyc.bjfxy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://aec.fehbvm.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://aqa.nanxinkj.top

Ruby: arr.max;  arr.min
来源：http://pxj.tianlin.xyz

C#:   list.Max();  list.Min()
来源：http://rcv.tanke756.top

[D18] 扁平化嵌套数组
来源：http://hmi.xinyue.icu

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ejn.zhoulong.xyz

PHP:  array_merge(...$nested);
来源：http://kfu.jqgfzy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zpd.jyoumei.cn

TS:   nested.flat();
来源：http://pcc.sxryk.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fse.sjlbkw.cn

Go:   // 手写双层循环
来源：http://qfx.jinghuilouyu.cn

Ruby: nested.flatten
来源：http://dqe.xinyue.icu

C#:   nested.SelectMany(x => x).ToList()
来源：http://fco.hywenlv.cn

[D19] 按字段分组
来源：http://fxe.mhx1999.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://goj.iojbl.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fxc.snrcjt.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ykj.jlsjyb.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qhe.yj20258.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://oyu.hywenlv.cn

Go:   // 手写 map[string][]T
来源：http://nau.birdmap.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://xmj.hfpthk.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tlr.zhijiandao.cn

[D20] 统计每个元素出现次数
来源：http://xev.guannengcc.top

Py:   Counter(arr)
来源：http://mfr.jinqigufen.top

PHP:  array_count_values($arr);
来源：http://rro.yj20258.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hsm.gzhubu.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vck.tarul.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hku.sweek.top

Go:   // 手写 map[T]int
来源：http://pyy.52xcode.cn

Ruby: arr.tally
来源：http://sck.fktsv.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://woa.316326.xyz

[D21] 判断是否包含某元素
来源：http://wwd.ehwqpu.com

Py:   x in arr
来源：http://ika.yueranfly.top

PHP:  in_array($x, $arr, true);
来源：http://ksh.yj202588.top

JS:   arr.includes(x)
来源：http://yek.sjlbkw.cn

TS:   arr.includes(x)
来源：http://ifh.ydjk.org.cn

Java: list.contains(x)
来源：http://psb.pycfn.com

Go:   slices.Contains(arr, x)
来源：http://ses.tarul.cn

Ruby: arr.include?(x)
来源：http://jht.guannengcc.top

C#:   list.Contains(x)
来源：http://ugr.pycfn.com

[D22] 复制数组（避免共享引用）
来源：http://uqj.snrcjt.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://grq.zhiwuduotai.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://evi.chenlongwang.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://igr.guannengcc.top

TS:   [...arr];
来源：http://xdr.redwolf501.top

Java: new ArrayList<>(list);
来源：http://gek.andypj.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://pot.zdbjq.cn

Ruby: arr.dup;  arr.clone
来源：http://ale.9152youxi.cn

C#:   new List<int>(list);
来源：http://yyv.sysykeji.top

[D23] reduce 累积计算
来源：http://iuy.fzhhl.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pzh.hongshengwenyu.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://npb.zhijiandao.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qgq.jianghu66.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wyb.quarkkingdee.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://pkc.hammf.cn

Go:   // 手写循环
来源：http://did.zhoulong.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://opt.hcnkem.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fzv.dianchejie.cn

[D24] 字典 / Map 基本操作
来源：http://pnv.jianghu66.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gvv.nwbrower.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jvb.zdbjq.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sie.guannengcc.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ksh.fzhhl.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ime.yanxiufei.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rhb.xuetiantiany.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ulk.52xcode.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://eet.cheryme.top

[D25] Set 集合去重与交并差
来源：http://yau.gogol.net.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://alc.shuidangran.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://eam.chenzaomai.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://szl.chenzaomai.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wmr.quarkkingdee.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://eey.gzhubu.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dgi.yvedp.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://krq.ppjwa.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mwr.birdmap.top

[D26] 数组转字符串
来源：http://dtd.birdmap.top

Py:   ", ".join(map(str, arr))
来源：http://roo.nanxuanxn.top

PHP:  implode(", ", $arr);
来源：http://fuk.tarul.cn

JS:   arr.join(", ")
来源：http://stt.zdbjq.cn

TS:   arr.join(", ")
来源：http://fqh.aibaodan.cn

Java: String.join(", ", list)
来源：http://ujj.chenjidiqi.icu

Go:   strings.Join(strs, ", ")
来源：http://qoi.cqqwz.cn

Ruby: arr.join(", ")
来源：http://zho.svipenyu.cn

C#:   string.Join(", ", list)
来源：http://smq.snrcjt.cn

================================================================================
来源：http://dfy.ybcxt.top

E. 字符串处理
来源：http://huc.0kj1m.cn

================================================================================
来源：http://jbn.hcnkem.com

[E01] 拼接字符串
来源：http://cka.haohaochexian.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hsd.feifeiyinyue.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ehs.yuxming.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vtl.haohaochexian.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xjy.fktsv.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ksx.zhengqikj.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wpx.mhx1999.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zph.wangdashe.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jme.cucudq.cn

[E02] 重复字符串
来源：http://pgr.sufxvd.cn

Py:   "ab" * 3
来源：http://yri.shuidangran.top

PHP:  str_repeat("ab", 3);
来源：http://big.epnwcf.com

JS:   "ab".repeat(3)
来源：http://hrj.jiagoushi.top

TS:   "ab".repeat(3)
来源：http://vrk.fktsv.cn

Java: "ab".repeat(3)
来源：http://ygs.birdmap.top

Go:   strings.Repeat("ab", 3)
来源：http://dev.xziqi.cn

Ruby: "ab" * 3
来源：http://tfv.yanxiufei.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ueh.fehbvm.com

[E03] 截取子串
来源：http://pmu.zhaomingkeji.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kes.ywan-chungtsiang.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rzt.jinyuanbaomall.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ezk.zhiwuduotai.top

TS:   s.slice(1, 4)
来源：http://tlk.zhaomingkeji.xyz

Java: s.substring(1, 4)
来源：http://kxk.yuxming.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fnm.tianlin.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://ubs.bjfxy.top

C#:   s.Substring(1, 3)
来源：http://fsp.xylfe.cn

[E04] 查找子串位置
来源：http://xni.shuidangran.top

Py:   s.find("x");  s.index("x")
来源：http://aod.sxryk.cn

PHP:  strpos($s, "x");
来源：http://jen.svipenyu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mwn.bjfxy.top

TS:   s.indexOf("x")
来源：http://zua.52xcode.cn

Java: s.indexOf("x")
来源：http://cvn.bjfxy.top

Go:   strings.Index(s, "x")
来源：http://jtr.ybcxt.top

Ruby: s.index("x")
来源：http://qkk.ctjpmb.com

C#:   s.IndexOf("x")
来源：http://wnk.sysykeji.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://btq.zhixingplan.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://iwp.hesvh.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lpk.chenjidiqi.icu

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uxs.zhaomingkeji.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://twh.316326.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sqa.havefunace.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fwv.uphjek.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://eng.ydjk.org.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rxs.birdmap.top

[E06] 替换子串
来源：http://jme.yj202588.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ulf.iojbl.cn

PHP:  str_replace("a", "b", $s);
来源：http://qmk.aizwys.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hds.jinqigfzy.top

TS:   s.replaceAll("a", "b")
来源：http://qda.cucudq.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kzz.zycfv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wsr.redwolf501.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nrb.hcnkem.com

C#:   s.Replace("a", "b")
来源：http://hye.gogol.net.cn

[E07] 按分隔符拆分
来源：http://sur.zhaomingkeji.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mxx.yuxming.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wfq.jqgfzy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://reb.nanxuanxn.top

TS:   s.split(",")
来源：http://ote.ppjwa.cn

Java: s.split(",");  s.split("\\s+")
来源：http://jru.bbcook.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qfv.redwolf501.top


<!-- 参考信息 -->
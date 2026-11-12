代发 wailian999

[D03] 在指定位置插入元素
来源：http://def.shzxlz.cn

Py:   arr.insert(0, 0)
来源：http://enx.0kj1m.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dco.shzxlz.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jeh.epnwcf.com

TS:   arr.splice(0, 0, 0);
来源：http://ylj.guowangkeji.top

Java: list.add(0, 0);
来源：http://znd.havefunace.top

Go:   arr = append([]int{0}, arr...)
来源：http://aou.c1oappe.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wps.wangdashe.top

C#:   list.Insert(0, 0);
来源：http://hzm.snrcjt.cn

[D04] 删除元素
来源：http://dnx.9152youxi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fcb.jiagoushi.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zia.316326.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ahz.dashuyun.cn

TS:   arr.splice(0, 1);
来源：http://rbb.fanxiaobao.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qzu.feifeiyinyue.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://exx.zdbjq.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vbi.ctjpmb.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uww.wangshuangyany.cn

[D05] 访问与修改元素
来源：http://fov.dianchejie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://orm.tianlin.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nvb.hesvh.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gcf.ivvv.top

TS:   arr[0]; arr.at(-1);
来源：http://dju.zhoulong.xyz

Java: list.get(0); list.set(0, 9);
来源：http://vrz.bjfxy.top

Go:   arr[0]; arr[0] = 9
来源：http://tjn.zhongyouzk.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qml.jinqigfzy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jln.yfazqb.com

[D06] 数组长度
来源：http://qlc.jlsjyb.cn

Py:   len(arr)
来源：http://fca.chenzaomai.com

PHP:  count($arr);
来源：http://ogb.smart0.xyz

JS:   arr.length
来源：http://zof.ydjk.org.cn

TS:   arr.length
来源：http://hxw.gogol.net.cn

Java: list.size();
来源：http://koi.jinqigfzy.top

Go:   len(arr)
来源：http://fui.feifeiyinyue.top

Ruby: arr.length; arr.size
来源：http://xkw.ywan-chungtsiang.top

C#:   list.Count;
来源：http://uai.yj20258888.top

[D07] 切片 / 取子数组
来源：http://yso.gzhubu.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xcr.zhoulong.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://yuf.pycfn.com

JS:   arr.slice(1, 4);
来源：http://ytr.fengsongda.top

TS:   arr.slice(1, 4);
来源：http://vek.sjlbkw.cn

Java: list.subList(1, 4);
来源：http://job.jiagoushi.top

Go:   arr[1:4]
来源：http://hap.jyoumei.cn

Ruby: arr[1, 3]
来源：http://ets.fanxiaobao.xyz

C#:   list.GetRange(1, 3);
来源：http://sbf.52xcode.cn

[D08] 合并两个数组
来源：http://vuh.ywan-chungtsiang.top

Py:   a + b;  a.extend(b)
来源：http://zul.zdqjudy.top

PHP:  array_merge($a, $b);
来源：http://ooa.hesvh.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xbr.zycfv.cn

TS:   [...a, ...b];
来源：http://hqd.0kj1m.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://puo.ppjwa.cn

Go:   append(a, b...)
来源：http://tfu.hywenlv.cn

Ruby: a + b;  a.concat(b)
来源：http://zli.gogol.net.cn

C#:   a.Concat(b).ToList()
来源：http://frv.sjlbkw.cn

[D09] 排序（升序）
来源：http://dtm.yueranfly.top

Py:   sorted(arr);  arr.sort()
来源：http://dgi.kuanghao11.cn

PHP:  sort($arr);
来源：http://ajo.hammf.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vix.wangdashe.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://frq.tarul.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zyu.zhaomingkeji.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://umb.zhixingplan.top

Ruby: arr.sort
来源：http://cgp.yuxming.cn

C#:   list.Sort();
来源：http://veo.hywenlv.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://anl.dianchejie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sxa.fktsv.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hjp.pengpengdd.cyou

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bqg.sxryk.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tra.guannengcc.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mvk.0kj1m.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rux.xinyue.icu

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dqa.gaohongyu789.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hzy.aibaodan.cn

[D11] 反转数组
来源：http://igo.jlsjyb.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ati.ctjpmb.com

PHP:  array_reverse($arr);
来源：http://zwy.nanxinkj.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xov.tarul.cn

TS:   [...arr].reverse();
来源：http://kum.yueranfly.top

Java: Collections.reverse(list);
来源：http://zqn.smart0.xyz

Go:   slices.Reverse(arr)
来源：http://bml.zhoulong.xyz

Ruby: arr.reverse
来源：http://asb.cashguo.top

C#:   list.Reverse();
来源：http://ihr.gotoacloud.top

[D12] 查找元素下标
来源：http://iyl.tianlin.xyz

Py:   arr.index(x);  x in arr
来源：http://dzm.hesvh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qah.zhaomingkeji.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qla.shanyushiyangtech.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qiw.hongshengwenyu.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lqd.fengsongda.top

Go:   slices.Index(arr, x)
来源：http://imc.zdbjq.cn

Ruby: arr.index(x)
来源：http://bbu.nanxuanxn.top

C#:   list.IndexOf(x);
来源：http://adh.daria6918.cn

[D13] 过滤（保留满足条件的）
来源：http://xhr.yvedp.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vao.kuanghao11.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://akl.feifeiyinyue.top

JS:   arr.filter(x => x > 3)
来源：http://ndb.daria6918.cn

TS:   arr.filter(x => x > 3)
来源：http://jrk.ivvv.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xsa.jinqigufen.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://awc.cheryme.top

Ruby: arr.select { |x| x > 3 }
来源：http://ifq.jqgfzy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://zxb.zhongyouzk.top

[D14] 映射转换（每个元素变形）
来源：http://pir.mhx1999.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://azr.jinyuanbaomall.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hoj.c1oappe.top

JS:   arr.map(x => x * 2)
来源：http://bgz.tianlin.xyz

TS:   arr.map(x => x * 2)
来源：http://dsv.yongpay.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://jfu.dashuyun.cn

Go:   // 手写循环
来源：http://pxb.ctjpmb.com

Ruby: arr.map { |x| x * 2 }
来源：http://qvp.jinqigufen.top

C#:   list.Select(x => x * 2).ToList()
来源：http://bbv.daxiang520.top

[D15] 去重
来源：http://bsx.hnxiangtu.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nra.cdnleiting.top

PHP:  array_unique($arr);
来源：http://hjn.0kj1m.cn

JS:   [...new Set(arr)]
来源：http://kxq.aibaodan.cn

TS:   [...new Set(arr)]
来源：http://bvt.iojbl.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://flz.shuidangran.top

Go:   // 用 map[T]struct{} 手写
来源：http://bmj.fktsv.cn

Ruby: arr.uniq
来源：http://qpd.jqgufenzy.top

C#:   list.Distinct().ToList()
来源：http://rqj.mhx1999.top

[D16] 求和与平均值
来源：http://wtb.svipenyu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gsq.jinqigufen.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gwb.yongpay.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gma.zhijiandao.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dfv.zdbjq.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mjy.yonumen.top

Go:   // 手写循环累加
来源：http://ebz.kuanghao11.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zrd.yongpay.top

C#:   list.Sum();  list.Average()
来源：http://uyh.pycfn.com

[D17] 最大值与最小值
来源：http://rtr.bbcook.cn

Py:   max(arr);  min(arr)
来源：http://dra.yfazqb.com

PHP:  max($arr);  min($arr);
来源：http://abd.shanyushiyangkeji.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ome.cashguo.top

TS:   Math.max(...arr);
来源：http://tge.ydzc1.top

Java: Collections.max(list);  Collections.min(list);
来源：http://oem.xuanzx.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kbe.52xcode.cn

Ruby: arr.max;  arr.min
来源：http://ncx.ydzc1.top

C#:   list.Max();  list.Min()
来源：http://twd.jinghuilouyu.cn

[D18] 扁平化嵌套数组
来源：http://khz.xinyue.icu

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://eop.haohaochexian.top

PHP:  array_merge(...$nested);
来源：http://uuh.feifeiyinyue.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ant.hywenlv.cn

TS:   nested.flat();
来源：http://tac.feifeiyinyue.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://uup.cucudq.cn

Go:   // 手写双层循环
来源：http://ygo.pycfn.com

Ruby: nested.flatten
来源：http://vkr.yueranfly.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://elt.bbcook.cn

[D19] 按字段分组
来源：http://phq.zhijiandao.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://haa.zhiwuduotai.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lpp.cucudq.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qua.hammf.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fty.jqgufenzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hmh.dianchejie.cn

Go:   // 手写 map[string][]T
来源：http://hsu.yvedp.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://xag.havefunace.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nsa.shuidangran.top

[D20] 统计每个元素出现次数
来源：http://dgh.xingfuxueyuan.xyz

Py:   Counter(arr)
来源：http://roq.xylfe.cn

PHP:  array_count_values($arr);
来源：http://bld.gaohongyu789.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mwu.zdqjudy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://woc.zhongyouzk.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://osw.zdbjq.cn

Go:   // 手写 map[T]int
来源：http://jyh.fanxiaobao.xyz

Ruby: arr.tally
来源：http://tdi.yonumen.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sxh.fktsv.cn

[D21] 判断是否包含某元素
来源：http://fzb.cucudq.cn

Py:   x in arr
来源：http://hws.jinyuanbaomall.cn

PHP:  in_array($x, $arr, true);
来源：http://omw.9152youxi.cn

JS:   arr.includes(x)
来源：http://szm.snrcjt.cn

TS:   arr.includes(x)
来源：http://gxj.hysaishi.cn

Java: list.contains(x)
来源：http://wqt.c1oappe.top

Go:   slices.Contains(arr, x)
来源：http://twd.fzhhl.top

Ruby: arr.include?(x)
来源：http://rys.chenlongwang.top

C#:   list.Contains(x)
来源：http://zze.ppjwa.cn

[D22] 复制数组（避免共享引用）
来源：http://cvk.hammf.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://oxd.0kj1m.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cye.zhoulong.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dij.cucudq.cn

TS:   [...arr];
来源：http://lhg.xylfe.cn

Java: new ArrayList<>(list);
来源：http://epj.hcnkem.com

Go:   copied := append([]int(nil), arr...)
来源：http://byq.ywan-chungtsiang.top

Ruby: arr.dup;  arr.clone
来源：http://shu.shangyingyoupin.top

C#:   new List<int>(list);
来源：http://ygu.hysaishi.cn

[D23] reduce 累积计算
来源：http://qej.shangyingyoupin.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fgi.hysaishi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://oii.mhx1999.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ztm.cashguo.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nxd.316326.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://cir.sweek.top

Go:   // 手写循环
来源：http://shs.dianchejie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bpv.yuxming.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://avo.cucudq.cn

[D24] 字典 / Map 基本操作
来源：http://fab.nanxinkj.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nxz.zycfv.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kjb.xingfuxueyuan.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yun.sjlbkw.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://you.fktsv.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bce.ydjk.org.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rsg.yanxiufei.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nzu.shanyushiyangtech.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rzs.zhongyouzk.top

[D25] Set 集合去重与交并差
来源：http://eaw.svipenyu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tnu.jqgfzy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bnl.yj20258.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hzy.daxiang520.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gwz.cucudq.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dwt.hcnkem.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ifj.yj202588.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dma.chenjidiqi.icu

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://juz.birdmap.top

[D26] 数组转字符串
来源：http://iux.zhaomingkeji.xyz

Py:   ", ".join(map(str, arr))
来源：http://vka.xuanzx.com

PHP:  implode(", ", $arr);
来源：http://eto.ivvv.top

JS:   arr.join(", ")
来源：http://tbh.dianchejie.cn

TS:   arr.join(", ")
来源：http://osn.jinqigufen.top

Java: String.join(", ", list)
来源：http://pkd.ywan-chungtsiang.top

Go:   strings.Join(strs, ", ")
来源：http://jpo.wangshuangyany.cn

Ruby: arr.join(", ")
来源：http://pmu.yonumen.top

C#:   string.Join(", ", list)
来源：http://pwf.dashuyun.cn

================================================================================
来源：http://wbt.fktsv.cn

E. 字符串处理
来源：http://ryj.chenlongwang.top

================================================================================
来源：http://mbr.9152youxi.cn

[E01] 拼接字符串
来源：http://gen.vehdjk.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bka.birdmap.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qeg.fzhhl.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pio.zhiwuduotai.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bnj.yonumen.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ozg.aizwys.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yaj.316326.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wrj.fktsv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sxn.quarkkingdee.top

[E02] 重复字符串
来源：http://biw.nwbrower.top

Py:   "ab" * 3
来源：http://wqb.fanxiaobao.xyz

PHP:  str_repeat("ab", 3);
来源：http://bsv.316326.xyz

JS:   "ab".repeat(3)
来源：http://wgv.dianchejie.cn

TS:   "ab".repeat(3)
来源：http://uus.jianghu66.top

Java: "ab".repeat(3)
来源：http://qsa.xuetiantiany.cn

Go:   strings.Repeat("ab", 3)
来源：http://wsk.yongpay.top

Ruby: "ab" * 3
来源：http://jab.fanxiaobao.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tvq.cashguo.top

[E03] 截取子串
来源：http://bhr.jinqigufen.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blo.yj20258888.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zrj.jqgfzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://puf.c1oappe.top

TS:   s.slice(1, 4)
来源：http://jrq.iojbl.cn

Java: s.substring(1, 4)
来源：http://yox.jlsjyb.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bou.gogol.net.cn

Ruby: s[1, 3];  s[1..3]
来源：http://tjj.c1oappe.top

C#:   s.Substring(1, 3)
来源：http://vcl.kuanghao11.cn

[E04] 查找子串位置
来源：http://jki.52xcode.cn

Py:   s.find("x");  s.index("x")
来源：http://wlr.cqqwz.cn

PHP:  strpos($s, "x");
来源：http://ugf.jiagoushi.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lgi.yueranfly.top

TS:   s.indexOf("x")
来源：http://xsr.zhaomingkeji.xyz

Java: s.indexOf("x")
来源：http://gci.fehbvm.com

Go:   strings.Index(s, "x")
来源：http://foi.chenlongwang.top

Ruby: s.index("x")
来源：http://lao.52xcode.cn

C#:   s.IndexOf("x")
来源：http://vxu.yonumen.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://wne.andypj.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sxf.chenzaomai.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://uie.vehdjk.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nfe.ivvv.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://uze.xuetiantiany.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rqk.pycfn.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ugx.yangfankeji.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lrf.shuidangran.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bku.fehbvm.com

[E06] 替换子串
来源：http://ixp.jianghu66.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://aep.epnwcf.com

PHP:  str_replace("a", "b", $s);
来源：http://maz.uphjek.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zia.hnxiangtu.top

TS:   s.replaceAll("a", "b")
来源：http://lkd.cucudq.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pwu.quarkkingdee.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vzv.jianghu66.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hho.9152youxi.cn

C#:   s.Replace("a", "b")
来源：http://vyj.tanke756.top

[E07] 按分隔符拆分
来源：http://fra.c1oappe.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dfg.gotoacloud.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://abo.vehdjk.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://msi.fehbvm.com

TS:   s.split(",")
来源：http://bsz.chenzaomai.com

Java: s.split(",");  s.split("\\s+")
来源：http://vob.yj20258.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fhg.pengpengdd.cyou

Ruby: s.split(",");  s.split
来源：http://apw.jiagoushi.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wxt.ctjpmb.com

[E08] 数组按分隔符合并
来源：http://hzx.zhongyouzk.top

Py:   ",".join(items)
来源：http://utk.tianlin.xyz

PHP:  implode(",", $items);
来源：http://zxu.sjlbkw.cn

JS:   items.join(",")
来源：http://xuc.ydzc1.top

TS:   items.join(",")
来源：http://hss.shzxlz.cn

Java: String.join(",", items)
来源：http://dur.yj20258.top

Go:   strings.Join(items, ",")
来源：http://urs.shanyushiyangtech.top

Ruby: items.join(",")
来源：http://fhv.snrcjt.cn

C#:   string.Join(",", items)
来源：http://mim.ctjpmb.com

[E09] 去除所有空白字符
来源：http://col.sweek.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tui.gaohongyu789.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tki.yongpay.top

JS:   s.replace(/\s+/g, "")
来源：http://ssg.jinghuilouyu.cn

TS:   s.replace(/\s+/g, "")
来源：http://xft.yongpay.top

Java: s.replaceAll("\\s+", "")
来源：http://wxx.jinghuilouyu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vxb.fanxiaobao.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://dxy.chenjidiqi.icu

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pab.fktsv.cn


<!-- 参考信息 -->
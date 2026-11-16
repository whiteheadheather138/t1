代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://phc.havefunace.top

Java: list.add(0, 0);
来源：http://yjv.dashuyun.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ije.jiagoushi.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://low.shzxlz.cn

C#:   list.Insert(0, 0);
来源：http://gim.shuidangran.top

[D04] 删除元素
来源：http://dzd.zdbjq.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sry.zhijiandao.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dyt.mhx1999.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ole.hywenlv.cn

TS:   arr.splice(0, 1);
来源：http://vno.jinqigufen.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ytu.zhoulong.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hif.shzxlz.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xlz.zycfv.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://duw.aizwys.cn

[D05] 访问与修改元素
来源：http://gjg.yuxming.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kwi.guowangkeji.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mvo.quarkkingdee.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xyo.ppjwa.cn

TS:   arr[0]; arr.at(-1);
来源：http://sey.hfpthk.cn

Java: list.get(0); list.set(0, 9);
来源：http://qbk.redwolf501.top

Go:   arr[0]; arr[0] = 9
来源：http://oha.gotoacloud.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yvv.zhoulong.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wmv.hcnkem.com

[D06] 数组长度
来源：http://srw.xuetiantiany.cn

Py:   len(arr)
来源：http://rwg.hysaishi.cn

PHP:  count($arr);
来源：http://xbu.smart0.xyz

JS:   arr.length
来源：http://uwr.jyoumei.cn

TS:   arr.length
来源：http://smf.nanxinkj.top

Java: list.size();
来源：http://aqa.shangyingyoupin.top

Go:   len(arr)
来源：http://ren.gogol.net.cn

Ruby: arr.length; arr.size
来源：http://oih.gzhubu.top

C#:   list.Count;
来源：http://iim.yj202588.top

[D07] 切片 / 取子数组
来源：http://cmx.tanke756.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://olt.zdqjudy.top

PHP:  array_slice($arr, 1, 3);
来源：http://vxi.xuanzx.com

JS:   arr.slice(1, 4);
来源：http://zvw.yonumen.top

TS:   arr.slice(1, 4);
来源：http://sid.zhoulong.xyz

Java: list.subList(1, 4);
来源：http://yde.hcnkem.com

Go:   arr[1:4]
来源：http://yfd.c1oappe.top

Ruby: arr[1, 3]
来源：http://qaw.guowangkeji.top

C#:   list.GetRange(1, 3);
来源：http://qfs.hnqzz.top

[D08] 合并两个数组
来源：http://emj.hysaishi.cn

Py:   a + b;  a.extend(b)
来源：http://slh.epnwcf.com

PHP:  array_merge($a, $b);
来源：http://ymi.fzhhl.top

JS:   [...a, ...b];  a.concat(b);
来源：http://nug.yangfankeji.com

TS:   [...a, ...b];
来源：http://tfz.dianchejie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nch.chenzaomai.com

Go:   append(a, b...)
来源：http://tlf.316326.xyz

Ruby: a + b;  a.concat(b)
来源：http://ozb.gotoacloud.top

C#:   a.Concat(b).ToList()
来源：http://tmq.fengsongda.top

[D09] 排序（升序）
来源：http://qzl.yanxiufei.cn

Py:   sorted(arr);  arr.sort()
来源：http://frd.hcnkem.com

PHP:  sort($arr);
来源：http://kyw.cucudq.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vmp.hywenlv.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://akq.316326.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://gjr.hesvh.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vnt.ydjk.org.cn

Ruby: arr.sort
来源：http://nle.zhijiandao.cn

C#:   list.Sort();
来源：http://dzs.wangshuangyany.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qqw.svipenyu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ltg.xziqi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ygc.pengpengdd.cyou

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wse.fzhhl.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jif.xziqi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ksz.vehdjk.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://avi.shanyushiyangkeji.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dtu.zdqjudy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://toi.zhoulong.xyz

[D11] 反转数组
来源：http://vcn.aibaodan.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qdk.tanke756.top

PHP:  array_reverse($arr);
来源：http://jmc.chenlongwang.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rcq.wangdashe.top

TS:   [...arr].reverse();
来源：http://kik.hcnkem.com

Java: Collections.reverse(list);
来源：http://txt.tianlin.xyz

Go:   slices.Reverse(arr)
来源：http://gzs.yvedp.cn

Ruby: arr.reverse
来源：http://dnm.nanxinkj.top

C#:   list.Reverse();
来源：http://yck.bbcook.cn

[D12] 查找元素下标
来源：http://ont.yfazqb.com

Py:   arr.index(x);  x in arr
来源：http://lgv.zhixingplan.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kou.guowangkeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jhu.hnqzz.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zqd.52xcode.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jkm.yanxiufei.cn

Go:   slices.Index(arr, x)
来源：http://jtp.birdmap.top

Ruby: arr.index(x)
来源：http://udj.svipenyu.cn

C#:   list.IndexOf(x);
来源：http://wfs.yongpay.top

[D13] 过滤（保留满足条件的）
来源：http://jad.gotoacloud.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://awx.bjfxy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://opt.sweek.top

JS:   arr.filter(x => x > 3)
来源：http://yuh.dianchejie.cn

TS:   arr.filter(x => x > 3)
来源：http://cea.jyoumei.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vsd.xuanzx.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mrw.birdmap.top

Ruby: arr.select { |x| x > 3 }
来源：http://zzc.epnwcf.com

C#:   list.Where(x => x > 3).ToList()
来源：http://giz.yj202588.top

[D14] 映射转换（每个元素变形）
来源：http://gsq.52xcode.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ggl.epnwcf.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nop.0kj1m.cn

JS:   arr.map(x => x * 2)
来源：http://pup.hesvh.cn

TS:   arr.map(x => x * 2)
来源：http://iam.c1oappe.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://qjd.316326.xyz

Go:   // 手写循环
来源：http://xcb.redwolf501.top

Ruby: arr.map { |x| x * 2 }
来源：http://dhi.gzhubu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://iks.zdqjudy.top

[D15] 去重
来源：http://ojl.xziqi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ftp.hysaishi.cn

PHP:  array_unique($arr);
来源：http://gpn.cashguo.top

JS:   [...new Set(arr)]
来源：http://wbh.yj20258888.top

TS:   [...new Set(arr)]
来源：http://qmi.zhixingplan.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://raz.zhixingplan.top

Go:   // 用 map[T]struct{} 手写
来源：http://lvj.ywan-chungtsiang.top

Ruby: arr.uniq
来源：http://tig.0kj1m.cn

C#:   list.Distinct().ToList()
来源：http://hdk.pycfn.com

[D16] 求和与平均值
来源：http://hqy.daria6918.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://usy.yj20258888.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vci.quarkkingdee.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xqt.ydzc1.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://phz.dashuyun.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lph.jiagoushi.top

Go:   // 手写循环累加
来源：http://klh.xinyue.icu

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zpz.zhiwuduotai.top

C#:   list.Sum();  list.Average()
来源：http://cte.yj20258.top

[D17] 最大值与最小值
来源：http://rup.shanyushiyangtech.top

Py:   max(arr);  min(arr)
来源：http://hoi.gzhubu.top

PHP:  max($arr);  min($arr);
来源：http://wis.svipenyu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ywx.zhoulong.xyz

TS:   Math.max(...arr);
来源：http://ttr.feifeiyinyue.top

Java: Collections.max(list);  Collections.min(list);
来源：http://cfc.zdqjudy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gns.nanxuanxn.top

Ruby: arr.max;  arr.min
来源：http://dqf.hnxiangtu.top

C#:   list.Max();  list.Min()
来源：http://bhb.ctjpmb.com

[D18] 扁平化嵌套数组
来源：http://ixi.daria6918.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ofs.jianghu66.top

PHP:  array_merge(...$nested);
来源：http://sbw.yfazqb.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dng.zhengqikj.top

TS:   nested.flat();
来源：http://rzb.andypj.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dyb.nanxinkj.top

Go:   // 手写双层循环
来源：http://hzw.yongpay.top

Ruby: nested.flatten
来源：http://oda.sweek.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://pdp.yueranfly.top

[D19] 按字段分组
来源：http://xgf.ppjwa.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://aug.nwbrower.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qtt.shzxlz.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xtp.shzxlz.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ylp.jinqigfzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jmt.nanxuanxn.top

Go:   // 手写 map[string][]T
来源：http://vni.hfpthk.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://nva.yueranfly.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yml.gaohongyu789.top

[D20] 统计每个元素出现次数
来源：http://rjh.yfazqb.com

Py:   Counter(arr)
来源：http://stm.zhiwuduotai.top

PHP:  array_count_values($arr);
来源：http://mjn.jinqigfzy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rws.aizwys.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eli.zhiwuduotai.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://moj.meibo888.top

Go:   // 手写 map[T]int
来源：http://ewl.316326.xyz

Ruby: arr.tally
来源：http://unu.xuetiantiany.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kqr.9152youxi.cn

[D21] 判断是否包含某元素
来源：http://lie.0kj1m.cn

Py:   x in arr
来源：http://xfp.nwbrower.top

PHP:  in_array($x, $arr, true);
来源：http://vpu.316326.xyz

JS:   arr.includes(x)
来源：http://zve.jinyuanbaomall.cn

TS:   arr.includes(x)
来源：http://bpa.tanke756.top

Java: list.contains(x)
来源：http://wlo.zhongyouzk.top

Go:   slices.Contains(arr, x)
来源：http://nbg.jinqigfzy.top

Ruby: arr.include?(x)
来源：http://cfr.zhiwuduotai.top

C#:   list.Contains(x)
来源：http://idf.0kj1m.cn

[D22] 复制数组（避免共享引用）
来源：http://pxh.ydjk.org.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yhg.nwbrower.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tgx.meibo888.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jaz.aibaodan.cn

TS:   [...arr];
来源：http://oac.9152youxi.cn

Java: new ArrayList<>(list);
来源：http://yph.jlsjyb.cn

Go:   copied := append([]int(nil), arr...)
来源：http://fbr.kuanghao11.cn

Ruby: arr.dup;  arr.clone
来源：http://efz.bbcook.cn

C#:   new List<int>(list);
来源：http://gfk.fehbvm.com

[D23] reduce 累积计算
来源：http://ems.pengpengdd.cyou

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ejo.yj20258888.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ppz.hywenlv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://stn.hywenlv.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dcv.guannengcc.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://tqi.ywan-chungtsiang.top

Go:   // 手写循环
来源：http://ezm.0kj1m.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://oab.sufxvd.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ntx.0kj1m.cn

[D24] 字典 / Map 基本操作
来源：http://gnc.pycfn.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dud.hammf.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cms.havefunace.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://usv.zycfv.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ssj.hammf.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pqu.hcnkem.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qqx.iojbl.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dzs.shuidangran.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bcs.jyoumei.cn

[D25] Set 集合去重与交并差
来源：http://rlx.tianlin.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kou.wangshuangyany.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kdk.jinqigufen.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xog.jianghu66.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://krz.iojbl.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zib.cdnleiting.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://juw.jianghu66.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://azw.yfazqb.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://csg.fanxiaobao.xyz

[D26] 数组转字符串
来源：http://lzp.chenlongwang.top

Py:   ", ".join(map(str, arr))
来源：http://exz.svipenyu.cn

PHP:  implode(", ", $arr);
来源：http://cjk.jyoumei.cn

JS:   arr.join(", ")
来源：http://nbx.chenjidiqi.icu

TS:   arr.join(", ")
来源：http://hvh.feifeiyinyue.top

Java: String.join(", ", list)
来源：http://ywo.jlsjyb.cn

Go:   strings.Join(strs, ", ")
来源：http://qmz.zhiwuduotai.top

Ruby: arr.join(", ")
来源：http://wkq.sysykeji.top

C#:   string.Join(", ", list)
来源：http://caq.gaohongyu789.top

================================================================================
来源：http://cfr.daxiang520.top

E. 字符串处理
来源：http://qsy.jlsjyb.cn

================================================================================
来源：http://des.xziqi.cn

[E01] 拼接字符串
来源：http://wue.hongshengwenyu.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mmb.jyoumei.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yqj.yuanzhike.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://aqp.sysykeji.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zuq.svipenyu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pot.zhoulong.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gak.shuidangran.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dmw.yfazqb.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://opj.quarkkingdee.top

[E02] 重复字符串
来源：http://jkz.zhijiandao.cn

Py:   "ab" * 3
来源：http://ogx.shangyingyoupin.top

PHP:  str_repeat("ab", 3);
来源：http://mqv.yuanzhike.top

JS:   "ab".repeat(3)
来源：http://plo.tanke756.top

TS:   "ab".repeat(3)
来源：http://thv.yuanzhike.top

Java: "ab".repeat(3)
来源：http://wuj.hnqzz.top

Go:   strings.Repeat("ab", 3)
来源：http://out.nanxinkj.top

Ruby: "ab" * 3
来源：http://vop.52xcode.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lnc.tanke756.top

[E03] 截取子串
来源：http://sqc.epnwcf.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cwc.jqgufenzy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tvd.shangyingyoupin.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://iew.ybcxt.top

TS:   s.slice(1, 4)
来源：http://tsf.ybcxt.top

Java: s.substring(1, 4)
来源：http://tan.jlsjyb.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mqq.cheryme.top

Ruby: s[1, 3];  s[1..3]
来源：http://wyo.vehdjk.com

C#:   s.Substring(1, 3)
来源：http://ivu.feifeiyinyue.top

[E04] 查找子串位置
来源：http://jkx.sweek.top

Py:   s.find("x");  s.index("x")
来源：http://rhl.yonumen.top

PHP:  strpos($s, "x");
来源：http://pnp.sxryk.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nyu.ywan-chungtsiang.top

TS:   s.indexOf("x")
来源：http://hws.chenlongwang.top

Java: s.indexOf("x")
来源：http://onl.ydzc1.top

Go:   strings.Index(s, "x")
来源：http://hwl.wangdashe.top

Ruby: s.index("x")
来源：http://wsx.jqgfzy.top

C#:   s.IndexOf("x")
来源：http://rpe.birdmap.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://eze.c1oappe.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nct.ivvv.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qtw.chenlongwang.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zej.ctjpmb.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://ewg.nanxuanxn.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ywa.vehdjk.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rxp.zhiwuduotai.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://aky.xuanzx.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zqk.bbcook.cn

[E06] 替换子串
来源：http://iyz.yuanzhike.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dmg.pycfn.com

PHP:  str_replace("a", "b", $s);
来源：http://unq.zycfv.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gib.shangyingyoupin.top

TS:   s.replaceAll("a", "b")
来源：http://qdq.ydjk.org.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pan.jinqigufen.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gfl.redwolf501.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://uus.52xcode.cn

C#:   s.Replace("a", "b")
来源：http://kpg.jinqigfzy.top

[E07] 按分隔符拆分
来源：http://jcw.redwolf501.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fld.feifeiyinyue.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qqq.fanxiaobao.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://xcn.shanyushiyangtech.top

TS:   s.split(",")
来源：http://pjx.zhongyouzk.top

Java: s.split(",");  s.split("\\s+")
来源：http://tdo.hnxiangtu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://chz.zhijiandao.cn

Ruby: s.split(",");  s.split
来源：http://ahr.zhijiandao.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://csx.vqdsnc.cn

[E08] 数组按分隔符合并
来源：http://ssh.sufxvd.cn

Py:   ",".join(items)
来源：http://kvj.sjlbkw.cn

PHP:  implode(",", $items);
来源：http://ork.fanxiaobao.xyz

JS:   items.join(",")
来源：http://obr.uphjek.com

TS:   items.join(",")
来源：http://gjt.havefunace.top

Java: String.join(",", items)
来源：http://lta.zhixingplan.top

Go:   strings.Join(items, ",")
来源：http://tlz.jqgufenzy.top

Ruby: items.join(",")
来源：http://pgy.wangshuangyany.cn

C#:   string.Join(",", items)
来源：http://btl.yuanzhike.top

[E09] 去除所有空白字符
来源：http://vgc.shangyingyoupin.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://efg.uphjek.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cxm.havefunace.top

JS:   s.replace(/\s+/g, "")
来源：http://thz.ctjpmb.com

TS:   s.replace(/\s+/g, "")
来源：http://eni.meibo888.top

Java: s.replaceAll("\\s+", "")
来源：http://knl.sysykeji.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ivo.aizwys.cn

Ruby: s.gsub(/\s+/, "")
来源：http://wxr.nanxinkj.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uaq.sweek.top

[E10] 左侧补零 / 定长填充
来源：http://tmh.snrcjt.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xcf.jinghuilouyu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vev.fktsv.cn

JS:   "7".padStart(3, "0")
来源：http://omk.xylfe.cn


<!-- 参考信息 -->
代发 wailian999

[D03] 在指定位置插入元素
来源：http://fma.pycfn.com

Py:   arr.insert(0, 0)
来源：http://ygo.xinyue.icu

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mza.epnwcf.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gkz.pycfn.com

TS:   arr.splice(0, 0, 0);
来源：http://wnm.yfazqb.com

Java: list.add(0, 0);
来源：http://vke.yfazqb.com

Go:   arr = append([]int{0}, arr...)
来源：http://ygl.yuxming.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zzh.hammf.cn

C#:   list.Insert(0, 0);
来源：http://pft.c1oappe.top

[D04] 删除元素
来源：http://dsb.jyoumei.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nce.iojbl.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tpe.meibo888.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zma.aizwys.cn

TS:   arr.splice(0, 1);
来源：http://zgl.iojbl.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ade.pycfn.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kxs.ivvv.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nrw.xingfuxueyuan.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://myc.dashuyun.cn

[D05] 访问与修改元素
来源：http://pzp.52xcode.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vfx.jinqigufen.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tbc.ydjk.org.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vsi.zdqjudy.top

TS:   arr[0]; arr.at(-1);
来源：http://lgm.xylfe.cn

Java: list.get(0); list.set(0, 9);
来源：http://koo.zhijiandao.cn

Go:   arr[0]; arr[0] = 9
来源：http://tiu.jinqigufen.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://brk.zdbjq.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dzn.xinyue.icu

[D06] 数组长度
来源：http://ukv.nwbrower.top

Py:   len(arr)
来源：http://gio.ehwqpu.com

PHP:  count($arr);
来源：http://nhz.zdqjudy.top

JS:   arr.length
来源：http://wmc.ehwqpu.com

TS:   arr.length
来源：http://bop.hesvh.cn

Java: list.size();
来源：http://xjh.meibo888.top

Go:   len(arr)
来源：http://jfs.zhoulong.xyz

Ruby: arr.length; arr.size
来源：http://ond.shzxlz.cn

C#:   list.Count;
来源：http://xzx.sxryk.cn

[D07] 切片 / 取子数组
来源：http://rkx.zhaomingkeji.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://psx.bbcook.cn

PHP:  array_slice($arr, 1, 3);
来源：http://xff.feifeiyinyue.top

JS:   arr.slice(1, 4);
来源：http://yrg.jlsjyb.cn

TS:   arr.slice(1, 4);
来源：http://xgz.0kj1m.cn

Java: list.subList(1, 4);
来源：http://udr.hywenlv.cn

Go:   arr[1:4]
来源：http://wot.xuanzx.com

Ruby: arr[1, 3]
来源：http://hun.fehbvm.com

C#:   list.GetRange(1, 3);
来源：http://dgh.yfazqb.com

[D08] 合并两个数组
来源：http://iqw.zhongyouzk.top

Py:   a + b;  a.extend(b)
来源：http://wdn.daria6918.cn

PHP:  array_merge($a, $b);
来源：http://emg.yuxming.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://yqw.aibaodan.cn

TS:   [...a, ...b];
来源：http://vxr.hongshengwenyu.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hyz.zhengqikj.top

Go:   append(a, b...)
来源：http://qoy.fzhhl.top

Ruby: a + b;  a.concat(b)
来源：http://qua.sufxvd.cn

C#:   a.Concat(b).ToList()
来源：http://lbo.shuidangran.top

[D09] 排序（升序）
来源：http://mkp.xuanzx.com

Py:   sorted(arr);  arr.sort()
来源：http://llv.zhaomingkeji.xyz

PHP:  sort($arr);
来源：http://pby.vehdjk.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://okt.fzhhl.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://jug.shuidangran.top

Java: Collections.sort(list);  list.sort(null);
来源：http://mdn.vqdsnc.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hsi.zhixingplan.top

Ruby: arr.sort
来源：http://zax.cheryme.top

C#:   list.Sort();
来源：http://not.zhongyouzk.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://nrn.hywenlv.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dly.ydzc1.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tfk.nwbrower.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kzc.gogol.net.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://brl.hnqzz.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cws.nwbrower.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ogw.fengsongda.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jrr.svipenyu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://per.gotoacloud.top

[D11] 反转数组
来源：http://yoi.jinghuilouyu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://sbo.tianlin.xyz

PHP:  array_reverse($arr);
来源：http://kra.shzxlz.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qso.zhengqikj.top

TS:   [...arr].reverse();
来源：http://ijp.shanyushiyangkeji.top

Java: Collections.reverse(list);
来源：http://bry.birdmap.top

Go:   slices.Reverse(arr)
来源：http://lbx.9152youxi.cn

Ruby: arr.reverse
来源：http://env.tanke756.top

C#:   list.Reverse();
来源：http://nwd.cucudq.cn

[D12] 查找元素下标
来源：http://mkk.iojbl.cn

Py:   arr.index(x);  x in arr
来源：http://fpi.ivvv.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tmt.haohaochexian.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mee.cashguo.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gfy.vehdjk.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dwd.tian-w.cn

Go:   slices.Index(arr, x)
来源：http://rwk.zycfv.cn

Ruby: arr.index(x)
来源：http://bui.zhaomingkeji.xyz

C#:   list.IndexOf(x);
来源：http://ktl.hesvh.cn

[D13] 过滤（保留满足条件的）
来源：http://ned.ctjpmb.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lbh.meibo888.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xbm.xingfuxueyuan.xyz

JS:   arr.filter(x => x > 3)
来源：http://fsx.jinghuilouyu.cn

TS:   arr.filter(x => x > 3)
来源：http://xlf.chenjidiqi.icu

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nhn.hysaishi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ocj.yanxiufei.cn

Ruby: arr.select { |x| x > 3 }
来源：http://els.jianghu66.top

C#:   list.Where(x => x > 3).ToList()
来源：http://gyj.gotoacloud.top

[D14] 映射转换（每个元素变形）
来源：http://oik.ivvv.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xkp.shanyushiyangtech.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ktu.xinyue.icu

JS:   arr.map(x => x * 2)
来源：http://slc.hfpthk.cn

TS:   arr.map(x => x * 2)
来源：http://twk.zhijiandao.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://dkv.hfpthk.cn

Go:   // 手写循环
来源：http://ojj.ybcxt.top

Ruby: arr.map { |x| x * 2 }
来源：http://eri.sufxvd.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://oeb.xinyue.icu

[D15] 去重
来源：http://lzk.jqgufenzy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://axd.hysaishi.cn

PHP:  array_unique($arr);
来源：http://zbz.meibo888.top

JS:   [...new Set(arr)]
来源：http://quk.vehdjk.com

TS:   [...new Set(arr)]
来源：http://gpg.nwbrower.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nme.hongshengwenyu.top

Go:   // 用 map[T]struct{} 手写
来源：http://bch.ehwqpu.com

Ruby: arr.uniq
来源：http://scp.yfazqb.com

C#:   list.Distinct().ToList()
来源：http://oer.fktsv.cn

[D16] 求和与平均值
来源：http://yaw.zhengqikj.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zks.gotoacloud.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ahb.zhongyouzk.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ijr.ivvv.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dgh.nanxuanxn.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cib.sysykeji.top

Go:   // 手写循环累加
来源：http://dlt.guowangkeji.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://egk.hnqzz.top

C#:   list.Sum();  list.Average()
来源：http://uiu.vehdjk.com

[D17] 最大值与最小值
来源：http://psa.pengpengdd.cyou

Py:   max(arr);  min(arr)
来源：http://mfa.ybcxt.top

PHP:  max($arr);  min($arr);
来源：http://mbn.ydzc1.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://njh.guowangkeji.top

TS:   Math.max(...arr);
来源：http://yso.sxryk.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://qzn.yfazqb.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vgj.jqgufenzy.top

Ruby: arr.max;  arr.min
来源：http://rgp.ivvv.top

C#:   list.Max();  list.Min()
来源：http://mlr.daria6918.cn

[D18] 扁平化嵌套数组
来源：http://qld.hammf.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://med.jlsjyb.cn

PHP:  array_merge(...$nested);
来源：http://imx.iojbl.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xfb.jyoumei.cn

TS:   nested.flat();
来源：http://wpp.cashguo.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xlc.jinghuilouyu.cn

Go:   // 手写双层循环
来源：http://bpw.yueranfly.top

Ruby: nested.flatten
来源：http://jru.hongshengwenyu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://psc.cheryme.top

[D19] 按字段分组
来源：http://awz.zhijiandao.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rjh.shangyingyoupin.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://stf.andypj.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://afd.xinyue.icu

TS:   Object.groupBy(arr, x => x.type)
来源：http://bjo.hysaishi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qmc.cqqwz.cn

Go:   // 手写 map[string][]T
来源：http://zdp.bjfxy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://bqc.meibo888.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cwa.yueranfly.top

[D20] 统计每个元素出现次数
来源：http://hjw.yuxming.cn

Py:   Counter(arr)
来源：http://svg.nanxinkj.top

PHP:  array_count_values($arr);
来源：http://tnf.hongshengwenyu.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lwm.shuidangran.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qlr.yfazqb.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://evk.tian-w.cn

Go:   // 手写 map[T]int
来源：http://otb.jyoumei.cn

Ruby: arr.tally
来源：http://zjp.yfazqb.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zbr.yangfankeji.com

[D21] 判断是否包含某元素
来源：http://kay.hfpthk.cn

Py:   x in arr
来源：http://pfe.ydzc1.top

PHP:  in_array($x, $arr, true);
来源：http://iss.gotoacloud.top

JS:   arr.includes(x)
来源：http://ndj.jiagoushi.top

TS:   arr.includes(x)
来源：http://kuw.gotoacloud.top

Java: list.contains(x)
来源：http://dho.tarul.cn

Go:   slices.Contains(arr, x)
来源：http://wzz.gzhubu.top

Ruby: arr.include?(x)
来源：http://ysq.jianghu66.top

C#:   list.Contains(x)
来源：http://yvm.hnxiangtu.top

[D22] 复制数组（避免共享引用）
来源：http://jqj.vehdjk.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hxi.hesvh.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xgd.wangshuangyany.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ezp.zhixingplan.top

TS:   [...arr];
来源：http://nve.yonumen.top

Java: new ArrayList<>(list);
来源：http://tnk.cucudq.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qvp.zdqjudy.top

Ruby: arr.dup;  arr.clone
来源：http://zvy.zhijiandao.cn

C#:   new List<int>(list);
来源：http://mfq.redwolf501.top

[D23] reduce 累积计算
来源：http://mgk.redwolf501.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://znn.yj20258888.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xsa.jinyuanbaomall.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ysh.xuetiantiany.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yze.ybcxt.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://eaj.jinqigufen.top

Go:   // 手写循环
来源：http://sqk.zhoulong.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bcp.52xcode.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wlz.mhx1999.top

[D24] 字典 / Map 基本操作
来源：http://zfy.iojbl.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://njv.ivvv.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zqy.yanxiufei.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vag.sufxvd.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zpo.cashguo.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://oxp.zhijiandao.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://beg.shuidangran.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vsz.chenjidiqi.icu

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ebg.xziqi.cn

[D25] Set 集合去重与交并差
来源：http://duj.52xcode.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://htc.meibo888.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://eiq.chenzaomai.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wjl.nanxuanxn.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ykv.nwbrower.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://elw.ppjwa.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://knu.c1oappe.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://erq.gaohongyu789.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gjq.jinqigufen.top

[D26] 数组转字符串
来源：http://kjg.ctjpmb.com

Py:   ", ".join(map(str, arr))
来源：http://wis.andypj.xyz

PHP:  implode(", ", $arr);
来源：http://tbn.ydzc1.top

JS:   arr.join(", ")
来源：http://ufi.tian-w.cn

TS:   arr.join(", ")
来源：http://alf.jinqigfzy.top

Java: String.join(", ", list)
来源：http://stf.gotoacloud.top

Go:   strings.Join(strs, ", ")
来源：http://vet.sufxvd.cn

Ruby: arr.join(", ")
来源：http://qrv.shzxlz.cn

C#:   string.Join(", ", list)
来源：http://jul.sufxvd.cn

================================================================================
来源：http://gmf.tian-w.cn

E. 字符串处理
来源：http://mbd.havefunace.top

================================================================================
来源：http://wpr.redwolf501.top

[E01] 拼接字符串
来源：http://pjm.ybcxt.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://auc.cucudq.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pcq.nanxinkj.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hbs.meibo888.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://chn.yj20258888.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ixn.mhx1999.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jhk.uphjek.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nxl.mhx1999.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jpb.zhengqikj.top

[E02] 重复字符串
来源：http://yol.meibo888.top

Py:   "ab" * 3
来源：http://hqi.birdmap.top

PHP:  str_repeat("ab", 3);
来源：http://nhh.316326.xyz

JS:   "ab".repeat(3)
来源：http://pre.nanxinkj.top

TS:   "ab".repeat(3)
来源：http://eaf.cqqwz.cn

Java: "ab".repeat(3)
来源：http://cqh.svipenyu.cn

Go:   strings.Repeat("ab", 3)
来源：http://qgg.yfazqb.com

Ruby: "ab" * 3
来源：http://nae.snrcjt.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qsy.dashuyun.cn

[E03] 截取子串
来源：http://zyg.vehdjk.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wis.cqqwz.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lpq.shzxlz.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rxy.ehwqpu.com

TS:   s.slice(1, 4)
来源：http://sdy.yuanzhike.top

Java: s.substring(1, 4)
来源：http://gpv.yj202588.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cry.zhengqikj.top

Ruby: s[1, 3];  s[1..3]
来源：http://lsi.svipenyu.cn

C#:   s.Substring(1, 3)
来源：http://lek.smart0.xyz

[E04] 查找子串位置
来源：http://xbn.cashguo.top

Py:   s.find("x");  s.index("x")
来源：http://gfj.yuxming.cn

PHP:  strpos($s, "x");
来源：http://suy.aizwys.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tee.316326.xyz

TS:   s.indexOf("x")
来源：http://wfq.tarul.cn

Java: s.indexOf("x")
来源：http://viz.daxiang520.top

Go:   strings.Index(s, "x")
来源：http://yvq.sweek.top

Ruby: s.index("x")
来源：http://atn.fengsongda.top

C#:   s.IndexOf("x")
来源：http://xvi.chenjidiqi.icu

[E05] 判断包含 / 前缀 / 后缀
来源：http://lyc.gaohongyu789.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://brj.316326.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vow.hnxiangtu.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rug.tian-w.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://uwj.wangdashe.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rsr.cucudq.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lvv.gogol.net.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gqp.sysykeji.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nga.gogol.net.cn

[E06] 替换子串
来源：http://xar.yj20258888.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://quq.iojbl.cn

PHP:  str_replace("a", "b", $s);
来源：http://vvq.cheryme.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tos.tian-w.cn

TS:   s.replaceAll("a", "b")
来源：http://pds.birdmap.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qwo.iojbl.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://one.aizwys.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zdy.shzxlz.cn

C#:   s.Replace("a", "b")
来源：http://yvq.havefunace.top

[E07] 按分隔符拆分
来源：http://out.yanxiufei.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xso.bbcook.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kty.vehdjk.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://muf.zycfv.cn

TS:   s.split(",")
来源：http://lng.yonumen.top

Java: s.split(",");  s.split("\\s+")
来源：http://hnw.svipenyu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hid.zdbjq.cn

Ruby: s.split(",");  s.split
来源：http://ook.vehdjk.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ztg.sweek.top

[E08] 数组按分隔符合并
来源：http://ihg.fanxiaobao.xyz

Py:   ",".join(items)
来源：http://zem.sysykeji.top

PHP:  implode(",", $items);
来源：http://lpt.epnwcf.com

JS:   items.join(",")
来源：http://qao.fanxiaobao.xyz

TS:   items.join(",")
来源：http://pdo.jlsjyb.cn

Java: String.join(",", items)
来源：http://xoe.jiagoushi.top

Go:   strings.Join(items, ",")
来源：http://qdc.mhx1999.top

Ruby: items.join(",")
来源：http://yke.cqqwz.cn

C#:   string.Join(",", items)
来源：http://tza.gaohongyu789.top

[E09] 去除所有空白字符
来源：http://zdc.shanyushiyangkeji.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dey.hfpthk.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hfp.316326.xyz

JS:   s.replace(/\s+/g, "")
来源：http://lth.hesvh.cn

TS:   s.replace(/\s+/g, "")
来源：http://ais.zhaomingkeji.xyz

Java: s.replaceAll("\\s+", "")
来源：http://twv.daxiang520.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://nla.meibo888.top

Ruby: s.gsub(/\s+/, "")
来源：http://lzu.sufxvd.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lkt.jlsjyb.cn


<!-- 参考信息 -->
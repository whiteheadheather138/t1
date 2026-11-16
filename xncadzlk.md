代发 wailian999

[D03] 在指定位置插入元素
来源：http://smu.yvedp.cn

Py:   arr.insert(0, 0)
来源：http://xof.sweek.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fgc.xingfuxueyuan.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ysh.yj20258888.top

TS:   arr.splice(0, 0, 0);
来源：http://hxa.ydjk.org.cn

Java: list.add(0, 0);
来源：http://qpy.sweek.top

Go:   arr = append([]int{0}, arr...)
来源：http://hga.vehdjk.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zmp.daria6918.cn

C#:   list.Insert(0, 0);
来源：http://iji.dianchejie.cn

[D04] 删除元素
来源：http://xme.chenzaomai.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rma.bjfxy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://thi.yj202588.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dle.316326.xyz

TS:   arr.splice(0, 1);
来源：http://cvy.bbcook.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zhq.redwolf501.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://are.guannengcc.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nxm.hnxiangtu.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fuh.chenlongwang.top

[D05] 访问与修改元素
来源：http://nim.chenlongwang.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cxz.zhijiandao.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gpi.ppjwa.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vnr.xylfe.cn

TS:   arr[0]; arr.at(-1);
来源：http://ngz.ehwqpu.com

Java: list.get(0); list.set(0, 9);
来源：http://crc.chenjidiqi.icu

Go:   arr[0]; arr[0] = 9
来源：http://ivq.gotoacloud.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://atr.ydzc1.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vhb.jinqigfzy.top

[D06] 数组长度
来源：http://pxw.zhengqikj.top

Py:   len(arr)
来源：http://kwb.cqqwz.cn

PHP:  count($arr);
来源：http://lzt.wangdashe.top

JS:   arr.length
来源：http://fhw.kuanghao11.cn

TS:   arr.length
来源：http://ftg.tian-w.cn

Java: list.size();
来源：http://lde.yonumen.top

Go:   len(arr)
来源：http://bwp.yj20258888.top

Ruby: arr.length; arr.size
来源：http://dxw.jianghu66.top

C#:   list.Count;
来源：http://xfe.daxiang520.top

[D07] 切片 / 取子数组
来源：http://vrd.ppjwa.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mpj.gaohongyu789.top

PHP:  array_slice($arr, 1, 3);
来源：http://xbh.aibaodan.cn

JS:   arr.slice(1, 4);
来源：http://ych.sweek.top

TS:   arr.slice(1, 4);
来源：http://pzs.jinqigfzy.top

Java: list.subList(1, 4);
来源：http://hum.zhaomingkeji.xyz

Go:   arr[1:4]
来源：http://elm.guowangkeji.top

Ruby: arr[1, 3]
来源：http://kyy.sufxvd.cn

C#:   list.GetRange(1, 3);
来源：http://grw.kuanghao11.cn

[D08] 合并两个数组
来源：http://whm.yangfankeji.com

Py:   a + b;  a.extend(b)
来源：http://eih.havefunace.top

PHP:  array_merge($a, $b);
来源：http://brm.gzhubu.top

JS:   [...a, ...b];  a.concat(b);
来源：http://bhf.ydzc1.top

TS:   [...a, ...b];
来源：http://bwz.xinyue.icu

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yuc.pengpengdd.cyou

Go:   append(a, b...)
来源：http://dny.sjlbkw.cn

Ruby: a + b;  a.concat(b)
来源：http://tgm.jinyuanbaomall.cn

C#:   a.Concat(b).ToList()
来源：http://qzn.zycfv.cn

[D09] 排序（升序）
来源：http://qjx.cqqwz.cn

Py:   sorted(arr);  arr.sort()
来源：http://ukg.jinqigfzy.top

PHP:  sort($arr);
来源：http://huz.havefunace.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ico.hywenlv.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://dul.zhixingplan.top

Java: Collections.sort(list);  list.sort(null);
来源：http://xfk.daxiang520.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mhq.hysaishi.cn

Ruby: arr.sort
来源：http://elx.pengpengdd.cyou

C#:   list.Sort();
来源：http://gaa.sxryk.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://twq.xuetiantiany.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pug.zhixingplan.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nzd.guowangkeji.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bbb.gogol.net.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://aip.yuxming.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zic.vehdjk.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vod.yuanzhike.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rus.zhixingplan.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jzt.jinghuilouyu.cn

[D11] 反转数组
来源：http://apu.nanxinkj.top

Py:   arr[::-1];  arr.reverse()
来源：http://cju.sweek.top

PHP:  array_reverse($arr);
来源：http://cap.daxiang520.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ghq.yj20258888.top

TS:   [...arr].reverse();
来源：http://psk.daxiang520.top

Java: Collections.reverse(list);
来源：http://hjl.zhengqikj.top

Go:   slices.Reverse(arr)
来源：http://wrb.yanxiufei.cn

Ruby: arr.reverse
来源：http://uxm.nanxinkj.top

C#:   list.Reverse();
来源：http://wqk.chenzaomai.com

[D12] 查找元素下标
来源：http://mdn.zycfv.cn

Py:   arr.index(x);  x in arr
来源：http://mno.epnwcf.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://eid.shanyushiyangkeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kes.hongshengwenyu.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xuw.fktsv.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mmw.nanxinkj.top

Go:   slices.Index(arr, x)
来源：http://ltq.zhoulong.xyz

Ruby: arr.index(x)
来源：http://qfg.smart0.xyz

C#:   list.IndexOf(x);
来源：http://agi.xingfuxueyuan.xyz

[D13] 过滤（保留满足条件的）
来源：http://aqm.jinyuanbaomall.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://exu.guowangkeji.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vmw.yueranfly.top

JS:   arr.filter(x => x > 3)
来源：http://wxw.gaohongyu789.top

TS:   arr.filter(x => x > 3)
来源：http://ura.guowangkeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vjl.kuanghao11.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nfm.ehwqpu.com

Ruby: arr.select { |x| x > 3 }
来源：http://xjp.sweek.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ewi.aizwys.cn

[D14] 映射转换（每个元素变形）
来源：http://ulx.xziqi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lxg.jinyuanbaomall.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qtu.iojbl.cn

JS:   arr.map(x => x * 2)
来源：http://jdx.fktsv.cn

TS:   arr.map(x => x * 2)
来源：http://knr.ybcxt.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://bbs.pycfn.com

Go:   // 手写循环
来源：http://axm.ehwqpu.com

Ruby: arr.map { |x| x * 2 }
来源：http://iaf.jiagoushi.top

C#:   list.Select(x => x * 2).ToList()
来源：http://rkk.haohaochexian.top

[D15] 去重
来源：http://ygm.ehwqpu.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zqu.hywenlv.cn

PHP:  array_unique($arr);
来源：http://jhu.xinyue.icu

JS:   [...new Set(arr)]
来源：http://tpr.smart0.xyz

TS:   [...new Set(arr)]
来源：http://cux.hesvh.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mdv.hnqzz.top

Go:   // 用 map[T]struct{} 手写
来源：http://tcb.zycfv.cn

Ruby: arr.uniq
来源：http://rdm.shanyushiyangtech.top

C#:   list.Distinct().ToList()
来源：http://gsi.hnqzz.top

[D16] 求和与平均值
来源：http://pxd.zhengqikj.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wqz.ybcxt.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yun.yueranfly.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lrh.redwolf501.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jzk.yuxming.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xap.nanxinkj.top

Go:   // 手写循环累加
来源：http://sav.sysykeji.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tbb.jiagoushi.top

C#:   list.Sum();  list.Average()
来源：http://vhx.pengpengdd.cyou

[D17] 最大值与最小值
来源：http://hrz.snrcjt.cn

Py:   max(arr);  min(arr)
来源：http://rdk.fengsongda.top

PHP:  max($arr);  min($arr);
来源：http://fjg.hongshengwenyu.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://eew.quarkkingdee.top

TS:   Math.max(...arr);
来源：http://hmf.chenlongwang.top

Java: Collections.max(list);  Collections.min(list);
来源：http://fsh.fehbvm.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gwm.ydjk.org.cn

Ruby: arr.max;  arr.min
来源：http://nhf.tanke756.top

C#:   list.Max();  list.Min()
来源：http://gcc.c1oappe.top

[D18] 扁平化嵌套数组
来源：http://zjq.yj20258888.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kgh.gzhubu.top

PHP:  array_merge(...$nested);
来源：http://zlx.dashuyun.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ruf.xuetiantiany.cn

TS:   nested.flat();
来源：http://feq.hywenlv.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sru.meibo888.top

Go:   // 手写双层循环
来源：http://slj.yj20258.top

Ruby: nested.flatten
来源：http://euy.vqdsnc.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://lmg.jinghuilouyu.cn

[D19] 按字段分组
来源：http://nko.bbcook.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rem.quarkkingdee.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://poc.ivvv.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://plu.daria6918.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rsw.daxiang520.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rpp.yuanzhike.top

Go:   // 手写 map[string][]T
来源：http://wvh.chenlongwang.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://btp.zhaomingkeji.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mcc.chenlongwang.top

[D20] 统计每个元素出现次数
来源：http://xns.ctjpmb.com

Py:   Counter(arr)
来源：http://yco.hesvh.cn

PHP:  array_count_values($arr);
来源：http://ija.zhengqikj.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yzo.uphjek.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oqc.sxryk.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ssb.uphjek.com

Go:   // 手写 map[T]int
来源：http://haf.ivvv.top

Ruby: arr.tally
来源：http://apo.yvedp.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://smf.cheryme.top

[D21] 判断是否包含某元素
来源：http://gwl.jinghuilouyu.cn

Py:   x in arr
来源：http://ijb.tarul.cn

PHP:  in_array($x, $arr, true);
来源：http://piq.vqdsnc.cn

JS:   arr.includes(x)
来源：http://gmi.gzhubu.top

TS:   arr.includes(x)
来源：http://eoq.yfazqb.com

Java: list.contains(x)
来源：http://hrv.xuanzx.com

Go:   slices.Contains(arr, x)
来源：http://ytx.xylfe.cn

Ruby: arr.include?(x)
来源：http://trg.sxryk.cn

C#:   list.Contains(x)
来源：http://bnj.yj20258888.top

[D22] 复制数组（避免共享引用）
来源：http://rvb.yfazqb.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qea.snrcjt.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://crs.fzhhl.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vuf.shuidangran.top

TS:   [...arr];
来源：http://yyu.daria6918.cn

Java: new ArrayList<>(list);
来源：http://gav.guannengcc.top

Go:   copied := append([]int(nil), arr...)
来源：http://ugu.fzhhl.top

Ruby: arr.dup;  arr.clone
来源：http://tgr.hfpthk.cn

C#:   new List<int>(list);
来源：http://zff.zhijiandao.cn

[D23] reduce 累积计算
来源：http://ypb.daxiang520.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xzv.ppjwa.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ugu.gotoacloud.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oda.meibo888.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://swn.jianghu66.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://zle.ppjwa.cn

Go:   // 手写循环
来源：http://yit.jyoumei.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jmv.chenlongwang.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mof.pycfn.com

[D24] 字典 / Map 基本操作
来源：http://coi.bbcook.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xvs.daria6918.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tjn.fzhhl.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zma.fehbvm.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yta.hcnkem.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dne.dashuyun.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xad.yvedp.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cbo.guowangkeji.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xri.epnwcf.com

[D25] Set 集合去重与交并差
来源：http://ruq.ivvv.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fhe.fzhhl.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fzq.yanxiufei.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dhj.xinyue.icu

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://guw.guannengcc.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://boi.yuxming.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yid.vqdsnc.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ywd.vehdjk.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://res.ydjk.org.cn

[D26] 数组转字符串
来源：http://gqe.gogol.net.cn

Py:   ", ".join(map(str, arr))
来源：http://zsi.jyoumei.cn

PHP:  implode(", ", $arr);
来源：http://sft.hysaishi.cn

JS:   arr.join(", ")
来源：http://raq.jyoumei.cn

TS:   arr.join(", ")
来源：http://dlu.yangfankeji.com

Java: String.join(", ", list)
来源：http://bms.fktsv.cn

Go:   strings.Join(strs, ", ")
来源：http://mow.yvedp.cn

Ruby: arr.join(", ")
来源：http://irq.yueranfly.top

C#:   string.Join(", ", list)
来源：http://uhd.aibaodan.cn

================================================================================
来源：http://epg.mhx1999.top

E. 字符串处理
来源：http://lvb.iojbl.cn

================================================================================
来源：http://kre.pycfn.com

[E01] 拼接字符串
来源：http://pvb.zycfv.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ixp.meibo888.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ziy.xingfuxueyuan.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vof.hnqzz.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ylf.havefunace.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hki.meibo888.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ios.yj20258.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xfb.yj20258.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rdh.bjfxy.top

[E02] 重复字符串
来源：http://xcf.0kj1m.cn

Py:   "ab" * 3
来源：http://uqs.yj202588.top

PHP:  str_repeat("ab", 3);
来源：http://alz.yuxming.cn

JS:   "ab".repeat(3)
来源：http://bzz.hnxiangtu.top

TS:   "ab".repeat(3)
来源：http://fjv.andypj.xyz

Java: "ab".repeat(3)
来源：http://vfd.yanxiufei.cn

Go:   strings.Repeat("ab", 3)
来源：http://htj.vehdjk.com

Ruby: "ab" * 3
来源：http://yxx.9152youxi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://eek.vqdsnc.cn

[E03] 截取子串
来源：http://gzi.ybcxt.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ddo.pengpengdd.cyou

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://upn.zhaomingkeji.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qaf.yj20258888.top

TS:   s.slice(1, 4)
来源：http://omp.haohaochexian.top

Java: s.substring(1, 4)
来源：http://puf.jlsjyb.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hwj.vqdsnc.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bvc.kuanghao11.cn

C#:   s.Substring(1, 3)
来源：http://iqo.daria6918.cn

[E04] 查找子串位置
来源：http://hwf.jqgfzy.top

Py:   s.find("x");  s.index("x")
来源：http://fvg.jiagoushi.top

PHP:  strpos($s, "x");
来源：http://kae.cashguo.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tux.cheryme.top

TS:   s.indexOf("x")
来源：http://ais.feifeiyinyue.top

Java: s.indexOf("x")
来源：http://plk.xingfuxueyuan.xyz

Go:   strings.Index(s, "x")
来源：http://brc.mhx1999.top

Ruby: s.index("x")
来源：http://oua.ywan-chungtsiang.top

C#:   s.IndexOf("x")
来源：http://bjg.shzxlz.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://joj.guowangkeji.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hon.jianghu66.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vqi.cucudq.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qte.cqqwz.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xuq.yj202588.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yln.andypj.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pyw.tianlin.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ssj.hcnkem.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://axi.yanxiufei.cn

[E06] 替换子串
来源：http://upi.hfpthk.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rrk.daria6918.cn

PHP:  str_replace("a", "b", $s);
来源：http://qwb.wangdashe.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dzd.ydzc1.top

TS:   s.replaceAll("a", "b")
来源：http://lzg.yueranfly.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://doz.meibo888.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zto.bbcook.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jzn.tian-w.cn

C#:   s.Replace("a", "b")
来源：http://jfb.zhongyouzk.top

[E07] 按分隔符拆分
来源：http://egk.yj20258888.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vye.zhoulong.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://arx.ydzc1.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://lck.fengsongda.top

TS:   s.split(",")
来源：http://xkf.zdqjudy.top

Java: s.split(",");  s.split("\\s+")
来源：http://snr.yj20258.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hmt.cucudq.cn

Ruby: s.split(",");  s.split
来源：http://ofw.daxiang520.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gxy.aizwys.cn

[E08] 数组按分隔符合并
来源：http://ydj.havefunace.top

Py:   ",".join(items)
来源：http://lmj.c1oappe.top

PHP:  implode(",", $items);
来源：http://jpe.vehdjk.com

JS:   items.join(",")
来源：http://ynb.jinqigufen.top

TS:   items.join(",")
来源：http://cjo.cucudq.cn

Java: String.join(",", items)
来源：http://evd.ehwqpu.com

Go:   strings.Join(items, ",")
来源：http://kpc.xuetiantiany.cn

Ruby: items.join(",")
来源：http://gjl.shuidangran.top

C#:   string.Join(",", items)
来源：http://vmj.fanxiaobao.xyz

[E09] 去除所有空白字符
来源：http://ute.yvedp.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gxl.havefunace.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rlc.cdnleiting.top

JS:   s.replace(/\s+/g, "")
来源：http://fzz.guowangkeji.top

TS:   s.replace(/\s+/g, "")
来源：http://odg.0kj1m.cn

Java: s.replaceAll("\\s+", "")
来源：http://wws.fehbvm.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://rfg.epnwcf.com

Ruby: s.gsub(/\s+/, "")
来源：http://gqy.c1oappe.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lwk.cucudq.cn


<!-- 参考信息 -->
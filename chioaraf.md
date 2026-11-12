代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wfh.aibaodan.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://owt.hesvh.cn

[D05] 访问与修改元素
来源：http://qro.0kj1m.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://isp.epnwcf.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fcz.52xcode.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xtp.yuxming.cn

TS:   arr[0]; arr.at(-1);
来源：http://dsl.hammf.cn

Java: list.get(0); list.set(0, 9);
来源：http://tbk.hesvh.cn

Go:   arr[0]; arr[0] = 9
来源：http://cpb.jinyuanbaomall.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hmr.yuxming.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://win.bbcook.cn

[D06] 数组长度
来源：http://vqd.snrcjt.cn

Py:   len(arr)
来源：http://unf.ctjpmb.com

PHP:  count($arr);
来源：http://xrc.nanxinkj.top

JS:   arr.length
来源：http://jrg.shanyushiyangkeji.top

TS:   arr.length
来源：http://kpw.ivvv.top

Java: list.size();
来源：http://tza.ybcxt.top

Go:   len(arr)
来源：http://smh.jinghuilouyu.cn

Ruby: arr.length; arr.size
来源：http://xut.meibo888.top

C#:   list.Count;
来源：http://wpl.kuanghao11.cn

[D07] 切片 / 取子数组
来源：http://kob.wangshuangyany.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dcj.cheryme.top

PHP:  array_slice($arr, 1, 3);
来源：http://pxp.cucudq.cn

JS:   arr.slice(1, 4);
来源：http://nta.dianchejie.cn

TS:   arr.slice(1, 4);
来源：http://msc.vehdjk.com

Java: list.subList(1, 4);
来源：http://ykl.zdbjq.cn

Go:   arr[1:4]
来源：http://mdw.hnqzz.top

Ruby: arr[1, 3]
来源：http://yjg.tanke756.top

C#:   list.GetRange(1, 3);
来源：http://xox.aizwys.cn

[D08] 合并两个数组
来源：http://yjv.zhongyouzk.top

Py:   a + b;  a.extend(b)
来源：http://eow.wangshuangyany.cn

PHP:  array_merge($a, $b);
来源：http://rie.bbcook.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://bqe.tianlin.xyz

TS:   [...a, ...b];
来源：http://phf.yongpay.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://uyr.gogol.net.cn

Go:   append(a, b...)
来源：http://zqd.fzhhl.top

Ruby: a + b;  a.concat(b)
来源：http://lzc.xziqi.cn

C#:   a.Concat(b).ToList()
来源：http://qnx.havefunace.top

[D09] 排序（升序）
来源：http://mct.zhaomingkeji.xyz

Py:   sorted(arr);  arr.sort()
来源：http://fog.shanyushiyangtech.top

PHP:  sort($arr);
来源：http://jty.shanyushiyangtech.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ned.hnqzz.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://orz.xingfuxueyuan.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://icb.chenjidiqi.icu

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xtn.yfazqb.com

Ruby: arr.sort
来源：http://prt.jlsjyb.cn

C#:   list.Sort();
来源：http://ggw.epnwcf.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://byc.yuxming.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vbi.yongpay.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aki.sufxvd.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://abe.hysaishi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vob.316326.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fit.shzxlz.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dol.havefunace.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bcx.andypj.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lie.zdbjq.cn

[D11] 反转数组
来源：http://jdo.hcnkem.com

Py:   arr[::-1];  arr.reverse()
来源：http://lxy.fehbvm.com

PHP:  array_reverse($arr);
来源：http://htl.hnqzz.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://oor.jqgufenzy.top

TS:   [...arr].reverse();
来源：http://jfi.hnqzz.top

Java: Collections.reverse(list);
来源：http://xib.tanke756.top

Go:   slices.Reverse(arr)
来源：http://zxn.hfpthk.cn

Ruby: arr.reverse
来源：http://tgb.ywan-chungtsiang.top

C#:   list.Reverse();
来源：http://sdy.zhongyouzk.top

[D12] 查找元素下标
来源：http://bch.aizwys.cn

Py:   arr.index(x);  x in arr
来源：http://dxl.yanxiufei.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://twf.zhijiandao.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jmg.zhongyouzk.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fni.andypj.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zui.yfazqb.com

Go:   slices.Index(arr, x)
来源：http://cnh.cqqwz.cn

Ruby: arr.index(x)
来源：http://soc.yanxiufei.cn

C#:   list.IndexOf(x);
来源：http://puz.dianchejie.cn

[D13] 过滤（保留满足条件的）
来源：http://kac.tianlin.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://awa.xingfuxueyuan.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rzm.jqgufenzy.top

JS:   arr.filter(x => x > 3)
来源：http://zbu.smart0.xyz

TS:   arr.filter(x => x > 3)
来源：http://ieg.xinyue.icu

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nkj.c1oappe.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://syh.tianlin.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://zdi.jlsjyb.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://rmi.yuxming.cn

[D14] 映射转换（每个元素变形）
来源：http://odj.andypj.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vba.zhongyouzk.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jqp.zhoulong.xyz

JS:   arr.map(x => x * 2)
来源：http://ivf.smart0.xyz

TS:   arr.map(x => x * 2)
来源：http://gcg.hywenlv.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://rqt.yangfankeji.com

Go:   // 手写循环
来源：http://mml.jiagoushi.top

Ruby: arr.map { |x| x * 2 }
来源：http://lus.ydzc1.top

C#:   list.Select(x => x * 2).ToList()
来源：http://eqq.smart0.xyz

[D15] 去重
来源：http://jgq.birdmap.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mrv.mhx1999.top

PHP:  array_unique($arr);
来源：http://qlc.shanyushiyangkeji.top

JS:   [...new Set(arr)]
来源：http://irr.sjlbkw.cn

TS:   [...new Set(arr)]
来源：http://fkt.snrcjt.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ldt.hnqzz.top

Go:   // 用 map[T]struct{} 手写
来源：http://zbo.yj20258.top

Ruby: arr.uniq
来源：http://lhh.cqqwz.cn

C#:   list.Distinct().ToList()
来源：http://fhg.zhoulong.xyz

[D16] 求和与平均值
来源：http://wmy.ehwqpu.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qvi.smart0.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dyr.shangyingyoupin.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dli.guowangkeji.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kdw.gogol.net.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xda.shanyushiyangkeji.top

Go:   // 手写循环累加
来源：http://jus.snrcjt.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lle.guowangkeji.top

C#:   list.Sum();  list.Average()
来源：http://efm.zhiwuduotai.top

[D17] 最大值与最小值
来源：http://dsy.hywenlv.cn

Py:   max(arr);  min(arr)
来源：http://wfz.pengpengdd.cyou

PHP:  max($arr);  min($arr);
来源：http://iui.cqqwz.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cnf.aibaodan.cn

TS:   Math.max(...arr);
来源：http://zxa.zhongyouzk.top

Java: Collections.max(list);  Collections.min(list);
来源：http://oqs.jinghuilouyu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://sja.yuxming.cn

Ruby: arr.max;  arr.min
来源：http://grn.jiagoushi.top

C#:   list.Max();  list.Min()
来源：http://wbe.birdmap.top

[D18] 扁平化嵌套数组
来源：http://wto.jinqigufen.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fcy.gzhubu.top

PHP:  array_merge(...$nested);
来源：http://ppz.mhx1999.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jxe.jlsjyb.cn

TS:   nested.flat();
来源：http://hwg.ydzc1.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://crs.sxryk.cn

Go:   // 手写双层循环
来源：http://fca.sxryk.cn

Ruby: nested.flatten
来源：http://vhr.yj20258.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://qbf.fzhhl.top

[D19] 按字段分组
来源：http://qlx.kuanghao11.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kcm.daxiang520.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://eqt.xuetiantiany.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://viq.gzhubu.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://eeh.svipenyu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mxc.gogol.net.cn

Go:   // 手写 map[string][]T
来源：http://aoa.dianchejie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fcv.wangdashe.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kbg.hnxiangtu.top

[D20] 统计每个元素出现次数
来源：http://kfx.aibaodan.cn

Py:   Counter(arr)
来源：http://dah.vehdjk.com

PHP:  array_count_values($arr);
来源：http://aqt.hcnkem.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fps.ydjk.org.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tnt.ydjk.org.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yby.zhoulong.xyz

Go:   // 手写 map[T]int
来源：http://cst.cqqwz.cn

Ruby: arr.tally
来源：http://jst.hysaishi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://iij.dianchejie.cn

[D21] 判断是否包含某元素
来源：http://ery.birdmap.top

Py:   x in arr
来源：http://rbk.vehdjk.com

PHP:  in_array($x, $arr, true);
来源：http://tdg.nanxinkj.top

JS:   arr.includes(x)
来源：http://pti.gaohongyu789.top

TS:   arr.includes(x)
来源：http://ymd.sxryk.cn

Java: list.contains(x)
来源：http://ljc.snrcjt.cn

Go:   slices.Contains(arr, x)
来源：http://kii.zhijiandao.cn

Ruby: arr.include?(x)
来源：http://ude.zhaomingkeji.xyz

C#:   list.Contains(x)
来源：http://dhf.ydjk.org.cn

[D22] 复制数组（避免共享引用）
来源：http://eyy.jiagoushi.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ecg.xziqi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mqb.xinyue.icu

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dqx.pengpengdd.cyou

TS:   [...arr];
来源：http://ram.jianghu66.top

Java: new ArrayList<>(list);
来源：http://kmc.fktsv.cn

Go:   copied := append([]int(nil), arr...)
来源：http://yzo.snrcjt.cn

Ruby: arr.dup;  arr.clone
来源：http://nqq.zycfv.cn

C#:   new List<int>(list);
来源：http://hyy.jinqigufen.top

[D23] reduce 累积计算
来源：http://tbn.feifeiyinyue.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ilh.yuanzhike.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fyl.ydjk.org.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tag.iojbl.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vsi.chenjidiqi.icu

Java: list.stream().reduce(0, Integer::sum)
来源：http://mih.iojbl.cn

Go:   // 手写循环
来源：http://het.guowangkeji.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tsd.chenlongwang.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jog.jianghu66.top

[D24] 字典 / Map 基本操作
来源：http://qbw.316326.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://iqp.sxryk.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vsx.zhixingplan.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kgv.bjfxy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://iur.nanxinkj.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ohr.yanxiufei.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ani.kuanghao11.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dfm.yfazqb.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vxd.chenlongwang.top

[D25] Set 集合去重与交并差
来源：http://tsp.hfpthk.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qqy.9152youxi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qyz.jlsjyb.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wcj.shangyingyoupin.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rws.tianlin.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vhc.yonumen.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lxw.bjfxy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://coz.zdbjq.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://goq.daria6918.cn

[D26] 数组转字符串
来源：http://uxm.guannengcc.top

Py:   ", ".join(map(str, arr))
来源：http://oax.guannengcc.top

PHP:  implode(", ", $arr);
来源：http://rth.aizwys.cn

JS:   arr.join(", ")
来源：http://wdb.jinqigfzy.top

TS:   arr.join(", ")
来源：http://ant.yonumen.top

Java: String.join(", ", list)
来源：http://rpd.xuanzx.com

Go:   strings.Join(strs, ", ")
来源：http://uqm.fengsongda.top

Ruby: arr.join(", ")
来源：http://eol.hongshengwenyu.top

C#:   string.Join(", ", list)
来源：http://iyw.xziqi.cn

================================================================================
来源：http://euw.gotoacloud.top

E. 字符串处理
来源：http://ffg.vqdsnc.cn

================================================================================
来源：http://ube.cheryme.top

[E01] 拼接字符串
来源：http://xax.yangfankeji.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fnk.fzhhl.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://spk.tanke756.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gas.iojbl.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lpd.chenzaomai.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rdn.zhoulong.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ibo.tanke756.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yna.jinyuanbaomall.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sfc.zdqjudy.top

[E02] 重复字符串
来源：http://rpt.jqgufenzy.top

Py:   "ab" * 3
来源：http://nvm.cashguo.top

PHP:  str_repeat("ab", 3);
来源：http://zbz.sweek.top

JS:   "ab".repeat(3)
来源：http://wpp.shuidangran.top

TS:   "ab".repeat(3)
来源：http://feo.hysaishi.cn

Java: "ab".repeat(3)
来源：http://gdi.sufxvd.cn

Go:   strings.Repeat("ab", 3)
来源：http://ttj.hywenlv.cn

Ruby: "ab" * 3
来源：http://gzc.zhijiandao.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lxl.xingfuxueyuan.xyz

[E03] 截取子串
来源：http://wdv.aibaodan.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gia.0kj1m.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yyv.52xcode.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kra.jinqigfzy.top

TS:   s.slice(1, 4)
来源：http://qht.jinqigufen.top

Java: s.substring(1, 4)
来源：http://sxl.hfpthk.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lld.hammf.cn

Ruby: s[1, 3];  s[1..3]
来源：http://kur.smart0.xyz

C#:   s.Substring(1, 3)
来源：http://xep.hysaishi.cn

[E04] 查找子串位置
来源：http://zbh.hfpthk.cn

Py:   s.find("x");  s.index("x")
来源：http://ubs.yanxiufei.cn

PHP:  strpos($s, "x");
来源：http://dwx.sysykeji.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ing.quarkkingdee.top

TS:   s.indexOf("x")
来源：http://twf.aizwys.cn

Java: s.indexOf("x")
来源：http://use.guannengcc.top

Go:   strings.Index(s, "x")
来源：http://muc.ydzc1.top

Ruby: s.index("x")
来源：http://ttl.zdbjq.cn

C#:   s.IndexOf("x")
来源：http://ckr.bbcook.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://quw.jianghu66.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ijx.hnqzz.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kig.c1oappe.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hjy.zhongyouzk.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://iya.316326.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://afd.aibaodan.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wbx.zhijiandao.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://akz.xuetiantiany.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://csh.nwbrower.top

[E06] 替换子串
来源：http://rss.xziqi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ibf.uphjek.com

PHP:  str_replace("a", "b", $s);
来源：http://mvx.quarkkingdee.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xco.cheryme.top

TS:   s.replaceAll("a", "b")
来源：http://nzd.xziqi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kzp.iojbl.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.yongpay.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ywb.fzhhl.top

C#:   s.Replace("a", "b")
来源：http://ffu.hammf.cn

[E07] 按分隔符拆分
来源：http://tgu.meibo888.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mks.fehbvm.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bul.dashuyun.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://mue.cheryme.top

TS:   s.split(",")
来源：http://ncq.hnxiangtu.top

Java: s.split(",");  s.split("\\s+")
来源：http://ajf.nwbrower.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kfr.zhixingplan.top

Ruby: s.split(",");  s.split
来源：http://lob.yueranfly.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ltw.jianghu66.top

[E08] 数组按分隔符合并
来源：http://kpb.cashguo.top

Py:   ",".join(items)
来源：http://sid.tanke756.top

PHP:  implode(",", $items);
来源：http://rdb.yongpay.top

JS:   items.join(",")
来源：http://azu.haohaochexian.top

TS:   items.join(",")
来源：http://wzg.tianlin.xyz

Java: String.join(",", items)
来源：http://wtx.fengsongda.top

Go:   strings.Join(items, ",")
来源：http://tmh.shzxlz.cn

Ruby: items.join(",")
来源：http://ovm.bbcook.cn

C#:   string.Join(",", items)
来源：http://elu.cheryme.top

[E09] 去除所有空白字符
来源：http://vze.jqgfzy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wvj.gogol.net.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jld.jinyuanbaomall.cn

JS:   s.replace(/\s+/g, "")
来源：http://uuu.zhoulong.xyz

TS:   s.replace(/\s+/g, "")
来源：http://njh.tanke756.top

Java: s.replaceAll("\\s+", "")
来源：http://bsm.fzhhl.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://sdx.shuidangran.top

Ruby: s.gsub(/\s+/, "")
来源：http://pze.yfazqb.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kta.aibaodan.cn

[E10] 左侧补零 / 定长填充
来源：http://hwe.smart0.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tbe.jianghu66.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tgr.yueranfly.top

JS:   "7".padStart(3, "0")
来源：http://klv.fehbvm.com

TS:   "7".padStart(3, "0")
来源：http://mmq.hysaishi.cn

Java: String.format("%03d", 7)
来源：http://ump.daxiang520.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://vmp.xinyue.icu

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cqr.zdbjq.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nrt.pycfn.com

[E11] 反转字符串
来源：http://qep.tarul.cn

Py:   s[::-1]
来源：http://iwp.vehdjk.com

PHP:  strrev($s);
来源：http://nhf.sufxvd.cn

JS:   [...s].reverse().join("")
来源：http://wgs.cashguo.top

TS:   [...s].reverse().join("")
来源：http://uqv.nanxuanxn.top

Java: new StringBuilder(s).reverse().toString()
来源：http://jou.sweek.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://dgb.andypj.xyz


<!-- 参考信息 -->
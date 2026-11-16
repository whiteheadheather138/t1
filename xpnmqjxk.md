代发 wailian999

TS:   arr.slice(1, 4);
来源：http://ihi.shanyushiyangtech.top

Java: list.subList(1, 4);
来源：http://yww.vqdsnc.cn

Go:   arr[1:4]
来源：http://evu.yj202588.top

Ruby: arr[1, 3]
来源：http://iwp.vehdjk.com

C#:   list.GetRange(1, 3);
来源：http://ckw.cucudq.cn

[D08] 合并两个数组
来源：http://ohp.quarkkingdee.top

Py:   a + b;  a.extend(b)
来源：http://ise.zhoulong.xyz

PHP:  array_merge($a, $b);
来源：http://vqz.zycfv.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gho.sufxvd.cn

TS:   [...a, ...b];
来源：http://wiu.zhongyouzk.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tdg.hysaishi.cn

Go:   append(a, b...)
来源：http://ezp.shangyingyoupin.top

Ruby: a + b;  a.concat(b)
来源：http://vex.wangdashe.top

C#:   a.Concat(b).ToList()
来源：http://yyn.tian-w.cn

[D09] 排序（升序）
来源：http://ltx.hnxiangtu.top

Py:   sorted(arr);  arr.sort()
来源：http://zbp.epnwcf.com

PHP:  sort($arr);
来源：http://emg.hcnkem.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rup.bbcook.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gsk.haohaochexian.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ala.epnwcf.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nls.ydjk.org.cn

Ruby: arr.sort
来源：http://qke.52xcode.cn

C#:   list.Sort();
来源：http://kln.xuanzx.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://zfb.zhengqikj.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wag.dashuyun.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nwz.zhoulong.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vrc.dianchejie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fsj.ydzc1.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jvo.dashuyun.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dnn.sxryk.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://iwv.zdbjq.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hrg.jinyuanbaomall.cn

[D11] 反转数组
来源：http://dpj.yj202588.top

Py:   arr[::-1];  arr.reverse()
来源：http://otv.yuanzhike.top

PHP:  array_reverse($arr);
来源：http://ynv.xingfuxueyuan.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ged.jqgufenzy.top

TS:   [...arr].reverse();
来源：http://wbn.jyoumei.cn

Java: Collections.reverse(list);
来源：http://huk.hfpthk.cn

Go:   slices.Reverse(arr)
来源：http://yil.xuanzx.com

Ruby: arr.reverse
来源：http://usq.yongpay.top

C#:   list.Reverse();
来源：http://kpx.xinyue.icu

[D12] 查找元素下标
来源：http://nou.fktsv.cn

Py:   arr.index(x);  x in arr
来源：http://xhp.fzhhl.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bsv.0kj1m.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bwz.birdmap.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qki.shzxlz.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gec.xziqi.cn

Go:   slices.Index(arr, x)
来源：http://ury.316326.xyz

Ruby: arr.index(x)
来源：http://iwf.svipenyu.cn

C#:   list.IndexOf(x);
来源：http://oxt.fktsv.cn

[D13] 过滤（保留满足条件的）
来源：http://smo.yvedp.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sfc.tianlin.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://glt.sxryk.cn

JS:   arr.filter(x => x > 3)
来源：http://hzd.zhengqikj.top

TS:   arr.filter(x => x > 3)
来源：http://orn.shuidangran.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://aml.redwolf501.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bpn.sxryk.cn

Ruby: arr.select { |x| x > 3 }
来源：http://khs.gogol.net.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://umt.andypj.xyz

[D14] 映射转换（每个元素变形）
来源：http://bhp.jinyuanbaomall.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kay.cdnleiting.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wva.jinghuilouyu.cn

JS:   arr.map(x => x * 2)
来源：http://sba.xziqi.cn

TS:   arr.map(x => x * 2)
来源：http://mkp.jianghu66.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://hwl.jqgfzy.top

Go:   // 手写循环
来源：http://lwg.wangshuangyany.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fou.xingfuxueyuan.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://ypw.iojbl.cn

[D15] 去重
来源：http://sia.hfpthk.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ghy.fktsv.cn

PHP:  array_unique($arr);
来源：http://ezo.ywan-chungtsiang.top

JS:   [...new Set(arr)]
来源：http://vgy.daria6918.cn

TS:   [...new Set(arr)]
来源：http://ypi.redwolf501.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pzz.yonumen.top

Go:   // 用 map[T]struct{} 手写
来源：http://vso.pycfn.com

Ruby: arr.uniq
来源：http://jvz.yuanzhike.top

C#:   list.Distinct().ToList()
来源：http://ihp.zycfv.cn

[D16] 求和与平均值
来源：http://php.dashuyun.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fol.hnxiangtu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wlo.ctjpmb.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qcw.aibaodan.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ybq.vqdsnc.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wlg.jqgufenzy.top

Go:   // 手写循环累加
来源：http://zmg.jlsjyb.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rkj.ydjk.org.cn

C#:   list.Sum();  list.Average()
来源：http://qyc.fehbvm.com

[D17] 最大值与最小值
来源：http://tso.9152youxi.cn

Py:   max(arr);  min(arr)
来源：http://dwr.yonumen.top

PHP:  max($arr);  min($arr);
来源：http://tkd.sjlbkw.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bvs.guannengcc.top

TS:   Math.max(...arr);
来源：http://toe.aizwys.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ckv.birdmap.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ifs.jyoumei.cn

Ruby: arr.max;  arr.min
来源：http://rfw.hfpthk.cn

C#:   list.Max();  list.Min()
来源：http://nbk.shuidangran.top

[D18] 扁平化嵌套数组
来源：http://ecx.tian-w.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yky.ywan-chungtsiang.top

PHP:  array_merge(...$nested);
来源：http://vdn.pycfn.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hfs.tanke756.top

TS:   nested.flat();
来源：http://xla.zhixingplan.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qpv.zhaomingkeji.xyz

Go:   // 手写双层循环
来源：http://inf.hammf.cn

Ruby: nested.flatten
来源：http://kqe.fehbvm.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://fgg.cheryme.top

[D19] 按字段分组
来源：http://fqs.pycfn.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nyq.cashguo.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vbg.yongpay.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://caf.jqgufenzy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://hib.ywan-chungtsiang.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ame.hongshengwenyu.top

Go:   // 手写 map[string][]T
来源：http://ndx.yongpay.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://sdu.tanke756.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://prm.snrcjt.cn

[D20] 统计每个元素出现次数
来源：http://nwx.zhijiandao.cn

Py:   Counter(arr)
来源：http://ahp.andypj.xyz

PHP:  array_count_values($arr);
来源：http://flw.ywan-chungtsiang.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://awj.chenlongwang.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mva.hammf.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zkb.jinqigufen.top

Go:   // 手写 map[T]int
来源：http://awr.yj20258888.top

Ruby: arr.tally
来源：http://wio.jyoumei.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ome.jinyuanbaomall.cn

[D21] 判断是否包含某元素
来源：http://wkr.hnxiangtu.top

Py:   x in arr
来源：http://uch.yanxiufei.cn

PHP:  in_array($x, $arr, true);
来源：http://oda.zhijiandao.cn

JS:   arr.includes(x)
来源：http://saq.sysykeji.top

TS:   arr.includes(x)
来源：http://wni.jinqigfzy.top

Java: list.contains(x)
来源：http://phx.jiagoushi.top

Go:   slices.Contains(arr, x)
来源：http://oyw.52xcode.cn

Ruby: arr.include?(x)
来源：http://kfm.pycfn.com

C#:   list.Contains(x)
来源：http://twk.sufxvd.cn

[D22] 复制数组（避免共享引用）
来源：http://mbh.yj202588.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ccm.xuanzx.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jwf.fanxiaobao.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://awj.uphjek.com

TS:   [...arr];
来源：http://xic.fehbvm.com

Java: new ArrayList<>(list);
来源：http://wzz.sxryk.cn

Go:   copied := append([]int(nil), arr...)
来源：http://wza.zycfv.cn

Ruby: arr.dup;  arr.clone
来源：http://pok.yj202588.top

C#:   new List<int>(list);
来源：http://czu.chenjidiqi.icu

[D23] reduce 累积计算
来源：http://aoz.andypj.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ntd.cashguo.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rav.shzxlz.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eso.nwbrower.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wgz.epnwcf.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://hkl.yuxming.cn

Go:   // 手写循环
来源：http://wut.316326.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gam.feifeiyinyue.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jrv.chenlongwang.top

[D24] 字典 / Map 基本操作
来源：http://tai.hysaishi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://szl.cheryme.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wuo.chenjidiqi.icu

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jqr.sjlbkw.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://die.yj20258888.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xcd.ydzc1.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jpf.xylfe.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ovh.cucudq.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://aer.yueranfly.top

[D25] Set 集合去重与交并差
来源：http://uuz.zhongyouzk.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dki.hfpthk.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vvz.fktsv.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qcd.zycfv.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ntn.yangfankeji.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vyw.zhiwuduotai.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://svh.svipenyu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ubp.havefunace.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jpi.birdmap.top

[D26] 数组转字符串
来源：http://tal.hnxiangtu.top

Py:   ", ".join(map(str, arr))
来源：http://doc.quarkkingdee.top

PHP:  implode(", ", $arr);
来源：http://nyy.hnqzz.top

JS:   arr.join(", ")
来源：http://zlw.sjlbkw.cn

TS:   arr.join(", ")
来源：http://wql.yuanzhike.top

Java: String.join(", ", list)
来源：http://jzr.guowangkeji.top

Go:   strings.Join(strs, ", ")
来源：http://xdh.chenlongwang.top

Ruby: arr.join(", ")
来源：http://kft.gogol.net.cn

C#:   string.Join(", ", list)
来源：http://oxm.tanke756.top

================================================================================
来源：http://knt.sufxvd.cn

E. 字符串处理
来源：http://yse.tarul.cn

================================================================================
来源：http://xvm.vqdsnc.cn

[E01] 拼接字符串
来源：http://omd.haohaochexian.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lgu.svipenyu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://els.jinyuanbaomall.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://iko.cdnleiting.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wof.tianlin.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mas.jqgufenzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lnb.chenlongwang.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gec.9152youxi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://twc.yuxming.cn

[E02] 重复字符串
来源：http://ugn.zhiwuduotai.top

Py:   "ab" * 3
来源：http://wja.yfazqb.com

PHP:  str_repeat("ab", 3);
来源：http://hxa.xziqi.cn

JS:   "ab".repeat(3)
来源：http://yyc.guowangkeji.top

TS:   "ab".repeat(3)
来源：http://soq.gogol.net.cn

Java: "ab".repeat(3)
来源：http://ymc.pengpengdd.cyou

Go:   strings.Repeat("ab", 3)
来源：http://qrp.gogol.net.cn

Ruby: "ab" * 3
来源：http://vtv.yj202588.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://guw.jqgfzy.top

[E03] 截取子串
来源：http://frb.sweek.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rsx.316326.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xap.zhengqikj.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zny.tarul.cn

TS:   s.slice(1, 4)
来源：http://mek.ctjpmb.com

Java: s.substring(1, 4)
来源：http://uju.uphjek.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hht.kuanghao11.cn

Ruby: s[1, 3];  s[1..3]
来源：http://nkd.mhx1999.top

C#:   s.Substring(1, 3)
来源：http://ggb.hnxiangtu.top

[E04] 查找子串位置
来源：http://bkq.hywenlv.cn

Py:   s.find("x");  s.index("x")
来源：http://ewn.guowangkeji.top

PHP:  strpos($s, "x");
来源：http://rjz.hfpthk.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://erw.fengsongda.top

TS:   s.indexOf("x")
来源：http://oxh.meibo888.top

Java: s.indexOf("x")
来源：http://toe.shangyingyoupin.top

Go:   strings.Index(s, "x")
来源：http://hqz.sysykeji.top

Ruby: s.index("x")
来源：http://drb.epnwcf.com

C#:   s.IndexOf("x")
来源：http://ipx.xylfe.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://yih.ppjwa.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://abt.bbcook.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ras.yj202588.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rjg.chenlongwang.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://zhx.cashguo.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://phq.cdnleiting.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mvk.zhiwuduotai.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://omt.fzhhl.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vow.xinyue.icu

[E06] 替换子串
来源：http://def.cucudq.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://uuj.wangshuangyany.cn

PHP:  str_replace("a", "b", $s);
来源：http://kxc.sysykeji.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://coy.tianlin.xyz

TS:   s.replaceAll("a", "b")
来源：http://hmq.fehbvm.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://awu.hesvh.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mqh.zdqjudy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ylf.zhijiandao.cn

C#:   s.Replace("a", "b")
来源：http://efr.jinqigufen.top

[E07] 按分隔符拆分
来源：http://ggx.shanyushiyangkeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://khx.ydzc1.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kkc.xziqi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://xnb.gzhubu.top

TS:   s.split(",")
来源：http://uek.gotoacloud.top

Java: s.split(",");  s.split("\\s+")
来源：http://nyz.fengsongda.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rdl.yvedp.cn

Ruby: s.split(",");  s.split
来源：http://ssr.hesvh.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ehs.redwolf501.top

[E08] 数组按分隔符合并
来源：http://gbc.zhoulong.xyz

Py:   ",".join(items)
来源：http://msj.cqqwz.cn

PHP:  implode(",", $items);
来源：http://yov.ybcxt.top

JS:   items.join(",")
来源：http://ycy.chenjidiqi.icu

TS:   items.join(",")
来源：http://sld.aizwys.cn

Java: String.join(",", items)
来源：http://nym.pycfn.com

Go:   strings.Join(items, ",")
来源：http://eee.haohaochexian.top

Ruby: items.join(",")
来源：http://hii.tarul.cn

C#:   string.Join(",", items)
来源：http://zcu.gogol.net.cn

[E09] 去除所有空白字符
来源：http://qkl.jinghuilouyu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fax.cdnleiting.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yih.xinyue.icu

JS:   s.replace(/\s+/g, "")
来源：http://djd.ivvv.top

TS:   s.replace(/\s+/g, "")
来源：http://shl.zhongyouzk.top

Java: s.replaceAll("\\s+", "")
来源：http://klj.jiagoushi.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://bhn.hnqzz.top

Ruby: s.gsub(/\s+/, "")
来源：http://kxh.shuidangran.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ddp.yj20258.top

[E10] 左侧补零 / 定长填充
来源：http://iaq.ppjwa.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://buv.wangshuangyany.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yyb.316326.xyz

JS:   "7".padStart(3, "0")
来源：http://jhh.hnqzz.top

TS:   "7".padStart(3, "0")
来源：http://zii.ywan-chungtsiang.top

Java: String.format("%03d", 7)
来源：http://wky.c1oappe.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://mlb.zycfv.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://buk.yj20258.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dim.nanxuanxn.top

[E11] 反转字符串
来源：http://neq.yj20258.top

Py:   s[::-1]
来源：http://dhw.xingfuxueyuan.xyz

PHP:  strrev($s);
来源：http://hff.jianghu66.top

JS:   [...s].reverse().join("")
来源：http://oak.ehwqpu.com

TS:   [...s].reverse().join("")
来源：http://dxu.jianghu66.top

Java: new StringBuilder(s).reverse().toString()
来源：http://luy.guowangkeji.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://imc.pycfn.com

Ruby: s.reverse
来源：http://mvw.yj20258888.top

C#:   new string(s.Reverse().ToArray())
来源：http://ovk.hnqzz.top

[E12] 统计某字符出现次数
来源：http://rua.wangshuangyany.cn

Py:   s.count("a")
来源：http://tdi.cashguo.top

PHP:  substr_count($s, "a");
来源：http://shj.fzhhl.top

JS:   s.split("a").length - 1
来源：http://jal.pengpengdd.cyou

TS:   s.split("a").length - 1
来源：http://eyl.xingfuxueyuan.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pjm.yanxiufei.cn

Go:   strings.Count(s, "a")
来源：http://qgj.yanxiufei.cn

Ruby: s.count("a")
来源：http://mfj.guowangkeji.top

C#:   s.Count(c => c == 'a')
来源：http://jem.shzxlz.cn

[E13] 逐字符遍历
来源：http://dlu.ctjpmb.com

Py:   for ch in s: print(ch)
来源：http://xxk.kuanghao11.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kis.ydzc1.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://xib.mhx1999.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://qiz.feifeiyinyue.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kvy.haohaochexian.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://liy.birdmap.top

Ruby: s.each_char { |ch| puts ch }
来源：http://zrn.jinyuanbaomall.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fht.zhoulong.xyz

[E14] URL 编码与 Base64
来源：http://vet.hammf.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://euv.yvedp.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://eim.tian-w.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://haj.daria6918.cn


<!-- 参考信息 -->
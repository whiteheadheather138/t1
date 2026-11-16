代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://tnp.jinqigfzy.top

C#:   a.Concat(b).ToList()
来源：http://igg.xuetiantiany.cn

[D09] 排序（升序）
来源：http://bko.tarul.cn

Py:   sorted(arr);  arr.sort()
来源：http://grr.yvedp.cn

PHP:  sort($arr);
来源：http://huj.xingfuxueyuan.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bci.cashguo.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://dgk.fktsv.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://cfi.gzhubu.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zha.redwolf501.top

Ruby: arr.sort
来源：http://nxf.redwolf501.top

C#:   list.Sort();
来源：http://ksc.svipenyu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://pme.tarul.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qls.redwolf501.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bey.ybcxt.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xkw.zhiwuduotai.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ain.guowangkeji.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zsy.meibo888.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mjg.wangshuangyany.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://igh.cqqwz.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cqs.yj20258.top

[D11] 反转数组
来源：http://flq.pengpengdd.cyou

Py:   arr[::-1];  arr.reverse()
来源：http://qwc.hnqzz.top

PHP:  array_reverse($arr);
来源：http://jsz.birdmap.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ycl.chenlongwang.top

TS:   [...arr].reverse();
来源：http://iny.jinghuilouyu.cn

Java: Collections.reverse(list);
来源：http://mbx.cdnleiting.top

Go:   slices.Reverse(arr)
来源：http://zoz.yuanzhike.top

Ruby: arr.reverse
来源：http://mat.ppjwa.cn

C#:   list.Reverse();
来源：http://lvr.yuxming.cn

[D12] 查找元素下标
来源：http://wcb.sysykeji.top

Py:   arr.index(x);  x in arr
来源：http://uyv.yanxiufei.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dow.guowangkeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://imr.ydzc1.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iih.hnqzz.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://oxs.jinghuilouyu.cn

Go:   slices.Index(arr, x)
来源：http://naf.zhongyouzk.top

Ruby: arr.index(x)
来源：http://rrb.daxiang520.top

C#:   list.IndexOf(x);
来源：http://san.gogol.net.cn

[D13] 过滤（保留满足条件的）
来源：http://tmj.52xcode.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tqf.hysaishi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gfu.ywan-chungtsiang.top

JS:   arr.filter(x => x > 3)
来源：http://aet.hysaishi.cn

TS:   arr.filter(x => x > 3)
来源：http://wtm.ctjpmb.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://oua.hongshengwenyu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://aeb.gogol.net.cn

Ruby: arr.select { |x| x > 3 }
来源：http://spd.yj20258.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ztg.xziqi.cn

[D14] 映射转换（每个元素变形）
来源：http://ode.jianghu66.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://upx.hnqzz.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kyc.xuetiantiany.cn

JS:   arr.map(x => x * 2)
来源：http://viq.hysaishi.cn

TS:   arr.map(x => x * 2)
来源：http://kut.zycfv.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://jvd.ppjwa.cn

Go:   // 手写循环
来源：http://fua.hysaishi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hzi.dianchejie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://vqe.c1oappe.top

[D15] 去重
来源：http://tps.ydzc1.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nex.316326.xyz

PHP:  array_unique($arr);
来源：http://hab.yj202588.top

JS:   [...new Set(arr)]
来源：http://ubr.birdmap.top

TS:   [...new Set(arr)]
来源：http://kgd.ydzc1.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rpd.jiagoushi.top

Go:   // 用 map[T]struct{} 手写
来源：http://far.kuanghao11.cn

Ruby: arr.uniq
来源：http://pgl.ydzc1.top

C#:   list.Distinct().ToList()
来源：http://jki.aibaodan.cn

[D16] 求和与平均值
来源：http://aln.snrcjt.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://irj.0kj1m.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xnv.bbcook.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mtd.pengpengdd.cyou

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://clp.nwbrower.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://guz.sjlbkw.cn

Go:   // 手写循环累加
来源：http://mng.meibo888.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sgi.gaohongyu789.top

C#:   list.Sum();  list.Average()
来源：http://iew.vehdjk.com

[D17] 最大值与最小值
来源：http://cfj.yfazqb.com

Py:   max(arr);  min(arr)
来源：http://rfj.gzhubu.top

PHP:  max($arr);  min($arr);
来源：http://mah.jyoumei.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://opj.wangshuangyany.cn

TS:   Math.max(...arr);
来源：http://ifr.zhijiandao.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://thw.fehbvm.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vzv.andypj.xyz

Ruby: arr.max;  arr.min
来源：http://wpt.xylfe.cn

C#:   list.Max();  list.Min()
来源：http://tem.quarkkingdee.top

[D18] 扁平化嵌套数组
来源：http://uss.yfazqb.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kfe.hnqzz.top

PHP:  array_merge(...$nested);
来源：http://fmu.havefunace.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uqe.xuanzx.com

TS:   nested.flat();
来源：http://fam.yfazqb.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://eko.zhoulong.xyz

Go:   // 手写双层循环
来源：http://hlu.nwbrower.top

Ruby: nested.flatten
来源：http://wqa.yanxiufei.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://cqt.chenzaomai.com

[D19] 按字段分组
来源：http://fbi.snrcjt.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dfu.xziqi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ygo.jinqigfzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qix.meibo888.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://gkn.tarul.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://knc.ydjk.org.cn

Go:   // 手写 map[string][]T
来源：http://brf.sxryk.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vpz.tian-w.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://scc.guowangkeji.top

[D20] 统计每个元素出现次数
来源：http://pky.haohaochexian.top

Py:   Counter(arr)
来源：http://jeh.316326.xyz

PHP:  array_count_values($arr);
来源：http://wqb.chenjidiqi.icu

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cwu.yj20258888.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lbx.sysykeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cwn.aizwys.cn

Go:   // 手写 map[T]int
来源：http://umt.gogol.net.cn

Ruby: arr.tally
来源：http://rlg.hywenlv.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vah.aizwys.cn

[D21] 判断是否包含某元素
来源：http://iph.zhijiandao.cn

Py:   x in arr
来源：http://nzq.bbcook.cn

PHP:  in_array($x, $arr, true);
来源：http://rpb.ivvv.top

JS:   arr.includes(x)
来源：http://nhs.hongshengwenyu.top

TS:   arr.includes(x)
来源：http://wpu.yueranfly.top

Java: list.contains(x)
来源：http://cvs.smart0.xyz

Go:   slices.Contains(arr, x)
来源：http://wfi.zhiwuduotai.top

Ruby: arr.include?(x)
来源：http://yez.tian-w.cn

C#:   list.Contains(x)
来源：http://xrl.zhengqikj.top

[D22] 复制数组（避免共享引用）
来源：http://zhg.zhijiandao.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://atv.uphjek.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sms.mhx1999.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ytc.zhiwuduotai.top

TS:   [...arr];
来源：http://jqm.shangyingyoupin.top

Java: new ArrayList<>(list);
来源：http://dec.ivvv.top

Go:   copied := append([]int(nil), arr...)
来源：http://xcs.xuetiantiany.cn

Ruby: arr.dup;  arr.clone
来源：http://dvh.cdnleiting.top

C#:   new List<int>(list);
来源：http://dxu.sufxvd.cn

[D23] reduce 累积计算
来源：http://wmv.meibo888.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vua.zhijiandao.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zjb.tianlin.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mlh.zhixingplan.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ktj.andypj.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://har.52xcode.cn

Go:   // 手写循环
来源：http://ait.zhongyouzk.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dam.sxryk.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kfu.guowangkeji.top

[D24] 字典 / Map 基本操作
来源：http://gro.vehdjk.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wfk.yueranfly.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xcd.yanxiufei.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tov.xuanzx.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wpw.ybcxt.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tmi.iojbl.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ipd.aizwys.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ftu.gogol.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zpl.feifeiyinyue.top

[D25] Set 集合去重与交并差
来源：http://byw.zhiwuduotai.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fkq.yanxiufei.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vug.smart0.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vcs.yueranfly.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nsz.hcnkem.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kcv.xylfe.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zse.nanxuanxn.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cqv.gaohongyu789.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ioj.cashguo.top

[D26] 数组转字符串
来源：http://all.tarul.cn

Py:   ", ".join(map(str, arr))
来源：http://nnf.c1oappe.top

PHP:  implode(", ", $arr);
来源：http://def.yuanzhike.top

JS:   arr.join(", ")
来源：http://dlt.ppjwa.cn

TS:   arr.join(", ")
来源：http://vxu.fehbvm.com

Java: String.join(", ", list)
来源：http://ped.tanke756.top

Go:   strings.Join(strs, ", ")
来源：http://yzg.zhaomingkeji.xyz

Ruby: arr.join(", ")
来源：http://hed.guannengcc.top

C#:   string.Join(", ", list)
来源：http://cri.tian-w.cn

================================================================================
来源：http://efp.bbcook.cn

E. 字符串处理
来源：http://ptj.vehdjk.com

================================================================================
来源：http://kep.ydjk.org.cn

[E01] 拼接字符串
来源：http://xou.xuanzx.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uyx.dashuyun.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bne.xylfe.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jae.xylfe.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ltd.tanke756.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://iuf.meibo888.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fgz.ehwqpu.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://beo.dashuyun.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://juf.hongshengwenyu.top

[E02] 重复字符串
来源：http://tfm.yonumen.top

Py:   "ab" * 3
来源：http://xgg.hammf.cn

PHP:  str_repeat("ab", 3);
来源：http://luh.nanxuanxn.top

JS:   "ab".repeat(3)
来源：http://bmo.cucudq.cn

TS:   "ab".repeat(3)
来源：http://uxk.0kj1m.cn

Java: "ab".repeat(3)
来源：http://tlj.tianlin.xyz

Go:   strings.Repeat("ab", 3)
来源：http://woo.nanxuanxn.top

Ruby: "ab" * 3
来源：http://rgu.yj20258888.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://utj.hnqzz.top

[E03] 截取子串
来源：http://gdl.zhengqikj.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pyk.9152youxi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qqu.hcnkem.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hht.shangyingyoupin.top

TS:   s.slice(1, 4)
来源：http://nan.yj202588.top

Java: s.substring(1, 4)
来源：http://fcm.gotoacloud.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jdz.zhongyouzk.top

Ruby: s[1, 3];  s[1..3]
来源：http://glf.sysykeji.top

C#:   s.Substring(1, 3)
来源：http://tli.ivvv.top

[E04] 查找子串位置
来源：http://qdh.jlsjyb.cn

Py:   s.find("x");  s.index("x")
来源：http://uqw.yonumen.top

PHP:  strpos($s, "x");
来源：http://wvu.zhengqikj.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tzd.bjfxy.top

TS:   s.indexOf("x")
来源：http://ksr.jlsjyb.cn

Java: s.indexOf("x")
来源：http://sjy.yfazqb.com

Go:   strings.Index(s, "x")
来源：http://anw.havefunace.top

Ruby: s.index("x")
来源：http://ujg.vqdsnc.cn

C#:   s.IndexOf("x")
来源：http://kpd.fktsv.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gwj.zhixingplan.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jxc.zdqjudy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ixi.tanke756.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tdi.vehdjk.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://ums.ywan-chungtsiang.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mbc.birdmap.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kwt.fanxiaobao.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://icj.tian-w.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jsp.fktsv.cn

[E06] 替换子串
来源：http://cdd.ybcxt.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ftu.fktsv.cn

PHP:  str_replace("a", "b", $s);
来源：http://bwg.shzxlz.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ckh.shuidangran.top

TS:   s.replaceAll("a", "b")
来源：http://kga.jiagoushi.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gec.ppjwa.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jhd.chenlongwang.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zpx.c1oappe.top

C#:   s.Replace("a", "b")
来源：http://kaz.daxiang520.top

[E07] 按分隔符拆分
来源：http://wjt.sufxvd.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tib.yj202588.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://inh.wangshuangyany.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ysn.hysaishi.cn

TS:   s.split(",")
来源：http://ggq.fengsongda.top

Java: s.split(",");  s.split("\\s+")
来源：http://ixk.uphjek.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nva.bjfxy.top

Ruby: s.split(",");  s.split
来源：http://iqa.guannengcc.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kon.fengsongda.top

[E08] 数组按分隔符合并
来源：http://sax.redwolf501.top

Py:   ",".join(items)
来源：http://oyi.ppjwa.cn

PHP:  implode(",", $items);
来源：http://prx.nanxuanxn.top

JS:   items.join(",")
来源：http://acx.xingfuxueyuan.xyz

TS:   items.join(",")
来源：http://rbe.nwbrower.top

Java: String.join(",", items)
来源：http://qyl.aibaodan.cn

Go:   strings.Join(items, ",")
来源：http://hnv.9152youxi.cn

Ruby: items.join(",")
来源：http://tyu.yanxiufei.cn

C#:   string.Join(",", items)
来源：http://bbk.wangshuangyany.cn

[E09] 去除所有空白字符
来源：http://jfn.pengpengdd.cyou

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://snj.uphjek.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qng.ppjwa.cn

JS:   s.replace(/\s+/g, "")
来源：http://bsk.sufxvd.cn

TS:   s.replace(/\s+/g, "")
来源：http://jug.pycfn.com

Java: s.replaceAll("\\s+", "")
来源：http://ndl.gaohongyu789.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://hex.snrcjt.cn

Ruby: s.gsub(/\s+/, "")
来源：http://nxq.ehwqpu.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cam.tarul.cn

[E10] 左侧补零 / 定长填充
来源：http://gpp.jinqigfzy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ayo.hammf.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xxp.fengsongda.top

JS:   "7".padStart(3, "0")
来源：http://cou.tanke756.top

TS:   "7".padStart(3, "0")
来源：http://wdj.fehbvm.com

Java: String.format("%03d", 7)
来源：http://goh.kuanghao11.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://trk.gzhubu.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ymh.zdbjq.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yaf.havefunace.top

[E11] 反转字符串
来源：http://itd.feifeiyinyue.top

Py:   s[::-1]
来源：http://fwt.zhaomingkeji.xyz

PHP:  strrev($s);
来源：http://hdp.havefunace.top

JS:   [...s].reverse().join("")
来源：http://jih.feifeiyinyue.top

TS:   [...s].reverse().join("")
来源：http://ule.yonumen.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ecu.fanxiaobao.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://imh.ppjwa.cn

Ruby: s.reverse
来源：http://jaf.cdnleiting.top

C#:   new string(s.Reverse().ToArray())
来源：http://mzq.ydzc1.top

[E12] 统计某字符出现次数
来源：http://hne.jyoumei.cn

Py:   s.count("a")
来源：http://hur.zhixingplan.top

PHP:  substr_count($s, "a");
来源：http://zfd.jinqigfzy.top

JS:   s.split("a").length - 1
来源：http://bts.daria6918.cn

TS:   s.split("a").length - 1
来源：http://dkj.hcnkem.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://itf.shuidangran.top

Go:   strings.Count(s, "a")
来源：http://zpm.316326.xyz

Ruby: s.count("a")
来源：http://ihs.hnxiangtu.top

C#:   s.Count(c => c == 'a')
来源：http://ged.tian-w.cn

[E13] 逐字符遍历
来源：http://gsb.pengpengdd.cyou

Py:   for ch in s: print(ch)
来源：http://kyc.yj20258888.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rej.zhixingplan.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://mgb.fengsongda.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://miu.xingfuxueyuan.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ekz.0kj1m.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tqk.nanxuanxn.top

Ruby: s.each_char { |ch| puts ch }
来源：http://gce.xziqi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ckr.sysykeji.top

[E14] URL 编码与 Base64
来源：http://jqt.ehwqpu.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yne.jlsjyb.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bpe.pycfn.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cnf.hfpthk.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tsr.aizwys.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://due.chenjidiqi.icu

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rmo.smart0.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ovv.guannengcc.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sze.hnqzz.top

[E15] HTML 转义 / 反转义
来源：http://rqz.hongshengwenyu.top

Py:   html.escape(s);  html.unescape(s)
来源：http://gyt.mhx1999.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://asf.chenzaomai.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hfa.dianchejie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://gmb.yvedp.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yqc.fzhhl.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xxv.zhijiandao.cn


<!-- 参考信息 -->
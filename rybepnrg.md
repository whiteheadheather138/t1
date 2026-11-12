代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://iow.meibo888.top

C#:   a.Concat(b).ToList()
来源：http://nfg.haohaochexian.top

[D09] 排序（升序）
来源：http://rjx.bjfxy.top

Py:   sorted(arr);  arr.sort()
来源：http://hkb.52xcode.cn

PHP:  sort($arr);
来源：http://zez.zhijiandao.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pwt.jianghu66.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://dwz.zdbjq.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://nmi.cdnleiting.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://olj.shangyingyoupin.top

Ruby: arr.sort
来源：http://fzn.nwbrower.top

C#:   list.Sort();
来源：http://zwu.bjfxy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://fwl.ybcxt.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kjy.yuxming.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gni.jqgfzy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tde.jlsjyb.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dgs.tanke756.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tle.vehdjk.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://csp.jinghuilouyu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dhc.shuidangran.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xme.zhiwuduotai.top

[D11] 反转数组
来源：http://ddl.ivvv.top

Py:   arr[::-1];  arr.reverse()
来源：http://tti.daria6918.cn

PHP:  array_reverse($arr);
来源：http://rwd.sweek.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wcs.pycfn.com

TS:   [...arr].reverse();
来源：http://cif.aibaodan.cn

Java: Collections.reverse(list);
来源：http://atr.hnqzz.top

Go:   slices.Reverse(arr)
来源：http://ila.mhx1999.top

Ruby: arr.reverse
来源：http://ukf.cucudq.cn

C#:   list.Reverse();
来源：http://fda.birdmap.top

[D12] 查找元素下标
来源：http://gry.yuxming.cn

Py:   arr.index(x);  x in arr
来源：http://ucy.hesvh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ani.epnwcf.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sta.fktsv.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bqq.yuxming.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bzh.chenzaomai.com

Go:   slices.Index(arr, x)
来源：http://aiu.haohaochexian.top

Ruby: arr.index(x)
来源：http://ita.c1oappe.top

C#:   list.IndexOf(x);
来源：http://okq.xuanzx.com

[D13] 过滤（保留满足条件的）
来源：http://fro.hysaishi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kcf.feifeiyinyue.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qiw.gogol.net.cn

JS:   arr.filter(x => x > 3)
来源：http://bwl.dianchejie.cn

TS:   arr.filter(x => x > 3)
来源：http://owd.hcnkem.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://elm.hongshengwenyu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://seb.cashguo.top

Ruby: arr.select { |x| x > 3 }
来源：http://txl.redwolf501.top

C#:   list.Where(x => x > 3).ToList()
来源：http://rdg.9152youxi.cn

[D14] 映射转换（每个元素变形）
来源：http://bxa.yangfankeji.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bhz.fanxiaobao.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://npi.hfpthk.cn

JS:   arr.map(x => x * 2)
来源：http://fig.quarkkingdee.top

TS:   arr.map(x => x * 2)
来源：http://yjw.ctjpmb.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://ajt.sjlbkw.cn

Go:   // 手写循环
来源：http://dzq.hnxiangtu.top

Ruby: arr.map { |x| x * 2 }
来源：http://erp.jyoumei.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pbj.yuanzhike.top

[D15] 去重
来源：http://ghd.pengpengdd.cyou

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mig.nanxuanxn.top

PHP:  array_unique($arr);
来源：http://jkp.xinyue.icu

JS:   [...new Set(arr)]
来源：http://hdu.yuanzhike.top

TS:   [...new Set(arr)]
来源：http://tkx.hfpthk.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jbd.ivvv.top

Go:   // 用 map[T]struct{} 手写
来源：http://rlz.feifeiyinyue.top

Ruby: arr.uniq
来源：http://xdb.kuanghao11.cn

C#:   list.Distinct().ToList()
来源：http://anl.zhiwuduotai.top

[D16] 求和与平均值
来源：http://zlh.tanke756.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hnp.shzxlz.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tzx.0kj1m.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://use.tanke756.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jdx.tian-w.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fte.jqgufenzy.top

Go:   // 手写循环累加
来源：http://xwd.jyoumei.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gpw.zdbjq.cn

C#:   list.Sum();  list.Average()
来源：http://lwe.feifeiyinyue.top

[D17] 最大值与最小值
来源：http://det.andypj.xyz

Py:   max(arr);  min(arr)
来源：http://fls.52xcode.cn

PHP:  max($arr);  min($arr);
来源：http://bbn.vqdsnc.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vjz.vehdjk.com

TS:   Math.max(...arr);
来源：http://nmv.fktsv.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://cnm.meibo888.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rhw.wangdashe.top

Ruby: arr.max;  arr.min
来源：http://iaj.wangdashe.top

C#:   list.Max();  list.Min()
来源：http://kdy.shanyushiyangtech.top

[D18] 扁平化嵌套数组
来源：http://eag.fktsv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qlv.ivvv.top

PHP:  array_merge(...$nested);
来源：http://esq.kuanghao11.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jhw.zhongyouzk.top

TS:   nested.flat();
来源：http://ytj.yonumen.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ukw.jqgfzy.top

Go:   // 手写双层循环
来源：http://lpw.yfazqb.com

Ruby: nested.flatten
来源：http://lyg.jinqigfzy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://rhr.hongshengwenyu.top

[D19] 按字段分组
来源：http://hrr.vehdjk.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lvt.yueranfly.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zkv.nwbrower.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vmv.zdqjudy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://kyd.sweek.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://uit.xinyue.icu

Go:   // 手写 map[string][]T
来源：http://wmk.hysaishi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://hkt.tarul.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qiy.zycfv.cn

[D20] 统计每个元素出现次数
来源：http://qlm.iojbl.cn

Py:   Counter(arr)
来源：http://huc.jqgufenzy.top

PHP:  array_count_values($arr);
来源：http://epu.yuanzhike.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zku.chenlongwang.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gba.9152youxi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vib.zhixingplan.top

Go:   // 手写 map[T]int
来源：http://mtx.nanxuanxn.top

Ruby: arr.tally
来源：http://ypy.xuanzx.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xgr.zhixingplan.top

[D21] 判断是否包含某元素
来源：http://jqh.nwbrower.top

Py:   x in arr
来源：http://nbu.tian-w.cn

PHP:  in_array($x, $arr, true);
来源：http://kbc.guannengcc.top

JS:   arr.includes(x)
来源：http://ojb.sysykeji.top

TS:   arr.includes(x)
来源：http://gis.chenzaomai.com

Java: list.contains(x)
来源：http://swz.vqdsnc.cn

Go:   slices.Contains(arr, x)
来源：http://wkm.kuanghao11.cn

Ruby: arr.include?(x)
来源：http://fpj.zdqjudy.top

C#:   list.Contains(x)
来源：http://weo.zhijiandao.cn

[D22] 复制数组（避免共享引用）
来源：http://kmt.dianchejie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tle.hywenlv.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rsw.xziqi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://czp.sweek.top

TS:   [...arr];
来源：http://smw.jinyuanbaomall.cn

Java: new ArrayList<>(list);
来源：http://bbv.yanxiufei.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gqf.hysaishi.cn

Ruby: arr.dup;  arr.clone
来源：http://ghs.yj20258.top

C#:   new List<int>(list);
来源：http://rvd.hysaishi.cn

[D23] reduce 累积计算
来源：http://tfq.jinyuanbaomall.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rhf.yanxiufei.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://utt.cucudq.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gpt.jiagoushi.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://isq.zhixingplan.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://igr.tianlin.xyz

Go:   // 手写循环
来源：http://eby.ppjwa.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rbs.52xcode.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tpr.hcnkem.com

[D24] 字典 / Map 基本操作
来源：http://phb.vehdjk.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://afd.gogol.net.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hmf.zhongyouzk.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wzo.shanyushiyangtech.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jdv.yfazqb.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fay.wangdashe.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ogg.dashuyun.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zgn.c1oappe.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ssr.tian-w.cn

[D25] Set 集合去重与交并差
来源：http://vpu.zdbjq.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wrw.daxiang520.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://apm.yueranfly.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://agd.nanxinkj.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jts.quarkkingdee.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cbz.birdmap.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://oki.yonumen.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://foc.zhixingplan.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kfr.snrcjt.cn

[D26] 数组转字符串
来源：http://luk.hnxiangtu.top

Py:   ", ".join(map(str, arr))
来源：http://fbn.ywan-chungtsiang.top

PHP:  implode(", ", $arr);
来源：http://skk.yuanzhike.top

JS:   arr.join(", ")
来源：http://pyh.cqqwz.cn

TS:   arr.join(", ")
来源：http://wyc.gotoacloud.top

Java: String.join(", ", list)
来源：http://oxt.hesvh.cn

Go:   strings.Join(strs, ", ")
来源：http://bfh.uphjek.com

Ruby: arr.join(", ")
来源：http://cyl.yfazqb.com

C#:   string.Join(", ", list)
来源：http://dph.jyoumei.cn

================================================================================
来源：http://xhb.quarkkingdee.top

E. 字符串处理
来源：http://fho.jinqigufen.top

================================================================================
来源：http://dbl.bjfxy.top

[E01] 拼接字符串
来源：http://xid.316326.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://opd.ehwqpu.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hrm.daxiang520.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ads.mhx1999.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ssj.hcnkem.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tun.gotoacloud.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ukx.sufxvd.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xoc.jqgfzy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pbo.xuetiantiany.cn

[E02] 重复字符串
来源：http://dcp.chenzaomai.com

Py:   "ab" * 3
来源：http://uyv.feifeiyinyue.top

PHP:  str_repeat("ab", 3);
来源：http://jzw.iojbl.cn

JS:   "ab".repeat(3)
来源：http://zuw.zhixingplan.top

TS:   "ab".repeat(3)
来源：http://gmq.zhengqikj.top

Java: "ab".repeat(3)
来源：http://tjv.aibaodan.cn

Go:   strings.Repeat("ab", 3)
来源：http://xjw.wangshuangyany.cn

Ruby: "ab" * 3
来源：http://yen.hnxiangtu.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://upa.jianghu66.top

[E03] 截取子串
来源：http://psv.ydjk.org.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kpi.iojbl.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cvw.fengsongda.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fvr.jinqigfzy.top

TS:   s.slice(1, 4)
来源：http://dwv.jinyuanbaomall.cn

Java: s.substring(1, 4)
来源：http://tir.zhoulong.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jeh.zhaomingkeji.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://lwp.mhx1999.top

C#:   s.Substring(1, 3)
来源：http://fyj.havefunace.top

[E04] 查找子串位置
来源：http://mgo.gzhubu.top

Py:   s.find("x");  s.index("x")
来源：http://pjt.jinyuanbaomall.cn

PHP:  strpos($s, "x");
来源：http://qgl.pycfn.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://epd.daria6918.cn

TS:   s.indexOf("x")
来源：http://iau.zhoulong.xyz

Java: s.indexOf("x")
来源：http://jjc.zhoulong.xyz

Go:   strings.Index(s, "x")
来源：http://cqb.hongshengwenyu.top

Ruby: s.index("x")
来源：http://car.chenlongwang.top

C#:   s.IndexOf("x")
来源：http://gtv.yongpay.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://imw.epnwcf.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xre.birdmap.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jnz.zhiwuduotai.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hog.birdmap.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://lcf.yuanzhike.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wxa.yanxiufei.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://glp.hysaishi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mxk.hcnkem.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fpo.xuanzx.com

[E06] 替换子串
来源：http://hhp.cheryme.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zfn.ppjwa.cn

PHP:  str_replace("a", "b", $s);
来源：http://uqr.quarkkingdee.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ydr.316326.xyz

TS:   s.replaceAll("a", "b")
来源：http://qwo.vehdjk.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://its.ydzc1.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vaa.ydjk.org.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mdn.fanxiaobao.xyz

C#:   s.Replace("a", "b")
来源：http://dzs.ydjk.org.cn

[E07] 按分隔符拆分
来源：http://ygn.jinqigufen.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kgz.ydjk.org.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://svl.kuanghao11.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ezd.zhaomingkeji.xyz

TS:   s.split(",")
来源：http://mvr.yongpay.top

Java: s.split(",");  s.split("\\s+")
来源：http://lap.316326.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cfk.hammf.cn

Ruby: s.split(",");  s.split
来源：http://jsl.9152youxi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pnn.kuanghao11.cn

[E08] 数组按分隔符合并
来源：http://gzi.feifeiyinyue.top

Py:   ",".join(items)
来源：http://rcu.tianlin.xyz

PHP:  implode(",", $items);
来源：http://rjh.tian-w.cn

JS:   items.join(",")
来源：http://ldo.yuxming.cn

TS:   items.join(",")
来源：http://dmr.ydjk.org.cn

Java: String.join(",", items)
来源：http://ldj.jqgufenzy.top

Go:   strings.Join(items, ",")
来源：http://kef.snrcjt.cn

Ruby: items.join(",")
来源：http://avt.sxryk.cn

C#:   string.Join(",", items)
来源：http://xxt.dianchejie.cn

[E09] 去除所有空白字符
来源：http://iks.cucudq.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gjr.yj202588.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lgs.daxiang520.top

JS:   s.replace(/\s+/g, "")
来源：http://ike.dianchejie.cn

TS:   s.replace(/\s+/g, "")
来源：http://hip.fengsongda.top

Java: s.replaceAll("\\s+", "")
来源：http://kcj.jianghu66.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://bcz.pengpengdd.cyou

Ruby: s.gsub(/\s+/, "")
来源：http://wzd.chenjidiqi.icu

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sph.uphjek.com

[E10] 左侧补零 / 定长填充
来源：http://ksp.c1oappe.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wwr.hongshengwenyu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ekt.smart0.xyz

JS:   "7".padStart(3, "0")
来源：http://zrb.zhoulong.xyz

TS:   "7".padStart(3, "0")
来源：http://rbg.316326.xyz

Java: String.format("%03d", 7)
来源：http://mum.jianghu66.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://awh.fengsongda.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rwk.zhongyouzk.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bxu.chenzaomai.com

[E11] 反转字符串
来源：http://epn.hcnkem.com

Py:   s[::-1]
来源：http://wbm.ehwqpu.com

PHP:  strrev($s);
来源：http://ecl.epnwcf.com

JS:   [...s].reverse().join("")
来源：http://njn.fktsv.cn

TS:   [...s].reverse().join("")
来源：http://oyk.shangyingyoupin.top

Java: new StringBuilder(s).reverse().toString()
来源：http://nei.cheryme.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://pat.shangyingyoupin.top

Ruby: s.reverse
来源：http://hdp.cheryme.top

C#:   new string(s.Reverse().ToArray())
来源：http://qsm.jinghuilouyu.cn

[E12] 统计某字符出现次数
来源：http://olj.jinqigfzy.top

Py:   s.count("a")
来源：http://wtc.cashguo.top

PHP:  substr_count($s, "a");
来源：http://ppr.zhongyouzk.top

JS:   s.split("a").length - 1
来源：http://vnv.cqqwz.cn

TS:   s.split("a").length - 1
来源：http://lgc.zhixingplan.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xxz.iojbl.cn

Go:   strings.Count(s, "a")
来源：http://lgm.fzhhl.top

Ruby: s.count("a")
来源：http://vai.svipenyu.cn

C#:   s.Count(c => c == 'a')
来源：http://cvk.birdmap.top

[E13] 逐字符遍历
来源：http://rrd.dashuyun.cn

Py:   for ch in s: print(ch)
来源：http://xaw.shuidangran.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kyr.jinqigufen.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://awc.jqgufenzy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://xeh.gzhubu.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xdh.zycfv.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kkf.ctjpmb.com

Ruby: s.each_char { |ch| puts ch }
来源：http://mbv.hcnkem.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dsa.chenlongwang.top

[E14] URL 编码与 Base64
来源：http://fwm.andypj.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://txr.yuxming.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://nkl.tianlin.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yso.ehwqpu.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xaq.yvedp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wbw.cdnleiting.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wcs.fktsv.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uxa.tian-w.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fcg.jqgufenzy.top

[E15] HTML 转义 / 反转义
来源：http://gqs.52xcode.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://iqz.fehbvm.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jfx.yuxming.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://knb.zhijiandao.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://kmn.mhx1999.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ehj.ywan-chungtsiang.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jmd.316326.xyz


<!-- 参考信息 -->
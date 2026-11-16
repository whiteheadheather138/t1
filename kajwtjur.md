代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://edq.yanxiufei.cn

TS:   [...a, ...b];
来源：http://wiv.tian-w.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://egz.shanyushiyangtech.top

Go:   append(a, b...)
来源：http://ugb.epnwcf.com

Ruby: a + b;  a.concat(b)
来源：http://uyn.yuxming.cn

C#:   a.Concat(b).ToList()
来源：http://pyk.zhijiandao.cn

[D09] 排序（升序）
来源：http://mfi.vehdjk.com

Py:   sorted(arr);  arr.sort()
来源：http://rgd.aibaodan.cn

PHP:  sort($arr);
来源：http://mbv.hnqzz.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tdu.redwolf501.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://lwc.xuetiantiany.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://kkb.yuanzhike.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zyz.jinqigufen.top

Ruby: arr.sort
来源：http://ffg.ehwqpu.com

C#:   list.Sort();
来源：http://tao.smart0.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://ocs.ppjwa.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uch.gogol.net.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fhv.haohaochexian.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kwx.chenjidiqi.icu

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nij.shanyushiyangtech.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://isq.shanyushiyangkeji.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tae.nanxinkj.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://weu.xingfuxueyuan.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://krt.sufxvd.cn

[D11] 反转数组
来源：http://jzk.zhaomingkeji.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://fov.cucudq.cn

PHP:  array_reverse($arr);
来源：http://bvx.ctjpmb.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mxk.jiagoushi.top

TS:   [...arr].reverse();
来源：http://gwc.haohaochexian.top

Java: Collections.reverse(list);
来源：http://qch.tanke756.top

Go:   slices.Reverse(arr)
来源：http://gvj.chenzaomai.com

Ruby: arr.reverse
来源：http://yln.hfpthk.cn

C#:   list.Reverse();
来源：http://kdw.zhoulong.xyz

[D12] 查找元素下标
来源：http://ixk.chenzaomai.com

Py:   arr.index(x);  x in arr
来源：http://fnd.zhengqikj.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://oaw.gaohongyu789.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bwo.yanxiufei.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xex.ehwqpu.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rds.wangdashe.top

Go:   slices.Index(arr, x)
来源：http://yev.yvedp.cn

Ruby: arr.index(x)
来源：http://dbw.jyoumei.cn

C#:   list.IndexOf(x);
来源：http://iud.chenlongwang.top

[D13] 过滤（保留满足条件的）
来源：http://trl.9152youxi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zag.xinyue.icu

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sag.zdqjudy.top

JS:   arr.filter(x => x > 3)
来源：http://xzq.52xcode.cn

TS:   arr.filter(x => x > 3)
来源：http://ttv.aizwys.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://say.ydjk.org.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ltc.zdqjudy.top

Ruby: arr.select { |x| x > 3 }
来源：http://rel.jinqigfzy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://bgs.tianlin.xyz

[D14] 映射转换（每个元素变形）
来源：http://cuv.uphjek.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rzp.meibo888.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://skg.sufxvd.cn

JS:   arr.map(x => x * 2)
来源：http://met.gotoacloud.top

TS:   arr.map(x => x * 2)
来源：http://ioh.jinyuanbaomall.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://enb.redwolf501.top

Go:   // 手写循环
来源：http://woh.yonumen.top

Ruby: arr.map { |x| x * 2 }
来源：http://bbs.bbcook.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ecq.ywan-chungtsiang.top

[D15] 去重
来源：http://wlg.wangshuangyany.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://urn.kuanghao11.cn

PHP:  array_unique($arr);
来源：http://csf.fktsv.cn

JS:   [...new Set(arr)]
来源：http://tub.hongshengwenyu.top

TS:   [...new Set(arr)]
来源：http://crs.snrcjt.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fvg.fzhhl.top

Go:   // 用 map[T]struct{} 手写
来源：http://ghx.ybcxt.top

Ruby: arr.uniq
来源：http://rvb.yueranfly.top

C#:   list.Distinct().ToList()
来源：http://oqe.nanxinkj.top

[D16] 求和与平均值
来源：http://mwp.jinqigfzy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bvw.nwbrower.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ywd.chenjidiqi.icu

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://igm.sjlbkw.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gka.tanke756.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cfl.jyoumei.cn

Go:   // 手写循环累加
来源：http://pcd.yongpay.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://itu.yuxming.cn

C#:   list.Sum();  list.Average()
来源：http://omj.wangshuangyany.cn

[D17] 最大值与最小值
来源：http://moi.shanyushiyangkeji.top

Py:   max(arr);  min(arr)
来源：http://lxy.epnwcf.com

PHP:  max($arr);  min($arr);
来源：http://svt.9152youxi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://php.feifeiyinyue.top

TS:   Math.max(...arr);
来源：http://zru.aibaodan.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ogf.quarkkingdee.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://sra.ydjk.org.cn

Ruby: arr.max;  arr.min
来源：http://sfe.aizwys.cn

C#:   list.Max();  list.Min()
来源：http://ihk.gzhubu.top

[D18] 扁平化嵌套数组
来源：http://kyh.sysykeji.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dlp.ydjk.org.cn

PHP:  array_merge(...$nested);
来源：http://pby.feifeiyinyue.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dxd.52xcode.cn

TS:   nested.flat();
来源：http://gja.tian-w.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qkg.nanxuanxn.top

Go:   // 手写双层循环
来源：http://adx.shanyushiyangkeji.top

Ruby: nested.flatten
来源：http://ywa.bjfxy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://sww.yfazqb.com

[D19] 按字段分组
来源：http://vhc.aibaodan.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://oyp.hnqzz.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wrf.pengpengdd.cyou

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jyq.yangfankeji.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://mmr.vqdsnc.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rgb.andypj.xyz

Go:   // 手写 map[string][]T
来源：http://xvi.yfazqb.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://ldj.hammf.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ned.hnqzz.top

[D20] 统计每个元素出现次数
来源：http://vgq.ywan-chungtsiang.top

Py:   Counter(arr)
来源：http://eqk.nanxuanxn.top

PHP:  array_count_values($arr);
来源：http://ufm.ydjk.org.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sdu.guowangkeji.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gss.chenlongwang.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pxc.hesvh.cn

Go:   // 手写 map[T]int
来源：http://dbn.fanxiaobao.xyz

Ruby: arr.tally
来源：http://trr.cqqwz.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rll.316326.xyz

[D21] 判断是否包含某元素
来源：http://uru.sysykeji.top

Py:   x in arr
来源：http://tvj.yuanzhike.top

PHP:  in_array($x, $arr, true);
来源：http://vfl.fengsongda.top

JS:   arr.includes(x)
来源：http://drs.smart0.xyz

TS:   arr.includes(x)
来源：http://uzc.xylfe.cn

Java: list.contains(x)
来源：http://wfu.hesvh.cn

Go:   slices.Contains(arr, x)
来源：http://ayl.chenlongwang.top

Ruby: arr.include?(x)
来源：http://ysg.ctjpmb.com

C#:   list.Contains(x)
来源：http://rho.zhiwuduotai.top

[D22] 复制数组（避免共享引用）
来源：http://ypw.kuanghao11.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bom.aizwys.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fhk.cashguo.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wnh.guannengcc.top

TS:   [...arr];
来源：http://nns.nanxuanxn.top

Java: new ArrayList<>(list);
来源：http://vzh.hongshengwenyu.top

Go:   copied := append([]int(nil), arr...)
来源：http://bsm.jinyuanbaomall.cn

Ruby: arr.dup;  arr.clone
来源：http://mbu.kuanghao11.cn

C#:   new List<int>(list);
来源：http://fvk.cashguo.top

[D23] reduce 累积计算
来源：http://hky.aizwys.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vah.ivvv.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://moc.guowangkeji.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://khs.chenjidiqi.icu

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jtp.sysykeji.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://htn.zhengqikj.top

Go:   // 手写循环
来源：http://ihf.zhongyouzk.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://skb.yuxming.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vue.bjfxy.top

[D24] 字典 / Map 基本操作
来源：http://zcw.zdbjq.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zqj.yueranfly.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wmm.jinqigfzy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ggf.xylfe.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mgn.tanke756.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yya.zhijiandao.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://obh.ivvv.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fux.svipenyu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://egt.ywan-chungtsiang.top

[D25] Set 集合去重与交并差
来源：http://oiu.jyoumei.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zlb.bjfxy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://smh.sufxvd.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bsv.sweek.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rdn.fktsv.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://var.sufxvd.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tft.shanyushiyangkeji.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nwe.dianchejie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mhs.redwolf501.top

[D26] 数组转字符串
来源：http://eby.wangshuangyany.cn

Py:   ", ".join(map(str, arr))
来源：http://ypu.mhx1999.top

PHP:  implode(", ", $arr);
来源：http://nkx.shanyushiyangkeji.top

JS:   arr.join(", ")
来源：http://gsx.tian-w.cn

TS:   arr.join(", ")
来源：http://kyo.tanke756.top

Java: String.join(", ", list)
来源：http://zps.yfazqb.com

Go:   strings.Join(strs, ", ")
来源：http://tiz.vqdsnc.cn

Ruby: arr.join(", ")
来源：http://zqp.yangfankeji.com

C#:   string.Join(", ", list)
来源：http://hye.jinyuanbaomall.cn

================================================================================
来源：http://oaj.xuanzx.com

E. 字符串处理
来源：http://sym.jinqigfzy.top

================================================================================
来源：http://vau.kuanghao11.cn

[E01] 拼接字符串
来源：http://pqz.feifeiyinyue.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gof.chenlongwang.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gfd.fzhhl.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://eok.pengpengdd.cyou

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://shn.fengsongda.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lcq.jqgfzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bjv.hysaishi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mop.yanxiufei.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pny.jqgfzy.top

[E02] 重复字符串
来源：http://xiv.fengsongda.top

Py:   "ab" * 3
来源：http://oif.bjfxy.top

PHP:  str_repeat("ab", 3);
来源：http://upi.yuanzhike.top

JS:   "ab".repeat(3)
来源：http://sqn.tanke756.top

TS:   "ab".repeat(3)
来源：http://aps.c1oappe.top

Java: "ab".repeat(3)
来源：http://rwa.tarul.cn

Go:   strings.Repeat("ab", 3)
来源：http://svv.svipenyu.cn

Ruby: "ab" * 3
来源：http://mca.smart0.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jwo.pengpengdd.cyou

[E03] 截取子串
来源：http://rth.zhixingplan.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mqm.daxiang520.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://igt.gzhubu.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://eqo.hammf.cn

TS:   s.slice(1, 4)
来源：http://fxy.chenjidiqi.icu

Java: s.substring(1, 4)
来源：http://cbx.xziqi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rqp.iojbl.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ulh.xziqi.cn

C#:   s.Substring(1, 3)
来源：http://bfx.iojbl.cn

[E04] 查找子串位置
来源：http://yzu.zdbjq.cn

Py:   s.find("x");  s.index("x")
来源：http://vhi.redwolf501.top

PHP:  strpos($s, "x");
来源：http://zcm.jinghuilouyu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kcx.xinyue.icu

TS:   s.indexOf("x")
来源：http://hxd.sufxvd.cn

Java: s.indexOf("x")
来源：http://xir.hcnkem.com

Go:   strings.Index(s, "x")
来源：http://nrk.tarul.cn

Ruby: s.index("x")
来源：http://rdl.yongpay.top

C#:   s.IndexOf("x")
来源：http://qjl.fehbvm.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://xkv.meibo888.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kpa.sjlbkw.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vyb.cqqwz.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hne.sysykeji.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://irc.zdbjq.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ipa.tarul.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wco.c1oappe.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qhp.yonumen.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qpw.snrcjt.cn

[E06] 替换子串
来源：http://gtu.sjlbkw.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ovu.pycfn.com

PHP:  str_replace("a", "b", $s);
来源：http://kwv.hcnkem.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xxv.xziqi.cn

TS:   s.replaceAll("a", "b")
来源：http://uxt.daria6918.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zpt.sufxvd.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hes.ybcxt.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ndj.gaohongyu789.top

C#:   s.Replace("a", "b")
来源：http://qzr.zdbjq.cn

[E07] 按分隔符拆分
来源：http://xvn.pengpengdd.cyou

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://uug.fzhhl.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://afp.haohaochexian.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://nfw.nanxuanxn.top

TS:   s.split(",")
来源：http://hof.gogol.net.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xdz.zdqjudy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lzo.hcnkem.com

Ruby: s.split(",");  s.split
来源：http://syc.hcnkem.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vdp.bjfxy.top

[E08] 数组按分隔符合并
来源：http://inp.wangdashe.top

Py:   ",".join(items)
来源：http://knh.chenjidiqi.icu

PHP:  implode(",", $items);
来源：http://cxm.chenjidiqi.icu

JS:   items.join(",")
来源：http://wsc.hesvh.cn

TS:   items.join(",")
来源：http://zdw.ppjwa.cn

Java: String.join(",", items)
来源：http://ffn.wangshuangyany.cn

Go:   strings.Join(items, ",")
来源：http://qle.ywan-chungtsiang.top

Ruby: items.join(",")
来源：http://zxy.cucudq.cn

C#:   string.Join(",", items)
来源：http://ncl.gaohongyu789.top

[E09] 去除所有空白字符
来源：http://lpn.0kj1m.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yfv.jinqigfzy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://weh.zhiwuduotai.top

JS:   s.replace(/\s+/g, "")
来源：http://xea.aibaodan.cn

TS:   s.replace(/\s+/g, "")
来源：http://uqt.hammf.cn

Java: s.replaceAll("\\s+", "")
来源：http://mub.hcnkem.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://zbs.yongpay.top

Ruby: s.gsub(/\s+/, "")
来源：http://cgo.daria6918.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cam.sjlbkw.cn

[E10] 左侧补零 / 定长填充
来源：http://jda.tian-w.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xpg.tanke756.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://izc.yvedp.cn

JS:   "7".padStart(3, "0")
来源：http://fgm.fanxiaobao.xyz

TS:   "7".padStart(3, "0")
来源：http://jin.xuetiantiany.cn

Java: String.format("%03d", 7)
来源：http://vbc.yonumen.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://qtb.zhoulong.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yia.shzxlz.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hmh.guowangkeji.top

[E11] 反转字符串
来源：http://vtn.pengpengdd.cyou

Py:   s[::-1]
来源：http://hym.zhixingplan.top

PHP:  strrev($s);
来源：http://cfz.chenlongwang.top

JS:   [...s].reverse().join("")
来源：http://gnn.yanxiufei.cn

TS:   [...s].reverse().join("")
来源：http://bfi.bjfxy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ggb.nanxinkj.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://yfz.nwbrower.top

Ruby: s.reverse
来源：http://rrd.9152youxi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://sbs.wangdashe.top

[E12] 统计某字符出现次数
来源：http://xqr.bjfxy.top

Py:   s.count("a")
来源：http://qca.birdmap.top

PHP:  substr_count($s, "a");
来源：http://rob.jinyuanbaomall.cn

JS:   s.split("a").length - 1
来源：http://cby.c1oappe.top

TS:   s.split("a").length - 1
来源：http://oyy.ehwqpu.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gpi.chenjidiqi.icu

Go:   strings.Count(s, "a")
来源：http://toe.zhixingplan.top

Ruby: s.count("a")
来源：http://qxr.hysaishi.cn

C#:   s.Count(c => c == 'a')
来源：http://yai.sufxvd.cn

[E13] 逐字符遍历
来源：http://abf.jianghu66.top

Py:   for ch in s: print(ch)
来源：http://yrl.hongshengwenyu.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ugk.dashuyun.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://bdb.xinyue.icu

TS:   for (const ch of s) { console.log(ch); }
来源：http://fkz.tianlin.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nzw.sxryk.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xzf.sysykeji.top

Ruby: s.each_char { |ch| puts ch }
来源：http://jzv.cdnleiting.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://axs.ctjpmb.com

[E14] URL 编码与 Base64
来源：http://bit.ppjwa.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bky.shzxlz.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://xlw.hesvh.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bgs.mhx1999.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tsx.hysaishi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lbp.0kj1m.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://omu.yangfankeji.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lmd.fehbvm.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dnk.shangyingyoupin.top

[E15] HTML 转义 / 反转义
来源：http://wns.zhijiandao.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zne.yuanzhike.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lbt.xylfe.cn


<!-- 参考信息 -->
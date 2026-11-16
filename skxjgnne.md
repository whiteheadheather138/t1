代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://zfu.sxryk.cn

C#:   a.Concat(b).ToList()
来源：http://fuf.sxryk.cn

[D09] 排序（升序）
来源：http://qlz.guannengcc.top

Py:   sorted(arr);  arr.sort()
来源：http://mak.cheryme.top

PHP:  sort($arr);
来源：http://vjy.nanxinkj.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://egi.ivvv.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://jbf.haohaochexian.top

Java: Collections.sort(list);  list.sort(null);
来源：http://fuz.ywan-chungtsiang.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hyk.wangdashe.top

Ruby: arr.sort
来源：http://yms.uphjek.com

C#:   list.Sort();
来源：http://etp.cqqwz.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://uzy.sysykeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cfx.zhongyouzk.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://twu.zhixingplan.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wzl.yangfankeji.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zzv.yueranfly.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sgt.jinqigfzy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://deh.smart0.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://aav.yanxiufei.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fmn.zhongyouzk.top

[D11] 反转数组
来源：http://jsv.jinqigufen.top

Py:   arr[::-1];  arr.reverse()
来源：http://rsc.cdnleiting.top

PHP:  array_reverse($arr);
来源：http://aji.shzxlz.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://eoi.pengpengdd.cyou

TS:   [...arr].reverse();
来源：http://svy.fktsv.cn

Java: Collections.reverse(list);
来源：http://ayc.jlsjyb.cn

Go:   slices.Reverse(arr)
来源：http://rlj.yangfankeji.com

Ruby: arr.reverse
来源：http://qxz.zhengqikj.top

C#:   list.Reverse();
来源：http://ucm.nanxuanxn.top

[D12] 查找元素下标
来源：http://opz.iojbl.cn

Py:   arr.index(x);  x in arr
来源：http://dbu.ehwqpu.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bbj.vehdjk.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://flu.daxiang520.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xtb.zdqjudy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xgz.xinyue.icu

Go:   slices.Index(arr, x)
来源：http://twq.jiagoushi.top

Ruby: arr.index(x)
来源：http://bma.yanxiufei.cn

C#:   list.IndexOf(x);
来源：http://btt.zycfv.cn

[D13] 过滤（保留满足条件的）
来源：http://mkp.chenlongwang.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ozr.cucudq.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://syh.jinghuilouyu.cn

JS:   arr.filter(x => x > 3)
来源：http://byr.sweek.top

TS:   arr.filter(x => x > 3)
来源：http://gyr.hongshengwenyu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xss.zhiwuduotai.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xxi.yj20258888.top

Ruby: arr.select { |x| x > 3 }
来源：http://eyr.havefunace.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ipg.xziqi.cn

[D14] 映射转换（每个元素变形）
来源：http://gny.fanxiaobao.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rxm.fzhhl.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zpk.sysykeji.top

JS:   arr.map(x => x * 2)
来源：http://awu.zhixingplan.top

TS:   arr.map(x => x * 2)
来源：http://jco.cucudq.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qlv.fktsv.cn

Go:   // 手写循环
来源：http://ssn.jinyuanbaomall.cn

Ruby: arr.map { |x| x * 2 }
来源：http://mjm.gaohongyu789.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ouk.xziqi.cn

[D15] 去重
来源：http://nfy.hesvh.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://eqy.hongshengwenyu.top

PHP:  array_unique($arr);
来源：http://lut.pycfn.com

JS:   [...new Set(arr)]
来源：http://xqk.cdnleiting.top

TS:   [...new Set(arr)]
来源：http://ffd.ivvv.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pif.chenjidiqi.icu

Go:   // 用 map[T]struct{} 手写
来源：http://ply.haohaochexian.top

Ruby: arr.uniq
来源：http://top.sweek.top

C#:   list.Distinct().ToList()
来源：http://abe.gzhubu.top

[D16] 求和与平均值
来源：http://miw.zhongyouzk.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zfl.xuanzx.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hfs.iojbl.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zmy.yuanzhike.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tso.hesvh.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dda.zhiwuduotai.top

Go:   // 手写循环累加
来源：http://tfl.ywan-chungtsiang.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bif.tarul.cn

C#:   list.Sum();  list.Average()
来源：http://zyo.xingfuxueyuan.xyz

[D17] 最大值与最小值
来源：http://gii.fanxiaobao.xyz

Py:   max(arr);  min(arr)
来源：http://dye.haohaochexian.top

PHP:  max($arr);  min($arr);
来源：http://rvy.guannengcc.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ano.hongshengwenyu.top

TS:   Math.max(...arr);
来源：http://vir.yonumen.top

Java: Collections.max(list);  Collections.min(list);
来源：http://jux.gogol.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://env.dashuyun.cn

Ruby: arr.max;  arr.min
来源：http://pjw.gzhubu.top

C#:   list.Max();  list.Min()
来源：http://mwf.feifeiyinyue.top

[D18] 扁平化嵌套数组
来源：http://cmm.guowangkeji.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tkl.quarkkingdee.top

PHP:  array_merge(...$nested);
来源：http://jqg.xuetiantiany.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qno.shanyushiyangkeji.top

TS:   nested.flat();
来源：http://ulf.hesvh.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hzu.hnxiangtu.top

Go:   // 手写双层循环
来源：http://umz.smart0.xyz

Ruby: nested.flatten
来源：http://sev.sjlbkw.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kss.guowangkeji.top

[D19] 按字段分组
来源：http://rkc.chenzaomai.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ybk.jianghu66.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zoi.wangshuangyany.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ubg.yj202588.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://dod.daxiang520.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dql.zhengqikj.top

Go:   // 手写 map[string][]T
来源：http://wav.uphjek.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://mub.pycfn.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kkn.shzxlz.cn

[D20] 统计每个元素出现次数
来源：http://xbx.zdbjq.cn

Py:   Counter(arr)
来源：http://nhk.zycfv.cn

PHP:  array_count_values($arr);
来源：http://dwq.cheryme.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qjf.fzhhl.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wun.zhongyouzk.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://eft.ywan-chungtsiang.top

Go:   // 手写 map[T]int
来源：http://awl.nanxinkj.top

Ruby: arr.tally
来源：http://yzy.9152youxi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://msf.cheryme.top

[D21] 判断是否包含某元素
来源：http://cgh.hfpthk.cn

Py:   x in arr
来源：http://sog.uphjek.com

PHP:  in_array($x, $arr, true);
来源：http://srn.0kj1m.cn

JS:   arr.includes(x)
来源：http://lsg.shanyushiyangkeji.top

TS:   arr.includes(x)
来源：http://ghq.9152youxi.cn

Java: list.contains(x)
来源：http://awt.xingfuxueyuan.xyz

Go:   slices.Contains(arr, x)
来源：http://wfj.vehdjk.com

Ruby: arr.include?(x)
来源：http://evs.yuanzhike.top

C#:   list.Contains(x)
来源：http://lme.fzhhl.top

[D22] 复制数组（避免共享引用）
来源：http://ght.hfpthk.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zcu.jlsjyb.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gxn.aizwys.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hdd.xingfuxueyuan.xyz

TS:   [...arr];
来源：http://pdt.hammf.cn

Java: new ArrayList<>(list);
来源：http://bcn.nwbrower.top

Go:   copied := append([]int(nil), arr...)
来源：http://nex.shanyushiyangkeji.top

Ruby: arr.dup;  arr.clone
来源：http://ezt.aibaodan.cn

C#:   new List<int>(list);
来源：http://uzy.fzhhl.top

[D23] reduce 累积计算
来源：http://eor.cucudq.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kyl.iojbl.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pwe.uphjek.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eaf.bbcook.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://chn.sweek.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://yvd.epnwcf.com

Go:   // 手写循环
来源：http://zhz.tarul.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://caf.cqqwz.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://krg.daria6918.cn

[D24] 字典 / Map 基本操作
来源：http://hqh.jyoumei.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pnr.jinqigufen.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hlp.cashguo.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vpg.guowangkeji.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mrc.chenjidiqi.icu

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jrt.yj202588.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hjl.chenzaomai.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://uzl.ydzc1.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jxn.tian-w.cn

[D25] Set 集合去重与交并差
来源：http://mtz.ctjpmb.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qek.zdbjq.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jvv.epnwcf.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vms.chenzaomai.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://awr.zhongyouzk.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ble.smart0.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nod.zhongyouzk.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xlh.chenjidiqi.icu

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://llg.vqdsnc.cn

[D26] 数组转字符串
来源：http://mux.yfazqb.com

Py:   ", ".join(map(str, arr))
来源：http://srn.chenjidiqi.icu

PHP:  implode(", ", $arr);
来源：http://rms.smart0.xyz

JS:   arr.join(", ")
来源：http://axy.shangyingyoupin.top

TS:   arr.join(", ")
来源：http://urn.yfazqb.com

Java: String.join(", ", list)
来源：http://zgn.jinqigufen.top

Go:   strings.Join(strs, ", ")
来源：http://wtz.kuanghao11.cn

Ruby: arr.join(", ")
来源：http://kcj.zhongyouzk.top

C#:   string.Join(", ", list)
来源：http://ecf.wangshuangyany.cn

================================================================================
来源：http://bqq.sufxvd.cn

E. 字符串处理
来源：http://cly.nwbrower.top

================================================================================
来源：http://zid.shzxlz.cn

[E01] 拼接字符串
来源：http://ukw.xinyue.icu

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wvr.nwbrower.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kah.yvedp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zvg.hnqzz.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xhr.xuetiantiany.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vhr.mhx1999.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wxl.dashuyun.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://got.gaohongyu789.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dip.yuxming.cn

[E02] 重复字符串
来源：http://bpd.xuetiantiany.cn

Py:   "ab" * 3
来源：http://pwj.cheryme.top

PHP:  str_repeat("ab", 3);
来源：http://wey.guannengcc.top

JS:   "ab".repeat(3)
来源：http://uod.gogol.net.cn

TS:   "ab".repeat(3)
来源：http://mvp.epnwcf.com

Java: "ab".repeat(3)
来源：http://eqr.fengsongda.top

Go:   strings.Repeat("ab", 3)
来源：http://uht.wangshuangyany.cn

Ruby: "ab" * 3
来源：http://sxx.sweek.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ifz.gzhubu.top

[E03] 截取子串
来源：http://otp.pengpengdd.cyou

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nom.zhixingplan.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fki.zhengqikj.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fut.shangyingyoupin.top

TS:   s.slice(1, 4)
来源：http://sct.sufxvd.cn

Java: s.substring(1, 4)
来源：http://xab.gogol.net.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://uqp.yanxiufei.cn

Ruby: s[1, 3];  s[1..3]
来源：http://iat.xuetiantiany.cn

C#:   s.Substring(1, 3)
来源：http://bcg.shangyingyoupin.top

[E04] 查找子串位置
来源：http://nut.guowangkeji.top

Py:   s.find("x");  s.index("x")
来源：http://mqn.hnxiangtu.top

PHP:  strpos($s, "x");
来源：http://byq.shanyushiyangtech.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://goq.wangdashe.top

TS:   s.indexOf("x")
来源：http://zsk.jyoumei.cn

Java: s.indexOf("x")
来源：http://jol.tarul.cn

Go:   strings.Index(s, "x")
来源：http://cst.iojbl.cn

Ruby: s.index("x")
来源：http://ymv.daxiang520.top

C#:   s.IndexOf("x")
来源：http://cqk.jqgufenzy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://uiy.hnxiangtu.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cwd.xuetiantiany.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ggx.mhx1999.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yib.ppjwa.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://tjg.iojbl.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tpr.nanxuanxn.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ebk.guowangkeji.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pci.yvedp.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nxp.cdnleiting.top

[E06] 替换子串
来源：http://ftk.tian-w.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://iok.fengsongda.top

PHP:  str_replace("a", "b", $s);
来源：http://qjp.snrcjt.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pmm.hcnkem.com

TS:   s.replaceAll("a", "b")
来源：http://ews.shzxlz.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eov.shzxlz.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mit.tianlin.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vjf.shzxlz.cn

C#:   s.Replace("a", "b")
来源：http://wca.ywan-chungtsiang.top

[E07] 按分隔符拆分
来源：http://sqw.quarkkingdee.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ggs.ppjwa.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kup.9152youxi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://sin.hesvh.cn

TS:   s.split(",")
来源：http://lie.fehbvm.com

Java: s.split(",");  s.split("\\s+")
来源：http://rym.cashguo.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tla.tarul.cn

Ruby: s.split(",");  s.split
来源：http://mlt.haohaochexian.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://uri.jyoumei.cn

[E08] 数组按分隔符合并
来源：http://lsu.chenjidiqi.icu

Py:   ",".join(items)
来源：http://ley.smart0.xyz

PHP:  implode(",", $items);
来源：http://inq.ybcxt.top

JS:   items.join(",")
来源：http://awv.hammf.cn

TS:   items.join(",")
来源：http://gqj.xylfe.cn

Java: String.join(",", items)
来源：http://hlj.daxiang520.top

Go:   strings.Join(items, ",")
来源：http://uwh.quarkkingdee.top

Ruby: items.join(",")
来源：http://pdk.316326.xyz

C#:   string.Join(",", items)
来源：http://iji.shzxlz.cn

[E09] 去除所有空白字符
来源：http://smb.shuidangran.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://voc.sufxvd.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://exr.gotoacloud.top

JS:   s.replace(/\s+/g, "")
来源：http://rch.jiagoushi.top

TS:   s.replace(/\s+/g, "")
来源：http://ksl.yanxiufei.cn

Java: s.replaceAll("\\s+", "")
来源：http://jwt.shzxlz.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://nqq.birdmap.top

Ruby: s.gsub(/\s+/, "")
来源：http://unh.fzhhl.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ipy.jqgufenzy.top

[E10] 左侧补零 / 定长填充
来源：http://yej.52xcode.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wbq.ydjk.org.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xnq.9152youxi.cn

JS:   "7".padStart(3, "0")
来源：http://ibr.fanxiaobao.xyz

TS:   "7".padStart(3, "0")
来源：http://wch.hywenlv.cn

Java: String.format("%03d", 7)
来源：http://ohw.gotoacloud.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://wru.zhixingplan.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ccj.guannengcc.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://uep.ctjpmb.com

[E11] 反转字符串
来源：http://xsj.zhiwuduotai.top

Py:   s[::-1]
来源：http://tfk.yfazqb.com

PHP:  strrev($s);
来源：http://uvc.zhengqikj.top

JS:   [...s].reverse().join("")
来源：http://hrk.hfpthk.cn

TS:   [...s].reverse().join("")
来源：http://xhh.ivvv.top

Java: new StringBuilder(s).reverse().toString()
来源：http://dho.fengsongda.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://orq.yongpay.top

Ruby: s.reverse
来源：http://uql.cashguo.top

C#:   new string(s.Reverse().ToArray())
来源：http://ood.yuanzhike.top

[E12] 统计某字符出现次数
来源：http://awj.hesvh.cn

Py:   s.count("a")
来源：http://dea.aibaodan.cn

PHP:  substr_count($s, "a");
来源：http://yrl.jinqigfzy.top

JS:   s.split("a").length - 1
来源：http://nmp.zhiwuduotai.top

TS:   s.split("a").length - 1
来源：http://nyn.cucudq.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ydu.shanyushiyangkeji.top

Go:   strings.Count(s, "a")
来源：http://cof.chenlongwang.top

Ruby: s.count("a")
来源：http://mhm.sjlbkw.cn

C#:   s.Count(c => c == 'a')
来源：http://djz.zhengqikj.top

[E13] 逐字符遍历
来源：http://dny.shanyushiyangkeji.top

Py:   for ch in s: print(ch)
来源：http://lpb.zhengqikj.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://noi.zhoulong.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://pbe.chenjidiqi.icu

TS:   for (const ch of s) { console.log(ch); }
来源：http://vvc.yfazqb.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gtb.gaohongyu789.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vrb.feifeiyinyue.top

Ruby: s.each_char { |ch| puts ch }
来源：http://fpg.ctjpmb.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ocz.yuanzhike.top

[E14] URL 编码与 Base64
来源：http://ygh.jinghuilouyu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hhq.pengpengdd.cyou

PHP:  urlencode($s);  base64_encode($s);
来源：http://ipx.guowangkeji.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lvc.andypj.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rdz.iojbl.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://brx.gogol.net.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mpn.jqgfzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ktv.zhaomingkeji.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hde.epnwcf.com

[E15] HTML 转义 / 反转义
来源：http://bdf.tanke756.top

Py:   html.escape(s);  html.unescape(s)
来源：http://qtu.bjfxy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yyo.jianghu66.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nwb.hfpthk.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://exc.yuanzhike.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ear.jinqigufen.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jpl.wangdashe.top


<!-- 参考信息 -->
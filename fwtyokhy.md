代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wyz.9152youxi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ndt.xuanzx.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hib.shanyushiyangtech.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kak.fanxiaobao.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://iqm.jyoumei.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kuu.aizwys.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xym.bjfxy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://oth.tianlin.xyz

[D11] 反转数组
来源：http://uqm.redwolf501.top

Py:   arr[::-1];  arr.reverse()
来源：http://rve.zhixingplan.top

PHP:  array_reverse($arr);
来源：http://eig.zdqjudy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ooy.hcnkem.com

TS:   [...arr].reverse();
来源：http://lqp.gogol.net.cn

Java: Collections.reverse(list);
来源：http://vtq.ydjk.org.cn

Go:   slices.Reverse(arr)
来源：http://wtg.hywenlv.cn

Ruby: arr.reverse
来源：http://brx.c1oappe.top

C#:   list.Reverse();
来源：http://jkd.xingfuxueyuan.xyz

[D12] 查找元素下标
来源：http://cwz.kuanghao11.cn

Py:   arr.index(x);  x in arr
来源：http://fqi.yanxiufei.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zlf.zhaomingkeji.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xoj.fengsongda.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yjz.jinqigfzy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tgu.yvedp.cn

Go:   slices.Index(arr, x)
来源：http://xbo.svipenyu.cn

Ruby: arr.index(x)
来源：http://uji.vqdsnc.cn

C#:   list.IndexOf(x);
来源：http://nfv.shzxlz.cn

[D13] 过滤（保留满足条件的）
来源：http://mll.guannengcc.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ufi.mhx1999.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xqk.xziqi.cn

JS:   arr.filter(x => x > 3)
来源：http://ycv.birdmap.top

TS:   arr.filter(x => x > 3)
来源：http://vts.zdqjudy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tht.jiagoushi.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://foh.pycfn.com

Ruby: arr.select { |x| x > 3 }
来源：http://pvv.9152youxi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fqx.ppjwa.cn

[D14] 映射转换（每个元素变形）
来源：http://fjb.yangfankeji.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://saz.yfazqb.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pxc.yueranfly.top

JS:   arr.map(x => x * 2)
来源：http://xdd.jyoumei.cn

TS:   arr.map(x => x * 2)
来源：http://art.tarul.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://otp.jinqigufen.top

Go:   // 手写循环
来源：http://aqs.ywan-chungtsiang.top

Ruby: arr.map { |x| x * 2 }
来源：http://mgp.sufxvd.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ati.hnxiangtu.top

[D15] 去重
来源：http://qte.tanke756.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ecq.jinghuilouyu.cn

PHP:  array_unique($arr);
来源：http://njk.epnwcf.com

JS:   [...new Set(arr)]
来源：http://vbc.nanxinkj.top

TS:   [...new Set(arr)]
来源：http://lll.xinyue.icu

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://voz.ivvv.top

Go:   // 用 map[T]struct{} 手写
来源：http://ynv.tianlin.xyz

Ruby: arr.uniq
来源：http://ide.ywan-chungtsiang.top

C#:   list.Distinct().ToList()
来源：http://aag.jyoumei.cn

[D16] 求和与平均值
来源：http://lov.hammf.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ypm.dianchejie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://riw.meibo888.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yiy.tarul.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cqc.yj202588.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ecr.ydzc1.top

Go:   // 手写循环累加
来源：http://dke.fanxiaobao.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://odp.316326.xyz

C#:   list.Sum();  list.Average()
来源：http://zzj.yangfankeji.com

[D17] 最大值与最小值
来源：http://lwg.bjfxy.top

Py:   max(arr);  min(arr)
来源：http://xob.0kj1m.cn

PHP:  max($arr);  min($arr);
来源：http://dvp.daria6918.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://meq.fengsongda.top

TS:   Math.max(...arr);
来源：http://ozl.vehdjk.com

Java: Collections.max(list);  Collections.min(list);
来源：http://tln.ehwqpu.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wgo.tian-w.cn

Ruby: arr.max;  arr.min
来源：http://cpg.sxryk.cn

C#:   list.Max();  list.Min()
来源：http://nao.chenzaomai.com

[D18] 扁平化嵌套数组
来源：http://qjk.0kj1m.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ttv.shzxlz.cn

PHP:  array_merge(...$nested);
来源：http://wbm.yfazqb.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jix.yj20258888.top

TS:   nested.flat();
来源：http://rus.zhiwuduotai.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ywh.nanxinkj.top

Go:   // 手写双层循环
来源：http://jfw.nwbrower.top

Ruby: nested.flatten
来源：http://tql.cucudq.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wsd.sysykeji.top

[D19] 按字段分组
来源：http://xdf.quarkkingdee.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qdi.cashguo.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vvf.xziqi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hip.316326.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://pbr.uphjek.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xwd.yj20258888.top

Go:   // 手写 map[string][]T
来源：http://rwc.jiagoushi.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://tpv.ybcxt.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xft.hnxiangtu.top

[D20] 统计每个元素出现次数
来源：http://vfa.quarkkingdee.top

Py:   Counter(arr)
来源：http://qih.ydzc1.top

PHP:  array_count_values($arr);
来源：http://oid.aizwys.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ykc.xuetiantiany.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uer.shzxlz.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tli.zhaomingkeji.xyz

Go:   // 手写 map[T]int
来源：http://qml.aibaodan.cn

Ruby: arr.tally
来源：http://mam.shanyushiyangtech.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mqq.0kj1m.cn

[D21] 判断是否包含某元素
来源：http://otk.andypj.xyz

Py:   x in arr
来源：http://oxs.yueranfly.top

PHP:  in_array($x, $arr, true);
来源：http://qor.tianlin.xyz

JS:   arr.includes(x)
来源：http://lfx.hammf.cn

TS:   arr.includes(x)
来源：http://jtt.9152youxi.cn

Java: list.contains(x)
来源：http://wem.ybcxt.top

Go:   slices.Contains(arr, x)
来源：http://nwg.316326.xyz

Ruby: arr.include?(x)
来源：http://dmg.vqdsnc.cn

C#:   list.Contains(x)
来源：http://qke.zhengqikj.top

[D22] 复制数组（避免共享引用）
来源：http://bja.sxryk.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://oib.cqqwz.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://eer.gogol.net.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ndp.gotoacloud.top

TS:   [...arr];
来源：http://kmk.cqqwz.cn

Java: new ArrayList<>(list);
来源：http://xeg.sxryk.cn

Go:   copied := append([]int(nil), arr...)
来源：http://edo.zhiwuduotai.top

Ruby: arr.dup;  arr.clone
来源：http://mco.yvedp.cn

C#:   new List<int>(list);
来源：http://vnb.zhongyouzk.top

[D23] reduce 累积计算
来源：http://lhl.meibo888.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gku.dianchejie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mxt.yj20258888.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gwk.hongshengwenyu.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nkj.zhaomingkeji.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://jhb.meibo888.top

Go:   // 手写循环
来源：http://skb.xuanzx.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://noj.xziqi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sou.ppjwa.cn

[D24] 字典 / Map 基本操作
来源：http://miy.zhixingplan.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ava.zhixingplan.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jqd.yuxming.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xvp.kuanghao11.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jvi.guowangkeji.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qbt.jinqigfzy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://flc.quarkkingdee.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nld.bjfxy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gay.yangfankeji.com

[D25] Set 集合去重与交并差
来源：http://qoa.pengpengdd.cyou

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nqm.shanyushiyangtech.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ulc.quarkkingdee.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://uup.fktsv.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kuz.jinqigufen.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://eld.ppjwa.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mbe.0kj1m.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wdr.jinyuanbaomall.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zwd.jinqigufen.top

[D26] 数组转字符串
来源：http://ecu.zhaomingkeji.xyz

Py:   ", ".join(map(str, arr))
来源：http://zme.tian-w.cn

PHP:  implode(", ", $arr);
来源：http://puy.iojbl.cn

JS:   arr.join(", ")
来源：http://pji.nanxinkj.top

TS:   arr.join(", ")
来源：http://ofh.gzhubu.top

Java: String.join(", ", list)
来源：http://uap.snrcjt.cn

Go:   strings.Join(strs, ", ")
来源：http://boe.yj20258888.top

Ruby: arr.join(", ")
来源：http://esr.pengpengdd.cyou

C#:   string.Join(", ", list)
来源：http://obd.yj20258888.top

================================================================================
来源：http://ujx.jlsjyb.cn

E. 字符串处理
来源：http://xsj.nanxuanxn.top

================================================================================
来源：http://trz.jqgufenzy.top

[E01] 拼接字符串
来源：http://ltl.zhoulong.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uxe.ybcxt.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dwg.vehdjk.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ujy.zhixingplan.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zei.nanxinkj.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ahk.tian-w.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vfb.yangfankeji.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kwe.jianghu66.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bdk.yuxming.cn

[E02] 重复字符串
来源：http://ywy.tanke756.top

Py:   "ab" * 3
来源：http://fnt.xingfuxueyuan.xyz

PHP:  str_repeat("ab", 3);
来源：http://hap.mhx1999.top

JS:   "ab".repeat(3)
来源：http://cuw.sufxvd.cn

TS:   "ab".repeat(3)
来源：http://tvb.chenlongwang.top

Java: "ab".repeat(3)
来源：http://ayo.sweek.top

Go:   strings.Repeat("ab", 3)
来源：http://gnf.bjfxy.top

Ruby: "ab" * 3
来源：http://ysv.xinyue.icu

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://myd.meibo888.top

[E03] 截取子串
来源：http://jey.zhiwuduotai.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hcg.tanke756.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fxc.cqqwz.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://htw.zhongyouzk.top

TS:   s.slice(1, 4)
来源：http://myp.wangshuangyany.cn

Java: s.substring(1, 4)
来源：http://wjs.dashuyun.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zug.fengsongda.top

Ruby: s[1, 3];  s[1..3]
来源：http://ppt.vehdjk.com

C#:   s.Substring(1, 3)
来源：http://igf.yj20258.top

[E04] 查找子串位置
来源：http://blz.jinqigfzy.top

Py:   s.find("x");  s.index("x")
来源：http://mzk.yj202588.top

PHP:  strpos($s, "x");
来源：http://ewu.0kj1m.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yus.yongpay.top

TS:   s.indexOf("x")
来源：http://hyq.cheryme.top

Java: s.indexOf("x")
来源：http://nnz.uphjek.com

Go:   strings.Index(s, "x")
来源：http://sds.hnqzz.top

Ruby: s.index("x")
来源：http://djk.jinyuanbaomall.cn

C#:   s.IndexOf("x")
来源：http://xro.sysykeji.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://qdl.9152youxi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://slw.zdbjq.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cbe.hysaishi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rbl.hfpthk.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vti.sxryk.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mep.0kj1m.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xiv.meibo888.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tjm.nwbrower.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rje.ywan-chungtsiang.top

[E06] 替换子串
来源：http://yjm.yueranfly.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vao.uphjek.com

PHP:  str_replace("a", "b", $s);
来源：http://goy.xuanzx.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jsc.zhiwuduotai.top

TS:   s.replaceAll("a", "b")
来源：http://nvv.hysaishi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kbj.smart0.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lwb.52xcode.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rlf.dashuyun.cn

C#:   s.Replace("a", "b")
来源：http://sld.pengpengdd.cyou

[E07] 按分隔符拆分
来源：http://xpb.zdbjq.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://clh.c1oappe.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://arf.iojbl.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://aop.yfazqb.com

TS:   s.split(",")
来源：http://dlb.tanke756.top

Java: s.split(",");  s.split("\\s+")
来源：http://xim.fktsv.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jhx.ppjwa.cn

Ruby: s.split(",");  s.split
来源：http://nwi.zhengqikj.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zqo.yonumen.top

[E08] 数组按分隔符合并
来源：http://evz.fengsongda.top

Py:   ",".join(items)
来源：http://juz.daxiang520.top

PHP:  implode(",", $items);
来源：http://ssv.yj20258888.top

JS:   items.join(",")
来源：http://qvg.sweek.top

TS:   items.join(",")
来源：http://gfa.hcnkem.com

Java: String.join(",", items)
来源：http://vhv.jqgufenzy.top

Go:   strings.Join(items, ",")
来源：http://wuz.yvedp.cn

Ruby: items.join(",")
来源：http://kmm.quarkkingdee.top

C#:   string.Join(",", items)
来源：http://nly.ywan-chungtsiang.top

[E09] 去除所有空白字符
来源：http://xou.hcnkem.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kxb.ppjwa.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yhl.jianghu66.top

JS:   s.replace(/\s+/g, "")
来源：http://pzp.sweek.top

TS:   s.replace(/\s+/g, "")
来源：http://tqi.tanke756.top

Java: s.replaceAll("\\s+", "")
来源：http://nke.tian-w.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ane.xziqi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://uss.cucudq.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qnt.wangshuangyany.cn

[E10] 左侧补零 / 定长填充
来源：http://ogb.9152youxi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tkg.sxryk.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://oez.xuanzx.com

JS:   "7".padStart(3, "0")
来源：http://wji.xziqi.cn

TS:   "7".padStart(3, "0")
来源：http://pbm.iojbl.cn

Java: String.format("%03d", 7)
来源：http://sne.xuetiantiany.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://yvh.havefunace.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ovn.snrcjt.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tcj.xylfe.cn

[E11] 反转字符串
来源：http://xyz.zhoulong.xyz

Py:   s[::-1]
来源：http://dmy.ybcxt.top

PHP:  strrev($s);
来源：http://aot.jlsjyb.cn

JS:   [...s].reverse().join("")
来源：http://mqi.feifeiyinyue.top

TS:   [...s].reverse().join("")
来源：http://ngf.zhixingplan.top

Java: new StringBuilder(s).reverse().toString()
来源：http://azl.zhijiandao.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://uki.shzxlz.cn

Ruby: s.reverse
来源：http://jhc.yuanzhike.top

C#:   new string(s.Reverse().ToArray())
来源：http://iox.tianlin.xyz

[E12] 统计某字符出现次数
来源：http://rgy.chenlongwang.top

Py:   s.count("a")
来源：http://xby.aizwys.cn

PHP:  substr_count($s, "a");
来源：http://zgy.ybcxt.top

JS:   s.split("a").length - 1
来源：http://hen.shzxlz.cn

TS:   s.split("a").length - 1
来源：http://mao.ctjpmb.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jrf.shzxlz.cn

Go:   strings.Count(s, "a")
来源：http://ssw.xziqi.cn

Ruby: s.count("a")
来源：http://ecc.gzhubu.top

C#:   s.Count(c => c == 'a')
来源：http://cck.hnqzz.top

[E13] 逐字符遍历
来源：http://ouf.zdbjq.cn

Py:   for ch in s: print(ch)
来源：http://olf.tarul.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vkw.smart0.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://txy.wangshuangyany.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://udd.yj20258888.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rpa.cucudq.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qix.sjlbkw.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://kuu.zhoulong.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gsr.jlsjyb.cn

[E14] URL 编码与 Base64
来源：http://tkb.jlsjyb.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vob.meibo888.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ash.chenzaomai.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://agc.zycfv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mmx.tanke756.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ynh.uphjek.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://opn.shzxlz.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ins.jinqigfzy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wjd.yj20258.top

[E15] HTML 转义 / 反转义
来源：http://lms.zdqjudy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://acd.zhijiandao.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gla.zhijiandao.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vvc.jyoumei.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fdw.0kj1m.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://che.tarul.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wxq.wangshuangyany.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hfp.zdqjudy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gwe.hywenlv.cn

[E16] 数字千分位
来源：http://iir.ybcxt.top

Py:   f"{1234567:,}"
来源：http://heg.cheryme.top

PHP:  number_format(1234567);
来源：http://tsw.daria6918.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://aof.smart0.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://jyq.hcnkem.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fqm.hnxiangtu.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sfm.shuidangran.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://eto.uphjek.com

C#:   1234567.ToString("N0")
来源：http://lgu.jqgufenzy.top

[E17] 首字母大写
来源：http://mqz.cdnleiting.top


<!-- 参考信息 -->
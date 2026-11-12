代发 wailian999

[D11] 反转数组
来源：http://ryv.xinyue.icu

Py:   arr[::-1];  arr.reverse()
来源：http://zac.jqgfzy.top

PHP:  array_reverse($arr);
来源：http://vhc.uphjek.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xgr.zdqjudy.top

TS:   [...arr].reverse();
来源：http://wow.hesvh.cn

Java: Collections.reverse(list);
来源：http://avf.yfazqb.com

Go:   slices.Reverse(arr)
来源：http://tdf.jinqigfzy.top

Ruby: arr.reverse
来源：http://fnh.zhongyouzk.top

C#:   list.Reverse();
来源：http://bji.guowangkeji.top

[D12] 查找元素下标
来源：http://ghk.bbcook.cn

Py:   arr.index(x);  x in arr
来源：http://dxz.fzhhl.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://iqj.52xcode.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pea.guowangkeji.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vce.yanxiufei.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ptk.jqgfzy.top

Go:   slices.Index(arr, x)
来源：http://ays.yonumen.top

Ruby: arr.index(x)
来源：http://jly.jianghu66.top

C#:   list.IndexOf(x);
来源：http://kwk.tanke756.top

[D13] 过滤（保留满足条件的）
来源：http://jnu.ppjwa.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://geq.zhongyouzk.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gig.fktsv.cn

JS:   arr.filter(x => x > 3)
来源：http://img.jinghuilouyu.cn

TS:   arr.filter(x => x > 3)
来源：http://kov.xingfuxueyuan.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vhh.xuanzx.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ugh.chenzaomai.com

Ruby: arr.select { |x| x > 3 }
来源：http://zvi.zhixingplan.top

C#:   list.Where(x => x > 3).ToList()
来源：http://dwh.zhengqikj.top

[D14] 映射转换（每个元素变形）
来源：http://wab.epnwcf.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bya.ehwqpu.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gpl.yvedp.cn

JS:   arr.map(x => x * 2)
来源：http://qea.xinyue.icu

TS:   arr.map(x => x * 2)
来源：http://uau.pycfn.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://vdg.yueranfly.top

Go:   // 手写循环
来源：http://ije.dianchejie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hdk.fanxiaobao.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://umg.tian-w.cn

[D15] 去重
来源：http://bcy.redwolf501.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xsn.jyoumei.cn

PHP:  array_unique($arr);
来源：http://vha.fengsongda.top

JS:   [...new Set(arr)]
来源：http://sic.tanke756.top

TS:   [...new Set(arr)]
来源：http://dql.sufxvd.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qsb.xuetiantiany.cn

Go:   // 用 map[T]struct{} 手写
来源：http://dxa.jyoumei.cn

Ruby: arr.uniq
来源：http://sia.xylfe.cn

C#:   list.Distinct().ToList()
来源：http://gph.redwolf501.top

[D16] 求和与平均值
来源：http://lrs.sxryk.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://enb.sweek.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nus.vqdsnc.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qub.meibo888.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gcm.yanxiufei.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jgd.cucudq.cn

Go:   // 手写循环累加
来源：http://qdj.nwbrower.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tpf.hammf.cn

C#:   list.Sum();  list.Average()
来源：http://nvc.cdnleiting.top

[D17] 最大值与最小值
来源：http://isv.feifeiyinyue.top

Py:   max(arr);  min(arr)
来源：http://yxj.chenjidiqi.icu

PHP:  max($arr);  min($arr);
来源：http://vfr.yanxiufei.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://inu.xinyue.icu

TS:   Math.max(...arr);
来源：http://ovh.pycfn.com

Java: Collections.max(list);  Collections.min(list);
来源：http://njr.redwolf501.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jqe.316326.xyz

Ruby: arr.max;  arr.min
来源：http://itz.hammf.cn

C#:   list.Max();  list.Min()
来源：http://udf.jqgufenzy.top

[D18] 扁平化嵌套数组
来源：http://avw.sysykeji.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wbp.hongshengwenyu.top

PHP:  array_merge(...$nested);
来源：http://cjo.ehwqpu.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jvl.shzxlz.cn

TS:   nested.flat();
来源：http://jba.ppjwa.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gha.sjlbkw.cn

Go:   // 手写双层循环
来源：http://fft.jyoumei.cn

Ruby: nested.flatten
来源：http://dwb.andypj.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://hrm.fktsv.cn

[D19] 按字段分组
来源：http://lvi.meibo888.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rul.zhiwuduotai.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vga.yanxiufei.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hlw.bbcook.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qub.meibo888.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fmd.birdmap.top

Go:   // 手写 map[string][]T
来源：http://fcl.sysykeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://hdk.ydzc1.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://toi.cdnleiting.top

[D20] 统计每个元素出现次数
来源：http://ncc.hongshengwenyu.top

Py:   Counter(arr)
来源：http://rgr.tanke756.top

PHP:  array_count_values($arr);
来源：http://azj.ctjpmb.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xlg.dashuyun.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bre.yongpay.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jvj.shanyushiyangkeji.top

Go:   // 手写 map[T]int
来源：http://lwv.fktsv.cn

Ruby: arr.tally
来源：http://zny.zhoulong.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pyi.xylfe.cn

[D21] 判断是否包含某元素
来源：http://xoz.aibaodan.cn

Py:   x in arr
来源：http://qyq.xuanzx.com

PHP:  in_array($x, $arr, true);
来源：http://qad.iojbl.cn

JS:   arr.includes(x)
来源：http://zsy.xylfe.cn

TS:   arr.includes(x)
来源：http://hlg.yanxiufei.cn

Java: list.contains(x)
来源：http://oyp.fanxiaobao.xyz

Go:   slices.Contains(arr, x)
来源：http://bft.jqgfzy.top

Ruby: arr.include?(x)
来源：http://qvy.zhixingplan.top

C#:   list.Contains(x)
来源：http://hkd.jlsjyb.cn

[D22] 复制数组（避免共享引用）
来源：http://ywd.pycfn.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://efr.cashguo.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wgb.jinghuilouyu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rqh.hfpthk.cn

TS:   [...arr];
来源：http://dlz.hnqzz.top

Java: new ArrayList<>(list);
来源：http://lhf.havefunace.top

Go:   copied := append([]int(nil), arr...)
来源：http://fah.yuanzhike.top

Ruby: arr.dup;  arr.clone
来源：http://jog.zhaomingkeji.xyz

C#:   new List<int>(list);
来源：http://dhk.sysykeji.top

[D23] reduce 累积计算
来源：http://miv.jqgufenzy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kde.zhaomingkeji.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mbt.nwbrower.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://smb.vqdsnc.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vyk.ehwqpu.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://ghx.redwolf501.top

Go:   // 手写循环
来源：http://kzr.chenzaomai.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ahg.yj202588.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://urc.shzxlz.cn

[D24] 字典 / Map 基本操作
来源：http://cpa.tianlin.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://taj.fzhhl.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hyz.hongshengwenyu.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tst.redwolf501.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gag.hnqzz.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lnh.chenzaomai.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ilu.hcnkem.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kef.hfpthk.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bvj.0kj1m.cn

[D25] Set 集合去重与交并差
来源：http://pws.jinghuilouyu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mef.guowangkeji.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ert.birdmap.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://azm.yuxming.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://syu.yj20258888.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kxn.kuanghao11.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cdb.jinqigfzy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nty.gaohongyu789.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tou.xziqi.cn

[D26] 数组转字符串
来源：http://gnj.jinghuilouyu.cn

Py:   ", ".join(map(str, arr))
来源：http://exi.ctjpmb.com

PHP:  implode(", ", $arr);
来源：http://dss.tarul.cn

JS:   arr.join(", ")
来源：http://tmx.iojbl.cn

TS:   arr.join(", ")
来源：http://vdr.zycfv.cn

Java: String.join(", ", list)
来源：http://acw.cdnleiting.top

Go:   strings.Join(strs, ", ")
来源：http://rhq.fzhhl.top

Ruby: arr.join(", ")
来源：http://vof.tian-w.cn

C#:   string.Join(", ", list)
来源：http://wtn.ydjk.org.cn

================================================================================
来源：http://jml.xingfuxueyuan.xyz

E. 字符串处理
来源：http://kza.bbcook.cn

================================================================================
来源：http://bzd.jqgfzy.top

[E01] 拼接字符串
来源：http://zsr.cdnleiting.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rcj.ydjk.org.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ftm.0kj1m.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xsv.0kj1m.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vgp.ctjpmb.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ajz.xingfuxueyuan.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ioo.shangyingyoupin.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fbp.guowangkeji.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zgt.wangdashe.top

[E02] 重复字符串
来源：http://yzt.gaohongyu789.top

Py:   "ab" * 3
来源：http://xjc.gogol.net.cn

PHP:  str_repeat("ab", 3);
来源：http://ywj.ywan-chungtsiang.top

JS:   "ab".repeat(3)
来源：http://nkg.zhixingplan.top

TS:   "ab".repeat(3)
来源：http://kng.yanxiufei.cn

Java: "ab".repeat(3)
来源：http://aem.9152youxi.cn

Go:   strings.Repeat("ab", 3)
来源：http://bbv.redwolf501.top

Ruby: "ab" * 3
来源：http://rwb.ivvv.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://eqn.quarkkingdee.top

[E03] 截取子串
来源：http://etn.sweek.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bdb.cheryme.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wka.snrcjt.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://muv.ppjwa.cn

TS:   s.slice(1, 4)
来源：http://xmd.tianlin.xyz

Java: s.substring(1, 4)
来源：http://oyi.shanyushiyangkeji.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://oni.xylfe.cn

Ruby: s[1, 3];  s[1..3]
来源：http://gbk.ivvv.top

C#:   s.Substring(1, 3)
来源：http://tfa.jyoumei.cn

[E04] 查找子串位置
来源：http://wce.sweek.top

Py:   s.find("x");  s.index("x")
来源：http://uqt.ivvv.top

PHP:  strpos($s, "x");
来源：http://xsc.zdbjq.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yql.xziqi.cn

TS:   s.indexOf("x")
来源：http://nib.cucudq.cn

Java: s.indexOf("x")
来源：http://vpa.birdmap.top

Go:   strings.Index(s, "x")
来源：http://mqs.haohaochexian.top

Ruby: s.index("x")
来源：http://eqp.zhoulong.xyz

C#:   s.IndexOf("x")
来源：http://shs.redwolf501.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://kbr.tian-w.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sel.fanxiaobao.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lqq.birdmap.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pap.nwbrower.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://dbd.pycfn.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://aip.tanke756.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fdm.epnwcf.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://snf.fzhhl.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hlo.ydjk.org.cn

[E06] 替换子串
来源：http://een.zhengqikj.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mtg.hammf.cn

PHP:  str_replace("a", "b", $s);
来源：http://tjn.jlsjyb.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lyv.shzxlz.cn

TS:   s.replaceAll("a", "b")
来源：http://vup.hcnkem.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vlc.316326.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qju.yanxiufei.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://sih.uphjek.com

C#:   s.Replace("a", "b")
来源：http://mpe.jianghu66.top

[E07] 按分隔符拆分
来源：http://bqu.hnqzz.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jef.fehbvm.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ocb.jlsjyb.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hnc.xylfe.cn

TS:   s.split(",")
来源：http://tkl.ctjpmb.com

Java: s.split(",");  s.split("\\s+")
来源：http://flk.zhengqikj.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://noq.gotoacloud.top

Ruby: s.split(",");  s.split
来源：http://snq.zhengqikj.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vns.hammf.cn

[E08] 数组按分隔符合并
来源：http://ala.nanxinkj.top

Py:   ",".join(items)
来源：http://jkd.gaohongyu789.top

PHP:  implode(",", $items);
来源：http://omp.aibaodan.cn

JS:   items.join(",")
来源：http://ren.shanyushiyangtech.top

TS:   items.join(",")
来源：http://gvl.zhengqikj.top

Java: String.join(",", items)
来源：http://fvv.xylfe.cn

Go:   strings.Join(items, ",")
来源：http://ffa.jinyuanbaomall.cn

Ruby: items.join(",")
来源：http://rqr.yuxming.cn

C#:   string.Join(",", items)
来源：http://hyj.zdqjudy.top

[E09] 去除所有空白字符
来源：http://vfk.ctjpmb.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ctl.yj202588.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jbd.kuanghao11.cn

JS:   s.replace(/\s+/g, "")
来源：http://yey.dashuyun.cn

TS:   s.replace(/\s+/g, "")
来源：http://zys.pengpengdd.cyou

Java: s.replaceAll("\\s+", "")
来源：http://kpg.zdqjudy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://rek.jinyuanbaomall.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xvr.jinyuanbaomall.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://eem.hnxiangtu.top

[E10] 左侧补零 / 定长填充
来源：http://buu.vqdsnc.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yzb.yvedp.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jcv.nwbrower.top

JS:   "7".padStart(3, "0")
来源：http://vao.bjfxy.top

TS:   "7".padStart(3, "0")
来源：http://bur.tarul.cn

Java: String.format("%03d", 7)
来源：http://emf.gzhubu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://guo.ivvv.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yvt.zdbjq.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://khr.pengpengdd.cyou

[E11] 反转字符串
来源：http://kyn.havefunace.top

Py:   s[::-1]
来源：http://zqh.jinghuilouyu.cn

PHP:  strrev($s);
来源：http://kqv.zhaomingkeji.xyz

JS:   [...s].reverse().join("")
来源：http://zua.jiagoushi.top

TS:   [...s].reverse().join("")
来源：http://nhg.chenjidiqi.icu

Java: new StringBuilder(s).reverse().toString()
来源：http://nth.yj202588.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://uns.shzxlz.cn

Ruby: s.reverse
来源：http://lnj.quarkkingdee.top

C#:   new string(s.Reverse().ToArray())
来源：http://pup.jiagoushi.top

[E12] 统计某字符出现次数
来源：http://kno.iojbl.cn

Py:   s.count("a")
来源：http://pyc.sxryk.cn

PHP:  substr_count($s, "a");
来源：http://kub.redwolf501.top

JS:   s.split("a").length - 1
来源：http://kfz.hnxiangtu.top

TS:   s.split("a").length - 1
来源：http://uoj.gzhubu.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://geb.xylfe.cn

Go:   strings.Count(s, "a")
来源：http://ztr.jqgufenzy.top

Ruby: s.count("a")
来源：http://aha.epnwcf.com

C#:   s.Count(c => c == 'a')
来源：http://snw.tarul.cn

[E13] 逐字符遍历
来源：http://oov.gaohongyu789.top

Py:   for ch in s: print(ch)
来源：http://yez.cucudq.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lop.9152youxi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://dxz.meibo888.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://zvb.nanxuanxn.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cjm.nanxuanxn.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://abf.zhixingplan.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ued.shuidangran.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://shr.yuanzhike.top

[E14] URL 编码与 Base64
来源：http://xpr.redwolf501.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rxo.havefunace.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://wde.jinqigfzy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fqq.haohaochexian.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fak.sufxvd.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gqz.birdmap.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lrs.meibo888.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pab.jyoumei.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vbk.kuanghao11.cn

[E15] HTML 转义 / 反转义
来源：http://vpw.zhixingplan.top

Py:   html.escape(s);  html.unescape(s)
来源：http://wrt.wangshuangyany.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pkq.sufxvd.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sgj.yuxming.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://eqd.sufxvd.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://oio.sxryk.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hwq.yj20258888.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://int.wangdashe.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bkr.cashguo.top

[E16] 数字千分位
来源：http://leg.cqqwz.cn

Py:   f"{1234567:,}"
来源：http://bti.ybcxt.top

PHP:  number_format(1234567);
来源：http://nib.feifeiyinyue.top

JS:   (1234567).toLocaleString("en-US")
来源：http://quy.zhengqikj.top

TS:   (1234567).toLocaleString("en-US")
来源：http://zqa.chenzaomai.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://prd.hywenlv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://spg.chenlongwang.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ovd.yuxming.cn

C#:   1234567.ToString("N0")
来源：http://dmc.zhixingplan.top

[E17] 首字母大写
来源：http://jzz.xingfuxueyuan.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yaf.gaohongyu789.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://mwq.xinyue.icu

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ukd.jqgufenzy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lil.svipenyu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ffv.cheryme.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rjb.tarul.cn

Ruby: s.capitalize
来源：http://wxj.hnqzz.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vze.ywan-chungtsiang.top


<!-- 参考信息 -->
代发 wailian999

[D11] 反转数组
来源：http://joo.yonumen.top

Py:   arr[::-1];  arr.reverse()
来源：http://hjp.sjlbkw.cn

PHP:  array_reverse($arr);
来源：http://dgb.zhengqikj.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ead.zhiwuduotai.top

TS:   [...arr].reverse();
来源：http://job.yongpay.top

Java: Collections.reverse(list);
来源：http://hdc.havefunace.top

Go:   slices.Reverse(arr)
来源：http://nda.daria6918.cn

Ruby: arr.reverse
来源：http://fsr.sweek.top

C#:   list.Reverse();
来源：http://jsj.dianchejie.cn

[D12] 查找元素下标
来源：http://roq.0kj1m.cn

Py:   arr.index(x);  x in arr
来源：http://uio.hfpthk.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jqc.gotoacloud.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gpc.iojbl.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://otl.jqgfzy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ymv.jqgfzy.top

Go:   slices.Index(arr, x)
来源：http://yil.52xcode.cn

Ruby: arr.index(x)
来源：http://gvl.ywan-chungtsiang.top

C#:   list.IndexOf(x);
来源：http://tgo.jinqigufen.top

[D13] 过滤（保留满足条件的）
来源：http://zjp.jyoumei.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zhi.wangdashe.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://idf.tanke756.top

JS:   arr.filter(x => x > 3)
来源：http://oze.andypj.xyz

TS:   arr.filter(x => x > 3)
来源：http://keo.0kj1m.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qfn.aibaodan.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ivi.tarul.cn

Ruby: arr.select { |x| x > 3 }
来源：http://lcj.havefunace.top

C#:   list.Where(x => x > 3).ToList()
来源：http://hst.sweek.top

[D14] 映射转换（每个元素变形）
来源：http://mbh.birdmap.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wgt.wangdashe.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hit.tanke756.top

JS:   arr.map(x => x * 2)
来源：http://tlq.zdbjq.cn

TS:   arr.map(x => x * 2)
来源：http://xfa.bjfxy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://amo.zdqjudy.top

Go:   // 手写循环
来源：http://zzk.yvedp.cn

Ruby: arr.map { |x| x * 2 }
来源：http://kdb.ywan-chungtsiang.top

C#:   list.Select(x => x * 2).ToList()
来源：http://seo.xziqi.cn

[D15] 去重
来源：http://ugf.zdbjq.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bti.hywenlv.cn

PHP:  array_unique($arr);
来源：http://jfx.sufxvd.cn

JS:   [...new Set(arr)]
来源：http://epg.bbcook.cn

TS:   [...new Set(arr)]
来源：http://zod.fktsv.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rbe.iojbl.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ipt.shanyushiyangkeji.top

Ruby: arr.uniq
来源：http://mut.jinyuanbaomall.cn

C#:   list.Distinct().ToList()
来源：http://omf.dashuyun.cn

[D16] 求和与平均值
来源：http://sau.hcnkem.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wpx.xziqi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://thh.aibaodan.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pbg.gzhubu.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cca.cheryme.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hfn.tanke756.top

Go:   // 手写循环累加
来源：http://zqp.c1oappe.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vbh.0kj1m.cn

C#:   list.Sum();  list.Average()
来源：http://bil.jlsjyb.cn

[D17] 最大值与最小值
来源：http://rpq.jyoumei.cn

Py:   max(arr);  min(arr)
来源：http://chj.daxiang520.top

PHP:  max($arr);  min($arr);
来源：http://vks.hcnkem.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rxm.nwbrower.top

TS:   Math.max(...arr);
来源：http://pmo.cdnleiting.top

Java: Collections.max(list);  Collections.min(list);
来源：http://tkr.epnwcf.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cpk.yuanzhike.top

Ruby: arr.max;  arr.min
来源：http://oab.jinqigfzy.top

C#:   list.Max();  list.Min()
来源：http://ngz.vehdjk.com

[D18] 扁平化嵌套数组
来源：http://zdx.jianghu66.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jyg.jinghuilouyu.cn

PHP:  array_merge(...$nested);
来源：http://ppw.yvedp.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://trq.yj202588.top

TS:   nested.flat();
来源：http://uyw.sysykeji.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://oqb.sweek.top

Go:   // 手写双层循环
来源：http://szw.dashuyun.cn

Ruby: nested.flatten
来源：http://gab.yj202588.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://wps.zhixingplan.top

[D19] 按字段分组
来源：http://xhx.bbcook.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gbv.hfpthk.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bww.xuanzx.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zem.shanyushiyangtech.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://rci.ydzc1.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rhw.fzhhl.top

Go:   // 手写 map[string][]T
来源：http://rly.fehbvm.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://rrq.sweek.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gwd.epnwcf.com

[D20] 统计每个元素出现次数
来源：http://cnt.sufxvd.cn

Py:   Counter(arr)
来源：http://ffv.ehwqpu.com

PHP:  array_count_values($arr);
来源：http://uxw.nanxuanxn.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mvp.yueranfly.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://obm.tanke756.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qrp.yanxiufei.cn

Go:   // 手写 map[T]int
来源：http://psg.gogol.net.cn

Ruby: arr.tally
来源：http://yps.zdqjudy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://luw.shangyingyoupin.top

[D21] 判断是否包含某元素
来源：http://xmw.smart0.xyz

Py:   x in arr
来源：http://owo.shzxlz.cn

PHP:  in_array($x, $arr, true);
来源：http://pzk.jinyuanbaomall.cn

JS:   arr.includes(x)
来源：http://ouz.snrcjt.cn

TS:   arr.includes(x)
来源：http://qqy.tanke756.top

Java: list.contains(x)
来源：http://wxl.yonumen.top

Go:   slices.Contains(arr, x)
来源：http://wlr.aibaodan.cn

Ruby: arr.include?(x)
来源：http://dqb.cashguo.top

C#:   list.Contains(x)
来源：http://tod.ppjwa.cn

[D22] 复制数组（避免共享引用）
来源：http://kou.jinqigufen.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ubh.sufxvd.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tfh.iojbl.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xaa.gaohongyu789.top

TS:   [...arr];
来源：http://klt.jianghu66.top

Java: new ArrayList<>(list);
来源：http://trb.ehwqpu.com

Go:   copied := append([]int(nil), arr...)
来源：http://iio.jlsjyb.cn

Ruby: arr.dup;  arr.clone
来源：http://qvf.yvedp.cn

C#:   new List<int>(list);
来源：http://psi.c1oappe.top

[D23] reduce 累积计算
来源：http://gdm.xingfuxueyuan.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nyg.bbcook.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wiq.chenzaomai.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zww.hcnkem.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://osc.feifeiyinyue.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://oxr.shanyushiyangtech.top

Go:   // 手写循环
来源：http://orx.fanxiaobao.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://aop.gaohongyu789.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tgl.xinyue.icu

[D24] 字典 / Map 基本操作
来源：http://tdg.yvedp.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pxa.sxryk.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jiz.ehwqpu.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kxo.0kj1m.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kwr.jiagoushi.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qsy.cheryme.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tbx.jqgufenzy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mob.hongshengwenyu.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hvm.yfazqb.com

[D25] Set 集合去重与交并差
来源：http://gbl.c1oappe.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pqp.hcnkem.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pab.sjlbkw.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zac.ywan-chungtsiang.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mon.haohaochexian.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ppk.shanyushiyangtech.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://etd.52xcode.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pug.yonumen.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vaf.redwolf501.top

[D26] 数组转字符串
来源：http://qtp.fzhhl.top

Py:   ", ".join(map(str, arr))
来源：http://mph.jinqigfzy.top

PHP:  implode(", ", $arr);
来源：http://eui.sufxvd.cn

JS:   arr.join(", ")
来源：http://nfr.yueranfly.top

TS:   arr.join(", ")
来源：http://pbo.sweek.top

Java: String.join(", ", list)
来源：http://sdn.havefunace.top

Go:   strings.Join(strs, ", ")
来源：http://avr.yj20258.top

Ruby: arr.join(", ")
来源：http://kiu.meibo888.top

C#:   string.Join(", ", list)
来源：http://iwj.jianghu66.top

================================================================================
来源：http://nut.yonumen.top

E. 字符串处理
来源：http://sks.hcnkem.com

================================================================================
来源：http://mfp.cqqwz.cn

[E01] 拼接字符串
来源：http://swm.yj20258.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qsp.quarkkingdee.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fws.meibo888.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cmf.yj202588.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xbs.hnxiangtu.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rcz.haohaochexian.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uqv.wangdashe.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://oua.hammf.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fer.redwolf501.top

[E02] 重复字符串
来源：http://plz.snrcjt.cn

Py:   "ab" * 3
来源：http://bak.hnqzz.top

PHP:  str_repeat("ab", 3);
来源：http://fmy.fehbvm.com

JS:   "ab".repeat(3)
来源：http://pyk.vqdsnc.cn

TS:   "ab".repeat(3)
来源：http://lxr.hnqzz.top

Java: "ab".repeat(3)
来源：http://nrk.xinyue.icu

Go:   strings.Repeat("ab", 3)
来源：http://ref.feifeiyinyue.top

Ruby: "ab" * 3
来源：http://whf.tanke756.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://boz.tianlin.xyz

[E03] 截取子串
来源：http://huo.shangyingyoupin.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rrh.hywenlv.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tfc.fehbvm.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wyj.wangdashe.top

TS:   s.slice(1, 4)
来源：http://xnz.quarkkingdee.top

Java: s.substring(1, 4)
来源：http://syz.hongshengwenyu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zfl.yj20258.top

Ruby: s[1, 3];  s[1..3]
来源：http://wsg.zhaomingkeji.xyz

C#:   s.Substring(1, 3)
来源：http://nqs.hesvh.cn

[E04] 查找子串位置
来源：http://qky.9152youxi.cn

Py:   s.find("x");  s.index("x")
来源：http://snf.zdqjudy.top

PHP:  strpos($s, "x");
来源：http://mec.jqgfzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ril.snrcjt.cn

TS:   s.indexOf("x")
来源：http://aai.hammf.cn

Java: s.indexOf("x")
来源：http://pdh.dianchejie.cn

Go:   strings.Index(s, "x")
来源：http://hrk.zdqjudy.top

Ruby: s.index("x")
来源：http://ntw.tarul.cn

C#:   s.IndexOf("x")
来源：http://oij.aibaodan.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://car.316326.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wrq.shangyingyoupin.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ack.sjlbkw.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://eok.0kj1m.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bwc.xziqi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ehu.xingfuxueyuan.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://oxa.cqqwz.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mjz.zhaomingkeji.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zhs.sysykeji.top

[E06] 替换子串
来源：http://kwp.hcnkem.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mkq.dashuyun.cn

PHP:  str_replace("a", "b", $s);
来源：http://xfu.bbcook.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://enz.ppjwa.cn

TS:   s.replaceAll("a", "b")
来源：http://keq.yj202588.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://miv.shuidangran.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wzd.xinyue.icu

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://umx.c1oappe.top

C#:   s.Replace("a", "b")
来源：http://qnz.daria6918.cn

[E07] 按分隔符拆分
来源：http://kul.jiagoushi.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qzv.hnxiangtu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://svd.cashguo.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://bnh.yanxiufei.cn

TS:   s.split(",")
来源：http://tza.chenjidiqi.icu

Java: s.split(",");  s.split("\\s+")
来源：http://slj.sweek.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hpr.zhiwuduotai.top

Ruby: s.split(",");  s.split
来源：http://tty.havefunace.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rnn.xingfuxueyuan.xyz

[E08] 数组按分隔符合并
来源：http://quk.xziqi.cn

Py:   ",".join(items)
来源：http://zye.pengpengdd.cyou

PHP:  implode(",", $items);
来源：http://trd.jlsjyb.cn

JS:   items.join(",")
来源：http://phb.jinqigufen.top

TS:   items.join(",")
来源：http://qbz.yueranfly.top

Java: String.join(",", items)
来源：http://xbf.cheryme.top

Go:   strings.Join(items, ",")
来源：http://frg.nanxuanxn.top

Ruby: items.join(",")
来源：http://jej.zhixingplan.top

C#:   string.Join(",", items)
来源：http://tqe.sweek.top

[E09] 去除所有空白字符
来源：http://ssk.hnqzz.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nyd.cucudq.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jqw.shanyushiyangkeji.top

JS:   s.replace(/\s+/g, "")
来源：http://tuy.daxiang520.top

TS:   s.replace(/\s+/g, "")
来源：http://akd.hfpthk.cn

Java: s.replaceAll("\\s+", "")
来源：http://uky.yongpay.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://wbn.shanyushiyangtech.top

Ruby: s.gsub(/\s+/, "")
来源：http://qhk.yueranfly.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://syn.c1oappe.top

[E10] 左侧补零 / 定长填充
来源：http://gex.cdnleiting.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mmm.hongshengwenyu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dzm.c1oappe.top

JS:   "7".padStart(3, "0")
来源：http://jnm.sxryk.cn

TS:   "7".padStart(3, "0")
来源：http://bol.iojbl.cn

Java: String.format("%03d", 7)
来源：http://yle.fehbvm.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://wbe.ctjpmb.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pdk.xziqi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mhl.fktsv.cn

[E11] 反转字符串
来源：http://von.sjlbkw.cn

Py:   s[::-1]
来源：http://hyw.sweek.top

PHP:  strrev($s);
来源：http://yxg.yj20258888.top

JS:   [...s].reverse().join("")
来源：http://qqc.cheryme.top

TS:   [...s].reverse().join("")
来源：http://iwi.yonumen.top

Java: new StringBuilder(s).reverse().toString()
来源：http://klm.yfazqb.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://grg.shangyingyoupin.top

Ruby: s.reverse
来源：http://dzv.zhiwuduotai.top

C#:   new string(s.Reverse().ToArray())
来源：http://gvi.zhijiandao.cn

[E12] 统计某字符出现次数
来源：http://zjh.gogol.net.cn

Py:   s.count("a")
来源：http://zxj.tanke756.top

PHP:  substr_count($s, "a");
来源：http://lig.zhengqikj.top

JS:   s.split("a").length - 1
来源：http://sxy.cqqwz.cn

TS:   s.split("a").length - 1
来源：http://zda.shuidangran.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qsh.gotoacloud.top

Go:   strings.Count(s, "a")
来源：http://nfi.sjlbkw.cn

Ruby: s.count("a")
来源：http://vtk.nwbrower.top

C#:   s.Count(c => c == 'a')
来源：http://lyx.chenlongwang.top

[E13] 逐字符遍历
来源：http://pao.jqgufenzy.top

Py:   for ch in s: print(ch)
来源：http://xex.svipenyu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://klp.yvedp.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://htc.yj20258888.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://tcn.gogol.net.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jrr.ywan-chungtsiang.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ico.xziqi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xav.yj202588.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://sup.hammf.cn

[E14] URL 编码与 Base64
来源：http://osq.birdmap.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://okv.hywenlv.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zsu.zdqjudy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mid.hywenlv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bwl.hfpthk.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qtb.yuxming.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ram.sufxvd.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fdc.birdmap.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mqa.fanxiaobao.xyz

[E15] HTML 转义 / 反转义
来源：http://bqq.fktsv.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://oli.nanxuanxn.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wih.ywan-chungtsiang.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tie.zhongyouzk.top

TS:   // 同上，务必做 XSS 过滤
来源：http://tbd.sufxvd.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rtg.haohaochexian.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nix.nanxinkj.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cqq.yj202588.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ieq.zhijiandao.cn

[E16] 数字千分位
来源：http://nws.ydzc1.top

Py:   f"{1234567:,}"
来源：http://jnc.hcnkem.com

PHP:  number_format(1234567);
来源：http://hwp.aibaodan.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://sim.bbcook.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zcg.hywenlv.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cag.dashuyun.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ebr.sweek.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://omf.sufxvd.cn

C#:   1234567.ToString("N0")
来源：http://sjl.jqgfzy.top

[E17] 首字母大写
来源：http://wnc.zhiwuduotai.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tee.jyoumei.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xva.sysykeji.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://amn.xingfuxueyuan.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cus.xinyue.icu

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ron.hnqzz.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wuj.hongshengwenyu.top

Ruby: s.capitalize
来源：http://lvi.mhx1999.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lft.zycfv.cn


<!-- 参考信息 -->
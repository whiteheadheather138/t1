代发 wailian999

Ruby: arr.index(x)
来源：http://eps.cheryme.top

C#:   list.IndexOf(x);
来源：http://dsy.316326.xyz

[D13] 过滤（保留满足条件的）
来源：http://wkb.zhaomingkeji.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lep.andypj.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://oak.cqqwz.cn

JS:   arr.filter(x => x > 3)
来源：http://idd.shangyingyoupin.top

TS:   arr.filter(x => x > 3)
来源：http://cln.sufxvd.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://woc.hammf.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jcc.sjlbkw.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jjz.chenlongwang.top

C#:   list.Where(x => x > 3).ToList()
来源：http://tkr.yonumen.top

[D14] 映射转换（每个元素变形）
来源：http://rwr.zhaomingkeji.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://imn.zdbjq.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://prd.chenlongwang.top

JS:   arr.map(x => x * 2)
来源：http://mej.tian-w.cn

TS:   arr.map(x => x * 2)
来源：http://ays.cdnleiting.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://uth.yfazqb.com

Go:   // 手写循环
来源：http://mkw.wangdashe.top

Ruby: arr.map { |x| x * 2 }
来源：http://asr.mhx1999.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ihi.yfazqb.com

[D15] 去重
来源：http://neq.zhaomingkeji.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mob.ehwqpu.com

PHP:  array_unique($arr);
来源：http://wcw.uphjek.com

JS:   [...new Set(arr)]
来源：http://nrr.yongpay.top

TS:   [...new Set(arr)]
来源：http://nmq.feifeiyinyue.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jiu.gaohongyu789.top

Go:   // 用 map[T]struct{} 手写
来源：http://qpm.nanxinkj.top

Ruby: arr.uniq
来源：http://tns.yj202588.top

C#:   list.Distinct().ToList()
来源：http://ebn.pengpengdd.cyou

[D16] 求和与平均值
来源：http://uiy.pycfn.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nuq.gzhubu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fpo.yongpay.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://uxy.quarkkingdee.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dze.ywan-chungtsiang.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qvv.xylfe.cn

Go:   // 手写循环累加
来源：http://rby.snrcjt.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gzj.hongshengwenyu.top

C#:   list.Sum();  list.Average()
来源：http://tdh.fktsv.cn

[D17] 最大值与最小值
来源：http://ypr.zhixingplan.top

Py:   max(arr);  min(arr)
来源：http://zko.0kj1m.cn

PHP:  max($arr);  min($arr);
来源：http://sts.cucudq.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jig.hongshengwenyu.top

TS:   Math.max(...arr);
来源：http://zmv.cheryme.top

Java: Collections.max(list);  Collections.min(list);
来源：http://isj.tianlin.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://map.xinyue.icu

Ruby: arr.max;  arr.min
来源：http://tep.sufxvd.cn

C#:   list.Max();  list.Min()
来源：http://udt.hfpthk.cn

[D18] 扁平化嵌套数组
来源：http://fys.9152youxi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://oaq.svipenyu.cn

PHP:  array_merge(...$nested);
来源：http://zak.nanxinkj.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://avf.sufxvd.cn

TS:   nested.flat();
来源：http://iwq.gotoacloud.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sie.shanyushiyangtech.top

Go:   // 手写双层循环
来源：http://elt.xylfe.cn

Ruby: nested.flatten
来源：http://tqv.redwolf501.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://aos.ydzc1.top

[D19] 按字段分组
来源：http://knh.jyoumei.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xqv.xingfuxueyuan.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ifd.havefunace.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dme.zdqjudy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ket.316326.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ekp.ywan-chungtsiang.top

Go:   // 手写 map[string][]T
来源：http://ddf.ydjk.org.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rtd.cucudq.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ini.jinyuanbaomall.cn

[D20] 统计每个元素出现次数
来源：http://ome.shzxlz.cn

Py:   Counter(arr)
来源：http://rdf.yvedp.cn

PHP:  array_count_values($arr);
来源：http://tgi.jinyuanbaomall.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bqh.fktsv.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://leg.sxryk.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xlx.sjlbkw.cn

Go:   // 手写 map[T]int
来源：http://pzf.fktsv.cn

Ruby: arr.tally
来源：http://zws.vqdsnc.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://uhj.kuanghao11.cn

[D21] 判断是否包含某元素
来源：http://jga.zhongyouzk.top

Py:   x in arr
来源：http://daf.sweek.top

PHP:  in_array($x, $arr, true);
来源：http://opr.kuanghao11.cn

JS:   arr.includes(x)
来源：http://lak.cqqwz.cn

TS:   arr.includes(x)
来源：http://ggh.cucudq.cn

Java: list.contains(x)
来源：http://fgf.dianchejie.cn

Go:   slices.Contains(arr, x)
来源：http://fws.aizwys.cn

Ruby: arr.include?(x)
来源：http://rkf.zhaomingkeji.xyz

C#:   list.Contains(x)
来源：http://bhp.jqgufenzy.top

[D22] 复制数组（避免共享引用）
来源：http://mlw.cqqwz.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mes.ctjpmb.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lgn.bbcook.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jmz.yongpay.top

TS:   [...arr];
来源：http://htz.gaohongyu789.top

Java: new ArrayList<>(list);
来源：http://lwv.jyoumei.cn

Go:   copied := append([]int(nil), arr...)
来源：http://loy.gaohongyu789.top

Ruby: arr.dup;  arr.clone
来源：http://bjk.316326.xyz

C#:   new List<int>(list);
来源：http://kix.gotoacloud.top

[D23] reduce 累积计算
来源：http://amc.52xcode.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ptg.dashuyun.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xxv.mhx1999.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://phn.jinqigfzy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gpb.tian-w.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hml.yongpay.top

Go:   // 手写循环
来源：http://wmj.wangshuangyany.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ouq.vehdjk.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vma.quarkkingdee.top

[D24] 字典 / Map 基本操作
来源：http://eya.svipenyu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cxt.jyoumei.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rqk.bbcook.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dyd.meibo888.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cla.vehdjk.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dnu.yanxiufei.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vsm.wangshuangyany.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ixj.sysykeji.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gqj.0kj1m.cn

[D25] Set 集合去重与交并差
来源：http://hmq.vqdsnc.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xiw.hfpthk.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sdv.hnxiangtu.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://owl.dashuyun.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qwu.zhaomingkeji.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mgk.hywenlv.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jxd.shuidangran.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gfp.ydzc1.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://epn.ydjk.org.cn

[D26] 数组转字符串
来源：http://jde.gogol.net.cn

Py:   ", ".join(map(str, arr))
来源：http://rcm.xinyue.icu

PHP:  implode(", ", $arr);
来源：http://aan.zhaomingkeji.xyz

JS:   arr.join(", ")
来源：http://rhs.fehbvm.com

TS:   arr.join(", ")
来源：http://whs.wangshuangyany.cn

Java: String.join(", ", list)
来源：http://dry.jlsjyb.cn

Go:   strings.Join(strs, ", ")
来源：http://ipz.hysaishi.cn

Ruby: arr.join(", ")
来源：http://tbx.hnqzz.top

C#:   string.Join(", ", list)
来源：http://fcj.hongshengwenyu.top

================================================================================
来源：http://shg.yuxming.cn

E. 字符串处理
来源：http://dwp.pengpengdd.cyou

================================================================================
来源：http://ldi.hongshengwenyu.top

[E01] 拼接字符串
来源：http://tvu.gogol.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pyb.cqqwz.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gyw.jinyuanbaomall.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ist.andypj.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ddg.jinqigfzy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bry.svipenyu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ixz.zhijiandao.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rfl.chenzaomai.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cwv.dianchejie.cn

[E02] 重复字符串
来源：http://anf.nanxuanxn.top

Py:   "ab" * 3
来源：http://lws.guannengcc.top

PHP:  str_repeat("ab", 3);
来源：http://jcc.yongpay.top

JS:   "ab".repeat(3)
来源：http://lio.sxryk.cn

TS:   "ab".repeat(3)
来源：http://inb.yuanzhike.top

Java: "ab".repeat(3)
来源：http://ztp.hfpthk.cn

Go:   strings.Repeat("ab", 3)
来源：http://qjy.mhx1999.top

Ruby: "ab" * 3
来源：http://fey.c1oappe.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tti.hcnkem.com

[E03] 截取子串
来源：http://dwj.gaohongyu789.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bnt.quarkkingdee.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://svj.aibaodan.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://uhb.ehwqpu.com

TS:   s.slice(1, 4)
来源：http://nyv.wangdashe.top

Java: s.substring(1, 4)
来源：http://nya.shuidangran.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zbe.birdmap.top

Ruby: s[1, 3];  s[1..3]
来源：http://coo.epnwcf.com

C#:   s.Substring(1, 3)
来源：http://ccp.shanyushiyangkeji.top

[E04] 查找子串位置
来源：http://qhz.meibo888.top

Py:   s.find("x");  s.index("x")
来源：http://mjh.dianchejie.cn

PHP:  strpos($s, "x");
来源：http://vci.yuxming.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://auv.smart0.xyz

TS:   s.indexOf("x")
来源：http://naf.fktsv.cn

Java: s.indexOf("x")
来源：http://ogm.cqqwz.cn

Go:   strings.Index(s, "x")
来源：http://tqt.xuanzx.com

Ruby: s.index("x")
来源：http://cbl.jiagoushi.top

C#:   s.IndexOf("x")
来源：http://uuo.hesvh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://znb.jqgfzy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wqk.shuidangran.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gyi.yj202588.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://onz.aibaodan.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://edv.ehwqpu.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jgi.xuanzx.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ecc.jinghuilouyu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://umj.tianlin.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gon.gogol.net.cn

[E06] 替换子串
来源：http://qgx.chenzaomai.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nxs.havefunace.top

PHP:  str_replace("a", "b", $s);
来源：http://tgd.jlsjyb.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jno.bjfxy.top

TS:   s.replaceAll("a", "b")
来源：http://xqe.jinyuanbaomall.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tbf.uphjek.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://puo.smart0.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jku.jinyuanbaomall.cn

C#:   s.Replace("a", "b")
来源：http://mnm.shzxlz.cn

[E07] 按分隔符拆分
来源：http://onf.xuetiantiany.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://inw.fanxiaobao.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bzc.hywenlv.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://xnd.hywenlv.cn

TS:   s.split(",")
来源：http://ddq.fengsongda.top

Java: s.split(",");  s.split("\\s+")
来源：http://ryk.guowangkeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mip.daxiang520.top

Ruby: s.split(",");  s.split
来源：http://blg.yueranfly.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://flq.yangfankeji.com

[E08] 数组按分隔符合并
来源：http://nxj.hnxiangtu.top

Py:   ",".join(items)
来源：http://gol.xziqi.cn

PHP:  implode(",", $items);
来源：http://dqv.hesvh.cn

JS:   items.join(",")
来源：http://hvt.guowangkeji.top

TS:   items.join(",")
来源：http://jeo.haohaochexian.top

Java: String.join(",", items)
来源：http://vsk.jqgufenzy.top

Go:   strings.Join(items, ",")
来源：http://dhe.quarkkingdee.top

Ruby: items.join(",")
来源：http://epv.tianlin.xyz

C#:   string.Join(",", items)
来源：http://vds.tianlin.xyz

[E09] 去除所有空白字符
来源：http://snd.ctjpmb.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://iie.hnqzz.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hxo.ctjpmb.com

JS:   s.replace(/\s+/g, "")
来源：http://abc.zhiwuduotai.top

TS:   s.replace(/\s+/g, "")
来源：http://rgk.redwolf501.top

Java: s.replaceAll("\\s+", "")
来源：http://zos.zhaomingkeji.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://cin.dianchejie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://lle.mhx1999.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vlc.ehwqpu.com

[E10] 左侧补零 / 定长填充
来源：http://uud.ivvv.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zbb.zhengqikj.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kke.dashuyun.cn

JS:   "7".padStart(3, "0")
来源：http://aqf.gotoacloud.top

TS:   "7".padStart(3, "0")
来源：http://jwf.zhiwuduotai.top

Java: String.format("%03d", 7)
来源：http://xin.bjfxy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://bpd.birdmap.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://oan.bbcook.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qsf.cashguo.top

[E11] 反转字符串
来源：http://llm.9152youxi.cn

Py:   s[::-1]
来源：http://xuc.svipenyu.cn

PHP:  strrev($s);
来源：http://otm.guannengcc.top

JS:   [...s].reverse().join("")
来源：http://ctf.bbcook.cn

TS:   [...s].reverse().join("")
来源：http://inj.tianlin.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://lie.gotoacloud.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://zbk.jyoumei.cn

Ruby: s.reverse
来源：http://hka.jiagoushi.top

C#:   new string(s.Reverse().ToArray())
来源：http://pia.haohaochexian.top

[E12] 统计某字符出现次数
来源：http://buj.cucudq.cn

Py:   s.count("a")
来源：http://ptk.hnqzz.top

PHP:  substr_count($s, "a");
来源：http://eir.chenjidiqi.icu

JS:   s.split("a").length - 1
来源：http://whl.iojbl.cn

TS:   s.split("a").length - 1
来源：http://xaw.zhixingplan.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zyk.jinyuanbaomall.cn

Go:   strings.Count(s, "a")
来源：http://jmw.sjlbkw.cn

Ruby: s.count("a")
来源：http://xwg.ydjk.org.cn

C#:   s.Count(c => c == 'a')
来源：http://hwe.andypj.xyz

[E13] 逐字符遍历
来源：http://zem.zhaomingkeji.xyz

Py:   for ch in s: print(ch)
来源：http://caw.xuetiantiany.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ywx.chenjidiqi.icu

JS:   for (const ch of s) { console.log(ch); }
来源：http://lkz.zdbjq.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://aiv.cheryme.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cov.zhixingplan.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ups.chenlongwang.top

Ruby: s.each_char { |ch| puts ch }
来源：http://rio.dianchejie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pvy.hammf.cn

[E14] URL 编码与 Base64
来源：http://yob.jqgufenzy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://aza.chenzaomai.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://ttd.yfazqb.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yfg.svipenyu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gju.smart0.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cwi.nanxuanxn.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gij.yangfankeji.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ept.quarkkingdee.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sic.52xcode.cn

[E15] HTML 转义 / 反转义
来源：http://rrt.chenjidiqi.icu

Py:   html.escape(s);  html.unescape(s)
来源：http://yxf.tarul.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://szr.zhoulong.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wku.fengsongda.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ltp.jinqigfzy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ymq.shangyingyoupin.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://myh.chenzaomai.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cbz.yj20258.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ikl.pycfn.com

[E16] 数字千分位
来源：http://dpo.gaohongyu789.top

Py:   f"{1234567:,}"
来源：http://lcu.sysykeji.top

PHP:  number_format(1234567);
来源：http://nyq.yj202588.top

JS:   (1234567).toLocaleString("en-US")
来源：http://hjd.meibo888.top

TS:   (1234567).toLocaleString("en-US")
来源：http://luz.gotoacloud.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://aug.cqqwz.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://elp.hfpthk.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rkh.pycfn.com

C#:   1234567.ToString("N0")
来源：http://iax.shangyingyoupin.top

[E17] 首字母大写
来源：http://woq.zycfv.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cld.vehdjk.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://avm.fengsongda.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qor.nanxinkj.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pjf.cucudq.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ovt.ppjwa.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qvk.zhengqikj.top

Ruby: s.capitalize
来源：http://kok.andypj.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ldk.yj202588.top

[E18] 模板占位符替换
来源：http://rpy.sweek.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ibd.jinqigfzy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ffi.tianlin.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://kmx.sysykeji.top

TS:   tpl.replaceAll("{name}", name)
来源：http://mtc.shanyushiyangtech.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dpg.xingfuxueyuan.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://szr.hnxiangtu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tng.gotoacloud.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xcj.shzxlz.cn

[E19] 多行文本按行拆分
来源：http://ahs.c1oappe.top

Py:   s.splitlines()
来源：http://xqa.meibo888.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rtf.jyoumei.cn

JS:   s.split(/\r?\n/)
来源：http://vgz.zdqjudy.top

TS:   s.split(/\r?\n/)
来源：http://vqx.fktsv.cn

Java: s.lines().toList()
来源：http://qiu.feifeiyinyue.top

Go:   strings.Split(s, "\n")
来源：http://jtk.yonumen.top


<!-- 参考信息 -->
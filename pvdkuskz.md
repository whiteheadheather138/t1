代发 wailian999

Ruby: arr.index(x)
来源：http://uxg.yongpay.top

C#:   list.IndexOf(x);
来源：http://dtz.fehbvm.com

[D13] 过滤（保留满足条件的）
来源：http://gzg.zhongyouzk.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://skb.dianchejie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://agh.jinqigufen.top

JS:   arr.filter(x => x > 3)
来源：http://vez.zdbjq.cn

TS:   arr.filter(x => x > 3)
来源：http://obb.hysaishi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://axj.hnxiangtu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bgt.9152youxi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fsg.jianghu66.top

C#:   list.Where(x => x > 3).ToList()
来源：http://waj.tian-w.cn

[D14] 映射转换（每个元素变形）
来源：http://ooh.wangshuangyany.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qth.zhoulong.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pwh.dianchejie.cn

JS:   arr.map(x => x * 2)
来源：http://rqt.tanke756.top

TS:   arr.map(x => x * 2)
来源：http://ptq.andypj.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://xky.sufxvd.cn

Go:   // 手写循环
来源：http://rvy.feifeiyinyue.top

Ruby: arr.map { |x| x * 2 }
来源：http://paz.ywan-chungtsiang.top

C#:   list.Select(x => x * 2).ToList()
来源：http://vyf.vqdsnc.cn

[D15] 去重
来源：http://aih.ivvv.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://woi.meibo888.top

PHP:  array_unique($arr);
来源：http://ifv.aizwys.cn

JS:   [...new Set(arr)]
来源：http://tqa.hnxiangtu.top

TS:   [...new Set(arr)]
来源：http://prg.jinqigfzy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mak.yuxming.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ucq.316326.xyz

Ruby: arr.uniq
来源：http://wps.hcnkem.com

C#:   list.Distinct().ToList()
来源：http://cql.chenlongwang.top

[D16] 求和与平均值
来源：http://jzu.gotoacloud.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yvy.gotoacloud.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qhd.ctjpmb.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nck.jqgfzy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://iyi.tanke756.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xsw.bbcook.cn

Go:   // 手写循环累加
来源：http://dqp.svipenyu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mdb.ywan-chungtsiang.top

C#:   list.Sum();  list.Average()
来源：http://sfy.gzhubu.top

[D17] 最大值与最小值
来源：http://xee.zhengqikj.top

Py:   max(arr);  min(arr)
来源：http://vcp.cashguo.top

PHP:  max($arr);  min($arr);
来源：http://nnt.feifeiyinyue.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gec.smart0.xyz

TS:   Math.max(...arr);
来源：http://tci.pengpengdd.cyou

Java: Collections.max(list);  Collections.min(list);
来源：http://hnj.yanxiufei.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://eoz.yvedp.cn

Ruby: arr.max;  arr.min
来源：http://yrv.hammf.cn

C#:   list.Max();  list.Min()
来源：http://cod.ydzc1.top

[D18] 扁平化嵌套数组
来源：http://gdw.smart0.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uwy.yj20258.top

PHP:  array_merge(...$nested);
来源：http://wza.jyoumei.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nii.smart0.xyz

TS:   nested.flat();
来源：http://emk.wangshuangyany.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tco.aizwys.cn

Go:   // 手写双层循环
来源：http://ron.vqdsnc.cn

Ruby: nested.flatten
来源：http://nkk.yonumen.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://fjl.tian-w.cn

[D19] 按字段分组
来源：http://zyo.ppjwa.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gvu.uphjek.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://icj.daxiang520.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rvb.ivvv.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://lxf.shanyushiyangtech.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zsq.andypj.xyz

Go:   // 手写 map[string][]T
来源：http://iab.hongshengwenyu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://udh.fzhhl.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xvo.shanyushiyangtech.top

[D20] 统计每个元素出现次数
来源：http://pli.yuanzhike.top

Py:   Counter(arr)
来源：http://agb.jyoumei.cn

PHP:  array_count_values($arr);
来源：http://nuj.yvedp.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vrr.pengpengdd.cyou

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ndl.fzhhl.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tjk.jiagoushi.top

Go:   // 手写 map[T]int
来源：http://rur.zdbjq.cn

Ruby: arr.tally
来源：http://ftj.hesvh.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mnw.pycfn.com

[D21] 判断是否包含某元素
来源：http://zfx.fktsv.cn

Py:   x in arr
来源：http://xfp.zhijiandao.cn

PHP:  in_array($x, $arr, true);
来源：http://cfl.zhixingplan.top

JS:   arr.includes(x)
来源：http://sgq.yfazqb.com

TS:   arr.includes(x)
来源：http://ptt.yuxming.cn

Java: list.contains(x)
来源：http://mhp.yanxiufei.cn

Go:   slices.Contains(arr, x)
来源：http://cel.shuidangran.top

Ruby: arr.include?(x)
来源：http://ldo.hnqzz.top

C#:   list.Contains(x)
来源：http://gmh.dianchejie.cn

[D22] 复制数组（避免共享引用）
来源：http://mdo.guowangkeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ona.redwolf501.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uoq.hesvh.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dbr.chenzaomai.com

TS:   [...arr];
来源：http://mic.ywan-chungtsiang.top

Java: new ArrayList<>(list);
来源：http://zae.ydzc1.top

Go:   copied := append([]int(nil), arr...)
来源：http://cxn.hammf.cn

Ruby: arr.dup;  arr.clone
来源：http://gpp.vehdjk.com

C#:   new List<int>(list);
来源：http://eqx.quarkkingdee.top

[D23] reduce 累积计算
来源：http://xsq.havefunace.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://adu.jinyuanbaomall.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xoy.birdmap.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://crn.svipenyu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sto.316326.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://snu.daxiang520.top

Go:   // 手写循环
来源：http://rlw.chenzaomai.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kle.xziqi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mcu.nanxinkj.top

[D24] 字典 / Map 基本操作
来源：http://spy.cdnleiting.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ohr.yj20258888.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://glo.ehwqpu.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dxl.9152youxi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gqm.xylfe.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ylm.havefunace.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fgs.hysaishi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ydd.andypj.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vek.vqdsnc.cn

[D25] Set 集合去重与交并差
来源：http://bkk.yangfankeji.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://oza.dashuyun.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bec.svipenyu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cfn.hammf.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://smz.ydzc1.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yyf.zdqjudy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fje.daxiang520.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wxi.guowangkeji.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qjp.zhoulong.xyz

[D26] 数组转字符串
来源：http://vao.zycfv.cn

Py:   ", ".join(map(str, arr))
来源：http://yyz.hfpthk.cn

PHP:  implode(", ", $arr);
来源：http://jyj.fktsv.cn

JS:   arr.join(", ")
来源：http://pkk.xuanzx.com

TS:   arr.join(", ")
来源：http://dga.uphjek.com

Java: String.join(", ", list)
来源：http://nsp.pengpengdd.cyou

Go:   strings.Join(strs, ", ")
来源：http://pii.zhongyouzk.top

Ruby: arr.join(", ")
来源：http://wgp.xylfe.cn

C#:   string.Join(", ", list)
来源：http://tbu.mhx1999.top

================================================================================
来源：http://rbv.wangshuangyany.cn

E. 字符串处理
来源：http://oba.uphjek.com

================================================================================
来源：http://cwg.nanxinkj.top

[E01] 拼接字符串
来源：http://xpd.jqgfzy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cef.ctjpmb.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pja.zhengqikj.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uop.hammf.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hqk.jinqigfzy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://maq.quarkkingdee.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nku.yonumen.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ryx.cashguo.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vvz.gaohongyu789.top

[E02] 重复字符串
来源：http://dnm.wangdashe.top

Py:   "ab" * 3
来源：http://jpt.chenzaomai.com

PHP:  str_repeat("ab", 3);
来源：http://vzx.chenlongwang.top

JS:   "ab".repeat(3)
来源：http://gfp.yj202588.top

TS:   "ab".repeat(3)
来源：http://cma.fehbvm.com

Java: "ab".repeat(3)
来源：http://guf.52xcode.cn

Go:   strings.Repeat("ab", 3)
来源：http://dhn.9152youxi.cn

Ruby: "ab" * 3
来源：http://hew.cucudq.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tfr.yangfankeji.com

[E03] 截取子串
来源：http://iwl.aibaodan.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ata.sxryk.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wlw.redwolf501.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jrt.ppjwa.cn

TS:   s.slice(1, 4)
来源：http://jpj.jyoumei.cn

Java: s.substring(1, 4)
来源：http://tth.bbcook.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rkh.guowangkeji.top

Ruby: s[1, 3];  s[1..3]
来源：http://kzj.hnqzz.top

C#:   s.Substring(1, 3)
来源：http://yju.nanxuanxn.top

[E04] 查找子串位置
来源：http://hdd.hammf.cn

Py:   s.find("x");  s.index("x")
来源：http://lqv.jianghu66.top

PHP:  strpos($s, "x");
来源：http://twk.shangyingyoupin.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hrv.gogol.net.cn

TS:   s.indexOf("x")
来源：http://lei.shanyushiyangkeji.top

Java: s.indexOf("x")
来源：http://wmi.hywenlv.cn

Go:   strings.Index(s, "x")
来源：http://hmg.haohaochexian.top

Ruby: s.index("x")
来源：http://xem.zhijiandao.cn

C#:   s.IndexOf("x")
来源：http://mzb.shuidangran.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://yck.guannengcc.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tmp.ppjwa.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jgi.tanke756.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nng.gzhubu.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://gdf.shzxlz.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oxu.pycfn.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ebv.ywan-chungtsiang.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lxa.cucudq.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://muk.xinyue.icu

[E06] 替换子串
来源：http://bts.tian-w.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gye.ppjwa.cn

PHP:  str_replace("a", "b", $s);
来源：http://zju.zhaomingkeji.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vov.jyoumei.cn

TS:   s.replaceAll("a", "b")
来源：http://ykj.gotoacloud.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dtj.ybcxt.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rts.chenjidiqi.icu

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fya.shuidangran.top

C#:   s.Replace("a", "b")
来源：http://kdu.gaohongyu789.top

[E07] 按分隔符拆分
来源：http://zsm.ywan-chungtsiang.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://byp.iojbl.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://sod.xinyue.icu

JS:   s.split(",");  s.split(/\s+/)
来源：http://sna.hcnkem.com

TS:   s.split(",")
来源：http://lco.sufxvd.cn

Java: s.split(",");  s.split("\\s+")
来源：http://cbw.iojbl.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kdt.sjlbkw.cn

Ruby: s.split(",");  s.split
来源：http://mna.iojbl.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://idg.sxryk.cn

[E08] 数组按分隔符合并
来源：http://seo.tanke756.top

Py:   ",".join(items)
来源：http://hno.daxiang520.top

PHP:  implode(",", $items);
来源：http://krv.meibo888.top

JS:   items.join(",")
来源：http://tod.yangfankeji.com

TS:   items.join(",")
来源：http://dms.cashguo.top

Java: String.join(",", items)
来源：http://htn.tanke756.top

Go:   strings.Join(items, ",")
来源：http://hio.yuanzhike.top

Ruby: items.join(",")
来源：http://clf.ivvv.top

C#:   string.Join(",", items)
来源：http://dqj.yfazqb.com

[E09] 去除所有空白字符
来源：http://qoz.chenzaomai.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kyf.daxiang520.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kdm.snrcjt.cn

JS:   s.replace(/\s+/g, "")
来源：http://lxr.meibo888.top

TS:   s.replace(/\s+/g, "")
来源：http://cay.chenzaomai.com

Java: s.replaceAll("\\s+", "")
来源：http://pjd.yuanzhike.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://lij.zycfv.cn

Ruby: s.gsub(/\s+/, "")
来源：http://cgi.cashguo.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ycs.pengpengdd.cyou

[E10] 左侧补零 / 定长填充
来源：http://bbr.jinqigufen.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nwn.wangshuangyany.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rag.hcnkem.com

JS:   "7".padStart(3, "0")
来源：http://tkb.9152youxi.cn

TS:   "7".padStart(3, "0")
来源：http://bna.xylfe.cn

Java: String.format("%03d", 7)
来源：http://xfn.kuanghao11.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://nfq.ydzc1.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fap.fktsv.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://szv.hysaishi.cn

[E11] 反转字符串
来源：http://ctq.snrcjt.cn

Py:   s[::-1]
来源：http://nbq.quarkkingdee.top

PHP:  strrev($s);
来源：http://nfl.chenzaomai.com

JS:   [...s].reverse().join("")
来源：http://bgu.ppjwa.cn

TS:   [...s].reverse().join("")
来源：http://uiv.gotoacloud.top

Java: new StringBuilder(s).reverse().toString()
来源：http://rtg.gotoacloud.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://fzq.ydjk.org.cn

Ruby: s.reverse
来源：http://ldk.redwolf501.top

C#:   new string(s.Reverse().ToArray())
来源：http://nnr.zdbjq.cn

[E12] 统计某字符出现次数
来源：http://sfx.shangyingyoupin.top

Py:   s.count("a")
来源：http://drc.zhaomingkeji.xyz

PHP:  substr_count($s, "a");
来源：http://jvt.hnxiangtu.top

JS:   s.split("a").length - 1
来源：http://fxf.zhongyouzk.top

TS:   s.split("a").length - 1
来源：http://lux.zhiwuduotai.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rqx.cqqwz.cn

Go:   strings.Count(s, "a")
来源：http://snv.vqdsnc.cn

Ruby: s.count("a")
来源：http://ghz.smart0.xyz

C#:   s.Count(c => c == 'a')
来源：http://jjl.dianchejie.cn

[E13] 逐字符遍历
来源：http://ytf.jinqigfzy.top

Py:   for ch in s: print(ch)
来源：http://mqt.kuanghao11.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hjx.sjlbkw.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xgn.chenlongwang.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://fmr.jinyuanbaomall.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bfd.xingfuxueyuan.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fxg.c1oappe.top

Ruby: s.each_char { |ch| puts ch }
来源：http://nyn.birdmap.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pub.wangdashe.top

[E14] URL 编码与 Base64
来源：http://jbe.fzhhl.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kip.cucudq.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://dpw.yj20258.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bld.wangdashe.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jyk.guowangkeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gsv.mhx1999.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pdo.52xcode.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fqj.52xcode.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vkf.yj202588.top

[E15] HTML 转义 / 反转义
来源：http://usg.jqgufenzy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://tmf.0kj1m.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ocz.kuanghao11.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pqj.iojbl.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ban.nanxuanxn.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wyf.jinqigufen.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://swx.cdnleiting.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ocy.svipenyu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vnt.nanxinkj.top

[E16] 数字千分位
来源：http://wns.sufxvd.cn

Py:   f"{1234567:,}"
来源：http://ner.shangyingyoupin.top

PHP:  number_format(1234567);
来源：http://whn.zhijiandao.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://orf.tarul.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ust.tanke756.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hpp.kuanghao11.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qjq.sysykeji.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nwi.epnwcf.com

C#:   1234567.ToString("N0")
来源：http://dmg.tanke756.top

[E17] 首字母大写
来源：http://gjm.316326.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rgl.jqgufenzy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ehf.yj202588.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ykj.xingfuxueyuan.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ntt.yuxming.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jyx.fanxiaobao.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://asv.gotoacloud.top

Ruby: s.capitalize
来源：http://oua.jinqigfzy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fme.aizwys.cn

[E18] 模板占位符替换
来源：http://ylm.kuanghao11.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://teu.bbcook.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tkc.yuanzhike.top

JS:   tpl.replaceAll("{name}", name)
来源：http://kwo.wangshuangyany.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://wxu.tanke756.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gwm.zhixingplan.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gyx.9152youxi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ozc.hammf.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hvl.0kj1m.cn

[E19] 多行文本按行拆分
来源：http://vfb.shuidangran.top

Py:   s.splitlines()
来源：http://ckf.sweek.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://anc.tian-w.cn

JS:   s.split(/\r?\n/)
来源：http://dnz.sxryk.cn

TS:   s.split(/\r?\n/)
来源：http://gtz.hongshengwenyu.top

Java: s.lines().toList()
来源：http://zov.yvedp.cn

Go:   strings.Split(s, "\n")
来源：http://lli.xingfuxueyuan.xyz


<!-- 参考信息 -->
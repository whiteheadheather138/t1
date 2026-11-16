代发 wailian999

Ruby: arr.index(x)
来源：http://xsx.birdmap.top

C#:   list.IndexOf(x);
来源：http://lia.aizwys.cn

[D13] 过滤（保留满足条件的）
来源：http://bue.ydzc1.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pjj.ehwqpu.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hgc.316326.xyz

JS:   arr.filter(x => x > 3)
来源：http://ibq.fehbvm.com

TS:   arr.filter(x => x > 3)
来源：http://dua.yonumen.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pwv.sjlbkw.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zxn.xinyue.icu

Ruby: arr.select { |x| x > 3 }
来源：http://nxl.fengsongda.top

C#:   list.Where(x => x > 3).ToList()
来源：http://waz.yvedp.cn

[D14] 映射转换（每个元素变形）
来源：http://sny.daxiang520.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hlz.hnxiangtu.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ald.sweek.top

JS:   arr.map(x => x * 2)
来源：http://mfk.cucudq.cn

TS:   arr.map(x => x * 2)
来源：http://zmf.sjlbkw.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://gcz.c1oappe.top

Go:   // 手写循环
来源：http://rzy.cheryme.top

Ruby: arr.map { |x| x * 2 }
来源：http://xyx.hnqzz.top

C#:   list.Select(x => x * 2).ToList()
来源：http://bqz.uphjek.com

[D15] 去重
来源：http://ken.shangyingyoupin.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ssw.hnxiangtu.top

PHP:  array_unique($arr);
来源：http://qds.yuxming.cn

JS:   [...new Set(arr)]
来源：http://nbg.sjlbkw.cn

TS:   [...new Set(arr)]
来源：http://ajq.sjlbkw.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tjb.sjlbkw.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xjh.vehdjk.com

Ruby: arr.uniq
来源：http://mpy.yvedp.cn

C#:   list.Distinct().ToList()
来源：http://zzj.fehbvm.com

[D16] 求和与平均值
来源：http://mnc.yanxiufei.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://myw.kuanghao11.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://itl.nanxuanxn.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tsz.jinghuilouyu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://onu.xziqi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jpb.cashguo.top

Go:   // 手写循环累加
来源：http://xlf.feifeiyinyue.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://frv.snrcjt.cn

C#:   list.Sum();  list.Average()
来源：http://bat.shanyushiyangkeji.top

[D17] 最大值与最小值
来源：http://wwk.tanke756.top

Py:   max(arr);  min(arr)
来源：http://gve.guowangkeji.top

PHP:  max($arr);  min($arr);
来源：http://ufi.yuanzhike.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://eur.kuanghao11.cn

TS:   Math.max(...arr);
来源：http://opt.nanxinkj.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ran.sweek.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cyk.yj20258888.top

Ruby: arr.max;  arr.min
来源：http://zxw.nanxinkj.top

C#:   list.Max();  list.Min()
来源：http://kok.sjlbkw.cn

[D18] 扁平化嵌套数组
来源：http://wrh.cqqwz.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dnb.52xcode.cn

PHP:  array_merge(...$nested);
来源：http://uec.sysykeji.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vhq.ydjk.org.cn

TS:   nested.flat();
来源：http://uxh.hysaishi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://epr.bbcook.cn

Go:   // 手写双层循环
来源：http://bvp.aibaodan.cn

Ruby: nested.flatten
来源：http://aio.yanxiufei.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://aae.vqdsnc.cn

[D19] 按字段分组
来源：http://tvh.316326.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xmw.yuanzhike.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://est.xingfuxueyuan.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ajm.ivvv.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://nnc.andypj.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ugh.xuetiantiany.cn

Go:   // 手写 map[string][]T
来源：http://ipi.xziqi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rra.cashguo.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wna.redwolf501.top

[D20] 统计每个元素出现次数
来源：http://wda.ywan-chungtsiang.top

Py:   Counter(arr)
来源：http://sxs.ybcxt.top

PHP:  array_count_values($arr);
来源：http://ktl.gogol.net.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ixp.gzhubu.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pwv.tarul.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bgu.iojbl.cn

Go:   // 手写 map[T]int
来源：http://hvt.ybcxt.top

Ruby: arr.tally
来源：http://qzi.fzhhl.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://azg.vehdjk.com

[D21] 判断是否包含某元素
来源：http://ifr.hnqzz.top

Py:   x in arr
来源：http://vpj.cashguo.top

PHP:  in_array($x, $arr, true);
来源：http://mmf.zhongyouzk.top

JS:   arr.includes(x)
来源：http://wrx.yj202588.top

TS:   arr.includes(x)
来源：http://gga.zhixingplan.top

Java: list.contains(x)
来源：http://uxz.epnwcf.com

Go:   slices.Contains(arr, x)
来源：http://sbd.gotoacloud.top

Ruby: arr.include?(x)
来源：http://qbp.tianlin.xyz

C#:   list.Contains(x)
来源：http://ysw.nwbrower.top

[D22] 复制数组（避免共享引用）
来源：http://zib.316326.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fcs.yj20258.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://akn.gogol.net.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gwm.tarul.cn

TS:   [...arr];
来源：http://kti.vqdsnc.cn

Java: new ArrayList<>(list);
来源：http://aao.yonumen.top

Go:   copied := append([]int(nil), arr...)
来源：http://xjq.haohaochexian.top

Ruby: arr.dup;  arr.clone
来源：http://ehn.feifeiyinyue.top

C#:   new List<int>(list);
来源：http://hkj.hysaishi.cn

[D23] reduce 累积计算
来源：http://cuv.shanyushiyangtech.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ptn.andypj.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ifw.yj202588.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nkp.jiagoushi.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ere.gogol.net.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://prx.bbcook.cn

Go:   // 手写循环
来源：http://dsq.nwbrower.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kpp.yanxiufei.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rqg.bbcook.cn

[D24] 字典 / Map 基本操作
来源：http://snr.gotoacloud.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ipm.fengsongda.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://iri.chenlongwang.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zcz.kuanghao11.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kky.dashuyun.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tgt.sysykeji.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qqc.fengsongda.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xgs.yongpay.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nda.haohaochexian.top

[D25] Set 集合去重与交并差
来源：http://yzh.daxiang520.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gyz.iojbl.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hzs.xingfuxueyuan.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jdd.zhiwuduotai.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xte.bjfxy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hda.xylfe.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lce.wangshuangyany.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ljx.mhx1999.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://apv.zhixingplan.top

[D26] 数组转字符串
来源：http://tij.9152youxi.cn

Py:   ", ".join(map(str, arr))
来源：http://ugt.guowangkeji.top

PHP:  implode(", ", $arr);
来源：http://isv.xuanzx.com

JS:   arr.join(", ")
来源：http://slr.zhijiandao.cn

TS:   arr.join(", ")
来源：http://ygy.jyoumei.cn

Java: String.join(", ", list)
来源：http://nwa.fengsongda.top

Go:   strings.Join(strs, ", ")
来源：http://bsq.daxiang520.top

Ruby: arr.join(", ")
来源：http://ynl.sufxvd.cn

C#:   string.Join(", ", list)
来源：http://kdl.gotoacloud.top

================================================================================
来源：http://asz.svipenyu.cn

E. 字符串处理
来源：http://hwi.sufxvd.cn

================================================================================
来源：http://pdl.xylfe.cn

[E01] 拼接字符串
来源：http://oof.smart0.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vje.epnwcf.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ncd.xziqi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://llr.yangfankeji.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vgy.ehwqpu.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ncw.guannengcc.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qgp.yj20258888.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zae.xziqi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hbq.ppjwa.cn

[E02] 重复字符串
来源：http://brl.epnwcf.com

Py:   "ab" * 3
来源：http://pzz.ehwqpu.com

PHP:  str_repeat("ab", 3);
来源：http://jyq.kuanghao11.cn

JS:   "ab".repeat(3)
来源：http://fpa.yfazqb.com

TS:   "ab".repeat(3)
来源：http://dby.birdmap.top

Java: "ab".repeat(3)
来源：http://cfa.jqgfzy.top

Go:   strings.Repeat("ab", 3)
来源：http://hns.sjlbkw.cn

Ruby: "ab" * 3
来源：http://zel.xinyue.icu

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kup.gotoacloud.top

[E03] 截取子串
来源：http://wwa.daxiang520.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vzk.hammf.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xoo.ywan-chungtsiang.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bqh.cqqwz.cn

TS:   s.slice(1, 4)
来源：http://tqy.hnqzz.top

Java: s.substring(1, 4)
来源：http://nbi.sjlbkw.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rae.shangyingyoupin.top

Ruby: s[1, 3];  s[1..3]
来源：http://oam.nwbrower.top

C#:   s.Substring(1, 3)
来源：http://giq.nanxuanxn.top

[E04] 查找子串位置
来源：http://mvv.birdmap.top

Py:   s.find("x");  s.index("x")
来源：http://juz.daxiang520.top

PHP:  strpos($s, "x");
来源：http://ofu.xuanzx.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://uyi.nwbrower.top

TS:   s.indexOf("x")
来源：http://vkh.yonumen.top

Java: s.indexOf("x")
来源：http://ant.cucudq.cn

Go:   strings.Index(s, "x")
来源：http://iav.sufxvd.cn

Ruby: s.index("x")
来源：http://eha.ywan-chungtsiang.top

C#:   s.IndexOf("x")
来源：http://lmr.nanxuanxn.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://koe.fzhhl.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xqw.shzxlz.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xau.zycfv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://smj.quarkkingdee.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://szw.nanxinkj.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://odx.shanyushiyangtech.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sxw.hongshengwenyu.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zrx.ctjpmb.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://psf.snrcjt.cn

[E06] 替换子串
来源：http://get.andypj.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qno.jqgfzy.top

PHP:  str_replace("a", "b", $s);
来源：http://ukj.andypj.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hhy.yanxiufei.cn

TS:   s.replaceAll("a", "b")
来源：http://jvl.shangyingyoupin.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wtk.guannengcc.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://aol.yongpay.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hvp.fengsongda.top

C#:   s.Replace("a", "b")
来源：http://ydl.xinyue.icu

[E07] 按分隔符拆分
来源：http://gka.zdbjq.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lcb.yonumen.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xuv.ppjwa.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://fyc.hnxiangtu.top

TS:   s.split(",")
来源：http://anh.shuidangran.top

Java: s.split(",");  s.split("\\s+")
来源：http://ryo.yuxming.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ybm.0kj1m.cn

Ruby: s.split(",");  s.split
来源：http://oza.vehdjk.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://esu.jinqigfzy.top

[E08] 数组按分隔符合并
来源：http://uar.tian-w.cn

Py:   ",".join(items)
来源：http://znd.meibo888.top

PHP:  implode(",", $items);
来源：http://prq.jqgufenzy.top

JS:   items.join(",")
来源：http://lhm.yueranfly.top

TS:   items.join(",")
来源：http://tvp.hongshengwenyu.top

Java: String.join(",", items)
来源：http://oci.quarkkingdee.top

Go:   strings.Join(items, ",")
来源：http://ddv.nanxuanxn.top

Ruby: items.join(",")
来源：http://unf.vqdsnc.cn

C#:   string.Join(",", items)
来源：http://toh.epnwcf.com

[E09] 去除所有空白字符
来源：http://rqn.ppjwa.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mbj.cucudq.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qgz.ppjwa.cn

JS:   s.replace(/\s+/g, "")
来源：http://hsx.ehwqpu.com

TS:   s.replace(/\s+/g, "")
来源：http://xxe.jqgufenzy.top

Java: s.replaceAll("\\s+", "")
来源：http://wae.cheryme.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://hap.shanyushiyangkeji.top

Ruby: s.gsub(/\s+/, "")
来源：http://yyc.jinyuanbaomall.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://eop.daria6918.cn

[E10] 左侧补零 / 定长填充
来源：http://ybw.hfpthk.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mqf.cashguo.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tol.fzhhl.top

JS:   "7".padStart(3, "0")
来源：http://ypp.yvedp.cn

TS:   "7".padStart(3, "0")
来源：http://hfy.zhixingplan.top

Java: String.format("%03d", 7)
来源：http://exk.yonumen.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://gtv.yj202588.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lcl.hcnkem.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lae.cashguo.top

[E11] 反转字符串
来源：http://mfg.hfpthk.cn

Py:   s[::-1]
来源：http://zkv.zycfv.cn

PHP:  strrev($s);
来源：http://zlz.snrcjt.cn

JS:   [...s].reverse().join("")
来源：http://dvr.zhixingplan.top

TS:   [...s].reverse().join("")
来源：http://roh.shanyushiyangtech.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ljh.jinyuanbaomall.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://uwx.ivvv.top

Ruby: s.reverse
来源：http://rcj.jyoumei.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xsc.gogol.net.cn

[E12] 统计某字符出现次数
来源：http://yej.cheryme.top

Py:   s.count("a")
来源：http://oun.pengpengdd.cyou

PHP:  substr_count($s, "a");
来源：http://fzp.shuidangran.top

JS:   s.split("a").length - 1
来源：http://vpt.ppjwa.cn

TS:   s.split("a").length - 1
来源：http://lma.yfazqb.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wqf.fanxiaobao.xyz

Go:   strings.Count(s, "a")
来源：http://xrd.zhengqikj.top

Ruby: s.count("a")
来源：http://bdg.uphjek.com

C#:   s.Count(c => c == 'a')
来源：http://uzb.hnxiangtu.top

[E13] 逐字符遍历
来源：http://moc.zhengqikj.top

Py:   for ch in s: print(ch)
来源：http://bbb.quarkkingdee.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://frf.fanxiaobao.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://lhg.mhx1999.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ftz.316326.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fkz.bbcook.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tci.zhongyouzk.top

Ruby: s.each_char { |ch| puts ch }
来源：http://cyk.52xcode.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fiv.bjfxy.top

[E14] URL 编码与 Base64
来源：http://aca.sysykeji.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cnz.ywan-chungtsiang.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://dah.yvedp.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dad.quarkkingdee.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rcm.zhixingplan.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wdr.gotoacloud.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pzm.guannengcc.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wvk.vqdsnc.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xmg.fehbvm.com

[E15] HTML 转义 / 反转义
来源：http://qxz.xingfuxueyuan.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://xiv.pycfn.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tta.jinyuanbaomall.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hup.guowangkeji.top

TS:   // 同上，务必做 XSS 过滤
来源：http://pkv.uphjek.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cwg.hnqzz.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rvb.zhengqikj.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dyj.nanxuanxn.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vxa.yanxiufei.cn

[E16] 数字千分位
来源：http://shg.quarkkingdee.top

Py:   f"{1234567:,}"
来源：http://nbu.gaohongyu789.top

PHP:  number_format(1234567);
来源：http://eop.hongshengwenyu.top

JS:   (1234567).toLocaleString("en-US")
来源：http://gql.sufxvd.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ihb.hfpthk.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://svi.shuidangran.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rqa.yuxming.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dtk.meibo888.top

C#:   1234567.ToString("N0")
来源：http://xlh.yangfankeji.com

[E17] 首字母大写
来源：http://yel.jinyuanbaomall.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rzc.yuanzhike.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://mjy.haohaochexian.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eyz.zycfv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rvb.wangshuangyany.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zbu.jlsjyb.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bfb.nanxinkj.top

Ruby: s.capitalize
来源：http://jvf.yj20258888.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ayb.tian-w.cn

[E18] 模板占位符替换
来源：http://glf.iojbl.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gdm.yj20258888.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cbc.vehdjk.com

JS:   tpl.replaceAll("{name}", name)
来源：http://ovm.feifeiyinyue.top

TS:   tpl.replaceAll("{name}", name)
来源：http://yev.zhaomingkeji.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gas.iojbl.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nde.gzhubu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nif.zdqjudy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yvf.snrcjt.cn

[E19] 多行文本按行拆分
来源：http://ieb.zhaomingkeji.xyz

Py:   s.splitlines()
来源：http://lph.vehdjk.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://uul.yuanzhike.top

JS:   s.split(/\r?\n/)
来源：http://dkx.zdqjudy.top

TS:   s.split(/\r?\n/)
来源：http://kok.shanyushiyangkeji.top

Java: s.lines().toList()
来源：http://ddy.vehdjk.com

Go:   strings.Split(s, "\n")
来源：http://cen.ydzc1.top


<!-- 参考信息 -->
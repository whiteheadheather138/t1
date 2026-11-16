代发 wailian999

Ruby: arr.index(x)
来源：http://pth.shanyushiyangtech.top

C#:   list.IndexOf(x);
来源：http://fdf.zhixingplan.top

[D13] 过滤（保留满足条件的）
来源：http://thl.ppjwa.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qtw.52xcode.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://piy.wangshuangyany.cn

JS:   arr.filter(x => x > 3)
来源：http://vsq.zhengqikj.top

TS:   arr.filter(x => x > 3)
来源：http://yel.chenzaomai.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tml.hongshengwenyu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nax.zhoulong.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://srm.bjfxy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://myk.yonumen.top

[D14] 映射转换（每个元素变形）
来源：http://vxj.zhaomingkeji.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nnz.iojbl.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bke.dashuyun.cn

JS:   arr.map(x => x * 2)
来源：http://pct.cashguo.top

TS:   arr.map(x => x * 2)
来源：http://cvc.jinyuanbaomall.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://eqa.zhongyouzk.top

Go:   // 手写循环
来源：http://tfd.jiagoushi.top

Ruby: arr.map { |x| x * 2 }
来源：http://qtt.cheryme.top

C#:   list.Select(x => x * 2).ToList()
来源：http://spp.guannengcc.top

[D15] 去重
来源：http://hgp.yongpay.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rci.cqqwz.cn

PHP:  array_unique($arr);
来源：http://xeb.316326.xyz

JS:   [...new Set(arr)]
来源：http://ldf.uphjek.com

TS:   [...new Set(arr)]
来源：http://vcc.zhixingplan.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wvm.9152youxi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wln.bjfxy.top

Ruby: arr.uniq
来源：http://xfv.hnxiangtu.top

C#:   list.Distinct().ToList()
来源：http://lye.zycfv.cn

[D16] 求和与平均值
来源：http://wis.sxryk.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zed.mhx1999.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rql.pycfn.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rov.ppjwa.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mrz.jqgfzy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yol.cdnleiting.top

Go:   // 手写循环累加
来源：http://nkn.pycfn.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zte.xingfuxueyuan.xyz

C#:   list.Sum();  list.Average()
来源：http://jyt.meibo888.top

[D17] 最大值与最小值
来源：http://mxs.shuidangran.top

Py:   max(arr);  min(arr)
来源：http://nbw.jinghuilouyu.cn

PHP:  max($arr);  min($arr);
来源：http://avr.shzxlz.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tjq.xingfuxueyuan.xyz

TS:   Math.max(...arr);
来源：http://jlk.yj20258.top

Java: Collections.max(list);  Collections.min(list);
来源：http://mdf.ybcxt.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://puu.bbcook.cn

Ruby: arr.max;  arr.min
来源：http://ckx.bjfxy.top

C#:   list.Max();  list.Min()
来源：http://qjv.yuxming.cn

[D18] 扁平化嵌套数组
来源：http://jsr.shangyingyoupin.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rtg.yj20258.top

PHP:  array_merge(...$nested);
来源：http://bng.yj202588.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://eze.yongpay.top

TS:   nested.flat();
来源：http://nup.yj202588.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://oav.c1oappe.top

Go:   // 手写双层循环
来源：http://mzf.gotoacloud.top

Ruby: nested.flatten
来源：http://veh.epnwcf.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://bbj.xuetiantiany.cn

[D19] 按字段分组
来源：http://ocu.hesvh.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://olv.gogol.net.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vdd.aibaodan.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ncw.yangfankeji.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://rnh.yuanzhike.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://znj.zhijiandao.cn

Go:   // 手写 map[string][]T
来源：http://iab.zycfv.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://qbn.yj20258.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yya.smart0.xyz

[D20] 统计每个元素出现次数
来源：http://glf.svipenyu.cn

Py:   Counter(arr)
来源：http://pef.jqgufenzy.top

PHP:  array_count_values($arr);
来源：http://mwj.gaohongyu789.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zyz.guannengcc.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pfa.nanxinkj.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wms.yuxming.cn

Go:   // 手写 map[T]int
来源：http://try.jinghuilouyu.cn

Ruby: arr.tally
来源：http://oxq.tanke756.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://aej.fehbvm.com

[D21] 判断是否包含某元素
来源：http://huz.shangyingyoupin.top

Py:   x in arr
来源：http://lfe.sweek.top

PHP:  in_array($x, $arr, true);
来源：http://pjb.jiagoushi.top

JS:   arr.includes(x)
来源：http://uji.cucudq.cn

TS:   arr.includes(x)
来源：http://wyx.hywenlv.cn

Java: list.contains(x)
来源：http://opq.ybcxt.top

Go:   slices.Contains(arr, x)
来源：http://hsb.ivvv.top

Ruby: arr.include?(x)
来源：http://tbn.snrcjt.cn

C#:   list.Contains(x)
来源：http://cww.cucudq.cn

[D22] 复制数组（避免共享引用）
来源：http://sjh.andypj.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nzz.zhijiandao.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yyo.aizwys.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mim.gogol.net.cn

TS:   [...arr];
来源：http://wzh.hnqzz.top

Java: new ArrayList<>(list);
来源：http://obn.zhengqikj.top

Go:   copied := append([]int(nil), arr...)
来源：http://csy.gzhubu.top

Ruby: arr.dup;  arr.clone
来源：http://htp.guowangkeji.top

C#:   new List<int>(list);
来源：http://uvh.yj20258888.top

[D23] reduce 累积计算
来源：http://cog.jinghuilouyu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gkm.zhongyouzk.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rkj.sxryk.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qrc.sxryk.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zxx.ydjk.org.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://vjy.nwbrower.top

Go:   // 手写循环
来源：http://hhu.jyoumei.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jfi.andypj.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zvs.xziqi.cn

[D24] 字典 / Map 基本操作
来源：http://uiu.fengsongda.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cdi.cdnleiting.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ztv.pengpengdd.cyou

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hwd.aibaodan.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lue.tarul.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ttk.c1oappe.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vkl.jqgfzy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rng.bbcook.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xof.yj202588.top

[D25] Set 集合去重与交并差
来源：http://kkc.sufxvd.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://frk.chenlongwang.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rdl.haohaochexian.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gfs.hfpthk.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://oxg.hysaishi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cqg.epnwcf.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://iev.jinqigfzy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gta.meibo888.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xlh.zhixingplan.top

[D26] 数组转字符串
来源：http://aia.dashuyun.cn

Py:   ", ".join(map(str, arr))
来源：http://irt.shanyushiyangtech.top

PHP:  implode(", ", $arr);
来源：http://zyo.zhixingplan.top

JS:   arr.join(", ")
来源：http://gyv.xylfe.cn

TS:   arr.join(", ")
来源：http://mpx.jinghuilouyu.cn

Java: String.join(", ", list)
来源：http://jee.xylfe.cn

Go:   strings.Join(strs, ", ")
来源：http://mda.hnqzz.top

Ruby: arr.join(", ")
来源：http://coj.quarkkingdee.top

C#:   string.Join(", ", list)
来源：http://dvt.quarkkingdee.top

================================================================================
来源：http://ttu.ivvv.top

E. 字符串处理
来源：http://clf.hysaishi.cn

================================================================================
来源：http://uyr.sweek.top

[E01] 拼接字符串
来源：http://vaa.zdbjq.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jcy.hfpthk.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pwc.zhixingplan.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nlj.shanyushiyangtech.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bob.pengpengdd.cyou

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://thn.quarkkingdee.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mlo.feifeiyinyue.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nmo.hesvh.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ofy.yangfankeji.com

[E02] 重复字符串
来源：http://dpo.ppjwa.cn

Py:   "ab" * 3
来源：http://mjo.yuxming.cn

PHP:  str_repeat("ab", 3);
来源：http://bnq.shanyushiyangkeji.top

JS:   "ab".repeat(3)
来源：http://okf.cqqwz.cn

TS:   "ab".repeat(3)
来源：http://fkp.chenzaomai.com

Java: "ab".repeat(3)
来源：http://fhv.jianghu66.top

Go:   strings.Repeat("ab", 3)
来源：http://zhy.sysykeji.top

Ruby: "ab" * 3
来源：http://tni.yj20258.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cis.ywan-chungtsiang.top

[E03] 截取子串
来源：http://cif.yangfankeji.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ulj.chenjidiqi.icu

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jmp.tanke756.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lvu.gaohongyu789.top

TS:   s.slice(1, 4)
来源：http://dpr.gzhubu.top

Java: s.substring(1, 4)
来源：http://eox.shuidangran.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fuj.fzhhl.top

Ruby: s[1, 3];  s[1..3]
来源：http://mwt.yuxming.cn

C#:   s.Substring(1, 3)
来源：http://hkw.hnxiangtu.top

[E04] 查找子串位置
来源：http://glj.dashuyun.cn

Py:   s.find("x");  s.index("x")
来源：http://ymn.kuanghao11.cn

PHP:  strpos($s, "x");
来源：http://zsk.ydzc1.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://udr.yangfankeji.com

TS:   s.indexOf("x")
来源：http://hax.chenjidiqi.icu

Java: s.indexOf("x")
来源：http://ioi.smart0.xyz

Go:   strings.Index(s, "x")
来源：http://izm.zycfv.cn

Ruby: s.index("x")
来源：http://gxj.wangdashe.top

C#:   s.IndexOf("x")
来源：http://tzb.havefunace.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://vwj.hammf.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hio.xuanzx.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tdl.shuidangran.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xch.snrcjt.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://onv.nanxuanxn.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ceq.shzxlz.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hta.yj202588.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lom.jinqigfzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dhd.cucudq.cn

[E06] 替换子串
来源：http://ydg.meibo888.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bgy.nanxuanxn.top

PHP:  str_replace("a", "b", $s);
来源：http://xam.jinghuilouyu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vpw.52xcode.cn

TS:   s.replaceAll("a", "b")
来源：http://ici.0kj1m.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pdm.ctjpmb.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dxv.sjlbkw.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://aeh.sxryk.cn

C#:   s.Replace("a", "b")
来源：http://cwq.cheryme.top

[E07] 按分隔符拆分
来源：http://noy.guowangkeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jyw.guannengcc.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rhd.cqqwz.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qrn.jinghuilouyu.cn

TS:   s.split(",")
来源：http://ctr.bbcook.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ntw.zhaomingkeji.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://omw.zhiwuduotai.top

Ruby: s.split(",");  s.split
来源：http://gtt.andypj.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tvv.hnqzz.top

[E08] 数组按分隔符合并
来源：http://nyn.chenlongwang.top

Py:   ",".join(items)
来源：http://ple.dashuyun.cn

PHP:  implode(",", $items);
来源：http://spo.shzxlz.cn

JS:   items.join(",")
来源：http://sqv.cheryme.top

TS:   items.join(",")
来源：http://byh.wangdashe.top

Java: String.join(",", items)
来源：http://dun.aizwys.cn

Go:   strings.Join(items, ",")
来源：http://ltf.cqqwz.cn

Ruby: items.join(",")
来源：http://zhp.fengsongda.top

C#:   string.Join(",", items)
来源：http://ngg.fzhhl.top

[E09] 去除所有空白字符
来源：http://tgd.pycfn.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://goo.gotoacloud.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kgz.gzhubu.top

JS:   s.replace(/\s+/g, "")
来源：http://ccl.nanxinkj.top

TS:   s.replace(/\s+/g, "")
来源：http://mli.zhijiandao.cn

Java: s.replaceAll("\\s+", "")
来源：http://sid.yuanzhike.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://baj.pengpengdd.cyou

Ruby: s.gsub(/\s+/, "")
来源：http://yne.sxryk.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cvh.hammf.cn

[E10] 左侧补零 / 定长填充
来源：http://jmh.jinqigufen.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gep.mhx1999.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zhc.hfpthk.cn

JS:   "7".padStart(3, "0")
来源：http://mjw.dashuyun.cn

TS:   "7".padStart(3, "0")
来源：http://oaf.hammf.cn

Java: String.format("%03d", 7)
来源：http://yaq.gotoacloud.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://tld.hammf.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://plp.ehwqpu.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://eox.cqqwz.cn

[E11] 反转字符串
来源：http://cdl.tanke756.top

Py:   s[::-1]
来源：http://hbm.nwbrower.top

PHP:  strrev($s);
来源：http://wlu.gaohongyu789.top

JS:   [...s].reverse().join("")
来源：http://hwx.tianlin.xyz

TS:   [...s].reverse().join("")
来源：http://epe.yj20258.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ixw.zdqjudy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://jxw.zhongyouzk.top

Ruby: s.reverse
来源：http://rrd.ybcxt.top

C#:   new string(s.Reverse().ToArray())
来源：http://lls.shanyushiyangtech.top

[E12] 统计某字符出现次数
来源：http://dcr.shangyingyoupin.top

Py:   s.count("a")
来源：http://tiw.yfazqb.com

PHP:  substr_count($s, "a");
来源：http://kiw.hysaishi.cn

JS:   s.split("a").length - 1
来源：http://btu.gaohongyu789.top

TS:   s.split("a").length - 1
来源：http://wyq.zhoulong.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://sny.xylfe.cn

Go:   strings.Count(s, "a")
来源：http://pny.tianlin.xyz

Ruby: s.count("a")
来源：http://hme.hcnkem.com

C#:   s.Count(c => c == 'a')
来源：http://iry.yuanzhike.top

[E13] 逐字符遍历
来源：http://oml.shzxlz.cn

Py:   for ch in s: print(ch)
来源：http://gbs.jyoumei.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zzt.fanxiaobao.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://zlt.ybcxt.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://tdz.316326.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hwc.chenlongwang.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://spl.zhijiandao.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://psc.9152youxi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://idk.ywan-chungtsiang.top

[E14] URL 编码与 Base64
来源：http://eab.bjfxy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bsk.haohaochexian.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://nly.aizwys.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://afb.c1oappe.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nna.yuanzhike.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hwf.feifeiyinyue.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ngm.hesvh.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lxv.zhoulong.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tgw.hcnkem.com

[E15] HTML 转义 / 反转义
来源：http://lho.nwbrower.top

Py:   html.escape(s);  html.unescape(s)
来源：http://kbw.vqdsnc.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jek.zdbjq.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gge.shzxlz.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://gxr.gotoacloud.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fva.yongpay.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zhq.nanxuanxn.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hlv.gzhubu.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vho.yonumen.top

[E16] 数字千分位
来源：http://yxq.zhixingplan.top

Py:   f"{1234567:,}"
来源：http://omm.daria6918.cn

PHP:  number_format(1234567);
来源：http://vag.zdqjudy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://fvo.ywan-chungtsiang.top

TS:   (1234567).toLocaleString("en-US")
来源：http://gzh.hcnkem.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://msy.fktsv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mww.hfpthk.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://smu.jqgufenzy.top

C#:   1234567.ToString("N0")
来源：http://ulv.cashguo.top

[E17] 首字母大写
来源：http://gle.iojbl.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tpc.tarul.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://tmb.chenlongwang.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fbw.cashguo.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wzj.xinyue.icu

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tcd.sweek.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mud.xylfe.cn

Ruby: s.capitalize
来源：http://xjm.zhaomingkeji.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://haj.shangyingyoupin.top

[E18] 模板占位符替换
来源：http://cte.sysykeji.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://obv.zhiwuduotai.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lls.ppjwa.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://yaf.haohaochexian.top

TS:   tpl.replaceAll("{name}", name)
来源：http://oja.zdbjq.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wmg.zhaomingkeji.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jae.jiagoushi.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kpk.tian-w.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rny.yanxiufei.cn

[E19] 多行文本按行拆分
来源：http://kgt.epnwcf.com

Py:   s.splitlines()
来源：http://swo.chenlongwang.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://isu.hnxiangtu.top

JS:   s.split(/\r?\n/)
来源：http://eqh.fanxiaobao.xyz

TS:   s.split(/\r?\n/)
来源：http://szg.cheryme.top

Java: s.lines().toList()
来源：http://tgm.jinyuanbaomall.cn

Go:   strings.Split(s, "\n")
来源：http://gsq.chenzaomai.com


<!-- 参考信息 -->